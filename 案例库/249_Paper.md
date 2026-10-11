---
title: "249_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_29bfc26c3342910eb8eb3ba4b84ea9c57295230462135641
file_size: 5708405
---

## Application of Laser Deprocessing Technique in Physical  Failure Analysis on Memory Bit-counting   

Yanlin PAN\*, Yuzhe ZHAO, Pik Kee TAN, Patrick KHOO, Pui Ying YEO, Siong Luong TING, Hao TAN,  and Changqing CHEN   GLOBALFOUNDRIES Singapore Pte. Ltd. 60 Woodlands Industrial Park D Street 2, Singapore 738406.  Phone: +65 9114 9926 Fax: +65 8765 4321 \*Email:  yanlin.pan@globalfoundries.com

Abstract-   With continuous technology scaling of semiconductor  devices, conventional physical failure analysis (PFA) techniques  becomes more and more challenging with the increased number of  transistors and layer stacks. This paper presents a new memory  bit-counting method in PFA by employing laser deprocessing  technique (LDT). This LDT assisted new method is more  cost-effective and efficient in the PFA on memory bit-counting in  terms of shortening the total FA cycle time and lowering the  requirements for the experimental equipment, which leads to the  increase of PFA throughput in memory devices especially for high  technology nodes.

Keywords  –  Laser deprocessing, PFA, Bit-counting, TEM .

## I. I NTRODUCTION 

Physical failure analysis (PFA) is an important failure  analysis (FA) branch for defect identification in devices and  process improvement. Layer by layer deprocessing and  inspection is one of the common PFA techniques. In many PFA  cases on memory failure devices, bit-counting for transmission  electron microscopy (TEM) analysis on various memory  failures is required after the target layer is reached.

In the static random access memory (SRAM) devices,  bit-counting is usually performed at Metal2 (M2) or lower  levels where both of the bit lines (BLs) and the word lines  (WLs) are visible and countable. However, for some special  cases where the critical dimension (CD) measurement on Via2  (V2) layer is requested or V2 void is suspected, bit-counting  needs to be performed at M3 layer or even higher level. Hence  the conventional method by mechanical polishing and scanning  electron microscopy (SEM) inspection is no longer suitable.  Therefore, new bit-counting method is highly desired. The  situation is similar in the non-volatile memory (NVM) devices.  For NVM devices, bit-counting needs to be done without  removing the M5 layer (the metal layer connecting the upper  electrode of the memory cell to the top metal layers) to avoid  the damaging on the target memory cells right below ( Fig. 1a,  b ) by mechanical polishing, which makes the WL counting in  the NVM devices one of the most challenging PFA processes  considering the large repeating bit array in each memory block.

Previously, two conventional methods have been developed  for the memory bit-counting for the NVM devices. One is  utilizing FIB to mill off the M5 layer at certain BLs away from  the target area to count the cells (count the WLs) along the M5  metal line direction.  The other one is counting the Mvia (count  the WLs) exposed by over-RIE the whole sample surface with

Pt protection on only the specific target area ( Fig. 2 ). For the  first method, FIB offers the advantages of localized milling and  real-time monitoring of the milling without transferring  samples between different inspections tools. However, this  method is only workable in the dual beam FIB-SEM system  which comes with higher cost compared to single beam SEM  system, and it would also be time consuming if the target bit is  far from the edge of the memory block. The second method  requires only a single beam SEM system, but would introduce  the risk of sample damaging by the Pt protection layer  miss-covering the target bit. The risk can be reduced by  increasing the size of the Pt protection layer while it costs more  machine time and Pt source. Moreover, with continuous NVM  device dimension scaling, below 28nm technology node the  Mvia size shrinks smaller than the M5 metal, which makes the  over-RIE method not applicable for bit-counting.

![(a)  BL1  BL2  BL3 Memorycell L1 WL2 WVL3 (D）  Count BLs 115 M5 trench c Mvia ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/817b37ae-867e-4d02-a880-1b47e63d0d11/817b37ae-867e-4d02-a880-1b47e63d0d11.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=8c07a75413797ae8e82c5f062f61254abfa642e2)
Fig. 1 . (a) Typical circuit diagram of NVM memory array. (b) Memory  bit-counting in the NVM devices.

In this paper, we will introduce a new method for the memory  bit-counting in PFA which is suitable for both SRAM and  NVM devices. The new method employs the laser deprocessing  technique (LDT) that has been used to flatten unevenness and  remove unwanted layers in PFA in the previous studies [1-4].

![Conventional method 1  Count the M5 (BLs) and the cells  FIB mills away the M5 layer to  Sample delayered to M5.   expose the memory cells.   (WLs) to Pt mark the target bit.  W2  Conventional method 2   Over-RlE to expose the Mvia. Count the  Roughly locate the target bit by  M5 (BLs) and the Mvia (WLs) to Pt mark  measurement and deposit a Pt  the target bit.  Sample delayered to M5.   protection layer on it.  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c240dd02-4bdc-4f5a-ba9d-c319d98c4551/c240dd02-4bdc-4f5a-ba9d-c319d98c4551.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=9d0f0ed897b827d1b771da169701c72ecb645143)
Fig. 2 . Conventional methods for memory bit-counting in the NVM devices. Red dash line circled is the target bit.

LDT is fast, simple, and provides uniform deprocessed sample  surface within large area. Compared with FIB, LDT is more  economical and efficient in the PFA on memory bit-counting.

## II.   TECHNIQUE   AND   EXPERIMENTS  

The experiments were performed on a   $28\,\mathrm{\nm}$  technology  node NVM device and a 40 nm technology node SRAM device.  After mechanical polishing (ALLIED polisher) on the sample, a  laser deprocessing system (New Wave Research Ezlaze3) was  used in the bit-counting experiments. The laser has a  wavelength of   $532\mathrm{nm}$   and was integrated into a probe station  (Cascade Microtech PM5). The laser pulse has an adjustable  energy ranging from 0 to   $0.5\;\mathrm{mJ}$   and a fixed pulse width of   ${\sim}5$    ns. Laser power and number of shot were studied on the dummy  sample at M5 level, as shown in  Fig. 3 . As per the results, we  selected one shot and   $90\%$   laser power for the deprocessing  experiments. It is worth to mention that the laser power would  be slightly different depending on the thickness of the dielectric  left on the M5 layer. A   $20\times$   objective lens was used for the  optical microscope (OM) with laser opening window size of 20   $\upmu\mathrm{m}\times40~\upmu\mathrm{m}$  . The window size is dependent on how many bits  to count. A single beam SEM system (FEI Magellan TM  400L)  equipped with a gas injection system was used for the sample  inspection and Pt mark deposition.

![OV   509%   80%   100%   70%  One shot   Oneshot   One shot   Twoshots  30%   70%   90%   60%  One shot   One shot   One shot   Twoshots  90%one shot was  chosen in this case  SEN  Notsuitabl   Suitableforbit-   Multipleshotscreate  counting   uneven surface. Not  suitable  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d366fcea-1646-464e-bc35-03f53f1005d0/d366fcea-1646-464e-bc35-03f53f1005d0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=ddc3ce5b36f02deb96d0bbe2414e79f893472d64)
Fig. 3 . Parameter study of the laser deprocessing on the dummy sample at M5  level.

![Laserbeam  aser deprocessingsystem   Ptmarks  Targetbit   Bit-counting area  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5fe1965a-265d-446e-8a45-a820270b1fb0/5fe1965a-265d-446e-8a45-a820270b1fb0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=cef1b9c9978bd1f5f76ac27f31ed3d1ab275b8e2)
Fig. 4 . Schematic of laser deprocessing and Pt marking steps in NVM devices.

The following steps describe how to use LDT to do the  memory bit-counting in NVM devices.

1)    Sample is delayered until M5 layer.    2)    Make Pt mark on the target BL in SEM as a reference for  the laser deprocessing in OM.    3)    Remove the M5 layer by laser deprocessing at certain BLs  away from the target BL to expose the cells in the reference  area. Water polish using the polisher to clean the laser burst  debris off the sample surface before bit-counting ( Fig. 4 ).    4)    Count the cells (WLs) in the laser deprocessed reference  area and the M5 metal lines (BLs) to locate the indicated  target bit from the memory block ( Fig. 4 ).    5)    Make Pt mark exactly on the target bit for TEM sample  preparation ( Fig. 4 ).

Table 1.  Operation time (in hours) comparison between the conventional  methods and the new method.

||        Ptmark                target                BL      |        Deposit                Pt protection                layer      |        over                RIE      |        FIB                milling      |        Laser                deprocessing      |        Count                LS      |Total|
|---|---|---|---|---|---|---|---|
|        Conventional                method 1      |NA|~0.6hr|~0.2hr|NA||～0.7hr|~1.5hr|
|        Conventional                method2      |~0.3hr|NA||~0.8 hr||~0.5hr|~1.6 hr|
| New method|~0.3 hr|NA||N|~0.1 hr|~0.5hr|~0.9hr|


For SRAM devices, the procedure is similar except Step 3  where both BLs and WLs need the laser deprocessed reference  area for the counting.  Table 1  shows the comparison of the  operation time between the conventional methods and the new  method. Time usage of each step varies slightly with the case  requirement and the experience of the operator. Here the time  usage is evaluated under the same condition. We can see the  new method shortens the operation time by   $40–45\%$  . TEM  sample was prepared using a dual beam FIB-SEM system (FEI  Helios NanoLab 450S). TEM analysis and EDX mapping were

performed using a 200kV Field Emission TEM (JEOL  JEM-2100F) equipped with SDD EDX detector (Oxford  X-Max N  100TLE).

## III. R ESULTS AND DISCUSSION 

## Case study on NVM device  

Fig. 5  shows the GDS layout of the M5 layer in the NVM  device. After the wafer sort, a data log provides the bitmap  information. Referring to the e-test results, the NVM chip  shows single bit open failure at the indicated location. The  sample was delayered until M5 level by mechanical polishing,  followed by LDT assisted memory bit-counting as shown in  Fig. 6 . A  $45^{\circ}$   angled Pt mark was marked below the target BL in  case the Pt mark on the target BL was not clearly visible in the  OM. LDT was used to expose an area of the memory cells at  around 30 BLs to the left of the target BL, in which the WLs  were counted. BLs were counted on the M5 metal lines. Then  the final Pt cross mark was deposited on the target bit for the  further TEM sample preparation and analysis.

![M15  Targetbit  DS  CoreStrip  X05Y12  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1b2bb2d8-19db-444b-98ce-f00653532b99/1b2bb2d8-19db-444b-98ce-f00653532b99.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=b4b837d69ce2f04746460813c2e2b5edbe2df161)
Fig. 5 . GDS layout of the M5 layer in the NVM device.

1.Pt markthetargetBL.

![Layout  OM   SEM  TargetBL  45°Pt mark  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/66a5e570-e7a0-4ed6-9b09-96ec06030e68/66a5e570-e7a0-4ed6-9b09-96ec06030e68.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=bfba4d7cbff8a9d3133b96d1809550dce14134d5)
Il.LaserdeprocessingontheareanearthetargetBL

![ONM   Laserdeprocessedarea  SEM  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d2a241b9-f695-4617-8968-dbdbe8324ca8/d2a241b9-f695-4617-8968-dbdbe8324ca8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=f4a04afa9ce77fce2296df53f111196c616af75f)
![Layout  NL2  NLD  RedundantWL   TargetWL  RedundantWL  DummyWL  DummyWL  SEM   Ptmarkon thetarget  SEM   Count the WLs in the   SEM   bit after locating it.  deprocessedarea.  TargetBL  TargetBL  TargetWL  一一  TargetWL  TEM direction  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8f34d57a-e334-443c-b843-15e139ca8c92/8f34d57a-e334-443c-b843-15e139ca8c92.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=d1a408b3f1564d01613d1bbf3d272ccdc2402e6f)
Fig. 6 . Schematic of the LDT application steps. Solution for the memory bit-counting at M5 level in the NVM device.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9abf749e-8225-405a-8d6d-92450bede703/9abf749e-8225-405a-8d6d-92450bede703.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=259cc6af53c7d9bdef3be1d4ac0b86e9761e572e)
Fig. 7 . TEM (Y direction cut on the sample in  Fig. 6 ) images of the target bit  and the reference bit.

From the TEM results ( Fig. 7 ), unlanded/partial landed M5  trench on the memory cell was observed at the target bit, which  is mainly due to the defect induced etching issue. In addition,  small cell dimension was observed, which is  ${\sim}20\%$   smaller than  the reference bit.

![SEM  Ref   arget   Ref  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f9e747ba-fab5-4221-8781-ec8f8743fcda/f9e747ba-fab5-4221-8781-ec8f8743fcda.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=2ca3933b363eeb93fa659e4619c8958b1fbf7f60)
Fig. 8 . STEM (X direction cut on another 28 nm NVM sample) images of the  target bit and the reference bit.

Fig. 8  shows the STEM images on another 28nm NVM  sample, where the TEM sample was cut across the M5 metal  lines (X direction). Compared to the reference bit, the target bit  has an abnormal Mvia bottom profile, which induced the higher  landing resistance. For X direction TEM analysis, this method  has its unique advantage on precisely determining the target  WL.

## Case study on SRAM device  

LDT is also very useful in PFA on SRAM devices .  In this  case, a SRAM of 40nm prototype chip with SRAM block was  analyzed by bitmap and found to exhibit a 3-bits cluster failure

mechanism. Cu void in V1 or V2 was highly suspected and CD  measurements were needed, so the delayering was stopped at  M3.  Fig. 9  shows the typical GDS layout of SRAM device. As  we can see, bit-counting at M3 level is impossible. Both WLs  and BLs cannot be properly identified and counted because of  the lack of reference structure and pattern. We can further  polish to V2 for the bit-counting and TEM analysis. However,  the CD measurements on V2 will be unavailable due to M3  missing, which sometimes are critical for the root cause  analysis. One failed example is shown in  Fig. 10 . In our work,  we resolve the problem by using LDT to create a reference area  near the target bit at M3 level ( Fig. 11 ), similar as we did in  NVM devices.

After the target bit was located and Pt marked, TEM analysis  was carried out for high spatial resolution analysis.  Fig. 12   shows the TEM images of the failed 3-bits cluster. Metal void  was observed in V1 and the CD measurements were taken as  required by customer. To study the void mechanism, EDX  elemental mapping was performed on the defect and the results  are shown in  Fig. 13 . The EDX results clearly revealed the Cu  migration/diffusion at the void, as arrowed. From the results of  TEM imaging and elemental analysis, it is suspected that the  root cause of the failure is the oxidation or corrosion of the seed  layer during the bulk Cu plating. High aspect ratio of the trench  etching in the damascene process could introduce the seed layer  thinning at bottom of the trench. In the subsequent plating  process, Cu seed could be attacked by  $\mathrm{H}+$   ions if the current is  not sufficient to protect the seed layer, which in turn induced  the void formation.

![V3/M3   V2/M2  V1/M1   CA/PC  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bef02427-4504-4a60-ae2f-eded490cea2a/bef02427-4504-4a60-ae2f-eded490cea2a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=0fc54ff02678aba81a416c64f4bbb2efd7bbbadb)
Fig. 9 . Typical GDS layout of SRAM device.

![TEN   STEM  CD measurements onV2 is not available  V2  V1  CD  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a8740aab-3e3c-4ffc-ba03-40f040977c32/a8740aab-3e3c-4ffc-ba03-40f040977c32.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=5707256cada90c5bf798dc18ab7e33bff228a554)
Fig. 10 . TEM & STEM images of the sample prepared at V2 level.

![. Laser deprocessed areas reach  1.At V3/M3 level, accurate bit-   V1/M1 level,inwhich BLs andWs  counting cannot be performed.   counting can be performed.  V1/M1  V3/M3   V3/M3  V1/M1  V3/M3TargetBLs  TargetWLs  TEM direc  Ill. Target 3-bit cluster is Pt marked  at V3/M3 level forTEM analysis    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ee0a22e4-4a45-4e33-9a6d-b06fb41de91d/ee0a22e4-4a45-4e33-9a6d-b06fb41de91d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=25dbb3081fb8b58cd2fa81d0e3932ed827d9d91a)
Fig. 11 . Schematic of LDT application steps. Solution for the memory bit-counting at M3 level in the SRAM device.

![W2  2  Defect  1  C  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0298a3b2-56ef-4f5a-a8a3-4f85d33ea925/0298a3b2-56ef-4f5a-a8a3-4f85d33ea925.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=2fed649a59ef214e7117b676bc8a448bf94739ae)
Fig. 12 . TEM images of the failed 3-bits cluster. Zoom-in images for CD  measurements and defect inspection.

![STEM   a  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/eb9c9b6a-930c-407a-99a1-09a7a4263740/eb9c9b6a-930c-407a-99a1-09a7a4263740.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=ddadf5f21f84ad46dbde87624c1b6f0a86553a68)
Fig. 13 . STEM micrograph with EDX quant maps on the defect area. Obvious  Cu void is observed in the Cu map.

## IV. C ONCLUSION 

In this paper, laser deprocessing technique (LDT) is  successfully applied into PFA on SRAM and NVM memory  bit-counting. Compared to the conventional bit-counting  methods, this LDT assisted new method is more cost-effective  and efficient in terms of shrinking down the total FA time cycle  and lowering the requirements for the experimental equipment,  which leads to the increase of PFA throughput in memory  devices especially for high technology nodes. Furthermore, this  method only requires basic FA skills including SEM and OM  inspection so is easy to be manipulated even for engineers at the  beginner level.

## R EFERENCES 

[1]    Y. Z. Zhao, Q. J. Wang, P. K. Tan, H. H. Yap, B. H. Liu, H. Feng, H. Tan,  R. He, Y. M. Huang, D. D. Wang, L. Zhu, C. Q. Chen, F. Rivai, J. Lam,  and Z. H. Mai, "Application of Fast Laser Deprocessing Techniques on  Large Cross-section View Area Sample with FIB-SEM dual beam  system" Microelectronics Reliability, Vol 64, pp.362-366, 2016.    [2]    H. H. Yap, P. K. Tan, L. Zhu, H. Feng, Y. Z. Zhao, R. He, H. Tan, B. H.  Liu, Y. M. Huang, D. D. Wang, J. Lam, and Z. H. Mai, "Application of  Laser Deprocessing Technique in PFA on Chemical Over-etched on  Bond-pad Issue" Microelectronics Reliability, Vol 64, pp.357-361, 2016.    [3]    H. H. Yap, P. K. Tan, J. Lam, T. H. Ng, G. R. Low, R. He, H. Feng, Y. Z.  Zhao, M. K. Dawood, H. Tan, B. H. Liu, Y. M. Huang, D. D. Wang, and Z.

H. Mai, "Application of Laser Deprocessing Techniques in Physical  Failure Analysis" ISTFA 2013: Proceedings from the 39th International  Symposium for Testing and Failure Analysis, pp. 563-568, 2013.

[4]    H. H. Yap, P. K. Tan, G. R. Low, M. K. Dawood, H. Feng, Y. Z. Zhao, R.  He, H. Tan, Y. M. Huang, D. D. Wang, Y. Zhou, P. S. Limin, S. James, J.  Lam, and Z. H. Mai, "Application of Fast Laser Deprocessing Techniques  in Physical Failure Analysis on SRAM Memory of Advanced  Technology" ISTFA 2014: Proceedings from the 40th International  Symposium for Testing and Failure Analysis, pp. 277-282, 2014.

