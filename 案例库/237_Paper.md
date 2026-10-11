---
title: "237_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_c0952a77268c304b3995602329a254457295230462135641
file_size: 674967
---

## A Systematic Failure Analysis Approach to Determine  True Electrical Overstress Failures on Integrated  Circuits  

Em Julius De La Cruz  Maxim Integrated, Gateway Business Park, Brgy. Javalera, Gen. Trias, Cavite, Philippines  Phone: +63 2 902 2000 loc. 2313 Email:  emjulius.delacruz@maximintegrated.com

Abstract-   Root cause determination of electrical overstress (EOS)  failures has become significantly important because of the  automotive industry's continual quest for quality improvement.   The determination of EOS as the failure type in a defective IC is  important, but incomplete without accurately attributing the  failure to a root cause such as a design flaw, manufacturing defect  or exposure to electrical stresses beyond the recommended  operating conditions.  Further improvement in outgoing quality  depends on an efficient and effective failure analysis process to  distinguish between units that fail due to EOS events, where  recommended operating limits are exceeded, and units that fail  due to a latent defect.  This paper presents a systematic approach  to failure analysis of EOS that accurately determines failure root  cause.  Case studies are presented that illustrate the process and  resulting root cause conclusions that enable implementation of  appropriate corrective actions.

Keywords  –  EOS, Electrically Induced Physical Damage,  Absolute Maximum Rating.

## I. I NTRODUCTION 

EOS is one of the top failure contributors in the  semiconductor industry.  EOS still accounts for about   $30\%$   of  the electrical failures both at manufacturing line and in the field.  This fraction for EOS has remained high for the past several  years.

![350  0020  200  150  100  50  NTF   EOS   FAB   Asmbly   Test   Device  'TypicalFailure ParetoAnalysis-SeveralSources   ESD  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e7bab905-9311-478b-8195-4642282a26fd/e7bab905-9311-478b-8195-4642282a26fd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=4297c302e7ceb06aa548d37c2e70ce5b010cc6dc)
Fig. 1  Typical Failure mechanism pareto [1].

One type of electrical stress,  Electrostatic Discharge (ESD),  has been approached in a systematic manner. ESD received so  much attention in technical literature, standards bodies,

educational workshops and tutorials, which resulted in  relatively successful practices for design of robust devices and  control procedures for the factory,  hence device-level ESD  failures have only small contribution in the total EOS picture  (Fig. 1).  In contrast, the semiconductor and electronics industry  has been challenged with a large portion of EOS failures with  limited way of addressing the issue in a systematic manner.   One of the major reasons is that root causes for EOS are broadly  diverse and very application dependent.  Thus, ESD models  such as Human-Body Model (HBM) and Charged-Device  Model (CDM) for ESD are not comparable  to address EOS root  causes [1].

EOS conclusions are made from failure analysis.  However,  without a proper FA approach where follow-up analysis or root  cause investigation is seldom done, EOS cases often remain  unresolved.  Most analysis results do not provide additional  valuable information which is often misleading during root  cause investigation. Thus, it is important that the analysis on  EOS failures is approached correctly in order to come up with  an accurate conclusion.  This is essential so that process experts  who will be involved in the root cause investigation will come  up with an effective corrective action.

Previously published technical works on EOS  were used as  reference in developing a systematic failure analysis flow to  approach potential EOS cases.  The objective is to be able to  determine and validate if the failure is really caused by EOS  event in order to provide a more complete and accurate FA  result.  Case studies will be presented to illustrate the  application and effectiveness of the developed FA approach.

## II.   REVIEW   OF   RELATED   WORK  

In 1968, a model for the thermal failure of semiconductor  devices due to pulse voltages was published by Wunsch and  Bell. The power-to-failure Pf originally normalized to the  junction area A plotted over the pulse width TP in a double  logarithmic manner became known as the Wunsch-Bell plot  (Fig. 2) [2]. However, as highlighted by Welsher, the typical  presentation of the Wunsch-Bell plot does not include the effect  of pulse rise time which is an important factor in determining  where and how a device might fail [1].

![scale  12  1/ln（T/1s)  const.  SafeArea  logscale  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/528c6971-c8aa-4d61-a009-29c24287d03b/528c6971-c8aa-4d61-a009-29c24287d03b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=b185db6f2165cdbaf0d0150c0d54e2c8921c54ee)
Fig. 2  The Wunsch-Bell characteristics model.

During the 2011 EOS/ESD symposium, Kaschani and  Gaertner presented a summary of possible causes of EOS (Fig.  3), illustrating that root causes for EOS are broad and  application dependent.

![Unpowered  Handling  Field induced   Lackof/poor  events   grounding  Charged  people   Charged  Charged devices/   cables  Unsuarasl/systems   Discharges  processes  Manu-facturing  Inappropriate   process  Handling&  welding  Storage  Unsuitable   Mechanical  damage  packing  Unsuitable  Environment  materials  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/946c71e4-3e45-458e-a1e8-2aef05d34ad8/946c71e4-3e45-458e-a1e8-2aef05d34ad8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=f893087a8fac5091ba32061899d9ffa87e42293d)
Fig. 3  Excerpt from diagram of possible causes of EOS as presented by  Kaschani and Gaertner [3].

Sectors from the field, especially those from the automotive  industry, were calling to establish EOS standards similar to  what has been done to tackle ESD.  Thus in 2011, an ad hoc  working group was convened in the ESD Association (ESDA)  and was a precursor to work undertaken in the Industry Council  on ESD Targets [1].  A white paper on EOS was released in  August 2016 to document these efforts which tackled a major  comprehensive review on EOS work.  The purpose of the white  paper is to introduce a new perspective about EOS to the  electronics industry, clarify what EOS really is and how it can  be mitigated once it is properly comprehended, and explain the  most important facts so that the involved partners in the  industry have the opportunity to understand and recognize  helpful steps for analysis and avoidance of EOS events [4].

One of the topics discussed in the white paper is to create a  common understanding and practical interpretation of EOS as it  has become obvious that there is a wide disparity in the  interpretation of EOS, a misunderstanding that can lead to

disastrous   result.      An   aligned   understanding   allows  semiconductor manufacturers to clearly provide the maximum  electrical limits for their devices and knowing these limits  allows system manufacturers to optimally incorporate those  devices into their systems while providing a working  environment in which the devices can safely operate [4].

Most of the time, Failure Analysis Engineers would likely  classify the term EOS to any visible damage that appears to be  caused by excessive current or voltage, even without the clear  knowledge on the maximum operation limits nor the real  application conditions [4].  This is where the misdiagnosis  comes in.   Thus, it is not established if the failure is really an  EOS operation beyond the operating limits or a failure due to a  defective device that failed under stress within the operating  limits.  The white paper established a practical interpretation of  EOS in terms of AMR (Absolute Maximum Rating) as  illustrated in Fig. 4.

![ElectricalOverstress  1009  Region A   Region B   Region C   Region D  Safe Handlingnand  Restriitions  HighatRisk of   Immmdigte  (Robust)   Damage  Maximum   AbsoluteMaximum   Electrical Stress  Operating Condition   Rating  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/af7a1430-4a09-4f2c-8e2e-3e2f4efcebab/af7a1430-4a09-4f2c-8e2e-3e2f4efcebab.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=b8cda8eef4dc22699a0cafe3375322915cfeff0f)
Fig. 4  A graphical illutration on how to interpret the AMR.  Yellow line  indicates the number of components suffering immediate, catastrophic EOS  damage [4].

In addition, the term “electrically induced physical damage”  (EIPD) was introduced as a terminology to use when it has not  yet been determined if a unit experienced EOS event [10].   Table I summarizes the definition of EOS versus EIPD as  defined in the published paper by Target Levels.    Hence, with clearer definition of EOS, there    Industry Council on ESD  can be an alignment and common understanding among failure  analysts, suppliers and customers.

Table I – White Paper Definition of EOS and EIPD

|Term|Definition|Definition|||
|---|---|---|---|---|
|EOS|An electrical device suffers an electrical overstress||||
||event when a maximum limit for either the voltage||||
||across, the current through, or power dissipated in the||||
||device is exceeded and causes immediate damage or||||
||malfunction, or latent damage eresulting||||
||unpredictable reduction of its lifetime.||||
|EIPD|Damage to   an|integrated||due  to|
||electrical/thermal stress beyond the level which the||||
||        materials could sustain. This would include melting of                silicon, fusing of metal interconnects, thermal damage      ||||
||to package material, fusing of bond wires and other||||
||||||
||damage caused by excess current or voltage.||||


## III. METHODOLOGY  

The published white paper was used as main reference in  developing a failure analysis flow.  Specifically applied was the  definition of AMR, EIPD and EOS. The EOS investigation  work flow will establish a systematic approach in the failure  analysis process (refer to Fig. 5).  The work flow will easily  guide the analysts to  identify possible sources of EIPD during  the analysis.

![FA Diagnosis is EIPD  FA Diagnosis is EIPD Assembly  Assembly   Yes  Yes  Improve Assembly  Improve Assembly Defect  Defect  Process  Process 7O  No  Damaged Site  Damaged Site  70  No  Improve Fab  Improve Fab  connected to  connected to  external pin  external pin  Process  Process yes  Yes Workwith  Work with EIPD similar  EIPD similar   yes  Yes customer to  customer to  to ESD stress  to ESD stress  eliminate sources  eliminate sources  signature  signature of ESD  of ESD No 7O  Failure  Failure   Yes  Yes  Investigate for  Investigatefor  signature is  signature is  Design weaknesses  Design weaknesses systemic  systemic 7O  No Work with  Work with AMR  AMR   yes  Yes customerto  customer to  exceeded  exceeded  eliminate sources  eliminate sources  ofEOS  of EOS No/lnfo not  No/Info not  available  available Workwith customerto  Work with customer to  investigate application conditions  investigate application conditions ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/97d84e7a-eb8b-4dc3-8d3d-9d49e5903274/97d84e7a-eb8b-4dc3-8d3d-9d49e5903274.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=61dc51c1584e09893e8f4ab2a6b39b1ed7f77adc)
Fig. 5  Snapshot of EOS investigation workflow.

With the EOS work flow in place, the failure analyst  can  make an assessment if the observed EIPD is caused by EOS as  per definition or was a defective device that was stressed within  the operating limits.  The assessment will be very critical in the  analyst’s engineering judgment as it will determine the  direction of additional failure analysis steps.

To test the feasibility of the EOS investigation work flow,  a  compilation and review of previous cases with physical damage  manifesting as EIPD and closed as EOS was done.  These were  subjected to the EOS investigation workflow to come up with  hypothesis on the possible sources of EIPD.  The compilation  data is shown in Fig. 6, showing the physical manifestation of  EIPD and the possible conclusion/hypothesis based on the  developed work flow.

|        Defect Location                Connected to                External Pin?      |EIPD Type|EIPD Signature|Possible Conclusions|
|---|---|---|---|
|        Yes, esd                 clamp       |        Melted                Metal      ||Application|
|         Yes, esD                 clamp       |        Fused                Silicon                ony      ||        related EOS/ESD.                ESD at customer.                ESD at assembly.      |
|        Yes, Non-ESD                 clamp       |        Melted                wire /ball                 bond only      ||Application|
||||        Assembly Process                related.      |
|        Yes, Non-ESD                 clamp       |        Melted                Metal      ||        Application                related EOS.                Design      |
||        Melted                Metal      |||
||        Silicon/                Oxide only      ||        Fab process                Related.      |
|         No, Non-ESD                 clamp       ||||


Fig. 6  Review of previously closed FA cases subjected to the EOS investigation  work flow, showing the most probable cause/source of EIPD.

On-going FA cases were subjected to the EOS investigation  work flow to determine if the failures are true EOS or was due  to manufacturing defect.  Two case studies are presented.

## Case Study 1  

A high current-high voltage Switching Regulator IC were  reported to fail at field with initial failure analysis results  showing shorted pins on supply and Boost Regulator pins [5].  Physical analysis revealed EIPD in the form of melted/burnt  circuitries in the low side and high side FETs (Fig. 7).

![High-SideFET  Low-SideFET  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c49f46f2-b4ca-46b8-acee-6db57f29f2d8/c49f46f2-b4ca-46b8-acee-6db57f29f2d8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=b36a80d9174db1f716b963a71df75a686ba66cbb)
Fig. 7  Laser scanning images showing EIPD in the form of melted/burnt silicon  (red arrows).

For this kind of failure mechanism (melted/burnt Silicon), the  FA engineer will typically conclude that the cause of failure is  due to EOS which is most likely induced at customer’s  application (external sources beyond the device’s AMR).   However, through the EOS investigation work flow, the  validity of the conclusion was tested.

Thus, using the EOS investigation work flow (Fig. 5), the  observed EIPD can be potentially caused by customer’s  application, or Fab/Assembly Process related.  To further gather  evidences to identify the source of failure, further analysis was  then carried out.  Results revealed passivation cracking (Fig. 8).

![ation1  Drive  HSFEL  Location3    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b2e07dea-360e-4dd2-816e-5bc4517f2e2e/b2e07dea-360e-4dd2-816e-5bc4517f2e2e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=1b2ea93471a1abb27c084404bae8f330ef0fd6d4)
Fig. 8  Location of passivation cracking.

Physical analysis through Focused Ion Beam (FIB) cross  section found Aluminum metal migration with polyimide  delamination   and   passivation   cracking   (Fig.   9)   [6].   Commonality analysis determined that failures are systemic to a  specific assembly vendor.

![RBL   Defamination  P  Passivation crack  Diepassivation  Metal3  Electrochemical migration  Electrochemical migration   ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7415a50f-9094-4207-88f0-f6f22f8a0870/7415a50f-9094-4207-88f0-f6f22f8a0870.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=8fee212003321d101dc0d734b6569d4f0d5a6c62)
Fig. 9  FIB cross section showing Aluminum metal migration [6].

Materials analysis determined that the electrochemical  migration was caused by the assembly vendor’s flux residue  seeping into the polyimide delamination and accessing the  metal lines.  This resulted to electrochemical migration causing  leakage (the assembly defect model is shown in Fig. 10).

![Polyimide delam and   Polyimide delam and  fluxresidue filled in   fluxresidue filled in  Polyimide   Polyimide       Electrochemical migration  Electrochemical migration    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/68b5e09e-1b8f-490b-8218-f1c61e88aacb/68b5e09e-1b8f-490b-8218-f1c61e88aacb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=4bd51e605558ad9497e5f83b37d8c11b44f3689d)
Fig. 10  Assembly defect model causing the EIPD [6].

Further mechanical stress, voltage and moisture can  accelerate the mechanism and eventually result to the observed  EIPD (melted/burnt Silicon) when the device is powered up  within the specified AMR.  Thus, the earlier hypothesis that the  cause of failure is due to EOS from customer’s  application is  not true.

A new package qualification, using an I2C compliant Speaker  Amplifier IC as die source, encountered high failure rate after  Life Test. Initial failure analysis results showed high shutdown  current and exhibiting leakage on the Supply Pin with respect to  ground [7]. Physical analysis revealed gate oxide damage on a  transistor in the Load Drop Out (LDO) regulator circuitry (Fig.  11).   Several units were analyzed and a common failure  mechanism at the same circuit location was observed on the  failing   units.      Based   on   the   analysis   results,   the  conclusion/hypothesis is that the failure was caused by EOS  (test/application beyond the device’s AMR).  This hypothesis  however will be tested using the EOS investigation work flow.

![11/19/2018HV  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5f422949-d7ee-47bd-b163-3d91efe820e6/5f422949-d7ee-47bd-b163-3d91efe820e6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=0d738c0ad5b12389f7a1309b2972e995ceadc37a)
Fig. 11  Gate Oxide damage on an internal circuit block.

Mapping out the EOS investigation work flow, the observed  EIPD can be potentially caused by Wafer Fab Process or  possibly induced by external source during testing.  The failure  analysis results were then forwarded to the Wafer Fabrication  facility and based on their initial investigation and historical  check, the failure is systemic with only a specific transistor  being affected. In contrast, fabrication defects are typically  random. There was also no changes made on the wafer fab  process with no reported quality excursion from the field.  Hence, the observed gate oxide damage is less likely caused by  wafer fab process.

Reviewing the layout and schematics, it was determined that  the affected transistor has a direct path to the external Supply  pin (refer to Fig. 12). Hence, the damage is highly induced by  external source.

![Supply Pin  Supply Pin  LDO Output  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c4dc4793-d134-469a-99c6-c6dc07fb03b8/c4dc4793-d134-469a-99c6-c6dc07fb03b8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215668%3B1743219268&q-key-time=1743215668%3B1743219268&q-header-list=host&q-url-param-list=&q-signature=cf7a896930e8380ec0a36b8e8c00cf614c0c9303)
Fig. 12  Circuit analysis showing that the damaged component has direct path to  the Supply pin.

Further investigation of the reliability process found a  defective burn in socket which could cause high current event  and eventually being fed to the Supply pin.  The high current is  beyond the device’s absolute maximum rating, hence, the  observed EIPD was caused by an external source during testing.   Therefore the cause of failure as earlier hypothesized as EOS is  correct.

## V. CONCLUSION  

Having a standard industry-wide definition of EOS is an  important step to eliminate the misunderstanding and  misconception about EOS.  The term EIPD was a key  terminology that was found to be very useful to failure analysis.   This enabled the author to come up with a systematic work flow  to determine and confirm if the EIPD failures are really caused  by EOS or by intrinsic manufacturing defects.  Based on the  presented case studies, the failure analysis conclusion on the  cause of failure was found to be accurate and has provided  valuable details to conduct further investigation and  implementation of precise corrective and preventive measures.

EOS occurrences can be expensive to the entire supply chain  (OEM, system supplier, module supplier, and IC supplier) in  terms of time to resolve and opportunity cost. Thus, preventing  misdiagnosis of EOS can save customers and suppliers millions  of dollars by preventing wasted efforts for addressing the wrong  root causes. Through a systematic FA approach on potential  EOS failures, accurate FA conclusions can be made, hence, the  real cause of failure is addressed and effectively resolved.

## ACKNOWLEDGEMENT  

The author would like to thank Maxim Integrated Failure  Analysis management, namely Zhiyong Wang and Jerome  Escobedo.  To the MPOC FA Team with special thanks to  ECBU for embracing the EIPD concept and being open to  continuously improve the FA processes.

## REFERENCES  

[1]    T.L. Welsher, “Rethinking Electrical Overstress,”  www.ESDA.org   Featured Article , pp. 43-45, May 2016.     [2]    D.C. Wunsch and R.R. Bell, “Determination of Threshold Failure Levels  of Semiconductor Diodes and Transistors,”  IEEE Transactions on  Nuclear Science , Vol. 15, No. 6, pp. 244-259, December 1968.     [3]    K.T. Kaschani and R. Gaertner, “The Impact of Electrical Overstress on  the Design, Handling, and Application of Integrated Circuits,”  in  EOS/ESD Symposium,  2011.     [4]    ESD Council on ESD Target Levels, “White Paper 4: Understanding  Electrical Overstress-EOS,” pp. 3-57, August  2016.     [5]    C.M. Casabuena, “CFAR40081482,”  Maxim Integrated Failure Analysis ,  March 2017.    [6]    Z. Wang, ” Maxim VTxx Summary,”  Maxim Integrated , August 2017.    [7]    T.J. Bautista, “IFAR40107125,”  Maxim Integrated Failure Analysis ,  December 2018.

