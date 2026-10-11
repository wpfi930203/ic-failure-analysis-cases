---
title: "tut-4.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_209195048dbc82b96025b595eef977ca7295230462135641
file_size: 5400003
---

## Role of EDA Tools in ESD Design  and Verification 

Michael Khazhinsky Silicon Laboratories, Inc.

## Abstract 

The verification of ESD protection networks in modern integrated circuits is a difficult challenge due to  increasing design and process complexity, higher-pin counts and the overall computational difficulties in  dealing with large data sets. Most chips today are segmented into multiple power domains, where ESD  currents must necessarily be shunted from one domain to another, across multiple-layer interconnect  paths that span major portions of the chip. Furthermore, circuit blocks that are traditionally not  associated with the I/O ring and which may be far from the I/O circuits themselves, may become  damaged as a result of the high voltages and currents produced during an ESD discharge. Relying on  manual verification alone poses a significant risk of missing hidden ESD pitfalls. Consequently,  automated ESD and latch-up rule checking is highly desired. An optimum verification flow should provide  broad and flexible design rule coverage and allow incremental verification as a design progresses to avoid  late-stage changes just before tape out. The integration of ESD checking tools into the standard design  flow allows these rules to be used directly by IC designers to identify and correct most ESD issues prior to  meeting with the ESD experts. This tutorial will outline the essential requirements of the ESD electronic  design automation (EDA) verification flow which would be aligned within the IC design community, as  discussed in the ESD Association Technical Report TR18.0-01-14 (ESD Electronic Design Automation  Checks). The tutorial will give an overview of existing ESD EDA solutions across industry, including both  commercial and in-house EDA tools and flows for automated ESD checks and will discuss directions for  future ESD EDA tool development.

## Purpose 

Give an overview of existing ESD electronic design automation (EDA)  solutions across industry

Present recent publications related to different classes of ESD verification  tools: schematics, layout, and simulation based

Discuss practical boundary conditions for the use of such tools

Outline the essential requirements of the ESD electronic design  automation (EDA) verification flow, as discussed in the ESDA Technical  Report TR18.0-01 (ESD Electronic Design Automation Checks)

Desired outcome: Make designer aware of available ESD EDA verification  approaches, flows and tools. Align with ESDA WG18 recommendations

## Outline 

Basic ESD Concepts for EDA Verification   ESD EDA Verification Methods   Design Verification Flow   Conclusions   References

## Basic ESD Concepts for EDA Verification 

EDA  (Electronic Design Automation)  – a category of software  tools for developing, designing and verifying electronic circuits.

Three Steps of ESD EDA Verification

1.  Identify ESD vulnerable devices   2.  Identify ESD protection devices and circuits. Verify  implementation of ESD protection   3.  Validate that each ESD vulnerable device is properly  protected

## Why ESD EDA Design Tools? 

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/92aff750-9e9f-4bed-9b5a-5def1fc67110/92aff750-9e9f-4bed-9b5a-5def1fc67110.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=7c44958faa7557adaf8dffebfce2f9c8e442b180)
Sisyphus rolling a rock uphill

Traditional DRC/LVS can  complete some checks, but not  all

Manual checks can be slow and  error prone

Specialized software tools have  been developed for ESD IC  design to improve efficiency

## Manual vs EDA Checks 

ESD Reviews historically manual   $\Rightarrow$  performed by ESD ‘Specialist’

•  Reviewer can filter ‘false’ violations on-the-fly   •  Reviewer can consider all solutions (even undocumented ones)   •  Reviewer can provide list of specific tasks– prioritized with options

## Negatives: 

•  Limited resource: difficult to scale   •  Time-consuming process, with limited reliance on automation   •  Risk of ‘missed’ violations   •  Generally limited to single top-level review of schematic and layout   •  Occurs late in design flow (completion of schematic/layout)    Conflict: Reviewer requesting changes after Design is ‘complete’   •  Often viewed as an ‘art’ rather than a ‘science’

Manual review negatives outweigh positives: desirous of automation – but without giving  up positives!

## ESD EDA Verification Flow Requirements 

Provide broad check coverage

ESD checks during all IC design phases

Limit the required manual checks to a minimum

Be transparent and seamlessly integrated into the adopted design flow

Be run directly by IC designers

Provide clear and informative descriptions of violations

Generate reports for final design ESD sign-off

## Basic ESD Concepts 

ESD Protection Requirements:

Robustness Transparency Effectiveness

![I ESD  ESD Thermal (2nd)  Thermal (2 nd )  Breakdown Region Breakdown Region  (Vt2,It2)  (V t2 ,I t2 ) IC   IC  Operating  Operating   ESD  ESD   Breakdown  Breakdown  Area Area   Design  Design   Area Area  Windo Windo  V H  w V t1 Nominal  Nominal   BV Bvox  ox  V Vprot  PROT Voltage Voltage  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c5402bbd-54bc-4569-9299-bfb62a38b2cd/c5402bbd-54bc-4569-9299-bfb62a38b2cd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=4f3ca914a2c32463e90b75f4307f50e1ab5301d7)
## Single Devices Failure Conditions 

ESD Failures Can be Related to:     Current/power density over time (semiconductor junctions and conductors).   Electric field over time (dielectrics).

![Wunsch-Bell Model for Power  Wunsch-BellModelforPower  P(t P（tf）  f )  to failure vs. time to failure  to failure vs. time to failure  area  area  [Wunsch68, Dwyer90,  [Wunsch68, Dwyer90,  Amerasekera93]  Amerasekera93] CDM CDM  ESD  ESD  EOS EOS  HBM  HBM  In(t)  ln(t) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0e6203c5-b0e8-4cd4-ab2b-13b5e7829216/0e6203c5-b0e8-4cd4-ab2b-13b5e7829216.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=3d5be786478cd62429326971af2b067a56050638)
![6 Time-to-breakdown (s) C   10  Temp.: 25°C  Temp.: 25°C  Physical  Physical 10 4  Norm. area:1.2um2  Norm. area:1.2 m 2  Tox: (nm)  Tox: (nm) 2 10  6.85  6.85 0 10  ▼5.2  5.2 10 -2  2.65  2.65 -4  ２.２  2.2 10 10  10 -6  HBM HBN   1.97  1.97 1.5  1.5 10 10  -8 -8  regime  regime  1-1  1.1 -10 10  10 10  2  3  45678910  4 5 6 7 8910  20  20 Voltage (V) Voltage (V)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6c7ca5b5-e4bc-45c3-9d46-8e31adf1f3db/6c7ca5b5-e4bc-45c3-9d46-8e31adf1f3db.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=7a22a0effdf7368448bfed90ceaa9aeec40ed6ee)
Voltage acceleration of NFET stressed in inversion for  different oxide thicknesses [Fong87, Wu00, Ille07].

## Single Devices Failure Conditions 

1

2

3

ESD Failures: ESD Failures:

Source/Drain junction failures 1-3, 1-4  Source/Drain junction failures 1-3, 1-4, 3-4 → P   → V(I  )

crit

crit

![ Oxide failures 1-2, 2-3, 2-4 → Ecrit → V  Oxide failures 1-2, 2-3, n+  n+ 2 p-sub  p-sub  oxide  oxide 4  1  W  3 4 Ecrit   2 1  E crit  P Pcrit  crit  3  2 Pcrit  crit   crit  Vcrit)  V(I  ) 4  1  V  crit  3 Ccrit  4 11 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/11a621a0-9959-4f60-b7bf-2db4576c1f7b/11a621a0-9959-4f60-b7bf-2db4576c1f7b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=141db08bcd22c851d0e633d7020de3de5405c3a1)
## Single Devices Failure Conditions 

![Passives Passives   Diodes  Diodes Resistors:  Resistors:  [VAcC_Forward _crin=VAc(IAC_Fonward _ori t)  VABcrit = VBA_crit = VAB(IAB_critst) =VBA(IBA_critst).  ). Vca_Revers_crit =VCca(ICA_ Reverse_ ri t)  Capacitors: Capacitors:  VAB_crit =VBA_crit =VAB_crit(IABst) = VBA_crit(IBA>t).  Anode  Anode A  A  A  A R  C  L  Z  D M  B 3   3  B  B  3  B  Cathode  Cathode ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b51789ae-80e8-4029-ace2-faed05a1fb00/b51789ae-80e8-4029-ace2-faed05a1fb00.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=63f025d622275d3fab6da7a0c449e247bcb49e5c)
## Single Devices Failure Conditions 

![Bipolars  Bipolars  MOs Transistors  MOS Transistors [VDs_ern = VDs(Ips_erinst)  V  V  ( I  , t )  [VBG_ert = VBG_er(IBGst)  VCE_crit =Vc(IcE_crist)   DS _ crit  DS  DS _ crit VEc_erit =VEc(IEc_critst)   VsD_erit = Vsp(IsD_crtst)  V SD _ crit  V SD ( I SD _ crit , t )  VGB_cr = VGB_ru(IGnst)  VBs_crit =VBs(IBs_critst)  V BS _ crit  V BS ( I BS _ crit , t )  VGD-_crt = VGD_er(IGD,t)  VCB_crit = VcB(IcB_critst)               VBC crit =VBc(IBC_crist)   VBD_erit =VBD(IBD_eritst)  V V VSsB_crit = VsB(IsB_critst)  SB _ crit  V V SB ( ( I I SB _ crit , t , ) t )  VGs_crit = VGs_corit(IGs st)  VDG crit = VDG crit(IpG,t)    BD _ crit  BD  BD _ crit VBE_ru =VBE(IBE_eriust)   V VDB_crit = VDB(IDB_crit st)  DB _ crit  V DB ( I DB _ crit , t )  VsG_crit = VsG _crit(I sG,t)  VEB_crit = VEB(IEB_critst)  Collector  Collector  Drain  Drain Base  Base  Gate β  Gate  凶Body  Body Emitter  Emitter  1③  13  Source  Source ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/43c9b7aa-d09a-4873-9439-62be335062ab/43c9b7aa-d09a-4873-9439-62be335062ab.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=bd4771fcc07f1962e86e482760dc912cbe8eddea)
![Generic Topology Failure Conditions Generic Topology Failure Conditions  Serial Connections  Serial Connections  Parallel Connections  Parallel Connections A A Component 1  Component1  {VAC =VAB(IABst)+VBc(IBCt)   Component 1  Component1  Component2  Component2 区B  B  Vca = VBa(IBA,t) + VcB(IcB,t)  Component2  Component2  M  E  B A  VAB = VAB _COMP _1(I AB_COMP_1,t) //  C nU  D冈T  D  I/VAB_COMP _2(IAB_COMP_2,t)  // V AB _ COMP _ 2 ( I AB _ COMP _ 2 , t ) D G网H  G Vsa = Vsg (Isg,t)+   B Vsg = Vsg _Mos (IsG _Mos ,t) //  B G  7B  B  + Vga (Iga st).   C  I/ Vsg _c(Isg _c>t).  I网cSO  S  1A  14  S ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0de1968e-b58a-4e53-8762-8d74a56fad78/0de1968e-b58a-4e53-8762-8d74a56fad78.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=6387269ecba713d16d20a4290e6dac47ede0e7d3)
## Basic ESD Concepts for EDA Verification 

## ESD Protection Strategies and Failure Conditions  

1. ESD energy is shunted through ESD clamp path (protected  devices cannot shunt ESD energy).  $V_{E S D\_C L A M P S\_P A T H}\geq V_{F A I L U R E\_C I R C U I T}\,.$

2. ESD energy is shunted through the protected circuit.   $\begin{array}{r}{\left\{I_{P R O T E C T E D_{-}C I R C U I T}\geq I_{F4I L U R E_{-}C I R C U I T}\right.}\\ {\left.V_{P R O T E C T E D_{-}C I R C U I T}\geq V_{F4I L U R E_{-}C I R C U I T}\right.}\end{array}.$

3. ESD energy is shared between the ESD clamp path and  the protected circuitry.   $\begin{array}{r}{\left\{I_{P R O T E C T E D\_C I R C U I T}\geq I_{F A I L U R E\_C I R C U I T}\right.}\\ {\left.V_{E S D\_C L A M P S\_P A T H}\geq V_{F A I L U R E\_C I R C U I T}\right.}\end{array}$

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7485b788-2643-4a8c-a088-b8807a266104/7485b788-2643-4a8c-a088-b8807a266104.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=3877dd44b39dfc686d8998ea1b115bf636f268f8)
## Basic ESD Concepts for EDA Verification 

## ESD Protection Strategies and Failure Conditions  

1. ESD energy is shunted through ESD clamp path (protected  devices cannot shunt ESD energy).

$$V_{E S D\_C L4M P S\_P4T H}\;\geq V_{F4I L U R E\_C I R C U I T}\;.$$
2. ESD energy is shunted through the protected circuit.   $\begin{array}{r}{\left\{I_{P R O T E C T E D_{-}C I R C U I T}\geq I_{F4I L U R E_{-}C I R C U I T}\right.}\\ {\left.V_{P R O T E C T E D_{-}C I R C U I T}\geq V_{F4I L U R E_{-}C I R C U I T}\right.}\end{array}.$

3. ESD energy is shared between the ESD clamp path and  the protected circuitry.   $\begin{array}{r}{\left\{I_{P R O T E C T E D\_C I R C U I T}\geq I_{F A I L U R E\_C I R C U I T}\right.}\\ {\left.V_{E S D\_C L A M P S\_P A T H}\geq V_{F A I L U R E\_C I R C U I T}\right.}\end{array}$

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5c686cf7-61ff-4aeb-8502-d8538d7d5d87/5c686cf7-61ff-4aeb-8502-d8538d7d5d87.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=67ee1a1ad5d51471ecaa83984d43238252908b94)
## Basic ESD Concepts for EDA Verification 

## ESD Protection Strategies and Failure Conditions  

1. ESD energy is shunted through ESD clamp path (protected  devices cannot shunt ESD energy).  $V_{E S D\_C L A M P S\_P A T H}\geq V_{F A I L U R E\_C I R C U I T}\,.$

2. ESD energy is shunted through the protected circuit.   $\begin{array}{r}{\left\{\begin{array}{l l}{I_{P R O T E C T E D\_C I R C U I T}\geq I_{F4I L U R E\_C I R C U I T}}\\ {V_{P R O T E C T E D\_C I R C U I T}\geq V_{F4I L U R E\_C I R C U I T}.}\end{array}\right.}\end{array}$

3. ESD energy is shared between the ESD clamp path and  the protected circuitry.   $\begin{array}{r}{\left\{I_{P R O T E C T E D\_C I R C U I T}\geq I_{F A I L U R E\_C I R C U I T}\right.}\\ {\left.V_{E S D\_C L A M P S\_P A T H}\geq V_{F A I L U R E\_C I R C U I T}\right.}\end{array}$

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7cfbc438-a490-4b11-b1e5-0be5ed09fa2c/7cfbc438-a490-4b11-b1e5-0be5ed09fa2c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=f95e9179d4bc72ced282a502bab8f244fea5369a)
## Basic ESD Concepts for EDA Verification 

## ESD Protection Strategies and Failure Conditions  

1. ESD energy is shunted through ESD clamp path (protected  devices cannot shunt ESD energy).  $V_{E S D\_C L A M P S\_P A T H}\geq V_{F A I L U R E\_C I R C U I T}\,.$

2. ESD energy is shunted through the protected circuit.   $\begin{array}{r}{\left\{I_{P R O T E C T E D_{-}C I R C U I T}\geq I_{F4I L U R E_{-}C I R C U I T}\right.}\\ {\left.V_{P R O T E C T E D_{-}C I R C U I T}\geq V_{F4I L U R E_{-}C I R C U I T}\right.}\end{array}.$

3. ESD energy is shared between the ESD clamp path and  the protected circuitry.   $\begin{array}{r}{\left\{{I_{P R O T E C T E D\_C I R C U I T}}\geq I_{_{F4I L U R E\_C I R C U I T}}\right.}\\ {\left.V_{E S D\_C L4M P S\_P4T H}\geq V_{F4I L U R E\_C I R C U I T}\right.}\end{array}.$

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/78e3a202-42a5-4f12-ae2b-c04a8f46ce47/78e3a202-42a5-4f12-ae2b-c04a8f46ce47.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=7047aa298c2e42d34bc48c213f313169e628ac99)
## Outline 

Basic ESD Concepts for EDA Verification   ESD EDA Verification Methods   Design Verification Flow   Conclusions   References

ESD EDA Verification Methods

![SPICE  SPICE   Static Topological Checks  Static Topological Checks   Compact  compact   Macro Checks  Macro Checks Models  Models Context Aware Layout Checks  Context Aware Layout Checks  Package  Package  TCAD TCAD  (Parasitic Device Checks)  (Parasitic Device Checks)    Checks  Checks Current Density  Current Density   System  System  (CD) Checks  (CD) Checks   Checks  Checks Point-to-Point  Point-to-Point  (P2P)  (P2P)  Resistance  Resistance  Checks  Checks  Schematic-Based  Schematic-Based  Layout-Based  Layout-Based  Simulation-Based  Simulation-Based  Other  Other ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c70155f3-7039-49e1-8031-aa9e5325d773/c70155f3-7039-49e1-8031-aa9e5325d773.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=7e82ff94d94a5b1437870c0d8c9b12bafbc345d9)
## Schematic-Based Methods 

## Definition: 

Schematic-based methods include all verifications that can be implemented  with commercial or custom EDA tools able to analyze circuit device and  connectivity topologies described in a netlist.

Netlists can originate from schematic views or can be derived from layout  extraction.

## Objectives : 

• Identify/verify devices to be protected from ESD   • Verify ESD protection network implementation

## Typical Schematic-Based Checks 

## Verification of Devices to be Protected from ESD: 

1. Report unprotected devices connected between I/O and supply pads     2. Report unprotected devices connected between supply pads   3. Report unprotected devices connected between different I/O pads   4. Report unprotected devices at Power Domain Signal Crossings (PDSC)    5. Report all transistors with body and source terminals connected to different supply nets   6. Report devices with unprotected gates connected to supplies / large nets

Devices to be  protected  from ESD

![igh ratio  6  VDD VDD1  1  5  VDD VDD2  2 1 2 I/o1  I/O 1  3  I02  I/O 2 4 1 VSS1  VSS  VSS2  VSS 6  1  5  2 22  22 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7af90814-dcd1-4548-959a-70f2a3016e92/7af90814-dcd1-4548-959a-70f2a3016e92.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=610b4557f058b0df61c05f86fb65dda24993ea0f)
## Typical Schematic-Based Checks 

## Verification of ESD Protection Network 

1. Verify presence and size of ESD protection device (diode or local clamp) between I/O and supply    pads.   2. Verify presence and size of ESD protection device between supply pads.   3. Verify presence and size of ESD protection device between different I/O pads.   4. Verify presence and size of ESD protection device between different power domains.

ESD Protection  Devices

![VDD,  VDD  VDD2  VDD 1  2 1 2 I/0 1  I/O 1  3  I02  I/O 2 4 1 VSS1  VSS 1  VSS2  VSS 2 23  23 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/22601ac3-d920-4bc5-90d8-f5d1fe8efae9/22601ac3-d920-4bc5-90d8-f5d1fe8efae9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=032ba3a6f6877f16fc766fbf6fe3c4f2224ebc9c)
## Protected Devices Check 

Objective: Report ESD vulnerable devices.

![I R Rvdd  Vdd (V (VT2,IT2)  T2 , I T2 ) FRA  R I/O  A R RNPN  NPN dV dt +  R RBS  B  NVA  M 1  (VT1，IT1)  (V T1 , I T1 ) V VSS  VSS  R RVss  Vss  V VT  H ESD  ESD  70  No  Error  Error Check  Check   Identify  Identify  Find  Find   Yes Yes,  Pad  Pad   Connected  Connected   V Vt1 >Vpad_max  T1 >V PAD_MAX  CK  OK V Nets  Nets   Devices Devices   T1 24  24 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e3aeef36-1b30-43b5-ad5a-19f1e743c493/e3aeef36-1b30-43b5-ad5a-19f1e743c493.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=a9584ccddbbcfb832c7d61f943ccec2c2530935b)
## ESD Network Check 1 

Objectives: Report missing ESD diodes and diodes with insufficient perimeter (P).

![D A  R Rvdd   I Vdd R RAE  I/O  A R Rdiode  Diode dV dt +  R RB  B V VSS  VSS  DB  D B  R Vss  VHdiode  V HDiode ESD  ESD  70  No  70  No  Error  Error Check  Check   Da,db  D A , D B  Pa>Pa_min  P >P ESD  ESD   A  A_MIN  Yes Yes  I/O   Pb>Pb_min  P  >P  CK  OK Diodes  Diodes   B  B_MIN Nets  Nets Exist  Exist 25  25 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1956da91-6770-47c2-9f9b-c38fa1910f4f/1956da91-6770-47c2-9f9b-c38fa1910f4f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=ef7af5f35b0a3c3997903eb70c1b8e97c5758976)
## ESD Network Check 2 

Objective: Report missing ESD clamps and ESD clamps with insufficient width (W).

![D  R Rvdd  Vdd  I A R RA  A dV  R Rclamp  Clamp I/O  dt +  R RB  B D  V B  R Rvss  Vss  VHclamp  V HClamp VSS ESD  ESD  7O  No  7O  No  Error Error  Check  Check   ESD  ESD  Yes  Yes Supply  Supply   Clamp(s)  Clamp(s)   W Wclamp>Wclamp_MIN  Clamp >W Clamp_MIN  OK Nets  Nets  Exist  Exist 28  26 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5429bb69-5771-4947-8d74-56d9753d6d11/5429bb69-5771-4947-8d74-56d9753d6d11.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=0a884e3f0ce89914644ccd35ea9a8832ff0144da)
## Verification of Gates along Power Cross  Domains Paths 

![VDD1  VDD2 VDD2  ESD  ESD  1  ESD  ESD clamp  clamp  clamp  clamp GC  GO  - VSS1 SS1   VSS2 VSS2  D 1  R pus  bus  D 2  Screenshot of the results of the cross- Screenshot of the results of the cross-gnd   gnd  gnd  domain schematic checking highlighting an  domain schematic checking highlighting an  NMOS (N10) whose terminals are  NMOS (N10) whose terminals are  connected to two differentpower domains  connected to two different power domains  +V.+V  V  V  V  V    V ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/202f39ff-5c4d-4df8-8487-8a4f97b98940/202f39ff-5c4d-4df8-8487-8a4f97b98940.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=f207ad7ef4c8321c5a576e455f91327b749a3c7f)
V ESDclamp  D 1  Rbus  D 2  pMOS  _ DS _ BD  nMOS AMO.S   _ GS RS  BD  _ BD

Cross-domain level shifter:  gate at  node 1 could be overstressed during an ESD event.

![Non-ESD  Non-ESD   Large  Large  Goal: Verify Big Buffer Topologies do not Form  Goal: Verify Big Buffer Topologies do not Forn  component  component   PMOS  PMOS   Low Impedance Path during ESD  Low Impedance Path during ESD VDD  VDD competing  competing  discharge path  discharge path Design netlist, top powers and  Design netlist, top powers and  failure_  Catastrophic  Catastrophic  failure   W   Power  Power   on-chip power pins name and  on-chip power pins name and   Input  ndui  …  OUT  OUT Clamp  Clamp  ground pins names ground pins names  PAD  PAD VSS  VSS Get (count) all PMOS and  Get (count) all PMOS and  ESD network  ESD network   NMOS (@ NetA)  NMOS ( @ NetA)  Instructions set designed  designed  Single NMOS finger failure  Single NMOS finger failure   discharge path  discharge path Calculate total PMOS width.  Calculate total PMOS width.  during HBM stress  during HBM stress  Find NMOS with minimum  Find NMOS with minimum  width. Find Ratio  width. Find Ratio OK  Is Ratio < Threshold Is Ratio< Threshold  Yes Yes   1NO  No Report violation with power and  Report violation with power and  ground net names  ground net names  Output  tndino  28  28  [Duvvury10, Trivedi13]  [Duvvury10, Trivedi13]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5e834599-5c74-46a8-a2a9-da9f20011cc8/5e834599-5c74-46a8-a2a9-da9f20011cc8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=21ce378a49793d3eaf1b637f1d83a5b0894c17a0)
Verification of Big Buffers

## Thin Oxide Gates Connected to Large Metal  Plates 

Most CDM charge resides on large metal plates (VSS, VDD).

Devices connected to VSS/VDD are on direct CDM discharge path and will  see large ESD voltage spikes.

a. Gates of thin oxide devices  must not be directly connected  to ground nets.   b. Gates of thin oxide devices  must not be directly connected  to power nets.

![VDD1  VDD1 I/O VDD VDD  ESD  TC ESD  core  core  IC VSS1  VSS1  circuit  circuit global VSs  global VSS Exposed  Exposed  Negative CDM event Negative CDM event   thin  thin  oxides Oxides  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5ce8e304-b251-4371-9657-34164c7ba053/5ce8e304-b251-4371-9657-34164c7ba053.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=7bb55a63677eda83487c551b02902700f3d9746d)
• Checks and reports all thin  oxide FETs with gates  connected to power/ground  nets.

## Netlist Inspection Based Methods 

![HIGHHIGH HIGHHIGH  PROPERTIES PROPERTIES WINDOWMINDOW V HIGHVHIGH  xVIOIO V IOmaxV1omax  yVV IOminV 1Omin  zVV LOWVLOW  D 0VLOWLOV LOWLOv  HBM min HBMmin ?/CDM min/CDMmin VCCBigBig IO CONTROL CONTROLCONTROL ClampCiamp CONTROLE CONTROLGND2GND2 GND1GND: 30](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/263fef2f-5571-4326-9908-2d260d747116/263fef2f-5571-4326-9908-2d260d747116.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=67cdcebf87f34d262dd2702cc29f7b81d32ef549)
## Initialization Method – Controllers 

Controller is placed in the  schematic with its terminals  connected to nets under  verification Each controller checks a  specific ESD configuration Operating voltage ratings and  ESD target is included as  controller properties

[Gevinti15]

![Large ESD  .arge ESD   Layout   Schematic  Network  Network  Topological  Verification /erification   netlist extraction  Extracted netlist   graph networks ton  Omission  omission  Topology-awareESD   Directed graph  of a core  of a core  networkrecognition  power  power   Graph   Graph  clamp  clamp   XML database   exploration   verification  between  between   EndingnodeID  tvo  two  bumps in  umpsin  row#48  an analog  n analog  domain domain  net #48 to net #47  (vddcore_N31 tovddcore S12)   B2B  GreenAt least one path exists.  Red No path found.   HVclamp  missing  WhiteStarting node =Ending node  GreyNo search done yet.  LVClamp  LVClamp  ③1  31  GNDANAVDD_ANA  Viale16  [Viale16] ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bc8a0114-2fda-4049-a0e8-a573ff98c67a/bc8a0114-2fda-4049-a0e8-a573ff98c67a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=75c35eac552b1cf7083f34cd84698c5d1a2dd53a)
Netlist Inspection Based Methods

## Netlist Reduction 

Identify ESD vulnerable elements and ESD discharge paths Eliminate circuit elements irrelevant for the ESD evaluation Apply stricter ESD rules to elements along critical ESD paths

![iavout   Raw  Netlists   Netlist Reduction  Reduced  (GB's)  Netlists  (MB'S)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/abbd4b32-4387-4225-a32c-156c2d5331af/abbd4b32-4387-4225-a32c-156c2d5331af.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=e0737763f6986045d5e32fb0d4e3d123fb100845)
## Input Data for ESD EDA Topological Analysis 

![INPUT INFORMATION INPUTINFORMATION  PINS  PINS PINS AMRs PINS AMRs   PINS BONDING  PINS BONDING  FUNCTIONALITIES FUNCTIONALITIES  CONDITIONS  CONDITIONS  (shorted, noConn, ..) (shorted, noConn,  ESD PROTECTION  ESD PROTECTION  NETLIST  NETLIST STRATEGY  STRATEGY  (common rail,  (common rail   VICTIMS/ VICTIMS/  ESD ROBUSTNESS  ESDROBUSTNESS  local protection,  local protection,   PROTECTIONS  PROTECTIONS  REQUIREMENT  REQUIREMENT  self-protection  self-protection)  V Vdrop VALUES   VALUES drop (HBM/CDM/SYSTEM) (HBM/CDM/SYSTEM)  STATIC  STATIC  TOPOLOGICAL  TOPOLOGICAL  CHECKER CHECKER  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a2057b48-f0d4-459a-9717-353f9143afc4/a2057b48-f0d4-459a-9717-353f9143afc4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=202b7ae405789f7ad55fd4f000eb5f039fd5a65e)
## Technology-Independent & TechnologyDependent Information 

![TECHNOLOGY-DEPENDENT  TECHNOLOGY-DEPENDENT  TECHNOLOGY-INDEPENDENT  TECHNOLOGY-INDEPENDENT   FILES  FILES INPUTINFORMATION  INPUT INFORMATION  FILES FILES  REDUCTION FILE REDUCTION FILE  PINS  PINS PINS AMRs  PINS AMRs  FUNCTIONALITIES  FUNCTIONALITIES  PINS BONDING  PINS BONDING   RULES ON ESD  RULES ON ESD  CONDITIONS  CONDITIONS  (shorted, noConn, :  (shorted, noConn, ..)  PROTECTION PATHS PROTECTION PATHS   CONFIGURATION FILE CONFIGURATION FILE  ESD PROTECTION  ESD PROTECTION   NETLIST  NETLIST STRATEGY  STRATEGY  (common rail,  (common rail,   VICTIMS/  VICTIMS/ ESD ROBUSTNESS  ESD ROBUSTNESS   PATTERN FILE  PATTERN FILE local protection,  local protection,   PROTECTIONS  PROTECTIONS   RULES ON WEAK  RULES ON WEAK  REQUIREMENT  REQUIREMENT  self-protection)  self-protection)  (HBM/CDM/SYSTEM)  (HBM/CDM/SYSTEM)   Vdrop VALUES  V drop  VALUES  TOPOLOGIES TOPOLOGIES  HEADER FILE HEADER FILE  STATIC  STATIC  TOPOLOGICAL  TOPOLOGICAL  CHECKER  CHECKER ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7e5b1236-2aab-4171-81a5-3627b00df72a/7e5b1236-2aab-4171-81a5-3627b00df72a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=1089c07f5313df9d90d599fe7b33aed4e30ebf1e)
## Layout-Based Methods 

## Definition: 

Layout-based methods include all verifications that can be  implemented with commercial or custom EDA tools able to  analyze integrated circuit layout and device shapes/geometry.

Layout-based methods would involve analyzing both back-end and front-end layers.

## Layout-Based Methods 

Logic Driven Layout (LDL)

Geometric check with information of connectivity, net-type,  voltage, etc.   Current Density (CD) Calculate current through routing layers Check each polygon’s CD against limit   Point to Point Resistance (P2P) Calculate total routing resistance Report R contributed by each polygon

## Layout-Based Methods: Use Cases 

Check if Anti-Parallel Diodes exist between separate ground domains     Check if parasitic bipolar exists between IO-to-power or power-to-power     Routing optimization for driver or clamp FET     Assess Electromigration risk of ESD path     Assess oxide overstress during CDM by ground resistance btw TX/RX,   APD, pad

## Potential Expansions: 

• Package and system level checks   • ESD device model in CD/P2P   • LDL/CD/P2P on LEF/DEF database   • Standard format for foundry & 3 rd -party IP

## Current Density Checks 

## Report insufficient (CD) metal lines and interconnects for ESD discharge paths 

1.  from I/O pad to Power through diodes or diode string;   2.  from I/O pads to Ground through diodes or diode string;   3.  from I/O pad to Ground through transistors;   4.  from Power pads to Ground pads through transistors;   5.  from Power pads to Ground pads through diodes;   6.  from Ground pads to Ground pads through diodes.

![VDD  VDD ESD  ESD  4  5 1  P-Diode  P-Diode Active  Active I/0  I/O  Rail  Rail  Return  Return Diode  Diode Clamp  Clamp Snapback  Snapback 2  ESD  ESD  FET  FET N-Diode  N-Diode  3 VSS1  VSS 1  VSS2  VSS 2 6 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5b7d6f1a-3f65-44db-9c5b-460db9ed95bc/5b7d6f1a-3f65-44db-9c5b-460db9ed95bc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=46b4c4f9a4585d37364733bf55a72e721adae7e5)
## P2P Resistance Checks 

## Report P2P resistance of metal lines and interconnects for ESD discharge paths 

1.  from I/O pad to Power through diodes or string;   2.  from I/O pads to Ground through diodes or string;   3.  from I/O pad to Ground through transistors;   4.  from Power pads to Ground pads through clamp transistors;   5.  from I/O diodes to clamp transistors through Power buses;   6.  from I/O diodes to clamp transistors through Ground buses;   7.  from Power pads to clamp transistors;   8.  from Ground pads to clamp transistors;   9.  from Power pads to Ground through diodes or string;   10.  from Ground pads to other Ground pads through diodes or     string.  string.

![7 VDD  VDD 5 4  9 ESDI  ESD 1  P-Diode  P-Diode Active  Active I/O  Rail  Rail  Return  Return Diode  Diode Clamp  Clamp Snapback  Snapback ESD  ESD 2  N-Diode  N-Diode  3  FET  FET VsS1  VSS 1  6  VSS2  VSS 2 10 10  8 39 39  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6bcc5bc0-80ae-4572-9b56-8086bebc9d66/6bcc5bc0-80ae-4572-9b56-8086bebc9d66.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=55200c4899b4229759b78f1d7a3a5f294d82230f)
## Basic CD and P2P Resistance Checks 

Objectives: Identify current density (J) metal and interconnect violations along ESD  path. Report non-compliant bus resistances.

![ESD  ESD  D A  R Rvdd  Vdd  No  Error  Error Check  Check   Analyze  Analyze  R FRA   Calculate  Calculate   Jm < Jm_max   J   < J  yes  Yes I/O  A  ESD   ESD   Current  Current   m  J  , J  J< Jv-MAX  J M  < J M_MAX  OK  Path  Path  FIow  Flow  M  V  V  V_MAX dV C  dt +  R RBS  B  ESD  ESD  7O  No   Error  Error D VSS  VSS  B  R Vss  Cpadk  Check   luxmraed  Extract   Caimuate  Calculate   RA≤RMAX  R A  < R A_MAX  yes  Yes lumped   OK  OK  Nets   Nets  Pad   R1, R2, R3, R4  R 1 , R 2 RS  R , R 5 3,  R 4 ,   lumped  Ra, RB  R A , R B  R B  < R B_MAX ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ec3b1382-e7e3-43a4-a75b-41ee14d2f4d5/ec3b1382-e7e3-43a4-a75b-41ee14d2f4d5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=9e70f49b081d5831a9be330d1308213dcc00a63b)
## Current Density Case Study 

![CD:SL_ESD_2_201_String_Pass_PERC_cd.report.cd.rdbx  PERCResultsPERCInfoResults  Filter:ShowAllSL_ESD_2_201_String_Pass,683585Results(in2of2Checks)  Diodes  Experment/Net/Test/Layer   Results   Vertices  A（um\~2）   LCD   ERROR(%)   Experiment   FIX   1（m）  日XExperiment SL_ESD.2.200.by_path  274997   0.00000   110.833   0.000000   SL_ESD.2.201.by_path   12.0000   1330.C  由xNetpad   139157   2   0.00000   1.12776   0.000000   SL_ESD.2.201.by_path   4.93200   5.5621  xNetvio   34702   0.00000   0.301906   0.000000   SL_ESD.2.201.by_path   4.10000   1.237E  ×NetX24/5   50569   0.004900   17.2957   0.000000   SL_ESD.2.201.by_path   0.004900   0.0847  xNetX24/6   50569   0.004900   17.2957   0.000000   SL_ESD.2.201.by_path   0.004900   0.0847  日X  Experiment SL_ESD.2.201.by_path  408588   0.004900  17.2957   0.000000   SL_ESD.2.201.by_path   0.004900   0.0847  中xNetgnd   148820   0.004900  17.2957   0.000000   SL_ESD.2.201.by_path   0.004900   0.0847  中xNetpad   142134  中xNetX24/7   58776  由xNetX24/8   58858  Experiment Comment:  Rulecheck Comment:Insufficient (CD) metal lines and interconnects for EsD discharge path from I/O pads to Ground through diodes  Nets  1   X24/7  Interconnect   42  X24/8  23  -gd  Test   #4-pad  Pattern   Simulation Setup- cd_2 Source Sink Connection  Sources:  #1-PORT-padALPA:1330.0 mA  Sinks  #1-PORT-gndALPA:0.0mV  Cornections:  -esd_ndio_25(x24/x3/x0esd_ndio_25()x24/x3/x0minus dio_np connects esd_ndio_25()x24/x3/x0esd_ndio_25()x24/x3/x0plus   Uohms  22   esd ndio_25（)   X24/X3/X1  minus dio_rp connects esd_ndio_25)  X24/X3/X1esdndio25（  X24/X3/X1  Plus  rwell   0ohm  esd_ndio_25()  x24/X4/x0 esd_ndio_25()  x24/X4/x0 minus dio_np cornects esdndio_25()  X24/X4/X0  esd ndio 25（)  X24/X4/X0  Dl1us  tvell   0ohms  esdndio250  x24/X4/X1esdndio_25（)  X24/x4/x1  minus dio_np connects esd ndio_25()  X24/X4/X1  esdndio_25（）  X24/X4/X1  Dlus  tuel   0ohms  esdndio_25()x24/x5/x0esd_ndio_25()  x24/x5/x0minus dio np connectsesd ndio_250  x24/x5/x0esdndio25)  X24/X5/x0   Tuell   0ohms  #6-esd_ndio_25)x24/x5/X1 esd ndio_25() x24/x5/X1 minus dio_np connects esd_ndio_250x24/x5/x1 esdndio_25() x24/x5/x1 plus rvell  0ohms  nge [0.001009, 374.307]; Total: 408588/408588 (100.00%):  Experinent SL_ES0.2.201.by  IOPad  CD  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fd348ba7-9fd7-45e4-8d7c-5bd27ea4caee/fd348ba7-9fd7-45e4-8d7c-5bd27ea4caee.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=eb64757ed45928972bddfe7bb1fd23dc2f77aad2)
Useful information from CD  check result

•  Current (mA) and  Current Density (CD) on  each conductor layer  shape   •  Limit & Error   $(\%)$   of CD  on each conductor layer  shape   •  Resistance (mOhm) of  each conductor layer  shape   •  Highlight & Color-Map to  visualize results such as  CD, Error, etc.   •  Histogram

## Layout Based Methods 

## Wire/Via Current Density Check 

Objective: Identify weak ESD  weak ESD  paths among all  mong all  possible paths  e paths  based on full-chip  on full-chip  extraction analysis  on analysis

![nt Density Check  pad  R1   R2   IV curve is used to  IV curve is used to  model all the  model all the  zap   C   cc   clamps and diode  clamps and diodes Voltage  Ron  Holding   Triggering  pad   (Vh,Ih)  Turnon   (Vt1,It1)  Roff  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/09993e95-ca8d-439a-a0ca-a9dc28394be0/09993e95-ca8d-439a-a0ca-a9dc28394be0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=225343ab8ba6e22f80d3e8419b67d09ef8538914)
Current Density Violation Maps

Current density  violations   Routing congestion,  stion,  narrow wires   Device voltage  overstress

## Layout Based Methods 

Point-to-Point (P2P) Resistance Check

Objective: Identify weak ESD paths among all  possible paths based on full-chip  extraction analysis

Signal-to-Power Resistance     Signal-to-Ground Resistance     Power Bus (diode to clamp)   Resistance     Signal Net Resistance (bump to   diode/clamp & diode/clamp to bump)     PG Resistance (bump to bump)

![C  round  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4d30f674-2034-4215-a4fc-611a77838776/4d30f674-2034-4215-a4fc-611a77838776.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=4386bf18193b078eb0cd43660da4d27530a87065)
baonocaton

![RCClamp  CDMdiode(secondarydiode)  HBMn/p-diodes  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/46c771dd-e58e-49a3-a616-4462746510d3/46c771dd-e58e-49a3-a616-4462746510d3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=5b091d022af4f11903fa9e031227e85be8b3864f)
![4.265   SO  SS  Signal-to-Ground ResistanceCheck(S2G_R_check)  (e.g.VREFCApad→cphy_IR_eESDPdiode_40_0→VDDIO  >cphy_IR_eESDRCClamp_2_0_3→VSS)  >RODT/VREFDQ/VREFCA havehighestresistanceESDpath.  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/652c7f70-c608-4292-aa7a-25232bbde8db/652c7f70-c608-4292-aa7a-25232bbde8db.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=590aa29f6b57e39186b94b799e02937bdcaea99a)
## Layout Based Methods 

![CORE_VDD_ne.1AVSS_885_510  9  Zoomin  LCOREVDS  FO  Show Top Contacts  Fil Top Contacts   Hotspot  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/497f4275-12e3-420e-91c1-1ec7c04d48fc/497f4275-12e3-420e-91c1-1ec7c04d48fc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=dd71ad5d907324cbf1ba3e83245c5d1c5c7430b5)
Wire/Via Current Density Check

Visualization of the current crowding issues  that were observed in the M9 layer

![ESD stress event:  ESD stress event: 1.4 14   Grounded pad:CORE_VDD power group  Grounded pad:CORE_VDD power group  Nets:  Nets: Stressed pad: 1_AVSS  Stressed pad: 1_AVSS Criticality (a.u.) 1.2 1.2   sign:  Sign:   negative  negative  ■1_AVSS  1_AVSS ■CORE_VDD  CORE_VDD 1 ■CORE_VSS  CORE_VSS 0.8 0.6 0.4 Automatedidentificatior  Automated identification of critical nets & layers  of critical nets & layers 0.2 0 M1 M2 M3 M4 M5 M6 M7 M8 M9 M10 AP n_odCont p_odCont VIA1 VIA2 VIA3 VIA4 VIA5 VIA6 VIA7 VIA8 VIA9 RV metals  metals  vias  vias Layer  Layer ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8f13d069-2d05-452e-bdf2-84cfd0d88fed/8f13d069-2d05-452e-bdf2-84cfd0d88fed.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=5867b38d6cbe3651675c86b8cf0585d703036e8a)
Detailed ESD event  analysis highlighting the  most critical layers, in  terms of resistance or  current density violation

## Verification of Bus Resistance between  Pad and ESD Cell/Device in an I/O Bank 

Tool extracts bus  resistances to  instances of power  clamps     Bus resistance compared  against specified  maximum allowed bus  resistance     Example showing  correlation between low  CDM results and I/Os  that had excessive power  bus resistance

![I/O Power Pin  I/O Power Pin VDDxwire  VDDx wire  ESD RES  ESD_RES  ESD  ESD V<ESD_LIMIT? V<ESDLIMIT?   resistance  resistance  power  power clamp  clamp V  I = ESD_CURRENT = ESD CURRENT   ±  ESD_SRC  ESD_SRC GND  GND GND  GND Last Metal VDDx bus  Last Metal VDDx bus Thin Gate I/O CDM Fails vs. Power Route Voltage Drop  Thin Gate I/O CDM Fails vs. Power Route Voltage Drop 1 1 = Pass, 0 = Fail  = o 'ssed  0 0               0.5            1.0             1.5            2.0            2.5           3.0 0.5   1.0   1.5   2.0   2.5   3.0  Power route voltage (ratio to breakdown voltage)  Power route voltage (ratio to breakdown voltage) 45  45 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/03a971c0-9523-4776-aea5-9092e9bb465b/03a971c0-9523-4776-aea5-9092e9bb465b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=d7cb43f14c31335deedfb9a248e76c5007d84291)
## Layout Based Methods 

Checking for Parasitic Low Impedance Paths

![1 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/08a71f02-e03f-4c14-ba34-35583c9943c3/08a71f02-e03f-4c14-ba34-35583c9943c3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=d70eab343263020efd80106c02234030bdc9a025)
Nwell-Pwell-Nwell

![2 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/688143e1-f337-42c7-844b-a5c4514f5da7/688143e1-f337-42c7-844b-a5c4514f5da7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=ae6e9be1bc96145441101cc260167e0bfb6a2f5d)
N-Pwell-Nwell

The parasitic device is typically not part of the  extracted netlist.     “Hot” parasitic bipolar NPN formed by adjacent ntype diffusions in the same substrate.      Parasitic NPN’s can be activated during ESD and  share ESD current.

![2 1 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/adc8af43-533d-4005-ba88-87b3885df232/adc8af43-533d-4005-ba88-87b3885df232.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=bce1f5e4d9b8e46e2581692249e24ec542be63fa)
## Layout Based Methods 

![VDD2  VDD2  VDD1  VDD1 Pr1 FrT  Pr2  Pr2  ‘ SVR  VR ’  ‘N+’  ">-++  ‘P-Sub'  ‘P-Sub’  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ddb18a49-b01f-4c09-9fc6-f504b31159a9/ddb18a49-b01f-4c09-9fc6-f504b31159a9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=be7d7d3c7e907a7319810deed3254c5812c705e9)
Detecting Parasitic Devices

![Input -Design GDS, Top  Input  -Design GDS, Top  Power/Ground,Rule File  Power/Ground, Rule File ‘ 'Get' Internal Power nets  Get ’ Internal Power nets All Power nets =  All Power nets  = Top + Internal Power nets  Top  + Internal Power nets ‘ 'Trace' connection for  Trace ’ connection for  "Hot_diffusions"  “ Hot_diffusions” D  D = Distance between two hot  = Distance between two hot  diffusions at different nets diffusions at different nets  D >  D critical  critical OK ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b42b70e7-e799-49b5-a406-87c5f42b03d1/b42b70e7-e799-49b5-a406-87c5f42b03d1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=80d261f5f002df7b51bbe27c278c766553cefa8c)
## Layout Based Methods 

![FSDPower  ESD Power Cell  I/O Cell  Driver  Receiver Receiver   VDD  VDD  ESD  ESD  Cell Del  VDD1 VDD   - Trigger  Circuit   VDD1 I/O VSS1 Voltage stress Voltage_stress  WSS  VSS ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bc9d05fa-e258-4546-a560-536069e6773b/bc9d05fa-e258-4546-a560-536069e6773b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=c3bcf85431e9b91bdc16d04a13214a482d1ad800)
Chip Integration Check with Point-to-Point Resistance Extraction

Vdd1_IO to Vss discharge has long and resistive path, but in schematic view it’s just a wire     Receiver gate exposed to high ESD stress     Different domains in different blocks, hard to spot     100’s/1000’s domain-crossing signals in SoC  48

## Layout Based Methods 

![VDD1  Ron1   Domain-4  Domain-3 c-ueoa  GND   Domain-1 Domain-1   Domain-4 Ron2  VDD2  Domain- omain-!  2 Domain-3 => Domain-4 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/73de7145-7d47-40bd-a9a3-75626a2e701e/73de7145-7d47-40bd-a9a3-75626a2e701e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=112c1a576c81ebed468b2013462f06725259fa4a)
Evaluation of ESD Robustness between Power Domains

Max voltage difference was 3.765V.

## Layout Based Methods 

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/19791f4b-0349-4bc4-960a-e5d3bdbf1ad6/19791f4b-0349-4bc4-960a-e5d3bdbf1ad6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=e691b1377a751514e58644d45646905a9a39a94d)
SEM Image of an Intra-Domain  Thin  Gate Oxide CDM Damage

![coremesh  victim  aggresso  resistive  only  With  inductance  inductive,all regions  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/877bcf26-eff8-46d9-9cff-b99a037c3618/877bcf26-eff8-46d9-9cff-b99a037c3618.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=ebf89759639194207fea17b784935b3403f93278)
![Aggressor-  Aggressorvictim  victim  bus  configuration  configuration  victim   of an intra-  of an intradomain  domain  aggressor  interface  interface ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/445e4efb-fd15-4fd8-baed-a3fd1822ad3d/445e4efb-fd15-4fd8-baed-a3fd1822ad3d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=021c0c56e124e809955d2e642035fedfe16aeaaa)
•  Simulation: Full chip & quasi-static   •  Ohmic contribution to impedance only cannot explain the defect   •  By including the impedance of the self-inductance (extracted by means of FastHenry), the voltage drop is high enough  $>$   BVox

## Layout Based Methods 

![Protection  Device  Bump  Common  Resistance  Victim  Device  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1466a201-d73c-4b5c-8e4a-780fc6b8ea01/1466a201-d73c-4b5c-8e4a-780fc6b8ea01.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=7ef90fda48557dc7781fd7d1b16e6886d5c2ef7c)
![RESD1 Rcommon  Rvictim I_ud（) I_v（2） udLv（) Expanded P2PExtraction Rules Rcommon + ResD1 =| ud Rcommon +Rvictim=|V REsD1 + Rvictim = ud_v ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6a5dbf75-bc0a-46a8-ae85-8e8181a5475f/6a5dbf75-bc0a-46a8-ae85-8e8181a5475f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=c5c85c2d8f79039939377ba9c2ed3904c279cf24)
Method for Removing Common IO Resistance in Layout Driven ESD Network Analysis

•  Use existing P2P extraction methods to protection devices   •  Added P2P extraction for IO to victim   •  Victim can be any device connected to IO that isn’t a protection device

$$R_{c o m m o n}=\frac{I_{-}u d+I_{-}v-u d_{-}v}{2}$$
## Other EDA Methods 

## Simulation-Based: 

• SPICE Compact Models   • TCAD

## Other: 

• Macro Checks   • Package Checks   • System Checks

## SPICE / Compact Modeling 

## ESD SPICE Challenges: 

Device compact model limitations in the ESD regime     Device failure modeling     ESD event source simulation     ESD testbench building

## Technology CAD (TCAD) Simulation 

Modern TCAD tools can be used to  bridge the gaps  in traditional ESD EDA design flow.

TCAD - physical device and process simulation. Device level TCAD  simulates device electrical  characteristics by solving semiconductor model equations either for a single device or within mixedmode circuit. Optionally, Finite Element (FE) analysis of physical semiconductor process steps can  be performed to obtain the devices structure.

TCAD allows predicting circuit performance when compact models are not available (e.g., during  technology definition and process development.

Mixed-Mode simulation supports analysis of circuits using both FEM and compact devices models.  Examples: parasitic structures formed in layout, transient latch-up problems, EOS cases, physical  ESD protection window; electro-thermal pulsed SOA, self-protection; physical mechanisms of  conductivity modulation, lateral isolation; impact of the device and process parameters on circuit  performance; multipoint sub-circuit optimization in ESD and OVP time domain; prediction of various  EOS effects for hot plug-in, inductive short, system level.

Advanced TCAD approach uses parameterized process and device templates extracted from  process diffused doping profiles. This allows bypassing very time-consuming process simulation.

## Macro Checks: Verification of I/O Placement  Rules 

Maximum number of I/O’s (i.e., distributed ESD protections) belonging to the same supply

ESD protection Frequency of power cells Frequency of trigger cells (if remote triggers are used) Placement of termination cells

![A  3  B  A I/O  IO power  I/O  IO power  I/O Interface Cell Termination cell  IO VDD IO VSS SS   IO VDD 00  IO VSS SSA   Termination cell Interface Cell I/O I/O I/O I/O  I/O Filler I/O I/O VDD VSS I/O I/O  I/O I/O I/O I/O C  C ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e851e302-a311-4a75-b2e1-ab5094fdc946/e851e302-a311-4a75-b2e1-ab5094fdc946.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=204742815875242e5e95b606c003f0d3f1e7a7ed)
![I/O Bank Integration  I/O Bank Integration  Violations Browser  Violations Browser /0wsm.ciamp  Marks segments and  areaswith ESDrule  violations  GroupsESDviolations  bytype  Provides information  aboutnatureofrule  violation  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/080c005c-7528-4061-853e-48cae26fe8be/080c005c-7528-4061-853e-48cae26fe8be.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=cb57921b3c6ff793344787508dc99dcf015678ce)
[Miller06, Etherton09]

## Package Level ESD Checks 

In traditional ESD EDA flows (topo/LDL/P2P/CD) does the package:   Only present another level of design hierarchy to check OR   Present unique ESD risks that need to be checked?     How does the package interact with other verification flows?   SPICE   Traditional flows (topo/LDL/P2P/CD)   System-level     Advanced packaging, chiplets, and 2.5D/3D integration   Is it necessary to check the entire system or is “divide and conquer sufficient”?   How to deal with multiple PDKs that will comprise a heterogenous package?   How to deal with complexity of multiple ESD targets (external I/Os, die-to-die)?   How to deal with the compute challenge, particularly for 3D/TSV/hybrid bonds?

## Package/System Checks: Integration  Verification - Package 

1.  Verify the integrity of the overall ESD protection network achieved at package pin   level.    2.  Verify that package RLC network is compatible with overall ESD protection scheme.   3.  Verify the integrity of the overall ESD protection network achieved at package pin level when  having multi-die (system in a package) designs.   4.  Verify that CDM peak current of the package-die system is below CDM current limit of the design


![Package  Package  Interconnect  Interconnect Bond Pad  Bond Pad VDD1  VDD1  VDD2区  VDD2 Power  Power   Power  Power  IN1  IN1  Clamp  Clamp   IN2区  IN2  Clamp  Clamp 1  2 N   N  VSS1-  VSS1  βVSS2  VSS2 57  57 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5027f3bd-1758-41c6-ae0e-16b19711220d/5027f3bd-1758-41c6-ae0e-16b19711220d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=d6d1ef09a103cd2d4c2cd757917a9880b5624c94)
![Cross-Die ESD  Current Path  买兴兴  Die1   le  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/de045861-3f22-4fa0-a322-394832dde08b/de045861-3f22-4fa0-a322-394832dde08b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=4b2225b8e30dd83e50e171a9b02df43af7faa478)
## System Level ESD Checks 

![TsV  VDD  VDD  chip   ChipB   chip   ChipA  Clamp   Clamp   TsV   Clamp   Clamp  SIG  Wss  Wss  TsV  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/be26d651-3ab5-4023-b0b7-92445b09560f/be26d651-3ab5-4023-b0b7-92445b09560f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=5cafb31cd8ea48f9387bb99ddda15a7c7791801e)
EDA for 3D-IC ESD Protection

EDA tools must perform component-level, not just die-level, ESD analysis to evaluate stress at internal I/O. Above: stacked dies from two design teams. Component ESD reliability can be sum of two, or limited by weakest  one, depending if rail clamps cooperate or compete.

## System Level ESD Checks 

|        Analysis                Components  TDPes      |        SEED (System                Efficient ESD                Design) Analysis      |Full Wave Analysis|        Near Field                Scanning                Analysis      |
|---|---|---|---|
|Simulation Engine|        Spice, Agilent ADS                transient, etc      |FullWaveDynamic|        NearField                Electromagnetic                Interference      |
|        Required Models for                Successful Simulation      |        PCB orselected                topologies on PCB      |        PCB or selected                topology on PCB      ||
|        Required Models for                Successful Simulation      |        ESD StressPulse or                TLP      |        ESD Stress Pulse,                (tlp?)      ||
|        Required Models for                Successful Simulation      |        PCB ESD protection                components (TVS,                cmc etc)      |        PCB ESD protection                components (TVS,                cImC etc)      ||
|        Required Models for                Successful Simulation      |IC pin response|IC pin response||
|        PCB/IC Operational                State      |Not Powered|Not Powered|        Poweredand                Operating      |


## Outline 

Basic ESD Concepts for EDA Verification   ESD EDA Verification Methods   Design Verification Flow   Conclusions   References

![Technology  Technology   Product Verification  Product Verification   Product  Product  Product Definition  Product Definition           ProductArchitecture  Product Architecture  Product Design  Product Design   Enablement  Enablement  Sign-off  Sign-off   Validation  Validation time iCProductDesignFiow  IC Product Design Flow  Floorplan IP Modules  Floorplan IP Modules and   Design IP Module  Design IP Modules   Full Chip IP  Full Chip IP  FullChip  Full Chip  Product   DesignI/OLibraries  Design I/O Libraries Digital I/O Banks,  andAnalogl/O  and Analog I/O  Ringsg  Rings  and I/O  I/O +  IP  +  Post-silicon/  Post-silicon /  Specifications  Specifications  Technology  Technology   Specifications  Specifications  Product  Product   Architecture and  Powidr &oGreund  Architecture and  Power & Ground  Product   Package  Package  Integration  Integration package  package +  Intackatgon  Integration Io  I/O +  DesignriRievtiw and  Design Review and  manufacturing  manufacturing  Pre-silicon/  Pre-silicon /   manufacturing  resalidatioAE  manufacturing  results & FAE validation  Grid Concept  package   Verification  +  +  System  System  System  System ESD Implementation Flow within a Particular Product Design(Life?) Cycle  ESD Implementation Flow within a Particular Product Design(Life?) Cycle   Co-design of  Es-designo   Es-dfsigncf  Co-design of   ESDTest  Define ESDProtection  Devicesand Devices to  be Protected from ESD  Devices and Devices to  be Protected from ESD  Define ESD Protection   DefineESD Com  Define ESD Components  or Cells per Pin  or Cells per Pin  Application  Application   Components and Library  Identify Required ESD  Identify Required ESD  Cells  Cells  andLibrary   New ESD and I/O  NewESDandI/O  LibraryCells  Design/Obtain  Design/Obtain  Library Cells   Co-design of ESD  Co-designofESD  andIP Modules  and IP Modules  Full Chip Integration  of IPs and I/Os,  Including ESD  IncludingESD   ESD for SOC  and Package andPackag   system(SEED)  system (SEED) Package  ESD for SOC,  Package and   ESDprotection  ESD protection sign-off  Qualification of IC  ESD Test  Product  Product ofIC  ESD Check Flow ESDCheckFlow  Schematic-Based Topological Checks  Schematic-Based Topological Checks Layout Based Checks(CD,P2P,LDL,DRC)  Layout Based Checks (CD, P2P, LDL, DRC) Package Checks  Package Checks System Checks  System Checks SPICE Modeling  SPICE Modeling TCAD Simulation  TCAD Simulation ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1862d92d-76e6-4e21-9ec0-26d2232a4d99/1862d92d-76e6-4e21-9ec0-26d2232a4d99.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=2a06419375ec054f3f1f3f4f7f8317782db9955d)
Design Verification Flow

## Design Verification Flow Implementation 

Check Objective:  Report ESD  vulnerable devices (V PAD_MAX  > V T1 )

Static Calculation of V PAD_MAX

$$\begin{array}{r l}&{V_{P A D_{-}M A X}=}\\ &{I_{E S D^{\times}}(R_{A}\!+\!R_{D i o d e}\!+\!R_{V d d}\!+\!R_{C l a m p}\!+\!R_{V s s})}\\ &{+V_{H D i o d e}\!+\!V_{H C l a m p}}\end{array}$$
![Rvdd  Rvss  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/dc77081a-867e-452a-b8ad-40d4b6915f44/dc77081a-867e-452a-b8ad-40d4b6915f44.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=940dcfac98d1b2bf7c65a1ea6c093f983bca1082)
What the EDA tool needs to do:

![70   ESD  Error  Check   Identify  Find   Yes  Pad   Connected  Nets   Devices   VT1   Vt1>Vpad_max   OK  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/669857f3-2f62-474a-b54c-7859df1cae02/669857f3-2f62-474a-b54c-7859df1cae02.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=43b433406c8098ddcfdcb9c447cf1487ee23460b)
What does the EDA tool need in order to do It?

## Design Verification Flow Implementation 

![NNO  No  ESD  ESD  Check  Check   Identify  Identify   Error Error  Find  Find  Pad  Pad   Connected  Connected   Yes  Yes Nets  Nets   Devices  Devices  V T1  V Vt1 >Vpad_max  T1 >V PAD_MAX  CK  OK ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6d80c0a4-a966-470b-a84d-3791cbc0f296/6d80c0a4-a966-470b-a84d-3791cbc0f296.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=4b80e9bfe0b6595ae49fcbdbd17b1e2b86c4d618)
|Task|Infrastructure/Data Required|Considerations/Questions|
|---|---|---|
|Find Pads|·Design Spec—List of Pads|·Where is Spec stored (in Design DB)?|
|Get Iesd|        ·Design Spec—-ESD Reqs.                ·Algorithm to Calculate IesD      |        ·Include headroom?                ·Based on nominal or hot ESD tester?      |
|        Find ESD                Cells and                Params      |        ·Template for ESD Cell matching                (name, topology)                ·ESD Cell Parameters      |        ·In Sync with ESD Library                ·How are parameters gathered?                ·Process variation?                ·Parameters stored in PDK      |
|         Routing                Res-      |        ·Design Spec                ·Extracted Values      |        ·Design Spec values prior to layout?                ·Extracted Values- How add to schematic      |
|Calc. Vpad|·Algorithm for calculation|·Allow series/parallel ESD Cells?|


## Design Verification Flow Implementation 

![NNO  No  ESD  ESD  Check  Check   Identify  Identify   Error Error  Find  Find  Pad  Pad   Connected  Connected   Yes Yes  Nets  Nets   Devices  Devices  V （11  T1  V Vt1>Vpad_max  T1 >V PAD_MAX  CK  OK ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/48b09598-171a-4dbc-8d98-a69dc69d2561/48b09598-171a-4dbc-8d98-a69dc69d2561.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=dcb98f3d62b3b302231bfc664d76d0010253f644)
|Task|Infrastructure/Data Required|Considerations/Questions|
|---|---|---|
|        Identify                Conn.      |        ·Template for how devices are                matched      |        ·In Sync with PDK devices                ·Able to handle large device portfolio      |
||        ·Template for how devices are                matched      ||
|||·Same device types (e.g. NMOS) |


## Design Verification Flow Implementation 

![7O  No  ESD  ESD  Check  Check   Identify  Identify   Error Error  Find  Find  Pad  Pad   Connected  Connected   yes  Yes WT1  VT1  Vti>Vpad_max  V  >V Nets  Nets   Devices  Devices  T1  PAD_MAX  OK ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9e142379-6ed7-47d0-95e7-ed1524bca148/9e142379-6ed7-47d0-95e7-ed1524bca148.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=7d490e148edf2de306eb97eed522c883e2233391)
|Task|Infrastructure/Data Required|Considerations/Questions|
|---|---|---|
|        Issue                 Error       |·Messages|        ·Nature of Error: Guideline? Warning? Error?                ·Nature of Message: What to do or what                condition was violated?      |
|        Issue                Error      |·Documentation/Help Guide|        · Explain why Error issued                · Explain what is expected as correction      |
|        Issue                 Error      |·Error Browsing/Documenting|        · Interface to catalog errors/comments                ·Method for Probing/Highlighting in Schematic      |


Alternate solutions allowed?  Are they coded?  If not, can ‘Error’ be waived?   MORE TO FOLLOW!!!

## Outline 

Basic ESD Concepts for EDA Verification   ESD EDA Verification Methods   Design Verification Flow   Conclusions   References

## Technical Report ESD TR18.0-01-14 

![ESDTR18.0-01-14  Revision ofESD TR18.01-11  ForESDElectronicDesign  AutomationChecks  Authors:  EDA Tool Working Group  ESDAssociation  ElectrostaticDischarge Association  7900 Turin Road,Bldg.3  Rome,NY13440  ASSOCIATION  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1f86b1db-bb64-450d-98ff-41a99f52029e/1f86b1db-bb64-450d-98ff-41a99f52029e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=d96f4ad01a22505514ff7a99fa3469c8e558600f)
The document provides a guideline for both EDA  industry and ESD design community

Establishes a comprehensive ESD  verification flow  satisfying the ESD design challenges of modern ICs.

This includes the definition of a common terminology  and the description of the required check types.

The document is aimed to convey the basic ESD  concepts and their implementation during the IC  design process to EDA industry and to make ESD  designer familiar with available types of EDA checks.

## Available for download from  

https://www.esda.org/store/standards/

## Acknowledgements 

## WG18 members: 

||        Michael Khazhinsky                Silicon Labs, Inc.      ||
|---|---|---|
|        Fabrice Blanc                ARM      |        Gianluca Boselli                Texas Instruments      |        Shuqing (Victor) Cao                GLOBALFOUNDRIES      |
|        Fabrice Blanc                ARM      |        Gianluca Boselli                Texas Instruments      ||
|        Norman Chang                ANSYS      |         Rosario Consiglio                Impulse Semiconductor, Inc.      |Maxim Ershov|
|        Norman Chang                ANSYS      |        Harald Gossner                Intel      |        Silicon Frontline                Matthew Hogan      |
|Mentor Graphics|        Harald Gossner                Intel      ||
|        Nitesh Trivedi                Infineon Technologies      |        Harald Gossner                Intel      |Vesselin Vassilev|
|        Nitesh Trivedi                Infineon Technologies      ||Novarell Technologies|


## Future ESD EDA Development 

ESD EDA verification using netlists extracted from layout   Improved run time/CPU/memory utilization/cloud computing   Better handling of large netlists   Expanded ESD check coverage (3D IC, modules, systems)   Hybrid static/dynamic EDA/SPICE analysis   Introduction of ESD EDA statistical and ML analyses    Standardization of input data for ESD EDA checks   Standardization of ESD EDA flow and verification approaches

## ESD EDA Tools and Methods Outlook 

![MIXED STATIC/SPICE-BASED MIXEDSTATIC/SPICE-BASED  MIXED LAYOUT/SCHEMATIC-BASED MIXEDLAYOUT/SCHEMATIC-BASED  Emerging  Emerging 2.5D/3D PACKAGE /MODULE-LEVEL 2.5D/3DPACKAGE/MODULE-LEVEL  Established Established  CLOUD COMPUTING CLOUD COMPUTING  SPICE COMPACT MODELING SPICECOMPACTMODELING  MACHINE LEARNING MACHINELEARNING  SYSTEMLEVEL  SYSTEM LEVEL PARALLEL COMPUTING PARALLELCOMPUTING  LOGICDRIVENLAYOUT  LOGIC DRIVEN LAYOUT CURRENTDENSITY  CURRENT DENSITY POINT-to-POINT RESISTANCE POINT-tO-POINTRESISTANCE  STATIC TOPOLOGICAL STATICTOPOLOGICAL  SPICE  SPICE TCAD  TCAD DRC  DRC 1980  1980  1985  1985  1990  1990  1995  1995  2000  2000  2005  2005  2010  2010  2015  2015  2020  2020  2025  2025  2030  2030 70 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7723705f-b4ce-4e44-a032-d19ddbd01ceb/7723705f-b4ce-4e44-a032-d19ddbd01ceb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=5640ee008c94adce1a15d4b4f2ac092c563bd965)
## Conclusions 

Automated verification tools for ESD are becoming more clearly defined and more  readily available     These tools provide great opportunities to expand the scope and precision of ESD  reviews     ESD EDA checks allow • Avoid many ESD design flaws, thereby reducing the overall design cycle time. •  Improve the ESD verification capabilities by operating on extended netlists.    •  Offer efficient method to check ESD robustness across all IC blocks at different  phases of design flow   •  Provide systematic approach for design optimization of ESD area and ESD protection  levels.

## References 

|[Alvarez17]|         DrAlvarez, N. Trivedi, M. Asam, “Influence of Self-Heating on ESD Current Distribution in Metal Lines,” EOS/ESD Symp                Proc., 2017, pp. 1-9.      |
|---|---|
|[Bairdo0]|        M. Baird and R. Ida, "VerifyESD: A Tool for Efficient Circuit Level ESD Simulation of Mixed-Signal ICs," EOS/ESD Symp                Proc., 2000, pp. 465-469.      |
|[Consiglio12]|        R.Consiglio, "Recent Developments inIntegrated Circuit (IC) ESD Electronic Design Automation (EDA), Silicon Valley                ESD Society Meeting Presentation at ISQED, March 2012.      |
|[Davis23]|        Jordan Davis, Chanhee Jeon, Woojin.Seo, “Method for Removing Common IO Resistance in Layout Driven ESD                Network Analysis,”IEW2023, poster #B6.      |
|[Di Sarro13]|        J. Di Sarro, B. Reynolds, and R. Gauthier, "lnfluence of Package Parasite Elements on CDM Stress," EOS/ESD Symp.                Proc., 2013, pp. 1-9.      |
|[Druen04]|        S. Druen, M. Streibl, K. Esmark, K. Domanski, J. Niemesheim, H. Gossner, D. Schmitt-Landsiedel; “Multi-Terminal                Pulsed Force  Sense ESD Verification of I/O'Libraries and ESD Simulations," EOS/ESD Symp. Proc., 2004, pp. 322-      |
|[Duvvury10]|C. Duvvury, “ESD On-chip Protection in Advanced Technologies,” EOS/ESD Symp. Tutorial, 2010.|
|[Ershov13]|        M. Ershov, Y. Feinberg, M. Cadjan, D. Klein, and M. Etherton, "EDA Software for Verification of Metal Interconnects in                ESD Protection Networks at Chip, Block, and Cell Level," EOS/ESD Symp. Proc., 2013, pp. 1-8.      |
|[Etherton09]|        M, Etherton, M. Khazhinsky, J: Miller, Y. Ziskis, A. Gilgur, Y. Lipa, “EDA Tool for Checking ESD Specific I/O Ring                Integration Rules," 3rd International ESD Workshop, 2009.      |
|[Etherton10]|        M. Etherton, M.Khazhinsky, S. Lorenz, L. Thiam, L, “EDA Tool for Checking Signal Power Domain Crossings,"                International ESD Workshop, 2010.      |
|[Franell08]|        E. Franell, S. Druen, H. Gossner, D. Schmitt-Landsiedel; “ESD full chip simulation: HBM and CDM requirements and                simulation approach", Adv. Radio Sci., 2008, pp. 245-251.      |
|[Gerdemann11]|        A. Gerdemann, J. W. Miller, M. Stockinger, N. Herr, A. Dobbin, and R. Ricklefs, "When Good Trigger Circuits Go Bad: A                Case History," EOS/ESD Symp. Proc., 2011, pp. 1-6.      |


## References 

E. Gevinti, M. Fragnoli, L. Cerati, A. Bogani, and A. Andreini, “HBM ESD EDA Check Method Applied to Complete Smart  Power IC’s - Functional Initialization and Implementation,” EOS/ESD Symp. Proc., 2013, pp. 1-8. E. Gevinti, L. Cerati, L. Di Biccari, G. Ballarin, A. Andreini, M. Fragnoli, and A. Bogani, “Schematic-Level and Layout-Level  ESD EDA Check Methodology Applied to Smart Power IC's - Initialization and Implementation,” EOS/ESD Symp. Proc.,  2015, pp. 1-10. E. Gevinti, G. Salzone, S. Angeli, L. Cerati, A. Bogani, A. Andreini, L. Di Biccari, L. Merlo, “EDA Checker for Identification  of Excessive ESD Voltage Drop – Implementation to Smart Power IC’s,” EOS/ESD Symp. Proc., 2017, pp. 1-10. S. Hayashi, F. Minami, and M. Yamada; “Full-Chip Analysis Method of ESD Protection Network,” ISQED Proc., 2004, pp.  439-444. M. Hogan, S. Srinivasan, D. Medhat, Z. Lu, and M. Hofmann, “Using Static Voltage Analysis and Voltage-Aware DRC to  Identify EOS and Oxide Breakdown Reliability Issues,” EOS/ESD Symp. Proc., 2013, pp. 1-8. K. Hsueh, S.-H. Ke, J. Lee, and E. Rosenbaum, “UVeriESD: An ESD Verification Tool for SoC Design,”  2008 APCCAS  Proc., 2008, pp. 53-56. Patrick Huff, Kai Esmark, Theresa Lutz, Christian Russ, “Influence of Bus Inductance on Product CDM Robustness,”  IEW2023, poster #B1. A. Ille, W. Stadler, T. Pompl, H. Gossner, T. Brodbeck, K. Esmark, P. Riess, D. Alvarez, K. Chatty, R. Gauthier, and A.  Bravaix, “Reliability Aspects of Gate Oxide under ESD Pulse Stress,” EOS/ESD Symp. Proc, 2007, pp. 328-337.   [Khazhinsky08]  M. G. Khazhinsky, V. Vassilev, H. Gossner, R. Consiglio, E. Franell, K. Hsueh, N. Trivedi, “Overview of ESD Electronic  Design Automation Check Requirements,” International ESD Workshop, 2008.   [Khazhinsky12]   M. Khazhinsky, S. Cao, H. Gossner, G. Boselli, and M. Etherton, “Electronic Design Automation (EDA) Solutions for ESDRobust Design and Verification,”  Custom Integrated Circuits Conf. (CICC) Proc., 2012, pp. 1-8.

[Huff23]

[Ille07]

## References 

[Khazhinsky15a]  M. Khazhinsky, “Verification Tools for ESD Protection Engineering (Part 1),” International ESD Workshop, 2015.   [Khazhinsky15b]  M. Khazhinsky, J. Scott, and P. Michelson, “Latch-up Verification/Rule Checking Throughout Circuit Design Flow,”  International ESD Workshop, 2015.   [Kim16]  J. Kim, N. Chan, H. Lan, K. Srinivasan, and N. Chang, “ESD Failure Analysis Methodology & Verification for Custom  Analog IP,” Design Automation Conf., 2016.   [Ku12]  T.-S. Ku, J.-W. Chen, G. Kokai, N. Chang, S.Lin, Y. Liu, Y.-S. Li, and B. Hu, "ESD Dynamic Methodology for Diagnosis  and Predictive Simulation of HBM/CDM Events," EOS/ESD Symp. Proc., 2012, pp. 1-9.   [Kunz10]  H. Kunz, G. Boselli, J. Brodsky, M. Hambardzumyan, and R. Eatmon, “An Automated ESD Verification Tool for Analog  Design,” EOS/ESD Symp. Proc., 2010, pp. 103-110.   [Kunz15]  H. Kunz, “Verification Tools for ESD Protection Engineering (Part 2),” International ESD Workshop, 2015.   [Lee00]  J. Lee, Y. Huh, J.-W. Chen, P- Bendix, S.-M. Kang, “Chip-Level Simulation for CDM Failures in MultiPower ICs,”  EOS/ESD Symp. Proc., 2000, pp. 456-464.    [Lee02]  J. Lee, K. Kim, and S. Kang, “VeriCDF: A New Verification Methodology for Charged Device Failures,” Design Automation  Conf. Proc., 2002, pp. 874-879.   [Lescot15]  J. Lescot, P. Dehan, W. Boujarra, D. Medhat, S. Billy, “A Comprehensive ESD Verification Flow   $@$   Transistor Level for  Large SoC Designs,” EOS/ESD Symp. Proc., 2015, pp. 1-10.   [Li10]  J. Li, R. Gauthier, A. Joshi, M. Lundberg, J. Connor, S. Chang, S. Mitra, and M. Muhammad, “Predictive Full Circuit ESD  Simulation and Analysis Using Extended ESD Compact Models: Methodology and Tool Implementation,” EOS/ESD  Symp. Proc., 2010,  pp. 1-8.

## References 

|[Lin09]|        L. Lin, X. Wang, H. Tang, Q. Fang, H. Zhao, A. Wang, R. Zhan, H. Xie, C. Gill, B. Zhao, Y. Zhou, G. Zhang, and X                Wang; “Whole-Chip ESD Protection Design Verification by CAD,”" EOS/ESD Symp. Proc., 2009, pp. 1-10.      |
|---|---|
|[Liu06]|        H.-Y. Liu, C.-W. Lin, S.-J. Chou, W.-T. Tu, C.-H. Liu, Y-W. Chang, and S.-Y. Kuo; "Current Path Analysis for                Electrostatic Discharge Protection," ICCAD Proc., 2006,      |
|[Lu1O]|        Z. Lu, D. A. Bell, “Hierarchical Verification of Chip-Level ESD Design Rules," EOS/ESD Symp. Proc., 2010, pp. 1-                6.      |
|[Miller06]|         J. Miller, M. Etherton, M. Khazhinsky, M. Stockinger, and J. Weldon, "Comprehensive ESD Protection for Flip-                Chip Products in a Dual Gate Oxide 65nm CMOS Technology." EOS/ESD Symp., 2006, pp. 1-10.      |
||        Chip Products in a Dual Gate Oxide 65nm CMOS Technology." EOS/ESD Symp., 2006, pp. 1-10.                S. Mitra, N. Palmer, M. Muhammad, and R. Gauthier, “Identification and Verification of BEOL Fails Due to ESD                Stress Using Current Density Analysis Tool," EOS/ESD Symp. Proc., 2013, pp. 1-8.      |
||        S. Mitra, N. Palmer, M. Muhammad, and R. Gauthier, “Identification and Verification of BEOL Fails Due to ESD                Stress Using Current Density Analysis Tool," EOS/ESD Symp. Proc., 2013, pp. 1-8.                [Muhammad10] M. Muhammad, R. Gauthier, J. Li, A. Ginawi, J. Montstream, S. Mitra, K. Chatty, A. Joshi, K. Henderson, N.                Palmer, B. Hulse, "An ESD Design Automation Framework and Tool Flow for Nanoscale CMOS Technologies,"                EOS/ESD Symp. Proc., 2010, pp. 1-6.                P. Ngan, R. Gramacy, C. Wong; D. Oliver, and T. Smedes, "Automatic Layout-based Verification of Electrostatic                Discharge Paths," EOS/ESD Symp. Proc., 2001, pp. 96-101.                A. Oberoi, M. Khazhinsky, J. Smith , and B. Moore, "Latch-up Characterization and Checking of a 55 nm CMOS                Mixed Voltage Design," EOS/ESD Symp. Proc., 2012, pp. 1-10.      |


## References 

[Okushima10]  M. Okushima, T. Kitayama, S. Kobayashi, T. Kato, M. Hirata, “Cross Domain Protection Analysis and Verification  using Whole Chip ESD Simulation”, EOS/ESD Symp. Proc., 2010, pp. 119-125.   [Pawaskar16]  P. Pawaskar, S. Mehetre, N. Pol, A. Narain, “Full-chip ESD Verification for Complex Multi-Domain Storage SoCs,”  Design Automation Conference, 2016.   [Qian04]  H. Qian, J.N. Kozhaya, S.R. Nassif, and S.S. Sapatnekar; “A Chip-level Electrostatic Discharge Simulation  Strategy,”  IEEE/ACM International Conference Computer Aided Design Proc., 2004, pp. 315-318.   [Rosenbaum11]  E. Rosenbaum, V. Shukla, and M.-S. Keel, “ESD Protection Networks for 3D Integrated Circuits,” 3D Systems  Integration Conf. (3DIC) Proc., 2011, pp. 1-7.   [Shukla13]  V. Shukla, G. Boselli, M. Dissegna, C. Duvvury, R. Sankaralingam, and E. Rosenbaum, “Predictive Modeling of  Peak Discharge Current during Charged Device Model Test of Microelectronic,” EOS/ESD Symp. Proc., 2013, pp.  1-8.   [Siha98]  S. Siha, H. Swaminathan, G. Kadamati, and C. Duvvury, “An Automated Tool for Detecting ESD Errors,”  EOS/ESD Symp. Proc., 1998, pp. 208-217.   [Smedes09]  T. Smedes, N. Trivedi, J. Fleurimont, A.J. Huitsing, P.C. de Jong, W. Scheucher, and J. van Zwol, “A DRC-based  Check Tool for ESD Layout Verification,” EOS/ESD Symp. Proc., 2009, pp. 292-300.   [Stockinger03]  M. Stockinger, J. W. Miller, M. G. Khazhinsky, C.A. Torres, J. C. Weldon, B. D Preble, M. J. Bayer, M. Akers, V. G.  Kamat, “Boosted and Distributed Rail Clamp Networks for ESD Protection in Advanced CMOS Technologies”,  EOS/ESD Symp. Proc., 2003, pp. 17-26.

## References 

M. Streibl, F. Zängl, K. Esmark, R. Schwencker, W. Stadler, H. Gossner, S. Drüen, and D. Schmitt-Landsiedel, “High  Abstraction Level Permutational ESD Concept Analysis,”  EOS/ESD Symp. Proc., 2003, pp. 122-130.   [Torres01]  C. A. Torres, J. W. Miller, M. Stockinger, M. D. Akers, M. G. Khazhinsky, J. C. Weldon, “Modular, portable, and easily  simulated ESD protection networks for advanced CMOS technologies,” EOS/ESD Symp. Proc., 2001, pp. 81-94.   [TR18.0-01-14]  M. Khazhinsky, F. Blanc., G. Boselli, S. Cao., N. Chang, R. Consiglio, M. Ershov, E. Gevinti, H. Gossner, M. Hogan, N.  Trivedi, and V. Vassilev, “ESD Electronic Design Automation Checks,” ESDA Technical Report TR18.0-01-14, 2014, pp. 1- 120.   [Trivedi07]  N. Trivedi, L Chant, P.C. de Jong, T. Smedes, “Two Approaches for design verification for ESD,” International ESD  Workshop Proc., 2007, pp. 408-418.   [Trivedi13]  N. Trivedi, S. Chakravarthy, D. Alvarez, and E. Weidner, “Optimized Netlist Checks - Full Chip ESD Verification,”  EOS/ESD Symp. Proc., 2013, pp. 1-8.   [Trivedi15]  N. Trivedi and D. Alvarez, “Essential - Integration of ESD Verification Methodologies,”  EOS/ESD Symp. Proc., 2015, pp.  1-9.   [Viale16]  B. Viale, M. Fer, L. Courau, P. Galy, and B. Allard, “An Automated Tool for Chip-Scale ESD Network Exploration and  Verification,” EOS/ESD Symp. Proc., 2016, pp. 1-10. M.-F. Wu, C.-C. Tsai, J.-C. Tseng, R. Chao, M.-H. Song, and Y.-K. Cheng, “An Efficient Full-Chip ESD Paths Resistance  Value Verification Flow for Large Scale Designs,”  EOS/ESD Symp. Proc., 2013, pp. 1-8.   [Zhan05]  R. Zhan, H. Xie, H. Feng, and A. Wang, “ESDZapper: A New Layout-level Verification Tool for Finding Critical Discharging  Path under ESD Stress,”  2005 ASPDAC Proc., 2005, pp. 79-82.

