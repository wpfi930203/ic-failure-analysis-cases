---
title: "251_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_3c6e06ebe84e0afb3f23cea3aff63ddb7295230462135641
file_size: 1089370
---

## Modeling and Simulation of Diode Triggered Silicon  Controlled Rectifier Behavior under ESD Stresses  

Meng Miao, You Li, and Robert Gauthier  Globalfoundries, Essex Junction, VT, 05452, USA.  Email:  meng.miao@globalfoundries.com

Abstract-   A Diode Triggered Silicon Controlled Rectifier (DTSCR)  is modeled. This DTSCR compact model is able to simulate the  DTSCR’s I-V characteristics with snapback. Overshoot related  parameters in this model also reproduces the overshoot  phenomenon in transient simulation. Simulation of non-linear  resistivity in the high current region is modeled based on the  electro-thermal behavior and velocity saturation. This model is not  only able to simulate quasi-static I-V under typical ESD stresses,  but can predict ESD failure with arbitrary input ESD waveforms.

Keywords  –  ESD, Modeling, Snapback, Thermal failure .

## I. I NTRODUCTION 

Electrostatic Discharge (ESD) is one of the major threats to  integrated circuit (IC) products and electronic devices. ESD  design involves evaluating the ESD robustness, as well as  establishing feasible ESD protection plans for various  applications. A generic ESD solution involves several types of  ESD devices, each having pros and cons, to handle different  ESD situations. ESD design methodology relied more on  hardware measurement than simulation for a reliable circuit  design must be eventually silicon validated. Due to the  difficulty of modeling device behavior under ESD stresses,  simulation methodology was barely used in ESD design.  However, in view of the evolving integration and complexity of  advance IC technologies, ESD simulation before IC fabrication  becomes an effective approach to validate the ESD robustness  of ICs and helps reduce design cost in tapout cycles.

Among typical ESD devices, Silicon Controlled Rectifier  (SCR) possesses the capability of conducting high ESD currents  which makes it a promising candidate for ESD protection.   High-trigger low-holding snapback characteristics challenge  the design to fit the ESD design window and introduce a nonmonotonic current versus voltage which may confuse the  simulator and cause convergence problems. On the other hand,  high current behavior is often modeled briefly as a single failure  current   It2  which ignores physical mechanisms within.  Improvements have been made, such as diode triggering and  base space tuning, to optimize SCR performance. Moreover,  new modeling techniques are introduced to implement  snapback behavior under ESD stress and to reveal the failure  mechanisms.

In this paper, a diode triggered SCR (DTSCR) structure is  modeled. Components of the DTSCR compact model are  introduced and simulation results are shown as well. The  DTSCR model not only can fit the quasi-static I-V with  measurement data but can reproduce overshoot behavior under

transient simulation which is valuable to evaluate turn-on  characteristic of DTSCR against fast Charged Device Model  (CDM) pulses. Incorporated a thermal network to model  electro-thermal behavior at high current region enables a model  applicable to arbitrary ESD waveforms.

## II.   M ODELING THE  DTSCR  

For a long period of time, snapback behavior or hysteresis  brings convergence issue to ESD simulation. It is very natural  to use an if-else statement to switch devices like SCRs between  pre-breakdown low current state and post- trigger high current  conducting. This on and off state switch, however, will create  discontinuities of derivatives around the negative resistance  region and may not be handled properly by today’s commercial  simulators (Spectre®, Hspice®, etc) based on Newton-Raphson  method.

Improvements have been made over time to work around  discontinuities. Some modeling methods rely on establishing a  sub-circuit of existing device models, like BJT and MOS, or  applying special simulator algorithm. But all models in the  circuit netlist will be eventually translated into analytical  equations by compiler and will be facing the same convergence  problem or using special build-in algorithm to get converged  solution.

It should be noted that ESD is always a transient event, rather  than a static I-V response. The conflict of multiple current  values versus single voltage input during snapback can be easily  solved by formulating monotonic I-V response in time domain.

![state 1NO on（1μA） Estate  THF off（OμA) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/41bb10ae-e976-42a4-98d3-f7b968552a8c/41bb10ae-e976-42a4-98d3-f7b968552a8c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215674%3B1743219274&q-key-time=1743215674%3B1743219274&q-header-list=host&q-url-param-list=&q-signature=3bd8ce2af9349b9d466274da40be2e4dcf2be015)
Fig. 1 Internal state delay model.

Circuit in Fig.1 provides a smooth transition of “off” to “on”  by introducing an internal state delay model [1].

$$\begin{array}{r}{I_{s t a t e}=\ 10^{-6}\cdot s t a t e\mathrm{~+~}\tau\ \frac{\partial s t a t e}{\partial t}}\end{array}$$
(1)

where the input control current   $I_{s t a t e}$   varies from 0 to 1  instantaneously, the voltage on a delay capacitor of   $\tau\,\upmu\mathrm{F}$   is not.  It varies gradually in time. The internal state delay model

mimics current generation as a result of impact ionization and  conductivity modulation which is time related.

By directly using an internal state variable to gradually  transform from “off” to “on” even a DC simulation can yield a  snapback I-V [2].

The on state current is extrapolated as a linear conducting  starting from holding point just after snapback.

$$I_{o n}(V)=\;I_{h}+G_{o n}\cdot(V-V_{h})$$
where   $V_{h}$   and   $I_{h}$   are the voltage and current values at holding  point,  $G_{o n}$   is the linear conductance characterizes the SCR’s onresistance. To smoothly transform from “off” to “on” and  properly represent the leakage before turn-on, off state current  is modeled as

$$\begin{array}{r}{I_{o f f}(V)=\,I_{S}\cdot e^{-\frac{V}{V_{T}}}\cdot\sqrt{1+\frac{\operatorname*{max}(V,0)}{V_{D}}}}\end{array}$$
where  $I_{s}$   is the reverse saturation current, the thermal voltage   $V T$   $\scriptstyle=K T/q$   is determined by Boltzman constant, ambient  temperature and charge of an electron,   $V_{D}$   marks the onset  voltage of conductivity modulation caused by impact  ionization.

Besides the hysteresis behavior at SCR’s trigger point, the  high current conducting and hard failure due to ESD stress must  be taken into account in ESD modeling and simulation, for the  circuit will be applied with stresses beyond its normal operation  region. Effects such as dielectric punch-through, self-heating  and velocity saturation cannot be neglected and show  significant impact on the high current characteristics.

The velocity saturation is often modeled as a mobility  reduction term that divides the conductance factor, or in a  reciprocal form to increase the on-resistance at high E-field  region by multiplying a factor of   $\mu_{r e d}$   [3].

stress regardless of the stress duration, self-heating will  continuously heat the device and increase the on-resistance  before the heating source is removed, namely pulse ends, or a  thermal equilibrium state is reached. The on-resistance  increment factor due to self-heating can be modeled as

$$R_{s h}(T)=\;R_{0}\cdot(1+T_{C1}\cdot\Delta T+T_{C2}\cdot\Delta T^{2})$$
where  $R_{\theta}$   is  the nominal value of the zero-bias resistance at the  nominal temperature   $T_{0},\varDelta T=T{\cdot}T_{0}$   represents the temperature  difference,  $T_{C l}$   and   $T_{C2}$   are the linear and quadratic temperature  coefficients.

The last effect related to ESD protection devices like SCR  and GGNMOS is thermal failure. A thermal network is used to  represent the thermal transmission during stress, as shown in  Fig.2. The  $C_{t h}$   is the thermal capacitance and  $R_{t h}$   is the reciprocal  of thermal conductivity. A Cauer ladder network with length   $\Nu{=}2$   is used in the paper to represent the silicon region in a SCR.  During ESD simulation, the voltage variation on  $C_{t h}$  , equivalent  to temperature variation, will rise as current flow through the  SCR. Although device failure temperature differs with  materials and device structures, the temperature rise during  ESD stresses can be always mapped into a 0 to failure  temperature   $(T_{f})$   scale with linear intervals [4]. Assuming the  temperature rise during ESD stress is from 0 to 1,000K, once  the thermal voltage on   $C_{t h I}$  , or hotspot temperature reaches a  critical value of   $T_{f}\!=1,\!000\mathrm{K}$   simulation will automatically stop  and feedback a failure message.

$$\begin{array}{r l r}&{}&{r_{\mu}^{v s}=\;r_{0}\cdot\mu_{r e d}=\;r_{0}\cdot[1+\sqrt{{\left(\frac{E-E_{c e}}{2E_{c r i t}}\right)}^{2}+\frac{d_{\mu}E_{c e}}{E_{c r i t}}}}\\ &{}&{+\sqrt{{\left(\frac{E+E_{c e}}{2E_{c r i t}}\right)}^{2}+\frac{d_{\mu}E_{c e}}{E_{c r i t}}}}\\ &{}&{-\sqrt{{\left(\frac{E_{c e}}{E_{c r i t}}\right)}^{2}+\frac{4d_{\mu}E_{c e}}{E_{c r i t}}}\;]}\end{array}$$
where

$$E_{c e}=\sqrt{E_{c o r n}{}^{2}+(2d_{\mu}E_{c r i t})^{2}}-2d_{\mu}E_{c r i t}$$
![Thermal Network  500  Rth1   Ru2  Anode   -eh1   Cuh2  Nonlineari  Resistor  Model  SCR  SEI   Nwelll  Pwell  Psub  Model  Cathode  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/69fb7c8b-1af0-40fd-9b66-90b2aaa8f2f8/69fb7c8b-1af0-40fd-9b66-90b2aaa8f2f8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215674%3B1743219274&q-key-time=1743215674%3B1743219274&q-header-list=host&q-url-param-list=&q-signature=cccfab6bee454501c0d5ef1b59f1fce738eba3a1)
Fig. 2 Model simulation circuit and a thermal network incorporated.

The   $\mu_{r e d}$   has a value of 1 when   $E=V/d=0$   and approaches   $I+(E{-}E_{c o r n})/E_{c r i t}$   for large E-field.  $d_{\mu}$   controls the “hardness” of  transition region around   $E\,=\,E_{c o r n}$   where velocity saturation  induced resistance increment becomes significant.

Another major effect for ESD devices at high current region  is the self-heating. Different from velocity saturation which  returns a fixed on-resistance increment for a certain voltage

The full-frame of DTSCR model consists of a snapback  model and a non-linear resistor model. The snapback model  simulates the behaviors of off state leakage current, SCR  triggering with negative resistivity and on state conducting after  holding point. In series with the non-linear resistor model the  resistance increment due to velocity saturation and self-heating  are included in simulation. There is a thermal network  embedded in the non-linear resistor model which captures the  overall transient I-V input to calculate temperature variation and  feedback   $T_{f}$  as the failure criterion. The trigger voltage is

parameterized with the number of trigger diodes as each diode  provides 0.8V extra trigger voltage. Although the  It2  value is  used to evaluate the current capability of ESD device and is a  straightforward failure criterion implemented in most compact  ESD models for quick simulation and validation, it has its own  drawback that a single device needs a set of  It2  values according  to different ESD stress models (HBM, MM, CDM, etc).  Standard ESD stresses may be changed by the loading circuit,  forming arbitrary input waveforms for the model which does  not apply to any pre-defined  It2  values. Instead, failure  temperature is the intrinsic cause for failure and applies to  different ESD conditions [5-6]. The length of thermal network  is determined by the trade-off between accuracy and model  complexity, as well as pulse widths available in the  Transmission Line Pulser (TLP) tester.

## III. S IMULATION  R ESULTS 

Fig.3 shows the simulation of a DTSCR with snapback and  high current I-V curve bending. The resistance increment due  to self-heating varies with different TLP stress pulse widths,  DTSCR I-V at high current region shows different bending  trend accordingly. It is verified and explained by monitoring  end of the pulse temperature rise on   $C_{t h I}$   as shown in Fig.3(b),  longer self-heating period TLP pulse (100ns) reaches   $T_{f}$  with  lower power level than vfTLP pulses (2ns-10ns).

![Quasi-Statice Current vs.Voltage Plot   1Current vs.Max Temperature during pulse  S.S   2ns vfTLPMea.(o）and Sim.()   5.5  MaxTe   der2nspulse  5.0  5ns vfTLP Mea.(o）and Sim.(-)   50   under l0ns  Ons vfTLP Mea.(o)and Sim   MaxTempunder100nspulse  45  100nsTLPMea.(o)andSim.()  40   40  35   3.5  3.0   23.0  52.S   52.5  32.0   20  T.S  1.0   10  0S  00  0S  30   S.0   20   11.S   0.00.20.40.60.81.01.1  Voltage(V)   Temperature Rise (k)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0aca5cc4-9a54-4a56-b0b4-b57f386315da/0aca5cc4-9a54-4a56-b0b4-b57f386315da.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215674%3B1743219274&q-key-time=1743215674%3B1743219274&q-header-list=host&q-url-param-list=&q-signature=bd0190fa40398ae286ebe4778aecb12083c43b6d)
Fig. 3 Simulated and measured I-V of DTSCR under 2ns\~100ns pulse widths  TLP (a), and temperature rise on  $C_{t h I}$   (b).

One essential concern about ESD design is the transient turnon characteristics of ESD devices. When designing ESD for fast  pulse stress such as CDM or first peak of system level IEC  stress, overshoot voltages may damage the inner circuit prior to  protection fully turns on to discharge the majority of ESD  energy. Modeling transient turn-on behavior of ESD devices is  a vital part of ESD evaluation. The simulation in Fig.4 picks  three points on a 2ns vfTLP I-V after DTSCR snapback and  generates voltage vs. time waveforms. Compared with the  overshoot peaks captured by measurement, the transient  simulation matches well with measured waveforms and  revealed a  ${\sim}11\,\mathrm{V}$   maximum overshoot voltage peak which is not  visible in quasi-static I-V plot. It is also notable that at a high  current of 4.3A, self-heating will be so drastic that even during

a 2ns short period the on-resistance increment can be observed  as the voltage rises till the pulse-end.

![Transient Response   Sun Jan 20 21:34:30  12.0  V(t)waveform @4.3AMea.（o)V(t)waveform@4.3ASim.()  V(t)waveform @3.5A Mea.(o)V(t)waveform @3.5AMea.(-)  10.5  V(t)waveform @2.7A Mea.(o)V(t)waveform @2.7A Mea.()  9.5  8.5  7.5  6.5  5.5  4.5  3.5  2.5  1.5  0.5  0.5  5.2   5.4   5.6  5.8  6.0   6.2  6.4  6.6   6.8   7.0  7.2  7.47.6  time (ns)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a0ed6486-d525-48dd-ab79-706d0fadb271/a0ed6486-d525-48dd-ab79-706d0fadb271.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215674%3B1743219274&q-key-time=1743215674%3B1743219274&q-header-list=host&q-url-param-list=&q-signature=7382e236346c319faf7d892fe0baaa29a5e79cd2)
Fig. 4 Transient voltage waveform measured and simulated at three different  current levels after DTSCR turns on.

As DTSCR trigger voltage is tunable by adjusting the trigger  diodes, the DTSCR compact model has parameterized the  trigger voltage with the number of diodes in diode string.  As  shown in Fig.5, with an intrinsic diode inside SCR, the trigger  diode string can tune DTSCR turn-on voltage by a 0.8V interval  for each diode in series. Also, by putting current in a logarithmic  scale, it is clearly shown that it requires certain amount of  current injection to trigger the positive feedback loop of NPN  and PNP bipolar inside SCR. The DTSCR trigger voltage is  actually the voltage value where the diode string injected  enough current into SCR’s base region to strongly forward bias  both bipolars.

![101  2 Trigger Diode Mea.(o)   2TriggerDiodeSim.(-)  Trigger Diode Mea. (o)   DiodeSim.  4TriggerDiodeMea.(o)   4Trigger DiodeSim.(-)  100  ≤10-1  1O  1O  0.0   0.5   1.0   1.5   2.0   2.5   3.0  3.5   4.0   45   5.0   5.5   6.0   6.5  Voltage(V)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0cfdc1de-79c0-4a90-a701-d2b793cb5538/0cfdc1de-79c0-4a90-a701-d2b793cb5538.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215674%3B1743219274&q-key-time=1743215674%3B1743219274&q-header-list=host&q-url-param-list=&q-signature=2fdb5e8542d260a55562594b8c598d20aa5e4048)
Fig. 5 Trigger voltage parameterized according to different number of trigger  diodes.

As aforementioned advantage, using temperature instead of  current as failure criterion gives the model the ability to predict  ESD failure with arbitrary input ESD waveforms. Fig. 6 and  Fig.7 plot the simulated transient I-V response of the DTSCR  under 2kV HBM and 250V CDM stresses. During the rise time  of the HBM pulse, the DTSCR triggers and clamps the voltage  low at 1.6V. The clamping voltage reaches its peak value  (23.5ns, 3.01V) slightly behind the peak current (17.5ns,

1.32A). It is because on-resistance is still increasing due to selfheating after the current starts decaying. This assumption is  supported by plotting in-device temperature variations on   $C_{t h I}$  and   $C_{t h2}$   in the same figure. The temperature on   $C_{t h I}$   keeps  climbing up even after HBM’s peak until the dissipation of heat  is larger than the generation. As the heat sink of Cth1, the  temperature on   $C_{t h2}$   is always one step slower and lower than  the hotspot   $C_{t h I}$  . As HBM current decays to the DTSCR’s  holding voltage, simulation I-V starts to oscillate. Similar  conclusions can be drawn from the CDM simulation in Fig.7.  But as the response of a short ESD stress with fast rise time, an  obvious overshoot voltage peak can be seen as the CDM pulse  rises up. Compared to long duration HBM pulse, the   $C_{t h I}$  reaches its peak temperature while   $C_{t h2}$   is still relatively cold.  This is physically reasonable that heating by short CDM pulse  is more like an adiabatic process. It is noted that the reverse  direction of CDM pulse swing is clipped because the model  only models the DTSCR forward turn-on and snapback. The  reverse conducting is not correctly modeled yet.

![HBMTransientResponse   Mon Apr 29 16:47:50  6.5   1.5   480.0  17.5ns 1.32A  lamping Voltage  1.4   614   52.2ns448K  6.0   iseon C_th1  iseon C th2   440.0  Clamping Current   E  5.s  400.0  12  5.0  360.0  57.3ns337K  4.5  10   320.0  4O  280.0  0.8  240.0  3.0  200.0  0.6  25  160.0  20  0.4  120.0  1.5  80.0  10  0.2  O   40.0  0.0   三0.0  [mnpmmmmpmmmmpmmmmmmmpmmmnpmmmmmqrmmmmpmmmmmnmmm  0.0   70.0   140.0   210.0   280.0   350.0  time(ns)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b6284dbc-4224-43af-8c08-5ecabf69eaa4/b6284dbc-4224-43af-8c08-5ecabf69eaa4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215674%3B1743219274&q-key-time=1743215674%3B1743219274&q-header-list=host&q-url-param-list=&q-signature=c566639dbd4e0395e612810de96acdff6205ed67)
Fig. 6 Simulated transient I-V response and in-device temperature variation  under a 2kV HBM stress.

![CDMTransientResponse   TueApr3013:26:2620191  12.0   7.0   480.0  lamping Voltage  183ps10.2V  riseonC_th1  440.0  10.8   6.3   Trise on C_th2  Clamping Current  573ps6.1A   400.0  9.6   5.6  1.23ns4   360.0  8.4   49   692ps7.59V  320.0  MN.N   280.0  3.5   240.0  48   22.8   200.0  160.0  3.6   2-1  120.0  24   14  80.0  12  40.0  0.0   0.0   0.0  0.0   0.3   0.6   0.9   1.2   1.5   1.8   2.1   2.4   2√   3.0  time（ns)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1da03e94-44c9-47a7-8249-f2586a691e3c/1da03e94-44c9-47a7-8249-f2586a691e3c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215674%3B1743219274&q-key-time=1743215674%3B1743219274&q-header-list=host&q-url-param-list=&q-signature=92a658647731febf39a68c28ed6350fcaca1e600)
Fig. 7 Simulated transient I-V response and in-device temperature variation  under a 250V CDM stress

## IV. C ONCLUSION 

A compact model of DTSCR is established. The combination  of snapback model and non-linear resistor model, complicated  physical mechanisms can be represented through device  behavioral models. This model is physically based on the  intrinsic cause of device failure and covers basic aspects of  DTSCR operation under ESD stresses, such as high current I-V  bending, overshoot voltage tunable trigger voltage. The new  ESD compact model is capable of evaluating DTSCR behavior  under arbitrary input waveforms.

## R EFERENCES 

[1]    R. Ida and C. C. McAndrew, "A physically-based behavioral snapback  model,"  Electrical Overstress / Electrostatic Discharge Symposium  Proceedings 2012 , Tucson, AZ, 2012, pp. 1-5.    [2]    T. Wang and C. C. McAndrew, "A Generic Formalism to Model ESD  Snapback for Robust Circuit Simulation,"  2018 40th Electrical  Overstress/Electrostatic Discharge Symposium (EOS/ESD) , Reno, NV,  2018, pp. 1-8.    [3]    C. Mc Andrew, “R3, an Accurate JFET and 3-Terminal Diffused Resistor  Model,”  Proc. Workshop on Compact Modeling,  Nanotech 2004.    [4]    H. Li, M. Miao, Y. Zhou, J. A. Salcedo, J. Hajjar and K. B. Sundaram,  "Modeling and Simulation of Comprehensive Diode Behavior Under  Electrostatic Discharge Stresses," in  IEEE Transactions on Device and  Materials Reliability , vol. 19, no. 1, pp. 90-96, March 2019.    [5]    Y. Zhou, M. Miao, J. A. Salcedo, J. Hajjar and J. J. Liou, "Compact  Thermal Failure Model for Devices Subject to Electrostatic Discharge  Stresses," in  IEEE Transactions on Electron Devices , vol. 62, no. 12, pp.  4128-4134, Dec. 2015.    [6]    M. Miao, Y. Zhou, J. A. Salcedo, J. Hajjar and J. J. Liou, "A New Method  to Estimate Failure Temperatures of Semiconductor Devices Under  Electrostatic Discharge Stresses," in  IEEE Electron Device Letters , vol.  37, no. 11, pp. 1477-1480, Nov. 2016.

