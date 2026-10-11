---
title: "237_Paper_updated.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_fee0ae293b48db1bde4ab3ccd6369b9a7295230462135641
file_size: 1207550
---

## RCA Case Study on MCU EOS Failure Caused by  Chip Crack  

He Shengzong 1 , Cai Jinbao 1 , Zhao Pengfei 1 , Yu Sida 1 , Qiu Baojun 1 , Chen Mianzhi 2 , Wang Yong 2 , Kong Lingming 2 , Chen Jun 2 1 CEPREI Lab. Guangzhou, 370611, China.  2 Guangzhou Power Supply Bureau. Guangzhou, 510410, China  \*Phone: +86-20-87237007 Fax: +86-20-87237185 Email: heshz03@163.com

Abstract —Failure analysis for large-scale integrated circuits  (LSIC) is often a challenging task. It necessitates a  comprehensive approach, incorporating failure data analysis,  examination of failure characteristics, and validation or  replication of the underlying failure mechanisms. This paper  article performs a root cause analysis (RCA) on overstressinduced (EOS) failures specific to a microcontroller (MCU)  utilized in home appliance applications. Firstly, the basic  situation of the case is introduced, and then the specific process  and root cause that caused the failure are identified through  anatomical analysis, fault analysis tree (FTA), and experimental  verification   work.   Finally,   corresponding   improvement  measures and prevention suggestions are proposed to reduce the  occurrence of similar failures, and provide a reference idea for  root cause analysis work of IC EOS failure.

Keywords—EOS failure, failure analysis, root cause analysis,  improvement measure, dielectric layer cracking

## I.    I NTRODUCTION  

MCU serves as a common electronic component widely  used in home appliances, industrial control, consumer  electronics, medical and other industries. However, due to  various reasons, EOS failures occur frequently, and failure  analysis for these cases can be particularly challenging in  defect localization [1], failure localization, and sample  preparation [2], especially for complicated circuits [3-4].  Effectively conducting RCA plays a vital role in eliminating  similar potential issues and enhancing product reliability [5].  This paper delves into an RCA case study on an MCU failure  in a home appliance product, exploring how the integration  of failure data, morphological features, fault analysis trees,  and experimental validation can improve the analysis  accuracy and efficiency.

The case study encompasses a type of MCU with a QFN64 package and copper wire bonding that experienced EOS  failure shortly after being shipped and used with the product.  The product failure rate is as high as   $3000\mathrm{pm}$  , which is  typical of early failure. The client describes that MCU was  applied to mass-produced products shortly after its  development and launch. The failure phenomenon shows  several kinds, including burnout, poor performance index,  communication abnormality, soft crash, control failure and so  on. After a preliminary investigation, it is analysed that the  product malfunction is caused by MCU failure, and the failed  ports are mainly the power ports, with the corresponding  ports on the internal chip being burned out. Figure 1 shows  typical EOS burn point images on failure chips.

In order to solve the problem, the client requested to carry  out RCA program to analyse the specific causes of failure and  formulate corresponding countermeasures.

![（a）  （Cb b）  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/54fb596b-413c-4834-9637-c588b302f08d/54fb596b-413c-4834-9637-c588b302f08d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=0ac95381d71ec0c87d8e1924e242a1d6a02096c5)
(a) Burn point on Chip.   (b) Lower layer structure burnout. Fig. 1 Typical EOS Burn point on MCU chip

## II.    E XPERIMENT AND  A NALYSIS 

## 2.1   Failure Data Analysis  

After investigation and analysis, it has been confirmed  that it has the following failure characteristics:

●    Failure or malfunction mainly occurs during board  functional testing or initial use. According to the  failure time characteristics, it is a typical case of early  failure [6].  ●    Failure MCU occurs on several kinds of electronic  control boards used in various applications, regardless  of the board type. The packaging batches of failed  devices do not have obvious concentration and are  relatively scattered.  ●    After diagnostic investigation, the main types of  device failure modes are as follows:   $\textcircled{1}$  functional  failure, control failure and soft crash;   $\circledcirc$  abnormal  performance indicators: such as low ground  impedance or short circuit of the power port; sampling  value error;   $\textcircled{3}$  abnormal communication function,  such as communication pins open circuit or inability  to establish communication links.

## 2.2   Failure Physical Morphology Analysis   

By dissecting the failed samples, it was observed that the  internal ports of the samples were burned. Through statistical  analysis of the abnormal characteristics mentioned above, it  presents characteristics as follows:

●    Sample appearance shows no obvious abnormalities,  such as burn marks or package cracking.  ●    Port IV testing revealed:   $\textcircled{1}$    approximately   $90\%$   of  abnormal ports were power ports(1.25V,2.5V,3.3V),  mainly exhibiting short-circuits in Fig.2(a) and preactivation or soft junction characteristics in Fig. 2(b);   $\circledcirc$    the remaining   $\mathtt{l o g}$   abnormal ports  were mainly signal communication  ports,   and   were   primarily   open  circuits or pre-activated;   $\widehat{\pmb{3}})$   abnormal  ports were all mainly concentrated in

the areas where the bond wires were  more densely packed.

![（a）  （Cb2 b）    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7a6dd05a-4d9b-4dca-aafc-91f911157099/7a6dd05a-4d9b-4dca-aafc-91f911157099.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=220b0d7f2548d46bf67cdd31a4359f0d29b42f32)
(a) Shorted power ports   (b) Pre-activation ports(signal)  Fig. 2  IV characteristics of failed sample ports

●    X-ray inspection showed no abnormalities. However  most failure samples have small-area delamination  interface between the plastic and the chip, and these  delamination areas often have burnt morphology  below. The layering and internal burnt areas are  mainly concentrated near the internal bonding points  of the power port, as seen in Figure 3.

![（a）  （Cb b）  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c0479b95-2f43-437f-97aa-40044c4de624/c0479b95-2f43-437f-97aa-40044c4de624.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=7e37e595f677ec996f0ae7a5ec13626beace8e70)
Fig. 3  Non-destructive inspection images of the samples

●    After removing the layers, it can be observed that  there are burning abnormalities in multiple locations  such as the port ESD protection network, passive  isolation area and high impedance area [7]. Figure 4  shows the typical morphology of  active area burnout  after metal and dielectric layers have been removed.  Some of the morphological features do not exhibit  complete electrical burnout but are more reminiscent  of mechanical damage in Fig. 4(d).

![（a）  （b）   （c）  （d）      ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fff109c8-6321-4dbb-80e1-ada927ecfbfc/fff109c8-6321-4dbb-80e1-ada927ecfbfc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=34395d323735cc09711cdf5d276570be5b309db6)
(a) Multiple burnout locations. (b) ESD protection diode burnout.  (c) ESD protection diode burnout. (d) Passive isolation area burnout.  Fig. 4 Typical burnout morphology of the active area

●    Some failure samples exhibit abnormal phenomena  such as cracking and delamination in the lower  dielectric layer. Meanwhile, burnout morphology can  be observed in most samples, but strangely enough,

none burnout morphology can be observed in the rest  ones. They exhibit two states in cracked and  delaminated samples: burnt and unburned. These  failures seem to be due to inherent defects in the  dielectric layer (cracking, delamination) [8]. Figure 5  shows typical dielectric layer morphology and  differences.

![（a）  （by b）  （c）  （Cd d）    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/68f79367-4e4b-4522-8bfd-10681aaca6a4/68f79367-4e4b-4522-8bfd-10681aaca6a4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=6c0409caeffee070079b98496127bd214de96e4a)
(a) Internal layer delamination. (b) Dielectric layer separation.  (c) Burnout and delamination. (d) Delamination without burnout.  Fig. 5 Typical dielectric layer morphology

## 2.3   Fault Analysis Tree  

Considering the analysis above, possible failure  mechanisms are hypothesized to include:

●    Burnt area on chip is located in power ports and  exhibits characteristics of overcurrent burning out,  similar to the characteristics of overcurrent burning  out of power port caused by Latch-up effect.  Therefore, there is a possibility of failure caused by  CMOS Latch-up effect.    ●    Burnt ports are mainly concentrated in the protection  network, and so there is a possibility of port  overvoltage breakdown caused by reverse power  connection, over-voltage or surge, or ESD [9-10].    ●    The burnt area is located in a densely bonded area and  it is copper wire bonding, which may cause damage to  the bonding and result in damage, leakage, and  burning.    ●    Internal dielectric layer cracks and exhibits two  characteristics: burnt and unburned. Therefore, it is  reasonable to speculate that the cracking dielectric can  lead to a resistance decrease thus resulting in burnout.  Cracking and delamination of the dielectric layer may  be related to defects in the chip itself and the dicing  process, with the latter being more likely.

Based on the above analysis, it is believed that the main  possible failure mechanism may be:

●    Incorrect   operation,   such   as   reverse   power    connection,  over voltage stress and voltage surge.    ●    Potential damage and failure caused by ESD [11].    ●    CMOS Latch-up effect causes burn out.    ●    Bonding craters cause damage to dielectric layer [12].

●    Delamination defects within the chip itself lead to  burnout failure.  ●    Chip dicing damage causes cracking in dielectric  layer, leading to burnout failure.

2.4   Mechanism Verification Test

The above analysis results indicate that the failure  mechanism of the sample may be caused by several types of  failure mechanisms. In order to further verify the possible  failure mechanisms, a corresponding troubleshooting test  plan is designed, as shown in Table 1.

Table 1. Possible Causes and Verification Methods

|Category|Possible Causes|VerificationMethods|
|---|---|---|
|incorrect operation|        Wrong operation                Overvoltageower surge      |        Power supply electrical overstress testing                Simulated electricaloverstresstesting      |
|ESD Discharge|Damage to protection network caused by ESD|        Device electrostatic discharge testing until failure occurs.                Failure morphology comparison.      |
|CMOS Latch-up|        Abnormal voltage pulse triggers Latch-up failure,                resulting in metallization burning out      |        Device latch capability testing                Conduct latchtests onapplicationcircuitsfrom power and signal ports      |
| Bonding crater|         Bonding crater leads to damage or leakage of the                underlying medium      |        Bonding crater tests on failed and unused samples.                Bonding crater tests on unused samples after temperature cycling      |
|Chip self-defect|        Chip dielectricinherent defects (insufficient                mechanical strength).      |FIB observation of non-conforming test samples|
|        Chip dicing caused                cracking      |        Scratching and packaging stress cause cracking of the                chip dielectric layer,resulting in leakage and burning,                leading to failure      |        uHAST, TC test to exacerbate crack defects.                 Conducting structural analysis.                Inspecting offline wafer sheets      |


## 2.5   Comprehensive Analysis and Conclusion  

The investigation into several factors that could  potentially cause device failure yielded the following  results:

●    Failure   morphology   caused   by   simulated  overvoltage or reverse connection operations is  inconsistent with characteristics of the on-site  failure morphology.  ●    Power ports did not fail in ESD test  at   8000V   (HBM   model),   and   the  simulated failed ports were signal  ports rather than power ports，with  different   failure   morphology  characteristics (Fig.6a).   ●    Samples have a strong Latch-up resistance, neither  normal   temperature   nor   high-temperature  conditions were able to trigger the Latch-up  phenomenon.  ●    Bonding crater tests on both failed samples and  unused sample chips did not reveal any crater  damage (Fig.6b).

![（a）  （Cby b）  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8747912f-9457-46eb-a4d0-268a7d001fb7/8747912f-9457-46eb-a4d0-268a7d001fb7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=0fc63c9a26a7fd98d91f919e62d2ee70150746df)
(a) ESD simulation failure image. (b) Crater test morphology.  Fig.6 Partial verification result images

●    In relation to factors associated with dielectric layer  delamination, through TC, uHAST test  and FIB  observation, unused samples were found failed in  uHAST test, with cracks existing between the metal  layer and dielectric layer (Fig. 7a, b), initiating from  the edge of the chip (scribe lane)  (Fig. 7c, d).  Further uHAST test could trigger similar failures in

more devices. Dissecting failed samples revealed  similar dicing damage (Fig. 7e,  f).

●    From morphological characteristics, it is evident  that edge of the scribe lane consists of slag after  laser ablation, and cracks begin to appear in  dielectric layer closer to the interior, extending  inward towards the active region of the chip,  crossing the isolation rings (Fig.7c).

![（a）  （b）     （C c）  （d）      （e）  （f） ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/55129657-2de5-4d37-9a64-c0fca9c5ed95/55129657-2de5-4d37-9a64-c0fca9c5ed95.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215766%3B1743219366&q-key-time=1743215766%3B1743219366&q-header-list=host&q-url-param-list=&q-signature=bf46c7b8f6084c58ae10a83b3af0a752171bf0c5)
(a) FIB section place. (b)Dielectric layer delamination.  (c) Delamination crossing the isolation ring.   (d,e,f) Delamination initiating from the edge of the chip.  Fig.7 Dielectric delamination verification analysis image.

Based on this, it is judged that cracks in the dielectric  layer are related to the laser scribing of the chip. The  thermal stress during laser ablation process causes the chip  to delaminate and crack, and then cracks are further  extended under the action of thermal stress during chip

packaging[13-14], reflow soldering thermal stress, and  electrical stress, as well as moisture and other factors  during use.

## III.    I MPROVEMENT  M EASURES AND  S UGGESTIONS 

Based on comprehensive analysis and investigation  outlined above, failure MCUs are attributed to thermal  stress from wafer laser scribing, which causes chips to  crack and delaminate, leading to a reduction in dielectric  withstand voltage between the metallization layers of the  chip[15]. Subsequently, during application, factors such as  soldering thermal stress, test electrical stress, and  operational thermal variation stress result in leakage,  breakdown, and burnout between the lower dielectric and  metallization layers, causing failures [16]. The following  improvement measures are recommended:

●    For the unused inventory devices that have already  been produced, it is advisable to conduct burn-in  tests before leaving the factory to eliminate as  many potentially defective devices as possible.  ●    For devices that will continue to be produced in the  future, the device supplier should be required to  optimize and adjust the wafer laser scribing process  without   affecting   the   subsequent   dicing  process[17], reducing slag at the edges of the chips,  and ensuring that the width of any remaining slag  is less than 3um.  ●    Conduct a thorough effectiveness assessment of  the risk of delamination in dielectric layer of the  improved process chips, and validate with tests  such as structural analysis, TCT/TST, and uHAST.

## IV.    C ONCLUSION 

This paper conducts a root cause analysis on the early  overvoltage failure problem of a certain type of MCU. The  failure mode and mechanism were determined through  failure data statistics, morphology feature analysis, fault  analysis tree, and experimental verification. The main  manifestation of failure is damage to the power port, which  may be caused by human factors, latch effects, overvoltage  breakdown caused by surges or electrostatic discharge, as  well as chip bonding crater damage and internal dielectric  layer cracking. Through further investigation and  verification experiments, other possible factors were ruled  out, and it was confirmed that chip scratch damage is the  fundamental cause of chip breakdown and burning during  early use. In addition, proposed optimization processes and  improvement measures to improve product reliability and  prevent similar failures. Certainly, this article merely  provides an illustrative example of a root cause analysis.  The analysis process encountered numerous adverse  factors and information distractions, and is offered solely  for the reference of applied analysis engineers.

## ●    A CKNOWLEDGMENTS 

Thanks team colleagues and customers for the technical  support provided in this case. This research was funded by  the Science and Technology Project of China Southern  Power   Grid   Co.,   Ltd.,   with   project   No.  GDKJXM20220236/030111KK52220019.

## ●    R EFERENCES 

[1]    Wu C ,Yao S ,Corinne B ."Leakage current study and relevant

defect   localization   in   integrated   circuit   failure  analysis"[J].Microelectronics Reliability,2015,55(3-4):463-469.    [2]    Pacheco, and Goyal. "Detection and characterization of defects in  microelectronic packages and boards by means of high-resolution  x-ray computed tomography (CT)." Electronic Components &  Technology Conference 2011.    [3]    Zhonghui, Fan , et al. "The Application of Root Cause Failure  Analysis in a Communication Module." Electronic Product  Reliability and Environmental Testing (2018).    [4]    Boubezari, Samir , and  J. Chhabria . "Failure and root cause  analysis for a system-on-chip: An industrial case study." Design &  Test Symposium IEEE, 2015.    [5]    R. Keith Moble."Root Cause Failure Analysis". ButterworthHeinemann, London, 1999.    [6]    Moosa, Mohamod S. ,  K. F. Poole , and  M. L. Grams . "Validating  IC early-failure simulation." Proceedings of SPIE - The  International Society for Optical Engineering 2635(1995):187- 193.    [7]    Zhu Kehan.“Design and Analysis of On-Chip ESD Protection  Devices for CMOS IC.” Jiangnan University, 2008.  朱科翰.CMOS集成 电 路片上 静电 放 电 防 护 器件的 设计与 分析 [D].江南大 学 ,2008.     [8]    Kawakami, N. , et al. "A super low-k   $(\mathrm{k}{=}1.1)$   silica aerogel film  using supercritical drying technique." IEEE International  Interconnect Technology Conference IEEE, 2000.    [9]    Amerasekera, A , and  C. Duvvury . "The impact of technology  scaling on ESD robustness and protection circuit design."  Components Packaging & Manufacturing Technology Part A IEEE  Transactions on 18.2(1995):314-320.    [10]    Liou, J. J , et al. "Challenges of electrostatic discharge (ESD)  protection in emerging silicon nanowire technology." IEEE (2012).    [11]    Amerasekera A., Duvvury C. ESD in silicon integrated circuits –  second edition [M].New York : John Wiley & Sons, 2002.    [12]    Hashim, et al. "Copper Wire Bonding." Microelectronics and  reliability (2014).    [13]    Li, Jianhua , et al. "Laser Dicing and Subsequent Die Strength  Enhancement Technologies for Ultra-thin Wafer." IEEE (2007).    [14]    Borkulo, Jeroen Van ,  R. Evertsen , and  R. Hendriks . "Enabling  Technology in Thin Wafer Dicing." Ecs Transactions 18.1(2009).    [15]    Sibailly, Ochelio , and  B. Richerzhagen . "Laser dicing of silicon  and composite semiconductor materials." Proceedings of Spie the  International Society for Optical Engineering 5339(2004):394- 397.    [16]    Zhao Laling. "Research on the Die Chipping Failure of Low-k  Dielectrics Wafer in Wafer Sawing." Suzhou University,2016.  赵 腊玲. Low-k介 质 硅晶 圆 切割崩裂失效 研 究[D].  苏 州大 学 , 2016.     [17]    Zhang, Fei , et al. "A study of 355nm DPSS UV laser  micromaching for silicon wafer." Laser Institute of America  (2010).

