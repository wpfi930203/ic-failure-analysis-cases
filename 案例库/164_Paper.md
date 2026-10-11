---
title: "164_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_c7021dd28cf4d4238ad101a795c0378c7295230462135641
file_size: 1319201
---

## Systematic Study on Failure Information of Thick  Film Hybrid Integrated Circuit  

Zhang xiaowen  1, L v hongjie  2, L iu xing  1 \*     1 Science and Technology on Reliability Physics and Application of Electronic Component Laboratory, 110 DongGuangZhuang  Road, Guangzhou, 510610, China.    2 No.43 Research Institute of China Electronics Technology Group Corp,  19 Hehuan Road, High-tech Zone, Hefei, 230088, China.   \* Phone: +86-020-87237725   Fax: +86-020-87237017   Email:  zhangxw@ceprei.com

Abstract-    Through the statistical analysis of failures of   components and interconnect in thick film HIC(Hybrid  Integrated Circuit), the failure mode and failure mechanism  affecting the reliability of HIC has been studied. Based on the  analysis of the factors which affecting the reliability of thick film  HIC, the failure mode and failure mechanism were summarized. 4  cases of failure analysis of thick film HIC were presented, and the  typical failure modes and failure mechanisms of the thick film  HIC were analyzed, which support the summary. Finally, based  on the failures analysis reports accumulated over many years, the  statistical analysis of the failure parts has been conducted to study  the main factor which dominate the reliability of thick film HIC. It  is indicating that the failure of components is the main cause of the  failure of thick film HIC, followed by the failure of wire bonding  and internal interconnection. In addition, some of the failures are  caused by external factors. Since the failure of active devices is the  main failure mode of thick film HIC, the selection of highly  reliable components is an effective way to improve HIC reliability.  Secondly, if necessary, optimize the soldering process to improve  the reliability of the components in thick film HIC.

Keywords  –  HIC reliability, statistical analysis, failure mode,  failure mechanism .

## I. I NTRODUCTION 

Thick film HIC(Hybrid Circuit) is the result of thick film  integration   technology   and   semiconductor   technology.  Compared with discrete components, it has the advantages of  small size, light weight, short circuit path, easy control of  parasitic parameters, it has less interface of intermetallic and  good ability to resist the vibration and shock, so it has higher  reliability. Because the hybrid circuit is composed of pre-tested  function block, the system is easy to test and fault tracking is  easier. Compared with monolithic ICs, the advantages are that  the changes of design  are easy, the sampling cycle is short, the  production can be started as soon as possible, high-performance  components (substrates and external components) can be  selected, components of different processes can be mixed and  assembled, and rework can be facilitated. It can Produce  complex circuits with reasonable yield and suitable for small  and medium batch production[1-2]. Therefore, thick film HIC  is widely used in satellite, radar, remote and data  communication, computer, industrial instrumentation and other  electronic equipment. As a circuit module, it contains a series of  components inside, each component and interconnection  structure may be failure during operation condition, which

resulting in various failure modes and failure mechanisms  during field usage.

many literatures have studied the reliability and failure  mechanism of thick film HIC, analyzed the reliability problems  of thick film HIC design and process, studied the root cause and  improvement suggestions of hybrid circuit failure, the main  factors affecting the reliability of thick film HIC has been  proposed Under different application environments stress, the  temperature characteristics of thick film HIC were further  studied, and the relationship between output voltage and  temperature was tested. Using the failure physics analysis  method, the reliability of key devices in the thick-film  switching power supply is studied, and the data of activation  energy and lifetime time of the key device failure mechanism  are obtained. However, there is still a lack of systematic  analysis and research on the main failure modes and failure  mechanisms in thick film HIC [3-11].

In view of the above reasons, based on the multi-layer HIC  failure analysis report accumulated over the 10 years, this paper  analyzes and studies the typical failure modes and failure  mechanisms that occur during the field usage, and then  statistically analyzes the failure numbers of various failure  parts, active devices and interconnection wiring With the  percentage, so as to clearly understand the main reliability  influencing factors in the use of thick film HIC, on this basis,  the method of improving the reliability of thick film HIC is  discussed. The research results are beneficial to the process to  control the main failure mechanism and improve the reliability  of HIC.

## II.   F AILURE  M ODE AND  M ECHANISM  A NALYSIS OF  T HICK  F ILM  HIC  

The factors Analysis of affecting the reliability of thick film  HIC. Through literatures research, thick film HIC failure  analysis report and the accelerated life test of thick film HICs,  the main problems affecting the reliability of thick film HIC can  be summarized into the following reliability of active devices,  internal wire bonding, contamination, substrate and package. In  addition to the above reliability concerns, since the HIC can be  used in Harsh environment, it may faces some other reliability  problems mainly caused by electrostatic damage and  irradiation.

Classification of the main failure modes and failure  mechanisms of thick film HIC. The thick film HIC contains a

series of components, the product can only work under the rated  temperature range and the specified load. In practical operating   condition, each component and interconnection in thick film  HIC may fail, which resulting in a variety of The failure mode  and failure mechanism, the failure mode and failure mechanism  are generally shown in Table1 [3-9]

T ABLE  I   -    THE MAIN FAILURE MODE AND MECHANISM OF THICK FILM  HYBRID CIRCUITS

|Failure mode|Failure component|Failure mechanism|
|---|---|---|
|electrical|Discrete device 、 IC|Parameter shift|
|Parameter shift|resistor 、 capacitance|Parameter shift|
|open|Discrete device 、 IC 、 Bonding wire|Solder layer fatigue 、 Organic paste layer aging  ， Bonding wire corrosion|
|short|Discrete device 、 IC 、 Bonding wire  、 solder|Sn ion migration in solder 、 Ag ion migration in conductive paste  、 the touch between Bonding wire and chip or between wires|


## III.   F AILURE ANALYSIS OF TYPICAL PRODUCTS   

## (1) Failure Analysis of VDMOS in thick film HIC  

The failure information of the thick film HIC is that: the input  resistance of the sample is low. After measuring, it confirmed  that the shutdown resistance of the VDMOS inside the thick  film HIC module is 880 Ω . According to the specification, the  VDMOS   should   have   a   shutdown   resistance   of   $60\mathrm{k}\Omega{\sim}80\mathrm{k}\Omega.$  .The I/V characteristics of the VDMOS of the  sample   were   measured   after   disconnected   peripheral  components. The results showed that between the gate and  source, and between the gate and drain of the VDMOS, there is  a current leakage path.

Failure analysis of the failed VDMOS was carried out by  using OBIRCH (Optical Beam Induced Resistance Change). A  voltage of 1.1V was applied between the terminal of drain and  source of the sample, which induced  a leakage current of  1.06mA, then the hot spot region on the failed sample was  detected by using OBIRCH, indicating that there was a current  hot spot on the surface of the VDMOS, as shown in Fig. 1.

![5X1.1V1.06mA    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3741aea4-81b2-47ae-911d-eaac41a58d46/3741aea4-81b2-47ae-911d-eaac41a58d46.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215639%3B1743219239&q-key-time=1743215639%3B1743219239&q-header-list=host&q-url-param-list=&q-signature=8d46e479f93af3a9b462c6ff505a13d4ace5b89c)
Fig. 1 the result of OBIRCH analysis on the VDMOS

After removing the metalized layer on the surface of the  sample, and observed under a metallographic microscope, it is  discovered that the dielectric layer in the hot spot region  appeared to have damage. In order to obtain the clear image of

the hot region, the SEM is used to observe the hot region of the  failed VDMOS again, it can be seen clearly that the dielectric  layer in the hot region is damaged as shown in Fig. 2.

![SD   WD20.7mm10.0kVx3.0k10um  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d4323002-d522-48d9-beb2-557442ed3557/d4323002-d522-48d9-beb2-557442ed3557.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215639%3B1743219239&q-key-time=1743215639%3B1743219239&q-header-list=host&q-url-param-list=&q-signature=1d63d54e4b44105ab27313a81ee78a1bbd994ce3)
Fig. 2  the  SEM image of failed cell on the VDMOS.

(2)Failure Analysis of Transformer in Thick Film HIC

A thick-film HIC with metal Hermetic seal failed during an  accelerated test. The method to do the accelerated test is to  increase temperature to the maximum value depicted in the  specification at a step of 10 Celsius started from 20Celsius. The  temperature stress on the sample maintained 48h per  temperature point, and the electrical parameters were tested per  24h until the temperature maximum was reached. During the  accelerated test, when the temperature rose to   $150\,^{\circ}\mathrm{C}$   with full  load the output was abnormal. The results is that when the input  voltage is 12.5V with no load, the sample has an output voltage  of 5.0V, but when the input voltage is 12.5V with load, the load  current is more than   $200\mathrm{mA}$  , in the same time the output  voltage decrease to zero. The electrical measurement results are  shown in Table 2.

T ABLE .II   -    HYBRID CIRCUITS THE OUTPUT VOLTAGE MEASUREMENT  UNDER DIFFERENT LOAD

|Input voltage (V)|Input current (mA)|Load current (mA)|Output voltage (V)|Output current (mA)|
|---|---|---|---|---|
|12.5|318|No load|5.0|0|
|12.5|387|200|0|0|


Decapsulation is done to expose the internal features of the  thick-film HIC for further FA, it was observed that the  transform in the sample was carbonized or turn yellow, and  there were obvious signs of overheating. The ferromagnetic  notch of the transformer showed the partial peeling appearance  of the transformer insulation layer. The resistance between the  pin 1 and the pin 14 of the sample (which corresponding to the  primary coils and secondary coils of the transformer) is  measured, and the measurement value vary between  $40\mathbf{k}\Omega$   and  3M Ω . Picking up the bottom of the transformer, there are signs  of burnt and discolored. After removing the transformer, gently  bypass one end of the coil, and the insulation layer between the  wires falls off. The typical shape is shown in Fig. 3.

The failure analysis results showed that when the sample is  subjected to high temperature test, the insulating glue between  the transformer coil are gradually cracked at high temperature,  which damaged the insulation layer between the transformer  coils and the current leakage occurs. When the output power

increases, the input current made the PWM chip trigger over  current protection, led to output voltage decreased to zero. The  power generated by the leakage current in the transformer  causes the temperature of the transformer to rise continuously,  resulting in carbonization and cracking of the insulating layer,  and sample failed eventually.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2281debf-6492-4451-9348-e9faa149dcd4/2281debf-6492-4451-9348-e9faa149dcd4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215639%3B1743219239&q-key-time=1743215639%3B1743219239&q-header-list=host&q-url-param-list=&q-signature=f9694d517f111e16e397db8ae338b8b976f833da)
Fig. 3 the insulator layer on the transformer coil fall off.

(3)Failure Analysis of Interconnect Structure in Thick Film  HIC

A thick film HIC with metal Hermetic seal failed during the  temperature cycle test of the whole machine. When the failure  occurs, the sample was experiencing the 10th high temperature  phase in the whole machine (the machine was powered on at the  high temperature phase and the low temperature phase during  the test, but the power was switched off at the temperature  transition region). When the sample failed, there was no voltage  output. According to GJB548B-2005 method 1018, the internal  water vapor content of the sample was tested, and it was found  to be  $24.3\%$   in the sample cavity, more than the requirement of  not exceed 5000ppm in the standard. The sample was unsealing  by mechanical method, and the morphology was observed  under the microscope. It was found that the bond wire of the  base of a triode was fused inside the sample, and The bonding  wire of the positive electrode of a diode is also burned down,  and the shape of the breaking is the same, showing signs of high  current burnout, and the surface of the two chips is intact, as  shown in Fig. 4 and Fig. 5.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/864f1295-890d-4eda-b607-be3cb2a19c26/864f1295-890d-4eda-b607-be3cb2a19c26.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215639%3B1743219239&q-key-time=1743215639%3B1743219239&q-header-list=host&q-url-param-list=&q-signature=8ccf8c27bf23bb4f781ee81b23d34f49184eeafc)
Fig. 4   t he fuse of gold wire on the base of the bipolar.

Subsequently, two chips were tested to check whether the pn  junction had a breakdown. First, the triode was measured, the  reverse breakdown voltage of the e and b junctions of the triode  was  $\mathrm{V}\mathrm{e}\mathrm{b}{=}11\mathrm{V}$  , and the reverse breakdown voltage between the  c and b junctions was   $\mathrm{Vcb=}170\mathrm{V}$  . The reverse breakdown

voltage between the c and e junctions. was  $\mathrm{Vce=}110\mathrm{V}$  . Then the  diode was measured, and its voltage regulation value is 12V.  From the above measurement data, it is indicated that no  breakdown occurs in both chips. After the Decapsulation, it can  be seen from the failure position inside the circuit that the  failure occurs in the auxiliary power supply circuit (see Fig. 6  for the partial schematic diagram), which shows that the high  current burned down the bonding wires connected to the base   of the triode and the positive electrode of the Zener diode  respectively.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/db0044c7-68e5-4b1c-81c3-20165fbaa4eb/db0044c7-68e5-4b1c-81c3-20165fbaa4eb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215639%3B1743219239&q-key-time=1743215639%3B1743219239&q-header-list=host&q-url-param-list=&q-signature=f2573aa77953cbfba81eb0d028bb141417f7f6af)
Fig. 5   t he fuse of gold wire on the base of the bipolar.

![PIN3 (+28V)  PIN3 （ +28V ） PWM  PWM Failure  Failure    circuit  circuit 15K 15K     The bonding  The bonding     wire fused  wire fused PIN5（-)  PIN5 （ - ） ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d9c0f9a5-af5a-436f-9db5-70a91fc97060/d9c0f9a5-af5a-436f-9db5-70a91fc97060.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215639%3B1743219239&q-key-time=1743215639%3B1743219239&q-header-list=host&q-url-param-list=&q-signature=a0c9631697600979c4c018bbca32b9c39a5a50e2)
Fig. 6  the local schematic within the sample.

From the analysis of the circuit, if the current is introduced  from the collector or emitter of the triode, If the bond wire  connected to the base fused, not only the triode will be  Breakdown, and since the current passing through the collector  and emitter is more larger, the bond wire connected to the  collector and emitter should be also burn out, but in fact the  triode function well and the bond wires connected to the  collector and emitter is not damaged.

However, when the pulse current is introduced from the  negative terminal of the circuit, the diode is forward biased, so  be the same with the PN junction between the triode b-c and b-e,  thus the equivalent resistance of the path decreased, and large  current will flow through the base of the triode and the diode.  Since the current flowing into the base of the triode will flows  out from the bonding wires connected to the collector and the  emitter, so the current flowing through the base of the triode  and the diode is the largest, which burned out the bonding wires  both connected to the base of the triode and the positive  electrode of the diode. Based on the above analysis, it can be

judged that the negative pulse introduced from the input end of  the sample generates a large instantaneous current in the circuit,  so that the bonding wires connected to the base of the triode and  the positive electrode of the diode are burned out which located  in the internal auxiliary power supply circuit of the sample,  resulting in the triode can’t be working properly, thus the  sample has no voltage output.

(4) thick film HIC failure analysis caused by external factors  A thick film HIC with metal hermetic seal has no voltage  output at room temperature after a temperature shock (no power  on) test. The package of the sample was intact, and there was no  abnormal appearance such as damage, corrosion, burning, etc,  and the glass insulator at the pin was not damaged. When the  voltage of 28V was applied to the input of the sample (the  normal input voltage of the sample), the input current shows  zero, and the output voltage is also zero. It is indicted from the  measurement that the input of the sample was open.

After Decapsulation, The failed sample was observed under  the microscope. There were many abnormal topography nearby  the internal pin 6 (Positive Input), in which the bond wire  connected to the source of the VDMOS were burned out(Fig.7),  the bond wire of the triode is also broken(Fig.8), and the  metalized wiring on the surface of the triode chip also shows  signs of burning. In addition, the metalized wiring connected to  the grounding line of the PWM chip also has burnt marks. The  partial schematic diagram of the circuit where the components  of the burnt are located is shown in Fig. 9. It can be seen from  the figure that all the bonding golden wire burnt are connected  to the ground, which are characterized by instantaneous over  current burning.

![Spherical at the breakpoint  Spherical at the breakpoint  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c69753fa-b585-4005-91d0-1f11c230c3af/c69753fa-b585-4005-91d0-1f11c230c3af.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215639%3B1743219239&q-key-time=1743215639%3B1743219239&q-header-list=host&q-url-param-list=&q-signature=8416fd2144c97322a565fb798d0bd62130cbcdac)
Fig. 7  the local schematic within the sample.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/15e6020c-5a5f-4e2a-9e94-31fcbd72781d/15e6020c-5a5f-4e2a-9e94-31fcbd72781d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215639%3B1743219239&q-key-time=1743215639%3B1743219239&q-header-list=host&q-url-param-list=&q-signature=d85a6c36a32af8bd4a488e69e893503795e03f70)
Fig. 8  the broken of gold wire on the anode of diode

![0oo  VCC WCC  Input + Input-D PWM  PWM G S Input-  Input -  GND  GND ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/16b37cf8-6cca-4589-90c9-41a7f8d6402f/16b37cf8-6cca-4589-90c9-41a7f8d6402f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215639%3B1743219239&q-key-time=1743215639%3B1743219239&q-header-list=host&q-url-param-list=&q-signature=65e96e2c28328f12018a2e9226fdab962739a7ed)
Fig. 9  the part schematic relative to the burn out within the sample  Therefore, the failure of the sample was that the negative  terminal of the input was incorrectly connected to the voltage of  28V, and an large current was generated in the circuit, so that  the bonding wires of the diode and the triode in the input circuit  were fused, led to the input circuit open, thereby causing the  sample Output fail.

## IV. T HICK FILM  HIC  FAILURE INFORMATION STATISTICS 

The failure of thick film HIC can be attributed to one or more  of the following reasons: case seals, substrates, contamination,  wire bonding, internal interconnects, components, and failures  caused by external factors. Based on statistical analysis of 40  failure analysis reports of thick film HICs, the number of  failures for various failure modes, and the percentage of failure  for various failure modes are listed in Table 3. Among them, the  number of failures of components and interconnects and the  percentage of failure are listed in Table 4.

T ABLE  III   -    THE FAILURE PERCENTAGE OF ALL SORTS OF FAILURE MODE

|Part|Number|percentage|
|---|---|---|
|Base seal|1|2.2%|
|substrate|0|0|
|contamination|1|2.2%|
|wire bonding|8|18.2%|
|internal interconnect|3|6.6%|
|component|27|61.4%|
|external factor|4|8.8%|


T

ABLE   IV   -    THE FAILURE PERCENTAGE OF ALL SORTS OF COMPONENT

|device|Number|percentage|
|---|---|---|
|diode|4|10.5%|
|VDMOS|4|10.5%|
|chip|9|23.7%|
|Optocoupler|0|0.0%|
|resisteror|1|2.63%|
|capacitor|3|7.89%|
|Transformer|6|15.8%|
|interconnect|11|28.9%|


It can be seen from Table 3 that the failure of component is  the main cause of the failure of thick film HIC. The failure of  active devices exceeds   $61\%$   of all failures. In general, the  failure of component passes through three failure stages,  namely early failure, random failure and wears out failure. The  failure of wire bonding and internal interconnects accounts for  approximately   $24\%$   of the total failure of thick film HIC and

ranked second in the failure cause of thick film HIC. In  addition, some of the failures are caused by external factors,  which may be caused by a misconnection of the positive and  negative terminals of the power of the circuit during operation,  or an excessively high input voltage is introduced externally,  resulting in failure of the circuit module.

At the same time, from the statistical data in Table 3,  contamination failure is not the main cause of thick film HIC  failure, but many other types of failure can ultimately be  attributed to the cause of contamination. For example,  conductive particles from epoxy, solder, wire bonding, and  encapsulation can cause short between the two conductors.

Among the failure ratios of the components, the failure of the  chip dominated, and the total failure of the switching transistor  and the chip exceeds   $34\%$   of all failures, which indicates that  the reliability of the chip influences the overall reliability of the  thick film HIC. The failure of the transformer also accounts for  a certain proportion, but the maximum proportion of all the  failures is the interconnection, including the gold wire bonding  wire, the solder joints at the input and output, and the terminal,  but it is necessary to pay attention to the failure of gold bonding  wire, which are often caused by other failure mechanism.

## IV. C ONCLUSION 

In addition to the processing, the application environment  also has a great influence on the reliability of thick film HIC,  the failure mode and failure mechanism are also different due to  the difference of the application environment. If the thick film  HTCs fail in the same failure mode, the mechanisms of failure  can be different, it may be duo to electronic over stress, heavy  load, poor bonding, large thermal resistance or high junction  temperature. So when Analyzing the mechanism of failure of  thick film HIC, it is need to consider of the application  environment.

Since the failure of component is the main failure mode of  thick film HIC, the selection of highly reliable components is an  effective way to decrease the failure of thick film HIC in the  field. Secondly, if necessary, optimizing the mounting process  to eliminate the impact of the soldering temperature on the  reliability during mounting process.

## R EFERENCES 

[1]    James J.Licari Leonard R.Enlow. Hybrid Microcircuit Technology  Handbook[M].Beijing:  Electronic Industry Press , 2003.  [2]    LI Zhenya, ZHAO Yu. The Development and the Prospect of Hybrid  Integrated Circuit Technology[J].  Journal of china academy of  electronics and information technology , Vol.4 (2), pp.119-124, 2009.  [3]    Zhang xiaowen, He xiaoqi, En yunfei. The process and environment of  failure in Hybrid Integrated Circuits[C]. Chongqing ： The 15th Conference  on Semiconductor Integrated Circuits and Silicon Materials , pp:435-439,    2007.\`  [4]    LUO Jun, QIN Guolin , LI Xiaohong etc. Reliability Techniques for  Hybrid Integrated Circuits [J]. Microelectronics , Vol.41(1), pp. 111-115,    2011   [5]    Zhang xiaowen, LU hongjie, He xiaoqi, etc. Study on Reliability  Evaluation Method for DC/DC Power Module [J].  Microelectronics ,  Vol.47(6), pp. 111-115, 2017    [6]    Zhang xiaowen, LU hongjie, He xiaoqi, etc. Study on Reliability  Evaluation Method for DC/DC Power Module based on the calculation of  active energy [J].  Electronics & packaging , 2018(10), pp. 9-12     [7]    Zhu chunjie. Research on Reliability of VDMOS of Key Devices in  DC/DC   Power   Modules[D].   Beijing   : Beijing   university   of  technology ,2008.     [8]    Zhang jie. Research on Reliability of Key Devices in Switching Power  Supply[D]. Beijing : Beijing university of technology ,2008.    [9]    Liu yang, LV Changchi, Xie Xuesong, etc. Reliability lifetime estimate  for DC/DC Converter[J].  Journal of functional material and devices ,  Vol.16(3):266-270,2010.     [10]   MIL-HDBK-338. Electronic reliability design handbook[S].    [11]   GJB299C-2006. Reliability prediction hand book for electronic  equipment[S].

