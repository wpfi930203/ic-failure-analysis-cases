---
title: "264_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_52f20cc0bb85d0ec8f84d0f4b7ee370f7295230462135641
file_size: 1068172
---

## Study of Internal Latchup Behaviors in Advanced  Bulk FinFET Technology   

Wei Liang\*, Robert Gauthier Jr., Souvick Mitra, You Li, Chen Yan  GlobalFoundries, 1000 River St., Essex Junction, VT, USA 05452  \* Phone: +1-802-769-9220, Fax: +1-802-769-9659, \*Email: wei.liang@globalfoundries.com

Abstract-   In this paper, Internal Latchup (ILU) behaviors are  studied in an advanced bulk FinFET technology. The  methodology of the ILU development and characterization are  introduced and the ILU characteristics of thin oxide (SG) and  thick oxide (EG) victim devices are discussed comprehensively.  Comparison between 7nm and 14nm Bulk FinFET technology has  been made on ILU characteristics.

Keywords  –  Internal Latchup, External Latchup, Overshoot,  Undershoot, SCR, FinFET .

## I. I NTRODUCTION 

Latchup in bulk CMOS technology stems from PNPN  structures formed by the base-collector coupled parasitic NPN  and PNP bipolar transistors. The placement of NFETs, NCAPs  or NWells at different potentials, and PFETs, PCAPs or PWells  in close proximity will result in the parasitic SCR or thyristor  structure. Fig. 1 shows the parasitic SCR structure in a CMOS  inverter. To simply the illustration, the fins are not shown.  When Latchup occurs, a low resistance path is formed between  supply voltage (Vdd) and ground (GND), and a significant  amount of current can be drawn through this parasitic SCR,  leading to the chip destruction.

![input  Input Output  Output Gnd  Gnd  V VDD  DD p+  STI  n+  NFET  NFET  +  n+  STI  p+  p+  PFET  PFET  p+  STI  n+ NPN  NPN R RP  PV  RPH  R  RN2  R  RNH  R NH  RN  R NV PH N2 PNP  PNP Rpw=Rph+Rpv  R  =R  +R  R RP2  P2  Rnw=RNh+Rnv  R NW =R NH +R NV PW  PH  PV P-vvell  P-Well  N-vell  N-Well ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c963f0bc-2ed1-47ef-aeb8-59b30fcf4d8a/c963f0bc-2ed1-47ef-aeb8-59b30fcf4d8a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215676%3B1743219276&q-key-time=1743215676%3B1743219276&q-header-list=host&q-url-param-list=&q-signature=0863bcfe3ff2fe5f02b8234d6c4808979e8e71c6)
Fig. 1. Parasitic SCR in a CMOS inverter.

Latchup issues are primarily classified into two main  categories, Internal Latchup (ILU) and External Latchup  (ELU). In ILU, internal circuits creating supply bounce,  on-chip transmission line reflections or on-chip generation of  carriers which can trigger parasitic SCRs formed in bulk  CMOS. In ELU, the parasitic SCRs are triggered by the  off-chip signals received by I/O circuits. These signals create  large voltage bounce or carrier injection that can trigger latchup  either within an I/O or in the weakest internal circuits adjacent  to I/O cells if these carriers are not contained within I/O.

Bulk FinFET technologies in development have scaled from  20nm down to 7nm node as of today. Based on the fact that the  low power requirement of the applications, the Vdd of the  internal core block has been reduced to below 1.0V as CMOS

technology scales. In applications with   $\mathrm{Vdd}{<}1.0\mathrm{V}$  , as holding  voltage (Vh)>Vdd, there is no sustained Latchup, thus minimal  Latchup risk in either ILU or ELU. However, there are  applications that the core circuit will be operating in overdrive  mode where   $\mathrm{Vdd}{>}1.0\mathrm{V}$   occurs. In this condition, there can be  sustained Latchup if the overdrive Vdd value is greater than Vh  and the ELU ground rules/prevention guidelines need to be  considered. Designers need to follow proper guideline in design  to make the ELU risk minimal. In 1.8V I/O blocks, the Vh is  always smaller than Vdd, so ELU risk is a concern all the time.

The general Latchup risk assessment in FinFET technology is  discussed in [1] [2] [3] and DNW-induced Latchup risk was  discussed in [4]. In this paper, a detailed study of ILU with  comprehensive dataset interpreting Latchup characteristics in  core circuit and I/O block in 7nm and 14nm bulk FinFET  technology is presented. In our study, the characteristics of ILU  of thin oxide (SG) and thick oxide (EG) victim devices are  studied. SG devices refer to the core circuit and EG devices  refer to the perimeter I/O blocks.  A brief introduction of  Latchup test structure and testing methodology is presented  first, and then the ILU characteristics and risks in SG and EG  devices under different supply voltage conditions are discussed.

## II.   T EST  S TRUCTURE AND  T EST  M ETHODOLOGY 

Fig. 2 shows the cross section and schematic of the ILU test  structure. The simplified 4-terminal SG and EG SCR are used  in ILU development to capture dominant features of victim  devices. Three key aspects including   $\mathrm{P}+$   (Anode) and   $\Nu+$  (Cathode) diffusion spacing (SAC), NW and PW tap length  (Ltap) which results in the lateral resistance, and NW and PW  contact area which results in the vertical resistance.

Overshoot (OS) and Undershoot (US) tests are usually  conducted in ILU characterization. Fig. 3 shows the test  configuration of OS and US. In the data processing, two key  parameters can be obtained from OS and US data, the Latchup  triggering voltage (Vt) and holding voltage (Vh). To assess the  Internal Latchup triggering and sustaining condition, Vmargin  and Vsustain will be used based on simple processing of Vt and  Vh, respectively.

NTERNAL  L ATCHUP  C HARACTERISTICS AND  D

SG devices represents the core circuit block in Latchup  development. We have symmetric NW/PW Ltap and the SAC  variation in our design of experiments (DoE). The normal  supply voltage in advanced bulk FinFET technology is below  1.0V which is smaller than the Vh of the SG device. Vh can be  obtained in ILU characteristics. Fig. 4 shows the   $25\mathrm{^\circC}$  and

$125^{\circ}\mathrm{C}$   SG ILU characteristics with Ltap variation under   $\mathrm{Vdd}{=}0.9\mathrm{V}$  . The   $25\mathrm{^\circC}$   and   $125^{\circ}\mathrm{C}$   SG ILU characteristics with  SAC variation under   $\mathrm{Vdd}{=}0.9\mathrm{V}$   are shown in Fig. 5. As an  explanation, Vsustain=Vh-Vdd which is used to assess the  Latchup sustaining condition.

![V DD Gnd  V DD p+  STI  n+  STI  p+  STI  n+  R NW p NPN R P  PV  RPH  R PH  RN2  R  R RNH  NH  R NV  n  PNP N2 NPN  p PNP R Rpw=RpH+Rpv  =R +R  R P2  RNw=RNh+Rnv  R NW =R NH +R NV  n PW  PH  PV R P-Well P-vvell   N-well  N-Well  PW Gnd ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bc966a42-ec6d-4db3-a441-e73587196a97/bc966a42-ec6d-4db3-a441-e73587196a97.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215676%3B1743219276&q-key-time=1743215676%3B1743219276&q-header-list=host&q-url-param-list=&q-signature=aee2b51455461d09ae42943f5e8f8d8408c1c9b3)
Fig. 2. 4-terminal Internal Latchup structure.

![Overshoot  Undershoct  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/02ca902b-d122-4ce3-bf32-945a6376776e/02ca902b-d122-4ce3-bf32-945a6376776e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215676%3B1743219276&q-key-time=1743215676%3B1743219276&q-header-list=host&q-url-param-list=&q-signature=0acf6e40f4ed0f431916e843fba2ef620b685a5b)
Fig. 3. Overshoot and Undershoot ILU characterization.

We can observe from Fig. 4 that when   $\mathrm{Vdd}{=}0.9\mathrm{V}$  , though  Vsustain decreases with higher temperature, the Vsustain>0 up  to Ltap=30um which means there is no sustained Latchup under  both temperatures. Therefore, ELU is not concerned in such  supply voltage condition. It is clearly shown in Fig. 5 that under  both temperatures, Vsustain>0 at the technology allowed  minimum SAC for SG which is   $60\mathrm{nm}$  , and Vsustain increases  with larger SAC so there is also no ELU risk.

![Oxide=SGVdd=0.9VSAC=60nmTest=Overshoot 0.45 0_40 250 125C 0.35 0.30 0.25 20.20 0.15 0_10 0.05 0.00 15  20  26  30 WellTapLength (um)   ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5af07cd9-455d-497c-835b-cc016d3bfe07/5af07cd9-455d-497c-835b-cc016d3bfe07.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215676%3B1743219276&q-key-time=1743215676%3B1743219276&q-header-list=host&q-url-param-list=&q-signature=45eea2c3a11f5b96c2a8f08a0a4447de7d85d51c)
Fig. 4.   $25\mathrm{^\circC}$   and  $125^{\circ}\mathrm{C}$   SG ILU characteristics with Ltap variation under  Vdd=0.9V.

![Oxide=SGVdd=0.9VLtap=25umTest=Overshoot  1.4-  25C  12  125C  1-0  0.6  D.4  D-O  1O  Anode To Cathode Spacing (um)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d5f6b214-7718-4b56-b6f8-52567ec8448c/d5f6b214-7718-4b56-b6f8-52567ec8448c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215676%3B1743219276&q-key-time=1743215676%3B1743219276&q-header-list=host&q-url-param-list=&q-signature=73e70f19737fd5a9c77340ae1d887cb5c8566729)
Fig.  $5.\,25^{\circ}\mathrm{C}$  and   $125^{\circ}\mathrm{C}$   SG ILU characteristics with SAC variation under  Vdd=0.9V.

However, if the SG device is under Vdd overdrive conditions,  there will potentially be an ELU risk if the overdrive supply  voltage exceeds Vh. Fig. 6 shows the  $25^{\circ}\mathrm{C}$   and   $125^{\circ}\mathrm{C}$   SG ILU  characteristics with Ltap variation under   $\mathrm{Vdd}{=}1.35\mathrm{V}$   which is  one possible boost voltage used in micro-processors. It is clear  in Fig. 6, Vsustain  ${\mathrm{<}}0\mathrm{V}$  which means under the overdrive  condition, once ELU event happens, the Latchup condition can  be sustained and will not go away until the power supply is  recycled, this can lead to chip destruction. Higher temperature  leads to a further decreasing in Vsustain. Fig. 7 shows the   $25^{\circ}\mathrm{C}$  and   $125^{\circ}\mathrm{C}$  SG ILU characteristics with SAC variation under   $\mathrm{Vdd}{=}1.35\mathrm{V}$  . We can observe from Fig. 7 that under both  temperatures, Vsustain<0 at technology allowed minimum  SAC but Vsustain will increase with larger SAC. However,  with technology allowed minimum SAC, the design will still  have ELU risk due to the sustained Latchup. Proper guidelines  must exist for designers to follow to make the ELU risk  minimal [5].

![Oxide=SGVdd=1.35V SAC=60nmTest=Overshoot  0.00-  -0.05   25C  125C  -0.10  0.15  0.20  0.25  0.30  -0.35  -0.40  1O   15   20   25  Well Tap Length (um)     ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c147a85c-9c83-49d6-a38f-4b8dca0ea91b/c147a85c-9c83-49d6-a38f-4b8dca0ea91b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215676%3B1743219276&q-key-time=1743215676%3B1743219276&q-header-list=host&q-url-param-list=&q-signature=a71f8630d6ce14eaed0176bac6adc2b136fde80d)
Fig.   $6.25^{\circ}\mathrm{C}$   and   $125^{\circ}\mathrm{C}$   SG ILU characteristics with Ltap variation under  Vdd=1.35V.

For EG devices, we have the same Latchup development  methodology. EG devices represents the I/O cell and  pre-drive/driver/receiver area in chip where hotzone goes up to.  As the operating voltage can be up to 1.8V or higher, in EG  devices, there will always be the risk of sustained Latchup

$\scriptstyle(\mathrm{Vh<Vdd})$  . Fig. 8 shows the   $25\mathrm{^\circC}$   and   $125^{\circ}\mathrm{C}$   EG ILU  characteristics with Ltap variation under  $\mathrm{Vdd}{=}1.98\mathrm{V}.$  . The   $25\mathrm{^\circC}$  and   $125^{\circ}\mathrm{C}$   EG ILU characteristics with SAC variation under   $\mathrm{Vdd}{=}1.98\mathrm{V}$   are shown in Fig. 9. It is clearly shown that the  Vsustain<0 under both temperatures with Ltap and SAC  variations so there is always a sustained Latchup risk where  prevention guidelines are needed to eliminate the ELU risks.

![Oxide=SGVdd=1.35VLtap=25umTest=Overshoot  0.8  25C  125C  0.6  0.4  ue  D2  Sns  0_0  -D.2  -0_4  0_1  Anode To Cathode Spacing (um)     ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/974ffca2-8e98-40c1-b135-9de8a4056845/974ffca2-8e98-40c1-b135-9de8a4056845.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215676%3B1743219276&q-key-time=1743215676%3B1743219276&q-header-list=host&q-url-param-list=&q-signature=a271f30edd30b1132b10894110f6383e848fbecc)
Fig.  $7.\,25^{\circ}\mathrm{C}$   and   $125^{\circ}\mathrm{C}$   SG ILU characteristics with SAC variation under  Vdd=1.35V.

![Oxide=EGVdd=1.98VSAC=0.42umTest=Overshoot  -0.4  25C  -0.5  125C  -0.6  -0_7  Ms  -0_8  -0.9  15   20   25   30  Well Tap Length (um)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/567c270a-3419-4ce8-ae08-f70176af0065/567c270a-3419-4ce8-ae08-f70176af0065.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215676%3B1743219276&q-key-time=1743215676%3B1743219276&q-header-list=host&q-url-param-list=&q-signature=de6d9a9b5189f656822b82105d91b11eb94ec5b9)
Fig.  $8.25^{\circ}\mathrm{C}$   and   $125^{\circ}\mathrm{C}$   EG ILU characteristics with Ltap variation under  Vdd=1.98V.

![Oxide=EGVdd=1.98VLtap=25umTest=Overshoot  0.0-  25C  125C  -0.2  ss  -0_4  -0.6  -0.8  -1.0  0.1   10  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c4a89fab-b8dc-49d7-9d77-ca279b1a61de/c4a89fab-b8dc-49d7-9d77-ca279b1a61de.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215676%3B1743219276&q-key-time=1743215676%3B1743219276&q-header-list=host&q-url-param-list=&q-signature=624db0d391b5441aa51cddcb687f15c23c920cc0)
Fig.  $9,25^{\circ}\mathrm{C}$   and   $125^{\circ}\mathrm{C}$   EG ILU characteristics with SAC variation under  Vdd=1.98V.

Comparing with 14nm node, though 7nm Bulk FinFET  technology has a similar Vdd below 1.0V, the difference in key  Latchup aspects can make the Latchup prevention strategy  different. Fig. 10 show the   $25^{\circ}\mathrm{C} $  and   $125^{\circ}\mathrm{C}$   SG ILU  characteristics   with   Ltap   variation   under    $\mathrm{Vdd}{=}1.35\mathrm{V}$  comparing 7nm and 14nm technology, respectively. Similar  comparison is also made under   $\mathrm{Vdd}{=}1.98\mathrm{V}$   for EG ILU  characteristics which is shown in Fig. 11. It is clear that the  Vsustain in 14nm technology is up to 0.6V higher than 7nm  technology, which means 14nm technology is more resistant to  sustained Latchup and therefore less ELU risks under overdrive  condition which higher than normal Vdd. Therefore proper  guideline to eliminate ELU risks is especially important in 7nm  Bulk FinFET technology.

![Oxide=SGVdd=1.35VSAC=TechMinTest=Overshoot  0.6   14nm(Temp=25C/SAC=96nm)  7nm (Temp=25C/SAC=60nm)  14nm(Temp=125C/SAC=96nm)  0.4   7nm(Temp=125C/SAC=60nm)  D.2  0.0  -0.2  -0.4  10   15   20   25   30  Well Tap Length (um)     ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/567141b1-72f7-42e1-ae87-a434f87f997a/567141b1-72f7-42e1-ae87-a434f87f997a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215676%3B1743219276&q-key-time=1743215676%3B1743219276&q-header-list=host&q-url-param-list=&q-signature=1693a253151a5f61f27d6b93d39e69922b216c51)
Fig.   $10.25^{\circ}\mathrm{C}$   and   $125^{\circ}\mathrm{C}$   SG ILU characteristics with Ltap variation under  Vdd=1.35V.

![Oxide=EGVdd=1.98VSAC=0.42umTest=Overshoot 0.2 14nm(Temp=25C) 0_0：  -7nm(Temp=25C) 14nm (Temp=125C) 7nm (Temp=125C) -0.2 -0.4 ss -0.6 -0.8 -1.0 10  15  20  25  30 Well Tap Length (um) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ea3b5c7b-936d-426c-83bf-64b9f511d2b8/ea3b5c7b-936d-426c-83bf-64b9f511d2b8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215676%3B1743219276&q-key-time=1743215676%3B1743219276&q-header-list=host&q-url-param-list=&q-signature=c0d65f10aa58631c520792aeb8d2d615d453bcc7)
Fig. 11.  $25\mathrm{^\circC}$   and   $125^{\circ}\mathrm{C}$   EG ILU characteristics with Ltap variation under  Vdd=1.98V.

## IV. C ONCLUSION 

In this paper, ILU characteristics was studied in 7nm and  14nm bulk FinFET technology. SG victim devices have two  design scenarios   $\mathrm{Vh{>}V d d}$   and Vh<Vdd) for ELU based on  different supply voltage, however, ELU always applies to EG  devices because of the sustained Latchup risk (Vh<Vdd).   The

ILU characteristics and discussion on Latchup risk assessment  shown in this paper will help designers in FinFET technologies  to have a better insight on how they decide on design trade-offs  in different chip scheme and also serve as a good reference for  future Latchup development in academic and industry research.

## R EFERENCES 

[1]    C. T. Dai et al., "Latchup in bulk FinFET technology," 2017 IEEE  International Reliability Physics Symposium (IRPS), Monterey, CA,  2017, pp. EL-1.1-EL-1.3.    [2]    K. Domanski, "Latch-up in FinFET technologies," 2018 IEEE  International Reliability Physics Symposium (IRPS), Burlingame, CA,  2018, pp. 2C.4-1-2C.4-5.    [3]    A. Kripanidhi and E. Rosenbaum, "Layout sensitivities of transient  external latchup," 2012 IEEE International Reliability Physics  Symposium (IRPS), Anaheim, CA, 2012.    [4]    C. Y. Huang et al., "Deep N-well induced latch-up challenges in bulk  FinFET technology," 2017 39th Electrical Overstress/Electrostatic  Discharge Symposium (EOS/ESD), Tucson, AZ, 2017, pp. 1-8.    [5]    K. Chatty, P. Cottrell, R. Gauthier, M. Muhammdad, “Method and  structure to suppress external latch-up”, US20050085028A1, 2005.

