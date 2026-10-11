---
title: "123_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_05dbb9e86160d959449f77b89068ec847295230462135641
file_size: 1275990
---

## Using Higher Accelerating Voltage of SEM   to Dig Out Implant Defects   

1 Wen Cheng Hsu,  1 Yu Hsiang Shu, and  2 Chenglong Pan    1 United Microelectronics Co., Ltd.   No, 3,Li-Hsin Rd. II, Hsinchu Science Park, Taiwan 300, R.O.C.  2 United Semi (Xiamen) Co., Ltd.  No.899 Wan Jia Chun Road, Xiang’an District, Xiamen 361100, P.R.China   Tel: 886-3-5782258 ext.37748; Fax: 886-3-5782965 Email:  jaffer_hsu@umc.com

Abstract- Implant defects are difficult to discover because they are    not quantified easily and not like bridge or open physical defects    to   find   them   by   standard   FA’s   instruments    We can get electrical proof but hard to prove the relationship with    implant defects. Here we highlight a phenomenon by using                                              higher electron beam accelerating voltage of SEM (Scanning    Electron Microscope), through the different penetration depth of    electrical charges in silicon; we can observe the variation of    contrast images at abnormal area of SRAM to verify possible    implant defects.

##                           1. Introduction  

Voltage Contrast (VC) is a technology we are familiar with  and is widely used by FA analysis. In normal conditions, we  used to take low kV accelerating voltage of SEM or FIB at low  beam current mode to observe contact VC, through the  brightness or darkness images of sample’s surface; we can get a  hint and focus on   the difference to isolate the possible defect  locations. As we know, different intensity of electrical beam  means different penetration depth of electrons in silicon, for  instance, electrical beam can penetrate about the depth of 35nm  in the condition of 1kV accelerating voltage; 30kV can even  penetrate about the depth of 11um. Here we used these  characteristics and combined with repetitive structures of  SRAM, we found irregular bright area images that are different  from the images of contact VC and helped us to focus on the  difference quickly. After a series of analysis procedures like  C-AFM (Conductive Atomic Force Microscopy), SCM  (Scanning Capacitance Microscopy), SEM DC (Dopant  Contrast), chemical stain, an abnormal P Well implant issue  was finally found.

## 2. Case study  

The case here described was a 0.11um process product  which suffered a problem of open short failure. We used Good  VS.   Bad dies comparison and confirmed all bad dies had the  short problem as shown in Figure 1.

![1.00E-04  5.00E-05  0.00E+00  -5.00E-05  B3   B  B6  -1.00E-04  -0.5   0.5  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cb16542f-9f60-4ee5-9139-7b230a7da393/cb16542f-9f60-4ee5-9139-7b230a7da393.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215627%3B1743219227&q-key-time=1743215627%3B1743219227&q-header-list=host&q-url-param-list=&q-signature=c1c6298b1f12c377f65c1a164c713cb165b8cd43)
Fig. 1  Good VS. Bad die I-V curve comparison.

First of all, IR OBIRCH (InfraRed Optical Beam Induced  Resistance Change) technology was used to locate possible  directly.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f3955b07-dc00-440b-aac8-6fa8412f9700/f3955b07-dc00-440b-aac8-6fa8412f9700.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215627%3B1743219227&q-key-time=1743215627%3B1743219227&q-header-list=host&q-url-param-list=&q-signature=1c1d03655708f8ce5df024971b132fca3f17a7c0)
Fig. 2 Abnormal OBIRCH spot was found.

Then we took several samples to do layer by layer checking till  AA (Active Area) but no abnormality was found. In order to  clarify the root cause, we reviewed OBIRCH spots of bad  samples and chose the spots located in the SRAM block on  account of its repetitive structure. Also no abnormality was  found at BEOL (Back End of Line). So, we suspected front end  problem might be the key issue. Then we used low beam  current FIB to focus on contact layer, and some bright NMOS  VC contacts were found as shown in Figure 3.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3b65dbb9-6df2-4e17-a6b8-fd5f962efcf5/3b65dbb9-6df2-4e17-a6b8-fd5f962efcf5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215627%3B1743219227&q-key-time=1743215627%3B1743219227&q-header-list=host&q-url-param-list=&q-signature=632072c3318c8a010a479c910dd8fcb221a7c88d)
Fig. 3 Bright VC contacts of  NMOS were found.

We used C-AFM to scan the abnormal NMOS contact area, and  then we found not only the abnormal NMOS area which had the  leakage issue, but also the adjacent PMOS contacts which had  larger leakage phenomena than the abnormal NMOS area as  shown in Figure 4.

![Bias+1V   Bias-1v  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f214cb91-2906-4d40-9113-adb0812360ad/f214cb91-2906-4d40-9113-adb0812360ad.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215627%3B1743219227&q-key-time=1743215627%3B1743219227&q-header-list=host&q-url-param-list=&q-signature=29196a7c20ac81a62867b68e38d621bd56dab110)
Fig. 4 C-AFM current mapping at   $+1\mathrm{V}$   showed abnormality (yellow  dashed line area).

This abnormal image of C-AFM was obviously different from  FIB contact VC image. It’s difficult to clarify the whole  boundary by C-AFM because this area seemed too big. In order  to get a clear vision of defects .SEM VC was adopted when  increased the accelerating voltage of SEM from 0.7kV to 5kV;  no obvious defect could be found, but when we increased to  10kV, then an irregular bright area was found as shown in  Figure 5.

![patern  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/adf32864-1639-48a4-872a-368b646f42fb/adf32864-1639-48a4-872a-368b646f42fb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215627%3B1743219227&q-key-time=1743215627%3B1743219227&q-header-list=host&q-url-param-list=&q-signature=ac5936aa69670a1a146b27ab3bde3378d8c20714)
Fig. 5 Irregular bright area was found at 10kV (red dashed line area).

We initially thought it might be artificial defects, so we did the  same procedure to increase sample counts and the same  phenomenon was proved again in Figure 6.

![pe  ae  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/297b5cb8-07bc-41b1-917b-e2e88e5ff300/297b5cb8-07bc-41b1-917b-e2e88e5ff300.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215627%3B1743219227&q-key-time=1743215627%3B1743219227&q-header-list=host&q-url-param-list=&q-signature=edf838c029a77099af2ff1ca20cc12aa6be97e62)
Fig. 6 Same Irregular bright area was confirmed again (red dashed line area).

According to the results above, physical defect was excluded  and implant defects were suspected. We used X-S (cross  section) SEM DC technology to check implant profile and used  chemical stain to enhance their boundary, and in order to get a  clear relationship of P/N implant, SCM image was adopted as  shown in Figure 7-9.

![NMOS   PMoS   NMOS.  ST  PWell   P Well  Well bridge  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a850e735-1ef4-4b54-9425-9c3a082163c6/a850e735-1ef4-4b54-9425-9c3a082163c6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215627%3B1743219227&q-key-time=1743215627%3B1743219227&q-header-list=host&q-url-param-list=&q-signature=5161c096d9b41b77e17c45f96a1690f9edd9007e)
Fig.7(a)Bad die of X-S SEM  DC image.

![NMOS   PMoS   NMoS  SIUSOUO  P well   N Well   PWvell  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e90d3099-9cf9-4bff-943a-496948265567/e90d3099-9cf9-4bff-943a-496948265567.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215627%3B1743219227&q-key-time=1743215627%3B1743219227&q-header-list=host&q-url-param-list=&q-signature=b03fd01936f00a1acdeafc069f7f18b6e39c8765)
Fig. 7 (b) Good die of X-S SEM DC images.

![PMOS   PMOS  Mellbri  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ef67e717-d6af-4a5e-8cd7-ca341380e8b1/ef67e717-d6af-4a5e-8cd7-ca341380e8b1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215627%3B1743219227&q-key-time=1743215627%3B1743219227&q-header-list=host&q-url-param-list=&q-signature=c8d012bbab7b4ea00fefb2febf4c661684ebdd79)
Fig.8(a)Bad die of chemical stain image.

![MMOS   PMOS   MOS  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2a5a5ac8-dcb9-42b8-b00e-8cbb5103bde8/2a5a5ac8-dcb9-42b8-b00e-8cbb5103bde8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215627%3B1743219227&q-key-time=1743215627%3B1743219227&q-header-list=host&q-url-param-list=&q-signature=4d83b97381744aff84b8d17cba74b78c613630f4)
Fig.8 (b) Good die of chemical stain image.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/eef0657b-4372-4b7f-9109-77441a696416/eef0657b-4372-4b7f-9109-77441a696416.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215627%3B1743219227&q-key-time=1743215627%3B1743219227&q-header-list=host&q-url-param-list=&q-signature=b778fec7de94a5d37a6a1e4eb321371f00df9053)
Fig.9(a) Bad die of  SCM image .

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f626e249-b518-4292-a4fe-c753bf8c149e/f626e249-b518-4292-a4fe-c753bf8c149e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215627%3B1743219227&q-key-time=1743215627%3B1743219227&q-header-list=host&q-url-param-list=&q-signature=6100c0157ccc39fc6053dd1a6c17a4271516257c)
Fig.9(b) Good die of  SCM image.

As we obtained a clear picture that abnormal PWELL implant  induced this abnormality that phenomenon was hard to  discover in logic area because of its versatile structure, but with  the help of repetitive structure of SRAM combined with the  effect of deeper electrons penetration depth of SEM,  abnormality was eventually found.   We fed back this conclusion  to FAB quickly and the root cause of Photo Resist collapse was  found, problem was solved after related actions of correction.

## 3. Discussion   

The structure of SRAM is a good platform to help us find out  the root cause of abnormality because of their repetitive characteristics. The application of VC technology can be  expanded because of the increased penetration depth of  electrons in silicon. Here we discuss how FIB VC images and  higher accelerating voltage of SEM cause different  accumulation of electrical charges. According to FIB low beam  current contact VC images, bright and dark images only appear  at contacts that help us to observe the abnormality on shallow  depth area like source drain doping region of contact layer. In  this case, abnormal PWLL implant also influenced some   $\Nu+$  dopant concentration which induced early break down  phenomenon at abnormal NMOS and decreased the  accumulative potential of positive charge at abnormal NMOS  contacts, and this is the reason why some bright NMOS  contacts were found in FIB VC images. In addition, abnormal  PMOS contacts discharged positive charges similar to normal  PMOS contacts die, so no specific PMOS VC contact was  highlighted in FIB VC images.   I-V curve of C-AFM and the  secondary electrons productive model in FIB low beam current  mode is shown in Figure 10.

![IVcurveofabnormalPMOS   IVcurveofnormalPMOS  IVcurveofabnormalNMos   IVcurveofnormal NMOS  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/24e8961c-e905-4dd7-a1e4-3b23773192b1/24e8961c-e905-4dd7-a1e4-3b23773192b1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215627%3B1743219227&q-key-time=1743215627%3B1743219227&q-header-list=host&q-url-param-list=&q-signature=c702a370c7ed893b631569a3af55fd29e274ace4)
Fig.10 (a) I-V curve of normal P/NMOS VS. abnormal  P/NMOS.

![FIB(lowbeam current)  Detector  DeepNWELL  Psubstrate  abnormal implant region   Normal implant region  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/969bd927-7126-4aea-b426-3c56a5c3dce9/969bd927-7126-4aea-b426-3c56a5c3dce9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215627%3B1743219227&q-key-time=1743215627%3B1743219227&q-header-list=host&q-url-param-list=&q-signature=a0914edddf8891b347e3bd49b82d4c6683322105)
Fig10 (b) The schematics of contact level at low beam current illumination of  FIB.

When accelerating voltage of SEM was forced to 10kV, deeper  penetration electrons could reach abnormal Well region, the    interface of junction between abnormal PWELL and Deep  NWELL induced negative charges accumulation in PWELL  region, but normal NWELL and Deep NWELL discharged  negative charges, and the difference between abnormal and  normal WELL regions produced different secondary electrons  reflection that helped us to dig out the implant issue in Figure  11.

![SEM Higher kV(eg.10kV)  Detecto  DeepNWELL  Psubstrate  abnormal implant region   Normal implant region  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9158db3f-8c4e-4492-8ac5-1a7b151dbf30/9158db3f-8c4e-4492-8ac5-1a7b151dbf30.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215627%3B1743219227&q-key-time=1743215627%3B1743219227&q-header-list=host&q-url-param-list=&q-signature=b1b56a9d903133653614d12020b2e49f96b71e2b)
Fig.11The schematics of  contact  level at higher kV illumination of SEM.

Implant defects are difficult to quantify, but increasing  accelerating voltage of SEM to drive incident electrons into  deeper   abnormal   regions,   and   combines   this   with  characteristics of SRAM, we discovered a successful  methodology to dig out implant issues finally.

## 4. Conclusion  

Using VC phenomenon to locate defect location was  suggested according to a previous study   [1].   Here we enrich  the application of VC technology to deeper region of device

and find out the root cause of malfunction which caused by abnormal PWELL definition. We discussed the reason why this phenomenon occurred and proved the existence of implant  defects through series methodologies of FA. Implant defects  are not easy to discover in normal conditions, how to narrow  down the possible defect location quickly is always a challenge  for FA engineers, but we found this method to be successful in  identifying the root cause of failure, and finally prevented the  scrap risk of mass production.

## Acknowledgments  

The authors would like to thank the FA1 and MA team  members of Product Engineering Division for their assistance  in producing the FA results.

## References  

[1]    C.H Wang, et .al.” Ion Beam Imaging Methodology of Invisible Metal  Under Insulator Using High Energy Electron Beam Charging ” IEEE  proceedings of 33rd ISTFA, 2007. pp. 168-170.    [2]    Hung – Sung Lin, Wen Cheng Hsu ” Using a Combination of C-AFM  and SCM for Failure Analysis of SRAM Leakage    in CMOS Process  with the Addition of a DNW Module  ”IEEE  Proceedings of 16th  IPFA-2009,pp.37-40.

