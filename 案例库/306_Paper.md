---
title: "306_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_1932598b09726bafcecde55a4d2cc66f7295230462135641
file_size: 716080
---

## A Study of Bonding Pad Corrosion Caused by  Contamination  

Hao Gan, Lin Shi, Xiuqun Zhang, Hongsheng Dai  ZTE Corporation, No.55,Hi-tech Road South, Nanshan District, Shenzhen, 518057, China  Phone: +86-0755-26777569  Email: gan.hao@zte.com.cn

Abstract- This paper introduces a typical corrosion phenomenon of  the Integrated Circuits.A three-terminal adjustable shunt  regulator outputted abnormal voltage on a PCBA because its  $\mathbf{V_{ref}}$  pin was open.Bonding pad corrosion was confirmed by  SEM&EDX analysis.The pad was electrical open to the  surrounding schematic.After a whole  investigation, several lots of  wafers were confirmed to be contaminated by silicone oil which  was introduced during the demolding process. Delamination  occurred between the molding compound and die.Plating solution  which contained chlorine and sulphur percolated into package  during Tin Plating.Supplier of the regulator was recommended to  improve   the   demolding   process.Besides,routine   reliability  monitoring(such as C-SAM, HAST) can be executed in quality  control process to eliminate this failure mode in customer’s  application.

Keywords  –  Regulator, Open, Silicone Oil, Contamination, Delam,  Corrosion

## I. I NTRODUCTION 

A three terminal adjustable shunt regulator offers excellent  temperature stability and outputs current up to 100mA. It is  widely used as a replacement of Zener diodes in many  applications which shows in Fig. 1.In this paper, a typical failure  mode of the regulator is studied.  $\mathrm{V_{ref}}$  Pin of the regulator (on a  PCBA )failed during field application especially in high  humidity area.The failure regulators were decaped and  analyzed  by SEM&EDX.Corrosion was found on the inner bonding pad  of the  $\mathrm{V_{ref}}$  Pin and abnormal elements S&Cl were detected. After  a whole investigation of  the manufacturing process, Tin Plating  Solution was confirmed as the source of S&Cl,and chemicals  percolated into the package when delamination existed between  molding compound and lead frame. At last,demolding process  improvement   and   routine   reliability   monitoring      is   recommended to eliminate this failure mode before field  application.

![+  OUTPUT  INPUT  Von\~2V  Voff = V+  VTH=2.5V  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cea68672-7aa0-44c5-a207-86574a9b2e04/cea68672-7aa0-44c5-a207-86574a9b2e04.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215695%3B1743219295&q-key-time=1743215695%3B1743219295&q-header-list=host&q-url-param-list=&q-signature=e6df3aeb1183e9e1fbe405856a5e5b850dbf1932)
Fig. 1 Typical Application---Single Supply Comparator with Temperature   Compensated Threshold

## II.   FAILURE ANALYSIS  

After disassembled from the fault PCBA, failure analysis of  the   three   terminal   adjustable   shunt   regulator   was  executed.Visual inspection showed no abnormality, IV curve  confirmed the   $\mathrm{V_{ref}}$   Pin of the NG Device(failure sample) was  open which should be a diode’s characteristic(Fig.2).Fig.3  indicated no wire bonding issue after X-ray.Ultrasound  Scan(C-SAM) showed partly delamination between the mold  compound and the substrate as in Fig. 4.

![VERT/DIV  10uA  CURSOR  (f:1/grad.)  HORIZ/DIV  50my  CURSOR  OK   (f:intercept)  DEVICE  PERSTEP  200mA  OFFSET  OmA  BORgm/DIV  50u  Xof  COLLECTOR  PEAK  VOLTS  30.9  NGDEVICE  AUX SUPPLY  0.00V  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ea943dd4-3a9d-4efd-9f89-d1c7b60ad8d7/ea943dd4-3a9d-4efd-9f89-d1c7b60ad8d7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215695%3B1743219295&q-key-time=1743215695%3B1743219295&q-header-list=host&q-url-param-list=&q-signature=e316fd3ddd5c02b671c9b1d8500b8be39bd4d7a6)
Fig. 2 IV Curve of  V

ref

Pin of  NG device Vs OK device

![  Vref  Vref  Vz  GND  GNID  Fig. 3 X-ray Image of NG Device  Fig. 3 X-ray Image of NG Device  Fig. 4 C-SAM Image of NG Device  Fig. 4  C-SAM Image of NG Device (Partly Delam)  (Partly Delam)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/24c19eba-5c61-49c7-95f0-c421399f9082/24c19eba-5c61-49c7-95f0-c421399f9082.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215695%3B1743219295&q-key-time=1743215695%3B1743219295&q-header-list=host&q-url-param-list=&q-signature=2383e0ddecfc65854dfb048928cf3c516f935eaf)
After   non-destructive   analysis,failure   sample   was  decaped.Bubble was observed on the die as Fig .5  showed.Internal microscope image indicated Aluminum layer  was corroded at the inner Bonding pad of   $\mathrm{V_{ref}}$    Pin as in   Fig. 6\~7[1\~3]. As corrosion leaded the pad open to surrounding  schematic, the device couldn’t work rightly. Further analysis  was performed on the corrosion site by SEM, EDX showed  chlorine/sulfur elements existed. Typical corrosion failure  mechanism was verified.

1

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/86f7f017-dfb5-4cd6-8c33-06df0d23639e/86f7f017-dfb5-4cd6-8c33-06df0d23639e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215695%3B1743219295&q-key-time=1743215695%3B1743219295&q-header-list=host&q-url-param-list=&q-signature=c235931acf77bfb787c00d60257e2b18b3c3c882)
Fig. 5 Decap Image of  NG Device (partly,Bubble found )

![k OK  NG NG Device Device  Device Device  S4700 5.0KV11.8 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4519d7cc-a86c-4d9f-bb01-ee8ad7d529f5/4519d7cc-a86c-4d9f-bb01-ee8ad7d529f5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215695%3B1743219295&q-key-time=1743215695%3B1743219295&q-header-list=host&q-url-param-list=&q-signature=0e20487b751e6443748f130ad1dc26756dbc35f3)
Fig. 6 SEM Image of  NG Device Vs OK Device

![Sum  Spectrum  (8kV   primary  bezm)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/448e8011-4734-4bea-ba4c-781d7645dce9/448e8011-4734-4bea-ba4c-781d7645dce9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215695%3B1743219295&q-key-time=1743215695%3B1743219295&q-header-list=host&q-url-param-list=&q-signature=05ecf4692a1a72324f4735949572bd23a3e08a55)
Fig. 7 SEM&EDX Image of  NG Device

## III. ROOT CAUSE AND DISCUSSION  

A whole investigation of manufacturing process was  conducted. Since S& Cl were confirmed in Tin Plating solution  & Replenisher, suspect process from Molding to Tin Plating was  fixed.There was a routine maintenance(molding clean process)  during molding.All failure devices were checked to be molded  after a maintaining of the mold tool.Routine molding clean  process was confirmed to be related to the failure of the device  as in Fig. 8.Mold tool cleaning adopted Silicone Oil which was  volatilized on a high temperature.Delamination formed easily  during molding when the oil remained on the surface of  die and  leadframe.

![  Spry  Spry   Silicone Oil  Silicone Oil   Demolding  Demolding      Cleaning  Cleaning   Trail  Trail    Normal Production  Normal Production    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5113b860-293c-423e-ad7c-01212ff3a24d/5113b860-293c-423e-ad7c-01212ff3a24d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215695%3B1743219295&q-key-time=1743215695%3B1743219295&q-header-list=host&q-url-param-list=&q-signature=573f586071a1776511319e87e158ffa79f6d247a)
Fig. 8 Routine Mold Tool Cleaning Process

Fig. 9 showed standard procedure requested 5mins or longer  after molding tool maintenance to make sure the temperature of  molding tool recovered and stable.Extended cooling time and  insufficient temperature climb of molding tool resulted in  delamination between the leadframe and molding compound.

![180  O  Lowtemp.time around45s  impact1shot  155  150   Tool opened (operating cycle)  145   Tool closed (operating cycle)   Tool had remained open (maintanace)  Tool closed (maintanance fnished)  130  125  60   120   210  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/58b89b95-fa43-4cc0-b522-7f4c79b6ed2a/58b89b95-fa43-4cc0-b522-7f4c79b6ed2a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215695%3B1743219295&q-key-time=1743215695%3B1743219295&q-header-list=host&q-url-param-list=&q-signature=202f62a0b371652677c584cf712b3e9995aea19a)
Fig. 9 Mold Tool Temperature(Maintenance Vs Standard Operation)

![Mold Tool with silicone Oil  InjectMold  Compound  Hot  PauseCure&OpenMold Tool  IseDela   Plating  Chemicals  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d4bb823e-ee92-44f1-b718-123e042cec0c/d4bb823e-ee92-44f1-b718-123e042cec0c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215695%3B1743219295&q-key-time=1743215695%3B1743219295&q-header-list=host&q-url-param-list=&q-signature=bb64f6c062e99a5bb8dc8872bf5ce817abd4debe)
Fig. 10 Molding and Tin Plating Process

Fig. 10 showed how chemicals which contained elements S&Cl  penetrated into the package along the gap formed in molding  process, and corrosion occurred on Al layer of  the bonding  pad[4-5].It   was   believed   chemical   corrosion   was   in  dominate,typical  chemical reaction formula were as follows:

，

.

To confirm the root cause,a series of experiments were  conducted.According to the results of  experiments in Table 1,it  was confirmed contamination with tin plating chemicals would  corrode the die as in Fig. 11-12.High temperature and high  humidity would accelerate corrosion.

Table 1 - Simulation Experiments of  Corrosion

|Experiment|Process|Conditions|Observation|
|---|---|---|---|
||        All tin plating                chemicals on                wafer      |Normal|Corrosion|
||        All tin plating                chemicals on                wafer      || occurred after|
|||        Environment,                RT(Room                Temperature)      |72Hrs|
|2|All tin plating|        Temperature)                THB(85'C/      |Corrosion|
||        chemicals on                wafer      |        THB(85'C/                85%.RH      | occurred after|
||||24Hrs|
|3¥|        Silicone oil+All                tin plating                chemicals on      |        Normal                Environment,                RT(Room      |Corrosion|
|||        Environment,                RT(Room                Temperature)      |        occurred after                96Hrs      |
||wafer|||
|4|        Silicone oil+All                tin plating                chemicals on      |THB(85'C/|        Corrosion                occurred after                72Hrs      |
|||85%.RH)||


![  Fig. 11 Wafer Image(patly) before  Fig. 11 Wafer Image(patly) before   Fig. 12 Wafer Image(patly) after 96hrs  Fig. 12 Wafer Image(patly) after 96hrs THB(85/85%.RH)  THB(85/85%.RH)   THB(85/85%.RH)  THB(85/85%.RH)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fc3857df-496b-4763-96a4-edafe21c5079/fc3857df-496b-4763-96a4-edafe21c5079.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215695%3B1743219295&q-key-time=1743215695%3B1743219295&q-header-list=host&q-url-param-list=&q-signature=d9d55905369e0534bd655695b0fe639e5d0d9ab0)
## IV. PROCESS IMPROVEMENT STUDY  

To have a good understanding of the process of corrosion,a  series of  trails were conducted.

Table 2 - Study of Contamination Formation

|Trails|Target|Process|Observation|
|---|---|---|---|
|1#|Voiding/ Contamination|heavy silicone oil on leadframe,cold mold compound|No bubbling, No Corrosion|
|2#|Voiding/ Contamination|heavy silicone oil on leadframe, RT mold compound|No bubbling, No Corrosion|
|3#|Voiding/ Contamination|heavy silicone oil on tool only, RT mold compound|No bubbling, No Corrosion|
|4#|Voiding/ Contamination|mold temp. 165°C, PMC 3h|No bubbling, No Corrosion|
|5#|Voiding/ Contamination|mold temp. 165°C, silicone oil on leadframe,PMC 3h|Bubbling found|
|6#|Voiding/ Contamination|mold temp. 185°C, PMC 3h|No bubbling, No Corrosion|
|7#|Voiding/ Contamination|mold temp. 185°C, silicone oil on leadframe,PMC 3h|No bubbling, No Corrosion|


According to the observations of  trails   $1\#{\sim}3\#$   in Table 2,it  was confirmed silicone oil on leadframe or tool wouldn’t caused  voiding when molding at a normal temperature (between  170\~180).According to the observations of trails   $4\#{\sim}7\#$  in  Table 2,it was confirmed silicone oil would left and cause  bubbling when molding at a lower temperature (below   $170\,\boxed{,}$  ).Bubbling  was observed on the surface of    $70\%$   trial  samples after molding.Mold compound lid showed dark  roughening/bubbling which matched pictures of lid from failed  device as in Fig. 13[6]. Improper control of opening time of  the  Mold Tool and usage of Silicone oil affected molding reliability.

![Trial Sample  Trial Sample   NG Device  NG Device  Match    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/05396a24-175b-4ec7-be41-d9942d2f76cd/05396a24-175b-4ec7-be41-d9942d2f76cd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215695%3B1743219295&q-key-time=1743215695%3B1743219295&q-header-list=host&q-url-param-list=&q-signature=2230472648540ddca2a1fc81558b82006319bc0d)
Fig. 13 Decap Pattern of  Trail Sample Vs NG Device

To take precautions against corrosion in field,some  improvements as in Table 3 were advised to make.

Table 3 - Improvement Actions

||Process||
|---|---|---|
||Maintenance||
|||        Action                #Review Working Instruction and machine /lot                documentation, including temperature control                (new min 175C)                #Documents who,what, when has repaired the                mold equipment/mold tool                Verify package quality and reliability                #Quarterly check delam per SOT23 package by      |
|||        Action                #Review Working Instruction and machine /lot                documentation, including temperature control                (new min 175C)                #Documents who,what, when has repaired the                mold equipment/mold tool                Verify package quality and reliability                #Quarterly check delam per SOT23 package by      |
||||
|24|QualityReview||
|||        #Quarterly check delam per SOT23 package by                C-SAM      |
|||#Quarterly HAST for SOT23 package|
|34|        Assembly                Process/                Final Test/                Quality Control      |#8Dstatus|
||        Assembly                Process/                Final Test/                Quality Control      |#ORT Failures|
||        Assembly                Process/                Final Test/                Quality Control      |        #Check and summary of records in terms of                abnormalities of last week      |


## V. C ONCLUSION 

On the basis of the above results, S&Cl from tin plating  solution caused bonding pad corrosion.The root cause was  improper using of silicon oil during the demolding  process.When the cooling time of the mold tool was longer,  silicone oil cannot  volatilized sufficiently, it remained on the  surface of die and lead frame which caused delam during  molding[7].Gap caused by delam between the mold compound  and lead frame offered entering path of Tin Plating solution.

By the analysis of this paper,supplier of the regulator is  recommended to improve the demolding process by controlling  the opening time of the Mold Tool.Besides,routine reliability  monitoring(such as C-SAM, HAST)can be executed in quality  control process to eliminate this failure mode in customer’s  application.

## A CKNOWLEDGMENT 

The author would like to give thanks to the support of   Reliability Department of Wireless Product, ZTE.The analysis  and reliability test assistance from the   National Joint  Engineering Research Center of Reliability Test and Analysis  for Electronic Information Products  and finance from  Guangdong Provincial Science and Technology Plan Project  under NO.2017B090903006  should be appreciated as well.

## R EFERENCES 

[1]    S.C.Kolesar, ”Principle of corrosion”, 12th Ann. Proc. International  Reliability Physics Symposium, p.155, 1974    [2]    C. D. Breach, F. W. Wulff. “A brief review of selected aspects of the  material science of ball bonding[J]”.Microelectronics Reliability  2010(50)1-20.    [3]    Y.hua, k. Lim Yeow etal. “Investigation and Failure analysis of   “flower-like” defect on Microchip Aluminum Bondpads in Wafer  Fabrication”.   IEEE international Conference on Semiconductor  Electronics[C]. 2006:626-629    [4]    Ma Teng, Han Zhenyao, Han Wei, “A review of atmosphere corrosion of         Aluminum and Aluminum Alloys” in Corrosion Science and Protection  Technology, Vol16, NO3. pp 155\~160. May 2004    [5]    Ernst P,Newman R C, Corrosion Science, 2002  44:927     [6]    McCafferty E, Corrosion Science, 2003  45:1421     [7]    Willford R E, Windisch C F Jr, Jones R H, Materials Science and  Engineering:A, 2000,28(1):54

