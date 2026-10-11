---
title: "205_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_eea4e48336251fb3ecca4f46d70421147295230462135641
file_size: 1778941
---

## An Efficient and Non-destructive Grounding Method  for Passive Voltage Contrast Fault Isolation   

Irene Tee\*, Kok Wah Lee, Jie Zhu and Zhi Qiang Mo  GLOBALFOUNDRIES Singapore Pte. Ltd,   60 Woodlands Industrial Park D, Street 2, Singapore 738406..   \* Phone: +65-66701515   Fax: +65-66700425   Email: irene.tee@globalfoundries.com

Abstract- Voltage contrast is widely utilized as a localization  method for opens (or shorts) on circuits and test structures.  Conventional Passive Voltage Contrast grounding methods are  mainly grouped into two types. First method, laser ablation  forming a hole down to substrate and connecting the substrate  with grounding pad using Focused Ion Beam (FIB) Pt deposition.  Second method, FIB ion mill a hole down to substrate and then  connect substrate with grounding pad using FIB Pt deposition.  New grounding method using OmniProbe micromanipulator  introduced to eliminate contamination due to laser ablation,  re-deposition during FIB milling and it is non-destructive with the  ease to switch grounding pad as needed.

Keywords – Passive Voltage Contrast, Grounding method,  Focus Ion Beam .

## I. I NTRODUCTION 

Defective interconnections are a common issue in  semiconductor production and pose a problem with every new  technology generation. Passive voltage contrast (PVC) is  commonly used for failure localization in semiconductor  product failure analysis. The common PVC localization method  is based on contrast differences in by either Scanning Electron  Microscopy (SEM) or Focused Ion Beam (FIB). It has the  capability to narrow down open, resistive or leaky node until  single via or contact dimension makes it widely used and  accepted across semiconductor failure analysis industry.  Grounding one end of the structure and leaving another one  floating is necessary step to gain PVC. The normal procedure is  to form a deep hole down to substrate and deposit Pt to connect  the pad to substrate through the deep hole. In this way, the pad  gets grounded through the Si substrate. In most of the time for  semiconductor devices, PVC requires to charge the sample  surface positively, so that all the exposed metal structures with  the grounding path will be bright while as the floating become  dark. As a result, any unexpected reversal in contrast indicates  abnormal occurs in the metal or its connections.

Conventional PVC grounding method can be grouped into  two methods. First method, forming a hole down to substrate  with laser ablation and connecting the substrate with grounding  pad using Pt deposition. The second method, forming a hole  down to substrate with Focused Ion Beam (FIB) and connecting  the substrate with grounding pad using Pt deposition. However,  both methods often encounter challenges such as laser ablation  induces large stress to structure (Fig.1), contaminates

surrounding ablated area with residue or particles from laser  ablation hole (Fig.2). Whereas, FIB milling is time consuming  to form large and deep enough hole down to Si substrate. Pt  deposition to connect the hole to grounding pad also creates  large conductive surface which jeopardize subsequent PVC test  result (Fig.3). Electron or Ion beam Pt deposition may cause  sensitive open structure exploded during Pt deposition. Both  laser ablation and FIB milling are destructive grounding  method, e.g., can’t change grounding pad  to another one if no  PVC is observed at first time or wish to have a different test  direction.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/87d65b0c-136b-4671-b013-7afa977af0f2/87d65b0c-136b-4671-b013-7afa977af0f2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215658%3B1743219258&q-key-time=1743215658%3B1743219258&q-header-list=host&q-url-param-list=&q-signature=8f42834ed9356c22edcb59e4b9c5c58a019d80fb)
Fig. 1 Via exploded due to stress after laser ablation.

![.  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5252dd11-ca0c-4c6e-88da-d11dbc5c7a3b/5252dd11-ca0c-4c6e-88da-d11dbc5c7a3b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215658%3B1743219258&q-key-time=1743215658%3B1743219258&q-header-list=host&q-url-param-list=&q-signature=e2dddfd2155c6d94a1f087c29bafb91840c67995)
Fig. 2 Laser ablation induces residue and particles at surrounding area.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9b726884-e0da-4434-ad92-f92a93afba7d/9b726884-e0da-4434-ad92-f92a93afba7d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215658%3B1743219258&q-key-time=1743215658%3B1743219258&q-header-list=host&q-url-param-list=&q-signature=2bf2a95f63eeefc2201d06b27b299f71239823a6)
Fig. 3 Contamination found on surrounding area after Pt deposition.

For the PVC condition, both SEM and FIB are tried on dual  Beam focused ion beam machine FEI Helios 450HP. For SEM,  different settings of accelerating voltage and electron beam  current are tried. For FIB, the accelerating voltage is fixed at   $30\mathrm{kV}$   to maintain a good lateral resolution and signal intensity.  The scanning dwell time is set to 300ns and ion beam current is  set to 28pA.

Introducing an efficient grounding method uses FEI Helios  450HP equipped with OmniProbe micromanipulator. This  method basically overcome most of the challenges encountered  using laser ablation and FIB grounding. It does not need to drill  hole to substrate level, save time and avoid any surface  contamination. This method also do not need to use any GIS Pt  deposition to bridge ground hole and pad, avoid current  over-flow and surface contamination. This is also a  non-destructive approach, allows us to probe on either side of  two grounding pads, higher success rate and flexibility to test  on either end of structure. Furthermore, it is very easy and  efficient grounding method and OmniProbe micromanipulator  is made of W which is a good conductor.

## II.   EXPERIMENTAL   RESULT  

## A.    Case Study 1  

The sample used for below experiment is shown in Fig.4. It is  a SOI wafer with metal 1/ via / metal 2 open issue. The structure  contains approximately 400 vias. De-processing is performed to  expose top covering metals and then the sample was inspected  with 1kV electron energy to ensure the structure surface is  clean, metals are intact and ready for PVC.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cd1d3e70-35a5-473c-a411-18b8fec57ee4/cd1d3e70-35a5-473c-a411-18b8fec57ee4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215658%3B1743219258&q-key-time=1743215658%3B1743219258&q-header-list=host&q-url-param-list=&q-signature=41b2af0356adba03337cc5ab6c5f2bbe7bcbe530)
Fig. 4 SEM image before FIB grounding.

Fig. 5 (a) shows a micromanipulator above the grounding  pad, before touching on pad all floating structure are dark.  OmniProbe manipulator is then lower down slowly to touch on  the grounding pad, successfully observed PVC at the 1st M2,  PVC appears quickly and remain stable as seen on Fig. 5 (b).  TEM sample was prepared along Metal 2 at the contrast  different shown by PVC. TEM analysis (Fig.6) show Cu voids  observed below via 1.

![a  (a)                                (b)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b42adf57-add5-4028-a256-ae4b035dbb5e/b42adf57-add5-4028-a256-ae4b035dbb5e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215658%3B1743219258&q-key-time=1743215658%3B1743219258&q-header-list=host&q-url-param-list=&q-signature=4d25ab04bab8fe7e5a2da25536add8db5aba10b1)
Fig. 5 (a) and (b) I-beam image before & after OmniProbe touch on pad.

![Ca  (a)                                (b)  Cb    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cfa6efd6-3869-4319-aeae-3364efa26d20/cfa6efd6-3869-4319-aeae-3364efa26d20.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215658%3B1743219258&q-key-time=1743215658%3B1743219258&q-header-list=host&q-url-param-list=&q-signature=6060eed7e49383d7fb17b705c57591ba790d501c)
Fig. 6 (a) and (b) TEM image along metal 2 reveal Cu voids below via 1 bottom.

## B.    Case Study 2  

Another experiment is conducted on a non SOI device with  tested CCV4 ET open issue. This new grounding method is  non-destructive and flexible to change either pad to be the  grounding pad making obtaining more than one defective  connector possible. As shown in Fig.7, the bottom pad is firstly  selected as the grounding pad. Obvious PVC is observed at the  9th row of the chain from bottom up.

![Ca  (a)                                (b)  b  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c0748b3a-fbab-4c61-bc87-8843283e4dd6/c0748b3a-fbab-4c61-bc87-8843283e4dd6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215658%3B1743219258&q-key-time=1743215658%3B1743219258&q-header-list=host&q-url-param-list=&q-signature=5323a1671eef42e61b6cf13ba3c4ecf27394f9d9)
Fig. 7 (a) and (b) Bottom pad as grounding pad.

![(a)                                (b)  Cb  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/443b9309-d775-438f-acd2-5436285abfe6/443b9309-d775-438f-acd2-5436285abfe6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215658%3B1743219258&q-key-time=1743215658%3B1743219258&q-header-list=host&q-url-param-list=&q-signature=205ae6f0865e67055c63741071e1a076b0785248)
Fig. 8 (a) and (b) Top pad as grounding pad.

The grounding pad is then changed to top pad. Obvious PVC  again obtained at 2nd row of chain from top down (Fig.8). It  eliminates the constraints of obtaining only the 1st defect from  the grounding pad, allowing PVC test from another direction  which may also provide second defective connector within the  same test structure feasible.

## C.    Case Study 3  

Benefited with the non-destructive signature, further  experiments can be carried out on same structure with tested ET  failure. This grounding method is flexible not only to change  different grounding pad, it even has the freedom to use selective  via as the grounding point. As shown in Fig.9, the  micromanipulator is then landed on the second row of via  chains, this make it become the new grounding point.

Multiple trial on different via as grounding point, PVC  observe contrast at multiple sites (Fig.10). Imply the whole ET  structure may have same issue instead of single or few vias  open.

![(a)                                (b)  b)    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/84dae025-78dd-43e1-ac82-9551f89e55a2/84dae025-78dd-43e1-ac82-9551f89e55a2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215658%3B1743219258&q-key-time=1743215658%3B1743219258&q-header-list=host&q-url-param-list=&q-signature=9b5d9825dc9e34e0dd63de56ca1503f09e0fcc7f)
Fig. 9 (a) and (b) Manipulator above via structure, structure all dark,  manipulator slightly touched on 2nd row of via chain from top.

![(a)                                (b)  b  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/01ca813f-949f-4198-acb9-148b47350895/01ca813f-949f-4198-acb9-148b47350895.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215658%3B1743219258&q-key-time=1743215658%3B1743219258&q-header-list=host&q-url-param-list=&q-signature=e3f92395ce930ff53033b35495c2bcd6dc1abce9)
Fig. 10 (a) and (b) 4th row & (b) 8th row of via chain selected as grounding  point.

FIB cross section cut on the failure location reveals the  missing of contact in the metal/via stack (Fig.11).

![Ca  (a)                                (b)  Co    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c6eaeef8-8282-472e-9310-3ea370f847c8/c6eaeef8-8282-472e-9310-3ea370f847c8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215658%3B1743219258&q-key-time=1743215658%3B1743219258&q-header-list=host&q-url-param-list=&q-signature=41e1b6ea3814885ca7f076ec2bf97d98e9ea6e0f)
Fig. 11 (a) and (b) FIB cross section on the failure sites.

## III. C ONCLUSION   

This efficient and non-destructive grounding method shows  great potential in eliminate most of the challenges encountered  while using conventional grounding method. As shown in these  experiments, application of the new grounding method using  OmniProbe manipulator is easy and flexible. Most importantly,  this new grounding method is non-destructive and it allows  further PVC analysis on different locations feasible.

## A CKNOWLEDGMENT 

The authors would like to thank Quality Management Team  for all the help and guideline in writing this paper

## R EFERENCES 

[1]    YiQiang Shen, Irene Tee and Jie Zhu, “Passive voltage contrast  investigation of metal/via stack connecting to substrate,” IPFA, 2018.    [2]    R. Rosenkranz, "Failure localization with active and passive voltage  contrast in FIB and SEM",  Journal of Materials Science , vol. 22, no. 10,  pp. 1523-1535, 2011.    [3]    R. Rosenkranz, W. Werner, “Active Voltage Contrast for Failure  Localization in Test Structures,”  Proc. of the 29th International  Symposium on Testing and Failure Analysis, ASM International  pp.  316-320, 2006.     [4]    Michael Strizich, MicroNet Solutions Inc., “Voltage Contrast and EBIC  Failure   Isolation   Techniques,”   Available:  https://docplayer.net/25443273-Voltage-contrast-and-ebic-failure-isolati on-techniques.html    [5]    Ruediger Rosenkranz, “Failure localization with active and passive  voltage contrast in FIB and SEM”, in Journal of Materials Science:  Materials in Electronics,” Oct, 2011.

