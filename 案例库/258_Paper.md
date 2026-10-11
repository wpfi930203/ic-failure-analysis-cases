---
title: "258_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_60d664798eabc774e481eb4aa626961c7295230462135641
file_size: 1224269
---

## Defect Location and Physical Analysis in  Chip-on-chip Device  

Zhibin Wang 1\* , Zhaoxi  $\mathrm{{W}u^{1}}$  , Jiajia  $\mathrm{Sun}^{1}$  , and Chao Duan 1   1   China Aerospace Components Engineering Center(CACEC), Beijing 100094, People’s Republic of China.  \* Phone: +86 6811 3476 Fax: +86 6874 6312 Email: wzb_1984@126.com

Abstract-   The failure analysis (FA) case of devices with short  defect is illustrated in this paper. First, X-ray microscopy reveals  the device package to be a chip-on-chip (CoC) type package.  Lock-in thermography (LIT) was then used to locate the short  position, including its XY position and Z-depth (upper or lower  die). Subsequently, three-dimensional (3D) X-ray was applied to  clarify the connecting relationship between the failed pin and the  bonding wire, further confirming whether the defect was on the  upper or lower die. To verify the defect location, the devices were  decapped and the short defect was confirmed by using optical  beam induced resistance change (OBIRCH) and focused ion beam  (FIB). The case study in this paper demonstrates the application of  several FA techniques used for advanced packaging device and  provides references for the defect location and physical analysis of  similar device.

Keywords  –  Defect location, Physical analysis, CoC package, FA  techniques .

## I. I NTRODUCTION 

Due to the advancement of process technologies, the  construction of integrated circuits (IC) becomes increasingly  complex: more levels of metal interconnect is realized to meet  the requirement of fast increasing number of transistors on a  die, and complicated 3D package like stacked die is widely used  to integrate the different chips into one package[1]. All these  developments put forward great challenges to the traditional  failure analysis tools[2]. Fortunately, the emergence of several  new technologies are able to meet the failure analysis demands  on such complicated ICs, which include defect location and  physical analysis[3, 4]. Using a case study of a short failure on  two CoC devices, this paper demonstrates the application of  some of these new failure analysis tools and provides references  to the defect location and physical analysis of similar  complicated device.

## II.   NEW   FA   TECHNIQUES  

As mentioned above, several new FA techniques are  developed for complicated ICs, such as LIT, 3D X-ray. These  new techniques, together with the traditional ones, are effective  in the FA of complicated ICs. The principles of these new  techniques are introduced in this section.

3D X-ray: As the most advanced X-ray technique, X-ray  computed tomography (CT), also called 3D X-ray, could realize  section scanning and 3D imaging[5, 6]. By the rotating sample  stage, the X-ray source radiates the sample from different  angles. Correspondingly, the 2D X-ray image of each angle is  received by the detector during the sample rotation. Finally, all

the 2D images are reconstructed to form the 3D image of the  sample through special computer program. The virtual section  image could be displayed at any position or in any direction of  the sample by post processing of computer program.

LIT: As an emerging non-destructive technique, LIT is  applied to determine the XYZ position of the defect[3, 7, 8]. By  pulsing the short defect with current of specific frequency, the  heat signal propagates from the source to the device surface and  causes the periodic temperature variation of the same frequency.  Indium-Antimonide (InSb) camera is adopted to image the  hotspot on the device surface to determine the XY position of  the defect. The Z depth information of the defect could be  obtained by testing the phase shift between the electrical  stimulation and the thermal response at the surface. The shift  results from the propagating path, including the material and its  thickness. For the same device, the larger shift corresponds to  deeper short defect.

Besides the above new emerging techniques, the  existing  techniques, such as OBIRCH[9] and FIB[10], are also the  powerful tools in the defect location and physical analysis of  complicated IC. In the next section, a detailed failure case study  illustrates the application of these techniques in the advanced  packaging device.

## III. FAILURE   CASE   STUDY  

A short failure occurred between I/O and ground pins in two  plastic ball grid array (PBGA) devices (labeled 1# and 3#, as  shown in Fig.1) after electro-static discharge (ESD) test. The  failure pin is P9-L7 and N8-M10 for 1# and 3# device  respectively, which was verified by curve trace as shown in  Fig.2.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b0bbf94d-213e-4fea-b760-474b8ff58851/b0bbf94d-213e-4fea-b760-474b8ff58851.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215675%3B1743219275&q-key-time=1743215675%3B1743219275&q-header-list=host&q-url-param-list=&q-signature=732492876220234634ca5db2768e1c866cf62323)
Fig. 1 The appearance of the PBGA device

![Cap  (a)     (b) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e1111800-997e-4c7e-a8a4-2004670ca10c/e1111800-997e-4c7e-a8a4-2004670ca10c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215675%3B1743219275&q-key-time=1743215675%3B1743219275&q-header-list=host&q-url-param-list=&q-signature=7e95431fd59352f8ecd95bd7bc58235b6bc68727)
Fig. 2 Curve trace for two failed devices, (a) 1# and (b) 3#, blue and red lines  representing the I-V curve before and after ESD test.

X-ray was applied on the device to clarify the inside  construction. As shown in Fig.3, one chip stacks above the  other with an interposer die to form a CoC construction, the  wire bonding is used to realize the connection from the chip to  the substrate. However, it was impossible to correspond the  failed pin ball to the inner bonding wire just based on this X-ray  photo. Therefore it cannot be determined whether the short  defect located on the upper or lower die.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5dd3dfad-ce14-4eda-96f0-ec2d0b60359e/5dd3dfad-ce14-4eda-96f0-ec2d0b60359e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215675%3B1743219275&q-key-time=1743215675%3B1743219275&q-header-list=host&q-url-param-list=&q-signature=d95acceeb4c639b4b255a9fc544c741b2946cc14)
Fig. 3 The X-ray photo of the failed device

In order to locate the XYZ position of the short defect, LIT  was used for the two devices, as shown in Fig.4. The hotspot  shown in the thermograph indicated the defect location in the  XY plane. The applied lock-in frequencies ranged from 1 to 10  Hz. The phase shift between the electrical stimulation and the  thermal response was measured for the two failed devices.  According to the LIT principle, the phase shift is larger when  the short defect is deeper away from the top surface of the  plastic package[7]. Therefore, by comparing the phase shift  shown in Fig.3, it can be concluded that the defect was on the  upper die for 1# device while on the lower die for 3# device.

![(a)    (b) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/464fc207-e42a-4b7e-af6a-cc24fbdd4c67/464fc207-e42a-4b7e-af6a-cc24fbdd4c67.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215675%3B1743219275&q-key-time=1743215675%3B1743219275&q-header-list=host&q-url-param-list=&q-signature=7a26fd1f71477b77637e6b2f26284dc5f82cd907)
![300  280   CCU  (c) 260  240  220  200  lock-in frequency, Hz  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/972ce68d-ee6a-481a-b76c-58f235da9b0e/972ce68d-ee6a-481a-b76c-58f235da9b0e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215675%3B1743219275&q-key-time=1743215675%3B1743219275&q-header-list=host&q-url-param-list=&q-signature=272fd0f61895cf9e4f81ae3be4bbb91089d41a34)
Fig. 4  LIT results of the two failed devices: hotspot of (a)1# and (b) 3#, (c)  phase shift measurement of the two failed devices

As mentioned above, traditional 2D X-ray is unable to  determine the connection between the pin ball and the bonding  wire. Therefore 3D X-ray was adopted to illustrate the  connection, further confirming whether the defect was on the  upper or lower die. As shown in Fig.5(a), the 3D image of the  device illustrated that the short bonding wires connect to the  lower die while the long bonding wires connect to the upper die.  The section scan results (Fig.5(b)) of 3D X-ray revealed that  P9\L7 pin balls connect with the upper die while N8\M10 pin  balls connect with the lower die, which further confirms that the  defect was on the upper die for 1# device while on the lower die  for 3# device.

![CaD  (a) (b)   ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1eec8437-c350-465b-beb6-584757d18a2c/1eec8437-c350-465b-beb6-584757d18a2c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215675%3B1743219275&q-key-time=1743215675%3B1743219275&q-header-list=host&q-url-param-list=&q-signature=b1daab0a4ed804c0abe27e4d452307d4c6827b14)
After the above nondestructive fault isolation, the failed  devices were decapped with acid. The OBIRCH was done on  the upper die of 1# device and lower die of 3# device from  backside. As shown in Fig.6, the emission spots were clearly  detected.

![(a) CaD  (b)     ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/988881f9-f1c0-41e8-bfa9-5d2d0ce169a8/988881f9-f1c0-41e8-bfa9-5d2d0ce169a8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215675%3B1743219275&q-key-time=1743215675%3B1743219275&q-header-list=host&q-url-param-list=&q-signature=bc81336d02c3b4557bea64a02b75c0162fd9f244)
Fig. 6  The backside OBIRCH results (already mirroring for defect location  from die front)of (a) upper die of 1# device and (b) lower die of 3# device

For 1# device severe burn out was found when observed from  the front of the upper die, as shown in Fig.7(a). However, no  abnormality was found for the lower die of 3# device. FIB was  used to show the defect, as shown in Fig.7(b).

![(a)     (b) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c65a6958-86d9-4ccb-aaea-73354e45e702/c65a6958-86d9-4ccb-aaea-73354e45e702.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215675%3B1743219275&q-key-time=1743215675%3B1743219275&q-header-list=host&q-url-param-list=&q-signature=c8ff872640f379486acab5339afcc5fadb96cc0f)
Fig. 7  Optical microscopy of upper die of 1# device and (b) FIB results of lower  die of 3# device

The physical analysis results matches well with the  nondestructive   defect   location   before   decap.   It   also  demonstrates the effectiveness in such techniques.

## IV. C ONCLUSION 

Through the case study on a short failure in a type of CoC  device, this paper illustrates the new techniques used in the  failure analysis for advanced packaging, including defect  location and physical analysis. The physical analysis results  matches well with the nondestructive defect location, which  provides references for the failure analysis of device with  similar advanced packaging.

## A CKNOWLEDGMENT 

The authors would like to thank colleagues from CACEC for  their technical support and useful discussion during this study.

## R EFERENCES 

[1]    D. Deng, F. S. Wu, L. Z. Zhou,  et al.,  “3D package and its latest research”,  Microelectron. Devic. Tech. , vol. 47(7), pp. 443-450, 2010.    [2]    D. P. Vallett, “From Microns to Molecules-Can FA Remain Viable  Through the Next Decade?”,  28th Int. Symp. Testing. Fai. Anal.(ISTFA) ,  pp. 11-20, 2002.     [3]    C. L. Henderson, “Failure analysis techniques for a 3D world”, Microelectron. Reliab. , vol. 53, pp. 1171-1178, 2013    [4]    X. L. Chen, G. H. Yuan, G. N. Xu,  et al ., “Advanced fault localization  techniques in microelectronics failure analysis”  Int. Conf. Reliab. Main.  Safety(RMS) , pp. 3-9, 2014    [5]    S. M. Zulkifli, B. Zee, W. Qiu,  et al ., “High-res 3D X-ray microscopy for  non-destructive failure analysis of chip-to-chip micro-bump interconnects  in stacked die packages”,  24th IEEE Int. Symp. Phys. Fail. Anal.  ICs(IPFA),  pp. 1-5, 2017.    [6]    D. T. Lin, Z. Sun, “Application of three-dimensional X-ray microscopy in  failure analysis for plastic encapsulated microelectronics”,  17th Int. Conf.  Electron. Packag. Tech.(ICEPT) , pp. 1284-1287, 2016.    [7]    W. Qiu, B. Zee, H. Deslandes,  et al .,   “Defect Z-depth determination in  flip-chip using lock-in thermography”,  24th IEEE Int. Symp. Phys. Fail.  Anal. ICs(IPFA),  2017.     [8]    C. Schmidt, F. Altmann, “Non-destructive defect depth determination at  fully packaged and stacked die devices using Lock-in Thermography”,  17th IEEE Int. Symp. Phys. Fail. Anal. ICs(IPFA),  pp. 1-5, 2010.    [9]    F. Beaudoin, G. Imbert, P. Perdu,  et al ., “Current leakage fault  localization using backside OBIRCH”,  8th IEEE Int. Symp. Phys. Fail.  Anal. ICs(IPFA) , pp. 121-125, 2001.     [10]   S. K. Loh, HT Teo, S.P. Neo,  et al ., “Application of Focus Ion Beam  circuit edit in failure analysis”,  IEEE Int. Conf. Semi. Electron. , pp.  634-636, 2006.

