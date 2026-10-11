---
title: "tut-1.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_f335a0a9cc62fdb6ce6470dbac66edbb7295230462135641
file_size: 6398842
---

## Three decades of IC-Probing Technology: The Great Loop from E-beam Methods to  Optical Methods and back to E-beam Methods 

James S. Vickers Thermo Fisher Scientific

## Tutorial Objective 

Learn how EFA problems have been solved over the past 40 years

Learn reasons for the recent resurgence of e-beam probing

Learn how e-beam probing works

Is Optical or e-Beam Probing Right for Your Lab?

## Outline 

Why is EFA Important     IDS5000: The First E-Beam Prober (1987 until late 1990s)     Optical EFA Tools (In use since mid 1990s)     Second-Generation E-Beam Probers (2020 until ?)     Voltage Contrast: The Mechanism of E-Beam Probing   Secondary Electron Energy Discriminator   Spectrometer Constant: Practical measure of VC sensitivity   Numerous affects that masquerade as VC, but are not   Voltage contrast in action: Barber poles and “CW” waveform  acquisition   Stroboscopic pulsed-electron method for waveform, spectral, and  frequency mapping of modern ICs

Conclusions

![MICRODEVICES  Physics and Fabrication Technologies  ELECTRON  BEAM  TESTING  TECHNOLOGY  Edited by  JOHN T.L.THONG  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/72fe119c-ea29-437d-a4d9-b4e962559ac6/72fe119c-ea29-437d-a4d9-b4e962559ac6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=5cb28e8e23099a44f95dd00a2823d2aa6a2f660d)
## Why is EFA Important? 

Static Measurements: Answers as-designed  vs . as-built issues   Contact Resistance, Opens/Shorts, Transistor Drive Strength, etc.

Dynamic Measurements: Answers at-speed issues   Why does   $1+1=3$   at high speed, or at high temperature, or … .

With 100B transistors on an IC, sometimes probing is required to learn  the root cause of a timing problem

Early Debug probed large transistors on ICs with needles, but…

![APRIL30.1987  Electronics  ANEWTOOL  DRAMATICALLY  CUTS VLSI  DEBUGGING  TIME  PAGE51  SENTRY TESTER  IS FIRST  TO DRIVE  E-BEAMPROBE  WITH CAD  DATA BASE  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ba77d203-2ae9-47fb-b428-5e6a374c9426/ba77d203-2ae9-47fb-b428-5e6a374c9426.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=865041f5d153a930a6851205761bd0867a55a3fc)
## E-Beam Probing   - First Round 

## IDS5k and IDS10k E-Beam Systems 

| Preceded by:|Physical needle probes/cards|
|---|---|
|■ Pros:||
|■ Pros:|CAD-NAV to identify nodes on IC, 0.18-μn|
|■ Pros:|E-Beam waveform probing up to 8 GHz|
|■ cons:|In vacuum operation|
|Why Replaced:|Introduction of Flip-Chip Technology|
|· Replaced by:||
||Optical Probing (LVP IDS2000, 2500, etc.)|


## Pulsed Optical Probing (Generalized) 

Thru-Silicon probing Pulsed Laser focused on  DUT Modulated DUT reflection  sent to photodetector Waveform is captured

![ElectricalSignal  ave100.0MHz  GNO   DD  SO  Objective   digital  digital Lens   TRIGGER TRIGGER  scope  scope Incoming   sssss  Laser  Modulated  Signal  Returning  signal  photo-  photoBeam   amplifier  amplifier Splltter   detector  detector Pulsed  Pulsed Laser  Source  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0ba1f470-1c74-4493-b9ce-c5eb1fe86b43/0ba1f470-1c74-4493-b9ce-c5eb1fe86b43.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=55be37ff5bf54eff8dc32e1745e558e543b4bf77)
Pulsed Laser Probing:   IDS2000, IDS2500, SMLL,  TDP, PDP, etc.

## IDS2000, IDS2500, SMLL, TDP, PDP Systems 

|· Preceded by:|E-beam front-side probing|
|---|---|
|■ Pros:|        LSM (0.18-μm) + CAD-NAV to identify IC nodes                Thru-backside-Silicon access to entire DUT      |
|||
|■ Cons:|        Complex Mode-Locked Laser, Invasive, DUT                Thinning / Sample Prep      |
|Why Replaced:|Simpler Non-Invasive Dynamic Emission|
|· Replaced by:|PlCA/ EmiScope Time-Resolved Emission|


## Time-Resolved Emission (1998 – 2008) 

Overall Principle:

Switching transistors emit picosecond flashes, Microscope images DUT to detector, Single-photon detectors capture light.

IBM Picosecond Imaging Circuit Analysis (PICA)   Created movies showing circuit activity at picosecond resolution   Very low QE (< 0.1%) imaging detector

Optonics EmiScope (Emission OscilloScope)   High-QE (50%) single-point detector

## Time-Resolved Emission Systems 

|· Preceded by:|Pulsed Laser Probing|
|---|---|
|■ Pros:|LSM with SIL (0.12-μm)|
||        CAD-NAV to identify IC nodes                Non-lnvasive, Simple Ease-of-Use      |
|||
|■ cons:|        Emission Signal drops precipitously as Vcc drop                Thinning / Sample Prep      |
| Why Replaced:|Impractical below Vcc = 1.5V|
|· Replaced by:|Pulsed Optical Probing (Ruby)|


## Pulsed Optical Probing (Ruby) 

Improvement over earlier  optical probing tools:

Phase-Locked Loop  synchronized MLL pulses  to the tester loop Up to 10x Faster

![Electrical Signal  vave100i.0MHz  GND   VD  510  Objective   digital  digital Lens   TRIGGER TRIGGER  scope  scope Incoming   sssss  Laser  Modulated  Signal  Returning  Signal  photo-  photoBeam   amplifier  amplifier Splltter   detector  detector Pulsed  Pulsed Laser  Source  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9cc64479-b380-491b-aa81-91284cb8af6c/9cc64479-b380-491b-aa81-91284cb8af6c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=e8715db4ed77d2b3037a6876b0e51064d07536e8)
LVP Mechanism is linear in  DUT voltage, whereas TRE  signal vanishes below 1.5V

## Pulsed Optical Probing (Ruby) 

| Preceded by:|Time-Resolved Emission (PICA, EmiScope)|
|---|---|
|■ Pros:|LSM with SIL (45 and 90-nm)|
||        CAD-NAV to identify IC nodes                Easily captures low-voltage waveforms      |
|||
|■ Cons:|Overdesigned: customers claimed to want >|
|Why Replaced:|        Telecom High-Speed Photodiodes (6 to 8 GH                became available; turned out 6 GHz was Ok      |
|· Replaced by:|Continuous-Wave (CW) Laser Voltage Probe|


## CW Laser Voltage Probing (LVP) 

Ruby: High-speed laser (ps pulses) with low-speed  detector (100 kHz bandwidth)

![ElectricalSignal  Aave100.0MHz  GND   DD  SO  Objective   digital  digital Lens   TRIGGER TRIGGER  scope  scope Incoming   ssss  Laser  Modulated  Signal  Returning  Signal   8GHz  8 GHz Beam   photo-  photo-  amplifier  amplifier Splltter  detector  detector Laser  Source  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/02987359-463a-49ce-a153-b1bf0b349df9/02987359-463a-49ce-a153-b1bf0b349df9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=d116468cd8f1c0fbd0566ad1a5b0e86651e8293c)
LVP: Low-speed laser (CW)  with high-speed detector      (8 GHz)

Ruby complexity replaced  with LVP simplicity

## Optical Laser Voltage Imaging (LVI) 

![ElectricalSignal  LVI image @ target  LVI image @ target  GNO   wDD   target frequency  target frequency  frequency  frequency SPAN  1.000kH2  SIO  Objective  Lens  Spectrum  Spectrum  Analyzer  Analyzer  LSM image  LSM image AC  AC Incoming   ssssss  Laser  Modulated  Signal  Returning  Signal   8 GHz  8 GHz  Amp/  Amp /  Beam   photo-  photoSplltter    splitter  splitter  DC detector  detector Laser  Source  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a5951333-575c-471b-b317-ece82a13e34f/a5951333-575c-471b-b317-ece82a13e34f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=83342fbe9feb2044b88822966720d01534eab663)
Search DUT image for  electrical activity at a  specific (e.g. clock)  frequency

Overlay LVI image  with LSM Image  proves useful for  signal location and  navigation

## CW LVP and LVI

| Preceded by:|Pulsed Optical Probing (Ruby System)|
|---|---|
|■Pros:|        Simplicity of System Design                LSM with improved SIL (      |


Why Bother Using a Scanning Electron Microscope?

## SEMs Extend Resolution of Optical Microscopy By Over Three Orders of Magnitude 

![Transistor  GateLength  Mcro   Atom  Processor   Bacteria  Hand  virus  DNA  Strandof  Fingerprint  Ohiid  ELECTRON MICROSCOPE  LIGHTMICROSCOPE  HUMANEYE  10cm   1cm   1mm   100pm   10m   1m   100nm   10nm   1nm   1A  1   10-m   10-2m   10-m   10-m   10-m   10-6m   10-7m   10-m   10-9m   10-10m  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8ed2b602-8be1-4c5c-8fac-990ffec8ed9c/8ed2b602-8be1-4c5c-8fac-990ffec8ed9c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=243e911d20d92a2e17a1d0c5beed884d251593d2)
SEMS Enable You To Learn About Tiny Things You May Not Want To Know About…

![ca.50.um  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a99d4210-70dd-49bb-bbca-c8f8fc927c2a/a99d4210-70dd-49bb-bbca-c8f8fc927c2a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=58c9ac6a1672f2fb406d13fd4041ba0f2988f8ec)
Philippe Crassous / FEI Company

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1f529bdd-7c3e-478e-899c-4bdf8967de5e/1f529bdd-7c3e-478e-899c-4bdf8967de5e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=dfbf444eb2547eca55b1dc24c21923ff6bd08a2d)
Louisa Howard / Dartmouth SEM Facility

## …As Well As Things You Want To Know About: SARS-CoV-2 

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4b5843c1-4c01-4a4c-93f8-96a66eec94d0/4b5843c1-4c01-4a4c-93f8-96a66eec94d0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=578a3a9851eb9ca4411628ac1cf9f0051f8ae2b5)
The high-resolution graphic of  SARS-CoV-2 seen on the Centers  for Disease Control and Prevention's  website is partially artistic — but the  red "spikes" seen on the virus's grey  body were created using an electron  microscope.

## 22-nm Tri-Gate Transistor 

![Gates   Fins  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2150fa94-9450-4e86-824b-235cb8a42653/2150fa94-9450-4e86-824b-235cb8a42653.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=2dc0c09f0918eca58c3553c94299e7e1588a2a98)
Intel, 2011

How Does a Scanning Electron Microscope Work?

![Electron   Schematic Diagram: Schematic Diagram:  source   SEM Column  SEM Column Anode  Scan generator  Condensor  lenses  Amplifier  x,y scancoils  Objective  Iens:  Back-scattered  electron detector  x-ray  detector  Secondary  electron detector  Sample  nanoScience  Instruments   Motorized stage  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a36ff5b7-9eed-41c2-a872-9bb28bce2c3c/a36ff5b7-9eed-41c2-a872-9bb28bce2c3c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=f7f786dada183fbcf9c7092d9e372636d905719c)
![Incidentelectronbeam  Visible light  Backscattered electrons  (cathodoluminescence)  Characteristic X-Rays   Augerelectrons  Bremsstrahlung  Secondaryelectrons  X-Rays  Heat  Sample surface  Diffracted electrons  Transmitted beam  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/55fe03b5-310e-40cf-b76a-b59f2a120ba4/55fe03b5-310e-40cf-b76a-b59f2a120ba4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=90a48eb8d1e26d89934a87efef555f1e46d0fea6)
Electron Interactions With Solids

Adams, F. and Barbante, C., Ch. 7: Electron-Based Imaging Techniques, Comprehensive Analytical Chemistry (93) 2015 pp. 269 – 313.

![Sample surface  Augerelectrons  Secondaryelectrons  CharacteristicX-Rays  Electron  Backscattered   interaction  electrons   volume  BremsstrahlungX-Rays  Secondaryfluorescence  0.5pm  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/06d96de6-445b-45ab-a500-3e3146a14acb/06d96de6-445b-45ab-a500-3e3146a14acb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=62c8404bcd537c67e7c699a7253dcb07c6d95311)
## Some Things Worth Knowing 

• Typical Primary Beam Energies for Semi Applications are 70 to 1000 eV

• By Definition:

1) Secondary Electrons (SEs) have energy below 50 eV In practice, most SEs have energy in the 1 to 3 eV range

2) Backscattered Electrons (BSEs) have energy above 50 eV In practice, most BSEs have energies near the primary energy

![Backscattered  electron  Inelastic  scattering  Elastic  scattering  BSE   SE  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a0d442fd-d36c-431b-989d-dc0161b09676/a0d442fd-d36c-431b-989d-dc0161b09676.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=4e1a1105c12d7a75ed98cfecf98b0adfb02b7759)
![Secondary electrons  Primary  5O   100   Deam  energy  EnergyE(eV)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/64fc82ae-de7a-4e19-8401-58de7b40995a/64fc82ae-de7a-4e19-8401-58de7b40995a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=d602e40c63ff120e2d30b6887bd3119c4ab247d8)
Fig. 2.4, Thong

## Some Things Worth Knowing About Secondary Electrons 

• Secondary Electrons are created  within the DUT  when  the primary electron beam scatters inelastically from  the DUT’s shell electrons, knocking SEs free • Eventually the primary electron loses all its energy  through such collisions, at which point many secondary  electrons will have been created inside the DUT • The higher the primary energy, the greater the distance  into the DUT the primary electron travel before it runs  out of energy, and the more SEs it makes, but… • The odds of low-energy SE escaping from the DUT  surface drop exponentially with depth from the surface • These competing effects maximize SE emission for  primary beam energies in the 500 to 1000V range.

![Primary Electron Primary Electron  Secondary  electron  Inelastic  scattering  50nm   500nm   5000nm  1kv   5kv   30kV  www.globalsino.com/EM/  8+m  Energy of Incident Electronbeam(keV)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3d011f2b-2125-4c31-a1de-344e1bcf5355/3d011f2b-2125-4c31-a1de-344e1bcf5355.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=5b2ba072f43548ef14a91a081811cd9aca40f024)
## Secondary Electron Yield Calculations 

|Element|Atomic Number|Maximum SE Yield|Primary Beam Energy at Maximum|
|---|---|---|---|
||1③|２.0|400V|
|si||0.89|450V|
|du|29|1.53|400V|


Note 1: Aluminum and Copper emit more SEs than incident primary electrons. Unless grounded, these  metals charge to a positive potential when bombarded with 400-eV electrons. Note 2: Al and Cu will appear brighter than Si in a SE SEM image at 400-eV.

Y. Lin and D. C. Joy, A new examination of secondary electron yield data, Surface  and Interface Analysis, 2005, 37, p. 895-900

What Else Can You Use A SEM For?

![Aluminium  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/87a1d140-c465-4338-b674-60d2eb202ffb/87a1d140-c465-4338-b674-60d2eb202ffb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=079d8609382efe565b74607270cfce08ee6d7655)
![50  00  Image Brightness   ③0  20   SSi   Atomic Number  10-  88  10   15   20   25  E(kev)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4c86f41a-b71a-4035-820e-db5f3f45bfb3/4c86f41a-b71a-4035-820e-db5f3f45bfb3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=c8f65ba846e0a454f6a402664caa5eb5dcdc48c3)
Backscatter Increases with Atomic Number, Z

Note: Al is darker than Cu in 10-kV backscatter SEM image, but Al is  brighter than Cu in 400-eV SE SEM image.

Fig. 4.8, Thong

## Mineralogy with Backscattered Electrons 

![mag.   F   正nt.   det.   WD   Pres.   2022-08-3016:54  30pm   3900×   132μm   10kV   Image   BSDFull   10.202mm   0.10Pa   Scheelite inPyrite  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/aaacffa8-c7a5-493a-b369-def4091df8fe/aaacffa8-c7a5-493a-b369-def4091df8fe.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=18e12632272a6f374dd18b73930279f4892e6eb9)
Regions of differing chemical  makeup have different backscatter  SEM intensities

## Voltage Contrast Mechanism 

Necessary Condition for Voltage Contrast: Some type of energy discriminator  (AKA electron energy spectrometer) in the SE detection path.

A traditional electron energy spectrometer consists of a retarding hemisphere  grid, but today energy spectrometers are built into the SEM column and use  suction tubes to attract SEs, a mirror electrode to retard low-energy SEs  (while passing high-energy BSEs), and “through-lens detectors” – AKA TLDs.

## Classical Electron Energy Spectrometer 

![Retardinggrid  SEdetector  Extraction  g  Ofset  V=Vw+Vs  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/52a3d159-d7ed-46aa-9f24-d4cc8f88401f/52a3d159-d7ed-46aa-9f24-d4cc8f88401f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=a9f3f91cb9e78ab5b606e822d57be4282ce60091)
All Figures taken from J. T. L. Thong, Electron Beam Testing Technology

![E Transmittedportion Aeflectedand returnedto N(E)dE specimen -e(v,-v) V-V）5  10 E(ew) Sv 10 V=-2.5V V.DV  V.-5V 0.5 一10  -5  V=-2V0  5V(V) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c9cd3bbf-fea0-45e4-af98-fcc6a8ad377b/c9cd3bbf-fea0-45e4-af98-fcc6a8ad377b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=2e0928a19859953f3483f5274940f78422eeb54b)
## Schematic: In-Column Secondary-Electron Bandpass Filter 

![-15V  - 15V  - -15V  15V SEO  SE0 SE2  SE2 +70V  + 70V  +70V +70V  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/28a13262-292d-4807-801c-eed015905641/28a13262-292d-4807-801c-eed015905641.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=fe17ac6bcbbdd1a1656c8eb749fadbfbfc413f97)
![DetectorSettings  Detector   TLO  Mode   SecondaryElectrons  Suction Tube   70.0V  Mirror   15.0  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e7373bb6-ea31-4be3-b1fa-e90f58e69848/e7373bb6-ea31-4be3-b1fa-e90f58e69848.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=b6a9521bdcc5906e9e57e6b001c8c99ab25fd68b)
## SE Mode: 

•   $+70\lor$   suction tube   • -15V mirror plate

SE0 : Secondary Electron from 0-V DUT SE2 : Secondary Electron from 2-V DUT

BSEs are not stopped by the -15V Mirror

In-Column Secondary-Electron Bandpass Filter

![Beam  Mirror  electrode  TLD  Push  electrode  Suction  tube  Sample  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8a6a4878-9086-44d0-b986-47888c7f247d/8a6a4878-9086-44d0-b986-47888c7f247d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=a7801bc09a6af36d53d9bc586d47edd978db874f)
In-Lens Band-Pass Filter for Secondary Electrons in Ultrahigh Resolution SEM

Ivo Konvalina \* , Filip Mika, Stanislav Krátký, Eliška Materna Mikmeková and Ilona Müllerová, Materials 2019, 12, 2307; doi:10.339

## COMSOL Simulation/Animation of SE Collection – Field Free 

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d99feac4-d714-41a0-b7fc-9c5e08a51451/d99feac4-d714-41a0-b7fc-9c5e08a51451.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=6a807cd9034d5859cc7822d368831ddc77580457)
## Assumptions: 

1.  Voltage of Suction tube  $=$   277 Volt   2.  Scintillator Voltage= 10,000 Volt    3.  Push Voltage= -100 Volt   4.  Mirror Voltage=-40 Volt   5.  Grounded pole piece    6.  Secondary electron emission is from a point   source on the sample and follows a   Lambertian distribution


Electrical Voltage Distribution

![)/eV k (E n Velocity (m) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ee12cd5d-5cd5-4bdf-89db-e6a5d98884a2/ee12cd5d-5cd5-4bdf-89db-e6a5d98884a2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=4de16b63994cca376bc8700dc0e3466fbe3edbc9)
![280  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0dc7993b-821e-407b-b8b2-364d096eedc8/0dc7993b-821e-407b-b8b2-364d096eedc8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=606f905d0af6d490d8045cf4eb892711c1fef7be)
![8000  With Bz field With Bz field  60100  4000  20100  Without Bz field  Without Bz field 55   10   15   25  tme(ns)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e33fb107-4b16-45e9-b74e-57553d3dde28/e33fb107-4b16-45e9-b74e-57553d3dde28.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=7f865dcc994338169a29c3884db6f68a2b3f3970)
COMSOL Simulation/Animation of SE Collection – Immersion Mode

Note: A 100 mT Bz is applied between the sample and the bottom of the pole piece  •  (Bz is inside the concentric cylinder hole geometry)

Measuring the Voltage Contrast Sensitivity (AKA the instrument Spectrometer Constant)

## Method 1: Measuring Voltage Contrast Sensitivity 

![· Capture SEM image of metal trace on DUT  • Capture SEM image of metal trace on DUT · Repeat for different trace potentials  • Repeat for different trace potentials Trace Brightness vs. Trace Potential  -1V: Brightest -1V: Brightest  Spectrometer Constant  Spectrometer Constant  AVRMS  C = 4.1E-9 V C = 4.1E-9 V√A S   𝑨 𝒔  √2It      Vrms = voltage  = voltage ோெௌ 0V measuremen  measurement uncertainty  uncertainty  beam current   beam current = integration   integration tinme  time -5V   GND   +5V  +1V : Darkest  +1V : Darkest = charge  = charge m3.00KV0.20nATLD857um7.6   Trace Potential  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9b99e44e-01df-4641-a598-237932737456/9b99e44e-01df-4641-a598-237932737456.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=ec4224871380c3c3520df18430cef9ff8d478cd2)
## Method 2: Single-Image Measurement of Spec. Constant: 361pA beam current, 4mm WD, UHR Mode, 100nsDwell 

![500  100H0   b0x1  box1  1V 1  box2  box2  O  0V 1.500  200-0  25:0-0  3000  3.5:0-0  400-0  .   HFD  444 F 1.00K127 nn1.0091 mmTL0   HudirG-Heti  1.0 0-0   2000   3.0:040   4010-0   500-0   60.0-0  bins of X-axis  35000  300-00  25000  20000  ne  15000  10000  500-0  100-0   200-0   300-0   4000  bins  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/91678322-2a8b-42fd-a8c4-2b5c07397260/91678322-2a8b-42fd-a8c4-2b5c07397260.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=814d44822c692b28166d321f24759daed5364d7d)
Apply 0 to 1V square wave on a DUT; Zoom in to a uniform region &  defocus the SEM beam for a flat image

Box 1 (1 Volt Region): 14123 ± 3889   Box 2 (0 Volt Region): 19604 ± 4289

Sigma  $=$   (sigma1+sigma2) / 2 = 4089

$$\begin{array}{r}{V_{R M S}=\frac{S i g m a}{\overline{{B o x~2}}-\overline{{B o x~1}}}\star\,1\lor=0.74\lor}\end{array}$$
$$\mathsf{C}=V_{R M S}\star\sqrt{2I*T}=6.3\mathsf{e-9}\;\mathsf{V}\sqrt{A s}$$
## Best Estimates For Spectrometer Constant 

$$\Delta V_{R M S}=\frac{C}{\sqrt{2\:I\:t}}$$
• Metals:   $\begin{array}{r}{\mathsf{C}\approx5\times10^{-9}\ V\,\sqrt{A\,s}}\\ {\mathsf{C}\ge9\times10^{-9}\ V\,\sqrt{A\,s}}\end{array}$    • Si FinFETs:

Note: Value for Silicon FinFETs depends strongly on quality of sample prep.

Worse performance on Si vs. Metal likely due to lower SE yield for Si.

|Element|Atomic Number|Maximum SE Yield|Primary Beam Energy at Maximum|
|---|---|---|---|
||1③|２.0|400V|
|Si|A|0.89|450V|
|du|29|1.53|400V|
|||||


39

## Other Affects that Masquerade as Voltage Contrast 

•  Changes in voltage of adjacent conductors can change SE collection and appear as VC

![+5V  +SV 3 -2-1  -3-2-1 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/91bfec10-9c83-44a8-9e7c-d684c36c3c88/91bfec10-9c83-44a8-9e7c-d684c36c3c88.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=2d6b769d836ca05cd432d033a13427549cc72bbb)
Fig. 2.19, Thong

•  AC signals can steer the incoming SEM beam slightly; uneven topography or edge-affects  can lead to “false” VC signals •  Contamination buildup sometimes reduces VC signal, but sometimes increases it as well

Voltage Contrast In Action

## Dynamic Voltage Contrast and Barber Poling (Taken from semitracks.com) 

![What might this  nat might this  image show? ageshow?  Clock / 2  Clock / 2 Clock (F)  Clock (F)  SEM IMAGE SCAN GND  GND VCC  VCC 094kx   2ky   815  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0744d066-1e75-43c5-8812-844d3930da3c/0744d066-1e75-43c5-8812-844d3930da3c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=e2dd3112c80bd1b1973863861528e3f47ac77991)
## Voltage Contrast Applied to Waveform Probing 

Q: Is e-beam probing really feasible today? Talk Spoiler: Yes!

Q: But didn’t we do all of this back in the 1990s?

A: Yes, but…

1) they probed front-side µm-sized metal traces   2) technology node then was 0.6, 0.5, & 0.35-µm   3) typical operating voltages were 2.5 or 3.3V   4) today’s requirements are for backside   probing, at 10-nm resolution, at 0.8V

![0000LS01  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f86fa5e3-ca77-4bf7-8cf5-589a38266500/f86fa5e3-ca77-4bf7-8cf5-589a38266500.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=48d7ad3713d446fb6791cc83df3ad452ddee698c)
Schlumberger IDS10000 8.75 GHz in 1996

## Remaining Outline 

Summarize our investigation into the feasibility of modern e-beam probing

## Pathway to Debugging Modern ICs using VC 

•

![Stroboscopic  Stroboscopic   2 GHz  2 GHz  Voltage Contrast  Voltage Contrast   2 GHz  2 GHz  e-beam  e-beam   Spectrum  Spectrum  Mechanism  Mechanism  Oscilloscope Oscilloscope  pulses  pulses  Analyzer  Analyzer 2000.000000MHZ  FWHM   20  enCy(Hz  40   S0  E(ev)  Typical SE Emission Spectrum ypical SE Emission Spectrum  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9bf47c4f-a256-42db-97e0-bf770ec4439c/9bf47c4f-a256-42db-97e0-bf770ec4439c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=30f1c6d0837b96a8e0b6dccc7951f9a4c1caa822)
## Example Waveform: Put Waveform on DUT and plug TLD output  into Oscilloscope 

![DUTWaveform,MetalTrace  10  1MHz  1 MHz 0.8  -1V: Brightest ()ieubis  64  5MHZ  5 MHz  02  00  10 MHz 10MHZ   Time(s)   1e-6  DetectorOutput,1.6nABeamCurrent  0.5  04  ()IeubIs  03  02  1V 1Vpp Signal   Signal  01  PP 00  Time(s)   1e-6  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/07fcd99c-483d-44a9-984a-b216fc2a8233/07fcd99c-483d-44a9-984a-b216fc2a8233.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=a81c84a6db3f0e371bdb395b399b4c6ecfa5d63e)
• DUT Signal • 1 Vpp, 1 MHz, 5 MHz, 10 MHz Sq. Wave

• SEM Settings: • 1.6 nA, Fast Detector setting

• Oscilloscope Setting • 10-ns binsize, 5 us span • No waveform averaging

• Noise Calculation using C:

$$\Delta V_{R M S}=\frac{C}{\sqrt{2\:I\:t}}=725~\mathsf{m V}_{\mathsf{R M S}}$$
## Example Waveform: Increase beam current from 1.6 nA to 6.4 nA 

![DUTWaveform,MetalTrace  10  1 MHz 1MHz  08  )ieubis  64  -1V: Brightest 5MHz  5 MHz  02  00  10 MHz 1OMHZ   Time(s)   1e-6  DetectorOutput,6.4nABeamCurrent  0.5  04  03  02  1Vpp Signal  1V   Signal  01  PP 00  Time(s)   1e-6  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/75c2f979-6c74-4b58-9e8f-24a21841728b/75c2f979-6c74-4b58-9e8f-24a21841728b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=804ebb074323fd666c4a76fb3e0f7c996e9d3947)
•

DUT Signal –  1 Vpp, 1 MHz, 5 MHz, 10 MHz Sq. Wave

•  SEM Settings: –  1.6 nA, Fast Detector setting

•  Oscilloscope Setting –  10-ns binsize, 5 us span –  No waveform averaging

•  Noise Calculation using C:

$$\Delta V_{R M S}=\frac{C_{C}}{\sqrt{2\:I\:t}}=362\:\mathsf{m V_{R M S}}$$
## Example Waveform: Have Oscilloscope average 10 waveforms 

![DUTWaveform,MetalTrace  10  1MHZ  1 MHz 08  )ieubis  64  -1V: Brightest 5MHz  5 MHz  02  00  10 MHz 1OMHZ   Time(s)   1e-6  DetectorOutput,6.4nABeamCurrent,10Avg  OLS  04  0.3  02  1V 1Vpp Signal   Signal  01  PP 00  Time(s)   1e-6  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/028348da-2ae0-42bc-8e2b-5ac3492823d1/028348da-2ae0-42bc-8e2b-5ac3492823d1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=f211660cedc47ae18a67f41292d6ec63dad51b9b)
•

DUT Signal –  1 Vpp, 1 MHz, 5 MHz, 10 MHz Sq. Wave

•  SEM Settings: –  1.6 nA, Fast Detector setting

•  Oscilloscope Setting –  10-ns binsize, 5 us span –  Waveform Averaging: 10

•  Noise Calculation using C:

$$\Delta V_{R M S}=\frac{C_{C}}{\sqrt{2\,I\,t}}=115~\mathsf{m V}_{\mathrm{RMS}}$$
## Example Waveform: Have Oscilloscope average 100 waveforms 

![DUTWaveform,MetalTrace  10  1MHZ  1 MHz 0.8  ()ieubis  604  -1V: Brightest 5MHz  5 MHz  02  0.0  10 MHz 10MHz   Time(s)   1e-6  DetectorOutput,6.4nABeamCurrent,100Avg  0.5  04  )Ieub!s  03   m  02  1V 1Vpp Signal   Signal  O1  PP 0O  Time(s)   1e-6  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2b76bdec-5cce-4513-930b-046ddd30c5ce/2b76bdec-5cce-4513-930b-046ddd30c5ce.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=c654dd76ffe53a3105f28c8340d154c5cf0be819)
•

DUT Signal –  1 Vpp, 1 MHz, 5 MHz, 10 MHz Sq. Wave

•  SEM Settings: –  1.6 nA, Fast Detector setting

•  Oscilloscope Setting –  10-ns binsize, 5 us span –  Waveform Averaging: 100

•  Noise Calculation using C:

$$\Delta V_{R M S}=\frac{C_{C}}{\sqrt{2\:I\:t}}=36~\mathsf{m V_{R M S}}$$
## What have we learned thus far? 

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/336bf986-968d-48d6-b464-c5361464a20e/336bf986-968d-48d6-b464-c5361464a20e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=3dd47853fad12db9acf52b4f748bbd8a1821a140)
Waveform shows up inverted in a SEM’s detector output signal

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8edd5ba4-5dd3-46b1-aabf-bfe436993b48/8edd5ba4-5dd3-46b1-aabf-bfe436993b48.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=0828e9f4ce411cb23d58d306a758bee7d99d66ef)
SNR is not great, but can be improved by increasing ►  beam current ►  signal averaging

This “CW” technique cannot measure frequencies above \~ 5 MHz

How can we measure 2 GHz signals if the system is limited to 5 MHz? We need a new technique.

## Pathway to Debugging Modern ICs using VC 

•

Part 2: How well can we strobe e-beam pulses?

![Stroboscopic  Stroboscopic   2 GHz  2 GHz  Voltage Contrast  Voltage Contrast   2 GHz  2 GHz  e-beam  e-beam   Spectrum  Spectrum  Mechanism  Mechanism  Oscilloscope Oscilloscope  pulses  pulses  Analyzer  Analyzer Spectrum@CF=2000.000000MHz  00  FWHM   -20   -10  Frequency（Hz)  levm  10   30   40   SO  E(ev)  Typical SE Emission Spectrum ypical SE Emission Spectrum  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/95262ecc-e4a4-4fc3-a026-35fd155c6e05/95262ecc-e4a4-4fc3-a026-35fd155c6e05.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=e6981a4d3f3c545dd195b19646a09ab1a63da5db)
## Fast Beam Blanker 

![e-Beam Source  e-Beam Source  Measured e-Beam Chopping Performance Measured e-Beam Chopping Performance  1kev  1keV  Beam Energy  Beam Energy  Effective Pulse Width at DUT Effective Pulse Width at DUT   e per pulse @ 6.4nA D  e -   per pulse @ 6.4nA DC 1000 ev  1000 eV  150 ps  150 ps  5 electrons  5 electrons C2 lens  C2 lens •  Strobe captures “snapshot” of DUT voltage in a   Strobe captures "snapshot" of DuT voltage in a  150-ps window  150-ps window  Fast Beam Fast Beam   • From C data, good SNR requires \~5000 electrons   From C data, good SNR requires \~5000 electrons e-Beam  e-Beam Blanker @ Blanker @  Aperture  Aperture Crossover Crossover   • Averaging repeated measurement gives better Sl   Averaging repeated measurement gives better SNR DUT  DUT  DUT Beam Curren  DUT Beam Current (150-ps FWHM pulses) (150-ps FWHM pulse  Plate 1 Voltage  Plate 1 Voltage  Blanked  Blanked -Unblanked  Unblanked Plate 2 Voltage  Plate 2 Voltage Blanked  Blanked 640 ns typ.  640 ns typ. ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3c615f2b-140e-46c9-96f9-547bb18d5c44/3c615f2b-140e-46c9-96f9-547bb18d5c44.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=1d193e32e7b22c68e77a1413c87bac71162c8e4b)
![•  Part 3: How do we measure a waveform  Part 3: How do we measure a waveform Stroboscopic  Stroboscopic   2 GHz  2 GHz  Voltage Contrast  Voltage Contrast   2 GHz  2 GHz  e-beam  e-beam   Spectrum  Spectrum  Mechanism  Mechanism  Oscilloscope Oscilloscope  pulses  pulses  Analyzer  Analyzer Spectrum@CF=2000.000000MHz  罗0.6   FWHM   -20   -10  Frequency(Hz  0.0   10   20   30   O   SO  E(ev)  Typical SE Emission Spectrum  Typical SE Emission Spectrum Service Mode  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/52c2720a-b53f-460e-9497-78881d4f5035/52c2720a-b53f-460e-9497-78881d4f5035.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=a5932bb615a68d92a9a5effd60178b40b34531f1)
Pathway to Debugging Modern ICs using VC 9991191

## Example:  Typical Waveform Acquisition 

![500 MHz Signal  500 MHz Signal EdgePlacementRawData  Average N times per point  Average N times per point 150  -1V: Brightest Acquire M points per waveform AcquireMpointsperwaveform  748   Z5O   752   754   756  Time(ns)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ce5edeb4-da59-4a99-9cd0-7f8ac990eb72/ce5edeb4-da59-4a99-9cd0-7f8ac990eb72.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=9a7c2d10d5bcc44bc2b1abd8c2d411301123d861)
•  Acquisition takes minutes to complete

![Program Delay Generator to  Program Delay Generator to  desired trigger offset  desired trigger offset Tester  Tester Not Done  Not Done Trigger  Trigger Not Done  Not Done Done  Done  Repeat  Repeat  Delay to  Delay to   N times  N times  Offset   Offset Display  Display  Waveform  Waveform  Point   Point  Strobe /  Strobe / Measure  Measure  Advance  Advance  Delay  Delay  Generator  Generator Waveform  Waveform Repeat M tin  Repeat M times es   Done  Done  Acquired  Acquired ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4eb804b5-6b4b-4bb6-8a46-452ddc3d35d3/4eb804b5-6b4b-4bb6-8a46-452ddc3d35d3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=b17333cf743a89d9063b637fa0628e264ca0a61d)
## Progress Since ISTFA 2019: Can Now Capture 2-GHz Waveforms with under 180 ps Rise Times 

![eVPWaveform:2021-08-0616:41:14   eVPWaveform:2021-08-0616:34:11  1800  1750  1750  1700  1700  -un.   1650  1650  1600  1600  1550  1550  1500  1500   1450  7S3   754   7S6   ZS7   758   753   7S4   755   756   758  Time(ns)   Time(ns)  600 MHz Metal Line  600 MHz Metal Line  1.9 GHz Metal Line  1.9 GHz Metal Line ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/531ddc30-1bc9-48a3-a3fb-5a4a38ed1dfb/531ddc30-1bc9-48a3-a3fb-5a4a38ed1dfb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=c548af8c7d84987fae16cf1236fff1b547e99d48)
Waveforms also captured from silicon, with SNR about half that of metal, but data is customer proprietary.

## Example:  Typical  Waveform Measurements 

![2GHZ  2 GHz -1V: Brightest  1.75 GHz  1.75 GHz 15 GHz  1.5 GHz 1.25 GHz 1.25 GHz  1GHz  1 GHz 750 MHz 750-MHz  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7a1b1f85-8bf6-4905-9ab4-246fc006ae1e/7a1b1f85-8bf6-4905-9ab4-246fc006ae1e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=ee4e579a5b0081fb8cbc8dfea27ed740b161fbad)
![Delay:198.598ns  三110  Time/div.100ps  uV/div.134.65341  Bin width.5ps  350.1  315.1  350  500V_6.4nA  _highestBW_SBV0_5MHz_110ps  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/639f25c9-ab32-40b6-b13b-59a5f4cbf766/639f25c9-ab32-40b6-b13b-59a5f4cbf766.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=ea3386692585f8e2d9afeb1b85a07205700b04d4)
Measured 10-90 % Rise Time = 160 ps

## Voltage-Contrast Waveform of 2 GHz Signal (400 mVpp, ADCMP580 DUT) 

![eVPWaveform  500 ps 500 ps  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f7cb39b7-2d8e-4c67-bfd6-55ae8cbdd160/f7cb39b7-2d8e-4c67-bfd6-55ae8cbdd160.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=2e59c222053a646031d6317418699a5e141e7553)
## Pathway to Debugging Modern ICs using VC 

![•  Part 4: How can we measure the DuT frequency?  Part 4: How can we measure the DUT frequency? Stroboscopic  Stroboscopic   2 GHz  2 GHz  Voltage Contrast  Voltage Contrast   2 GHz  2 GHz  e-beam  e-beam   Spectrum  Spectrum  Mechanism  Mechanism  Oscilloscope Oscilloscope  pulses  pulses  Analyzer  Analyzer 00  FHM   30-   -20   -10  Ievm  30   40   SO  E(ev)  Typical SE Emission Spectrum ypical SE Emission Spectrum  viceMod  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e4a1a59e-1729-4ece-95fe-fc7dafb7bda6/e4a1a59e-1729-4ece-95fe-fc7dafb7bda6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=e419741d196aacb363ff8b867ec0e80c444c1fef)
## What is frequency-domain data good for? 

![e9   Spectrum@CF=2000.000000MHz  14  S10  20.8  06  -1V: Brightest 20   -10  Frequency(Hz)   t2e9  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ab3c8364-d71a-46da-a373-771ed5781315/ab3c8364-d71a-46da-a373-771ed5781315.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=5d1ff597e4f23374a1c7b8a114e96637e2ea4acd)
•  Put system in Spectrum Analyzer Mode   •  Point beam around DUT until you find active circuitry

![180° Phase 180°Phase  O°Phase  0° Phase ServiceMode  11/17/2017  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/74632db0-c8fb-4019-873a-e79a4ab15960/74632db0-c8fb-4019-873a-e79a4ab15960.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=58369120978c40950754a209501eb7f80977ca8d)
![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cb73f03b-e166-43da-afa6-eab15b5f3dd3/cb73f03b-e166-43da-afa6-eab15b5f3dd3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=8a51bf608b2bdc6cd90ca0e8a9e8e94790ee603b)
![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c39bd385-f105-4942-8582-ae969dd3c7c3/c39bd385-f105-4942-8582-ae969dd3c7c3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=3398ad0221e9e3f96396d44221cd2a891ee8582d)
SEM Image

of underside FinFETs

Inphase (I) signal shows clock with phase

Overlay shows active regions Useful for Navigation

## Progress Since ISTFA 2019: More Examples of System Capabilities 

![EdgePlacementRawData  200  150  200  248   754   756  Time(ns)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/eeba44a8-21da-4fad-876f-187ef8f825b9/eeba44a8-21da-4fad-876f-187ef8f825b9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=298650052f49a2a903e04e7a51d529ab43a6c138)
Edge Placement Accuracy is much finer than system rise/fall times.

![1e9   Spectrum@CF=2000.000000MHz  14  cun  10  0.6  0.4  02  0.0  -30   -20   -10   10   20   30  Frequency(Hz)   +2e9  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/51a050ec-a640-44a5-a6f3-8a590ba626aa/51a050ec-a640-44a5-a6f3-8a590ba626aa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=a5c7ef9bf6fd6cee9ea61304412ba827e7ed74c5)
Spectrum Analyzer Mode up to 2 GHz

## Voltage Contrast Spectra from 100 to 2000 MHz 

![S08  S06  208   08  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3c377808-3deb-4725-b533-ab4604efb762/3c377808-3deb-4725-b533-ab4604efb762.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=4bfce04f1a00c06baca9c160df11c5efe5deb642)
## Spectrum Analyzer Signal Strength vs Frequency 

Meridian-E Signal Spectrum Analyzer; Strength vs Frequency; 6.4nA 500 eV

![16  16 14 12 Signal Strength (Arb. Units) 管10  10 8 C  6 4 2 0 0  200  200  400  400  600  600  800  800  1000  1000  1200 1200   1400 1400   1600 1600   1800 1800   2000  2000 Frequency (MHz)  Frequency (MHz) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/22c7a8d6-6d2d-4c7f-9eb6-2b9fa154f8f2/22c7a8d6-6d2d-4c7f-9eb6-2b9fa154f8f2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=5926b2704fc8ebe9dc26801c18c838eaa00531e4)
BW seems flat out to 2 GHz; amplitude variation is likely due to probing new spots each measurement.   There is no obvious sign of a roll off in the frequency domain, suggesting 2 GHz system bandwidth.

## Frequency Maps: 500 MHz, 1000 MHz, 1700 MHz, 2000 MHz 

![Service Mode   Service Mode  8mode   rrame   mode  Service Mode   Service Mode  modeframe   8/6/2021   H   ND   det   HFvV   3um   modeframe   8/6/2021   vD   cet   HFv  1.2ml   4:03:54PM   1.00kV   lios PFIB   20.7um   Helios PFIB  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7edbb07e-5db9-4e09-904f-8001ac0cd9b2/7edbb07e-5db9-4e09-904f-8001ac0cd9b2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=13b3fdb69e6202c60a53c7f6f72a638e158cef96)
## Frequency Map on Silicon FinFET Transistors 

![Service Mode  mode   frame   8/13/2021   H   curr   WD   det  HF   dwell  Custom  2.6min  4:32:46PM   1.00kV  5OPA  3.0mm   TLD  20.7μm  100.00μs  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/24f580b9-667f-4c99-a278-f33af8a5abfb/24f580b9-667f-4c99-a278-f33af8a5abfb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=1ffeea7948dc4b7da017bf388ea4e6c4652e7bad)
•  User can find active regions on IC using:

•  low-current “CW” frequency mapping for clock frequencies < 5 MHz, or   •  Standard pulsed operation for any clock frequency up to 2 GHz.

Locking the Tester Clock with the Meridian-E Clock enables phase frequency maps.

## E-Beam Applications 

## V oltage  C ontrast 

## E lectron  V oltage  I maging 

## E lectron  I nduced  D evice A lteration 

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/50a1c786-58f3-4293-851d-355e19e6d00f/50a1c786-58f3-4293-851d-355e19e6d00f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=f2734c6ccdecb89e57ab70092c33ee278f92e2b3)
Ability to visually map logic high or  lows in FOV

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6260e805-d0f7-496b-8b06-c1a740e2f95a/6260e805-d0f7-496b-8b06-c1a740e2f95a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=c8c3f75bb41c4abda06d9a61e03d9fe1f1068178)
Ability to map transistors switching at  specific frequency

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/275cd24b-0e98-42b6-9ae1-89abad929a4a/275cd24b-0e98-42b6-9ae1-89abad929a4a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=1b4fc05f23916fbfd03ef8a44ae6beefef3f8e31)
Ability to alter a devices performance  and map area’s which are sensitive  to induced parasitic current

## E lectron  V oltage  P robing 

## E lectron  B eam  I nduced  R esistive  Ch ange 

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/091c2c0f-487e-405f-a022-830fe3974804/091c2c0f-487e-405f-a022-830fe3974804.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=d3b36f908738f7a2f177422eed30b201a04624c6)
![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/97ceb5bd-f974-4425-9443-ebd61c097aed/97ceb5bd-f974-4425-9443-ebd61c097aed.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=b62d904905d06d3ad2173e9123291af72fbb4e4b)
Ability to directly measure timing and  voltage of a transistor or metal line as a  function of time

Ability to map current paths

## E-Beam Probing Conclusions 

Described workings of a SEM system using VC to probe active modern ICs     Waveforms, Spectra, and Frequency Mapping up to 2 GHz was disclosed   A roadmap to a 6 GHz system seems feasible     SEM systems afford three orders of magnitude improvements in resolution over  optical toolsets   Numerous SEM-based techniques, besides just VC-based measurements, are available   EBIC, EBAC, EBIRCH   Passive voltage contrast   Logic-state mapping   Nanoprobing

SEM-based tools are becoming indispensable for modern IC characterization  and debug applications

## Thank You! 

