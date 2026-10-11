---
title: "138_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_46a695763d72d3bb34b1cdd372d6e51f7295230462135641
file_size: 1164425
---

## TOF-SIMS Analytical Method for Gate Oxide  Breakdown Voltage Shift Failure  

Lei Zhu 1 , Lingling Teo 1 , Yanfei Zhao 2 , Henry Leong 1 , Penny Long 1 , Younan Hua 1 , Xiaomin Li 1,2  Hao Zhou 3 , Qian Chen 3

1 Wintech Nano-Technology Services Pte. Ltd.  10 Science Park Road, #03-26, Singapore 117684, Singapore   2 Wintech-Nano (Suzhou) Co., Ltd.  Room 507, Building 09, Northwest District, Nano City, No. 99, Jinjihu Ave, Suzhou Industrial Park, Suzhou, China 215123  3 China Resources Microelectronics Limited, 14 Liangxi Lu, Wuxi, JiangSu Province, China  Phone : (+65)90027916, Email :  zhulei@wintech-nano.com

Abstract —Traditional failure analysis for gate oxide (GOX)  breakdown voltage (BV) shift involves electrical fault isolation  of the defect and wright etch to discriminate plasma induced  defects or contamination. To further nail down the root cause of  the contamination, secondary ion mass spectrometry (SIMS) is  proposed due to its superior detection sensitivity at ppm or ppb  level and superior mass resolution to determine the foreign  elements or materials unambiguously. In this paper, a PMOS  device failure was found to be gate oxide breakdown voltage  shifted down. Time-of-Flight (TOF) -SIMS depth profile is thus  used for the all-elements search mode analysis to figure out the  contamination, which is consistent with the inline process  commonality analysis results.

Keywords—GOX BV failure, TOF-SIMS, implant, PMOS

## I.    I NTRODUCTION 

As the technology advances toward 5nm or smaller tech  nodes, more quality requirement is demanded for gate oxide  in terms of dielectric property, defect density, contaminationfree, and interface uniformity. As such, to analyse gate oxide  integrity and dielectric breakdown related failures becomes  more important [1,2]. Traditionally the electrical fault  isolation was firstly used to locate the defect positions using  emission microscopic tools such as EMMI or OBIRCH.  Subsequently focus ion beam (FIB) was used to prepare the  defect lamella, which was then viewed by transmission  electron microscopy (TEM) to find out the basic feature and  nature of the defects. However, without the enough elemental  detection sensitivity, in some cases, the root cause is still not  clear. For GOX failure investigation in wafer fabrication  processes, the enhanced detection sensitivity for short-loop  wafers can be achieved by use of the Vapor Phase  Decomposition (VPD) and Inductively Coupled Plasma Mass  Spectrometry (ICP-MS). The ICP-MS technique sensitivity is  at ppb to ppt level and is mostly for metal ions. This enhanced  sensitivity enables effective investigation of contamination  caused by specific process. For finished wafer, the ICP-MS  may not be applied as the test key or actual gate oxide size is  too small for VPD droplet scan area requirement [3].

In this paper, a PMOS GOX failure was found to be gate  oxide breakdown voltage shifted down. We propose to use  Wright Etch and secondary ion mass spectrometry (SIMS)  analysis techniques in combination to identify the root cause  of the GOX failures after electrical FA fault isolation. Firstly,  Wright Etch is to use chemicals etch on silicon to generate  various shapes for different defect types due to the preferential  lattice orientation etching. The shape of the defect might give

indication on the GOX failure which may be related to plasma  induced defects (PID) or foreign contamination [1]. If it is due  to foreign contamination, Time-of-Flight (TOF) -SIMS is  used to further determine the contamination source at ppm to  ppb level. The additional advantage of SIMS is that it is  particularly sensitive to dopant concentration if the implant  issue is involved in the GOX failures.

![II.    EXPERIMENTS  E XPERIMENTS   GOX  GOX    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e907849c-697e-4e79-9fd3-740462afed2c/e907849c-697e-4e79-9fd3-740462afed2c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215847%3B1743219447&q-key-time=1743215847%3B1743219447&q-header-list=host&q-url-param-list=&q-signature=c362604d06f3e632139140753293daeac1d3f743)
Fig. 1. Illustration of the GOX test key

The sample is a finished wafer with test breakdown  voltage shifted from 4V down to 1V or less. The gate oxide  thickness is 30A. The test pad of the GOX is illustrated in Fig.  1. The failed wafers have been tested with EMMI showing  random hot spots on the GOX area.

As the dimension of the GOX test key is from 30um in  width and 100um in length, it is suitable for TOF-SIMS depth  profile analysis. One good and one bad sample are carefully  delayered until polySi for TOF-SIMS analysis. TOF-SIMS  data were collected using a TOF-SIMS 5 instrument (IONTOF GmbH) in dual-beam mode. The sputter beam (O2 or Cs  source) was at 1KeV with a current of 17nA raster scanned  over an area of   $30\mathrm{x}30~\upmu\mathrm{m}2$  . A short-pulsed (10 ns) primary  ion beam (Bi1 +, 25keV energy,   ${\sim}1$   pA measured sample  current) was raster over a   $10\times10~\upmu\mathrm{m}2$   area at the center of the  sputter beam spot. The analysis was acquired at a base  pressure of about  $5\times10–8$   mbar with the primary ion beam  set in high current bunched mode. Effective charge  compensation was obtained by using an electron flood gun  (20eV). All detected secondary ions had either negative or  positive polarity and mass resolution >4000 (m/δm) [4].

## A.   Wright etch  

The optical microscope and SEM image of the GOX area  of bad sample is shown in Fig. 2 and Fig. 3 respectively.  Obviously, there are no corresponding Si defect found from  the Wright etch. It is quite confusing as no sign of defects  associated with the GOX failure. From the Wright etch results,  one thing is confirmed that it is not due to PID. However, it is  not sure if the phenomena of no defect sign might be due to  the quantity of contamination that is beyond the sensitivity of  the Wright etch test. Therefore, TOF-SIMS analysis has to be  approached directly.

![Laser mark for  Laser mark for  analysis location  analysis location     ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3dbf41b4-65d5-4fc6-a0ce-ff6788e3e47a/3dbf41b4-65d5-4fc6-a0ce-ff6788e3e47a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215847%3B1743219447&q-key-time=1743215847%3B1743219447&q-header-list=host&q-url-param-list=&q-signature=e1f8de618d4c99ff34244ecdbc19b8e5002eb3dc)
Fig. 2. Optical microscope image of the GOX area of bad sample after  Wright etch

![IProbe=80pAMag=1.00KX   WD = 4.8 mm   EHT= 2.00kV   SignalA=SE2   ESB Grid= 500  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1354ac8e-b6cb-4cc7-bb79-2b31bfd8a1b1/1354ac8e-b6cb-4cc7-bb79-2b31bfd8a1b1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215847%3B1743219447&q-key-time=1743215847%3B1743219447&q-header-list=host&q-url-param-list=&q-signature=599cd2537d80ffb69194aa3b7ef1c7c65e1b8968)
Fig. 3. SEM image of the GOX area of bad sample after Wright etch

## B.   TOF-SIMS depth profiles  

Fig. 4 and Fig. 5 show the optical images of the GOX  analysis area for good and bad samples respectively. The  analysis area has to be within the boundary of the GOX test  pad to avoid any interference from possible surrounding

structures. These neighboring structures may or may not  contain the contamination of interest.

![TOF-SIMS  TOF-SIMS  analysis area  analysis area    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/84ab69f3-ccaa-41c1-a0f8-bb0142fadb16/84ab69f3-ccaa-41c1-a0f8-bb0142fadb16.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215847%3B1743219447&q-key-time=1743215847%3B1743219447&q-header-list=host&q-url-param-list=&q-signature=f47f4ba43833273d30039dba6c8a6230700c8601)
Fig. 4. TOF-SIMS analysis area for good sample

![TOF-SIMS  TOF-SIMS  analysis area  analysis area  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/36ae5076-a610-49e9-b2a7-c5db9d547c94/36ae5076-a610-49e9-b2a7-c5db9d547c94.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215847%3B1743219447&q-key-time=1743215847%3B1743219447&q-header-list=host&q-url-param-list=&q-signature=ae9269d4b7f43cc5c532fd4bcadb46a4adf7a00a)
Fig. 5. TOF-SIMS analysis area for bad sample

Fig. 6 show the   $\mathrm{Na+}$   ion depth profiles of the GOX for  good and bad samples respectively. From the depth profile  analysis, the delayering for both samples may or may not  exactly stop at the poly which has the feature of CoxSiy  silicide (not shown). However, that doesn’t affect the depth  profile analysis from the poly down to the gate oxide layers.

The small bump on the Si ion depth profile corresponds to  the gate oxide region. The SiO2 depth profile shows more  obvious bump right at the same depth of the gate oxide region.  The   $\mathrm{Na+}$   ion (red line) detected from the bad sample has a  much higher peak than that detected from the good sample  (blue line) around the GOX region before disappearing into Si  substrate sharply. The level of the Na could be at lower ppm  level from the TOF-SIMS assessment, and it might be the  reason why Wright etch may not show the defect formation in

the earlier experiment. From the depth profile comparison  between the good and bad sample, distinct difference of the   $\mathrm{Na+}$   spike around the GOX region is observed. Fig. 7 shows  the positive depth profile for   $\mathrm{Ca+}$   ions. Similar to   $\mathrm{Na+}$   depth  profile results, the  $\mathrm{Ca+}$   ions are higher in the GOX region for  bad sample than that in good sample. Fig. 8 shows the   $\mathrm{K}+$   ion  depth profile. The  $\mathrm{K}+$   ion shows a higher spike from the bad  sample than that from the good sample in the GOX region as  well. For comparison purpose, we have also caried out similar  analysis for other metallic ions such as   $\mathrm{Fe+}$   and   $\mathrm{Cu+}$  . Fig. 9  and Fig. 10 showed the   $\mathrm{Fe+}$   and   $\mathrm{Cu+}$   depth profiles  respectively. The   $\mathrm{Fe+}$   shows noise level along the depth  especially at GOX region for both bad and good samples. The   $\mathrm{Cu+}$   shows no counts along the depth at the GOX region. It  means both  $\mathrm{Fe+}$   and  $\mathrm{Cu+}$   are not present throughout the poly  to GOX. The same analysis process for all other elements has  been performed, however, no abnormality for other metallic  ions like  $\mathrm{Fe+}$   and  $\mathrm{Cu+}$   has been found. After checking through  the GOX process in the manufacturing, the distinct   $\mathrm{Na+}/\mathrm{K+}/\mathrm{Ca+}$   ions could come from one of its furnace  chambers because after thorough cleaning of the chamber the  failure didn’t appear again. These  $\mathrm{Na+}/\mathrm{K+}/\mathrm{Ca+}$  metallic ions  are quite mobile. If they are present in the gate oxide layer, it  is not surprised that lower breakdown voltage failures will be  caused [5].

![1.E+05  1.E+05  1.E+03  1.E+03 Si  Si 1.E+04  1.E+04 SiO2  SiO2 Intensity (arb.unit.)  1.E+O2  1.E+02 1.E+03 1.E+03  1.E+02 1.E+02  Na-bad  Na - bad 1.E+01  1.E+01 IsU  1.E+01 1.E+O1  Na - good Na-good  1.E+0O  1.E+00  1.E+0O  1.E+00 0  200 200   400  400  600  600 Depth (nm)  Depth (nm)   ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2f1a64a7-b0e3-4b1a-a000-7c83f6f43629/2f1a64a7-b0e3-4b1a-a000-7c83f6f43629.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215847%3B1743219447&q-key-time=1743215847%3B1743219447&q-header-list=host&q-url-param-list=&q-signature=ea1dc1f5eeeddb125f5e1cac4b218f913a6ff2f8)
Fig. 6. Positive TOF-SIMS depth profile for  $\mathrm{Na+}$   ions

![1.E+03  1.E+03  1.E+O5  1.E+05 Si  Si 1.E+04   1.E+04 Intensity (arb.unit.) 1.E+02  1.E+02 n   1.E+O3  1.E+03 SiO2  SiO2 1.E+O2  1.E+02 1.E+O1  1.E+01 Ca-good  Ca - good  Ca - bad  Ca - bad 1.E+O1  1.E+01 1.E+00 1.E+0O   1.E+00  1.E+00 0  200  200  400  400  600  600 Depth (nm)  Depth (nm)   ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3e51c74d-1f83-439c-834a-249aca18d8a4/3e51c74d-1f83-439c-834a-249aca18d8a4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215847%3B1743219447&q-key-time=1743215847%3B1743219447&q-header-list=host&q-url-param-list=&q-signature=732c611e628b3bf150257ad6a5f3cebebcae30aa)
Fig. 7. Positive TOF-SIMS depth profile for   $\mathrm{Ca+}$   ions

![1.E+05  1.E+05  1.E+03  1.E+03 Si 1.E+04  1.E+04 SiO2  SiO2 1.E+O2  1.E+02 1.E+03  Intensity (arb.u.) 1.E+03 ≥1.E+02  1.E+02 1.E+O1  1.E+01 K - good  K-bad  K - bad 三 1.E+01  1.E+01 1.E+OO  1.E+00  1.E+OO  1.E+00 0  200  200  400  400  600  600 Depth (nm)  Depth (nm)   ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ad016fe6-0661-4a04-a8a5-4bfa3a760728/ad016fe6-0661-4a04-a8a5-4bfa3a760728.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215847%3B1743219447&q-key-time=1743215847%3B1743219447&q-header-list=host&q-url-param-list=&q-signature=580599f970869ced529fca8096c16e9d088bc0c9)
Fig. 8. Positive TOF-SIMS depth profile for   $\mathrm{K}+$   ions

![1.E+05  1.E+05  1.E+03  1.E+03 SA  Si  1.E+04  1.E+04 SiO2  SiO2 1.E+O2  1.E+02 Intensity (arb.u.) 1.E+03 1.E+01  1.E+02 1.E+O1  1.E+01 Fe - good  Fe - good 1.E+O1  1.E+01 1.E+OO  1.E+00  1.E+OO  1.E+00 C  0  200  200  400  400  600  600 Depth (nm)  Depth (nm)   ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/29168adc-d89f-4030-8204-4f6222eadb32/29168adc-d89f-4030-8204-4f6222eadb32.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215847%3B1743219447&q-key-time=1743215847%3B1743219447&q-header-list=host&q-url-param-list=&q-signature=daf60d93598393873e951c34e2d099b009f144ce)
Fig. 9. Positive TOF-SIMS depth profile for   $\mathrm{Fe+}$   ions

![1.E+05  1.E+05  1.E+03  1.E+03 Si  Si 1.E+O4   1.E+04 1.E+O2  1.E+02 1.E+03  Intensity (arb.u.) 1.E+03 SiO2  SiO2 ≥1.E+02  1.E+02 1.E+01  1.E+01 三 1.E+01  1.E+01 Cu-good  Cu - good Cu-bad  Cu - bad 1.E+OO  1.E+00  1.E+0O  1.E+00 C  0  200  200  400  400  600  600 Depth (nm)  Depth (nm)   ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/acf7e551-db43-47b5-a69c-5bae063d284e/acf7e551-db43-47b5-a69c-5bae063d284e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215847%3B1743219447&q-key-time=1743215847%3B1743219447&q-header-list=host&q-url-param-list=&q-signature=b195d739d8b496dd5d221a7c250c17bccc385539)
Fig. 10. Positive TOF-SIMS depth profile for  $\mathrm{Cu+}$   ions

## IV.    C ONCLUSIONS 

TOF-SIMS depth profile analysis was used for the GOX  BV failure on both the good and bad samples. It is found  abnormal   $\mathrm{Na+}$  ,  $\mathrm{Ca+}$   and   $\mathrm{\bar{K}+}$   mobile ions distribution in gate  oxide in bad sample as compared to good sample, which is  believed to be the root cause of the gate oxide breakdown  voltage shift failures.

## A CKNOWLEDGMENT  

The authors would like to thank engineers from GFA of  Wintech Nano-Technology Services Pte. Ltd. for their help in  sample preparations.

## R EFERENCES 

[1]    Y. N. Hua, G. B. Ang, S. Redkar and Yogaspari, “Failure Analysis of  Contamination and Gate/Tunnel Oxide Failure in Wafer Fabrication”,  ISTFA 2001: Proceedings from the 27th International Symposium for  Testing and Failure Analysis, 11-15 Nov, Santa Clara, CA, USA,  pp.425-430    [2]    Y.N. Hua, S. Chu, D. Gui, Z.Q. Mo, Z.X.Xing, B.H.Liu, A.Ng and  T.Tsai, “A New Failure Analysis Flow of Gate Oxide Integrity Failure  In Wafer Fabrication”, ISTFA 2001: Proceedings from the 35th  International Symposium for Testing and Failure Analysis, November  15–19, 2009, San Jose, California, USA, p 177-181    [3]    M. Beebe, S.Anderson, “Monitoring wafer cleanliness and metal  contamination via VPD ICP-MS: Case studies for next generation  requirements”, Microelectronic Engineering, vol.87, pp1701-1705,  November 2010    [4]    L. Zhu, H.W.Teo, K. Ong, Y.H.Huang, Y.N.Hua, “Time-of-Flight  Secondary Ion Mass Spectroscopic Characterization of the Nitrogen  Profile of Shallow Gate Oxynitride Thermally Grown on a Silicon  Substrate”, Surface and Interface Analysis, vol.44, pp1558-1564, May  2012    [5]    S. Lombardo, J.H.Stathis, B.P.Linder, K.L.Pey, F.Palumbo, &  C.H.Tung, “Dielectric breakdown mechanisms in gate oxides”, Journal  of Applied Physics, vol. 98(12), pp121301-36, December 2005

