---
title: "129_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_64a192323716e0855590fdc2638800557295230462135641
file_size: 3058496
---

## Research on Failure Mechanism of SerDes PhaseLock-Loop (PLL) Lose Lock  

Xixiong Wei 1,2 , Xinyi Lin 2 , Shuanshe Chao 2 , Yaping Huang 3 , Dan Yang 2 , Na Mei 1 , Jie   $\mathrm{{H}u^{3}}$    1  State Key Laboratory of Mobile Network and Mobile Multimedia Technology, Shenzhen, China    2 Department of Reliability Engineering, Sanechips Technology Co., Ltd., Shenzhen, China  3 Department of analog design, Sanechips Technology Co., Ltd., Shenzhen, China  Phone : (+86)13423645766, Email :  wei.xixiong@sanechips.com.cn

Abstract —With the continuous improvement of chip  performance,   the   requirement   of   Serializer-Deserializer  (SerDes) performance is becoming higher and higher, faster  transmission rate and lower power consumption, etc. The  improvement of SerDes performance means more complicated  structure accordingly and more challenges for failure analysis  (FA). The paper analyzed the SerDes PLL lock loss case, which  utilizing the FA method of dynamic emission microscope  (dynamic EMMI), Conductive Atomic Force Microscope (CAFM) and Nanoprobe to successfully found out the root cause  of the failure and made an in-depth analysis of the failure  mechanism. With the methods of circuit simulation analysis,  circuit design issue is found and resulting in the risk of  overvoltage in the use of the device, which eventually leads to  the PLL lose lock.

Keywords—PLL lose lock, Dynamic Emission Microscope,  Conductive Atomic Force Microscope, Nanoprobe, Design for  manufacturability

## I.    I NSTRUCTIONS 

With the continuously rapid development of SerDes  technology, its structure has become more and more complex  [1]. Therefore, the FA for SerDes is also facing more  challenges. The circuit structure of SerDes is shown in Fig. 1  PLL generates a high-speed clock signal. If PLL is un-locked,  it will have a serious impact on the function of SerDes. For the  analysis of the PLL lose lock problem, because there is normal  in its static characteristics, the conventional FA method cannot  find out the root cause.

![chann  TX   zlea   RX  data   data  PLL   TXcIk   RXcIk   CDR  refclk  RXcIk  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d3fce3ac-931c-4bff-91cb-cd9ddd141d58/d3fce3ac-931c-4bff-91cb-cd9ddd141d58.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215837%3B1743219437&q-key-time=1743215837%3B1743219437&q-header-list=host&q-url-param-list=&q-signature=6035892e97779784b91e962b4e1ef9dcb661c8cd)
Fig. 1.   SerDes structure diagram

Through the analysis of SerDes PLL lock loss case, this  paper digs out the design risks and defects on SerDes IP. First  of all, with the test method of reference [2], dynamic EMMI  test environment was built up to locate the failure position,  which helps to find out the failure module is   $1^{\mathrm{st}}$  stage low  dropout regulator (LDO) boost circuit. After the sample was  delayer to the contact layer, the region of interest (ROI) was  further to narrow down by C-AFM technology [3], then found  out the NMOS have abnormal leakage between S/D and the  substrate. Combined with the layout information, the  abnormal electrical properties of the device could be tested by

nanoprobe. Finally, with the circuit simulation analysis, the 1 st stage LDO boost circuit was found to have the design defect,  which leads to the risk of overvoltage of the devices when the  chip is working normally and seriously affects the life of the  chip.

## II.    C ASE  S TUDY 

After using the chip for a six months to one year, there was  SerDes functional failure, its particular characterized by  Transmit (TX) PLL and Receive (RX) PLL lose lock. As  shown in TABLE I. , the power consumption of the failed unit  SerDes is lower, but the I-V curve of relevant pins is normal.  In this way, it can only locate the failure position with dynamic  EMMI analysis.

As shown in Fig. 2, the test environment was set up to  combine automatic test equipment (ATE) 93K, male board,  loadboard and socket [2]. The test pattern will be load to chip  and make it working in specific state. And then, the InGaAs  camera will capture the photons emitted by chips in specific  states. The results of good unit are also obtained through the  same method, allowing good unit to work in the same state.  The dynamic EMMI results both bad unit and good unit will  be compared in the same area.

TABLE I.     S ER D ES  P OWER  D ISSIPATION

|Sample|SerDes state|SerDes state|SerDes state|
|---|---|---|---|
|Sample|Download MCU (normalization)|Initialization (normalization)|Download FW (normalization)|
|NG1|0.47|0.73|0.4|
|NG2|0.44|0.81|0.3|
|Good unit|1|1|1|


![eia  oaxia  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b9c3b811-bfe3-4aed-b4f5-a7baaf713e35/b9c3b811-bfe3-4aed-b4f5-a7baaf713e35.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215837%3B1743219437&q-key-time=1743215837%3B1743219437&q-header-list=host&q-url-param-list=&q-signature=b6bb7c649aef15a31ead641706e4120bbb3d3705)
Fig. 2.   Dynamic EMMI test environment [2].

Dynamic EMMI results are shown in Fig. 3 (a) bad unit  and Fig. 3 (b) good unit. After comparing dynamic EMMI  results of good unit and bad unit, we find that red box area of  bad unit has photon emission, while the good unit have no  photon emission at the same area. It’s mean that there may be  leakage current or other abnormal in this area. Therefore, the  failed module was located within the red box of Fig. 3 (a).  Based on the layout information, we can know the ROI 1 is  the LDO of TX PLL, and  ROI 2 is the LDO of RX PLL. We  suspected the LDO circuit has damage or defect.

![an  nparisoi  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/83f838d6-e9c0-4496-ad80-0b5b9ff038c2/83f838d6-e9c0-4496-ad80-0b5b9ff038c2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215837%3B1743219437&q-key-time=1743215837%3B1743219437&q-header-list=host&q-url-param-list=&q-signature=c78e1905c6fb2ae41084732c2fccb26eeeff5aac)
Fig. 3.   Dynamic EMMI results both  (a) failure unit and (b) good unit.

In order to identify the root cause of this issue, we  conducted layer by layer analysis on ROI 1 and ROI 2, from  aluminum pad (AP) layer to the contact layer. As shown in Fig.  4 (a), these delayer results of contact layer indicates that there  is no abnormalities were found, such as burn mark, crack, and  so on. May be the defect or damage is too small to be observed  under OM. As show in  Fig. 4 (b), the dynamic EMMI results  of ROI 1 was superimposed on the corresponding layout.  Thus, we can observe that the position of the abnormal module  more clearly. And the red box area is the boost circuit of TX  1 st  stage LDO.

![ap  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cf3870a4-6803-48cd-853e-09b83e097e99/cf3870a4-6803-48cd-853e-09b83e097e99.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215837%3B1743219437&q-key-time=1743215837%3B1743219437&q-header-list=host&q-url-param-list=&q-signature=00fd08607ae8bc845d502d94f5bfa9d4031b85bd)
Fig. 4.   (a) Delayer results in Contact layer, (b) superimposed image of  emission image and Layout.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b55790ce-9981-4204-91e0-ba34b97750a7/b55790ce-9981-4204-91e0-ba34b97750a7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215837%3B1743219437&q-key-time=1743215837%3B1743219437&q-header-list=host&q-url-param-list=&q-signature=6690d6fe93168216db8647fbc76ad1d6e9dc699a)
Fig. 5.   (a) Layout information of ROI 1, (b) Active area of ROI 1.

For narrow down ROI, device-level positioning is carried  out through passive voltage contrast (PVC) and C-AFM  technology. Prior to this, we need to obtain the key layout

information of ROI 1. The layout information has shown in  Fig. 5. And then, the PVC analysis was conducted on the  active area of ROI 1, and the results was shown in Fig. 6. No  obvious difference was found between abnormal area and  normal area. Perhaps because its electrical performance did  not show obvious open or short issues, PVC was unable to  locate the failure location.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5d828656-535c-4b17-b68b-ac28815669f5/5d828656-535c-4b17-b68b-ac28815669f5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215837%3B1743219437&q-key-time=1743215837%3B1743219437&q-header-list=host&q-url-param-list=&q-signature=e6ea4352344583d970fd6a2ba5fbbc79b60c6b0b)
Fig. 6.   PVC results of active area.

The ROI 1 was conducted C-AFM analysis for find the  failure devices. Based on the working principle and power-on  conditions of the C-AFM, under a positive bias, the P/N  junction formed between the source/drain of an NMOS device  and the substrate is in conduction state, so it will be lit. By  contrast, a PMOS device will not be lit. Similarly, under a  negative bias, a PMOS device will be lit while an NMOS  device will not be lit.

These results are shown in Fig. 7 (a) (at bias voltage is +  1V) and Fig. 7 (b) (at bias voltage is -1V). Combined with the  layout information (as shown in Fig. 5 (b)), the NMOS devices  in the red box have leakage current under positive and  negative bias. It indicated that there is an leakage current  between substrate and source/drain. As shown in the white  box in the Fig. 7. (a) and Fig. 7 (b), these normal NMOS  devices is bright in the positive bias and not bright in the  negative bias.

![1_231122_Current_Forward_25  355  Bias@+1v  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/844a6f23-2acb-45fd-8c5f-b1c370af0dcc/844a6f23-2acb-45fd-8c5f-b1c370af0dcc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215837%3B1743219437&q-key-time=1743215837%3B1743219437&q-header-list=host&q-url-param-list=&q-signature=f7db9681346a8282beef23f7b5b4adc952408cd0)
![1_231122_CurrentBackward 25  Bias @-1V  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e391d269-a369-4a34-9a04-4fb99f309787/e391d269-a369-4a34-9a04-4fb99f309787.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215837%3B1743219437&q-key-time=1743215837%3B1743219437&q-header-list=host&q-url-param-list=&q-signature=7a42a7b875a266bd11e8d95bbe6fe64bbd25340c)
Fig. 7.   C-AFM results at bias  $+1\mathrm{V}$   (a) and bias -1V (b) in active area.

In order to further analyze the root cause, we performed a  nanoprobe to test the I-V curve of P/N junction in the  abnormal NMOS device. And comparing with the normal area  NMOS. The test image are shown in Fig. 8 (a). The I-V curve  of abnormal area and normal area are shown in Fig. 8 (b). It is  found that the P/N junction of abnormal area has reverse  abnormal leakage, and the leakage current ratio is two order  larger than the normal area. It’s indicating that the P/N  junction between the substrate and the source/drain is  damaged, which is maybe caused by electrical over stress  (EOS) or electrostatic discharge (ESD).

![（a) （b） Current (A)  I-V curve of p/n junction 1.00E-10 7.50E-11 Leakage 5.00E-11 2.50E-11 Normal 0.00E+00 0.4  0.8  1.6 Voltage (v) Normalarea  Abnormalarea ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ac14e095-8936-4e6e-9c9a-76f21a24bb65/ac14e095-8936-4e6e-9c9a-76f21a24bb65.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215837%3B1743219437&q-key-time=1743215837%3B1743219437&q-header-list=host&q-url-param-list=&q-signature=895fe8461239f0a17409544bc92026e6ccdcce1c)
Fig. 8.   (a) Nanoprobe test image, (b) Nanoprobe test results

## III.    C IRCUIT  A NALYSIS   

As shown in Fig. 9 (a), is a 2-stage LDO structure. The 1 st  stage LDO use booster to generate higher bias voltage, NMOS  source follower LDO can have better Power Supply Rejection   Ratio (PSRR). Rvdd is the LDO on the TX PLL end, which  provides power to the charge pump clock (CHPMPCLK).

Because the FA results indicate that there is an  abnormality in   $1^{\mathrm{st}}$  stage LDO boost circuit. Thus, we  conducted safe operating area (SOA) analysis on this circuit  to confirm whether there is an overvoltage risk in the transistor  of boost circuit. Through simulation analysis, it was found that  when the CHPMPCLK signal flips, there will be an overshoot  problem in pump (PMP) module. Which can cause the four  terminal voltages (Vgb, Vsb, Vdb, Vds  ≤  1.1\* Vdd) of some  devices in PMP module to exceed the design capacity. As  shown in Fig. 9 (b) and TABLE II. , the M1 and M2 devices  of the PMP block had overvoltage risk. The voltage value of  the gate & bulk (Vgb) and source & bulk (Vsb) exceeded the  design capability   $(\leqslant\!1.98\mathrm{V})$  . The design issue of boost circuit  in   $1^{\mathrm{st}}$  stage LDO was be confirmed.

![（a)  1ststageLDO structure TXO 0sub  DataPoir M1/M2Vgb M2Vsb 2.16V M1Vsb 2.16V ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7e906fdc-25a9-422c-a3f8-999c84169c6e/7e906fdc-25a9-422c-a3f8-999c84169c6e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215837%3B1743219437&q-key-time=1743215837%3B1743219437&q-header-list=host&q-url-param-list=&q-signature=abbbe099007c66d85e241866de0ee180eab33778)
Fig. 9.   (a)  2-stage LDO structure. (b) Simulation results of boost circuit

TABLE II.     S IMULATION  R ESULTS OF  B OOST  C IRCUT

|Device|Vgs|Vgb( ≤ 1.98V)|Vsb( ≤ 1.98V)|
|---|---|---|---|
|M1|＜ 1.8V|2.15V(RISK)|2.26V(RISK)|
|M2|≤ 1.8V|2.15V(RISK)|2.16V(RISK)|


As shown in Fig. 10, the location of M1 and M2 device is  same as the abnormal area in C-AFM results. The simulation  results match well with the FA results.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cf7049fe-756a-44f3-8300-798fabf0e4d7/cf7049fe-756a-44f3-8300-798fabf0e4d7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215837%3B1743219437&q-key-time=1743215837%3B1743219437&q-header-list=host&q-url-param-list=&q-signature=05ff924c3b4513b41bab0311f8ab91f873e5ff86)
Fig. 10.   (a) Local circuits of M1 and M2 device, and (b) the location of M1  and M2.

In order to solve this design issue, we have found a  solution by analyzing the two stage LDO circuit structure. We  can restore the function of PLL to normal by bypassing the  $1^{\mathrm{st}}$  stage LDO. As show in Fig. 9 (a), the red line indicates the  voltage states before bypass, and blue line indicates voltage  states after bypass. In before bypass states, the input signal of   $2^{\mathrm{nd}}$    stage LDO is output signal of 1st stage LDO. If the  $1^{\mathrm{st}}$   stage  LDO malfunctions, the function of two stage LDO module  will fail, and ultimately lead to PLL lose lock. After bypass  the  $1^{\mathrm{st}}$   stage LDO, the input signal of  $2^{\mathrm{nd}}$   stage LDO is directly  provided by VAAH. The failure of the  $1^{\mathrm{st}}$   stage LDO will not  affect the functionality of the   $2^{\mathrm{nd}}$   stage LDO. Therefore, the  PLL function can be recovered. Because the chip has been  mass-produced for many years, the failure rate of this problem  is not high. In addition, re-manufacturing costs a lot and takes  a long time, so we select the solution of bypassing the  $1^{\mathrm{st}}$   stage  LDO.

TABLE III.     B YPASS  R ESULTS

|Sample|SerDes PLL lock result|SerDes PLL lock result|SerDes PLL lock result|SerDes PLL lock result|
|---|---|---|---|---|
|Sample|Before bypass|Before bypass|After bypass|After bypass|
|Sample|TXPLL|RXPLL|TXPLL|RXPLL|
|NG1|Lose lock|Lock|Lock|Lock|
|NG2|Lock|Lose lock|Lock|Lock|
|NG3|Lose lock|Lose lock|Lock|Lock|


The operation of bypassing 1st stage LDO is mainly  divided into three categories: bypassing TX’s   $1^{\mathrm{st}}$   stage LDO,  bypassing RX’s  $1^{\mathrm{st}}$   stage LDO, and bypassing   $1^{\mathrm{st}}$   stage LDO  of TX and RX. Three bad units were selected for bypass  testing, and these results are shown in TABLE III. It can be  seen that these PLL function of bad units has been restored to  lock after bypass  $1^{\mathrm{st}}$   stage LDO of TX and RX.

At the same time, we also compared these dynamic EMMI  results of bad unit at before and after bypass states. As shown  in Fig. 11 (a) and (b), the dynamic EMMI result of NG1  indicates that the abnormal emission spot was disappeared  after bypass the TX’s   $1^{\mathrm{st}}$   stage LDO. Fig. 11 (c) and (d) are   indicates that abnormal emission spot of NG2 was  disappeared after bypass the RX’s  $1^{\mathrm{st}}$   stage LDO. And Fig. 11  (e) and (f) are  indicates that abnormal emission spot of NG3  was disappeared after bypass the1 st  stage LDO of TX and RX.  By the way, our solution is to bypass both the   $1^{\mathrm{st}}$   stage LDO  of TX and RX.

![a)  [b） [C】 eLDC eLDC ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/38310f8b-e417-4973-9d97-c2b9ecd9e13d/38310f8b-e417-4973-9d97-c2b9ecd9e13d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215837%3B1743219437&q-key-time=1743215837%3B1743219437&q-header-list=host&q-url-param-list=&q-signature=8238a2ab851321123619941b416b793a860f12a2)
Fig. 11.   Dynamic EMMI result of NG1 both (a) before bypass and (b) after  bypass TX’s   $1^{\mathrm{st}}$   stage LDO, and dynamic EMMI result of NG2 both (c)  before bypass and (d) after bypass RX’s  $1^{\mathrm{st}}$   stage LDO, and dynamic EMMI  result of NG3 both (e) before bypass and (f) after bypass the   $1^{\mathrm{st}}$  stage LDO  of TX and RX.

After bypass 1 st  stage LDO, although the PLL function can  be recovered, but the performance of resisting noise from  external power sources maybe degenerated. Therefore, we  built a test bench to evaluate the impact of PLL performance  after bypassing   $1^{\mathrm{st}}$   stage LDO. As shown in Fig. 12, the PLL  performance after bypass is tested by the test bench. As shown  in Fig. 13, the test results indicate bypassing 1 st  stage LDO not  affects the PLL performance.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/afe025e9-aa8b-42f4-8b79-42e10be7e77c/afe025e9-aa8b-42f4-8b79-42e10be7e77c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215837%3B1743219437&q-key-time=1743215837%3B1743219437&q-header-list=host&q-url-param-list=&q-signature=df42ffe897d8ee8bac37520d31d69d58ad2d6625)
Fig. 12.   Test bench of PLL performance

![bypass_pllpmp=0   bypass_pllpmp=1  TJ=2.67ps;RJ=187fs   Beforebypass   TJ=2.68ps;RJ=188fs   Afterbypass  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/52675a21-4a70-440e-a18c-6f9afb696db0/52675a21-4a70-440e-a18c-6f9afb696db0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215837%3B1743219437&q-key-time=1743215837%3B1743219437&q-header-list=host&q-url-param-list=&q-signature=fb71417c9b306bac3759677082b4263c8c57083d)
Fig. 13.   Test results of PLL performance both (a) before bypass and (b) after  bypass  $1^{\mathrm{st}}$   stage LDO

## IV.   C ONCLUSION 

This paper makes an in-depth analysis of the case of highspeed SerDes PLL lose lock. Through dynamic EMMI, CAFM and Nanoprobe technology to find that the PMP module  of   $1^{\mathrm{st}}$   stage LDO has EOS damage. Further circuit simulation  analysis has found that the circuit structure of   $1^{\mathrm{st}}$   stage LDO

has design defects, and it will make the EOS damage in PMP  module. This problem can be solved by bypassing the   $1^{\mathrm{st}}$   stage  LDO. The effectiveness of this solution has been evaluated by  test bench and confirmed there is no impact on the PLL  performance.

## R EFERENCES   

[1]    S. Sutardja, “The Future of IC Design Innovation,” ISSCC,  SESSION1, PLENARY 1.2, 2015.    [2]    S. Chao, X. Lin, X. Wei, e.t, “Research on the Functional Failure of  Large Scale Chips Caused by Recoverable Latch up,” 2023 IEEE  International Symposium on the Physical and Failure Analysis of  Integrated Circuits (IPFA), Penang, Malaysia, 2023, pp. 1-5.    [3]    C. Chong, W. Cheng Hoe, e.t, “Applications of C-AFM Analysis  Techniques at Advanced IC on ATPG/Scan Failure”, 2011 18th IEEE  International Symposium on the Physical and Failure Analysis of  Integrated Circuits (IPFA), Incheon, Korea, 2011.    [4]    H. Zhang, W. Cheng Hoe, e.t, “Applications of C-AFM analysis  techniques at advanced IC on SRAM soft failure”, 2010 17th IEEE  International Symposium on the Physical and Failure Analysis of  Integrated Circuits (IPFA), Singapore, Singapore, 201

