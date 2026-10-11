---
title: "246_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_e25ebdce092371105d473c9cb3fe213c7295230462135641
file_size: 808441
---

## High-resolution 3D X-ray Microscopy for  Structural Inspection and Measurement of  Semiconductor Package Interconnects   

Syahirah, Mohammad-Zulkifli 1 \*, Bernice, Zee 1 , Gregorich, Thomas 2 , Allen,   $\mathrm{{Gu}}^{2}$  , YanJing, Yang 2 , Terada, Masako 2 Weijie, Lee 3   1 Advanced Micro Devices (Singapore) Pte Ltd, 508 Chai Chee Lane, Singapore 469032  2 Carl Zeiss SMT Inc., 4385 Hopyard Rd, Suite 100, Pleasanton, CA, USA 9458871  3 Nanyang Technological University, School of Materials Science & Engineering, 11 Faculty Ave, Singapore 639977  Phone : +65 67969888 ; Fax :  $+65$   62339080 ; \*Email :  Syahirah.Mohammad-Zulkifli@amd.com

Abstract-   3D X-ray Microscopy (XRM) has become an established  failure analysis (FA) tool for bridging fault isolation and physical  failure analysis (PFA) because it enables the visualization of  defects without destroying the device under test (DUT). Through  workflow improvements, it offers the opportunity to improve  process characterization and device qualifications. This paper  describes the application of new automated scanning and image  acquisition capability for repetitive XRM device inspection in  defined regions of interest (ROI). Results obtained from two test  matrices showed good positioning repeatability meeting accuracy  requirements for both small and medium-sized test vehicles with  fast acquisition times.

## I. B ACKGROUND AND  O BJECTIVES 

3D X-ray Microscopy (XRM) has become an established  failure analysis (FA) tool for bridging fault isolation and  physical failure analysis (PFA), because it enables the  visualization of defects without having to destroy the device  under test (DUT). Furthermore, when using XRM, FA analysts  have better information for determining the best approach to  conduct PFA for root cause analysis. The application of XRM  in advanced packaging FA has been demonstrated and reported  by various groups [1-9].

The advantages of using non-destructive, high-resolution  imaging make XRM an excellent option for routine inspection  of semiconductor package features such as traces, C4 bumps,  and micro-bumps. However, XRM set-up and acquisition times  have limited its proliferation and adoption beyond failure  analysis and manual measurement applications. XRM  workflow improvements offer the opportunity to realize the  efficiency and throughput benefits of automated device  handling for productivity in high-resolution, site-specific  inspection and measurement applications.

The paper describes the application of new automated  XRM scanning and image acquisition capability for inspecting  defined regions of interest (ROI) on multiple identical packages  (i.e., repetitive scanning). Test vehicles were used to validate  the scan position repeatability and accuracy as well as to

demonstrate the ability to execute measurement of identified  features with minimized human intervention and fast time to  results.

## II.   R EPETITIVE IMAGING AND MEASUREMENTS 

A   combination   of   XRM   hardware   and   software  enhancements enables efficient repetitive scanning, image  reconstruction and measurement capability.  Flexibility exists  to uniquely customize workflow aspects to realize optimized  time to results for each type of repetitive sample.  Measurement  results, including critical dimensions (CDs), may be  summarized and exported for further statistical analysis. The  maximum number of semiconductor packages that can be  loaded into the system at one time ranges from 14 up to 70,  depending on sample dimensions.

## III.   T EST  M ETHODOLOGY AND  R ESULTS 

The repetitive-positioning study on repeatability and  accuracy was performed on two sets of test vehicles. Each set of  test vehicles included three identical   $24.5\,\mathrm{~x~}\,24.5\,\mathrm{~x~}\,1.5\,\mathrm{~mm}$  (Small Sample) or  $40\,\mathrm{x}\,40\,\mathrm{x}\,2.3\,\mathrm{mm}$  (Medium Sample) flip chip  packages. For each set of test vehicles, two regions of interest  (ROI) were identified; Corner C4 bumps and Center C4 bumps,  as shown in Fig 1.

![SmallSample   Medium Sample  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9e692737-9486-4cad-8b26-79cf0537ed9f/9e692737-9486-4cad-8b26-79cf0537ed9f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=e3e89b3a0484e981dc2592e3d95e34de5340f724)
Fig 1. ROI for both small and medium sized samples; centre and corner .

Samples were mounted vertically onto sample holders  optimized for automated serial scanning. Prior to establishing  repetitive imaging instructions, the scan parameters affecting  scan speed and image quality of the C4 bumps were identified.

The scans were run with a field of view of 2.8 mm in diameter,  voxel size of  $2.75~\upmu\mathrm{m}$   and a scan time of 30 minutes per ROI.

Repetitive imaging instructions are based on the concept of  protocol creation, where recipes are created to define ROIs and  to register unique feature locations in the sample, thus enabling  automated alignments of the ROIs. Each protocol includes a  tomography recipe that includes all ROIs and one set of unique  location registrations for each ROI.

For each set of test vehicles, the protocol scan was performed  on three samples labeled Sample 1, 2, and 3. For each protocol  scan a standard tomography scan without any registration was  performed on one sample as a baseline measurement.  Subsequently all three samples were then subjected to protocol  scans with registration. The protocol scans were then repeated  three times.

The positioning accuracy and repeatability was determined  by calculating the  $\%$   of FOV offset in X, Y, and Z axes for each  protocol-generated image compared to its baseline image. An  example on the offset measurement of a Small Sample X-Y  offset is illustrated in Fig. 2. In Fig. 2, the Sample 2 scan  deviated by   $1\%$   of FOV in the Y axis and   $2\%$   of FOV in the X  axis.

![1%ofFOV  YOffset  XOffset  2%ofFOV  2S0   Baseline   2S0immm   Sample2  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/892bff8e-3095-4a7f-8eec-4e5947881b4b/892bff8e-3095-4a7f-8eec-4e5947881b4b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=adc93fb49aa34e996e07b6cde76f0d9018c9f67c)
Fig 2. Offset measurement in X-Y axis of sample 2 from baseline.

The   $\%$   of FOV offset measurements for both sets of test  vehicles were tabulated in Fig. 3 and Fig. 4 respectively. The  $\%$    offset measurements for both Small and Medium samples were  observed to be well-within a   $5\%$   offset, suggesting very good  accuracy and repeatability of scan locations.

|No of Scans.|Sample|Remarks|Corner|Corner|Corner|Center|Center|Center|
|---|---|---|---|---|---|---|---|---|
|No of Scans.|Sample|Remarks|(Offset,%)|(Offset,%)|(Offset,%)||(Offset,%)||
|No of Scans.|Sample|Remarks|Y|||X|||
|Scan1|Sample 1 (Baseline)|        Self Testat                Baseline      |09%6|09%6|09%6|09%6|096|09%6|
|Scan1|Sample2|Repeat 1, W Reg vs Baseline |4%6|09￥6|19%6|398|09%6|19%6|
|Scan1|Sample3|Repeat 1, W Reg vs Baseline|09%6|09%6|29%6|096|096|19%6|
|Scan2|Sample 1 (Baseline)|        Self Test, Repeat 2, WReg s                Baseline      |09%6|09%6|09%6|0986|09%6|09%6|
|Scan2|Sample2|Repeat 2, W Reg vs Baseline|49%6|09%6|19%6|39%|086|09%6|
|Scan2|Sample3|Repeat 2, W Reg vs Baseline|09%6|09￥6|29%6|096|09%6|19%6|
|Scan3|Sample 1 (Baseline)|        Self Test,at,                Baseline      |09%6|096|19%6|096|09%6|09%6|
|Scan3|Sample2|Repeat 3, W Reg vs Baseline|59%6|09%6|09%6|398|1%6|19%6|
|Scan3|Sample3|Repeat 3, W Reg vs Baseline|49%6|096|29%6|29%6|09%6|19%6|


Fig 3. Tabulation on the  $\%$   offset measurement for small sample.

Fig 4. Tabulation on the  $\%$   offset measurement for medium sample.

|No ofScans.|Sample|Remarks|Corner|Corner|Corner|Center|Center|Center|
|---|---|---|---|---|---|---|---|---|
|No ofScans.|Sample|Remarks|(offset,%)|(offset,%)|(offset,%)|(offset,%)|(offset,%)|(offset,%)|
|No ofScans.|Sample|Remarks|||||||
|Scan1|Sample 1 (Baseline)|        SelfTestRat W                Baseline      |29%6|19%|09X|29%6|19%6|0986|
|Scan1|Sample2|Repeat 1, WReg vs Baseline|19KG|1%6|1%|186|19G|098G|
|Scan1|Sample3|Repeat1, WRegvs Baseline|2986|1笼|1强|2986|19?6|086|
|Scan2|Sample 1 (Baseline)|        SelfTest, Repet 2,WRg                Easeline      |2986|19%|0X|2986|1986|09?|
|Scan2|Sample2|Repeat2, WRegvs Baseline|0986|19%|0|186|1986|09|
|Scan2|Sample3|Repeat 2, WReg v Baseline|29G|1%6|1粥|2986|19G|1986|
|Scan3|Sample 1 (Baseline)|        SelfTestRatW                Baseline      |29%6|19%|0X|29%6|19%6|0986|
|Scan3|Sample2|Repeat3, WRagvs Baselina |1%6|1%||1%6|19%6|08|
|Scan3|Sample3|Repeat3, WReg vs Basellne|29X6|1著|1强|2986|19￥6|0986|


With good repeatability of RepScan offset measurements  established, a routine automated workflow to inspect the Small  sample at predetermined ROI was developed.

Additionally, a template was successfully set up to auto  measure several interconnect parameters based on RepScan  data from the Small Sample, including the solder bump  stand-off height, solder volume, percentage of voids, and void  volume. Visualization images of these measurements of solder  bumps are shown in Fig. 5, 6, and 7 respectively. A tabulation  of the automated measurements is shown in Fig. 8

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/82f6809c-06ef-4ca5-a06e-78864b1c1574/82f6809c-06ef-4ca5-a06e-78864b1c1574.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=636f5b41fe421785d225a448d7e188fd6195676b)
Fig 5. Visualization image of solder stand-off height measurement.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/af6b619d-8dce-4ec1-8680-80c4e90a55ab/af6b619d-8dce-4ec1-8680-80c4e90a55ab.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=f5afe31cf84816940aa3e524a62ed1e1ddba35c9)
Fig 6. Visualization image of solder volume measurement.

![2496.43  219.10  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ee610c25-8d16-4127-801b-5f0bb5c4d7ae/ee610c25-8d16-4127-801b-5f0bb5c4d7ae.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=6d67ad44814930bbc50d04810a25a0bc562d8873)
Fig 7. Visualization image of solder voids% measurement.

Fig 8. Tabulation of the automated measurement at the predetermined ROI.

|C4Bump|Solder Height (um)|Volume [μm3]|        Void%                0.01      |
|---|---|---|---|
||90.80|650678.82|        Void%                0.01      |
||89.05|651164.15|0.01|
||94.71|652406.07|0.05|
||94.71|656845.57|0.07|
||95.19|658280.33|0.08|
||93.82|662025.94|0.06|
||90.70|662122.21|0.08|
||86.66|666591.63|0.07|
|9|87.44|669088.62|0.07|
|10|87.04|669446.83|0.10|


## IV. C ONCLUSION AND  F UTURE  W ORK 

Results showed good positioning repeatability meeting  accuracy requirements for both the Small and Medium test  vehicles at two positions per test vehicle. In addition, images  acquired from 30-minute XRM scans provide enough  resolution for C4 bump interconnect measurement and solder  volume characterization. This suggests that XRM could be  suitable for routine automated workflows to inspect devices at  predetermined ROI, thus bringing about productivity and  throughput improvements. Future work will include using this  improved inspection workflow to evaluate defects in actual  parts.

## A CKNOWLEDGMENT 

The authors would like to thank colleagues from ZEISS  Process Control Solutions for their technical support during this  study. The authors also thank colleagues from Device Analysis  Laboratory, Advanced Micro Devices (Singapore) for their  support.

$\copyright$  2019 Advanced Micro Devices, Inc. All rights reserved.  AMD, the AMD Arrow logo, and combinations thereof are  trademarks of Advanced Micro Devices, Inc.  Other product  names used in this publication are for identification purposes  only and may be trademarks of their respective companies.

## R EFERENCES 

[1]    F. Altmann and M. Petzold, “Innovative Failure Analysis Techniques for  3-D Packaging Developments,” in IEEE Design & Test, vol. 33, no. 3, pp.  46-55, June 2016.     [2]    L. Sylvester, B. J. Hunter, R. Estrada, “3D X-ray Microscopy: A  Near-SEM Non-Destructive Imaging Technology Used in the  Development of 3D IC Packaging.” 3D Systems Integration Conference  (3DIC), in: Proceedings of the IEEE International, 2013, pp. 1.    [3]     K. Fahey, R. Estrada, L. Mirkarimi, R. Katkar, D. Buckminster, M.  Huynh, “Applications of 3D X-ray microscopy for advanced package  development,” IMAPS 2011 44th International Symposium on  Microelectronics, October 9-13, 2011.    [4]    A. Merkle, J. Gelb, “The ascent of 3D X-ray microscopy in the  laboratory.” Microscopy Today 21(2) 2013, pp. 10–15.    [5]    Y. Sylvester  et al ., “3D X-ray microscopy: A non-destructive  high-resolution   imaging   technology   that   replaces   physical  cross-sectioning for 3DIC packaging,” ASMC 2013 SEMI Advanced  Semiconductor Manufacturing Conference, Saratoga Springs, NY, 2013,  pp. 249-255.    [6]    C. Y. Liu, P. S. Kuo, C. H. Chu, A. Gu and J. Yoon, "High resolution 3D  X-ray microscopy for streamlined failure analysis workflow," 2016 IEEE  23rd International Symposium on the Physical and Failure Analysis of  Integrated Circuits (IPFA), Singapore, 2016, pp. 216-219.    [7]    M. Yazdan Mehr  et al ., "An overview of scanning acoustic microscope, a  reliable method for non-destructive failure analysis of microelectronic  components," 2015 16th International Conference on Thermal,  Mechanical and Multi-Physics Simulation and Experiments in  Microelectronics and Microsystems, Budapest, 2015, pp.1-4.    [8]    C. Y. Liu, P. S. Kuo, C. H. Chu, A. Gu and J. Yoon, “High resolution 3D  X-ray microscopy for streamlined failure analysis workflow,” 2016 IEEE  23rd International Symposium on the Physical and Failure Analysis of  Integrated Circuits (IPFA), Singapore, 2016, pp. 216-219.    [9]    S. Zulkifli, B. Zee, W., Qiu, A. Gu., “High-Res 3D X-ray Microscopy for  Non-Destructive Failure Analysis of Chip-to-Chip Micro-bump  Interconnects in Stacked Die Packages” 2017 IEEE 24th International  Symposium on the Physical and Failure Analysis of Integrated Circuits  (IPFA), Singapore, 2017, pp. 1-5.

