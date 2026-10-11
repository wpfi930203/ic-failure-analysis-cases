---
title: "207_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_404ed006da976a7bcb9203a274c4dc6b7295230462135641
file_size: 839527
---

## GaAs pHEMT Single Pole Double Throw(SPDT)  RF Switch Failure Analysis  

Lin Shi 1 , Qiang Li 1 , Hongsheng Dai 1 , Zhida Wang 1 , Huanqiang Jing 1   1 ZTE Corporation, No.55,Hi-tech Road South, Nanshan District, Shenzhen, 518057, China  \* Phone: +86 0755-26777522   Email: shi.lin52@zte.com.cn

Abstract-   SPDT radio frequency (RF) switch which fabricated in  GaAs pHMET technology  was field return. Failure analysis was  performed on the typical sample. Some failed units can recover   after baking in high temperature chamber, which seemed to be  fake failure. During non destructive analysis such as X-ray &  C-SAM, no abnormality was found. After decapsulation, die  surface was clean and integrated. Through OBIRCH test, hot spot  was detected on the surface of a Metal-insulator-Metal (MIM)  capacitor. Then FIB cut was implemented on the spot, cross  section SEM image shown insufficient passivation coverage and  dielectric crack  in the MIM cap. According to the failure  phenomenon and pHEMT technology structure, the failure  mechanism was discussed. In the end of the paper, design based  corrective action and reliability test were recommended to  improve product reliability.

Keywords  –  GaAs pHMET, SPDT switch, Failure Analysis,  MIM cap, Fab defect

## I. I NTRODUCTION 

Mobile communication systems has developed rapidly in  recent years. The    3 rd  & 4 th  generation communication is now all  around us and will out of stage soon, 5G has already come.  Although the carried frequency, base band bandwidth are  increasing, the structure of RF front end  in Radio Remote  Unit(RRU) will not change in short time. RF switch was one of  the key components widely employed to build the transceiver  chain. RF switch has many applications such as VSW detection,  DPD alignment and Tx to Rx chain switching in TDD system.  This paper studied a field  SPDT switch failure case, the switch  was fabricated in GaAs pHMET technology. Background  investigation shown that the failed units had already worked for  several months, and  higher humidity areas get higher failure  rate. After baking the failed samples in the chamber(125,  24hrs or longer), some of them can recover its function. Pressure  cook test can re-occur the failure phenomenon. Non-destructive  analysis found no obvious abnormality. After decapsulation, still  no failure signs was detected. Then  the samples were sent to  IR-OBIRCH (Infra Red Optical Beam Induced Resistance  Change) analysis, hot spot was found on the surface of MIM cap.  After FIB cut on the hot spot SEM image shown insufficient  passivation coat and dielectric crack  in the MIM cap.

right power. In Mode B RFIN is connect to RF2, downlink  route send signal to the digital system to confirm whether  the  antenna receive accurate signal power.

![ANT  RFIN   RF1  RV  IRF2  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/67b787a4-34a2-4f18-88de-6705ac7b68ee/67b787a4-34a2-4f18-88de-6705ac7b68ee.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215656%3B1743219256&q-key-time=1743215656%3B1743219256&q-header-list=host&q-url-param-list=&q-signature=503c26bb76aa643cc41e5098f46a2a641d70491e)
Fig. 1 SPDT Switch’s  Typical Application

Channel isolation, switching time & maximum power limit  are the key characteristics of RF switch, switch based on GaAs  technology can greatly meet the requirement. Function block of  the RF switch was shown in Fig.2. The main structure is  series-parallel, which offers a high isolation symmetric  topology, it has excellent linearity and power handling  capability. The design is non-reflective, RF ports 1 and 2 are  terminated to 50ohm resistor in the off-state.The failed switch  works from 5MHz to 6GHz, affords 60dB isolation and 1dB  insert loss at 3GHz, and is also1.8V logic compatible. It should  be noted that capacitor based on GaAs is MIM)structure, the  switch was packaged in QFN.

![C  RF2  WCTL   11   GNC  RFIN   RNC  RFI  E   C  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/706b8cbd-5f3f-429e-9bb8-622bad7e23a0/706b8cbd-5f3f-429e-9bb8-622bad7e23a0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215656%3B1743219256&q-key-time=1743215656%3B1743219256&q-header-list=host&q-url-param-list=&q-signature=131958cf6971decf8e93e04aa16980d0267bc068)
Fig. 2  Functional Block Diagram  III. F AILURE ANALYSIS

## II.   RF  SWITCH APPLICAITON 

As discussed above, SPDT switch’s fuction varies according  to RRU requirement, and the specific application  in this  paper  is shown in Fig.1. In mode A RFIN is connected to RF1, uplink    route feedback power to the system by microstrip line coupling   way, in order to ensure the power amplifier(PA) block output

After the failure samples returned from outside filed,   background investigation was taken, the results indicated that  the returned parts had already worked for one and a half year,  with higher failure rate in higher humidity area. According to  those switches’ working time, it is representative early failure.

Then the failed units were analyzed with physics methods from  nondestructive to destructive flow.Visual inspection result  excluded mechanical damage and contamination. Typical IV  curve confirmed RF pin shorted to GND, which should be PN  junction characteristic. During failure verification, some of the  failed units recover its IV  characteristics after baking in   $125\,^{\circ}\mathrm{C}$  oven and even passed function test, this phenomenon can be  called fake failure. Typical IV cure contrast was shown in Fig 3.  It should be noted that not all the failed units can  recover.

![Tektronix 370B   2019/02/21 12: 14  VERT>DIV  5mA  CURSOR  (f:1/grad.)  HORIZ/DIV  NG unit   NG uhit   5  CURSOR  (f:intercept)  PER STEP  200mA  OFFSET  GmA  Normal unit  Normal unit   BOR gm/DIV  25m  COLLECTOR  EAK  VOETS  100.0  AUX SUPPLY  0.00V  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d14df7d1-72f8-45e1-b2a4-7195d95e51ca/d14df7d1-72f8-45e1-b2a4-7195d95e51ca.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215656%3B1743219256&q-key-time=1743215656%3B1743219256&q-header-list=host&q-url-param-list=&q-signature=0b4f8ac71f44151b41fb115d2965b41614323474)
Fig. 3 Representative failure IV curve

Then X-ray inspection was executed, all the units were in  good wire bonding condition, no void or matter in the package  (Fig4). The C-SAM result didn’t shown any interface  delamination between lead frame and molding compound or die  and lead frame. So wet acid decapsulation was taken, no  obvious abnormalities was found on the die surface by internal  visual inspection.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7968243b-0c27-4a6a-8e75-dc5a1904cda6/7968243b-0c27-4a6a-8e75-dc5a1904cda6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215656%3B1743219256&q-key-time=1743215656%3B1743219256&q-header-list=host&q-url-param-list=&q-signature=12a78d9b42be03e31fe7e8d937517b6149a9e379)
Fig. 4  Typical X-ray image of failure units

Advanced OBRICH method was employed, while added a  tiny current between the  IV failed pin and GND, hot spot (Fig.  5) was detected at the edge of MIM cap. In order to confirm the  failure morphology, FIB cut was applied to the spot. At the  beginning MIM structure was normal, when it came to the  middle of hot spot, cross section under SEM indicated  insufficient passivation coating and dielectric crack (Fig. 6). By  now, the physical analysis  was done.

![Hot Spot Hot Spot    FIB direction  B dir  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7a84ad0f-1cda-44f8-bd46-fd51976bc079/7a84ad0f-1cda-44f8-bd46-fd51976bc079.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215656%3B1743219256&q-key-time=1743215656%3B1743219256&q-header-list=host&q-url-param-list=&q-signature=a1962b316b795297a06107be2904ed244bb9053a)
Fig. 5 Typical IR-OBIRCH Image of the Failure Sample

![Top Plate  Top Plate   Bottom plate Bottom plate  (a) Normal structure at the beginning  (a)  Normal structure at the beginning   Top passivation layer Top passivation layer    Insufficient Passivation  Insufficient Passivation  cover at the profile  cover at the profile   Dielectric Crack  Dielectric Crack    (b)Abnormal structure in the middle  (b)  Abnormal structure in the middle   ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b3222b57-3a99-4e94-b36e-2b63df409ab6/b3222b57-3a99-4e94-b36e-2b63df409ab6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215656%3B1743219256&q-key-time=1743215656%3B1743219256&q-header-list=host&q-url-param-list=&q-signature=1fb938d662e004b444d97ac4025526b4d490e217)
IV. F AILURE MECHANISM DISCUSSION

Fig. 6 Typical failure morphology

When discussing the failure mechanism, it is need to point  out that GaAs pHMET process’s  top layer is Poly-p-phenylene  benzobisoxazole(PBO) material which can  absorb moisture  easily(Fig7). QFN package’s compound isn’t moisture  prohibited material, so insufficient passivation coating make  moisture(  $\mathrm{H}_{2}\mathrm{O}$   in vapour form) possibly penetrated into the  MIM cap, via dielectric crack, moisture can stay in the  capacitor which result in short between top and bottom  plate(Fig. 8). The MIM cap is parallel with RF port in the

switch, so in case of MIM cap shorted by moisture the RF  switch can’t work properly. When baking the failed parts,  moisture evaporates from the MIM cap, then the shorted  phenomena disappear (assume no EOS occur during the shorted  state). It is easily to understand that high temperature and  humidity areas have the higher failure rate. Certainly, during  FA we also found representative EOS failure sample, but the  failure root cause owe to MIM cap process defect.

![+++++++  Mesa Resistor or  D-mode pHEMT   Capacitor   E-mode pHEMT   Thin film resistor  Epi Resistor  Mesa   e1  Ohmic   OEgate   ODgate  Implant   Nitride  TFR   MET1   Niinae   vis3   MET2  Protect   Plating  PBO   Backvia   Street  Nitride   Metol  Fig. 7 pHEMT process structure  Fig. 7 pHEMT process  structure  TopPlate  Moisture  inthe   PlateShortedcausedbyHO  package  BottomPlate  PBO   Dielectirc  Passivation   Metal  Fig.8FailureMechanismDiscussing  Fig. 8 Failure Mechanism Discussing   ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d25f453f-200c-4dc3-80b8-7aae0304af14/d25f453f-200c-4dc3-80b8-7aae0304af14.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215656%3B1743219256&q-key-time=1743215656%3B1743219256&q-header-list=host&q-url-param-list=&q-signature=883019f6c5f726ccc66cf1ce02dfa7ebf97e81ce)
V. R OOT CAUSE AND CORRECTIVE ACTION

Based on GaAs pHEMT process structure, the MIM cap is  composed by two meta layer(M1/M2) and   $\mathrm{Si}_{3}\mathrm{N}_{4}$   dielectric.  when developing passivation on M2, there is a coat thickness  inconformity at the border of the MIM cap. Some MIM caps’  border may not get enough passivation thickness. As for the  dielectric crack,   $\mathrm{Si}_{3}\mathrm{N}_{4}$    has a glass characteristic, particle,  reflectivity & stress will be monitored during GaAs fab process  control monitor(PCM), this method was done by sampling, not  all the defect units can be screened out. It is estimated that the  dielectric crack maybe caused by thermal stress release or  particle. This type component can pass the screening test but  would occur early failure in feild application. It is advised to  thicken the passivation layer to eliminate border insufficient  passivation. Besides process improvement, screen method  such  as add MIM cap breakdown voltage test at the electrical test is  recommended, autoclave test on going reliability test can also  be considered.

## VI. C ONCLUSION  

The paper firstly introduce the application of SPDT switch in  RRU system.Then internal schematic of the switch was briefly  discussed.In the third part, detail failure analysis information

was given especially on the failure morphology. Failure  mechanism was also explained. In the end of the paper, design  and screen  corrective actions were recommended to improve  component reliability and reduce early failure rate .

IC(integrated circuit) failure analysis is an important way to  improve devices’ reliability, but it is often difficult to find the  root cause especially in EOS failure. Luckily, with the  development of analysis equipment and techniques, root cause  seeking become easy. GaAs based RF component has many  applications in communication system and will survive for a  long time, as discussed in the paper, only when root cause is  confirmed, the corrective actions can be efficient and targeted.  The analysis of RF switch in the paper not only verify early  failure often owe to defect units flow out, but also a good  reference for GaAs component failure analysis.

## A CKNOWLEDGMENT 

The authors would like give thanks to the support of ZTE  wireless reliability department for this work. Mechanism  discussion with National Joint Engineering Research Center of  Reliability Test and Analysis for Electronic Information  Products also offers big help. The analysis and reliability  testing assistance from  iST (Shanghai) and finance support  from Guangdong Provincial Science and Technology Plan  Project under NO.2017B090903006 should be appreciated as  well.

## R EFERENCES 

[1]    Frank Gao, “High reliability in pHEMT MMICs with dual-etch-stop AlAs  layers for high-speed RF switch applications”, Microelectronics  Reliability, Vol. 43, pp. 829-837, June 2003.    [2]    Steven V. Pabbisetty, “Failure Analysis Overview”, Microelectronics  Failuer Analysis, US, Desk Reference  $5^{\mathrm{th}}$   Edition, PP. 1-14, October 2004    [3]    Feng-Tso Chien, Da-Wei Lin, Chih-Wei Yang, Jeffrey S. Fu, Hsien-Chin  Chiu, “A low insertion loss GaAs pHEMT switch utilizing dual   $\mathrm{n+}$  -doping AlAs etching stop layers design”, Solid-State Electronics, Vol.  54,  pp. 231-234, March 2010.    [4]    Hsien-Chin Chiu, Chia-Shih Cheng, Jeffrey S. Fu, Kuang-Po Hsueh,  “Harmonics   suppression   investigations   of   pHEMT  single-pole-single-throw   switches   using   multi-gate   structures”,  Microelectronic Engineering, Vol. 87, pp.2592-2595, December 2010.    [5]    Jia Lu, BoCheng Cao, WenShe Wu, YuFeng Dai, G. Mura, “MIM  capacitor-related early-stage field failures”, Microelectronics Reliability,  Vol. 52,  pp. 2073-207, October 2012.     [6]    Chunlei  Wu,  Suying  Yao, “A  Dynamic  Synchronization  Method  to   Realize Soft  Defect  Localization  Applied  on  Digital  and  Mixed-mode   Analog  ICs  in Failure  Analysis”, Microelectronics Reliability, pp.  993-999,  May 2014.     [7]    Xuanlong Chen, Liyuan Liu, Enliang L, “Metal defect localization of  GaAs or Si based ICs by   dynamic emission microscopy”,  Microelectronics Reliability ,  Vol.72, pp.   24-29, May 2017.    [8]    Justin Parke, Randy Lewis, Kathy Ha, Harlan Cramer, Harold Hearne,  “Design and process related MIM cap reliability improvement”,  Microelectronics Reliability, Vol. 55, pp.2516-2521, December 2015.

