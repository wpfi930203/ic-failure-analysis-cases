---
title: "297_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_9d1dc401e301f207b05ae6e91dc276257295230462135641
file_size: 589295
---

## Breakdown Voltage Impact on Lifetime of 1200V  IGBT modules under H3TRB-HVDC Testing  

HaiTao Deng \* , JinLei Meng, Daniel-Bo Wang and Wenliang Zhang   Department of Power Electronics, ABB (China) Ltd., No.10 JiuXiangQiaoBei Road, Beijing, 100015, China.  \* Phone: +86-10-6423-3111   Fax: +86-10-6423-1649   Email:  Haitao.deng@cn.abb.com

Abstract-   The focus of the High Humidity High Temperature  Reverse Bias with High DC Voltage (H3TRB-HVDC) is the  quality of the chips and the package of the IGBT modules. For  H3TRB-HVDC, the blocking voltage of  $\bf{80\%}$   normal voltage was  applied to the samples instead of 80V bias. In order to confirm  that whether the measured breakdown voltage has influence on  the lifetime of IGBT modules, two groups of samples with  different breakdown voltage used in this paper. The test results  shown that the lifetime was positively correlated with the  breakdown voltage. The failure spot was found out at edge  terminal edge passivation layer of IGBT chip by the failure  analysis.

Keywords  –   Breakdown voltage, IGBT, H3TRB-HVDC,  Lifetime, Failure Analysis .

## I. I NTRODUCTION 

Insulated Gate Bipolar Translator (IGBT) modules have  important application in various fields, such as automotive  electronics, photovoltaic inverter, frequency converter and so  on. H3TRB-HVDC test, an abbreviation for High Humidity  High Temperature Reverse Bias with High DC voltage, aims to  find out the weaknesses of the chips or/and the package of  1200V IGBT modules due to moisture penetration. As we  know, the moisture penetrates the package along the inside  delaminated interfaces or diffuses through the silicon gel. That  would greatly influence the performance and reliability of  IGBT modules [1].

Usually,   the   H3TRB   testing   results   provided   by  semiconductor manufactures that the bias was commonly  limited to 80V to fulfil the general standard. In fact, the IGBT  modules biased with 80V did not show the degradation of the  blocking ability after 1000h at 85 degrees Celsius and 85  percent relative humidity. Nevertheless, the blocking voltage of  1200V IGBT module is approximate  $80\%$   of the normal voltage  (960V) in a practical application. It is well known that increases  in bias would greatly accelerate the H3TRB test [2-3].  Compared with the traditional H3TRB test, H3TRB-HVDC test  is more suitable for practical application.

This paper studied the relationship between the lifetime of  H3TRB-HVDC test and the static electrical characteristic  parameters for IGBT modules. Long-time applied high voltage,  high humidity, and high temperature accelerated the  degradation, general defects might occur around the electrical  field area. The failure analysis based on the known failure  modes was carried out for the failed samples after the  H3TRB-HVDC test [4-5]. This aims to find out the fragility of

the IGBT modules and provide   information that could be  improved for the design of IGBT modules.

## II.   EXPERIMENTS  

The test circuit for H3TRB-HVDC testing is shown in Fig.1.  The gate and emitter terminals of IGBT modules are shorted to  the grand or reversely biased by a low voltage power supply.  The positive voltage is applied to the collector-emitter terminals.  And a resistor is connected in series in the circuit for protection  purpose or leakage current measurement.

Fig.2 gives the overview schematics of H3TRB-HVDC  testing platform based on the test circuit as shown in Fig.1. The  physical view of H3TRB-HVDC setup is shown in Fig.3. This  test platform includes climatic chamber, data acquisition, PC,  High voltage DC power supply and cabinet for other equipment.  The climatic chamber is used for providing high temperature  and high humidity stress for IGBT modules. High voltage DC  power supply is used for applying high voltage to the  collector-emitter terminals. The PCB is designed to convert the  micro-ampere level leakage current into millivolt level voltage  by using high precision resistors. The voltage will be measured  by the NI data acquisition card.

![DUT  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7adbc616-7b96-4814-9d1e-d70621d526af/7adbc616-7b96-4814-9d1e-d70621d526af.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215712%3B1743219312&q-key-time=1743215712%3B1743219312&q-header-list=host&q-url-param-list=&q-signature=56877d1ab0e64a5ac617fef098f7eb2edd53cbe9)
Fig. 1 Test circuit for H3TRB-HVDC test

![IPC  Erheraet  NIeDAQ-s1744seh  Barksidelayou  I2VDC  sowree  high temperature and high humidity  lery data acquisition PCB    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/55293788-9b7f-4f6e-948b-97dff3778a60/55293788-9b7f-4f6e-948b-97dff3778a60.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215712%3B1743219312&q-key-time=1743215712%3B1743219312&q-header-list=host&q-url-param-list=&q-signature=65ad3fb200e448e384b30f3b4783eaa40248fdd7)
Fig. 2 The schematics of the H3TRB-HVDC platform

![NI Data acquisition  IDataaco  PC  Climatic chamber  Ciima  Cabinet for  abinet fol   other  other   High vo  High voltage   equipment  quipmen   DC power supply  C power sup    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c63b2040-1bd7-40e1-b7aa-761136d8dea4/c63b2040-1bd7-40e1-b7aa-761136d8dea4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215712%3B1743219312&q-key-time=1743215712%3B1743219312&q-header-list=host&q-url-param-list=&q-signature=9624551f1daa56c6532a85b5ee9e4bb64fe164aa)
Fig. 3 The physical view of the H3TRB-HVDC setup

As we all known, the leakage current can result self-heated of  the IGBT modules, which prevent a local reduction of the  moisture. Therefore, an additional heatsink is used to dissipate  heat caused by leakage current. Meanwhile, in order to decrease  the junction-to-ambient thermal resistance, the thermal grease  is painted between IGBT module and heatsink. Thus, the  junction temperature of IGBT module is very closed to the  chamber temperature.

The maximum limitation of the collector leakage current for  sample protection is set to 50mA. If the tested sample leakage  current surmounts this limitation, the data acquisition system  can remove the reverse bias for this sample to protect it from  further damage.

## III. R ESULTS AND DISCUSSION 

The Collector-emitter voltage   $\mathrm{V_{CE}}$   and the continuous DC  collector current IC of IGBT modules tested in this paper are  1200V and 150A respectively. The detailed test conditions are  as follows:

The static testing items and conditions for the parameters and  curves are listed in Table I. The IGBT modules were performed  with the static testing before H3TRB-HVDC testing.   In order to confirm that weather the measured value of  breakdown voltage has influence on the lifetime under the same  bias voltage stress. The samples were divided into two groups  based on the measured results and each group contained 3  IGBT modules. The breakdown voltage range of one group (A)  is 1300V\~1350V, and another group (B) is   $1350\mathrm{V}{\sim}1400\mathrm{V}$  .  Fig.4 shows the IGBT breakdown curves of group A and group  B which were tested with the static characteristic test  equipment.

Table I - The Testing Static Items and Conditions

|Test|Test Items|Conditions|Unit|
|---|---|---|---|
|Parameters|V CEsat|V GE =15V, I C =150A|V|
|Parameters|V GE(th)|I C =5.30 mA, V CE =V GE|V|
|Parameters|I GES|V CE =0V, V GE =20V V CE =0V, V GE =-20V|nA|
|Parameters|I CES|V CE =1200V, V GE =0V|μA|
|Parameters|V (BR)CES|V GE =0V, I C =1mA|V|
|Curves|Breakdown curves|V GE =0V, I C =1mA|V|


![12  GroupA  131SV-1325V  GroupB  1363V-1377V  02  1100   1150   1200   1250   1300   1350   1400   1450   1500  Breakdown voltage (V)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/099519d1-aa4d-4069-905b-949fb282fc2d/099519d1-aa4d-4069-905b-949fb282fc2d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215712%3B1743219312&q-key-time=1743215712%3B1743219312&q-header-list=host&q-url-param-list=&q-signature=3def668448631f3cbe2909db47548f95ce4fe4ba)
Fig. 4 The breakdown curves of Group A and group B

For the H3TRB-HVDC testing, the predominant failure  parameter is the leakage current I CES  which   is the key parameter  for failure criteria. The leakage current I CES  of the samples in  each group were measured each six minutes during the 1000  hours burn-in testing. The failure criteria for IGBT modules  H3TRB-HVDC test is that leakage current is less than   $100\upmu\mathrm{A}$    during the whole aging period.

Fig.5 shows the leakage current I CES  change of group A and  group B track of the aging time. For group A samples, the  leakage exceeded failure criteria at the beginning stage or after  hundreds of hours. The sample almost have no immunity to the  burn-in testing. For group B samples, the leakage current didn’t  exceed failure criteria during the whole burn-in test. The groups  B samples are ability to withstand at least 1000hrs burn-in  testing.

![Chart AreaEs (μA)  10000  GroupA  L004  l00Afa  100  GroupI  Time(hrs)  1-0-0   200   300   400   S00   600   200   800   900   1000  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/461bf5dc-4389-457c-baae-1ac4190708dd/461bf5dc-4389-457c-baae-1ac4190708dd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215712%3B1743219312&q-key-time=1743215712%3B1743219312&q-header-list=host&q-url-param-list=&q-signature=267122197b4aeb3f126e672587c304c130f380f8)
Fig. 5 The collector leakage current change with aging time

The results from experimental indicate that group A samples  have no immunity and group B samples have absolute  immunity for 1000hrs H3TRB-HVDC testing. There is almost  no failure occurs when the breakdown voltage of IGBT  modules is large than 1350V under high humidity   $(85^{\circ}\mathrm{C})$  , high  temperature (  $85\%$   RH) and high voltage (  $80\%$   normal  breakdown voltage).

In Fig.6, the relationship between the lifetime and the  measured breakdown voltage were extracted. For group A  samples, the lifetime of the different measured breakdown  voltage was 25.9hrs, 470.6hrs and 525.8hrs respectively.  For

group B, the lifetime of all the samples exceeded 1000 hrs. it  was found that the lifetime was positively correlated with the  measured breakdown voltage.

![1000  Maximum aging time10o0 hours  900  800  70O  600  o525.8hrs  500  470.6hrs  400  300  200  100   25.9hrs  1310   1320   1330   1340   1350   1360   1370   1380  The measured breakdownvoltage (V)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3dd07b84-0c6a-4247-817f-cc7f95ec07b9/3dd07b84-0c6a-4247-817f-cc7f95ec07b9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215712%3B1743219312&q-key-time=1743215712%3B1743219312&q-header-list=host&q-url-param-list=&q-signature=cb83a80b3205ca50af6e9bdfdde3cfaccf1a0396)
Fig. 6 The relationship curve of lifetime and the measured breakdown voltage

The static parameters testing was carried out before and after  the H3TRB-HVDC burn-in testing according to the test items  and conditions of Table I. The failed static parameters of the  samples from group A were shown in Tab II. It can be seen that  there are two failed static parameters included I CES  and V (BR)CES .  Two parameters I CES  and V (BR)CES  essentially reflect the  blocking ability of the samples.  The test results indicated that  the H3TRB-HVDC testing only affects the reverse blocking  ability of the IGBT modules.

Table II – The test results of static parameters before and after H3TRB-HVDC

|Static Parameter|Test Condition|Unit|Measured Value|Measured Value|Measured Value|
|---|---|---|---|---|---|
|Before H3TRB-HVDC testing|Before H3TRB-HVDC testing|Before H3TRB-HVDC testing|Before H3TRB-HVDC testing|Before H3TRB-HVDC testing|Before H3TRB-HVDC testing|
|I CES|V CE =1200V, V GE =0V|μA|0.1|0.1|0.2|
|V (BR)CES|V GE =0V, I C =1mA|V|1318|1325|1323|
|After H3TRB-HVDC testing|After H3TRB-HVDC testing|After H3TRB-HVDC testing|After H3TRB-HVDC testing|After H3TRB-HVDC testing|After H3TRB-HVDC testing|
|I CES|V CE =1200V, V GE =0V|μA|1.0|1.0|1.0|
|V (BR)CES|V GE =0V, I C =1mA|V|1075|1186|1096|


There are two aspects that can affect the H3TRB-HVDC  reliability of the IGBT modules through literature investigation  [6-7]. The most important aspect is the chip technology,  including the design of the junction termination, the chemical  component of the metallization, and the passivation layer on the  topside of the chip. The second important aspect is the  packaging technology, mostly related to the silicone gel inside  of the module, and the materials of the bonding wire and solder  layers.

In order to analyze the failure cause of group A samples  based on the above two failure parameters, the failure analysis  was carried out in this paper. The failure spot of 525.8hrs failed  modules was observed using the optical microscope. Fig.7  shows the breakdown spot and the leakage current directions.  However, there are no significant failure point for two other  failed modules.

For IGBT chip, the leakage current is usually generated by  two areas, as shown in Fig.8. One area is in the internal PN  junction of active area. The other one is the surface of edge  termination area and passivation layer. According to the failure

analysis result, the leakage current is caused by the surface  degradation of edge termination area and passivation layers.

![Leakage current  downspot   direction  Edgete  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a39106ab-ff4f-4cf0-ae5f-58d9d2c3d2bc/a39106ab-ff4f-4cf0-ae5f-58d9d2c3d2bc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215712%3B1743219312&q-key-time=1743215712%3B1743219312&q-header-list=host&q-url-param-list=&q-signature=21b9b3e16a04aab239f5333423d8f008ad1b703c)
Fig. 7 The failure spot and the leakage current direction.

![Active Area  EdgeTermination and  passivationlayer  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a2f52b25-aaa7-43eb-852c-411260704c40/a2f52b25-aaa7-43eb-852c-411260704c40.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215712%3B1743219312&q-key-time=1743215712%3B1743219312&q-header-list=host&q-url-param-list=&q-signature=3cde74ca9cb3f8e5d296d69373aba296166c97e3)
Fig. 8 The top view of IGBT chip.

From Fig.7, it shows that the main damage is located at the  outermost edge of the edge termination and passivation layer.  The chip edge termination area should be protected by  passivation layer. However, moisture penetrated inside the  passivation layer by the gap between the metallization layer and  the passivation layer at the outermost edge during the  H3TRB-HVDC testing. Meanwhile, the strongest electrical  field position was located at this edge termination area. The  metal corrosion can be most likely occurred under the  combined conditions of the moisture penetration and the strong  electronic fields.

To summarize, the possible failure mode of 525.8hrs failed  module is aluminum corrosion located at the outermost edge  termination of the IGBT chip. In the future, a deeper analysis of  the failure mechanism on edge termination area is necessary.  For two other modules, the failure mechanisms need to be  further analyzed.

## IV. C ONCLUSION 

In this paper H3TRB-HVDC test was carried out at bias  levels up to   $80\%$   nominal voltage on two groups to investigate  the relationship between lifetime and the breakdown voltage.  All of the group A samples failed at the beginning stage or after  hundreds of hours. however, all of the group B samples didn’t  fail after 1000 hours of H3TRB-HVDC. It can be seen that the  IGBT modules have immune effect under high humidity high  temperature with    $80\%$   nominal voltage bias when the  breakdown value reach to and/or greater than 1360V. The result  of failure analysis indicated that the leakage current spot was  located at the outermost edge terminal of IGBT chip. The  design of edge terminal should be improved to enhance IGBT  modules reliability.

## A CKNOWLEDGMENT 

Thanks to River-Tinho Li for his support and advice in  H3TRB-HVDC experiment and failure analysis. Thanks to  Jiefeng Zhi and Haoshi Li for the testing work done in this  project.

## R EFERENCES 

[1]    Christian Zorn et al., “Acceleration of Temperature Humidity Bias (THB)  Testing on IGBT Modules by High Bias level,”  Proceedings of the 27th  International Symposium on Power Semiconductor Devices & IC’S , pp.  385-388, May 2015.    [2]    Jianwei zhou et al., “Insulation Degradation and Bias Acceleration Effect  study under THB Test,”  8th International Conference on Electronic  Packaging Technology , pp. 1-4, August 2007.    [3]    Christian Zorn et al., “Temperature Humidity Bias (THB) Testing on  IGBT Modules at High Bias Levels,”  8th International Conference on  Integrated Power Electronic Systems , pp. 1-7, February 2014.    [4]    Daniel Minzari et al., “Electrochemical Migration on Electronic Chip  Resistor in Chloride Environments,”  IEEE Transactions on device and  materials reliability , vol.9, no.3, pp. 392-402, September 2009.    [5]    Christian   Zorn   et   al.,   “Temperature-humidity-bias   testing   on  insulated-gate bipolar transistor modules-failure modes and acceleration  due to high voltage,”  IET Power Electron. , Vol.8, Iss. 12, pp. 2329-2335,  July 2015.    [6]    Eric D. Sword et al., “Humidity-Induced Damage in polyvinyl Toluene  and polystyrene plastic scintillator,”  2017 IEEE international symposium  on technologies for homeland security (HST) , pp.1-4, March 2017.    [7]    Huang JiaoYing et al., “Analysis of water Vapor Control and passive  Layer Process Effective on transistor performance and Aluminum  Corrosion,”  2014 prognostics and system health management conference  (PHM-2014 Hunan) , pp. 26-30, August 2014.

