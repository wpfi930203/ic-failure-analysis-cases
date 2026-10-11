---
title: "198_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_c5153a3b8b69e693a2fcf75d9bdd83207295230462135641
file_size: 560833
---

## Defect Density Reduction of Thin SiO2 MOSFET  through Oxidation Pre-cleaning improvement – a Fast  Wafer Level Reliability Monitoring  

Kamaruddin M.H. 1 \*, Soin N. 2 , Veriven C. 1 , How C. M. 1 , Ang C. K. 1  1 Infineon Technologies (Kulim) Sdn. Bhd., Lot 10 & 11, Jalan Hi-Tech 7, Industrial Zone Phase II, Kulim Hi-Tech Park  Kulim, Kedah Darul Aman  09090, Malaysia.  2 Department of Electrical Engineering, University of Malaya, Kuala Lumpur, Malaysia.   \* Phone: +6044278726 Fax: +6044278441 \*Email:  mohdhanif.kamaruddin@infineon.com

Abstract-   We conducted experiment to reduce the level defect  density in 7.5nm thin SiO2 CMOS by improving the pre-cleaning  of silicon surface before gate oxidation. Fast wafer level reliability  monitoring is implemented using ramped voltage stress (RVS)  where from the breakdown Weibull chart, the inclination point of  intrinsic and extrinsic will give the measurement of defect density  (unit is number of defect per cm2). We measured high defect  density of  ${\tt>}20$   times the defect density target. Through systematic  problem solving methodology, root cause was found to be due to  ineffective cleaning method. With the additional SPM cleaning in  the gate oxidation pre-clean step, defect density reduced by almost   $\bf{95\%}$  . SPM chemistry reduces the surface roughness and also  improves contaminations removal on the wafer surface prior to  gate oxidation. Rougher interface of Si-SiO2 leads to early failure  and lower TDDB. Inline silicon surface roughness check is not  practical due to very small nature of embedded-type contaminants  a rough silicon surface creates. In order to increase detection  probability of micro-sized particles, a good reliability monitoring  strategy using special test structures is implemented.

Keywords  –  Integrated circuit reliability, CMOSFETs, Dielectric  breakdown

## I. I NTRODUCTION 

Different defect sizes in manufacturing process leads to  different outcomes: no impact, early life failures or yield  failures. It has been shown that product reliability is a function  of both yield and defect density, and reducing defect density  allows manufactures to meet the reliability target [1]. The  ramped voltage stress (RVS) is one of the fast wafer level  reliability (fWLR) time dependent dielectric breakdown  (TDDB) measurements that are used to monitor extrinsic  reliability performance in a given technology [2]. Bias voltage  is applied to gate in inversion mode until breakdown, where  source/drain and wells are connected to ground. RVS is  performed on dedicated SiO2 dielectric test structures and we  monitor the voltage to breakdown (Vbd), current to breakdown  (Ibd) and charge to breakdown (Qbd). The breakdown data is  plotted in a Weibull distribution, where we can identify the  intrinsic vs. extrinsic branches, as illustrated in Fig. 1. The  intersection point between intrinsic and extrinsic branches will  give us the maximum defect density, eDD, of the extrinsic,  determined by [3]

$$\begin{array}{r}{e D D=-\frac{\ln(1-F)}{A o x}}\end{array}$$
(1)

where Aox is the dielectric area and F the cumulative part of  failed devices.

![intersection  oQbdextractedfrom  points  CVSmeasurement  Qbdfrom   Intrinsic  Intrinsic RCSmeasurement  15  6   Extrinsic Extrinsic  8  109   10   10   10   10   10   101  Qbd（C/cm²     ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/36f8ce61-68d5-4e29-82ec-b2e462b1da94/36f8ce61-68d5-4e29-82ec-b2e462b1da94.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215648%3B1743219248&q-key-time=1743215648%3B1743219248&q-header-list=host&q-url-param-list=&q-signature=11cc5a225c2f315eca4f4db693dc73b9dd90b452)
Fig. 1 – Figure extracted from G. Diestel et al. illustrating the inclination point,  intrinsic and extrinsic branches [3].

fWLR monitoring can detect, minimize or eliminate  reliability fails of products due to processing problems after  process qualification [4]. These types of reliability fails cannot  be detected by the outgoing electrical functional tests.

For a specific automotive IC product, the fWLR extrinsic  monitoring is implemented. The monitoring strategy adopts the  methodology proposed by A. Martin and R.P. Vollertsen [4] to  give fast detection of process issue through in-line fWLR  measurements. Dielectric reliability control monitor (RCM) is  fabricated in the scribe line for every reticle shot and eDD  measurements are assessed to detect potential early dielectric  lifetime failure. Out of control action plan (OCAP) is triggered  in the event of processing problems. Root cause of the failure is  determined and corrective action is applied to eliminate it  permanently. This paper is written to illustrate the application  of fWLR dielectric monitoring and its use in detecting process  problems and verify the improvement plan.

(1)

The RCM structures are fabricated in the scribe line of  productive wafers and follows JEDEC JEP159 inter-level  structure of orthogonal comb-comb requirement. They are  planar NMOS and PMOS transistor arrays, with area of   $7.5~\mathrm{x}$     $10–4\;\mathrm{\;cm}2$   and   $7.5\mathrm{nm}$   gate oxide thickness. The RCMs are  stressed with RVS method. Both NMOS and PMOS are  stressed in inversion mode (positive gate bias for NMOS,  negative gate bias for PMOS). By referring to JEDEC  JESD35-A for  $7.5\,\mathrm{x}\,10–4\,\mathrm{cm}2$   oxide area, we would require 800  RCMs to prove the product meets the eDD target with   $95\%$    confidence level. However to increase the confidence level, we  monitored up to 15000 RCMs. The RCM are located in 22  reticle shots across productive wafers.

The fWLR measurements conform to JEDEC JEP159 and are  performed at room temperature. Table 1 summarizes the input  parameters of the RVS as per JEP159. Measurements are done  using standard TSK UF200 wafer prober.

Table 1 – The key RVS input parameters

|Parameter|umit|Comment|
|---|---|---|
|Vuse||Pre-RVS initial screening to remove initially|
|||        failed RCM. 3.3V for NMOs, -3.3V for                PMOS      |
||||
|Tuse||Oxide current at Vuse and must be > 1 x 10-13|
|Vstress|||
|||        Oxide stress voltage. The voltage starts at                Vuse, and ramps at predefined voltage, Vstep,                for duration Tstep until oxide breakdown.                During the Vstress ramp, the current is                monitored. Vstep=0.75V, Tstep=30ms      |
||||
||||
|Imeas||Measured oxide current at Vstress|
|vba|A|        Oxide breakdown voltage when Imeas > 10 x                Tuse      |
||||
|Vmax||        Maximum voltage of Vmax. In this                 experiment it is 14V      |


## III. R ESULTS AND DISCUSSION 

RVS fWLR is performed on more than 15,000 RCMs. From  the Weibull plot of Vbd for PMOS and NMOS RCM structure,  the intrinsic-extrinsic inclination point is determined and eDD  is calculated using Formula (1). The result is normalized to  show the factor of deviation of the measured eDD when  compared against target. The result is shown in Fig.2. The plot  indicates that based on intrinsic-extrinsic inclination point,  PMOS is 21 times larger and NMOS is 7 times larger than eDD  target. Clearly, the current process steps are not able to deliver  the required product reliability level needed.

![30  25   OPMOS  NMOS  20   AttargetDefectDensity  10   TS   20  VBD[V]  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/db342c64-ecf0-421e-a9cc-a636f1d70d09/db342c64-ecf0-421e-a9cc-a636f1d70d09.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215648%3B1743219248&q-key-time=1743215648%3B1743219248&q-header-list=host&q-url-param-list=&q-signature=bbadad17f2e90ac2d9b47b48b9e01c1b71c09b06)
Fig. 2 – Inclination of intrinsic vs extrinsic branch (marked with BLUE arrow)  is used to extract defect density and determined the factor of deviation from  defect density target. A factor of ZERO means the RCM meets the technology  eDD target

Root cause finding and corrective action to reduce the  measured eDD to be closer to eDD target is using  cause-and-effect analysis as per JEDEC JEP132 guidelines. A  graphical description of the various potential root causes that  could lead to the eDD violation is constructed in a form of  "fishbone diagram" or "Ishikawa diagram". Fig. 3 shows the  cause-and-effect diagram for this failure, where every potential  cause is being investigated to prove and disprove its relevance  to the failure.

![MACHINE  Particles being introduced.  during implant steps  Furnace particle  contaminates the gate  oxide during oxidation  High eDD (>5cm”)  Gate oxidation pre-   Lot process at   Too thick sacrificial  clean method   oxide leading to  endofRCA  chemical   oxide residue  lifetime   Negatively charged pn-junction  Overusing of   attractspositively charged  Plasma  RCA chemical   Gate oxidation pre-   plasma leading to rougher  induced  during gate   clean cross   substrate surface before gate  damage (PID)   oxidation pre-   contamination due   on the gate   oxidation  cleam   to mixing of all  Oxide  different  technologies  METHOD   MATERIAL  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/002e8c3d-ee7e-4a66-b513-e1d640f28be8/002e8c3d-ee7e-4a66-b513-e1d640f28be8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215648%3B1743219248&q-key-time=1743215648%3B1743219248&q-header-list=host&q-url-param-list=&q-signature=03195d4afb9d101f1c2b900e3c82c16c5879fb52)
Fig. 3 – 4M (Man, Method, Machine, Material) approach in identifying the root  cause of high eDD.

All 9 hypotheses are tested and we narrowed them down to  the gate oxidation pre-clean method. VBD results as per Fig.2  shows that PMOS has higher extrinsic or early breakdown than  NMOS, and PMOS is stressed under negative voltage. This  indicates that a potential structural transition layer (STL) near  Si/SiO2 interface contributes to faster and easier breakdown of  gate oxide [7]. We hypothesize that insufficiently cleaned  silicon leads rough silicon surface and surface roughness  increases the level of STL. Pre-clean or surface treatment  before gate oxidation adopts the commonly used dilute

hydrofluoric acid (DHF) to remove sacrificial oxide followed  by RCA. RCA consists of standard clean one (SC1:  NH4OH/H2O2/H2O)   and   standard   clean   two   (SC2:  HCl/H2O2/H2O) [6]. The cleaning steps chemistry with  de-ionized (DI) water rinsing is summarized in Table 2.

Table 2 – The gate oxidation pre-clean steps

|Step|Chemical|Duration (sec)|
|---|---|---|
|1|DHF|330|
|2|DI water rinse|Quick dump|
|3|SC1|150|
|4|DI water rinse|Quick dump|
|5|SC2|150|
|6|DI water rinse|Quick dump|


Wenyu, Zhongli and Zhijing have proven that DHF has  roughening effect on the silicon surface and adding a sulfuric  acid (H2SO4) and hydrogen peroxide (H202) mixture (SPM)  after DHF suppresses pitting effect that occurs during  oxidation, removes metallic contaminants and smoothens wafer  surface [8]. A 420 seconds SPM cleaning step followed by  quick dump DI water rinse is added after Step 2. We compared  the silicon surface roughness between DHF  $_{\mathrm{">SC1->SC2}}$   and  DHF-  $\cdot>$     $_{\mathrm{PM-SC1-SC2}}$   cleaning schemes using Atomic  Force Microscopy (AFM). Based on arithmetic average, Ra, of  the absolute values of the surface height deviations measured  from the mean plane,   $12.4\%$   surface roughness reduction is  observed in the sample with SPM step. Fig. 4 and Table 3  illustrate the AFM results. DHF has high etch rate but this does  not lead to effectively removing non-metallic contaminants:  adding SPM clean increases efficiency in removing particle due  to its strong oxidizing force [9]. The tested wafers are processed  in SC2 with very low contamination level and it has been  proven that <1ppb metallic contaminants inside SC2, whether  they are from the chemical supplier or processed wafers, have  no severe effects on product reliability performance [10]. Thus,  metallic contamination is ruled out as root cause.

![2.0nm  -2.0nm  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2795e710-9461-43bc-935b-9011e08fa40b/2795e710-9461-43bc-935b-9011e08fa40b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215648%3B1743219248&q-key-time=1743215648%3B1743219248&q-header-list=host&q-url-param-list=&q-signature=9865ddb991f0cff71763eeb4f475afa49afc4d95)
Fig. 4 – AFM measurement output on one sample

Table 3 – Average surface height from mean flat plane,  Ra

|Sample|Description|Ra (nm)|
|---|---|---|
|1|DHF- SC1 - SC2|0.185|
|2|DHF - SPM - SC1 - SC2|0.162|


The implementation of the new SPM cleaning step is  monitored for 2 months via fWLR RVS and sample size of  more than 20,000 RCMs are obtained. As shown in Fig. 5, after  process improvement (additional SPM cleaning step), eDD is  now reduced. We measured the new eDD: PMOS is at a factor  of 0.07 and NMOS at 0.17 when compared to eDD target. By  comparing with the factor value of eDD before process  improvement, we have reduced the PMOS defect density by  almost   $95\%$   and NMOS by almost   $85\%$  .

![30  PMosbeforeimprovement  25   PMOS afterimprovement  口NMoSbeforeimprovement  20   NMoSafterimrovement  At targetDefectDensity  1O  ey  1O   15   20  VBD[V]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a4d5ea9f-7a8b-4ea4-bb69-59df3709a5af/a4d5ea9f-7a8b-4ea4-bb69-59df3709a5af.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215648%3B1743219248&q-key-time=1743215648%3B1743219248&q-header-list=host&q-url-param-list=&q-signature=71f2ae375334a69df74405afbf36ddbb2dff8645)
Fig. 5 – The addition of SPM cleaning step improved the eDD performance  (NMOS’, PMOS’): the measured eDD of NMOS and PMOS after the  improvement showed the level of defect density is at target values.

Fig. 7 Output characteristics of IGZO TFT with  $L_{G D O}=0.3~\upmu\mathrm{m}$   with   $V_{D}\,{=}50~\mathrm{V}$  .

Our observation of reduced defect density with reduced  silicon surface roughness also correlates with Park et. al. where  they have successfully prove the reduction of defect density  with reduced roughness of Si-SiO2 interface [11]. They have  also shown increased of Qbd in smoother surface and this also  indicates increase of time-dependent-dielectric-breakdown  TDDB [12]. It is evident from this work that a good reliability  monitoring system has to be established to uncover critical  reliability issues from insufficient wafer processing, as  outgoing functional and PCM tests alone cannot detect them.  Inline silicon surface roughness checking after wet cleaning  step is difficult and not economical in mass production mode:  the best case is to eliminate the source of failure by systematic  wet cleaning process improvement [13]. High surface  roughness can also lead to very small contaminants of  embedded-type that cannot be detected by state-of-the-art  dark-field and bright field inspection tools but we have shown  that good reliability test sampling strategy increases problem  detection probability. However detection of problem alone is

not beneficial, unless failure mechanism can be understood to  enable effective corrective action implementation.

## IV. C ONCLUSION 

We have successfully applied the fast wafer level   monitoring  (fWLR) concept. The used of   Ramped Voltage Stress (RVS) on  the Reliability Control Monitor (RCM) structures in the scribe  line of productive wafers enable us to detect problems in the  pre-clean   before   gate   oxidation.   Through  out-of-control-action-plan   (OCAP)   and   cause-and-effect  analysis, the root cause of deviation is detected and eliminated.

[13]    R. Van Roijen, D. F. Hilscher, C. Meagher, R. Rettmann and D.  McKindles, Optimizing Wet Clean operations in an established  manufacturing environment,  2016 27th Annual SEMI Advanced  Semiconductor Manufacturing Conference (ASMC), Saratoga Springs,  NY, 2016, pp. 367-370.

## A CKNOWLEDGMENT 

The authors would like to thank all the anonymous reviewers  for their time invested, valuable comments and suggestions to  improve the technical content of this paper.

## R EFERENCES 

[1]    J. Siddiqui, J. Ortega and B. Albus, On the relationship between  semiconductor manufacturing volume, yield, and reliability,  2017 IEEE  International Reliability Physics Symposium (IRPS), Monterey, CA,  2017, pp. SR-1.1-SR-1.5.    [2]    A. Martin, Reliability of gate dielectrics and metal–insulator–metal  capacitors,  Microelectronics Reliability,   Volume 45, Issues 5–6,   2005,   p.834-840 .    [3]    A. Martin, Special Interest Group (Sig): Fast Wafer Level Reliability  (Fwlr) Monitoring,  2007 IEEE International Integrated Reliability  Workshop Final Report, 2007, p. 159 - 160     [4]    G. Diestel  et al. , Quality assessment of thin oxides using constant and  ramped stress measurements,  Microelectronics Reliability,   Volume 41,  Issue 7,   2001,   p.1019-102.     [5]    A. Martin, R. P. Vollertsen, An introduction to fast wafer level reliability  monitoring for integrated circuit mass production,  Microelectronics  Reliability,   Volume 44, Issue 8,   2004,   p.1209-1231 .    [6]    B. Pathangey, L. D. McCarthy, D. C. Skilbred, Effect of Metal  Contaminants in Pre-Gate Oxide Cleans for Sub-100-nm Devices,  IEEE  TRANSACTIONS ON DEVICE AND MATERIALS RELIABILITY, VOL.  5, NO. 4, DECEMBER 2005     [7]    S. Wu, X. He, Y. Liu, G. Chen, Polarity dependent of gate oxide  breakdown from measurements,   2013 IEEE 10th International  Conference on ASIC, Shenzhen, 2013, pp. 1-2.     [8]    G. Wenyu, L. Zhongli, H. Zhijing, "Dependence of ultra-thin gate oxide  reliability on surface cleaning approach,"  1998 5th International  Conference on Solid-State and Integrated Circuit Technology.  Proceedings (Cat. No.98EX105), Beijing, China, 1998, pp. 291-294.     [9]    Mitsushi Itano et al., Particle Removal from Silicon Wafer Surface in  Wet Cleaning Process,   IEEE Transactions On Semiconductor  Manufacturing. Vol 6. No 3. August 1993     [10]    K. H. R. Tan, P. L. E. Liew, C. C. Chin and C. Y. J. Wong, A study on  device robustness with integrated effects from low parts-per-billion level  of metallic elements in wafer cleaning process chemicals,  2016 IEEE  23rd International Symposium on the Physical and Failure Analysis of  Integrated Circuits (IPFA), Singapore, 2016, pp. 256-261.     [11]    H. Park et al., Impact of SiO2/Si interface micro-roughness on SILC  distribution and dielectric breakdown: A comparative study with  atomically flattened devices,  2017 IEEE International Reliability  Physics Symposium (IRPS), Monterey, CA, 2017, pp. DG-7.1-DG-7.5.    [12]    E. Mullen, C. Leveugle, J. Molyneaux, J. Prendergast and J. S. Suehle,  Relationship between TDDB testing and wafer level ramped QBD  testing using both fixed current and current density stressing,  2001 IEEE  International Integrated Reliability Workshop. Final Report (Cat.  No.01TH8580), Lake Tahoe, CA, USA, 2001, pp. 74-77.

