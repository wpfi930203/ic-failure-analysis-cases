---
title: "240_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_bb8456af50a3d7a78565f872242ea5007295230462135641
file_size: 780976
---

## Identification of Recovering Package  Leakage Failure Mode Via Novel  Comprehensive Failure Analysis Technique  

Izhar Helmi Ahmad, Nazirul Izzat Bin Mohd Arifen, Mohammad Eizwan Bin Rosle,  Mohd Fakhrul Bin Mohamad,   Shahril Amir Bin Mohd Desa    Failure Analysis Laboratory, Nexperia Malaysia Sdn. Bhd.,   PT 12687, Tuanku Jaafar Industrial Park, Kawasan Perindustrian Tuanku Jaafar, 71450 Seremban, Negeri Sembilan, Malaysia.  Phone :   $(+60)$   676 6299, Email: Izhar.Helmi.Ahmad@nexperia.com

Abstract-The packaging of semiconductors  significantly impacts their performance, especially with  the current emphasis on energy-saving applications.  Increasing package complexity has led to issues such as  leakage. Therefore, failure analysis (FA) is crucial in  identifying the actual root cause of these failures. Device  recovery issues have been rising, correlating directly  with advancements in new process technologies and  packaging methods. This paper introduces a novel FA  methodology that combines electrical characteristic  analysis, precise package fault isolation, mechanical  cross-sectioning,   and   Focused   Ion   Beam   (FIB)  techniques. This integrated approach helps resolve  failure recovery issues and efficiently identify the root  causes of failure mechanisms. Without proper FA  procedures for recoverable package leakages, critical  evidence might be missed, leading to inaccurate FA  results or conclusions and a high chance of recurring  failures. The proposed methodology begins with  electrical   characterization   to   identify   anomalies,  followed by precise fault isolation to pinpoint the fault.  Mechanical cross-sectioning or FIB allows for a detailed  examination of the package layers. By integrating these  techniques, our methodology provides a comprehensive  view of the failure mechanism, ensuring no potential  cause is overlooked. In summary, this work presents a  comprehensive FA methodology that enhances the  identification of device failure mechanisms. As a result,  package recovery issues are addressed effectively,  providing the production team with precise insights into  the failure mechanisms and facilitating accurate  investigations. This methodology resolves immediate  recovery   issues   and   contributes   to   long-term  improvements   in   semiconductor   packaging   and  performance.

## I.    OBJECTIVE  

This paper endeavors to investigate package leakage  failures through a novel methodology that combines  electrical characteristic analysis, precise package  fault   isolation   [1],   and   mechanical   crosssectioning/Focused Ion Beam (FIB) [4] techniques.  By leveraging these complementary approaches, we  aim to provide a comprehensive understanding of the  failure mechanisms involved, ensuring accurate  identification and resolution of leakage issues. This  integrated approach enhances the accuracy of failure  analysis and reduces the time required to pinpoint the  root cause, ultimately leading to more reliable and  robust semiconductor packages.

## II.   INTRODUCTION  

Package leakage is unwanted electrical leakage  within semiconductor device packages, resulting  from defects in packaging material, improper sealing,  or   contamination.   This   leakage   can   degrade  performance or cause device failure, making  detection   and   mitigation   critical   for   reliable  semiconductor   manufacturing.   Techniques   like  electrical testing and package inspection help identify  and address leakage issues.

Semiconductor packaging materials, such as epoxy  resins or ceramics, must have high-insulating  properties. However, defects like voids, cracks, or  impurities can compromise insulation, leading to  leakage. Contamination from dust, moisture, or oils  during packaging can also create conductive paths  and increase leakage risk. Thermal cycling and  mechanical stress during device operation can worsen  these defects over time, impacting long-term  reliability.

In high-reliability applications, such as aerospace or  medical devices, even minor leakage can be  catastrophic, necessitating rigorous failure analysis  (FA) methodologies. Traditional FA involved front

side defect localization followed by chemical  decapsulation, which could induce high temperatures  and obscure defect evidence.

A novel comprehensive FA method combines  electrical characteristic analysis, precise package  fault isolation, and mechanical cross-sectioning or  Focused Ion Beam (FIB) techniques. This approach  enhances failure mechanism identification accuracy  and reduces diagnostic time. It is especially valuable  for new process technologies and packaging methods,  offering   insights   for   improving   design   and  manufacturing processes, and leading to more robust  and reliable semiconductor packages.

## III.   METHODOLOGY  

Conventional failure analysis uses non-destructive  methods like X-ray and SAM to detect defects,  followed   by   electrical   verification.   Chemical  decapsulation then exposes the internal structure, but  high temperatures can alter or repair the failure site,  leading to inaccurate analysis. This process often  obscures   the   original   failure   mechanism,  necessitating advanced techniques.

![Non-destructive analysis  (External visual, Internal visual, SAM)  Electrical verification  Chemical decapsulation  Visual inspection  Re-electricalverification afterbackside polish  Topside fault isolation  (Photoemission, OBIRCH, LIT)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1eb0c326-ade7-4048-898a-068d0743ee3c/1eb0c326-ade7-4048-898a-068d0743ee3c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=ebc2f99ad58d336aaa893d1fcf3e7ed4963c3657)
Fig. 1. Conventional front-side process flow

A back-side defect localization analysis   was  conducted to determine the root cause of failure. First,  non-destructive methods like X-ray and SAM  identified package anomalies, followed by electrical  verification to confirm the failure. The sample then  underwent mechanical backside polishing to expose  the silicon die for further analysis. However, the  sample recovered after polishing, making fault  isolation impossible. This recovery is common in  traditional   FA   approaches,   where   heat   and  mechanical stress during preparation can alter or  repair the failure site, leading to inaccurate analysis.

![Non-destructive analysis  (External visual, Internal visual, SAM)  Electrical verification  Chemical decapsulation  Visual inspection  Re-electrical verification after backside polish  Topside fault isolation  (Photoemission, OBIRCH, LIT)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/312975c9-8c9f-487a-a2dd-af06e69eb149/312975c9-8c9f-487a-a2dd-af06e69eb149.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=68b75f80d8413f9ecf482c1117ce68acfb3d4a4f)
Fig. 2. Conventional back-side process flow

To address the device's recovery issue, a novel  comprehensive FA method was developed. This  method combines electrical characteristics, precise  package fault isolation, and mechanical crosssectioning or Focused Ion Beam (FIB) techniques.  Non-destructive analysis using optical scopes, X-ray,  and Scanning Acoustic Microscopy (SAM) examines  package abnormalities. Electrical verification with a  curve tracer and continuity testing detect shorts,  leakage, or open junctions. This integrated approach  ensures thorough investigation of all potential failure  mechanisms, providing high-resolution insights and  precise fault isolation to accurately identify the root  cause of failure.

![ Non-destructive analysis   (External visual, Internal visual, SAM)  Electrical verification & Characterization  Package isolation  (Topside package polishing)  Curve tracer continuity testing at each node of  isolationwire.  Topside fault isolation  (LIT or OBIRCH)  Focus lon Beam/ Mechanical Cross section cut   Optical inspection/ SEM/ EDX analysis on the cross-sectionplane  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7b9af56c-6e48-47f0-a4ce-dec1f6c432d9/7b9af56c-6e48-47f0-a4ce-dec1f6c432d9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=14463dfd581f31f8fddef3373d95b5482778b02d)
Fig. 3. Novel comprehensive process flow

After confirming the failure mode, package isolation  is conducted by mechanically polishing from the  topside of the package. The objective of this  polishing is to sever the wire loop to differentiate  the connection between the die level and package  level. Subsequently, continuity testing is carried out  by performing micro-probing at each isolation wire  loop point. This testing is conducted in conjunction  with the reference sample. Any abnormal or noncomparable curves compared to the reference will  be recorded.

When the short or leakage path is identified, the unit  undergoes top-side fault isolation using Lock-In  Thermography (LIT), designed to detect hotspots at  the package level. The novelty of LIT lies in its  ability to perform fault isolation without requiring the  removal of the mold compound. Once the localized  hotspot is detected, the X and Y measurements from  the hotspot site to the nearest reference mark are  recorded and used for FIB and cross-section marking.  These localized measurements on the topside surface  serve as a guide for physical analysis.

Since this package leakage mode tended to recover,  the Focused Ion Beam (FIB) or mechanical crosssection cut approach was used to uncover the failure  mechanism and prevent device recovery issues. The  sample underwent sample preparation, followed by  cross-section   analysis   based   on   the   hotspot  measurement. The cross-section cut is performed  progressively, and any abnormal structure in the  crosscut plane will be captured using a high-power  scope and Scanning Electron Microscopy (SEM).  Further Energy Dispersive X-ray Spectroscopy  (EDX) [3] analysis will be conducted to investigate  any suspected foreign material elements.

This comprehensive approach ensures that the root  cause of the failure is accurately identified and  properly addressed, thereby improving the reliability  and performance of semiconductor devices.

## IV.   EXPERIMENTAL   RESULT,   ANALYSIS   AND DISCUSSION  

In this paper, two case studies will be discussed with  dissimilar failure mechanisms, utilizing the novel FA  methodology introduced to uncover the failure  mechanism and successfully prevent the device from  recovering. This comprehensive approach ensures  that the root cause of each failure is accurately  identified and properly addressed, thereby improving

the reliability and performance of semiconductor  devices.

## Case study 1  

A returned SOT1255 package device was received  with the problem description 'ICC failure.' External  and internal package inspections, as shown in Figure  4 and Figure 5, did not reveal any abnormalities.

![P2(GND)  P2(GND)  P1(VCC)  P1 (VCC)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/901eeb1d-c752-4c79-89cc-7c3147296170/901eeb1d-c752-4c79-89cc-7c3147296170.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=f908fe6c2f039b47f7c202000c824ad41ace12f4)
Fig. 4. External package image.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3ae1b5d6-625a-4d7a-827e-21683f26b2f6/3ae1b5d6-625a-4d7a-827e-21683f26b2f6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=9b5fdccae2867865f1df5fd3e346df03bb99e8ab)
Fig. 5. X-ray examination image. No internal abnormal structure  was observed.

The pin-to-pin curve tracer was conducted, verifying  leakage between pin 1 (VCC) and pin 2 (GND).  Bench testing confirmed that the unit had indeed  failed for ICC, as reported in the ATE data. This  comprehensive testing approach ensured accurate  identification of the failure mode and provided the  necessary data for further analysis.

![VCCAtOGND  300.0UA:  200.0U  00.0  100.0  200C  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3b74f8c5-c7e3-488a-ac34-c1be0c8d098b/3b74f8c5-c7e3-488a-ac34-c1be0c8d098b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=ddb3f7b7bb8c7266613a250fe49ef24a7e360623)
Fig. 6: Pin-to-pin curve tracer showed leakage curve between pin  1(VCC) and pin 2(GND)

A representative unit, SN1, and a known good unit  (KGU) underwent topside package polishing to

isolate the wires. Subsequently, micro-probing was  conducted between pin 1 (VCC) and pin 2 (GND).  Each wire was separated into two parts: one  connected to the external pin and the other to the die.  In this case, a resistor short junction was observed  when probing between the wire connected to external  pin #1 (VCC) and the wire connected to bond pad #2  on the die (GND). This indicated that the leakage was  from the grounded die substrate to external pin #1.

This detailed analysis confirmed the presence of a  leakage path originating from the die substrate, which  was grounded, to external pin #1 (VCC). Such  findings are crucial for identifying the root cause of  the failure and implementing corrective actions to  prevent recurrence.

![Wire connected to bond  Wire connected tobond  pad die #2 (GND)  pad die #2 (GND)  probe  Wire connected to external  Wire connected to external  pin #1 (VCC)  pin #1 (VCC)  probe  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3446475e-d0a9-4953-a041-e1e755c10018/3446475e-d0a9-4953-a041-e1e755c10018.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=9151f3a1bfecb6304d51f290b47ccacba6d9ff36)
Fig. 7. Optical inspection image after top side polishing. The wires  were isolated. The red arrows showed the location of probe  between wire connected to external pin#1 (VCC) and wire  connected to bond pad#2 (GND)

![VCCAleadtoGNDdie  3000UA:  200L0U  1000UA  1000u  200.0  Leosnd  SN#T9  30  MuDrS  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2122a599-df98-4209-ac8a-c15cbc4f9015/2122a599-df98-4209-ac8a-c15cbc4f9015.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=db69cda0ad844e6686d0185646af65e05ffa9b0d)
Fig. 8. Micro probing test between wire connected to external  pin#1 (VCC) and wire connected to bond pad#2 (GND) showed  resistance short junction.

The unit was then further polished on the top side  until it reached near the top side of the die. This  process was carried out slowly and carefully to  prevent over-grinding of the topside die's active area.  The additional thinning-down process was necessary  only for units that required top-side OBIRCH testing,  as the OBIRCH spot could not penetrate the mold  compound. In contrast, topside LIT could be  performed without the need to thin down the mold  compound.

Thinning down the mold compound ensures that the  OBIRCH test can effectively detect faults in the  package. It's a delicate process, requiring precise  control to avoid damaging the active area of the die.  This step is critical for ensuring accurate fault  isolation and identifying the root cause of the  failure.

![probe  OBIRCHspot location  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0330dd72-6b87-432a-a46a-25f8040f2b89/0330dd72-6b87-432a-a46a-25f8040f2b89.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=599b0f8c25057569416fec8f5005c4dc91e95452)
Figure 9: Optical inspection image after further topside polish. It  still has a very thin layer of mold compound remaining on top  surface.

Furthermore, top-side OBIRCH [5] analysis was  conducted by biasing between the wire connected to  external pin #1 (VCC) and the wire connected to  bond pad #2 (GND). Details of the biasing  connection are illustrated in Figure 9. A localized  OBIRCH spot was detected at the edge of the die.

This OBIRCH analysis provided critical insight into  the location of the leakage path. By biasing between  specific connections, we were able to pinpoint the  exact area where the electrical leakage occurred. This  information is crucial for further analysis and  corrective actions to prevent similar issues in future  units. The OBIRCH technique, with its ability to  detect faults without needing to thin down the mold

compound, proved essential in this case for its  precision and non-destructive nature.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a23a1836-dd58-481e-81ef-32e32ce8e90f/a23a1836-dd58-481e-81ef-32e32ce8e90f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=d2a4573502000820f231b620395137c462b3ce3d)
Fig. 10. OBIRCh spot was detected at the edge of the die near with  pin1 when unit was biasing between wire connected to external  pin#1 (VCC) and wire connected to bond pad#2 (GND).

Once the localized OBIRCH spot was detected, the  unit underwent mechanical cross-sectioning. Optical  inspection and SEM examination of the cross-section  revealed evidence of a tilted die, causing the bottom  of the die to touch and contact the lead of pin 1,  resulting in a short junction between the VCC and  GND terminals.

This detailed cross-section analysis confirmed the  physical root cause of the electrical leakage. The  tilted die led to unintended contact between the die's  bottom and the lead of pin 1, causing the electrical  short. Such findings are critical for understanding the  failure mechanism and implementing corrective  measures to prevent similar issues in future units.

The   combination   of   OBIRCH   analysis   and  mechanical   cross-sectioning   provided   a  comprehensive understanding of the failure, ensuring  accurate root cause identification and effective  resolution. This approach highlights the importance  of advanced analytical techniques in semiconductor  failure analysis.

![Diesubstrate   Diesubstrate  Bright field microscope image   Darkfieldmicroscopeimage  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/59038582-2ca9-4c78-9adc-b1b388caac33/59038582-2ca9-4c78-9adc-b1b388caac33.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=9b08c7dcf7e0d531cd4db639b8842c3e793a7a31)
Fig. 11. Optical inspection showed a touching between die  substrate and the contact lead of pin 1.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b39fbff8-2891-4725-95e7-411416915b8e/b39fbff8-2891-4725-95e7-411416915b8e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=0a6b0de98e722aabea8d63ebf88aeb00ac5c978d)
Fig. 12. SEM examination showed a touching between die  substrate and the contact lead of pin 1.

Furthermore, EDX analysis was performed to  confirm the elements present at the contact area.  Nickel (Ni) elements were detected at the touching  area between the die substrate and the contact lead of  pin 1.

This EDX [6] analysis provided crucial confirmation  of the materials involved in the contact area. The  presence of nickel suggests that the material of the  contact lead of pin 1 contributed to the unintended  electrical short with the die substrate. Such findings  are essential for understanding the interactions of the  materials   causing   the   failure   and   informing  improvements in manufacturing processes.

The combination of OBIRCH analysis, mechanical  cross-sectioning, and EDX provided a comprehensive  investigation into the root cause of the failure. This  approach   ensures   accurate   identification   and  resolution   of   semiconductor   device   issues,  maintaining   high   reliability   and   performance  standards.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/67e5075c-a1dc-406b-8367-301ddb65c32d/67e5075c-a1dc-406b-8367-301ddb65c32d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=a906af32a544a34c26cc57dfc687ecc6a88010d4)
Fig. 13. Mapping EDX analysis showed Ni (Nickle) element at  touching between die substrate and the contact lead of pin 1.

## Case study 2  

A returned SOT1255 package device was received  with the problem description "Please check for any  assembly defects in the package." External and  internal package inspections were conducted, but no  abnormalities were found (refer to Fig. 14 and Fig.  15).

This comprehensive inspection involved detailed  external and internal examinations using advanced  inspection techniques. Despite thorough scrutiny, no  visible defects or anomalies were detected in the  packaging material or assembly.

The absence of abnormalities suggests that the initial  assembly process and package integrity were  maintained. This finding is crucial for ensuring the  device's reliability and functionality in its intended  application.

![P1  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4d1dbece-562d-402e-8fd7-c89d5aa8f6d1/4d1dbece-562d-402e-8fd7-c89d5aa8f6d1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=5bb98ea18f2c17f987a8d57f8b8582fe1db3835a)
Fig. 14. External package image.

![   ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6ecd7604-50f8-4f93-9454-b569b3be3628/6ecd7604-50f8-4f93-9454-b569b3be3628.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=5f62d54616ed684c7f6ed3505094991fb443cb69)
Fig. 15. X-ray examination image. No internal abnormal structure  was observed.

The pin-to-pin curve tracer confirmed a short  junction between pin 4 (B1) and pin 1 (GND), as  shown in Figure 16.

![#4 refA P2-P1  4A1P3-P1  ##   APPPSP  #4ENP6-P1  soon  4.SU  5 4.5 4 -3.5 -3 2.5 -2 -1.5 -1   11.522533.5  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/017b6eab-b219-44dd-a536-8af6e103b5c5/017b6eab-b219-44dd-a536-8af6e103b5c5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=b59a99d89b33415273cd09263c2b1ac592a48bab)
Fig. 16: Pin-to-pin curve tracer showed leakage curve between pin  4 (B1) and pin 1(GND)

A representative unit, SN4, and a known good unit  (KGU), underwent topside package polishing to  isolate the wires. Following this, micro-probing was  conducted between pin 4 (B1) and pin 1 (GND).  Each wire was divided into two parts: one connected  to the external pin and the other to the die. In this  scenario, a resistor short junction was identified  during probing between the wire linked to external  pin #4 (B1) and the wire linked to bond pad #1 on the  die (GND). This indicates that the leakage originated  from the grounded die substrate to external pin #4.

This detailed analysis confirmed the presence of a  leakage path from the grounded die substrate to  external pin #4. Such findings are crucial for  identifying the root cause of the failure and  implementing   corrective   actions   to   prevent  recurrence.

To further investigate, OBIRCH analysis was  conducted by biasing between the wires connected to  pin 4 (B1) and pin 1 (GND). The OBIRCH spot

detected near the die edge corroborated the presence  of a localized leakage path at the die surface.

The combination of micro-probing and OBIRCH  analysis provided comprehensive insights into the  failure mechanism. The identified short junction and  localized leakage path at the die edge were critical  findings that guided subsequent mechanical crosssectioning and material analysis.

![PPI   P6S  PB  Wire connected to  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6a0c32c3-b86f-448c-b221-0312dfeed2b2/6a0c32c3-b86f-448c-b221-0312dfeed2b2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=2df7d92481f799fb1154e2fb5d958a10f1543057)
Fig. 17. Optical inspection image after top side polishing. The  wires were isolated. The red arrows showed the location of probe  between wire connected to external pin#4 (B1).

![IF  1  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4d39e8da-20f3-46a1-97ed-1d5f1df6374c/4d39e8da-20f3-46a1-97ed-1d5f1df6374c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=c3bd21d66f17f522780f53a0d145c695c80d2448)
Fig. 18. Pin-to-pin curve tracer showed leakage curve between pin  2 (refA) and pin 1(GND), curve remain similar before wire  isolated.

Following   that,   the   unit   underwent   Lock-In  Thermography   (LIT)   for   fault   isolation   and  localization, as illustrated in Figure 19. A localized  LIT spot was identified at the edge of the die.

![GND  B1  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/86df1e03-c6ae-433f-9fe2-b5be967caf96/86df1e03-c6ae-433f-9fe2-b5be967caf96.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=263e59e08e97927aedba7f2ed80f8e15776a2158)
Figure 19: LIT image showing hotspot near to Pin4 (B1) with  biasing conditions between P1 (Gnd) and Pin4 (B1).

After the localized LIT spot was detected, the unit  underwent Focused Ion Beam (FIB) analysis. The  FIB analysis subsequently revealed evidence of  Palladium (Pd) element traces between the lead frame  of B1 and the die edge, causing the bottom of the die  to make contact with and touch the lead of pin 4 (B1).  This contact resulted in a short junction between the  B1 and GND terminals.

This detailed analysis using FIB confirmed the  physical root cause of the electrical short. The  presence of Palladium traces indicated material  interaction between the lead frame and the die,  leading to unintended electrical contact. Such  findings are crucial for understanding the failure  mechanism and implementing corrective actions to  prevent similar issues in future units.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d5a44b47-fce4-46d1-8923-5e6392b6faf3/d5a44b47-fce4-46d1-8923-5e6392b6faf3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=608a86e34af6e8761fe998d16a28acb6e1dffda7)
Fig. 20. FIB showed a touching between die substrate and the  contact lead of pin 4.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/10891649-b5e4-43b1-be00-392758ce8d54/10891649-b5e4-43b1-be00-392758ce8d54.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=c1135af1fad14d7ec4361a3b9a99e7d295dc4e2e)
Fig. 21. FIB examination showed a touching between die substrate  and the contact lead of pin 4.

Additionally, Energy-Dispersive X-ray Spectroscopy  (EDX) analysis was conducted to confirm the  presence of elements at the contact area. Palladium  (Pd) elements were detected at the contact point  between the die substrate and the lead of pin 4.

This EDX analysis, shown in Figure 22, provided  crucial confirmation of the materials involved in the  contact area. The presence of Palladium suggests that  material from the lead of pin 4 contributed to the  unintended electrical short with the die substrate.  Such findings are essential for understanding the  material interactions causing the failure and for  informing improvements in manufacturing processes.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/90f08ee1-ad5d-45f4-8d30-c6ce04b4e63b/90f08ee1-ad5d-45f4-8d30-c6ce04b4e63b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215765%3B1743219365&q-key-time=1743215765%3B1743219365&q-header-list=host&q-url-param-list=&q-signature=f84acf4a7b17e5e2a00073675c4eef42f655cb94)
Fig. 22. Mapping EDX analysis showed Pd (Palladium) element at  touching between die substrate and the contact lead of pin 1.

## CONCLUSION  

This work introduces a novel Failure Analysis (FA)  methodology utilizing a combination of electrical  characteristics, precise package fault isolation,  mechanical cross-section techniques, and Focus Ion  Beam (FIB) to address the issue of recovering  package leakage. Employing this comprehensive  technique resolves the problem of failure recovery  and efficiently identifies the precise root cause of  the failure mechanism.  In the absence of proper FA  steps performed on the package leakage failure, there

might be a tendency to overlook evidence and  provide an inaccurate FA result or conclusion. This  could lead to misleading conclusions if the exact root  cause is not properly addressed and corrected.

## V.   ACKNOWLEDGMENT  

We would like to extend our gratitude and  appreciation to Edward Ooi Cheow Hoe, Saraswathy  Supramaniam, Yew Boon Tan, and the members of  the Failure Analysis Department for their invaluable  support and contributions to completing this technical  paper. Their expertise, dedication, and collaborative  efforts were instrumental in developing and refining  the novel FA methodology discussed in this work.  Their insights and feedback greatly enhanced the  quality and comprehensiveness of our analysis.

Their commitment to excellence and their willingness  to share their knowledge and experience were  essential in addressing the challenges encountered in  the research and development of this methodology.  We are sincerely thankful for their assistance  throughout this project.

## REFERENCE  

[1]    Izhar Helmi Ahmad, “Innovative Fault Isolation Analysis  Technique to Identify Failure Mechanism on Recovering  Device Failure.,” ,  IEEE 23rd International Symposium on  the Physical and Failure Analysis of Integrated Circuits  (IPFA), 2016.     [2]    Yusnani Mohamad Yusof, Evaluation of Thermal Mapping  Analysis Technique for Failure Mechanism..,  Proceedings of  the 20th IEEE International Symposium on the Physical and  Failure Analysis of Integrated Circuits (IPFA), 2013.      [3]    Hua Younan, “Studies of TEM/EDX data process and  application in identification of Cu oxide compounds”,  IEEE  24th International Symposium on the Physical and Failure  Analysis of Integrated Circuits (IPFA), 2017.      [4]    Nazirul Izzat Mohd Arifen; Mohd Azlan Mat Ayob;  Nurashikin Ismail “Failure analysis technique of backside  focused ion beam on decapsulated device”,  IEEE 24th  International Symposium on the Physical and Failure  Analysis of Integrated Circuits (IPFA), 2017.      [5]    Xiaoling Lin; Hongqi Zhang, “OBIRCH based on differential  imaging locating method”,  10th International Conference on  Reliability, Maintainability and Safety (ICRMS), 2014.     [6]    Hua Younan, “Studies of TEM/EDX data process and  application in identification of Cu oxide compounds”,  IEEE  24th International Symposium on the Physical and Failure  Analysis of Integrated Circuits (IPFA), 2017.      [7]    Rafael Espino Campos; Elson Y. Sakô; Hugo Soeiro  Moreira; João Lucas de S. Silva; Marcelo G. Villalva  “Experimental Analysis of a Developed I-V Curve Tracer  under Partially Shading Conditions”,  IEEE PES Innovative  Smart Grid Technologies Conference - Latin America (ISGT  Latin America), 2019.

