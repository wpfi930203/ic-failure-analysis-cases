---
title: "294_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_c2796706d5aba51a59aa6860f52a3c6f7295230462135641
file_size: 729413
---

## Comparative Study of Total Ionizing Dose Effects on  the Silicon-Controlled Rectifier Devices for HV and  LV ESD Protections  

Zhuojun Chen 1,\* , Wenzhao  $\mathrm{{L}}\mathbf{u}^{1}$  , Ming Wu 1 , Wei Peng 1 , Yun Zeng 1 , and Xiangliang Jin 2  1 Department of School of Physics and Electronics, Hunan University, Changsha 410082, China  2 Department of School of Physics and Electronics, Hunan Normal University, Changsha 410081, China  \* Phone: +15901655895 Email: zjchen@hnu.edu.cn

Abstract-   In this paper, the total ionizing dose (TID) effects on low  voltage triggering silicon controlled rectifier (LVTSCR) and  LDMOS-SCR are studied for low voltage (LV) and high voltage  (HV) ESD protections, respectively. They are fabricated in a  5V/24V 0.5-μm CDMOS process and exposed to   ${}^{60}\mathbf{C}\mathbf{o}$   gamma rays  up to 200 krad(Si). The transmission line pulse (TLP) tests are  performed before and after irradiation, and then the ESD  performances are compared and discussed.

Keywords  –  Electrostatic discharge (ESD), Total ionizing dose  (TID), Low voltage (LV), High voltage (HV) .

## I. I NTRODUCTION 

With the development of aerospace technology, more and  more integrated circuits (ICs) are working in the radiation  environment. Therefore, the electrostatic discharge (ESD)  protection devices for ICs should guarantee to operate properly  after radiation exposure [1]. The semiconductor devices will  suffer from many effects including single-event effects (SEEs)  and total-ionizing dose (TID) effects [2].

The SEEs may cause abrupt change when radiation particles  such as heavy ions, alpha particles and neutrons strike into the  semiconductor materials. And the TID represents long-term  exposure to the radiation environment, resulting in the  accumulation of trapped charges in the dioxide layer and the   $\mathrm{Si-SiO}_{2}$   interface, which may lead to degradation of the device  performance or even direct failure [3-6]. Recently, Liang first  tested the performance of different commonly used ESD  protection devices under  $\mathrm{He+}$   irradiation, and the conventional  silicon controlled rectifier (SCR) showed quite sensitive to TID  effects and lost its typical functionality directly [7].

The ESD design windows are mainly determined by the  operating voltages and the breakdown voltage of the certain  process. Typically, the SCR becomes an excellent choice owing  to its strong current-tolerating capability per area. For low  voltage (LV) ESD protections, the low voltage triggering SCR  (LVTSCR) has been widely used. Besides, the SCR based on  laterally diffused metal oxide semiconductor (LDMOS) has  been commonly used for ESD protections of high voltage (HV)  circuits.

In this work, the impacts of TID effects on the LVTSCR and  LDMOS-SCR devices were investigated comprehensively,  which were designed for LV and HV ESD protections,

![restboa  gammer-ray  ource  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e87f7ad6-b060-46fc-a197-a8de47a8f70b/e87f7ad6-b060-46fc-a197-a8de47a8f70b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215690%3B1743219290&q-key-time=1743215690%3B1743219290&q-header-list=host&q-url-param-list=&q-signature=fc3fc78cc47236f372aaffa92f0d8187f7da11ef)
Fig. 1 TID Irradiation setup using a  $^{60}\mathrm{Co}$  gammar-ray source.

![Anode   Cathode  2+   P+  PVv  ND  P-sub  Anode   a   Cathode  P+   D+  PVVr  ND  P-sub  Anode   CD   Cathode  2+   P+   +  PVV  NND  P-sub  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fc03890c-d810-4cbc-9ef4-6acc48fd247a/fc03890c-d810-4cbc-9ef4-6acc48fd247a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215690%3B1743219290&q-key-time=1743215690%3B1743219290&q-header-list=host&q-url-param-list=&q-signature=92ae1e62ddb3f137b94a5569ca4e64b3923587d8)
Fig. 2 Cross sectional views of (a) the conventional SCR, (b) LVTSCR and (c)  LDMOS-SCR.

respectively. The transmission line pulse (TLP) tests were  conducted right after   $^{60}\mathrm{Co}$   gamma-ray irradiation. Finally, some  key ESD parameters including trigger voltage, holding voltage,  failure current and leakage current were compared and  discussed.

![a  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7d0b5347-34c7-42b1-a3ac-40dfebbc1438/7d0b5347-34c7-42b1-a3ac-40dfebbc1438.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215690%3B1743219290&q-key-time=1743215690%3B1743219290&q-header-list=host&q-url-param-list=&q-signature=32bac53f4f61e8f5a2e56c37baca2933e87ca19a)
Fig. 3 Photographs of fabricated devices of (a) LVTSCR and (b)  LDMOS-SCR.

![10-1310-1210-1110-10 10-9 10-8 10-7 10-° 10-5 10-4 10-3 10-² 10-1  Pre-Irradiation  50krad(Si)  100krad(Si)  )   -10  Voltage (V)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0d09476a-9950-46a4-84a1-02ce4f260dc0/0d09476a-9950-46a4-84a1-02ce4f260dc0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215690%3B1743219290&q-key-time=1743215690%3B1743219290&q-header-list=host&q-url-param-list=&q-signature=67980b45f858a8919baebe5830853eadd47b3c83)
Fig. 4 The pre- and post-irradiated TLP I-V curves of the LVTSCR.

## II.   E XPERIMENT  S ETUP 

The LVTSCR and LDMOS-SCR devices were fabricated in a  5V/24V   $0.5{\mathrm{-}}{\upmu\mathrm{m}}$   CDMOS process and assembled using the  COB technology. Fig. 3 shows the corresponding manufactured  device photographs. The   $^{60}\mathrm{Co}$   gamma-ray experiments were  carried out at a dose rate of 100 rad(Si/s) and irradiated up to  200 krad(Si), as shown in Fig. 1. During irradiation exposure,  the LVTSCR and LDMOS-SCR devices were biased at the  maximum supply voltages of   $5.5\mathrm{~V~}$   and   $26.4~\mathrm{V}$  , respectively.  The transmission line pulse (TLP) tests were performed before  irradiation and after each irradiation step of 50 krad(Si), 100  krad(Si) and 200 krad(Si).

## III. TID  EFFECTS ON THE  LVTSCR  DEVICES 

Figs. 2 (a) and (b) show the cross sectional views of the  conventional SCR and LVTSCR. The impact of TID effects on

![Leakage Current (A)@26.4V  10-1510-1410-1310-1210-1110-10 10-9 10-8 10-7 10-6 10-5 10-4 10-3  Pre-Irradiaton  50krad(Si)  100 krad(Si)  20   30   0   50  Voltage (V)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5641497f-fb65-4c3e-a03e-3bdda1f251ba/5641497f-fb65-4c3e-a03e-3bdda1f251ba.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215690%3B1743219290&q-key-time=1743215690%3B1743219290&q-header-list=host&q-url-param-list=&q-signature=9ed5f1e04a36a5fea28bbabc863e8164d6dc3e26)
Fig. 5 The pre- and post-irradiated TLP I-V curves of the LDMOS-SCR.

Table I – Key parameters of the LVTSCR under TID effects

|Device name|Total dose (krad(Si))|V t1 (V)|V h (V)|I h (A)|I t2 (A)|W (μm)|
|---|---|---|---|---|---|---|
|LVTSCR|0|13.56|2.88|0.32|3.65|50|
|LVTSCR|50|12.63|2.86|0.28|3.40|50|
|LVTSCR|100|13.57|2.78|0.25|3.45|50|
|LVTSCR|200|71.12|N/A|N/A|0.87|50|


the conventional SCR has been reported in Ref. [7]. It showed  that the leakage current increased with total dose, and it lost the  hysteresis characteristics of typical SCR after irradiation. Fig. 4  shows the measured pre- and post-irradiated TLP I-V curves of  the LVTSCR.

The leakage current of the LVTSCR when irradiation up to  100 krad(Si) is still maintained at a very low level. Compared  with the conventional SCR, the LVTSCR introduces a parasitic  gate-grounded NMOS (GGNMOS) in order to reduce the  trigger voltage. From Fig. 2(b), some of the field oxide is  replaced with a thin gate oxide layer and polysilicon along the  channel direction due to the existence of the parasitic NMOS. A  thin gate oxide generates less trapped charges when subjected  to the TID effects, making it relatively difficult to create a  leakage current path in the channel direction when the  LVTSCR has not been turned on.

Table I summarizes the key parameters of the LVTSCR  before and after irradiation. The trigger voltage decreases at  total dose of 50 krad(Si) and then rises as total dose increases.  Besides, the holding voltage, holding current and second  breakdown current are slightly degenerated. However, when  the total dose raises to 200 krad(Si), the trigger voltage of

![Anode  OCathode  +  Leakage path   TotalCurrentDensity(A\*cm^-2)  1.77e+03  3.96e-04  8.88e-11  1.99e-17  4.46e-24  1.00e-30  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e1876daf-38d8-4e24-8521-bf10e0ef357b/e1876daf-38d8-4e24-8521-bf10e0ef357b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215690%3B1743219290&q-key-time=1743215690%3B1743219290&q-header-list=host&q-url-param-list=&q-signature=64948533ea872639a640614ba6a382e891801987)
Fig. 6 Simulated total current density distribution of the LDMOS-SCR under  TID effects. (Oxide in the figure is hidden)

LVTSCR increases to 71.12 V and it immediately fails after  triggering.

IV. TID  EFFECTS ON THE  LDMOS-SCR  DEVICES

Fig. 2 (c) shows the cross sectional view of the LDMOS-SCR  device and the pre- and post-irradiated TLP I-V curves of the  LDMOS-SCR are depicted in Fig. 5. In order to protect high  voltage and power ICs, the SCR structure is embedded into  LDMOS to form the LDMOS-SCR, fwhich has excellent ESD  protection   performance   with   high   area   efficiency.  Unfortunately, when total dose increases to 100 krad(Si), the  leakage current of LDMOS-SCR has already increases up to   $10^{-7}$   A, which is not acceptable for IC applications in the  radiation environment. To find out its internal mechanism, the  total current density   $\left(\mathsf{A}/\mathsf{c m}^{2}\right)$   of the LDMOS-SCR, when  LDMOS-SCR has not been turned on, is shown in Fig. 6. It can  be seen that the main leakage current from anode to cathode is  sidewall leakage current, and the main sidewall leakage current  is between the thick gate oxide of the   LDMOS-SCR and   $\mathrm{N}+$    region at cathode. This is due to the thick gate oxide and the  sidewall oxide will produce positive traps under the TID effects,  in which the thick gate oxide will produce more positive traps in  oxide layer. Then the positive traps in oxide will attract  electronic at the   $\mathrm{Si-SiO_{2}}$   interface, which produce sidewall  parasitic transistors [8]. The parasitic transistors are composed  by N-Wells (NWs), sidewall silicon and  $\Nu+$   regions at cathode,  which produce a leakage path from anode to cathode. Moreover,  due to the existence of thick gate oxide and high operating  voltage, the LDMOS-SCR is more likely to produce a leakage  current path when subjected to the TID effects. Therefore, the  leakage current of the LDMOS-SCR increases with total dose  level.

Some key ESD parameters of the LDMOS-SCR are  summarized in Table II. The trigger voltage of the

Table II – Key parameters of the LDMOS-SCR under TID effects

|Device name|Total dose (krad(Si))|V t1 (V)|V h (V)|I h (A)|I t2 (A)|W (μm)|
|---|---|---|---|---|---|---|
|LDMOS-SCR|0|41.88|3.28|0.97|8.06|50|
|LDMOS-SCR|50|44.52|2.49|0.89|8.12|50|
|LDMOS-SCR|100|44.71|2.56|0.84|8.27|50|
|LDMOS-SCR|200|N/A|N/A|N/A|N/A|50|


LDMOS-SCR is increased, and the holding voltage is  decreased when suffered from TID effects. In addition, TID  effects with low total dose make negligible impacts on the  holding current and second breakdown current. However, when  total dose rises up to 200 krad(Si), the LDMOS-SCR is  complete failure, as shown in Table II.

## IV. C ONCLUSION 

In this work, the LVTSCR and LDMOS-SCR devices are  investigated under different total dose levels. When  accumulating total dose to 100 krad(Si), the LVTSCR shows  negligible change; however, the leakage current of the  LDMOS-SCR increases by more than three orders of  magnitude. And both of them fail to protect the circuits under  electrostatic discharge stress after irradiation up to 200 krad(Si).  It demonstrates that the LVTSCR features a 100 krad(Si) total  dose tolerance, which can still be used for LV ESD applications  for some low earth orbit missions. However, the LDMOS-SCR  is quite sensitive to TID effects and some hardness techniques  should be taken into consideration for HV space applications.

## A CKNOWLEDGMENT 

This work is supported in part by the National Natural  Science Foundation of China under Grant 61804053, Grant  61827812, and Grant 61705065, in part by the Fundamental  Research Funds for the Central Universities under Grant  2014YJS137, in part by the Natural Science Foundation of  Hunan Province under Grant 2019JJ50092, and in part by the  Technology Program of Changsha under Grant kq1703001.

## R EFERENCES 

[1]    R. K. Jain and L. H. Capots, "ESD Mitigation Method for Space Solar  Arrays," in  IEEE World Conference on Photovoltaic Energy Conference ,  Waikoloa, HI, USA, May 2006, pp. 1983-1985.    [2]    P. Pelissou, B. Daout, C. Romero, and K-F. J. Wolf, "Critical review of  the ECSS-E-ST-20-07C ESD test set-up for testing spacecraft  equipment," in  2016 ESA Workshop on Aerospace EMC  ( Aerospace  EMC) , Valencia, Spain, May 2016, pp. 1-4.    [3]    D. Linten, V. Vassilev, S. Thijs, G. Hellings, A. Griffoni, G.  Meneghesso, J. Wouters and G. Thys, "Anti-series GGNMOS ESD  clamp for space application IC's," in  Electrical Overstress/Electrostatic  Discharge Symposium (EOS/ESD) , Tucson, AZ, USA, Sept. 2014, pp.  1-7.    [4]    F. W. Sexton, "Destructive single-event effects in semiconductor  devices and ICs,"  IEEE Transactions on Nuclear Science ,   vol. 50, no. 3,  pp. 603-621, Jul. 2003.    [5]    H. J. Barnaby, "Total-Ionizing-Dose Effects in Modern CMOS  Technologies,"  IEEE Transactions on Nuclear Science ,   vol. 53, no. 6, pp.  3103-3121, Dec. 2006.    [6]    D. M. Fleetwood, "Total Ionizing Dose Effects in MOS and  Low-Dose-Rate-Sensitive Linear-Bipolar Devices,"  IEEE Transactions  on Nuclear Science ,   vol. 60, no. 3, pp. 1706-1730, Jun. 2013.    [7]    W. Liang, K. Alexandrou, M. Klebanov, C. Kuo, I. Kymissis, K. B.  Sundaram and J. J. Liou, "Characterization of ESD protection devices  under total ionizing dose irradiation," in  2017 IEEE 24th International  Symposium on the Physical and Failure Analysis of Integrated Circuits  (IPFA) , Chengdu, China, Jul. 2017, pp. 1-4.    [8]    M. McLain, H. J. Barnaby, K. E. Holbert, R. D. Schrimpf, H. Shah, A.  Amort, M. Baze and J. Wert, "   "Enhanced TID Susceptibility in Sub-100  nm Bulk CMOS I/O Transistors and Circuits,"  IEEE Transactions on  Nuclear Science ,   vol. 54, no. 6, pp. 2210-2217, Dec. 2007.

