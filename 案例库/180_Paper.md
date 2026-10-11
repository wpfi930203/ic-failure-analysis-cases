---
title: "180_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_f43055b2f2ae177ed9fc983ffe931cb77295230462135641
file_size: 605019
---

## Case Study on Package Level Defect Localization  through Optimized Lock-in Thermography Frequency   

Carlo M. Casabuena, Em Julius De La Cruz  Failure Analysis Department, Maxim Integrated  Gateway Business Park, Brgy. Javalera, General Trias, Cavite, Philippines  Email:  Carlo.Casabuena@maximintegrated.com ;  Emjulius.Delacruz@maximintegrated.com

Abstract-  This case study outlines the successful package-level  failure site detection by optimizing the Lock-In Thermography  (LIT) frequency based on resistance, combined with 3D X-ray for  locating the defect and EDX (Energy Dispersive X-ray) for  root-cause analysis. By optimizing the lock-in frequency, the exact  location of the defect on the package was identified, thus, leading  to effective determination of failure mechanism and accurate root  cause investigation.

## I. I NTRODUCTION 

Lock-in Thermography (LIT) is a form of dynamic IR  thermography which provides a much better signal-to-noise  ratio, increased sensitivity and higher feature resolution than  steady-state   thermography.      LIT   offers   a   "through  package" analysis, thus, allows failure analysts to perform  non-destructive fault localization.    The usefulness of Lock-in  Thermography is given mainly by the fact that it allows a  relatively coarse but very sensitive localization of any leakage  current or other local heat source in an integrated circuit with a  very high success rate without any preparation expense.  The  technique minimizes incidents of failure recovery due to  introduction of destructive steps such as backside sample  preparation or decapsulation prior to fault isolation process.

Lock-in amplifiers are used to detect and measure very small  AC signals. Accurate measurements may be made even when  the small signal is obscured by noise sources. Lock-in  amplifiers use a technique known as phase-sensitive detection  to single out the component of the signal at a specific reference  frequency and phase. Noise signals, at frequencies other than  the reference frequency, are rejected and do not affect the  measurement.

The lock-in frequency is one of the most important  measurement parameters during LIT. If an incorrect lock-in  frequency was chosen, this can lead to an invalid hotspot.   Measuring at multiple frequencies improves the accuracy and  confidence level of the defect localization.

This case study outlines the   successful detection of the failure  site in a QFN packaged sample through optimization of the  lock-in frequency based on resistance, whereby the exact  location of the defect was determined.  With the help of other  non-destructive   analysis   techniques   such   3D   X-Ray,  destructive   methods   accurately   identified   the   failure  mechanism.

## II.   METHODOLOGY  

LIT Characterization of lock-in frequency based on resistance  for a single layer die QFN package

Short failures with different resistances from   $0.9~\Omega$   to   $3\,\mathrm{~k}\Omega$    were subjected to LIT by probing the shorted pins with 60  seconds exposure time and lock-in frequencies of 1, 5 and 10  Hz obtaining 1 mW power dissipation. It was observed that for  a low-ohmic shorts (  $0.9~\Omega$   to   $45~\Omega$  ), lower lock-in frequency  provides very sensitive detection resulting to an invalid hotspot.  For higher resistances (  $150~\Omega$   to   $3\ \mathrm{k}\Omega$  ), low and high lock-in  frequencies provide valid hotspot, but higher lock-in  frequencies provide more precise and accurate defect site.  Figure 1 shows the characterization of lock-in frequency based  on resistance.

![  1 Hz Lock-in Frequency    0.9   45   150   3 k2    lovalid defect site    Invalid defect   (other circuil    site (oubide pin   connrcted to     ofthe onit   fifing pinj  Vaid defect site  Walid defeet cite          ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4ff932fd-8f08-4240-b799-b6025dfd00ec/4ff932fd-8f08-4240-b799-b6025dfd00ec.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215641%3B1743219241&q-key-time=1743215641%3B1743219241&q-header-list=host&q-url-param-list=&q-signature=1a53a73c87bd989f57be590d68d6909a38744e01)
Figure 1. 1Hz lock-in frequency is the most sensitive to used but produces  invalid results in the lowest ranges (  $0.9\;\Omega$   to   $45\;\Omega$  ) of ohmic shorts. At higher  ohmic shorts   $.150~\Omega$  to   $3~\mathrm{k}\Omega$  ), it provides a valid defect site but with a larger  hotspot area.

![5 Hz Lock-in Frequency    0.9   4592      1500   3:42      Valid defeet site  Valid defect cite     Walid defect site      outide pia.    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d592cb5e-3ef7-4f09-823d-d90c83c59b53/d592cb5e-3ef7-4f09-823d-d90c83c59b53.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215641%3B1743219241&q-key-time=1743215641%3B1743219241&q-header-list=host&q-url-param-list=&q-signature=5f8317a53cdf076cc1bf5e886dcf64841c70f862)
Figure 2. 5 Hz lock-in frequency produces invalid results for shorts in the  lowest ohmic short  $(0.9\,\Omega)$  . At 45 Ω, it provides a valid defect site but there still  area with a weak hotspot.  At higher ohmic shorts (  $150\,\Omega$   to  $3\,\mathrm{k}\Omega$  ), it provides a  valid defect site but with a smaller hotspot area than 1 Hz.

![   10 Hz Lock-inFrequency     0.90   450   1500   3k         Validdefectsit   Valid defect site     defectsite        ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b3f10427-eef6-4c71-a6db-376ccc780a37/b3f10427-eef6-4c71-a6db-376ccc780a37.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215641%3B1743219241&q-key-time=1743215641%3B1743219241&q-header-list=host&q-url-param-list=&q-signature=1e5e2d5f7d05fea27aaee6c4c8158fcfeeca5255)
Figure 3. 10 Hz lock-in frequency produces valid defect site on all ohmic short  ranges (  $0.9\,\Omega$   to  $3\,\mathrm{k}\,\Omega$  ). It provides a defect site with a smaller hotspot area than  1 Hz and 5 Hz.

It was observed that using higher lock-in frequency for lower  resistance   $(<\!45\Omega)$   provides a valid, more precise and accurate  defect site. The optimized frequency setting was then applied to  a sample with electrical short of   $40~\Omega$   between two adjacent  pins (6 and 7).

Setting the lock-in frequency to   $10\,\textrm{Hz}$   and the voltage and  current limit to obtain a   $1\:\mathrm{\mW}$   power dissipation with 60  seconds exposure time, detected a valid hotspot between the  wire bonds connected to the failing pins 6 and 7. The hotspot is  concentrated on a single location which indicates a more  accurate and precise defect site. Figure 2 shows the LIT result  with lock-in frequency  $=10\mathrm{Hz}$  .

![  MAX9259      GTN/V-734      NQVBZRG          OverlayX-rayimage  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/445b5747-5ff9-413d-b649-205d62439f0c/445b5747-5ff9-413d-b649-205d62439f0c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215641%3B1743219241&q-key-time=1743215641%3B1743219241&q-header-list=host&q-url-param-list=&q-signature=b045d85140e6c8f8426b61d9575b92e80777f696)
Fig. 2. LIT and overlay X-ray images with lock-in frequency  $=10\mathrm{Hz}$

Since a valid hotspot was observed during LIT indicating a  precise and accurate failure location, the next FA step is X-ray  inspection. Normal 2D X-ray inspection and pseudo-colour  option did not reveal anomaly coincident with the valid hotspot.  We have tried changing the voltage and current on X-ray, but  still, no   anomaly was observed. Figure 3 shows the 2D X-ray  inspection images.

![PP  Pseudo-Colour  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f3e29640-2409-4ef6-9bbc-cdd66047a685/f3e29640-2409-4ef6-9bbc-cdd66047a685.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215641%3B1743219241&q-key-time=1743215641%3B1743219241&q-header-list=host&q-url-param-list=&q-signature=6a5eb3c48e4a73f83d93b81cfb9783e7ed544653)
Fig. 3. 2D X-Ray images showing no obvious anomaly

The device is subjected to 3D X-ray focusing on the valid  hotspot location. A suspected defect coincident with the valid  hotspot was noted. The suspected defect was observed by  setting the noise unfiltered. When the noise was filtered, the  suspected defect was also filtered and cannot be observed  anymore. Figures 4 and 5 show the 3D X-ray inspection  images.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7df5cbfa-74a7-4869-a113-71f2b1ffce4a/7df5cbfa-74a7-4869-a113-71f2b1ffce4a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215641%3B1743219241&q-key-time=1743215641%3B1743219241&q-header-list=host&q-url-param-list=&q-signature=fd6e39bd14d482c885462aa0edb44d42ffdf6992)
Fig. 4.  3D X-ray images showing no anomaly with noise filtered.

![Suspecteddefect  coincidenfwith  the valid hotspot  P  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5c7a8fb8-e330-4fae-9036-1ed895837660/5c7a8fb8-e330-4fae-9036-1ed895837660.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215641%3B1743219241&q-key-time=1743215641%3B1743219241&q-header-list=host&q-url-param-list=&q-signature=c77b4bc6741d2c15196d562950484a7aee3cc499)
Fig. 5.  3D X-ray image showing the suspected anomaly with   noise unfiltered.

## Destructive Analysis (Package polishing)  

Since an accurate defect location has been detected, destructive  analysis through successive package polishing and optical

inspection was pursued. Foreign material was observed  between the wire bonds connected to pins 6 and 7 coincident  with the suspected anomaly observed during 3D X-ray  inspection. Figure 6 shows the optical image (dark field) of the  defect.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/425c5f38-0794-411a-b445-34bc7ae64e9f/425c5f38-0794-411a-b445-34bc7ae64e9f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215641%3B1743219241&q-key-time=1743215641%3B1743219241&q-header-list=host&q-url-param-list=&q-signature=82cba5ee5099c69924a64bfa31f2e9784512bf80)
Fig. 6. Optical image (dark field) showing the defect

## EDX (Energy Dispersive X-ray) Analysis  

Energy Dispersive X-Ray (EDX) analysis of the observed  foreign material showed high peak of Silver (Ag). Figure 7  shows the EDX result.

![New Project(127)_pt1  14000  12000  10000  8000  6000  4000  2000  S  klm -46-Pd   kev  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7d17a800-6285-4c24-b04f-c5fe61b989fa/7d17a800-6285-4c24-b04f-c5fe61b989fa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215641%3B1743219241&q-key-time=1743215641%3B1743219241&q-header-list=host&q-url-param-list=&q-signature=29268f6bf0dfb33be584a1d814cfaf6a10fc8918)
Fig. 7.  EDX result detected high Ag peak

Root-cause Analysis

The foreign material is primarily consisting of Silver (Ag).  There are two possible sources of Silver material during  assembly process. One is from leadframe plating and the other  from epoxy die attach. By using EDX for the element weight  $\%$

comparison, it shows that the silver foreign material is most  likely from leadframe plating and not from epoxy die attach.  Table 1 shows the element weight  $\%$   comparison result.

||Foreign material|Leadframe plating|Epoxy die attach|
|---|---|---|---|
|Silver (Ag) element weight %|93%|92%|15%|


Table. 1 Element weight   $\%$   comparison of Ag from different sources

## III. RESULTS AND DISCUSSION  

The characterization of lock-in frequency based on resistance  for a single layer die QFN package showed that using higher  lock-in frequency for low resistance failure provides a valid,  more precise and accurate defect site. With this observation, a  low resistance failing device was subjected to LIT at higher  frequency (10Hz) and resulted to an exact failure location.  Based on physical failure analysis, the device is failing due to a  foreign material between the wire bonds connected to pins 6  and 7 which causes short. The foreign material is primarily  consisting of Silver (Ag). Since it is thin and silver has lower  density than gold, it is not easily being detected even by 3D  X-ray. The root-cause of the defect was determined from the  assembly process using EDX (Energy Dispersive X-ray)  analysis. By comparing the Silver element weight   $\%$   of the  foreign material to the assembly processes which uses Silver, it  shows that the silver foreign material is most likely from  leadframe plating.

## IV. CONCLUSION  

The case study has shown that using the correct Lock-in  Thermography frequency setting can increase the accuracy of  thermal detection on package level samples.   Combining the  fault isolation result with other non-destructive techniques like  3D X-Ray can achieve almost  $100\%$   success rate of finding the  physical defect.  Other techniques such as EDX has provided  additional data leading to accurate root cause investigation and  corrective actions.

It is recommended to have more case studies about the  characterization based on resistance, thickness of package and  power dissipation for easier and accurate use of LIT system.  Also, higher X-ray sensitivity for detection of thin and low  density material is needed for accurate package defect location.

## A CKNOWLEDGMENT 

The authors would like to thank Zhiyong Wang and Jerome  Escobedo, Failure Analysis Department, for the support in  completing this technical paper.

## R EFERENCES 

1.    Naoki Seimiya, et. al,  $2\pmb{\theta}^{t h}$   IEEE International  Symposium on the Physical and Failure Analysis of  Integrated Circuits (IPFA) , 2013, 337–340.     2.    Yu Chi Wang, et. al,  $24^{t h}$   IEEE International Symposium  on the Physical and Failure Analysis of Integrated  Circuits (IPFA) , 2018       3.    Rudolf Schlange, et. al,  37th International Symposium   for Testing and Failure Analysis , 2011      4.    Kannu Wadhwa, et. al,  21 st   IEEE International  Symposium on the Physical and Failure Analysis of  Integrated Circuits (IPFA) , 2014


