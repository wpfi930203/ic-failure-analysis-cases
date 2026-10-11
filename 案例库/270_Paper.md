---
title: "270_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_d5a17c4aee3fb73e2e8ee5965901948d7295230462135641
file_size: 755638
---

## In-depth Analysis of 10 nm Exynos Processor using  Micro CT and FIB-SEM System  

Sharang S.¹, Jiri Dluhos², Dominika Kalasova³, Andrey Denisyuk², Rostislav Vana 1 , Tomas Zikmund 3 , Jozef Kaiser 3   and Jozef Vincenc Obona 2  1 TESCAN Brno s.r.o., Brno, Czech Republic  2 TESCAN ORSAY Holding a.s., Brno, Czech Republic.  3 CEITEC – Central European Institute of Technology, Brno University of Technology Brno, Czech Republic   \* Phone: +420-530-353-209   Email: sharang@tescan.com

Abstract-   Latest technology nodes have made finer, more  precise physical failure analysis techniques to emerge.  Conventional techniques for larger technology nodes are slowly  becoming ineffective. In this paper, we discuss effective yet  non-invasive technique like micro CT where we get high  fidelity images of the Exynos processor and complement it with  further analysis using FIB-SEM systems-based preparation  techniques like site-specific homogenous delayering, in-situ  probing and TEM lamella preparation which enables failure  analysis and reverse engineering techniques like nanoprobing  and TEM imaging possible.

–  Delayering, Micro CT, TEM, FIB-SEM, Nanoprobing

.

## I. I NTRODUCTION 

3D X-ray imaging popularly cited as Micro Tomography  (Micro CT) is an extension of Computerized Axial  Tomography (CAT scans) application used in medicine  industry but for relatively much smaller samples but with  highly improved resolution. Technique boasts of minimum to  no sample preparation required, is non-destructive and helps  capture a complete three-dimensional image. It renders a 3D  image in a single scan of the complete structure under  investigation. Major applications of a micro CT systems were  in medical and geological samples where it can help with their  imaging, 3D reconstruction, 3D visualization and quantification.  [2] It helps characterize samples how they come into being and  how they may fail with nanometer scale spatial resolution.

![Projected Image  Sample  X-RaySource  X-RayDetector  Rotating Stage    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/16208bc6-8a07-4780-9916-49e769fb782b/16208bc6-8a07-4780-9916-49e769fb782b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215679%3B1743219279&q-key-time=1743215679%3B1743219279&q-header-list=host&q-url-param-list=&q-signature=49356ac1e1c9ea011e0dc9b0af6092236e0678f6)
Fig. 1 – Working of a micro CT for imaging a processor chip

It works with the help of micro-focus X-ray source that

illuminates the sample. By rotating the sample in fraction of a  degree on a calibrated rotational stage after every X-ray image  captured on the X-ray detector as a 2D projection image. The  rotation of the sample can be to a complete 180 or 360 degrees  to acquire all the required facets of the sample. The acquired set  of projection images is put through computation for  cross-sectional images which can be further processed into 3D  models.

The ultimate resolution for these significantly larger fields of  view can be as low as 500 nm. On one hand it helps narrow  down the area of failure, but it does not offer sub-nanometer  scale signal for imaging structures like transistors MOS layer of  a semiconductor chip. FIB-SEM systems offer a plethora of  possibilities with relatively smaller fields of view (few   $\upmu\mathrm{m}$   to   ${\sim}1~\mathrm{mm})$   and ultimate resolution under 0.5 nm. Focused ion  beams allows us to perform various other applications other  than imaging like delayering and TEM lamella preparation.  This has now become one of the most important applications in  FA labs, they can do layer-by-layer investigation after  delayering with techniques like in-situ nanoprobing (Fig.2),  C-AFM and EBAC to find faulty circuitry and eventually  extract a thin lamella from the area of interest for further  angstrom scale TEM analysis. [1, 3]

![5oopm  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/23fc02c3-33ef-48f8-adaf-5186f27bba0d/23fc02c3-33ef-48f8-adaf-5186f27bba0d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215679%3B1743219279&q-key-time=1743215679%3B1743219279&q-header-list=host&q-url-param-list=&q-signature=3e2935c74631760f00db7eebc457d81eb0218e6d)
Fig. 2 – Kleindiek’s Nanoprober shuttle PS8 with four active probes  approaching the processor chip viewed under the SEM.

In this paper, we want to perform a teardown of 10 nm node  technology chip starting with micro CT over the complete chip  and then perform homogenous delayering and we will also  deliver TEM lamella preparation with both Xe plasma and Ga  FIB-SEM systems.

## II.   EXPERIMENTS   AND   RESULTS  

The device used in this study is a commercially available  processor. Exynos 8995 manufactured using the   $10\ \mathrm{~nm}$    technology node. The tomographic measurements were  performed (prior to decapsulation and mechanical polishing) in  X-ray micro and nano computed tomography laboratory of  Central European Institute of Technology, Brno University of  Technology (CEITEC BUT). The sample was scanned on a GE  phoenix v|tome|x L240 system, equipped with a   $240\;\mathrm{~kV~}$    microfocus   X-ray   tube   and   high-contrast   flat   panel  detector. The parameters of tomographic measurements were  set according to the size of the sample piece. The whole mobile  was scanned with   $180~\mathrm{keV}$   acceleration voltage,   $220~\upmu\mathrm{A}$   tube  current, 500 ms exposure time, 2000 images and the resulting  linear voxel size was  $90~\upmu\mathrm{m}$  . The small individual components  were scanned with   $160~\mathrm{keV}$   acceleration voltage,   $80~\upmu\mathrm{A}$  tube  current, 500 ms exposure time, 2300 images and the resulting  linear voxel size was   $10~\ensuremath{\upmu\mathrm{m}}.$  . The tomographic reconstruction  was realized using GE phoenix datos|x 2.0 software. 3D image  was rendered using the control software as can be seen in Fig. 3.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fdf774b5-23fe-490d-8e68-44a8d8cac9f2/fdf774b5-23fe-490d-8e68-44a8d8cac9f2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215679%3B1743219279&q-key-time=1743215679%3B1743219279&q-header-list=host&q-url-param-list=&q-signature=7c6fd731e4cee4f60a25afc75aef4e73682c5659)
Fig. 3 – Reconstructed 3D CT image of Exynos 8995.

Encapsulated chip’s micro CT helps investigate non-invasively  the chip for -

Functional inspection (possible electrical tests and  likely functional failures)       External inspection of the package      Internal inspection of the structure and the possible  need for invasive techniques.

The changing contrast is dependent on the density of  structures and the overall thickness of the packaged chip.

The chip was later de-capsulated and mechanically polished  for performing invasive applications like delayering. We  opened as Fig. 4 shows a   $100\times100~\upmu\mathrm{m}^{2}$   area opened using Xe  FIB by aligning the sample at analytical working distance to  SEM positioned orthogonal to the FIB. GIS was inserted to  inject A-Maze (TESCAN proprietary gas) on to the area of

interest. Suitable current density and beam shape was prepared  to conduce planarity in the presence of the gas chemistry and  the process was monitored using end point detection based on  the SE   signal being generated during the etching process.   The  end pointing recognizes each peak as the metal layer and the  trough as via layer which gives full control to the operator to  start and stop the process in any layer of interest. Xe plasma FIB  was used with   $15\,\mathrm{kV}$   beam energy and the process of delayering   $100~\upmu\mathrm{m}\mathrm{~x~}~100~\upmu\mathrm{m}$   from metal layer 8 down to transistor  contacts takes about 13 mins. Once in the layer of interest i.e.  the transistor contact layer we could perform in-situ  nanoprobing on MOS transistors (Fig. 4).

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/291bf7a6-afd9-43f3-9dd5-ff5562e43164/291bf7a6-afd9-43f3-9dd5-ff5562e43164.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215679%3B1743219279&q-key-time=1743215679%3B1743219279&q-header-list=host&q-url-param-list=&q-signature=6d4d63263487326694c0c2cd07a4cbe1720fd5e6)
Fig.  $4-500~\mathrm{eV}$   SEM image of  $100\times100\;\upmu\mathrm{m}$   window opened by FIB-GAE  delayering. (Scale of   $20\;\upmu\mathrm{m}$  )

Kleindiek Nanotechnik Prober Shuttle PS8 with 4 probes  carrying 10 nm diameter thin tips for easy access to the 10 nm  node technology was mounted into TESCAN’s S8000X with  Xe plasma FIB and potential tube based Ultra High Resolution  SEM column with low-KV imaging capabilities.  The  nanoprober sub-stage can be tilted to FIB working conditions  with easy “plug & play” installation procedure. PS8 sub-stage  allows sample motion in all three axes (10 mm, 10 mm, and 0.5  mm). Delayering is performed at   $55^{\circ}$   tilt, WD 6 mm and the  sample is positioned so that the delayering can be performed a  few millimeters from the probe needles. This tackles  re-deposition on the tips from delayering process. Nanoprobing  is performed at   $0^{\circ}$   tilt, WD around 3 mm and sub-stage with  sample moved below the probes.

Probe shuttle PS8 when used in-situ has many advantages – it  allows delayering and nanoprobing in one vacuum cycle,  sample is not exposed to external environment that can lead to  creation of an oxide layer as the sample is probed right after  delayering. Plasma cleaning can be used to further  decontaminate the chamber post delayering – a 5 min  decontamination cycle post delayering can tackle hydrocarbons  created as by-products can be efficiently eliminated from the  surroundings of area of interest.

Upon making stable mechanical and electrical contact with the  MOS transistors under measurement (Fig. 5a), we could  measure the I-V characteristics for both transistor types at  different gate voltages. Properly delayered surface has very low  ohmic resistance with no impeding layers created due to  adsorption of volatile hydrocarbons created as a by-product.  Current measured from the smooth curves with highest max.  current with range of  ${>}120~\upmu\mathrm{A}$   for both transistor types (Fig. 6).  [4]

Interesting cells were then extracted in the form of a lamella and  investigated under TEM (see Fig. 5b) to measure the pitch of  the FIN-FETs.  Lamellae were made with the gallium FIB and  the final thickness of under 15 nm was achieved.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fed9c03a-392c-4180-a6bd-5407a464e331/fed9c03a-392c-4180-a6bd-5407a464e331.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215679%3B1743219279&q-key-time=1743215679%3B1743219279&q-header-list=host&q-url-param-list=&q-signature=e15f0068d286af8bdf3e6df8307d9b0f842b64d7)
Fig. 5a) 500 eV SEM image of SRAM cells with nanoprobes (Scale of  $500\,\mathrm{nm}$  ),  b) TEM image of lamella depicting FIN-FET from 10 nm Exynos.

![IV-familyLC  11B4   gate0.249v  9.0E-5  gate0.498v  B.OE-5  gate0.747V  7.0E-5   gate0.996  S.OE-S.OE-5  4.0E-5  B.OE-   DateTP3  2.0E-1.0E-S  O1   0.2   0.3   0.4  ource-drainvoltage(V)  10E-S   sistorIV-familyLCT   nvalu  0.0E+0   ate-0.326V  10E-S   gate-0.650V  -2.0E-5   gate-0.954v  -3.0E-5   gate-1.236V  -4.0E-5  S.OE  SOE   atetp  -7.0E  B.OE-S  tartv:  9.0E-1.0E-0.8   04   G2  source-drainvoltage(V)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6578abf4-cf81-4f8f-a5ef-cb73865811de/6578abf4-cf81-4f8f-a5ef-cb73865811de.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215679%3B1743219279&q-key-time=1743215679%3B1743219279&q-header-list=host&q-url-param-list=&q-signature=cab23ec8631854e77f2e69402640c3fbf43949ef)
Fig. 6 I-V curves for a) NMOS transistor and b) PMOS transistor

A  $20\times20~\upmu\mathrm{m}^{2}$   block of area was also opened using Ga FIB to  uncovering transistor contacts with final planarity under 10 nm  RMS and accessibility to underlying layer architecture for  pattern recognition and detecting spyware circuitry.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7b3a7ce7-99bb-4d0d-9b65-839fee08651b/7b3a7ce7-99bb-4d0d-9b65-839fee08651b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215679%3B1743219279&q-key-time=1743215679%3B1743219279&q-header-list=host&q-url-param-list=&q-signature=26982f5b9ebc158d29f4941b73b2c4152004b06a)
Fig. 7 Gallium FIB delayered window edge size  $20\;\upmu\mathrm{m}$   down to transistors.

The method delivers significant advantages in terms of  localized, precise and layer-by-layer removal along with  constant monitoring using the acquired SE signal for end point  detection. The process is capable of performing delayering for  10-12 layers on sub-20 nm process nodes. Usual size of the area  exposed with delayering can be as big as   $20~\ensuremath{\upmu\mathrm{m}}$   and can be  achieved in about 12 minutes. It enhances the workflow  capability by enabling yet another application for a Ga FIB and  making a ‘must-have’ tool in semiconductor for physical failure  analysis as well as cyber-security applications.

## III.   CONCLUSION  

A holistic approach for FA labs and reverse engineering labs  starting with a complete encapsulated chip using Micro CT to  recognize the characteristics of failure across the encapsulated  chip. Eventually, opening it up for FIB-SEM based techniques  like delayering with in-situ nanoprobing and TEM lamella  preparation. Delayering was performed with both Xe plasma  and Ga FIB and their characteristic benefits were enlisted. Xe  plasma FIB based delayering with in-situ nanoprobing was also  described.  It enable extensive electrical analysis within a single  machine making it a workhorse tool for fast and reliable fault  isolation and analysis. Ga FIB based delayering enhances the  capability of gallium FIB as a workhorse in reverse engineering  labs.

## IV.   ACKNOWLEDGEMENTS  

This work was supported by project CEITEC 2020 (LQ1601)  with financial support from Ministry of Education, Youth and  Sports of the Czech Republic under the National Sustainability  Programme II and support of CEITEC Nano Research  Infrastructure (MEYS CR, 2016-2019).

## V.   REFERENCES  

[1]    D. Zudhistira  et al ., ”Precision Xe Plasma FIB delayering for Physical  Failure Analysis of sub-20 nm Microprocessor Devices”  ISTFA  Proceedings -  $\mathcal{43^{r d}}$  , pp. 574-579 , 2017.    [2]    V. Cnudde  et al. , “High resolution X-ray computed tomography in  geosciences: A review of current technology and applications”  Earth  Science Reviews 123 , pp. 1-17, 2013.    [3]    D. Zudhistira  et al ., “ Integration of Probing Capability into Plasma FIB  for In-situ Delayering, Defect Inspection, and EBAC on BEOL Defects  of sub-20 nm FinFET Devices”  ISTFA Proceedings -  $\mathcal{M}\mathcal{M}^{t h}$  , pp. 232-237  ,   2018.    [4]    M. Sikula  et al., ” SEM-based Nanoprobing on In-situ Delayered  Advanced 10 nm Technology Node IC”,  IPFA   Proceedings -   $25^{i h}$  ,  pp.  1-4 , 2018.

