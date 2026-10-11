---
title: "322_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_5d9131867fcc9e88bcf599beff8aae697295230462135641
file_size: 233978
---

## An overview of failure analysis expert system based  on Bayesian networks  

Hongjian Wang \* , Liyuan Liu, Zeya Peng, and Youliang Wang  Reliability Research and Analysis Center, CEPREI, Dongguanzhuang Road, Guangzhou, 510610, P.R. China.  \* Phone: +86-20-87053229   Fax: +86-20-87237185   Email:  wanghongjian@ceprei.com

Abstract-   Nowadays, with the products and systems becomes more  complex, it will be more difficulty to process the failure analysis in  the dependability. Besides we can see the great progress in the field  of machine learning, and the joint applications of machine learning  and other fields are becoming more widespread. In this paper we  propose a new function which combine the expert system and  Bayesian networks to failure analysis. This method starts with data  mining which will collect the clear, complete data to a data  warehouse. Then it takes advantage of the Fault Tree and mapping  it to Bayesian networks. At last we use the Bayesian networks and  the statistical data to compute the probability of the failure in  order to take analysis. We give an example to explain how this  model works, and it will get a well performance because of it uses  the data from failure cases and other related data.

Keywords  –  Bayesian networks, failure analysis expert system,  dependability, faulty tree, data mining .

## I. I NTRODUCTION 

Recently the potential of Bayesian networks (BN) and data  mining had been demonstrated for the industrial system,  sophisticated products and the higher performance of the  reliability. The classical reliability evaluation method can not  adapt to the rapid advances of the requirements of the complex  application environment and deeper analysis. The reliability is  quality over time, it means improving reliability will be a full  life process, it may concern the whole progress of the product  manufacture. The dependability area should have prior  probability about uncertainty system, which makes it a  complicated system about design, produce, process, material,  package, environment, stress and organization and human  factors.

![Organization system Organization system  influence  influence Human system  Human system influence  influence Environmentalfactors:  Environmental factors:   Technical system:design,  Technical system: design,  influence  influence temperature,humidity...  temperature, humidity...  produce, process, material produce,process,material    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/677358e7-34a9-4b73-a612-b56340113aa2/677358e7-34a9-4b73-a612-b56340113aa2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215700%3B1743219300&q-key-time=1743215700%3B1743219300&q-header-list=host&q-url-param-list=&q-signature=1667725b1dba132183a1260e17e6b0cdddf66265)
Fig. 1 Context of the complex system to be modeled

It’s usually to simplify the model in the previous reliability  assessment and failure analysis, which assumes that the  conventional failure assessment only on the technical part of the  system, in order to get the effectively result. Obviously, these  simplifying assumptions will abandon many important factors  in reliability. This assumption in no longer valid, according to  the importance of other factors in reliability field and it may  need a very sophisticated graph model which include as much  as possible influence causes.

There are almost many research focus on the uncertain  knowledge in probabilistic system and have been applied to a  variety of realistic problems. Weber [1] proposed an overview  about the trend in reliability, compare the fault tree and  Bayesian networks, Oliva [2] present the same idea and  introduce some application and method which can replace the  traditional fault tree. Khakzad [3] , Li [4] and Langseth [5] also  introduce the Bayesian network and other statistical method  which can be used in reliability. Bobbio [6] has proposed the  method about mapping FT to BN. Concretely, there are almost  some methods on transform fault tree to Bayesian networks  [7][8], and used Bayesian prior probability to estimate the fuzz  reliability assessment or the posterior probability to analysis.

The Bayesian networks can integrate important issues such as  the parameter about design, produce, process, material,  package, environment, stress, then the qualitive information  with quantitative knowledge on varying abstraction levels.  Because of Bayesian networks can model the probabilistic  formalism, it can use our failure analysis expert experience to  construct the statistical model, and represent the uncertain  knowledge by the Bayesian probability. BN is the powerful tool  generalized the complex and abstract reliability model. The  structure of BN is large and the content of it is mainly about  data across the full life cycle of a product, include maintenance,  laboratory test data, environment conditions, feedback data,  experts’ judgment and expertise. The characteristics of BN is  that it can represent the dependences between events and  failure.

Except for the BN, there are many other machine learning  algorithms used in the reliability field, for example, the Markov  chains [9], Petri Networks [10] and other classical clustering,  regression algorithms. All of these statistical algorithms can be  used in the failure analysis expert system and the simple  reliability statistic. But only Bayesian networks have a more  general model to represent the real world. In the failure analysis  expert system [11], the machine learning tools is mainly used in  knowledge acquisition and inference engine modules,

furthermore it’s also the most important part of the system.  These parts collect the data in failure analysis, and use data to  imitate experts’ thinking. Then we can use machine to assist  failure analysis.

## II.   F AILURE  A NALYSIS  E XPERT  S YSTEM   

Failure analysis expert system is the complete system which  integrate all the knowledge across the product life. There are  much experience just stay in separate part such as failure  analysis case library, prior knowledge about reliability,  statistical learning method. What the expert system need is to  incorporate all these issues to generate an assistance failure  analysis system. This expert system mainly includes four  modules: knowledge database and management system,  knowledge acquisition module, basis data warehouse and  management system, inference component.

![Failure  Failure   Inference  Inference   Life  Life  analysis  analysis  component  component  prognosis  prognosis knolowdge  knolowdge  base  base Clustering  Clustering   Data mining Regression  Regression Aprior  Aprior Outlierdetect  Outlier detect ... Data  Data  warehouse  warehouse ETL OLAP...  ETL OLAP... Material  Material   Enviroment  Enviroment  Case library  Case library  Other factors  Other factors library  library  factors  factors ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2578ea27-a7cb-42b1-87c4-a239f2b510f6/2578ea27-a7cb-42b1-87c4-a239f2b510f6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215700%3B1743219300&q-key-time=1743215700%3B1743219300&q-header-list=host&q-url-param-list=&q-signature=f28d3e36f2aefbd0bcff3907e659efb55c12baf4)
Fig. 2 Failure analysis expert system

First of all, we need to collect related data and knowledge  from the basis database, which need to gather data into a coarse  level of database, these data are complete and untargeted, but  it’s fit to the database normal form. Then it will use the  knowledge acquisition module which uses data mining to  extract, transform and load data to abstract layers. In this layer,  the data is based on the special target and objective, the data is  sorted to some particular goals, it will extract interrelated data  in a fine layer, which is convenient to do the machine learning.  Lastly, we get the inference module, this component of system  uses the knowledge database to do some data mining and  statistical machine in order to get the rule of clustering,  classification, outlier detect, association rule, and then we can  need these knowledges to failure analysis, life prognosis in the  very complex and uncertainty multi-relational failure decision  model.

## III. D ATA PREPROCESSING AND MACHINE LEARNING   

In order to take failure analysis, we need a full vector data  include all the related domains across the whole life of system.  Then we can get a coarse level of databases, which can be

refining to a fine level. For example, we have a lot of failure  analysis cases and reports, but it need to be extracted to get the  information and regular data include: failure phenomenon,  failure mode, failure mechanism, failure reason, system or  component information, use information, environment factors  and so on. After that, we can establish a conditional probability  network, which can represent the relations between the factors.

We can subsequently apply the data mining [12] functions to  extract some patterns, correlations, rules of inference and other  knowledge. Vapnik [13] demonstrate how the abstract learning  theory established conditions for generalization which are more  general than those discussed in classical statistical paradigms  and how the understanding of those conditions inspired new  algorithms approaches to function estimation problems.

As we know the generalization of statistical model mainly  included 3 components:

1)    A vector which generated by a fixed distribution  P(x)     2)    Each vector x makes an output y by the supervisor,  according to a conditional distribution function   $\mathsf{P}(y|x)$      3)    A learning machine capable of implementing a set of  functions   $\mathrm{f}(\mathrm{x},\upalpha),\upalpha\in\Lambda$

Then we need to choose from the given functions in the best  possible way. It needs to minimizes the lost function   $\mathrm{L}(\mathbf{y},\mathbf{f}(\mathbf{x},\upalpha))$  , which is discrepancy between the response y and  the response   $\mathbf{f}(\mathbf{x},\upalpha)$   provided by the algorithms. We can give  the risk function to expect loss value

$$\mathrm{R}(\alpha)=\int L(y,f(x,\alpha))d P(x,y)$$
Then we need to find the suitable   $\mathbf{f}(\mathbf{x},\alpha)$   to minimize the risk  value.

As for the specific algorithm Bayesian networks, it use the  probabilities between nodes and statuses to denote the  connection of reason and appearance. The data we gathered is  most about the number of times of each node ant their  connection according to their original FT, and the prior,  posterior probabilities to filling in the conditional probability  table. After we have the entities of each unit of the table, we can  compute the lost function and risk function to get the most  accurate result and the uncertain knowledge.

## IV.   M APPING  F AULT  T REE  T O  B AYESIAN  N ETWORKS   

Fault Tree (FT) is a deductive, structure methodology to  determine the potential causes of an undesired event, referred to  as the top event. The top event is the major causing safety  hazards or economic loss [14]. While the top event is placed at  the top of the tree, the tree is constructed downwards, dissecting  the system for further detail until the primary events leading to  the top event are known. Fault tree analysis (FTA) is a system  analysis technique used to determine the root causes and  probability of occurrence of a specified undesired event. It is a  top-down method to evaluate the risk of a system. FT can be  analyzed both qualitatively and quantitatively. In the qualitative  evaluation, using Boolean algebra, an expression is derived for

the top event in terms of combinations of primary events. In  quantitative part, the probability of the top event is expressed in  terms of the occurrence probability of the primary events or in  terms of the minimal cut-sets.

FMEA is another important method in reliability area. FMEA  is a bottom-up method for the purpose of preventing the  happening of undesired situations. Conversely the FT is a topdown method to get the each leaf nodes’ probability.

Bayesian networks are a widely used formalism for  representing   uncertain   knowledge   in   Artificial  Intelligence[15,16].   They   have   become   the   standard  methodology for the construction of systems relying on  probabilistic knowledge and have been applied in a variety of  real-world tasks[17]. The main feature of the formalism are a  graphical encoding of a set of conditional independence  assumptions and a compact way of representing a joint  probability distribution between random variables.

In a BN, the topology of the network represented by the DAG  (Directed Acyclic Graph) and a quantitative part. The  qualitative part represents a set of conditional independence  assumptions that can be captured through a graph theoretic  notion called d-separation [18].

BN is suitable to express and analyze the uncertain  knowledge based on the bidirectional inference mechanism and  the state description of BN. FT is a logical reasoning using the  graphical interpretation in case of certain condition of event  fault. The FT analysis conducted by a logical diagram comes  into being the cause of a system failure. There is a limit when  FTA is employed in large complex and dynamic system, due to  the assuming constraints. BN has been widely used in the field  of reliability at home and abroad because of the conditional  independence of BN nodes and bidirectional reasoning  mechanism [19]. Due to FT is composed of many gates and  event, and these entities can be easily represented by generic  binary component and the root/leaf node, their link can be  represented by the corresponding CPT. So we can mapping an  FT to a BN.

Here we can see some basic mapping methodology, and how  the gates convert to the nodes in BN.

i.    Events are binary events (working/not working);    ii.    Events are statistically independent;    iii.    Relationships   between   events   and   causes   are  represented by logical AND and OR gates;    iv.    The root of the FT is the undesired Top Event to be  analyzed.

After the given the rule of mapping from FT to BN, we can  see how the OR and AND gate conversed in figure 3. The parent  nodes A and B are assigned prior probabilities, the child node  C is assigned its CPT. Then the OR and AND gates represents  the deterministic casual relationships, all the entries of the  corresponding CPT are either 0s or 1s.

![FaultTree Fault Tree Bayesian NetworksBayesianNetworks C=A or BC=AorB A BCPT: CPT:P(C=1|A=0,B=0)=0 P(C=1|A=0,B=0)=0C P(C=1|A=0,B=1)=0P(C=1|A=0,B=1)=0 A B P(C=1|A=1,B=0)=0 P(C=1|A=1,B=0)=0P(C=1|A=1,B=1)=1 P(C=1|A=1,B=1)=1(a).ORGate (a). OR Gate (b).OR Node (b). OR NodeC=AANDB C=A AND BA BCPT:CPT: P(C=1|A=0,B=0)=0 P(C=1|A=0,B=0)=0C P(C=1|A=0,B=1)=1 P(C=1|A=0,B=1)=1A B P(C=1|A=1,B=0)=1 P(C=1|A=1,B=0)=1P(C=1|A=1,B=1)=1P(C=1|A=1,B=1)=1 (c).AND Gate (c). AND Gate (d).AND Node (d). AND Node](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0392373a-e709-4754-bc87-572795b88ddb/0392373a-e709-4754-bc87-572795b88ddb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215700%3B1743219300&q-key-time=1743215700%3B1743219300&q-header-list=host&q-url-param-list=&q-signature=81a3ba6f4a2221b6be7ff8c37b2ed0015782d7bd)
Fig. 3 The OR and AND gate in FT and BN representation

By the basic convert rules for the gates and other nodes, it is  straightforward to map a FT into a BN. We can see from the  Bobbio [6] that the (k:n) gates, common cause failures, noisy  gates, multi-state variables, sequentially dependent failures.  These can make the model one be more precise, and more  general.

After get the Bayesian Networks, we can then take the  qualitative and quantitative analysis to compute the unreliability  of the TE and the unreliability of the given subsystem. We can  fill in the CPT entries according to their Boolean gates. Usually  the quantitative analysis involves: compute the overall  unreliability of the system, compute the unreliability of each  subsystem, compute the importance of each minimal cut-set.  Moreover, we can obtain other interesting measures which  cannot be evaluated in an FT. What we can obtain from BN and  is not suitable in FT is: unreliability of TE, unreliability of a  given subsystem and so on. BN can be used to take the  diagnostic inference to compute the posterior marginal  probability distribution on each component, compute the  posterior joint probability distribution on subsets of component,  compute the posterior joint probability distribution on the set of  all nodes.

## V.   T HE INFERENCE MODULE OF FAILURE ANALYSIS EXPERT  SYSTEM   

After we get the Bayesian networks model, we can use it as  the inference module of the failure analysis expert system. The  principle of the inference is to use CPT to get all of the failure  reason. Compare to the FT’s severity, we can also use BN to  calculate item’s influence factor. Due to use the Bayesian  principle and posterior probability, it’s easy to compute  incidence rate of each part.

In the top-down process of the BN, it’s a deductive analysis  from failure phenomenon to failure reason and mode. Here it’s  necessary to use CPT which is from the Boolean relation  between the FT gate. This process can get the qualitative result.  Besides we can use the posterior probability about the top event  to decide a most probable reason, this result is from a  quantitative analysis.

In the bottom-up process of the BN, it’s similar to FTA and  FMEA, but due to the BN’s characteristics, we can add any  related nodes include environment, human, organization to the  networks. BN can get more precise and accurate.

## VI.   C ASE  S TUDY 

We use the example FT from GJB768 to explain how our  model works, this case is about the signal switch circuit which  descripted several failure phenomena like circuit short or open.  In order to increase the dependability of the circuit, this circuit  use 4 redundancy switches, each component of the circuit are  assumed binary (work/fail). We can compute each components’  failure rate and the occurrence frequency to obtain the prior and  posterior probability.

![SN1  SW1  S2  SW2 S3  SW3  SWN4  SW4 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/583e772e-26b6-424f-94f9-6e6bc9ca8e92/583e772e-26b6-424f-94f9-6e6bc9ca8e92.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215700%3B1743219300&q-key-time=1743215700%3B1743219300&q-header-list=host&q-url-param-list=&q-signature=802559d5552969eac6bc75601e5a57ca59512a11)
Fig. 4 signal switch circuit

Table I – the meaning of symbol in Fig.5

|Symbol|Event|
|---|---|
|X11|Switch1 open|
|X31|Switch3 open|
|X21|Switch2 open|
|X41|Switch4 open|
|E3|Left component open|
|E4|Right component open|
|E1|Circuit open|
|X12|Switch1 short|
|X42|Switch4 short|
|X22|Switch2 short|
|X32|Switch3 short|
|E7|Right component short|
|E5|Switch1 and right component circuit short|
|E6|Switch3 and left component circuit short|
|E2|Circuit short|
|TE|Circuit fault|


The FT of this circuit and its’ corresponding BN shows in Fig.  5. The mapping methods is followed by the rules which is  mentioned above. The prior and posterior probabilities are  presented in Table II.

![TE TEEL E1 E2 E2EB E3 E E4 E5 E5 E6 E6X11 X11 X31X31  X21XD  X41 X12 E7 X32X32  E之 E7X22 X42 X22 X42X42 X22 x42 X42 x22 X22 x42 X42X11 X31 X21 X41 X12 E7 X32 E7E3 E4 E5 E6E6 E2E1TE](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ba5ecd78-8d85-4878-b652-c01bf86ef5e7/ba5ecd78-8d85-4878-b652-c01bf86ef5e7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215700%3B1743219300&q-key-time=1743215700%3B1743219300&q-header-list=host&q-url-param-list=&q-signature=c9a060cfcdcb63f78a4f521cfb41fee4b458394d)
Fig. 5 FT and its’ mapping BN

Table II – component prior, posterior probabilities

|Prior fail probabilities|Posterior fail probabilities|
|---|---|
|0.001|0.01|
|0.001|0.0001|


$X_{i1}$   and   $X_{i2}$     $\mathrm{(i=1,}2,3,4)$  ) represents the failure about open and  short of switches. Table I shows the failure rate about the prior  probabilities and the occurrence frequency represent the  posterior probabilities of each switch. The forward propagation  on the BN can be use to calculate the unreliability of the TE as  the priori probability is   $\mathrm{P}(F a u l t)=6\times10^{-6}$  .

According to the FTA, we can get the minimal cut-set of this  failure tree:   $\{X_{11},X_{31}\}$  ,   $\{X_{21},X_{41}\}$  ,   $\{X_{12},X_{22}\}$  ,   $\{X_{12}X_{42}\}$  ,   $\{X_{32},X_{22}\}$  ,   $\{X_{32},X_{42}\}$  . In FTA we can only compute the  importance of each component, but in reliability it’s more  suitable to consider the posterior joint probability of all the  components. For example, we can inference by BN to have the  exactly the open circuit fault:   $\mathrm{P}(X_{11},X_{31},X_{21},X_{41}|\mathrm{Fall})=$   $10^{-8}$  .

By the Bayesian networks, we can take advantages of the  model to analysis and quantification of the parameter of  reliability. The backward inference which use the posterior can  make the failure analysis expert system to obtain a complete  reasoning.

## VII. C ONCLUSION 

Bayesian networks is now a very popular methods used for  the complex and huge technique system, in this paper, we  propose the overview on failure analysis expert system and its’  composition. The expert system include data collect module,  data mining module and inference module. Inference module is  the key point of the system. Our paper compares some of the  novel machine learning algorithms, and apply the Bayesian  networks. Because we can mapping FT to BN easily, and BN  can include a complete reliability factors, besides it is a very  general model to represent the real world. Finally we use a case  to explain how our model and analysis system work. We  introduce the prior and posterior probability calculate method  and how to solve the real problem. Expect for  points we talked  before, we should know the BN has some modeling aspects to  deal with, thus, it’s necessary to make BN interoperable with  other tools in order to complement the capabilities of BN to  better represent the characteristics of a system.

## R EFERENCES 

[1]    Weber P , Medina-Oliva G , Simon C , et al. Overview on Bayesian  networks applications for dependability, risk analysis and maintenance  areas[J]. Engineering Applications of Artificial Intelligence, 2012,  25(4):671-682.     [2]    Oliva G M , Weber P , Simon C , et al. Bayesian networks Applications  on Dependability, Risk Analysis and Maintenance[J]. IFAC Proceedings  Volumes, 2009, 42(5):215-220.    [3]    Khakzad N , Khan F , Amyotte P . Safety analysis in process facilities:  Comparison of fault tree and Bayesian network approaches[J]. Reliability  Engineering and System Safety, 2011, 96(8):925-932.    [4]    Li Y F, Huang H Z, Liu Y, et al. Notice of Retraction A novel dynamic  fault tree analysis method[C]// International Conference on Quality. 2013.    [5]    Langseth H , Portinale L . Bayesian networks in reliability[J]. Reliability  Engineering & System Safety, 2007, 92(1):92-108.    [6]    Bobbio A , Portinale L , Minichino M , et al. Improving the analysis of  dependable systems by mapping fault trees into Bayesian networks[J].  Reliability Engineering & System Safety, 2001, 71(3):249-260.    [7]    Chenyu Yao, Dongning Chen, Bin Wang. Fuzzy Reliability Assessment  Method Based on T-S Fault Tree and Bayesian Network[J]. Journal of  Mechanical Engineering, 2014, 50(2):193-201.    [8]    Chengyu Yao, Yingyi Zhang, Dongning Chen, et al. Research on T-S  Fuzzy Importance Analysis Methods[J]. Journal of Mechanical  Engineering, 2011, 47(12):163-169.    [9]    G. W A D. Practical methods for reliability data analysis (Oxford  statistical science series - 14) : J.I. ANSELL M.J. PHILLIPS OXFORD  UNIVERSITY PRESS, Saxon Way West, CORBY NN18 9ES, England.  £ 30.00.(ISBN: 0-19-853664-X). Published 1994[J]. Microelectronics  Reliability, 1995, 35(8):1196-1197.    [10]   Dutuit Y, Châtelet E, Signoret J P, et al. Dependability modelling and  evaluation by using stochastic Petri nets: application to two test cases[J].  Reliability Engineering & System Safety, 1997, 55(2):117-124.    [11]   Langseth H , Portinale L . Bayesian networks in reliability[J]. Reliability  Engineering & System Safety, 2007, 92(1):92-108.    [12]   Han J . Data Mining: Concepts and Techniques[M]. Morgan Kaufmann  Publishers Inc. 2005.    [13]   Vapnik, V. N . An overview of statistical learning theory[J]. IEEE  Transactions on Neural Networks, 1999, 10(5):988-999.    [14]   Lewis EE. Introduction to reliability engineering. 2nd ed. New York: John  Wiley& Sons; 1994.     [15]   Pearl J. Probabilistic reasoning in intelligent systems. Los Altos, CA:  Morgan Kaufmann, 1989.    [16]   Neapolitan RE. Probabilistic reasoning in expert systems. New York:  Wiley, 1990.    [17]   Heckermann D, Wellman M, Mamdani A, editors. Real-world  applications of Bayesian networks. Communications of the ACM  1995;38(3).    [18]   Pearl J. Probabilistic reasoning in intelligent systems. Los Altos,  CA:Morgan Kaufmann, 1989.     [19]   Su H , Che Y . Reliability assessment of CTCS-3 using Bayesian  networks[C]// 2013 International Conference on Quality, Reliability,  Risk, Maintenance, and Safety Engineering (QR2MSE). IEEE, 2013.

