---
title: "148_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_d61906323e269ac3aab944556a20bd6b7295230462135641
file_size: 2148086
---

## Research on intermittent fault mechanism of bond  wire under vibration and environmental shock based  on simulation  

Wenxiang Yang 1,2 , Guanjun Liu 1,2 , Kehong Lyu 1,2 , Xinyu Luo 1,2 , Kai Shen 1,2 , Jing Qiu 1,2,\*   1 College of Intelligence Science and Technology, National University of Defense Technology, Changsha, Hunan  2 Science and Technology on Integrated Logistics Support Laboratory, National University of Defense Technology, Changsha, Hunan  410073, People's Republic of China  Phone :(Country Code)860731-, Email : qiujing16@sina.com

Abstract —High Density Integrated circuit (HDIC) is an  important component of modern electronic equipment. As a key  electrical connection component, bond wire is also a weak  component, which is prone to failure when subjected to  vibration and environmental impact. Compared with the  traditional research focusing on permanent faults, intermittent  faults are rarely studied due to their variable transformation  characteristics, but the existence of intermittent faults cannot be  ignored. In this paper, the temperature shock and vibration  simulation of the bond wire are carried out, and the relevant  model is constructed according to the contact resistance theory  to calculate, and the intermittent breakage and short circuit  mechanism of the bond wire under vibration and environmental  impact are studied. This paper provides some theoretical and  technical support for the intermittent faults of high-density  integrated circuits.

Keywords—Intermittent   fault,   Bond   wire,   Simulation,  Integrated circuit, Contact resistance

## I.    I NTRODUCTION 

With the development of science and technology,  electronic devices play an important role in various fields. As  one of the core components of various modern electronic  devices, the reliability of high-density integrated circuit  (HDIC) is very important. The failure of the HDIC may lead  to the scrap of the entire electronic equipment. Experiments  and reliability data show that transient and intermittent faults  are the main faults experienced by modern computers, and  intermittent faults are one of the main causes of semiconductor  device faults [1]. As the key electrical connection component  of HDIC, the bond line is also its weak component, so it is of  great significance to study its fault.

Intermittent Fault (IF) refers to a failure of a product that  recovers its prescribed functions without repair for a limited  period of time after intermittent fault. Intermittent faults have  the characteristics of short duration, appearing and  disappearing from time to time, and can be repeated [2].  Intermittent faults exist widely in various electronic systems,  and field data from the US military equipment and electronics  industry show that 70 to  $90\%$   of the faults detected by modern  equipment are intermittent faults. Intermittent faults in  integrated circuits are usually 10 to 30 times more frequent  than permanent faults   [3]. In an integrated circuit, the chip is  the core component. The bonding line is a relatively weak part  of the chip, and its reliability is crucial. But the traditional chip  production process only removes products with obvious  damage or that have shown permanent failure, failing to detect  potential damage, and intermittent failure during subsequent  use is rarely studied. In fact, intermittent failure of the bonding  line is likely to occur during subsequent use due to various

environmental impacts. In some cases, the instantaneous  failure may cause serious problems, so it is necessary to study  the   mechanism   of   intermittent   failure   caused   by  environmental shock and vibration.

![Bonding wire  Criticalposition  analysis  Temperature   Frequency  Temperature  Simulation   Vibration  shock  Tine   Amplitude  Data extraction  Resistance  Intermittentfault  analysis  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fec651be-63c5-4768-8073-5c0412a51579/fec651be-63c5-4768-8073-5c0412a51579.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=42fcb8a42b3cf6fed6dc86f33d1522ed4802292b)
Fig. 1.   Thesis research ideas.

The research idea of this paper is shown in Fig. 1. Through  theoretical analysis, this paper will select the weak part of the  bond line and build the contact resistance model for the weak  part. Then, the temperature shock and vibration shock are  applied to the bond line, and the influence of environmental  shock and vibration on the bond line is studied by adjusting  the relevant parameters, such as the maximum and minimum  temperature, vibration frequency, amplitude, etc., and the  mechanism of intermittent failure of the bond line is studied.  This paper provides some theoretical and technical support for  the study of intermittent faults in high-density integrated  circuits.

## II.   S IMULATION   

## A.   Theory  

Holm first proposed the electrical contact model [4]. He  believed that current transmission on the contact surface is  realized by many contact points in the contact area, which are  called conductive spots. The variation of the contact resistance  is determined by the depth of the microconvex body pressed  into the plane. Then many researchers proposed that two  rough surfaces in contact can be equivalent to a single rough  surface in contact with a smooth surface, which makes the  calculation of contact resistance easier [5]. Inspired by this,  the model of the crack position in this paper is constructed.  Two rough surfaces in contact are equivalent to a single rough  surface in contact with a smooth surface, and the surface

microconvex body of the equivalent contact surface is  simplified to a series of circular tips.

## B.   Construction of simulation model  

According to literature research and previous research, the  dangerous position of bond wire is mainly located at the  welding position of bond wire and high-density integrated  circuit. And according to the existing research results, even if  the bond line cracks, as long as it is not completely broken, the  resistance change is not large [6]. Therefore, in this paper, it  is assumed that the bonding lines will be completely broken  but there are some connections between each other, which is  more consistent with the situation when intermittent faults  occur. The constructed model is shown in Fig 2a. Fig. 2b  shows a magnified view of the crack position. The bond wire  material is gold, the pin material is copper, and the highdensity integrated circuit material is silicon. The temperature  change is applied to the bond wire surface, and the vibration  is applied to the chip and the pin. The physical fields used are  Solid Mechanics and Heat Transfer.

![（a） （b) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9994be99-16c4-4fec-bcaa-af263d46b268/9994be99-16c4-4fec-bcaa-af263d46b268.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=774507c38d20851031718f95590c256ca9f549d5)
Fig. 2.   (a) three-dimensional model (b)  enlarged image of crack location.

The mesh division of the finite element model is shown  in the following figure. Due to the large difference in model  size, the mesh division of the crack position is further refined  in this paper to ensure accuracy, and the calculation is carried  out by a reasonably high performance computer. As shown in  Fig. 3.

The applied temperature shock is shown in the following  figure, where the simulation puts the bond line in a high  temperature environment and then instants to the extreme case  of a low temperature environment. The temperature impact  strength is 10K, 20K, 40K, 80K, 160K, 240K. (See Fig. 4)

The vibration simulation model is the same as the  temperature shock model, and the same vibration is applied to  the high-density IC and the pins. The input vibration shock is  a decaying sine wave, and the direction is perpendicular and  parallel to the direction of the lower surface of the highdensity integrated circuit. Fig. 5 shows the relationship  between input vibration impact time and amplitude.

![ca) （b） CCJ  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f12b99eb-ee50-41a6-b13a-61dc5cec1fcb/f12b99eb-ee50-41a6-b13a-61dc5cec1fcb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=d82bb5a6c11300fa5196fe2cff08b5ad038b8f52)
Fig. 3.   (a) Model grid division; (b) Meshing of crack locations and (c) plan  views of the contacting faces.

![420  OK  400  1 0K  w80   20K  40K  36０  80K  340  160K  320   ２40K  280  260  240  2201  200  180  160-  1O  Time (s)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c35c2ddb-9a04-4aad-8d4c-dddedbd32bda/c35c2ddb-9a04-4aad-8d4c-dddedbd32bda.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=6812330f46cb0d415640bb54ba198d8bd46d0517)
Fig. 4.   Temperature impact curve.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/924b1afd-404d-45af-8602-dbd184b4013a/924b1afd-404d-45af-8602-dbd184b4013a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=8b4c452cadacf05fcd109fcb7104766af6f8d458)
Fig. 5.   Vibration impact curve.

## III.   R ESULTS AND  D ISCUSSION 

Fig. 6 shows the deformation of the bond line when  subjected to temperature shock, and the deformation is  magnified for easy display. It can be seen that the thermal  deformation mainly occurs on the bonding line, thus causing  deformation at the crack position.

For bond wire, intermittent faults at the damage are  essentially changes in contact resistance at the crack.  Therefore, in this paper, the change of contact resistance when  the bond line is subjected to temperature shock is simulated  and analyzed. Fig. 7 shows the contact resistance variation  when the bond wire is subjected to different degrees of  temperature shock.

![(a）m(1)-120时间-1.55 （b） ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f173c0b0-e568-499c-9e44-ed222ef64043/f173c0b0-e568-499c-9e44-ed222ef64043.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=bfc91c3bb491c2a39047c6d5d99d6ffcb500c875)
Fig. 6.   (a) The overall thermal deformation of the bond wire under  temperature impact; (b) thermal deformation at the crack location of the bond  wire.

It can be seen from Fig. 7 that the contact resistance is  mainly mutated at the temperature mutation position and  remains fluctuating within a certain range after a certain  mutation. The contact resistance value is related to the holding  temperature; a higher initial temperature leads to a lower  impact temperature and a lower contact resistance. This is  because both high temperature and low temperature will lead  to obvious deformation of the bond line, which makes the  contact surface to the micro-convex body and the upper  surface contact intensified.

![1000  900-   OK  20K  800-  40K  700   80K  160K  600  240K  S00  400  300  200  100  10  Time (s)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/936bd2c3-f574-4389-aa22-95d1d1071eaf/936bd2c3-f574-4389-aa22-95d1d1071eaf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=fd06dccafb618b4e4940c3d05703e2007e0834d0)
Fig. 7.   The contact resistance changes at the crack when the bond wire is  impacted by different temperatures.

Fig. 8 shows the strain cloud diagram of the bond line at  0.5s, 1s and 1.5s. It can be seen that the strain values before  and after the temperature mutation are significantly larger than  those when the temperature mutation occurs. As the  temperature decreases, the bond line shrinks, the down  pressure recovers, the contact decreases, and the contact  resistance increases sharply. Subsequently, the temperature  continues to drop, the inner side is pressed down, the contact  is intensified, and the contact resistance continues to decrease.

![（a) 0.5S 1.5s ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1bd38895-9ec1-4f1f-bbc9-6d31e5a49a7b/1bd38895-9ec1-4f1f-bbc9-6d31e5a49a7b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=4e7dfb8c818f2ef34868d1d7c7b0224080376aae)
Fig. 8.   Strain diagram of the bond line crack position at 0.5s, 1s and 1.5s in  (a), (b) and (c).

![（a）0.5s （b）1s （c）1.5s ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/77fd0c2c-503c-409d-9827-48986acc9dee/77fd0c2c-503c-409d-9827-48986acc9dee.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=53445408ee4154b3a2ebfb87cd54bf64761b15a6)
Fig. 9.   Stress distribution diagram of bond line crack position at 0.5s, 1s  and 1.5s in (a), (b) and (c).

It can be seen from the stress diagram (as shown in Fig. 9)  that the stress is mainly concentrated in the micro-convex  body, and the contact resistance decreases with the increase of

stress, indicating that the micro-convex body at the  corresponding position is compressed, the contact area  increases, and the resistance decreases. By comparing the  stress changes in the temperature impact process, it can be  seen that the larger the stress, the smaller the contact resistance.  Before and after the temperature mutation (0.5s, 1.5s), the  stress was significantly greater than that at the time of  temperature change (1s).

In general, the change of the contact resistance is caused  by the alternating change of the contact condition of the  contact surface, and the temperature shock has an important  impact on this. When the resistance change is greater than a  certain degree, it will show intermittent circuit breakage.

Compared with the temperature shock, the vibration shock  has a greater impact on the bonding line. The contact  resistance changes of longitudinal and transverse vibration  impact are shown in Fig. 10.

![（a) 1000 S000 RS 40OKD 2000 02  06  0S Cb5 Time (s) LONOMONN SO0O RS ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3cd207b0-71fd-4d18-84d7-b5d45f19beec/3cd207b0-71fd-4d18-84d7-b5d45f19beec.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=ddd63b1be6586577bde5e024a76e148548f22660)
Fig. 10.   Variation of contact resistance at the crack of the bonding line under  the impact of (a) longitudinal and (b) transverse vibration.

It can be seen that for the bond line close to fracture, the  vibration influence is very huge. Except for the initial  vibration stage, most of the time is almost in the open state.  Although there is some contact, it has been completely unable  to work normally, and there is a risk of complete fracture at  any time.

According to the previous study, if the bond wire is not  completely broken, the resistance changes little. However,  there may still be a short circuit problem between the two bond  lines. In particular, when the bond line is impacted by lateral  vibration, the swing amplitude will gradually increase. When  it reaches a certain level, contact will occur between adjacent  bond lines, resulting in short circuit (as shown in Fig. 11). In  this regard, we carried out further research.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ee06d058-8544-4b1e-a61c-12f30a8f4917/ee06d058-8544-4b1e-a61c-12f30a8f4917.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=b1218debae9b2ef891da65f276e21af9ea141087)
Fig. 11.   Model when two adjacent bond lines are in contact.

![0.0014  AM=0.05mF=50Hz  0.0012  AM=0.05mF=40 Hz  AM=0.05mF=20 Hz  0.0010-   AM=0. 05mF=10 Hz  0.000  0.0004  0.0002  0.0000  0.00   0L0S   010  Time(s)  0.00  AM=0.05mF=80 Hz  AM=0.05 m F=60 Hz  0.003  AM=0.05mF=100Hz  d  0.002  0.001  0.000  0.00   005   0.10   0.1S   020  Time (s)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/236017d1-c66b-46ae-8914-40ba906fafee/236017d1-c66b-46ae-8914-40ba906fafee.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=d731089b50362f72ca2ad546e338cbe914270618)
Fig. 12.   The difference of the maximum lateral displacement minus the  standard spacing when two adjacent bond lines are subjected to lateral  vibrations of different frequencies.

Fig. 12 shows the difference of the maximum lateral  displacement of two parallel bond lines minus the spacing  when the high-density integrated circuit is subjected to  vibration of the same amplitude and different frequencies. If it  is greater than 0, it can be considered as contact, that is, short  circuit. Fig. 13 shows the influence of vibration with different  vibration amplitudes at the same frequency on the contact  situation of two parallel bond lines.

It can be seen that vibration has an obvious effect on bond  line short circuit. With the increase of frequency and  amplitude, the frequency of contact between each other  increases, and the number of short circuit increases.

![0.004  AM=0.01mF=50Hz  AM=0.02mF=50Hz  0.003  AM=0.05mF=50Hz  AM=0.1mF=50Hz  量0:002  0.001  0.000  0,00   0.05   0.10   0.15   0.20  Time (s)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/888db39c-8db0-477e-9860-7fda29c469fc/888db39c-8db0-477e-9860-7fda29c469fc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215855%3B1743219455&q-key-time=1743215855%3B1743219455&q-header-list=host&q-url-param-list=&q-signature=97391b6ca7de9d04b93331190c2c81e5ce5d95c2)
Fig. 13.   The difference of the maximum lateral displacement minus the  standard spacing when two adjacent bond lines are subjected to lateral  vibrations of different amplitudes.

## IV.   C ONCLUSION 

Finally, some important conclusions are obtained through  the simulation study of the impact and vibration of the bond  wire under different temperatures.

Firstly, it is obvious that vibration and temperature shock  have obvious effects on intermittent fault of bond lines.  Temperature shock may lead to intermittent circuit breakage,  and vibration may lead to intermittent circuit breakage and  short circuit.

Second, the change of the contact resistance at the crack  position occurs at the moment of the temperature change, and  the contact resistance remains basically unchanged when the  temperature is unchanged. According to the mechanism  analysis, the change of contact resistance is due to the change  of thermal deformation when the ambient temperature of the  bonding line changes, which leads to the change of the contact  situation above and below the crack position, and finally leads  to the change of contact resistance. The variation of the

contact resistance is correlated with the variation of the  ambient impact temperature. However, whether the contact  resistance increases or decreases and how much the contact  resistance changes depends on the initial temperature of the  temperature shock. The higher the temperature at high  temperature impact, the lower the contact resistance, and the  lower the temperature at low temperature impact, the lower  the contact resistance. In theory, intermittent failures can be  suppressed to some extent by stable high and low  temperatures.

Thirdly, the impact of vibration on the cracked bond line  is very obvious, and the contact resistance changes greatly  except for the initial vibration stage. The higher the vibration  frequency and amplitude, the greater the contact resistance  fluctuation, and the higher the frequency of intermittent circuit  breakage.

Fourth, vibration can also lead to intermittent short circuits  of two adjacent bond lines. The higher the vibration frequency  and the larger the amplitude, the higher the frequency of  intermittent short circuits.

## R EFERENCES 

[1]    ZHONG T, QU J, FANG X, et al. The intermittent fault diagnosis of  analog circuits based on EEMD-DBN [J]. Neurocomputing, 2021,  vol.436, pp.74-91.    [2]    ZHOU D, ZHAO Y, WANG Z, et al. Review on Diagnosis Techniques  for Intermittent Faults in Dynamic Systems [J]. IEEE Transactions on  Industrial Electronics, 2020, vol.67(3), pp.2337-47.    [3]    PAN S, HU Y, LI X. IVF: Characterizing the Vulnerability of  Microprocessor Structures to Intermittent Faults [J]. IEEE Transactions  on Very Large Scale Integration (VLSI) Systems, 2012, vol.20(5),  pp.777-90.    [4]    HOLM, RAGNAR. Electric contacts : Theory and application /-4th ed  [M]. Electric contacts : Theory and application /-4th ed, 1979.    [5]    BAHRAMI M, CULHAM J R, YOVANOVICH M M, et al. Thermal  Contact Resistance of Non-Conforming Rough Surfaces Part 1:  Contact Mechanics Model [J]. 2004, vol.18(2), pp.209-17.    [6]    YANG W X, ZHANG Y, QIU J, et al. Research on intermittent fault  of bond wire under thermal and vibration shock based on simulation  and experiments  [J]. Microelectronics Reliability, 2023, vol.150,  pp.115214.

