---
title: "291_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_8f5aa944b2d61f09491caa88706d47b87295230462135641
file_size: 365304
---

## Analysis of Turn-on Uniformity of Multi-finger  DDSCR Devices under ESD Stress  

Yang Wang 1,3 \* , Dandan Jia 1,3 , Xijun Chen 1,3 , and Xiangliang Jin 2,4   1 Department of Physics and Optoelectronics, Xiangtan University, Xiangtan, Hunan, 411105, China   2 Department of Physics and Electronics, Hunan Normal University, Changsha, 410081, China    3 Hunan Engineering Laboratory for Microelectronics, Optoelectronics and System on A Chip, Xiangtan, Hunan, 411105, China   4 SuperESD Microelectronics Technology CO.,LTD., Changsha, Hunan, 410100, China   \* Phone: +86 731 58292195     Fax: +86 731 58292332     Email:  wangyang@xtu.edu.cn

Abstract-    This paper presents a detailed study of turn-on  uniformity under electrostatic discharge events in single-finger  and multi-finger traditional DDSCR devices. Since the structure  of the multi-finger DDSCR device is not completely symmetrical,  the electric field strength of each finger breakdown junction is  different, resulting in different impact ionization rates. Therefore,  each finger of device cannot be turned on at the same time, and the  turned-on finger enters the snap back region and pull down the  voltage of the device. If the ESD failure voltage Vt2 of the  multi-finger device is less than the trigger voltage Vt1, then  other  fingers will not turn on until the device fails, and the ESD current  can be only discharged through the partial area. The transmission  line pulse (TLP) test results show that the failure currents It2 of  the single-finger, 2-finger and 4-finger DDSCR devices are 6.22A,  11.83A and 13.33A, respectively, and the 4-finger device cannot be  uniformly turned on.

Keywords  –   ESD, DDSCR, Turn-on uniformity, Device  simulation , Multiple-finger.

## I. I NTRODUCTION 

Silicon Controlled Rectifier (SCR) device is a very effective  ESD protector, which has the advantages of large discharge  current per unit area, small on-resistance, strong robustness and  high protection level, and it can be realized in semiconductor  planar process, receiving attention from the industry widely [1,  2] . Albert Wang first proposed the Dual Directional Silicon  Controlled (DDSCR) in 2001, which clamps the voltage in both  forward and reverse directions [3, 4]. In order to use the layout  area effectively, it will be generally made into a multi-finger  device, and the ESD protection capability is improved by  increasing the number of fingers. However, the multi-finger  device has uneven conduction problem. Some papers have  studied the uneven triggering phenomenon of GGNMOS and  proposed some solutions, but there is still little research on the  current discharge uniformity of multi-finger DDSCR devices  [5] - [7]. In 2013, a variety of multi-finger unidirectional SCR  triggering schemes were included in a US Patent, but did not  involve specific device fabrication and test results comparison  [8]. From the perspective of the layout, You Li examined the  influence of the two layout ACA and CAC of SCR devices  on  the failure current [9]. But in fact, once the number of fingers is  greater than two, the layout of the device will be a mixture of

two forms, and the reference for layout design of SCR device  with more than two fingers is of little significant. Therefore,  grasping the ESD performance of the DDSCR device and  analyzing its cause of non-uniformly in the ESD event is  beneficial to better design and optimize the DDSCR ESD  protection device.

Based on a   $0.5{\mathrm{-}}{\upmu\mathrm{m}} $  5V/18V CDMOS technology, the  DDSCR devices with different fingers were compared and  analyzed. The impact ionization rate and current distribution  characteristics of multi-finger DDSCR devices are simulated  and analyzed by TCAD, and Thermo's Celestron TLP machine  is used to test the device I-V characteristic curve. The test  results confirm the correctness of the simulation analysis.

## II.   EXPERIMENTS  

Fig. 1 is a cross-sectional of  2-finger DDSCR device. The  cathode of the device shares a P-well (PW), and each PW and  the substrate P_SUB are isolated by an N-type deep well  (NWD), so that the fingers in different PWs become mutually  independent bipolar transistors. The 2-finger structure of the  DDSCR is completely symmetrical.

![Leftside  Left side   Centralaxis  Central axis  Rightside  Right side  finger  finger  finger  finger Anode  Anode  Cathode  Cathode  Anode  Anode F  F FOX  FOX  FOX  O  FOX  FOX  O  FOX  FOX  FOX X  X P+ N+ B+  7T   P+  P+ 一+   N+ P+ +   N+ +   P+ 一+   P+ 一+   N+ P+ +  P+  Pv  PW  PW  Pv  PW NMMD  NWD PSUB  PSUB Fig. 1 Cross section of 2-finger DDSCR device.  Fig. 1 Cross section of 2-finger DDSCR device.   ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7e67a96c-3c27-47de-a10b-4c81ad20d0a5/7e67a96c-3c27-47de-a10b-4c81ad20d0a5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=01baa16c320cf51f1e54ec27b12936b29887bea8)
Fig. 2 shows a cross-section of the 4-finger DDSCR device,  which has an interdigital finger of a common anode PW and an  interdigital finger of a common cathode PW. The device has  two fingers on both sides of the central axis, and the PW is  shared by the cathodes on the same side. There is one  $\Nu+$   in the  outer interdigitated anode PW, and two   $\Nu+$  in the inner  interdigitated anode PW, so the 4-finger structure is not  completely symmetrical.

![Leftside  Left side   Central axis  Central axis  Right side  Right side  fingers  fingers  fingers  fingers Anode  Anode  Cathode  Cathode  Ariode  Anode  Cathode Cathode   Anode  Anode F  F  F  F FOX  FOX  O  FOX  FOX  O  FOX  FOX  O  FOX  FOX  O  FOX  FOX X  X  X  X P+ N+  P+  P+  N+ P+ N+  P+  P+  N+ P+ N+  P+  P+  N+ P+ N+  P+  P+  N+ P+ Pvv  PW  P  PW  PW  PW PP   Pvv  PW NWD NVVD  PSUB PSUB  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/21ca6d6a-47ec-4ecb-9575-99dae69e114a/21ca6d6a-47ec-4ecb-9575-99dae69e114a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=8d7bd6d2f73ba1f1ad26fe01b0e99f0392035f7b)
Fig. 2 Cross section of 4-finger DDSCR device.

The structure of the multi-finger device except the two-finger  device is not completely symmetrical, and the internal finger  and external finger electric field strengths are different, so that  the impact ionization rate is different near the breakdown  junction formed by the   $\mathrm{P}+$  and NWD regions [10]. The  breakdown junction  with a higher impact ionization rate will  first reach the avalanche breakdown condition and the  avalanche breakdown will cause the finger to turn on first,  resulting in non-uniform conduction of the device.

Taking forward conduction as an example, when a positive  ESD pulse appears on the Anode, if a finger of the DDSCR is  turned on first, the finger will quickly enter the snap-back  region to lower the device voltage. Since the base of each finger  parasitic NPN tube is isolated by the NWD, the substrate  current of the finger cannot flow to the base of the  non-conducting finger, and the base potential cannot be raised  to cause the non-conducting finger to trigger.

The relationship between electric field strength E and impact  ionization rate α  :

$$\alpha_{\mathrm{i}}=A\mathrm{exp}[-(\frac{B}{E})^{m}]$$
(1)

Where A, B, and m are constants. It can be seen that the  impact ionization rate is strongly dependent on the electric field  strength, and the impact ionization rate increases as the electric  field strength increase.

The range of the barrier region is represented by 0 to xd, and  the relationship between the impact ionization rate  α   and the  avalanche multiplication factor M is as follows:

$$M=\frac{1}{1-\displaystyle{\int_{0}^{x d}}\!\!\!\alpha_{i}d x}$$
(2)

Avalanche breakdown conditions：

$$M\rightarrow\infty$$
(3)

Equation (3) can be written as:

$$\int_{0}^{x d}\!\!\!\alpha_{i}d x\!\rightarrow\!1$$
(4)

It can be seen from the formula (4) that the higher the impact  ionization rate, the faster the avalanche breakdown condition  can be satisfied and the avalanche breakdown occurs.

Fig. 3 (a) shows the impact ionization rate of the 2-finger  DDSCR device at the time of triggering. Since the structure of

the 2-finger device is completely symmetrical and the electric  field strength is the same, the impact ionization rate near the  breakdown junction of the two fingers is similar, and the  avalanche breakdown can occur simultaneously. Fig. 3 (b) is  the current density distribution of the 2-finger device, the  2-finger device can be turned on evenly.

![(a)  (a) Anode  Anode  Cathode  Cathode  Anode  Anode S3N4  silicor  S102  Conductoi  Electrode:  （b)  (b) Anode Anode   Cathode  Cathode  Anode Anode  S3N4.  Conductor  Electrode  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1756ab3c-bee4-4730-9182-a8e7acf53b73/1756ab3c-bee4-4730-9182-a8e7acf53b73.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=344af1faf9d389701d289ce1379d84c5d575f706)
Fig. 3 Impact ionization rate (a), and current density distribution (b) of  2-finger DDSCR.

Fig. 4(a) shows the impact ionization rate of the breakdown  junction when the 4-finger device is triggered. Fig. 4(b) shows  the current density distribution of the 4-finger device. It can be  seen that the inner two finger impact ionization rate is higher  than that of the other fingers, so the avalanche breakdown  condition is first reached. After the inner two finger avalanche  breaks down, it enters the snap back region, pulling down the  device voltage, making the remaining fingers unable to turn on  because they cannot meet the conditions. Therefore, the  internal two finger of the device turn on, while the external two  fingers pass through without current.

## III. R ESULTS AND DISCUSSION 

The DDSCR devices of 1, 2 and 4 fingers were fabricated  by 0.5-µm 5V/18V CDMOS technology. Fig. 5 shows the TLP  test curves for different finger DDSCR devices. The key test  parameters are listed in Table 1.

![(a) a)  Anode  Cathode  Anode  Cathode  Anode (b) Anode  Cathode  Anode  Cathode  Anode ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fad68335-8ada-4fd4-b770-9fd2b9ff55bc/fad68335-8ada-4fd4-b770-9fd2b9ff55bc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=e91b56605a7411244c4e7c2f845a75c468f192f1)
Fig. 4 Impact ionization rate (a), and current density distribution (b) of  4-finger DDSCR.

The failure currents It2 of the 1, 2, and 4 traditional devices  of the DDSCR are 6.22A, 11.83A, and 13.33A, respectively.  2-finger DDSCR's It2 is twice as large as a single-finger  device, so the device can be turned on evenly. The It2 of the  4-finger device is similar to the 2-finger device, and it can be  considered that only two fingers are working, and the device is  non-uniformly turned on. The venting capacity has not been  fully explored. After the two fingers of the 4-finger DDSCR  are turned on, the device enter the snap back region to pull  down the device voltage. Since the device's failure voltage Vt2  is lower than the non-conducting finger's trigger voltage Vt1,  the non-conducting fingers cannot be turned on before the  device fails.

![Leakage( A) Leakage（A）1E-10 1E-9 1E-8 1E-7 1E-6 1E-5 1E-4 1E-3 0.01 0.1 1E-10 1E-9 1E-8 1E-7 1E-6 1E-5 1E-4 1E-3 0.01 0.1 114- 141212- 10— 10Current(A)Y 864 1-finger DDSCR1-finger DDSCR 22-fingerDDSCR  2-finger DDSCR 4-finger DDSCR4-finger DDSCR 0-1010 -5051015202530354045505560 -5 0 5 10 15 20 25 30 35 40 45 50 55 60Voltage(V) Voltage（V）](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/26099d23-d595-4dcb-a1ed-e9631410be98/26099d23-d595-4dcb-a1ed-e9631410be98.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=87042bda7b19caf767f9089dfed85d37962baa63)
Fig. 5 TLP I-V curve for DDSCR devices with different number of fingers.  In addition, Table 1 shows the Vh of 1, 2 and 4 finger  devices, which are 10.42V, 6.67V and 5.52V, respectively,  and as the number of fingers increases, the Vh decreases  accordingly. If the device with high ESD failure current is to

be obtained by increasing the number of fingers, it may cause  the latch-up risk of the protected circuit. Therefore, when  applying a multi-finger DDSCR device to protect the core  circuit, a trade-off should be made between the holding  voltage and the fail current.

Table I - TLP data for 1-finger, 2-finger and 4-finger DDSCR

|        Device                name      |Vt1（V)|vhV|Vt2(V）|It2(A)|
|---|---|---|---|---|
|        1-finger                DDSCR      |20.26|10.42|45.15|6.２２|
|        2-finger                DDSCR      |21.57|6.67|38.19|11.83|
|        4-finger                DDSCR      |21.26|S.S２|22.17|13.33|


## IV. C ONCLUSION 

This paper introduces a traditional DDSCR device under a  0.5-µm 5V/18V CDMOS technology. Through the TCAD  electrical performance simulation and TLP test of the  multi-finger DDSCR device, the reason for the DDSCR turn-on  uniformity is analyzed. Test and simulation analysis show that  the failure current of the 2-finger DDSCR device is twice as  high as that of the single finger, and the 4-finger DDSCR device  has little difference from the It2 of the 2-finger DDSCR device.  This is because the structure of the 2-finger DDSCR device is  completely symmetrical. The impact ionization rate of the  2-finger device's breakdown junction is similar, and the  avalanche breakdown condition can be achieved at the same  time, so the two fingers are simultaneously turned on. The  structure of the 4-finger device is not completely symmetrical.  The highest impact ionization rate of the breakdown surface is  the first to reach the avalanche breakdown condition. The  first-on finger enters the snap-back region, causing the device  voltage to drop and  other fingers to be unable to turn on. At  the same time, it can be observed that the DDSCR device has a  significant decrease in the sustain voltage as the number of  fingers increases, increasing the risk of latch-up. Therefore,  when we want to increase the degree of protection of the device,  we cannot increase the number of fingers blindly.

## A CKNOWLEDGMENT 

This work is supported by National Natural Science  Foundation of China (Grant No. 61704145, 61774129,  61827812), by Hunan Provincial Natural Science Foundation  of China (Grant No. 2019JJ50609) and by Key Technology  Program of Changsha (Grant No. kq1703001).

## R EFERENCES 

[1]    Keppens B, Mergens M P J, Trinh C S, et al. ESD protection solutions for  high voltage technologies[J]. Microelectronics Reliability, 2006, 46(5):  677-688.

[2]    Ker M D, Hsu K C. Overview of on-chip electrostatic discharge  protection design with SCR-based devices in CMOS integrated  circuits[J]. Device and Materials Reliability, IEEE Transactions on, 2005,  5(2): 235-249.

[3]    Wang A Z H, Tsay C H. On a dual-polarity on-chip electrostatic discharge  protection structure[J]. Electron Devices, IEEE Transactions on, 2001,  48(5): 978-984.    [4]    Wang A Z H. On-chip ESD protection for integrated circuits: an IC design  perspective[M]. Springer Science & Business Media, 2002: 115-121.    [5]    Mergens M P J , Verhaege K G , Russ C C , et al. Multi-finger turn-on  circuits and design techniques for enhanced ESD performance and  width-scaling[C]//   Electrical   Overstress/electrostatic   Discharge  Symposium. IEEE, 2003.    [6]    Ker M D , Chen J H . Self-Substrate-Triggered Technique to Enhance  Turn-On Uniformity of Multi-Finger ESD Protection Devices[J]. IEEE  Journal of Solid-State Circuits, 2006, 41(11):2601-2609.    [7]    Huh Y J , Axerad V , Chen J W , et al. The effects of substrate coupling  on triggering uniformity and ESD failure threshold of fully silicided  NMOS transistors[C]// Symposium on Vlsi Technology. IEEE, 2002.    [8]    Ker M D, Lin C Y, Wang C T. ESD protection circuitry with multi-finger  SCRS: U.S. Patent 8379354[P]. 2013-2-19.    [9]    Li Y, Liou J J. Multiple-finger turn-on uniformity in silicon-controlled  rectifiers[J]. Solid-State Electronics, 2010, 54(12): 1641-1643.    [10]   Wolf, HelmutF. Semiconductors[M]. Wiley-Interscience, 1971.

