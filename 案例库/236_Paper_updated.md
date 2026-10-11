---
title: "236_Paper_updated.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_35c29bff098a367efb685e994bcee2b07295230462135641
file_size: 2187220
---

## The application of Time-Domain Reflectometry  (TDR) technique in characterizing Solder ball  failure and accumulated damage in SiP device  

Jiahao Liu 1,2 , Jialin Yi 1 , Fangzhou Chen 1 , Xuanlong Chen 1 , Lijin Qiu 2 , Jianxiong Liu 1 ,   Hao Zhao 1\* , Zhenbo Zhao 1\* , Yiqiang Chen 1\*   1 China Electronic Product Reliability and Environmental Testing Research Institute, Guangzhou 511370, China  2 Department of of Integrated Circuits, Harbin Institute of Technolog, Shenzhen, 518055 , China  \*: corresponding author; Email : 1440186660@qq.com, zhaozb@ceprei.com, yiqiang-chen@hotmail.com

Abstract —Compared to traditional packaging, System-inPackage (SiP) devices have advantages such as high integration  density, short development cycle, and lower manufacturing  costs. However, as the packaging density increases and the  number of stacked layers grows, the occurrence of SiP device  failures caused by Solder balls has become more frequent.  Currently, there is a lack of specialized non-destructive testing  methods for SiP device solder balls. This paper proposed a nondestructive testing technique based on Time-Domain  (TDR)   technology, which successfully located the failed Solder balls.  Moreover, the TDR non-destructive testing technique can be  used to monitor the accumulated damage of solder balls in SiP  devices, providing a reference for characterizing the  degradation of Solder ball  during operating.

Keywords—Time domain reflection technology(TDR), System  in Package(SiP), Solder ball, Failure localization, Cumulative  damage

## I.      I NSTRUCTIONS 

System-in-Package (SiP) encapsulates the most advanced  packaging technologies, including Chip-on-Chip (CoC)  stacking, Wafer-Level Packaging (WLP), Package-onPackage (PoP), passive component and embedded circuit  integration, embedded chips, Integrated Passive Devices  (IPD), Flip Chip (FC), Through-Silicon Via (TSV), etc. It has  become the mainstream development trend in packaging  technology. As shown in Fig. 1, The HTCC vertical stacked  SiP device utilizes solder balls to establish electrical  interconnection between the HTCC substrate and RF chips,  as well as control chips.

![Valuablealloy   RFchip   Surfacemountdevices   SolderBall  Solder   Mire   Conttolchip   HTCCSubstrate   HeatSink  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/47f13f3e-f1b6-44f6-83fc-eb81dd99dfe6/47f13f3e-f1b6-44f6-83fc-eb81dd99dfe6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=8cf41f295b2b54edd7ed6112e7b502938866ba76)
Fig. 1.    SiP device schematic diagram

However, with the packaging density and the number of  stacked layers increasing, the pitch of interconnections of  solder ball continues to decrease, which  poses a challenge to  the reliability of SiP devices [1]. In addition,  Solder balls of

SiP devices face the following issues compared to traditional  packaging: 1) Due to the limited I/O space caused by  numerous internal devices in SiP, there are fewer ports  available for Solder ball testing; 2) If solder ball failures  occur during the test of the final product, it is difficult to  accurately locate the failure point. Therefore, monitoring the   behavior and reliability of solder balls is a crucial issue that  needs to be addressed in the development process of SiP  devices.

Currently, in the field of non-destructive testing  technology for SiP devices, the existing reports mainly  include X-ray (2D/3D X-ray) and Scanning Acoustic  Microscopy (SAM)[2, 3]. However, due to the high density  and high integration of SiP devices, there are technical  bottlenecks such as poor spatial resolution in 2D/3D X-ray  and SAM, make it difficult to accurately locate solder ball  failures in SiP devices. Compared to the aforementioned nondestructive   testing   methods,   non-destructive   testing  technology based on TDR has advantages such as high  resolution and fast response speed, which can be used to  monitor   impedance   changes,   thereby   reflecting   the  cumulative damage to the solder balls [4-7]. However, there  are fewer reports on this technology. In this paper, the TDR  technology was used to perform failure analysis on a SiP  device. The isolation and localization of faulty solder balls  were achieved, validating the application of TDR technology  for characterizing cumulative  damage in solder balls.

## II.    D EVICE  D ESIGN AND  E XPERIMENTAL  S ETUP 

As shown in Fig. 2, this study presented a SiP device  based on High-Temperature Co-fired Ceramic (HTCC)  vertical interconnect technology (the resistors, capacitors,  and inductors are omitted). The dimensions of HTCC  substrate  $\#1$   and HTCC substrate  $\#2$   were  $23\;\mathrm{mm}\times23\;\mathrm{mm}\times$  2 mm and   $41~{\mathrm{mm}}\times41~{\mathrm{mm}}\times3~{\mathrm{mm}},$  , respectively. 33 solder  balls between the substrates were arranged in an array. The   diameter and the  pitch of the solder balls were  $0.5\;\mathrm{mm}$  and 3  mm, respectively. The solder balls were electrically  interconnected by tungsten, with 6 solder balls on each line.  Among them, line #1 and line #4 were symmetrically  distributed around the center, while line #2 and line #3 were  consistent. However, the distance between solder balls on  line #1 and line #4, specifically between solder ball #4 and  #5, was noticeably different  (6 mm and 9 mm, respectively).

![<a)  HTCC  Substrate2  -2  HTCC  Substrate:1:  HTCC  Substrate1  Line2  9mm  Locating  Line1  Hole  Probe  Contact  SolderBall  Goldfinger  HTCC  Substrate2  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b9dac7ab-f1fc-4bd1-bc6d-504d47ee4c1e/b9dac7ab-f1fc-4bd1-bc6d-504d47ee4c1e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=e899aff022099135feae76718aaf4c591f98e981)
Fig. 2.    SiP device: (a)physical image ; (b)schematic diagram

Fig. 3 illustrates a schematic diagram of the TDR testing  system for SiP device,. It utilized a vector network analyzer  (Keysight NS227B) with a probe station (Cascade BTS1000)  to measure the RF impedance of the SiP device. The vector  network analyzer was set to a testing frequency of   $10\;\mathrm{GHz}$  ,  and the testing mode adopted single-ended impedance  detection for the SiP device.  After the TDR testing, the SiP  devices were subjected to accelerated thermal fatigue failure  using a high and low-temperature humidity chamber (GWS,  EL-04KA). The thermal cycling test parameters were set as  follows: the highest temperature was   $125\ \mathrm{~}^{\circ}\mathrm{C}$  , the lowest  temperature was   $-55\ \mathrm{~}^{\circ}\mathrm{C}$  , the dwell time at high and low  temperatures was 12 min, and the rate of temperature rise and  fall  was   $10~^{\circ}\mathrm{C/min}$  , respectively. After 600 cycles, 900  cycles, 1200 cycles, and 1500 cycles, the SiP devices were  extracted for impedance testing. Following the impedance  testing, the SiP devices were sealed using epoxy resin. Then,  the SiP devices were polished using a metal grinding and  polishing   machine   (QATM,   SAPHIR560),   and   the  microscopic structure of the solder balls of  SiP devices was  observed using the scanning electron microscope (Hitachi  U8010). Finally, Workbench and CST simulation software  are used to perform thermal-mechanical coupling simulation  and TDR electromagnetic simulation of the SiP devices,  respectively. The physical parameters of the SiP devices used  in the simulations are shown in Table 1[8,9].

![HTCCSubstrate1  Goldfinger  HTCCSubstrate2   SolderBall  wire  Vectornetworkanalyzer  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/24a57477-4bf7-44b9-bf53-b8a88ff14c68/24a57477-4bf7-44b9-bf53-b8a88ff14c68.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=f6d7c624df4b536151e28eb229e0ba6dd5b0814f)
Fig. 3.    The schematic diagram of the TDR test for the SiP  device

TABLE I.  SIP DEVICE MATERIAL PROPERTIES TABLE:

|Material|Electrical Conductivity|Elastic Modulus|Poisson's ratio|Thermal Expansion Coefficient|
|---|---|---|---|---|
|Units|S/m|GPa|/|ppm/°C|
|HTCC|10^-10|370|0.22|7.9|
|W|5.8×10^7|345|0.28|39.7|
|Solder Ball|3.24×10^6|30|0.35|25|


## III.    TDR   T ESTING  P RINCIPLE 

When there is an impedance change in the transmission  line of SiP device, a portion of the signal will be reflected  while the other portion continues to propagate along the  transmission line. By monitoring the incident voltage   $(\it V_{\mathrm{in}})$   and  reflected voltage   $(\mathit{V}_{\mathrm{e}})$   collected by the TDR, the reflection  coefficient   $\rho$   and the impedance  at the measurement point ( Z  ) can be calculated by  Equation 1 and Equation 2[10].

$$\rho\,{=}\,\frac{V_{\mathrm{re}}}{V_{\mathrm{in}}}$$
(1)

$$Z_{L}=Z_{0}\times\frac{1+\rho}{1\!-\!\rho}\!=\!Z_{0}\times\!\frac{V_{i n}+V_{r e}}{V_{i n}-V_{r e}}$$
(2)

As shown in Fig. 4, the waveform diagrams of the  reflected waves caused by different resistive loads   $(Z_{\mathrm{{L}}})$   were  given. When the load impedance matched the characteristic  impedance, the reflection coefficient was 0, indicating that  the probing pulse will be absorbed by the load without  generating any reflected echo. When an open circuit fault

occured in the transmission process, the load impedance   $Z_{\scriptscriptstyle L}$  approached infinity. In this case, the reflection coefficient  was equal to 1, and the reflected echo was equal to the  amplitude of the incident pulse with the same polarity.

Similarly, when the load impedance   $Z_{\scriptscriptstyle L}$    increases, there will  also be reflected echoes with the same polarity, but the  reflection coefficient is less than 1. When a short circuit fault  occurs in the transmission process, the impedance approaches  0. In this case, the reflection coefficient is equal to -1,  meaning that the amplitude of the reflected echo is equal to  the amplitude of the incident pulse but with opposite polarity.  Similarly, when the load impedance decreased, there will also  be reflected echoes with opposite polarity, but the reflection  coefficient was greater than -1.

![ZL=∞∞,p=+1  ZL> Zo,p<+1  ZL=Zo, p=0  Incidence-   Reflex  ZL<Zo,-1<p<0  Z=0, p=-1  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/89a811d7-7243-41a9-a552-abaf9279ed8b/89a811d7-7243-41a9-a552-abaf9279ed8b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=d9b50805ff1e09f0053f4b659f3bc71e03fba4b6)
Fig. 4.    Translation: TDR tests impedance waveform

As shown in Fig. 5, taking a wire as a typical electronic  component, the TDR technology was used to test it. The test  waveform was a function of impedance variation over time.  Due to the high frequency signal  and the short test distance  during the TDR test, it was approximately assumed that the  speed of signal propagation remains constant. Therefore, the  function of impedance changing with time can be  equivalently represented as a function of impedance variation  over  transmission distance. As shown in equation 3, by  obtaining the time of impedance anomaly points, the location  of device failure can be calculated. Where   $D\,,\,\nu\,,t$     were  the distance, speed and delay time, respectively.

![Incident  L1=v\*t/2   L2=v\*t2/2  Time  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/09529626-c2f3-4ea6-ac3f-81be28ef9ff4/09529626-c2f3-4ea6-ac3f-81be28ef9ff4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=29e51fdb1ad655634ecb0d171cbb929457ba1f0f)
Fig. 5.    Waveform graph of impedance variation over time

$$D\,{=}\,\frac{\nu t}{2}$$
(3)

## IV.    R ESULTS AND  D ISCUSSION 

A.   Application of  TDR for locating failures of SiP solder  balls

In order to eliminate random errors, 4 samples from the  same batch were selected for each test, and the test results of  the signals from the same channel were averaged.  The

waveform of impedance variation over time  for line #1 and  line  $\#2$   of the initial SiP devices was shown in Fig. 6. Due to  the impedance of the wires in the SiP device design being set  at 45Ω, which was higher than the impedance of the solder  balls (20-30Ω)[11-13]. The solder balls were located at the  trough position of the waveform in Fig. 6. Additionally,  during the testing process, two probes were introduced at the  input/output ports. Therefore, in Fig. 6, the eight troughs from  left to right represent probe #1, solder balls #1-#6, and probe  #2, respectively. From Fig. 6, the times of signals  passed  through solder ball #4 and solder ball #5 on line #1 and line  #2 were 0.1257 ns and 0.1882 ns, respectively. The distances  between solder ball #4 and solder ball #5 on line  $\#1$   and line  #2 were 6 mm and 9 mm, respectively. Using equation 3,  the  propagation velocity of the time-domain reflection signals in  the SiP device can be calculated as  $9.56\!\times\!10^{7}\,\mathrm{m/s}$  .

![(a) 56 Line1 Line2 S Probe 18 0.4  08  12 Time (ns) （D) 60 Line1 SS Line2 S2 0.1257ns 0.1882ns O.S  0.6  07  08  0.9  1.0 Time (ns) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7158d4e6-126b-4c2c-849b-5432ae1c2dc1/7158d4e6-126b-4c2c-849b-5432ae1c2dc1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=fddd855ca3b6af40d037b0fe0c16752b9fc1df61)
Fig. 6.    Waveform graph of impedance variation over time of  SiP device:(a) channels  of Line 1 and Line 2;  (b) Zoomed-in  image in Fig. (a)

The waveform of SiP Solder balls after 1500 cycles of  temperature cycling was shown in Fig. 7. Compared to the  initial waveform, the waveform of Line #1 of SiP device  is  significantly different after 1500 cycles. At the edge of  solder  ball , the impedance increased sharply, indicating the  presence of an open circuit near the solder ball #1.  Additionally, the time from probe #1 to the failure point in  Fig. 6 was 0.2018 ns. The distance of the failure point can be  calculated using equation 3 (  $9.64\:\mathrm{\mm})$  . This result was

adjacent to the distance between probe #1 with  solder ball  #1.

![SS  Probe2  48  Pobe1   Initial state (O cycle)  lailure stats(1500 cycles)  0.0   0.4   0.8   12   20  Time(ns)  60  58  48  LProbel:  0.2018 1s   Initial state (0 cycle)  Failure state (1500 eyeles)  10,0   0２   0,4   0_6   0.8   1.0  Time(ns)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f4d25b13-8427-44bb-8e5d-c25e0708f3da/f4d25b13-8427-44bb-8e5d-c25e0708f3da.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=772d54be93437b50e32261460c10f8f5da1441d7)
Fig. 7.    Waveform graph of SiP device impedance over time  after 1500 cycles:(a) channels  of Line 1;  (b) Zoomed-in  image in Fig. (a)

To further determine the failure location of the SiP  device, metallographic samples were prepared. Then, the  solder balls were microscopically observed after 0 cycles,  600 cycles, 900 cycles, and 1500 cycles. As shown in Fig. 8,  it can be observed that the failure point is the solder ball #1  on line 1. Furthermore, as the thermal cycles increased, the  proportion of cracking in solder ball #1 continued to increase  until complete through-cracking.

![（a)  100um   100pm  100μm   100pm  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/99e16ee0-7af8-4544-b8b7-6923f71ef3d4/99e16ee0-7af8-4544-b8b7-6923f71ef3d4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=3e897b4cc24a661a3acec9a737b202039c582e4d)
Fig. 8.    Microscopic morphology of Solder ball #1 at different  thermal cycling cycles:(a) 0 Cycle;  (b) 600 Cycle; (c) 900  Cycles;  (b) 1500 Cycle;

## B.   Application of TDR in characterizing cumulative  damage of SiP Solder balls.  

The network of Ansys Workbench was used to establish  thermal-structural coupled simulation model. The thermal  cycling loads consistent with the experiment mentioned  above. As shown in Fig. 9, the simulation results indicate that  the corner solder balls experience the highest stress (43.04  MPa). The solder ball #1 on line #1 was also located at the  edge, The stress (40.10 MPa) was comparable to the stress of  the corner solder ball, which indicates a high risk of failure at  this solder ball.

![122204  Max point  Equivalent Stres  Type: Equivalent   Unit:Pa  Time:9900 s  2024-2-1 9:15  4.0093e7Max  3.5754e7  3.1415e7  2.7077e7  2.2738e7  1.8399e7  1.406e7  9.721e6  5.3821e6  1.0432e6 Min  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/289b4712-1f0a-4d99-958f-922f8ee0b672/289b4712-1f0a-4d99-958f-922f8ee0b672.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=a017066b6b9c86e4ac17ab9979e2217e8db519af)
Fig. 9.    Stress-strain contour maps of SiP devices:(a) Solder  balls of SiP device;  (b) Zoomed-in image in Fig. (a);

The stress-strain hysteresis curve of solder ball #1 on line  #1 was shown in Fig. 9(a). It can be observed that the solder  ball undergoes continuous irreversible plastic deformation  during the thermal cycling process. As shown in Fig. 9(b),  with the cycles increasing, the strain energy of solder ball #1  continued to increase within each cycle, Which indicates that  the solder ball accumulates damage during the thermal  cycling process. This result was consistent with the  observations of microstructure of  solder ball #1 mentioned  above.

![(a）  5×10 4×107 3×107  Hysteresis loop 另2×107 1X10 0.0  1.0×10²2.0×10-²3.0×10-3  4.0×10-3  5.0×10-3 5.0×10 4.0×10 3.0×10 2.0×10 cycle 1.0×10 0.0 0.0  5.0×103  1.0×104  1.5×104  2.0×104 Time (s) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b438412f-16e8-4b5c-be09-457e75f4bbf6/b438412f-16e8-4b5c-be09-457e75f4bbf6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=ce538d7c3ce2577ac6cd35291e25e7f44440fe85)
Fig. 10.    Thermal-mechanical coupling simulation results of  $1\#$    solder ball on line 1:(a) Stress-strain hysteresis curve;  (b)  Cumulative strain energy

The GMW3172-2012 standard specifies that the crack in  the solder ball should not exceed   $25\%$   of the transverse  interface after temperature cycling testing. The QJ3086A2016 standard specifies that the surface and internal cracks of  the solder ball should not exceed  $25\%$   of the entire solder fill  area.   However,   traditional   testing   methods   require  destructive testing of the SiP device, which have certain  limitations.

In this study, TDR technology was used to characterize  the cumulative damage of solder balls. Impedance testing of  SiP devices after 600 cycles and 900 cycles was conducted  using TDR, and the impedance waveform was shown in Fig.  11. From Fig. 11, it can be observed that compared to the  initial SiP devices, the impedance of the solder balls  continues to increase with the continuous increase of thermal  cycle. This result is consistent with the findings reported by  Daeil et al[14].

![S6  S2  (U)z   S0  48  46  (cycle  Probel   600 cycles  900 cycles  1500cycles  0.0   0.2   0.4   0.6   0.8   1-0  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7e7a509d-d9a4-4fa9-af5d-6a83a7d5b4cc/7e7a509d-d9a4-4fa9-af5d-6a83a7d5b4cc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=ee598d8ef3f8afefc2aa7f990be67c98efc21207)
Fig. 11.    Impedance waveforms of line 1 of SiP device after  different thermal cycling cycles

As shown in Fig. 12(a), a simulation model with cracked  SiP device was constructed using CST software to simulate  and validate the failure of Solder ball 1# on Line 1. The crack  ratios of the solder ball were set to 0,   $30.33\%$  , and   $50\%$  respectively. The impedance waveform of solder balls with  different proportion of crack ratios  was shown in Fig.11(b).  With the crack ratio of the solder ball increasing, the  impedance of the Solder ball also increased. This result was  consistent with the TDR test results, indicating that TDR  technology can effectively characterize the cumulative  damage of solder balls.

![（D） SO ¥048 Z41  Cracked50% 46  Cracked-30% SS  Initialstate 人 ０Ｓ  H.S ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b068bfaf-90b4-47ec-b070-707d98c30a7c/b068bfaf-90b4-47ec-b070-707d98c30a7c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=96dbc13741169742a6b2135db7bad23dd79464c6)
Fig. 12.    TDR simulation model and results: (a) TDR  simulation model; (b) Simulation results of Solder ball  impedance

## V.    C ONCLUSION 

This paper proposes a non-destructive testing technique  based on TDR. This technique can achieve the failure  localization of solder balls in SiP devices, characterize the  accumulated damage of solder balls during temperature  cycling, and thereby reveal the failure mechanism and failure  modes of SiP devices.  1.   In the waveform of impedance variation over time , the 8  trough positions from left to right represent probe #1, solder  balls  $\#1\mathrm{-}\#6$  , and probe  $\#2$  , respectively.  2.   The propagation velocity of electromagnetic wave signals  in the SiP device is  $9.56\!\times\!10^{7}\,\mathrm{m}/\mathrm{s}$  . By measuring the time of  abnormal points on the impedance waveform, the location of  the fault points can be indirectly obtained.  3.   In thermal cycling experiments, solder balls undergo  cumulative fatigue damage, with the greatest impact on the  solder balls at the edges. During the failure process,  microcracks inside the solder ball gradually transform into  macroscopic cracks. As the crack propagationed, the  impedance of the solder ball also increased. Time Domain  Reflectometry (TDR) technology can effectively monitor the  impedance changes in solder balls.

## A CKNOWLEDGMENT  

This work was supported in part by the Key-Area  Research and Development Program of Guangdong Province  under Grant 2022B0701180002, and CEPREI Innovation and  Development Fund No. 22Z04, which were acknowledged

## R EFERENCES 

[1]    Dai, W.J., Wang, Z.K. and Xue, K., “Multi-objectives design  optimization based on multi-objectives Gaussian processes for systemin-package,”IEEE 71ST Electronic Components and Technology  Conference (ECTC 2021), pp. 2151-2157, 2021    [2]    Sessa, V., “X-ray polycapillary characterization and 3D imaging  properties,” International Conference on charged and neutral particles  channeling phenomena, Vol. 6634, pp. 634-642, 2007.    [3]    Zhang, F.,  Zhang, L.“Ultrasound imaging for non-destructive  evaluation of packaging materials. Packaging Technology and  Science,”,vol. 31, no. 10, 661-674, 2018    [4]    Bidzo, D., Poirier, P., Descamps, P. and Domengès, B.,“Isolating  failing site in IC packages using time domain reflectometry case  studies,” Microelectronics Reliability,  Vol. 45 Nos 9/11, pp. 1639- 1644, 2005.    [5]    Chen, M.K., Tai, C.C., Huang, Y.J. and Wu, I., “Failureanalysis of  BAG package by a TDR approach ,” 2020 Int’l Symposium on  Electronic Materials and Packaging, pp. 112-116, 2020.    [6]    He, H.L., Aogu, K., Li, M., Xu, J., Sheng, W., Jones, S.B.,GonzalezTeruel, J.D., Robinson, D.A., Horton, R.,Bristow, K. and Dyck, M., “A  review of time domain reflectometry (TDR) applications in porous  media, ”Advance in Agronomy, Vol. 168, pp. 83-155.,2021.     [7]    Kong, Y., Bennett, C.J. and Hyde, C.J., “A review of non-destructive  testing techniques for the in-situ investigation of fretting fatigue cracks,  ”Materials & Design, Vol. 196, pp. 256-273, 2020.     [8]    Cao, S., Zhang, L. “ Numerical simulation of thermal fatigue behavior  in Solder balls under power cycling conditions.,“ Journal of electronic  packaging, vol. 142, no. 2, 021007, 2020.     [9]    Cao, S., Zhang, L. “Numerical simulation of thermal fatigue behavior  in Solder balls under power cycling conditions,“ Journal of  Electromagnetic waves and applications, vol. 34, no. 13, p. 1771-1781,  2020.     [10]   Lee, L.Y., Chua, K.K., “Enhanced package fault isolation method  using time domain reflectometry (TDR) incorporation with  mathematics,” 2019 IEEE International symposium on the physical and  failure analysis of integrated circuits (IPFA), p. 193-196, 2019.    [11]   DAEIL K, MICHAEL H A, MICHAEL P, “Detection of Solder ball  degradation using RF impedance analysis,” 2008 Electronic  Components and Technology Conference,(ECTC), 2008.    [12]   DAEIL K, MICHAEL H A, MICHAEL P,“Effect of solder. Joint  degradation on RF impedance,“IEEE Explor, vol.12 , p. 566-570,2008.    [13]   DAEIL K, MICHAEL, H A, MICHAEL P, “Detcction of Solder ball  failure precursors on tin-lead and lead-free assemblies using RF  impedance analysis,“ 2009 Eleetronie Components and Technology  Conferenee, 2009.    [14]   DAEIL K, MICHAEL H A, MICHAEL P, “Identification of  interconnect failure mechanisms using RF impedance analysis,“ SPIi,   vol.978, no. 1, p. 234-239,2009.

