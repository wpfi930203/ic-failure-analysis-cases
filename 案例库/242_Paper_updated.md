---
title: "242_Paper_updated.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_0287c2787235ea0c7fc5f0ac7c7522367295230462135641
file_size: 1447315
---

## Overcoming Challenges in Foreign Material (FM)  Analysis within BGA Packages using FTIR  Spectroscopy with Solder Ball Shear   

Tatiya Ngoenklan 1 , Dumrong Sakulhirirak 1 , Manita Duangsang 1 , Weeraphong Koetkhwamsuk 1  1 Product Quality Center - Bangkok, NXP Semiconductor (Thailand) Co.,Ltd., Changwattana Rd., Bangkok, Thailand  Phone : (+66)811076761, Email :  tatiya.ngoenhlan@nxp.com

Abstract —Fourier-transform infrared spectroscopy (FTIR)  is a valuable tool for identifying foreign materials (FMs) in  semiconductor integrated circuits (ICs). Conventional FTIR  techniques face limitations when analyzing FMs beneath Ball  Grid Array (BGA) packages due to solder ball obstructions.  Traditional methods are hindered by the physical barrier of  solder balls. This paper presents an alternative approach  utilizing solder ball shear followed by ATR FTIR analysis to  effectively characterize FMs within BGA packages. Four  common ball bond removal methods have been discussed and  summarized demonstrating limitations to specifically FMs’  obstacle conditions. Desoldering risks damaging the FM, while  polishing and milling introduce contamination or flatness issues.  The proposed ball shear method involves high-precision  shearing the solder ball to expose the underlying FM, enabling  direct contact with the ATR crystal for FTIR measurement.  This approach avoids altering the FM's chemical structure  while offering precise control over the shearing depth.  Experimental results demonstrate the effectiveness of this  method in acquiring high-quality FTIR spectra of an embedded  FM identified as Polyvinyl Formal (PVF). The characteristic  peaks of the FM become clearly distinguishable after solder ball  shear, significantly improving the signal-to-noise ratio and  facilitating accurate identification.

Keywords—FTIR, BGA, Foreign Material, Solder Ball Shear,  ATR, IRAS, Chemical Analysis, Polyvinyl Formal

## I.    I NTRODUCTION 

Fourier-transform infrared spectroscopy (FTIR) is a  technique used to obtain an infrared spectrum of a solid,  liquid, or gas. An FTIR spectrometer simultaneously collects  high-resolution spectral data over a wide spectral range [1]. In  FTIR spectrometry, all the resolution elements are measured  at all times during the measurement, corrected information of  radiations that passed between the source and the detector for  each resolution element. FTIR is being used widely in  semiconductor   integrated   circuits   (ICs)   to   analyse  composition elements of non-conductive contaminants or  Foreign Materials (FM) in the assembly process that led to the  root cause finding and quality improvement activities. The  potential consequences of undetected FMs are device failures  performance degradation, and safety hazards. Several FTIR  analysis sampling techniques can be used to understand a  material’s structure and identify the material, each with their  own proficiency such as Attenuated Total Reflectance (ATR),  Specular Reflectance (SR), Reflection-Absorption – Infrared  Reflection Absorption Spectroscopy (IRAS), Transmission,  and Photoacoustic [2]. ATR imaging mode is a powerful tool  and provides the opportunity in the applications to dissolution  of chemical structure by the characteristic absorbance of  corresponding molecular vibrations in the sample One of the

key advantages of ATR-FTIR imaging is that it requires  minimal or no sample preparation prior to spectral  measurements. This is due to the fact that the penetration  depth of IR light in the sample for ATR measurements is  independent of sample thickness [3]. However, when size of  FM gradually goes down, signal-to-noise ratio (SNR)  deteriorates due to smaller FM signal and huge background  noise was observed in most practical case. When FM resides  beneath Ball Grid Array (BGA) packages, conventional FTIR  analysis encounters limitations due to the physical barrier  posed by the solder balls, preventing direct contact between  the FM and the detector tip. This paper explores various  strategies to overcome this challenge and enable effective  FTIR analysis within BGA packages. Then, demonstrates the  alternative effective method for the analysis.

## II.   M ETHODS AND RESULTS 

This paper discusses the presence of FM within the solder  ball area, obstructing direct contact between the ATR-Crystal  and the FM as depicted in Fig. 1. To identify the FM, the  solder ball needed removal for FTIR analysis, ensuring no  alteration to its chemical structure while keeping the FM  intact within the sample. Thus, initial measurements of the  FM's height and width were crucial to verify compatibility  with the FTIR machine's detection capabilities. The measured  dimensions of the expose area of the FM were approximately  120x490um with 10um height, using Nikon Measuring  Microscope model: MM-60. This paper will discuss four  common solder ball removal techniques: desoldering,  polishing, milling, and solder ball shear. We will explore their  limitations in exposing the foreign materials beneath the bond  pad, highlighting the need for the proposed method.

![ATR-Crystal  300 U:  350um  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f7c7f07f-d0b5-41a2-88a5-82390de5f497/f7c7f07f-d0b5-41a2-88a5-82390de5f497.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=dddb334673c382796c4fdb6e7824730751cb7740)
Fig. 1.   The sample before the solder ball shear indicates that the ATRCrystal is not in contact with the foreign material due to its proximity to the  solder ball.

The solder ball removal process involves extracting the  original solder balls from the sample. In this paper, four  methods of solder ball removal are studied:

## A.   Desoldering wick  

In this study, desoldering wick is utilized for this purpose.  During the solder ball removal process using solder iron  together with a copper braid (desoldering wick), the package  is secured with the solder balls facing upwards. Soldering  iron is employed to heat a desoldering wick, which is  manually moved over the solder ball. Then, the solder ball  melts and is absorbed into the wick. This method is a simplest  cost-effective and suitable for removing multiple balls  effective in a big area simultaneously. However, it involves  applying heat with additional material (desolder wick)  directly over the solder ball, posing a harmful risk of  damaging the foreign materials or could have lost it (as  demonstrated in Fig. 2).

![Tweezer  Desoldering wick  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/20b65ad4-e94a-4d00-9aad-2dd6f721a7ae/20b65ad4-e94a-4d00-9aad-2dd6f721a7ae.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=aa9750f9ec1c2a0c6578ebb9ac12b2cdfad13370)
Fig. 2.   Solder ball removal by a common soldering and desoldering wick  method.

## B.   Polishing  

The second method explored in this investigation is wet  polishing, a technique delineated in Fig. 3. Dry polishing is  omitted from consideration due to its propensity for causing  smearing effects. In this method, the sample is oriented with  the solder ball facing downwards, in contact with a diamond  lapping film. This film comprises a micro-abrasive layer  coated with slurry, embedding grains within a resin that  adheres to a Polyethylene Terephthalate (PET) substrate.  Employing even pressure on the BGA package while moving  it in a patterned manner, the solder balls undergo grinding via  friction, resulting in the detachment of chips or debris from  the sample’s surface.

To facilitate this process, water is introduced to cool the  workpiece, minimize friction, and remove debris. However,  managing the height and flatness angle to prevent dislodging  of adhered foreign material presents a challenge. Moreover,  the procedure may yield a smear effect around the soldered  ball,   potentially   obscuring   the   surrounding   area.  Additionally, the composition elements of FMs may be  influenced by the presence of water.

Hence, while wet polishing offers a viable method for  solder ball removal, meticulous control and consideration are  required to mitigate potential drawbacks such as height  control and smearing effects, ensuring accurate analysis of  the BGA package's interior.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3753be68-d226-4934-8d45-d227f2d9d143/3753be68-d226-4934-8d45-d227f2d9d143.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=9ceba42ec73d3ab530932ed06700d124939e1658)
Fig. 3.   Solder ball removal by polishing method.

## C.   Milling  

The third method examined in this paper is a high  precision milling, as depicted in Fig 4. This process requires  the use of Allied X-Prep machine. X-Prep is a specialized   5-axis   CNC-based   milling/grinding/polishing   machine  designed to handle applications that require high-accuracy  sample preparation. The standard setup of the machine  requires; sample mounted on the glass slide and place the  grinding side upward, inserted the sample on the glass and  aligned the sample perpendicular with horizontal, place the  glass slid into the   $2^{\ast\ast}\mathbf{x}2^{\ast\ast}$   fixture and secure with the screws,  filled the   $2^{\ast\ast}\,_{\mathbf{X}}2^{\ast\ast}$   fixture with “Green Lube” lubrication oil.  Green Lube is a medium viscosity hexylene glycol based  lubricant used for general metallographic preparation. The oil  contains both of hazardous and organic elements which  tremendously affect the FMs compositions that end up with  fault FTIR detecting results [4].

![Millingtip  2x2Fixture  Green Lube  samplemounted  ontheglassslide  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/02c62c37-d431-401c-aede-2f16f9a2b2d5/02c62c37-d431-401c-aede-2f16f9a2b2d5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=b3b5a6376e2ec47679a572626eab7e19b1e0d70e)
Fig. 4.   Solder ball removal by milling method.

## D.   Solder ball shear  

The final method examined in this study is solder ball  shear, as depicted in Fig 5. The equipment utilized is DAGEseries 4000PXY. In this process, the sample is clamped  within a jig fixture, various parameters are set as follows;   -    Load cell is configured to   $5\;\mathrm{kg}$

-    Shear speed is maintained at 100um per second  -    Shear height is set to 10um  which corresponds to the  height of the foreign material


As per the recommendations of JESD22-B117B (Index:  4.6 – Shear Tool), the shear tool should not make contact with  the sample surface throughout the monitored shear tool travel  distance, and special precautions must be taken to ensure that  the solder ball under test is not touched during the initial setup  operation. Prior to the operation, solder balls were visually  examined [5]. According to a very limited defective samples  quantity only 2 units, to ensure an accuracy of the ball bond  shearing results with ball height (10um), an experiment was  done with a total of 10 balls before releasing the setup to the  unit under test, and the results are presented in Table I,  indicating the height of the solder balls after sheared.

![Sheartip  Jigfixture  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/61bc6856-2366-43c3-81be-313e048e4706/61bc6856-2366-43c3-81be-313e048e4706.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=e7670300f1005b53fee38f943f32d74db2a900b1)
Fig. 5.   Solder ball removal by solder ball shear method.

TABLE I.     R EMAINING BALL HEIGHT MEASUREMENT .

|Ball Number|Ball height (um)|Tolerance (T) (um)|
|---|---|---|
|1|9|-0.1|
|2|10|0|
|3|11|0.1|
|4|10|0|
|5|10|0|
|6|10|0|
|7|11|0.1|
|8|10|0|
|9|10|0|
|10|10|0|


From the test of all 10 balls, the height of the balls after  shearing ranges from 9 to   $11~\mathrm{{um}}$  . The tolerance rate from the  experiment is  $\pm\:0.1\mathrm{up}$  . Therefore, the results ensure that the  ATR detectable has no impact from the delta height between  the FA and the remaining ball bond as will be described in the  section II (E). Summary of four well-known solder ball  removal methods, shown as in the TABLE II.

TABLE II.     S UMMARIZES AN INTERFERENCE OF ALL FOUR WELL - KNOWN METHODS .

|Method|FMs’ interferences|FMs’ interferences|FMs’ interferences|
|---|---|---|---|
|Desoldering|Heat|Uncontrollable height|Not possible for small area|
|Polishing,|Water|Strain|Flatness control|
|Milling|Oil|||
|Solder ball shear||||


Solder ball shear emerges as the most suitable method for  solder ball removal, as indicated in Table II, particularly when  foreign material is situated beneath the ball bond. Upon  implementing this selected method at the location of the  foreign material, the Scanning Electron Microscope (SEM)  image in Fig. 6 illustrates successful solder ball removal in  both faulty devices, clearly exposing the foreign material.  Inspection of the SEM image confirms that the surface of the  foreign material remains unaffected by the shear tip or strain,  consistent with the findings presented in Table II.

![Foreignmaterial  Sheardirection  Solderball  1/22/2024dwellmagHV   D   detHFW   SOO  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c74db295-0aa4-4085-b350-501ce3fb763b/c74db295-0aa4-4085-b350-501ce3fb763b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=6a36b5bc708c9d5efbf657e3a38f007bdac2798f)
Fig. 6.   SEM image after the ball bond removal by solder ball shear method  at the foreign material in the defective device.

## E.   FTIR spectrum illustration  

As depicted in Fig.7, ATR is employed to collect FTIR  spectra prior to sample preparation using the solder ball shear  method. While ATR is a commonly used technique in FTIR  for studying thin films and monolayers, specifically designed  for investigating surfaces and interfaces, it was found that it  cannot capture the signal of the foreign material. This  limitation arises because the FM is in close proximity to the  solder ball, preventing direct contact with the ATR-crystal, as  indicated in Fig.1. Following the sample preparation via  solder ball shear, FTIR can acquire spectra in ATR mode.  FTIR spectra are further interpreted by analyzing functional  group vibrations. The chemical structure of polyvinyl formal  (PVF) is illustrated in Fig.8. Fig.9 illustrates the spectral  comparison between the foreign material and the PVF   $83\%$  match calculating from two spectrograms. Frequencies  appear in the x-axis in units of inverse centimeters  (wavenumbers) and intensities are plotted on the y-axis in  percentage units. As depicted in Fig. 9, the bands observed the  wavenumbers range of   $2800{-}1000~\mathrm{cm}^{-1}$   can be attributed to  the stretching vibrations of C-H bonds within the polymer.  Additionally, bands within the range of   $1700{\cdot}1750\;\;\mathrm{cm}^{-1}$    signify  $\mathrm{C=O}$   stretching vibrations. The bands appearing in the

region of   $1000{-}1200\ \ \mathrm{cm^{-1}}$   are associated with C-O-C  stretching vibrations, a result of the reaction between  polyvinyl alcohol and formaldehyde. Peaks found in the  fingerprint region (below   $1500\;\mathrm{\cm^{-1}}$  ) may correspond to  various vibrations within the polymer.

PVF is a polymer synthesized through the reaction of  polyvinyl alcohol with formaldehyde. Classified as a  thermoplastic resin, it finds utility in diverse applications  owing to its distinctive characteristics. The synthesis entails  the controlled reaction between polyvinyl alcohol and  formaldehyde. Polyvinyl formal is a colorless, flexible, tough  solid, boasting noteworthy properties such as resistance to  moisture, greases, oils, and alkalis.

![ATRbeforesolderballshear  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/18f6bcf1-5f63-4f86-9bc2-5f0473094204/18f6bcf1-5f63-4f86-9bc2-5f0473094204.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=7ebb060b2feb66906f039634dfe55d736bb3c00f)
Fig. 7.   FTIR spectrum before solder ball shear using the ATR technique.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/14ae14e4-6469-4fd4-99c5-9cd42123afdf/14ae14e4-6469-4fd4-99c5-9cd42123afdf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=db322f1b97d49e527a42a8aac928f1d8dd444fd4)
Fig. 8.   The chemical structure of polyvinyl formal [6].

![ATRAftersolderballshear  188  S5  Polyvinylformal  F40P0   3500   3000   2500   2000   1500   100O  cm-1  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/27d8d0e7-e6d1-41bb-9852-340611cc55a3/27d8d0e7-e6d1-41bb-9852-340611cc55a3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=a7633911ae27b8d2387081acde774baab3958ee3)
Fig. 9.   FTIR spectrum after solder ball shear using the ATR technique.

In FTIR analysis, a pristine PVF spectrum serves as a  reference, exhibiting a high degree of similarity (  $83\%$   after  correction for foreign material). This reference spectrum  represents the unprocessed material's native topology with  intact chemical structures stored in the FTIR library.   However, throughout assembly, foreign materials might  engage in reactions with other chemicals or undergo backend  processes. Consequently, the  $17\%$   disparity can be ascribed to  variations in absorption rates between robust (PVF) and

fragile (FM) bonds within the  $\mathrm{C=O}$     $\sim\!1700~\mathrm{cm^{-1}}$  ) and alcohol   $(\mathrm{>}1500\;\mathrm{cm}^{-1})$  ) regions.

## C ONCLUSION :  

BGA packages present difficulties for traditional FTIR  analysis methods, but there are several strategies available to  address these challenges effectively. Factors such as the  location of FM within the BGA package, its depth, and the  desired level of detail in analysis should inform the choice of  approach. Ongoing advancements in FTIR technologies and  sample preparation techniques offer promise for further  improving the analysis capabilities, especially within  complex, multi-layered structures like BGA packages.

The successful application of FTIR analysis plays a crucial  role in identifying the root causes of issues, whether they  originate from suppliers or assembly processes. This, in turn,  facilitates the implementation of effective corrective actions  to mitigate the presence of foreign materials and prevent  future occurrences.

## A CKNOWLEDGMENT 

The authors wish to express their gratitude to the  colleagues at the Product Diagnostic Quality Center (PDQC)  Bangkok, Thailand for their invaluable contributions to the  operational   and   execution   aspects   that   significantly  contributed to the successful completion of this paper.

## R EFERENCES 

[1]    Griffiths, P.; de Hasseth, J. A. (18 May 2007). Fourier Transform  Infrared Spectrometry (2nd ed.). Wiley-Blackwell. ISBN 978-0-471- 19404-0    [2]    J. Mathias, “How does FTIR analysis work?,” Innovatech Labs,  http://www.innovatechlabs.com/newsroom/672/stuff-works-ftiranalysis/ (accessed Feb. 2, 2024).    [3]    S.G. Kazarian and K.L.A. Chan, “Applications of ATR-FTIR  spectroscopic imaging to biomedical samples,” Biochimica et  Biophysica Acta, vol. 1758, 858–867, 2006.    [4]    Allied High Tech Products, “X-Lube Cutting/Grinding/Polishing  Fluid,” safety datasheet, June. 2022 [Revised June. 2022].    [5]    Solder Ball Shear, JEDEC standard JESD22-B117B, 2020.    [6]    David R. Rohindra and Jagjit R. Khurma, “Miscibility, melting and  crystallization of poly(ε-caprolactone) and poly (vinyl formal) blend,”  2007 The South Pacific Journal of Natural Science, pp. 53-60, 2007.

