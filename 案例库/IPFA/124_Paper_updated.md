---
title: "124_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_fa2c608167ea5e0e9f271d00193b95b87295230462135641
file_size: 1969598
---

## Fluorocarbon Film Deposition Using Reactive Ion  Etcher and Its Application for Physical Analysis of  3D Stacking TSV, Micro Bump and Hybrid Bonding  

Chih-Ming LEE 1 , Hsiu-Pin CHEN 1 , Yu-Chen CHANG 1,2 , Wan-Kang HSIEH 1 , Li-Heng KAO 2  1 Failure Analysis Department, Winbond Electronics Corporation, Kaohsiung City, Taiwan  2 Department of Chemical and Materials Engineering, National Kaohsiung University of Science and Technology, Kaohsiung City, Taiwan  Phone : (+886)7-6278168, Email :  hpchen9@winbond.com

Abstract —Through-silicon via (TSV), micro bump, and  hybrid bonding are three critical structures for threedimensional (3D) integrated circuits (IC) stacking technology.  The large-scale (\~um level) feature size will be the challenge for  conventional physical analysis and the development of new  techniques must be considered. During the sample preparation  process in focused ion beam (FIB), a protection layer deposition  is necessary to avoid the damage by subsequent ion milling,  especially for samples where the region of interest (ROI) is on  the surface. It consumes time and only small area is capable due  to the low deposition rate in FIB. Besides, the material contrast  in scanning electron microscope (SEM) images is low if only  metallic precursors in FIB can be selected. Therefore, a new  protection layer which is non-metallic material and can be  deposited over a large area is considered.    This paper  investigates the possibility of fluorocarbon film deposition  utilizing the reactive ion etcher (RIE) as a new option for the  protection layer. The precursor trifluoromethane (CHF 3 ) is  generally used for silicon oxide etching in RIE. However, the  literature indicates that it can also be used for fluorocarbon film  deposition under specific process conditions. The experiment  results show that the fluorocarbon film can be deposited  successfully in RIE using CHF 3  without oxygen (O 2 ). Lower  radio frequency (RF) power and higher chamber pressure  enhance the deposition rate. The profile can be observed by  SEM images and energy dispersive spectroscopy (EDS) verified  the existence of carbon and fluorine compounds on the surface.  The fluorocarbon film is further applied as the protection layer  on TSV, micro bump and hybrid bonding samples for  subsequent FIB cross-sectional preparation. It not only saves the  deposition time in FIB, but also provides high transparency for  target navigation by top view and better material contrast for  cross-sectional images. This study successfully develops a new  technique for physical analysis in 3D stacking technology and  creates a deposition function on the etching tool, which is a  significant achievement in the physical and failure analysis  laboratory.

Keywords—TSV, micro bump, hybrid bonding, fluorocarbon  film, trifluoromethane, RIE

## I.    I NTRODUCTION 

The era of artificial intelligence (AI) computing drives the  demand for high-density, high-speed, and high-bandwidth  memory (HBM). However, semiconductor process shrinkage  has reached its physical limitations. Therefore, threedimensional (3D) integrated circuits (IC) stacking technology  has become the new solution. It includes three critical  structures: through-silicon via (TSV), micro bump, and hybrid  bonding, which can reduce the package size and shorten the  data path compared to conventional wire-bonding and  packaging technologies. However, the large-scale (\~um level)  feature size is the challenge for physical analysis, as the  conventional techniques are designed for small-scale (\~nm

level) feature size with high imaging resolution and high  targeting accuracy. Therefore, it is necessary to consider and  develop new physical analysis techniques for these structures.

In the laboratory, focused ion beam (FIB) is utilized to  prepare samples for cross-section profile observation and  element identification by scanning electron microscope  (SEM), especially for specific locations that require accurate  targeting and cannot be approached by random polishing. A  protection layer deposition on sample surface is necessary to  avoid the damage during subsequent ion milling in FIB,  especially for samples where the region of interest (ROI) is on  the surface.

The conventional technique of protection layer deposition  is performed directly in FIB. However, it consumes time and  only small area deposition is applicable due to low FIB  deposition rate. In addition, the SEM image shows low  material contrast between the protection layer and sample  surface if only platinum (Pt) precursor can be selected in FIB  because the sample surfaces of TSV, micro bump and hybrid  bonding are metal-based materials, such as copper (Cu) and  aluminium (Al).

To solve the above problems, other types of protection  layers are considered. Plasma-enhanced chemical vapor  deposition (PECVD) is one of the options. It can deposit  silicon oxide and silicon nitride as the protection layers, but it  incurs additional costs to purchase the tool. Therefore, the  purpose of this paper is to develop a new protection layer  which is a non-metallic material and can be deposited over a  large area using the existing reactive ion etching tools.

## II.   L ITERATURE  R EVIEW 

## A.   Reactive Ion Etching  

Reactive ion etcher (RIE) is one of the dry etch tools in the  semiconductor manufacturing process. In the laboratory, RIE  is applied for delayering during sample preparation.  Generally, the main precursors include trifluoromethane  (CHF 3 ), tetrafluoromethane (CF 4 ), and sulfur hexafluoride  (SF 6 ).  ${\mathrm{CHF}}_{3}$   and   $\mathrm{CF_{4}}$   are utilized for silicon oxide   $\mathrm{(SiO_{2})}$   and  silicon nitride (Si 3 N 4 ) removal, while SF 6  is applied for  tungsten (W) and silicon (Si) etching. For the etching recipes,  these precursors are used in combination with oxygen   $(\mathrm{O}_{2})$  because the presence of   $\mathrm{O}_{2}$  can enhance the formation of  fluorine (F) radicals to speed up the etching reaction [1].

The above precursors have different atom ratios,  F/(C,H,S), as shown in Table I. The literature points out that  the precursors with lower atom ratios of F/(C,H,S) will also  induce the formation of fluorine compounds during the  etching reaction. This means that the deposition behavior is  achievable via the selection of precursors and the control of

reaction parameters in the RIE tool, especially for CHF 3  with  the lowest atom ratio in the range of   $2{>}\mathrm{F}/(\mathrm{C,H,S}){>}0$  . This is  because the lower atom ratio of F/(C,H,S) will induce a higher  network or cross-linking structure [2].

TABLE I.     A TOM  R ATIOS OF  T HE  P RECURSORS

|Precursors|Atom Ratio: F/(C,H,S)|
|---|---|
|Trifluoromethane (CHF 3 )|1.5|
|Tetrafluoromethane (CF 4 )|4|
|Sulfur hexafluoride (SF 6 )|6|


## B.   3D IC Stacking Technology  

TSV is a high aspect ratio contact structure that passes  through the silicon substrate for the internal vertical electrical  connection of stacked chips. A classic TSV structure is shown  in Fig. 1 [3], the contact profile is etched and filled with Cu,  followed by chemical-mechanical polishing (CMP) to isolate  the contacts. The Cu gap-filling ability and grain size, as well  as the flatness of the Cu after CMP, are the focus of  observation in physical analysis.

![Si substrate  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/86c00cec-ebc0-4305-8d30-7a9f872088a6/86c00cec-ebc0-4305-8d30-7a9f872088a6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215841%3B1743219441&q-key-time=1743215841%3B1743219441&q-header-list=host&q-url-param-list=&q-signature=a9b0205c73563bdcd5958572fe187aba49228238)
Fig. 1.   TSV (post-CMP): (a) tilt view; (b) cross-section view [3].

Micro bump is a pad-to-pad solder bump that creates an  external electrical connection between stacked chips. The  schematic diagram of a micro bump is illustrated in Fig. 2 [4].  The size of micro bumps is much smaller than that of  conventional solder bumps, allowing for higher density  connections. The main problem encountered in physical  analysis is that the observation range is in the tens of  micrometers, which requires a large area of the protection  layer.

![Micro-bump  TV-2l  →Micro-bump  TsVdevice  orinterposer  TSVdeviceorTsVinterposer   Micro-bump  FlipChip  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/972c2c1c-7902-453c-88d4-35dbadd94389/972c2c1c-7902-453c-88d4-35dbadd94389.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215841%3B1743219441&q-key-time=1743215841%3B1743219441&q-header-list=host&q-url-param-list=&q-signature=0d3b361f6e12e5c0081bea5c3115a67dd2503c30)
Fig. 2.   Micro bump: various package types illustration [4].

Hybrid bonding is a new concept for stacked chip  interconnection, which bonds Cu pads between chips directly  by thermal compression bonding (TCB) instead of micro  bumps. An example of hybrid bonding is shown in Fig. 3 [5].  Because there is no solder bump between pads, the resistance  is lower. However, hybrid bonding is a direct bonding of chipto-wafer or wafer-to-wafer, where the accuracy of pad-to-pad  alignment is very critical. In addition, the dishing of Cu on the  surface after CMP will affect the bonding success rate.

![CC  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/272b33d1-7833-4a75-a4a0-b43fccb51e80/272b33d1-7833-4a75-a4a0-b43fccb51e80.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215841%3B1743219441&q-key-time=1743215841%3B1743219441&q-header-list=host&q-url-param-list=&q-signature=7c558c3786a890e53785f83bf89a64b4513cf5f1)
Fig. 3.   Hybrid bonding: (a) overview; (b) left side; (c) right side [5].

All the above structures are large-scale (\~um level) and  most of the in-process wafers come from etching and CMP  processes with exposed Cu and Al. Therefore, a large area  protection layer is necessary for physical analysis in 3D  stacking technology.

## III.   E XPERIMENTAL  M ETHOD   

Based on the above research, this paper investigates the  possibility of fluorocarbon film deposition utilizing the  reactive ion etching tool. The deposition experiments are  carried out on Trion Phantom III RIE using silicon oxide   $\mathrm{(SiO_{2})}$   samples to evaluate the effects of different gas flow  rates, radio frequency (RF) power, chamber pressure, and  process time. To verify the deposition results, the sample  surface is inspected by Olympus BX53M optical microscope  (OM). Cross-section and top view images are observed on  Hitachi SU8240 SEM, which is also equipped with Oxford  Aztec energy dispersive spectroscopy (EDS) for elemental  identification to confirm the existence of the fluorocarbon  films. Fourier transform infrared (FTIR) and X-ray  photoelectron spectroscopy (XPS) are performed by  PerkinElmer Spectrum 3 and PHI VersaProbe4, respectively,  to investigate their chemical composition. The   $\mathrm{SiO}_{2}$   samples  come from bare silicon wafers with additional silicon oxide  deposition (  $(2400{\scriptstyle\pm20\;\mathrm{nm}})$  ).

The optimized fluorocarbon film deposition conditions are  further applied to TSV, micro bump, and hybrid bonding  samples as protection layers. The application results are  compared with the conventional technique of in-FIB platinum  deposition. ThermoFisher Helios 5EX FIB is used to prepare  the cross-sections and evaluate the electrical conductivity of  the samples. The TSV samples are etched through-silicon vias  with copper filling and have been planarized by chemicalmechanical polishing (CMP). The micro bump samples have  completed the entire fabrication process with Al pads

exposed, and the hybrid bonding samples are also post-CMP  wafers after Cu deposition on etched patterns.

## IV.   R ESULT AND  D ISCUSSION 

## A.   Fluorocarbon Films Deposition  

1)   Effect of   $O_{2}$   Content:  Gas mixtures of   $\mathrm{CHF}_{3}/\mathrm{O}_{2}$   are  widely used for etching. To evaluate the effect of   $\mathrm{O}_{2}$   content  on deposition, the first investigation for deposition is on  different  $\mathrm{CHF}_{3}/\mathrm{O}_{2}$   flow rate ratio, as shown in Fig. 4. SEM  images illustrate the phenomena from etching to deposition  by measuring the silicon oxide remains. Fig. 5 suggests that  higher O 2  flow rate enhances the etching process, resulting in  less silicon oxide remains until the   $\mathrm{O}_{2}$   flow rate exceeds   $2\mathbf{X}$    SCCM (with the  ${\mathrm{CHF}}_{3}$   flow rate fixed at 10x SCCM). This  result indicates that the optimal   $\mathrm{CHF}_{3}/\mathrm{O}_{2}$   flow rate ratio for  etching is approximately 10:2. This is because low  $\mathrm{O}_{2}$   content  can enhance the F   radicals for etching, but high   $\mathrm{O}_{2}$   content  will lead to the dilution of F   radicals in the chamber [1].  Besides the etching behavior, it is notable that the deposition  of the fluorocarbon film occurs when the   $\mathrm{O}_{2}$   flow rate is  reduced to 0 SCCM.

![02=4xSCCM   O2=2xSCCM   O2=1xSCCM   O2=0SCCM  Etching   Etching   Etching   Deposition  SiO2   2,196nm   SiO2   2,360nm  SiOz   2,048nm   SiO2   2,058nm  CHF:O2=10:4   CHF:O2=10:2   CHF:O2=10:1   CHF:O2=10:0  Etchin   Etching   Etching   position  CHF3=10xSCCM;RFpower=20yW;Pressure=35zmT  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1b9543fb-c470-4e00-b6df-f7866ee7a4be/1b9543fb-c470-4e00-b6df-f7866ee7a4be.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215841%3B1743219441&q-key-time=1743215841%3B1743219441&q-header-list=host&q-url-param-list=&q-signature=9172be891c882696b4e50a7c6ddf6d29264ddfaa)
Fig. 4.   Fluorocarbon film deposition by different  $\mathrm{O}_{2}$   content.

![2400  2350  2300  uuu  2250  2200  pixo   2150  2100  2050  2000  02=4xSCCM   02=2xSCCM   02=1xSCCM   02=0xSCCM  CHF=10xSCCM  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/664bb76b-5c9f-43f0-ab4d-095a6070b1c1/664bb76b-5c9f-43f0-ab4d-095a6070b1c1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215841%3B1743219441&q-key-time=1743215841%3B1743219441&q-header-list=host&q-url-param-list=&q-signature=4f9156e7a083975ec68c2fc01e926f736b776bcb)
Fig. 5.   Silicon oxide remains distribution by different  $\mathrm{O}_{2}$   content.

2)   Chemical Composition:  The existence of the  fluorocarbon film is verified by EDS analysis. As  summarized in Table II, the elemental weight percentages of  carbon (C) and fluorine (F) are significantly higher for the  sample with  $\mathrm{O}_{2}=0$   SCCM compared to the other samples.

The FTIR spectrum shown in Fig. 6 is further analyzed to  investigate the chemical bonding. The characteristic peaks at   $1720\,\mathrm{cm}^{-1}$   (  $\scriptstyle\mathrm{C}=\mathrm{CF}_{2}$  ,   $1220{\cdot}1160\,\mathrm{cm}^{\cdot1}\left(\mathrm{CF}_{2}\right)$  , and   $730\,\mathrm{cm}^{\ensuremath{-}1}$   (CFCF 3 ) are identified [6]. The XPS spectrum is presented in Fig.  7. The distribution of the C 1s peak corresponding to the  binding energies of   $280{-}300\ \ \mathrm{eV}$   indicates that   $\mathrm{CF}_{2} $  is  dominant [2] in the fluorocarbon film sample.

TABLE II.     EDS  WEIGHT PERCENTAGE BY DIFFERENT  O2  CONTENT .

||O 2 =4x SCCM|O 2 =2x SCCM|O 2 =1x SCCM|O 2 =0 SCCM|
|---|---|---|---|---|
|C|0.65%|1.08%|1.09%|64.96%|
|O|50.52%|49.17%|50.42%|17.13%|
|F|3.02%|3.07%|1.89%|13.28%|
|Si|45.81%|46.68%|46.60%|4.63%|


![1220-1160  80-  60  730  )uond   40   1720  20-  O一  2000   1800   1600   1400   1200   1000   800   600  Wavenumber (cm -1)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ed230496-17de-479a-8dad-8a19422e9320/ed230496-17de-479a-8dad-8a19422e9320.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215841%3B1743219441&q-key-time=1743215841%3B1743219441&q-header-list=host&q-url-param-list=&q-signature=4d0abf00282ce2c134e149d64d2678e39bd15d41)
Fig. 6.   FTIR spectrum   for the fluorocarbon film sample.

![Atomic%  F1S   F1s85.0  8112  C1speakdistribution  01S   C1S  1400   1200   1000   B0O   SOO   200  Binding Energy (eV)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/253a3cf7-e4f4-4655-9088-cc4897cdddcf/253a3cf7-e4f4-4655-9088-cc4897cdddcf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215841%3B1743219441&q-key-time=1743215841%3B1743219441&q-header-list=host&q-url-param-list=&q-signature=6041da4fec732388d81b68a2cb6b8b02bb8736a4)
Fig. 7.   XPS spectrum   for the fluorocarbon film sample.

3)   Effect of RF Power and Chamber Pressure:  RF power  and chamber pressure are two critical parameters for etching.  To evaluate the difference of process conditions between  etching and deposition, the second investigation for  deposition is on different RF power and chamber pressure, as  shown in Fig. 8. SEM images illustrate that deposition is  formed for all chamber pressure conditions at RF power of  10y W, and the silicon oxide loss is the least at chamber  pressure of  $35z\,\mathrm{mT}$  . This result indicates that lower RF power  and higher chamber pressure are beneficial for deposition,  whereas higher RF power and lower chamber pressure  promote etching. It is supposed that the lower RF power

decreases the   $\mathrm{CHF}_{3}$   ionization and dissociation to inhibit the  etching rate [1] and higher chamber pressure increases the  concentration of   ${\mathrm{CHF}}_{3}$   for fluorocarbon films formation.

![RFpower=10yW   RFpower=20yW   RFpower=30yW  2S2  S1O2   3701  SiOz   180n  89  Sioz   2,360nm   SiO2   2.2171  sio2   942  SiOz  2,387nm   s102   2,360n  sio   2.006  CHF=10xSCCM;O=0SCCM  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5636bf42-7bf7-4222-ba31-e9b9a5edad67/5636bf42-7bf7-4222-ba31-e9b9a5edad67.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215841%3B1743219441&q-key-time=1743215841%3B1743219441&q-header-list=host&q-url-param-list=&q-signature=fe5f7ae7710fc0462eb351cf304d4731d81f998c)
Fig. 8.   Fluorocarbon film deposition by different RF power and pressure.

4)   Effect of CHF 3  Flow Rate:  The CHF 3  flow rate  correlates with the concentration of the precursor in the  chamber during the process. To evaluate the effect of the  CHF 3  flow rate on deposition performance, which is judged  by higher fluorocarbon film thickness and less silicon oxide  loss to maintain the original physical profile, the third  investigation for deposition is on different CHF 3  flow rates,  as shown in Fig. 9. SEM images show higher fluorocarbon  film thickness with less silicon oxide loss at  ${\mathrm{CHF}}_{3}$   flow rate  of 30x SCCM. This result indicates that higher CHF 3  flow  rate can increase the thickness of the fluorocarbon film and  decrease the silicon oxide loss.

![CHF=10xS  SiO2   2,387n   SiO2   2,390n   SiOz   2400  135nm  62nm   95nm  O=0SCCM;RFpower=10yW;Pressure=35zmT  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c40fc8a2-48dc-4c3d-b30b-abd133973ec0/c40fc8a2-48dc-4c3d-b30b-abd133973ec0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215841%3B1743219441&q-key-time=1743215841%3B1743219441&q-header-list=host&q-url-param-list=&q-signature=9570ac4152e45e86595c63add15bc3c405c599e6)
Fig. 9.   Fuorocarbon film deposition by different CHF 3  flow rate.

5)   Process Time and Modelling:  The fluorocarbon film  thickness can be controlled by the process time. To establish  a mathematical model of the deposition rate versus process  time as a reference for practical applications, the fourth  investigation for deposition is on different process times, as  shown in Fig. 10. SEM images illustrate that the fluorocarbon  film thickness increases with the process time, and the trend  chart is shown in Fig. 11. It shows a linear correlation. The  linear fitting equation quantifies the deposition rate of 37.85  nm/minute after an initialization time of 1.62 minutes.

![Time=3min.   Time=5min.   Time=7min.   Time=9min.  278nm  135n   202r  CHF=30xSCCM;O2=0SCCM;RFpower=10yW;Pressure=35zmT  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2c78cdff-a598-4dca-b175-aa9f3ab446b9/2c78cdff-a598-4dca-b175-aa9f3ab446b9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215841%3B1743219441&q-key-time=1743215841%3B1743219441&q-header-list=host&q-url-param-list=&q-signature=a1e3c32a93404acdd8fbe9845caae73ecbd504f2)
Fig. 10.   Fluorocarbon film deposition by different process time.

![FluorocarbonFilmDepositionRate  300  250  uuus  200  y=37.85x-61.35  R²=0.9975  ProcessTime(min)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c8d92650-3731-4c72-a362-66ca6dfc6d5f/c8d92650-3731-4c72-a362-66ca6dfc6d5f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215841%3B1743219441&q-key-time=1743215841%3B1743219441&q-header-list=host&q-url-param-list=&q-signature=25a89e73c37a429b2fe955d1c7aa5b5651424068)
Fig. 11.   Fluorocarbon film deposition for deposition rate modelling.

6)   Electrical Conductivity:  Prior to the application of  fluorocarbon films as protection layers, the electrical  conductivity evaluation in the chamber of FIB is required  because the electron charge accumulation on the sample  surface will induce image drifting and affect target navigation  in FIB. The specimen current can be referred to evaluate the  electrical conductivity of the fluorocarbon film. Table III  shows the specimen current in FIB with different materials  on the surface of the samples. The specimen current of the  fluorocarbon film is higher than that of the silicon oxide film.  This means that the deposition of the fluorocarbon film can  also help to improve the electrical conductivity of the  samples.

TABLE III.   IN-FIB SPECIMEN CURRENT COMPARISON.

|Material Type|Specimen current in FIB (5kV, 1.6nA)|
|---|---|
|Copper film|1.0 nA|
|Tungsten film|1.1 nA|
|Silicon oxide film|0.1nA|
|Fluorocarbon film|0.5nA|


## B.   Fluorocarbon Films Application  

1)   TSV:  The first application of fluorocarbon film as a  protection layer on TSV is shown in Fig. 12 to evaluate the  profile, dimension and grain size of Cu TSV. Both OM and  FIB top view images show the clear TSV pattern for target  navigation due to the high transparency of the fluorocarbon  film. SEM cross-sectional images indicate higher material  contrast at the Cu TSV top boundary with fluorocarbon film  deposition compared to in-FIB platinum deposition.

![aIn-FIBplatinumdeposition   (b)Fluorocarbonfilm deposition  XES  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6f45ce1f-76fb-4234-a6a3-5de4efa4bed1/6f45ce1f-76fb-4234-a6a3-5de4efa4bed1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215841%3B1743219441&q-key-time=1743215841%3B1743219441&q-header-list=host&q-url-param-list=&q-signature=1b4c1269a9c61c682cea4fb6a6c664e138456a6f)
Fig. 12.   Fluorocarbon film application for TSV sample.

2)   Micro Bump:  The second application of fluorocarbon  film as a protection layer on micro bumps is shown in Fig. 13  to evaluate the stacked metal layers and TSV under the pads.  Both OM and FIB top view images show that the  fluorocarbon film deposition offers whole-area coverage on  the sample surface with the freedom to cut the cross-section  anywhere. In contrast, with in-FIB platinum deposition, only  a small deposition area is capable for cross-section cuts, and  the other areas without deposition might be damaged by  subsequent ion milling. SEM cross-sectional images show  the results of the whole pad profile for pre-bumping pads  overview.

![(a) In-FIB platinum deposition   (b) Fluorocarbon film deposition  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4318a812-766b-4f04-8de9-d44b9472e9fe/4318a812-766b-4f04-8de9-d44b9472e9fe.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215841%3B1743219441&q-key-time=1743215841%3B1743219441&q-header-list=host&q-url-param-list=&q-signature=038faa0f2e162157575d1d8e6def4125569d79c4)
Fig. 13.   Fluorocarbon film application for micro bump sample.

3)   Hybrid Bonding:  The third application of fluorocarbon  film as a protection layer on hybrid bonding is shown in Fig.  14 to evaluate the dishing degree on the surface of the Cu pad,  which is critical for the subsequent bonding process. Both

OM and FIB top view images also show the clear hybrid  bonding pattern for target navigation due to the high  transparency of the fluorocarbon film. SEM cross-sectional  images also indicate higher material contrast at the Cu pad  top boundary with fluorocarbon film deposition compared to  in-FIB platinum deposition.

![(a) In-FIBplatinumdeposition   (b) Fluorocarbon film deposition  AES    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e27c43f6-e808-47fb-8797-f1971027edfb/e27c43f6-e808-47fb-8797-f1971027edfb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215841%3B1743219441&q-key-time=1743215841%3B1743219441&q-header-list=host&q-url-param-list=&q-signature=07f2c232f4f29377648284ba720102ae7e3c42d0)
Fig. 14.   Fluorocarbon film application for hybrid bonding sample.

## V.   C ONCLUSION   

This study successfully demonstrates the possibility of  depositing fluorocarbon films using a reactive ion etching  tool. Fluorocarbon films can be deposited in an oxygen-free  (O 2 ) environment at lower RF power and higher chamber  pressure. Additionally, higher CHF 3  flow rate accelerates the  deposition of fluorocarbon films, and the deposition rate can  be modeled through a linear fitting equation with regard to the  deposition process time, serving as a reference for practical  applications.

TABLE IV.     P ROTECTION  L AYER  T ECHNIQUES COMPARISON .

||In-FIB platinum deposition|Fluorocarbon film deposition|
|---|---|---|
|Protection Region|Small area (target only)|Large area (whole surface)|
|Process Time (min.)|3~38|9|
|Equipment Cost (USD)|4.4~82.9|0.9|
|Transparancy (OM)|Low|High|
|Transparancy (SEM)|Low|High|
|Material Contrast (SEM)|Low (for metal)|High (for metal)|
|Conductivity (FIB/SEM)|High|High|


The newly developed fluorocarbon film is applied on  TSV, micro bump and hybrid bonding samples as protection  layers for physical analysis and is compared with the  conventional technique of in-FIB platinum deposition, as  shown in Table IV. The large area coverage capability on  sample surface avoids ion beam damage and saves time for  platinum deposition in FIB. The high transparency of the

structure observed under OM and SEM greatly reduces the  difficulty of finding targets, and the high material contrast on  SEM images enhances the resolution of metal boundaries.  Additionally, the good electrical conductivity can help to  reduce electron charge accumulation on the sample surface.

This achievement not only establishes the physical  analysis technique for 3D IC stacking technology, but also  develops a new capability for the reactive ion etching tool,  which is an important contribution to the physical failure  analysis laboratory.

## A CKNOWLEDGMENT 

The authors would like to thank the laboratory members  for their generous support with tool time for this work and the  process team members for providing samples.

## R EFERENCES 

[1]    Y. Y. Xia, B. Liu, Q. Wang, D. N. Yao, D. Gao, Z. Xu, Z. H. Zhang,  Z. T. Song, S. N. Song, X. H. Guo, H. Zheng, and S. L. Feng,  "CHF3/O2-based plasma reactive ion etching of GeTe for nonvolatile

phase   change   memory,"   Transactions   on   Semiconductor  Manufacturing, Vol. 29, No. 2, pp.8-103, May 2016.    [2]    C. M. Lee, Y. H. Pai, and F. S. Shieu, "Ultrahydrophobic and  microporous electrodes fabricated by fluorocarbon plasma etching of  carbon fiber," Journal of The Electrochemical Society, vol. 156, no.  8,pp. B923-B926, 2009.    [3]    P.-C. Lin, J.-H. Xu, P. Li, Y. J. Ding, Z. Y. Ma, C. Xing, J. Jing, and  Y. C. Wang, "TSV CMP process development and pitting defect  reduction,"   International   Conference   on   Planarization/CMP  Technology (ICPT), 2012.    [4]    S. W. Yoon, J. H. Ku, N. Suthiwongsunthorn, P. C. Marimuthu and F.  Carson, "Fabrication and packaging of microbump interconnections for  3D TSV," International Conference on 3D System Integration, 2009.    [5]    L. Ji, F. X. Che, H. M. Ji, H. Y. Li, and M. Kawano, "Wafer-to-Wafer  hybrid bonding development by advanced finite element modeling for  3-D IC packages," Transactions on Components, Packaging and  Manufacturing Technology, vol. 10, issue 12, pp. 2106-2117,  December 2020.    [6]    K. P. Huang, P. Lin, and H. C. Shih, “Structures and properties of  fluorinated amorphous carbon films,” Journal of Applied Physics, vol.  96, no. 1, pp. 354-360, 2004.

