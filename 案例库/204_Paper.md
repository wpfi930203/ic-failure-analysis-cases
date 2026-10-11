---
title: "204_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_9a90b2e63f0902dcdf7590144db6ef2f7295230462135641
file_size: 465821
---

## Capacitor Modeling Methodology for System-level  ESD Simulation  

Li Xiang \* ,   Xie Xiaofei, Xia Nan, and Gu Zhengdong    Huawei Technologies Co., LTD. Simulation lab; No. 2222, Xinjinqiao Road, Pudong Shanghai, P.R. China.  \* Phone: +86 17521260094 Email: lixiang128@huawei.com

Abstract-   To enhance the accuracy of  system-level ESD  simulation, single components on the printed circuit board (PCB)   are required to be precisely modeled. A new method of capacitor  modeling is presented. The model has been evaluated in different  simulation software and verified in several ceramic capacitors. A  comparison of measurements and simulation results have been  carried out and the simulation accuracy of peak voltage is high.

Keywords  –  System-level, Ceramic capacitor, Simulation,  Model, S-parameter.

## I. I NTRODUCTION 

Electrostatic discharge (ESD) protection has been one of the  most crucial issues for the robustness of terminal equipment.  Soft failures caused by ESD events are hard for trouble  shooting because of their randomness and complexity within  diverse application scenarios. In order to predict the risk points  of ESD failure in the design phase of terminal equipment and  help analyze the soft failure, electrical simulations based on  ESD models are widely used [1]. Actually, the behavior of  components under transient high voltage is related to many  factors: temperature, package parameter, etc. However, if all  factors are taken into account, the model will be too  complicated and the accuracy will not be greatly improved  when performing field-path co-simulation.

This paper aims to present a new approach to capacitance  modeling that ensures high accuracy and simplicity of the  capacitor at system level ESD events. It has been validated  using several ceramic capacitors (33pF, 1nF, 10nF, 2.2uF,  10uF). In the test of electrostatic gun (IEC 61000-4-2), the  correlation between peak voltage measured by oscilloscope  and simulation result is good.

## II. SMALL SIGNAL MODEL OF CAPACITOR  

In general, the small signal model of capacitor can be  represented by a RLC series circuit [2] as shown in Fig.1.

![R leakage  ESE  ESR    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8b51fcd2-fe40-404a-b3b0-d7bf57e84516/8b51fcd2-fe40-404a-b3b0-d7bf57e84516.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=116b7ac789778373faa35146fa411cf7524f827f)
Fig. 1 Small signal model of capacitor.

R ESR  stands for equivalent series resistance. Capacitors can be  represented by a resistor and a capacitor in series because of the

resistance of the manufacturing material and the loss of the  insulating medium.

Similar to   $R_{E S R},L_{E S L}$   is used to describe the inductive part of  the impedance of a capacitor while all physical devices are  connected to a circuit through conductive leads, which contain  inherent inductance.

The capacitor dielectric cannot be absolutely non-conductive,  so the capacitor exhibits leakage characteristics under transient  high voltage and  R leakage   is used to indicate this phenomenon.

The values of the components in the equivalent circuit of  Fig.1 can be obtained by analyzing the S parameters of the  capacitor measured by a VNA (Vector Network Analyzer).

Fig.2 depicts the impedance-frequency characteristics of a  certain capacitor.

![|Z|=wL  ESR  Frequency (Hz)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f8bd72d1-c428-4a8f-b9b3-080ddda68b27/f8bd72d1-c428-4a8f-b9b3-080ddda68b27.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=bdacb0508eb098a3576d0576a35719f90d3c08f1)
Fig. 2 |Z|-frequency characteristics of a 10uF capacitor.

![Simulation  Measurement  aP)  TTS  Frequency (MHz)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e2109d62-2010-40fb-b25c-544520fa4fd5/e2109d62-2010-40fb-b25c-544520fa4fd5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=2749f92673c28eaf0cafd9c5ddc9c71b18748e82)
The impedance of the capacitor is related to the frequency [3].  Capacitor exhibits capacitive characteristic at a low frequency,  and the equivalent impedance decreases as the frequency  increases, as shown by the red line in Fig.2. When the frequency  increase to the resonant frequency,   $|Z|$   is equal to ESR. After  that, the component will transform into inductive characteristic  and the impedance will be proportional to frequency, as  indicated by the green line in Fig.2. The value of L is given by  equation (1).

$$\mathrm{Z}=R_{E S R}+\mathrm{j}\omega\mathrm{L}$$+ jωL
(1)

After calculating the values of   $R_{E S R}$   and   $L_{E S L}$  , the S  parameters of the equivalent circuit can be simulated and  compared with that measured by a VNA. The values of   $R_{E S R}$  and L ESL  are fine-tuned so that the two curves can basically  fitted. Fig.3 depicts a comparison between simulated and  measured S parameters of a 10uF ceramic capacitor.

## III. C-V   CHARACTERISTICS   UNDER   TRANSIENT   HIGH VOLTAGE   

Ceramic capacitors with high induction ratios generally use  barium titanate   $({\mathrm{BaTiO}}_{3})$  ) as the main material of the dielectric  [4]. Under normal conditions, the spontaneous polarization of   $\mathrm{BaTiO}_{3}$   is in a randomly oriented state, but when a voltage is  applied from the outside, since the spontaneous polarization in  the dielectric is bound by the direction of the electric field, the  phase transition is less likely to occur. As a result, the  electrostatic capacity of the capacitor is lower than before the  bias is applied. Fig.4 shows the C-V curve of a 10uF ceramic  capacitor.

![/  DCBias(V  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/090c2d3d-b08f-41e1-855b-295298ec858e/090c2d3d-b08f-41e1-855b-295298ec858e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=faeee8a4a0764cad11570d4f31952ff5c2a12aa4)
Fig. 4 DC C-V curve of a 10uF capacitor.

According to [5], for the same capacitor, the DC bias voltage  and the transient high voltage have different effects on the  variation of the capacitance value. Transmission-line pulse  (TLP) can be used to test the values of a capacitor under  different transient high voltages.

![Voltage   Current  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ad4454b1-8b59-40c4-aa00-9f2ec2e57902/ad4454b1-8b59-40c4-aa00-9f2ec2e57902.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=d5a4bc91aca3b6ccd098e8dc678f135df7a36906)
Fig. 5 TLP results of a capacitor in certain pulse voltage.

During testing, the TLP system applies a series of test pulses  of varying amplitude to the capacitor. Each pulse corresponds  to a set of voltage and current data. Fig.5 shows an example.

According to the definition of capacitor, the charge stored in  the capacitor is the integral of the current flowing through it:

$$\textstyle Q=\int I d t$$
Record all the values of Q and   $\mathrm{V}$   and plot them on a single  graph. For nonlinear capacitors, the relationship between  capacitance and charge can be expressed as (3).

$$\complement={\frac{d Q}{d V}}$$
The calculated capacitance-voltage curve can be fitted by the  formula proposed by Johnson in [6]:

$$\frac{\epsilon^{\prime}}{\epsilon_{0}}\approx{[1+\alpha\epsilon_{0}^{3}E^{2}]}^{-\frac{1}{3}}$$
(4)

Where   $\epsilon^{\prime}$   is the incremental permittivity,   $\epsilon_{0}$   is the  permittivity without applied electric field and when the  capacitance C is directly proportional to  ϵ , formula (4) can be  re-expressed as:

$${\mathsf{C}}=C_{0}(1+a V^{b})^{c}$$
(5)

Where V is the applied voltage, C is the capacitance at bias  point,   $C_{0}$   equals to the capacitance at 0V and a, b, c are all  constants.

However, after modeling with the capacitance values under  DC bias voltage and transient high voltage respectively, it is  found that there is no obvious difference between the two for  system-level simulation. Considering that the former data is  easier to access, it can be directly used for modeling. This  phenomenon is due to the high voltage applied to the capacitor  in the system-level test. At several hundred volts, the  capacitance values measured by the two test methods is  basically the same. Fig.5 depicts the DC C-V curve fitted using  equation (5).

![measurement  fitcurve  Voltage  fit curve-residuals  Voltage  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f2cc0728-efe7-4747-b125-0481cd0c7eea/f2cc0728-efe7-4747-b125-0481cd0c7eea.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=cc97fd9f8a63342cc8d208d0f940703ad2eccd48)
Fig. 5 DC C-V curve of a 10uF capacitor.

## IV.   COMPARISON   OF   MEASUREMENT   AND   SIMULATION   RESULTS   

In order to verify the accuracy of the above modeling method  in system level simulation, a test system as shown in Fig. 6 is  constructed.

![Coaxial cable  Oscilloscope  TESTBOARD  GND  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/500c7517-c8ee-47df-84be-e42fe1662886/500c7517-c8ee-47df-84be-e42fe1662886.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=e8cbd1aa60be7aabaface758153b424c408cb436)
Fig. 6 Setup using an E-Gun as generator.

In the simulation, the models of the coaxial cable and the test  board are S-parameter models measured by a VNA (Vector  Network Analyzer). The capacitor model is built in PSpice  taking into consideration all these factors presented above.  Fig.7 describes the simulation and measurement of two ceramic  capacitors at different test voltages.

![t(ns)  （ms) t(ns)  t ns) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/59489f57-08ae-4274-9261-ed98c1f6ceca/59489f57-08ae-4274-9261-ed98c1f6ceca.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=5ffc2deb0b934ba378a686b40c748a3de715a680)
Fig. 7 Comparison of measurement and simulation results (a) 10uF ceramic  capacitor under 1kV and 8kV test voltage (b) 10nF ceramic capacitor under  1kV and 2kV test voltage.

The results in figure 7 (b) show that the peak voltages  measured at the oscilloscope do not change linearly when 1kV  and 2kV test voltages are applied to 10nF capacitors  respectively (12.8v at 1kV test voltage, 41.2v at 2kV test  voltage), which also illustrates that it is reasonable to use the CV characteristic curve for capacitance modeling.

Several other capacitors are verified by the same testing  method (33pF, 1nF, 10nF, 2.2uF, 10uF), and all show good  correlation between simulation and test results.

## V. C ONCLUSION 

System-level ESD simulation is a very complex project  involving a complete structural model, PCB models including  detailed metal traces, power-on chip models, device models,  software working principles, etc. The results of system-level  simulation are relevant if only the accuracy of each model is  high enough. In this work, a simple and efficient modeling  method of ceramic capacitor is proposed, the S parameters  measured by a VNA and the transient current and voltage values  tested by a TLP system can be used to build a Spice model with  the good correlation between simulation and test result in  system-level ESD test. However, when applying this model to  the whole machine simulation, there may be other cases that  need to be considered, such as breakdown characteristics, which  is also the direction that needs to be further explored.

## R EFERENCES 

[1]    Gossner, Harald, Kai Esmark, and Wolfgang Stadler. "Simulation  methods for ESD protection development,"  Elsevier , 2003.    [2]    L. A. Pipes, "A mathematical analysis of a series circuit containing a  nonlinear capacitor,"  Transactions of the American Institute of Electrical  Engineers, Part I: Communication and Electronics , vol. 72, no. 3, pp.  238-244, July 1953.    [3]    Scheier, Stanislav, and Stephan Frei. "Characterization and modeling of  ESD-behavior of multi layer ceramic capacitors."  2013 International  Symposium on Electromagnetic Compatibility.  IEEE, 2013.    [4]    Streibl, Franz. "Electrostatic discharge performance of passive surfacemount components,"  Books on Demand , 2011.    [5]    Hongyu Li, Khilkevich, V., Tianqi Li, Pommerenke, D., Seongtae Kwon,  Hackenberger, W.. "Nonlinear capacitors for ESD protection,"  IEEE  Electromagnetic Compatibility Magazine , vol.1, no.4, pp. 38-46, 2012.    [6]    Johnson, Kenneth M. "Variation of dielectric constant with voltage in  ferroelectrics and its application to parametric devices."  Journal of  Applied Physics , vol. 33, no.4, pp. 2826-2831, 1962.

