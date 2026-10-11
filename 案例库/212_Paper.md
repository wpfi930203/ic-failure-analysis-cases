---
title: "212_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_7bb5fbf44ed88c2005a6ea64235ddf2a7295230462135641
file_size: 465728
---

## 100V Integrated Bootstrap Diode with Dynamic Field  Limiting Rings for Solving Reverse Recovery Failure  in GaN Gate Driver ICs  

Ajiang Li, Shaohong Li, Jing Zhu, Long Zhang, Tian Tian, Guichuang Zhu ， Yanqin Zou, Hao Zhu  and Weifeng Sun\*  National ASIC System Engineering Research Center, Southeast University, Nanjing, China    Phone: 86-25-83795811   Fax: 86-25-83795077 \*swffrog@seu.edu.cn

Abstract-  The mechanism of reverse recovery failure in the lateral  integrated Bootstrap Diode (BST-Diode) is investigated through  physical TCAD simulation in this paper. It is found that the  crowding of electric potential lines in the vicinity of the outermost  anode metallization and the cathode region cause two high electric  field peaks and severe impact ionization at the anode and cathode  sides. Consequently double-sided dynamic avalanche occurs and  reverse recovery failure takes place. An optimized structure with  several disconnected   $\mathbf{P}+$   dynamic field limiting rings (DFLR) at  the anode side is proposed. The reverse recovery robustness of the  optimized diode is improved by more than  $\bf{200\%}$  .

Keywords  –  BST-Diode, double-sided dynamic avalanche,  Reverse recovery failure, Dynamic field limiting rings .

## I. I NTRODUCTION 

Nowadays, Silicon-based power devices meet bottleneck in  the development towards higher switching frequency. The  emerging gallium nitride (GaN) based power devices [1]-[2]  with higher switching frequency and junction temperature are  promising alternatives to the traditional Silicon-based power  devices. However, appropriate silicon-based High Voltage gate  drive IC (HVIC) providing high-frequency and reliable gate  driving signal has become one of the biggest challenges in the  development of GaN-based power device.

Fig. 1 shows schematic of HVIC used to control GaN-based  power device in half-bridge topology. Even though BST-Diode  is the key component in HVIC, nowadays most accessible  BST-Diodes could only be used in the HVIC driving  Silicon-based power devices [3]. Few attention have been paid  to the Bulk-Silicon integrated BST-Diode [4] which could be  applicable to GaN-based gate driver IC.

In this paper, the conventional Bulk-Silicon lateral integrated  Bootstrap Diode, which could be adopted in HVIC to drive  100-rated GaN-based power devices, is first presented. The  reverse recovery failure mechanism is investigated in detail  through TCAD simulations and experiments. Finally, a novel  structure with DFLR is proposed to improve the reverse  recovery ruggedness. Furthermore, the proposed structure has  good   compatibility   with   the   conventional  Bipolar-CMOS-DMOS (BCD) process and does not require an  additional mask.

##  II. D EVICE STRUCTURE AND MECHANISMS   

Fig. 2 shows the conventional structure of Bulk-Silicon  lateral integrated BST-Diode. The con-diode adopts lowly  doped anode region to reduce hole injection efficiency. As a  result, the con-diode has very short reverse recovery time   $(\mathrm{tr})$  .

![BootstrapDiode  Bootstrap Diode WDC  VDC C IBS  BS  Upto100V  Up to 100V WCC  VCC  HO  HO Highside  High side   GaN GaN  HI  Control Units  Control Units  drive circuit  drive circuit  WSS  VSS LI  LO  LO Lowside  Low side  GaN  GaN drive circuit  drive circuit GND  GND HVIC  HVIC ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bc821222-ea8c-45c5-ae8a-bd1148085749/bc821222-ea8c-45c5-ae8a-bd1148085749.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=5e1d679000dda931ba8d1e17fa6d2eefd08c5703)
Fig. 1 Schematic of HVIC used to control GaN-based power devices

![sub  sub  cathode  cathode  anode  anode  cathode  cathode  sub  sub ···  ··· ···  ··· N+  PX  PX  N+ NB  TB  TB PK  PK  PK  PK >n+m  n+n  N-EPI  N-EPI junction  junction BP  BP  BTN  BN  BP  BP P-sub  P-sub ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bd7f3b72-fd03-454a-8ea2-9c1c85c0809c/bd7f3b72-fd03-454a-8ea2-9c1c85c0809c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=98eea024ffd9518e7ba1a8b1f28399a62b40dc83)
Fig. 2. Cross-section of the con-diode.

![20V/div(V 20V/div   D ) C L DUT  DUT 0.1A/div  0.1A/div A  (I QDS)  DS ) Double  Double  V pulse pulse   D  BUS  BUS T1  M1  Reverse Recovery  ReverseRecovery  R g G  S  Failure  Failure 15V/div(V 15V/div(V)  G ) a  (a)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b0bd09fd-fb94-41d9-aeca-3255a4792d80/b0bd09fd-fb94-41d9-aeca-3255a4792d80.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=39622ead279a8f3c0b6afd9020e14e66d298b5fe)
![subanodeAl2n-driftpad  sub  anode  Al2  n-drift  pad  cathode  cathode P+ n+ nsub sub  Pcathode cathod  anode node  burn-out  puirn  points points  (b)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c4b5e9ce-47aa-42c3-aa38-7076d0c1939f/c4b5e9ce-47aa-42c3-aa38-7076d0c1939f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=400d539637750daf0e7a9b748078e86367cc33ee)
Fig. 3. (a) Reverse recovery waveforms (b) Photograph of the failure  BST-Diode.

![Impact ioniza tion  Impact ionization Y(um)  Y (μm)  cathode cathode   anode  anode  [cm [cm-²s-1]  -3 s -1 ] 4E+27  4E+27 14 3E+24  3E+24 10 10  2E+21 2E+21  1E+18 1E+18  6 7E+12 7E+12  2 0 18  26  34 3   42X (μm)  42  X (μm) CCD  (c)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e8b17a48-8c9a-4151-930b-80e0c319fad3/e8b17a48-8c9a-4151-930b-80e0c319fad3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=79819ee282e2b5e20ce9a2e48bbf3d42465d6003)
Fig. 5. (a) Distribution of electric potential contours at time T0 (b) Distribution  of surface electric field along   $\mathrm{Y{=}}13\,\upmu\mathrm{m}$   at time T0 (c) Distribution of impact  ionization at time T0.

![0.0 0.0  -0.3  -0.3 Current(A) 蒙-0.5  -0.5  no reverse  noreverse  recoveryfailure  recovery failure 3-0.8  -0.8 reverserecovery  reverse recovery  -1.0  -1.0  failure occurrence  failure occurrence —di/dt=45A/μs    di/dt=45A/μs -di/dt=110A/μs   di/dt=110A/μs -1.3 -1.3  15.01 15.01   15.02 15.02T0  15.03  15.03  15.04  15.04    15.05  15.05  15.06  15.06 T0 Time(μs) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bc07e1a4-9f9a-4e7c-b264-d29879d1072d/bc07e1a4-9f9a-4e7c-b264-d29879d1072d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=2436196ba2b3e332ae68645aa6f3bb8dc643df93)
Fig. 4. Simulated reverse recovery waveforms.

![Electrostatic  Electrostatic  Yum  Y (μm) cathode cathode   anode anode   Potential[V]  Potential[V] 100 100  14 80 80  10  60 60  N-drift  N-drift  40 6 20 2 0     18 18   26  34  42X(μm)  42 X (μm) a  (a)   3.0x10 3.0x10  5 Peak at the  Peak at the  ） 2.5x10  2.5x10 5  anodeside  anode side V\*cm^-1 2.0x10  2.0x10 5 （ 1.5x10  1.5x10 5  Peak at the  Peak at the  Electric Field  cathode side  cathode side 1.0x10  1.0x10 5 5.0x10  5.0x10 4 0.0 20  20  24  24  28  28  32  32  36 36   40 0  Position(μm)  Position(μm)     (b)  b  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5eea41ed-6105-40dc-bad2-2d53b18e5085/5eea41ed-6105-40dc-bad2-2d53b18e5085.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=5e571200bb0d0a69766f23ca365e3aaac229c28b)
The reverse recovery characteristics of the con-diode have  been tested through the circuit shown in Fig. 3(a). The forward  operating current is 0.1A and   $\mathrm{V_{BUS}}$   is set at 100V. Fig. 3(a)  shows the failure waveforms of reverse recovery. The reverse  recovery current increase abruptly when reverse recovery  failure has occurred. Fig.3 (b) shows photograph of the failure  con-diode. Burn-out points are observed in the vicinity of the  Cathode and the Anode region. The burn-out points reveal the  location where the thermal failure occurred.

The test circuit shown in Fig. 3(a) is constructed by mixed  model in Sentaurus TCAD to analyze the failure mechanism of  the conventional structure. The waveforms of reverse recovery  is shown in Fig. 4. Under the condition of   $\mathrm{{dt}/\mathrm{{dt}}{=}45A/\upmu s}$  , no  reverse recovery failure takes place, while di/dt is increased up  to   $110\mathrm{A}/\upmu\mathrm{s}$  , reverse recovery failure occur after the moment T0.  T0, which is labelled in Fig. 4, is the critical point at which  reverse recovery failure is about to take place.

During reverse recovery, stored carriers would be swept out  from the depletion region to both anode and cathode sides of the  diode.  Fig. 5(a), Fig. 5(b) and Fig. 5(c) show the distribution of  the electric potential contours, the surface electric field along   $\mathrm{Y}{=}13$   and the impact ionization at time T0, respectively. As we  can see in Fig. 5(b) and Fig. 5(c), the crowding of electric  potential contours (shown in Fig. 5(a)) in the vicinity of the  outermost anode metallization and the cathode region bring  about two high electric field peaks and impact ionization at both  sides, which result in double-sided dynamic avalanche.  Consequently, the reverse recovery failure and thermal damage  taken place.

## III. I MPROVED STRUCTURE AND MEASURED RESULTS   

To improve the reverse recovery ruggedness of BST-Diode,  the electric field peaks at both sides should be further  suppressed. An optimized diode with  $\mathrm{P}+$   dynamic field limiting  rings at the anode side is proposed (see Fig. 6). Table I lists key  parameters of the optimized structure.

![sub  cathode cathode   anode anode   cathode  sub ···  ··· ···  ··· N+  PX  N+ TB  TB PK PK   n-++n  n+n   PK PK  junction  junction N-EPI  N-EPI BP  BP  BN  ZOOM IN LOOMIN   BP BP  P-sub  P-sub E PX S L  W L P+  P+  P+  P+ the outmost anode  theoutmostanode  metallization  metallization  DFLRs DFLRS  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7814f136-076c-4031-8905-27a2c15bfa93/7814f136-076c-4031-8905-27a2c15bfa93.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=ac255c99662a8c04698038fc47d27b7dbab5d466)
Fig. 6. Cross-section of the optimized diode.

Table I: Key parameters in optimized structure

|Parameters|Optimized structure|
|---|---|
|Extension of PX beyond Anode electrode, Epx (μm)||
|Distance between adjacent DFLRs, SL (μm)|O.S|
|Epitaxial layer thickness, W (μm)|O.S|
|Doping concentration of DFLRs, N (cm-3)|5E17|
|Width of the Cell Pitch (μm)|152.9|
|Doping concentration of EPI (cm-3)|1.2e15|
|Length of anode metallization (μm)||


$$\frac{d E}{d x}\!=\!\frac{q}{\xi}(\frac{j_{e}}{q\!\cdot\!\nu_{s a t(e)}}\!-\!N_{D})$$
x

$\xi$  : dielectric constant

$j_{e}:$  : total electron current            $N_{D}$   : donor concentration   $\nu_{s a t(e)}$  : electron saturation velocity

In the optimized structure we add several   $\mathrm{P}+$   dynamic field  limiting rings in the PX region to suppress the electric field  peak at the Anode side. In addition, according to the equation  above [5], the electric field peak  $\mathrm{Enn+}$   at the Cathode side could  be eased if the doping concentration near the Cathode side  (namely  N D ) is increased. The optimized concentration of TB  region is   $9.0\mathrm{e}12\mathrm{cm}^{2}$  .

![3x105  3x10 5 3x105  3x10 5    optimized diode  optimized diode Electric Field   con-diode con-diode  (V\*cm^-1) 2x105  2x10 5 2x10  2x10 5 1X10  1x10 5 5x10 5X10  4 0 1x10 X10  29 Impact ionization (cm^-3\*s^-1) 1x10 22 1x10 15 1x10 X10  8 1x10 1x101  1 20  20  24 24   28  28  32  32  36  36  40  40 Position(um)  Position(μm) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d8130bdb-467c-4f14-ab72-4c6663274d8f/d8130bdb-467c-4f14-ab72-4c6663274d8f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=059aaf7df33b3af05b1d8745d7abcc2cc5a43abe)
Fig. 8. The surface electric field and impact ionization of the optimized diode  and the con-diode along   $\mathrm{Y{=}}13\upmu\mathrm{m}$   at time T1 and T2, respectively.

![0.0  0.0 Current(A) -0.31  -0.3 -0.6 -0.61  -0.9  -0.9 -1.2  -1.2   optimized diode  optimized diode 100:  100   con-diode  con-diode Voltage(V)  75 S0  50 25  25 0 15.00 15.00   15.01 15.01T115.02 T2  T1  15.02 T2  15.03  15.03  15.04  15.04 Time(μs)  Time(μs) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/de46f159-99f1-4b54-9df7-522959891d25/de46f159-99f1-4b54-9df7-522959891d25.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=a7fe962f37d55763fbd4a6792662ebe229089a7c)
Fig. 7. Switching waveforms for the con-diode and the optimized diode.

![2-5  2.5 thecon-diode   the con-diode the optimized diode   the optimized diode 2.0 2.0  Current(A) 1.5 51.0  1.0 0.5 0.0 0  1  2  3  4  5 Voltage(V) Voltage(V)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/de77923b-a2c3-4da6-b908-973496f4cc79/de77923b-a2c3-4da6-b908-973496f4cc79.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=66f0dd35adbc822939011a19e679ccfb0177c9c7)
Fig. 9. Forward characteristics of the conventional and the optimized structure.

![  the con-diode  the con-diode 9E-10  9E-10 the optimized diode   the optimized diode 8E-10  8E-10 Current(A) 6E-10  6E-10 5E-10  5E-10 3E-10  3E-10 2E-10  2E-10 0E+00  0E+00 0  30  30  60 60   90  90  120:  120  150 IS0  Voltage(V)  Voltage(V) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/eb0a6b6d-864f-4d1e-8f36-54830c5280a9/eb0a6b6d-864f-4d1e-8f36-54830c5280a9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=c4956af5651c824f1759ee32a20bfaf5052b3834)
Fig. 10. Reverse characteristics of the conventional and the optimized structure.

Fig. 7 shows the switching waveforms of the conventional  structure and the optimized structure under di/dt of   $110~\mathrm{A}/\upmu\mathrm{s}$  and   $350\mathrm{A}/\upmu\mathrm{s}$  , respectively. The optimized structure shows no  reverse recovery failure under   $\mathrm{{dt}/\mathrm{{dt}}{=}350A/\upmu s}$  . The reverse  recovery robustness of the optimized structure is improved by  more than   $200\%$  . Fig. 8 shows the comparison of surface  electric field in the con-diode and the optimized diode at time  T1 and T2, respectively. T1 is defined as the moment when the  voltage drop of optimized diode reach 73V during reverse  recovery process. T2 is defined as the moment at which the  voltage drop of con-diode reach 73V during reverse recovery

process. Compared with the conventional structure, the  optimized structure has effectively suppressed peak electric  field and in turn has lower impact ionization at both sides  during reverse recovery period. Consequently, the reverse  recovery ruggedness of the optimized structure is significantly  improved. Fig. 9 and Fig. 10 show the forward and reverse  characteristics of the con-diode and the optimized diode. The  optimized structure has lower forward conducting voltage due  to its higher doping concentration at the cathode side. In  addition, the optimized structure has the same reverse blocking  ability as the conventional structure.

## IV. C ONCLUSION 

In this paper, the reverse recovery failure mechanism of the  conventional BST-Diode is studied in detail. Severe electric  field peaks at the anode and cathode side is responsible for the  reverse recovery failure under the condition of high  commutating di/dt. The optimized structure with dynamic field  limiting rings and higher injection dose of TB region can  suppress the electric field peak at both sides. The reverse  recovery robustness of the optimized structure can be improved  by at least   $200\%$   without sacrificing forward conducting  capability and reverse blocking capability.

## A CKNOWLEDGMENT 

This work was supported in part by the National Natural  Science Foundation of China under Grant 61804026, Grant  61874026, and Grant 61674030, and in part by the National  Key Research and Development Plan (2017YFB0402900).

## R EFERENCES 

[1]    Takafumi Akagi, Shohei Miyano, Seiya Abe, and Sathoshi Matsumoto,  “A Silicon Based Multi-Tens MHz Gate Driver IC for GaN Power  Devices,” IEEE APEC, pp. 1978-1982, 2017.    [2]    Zhou Dong, Zhiliang Zhang, Xiaoyong Ren, Xinbo Ruan, and Yan-Fei  Liu2, “A Gate Drive Circuit With Mid-Level Voltage for GaN Transistors  in A 7-MHz Isolated Resonant Converter,”   IEEE APEC,   pp.  731-736,2015.    [3]    Jing Zhu, Weifeng Sun, Yunwu Zhang, Shengli Lu, Longxing Shi, Sheng  Zhang, and Wei Su, “An Integrated Bootstrap Diode Emulator for 600-V  High Voltage Gate Drive IC With P-Sub/P-Epi Technology,”  IEEE  Transactions on Power Electronics , vol. 31, NO. 1, January 2016.    [4]    Hideyuki Funaki, Yoshihiro Yamaguchi, Keizo Hirayama, and Akio  Nakagawa, “Lateral SO1 Diode Design Optimization for High  Ruggedness and Low Temperature Dependence of Reverse Recovery  Characteristics,” Proc. 12th ISPSD, pp. 33–36, May 1998.    [5]    Zhuo Yang, Jing Zhu, Xin Tong, Weifeng Sun, Fangjuan Bian,  and Ye  Tian, “Investigations of inhomogeneous reverse recovery behavior of the  Body Diode in Superjunction MOSFET,” Proc. 29th ISPSD, pp. 155–158,  May 2015.

