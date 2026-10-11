---
title: "Baozhen_Li_MOL and BEOL_Reliability.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_e9142c3c7f4ac9f6d93429b2739090bc7295230462135641
file_size: 4657910
---

## MOL & BEOL Reliability  Challenges for Advanced  Technology Nodes  

Baozhen Li  李保振 IBM Systems Essex Junction, VT 04542, USA

A tutorial for IEEE IPFA,  Hangzhou, China; July 2, 2019

## MOL & BEOL Reliability Challenges  for Advanced Technology Nodes  

Aggressive technology scaling places severe challenges on patterning, process integration, material selection and  reliability.  In this tutorial,  the interactions among these challenges will be highlighted.  The focus will be on middle  of line (MOL) and back end of line (BEOL) reliability challenges including electromigration (EM), dielectric integrity  (TDDB), and Stress Migration (SM).  After a review of the fundamentals of each reliability mechanisms, details will  be given on how the new patterning, integration schemes and material sets impact each of the reliability failure  mechanisms.  To meet these challenges, demands and progress on new understanding, innovation and reliability  models will also be reviewed.

## Outline  

•  Introduction         -  MOL/BEOL architecture       -  Reliability Fundamentals    •  BEOL/MOL Reliability Mechanisms         - Electromigration (EM)         -  Stress Migration (SM)         -  Thermal Fatigue/ Thermal Cycle (TC)         -  Low K Time Dependent Dielectric Breakdown (TDDB)    •  Reliability Challenges with Technology Scaling         -  Dimensional Scaling        -  Material Scaling        -  BEOL Reliability Challenges        -  MOL Reliability Challenges    •  Summary Remarks

## Outline  

•  Introduction         -  MOL/BEOL architecture        -  Reliability Fundamentals    •  BEOL/MOL Reliability Mechanisms         - Electromigration (EM)         -  Stress Migration (SM)         -  Thermal Fatigue/ Thermal Cycle (TC)         -  Low K Time Dependent Dielectric Breakdown (TDDB)    •  Reliability Challenges with Technology Scaling         -  Dimensional Scaling        -  Material Scaling        -  BEOL Reliability Challenges        -  MOL Reliability Challenges    •  Summary Remarks

## Introduction – Chip stack/Architecture  

FEOL  (Front End of Line) :      Devices/Transistors   MOL (Middle of Line):   Local interconnect for  transistors (CA, M0)  BEOL (Back End of Line):      Interconnects (Mx, Vx)  FBEOL (Far Back End of Line):  Connecting chip to  packages (BLM, C4…)

![TSMC 7nm Stack,  TSMC 7nm Stack  Wikipedia  Wikipedia  IEDM2016  IEDM2016  lead-free  solderbump  Cr,Quand Au liners  FBEOL  FBEOL   seal layer （nitide or oxde)  PSG   SiNseal layer  C5  SOD  4   C   4  Ta/TaNbamer layer   SiCetch stoplayer  BEOL  BEOL  C3  SiCetch stoplayer  Gu2  SOD   PE-TEOS  SiCseal layer   SOD  MOL  MOL   Pohystgaae  tungsten  FEOL   spacer  FEOI   USG  Pwied Sior  p-piican wafer  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f3b170a2-d235-4d96-af9e-734529fce287/f3b170a2-d235-4d96-af9e-734529fce287.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=b94f9e0b8a9f9ba1c3ae92743ff9c53899c2e529)
## Introduction – MOL stack/Architecture  

![1  CBbar  Fin  STI  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d8ea1589-eefa-4c76-8e96-426097b0880b/d8ea1589-eefa-4c76-8e96-426097b0880b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=3a3d9627b1b922e7ed4399a9c9e9025b3b69cb0c)
R. Xie, et al IEDM 2016

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f367432e-ac0d-48ad-9636-f870e1752cff/f367432e-ac0d-48ad-9636-f870e1752cff.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=a4977f8ab44daf9310d1663d5b28045b67000e89)
K. Cheng, et al IEDM2016

Main Reliability Challenges for MOL:  PC-CA TDDB (Time Dependent Dielectric Breakdown)

![M3  Dielectric  Dielectric   Cu Line  Cu Line  V2  M2  Cap   Cu Via  CuVia   Liner  iner  V1  Cu Line   M1  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/83400c39-3fe4-4069-916f-02fea02490e7/83400c39-3fe4-4069-916f-02fea02490e7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=b204c394600208bca1540315712d3cb5c9b66a48)
![IBM  IBV  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9906cc16-a365-4df1-9995-5fa2316b8a11/9906cc16-a365-4df1-9995-5fa2316b8a11.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=86975f96db52c4f9f7a8d6df88c230352b96a65d)
![Inte  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b712986d-9798-4bbe-aa4e-66a550aa1f15/b712986d-9798-4bbe-aa4e-66a550aa1f15.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=e4d4ebb76764c344977fda4a18d8d9a59ff41a34)
Main Reliability Challenges for BEOL:  EM, TDDB, SM, TC & CPI

## Introduction – BEOL Architecture  

![Ti/TiN  TiVTiN   Al  W  Al   SiO2  SiO2  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/930617f9-cf7a-4093-932a-527bfd3549cf/930617f9-cf7a-4093-932a-527bfd3549cf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=30b6c5c061621db837b0fbea2ebc48352f845e9a)
Al or Al-0.5%Cu Interconnect

•  Mainly for 180nm & older     tech node  •  Alloying with Cu (\~0.5%)  to enhance EM reliability  •  Subtractive process

![Ta/TaN  Ta/TaN.   Cu  SiCN cap.  SiCN cap  Cu  CU   LoW K  Low K  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d780d264-4d0e-49de-930b-b59d090193ef/d780d264-4d0e-49de-930b-b59d090193ef.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=92f1ba858b0af54075761d334515b8010750ed98)
Cu Interconnect

•  Mainly for 130nm or newer  tech node  •  Alloying with Mn or Al (\~0.5%)  to enhance EM reliability  •  Damascene Process

## Introduction – BEOL Architecture  

Metal Deposition

|SiO2|
|---|


Metal Etch to Define Lines

![Al  SiO2  SiO2  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a9de3034-837a-400e-a7bd-3f3293f1a15e/a9de3034-837a-400e-a7bd-3f3293f1a15e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=e89a45210927621ca649a2604bc3155e03481897)
![ILD Deposition & CMP  ILD Deposition & CMP  Al  SiO2  SiO2  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/605d311c-0ae2-4b6b-b221-6c7cbad2d0a8/605d311c-0ae2-4b6b-b221-6c7cbad2d0a8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=d28e3f86b72fae1f9ddf8706b76eeec12822e08c)
Subtractive Process for Al

IPFA2019, B. Li

Etch Trenches into ILD (Low K)

![Metal Deposition  Metal Deposition  CMP & Capping  CMP & Capping  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/92118a4e-ffc5-4880-9da3-2c1911b2b59d/92118a4e-ffc5-4880-9da3-2c1911b2b59d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=339838a7d9df9db2407ac431f588a24451c309c7)
Damascene Process for Cu

## Outline  

•  Introduction          -  MOL/BEOL architecture       -  Reliability Fundamentals    •  BEOL/MOL Reliability Mechanisms         - Electromigration (EM)         -  Stress Migration (SM)         -  Thermal Fatigue/ Thermal Cycle (TC)         -  Low K Time Dependent Dielectric Breakdown (TDDB)    •  Reliability Challenges with Technology Scaling         -  Dimensional Scaling        -  Material Scaling        -  BEOL Reliability Challenges        -  MOL Reliability Challenges    •  Summary Remarks  •   The nature of reliability    Probability Projection       - Probabilistic vs deterministic        - Projections          \*  Statistical Projection:                From small samples   product population               From high percentile   low percentile of failure distributions        \*  Acceleration Projection:               From accelerated failure times (minutes/hours)   product lifetime            From accelerated conditions   product use conditions        -  Projection Results            \*   Probability of cumulative failure, lifetime, etc.             \* Confidence level/bound under given assumptions            IPFA2019, B. Li    •  Three Key Terms:       -  Acceleration          Accelerate failure to a short time         Thermal, voltage, current, …     -   Distribution           Failure time variations         Sample size determination      -   Size/Area/Content Scaling            Sample area/content vs product          -- also part of acceleration

![Stress  Stress  Data  Data   Acceleration Factor  Acceleration Factor  Project to use condition ProjecttotargetCDF Project to use condition   roieo..  Percentile  Distribution  Distribution   ctto..........  TargetCDF  Target CDF   EOL  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ea486053-631a-477c-90b4-3b905fbf6c98/ea486053-631a-477c-90b4-3b905fbf6c98.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=8daec5455c8939a0a5dc5a316193ed3ff7d8c646)
## Terminology:   

Acceleration Factor – fail time ratio @ use vs @stress; CDF   Cumulative Failure;  EOL   End of Life;  POH   Power On Hours

IPFA2019, B. Li

## Models & Projections  

•  Reliability Projection Models             F(t) = g(j, E, T…)\*f(t)      -   Acceleration  g(j,E,T…) – Kinetics       \*  Accelerate failures by elevating driving forces, e,g. j, E, T…        \*  Project from sec or hours to years             many orders of magnitude projection, accuracy is critical        \*  Should only make fails faster under same mechanism             not introducing new failure mechanisms     -   Distribution  f(t)        \*  Should reflect the failure mechanism        \*  Project from high (sample) to low percentiles (usage, \~ppm)     -   Model selection            a) can fit the stress data (Mathematics)         b)  consistent  with the underlying physics (Physics)

IPFA2019, B. Li

•  Reliability models built on certain assumptions & simplifications

-  Application ranges, pitfalls       -  Parameter meanings and calibrations        -  Physics vs Mathematics       -  Projection results, confidence, common sense          \* Little difference in stress data   huge difference in lifetime projection

![100  AAAAAAAAAAAAAAAA A 10  AAAA A  Stress  Stress  Failure %   A 1  Weibull  Weibull   Data  Data  0.1 0.01   LogNormal  LogNormal  0.001 1  Failure Times  Failure Times  100  ２0０  200 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/12a395bc-4118-4261-8da5-9aab4da5ef44/12a395bc-4118-4261-8da5-9aab4da5ef44.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=6c54f57b6421f14fb1647fc9e112e4d82008e42f)
Distribution Model

IPFA2019, B. Li

![exp(1/v)  exp(-vV) \~exp(-√E)  exp(-V)  Stress Window↓  Stress Window  Applied V or E  Applied V or E  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/32d96f75-3399-4265-b8f5-8add88d16d3b/32d96f75-3399-4265-b8f5-8add88d16d3b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=6745838d7eae24b903d1cbc8065f65520f43808e)
Acceleration Model

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fe1d6afb-1be7-4e19-bc0f-9776d6433da9/fe1d6afb-1be7-4e19-bc0f-9776d6433da9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=d4945dc6f51e0e17d01697bdc6112eb1a5b9049a)
•  Practical Considerations of Reliability         -   Balance cost, performance & reliability                sustainable business               “right” reliability margins

•  Reliability   Risk management

•  The best compromise   between needs for  reliability, cost effectiveness and time-to-market  (competitiveness)

•  Reliability cannot be low, need not be higher than  necessary, but has to be adequate   for a particular  application

![Cost  Performance   Reliability  Hommel, 2014  Hommel, 2014  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ae2bb31a-4b5a-4279-b291-4601691c4930/ae2bb31a-4b5a-4279-b291-4601691c4930.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=ed4c9699fed673d298091296b08e426cea325343)
Key Parameter Triangle

## Reliability vs Quality  

![Early fails due to defects.  Early fails due to defects  Improved by burn In & screen    Improved by burn In & screen   Reliability  Reliability  Concerns  Concerns  Part of Qualify Control   Part of Qualify Control  Failure Rate   Bathtub Curve  Bathtub Curve  Mortality  Mortality  Infant  Infant   Product Useful Life  Product Useful Life   Wear out  Wear out  Time  Time  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ad7d2d01-57f4-4822-83a2-0e2b584420d4/ad7d2d01-57f4-4822-83a2-0e2b584420d4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=f561395c001a1ef518032cc76763cf3bf99a4830)
• Product Quality – focus on early fails       -- Process defects, test escapes    • Technology Reliability – focus on wear out (near end of product life)       --  Make sure no wear out during product useful lifetime    • Field returns vs reliability         Returns: Defects and test escapes, not wear out fails

## Reliability vs Quality  

## Reliability/Quality Failure Categories  

- Very low (nearly zero) failure probability until onset, then increasing rapidly            \*  Should see virtually no wear-out fails during product use life         - Caused by technology or application limits         -  Eliminate wear-out from design point             \*  Technology definition             \*  Design ground rules             \*  Application specification              -- e.g.  EM – Jmax for given temp, and lifetime                          TDDB  -- Vmax for given temp, area and lifetime         -  BI (burn-in) & screen should not help, may cause some useful life degrade

## Reliability/Quality Categories   

## 2. Systematic Defects  

- Process marginality           - Strategy            \*  Process and technology control                - Design rules for manufacturability and yield                - Process window optimization                - Process monitoring                  e.g.  Alignment and CD control caused via-line spacing marginality        -  Sometimes, hard to distinguish Systematic defects vs Wear-out            \* Early fails or adders to wear-out        -  Burn in & screen may or may not help

## Reliability/Quality Categories  

## 3. Random Defects  

-  Seen as early product fails        -  Caused by process deficiencies        -  Strategy            Continual defect reduction            Process/tooling optimization            BI or Screen out residuals & outliers              e.g.  CMP scratches caused near shorting

4. Process Vintages and Excursions      - Gross defects      - Gross deviation from process targets

## Outline  

•  Introduction         -  MOL/BEOL architecture       -  Reliability Fundamentals    •  BEOL/MOL Reliability Mechanisms          - Electromigration (EM)         -  Stress Migration (SM)         -  Thermal Fatigue/ Thermal Cycle (TC)         -  Low K Time Dependent Dielectric Breakdown (TDDB)    •  Reliability Challenges with Technology Scaling         -  Dimensional Scaling        -  Material Scaling        -  BEOL Reliability Challenges        -  MOL Reliability Challenges    •  Summary Remarks

## Reliability Mechanisms  

•  Reliability Mechanisms         - EM   Electromigration        - SM   Stress Migration      - TC   Temperature Cycling        - TDDB   Time Dependent Dielectric Breakdown    •  Overview of Each Mechanism         - Physics Behind Each Mechanism        - Acceleration Models (E/V, I, T)        - Failure Time Statistics        - Lifetime Projection        - Process & Integration Impacts        - Circuit/Chip Design Concerns

## BEOL Reliability Mechanisms  

![L. Clevenger, MAM 2013  L. Clevenger, MAM 2013   IEM  CPI  EM  TDDB  Chip-PackageInteraction  Crackstop  UItrathick Cu (Adhesion)  Fatline/thinline transition  Capthicknessvs.reliability  ULK TDDB, Vmax  ULK graded layer thickness  Metallization(void-free)  Cu electromigration  Alloy extendibility (Eg, g.s.)  Backup metal cap process  Cu grainsize, microstructure  Edeistein,20121ITC   MOL/BEOLinterface  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0bba6e02-d24f-4300-912f-078c6dc1f8c7/0bba6e02-d24f-4300-912f-078c6dc1f8c7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=aa4dbceafa5584482bb26cd9a095e554f03aca35)
## Outline  

•  Introduction         -  MOL/BEOL architecture       -  Reliability Fundamentals    •  BEOL/MOL Reliability Mechanisms         - Electromigration (EM)         -  Stress Migration (SM)         -  Thermal Fatigue/ Thermal Cycle (TC)         -  Low K Time Dependent Dielectric Breakdown (TDDB)    •  Reliability Challenges with Technology Scaling         -  Dimensional Scaling        -  Material Scaling        -  BEOL Reliability Challenges        -  MOL Reliability Challenges    •  Summary Remarks

## EM Introduction  

•   Electromigration (EM)   An current driven wear out mechanism     -  Mass Transport due to momentum exchange between electrons & metal ions

electron wind carries metal ions/atoms away, leaving void behind (cathode)    metal atoms pile up at anode, extrusion to short with neighboring lines

Electrons push Cu moving with them

Cu

e-

Cu

e-

Cu

e-

Cu

Cu

e-

Cu

Cu

Cu

Cu

Cu

Cu extrusion

Cathode

Cu moves out,

leaves void behind

Cu piles up

Anode

Void underneath

via in the Cu line

IPFA2019, B. Li

Void in the via

Cu extruded out from a line and  shorted with a neighboring line

## EM Driving Force and Cu Migration  

•   Driving Force for EM  F =  Z\*e

Z\* Negative - metal migrates with e-  wind, void forms at cathode  Z\* Positive – metal migrates against e- wind, void forms at anode  •   Nernst-Einstein Eq. – drift velocity of moving ions/atoms

![D  A  H  (   )     O,eff  ,0 eff  e  kT  ( Z  \* e       ) d  kT  eP   L ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/336eb0b5-860d-4e81-bb52-f2797494e0ab/336eb0b5-860d-4e81-bb52-f2797494e0ab.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=3a7c9cd1ad6e1faf281f28d3f6ecaf1c94400a8f)
Diffusion   Driving force   Back flow force  Thermal effect   Current density effect   Stress effect

D 0,eff  – Effective diffusivity;    H -- Activation energy for metal diffusion        -- Specific resistivity of metal     j  -- current density;     -- Atomic volume;    / L – Stress gradient

##  Blech Effect  

•   Nernst-Einstein Eq. – drift velocity of moving ions/atoms

![D  ( H )      o,eff  ,0 eff  e  kT  ( Z  \* e   ) d  kT  ep   L ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/80074cde-b61c-49a1-9ff5-28a0d10a2b94/80074cde-b61c-49a1-9ff5-28a0d10a2b94.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=45c384243b2ed4a1ab641d2760c186df87c68f94)
Diffusion   Current driving force   Back flow force

Blech Effect   a special case of N-E relation   $@\;\mathsf{v}_{\mathsf{d}}=0$

When driving force is balanced by back flow force

EM immortality

$$\nu_{d}=\frac{D_{0,e f f}}{k T}e^{(\frac{-\Delta H}{k T})}(Z^{*}e\rho j-\Omega\frac{\Delta\sigma}{\Delta L})=0$$
then

![e-    Δσ/L   L  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/aa34a2be-dab6-4b6a-87a6-92ee335b1bdb/aa34a2be-dab6-4b6a-87a6-92ee335b1bdb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=775350f3b9ef540283fbbfad00270fe7d5c316a6)
Blech effect    important for circuit  designs to fight EM  limitations   short lines can  carry higher current or  become EM immortal!

$(j L)_{c}=\frac{\Omega\Delta\sigma}{Z^{\ast}e\rho} $  (jL) c  – Blech effect threshold product     $\mathsf{I f}\left(\mathsf{j L}\right)<\left(\mathsf{j L}\right)_{\mathsf{c}},$  , no concern for EM failure, immortal    – threshold stress   related to dielectric confinement

## Cu Migration Paths  

•   Key Factors for EM Reliability        -    Flux divergence (J out  > J in )           \*  Essential for void formation  (triple points, defects…)           \*  Void nucleation and growth         -   Final critical void location       \* Critical void size to fail        -   Backflow stress (Blech effect)        -   Fast diffusion path             Major engineering focus to improve EM           \*  EM kinetics ( H)         Different  H for different path           \*  Historically, Cu/Cap as the fastest       \*  Grain boundary important                bamboo vs poly-grains

![Cap Layer  Cap Layer   Grain Boundary  Grain Boundary  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/696bdfe4-12e1-46a0-9b3b-a71531cedea8/696bdfe4-12e1-46a0-9b3b-a71531cedea8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=02268f34c614fd90250a2f8b9e6025d8890ae1a9)
e- flow direction: left to right

Liner

diffusion along Cu/cap interf.  diffusion along grain boundaries  diffusion across grain bulk  diffusion along Cu/liner interf.

## EM Failure Modes  

•   Failure Mode for Dual Damascene Cu Interconnect     -  Cu can not diffuse through via bottom liner (Ta/TaN)           two distinct failure modes for dual damascene Cu

1.Via-depletion  (upstream) mode

• Electrons flow from via up to line    • EM void usually forms in the via    • Via liner and seed coverage is key

2.Line-depletion  (downstream) mode

• Electrons flow from line down to via  • EM void usually forms under the via in  the line    • Via/line contact is key

![ e-    M2 2    Void  Void  V1  M1 V1    Liner   Liner  Via Depletion – Upstream  via   Depletion - Upstream  Cap  cap  Void  Void   V1   e-   M1 1    Liner   Liner  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3ab05c42-7ced-485a-b503-24fe93e1a3d5/3ab05c42-7ced-485a-b503-24fe93e1a3d5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=c0ec76988d239eb4b91275f5232818014b1f16bb)
Line Depletion – Downstream

## Process Impacts on EM  

## •   Process Impacts on EM  

-   Strengthening Cu/Cap interface to slow down the fast Cu diffusion          \*  Pre-cap cleaning on Cu surface; Cu resistance increase if over-cleaned          \*  Cu-alloy seed (Cu-Al, Cu-Mn): alloy element segregation to Cu/Cap interface          \*  Metal cap layer (CVD Co, Ru, CoWP,…) between Cu and dielectric cap            All can increase EM activation energy ( H )      -   Better liner coverage on via bottom and sidewalls          \*  Improve Cu fill to reduce pre-existing voids, esp sidewall voids          \*  Remove early fails (slit void in or under via)          \*  Keep liner/Cu interface as a slow Cu diffusion path      -   Grain size engineering to reduce grain boundary Cu diffusion          \*  Prefer bamboo structures           \*  Fine grains reduce effectiveness of Cu/Cap interface strengthening           \*  Grain size distribution impacts   due to V c  (critical void size) and   $\upnu_{\mathsf{d}}$   variations

## EM Failure Time Acceleration  

## •   EM Failure Time  

=  𝑉 𝑣𝑜𝑖𝑑,𝑐  -- Void volume = net amount of metal migrated out  𝑡 𝑓  𝐴𝑣 𝑑          once void volume (V void ) = critical value, EM fail occurs

## •   EM Failure Time Acceleration  by j and T  

$M T F(t_{50})\!=\!\frac{A}{(j-j_{c})^{n}}e^{\frac{\Delta\mathrm{H}}{k T}} $  -- Modified Black equation   MTF – Median time to failure   $({\sf t}_{50})$      When  $j\rightarrow j_{c},$   failure time becomes   A – Constant, geometry & material related    sensitive to process variability   j – Stress current density    --  t  distribution becomes broad   j c  – Threshold current density (Blech effect)    f   when close to Blech threshold   n  -- Current exponential constant  H  -- Activation energy, usually in eV   kT  -- Normal thermal energy term

## •  LogNormal - widely used for EM failure    

-  Probability Distribution Function (PDF)

$$f_{L N}(t)\,{=}\,\frac{1}{\sqrt{2\pi}\sigma t}e^{-[(L n(t)-L n(t_{50})]^{2}/(2\sigma^{2})}$$
-  Cumulative Distribution Function (CDF)

$$F_{L N}(t_{p})=\int_{0}^{t_{p}}\frac{1}{\sqrt{2\pi}\sigma t}e^{-[(L n(t)-L n(t_{50})]^{2}/(2\sigma^{2})}d t=\int_{-\infty}^{Z_{p}}\!\!\frac{1}{\sqrt{2\pi}}e^{-[(L n(t)-L n(t_{50})]^{2}/(2\sigma^{2})}d t.$$
![9=0.2  =0.2  PDF   0=0.3  =0.3  0=0.4  =0.4  PDF plot  PDF  PDF  t 50  60  Time To Fail  Time To Fail  Higher o, shallower  CDF plot  , shallower  Percentile   distribution  distribution  ........  CDF  CDF  Time To Fail  Time To Fail  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1bcd2c86-55bf-473e-b6c6-8631120d8493/1bcd2c86-55bf-473e-b6c6-8631120d8493.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=08a9d401f063aa7597009d840c512db6a2bc0d68)
$$z\,{=}\,\frac{L n(t)\,{-}\,L n(t_{50})}{\sigma}$$
-  Two parameters define distribution:   & t 50

\*  t 50  – median time to failure

•  Bi-modal LogNormal      -   Superposition model             -- mixture of different failure modes (A & B)         CDF(t) = p(A)\*CDF A (t) + (1-p(A))\*CDF B (t)         PDA(t) = p(A)\*PDF A (t) +(1-p(A))\*PDF B (t)         p(A) is the probability for mode A      -   Competition  ( Weakest-link) model            -- failure modes in serial fashion         CDF(t) = CDF A (t) + CDF B (t) – CDF A (t)\*CDF B (t)         PDF(t) = PDF A (t)\*(1-CDF B (t)) + PDF B (t)\*(1-CDF A (t))     -   Parameters to define the distribution        -- 4-param with common  :  f a ( , t 50a ),  f b ( , t 50b ) &        -- 5-param:   $f_{a}(\upsigma_{\mathrm{a}},\,\mathfrak{t}_{50\mathrm{a}})$  ,  f b ( b , t 50b ) &  p

![CDF(t)  measured timetofailure  datafit  NO  P(A)=0.50  t50A=10.1h0A=0.34  t508=61.5h 0g=0.37  10   20   50   100  t[h]  0.06PDF(t)  PDF(t)  [1/h]  P(A)·PDFA(t)  0.04  0.02   (1-P(A)·PDFs(t)  10   20  th]   50   100  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f5bd7b9b-9e74-4605-94b6-23c0f893bc6e/f5bd7b9b-9e74-4605-94b6-23c0f893bc6e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=3ce775f1f6879a9024c9f9f0c53cc6ba20d8d4e6)
Fischer et al, IRPS 2000

## •  3-parameter LogNormal  

-  Lognormal with threshold

50

ln

2

1

0

t

X

f t t

,

X

)

t

( t

50

exp

0

X

X

0

) 2

2

0

2

2

,

t

X

0

-    ${\sf X}_{0}$   is the threshold value, the 3 rd  parameter (in addition to t 50  &  )    \*  For EM, it is the minimum failure time for the distribution

![  tn=25, 0=0.2  t.=25, 0=1.0  Percentile   Broken line - 2-parm   Percentile  Solid lines - 3-parm    X。=0,1,3,6,9  X=0,1,3,6,9  Failure time, Log[hrs]  Failure time, Log[hrs]   Failure time, Log[hrs]  Failure time, Log[hrs]  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2971a878-d56e-4c53-a635-e4c49889509c/2971a878-d56e-4c53-a635-e4c49889509c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=abe68f92bdb3dd836ea3c92b954547f9cb0ae638)
Difference between 2- and  3-parameter LogNormal:  -- sensitive to   and  $\mathsf{X}_{o}$    -- Higher  , clearer   bending down

## Failure Time Projection  

•  EM Lifetime Projections  (single mode LogNormal)         -  From stress conditions ( j stress ,  T stress ) to use conditions   $({{j}_{u s e}},\mathrm{~}{{T}_{u s e}})$  :

![H  1  1 j  (    ) TTF  = MTF    MTF  (  stress  stress  ) n e  k  T Luse  use  T Tstress  stress  e eeo  Z se  use  str&ss  stress  j .se  use Acceleration  Acceleration   Distribution  Distribution  t  ( 1 )  [ Z H (  1 1     1  )] j    Istress  j  (  50 50 stress  stress  )  n  e  n  nk  T use  use  Tsiress  T stress Inmax  max  stress  t lifetime  lifetime ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/42921709-59bb-4062-8dda-20f010da5f95/42921709-59bb-4062-8dda-20f010da5f95.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=ce26c36d4f9818395e72b99d1bc3fdc8e15583b7)
Z – Z-score from test  structure failure target, not  chip failure target     Z   failure probability  per metal line (for a simple  EM structure) at end of life     e.g. Z=-3.09   CDF  =0.1% per metal line, not  per chip, unless only one  metal line per chip has EM  concerns.

## Failure Time Projection  

•  EM Lifetime Projections  (single mode LogNormal)         -  From stress conditions   $(j_{s t r e s s},\;T_{s t r e s s})$   to use conditions   $(j_{u s e},\,T_{u s e})$  :

![AH  H  1  1 j  (    ) TTF  =MTF    MTF  (  stress  stress  ) n e  k  T Zuse  use  T Istres  stress  e Z use se   stress  stress  j use  use  Acceleration  Acceleration   Distribution  Distribution  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c4226a02-14c4-42ee-81be-273d7213d3f3/c4226a02-14c4-42ee-81be-273d7213d3f3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=4fb79eb15b8d5c817e91b905af2a25053f0c5642)
-  Very sensitive to  H, t 50  &     \*    sensitivity depends on Z       how far down on percentile       tighten process variations,         greatly help tightening     For higher Jmax or longer lifetime:  Longer  t 50  Smaller

![1.2 N.2  Above  Red line  Above Red line  1.0 7.O  Sigma   0.8 0.8   Jmax < target  Jmax < target  sigma  Range we typically  Range we typically  06[work with  0.6  work with  Below Red line  Below Red line  0.4  0.4  Jmax > target  Jmax > target  0.２  0.2 10  10O  100  1000  1000  t5o, hrs  t 50 , hrs  t50, hr ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4e1514f8-ca40-474f-9880-2a632537f1fd/4e1514f8-ca40-474f-9880-2a632537f1fd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=eb643a1f58e29f41832da3b3e40e3585e01d319f)
## Outline  

•  Introduction       -  MOL/BEOL architecture     -  Reliability Fundamentals

•  BEOL/MOL Reliability Mechanisms          - Electromigration (EM)          -  Stress Migration (SM)         -  Thermal Fatigue/ Thermal Cycle (TC)         -  Low K Time Dependent Dielectric Breakdown (TDDB)

•  Reliability Challenges with Technology Scaling

-  Dimensional Scaling      -  Material Scaling      -  BEOL Reliability Challenges      -  MOL Reliability Challenges

•

Summary Remarks

## SM Introduction  

•  Stress Migration (SM) or Stress Induced Voiding (SIV)       -  Mass transport due to stress gradient (thermal mismatch)

![•  SM vs EM Failure  SM vs EM Failure   α= 17 ppm/K  E = 120 GPa      -  Metal transport to form  - Metal transport to form     voids or extrusions  voids or extrusions   (a) After Cu     → both thermally accelerated    both thermally accelerated   CMP (25°C)      -  Driving force:  - Driving force:   SiO，   E = 70 GPa  α= 1.1 ppm/K         EM: EM: electron winds   electron winds          → applied externally   applied externally   (b) during SiN  deposition     SM: SM: stress gradient due to   stress gradient due to   (400°C)     difference in TCE of different  difference in TCE of different  SiI-   layers and process/use  layers and process/use     temperatures  temperatures   (c) after SiN   Voids  deposition   relieve         → built internally   built internally   (2S°C)   stress                Gambino, IRPS Tutorial 2010  Gambino, IRPS Tutorial 2010  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/91bfe709-9626-4f76-9d2d-574194a5c610/91bfe709-9626-4f76-9d2d-574194a5c610.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=1dfc01a2f643e6ecdb3b9f3cbab186f8546d762f)
![Al Lines  Al Lines  M2 V1 M2  Cu  M1  Cu  Sm Voids  SM Voids  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ebd1f100-bd9d-4f87-bf40-eaa5ad03e727/ebd1f100-bd9d-4f87-bf40-eaa5ad03e727.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=4c32061ca0939ecaf6cf8cee452cf675fac78b99)
## SM Acceleration  

## •   SM Acceleration 

-  Vacancy diffusion process driven by stress gradient

\*   Two competing factors for void growth       -- tensile stress   temperature difference from “zero stress”       -- mobility   thermal          Peak (sweet spot) for acceleration     -  Challenge for reliability evaluation      \*  Very limited widow for acceleration               -- Temperature is the only knob      \*  Often hard to generate sufficient failures       for modeling

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d754c844-8400-4496-9704-0e171b2afa47/d754c844-8400-4496-9704-0e171b2afa47.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=65782da710a5336f43cb2cc26834ec5e7e8c0b85)
![Stress:ox   （7.-7）"  Voiding Rate = A(T - T)" exp  Mobility:u  J. McPherson,  J. McPherson,  Temperature   IEEE 2007 CICC  IEEE 2007CICC  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f604cf9e-2620-4660-940d-f669f0e5161f/f604cf9e-2620-4660-940d-f669f0e5161f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=903f8aa7a1e06a1e8eb7a04c3276abec8df3e6d2)
## SM Control  

## •  SM Controlling Factors  

-  Stress Gradient and Mobility       \* Process sensitivity causing higher stress           -- Cu Cap deposition (Can change T 0  and T crit )           --  Material property (modulus, TCE…)           \*  Process sensitivity causing fast diffusion path          -- Cap/Cu, Via/Line, liner/Cu interface          -- Geometry sensitivity   local high stress  -   Vacancy Sources  \*  Grain growth, grain boundaries  \*  Defect, poor Cu fill, process damages     -   Geometry Sensitivity         \*  Stress gradient         \*  Active diffusion volumes         \*  Via redundancy

![Plate Below  PlateAbove  Void underneathvia  Void within via  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f56e03d2-419d-48bf-acdd-c6f5773c4828/f56e03d2-419d-48bf-acdd-c6f5773c4828.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=13ce3b8b5502205d94d051e1ff36968ef0a9b3b5)
Hommel, IRPS 2006

Fischer et al, IRPS 2007

## Outline  

•  Introduction       -  MOL/BEOL architecture     -  Reliability Fundamentals

•  BEOL/MOL Reliability Mechanisms          - Electromigration (EM)         -  Stress Migration (SM)          -  Thermal Fatigue/ Thermal Cycle (TC)         -  Low K Time Dependent Dielectric Breakdown (TDDB)

•  Reliability Challenges with Technology Scaling

-  Dimensional Scaling      -  Material Scaling      -  BEOL Reliability Challenges      -  MOL Reliability Challenges

•

Summary Remarks

## TC Introduction  

## •  Temperature cycles   repeated cyclic plastic deformation  

-   A fatigue process          -  Common damage to interconnect   delamination          -  Not commonly seen from wafer level stresses          -  Critical for CPI (chip –package interaction)          -  Adhesion and stack TCE mismatch are key factors          -  Commonly used model:              Modified Coffin-Manson eqn:  N    Kf  m /1(  T ) n [ e H  / 3 k B T max  ] N – number of cycles to failure;    n – cyclic strain exponent    f --  Cyclic frequency

IPFA2019, B. Li

![TC caused  TC caused  delamination  delamination  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e33cc730-d185-4b48-919f-7ccffee2733a/e33cc730-d185-4b48-919f-7ccffee2733a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=8e4abfa0a98fa4746b3e8c45efa2c18b767edfc6)
![TC caused via  TC caused via  shearing  shearing  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ccfd6cfd-e031-4523-873f-1ad60020ce8d/ccfd6cfd-e031-4523-873f-1ad60020ce8d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=c0543cd1d44aff5287737e0135724eb6fcfd1aed)
## Outline  

•  Introduction         -  MOL/BEOL architecture       -  Reliability Fundamentals    •  BEOL/MOL Reliability Mechanisms          - Electromigration (EM)         -  Stress Migration (SM)         -  Thermal Fatigue/ Thermal Cycle (TC)          -  Low K Time Dependent Dielectric Breakdown (TDDB)    •  Reliability Challenges with Technology Scaling         -  Dimensional Scaling        -  Material Scaling        -  BEOL Reliability Challenges        -  MOL Reliability Challenges    •  Summary Remarks

## TDDB Introduction  

•   Time Dependent (Low K) Dielectric Breakdown -- TDDB       -  An electric field or electron-energy driven wear out mechanism         \* Cu diffusion accelerates breakdown    Very controversial, jury is still out

•  The most dynamic area among  the BEOL wear out mechanisms      -   Experimentally, similar observations     -  Quite different interpretations and     projections          \*  Breakdown process          \*  Acceleration model          \*  Distributions model

![Dielectric  Dielectric   Cu Line  Cu Line  Via top to line  Via top to line  Cap   Cu Via  CuVia   :Iiner  Liner  Via bottom to line  Via bottom to line  Cu Line  Cu Line  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/370fe9d8-4ade-47b3-b938-a11695e17442/370fe9d8-4ade-47b3-b938-a11695e17442.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=7083d9c5ac00aa08375f6535be1b871466d0018e)
Intra-level dielectric  breakdown

breakdown

## TDDB Acceleration Models  

## •  Voltage/E-field acceleration  

E-model    $t_{B D}=A_{r}e^{-\gamma_{_{E}}E}=A_{r}e^{-\gamma_{_{V}}V}$  Square Root E-model    $t_{B D}=B_{r}e^{-\gamma_{_{E}}\sqrt{E}}=B_{r}e^{-\gamma_{_{V}}\sqrt{V}}$   $\begin{array}{r l}&{\mathsf{w e r\;L a w\;M o d e l}\quad t_{B D}=C_{r}(\frac{E}{E_{0}})^{-n}=C_{r}(\frac{V}{V_{0}})^{-n}}\\ &{\mathsf{p a c t\;D a m a g e\;(L u c k y\;e)\;t_{B D}}=\frac{D_{r}}{E}e^{\left(-\frac{\beta}{K T}\sqrt{E}+\frac{\alpha}{E}\right)}}\\ &{\mathsf{\bar{E}}\!-\!\mathsf{m o d e l}\quad t_{B D}=G_{r}e^{-\gamma_{\varepsilon}\frac{1}{E}}=G_{r}e^{-\gamma_{v}\frac{1}{V}}}\end{array}$

g V  – voltage acceleration parameter   g E  – field acceleration parameter

![Wu, IRPS2015  Wu,IRPS2015  exp(1/V)  exp(-vV)\~exp(-↓E)  exp（-V)  Stress Window  Stress Window  Applied V or E  Applied V or E   44  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7030151c-c810-4fad-82c7-122809cb6e60/7030151c-c810-4fad-82c7-122809cb6e60.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=20247c8af2fadb08ae177872ade3cc68ba803f5b)
•  Voltage/E-field acceleration     - Regular stress failure times:              -- minutes to 1000hrs      -  All models fit the stress data well      - Order of magnitude difference           projecting to use conditions      -  Need years of stress data to            confidently distinguish    - Root E & Power Law – the two   most popular models for MOL &   BEOL TDDB    -  While we live in linear time dimension, many of the   reliability mechanisms, including TDDB, are in   logarithm time dimensions

![14%fails Emodel 10 RootE 73%fails PowerLaw 102  ImpactDamage 10V  1overRootE 1E 11V 10 10Y  14V 15V 10 16W 102  180 19W 0.25  0.30  0.35  0140  0.45  0.50  0.55 Field(V/nm） ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0e9fd5dd-e022-4ff3-9b67-ee42d8a2d154/0e9fd5dd-e022-4ff3-9b67-ee42d8a2d154.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=07bcf19e748837fe8f515895fbed2a7e27a2243f)
Liniger, IRPS2015

## TDDB Acceleration Models  

## •  Thermal (temperature) acceleration  

$$t_{B D}=M_{r}e^{\frac{-\Delta H(E)}{K T}}$$
• Arrhenius thermal  acceleration is  generally accepted

• Activation energy  H(E) decreases  with E-field (or V)  increase

![VGCV):   口3.6  3.8  3.   .  3.2  3.4  44.0  2.0   2.4   2.8   3.2  1000/T（1/K)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0a4fd75f-0a32-4638-90d2-004938157122/0a4fd75f-0a32-4638-90d2-004938157122.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=9203548144b08100dc89007e20f55850526be2ec)
![11 1.59-0.021\*V 10 0.8 07 06 0.5 25  30  35  4D  45  50 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4fcea69b-2ff0-4b83-9c39-4970e4d32e2d/4fcea69b-2ff0-4b83-9c39-4970e4d32e2d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=ef525fb6c3d6579a1a379f3a3394b8e512048f2f)
Gate Oxide (SiO2)  Slope decrease with Vg increase  E. Wu, Solid-State Electronics, 2002

Low K Dielectric

Chen, IRPS 2006

## TDDB Failure Time Distribution  

• Historical Weibull vs Longnormal Debates         \*  Weibull for weakest link             vs Lognormal with growth component         \*  Weibull widely accepted for  $\sf t_{b d}$   distributions  ns   CDF:    $\begin{array}{l}{{f_{W B}(t)=\displaystyle\frac{\beta}{\eta}(\frac{t}{\eta})^{\beta-1}e^{[-(\frac{t}{\eta})^{\beta}]}}}\\ {{F_{W B}(t)=1-e^{-(\frac{t}{\eta})^{\beta}}}}\end{array}$   Weibit:    Ln[-Ln(1-F  $\mathsf{L}\mathsf{n}[\cdot\mathsf{L}\mathsf{n}(1\!\!-\!\mathsf{F}_{\mathsf{W B}})]=\!\!\beta\ln\frac{t}{\mathsf{n}}$

![33 一 1000 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cdc8a39e-9e2c-4245-9ca0-3a32b89839c0/cdc8a39e-9e2c-4245-9ca0-3a32b89839c0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=9ec8756cda3f3c93db8ff0b129aa9d2b068c142e)
$(t_{\mathrm{bd}})$

• Weibull distribution is for single random variable       \*  Theoretically,   $\sf t_{b d}$   follows Weibull only for samples     with uniform spacing

## TDDB Failure Time Distribution  

-  Weibull is for single random variable       \*  For BEOL, spacing variation is significant         - die to die         - structure to structure within the same die,         -  spacing variation within structure           A final composite distribution             Two random variables: t bd  and s

A major challenge for t bd  distributions  with non-uniform spacing

![Composite  Composite  distribution  distribution  Distributions for each  Distributions for each  uniform spacing  uniform spacing  t bd  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c055291b-cc2e-46d0-9501-298fad187ec4/c055291b-cc2e-46d0-9501-298fad187ec4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=6f85ceeb18951668d02cec82d2d619b0c3313d3f)
48

![•  Line-line, Line-via spacing variations  Line-line, Line-via spacing variations   Vx to Mx overlay  Vx to Mx overlay  \* Critical Dimension (CD) Variation  \* Critical Dimension (CD) Variation  Mx+1  V×+1  \* Overlay/Alignment tolerance  \* Overlay/Alignment tolerance   Mx to Mx-1 overlay  Mx to Mx-1 overlay  \* Line Edge Roughness (LER)  \* Line Edge Roughness (LER)  Vx   Vx-1 to Mx-1 overlay  Vx-1 to Mx-1 overlay  Mx top CD  Mx top CD  Vx top CD  Vx top CD  Mx  VX  Vx-1  Mx CD  Mx CD  Vx cD  Vx CD  Via Misalignment  Via Misalignment   Line Edge  Line Edge   Mx-1  Roughness (LER)  Roughness (LER)  Example of via-line spacing variation  Example of via-line spacing variation  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e94e0c43-4ddc-47be-86d6-5de79ea9ee99/e94e0c43-4ddc-47be-86d6-5de79ea9ee99.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=7543a443407f24fe41f2abf8dbe2a44d1ed71cb9)
## •  Lifetime Projections with Non-uniform  $\mathbf{t}_{\mathfrak{h d}}$   Distributions   

- Integral method for all individual distributions

For discrete spacing distributions

$$F_{t o t a l}=\sum_{i}p_{i}F_{i}\left(s_{i}\right)$$
For continuous spacing distributions

$$F(t)=\int_{s_{m i n}}^{s_{m a x}}\!p(s;\mu,\sigma)F\big(t;\boldsymbol{\upeta}(s),\beta(s)\big)d s$$
-- spacing distribution, p(s;  m ,  );  m  = mean,   = deviation  -- TDDB failure CDF with spacing,  $\mathsf{F}\big(t;\boldsymbol{\upeta}(s),\beta(s)\big),$           (s) – t 63  variation with spacing;   $\upbeta(s)-\upbeta$   variation with spacing  --  Area scaling, could be very complicated

![Composite  Composite  distribution  distribution  t tbd  bd  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cf73adc5-4543-48d7-8f05-0dd6cb3aee1e/cf73adc5-4543-48d7-8f05-0dd6cb3aee1e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=4aa55d27084851ae778f201ee36a4af37dd1baa5)
Distributions for each uniform  spacing

## •  Lifetime Projections with Non-uniform t   Distributions   bd 

- Time Dependent Clustering Model

\* Inspiration from Clustering yield model:

)

𝛼

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5251863f-db25-4be6-81cc-f7cc86db21fd/5251863f-db25-4be6-81cc-f7cc86db21fd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=e98492f8e63b4b4fb23bf00f2ba870be762671f2)
A – area; D – defect density

\*   Introduce time-dependent variable:

$$A D=(\frac{t}{\mathfrak{n}})^{\beta}$$
\*   The clustering model

$$F(t)=1-(1+\frac{1}{\alpha}(\frac{t}{\eta})^{\beta})^{-\alpha}$$
a  – clustering factor;  a  small, less uniform  a   ∞  , Clustering   Weibull

![Weibuw   1054.0  0-1.0  (0)00]  0=0.2  ((-L)uT-)u   m=10s    B=1.5  Weibull restores in  low percentile  4.E-01   1.E+01   1.E+03   1.E+05  Time (s)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ea0cfed3-3aeb-4c77-8e9c-c153b2f591eb/ea0cfed3-3aeb-4c77-8e9c-c153b2f591eb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=c45e4b90a1fdfd29f8762f6ac81207ca7b9a03f4)
## TDDB Area Scaling  

## •  Area Scaling  

-  Scale CDF or lifetime from stress area to application area

-  Poisson area scaling (Weakest-link)

−𝐴𝐷

𝐹= 1 −𝑒

$$F_{2}=1-(1-F_{1})^{\frac{A_{2}}{A_{1}}}$$
so called “vertical shift”

![Area(cm2):  410-3   =1-（1-F)  410-4  -  Verticalshift  \~800  samples   Area-scaling  Tox=2.67 nm   Weibull plot  0=0.003nm  -10  1.E-02   1.E+00   1.E+D2   1.E+00   1.E+02   1.E+04  Time (s)   Time (s)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a26e846b-d9cf-4969-8f17-b5b45ecd4ed1/a26e846b-d9cf-4969-8f17-b5b45ecd4ed1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=cf78aefc3d1e65c1b31cf90ec0e58b08eaff1999)
distribution

$$\begin{array}{r}{\eta(A_{2})=\eta(A_{1})(\frac{A_{1}}{A_{2}})^{\frac{1}{\beta}}}\end{array}$$
Wu, IRPS 2015

Poisson area scaling     --  all distributions merge to a universal line after area normalization

## TDDB Area Scaling  

## •  Area scaling for non-uniform distributions  

-    With spacing variations, area scaling may not follow simple Poisson              distributions not merge to a single line after area normalization

- Area scaling provides  alternative ways to  check selfconsistency    - Appropriate area  scaling is important  for “accurate” lifetime  projections

· Clustering model restores Poisson area scaling at low percentiles with the assistance of small area (Aret)

![F, =1-(1-F)A2/A  Poisson model  Clustering model  533k  [-L)u-]   一  53H  5.3k  0=0.6  +533K  B=2.82  -5   +53k   -15  ·5.3k   : 0.001k  CES  1.E+02   1.E+03   1.E+04   1.E+05   1.EH06   1.E+01   1E+\$2   1E+0s   1.E04   1.EHgs.   1.E+06  Time (A ul]  Tnne (s)  Wu, IRPS 2015  Wu, IRPS 2015  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0709a8a2-3395-42e2-bb8b-9e32a6dec8f7/0709a8a2-3395-42e2-bb8b-9e32a6dec8f7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=4fd5ad1484c4aa4c50fe0511f3aab205f819545b)
## TDDB Progressive Breakdown (BD)  

## •  A few words about multiple SBD (Soft BD or Nucleation) and Progressive BD 

Independent & random multiple BD events

Multiple competing progressive BD

Localized BD events  Progressive BD/unstable SBD

Extensive studies in FEOL on  Progressive and multiple BDs

Courtesy:  Ernest Wu

## TDDB Progressive Breakdown  

## •  Defect Nucleation and Growth Model  

See TSMC (Lee & Oates) & IMEC (C. Wu, et al) publications in IITC & IRPS 2016 & 2017

![10-5  Small Structure  Small Structure   Large Structure  Large Structure  Defect  Growth  Defect   Defect   10  Defect  Nucleation   Growth   10-  Nucleation  10  11-0-10   167r  16  0  10-13   101  10-14  Cu line length, L= 80um  -15   Cu LineLength L =8000um  20714  Timme   S. C. Lee  S. C. Lee   Time  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/db9638a3-e0c9-4f82-94b2-5d2254d2b302/db9638a3-e0c9-4f82-94b2-5d2254d2b302.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=de1a150e75750d2af899b703eca7428d3e991881)
Separate breakdown time   $(\mathsf{t}_{\mathsf{H B D}})$   into 2 segments: nucleation and growth time   $\mathsf{t}_{\mathsf{H B D}}=\mathsf{t}_{\mathsf{n u c l}}+\mathsf{t}_{\mathsf{g r o w}}$

##  TDDB Progressive Breakdown  

## •  Defect Nucleation and Growth Model  

- The concept & statistics for > 17 years for FEOL TDDB             Soft & Progressive breakdown     ____-__Basic Characteristics:            \* t nuc  or t SBD  follows Poisson area scaling           \* t grow  or t PBD  is area independent   (vm)        -  Still not applied in main stream for FEOL TDDB            \*  Complexity in stress and projection         -  BEOL Proposal (S. C. Lee et al)            \* Take full advantage of area scaling              NO area scaling for t grow           \* For small macro stress               t nuc  comparable to t grow           \*  Project to product area              t grow  >>> t nuc     IPFA2019, B. Li    •  Defect Nucleation and Growth Model  -- Challenges     ____-__Stress Challenges           \*  Large Macro                  high leakage, hard to determine t growth                 high possibility to have multiple nucleation (soft BD) spots (multiple BD)          \*  Small Macro                 Nucleation time long, very long stress time needed          \*  Multiple stage stresses                 Determine where/when to switch from high V to low V stress       -  Projection Challenges (for the BEOL proposal)          \*  Fundamental assumption:  Single nucleation spot               -- assumes low percentile with single nucleation spot          \*  Multi- nucleation spots, the 1 st  nucleated one may not be the one causing HBD          \*  To watch/consider               To ensure single nucleation spot: t nuc  >> t grow               The BEOL proposal at product area: t grow  >> t nuc     IPFA2019, B. Li

![1000  Current-based  10:0:   1nm nFET  at 2.4 V  PBD  1st SBD  0.1   10:0:   1000   10000  Time (s)  Linder, et al, EDL 2002  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fba526f3-ac77-4287-a9c9-1bb158e69acf/fba526f3-ac77-4287-a9c9-1bb158e69acf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=4730e9dd77f0dac099864ead192521c50ecb9bca)
## BEOL Reliability Mechanisms: Summary  

•  Two requirements:     \* Place elements where they belong     \* Keep them where they are placed  •  Two considerations for design:     \* Stay within the I, V & T limits     \* Control the hot spots  •  Two factors for reliability:     \* Adhesion between layers     \* Migration of elements

![Dielectric  Dielectric   Cu Line  Cu Line  Cap   Cu Via  Liner  Liner  Cu Line  Cu Line  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e9bf0b86-3be7-40ce-83c6-d82050dfd4c5/e9bf0b86-3be7-40ce-83c6-d82050dfd4c5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=ddc3583124b5e199c73bc022304c4318a53774d5)
![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2f2f7ef9-423c-4323-952e-1b3c072e4921/2f2f7ef9-423c-4323-952e-1b3c072e4921.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=2625f533c3136cb00361a1365e056450d73ab795)
TDDB Concerns  EM/SM Concerns  TC/CPI Concerns

## Outline  

•  Introduction         -  MOL/BEOL architecture       -  Reliability Fundamentals    •  BEOL/MOL Reliability Mechanisms          - Electromigration (EM)         -  Stress Migration (SM)         -  Thermal Fatigue/ Thermal Cycle (TC)         -  Low K Time Dependent Dielectric Breakdown (TDDB)    •  Reliability Challenges with Technology Scaling         -  Dimensional Scaling        -  Material Scaling        -  BEOL Reliability Challenges        -  MOL Reliability Challenges    •  Summary Remarks

## Technology Scaling for Modern Interconnect  oeanig  

![Double pattering   SAQPDD   seni  damascene  SYICUH  spin  PMD  LELELEMI   SADPDD  LELEVia  SAC  22/20nm   14nm   1onm   MO  OFIC  7nm   5nm   3nm   3n  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/019bd2f6-2b22-4cc1-85f9-4299b4ee9d95/019bd2f6-2b22-4cc1-85f9-4299b4ee9d95.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=a5dee8eac358024b9b0a4b7a7544fdbe401b057e)
Tokei, IITC2016

60

## Technology Scaling  

## •  System scaling  

• Architectural innovation:     -  2.5D, 3D, chip stacks     -  Multiple cores

• Hierarchical wiring for on chip interconnects       - Local interconnects       - Mixed pitch & metallization     highly integrated chips/systems

## •  Material scaling  

• New materials for performance, reliability and yield      More suitable electrical, mechanical, thermal and chemical properties

## •  Dimensional scaling  

• For performance and density   cost & power     faster, smaller, tighter, higher density

61

## Technology Scaling  

• Technology Scaling:           -  Driven by performance & cost   \$\$\$          -  Usually, causes reliability deterioration              \*  Innovative integration schemes to minimize reliability deterioration               \*  New models/methodology for more accurate reliability projections

All scaling factors interlocked with positive & negative  feedbacks

62

## Outline  

## •  Introduction   

-  MOL/BEOL architecture     -  Reliability Fundamentals

•

BEOL/MOL Reliability Mechanisms          - Electromigration (EM)         -  Stress Migration (SM)         -  Thermal Fatigue/ Thermal Cycle (TC)         -  Low K Time Dependent Dielectric Breakdown (TDDB)    •  Reliability Challenges with Technology Scaling         -  Dimensional Scaling        -  Material Scaling        -  BEOL Reliability Challenges        -  MOL Reliability Challenges    •  Summary Remarks

## Dimensional Scaling Challenges  

• New Patterning Schemes        Single patterning   multiple  patterning         \*  LE  LELE   LELELE   SADP   SAQP   EUV         \*  Higher # of masks per level until EUV         \*  More process steps & more layers            higher cost & process variability    • RC Increase         \*  Size effect   Cu resistivity increase        \*  Smaller spacing               inter & intra-metal capacitance increase        \*  RC increase can negate most of the            performance gains from device scaling

64

![15  p = p(Bulk+impurity) + g(mv,_/(ne))/A  FRU  Ru   p/ = mv/(Ne) (10²Q-nm)  Cu 6.61  Co8.9712  Ru 7.113  Co  Liner   Ps + Pimpurity   Cu  Tam   6.8 + 0.2   11 +0.5  TTN   6.1 + 0.2   11 + 0.4  Tam   13+0.1   11 +0.5  1000   10000  Cu ,  Co  or  Ru  Area (nm 2 )  Cu, Co or Ru Area (nm2)  C.K. Hu, IITC2017  C.K. Hu, 1TC2017  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a82445f1-dd0b-49ea-964c-f1d8f9cccd5d/a82445f1-dd0b-49ea-964c-f1d8f9cccd5d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=c2f5895f4459dc61de8493b9379a42e31c80ce09)
## Dimensional Scaling Challenges -- Patterning  

![一  •  Double Patterning Solutions  Double Patterning Solutions   Pitch Split:   Pitch Split:   1stTrenchLitho    - Patterning same level multiple times  - Patterning same level multiple times        → Achieve finer pitch   Achieve finer pitch   EtchTrench    -  Extend DUV capability  Extend DuV capability  2ndTrenchLitho    -  Litho-Etch (LE)  Litho-Etch (LE) →Litho-Etch-Litho-Etch (LELE)  Litho-Etch-Litho-Etch (LELE)  Etch2ndTrench  - Challenges:  - Challenges:     \*  Overlay tolerance control    Overlay tolerance control   MainEtch     \*  CD variation between different   CD variation between different     colors (litho sequence)  colors (litho sequence)     \*  Preferred vs non-preferred orientation   Preferred vs non-preferred orientation  Design Layout  Design Layout   On Wafer  On Wafer  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8cb338cf-aec7-4440-8421-39954ad82698/8cb338cf-aec7-4440-8421-39954ad82698.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=49a870fa59ad2181a09056b33ddcc5c9f980672c)
## Dimensional Scaling Challenges -- Patterning  

•  Sidewall Image Transfer (SIT)       Aka:  Self Aligned Double Patterning (SADP)  - Define metal lines as Mandrel and   NonMandrel  - NonMandrel lines defined by sidewalls  of Mandrel lines  - Cut/Block to define line ends & larger  spaces  - Mandrel vs Non-Mandrel CD variation  - Cut mask control & line-end/corner effects  - Spacing & orientation limitations

![TsrLitho  SpacerDep  SpacerEtch  2ndLitho  MainEtch  Mandrel  Mandrel   Mandrel  MandrePNon-Mandre  Non-Mandrel  Design Layout  Design Layout   On Wafer  On Wafer  66  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cea84007-6ee8-410c-8387-df7df72f3dd8/cea84007-6ee8-410c-8387-df7df72f3dd8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=055c04090277dcdb9d50e325af9e13ac3cdfbdfc)
## Dimensional Scaling Challenges -- Patterning  

•  EUV Patterning        - MOL & Selected BEOL layers @7nm node       -  Back to single pattering       -  Simplified mask and design       -  Output & manufacturing maturity

## Dimensional Scaling Challenges – Performance and Reliability  

![Resistance  (n/)   2000  2021  2019  200  k2017  Time  Time  +2015  20  1O   20   30  line width (nm)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/18a68904-b04d-4016-a5c9-c1872b5803b1/18a68904-b04d-4016-a5c9-c1872b5803b1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=6f40095b23b1c9693d166c83c988add4da6b9182)
• Three trends with scaling:

Resistance     TDDB lifetime    EM lifetime

##  New material and process  innovations needed  

IPFA2019, B. Li

![EV  EM  10  Trench mode  (-n'e) os1   Slit mode  Time  Time  Technology node (nm)   Oates IRPS 2012  Oates IRPS 2012  TDDB  TDDB  Experimental data (K=2.6)  Model prediction  Model  YNE  =t。(L/a。)  163  Time  Time  T=125C, E = 6 MV/cm   Lee IRPS 2014  Lee IRPS 2014  20   40   60   80   100  Line - Line spacing (nm)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/992d560b-0db8-4fd1-a597-a04e3132a1f6/992d560b-0db8-4fd1-a597-a04e3132a1f6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=05a6396d706508102d63b35ebf57607d3307c37b)
## Outline  

•  Introduction         -  MOL/BEOL architecture       -  Reliability Fundamentals    •  BEOL/MOL Reliability Mechanisms          - Electromigration (EM)         -  Stress Migration (SM)         -  Thermal Fatigue/ Thermal Cycle (TC)         -  Low K Time Dependent Dielectric Breakdown (TDDB)    •  Reliability Challenges with Technology Scaling         -  Dimensional Scaling         -  Material Scaling        -  BEOL Reliability Challenges        -  MOL Reliability Challenges    •  Summary Remarks

## Technology Scaling – Materials Innovation  

![11Elements  980s]  +4Elements  1990S1   +45Etemeants  [2000s]  Now elements on a chip almost cover 2/3 of  ements on a chip almost cover 2/3 of  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7ba95eef-732b-44cc-a595-28fcca439e1e/7ba95eef-732b-44cc-a595-28fcca439e1e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=192c203b421d2d7addcb7e3499ac537457646bb5)
P. Besser, Semicon Korea, 2014

the periodical table

IPFA2019, B. Li

70

## Technology Scaling – Materials Scaling  

## Materials scaling   

__ - Metallization__          To overcome Cu resistivity increase with dimensional scaling            \*  liner scaling to increase the relative volume of Cu                Thinner liner or linerless                  Replacing TaN with Ta nitridation                 Replacing Ta with Co, Ru           \*  Alternate metals               Co is here; Ru & other metals being evaluated               Nano wire               Non metal – graphene, CNT …

Intel’s 10nm Interconnect Stack

|         scaling                CO, SAQP      |T aver|Pitch (mm)|Scalhng|
|---|---|---|---|
|         scaling                CO, SAQP      ||34|0.81|
|         scaling                CO, SAQP      |Contacted Gate|5||
|         scaling                CO, SAQP      |Metal o||0.71|
|         scaling                CO, SAQP      |Metal 1|36|051|
|         scaling                CO, SAQP      ||||
|        SADP                Cuw/      |Metal 2||0.85|
|        SADP                Cuw/      |Metal 3|4|0.79|
|        SADP                Cuw/      |Netal 4||0.55|
|liner  cap|Metal 5||0..51|
|liner  cap|Metal 6|8||
|liner  cap|Metal 6|8|0.53|
|liner  cap|Mletal 7|112|0.70|
|liner  cap|Metal 8|112|10.70|
|liner  cap|etal 9|1 610|0.63|
|liner  cap|Metal 10|1 601|0.63|
|liner  cap||1080|1.0|
|liner  cap|Ti.| 1 1 μm|0.78|


71

## Technology Scaling – Materials Scaling  

## Materials scaling   

-  Dielectric             \*  Low K scaling has been slowing down                  -- staying at K above 2.2               Integration and CPI concerns                 -- integration damage & mechanical strength             \*  Air gap in selected levels/circuits

Intel’s 10nm Interconnect Stack

|T.aver|Pitch (mm)| Scaling|
|---|---|---|
||31|0.81|
|IContacted Gate|5||
|Mfetal o||0.71|
|Metal 1||051|
||||
|Metal 2||0.85|
|Metal 3||0.79|
|Metal 4||0.55|
|Metal 5||0.51|
|Metal 6|81|0.53|
|Metal 7|112|0.70|
|Metal 8|112|10.70|
|Mfetal 9|1 6101|10.63|
|Metal 10|1 601|0.63|
||1080|1.0|
|T1.|1 1 μm|0.78|


Intel IEDM 2017

72

## Modern Interconnect Evolution/Revolution  

Chronicle of Major  Interconnect Material  Changes

Al  Cu @1997    Oxide   Low K @1999

![1000  Al, Al(Cu),SiO2  Al, AI(Cu),SiO2  Fluorine-dopedILD   Copper  0.1   Low-kES,2viasizes   100  Carbon-dopedoxide  uumn   Self-alignedvia   nnn  ThickUpperMetal  PlanarCapacitor   SADP,Airgap  0.01   10  Brain (Intel), IEDM 2016  Brain (Intel), IEDM 2016  001  1990   2000   2010   2020  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c1e5bd7c-744c-4cc3-8860-d905bb132cc6/c1e5bd7c-744c-4cc3-8860-d905bb132cc6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=4fabe1bb98163f08647cf43909922b7d569e5453)
73

## Modern Interconnect Evolution/Revolution  

Chronicle of Major Improvements in Cu Metallization

![ - Metal Cap  - Metal Cap   - Cu-Mn & Cu Al  - Cu-Mn & Cu Al   - Co liner  - Co liner    ht\*W+TODUSA  20 years  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/dc7a748f-cb93-49c9-82d5-7587d241cfe6/dc7a748f-cb93-49c9-82d5-7587d241cfe6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=6ae2a848c37b364bedf645afb1ec11c623d492c0)
Edelstein, IEDM2017  Edolctoin   EDN42017

74

## Outline  

•  Introduction         -  MOL/BEOL architecture       -  Reliability Fundamentals    •  BEOL/MOL Reliability Mechanisms          - Electromigration (EM)         -  Stress Migration (SM)         -  Thermal Fatigue/ Thermal Cycle (TC)         -  Low K Time Dependent Dielectric Breakdown (TDDB)    •  Reliability Challenges with Technology Scaling         -  Dimensional Scaling        -  Material Scaling         -  BEOL Reliability Challenges        -  MOL Reliability Challenges    •  Summary Remarks

## Reliability Challenges with Technology Scaling  

Scaling has always gone against interconnect reliability.  The problems are not new, but grow more acute as the deeper scaling

公

void

![Scaling  Experimental data (K=2.6)   Model prediction   (s aiso   CPI  CPI      TDDB  TDDB  Model  YNE  ts, =t.(L/ a.  Lee, et al, IRPS 2014  Lee, et al, IRPS 2014  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d76083af-cc15-4c3d-abaf-6810b332b95b/d76083af-cc15-4c3d-abaf-6810b332b95b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=5870d6163d7b91cc792492e88e57f284a452580a)
![EM   T=125C, E = 6 MV/cm   Scaling   NO   0   80   100  Line - Line spacing (nm)  EM Lifetime decreases  EM Lifetime decreases   Low K TDDB Lifetime  Low K TDDB Lifetime  with line/via size shrink  with line/via size shrink   decreases with line spacing  decreases with line spacing  >Impactofdimensional scalingonreliability  Impact of dimensional scaling on reliability  >Materials/integration improvement to reverse this impact  Materials/integration improvement to reverse this impact  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/64b922e4-cc00-4572-97ac-b6f27d7ffd83/64b922e4-cc00-4572-97ac-b6f27d7ffd83.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=7a46f62c084799bee300683846fe096859d27286)
NominalDielectricConstant,k

Cohesive strength  decease with K – CPI

concerns

IPFA2019, B. Li

76

![Metallization Improvement for EM  Metallization Improvement for EM  Metal Cap & better liner  Metal Cap & better liner  AI > Cu  Al   Cu   99.9   Cu Alloying  Cu Alloying   cocap  94599015   SicNcap   Cowrap-CuMn0.25%  around  > 110X   Purel  50   10X  1000x  Al(Cu)   CuMno.  T50 = 1.31 Hrs   T50 = 147.7 Hrs  10  J=2.5 E+6 A/cm  Temp =295°C  0.1   10   100   1000:  Time to Failure (a.u.)  Stress Time (Hrs)   OD  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/779e77de-50a6-407a-906f-06331b1be965/779e77de-50a6-407a-906f-06331b1be965.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=a7f51159937436ac998b5490d0a6bfb7b51023c8)
Co liner and Co cap  Dramatic EM  improvement

Metallization improvement greatly enhanced EM reliability

• Dimensional scaling mainly for performance    • Metallization improvement mainly for reliability & performance    • Next major challenge is resistance           Fighting resistance increase is the key for next scaling

77

## Integration Improvement for TDDB   

• TDDB – E field driven         - Operating voltage (Vmax) scales much slower than spacing             E = Vmax/s               E field increases from technology scaling

• Integration Schemes to maximize minimum spacing for each node

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ea103721-3a7b-450a-87ef-92ece64ac338/ea103721-3a7b-450a-87ef-92ece64ac338.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=4b9542f9e8c40d2ebee28d67d0b17c9ed9a2483b)
-  Variability control for spacing variation        -  For BEOL TDDB, Via/Line spacing is the main concern              via-via spacing is usually relaxed        -  SAV (Self Aligned Via) to improve Via top to line spacing           \*  SAV vs Non-SAV direction        -  FAV (Fully Aligned Via) to improve Via bottom/chamfer to line spacing

78

## Integration Improvement for TDDB   

## •  SAV only solves half of the TDDB problem – Along the SAV direction  

![Non-SAV   SAW  SAVViadirection  TDDB  TDDB   Non SAv  SAW!  Non-SAV Via direction of SAv  Non-SAV Via direction of SAV  一  1.E-01 1.E+01 1.E+03 1.E+05 1.E+07  Time (s)  Curtesy of P. McLaughlin  Curtesy of P. McLaughlin  Now along non-SAV direction is the TDDB weak  Now along non-SAV direction is the TDDB weak  spot, need FAV  spot, need FAV  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/335547e1-aaf9-462f-bce4-49085c77db87/335547e1-aaf9-462f-bce4-49085c77db87.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=fa0d0466c3f032a35c51c292f004d948789a1ad9)
79

## Integration Improvement for TDDB   

Recess the Cu  line to allow via  landing and  alignment

![FAV   M×+1  Critical  Critical  spacing  spacing  for TDDB  for TDDB  MX  Briggs, IEDM201  Briggs, IEDM2017  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/679bbe7a-b379-4a0d-a292-a95ea9f6f291/679bbe7a-b379-4a0d-a292-a95ea9f6f291.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=9bff54c934f5f00b644b92e11d8691ec7383db0a)
•  FAV – Control via chamfering for Mx-Vx spacing improvement

80

## •  Dielectric K reduction limited by  reliability  

-  Lower K   more porosity          \*  Mechanically weaker:               cracking, delamination               Major CPI concerns              Air gap only for selected levels & layouts          \*  Lower TDDB breakdown strength          \*   Harder for integration                 the effective K   $(\mathsf{K}_{\mathsf{e f f}})$   reduction is   limited by integration

•  RC reduction now mainly focused on R  reduction

![4.0   Keff  Kbulk  SiO2   SSG  W!   210  3.0   siCOH   30  p-SicOH  20+  2.0  200   150   100   50  node (nm)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/614a2d78-5965-49e9-94c9-ac4acc0b40e5/614a2d78-5965-49e9-94c9-ac4acc0b40e5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=921cf89e498ec10edbebfdc1bbc13e8f294ae95c)
Gambino, IPFA2018

## Scaling Challenges: RC Reduction  

•  Control the rapid R increase w/ scaling is essential        - R increase can negate all performance gains from scaling       - R increase due to          \* grain boundary/surface scattering          \* increase of liner/Cu volume ratio          \* liner @ via bottom for via resistance

![Liner  er  Cu  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7a414d4a-1a2b-4ba6-8e27-edecbbc15ef3/7a414d4a-1a2b-4ba6-8e27-edecbbc15ef3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=ab31e6a8c9707bd2c6d8090af7d82c39dfb21b2e)
![Coremetalwidth   SimpleShrinkLeadsto   LowerLineResistanceOptions  Line Resistance Issues  Notenoughroomforcoremetal   Alternatebarrier   Nobarrier  Copper  AIt  meta  Barrier  Totallinewidth   Total linewidth  L. Zhao. Semicon. Eng.201  L. Zhao, Semicon. Eng, 2017  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7a6fe41d-a9fa-4945-96c3-35d718941122/7a6fe41d-a9fa-4945-96c3-35d718941122.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=8518991d11031147fd0905c36f2a85e2b77168a0)
## Scaling Challenges: RC Reduction on Reliability  

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/41719c9c-aee0-403d-a63d-94e7b7d87a85/41719c9c-aee0-403d-a63d-94e7b7d87a85.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=cdc0b7789091fd88d647a645441a75e79cc2d727)
•  Control the rapid R increase with scaling is essential         - For Cu metallization           \* Most significant button is to reduce liner/Cu volume ratio               For a 4nm thick liner   $@$   bottom & sidewall               Liner/Cu volume = 27% for a line W  $\circeq$  48nm, H=72nm               Liner/Cu volume = 64% for a line W=24nm, H=48nm           \*  Thinning the liner has direct reliability consequences   Sidewall   Void               -- Good liner coverage on trench is essential for good Cu fill                   Sidewall void from poor liner coverage                     Fatal for EM/SM               --  Good liner/Cu adhesion crucial for EM/SM               --  Cu diffusion blocking barrier at via bottom                    Necessity for short length EM benefits       -  Non-Cu with very thin or no liner

Blech effect

•  Variability Impact on EM Lifetime Projection      -   Scaling causes EM failure time   $(t_{50})$   to decrease

Critical void size   $(V_{c})$   smaller           Fast migration path variation        -  Scaling causes relative variation to increase             $V_{c},\,n_{d},\,j_{c},\,A_{s}$    variation increase              increase    -    $t_{50}$   decrease +   increase   double trouble for EM lifetime

$$t_{f_{i}}=\frac{V_{c_{i}}}{A_{s_{i}}\nu_{d}}\approx\frac{K L_{\nu_{i}}d_{\nu_{i}}w_{i}}{A_{s_{i}}(j_{i}-j_{c i})}$$
![Volume=V  Area=A,  Oates IEDM 2014  Oates IEDM 2014 PureCuCuMn ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7bc11823-3a4b-480e-8d7b-1fda9c899973/7bc11823-3a4b-480e-8d7b-1fda9c899973.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=cac99d2edd5d277753e33ba3c895c286ff4cc472)
![1. 00    PazTTeWION  142232456590130180  Technoloqv Node  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e3b412ae-eebd-44bc-a889-6d8102dfaac3/e3b412ae-eebd-44bc-a889-6d8102dfaac3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=a6da60251107d47a9c1431c561dbd5032c0fab5b)
![99  99 90  90  AAAAAAAA 5C  50  BB B BBBBBBBBBBBB e lit n  10 e  A  B  c r e  1 P 0.1  0.1 0.01  0.01 0.001  0.001 0.0001 0.000'  5  10  10  50.100  50  100  500  500 Time to Fail (hrs)  Time to Fail  (hrs) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e657126f-ceef-46fd-b3c0-9418993a7957/e657126f-ceef-46fd-b3c0-9418993a7957.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=e39737556d1cd5443288aa9176fc9c8dc4652257)
## Scaling Challenges: Variability 

![LineWidth  Technology   Representative Grain Orientation Mapping  nm)  9onm   120  45nm  28nm   AS  22nm  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/23b22f75-b109-491d-9f9e-f4ef09d8268e/23b22f75-b109-491d-9f9e-f4ef09d8268e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=8c4a2f033d430e30f481ee6b5265190f26f364fe)
Grain Size and Distribution with Dimensional Scaling

S-T Hu, et al IEDM2018

•  Variability Impact on EM Lifetime Projection        -  Scaling causes grain growth harder        -  Fine grains   more grain boundaries (GB)              critical void size decrease              faster Cu diffusion path along GBs              decrease metal cap effectiveness       -  Wider variation of grain size distributions           Blocking grain distribution variation                deterioration

![(a) Ideal Bamboo structure  (a) Ideal Bamboo structure  (b) Bamboo dominated structure  (b)Bamboo dominated structure  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5a7ae818-2c18-432f-a938-c6972b378d77/5a7ae818-2c18-432f-a938-c6972b378d77.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=9af665baed0d4cb059bb12e9998a1706fd372c5f)
(c) Polycrystalline dominated structure

Blocking grain

![99  98  CoWP_SG,=0.5  95  CoWP LG, =0.9  90  Cao et al, APL 2013  Ca0 et al, APL 2013  ()  70554320   14×  10  21   330°C,1.03 MA/cm²  Time (a.u.)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e8835088-2ace-4e05-9156-aae0fbb1f260/e8835088-2ace-4e05-9156-aae0fbb1f260.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=51beb610178ed549c4a8d5983911e85bcec9cb5b)
## Scaling Challenges: Variability  

•  Variability Impact on TDDB Lifetime Projection        -  TDDB: a spacing control driven reliability concern              Allowed minimum spacing corner       -  Small spacing             shorter   $t_{63}$   and smaller  \*                Percolation effect      -  Higher variability          CD, overlay control, LER …            spacing distribution even broader            higher TDDB failure probability

\*   For Weibull, larger  , tighter distribution       For LogNormal, smaller  , tighter distribution

An example of TDDB failure impact by t bd  distribution variation ( ) and spacing variation ( )

IPFA2019, B. Li

![999６  6396   LER,Via Overfay  1006  106  rOates IEDM 2014  Oates IEDM 2014  Failure Time  βo=1.5  0 =1.5  βo=z.0  0 =2.0   β0=2.5  0 =2.5  Spacing distribution variation,  Spacing distribution variation, o    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1ae759d0-8a6c-4ec7-a97c-8d5d1a70ed7c/1ae759d0-8a6c-4ec7-a97c-8d5d1a70ed7c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=7d6c656ab51873a2363d3b354445d42e47b12973)
Impact by  $\sf t_{b d}$   variation ( ) and spacing variation ( )

## Scaling Challenges: Variability  

## •  Concerns with New Integration Schemes   

-  Multiple patterning   more variability        -  SADP/SAQP           \*  More masks and process steps                 alignment variability           \*  Block and Cut                 Cutting & line end shapes       - EUV           \*  Fewer masks, better overall variability           \*  Some claims that LER (line edge roughness)               may become worse

![Length=1000m  for k=2.6 dielectric  V=0.75volt  9/6 L\*0  Double patterning   Doublepatterning  'aw i   more alignment  more alignment  variabilitysic Low-k TDDB  variability  Single patterning-TDDB  Double patterhing TDDB  1 0101   5801   E101   1.01   101  Nominal Line-Line Spacing (nm)  Lee, IRPS 2014  Lee, IRPS 2014  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8e6743bb-ba04-4951-a9d2-289369182f0e/8e6743bb-ba04-4951-a9d2-289369182f0e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=e5f632206a37d7f2b90ab0ad635e24e1a5ad66f2)
## Scaling Challenges: Variability  

## Line-edge roughness (LER)  &  TDDB modelling  

- LER/TDDB effect modelled by discrete columns w/  different thickness in competition to BD

![THK:  THK:  30nm  30nm  1.0  1.0  d (u)   d(um)     1.0  1-0   0  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a823253a-a103-495d-8ec8-9f5e16851fad/a823253a-a103-495d-8ec8-9f5e16851fad.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=108bdaf471efe51cd2449f40cfd5511d6e96cffb)
- The nature of LER   reduce the local  ILD thickness   increase E field

IPFA2019, B. Li

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e442beb7-b2b3-4e79-b3aa-0e8da1d1a1b0/e442beb7-b2b3-4e79-b3aa-0e8da1d1a1b0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=e2b8e242a4aeab2cfd708d977e49fc4023d87805)
![TDiel=30nm  T Diel =30nm  3nm  3nm  2nm  2nm  =   1nm  1 nn  1.E-06   1.E-04   1.E-02   1.E+00   1.E+02  Time(a.u.)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6e86833e-428b-430a-8c55-89409f10e3dd/6e86833e-428b-430a-8c55-89409f10e3dd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=0949bd5f81655d65dee065e2a6d2e0b0ffab0b58)
## Scaling Challenges to Reliability – Joule Heating  

•  Joule Heating becomes critical         -   Power density increases             Driven by circuit density & performance         -   FinFets aggravates joule heating             Poorer thermal conduction        -   A portion of the heat transfers from       FEOL/MOL to BEOL        -   2.5D and 3D packaging            Poorer thermal conduction          Major impact on EM                −∆𝐻  𝑡   ∞ 𝑒  𝑘𝑇     𝑙𝑖𝑓𝑒

![Sun's Surface  RocketNozzle  NuclearReactor  Pentiuma  8086  HotPlate  9004   8085  8008  386  286  486  8080  8O   NOSNO  Year  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/52d6bdac-943f-41f2-9c44-6a40e226c2b2/52d6bdac-943f-41f2-9c44-6a40e226c2b2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=27c9b27e1935c52882760a8d8c979c9e6a2198ec)
90

![--1  1..   LOW K TDDB  0.8  0.2   FlectromElatiess Mietation  ..0  Temp Rise. "C  90  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/695077db-7afc-4d2d-b1fa-1c2ab7a4f625/695077db-7afc-4d2d-b1fa-1c2ab7a4f625.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=04f94beaa6b2b767e9101e12634f4859f8e0cbd1)
## Scaling Challenges to Reliability – Joule Heating  

•  Temperature Profile is important        -  Non-uniform temp across a chip        -  Dynamic temperature profile           \* Workload variation          \*  Cooling & environment condition        -  Hot spots          \* In space domain              Active circuits/areas          \*In time domain             High demand period          EM budgeting based on demand

![5  Y  X   s  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a3b06626-134e-48bc-a5e6-2be8e6a008af/a3b06626-134e-48bc-a5e6-2be8e6a008af.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=d84f9e6338da7a0ef29f7de1228bc16b4f141cc8)
Temp Profile Across A Chip

![H  ++++ +++++ + HH++ H++++  HHHHHH  HHHHHHH- +++++++  +丰#：  ++++ ++++++ ++++++++++  主+++  +++  +++++++H +++#+ H++ ++-++  ++++  +H+H+ T++  ++++ +++  HHHH+++  ++H  +++  4++-+ +HHHHH  HHHT  +丰美  + + + 丰+  HHH  +++  +++ ++ +  +++ +HH HHHHH +++  +++++  ++++ +  +++++++  +丰+  + +#  ++  ++++++  ++ ++T++ ++++++ +++±++  +++++  ++  +++++++  ++++++ ++++  H+++  +++ 丰++++手++丰+丰  +++++++++ ++++ HH1  ++++++ H++H Temperaturevariationwithtime ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6c43336e-1fbb-44a7-b656-e4103372acaf/6c43336e-1fbb-44a7-b656-e4103372acaf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=1d13a70c24dfc7438f1bee6d32229b36f8ddbc01)
B. Li, IRPS 2015

91

## Outline  

•  Introduction         -  MOL/BEOL architecture       -  Reliability Fundamentals    •  BEOL/MOL Reliability Mechanisms          - Electromigration (EM)         -  Stress Migration (SM)         -  Thermal Fatigue/ Thermal Cycle (TC)         -  Low K Time Dependent Dielectric Breakdown (TDDB)

•  Reliability Challenges with Technology Scaling

-  Dimensional Scaling      -  Material Scaling      -  BEOL Reliability Challenges       -  MOL Reliability Challenges   Summary Remarks

•

## MOL Reliability  

•  MOL reliability only draws attention recently      -  Historically:

\*  Larger spacing than gate           \*  More stable materials than BEOL               W, Silicide, SiN, TiN, SiO2           \*  Intrinsic reliability not a problem              Main issues   process defects       -  With technology scaling          \*  PC-CA spacing down to a few nm          \*  New materials for lower contact resistance              W   Co or even Cu?

![1  MEO  VO  CBbar  Fn  PC  ST  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f496bd17-fcbc-4d0f-83e9-1c4b85c1b483/f496bd17-fcbc-4d0f-83e9-1c4b85c1b483.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=4a1353f6b81b1c2abccba74165c785f7507f7fb9)
## MOL Reliability – TDDB Challenges  

•  RC Reduction   SAC Cap         -  PC-CA spacing reduction               Double trouble for TDDB           \*  Parasitic capacitance increase              SiN spacer   lower K               Weaker TDDB strength           \*  Smaller spacing   higher Emax       - For advanced nodes           \*  MOL TDDB is one of the most challenging  enging

![C  FC   FC  SD Epi   S/'D Epi  Silicide   Silicide  Substrate  spacer  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/035ef7ce-9acb-4b06-b629-f0c70f710e39/035ef7ce-9acb-4b06-b629-f0c70f710e39.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=f0d428a18763a58d8c0322b637046fc5f6dfca21)
## MOL Reliability – TDDB Challenges  

## •  PC-CA TDDB  

-  Controlling PC-Ca spacing         \*  Nominal spacing important               determines overall distribution               defined by tech node         \*  Lower corner more important               higher Emax               early TDDB fails               defined by process control


![Major  Major  contribution  contribution  to TDDB  to TDDB  failure  failure  PC-CA Spacing   PC-CA Spacing  Teng, IRPS  Teng, IRPS  2019  2019  PC   S  STI  Sdrawn  95  95  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d612fea1-6650-491f-8e50-6813bf3597b3/d612fea1-6650-491f-8e50-6813bf3597b3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=df863eaa00513439f191d05bd56301648520dbd7)
## MOL Reliability – TDDB Challenges  

•  Minimum PC-CA Spacing       -  Controlling process variation          \*  CD control              PC & CA sizes          \*  Profile control              PC, CA tapering          \*  Edge roughness          \*  Overlay/alignment control

![Coho.  O EPi   S/D Epi  Hicide   Silicide  TDDB Challenges  TDDB  Challenges  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6f597c31-3490-475a-9bf8-5785fb38c1e9/6f597c31-3490-475a-9bf8-5785fb38c1e9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=2ff108561484ccb90e237a421019694e38d99042)
## MOL Reliability – EM/SM/TC  

•  New Metallization         - Contact resistance reduction           \*  Co or Cu replacing W           \*  Liner thinning           \*  Metal fill quality in CA    -  Short connections           \*  Benefit from Blech effect for EM        -  EM/SM/TC            \*  “Don’t care”   concern?                  watch and see

![Ioho.  FC   FC  O EPi   S/D Epi  Hicide   Silicide  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9b69a47a-2551-491e-b64d-fc29e2f52e47/9b69a47a-2551-491e-b64d-fc29e2f52e47.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215603%3B1743219203&q-key-time=1743215603%3B1743219203&q-header-list=host&q-url-param-list=&q-signature=5d693cb9586e7fb01884bb5ac8be0e1cb9d5a5e4)
## Outline  

•  Introduction         -  MOL/BEOL architecture       -  Reliability Fundamentals    •  BEOL/MOL Reliability Mechanisms          - Electromigration (EM)         -  Stress Migration (SM)         -  Thermal Fatigue/ Thermal Cycle (TC)         -  Low K Time Dependent Dielectric Breakdown (TDDB)    •  Reliability Challenges with Technology Scaling         -  Dimensional Scaling        -  Material Scaling        -  BEOL Reliability Challenges        -  MOL Reliability Challenges    •  Summary Remarks

## Summary  

• Technology Scaling for performance and density

• While Dimensional Scaling improves density      - New patterning and integration schemes needed       - RC degradation – major challenge      - Reliability degradation – major challenge

• Material Scaling overcomes RC/Reliability degradation & integration complexity      - Better electrical/mechanical/chemical properties

• Contents Scaling improves system level performance      -  More contents & functions      -  More stringent on element level reliability

## Summary  

•  As technology scales, BEOL/MOL reliability challenges become more important    •  New metallization (Co or Cu with Co liner/Co Cap) significantly improves EM         -- Sufficient to counterbalance the dimensional scaling effect    • Both dimensional scaling and new integration schemes impose major concerns   on TDDB         -- No magic process knobs seen to alleviate this concern         -- New TDDB models/methodologies needed for further scaling    • Variability plays a major role for leading edge technologies        -- Variability challenges become a major part of the life for reliability

## Q & A  

## •  Any questions? 

Enjoy the rest of the IPFA !!!  Have great Time!

