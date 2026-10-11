---
title: "108_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_6aa39bd351d7a3b8db18f33ab9fdd67d7295230462135641
file_size: 1477573
---

## Scanning-TEM EDX Elemental Mapping Study and  Observations in Semiconductor Device Failure  

Analysis

Gek Li Lee, Jie Zhu  Corporate Quality, GLOBALFOUNDRIES Singapore Pte Ltd, 60 Woodlands Industrial Park D, Street 2, Singapore 738406  Phone : (+65) 6670-0243,   Email:  gekli.lee@globalfoundries.com

Abstract: Scanning-TEM EDX mapping has become a  mainstream analytical technique in semiconductor device  failure analysis as it offers fast elemental identification with high  spatial resolution. This is made possible with the technological  advancement in the silicon drift detectors (SDD) which replaces  conventional lithium-drifted silicon Si (Li) detectors. The higher  X-ray count rate from SDDs significantly reduces EDX mapping  collection time while improving the sensitivity of low atomic  weight elements. In this paper, we present some common  challenges that may happen during EDX analysis. These case  studies discuss problems with peak overlapping, signal  absorption, and beam-sensitive material. Through the findings  and observations of this study, we proposed strategies that can  be used to achieve better and more reliable EDX mapping  results .

Keywords — energy-dispersive X-ray spectroscopy, EDX  mapping, silicon drift detector ( keywords )

## I.    I NTRODUCTION  

In the semiconductor industry, Energy-dispersive X-ray  spectroscopy (EDX) is widely used in Failure Analysis (FA)  for elemental analysis of the devices. While there are other  commonly used techniques for X-ray analysis, EDX mapping  has become a mainstream analytical technique as significantly  better resolution maps have been attainable in recent years.  With the technological advancement in the silicon drift  detector (SDD) designs, there is an increased transition from  lithium-drifted silicon, Si (Li) detectors to SDDs in EDX  analysis. The new generation EDX detector has increased  solid angle (SA) which allows higher X-ray count rates within  a shorter time, one of the important criteria for better maps. Its  windowless designs further enhanced the EDX system’s  sensitivity for light element detection [1, 2]. These features are  especially critical for beam-sensitive materials. Furthermore,  the integrated data acquisition and signal processing  electronics   make it possible to collect and store the entire  spectrum at every pixel for post-data “mining” [3].

To maximize counts per second (CPS) for the acquisition  of EDX mapping data, Transmission Electron Microscopy  (TEM) settings such as gun lens, spot size, extraction voltage,  and condenser aperture need to be taken into consideration [4].  To obtain high CPS without sacrificing image resolution, all  parameters need to be optimized. Beam current could be  increased by reducing spot size and gun lens as well as by  increasing extraction voltage and condenser aperture size.

Despite relatively little effort being required in the  acquisition of STEM EDX maps, precautions during analysis  are necessary to avoid misinterpretations .   This work  demonstrated the data collection and analysis strategies that  can be used for achieving better and more reliable EDX  mapping results. We examined the various challenges  encountered in this study and delivered proposed solutions  through these findings.

## II.   E XPERIMENTAL 

In this work, EDX mapping analyses were carried out on  Tecnai F20 G2 TEM (Thermo Fisher Scientific) operated at   $200\mathrm{keV}$   acceleration voltage with Schottky type FEG. The  EDX maps were acquired using a large detection area   $(70\mathrm{mm}^{2})$   SDD detector (EDAX Elite T). TEM specimens  were prepared by dual-beam focused-ion beam microscope  (Helios450HP, Thermo Fisher Scientific).

## III.   R ESULTS AND DISCUSSION 

A.   Effect of EDX mapping time on counts and  copper/tantalum overlapping when analyzing Ta barrier

Copper (Cu) and Tantalum (Ta) are widely used for the  fabrication of interconnects at the back-end-of-line (BEOL)  processes. EDX analyses are often carried out for the  investigation of its failure in electrical performance. Since the   $\mathrm{Cu-K}_{\alpha}$   line   $(8.040\mathrm{keV})$   is closely spaced with the Ta-L α  line   $(8.145\mathrm{keV})$  ), the classic peak overlap issues posed a challenge  here. In this case study, we demonstrated that the Cu and Ta  overlapping issue is resolvable by using a longer acquisition  time. Collecting sufficient X-ray counts improves the signalto-noise ratio (SNR) of these EDX maps. This enables the  EDX system to discern peaks from the background and  specimen peaks from artifact peaks, thus rectifying peakoverlapping issues [5].

Fig. 1 compares the Oxygen-K, Cu-K, and Ta-L maps  acquired in 15, 30, 45, and 60 minutes, respectively. The  High-angle annular dark-field (HAADF) STEM images show  a sample with Cu via void. All elemental maps are   $\bar{2}56{\times}200$  pixels in size and were acquired by EDX with   $100\upmu\mathrm{s}$  dwell  time/pixel and drift correction. From the Ta map in Fig. 1(a),  we observed a weak contrast in the area where Cu is present  due to its stronger intensity influence.

This is verified by post-data analysis using the EDX  analysis system, TEAM™ software suite. By extracting an  area within the weak Ta contrast region from the EDX map,  we were able to analyze its element distribution. As suspected,  Ta element was not present. The Ta-L map acquired with the  longest time (60 minutes) as seen in Fig. 1(d) shows the most  well-defined elemental distribution of the Cu and Ta element.

The oxygen-K map further reveals that oxygen was  present at the Ta barrier around the via void area. This  confirms that Cu via void was due to the oxidized Ta barrier  which weakens the adhesion with subsequent Cu seed layer.

![(a)HADDFSTEM   (a) O-K  (a)Cu-k   (a)Ta-L  (b)HADDFSTEM   (b) O-K  (b)Cu-k   (b)Ta-L  ()HADDFSTEM   (c) O-K  (c)Cu-k   (c) Ta-L  （d)HADDFSTEM   (d) O-K  (d)Cu-k   (d)Ta-L  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2ba002bb-aefd-48af-9820-3b076c3719f3/2ba002bb-aefd-48af-9820-3b076c3719f3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=184372f95c604a20b4f67c1331fbf11615b2aaa5)
Fig. 1.   Cu Via HAADF STEM images and respective EDX Oxygen-K,  Cu-K, and Ta-L maps acquired in (a) 15 minutes (b) 30 minutes (c) 45  minutes (d) 60 minutes.

## B.   Pt-L and Ta-L peak overlapping   

Fig. 2 displays several elemental maps of selected  elements from a SRAM failure analysis. All elemental maps  are   $256{\times}200$   pixels in size and were acquired simultaneously  by EDX with   $100\upmu\mathrm{s}$   dwell time/pixel and drift correction in  \~60mins. The EDX mapping result shows a contact void at the  failing bit. Cu from metal 1 layer has filled into the empty  contact. We observed the result from the Platinum (Pt) map  was not accurately exhibited, showing a weak contrast in the  area where Ta was present.

It is interesting to note that based on the observations from  the first case study, we used longer acquisition time to achieve  better count rates. However, it was still insufficient to  distinguish between Ta and Pt distribution successfully from  these EDX maps. After closer examination of the map sum  spectrum, we noticed that the Ta-  $\cdot\mathrm{{L}}_{\upbeta}$    line was closely spaced  with the   $\mathrm{Pt-L}_{a}$   line (9.441keV). Since Pt has another  characteristic  $\mathbf{M}_{\alpha}$   line (2.048keV) we had chosen this line to

rebuild the EDX maps [6]. The result revealed a noticeable  improvement in the accuracy of Pt element distribution as  shown in Fig. 2(e).

Here, we also observed that in the first case study, Ta-L α2   $(8.089\;\mathrm{keV})$   and   $\mathrm{Cu-K}_{\alpha1}$   (  $8.048~\mathrm{keV})$   lines were further apart  at   $0.041\mathrm{keV}$  . In addition, both Cu/Ta elements were in  abundance and the peak overlapping could be resolved with  sufficient X-ray counts acquired to allow successful  differentiation of the signals. As compared to the second case  study,   $\mathrm{Pt-L}_{\alpha2}$   (9.364keV) and Ta-L β1  (9.345keV) lines were  only   $0.019\mathrm{keV}$   apart, as shown in Fig. 3. Besides, the  concentration of Ta and Pt was relatively low too. This could  potentially make the map reconstruction process more  challenging.

Fab had feedback that the contact void had happened  during the chemical mechanical polishing step which  matched with the EDX results whereby Cu overflowed into  the contact void location.

![(b) Cu-k   (c)Ta-L  (a)HADDFSTEM  (d) Pt-L   (e)Pt-M  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c44944da-bc63-4107-87d9-60f5c6ee49c8/c44944da-bc63-4107-87d9-60f5c6ee49c8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=c713fce369633a7c5145da0881b7650493bf2fff)
Fig. 2.   Contact HAADF STEM images and respective EDX Cu-K, Ta-L,  Pt-L, and Pt-M maps.

## C.   Blocking/absorption effect from sample to detector  orientation  

Another common challenge faced when performing EDX  mapping is the X-ray detector blocking/absorption effect.  Ideally, the TEM lamella’s interface should be parallel to the  detector axis and the beam to improve the path between the  specimen and detector. This will increase the effective solid  angle and more X-rays will be collected [7]. However, in the  opposite scenario, low-energy X-rays could hit the edge of  the sample holder creating more stray peaks or block by the  feature on the specimen and not have enough energy to  penetrate through. They are being absorbed by the sample  holder or the specimen. As for higher energy X-rays, they are  not affected by this absorption effect. Therefore, this affects  only light element detection, especially Nitrogen (N)  element.

![ca  (a)  65.7K  CuKa18.048  CuKo1  584K  51.1K   TaLα18.147  43J8K  B6L5K  29.2K  CuKα28.028  21-9K  4L6K  TaLa28.089    b  (b)  PtLα19.439  TaLβ19.345  TaLβ29.649  Ta LB1  GaKa1   LOT  9.08   9.26   Pt Lα29.3649.44   9.62  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6956bf88-45f7-4655-a178-00a4a503b8fa/6956bf88-45f7-4655-a178-00a4a503b8fa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=d7dddd129c495c335d1b33a5ff1b968e86110b27)
Fig. 3.   (a) EDX sum spectrum of the map showing Ta  $\cdot\mathrm{L}_{02}$     $8.089\;\mathrm{keV})$   and  $\mathrm{Cu-K}_{u1}$     $3.048~\mathrm{keV}$  ) line overlap area, (b) EDX sum spectrum of the  map, insert is the magnified of Pt-Lα2   $(9.364\mathrm{keV})$   and Ta-Lβ1   $(9.345\mathrm{keV})$  ) line overlap area.

Fig. 4 displays the elemental maps from a Cu bump  defect. All elemental maps are   $256{\times}200$   pixels in size and  were acquired simultaneously by EDX with   $100\upmu\mathrm{s}$   dwell  time/pixel and drift correction in 60mins. Based on the TEM  brightfield image, it was inferred that the NBLOCK layer  would follow the Cu bump profile. However, from the EDX  maps, the NBLOCK layer was not visible. As such, it was  highly suspected this was caused by the blocking or  absorption effect from the detector. To verify this  assumption, we reloaded the holder with the grid rotated at   ${\sim}180$   degrees.

The second set of results revealed an improved resolution  on the N, O, and C maps as shown in Fig. 5. All elemental  maps are   $256{\times}200$   pixels in size and were acquired  simultaneously by EDX with  $100\upmu\mathrm{s}$   dwell time/pixel and drift  correction in 60mins. Due to good agreements between the  TEM and EDX mapping results, it was concluded that the  root cause of the defect was due to Cu migration signature.

By rotating the sample to face toward the detector, the  absorption effect is greatly reduced, allowing the X-ray  collection process to be substantially improved. This is  illustrated in Fig. 6.

With the latest EDX system technology, this limitation  has since been improved immensely with a double detector  or in a more advanced system, 4 detectors.

![(a) HADDF STEM   (b) Cu-K  (c) Si-K   (d) N-K  (e)O-K   (f C-K  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4755d598-3b66-4732-85eb-e5e80a283b1a/4755d598-3b66-4732-85eb-e5e80a283b1a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=2aa3157456714d48a835ca339e818db50fd23c06)
Fig. 4.   Cu bump  HAADF STEM image and respective EDX Cu-K, Si-K,  N-K, O-K  and C-K maps at first EDX mapping attempt.

![(a) HADDF STEM   (b) Cu-K  (c) Si-K   (d)N-K  (e) O-K   (f C-K  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/167bfa64-8a67-4620-b8ef-4d789dd3ae5c/167bfa64-8a67-4620-b8ef-4d789dd3ae5c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=ebca493366683628c56476cb12fbfac61d061edf)
Fig. 5.   Cu bump  HAADF STEM image and respective EDX Cu-K, Si-K,  N-K, O-K  and C-K maps after grid rotation at  $\mathord{\sim}180$   degrees.

![EDXdetectol  (a)  EDXdetector  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d59ecf21-63ba-42b6-8f0d-6411cb6547d7/d59ecf21-63ba-42b6-8f0d-6411cb6547d7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=4ad89eb61dc73f126ecc25cea2a1fa506d590f16)
Fig. 6.   (a) Orientation of EDX detector with respect to the specimen  during the first EDX mapping attempt. (b) Orientation of EDX detector  after rotating the grid at   ${\sim}180$   degrees.

## D.   Beam-sensitive material analysis  

Due to the improved sensitivity of SDD, fast EDX map  acquisition has become achievable. High-speed EDX  mapping not only boosts efficiency but also minimizes beam  damage to the samples. Post-data analysis can be carried out  in detail after the data is collected.

This application is illustrated in the following device  delamination issue, shown in Fig. 7. The EDX linescan  acquired by the old Si (Li) detector was unable to distinguish  the material difference across the abnormal layer due to  sample damage caused by long dwell time (1 second/point) as  shown in Fig. 8. With the new SDD, beam damage is  significantly reduced as the dwell time/point is reduced from  1s to 50us. The EDX mapping result revealed a thin Si-rich  layer as shown in Fig. 9(a). The extracted line profile as shown  in Fig. 9(b) also reaffirmed the finding. All elemental maps  are   $200\!\times\!120$   pixels in size and were acquired simultaneously  by EDX with   $50\upmu\mathrm{s}$   dwell time/pixel and drift correction in  15mins.

This finding has enabled Fab to correlate the case with a  Silane burst incident from the chamber, allowing the proper  action to be taken.

![Delamination  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fff4a985-a81c-4461-af05-ae61c214684b/fff4a985-a81c-4461-af05-ae61c214684b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=5e0d64e70de8ed3cb2f42f49f603f6b8a5d6239f)
Fig. 7.   HAADF STEM image of a device with delamination issue.

![a 七 Beam Abnormal  damage layer  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/329d56ab-d735-416f-8182-998d3d939168/329d56ab-d735-416f-8182-998d3d939168.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=eb4fea892c2f4f70a568bcf03a84063f48127ce0)
Fig. 8.   (a) EDX linescan result across the residue layer, (b) HAADF  STEM image showing beam damage after the EDX linescan acquisition.

![O-K  a  SiiK   Si rich layer  HAADFSTEM  Cb  Oxygen profile  Siprofile  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c37dcc15-ccf7-4cc5-8022-95312e98bd9e/c37dcc15-ccf7-4cc5-8022-95312e98bd9e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215819%3B1743219419&q-key-time=1743215819%3B1743219419&q-header-list=host&q-url-param-list=&q-signature=8671e8adf6c8a36e16c009ee6028544b4de83007)
Fig. 9.   (a) HAADF STEM image and respective EDX O-K and Si-K  map  of the abnormal layer, (b) extracted line profile from the EDX map.

## IV.   C ONCLUSION   

The work presented in this paper discusses the application  of STEM EDX mapping in semiconductor device failure  analysis. Through these case studies, we proposed solutions  for some of the common challenges in EDX mapping analysis  related to peak overlapping, signal absorption and beam  damage on sensitive material.

In the first two case studies, we discussed the peaks  overlapping issues. Depending on the elements that are  affected, this can be addressed through longer data acquisition  time to achieve high-SNR EDX maps or by selecting an  alternative X-ray line energy for data reconstruction. For  optimal EDX mapping results, proper sample tilting is another  crucial factor, especially in light element detection as  explained in the third case study. This ensures there are  sufficient count rates by minimizing the detector blocking or  absorption effect. In the last case study, we validated that with  the high X-ray collection efficiency of the detector, fast  acquisition of EDX data was beneficial in the detection of  beam-sensitive material.

Although EDX data collection is made straightforward  with the assistance of modern technologies, analysts’  interference and experience are still needed in complex failure  analysis. One needs to understand how the results obtained are  derived to correctly interpret   the information. Ambiguity  could arise during the data acquisition and processing stages.  As such, appropriate techniques should be employed to  counter it.

## A CKNOWLEDGEMENT 

The   authors   acknowledge   the   support   from  GlobalFoundries’ Corporate Quality management in this  work. The authors thank the four anonymous reviewers and  the mentor for their valuable comments and corrections. Some  of their original comments have been incorporated into the  paper.

## R EFERENCES   

[1]    Elite T EDS System Product Bulletin.   $\copyright$   EDAX Inc., 2019 July.    [2]    K Tamura, R Namekawa, R Buchhold, B Hammell, A Sandborg, T  Sato, M Konno, H Inada, K Nakamura, Y Taniguchi, T Hashimoto, The  Development of A Large-Area Windowless Energy Dispersive X-ray  Detector for STEM-EDX Analysis, Microscopy and Microanalysis,  Volume 19, Issue S2, 1 August 2013, Pages 1192–1193,  https://doi.org/10.1017/S1431927613007952.    [3]    Friel JJ, Lyman CE. Tutorial Review: X-ray Mapping in ElectronBeam Instruments. Microscopy and Microanalysis. 2006;12(1):2-25.  doi:10.1017/S1431927606060211    [4]    Ming Q. Chu, Department of Metallurgy and Materials, University of  Birmingham, UK.  Microscopy and Analysis 24(2):11-14 (EU),2010:  Analytical TEM of Materials using a Large Area Silicon Drift EDS  Detector.    [5]    D. B. Williams and C. B. Carter, Transmission Electron Microscopy:  A Textbook for Materials Science, 2nd ed. (Springer, New York, USA,  2009), pp. 626 - 627.    [6]    J. Zhu, Y. Q. Shen and S. P. Zhao, "Chemical analysis of  semiconductor   devices   using   TEM   energy-dispersive   X-ray  spectroscopy (EDS) and electron energy-loss spectroscopy (EELS),"  2016 IEEE 23rd International Symposium on the Physical and Failure  Analysis of Integrated Circuits (IPFA), 2016, pp. 86-93, doi:  10.1109/IPFA.2016.7564254.    [7]    Zaluzec, N. (2014). Analytical Formulae for Calculation of X-Ray  Detector Solid Angles in the Scanning and Scanning/Transmission  Analytical   Electron   Microscope. Microscopy   and  Microanalysis, 20(4), 1318-1326. doi:10.1017/S1431927614000956.

