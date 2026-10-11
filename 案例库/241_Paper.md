---
title: "241_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_b47b8f4192bd399663ae178af77c70ae7295230462135641
file_size: 900142
---

## Low-Trigger LDMOS-SCR For ESD Protection Of  Single Photon Detector  

Yang Wang 1 , Xiangliang Jin 1\*   1 Department of College of Physics and Electronic Science School of Hunan Normal University, Changsha 410081, China.  Email: Jinxl@hunnu.edu.cn

Abstract-   In order to improve the anti-ESD capability of the single  photon detector core chip, a one-way low-trigger LDMOS-SCR  device structure is used for on-chip ESD protection. Based on a   $\mathbf{0.5upm}$   standard CMOS process, Analyze the working mechanism  of the device through the equivalent circuit and two-dimensional  device simulation. The   $\mathbf{P}+$   implant region is set on the trigger  surface of the LDMOS-SCR to reduce the trigger voltage of the  device, and DNW is added to prevent the substrate noise carriers  from affecting the device. The results show that the trigger voltage  of the low-trigger LDMOS-SCR device is 19.57V, the sustain  voltage is 5.37V, the failure current is 7.35A, and the HBM level is  11KV. The test results meet the ESD protection requirements of  the single photon detector core chip. By adjusting the size of D6, it  is found that the increase of D6 size can effectively improve the  sustain voltage of LDMOS-SCR device and effectively prevent  latch-up effect. And the failure level of the device will not be  significantly reduced.

Keywords  –  CMOS, LDMOS-SCR, HBM Level .

## I. I NTRODUCTION 

The level of integrated circuit manufacturing technology  continues to increase, and the problem of robustness of  single-photon detector core chips has become increasingly  prominent[1]. The window metrics currently used for integrated  ESD protection devices on single photon detectors are: the ESD  device trigger voltage is less than 24V, the sustain voltage is  greater than 4V, and the HBM level is greater than 8KV. The  data is shown in Table I.

TABLE I ESD PROTECTION DEVICE DESIGN SPECIFICATION FOR ON-CHIP INTEGRATED SINGLE PHOTON DETECTOR

|ESD Window||VV）|Ir(A)|HBM|
|---|---|---|---|---|
|On-chip ESD device|||VS.S||


LDMOS-SCR devices fabricated in standard CMOS  processes are the best choice for ESD protection of single  photon detector I/O ports[2-4]. SCR has the best robustness per  unit area, and the unique snapback characteristic of the device  can effectively improve the failure ability of SCR[5]. However,  the trigger voltage of the conventional SCR structure is higher,  which is not conducive to on-chip integration of the device. In  the standard CMOS process, an optimized structure of LDMOS  is generally used as the ESD protection device, and the LDMOS  structure discharges the ESD current through the internal  parasitic BJT, but the failure level is difficult to increase. The

traditional LDMOS-SCR device combines the advantages of  the above two structures[6-8]. This paper improves the  structure of the traditional LDMOS-SCR device, reduces the  trigger voltage of the device, increases the device's failure  capability, and adjusts its ESD window, enable LDMOS-SCR  to meet the ESD design requirements of the target chip. And by  adjusting the size D6, the purpose of increasing the sustain  voltage without reducing the failure current is achieved.

II.

D

## ESIGN  A ND  D ISCUSSION  O F  L OW -T RIGGER  LDMOS-SCR  

Single photon detectors need to work in Geiger mode for  single photon detection, therefore, the LDMOS-SCR for high  voltage applications meets the requirements of high voltage  ESD protection.

Although the conventional LDMOS-SCR structure can  provide one-way ESD protection, the device trigger voltage is  too high and the failure level is low. The device does not meet  the ESD protection requirements of the single photon detector  core chip, and the chip cannot be effectively protected.  Therefore, on the basis of the conventional LDMOS-SCR  structure, by adding a  $\mathrm{P}+$   implant region for forming the trigger  faces of   $\mathrm{P}+$   and DNW, the trigger voltage is lowered, and the  substrate isolation is performed by using DNW to prevent  carrier migration. The cross-sectional view and equivalent  circuit of the low-trigger LDMOS-SCR device are shown in  Fig. 1 and Fig. 2. In order to further increase the holding voltage  of the device and prevent the latch-up effect, the size D6 is  adjusted on the basis of the original size of the device in order to  increase the holding voltage of the device without significantly  reducing the failure level of the device.

![Cathode  Cathode  Anode  Anode FOX  FOX   FOX  FOX   FOX  FOX   FOX  FOX   FOX  FOX   FOX  FOX  P+  P+   +  N+   D3  D3  P+ P   P  P+   T  N+  S  D5  D4   D6  DDS  D5 D6  LDI  D1  LDI  D1  D2_   LDI  D1  LID1-  D1 P-vell  P-Well DNWELL DNWELL  P-SUB  P-SUB ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/48545573-4143-40a8-8fd6-bf638f277c3d/48545573-4143-40a8-8fd6-bf638f277c3d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=bf641f9e37bd34fbba6c6f9bd4280b9be8b8dc65)
Fig. 1 Cross section of the low-trigger LDMOS-SCR.

When the single photon detector works normally, the trigger  voltage of the LDMOS-SCR device cannot be reached due to  the normal working voltage of the chip. That is, the avalanche  breakdown voltage of the   $\mathrm{P}+$  implant region and the DNW

reverse PN junction. Therefore, the LDMOS-SCR structure  will not be turned on. However, when the forward ESD stress  reaches the I/O port of the single photon detector, the floating   $\mathrm{P}+$   and DNW of the low-trigger LDMOS-SCR device  avalanche breakdown, the large amount of avalanche carriers  generated by the avalanche effect will cause the voltage drop of  the parasitic resistance RP-Well of the P-Well to increase.  When the voltage drop reaches the turn-on voltage of the  parasitic NPN (DNW/P-Well/cathode  $\mathrm{N}+\mathrm{'}$  ), the NPN is turned  on. ESD current stress is vented. Due to the positive feedback,  the parasitic PNP (anode P+/DNW/cathode   $\mathrm{P}+$  ) is also turned  on due to the voltage drop caused by the avalanche carrier at the  parasitic resistance RDNW of the DNW. The PNPN path  consisting of the anodes   $\mathrm{P}+$  , DNW, P-Well, and cathode   $\Nu+$   is  gradually formed, that is, the SCR path is turned on, and the  ESD current stress is released. The low-trigger LDMOS-SCR  device reduces the trigger voltage of the device by adding a  floating   $\mathrm{P}+$   structure to meet the ESD trigger window  requirements of the single-photon detector core chip. The role  of DNW can provide the parasitic resistance RDNW of the  parasitic PNP. It can also effectively isolate the influence of the  substrate carriers on the device and prevent the latch-up effect.  The existence of the isolation layer on the right side of the  floating   $\mathrm{P}+$   makes the conduction path of the anode to the  cathode become longer, effectively increasing the sustain  voltage of the device. The low-trigger LDMOS-SCR can meet  the window requirements of the ESD sustain voltage of the  single photon detector core chip.

![Anode Anode  RDNw  R DNW PNP  PNP NIPN  NPN RP-Well  R P-Well Cathode Cathode  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5fc576ba-1e0d-45d6-a526-45cc7087ac31/5fc576ba-1e0d-45d6-a526-45cc7087ac31.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=70b17515bec440b5f54603ba296339b2e8f934f6)
Fig. 2 Equivalent circuit of the low-trigger LDMOS-SCR.

effect, the electron current   increases with distance. At  $\mathbf{X}{=}\mathbf{a}$  , the  electron current is:

$$\tilde{I}_{\pi}(\alpha)=M_{\pi}\tilde{I}_{\pi0}$$
(1)

$M_{\pi}$   is an avalanche multiplication factor, and the hole current  gradually increases in the depletion region and reaches a  maximum at  $\scriptstyle{\mathbf{X}=0}$  . Within the PN junction, the electron current  increase at x is:

(2)

$$\begin{array}{r l r}&{}&{\mathsf{d}I_{n}(x)=I_{n}(x)\alpha_{n}\mathsf{d}x+I_{p}(x)\alpha_{p}\mathsf{d}x}\\ &{}&{\quad\frac{d I_{n}(x)}{d x}=I_{n}(x)\alpha_{n}+I_{p}(x)\alpha_{p}}\end{array}$$
(3)

$\alpha_{n}$   and  $\alpha_{p}$   represent electron ionization rate and hole ionization  rate, respectively.

The total current is:

(4)

$$\begin{array}{c}{{{\tt I}={\tt I}_{n}(x)+{\tt I}_{p}(x)}}\\ {{\displaystyle\frac{d{\tt I}_{n}(x)}{d x}\!+\!\left(\alpha_{p}-\alpha_{n}\right)\!{\tt I}_{n}(x)=\alpha_{p}{\tt I}}}\end{array}$$
(5)

Assuming that the electron ionization rate and the hole  ionization rate are the same, the equation (5) is integrated over  the entire space charge region:

Analysis of the breakdown mechanism of   $\mathrm{P}+$   and DNW,  ensure that enough carrier-conducting parasitic SCR paths are  generated.  $\mathrm{P}+$   is a heavily doped region and DNW is a lightly  doped region. The physical mechanism for forming  reverse-bias PN junction breakdown is divided into tunnel  breakdown and avalanche breakdown. Due to the low doping  concentration of DNW, the avalanche breakdown probability is  much greater than the probability of tunnel breakdown.  Suppose that at  $\scriptstyle{\mathbf{X}=0}$   of the PN junction, the reverse bias electron  current   enters the depletion region. Due to the avalanche

(6)

$$\begin{array}{l}{{\displaystyle I_{n}(\alpha)-I_{n}(0)=I\int_{0}^{\alpha}\!\!\alpha d x}}\\ {{\displaystyle\frac{M_{m}I_{m0}-I_{n}(0)}{I}{}=\int_{0}^{\alpha}\!\!\alpha d x}}\end{array}$$
Since  $M_{\pi}\bar{I}_{\pi0}$   is approximately equal to   $I,I_{n}(0)\!\!=\!\!I_{n0}$  , therefore:

$$\scriptstyle1-{\frac{1}{M_{n}}}=\int_{0}^{\alpha}\!\alpha d x$$
(8)

When the multiplication factor   $M_{\pi}$  reaches infinity, it is defined  as the avalanche breakdown voltage.

$\mathrm{P}+$   and DNW are   $\mathsf{p}\mathrm{+}\mathsf{n}$   junctions, and their maximum electric  field strength is:

$$E_{m a x}\!=\!\frac{e N_{d}x_{\pi}}{\mathsf{E}_{s}}$$
(9)

The breakdown voltage Vb of the  $\mathsf{p}\mathrm{+}\mathsf{n}$   junction is:

$$V_{b}=\frac{\dot{\mathsf{S}_{s}}\,E_{m a x}}{2e N_{B}}$$
(10)

$N_{B}$   is the concentration on the low doped side. The trigger  voltage of the low-trigger LDMOS-SCR is thus obtained, and  by theoretical analysis, the avalanche carriers generated after  the avalanche breakdown are sufficient to open the parasitic  SCR path inside the device.

## III.   T WO -D IMENSIONAL  S IMULATION  A ND  D ISCUSSION 

Two-dimensional   device   simulation   of   low-trigger  LDMOS-SCR devices using TCAD software, using the atlas  simulator to verify the device's operating principle. Fig. 3  shows the impact ionization distribution of the low-trigger  LDMOS-SCR device. It can be clearly seen that the peak of the  impact ionization is at the reverse bias PN junction of   $\mathrm{P}+$   and  DNW. And as seen from Fig. 4, the intensity of the electric field  of the device is   $105~\mathrm{V/cm}$  , indicating that the breakdown effect  of the device is avalanche breakdown, not tunnel breakdown.  Fig. 5 shows the initial on-current path of the device. The main

bleed path of the current is in the low-resistance, highly doped   $\mathrm{P}+$   implant region, forming a BJT path from the anode  $\mathrm{P}+$   to the  cathode   $\mathrm{P}+$  , indicates that the SCR path is not fully formed  when the device is initially turned on.

Fig. 6 shows the current density distribution after the device  is fully turned on. The PNPN path consisting of the anode  $\mathrm{P}+$  ,  DNW, P-Well, and cathode  $\Nu+$   is fully formed, and the current  density is evenly distributed inside the device. The main  conduction path is still the low resistance region formed by the  floating  $\mathrm{P}+$  . Fig. 7 shows the lattice temperature after the device  is fully turned on. It can be clearly seen that the peak of the  lattice temperature is in the reverse bias PN junction of   $\mathrm{P}+$   and  DNW, so the failure point of the device after reaching the  secondary breakdown current can be predicted.

![Impact ionizationofP+ andDNW  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/71dc1715-441a-4af4-935c-3a50c0c3d83f/71dc1715-441a-4af4-935c-3a50c0c3d83f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=36c466c04c038d931b19c26696dbcbbc17c28f51)
Fig. 3 Impact ionization of low-trigger LDMOS-SCR.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f3186515-1c14-4953-87dc-dfaebdf07c7f/f3186515-1c14-4953-87dc-dfaebdf07c7f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=b5a5331f281bee370e5edc26aa482cc7318cc267)
Fig. 4 The Electric field distribution when the low-trigger LDMOS-SCR is  slightly turned on.

![PNPcurrentpath  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d47f3434-4e17-429e-80cf-09990160f38d/d47f3434-4e17-429e-80cf-09990160f38d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=77bac1394f42f201b55f33bebc142ee7cbd91702)
Fig. 5 The total current density distribution when the low-trigger LDMOS-SCR  is slightly turned on.

Floating  $\mathrm{P}+$   is the main current bleed path of LDMOS-SCR.  Therefore, adjusting the size of floating   $\mathrm{P}+$   can effectively

increase the distance from the anode to the cathode of the  device, thereby increasing the sustain voltage. However, the  longer the size of the floating   $\mathrm{P}+$  , the more the number of  carriers at the time of conduction, so the failure capability is  significantly reduced.

![SCR current path  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/521cd46d-ab0c-4ed7-9ed8-cf36c0c7f6a0/521cd46d-ab0c-4ed7-9ed8-cf36c0c7f6a0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=9bd7ae9745048ed679648b9c4b10272ff2ee5c86)
Fig. 6 The total current density distribution when the low-trigger LDMOS-SCR  is fully turned on.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2c1318a0-835d-4f0c-acd5-26b7ccb50563/2c1318a0-835d-4f0c-acd5-26b7ccb50563.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=6495c96ed9c1fc5f5e42c3abe3bbde759d0d7995)
Fig. 7 The lattice temperature when the low-trigger LDMOS-SCR is fully  turned on.

## IV .   E XPERIMENTAL  R ESULTS  A ND  D ISCUSSION 

Single-finger low-trigger LDMOS-SCR device designed  through a   $0.5\upmu\mathrm{m}$   standard CMOS process. Tested with a 10 ns  rise time and a 100 ns pulse width transmission line pulse （ TLP ） , the trigger voltage, sustain voltage, and failure current of the  device under HBM ESD impact were investigated. A  micrograph of the low-trigger LDMOS-SCR device is shown in  Figure 8.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/41464cfd-1138-4fe0-b1c7-c26738cafc55/41464cfd-1138-4fe0-b1c7-c26738cafc55.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=0936a2c3f8c818b937d2c4347ac0cf77f64cac9d)
Fig. 8 Microscope image of the low-trigger LDMOS-SCR.

Figure 9 shows a TLP test plot for a single-finger low-trigger  LDMOS-SCR device. The results show that the device has  good snapback characteristics, and the leakage current is stable  at nA level until the second breakdown occurs in the device,  and the leakage current drift exceeds   $\upmu\mathrm{A}$  . The trigger voltage of  the device is 19.57V, which exceeds the normal operating  voltage of the single photon detector and is lower than the  breakdown voltage of the thinnest gate oxide of the chip. The

sustain voltage is 5.37V, the failure current is 7.35A, and the  HBM level is 11KV, which can meet the on-chip ESD  protection requirements of single photon detectors and prevent  the occurrence of latch-up effect, protect the complete  transmission of circuit signals.

of D6, the device can effectively increase the sustain voltage  while maintaining the failure level, Stay away from the negative  effects of the latch-up effect. The low-trigger LDMOS-SCR  two D6 size data is shown in Table II.

![Leakage(A)  1E-10   1E-9   1E-8   1E-7   1E-6   1E-5   1E-4   1E-3  Voltage (V)  Leakage (A)  20   30   S0  Voltage (V)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3894153a-363a-469a-adb6-376ddbc697c3/3894153a-363a-469a-adb6-376ddbc697c3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=031d410dc21897d9f2b9542e0f768c59b76fd0c1)
Fig. 9 TLP I-V curves of single-finger low-trigger LDMOS-SCR.

## V .   C ONCLUSION 

In this paper, the structure of low-trigger LDMOS-SCR  device is introduced, and the working mechanism of the device  is analyzed. The ideal characteristics of the device are described  in detail through TCAD two-dimensional device simulation and  equivalent circuit. Low-trigger LDMOS-SCR device fabricated  on a   $0.5\upmu\mathrm{m}$   standard CMOS process, Through the TLP test, the  device results meet the ESD protection requirements of the  single photon detector core chip. In addition, through the  discussion of the size D6, the key factors affecting the sustain  voltage of the device are found, and the sustain voltage of the  device can be improved while ensuring the failure current, and  the latch-up effect is prevented. In summary, this low-trigger  LDMOS-SCR structure can provide a better design idea for the  ESD design of single-photon detectors.

![10°101010′10°10101010²1010°10′10²10²101010  1  LDMOS-SCR（D6=2.5um)  LDMOS-SCR(D6=5.0m)  Leakage current(A)  10\* 10\* 10\* 10 10 10 10° 10' 10 10′ 10′ 10 10  Voltage (V)  45   55   30   35   40   45   50   55  Voltage (V)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3b2b58bc-6e6d-4c77-95bc-ec716dccb68a/3b2b58bc-6e6d-4c77-95bc-ec716dccb68a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=fde4219213984e78d2da22e16d2becb4cc2ae617)
## A CKNOWLEDGMENT 

This work is supported by the National Natural Science  Foundation of China (Grant No. 61827812, 61774129) and  Changsha   Science   and   Technology   Plan   Key  Projects(kq1801035).

## R EFERENCES 

Fig. 10 TLP I-V curves of single-finger low-trigger LDMOS-SCR.(  $_{ Ḋ }\mathrm{Ḋ}6 Ḍ Ḍ {=}2.5\upmu\mathrm{m}$  ,   $5\upmu\mathrm{m})$  ).  TABLE II  L OW -T RIGGER  LDMOS-SCR   D EVICE  T EST  R ESULTS

|Device name|VV)|VV）|Ir(A)|HBM|
|---|---|---|---|---|
|LDMOS-SCR (D6=2.5μm)|19.57|5.37|7.35|11.02|
|LDMOS-SCR (D6=5.0um)|19.61|6.0|7.35|11.02|


In order to further increase the sustain voltage of the  low-trigger LDMOS-SCR device, the risk of latch-up of the  device is reduced. The size of the device D6 was increased from   $2.5\ \upmu\mathrm{m}$   to  $5.0\;\upmu\mathrm{m}$  . Since the position of D6 is not the main path  for device bleed, increasing the size of D6 can lengthen the  distance between the anode and the cathode, effectively  increase the sustain voltage, and ensure that the failure  capability of the device does not decrease significantly. The  TLP test curve of D6 size comparison is shown in Figure 10. It  can be seen that when   $\scriptstyle{\mathrm{D}}6=5\upmu\mathrm{m}$  , the trigger voltage of the  low-trigger LDMOS-SCR device has no significant change, but  the sustain voltage of the device is increased to 6V, and the  failure current is still 7.35A, the HBM level is 11KV. Verify the  theoretical derivation of Section 2, that is, by changing the size

[1]    Dead Time Compensation in CMOS Single Photon Avalanche Diodes  With Active Quenching and External Reset[J]. IEEE Transactions on  Electron Devices, 2014, 61(8):2725-2731.     [2]    Liang H , Gu X , Dong S , et al. RC-Embedded LDMOS-SCR With High  Holding Current for High-Voltage I/O ESD Protection[J]. IEEE  Transactions on Device & Materials Reliability, 2015, 15(4):495-499.     [3]    Lee J H ,  Prabhu M ,  Natarajan M I . Engineering ESD Robust LDMOS  SCR Devices in FinFET Technology[J]. IEEE Electron Device Letters,  2018:1-1.    [4]    Danilo Bronzi ; Simone Tisa ; Federica Villa ; Simone Bellisai ; Alberto  Tosi ; Franco Zappa. Fast Sensing and Quenching of CMOS SPADs for  Minimal Afterpulsing Effects[J]. IEEE Photonics Technology Letters ， Year: 2013 , Volume: 25 , Issue: 8 Pages: 776-779.     [5]    Liu, Wen , et al. "Bidirectional Diode-Triggered Silicon-Controlled  Rectifiers for Low-Voltage ESD Protection." IEEE Electron Device  Letters 33.10(2012):1360-1362.    [6]    Do XY, Dong SR, Han Y , Liou JJ. Analysis of Metal Routing Technique  in a Novel Dual Direction Multi-finger SCR ESD Protection Device. 9th  International   Conference   on   Solid-State   and   Integrated-Circuit  Technology. (2008).     [7]    K Zhu, Z Yu, S Dong, Y Han. Design analysis of a novel low triggering  voltage dual direction SCR ESD device in   $0.18~\mathrm{~\upmum}$  mixed mode  RFCMOS technology. Chin. J. Semicond. vol. 29, no. 11, pp. 2164–2168,  2008.    [8]    Yuan Wang, Guangyi Lu, Jian Cao, Song Jia, Ganggang Zhang, Xing  Zhang. Analysis of dummy-gate dual-directional SCR (dSCR) device for  ESD protection. Proceedings of the 20th IEEE International Symposium  on the Physical and Failure Analysis of Integrated Circuits (IPFA). Year:  2013 Pages: 720 – 723.

