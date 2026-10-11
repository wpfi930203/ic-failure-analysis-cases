---
title: "178_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_691075c132e719d9bf732c19aca2dd1a7295230462135641
file_size: 642283
---

## Optical Failure Analysis on Pulsed Signals Embedded  in Logic Cloud – A Case Study of Laser Voltage  Tracing   

Yuzhu Sun 1 \*, Daisy  $\mathrm{L}\boldsymbol{\mathrm{u}}^{2*}$  , Dave Mark 2 , Chennian   $\mathrm{D}\mathrm{i}^{2}$  , Jenny Fan 2  and Neel Leslie 1  1 Thermo Fisher Scientific, 3400 W. Warren Ave, Fremont, CA, 94538  Phone: +1 510-897-6433  Email: yuzhu.sun@thermofisher.com  2 Xilinx, Inc., 2100 All Programmable Drive, San Jose, CA, 95124  Phone:+1 408-879-6827  Email: daisyl@xilinx.com

Abstract-   LVx, including Laser Voltage Imaging(LVI) and Laser  Voltage Probing(LVP), is an indispensable optical failure analysis  tool set for design debug and yield ramp-up. Although LVI and  LVP together provide a good coverage for failure analysis cases  involving scan-chain functionality testing, their applicability  remains limited when addressing pulsed signals from logic circuits  with ever growing complexity. Laser Voltage Tracing(LVT), as a  recent addition to the LVx suite, provides a global map,  highlighting the active region with low duty-cycle voltage  transition pattern. In this paper, we present a case study of the  detection of timing abnormality for a waveform feature with   ${\tt<}{\bf0.1\%}$   duty cycle by applying LVT. Complemented by LVP and  Soft Defect Localization (SDL), the fault was localized down to  two interconnected logic gates. Resistive interconnection was  confirmed with Physical Failure Analysis(PFA).

Keywords – LVx, Laser Voltage Tracing,  Low duty cycle signal

## I. I NTRODUCTION 

Quality assurance for integrated circuits with increasing  density and complexity has demanded the development of more  efficient electrical and optical failure analysis techniques.  Although PFA is usually adopted for revealing the root cause,  fault area localization with preceding test procedures is a  prerequisite for successful PFA. With the design for testing  techniques such as scan chain, faulty device behavior down to  certain functional path or test nodes could be detected with  customized Automatic Test Pattern Generation(ATPG) patterns.  To further isolate the failure site, there exists a suite of  well-established optical methods either based on Photon  Emission Microscope(PEM), or coupled with Laser Scanning  Microscope(LSM).

Within the family of LSM based techniques, SDL directly  pinpoints the soft defect location by monitoring the pass/fail  state of a device under laser-induced local heating [1]. However  the spots could be real spots or victims. LVI provides a visual  display that highlights the transistors toggling at the selected  frequency as the laser is scanned across a running device. LVP  provides direct waveform information induced by the working  transistors as the laser is parked at certain locations. Although  LVI has proven to be productive in scan chain stuck-at shift  failure analysis [2], or in providing better guidance on where to  perform laser probing [3], its requirements for periodic signal

and 50/50 duty cycle [4] makes it unsuitable for debugging  failure in deep logic cloud, as it is almost impossible to generate  a known frequency toggling data pattern through scan chain

![resistiveinterconnect    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/935bfac3-bf94-4ca8-ad79-f5b699d5433b/935bfac3-bf94-4ca8-ad79-f5b699d5433b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=53a46ea8e56fef2a23e2500b95fc4b898acd32e4)
Fig1. Diagram showing the resistive interconnect of  about 5um between  suspected logic unit

feed in. Probing with LVP can be costly for both engineer effort  and tool time.

A recently developed technique called LVT relaxed the  limitations on detectable signals imposed by LVI [5].  LVT  records the integrated effect of waveform features within a  defined gate. It creates a mapping between these waveform  features and the embedded functional nodes location. Thus  LVT also alleviates the burden of relentless probing with LVP.  In the second part of this paper, we will provide more details of  the LVT principles and applications. In the third part, we will  describe a case study on isolating a failure site around a NAND  gate within the sea of logic as shown in Fig. 1. A full failure  analysis workflow was implemented for this case including  electrical logic analysis, PEM, LVT and SDL. Further PFA  found faulty resistive interconnect that causes transmission  delay and signal stuck-at leading to the spot pinpointed by both  LVT and SDL.

## II.   B ACKGROUND ON  L ASER  V OLTAGE  T RACING 

LVT emanates from the need of extracting voltage transition  information of circuits processing low duty-cycle pulses. The

![Running device  Beam  Detector  splitter   RFsignal  Gated integrator  Aperture  Aperture  Cwlaser  Simplified diagram of LSM  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c8b5621e-1c02-40b8-9ddd-921c0cea2540/c8b5621e-1c02-40b8-9ddd-921c0cea2540.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=df7b3aeb6defc43ad72b305f5cbfc27cffc3f8b7)
Fig. 2 Schematic of simplified LVT implementation.

simplified implementation of LVT is illustrated in Fig. 2. The  LVT setup is similar to that of the LVI or LVP, as it performs  waveform analysis on the reflected laser beam from the LSM.  In more details, the optical properties within the active regions  of the Device Under Test(DUT) is perturbed by the changing  density of free carriers. When the laser beam is focused on to  these regions, the combinational effect of changing absorption  coefficient, reflectivity, and refractive index will be reflected as  the free-carrier induced modulation on the reflected laser beam.  The RF component of the electrical output from the LSM,  which is mentioned as the LVx signal, is analyzed with a gated  integrator. By cutting out a tight temporal window near the  waveform feature of interest for integration, irrelevant noise  could be excluded, and thus improving the signal to noise ratio  (SNR) performance.

![Synchronous  trigger  LVx Signal, V(t)  Gated signal, V,(t)  Measurement   Baseline  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2907aec4-a57c-4ade-9f92-d353a1fa1bf5/2907aec4-a57c-4ade-9f92-d353a1fa1bf5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=f815d86eddb03daefdb10a9acceb0c8ec2e7571d)
Fig3. Temporal diagram for LVT gated integrator.

The temporal diagram of the gated integrator operation is  shown in Fig. 3. A trigger of period T synchronous with the test  loop is required for the LVT integrator. A measurement  window is set with a delay of  relative to the trigger, and a gate  width of   . To account for the DC level change, a baseline  window of the same gate width   $\delta\ddagger$   is placed in a temporal  location with no signal. The integrated signal level from the  measurement window is subtracted by that from the baseline  window, and then averaged over a number of n trigger period.  As the LSM laser beam raster scans across the region of interest,  such operation is performed at each pixel to construct the LVT  data layer. Assuming the LVx signal is V(t), the LVT layer  pixel value can be written as:

$$\bar{F}=\pi K\int_{\bar{s}}^{\bar{s}+\bar{s}\bar{t}}\bar{F}(\bar{s})\,d\bar{t}-\pi K\int_{\bar{s}_{\bar{s}}}^{\bar{s}_{\bar{s}}+\bar{s}\bar{t}}\bar{F}(\bar{s})\,d\bar{s},$$
where K is determined by the integrator gain factor. Depending  on the sign of the net integration value, we will have a white  (positive value) or a black (negative value) pixel. With proper  setting of the gate width and position, LVT has another benefit  of separating out real signal in the presence of cross-talk [6].

III. Case Study: LVT for fault isolation in deep logic cloud

A failure from scan transition test on the DUT was analyzed  during yield ramp up. Logic fault isolation suspected defective  inverter of combination logic gate embedded in deep logic  cloud, as shown in Fig. 4(a). The failure was marginal to Vcc,  and PEM shows no anomaly on the bad unit. Although SDL  identified the NAND gate at the next stage, as shown in Fig.  4(b). However, to further confirm the failure location, direct  investigation on the voltage transition is needed. Due to the

![SDL point to A1;  abnormal LVT implies  delayedtransition  Resistiveviafound from  INV output toA1  Suspected by logic  fault isolation, LVT  normal  NAND  SDL @ NAND gate  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/216b010d-7fc7-49eb-a792-d785710b068b/216b010d-7fc7-49eb-a792-d785710b068b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=174ae255582b5c8b63cc207647a8fedd9883ce87)
Fig. 4 (a)The combination logic gate at investigation. (b)SDL spot pointing to  the input port of NAND. Electrical testing points to the invertor, while SDL  points to the NAND. LVT also only shows abnormal pattern at NAND with the  A2 port staying quiet during testing

lack of regular toggling pattern on the failing path, LVI is not  suitable for the case study. In order to avoid the timing cost of  intensive probing within the suspected region, LVT was  performed near both inverter and the NAND gate to obtain a  visual guidance on probing locations. To perform LVT on the  suspected nodes, the DUT was set to loop on one compressed  transition pattern. An ATPG pattern that triggers a pulse  generation during the launch and capture period of scan chain  testing was shifted in. The timing diagram is shown in Fig. 5.   As a reference, the pulsed waveform was first observed on a

good unit once for optimizing the gate width and location  settings. The same settings were applied for LVT imaging on  both the good and bad unit for comparison.

The LVT imaging results from both the invertor and the  NAND gate are shown in Fig. 6. In this case, the expected  waveform feature is of width 49.4ns within a test loop of  58.4us, which corresponds to a duty cycle of about   $0.085\%$  . At  each pixel, the measurements were averaged over 4096 trigger  loops. The width of the gates was set as 59.4ns to cover only the  expected pulse as much as possible for SNR consideration. The  two gates are temporally separated by 537ns. Since the two  active logic nodes at investigation are located about 5um apart,

![LVT gate Is set to cateh the transldlon  Apulse during  launch and capturc  phase atthe  investigated node  CLK  SEM  Shiftin   Launch/   Shiftout  Capture  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a35f481f-db6d-4b6d-afb3-a2ea6a48182c/a35f481f-db6d-4b6d-afb3-a2ea6a48182c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=3d702dec94e0a427e2d4750359b655d87ac59da6)
Fig. 5 Timing schematic of the investigated device. Scan Enable(SEN) is set to  1 during the shift in and shift out period. Once all the bins have been shifted in,  SEN is set to 0. During the launch and capture period, we toggle the clock signal

twice. The first clock signal launches a pulsed transition in the relevant  combinational logic circuit, which is then captured by the scan chain following  the second clock signal.

![Good invertor   Badinvertor  ROI: 0.96um.1.09  ROl:0.87um.1.19um  GoodNAND   BadNAND  3   .31m  m.1.3m  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0720619f-ec4b-4c72-b468-3e0f76580f3c/0720619f-ec4b-4c72-b468-3e0f76580f3c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=7707fc7771bccf7af15c209b85f0dd0b9decc0d3)
Fig.6 LVT image comparison between good and bad unit. Spot A and B    correspond to two complementing PMOS and NMOS within the NAND gate.    Spot C and D are from a neighboring logic gate which is not on the failure path  but is toggling synchronously with the trigger signal.

LVT scans were carried out within region of interest (ROI) box

drawn near the invertor and the NAND separately. Fig 6(a) and  6(b) show identical LVT pattern from the invertor on the good  and bad unit. However for spots A and B within the NAND gate  in Fig. 6(c) and 6(d), the polarity change of the LVT pattern  indicates the fault has caused the pulsed waveform feature to be  shifted out of the measurement gate.

To confirm the toggling pattern changes at the NAND gate,  we performed LVP at the four spots A, B, C and D. The  obtained waveforms are shown in Fig. 7. Fig.7(a) from spot A  shows the rising edge is delayed by about 50ns, and is stuck at  high. Fig. 7(b) from spot B shows the falling edge is also  delayed by about 50ns, and is stuck at low. Since the LVT

![a    C    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/36b4b6c4-1928-47b9-b109-53b80e039b9d/36b4b6c4-1928-47b9-b109-53b80e039b9d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=a033fb8caea53229ffe19839c1060fcff5ad8d59)
Fig. 7 (a), (b), (c), (d) are waveforms obtained at spot A, B, C and D  respectively. The blue waveforms are obtained from a good unit. The pink ones  are obtained from the bad unit. The acquisition span was set as 400ns.

measurement gate only covers the expected pulse, the delay

changes the polarity of the LVT net outcomes at spot A and B  on the bad unit. The waveforms obtained from spot C and D  remains similar between the good and bad unit. PFA was then  directed to be focused from the output of the invertor to the  NAND gate. And electron beam absorbed current (EBAC)  revealed resistive interconnect on the metal 3 layer.

## IV. C ONCLUSION 

Here we provide a use case of LVT for debugging faulty  logical circuits involving pulsed signal. In summary, LVT  provides visual mapping of pulsed signal generated within  defined temporal gates. As a global technique, LVT extends the  capability of the LVx family by breaking the limitation on  signal condition posed by LVI. It also serves as an additional  tool when pass/fail test pattern is not available for soft defect  localization. As a visual guidance, LVT improves LVP  efficiency by highlighting the region with unexpected signal  integration outcome.

## A CKNOWLEDGMENT 

The authors would like to thank Xilinx and Thermo Fisher  Scientific management team for supporting this collaboration  work. We would also like to thank Christopher Nemirow for his  initial work on this project.

## R EFERENCES 

[1]    Bruce, M. R., et. al, “Soft Defect Localization (SDL) in Integrated  Circuits using Laser Scanning Microscope”, LEOS, Vol. 2, PP. 662-663,  2003    [2]    Liao, Joy Y.,  et. al , “Scan Chain Failure Analysis using Laser Voltage  Imaging”, Microelectronics Reliability, Vol. 50, Issues 9-11, pp.  1422-1426, 2010    [3]    Kasapi, Steven,  et. al , “Advanced Scan Chain Failure Analysis Using  Laser Modulation Mapping and Continuous Wave Probing”, ISTFA  Proceedings, pp. 12-17, 2011    [4]    Ng, Yin S.  et. al , “Laser Voltage Imaging: A new Perspective of Laser  Voltage Probing.” ISTFA Proceedings, pp. 5-13, 2010    [5]    Nemirow, Christopher,  et. al , “Laser Voltage Tracing: A Novel  Approach for Imaging Pulsed Signal”, ISTFA Proceedings, pp 44-49,  2016    [6]    Ravikumar, V. K.,  et. al,  “Laser Voltage Tracing for Electrical Fault  Isolation of Circuits Propagating Aperiodic Signals”, ISTFA  Proceedings, pp 221-227, 2017

