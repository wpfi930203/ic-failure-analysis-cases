---
title: "DimitriosIoannou_Reliability of 3D Through-Silicon-Via (TSV) Technologies_ 2019 IPFA Tutorial.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_5acfdde4600e0b190b7dc412a0cbf2407295230462135641
file_size: 3391628
---

## Reliability of 3D Through-Silicon-Via (TSV) Technologies 

Dimitris P. Ioannou, Ph.D GlobalFoundries, NY USA

## Outline 

3D LSI Technologies background

•  Through-Silicon-Via (TSV) applications

TSV Integration schemes

TSV Process flow and considerations

TSV Integrity and potential reliability concerns

TSV induced thermo-mechanical challenges

•  effect on device performance (TSV proximity effects)

•  effect on FEOL/BEOL reliability

Chip Package Interaction (CPI) challenges

Concluding remarks

## 3D IC Background 

3D IC: A “ more than Moore” disruptive technology that  vertically stacks multiple dies with a high density die-to-die  interconnect

Through-Silicon-Via: a key enabling component

## Key advantages: 

Reduction of interconnect length and hence reduction in   interconnect delay     Higher bandwidth/lower power     Rapid access to memory     Wide range of possibilities of heterogeneous integration     Smaller Form-Factor

## Benefits of 3D chip stacking with TSV 

![TsU  C1   2   3   C   2D wires  CS   CA   03  3Dwires   Memory  Processor Core  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f741c2ee-d1bb-47bd-b06e-dad173d92de7/f741c2ee-d1bb-47bd-b06e-dad173d92de7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=367a38ef83f94fe42d5bcbdb6ebb166e17a9a602)
“Memory Wall” challenge:

diverging exponential increase in performance of processors and memory  [1] 3Di presents an excellent solution:

Large chip can be partitioned into smaller blocks vertically stacked:

shorten global interconnect length and hence improve signal propagation  and reduce power.

Multi-core processor architectures are increasingly “hungry” for data Placing memory directly on top of processor:

High density of parallel connections (achieved by finely-pitched TSVs and  optimization of bonding technology) improves data bandwidth  [2]

[1] W.A. Wolfe and S.A. McKee, Computer Architecture News, Vol. 23,No. 1, Mar. 1995   [2] K.N. Chen and  C.S. Tan,  IET Comput. Digit. Tech., 2011, Vol. 5, Iss. 3

## Evolution of 3D IC Technology 

![Analog  FF   Passive  Logic  Memory  Traditional   Silicon Interposer   3Di  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2970ee7c-8d69-4526-a1cf-60f28138470f/2970ee7c-8d69-4526-a1cf-60f28138470f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=1ad04202b340088ba4786f853738b763aa658eac)
Silicon Interposer (2.5D):

Passive silicon with TSVs Enables heterogeneous integration

“Full” 3D:

Active silicon with TSVs   Enables heterogeneous integration   Enables Logic functionality and even higher memory bandwidth

i-Micronews, October 2010

## TSV Si Interposer Application- 2.5D 

![metal connections (micorbumps to TSVs)  Microbumps (access to power/ground/Ios, logic)  Through-Silicon-Vias  C4 bumps  28 nm FPGA slices  (Side-by-Side Die Layout)  SLR3   SLA2   SLRI   SLRO  65 nm passive Si interposer  (no transistors - low risk)  Package Substrate  BGA Solder balls  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9f5cc3cb-c7c9-4817-ac26-48bcbd00333c/9f5cc3cb-c7c9-4817-ac26-48bcbd00333c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=06c952449a4ae3c807daabdb0fb382fcbe5cba79)
## High Bandwitdh Memory (HBM)  Architecture 

![TSV  HBMDRAMDie  Microbump  HBMDRAMDie  HBMDRAMDie  HBMDRAMDie  LogicDie   PHY   PHY   GPU/CPU/SocDie  Interposer  PackageSubstrate  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d2fa37c0-461f-470b-b3c9-099c3965915b/d2fa37c0-461f-470b-b3c9-099c3965915b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=6554d0ee3522bdc67c0a03152d804f2e237f7af4)
HBM is a new type of memory chip with low power consumption and ultrawide communication lanes. It uses vertically stacked memory chips  interconnected by microscopic wires called "through-silicon vias," or TSVs.

Those towers connect to the CPU or GPU through an ultra-fast interconnect  called the “interposer.” Several stacks of HBM are plugged into the interposer  alongside a CPU or GPU, and that assembled module connects to a circuit  board.

Source: AMD

## TSV enabled Hybrid Memory Cube (HMC)  Architecture 

![DRAMLayers  Substrate   LogicLayer  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cce7d72b-6ef3-4008-b26e-378b79be8e51/cce7d72b-6ef3-4008-b26e-378b79be8e51.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=10363a02f1337b76721b53dc754e33132e5f608d)
Hybrid Memory Cube: A revolutionary memory technology that combines  DRAM and Logic into a single heterogeneous package.

At the core of the Hybrid Memory Cube is a small, high-speed logic layer that  sits below vertical stacks of DRAM dies connected through TSVs

DRAM is designed to solely handle data with the logic layer handling all DRAM  control within the HMC.

Source: Micron

## TSV Capability at GLOBALFOUNDRIES 

•  Two separate TSV integration schemes developed in parallel  within GLOBALFOUNDRIES

|Facility/TSV|EFK Fab 10|EFK Fab 10|Malta Fab 8|
|---|---|---|---|
|Facility/TSV|25 |26|rwni 5 |
|Integration Level|Fat Vvire|Fat Vvire||
|Cross Section|2.9Bum|||
|Nodes|32nm, 22nm (SOl)|32nm, 22nm (SOl)| 14nm |
|TSV Diameter|19/8um (OD/ID)|7umm|5u mm|
|TSV Pitch|50umm |50umm |4oum|
|Device KOZ|5umm|5umm|5umm|


Process flows are nearly identical, which enables close unit process cooperation  between Malta and EFK Fabs.

Implementation of best learnings and practices across sites, which leverages  over 15yrs of collective TSV processing experience across multiple nodes.

source:GLOBALFOUNDRIES

## Outline 

3D LSI Technologies background •  Through-Silicon-Via (TSV) applications     TSV Integration schemes     TSV Process flow and considerations     TSV Integrity and potential reliability concerns     TSV induced thermo-mechanical challenges  •  effect on device performance (TSV proximity effects) •  effect on FEOL/BEOL reliability     Chip Package Interaction (CPI) challenges     Concluding remarks

## 3D Integration schemes 

3D Integration is classified into various categories based on the  following differentiators:

Singulation level: chip-to-chip, chip-to-wafer or wafer-to-wafer   •  with chip-to-chip bonding it is easier to achieve high yield by   selecting known good chips •  also can select different sizes for the stacked chips   •  wafer-to-wafer bonding is currently the least mature   technology but it has the potential to further increase the   interconnect density    Stacking orientation: face-to-face or face-to-back stacking   Bonding medium: metal-to metal, dielectric-to-dielectric or hybrid   TSV formation: via first, via middle or via last   •  Via first (TSV introduced before FEOL)   •  Via middle (TSV introduced after FEOL and before BEOL)   •  Via last (TSV is captured at last BEOL level)

## TSV Integration choices 

![Solder  Solder  Passivation  BEOL  N1  FEOL   C  (CMOS)  S  TSVFirst   TSVLast(WL)   TSVMiddle   TSV Last  (Passivation)   (Backside)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3c61354c-3b73-41b1-8b4a-398fc4fc2368/3c61354c-3b73-41b1-8b4a-398fc4fc2368.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=c29a9c42e35d5ad8270ed18d253cfea83213b693)
The choice is a compromise between process complexity of  integrating a high aspect ratio via and the required exclusion  zones for implementation

K.J Moon, AMC 2010-Samsung

## Typical process flow for TSV-middle integration 

![Wafer front side   Wafer back side   Module assembly  Heat Sink  C4 deposition  Build transistors   wafer bonding  and BEOL wiring   to handler   on RDL  Full Thickness Die  01o1o1o1o1o1o1o1o1o1o1o1o1o1o101o1o1o1o1o1o1o  ThinnedDiewithTSVs  dicing stage  TSV processing   backside thinning   die level joining  Laminate  expose TSV  complete  BEOL layers   backside (RDL)   Heat sink  Wiring  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/58b56ff8-255a-4222-80e5-c3a3cce2c23e/58b56ff8-255a-4222-80e5-c3a3cce2c23e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=6cf6041db2a00dbe6f505748b906228a043e645b)
Each one of the integration phases presents its own manufacturing  challenges and possible reliability exposures

## IBM 45 nm 3D module (Face to Back) 

![Full thickness  logic die  w/eDRAM  Thinned logic  Diew/eDRAM  Organic  Laminate  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c53baf85-64ff-4593-8f29-162242d21ce6/c53baf85-64ff-4593-8f29-162242d21ce6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=58986e404d09c13e93cef961efd0de11a50a7cec)
## Close up of IBM 45 nm 3D module (Face to Back) 

![FEOL  &BEOL  —Pb-freeC4  Grind side  TSV  Device side  Thinned Die  --5   FEOL  &BEOL  Pb-free C4  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c29f8d35-7aa8-47c2-a38b-4273a49ecba4/c29f8d35-7aa8-47c2-a38b-4273a49ecba4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=c4cc305bb4b1200c85ce4b610beb7f3e54077a97)
## Outline 

3D LSI Technologies background •  Through-Silicon-Via (TSV) applications     TSV Integration schemes     TSV Process flow and considerations     TSV Integrity and potential reliability concerns     TSV induced thermo-mechanical challenges  •  effect on device performance (TSV proximity effects) •  effect on FEOL/BEOL reliability     Chip Package Interaction (CPI) challenges     Concluding remarks

## TSV Process Flow 

![TSV diameter  dap Ase  Silicon Substrate  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/51b485a3-0c51-41b2-9c52-0c6c874efdc2/51b485a3-0c51-41b2-9c52-0c6c874efdc2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=9b437d00b8f662fc642cea641af639703eb3504f)
![1. TSV etching  (DRIE process on Si)  Oxide depa-Litien  Via filling with Cu  (Cu electroplating)  5. TSV anneal and CMP  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/475258d0-cf93-44fd-919f-6b15efe52880/475258d0-cf93-44fd-919f-6b15efe52880.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=9ecd572542772c0b56a6a0d3c3f69f2d739240c9)
y anheal ang yvl

## SEM images for TSV Process Flow 

![viaetch   barrierseed   CuECDFill   TSVanneal&CMP  oxideliner  50nm  Liner  PMD  STI  TOP   Si  5pm  501ym  47.85ym  48.61um   Middle  55m   Bottom  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fe531290-a128-4b95-b491-c26bafa464da/fe531290-a128-4b95-b491-c26bafa464da.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=f8cf6e1d8170148aa394950f83b35ead7e1fac2b)
## TSV Process considerations 

Metallization of TSVs is becoming increasingly challenging as the  aspect ratios of Vias continue to increase

•  BOSCH DRIE Process

The insulating layer of SiO2 is typically deposited using conformal  chemical vapor deposition (CVD) process on the wall of the TSV •  required to have uniform coverage along the TSV sidewalls

Preparation of a continuous barrier that will keep Cu from diffusing  out of the vias is another critical TSV production step (Via-Liner)

•  deposition of a thin layer to serve as a Cu diffusion barrier (TaN or  Mn 4 N) •  deposition of a smooth and conductive Cu seed layer to initiate Cu  electroplating for TSV filling- void free and full via filling •  physical vapor deposition is often used for the liner formation •  direct-Liquid-injection (DLI) CVD recently demonstrated as a very robust  process to coat high aspect ratio vias with conformal Cu seed layer [1]

## TSV integrity and reliability concerns 

TSV Liner integrity     TSV defects     Cu protrusion     Cu contamination/Mobile ion penetration

## TSV Oxide Liner Integrity 

TSV oxide liner functions as electrical isolation between the TSV Cu  fill and the Si substrate. It needs to satisfy the following requirements:

zero leakage, high breakdown voltage, minimal charge inclusion   low stress/modulus and TSV process temperature compatibility   excellent step coverage and uniformity

Conformality of the dielectric liner is critical in high aspect ratio TSVs  to enable a continuous metal barrier and seed layer coverage which  in turn is critical for the subsequent Cu fill

good step coverage is also critical in avoiding variation in dielectric  thickness which can cause leakage, inconsistent reliability and  inconsistent signal delays through the TSV arrays.

## Room Temperature Atomic Layer Deposition  (ALD) Oxide Liner Characteristics  

A room temperature ALD process for use as a TSV dielectric liner  was developed by GLOBALFOUNDRIES [1]

Process optimization was completed to achieve a 100 nm thickness  of SiO2 liner for high aspect ratio TSV with nearly 100% conformal  sidewall coverage.

Electrical characterization of the ALD dielectric liner showed  breakdown voltage, TSV leakage and capacitance as good as or  better than the Plasma Enhanced Chemical Vapor Deposition  (PECVD) based dielectric process.

The new ALD SiO2 dielectric liner material was validated through the  downstream TSV fabrication with no adverse effects

Void-free copper filling successfully achieved with 100 nm ALD Liner     No delamination observed between the ALD oxide liner and the Ta barrier  after Cu plating and annealing (good adhesion between oxide and barrier  liners)     No cracks observed after  TSV Cu CMP

## Cross-sectional SEM images after  ALD oxide liner deposition (left) and TSV Cu filling(right) 

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b1c2922f-e447-49d8-9494-4ecd1506c207/b1c2922f-e447-49d8-9494-4ecd1506c207.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=01c1b76c9e070b4c3c9963304079bc66740645ea)
cross-sectional SEM images for a 3x50  m m  TSV after ALD oxide liner deposition:

a)  \~95 nm thick film on TSV top b)  \~91 nm thick film on TSV middle sidewall c)   \~93 nm thick film on TSV bottom corner d)   \~95 nm thick film on TSV bottom

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/86828935-79c5-4e84-8316-c0aeb5e6a0b5/86828935-79c5-4e84-8316-c0aeb5e6a0b5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=8f5f0529f4eefa17fb24223bb363175a02f9665b)
cross-sectional FIB-SEM images for a 6x55  m m with 100 nm ALD oxide liner after Cu filling  and CMP at a) TSV top b) TSV middle c) TSV  bottom. Void-free Cu filling.

## TSV Defects 

![Fin defect Fin defect   Cu cracks Cu cracks  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bd2be432-af33-46ca-b465-cff5987dea54/bd2be432-af33-46ca-b465-cff5987dea54.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=4fbe3aba5b8ce962b7cf39ea186d26b10611ca5c)
Side view SEM image of Cu diffusion to Si induced by  Si Fin defects at TSV bottom

## Silicon Fin Defect at TSV Bottom 

![.152+3  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/76a4f811-d881-49c6-a8a5-e6c748cb7125/76a4f811-d881-49c6-a8a5-e6c748cb7125.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=cc41a363c3adab0a332c63ab8c8eeed857aebcc0)
Fin defect found after TSV DRIE process at the bottom, attaching to sidewall\~10 um high, 1 um extended     TSV Killer defect could serve as a weak point for isolation liner deposition could serve as a weak point for barrier/seed layer deposition may cause mechanical failures during TSV backside reveal     Possible root cause: bulk micro defects serve as micro masks during the TSV  etch resulting in Si Fin defects

D. Zhang et al., Electronics Letters, Vol.  50, No. 13, p. 954

## Bulk Micro Defect (BMD) 

![surface SIDNZ TSV BVD ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2cf1bbe7-7a74-4781-a1ab-ca07db5e5242/2cf1bbe7-7a74-4781-a1ab-ca07db5e5242.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=8a5371bdda84f2b07c94e5a0ca2fa2f27771a8f8)
Courtesv  SEMULLAR

## TSV gets into where devices have not gone before 

T.M. Mak et al., 3D Test Workshop, October 2014

commonly refer to oxygen precipitates in  silicon (in fact could be any imperfections  including oxygen precipitates, voids,  inclusions, slip lines, etc.)

Act as gettering sites at which impurities tend  to concentrate

The profile of BMDs is often controlled via a  complex series of high temperature  processes, to create a “denuded zone,” so  that the surface layer silicon, where the MOS  transistor action takes place, is free of  oxygen precipitates (oxygen precipitates in  the underlying silicon acts as a gettering site  to keep impurities away from the MOS  transistors)

Imperfections in the lattice of a  semiconductor and impurities create energy  states in the bandgap, decrease carrier  lifetime, and increase junction leakage

## Cu protrusion 

Via protrusion: a widely known challenge with TS V  processing.

Annealing a TSV wafer puts the Cu TSVs under high stress and  may form a protrusion where the Cu is forced out of the blind  via.

This phenomenon occurs because of the large mismatch in the  coefficient of thermal expansion between Cu via and Si  surrounding it.

•  caused by Cu recrystallization and grain growth during high-temperature  process in BEOL. •  can lead to crack or delamination of the back-end-of-line.

Optimization of the TSV process with respect to parameters  such as via diameter, depth, pitch, annealing temperature and  duration is critical for minimizing Cu protrusion and its effects  on reliability.

## Cu protrusions 

• Popping out during high-temp  processing steps

• Cracking/flaking of dielectrics over  Cu TSV and open vias to above  metallization lines

• Integrations issues as well as serious  reliability concerns

![Source:SEMATECH  10.0V0.0m5.06SEMLA04302010  22-JUL-04  MADRID5.0kVX11.0K2.73m  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1e0dd5ab-c7d6-48c1-ac7b-d98fb69f9efb/1e0dd5ab-c7d6-48c1-ac7b-d98fb69f9efb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=9f036c4359bc917f0231e0947cd99329544f0c95)
## Effect of Annealing on Cu protrusion 

![m  0.8  a  0.6  04  0.2  S0   100150200250300350400450  350 90.   400 9C.   4509C   Annealing temperature (°C)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/47003ace-a13e-466e-87de-a15b94da5ba7/47003ace-a13e-466e-87de-a15b94da5ba7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=a40b60bd0a761feb18383d8de5a93ffe1b2aa603)
SEM images showing protrusion at various annealing Temps   Protrusion increases with Annealing Temperature   Protrusion may occur at the TSV edge or center

## Effect of TSV geometry on Cu protrusion 

![0.8  DTS   High tem pera ture  sn.mo.d   0.6   Room temperature  04  0.2  HS   JS   30  Via diameter (μm)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a243e3f2-0fd6-430a-9fd5-174e1d4396af/a243e3f2-0fd6-430a-9fd5-174e1d4396af.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=e71938555aeebc8d6003bee6c24ba044e5560d24)
Cu protrusion increases with decreasing  aspect ratio (increasing via diameter) for  a given via depth     Cu protrusion increases with increasing  aspect ratio (increasing via depth) for a  given via diameter     Cu volume directly affects Cu protrusion

![0.8  0.T  0_6  (um) uoisn.no.d n)   O.S  04   High tempera ture  Roomtemperature  0.3  0.2  20   30   0   SD   60   80   90   100  TSV depth (μum)  0.8  ■High tempera ture  0.6   Room temperature  1mO  04  0.2  0.1   1O   100  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ebf07132-c729-48ce-b815-0b0c4d6cbe49/ebf07132-c729-48ce-b815-0b0c4d6cbe49.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=a812acc88f41686f717f807fdd2671b9a6d3e8ab)
F.X. Che et al., IEEE Trans. Compon. Packag. Technol., Vol.3, No. 5, p. 732

## Cu contamination 

Cu TSV presents a risk for metallic contamination:

Cu atoms diffuse out of the via and into nearby devices if the blocking  property of the barrier layer to Cu is not sufficient.

• quite challenging to achieve high quality barrier for all Cu TSVs in  a wafer particularly in the case of high-density TSV with small  diameter and high aspect ratio. • minimizing the so called sidewall scalloping (TSV sidewall surface  roughness caused by the BOSCH DRIE via formation process) is  critical for realizing a robust conformal deposition of  dielectric/barrier liners and thus preventing Cu out-diffusion.

Cu atoms can be stuck on the background surface during wafer  thinning and may not be completely eliminated even after the  cleaning process.     Cu is extremely mobile in Si and SiO2. It exhibits the highest  diffusivity in Si among all metal elements.     If Cu atoms reach the active region they can cause device  performance degradation and early breakdown.

## Cu contamination characterization through  transient capacitance measurements (C-t) 

![GateElectrode  GateOxide  Depleted  Space-Charge  SiSubstrate  Region  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/467f9a5b-95f5-44db-93e1-3f3ea8eabd57/467f9a5b-95f5-44db-93e1-3f3ea8eabd57.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=906d2bcf834cdd4def61f6388774ecadeb038353)
Extraction of generation lifetime of minority carriers in the depletion  region, where Cu impurities generate deep levels at mid gap in energy  band and increase G-R rate between electrons and holes

Capacitance change of the MOS structure is measured after applying a  voltage pulse to the gate during the transition from deep depletion to a  steady-state inversion

F.P Heiman, TED, Vol. ED-14, No. 11, p.781

Cu contamination characterization through  transient capacitance measurements (C-t)

![e.o  J0o/0  tinne  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/981a9a1f-89cf-440b-9ec4-97b29fd68a7b/981a9a1f-89cf-440b-9ec4-97b29fd68a7b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=df6d29abe843d062c3d58796f70568beb8e98224)
C-t curves as plotted as a function of normalized C/Cf vs. time where C is the high  frequency capacitance in the deep deletion condition and Cf is a steady-state capacitance  in the inversion condition.

Capacitance gradually increases to the final value of Cf as minority carriers are generated  in the depletion region. The transient time required to reach steady state is a measure of  the generation lifetime of the minority carriers.

Longer generation lifetime (and hence longer transient time) implies less crystal defects  ( less Cu contamination)

## Cu contamination characterization through  transient capacitance measurements (C-t) 

![Cu/TaElectrode  CuTSV （Φ500um） Oxide（200nm)  ←Ta（minimal） ta OxideLiner Depleteg Space-Gharge Region(SCR)  Si Substrate p-typeSi  100-nm NDNE  SE  10.0kVX100.000  100nm  WD3.0mm ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e8d233f6-1bdd-4415-ba39-38a14a2c41b7/e8d233f6-1bdd-4415-ba39-38a14a2c41b7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=8c6d6418cc1b1659127cd69421fc935e8020fd78)
Trench MOS capacitor with Cu/Ta gate electrode and  Cu TSVs     Study the barrier layer effect on Cu-diffusion trough C-t analysis effect of Ta liner thickness effect of sidewall scalloping effect of TSV proximity  K-W Lee at al., TDMR, Vol. 140, No.1, p. 451 effect of anneal temperature

## Effects of sidewall scalloping and Ta liner  thickness on Cu contamination 

![12   12  20min   Scalloping(30nm)   10min   Scalloping（200nm)  1.0   10  \~As-Depo.  0.810min   0.8   5mnin   As-Depo.  30.6   As-Depo.   0.6  As-Depo.  5min  5min  0.4   1omin   04  10min  20min  0.2   0.2  100   200   300   400   500   100   200   300   400   500  Time(sec)   Time(sec)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a6adfcdf-0404-4a6f-ada7-2eadee1f5d13/a6adfcdf-0404-4a6f-ada7-2eadee1f5d13.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=20fdf7e71a90f1db4c93fa2c86b7fdbe87987f4b)
C-t curves of the trench capacitors with 200 nm scalloping roughness  show far more severe degradation (much shorter tf)

![1000 -Ta（100nm)/Scallop（30nm) 100 Ta（100nm)/Scallop（200nm) -Ta（10nm)/Scallop(200nm） 10  -Ta（10nm)/Scallop（30nm) 10  20  30  40  50  60 AnnealingTime（min） ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/46f22d1d-9aee-4e98-83ae-c80c15e547ca/46f22d1d-9aee-4e98-83ae-c80c15e547ca.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=e4f33a1cf65b7bf0daaac4a87e12a984bdd50961)
Significant degradation of  the generation lifetime for  the trench capacitors with  thin Ta thickness even in the  case of small scalloping  thickness

No degradation observed for  thicker Ta liner

## Effect of TSV proximity on Cu contamination 

![Cu/TaGate  Electrode   1000  Distance,d  100  (Cu Diffusion)  As-Depo.  Depleted   10  CuTSV   Space-Charge   300°℃，5min  Region   300℃,10min  p-type Si  20   40   60   80   100  Distance from CuTSV（μm）  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cb61d08d-c2ab-4e1d-8c56-b77e3d8da8a4/cb61d08d-c2ab-4e1d-8c56-b77e3d8da8a4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=0daea445883a8b8d296fba54fa35936bc0dbfc17)
configuration cross-structure  of a planar MOS capacitor  placed near Cu vias.

to intentionally diffuse Cu into  the MOS depletion layer,  trench via features an  unoptimized sidewall and a  thin Ta liner layer

minority carrier lifetime vs. distance of  the trench capacitor from Cu TSV

degradation is more pronounced for  reducing distances from TSV and  increasing anneal duration

## Mobile ion penetration effect on devices in  close proximity to TSV 

mobile ion contamination has been eliminated from advanced  technology nodes as a result of improvements in BEOL chemistries  and the barrier layer properties.

TSVs intrinsically involve etching through the barrier layers that  decouple FEOL and BEOL and thus allowing a pathway for potential  mobile ions to migrate            risk for mobile ion contamination.

mobile ion contamination can cause  parametric shifts (Vt, Ion) for devices in  proximity to TSV

effect is of electrostatic nature and  fundamentally different from the TSV induced  mechanical stress

Optimizing post-etch cleaning and TSV liner  formation processes is critical to mitigate risk

![S2  Silicon  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a5248d5b-6534-4fa8-ac81-ba710eb113a9/a5248d5b-6534-4fa8-ac81-ba710eb113a9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=ead242f68ec4a085d1c3d0059dc4ba9ad93ae908)
## Mobile ion penetration effect on devices in  close proximity to TSV  1.0e-3  

![1.0e-3   1.0e-3  1.0e-4  1.0e-4  1.0e-4  Control   Control /  1.0e-5  (ne)   1.0e-5  TSV  1.0e-6  TSV   1.0e-6  1.0e-6  1.0e-7  PFEN   1.0e-7   NFET   1.0e-7  1.0e-8   5  [mplant  TSy  TSV   TSV  1.0e-9   1.0e-8   1.0e-8  Fig3a   Fig3b   PFET  vgate   vgate  1.0e-10   1.0e-9  -1.00 -0.80 -0.60 -0.40 -0.20   0.2   04   D_6   0.8   10   1.0e-9  -1.00-0.80-0.60-0.40-0.20  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/72ca7465-601c-49d9-a697-ffa49dda2d03/72ca7465-601c-49d9-a697-ffa49dda2d03.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=8919c6bab1ef42d8bdaba48df623013aca0587f7)
PFETs in proximity to TSV show a significant shift in Vt compared to control  devices

shifts are inconsistent with the mechanical stress effect from TSV  (opposite direction)

The absence of shift in NFETs and the reduction of shifts for PFETs placed  nearby NFETs is consistent with mobile ion penetration in CMOS and  attributable to the gettering properties of As.

C. Kothandaraman et al., IEDM 2014

![1.4E-11  1.2E-11  Peak  1.0E-11  TSyf  8.1E-12   di els.  6.1E-12  4.1E-12  21E-12   Control  Dies  1.0E-13  -30   -20:   -10   -1-0:   20   \$00   SDD  voltage  1e16  TSV  1e15  -1.0   -0.5   0.0   0.5   1.0   1.5  Depth, um  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b1ddbb18-51ca-4272-b7d6-0dd2515ed861/b1ddbb18-51ca-4272-b7d6-0dd2515ed861.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=1368f4ff769c59f09ddddd65ab77b675bc95d073)
## identification of mobile ion species through  Triangular Voltage Sweep (TVS) and SIMS profiling 

Sharp peaks on TVS spectrum  represent fast moving ions (i.e. Na)  [1]

Larger atomic elements such as Cu   show peaks at higher voltages (not  present in these samples)

Total charge is equal to the area  under the peak

SIMS profiling confirming the  presence of Na

Na concentration decreases with  increasing distance from TSV

[1] D.K Schroeder,Semiconductor Material  and Device Characterization,  $3^{\mathfrak{r d}}$    edition,  2006, p. 340

## Benchmarking an optimized TSV process through  DRAM retention characterization 

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ee6da90d-1da6-4246-9dbc-723d220b2759/ee6da90d-1da6-4246-9dbc-723d220b2759.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=215116099a87a1419875553c8803ddb8185145ac)
TSV enabled  96Mb embedded  DRAM  product array constructed in IBM’s 32SOI high  performance logic technology.

DRAM retention characteristics are known to  be sensitive to the presence of mobile ions

Comparison of the retention statistics before  and after the introduction of the optimized TSV  show no difference

![BeforeTSV  AfterTSv  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/590c04f6-5caa-477f-87da-113df813c141/590c04f6-5caa-477f-87da-113df813c141.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=bd899f067404697acfc709aeaa55adc1aa671398)
Log (Retention Time)

## Dual Ramp Rate controlled IV as a method to study  barrier/liner integrity in TSV applications 

Voltage ramp or controlled IV and variations of this method (i.e. multiple  ramp rates based IV) have been used as an alternative to TimeDependent-Dielectric-Breakdown (TDDB) reliability measurements [1][2]  • better time efficiency than traditional TDDB measurements • particularly suited to TSV oxide/liner integrity study where high nonuniformity in liner thickness inherent to the Bosch etch process can  cause large variation in the failure times of TSVs

![t50%(E)\~exp(-E)  t50%  High Y→  goodTDDB  LowY  badTDDB  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5be734cd-babc-47c9-932b-6a99d688904b/5be734cd-babc-47c9-932b-6a99d688904b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=b6cfcd40276da0e90bdfb46ba3e8604b629bb7d1)
TDDB method

E-model t 50 %  \~  exp( E )

![EBD(R)=EBD(R。)+/ In(R/R。)  EBD  Low y-I →  goodTDDB  High Y'→  bad TDDB  In(R/R.)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/55009dec-281e-4f4e-a021-e5e998cd05a9/55009dec-281e-4f4e-a021-e5e998cd05a9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=b923e1f8e8a08fba675bc51c542c11c9b5e50020)
Controlled IV method

[1] Berman A, IRPS 1981, p. 204 [2] Y.-L.Li et al., ECTC 2012, p.304

## Switching polarities in controlled IV to detect Cu presence  

•  Application of negative Voltage (-V)  repels positively charged Cu ions away  from SiO2           coper ions can not drift  into SiO2 irrespective of barrier quality. •  With application of positive bias   $\left(+\mathsf{V}\right)$  ,  Cu ions will be forced towards SiO2.  • in case of a good barrier, Cu ions do  not penetrate into SiO2 and a high  is maintained. • poor quality barrier will allow Cu  ions to penetrate into SiO2 and  degrade  .

K. Croes et al., International Symposium on  the Physical and Failure Analysis of Integrated  Circuits (IPFA), 2012.

![>copper   → copper  ionsrepelled   ionsforced  from SiO2   into SiO2  cu+   Metal  (barrier)  SiOz   Insulator  Semiconductor  GND  Bad barrier   High y   Lowy  Good barrier   High y   High y  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b5949a98-05c7-481c-a4fd-22b798859dac/b5949a98-05c7-481c-a4fd-22b798859dac.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=44113dfe05b78fb2ae06be97319a010d64e1753d)
![10  (/An)   In(R/R.)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/684258a5-f6e4-4268-bbf6-72379cb0b068/684258a5-f6e4-4268-bbf6-72379cb0b068.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=f15ecfce80ec6c8a201ea13b5b54bf249fa0b674)
## Outline 

3D LSI Technologies background •  Through-Silicon-Via (TSV) applications     TSV Integration schemes     TSV Process flow and considerations     TSV Integrity and potential reliability concerns     TSV induced thermo-mechanical challenges  •  effect on device performance (TSV proximity effects) •  effect on FEOL/BEOL reliability     Chip Package Interaction (CPI) challenges     Concluding remarks

## Thermo-mechanical stress in 3D TSV Technologies 

Due to the mismatch in the coefficient of thermal expansion (CTE) of the Cu  TSV and the Si, thermo-mechanical stress is induced in the region  surrounding the TSV during fabrication process and thermal cycling of TSV  structures.

The induced thermo-mechanical stress can

• affect the electrical characteristics of devices placed in proximity to TSVs   • drive crack growth in the 3D interconnects in proximity to TSVs

TSV induced mechanical stress can be experimentally evaluated indirectly  from electrical characterization of devices in proximity and directly using  micro-Raman spectroscopy [1]

Various fabrications steps employed by 3D IC technologies such as  wafer/die thinning, wafer/die mounting, chip stacking, solder ball  solidification act as additional  stress sources and need to be accurately  accounted for:

• determining the overall chip-stack performance and reliability   • design optimization for the so-called TSV keep-out-zone (KOZ)

## Sources of thermo-mechanical stress in 3D chip stacking 

![mpact of Flip Chip   Impact of TsV/uBump  ackage on 3D chip-   on top die  stack (cPI)   ●Built-in stress  Stress induced by Cu-   ·Stress varies as function of  illars on low-K   temperature  Impact of 3D-SIC  Stress induced by  bonding on dies  vermold,laminates CTE   mie 5  ·Stress during bonding  nismatch  ·Stress due to underfill  CTE mismatch  Impact of die thinning   Impact of Tsv on  ·Releases stress   bottom die  ·Strength of die   ·Built-in stress  ·Stress varies as  function of temperature  Stress/strain can lead to  .mechanicalfailuresdueto  delamination, peel, fatigue, ..  · electrical impact due to   Multi-scale  parameter shifts, increased variability, EM,..  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a8e77801-0af8-4170-9056-57f206e61ec7/a8e77801-0af8-4170-9056-57f206e61ec7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=d415b3d1aa2b844138ddc503e90dc554e4d8fbc3)
## thermo-mechanical effects on devices in proximity to TSV 

Thermo-mechanical stress applied to metal/semiconductors changes the  inter-atomic spacing which alters the band structure making it easier or  harder (depending on the material and the strain) for electrons to be  raised into the conduction band

Electrical parameters of devices placed in proximity to TSV impacted:

•  Low-field mobility and saturation velocity changes are attributed to the straininduced carrier effective mass and scattering [1]  $\succcurlyeq\upmu={\sf e r}/{\sf m}*$  (Drude’s approximate model)     threshold voltage changes are due to the strain-induced shifts in conduction  and valence band electronic band potentials [2] [3]

Magnitude of stress-induced electrical variations in 3D transistors  depends on the distance of the devices from the TSVs, the transistor  channel orientation, Temperature, device geometry and layout.

For the relatively small TSV-induced strains, piezoresistivity can be  applied to evaluate changes in electrical parameters as a function of  stress components.

Piezoresistive effect: change in electrical resistance of a solid when subjected to  stress field

[1] Y. Sun et al., Journal of Applied Physics, Vol. 101, No. 10, p. 104503-1   [2] C.G.V. de Walle, Phys. Rev. B, Vol. 39, p.1871 [3] C. Herring and  E. Vogt, Phys. Rev., Vol. 101, p. 944

46

## Stress field around a  TSV 

Lame equation:  2   D      Cu   r  D: TSV diameter r: diastance from TSV

![Tangential  Compression  Radial  tensiona,  TsV  [GPa]   [GPa]  Du0S  OXX   D02   DW02  00  0.D1  0.01-10   0.03  002   0.02  20  -0.03   -003  SO  20   29  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/912423eb-eb5f-476d-bd6d-4154d6f7eba9/912423eb-eb5f-476d-bd6d-4154d6f7eba9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=2d1243f6f7451045bb5b43994750f22434ee2d27)
Translation of stresses from  the cylindrical to the Cartesian  coordinates results in the  “flower shape” stress patterns

The stress in the Si around the TSV has a cylindrical symmetry with two main  components: the radial (tensile) and the tangential (compressive) stress  components. Vertical stress component becomes negligible at 1  m m away from  TSV (3D         2D problem)

The stress levels in radial and tangential direction are of opposite sign but equal  in amplitude and are proportional to the square of the TSV diameter D and  inversely proportional to the square of the distance from the TSV r

Guo et al., IEDM 2012

## Effect of TSV induced stress on carrier mobility (piezoresistivity effect of Si) 

![nMOSFET  (Perpel  dicular)  Residual Strain   Residual Strain  (Tensile)   （Tensile)  Sv  nMOSFET   pMOSFET  (Parallel})   (Paralel)  PMOSFET  (Perpedicular)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/30c4fb83-6e4c-41e6-979e-2e4820d366e2/30c4fb83-6e4c-41e6-979e-2e4820d366e2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=cba0610f0c2e702f3e984cc2772a7632e1bbd554)
![PlanarW/L=500/900nm  200   nFET  Horizontal  15  Vertical  PFET  Horizontal  Vertical  -2.5/r  2.7/r  5   0.5/r2  -0.5/r²  200  46  8  101214   6  1820  Distance from device center to TsV center(um)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bb93c8e1-2c47-4a9c-8846-7ac9a83eb86f/bb93c8e1-2c47-4a9c-8846-7ac9a83eb86f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=c443fed9f81e85fc367ce57b47881ebce2da30dd)
||nFET mobility|pFET mobility|
|---|---|---|
|Perpendicular|decrease|increase|
|Parallel|increase|decrease|


The relative change of Si resistivity (and hence mobility carrier) is related to the TSV  stress by the piezoresistance coefficients. Piezoresistance coefficients have different  values for n-type/p-type Si and the radial and tangential stress components have  magnitudes of opposite sign          Effect from TSV stress on nFETs is different from that  on pFETs

Guo et al., IEDM 2012   S.K. Ryu et al., TDMR Vol. 12, No.2 p. 255

## Impact of Temperature on TSV stress 

![口 125C 色75C Wafer with TsV process  -30C 0-30C 一  1520253035  4045 50 Distance from TsV (um) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6ba60aa3-a172-46ce-9d0a-6faafaefc4e1/6ba60aa3-a172-46ce-9d0a-6faafaefc4e1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=1f81480d75b9ebb03473f824ba9d96eb5dbfe069)
pFET max transconductance gm vs.  distance from TSV characteristics  measured for various temperatures [1]

stress-induced gm change reduces  with temperature. No proximity effect at  125C.

[1] D.P. Ioannou et al., IRPS 2014   [2] A. Mercha et al., IEDM 2010

![6.0   lonchangesalmost linearly  versustemperature  5.O  TCADpredicts zero impact  ()  4.0   at\~145°℃  3.0  Linearextrapolationshows  noimpactat\~130°C  2.0  Measurements  1.0   Linearfit  Simulation  0.0  20   40   60   80   100120140160  Temperature(C)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/24da6965-60c6-4901-b8ef-c37e8f3775fd/24da6965-60c6-4901-b8ef-c37e8f3775fd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=c2f3dc4c121d58b2c39d5d59653a57357325dea9)
pFET Ion change vs. temperature and  extrapolation to zero stress  temperature [2]

Cu exhibits elastic mechanical  behavior that gives linear stress  reduction with temperature. TSV proximity effects are expected to  disappear at the stress free  temperature

## Single vs. array of TSVs induced stress  

![push  Single  TSV   MOSFET  ou  push  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b8d9e3a5-abc2-4185-a1de-cd4fe377eea0/b8d9e3a5-abc2-4185-a1de-cd4fe377eea0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=8b14b9286d64a759297d194e8e3d38389fddc496)
![ParallelTsVrow   PerpendicularTsVrow  push  pul  push  push   push  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f02e4868-5bee-43ac-8ab2-9bbc3585a722/f02e4868-5bee-43ac-8ab2-9bbc3585a722.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=548342cad4307d99fe09ca5f28d9dadc8ada8198)
A single TSV creates both radial  mechanical tension and tangential  compression in the surrounding Si.

In case of a parallel TSV row the stress effects  are enhanced. Perpendicular TSV row creates  rotated stress patterns with the angle  increasing  for each subsequent  TSV in the  row

When multiple TSVs are placed in close proximity to each other they create  different  stress interference patterns depending on the TSV placement layout

Details of the TSVs topology can have a profound effect on the electrical  characteristics of an FET within the TSV array

A. Mercha et al., IEDM 2010

## Impact of single vs. array of TSVs induced stress on FET performance 

![NoTSv's   1TSV   4TSVs   4TSVs   9TSVs  reference   centered   "square"   rdiamoron  TSW  Stresses  addup  Stresses  cancelout  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a51835df-00a3-4d88-af16-8bdedeaf4057/a51835df-00a3-4d88-af16-8bdedeaf4057.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=f203a344fc7496aa8e3e09647c589f948a0119f9)
simulated stress distribution within  the 9 TSVs matrix showing areas  where stress is enhanced or  cancelled out

![296  096  296  1TSV  496   4TSVssqu  4TSVs   amond  -696   SV  -896  2D  Distance AlongX Axis,jum  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fa92c099-c81c-40e3-88d2-eb3880c41e1f/fa92c099-c81c-40e3-88d2-eb3880c41e1f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=2c04aece674ece98a9eb1f13c04ea077aba3fd04)
TSV induced proximity effect on 40 nm pFET is shown to depend on the specifics of TSV  layout/placement

## Outline 

3D LSI Technologies background •  Through-Silicon-Via (TSV) applications     TSV Integration schemes     TSV Process flow and considerations     TSV Integrity and potential reliability concerns     TSV induced thermo-mechanical challenges  •  effect on device performance (TSV proximity effects) •  effect on FEOL/BEOL reliability     Chip Package Interaction (CPI) challenges     Concluding remarks

## Effects of TSV process and wafer thinning on FEOL reliability (the 32 nm SOI HKMG CMOS logic technology paradigm) 

||3D processes impact to devices|
|---|---|
|        T'STr                 process      |Proximity effects on FEOL|
|        T'STr                 process      |        reliability induced by TSV                mechanical stress      |
|        T'STr                 process      |        reliability induced by TSV                mechanical stress      |
|        T'STr                 process      |        reliability induced by TSV                mechanical stress      |
|        T'STr                 process      ||
|        T'STr                 process      ||
|        T'STr                 process      |Global effects (independent of|
||TSV proximity) on FEOL|
||reliability related to TSV|
||        processes such as extra heat                cycle, etching, etc.      |
||        processes such as extra heat                cycle, etching, etc.      |
||        TC: -65C to 150C,500 cycles                SV:225C,500 hours                FEOL reliability stressing was                carried out on chips of the same      |
|||
|||
||        wafer before and after TC and                STr.      |
|        Wafer                 thinnimg                 process.      |Verify any possible impact to|
|        Wafer                 thinnimg                 process.      |        FEOL reliability of wafer                thinning process.                Wafer is testable from the front                Side      |
|        Wafer                 thinnimg                 process.      ||
|        Wafer                 thinnimg                 process.      ||


M. Farooq et al., IRPS 2015

||||        Effects of TsV process on                devices on thick wafers      ||
|---|---|---|---|---|
|FEOL RE mechanism|FEOL RE mechanism||        Effects of TsV process on                devices on thick wafers      |        Effect of wafer                thinning process on                devices      |
||SG||TSV Proximity effects||
||SG||        SG/EG n/pFET 2D CHCSG/EG n/pFET 2D CHC                No effects                models supported with TSVmodels supported with TSV                proximity for dmm ≥5um.proximity for dmm ≥5um.                Global 3D effects      ||
|IICI ||m/pFET|        TSV process induced EG                n/pFET HC enhancement                respect to 2D baseline.                EGn/pFET HC model                updated as part of the 3D      |        Further increase in                CHC HC shift due to      |
|IICI |ECG ||        respect to 2D baseline.                EGn/pFET HC model                updated as part of the 3D                reliability guidelines                TC and Sy      ||
||||No effects observed.||
||SG|m/'pFET|TSV Proxinity effects||
|BTI|SG|m/'pFET|        Equivalent RE                performance between 2D                and 3D processed at      |No effects|
|BTI|EG |||No effects|
||SG||        performance between 2D                and 3D processed at                recommended TSV                proximity design rules.                Global 3D effects                No effects observed      ||
|TDDB||||No effects|
|TDDB|ECG|n/pFET|TC and sy|No effects|
|TDDB|ECG|n/pFET|No effects were observed.|No effects|


## TSV effects on 32 nm SOI HKMG Hot Carrier reliability 

![Ydirection:  Tensile stress  onchannel  KOZ  一   Xdirection:  Gate  Compressive  ActiveArea  stess  TSV  onchannel  KOZ-Keep out Zone  Tensile stress  ACompressive stress  d=distancebetween theKOZand theDevicegateactiveoverlapclosertoKOZedge  Channel Current  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1c2200a3-5aad-4281-b0dd-1642738c1123/1c2200a3-5aad-4281-b0dd-1642738c1123.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=ab1879fd7b5692097528c6fc127af2143671bf32)
![12  1.15   EGFET  1.05  lesp  nFET2D thickwafer  0.95  OnFET3D thickwafer  09   nFET3Dthinnedwafer  pFET2Dthickwafer  0.85   pFET3Dthickwafer  pFET3Dthinnedwafer  08  0.9   0.95   1.05  Normalized Initial Idsat  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/dc9fdbf8-3496-4baa-af02-08a47706a512/dc9fdbf8-3496-4baa-af02-08a47706a512.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=a88cbf1e0eb2923b37f05b698db77d976986d4de)
![3Dthinnedwafer-Xdir  109  --3D-thickwafer-Xdir  1.08  107   →-3Dthinnedwafer-Ydir  -3Dthickwafer-Ydir  1.06  每1.05  8104   EGPFET  1.03  ezet  102  1.01  20.99  0.98  0.97   EstimatedHCEOL  0.96   targetof2D32SOl.  0.95  FET distance fromKOZ（um)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/249f111a-a160-46d0-aacb-668150eb6f44/249f111a-a160-46d0-aacb-668150eb6f44.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=cdafc290d5a111d4171ba9b254bc93c33ec200cc)
Normalized average pre-stress Idsat as  function of device distance from TSV trends  are consistent with the TSV mechanical  stress effects on pFET. Wafer thinning has  no impact on TSV proximity effects.

Hot carrier induced % Idsat degradation  dependence on TSV proximity is a function  of the pre-stress Idsat, irrespectively of the  wafer type.

## 3Di Global effects on 32 nm SOI HKMG Hot Carrier reliability 

$$\begin{array}{r l}&{\mathcal{L}_{1}=\underbrace{\left[\begin{array}{l}{1}\\ {0}\end{array}\right]\times\left[\begin{array}{l}{\bar{\mathcal{X}}_{12}}\\ {\bar{\mathcal{X}}_{21}}\\ {\bar{\mathcal{X}}_{31}}\\ {\bar{\mathcal{X}}_{41}}\end{array}\right]+\underbrace{\left[\begin{array}{l}{\bar{\mathcal{X}}_{22}\times\bar{\mathcal{X}}_{13}\times\bar{\mathcal{X}}_{23}}\\ {\bar{\mathcal{X}}_{22}\times\bar{\mathcal{X}}_{33}}\\ {\bar{\mathcal{X}}_{43}\times\bar{\mathcal{X}}_{44}}\\ {\bar{\mathcal{X}}_{5}\times\bar{\mathcal{X}}_{5}}\\ {\bar{\mathcal{X}}_{6}\times\bar{\mathcal{X}}_{6}}\end{array}\right]}_{\begin{array}{l}{1}\\ {0}\end{array}}f\left[\begin{array}{l}{f}\\ {f}\\ {\bar{f}}\\ {\bar{\mathcal{X}}_{8}}\\ {\bar{\mathcal{X}}_{9}}\\ {\bar{\mathcal{X}}_{11}\times\bar{\mathcal{X}}_{12}}\\ {\bar{\mathcal{X}}_{13}\times\bar{\mathcal{X}}_{13}\times\bar{\mathcal{X}}_{14}\times\bar{\mathcal{X}}_{8}\times\bar{\mathcal{X}}_{16}}\end{array}\right]},}\end{array}$$
![2D thick wafer  口_9  +-3D thick wafer  □_8  -3D thinned wafer  O_F  0_6  0.5  0.3  0.2  国_1  C  %dsat CHcinduced shit  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/194330b6-fdbe-4be7-b65a-e52c0d2eb610/194330b6-fdbe-4be7-b65a-e52c0d2eb610.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=57a3a5df2d2bf0595dc19560927e872ac52e7390)
Hot carrier induced cumulative %Idsat distributions for a reference nFET (far  away from TSV) for 2D, 3D thick and  3D thinned wafers.

nFET hot carrier sensitivity increases  with the wafer thinning process.

Hot carrier degradation enhancement  due to 3D global effects is attributable  to the extra heat treatment that devices  experience during the 3D processing  with respect to the 2D process flow.

Extra thermal treatment results in an  increased availability of Si-H bonds and  a corresponding increased rate of Si-H  bond breaking.

## p-channel MOSFET NBTI effects in proximity to TSV 

Gate-Oxide reliability in strained-Si MOSFETs has been studied to some  extent with the reported results varying significantly on their conclusions  [1][2][3]

•  most stress device engineering techniques require additional processing steps which  render the results from a comparative study of devices with and without process-induced  strain difficult to interpret.

A study of the impact of mechanical compressive and tensile stress on  device performance and NBTI reliability of pFETs with identical gate oxide  was reported in [4]

These effects were investigated by placing identical pFETs in proximity to TSV   pFETs fabricated in a 22 nm HKMG SOI CMOS Logic technology.

Electrical device characterization at time-zero (pre-NBTI stress) confirmed  the pFET mobility modulation dependence on proximity to TSV, device  channel orientation, and device temperature.

NBTI induced Threshold Voltage shifts were found to be unaffected by the  mechanical stress.

On the contrary, the NBTI component contributing to mobility degradation  was found to strongly depend on the level of applied mechanical stress.

[1] A. Shickova et al., EDL, Vol. 28, No. 3, p. 242 [2] H.S Rhee ate al., IEDM 2005 [3] J.B Young  et al., TED, Vol. 57, No. 1, p. 238 [4] D.P. Ioannou and G. LaRosa, IRPS 2014

## p-channel MOSFET NBTI effects in proximity to TSV 

![100  NBTI:-1.7V, 65 °C  Wafer with TSV process  (w) u!IAV   X=50 um  X=5 um   X=3 Hm  +X=0um  X=-1 um  x Y=2 um  10   100   1000   10000  Stress Time (sec)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c5c4d959-f552-437c-a403-2eea6dd259d9/c5c4d959-f552-437c-a403-2eea6dd259d9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=129afab68f4e86b9fd32cac136110da2cfda9890)
D.P. Ioannou and G. LaRosa, IRPS 2014

![ne)  uuB  wnwixew  口125C  △75C   Wafer with TSV process  -30C  -30C  C   1５   20   25   ③0   ③5   45   50  X Distance from TsV (um)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fd88c272-42bc-426d-ab77-71285099d2a8/fd88c272-42bc-426d-ab77-71285099d2a8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=ace858a76c78f391bb90622f8ee17e5b6d81714e)
pre-stress maximum gm vs. X distance to TSV  characteristics at various temperatures are  consistent with the TSV-induced compressive  stress on pFETs in proximity.

NBTI induced Threshold Voltage shifts vs.  stress time characteristics for devices at  various proximities to TSV.   Threshold Voltage shift is unaffected by TSV  mechanical stress.

## p-channel MOSFET NBTI effects in proximity to TSV 

![3.E-06  NBTI:-1.7V, 65 °c  △Tot   X=50um  ○X=5um  2.E-06  △X=2um  ×X=1um  +X=0 um  △V: parallelI-V shift   X=-1 um  \*Y=2 um  1.E-06  time-zeroI-V   YX  post-stress I-V (without mobility degradation)   post-stress I-V (including mobility degradation)  0.E+00  0.２   0.4   0.6   0.8   1.２  Vgs (v)   1０   100   1000   1000  Stress  Time (sec)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/adba8332-0dea-4ac6-94c6-a296597a1790/adba8332-0dea-4ac6-94c6-a296597a1790.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=5a6c9f675f09508a249ec6b9610a4ac9baf03166)
NBTI stress effects on FET I-V characteristics. D I current degradation corresponds to  D V  parallel I-V shift (no mobility degradation. D I Total  is the overall current degradation  including carrier mobility degradation effect.

NBTI induced current degradation vs.  time characteristics show dependence  to the TSV proximity

## NBTI induced mobility degradation effects for pFETs in proximity to TSV 

Temp: 140C

![2.0E-06  4.0E-06   4.0E-06  Total△I >△Total△I>△lTotal△1   NBTI:-1.7V, 140 'c  NBTI:-1.7V, 65 °C  X=50um  X=50um  1.5E-06   X=-1um   3.0E-06   X=-1 um   3.0E-06  Y=2um    Y=2 um  soilid lines:△I  soilid lines: AI  1.0E-06    data points: △lTotal   2.0E-06 data points: △ITotal   2.0E-06  1.0E-06   1.0E-06  5.0E-07  0.0E+00    0.0E+00  0.0E+00  20   30   40   50   60  15   20   25   ③0   Av or AvT (v)  △Vor △V (V)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/426fbe5a-499e-4800-9d78-2883a71202ca/426fbe5a-499e-4800-9d78-2883a71202ca.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=112349c50259d24ec92dcdaf8cb82f24765123d5)
LHS Plot: 65C NBTI induced  D I Total  -  D I current degradation (component related to  mobility degradation) depends on pFET channel orientation and proximity to TSV.  Largest  mobility degradation (largest  D I Total  –  D I offset) is observed for the device  with the highest mechanical stress induced time-zero mobility enhancement

RHS Plot: Effects are diminished for 140C NBTI where TSV mechanical stress is  significantly attenuated.

D.P. Ioannou and G. LaRosa, IRPS 2014

## Electromigration of 3D-IC TSV Interconnects 

Electromigration: Electron flux induced displacement of Cu ions resulting in  voids/hillocks

Voids results in interconnect resistance increase and ultimately to  interconnect opens

3D ICs introduce new challenges with respect to EM reliability [1]:

•  demand for higher current densities of the interconnects through the stacked  package.   •  TSV induced stress effects.   •  significant dimension mismatches between metal wires, TSVs and landing  pads

Typically, TSV is captured by metal landing pads at the top or device side (capture  level) and bottom or backside (redistribution layer, RDL)

Maximum allowed DC current through the TSV (within chip) is limited by a  combination of the following elements [2][3][4]:

•  TSV cross-sectional area , TSV/capture level area and TSV/RDL area •  Of particular interest from EM perspective is to identify the weakest link  among these elements.

[1] J. Pak et al., ECTC 2011, p. 1420 [2] T. Frank et al., ECTC 2012, p. 326 [3] T. Frank et al.,  Microelectron. Reliab. Vol. 53, 2013, p. 17 [4] P. Periasamy et al., accepted ECTC 2016

## Critical TSV interfaces for EM degradation and stress configurations 

![TSV   MTOP  MBOT  3.4um  2.3um  TS  Zome of  TSV  MToP   SiO2   Zome of   Woidig  C   Woiding  SN  SITN   SiKO  U  TN  TN  MBOT   Down-stream   Up-stream  ST   configuration   configuration  SiO22   TKS  C  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/52b4a134-b728-4b7d-ab82-2cbe39b38fe2/52b4a134-b728-4b7d-ab82-2cbe39b38fe2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=9a48f687b0f89912329e38101470031864281cb8)
Details of bottom and top interfaces of TSV

Two different processes are employed to  enable EM studies on metal thicknesses of  0.25 and 3  m m

Down- and up- stream configurations with  electron flux to address EM degradation  occurring respectively in bottom and top  TSV interfaces.  In both cases, zone of  voiding is adjacent to TSV.

## Resistance traces and void formation mechanism for thin metal process 

![10  270°C 25mA  300°C 25mA  Failure Criterion  8   10   1.00  t [h]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/15a52f03-653f-4097-8956-efad3b1549d4/15a52f03-653f-4097-8956-efad3b1549d4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=9e578d9c321aca902f23dedb8ffa5bcfbf39de21)
Resistance traces show a first latency  period during which resistance remains  constant followed by a progressive increase

![WO1O  STN   Void  KTSV  Crosssectionview  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7446aff2-cf5d-4532-b6ff-91a33361d717/7446aff2-cf5d-4532-b6ff-91a33361d717.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=c05096645a688a523c48b7856bc521bcec7de800)
3D FIB-SEM made on down-stream  configuration indicates that void nucleates in  M BOT  inside the perimeter of the TSV bottom  section. The shape of the void indicates that  the vacancy diffusion path is the Cu/SiN capping layer interface

![THSHT TWnoidl 551 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4c03924d-855e-4c9f-ae57-39fd5660cf61/4c03924d-855e-4c9f-ae57-39fd5660cf61.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=375a8720480bcde4c96f2ac8173b0e4f880a0491)
Resistance increase occurs as the void becomes larger than the TSV conducting  section forcing the electrons to flow through the high resistive TiN barrier

Since the void spans over the whole line thickness, an increase in metal line  thickness should enhance EM reliability    T. Frank et al., ECTC 2012, p. 326

## Resistance traces and void formation mechanism for thick metal process 

![10  270°C 180mA  300°C 180mA  Failure Criterion  10   1.00    1000  t rhT  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/78dffd48-5208-47f4-824e-8c05f2f235f2/78dffd48-5208-47f4-824e-8c05f2f235f2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=6dd2a47f4453cd52df261a81cfd69ef4d3af19c7)
Contrary to the case of thin metal,  resistance traces for the thick metal  show an abrupt step up until open

![STY   SSAV  ShigeaUA/= (D8   W8p  TN  SW  1DD   Non-failed  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c64af5d5-b77c-4c24-b62c-11d8bd6af65e/c64af5d5-b77c-4c24-b62c-11d8bd6af65e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=75f98c5c616d0130bab45cbe2a5b6f9a70ffb507)
Failure analysis of the thick metal process also shows a void growth right above/under  TSV. The site of voiding is now at the metal/TiN interface.

Thick metal process fails mostly due to slit voids (e-g) without exploiting the benefit of  a higher matter depletion capability. Hence, a very thick metal line may not be the  optimum solution for EM reliability improvement.

## EM structure to test the TSV /capture level interface with single and five  parallel fingers connecting two TSVs  

![TSV/Capturelevel-fiveparallelfingers  0.95  0.91  0.84  t5approximately10xgreater  05  03  0.16  TSV/Capturelevel-009  0.05   singlefinger  0.015  Time to failure,arbitraryunits  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/303deae4-9247-4e6b-b7e8-b733660bb009/303deae4-9247-4e6b-b7e8-b733660bb009.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=1be8f14c44961645a495796fd8ee427230897d82)
P. Periasamy et al., accepted ECTC 2016

![Capturelevelparallelfingers  connectingtwoTsV's  LandingPad  TSW   TSV  RDL  ca)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/88d78bf8-310a-44e2-82f9-77fedc448339/88d78bf8-310a-44e2-82f9-77fedc448339.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=243c928984ef774f4c078d97e771163a9ae77bc2)
single capture level finger shows superior EM  reliability over the five parallel fingers case.

TCR measurements indicate a 5 fold increase  in Joule heating of the 5 finger structure over  the single finger.

Simulations indicate current crowding effect  where current flow is restricted to only the  inner fingers effectively reducing the effective  electrical cross-sectional area.

## Outline 

3D LSI Technologies background •  Through-Silicon-Via (TSV) applications     TSV Integration schemes     TSV Process flow and considerations     TSV Integrity and potential reliability concerns     TSV induced thermo-mechanical challenges  •  effect on device performance (TSV proximity effects) •  effect on FEOL/BEOL reliability

Chip Package Interaction (CPI) challenges

Concluding remarks

## CPI challenges in emerging packaging integrating solutions 

CPI: The interaction between the semiconductor package stresses and  the semiconductor device.     CPI has gained increasing attention in advanced technology nodes  mainly due to   Introduction of low-K (LK) and ultra-low-K (ULK) materials in the back  end of line (BEOL) to meet the demands for higher performance and  lower power consumption.

![RCdelay   Unwantedresult:  Dielectric   Crosstalk  LowModulus  Material  Power consumption   (CPIRisk!)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/04d13dbf-2ead-4d41-9ee3-66d4c1e42a71/04d13dbf-2ead-4d41-9ee3-66d4c1e42a71.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=07162f698897574f421785ff5a64667868c839d4)
Introduction of Cu pillar which has been used to replace lead-free  solder to achieve fine pitch chip-packaging interconnect which exerts  more higher stress in the ULK layer.

Emerging packaging solutions pose additional challenges to CPI   3D Integration using TSV technology   New process flow and material used

## Backside Integration challenges and main factors  contributing to CPI stress 

![contributing to CPl stress  Temporary Bonding:  IM o ld in g:   Si processing   : TTV control   Over mold   · BEOL/FBEOL layers   : Bond ing/debonding process  Exposed mold   Cu contamination control  Package warpage  Interconnects:  Assembly/Package  Processing:   TSTs   Fine pitch  Dicing ultra thin dies  microbumps  Singulation  Built-in stress  Ch ip-attach  encaDsmeton  Underfill Challenges:  Preapplied (NCP/NCF/NUF)   Material and thewmo-mechanical prope rties  Wafer applied    Stress induced by die-Laminate CTE  Capillary   m ismatch   Thermal properties    stress induced by Cu-pillars on low-k  Delamination  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c9c56333-6f67-47d6-b5ec-2eb2a0489505/c9c56333-6f67-47d6-b5ec-2eb2a0489505.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=c5c8474befc68c7d6bb6741077440fdb3e131611)
## CPI challenges in 3D package 

TSV Impact on BEOL

• doming effect observed after TSV chemical mechanical  polishing (CMP) process   • decreases metal 1 thickness thereby increasing its  resistance

![00506WCDense TSV  PotoD.  without doming without doming  (same wafer) (same wafer)  19.84nm   39.69nm   33.07nm   19.84nm  00506WEDenseTSV  PotoD.  with doming with doming  5.622mm  (same wafer) (same wafer)  19.84nm   39.69nm   33.07nm   33.07nm   26.46nm  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a3d9e84a-c9c8-4d78-9b8c-3e73f021b43a/a3d9e84a-c9c8-4d78-9b8c-3e73f021b43a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=bbd518bfef083186a612efb94a11242156324c76)
## Test structure to characterize reliability  impact from potential Cu protrusions 

![Pad1-V+ Pad2-1+ Pad 6-1+ Pad7-V- >Metal2(32nmwidth) Pad5-V+  Pad8-1 >TSV(6um) Pad3-V- Metal1(32nm width) Pad 4-|- ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4a64eb77-9008-45ce-9c99-abc016a27373/4a64eb77-9008-45ce-9c99-abc016a27373.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=ad21a25070212b75369f659730f3229ac6b29ade)
![Pad1-V+ Pad2-1+ Pad6-1+ Pad7-V- >Metal2(32nmwidth) Pad5-V+  Pad8-1- TSV(6um) Pad3-V- Metal1(32nm width)< Pad4-1- ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/333e600c-e071-41db-9ca3-07b77a6c5cf9/333e600c-e071-41db-9ca3-07b77a6c5cf9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=17856e227cd6ee8803a1ed933c432e0ea313030a)
M1 and M2 serpentines are aligned orthogonally     Test structure allows for M1, M2 resistance measurements  and leakage between M1, M2     Reference with no TSV underneath is required to provide  baseline

## Cu protrusion effect on interconnect resistance  for metals running directly above TSV 

![Probability Plot of Resistance  Weibull - 95%6 CI  50   100   2010  Wlafer 1o   Sancture  Post R5 Anneal   Mi-Serpentine  Post R5 Amnea   M2-Ser pentine  Post R5 Amned   TSV-Ml-Sarpentine  Post R5 Annea   TSV-M2-Serpentine  28898   Pre Anneal   Mi-Serpentine  Pre Amneal   M2-Sapantine  Pre Amneal   T5V-Ml-Sarpantine  Pre Amnea   TSV-M2-Serpentine  Shsps   0.598   0.19.  4.100   218.8   0.446   5-0.250  26.07   118.8   0.442   5-0.250  4.907   193.0   10.703   10.058  501   10o   200  Resistance  Shape  Scale:  Panel variable: Mx Level  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/571cb8c0-20d5-4136-94d1-ecb108f8d5c5/571cb8c0-20d5-4136-94d1-ecb108f8d5c5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215609%3B1743219209&q-key-time=1743215609%3B1743219209&q-header-list=host&q-url-param-list=&q-signature=39dfab25dd6e7c9cb37bdf3188a63efc048a30ad)
Cu pumping can affect BEOL, possibly reducing End-Of-Life (EOL) reliability   TSV-M1 Serpentine resistance distribution is degraded compared to reference M1 Serpentine  (left panel)     TSV-M2 Serpentine resistance is not affected (right panel)

S. Kannan et al., IMAPS New England Symposium, 2015

## Concluding Remarks 

Rapid access to memory, increased bandwidth & heterogeneous  integration are the main drivers for 3Di.

High Integrity Cu TSVs can be seamlessly integrated into CMOS  Technologies while achieving good Reliability performance.

3D IC Technology has the potential to become the pervasive  technology in the near future.

## Acknowledgements 

I would like to thank my colleagues for engaging in intellectually  stimulating discussions on 3Di Technology

Raman Kothandaraman (IBM)  Luke England, Daniel Smith (GLOBALFOUNDRIES)

I would like to thank my managers Byoung Min & Martin Gall for  their support.

