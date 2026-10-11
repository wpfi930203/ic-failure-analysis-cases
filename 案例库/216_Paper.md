---
title: "216_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_b2969cacfc14156f58c3d94a0f898e377295230462135641
file_size: 665988
---

## Calculating Activation Energy (Ea) of SRAM Product  Using The Vmin Variation Method  

Tseng Wu Han and Kuo Shuen Chao and Huang Kuan Chieh  Reliability Engineering Department, Powerchip Semiconductor Manufacturing Corp.  No. 18 Li-Hsin Rd. 1, Hsin Chu Science Park, Hsin Chu, Taiwan, R.O.C.     \*   Phone: 886-3-5795000 EXT 4977  Fax: 886-3-5792142  Email: whtseng@powerchip.com

Abstract-   TAF is a necessary value for calculating the operation  Lifetime of IC product. The activation energy (Ea) is the  parameter value required to calculate the TAF. Each company  has different ways of obtaining activation energy (Ea). Some used  function test pass/fail and also current change. Our method is  based on the characteristics of SRAM products and the memory  unit data storage capacity was used. The activation energy (Ea)  value was calculated by analyzing the decay of the lowest  operating voltage of the data after two kinds of accelerations at  high temperature and high bias. After the experiment, we  obtained the activation energy (Ea) value of 0.81eV. The relevant  research are all in this paper.

## I. I NTRODUCTION 

Fig.1 is a 6T SRAM cell architecture.[1] The 6T SRAM cell  is composed of 6 transistors. Both transistors M5 and M6 are  used as switches. One inverter is composed of M1 and M2  transistors, the other inverter is composed of M3 and M4. The  output terminals of the two inverters are connected respectively  to the input terminals of the other inverters forming a latch  circuit which can latch the storage data. Thus, it forms a  bis-table circuit which can be used for storing 0 and 1

![wdd  3  EB   EL  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/97ce73a6-92e8-4571-8b83-cc7e2f5addfc/97ce73a6-92e8-4571-8b83-cc7e2f5addfc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215659%3B1743219259&q-key-time=1743215659%3B1743219259&q-header-list=host&q-url-param-list=&q-signature=13d1bd2a0940f4cc62fe6d45d7bcc56afe1f63d2)
Fig. 1 6T SRAM Cell Architecture

Operation life time is a very important item in reliability  qualification. To calculate operation life time, we first needed  to calculate the temperature acceleration factor (TAF). To find  the TAF, it is necessary to obtain the activation energy (Ea)  first.[2]

The mathematical relationship between reaction rate and  temperature is described by the Arrhenius equation (Formula 1)

Arrhenius equation is as follows

$$T_{A F}={\frac{L_{n}}{L_{s}}}=\exp\biggl[{\frac{E_{a}}{k}}\left({\frac{1}{T_{n}}}-{\frac{1}{T_{s}}}\right)\biggr]\;\;{\mathrm{(~Equation~1~)}}$$
TAF is the temperature acceleration factor and Ea represents  the activation energy, k represents the Boltzmann constant and  Tn and Ts represent the absolute temperature under normal  conditions and the absolute temperature under accelerated test,  respectively. From the equation, it is obvious that the activation  energy (Ea) is the necessary for calculating TAF. At present,  various semiconductor factories use different methods to derive  the activation energy (Ea) of SRAM products. As Table.1  indicates company A used the product to perform accelerated  tests at different ambient temperatures. As the acceleration time  increased, the standby current variation of SRAM product had  an activation energy (Ea) of 1.21 eV.

Table 1 Activation energy (Ea) Calculation for Company A

|LOf| Tempeiature|Back(his)|Back(his)|Back(his)|Back(his)|Back(his)|Ref.I(uA)|Life time(hrs)|
|---|---|---|---|---|---|---|---|---|
|LOf| Tempeiature||24|168|500|1000|Ref.I(uA)|Life time(hrs)|
|Lot-A|225'C|26.32uA25.95uA2|26.32uA25.95uA2|26.05uA|25.69uA|25.23uA|19|7969.0|
|Lot-B|250'C|27.39uA26.20uA|27.39uA26.20uA|26.06uA|25.34uA|24.12uA|19|1731.2|
|Lot-C|275'C||||||19|467.6|


Table.2 indicates company B calculated the activation energy  (Ea) of   $1.28\mathrm{eV}$   using the pass/fail judgment of the product  components.

|LotNo|Temp|||||||||||||
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|LOt-A|300′C|Initial|24hrs|72hrs|168hrs|||||||||
|LOt-A|300′C|05|0M5|045|45/45|||||||||
|Lot-B|250C|Initial|168hrs|504hrs|1008hrs|||||||||
|Lot-B|250C|05|05|045|045|0/45|15/45|||||||
|Lot-C|200′C|Initial.|168h1s|504hrs|1008hrs|1512hrs|2016hrs3|||||||
|Lot-C|200′C|05|05|045|045|0745|0v4.5|045|0V45|0VM5|0M5|0M45|045|


Table 2 Activation energy (Ea) Calculation for Company B

Some companies did not calculate the actual activation energy  (Ea) value, they used the empirical value   $0.7\mathrm{eV}$   for the Ea to  calculate the operation life time.

## II.   EXPERIMENTS  

Our concept was to use the device characteristics of SRAM  and the data storage capability in the memory cell, both were  then stressed under both high temperature and high bias voltage  accelerations experiment. Analysis of the data retention with  degradation amount of the lowest working voltage gave us the  temperature acceleration parameter (Ea). Our experimental  procedures were as follows: (a) used three groups of samples,  and each group must have sufficient samples to make a  lognormal distribution. (b) Write the data under normal  operating voltage. (c) The groups are accelerated with three  different ambient temperatures (  $120\,^{\circ}\mathrm{C},$  ,   $135\mathrm{~}^{\circ}\mathrm{~C~}$   and   $150\,^{\circ}\,\mathrm{C})$  ),  respectively. (d) Perform electrical performance test at   $85\mathrm{~}^{\circ}\mathrm{~C~}$    after reducing the cell operating voltage (Vcc) to ensure the  minimum operating voltage of the cell Vmin state.

As the accelerated stress time increases, we found that the  minimum operating voltage of the cell (Vccmin) exhibited a  gradual increase, signifying the gradual degradation  phenomenon of the cell. We recorded the relationship between  the shift value of Vccmin (increasing 0.04V) and the stress time.  Fig.2 is the trend plot of Vccmin with stress time at the three  temperatures of   $120\,^{\circ}\mathrm{C}\;/\;135\,^{\circ}\mathrm{C}\;/\;150\,^{\circ}\mathrm{C}.$  . At   $150^{\circ}\mathrm{C}$  ,   $135^{\circ}\mathrm{C}$   and   $120^{\circ}\mathrm{C}$   temperature accelerations, it can be found that the   $150^{\circ}\mathrm{C}$  temperature acceleration led to sample degradation faster in the  minimum operating voltage of the cell (Vccmin). Failure  criteria judgment was  $20\%$   Vccmin shift level, this depends on  the product characteristics. All samples have reached   $20\%$    Vccmin shift level at around 96hrs. As for two groups of  samples, then reached  $20\%$   Vccmin shift level with a stable  state at around both 1116hrs at   $135\,^{\circ}\mathrm{C}$   and 1128hrs at   $120\,^{\circ}\mathrm{C}$   of  accelerations stress.

![  309XG     120C  150'C  —135'C  150°C  269%6     120°C  209XG     135°℃  169X6     1-09X6       696  0re6        Stress Time (Hrs)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/256de20a-93f7-4add-a656-19c9e914146b/256de20a-93f7-4add-a656-19c9e914146b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215659%3B1743219259&q-key-time=1743215659%3B1743219259&q-header-list=host&q-url-param-list=&q-signature=db10186e6c8cc824ae0bdab3b06b52284ac1c1f2)
Fig 2 Trend Plot of Vmin with Stress Time

Next, we performed activation energy (Ea) calculations by  combining the individual Vmin variation with the stress time  under temperatures of   $120~^{\circ}\mathrm{C}$  ,  $135\,^{\circ}\mathrm{C}$   and   $150~^{\circ}\mathrm{C}$  , respectively.  Table 3 is the variation of Vmin from each sample with  increasing stress time at   $120\,^{\circ}\mathrm{~C~}$  ,   $135\mathrm{~}^{\circ}\mathrm{~C~}$   and   $150\,^{\circ}\mathrm{~C~}$  .

## III. R ESULTS AND DISCUSSION 

Because we obtained three groups of Vccmin degradation  values with accelerated stress at three temperatures, we used the  lognormal distribution with the most approximate method  (MLE) to obtain the TTF probability plot and then calculated an  Ea of 0.81eV. Because the lognormal distribution is also  applicable to IC samples with temperature accelerated lifetime  distribution , we can also obtain the minimum operating voltage  of the cell (Vccmin) with fast degradation state ； a bi-model type  distribution at   $150\mathrm{^\circC}$  stress is shown in Fig.3 However, we need  to further explore the degradation behaviors and mechanisms of  the minimum operating voltage of the cell (Vccmin).

![ProbabilityPlot(FittedArrhenius)forTTF  Lognoamal  CcnsoringColumninccnsor-ML Eshimatts  SSS  SS  2B3S0   200  0   Ea=0.81eV  10   100   1000  TTE  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d0982324-e429-4dc6-b11a-b8dc9fbbbb78/d0982324-e429-4dc6-b11a-b8dc9fbbbb78.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215659%3B1743219259&q-key-time=1743215659%3B1743219259&q-header-list=host&q-url-param-list=&q-signature=4b050da96ac332ad9f968fad3aecb0c9159b95dd)
Fig.3 Probability Plot of TTF

Probability plot exhibited bi-model type distribution at   $150\mathrm{^\circC}$  acceleration stress, we further performed electrical  characteristic analysis for Vccmin degradation exploration by  nano-probe detection. Fig.4 revealed both PGR and PDL  devices of the abnormal cell had a weaker threshold voltage  than that of other normal cells.

![FailBit  DDC  VDDC  POR  ss  PO_VgHdcurve  PG_Vg-idcurve  POLVEh  PGVh  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c658f89c-d65f-4e16-82f2-94664230b4e9/c658f89c-d65f-4e16-82f2-94664230b4e9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215659%3B1743219259&q-key-time=1743215659%3B1743219259&q-header-list=host&q-url-param-list=&q-signature=dcf2c40449ed093b89843565181b8f17e8160145)
Fig.4 Id-Vg Curves of PGR and PDL Devices

The main reasons for PGR and PDL devices to exhibit  abnormal electrical characteristics ： (a) The PGR device of  abnormal cell had a weaker channel length than that of other  cell. Thus, it created a larger driving current when the device  was operating. The exploration of mechanisms were done at a  read data   $"0"$   state, BLB/BL performed a pre-charge to a high  voltage level, and the PGR and PGL devices turned on.  Meanwhile, the driving current of PGR device was higher due  to the channel length of the device being weaker.

This phenomenon means that the PGR device induced the  voltage level of storage node B to rise, Fig.5

![Stronger  IPG  PXR   IPD  PGE   Weaker  SGL   0V+c  PXR  BLB   BL  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0bd29b32-4625-42f5-b267-e2a2c01c14ab/0bd29b32-4625-42f5-b267-e2a2c01c14ab.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215659%3B1743219259&q-key-time=1743215659%3B1743219259&q-header-list=host&q-url-param-list=&q-signature=07dc707ac162fc56494ef9d8d2ec567e55a51cd2)
Figure 5 Strengthen PGR Device Current

(b) The PDL device itself had a weaker threshold voltage  causing the device to turn on early, resulting in storage node B’s  voltage level to rise. This caused the access data to be reversed   $(1{>}0)$   for storage node A, Fig.6

![Stronger  IPG  IPD  Weaker  y+o  BLB   B  CH  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d4a5aca0-2a70-4b93-8b55-f9da7c6b3540/d4a5aca0-2a70-4b93-8b55-f9da7c6b3540.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215659%3B1743219259&q-key-time=1743215659%3B1743219259&q-header-list=host&q-url-param-list=&q-signature=42da41786375d68f39d9234b7b90c9dbd6799d32)
Figure 6 Access data was reversed for Storage Node A

Node A at “L” voltage level turned on the PUR device, which  then caused storage node B to rise to an “H” voltage level,  causing the access data to be reversed   $(0->1)$  , Fig.7

![Stronger  IPG  PILJR  IPD  on-   Weaker  BLB  EH   H  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/add6db8f-ebc2-4ec0-acf8-27edad28db86/add6db8f-ebc2-4ec0-acf8-27edad28db86.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215659%3B1743219259&q-key-time=1743215659%3B1743219259&q-header-list=host&q-url-param-list=&q-signature=292cfe39a825e280fd081480d4d09737a8594161)
Figure 7 Access data was reversed for Storage Node B

According to descriptions above, when the SRAM memory  operations is at a high temperature state, it exacerbated the  threshold voltage of the cell device and made it grow weaker.  Thus, we considered that the SRAM memory had a high rate of  read stability failure under high temperature operation.

Causes for read stability failure include cell devices with  lower threshold voltage degraded faster within a 12hr period.  Under the SRAM memory accelerated stress with both higher  bias and higher temperature   $(125\,^{\circ}\mathrm{C}\,)$  ) conditions exacerbated  threshold voltage of cell transistors.

A further cause was due to the threshold voltage variation in  implant process during wafer fabrication. The main  contribution was from random dopant fluctuation effect, which  had a great impact on the variation of the number of dopant  atoms, which directly affects the threshold voltage of  MOSFET.

## IV. C ONCLUSION 

Most companies calculated the operation life time directly  using the empirical value   $\mathrm{Ea{=}0.7e V}$  , which does not indicate the  true value of the different products. SRAM is quite a mature  product. It is very difficult to calculate Ea value with large  amounts of failures in a short time. However, this method is  based on the characteristics of the SRAM product and combined  with accelerated experiments; the calculation uses the statistical  distribution mode. As the Stress time increased, the minimum  operating voltage was raised gradually, which represented the

minimum operation degradation of the IC product; we then used  this change in operation voltage to calculate the Ea. This  accelerated stress time is shorter than that of other known  companies because this method can reduce a lot of test time in  accelerated stress tests.

## A CKNOWLEDGMENT 

I would like to thank all colleagues and partners who contributed  to this study and thanks for my wife and daughter support.

## R EFERENCES 

[1]    Robert Entner, Modeling and Simulation of Negative Bias Temperature  Instability, 7.3 6T SRAM Cell,2007.     [2]    Arrhenius, S. A. (1889). "Über die Dissociationswärme und den Einfluß  der Temperatur auf den Dissociationsgrad der Elektrolyte". Z. Phys.  Chem. 4: 96–116. doi:10.1515/zpch-1889-0408.    [3]    Jump   up   to:a b Arrhenius,   S.   A.   (1889).   "Über   die  Reaktionsgeschwindigkeit bei der Inversion von Rohrzucker durch  Säuren". Z. Phys. Chem. 4: 226–248.    [4]    Jump up to:a b Laidler, K. J. (1987) Chemical Kinetics, Third Edition,  Harper & Row, p.42    [5]    Huang, Chia-Sheng, Abstract NOR Flash New EA Extracted Method-Using the variation of FG Electrons concentration, 2017 IPFA.

