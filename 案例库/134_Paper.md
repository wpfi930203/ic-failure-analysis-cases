---
title: "134_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_9388a4fedb3cfddd10d62e01cab591477295230462135641
file_size: 543405
---

## Radiation-Hardened Memory Cell for Ultralow Power Space Applications 

Chunhua Qi a) , Guoliang Ma a) , Tianqi Wang a) , Chaoming Liu a) ,    Liyi Xiao b) , Heyi Li a) , Yanqing Zhang a)\* , Kairui Guo  a) , Mingxue Huo a) , Guofu Zhai c)

a)    Laboratory for Space Environment and Physical Sciences, Harbin Institute of Technology, Harbin, 150001, China.  b)    Microelectronics Center, Harbin Institute of Technology, Harbin, 150001, China.    c)    Reliability Institute for Electric Apparatus and Electronics, Harbin Institute of Technology, Harbin, 150001, China.  \*Email: zhangyanqinghit@163.com

## Abstract 

In this paper, a novel radiation hardened memory cell for low-voltage operation and ultralow power space applications is  proposed, and named as RHDMC. By special layout design, RHDMC can not only tolerate single event upset, but also can mitigate  single event multiple upsets. Compared with recently published low power memory cell for low-voltage operation, simulation  results (not on experimental data) show that, at the expense of a   $129.5\%$   area overhead, the proposed memory cell can provide  much lower power consumption during SEU occurrence. To make comparisons, access time and power are also investigated  between our proposed memory and LA13T.

I.

## INTRODUCTION 

As stated by international technology roadmap for  semiconductors (ITRS),   $90\%$   of the processor’s chip area is  occupied by SRAM  [1] . It makes researchers draw great  attention to reduce power consumption of SRAM cell to  achieve low power integrated circuit (IC) design. Previous  research has found that reducing the supply voltage to the  near-threshold or subthreshold region  [2]  is the most efficient  way to achieve low power operation. As a guideline, designers  have proposed many memory cells for low-voltage operation  [3-5] . However, when these low power memory cells are used for  harsh space applications, they cannot tolerate single event  upsets (SEU). Thereby, designing a memory cell for ultralow  power space application and low-voltage operation has become  an urgent need.

Fortunately, some memories used for this area have been  proposed these days  [6-7] . LA13T  [7]  proposed by Lior Atias is  one of these memory cells, which can not only tolerate SEU  occurring on its internal nodes, but also achieve ultralow power  consumption at low supply voltage operation. However,  LA13T cell has its drawback, that is, an undesired path from  Vdd to Gnd will be formed during SEU occurring on some of  its internal nodes. This undesired path makes LA13T consume  a lot of energy, which is not discussed in [7].

In this paper, we proposed a radiation hardened by design  memory cell for low-voltage operation and ultralow power  space applications to solve the problem occurring on LA13T  cell, and named as RHDMC. The basic principle of this design  is to block the unwanted paths from Vdd to Gnd in LA13T to  save energy.

In fact, the memory cell proposed here is an enhanced  structure of our previous work of RHD13T  [8] . The asymmetric  structure (one C-element) in RHD13T is replaced with the  symmetrical structure (two C-elements) to enhance the  radiation resistance of node Q and A. Simulation results (not on  experimental data) show that node Q and A of RHDMC can  tolerate more than 114.5fC injected charge, by contrast, node A  and Q of RHD13T designed in our previous work can just  tolerate no more than 30fC injected charge  [8] .

The remaining of this paper is organized as follows: in  Section 2, our proposed RHDMC cell is given and discussed.  Post-simulation results are shown in Section 3. Section 4  concludes this paper.

## II.   PROPOSED MEMORY CELL 

Fig. 1 shows the structure of our proposed RHDMC. It is  designed to solve the problem of LA13T mentioned in section  1. Instead of inverter dual-driven separated-feedback  mechanism in LA13T, the node Q in our proposed RHDMC is  driven by two C-elements which are made up by transistors N3,  N4, N6, N7, P3, P4, P6 and P7 respectively. The inputs of these  two C-elements are node QB1 and QB2.

![MBL WBLVDDDD  DD VDDWWLAEPI P1 P2 P2WDD VDDP3P3  Ps P5P6 P6QB1 QB1 P4 P4 P P7 OB2 QB2T3 N3 Q DNY  N6N4 DBL N7MS N53 BN1 2 N2WBL WBL WWL WWL](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/47f67bdb-5466-437a-954c-2cad4f790588/47f67bdb-5466-437a-954c-2cad4f790588.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=a96d6225c7a707ce35d5ec0a58d103cd273086a8)
Fig. 1. Proposed memory cell----RHDMC.

Assuming our proposed memory cell store state 1 at Q, the  ON/OFF states of the devices at the internal node states are  shown in Fig. 2 (a). If an energetic ion strikes on node QB2, the  state of node QB2 upsets from 0 to 1, it temporarily turns on  transistor N4, N5, and N6, turns off transistor P3, P5 and P7.  The ON/OFF state of changed transistors is high-lighted with  yellow line in Fig. 2 (b), which shows that there is no path  forming from Vdd to Gnd during SEU occurrence. The same

conclusion can also be drawn that the unwanted path from Vdd  to Gnd cannot form during an SEU occurring on any of these  five nodes, that is A, B, QB1, QB2, and Q. Accordingly, if  assuming RHDMC stores state 0 at Q, the undesired path  cannot form either. It means that by changing inverter to  C-element, our proposed memory cell can well solve the  problem appearing in LA13T during SET occurrence.

![DD  VDD  DD  VDD A  “ 1 ” P1 P1   P2  P2 VD D P3  P5 P6 P6  QB1  QB1  P4  P7  QB2 OB2  “ 0 ”  “ 1 ”  “ 0 ” N3  Q  N6 N4 N7 ZZS  N5 B 21  N1  N2 “ 133  1 ” (a) Logic “1” state.  (a) Logic “1" state.  DD  VDD  VDD  VDD A  “ 1 ” P1  P2  P2 VD D P3  P5 P6 PS  QB1 QB1   P4  P7  QB2  QB2 “ 0 ”  “ 1 ”  “ 1 ” N3  Q  N6 76  N4 N7 NS  N5 B N1  N2 “ 1 ”   (b) An SEU occurs on node QB2.  (b)AnSEUoccursonnodeOB2  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9686f271-0b61-471f-84e5-f0f62b2b1ec3/9686f271-0b61-471f-84e5-f0f62b2b1ec3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=898ab1e7780e7957c103391051efff2b4c46d97a)
Fig. 2. Stable state 1 of our proposed RHDMC. For simplicity, access  transistors were omitted from these figures.

The behavior of the proposed memory cell against SEU is  explained in details here (assuming state 1 is stored at node Q):

1) If an SEU occurs on node QB2 (or QB1), the state of node  QB2 upsets from 0 to 1, it makes the output of C-element, node  Q, become high impedance. In other words, node Q will not be  affected. With the help of on-transistor N2, node QB2 can be  recovered to its initial state 0.

2) If an SEU occurs on node Q, the state of Q will change  from 1 to 0, which temporarily changes the state of node A to 0  through on-transistor P5. The change of node A to 0 is a very

slow process, because PMOS transistor P5 can only provide a  weakly driven ability for state 0. However, the stacked PMOS  transistors P3, P4, P6, and P7 provide a strongly driven current  for the state 1 of node Q. With the help of strongly driven  ability provided by transistor P3, P4, P6, and P7, node Q will  recover to its original state 1 faster than node A changes to 0,  which means RHDMC can tolerate this SEU event. The  simulation results of SET behaviors for node A and Q in Fig.3  can verify the analytical conclusion in this section.

![500m 500m Time（S) 10  1.002u ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b0fd4105-a575-42aa-abd9-5c9c7d37a83e/b0fd4105-a575-42aa-abd9-5c9c7d37a83e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=f6405d1cf68c8d96a72d36854d4fdf563fb22a3d)
Fig.3 SET behaviors of node A and Q when node Q is hit

3) If an SEU occurs on node B, transistors N1 and N2 will  both turn off. However, this cannot further affect the states  stored at node QB1 and QB2. Since transistor N5 still at its off  state, node Q will not be affected either.

4) Since the current induced by a particle hit always flows  from n-type diffusion to p-type diffusion through a p-n junction  [9-10]. A radiation particle strike cannot flip the state of node A  from 1 to 0 because it is made up of only PMOS transistors;  vice versa, if stores state 0 at node Q, the node voltage cannot  flip the state of node B from 0 to 1 for only NMOS transistors  surrounding it.

These analyses will be verified by corresponding  post-simulations (not on experimental data) in next section.

## III.   EVALUATIONS 

Simulations in this section are HSPICE post-simulations  using 65 nm commercial technology with   $0.5~\mathrm{V}$   power supply  at room temperature. Here, we injected charge on node QB2,  QB1, Q, and B (or A, depend on store state) at 0.5 µs,   $0.8~\upmu\mathrm{s}$  ,   $1.1~\upmu\mathrm{s}$   and  $1.4\;\upmu\mathrm{s}$   successively. To simulate the behavior of the  upset striking on a node, a well-known time-varying  exponential current source is utilized which is proposed in [11]:

$$I(\mathrm{t})\,{=}\,I_{0}\biggl(e^{\frac{-t}{\tau_{\alpha}}}{-}e^{\frac{-t}{\tau_{\beta}}}\biggr)$$
where τα is the collection time constant of the junction;  $\uptau\upbeta$   is  the time constant for initially establishing the ion track.  Considering references [12–19], τα and  $\uptau\upbeta$   are set to 164 ps and  50 ps, respectively. The value of   $1\,\mathrm{\mA}$   is chosen for   $I_{0}$   to  simulate a 114.5 fC disruption at each node. The simulation  results of node Q are plot in Fig. 4, it can be concluded that our  proposed memory cell can tolerate SEU occurring on any of its  single node, which confirmed the discussions in section 2.

Table 1 shows the power consumption under different  injected charge quantities during SEU occurrence. It can be  concluded that when an SET occurs on the node QB1, our  proposed memory cell consumes almost the same power as  LA13T (in fact, at least   $20\%$   lower than LA13T). However,  when an SET occurs on the node QB2, LA13T consumes more  power than our proposed RHDMC, it is hundreds of times

higher than our proposed memory cell. These results can be  easily explained by Fig. 5.

![1.5  ：500m  (a) Store 0  (a) Store 0 A QB2  QB2  QB1  QB1  Q Voltage (V)  EB  B 500m  (b) Store 1  (b) Store 1 -500m  SET  SET injected  injected 5□0工   1三   1.5红  Time (s)  Time (s) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b8e5185b-bd69-4a7b-af64-ea6e1efa0289/b8e5185b-bd69-4a7b-af64-ea6e1efa0289.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=ef14aa5f2be037e5d0cba67e866934188f296141)
Fig. 4. SET tolerance simulation results of node Q in RHDMC.

Fig. 5 is the simulation results of 45.8 fC charge injected on  the node QB1 and QB2, we can see when an SET occurs on  node QB1 no matter in LA13T or RHDMC, it will recover very  fast, which leads to very little power consumption. However,  when an SET occurs on node QB2, the node QB2 in LA13T  needs a long time to recover to its original state, this makes the  path from VDD to GND in LA13T has a long opening time  consuming a lot of energy, while node QB2 in RHDMC  recovers as fast as node QB1.

Table 1 Power consumption during the memory upset

|Injected|RHDMC|RHDMC|LA13T|LA13T|
|---|---|---|---|---|
|charge|OnQB1|OnQB2|OnQB1|        OnQB2                nw      |
|(FC）|nw|nw|nw|        OnQB2                nw      |
|Ｓ|1.01|1.30|1.33|442.60|
|11.4|1.19|1.65|1.53|439.69|
|17.1|1.28|1.87|1.65|438.32|
|２２.9|1.35|2.03|1-74|437.60|
|28.6|1.40|２.１２|1.81|437.08|
|34.3|1.4S||1.87|436.62|
|40.0|1.49|２.3１|１.9２|436.18|
|4S.8|1.53|2.40|1.97|435.94|


![4口m  ②□m   266m  SET  SET  SET  SET -200m    -200m  -400m   1-4口口m  -600m   -600m  -800m   -800m  (a) node QB1 in LA13T  (a) node QB1 in LA13T  (c) node QB1 in RHDMC  (c) node QB1 in RHDMC Voltage (V) 6ggm   Voltage (V) 多目目用  -290m   SET  SET -200m   SET  SET -400m   -40m  -600m    -600m   -800m    -800m   一一   (b) node QB2 in LA13T  (b) node QB2 in LA13T  一1   (d) node QB2 in RHDMC (d)nodeQB2inRHDMC  1三   3   51   1   55  Time (s)  Time (s)  Time (s)  Time (s) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/227a759f-3ce6-4f2c-80fe-0b3eb3800f23/227a759f-3ce6-4f2c-80fe-0b3eb3800f23.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=327bbfe7b9caf7177220db324dc9b2948863afe8)
Fig. 5. SET recovery behavior.

T he layout of our proposed memory cell is implemented in  65nm commercial technology and shown in Fig. 6. Nowadays,  as technology scales, a single high-energy particle strike can  disrupt several reversed-biased p-n junctions simultaneously,  which is so called single event multiple nodes upsets. In order  to separate these reversed-biased nodes, the layout of our  proposed RHDMC has been specially designed, which makes  every pair of these sensitive nodes separated either by distance  or by placing an unbiased junction. That is, we use unbiased  junction to separate Q or QB1/QB2 for protection, and this  technique has been discussed in details in [7]. Besides. the  distance is used to separate Q and A or B. By measuring layout  in Fig.5, the straight-line distance between Q and A (or Q and  B) is   $1.80~\,\upmu\mathrm{m}$   (or   $1.78~\,\upmu\mathrm{m})$  ), which means that the actual  distance in the same well (or substrate) between them nears 2   $\upmu\mathrm{m}$  . As state in [20], the range of charge sharing is about   $2~{\upmu\mathrm{m}}$

between NMOS (or PMOS) transistors, it means that charge  sharing will never occur between Q and A (or Q and B). So, by  the special layout design, RHDMC can mitigate single event  multiple upsets, and it occupies   $3.48\upmu\mathrm{mX1.68\upmu\mathrm{m}}$   area  overhead. Compared with LA13T cell which re-implemented  in the same technology, our proposed RHDMC cell has a   $29.5\%$   increase in nominal area.

Fig. 7 is the simulation results of average access time and its  corresponding dynamic power consumption. It can be seen that  read access time and power consumptions of our proposed  memory cell is smaller than LA13T. However, write access  time and power consumption of our proposed memory cell are  much larger. This is due to the stacked structure C-element  used in our proposed memory. Though our proposed memory  has poor performance of write access time and write dynamic  power consumption, RHDMC has successfully solved the  problem appearing in LA13T and saved much more energy

which would be consumed in LA13T during SEU occurrence.  Last but not least, as stated in [21], most of the time SRAM  cells stay in the standby mode. It means when used in harsh  radiation environment, the increasing write access time and  write dynamic power consumption of our proposed memory  worth it.

![y(μm)  y( μ m) VDD 3.5 P1  P4  P3  P6  P7  P2 Q 3 2.5 B RBL P5 2  RVVL.  RWL QB1 DBI   QB2 WWL 1.5  N5 WBL A 1 Q 0.5 N1  N3  N4  N7  N6  N2 GND 0  0.5  1  1.5  x( μ m)  x( μ m) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/43cfaa18-d225-4b7d-a81f-5733d2aad5c4/43cfaa18-d225-4b7d-a81f-5733d2aad5c4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=48c83dadedf9f0fd30b3d0093585fb6aa453caa8)
Fig. 6. Layout of the proposed memory cell.

![write power HieDowerl   1.65 write access time tnte access ine   1 1.53 .S3  1 read power cadpower   0.86 read access time  1 0.99 0.99   RHDMC RHDMC  1  LA13T LA13T  0_0  0.0  ０.Ｓ  0.5  1.0  1.0  1.Ｓ  1.5 Normalized  Normalized ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e95f175c-8960-4f47-818f-b42a2c3c879e/e95f175c-8960-4f47-818f-b42a2c3c879e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=4bbcadefd2a0d5914eddafd622a2c8c8d00833a8)
Fig. 7. Access time and dynamic power consumption  (normalization)

## Conclusion 

A novel memory cell design for both low voltage and space  applications has been proposed in this paper. It is a variant of

the LA13T cell and referred to as RHDMC. By the special  layout design, it can not only tolerate single event upset, but  also can mitigate single event multiple upsets. A set of HSPICE  post-simulation results show that at the cost of   $129.5\%$   area,  our proposed memory cell has successfully solved the problem  appearing in LA13T.   Considering the main purpose of our  design is used in harsh radiation environment, compared with  the other memories, the performance degradation of write  access time and write power consumption is worthy.

## Acknowledgments 

This work was supported by the National Natural Science  Foundation of China (Grant Nos. 61704039, 61771167,  11775061, 11805045), the Natural Science Foundation of  Heilongjiang Province (Grant No. QC2017073), the Science  and Technology Innovation Foundation of Harbin (Grant No.  2016RAQXJ068), the Fundamental Research Funds for the  Central Universities (Grant No. HIT. NSRIF. 2018.09) and the  “111 project” (Grant No. B18017).

## References 

[1]    S. Pal, A. Islam, “Variation Tolerant differential 8T SRAM cell for  ultralow power applications,” IEEE Trans. Circuits Syst. I, Reg. Paper,  vol. 35, no. 4, pp.549-558, Apr. 2016.    [2]    S. Fisher, A. Teman, D. Vaysman, A. Gertsman, O. Yadid-Pecht, A.  Fish, “Digital Subthreshold Logic Design-Motivation and Challenges,”  in Proc.25th Convention of Electrical and Electronics Engineers in  Israel, Eilat, Israel, 2008, pp. 702-706.    [3]    N. Verma, A. P. Chandrakasan, “A 256 kb 65 nm 8T subthreshold  SRAM employing sense-amplifier redundancy,” IEEE J. Solid-State  Circuits, vol. 43, no. 1, pp.141-149, Jan. 2008.    [4]    S. Basuta, M. Shams, “Single-ended 6T Sub-threshold SRAM with  Horizontal Local Bit-Lines,” in Proc. MWSCAS, Fort Collins,  Colorado, USA, 2015, pp.1-4.    [5]    S. Pal, A. Islam, “9T SRAM cell for reliable ultralow-power  applications and solving multi-bit soft-error issue,” IEEE Trans. Device  Mater. Rel., vol. 16, no. 2, pp.172-182, Jun. 2016.    [6]    K. Wang, L. Chen, J. Yang, “An Ultralow Power Fault Tolerant SRAM  Design in 90nm CMOS,” in Proc. Canadian Conference on Electrical  and Computer Engineering, St. John’s, Newfoundland & Labrador,  Canada, 2009. pp. 1076-1079.    [7]    L. Atias, A. Teman, R. Giterman, P. Meinerzhagen, A. Fish, “A  low-voltage radiation-hardened 13T SRAM bit-cell for ultra-low power  space applications,” IEEE Trans. Very Large Scale Integr. (VLSI) Syst,  vol. 24, no. 8, pp.2622-1633, Aug. 2016.    [8]    Qi C, Xiao L, Huo M, et al. A 13T radiation-hardened memory cell for  low-voltage   operation   and   ultra-low   power   space  applications[C].International Symposium on Quality Electronic Design.  IEEE, 2017.    [9]    R. Garg, S. P. Khatri, “A novel, Highly SEU Tolerant Digital Circuit  Design Approach,” in Proc. IEEE International Conference on  Computer Design, Lake Tahoe, USA, 2008, pp.14-20.    [10]    P. E. Dodd, L. W. Massengill, “Basic mechanisms and modeling of  single-event upset in digital microelectronics,” IEEE Trans. Nucl. Sci.,  vol. 50, no. 3, pp.583-602, Jun. 2003.    [11]    Messenger G C. Collection of charge on junction nodes from ion tracks.  IEEE Trans. Nucl. Sci., 1982, 29: 2024–2031.     [12]    Rajaei R, Tabandeh M, Rashidian B. Single Event Upset Immune Latch  Circuit Design using C-Element. In: Proceedings of the 2011 9th IEEE  International Conference on ASIC. Xiamen: IEEE, 2011. 252-255.    [13]    Xuan S X, Li N, Erstad D O. SET tolerant dynamic logic. IEEE Trans  Nucl. Sci., 2012, 59: 434–438.    [14]    Xuan S X, Li N, Tong J. SEU tolerant latch based on error detection.  IEEE Trans Nucl. Sci., 2012, 59: 211–214.    [15]    Namba K, Ikeda T, Ito H. Construction of SEU tolerant flip-flops  allowing enhanced scan delay fault testing. IEEE Trans Very Large  Scale Integr (VLSI) Syst., 2010, 18: 1265–1276.    [16]    Lu Y, Lombardi F, Pontarelli S, et al. Design and analysis of  single-event tolerant slave latches for enhanced scan delay testing.  IEEE Trans Dev Mater Reliab., 2014, 14: 333-343.    [17]    Garg R, Khatri S P. Analysis and Design of Resilient VLSI Circuits  Mitigating Soft Errors and Process Variations. Springer, USA, 2009.    [18]    Sayil S, Wang J. Single-event soft errors in CMOS logic. IEEE  Potentials, 2012, 31: 15-22.    [19]    Zhou Q, Mohanram K. Gate sizing to radiation harden combinational  logic. IEEE Trans. Comput.-Aided Design Integr. Circuits Syst., 2006,  25: 155-166.    [20]    O. A. Amusan, A. F. Witulski, L. W. Massengill, B. L. Bhuva, P. R.

Fleming, M. L. Alles, A. L. Sternberg, J. D. Black, R. D. Schrimpf,  “Charge Collection and Charge Sharing in a 130 nm CMOS  Technology,” IEEE Trans Nucl. Sci., vol. 53 no. 6, pp. 3253-3258, Dec.  2006.  [21]    O. A. Amusan, A. F. Witulski, L. W. Massengill, B. L. Bhuva, P. R.  Fleming, M. L. Alles, A. L. Sternberg, J. D. Black, R. D. Schrimpf,  “Charge Collection and Charge Sharing in a 130 nm CMOS  Technology,” IEEE Trans Nucl. Sci., vol. 53 no. 6, pp. 3253-3258, Dec.  2006.

