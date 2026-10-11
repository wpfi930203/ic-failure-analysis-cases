---
title: "292_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_461751e64e10731e7f726709f710e40c7295230462135641
file_size: 982632
---

## Failure Analysis and Improvement of Superjunction  MOSFET under UIS Stress Condition  

Min Ren 1\*, Yining Ma 1, Shengrong Zhong 2, Wei Li 2, Songrong Wu 3, Zehong Li 1, Wei Gao 1, Bo Zhang 1  1  State Key Laboratory of Electronic Thin Films and Integrated Devices, University of Electronic Science and Technology of China,  Chengdu, Sichuan, 610054, China  2  Wuxi China Resources Huajing Microelectronics Co. LTD, Wuxi, Jiangsu, China  3  Key Laboratory of Magnetic Suspension Technology and Maglev Vehicle, Ministry of Education, Chengdu, Sichuan, China   \*  Fax: +86-28-83207790   Email: renmin  $\@$   uestc.edu.cn

Abstract-   Reliability has increasingly become an important  concern in Superjunction MOSFET (SJ-MOS) design. Failure  mechanism and improvement in the process of unclamped  inductive switching (UIS) are always the research focuses of  SJ-MOS reliability. This paper analyzes the failed SJ-MOS  devices in the UIS test, and then studies the influences of   drift-region design on the avalanche durations of SJ-MOS and  proposes the improvement suggestions.

Keywords  –  Superjunction, Reliability, UIS, avalanche

## I. I NTRODUCTION 

Power MOSFETs have widespread appilcations in various  power systems due to the excellent characteristics such as  simple driving circuit, low driving power dissipation and fast  switching rate. However, there is a “silicon limit” between the  specific on-resistance   $\mathrm{(R_{on,sp})}$   and the breakdown voltage (BV)  of Power MOSFET [1]. The SJ-MOS based on charge  compensation theory breaks the “silicon limit”, which can  withhold high voltage by the mutual depletion of P-pillar and  the N-pillar in its drift-region. Since BV of SJ-MOS depends  only on its drift-region thickness, regardless of the doping  concentration, the relationship of    $\mathrm{R_{on,sp}}\mathrm{\timesBV^{2.5}}$   for the  conventional Power MOSFET changes to   $\mathrm{R_{on,sp}}\mathrm{\timesBV^{1.32}}$   [2].

For power MOSFETs, UIS process has been regarded as an  extremely severe electrical condition because all of the  electrical energy stored in the unclamped inductor will be  discharged by the MOSFET when it changes from on-state to  off-state [3] – [5]. The maximum avalanche energy in single  pulse   $\mathrm{(E_{AS})}$   that the device can endure before failure in the UIS  test is usually used to assess the ruggedness of a MOSFET. As a  type of power MOSFETs, SJ-MOS is similarly required to have  not only good performances but also high reliability.

Recently, the UIS failure mechanism and improvement  methods of SJ-MOS have always been the research focuses.  Zhu et al.  analyzed the failure mechanisms of SJ-MOS devices  with different charge imbalance conditions   $(\mathrm{Q_{p}{<}Q_{n}}$   and   ${\mathrm{Q_{p}}{>}{\mathrm{Q_{n}}}}$  )  under UIS condition [6].  Ren et al.  proposed a novel SJ-MOS  structure with high avalanche duration [7].  J. Roig et al.  studied  the energy limits of high-voltage planar and super junction  power MOSFETs under UIS condition [8]. However, the  comprehensive and systematic studies on   the   effects   of  drift-region design of SJ-MOS on its UIS duration are  relatively lack.

In this paper, the failure cause of SJ-MOS in the UIS test is  analyzed, and the relations between drift-region parameters and  UIS capacity of SJ-MOS are thoroughly studied by simulation,  and then the improvement suggestions are provided.

## II.   E XPERIMENTS 

The equipment of UIS test is ITC 55100 made according to  MIL-STD-750 as shown in Fig.1 (a), and the device under test  (DUT) are 600V class SJ-MOS devices manufactured by  China  Resources Huajing Microelectronics . According to the test  circuit shown in Fig.1 (b), fix the inductor L to   $10\mathrm{mH}$  and  gradually extend the pulse time   $t_{g}$   to increase the energy stored  in the inductor until the device fails. It is obtained that the   $\mathrm{E_{AS}}$  per unit area is about   $30\mathrm{mJ/mm}^{2}$  .

Fig.2 shows a typical decapped device failed in the UIS test.  Most burnout points of the failed devices are randomly located  in active region, which means that the breakdown firstly occurs  in the active region. Therefore, the terminal region is well  designed and has high enough BV. In order to further improve   $\mathrm{E_{AS}}$  , this paper will focus on the active region, especially the  drift-region parameters of the cell.

![L=10mH  L=10mH  V WDS  DS DUT DUT  R RG   vdd=50V  V dd =50V G t  V G g a  (a)                                                            (b)  CDJ  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/addc64ec-fe67-463c-ad5c-80569c3ccc22/addc64ec-fe67-463c-ad5c-80569c3ccc22.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215689%3B1743219289&q-key-time=1743215689%3B1743219289&q-header-list=host&q-url-param-list=&q-signature=029ec5ddd932a7a04671f8c8332c9bfaa630a9ce)
Fig. 1 The UIS test equipment ITC 55100 (a) and test circuit  (b).

![GatePad  Gate Pad Burnoutpoint  Burnout point Active Region  Active Region Termination Region  Termination Region ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e2686811-e5ca-45ba-b340-9dbe2d6b3e22/e2686811-e5ca-45ba-b340-9dbe2d6b3e22.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215689%3B1743219289&q-key-time=1743215689%3B1743219289&q-header-list=host&q-url-param-list=&q-signature=4adf911d0abc5f38bcc13966666bf359462fee5c)
Fig. 2 A typical SJ-MOS device failed in the UIS test.

A 600V class SJ-MOS is designed and simulated by  Medici   to study the effects of drift-region parameters on BV and   $\mathrm{E_{AS}}$  .  The parameters used in the simulations are provided in Table 1,  in which the impurities in P-pillar and N-pillar (N-epi) satisfy  charge-balance principle. The mixed-mode device and circuit  joint simulation was adopted to predict avalanche duration of  the device: the designed SJ-MOS is invoked to the circuit  shown in Fig.1 (b) and a thermal resistance is added between its  drain electrode and the ambient; then its transient characteristic  is analyzed. The ambient temperature is set to 300K in the  simulations as thermal boundary condition. Fig.5 (a) provides a  typical I-V curve of the destroyed SJ-MOS in the UIS  simulation. The device failure can be predicated because its  drain current does not drop to zero when the drain voltage drops  to   $\mathrm{V_{dd}}$  ; at the moment the maximum lattice temperature has  exceeded the intrinsic excitation temperature of silicon, as  shown in Fig.5 (b). In this paper, the UIS capacity is  represented by the peak avalanche current  $(\mathrm{I}_{\mathrm{AS}})$  ） .

T ABLE  1   T HE MAIN DEVICE PARAMETERS USED IN THE SIMULATIONS

|Parameters|Values|
|---|---|
|Cell size|15μm|
|P-body concentration|3e16cm -3|
|P pillar width|5μm|
|P pillar concentration|2e15 cm -3|
|N pillar width|10μm|
|N epi resistivity|4.49Ω·cm|
|P- pillar thickness|34μm|


![0 JFET region  JFET region N+  R B  P-body  P-body 10  Parasitic BJT  Parasitic BJT Distance (μm) 20 P Pillar  N Pillar  N Pillar  P Pillar PPillar  （ (N-Epi)  N-Epi ） 30 40 N+substrate N+substrate  2  4  6  8  8  10  10  12  14 Distance (μm)  Distance (μm) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3f48d369-4341-4ef8-8eaa-afd7d94ee1e0/3f48d369-4341-4ef8-8eaa-afd7d94ee1e0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215689%3B1743219289&q-key-time=1743215689%3B1743219289&q-header-list=host&q-url-param-list=&q-signature=279b60c12fabfc5db7cf21b844ef1719f7d961de)
Fig. 3 The structure and parameters of the 600V-class SJ-MOS cell simulated  by  Medici .

![口..  3  02  uea   BV B\$  0L0  100  200300400500   6007D0  V（Drain) (Volis)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2a2ba214-4f5e-4e80-a5d7-bbc2b11e1ac8/2a2ba214-4f5e-4e80-a5d7-bbc2b11e1ac8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215689%3B1743219289&q-key-time=1743215689%3B1743219289&q-header-list=host&q-url-param-list=&q-signature=ca6bf1dfb9b8e15a9860a9cc75f459d91533d59f)
Fig. 4 The reverse I-V curve of the SJ-MOS and its electric field distribution at  the breakdown voltage.

![一  IAS.  1500   a (a)                                                            (b) CD ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d9381b52-c161-4607-a375-4b811198bf90/d9381b52-c161-4607-a375-4b811198bf90.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215689%3B1743219289&q-key-time=1743215689%3B1743219289&q-header-list=host&q-url-param-list=&q-signature=a846a5b49aa87b0ba507c2fed0aa96f5d274c5b7)
Fig. 5 (a) typical I-V curve of the SJ-MOS destroyed in the UIS simulation; (b)  lattice temperature distribution of the destroyed SJ-MOS at the moment that the  drain voltage drops to   $\mathrm{V_{dd}}$  .

The influences of main drift-region parameters on the UIS  capacity of SJ-MOS are discussed below.

## P-pillar Doping Concentration  

As shown in Fig.6, BV declines when the doping  concentration of P pillar is deviated from the balance doping  concentration （  $(\,2\mathrm{e}^{15}\mathrm{cm}^{3}\,)$  ） due to charge imbalance of P/N pillar.  However, I AS  increases monotonically as P-pillar doping  concentration increases. The reason can be explained that the  breakdown point and avalanche current path will shift with the  charge imbalance degree of P/N pillar. As shown in Fig.7, with  the increasing of P-pillar doping concentration, the location of  electric field peak moves from the junction between P-body and  N-epi to the junction between P-pillar bottom and N-epi.  Consequently, the breakdown point gradually moves to interior  of the cell, so that the avalanche currents passing through  P-body region under   $\mathrm{N}+$  source reduce, lowering the risk of  parasitic BJT triggering. Therefore, the avalanche duration of  the device is improved.

According to the above analysis, synthetically considering  about the electrical characteristics and reliability of SJ-MOS ， the most suitable doping concentrations of P pillar and N pillar  should be within a certain range of   $\mathrm{Q_{p}{>}Q_{n}}$   rather than at the  charge balance point （  $(\mathbf{Q_{\mathrm{p}}{=}Q_{\mathrm{n}}})$  ） .

## P pillar doping concentration distribution  

BV and   $\mathrm{{I_{AS}}}$   will be affected by the doping concentration  distribution of P pillar even though P pillar and N pillar satisfy  charge balance. Three doping distributions of P pillar are  simulated. Distribution A   $(\mathrm{D_{A}})$  : uniform doping   $({\bar{2}}\mathrm{e}^{15}\mathrm{cm}^{3})$  ;  Distribution B   $(\mathrm{{D}_{B})}$  : doping concentration increasing from top  to bottom; Distribution C    $(\mathrm{D}_{\mathrm{C}})$  : doping concentration  decreasing from top to bottom.

As shown in Fig.8, BV is lowered when P pillar has a  non-uniformly doping distribution in the vertical, while the  change of   $\mathrm{{I_{AS}}}$   is reversed. According to the electric field  distribution in Fig.9, non-uniform doping introduces new  electric field peak in the P pillar, which fixes the avalanche  breakdown point in the interior of P pillar and thus reduces the  avalanche current passing through the parastic resistor   $\mathrm{(R_{B})}$   in  the P-body region.

![2.31  2255  1.510   210   2.5519   3.0s10号  P pillar deping concentration(em\~3)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e6fc46a3-4961-4b83-b06d-5eec79c37e22/e6fc46a3-4961-4b83-b06d-5eec79c37e22.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215689%3B1743219289&q-key-time=1743215689%3B1743219289&q-header-list=host&q-url-param-list=&q-signature=66343db0f7433090dc532ef4bf1ec3441e3c4396)
Fig. 6 Variation of BV and  $\mathrm{I_{AS}}$    with P pillar doping concentration.

![ E-field distributions  E-field distributions   Current Flowlines  Current Flowlines 925  y ( μ 0   m) m) μ y (  x( μ m)  x(μ m)  x( μ m) (a)  312.5   y ( .5   μ m) MO.S  m) y ( μ  x( μ  2  11  m)  x（μm)  x( μ m) （D)  (b)  y ( μ m) y (  m) μ  μ m)  x( x(.μm)  x( μ m) (c)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d077ca17-9088-4d3c-bbd1-770291873eeb/d077ca17-9088-4d3c-bbd1-770291873eeb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215689%3B1743219289&q-key-time=1743215689%3B1743219289&q-header-list=host&q-url-param-list=&q-signature=62fa501b4a1a9ec323696fce4bb240e0b4b2020d)
Fig. 7 Electric field distribution and current flowline   at the breakdown voltage  with different P pillar doping concentrations. (a)   $1.4\mathrm{e}^{15}\mathrm{cm}^{3}$  ; (b)  $2\mathrm{e}^{15}\mathrm{cm}^{3}$  ; (c)   $2.9\mathrm{e}^{15}\mathrm{cm}^{3}$  .

![335040  11.4  660:  DA  D A  DB  D B  Dc  D C P pilar dopingc   entration distribution in vertieal  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e98b0881-86c3-4678-89d4-b836e0b52112/e98b0881-86c3-4678-89d4-b836e0b52112.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215689%3B1743219289&q-key-time=1743215689%3B1743219289&q-header-list=host&q-url-param-list=&q-signature=8ee4e45bded014e2dd8d3579dd43558a7151707d)
Fig. 8 Variation of BV and  $\mathrm{I_{AS}}$   with different P pillar doping concentration  distributions in vertical

![ E-field distributions E-field distributions  Current Flowlines Current Flowlinesy (μm)y ( m)μ μm) x(x(m) x(μm)(a)(a) y (μm)m)y ( μμm) x( x(μm)（Hm） (b)y (μm) (c)m)y (μ μm) x( x(（pm） μm)v （C) (c)](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e26a01c1-e8fe-4fe5-be4c-c48b3b651018/e26a01c1-e8fe-4fe5-be4c-c48b3b651018.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215689%3B1743219289&q-key-time=1743215689%3B1743219289&q-header-list=host&q-url-param-list=&q-signature=c40abf661b431ede5200cd37f46dfe2cbf3cbe46)
Fig. 9   Electric field distributions and current flowlines at the breakdown  voltage with different P pillar doping concentration distribution in vertical. (a)   $D_{A}$  ; (b)  $D_{B}$  ; (c)  $D_{C}$  .

## N-epi resistivity  

Fig.10 shows BV and   $\mathrm{{I_{AS}}}$   versus N-epi resistivity. It can be  found that BV gets maximum value when N-epi resistivity  satisfies charge balance of P/N pillar. However,   $\mathrm{{I_{AS}}}$   increases  when the N-epi resistivity drops. In fact, with the decrease of  N-epi resistivity,   $\mathrm{R}_{\mathrm{on}}$   of the SJ-MOS reduces, leading to the  decrease of power consumption and heat quantity; meanwhile,  the intrinsic temperature of N-epi rises. These two reasons  above facilitate the improvement of avalanche duration.

![228  02m  224  220  Epi resistivity(fxem)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/eb898d6f-3e0e-4488-bafc-b74b3874dbe7/eb898d6f-3e0e-4488-bafc-b74b3874dbe7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215689%3B1743219289&q-key-time=1743215689%3B1743219289&q-header-list=host&q-url-param-list=&q-signature=b7620cf932ef2b5466d5b712051982e7bb8ca88a)
Fig. 10 Variation of BV and  $\mathrm{{I_{AS}}}$   with N-epi resistivity.

Carrier Lifetime

Fig.11 indicates that the shorter the carrier lifetime, the better  the avalanche duration. The tendency can be explained as  follows, when the avalanche breakdown occurs during the UIS  process, a great number of electron-hole pairs are generated in  the depletion region. The electrons move toward the drain and  the holes move toward the source. These moving carriers break  the charge balance of P/N pillar, which reduces the breakdown  voltage and reliability of SJ-MOS. Short carrier lifetime  accelerates the recombination of electron-hole pairs and  avalanche multiplication effect is relieved accordingly.

Although BV hardly changes with carrier lifetime, short  carrier lifetime means more recombination centers, which  results in the increasing of reverse leakage current. So, even  UIS capacity can be enhanced by reducing carrier lifetime, the  problem of leakage current caused by too low carrier lifetime is  also detrimental to reliability of SJ-MOS.

![二 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/69f9827b-9e1a-4127-a8aa-dda092b08f21/69f9827b-9e1a-4127-a8aa-dda092b08f21.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215689%3B1743219289&q-key-time=1743215689%3B1743219289&q-header-list=host&q-url-param-list=&q-signature=d715d61661d47521e1fd9a2c3e5b6736d6ba30d7)
Fig. 11   Variation of BV and  $\mathrm{I}_{\mathrm{AS}}$   with carrier lifetime.

JFET doping concentration

Change the doping concentration of JFET region from   $\mathrm{Re}^{14}$   $\mathrm{cm}^{-3}$   to  $\mathsf{\breve{5}e^{15}\,c m^{-3}}$    to study its effect on BV and  $\mathrm{{I_{AS}}}$  . As shown in  Fig.12, BV slightly decreases with the increasing of JFET  doping concentration because high JFET doping concentration  results in higher electric field between P-body and JFET and  causes prematurely breakdown, as shown in Fig.13.

$\mathrm{{I_{AS}}}$   firstly increases with the JFET doping concentration until   $1.2\mathrm{e}^{15\mathrm{c}}\mathrm{m}^{3}$   and then decreases. The doping concentration of  JFET region will affect   $\mathrm{R_{on,sp}}$   and the electric field distribution  in the JFET region. When the JFET doping concentration  increases, on the one hand,   $\mathrm{R_{on,sp}}$    will decrease; on the other  hand, the electric field peak in JFET region will increases.  Therefore, there is an optimal JFET doping concentration by  the tradeoff between BV and I AS .

## IV. C ONCLUSION 

From the discussion above, except conventional methods  such as lowering the parasitic resistance in the P-body to avert  the turn-on of parasitic BJT, the drift-region parameters can be  carefully designed to improve the avalanche duration of  SJ-MOS. According to the experimental results, the   $\mathrm{E_{AS}}$   of the  optimized devices are promoted by about   $50\%$  .

![23.10  23105  23.00  s  22185  22150  22.75  1x102x103x104x105x10  JFET dose(cm)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/385092a9-1957-4a0c-b27a-5ce8d2ab7572/385092a9-1957-4a0c-b27a-5ce8d2ab7572.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215689%3B1743219289&q-key-time=1743215689%3B1743219289&q-header-list=host&q-url-param-list=&q-signature=8014ecb55e6782cc16bdceb92f13a91d6ae4ca3a)
Fig. 12   Variation of BV and  $\mathrm{I_{AS}}$   with   JFET doping concentration.

![y ( μ m)  x( μ m)  y ( μ m)  x( μ m)  y ( μ m)  x( μ m) (a)   （D)  (b)   （C）  (c)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4c454642-abff-4cd3-a316-75ec9f6513d8/4c454642-abff-4cd3-a316-75ec9f6513d8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215689%3B1743219289&q-key-time=1743215689%3B1743219289&q-header-list=host&q-url-param-list=&q-signature=48c18e987abea1128f9245f334a2e2771422688b)
Fig. 13 Electric field distribution at the breakdown voltage with differrent JFET  doping concentrations. (a)   $1\,\mathrm{e}^{14}\mathrm{cm}^{3}$  ; (b)   $1.2\mathrm{e}^{15}\mathrm{cm}^{-3}$  ; (c)   $5\mathrm{e}^{15}\mathrm{cm}^{3}$  .

## A CKNOWLEDGMENT 

This work was sponsored by Natural Science Foundation of  Guangdong Province (No. 2018A030313133)

## R EFERENCES 

[1]    T. Fujihira and Y. Miyasaka, "Simulated superior performances of  semiconductor   superjunction   devices,"  Proceedings   of   the   10th  International Symposium on Power Semiconductor Devices and ICs.,  pp.  423-426,   1998.    [2]    Xing-Bi Chen and J. K. O. Sin, "Optimization of the specific on-resistance  of the COOLMOS TM ,"  IEEE Transactions on Electron Devices , vol. 48,  pp. 344-348, Feb 2001.    [3]    K. Fischer and K. Shenai, "Dynamics of power MOSFET switching under  unclamped inductive loading conditions," in  IEEE Transactions on  Electron Devices , vol. 43, pp. 1007-1015, June 1996.    [4]    O. Alatise  et al ., "The Impact of Repetitive Unclamped Inductive  Switching on the Electrical Parameters of Low-Voltage Trench Power  nMOSFETs," in  IEEE Transactions on Electron Devices , vol. 57, pp.  1651-1658, July 2010.    [5]    J. Yedinak, D. Probst, G. Dolny, A. Challa and J. Andrews, "Optimizing  oxide charge balanced devices for Unclamped Inductive Switching  (UIS),"  22nd International Symposium on Power Semiconductor Devices  & IC's. , pp. 333-336, 2010.       [6]    J. Zhu, W. Sun, Y. Wu, S. Lu and Y. Yi, "Failure Analysis of  Superjunction VDMOS Under UIS Condition,"  IEEE Transactions on  Device and Materials Reliability , vol. 14, pp. 523-528, March 2014.    [7]    Ren Min, Li Ze-Hong, Deng Guang-Min, Zhang Ling-Xia, Zhang Meng,  Liu Xiao-Long, Xie Jia-Xiong, Zhang Bo, "A novel superjunction  MOSFET with improved ruggedness under unclamped inductive  switching,"  Chinese Physics B  21.4(2012):048502.    [8]    J. Roig, P. Moens, J. McDonald, P. Vanmeerbeek, F. Bauwens and M.  Tack, "Energy limits for unclamped inductive switching in high-voltage  planar and SuperJunction power MOSFETs,"   Proceedings of the 23rd  International Symposium on Power Semiconductor Devices and ICs. , pp.  312-315, 2011.

