---
title: "207_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_69cab4a0206b7d06db454c61bbc686157295230462135641
file_size: 896058
---

## Static Fault Isolation on Memory BIST Failure  

J.C. Alag, A.C.T. Quah, D. Nagalingam, P.T. Ng, Y.K. Teoh, Y.H. Chan   QA-EFA, Globalfoundries Singapore Pte. Ltd.  60 Woodlands Industrial Park D Street 2, Singapore 738406    Phone : (+65)83110599, Email :  jeromecuevas.alag@globalfoundries.com

Abstract —Conventionally, memory bitmapping is utilized to  identify the failing location in the Static Random Access  Memory (SRAM) array for physical failure analysis. However,  in a foundry environment, this capability may not always be  available for memory BIST failure debug. In our previous  publication, we have reported that photon emission microscopy  (PEM) can be utilized to localize subtle short and open defects  that have impacted the local or global wordline resulting in  detectable emission from the pass gate transistor [5].

In this paper, we extended this study and described three  case studies that illustrate additional SRAM failure modes that  could   potentially   produce   detectable   hotspot   using   a  combination of PEM and TIVA techniques for fault isolation.  This would serve as a good reference to better understand the  static fault isolation defect detection coverage on SRAM cell  functional failure.

## I.    I NTRODUCTION 

The increasing demand for low power and high-speed  embedded memory continues to drive the increase in SRAM  capacity in todays’ CPUs, GPUs and SOC for internet of  things applications. As a result, SRAM memory blocks  occupy substantial chip area and have the highest transistor  packing density with the most stringent design rule. This has  made SRAM blocks more vulnerable to manufacturing  defects and process variations from the lower backend-of-line  (BEOL) to frontend-of-line (FEOL) process steps. Thus,  failure analysis capabilities on SRAM failure are critical in  new product or technology node yield learnings and resolving  of low yield issue during volume production.

Memory bitmapping is the well-established industry  approach in isolating SRAM hard defects resulting in  functional memory BIST failure. With the descrambling of the  electrical failing bit/s addresses to physical failure cell/s  coordinates, physical failure analysis can follow suite for  single bit, pair bits, quad bits, partial column and row failures.  For more complex failure cells pattern, e.g., full or multiple  rows / columns failure, dynamic fault isolation techniques  such as LADA and SDL can be utilized [1],[2],[6] for further  isolation. However, such capabilities are not always enabled  in the foundry environment for debugging low yield issues.  This is especially evident for mature technology node devices  that lose software diagnostic capability due to shorter product  lifespan and cost reduction initiatives. IP confidentiality  concern also deterred the enablement of dynamic FI support.  Consequently, foundry has to fall back to static fault isolation  techniques, namely PEM[4] and TIVA[3], or even random  physical FA inspection to attempt to localize the defects.

It was commonly perceived that static fault isolation  techniques were ineffective in localizing defects in SRAM,  apart from isolating bigger defects that resulted in resistive  short between the memory VDD and VSS nodes, where the  latter should usually be binned out in the earlier power short/  leakage test instead of functional MBIST test. Fig. 1(a) and  1(b) show the schematic diagram and layout of a 6T SRAM

cell respectively with the electrical nodes labelled. CAREC  refers to a rectangular contact that connects the output of one  inverter to the input of the other cross coupled inverter in the  SRAM circuit. In our previous publication, we have shown  that subtle defects resulting in wordline (WL) opens or  wordline-bitline (WL-BL) shorts could produce detectable  photon emission from the partially turn-on pass gate (PG)  transistor for localization using static PEM [5]. The limitation  to this approach is that the minute PG leakage is usually not  distinguishable from static VDD vs VSS IV measurement or  observed from the wafer sort datalog. Thus, without any  means to cherry pick the best failure dies for fault isolation,  successful localization requires interrogating multiple failure  units to increase the probability of PEM hits. In this paper, we  supplement the previous work and showcase that apart from  the PEM successful localization on WL defectivities,  defectivities at the cell CAREC and VSS nodes, mapped out  in Fig. 1(a), may also be detectable with a combination of  PEM and TIVA techniques. Three case studies would be  described to illustrate how different failure modes on these  sensitive nodes were leveraged to achieve successful fault  isolation for low yield MBIST debug.

![WL VDD WLDefect PU1 CAREC PG1  PG2 Defect PD1  HHPD2 VSSDefect BL  Wss  BLB (a) a WM JSS1  一一 PD1  PU1  PG2 S2  NLM2 AAAA PG1 PU2  PD2 ISS2  (b) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0963e1a7-ddde-4db1-a12c-a2bbf7e84431/0963e1a7-ddde-4db1-a12c-a2bbf7e84431.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=4c32cbb8aed2976a1892d241a8824c2899886bd6)
Fig. 1(a) CMOS circuit diagram of a 6T SRAM and (b) layout of 6T  SRAM.

## II.   CASE   STUDIES  

## Case Study 1: WL-BL short and CAREC-CAREC short  

The first case study described a memory BIST low yield  issue on a 55nm device. Fig 2(a) illustrates the wafer sort map  of the impacted wafer showing the MBIST failing signature in  a seemingly rotating crescent pattern. Neither bitmap nor  dynamic capabilities were enabled on this device. Based on  the previous learnings of the possibility of static PEM  detection on WL defectivities, static fault isolation was  proceeded on 10 fail dies that were selected from the 2 higher  failure impacted regions circled in red. From the I-V curve  trace comparison between the good reference and bad units on  the VDD supply as shown in Fig. 2(b), 9/10 units were found  to be comparable with no abnormal leakages. Only 1 bad unit  observed   marginally   higher   IDD   current.   However,  subsequent PEM analysis was unable to localize any abnormal  hotspot from all the 10 fail units, including the marginally  leaky unit.

Subsequently, TIVA analysis was employed to further  investigate the single leaky unit, named as unit A. It was  delightful to observe that a TIVA hotspot (arrowed in red)  could be localized in the memory block as shown in Fig. 3(a).  Further TIVA analysis at higher magnification unveiled that  there were actually two distinctive hotspots, one in the  memory array and one at the decoder as illustrated in Fig. 3(b).  High magnification PEM was also performed, and a weak  emission spot could indeed be detected as illustrated in Fig.  3(c). It was, however, too weak to be identified from the  background emission during low magnification PEM analysis.

With this successful localization, TIVA was performed on  the remaining 9 units that had no observable IDD leakages. It  was interesting to observe that, out of the 9 units, 2 of them  could observe exclusive single TIVA spot in the memory  array. Fig 3(d) shows the high magnification TIVA overlay of  one of these two units, termed as unit B. However, no  emission could still be detected on unit B even at higher  magnification. The different hotspot signatures between unit  A and B could possibly indicate that a similar defect was  affecting different electrical nodes within their respective  failing SRAM cell.

Subsequently, progressive FIB was performed on unit A  at the TIVA/PEM spot location in the memory array. From the  FIB cuts as shown in Fig 4(a) and (b) a thin metallic residue  was observed, at the interface between metal 1 and contact  layer, causing WL-BL short. Fig 4(c) further illustrated the  layout perspective of the bridging nodes. The TIVA spot  location at the decoder was also inspected and no evidence of  anomalous residue was observed. This spot was likely induced  due to the WL-BL short. Layout analysis traces this spot  related to the multiplexer combinational circuit responsible for  the selection of BL for pre charging.

Unit B went through top-down physical failure analysis  approach instead and a similar residue could be observed from  high kV SEM inspection at metal 1 layer. However, in this  unit the bridging occurred between the two CARECs of the  cell, as shown in Fig 5. To better understand the static FI  detection sensitivity on resistively shorted CAREC-CAREC,  an SRAM cross-coupled inverter cell circuit model was  realized using Cadence. A simulation was conducted to  comprehend the cell   $I_{d d}$   current variation over varying short  resistance across 2 CARECs node. Fig. 6 illustrates the  simulation results displaying an intriguing leakage trend.

From this leakage trend, the PEM detection sensitivity can be  correlated to the leakage level while TIVA sensitivity is  closely related to the gradient which describes the current (or  power) change over the resistance change during thermal  stimulation. It is interesting to observe that from low ohmic  short to  $\sim100\mathrm{k}\Omega$  , only very marginal   $I_{d d}$   leakage current was  observed and it remained rather constant despite increasing  short resistance. At this region, static FI detection is likely not  possible due to the low leakage level and insensitivity of  current change with resistance changes.

However, as the resistance increases further from   $100\mathrm{k}\Omega$    to 1MΩ, boxed in red in Fig. 6, an abrupt change in the leakage  current was observed.  I dd  increases sharply, peaks at   $\sim8\mathrm{uA}$  ,  and decreases less rapidly with increasing resistance. The  large current change gradient would constitute to improve  TIVA sensitivity. A higher leakage level would also indicate  the possibility of weak photon emission. Therefore, it was  believed that the thin layer of conductive residue, in unit B,  had resulted in high ohmic short which was more easily  detectable with TIVA as compared to PEM (only observable  at higher magnification).

Beyond 1 MΩ, the  I dd  decayed to pA level as it behaves  towards a non-defective scenario. Fault isolation would not be  successful in this region due to extremely low leakage current.

From this case study, it is evident that laser induced  techniques could complement PEM and improve static FI  defect detection coverage on SRAM functional fail as it is  more effective in localizing defects causing WL-BL and  CAREC-CAREC shorts.

![1.0E-3   VDDvsVSS  -Bad1  Bad2  0.5  Bad3  1.0E-3   Bad4  Bads  -2.0E-3   Baae  -3.0E-3   Bad8  Bad9  4.0E-3   Bad10  -Ref1  --Ref2  -5.0E-3     Voltage(v)  (a)  Ca   Cb  (b)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3fd037a3-2365-461a-b479-4326648bfcba/3fd037a3-2365-461a-b479-4326648bfcba.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=675b907a190a55a7c32412881d0ab479af1b7335)
Fig. 2 (a) Wafermap with MBIST rotating crescent pattern and (b) VDD  vs VSS I-V comparison.

![Spotat  decoder  Suspected  defectlocation    (a)UnitA TIVAoverlay (low  (a) Unit A TIVA overlay (low   (b)Unit A TIVA overlay (high  (b) Unit A TIVA overlay (high  mag  mag)    mag  mag)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1d0c5bd8-3e33-4476-a9b4-95923dc90a2c/1d0c5bd8-3e33-4476-a9b4-95923dc90a2c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=c53c86666808e7129d9b65c1b85015becfaaf667)
![Suspected  defectlocatic       (c) Unit A PEM overlay (high  (c) Unit A PEM overlay (high   (d) Unit B TIVA overlay (high  (d) Unit B TIVA overlay (high  mag)   mag)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a9c30134-2c67-4583-9439-0e8879c15a22/a9c30134-2c67-4583-9439-0e8879c15a22.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=552976958d3f8795de4413f072ddfa780234f88d)
Fig. 3(a) Exclusive TIVA signal of Unit A at low mag, (b)High mag TIVA  signal of unit A, (c) PEM spot at high mag of unit A and (d) Exclusive  TIVA signal of unit B.

![  (a)AA”  (a) AA’   (b)BB"  (b)BB’  B.cut    CCJ  (c)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bb06a445-f2f7-4d7d-a1e7-13bd61dad6a2/bb06a445-f2f7-4d7d-a1e7-13bd61dad6a2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=9211d8c8ee31ed6562ee1f224831bfe602b37d6e)
Fig. 4(a) AA’ is the Initial FIB cut-particle short to BL (b)BB’ is the Final  FIB cut-particle short to WL (c) top-down visualization of defect from  layout perspective.

![  AREC  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ca4e5b18-c9dd-483e-8282-49a6a1c0a79d/ca4e5b18-c9dd-483e-8282-49a6a1c0a79d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=6e853fb66fbacc9733fb63b5e4d6f32d242b88f8)
Fig. 5 SEM M1 high beam inspection showing abnormal particle.

![High OhmicRegion  9.0E-06  B.0E-06  70E-06  LowOhmicres  .0E-06  VeryHighOhmicregior  0.0E+00  1E-011E+001E+011E+021E+031E+041E+051E+061E+071E+081E+091E+101E+11  Resistance(ohm)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ad7df347-922d-43d4-b717-97104eb4325e/ad7df347-922d-43d4-b717-97104eb4325e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=936ec35f5f13c3f6a18270514b5518598d8bb63e)
Fig. 6 Simulation result of leakage current against resistance.

## Case Study 2 : CAREC Open   

In this case study, Fab encountered a single wafer low  yield issue mostly contributed by BIST failures on a 55nm  product. Since only a single wafer experienced a random  pattern of BIST failures shown in Fig. 7(a) there was not  enough data of tool commonality that can be derived. It is  unfortunate that even e-tests do not present any evidence that  will steer the investigation to a certain failure. There was also  no indication of the best failing sample to work on since VDD  to VSS I-V comparison between the BIST failing dies and  reference dies showed no hint of leakages as shown in Fig.  7(b). For the purpose of solving the issue, even without  evident leakage difference, PEM and TIVA analysis were still  performed on more units. In one of the analyzed units, an  exclusive PEM spot with no corresponding TIVA signal was  observed. Fig. 8(a) and (b) shows the exclusive PEM spot at  the SRAM region indicated by the red arrow. This BIST unit  proceed for physical analysis to determine the failure and at  CA inspection, a shrunken and abnormally dark contrast  CAREC was observed at the spot location as shown in Fig.  9(a). Fig. 9(b) is the TEM image of the abnormal CAREC  showing portions of the CA is missing. The same defect was  subsequently also found on other samples which validated the  cause of the yield loss.

![/DDvsVSS    Ca  (a)   CD  (b)   ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e3a7a554-86ba-48bb-9c9c-d2b071d599d9/e3a7a554-86ba-48bb-9c9c-d2b071d599d9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=c2e0d01af3e88bd9521f52b9af4af39a58806e73)
Fig 7. (a) Wafermap showing gross random BIST failures and (b)VDD vs  VSS I-V curve comparison.

![(a) PEM overlay  (a) PEM overlay   (b)PEM overlay  (b) PEM overlay  (low mag)  (low mag)   (high mag)  (high mag)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/baf1cc89-9ca3-4cb8-8218-8dc257e82c10/baf1cc89-9ca3-4cb8-8218-8dc257e82c10.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=03a3dde2b3cfab60378a3471c72e0e3cbd2252c6)
Fig. 8 Exclusive PEM spot at SRAM in (a)low mag and (b) high mag.

![Missing Portion of CA  Ref  Shrunkeniand  darkPVC  TE    a  (a)   b  (b)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e82b0413-9ec1-4c10-9666-cf63747624db/e82b0413-9ec1-4c10-9666-cf63747624db.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=eeab751042f517823a611699aac2641ff84c2354)
Fig. 9(a) Shrunken CAREC and (b) TEM image showing missing portions  of CA.

This case demonstrates open CAREC resulting in unusual  PEM signal and no observed TIVA signal. Fig. 10 shows the  circuit diagram of a 6-transistor SRAM depicting the open  CAREC failure indicated by red dashed line and the blue line  corresponds to the net of the floating PU and PD gates. Open  failure at CAREC sets the PU and PD gates to a floating  condition which will set these gates on an arbitrary voltage  that can saturate the transistors and in turn produces the  emission.

![WWL VDD PG1  PG2 OpenCAREC Floating gates PD1  BD2 IBL  rss  BLBI ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fcb1840c-0ba4-456b-b99b-40f6f84ddb24/fcb1840c-0ba4-456b-b99b-40f6f84ddb24.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=84085a3d5d5dfe9e205ed9cb86555ff0b7564eea)
Fig. 10 6T SRAM illustrated in a CMOS circuit with open CAREC and  floating PU and PD gates.

## Case study 3: VSS open/resistive  

In this case study, Fab ran into a low yield issue on a  $55\mathrm{nm}$    product with gross wafer edge failure mostly contributed by  MBIST (blue color) and scan failure (orange color) as  illustrated in wafer sort map shown in Fig. 11(a). Initial

investigation identified the suspected impacted layer was at  Metal 2.  I-V comparison was performed, and no significant  leakage difference was observed between BIST failing dies  and good reference dies as presented in Fig. 11(b). PEM and  TIVA analysis was then carried out. At low magnification,  PEM shows a localized spot while TIVA analysis was carried  out only using higher magnification. Both fault isolation  techniques were able to detect localized spots at the SRAM  region. Although both can localize the spot, it was notable that  TIVA signal was weak and not easily detectable. Fig. 12(a)  shows the PEM exclusive spot while Fig. 12 (b) shows TIVA  exclusive spot.

During the physical analysis, abnormally dark PVC was  observed on a V2 VSS node shown in Fig. 13(a). The dark via  PVC is a strong indication of a highly resistive or open failure.  Fig. 13(b) further illustrates M2 void which more to a resistive  failure rather than fully open. A schematic diagram of 6T  SRAM with resistive/open VSS is illustrated in Fig. 14. These  findings correlate with the initial investigation result relating  to M2 deposition. On a resistive/open VSS node, there is a  potential difference between the source of PD2 (Vs) and the  global VSS. This potential difference will put Vds of PD2  transistor to an undetermined state and will directly influence  the gates inputs of PU1 and PD1 transistors. It is believed that  the emission is generated from the undetermined state of PU1  and PD1 gates. It is however suspected that the TIVA signal  was generated due to the resistive nature of the defect.

![VDDvsVSS     Voltage(v)  aD  (a)   b  (b)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d43102f7-d5ee-4233-b97a-c12b2227c903/d43102f7-d5ee-4233-b97a-c12b2227c903.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=95e8d8c216140199e37bbb996c0fe79aa220b5a6)
Fig. 11(a) Wafer sort map with MBIST edge failure pattern and (b) VDD  vs VSS I-V curve comparison between bad and reference dies.

![(a)   (b)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f74bdfae-3456-4d26-935b-6f312e0f6337/f74bdfae-3456-4d26-935b-6f312e0f6337.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=225da216f083365c2a87297a6fb1752d1d49db8b)
Fig. 12(a) PEM exclusive spots and (b) TIVA exclusive spots.

![v2  M2VOi    (a)   (b)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8b471a65-4b00-4d7a-ae74-4d8f9b359c76/8b471a65-4b00-4d7a-ae74-4d8f9b359c76.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=f1ce197dbf7f0e414ba0ea9e174535bb42bc85c2)
Fig. 13 (a) Abnormal dark V2 PVC and (b) TEM image showing M2 void.

![WWL VDD PG1  PG2 一  wdl  vds PD1  PD2 us Resistive Wss BL  Vss  BLBI ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8ee2d7ca-2472-4c28-ab9a-b781deaab2ae/8ee2d7ca-2472-4c28-ab9a-b781deaab2ae.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=287b180258e60ce03bc4591534fc575b6a500358)
Fig.14 6T SRAM illustrated in a CMOS circuit with resistive/open VSS.

## III.   CONCLUSION  

We have discussed three case studies demonstrating  additional sensitive SRAM failure modes which could be  leveraged to achieve successful static fault isolation for  memory BIST low yield debug. TABLE I. was compiled to  summarize the detection sensitivity of fault isolation  techniques on these SRAM failure modes. This information  would be useful for debugging SRAM failures even without  bitmap or dynamic analysis capabilities.

TABLE I.     S UMMARY OF  S TATIC  F AULT ISOLATION COVERAGE ON  SRAM   F AILURE MODES

|Failure modes|Failure modes|PEM hotspot|TIVA hotspot|
|---|---|---|---|
|1|WL Open|Detectable [5]|Not observed[5]|
|1|WL-BL short|Detectable [5]|Detectable *|
|2|CAREC- CAREC short|Not observed|Detectable|
|2|CAREC open|Detectable|Not observed|
|3|VSS resistive open|Detectable|Not easily detectable|


\*Induced hotspot in decoder could be detected

## A CKNOWLEDGMENT   

The authors would like to thank the Failure Analysis and  Physical Analysis teams for the analysis data and their  engagement in the discussion of failure mechanism.

## R EFERENCES   

[1]    Zhigang Song,”SRAM failure analysis evolution driven by technology  scaling”, Proc. Intl Symp. Physical & Failure Analysis of Integrated  Circuits (IPFA), pp.223-230, 2014.    [2]    Moon Seung Je et al, “Application of Soft Defect Localization  Technique for SRAM Soft Fail Debug”, Proc. Intl. Symp. For Testing  and Failure Analysis (ISTFA), pp.316-320, 2014    [3]    J.C.H. Phang et al, “A Review of Laser Induced Techniques for  Microelectronic Failure Analysis“, Proc. Intl. Symp. Physical &  Failure Analysis of Integrated Circuits (IPFA), pp.255-26, 2004    [4]    J.C.H. Phang et al, “A Review of Near Infrared Photon Emission  Microscopy and Spectroscopy“, Proc. Intl. Symp. Physical & Failure  Analysis of Integrated Circuits (IPFA), pp.275-281, 2005    [5]    N. Dayanand et al., "Static fault localization on Memory failures using  Photon Emission Microscopy," 2015 IEEE 22nd International  Symposium on the Physical and Failure Analysis of Integrated Circuits  (IPFA), pp. 322-326, 2015    [6]    BL Yeoh et al., " Debugging MBIST hard fails without bitmapping,"  2015 IEEE 22nd International Symposium on the Physical and Failure  Analysis of Integrated Circuits (IPFA), pp. 138-143, 2015

