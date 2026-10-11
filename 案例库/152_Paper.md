---
title: "152_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_80e4f99eaf25b93d7f88f101023c7e9a7295230462135641
file_size: 1175142
---

## The Solutions of Bit Line Failure Analysis: Low kV  E-Beam, EBAC and LVI    

Link Chang 1\* , Rick HC Wang 1 , Andy CH Chang 1 , Simon TC Wang 1 , and Yu Pang Chang 1 , C G Song 2   1  United Microelectronic Corporation, Ltd. No. 18, Nake  $2^{\mathrm{nd}}$   Rd., Tainan Science Park, Sinshih Dist. Tainan City , Taiwan, R.O.C  2  HeJian Technology (Suzhou) Co., LTD.  Phone: 886-6-5054888 Ext 11391, Fax: 886-6-5051217, Email:  link_chang@umc.com

Abstract-   As the analysis of SRAM Memory Built In Self Test  (MBIST), some failure modes such as single bit (SB) or dual bit  (DB) failure can be localized accurately. The inspection area of  SRAM SB/DB is around   $\scriptstyle\mathbf{1}\sim\mathbf{2u m}^{2}$  . Traditionally, we can use the  Focus Ion Beam (FIB) for cross section (X-S) checking as a much  quicker inspection. However, X-S FIB inspection is not suitable to  analyze some other failure modes such as bit line (BL) failure,  which has a larger inspection area, around  $\mathbf{200u m}^{2}$  . We usually use  the Scanning Electron Microscope (SEM) and I-Beam Voltage  Contrast (VC) methods to have a plane-view check along the failed  BL to find any abnormality. Sometimes a tiny defect is not easy to  observe by plane-view checking. In this paper, three alternative  methods, Low kV Electron Beam (E-Beam), Electron Beam  Absorbed Current (EBAC) and Laser Voltage Image (LVI) are  used in three real cases, and achieve a goal of higher hit rate and  shorter cycle time .

## I. Introduction  

In semiconductor manufacture, the product wafers are  tested by electrical test programs. Under conditions of low yield,  we execute the failure analysis to dig out the root cause. In  general, the SRAM can be a monitor vehicle for in-line process  yield improvement.

## II. Low kV E-Beam VC Method  

## (1)   Principle:   

Voltage Contrast (VC) is a well known method and has  been widely applied in the   semiconductor failure analysis field.   VC means brightness differences in FIB or SEM images of  structures having different electrical properties.

Fig.2 (a) shows the escape depth of secondary electrons,  back-scattered electrons and X-rays when the primary beam is  injected into a substance. Fig.2 (b) shows low kV E-Beam  image. Comparing the charging in FIB and SEM, FIB charging  is positive, whereas SEM charging can be positive or negative,  depending on primary beam energy [5]. We can utilize the  characteristics of SEM to change different beam energy to  perform VC. In the following case, low kV E-Beam VC was  applied.

For SRAM MBIST failure analysis, there are several fail  modes in the SRAM area, such as single bit, dual bit, four bit,  and bit line failure. With BL failure, which includes hundred  bits and peripheral circuit, it is more difficult to identify the  precise location compared with other failure modes. Fig.1  shows the inspection area of SB and bit line fail. In BL failure  cases, failure analysis takes a lot of time, because it is  necessary to check from the multi-metal layers down to the  Contact/Active Area for SRAM bit line pattern by I-Beam VC  and plane view SEM. In this paper, we will utilize Low kV  E-Beam VC, EBAC [1][2] and LVI [3][4] to analyze the BL  failures. By using these three methods, we successfully  localize the failure site and find the abnormality.

![Peripheral  circuit  Bitlinefail  Peripheral   SRAMArray  circuit  Singlebitfail  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ab5302dc-c866-4c95-b77c-82e03ea8cf96/ab5302dc-c866-4c95-b77c-82e03ea8cf96.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215637%3B1743219237&q-key-time=1743215637%3B1743219237&q-header-list=host&q-url-param-list=&q-signature=46cc6f580c7a3ea22031cb5e6df013de5d83e321)
Fig.1 The scheme of SB and BL fail inspection range in SRAM memory

![Can  (a)                                              (b)  IncidentElectrons   vcImage  Surface ofsample   Secondary Electrons  Back-scattered  x-rays   Electrons  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0f4fb6e9-b2fb-4511-baae-2dfcce7af634/0f4fb6e9-b2fb-4511-baae-2dfcce7af634.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215637%3B1743219237&q-key-time=1743215637%3B1743219237&q-header-list=host&q-url-param-list=&q-signature=4ee42d14355d25fac39bc0464775ac3896fe03ad)
Fig.2. (a) The escape electron depth (b) Low kV E-Beam image

## (2)   Case study:  

In this bit line failure case, at first we could not observe any  abnormality by I-beam detection. Then, by using low kV  E-Beam VC method, we found a bright BL Via1VC in the  SRAM structure. See in Fig.3.

![(a) cap                                              (b)  1-BeamVC   LowKVVC  BrightVia1(BL)VCwasfound  No obvious abnormality    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/182e9068-ba12-4432-8dfe-f967f63fba77/182e9068-ba12-4432-8dfe-f967f63fba77.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215637%3B1743219237&q-key-time=1743215637%3B1743219237&q-header-list=host&q-url-param-list=&q-signature=98763caaf83e54b45053683a8f3906c80af70462)
Fig.3 (a) I-Beam VC image, no solid abnormality; (b) Low kV E-Beam VC  image, bright BL VC was found.

In the above case, the E-Beam energy was varied from   $0.5\,\mathrm{kV}$   to  2kV. At the condition of  $0.5\mathrm{kV}$  , we can observe the noticeable  contrast. To double confirm the bright Via VC, we executed  C-AFM analysis and found the leakage path. The electrical  result is shown in the Fig 4 and Fig 5.

![AFM,Via1  AFM, Via1   +1V   -1V  IM  BL leak to P+  BL leak to  P+ ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/df94579c-4417-4fcd-8fe2-47799237a3b5/df94579c-4417-4fcd-8fe2-47799237a3b5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215637%3B1743219237&q-key-time=1743215637%3B1743219237&q-header-list=host&q-url-param-list=&q-signature=2b2ef76cc6189c139f1f0f059eb85401a74196fa)
Fig.4 C-AFM double confirms the bright Via1 VC, BL leak to  $\mathrm{P}+$   was found.

![I-V, Ref I-V, Ref  I-V,Bad I-V, Bad Ref Ref BL leak to P- BL leak to P+ ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2a629fad-3d3f-4cda-a96f-9733a405b2b5/2a629fad-3d3f-4cda-a96f-9733a405b2b5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215637%3B1743219237&q-key-time=1743215637%3B1743219237&q-header-list=host&q-url-param-list=&q-signature=12706b41d07b293cf0323c528af1e628c13345e8)
Fig.5 I-V measure of bright Via1

The PFA was performed by FIB  cross section, and a defect  was  found at CT bottom, shown as Fig.6. Ni element was detected by  EDS mapping, shown as Fig.7.

![X-S FIB image  T.S.1...T.T.  Defect was found  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c09d945e-acf4-4eba-aa57-0a284d64e792/c09d945e-acf4-4eba-aa57-0a284d64e792.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215637%3B1743219237&q-key-time=1743215637%3B1743219237&q-header-list=host&q-url-param-list=&q-signature=35c2207fff152bae1644694fe0e9380852730344)
Fig.6 defect at CT bottom was found by FIB cross-section.

![EDS  N  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e08661c6-8632-46af-a62d-2baac269e5d1/e08661c6-8632-46af-a62d-2baac269e5d1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215637%3B1743219237&q-key-time=1743215637%3B1743219237&q-header-list=host&q-url-param-list=&q-signature=883a3d8e16038200802a75ae76a55f5cfddd6a5c)
Fig.7 EDS mapping, Ni element was detected.

## III. Electron Beam Absorbed Current (EBAC) Method  (1)   Principle:   

EBAC [1][2] system is equipped with nano-probing and  SEM. The electron beam passes through the dielectric layers  allowing the lower level metallization layer to absorb the  electron beam current. The penetration depth of electron is  dependent on the acceleration voltage of SEM and sample  material.

The electron beam is an injection current source and the  current flow into metal/via structure was measured by the probe  shown in Fig8. If the metal/via chain is broken or open, the open  position can be localized by the change of EBAC contrast image  that is superimposed upon the SEM image. Some short or  leakage sites   also can be found by using two probes in EBAC  analysis. One probe is applied to the failure site which is  connected to the amplifier and the other is connected to ground.

![SEMdetector   E-Beam  Nano-probe  BAC  Superimpos  Image  ielectric  Metalline-   SEMdetectorSignal  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e449b3d8-18b2-48e4-acd3-7815ed3d654a/e449b3d8-18b2-48e4-acd3-7815ed3d654a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215637%3B1743219237&q-key-time=1743215637%3B1743219237&q-header-list=host&q-url-param-list=&q-signature=0871816525d24b76b16894ff15d000beb51c2195)
Fig.8 EBAC scheme

## (2)   Case Study:  

As an EBAC application for this BL fail case, two probes  were employed,  one on BL and the other on the N-Well as the  ground. Fig.9 and Fig10 schematically point out the probe  position and the leakage path of  the SRAM CT.

![EBACtip  Groun  Fig.9. EBAC method for bit line fails.  Fig.9. EBAC method for bit line fails.    N-Well  Leakagepath    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a36b17fd-b126-4cd3-a3a9-441ccbd3cf36/a36b17fd-b126-4cd3-a3a9-441ccbd3cf36.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215637%3B1743219237&q-key-time=1743215637%3B1743219237&q-header-list=host&q-url-param-list=&q-signature=57bd65e487e02e190b6405a120092cb7d75d881b)
Fig.10 The scheme of leakage path, from BL node leak to Vss through Fin  structure

Fig.11 is the EBAC detection result, which shows  abnormal EBAC signals at Vss. In this case the different  accelerating voltage dependence (5kV, 1kV) of detection was  also studied. In this study, abnormal Vss signal was observed  when the E-Beam energy was at 1kV, but at 5kV, there was no  abnormal signal, as all devices were turned on.

![IKV   5KV  BLsignal  11111111  SAS  AbnormalVsssignal  Noabnormalsignalat5ky  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bfa395d6-7e17-469d-a014-71118863951e/bfa395d6-7e17-469d-a014-71118863951e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215637%3B1743219237&q-key-time=1743215637%3B1743219237&q-header-list=host&q-url-param-list=&q-signature=cd0f3f95ed3a92f00e41604894d52f89dd14b1a1)
Fig.11 EBAC detection, (a)1kV, EBAC shows abnormal signals at Vss;  (b) 5kV, no abnormal signal.

Figure 12 shows the PFA result for bit line fail by EBAC  method. The X-S TEM investigation revealed a stack fault on  the fin structure.

![Oxide  Stack fault  Silicon substrate     ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7d067f6f-f852-4f70-862a-4490d53eb1b8/7d067f6f-f852-4f70-862a-4490d53eb1b8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215637%3B1743219237&q-key-time=1743215637%3B1743219237&q-header-list=host&q-url-param-list=&q-signature=87e62800d1234536543525aed2069d0cab3355dc)
Fig.12   Fin stack fault was found.

## IV. LVI Method  

## (1)   Principle:   

In traditional EFA analysis, it usually uses only 2\~4 pin  to apply DC power and it is useful to detect general DC  failure like short/leakage but not function failure like  MBIST. The new method, Dynamic-EFA, is different from  traditional EFA. It can combine tester and back-side analysis  tool, apply several power settings and signals by probe card   to simulate the real testing environment.

## (2)   LVI function:  

The LVI can be referred to as “frequency mapping”,  and it shows the indicated locations of transistors are  activated at a specific frequency. By mapping the frequency  of a region of interest (ROI), failure analysts can quickly  trace circuit functionality through suspected circuitry to  isolate defects with nanometer precision. Because of these  characteristics of LVI, it has been widely used for circuit  interconnection debugging.

(3)   Case study:

As an LVI application for this BL fail case, the input signal  was a repeating 11001100…   $(50\%$   duty cycle) clock loaded  serially into the BL circuit with a 1.25MHz clock frequency. By  setting the SRAM program, the 1.25MHz clock signal could  load into specific BLs  simultaneously from input pad .

After comparing the LVI results between bad BL and  good BL, it could find different LVI signals at BL decoder  area, shown as in Fig13.

![BadBL   GoodBL  SRAMCell   SRAMCell  Y-MUX   Y-MUX  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f4a17d4c-84b6-4612-9215-c2b6c33ffe61/f4a17d4c-84b6-4612-9215-c2b6c33ffe61.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215637%3B1743219237&q-key-time=1743215637%3B1743219237&q-header-list=host&q-url-param-list=&q-signature=9d8af83dbd3cd18a6496850efcdbaa2a9a3c604d)
Fig.13 LVI analysis Image (a) bad sample, abnormal signal (b) Ref sample

Combining LVI results and layout, it found the signal difference  was happened at the read path of BL decoder shown as Fig.14.

After analyzing and tracing the circuit interconnection of read  path by TEM inspection, Cu loss of via bottom was found,  shown as Fig.15.

![BadBL   GoodBL  Read Circuit  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d02f9eef-1596-4005-a688-e47752a4f334/d02f9eef-1596-4005-a688-e47752a4f334.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215637%3B1743219237&q-key-time=1743215637%3B1743219237&q-header-list=host&q-url-param-list=&q-signature=4b5d8fc14d80025c8261e461f1c75850f942b24f)
Fig.14   LVI analysis image superimpose layout, no signal in read path of BL  decoder.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5117bae2-f43f-4342-b659-7d74e541d291/5117bae2-f43f-4342-b659-7d74e541d291.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215637%3B1743219237&q-key-time=1743215637%3B1743219237&q-header-list=host&q-url-param-list=&q-signature=d6f23b8685569f96c1b45a047988a27ca41d58d1)
Fig.15 TEM, Via2 bottom Cu loss was found.

## V. Conclusion  

As the semiconductor technology continues to shrink,  defects have become more difficult to be detected by

conventional methods. Especially the inspection range was wide.  In this paper, three methods, low kV E-Beam, Electron Beam  Absorbed Current (EBAC) and Laser Voltage Image (LVI) were  presented to solve the bit line failure in SRAM analysis. By  using these methods the fail site was localized and abnormality  can be found. We also enhance failure analysis hit rate and  provide a direction to yield improvement.

## R EFERENCE 

[1] W.P.  Lin and H.J Hsu, “Physical Failure Analysis Cases by Electron Beam  Absorbed Current & Electron Beam Induced Current Detection on  Nano-Probing SEM System”,  $17^{\mathrm{th}}$   International Symposium on the Physical  and Failure Analysis on Integrated Circuit, Session 04.04, July 2010    [2] Link Chang, Kuo Yu Wang, Simon TC Wang, Yu Pang Chang, “The  Investigation of Active VC and EBAC Analysis Utilization on Test  Structure”, International Symposium on the Physical and Failure Analysis  on Integrated Circuit, Session P2-2, 2015    [3] Yin S Ng, Ted Lundquist, Dmitry Skvortsov, Joy Liao, Steven Kasapi,  Howard Marks, “Laser Voltage Imaging: A new Perspective of Laser  Voltage Probing”.   $36^{\mathrm{th}}$   International Symposium for Testing and Failure  Analysis, Session1, Nov. 2010.    [4]   Shih Yuan Liu , “ Laser Voltage Imaging and Probing, efficient techniques  for scan chain verification on Advanced Node”, International Symposium  on the Physical and Failure Analysis on Integrated Circuit, Session FA-2  A0304, 2017    [5] Rue. Rosenkranze,“Failure Localization with Active and Passive Voltage  Contrast in FIB and SEM,” Microelectronics Failure Analysis Desk  Reference Six Edition, pp. 269-278, 2011.

