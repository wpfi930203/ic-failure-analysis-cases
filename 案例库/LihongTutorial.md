---
title: "LihongTutorial.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_9e8cfcdc7791fd626275f71703d297d27295230462135641
file_size: 4397270
---

## Advanced 2.5D/3D Package  Level Fault Isolation 

IPFA Tutorial July 2, – 5 , 2019 Hangzhou, China

Dr. Lihong Cao   Director   ASE (U.S.) INC.   Sunnyvale, CA, USA

1

## Purpose 

Understand challenges of package level failure analysis

Introduce basic fault isolation techniques for package level  defect localization

Demonstrate case studies to determine the best techniques

Future challenges

## Outline 

Introduction of package level failure analysis

Package level fault isolation techniques

Brief physics of fault isolation techniques with case studies

Summary

## Introduction 

System trends in the industry driving improvements in  performance lead to new factors

![Disruptive Technology  Motion sensing  Olactometry   Driver-less  HDVoice  Augmented  imaging   Processing  humos  Ardio  Robothome  Next-gon  Holographkc  Smarphone   interaction  Ae  astiseant  snartphc   5G   withatch  Mobe  Seneiting  EDGE  TRENDS   SCLOUD   SPECIALIZATION  P   Mobile   Smart   Robotics   Human Augmentation  1990   1995   2000   2006   2010   2014   2017   2020   2030   2040  3Dgpics   DP   Deepneursl   S   Aeca   FirstSoCwith   HWforaudo  eal   network with   NPU  necwork   GP  LYOLE  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f07445b9-0e68-4059-8d39-898f12d18c58/f07445b9-0e68-4059-8d39-898f12d18c58.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=e6d5fa512484400c72f28395dbfcea92560c1bc9)
## Introduction 

The Evolution of Advanced Packaging

![Networking/  Networking/  Automotive  Automotive Data Center  Data Center 5G/Edge  5G/Edge  I0T  IoT ML/AI  ML/AI  Others  Others ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/281a186a-eced-4c34-9848-f91760549445/281a186a-eced-4c34-9848-f91760549445.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=2a36c61503bb036f817ebd881948f0b46c7d1a28)
## Introduction 

IC packages more complex: increase body size & I/O,  application of integrated packages

MCM (multi-chip modules), POP (package on package), CSP (Chip  scale packages),  MCP (Multi-chip packages), SIP (System in  Package) & 2.5D, 3D stacked die package

Wire-bond, flip chip, Cu pillar, WLCSP, FOWLP, Die to Die

![3DieStacked  CSP  "Stacked"  BGA  Flip Chip CSP  FBGA  uBGA  BareDie   ChiP  KGD  Package-on-Package(PoP TMV)  Hybrid  Packages  Multi Chip  Modules (MCM)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d8e7e3c8-7e05-47f6-80c2-16a8de40ca22/d8e7e3c8-7e05-47f6-80c2-16a8de40ca22.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=b0cfdc7324bf9ebac2fdb129d2e0200d7e550601)
ChipScalePackageOverview

6

5

## Introduction 

##   IC packages become complex (Cont.) 

![SYSTEmPIus  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/07d9005d-8193-4bf0-bb22-85cbd8d34b14/07d9005d-8193-4bf0-bb22-85cbd8d34b14.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=01adca6c871d16af627047aec669da7e06017a75)
IBM via-middle TSV process die stacking ( cited: Solid State Technology)

3D IC Pyramid Assembly Die Stacking  (cited: www. palomartechnologies.com

Apple FOWLP PoP packaging (InFO) ( cited: SystemPlus Consulting)

![conndctioris  SKHynixHBM   MicronHMC  AMD Fiji GPU TSV package  AMD Fiji GPU TSV package  TSVs  TSVs       μBumps uBumps  ( cited from Wikimedia Commons) (citedfromWikimediaCommons)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6a627ebc-a2cd-47db-968c-b5ead9b3008b/6a627ebc-a2cd-47db-968c-b5ead9b3008b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=1fb773bb68a82be916ceab5463bbe5f01874ab4f)
7

6

## Introduction 

IC packages moving to Heterogeneous Integration

![SNT  Antenna   Molding  Interconnection   -Passives  -Package integration   -UF  Flip Chip & Wire Bond   -Components  Shielding   for 2.4G/5G/60GHz   -Exposed die  -Connectors  -Board or package level  -Compartmental  Photonics   MemoryDie  Hybrid Flex  Interconnect  Passives/IPD  -lntegrated Passive  Devices  Photonics Layer  MLCC  PIC Chip- optical bus   Mechanical Assy  Embedded Technology   -Laser welding  Wafer Bumping/WLP   -Passive component   -Flex bending  -Lead-free / Cu Pillar   -Active device   Die/Pkg Stacking  -Die thinning   Source:ASEwithad  -Bare die package  -Die interconnect  semi"  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4bb478ff-2e00-4821-9f80-0ef01f345403/4bb478ff-2e00-4821-9f80-0ef01f345403.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=8275f00fa635fd4f7920b5b3816bcee36eab68ff)
## Introduction 

## Package level failure analysis challenges 

Packages “black-boxes”--electrical test data available for PFA      No distinction between defects without opening / removing the  package  either in: 1) package / lead-frame; 2) bond-wires; 3) internal  to the die      Complex IC packages (MCM, POP & 2.5 D/3D Stacked die) & require  Z resolution for fault localization.

![W-EEd  Top-Ctop  (17  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/22983645-a48a-40ac-9221-0ce253984d34/22983645-a48a-40ac-9221-0ce253984d34.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=2051a2c9e6ff08b9e283a8badbe8ff5caaa912bf)
Source Fraunhofer IZM Munich

![Chip on Chip Wafer Chip on Chip Wafer  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1c4d0a91-a47a-4751-b959-5b6798c7a2a7/1c4d0a91-a47a-4751-b959-5b6798c7a2a7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=49716845255d903d9bf367fe087ca991f3071fb6)
Source: Manessis, Ostwald, Fraunhofer IZM,  Advanced pack. July 2008

9

8

## Introduction 

##   What is the definition of package level failure analysis 

In general : except Si die failure analysis, all other components  are considered package level FA.

##   General and common package level failure signatures 

The 1 st   or high level failure reported in the initial product testing     Electrically, open/short/leakage failures     Visually, contamination, chippage/crack/surface damage,   discoloration/burnt mark

## Introduction 

![Visual inspection  Visual inspection  EFA  EFA  Device Verification & Electrical Characterization, Initial FI Device Verification & Electrical Characterization, Initial Fl  Open/short/leakage failure Open/short/leakage failure   Functional failure Functional failure  Si die level (Lab based FI/Debug) Si die level (Lab based Fl/Debug)  Package level fault isolation  Package level fault isolation  ( thermal/photon/probing) thermal/photon/probing  (CSAM, RTX, TDR, thermal imaging) (CSAM, RTX, TDR, thermal imaging)  PFA  PFA  Package or Die Physical Failure Analysis Package or Die Physical Failure Analysis  (X-section, FS/BS delayering, SEM. FIB. EDX etc) X-section, FS/BS delayering, SEM. FIB. EDX etc  Root Cause Determination  Root Cause Determination  Corrective Action Corrective Action  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7c4cf8f5-8d8c-4ece-a01a-6b0654a32bad/7c4cf8f5-8d8c-4ece-a01a-6b0654a32bad.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=d6c789b422e31bb685ede485f2485a1d65cdccb3)
11

## Key package fault isolation techniques 

Tools/Techniques Used for EFA

Electrical characterization (curve tracer/micro probing)     Time Domain Reflectometry (TDR)     Electro-optical Terahertz Pulse Reflectometry (EOTPR)     Real Time X-ray (RTX, 2D & 3D)     Acoustic Scanning Microscope (SAM)     Thermal emission (Thermal Lock-in)     Superconducting Quantum Interference Devices   Microscopy (SQUID)     Space Domain Reflectometry (SDR)

## Key package fault isolation techniques 

Tools/Techniques Used for PFA

Optical Microscope     Secondary Electrical Microscope (SEM) with Energy Dispersive   X-ray (EDX)      Single and Dual Beam Focused Ion Beam (FIB)     High Through Plasma Dual beam FIB      Transmission Electron Microscope (TEM) with EDX & EELs      Auger/XPS/SIMS/AFM/FTIR     Chemical Wet Etch     Parallel Lapping/X-section     Wire Bond/Reball/Chemical or laser Decapsulation

## Brief physics of EFA techniques 

##   Time Domain Reflectometry (TDR) 

A measurement of reflection in an unknown device, relative to

the reflection in a standard impedance.   It is used for isolate Open/Short failures   Basic working principle for fault isolation

![Underfill  C4 bump Si Substrate  Substrate V ss  External pins Reported   TDR  TDR  faulty pin,  probe  probe D0 TDS8000 TDS8000  Digitizing  Digitizing  Oscilloscope Oscilloscope  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/110dc269-d140-48e0-86d1-0ed3b9d1d8e5/110dc269-d140-48e0-86d1-0ed3b9d1d8e5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=50f2f0801ee3e4b1a25edb2637bd39729772e670)
•  A digital sampling oscilloscope with a TDR  module supplies a fast rise time voltage • The oscilloscope records the voltage of  reflections • The time delay between  incident &  reflected signals  analyzed to characterize   electrical path of the signal p in

## Brief physics of EFA techniques 

##   Time Domain Reflectometry (TDR) 

![（A)OpencircuitTerminalZL=oo ineieent  nelecled Sour-0g Cable: Z 。 .Ta  DUT: Z 0UT mination Ruuw=500 20=500  （B)ShortcircuitTerminalZL=0 Then V incdent = % V TDR Open 210000 Impedance 2\*toabe  2\*t cabe  open 1.2号  5012 （C）LineTerminalZL=2Z0 05.2 TDR short Impedance  V  ZL – Z0Shan  reflect reflect ZL - ZO r = —— =     ————V ZL + ZO ZL + Z0      incident](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ebee2c44-33cb-4bef-9d42-715267c9fae4/ebee2c44-33cb-4bef-9d42-715267c9fae4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=58d419c4711e4266f9540e05aa5e759fc2770336)
Basic working principle for fault isolation:

--Impedance change  $\Rightarrow$  amplitude of step --Ratio of reflected to incident (voltage reflection coefficient)

## Brief physics of EFA techniques 

##   TDR Probe Resolution  

![TDR probe with TDR probe with  Cable Cable   signal and ground  signal and ground connections  connections TDR TDR   00  oooooooo  00  00O   Instrument Instrument   ○○  00   00  oooooo0o  oooooooo  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9dd63e11-93ba-4acc-af4e-4654170ffa30/9dd63e11-93ba-4acc-af4e-4654170ffa30.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=5e0878055f0a46e772ddd4b78ade1194a8d56217)
The time or spatial resolution depends on measurement signal rise time. - Typical TDR Rise Time: \~ 35ps   - TDR Resolution: Half the TDR Rise Time (\~17ps)   - Losses in a cable and board affect the effective rise time

## Brief physics of EFA techniques 

TDR Probe Resolution (Cont.)

Current Agilent Probe System:

Spec Bandwidth: 6GHz; Actual Bandwidth: \~4.5GHz (measured)

TDR Instrument Bandwidth: \~ 35ps

Actual Rise Time deliver to DUT:

$$t_{m e a s u r e d}=\sqrt{t_{T D R}^{2}+2\cdot\left(\frac{0.35}{f_{3d B}}\right)^{2}}$$
t meas = \~ 115ps (Large Resolution degradation)

To improve TDR resolution, high bandwidth Probe system  needed.

Rise Time Deliver to DUT: t meas = \~ 37ps (40GHz)

t meas = \~ 43ps (20GHz )

## Case studies with TDR technique 

•  Case 1: Open failure for C4 flip-chip package in C4 bump region

![Continuous  Continuous  Cracks at C4  Cracks at C4   C4 bump open  C4 bump open  Bump  Bump   due to CNW due to CNW  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9eccaec2-8c1f-436f-9e7a-4936bc9d5821/9eccaec2-8c1f-436f-9e7a-4936bc9d5821.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=7d401b95b1ab0be39b24e0f8a067f174bc7ea026)
Impendence for failed unit same as bare substrate

Impendence for failed unit slightly  lower than bare substrate

18

17

## Case  studies with TDR technique 

•  Case 2: Open failure of C4 flip-chip package in substrate

Broken Cu trace in the  Broken Cutracei

![substratepathoffaili  substrate path of failing Pin Ping  Pin   888  AF13  AF13 TDR sh  impeda  near to  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0efe7fe9-396f-4349-91b7-d5d65c2f8f30/0efe7fe9-396f-4349-91b7-d5d65c2f8f30.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=a7382a3a74c61da58f3cfe5e07b915338fc7b055)
TDR shows high  impedance in substrate  near to pin region.

## Case studies with TDR technique 

•  Case 3:  Functional JTAG Vspect failure—Thinner Cu tracer in  substrate

![The TDR curve for the  The TDR curve for the  Bare_Sabstrate  failing curve  failing curve  separates from the  separates from the  curve for good unit  curve for good unit  before the C4  before the C4  interface, suggesting  interface, suggesting  Substrate   C4 bump interface  C4 bump interface failure in package.  failure in package. TDR  Zoom In FIB Result  FIB Result FIB  FIB  direction  FailingtraceBG23  direction  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/edc9bdd5-4efa-4be6-996d-bafe21e165e4/edc9bdd5-4efa-4be6-996d-bafe21e165e4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=8c8112ffd196e9f4990cc77cdcaef980e4c1780b)
Cu trace for the failing pin thinner than the good pin traces.

![ASEGROUP   ASEGroup.Allrightsreserved  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f5fbadb7-cfcc-42b3-ad7b-bb7c5210a0d8/f5fbadb7-cfcc-42b3-ad7b-bb7c5210a0d8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=cb9c3f0e8e205fc3de6c1fcf1d15dbfec42f620f)
20

19

## Case studies with TDR technique 

•  Case 4:  Short failure in C4 bump region

![Dare  9010.0  Failure Failure  vSS  VSS  Bump Bump  AK8 TDR shows low  TDRshowslow  impedance at the  impedance at the  bump region.  bump region. bare  Failure  Failure  Bump,  Bump  AE1 VSS FSS  AGG  TDR shows low impedance at the bump  TDR shows low impedance at the bump  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/729486f6-a7b8-46b4-a8d4-63cfde13f357/729486f6-a7b8-46b4-a8d4-63cfde13f357.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=f417327b9b601f580004af021c90c02d8b4213fc)
## TDR challenge and solution 

Detecting failure mechanism at package level has become  more challenging with shrinking geometry and increasing  complexity of today’s packages (3D-stacking)

Conventional TDR has limit about 500-µm distance-to-defect  accuracy. It can’t provide more accuracy for small geometry  (3D ubump/ TSV) stacking

Electro-optical terahertz pulse reflectometry (EOTPR) for  non-destructive fault isolation with improvement of resolution

## Brief physics of EFA techniques  

Electro-optical terahertz pulse reflectometry (EOTPR)

Basic working principle for fault isolation:

– EOTPR measures impulse response instead of step response  (conventional TDR)

High impedance           positive peak Low impedance           negative peak

![Optical fiber Optical fiber  Emitter   Receiver  Photo conductive  gap in THzemitter  Opticaldelay  Optical delay  Strip-line  Photo  Photo  conductive  conductive  elements  elements 110G  110G  Launch pulses into samplevia  800nm  800nm  HZ  Hz   Receive pulse echoes from faults  strip lineand probe  laser  laser  Probe  Probe  insample  Time delaygivespositionof fault   probe  00do0o  000000  TPI Core system  TPI Core system  000000  DUT  DUT  DUT ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/45cff6e2-8776-41c1-96de-9d8a8ce420d8/45cff6e2-8776-41c1-96de-9d8a8ce420d8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=4330b5b5aa9ad2a04179e246158331550a6c0154)
23

22

## Brief physics of EFA techniques 

Electro-optical terahertz pulse reflectometry (EOTPR)    Resolution test:

–  A high-frequency probe moved 10µm increments           ten  waveforms recorded @ each position.

10 µm shifting in position           clearly reflection resolved.

–  10 µm distance-to-defect accuracy achieved.

![Optical Delay /ps  10 um steps  397.0   397.5  Optical Delay/ps  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/10526dd1-db14-4486-a59b-36bd3b22273d/10526dd1-db14-4486-a59b-36bd3b22273d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=b642d9bdb46d80ce147b0087d20c653cb7984385)
![TeraViewEOTPR-1OumResolutionTest-Waveforms  10 repeated  10 repeated  measurement measurement  s at each  s at each  point pointm  LOO  10pmsteps  395.5   397.0:  3973   3980   398.5   399.0  DpticalDelay/ps  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f6cffc26-cda8-4b2d-aafe-f24b80ef1aa5/f6cffc26-cda8-4b2d-aafe-f24b80ef1aa5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=9b98792517db64265559d4cfbce89e75e737db8e)
## Brief physics of EFA techniques 

Electro-optical terahertz pulse reflectometry (EOTPR)

## Failure location distance calculation:  

–  To get failure location , time-based data               distance data by  calculating the phase velocity, Vp, of the electromagnetic wave. It  can be expressed:

$$v_{p}={\frac{c}{\sqrt{\epsilon_{e f f}}}}$$
Where, Vp, is the phase velocity, C is velocity of light in free space,   ε eff  is the effective dielectric constant of the package

ε eff  is different for different package  estimated using known package  structure locations in EOTPR  waveform.

25

## Case studies with EOTPR technique 

Case 1: To evaluate accuracy of EOTPR for distance-to-defect

A focused ion beam (FIB) to generate defects @ different locations from a  C4 bump pad in 3 samples on a 2D flip-chip package

Physical distance of defects from C4 bump pad is measured

![Bad2  Bd3   Bad4  Sample   Distance A  Bump   Hole   cpm)  Bad2   9.96  Bad3   15.16  Bad4   85.71  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/96d7f02a-c646-40a4-a435-a045b6b16484/96d7f02a-c646-40a4-a435-a045b6b16484.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=7735a89d3f2483865ee6763b570ebe43dff7d9ce)
## Case studies with EOTPR technique 

Case 1: To evaluate accuracy of EOTPR for distance-to-defect (Cont.)

EOTPR waveforms on 3 samples           strong negative curve (short failure  created by FIB)

Measurement on distance to defect matched very well with actual distance  created by FIB

![Bad2  Bad 3.  Bad4  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4a73d644-adbe-4ef0-9ea4-45213e29f323/4a73d644-adbe-4ef0-9ea4-45213e29f323.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=512b71a67e4ba3b002af78d51c25f9697f8940ba)
|Disance|Actuall (pm)|EOTPR (pm)|
|---|---|---|
|Bad 3 - Bad 2|52|54|
|Bad 4- Bad 2|75.0|339|
|Bad 4 -Bad 3|69.8|585|


## Case studies with EOTPR technique 

Case 2:  EOTPR on 2.5D with TSV structure

An open defect created by local mechanical milling on a 2.5D  with TSV structure on  flip-chip package     Open defect location about 18um away from top of interposer   EOTPR clearly separate failed sample with bare interposer   Distance to defect is about 23um only 5um deviation from real  defect

![TSVinterposer  The plots show EOTPR  waveformsfrom the  good interposer and  bad2   231m  ·We find the fault in bad  2to be located23μm  Open failureunit  after the interposer  termination  Distance in DUT  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4b6b26af-1343-411b-b06a-277127436bce/4b6b26af-1343-411b-b06a-277127436bce.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=ae7eadf79f4c8485494b6a4fbc4688364b72c87e)
![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/aa653410-e526-4526-a75b-60f3c9cef4e4/aa653410-e526-4526-a75b-60f3c9cef4e4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=fc90039640e7c60368c2bb8788776e30e806c993)
28

## Case studies with EOTPR technique 

Case 3:  EOTPR for 3D open failure   Open failure reported & confirmed with electrical characterization   Open was located 100μm after bare substrate at the top of C4 or UBM   PFA revealed passivation residue at TSV/C4 pad with 105um distance to  defect (only 5um deviation)

![100Nm  a   Bare substrate  Openin  termination  failedunit  Contact  feature  Interposer  termination  tary E RE3   TSV  TSV  C4  C4  Passivation  Passivation  residue  residue C4bumD  SourcefromYi-Sheng Lin(ASE)etc.,ISTFA 2017  Source from Yi-Sheng Lin  ( ASE) etc.,  ISTFA 2017 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f9c15beb-0279-4eef-84f1-207071851fd1/f9c15beb-0279-4eef-84f1-207071851fd1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=4238e32e90792f8d59b248b07cffc0926186b3d0)
## Case studies with EOTPR technique 

Case 4:  EOTPR for WLP open failure

Open failure was artificially created & distance to defect about 33um   EOTPR results showed 30um open defect distance

![30   30m   Openfailureinunit1  Cut1:Openin  topRDLtrace   top-taca  BGAcontact  PSd  OitascetoDuT/mm  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2d0bccea-45da-417d-a9ef-d2243dc7b2b8/2d0bccea-45da-417d-a9ef-d2243dc7b2b8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=f1bb9c361047470323dd732329ff2d24fd851ee6)
Source from Yi-Sheng Lin  ( ASE) etc.,  ISTFA 2017

![Cut1:Open  in toptrace  TSVUP  Interface  TSM  Bottom  Interface  crack  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f44534e3-cda8-4185-bde0-a3f44b269851/f44534e3-cda8-4185-bde0-a3f44b269851.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=4e6154f3d12a9ebc3e81e9549a00ea086935a18b)
## Brief physics of EFA techniques 

2D & 3D Real Time X-ray (RTX )

![Manipulation/Panning  Iage  Sample  X-Ray  Detector  X-RaySource  Zoom/Magnification  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/087412db-92a2-4f77-9d55-0ca0780da973/087412db-92a2-4f77-9d55-0ca0780da973.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=8475a82915c15c20da9389fcbe56dccebfd29a02)
3D RTX System acquires 2D X-ray images with progressively rotating  sample by 360° at a certain increments. The computerized tomography  (CT) to generate a 3D virtual micro-sectioning

## Brief physics of EFA techniques 

2D & 3D Real Time X-ray (RTX ) spatial resolution

DS5:

Sample

Center

oos:

The high magnification     The high magnification

![The small focal spot & sample size The small focal spot &  Detector   High SNR (signal to noise ratio High SNR (signal to noi  Sourced   Attaining high contrast  Attaining high contrast Spot Size   DetectorPixel Size  meas|  TZ  SS   S   SS  Geo Mag component  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/549ae9b2-099d-4025-a516-f711bfd578d8/549ae9b2-099d-4025-a516-f711bfd578d8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=a63678f5fae3bab7809352a17a6d290ce2e06c08)
## Case studies with 2D/3D RTX technique 

Case 1: Comparison of 2D vs 3D RTX for Flip-chip package

An I-O pin Open failure reported     2D showed failed C4 bump abnormal but can’t determine open failure      3D RTX on failed C4 bump by 360° rotating sample at increments of 1° per   step under 110KV. with15 mins

![protrusion  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2094df0c-696a-4234-86c6-812899b3ad5a/2094df0c-696a-4234-86c6-812899b3ad5a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=20f091a0961fa1ca91191a3949484c6a37cfa1ca)
2D RTX image showing  protrusion of C4 bump

![Defective C4  DefectiveC4   Defective C4 bump   00-00  sanpcatsingogot  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/dd7ae22e-822e-466f-b543-f6d7bd31a933/dd7ae22e-822e-466f-b543-f6d7bd31a933.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=d434a4d22651f2301fe71127bb6833bdd2324000)
Non-contact bump seen in  mechanical cross-section

3D RTX images on the defective C4 bump  (Connect Non-Wetting)

## Source from Lihong Cao ISTFA 2014 

33

## Case studies with 2D/3D RTX technique 

Case 2:  C4 bump cracking inspection through 3DRTX

![Low-volumesolder   Passingsolder  D  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/23eda203-19f8-499e-b206-d16fb4862d35/23eda203-19f8-499e-b206-d16fb4862d35.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=5e120b603feaf21e99aae6655bf1ebdae3b86b43)
Virtual & physical cross section on failing  low-volume and passing C4

Source from Mario Pacheco ISTFA 2008

|Comparison Matrix|Comparison Matrix|Comparison Matrix|
|---|---|---|
|Parameten|Physical XRay CT|Physical XRay CT|
|Analyzedbumps|10-20|60-100|
|Numberofrows||610|
|Xsections/bump||Multiple|
|Time-to-information|3-4h|12h|
|Planeviews|Cannot|Multiple|
|Progressive test?|NO|Yes|


![Crackedjoint   Goodjoint  Virtual  PlanarView  VirtualCross  SectionView  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1a0b7986-59f2-4465-b66c-a9e3b12e1864/1a0b7986-59f2-4465-b66c-a9e3b12e1864.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=b1481572eb58ea12302e4b7d4ba172da29fa3155)
X-ray image comparison between a failing C4 bump (left images) and a passing C4 bump (right  images)

## Case studies with 2D/3D RTX technique 

Case 3:  3D RTX analysis in Multi-Stacked Packages

•  A flash device failed for high Icc leakage and Vcc pin open   •  3D RTX performed under 140Kv with 30 minutes acquisition

![Psnw1  O  SS  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4907d42d-b91d-476b-8c51-9c4bce874a7f/4907d42d-b91d-476b-8c51-9c4bce874a7f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=a4c011022fe810761aca01d87a5b30f7c298b58d)
3D RTX side view

3D RTX top view  image

35

## Case studies with 2D/3D RTX technique 

Case 4:  3D RTX analysis in 2.5D Stacked Packages

•

2.5D ASIC + 2 HBM  SI interposer device short failure Scan on ROI with 1mm/voxel resolution on 1x1x1mm 3   volume (80keV & 4h)

•

![(a)Virtual cross-section   (b)Tsv  (c)C4bumps  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5de61233-f026-40b1-8168-df2beca8119f/5de61233-f026-40b1-8168-df2beca8119f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=19bfc30df89e0df9289158f2ce158045b57dd763)
3D RTX Reconstruction view

Defect can be seen bridging two C4 bump  landing pad at the TSV/C4 i\interface

Source from Bernice , ISTFA 2018

36

## Case studies with 2D/3D technique 

Case 5:  Open/Short failure in Multi-Stacked Packages

![ca  Best2Dx-ray  image  CN  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/02f3f0dd-6bd7-44c8-b29b-e3d84b447ba7/02f3f0dd-6bd7-44c8-b29b-e3d84b447ba7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=54195cfea26fdcfc71172f30a3e1bff3a3b4e40f)
Figure a shows the best 2D x-ray image,  unable to detect the wire break. Figure b  and c show the results obtained with xray CT. The wire breaks are clearly seen  using either virtual cross section (Fig. b)  or 3D model view (Fig.c). Source from Mario Pacheco ISTFA 2008

![a  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0f567d37-13bf-4232-817e-2e518b45376a/0f567d37-13bf-4232-817e-2e518b45376a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=2bd80887a0ce4b95fa9f6505b0f86f4ed14f6a96)
2D x-ray images showing overlapping wire  bonds in dual-stacked package: (a) lateral view,  and (b) top view. Can’t tell failure

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5acbd405-8f45-420a-ab1e-2c0a46c0ba7f/5acbd405-8f45-420a-ab1e-2c0a46c0ba7f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=ed2d48d3fee0de6fdbdd8f17eb7af2db28cdb058)
X-ray CT results: (a) Virtual 3D model clearly showing physical contact between failing wire bonds

## Brief physics of EFA techniques 

## Scanning Acoustic Microscope (SAM) 

## Basic work principle Basicworkprinciple  

![0 Trigger Pulse  1 Trigger Pulse Pulser  Pulser 2 200Volt  200 Volt Spike Pulse  Spike Pulse  Receiver  Receiver  A to D Converter  A to D Converter  8  6 1010111  1010111  Amplified WaveForm  5 Amplified WaveForm  Digital  Digital  Waveforn  Waveform 4  Low Voltage  Low Voltage   Time difference: 125 ns [ = 527 μm]   Gate Pos.: 9000 ns Width: 108 ns 100%  1_0-  RF WaveForm  RF WaveForm Transducer  Transducer  0L5-  0L0-  High Freq HighFrea  Sound Wave SoundWave   -0. 5  Test Specimen  Test Specimen -1_0-  850086008700880089009000910n920n930094ne1  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3e7a1935-1f6c-4928-973e-c955d4374f5b/3e7a1935-1f6c-4928-973e-c955d4374f5b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=6af1933db1684f19301e88d501ecf28bac7c41f2)
1.  A-D initiates sequence & fires pulse with 5 volt trigger                          2. Pulse sends a 200 volt spike pulse to transducer.    3. Transducer’s piezo-electric crystal converts 200 volts  electrical energy into sound    energy   4. Reflected sound returns to low voltage electrical output           5. Receiver amplifies  low voltage signal.            6. A-D converts analog waveform to binary format, computer can process & display.

## Brief physics of EFA techniques  

Scanning Acoustic Microscope (SAM)

–  Two key factors to impact SAM imaging:

•  Transducer frequency------higher frequency, higher  resolution, higher energy loss. •  Focal Length (FL)-------Higher frequency, shorter FL, less  penetration.

–  Fault isolation---Delamination, voids, cracks, poor interface  adhesion

## Brief physics of EFA techniques  

Scanning Acoustic SAM Resolution vs Depth

![117μm  117  m m 1.5  8.5  25  15  No Underfill  No Underfill Focus @ die/water interface  Focus @ die/water interface 8.9   1.5   2.0   3.8   4.5  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8542ed18-0354-4a9c-9df1-74508961dec3/8542ed18-0354-4a9c-9df1-74508961dec3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=4997f4aab2dd478913774128d97524dc7d8c1adf)
Sandia ATC 4.2   $250\upmu\mathrm{m}$   Bump Pitch Test Chip

Source from Thomas M Moore ISTFA 2018

l  = 50 m m @ 180MHz in Si  (no absorption)

D = 1.02  l  /NA for Pulse-Echo  (NA \~ .25 - .50)

Spatial resolution \~100-200 m m  at 180MHz CF

At 400MHz, resolution \~50- 100 m m

## Brief physics of EFA techniques  

Scanning Acoustic Microscope (SAM)

– 1GHz die surface inspection

– 1-2GHz transducers produce micron-scale image resolution  and depth penetration

![200MFL500μm   )400MHz(FL200um)   d）1CHz(FL80m  CINPUT   OUTPUTPTOAMP  TOCRT  PULSEGENERATOR  -TRANSDUCER  A1203  LENS  H20  SURFACE  frequency.resolution  focal length.penetrationdepth  Ultra-high resolutionSAM(GHzsetup)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8a663a99-f954-4c23-a884-bd353bbbd7d8/8a663a99-f954-4c23-a884-bd353bbbd7d8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=206a00cdd5fef49ac92518d7912ddd5750dc5fa3)
Source from Thomas M Moore ISTFA 2018

## Case studies with SAM technique 

Case 1: Short failure in Flip chip package due to thermal runaway

CSAM: Polyimide-UF Interface CSAM:Polyimide-UFInterface

## CSAM: UF-Substrate Interface CSAM: UF-Substrate Interface  

![RT X-ray RT X-ray  Thermal  runaway  signature  Meltedsolderonberved  underX-rayinspoction  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d38e25f6-afbf-4c98-afdf-2851275fd758/d38e25f6-afbf-4c98-afdf-2851275fd758.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=3ace443ed28b44f0086a57b955a73bdc04a2b8ac)
Solder melting  signature was  observed at a corner  under SAM

RT X-ray inspection  also observed melted  solder

Thermal runaway is  cause of short failure

Source from ZY, IPFA 2012

## C ase studies with SAM technique 

Case 2: Micro-delam detection in Automotive parts

C-Scan and A-Scan found minor delam

![MonMr092015  TF   1570  FEGainAB   46.500  GatePos   0152  Gateicthe   0.302  ScanSe   44.09mm  xDucerFreqMhz   30J00  Delam Delam  2（200ngliv)  EMC/Lead finger Delam EMC/Lead finger Delam  QRA.15.0kV8.6mmx25.0kSE（U）  Mechanical X-section Mechanical X-section   DB FIB X-section DBEIBX-section  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3794f638-d2d1-41df-8a81-039d30c3b455/3794f638-d2d1-41df-8a81-039d30c3b455.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=f85de370c3ce0d9c4ac03e624a9fbc0ccc2e9de4)
CSAM with 30MHz  found minor delam

Mechanical X-section  and DB FIB X-section  confirmed micro delam between EMC & lead  finger

Source from  Hyunsoo Kim,  ISTFA 2015

## Case studies with SAM technique 

Case 3: Acoustic & Photoacoustic inspection of TSV in GHz band

![x，y，z-scanningstage  motorizedx-ystage  acousticGHz-lens   forscanningsample  couplant  sample  Laserbeam  LaserSource  Laseroptics  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/70538bf1-c7fa-4d04-bcc6-b9e629df647f/70538bf1-c7fa-4d04-bcc6-b9e629df647f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=82c22b7cdc816427e132d1c1dc613dec80b1f04b)
1. The lens focuses the laser spot  inside the sample.   2. Optical & acoustic lenses are coaligned & synchronized for capturing  the acoustic signals.   3. SAM was operated at 1GHz.    4. Laser with 1064nm wavelength to  generate broadband acoustic signals


Schematics of GHz scanning Photoacoustic Microscope

## Case studies with SAM technique 

Case 3: Acoustic & Photoacoustic inspection of TSV  (Cont.)

TSV with  minor voids in the  upper 2 – 3 μm region.

TSV (right) with void at a depth of  3 – 10 μm

TSV with no defect

DB FIB X-section

## Case studies with SAM technique 

Case 4: GHz Acoustic inspection of 3D Die to Die Bond

![power-ampllier   TRswitch   pre-amplifier   pre-processing  ADC  ultrasonic transdupef  sampie  coupling tluld  PO  SO  N  line-signal  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2ddef77a-f66b-4247-a765-ba74359b91ef/2ddef77a-f66b-4247-a765-ba74359b91ef.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=270adbf84346c6e2d79f8d5f1471a6bfac18d325)
SAM operated @1GHz with FL 80μm &  semi-aperture angle of 50°. Deionized &  degassed water used at  $\scriptstyle{21^{\circ}\mathbb{C}}$    Acoustic lens excited by a tone burst of  20ns length & amplitude of 18 V peak-topeak   GHz-SAM data recorded in V(z) scan  sequences at decreasing distance between  probe tip & sample from 45μm above  sample downward in steps of 1 μm until 5  μm above sample    It ensured the sharpest contour & relevant  subsurface features recorded

Schematics of GHz scanning Photoacoustic Microscope

## Case studies with SAM technique 

Case 4: GHz Acoustic inspection of 3D Die to Die Bond (Cont.)

![vvafer1   Silicon  vvafer 2   Naer2   vvafer  DieA  Schematic pictures of hybrid wafer to wafer bond  nematicpicturesofhybridwafertowaferbond  Silicon  DieB  Daisy chain: We-W./Pitch (nm)   IDie A.   Die B  In-line SAM images (@175 MHz) of die A -line SAM images (@175 MHz) of die A   DC11: 1080-540 /1710 (40% Cu)   BALID  (left) & die B (right) with indication of the  t) & die B (right) with indication of the  DC22: 1620-540 /2340 (48% Cu)   3.10   BL  daisy chains DC11, 22, 30 and 40. sy chains DC11, 22, 30 and 40.  DC30: 2700-900 /5400 (25% Cu)   C.  DC40: 900-900/2250 (16%6 Cu)  Source from  ourcefromIngrid deWolfISTFA2018  Ingrid de Wolf  ISTFA 2018 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/81a1e5af-db19-4a8e-94c9-02f0ce336b0a/81a1e5af-db19-4a8e-94c9-02f0ce336b0a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=a3db615b3b3d877d5b1a51bc7c3dea72734d4af9)
## Case studies with SAM technique 

Case 4: GHz Acoustic inspection of 3D Die to Die Bond (Cont.)

![DieA  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8e1a1370-b33d-40af-a299-eb23f2f68e42/8e1a1370-b33d-40af-a299-eb23f2f68e42.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=9e66551d29a7b2535a48b78fe35e4232d9b7c6b0)
SAM @175 MHz) of die A & die B

|Daisy chain: W-W./Pitch (nm)|Die 4|Iie B|
|---|---|---|
|DC11: 1080-540/1710 (40% Cu)||1B.0|
|DC22: 1620-540 /2340 (48% Cu)|BAO|BAD|
|DC30: 2700-900/5400 (25% Cu)|||
|DC40:900-900/2250 (16% Cu)|OK.||


![ocusdepth  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0999ced1-78c1-422a-bbdf-088fa9b58032/0999ced1-78c1-422a-bbdf-088fa9b58032.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=2c6cc62fefcd3526201fa7c4803dcf8d7602da96)
![DEA  SON  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a92cc464-878e-4e57-a7eb-4740e5f9a45c/a92cc464-878e-4e57-a7eb-4740e5f9a45c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=e5edf3b9de46c9d12b76284c82cef8091ef56784)
GHz SAM Image of daisy chain DC22 for die A  & die B, showing circle-like features at many  positions of defects

GHz SAM Image of daisy chain DC11 for die A & die  B, showing circle-like features at many positions of  defects

Source from   Ingrid de Wolf  ISTFA 2018

## Case studies with SAM technique 

Case 4: GHz Acoustic inspection of 3D Die to Die Bond (Cont.)

![DieA  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3656b3bd-d9fe-40c5-bb31-31c070de38a4/3656b3bd-d9fe-40c5-bb31-31c070de38a4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=903b5246cf49d6d836a94662abc013007cf1cee3)
SAM @175 MHz) of die A & die B

|Daisy chain: W-W./Pitch (nm)|Die 4|Iie B|
|---|---|---|
|DC11: 1080-540/1710 (40% Cu)||1B.0|
|DC22: 1620-540 /2340 (48% Cu)|BAO|BAD|
|DC30: 2700-900/5400 (25% Cu)|||
|DC40:900-900/2250 (16% Cu)|OK.||


![DEA   DIEB  Som  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2f6889d2-0b26-48b1-9020-9396ae0273d8/2f6889d2-0b26-48b1-9020-9396ae0273d8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=972906453f080f9b6988d3e904ddb6e7d6b35d50)
GHz SAM Image of daisy chain DC30 for die A &  die B, showing circle-like features at many  positions of defects, especial at die B

![OEA   DIEB  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/df5e05a2-d3be-4df5-af36-bc9cd49ea241/df5e05a2-d3be-4df5-af36-bc9cd49ea241.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=822d90b26802e3b79ea36733e5674298640fab97)
GHz SAM Image of daisy chain DC30 for die A & die  B, showing no detects

Source from   Ingrid de Wolf  ISTFA 2018

## Case studies with SAM technique 

Case 4: GHz Acoustic inspection of 3D Die to Die Bond (Cont.)

![BUMP  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ebe634ed-c102-434b-afb5-9aa7735557a0/ebe634ed-c102-434b-afb5-9aa7735557a0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=5638c5a9d3f4cbdb646658b97d9bac8e41318c48)
Zoom in GHz SAM Image of daisy chain DC30 for  die B,  1 to 3 Cu to Cu pad  positions

The defect for bump 1&2 at non-bonded  region just about 1um, which is within the  detection limit of  GHz-SAM  Bump 3 only has a small non-bonded  region only about 280nm. This was not  detected in the GHz-SAM and beyond its’  limitation

DBFIB X-section at bumps 1 to 3 as indicated on  the zoomed-Daisy chain DC30

Source from   Ingrid de Wolf  ISTFA 2018

## SAM technique challenge for stacked package 

Higher spatial resolution, less penetration of depth

Stacked dies with mixed interconnect (WB/FC), difficult to penetrate with  acoustics (multiple resonances, high losses)

Potential solution:

-- Improve SAM resolution and penetration through transducer design  and increase high power.

-- Advanced Spectrum analysis methodology-- Inverse Fourier  transform of the log-magnitude Fourier spectrum

-- Combination of Acoustic & Photoacoustic techniques

![PULSERRECEIVER  ELECTRONICS  Extendedpower,bandwidth  and-lownoise  Improved efficiency,  powerand lens shape  (Asphericlensapplications  limiteddue tonarrow  range offocus)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8e552894-9380-4e52-8d54-f79b93cf819a/8e552894-9380-4e52-8d54-f79b93cf819a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=e518ac9ee6fe98554b2c374145cd4c64fced7f73)
Source from Thomas M. Moore  ISTFA 2016

51

## Brief physics of EFA techniques 

## Lock-in Thermal Imaging (LIT) 

Conventional thermal emission techniques (OBIRCH/TIVA/LIVA)  limit for isolating package-level short failure due to vertical Z  resolution     LIT (Thermal Lock-in) as new technique for on-die defect  localization through homogeneous covering package material  with moderate lock-in frequencies (< 25 Hz) yielded sufficient layer  resolution     LIT will provide non-destructive localization and differentiation  through the Package A) only 1 => classification by x,y location B) 1 & 3 possible with differentiation via thermal delay

![surface 一 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1ee5a5df-a9bc-4a62-89b2-5425ef33b811/1ee5a5df-a9bc-4a62-89b2-5425ef33b811.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=7861495c6b36eb166bc221f08bfffa24342797f9)
## Brief physics of EFA techniques 

LIT working principle for package level fault localization

![IR-image (V = off) IR-image (V = off) IR-image (V = on)   IR-image (V = on )  一   "on-images'  “on-images”  –  “off-images” "off-images  detectsYemperatui  detects temperature  differences only  differences only FR  IR  amplitudeimage  Camera Camera   (frame rate (framerate≥100Hz)   ≥100Hz)  xy defect  xy defect  localization  localization t  surface surface  phaseimage  thermal delay  thermal delay - defect depth (z) v ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1c154f13-ccda-42b7-80fc-f83e3bee3acd/1c154f13-ccda-42b7-80fc-f83e3bee3acd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=0f4866c7169ec286506ac8df9cff6be34011c28e)
53

## Brief physics of EFA techniques 

LIT working principle for package level fault loca lization

Comparisonsteady-statevs.Lock-inthermography

![Aagaude  Amplitude: Number of Puriod:30884   400gam   Nunber of Periods: s023  Clobal phgse   100   118+TA   Cobal Phase   140   1:7.7mA  Freqiency   staacy   Frequercy   25  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b1e146d2-a651-4ec6-ab30-f1a56132d5a3/b1e146d2-a651-4ec6-ab30-f1a56132d5a3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=97b8cd47b68f5837dc0fa013bd86c7df5e452829)
Source from Sebastian Brand, ISTFA 2017

54

54 54

## Brief physics of EFA techniques 

LIT working principle for package level fault loca lization

![f=1Hz  f=1Hz ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/87be802d-2bfc-4a8a-93e8-e898104f01a5/87be802d-2bfc-4a8a-93e8-e898104f01a5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=0bc4704870ffc09c9a56a47dfadbb88627768c5b)
![Allmathisappliedtoeverypixelindividually  Incomingimages  andatrealtime-withoutacquisitiontimelimit  opoaraphy  Topography and Results based on same data  noregistrationerror!!  Amplitude:   Phase:  - good spatial resolution   -emissive corrected  -containsemissive   -poorspatialres.  sin(t)   in-phase/o°  "thermal delay”  amplitude image   phase image  -cos(t)  out-of-p   91D  Amp=√（0)  +（90°)2   Φ = arctan90%  Amplitude: ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e9fb624c-598d-4cff-ac20-c9d282297549/e9fb624c-598d-4cff-ac20-c9d282297549.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=ea251c11fc3eca77f5e3f365d9a3aded52d91499)
![f=10Hz  f=10Hz ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b35cda1b-3cd8-4a3f-a737-2ce6fbc8818c/b35cda1b-3cd8-4a3f-a737-2ce6fbc8818c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=d5ecdfd04cdc988fe99d1c1ed7586d4f5d4d02eb)
Amplitude :

A

=

0

( S

)

![f=30Hz  f=30Hz ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4fc87bd4-468a-4183-a8f9-22f882cde41b/4fc87bd4-468a-4183-a8f9-22f882cde41b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=c3496249636075f6e7f00195c6b3fa8daa924b9a)
2

( S

−

90

)

2

Phase

$$\phi=\arctan\left(\frac{-\,S^{-90}}{S^{0}}\right)$$
## Case studies with LIT technique 

Case 1: Homogeneous 3D package structure

–  Homogeneous package structure--- (Die-Attach-Tape--DAT), Molding  compound (MC) & Si die             larger thermal delay.   –  LIT measures phase, φ can be used to calculate depth of defect –  Calculation of defect depth requires precise thermal properties of  material, such information is not readily available

–  Calibration via reference measurement needed

![thermaldelay  mold-comp.   03  simiufation  S   eoperiment  2m  linear dependency!  simulation model  =1H2  8LB  thicknessofmold-compound[mm]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/26857197-28fe-475e-b4ba-c3c64f81df73/26857197-28fe-475e-b4ba-c3c64f81df73.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=a8397597e6383c1d8ffea85fec5ce4fa10211477)
Source from “Rudolf  Schlangen, Shinobu Motegi” at ISTFA 2011

## Case studies with LIT technique 

Case 1: Homogeneous 3D package structure (Cont.)

•  Homogeneous package structure--- Molding compound (MC) & Si die larger  thermal delay. ELITE measures phase, φ can be used to calculate depth of  defect   •  Fully encapsulated SIP with two dies stacked on each other. The failing device  shows a \~13Ω short at one IO pin. Reference heat source ( I/O diode): Upper  die—A;  Lower die—B  die-A;Lowerdie-   10:0

![-fail  -upperdie  lowerdie  mould   upper(ref)  lower(ref)  upperdie   60  Llowerdie   40  multi-layerlead-   20  frame  fiock-in [Hz]   1D  (1) The higher phase shift—defect below lower die  (1) The higher phase shift-defect below lower di  (2) Difference is small— short in the uppermost  (2) Difference is small- short in the uppermost  layer of the lead-frame  layer of the lead-frame simulation model  (3) Confirmation 3D X-ray or PFA. (3) Confirmation 3D X-ray or PFA.  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/474ec3d9-40d1-48c2-815a-15373d7e9eaf/474ec3d9-40d1-48c2-815a-15373d7e9eaf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=d30a876b36239894ff0f945f5caed146ace4f3e6)
Source from “Rudolf Schlangen, Shinobu Motegi” at ISTFA 2011

## Case studies with LIT technique 

Case 2: 3D defect localization based on phase simulation SW –  Stacked memory devices consist of 8 stacked memory dies.

Memory dies bonded in parallel architectures,  IO diodes as reference  heat sources is not applicable     Minimum variation of layer allowed SW to calculate phase values vs.  lock-in frequency for all relevant layers     SW based on 1-dimensional heat spread function, generates a layer  model of including all layers, thicknesses and materials     Fine-tune model by adjusting material parameters to match reference

![350  simulationmodel  measurements  tbadSNR  200   long acquisition time  S50  HONO  (8+1uSDbyToshiba)  fioek-in[Hz]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1c47976a-86d6-43a6-bf7e-f81fac9db239/1c47976a-86d6-43a6-bf7e-f81fac9db239.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=3358ee5a04427128914cb6fefbe874a2423a61df)
![controller  712从m  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3af2cd12-d8d5-4dd3-995f-caee9a5308ff/3af2cd12-d8d5-4dd3-995f-caee9a5308ff.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=18beef7293259b0cd448cf77a7d4cfd4f8791a70)
Source from “Rudolf Schlangen, Shinobu Motegi” at

ISTFA 201 8

## Case studies with LIT technique 

Case 3: 3D defect localization step by step

## –  2 stacked dies with wire bond structure 

![HotSpot   HotSpot  HotSpot  1stinvestigation:   2ndInvestigation:   3rdinvestigation:  Hotspotlocalized   Mouldremoved   disconnectedbondwireof  withinICarea   →localspot,but   upperic  whichIClevel?   hotspotstillpresent  →defectatlowerIC  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c9eafb18-3feb-4e3e-895b-6728370a7c21/c9eafb18-3feb-4e3e-895b-6728370a7c21.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=ee89ab854de1a5b0875f132ec68b0881e4f212fe)
Source from Sebastian Brand, ISTFA 2017

59

## Case studies with LIT technique 

Case 4: 3D defect localization by using higher Lock-In Frequency

![iopDie  Gluel  Bottom Die  Glue  Substrate  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/916cc07e-593f-4c33-aba1-590f9f040755/916cc07e-593f-4c33-aba1-590f9f040755.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=fb641383086aa5af8d8e863e10b54b7270930637)
![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9a5b33c9-668d-4eef-8eb1-68462efecdcd/9a5b33c9-668d-4eef-8eb1-68462efecdcd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=3e3f2c79f1cd7bbf64767517659e66f9c8d03b39)
Phase shift image of the lock-in  frequency at (A) 0.1Hz, (B) 0.3 Hz,  (C) 0.5 Hz, (D) 1 Hz, (E) 2 Hz, (F) 4  Hz, (G) 5Hz, (H) 6 Hz, and (I) 7 Hz.

Amplitude image of the lock-in frequency  at (A) 0.1 Hz, (B) 1 Hz, (C) 2 Hz, (D) 4 Hz,  (E) 6 Hz, (F) 7 Hz, (G) 8 Hz,(H) 10 Hz, and  (I) 12 Hz.

## Case studies with LIT technique 

Case 4: 3D defect localization by using higher Lock-In Frequency

![BonomD  Substrate  Overlaid phase shift  Overlaid phase shift  and amplitude  and amplitude  image of at (A) 0.5  image of at (A) 0.5  Hz, (B) 5 Hz, (C) 8 Hz,  Hz, (B) 5 Hz, (C) 8 Hz,  and (D) 12 Hz.  and (D) 12 Hz. ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/45100c23-a64a-475c-9bbc-9f1d5f30abf6/45100c23-a64a-475c-9bbc-9f1d5f30abf6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=3e82853aaf34522b9fc846d4a3f9e7bd17b74252)
![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fbb11e42-5e56-46e1-b5b2-e231f7e90724/fbb11e42-5e56-46e1-b5b2-e231f7e90724.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=94d0d85722fdb650e914c2b987f876e40b6fe57d)
Overlaid optical image with the X-ray  image; LIT spot location in the substrate  layout, as shown by a black

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/006438a3-44a9-4e9e-a6a1-d9074dc22c47/006438a3-44a9-4e9e-a6a1-d9074dc22c47.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=aaec10369c6ed6e95317bbadf8f036e8e13deeca)
Source from Ke Ying Lin, ISTFA 2018

Defect between two  Cu traces in the  substrate. Anomaly  particle ( C based)  causing leakage

![mt  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/32740992-c780-4214-b9ce-e218dbf78e29/32740992-c780-4214-b9ce-e218dbf78e29.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=87c6ca78046d1dc91b9dc12202837ad0425310d7)
61

## Case studies with LIT technique 

Case 5: Inhomogeneous package structure

–Inhomogeneity of flip chip structure---Pb-free C4 bumps, Cu conductors in  organic substrate & Si Die           smaller thermal delay

– Special sample preparation to set up reference  for relevant layers

• Parallel polishing with \~10° tilt

• Probing needles from backside to generate hot spots

• LIT measures thermal delay

cleardifferentiationofsurface-nearlayers& exactmatchbetweenresultsandtheory forLiTfrequencies>100Hz

![Si-die   80   PCBM2  PCBM1  bun  ys  in-C4-ball  substrate  20  dieUBM  90  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/18898030-6a05-44af-b923-bfedd76caa8d/18898030-6a05-44af-b923-bfedd76caa8d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=ec5eef6ffce15d1a1889636b9b53eef47b4a1837)
## Case studies with LIT technique 

Case 5: 2D package C4 bump short failure isolated by LIT

•  A sample with I/O short failure. Curve trace confirmed a leaky I-V  curve   •  Acoustic scanning microscopy (CSAM) didn’t reveal silicon die-level  delamination

![Anode Current (A)   pincontshort  0.1-   ++ ++ +  01  0.1  0.0  0.0..........  00  -0.0-  50.0  0.1   Lepend  Good  01  AnodeVotage (V)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4a22c88f-ae98-4c6b-bae5-39f3c55c133c/4a22c88f-ae98-4c6b-bae5-39f3c55c133c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=180fc4ecff1d2e648d7276d265074b86a35d4e5d)
I-V curve   results

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/101ae6b3-209e-42f3-ac8a-188f9d673f04/101ae6b3-209e-42f3-ac8a-188f9d673f04.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=aee337876bf62454bc354fa7e02b5f48960652fd)
CSAM results

63

## Case studies with LIT technique 

Case 5: 2D package C4 bump short failure isolated by LIT(cont.)

•  LIT with10x lens & 256x256 pixels, two potential defect sites appeared  within 15 mins

• At 0.5 Hz lock-in frequency, phase delay observed at point 1 (20.217º)  &  point 2 (23.965º)

• Compared to reference, hot spot 1 at C4 bump level & hot spot 2 at  organic substrate interface in the package

![Filament Shont  PCBI  inC41  dieuB  lochequincy ]  Si ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fee2029a-04e0-4b49-aa9c-d14747489e01/fee2029a-04e0-4b49-aa9c-d14747489e01.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=ff40c576ea9b08f41479a23abeac0045e5f1caa9)
LIT thermal emission and phase results at 0.5Hz

## Case studies with LIT technique 

Case 5: 2D package C4 bump short failure isolated by LIT ( Cont.)

•  Real-time x-ray revealed solder filament short between failed memory  bump & VSS @ hot spot 1   •  CSAM revealed C4 to substrate interface delamination   $@$   hot spot 2 •  Failure signatures consisted with LIT results

![Filament-short  MA DATAH14]  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0a867dbe-81c8-42ba-aeef-195cdc566966/0a867dbe-81c8-42ba-aeef-195cdc566966.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=e7e52a957449986f61745bbd0041dc910e3aabb0)
Real-time x-ray result   $@$   hot spot 1.

![Si ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ff788bcd-1360-4b04-ba92-e777f8956284/ff788bcd-1360-4b04-ba92-e777f8956284.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=fac5e0e6f247e658f91ca8032348e4e561a8ce2a)
CSAM result @ hot spot 2.

65

## Case studies with LIT technique 

Case 6: 2.5D package power supply short failure

•  LIT measures thermal delay at the relevant layers

![ASICDe   (a)Die Diode   Solid Line-Reference   Substrate  Dots-Experimental Data  2uhumpshert  Interposer   Interposer  13j c Bump shon  Substrate  ubsrmsi  Lock-tn Freusney [t)  SEMimage  ASKCDie  ubump  Sn  Interposes  spectedsolder  C4bump   materiai shocting the  faluesipralpin  Source from Bernice at ISTFA 2018 atISTEA2018   Solder short in C4 substrate interface SoldershortinC4substrateinterface  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2602fc05-83fc-41bb-85f7-cb907241c083/2602fc05-83fc-41bb-85f7-cb907241c083.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=b11153638836639ac17d816ddf83904d7918a13d)
Rernice

## Case studies with LIT technique 

Case 7: 3D TSV stacked HBM short failure isolated by LIT   • TSV test structure with electrical short between two isolated TSV stacks

![TSVs  WldeDataPath  DRAM  LogicChip  Case 6--Focused  Phase   RO1of9x9Pixel   Topography  S  TSV3  Si ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d8d0fc7a-35fa-424f-9b45-79ee750b512e/d8d0fc7a-35fa-424f-9b45-79ee750b512e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=816839d7fad252209a5e8d5a0886734708df81da)
Source from Altmann  ISTFA 2015

## Case studies with LIT technique 

Case 8: 3D TSV stacked HBM short failure isolated by LIT (Cont.)

• LIT isolated short failure at 2 nd   stacked die & DBFIB confirmed TSV  sidewall damage

![LIT at metallographic cross section  ProberneedlesonPtpads  Si-substrat  Si-substrate Diffuse signal in   Cu-TSV  Cu-TSV layerbetweendles  TSV isolation  TSV isolation hotspotatTSV  Defect size: 100nm  Defect size: 100nm ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/71544607-fe33-43ff-a356-2f9c6ce7c2e8/71544607-fe33-43ff-a356-2f9c6ce7c2e8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=f4bb5febc48c5a61c776532cbc479a3baf577a52)
Uncovered metallographic  cross section

2nd measurement after  black painting

DB FIB cross sectioning

Si

Source from Altmann et. al. ISTFA 2015

## Brief physics of EFA techniques 

## SQUID (Superconducting Quantum Interference Devices 

Magnetic current imaging: Mainly used for shorts, resistive  opens Current passed through a layer in the package and a  magnetic field is produced.     Magnetic sensor is scanned in close proximity to sample to  detect magnetic field.     Acquired magnetic field info. converted to current density info.     High current density, abnormal current paths, decaying current  indicated defect location (Active dimension: \~ 30 um; Peak  resolution: +/- 3 um

![Sensor  Current Density Signal  Magnetic Field  Package  Substrate  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5f9e4d6d-b8b3-49ff-966c-8c0c3a972975/5f9e4d6d-b8b3-49ff-966c-8c0c3a972975.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=1ce50ac244cc48326e00d1f12b9033f2a1b7e2dc)
![Magnetic Field  Magnetic Field   Current density  Current density   Data to Optical  Data to Optical  Data  Data  image  image  imageoverlay  image overlay Magnetic  Magnetic  Field  Field  conversion conversion  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/964fba77-8640-42df-bdf9-9b06e2821093/964fba77-8640-42df-bdf9-9b06e2821093.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=18cd2ac120d319c06d0da705966776f680941d46)
Source by David Vallett, ISTFA 2016

## Brief physics of EFA techniques 

## SQUID (Superconducting Quantum Interference Devices)  

Magnetic field pass through Si chip, package & PCB material  unperturbed. A signal injected to DUT ( DC or few kHz AC for  short, RF up to 100MHz for open)

No thermal conductivity absorption & refraction

MCI requires only a small sufficient current such that avoids  subtle defect damage by excessive voltage, current and heat

![Thermal  Photonic(inbound)   e-beam/ionbeam  Magnetic  Photonic  (outbound)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6c99f9a5-80d9-4260-9a74-d62f6dab71cf/6c99f9a5-80d9-4260-9a74-d62f6dab71cf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=55c97317589fb1c98f87544c1da4a32d6b56c858)
|A|1.000022|
|---|---|
|Si|0.999996|
|C|0.999990|
||1.000068|
|Pb|0.999982|


Source by David Vallett, ISTFA 2017

## Brief physics of EFA techniques 

SQUID (Superconducting Quantum Interference Devices)

Short Circuit Signatures :

--- Current density image varies with relative width of source and sink paths:

![150  0716 NSVTM  1150749.1  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/57888aba-bd00-4d6f-82ea-abed9451ce04/57888aba-bd00-4d6f-82ea-abed9451ce04.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=d7ffb7c434cfe2d8ea37f811bf1affb8408e32ac)
Source by David Vallett, ISTFA 2017

71

## Case studies with SQUID technique 

Case 1: 2.5D Si interposer with 2 HBM short failure

![Optical Image     MFI (magnetic field)    CDI (current density image) Optical Image   MFI (magnetic field)   CDI (current density image  SOUID  sensor  Pobe  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/aff68923-f5c2-4b29-8ae5-c06e8d52fd4f/aff68923-f5c2-4b29-8ae5-c06e8d52fd4f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=a685dbf536b7b5fed6da74d629e77cedbb0078ea)
High resolution CDI by focus on ROI

Source by David Vallett, ISTFA 2018

## Case studies with SQUID technique 

Case 1: 2.5D Si interposer with 2 HBM short failure ( Cont.)

![C3  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ad909db3-0f86-45b5-86e4-de4fdbdf1283/ad909db3-0f86-45b5-86e4-de4fdbdf1283.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=a0a4d2260155c57f52b2084b994af91c07e8b6c5)
(a): 3D current path obtained by  3D solver (mm)  (b): Top view of the 3D path.

![soher   SOURD  locaton   △z-63μm  ASC  sberposes  CDup  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/289ed184-3787-4e7e-9d8e-86475a28dd6c/289ed184-3787-4e7e-9d8e-86475a28dd6c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=937fcc7a2d1c1ad2c5e95d569f4726fcafc489e9)
XY  location determined by further focus on ROI Z location by using 3D solver to modify current  path in three dimensions to fit to magnetic field 3 Critical distance to sensor o btained.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/24eec3e4-f658-4501-a5b6-b60a220ae5fe/24eec3e4-f658-4501-a5b6-b60a220ae5fe.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=ab79f90a4d9bc057c4d9d70664f7ece7ef1baae9)
3D solver provides 1193um relative to sensor while  1130um actual physical location by 3D XRM   $(\triangle_{\bf z=63u m})$

73

## Case studies with SQUID technique 

Case 2: Power supplier short in Flip chip packag e

![Tilted  Tilted   Top view  Top view view  view Fine solder bridging Fine solder bridging  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3aaf8ab0-7f98-4001-8baa-e0a31ff4b081/3aaf8ab0-7f98-4001-8baa-e0a31ff4b081.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=7765e9b5ab40e6fbacf24f2ff1c1cae07fdaaadd)
Fine solder bridging can be observed between Vdd bump and Vss bump at the die  corner, where a strong current path was detected by SQUID analysis

74

## Case studies with SQUID technique 

Case 3: Power supplier short in wire bond package

BGA292 (Good)

BGA292 (PS Short)

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f6d85ab9-ab73-46d0-a9f5-d81cce962fe9/f6d85ab9-ab73-46d0-a9f5-d81cce962fe9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=59b12949015fb0bba24dc751b18b5aa7701594e2)
![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/dd14f6eb-72f3-497c-a668-57af2a7cfb3a/dd14f6eb-72f3-497c-a668-57af2a7cfb3a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=6593257bb74fc0f8658e9148c1f180fd5c360afa)
The current path on the  failed unit seen to short at the left-up corner and outside the die

![Ground  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2cdd814f-ea2a-4d12-a0c4-e9ff7ac9dfa5/2cdd814f-ea2a-4d12-a0c4-e9ff7ac9dfa5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=57ab20e800f1ab96bbaa5ef78ecdd4ec5571d90e)
RTX zoomed in the suspected short location in finding  that the wire of Vcc touches the lead frame of Vss.

## Brief physics of EFA techniques 

## Space Domain Reflectometry (SDR) 

SDR--A new approach for isolation of open based on mapping  radio-frequency (RF) magnetic field produced by failed device     It employs a SQUID by increasing bandwidth into RF range to  find open in packages or die     It provides 2D failure isolation capability with resolution  about 50 microns   For Open circuit     Under DC & low frequency,  no current flow.     Under RF frequency,  magnetic field will vanish  or significantly change in  amplitude and phase near  open location

![pin A   pin B  51  Z\~5052  ground plane  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/04a41ab1-25b4-44fa-b836-b38b24205985/04a41ab1-25b4-44fa-b836-b38b24205985.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=dfefb07790718c59d98e4ea89fdd21f131bb4c9c)
76

## Brief physics of EFA techniques 

Space Domain Reflectometry (SDR)

![open boundary  incident+reflected  incidtn  refected   transimitted=0  siandingwave  curent amglitude  posascn  signalconcucto  ground conductor   insuiator  feed-anc   qroand-ponb  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0ce0016a-1927-418c-869d-9cbc3d41f0ea/0ce0016a-1927-418c-869d-9cbc3d41f0ea.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=b374d155b17527d49cf4178a09add33cbb2a421a)
![SOUD   computer  RFelectronics   control  vacuum  SQUIDsensor  chamber  traceunder   (inside vacuum  w/cryocooler  stuidy   chamber)  de  coax cable   package  z.stage   BGA  XY-stage  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1774b8c4-33a8-414d-a5db-29e06e373bef/1774b8c4-33a8-414d-a5db-29e06e373bef.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=d476092d41ab2e7a66065368cccb88d656fe7e64)
For Open Trace location: The amplitude of a  standing wave current I  along trace can be found as  follows:

$$I=2\sqrt{\frac{P}{Z_{0}}}\sin(\gamma x)\simeq\sqrt{\frac{P}{Z_{0}}}\gamma x\propto\sqrt{P}\omega x$$
where P ---power of  RF -- effective dielectric constant X--position along the trace.

Source from “Mayue Xie”  at ISTFA 2012

## Brief physics of EFA techniques 

Space Domain Reflectometry (SDR)

RF signal decay is effectively linear at the open

![RFmagnetic  fieldorcurrent  SQUID tip(inside  vacuumchamber)  z(a.u.)  defectivetrace  signalwire  insulator  groundwire  ground-plane(optional)  RF/microwavefeed-line  ohmical  connection  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/48b7e1cf-8ce6-4945-8520-2b2971ad50a4/48b7e1cf-8ce6-4945-8520-2b2971ad50a4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=cc141fd369a86d48bb989e08e8a95cbd4815af8a)
78

## Brief physics of EFA techniques 

Space Domain Reflectometry (SDR)

SDR linear decay model

![320E+2  3.00E+2-  2.80E-2-   standing-waveRFcurrent  260E-2-  2.40E+2-  220E-2-  linearfit  2.00E+2-  180E-2-  160E-2-  140E-2-  120E-2-  00E·2-  8:00E  600E-1-  400E-1-   opensation  200E-1-   (currentnou)   noisefloor  0.00E-0-  1000  2000   3000   50006000   7000   800  position(um)  Source by David Vallett, ISTFA 2017 SourcebyDavidVallett.ISTFA2017  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/076653b1-6150-47b3-9a9b-fef110528fc9/076653b1-6150-47b3-9a9b-fef110528fc9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=a165a3bc456317f99dc7239e6531e29d6d2ec4cc)
79

## Case studies with SDR technique 

Case 1: Fine trace to tracer open in TV

![Case 6--Focused  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0b982fbf-87b8-422c-8385-238a34f9877d/0b982fbf-87b8-422c-8385-238a34f9877d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215622%3B1743219222&q-key-time=1743215622%3B1743219222&q-header-list=host&q-url-param-list=&q-signature=cef1296faef6a21e37f3cc6e3c752370414b8c5d)
Case 2:  Package with a trace cracking after reliability testing

![Suspectlocation  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/da6324c5-095e-47bf-8228-63d3091c4b13/da6324c5-095e-47bf-8228-63d3091c4b13.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215623%3B1743219223&q-key-time=1743215623%3B1743219223&q-header-list=host&q-url-param-list=&q-signature=6f660986218f35d2041322efd39030d885569667)
Si

Source from “Mayue Xie”  at ISTFA 2012

## Case studies with SDR technique 

Case 3: Broken Copper Trace in Substrate

![32-2  3:00E-2  standing-waveRFcurrent  2B0E-2  250E-2  24  ne  220-2  200E-2   Iinearfit  1BC-2  140-2  120E-2  100-2  500C-1  4-00E-1   openlocation  200E-1   (currentnode)   nolsefloor  10002000   32G0F   4000   5005  position（um)  Si ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ae48b843-d860-4693-8486-969ca2b12e63/ae48b843-d860-4693-8486-969ca2b12e63.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215623%3B1743219223&q-key-time=1743215623%3B1743219223&q-header-list=host&q-url-param-list=&q-signature=7c717f71a9a3c1effac46a2e89e8ca3b660b19b4)
81

## Case studies with SDR technique 

Case 4: Open failure in die region

![Lineardecayanalysis  Linear  decayanalysisoncurrent   Openlocationprojected  10-1  4.40+3   densityimage   ontooptical image  30年+2  20+  20+2  EE+2-   open  140C+1   location  S4O+E  OEOC-O  SOC+E  150100012509  Si ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/00c4b9b6-7d76-448d-a0ca-c3a41dbf7bc0/00c4b9b6-7d76-448d-a0ca-c3a41dbf7bc0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215623%3B1743219223&q-key-time=1743215623%3B1743219223&q-header-list=host&q-url-param-list=&q-signature=9c3e355d03282dd018f4561a441da020c81f02bd)
## Summary 

##   Package level Fault Isolation Today 

TDR, SDR and EOTPR have become effectively techniques  for open/resistive open failure for 2D and 3D packages

LIT and SQUID are critical techniques for short/leakage  failure, especial for 3D packages

Package level Fault Isolation Future Challenges

SAM developments (time domain analysis, transducer  development, higher power pulses) as well combination of  Acoustic & Photoacoustic techniques for 3D package FI     3D RTX is required with sufficient resolution (X, Y, Z)  throughput for production support     Improved spatial & vertical resolution for LIT, SDR & SQUID  to meet package small geometries and stacked structures is  very critical. Separation of deep & parallel paths is  challenging

## Thank You for Your Attention  

84

