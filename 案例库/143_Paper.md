---
title: "143_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_baff1b0586799dd1f198b1a836a460ea7295230462135641
file_size: 1944162
---

## Robust Package Development for Automotive  Application  

Chng Kheaw Chung, Chew Su Fang, Chua Kok Keng, Xueren Zhang  Device Analysis Lab, Xilinx Asia Pacific, 5, Changi Business Park Vista, 486040 Singapore.  Phone: +65 6407 3000  Email: kcc@xilinx.com

Abstract-   Flip chip ball grid array (FCBGA) packages is becoming  more attractive for automotive applications driven by the high  performance requirement. Stacked vias are widely used in  FCBGA substrate due to higher routing request. The reliability of  stacked vias is challenging when the package is working under  harsh environments, especially for automotive application. In this  paper, the crack issue of stack VIAs encountered during product  qualification will be presented. Failure analysis has been done to  identify the failure, 3D finite element (FEM) simulation has been  carried out to understand the mechanism and to provide guidance  of improvement. Solutions has been implemented in the new  substrate, and the product has been qualified successfully for  automotive application.

Keywords  –  Stacked VIAs, Substrate Defect, Vias Cracks ,  FEM  Simulation

while biasing the device. It is one of the challenging tests to  assure the reliability performance of power device modules in  automotive application. The objective of PTC is to simulate a  device working at an environment. It can screen the latent  defects, and identify design weakness for further improvement.  From the test results, the lifetime of a component, e.g. power  converter, in specific application can be predicted [2].

A case study of a FCBGA product qualification for  automotive will be demonstrated in this paper. Stacked via  cracking issue encountered will be presented. Failure analysis  will be done to identify the failure, 3D finite element (FEM)  simulation will be carried out to understand the mechanism and  to provide the guidance and solutions for improvement.

## II.   T EST  R ESULTS 

## I. I NTRODUCTION 

Flip chip ball grid array packages have been widely used for  consumer and mobile applications, they are still relatively new  for automotive applications. As the automotive industry is  pursuing high performance, low cost packaging solutions, flip  chip ball grid array packages are becoming more attractive  nowadays (Figure 1).

Stacked vias are common used in the substrate of FCBGA.  The purpose of high density stacked vias in substrate is to  reduce package size and decrease the surface of device  mounting. However, high density stacked vias could encounter  reliability issue due to the material mismatch between copper  traces and dielectric materials.

![Substrate   Silicon   Bump   Tid   Underfill  SolderBall  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/625da36f-67eb-4dfa-8211-733f3bdea09f/625da36f-67eb-4dfa-8211-733f3bdea09f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215633%3B1743219233&q-key-time=1743215633%3B1743219233&q-header-list=host&q-url-param-list=&q-signature=64c4e305e44abf1cbd5dee5e6c9736fb8d6a3a84)
Fig. 1 Bare die FCBGA package

For automotive application, according to AEC Q100  specification [1], a set of stringent tests will be carried out for  product qualification, e.g.,   High Temperature Operating Life  (HTOL), Temperature Humidity Bias (THB), Temperature  Cycling (TC), Power Temperature Cycling (PTC) etc. .

Power Temperature Cycling (PTC) is the process of cycling  through extreme low and high temperatures (from -40C to 125C)

Following AEC Q100 specification, all necessary tests for the  bare die FCBGA package   $(19\mathrm{mm}\mathrm{x}19\mathrm{mm})$   have been passed,  except PTC. Several devices reported lower current on several  pins after PTC 2000 hours. Figure 2 shows the curve of current  vs device temperature. As the temperature increase, the device  current will be increased normally. The current of bad devices  dropped significantly when the temperature increase to certain  level. The results seem to indicate high resistance or open  connections, possibly in the substrate or in the die.

![S/N#O01  S/N#O02  S/N#O03  Currentdropwhen  temperatureincrease  Temperature  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/06170f5c-bbf0-4656-9a21-c7f7414316a7/06170f5c-bbf0-4656-9a21-c7f7414316a7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215633%3B1743219233&q-key-time=1743215633%3B1743219233&q-header-list=host&q-url-param-list=&q-signature=9db7f54fe24885c0ae1186db0b87c20f9084e0ba)
Fig. 2 Devices characteristic of current vs. temperature. As the temperature  increase, the device current will be increased normally. It will dropped  significantly when there is failure.

Physical failure analysis was performed on the failure units to  understand the failure mechanism. Firstly, EMMI and OBIRCH  (Optical Beam Induced Resistance Change) analysis were  performed, however no obvious difference between good and  bad units was observed.  With electrical analysis and substrate  layout tracing, the failing pins were identified, and further  localized at the stacked via which was the probable suspect

location, which connecting solder bumps to substrate. Physical  failure analysis was performed on   $\mathrm{S/N}\#001$   by mechanical  cross section on the suspected stacked vias. Scanning Electron  Microscope (SEM) inspection is used to observe the area of  suspected stacked vias. Figure 3 shows the stacked vias and a  crack is revealed. The crack is located at the connection of   $2^{\mathrm{nd}}$    via bottom to  $3^{\mathrm{rd}}$   via pad, which results in poor connection (and  sometime open) between substrate and device, such that lower  current is seen.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fed1f494-ea23-4f3a-90c4-1dc38e9ab5da/fed1f494-ea23-4f3a-90c4-1dc38e9ab5da.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215633%3B1743219233&q-key-time=1743215633%3B1743219233&q-header-list=host&q-url-param-list=&q-signature=a8c9b31d8e4359443774be89f580c89293bce527)
Fig. 3 Mechanically cross section on suspected failure location on S/N#001.  Crack in stacked vias were observed.

For two cases on   $\mathrm{S/N}\#002$   and S/N#003, no clear crack is  seen from mechanical cross-section for suspected stacked vias.   Additional physical failure analysis was continued, with the  following of ion milling. The hairline cracks are visible under  SEM inspection, as shown in Figure 4. The similar failure  mechanism is confirmed for the test failures. Anyway, the  cracks in Fig.4 is located at the   $1^{\mathrm{st}}$   via bottom to 2 via pad  connection.

![厂        craci  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/640dd9f3-1e3a-4827-bfdd-8c30323fe7eb/640dd9f3-1e3a-4827-bfdd-8c30323fe7eb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215633%3B1743219233&q-key-time=1743215633%3B1743219233&q-header-list=host&q-url-param-list=&q-signature=9224ed0bb8dd7a2720b0a0f53284ff245aa82b58)
Fig. 4 Hairline cracks in stacked vias with Ion Milling. Top Image from  S/N#002 and below image from S/N#003

From the reliability tests and PFA, it is confirmed that this is an  intrinsic weakness for the stacked vias in the substrate. Further  work is necessary for product reliability improvement.

##                              III. FEM SIMULATION  

Finite element method (FEM) is current widely used to  understand the package stress behavior during test and  application. A 3D FEM model was created to evaluate the stress  level of stacked vias and to provide the possible the guideline of  improvement. 1 quarter model is built due to symmetry. Due to  large model size, a local-global modeling methodology has  been adopted to model the full package, as shown in Figure 5.

![Packagecente  Global package   Localviamodel  model    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f7f4f956-cf91-4ce8-86a9-5577dbbc9402/f7f4f956-cf91-4ce8-86a9-5577dbbc9402.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215633%3B1743219233&q-key-time=1743215633%3B1743219233&q-header-list=host&q-url-param-list=&q-signature=6cdf9aa048ac3268cbc360e76ac814942cd11abd)
Fig 5 FCBGA FEM model

Conventional stacked vias design was found to be cone shape  i.e. Larger diameter on top and smaller diameter at bottom of  VIA, refer to Figure 6.

![Actualsample   3Dmodel  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b2bdacd9-98cc-4c67-8300-3dfe1ad3fdda/b2bdacd9-98cc-4c67-8300-3dfe1ad3fdda.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215633%3B1743219233&q-key-time=1743215633%3B1743219233&q-header-list=host&q-url-param-list=&q-signature=5b61cd7f801308da8014f6aff29c63da1db7313a)
Fig. 6 Conventional design, cone shape stacked vias

For the original stack via design (Conventional), Figure 7  shows the principal stress level of these stacked vias. It can be  seen that the maximum stress is located at via bottom, which  correlates to the via cracks seen from test. The stress level at  bottom via is approximately 168 MPa.

![（MPa) 92.17 37.1571  14.0794  55.3159  116.552  167.789 Stress Results ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e0167313-8783-4c69-9e39-616a747168db/e0167313-8783-4c69-9e39-616a747168db.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215633%3B1743219233&q-key-time=1743215633%3B1743219233&q-header-list=host&q-url-param-list=&q-signature=42fdafe4440e9473f8f0121c33259ddc5e63230f)
Fig. 7 Cone shape stacked vias having higher stress level at bottom of VIAs.

Hence to reduce the via stress, it was started with enlarge the  via bottom diameter. Thus the conventional cone shape stacked  vias design were replaced by a cylinder shape. 3D FEM  simulation result shows that enlarged via bottom diameter helps  to reduce via stress. Figure 8 shows the improvement design of  stacked vias.

From 3D FEM simulation and design optimization, it is  indicated that the VIAs stress level can be reduced by enlarging  the via bottom diameter. This cylinder shape stacked vias is a  more robust design compared to conventional design (cone  shape). Therefore, the new and improved design has been  proposed and accepted by for product improvement.

The new product lots were built with the new stacked vias  design change. Figure 10 shows the cross section image of  cylinder shape stacked vias. PTC stress test was executed on the  engineering lot to verify the robustness of stack via. After PTC,   no failure was reported by Automated Test Equipment (ATE)  parametric test. Hence, this proven cylinder shape stacked vias  is more robust as compare to conventional design. The FCBGA  product has been qualified successfully for automotive  application.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d401b27a-a3ac-4be6-99fe-4ee9355f3823/d401b27a-a3ac-4be6-99fe-4ee9355f3823.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215633%3B1743219233&q-key-time=1743215633%3B1743219233&q-header-list=host&q-url-param-list=&q-signature=a28dc157f4732f190e57746f7cd0fd80ec8e8cb7)
Fig. 10 Cylinder shape stacked vias design.

![EE  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ff21ccfa-5c58-4054-8a4d-81893dc27f47/ff21ccfa-5c58-4054-8a4d-81893dc27f47.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215633%3B1743219233&q-key-time=1743215633%3B1743219233&q-header-list=host&q-url-param-list=&q-signature=b4560cfae4fe256a405656c5ffd5d4acff66f8c5)
Fig. 8 Improved stack VIA design, cylinder shape.

With the design improvement, the stress level of stacked vias  was decrease by approximate 10 percent. Figure 9 shows the  stress result of cylinder shape stacked vias.

![（MPa) 5.B20  25.B2 49.1843  81768  50.8196  100.822  150.824 StressResults ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/af997031-3444-44b7-9c0e-3747e6cf1995/af997031-3444-44b7-9c0e-3747e6cf1995.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215633%3B1743219233&q-key-time=1743215633%3B1743219233&q-header-list=host&q-url-param-list=&q-signature=027a41ac77fdc4222f4caa76751b3b7c6a4b107d)
Fig. 9 Lower stress level at bottom of VIAs for cylinder shape stack.

## A CKNOWLEDGMENT 

The authors would like to thank their colleagues in Xilinx Asia  Pacific Device Analysis Lab, Reliability Lab and San Jose  Device Analysis Lab for their support.

## R EFERENCES 

[1]    AEC Q100, Automotive Electronics Council, FAILURE MECHANISM  BASED STRESS TEST QUALIFICATION FOR INTEGRATED  CIRCUITS, 2014

[2]    Ui-Min Choi , Member, IEEE, Frede Blaabjerg, Fellow, IEEE, and Søren  Jørgensen, “Power Cycling Test Methods for Reliability Assessment of  Power Device Modules in Respect to Temperature Stress” IEEE  TRANSACTIONS ON POWER ELECTRONICS, VOL. 33, NO. 3,  MARCH 2018.

