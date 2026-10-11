---
title: "319_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_77c21996ef182e62ea3ff33cb33450247295230462135641
file_size: 748020
---

## Failure Analysis of Solder Joint Cracking in a CBGA  Assembly Applied for Aviation Equipment  

Hui Xiao, Daojun Luo, and Weiming Li  Reliability Research and Analysis Center, China CEPREI Laboratory, Guangzhou, China.  Phone: +86-20-87053229   Email: xiaohui_ceprei@163.com

Abstract-   Board-level thermal-mechanical reliability is one major  concern in CBGAs. A typical early fault case of some aviation  equipment was studied in this paper. The failure phenomenon was  manifested as malfunction of the main board in the flight control  computer. The results of fault location showed that there was  interconnection failure in the CBGA module in the main board. A  serial of experimental technologies were used for the failure  analysis, such as 3D X-ray inspection, microsectioning, optical  microscope, scanning electron microscope (SEM), etc. The results  showed that some Pb37Sn63 solder joints’ through cracking in the  CBGA assembly was the immediate cause of the equipment’s  malfunction.   The   main   reason   for   the   cracking   was  thermal-mechanical fatigue with microstructure coarsening  degradation, resulting in early failure of the main board. It is  suggested to carry out components’ board-level application  verification in aviation equipment and other high reliability field.

Keywords  – Failure analysis, CBGA assembly, Solder joint  cracking, Thermal-mechanical fatigue .

## I. I NTRODUCTION 

Ceramic ball grid array (CBGA) is a kind of high-density  surface mount package, which can be connected to the printed  circuit board (PCB) by solder balls as the I/O circuit ends.  Because the ceramic substrate can offer the advantages of finer  routing density, multiple power and ground planes, improving  signal integrity, moisture resistance and thermal conductivity,  CBGA packaging has been gradually used in aviation  equipment and other high reliability field in recent years [1].

However, the CBGA package exhibits poor solder joint  reliability when compared to organic packaging technologies,  there is still limited second-level interconnect reliability for  large-size CBGAs [2]. Solder joint failures for surface mount  packages are typically a result of fatigue cracking caused by  shear strain accumulated during the life of the component [3, 4].  The crack would often induce the failure of whole system or  even more severe problem, because such package is usually  used as the core component, such as CPU, FPGA, DDR, and so  on [5, 6]. Therefore it is necessary and important to study such  crack failure cases, since it could help find the reliability  weakness and further provide guidance for the package design  or assembly application to prevent such crack failure [7, 8].

In this paper, a failure case of solder joints’ cracking in a  CBGA assembly applied for aviation equipment was  investigated and the failure cause was revealed.  Furthermore,  the package fatigue mechanism was studied, which gives

suggestion about the solder selection and structure design to the  reliability application.

## II.   S AMPLES AND  M ETHODS 

## A.    Sample Discription  

The test samples used for this research were some failure  printed circuit board assembly (PCBA) products in flight  control computers applied in some aviation equipment after two  years’ service. The failure phenomenon was manifested as  malfunction of the main board in the flight control computer.  The results of fault location showed that there was  interconnection failure in the CBGA module in the main board,  as shown in Fig. 1. For the CBGA module, the Pb37Sn63 solder  balls were planted on the component pads, and the component  was mounted onto the FR4-type PCB by reflow soldering using  Pb37Sn63 solder.

![CBGA  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/73ef8a9e-daf1-4eee-bdc4-779ed8f42a85/73ef8a9e-daf1-4eee-bdc4-779ed8f42a85.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215698%3B1743219298&q-key-time=1743215698%3B1743219298&q-header-list=host&q-url-param-list=&q-signature=173e8e971e045c5adfa1e49a495969a9fb40f52d)
Fig. 1  Sample local appearance picture

Failure analysis was performed for these CBGA assembly  failure samples. Some PCBA products with the similar  application environment with the failure samples were used for  assistant analysis, in which the CBGA component had   $\mathrm{Pb90SD10}$   solder balls planted on the component pads and the  component was mounted onto the FR4-type PCB by reflow  soldering using Pb37Sn63 solder. And there was not  interconnection failure in the CBGA module with Pb90Sn10  solder balls in the main board after two years’ service.

## B.    Failure Analysis Methods  

A serial of experimental technologies were used for the  failure analysis.

Visual Inspection

Visual inspection was conducted to observe the soldering  quality of the CBGA solder joints under the stereomicroscope.  Some solder joints’ surface defects (such as surface cracks,  poor wetting, and so on) can be detected by this inspection.

3D X-Ray Inspection

3D X-ray inspection was conducted to observe the CBGA  solder joints in the failure PCBA samples, focusing on the  process defects, such as solder joint voids, cracking, head in  pillow (HIP), etc.

## I-V testing for the IC  

The main CBGA chip device was desoldered from one failure  PCBA sample by hot air gun. I-V characteristic testing was  conducted for the IC of the desoldered CBGA device, and the  testing results as the I/O port features were compared with that  of the OK CBGA device samples which were not assembled.

## Microsectioning and microscope analysis  

Microsectioning was conducted for the main CBGA chip  device solder joints, and the microstructure was observed by  optical microscope and scanning electron microscope (SEM).  The CBGA solder joints’ sectioning was conducted in the order  that first for periphery solder joints and later for central solder  joints.

## III. Results and discussion  

It was found under the stereomicroscope that there were some  surface voids in some CBGA solder joints, as shown in Fig. 2.  The results of 3D X-ray inspection showed that there were  some voids in CBGA solder joints, but not any defects such as  leakage solder, solder bridge, head in pillow (HIP), etc., as  shown in Fig. 3. These phenomena manifested that the  soldering quality of the CBGA module was not very well.

The representative cross-sectional views of the solder joints  for the failure PCBA sample, lying in the CBGA ’ s periphery  and central location, are as shown in Fig. 4 and Fig. 5.

![     void  void  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ccca8951-3ead-4c1f-8927-7f4121a16a0b/ccca8951-3ead-4c1f-8927-7f4121a16a0b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215698%3B1743219298&q-key-time=1743215698%3B1743219298&q-header-list=host&q-url-param-list=&q-signature=d82c4f7f4722988ccc2bdd169cbe498584829037)
Fig. 2  Views of visual inspection results for the CBGA solder joints

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3407f2f7-5cf3-4285-8d27-e73314b44b93/3407f2f7-5cf3-4285-8d27-e73314b44b93.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215698%3B1743219298&q-key-time=1743215698%3B1743219298&q-header-list=host&q-url-param-list=&q-signature=767fcab25917a493ac17c07d23b1194172fa64f0)
Fig. 3  Representative views of 3D X-ray inspection for the CBGA solder joints

Fig. 4 details the representative cross-sectional view of the  solder joints lying in the CBGA’s periphery location. It can be  seen that there was through cracks near the PCB pad in the  periphery CBGA solder joints. And there was coarsening  microstructure along the cracking zone, which was indicated as  thermo-mechanical fatigue characteristics [9]. The solder  joints ’ failure phenomena with significant location feature  were related to the large CTE mismatch between the ceramic  package and PCB board in the CBGA module.

![  +++++++  (a) Through crack near the PCB pad  (a) Through crack near the PCB pad     H1=3.896  iag=  344X   WD=8.1mm   EHT=20.00KV   FASE  (b)Microstructure coarsening  (b) Microstructure coarsening   ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/df84111e-bca9-4126-94c1-d75c72af77f5/df84111e-bca9-4126-94c1-d75c72af77f5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215698%3B1743219298&q-key-time=1743215698%3B1743219298&q-header-list=host&q-url-param-list=&q-signature=d80f90097046efa32d1fddf564125aa5c9c24198)
Fig. 4  The representative cross-sectional views of the failure solder joints

Fig. 5 shows the micromorphology of the solder joints lying  in the CBGA ’ s central position. It can be seen that there was  uniformly microstructure in the solder joints, and there was not  any obvious coarsening microstructure in the interfacial zone.

Fig. 6 shows the statistical matrix of the microstructure  observation results for the CBGA solder joints. The results  showed that there were some solder joints with cracks near the  PCB pads, lying in the BGA ’ s periphery. And for the four  corner of the array, there were solder joints with through cracks.  However, it was not found any cracks in the solder joints in the  BGA ’ s central position. This failure phenomenon of solder  joints with location feature was related to the stress/ strain  distribution in the CBGA module.

Fig. 7 shows the cross-sectional views of solder joints for the  different CBGA assembly samples, with different BGA solder  composition, which were used in the similar application  environment. It can be seen that there were different solder  joints ’  height for the same PCB pad size, the height of the  Pb90Sn10 solder joints was higher than that of the Pb37Sn63  solder joints. It is related to the different collapse resistance of  the Pb37Sn63 solder ball and the   $\mathrm{Pb90SD10}$   solder ball, which  eventually resulted in the difference of CBGA solder joints ’   fatigue life.

![  (a) Solder joint lying in the CBGA’s central position (a) Solder joint lying in the CBGA's central position    WD=8.0m  (b) Uniformly microstructure in the interfacial zone   ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/128379bd-7eed-45fd-910a-270bf50a5dc4/128379bd-7eed-45fd-910a-270bf50a5dc4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215698%3B1743219298&q-key-time=1743215698%3B1743219298&q-header-list=host&q-url-param-list=&q-signature=b25993e7d876439409267f0b35894b3ddd4ca4bb)
Fig. 5  The representative cross-sectional views of the central solder joints

![19  18  16  14  11  1C  ABCDEFGHJKLMNPRTUVW   Unchecked solder joints   Unchecked solder joints  Solder joints with local cracks   Solder joints with local cracks   Solder joints without cracks   Solder joints without cracks   Solder joints with through cracks  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/51bd2ee5-3488-4eeb-bb8e-ddcb2515ccdf/51bd2ee5-3488-4eeb-bb8e-ddcb2515ccdf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215698%3B1743219298&q-key-time=1743215698%3B1743219298&q-header-list=host&q-url-param-list=&q-signature=ce6c9620b2d877927a47461ac2412a15d141186d)
Fig. 6  Statistical matrix of the microstructure observation results for the CBGA  solder joints

![  (a) CBGA with Pb37Sn63 solder balls  (a) CBGA with Pb37Sn63 solder balls     (b) CBGA with Pb90Sn10 solder balls  (b) CBGA with Pb90Sn10 solder balls   ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f061408c-e703-49a0-afa7-e82fea13e899/f061408c-e703-49a0-afa7-e82fea13e899.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215698%3B1743219298&q-key-time=1743215698%3B1743219298&q-header-list=host&q-url-param-list=&q-signature=212cdff3142e34f4ab7ae14f46c5cc546c63cec0)
Fig. 7  PCBA samples with different CBGA solder compositions applied in the  similar application environment

The influence of material and structure characteristics leads  to the difference of solder joints’ thermal-mechanical fatigue  [10, 11], as shown in Equation 1 and Equation 2.

$$\mathrm{N_{f}}\,(50\%)\,=\,\frac{1}{2}\,[\frac{2\varepsilon_{\mathrm{f}}}{\Delta\mathrm{D}}]^{\backprime}{}^{\frac{-1}{c}}$$
（1）

$$\Delta\mathrm{D}(\mathrm{leakell})\,=\left[\frac{\mathrm{FL}_{\mathrm{D}}\Delta(\upalpha\Delta\mathrm{T})}{h}\right]$$
（2）

where

$\mathrm{N_{f}}\,(50\%)$   is the median cyclic fatigue life;

$\upvarepsilon_{\mathrm{f}}$   is the fatigue ductility coefficient;

ΔD   is the cyclic fatigue damage term;    $c$   is the temperature and time-dependent exponent;

$\mathrm{L}_{\mathrm{D}}$  is the maximum distance between component solder joints  measured from component solder joint pad centers;

$\Delta(\upalpha\Delta\mathrm{T})$    is the absolute cyclic expansion mismatch, accounting  for the effects of power dissipation within the component as  well as temperature variations external to the component;

$h$   is the solder joint height.

It can be seen that the different height of solder joints is the  key factor resulting in the different thermal fatigue life of the  above PCBA samples. It is suggested that board-level process  verification should be conducted before production definition  of the electronic equipment, in order to ensure that solder  joints ’  interconnection meets the environment requirement in  service.

## IV. C ONCLUSION 

Some Pb37Sn63 solder joints’ through cracking in the CBGA  assembly was the immediate cause of the equipment’s  malfunction. The main reason for the cracking was  thermal-mechanical fatigue with microstructure coarsening  degradation, resulting in early failure of main board in the flight  control computer. Solder selection is a key factor in the  selection of package materials and the design of the structure.  Board-level temperature cycling reliability is one major  concern in CBGAs. It is suggested to carry out components’  board-level application verification in aviation equipment and  other high reliability field.

## A CKNOWLEDGMENT 

This study was supported by the National Key R&D Program  of China under Grant No. 2017YFB0305700, the Fund Project  of Chongqing Science & Technology Commission under Grant  No. cstc2016jcyjA0303, which were acknowledged.

## R EFERENCES 

[1]    L. Tong, C. Jiang, and G. Ao, “Research on the board level reliability of  high density CBGA and CCGA under thermal cycling”,  Proceedings of  the 19th International  Conference on Electronic Packaging Technology  (2018) , pp. 1382-1386.    [2]    A. E. Perkins, and S. K. Sitaraman, “Acceleration Factor to Relate  Thermal Cycles to Power Cycles for CBGA Packages”,  Solder Joint  Reliability Prediction for Multiple Environments , Springer, pp. 157-169,  2009.    [3]    J. C. Roberts, M. Motalab, S. Hussain, J. C. Suhling, R. C. Jaeger, and P.  Lall, “Characterization of compressive die stress in CBGA  microprocessor packaging due to component assembly and heat sink  clamping”,  Journal of Electronic Packaging , Vol. 134, 2012.    [4]    W. Wang, Z. G. Wang, A. P. Xian, and J. K. Shang, “Microstructure and  fracture of Pb-free solder interconnects in CBGA packages under  thermal cycling”, Acta Metallurgica Sinica, Vol. 42, pp. 647-652, 2006.    [5]    R. Kandasamy, and A. S. Mujumdar, “Thermal analysis of a flip chip  ceramic ball grid array (CBGA) package”, Microelectronics Reliability,  Vol. 48, pp. 261-273, 2008.    [6]    W. Li, and X. Zhang, “Thermal-mechanical failure and life analysis on  CBGA package used for great scale FPGA chip”, Proceedings of 2009  International  Conference on Electronic Packaging Technology & High  Density Packaging, pp. 1216-1219.    [7]    X. Lv, Y, Huang, Peng, Lin, X. Jiang, B. Lian, Q. Yao, “Reliability  Study of the solder joints in CCGA package during thermal test”,  Proceedings of the 15th International Conference on Electronic  Packaging Technology (2014), pp. 854-857.    [8]    J. C. Lee, C. C. Chen, D. Lee, C. Chen, and A. Lin. “The novel failure  mechanism of the polymer ball interconnected CBGA under board level  thermal mechanical stress”, Proceedings of the 67th Electronic  Components and Technology Conference (2017), pp. 2015-2020.    [9]    P. Borgesen, L. Wentlent, S. Hamasha, S. Khasawneh, D. Schmitz, T.  Alghoul, C. Grenne, and L. Yin. “A mechanistic thermal fatigue model  for SnAgCu solder joints”, Journal of Electronic Materials, Vol. 47, pp.  2526-2544, 2018.    [10]    IPC-SM-785. Guidelines for accelerated reliability testing of surface  mount solder attachments. IPC, 1992.    [11]    A. Perkins, and S. K. Sitaraman, “Universal fatigue life prediction  equation   for   ceramic   ball   grid   array   (CBGA)   packages”,  Microelectronics Reliability, Vol. 47, pp. 2260-2274, 2007.

