---
title: "122_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_a161b9342c5ebfc978b61be6726d87297295230462135641
file_size: 9419283
---

## Nanoprobing Analysis on MOSFET Current Drift  Caused by Gate Oxide Defect  

Wei Huang 1\* , Tze Ping Chua 1 , Hong Bo Zhang 1  and C G Song 2   1   United Microelectronics Corporation (Singapore Branch), No. 3 Pasir Ris Drive 12, Singapore 519528.  2   HeJian Technology (Suzhou) Co., Ltd.   \*  Phone: +65 6213 0018-1624 Fax: +65 6213 0004 Email: zenniss_huang@umc.com

Nanoprobing technique plays an increasingly significant role during  debug on failed devices. Either higher or lower current may induce  device mismatch, which will cause the functional failure of logic  gate or memory cell if magnitude increases further. This paper will  share a new detect type - poor Gate Oxide (Gox) uniformity - which  can induce lower on-state current (I ON ) with/without asymmetry.  Further solutions and possibilities are also discussed for this kind of  cases .

Keywords  –  Nanoprobing, Transistor FA, Gate Oxide Defect .

## I. I NTRODUCTION 

MOSFET stands for Metal-Oxide-Semiconductor Field  Effect Transistor. For NMOS (n-type MOSFET), since the  channel is P-type doped whereas the source/drain is n-type  doped, if there is no voltage bias on Gate, the transistor is at off  state. According to "like charges repel, opposite charges attract"  theory of static electrical field, if there is a positive voltage  applied on Gate, the hole in p-type channel will be pushed away  , whereas electron in bulk silicon will be pulled up to the  sub-surface of the channel. With the Gate voltage increasing,  the channel will become into strong inversion mode from  accumulation and depletion mode. In this situation, the majority  carrier in both channel and source/drain is electron. If biasing a  positive voltage on drain terminal, the electron will flow from  source to drain. This is what we call "on-state".

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/28db3038-d4aa-4ee6-becb-74dd698d591a/28db3038-d4aa-4ee6-becb-74dd698d591a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=13a7ce8e518d59ba440852bd8ac06fee0dfd3a58)
Fig. 1 Energy band diagram of inversion mode [1].

As shown in Fig. 2, when the transistor is at on-state, the  current path from source to drain will include Contact of

Source/Drain (S/D), S/D junction, Light Doped Drain (LDD) of  S/D and channel. Therefore the resistance of MOSFET can be  broken down into four components,

$$\Sigma\mathrm{R=}\mathrm{R}_{\mathrm{COM}}+\mathrm{R}_{\mathrm{S/D}}+\mathrm{R}_{\mathrm{LDD}}+\mathrm{R}_{\mathrm{C h a n e l}}$$
(1)

R CONT  stands for resistance of S/D CONT and silicide,  $\mathrm{R}_{\mathrm{S/D}}$    is  for resistance of source and drain.    $\mathrm{R}_{\mathrm{LDD}}$   and   $\mathrm{{R}_{C h a n n e l}}$    represent  the resistance of LDD and channel respectively. Based on  Ohm's law   $\scriptstyle\mathrm{I}=\mathrm{V}/\mathrm{R}$  , when voltage bias on drain is constant,  current will only be dependent on the resistance of transistor.  Any variation in these four parts will induce the on-state current  drifting. If this drifting is strong enough, the circuit will  malfunction [2]

![RCONT  >>  >>>/  RSAD   RtoD   Rchannel   RLDD   RSFD    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/908a3c11-2b29-4bdc-a30b-635327c55f3f/908a3c11-2b29-4bdc-a30b-635327c55f3f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=a52e35c380b8bae5e3e1a9359d920e075d01cc4e)
Fig. 2 X-S diagram of MOSFET on-state Resistor Model.

![（C） Poly  Poy Poly ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/abda4e8f-93af-428c-8daa-56bcfbf34dc3/abda4e8f-93af-428c-8daa-56bcfbf34dc3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=30c1daeb7312520cd2fd312ae7538790fef3baad)
Fig. 3 Defects in real cases and published papers which induce MOS lower ION  and/or asymmetric. (a) Oxide residue at CONT bottom interface, (b) LDD  missing, (c) CONT Silicide missing, (d) Poly undercut, (e) AA pitting, (f) Poly  depletion.

Many published papers [2] - [4] have disclosed defect types  that could induce MOSFET lower I ON . Fig. 3 lists some of  common defects. All these defects can be traced back to the  four components in formula (1).  Fig. 3(a) and Fig. 3(c) are  caused by higher CONT resistance. LDDs are missing in Fig.  3(b) which results in higher LDD resistance. Polycrystalline  silicon gate undercut in Fig. 3(d) and AA pitting in Fig. 3(e) can  also introduce higher LDD resistance into the current path. Poly  depletion in Fig. 3(f) (poly residue after chemical solution stain)  will affect threshold voltage   $\left({{\mathrm{V}}_{\mathrm{T}}}\right)$  , which will make transistor  suffer from higher channel resistance due to lack of mobile  electrons.

Above types of resistive defects not only will lead to lower  I ON  problem of transistor, they could also cause the transistor  behave asymmetrically [2] [5]. When resistive defect locates at  drain side of the transistor (Fig. 4(a)), and a V DD  bias is applied  on Gate and Drain, V GS  (gate to source voltage) should still  equal to   $\mathrm{V_{DD}}$  , but the voltage of node "D" in Fig. 4(a) will be  smaller than  $\mathrm{V_{DD}/V_{G S}}$  . As a result, Fig. 4(d) is observed, which  shows the extension of red dashed rectangle in Fig. 4(c) along x  axis. In this situation, the transistor works in linear region.  When the resistive defect locates at source side (Fig. 4(b)),  since there is a voltage drop between node "S" and GND, the  V GS  equals to   $\mathrm{V_{DD}}$   but smaller than   $\mathrm{V_{DD}}$  . In this situation, the  transistor still can work in saturation mode, but with   $\mathrm{V_{GS}}$   and   $\mathrm{V_{DS}}$   being smaller, the   $\mathrm{LoN}$   will be smaller than that of normal  transistor. Thus Fig. 4(e) is observed, which shows the  extension of blue dashed rectangle in Fig. 4(c) along both x and  y axis. In conclusion, high resistance of defect will induce the  lower Ion, and the location of resistive defect will cause the  asymmetry.

![L00E-05 （d） P_OOE-O 6.00E-05 Vds < Vgs = VDd  5.00E-05 ep （C VDs = Vgs<VDD 5.D0E-0 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/48609859-01e0-41a5-b77d-a88032057ed0/48609859-01e0-41a5-b77d-a88032057ed0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=17f0dbd6ac9e159d966467b6153e256d77f061a7)
Fig. 4 Electrical model of MOSFET lower  $\mathrm{{Longleftrightarrow}}$   and asymmetric behavior.

## II.   C ASE  S TUDY  I  

One of test chips suffered from Vccmin tail bit failure. Based  on the shmoo result of the failed chips as shown in Fig. 5 and  Fig. 6 below, we can see that this was soft failure and  dominated by WRM (write read margin). Up to the stage of  Conductive Atomic Force Microscope (C-AFM) at CONT  layer on sample#1(Fig. 7), no anomaly was observed through  plane-view inspection process.

![-AXIS:  VCEII  Y-AXIS:  VPERI  1:440V   1.140V   840.OMV(VCELL)  (VPERI)  1.440V   1.140V   840.OMV(VCELL)  1.440V   1.140V   840.0MV  (VCELL)  (VPERI)  1.440V   1.140v   840.OMV(VCELL)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0358788f-7eca-4e08-a26b-bf3ef1a5df34/0358788f-7eca-4e08-a26b-bf3ef1a5df34.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=77754e43cbef9a000745834fffc66ebe2d43b0e1)
![opography   PMOSCurrent Map  NMOS   PNIOS  2.0OE-0  1.50E-0F   SOOE-0  100E-07  -100FE  S.00E-08  -500E-08   2.00E-07  voltage   voltage  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/66c24806-2d0b-43d9-82ce-9fbc610e231f/66c24806-2d0b-43d9-82ce-9fbc610e231f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=ae627578b21d10a9f878170daec9814978942ccb)
Fig. 7 C-AFM data collected at CONT layer.

Further measurement of I-V characteristic curve of all 6  transistors was employed with Nanoprobing. To monitor the  property of symmetry, drain-sweep and source-sweep were  subsequently conducted on every transistor. Data in comparison  sheet indicated that lower I ON  with asymmetric behavior was at  NMOS passing gate at BLB side (Table 1).

Table 1 I ON  and   $\mathrm{I_{OFF}}$   data of passing gate of failed bit

||||PG-Failure Bit|PG-Failure Bit|PG-Failure Bit|PG-Failure Bit|PG-Failure Bit|PG-Failure Bit|
|---|---|---|---|---|---|---|---|---|
||||B|B|B|BLB|BLB|BLB|
||||||Drain Sweep (a)Source Sweep(b)|Drain Sweep (a)Source Sweep(b)|        Deviation                (laHbly/min(a,b)      |DrainSweep(a)|
|        Vg=12Vd                vd=12v                Vs=Vb=0g                V(lon)      ||3.92E-05|-3.80E-05|3.01%|8.49E-06|-1.38E-05|-62.379%||
|        Vg=12Vd                vd=12v                Vs=Vb=0g                V(lon)      ||1.36E-12|1.22E-12||-1.67E-14|4.68E-13|||
|        Vg=12Vd                vd=12v                Vs=Vb=0g                V(lon)      ||-3.92E-05|3.80E-05|3.01%|-8.49E-06|1.38E-05|-62.379%||
|        Vg=12Vd                vd=12v                Vs=Vb=0g                V(lon)      ||NA|NA||NA|NA|||
|        Vg=Vs=Vs                b=0v(1om)|b      ||1.95E-12|8.61E-13||6.12E-13|5.05E-13|||
|        Vg=Vs=Vs                b=0v(1om)|b      ||2.66E-13|3.34E-13||-2.84E-13|3.73E-13|||
|        Vg=Vs=Vs                b=0v(1om)|b      ||-2.03E-12|4.69E-13||1.16E-13|1.61E-13|||
|        Vg=Vs=Vs                b=0v(1om)|b      ||NA|NA||NA|NA|||


By plotting out the I-V curve, we can better understand the  behavior of a certain transistor. Compared with the reference  transistor (Fig. 8(c)), the  $\mathrm{I_{d}-V_{d}}$   curve of failed transistor showed  a distinct asymmetric turn-on behavior with lower I ON . When  swept from drain side (Fig. 8(a)), transistor can work in  saturation region. Curve from source-sweep (Fig. 8(b)) showed  the transistor can only work in linear region. This indicated a  high resistance factor was located at source side.

![2.00E-05   3.00E-05  1.80E-05  2.50E-05  1.60E-05  1.40E-05   18uA   2.00E-05   28uA  1.20E-05  1.00E-05   1.50E-05  8.00E-06  1.00E-05  6.00E-06  4.00E-06   5.00E-06  2.00E-06  0.00E+00  0.00E+00   OS   1S  D.S   15  -2.00E-06   -5.00E-06  Drain Voltage   （a)   Source Voltage   （D)  6.00E-05  5.00E-05  56uA  4.00E-05  3.00E-05  2.00E-05  1.00E-05  0.00E+00  D.5  -1.00E-05     Reference   （C  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/59b0fef3-7a1e-4cee-a335-92b8d58e8fde/59b0fef3-7a1e-4cee-a335-92b8d58e8fde.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=354d94c79cc7d15c539f05481bd52596a2fff6dc)
Fig. 8 (a) Drain Sweep Id-Vd curve of failed Transistor, (b) Source Sweep  Id-Vd curve of failed Transistor, (c) Drain Sweep Id-Vd curve of reference  Transistor

To further analyze this problem, we firstly conducted TEM  junction stain. This would enable us to observe both the dopant  profile of LDD and S/D junction as well as the basic device  profile concurrently in one TEM specimen.

![PolyGate  Junction  Oxide  ActiveArea   Defect    ActiveArea  Fig-9   Fig.10  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8f8b2a2b-d523-4203-befa-7b83440a45f3/8f8b2a2b-d523-4203-befa-7b83440a45f3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=1732609184b50b2c37ff8116bad0df3344f55e32)
Fig. 9&10 TEM images after Junction Stain.

According to junction stain images of failed transistor (Fig.  9), the LDD and junction profile of failed transistor appeared no  abnormity as compared to that of the adjacent reference  transistor. However, by focusing on failed transistor in details  (Fig. 10), we found that there was a suspected thicker oxide film  between Poly-gate and channel at source side. The location of  suspected defect matched with our previous Nanoprobing  observation. To confirm if the suspected thicker oxide layer is  an artifact induced by chemical treatment or a real defect, we

performed Nanoprobing analysis followed by TEM on 2 nd   sample.

Table 2.   $\mathrm{{I_{ON}}}$   and I OFF  data of passing-gate of 2nd sample

|||PG-FailureBit|PG-FailureBit|PG-FailureBit|PG-FailureBit|PG-FailureBit|PG-FailureBit|
|---|---|---|---|---|---|---|---|
|||BL|BL|BL|BLB|BLB|BLB|
|||||Deviation|||Deviation|
|        Vg=1.2V                Vd=1.2V                Vs=Vb=0                M(lon)      ||1.15E-05|-1.15E-05|0.149%|3.98E-05|-3.94E-05|1.1496|
|        Vg=1.2V                Vd=1.2V                Vs=Vb=0                M(lon)      ||||||||
|        Vg=1.2V                Vd=1.2V                Vs=Vb=0                M(lon)      ||-1.15E-05|1.15E-05|0.149|3.98E-05|3.94E-05|1.1396|
|        Vg=1.2V                Vd=1.2V                Vs=Vb=0                M(lon)      ||||||||
|        Vd=1.2V                Vg=Vs=Vs                b=0v(1of)b      ||-3.52E-14|-5.43E-13||1.61E-12|-9.10E-13||
|        Vd=1.2V                Vg=Vs=Vs                b=0v(1of)b      ||8.46E-14|2.24E-13||-1.58E-13|-2.18E-13||
|        Vd=1.2V                Vg=Vs=Vs                b=0v(1of)b      ||-2.45E-13|-2.31E-13||-9.39E-13|1.39E-12||
|        Vd=1.2V                Vg=Vs=Vs                b=0v(1of)b      ||NA|A||RA|NA||


As showed in Table 2 above, despite no asymmetric behavior  was observed, lower I ON  was still found at BL (Bit-line) side  passing gate as compared to BLB side. Thus, we decided to use  High Resolution Transmission Electron Microscope (HRTEM)  without junction stain to confirm if there is thicker oxide  between poly-gate and the channel. To obtain a sharper  interface and clearer image of Gox layer, low KeV FIB milling  was adopted for TEM sample preparation.

Fig. 11 is the HR TEM image of the failed passing gate  transistor, a defect was observed at the interface between poly  gate and channel. EELS (Electron Energy Loss Spectrum)  mapping (Fig. 12) analysis of Oxygen element further  confirmed that the defect was oxide and no other light element  was detected. In accordance of the FA results of both samples,  we confirmed that the Vccmin tail bit failure was caused by  poor Gox uniformity

![PolyGate   Poly Gate  Oxide  Defect  Oxide   AA  ActiveArea   Defect  HRTEM   EELS of O  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e14758f7-5348-47df-89b6-9e6e07a126f5/e14758f7-5348-47df-89b6-9e6e07a126f5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=85b44000e8a34364ee8e2066dfa03f4cbbdb01f9)
Fig. 11&12 HRTEM image and EELS mapping result.

Based on the PFA result in Case Study together with Fig. 4,  we can summarize the electrical model of this Gox defect case  as Fig. 13. When the thicker Gox locates at source side of  nMOS (Fig. 13(a)), the   $\mathrm{V_{T}}$   of this local region will become  larger. This will result in higher channel resistance at this area,  which is tuned by voltage applied on the gate (Fig. 13(b)).  Based on the theory in Fig. 4, this thicker Gox will make the  transistor working in linear region when sweep from source  side, whereas when sweep from drain side, transistor will work  in saturation region with lower I ON . If the thicker Gox is at the  center of channel area (Fig. 13(c)), this can only cause the  resistance of transistor to be higher than normal, whereas the  I-V characteristics curve is free of asymmetric behavior.

![PolyGate  Poly Gate Oxide Defect Defect Active Area ActiveArea （a)  CC （d） ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/917014e8-4467-4dec-96fe-aa4644ae8c4e/917014e8-4467-4dec-96fe-aa4644ae8c4e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=8feeb113ce4d1871a6477651dba0527b3624e6f4)
Fig. 13 Electrical Model of Gox defect case.

## III. C ASE  S TUDY  II  

In another product, one lot wafer suffered from low yield  issue. According to the Pareto chart of failed chips’ bitmap, the  main yield killers were SRAM cluster failure and random single  bit failure. After we de-process the cluster-failure sample to  CONT layer, abnormal dark Wordline CONT PVC (Passive  Voltage Contrast) (Fig. 14) was observed at failure address.  Since the dark PVC indicates either an open CONT or smaller  capacitance [4], we decided to perform cross section TEM  analysis parallel to word-line poly-gate to cover as many  components as possible. Compared to reference bit (Fig. 16),  thicker Gox was observed between poly-gate and Active Area  (Fig. 15).

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c57a0e6e-0b12-45fd-a4db-b201b042c746/c57a0e6e-0b12-45fd-a4db-b201b042c746.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=b9ad7866fcd9764eabf92fed265b24854c5962ab)
Fig. 14 PVC image of cluster bits failed sample.

![Fig.15   PolyGate   Fig.16  PolyGate  Reference  Target  ActiveArea   ActiveArea     ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8c302467-3a0c-411e-8292-df0df1b9fd44/8c302467-3a0c-411e-8292-df0df1b9fd44.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=be726dcf10d2b9d9276272ccc8623a1364d24a9b)
Fig. 15&16 TEM image of failed and reference bit.

For random single bit failed sample, plane-view PFA was  performed followed by Nanoprobing measurement. Referring  to the test result in Table 3, lower I ON  was observed at BL side  compared with data at BLB side. Since this case is categorized  as single wafer low yield issue, with the solid PFA result on  cluster-bits failed sample, we carried out HRTEM inspection  (Fig. 17) on this single-bit failed sample. Thicker Gox was  indeed observed to induce the failed transistor with lower  on-state current. The size of defect resulted in different failure  mode. If the thicker Gox defect covered more than one SRAM  cell, the failure mode should be twin-bits or cluster bits. For  smaller Gox defect within one transistor, it could only induce  single bit failure.

Table 3 Test result of failed SRAM bit.

|||BL|BL|BLB|BLB|
|---|---|---|---|---|---|
|||        Drain                Sweep      |        Source                Sweep      |        Drain                Sweep      |        Source                Sweep      |
|        VS=DV                (ION)      |d|2.99E-05|-3.30E-05|7.49E-05|-7.42E-05|
|        VS=DV                (ION)      ||9.61E-12|1.49E-11|2.26E-11|2.64E-11|
|        VS=DV                (ION)      ||-2.99E-05|3.30E-05|-7.49E-05|7.42E-05|
|        VS=DV                (ION)      ||2.75E-10|2.46E-10|1.51E-10|1.98E-10|


![AbnormalGoxThickness  PolyGate  ActiveArea  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a3aef1ff-b4fe-4226-9831-b4b3fb2e1a15/a3aef1ff-b4fe-4226-9831-b4b3fb2e1a15.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=aec38790b90799ba8072b19d279de5e6da52aadf)
Fig. 17 TEM image of failed transistor.

## IV. C ONCLUSION 

Through the investigation on these two cases, we can  conclude that the poor Gox uniformity can result in lower I ON   and asymmetric behavior of transistor. According to the  formula of MOSFET threshold voltage   $\left({{\mathrm{V}}_{\mathrm{T}}}\right)$   and the formula of  capacitance, thicker Gox induces the MOSFET on-state current  drift by affecting the   $\mathrm{V_{T}},$  , which is partially dominated by  capacitance of MOS structure. In case study II, the drift of MOS  capacitance is significant enough for SEM PVC to detect the  difference. For small defect in case study I, if we employ  capacitance measurement after we observe the abnormal  current through static I-V test, we may detect this tiny  capacitance variation instead of performing junction stain

analysis.   Combining   capacitance   test   with   traditional  Nanoprobing static measurement could improve the success  rate of PFA.

## A CKNOWLEDGMENT 

Authors would like to thank UMC Failure Analysis  Department colleagues for their assistance on TEM and EELS  mapping result.

## R EFERENCES 

[1]    Chenming Calvin Hu,  Modern Semiconductor Device for Integrated  Circuits , pp. 157-165, 2010.     [2]    Hung-Sung Lin  et al., “ An Application of Nanoprobe Technique in the  Characterization of Advanced SRAM Devices”,  Proceedings of   $34^{t h}$    International Symposium for Testing and Failure Analysis (ISTFA) , pp.  417-422, 2008.     [3]    Hun-Seong Choi  et al ., “MOSFET implant failure analysis using  plane-view scanning capacitance microscopy coupled with nano-probing  and TCAD modelling”,  Proceedings of International Symposium on the  Physical and Failure Analysis on Integrated Circuit (IPFA),  pp. 5-8,  2014.    [4]    Stefan Doering  et al ., “Polycrystalline silicon gate originated CMOS  device failure invested by Scanning Spreading Resistance Microscopy”,  Microelectronic Engineering, Volume 142.  pp. 40-46, 1 July 2015    [5]    Cha-Ming Shen  et al ., “Combining the Nano-Probing Technique with  Mathematics to Model and Identify Non-Visual Failures”,  Proceedings of   $33^{t h}$    International Symposium for Testing and Failure Analysis (ISTFA),  pp. 214-218, 2007.     [6]    Rue. Rosenkranz, “Failure Localization with Active and Passive Voltage  Contrast in FIB and SEM”,  Microelectronics Failure Analysis Desk  Reference,   $6^{t h}$   Edition , pp. 269-278, 2011

