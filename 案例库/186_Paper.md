---
title: "186_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_122a44c4ede9ff803fb7ba0605d28c847295230462135641
file_size: 615900
---

## A Failure Analysis of a SOP IC Creep Corrosion on  power module  

Weiwei Zhang \* , Yuanxin Lee, Yi Zhang, etc.  H3C Technologies Co., Limited, Failure Analysis Team, Hangzhou, China.  \* Phone: +86-571-86761878   Fax: +86-571-86762705   Email:  Weiwei_zhang@h3c.com

Abstract-   Creep corrosion classically happens on PCBs and  PCBAs working in Sulfur-rich environment with humidity.  Copper and silver metallization on PCB and PCBA could be  corroded by Sulfur-base gases. The associated corrosion products  can creep to adjacent circuits, making electrical short failure of  the system due to closely spaced metallized features on PCBs and  PCBAs. This paper will introduce a novel creep corrosion failure  of a SOP IC on power module. We found that a serial of flaws of  the SOP package could be the original point of creep corrosion  between adjacent pins. Finally, a serial of corrective methods was  proposed to mitigate the creep corrosion problem on this SOP  component.

Keywords  –  Creep corrosion, Copper, Silver, Corrosive gases,  Confirmal coating .

## I. I NTRODUCTION 

Creep corrosion, often happens on PCB and PCBA, is the  corrosion of the metallization (copper or silver) and the  migration of the corrosion product (copper and silver sulfide)  across the PCB & PCBA surface [1]. In harsh environments, the  sulfur bearing gases produce copper sulfide on PCB, which  may lead to electrical leakage failure between adjacent pads and  traces. G. Vogel proposed a mechanism for the creeping  corrosion of copper. He illustrated that at a relative humidity of   $>60\%$   and in the presence of H2S the whole PCBA is covered  with a layer of dilute acid. In pores or cracks over bare copper  immobile copper sulfide can be oxidized to mobile copper  oxide which moves to the surface [2].

A serial of power modules was reported “output voltage  error” in the field and the returned to FA lab for root cause  identification. Creep corrosion was found on a SO-8 chip along  the trimming flash between adjacent pins by optical inspection.  Optical Microscope, real time X-ray, SEM/EDS were used to  confirm the corrosion problem. EDS found the major elements  of the corrosion product crept along the flash were Cu, S, Ag,  and Cl. Optical inspection comparison was executed between  corrode chip type and no corrode chip type in new modules.  Exposed copper was found on corrode-type chip at the mold  trimming position, while by contrast, pins on non-corrode type  chip were finely enclosed with Ni/Sn. Cross section was  executed to find the structure of lead frame and the molding  compound. It was confirmed that the combination of the lead  frame and the molding was not solid, the silver layer for stich  bond on the lead frame inside the molding could react with the  corrosive gas via the micro crack of the package.

A reliability test with accelerated corrosive environment was  introduced to new modules with and without copper exposure  on the package. It was confirmed that chips with copper  exposure suffered creep corrosion obviously while chips with  pins finely enclosed by Ni/Sn or conformal coating were not  corrode.

A serial of improvement measures was proposed to solve the  problem after root cause identification and experimental  verification. A conformal coating of epoxy resin could be  sprayed by module manufacture to protect the exposed copper  and silver on the module. This proposal can effectively improve  the resistance to corrosion of the module without much process  change, but will induce challenge to rework process and cost  raise is predictable. To ameliorate creep corrosion issue,  module manufacture could also choose ICs without Cu & Ag  exposure by pushing IC supplier to improve the package  process or changing to IC suppliers without this kind of  package issue.

## II.   ANALYSIS  

Power modules with output voltage error were sent to FA lab  for root cause identification. External inspection of the module  PCBA found a SO-8 chip, used for voltage feedback, suffered  creep corrosion along the trimming flash between adjacent chip  pins, as shown in Fig 1. Failed chips were cut down from PCB  and sent to X-ray examination. Slight shadow was found  between adjacent pins at the trimming area, as shown in Fig 2.

![a  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/236d1fbf-303e-4934-a432-5c4e2dda9517/236d1fbf-303e-4934-a432-5c4e2dda9517.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215644%3B1743219244&q-key-time=1743215644%3B1743219244&q-header-list=host&q-url-param-list=&q-signature=46593b4103d8c5b2653c386d7c0936c23889a637)
Fig. 1 (a) Overall view and (b) detail view of the failure SO-8 chip.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4acbfa51-9264-4f84-b9d4-8d0ae599c742/4acbfa51-9264-4f84-b9d4-8d0ae599c742.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215644%3B1743219244&q-key-time=1743215644%3B1743219244&q-header-list=host&q-url-param-list=&q-signature=e53d43ec2198d2411fe82a15af6e4e13933d793d)
Fig. 2 X-ray image of the chip, suspect substance was found on the trimming  flash.

These failed SO-8 chips were sent to SEM/EDS analysis.  Dendritic growth of the corrosion product was seen at the  trimming flash between adjacent pins, as shown in Fig 3. The  major constituents of the corrosion product are copper & silver  sulfide with small amount of chloride. The copper sulfide  $\mathrm{Cu}_{2}\mathrm{S}$    is electrically conductive, which made short failure between  adjacent pins of the chip. Exposed copper was found on corrode  chip at the mold trimming position, while pins on no corrode  chip are finely enclosed with Ni/Sn by contrast, as shown in Fig  4. Creep corrosion can be easily happened when the exposed  copper of the chip lead frame contact with sulfur environment.

The SO-8 chip short failure is consistent with the failure  mode of the power module. After taking off the corrosion  product from the chip, the function of the power module was  recovered. It could be the conclusion that the failure of the  module was induced by creep corrosion of the copper in lead  frame.

Ag was found in the dendritic corrosion product as shown in  Fig 3. The lead frame outside molding compound is base  material copper with Ni and Sn plating. The source of Ag was  un-determined as no Ag contained in the lead outside the  molding compound. Cross section was introduced to find the  structure of lead frame and the molding compound, as shown in  Fig 5. It was confirmed that the combination of the lead frame  and the molding was not solid, the silver layer for stich bond on  the lead frame inside the molding could react with the corrosive  gas via the micro crack of the package, which leads to the Ag  corrosion.

![SEM HV:10.0 KV  WD:15.01 mm SEM MAG: 1.00 kx  Det:BSE  So View field: 189 μmDate(m/dy):08/10/15 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b1ad6dae-2702-4059-a2bd-33a266a43ecf/b1ad6dae-2702-4059-a2bd-33a266a43ecf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215644%3B1743219244&q-key-time=1743215644%3B1743219244&q-header-list=host&q-url-param-list=&q-signature=88a2ab506a1e517bc223ea44d9c76c95babed7e4)
Fig. 3 SEM image of the corrosion product.

![(aD  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/44cc5220-e874-4ed3-8dbc-a2b9e8f6181f/44cc5220-e874-4ed3-8dbc-a2b9e8f6181f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215644%3B1743219244&q-key-time=1743215644%3B1743219244&q-header-list=host&q-url-param-list=&q-signature=9f9bb8c24d59648a0512c86d3f63964a649d2c7a)
Fig. 4 (a) Corrode type: exposed copper at trimming position. (b)  Non-corrode type: copper is finely enclosed by Ni/Sn.

![Aglayer  GapofCapsulation  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e487b789-e735-48b6-bde6-536c4349e851/e487b789-e735-48b6-bde6-536c4349e851.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215644%3B1743219244&q-key-time=1743215644%3B1743219244&q-header-list=host&q-url-param-list=&q-signature=cd24556adf04514d5f1dce9cf45e7b85b189273c)
Fig. 5   Cross section of the corrode type chip. Ag layer can contact with air by  the micro gap between lead frame and the molding.

## III.   EXPERIMENTS  

A reliability test was executed on 3 groups 18 modules to  verify the creep corrosion in Mixed Flowing Gas condition. The  MFG test condition was followed GR-63-core outdoor [2]. Fig  6 showed the test system and EUT distribution.

EUT:

Group I. 6 modules used the copper exposed SO-8 chips,  same with the failure modules;

Group II. 6 modules used the same SO-8 chip with group I,  but with epoxy resin conformal coating on the chip;

Group III. 6 modules used another type of SO-8 chips with  pin copper enclosed with Ni/Sn.

Temperature/Humidity: 30,   $70\%$   R.H.

Gas source and concentration: Cl2=20 ppb, H2S=100 ppb,  NO2=200 ppb, SO2=200 ppb.

Test time: 240 hours.

MFG test result is shown in Fig 7 and Fig 8, group I suffered  creep corrosion of copper and silver while group II and group  III were clear. The failure of the power module with Cu & Ag  exposure on lead frame was reproduced by the test.  Improvement measures like conformal coating and IC supplier  changing were verified at the same time.

![b） ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2e2efb77-f1eb-4d3f-b122-98f449eaf6df/2e2efb77-f1eb-4d3f-b122-98f449eaf6df.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215644%3B1743219244&q-key-time=1743215644%3B1743219244&q-header-list=host&q-url-param-list=&q-signature=3c6f9bbf86904ddcf65eb08244367f7867abfc9e)
Fig. 6 (a) MFG test system and (b) EUT distribution.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/99ebcbc9-6089-4945-bf01-f2a839385b3c/99ebcbc9-6089-4945-bf01-f2a839385b3c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215644%3B1743219244&q-key-time=1743215644%3B1743219244&q-header-list=host&q-url-param-list=&q-signature=bd3a54e2ba91ae70fa0f732d4e43f28ae3d536fc)
![C  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9e847e8e-6013-485b-9260-901e69a0a662/9e847e8e-6013-485b-9260-901e69a0a662.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215644%3B1743219244&q-key-time=1743215644%3B1743219244&q-header-list=host&q-url-param-list=&q-signature=ebd994f1c76a321cf77bec5ff6fc8ad2c9f3c475)
Fig. 7 MFG verification result. (a) Group I: chip pins copper exposed, suffered  creep corrosion on lead frame; (b) Group II: conformal coating, clean on lead  frame; (c) Group III: chip pins copper enclosed with Ni/Sn, clean on lead frame.

![Elem   Weight   Ltotm  ernt  23.59  89   12.15  23.71   12.23  Ag L36.8611.20  Tota1100.00  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/54db9738-11ac-4c63-b3f6-d4627d932529/54db9738-11ac-4c63-b3f6-d4627d932529.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215644%3B1743219244&q-key-time=1743215644%3B1743219244&q-header-list=host&q-url-param-list=&q-signature=0ba79f0172d9f3f59174bf553a73df6c5b080534)
Fig. 8 Corrosion product of Group I.

## IV. C ONCLUSION 

Creep corrosion induced failures were found on power  modules, corrosion product along the trimming flash short  adjacent pins of the voltage feedback SOP chip. FA decided  that the root cause could be the package flaws of the chip, such  as Cu exposure at trimming position and Ag exposure by  non-solid combination of lead frame and molding compound.  The performed MFG test reproduced the failure phenomena and  verified the effectiveness of the improvement measures.  Conformal coating of epoxy resin can solve the problem  without much process change, but will induce cost raise and  challenges to rework process. Package process change of the  SOP IC to enclose Cu with Ni/Sn could effectively mitigate the  creep corrosion issue.

## R EFERENCES 

[1]    Randy Schueller, “Creep corrosion on lead-free PCB in high sulfur  environments”,   Intel, SMTA Proceedings, Orlando, FL, Oct. 2007.    [2]    Gert Vogel, “Creeping corrosion of copper on printed circuit board  assemblies”, Microelectronics Reliability (September 2016), Vol 64, pp.  650-655, https://doi.org/10.1016/j.microrel.2016.07.043.    [3]    Issue 5 of GR-63, NEBS Requirements: Physical Protection, Chapter 5,  pp. 51-60, 2017.

