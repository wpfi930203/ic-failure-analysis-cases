---
title: "tut-2.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_b19c12c930390ab3fffd9743ebaa30a07295230462135641
file_size: 4687740
---

## Advanced Packaging technologies for chiplet  and memory integration 

Yan Li

Samsung Advanced Package Business Team (AVP),  San Jose, CA, USA

## Outline 

• Introduction    • Chiplet integration   • Memory integration   • Quality, Reliability, and FA challenges    • Conclusions

Introduction

## Why advanced packaging? 

Advanced packaging techniques are utilized to meet the market needs

![Microprocessor Transistor Count --- 2X every 2 years  1012   Apple  M2Uitra  1011  Moore'slaw  Moore’s law 1010  109   BN  108  107   AMD  10６  105   Motorola  104  intel  4004  103  19701980199020002010202020302040  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/83de03c6-6e0f-464a-b3ad-d1a4a4fb6490/83de03c6-6e0f-464a-b3ad-d1a4a4fb6490.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=bd5472e491c0e0d746b6d47c43b7f12c4cf07d78)
Moore’s law predicts the exponential growth  of ICs since 1970s- -- Market needs

https://semiconductor.substack.com/p/therelentless-pursuit-of-moores

![CostPerYieldedmm?fora 250mm²Die  200  450m   32n0   2.8mm   20nm:   Hn6nm   mmi  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/250e88d4-d24f-4428-9b9c-dcc14bd0b71b/250e88d4-d24f-4428-9b9c-dcc14bd0b71b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=33f7047a2b1f83bf6849aac805aab88d2245a3f6)
The exponential growth of cost per Yielded   $\mathsf{m m}^{2}$    for  $250\;\mathsf{m m}^{2}$    die  ---- Challenges for  Si level scaling and yielding

•  Chiplet •  Heterogeneous  integration •  Die stacking

Introduction

## Advanced packages on market 

Smaller interconnects; Higher performance; Lower power consumption

![CPU die  FLI  Substrate!   Microbumps  SLI  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ebdb6db8-dd76-45ec-993d-b7d8106f242b/ebdb6db8-dd76-45ec-993d-b7d8106f242b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=7c78556876d0538860f4e7e97286e5faaabb489c)
Embedded Multi-Die Interconnect Bridge  (EMIB) from Intel

![bor   DRAM  DRAM die   package  CPU die   Microbumps  POPsolder  TsW   joints  -Substrate  SLI  Foveros technology from Intel  Foveros technology from Intel ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7a3f4c99-8b30-4517-b687-417fd4794d6c/7a3f4c99-8b30-4517-b687-417fd4794d6c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=4fbcbb8faf04426c4b02c88db8258897442cf68f)
![GPU  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b6ed6d18-8266-46bd-a831-d4706933cdf2/b6ed6d18-8266-46bd-a831-d4706933cdf2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=0bfb60f7a9a3c0348141ad15e523f41d5bd8a773)
![Silnterposer  Substrate  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/74b00140-d9b7-42bf-9da0-a8d81423ba2e/74b00140-d9b7-42bf-9da0-a8d81423ba2e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=5c559b88e00436ff3e777e756fa8ab1f13ecd620)
AMD Radeon™ Fury

Chip-On-Wafer-On-Substrate (CoWoS) from TSMC

![HBN   HBM  SiliconInterposer  SUBSTRATE  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/183f1f4f-2dc8-4e58-bb06-8dc8b3028990/183f1f4f-2dc8-4e58-bb06-8dc8b3028990.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=7eb54a854614c327018b16dc8f696434eff23bef)
AMD Instinct™ MI300 Family

3D Hybrid bonded chips on  CoWoS from TSMC

3D Microelectronic Packaging: From Architectures to Applications, 2 nd   edition, Springer, 2021, ISSN 1437-0387  https://www.club386.com/amd-instinct-mi300-architecture-speaks-to-massive-ai-performance/

Introduction

https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10195617

Smaller interconnects; Higher performance; Lower power consumption

![HBM   Logic   HBM   Cu-CuHybridBond  HBM   Logic   HBM  NIold   HBM   3DASIC   HBM   -Stiffener  SiInterp   TSV  Siinterpos  si-bridge   siHbridge   RDLinterpo  gooo  I-Cube S: Si interposer from  I-Cube S:  Si interposer from   I-Cube E: Embedded Si bridge  I-Cube E:  Embedded Si bridge   3.5D packaging hybrid bonding 3D chips on Si  3.5D packaging  hybrid bonding 3D chips on Si   Samsung  Samsung  RDL interposer from Samsung  RDL interposer from Samsung   interposer from Samsung  interposer from Samsung Hybrid Cu Bonding  μBump(TCB)   Bumpless(HCB)  X-Cube: logic to logic die  X-Cube:  logic to logic die   X-Cube: logic to logic die  X-Cube:  logic to logic die   16H HBM by HCB  16H HBM by HCB  from Samsung  from Samsung  stacking- μBump from Samsung  stacking- µBump from Samsung   stacking- Hybrid Cupper Bonding  stacking- Hybrid Cupper Bonding  Samsung  Samsung ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e62b662c-7165-4d76-9032-01086f8e6115/e62b662c-7165-4d76-9032-01086f8e6115.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=a00e18e57f75bbced598c743200a1aba13ce555a)
W. Kim, “Advanced Packaging in the Era of HPC and AI” Seventh Annual Symposium on Heterogeneous Integration, February, 2024. https://ieeetv.ieee.org/video/heterogeneous-integration-platform-for-next-generation-computing-beyond-moore

Introduction

## Assembly Technology Development Challenges 

3D Microelectronic Packaging: From Architectures to  Applications, 2 nd   edition, Springer, 2021, ISSN 1437-0387

• Assembly Process Challenges

•  More challenging assembly steps (TSV, COW, TCB, die embedding, substrate process)   •  Yield and defect monitoring for each step   •  Cost reduction reducuon

![CPUdie  FLI  Microbun  Substrate  (a)DietoWaferBonding  SLI-Epoxyflux   TCB Head  (b)CarrierDe-bonding  EpoxyFluxDispense   TCBProcess   UnderfillCure  Fig.10.6 Schematics of TCB using epoxy flux  (d)Package Attach  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9c12daf3-728f-4a17-9738-ca512153655e/9c12daf3-728f-4a17-9738-ca512153655e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=9ee0f8799f1cf2933d64baa9cb5db7cc928d7e55)
![SYSTEUMPI  Diameter20um  Pitch46um  TSW  vDia  neter6un  Pitch46um  Micro-bu  VDiameter  22m  Pitch92.5um  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/955f3b19-246c-4109-8b11-b8d8be23f117/955f3b19-246c-4109-8b11-b8d8be23f117.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=7dc63166e0a5160d1da4c6a2d75572d97be3e606)
Introduction

## Assembly Technology Development Challenges 

3D Microelectronic Packaging: From Architectures to  Applications, 2 nd   edition, Springer, 2021, ISSN 1437-0387

• Thermal Management, Package Design, and Modeling Challenges

•  3D stack increases the complexity of heat paths    •  Very complicated Packagee design: design software   •  Thermal Mechanical Modeling Challenges

Fig.4.11Distributionofthe vonMisesstressina Cu-TSVstructurefroma linearelasticmechanical modelwithCugrain microstructure[45]

![Heat Spreader   DRAN  Processor   DRAM   Dcessor  Package  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cef7c355-ebeb-4099-848a-4e04b2c8132d/cef7c355-ebeb-4099-848a-4e04b2c8132d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=0b7f2f2da20b66493efc945e7be384ae31e8d340)
![MPa  350  80  125  60   100  SO  VS  40  30   SO  20  2S  1O  20  30   40   SO  x,m  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a8e97da4-83f4-4583-b8b5-f53912a2120d/a8e97da4-83f4-4583-b8b5-f53912a2120d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=f29dd1ae94db61b90a3bf6e80d2aab8df620b5b0)
Introduction

## Assembly Technology Development Challenges 

3D Microelectronic Packaging: From Architectures to  Applications, 2 nd   edition, Springer, 2021, ISSN 1437-0387

## • Material and Substrate Challenges 

•  Flux, epoxy, Non-Conductive Film  (NCF) material challenges  •  Substrate process challenges (small  vias, Through Holes, trace to trace,  embedding die etc)

![E-lyticCuplating  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a93a365f-25fa-4416-a752-1421722a1914/a93a365f-25fa-4416-a752-1421722a1914.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=b97fb042ed925c4db0907c115c43dba8ce79f7a0)
![TCB  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e747f09f-b511-4939-be59-a4b2d92fcdfa/e747f09f-b511-4939-be59-a4b2d92fcdfa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=eb9c0f7584c70397a84d320f7b77ca05b10c339d)
## Introduction 

## Advanced Packaging Development trends Transition from Solder Based Interconnects to Cu-Cu interconnects  

![TopDie   Y. Kim et al, ECTC 2023  Y. Kim et al, ECTC 2023 Cu-Cu bond Cu-Cu bond  Hybrid Cu  Hybrid Cu  5555554  Bonding  Bonding   CuPad  dngnt  (HCB)  (HCB) Top Die  Buier   4u  Thermal  Thermal   &BEOL  FEOL  Compressive  Compressive   Pb-freeC4  Bonding (TCB)  Bonding (TCB) BumpPitch(μm)   Grind side  TSV  10:   20   30   40   50   Device side   Thinned Die  Ravi Mahajan, ISTFA 2021 RaviMahajan,ISTFA 2021   FEOL  &BEOL  •  Die to Die (D2D) interconnect scaling down: HCB replacing TCB  Die (D2D) interconnect scaling down: HCB replacing TCB  Pb-freeC4    Tighter bump pitch; smaller bumps  Tighter bump pitch; smaller bumps  Solder based  Solder based   Gapless -thermal advantages  Gapless –thermal advantages ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1fdb77c7-f57f-4a73-869e-371dd630ec44/1fdb77c7-f57f-4a73-869e-371dd630ec44.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=de4cad30ebf8860d7eb92a29ff376d6e40e4ef34)
3D Microelectronic Packaging: From Architectures to Applications, 2 nd   edition, Springer, 2021, ISSN 1437-0387

Introduction

## Advanced Packaging Development trends 

The Boundary between Si and Advanced Packaging is blurring HCB is replacing TCB

![3μm pitch  3µm pitch 9µm pitch 9um pitch   1μm pitch  1µm pitch  0.4μm pitch  0.4µm pitch DoW  DoW  wow  WoW 10um  7.20kx   58.2um   8.18mm  Scan Mode  9OOPA   UH-RESOLUTION   2k0v  Cu-Cu Hybrid Bonding enables aggressive pitch scaling to   1µm ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7a254727-2d8d-457b-87ba-3437692656fb/7a254727-2d8d-457b-87ba-3437692656fb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=46df3203978eeb65a413174b7168cc820a0a5993)
P. Tadayon, IMPAPS DPC 2024

Introduction

## Advanced Packaging Development trends 

Glass interposers and Glass substrates

![Glass Interposers  Glass Interposers  Glass substrates Glass substrates  Chip   Chip   Chip     Chip  Chip   chip  Interposer(Glass)   Interposer  Glass Core  Laminate Core   Giass  Core  •  Thin  Thin  •  Thick  Thick •  2-3 RDL  2-3 RDL   •  10+ RDL   RDL  layers layers   layers  layers ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/75fc691b-e0c3-42b2-9d1a-91ae901e9bf1/75fc691b-e0c3-42b2-9d1a-91ae901e9bf1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=acc5dc02cda82d5b2e6557af07dcd554c055ee87)
## Glass has excellent  properties 

Mechanical  (Smooth; High Young’s  modulus)     Environmental  (Chemically Robust;  Impermeable to  Moisture; High T  Compatible)     Electrical (High  Resistance; Low Loss  (GHz))

P. Tadayon, IMPAPS DPC 2024

## Introduction Advanced Packaging Development trends 

![Rapid adoption of Advanced Packaging in Si Photonics  3DEIC stackonPIC  IMicro-pillars  2.5 D Flip chip  Host chip (ASIC,FPGA..  withEMIB   TSW  BGA laminate  Wire bond  PCB(motherboard)  2D   WireBonds  OpticalFibers  PhotonicIC   Electronic  POB  FPGADie   O-Tile  O-Tile  2.5D  ElectronicIc  OpticalFiber  PhotonicIC   solderBu  UuuCu Pilars uu  2.5DFlipchipInterposer  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c9cb7b57-1bcb-423e-a146-84c1e3d9a910/c9cb7b57-1bcb-423e-a146-84c1e3d9a910.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=ab5269b1c061f85fd2f3939f0efe9b3c425011bb)
## Chiplet integration 

## Chiplet; Heterogenous integration; die stacking 

![Con   Gen   oon   Gen  Nnode   NN-1  mon   non  Specialty  PKG  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/684998cc-4f1a-4501-bcc8-c83d56663705/684998cc-4f1a-4501-bcc8-c83d56663705.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=5976c4785c1bbd490eac5239adc2e27a98fe1c2c)
![memory memory  N N-1  N-1 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bb36fdc5-2893-491f-8db2-27a987092ab1/bb36fdc5-2893-491f-8db2-27a987092ab1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=bf9357c47e754c2571293d5d42d2ff2f5a5fd69a)
High yielding smaller chips and  optimal process selection

Modular design, design reuse and  mix & match

Die stacking  footprint reduction

M. Kang, “Heterogeneous Integration Platform for Next Generation Computing” Sixth Annual Symposium on Heterogeneous Integration, February, 2023.

## Chiplet integration 

Technical and Logistic Challenges

•  Multi-domain co-design  involving both  power  and  signal  routing   •  Thermal management   •  Facilitate Industry open platforms and  standardizations  for high-speed and low power chiplet D2D  communications: Universal Chiplet Interconnect Express (UCIe), Bunch of  Wires (BoW), and High Bandwidth Interconnect (HBI) etc.   •  Establish and Clarify Agreements  on Si security and  responsibilities in yield, Known Good Die (KGD), product or chiplet quality  and reliability.

Y. Li, et al, IMAPS DPC, 2024

## Chiplet integration 

Advanced Packaging (AVP) Turnkey solutions

![Foundries   MemoryVendors   Edpa  Design methodology  Customer   Design, Specs,   Packaged   Chiplet IF   Including memory  Outsourced si,   Products  Memory   CsiP)  OSAT   Cooperation  Samsung Foundry   AVP   Samsung Memory  Samsung Sip Platform   PB   & More Supply Chain  Uitimate System-in-Package Provider: Flexible Service + Synergy Platform  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/61d6706f-0d60-451f-bb55-c26fd7f71944/61d6706f-0d60-451f-bb55-c26fd7f71944.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=44ba41105c1f1451d9a3a42a13e03659916e27c0)
End to End, Flexible, Synergy, Eco system

M. Kang, “Heterogeneous Integration Platform for Next Generation Computing” Sixth Annual Symposium on Heterogeneous Integration, February, 2023.

## Chiplet integration 

Chiplet Based Heterogeneous Integration Platform

|rype|        Current                offering      |Roadmap|Pictures|Type|        Current                offering      |Roadmap|Pictures|
|---|---|---|---|---|---|---|---|
|PLP|        RDL L/S: 5μm;Bump                pitch: 90μm; Pkg-                thickness:0.58mm      |        RDL L/S: 5μm;Bump                pitch: 90μm; Pkg.                thickness:0.58mm      |FOPLP|I-Cube E|        Interposersize: 3x                reticle; #of HBM: 8x;                μbump pitch: 40μm;                Interposer C4 pitch:                150μm; Package                size:85x85mm²      |        Interposer size: 4+                reticle; # of HBM: 12x;                μbump pitch: 25μm;                Interposer C4 pitch:                125μm; Package size:                100x100mm²      |Lo9c|
|UALIP|        RDL L/S: 2μm;Bump                pitch: 90μm; Pkg-                thickness:0.35mm      |        RDL L/S: 1um; Bump                pitch: s75um; Pkg.                thickness:0.33mm      |FOWLP|I-Cube E|        Interposersize: 3x                reticle; #of HBM: 8x;                μbump pitch: 40μm;                Interposer C4 pitch:                150μm; Package                size:85x85mm²      |        Interposer size: 4+                reticle; # of HBM: 12x;                μbump pitch: 25μm;                Interposer C4 pitch:                125μm; Package size:                100x100mm²      |Lo9c|
|UALIP|        RDL L/S: 2μm;Bump                pitch: 90μm; Pkg-                thickness:0.35mm      |        RDL L/S: 1um; Bump                pitch: s75um; Pkg.                thickness:0.33mm      |FOWLP|        X-Cube                (TCB)      |        Bump pith: 25μm;                Silicon thickness:                -40Pm      |        Bump pitch: ≤21μm;                Silicon thickness:                c40m      |        μBump(TCB)                S      |
|tubes|        Interposersize: 3x                reticle;#of HBM: 8x;                μbump pitch: 40μm;                Interposer C4 pitch:                150μm; Package                size:85x85mm²      |        Interposer size: 4+                reticle;#of HBM: 12x;                μbump pitch: 25μm;                Interposer C4 pitch:                125μm; Package size:                100x100mm²      ||        X-Cube                (TCB)      |        Bump pith: 25μm;                Silicon thickness:                -40Pm      |        Bump pitch: ≤21μm;                Silicon thickness:                c40m      |        μBump(TCB)                S      |
|tubes|        Interposersize: 3x                reticle;#of HBM: 8x;                μbump pitch: 40μm;                Interposer C4 pitch:                150μm; Package                size:85x85mm²      |        Interposer size: 4+                reticle;#of HBM: 12x;                μbump pitch: 25μm;                Interposer C4 pitch:                125μm; Package size:                100x100mm²      ||        X-Cube                (HCB)      |        Bump pitch: 4μm;                Silicon thickness:                10pm      |        Bump pitch: ≤3μm;                Silicon thickness:                c10pwm      |Bumpless(HCB)|
|||||||||


M. Kang, “Heterogeneous Integration Platform for Next Generation Computing” Sixth Annual Symposium on Heterogeneous Integration, February, 2023.

Y. Li, J. Yang, K. Chatterjee, P. Asrar, S. Jeong, and W. Kim, “Advanced package technologies for chiplet adoption and memory integration in HPC/AI applications”, OCP global summit, Future Technologies symposium, October 18, 2023, San Jose.

## Chiplet integration 

## Higher Thermal Design Power requirement leads to Power Integrity (PI) Challenges 

![Thermal Design Power (TDP) growth in CPU and GPU  Thermal Design Power ( TDP) growth in CPU and GPU PowerSupportVs.TechnicalFluidTemperature  2030  2029  2028  S0  2027  50  50  2026  ea  409  2025   D  2024   300  30  2023  20  2022  1O  2021  2020  100   200300400  500600700800900100011001200130014001500  Power(w)  GPUPower   CPUPower   Technical FluidTemperature  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d68ef834-5a8b-4804-8c02-f7d3b7766ea1/d68ef834-5a8b-4804-8c02-f7d3b7766ea1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=36093edf827b147a38e5c97284dd1aa1f9908147)
H. Dhavaleswarapu, IMAPS DPC, 2024

![LEADINGSUPERCOMPUTER  PERFORMANCE  1exaFLOP  Frontier  1petaFLOP  1gigaFLOP  19901995200020052010201520202025  Source:https://www.top500.org  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/70406ea1-c81d-4c39-8af8-1ad1d436ad17/70406ea1-c81d-4c39-8af8-1ad1d436ad17.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=c4e58cffe5b944c9dfa7b4c51801996a08936d7b)
## Chiplet integration 

## Novel Integrated Stack Capacitors (ISC) integration 

![2um  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9aaabc71-6449-4c85-9a76-47f52e71cfcf/9aaabc71-6449-4c85-9a76-47f52e71cfcf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=9c3dcc8981df8f0e2692a176c3b7e9b599e5303d)
Schematic illustration of ISC with a silicon  area of 2 × 2 µm 2

•  High Power demands in HPC   •  Low impedance Power Distribution Network  (PDN)    •  Capacitors with small form factors, high  capacitance density, stable at high T.

||        Metal-Insulator-                Metal (MIM)      |        Deep Trench                Capacitor (DTC)      |        Integrated Stack                Capacitors (ISC)      |        Multilayer Ceramic                Capacitor (MLCC)      |
|---|---|---|---|---|
||Highk dielectr||D000000||
|Cap. density|×1-0|×7.5|×7.5|×7５|
|Cap. Height|≤2μm|～ 30μm|～2pm|~ 1mm|
|        Cap. density                change with T?      |20|20|20|Drop at high T|


E. Song, D. et al, “Power Integrity performance Gain of a Novel Integrated Stack Capacitor (ISC) Solution for High-end Computing Applications”, IEEE   $70^{\mathrm{th}}$    Electronic Components and Technology Conference (ECTC), 2020, pp. 1358-1362.

## Chiplet integration 

Novel Integrated Stack Capacitors (ISC) integration

ISC

ISC

ISC

ISC

ISC

Si

ISC is embedded

between metal layers  in a Si interposer

ISC die is embedded  inside a RDL  interposer along with  the bridge dies

## Chiplet integration 

## Novel Integrated Stack Capacitors (ISC) integration 

![- Board Cap  Board Cap + PKG Cap  "".."Board Cap +PKG Cap+ISC  Impedance  Impedance  drop with ISC  drop with ISC   10M1   100M   1G   Frequency (Hz)  HBM   Logic   HBM  snter  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e6a2da39-6cbf-4481-8405-6c706eab6162/e6a2da39-6cbf-4481-8405-6c706eab6162.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=6a17d35715833c3638e4532afd39b14dfc3557ea)
M. Kang, “Heterogeneous Integration Platform for Next Generation Computing” Sixth Annual Symposium on Heterogeneous Integration, February, 2023.

Modeling showing  significant impedance  drop at high frequency  range by adding ISC to Si  interposer

E. Song, D. et al, “Power Integrity performance Gain of a Novel Integrated Stack Capacitor (ISC) Solution for High-end Computing Applications”, IEEE 70 th   Electronic Components and Technology Conference (ECTC), 2020, pp. 1358-1362.

![Current  ISC Cqp density  1.350 6   2,2002   2.750  (nF/ mm2 )  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/55bf268c-1bc7-4ea4-821c-b5a4b4043c03/55bf268c-1bc7-4ea4-821c-b5a4b4043c03.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=8ee4b717d17aebf06ab61868ac27f5c26439e8c8)
## Chiplet integration 

## Chiplet integration development trends 

![uBump(TCB)   Cu-CuHybridBond  HBM   Logic   HBM  3DASIC  Mold-   HIBNI   HIBNI   -Stiffener  si Interposer   SiInterposer   TSV  Substate  3.5D  3.5D 2.5D  2.5D  3D  IMicro-pillars   CPO  CPO Bumpless(HCB)  HBM   Logic   HBM  Host chip(ASIC,FPGA,..)  TSV  SiHbnidg   RDLinterpose  BGA laminate  PCB (motherboard)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e907cdc0-3ed8-44da-8f8b-42174964002b/e907cdc0-3ed8-44da-8f8b-42174964002b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=0cc00e4f7bb4812ecd9865ab92c9effd0681d75b)
## Chiplet integration 

Chiplet integration development trends

![TSVPitch  DRAMonCPU   Coreson Cores   Die2   Die2  CPUonCPU  CoresonUncore   Die'1  Die1  FULLDIE-TO-DIE   IPONIP   MACROINMACRO   CIRCUITSLICING  FOLDING/SPLITTING  C.Buch, IMAPS DPC, 2024  C. Buch, IMAPS DPC, 2024 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b31e853a-8666-4617-a7d4-771eb2b1ed0d/b31e853a-8666-4617-a7d4-771eb2b1ed0d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=4fee8162962d9b5579e5cd6b5dba3bfe292542ce)
## Chiplet integration 

## Chiplet integration development trends 

## Dramatic scaling down of interconnects in 3D Packaging 

![1E+08   0.1  nTSV (BSPDN)  1E+07  E    W2W HB - imec R&D  1E+06   I W2W HB - industry  △. D2W HB - imec R&D  1E+05   w2W口   . D2W HB - industry   D2W μBump - imec R&D  1E+04   D2W μBump - industry  1E+03   D2WV μbump  D2W= Die-to-wafer bonding  W2W= Wafer-to-Wafer bonding  HB= Hybrid bonding  1E+02   100  2005   2010   2015   2020   2025   2030  Year  mnec   AC  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/49746c61-e71f-49fc-8d3e-e3077b73da53/49746c61-e71f-49fc-8d3e-e3077b73da53.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=2474a9c56f1cc8134b9505575f1e6e7c91ae8831)
Design   Process   Yield & Reliability Failure Analysis

Adopting  well-developed  methodologies  currently  used in  Si Fabs  to advanced  packaging area is  imperative  to meet the short product  development cycle demands

## Memory integration 

Various Memory types and integration techniques

![HBM  Logic  BufferlessHBM  Interposer  LLV  Logic   Logic  RDDL  Cache DRAM   2.XD   OWPO   609  LPDDR  Logic   Interposer  Bridge  3.5D   Logic  0601+2607   3DD   FOPKG  uBump/HCB   PLP/WLP  Logic/SRAM  Platform Map   Logic  LPDDR  Logic   Substrate  B/VW   Platform   Configuration   Technology   Technology   Configuration   Platform   B/V  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/185674ff-7400-4e12-bee0-23510b6951f0/185674ff-7400-4e12-bee0-23510b6951f0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=e32aae072a01b2f5c202f408b2f72c8b3d3411df)
M. Kang, “Heterogeneous Integration Platform for Next Generation Computing” Sixth Annual Symposium on Heterogeneous Integration, February, 2023.

## Memory integration 

## Memory integration Challenges 

•  Memory and Bandwidth limited Era after GPT-2 •  Bigger and 2.5 & 3.5 D packages for more chiplet and  HBM integration •  Innovative memory integration approaches are needed.

![Performance and market needs  driveBigger Packages for more chiplet  and HBM integration  Assembly Challenges of bigger packages  call for innovative memory  integration approaches  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e9c89d8d-40fd-4c81-8c71-8dda0a72e8be/e9c89d8d-40fd-4c81-8c71-8dda0a72e8be.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=0d38dfd840dd8b1c81b02cb2e625609e2e6513ce)
![Compute   MemoryandBandwidth  Limited Era   LimitedEra  wodel  10T  Parameter   DLRM-10T  Model Parametor   GPT-4  Memory  Memory Capecity   PaLM   wal  I0OB  AMDMI300x（192GB)  Megatr  10B  100(80GB)   NvidiaH200(141GB)  TPUV2(64GB)  TPUV3（32GB)   Nvidia H100(80GB)  NvidiaV100(32GB)   nferentia2(32GB)  GPT-2  1B  NvidiaP100(16GB)  ·BERT  GPT1  ResNext-101   TransformerSize:240x/2years  Inception   ResNet-50   AIHWMemory:2X/2years  2015   2016   2012   2018   2019   2020   20212022202320242025  https://www.celestial.ai/technology nnology  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/af98f94e-51cc-46db-ae63-37af059e02d2/af98f94e-51cc-46db-ae63-37af059e02d2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=7213db8861ee779f554c44005c4777e37e450e6c)
Y. Li, J. Yang, K. Chatterjee, P. Asrar, S. Jeong, and W. Kim, “Advanced package technologies for chiplet adoption and memory integration in HPC/AI applications”, OCP global summit, Future Technologies symposium, October 18, 2023, San Jose.

## Memory integration Memory Integration development trends 

## 3D Memory Integration 

![DRAM die  stack  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/536bfff6-9103-4a11-9cdb-3f5a09041a23/536bfff6-9103-4a11-9cdb-3f5a09041a23.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=9088be60a058f0b1aa37b845b371568c756b56e3)
3D custom HBM

![Cache DRAM  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/47c2fbf0-1525-40a6-bf6d-f91c1bb1c32b/47c2fbf0-1525-40a6-bf6d-f91c1bb1c32b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=42395201bb64f8eed0e3916c6be5b13c1d5bdc4b)
## 3D Cache Memory 

Y. Li, J. Yang, K. Chatterjee, P. Asrar, S. Jeong, and W. Kim, “Advanced package technologies for chiplet adoption and memory integration in HPC/AI applications”, OCP global summit, Future Technologies symposium, October 18, 2023, San Jose.

## Memory integration 

## Memory Integration development trends 

## HCB replacing TCB in 3D die stacking  

Cu-Cu replacing solder based  micro bumps

•  \~  ×  100 denser  interconnects   •  Up to  $\pmb{\times}$   150 more bandwidth   •  Up to  30% more allowable power

![Solder based micro bump by TCB  Solder based micro bump by TCB   Cu-Cu by HCB  Cu-Cu by HCB  >20µm in bump size and pitch >20um in bump size and pitch   A few μm in bump size and pitch  A few µm in bump size and pitch ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/20779e90-3d77-428a-8a7d-9180c5624d95/20779e90-3d77-428a-8a7d-9180c5624d95.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=bf5973ceb2cd0ef960e0c60ad63fc4cb4cc8a2b1)
Y. Li, J. Yang, K. Chatterjee, P. Asrar, S. Jeong, and W. Kim, “Advanced package technologies for chiplet adoption and memory integration in HPC/AI applications”, OCP global summit, Future Technologies symposium, October 18, 2023, San Jose.

## Memory integration 

## Memory Integration development trends 

## HCB replacing TCB in HBM  

![TCB   HCB  Thermo-CompressionBonding   Hybrid CuBonding  Ws.  chip chiip  Gapless  Chip gap  Chip gap chip  chip ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f555659a-f3d5-4b0b-9184-074fc810e877/f555659a-f3d5-4b0b-9184-074fc810e877.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=b2b97a561c4e4daa9b1d255243e7d1349bf7bf70)
W. Kim, “Advanced Packaging in the Era of HPC and AI” Seventh Annual Symposium on Heterogeneous Integration, February, 2024.

## Memory integration 

## Memory Integration development trends 

## Optical Interconnects could be a promising approach 

•  Exceptionally high bandwidth densities   •  Ultra low power consumption per bit or per distance

![HBM HBM   Logic   HBM HBM  Photonic interposer Photonicinterposer  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ad98c125-0a79-4040-a00f-a6743f39e3aa/ad98c125-0a79-4040-a00f-a6743f39e3aa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=c67e74858427522f6cb55b798058ad1b53db7b7c)
Development trend:  Optical interface between  HBM and Logic

![HBMHBM  HBM Logic  optical meo!ndo  HBMHBM  HBM optical ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/76caaa2f-edf0-450c-8104-e7c85d092c89/76caaa2f-edf0-450c-8104-e7c85d092c89.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=327cddee6ce830381a20726d5bea1b33c132c017)
Development trend:  Optical connection between  logic and HBM packages

M. Tan, et al “ Co-packaged optics (CPO): status, challenges, and solutions”, Frontiers of Optoelectronics”, 16:1, 2023   N. Pleros et al “Optical Interconnect and Memory Technologies for Next Generation Computing”,  2016 18th International Conference on Transparent Optical Networks (ICTON), Trento,  Italy, 2016, pp. 1-4, doi: 10.1109/ICTON.2016.7550267.    Y. Li, J. Yang, K. Chatterjee, P. Asrar, S. Jeong, and W. Kim, “Advanced package technologies for chiplet adoption and memory integration in HPC/AI applications”, OCP global summit, Future Technologies symposium, October 18, 2023, San Jose.

## Quality, Reliability, and FA challenges  

## Quality and Reliability Concerns 

![Infant  Wear out  Mortality  failures  failures  fCt）  Intrinsic failures  Extended  11   TTime  test time  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1d279033-52c3-42e0-a4a7-c7f1a901d69a/1d279033-52c3-42e0-a4a7-c7f1a901d69a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=f893df892a016e43071d63f9f9afb92be5c3f160)
Schematic of Bathtub curve showing failure rate versus  reliability test time

##   Product Use Condition   Reliability Tests: 

Preconditioning (PC) Test    $\checkmark $  Temperature Cycling (TC) Test     $\checkmark $  Baking Test     Unbiased Highly Accelerated Stress Test  (UHAST) and Biased Highly Accelerated Stress   Test (BHAST)     $\checkmark $  Interconnect Electron Migration (EM) Test     Thermal Test

## Quality, Reliability, and FA challenges  

## Quality and Reliability Concerns 

3D Microelectronic Packaging: From Architectures to  Applications, 2 nd   edition, Springer, 2021, ISSN 1437-0387

## Failure Mode examples 

![Blister/delam  TSAM   ross section  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0e9fc81b-1952-4f94-b55b-5cd2a8cbcb73/0e9fc81b-1952-4f94-b55b-5cd2a8cbcb73.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=c16ee4803d1305a8a152703dc4acc2f109cccc65)
![s5-20m  Microbumps  Flipchip  solder joint (C4)  BGA  Laminate  BGAsolderjoint  PCB  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b696fbcd-9f4a-4a21-ae3e-e61d3a8cef24/b696fbcd-9f4a-4a21-ae3e-e61d3a8cef24.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=4334b7a652d2127c3433ab1558b07bcf0c910575)
Noscalebar

## Quality, Reliability, and FA challenges  

## Why FA? 

• Identify defects of Electrical Device Failures (post reliability  tests or at End of Line)   • Investigate root cause of the failures (Propose failure    mechanisms)   • Provide data feedbacks and solution paths for problem solving.

## Quality, Reliability, and FA challenges  

## FA Challenges from Technical Point of View 

![memorydice  Micro-bumps  logic die  FLI solderjoints  substrate  SLI solder  Ejoints  PCB  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ca5c296b-ea68-4158-b431-d6710cd13839/ca5c296b-ea68-4158-b431-d6710cd13839.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=50bb93408801b0a134a1d059025d061194f86e16)
•  Physical Failure Analysis:  1) artifact  free 2) revealing fine features in a large area •  Material analysis:  1) ppm level  contamination at interface; 2) organic materials  with sub micron resolution

•  Electrical Failure Analysis:  1) Multiple  failures in one unit. 2) Each failure needs x, y,  and z identification •  Imaging:  1) Non-destructive. 2) high  resolution 3) large field of view

![TSV voids TSV voids  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/be753abb-106a-4fe2-809b-44edf8cbc6c9/be753abb-106a-4fe2-809b-44edf8cbc6c9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=a52dffbead203768b9127f8a930aec45e26c5c2d)
Quality, Reliability, and FA challenges

## FA Challenges from Business Point of View 

Demand of Short product develop timeline; High volume manufactory; Cost saving

•  Low Cost   •  Short Through Put Time (TPT)   •  High Success Rate

3D Microelectronic Packaging: From Architectures to  Applications, 2 nd   edition, Springer, 2021, ISSN 1437-0387

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f3f0a522-a487-40a9-bb5d-6731b33e9a70/f3f0a522-a487-40a9-bb5d-6731b33e9a70.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=45ae3d940bd7b8dd4ec8333182cefbb27509dd29)
## Quality, Reliability, and FA challenges  

## Generic failure analysis flow  

![Problem   Failure analysis  Statement Review   report  Failure Verification  High-resolution imaging  and/or Physical Failure  Analysis & Material  Verified  Analysis  Failure ?  YES  YES  Non-destructive  Defect  inspection for  located?  possible gross defects  Gross   rO   ElectricalFailure  defects?   Analysis  Y"ES  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ff0be222-962f-41a7-8f14-0f59cd8b0c6d/ff0be222-962f-41a7-8f14-0f59cd8b0c6d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=d850c55157940b95d6e30d4947475ba7fd244597)
Schematic of failure analysis flow.

•  Problem statement review   •  Failure verification,    •  Non-destructive investigation    •  Electrical Failure Analysis   •  High resolution imaging or Physical  Failure Analysis  (Sample Preparation;  Defect Imaging; Material Analysis)

## Quality, Reliability, and FA challenges  

## FA workflow: Problem Statement Review  

The most critical step for successful failure analysis

•  Failure occurrence condition  and history— EOL? Post Reliability  test? Customer Return?   •  Failure rate analysis ---- Failure  rate at EOL; Failure rate vs Reliability test  time   •  Historical failure analysis  data leveraging

![Infant  Wear out  Mortality  failures  failures  fCt）  Intrinsic failures  Extended  TTime  test time  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/40d3ec9b-e285-4ba6-a496-0d8e40aca281/40d3ec9b-e285-4ba6-a496-0d8e40aca281.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=deff07b6b6db8669220a356d3a612e7cbac9dc25)
Schematic of Bathtub curve showing failure rate versus  reliability test time

## Quality, Reliability, and FA challenges  

## FA workflow: Failure Verification  

Common tester contact issues, test program immaturity, and failure intermittency

![Current(A)  0.6  Voltage (v)  -0.6  Fail  Pass  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/32da540d-56ac-404b-87c4-706ef2816c6d/32da540d-56ac-404b-87c4-706ef2816c6d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=45545a5ccd25597df53be29998b8a2d157d5641a)
I-V curve trace from a passing (in green) and a failing  unit (in red).

•  Parametric Failures —  I-V Curve  trace; Resistance or Current measurement;  comparing with those from a test good device •  Functional Failures —  Debug  testers and test programs; compare results  from “failing” vs “passing”

## Quality, Reliability, and FA challenges  

## FA workflow: Non-destructive investigation 

•  Optical Microscopy   •  Infrared (IR) Imaging   •  Scanning Acoustic Microscopy (SAM)   •  2D X-ray

![Fast TPT for units  Fast TPT  for units  having Gross Defects  having Gross Defects ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/24b1697c-4dbc-4de1-9f86-9beec1cf65a6/24b1697c-4dbc-4de1-9f86-9beec1cf65a6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=5237ef1941c6bab18187bcc475d5f35df31452a0)
![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/33e114a0-1da0-4c9a-b066-1549c2d7d7a8/33e114a0-1da0-4c9a-b066-1549c2d7d7a8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=db066875ff93e3d5116ebcc02391713cd04ad1e9)
TSAM of a PCB with embedded chips showing defects  in one embedded chip

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0150d199-f5b5-4a9e-ba97-d14300ec1e52/0150d199-f5b5-4a9e-ba97-d14300ec1e52.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=25b9f24857ebc84bf20026a07d05078d13589560)
2D X-ray images taken non-destructively and the corresponding  optical images of FLI solder interconnects cross sectioned post  2D X-ray imaging: (a) & (e) normal or defect free, (b) & (f)  partial non-wet, (c) & (g) complete non-wet, (d) & (h) noncontact open

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/744227d6-2196-46f1-b454-3151086947b6/744227d6-2196-46f1-b454-3151086947b6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=2bef40a0f73082457f9d3665e4a7de08abdca4f1)
IR image taken from die backside showing  internal die cracks highlighted by the red arrows

## Quality, Reliability, and FA challenges  

## FA workflow: Electrical Failure Analysis (EFA) 

locate tiny defects in very complicated electrical systems

•  Parametric failures — Timedomain reflectometry (TDR), Lock-In  Thermography (LIT), Magnetic Field Imaging  (MFI), Micron probing   •  Functional failures---- Optical fault  isolation tools, E-beam imaging and probing  techniques, nanoprobing   •  Non-destructive, High  resolution, providing x, y, z  location of defects

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9dca4aaf-7e1c-40cb-a683-2f4e7a1e19bf/9dca4aaf-7e1c-40cb-a683-2f4e7a1e19bf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=4c5894eafa62a53e4648e8a5693cc66a2ecfe8c4)
![AP3  MC Die3 A中 DAT Die2 AD1 DAI ie Leadframe 250 Die1 200 150 Die2 100 SO  中  Die3 AΦ3 10  15  20  25  30 lock-infrequency(Hz) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/03b2440d-6daa-46dd-ba9c-ab7e8baf88d4/03b2440d-6daa-46dd-ba9c-ab7e8baf88d4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=675dbb552d227f747a9743d5bd9d60ac08379a9c)
Measurement results of  Lock-in frequency vs phase  shift curves from reference  units with short failures at  die 1, die 2, and die 3 of a  package with stacked die  configuration showing in  dots compared to a  calibrated simulation model  (lines)

## Quality, Reliability, and FA challenges  FA workflow: High resolution imaging 

3D Microelectronic Packaging: From Architectures to  Applications, 2 nd   edition, Springer, 2021, ISSN 1437-0387

![•  3D X-ray Computed Tomography (CT)  3D X-ray Computed Tomography (CT) •  High resolution SAM High resolution SAM   Fast TPT Fast TPT  •  High resolution IR imaging  High resolution IR imaging  for units with known  for units with known  •  Non-destructive; good for multiple  Non-destructive; good for multiple   failure mechanism  failure mechanism failures in one unit  failures in one unit LIT define a failing area (AOI)  LIT define a failing area (AOI)  Package-without-die   FLI    in top die  in top die Tracecracl  -bare substrate   -FLIS  failed  \*golden  MLI  substrate  SI  Failingpin  FLI   (schematic)  TDR spectra from a failed unit, a golden unit, a bare SIP  TDR spectra from a failed unit, a golden unit, a bare SIP  Trace cracl  substrate, and a SIP package without FPGA die, showing  substrate, and a SIP package without FPGA die, showing  the open failure is close to the FLI solder joint in the  the open failure is close to the FLI solder joint in the   3D view, (b) virtual cross-sectional view, and (c)  3D view, (b) virtual cross-sectional view, and (c)  FPGA package of a SIP package  FPGA package of a SIP package   virtual planar view of the 3D X-ray CT showing  virtual planar view of the 3D X-ray CT showing   CSAM image of the AOI showing three  CSAM image of the AOI showing three  trace crack in a package  trace crack in a package   "white spots" (Si layer delam)  “white spots” (Si layer delam) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/459f9d42-2d51-43fd-8426-3834b0bda9f3/459f9d42-2d51-43fd-8426-3834b0bda9f3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=97700de3077f8556ea6ce729e059d817df6cf89f)
## Quality, Reliability, and FA challenges  

## FA workflow: Physical Failure Analysis (PFA)-Sample Preparation 

PFA --1) Disclosing the details of defects for root cause investigation 2) Utilizing techniques of sample preparation, defect imaging, and material analysis.

•  Mechanical Polishing  (cross section or planar grinding; low cost; faster TPT; operator dependent)   •  Laser ablation  (relatively fast TPT; low spatial resolution; laser induced thermal damage)    •  FIB  (Ga)  and Plasma-FIB  (Xe)

•

Broad-beam Ion milling  (low cost)

![Low Cost  Low CostShortTPTArtifactFree ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ff201cc1-79a7-4669-b7d7-c30d14b4b322/ff201cc1-79a7-4669-b7d7-c30d14b4b322.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=4fe176546273c0cf5302d8347303a672dd311560)
![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/038d48d7-2988-40c9-9c01-3f6126fb3e57/038d48d7-2988-40c9-9c01-3f6126fb3e57.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=1fed42f9c063cf89831e990987b14c3a60ba02ea)
Mechanical polishing

![FIB  Plasma FIB   lonmillingcrosssection  100  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1de1fc02-18a9-415f-b21f-c35cefa5cefc/1de1fc02-18a9-415f-b21f-c35cefa5cefc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=361010163a62369bbbc7bfc459ed30bbf032ec70)
(a). SEM image of Si layer ILD delamination by FIB cross section.  (b) and (c). SEM images of TSVs by plasma FIB and Ion milling  cross section, respectively

## Quality, Reliability, and FA challenges  

## FA workflow:  PFA-Defect Imaging 

Reveal subtle details of the defects for root cause understanding

•  Optical and IR microscopy •  Scanning Electron Microscopy  (SEM)

![R09Z6296  EAG3.0kV4.2mmX20.0k   2.00um  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6b20601f-af0f-472c-9941-6b4ddb9ee5df/6b20601f-af0f-472c-9941-6b4ddb9ee5df.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=e3e801c799ee495c643d1ecd4d02984971e1e7c8)
SEM cross-sectional image of bump-less Cu-Cu bonded structure

•

Transmission electron  microscopy (TEM)

![void  50nmm  imterfac  200mm  TEMimage of the Cu-Cu bonded interface  TEM image of the Cu-Cu bonded interface  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/06e4987d-1cfc-40ec-ab8e-010eb40cc482/06e4987d-1cfc-40ec-ab8e-010eb40cc482.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=f69ec3a477dcc80d2eec17974e5d7ce69ef7d6f6)
## Quality, Reliability, and FA challenges  

## FA workflow: PFA- Material Analysis 

Crucial for failure mechanism hypothesis, validation, and solution path identification

![EDX  EDX  TOF-SIMS TOF-SIMS  IMCs  Fulnfai  c-axisandeflow  The SEM image and the corresponding EBSD  The SEM image and the corresponding  EBSD  mapping of a failed solder interconnect after EM reliability  mapping of a failed solder interconnect after EM reliability  tests with fast Ni dissolution when the c-axis of the single  tests with fast Ni dissolution when the c-axis of the single   Sn grain of the bulk Solder is in-line with   Sn grain of the bulk Solder is in-line with   the electron flow direction,  the electron flow direction,  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f6b5c362-9eb8-4746-b61f-21e53a177b0e/f6b5c362-9eb8-4746-b61f-21e53a177b0e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=d2668494dd6fca9d9440792df1f12746261be04f)
![110°Cfor240F   samplepostuHAST_130°C   AFM-IR  AFM-IR O-PTIR O-PTIR  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7d8e8701-eb4a-4399-9bf8-5ebcb154f14b/7d8e8701-eb4a-4399-9bf8-5ebcb154f14b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=223a4c6a8bc9a1f697f8e39632d74a4e8fc69537)
www.microscopy-today.com • 2020 May, P29

•  Energy-dispersive X-ray spectroscopy (EDX)  (Elemental information)   •  Electron Backscatter Diffraction (EBSD)  (crystallographic orientation)

•  X-ray Photoelectron spectroscopy (XPS) &Time-of-Flight Secondary Ion Mass Spectrometry (TOFSIMS),  (surface or interface ppm level contamination; chemical state)   •  Fourier Transform Infrared spectroscopy (FTIR), Atomic Force Microscopy based Infrared  spectroscopy (AFM-IR), and Optical Photothermal Infrared Micro spectroscopy (O-PTIR)  (organic  material identification, sub-micron, liquid, etc.)

## Quality, Reliability, and FA challenges  

Automation and Artificial Intelligence (AI) applications in Failure Analysis  Future Development Trends

![Traditional Programming  Artificial Intelligence  Input  Computation   Results  Program  Machine Learning  Machine Learning  Deep   Input  Computation   Program  Learning   Desired  result  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a5303847-70b0-41c3-b29c-15419cc1f21f/a5303847-70b0-41c3-b29c-15419cc1f21f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=7b30a4bc49a0973e8bfde28e1438209746032c5e)
M. Kögel et. al, ISTFA 2021

![ Machine Learning   • Input   [Output  Classification  Extraction  Deep Learning   • Output  Input  Feature Extraction  Classiticatior  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/12e5614c-48ca-437e-a543-13e04abb1a88/12e5614c-48ca-437e-a543-13e04abb1a88.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=ae70fcdc07eab20eedb6afde47df156ae65fc707)
Combination of Automation  and AI in imaging and Fault  isolation. Failure mode identification  and prediction  (Pattern  recognition; Classifying FA report)

![Missinghole  Mousebite  Open cireuit   Figure2.S   lewiththeR  ort4as  Failure mode identification  Failure mode identification   Failure Analysis report  Failure Analysis report  Defect detection and  Defect detection and   Noise reduction in  Noise reduction in   by clustering and pattern  by clustering and pattern   Classification and Failure  Classification and Failure  classification  classification  SEM/TEM/SAM images  SEM/TEM/SAM images  recognition  recognition  mode prediction  mode prediction ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4ccb1037-e20b-4f73-b698-9f73ade98028/4ccb1037-e20b-4f73-b698-9f73ade98028.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=7c1c1ddd1e6b598edb6e469736d21e04ea40f206)
## Quality, Reliability, and FA challenges  Future Development Trends 

Fast, High resolution, and Non-destructive Fault isolation and  imaging techniques

MFI

![Wafer-to-Waferhybridbonding   SAM imaging  SAM imaging SAMofbondedwafers   GHz-SAMofbondedwafers  Silicon  @175MHz   @1GHz  900nm  2700nm  Silicon  DieA  SingleCupads  Single Cupads  inarraysarenot   BUMPI  arevisible   se100n  visible  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/06279b86-ae04-4258-99b5-15af5718cfa3/06279b86-ae04-4258-99b5-15af5718cfa3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=6f0aa4aadee019593a05a87e0ad972bc294de128)
De Wolf et. al, ISTFA 2018

LIT

T. Gandhi, Microelectronics Failure Analysis Desk

Reference 7th edition, ASM International, 2019

## Quality, Reliability, and FA challenges  

## Future Development Trends 

Sensitive Material Analysis tools for sub-micron resolution with minimal  or no sample preparation needs

![OPTIRanalysislocation  RightSide  6  substrate  2sum  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fa61513a-8361-468d-b7fb-c383be5f19db/fa61513a-8361-468d-b7fb-c383be5f19db.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=07c9aa2a9df0d208f97499540fdf8620f292a3b7)
O-PTIR analysis on sub-micron Foreign  Materials

![DERECO  O-PTIR  O-PTIRXSeCRIGHT  Directly analyzed  Probablecomponent1:  acrylicresins  mixture  Probable component 2:  resinacrylicemulsion  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9068bd60-494d-428c-8e5c-b8ef78f3cc66/9068bd60-494d-428c-8e5c-b8ef78f3cc66.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=540711383d55d66a8a676c5d798ca3108a3b1f01)
Lau, 2023, IPFA, Paper 116; 10.1109/IPFA58228.2023.10249138

## Quality, Reliability, and FA challenges  Future Development Trends 

![Signal Trace-Cracking,  overetch  μ-bumps-misalignment  TSV-delamination  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5d0be732-537c-4fc1-909a-5c42475c8265/5d0be732-537c-4fc1-909a-5c42475c8265.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=7d3d9799a3b7b6f2997fdefccd1e2b9785ab3762)
![Startof  topitrace  Reflection  fromC4  Measuredreference-decb  Model (reference)-deco  1SG   200  B   Time (ps)  Openfault   Reflection  in top trace   fromC4  Measured reference-decor  Model (reference)-deconv  Measuredopen-deconv  Model (open)-deconv  125   150   125   2D0   225   250   5  Time (ps)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f9455a06-b272-420d-b061-7d5dd28534d5/f9455a06-b272-420d-b061-7d5dd28534d5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215806%3B1743219406&q-key-time=1743215806%3B1743219406&q-header-list=host&q-url-param-list=&q-signature=719c05c1c3628e37dbf5b92073f6065fcdcd3483)
• Modeling and Simulation  assisted FA

• Design for test and FA

Emma Kowalczuk et al. IEEE International 3D System Integration Conference, December, 2014

## Conclusion 

•  Advanced Packaging   •  Chiplet and Memory Integration   •  Quality, Reliability, and FA

ASMTECHNICALBOOKS Electronic Device Failure Analysis Technology RoadmapO

ElectronicDeviceFailureAnalysisSociety

