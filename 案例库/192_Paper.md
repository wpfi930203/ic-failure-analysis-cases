---
title: "192_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_3f26bda0155f02537aeaadb1379ff2ba7295230462135641
file_size: 1226722
---

## A new study of backend process on 0.18um BCD NLDMOS  on-state BV characteristics  

Shuxian Chen, Feng Lin\*, Bin Yang, Chunxu Li, Yu Huang  Technology Development Division, CSMC Technologies Corporation, Xinzhou Road,Wuxi, China  \*Phone: 86-510-88113682 Fax: 86-510-88115555-3682 Email: linfeng@csmc.crmicro.com

Abstract- With the continuous expansion of power ICs in various  industrial   and   consumer   levels,   the   requirements   for  Laterally-Double-Diffused MOS(LDMOS) characteristics are  getting more and more aggressive. BVon characteristics of  LDMOS is rather critical for wide Safe Operation Area (SOA),  requesting in higher-end fields such as automotive electronics. In  this paper, based on the modular design of the   ${\bf0.18\mu m}$  Bipolar-CMOS-DMOS (BCD) medium and high voltage process  platform, the process platform should not only consider the  impact of the introduction of high-voltage process on CMOS, but  also the impact of the special Back- End-Oxide-Layer(BEOL)  process customized for embeds Non-Volatile Memory (E-NVM)  on high-voltage devices. For the problem of insufficient on-state  breakdown voltage (BVon) and poor on-chip uniformity of  NLDMOS, we studied the influence mechanism about BEOL  process on NLDMOS BVon characteristic.

Keywords:  –  RESURF ， surface electric field ， SAB thickness ， CESL material  ， ILD thickness .

designed as a surface-dense type device with floating poly and  metal field plates to enhance surface depletion, reduce surface  electric field, and increase breakdown voltage. The  schematic structure of NLDMOS is shown as Figure 1.

![Gate  N+  P-e   N-weH  P-body  N-drift  BN  Psub  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f3e159e4-4379-4081-a9e1-813369a7fa83/f3e159e4-4379-4081-a9e1-813369a7fa83.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215648%3B1743219248&q-key-time=1743215648%3B1743219248&q-header-list=host&q-url-param-list=&q-signature=50cca5e004b0246123b3d43bc53105d6520d84d8)
III. R ESULTS AND DISCUSSION

## I. I NTRODUCTION 

With the continuous expansion of power ICs in various  industrial and consumer levels, the requirements for Laterally  Diffused   Metal   Oxide   Semiconductor   (LDMOS)  characteristics are getting more and more aggressive [1-3].  Regardless of the application area, it is hoped that the ratio of  LDMOS to the chip area is as small as possible, so the attention  of resistivity of drain to source at on-state (Rdson) and off-state  breakdown voltage (BVoff) has been very high. However, the  on-state breakdown voltage (BVon) characteristics of LDMOS  is very critical for wide safe operation area (SOA), requesting  in higher-end fields such as automotive electronics. But so far,  few articles have reported about it [4] – [7].

## II.   E XPERIMENTS 

The research in this paper is based on the modular design of  the   $0.18\upmu\mathrm{{m}}$    BCD medium and high voltage process platform,  which is compatible with logic processes and embeds  Non-Volatile Memory (E-NVM) devices. Therefore, the  process platform should not only consider the impact of the  introduction of high-voltage process on CMOS, but also the  impact of the special Back-End-Oxide-Layer (BEOL) process  customized for E-NVM on high-voltage devices. For the  problem of insufficient BVon and poor on-chip uniformity of  NLDMOS, we studied the influence mechanism about BEOL  process as Inter-Layer-Dielectric (ILD) thickness, Salicide  –Area-Block (SAB) thickness and Contact-Etch-Stop-Layer  (CESL) type on NLDMOS BVon characteristic.

To achieve the minimum resistivity of drain to source at  on-state (Rdson), the NLDMOS in the 0.18um BCD is

![NLDMOSBVoff/BVonV.S.Rulem  SiliconBVoff  100   100  SiliconBVon  SimulationBVoff  SimulationBVon  8  1-6   2.6   3.6   12  Rulem  a  (a)   NLDMOSBVoff/BVonV.S.Rulen  100   100  SiliconBVoff  SimulationBVoff  SiliconBVon  Simulation BVon  Rule n  (b)   ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e1ccf525-6aa4-42ff-b712-4cd66d7e84d3/e1ccf525-6aa4-42ff-b712-4cd66d7e84d3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215648%3B1743219248&q-key-time=1743215648%3B1743219248&q-header-list=host&q-url-param-list=&q-signature=e079f230bd339659a5e1c036dba863eb0cbb7632)
Fig. 2 (a) The silicon data and TCAD simulation data of 60V NLDMOS   BVoff V.S. rule m and n (b).The silicon data and TCAD simulation data of  60V NLDMOS BVoff V.S. rule m and n.

It is planned to adjust the BVoff  and BVon of the NLDMOS

simultaneously by changing the number of floating poly (rule n)  and the length of the metal field of the drain end (rule m).   Actually, we found that the BVoff of NLDMOS is up to  standard, but the BVon is low, and the trend of  BVon changing  with rule m and n is not consistent with the simulation. Figure 2  shows the measured data of 60V NLDMOS BVoff/BVon and  Technology-Computer-Aided-Design (TCAD) simulation data  with rule m and n. Rule   $\scriptstyle{\mathrm{m}}=3.6{\mathrm{um}}$   and rule   $\mathord{\mathfrak{n}}\!\!=\!\!5$   is chosed as  center size.

The TCAD simulation shows large electric field and serious  impact ionization at the drain side of on-state (Fig. 3). The rule  n and m has been determined by BVoff, so we try to improve  the drain side electric field from the process. Take the 60V  NLDMOS as an example:

![PB  (a)  (b)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b7e9a536-cd0a-40c3-ab33-e86793f46dbf/b7e9a536-cd0a-40c3-ab33-e86793f46dbf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215648%3B1743219248&q-key-time=1743215648%3B1743219248&q-header-list=host&q-url-param-list=&q-signature=d09b6ef59c8d078a853734e3f692403527a1d4fe)
Fig.3 (a) The electric field of 60V LDNMOS at on state; (b) The impact  ionization of 60V LDNMOS at on state.

From Fig.4(a),we can see that when the total thickness of  ILD changes from   $5500\mathrm{\AA}$   to 7500Å, NLDMOS BVon shifts  significantly from 52.5V to 75V. ILD Thickened 2000A, BVon  can increase 20V and the uniformity is obviously better. The  increase of ILD thickness can reduce the depletion of metal  field plate to the NLDMOS surface, so that the depletion layer  will not grow up too closely to the drain side, the electric field  at drain side is weakened due to the Kirk effect is subdued.

The TCAD simulation is consistent with the real situation,  and the improvement effect of the ILD thickening on the drain  end impact ionization and electric field strength can be clearly  seen in Fig.4(b) and Fig.4(c).

Replacing   Contact-Etch-Stop-Layer   (CESL)   from  SION350A (CESL1) to PEOX200A+UVSIN600A (CESL2)  will reduce the device's BVon and limit it to 55V. While  switching to SION150A +UVSIN300A (CESL3), BVon can be  boosted about 5V. The output characteristic curves of 60V  NLDMOS with different CESL are shown as Fig.5. It is  speculated that  Ultraviolet-  $\mathrm{Si}_{3}\mathrm{N}_{4}$  ( UVSIN) captures some  electrons in CESL3, resulting in a decrease in the number of

effective electrons on the silicon surface and a reduction in the  surface electric field. However, as the UVSIN is thickened in  CESL2, the electrons are trapped too much. It causes a change  of the gate potential, which is equivalent to adding a negative  bias voltage on the gate. Thereby, it increases the drain to gate  voltage difference and  strengthens the Drain side electric field.  As a result, the BVon is stepped down.

![DifferentILDThicknessesAffecteBV  BVoff  Bvo  BVon  ILDS500   ILD6500   ILD7500  a  (a)  60VNLDMOSElectricFieldatOn-State  driftare:  ILD5500  DS   ILD6500  ILD7500  dummaypoly    (b)      (c)  CCD  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/391eff9f-e168-45ef-8dcf-47bddf978e49/391eff9f-e168-45ef-8dcf-47bddf978e49.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215648%3B1743219248&q-key-time=1743215648%3B1743219248&q-header-list=host&q-url-param-list=&q-signature=4ef8d39b5baee048e1ff20a1499100a4b3f05baa)
Fig.4: (a) BVoff and BVon of 60V NLDMOS with different ILD thickness; (b)  The electric field of 60V NLDMOS at on state with different ILD thickness; (c)  The impact ionization of 60V NLDMOS at on state with different ILD  thickness.

As the SAB thickness is reduced from  $2000\,\mathrm{\AA}$   to   $1500\,\mathrm{\AA}$  , and  the BVon of the device increased nearly 8 V. When SAB  thinned to 1200 A, the BVon continues to increase 4 V  ，  as  shown in Fig.6.  Under the premise that the thickness of the ILD  to silicon is constant, the thinner the thickness of the SAB, the  less susceptible the CESL layer is damaged by the CMP  process [8]. On the other hand, for the UVSIN in CESL layer is  charged, the metal field plate RESURF should really use the  oxide which is medium between AL1 and CESL. When CESL  is thinned, the effective oxide thickness is thickened, the metal  RESURF is weakened, the same mechanism with the total ILD  thickness variation. But the changeless of SAB thickness is  only a few hundred angstroms, the variation of BVon is not so  obvious as the thickness of the ILD.

![DifferentCESLsAffecteBV  BVoff  Byoff  BVon  1B+  SION350   SION150   PEOX200  +UVSIN300   +UVSIN600     a  (a)  Id-Vd Curve of Different CESL  SION350  PEOX200+UVSIN600  Vg=5V  Vg=5V SION150+UVSIN300  \$20  20   30  vds/y     Cb  (b)  ElectricFields ofDifferentCESLs at On-State  4.0x10  SION350  3.5x10   PEOX200+UVSIN600   driftarea  SION150+UVSIN300  3.0x10  2.5x10  sou    (c)  （C  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/976f48e9-3bed-4a6f-a70f-3933266a7b43/976f48e9-3bed-4a6f-a70f-3933266a7b43.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215648%3B1743219248&q-key-time=1743215648%3B1743219248&q-header-list=host&q-url-param-list=&q-signature=6291aa5c86ede827d2eee99f59ad53a0b94aed59)
Fig.5: (a) BVoff and BVon of 60V NLDMOS with different CESL; (b) The  output characteristic curves of 60V LDNMOS with different CESL; (c) The  electric field of 60V LDNMOS at on state with different CESL.

![Different SABThicknesses AffecteBV  Byoff  BVoff  BVon  ByoI  SAB2000   SAB1500   SAB1200  a  (a)  Electric Fields of Different SAB Thicknesses at On-State  4.0x10\~  SAB1200  3.5x10   drift area near drain  SAB1S00  SAB2000  3.0x10  2.5x10  pi!  2.0    b  (b)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b54d0b11-73e1-4f89-89aa-71ae32f1b9ce/b54d0b11-73e1-4f89-89aa-71ae32f1b9ce.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215648%3B1743219248&q-key-time=1743215648%3B1743219248&q-header-list=host&q-url-param-list=&q-signature=d4e2e3fd03fa1a08018f6576b86d7d32c13a9430)
Fig.6 (a).BVoff and BVon of 60V NLDMOS with different SAB thickness; (b)  The electric field of 60V NLDMOS at on state with different SAB thickness.

![OptimizedBVoff/BVonV.S.Rulem  OptimizedBVot  OptimizedBV  ginalBVo  NA   15   2.6   3.6   42  Rulem  a  (a)  OptimizedBVoff/BVonV.S.Rulen  ptimizedBVoff  OriginalBV  Rulen  b  (b)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/64ee4c4e-1ad5-4b47-be1f-a74f4f7c6359/64ee4c4e-1ad5-4b47-be1f-a74f4f7c6359.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215648%3B1743219248&q-key-time=1743215648%3B1743219248&q-header-list=host&q-url-param-list=&q-signature=f0220b3054b3a3749244d8eab517c2eed9b9e547)
Fig.7(a) The final 60V NLDMOS BVoff and on BV V.S. rule m; (b) The final  60V NLDMOS BVoff and BVon V.S. rule n.

Finally, we choose ILD thickness 7500Å, SAB thickness  1500 Å with SION150A +UVSIN300A CESL layer, the BVon

of 60V NLDMOS can be improved obviously 15V while   BVoff remain unchanged, as shown in Fig.7. The final 60V  NLDMOS BVoff and BVon characteristic V.S. rule m and n all  showed good results.

## IV. C ONCLUSION 

In this paper, we studied the influence of BEOL process such  as ILD thickness, SAB thickness and CESL type on NLDMOS  characteristic, especially BVon characteristic. While ILD is  thickened 2000A, BVon can increase 20V and the uniformity is  obviously better. Replacing CESL film from SION350A to  SION150A +UVSIN300A, BVon can also be boosted about  5V. Reduce the SAB thickness from 2000 Å to   $1200\mathrm{~\AA~}$  , the  BVon increases nearly to 12V. To sum up the above points, the  key element which can determinate NLDMOS BVon is metal  RESURF resulting in drain end impact ionization and electric  field strength. Finally, we choose ILD thickness 7500Å, SAB  thickness 1500 Å with SION150A +UVSIN300A CESL layer,  the BVon of NLDMOS can be improved obviously while  BVoff  remain unchanged.

As LDMOS's operating voltage gears continue to rise, and  toward smaller line widths and higher cost performance, the  device characteristic is consequentially   more sensitive to the  process, and the process window is also shrinking. We need to  consider and take advantage of the process to improve the  characteristics and stability of the LDMOS.

## A CKNOWLEDGMENT 

This work was supported in part by   School of  Microelectronics, Southeast University.

## R EFERENCES 

[1] A. W. Ludikhuize, “A review of RESURF technology,” Proc. of  ISPSD,2000, pp. 11–18.    [2] Tsung-Yi Huang1 et. al., “Demonstration of a HV BCD Technology with  LV CMOS Process”, ISPSD, pp. 193-196, 2015.C.     [3] Kwang-Sik Ko et. al., “HB1340 Advanced 0.13um BCDMOS  technology  of complimentary LDMOS including fully isolated transistors”, ISPSD,  pp. 159-162, 2013.298    [4] P. A. Heimann, S. P. Murarka, and T. T. Sheng, “Electrical conduction and  breakdown in oxides of polycrystalline silicon and their correlation with  interface texture,” J. Appl. Phys., vol. 53, pp. 6240-6245,1982.    [5] Andersen and D. R. Ken, “Evidence for surface asperity mechanism of  conductivity in oxide grown on polycrystalline sili- con,” J. Appl. Phys.,  vol. 48, pp. 4834-4836, 1977.     [6] M. Denison, M. Pfost, K.-W. Pieper, S. Märkl, D. Metzner and M. Stecher,  “Influence of Inhomogeneous Current Distribution on the Thermal SOA  of Integrated DMOS Transistors”, Proc. of ISPSD’04, pp. 409-412, 2004.     [7] H. Fujii, T. Mori and T. Ipposhi, “A Recessed Gate LDMOSFET for  Alleviating HCI Effects”, Proc of ISPSD’16, pp.167-170, 2016    [8]  Guanyu Chen, “The data Retention Improvement with 2T Structure OTP    on 0.18um CMOS Technology”, IEEE 2015. 978-1-4799-8485-5.

