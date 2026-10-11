---
title: "232_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_94d7ff5a481bfd7b5a04c01e12b34ea47295230462135641
file_size: 1120677
---

## Reliability hazard characterization of wafer-level  spatial metrology parameters based on LOF-KNN  method  

Jinli Zhang, Hailong You, and Renxu Jia  Institute of Microelectronics, Xidian University, Xi'an, Shaanxi  \*  Email: jlzhang95@163.com

Abstract-   This paper presents a new method for characterizing  device reliability hazard by using wafer-level spatial analysis. The  method is based on the combination of the LOF algorithm and  KNN algorithm, which can effectively identify and quantify the  reliability of the device and detect local outliers. Outlier devices  often have serious reliability hazard. This approach takes into  account variations in device measurement data due to process  variations on the wafer, increasing device reliability and saving  cost. The method is verified using the electrical parameter  measurements of devices. The results are compared with  traditional method.

Keywords  – Wafer-level spatial analysis, Reliability hazard,  Detect outliner, LOF, KNN

## I. I NTRODUCTION 

The spatial variation of device performance is introduced by  the nature of the fabrication processes, along with pattern  dependent effects. Most semiconductor processes exhibit  spatially revolved variation. The electrical metrology data is  spatially distributed across all the dies within the same wafer.  Defects are inevitably introduced during the manufacturing  process of the devices. Many defects do not directly cause hard  fail, but bring quality or reliability risks. The normal process  has certain continuity, so the wafer measurement parameters  data are gentle in spatial variation. Anomalous devices caused  by defects/materials or design reasons could behave as  abnormal outliers in certain dimensions. A large number of  experiments have proved that outlier's devices often exhibit  small Margin, BI fail, early failure and other phenomena [1],  and there are great chances of reliability hazard. Therefore, the  local outlier of wafer which considering spatial level analysis is  the focus of reliability hazard detection [2][3].

In this paper, a LOF-KNN-based scheme is proposed to  identify abnormal data by wafer-level spatial parameter  analysis and to detect devices with reliability hazard. The  method considers the influence of parameter fluctuations in the  local area of the wafer, which is more sensitive to the local  outlier of a single device. The accuracy and stability of the  identification are effectively improved. Furthermore, the  scheme is fast in calculation, the statistics and the raw data are  in one-to-one correspondence, which facilitates subsequent  data analysis. The program uses the idea of unsupervised  learning, not based on any mathematical model, has a wider  range of application. The method is verified using wafer  measurement data for devices.

## II.   H YPOTHESIS AND  METHOD  

## Hypothesis  

The traditional approach has been to define a maximum  permissible value or a minimum permissible value for  parameter, called “parameter Threshold”. All devices having a  vector with parameter higher or lower than “parameter  Threshold” are considered likely to be defective and are either  rejected or subjected to burn-in test. All devices that meet the  requirements pass the parametric test.

However, as the product yield increases, the reliability  requirements of the device become higher and higher, and this  method has serious problems.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/82e11ee0-0f33-44f1-8c62-4a99fb7f3e7c/82e11ee0-0f33-44f1-8c62-4a99fb7f3e7c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215666%3B1743219266&q-key-time=1743215666%3B1743219266&q-header-list=host&q-url-param-list=&q-signature=42b4a51fe085fe5aa0fffe892f3194cef6de2707)
Fig. 1 Typical distribution of chip parameters

A typical distribution of devices parameter values is shown in  Fig.1. Some die can't pass the parameter test, such as the red  dot, which are global exception, but some die pass the  parameter test but have reliability hazards, such as blue dot,  which are local exception. A local abnormal die that pass the  parameter testing but has a reliability hazard which will reduce  device reliability and increases production costs. Therefore,  semiconductor manufacturers need to define metrics for device  parameter pass/fail decisions very carefully [4].

It is suggested that the presence of a defect should result in a  “step” in the current signature, instead of a gradual change as in  the case of a good die. The KNN-LOF scheme proposed in this  paper is based on the assumption that the wafer-level spatial  measurement parameters data are correlated, and the spatial  variation are stable due to the stability of the process. Any  abnormal spatial changes may be caused by reliability hazards  or defects [5]. In a sense, device that is located close to each  other on the same wafers will have more similar performances  than ones far away. If a die has parameter considerably higher  than its neighbors (i.e. a high-frequency spike) ,it is likely to be

a defective. On the contrary, if a die has very low parameter  compared to its neighbors (a negative spike), it is also likely to  be defective. Due to the continuity of the space, the abnormal  peak which is a greater probability caused by the unknown  defect and has greater probability in the reliability hazard.

## Method  

The main idea of the LOF-KNN algorithm is to first calculate  the neighbour difference statistics of data points by using KNN  algorithm, and then use the LOF algorithm to obtain the local  anomaly factor [6]. Finally, the threshold LOF_L, which is the  control limit, is determined for fault detection. If the detection  index LOF exceeds LOF_L, the test data is considered to be  abnormal data; otherwise, the test data is normal data.

The basic steps of abnormality detection based on LOF-KNN  for judging whether a data point is normal are as follows:

Step1 ：  A coordinate system is established for the wafer data  to determine the position of each die.

Step2 ：  According to the equation (1), the squared difference  K2 of the neighbourhood differences is calculated to represent  the spatial variation difference of the data i.

$$K2(i)\!=\!\sum_{j=1}^{k}\!d_{i j}^{2}\,/\,k$$
(1)

Where: k is the number of neighbours of the data   $\mathrm{i},d_{i j}^{2}$   is the  square of the difference between the parameter i and its jth  neighbour.

The King-move neighbours used in this article are common  neighbourhood definitions in spatial statistics [7], as shown in  Fig.2.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a560daf7-0738-4b2d-9295-3516d764955c/a560daf7-0738-4b2d-9295-3516d764955c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215666%3B1743219266&q-key-time=1743215666%3B1743219266&q-header-list=host&q-url-param-list=&q-signature=945b5648f135e2ec0bb3d57c8e965064fb992a57)
Fig.2 King-move neighbors

Step3 ：  According to equation (2), the local outlier factor  LOF is calculated to characterize the degree of local outlier of  the data i.

(2)

$$L O F(i)\!=\!\frac{k^{*}K2(i)}{\displaystyle\sum_{f=1}^{k}\!K2(\mathbf{x}_{i}^{f})}$$
Where,   $\mathbf{X}_{i}^{f}$    is the fth neighbour of data i.

If the local outlier is much larger than 1, it means that the  spatial variation of data i is much larger than the difference of  its neighbour’s, and it is more likely to be an abnormal point.

Step4 ： Determine the control limit LOF_L for anomaly  detection and mark the abnormal data.

The appropriate control limit needs to be set. A loose control  limit will miss a large amount of abnormal data, and a strict  control limit will greatly reduce the output. Therefore, the data

limit that slightly lower than the pass rate of   $1\%$   is generally  selected as the control limit.

If the local outlier factor LOF statistic of data i is greater than  the control limit, the data is marked as an abnormal data.

Because the method is not based on any a priori mathematical  model, the scope of application is broader. Also, local  neighbourhood-based anomaly detection makes it more  sensitive to local outliers of single point. However, it should be  noted that this method can only deal with the spatial correlation  of die parameters too.

## III. R ESULTS AND ANALYSIS   

## Measurement parameter basic informations  

This paper uses the VTH measurement data of an 8-inch  MOSFET device to verify and discuss the algorithm in this  paper.

The wafer level space measurement data is electrical  performance test data of the MOSFET, and the electrical  parameter is VTH. The test result specification is Min Limit:  2.6000V, Max Limit: 4.400V; a total of 2270 data, 22  non-compliant data.

## Process and results  

According to the method mentioned in the previous section,  the wafer data is processed to detect reliability hazards in the  data. The process and results are as follows.

As shown in the Fig3, a coordinate system is established for  the wafer data. The parameter value of the die is Z value, and  the picture is a top view.

![15   25   45  5055  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/aca5dcd0-f782-4d0e-b7a5-d05141d63843/aca5dcd0-f782-4d0e-b7a5-d05141d63843.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215666%3B1743219266&q-key-time=1743215666%3B1743219266&q-header-list=host&q-url-param-list=&q-signature=f1c5eba4a92df2e671103b296f7356dc23ad2291)
Fig. 3 Wafer raw data with coordinates

As shown in the Fig4, the statistic K2 values are calculated.

![50  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/83ac61d1-27e2-4773-b443-65f0cf4550e4/83ac61d1-27e2-4773-b443-65f0cf4550e4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215666%3B1743219266&q-key-time=1743215666%3B1743219266&q-header-list=host&q-url-param-list=&q-signature=fd808f6b2b5ab579b9451cb7ab09613c174c4dce)
Fig. 4 KNN statistic results graph

As shown in the Fig5, the statistic LOF values are calculated.  The abnormality data is the measurement parameter whose  LOF value exceeds the control limit.

Because the control limits cannot be set based on known  experience, they can only be based on a reduction budget that

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fad1ad7c-0869-4d17-8443-5ca69fe82eff/fad1ad7c-0869-4d17-8443-5ca69fe82eff.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215666%3B1743219266&q-key-time=1743215666%3B1743219266&q-header-list=host&q-url-param-list=&q-signature=d9eabd993c954e3e28a66e0a9da8a3362a6b0c58)
Fig.5 LOF statistic results graph

can be tolerated. Considering that the pass rate of this wafer is  about   $99.03\%$  , the control line is set to   $98\%$  . Calculate the  control limit corresponding to the   $98\%$  , the upper limit of  control is LOF_L=3.1229.

## Analysis  

The detected abnormal data are divided into two types:  non-compliant data and data with reliability risks. The results of  these two types’ abnormal detection data are analysed  separately below.

The non-compliant data are VTH voltage values less than  2.6V or greater than 4.4V. All non-compliant (22) data are  detected by the LOF-KNN program without any omissions.

Table.1 Non-compliant data

|||Lvalue|LOFvalue||||Lvalue|LOF vslue|
|---|---|---|---|---|---|---|---|---|
|||0.024|6.45284||||0.188|7.99983|
|||0.192|5.79708||28||0.227|7.99994|
||29|1.104|7.99985||30||1.182|7.99992|
||16|0.669|7.99976||||0.076|7.99995|
||48|0.082|7.20407|16|36||0.006|6.30782|
|||0.005|6.30466||36||1.621|7.99982|
|||0.069|7.99995|18|||1.410|7.99990|
|16||0.052|7.99994|19|99||0.353|3.38171|
|||0.581|7.99991|||13|0.257|3.61864|
|||0.117|7.99994||||0.180|7.99969|
||A8|0.153|7.99991|||30|1.614|7.99990|


As shown in the Table.1, it can be preliminarily proved that  the LOF-KNN scheme has the possibility of replacing the  traditional data specification detection scheme.

Table.2 Data with reliability risks

|||Lvalue|LOF value||||Lvalue|LOF value|
|---|---|---|---|---|---|---|---|---|
|13||3.400|3.57700|13||32|3.419|3.68292|
|13||3.401|3.75141|||2S|3.421|3.97526|
|||3.417|3.12288||||3.437|4.68291|
|16|18|3.419|3.17259|16||SO|3.449|3.27589|
|||3.406|3.39622||||3.419|4.29507|
|18||3.424|4.91253|18|36|0|3.423|3.53339|
||26|3.415|4.24174|9|38|16|3.424|3.16964|
|||3.418|3.43683||||3.420|3.42583|
|26||3.419|3.80681|||2S|3.404|4.71720|
|26||3.420|4.11635||46||2.832|6.18307|
|||3.420|4.30890|2S|S|18|3.331|3.75147|
|||3.436|3.02210||||3.315|3.28354|


As shown in Table 2, the following are the data with  reliability risks detected in the LOF-KNN scheme. These data

meet the specifications but the LOF values exceed the control  limit.

The following section analyses some of the data to prove the  effectiveness of the scheme.

From the perspective of global, the appeal data are normal  data; the VTH voltage values are greater than 2.6V and less  than 4.4V which meet the specification requirements. Select the  data points as 6, 12, 18, and 24 and compare it with local data.  The graphical results are shown in Fig.6:

![(18.12)  (18,12) 3.437 3.433 3.429 3.425 12 13  18  (a)(18,12) (a) (18,12) (27,15)  (27，15) 3.443 3.438 3.433 2 26  26   (b) (27,15) (b) (27,15) （36，20)  (36，20) 3.430 3.425 3.420 20  37 36 35  35   （(c）(36,20) c） (36,20) (53.34)  （53,34) 3.37 62 333 3.32 3.31 53 52  52   (d) (53,34) (d）（53.34) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/84fb33c3-508e-4fb9-a8db-5bdfe296cf05/84fb33c3-508e-4fb9-a8db-5bdfe296cf05.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215666%3B1743219266&q-key-time=1743215666%3B1743219266&q-header-list=host&q-url-param-list=&q-signature=f220935b3a13dfaed9ba9c80f4d11e30d01c1ba6)
Fig.6 Comparison of raw data and result data of  6-(a), 12-(b), 18-(c), 24-(d)  The left side of the graph is the raw data, and the right side is  the corresponding LOF value. As shown in Table 3, the specific  values of the raw data are displayed.

Table.3   Specific data of 6-(a), 12-(b), 18-(c), 24-(d)

|X/Y|11||12||13||||X/Y||14||15||16|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|17|3.433||3.430||3.432||||26||3.442||3.442||3.437|
|18|3.432 3.424||||3.434||||27||3.443 3.436||||3.438|
|19|3.435||3.433||3.437||||28||3.442||3.439||3.440|
|(a) (18,12)  (b) (27,15)|(a) (18,12)  (b) (27,15)|(a) (18,12)  (b) (27,15)|(a) (18,12)  (b) (27,15)|(a) (18,12)  (b) (27,15)|(a) (18,12)  (b) (27,15)|(a) (18,12)  (b) (27,15)|(a) (18,12)  (b) (27,15)|(a) (18,12)  (b) (27,15)|(a) (18,12)  (b) (27,15)|(a) (18,12)  (b) (27,15)|(a) (18,12)  (b) (27,15)|(a) (18,12)  (b) (27,15)|(a) (18,12)  (b) (27,15)|(a) (18,12)  (b) (27,15)|(a) (18,12)  (b) (27,15)|
|X/Y|19||20||21||||X/Y||33||34||35|
|35|3.430||3.425||3.427||||52||3.377||3.370||3.362|
|36|3.429 3.423||||3.427||||53||3.339 3.315||||0.000|
|37|3.427||3.428||3.427||||54||0.000||0.000||0.000|


It can be analysed from the appeal data table and graph that  the detected data have significantly higher die parameters than  its neighbour’s (ie, high frequency spikes) or significantly  lower than its neighbour’s (negative spikes).

Since the normal process has certain continuity, the wafer  data are gentle in spatial variation. Anomalous dies caused by  defects/materials or design reasons will appear as outliers in  some dimensions. Although the above data meet the  specifications, they all form abnormal peaks. Due to the  continuity of space, anomalous peak has a greater probability of  defects due to unknown causes and have a greater chance which  is a reliability hazard. Therefore, the LOF-KNN detection  scheme can effectively detect reliability hazards.

## IV. C ONCLUSION 

In actual production, chips that fail the wafer test will be  rejected. Because too few people can prove that the cost of  additional packaging and testing is reasonable, and the  reliability risk is dangerous. The philosophy behind using  spatial information is that not all die that can't pass the  parametric test are bad and not all die that pass all tests are good.  The wafer level spatial measurement parameter anomaly  identification scheme can effectively screen and evaluate the  reliability of the device. It can not only reduce the production  cost, but also improve the reliability of the device.

This work has demonstrated that the use of spatial  information for reliability hazard detection is a valuable  technique that allows us to consider process variations while  detecting fault-free parameter values. In future test scenarios,  spatial information can be correlated to reduce early failure  rates.

## R EFERENCES 

[1]    R. Madge, M. Rehani, K. Cota and R. Daasch ,“Statistical post-processing  at wafer sort: an alternative to burn-in and a manufacturable solutions to  test limit settling for submicron technologies ,” Proc. 20th IEEE VLSI Test  Symp. (VTS’02) , pp. 69-74, May 2002.    [2]    W. R. Daasch et al. “Variance Reduction Using Wafer Patterns in IDDQ  Data,”  Proceedings International Test Conference 2000 , pp. 189-198,  Oct. 2000.    [3]    W.R. Daasch et al., “Neighbor Selection for Variance Reduction in IDDQ  and Other Parametric Data,”  IEEE Intl. Test Conf  , pp. 92-100,Oct. 2001.    [4]    S. Sabade and D. M. H. Walker, “Improved Waferlevel Spatial Analysis  for IDDQ Limit Setting,”  IEEE Intl. Test Conf .,  pp. 82-91, Oct. 2001.    [5]    Fang L , Lemnawar M , Xing Y ,”Cost Effective Outliers Screening with  Moving Limits and Correlation Testing for Analogue ICs[C]”  IEEE  International Test Conference. IEEE , pp. 92-100, Oct.2006.    [6]    Kang B , Kim D , Kang S H ,”Real-time business process monitoring  method for prediction of abnormal termination using KNNI-based LOF  prediction[J],”  Expert Systems with Application s, pp. 6061-6068, April.  2012.    [7]    Frommelt, Ester, M., A., Kriegel, H.-P., and Sander, J, ”Algorithms for  Characterization and Trend Detection in Spatial Databases”,  Proc. 4th Int.  Conf. on Knowledge Discovery and Data Mining , pp.44-50, August.1998.

