---
title: "205_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_165156f7936d61a0ebe95e2fc87e92f57295230462135641
file_size: 449900
---

## Towards an FA ChatBot with   Retrieval-augmented Language Modeling  

Maik Fichtenkamm 1,3 , Markus Kofler 2,3 , Konstantin Schekotihin 3 , Christian Burmer 1  1 Infineon Technologies, Siemensstr. 2, 9500 Villach, Austria  2 Infineon Technologies, BO5 Lakeside, 9020 Klagenfurt, Austria  3 University Klagenfurt, Universitätsstr. 65-67, 9020 Klagenfurt, Austria  Email : firstname.lastname@infineon.com, konstantin.schekotihin@aau.at

Abstract —Failure Analysis (FA) data storages, like  databases or file shares, host a lot of textual data comprising  important information about products, best practices, or past  cases. FA engineers require this information at their  fingertips to accomplish their tasks efficiently. However,  common keyword search interfaces provided by most  information systems and databases are insufficient as they  force an engineer to formulate a correct query, read returned  documents, and manually extract required knowledge from  them. In this paper, we suggest a cost-effective approach that  augments retrieval systems with the capabilities of modern  Large Language Models (LLMs) to provide straight-to-point  answers to engineers’ questions. Preliminary evaluation  shows that the suggested system can generate high-quality  responses to a set of simple benchmark queries but also lacks  complex reasoning capabilities for answering complex  queries.

Keywords—AI, generative models, retrieval-augmented  generation

## I.    I NTRODUCTION 

The process of detecting and locating semiconductor  failures is a challenging and labor-intensive task that  requires an FA engineer to have quick access to relevant  information about past jobs, used technologies, and best  practices. However, existing information systems often  store this knowledge in the form of text documents, making  it difficult to find and access using existing methods, such  as keyword-based search. As a result, engineers must  manually query multiple systems to find, merge, and  analyze relevant information to determine its usefulness for  the current job.

Recent advances in Natural Language Processing (NLP)  have shown that it can be a valuable tool in solving the FA  information search problem [1, 2]. Automated query  answering using LLMs is one of the most recent and  emerging applications of NLP. These generative models are  trained on huge text corpora and can give answers to various  general questions, summarize/rewrite provided texts, or  solve simple mathematical problems. However, when used  in domain-specific scenarios, like FA labs, the performance  of LLMs may drop significantly since the proportion of  texts relevant to the target domain in the training corpora  might be very small. Retraining these models on FA data is  problematic since there are no sufficiently large datasets  comprising FA texts, and the computation power available  for training on companies’ infrastructures is limited.

Therefore, we suggest a novel Retrieval-augmented  Language Modeling (RALM) 1  that exploits the zero-shot  learning capabilities of modern LLMs to condition their  output towards the application domain. The latter can be  achieved by extending user queries with domain-specific  data available in FA information systems. This paper  applied simple and cost-effective RALM approaches to  avoid high computational and dataset labeling costs.  Evaluation results indicate that correctly selected FA texts,  together with their careful integration with the query, allow  for the generation of high-quality answers and enable  scalable development of chatbots in the FA domain.

## II.    B ACKGROUND 

Recent advances in Large Language models (LLM) such  as ChatGPT led to a significant increase in their capabilities,  demonstrated by their remarkable achievement in machinegenerated texts across various domains. Despite these  successes, LLMs exhibit limitations, especially in domainspecific question answering. LLMs tend to generate  inaccuracies or even completely incorrect answers, known  as hallucinations [3], and cannot consider the latest data,  which was not available during the training process [4, 5].  Fine-tuning an LLM for FA-specific tasks requires  substantial computational resources and large volumes of  high-quality training data representing interactions of FA  engineers with Chatbots. At the moment, neither is available  in many FA labs.

Retrieval-Augmented Language Modelling (RALM)  aims to enhance the performance of LLMs by incorporating  data from external data stores into the generation process.  Grounding LLMs on relevant documents leads to higher  accuracy of generated answers [6], accommodates temporal  changes in data [5], and increases interpretability by  allowing users to trace outputs to specific data sources [7].

A general RALM approach consists of three high-level  components [7]:

•    Retrieval  focuses on efficiently and accurately  extracting (parts of) documents relevant to a given  query from available data sources. Depending on the  type of external source used, this process might  require different retrieval strategies.

•    Augmentation  of the user query with the retrieved  data aims to create a new prompt, providing LLM  with examples and explanations it can use to answer  the query. Augmentation strategies can be applied at

different stages of RALM, and various data  integration methods can be used.

•    Generation  of consistent texts given one or a  sequence of augmented user queries, depending on  the augmentation and/or strategies implemented in  the approach.

RALM research provides answers to fundamental  questions arising during the implementation of the phases  discussed above, like what data, how, and when must be  retrieved to provide the most valuable information for the  LLM. Fig. 1 depicts distinguishing features for a  classification of RALM approaches.

![Structures   Pre-training  Chunks   Fine-tuning  Tokens   Whatto   Atwhich   Inference  retrieve?   stage?  RALM  Whereto   Features   whento  Input   >One-time  augment?   retrieve?  Intermediate   Iterative  Output   Adaptive  Howto  design?  Naive   Modular  Advanced  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/94777653-0f85-4f80-affa-521076a30017/94777653-0f85-4f80-affa-521076a30017.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215889%3B1743219489&q-key-time=1743215889%3B1743219489&q-header-list=host&q-url-param-list=&q-signature=915ce148c4d8f759e43be3447f67fe535915e16a)
Fig.1   Classification of RALM methods

Retrieval techniques  must determine what data must be  selected and progressed from extracting simple tokens  (units of text) to chunks (sequences of tokens) over to  complex structures such as entities. The exploration of when  to retrieve has resulted in the development of three main  strategies:  single , which retrieves data only once for a query;  adaptive , which can do (multiple) retrievals based on  specific demand; and   iterative , which continuously

improves the state of the data with various queries.  Addressing the question of how to use retrieved data  initiated the development of multiple approaches integrating  the data into the input, intermediate, or output layers of an  LLM [8].

Additionally,   various   methodologies   exist   for  incorporating retrieved data  into the LLM component of a  RALM system. Researchers differentiate between three  central integration stages. First, retrieved documents can be  embedded at the  pre-training  stage of an LLM, resulting in  superior performance in knowledge-intensive tasks, albeit  requiring extensive datasets and significant computational  resources. Second,  fine-tuning  RALM techniques aims to  enhance the retriever or generator components to align their  outputs in a customized manner, resulting in enhanced  capabilities of the LLM. However, fine-tuning demands  specialized datasets and increased computational resources.  Finally, the most cost-effective RALM systems rely on  zero-shot learning that directly integrates retrieved  knowledge into the prompt in a way that can enhance the  inference  performance of LLMs.

From the architecture perspective, RALM designs can  be classified into three types: naïve, advanced, and modular.  The  naïve RALM   systems  are the simplest ones, requiring  any external data to be converted into standardized text to  facilitate subsequent processing by retrieving and  generating LLM components. The text is segmented into  chunks and transformed into vector representations via a  retrieval model. These representations are stored in a vector  database, and each chunk is associated with an index to  boost efficient search operations. During retrieval, a user's  input query is translated into a vector representation using  an embedding model, enabling the identification of relevant  chunks based on a similarity score. Subsequently, the  identified chunks are integrated into the original question,  and the LLM generates an appropriate response [7].  Advanced RALM approaches  enhance retrieval quality by

![Query  What kind  of physical failure is  characterized bya Pin Short in the  latestreports?   FA Engineer  Answer  WithRALM  Retrieval   Augmentation   Generation   Based on the reports provided,a  pin short ischaracterizedbya  QueryAPI   phyiscal failure called EIPD,  whichis   observed   afer  Prompt   decapsulation.  enhancer   WithoutRALM   MN  LLM   VectorDB   LLM   A pin short is a type of physical  Embeddings   Generator   failure. It happens whena  conductive pathiscreated  between two pins that should  not be connected. This can  Relevant Documents   Rewritten Query   occurduetoavarietyofreasons  Chunk1:Themeasured shortsatVCC are   Question:What kind of physical  due to themassiveEIPD damage observed   failure ischaracterized by a pin short  after decapsulation.   in thelatest reports?  Chunk2:The eletrical signature of the  measured shortsisPinShort   Chunk 1:The measured.  Chunk 3:The physicalfailure of the   Chunk 2:The electrical...  measured shorts is EIPD   Chunk 3:The physical...  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/17bc11b8-7c7f-4422-9bc4-100d74856cab/17bc11b8-7c7f-4422-9bc4-100d74856cab.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215889%3B1743219489&q-key-time=1743215889%3B1743219489&q-header-list=host&q-url-param-list=&q-signature=6a5875792e1dd60ba85ca76c31aba0d1dde1bb77)
Fig. 2.  RALM architecture for FA. Example outputs have been generated using an internal ChatGPT 3.5 instance.

![Training  Documents   FAData  Pre-   Qdrant  FAjobs   Storage  Vector  processing  Databases   Crawler  DB  Vvikis  ElasticDB   LLN  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e5880453-efae-4767-a2ac-c9d5f26f4fd4/e5880453-efae-4767-a2ac-c9d5f26f4fd4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215889%3B1743219489&q-key-time=1743215889%3B1743219489&q-header-list=host&q-url-param-list=&q-signature=4cd57e14b7419ebd5d8a231563d3a02a3d7ed887)
Fig. 3. FA Indexing Process

implementing pre-retrieval and post-retrieval strategies.  These techniques encompass optimized indexing, finetuning text-to-vector embeddings generated by retrieval  models, re-ranking retrieved documents based on their  significance, and compressing the obtained information.  Finally, a  modular RALM framework  aspires to introduce  flexibility by employing sophisticated techniques tailored to  address specific challenges. The approach introduces the  development of serialized pipelines and end-to-end training  methodologies, incorporating multiple interconnected  modules [7].

## III.   M ETHODOLOGY 

This paper suggests variants of naïve and advanced  RALM for FA, whose general architecture is shown in Fig.  2. The design adheres to the previously discussed RALM  framework and incorporates Data, Retrieval, Augmentation,  and Generation modules. All its subcomponents can be  realized in a cost-effective and scalable manner.

## A.   Data  

## 1)    FA Benchmark  

A preliminary survey revealed that there are two  prominent use cases for question answering in FA:

•    Specific-sample  question answering encompasses  information and questions related to a specific  analysis or given sample, i.e . I have to perform an  analysis for a device failing with a given error  pattern. What is the analysis’s next step?

•    General knowledge  question answering targets to  summarize available know-how, such as  What is the  latest state of fault localization using solid  immersion lenses?

An initial dataset was compiled to facilitate the  assessment of RALM pipelines for these scenarios. The  dataset contains sample queries from FA engineers, with a  total of 20 questions spanning five categories:

•    Next-step prediction  addresses questions related to  the subsequent process steps or method selection for  an active FA analysis.  •    Related information identification   refers to  finding similar defects, products, and failure analysis  for the specifications.  •    Failure mode identification   includes specific  questions about failure modes and error types.  •    Safety verification  questions relate to checking the  settings of a device for a laboratory test.

•    Default knowledge retrieval  is the base category if  a question does not fit into the previously introduced  categories.

## 2)    FA Data  

To facilitate effective data retrieval, Fig. 3 depicts  deploying a vector database via an FA indexing process.  Various support systems used in FA provide a wealth of  structured and unstructured data sources, such as databases,  wikis, and file shares. The structured FA data relates to  specific FA jobs within Infineon, tracked in the internal  software system  iFAct.  This data includes analysis results,  information about the examined sample, laboratory test  data, and metadata. Unstructured data exists in a textual  form, such as presentations, articles, and research papers.  An FA storage crawler systematically traverses and indexes  these data, creating over 9 million records in an Elastic  database.

The subsequent preprocessing steps depend on whether  the data is from  iFAct  or unstructured sources.  iFAct  data,  comprising over 87 different features, is extracted from the  Elastic database in JSON format. Of these features, 32 are  deemed significant by FA experts for semantic search.  Additionally,   deduplication   and   irrelevant   feature  elimination are performed. To keep coherent text blocks  together, the FA data structure necessitates segmenting  JSON dictionaries into chunks of size 512 by a custom  JSON splitter. Unstructured data undergoes intensive  cleaning, including removing duplicates, unnecessary  whitespaces, bullet points, and special ASCII characters.  The textual data is then segmented into chunks of size 512  with a standard text splitter.

Subsequently, the embedding model  bge-base-en-v1.5 is employed to generate embeddings of the data chunks.  Finally, the generated embeddings are loaded into a  Qdrant vector database for further processing. Initially, only  iFAct  job data was integrated into the vector database, with  unstructured data added later.

## B.   Retrieval  

A query API provides an interface for retrieving relevant  data for a query. First, an LLM generates a vector  embedding of the query and sends it to the vector database.  The vector database includes the functionality to return the  top   $k$   relevant data chunks for a given embedding vector  based on a cosine similarity search. The response is returned  to the augmentation component.

## C.   Augmentation  

During augmentation, a prompt enhancer combines the  initial query with the retrieved context by a predefined  prompt template, considered a naïve RALM. The prompt  template includes instructions for the LLM generator  regarding   the   context,   the   format,   and   the

comprehensiveness of the expected answer. Then, the  combined prompt is sent to the LLM generator.

Research indicates that additional processing of  retrieved documents can mitigate challenges such as  exceeding the context length of LLM generators, noise of  retrieved documents, and providing irrelevant information  [7]. Therefore, we tested various  re-ranker models  to locate  the relevant information on the edges of a prompt and  eliminate unnecessary information:

•    Reordering  re-rankers use the fact that RALM  pipelines perform best when the most significant  retrieved data is positioned at the start or end of a  prompt. A reordering re-ranker rearranges retrieved  documents based on their similarity score at the  start or end of the prompt template. [9]

•    Semantic  re-rankers measure the similarity between  the query and retrieved documents leveraging  specialized re-ranker models [7]. Then, retrieved  documents are pruned based on the calculated  semantic similarities.

## D.   Generation  

The combined prompt from the augmentation phase is  sent to the LLM generator to produce a context-specific  answer. Finally, the generated answer is returned to the end  user. Distinct response modes define the frequency of LLM  calls per query and how multiple answers are synthesized  into one final response.

•    Compact  mode retrieves a single time and  amalgamates as many retrieved chunks that fit into  the LLM’s context length.  •    Create - and - refine  procedure starts with integrating  only one retrieved chunk into a prompt and  generating a temporary answer. Subsequently, the  prompt enhancer iterates through the remaining  retrieved documents, combines a single retrieved  document with the temporary answer in a specialized  refine prompt, and calls the LLM generator again.  This approach leads to one LLM call per retrieved  document.  •    Tree - summarization  is similar to compact mode  and concatenates retrieved documents up to the  context length. It permits multiple iterations to show  all documents at least once to the LLM generator,  synthesizing the multiple answers into a cohesive  response using a summarization template. [10]

## E.   Advanced RALM pipeline  

Advanced RALM pipelines can include complex and  expensive elements such as fine-tuned subcomponents. This  study intends to evaluate straightforward, advanced RALM  pipelines, such as routing and recursive approaches.

Routing is a technique for choosing appropriate actions  for a user question from a set of choices. If several  databases, query engines, or tools are available, routing can  be used to determine the optimal service. Given the complex  nature of FA, it can be assumed that tailored prompts for

different question categories perform better than a general  prompt. Thus, we implemented a Router RALM capable of  categorizing a query according to its question category.  Based on this classification, the query engine is initiated  with a specialized prompt template.

Recursive RALM aims to enhance retrieved documents  by repeating retrieval and integrating related information of  retrieved documents. Pre-processing might spread coherent  information across several chunks. Recursive retrieval  addresses this by first retrieving semantically related smaller  chunks. Next, recursive retrieval explores links of these  chunks to related information and integrates these into  larger segments. FA analyses are divided into five chunks  on average and might even be linked to another existing  analysis. Therefore, recursive retrieval could significantly  increase performance in such cases.

## IV.    E XPERIMENTS 

## A.   Setup  

Our study investigates whether naive and cost-effective  RALMs can accurately answer questions in FA. Moreover,  we want to identify the best hyperparameters of a RALM  pipeline, leading to improved performance. For this  purpose, the  Elastic  and  Qdrant  databases were constructed  in advance. It is important to note that only internally  deployed LLMs were utilized due to the sensitive nature of  the data. Moreover, we assessed the impact of unstructured  data on the performance of the RALM pipeline.

Given the absence of a comprehensive benchmarking  dataset in FA and the high costs associated with large-scale  human evaluation, we conducted the evaluation in two  steps. First, the RALM pipelines should be evaluated within  an ablation study based on reference-free metrics, and  second, we selected three RALM pipelines for further  evaluation by human experts.

Reference-free metrics  do not rely on a golden answer  and enable evaluation without validation datasets. Thereby,  the technique LLM-as-a-Judge utilizes the LLM itself as an  evaluator, which was recently found to show a high  correlation with human judgments [11]. Thus, responses  generated by our RALM approaches were presented to an  LLM evaluator with a specialized prompt instructing the  LLM-as-a-Judge to assess the generated response according  to a dimension. Following the RAGAs framework, we  adopted the four metrics: answer faithfulness, answer  relevance, context recall, and context precision [12].

•    Answer Faithfulness  assesses how a generative  answer is grounded and correct based on the  retrieved context. Each generation statement should  be derivable from the provided context.   •    Answer Relevance  evaluates if the generated  answer addresses the given query to a satisfactory  degree.  •    Context Recall  measures the extent to which the  ground truth aligns with the retrieved contexts.  •    Context Precision  evaluates whether all of the  essential parts of the ground truth data related to a  question are present in the retrieved contexts.

Based on these metrics, we conducted an ablation study  to analyze the impact of hyperparameters. However, it  should be noted that evaluation by LLMs entails certain  costs, as evaluating one question-context-answer triplet can  result in multiple LLM calls. To determine the influence of  unstructured data on performance, initial pipelines were  carried out with solely structured data and then combined  with unstructured data.

The various RALM pipelines were realized with the  library  LlamaIndex [13] , and the following range of  hyperparameters was examined:

•    Top-k (2, 5, 10)  defines the number of retrieved  documents from the vector database.    •    Response mode  ( compact, create-and-refine, treesummarize ) specifies how retrieved documents are  incorporated into a prompt and how often the LLM  generator is called.    •    As a  LLM generator   llama2-70b  ( llama2 ),  StarlingLM-7B-alpha  ( starling ), and  Mixtral-8x7B-Instructv0.1  ( mixtral ) were tested.    •    Rerankers  post-process the retrieved documents by  simple  reordering  or semantic reranking combined  with pruning. We utilized the  BAAI/bge-rerankerlarge  model with the   FlagEmbeddingReranker   ( FER ) utility from  LlamaIndex  and the internally  hosted  BAAI/bge-base-en-v1.5  paired with the  SentenceEmbeddingOptimizer  ( SEO ). In both  cases, we pruned  $50\%$   of the retrieved documents.    •    The  design  of the RALM pipeline was tested as a  naïve  pipeline, a  naïve  pipeline with a  re-ranker ,  advanced   routing ,   and   recursive retrieval ,  as well

as a combination of advanced RALM with  rerankers.

## B.   Reference-free evaluation  

## 1)    Structured data only  

In the experiments, we changed one component at a time  and evaluated the results based on the four RAGAs metrics.  The harmonic mean unifies these four aspects and gives a  single performance measure. Table I shows the performance  of different RALM pipelines based only on structured data.  First, we evaluated the basic hyperparameters top-k,  response mode, and LLM generator for a naïve RALM. As  the basic version of the naïve RALM pipeline, we used the  following settings: top-k: 2, response mode: compact, LLM:  Starling, complexity: naive. For instance, when evaluating  different top-k values, we used an LLM starling as a  compact response mode and as a naive design.

Varying top-k values, LLM generators, and response  modes show negligible fluctuations in performance. A  notable consistency was observed in context recall across all  nine RALM configurations, with  $30.83\%$  . This suggests that  if the retriever component successfully locates relevant  documents, it is achieved within the top two retrieved  documents. Optimal context precision was attained at a topk value of 10. Compact mode as a response mode reduced  the LLM generator calls significantly. Starling, as an LLM  generator, achieved the best harmonic mean. Subsequently,  we utilized these hyperparameter settings in further  experiments.

Integrating a re-ranker into naïve RALM led to a  substantial increase in performance. Compared with naïve  RALM, the advanced pipeline resulted only in a slight  improvement. The naive RALM pipeline, paired with the  SEO reranker, outperformed its advanced and combined  counterparts.

T ABLE  I.

ABLATION   STUDY   ONLY   ON   STRUCTURED   FA   JOB   DATA

|H yper - parameter|Value|Context Precision|Context Recall|Answer Relevancy|F aithfulness|Harmonic Mean|
|---|---|---|---|---|---|---|
|Top-k|2|26,44%|30,83%|45,37%|69,29%|37,48%|
|Top-k|5|24,84%|30,83%|44,08%|75,64%|36,83%|
|Top-k|10|27,17%|30,83%|45,92%|61,31%|37,27%|
|Response mode|Create-and-refine|25,09%|30,83%|47,97%|79,49%|37,84%|
|Response mode|compact|26,34%|30,83%|47,77%|75,00%|38,22%|
|Response mode|Tree-summarizes|26,06%|30,83%|45,80%|79,17%|38,00%|
|LLM generator|starling|28,73%|30,83%|49,88%|62,50%|38,73%|
|LLM generator|mixtral|26,23%|30,83%|50,23%|71,30%|38,28%|
|LLM generator|llama2|25,36%|30,83%|51,46%|60,78%|37,12%|
|Re-ranker|reordering|25,13%|52,63%|49,51%|88,89%|44,33%|
|Re-ranker|FER|28,49%|66,67%|39,83%|76,11%|45,27%|
|Re-ranker|SEO|40,70%|70,18%|38,52%|76,79%|51,41%|
|Design|recursive|26,77%|36,92%|55,70%|60,26%|40,41%|
|Design|routing|28,05%|34,35%|45,18%|62,18%|38,85%|
|Design|recursive, SEO|40,90%|66,67%|33,94%|36,67%|41,59%|
|Design|routing, SEO|39,99%|65,74%|34,96%|68,89%|48,00%|


|Design|Response Mode|Context Precision|Answer Relevancy|Context Recall|Faithfulness|Harmonic mean|
|---|---|---|---|---|---|---|
|naïve|compact|51,43%|57,12%|62,15%|51,18%|55,11%|
|naïve|Create-and-refine|54,75%|62,12%|68,15%|54,18%|59,27%|
|recursive|compact|50,71%|30,00%|30,00%|47,00%|45,29%|
|recursive|Create-and-refine|51,57%|41,08%|41,08%|86,67%|56,32%|
|router|compact|45,92%|39,75%|74,62%|69,48%|53,53%|
|router|Create-and-refine|50,71%|44,53%|79,63%|81,48%|59,69%|


## 2)    With unstructured data  

For the second experiment, the unstructured data was  also included in the vector database. We only tested the best  approaches from the previous analysis and advanced  RALM pipelines to reduce costs during evaluation using  the following default settings: top-k – 10, response mode –  compact, LLM – Starling, and re-ranker – SEO. We also  suspected that the recursive response mode is more  compatible with the SEO re-ranker, as SEO prunes the  documents. Thus, the create-and-refine method does not  result in many LLM generator calls and could filter out  additional irrelevant information. Table II shows the results  of different RALM pipelines, indicating the superiority of  the create-and-refine method compared to compact as  response mode. The router pipeline with create-and-refine  mode and SEO as re-ranker exhibited the best performance.

## C.   Human evaluation  

Expert evaluations were conducted to assess the quality  of the RALM pipelines. Three distinct RALM pipelines  were chosen, two based on their performance according to  the harmonic mean and one naïve pipeline as a baseline:

•    Pipeline A . Design: router (combined), response  mode: refine-and-create, re-ranker: SEO, data:  structured and unstructured.  •    Pipeline B . Design: naive, response mode: refineand-create, re-ranker: SEO, data: structured and  unstructured.  •    Pipeline C . Design: naive, response mode: compact,  data: only structured.

The experts rated the pipelines' responses to a set of 20  questions regarding accuracy and usefulness using a 5- point Likert scale, where 5 relates to high quality and 1 to  low quality/uselessness. Table III shows the results of the  human evaluation. The analysis revealed that the language  models' refusal mechanism was triggered for two  questions, declining to respond due to inadequate context,  which negligibly influenced the overall average. Pipeline A  performed best, ahead of the baseline RALM and the router  approach. It is noticeable that the RALM pipelines perform  best in the categories of next-step prediction, default  knowledge retrieval, and failure mode identification. This  is because the knowledge to answer these questions can be  provided using simple retrieval.

T ABLE  III.   H UMAN  E VALUATION  R ESULTS ON A  5- POINT  L IKERT SCALE

|Pipeline|A|B|C|
|---|---|---|---|
|Total average|2,00|2,40|2,10|
|Total average without refusal|2,03|2,39|2,09|
|Next-step prediction average|2|2,5|2,17|
|Related information identification|1,83|1,67|1,33|
|Failure mode identification|1,83|2,83|2,83|
|Safety verification|1,17|2|2,33|
|Default knowledge retrieval|2,44|2,63|2|


Success in these categories is attributed to the simplicity  of the retrieval process required to formulate accurate  responses. In general, questions in the categories of safety  verification and related information identification require  more complex retrieval and reasoning capabilities, leading  to reduced performance.

Notably, Pipeline A's performance was weakest when  employing the router approach. Further analysis identified  two factors that contributed to this underperformance.  Analysis showed that two of the router pipeline's specialized  prompts did not contain instructions for condensing  information, which led to responses perceived as too long  and rated poorly. Additionally, incorrect question category  classification by the LLM resulted in the application of  inappropriate prompt templates.

In conclusion, while generating high-quality responses  for some questions was possible, the expert evaluation  highlighted substantial opportunities to refine the RALM  pipelines. A critical area identified for improvement was  retrieving pertinent and accurate documents. Advancements  in retrieval efficacy are anticipated to boost the overall  performance of the RALM pipelines.

## D.   Case study  

The RALM pipelines yield satisfactory results for  general knowledge queries because relevant information  for answering the query was possible by single retrieval  (see Table IV).

T ABLE  IV.

RESULTS   RALM   PIPELINE   B,   QUESTION   7

|Question|What is the Failure mode 'Fused Wire' related to?|
|---|---|
|Ground truth|Electrical Overstress or Overcurrent: Fused wire occur once a too high current load is causing the meltdown of the wire|
|Generated Answer|The Failure mode 'Fused Wire' is related to a short circuit or overcurrent condition in a semiconductor device, causing the bond wire to melt and fuse, leading to a failure in the electrical connection.|


Moreover, pipeline B could produce high-quality  responses when the queries are specific, detailed, and do not  necessitate complex reasoning capabilities, see Table V.

T ABLE  V.

R ESULTS  RALM   P IPELINE  B,  QUESTION  12

|Question|What is the root cause of the observed corrosion in JOB_A|
|---|---|
|Ground Truth|Chlorine and sulfur contamination was detected using TECHNIQUE_A|
|Generated Answer|The root cause of the observed corrosion in JOB_A is not explicitly provided in the given context. However, it can be inferred that the corrosion may be related to the presence of Cl ions, as mentioned in the context of another analysis JOB_B. The Cl ions can lead to Al pad corrosion, which might be the cause of the observed corrosion in JOB_A.|


For queries of increased complexity, the approach faces  challenges   in   summarizing   essential   and   relevant  information. For instance, although the ground truth is  present in the answer in Table VI, a number of the generated  proposals are inaccurate and false.

T ABLE  VI.       R ESULTS  RALM   P IPELINE  B,   Q UESTION  2

|Question||
|---|---|
|Question|        I found an short in a device which is not decapsulated                yet. What would be the best method for localisation                of the short in the package?      |
|||
|        Ground                Truth      |Use IR-LIT or Magnetic Microscopy|
||        To localise the short in the package without                decapsulation, you can follow these steps:      |
||1. Perform curve tracing of the affected pin to|
||identify the shorted pad or bond wire.|
||2. Use infrared (IR) imaging to detect hot spots or|
||        damaged components, such as ESD diodes, in the                area of the shorted pin.      |
|||
||3. Utilize optical microscopes and X-ray imaging to|
|        Generated                Answer      |inspect the package for any visible defects or|
|        Generated                Answer      |irregularities.|
|        Generated                Answer      |4. Analyze the images and data obtained from the|
|        Generated                Answer      |above steps to pinpoint the location of the short|
|        Generated                Answer      |within the package.|
||5. If necessary, perform further analysis using|
||techniques like  thermography or electrical|
||measurements to confirm the short's location.|
|||
||Remember that the specific steps and tools used may|
|||
||equipment.|


For questions requiring advanced retrieval and  reasoning capabilities, sometimes retrieval of relevant  documents is unfeasible and can lead to hallucinations, see  Table VII.

T ABLE  VII.   R ESULTS  RALM   P IPELINE  B,   Q UESTION  13

|Question|Scan test is a structural test in order to check the functionality of the logic blocks within a semiconductor device. What is the best localization method to be used if the test is failing depending on the applied supply voltage?|
|---|---|
|Ground Truth|It is Soft Defect Localization (SDL). SDL uses a Laser scanning across the logic block (applying local Heat) while the device is stimulated repetitively close to the pass/fail border.|
|Generated Answer|For the given scan test failure depending on the applied supply voltage, the best localization method|


|would be a combination of optical or particle beam|
|---|
|techniques, and magnetic techniques. These methods|
|can help narrow down the fail area to tens of|
|micrometers at the circuit and intra-circuit level,|
|which is crucial for effective defect localization in|


To mitigate such hallucinations and improve retrieval  quality, we aim to employ a hybrid search combining  keyword and vector search, which ensures more pertinent  retrieved documents by metadata filtering. Moreover, future  research for developing a cost-effective chatbot should  consider agentic RALMs, introducing more complex  reasoning capabilities.

## V.    C ONCLUSION 

In this paper, we have introduced a simple and costeffective yet promising question-answering pipeline based  on Retrieval-Augmented Language Modeling in the  complex domain of semiconductor failure analysis. First, in  an ablation study, we determined the best hyperparameters  of a RALM pipeline by evaluating reference-free metrics.  Second, we evaluated the RALM pipelines by human  experts, indicating that RALM pipelines can generate highquality responses but still lack reasoning capabilities for  answering complex questions.

To overcome these challenges, more advanced RALM  techniques should be applied. Therefore, in the future work  we want to implement Hybrid Search and agentic  approaches focusing on enhancing the retrieval quality and  utilizing more powerful LLMs such as Llama 3.

## R EFERENCES 

[1]    C. Grabner, A. Safont-Andreu, C. Burmer, and K. Schekotihin,  "A BERT-Based Report Classification for Semiconductor Failure  Analysis," in I STFA 2022: Conference Proceedings from the 48th  International Symposium for Testing and Failure Analysis,   Pasadena, California, USA, 2022, pp. 28–35.    [2]   F. Platter, A. Safont-Andreu, C. Burmer, and K. Schekotihin,  "Report Classification for Semiconductor Failure Analysis," in  ISTFA 2021: Conference Proceedings from the 47th International  Symposium for Testing and Failure Analysis , Phoenix, Arizona,  USA, 2021, pp. 1–5.    [3]   L. Huang  et al.,  "A Survey on Hallucination in Large Language  Models: Principles, Taxonomy, Challenges, and Open  Questions," 2023, unpublished.    [4]   Nikhil Kandpal, H. Deng, Adam Roberts, Eric Wallace, and Colin  Raffel, "Large Language Models Struggle to Learn Long-Tail  Knowledge," in  International Conference on Machine Learning ,  2022. [Online]. Available: https://api.semanticscholar.org/ CorpusID:253522998    [5]   K. Luu, D. Khashabi, S. Gururangan, K. Mandyam, and N. Smith,  "Time Waits for No One! Analysis and Challenges of Temporal  Misalignment," in  Proceedings of the 2022 Conference of the  North American Chapter of the Association for Computational  Linguistics: Human Language Technologies , Seattle, United  States, 2022, pp. 5944–5958.    [6]   Gautier Izacard  et al.,  "Atlas: Few-shot Learning with Retrieval  Augmented Language Models,"  The Journal of Machine  Learning Research , vol. 24, 251:1 ‐ 251:43, 2023. [Online].  Available: http://jmlr.org/papers/v24/23-0037.html    [7]   Y. Gao  et al.,  "Retrieval-Augmented Generation for Large  Language Models: A Survey," 2023, unpublished.    [8]   A. Asai, S. Min, Z. Zhong, and D. Chen, "Retrieval-based  Language Models and Applications," in  Proceedings of the 61st  Annual Meeting of the Association for Computational Linguistics  (Volume 6: Tutorial Abstracts) , Toronto, Canada, 2023, pp. 41– 46.    [9]   N. F. Liu  et al.,  "Lost in the Middle: How Language Models Use  Long Contexts,"  Transactions of the Association for  Computational Linguistics , vol. 12, pp. 157–173, 2024, doi:  10.1162/tacl_a_00638.    [10]   J. Liu,  Response Modes.  [Online]. Available: https:// docs.llamaindex.ai/en/stable/module_guides/deploying/query_ engine/response_modes/ (accessed: Jun. 10 2024), unpublished.    [11]   L. Zheng  et al.,  "Judging LLM-as-a-Judge with MT-Bench and  Chatbot Arena," in  Advances in Neural Information Processing  Systems , 2023, pp. 46595–46623. [Online]. Available: https:// proceedings.neurips.cc/paper_files/paper/2023/file/ 91f18a1287b398d378ef22505bf41832-Paper-Datasets_and_ Benchmarks.pdf    [12]   S. Es, J. James, L. Espinosa Anke, and S. Schockaert, "RAGAs:  Automated Evaluation of Retrieval Augmented Generation," in  Proceedings of the 18th Conference of the European Chapter of  the Association for Computational Linguistics: System  Demonstrations , 2024, pp. 150–158. [Online]. Available: https:// aclanthology.org/2024.eacl-demo.16    [13]   J. Liu,  LlamaIndex , 2022. [Online]. Available: https://github.com/ jerryjliu/llama_index  (accessed: Jun. 10 2024), unpublished.

