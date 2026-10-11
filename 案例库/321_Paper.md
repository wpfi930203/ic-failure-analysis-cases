---
title: "321_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_24d0351a56e736ec8a835bf0ca069be37295230462135641
file_size: 2400234
---

## Application of EBIC and EBAC for Nanoscale Fault  Isolation of FEOL Defect  

F. Rivai, P.T. Ng , Y.Z. Ma, A.C.T. Quah, N.Y. Xu, J.C. Alag, C.Q. Chen  GLOBALFOUNDRIES Pte Ltd  60 Woodlands Industrial Park D Street 2, Singapore 738406  Fransiscus.rivai@globalfoundries.com

Abstract-   The advancement of semiconductor integrated circuit  technology demands for nanoscale fault localization techniques to  pinpoint the defect location. This is especially critical for subtle  front-end of line defects which are easily destroyed from  conventional top-down physical delayering or cross-section FIB  and would require precise TEM to visualize the defects. In this  paper, 3 case studies of nanoscale fault isolation were  demonstrated using EBAC/EBIC method to localize the weak  point of an ESD implanted clamp transistor design, to isolate the  defect that resulted in erase failure in an embedded NVM device  and to pinpoint the defect that caused high dark current in PIN  SiGe photodiode.

Keywords  –  EBIC, EBAC, Nanoprobing, Nanoscale, Fault  Isolation, Failure Analysis

## I. I NTRODUCTION 

With the continuous advancement of semiconductor  integrated circuit technology, fault isolation has become more  challenging, especially for subtle Frontend-of-line (FEOL)  defects.   Conventional   laser   induced   techniques   like  TIVA/OBIRCH and Photon Emission Microscopy (PEM) lack  resolution to sufficiently localize these defects. Therefore  nanoscale fault isolation techniques like EBAC (Electron Beam  Absorbed Current) and EBIC (Electron Beam Induced Current)  are required to increase the success rate of defect viewing at  subsequent TEM analysis. While EBAC has been widely  utilized to reveal open and short in backend-of-line metal  routings [1] and gate oxide breakdowns [2], EBIC is used to  localize junction anomalies and transistors related defects [3].

Although the tool operations for EBAC/EBIC are not  complicated, there are various biasing or setup combinations  that are more effective for different type of defects than others.  This might be due to different signal interference and response  from different structure. Some of things to be considered are the  probing layer, the suspected defect layer, the leakage level  (hard short or minor junction leakage), and the structured to be  probed. For instance, using high kV e-beam when probing near  the RX layer without properly grounding the connected  junction may cause a lot of unwanted EBIC signal from the  surrounding RX structure. However, grounding the wrong  junction connection may prevent the actual defect signal to  show up.

In this paper, 3 different case studies that utilized  EBAC/EBIC for nanoscale fault isolation on different FEOL

structures were discussed. Different setups and biasing  conditions were employed to achieve successful defect  localization. Transmission Electron Microscopy (TEM) results  of each defect will also be presented for root cause  understanding.

II.   C ASE  S TUDY  1:   EBAC   F AULT  I SOLATION FOR  M EMORY  B LOCK  E RASE  F AILURE

This case study described the usage of EBAC to localize  subtle residue defect between control gate and erase gate of a  NVM block that suffered from erase failure. Fig. 1 showed the  layout of the NVM cells where the erase (EG), control (CG) and  select (SG) gates were running in parallel across the bit lines.  While the CG and SG were shared among 4864 bits, the erase  gate was divided into segments and each gate segment was  shared among 32 bits.

![  BL0   BL1   BL2   BL30   BL31   BL32  BL33  BL34   BL62BL63  SGPoly  CGPolv  EGPoly   EGPoly  CGPoly  SGPoIy  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b59a18c9-1391-4c96-b734-4fc23b2dc071/b59a18c9-1391-4c96-b734-4fc23b2dc071.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=35bde002b68c143d405e5b3d66ac500774cecc1f)
Fig. 1 NVM EG, CG, and SG poly arrangement

Test debug could localize to the failing EG segment but could  not narrow down to the failure bit for direct TEM analysis.  Thus, further nanoscale fault isolation was still critical to  identify the precise failing location. The sample was  de-processed to via 1/metal 1 to check that there was no  backend-of-line short before delayering to contact level for  further analysis. Fig. 2 is the SEM image of the contact level  passive voltage contrast (PVC) analysis which showed an  abnormal bright contact at the failing EG.

![Abnormalbright  PVCpolyCA  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b3b9b013-a74e-448b-aa70-956769ed8f8c/b3b9b013-a74e-448b-aa70-956769ed8f8c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=5ffd769fd780299d5560f3eb68691d2cd5d17dc2)
Fig. 2 SEM image PVC at contact level

Nanoprobing measurement result indeed observed a short  between the EG and CG as shown in Fig 3. EBAC was  performed with single current sensing probe on the failing EG.  Fig. 4 showed that the EBAC signals from the EG and the  shorted CG were clearly observed. In additional, an anomalous  EBAC signal with stronger contrast (circled in red) was also  revealed along the segment where the EG and CG were running  side by side. With this finding, TEM sample preparation was  able to precisely mill to the defect location and revealed the  silicide poly residue causing the EG-CG short as shown in Fig.  5

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ef52efbf-d45c-4f55-84c2-a21ec5e0b293/ef52efbf-d45c-4f55-84c2-a21ec5e0b293.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=38400f9c415bb86c265f41028ed7f2a327c5bfe3)
Fig. 3 I-V measurement of bad (shorted) EG vs CG

![Bad   Ref  Anomaly    a  (a)   (b)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/157e1334-9c14-4c6a-8f97-d7b7081ed697/157e1334-9c14-4c6a-8f97-d7b7081ed697.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=ad1a4d5445048ed72e646fb45430a274d43b9346)
Fig. 4 EBAC signal of (a) the shorted EG and CG and (b) reference EG

![NiSi Residue  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2a9a5669-7e11-4474-b927-8cb3df0f3ca4/2a9a5669-7e11-4474-b927-8cb3df0f3ca4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=08938de8d065cfc1706d87efe424be8819ae7223)
Fig. 5 TEM image of NiSi poly residue which shorting bad EG and CG

III.   C ASE  S TUDY  2:   T WO  P ROBE  EBIC   A NALYSIS ON  ESDNFET

In this case study, a 5V ESD implanted GGNMOS transistor  was subjected to transmission-line pulse (TLP) with increasing  current, until a transient I off  leakage was observed, to  understand the design weak point of the ESD clamp transistor  [4]. The cross-section view of the GGNMOS with additional  ESD implant (shaded in yellow) was shown in Fig. 6. Global  fault isolation with PEM observed a distinctive emission spot  on the failed structure as shown in Fig 7(a). Fig 7(b) showed  emission spot overlaid on the layout. It seemed to indicate that  the hotspot was falling at the poly corner. However, without a  precise TEM to reveal the actual defect, the design weakness  was uncertain for the understanding of the failure mechanism  and process optimization.

![Body  Source   Poly  Drain  SAB  Pvv  DN  PSUB  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d87e9454-9c8a-47d7-bbca-df72e21cc863/d87e9454-9c8a-47d7-bbca-df72e21cc863.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=a06748a652427d3b694927063350fdf8a73c4ba6)
Fig. 6 Cross-section view of the GGNMOS with additional ESD implant

![active    (a)   b  (b)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b6766863-98ce-4318-8028-8ccb1fe1ec6b/b6766863-98ce-4318-8028-8ccb1fe1ec6b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=4446455715092d8bb3c79417d45a5de4aea5d79c)
Fig. 7 (a) PEM overlay image showing weak emission and (b) SEM image  showing minor metal void at emission spot.

Physical delayering was performed to polish the sample to  contact level with subsequent nanoprobing to measure the  Drain – Well leakages of the 1st three drain fingers as shown in  Fig 8(a). The 1st drain finger, where the hotspot fell along,  revealed higher leakage  $\mathrm{\sim0.6uA}$   at 5V in Fig. 8(b) as compared  to the neighboring reference drain fingers   $(<20\mathsf{p A})$  . High KV  SEM inspection could not observe any anomaly. A  cross-section FIB could be performed at the approximate  hotspot location to observe the defect for TEM. However, with  such a low level leakage, the defect was expected to be minute  and the typical progressive FIB approach would have a high  probability of missing the defect.

![1stdrain  Ref1Ref2  finger   1.0E-06  Bad  8.0E-07   Ref1  Ref2  5.0E-07  4.0E-07  2.0E-07  D.OE+O  VD（V)    a  (a)   b）  (b)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/664da223-eb8b-4090-bf2c-409c571a31fd/664da223-eb8b-4090-bf2c-409c571a31fd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=f9fa030b9cb68e9ce4f944553fcfe1e8ce15cf3e)
Fig. 8 (a) SEM image of the measured bad and reference transistors and (b) I-V  measurement comparison between bad and reference transistors

Thus, EBIC analysis was employed in attempt to localize the  defective weak point with higher resolution. Single probe EBIC  at the leaky 1st drain with sample stage grounded could not  observe any anomaly. However, with additional grounding  probe at the P-well, a weak distorted EBIC signal at drain-well  junction was observed at the poly corner as shown in Fig. 9(a)  and Fig. 9(b). This anomalous signal coincided with the  emission spot location and thus pinpointed to the defect  location. Subsequent TEM analysis revealed damage active at  the poly-to-ESD implant spacing as shown in Fig. 10. The  location of the damage validated the hypothesis of current  crowding at the poly-to-ESD region due to parasitic  N+/P-Well/N+ shallow surface conduction path indicated by  the red lines in Fig. 6. This result suggested to the Fab that  process optimization of poly-to-ESD spacing was critical in  improving the ESD performance of the clamp design.

## IV.   C ASE  S TUDY  3:   T WO  P ROBES  B IASED  EBIC   A NALYSIS FOR  P HOTODIODE  H IGH  D ARK  C URRENT  F AIL   

In the third case study, a vertical PIN SiGe photodiode  structure that experienced high dark current was analyzed. Pad  level benching results in Fig. 12 showed very high dark current  on bad unit as compared to good unit, and a localized emission  spot was observed at 4V reverse biased as shown in Fig. 13.  PFA was performed but found no anomaly until CA layer.  Progressive X-FIB could be done around the emission spot  location to check for any abnormalities in the FEOL, however it  was difficult to accurately target the defect location from the  low resolution emission spot image.

![8.00E-06  6.00E-06  4.00E-06  2.00E-06  0.00E+00  1.5-2.00   O.5   1.5   2.5   3.5   4.5   -Ref  -4.00E-06   Bad1  -6.00E-06  -8.00E-06  -1.00E-0  -1.20E-05  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/33377d30-47dd-4e5c-85b0-fdb923cbc3ca/33377d30-47dd-4e5c-85b0-fdb923cbc3ca.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=291273c2a1b7b5e42809d3968dc04ee4760ffeac)
Fig. 12 Pad level I-V measurement on bad and reference unit

![Bad  Bad  Ref  Ref 00000000009000    (a)   (b)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a6ba5918-d1df-40f2-8dda-b3fca7553c8b/a6ba5918-d1df-40f2-8dda-b3fca7553c8b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=f35ba83fca342d68708e3044df7f431fb48abdd7)
Fig. 9 Single probe EBIC signal with additional grounding probe of (a) bad and  (b) reference structure

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4c577577-785a-49c6-bf3f-d039fd3b6459/4c577577-785a-49c6-bf3f-d039fd3b6459.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=218f481841a35f1ff40950856c3823649780bbbf)
Fig. 10 Damage active at the poly-to-ESD implant spacing

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/768ace4f-f39e-43da-8983-753ae1d4e827/768ace4f-f39e-43da-8983-753ae1d4e827.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=c726ebd63ec66b75e88ea472f78d2f378244173a)
Fig. 13 Localized emission spot at 4V reverse biased on the bad photodiode  structure

Subsequently, two probes EBIC analysis with voltage biased  was carried out in an attempt to pinpoint the defect location.  Initially, when zero bias was applied and EBIC signal  highlighted the entire diode junction with no indication of the  weakness as shown in Fig. 14.

![5KV0V  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f3b02089-b993-4e20-a6c3-c42a8781bc10/f3b02089-b993-4e20-a6c3-c42a8781bc10.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=2be3229672431c56c7f3be8bf445aeff3cbd811f)
Fig. 14 Non-biased EBIC signal on the bad photodiode structure

By slowly increasing the biasing voltage from 0.4V to 5V  while landing two probe at P and N contacts, a localized EBIC  signal spot started to show up at 4V bias and became more  distinctive at 5V bias as shown in Fig. 15.

![5KV0.4V   5KV2V   5KV3V  5KV4V   5KV5V   5KV5V  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3db407ab-5a4b-4772-af04-ea717ef2f167/3db407ab-5a4b-4772-af04-ea717ef2f167.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=b5f38412dce9922126332833d248e4e776243c22)
Fig. 15 EBIC signal on the bad photodiode structure with increasing biased  voltage

By using the higher magnification image to pin point the  possible defect location, a TEM cross-section cut was  performed. TEM result observed large Ge crystal anomaly near  the Ge-Si bottom boundary as circled in Fig. 16. This Ge crystal  defect could act as the electron-hole pair recombination center  which induced the dark current leakage in the bad photodiode  structure.

![Bad   Ref  AnomalyinGe  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/656f9552-0b87-485e-9166-0cbe71b32434/656f9552-0b87-485e-9166-0cbe71b32434.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=c988f26af2a6901de0d658a47728359beee881c0)
Fig. 16 Ge crystal anomaly in Ge-Si bottom boundary at the anomalous spot  location

## V. C ONCLUSION 

In conclusion, the 3 studies have illustrated how important  EBAC/EBIC techniques are in the Failure Analysis process, to  pinpoint the exact defect location with nanoscale resolution.  They also illustrated the need to always experiment with  different biasing approaches to achieve optimal nanoscale  defect localization sensitivity.

## A CKNOWLEDGMENT 

We would like to thank Globalfoundries Singapore EFA and  TEM team, especially all the engineers who are directly  involved, for their continuous support on all these cases.

## R EFERENCES 

[1]    P. Larre, Mr & H. Tupin, Ms & C. Charles, Mr & R. H. Newton, Mr &  Reverdy, Antoine, “Precise Localization of 28nm Via Chain Resistive  Defect Using EBAC and Nanoprobing,”  in ISTFA. , pp. 67-70, November   2012.     [2]    P. K. Tan et. al, “Nanoprobing EBAC technique to reveal the failure root  cause of gate oxide reliability issues of an IC process,”  in IIRW. , pp.  10-15, October 2014.     [3]    W. P. Lin, H. J. Chang, “Physical failure analysis cases by Electron Beam  Absorbed Current & Electron Beam Induced Current detection on  nano-probing SEM system,”  in IPFA. , July 2010.    [4]    P. Mahajan, S. Suresh, A.C.T Quah, F. Rivai, R. Jain, U. Singh, R.  Gauthier, K. J. Hwang, “Robust ESD Implanted 5V GGNMOS Clamp  Design and Process Optimazation with Maximized ESD Design  Window,”  in EDT.,  March 2019.

