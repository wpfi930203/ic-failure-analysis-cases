---
title: "225_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_96fd74c976bfc28de86d21bfeacb03b57295230462135641
file_size: 1270805
---

##  Research on SRAM Exhibiting Abnormal Behaviors  of Electrical Characteristics after Accelerated Stress in  Reliability  

Yi Heng Chen 1 , Chih Liang  $\mathrm{Lo}^{2}$   and Wu-Han Tseng 3  Yi-Ying Chen 4   Reliability Engineering Department, Powerchip Semiconductor Manufacturing Corp.   No. 18 Li-Hsin Rd. 1, Hsin Chu Science Park, Hsin Chu, Taiwan, R.O.C  Phone: 886-3-5795000 Ext: 3031   Fax: 886-3-5792142   Email:  peterch@powerchip.com

Abstract-   In the researches on embedded memories SRAM, we  found two components exhibited abnormal behaviors in electrical  characteristics with product electrical verification after product  reliability accelerated stress test. Relevant analyses revealed two  failure modes. One was gate oxide defect induced higher threshold  voltage of pull up devices (pMOS transistor) for writing mode  failure at  $\mathbf{-40^{\circ}C}$  of electrical verification; The other was both access  and pull down devices (nMOS transistors) with lower threshold  voltage caused read stability failure at   $\mathbf{88}\,^{\circ}\!\mathrm{C}$   of the electrical  verification. Both failures behaviors and physical mechanisms are  discussed in this paper.

Keywords  –  SRAM, pMOS, nMOS Transistors, nano-probe

## I. Introduction  

SRAM uses bi-stable latching circuitry made of  Transistors/MOSFETS to store each bit. Some study results  have shown that the conventional 6T SRAM suffered severe  stability degradation. The goal of this paper was investigations  in both abnormal behaviors in electrical characteristics and  physics mechanisms of failure modes for our company  embedded memory-CMOS 6T SRAM cell through relative  electrical verifications and failure analyses after HTOL 500hrs  stress.

## II.   Product Stress and Electrical Verification Results  

These two SRAM products through HTOL (High  temperature operation lifetime) stress with March C test pattern  using standard March C- algorithm (10N) was effective for  detecting the most of the classical memory faults. After 500hrs  accelerated stress, using electrical verification,   we found two  kinds of failure with a single bit failure mode from product A  and product B, respectively. According to product electrical  verification results revealed failure items were function failures.  Product A was a writing mode failure at   ${-40}^{\circ}\mathrm{C}$   and Product B  was a read stability failure at   $88\,^{\circ}\mathrm{C}$   of electrical verifications  based on our product requirements. From the two failures with a  severe variation of Vccmin degradation up to 1.08V were  observed  Fig.1  and  Fig.2 , respectively. Thus, we believed  extraordinary electrical characteristics of devices caused

functions and had a great impact on SRAM product under  V CC min state.

![BoxPlotDistributionsof16MSRAMVCCminat-40°CforWriteFailure  1..10  1.08   1.08  QTFailure  1,05  1.00   1.00  100  1.00  0.90   0.90  0.88   0.88   0.88   0.88  0.85  0.84   0.84   0.84   0.84   0.84  D8D  Pre-test (-40′C)   Pre-conA(-40C)   HTOL_HTS 168H(-40'C)HTOL_HTS 500H(-40°C)HTOL_HTS 1000H(-40°C)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b649d006-3be1-488b-afe6-f0e4dc9e505c/b649d006-3be1-488b-afe6-f0e4dc9e505c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215662%3B1743219262&q-key-time=1743215662%3B1743219262&q-header-list=host&q-url-param-list=&q-signature=3e330f20e5f87b0be30b6dcee8d7c43c3f93266c)
Figure 1 Product A VCCmin Degradation of Writing Mode Failure

![BoxPlotDistributionof16MSRAMVcCminat88CforReadDisturbFailure  Vmin(V)   1.08   QTFailure  1.08  104  1.O  100   1.00  10O  0.96  0.92  0.88  D84  Pre test_QT(85C)   Pre con_QT(85C)   168H_QT(85C)   500H_QT(85C)   1000H_QT(85C)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8eb0b138-63fd-4441-af21-e2ac426ef47d/8eb0b138-63fd-4441-af21-e2ac426ef47d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215662%3B1743219262&q-key-time=1743215662%3B1743219262&q-header-list=host&q-url-param-list=&q-signature=9544bba84a3c85f17f28a1f859472458ab5b916e)
Fig 2 Product B VCCmin Degradation of Disturbance Failure

## III. Analysis Results of Electrical Characteristics  

Two kinds of failures explorations were from product A and  product B, we further performed electrical characteristic  analyses using nano-probe detection. Product A, the data  writing mode failure at   ${-40}^{\circ}\mathrm{C}$  of electrical verification. The PUL  device (pull up pMOS transistor) of the abnormal cell had a  higher threshold voltage (up to -1V) than that of other normal  cells, the   $\mathrm{I_{DS}{-}V_{G S}}$   curve shown in  Fig.3 (a)

Product B was read stability failure   at   $88\,^{\circ}\mathrm{C}$   of electrical  verification. It revealed both PGR (access nMOS) and PDL  (pull down nMOS) transistors of the abnormal cell had a  weaker threshold voltage   (PGR Vth: 0.19V and PDL Vth:

0.15V) than that of other normal cells indicated in the  $\mathrm{I_{DS}{-}V_{G S}}$    curves shown in  Fig.3 (b)

![3（a)  PU_Vg-Id curve  VTPULshift  EUOEHOS  EUOELOX  1UOE  PGR  EOE-SN  E  PDL  BLX   B.  Fig.3 (a) Ips-Vgs Curve for Product A  Fig.3 (a)   Curve for Product A  3(b)  SelectBL  Un-SelectBL  -Vthshif    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ecf7dce3-a48a-4eff-b058-3056f9e71a0f/ecf7dce3-a48a-4eff-b058-3056f9e71a0f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215662%3B1743219262&q-key-time=1743215662%3B1743219262&q-header-list=host&q-url-param-list=&q-signature=9e7cfd4100ea5ef065634b30308e2af1b0238c49)
Fig.3 (b)  $\mathrm{I_{DS}{-}V_{G S}}$   Curves for Product B

## IV. Exploration of Failures and Mechanisms  

From previous descriptions, we are able to understand two  products with threshold voltage (Vth) shifts of cell devices.  Thus, we need to further explore mechanisms in threshold  voltage shifts of cell devices cause abnormal behaviors in the  electrical characteristics for these two products. First, compared  with gate dielectric of the normal PUL device, the gate  dielectric of abnormal PUL device with defect was observed  Fig.4  The gate dielectric of the PUL device with defect caused  higher threshold voltage inducing a weaker driving current   $\mathrm{(I_{D})}$  than that of other PUL devices. It means that the carrier  concentration was not enough to form channel conductivity for  PUL device at negative gate bias with dielectric defect   under  low temperature   $(-40\,^{\circ}\mathrm{C}$  ). The state induced poor channel  mobility of PUL device restrained write performance with  negative gate bias under low temperature   $(-40^{\circ}\mathrm{C})$  ).

![Failureaddress   Normaladdress  PUL  Abnormal  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c5d1b5d2-f450-47de-a315-2a9a85a2920e/c5d1b5d2-f450-47de-a315-2a9a85a2920e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215662%3B1743219262&q-key-time=1743215662%3B1743219262&q-header-list=host&q-url-param-list=&q-signature=ab09f9e02b600d04ab78359bb9fa944c48801a97)
Figure 4 Comparisons of Gate Dielectrics of PUL Devices for Product A

Consequently, in writing data mode, PUL device (pull up  pMOS transistor) of this memory cell can’t be turned on  causing data “1” can’t be written for storage node B under  “low” signal input. Data “0” can’t be written for storage node A  of the opposite invertor also under “high” signal input  Fig.5

![PUX   PXUR  PGR  PGL  PXL   XDR  Discharge  BLX  ·Node A is Lower voltage level through  discharge to BL  ·PUL device can't be turned on  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/239d572b-ba67-4445-aa1d-8656a4b23295/239d572b-ba67-4445-aa1d-8656a4b23295.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215662%3B1743219262&q-key-time=1743215662%3B1743219262&q-header-list=host&q-url-param-list=&q-signature=a2ef576b769edc24af7bb7c93e5f5bb7fb388bd9)
Figure 5 PUL Device Vth of Cell Circuits for Writing Mode

Second, another failure under   electrical verification was at   $88\,^{\circ}\mathrm{C}$  .  Fig.6  shows the PGR device of abnormal cell had weaker  channel than that of other cell for product B.

![PGR   Langth  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/01a9cee7-47a3-4f23-9f1b-4179fcfcf77b/01a9cee7-47a3-4f23-9f1b-4179fcfcf77b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215662%3B1743219262&q-key-time=1743215662%3B1743219262&q-header-list=host&q-url-param-list=&q-signature=52962de2597e931e7fe2f7e6931bcb39424cf495)
Figure 6 Weak Channel Length of PGR Device for Product B

This phenomenon crated larger leakage current. While read  data “0” state, BLB/BL will perform pre-charge to high voltage  level and the PGR and PGL two access transistors will turn on.  Meanwhile leakage current of PGR device moved to storage  node B due to bi-directional two access transistors when  devices were operating.  Fig.7 shows phenomenon means that  strengthened PGR device in electrical characteristic induced  voltage level of storage node B was raised to a higher level .

![TVo   Stronger  PG  P   PXR   IPD  PGE   Weaker  PGL   0V+a  PXL   PXR  BLB   BL  H  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/01f99681-7f7e-47d2-be28-a2016a28c9a2/01f99681-7f7e-47d2-be28-a2016a28c9a2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215662%3B1743219262&q-key-time=1743215662%3B1743219262&q-header-list=host&q-url-param-list=&q-signature=686a9f35d1c44c6b83060f02c72f9f20d49c403b)
Figure 7 Weaker Channel Length Strengthen PGR Device Current

From the circuit design of CMOS 6T SRAM, it indicated that  storage node B controls the input of inverter 1.Moreover, it  previously descripted that the PDL device was also weaker in  threshold voltage. Thus, this phenomenon turned on invertor1’s  PDL device (pull down transistor). This was caused by Node B  voltage level rising. Thus, the situation caused the access data  to be reversed   $(1{>}0)$   for storage node A [read action ->write  action], shown in  Fig.8

![Stronger  IPG  PXI  IPD  Weaker  BLB  Invertor 1   Invertor2  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8c85de4d-07e1-41f0-8e3b-ef288f0f1c51/8c85de4d-07e1-41f0-8e3b-ef288f0f1c51.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215662%3B1743219262&q-key-time=1743215662%3B1743219262&q-header-list=host&q-url-param-list=&q-signature=81e83b6a6d3347323db6d36f7d5b4ea0b92eadaa)
Figure 8 Access data to be reversed for Storage Node A

While storage node A access data was “0” (“L” voltage level)  that turned on PUR device of invertor 2 induced storage node B  rise to a “H” voltage level from VDD. It caused the access data  to be reversed   $(0\mathrm{~}->1)$  ) resulting in error for storage node B.  Fig.9  considered this a failure in read stability, a selected WL  and un-selected BL read disturbance failure.

![Stronger  PG  IPD  Weaker  PXR  BLB   BL  H   H  Invertor 1   Invertor 2  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/043b4674-f266-4d8c-89d3-9d69ee8cf5b2/043b4674-f266-4d8c-89d3-9d69ee8cf5b2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215662%3B1743219262&q-key-time=1743215662%3B1743219262&q-header-list=host&q-url-param-list=&q-signature=0e642d8b914825d283ce337c106183bfb8cb7745)
Figure 9 Access data to be reversed for Storage Node B

According to descriptions above, when the SRAM memory  accelerated stress with both a higher bias and a higher  temperature   $(125\mathrm{^\circC})$   conditions that exacerbated the threshold  voltage of cell transistors and made it grew weaker till devices  failed. Thus, SRAM memory occurred abnormally functional  behaviors at   $88~^{\circ}\mathrm{C}$   of the electrical verification finally.   Moreover, the PDL device (pull down nMOS transistor) of  invertor 1 suffered a lower threshold voltage issue. It came from  doping with its non-uniform distribution in a smaller area of  CMOS short channel devices   during wafer fabrication. This  was a random dopant fluctuation effect in our detail  investigations. Because random dopant fluctuation as the  source of intrinsic fluctuation. It has a great impact on variation  of number dopant atoms directly affect the threshold voltage of

MOSFET [1].Since threshold voltage depends on the charge of  the ionized dopants in the depletion region  Fig.10  The main  contribution was random dopant fluctuation effect, nMOS  exhibits a much larger threshold voltage (Vth) variation  compared to the pMOS ones. This is believed to be attributed to  the boron clustering effect in nMOSFETs [2-3] effects of  random dopant fluctuation in the influence of threshold voltage  variation have changed within process conditions and different  device structure. Therefore, the impact of threshold voltage  variation is a significant issue to IC chip makers.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a98553c7-1302-4846-bc93-c8a351c7dcb2/a98553c7-1302-4846-bc93-c8a351c7dcb2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215662%3B1743219262&q-key-time=1743215662%3B1743219262&q-header-list=host&q-url-param-list=&q-signature=3e68b523553364f15c6a18240a5abc8ca4155c2b)
Figure 10 Non-uniform Distribution of Doping with RDF Effect

## V. Results and Discussions  

Both product A and product B failures were exhibited at  500hrs of HTOL accelerated stress. Thus, it was important for  us to explore the degradation state of these two products. (a)  Vccmin degradation plot of product A revealed Vccmin state  was stable from initial step to the   $3^{\mathrm{rd}}$   step electrical verifications  (168hrs). Although product with defect of gate dielectrics, this  IC product still existence within 168hrs of accelerated stress.  Because the Vccmin was still kept 1V level is shown in  Fig. 11   However, continued accelerated stress IC product at 500hrs  degraded the PUL device (pMOS transistor) with defect in gate  dielectrics. The exacerbation stress raised threshold voltage of  pMOS transistor causing writing data mode failure under  Vccmin (1V). Consequently, it extended writing data mode  normally under Vccmin (1.08V) finally.

![BoxPlotDistributionsof16MSRAMVCCminat-40°CforWriteFailure  1_10  L08   08  QTFailure  105  1.00   1.00   100  1_0O  10.95  0.90  0_85  0.84   084  080  Pre-test ([-4O"C]  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4e70e493-b608-44d7-a070-ad50f96ea045/4e70e493-b608-44d7-a070-ad50f96ea045.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215662%3B1743219262&q-key-time=1743215662%3B1743219262&q-header-list=host&q-url-param-list=&q-signature=2472ae85b01618f70e4940714519c43d8a568b2c)
Figure 11 Vmin Degradation Plot of Product A

(b) Product B with read stability failure. Major reason was  cell devices with lower threshold voltage caused gradual  degradations to cell devices within 168hrs of accelerated stress.  Because the Vccmin was raised to 1.04V level  Fig. 12  The  accelerated stress exacerbated both PGR (access nMOS

transistor) and PDL devices (pull down nMOS transistor) by  168hrs to 500hrs. By reading data mode was failure under  Vccmin (1V). It extended to 1.08V we will get a normal read  data mode. It means that SRAM cell devices with reliability  concern couldn’t keep a normally functional operation within a  lower working voltage.

![BoxPlotDistributionof16MSRAMVCCminat88CforReadDisturbFailure  Vmin(v)   1.08   QTFailure  1,08  10q  1O  1.00   1.00  LOO  0.88  Pre:con   1000H  etest_QT(85C)   H_QT(850)   H_QT(85C)   QT(SS0  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bbe34176-0ad2-4d65-941f-c92b51dfc3c9/bbe34176-0ad2-4d65-941f-c92b51dfc3c9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215662%3B1743219262&q-key-time=1743215662%3B1743219262&q-header-list=host&q-url-param-list=&q-signature=779c2eefd4162cbfcd09841326afd03e4ca07144)
Figure 12 VCCmin Degradation Plot of Product B

The state of a cell will flip when word line is turned on during  read operation [4]. For this failure issue, because read failure  voltage (Vread) rose at storage node B was over trip voltage  (Vtrip) of the opposite invertor and reversed original data  Fig.13  The main reason of read voltage (Vread) increment was  a threshold voltage (Vth) mismatch of SRAM cell transistors. A  major contribution to the threshold voltage (Vth) was random  dopant fluctuation effect. Thus, for read stability requirement,  strengthen PD devices (pull down nMOS transistors) and  weaken PG devices (passing nMOS transistors)

![PG   MPG(W / L)PG   IPU   uPU(W/ L)PU  Vread   vtnip  IPD   μpD (W / L) pD   IPD   μpD (W / L) pD  Vread  PUL  PGR  PDR  ELL   BLX  Vtrip  Invertor1   Invertor2  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/18499988-cfe9-4229-ab9f-cac2348f8ed1/18499988-cfe9-4229-ab9f-cac2348f8ed1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215662%3B1743219262&q-key-time=1743215662%3B1743219262&q-header-list=host&q-url-param-list=&q-signature=dc0ead6dd5f49a43024fb9ea7b35998ade6ee4d5)
Figure 13 Degradation Behavior of Product B

The   threshold voltage (Vth) mismatch of SRAM cell  transistors was ameliorated with the  $2^{\mathrm{nd}}$   reliability qualification.  The threshold voltage improvement in cell devices with implant  parameter   adjustments   during   wafers   fabrication.   All  parameters of implant process were simulated under a certain  input combination, which comprises of a sequence many times.

## VI. Conclusion  

Reliability issue was solved with process ameliorations.  However, Vth variation of devices will greatly increase the  difficulty in the SRAM design field. Vth variation will cause a

narrow window of SRAM operation and poor noise margin  which will increase the signal error probability of the digital  circuit system.   Therefore, it is proven that an improved process  will provide sufficient process window to reduce the chance of  product failure in the market. And then problems won’t be  found in electrical detection within operation specifications.

## Acknowledgment  

This work was assisted in part by the department of product  failure analysis.

## References  

[1]  K. Takeuchi et al., Tech. Dig. IEDM, p. 841, 1997.  [2] T. Tsunomura et al.,  Symposium on VLSI Tech. , p.110, 2009  [3] E R. Hsieh and S. S. Chung et al., Symposium on VLSI Tech., p. 194, 2011  [4] J.J Chang.et al, “Fast and Accurate Estimation of Nan scaled SRAM Read  Failure Probability using Critical Sampling”, IEEE CICC, March 2005.

