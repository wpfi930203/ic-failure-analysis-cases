---
title: "209_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_0ddab66459d7b79c80bc894874bd8d517295230462135641
file_size: 1409434
---

## Electrical field accelerated GND corrosion of  copper wire in high humidity conditions  

Xuanlong Chen 1, 2, \* , Jianming Fang 1, 2 , Wenfeng Huang 1, 2 , Yong Wei 1, 2 , Chengcheng Chen 1, 2   1 China Electronic Product Reliability and Environmental Testing Research Institute, Guangzhou 510610, China  2 Reliability Research and Analysis Centre, China CEPREI Laboratory, Guangzhou 510610, China  Phone: (86-20) 87239769   Fax: (86-20)87237185   Email:  chenxl@sina.cn ,  chenxl@ceprei.com

Abstract- Galvanic corrosion of copper wire in high humidity  conditions has been widely studied. Cu-Al system in water forms a  battery cell and Al is corroded. The commonly known factors that  accelerate the corrosion include humidity, ions, pH, etc. In a real  case failure analysis and biased high humidity test, an accelerated  corrosion was observed to be related with bias or current direction.  The GND copper wire terminal disconnection was proved to be  easier to occur, and electrochemical reactions identified as  electrolytic cells played a dominant role. The failure mechanism is  hard to be recognized sometimes for carbonized molding  compound surrounded around the pad, which will lead to an  improper conclusion of electrical overstress (EOS). Electrical field  accelerated corrosion is a degradation process which might not  cause a sudden failure.

Keywords – copper wire ,  galvanic corrosion ,  cathodic protection ,  degradation failure ,  open failure

## I. I NTRODUCTION 

Copper wire interconnection is widely used in plastic  integrated circuit, including high density packages like Ball  Grid Array (BGA). Great efforts have been made in industry to  improve the reliability of copper bond through researches and  engineering practices. High temperature test demonstrates the  mechanical strength, measured with ball shear test, of ball bond  did not significantly change over the full range of Al  consumption[1].   Palladium-coated   copper   (Pd-Cu)   or  palladium-gold-coated copper (Pd-Au-Cu) wire have been  adopted for its better performance of oxidation and corrosion  resistances[2], which improve the bond reliability by protecting  the intermetallic compounds (IMC) from the propagation of  micro cracks. The molding compounds have also been adjusted  to high purity resin, increased ion catcher content and neutral  pH[3].

Owing to the researches in this field, the enhancement of long  lifetime and reliability promote the mass production of copper  wire. The concerns for susceptibility of Cu wire are mainly on  humidity applications. There are three types of corrosion that  can occur in wet environment of microelectronic package,  namely, chemical reaction, galvanic corrosion and electrolytic  cell. The IMC, especially Cu 9 Al 4 , of Cu-Al system is prone to be  attacked by Cl -  ion[2,4], resulting in open failures. Galvanic  corrosion is another key factor that affects the lifetime in  application [5]. Even in Pd-Cu system, the electrochemical  effect is non-negligible[6]. Although these chemical reactions  have already been restricted through process adjustment,  degradation occurs when environment is not fully under control

in real-life applications, especially when electrical bias and high  humidity are both applied on the devices.

Recently, about 10 ppm per month failure rate of Hall Effect  sensor of two different types was found in the electrometric  oven after working for two years. Both short circuit and open  circuit were observed in products returned from customers.  Initial analysis conclusion demonstrates that electrical  overstress was responsible for the failure. Since the aluminum  pad was surrounded by carbonized molding compound, which  indicated an over current and heat was generated. However,  insight investigations including circuit tests and PCB board  analysis were performed and no electrical anomaly was found,  the mechanism of the failure was still undefined. As the failure  was still continuing, more physical analysis was performed and  eventually gave available statistical information about the failed  features. Most of the ball lift occurred at the GND terminal, very  few opens occurred at the I/O terminal and no failure was found  at Vcc terminal. Beside carbonized molding compounds,  oxidation and corrosion of Al also provided another insight. It  means that there is extra driving force to accelerate the reactivity  of corrosion, because galvanic corrosion should exit in Cu-Al  systems, not just in GND terminal. In this work, a failure  hypothesis that the failure might be related to electrical bias or  current direction was proposed. Based on these assumptions,  biased high temperature and humidity test was performed to  assess the root cause.

## II.   E XPERIMENT AND METHODOLOGY 

## A. Sample Preparation 

According to the copper wire chemical etching method[7,8],  the decapsulation flows is shown in Fig.1. The optimized  decapsulation condition is fuming   ${\mathrm{HN}}{\mathrm{O}}_{3}$   and   $\mathrm{H}_{2}\mathrm{SO}_{4}$   (  $96\%$  concentrated acids) with the weight proportion of 3:2 at   $150\,^{\circ}\mathrm{C}.$  .  After chemical etching, the sample was cleaned with acetone,  deionized water, and ethanol respectively in an ultrasonic bath  for 30 seconds at room temperature.

![(a)   Laser Laser  Molding compound  Molding compound C   CuWire  Cu Wire Die  Die ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1aafad3c-c513-42c3-b793-75bbf95fe098/1aafad3c-c513-42c3-b793-75bbf95fe098.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=6602e267046bd1ee725154c43e6f6387c88a1c2f)
![(b)  Tweezer  Tweezer Dropper  Dropper Block heater  Block heater       (c)  CC    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a0d869da-d1d3-4b51-b251-5ef8ea638978/a0d869da-d1d3-4b51-b251-5ef8ea638978.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=7db1073ae1ac26f6bd4c4779919dd5f6b7fe35e9)
Fig. 1. Moulding compounds decapsulation flows for Cu wire bonding.

On the other hand, to avoid chemical or electrochemical effect  bringing contamination and affecting elements analysis, cross  sectioning and ion milling were also performed to inspect the  interface between copper wire and aluminum pad.

## B. Physical Analysis 

High resolution X-ray radiography was carried out to estimate  the chip size in order that laser and chemical etching is in the  proper window. After ion milling, SEM and EDX analysis were  performed to identify and investigate the refined physical  characteristics and determine the elemental composition or  possible contaminations, oxidation in corrosion area.

## III. R ESULTS AND DISCUSSION 

## A. Failed sample analysis 

Two types of Hall Effect sensors integrated with H-bridge  transistors returned from customer were investigated, in which  the bonding wire was made of pure copper. Electrical tests  revealed some of the failures are unstable even though most of  the damages are permanent. Current-voltage (I-V) curves of  these samples confirmed that the unstable phenomenon was  caused by increased resistance. It indicated that these failures  might come from copper wire instead of die. Most Cu-Al bonds  failed at the GND terminal with carbonized resin, as shown in  Fig. 2 and Fig. 3, few samples were found only copper bonds  lifted without any carbonization. The carbonization indicated  localized heat had generated around the bond during operation.  As commonly known that heat is a result of EOS failure, such as  transistor breakdown under bonds, overcurrent of contacts, etc.  In this case, no PN junction was under the pad but emitter  contacts. Therefore, the heat might be from overcurrent. The  contradiction is that current formed a loop, and the power supply  pad flowed the same current as ground while no heat induced

damage was observed. Since the load was inductor in fan,  overcurrent might be triggered if the fan got stuck. This  hypothesis was easily verified, and the results indicated that  during high temperature operation, H-bridge transistors burned  out first instead of pad.

The heat concentrated around the pad indicated the initial  defect should be related to specific bias conditions. It can be  inferred extra power consumption occurred at the bond, possibly  caused by the increased resistance of bond. To investigate the  exact failure mode at bonding interface, cross-sectioning  inspection was performed using SEM.

![(a)  Vcc  GND  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/21c621dc-6c6c-42f5-81ff-6a6e52d0a92c/21c621dc-6c6c-42f5-81ff-6a6e52d0a92c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=c4ad48e9b9727128a0c4870c13a5d76f0382cdc6)
![(b)  GND  Vcc  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2352dda8-f24e-4aec-a2ad-670d5ba19e98/2352dda8-f24e-4aec-a2ad-670d5ba19e98.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=14b9b7251dfc9fcbd2ecbca97bb07779fdb1ebdd)
Fig.2 Copper bond failures at the GND terminal.

![(a) F1-2  初16.3  n10.0kV ×1-01 SES ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4bd9bc1c-43a1-448a-85ae-2c64cfc5820a/4bd9bc1c-43a1-448a-85ae-2c64cfc5820a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=1be3dedc5982470177c3ab2d94aa822f2bd8c59f)
![(b)  Mag=500X   EPT   0.00 kv   SE2  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/302bdf4b-3119-46b6-a698-c7f700c5e91f/302bdf4b-3119-46b6-a698-c7f700c5e91f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=1aa1d21cdad4eef4327b16d6deb10dffc1d05677)
Fig.3 The magnified image of failed pad with carbonized plastic.

Cross sectioning SEM images indicated the crack was at the  interface of intermetallic compounds and aluminum pad, in  which a thick layer of aluminum oxide film was observed  (Fig.4). No obvious contaminants were detected, which  suggested there was another force to decompose the aluminum  when exposed in air, e.g. corrosion.

![(a)  (a)  Carbonization  Carbonization  (b)  Al oxide layer Crack  Al oxide layer  Crack   IMC  ND=74m   FHT=15.00KV   SignalA=AsP  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0a5002f8-74d2-4965-9042-78f25e19d15d/0a5002f8-74d2-4965-9042-78f25e19d15d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=f6d64ac236435a03409cc3e98891a6f2b8742d9e)
Fig.4 Cross sectioning reveals the failure nature: (a) entire bond, (b) zoomed in  sections.

The samples were biased for 1 h and stored for 3 h, while the  temperature was set at   $85\ ^{\circ}\mathrm{C}$   and the humidity was   $85\%$   RH.  Five in forty-four samples failed after 500 h tests, with  resistance of GND increased slightly. The physical failure  analysis confirmed that the crack located at the aluminum pad  which was possibly corroded, the signature was almost the same  as field return products. Micro-crack was also observed in the  well performance samples, in which the embryonic zone of  crack located around the bond, as shown in Fig.5.

![Al oxide layer  Al oxide layer  Crack  Crack  S5   F2-11WD13.9mm 10.0kV x20k   2Um  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/dc6e6da1-9763-4d6c-886b-172f751e8cab/dc6e6da1-9763-4d6c-886b-172f751e8cab.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=8211e092ab67ddfc767182bacc0af513ee67ea31)
Fig.5 Embryonic zone of crack located around the bond.

## C. Failure mechanism study 

There are various corrosion mechanisms inducing this kind of  failure. From previous study[9], ionic contaminant (e.g. Cl - )  triggered failure will result in decomposition of IMC, and  copper re-deposition should be observed. The positive electrode  attracting anion is more prone to be corroded. This is  contradictory to our experiments, in which no obvious  contaminant was detected and no positive electrode failed.  Therefore, there must be another dominant factor driving the  failure. The failure might be formed in several steps, and  galvanic corrosion (Fig.6) is one of the causes, which initially  caused Al dissolution and crack at the   $\mathrm{{Cu}/A l}$   interface. Since  galvanic corrosion effect is equal for all bonds, the galvanic  degradation process is not fully responsible for the failure.

![H,O+2e-+O2—→2OH-  H O+2 e - + O  2OH - 2  2 Cathode  Cathode H++e—→H  H + + e -  H  Cu C  e - Al—→Al3++3e  Al          Al 3+ +3 e -  Al Anode  Anode ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f6639071-58b9-4569-bce1-43221d6d3fd4/f6639071-58b9-4569-bce1-43221d6d3fd4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215657%3B1743219257&q-key-time=1743215657%3B1743219257&q-header-list=host&q-url-param-list=&q-signature=60cc6f34f151ca92982d4393432219471d4e62d0)
Fig.6 Schematic diagram for galvanic corrosion at Cu-Al bond [5].

## B. Biased high temperature and high humidity test 

Copper wire has proved its robustness in high temperature  operation test, and as far as we know, no signature of crack  location distribution has been reported. Therefore, high  temperature and high humidity operation test was preferentially  chosen to recur the failure.

There is another force to increase the reactivity, probably  electrolytic reaction, which is a selective corrosion under  electrical field bias and causes fast failure. Electrolytic reaction  also forms metal decomposition, the conditions are: a film of  polar liquid (usually water) to form an electrolyte, bias and  operating time. GND staining caused by electrolytic reaction  has been reported in several literatures [10-11]. Even at wafer  level manufacturing, aluminum pad corrosion could not be

neglected. The built-in potential in the PN junction and the  basic/acidic solution cause the GND corrosion.

The ionic solution in an electrolytic reaction is generally  classified into three categories: neutral solution, acidic solution  and basic solution. In neutral and acidic solution, aluminum in  anode is preferential to dissolve, the reaction formula is the  same as follows:

Acidic/neutral solution    Cathode   6H +  + 6 e -  →  3H 2       Anode       $2\mathrm{Al}\cdot6e^{\cdot}\rightarrow\ 2\mathrm{Al}^{3+}$    Basic solution    Cathode   2H  $2\mathrm{H}_{2}\mathrm{O}+2e\mathrm{\cdots}\rightarrow\ 2\mathrm{OH}\mathrm{+}\mathrm{H}_{2}$      Anode       $2\mathrm{Al}\cdot6e\cdot4\mathrm{OH}\cdot\rightarrow\ 2\mathrm{AlO}_{2}\cdot+2\mathrm{H}_{2}\mathrm{O}.$  .

In high humidity environment, absorbed water will eventually  forms a thin film of water on the surface of die. The pH of the  package would change towards weak acid. As the bias was  applied, the potential of aluminum pad was higher than copper  wire for GND terminal, forming electrolytic cell and dissolves  the pad. As a result, the strength of the bond was decreased and  crack was expanded. As the effective contact size decreased  significantly, the current density of the residual Cu-Al bond  increased and generated heat concentration, resulting in molding  compounds carbonization. The carbonization is a polarized  conductor with a relatively high resistance to replace the Cu-Al  bond, that’s why lifted bond will not cause a sudden failure.

As for Vcc terminal, the electrical field of aluminum is lower  than that of GND terminal and the electron flow direction is  from Al to Cu, protecting Al from losing electrons, known as  cathodic protection.

D. Methods improving the corrosion resistance of Cu-Al bond

After discussing the corrosion mechanisms and the factors  impacting the reactivity, in this section, we propose methods to  avoid or decrease the failures. As mentioned above, the  corrosion attack is mainly caused by electrochemical effect  including humidity environment, heterogeneous chemical  composition, or pH. Therefore, reducing the influence of  inducing factors could enhance the corrosion resistance, such as  introducing inertia element (Pd, Au, etc.) [2], reducing chloride  concentration [6], and improving the molding compound. Since  the influence of water is the dominant factor, water barrier layer  outside the circuit is also suggested applying in system level  applications.

## IV. C ONCLUSION 

Cu-Al bond is susceptible in high humidity conditions,  especially for GND terminal, resulting in corrosion. Hall sensors  are probably most exposed to such problem, since many of them  are operating under harsh environment conditions including  high humidity condition. The failure was caused by  electrochemical corrosion of aluminum pad. Apart from  galvanic corrosion, there exists an accelerated factor to GND  terminal, probably electrolytic reaction. Positive electrode  (aluminum) is consumed faster than the negative electrode  (copper), which causes crack and higher current density.  Localized heat caused by high current density might carbonize

the molding compounds and degrade the bonds. It should be  noted that the carbonization is not a result of EOS.

## A CKNOWLEDGMENT 

At the point of finishing this paper, we’d like to express our  sincere thanks to all those who have support us with the analysis  and summary to complete this work in China CEPREI  Laboratory. This work was supported by grants from the quality  and reliability research project (No.1707XXXX17), the 2017  Industrial Transformation and Upgrading (Made in China 2025)  Fundation (Departmental Budget) - Promotion and Application  of Reliability Design Technology for Intelligent Household  Appliances and Advanced Consumer Electronic Products  (No.TC170A5UG/2).

## R EFERENCES 

[1]  R. Pelzer, R. Nelhiebel, R. Zink, et al. “High temperature storage reliability  investigation of the Al-Cu wire bond interface,”  Microelectron Reliab , vol.  52, pp. 1966-1970, 2012.    [2]  H. W. Park, S. J. Lee, D. C. Cho, et al. “Behavior of Au and Pd and the  effects of these metals on IMCs in Pd-Au-coated copper wire,”  Microelectron Reliab , vol.91, pp. 283-290, 2018.    [3]  T. S. Kiong, S. T. S. Hian, N. Khan. “Mold compound optimization and  certification for Cu Wire leaded package,”   $I\mathcal{A}^{t h}$   Electronics Packaging  Technology Conference (EPTC) , pp. 542-546, Singapore, December 2012.    [4]  P. S. Liu, L. Y. Tong, J. L. Wang, et al. “Challenges and developments of  copper wire bonding technology,”  Microelectron Reliab , vol. 52, pp.  1092-1098, 2012.    [5]  S. H. Kim, J. W. Park, J. T. Hong, et al. “The interface behavior of the Cu-Al  bond system in high humidity conditions,”   $I2^{t h}$   Electronics Packaging  Technology Conference (EPTC) , pp. 545-549, Singapore, December 2010.    [6]  Y. L. Wu, K. N. Subramanian, S. C. Barton, et al. “Electrochemical studies  of Pd-doped Cu and Pd-doped Cu-Al intermetallic for understanding  corrosion behavior in wire-bonding packages,”  Microelectron Reliab , vol.  78, pp. 355-361, 2017.    [7]  M. Krüger, J. Krinke, K. Ritter, et al. “Laser-assisted decapsulation of  plastic-encapsulated devices,”  Microelectron Reliab , vol. 43, pp. 1827-1831,  2003.    [8]  S. Murali, N. Srikanth. “Acid decapsulation of epoxy molded IC packages  with copper wire bonds,”  IEEE Trans Electron Packag Manuf. , pp. 179-183,  2006.    [9]  X. L. Chen, L. Y. Liu. “Failure analysis on corrosion induced Cu-Al bond  failures,”  in Symposium on the Physical and Failure Analysis of Integrated  Circuits (IPFA) , pp.69-72, Singapore, July 2016.    [10]  H. Endoh, T. Naoe. “Copper wire bonding package decapsulation using the  anodic protection method,”  Microelectron Reliab , vol. 55, pp. 207-212,  2015.    [11]  K. E. Mautz, M. Hall, J. Cadenhead. “Elimination of bond pad corrosion  caused by solvent exposure,”  in Proceedings of the Third International  Symposium on Corrosion and Reliability of Electronic Materials and  Devices , the Electrochemical Society, pp.253-259, 1994.

