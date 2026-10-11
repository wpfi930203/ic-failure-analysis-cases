---
title: "229_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_660982898377cdf9211056c8c7c99f237295230462135641
file_size: 331769
---

## Modeling IC Snapback Characteristics Using a VCCS  Model for Circuit-Level ESD Simulation  

Yunhao Li, Yize Wang, and Yuan Wang \*   Key Laboratory of Microelectronics Device and Circuits (MoE),  Institute of Microelectronics, Peking University, Beijing, 100871, China.   \*  Email:  wangyuan@pku.edu.cn

Abstract-   Snapback behaviors under electrostatic discharge (ESD)  stress are difficult to be simulated due to the limitation of SPICE  tools. This paper proposes a novel way to model avalanche effect  using a voltage-controlled current source (VCCS). This method  greatly simplifies the calculation of the avalanche multiplication  factor M and improving the convergence properties. This can  change the exponential relationship of the M into a linear  relationship of the gain of the VCCS. Meanwhile, this method can  be used for mixed simulation at the circuit-level and device-level  and model double snapbacks phenomenon appearing in power  clamp circuits. Measurement and simulation of the new approach  indicates that this approach is useful.

Keywords    –   Electrostatic   discharge   (ESD),   Avalanche  breakdown, VCCS, Double snapbacks .

## I. I NTRODUCTION 

As the feature size of integrated circuits scaling down,  designing circuits with higher reliability and robustness  becomes more important and challenging in advanced  processes. The scaling down of integrated circuits will reduce  the power supply of the transistor, increase the thickness of the  gate insulating layer, which will make the devices more  susceptible under ESD/EOS stress. That is the main reason for  the failure of the integrated circuits. Therefore, designing high  performance, simple structure, and versatile ESD protection  devices/circuits is particularly important. The main method of  ESD design, at present, is still the traditional method of “trialand-error”, which has some shortcomings such as high design  cost and long time-consuming. We need to develop better  SPICE simulation methods and models to characterize the  electrical characteristics of the ESD protection device/circuit,  and then predict the ESD protection capability accurately.  Another difficulty is that the device model in the standard  library cannot be applied to SPICE simulation of ESD behavior,  so customized models need to be applied to SPICE simulation.  The device-level ESD protection structure generally uses a  compact model such as MEXTRAM BJT model or VBIC BJT  model [1, 2]. For circuit-level ESD protection circuits, however,  only using circuit-level simulation does not yield accurate  simulation results sometimes [3]. The reason is that the big  MOS transistor has serious parasitic effects, which are certainly  not negligible under ESD stress. Hence, circuit- and devicelevel mixed simulation need to be used.

In this paper, a new approach to model snapback of MOS  ESD protection devices is presented and this compact model  can be used to model double snapbacks of power-rail ESD

clamp circuit which is simulated by mixed simulation method.    The simulation result is verified by the measured data.

## II.  AVALANCHE MODEL 

The MOS devices in the traditional standard process library  do not include the weak avalanche multiplicative effect, which  is the main reason for the snapback of the MOS transistors  under ESD stress. The fundamental way to model the weak  avalanche multiplicative effect is to use a simple BJT model, a  resistance and a current-controlled current source (CCCS) [4]- [6], or to use advanced standard BJT model that include weak  avalanche multiplicative effects, such as MEXTRAM model  [2][7][9]. The key factor of modeling accuracy of the weak  avalanche multiplicative effect is critical. In [4][6][8], using a  current-controlled current source to model the avalanche  multiplicative effect, the avalanche multiplication factor M can  be calculated as

$$\begin{array}{r}{M=\frac{1}{1-k_{1}e x p\left[-\frac{k_{2}}{V_{d}-V_{d s a t}}\right]},}\end{array}$$
where  k 1 ,  k 2  are fitting parameters related to the drain depletion  width and impact ionization coefficients, and   $V_{d s a t}$   is the MOS  saturation voltage. A drawback of the Eq. (1) is that it has the  relatively serious convergence problem. In the paper [4], the  discontinuity of M is overcome by a continuous function:

$$M=\exp[k_{1}(V_{d}-V_{s a t}-d_{1})]+\exp[k_{2}(V_{d}-V_{s a t}-d_{2})]$$
where   $k_{I},~d_{I},~k_{2},~d_{2},$  , are fitting parameters. The avalanche  multiplication factor in Eq. (2) includes two exponential terms.  The   first   exponential   term   indicates   the   avalanche  multiplication factor between the drain and substrate of the  MOS, and the other exponential term is the avalanche  multiplication factor of collector and base of the parasitic  bipolar transistor.

![CCCS   VCCS  Mbig.   Mbig  NPN   NPN  R  ap  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2cac4e0b-a0c3-427e-8d86-91b1f8448463/2cac4e0b-a0c3-427e-8d86-91b1f8448463.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215664%3B1743219264&q-key-time=1743215664%3B1743219264&q-header-list=host&q-url-param-list=&q-signature=718f422ce8be991045197bb171fe2883b9813cc7)
Fig. 1 Scheme for simulating MOS breakdown, (a) with CCCS and (b) with  VCCS.

![VCCSSRO R0 Mp Mbigibi  RC R0 Mp MbigA ANPNNPM Mn MnR1C0 C0Mf Mfap (a) b） (b)](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/289c73f6-9fd9-4119-8090-8eff74d91316/289c73f6-9fd9-4119-8090-8eff74d91316.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215664%3B1743219264&q-key-time=1743215664%3B1743219264&q-header-list=host&q-url-param-list=&q-signature=e949415fb37a5d8b0841bbd6df1d36d025da9c97)
Fig. 2 RC power clamp circuit, (a) circuit diagram (b) simulation diagram.

In this work, the proposed compact model used a VCCS  instead of CCCS as shown in Fig. 1. The avalanche  multiplication factor in this compact model only needs to  consider the gain of VCCS. Regardless of the influence of the  drain voltage, the avalanche multiplication factor only has one  necessary factor, the gain of the VCCS, to consider, which  greatly simplifies the compact model.

## III.  DOUBLE SNAPBACKS 

When the ESD event is applied to the VDD rail of the RC  power supply clamp circuit based on the feedback structure (as  shown in Fig. 2(a)), the voltage of node A still maintains low  potential due to the coupling effect of the capacitor C. The  output of the inverter is logic high, which changes the   $\mathbf{M}_{\mathrm{big}}$   to  on-state. Due to the retention of the feedback structure, the turnon time of the MOS is prolonged, which sufficiently discharges  of the large current [3]. Reasons for the two snapbacks are  different. The first snapback is caused by triggering of the  parasitic bipolar transistor, which needs to be implemented by  modeling the advanced model or customized model including  avalanche breakdown effect; and the second one is due to the  feedback structure of the circuit itself under the action of the RC  time constant. So the double snapbacks are device-level  snapback and circuit-level snapback, respectively.

We can use the following expression to get the gain of VCCS  in the double snapback model:

(3)

$$g=\left\{\begin{array}{c c}{{0}}&{{0<V<V_{1}}}\\ {{k_{2}\times(V-V_{1})}}&{{V_{1}\leq V\leq V_{2}}}\\ {{k_{1}\times(V-V_{1})+b_{1}}}&{{V_{2}\leq V\leq V_{3}}}\\ {{0}}&{{V>V_{4}}}\end{array}\right.$$
where  $k_{I},\,k_{2},\,b_{I}$   are fitting parameters and   $V_{I},\,V_{2},\,V_{3},\,V_{4}$   are the  charge voltages corresponding to V t1 , V h1 , V t2 , V h2  which are  the trigger voltages and holding voltages of first and second  snapbacks. In general,  $k_{I}$   is less than   $k_{2}$   which can be explained  by the following analysis: when the voltage value is between  the trigger voltage and the holding voltage, it is a decreasing  process. A larger gain factor is required to maintain the  corresponding avalanche multiplication factor, however when  the voltage value is beyond the holding voltage, the voltage is  an increasing process. Compared with the previous gain factor,  a small gain of VCCS can obtain corresponding equivalent  avalanche multiplication factor. The value of   $b_{I}$   is an offset  factor that can be determined by equalizing the two linear  functions in the point of holding voltage. The gain is zero when

the charge voltage is greater than   $\mathrm{V}_{\mathrm{h}2}$  . It is because the circuitlevel snapback occurs at this time, and the drain voltage drops  to a small value, which is much smaller than the avalanche  breakdown voltage of the parasitic bipolar transistor and dose  not maintain the on-state of parasitic bipolar transistor.

## IV.  SIMULATION AND VALIDATION 

The RC power clamp circuit is fabricated in a standard 65- nm CMOS process with 2.5-V thick-oxide devices. Table I  summarizes all the used device parameters in this work. It  should be noted that  $\mathbf{M}_{\mathrm{big}}$   is composed of 16 fingers with each   $80{\mathrm{-}}{\upmu\mathrm{m}}$   width of each one.

Table I – Device parameters for RC clamp circuit

|Devices|R 0 (kΩ)|C (fF)|M fb (µm/µm)|M p (µm/µm)|M n (µm/µm)|M big (µm/µm)|
|---|---|---|---|---|---|---|
|Parameters|30|300|0.5/0.5|8/0.5|4/0.5|1280/0.28|


![0.30 0.30   Measurment Measurment   Simulation Simulation  0.25  0.25 TLP Current (A) 0.15  0.20 0.15 Jno  0.10  0.10 0.05  0.05 0.00 0.00F  0.5 1.0 1.5 2.0 2.5 3.0 3.5 4.0 4.5 5.0 5.5 6.0 6.5 7.0 7.5  0.5 1.0 1.5 2.0 2.5 3.0 3.5 4.0 4.5 5.0 5.5 6.0 6.5 7.0 7.5 TLP Voltage (V)  TLP Voltage (V) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6ce52c13-285a-4c65-b669-76ddb4368cce/6ce52c13-285a-4c65-b669-76ddb4368cce.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215664%3B1743219264&q-key-time=1743215664%3B1743219264&q-header-list=host&q-url-param-list=&q-signature=f1c6cad7b2c402b95f38752e93b63a412fd08c45)
Fig. 3 Measured and simulated TLP I-V curve of double snapbacks about  transient power-rail ESD clamp circuit.

![25.0  25.0 22.5  22.5  Vcharge Vcharge  20.0  20.0   y1=4.8（x-6） y1=4.8 (x-6)   y2=3.4(x-6)+2.8 y2=3. 4 (x-6) +2. 8  17.5  17.5 gain (mMhos) 15.0  15.0 112.5  12.5 10.0 10.0  品7.5  7.5 5.0 2.5 2.号  0.0  0.0 -2.5 -2.5  5.05.5 6.0 6.5 7.0 7.5 8.0 8.5 9.0 9.5 10.0 10.5 11.0  5.0  5.5  6.0  6.5  7.0  7.5  8.0  8.5  9.0  9.5 10.0 10.5 11.0 Voltage (v)  Voltage (V) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/72c57227-a59c-4f5f-a88e-f0d325477862/72c57227-a59c-4f5f-a88e-f0d325477862.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215664%3B1743219264&q-key-time=1743215664%3B1743219264&q-header-list=host&q-url-param-list=&q-signature=47939649cf9d5dc9c7c1c89cd2b295eef0535776)
Fig. 4 The gain of VCCS as a function of charging voltage, and different gain  expressions in different voltage regions.

The simulation schematic diagram of RC power clamp circuit  to achieve double snapback can be seen from Fig. 2(b). Fig. 3 is  a comparison of the measured data and simulation data of the  RC power-rail ESD clamp circuit. We can find that the double  snapbacks can be simulated well by the hybrid simulation of the

circuit-level and the device-level, especially the first snapback  fit very well. The process from the first snapback to the second  snapback can be divided into two different states, they have  different gain expressions of the VCCS, the specific results are  shown in Fig. 4, the reasons for the difference between the two  linear curve slopes has been discussed above. In the second  snapback, the simulation of the holding voltage has the same  trend with the measured data but a little difference. The reason  may be that the influence of the parasitic resistance generated  in fabricating the big MOS transistor process is not considered.   The equivalent multiplication factors M, which come from the  product of the gain of VCCS and the  $\mathrm{V_{charge}}$  , has the same shape  as the exponential function shape (seen from Fig. 6).

![250 250  225  225   multiplication factor1 multiplicationfactorl   multiplication factor2 multiplicationfactor2  200  200  exponential function exponentialfunction  175 175  150  150 125 125  M 100 1. 00  75 50  50 25  25 0 -25 5.5 5，5   6.06.57.07.58.08.59.09.510.010.511.  6.0  6.5  7.0  7.5  8.0  8.5  9.0  9.5  10.0 10.5 11.0 Voltage(v)  Voltage (V) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e1c742cf-333d-43e1-9bbd-55dc08d85c9a/e1c742cf-333d-43e1-9bbd-55dc08d85c9a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215664%3B1743219264&q-key-time=1743215664%3B1743219264&q-header-list=host&q-url-param-list=&q-signature=432fd64c495b7bf12652862f9a68d55f94425266)
Fig. 5 The equivalent multiplication factors M, which come from the product  of the gain of VCCS and the  $\mathrm{V_{charge},}$  , and the multiplication factor of  exponential function.

## . C ONCLUSION   

[2]    Y. Zhou, J. Hajjar, A. W. Righter, and K. P. Lisiak, "Modeling snapback  of LVTSCR devices for ESD circuit simulation using advanced BJT and  MOS models," in  Proc. EOS/ESD Symp. ,  2007,  pp. 3A.3-1-3A.3-10.    [3]    G. Lu, Y. Wang and X. Zhang, "Double snapback phenomena in transient  power-rail ESD clamp circuits for latch-up free concerns,"  in Proc. IEEE  IPFA , 2015, pp. 275-278.    [4]    S. Lim, X. Zhang, Z. Yu, S. Beebe, and R. W. Dutton, "A computationally  stable quasi-empirical compact model for the simulation of MOS  breakdown in ESD-protection circuit design," in  Proc. IEEE SISPAD,  pp.  161-164, 1997.    [5]    X. F. Gao, J. J. Liou, J. Bernier, G. Croft, and A. Ortiz-Conde,  "Implementation of a comprehensive and robust MOSFET model in  cadence SPICE for ESD applications,"  IEEE Trans. Computer-Aided  Design , vol. 21, no. 12, pp. 1497-1502, Dec. 2002.    [6]    J. Li, H. Li, R. Barnes and E. Rosenbaum, "Comprehensive study of drain  breakdown in MOSFETs,"  IEEE Trans. Electron Devices , vol. 52, no. 6,  pp. 1180-1186, June 2005.    [7]    A. Ramanujan, M. Kadi, J. TrÉmenbert, F. Lafon, and B. Mazari,  "Modeling IC snapback characteristics under electrostatic discharge  Stress,"  IEEE Trans. Electromagn. Compat. , vol. 51, no. 4, pp. 901-908,  Nov. 2009.    [8]    A. Amerasekera, Mi-Chang Chang, C. Duvvury and S. Ramaswamy,  "Modeling MOS snapback and parasitic bipolar action for circuit-level  ESD and high-current simulations,"  IEEE Circuits and Devices Magazine ,  vol. 13, no. 2, pp. 7-10, Mar 1997.    [9]    J .  Cao, J. Xu, Y. Wang, G. Lu, and X. Zhang. “A compact SCR model  using advanced BJT models and standard SPICE elements,”  Science  China Information Sciences,  vol. 59:109302, 2016.

A new compact model approach for modeling ESD MOS  snapback and power-rail clamp circuit double snapbacks is  presented in this paper. The compact model uses VCCS instead  of CCCS to model the weak avalanche breakdown effect. The  advantage of this model is that it is no longer necessary to  consider the effect of the drain voltage on the avalanche  multiplication factor, but only consider the effect of the gain of  the VCCS, which can simplify the calculation of M and reduce  the fitting parameters to be considered. The model can also be  used in mixed simulation method and model double snapbacks  of power-rail ESD clamp circuit. By comparing with the  measured data, the model has a good SPICE simulation results.

## A CKNOWLEDGMENT 

This work was supported by National Natural Science  Foundation of China (Grant No. 61774005).

## R EFERENCES 

[1]    Y. Zhou, D. Connerney, R. Carroll, and T. Luk, "Modeling MOS  snapback for circuit-level ESD simulation using BSIM3 and VBIC  models," in  Proc. IEEE ISQED , 2005, pp. 476-481.

