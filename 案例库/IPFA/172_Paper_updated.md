---
title: "172_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_f633d08f6afecef265f358a4484ccf647295230462135641
file_size: 1180466
---

## Improved Yield Prediction and Failure Analysis in  Semiconductor Manufacturing with XGBoost and  Shapley Additive exPlanations Models  

Shiqi Wang 1 , Yining Chen 2  1   School of Microelectronics, University of Science and Technology of China, Fuxing Road, Hefei, Anhui, China  2 School of Integrated Circuits, Zhejiang University, Honghui Road, Hangzhou, Zhejiang, China  Phone: (+86)13003630090, Email: yining.chen@zju.edu.cn

Abstract —In the domain of semiconductor manufacturing,  the accurate prediction of wafer yield and subsequent failure  analysis (FA) are of critical importance with respect to the  assurance of product quality and the optimization of production  processes. However, traditional methods frequently exhibit a  high dependency on engineering expertise, modest accuracy,  and an inability to adapt swiftly to manufacturing environment  changes. To address these issues, this study introduces an  advanced machine learning (ML) model that combines Particle  Swarm Optimization (PSO) with XGBoost. This innovative  approach is adept at capturing the complex non-linear  relationships between wafer acceptance test (WAT) data and  wafer yield. The integration of PSO enables effective WAT  feature selection while fine-tuning the hyperparameters of the  XGBoost, thereby resulting in a significant improvement in  model performance. The proposed PSO-XGBoost model  exhibits remarkable accuracy  $(96.4\%)$  , AUC-score   $(\mathbf{91.4\%})$  ), F1- measure   $\mathbf{(97.9\%)}$  , precision   $(\pmb{97.2\%})$  , and recall   $(98.6\%)$  .  Moreover, the integration of the Shapley Additive exPlanations  (SHAP) method facilitates the interpretability of the model,  elucidating the critical WAT parameters that influence yield on  both global and local scales. This study not only provides a costeffective methodology that reduces reliance on human expertise  but also paves the way for the expanded role of artificial  intelligence (AI) in enhancing semiconductor manufacturing  processes. This represents a new era in the field of smart  manufacturing and quality assurance.

Keywords—Wafer yield prediction, failure analysis, XGBoost,  particle swarm optimization, SHAP method

## I.    I NTRODUCTION 

At the forefront of advancements in artificial intelligence  (AI), integrated circuits (ICs) stand as indispensable  components, crucial for the operation of systems across a  multitude of applications. However, the manufacturing  process of ICs is characterized by its intricate and  multifaceted nature[1,2]. The process of fabricating an IC  typically unfolds through four distinct stages: wafer  manufacturing, wafer probing, packaging, and final  testing[3]. Of these stages, wafer manufacturing holds  particular significance, serving as the foundational pillar of  IC production. Herein, pristine silicon-based substrates  undergo a meticulously orchestrated sequence of operations,  encompassing oxidation, deposition, lithography, etching,  ion implantation, and various other processes, each  contributing   to   the   intricate   fabrication   process.  Consequently, this intricate process often incurs yield  losses[4]. Timely detection of suboptimal wafers and diligent  failure analysis (FA) at this juncture are imperative, serving  to avert futile capital investment in defective units, thereby  conserving resources and mitigating subsequent financial  expenditures[5].

In wafer manufacturing, the wafer acceptance test (WAT),  also known as process control monitor (PCM), assumes a  pivotal role in ensuring adherence to stringent specifications.  It serves as a critical tool for tracking upstream process  parameters when encountering discrepancies in wafer  yield[6,7]. However, in instances of yield loss, the  conventional recourse entails a meticulous manual review of  WAT data by engineers to ascertain the underlying cause of  yield deviation. This process is both time-intensive and  reliant on the expertise of individuals, ironically highlighting  a reliance on human acumen despite the endeavor to augment  it through AI technologies[8-10]. Urgent attention is thus  warranted to devise novel methodologies that enable efficient  and accurate wafer yield prediction (WYP) and FA, thereby  reducing costs and diminishing the reliance on highly  specialized engineers.

The burgeoning integration of AI into process  engineering, particularly through machine learning (ML) and  deep learning (DL) modalities, presents a compelling avenue  for innovation in WYP and FA[11-13]. For example, Xu et  al. introduced the deep belief networks (DBN) to predict  wafer yield. Their approach amalgamated the minimum  redundancy maximum relevance (mRMR) method with  genetic algorithm (GA) to select key WAT parameters, which  improved the prediction accuracy of the model[14]. Jiang et  al. employed an integrated model with a voting mechanism  to predict wafer yield. They ranked the most important WAT  parameters for the prediction results based on the feature  importance score of the model[15]. In a subsequent study,  Jiang et al. proposed utilizing a Gaussian mixture model  (GMM) to pre-cluster samples for improved model  performance[16]. Additionally, Xu et al. introduced a support  vector machines (SVM) model for yield prediction. To  enhance accuracy, they advocated a high-dimensional  alternating feature screening (HAFS) method for automated  WAT feature selection[17]. These endeavors leverage ML  models to address the WYP challenge and incorporate feature  selection techniques, including filtering methods and  intelligent optimization algorithms, to enhance WYP  performance by extracting key WAT parameters.

Feature screening plays a crucial role in enhancing model  prediction speed and accuracy by eliminating redundant and  irrelevant features, thereby significantly impacting prediction  outcomes and mitigating overfitting[18]. However, a  considerable proportion of research has overlooked the  influence of model hyperparameters on WYP results. Model  hyperparameters directly govern algorithm behavior, thus  exerting a profound effect on model performance[19,20].  Commonly used methods for hyperparameters optimization  include grid search, random search, Bayesian-based methods,  and intelligent optimization algorithms. Among these

methods, intelligent optimization algorithms, such as GA,  whale optimization algorithm (WOA), and particle swarm  optimization (PSO), have shown considerable performance in  recent studies[21,22]. The development of PSO is grounded  in observations of the social behavior exhibited by birds and  fish. In comparison to alternative algorithms, the PSO offers  several appealing attributes. Each particle possesses memory  and can retain its individual knowledge of favorable  solutions. Moreover, all particles engage in constructive  cooperation, exchanging information concerning the global  optimal solution. Recognizing the promising application  prospects of the PSO in both feature selection and  hyperparameter optimization, this study treats feature  extraction and hyperparameter optimization as a unified  optimization task and adopts the PSO to concurrently address  feature selection and hyperparameter optimization.

Moreover, a significant portion of existing research  focuses exclusively on WYP issues, overlooking the pivotal  step of post-prediction FA in refining subsequent production  recipes. This oversight stems from the opaque nature of many  ML models, which hinders researchers' ability to comprehend  and interpret the operational patterns of the model[23]. The  extraction of causal explanations from these 'black box'  models has long perplexed semiconductor experts. In  response to this challenge, the present study introduces the  Shapley Additive exPlanations (SHAP) method, a widely  used interpretable ML tool, to facilitate a transparent analysis  of the WYP model and to conduct FA on low-yield wafers.

In summary, this study proposes the application of  interpretable ML techniques to achieve WYP and FA of lowyield wafers in semiconductor manufacturing. Various  popular ensemble tree models, including random forest (RF),  gradient boosting decision tree (GBDT), XGBoost, and  Catboost, are considered for serving as the WYP model. The  PSO algorithm is employed to optimize both the WAT  feature set and model hyperparameters to attain enhanced  performance. Furthermore, the prevalent SHAP method,  rooted in game theory, is utilized to elucidate the prediction  output of the model and facilitate comprehensible FA to aid  engineers in rectifying low-yield wafers. As depicted in Fig.  1, the proposed method enables robust WYP and FA in  semiconductor manufacturing, thereby offering valuable  decision-making guidance to practitioners and ultimately  reducing time and labor costs. This study achieves parallel  processing of feature screening and hyperparameter  optimization based on existing research in the field of WYP  and advances the application of the SHAP method for FA,  thereby providing valuable insights into the future  development of AI in semiconductor manufacturing.

The subsequent sections of this paper outline our research  as follows: Section 2 presents the problem statement and data  description, detailing the research methods and evaluation  metrics. Section 3 introduces data preprocessing, discusses  and analyzes the prediction results of various ML models.  Section 4 focuses on interpretability analysis, encompassing  FA for low-yield wafers. Finally, Section 5 concludes with a  discussion of the results and implications of this study.

![WaferManufacturing   WaferProbing  Input   TheProposedWYP  WAT   withFAModel  Oxidation   Data  Output  Deposition  Failure  Analysis   Packaging  Lithography  Lowyield   Highyield  Control   wafers   wafers  Etch   Adjust  Implantation   Terminate/Scrap  Final Testing  Expert     ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5eaacf7b-f581-499e-9835-6cc42045494a/5eaacf7b-f581-499e-9835-6cc42045494a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215868%3B1743219468&q-key-time=1743215868%3B1743219468&q-header-list=host&q-url-param-list=&q-signature=35dfdea07a88d449a671bdfe21afab60f71c7a15)
Fig. 1.    Applications of WYP and FA model in semiconductor  manufacturing

This research is supported by Zhejiang Provincial Department of Science and  Technology’s 2024 R&D Project (2024JCZX0031), and SUTD-ZJU IDEA  Visiting Professor Grant SUTD-ZJU (VP) 201906.

## II.    P RELIMINARIES AND METHODS 

## A.   Data Description and Problem Statement  

An authentic dataset of WAT measurements, sourced  from a 12-inch 55 nm full production mini-line in Zhejiang  Provincial CMOS IC innovation center, serves as the  empirical foundation for the evaluation of our research. The  employed dataset encompasses eight distinct wafer lots,  totaling over 1600 wafers and each wafer is delineated by  1308 WAT parameters and a yield value. The statistical  information of the actual dataset is represented in Table 1.

The WAT parameters encompass a variety of electrical  characteristic parameters related to the active and passive  devices, as well as isolation structures within the die. These  parameters include threshold voltage ( V t ), saturation current   $\left(I_{\mathrm{sat}}\right)$  , and leakage current ( I off ) associated with MOS  transistors. Table 2 provides a comprehensive list of primary  WAT parameters along with their corresponding units. Each  parameter serves as an input feature for forecasting wafer  yields within the model. Thus, the WYP is framed as a typical  ML problem utilizing (a) the input characteristics from the  WAT dataset    $\scriptstyle{X=\{x_{I},\ x_{2},\ \dots,\ x_{n}\}}$   and (b) the corresponding  wafer yield to train a classifier model denoted as  ܻ ,

$$Y\,\bigtriangledown C\,(x_{I}\bigtriangledown x_{2}\bigtriangledown\bigcirc...\bigtriangledown x_{n}\bigtriangledown$$
where   $C$   represents the ML algorithm model employed. In  this study, prediction performance is enhanced through WAT  feature selection and model hyperparameter optimization  using the PSO algorithm. Subsequently, the post-explanatory  SHAP method is applied to conduct robust FA of low-yield  wafers.

TABLE I.    S TATISTICAL INFORMATION OF THE ACTUAL  WAT  DATASET

|Data set|Measurement|Values|
|---|---|---|
|WAT001|Dataset size|22.90 MB|
|WAT001|Number of low yield wafers|1404|
|WAT001|Number of high yield wafers|252|
|WAT001|Number of features|1308|


TABLE II.

I NFORMATION ABOUT  W AFER  A CCEPTA NCE   T EST

P ARAMETERS

||No.|Wafer Acceptance Test Parameters|Units|
|---|---|---|---|
|MO S|1|IBOFF: Bulk Leakage Current|pA/ ߤ m|
|MO S|2|IDOFF2: Drain Leakage Current|pA/ ߤ m|
|MO S|3|IGOFF: Gate Leakage Current|pA/ ߤ m 2|
|MO S|4|ISOFF: Source Leakage Current|pA/ ߤ m|
|MO S|5|IDL: Drain Linear Current|ߤ A/ ߤ m|
|MO S|6|IDS: Drain Saturation Current|ߤ A/ ߤ m|
|MO S|7|VTL: Linear Threshold Voltage|V|
|MO S|8|VTS: Saturation Threshold Voltage|V|
|Chip|9|IDDQ: Isolation Leakage Current (WL OFF)|nA|
|Chip|10|ILeak: Isolation Leakage Current (WL ON)|nA|
|Chip|11|LKG: Leakage Current|nA|
|Chip|12|RS: Sheet Resistance|ohm|


## B.   Ensemble Tree Models  

Among various ML models, tree models and their  variants, including RF, GBDT, XGBoost, and Catboost, have  demonstrated superior performance compared to logistic  regression (LR), SVM, and neural networks in handling  tabular data[24]. RF enhances prediction performance by  constructing multiple decision trees, each trained on a  random subset to increase model diversity. GBDT improves  prediction performance through iterative training of a series  of tree models. XGBoost builds upon GBDT by introducing  regularization and an improved split-node strategy to enhance  the speed and accuracy of the algorithm. Catboost further  extends the model's framework for processing data with  categorical features without the necessity of one-hot  encoding.

## C.   Particle Swarm Optimization  

The PSO algorithm is a stochastic optimization technique  inspired by the social behavior observed in bird flocks[25]. It  commences with the random initialization of a population of  particles, each characterized by a position and velocity. The  PSO algorithm iteratively updates the position and velocity  of each particle based on the best-performing particle in the  group, gradually converging towards the optimal solution.  Specifically, the velocity of each particle is updated  according to (1).

where  $x t{+}I$   id  and  xt id  represent the positions of the particle  at the next moment and the current moment, respectively.

Furthermore, to improve the performance of the PSO  algorithm, the inertia weight is adjusted using (3).

ω  ω min  ω max    ω min 1  t t max

where  $t$   and   $t_{m a x}$   denote the current number of iterations and  the maximum number of iteration, respectively.

The fitness function plays a key factor in the PSO method.  In our research, the fitness function is defined as follows:

fitness  α ACC  1   α 1  S selected S total

where  ACC  represents the classification accuracy of the  model, and a technique called threefold cross-validation was  used to enhance the reliability.  S selected  is the number of  features selected,  S total  is the total number of features in the  original dataset,   $\alpha$    represents the weight, and   $\alpha\!\in\left(0,1\right)$  .

## D.   Shapley Additive exPlanations  

The SHAP method is a post hoc explanation model based  on game theory principles, originally proposed by Shapley in  1953[26].

This method elucidates the inner workings of ML models,  often referred to as "black boxes," from both a global and  local perspective. Specifically, Shapley values offer an  explanatory framework that approximates the original ML  model by quantifying the marginal contribution of each  feature to the model output. This can be described by  equations (5) and (6)[27]. In (5) and (6), the explanatory  model and the ML model are represented by   $m$   and   $f,$    respectively.  x  represents all input features, represented by   $\scriptstyle{x^{\prime}\in\{0,1\}^{\mathrm{N}}}$  , where   $N$   is the total number of features. In   $x^{\prime}$  , a  value of 1 means the inclusion of a feature in the explanatory  model, while 0 indicates its exclusion.  $F$   and  $S$   are the set of  all features and the feature subset that excludes the  $j$  -th  feature, respectively.  $x_{s}$   represents the input features in subset  S . The influence of the  $j$  -th feature is expressed as  $\upvarphi_{j}$  .

$\nu t{+}I$   id  ωvt id  c 1  r 1   pt id,pbest  xt id  c 2  r 2   pt

d,gbest xt id

$$\begin{array}{r}{m(x^{\prime})=\varphi_{0}+\sum_{j=1}^{N}\dddot{\dddot}\dots\dddot\varphi_{j}x_{j}^{\prime}}\end{array}$$
where  $\nu t{+}I$   id  and  vt id  represent the speed of the particle at  the next moment and the current moment, respectively.  ω   denotes the inertia weight,  c 1  stands for the individual  learning factor,  c 2  denotes the group learning factor,   $r_{I}$   and  $r_{2}$    are both random number where  $_{r_{I}\in[0,1\rangle}$   and   $_{r2}{\in}[0,\!1\rangle$  .  pt id,pbest  and  pt d,gbest  signify the individual and group  historical optimal positions at the current moment  respectively.

$$\begin{array}{r}{\varphi_{j}=\sum_{S\subseteq F\backslash\{j\}}^{\ddagger\dotsi}\frac{|S|!(|F|-|S|-1)!}{|F|!}\big[f_{S\cup\{j\}}\big(x_{S\cup\{j\}}\big)-}\end{array}$$
Then, the particle's position is updated according to (2).

݂ ௌ

(ݔ

ௌ

)]

The Shapley value of a variable is higher when its  contribution is greater[28]. This method locally quantifies the  contribution of each feature to the prediction result of a given  sample, while utilizing the average of the absolute values of  all Shapley values to measure the global importance of the  feature. Thus, both local and global interpretability of the  model can be obtained.

## E.   Assessment Metrics for Evaluation  

Evaluation metrics play a crucial role in assessing ML  models, especially in the domain of classification algorithms.  Commonly employed metrics include accuracy, F1-measure,  precision, recall, and the AUC-score. The mathematical  formulations of these metrics are presented in Table 3. In this  table, TP, TN, FP, and FN denote true positives, true  negatives, false positives, and false negatives, respectively.  In this study, low-yield wafers are considered the primary  objects to be captured, representing the positive class.

"Accuracy" denotes the ratio of correctly identified  wafers to the total number of wafers. "Precision" represents  the fraction of true low-yield wafers accurately identified out  of all wafers classified as low-yield. "Recall" signifies the  proportion of low-yield wafers accurately classified relative  to the total number of actual low-yield wafers. It is important  to note that these metrics may be significantly influenced by  the distribution of positive and negative samples in the  dataset[29]. The F1-measure is the weighted harmonic mean  of precision and recall, providing a balanced assessment of  the model's performance. A higher F1 score indicates a more  robust classifier. Additionally, the AUC-score, which stands  for the area under the Receiver Operating Characteristic  (ROC) curve, evaluates the model's performance across  various thresholds, thereby eliminating subjective bias in  threshold selection. Unlike other metrics, the AUC-score is  insensitive to imbalances between the positive and negative  classes, making it the standard assessment criterion for  classification algorithms[30]. In this research, we utilize all  five performance evaluation metrics to comprehensively  assess the effectiveness of the proposed method.

TABLE III.

C OMMON PERFORMANCE EVALUATION METRICS

|Learning Algorithm|Evaluation Metrics|Equation|
|---|---|---|
|Supervised Classification|Accuracy|ܥܥܣ= ܶܲ+ ܶܰ ܶܲ+ܲܨ+ ܶܰ+ܰܨ|
|Supervised Classification|Precision|ܲ݁ݎ= ܶܲ ܶܲ+ܲܨ|
|Supervised Classification|Recall|ܴ݁ܿ= ܶܲ ܶܲ+ܰܨ|
|Supervised Classification|F1-measure|ܨ1 = 2 ∗݌݊݋݅ݏ݅ܿ݁ݎ∗݈݈ܽܿ݁ݎ ݌݊݋݅ݏ݅ܿ݁ݎ+݈݈ܽܿ݁ݎ|
|Supervised Classification|AUC-score|-|


## III.    E XPERIMENTS AND RESULTS   

## A.   Data Preprocessing  

The input WAT dataset exhibits significant variations in  dimensional scales across different test items. As depicted in  Table 2, the unit ranges for each test item diverge  substantially, with certain items differing by up to nine orders  of magnitude. This disparity can be attributed to the  operational characteristics of transistors, where the drain  current can vary across approximately eight orders of  magnitude, while the drain voltage typically fluctuates  between   0-1V   for   N-channel   Metal-oxide  Semiconductors[31]. Such dimensional inconsistencies could  introduce feature sensitivity in the classification model,  thereby adversely affecting algorithmic performance. To  mitigate this issue, the RobustScaler is initially employed to  normalize the feature dimensions while retaining as much of  the original data's information as possible.

After normalizing the data, we utilized the Pearson  correlation coefficient to analyze the linear correlation  between variables. In the WAT process, nine predetermined  test coordinate points are selected on a wafer to ensure  comprehensive evaluation of all possible situations, a  standard practice in most foundries to ensure objectivity and  accuracy in the assessment process. The names of the WAT  parameters include numbers from 1 to 9, corresponding to  different testing points. Additionally, the letters "L" and "R"  indicate the left and right positions of the same test key.  However, for most standard processes, the results obtained  from the left and right positions at the same test key will  exhibit high linearity due to their similar process parameters.  Fig.2 displays the heat map of the first ten features in the  original WAT dataset. The color red indicates a high degree  of linear correlation, while blue indicates the opposite. From  Fig.2, a strong linear relationship with a correlation  coefficient of 1 between WAT items at the left and right  positions of certain identical test keys is observed. One  example is the first two WAT parameters in the dataset –  IBOFF_1158PD_3_L   and   IBOFF_1158PD_3_R   –  representing the bulk leakage current situated on either side  of test point 3. To mitigate this issue, only one of the features  with correlation coefficients exceeding 0.7 was retained,  thereby reducing the original 1308-feature dataset to 394  salient features[32]. Fig.3 displays the revised correlation  coefficients for the first ten features in new dataset,  confirming the mitigation of strong inter-feature correlations.

![1.U  IBOFF_1158PD 3L  1.000  1.000  0.023  0.234  -0.006-0.006  0.120  0.103  0.131  0.131  IBOFF_1158PD_3_R  1.000  1.000  0.023  0.234  -0.006-0.006  0.120  0.103  0.131  0.131  0.8  IBOFF_1158PD_6_L  0.0230.023  1.000  0.384  0.361  0.361  0.4440.458  0.005  0.005  IBOFF_1158PD_6_R-  0.234  0.234  0.384  1.000  0.199  0.199  0.125  0.129  0.064  0.064  0.6  IBOFF_1158PG1_2_L--0.006-0.006  0.361  0.199  1.000  1.000  0.3140.323  -0.007-0.007  IBOFF_1158PG1_2_R  -0.006  -0.006  0.361  0.199  1.000  1.000  0.314  0.323  -0.007  -0.007  0.4  IBOFF_1158PG1_5L  0.120  0.120  0.444  0.125  0.314  0.314  1.000  0.998  0.107  0.107  IBOFF_1158PG1_5_R  0.103  0.103  0.458  0.129  0.323  0.323  0.998  1.000  0.111  0.111  0.2  IBOFF_1158PG2_1_L  0.131  0.1310.005  0.064-0.007-0.0070.107  0.111  1.000  1.000  IBOFF_1158PG2_1_R  0.131  0.1310.005  0.064-0.007-0.0070.107  0,111  1.000  1.000  0_0  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fe6522be-96eb-4dec-bedd-aa2ca8274a4d/fe6522be-96eb-4dec-bedd-aa2ca8274a4d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215868%3B1743219468&q-key-time=1743215868%3B1743219468&q-header-list=host&q-url-param-list=&q-signature=62a39173033d35d5e43edcda2828697b16416391)
Fig. 2.    Correlation coefficient of the first ten features of the  original data set

![1.0 IBOFF 1158PD 3L 1.000 0.234 -0.006 0.120 0.131 0.170 0.014 0.1090.1090.002 IBOFF_1158PD_6_R 0.234 1.000 0.199 0.125 0.064 0.085 0.006 0.232 0.113 -0.002 0.8 IBOFF_1158PG1_2_L -0.006 0.199 1.000 0.314 -0.007 0.219 0.019 0.141 0.141 -0.002 IBOFF_1158PG1_5_L 0.120 0.125 0.314 1.000 0.107 0.280 0.025 0.180 0.003-0.001 0.6 IBOFF_1158PG2_1_L 0.1310.0640.0070.107 1.000 0.0720.005 0.097 0.006-0.002 IBOFF_1158PG2_4_L 0.1700.085 0.2190.280 0.072 1.000 0.084 0.1250.005-0.002 04 IBOFF_1158PG2_4_R 0.0140.006 0.019 0.025 0.005 0.084 1.000 0.011 -0.002-0.001 IBOFF_1158PU_3_L 0.109 0.2320.141 0.180 0.097 0.125 0.011 1.000 -0.004-0.001 0.2 IBOFF_1158PU_6_L 0.109 0.113 0.141 0.003-0.0060.005-0.002-0.004 1.000 -0.002 IBOFF_620PD_3_L -0.0020.002-0.002-0.001-0.002-0.002-0.0010.001-0.002 1.000 0_0 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/885f5c04-9810-43f7-8bd8-7d0ff16a0c73/885f5c04-9810-43f7-8bd8-7d0ff16a0c73.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215868%3B1743219468&q-key-time=1743215868%3B1743219468&q-header-list=host&q-url-param-list=&q-signature=3222827cd47e9a0574ecae26a5fdc479dfbcfb97)
Fig. 3.    Correlation coefficient of the first ten features after  Pearson analysis

## B.   Classifier Performance Evaluation  

Four different ensemble tree models, namely RF, GBDT,  XGBoost, and Catboost, were employed for WYP. To ensure  robust evaluation, the entire dataset was divided into a  training set of   $80\%$   and a test set of   $20\%$  . The models were  trained on the training set and evaluated on the test set, with  the results presented in Table 4. No further feature screening  or hyperparameters optimization was performed on each  model. Table 4 illustrates that XGBoost outperforms other  classifiers in terms of training time, accuracy, F1-measure,  and recall. Although Catboost performs slightly better than  XGBoost in terms of AUC-score and accuracy, it requires 31  times more training time (12.477s vs. 0.402s for XGBoost),  falling short of engineers' expectations for practical  efficiency. The performance of RF and GBDT is less  competitive than that of XGBoost.

Moreover, in WYP, significant emphasis is placed on the  recall index of the models. The recall rate indicates the  model's ability to accurately identify low-yield wafers from  all low-yield wafers, which is crucial for practical  applications. As depicted in Table 4, XGBoost exhibits a  significantly higher recall rate than other models, at   $98.2\%$  ,  indicating excellent performance in identifying low-yield  wafers. Therefore, XGBoost is the preferred model for WYP  and subsequent FA for low-yield wafers after comprehensive  consideration.

TABLE IV.

P ERFORMANCE COMPARISON OF DIFFERENCE  MODELS

|Evaluation Metrics|RF|GBDT|XGBoos t|Catboost|
|---|---|---|---|---|
|Training time(s)|0.886|13.850|0.402|12.477|
|Prediction time(s)|0.009|0.004|0.009|0.020|
|Accuracy|0.928|0.928|0.949|0.940|
|AUC-score|0.837|0.853|0.873|0.876|
|F1-measure|0.958|0.957|0.970|0.965|
|Precision|0.948|0.954|0.958|0.961|
|Recall|0.968|0.961|0.982|0.968|
|Total Rank|15|13|25|20|


## C.   Model Optimization Evaluation  

To   enhance   model   prediction   performance,   we  specifically utilized the PSO method for feature selection and  model hyperparameter optimization on the dataset. Feature  selection filters redundant and irrelevant features in the WAT  dataset, thereby improving the accuracy and speed of WYP.  Additionally, four key XGBoost hyperparameters that  significantly affect the model's prediction ability were  optimized, including  n_estimators ,  max_depth ,  gamma , and  learning_rate [33,34].   For   the   PSO   method,   it   is  recommended to set both the individual learning factor and  the population learning factor of the algorithm to 2.  Moreover, the maximum value of the inertia weight is set to  0.9, while the minimum value is set to 0.4. The population  size is set to 50, and the number of iterations is set to 300.

After applying the PSO algorithm, the initial 394 WAT  feature sets were reduced to 162. The optimized XGBoost

hyperparameter   configuration   was   n_estimators =347,  max_depth =5,  gamma =0.7, and  learning_rate  $\mathord{\approx}0.096$  . Table  5 compares the performance of unoptimized XGBoost and  PSO-XGBoost on the test set. The results indicate that the  prediction accuracy of PSO-XGBoost increased by  approximately   $1.5\%$  , and the AUC-score increased by  approximately   $4.1\%$  . Moreover, the other performance  metrics also showed improvement within a certain range,  demonstrating the effectiveness of the PSO method. Given  the high financial stakes in semiconductor manufacturing —  each wafer potentially valued in the thousands of dollars —  the incremental performance gains can translate to substantial  economic benefits.

TABLE V.

P ERFORMANCE COMPARISON BETWEEN  XGB OOST  AND  PSO-XGB OOST

|Evaluation Metrics|XGBoost|PSO-XGBoost|
|---|---|---|
|Training time(s)|0.402|0.846|
|Prediction time(s)|0.009|0.001|
|Accuracy|0.949|0.964|
|AUC-score|0.873|0.914|
|F1-measure|0.970|0.979|
|Precision|0.958|0.972|
|Recall|0.982|0.986|


## IV.    I NTERPRETABILITY ANALYSIS   

Based on the predicted performance results, we have  concluded that PSO-XGBoost is the optimal model for WYP  and FA on low-yield wafers. To provide an in-depth analysis  of the prediction results and FA of low-yield wafers, we  employed the SHAP method, a post hoc interpretation  method, to offer insightful interpretation.

## A.   Feature Importance Plot  

The SHAP method calculates the importance score of  each feature by averaging the absolute values of their SHAP  values and presents it in a standard bar chart. Fig.4 displays  the feature importance plot of the PSO-XGBoost model for  WYP, illustrating the relative importance of the top 20 most  important features. As depicted in Fig.4, the feature  RS_525_PO_CS_CHAIN_18 exhibits the highest SHAP  value of 0.55, suggesting that it exerts the most significant  impact   on   the   results   of   WYP.   Additionally,  RS_525_PO_CS_STACK_3, RS_525_PO_CS_STACK_20,  and IDL_789bPU_3_L are also substantial contributors to  WYP. In contrast, features such as IGOFF_789bPD_3_L,  IGOFF_789bPD_1_L,   and   IDL_789PG_4_R   have   a  relatively minor impact on the prediction results.

![RS_525_PO_CS_CHAIN_18   +0.55  RS_525_PO_CS_STACK_3   ++0.45  RS_525_PO_CS_STACK_20   +0.39  IDL_789bPU_3_L   H0.36  LKG_525_PAA_PAA_1_1.2VDD   H0.34  IBOFF_620PU_5_L   0.33  RS_525_PO_CS_CHAIN_16   +0.33  RS_525_PO_CS_STACK_4   H0.29  IGOFF_789bPU_3_R   H0.24  IBOFF_974PU_5_L   +H0.24  RS_525_PO_CS_STACK_8   +0.23  IBOFF_974PU_2_L   0.21  RS_525_PO_CS_CHAIN_10   +0.21  RS_525_PO_CS_STACK_19   0.17  RS_789_PO_WLM3_STACK_4   +0.17  IDL_789PU_1_L   40.14  IGOFF_789bPD_3_L   +0.13  IBOFF_789bPU_1_L   +0.13  IDL_789PG_4_R   10.13  RS_789_AA_BL_STACK_19   +0.11  02   03   0S  mcan(SHAP value)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8d6f97f2-58ca-4694-a9df-e28f7403f939/8d6f97f2-58ca-4694-a9df-e28f7403f939.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215868%3B1743219468&q-key-time=1743215868%3B1743219468&q-header-list=host&q-url-param-list=&q-signature=caccecab6cae7471d7b09308333f2e2f8eadbb46)
Fig. 4.    SHAP feature importance plot

## B.   Summary Plot  

Fig.5 presents the summary plot of the feature density  calculated using the SHAP method. The vertical axis sorts the  top 20 WAT parameters by feature importance, while the  horizontal axis represents the SHAP values. Each feature is  depicted with different colors indicating various feature  values, with red indicating larger feature values and blue  representing smaller ones. Unlike the feature importance plot,  the summary plot evaluates not only the impact of each  feature but also the influence of the feature value on model  prediction results. Among the selected WAT parameters,  RS_525_PO_CS_CHAIN_18 was utilized to verify the Node  net open behavior of the PO-CT-M1 layers, i.e., contact via  and Poly. As observed from Fig.5, a lower value of  RS_525_PO_CS_CHAIN_18 corresponds to a higher SHAP  value, indicating that a smaller resistance value implies better  connection between the via and the Poly. Additionally, a  smaller resistance value may lead to a reduced voltage drop,  resulting in lower power consumption and heat dissipation.

The WAT parameters RS_525_PO_CS_STACK_3 and  RS_525_PO_CS_STACK_20 are also crucial factors  following RS_525_PO_CS_CHAIN_18. They are both  employed to verify the Node net open behavior between POshare CT-M1-V1-M2 layers, specifically via and M1 metal  layers. As depicted in Fig.5, lower eigenvalues of  RS_525_PO_CS_STACK_3   and  RS_525_PO_CS_STACK_20 correspond to higher SHAP  values, consistent with RS_525_PO_CS_CHAIN_18.

The   fourth   significant   WAT   parameter,  IDL_789bPU_3_L, denotes the current in the linear region  when the PMOS transistor is turned on. It has been observed  in Fig.5 that higher IDL values positively impact the model,  while lower values have a negative effect. This finding aligns  with existing knowledge that larger IDL reflects faster and  better device performance. The subsequent significant WAT  parameter, LKG_525_PAA_PAA_1_1.2VDD, exhibits a  greater positive impact on the model when its value is low.  This parameter verifies the isolation between the active areas  (AA) by testing the leakage current between the two  pMOSFET active areas. Maintaining a minimal leakage  current is crucial, as such current does not contribute to the  device's performance. Additionally, similar analysis can be  applied to the remaining features to establish a correlation  between the value of the WAT parameter of interest and the  model predictions. The summary plot elucidates the

relationship between characteristic values and characteristic  SHAP values, offering valuable insights into the effect of  various WAT parameter values on wafer yield.

![High  RS_525_PO_CS_CHAIN_18  RS_525_PO_CS_STACK_3  RS_525_PO_CS_STACK_20  IDL_789bPU_3_L  LKG_525_PAA_PAA_1_1.2VDD  IBOFF_620PU_5_L  RS_525_PO_CS_CHAIN_16  RS_525_PO_CS_STACK_4  IGOFF_789bPU_3_R  IBOFF_974PU_5_L  RS_525_PO_CS_STACK_8  IBOFF_974PU_2_L  RS_525_PO_CS_CHAIN_10  RS_525_PO_CS_STACK_19  RS_789_PO_WLM3_STACK_4  IDL_789PU_1_L  IGOFF_789bPD_3_L  IBOFF_789bPU_1_L  IDL_789PG_4_R  RS_789_AA_BL_STACK_19  SHAPvalue(impactonmodeloutput)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4bf218f2-0ec5-4db3-8f7d-f86047eb459f/4bf218f2-0ec5-4db3-8f7d-f86047eb459f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215868%3B1743219468&q-key-time=1743215868%3B1743219468&q-header-list=host&q-url-param-list=&q-signature=5ca19269e8f58c90a8a2173970ff08d496873599)
Fig. 5.    SHAP summary plot

## C.   Low Yield Wafer Analysis  

Fig.6 presents a waterfall diagram elucidating a low-yield  wafer prediction result. In the diagram, red indicates a  feature's positive contribution to the predicted value, while  blue signifies a negative contribution. The feature's value is  depicted on the left side of the diagram. As depicted in Fig.6,  the value of RS_525_PO_CS_CHAIN_16 (approximately   $10^{30})$   significantly deviates from the baseline value (typically   $10^{8}$   to   $10^{\circ}.$  ), resulting in a decrease of 0.45 in the predicted  yield.   The   structure   of   the   test   key  RS_525_PO_CS_CHAIN_16 is illustrated in Fig.7. This test  item primarily examines the connection of the contacts  between the Poly layer and the M1 layer. In Fig.7, the total  resistance of the area is computed using the voltage and  current values measured by the H and L pads, then divided  by the number of contacts in the area to obtain the resistance  value for each contact. The RS_525_PO_CS_CHAIN_16 of  the low-yield wafer in Fig.6 does not meet the specified  baseline of this test key, which is a major cause of the wafer's  yield failure.

Additionally, in Fig.6, WAT items with results within the  specified baseline range, such as IGOFF_789bPU_3_R and  LKG_525_PAA_PAA_1_1.2VDD, have a positive impact  on yield prediction results. It is important to note that the  order of feature importance in the waterfall plot of a specific  sample may differ from the global ranking in Fig.5. This  discrepancy arises because the importance of each feature  may vary for a specific sample. In summary, the analysis of  waterfall diagrams for low-yield wafers visually displays the  faulty WAT parameters of each low yield wafer, providing  valuable insights for achieving fast and intelligent FA postmanufacturing.

![fx)=4.937  9.972=IGOFF_7896PU_3_R   +0.75  8367226522=LKG_525PAA_PAA_1_1.2VDD   +0.65  0.139=IDS 974PD3L   +0.49  12000000000000001364515404906496=RS_525_PO_CS_CHAIN_16   -0_45  9.556=IBOFF_789PU1L   H0.26  265427892.8=RS_525_PO_CS_STACK_3   0.21  530855785.6=RS_789_PO_CS_STACK_4  0.051=IDS_974PG1_5L  -0.279=VTS_789PU_1_R   D1  153 other features  -0.33  30   35   4S   S0  E[f（x)]=2.548     ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/472d3466-2eaf-4fbd-a973-7c3a2d856d97/472d3466-2eaf-4fbd-a973-7c3a2d856d97.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215868%3B1743219468&q-key-time=1743215868%3B1743219468&q-header-list=host&q-url-param-list=&q-signature=0b6d286e8c652035e97484154e0b0a4e037df037)
Fig. 6.    Waterfall diagram for low yield wafer analysis

![TI1   TII   III   TVI  Poyy   Poy   PoI  STI  PV  P-Sub     Fig.7.  Fig. 7.    Test  Test   structure  structure   diagram  diagram  RS525POCSCHAIN16  RS_525_PO_CS_CHAIN_16  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c85dc9dd-248e-4990-bc7d-95bfe6fedc4e/c85dc9dd-248e-4990-bc7d-95bfe6fedc4e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215868%3B1743219468&q-key-time=1743215868%3B1743219468&q-header-list=host&q-url-param-list=&q-signature=f14e1fcddc94e5eb02810a0665d57f9ed80237e7)
## V.    C ONCLUSION 

The significance of a meticulous and astute yield  prediction model in conjunction with FA in the contemporary  semiconductor manufacturing industry cannot be overstated.  Such a model serves as an invaluable tool in expediting  production efficiencies and, consequently, in amplifying the  return on investment. This study proposes a WYP model  based on XGBoost. The PSO algorithm is utilized for  simultaneous   feature   selection   and   hyperparameters  optimization, resulting in enhanced model performance. And  the SHAP method is employed to achieve interpretability of  the prediction results and FA of low-yield wafers. The  proposed PSO-XGBoost model helps to identify low-yield  wafers immediately after fabrication and pinpoint the  corresponding WAT failures without necessitating prior  domain-specific expertise. In conclusion, the methodologies  and insights presented in this research offer significant  potential for future research and practical applications in the  domain of AI in semiconductor manufacturing.

## A CKNOWLEDGMENT  

We thank all partners who provided suggestions for this  study. We thank Zhejiang Provincial CMOS IC innovation  Centre for providing the data source for this study.

## R EFERENCES 

[1]   K. J. Kanarik, W. T. Osowiecki, Y. J. Lu, D. Talukder, N. Roschewsky,  S. N. Park, M. Kamon, D. M. Fried, and R. A. Gottscho, “Humanmachine collaboration for improving semiconductor process  development,”  Nature , vol. 616, no. 7958. pp. 707–711, 2023.    [2]   M. Khakifirooz, C. F. Chien, and Y.-J. Chen, “Bayesian inference for  mining semiconductor manufacturing big data for yield enhancement  and smart production to empower industry 4.0,”  Applied Soft  Computing , vol. 68. pp. 990–999, 2018.    [3]   B. Waschneck, T. Altenmüller, T. Bauernhansl, and A. Kyek,  “Production Scheduling in Complex Job Shops from an Industry 4.0  Perspective: A Review and Challenges in the Semiconductor  Industry,”  SAMI@ iKNOW , vol. 1793. 2016.    [4]   D.-H. Lee, C.-H. Lee, S.-H. Choi, and K.-J. Kim, “A method for wafer  assignment in semiconductor wafer fabrication considering both  quality and productivity perspectives,”  Journal of Manufacturing  Systems , vol. 52. pp. 23–31, 2019.    [5]   D. Kim, P. Kang, S. Cho, H. Lee, and S. Doh, “Machine learning-based  novelty detection for faulty wafer detection in semiconductor  manufacturing,”  Expert Systems with Applications , vol. 39, no. 4. pp.  4075–4083, 2012.    [6]   S.-K. S. Fan, C.-W. Cheng, and D.-M. Tsai, “Fault diagnosis of wafer  acceptance test and chip probing between front-end-of-line and backend-of-line processes,”  IEEE Transactions on Automation Science and  Engineering , vol. 19, no. 4. pp. 3068–3082, 2021.    [7]   H.-C. Hong, and L.-Y. Lin, “Accurate and fast on-wafer test circuitry  for device array characterization in wafer acceptance test,”  IEEE  Transactions on Circuits and Systems I: Regular Papers , vol. 66, no.  9. pp. 3467–3479, 2019.    [8]   C.-F. Chien, W.-C. Wang, and J.-C. Cheng, “Data mining for yield  enhancement in semiconductor manufacturing and an empirical  study,”  Expert Systems with Applications , vol. 33, no. 1. pp. 192–198,  2007.    [9]   C. K. Shin, and S. C. Park, “A machine learning approach to yield  management in semiconductor manufacturing,”  International Journal  of Production Research , vol. 38, no. 17. pp. 4261–4271, 2000.    [10] C.-W. Liu, and C.-F. Chien, “An intelligent system for wafer bin map  defect   diagnosis:   An   empirical   study   for   semiconductor  manufacturing,”  Engineering Applications of Artificial Intelligence ,  vol. 26, no. 5–6. pp. 1479–1486, 2013.    [11] M. Ghahramani, Y. Qiao, M. C. Zhou, A. O’Hagan, and J. Sweeney,  “AI-based   modeling   and   data-driven   evaluation   for   smart  manufacturing processes,”  IEEE/CAA Journal of Automatica Sinica ,  vol. 7, no. 4. pp. 1026–1037, 2020.    [12] J. Senoner, T. Netland, and S. Feuerriegel, “Using explainable  artificial intelligence to improve process quality: Evidence from  semiconductor manufacturing,”  Management Science , vol. 68, no. 8.  pp. 5704–5723, 2022.    [13] T. Kim, and K. Behdinan, “Advances in machine learning and deep  learning applications towards wafer map defect recognition and  classification: a review,”  Journal of Intelligent Manufacturing . pp. 1– 33, 2022.    [14] H. Xu, J. Zhang, Y. Lv, and P. Zheng, “Hybrid feature selection for  wafer acceptance test parameters in semiconductor manufacturing,”  IEEE Access , vol. 8. pp. 17320–17330, 2020.    [15] D. Jiang, W. Lin, and N. Raghavan, “A novel framework for  semiconductor manufacturing final test yield classification using  machine learning techniques,”  Ieee Access , vol. 8. pp. 197885– 197895, 2020.    [16] D. Jiang, W. Lin, and N. Raghavan, “A Gaussian Mixture Model  Clustering Ensemble Regressor for Semiconductor Manufacturing  Final Test Yield Prediction,”  IEEE Access , vol. 9. pp. 22253–22263,  2021.    [17] Q. Xu, C. Xu, and J. Wang, “Forecasting the yield of wafer by using  improved genetic algorithm, high dimensional alternating feature  selection and SVM with uneven distribution and high-dimensional  data,”  Autonomous Intelligent Systems , vol. 2, no. 1. p. 24, 2022.    [18] R. Zebari, A. Abdulazeez, D. Zeebaree, D. Zebari, and J. Saeed, “A  comprehensive review of dimensionality reduction techniques for  feature selection and feature extraction,”  J. Appl. Sci. Technol. Trends ,  vol. 1, no. 2, pp. 56–70, 2020.    [19] L. Yang, and A. Shami, “On hyperparameter optimization of machine  learning algorithms: Theory and practice,”  Neurocomputing , vol. 415.  pp. 295–316, 2020.    [20] J. Wu, X.-Y. Chen, H. Zhang, L.-D. Xiong, H. Lei, and S.-H. Deng,  “Hyperparameter optimization for machine learning models based on  Bayesian optimization,”   Journal of Electronic Science and  Technology , vol. 17, no. 1. pp. 26–40, 2019.    [21] Y. Qiu, J. Zhou, M. Khandelwal, H. Yang, P. Yang, and C. Li,  “Performance evaluation of hybrid WOA-XGBoost, GWO-XGBoost  and BO-XGBoost models to predict blast-induced ground vibration,”  Engineering with Computers , vol. 38, no. S5. pp. 4145–4162, 2021.    [22] T. Kavzoglu, and A. Teke, “Advanced hyperparameter optimization  for improved spatial prediction of shallow landslides using extreme  gradient boosting (XGBoost),”  Bulletin of Engineering Geology and  the Environment , vol. 81, no. 5. 2022.    [23] B. Tan, Z. Gan, and Y. Wu, “The measurement and early warning of  daily financial stability index based on XGBoost and SHAP: Evidence  from China,”  Expert Syst. Appl. , vol. 227, p. 120375, 2023.    [24] Y. Shi, Y. Cai, S. Lou, and Y. Chen, “Explainable prediction of  deposited film thickness in IC fabrication with CatBoost and SHapley  Additive exPlanations (SHAP) models,”  Appl. Intell. , vol. 54, no. 1,  pp. 246–263, Jan. 2024.    [25] H. Zhu, Y. Wang, K. Wang, and Y. Chen, “Particle Swarm  Optimization (PSO) for the constrained portfolio optimization  problem,”  Expert Syst. Appl. , vol. 38, no. 8, pp. 10161–10169, 2011.    [26] S. M. Lundberg, and S.-I. Lee, “A unified approach to interpreting  model predictions,”  Advances in neural information processing  systems , vol. 30. 2017.    [27] C. Cakiroglu, S. Demir, M. H. Ozdemir, B. L. Aylak, G. Sariisik, and  L. Abualigah, “Data-driven interpretable ensemble learning methods  for the prediction of wind turbine power incorporating SHAP  analysis,”  Expert Syst. Appl. , vol. 237, p. 121464, 2024.    [28] A. Gramegna, and P. Giudici, “SHAP and LIME: an evaluation of  discriminative power in credit risk,”  Front. Artif. Intell. , vol. 4, p.  752558, 2021.    [29] A. Tharwat, “Classification assessment methods,”  Applied computing  and informatics , vol. 17, no. 1. pp. 168–192, 2020.    [30] N. W. S. Wardhani, M. Y. Rochayani, A. Iriany, A. D. Sulistyono, and  P. Lestantyo, “Cross-validation metrics for evaluating classification  performance on imbalanced data,”  2019 international conference on  computer, control, informatics and its applications (IC3INA) . IEEE,  pp. 14–18, 2019.    [31] B. Zhou, P. Jieming, M. Sivan, A. V.-Y. Thean, and J. Senthilnath,  “Quantile Online Learning for Semiconductor Failure Analysis,” in  ICASSP 2023-2023 IEEE International Conference on Acoustics,  Speech and Signal Processing (ICASSP) , IEEE, 2023, pp. 1–5.    [32] Y. Chang, and C. Mastrangelo, “Addressing multicollinearity in  semiconductor manufacturing,”  Quality and Reliability Engineering  International , vol. 27, no. 6. pp. 843–854, 2011.    [33] H. Zhang, D. Qiu, R. Wu, Y. Deng, D. Ji, and T. Li, “Novel framework  for image attribute annotation with gene selection XGBoost algorithm  and relative attribute model,”  Applied Soft Computing , vol. 80. pp. 57– 79, 2019.    [34] J. Guo, L. Yang, R. Bie, J. Yu, Y. Gao, Y. Shen, and A. Kos, “An  XGBoost-based physical fitness evaluation model using advanced  feature selection and Bayesian hyper-parameter optimization for  wearable running monitoring,”  Computer Networks , vol. 151. pp. 166– 180, 2019.

