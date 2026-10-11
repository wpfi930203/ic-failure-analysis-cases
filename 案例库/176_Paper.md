---
title: "176_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_e9d61859b67f67dda7974470c52c71377295230462135641
file_size: 762904
---

## Backside and Topside OBIRCH Defect Localization  on Multi-layer Finger Structure MOSFET Capacitor  with the aid of Focused Ion Beam (FIB)  

Ronald C. Apolinaria  1 , Febus Reidj G. Cruz  2 , and Flordeliza L. Valiente  3   1 Failure Analysis - Maxim Integrated, Gateway Business Park, General Trias, Cavite, Philippines.  2, 3 School of Electrical, Electronics, and Computer Engineering, Mapua University, Manila, Philippines.   1 Phone: +632 902 2000 local 2396; Email: Ronald.Apolinaria@maximintegrated.com;

Abstract-   Fault localization using backside OBIRCH (Optical  Beam Induced Resistance Change) on metal finger structures is  not always effective, especially when the Integrated Circuit (IC)  device is composed of multiple metal layers and the defect is  located on the mid or upper metal lines. The use of both backside  and topside OBIRCH techniques is a known effective approach  that increases the success rate in determining the failure  mechanism for these cases. However, fault isolation systems are  either configured for backside or topside method only. In the  Maxim Integrated Philippines Failure Analysis laboratory, only  the backside OBIRCH system is available. Thus, defect  localization on faulty internal nodes becomes a challenge when  only one type of fault isolation system configuration is available.  This study presents a new method by doing FIB (Focused Ion  Beam) circuit edit to enable topside OBIRCH using the available  backside-configured OBIRCH system. The new method was  found to be an effective alternative in resolving particle-related  problem on multi-layer finger metal structure MOSFET  capacitor.

Keywords  –  MOSFET, FIB, Topside, Backside, OBIRCH,  Finger metal structure.

## I.  I NTRODUCTION 

With the advancement of semiconductor technology, IC  feature sizes continue to shrink, and more transistors are being  integrated in the same chip area. Consequently, the difficulty of  failure localization increases. A failure point is more likely to  be buried and could no longer observed directly on the die  surface [1]. In addition, smaller metal line widths and additional  metal layers reduce the effectiveness of sole reliance on topside  or backside fault localization [2]. To locate a failure point  within a five or six metal layer stack is extremely difficult  without an effective, precise positioning technology. Precise  positioning can provide correct analysis direction for  subsequent physical analysis. Thus, the defect localization  technology is particularly important, especially for analysis of  the defects in dense metallization [1].

Owing to high efficiency and resolution, OBIRCH is widely  used in FA labs worldwide. OBIRCH is a laser induced defect  localization technique, where the laser stimulation causes a  resistance change through localized heating of the underlying  circuit. An abnormal current change corresponds to the heating  on the site of a potential defect. OBIRCH has been used

successfully to locate resistive and open/short metallization  defects [1].

Two previous FA cases with failures located in MOSFET  capacitors were used for illustration. In the two cases, the  defective capacitor was isolated by employing photon emission  analysis and micro-probing. Once the failure site was isolated,  backside OBIRCH was performed by biasing the leaky internal  nodes through probe pad test points deposited using Focused  Ion Beam (FIB). An OBIRCH image was acquired of the region  within the defective capacitor as shown on Fig. 1.1. However,  physical analysis with deprocessing and FIB cross section did  not reveal the defect that caused the unit to fail.

![(a)   (b)    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e6cebc30-3851-485b-9073-9d85a01f6064/e6cebc30-3851-485b-9073-9d85a01f6064.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215639%3B1743219239&q-key-time=1743215639%3B1743219239&q-header-list=host&q-url-param-list=&q-signature=68b55afaba0243b2195e10117c38f776bc532609)
Fig. 1.1 (a) and (b) Previous FA cases showing backside OBIRCH signal on  defective MOSFET capacitor.

In both cases, only backside OBIRCH equipment was  available at the time of analysis, so only the backside method  could be employed during fault localization. To overcome the  limitation, a method was developed to perform both backside  and topside OBIRCH using equipment designed for only  topside or bottom side.  The new method re-routes metal lines  of faulty internal nodes to the nearest metals that were directly  connected to the package external pins. This would require FIB  circuit edit for connecting several metal lines. The method  allows the topside OBIRCH method to localize defects within a  faulty MOSFET capacitor with finger metal structures using a  backside OBIRCH system.  The new technique is valuable  because finger metal structures have been used in more and  more IC design for its high density and simplicity to  manufacture as shown on Fig. 1.2 [4].

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1126e736-589f-4d19-a833-690e87ce62d9/1126e736-589f-4d19-a833-690e87ce62d9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215639%3B1743219239&q-key-time=1743215639%3B1743219239&q-header-list=host&q-url-param-list=&q-signature=46fe1fa609d72911575580eca575e0c99d39de5c)
Fig. 1.2 Finger metal structure model.

Specifically, the study aimed: (a) to create a method to do  topside OBIRCH while utilizing backside OBIRCH system and  (b) eliminate unknown FA case with defective MOSFET  capacitor.

By successfully locating the failure mechanism, the quality  of the process and product was improved.  Completing root  cause analysis and corrective action implementation were  critical in this effort and depend on resolving all FA cases  successfully. The case studies presented on this paper involve  customer return devices with a six-metal layer structure.

## II.   R EVIEW OF  R ELATED  L ITERATURE 

The OBIRCH analysis technique scans a laser across a die or  partial area of a die. The scanning laser creates localized  heating and causes resistance change in some defects. The  defect location is determined by monitoring for resistance  changes in the underlying circuit. OBIRCH provides good  solution for locating issues such as metal defects [8]. When the  input voltage is fixed, the current through an interconnect line is  altered and heat induced by scanning the laser causes a change  in resistance [5]. The principle of detecting a current change  (ΔI) at the location exposed to the laser is illustrated in Fig. 1.3.

![PRINCIPLEOFOBIRCHANALYSIS  Laser : =1.3 μm   Laser (frontside)   Leakage CurrentPath  A1  Heated   (△R/V1  Si-sub  α △T, TCR  Laser(backside)  Dependsondefects andmaterials  △V=△RxI  I : Current before laser irradiation  Defects in Metal Line  V : Voltage change due to laser rradiation (when constant current is applied) -  R : Resistance increase with the temperature increase due to laser irradiation  T : Temperature increase due to laser irradiation  TCR:Tem   fficientofresistance  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/af9e96b6-a359-46ff-8f24-af7f146ea109/af9e96b6-a359-46ff-8f24-af7f146ea109.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215639%3B1743219239&q-key-time=1743215639%3B1743219239&q-header-list=host&q-url-param-list=&q-signature=adfe8bec934fff7ef091dbe99f82a9f881537028)
Fig 1.3 Principle of OBIRCH Analysis.

FIB is also a useful tool for IC failure analysis. A FIB system  functions similarly to other focused electron beam systems such  as scanning electron microscope or transmission electron

microscope. However, instead of electrons being directed  towards the sample, the FIB system uses a beam of ions.  The  FIB ion beam interacts with the sample to cause a continuous  milling process during beam exposure. The milling process  occurs as an atomic collision process, and the milling rate is  proportional to the beam current.  Material removal increases  with the higher beam currents. Milling is the most powerful  capability of a FIB and is directly related to the choice of ion, its  energy range and the momentum of the particle [6].

During the  $16^{\mathrm{th}}$   IPFA 2009, a study was presented entitled “A  study of combining FIB circuit edit and OBIRCH technology  for failure analysis”. The paper discussed combining focused  ion beam (FIB) circuit edit with OBIRCH analysis. FIB can cut  or rewire an integrated circuit while OBIRCH can locate the  failure location. By applying FIB circuit edit and OBIRCH at  the same time, failure site was isolated and the root cause of the  failure was determined [6].

A study on Topside Defect Localization using OBIRCH  Analysis was presented during the 31st ISTFA proceedings  2005. The study showed that OBIRCH analysis can effectively  identify the defect once the failing signal is located and  characterized. It can be very useful when the signal in question  have long routes. As technologies become more complex with  many metal layers and computer-generated routing of signals,  the isolation technique becomes more important. It was noted  that OBIRCH analysis has become a valuable tool for defect  localization; however, it cannot be used in all cases.  Nevertheless, the study on OBIRCH analysis has helped  improve success rate and decrease analysis cycle time [7].

Another study entitled “Voltage choosing of OBIRCH for  finger metal structure” was presented on the 23rd IPFA 2016.  The study noted that OBIRCH amplification depends on the  resistance and the voltage bias; hence, choosing the proper  voltage was important. Proper voltage of OBIRCH used to the  finger metal structure. Cases showed proper voltage arose while  the sigma had the maximum value. It was provided that the  method is effective to choose a correct voltage for the working  of OBIRCH. OBIRCH is the useful tool for detecting failures  under a direct power condition [4].

Lastly, the current common practice in the industry is to use  both fault isolation systems configured for backside and topside  method to perform backside and topside OBIRCH techniques in  FA cases dealing with internal faulty nodes.

## III. R ESULTS AND DISCUSSION 

A methodical approach in achieving the desired results of the  study is presented in this section.

![Is there any    Perform basic FA steps  FIB circuit edit   return unit with   up to Layout and  characterization   suspected ca-   Hes   Schematic Review  pacitor issue  Start  Is it related to  OBIRCH signal analy-   failing MOSFET  sis, deprocessing, FIB   capacitor  cross section,Report   Emd  Generation  res  FIB probe pad deposition,  Electrical characterization  Is OBIRCH   Vary bias volt-signal on ca-   age and LASER   pacitor visible   parameter    backside OBIRCH  Vary LASER pa-rameter, change site   Is there any   positioning  valid OBIRCH  signal within  Layout and Schemat-   capacitor  topside OBIRCH   ic Review, FIB probe  pad circuit edit  Yres  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1c97a5d9-0046-4864-9486-2dd109d98af1/1c97a5d9-0046-4864-9486-2dd109d98af1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215639%3B1743219239&q-key-time=1743215639%3B1743219239&q-header-list=host&q-url-param-list=&q-signature=64bd84afe96f8fd59f2751502f68bae3b2d41958)
Fig. 3.1 Case Study Flow Chart.

In the first step, FIB circuit edit characterization was  performed. Since the proposed OBIRCH topside method  utilized the available backside system, circuit edit was needed  to connect the failing internal nodes to the package external  pins as illustrated in Fig. 3.2. However, characterization was  performed since the FIB deposited metals would behave as if it  is a metal defect and could produce false OBIRCH signal  during fault isolation. The characterization aimed to determine  the least OBIRCH signal intensity that was produced by  varying the deposited metal width and LASER power from   $30\%$   to   $50\%$  .

![Defective  Defective  Node  Node  Connected to  Connectedto  package  package  external pin  external pin  FIB Circuit  FIB Circui  Edit  Edit    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/96e6b0d1-dbe3-426b-bf39-4fd99fe23569/96e6b0d1-dbe3-426b-bf39-4fd99fe23569.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215639%3B1743219239&q-key-time=1743215639%3B1743219239&q-header-list=host&q-url-param-list=&q-signature=e5badd9ddc68e6573de5e5a4e0c7990952cedc97)
Fig. 3.2 FIB Circuit Edit Sample

The device under test (DUT) that was analyzed is dependent  to the returned unit/s from field. The failing unit undergone the  normal FA process such as non-destructive analysis, fault  isolation and circuit analysis using layout and schematic review.  Different types of defect such as faulty MOSFET capacitor can  be deduced based on the emission pattern from photon emission

analysis. Probe pad deposition was performed on suspected  faulty internal nodes in preparation for further electrical  characterization using parametric analyzer and then followed  by backside OBIRCH analysis.

Once the OBIRCH signal was observed within the suspected  faulty MOSFET capacitor, further layout and schematic review  were required to check the adjacent metal structures that are  directly connected to the package external pins. Then, FIB  probe pad circuit edit followed to reroute the leaky internal  nodes to the package outside pins. Topside OBIRCH was  performed while parameters such as LASER power and  position of the scanned portion of the die were varied to obtain  the expected OBIRCH signal on the area of interest.

Once both backside and topside OBIRCH results were  available, further OBIRCH analysis was done to better  understand the location of the defect within the multi-layer  metal finger structure. It was helpful to identify the correct cut  starting point and direction. Deprocessing was performed prior  to FIB cross-section such that the large metal layers on top of  the finger structures were removed.

## IV. R ESULT AND  D ISCUSSION 

Table 4.1 shows the FIB circuit edit characterization results  by varying the metal width and LASER power. Results showed  that the OBIRCH signal intensity was reduced with increasing  metal width. Moreover, LASER power did not have significant  effect on the OBIRCH signal intensity.

||Metal Width|Metal Width|Metal Width|
|---|---|---|---|
|LASER power|1.75um|3.51um|4.82um|
|30%||||
|35%||||
|40%||||
|45%||||
|50%||||


Several failure analysis techniques such as photon emission  analysis and micro-probe were performed to determine the

defective capacitor. Internal nodes regamp and vss were  electrically characterized using parametric analyzer and found  to have a resistive short as shown on Table 4.2 and 4.3. The  proper voltage bias used for OBIRCH was identified through  the data collected using parametric analyzer to achieve a good  OBIRCH amplification [6].

![Table 4.2. Case 1 REGAMP to VSS/GND I/V Curve  Table4.2.Case1REGAMPtoVSS/GNDI/VCurve  Correlation Unit  Correlation Unit   DUT  DUT      Table 4.3.Case 2 REGAMP toVSS/GNDI/V Curve  Table 4.3. Case 2 REGAMP to VSS/GND I/V Curve  Correlation Unit  Correlation Unit   DUT  DUT    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/aae1d710-9ab4-4f66-84bd-59ded4121609/aae1d710-9ab4-4f66-84bd-59ded4121609.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215639%3B1743219239&q-key-time=1743215639%3B1743219239&q-header-list=host&q-url-param-list=&q-signature=7b9eef468c65c65fe37dfad578db50bc7cce9f51)
Since the failing signal was isolated on a certain node,  backside OBIRCH was performed by biasing the leaky internal  path through probe pad test points deposited using Focused Ion  Beam (FIB). The faulty internal nodes were biased under  constant voltage. The positive supply was connected to the  regamp and the negative supply was connected to vss. An  OBIRCH image was acquired lying within the defective  capacitor as shown on Fig. 4.1 (a) and 4.2 (a).

observed within the defective capacitor as shown on Fig. 4.1 (b)  and 4.2 (b). In case study 1, the location of topside OBIRCH  signal coincided with the backside signal location (See Fig. 4.1  (c)). The topside signal was weak, indicating that the defect was  located on lower metal layer. In case study 2, by superimposing  the backside and topside images as shown on Fig. 4.2 (c),  topside OBIRCH signal had a significant offset with respect to  the backside OBIRCH signal.

![(a)  （a)  (b)  (c)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/26708f72-61b0-477f-8689-6c108044d04e/26708f72-61b0-477f-8689-6c108044d04e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215639%3B1743219239&q-key-time=1743215639%3B1743219239&q-header-list=host&q-url-param-list=&q-signature=e0920611fd0d32b663d66788b4cf084af97a14f8)
Fig. 4.1 Case 1 (a) Backside OBIRCH (b) Topside OBIRCH (c)  Superimposed Backside and Topside OBIRCH images.

![(a)  a1    (b)    (c)  C  Validba  OBIR  Validtopside  BIRCH  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a3ceb7f8-7253-40f1-ae56-657845deff73/a3ceb7f8-7253-40f1-ae56-657845deff73.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215639%3B1743219239&q-key-time=1743215639%3B1743219239&q-header-list=host&q-url-param-list=&q-signature=1e3a1c48dd295257657d5774e651c22f9d1eb783)
Fig. 4.2 Case 2 (a) Backside OBIRCH and (b) Topside OBIRCH (c)  Superimposed Backside and Topside OBIRCH images.

As laser imaging did not observe any anomaly at the spot  location for both cases, deprocessing was performed to expose  the metal finger structure at metal 4.

Since the defect was localized, FIB cross-section was  performed instead of doing physical deprocessing techniques  until an anomaly is observed. This was an advantage because  physical deprocessing can be very iterative and time  consuming. On the other hand, FIB cross-sections can be  performed much faster. The time advantage of FIB  cross-sectioning versus top down deprocessing is magnified  with more complex technologies that have more metal layers  and FIB cross-section provides better defect detail. In the case  of a wafer fabrication defect, FIB cross-section can be helpful  in pinpointing the process step where the defect originated.

Topside OBIRCH analysis was performed after the units  were subjected to FIB circuit edit. OBIRCH signal was still

FIB cross section analysis confirmed the presence of metal  defect bridging the metal lines connected to regamp and vss.  The defect structure was primarily composed of Titanium (Ti)

material as verified during Energy Dispersive X-ray (EDX)  analysis.

![(a)  CaD  (b)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1d73c6dc-4fb4-4184-82ae-07293ef6367b/1d73c6dc-4fb4-4184-82ae-07293ef6367b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215639%3B1743219239&q-key-time=1743215639%3B1743219239&q-header-list=host&q-url-param-list=&q-signature=253ee1c23aaf36ee375ab6847490eaed671f7a96)
Fig. 4.3 (a) Case 1 and (b) Case 2 FIB Cross Section Results.

## A CKNOWLEDGMENT 

The author would like to acknowledge Ma. Rozelle  Velasquez and Jonelle Mananguit for the FIB support. The  author would also like to thank Em Julius Dela Cruz, Tejinder  Gandhi and Maxim MPOC FA ECBU for analysis  brainstorming.

## R EFERENCES 

In case study 2, the defect was found on the location pointed  by topside OBIRCH. It illustrates an important point that if a  cross-section was performed when the backside OBIRCH site  was identified, the defect may never have been found.

[1]    Xiaoling Lin and Hongqi Zhang, “OBIRCH Based on Differential  Imaging Locating method”,  2014 10th International Conference on  Reliability, Maintainability and Safety (ICRMS) , pp. 270-274, August  6-8, 2014.     [2]    Li Tian, Guoqiang Zhang, Kuibo Lan, Gaojie Wen and Dong Wang,  “Application study of simply and low cost numerical aperture increasing  lens (NAIL) system for OBIRCH and EMMI in backside failure  analysis”,  22nd IPFA , pp. 531-534, July 6-10, 2015.     [3]    R Clegg, et al., “Engineering Failure Analysis”,  Volume 82 , December  2017, pp 1-862, 2017.    [4]    LinMeng Yang, Bobby Chan, Gang Qian, LiLung Lai and Rui Fang,  “Voltage choosing of OBIRCH for finger metal structure”,  23rd IPFA  2016 , pp. 1-4, July 18-21, 2016.     [5]    https://www.hamamatsu.com/resources/pdf/sys/SSMS0019E_iPHEMOS s.pdf.    [6]    JingLin Yan, Xuesen Liu, Mike Liu and YiLing Liu, "A Study of  Combining FIB Circuit Edit and OBIRCH Technology for Failure  Analysis",  IPFA 2009 IEEE 16th International Symposium , pp. 545-548,  July 2009.     [7]    Clifford Howard, Anusha Weerakoon, Diana Mitro and Dawn Glaeser, "  Topside Defect Localization Using OBIRCH Analysis",   IEEE  proceedings 31st International Symposium for Testing and Failure  Analysis (ISTFA) , November 6-10, 2005.    [8]    K. Nikawa, and S. Inoue, " New capabilities of OBIRCH method for fault  localization and defect detection",  6th Asian Test Symposium , pp.  214-219, November 17-19, 1997.

## V. C ONCLUSION 

A method of doing topside OBIRCH using backside system  was demonstrated to be effective as presented in the case  studies. In case study 1, the defect was found coincident to the  topside and backside OBIRCH signal location. However, in  case study 2, topside OBIRCH signal had significant offset with  respect to backside OBIRCH. During physical analysis, the  defect was found on the area pointed by topside OBIRCH at  metal layer 4. The outcome in case 2 illustrates an important  point that if a cross-section was performed when the backside  OBIRCH site was identified, the defect may never have been  found. Combining backside and topside OBIRCH method was  found to be effective in localizing the fault on finger metal  structure of MOSFET capacitor. Indeed, the study was  successful in eliminating unknown FA case related to MOSFET  capacitor failure.

## R ECOMMENDATION 

For further studies, it is recommended to simulate the defect  between regamp to vss for FIB circuit edit characterization. In  doing so, an advanced Focused Ion Beam deposition method is  required to put a leaky path with a resistance range of 1k to 10k  ohms. If the leaky path between the nodes can be reproduced  using FIB technique, characterization can be done to further  lessen the OBIRCH signal generated by deposited metals used  to re-route the faulty nodes to the package external pins. In  addition, the proposed new topside method can also be used for  backside OBIRCH when the only available equipment is a  topside OBIRCH system.

