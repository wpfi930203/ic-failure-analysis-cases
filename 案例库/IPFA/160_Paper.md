---
title: "160_Paper.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_07d1857889dba45f38812e7a4cdb9ba87295230462135641
file_size: 1150627
---

## Reliability Analysis and Comparison on Electromigration of SACQ and SAC305 Solder Balls 

Yang Xuan 1,2 , Yalan Sheng 2 , Niuyi   $\operatorname{Sun}^{2^{*}}$  , Zhuqiu Wang 2 , Dan Yang 2\* , Na Mei 1\* 1 State Key Laboratory of Mobile Network and Mobile Multimedia Technology, Shenzhen, China 2 Department of Reliability Engineering, Sanechips Technology Co., Ltd, Shenzhen, China Phone : (86)15715556881, Email : xuan.yang@sanechips.com.cn

Abstract —In this paper, the electromigration (EM) analysis of Sn-4.0Ag-0.5Cu-3.0Bi-0.05Ni (SACQ) and Sn-3.0Ag-0.5Cu0.05Ni (SAC305) solder balls is investigated. To study the EM reliability performance, multi-level accelerated life tests are designed. A novel temperature calibration method is proposed to characterize the Joule heating effect of solder balls when subjected to high currents. An EM prediction model, based on the modified Black equation, is employed to compare the reliability properties of SACQ and SAC305. As per the results of reliability statistics, the activation energy of SACQ and SAC305 is estimated to be  $\mathbf{0.97\,\pm\,0.2\,\,eV}$   and   $\mathbf{0.78\,\pm\,0.1\,\,eV}$  , respectively, with the current coefficient being   $\mathbf{11.9\:\pm{\:1}}$   for SACQ and   $\mathbf{3.15\:\pm{\:0.6}}$   for SAC305. The failure mechanism is discussed  using  optical  microscope,  scanning  electron microscope, and energy dispersive X-rays. The observed failure results of the SAC-based solder system concur with the Liquid-solid failure mode, as portrayed in the extant literature. Moreover, this work delves into the prevailing polarity effect inherent  in   $\mathbf{Cu}/\mathbf{Sn} $  interconnects  and  the  EM reliability augmentation fostered by Bi-doping.

Keywords—electromigration, SCAQ, SAC305, solder ball, liquid-solid failure mode.

## I.  I NTRODUCTION 

In light of the environmental and health hazards posed by lead   $\mathrm{(Pb)}$  , as well as global Pb-free legislation, the Sn-Ag-Cu (SAC) solder systems have been recommended by JEIDA and NEMI for use in the semiconductor industry due to their superior mechanical properties and thermal fatigue reliability [1]-[4]. Furthermore, with the increasing integration of packaging, the size of interconnecting solder joints in electronic products has significantly decreased, leading to higher current density and a notable temperature rise in the solder joints [5]. This has made electromigration (EM) a significant reliability concern in electronic packaging [6]-[7]. A range of interconnect failures, including intermetallic compound (IMC) formation, hillocks, and cracks, pose a serious threat to the reliability of solder joints [8]-[9].

Based on current research, the addition of specific minor elements has been found to improve mechanical performance. Studies have shown that SAC-based solder joints exhibit increased resistance to creep and thermal fatigue with Bidoping, while IMC growth in Ni-doped SAC solder joints can be suppressed [10]-[11]. As a result, Sn-4.0Ag-0.5Cu3.0Bi-0.05Ni (SACQ) has been developed in recent years [12]-[13].

While there has been extensive research on the EM characteristics of SAC solder balls, there is still a lack of knowledge on the EM reliability of SACQ involving its failure mechanism and the potential impact of alloying element Bi. In this paper, we conduct accelerated life tests

(ALTs) on SACQ and Sn-3.0Ag-0.5Cu-0.05Ni (SAC305) solder balls and propose a new temperature calibration method to predict the actual temperature of the solder balls. We also employ a modified Black equation that takes into account the Joule heating effect of the solder balls to compare the EM properties of SACQ and SAC305. The failure mechanism is investigated using optical microscopy (OM), scanning electron microscopy (SEM), and energy dispersive X-rays (EDX).

## II. E XPERIMENTS 

## A. Experiments Preparation 

To obtain more information and reduce test time, a daisy chain test structure is designed for the experiment. The resistance and temperature of the daisy chain are monitored using the Kelvin method and optical fiber temperature measurement. Fig. 1(a) shows the sketch of the daisy chain test structure, and Fig. 1(b) presents the schematic diagram of the Kelvin method in which  $R_{\mathrm{n}}$   represents the resistance of the solder ball in the daisy chain, while    $R_{\mathrm{a}}$   and    $R_{\mathfrak{b}}$   are the resistances of the sensing wire connected to the ammeter and voltmeter.

![ICSubstrate PCB  ball （DD ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/59a0044c-5bec-4ccf-a218-859dac933b46/59a0044c-5bec-4ccf-a218-859dac933b46.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215863%3B1743219463&q-key-time=1743215863%3B1743219463&q-header-list=host&q-url-param-list=&q-signature=c7be911bb17372e1b23e257b07299bc4b895df28)
Fig. 1. Test structure of daisy chain. (a) Sketch of the daisy chain. (b) Schematic diagram of the Kevin method.

Due to the Joule heating effect caused by the operation of solder balls in a large direct current (DC), it is not feasible to simply substitute the temperature of the solder balls with the ambient temperature [14]. Fig. 2 illustrates the schematic of the optical fiber temperature measurement method used to accurately measure the temperature of the solder balls.

The temperature measurement method is performed with a LUNA OBR4600 backlight reflectometer with a spatial resolution of   $10~\upmu\mathrm{m}$  . The fiber optic thread runs from right to left through each row of the daisy chain. Optical signal changes  are  collected  by  fiber  optic  sensors  during temperature changes, enabling temperature measurement.

1

![TPI  TP   IC Substrate  PCB  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/362de3c2-4082-4585-9e24-7eb756373d0c/362de3c2-4082-4585-9e24-7eb756373d0c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215863%3B1743219463&q-key-time=1743215863%3B1743219463&q-header-list=host&q-url-param-list=&q-signature=52d0bf2795ff9527fe05f2634c16d7259ea36e5e)
Fig. 2. Schematic of the optical fiber temperature measurement.

In this experiment, the printed circuit board (PCB) used is coated with electroless nickel/immersion gold (ENIG), and the IC substrate is coated with IT and standard operation procedure (SOP). The material and size of the SACQ and SAC305 solder balls used are shown in TABLE I. Both types of solder balls have the same ball diameter and pitch value, but the elemental composition is different.

TABLE I.  T HE  M ATERIAL AND  S IZE OF  SACQ  AND  SAC305 S OLDER B ALLS

|Solder Balls|        Elemental                Composition      |        Diameter                wm)      |        Pitch                um)      |
|---|---|---|---|
|Solder Balls|        Elemental                Composition      |        Diameter                wm)      |        Pitch                um)      |
|SACQ|        Sn-4.0Ag-0.5Cu-                3.0Bi-0.05Ni      |S00|1000|
|SACQ|        Sn-3.0Ag-0.5Cu-                0.O5Ni      |S00|1000|
|||||


## B. Temperature calibration method 

In general, the EM characteristic lifetime of metal interconnects can be predicted by the Black equation [15], which is expressed as follows (1):

$$M T T F=A\cdot j^{n}\cdot e x p[\:E a\:/\:k T(j\:,\:T_{0})\:]$$
where MTTF is the mean time to failure,  $A$   is a constant that depends on the material properties,  $j$   is the current density,  n is the current coefficient,  Ea  is the activation energy that reflects the mass transport mechanism and path in EM [16]- [18],  $k$   is the Boltzmann's constant, and    $T$   is the temperature of the solder balls which is dependent on  $j$   and the ambient temperature    $T_{0}$  . Therefore,    $T$   can be modified by (2):

$$T=T_{0}+\Delta T_{j o u l e}$$
The temperature rise denoted as    $\Delta T_{j o u l e}$  , which is caused by the Joule heating effect [19], is measured through the optical fiber array in the solder balls configuration as shown in Fig. 3(a). The peak temperature identified within the interconnected daisy chain of solder balls represents the temperature of interest. To mitigate the impact of random errors, the average of the peak temperatures across each row is calculated and utilized as the representative  $\Delta T_{j o u l e}$   value.

The Joule heating dissipation    $P_{j o u l e}$   [20] can be expressed by (3):

$$P_{j o u l e}=I^{2}R$$
where    $I$   denotes the stress current and    $R$   represents the resistance  of  the  daisy  chain.  An  assumption  of  an approximately linear relationship between    $R$   and    $T$   is also made in this work.  $R$   can be represented as (4):

$$R(T)=a T+b$$
where    $a$   and  $b$   are fitting parameters.

As  demonstrated  by  our  measurements,  the  linear correlation depicted in Fig. 3(b) between    $\Delta T_{j o u l e}$   and    $P_{j o u l e}$   is indeed evident. This relationship can be mathematically expressed as (5):

$$\Delta T_{j o u l e}=c P_{j o u l e}+d$$
where    $c$   and    $d$   are fitting parameters.

![12  PeakTemperature  10   8o  0oo  a  Length(m)  a  80  64  20  10   1S   20   25  Pjoule/w  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1444808f-d427-47a9-b7fb-fccadf1c5d89/1444808f-d427-47a9-b7fb-fccadf1c5d89.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215863%3B1743219463&q-key-time=1743215863%3B1743219463&q-header-list=host&q-url-param-list=&q-signature=6c7ff7a4b45b1780e097c474ea417baf5d6d9e13)
Fig. 3. The measured data of optical fiber. (a) The relationship between  $\Delta T_{j o u l e}$   and optical fiber length. (b) The relationship between  $\Delta T_{j o u l e}$   and  $P_{j o u l e}$  .

From (2) to (5),    $T$   can be derivated as (6):

$$T=\left(T_{0}+b c I^{2}+d\right)/\left(I-a c I^{2}\right)$$
Fig.  4(a)  illustrates  the  calibration  flow  of  the temperature rise in SAC-based solder balls, which can be divided into four distinct stages: (1) Design of Experiment (DOE) for Temperature Measurement, (2) Optical Fiber Measurement, (3) Model Setup, and (4) Model Prediction. Specifically, the DOE for temperature measurement, as depicted in Fig. 4(b), aims to provide measurement points for the subsequent step. In the stage of Model Setup, a simulated annealing (SA) algorithm [21] is chosen to optimize the multi-parameter fitting, as denoted by (6). A shmoo plot of the solder balls temperature predicted by our model under various stress conditions is exhibited in Fig. 4(c), while the maximum error between the measurement and prediction value is less than   $3.7\%$  , as shown in Fig. 4(d).

## C. Experiment Condition 

Multi-level ALTs are designed to investigate the EM failure distribution of SACQ and SAC305 solder balls while the selection of aging conditions and total sample sizes of ALTs are listed in TABLE II. The resistance of the daisy chain is monitored in real time until an open circuit failure occurs.

TABLE II.  T HE  A GING  C ONDITIONS AND  S AMPLE  S IZES

|        Solder                Balls      |        Ambient                Temperature      |        Current                A      |        Sample                size(ea)      |
|---|---|---|---|
|SACQ|100~140|2.3—3|3S|
|SAC305|110~130|2.2—3.3|AN|


![TO/C   VA   Tmes/°CTfit/CError/%  DOE for Temperature   T>I   TA   1.5A   2A   2.5A   2.7A   3   30   0.1   30.0   31.1   3.64  Measurement   30°C   30   36.4   35.9   1.36  30   1.5   43.8   42.4   3.14  50°C   30   S4.2   52.5   3.12  30   2.5   67.6   67.4   0.24  75°C   30   2√   74.8   75.2   0.57  30   89.3   89.5   0.25  100-C   SO   0.1   50.0   S1.1   2.20  OpticalFiber  SO   57.7   56.5   2.02  Measurement   120°C   SO   75.1   75.3   0.26  140-C   SO   2   99.3   101.0   1.67  NS   0.1   75.0   76.1   1.48  1.5   90.6   90.7   0.16  2.5   122.6   123.1   0.38  TOI   1.5   2.2   2.5   27   33   3.5   100   01   100.0   101.1   1.11  ModelSetup   80   87.5   96.1  109.5116.5129.2139.6158.5182.9  203.2   1100   109.3   108.1   1.09  100   133.9   132.3   1.22  90   97.8106.9120.9128.2141.6152.4172.3197.9219.2   100   2.5   155.3   154.0   0.86  100  108.1117.6132.3140.0154.0165.3186.1  212.9235.2   100   184.0   186.1   1.13  110  118.4128.3143.7151.7166.3178.2199.9  227.8251.2   120   0.1   120.0   121.1   0.93  120   1.5   139.5   139.1   0.31  120  128.7  139.1  155.0163.4178.7191.0  213.7  242.8267.1   120   1S5.1   155.0   0.03  130  139.1149.8166.4175.2  191.0203.9227.5257.8283.1   120   214.9   213.7   0.57  ModelPrediction   140   140.0   141.1   0.81  140149.4160.5177.8186.9  203.4216.8241.3272.8299.1  140   149.8   149.4   0.29  150159.7171.3189.2198.6215.8229.6255.1287.8315.1   140   178.5  177.8   0.37  C   Cd  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b3858a8d-751b-476a-a509-b424f46e533a/b3858a8d-751b-476a-a509-b424f46e533a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215863%3B1743219463&q-key-time=1743215863%3B1743219463&q-header-list=host&q-url-param-list=&q-signature=8b6e411f873430c26f6608353a2282bd4fc34382)
Fig. 4. Temperature calibration method. (a) The calibration flow of the temperature rise in SAC-based solder balls. (b) The DOE for temperature measurement. (c) A shmoo plot of the solder balls temperature prediction. (d) The fitting results between the measurement and prediction value.

## III. R ESULTS AND  D ISCUSSION 

## A. EM Reliability Modeling 

Some typical two-stage resistance degradation curves are also observed in SAC-based solder balls, as shown in Fig. 5. Similar to Cu or Al metal lines [22], the resistance of daisy chains under stress at   $2.5~\mathrm{A}/140^{\circ}\mathrm{C}$  initially increases slowly with time and then increases sharply in a very short time, indicating that some open defects may have been generated in the interconnect, leading to sample failure. It should be noted that the resistance may become abnormally small due to the internal melting of Sn, and this anomaly should be eliminated in the analysis.

![100  90  80  28  en   S0  30  20  1O  -10  100   200   300   400   500   600  Time(hr)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9552d514-3cc2-425e-91c7-fbada02e84dc/9552d514-3cc2-425e-91c7-fbada02e84dc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215863%3B1743219463&q-key-time=1743215863%3B1743219463&q-header-list=host&q-url-param-list=&q-signature=f19bb16e22722e564cc0a6cc49886cf41dd718f6)
Fig. 5. The resistance variation of daisy chains under stress at 2.5  $\mathrm{A}/140^{\circ}\mathrm{C}$  .

The time to failure (TTF) of the solder balls in this paper is defined as the time when the resistance of the daisy chain dramatically degrades in the second stage. The MTTF can be obtained from TTF distributions based on different ALTs results. Fig. 6 shows the cumulative failure rate (CFR) with TTF distributions of SAC305 and SACQ solder balls under different aging conditions. The lognormal distribution is the best-fitting distribution.

The current coefficient    $n$   and activation energy  Ea  can be extracted by fitting a modified Black equation using (7):

$$L n(M T T F)=-n L n I+L n A+E a\,/\,k T$$
![0.98  Current/Temp=2.3A/140°℃ 0.95  Current/Temp=2.5A/140°℃ 0.9  Current/Temp=2.7A/120°℃ Current/Temp=2.7A/130°℃ 0.8 Current/Temp=3A/100°℃ 0.3 0.2 0.1 0.05 0.02 200  400500 7001000  2000 TTF(hr) b  8.88  Current/Temp=2.2A/120°℃ Current/Temp=2.5A/125°℃ 0.95 Current/Temp=2.7A/120°℃ 09 Current/Temp=3.3A/110C 08 Current/Temp-3A/110°C Current/Temp=3A/130°C 83 02 01 0.05 8:8元0 20.30  10020040010003000 TTF(hr) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0317ba4b-73ef-4820-80d2-a59ebf02a5c8/0317ba4b-73ef-4820-80d2-a59ebf02a5c8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215863%3B1743219463&q-key-time=1743215863%3B1743219463&q-header-list=host&q-url-param-list=&q-signature=eac385a93420d11f4e0b5d8975ec7e03380af635)
Fig. 6. The CFR with TTF distributions of solder balls under different aging conditions. (a) SACQ. (b) SAC305.

Based on the least squares method [23], the best fittings of the Black equation for SACQ and SAC305 solder balls are demonstrated in Fig. 7(a) and Fig. 7(b). Notably, the experimental points (represented as black spheres) are scattered around the regression surface, indicating a high level of consistency and good fitting. As illustrated in Fig. 7(c) and Fig. 7(d), the fitted curves align with the results presented in Fig. 7(a) and Fig. 7(b), thereby further substantiating the consistency of the findings.

The current coefficient  n  and activation energy  Ea  are extracted based on the optimal fitting results mentioned above and are listed in TABLE III.

TABLE III. THE VALUE OF THE CURRENT COEFFICIENT AND THEACTIVATION ENERGY FOR SOLDER BALLS

|Solder Balls||Ea (eV)|
|---|---|---|
|SAC305|3.15 ± 0.6|0.78 ± 0.1|
|SACQ|11.9±1|0.97 ± 0.2|


3

![s   E6  MTTF(Prediction)   MTTF (Prediction)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5fa43469-bbdc-40a6-a5ff-e4b43ea4bf4e/5fa43469-bbdc-40a6-a5ff-e4b43ea4bf4e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215863%3B1743219463&q-key-time=1743215863%3B1743219463&q-header-list=host&q-url-param-list=&q-signature=c19763752afd99e6b1f8aab467a83d8cadecb0b6)
Fig. 7. The results of parameter fitting of Black equation and goodness of fitting analysis. (a) The fitting diagram of SACQ. (b) The fitting diagram of SAC305. (c) The fitting accuracy of SACQ. (d) The fitting accuracy of SAC305.

The  Ea  of SACQ and SAC305 is similar to the values previously reported for Cu interconnects (0.7-1.0 eV) [22], whereas  n  is greater than that of Cu interconnects. A noteworthy finding is that both  Ea  and  n  of SACQ are greater than those of SAC305, suggesting that SACQ solder joints have a longer lifetime under identical usage conditions, which could be evident in Fig. 8. The possible explanation for the disparity of EM resistance between SACQ and SAC305 will be further expounded upon in the following section.

![Lifetime Comparsion I↓T↓  中SACS0S %L0 Usage conditions ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cad56643-53c4-4785-b3f3-df775d369391/cad56643-53c4-4785-b3f3-df775d369391.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215863%3B1743219463&q-key-time=1743215863%3B1743219463&q-header-list=host&q-url-param-list=&q-signature=31e1607b9604593653d32ba4b3e02b8c6060c6cc)
Fig. 8. The lifetime prediction of SACQ and SAC305 under identical usage conditions.

## B. Failure Analysis 

## 1) Failure Phenomenon . 

The OM images of the failure position at the interface between the SACQ solder balls and the IC substrate in the top view is shown in Fig. 9. Some cracks are clearly visible at the corner of the Sn balls.

![raer  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5d8f7b01-a526-46dd-aacb-fe85c5b294fa/5d8f7b01-a526-46dd-aacb-fe85c5b294fa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215863%3B1743219463&q-key-time=1743215863%3B1743219463&q-header-list=host&q-url-param-list=&q-signature=1b5ebebedcafa5e2be1403c088c40ad6da238b19)
Fig. 9. The OM images of the SACQ failure sample in the top view.

Fig. 10 presents the OM cross-section analysis of SACQ and SAC305. The OM images of SACQ and SAC305 samples, test either with or without stress and current polarity effect, are displayed in Fig. 10(a)-(c) and Fig. 10(d)- (f), respectively. Three remarkable failure patterns could be detected.

![withoutaging  Cd  without aging  ep  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/91f99dd3-bfe4-4528-a89b-15212677d46d/91f99dd3-bfe4-4528-a89b-15212677d46d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215863%3B1743219463&q-key-time=1743215863%3B1743219463&q-header-list=host&q-url-param-list=&q-signature=da36ba874a65a54fdebb68cb0ac4a4c0dba001fe)
Fig. 10. The cross-section analysis of SACQ and SAC305 by OM. (a) SACQ EM failure sample in downstream mode. (b) SACQ sample in upstream mode. (c) SACQ sample without aging stress. (d) SAC305 failure sample in downstream mode. (e) SAC305 sample in upstream mode. (f) SAC305 sample without aging stress.

Firstly, in alignment with the observations of Fig. 9, crack defects can also be detected at the interface between the SAC-based solder balls and Cu trace on the side of the IC substrate as shown in Fig. 10(a) and Fig. 10(d), although almost no cracks or voids are present at the PCB side’s interface regardless of the direction of electron flow.

Secondly, as revealed by the enlarged views of Fig. 10(a) and Fig. 10(d), more fatal voids resulting in an open circuit could be found in the Cu trace adjacent to solder balls. It is evident that part of Cu trace has been substituted by Sn when compared to a fresh sample that has not undergone EM aging as shown in Fig. 10(c) and Fig. 10(f). A typical Snbackfill phenomenon predicated by liquid-solid (L-S) failure mode could also be observed in Cu/SACQ interconnect.

Thirdly, by comparing the SEM images in Fig. 10(a) and Fig. 10(b) or Fig. 10(d) and Fig. 10(e), the difference in EM degradation when the direction of the stress current is opposite can be observed in our studies. The term "upstream mode" refers to the flow of electrons from the PCB to the IC substrate, while "downstream mode" denotes the opposite direction. As thicker IMC layer and more severe crack defects were found at the interface when operating in the downstream mode, it is evident that the solder balls of both SACQ and SAC305 aged in the downstream mode (as shown in Fig. 10(a) and Fig. 10(d)) degrade faster compared

to those aged in the upstream mode (as shown in Fig. 10(b) and Fig. 10(e)).

Fig. 11(a) and Fig. 11(b) provide enlarged SEM results of both SACQ and SAC305 failure samples aged in the

downstream mode. Observable color variations near the EMinduced crack suggest the presence of multiple phases at the cathode interface.

![①②③④5 SACQ-5 Elen Kent Atom(%) sn  55.13 Dcu  21.75 ②CusSn  14.25 8.53 ③ CusSns  0.23 ④C/O 5Sn/Bi ?Sn/Cu/Bi SACQ   Sn/Cu SACQ-6  m（%） C  CusSn  CusSns  Crack  Sn/Cu/Bi  56.45 21.11 13.52 207 6.55 23④556  D.29 Dcu ②CuSn  Cd ③ CueSns ④C/O  SACQ-④  0（%6） 5Sn  55.90 ?CuSn  21.96 14.32 2.31 SAC305 CusSn  CueSns  Crack  SnCu Ce ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fc9aa5b9-8da2-4ae9-ae07-ec52d6456092/fc9aa5b9-8da2-4ae9-ae07-ec52d6456092.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215863%3B1743219463&q-key-time=1743215863%3B1743219463&q-header-list=host&q-url-param-list=&q-signature=8de217500f86bc65eab478b7e0f6dd7a00ffe6fe)
Fig. 11. The SEM results of SACQ and SAC305 failure samples. (a) SACQ. (b) SAC305.EDX energy spectrum of (c) SACQ-  $\mathcal{\left(5\right)}$  , (d) SACQ-  $\textcircled{6}$  , and (e) SACQ-  $\boldsymbol{\mathcal{Q}}$  .

EDX  analysis  conducted  of  SACQ  and  SAC305 indicates that  $\mathrm{Cu}_{3}\mathrm{Sn}$   (landmark 2 in Fig. 11(a) and Fig. 11(b)) and   $\mathrm{Cu}_{6}\mathrm{Sn}_{5}$   (landmark 3 in Fig. 11(a) and Fig. 11(b)) are formed in the regions between the Sn-rich and Cu-rich areas, whereas the crack (landmark 4 in Fig. 11(a) and Fig. 11(b)) adjacent to Cu-Sn IMCs is observed to have occurred within the Sn-rich region. Due to Cu diffusion toward the Sn ball, there are some Cu atoms (landmark 7 in Fig. 11(a)) even CuSn IMC (landmark 6 in Fig. 11(b)) could be found in the bulk of SAC-based solder balls. However, there are hardly any Cu atoms on the side of the crack close to the solder ball (landmark 5 in Fig. 11(a) and Fig. 11(b)), implying that almost all copper atoms are replaced by Sn atoms. The concentration of Bi atoms has been observed near the identified crack, as denoted by landmark 5 in Fig. 11(a). The elemental abundance of Bi in the vicinity of the crack (landmark 5 or 6 in Fig. 11(a)) is greater than the concentration of Bi found in the bulk (landmark 7 in Fig. 11(a)) which can not be detected by EDX. The detection of Ni in SACQ and SACQ305 solder balls might be impeded by its potentially low elemental concentration, making it difficult to assess the impact of Ni on the EM reliability of SAC-based solder joints. By contrast, the enhancement effect of Bi atom on the EM reliability of SACQ solder can be proved by the component comparison in Fig. 11 as well as the lifetime prediction as compared to SAC305 in Fig. 8.

The spatial distribution of each element in the SACQ ball interconnection structure is further understood using

EDX mapping, and the distribution of related elements (distinguished by different colors) is shown in Fig. 12.

![AI  Ag  Esn  Cusioc  C   SE  CC   25un  B1  en  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3647a025-ba62-4bfc-aefe-445a9d0c21e9/3647a025-ba62-4bfc-aefe-445a9d0c21e9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215863%3B1743219463&q-key-time=1743215863%3B1743219463&q-header-list=host&q-url-param-list=&q-signature=37413133f64d3f69af66de69648865b941ca0585)
Fig. 12. The element mapping of Fig. 11 (a). (a) The SEM result. (b) The element mapping result. (c) Cu. (d) Sn. (e) Bi. (f) Ag.

Obviously, Cu atoms are almost completely exhausted and replaced by Sn atoms on the right side of the crack, but the Cu content on the right side of the crack is hardly detected as shown in Fig. 12(c). A high concentration gradient of Sn atoms exists near the crack as shown in Fig. 12(d), resulting in the absence of Sn atoms at the far end of Cu Trace. Although the Bi atoms content is much lower than that of Sn atoms in the SACQ solder ball, a considerable amount of Bi could still be observed on the left side of the crack as shown in Fig. 12(e). It is interesting that the aggregation effect of Ag atoms is also observed in the bulk of SACQ solder balls and is hard to form IMCs with Sn or Bi atoms as shown in Fig. 12(f), indicating that Ag atoms might have no impact on SACQ EM.

## 2) The failure mechanism. 

As stated in our previous work [7] and other publications [24]-[25], the degradation process of L-S mode can be represented in Fig. 13. L-S mode is demonstrated as the dominating failure mechanism of Ni-doped SAC solder which could  also be used to  explain similar  failure phenomena observed in SACQ solder joints.

![Cutrace   Cu/sn  CU  interface  SE   IMC   Sn-rich   ouaSn   Cu-rich  CusSns  Cutrace  INC   Cu/sn   C   EIMC.   Cu/sn  interface   interface  sn   CurrentCrowding   sn  (hotspot)  IMC  C   C  Cu/sn   Cu/sn  interface   interface  sn   sn  Crack  IMC   C   IMC   C  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/85c41fce-fb22-4b17-877e-92d4a188bb28/85c41fce-fb22-4b17-877e-92d4a188bb28.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215863%3B1743219463&q-key-time=1743215863%3B1743219463&q-header-list=host&q-url-param-list=&q-signature=e10b38f34a54105c78e3d5f2fbf57601726b7451)
Fig. 13. The degradation process of L-S mode. (a) As reflowed. (b) Current crowding effect. (c) IMC growth. (d) IMC mixture and Sn backfill. (e) Crack occurrence in Sn-backfilled trace.

To gain a profound insight into the current density and temperature distribution within the solder ball, an electricthermal coupling simulation as shown in Fig. 14 is conducted using Abaqus.

The simulation results for cloud maps current density and temperature are presented in Fig. 14(a) and Fig. 14(b), demonstrating  that  the  current  crowding  effect  and temperature clustering occur at the cathode/anode interfaces that also correspond to the position of EM-induced cracks observed in the results of OM and SEM. The maximum current density and local temperature at the IC substrate side are higher than those at the PCB side due to the asymmetric  $\mathrm{Cu/SAC}$   interconnect structure, which is evident to explain why there are almost no cracks or voids present at the PCB side’s interface as mentioned earlier. In the context of the finite element method, it is observed that there isn't a distinct variation in temperature and current density distribution when the direction of the current is altered.

The  influence  of  solder  joint  geometry,  which encompasses the height, diameter, and volume of the solder ball, on current density and temperature has been examined through Abaqus simulation. The maximum recorded values

of current density and temperature are presented in TABLE IV. It is noted that ball diameter is the main factor impacting the maximum value of current density and temperature in the solder ball compared to ball height.

![ECDHER   al current per unit area  1.324E+02  1.180E+02  1.036E+02  8.928E+01  7491E+01   ax.Value=.132.4  L054E+D1  4.617E+01  3.180E+01  1.743E+01  3064E+D0  Max-1.324E+02  Min-3.054E+00  NT11-Nod   e(Scalarvalue)  1.455E+02  1.454E+02  1.453E+02  1.452E+02   micMax.Value  1.451E+02  1.450E+02  1448E+02  1.447E+02  1.446E+02  1.445E+02  Max=1.455E+02  Min = 1.445E+02  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2350d1be-6faf-43a7-b68e-6b87471ab92d/2350d1be-6faf-43a7-b68e-6b87471ab92d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215863%3B1743219463&q-key-time=1743215863%3B1743219463&q-header-list=host&q-url-param-list=&q-signature=d044fcc3b933ab34633fb1bed9fcb8319c2bde0d)
Fig. 14. The electric-thermal coupling simulation of SAC-based solder ball working  in  the  condition  of   $2\mathrm{A}/120^{\circ}\mathrm{C}$  .  (a)  Current  density.  (b) Temperature.

TABLE IV.

T HE  I NFLUENCE OF  S OLDER  J OINT  G EOMETRY

|        Height                (mm)      |        Diameter                (mm)      |        Maximum                current density                (A/mm²)      |        Maximum                temperature                C）      |
|---|---|---|---|
|0-4|0.72|132.4|145.5|
|0.35|0.72|133.0|145.4|
|0-4|0.66|129.2|145.7|


To understand the current polarity effect found in OM observations, it is necessary to consider the mass transport of Cu and Sn atoms in different current modes and its impact on IMC growth. The atomic diffusion flux [26] undergoing EM is applied to quantitatively represent mass transport as above and expressed by (8):

$$J\!=\!J_{d r i f t}+J_{d i f f}\!=(C D/k T)\rho j Z^{*}e\cdot D(\partial C/\partial x)$$
where    $J_{d r i f t}$   is the flux caused by the electron wind force,  J diff is the flux caused by the chemical potential gradient,    $C$   is the atomic density,    $D$   is the diffusivity,    $k$   is Boltzmann constant,    $T$   is temperature,  $\rho$   is the resistivity of liquid Sn,  j is the current density,  $Z^{*}$    is the effective charge number, and  $e$   is the electron charge.

The effect of electrons' current polarity on atomic diffusion rate is shown in Fig. 15. In the downstream mode, the drift and diffusion motion of Cu atoms near the cathode interface superimpose in the same direction, so Cu atomic flux    $J_{C u}$   could be written as  $J_{C u}=J_{C u\_d i f f}+J_{C u\_d r i f t}$  . However, in the upstream mode, the drift and diffusion motion of Cu atoms are opposite and offset each other, resulting in a smaller Cu atomic flux    $J_{C u}$   that could be expressed as    ${{J}_{C u}}=$   $J_{C u\_d i f\_d i f\_d i f t}~.~J_{C u\_d r i f t}$  . Since liquid Sn has a larger diffusion coefficient, resulting in    $J_{S n\_d i f\!f}>>J_{S n\_d r i f\!t}$  , Sn atomic flux    $J_{S n}$

could be described by  $J_{S n}=J_{S n\_d i f f}\pm J_{S n\_d r i f t}\approx J_{S n\_d i f f}$   whether in downstream or upstream mode. It can be seen that a larger flow of Cu atomic flux might accelerate the consumption of Cu elements on the IC substrate side and promote the growth of IMC as well as Sn-backfill, leading to earlier failure in the downstream mode.

![Cu(Sub)  Cu(Sub) sn  sn Cu(PCB)  Cu(PCB) dr C sn  sn (a)a  (b)](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/aae245a8-31fe-4133-ac8d-af0ed7685798/aae245a8-31fe-4133-ac8d-af0ed7685798.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215863%3B1743219463&q-key-time=1743215863%3B1743219463&q-header-list=host&q-url-param-list=&q-signature=0e55e13acce4a7347b766da2a0e58559686888f0)
Fig. 15. The effect of electrons' current polarity on atomic diffusion rate. (a) Downstream mode. (b) Upstream mode.

## 3) The influence of Bi. 

The previous section has revealed the enhancing effect of Bi element on the EM lifetime of SAC-based solder joints, and  a  qualitative  explanation  of  the  mechanism  for strengthening the EM properties by Bi doping has been proposed.

![76  Trace  iSn/Bis  cusn  Cu/Bi   Crack  IMC  SACQBall  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/11d513fa-7700-4d74-a975-a7f1c629940f/11d513fa-7700-4d74-a975-a7f1c629940f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215863%3B1743219463&q-key-time=1743215863%3B1743219463&q-header-list=host&q-url-param-list=&q-signature=9a3d8b3b9a4bb1f98c211504b9907101905ffbc2)
Fig. 16. The elements variation of SACQ EM failure sample. (a) The element abundance with distance. (b) The diffusion coefficient of Sn atoms in Bi. (c) The diffusion coefficient of Sn atoms in Cu.

Based on the results of EDX line scan of Cu Trace adjoined to SACQ solder ball, the normalized elemental distributions of Cu, Sn and Bi at the interface are presented in Fig. 16(a). A relatively small variation of Bi content is found in the whole Cu trace, and the diffusion distance of Sn is much shorter than that of Bi, indicating that Bi atoms in Cu grain have faster diffusion velocity with agreement to previous research [27]-[28] due to Bi diffusion through grain boundaries of   $\mathrm{Cu}/\mathrm{Sn}$   phase. As reported in [29]-[30], Bi atoms generally adhere to the surface of Cu-Sn or Ag-Sn IMCs, which could block the mass transport of Sn, Cu, and Ag, thereby suppressing the growth of IMCs. In this case, Bi atoms act as a "barrier layer", hindering the diffusion of Sn atoms from the Sn ball to the Cu trace. Specifically, the diffusion coefficient of Sn atoms in Bi is smaller because in Bi matrix, Sn atoms exist in the form of interstitial atoms as described in Fig. 16(b), and the diffusion coefficient of interstitial diffusion is generally smaller. In contrast, the diffusion coefficient of Sn atoms in Cu matrix is larger because in Cu matrix, Sn atoms exist in the form of substitutional atoms as described in Fig. 16(c). Finally, the suppression of IMC growth at the Cu/SACQ interface due

to the blocking effect of Bi atoms leads to more reliable EM performance.

## IV. C ONCLUSION 

In this study, a series of ALTs are applied to evaluate the EM reliability performance of SACQ and SAC305 solder balls. A novel temperature calibration method is proposed to accurately assess the temperature of the solder balls, including temperature rise due to Joule heating under different  ambient  temperatures and  current  conditions. Through statistical analysis of ALTs data, both  n  and  Ea  of SACQ  and  SAC305  solder  joints  are  extracted  and compared. The SACQ solder balls exhibit better EM performance due to their longer expected lifetime with a constant cumulative failure rate of   $0.1\%$  .

EM-induced failures in the daisy chain test structure are observed to initially occur at the interface between the SACbased solder joints and the Cu trace. This can be attributed to the combination of the current crowding effect and the L-S failure mechanism. The polarity effect of EM in SAC-based solder systems may be due to two competing mechanisms existing in the  $\mathrm{Cu}/\mathrm{Sn}$   inter-diffusion process.

Furthermore, our experiments suggest that the presence of Bi atoms act like a diffusion-blocking layer, suppressing the growth of IMC, leading to an enhancement in the lifetime of the SACQ solder joints.

## R EFERENCES 

[1]  X. P. Zhang, L. M. Yin and C. B. Yu, “Advances in research and application  of  lead-free  solders  for  electronsic  and  photonic packaging,” Journal of Materials Research, vol. 22, no. 1, pp. 1-9, February 2008.   [2]  S. Cheng, C. M. Huang and M. Pecht, “A review of lead-free solders for electronsics applications,” Microelectronsics Reliability, vol. 75, no. 8, pp. 77-95, August 2017.   [3]  L. Chu, J. Shi and R. Braun, “The impacts of material uncertainty in electro-migration of SAC solder electronsic packaging by monte carlo-based stochastic finite-element model,” IEEE Transactions on Components, Packaging and Manufacturing Technology, vol. 11, no. 11, pp. 1864-1876, November 2021.   [4]  H. Ma and T. K. Lee, “Effects of board design variations on the reliability  of  lead-free  solder  joints,”  IEEE  Transactions  on Components, Packaging and Manufacturing Technology, vol. 3, no. 1, pp. 71-78, January 2013.   [5]  S. Q. Gu, “Material innovation opportunities for 3D integrated circuits from a wireless application point of view,” MRS Bulletin, vol. 40, pp. 233-241, September 2015.   [6]  J. F. Xu, C. Y. Cai, V. Pham, K. Pan, H. Y. Wang and S. Park, “A comprehensive study of electromigration in lead-free solder joint,” 2020 IEEE 70th electronsic Components and Technology Conference (ECTC), Orlando, FL, USA, 2020, pp. 284-289.   [7]  X. P. Wu, N. Y. Sun, D. Yang, N. Mei and T. B. Sun, “Identification of  electromigration  failure  mechanism  dominated  in  FCBGA applications,” 2022 23rd International Conference on electronsic Packaging Technology (ICEPT), Dalian, China, 2022, pp. 1-5.   [8]  H. R. Christine and Y. W. Yau, “Electromigration reliability of solder balls,” 2018 IEEE International Symposium on the Physical and Failure Analysis of Integrated Circuits (IPFA), Singapore, 2018, pp. 1-5.   [9]  T. Y. T. Lee, T. Y. Lee and K. N. Tu, “A study of electromigration in 3-D flip chip solder joint using numerical simulation of heat flux and current density,” IEEE Transactions on Components and Packaging Technologies, vol. 27, no. 3, pp. 472-479, September 2004.   [10] A. A. El-Daly, A. M. El-Taher and T. R. Dalloul, “Improved creep resistance and thermal behavior of Ni-doped Sn-3.0Ag-0.5Cu leadfree solder,” Journal of Alloys & Compounds An Interdisciplinary Journal of Materials Science & Solid State Chemistry & Physics, vol. 587, pp. 32-39, February 2014.   [11] M. Y. Tsai, Y. S. Lin, C . L. Kao, S. B. Wang, T. C. Lin and Y. C. Hung, “Effect of novel SAC-Bi solder joints on electromigration reliability for  wafer level chip scale  packages,” International Symposium on Microelectronsics (ISM), Naples, Italy, 2021, pp. 136 – 141.   [12] P. Lall, V. Yadav, J. Suhling and D. Locker, “High strain rate mechanical behavior of SAC-Q solder,” 2017 16th IEEE Intersociety Conference on Thermal and Thermomechanical Phenomena in electronsic Systems (ITherm), Orlando, FL, USA, 2017, pp. 1447- 1455.   [13] T. S. Yeung, H. Sze, K. Tan, J. Sandhu, C. W. Neo and E. Law, “Material characterization of a novel lead-free solder material  — SACQ,” 2014 IEEE 64th electronsic Components and Technology Conference (ECTC), Orlando, FL, USA, 2014, pp. 518-522.   [14] R. Verma, S. Bhattacharya and S. Mahapatra, “Theoretical estimation of electromigration in metallic carbon nanotubes considering joule heating effect,” IEEE Transactions on electrons Devices, vol. 59, no. 9, pp. 2476-2482, September 2012.   [15] J. R. Black, “Electromigration  —  A brief survey and somerecent results,” IEEE Transactions on electronsDevices, vol. 16, no. 4, pp. 338-347, April 1969.   [16] X. Zeng, Z. H. Huang, S. J. Wang, M. Xiao, Y. Z Meng and Y. Liu, “Simulation on interplay between morphological evolution and defect in polycrystalline TSV During EM”, IEEE Transactions on electrons Devices, vol. 71, no. 1, pp. 322-330, January 2024.   [17] S. P. Prasad, Y. Singh, P. K. Vaitheeswaran and G. Subbarayan, “The connection  between  electromigration  resistance  and  thin-film adhesion and their degradation with temperature”, IEEE Transactions on Components, Packaging and Manufacturing Technology, vol.13, no.3, pp. 426-443, March 2023.   [18] B. Xu, R. Chen, J. Zhou and J. Liang, “A modeling study on electrical and thermal behavior of CNT TSV for multilayer structure”, IEEE Transactions on electrons Devices, vol. 70, no. 9, pp. 4779- 4785, September 2023.   [19] Y. J. Hou and C. M. Tan, “Requirement for accurate interconnect temperature measurement for electromigration test,” Proceedings of the 2009 12th International Symposium on Integrated Circuits, Singapore, 2009, pp. 522-525.   [20] C. Chen, H. M. Tong and K. N. Tu, “Electromigration and thermomigration in Pb-Free flip-chip solder joints,” Annual Review of Materials Research, vol. 40, no. 1, pp. 531-555, April 2010.   [21] S. Bandyopadhyay, S. Saha, U. Maulik and K. Deb, “A simulated annealing-based multiobjective optimization algorithm: AMOSA,” lIEEE Transactions on Evolutionary Computation, vol. 12, no. 3, pp. 269-283, June 2008.   [22] W. K. Chien, A. Zhao and V. Chang, “Parameter and trend analysis on electromigration acceleration model,” Semiconductor Technology, vol. 34, no. 11, pp. 1110-1113, November 2009.   [23] A. Fitzgibbon, M. Pilu and R. B. Fisher, “Direct least square fitting of ellipses,” IEEE Transactions on Pattern Analysis and Machine Intelligence, vol. 21, no. 5, pp. 476-480, May 1999.   [24] Z. J. Zhang and M. L. Huang, “In situ study on liquid-solid electromigration behavior in   $\mathrm{Cu/Sin-}37\mathrm{Pb/Cu}$   micro-interconnect”, Acta Metallurgica Sinica, vol. 56, no. 10, pp. 1386-1392, January 2020.   [25] C. K. Lin, Y. W Chang and C. Chen, “Experimental and simulation analysis of concave-down resistance curve during electromigration in solder joints,” Journal of Applied Physics, vol. 115, no. 08, pp. 5451- 5457, February 2014.   [26] H. Gan and K. N. Tu. “Polarity effect of electromigration on kinetics of intermetallic compound formation in Pb-free solder V-groove samples”, Journal of Applied Physics, vol. 97, no. 06, pp. 1-10, 2005.   [27] L. Sun, J. S. Yan, L. M. Wang, and W. Xiao. “Effects of alloying elements on the dissolution and diffusion of Bi in Sn: A firstprinciples  study,”  2021  IOP  Conference  Series:  Earth  and Environmental Science, Shenzhen, China, 2021, pp.12-18.   [28] L. T. Chen and C. M. Chen, “Electromigration study in the eutectic SnBi solder joint on the Ni/Au metallization,” Journal of Materials Research, vol. 21, no. 4, pp. 962-969, December 2006.   [29] Y. Chen, C. Wang and Z. Q. Liu, “Fracture characteristic and microstructure evolution of new Sn-Bi-Ag(Cu) solder joints,” 2020 21st International Conference on electronsic Packaging Technology (ICEPT), Guangzhou, China, 2020, pp. 1-4.   [30] G. Ju, W. Bi, F. Lin, Y. Han and X. Wei, “The comparative study on interfacial IMCs growth of three Cu/SnAgCu/Cu solder joints with Bi and Cr additions during thermal aging,” 2012 13th International Conference on electronsic Packaging Technology & High Density Packaging, Guilin, China, 2012, pp. 194-199.

