---
title: "247_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_cc1d88d53c1423af7cce84b897acbe897295230462135641
file_size: 1499519
---

## Metallic Trace Contaminant Detection Using SEM/EDX 

Aaron, Lee\*; Bernice, Zee; Fang Jie, Foo

Advanced Micro Devices (Singapore) Pte Ltd, Device Analysis Lab 508 Chai Chee Lane Singapore 469032  Phone: +65 6796 9888 \*Email:  Lee.Waikenaaron@amd.com

## Abstract 

Surface characterization techniques such as Auger Electron Spectroscopy (AES) and X-ray Photoelectron Spectroscopy (XPS)  are commonly used to analyze surface contaminants to determine their elemental composition and/or chemical states. However,  one may not have easy access to these techniques due to high cost of ownership and stringent analysis requirements. Thus, an  alternative characterization technique, such as Scanning Electron Microscopy (SEM)/Energy Dispersive X-ray (EDX)  spectroscopy, could be considered for trace contamination detection if precise elemental composition identification is not required.  This paper describes the application of SEM/EDX in detecting trace amounts of Cu on Si die surface. Overall, the results showed  that at a low accelerating electron voltage, EDX was able to conclusively detect Cu contaminant.

## Background and Objective 

The need for an ultra-clean Silicon (Si) wafer surface is of  utmost importance in semiconductor manufacturing because  microcontaminants such as ions, particulates and organics may  have detrimental effect on the performance and yield of  electronic devices [1]. As semiconductor device geometries  continue to shrink, such microcontaminants will have an everincreasing detrimental impact on device yield and reliability.  Impurities of transition metals such as Copper (Cu) are of  concern because they are notoriously known to be highly  diffusive and soluble in bulk Si, with the ability to form  precipitates in p–n junctions or at silicon/silicon dioxide  interface, thus decreasing the gate oxide integrity and increasing  leakage currents [2,3]. During fabrication, Si wafers can be  easily contaminated with Cu since it is widely used as an  interconnect material in the back-end-of-line (BEOL) process  as well as interconnect bumping. Surface characterization  techniques such as Auger Electron Spectroscopy (AES) and Xray Photoelectron Spectroscopy (XPS) are commonly used to  analyze surface contaminants to determine their elemental  composition and/or chemical states [4]. These techniques are  highly sensitive, precise and provide near surface information  (i.e. top few nanometers) of the sample being investigated.  However, engineers may not have easy access to these  techniques due to high cost of ownership. Furthermore,  stringent analysis requirements may mean longer time to  results. Thus, an alternative characterization technique, such as  Scanning Electron Microscopy (SEM)/Energy Dispersive Xray (EDX) spectroscopy, could be considered for trace  contaminant detection if precise elemental composition  identification is not required. While SEM/EDX has historically  been considered a bulk material analysis tool, advancements in  SEM resolution, EDX detector geometry such as larger detector  window size and analytical solid angle, and electronics have  improved the theoretical detection sensitivity of EDX [6].

It is observed that the detection limits of SEM/EDX are  comparable with the other surface characterization techniques,  as shown in Fig. 1, indicating that SEM/EDX is a viable option  for trace element detection when used under appropriate  conditions. In order to reach the theoretical detection limit of  SEM/EDX in terms of spatial resolution and sensitivity,  sufficiently low acceleration electron voltage must be used to  reduce   the   electron   interaction   volume   and   enough  characteristic X-ray signal needs to be collected by the EDX  detector.

Fig. 1 – Detection limits of various surface characterization  techniques [5].

|        Surface                Characterization                Technique      |SEM/EDX|AES|XPS|
|---|---|---|---|
|Signal Measured|        Backscatter or                Secondary Electrons      |Auger Electrons|Photoelectrons|
|DetectionLimits|~0.1Atomic%|0.01-0.1Atomic%|~0.1Atomic%|


Since trace contaminants are typically in the top few  nanometers of the Si surface and do not homogenously cover  the surface, using very low accelerating electron voltages (2keV  or less) is ideal for SEM imaging and EDX analysis. According  to observations from simulations, the electron interaction  volume at 5keV is much smaller compared to   $20\mathrm{keV}$  , as  illustrated by Fig. 2, which means within the analyzed volume,  total contaminant concentration could be more than the  detection limit of the EDX. However, the problem with low  accelerating electron voltage is the low X-ray signal collected  by the EDX detector.

![ElectronBeam  ElectronBeam Interaction Volume Interaction Volume （b） ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2801cdfb-68ae-44c8-b589-1dcfd8e4d4d6/2801cdfb-68ae-44c8-b589-1dcfd8e4d4d6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215669%3B1743219269&q-key-time=1743215669%3B1743219269&q-header-list=host&q-url-param-list=&q-signature=cde2f5b634438bd8e62b96b796b02cebae7d8687)
Fig. 2 – Electron interaction volumes for Si at (a)  $20\mathrm{keV}$   and (b) 5  keV [7].

This paper describes the application of SEM/EDX in  detecting trace amounts of Cu on Si die surface. Various  accelerating electron voltages were tested for feasibility and  determination of the optimum condition that will allow trace Cu  to be detected.

## Equipment Set-up and Test Conditions   

SEM/EDX analysis was performed using Thermo-Fisher  Scientific Quanta 650 SEM with Bruker xFlash 6|60 EDX  detector. The acceleration electron voltage used for EDX  analysis was determined based on the characteristic X-ray  energies of the element being detected. In the case of Cu, the Xray intensities are 8.0413 and 0.9297 for Kα and Lα respectively  [10], thus the acceleration electron voltage used for analysis  ranged from 4keV to  $20\mathrm{keV}$  . Theoretically, 2keV is enough to  analyze Cu Lα line but as mentioned above, too low an  accelerating electron voltage would mean insufficient X-ray  signal collected by the EDX detector and the contaminant  would not be detected. The EDX measurement duration was set  at three minutes to minimize sample drift as well as allow  enough X-ray counts to be collected for good signal-to-noise  ratio (SNR). The device analyzed came from an engineering lot  with known Cu contamination on die backside. To quantify the  elements detected on the die backside, average normalized mass  percentage (Ave. Mass Norm.   $\%$  ), average atomic percentage  (Ave. Atom   $\%$  ) and characteristic x-ray spectrum were  collected.

## Results and Discussion 

EDX data of the device with Cu contamination were obtained  using acceleration electron voltages of   $20\mathrm{keV}$  , 15keV, 10keV,  and 4keV. As Cu is a heavier Z element as compared to Si, its  contaminants will tend to have a high contrast with respect to Si  when view under the SEM.  From Tables I to III, it was  observed that Cu could not be detected on the die backside at   $20\mathrm{keV}$  , 15keV, and   $10\mathrm{keV}$  . This observation is consistent with  theory that for a given material, the electron interaction volume  increases with increased acceleration energy. As the Cu  contamination was expected to be trace and near the surface, the  EDX data indicated that acceleration voltages higher than   $10\mathrm{keV}$   were not suitable for conducting trace analysis of  transitional metal on Si. This was because characteristic X-ray  signals were being generated from deep within the bulk silicon  instead of the surface, thus surface Cu could not be detected.

TABLE I.     EDX   D ATA AT  20 KE V   –   N O CU WAS DETECTED

|Element|Ave. Mass Norm. [%]|Ave. Atom [%]|
|---|---|---|
|Carbon|21.67|38.94|
|Oxygen|1.52|2.05|
|Silicon|76.81|59.02|


![EDXpoint  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7e3509f2-9340-4afb-85d6-a4916004cc97/7e3509f2-9340-4afb-85d6-a4916004cc97.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215669%3B1743219269&q-key-time=1743215669%3B1743219269&q-header-list=host&q-url-param-list=&q-signature=e62507a0ec206ba07e121c9d5721d271e4fd383d)
Fig. 3 - SEM image of Si die surface at  $20\mathrm{keV}$   with location of EDX  analysis.

![cps/ev  Spectrum1  3S  303  25  Energy[keV]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/53c2c914-0b08-4a88-b124-0430a4280355/53c2c914-0b08-4a88-b124-0430a4280355.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215669%3B1743219269&q-key-time=1743215669%3B1743219269&q-header-list=host&q-url-param-list=&q-signature=5a170f1f6f1340228952d8c27c19c1a3e0fd5993)
Fig. 4 – EDX spectrum of Si die surface analyzed at  $20\mathrm{keV}$  .

TABLE II.     EDX   D ATA AT  15 K EV   –   N O CU WAS DETECTED

|Element|Ave. Mass Norm. [%]|Ave. Atom [%]|
|---|---|---|
|Carbon|37.01|57.61|
|Oxygen|0.92|1.08|
|Silicon|62.07|41.32|


![EDXpoint  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1f8f0e04-8a17-49cf-a13d-759a183e8d2d/1f8f0e04-8a17-49cf-a13d-759a183e8d2d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215669%3B1743219269&q-key-time=1743215669%3B1743219269&q-header-list=host&q-url-param-list=&q-signature=3184b4304280f625f7433063a653b3e6816b2076)
Fig. 5 - SEM image of Si die surface at   $15\mathrm{keV}$   with location of EDX  analysis.

![s/ev  18  163  14  123  103  Energy [keV]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2fbbe743-3c22-4449-b0a9-007d95d4d848/2fbbe743-3c22-4449-b0a9-007d95d4d848.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215669%3B1743219269&q-key-time=1743215669%3B1743219269&q-header-list=host&q-url-param-list=&q-signature=b3812da5f69ab2b678bec80775418dfebbcfb51d)
Fig. 6 - EDX spectrum of Si die surface analyzed at  $15\mathrm{keV}$  .

|Element|Ave. Mass Norm. [%]|Ave. Atom [%]|
|---|---|---|
|Carbon|57.33|75.43|
|Oxygen|1.34|1.32|
|Silicon|41.33|23.25|


![EDXpoint  Ch1 MAG:87.7kx     ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a2f41f1b-295a-4cc0-b7dc-1d38cf25dd36/a2f41f1b-295a-4cc0-b7dc-1d38cf25dd36.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215669%3B1743219269&q-key-time=1743215669%3B1743219269&q-header-list=host&q-url-param-list=&q-signature=1f61b952c4dfbd09e4e78f263b8b31bf5de25d03)
Fig. 7 - SEM image of Si die surface at  $10\mathrm{keV}$   with location of EDX  analysis.

![cps/ev  Spectrum1  12  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/66827937-b22a-403e-9ff6-825c377894bb/66827937-b22a-403e-9ff6-825c377894bb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215669%3B1743219269&q-key-time=1743215669%3B1743219269&q-header-list=host&q-url-param-list=&q-signature=8e185790639f6af8442f204f010066ed51025d34)
Fig. 8 - EDX spectrum of Si die surface analyzed at   $10\mathrm{keV}$  .

Subsequently, when the acceleration voltage was reduced to  4keV, EDX data showed that Cu could be detected on the die  backside as seen from Table IV. Similarly, this observation is  consistent with theory that the electron interaction volume  decreases with reduced acceleration energy and surface Cu can  be detected.

![cps/ev  Spectrum1  1.0  10   2.0   2.5   3.0   3.5   4.0   4.5   5.C  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/43e0dced-8ce7-4ec9-b087-6a4208c2fd8b/43e0dced-8ce7-4ec9-b087-6a4208c2fd8b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215669%3B1743219269&q-key-time=1743215669%3B1743219269&q-header-list=host&q-url-param-list=&q-signature=6868a590a92487c2431fb8313c500020c11da1f6)
Fig. 10 - EDX spectrum of Si die surface analyzed at 4keV.

To verify the SEM/EDX data, a TEM lamella was prepared  from a location where Cu was detected. EDX analysis in TEM  confirmed the presence of Cu on the die backside as shown in  Fig. 11.

![Mixture o   si/o/sn.   Copper Silicide  Crystalline  Silicon  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7ed661e2-0248-4941-b9ce-08282e65da52/7ed661e2-0248-4941-b9ce-08282e65da52.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215669%3B1743219269&q-key-time=1743215669%3B1743219269&q-header-list=host&q-url-param-list=&q-signature=9651fe9ec9d95f22b06b98f075cf556394b2f6ae)
Fig. 11 - TEM Image and EDX Mapping of die backside Cu  contamination.

## Conclusion 

SEM/EDX at low accelerating electron voltage was able to  detect trace Cu contaminant on Si die surface, providing a much  more accessible alternative to surface characterization of  metallic contaminants. Possible future considerations could  include measurements from XPS.

## Acknowledgment 

TABLE IV.     EDX   D ATA AT  4 KE V   –   C U WAS DETECTED

|Element|Ave. Mass Norm. [%]|Ave. Atom [%]|
|---|---|---|
|Carbon|24.53|46.63|
|Oxygen|6.54|9.34|
|Silicon|42.45|34.52|
|Copper|26.48|9.52|


![EDXpoint  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c9085c2d-8f99-444c-83f8-a01cd7f4aa73/c9085c2d-8f99-444c-83f8-a01cd7f4aa73.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215669%3B1743219269&q-key-time=1743215669%3B1743219269&q-header-list=host&q-url-param-list=&q-signature=b13f0c61e310219774bae1b40fe1b973176d065a)
The authors would like to thank their colleagues for their  support and contributions as well as The Bruker Corporation for  their applications support.

$\copyright$   2019 Advanced Micro Devices, Inc. All rights reserved.  AMD, the AMD Arrow logo, and combinations thereof are  trademarks of Advanced Micro Devices, Inc. Other product  names used in this publication are for identification purposes  only and may be trademarks of their respective companies.

## References 

[1]    Baltzinger J.L.,  et al . Contamination monitoring and analysis in  semiconductor manufacturing, Semiconductor Technologies, Chapter 4,  Contamination   Monitoring   and   Analysis   in   Semiconductor  Manufacturing    [2]    Hoelzl R.,  et al ., “Modeling of Cu gettering in p- and n-type silicon and  in poly-silicon”, Appl. Phys. A 75,2002, Page(s): 525–534.    [3]    Istratov A. A.,  et al ., “Diffusion, solubility and gettering of copper in  silicon”, Materials science and engineering B72, 2000, Page(s): 99-104.    [4]    K. Miyoshi et al, Surface Characterization Techniques: An Overview,  [Online].   Available:  https://ntrs.nasa.gov/archive/nasa/casi.ntrs.nasa.gov/20020070606.pdf.  [Accessed 16 Jan 2019]    [5]    Evans Analytical Group, "Analytical Resolution vs Detection Limit"  [Online]. Available:   http://www.eaglabs.com.tw/cmss_files/attachmentlibrary/analyticalresolution-versus-detection-limit-BR004.pdf. [Accessed 16 1 2019].    [6]    S. Burgess,  et al , "Ultra-low kV EDS – A New Approach to Improved  Spatial Resolution, Surface Sensitivity, and Light Element  Compositional Imaging and Analysis in the SEM" [Online]. Available:  https://pdfs.semanticscholar.org/bb30/ef3913d925f3471f10c9ff43a88ef df9de47.pdf. [Accessed 16 1 2019].    [7]    H   C. E. Lyman,  et al . “Tutorial Review: X-ray Mapping in ElectronBeam Instruments” Microscopy and Microanalysis, 12(01), p. 2-25,  2006.    [8]    H.S. Wong, N.R. Buenfeld, “Monte Carlo simulation of electron-solid  interactions in cement-based materials”, Cement & Concrete Research,  Vol. 36, p. 1076-1082, 2006.    [9]    Electron Microanalysis  $@$   NAU, [Online]. Available:  https://www2.nau.edu/microanalysis/wordpress/index.php/signals/#electron_interaction_volume.  [Accessed 16 Jan 2019].    [10]   Periodic_Table_and_X-ray_Energies, [Online]. Available:  https://www.bruker.com/fileadmin/user_upload/8-PDF-Docs/XrayDiffraction_ElementalAnalysis/HHXRF/Misc/Periodic_Table_and_X-ray_Energies.pdf. [Accessed 16 Jan  2019].

