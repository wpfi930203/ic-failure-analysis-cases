---
title: "234_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_62cdf4584fba44e928361e9496e3757b7295230462135641
file_size: 662248
---

Provocation tests, design of experiments and advanced statistical  modeling to estimate product sensitivity to a defect:  delamination failure case study for automotive semiconductors

Corinne Bergès 1 , Jinrong Song 2 , Chi   $\mathrm{He}^{2}$  , Xuejian Qian 2 , Jun Ren 2 , Li Tian 2 , Gaojie Wen 2  and Haus Zhang 2   1 Structured Problem Solving Organization, NXP, Toulouse, France  2 Failure Analysis Laboratory, NXP, Tianjin, China  Email - corinne.berges@nxp.com

Abtract-  During a short period, a malfunctioning happened on  a   manufacturing   equipment   in   which   about   twenty  semiconductor parts for automotive have been submitted on a  process step. A same defect of inter-layer dielectric  delamination was generated but each product showed different  sensitivity to this defect. Failure that was generated was a latent  one and occurred in field, which is fitting with the most serious  situation for a final customer. Knowing how to predict quantity  of failures expected to happen is very critical. Two  semiconductor products for automotive have been specifically  studied: the first one was a valve driver, the second one was an  accelerometric sensor. Purpose was to highlight the main  factors on sensitivity to defect. Was it possible to build a model  from these factors to estimate sensitivity of any impacted  product among the twenty ones ? For that, many technics have  been implemented, from most typical reliability and  provocation tests, until advanced design of experiments and  modeling. Some strong results were obtained, as a model  validated, but above all, in order to fully analyze a failure, to  understand   product   sensitivity,   and   to   assess   risk,  complementarity of typical reliability tests with advanced  statistical technics was definitively proved.

Keywords _ Failure Analysis, Reliability, Field modeling,  Design of Experiments, Product Sensitivity to a Defect

## I. Introduction  

In semiconductor industry for automotive, failure  distribution modeling is performed to study the defect and to  predict the quantity of failures that can be expected later. This  study is often part of a risk assessment, required by the  customer facing a field failure.

When a component has been impacted by several types of  failures, a typical study is to compare models and parameters,  according to the defect. It is tempting to think that knowledge  of the model and of its parameters, could avoid some steps in  a failure analysis. Some papers tried to establish a link  between the value of the scale parameter, β, from a Weibull  distribution, and the defect type [5].

But, what about if, this time, instead to face several failures  for a product, a same failure is observed on several products?  What conclusion could be extracted, from the comparison of  the model parameters for all the products ? However, the case  where a same failure impacts several products is rare: it would  mean that somewhere, there is the same root cause for this  defect.

This rare case happened with a malfunctioning of a  manufacturing equipment in which several products have  been submitted during a process step. Two semiconductor  products for automotive have been specifically studied: the  first one was a valve driver, the second one was an  accelerometric sensor.

## II. Steps of this study  

A first step for this case study is fitting with a full failure  analysis performed on the failing parts.

Then, product sensitivity to failure in field is estimated for  the two products, modeling their field failure distributions:  the models providing the best fitting on data are chosen. The  different parameters of these models are compared between  the two products. Thus, at this step, a link is obtained between  the model parameters and sensitivity to failure in field,  expressed in failure quantity observed (Fig 1.).

![Field   Modeling of   Model type   Product  failures   field failure   and model   sensitivity  observed   distributions   parameters   to defect  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bf1758c4-b121-48d1-93d0-08b617443c67/bf1758c4-b121-48d1-93d0-08b617443c67.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215666%3B1743219266&q-key-time=1743215666%3B1743219266&q-header-list=host&q-url-param-list=&q-signature=26c5efe403ff7799bd4bd43435289d49f0b5ec85)
Fig 1. Link between sensitivity to defect observed in field, and  model parameters obtained from field modeling.

In a next step, reliability tests or more precisely provocation  tests are performed on samples from the two products: it deals  with generating the defect by a specific recipe and with  estimating the failure quantity observed. The concept of  design of experiments (DOE) is used to generate this specific  recipe per test, since a recipe is fitting with several  parameters: using a DOE algorithm allows to cover the full  experimental space. Need for testing different provocation  test recipes comes from the fact that products may be  impacted by the issue root cause, differently, mainly by their  different time spent in the failing equipment.

The provocation recipe could be also calibrated by field  failure rate: for each application case with a same  environment, provocation test results and field failure  quantity would have to be similar (Fig 2.): unfortunately, this  calibration may require a very large sample size in  provocation tests, and failure rate observed in field rarely fits  with only one application in only one environment.

![Fieldfailures   Fieldmodeling   Provocation  observed   result   testrecipe  Different   Yes  calibrated  results?  Provocation   Provocation  testrecipe   testresult  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/51f22a3f-b1fe-4340-8d14-8788ec7ce1ed/51f22a3f-b1fe-4340-8d14-8788ec7ce1ed.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215666%3B1743219266&q-key-time=1743215666%3B1743219266&q-header-list=host&q-url-param-list=&q-signature=ca5e8a916a06e81486e0a0bfeaa707e95dea3f07)
Fig 2. Provocation test recipe could be adjusted so that failure rate  observed from test was similar to the field failure rate.

Then, concept of design of experiments (DOE) is used again  and will benefit to all the products submitted to this  malfunctioning manufacturing step and so impacted by the  defect: factors for this DOE are fitting with design and  application features for a product, and response is  corresponding with provocation results for this same product.  Several products are therefore subjected to a defect  provocation test, and the result of this test is confronted to the  different design and application features: lastly, DOE analysis

allows to build, for any product, a model for failure rate, in  function of design and application features for this product  (Fig 3.).

As provocation test results were previously correlated to  product sensitivity to the defect, a model is therefore available  for sensitivity to this defect for any product.

![Design of Experiments (DOE)  -Factors : design and application features,  provocation test recipe  -Response : provocation test results  Model: sensitivity to defect  DOEresult  = function (level of exposure to  analysis  equipment failure, design, application)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/34887029-1e82-41e7-ab4b-43fca57d075f/34887029-1e82-41e7-ab4b-43fca57d075f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215666%3B1743219266&q-key-time=1743215666%3B1743219266&q-header-list=host&q-url-param-list=&q-signature=89ff5bb13bd1e369d3f66e69a7cdc1d02b804538)
Fig 3. Implementation of a Design of experiments to model  sensitivity to defect

Finally, not only qualitative but also quantitative  predictions on expected failures were possible, from product  characteristics.

This paper describes below the different steps with more  details.

## III. Failure analysis and root cause  

## 1. Failure analysis  

For the two products, different failure signatures were  observed and impacted different functions in the component.  Several failing parts for the two products were submitted to a  full failure analysis, from localization techniques as Emission  Microscopy (EMMI), Optical Beam Induced Resistance  Change (OBIRCH), or micro-probing technics, until a  physical characterization and inspection by Scanning  Electron Microscopy (SEM) or FIB (Focused Ion Beam)  technic [1, 4].

Inter-layer dielectric delamination was observed for the two  products, always at the die edge (Fig. 4, 5).

![2G    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bf8b7798-3138-4853-b20f-164440c61a89/bf8b7798-3138-4853-b20f-164440c61a89.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215666%3B1743219266&q-key-time=1743215666%3B1743219266&q-header-list=host&q-url-param-list=&q-signature=ced25c5f477069c39422db4c278a637498ee23a1)
Fig. 4. Optical view of delaminated areas

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/115e8ada-9805-4466-8fd4-d014954766f2/115e8ada-9805-4466-8fd4-d014954766f2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215666%3B1743219266&q-key-time=1743215666%3B1743219266&q-header-list=host&q-url-param-list=&q-signature=11fae98c77bbe9626a592ba3119905c9c0a4245b)
Fig. 5. SEM picture of an inter-layer dielectric delamination defect

## 2. Failure root cause  

Failure was latent, and happened only in field, but a careful  root cause investigation allowed to correlate the failing parts  to a manufacturing equipment that failed while they were in  manufacturing step. This malfunctioning generated an interlayer dielectric delamination that allowed humidity to  penetrate from die edge. Besides humidity penetration, a  mechanical tension may have increased failure occurrence,  disconnecting vias (Fig. 6).

At this step, it is possible to perform some assumptions  about the factors that could impact sensitivity to this defect  for a specific product.

Humidity penetration that generates this delamination  defect could be made easier by a tensile force that would trend  to separate the different layers of the component: this could  be observed in specific customer’s applications due to, for  example, thermal dilatation stresses.

At the contrary, it could seem that, more layers constitute  the die, more resistance to this separating tensile force will be  provided. Edge seal design may also impact sensitivity to  defect, because a via present in the edge seal can make it more  robust. Areas in edge seals are sometimes for some products  show a high via density, which makes the products less  sensitive to this delamination defect.

Passivation thickness may be also included in the factors  impacting sensitivity to defect, as it is fitting also with a  protection against humidity penetration.

So, failure root cause investigation has allowed to list some  key factors in sensitivity to defect, that will be factors in the  design of experiments to build a full model for sensitivity to  defect.

![Tensile  force  Metal Layer  Inter-layer   Humidity  via   via   penetration  dielectric  via die edge  Delamination  Silicon   defect  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2e3adc8e-56b8-4156-b99a-a73fb21e041d/2e3adc8e-56b8-4156-b99a-a73fb21e041d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215666%3B1743219266&q-key-time=1743215666%3B1743219266&q-header-list=host&q-url-param-list=&q-signature=53b2a22c3a3e0ef2bb9435e39119366e54144420)
Fig 6. Design scheme and delamination defect

## IV. Field modeling with defective subpopulation Frechet  model  

A field modeling performed on the observed field failures  revealed that, for the two products, a same defective  subpopulation Frechet model was providing the best fitting  on input data (Fig. 8, 9) [2,3]. This model did correspond to  the physical phenomenon and failure mode, by its specific  failure rate curve, firstly increasing until a maximum failure  rate, then decreasing. The increasing failure rate portion  aligned to period of time before and just after vehicle sale,  when humidity increased. The decreasing portion fitted with  period of time after vehicle sale, where internal heating by  engine dries out part (Fig. 7). Saying that, it is very easily  possible to imagine that a customer’s application in which the  die is subjected to a higher temperature for example due to a  location closer to the car engine, will make the component  less sensitive to the defect, by drying humidity contained in  it.

![Duration infield (in days)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/efaa060e-e146-4a9f-a401-cf152759f111/efaa060e-e146-4a9f-a401-cf152759f111.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215666%3B1743219266&q-key-time=1743215666%3B1743219266&q-header-list=host&q-url-param-list=&q-signature=b1bb50d7e9cc16d930bf416dfb0829e662ef2f9f)
Fig 7. Failure rate curve for a defective subpopulation model

The three parameters for the models were compared  between the two products: it was obvious that sensitivity to  defect could be estimated through the p parameter.

Observed Cumulative Density Function (CDF)   $\mathrm{F_{obs}(t)}$   is  equal to (Eq. 1):

$$\mathrm{F_{obs}(t)=p\ x\ F_{m}(t)}$$(t)
(1)

where  t is the time of measurement for the lifetime event (in  day),   $\mathrm{F_{m}(t)}$   is the CDF of the mortals and p is the fraction of  mortals (units with the fatal defect) in the total population.

For a Frechet distribution, the CDF is the following one (Eq.  2):

$$\begin{array}{r}{F(t,\upmu,\sigma)=e x p\left[-\mathrm{exp}\left(-\frac{\mathrm{log}(t)-\upmu}{\sigma}\right)\right]}\end{array}$$
(2)

where   $\upmu$  , location, and   $\upsigma$  , scale, are estimated by calculating  the usual maximum likelihood estimations.

Table I is comparing the Frechet model parameters for the  two products studied. A higher sensitivity to defect is clearly  highlighted for the sensor product. Study of location estimate  shows also that maximum failure rate time is farer for the  sensor product than for the analog one. Lastly, scale  comparison allows to conclude that failure rate decreasing  speed is far slower for sensor than for analog part (Fig 10 and  11): this last point is important since it may indicate the period  which new failures could happen during.

![Duration in days  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e10809e0-c76a-4367-ac68-d761a7806a41/e10809e0-c76a-4367-ac68-d761a7806a41.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215666%3B1743219266&q-key-time=1743215666%3B1743219266&q-header-list=host&q-url-param-list=&q-signature=8e59ee5c8cb04eb77faafd22e1d2579cf6ef03be)
Fig 8. Field modeling for the sensor: density probability curve

![Duration in days  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/05a1c81e-8a58-49ea-9fa0-2e0844203a6c/05a1c81e-8a58-49ea-9fa0-2e0844203a6c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215666%3B1743219266&q-key-time=1743215666%3B1743219266&q-header-list=host&q-url-param-list=&q-signature=e3339a3f12025233fea9fb638cc1b4cfd3a7405e)
Fig 9. Field modeling for the analog part: density probability  curve

Table I – Analog product versus sensor one comparison for the field model  parameters

|Parameter|        Location                estimate      |        Scale                estimate      |estimate|
|---|---|---|---|
|        Sensor/Analog                ratio      |||10000|


![Duration in days  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/24af01ca-1f03-4e3d-9ad9-1d18b6aed79c/24af01ca-1f03-4e3d-9ad9-1d18b6aed79c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215666%3B1743219266&q-key-time=1743215666%3B1743219266&q-header-list=host&q-url-param-list=&q-signature=9600f94ba5ae9ddb73db05755a9c42dd04e11854)
Fig 10. Failure rate curve for the sensor part

![Duration in days  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ce1e71e3-0e7f-4a92-90a5-5255ab609c06/ce1e71e3-0e7f-4a92-90a5-5255ab609c06.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215666%3B1743219266&q-key-time=1743215666%3B1743219266&q-header-list=host&q-url-param-list=&q-signature=16cda532c0faa57bee644a46ad95f565d2ea9d44)
Fig 11. Failure rate curve for the analog sensor

## V. Provocation tests  

Full issue root cause study revealed that due to the failing  manufacturing equipment, the impacted parts were as  exposed to phosphorus during a more or less long duration.

So, a provocation test will correspond with exposing the  parts to Phosphorus. The two factors for this issue,  Phosphorus concentration and exposition time, were set  according to a design of experiments (DOE) methodology  where response was the failure rate observed for each  combination of these factors. Which means that reliability has  been linked to the issue factor values.

## VI. Product design and application  

Besides this DOE for provocation tests, design of the two  products were compared in term of number of layers,  passivation thickness, edge seal design: product applications  were also studied, about self-heating level that could dry the  parts and decrease failure occurrence (Table II). Environment  is also taken into account, as a car can be used in a wet or dry  climate.

Table II - Sensitivity factors in term of design, customer’s  application and reliability results to provocation tests (unit: analog  part vs sensor ratio for the figures provided)

|Risk Factor(Ratio)|Analogpart|Sensor|
|---|---|---|
|Number of metal layers|||
|Passivation thickness|Thin|Thin.|
|EdgeSeal|        Less robust (only some                vias in the edge seal)      |        Less robust (only some                vias in the edge seal)      |
|        Mechanical Package                Stress at 125°℃      |||
|        Mechanical Package                Stress at-40°℃      |||
|Fracture Strength|||
|        Relative die stress for                identical package case                overtemperature      |||
|Provocation fail point|||
|Self Heating|||


## VII. Risk model  

From this study and from failure quantity observed, a  function was built to predict product sensitivity to the defect,  according to the product features. Impact of each factor, as  number of metal layers or self-heating, on failure quantity,  was estimated and ranked among the other ones (Fig. 12).

Unfortunately, this delamination defect did not impact only  the two products studied, but about twenty products, analog  products or sensors. The model founded by this study was  applied to the other products and allowed to estimate failure  rate for each one.

## V. Conclusion  

This study implemented many strong concepts in different  areas: provocation tests in reliability, design of experiments  to understand the main factors on sensitivity to defect, field  modeling for a prediction purpose.

This work allowed to extract some interesting conclusions:  defective subpopulation model was highlighted as typical for  an inter-layer dielectric delamination issue; product

sensitivity to defect was found correlated with design and  application features; lastly, it was possible to build a  reliability model to predict failure rate for each product  impacted by this issue.

This last point is maybe the most important one. Whatever  the field issue, it is very important to perform a reliability risk  assessment in term of predictions on the number of pending  failing parts. Final customers will request also regular updates  of these analysis, to validate predictions performed on the  previous one, and to make them still more precise.

It was always difficult to set frequency of these updates,  between too close ones that may make to waste time and too  far ones that may miss a change in field and a failure rate  increase. For the first time, thanks to the sensitivity model  built, it was possible to objectively adjust an updating  frequency, higher for higher sensitivity and for a farer  maximum failure rate time, and this criterium was applied for  the twenty impacted products and their fitting risk  assessment.

Lastly, using statistical methods in this study, reliability  stress test on sampling, design of experiments, advanced  modeling, it was possible to provide all the results within  confidence intervals, which guarantees them in a risk level  defined.

## A CKNOWLEDGEMENT 

The author would like to thank Steven Garling, NXP  Technical Project Manager, for part of data shared in this  paper.

## R EFERENCES 

[1]   Wu M, Wang W, Tian L, Wu C, Fan D, “A novel data analysis  methodology in failure analysis”,  ISDEA 2012     [2]   Bergès C, Goxe J, “Benefits of field failure distribution modeling to the  failure analysis”,  ESREF 2013     [3]   Bergès C, Chandon Y, Soufflet P, ‘’Reliability Analysis From Field  Data And Prediction Models For Customer Risk Assessments: Case  Studies And Strategy’’,  IPFA 2014     [4]   Castignolles M, Zirilli T, Cattey E, Lewenstein J, Schauer S, Liu W,  Chen J, Hammett J and Subramanian S, “Failure Analysis of ILD  Delamination _ Uncovering Multiple Root Causes”,  ISTFA 2015     [5]   Bergès C, Feybesse A and Othman W, “Reliability and risk assessment  from accelerated test result and field modeling: delamination issue case  study for automotive semiconductors”,  IPFA 2016     [6]   Bergès C, Chandon Y, Gubian R, “Innovative methodology for failure  rate estimation from quality incidents, for ISO26262 standard  requirements”,  IPFA 2012     [7]   Barnett TS, Grady M, Purdy KG, Singh AD, “Combining negative  binomial and weibull distributions for yield and reliability prediction”,  IEEE 2006     [8]   Haggag A, Barr A, Walker K, Winemberg L, “Realistic 55nm IC Failure  In Time (FIT) estimates from automotive field returns”,  IRPS 2013     [9]   Alam MM, Suzuki K, “Lifetime estimation using only failure  information from warranty database”,  IEEE Trans Reliab 2009 ;58(4)

![Produced   Manufactured  Yes  EdgeSeal   Mechanical   Application   Ambient   Previous   Self-   Lowr  High field  population   with failing   Design   Stress   Hermeticity   Moisture   failures   Heating   failure risk  equipment   Profile   Level  Mwore   Nofailureor  Compres   Hermetic   Dry   High  robust   failuresatOkm  siwe  Medium  70   70   70   70   70  Risk   Risk   Risk   Risk   Risk    Okm risk   field risk    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5c5d7cfc-546b-478a-b39b-2533a14f64fc/5c5d7cfc-546b-478a-b39b-2533a14f64fc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215666%3B1743219266&q-key-time=1743215666%3B1743219266&q-header-list=host&q-url-param-list=&q-signature=4f14a3af1d0ad992446f3086d47ec4e7bf05b049)
Fig 12. Sensitivity model built on design, application and reliability

