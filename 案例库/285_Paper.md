---
title: "285_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_9e76f9bea88bac1c182eeee8215d5d797295230462135641
file_size: 464941
---

## Failure Analysis of Microwave Module by ESD  Effect  

Zhimin Ding, Chao Duan, Xiaoqing Wang, Zhaoxi Wu, Yang Tian, Meng Meng  1 Center of Failure Analysis Affiliation, China Academy of Space Technology, Beijing, China.  \* Phone: +86-185-010-32689   Fax: +86-10-6874-6312   Email:  dingzm1130@163.com

Abstract —In this paper, it is confirmed that the electrostatic  discharge is the cause of failure of the microwave module. The  confirmation is based on a series of failure analysis, simulation  tests as well as theoretical analysis on the failure case of a  microwave module. In order to ensure the microwave  performance, no electrostatic protection circuit was designed  during the production and application of microwave modules,  thus making the electrostatic discharge one of the main reasons  for microwave module failure. In this paper, the characteristics  of the harm of ESD toward microwave module are analyzed  and an improved method is proposed through verification test.  That is to add electrostatic protection measures around the  circuit. This case provides reference and basis for prevention  and control of electrostatic discharge hazards during  production and application of microwave modules in the  future.

Keywords - Microwave Module; Failure; ESD

## I.      I NTRODUCTION 

The microwave module is of high efficiency, convenient  utility and other advantages, which are of important  significance for radar, communication and other electronic  equipment to achieve complete solid state. With the  continuous progress of microwave technology, microwave  semiconductor devices have been widely applied to  microwave communication systems, telemetry systems,  radar, navigation, artificial satellites, spacecrafts and other  fields. However, quality and reliability problems during  utilization are also increasing day by day. Those reliability  problems have directly affected the systematic reliability of  the whole unit.  [1-2]

Compared with the conventional electromagnetic pulse,  the electrostatic discharge process is influenced by the shape  and the texture of object and the resistance value of  discharge circuit. Besides, the randomness of the discharge  process complicates the damage mechanism and the  consequent analysis. There are few studies on the  electrostatic damage of microwave module. In order to  guarantee the microwave performance of microwave  module, no anti-static design is made in the microwave  module, which makes it more sensitive to electrostatic  discharge. [3]  Thus, the study on electrostatic discharge  damage of the microwave module is of important  significance.

In this paper, the failure case of a microwave module was  analyzed, its failure was positioned, and at the same time the  failure mechanism was analyzed and verified in a manner of

experiment. The reason for the failure was confirmed to be  related to the abnormal voltage stress caused by electrostatic  discharge. Those have provided the basis for preventing the  impact of static electricity during microwave module  production and application in the future.

## II.    F AILURE  A NALYSIS  C ASE 

During the electrical testing on a microwave module in a  circuit system, it was found that the gain of the velocity  measurement receiving channel 3 was abnormal, decreasing  by 43dB.

A 5V of working voltage was applied to the microwave  module pursuant to its normal working condition. Then, the  module was tested by a multimeter. The output signal was  2.8V but it should have been 0V in normal condition; the  input signal of the amplification channel at the output end  was measured to be 0V (normal).  Thus, it was determined  that the abnormal condition exists at the amplifier channel at  the output end of the module.

An examination of the internal structure of the module  showed that the attenuator circuit at the output end of the  module was burnt, there was a breakdown trace existing on  the upper blocking condenser on the amplifier chip and the  field-effect tube grid was burnt. Next, the channel where the  prime amplifier locates was opened to check its internal  structure and no abnormal conditions were observed in  attenuator, blocking condenser and field-effect tube.

The burn morphology of output attenuator, output  blocking condenser and upper field-effect tube of amplifier  chip are shown in figure 1, 2 and 3, respectively.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3c0fe1fe-6d4d-4d10-b64d-57a6049c04e9/3c0fe1fe-6d4d-4d10-b64d-57a6049c04e9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=115243ece55e18da3c397fc492035d77558bebd1)
Figure 1.    Burnt Morphology of Output Attenuator of Module

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8590f2a2-bb62-46d5-adb6-dff30b42f3e8/8590f2a2-bb62-46d5-adb6-dff30b42f3e8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=179d03c74b14f229bbeb17df1871e0c8bead2068)
Figure 2.    Burnt Morphology of Output Blocking Condenser of Module

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7f8e52b0-4999-4fe8-a651-2732a8cabd87/7f8e52b0-4999-4fe8-a651-2732a8cabd87.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=9280ce3c7d03f111dc525213a698340228fcc3c4)
Figure 3.    Burned Morphology of Upper Field-Effect Tube of Amplifier  Chip

## III.    M ICROWAVE  M ODULE  F AILURE  A NALYSIS 

Under the normal working condition of the 5V power  supply voltage, the signal at the output end of the module  should have been 0V. However, the electrical test after  failure showed that the signal at the output end was 2.8V.  The internal examination of the module showed damages in  three components. The attenuator circuit at the output end  was burnt, there was a breakdown trace existing on the upper  blocking condenser on the amplifier chip and the field-effect  tube grid was burnt, respectively. According to the electrical  test and the damage traces inside the module, possibilities to  cause module failure are as following analysis in detail.

Firstly, three burnt devices were analyzed. The output port  of the module adopts a topological structure with negative  feedback as shown in figure 4.

![RC1  R1   R1  R2  RS  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f88b653c-6e17-4016-8029-a8307b134904/f88b653c-6e17-4016-8029-a8307b134904.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=c369c029cb18e41d3c773382422b68413d9c9828)
Figure 4.    Schematic Diagram of Cascade between Low Noise Amplifier  and Fixed Attenuator inside the Module

The DC bias network consists of the resistance Rd, the  inductance Ld and the resistance Rs. The typical value for  the normal operating current of the device is 30mA. In the  figure, the resistance Rd (20Ω) can withstand the current of  100mA and the Ld is choke inductor. When the chip is in  normal operation, the DC voltage through Rd and Ld  decrease to about 1V. The damage was observed in the film  resistor of attenuator, the blocking condenser and the  amplification field-effect tube at the output end inside the  device. The relationship among the three damages was  analyzed as follows.

•    If the damage only happens to the attenuator inside  the device, the failure mode will be as follows. The  equivalent resistances R1, R2, R3 to the ground and  the output were increased, which would not damage  the prime blocking condenser and field-effect tube.     •    If the breakdown only happens to the blocking  condenser, the voltage at point A will be 3.63 V after  simulation test; at the same time, the current through  the resistance R2 is   $15~\mathrm{mA}$  , which is not enough to  burn the film resistor of the attenuator. A 4V of  voltage was directly applied to the sample end of the  2dB fixed attenuator. The conduction time was 24  hours and the fixed attenuator was intact.    •    If the breakdown only happens to the grid of the  amplification field-effect tube and causes the fieldeffect tube to fail, a low resistance channel will be  formed between the power supply Vd and the  ground, causing the device to fail. However, the  breakdown cannot disable the capacitance and the  attenuator at the output end.

Therefore, the possibility can be ruled out that a failure of  one point inside a device can cause failures of another two  points. Then, it was estimated that the failure of the module  should be caused by one-time damage to all three internal  components.

Secondly, the module to be analyzed accepted the aging  test at the screening stage and the conditions were   $\mathrm{TA}=85\,+$     $3\,^{\circ}\mathrm{C}$  , 360h,   $\mathrm{V_{D}}=+5\mathrm{V}$  ,   $\mathrm{V_{G}}=\mathrm{-}5\mathrm{V},$  , Vs1, Vs2, Vs3, Vs4, Vs5,   $\mathrm{Vs}6=+5\mathrm{V}$  ,   $\mathrm{f_{LO}}=\,16\mathrm{GHz}$  ,   $\mathrm{P_{LO}}=\mathrm{-4dBm}$  . The aging electric  stress completely covered the service stress. Therefore, the  possibility of failure due to the chip defect inside the module  is small. Particularly, it is impossible to have a failure caused  by the simultaneous defect of all three internal components.

Finally, the blocking condenser and the field-effect tube  are located at the position where the amplifier channel at the  final level relates to the output end. The channel adopts the  same power supply and ground signal as the prior level of  amplifier channel. Given the damaged attenuator inside the  module, there were no abnormalities in the prior level of  attenuator and amplifier chip. Thus, it was estimated that the  electrical stress causing the module to fail should come from  the output port of the device. There are two kinds of  abnormal electrical stress damage at the output port. One is  the module damage caused by the over-current stress at the  input port and the other is the module failure caused by  electrostatic discharge. Two kinds of damages were analyzed  as follows.

A.    The module damage is caused by over-current stress at  input port.

The module was monitored throughout the whole  operation process. The input signal of the module was output  by signal processing and control distributor module and then  connected by high-frequency cable. At the same time, the  output waveform of signal processing and control distributor  upon energizing was monitored. The results showed that no  over-current stress was detected as shown in figure 5 and 6.

![Cu/=Pw 1E  oR  IRMLSSE  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c9227c96-553d-40ba-a777-f050877bea05/c9227c96-553d-40ba-a777-f050877bea05.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=bf56a237a489db6b39f9bc0c5e9e6c7690c0a5e6)
Figure 5.    Output Waveform of Distributor upon Energizing

![|+  HHH  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5fc3eb10-e146-4275-aa25-34431cab62d8/5fc3eb10-e146-4275-aa25-34431cab62d8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=64a74cb0c68879fe66a7c065eeb0c752c7c63640)
Figure 6.    Output Waveform during Normal Operation

## B.    Module Damage Caused by Electrostatic Discharge  

During the joint test of the failure module, it was only  connected to the distributor through high-frequency cable.  The abnormal electrical stress comes from the input port.  Therefore, the most possible reason is that the highfrequency cable with static electricity damaged the attenuator  during plugging in/out process.

## IV.    M ECHANISM  A NALYSIS 

ESD failure can be divided into the sudden complete  failure and the potential delayed failure.  [4-5]

## A.    Sudden Failure  

It refers to the sudden deterioration of device parameters  and parameter drift. It is usually manifested as open circuit,  short circuit and even complete failure, such as metal strip  fusing, dielectric layer breakdown and other malfunctions.  For the microwave component, many of the chips adopted  here are electrostatic sensitive components. Under the  transient abnormal voltage stress of electrostatic discharge,  the internal components will be melted and burnt, which falls  into the sudden failure category.

## B.    Potential Delayed Failure  

If the electrostatic potential or the stored energy of the  charged body is relatively low, or if there is a currentlimiting resistance in the ESD loop, once of ESD is not  enough to bring about a sudden failure to the device.  However, it will cause potential damage inside the device,  continuously degrade its performance in service and  eventually lead to parameter drift or malfunction of the  device.

The parts vulnerable to electrostatic impact are mainly  input loop, output loop, the edges of concentrated electric  fields and weak parts in the structure. The damages are  featured by randomness, latency and complexity. [6]

•    the randomness refers to the possibility of  electrostatic failure during production, transportation  and application.    •    the latency refers to the fact that some components  do not demonstrate an obviously decrease of  function after being damaged by static electricity.  However, their functions will be degraded with the  increase of subsequent operating stress.    •    The complexity refers to the fact that it is difficult to  tell some electrostatic damages from the damage  caused by other reasons, which conceals the real  cause of failure.

Unpacked chip, film resistors and other ESDS-sensitive  components are widely adopted in microwave modules, such  as microwave low-noise amplifier chips, power amplifier  chips and digital circuit control chips, etc. Therefore, they  are extremely vulnerable to electrostatic damage. [7]

The internal circuit of the failure module is as follows.

![RT  R1  R2  R2 Amplifier Amplifiei  in  in  out  out R3 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4240a1e8-5637-481c-b7f9-4a9998e0daf2/4240a1e8-5637-481c-b7f9-4a9998e0daf2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=6d217ba637faec0f25fe0a33331f814f427bc143)
Figure 7.    Schematic Diagram of Internal Circuit in Failure Module

The DC voltage was applied to the chip’s input end; the  voltage value was changed before R9 or R11 was burnt. The  test verified that when the voltage was greater than 19V (the  current was greater than 56mA), R11 was burnt; when the  voltage was 15V (the current was greater than   $45\mathrm{mA}$  ), the  chip showed no sign of burn after 10 min of conduction time.

During the whole process, the static-induced electrical  stress could only be introduced immediately when the cable  was connected to the failure module. Next, there will be a  verification test to determine if the failure of the microwave  module is caused by the electrostatic discharge model.

## C.    Verification Test  

The sample same with the failure module was selected  and the electrostatic discharge simulation test was carried out  between the sample’s output end and the ground. At first, the  microwave module simulation test on anthropometric  dummy was carried out. The module function did not fail at  3000V of voltage but failed at 4000V and 6000V. Therefore,  due to the anti-static capacity of the module is greater than  3000V and that will rule out the possible damage caused by  human static electricity.

Then, a simulation test was carried out on the machine  model. After 200V of discharge to the machine model, the  module sample was test electrically and the signal at the  output end was 2.6V. The sample’s internal structure was  under examination and the film resistor of the attenuator at  the output end of the module was damaged, the breakdown  point was on the blocking condenser and the field-effect tube  grid was burnt. The damage morphology is shown in photos  8, 9 and 10.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1312cb07-42dd-4353-bd11-9e66f4f84950/1312cb07-42dd-4353-bd11-9e66f4f84950.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=096a8bba2632a8350e16b1bf1cfbb5fbd3cc85e8)
Figure 8.    Burnt Morphology of Attenuator at Output End of Module

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9427cad5-11d7-45c5-a485-b78d69b000d1/9427cad5-11d7-45c5-a485-b78d69b000d1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=99e713905d7a7ed0c59d1f39d7aebdc1b8f7ac73)
Figure 9.    Burnt Morphology of Blocking Condenser at Output End of  Module

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/480da1d7-f810-4bdf-bd19-44cc8cf761d6/480da1d7-f810-4bdf-bd19-44cc8cf761d6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=5d49da6457a6d9a20cb36aa7c78f2b4049a0a1f3)
Figure 10.    Burned Morphology of Upper Field-Effect Tube of Amplifier  Chip

The verification test shows the electrical test results of  the sample and its internal damage morphology are  consistent with the failure module, indicating that the  electrostatic stress of the machine model from output end can  cause similar failure. That is to say, the electrostatic  discharge causes the burn inside the module and the failure  of the module.

It can be seen from the analysis on schematic diagram of  the microwave module that there is no discharge circuit for  abnormal electrical stress inside the failure module.  Subsequently, the microwave module was improved. The  improved schematic diagram is as follows.

![RI  R1  R2  R2 Amplifier Amplifier  in  out out  L R3 R3  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/23432a0a-1afb-4ceb-86c5-5b656c43dce1/23432a0a-1afb-4ceb-86c5-5b656c43dce1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=2d5b55f88ebb1c27f6069db8d53bdfb172b42891)
Figure 11.    Schematic Diagram Morphology of Improved Module

A discharge circuit was added to the improved schematic  diagram. That helps a lot to improve the anti-static capacity  of the microwave device. The electrostatic discharge stress  was applied to the improved microwave device through  machine model and it was found that the anti-static capacity  of the device was promoted from 200V to   $400\mathrm{V}$  , a double  improvement.

## V.    C ONCLUSION 

Through the above analysis and the test results verified  that the module failure is caused by the burn of 3 internal  components due to the abnormal voltage stress from output  port of the operating module. The fundamental reason for  such failure lies in the electrostatic discharge. The  electrostatic discharge is an abnormal voltage stress with  high energy. During the module application, the factors that  may cause electrostatic discharge include the equipment’s  live plugging in/out, the cable-induced voltage, the failed  normal connection between equipment and ground, the  oscilloscope probe-induced high voltage, the high voltage  caused by the self-excited oscillation inside the circuit and  other   abnormal   voltage   stresses.   Active   and   strict  electrostatic protection measures shall be taken during the  application, assembly, debugging and other processes of  microwave modules so as to avoid the module damage and  especially the potential damage caused by static electricity.  In this way, can a sudden failure during the operation of the  whole machine be avoided.

During the verification test, the circuit inside the module  was improved and a discharge circuit was added. Thus, its  anti-static capacity has been greatly promoted, which is of  important   significance   for   the   subsequent   design  improvement in the microwave circuit.

## A CKNOWLEDGMENT 

First of all, I would like to extend my sincere gratitude to  my dear colleague, Mr. Chao Duan, for his instructive advice  and useful suggestions on this paper. I am deeply grateful of  her help in the completion of this paper.   High tribute shall be paid to Ms. Xiaoqing Wang, who have  helped me a lot in this failure analysis.

Last my thanks would go to my lovely family for their  great confidence in me. I also owe my sincere gratitude to  my friends who gave me help and time in listening to me and  helping work out my problems during the difficult point  during the failure analysis.

## R EFERENCES  

[1]    Yudong, Liu, Lei Du, Peng Sun, et, al. Effect of Electrostatic  Discharge on I-V and Low Noise Characteristics of Power Schottky  Diodes.[J]  Acta Physica Sinica, 2012,61(13): 137203-1-137203-8.    [2]    LIU Shanghe, WU Zhangcheng, ZHU Changqing, et al. ESP and  hazard protection[M].Beijing, China: Beijing University of Posts and  Telecommunications Press, 2004:36-37.    [3]    LIU Shanghe, WEI Guanghui, LIU Zhicheng, et al. Electrostatic  theory and protection[M]. Beijing, China: Weapons Industry Press,  1999:22-24.    [4]    Zhenyu Zhu. The harm of ESD to microwave module and its  protection.[A] Reliability and Environmental Test of Electronic  Products, 2013,31(3):19-24.    [5]    YANG Jie, LIU Shanghe, YUAN Qingyun, et al . Square-wave EMP  damage of microwave low-noise silicon transistors[J] High Voltage  Engineering, 2007, 33(7):111-114.    [6]    Baohua Shi, Xinzhang Jia, Desheng Zhang. Reliability of  Microelectronic Devices[M].Xi’an: Xidian University Press,1999.    [7]    EVELOY V, HWANG Y C, PECHT M G. The effect of electrostatic  discharge on electrical overstress susceptibility in a gallium arsenide  MESFET-based device[J].IEEE Transactions on Device and  Materials Reliability, 2007,7(1):200-208.

