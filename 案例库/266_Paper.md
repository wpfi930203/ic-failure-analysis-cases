---
title: "266_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_79d52604852b8db18b844c3515a3dea37295230462135641
file_size: 801341
---

## Investigation of Conductance Fluctuations of Analog  RRAM during Weight Update Process with Kinetic  Monte Carlo Simulation  

Feng Xu, Bin Gao\*, Huaqiang Wu and He Qian  Institute of Microelectronics, Tsinghua University, Beijing, 100084, China.  E-mail:  gaob1@tsinghua.edu.cn

Abstract-  In this work, we investigate the mechanism of  conductance fluctuations during continuous weight update  process in analog type Resistive Random Access Memory  (RRAM). With the developed Kinetic Monte Carlo (KMC)  simulation method, the evolution of oxygen vacancies (V O )  distribution during resistive switching process is presented.  Based on the statistical analysis of the maximum V O -V O   bond cluster size, it is found that the conductance  fluctuation is highly relevant to the maximum cluster size  fluctuation. This can be explained based on the percolation  theory. When the V O  at the key location migrates under the  electric field and thermal activation, the maximum cluster  composed of  $\bf V o^{-}V o$   bond will divide, causing the change of  percolation paths and conductance fluctuation.

Keywords  —  RRAM, Conductance fluctuation, Kinetic  Monte Carlo, Percolation theory

## I.   I NTRODUCTION 

Analog RRAM is proposed as artificial electronic synapse  for in-memory neuromorphic computing. To train the RRAM  based neural network on-chip, the conductance should be tuned  in an analogue way during SET and RESET process. How to  get uniform and continuous conductance tuning behavior is the  key issue for this new application [1]. Several analog RRAM  devices with excellent multilevel reliability and fast  conductance tuning speed have been developed [2]. The device  conductance, which represents synaptic weight, can be tuned  linearly with the identical voltage pulses [3]. However, this  oxide-based filamentary type analog RRAM still face large  conductance fluctuation issues during the weight update  process, which may degrade the learning accuracy and  converging speed. Therefore, it is highly important to  understand the physical origin of the fluctuations and find the  way to suppress them. Unfortunately, owing to the difficulty of  direct observation of V O  distribution, it is still unclear why  conductance change randomly and even may change to the  opposite direction during the weight increase or decrease  process.

We have developed a KMC simulation method to investigate  resistive switching mechanisms and provide design guidelines  for RRAM. In this work, we study the conductance fluctuation  mechanism using this KMC simulation. Based on percolation  theory [4, 5], we find that conductance fluctuation is originated  from the   $\mathrm{V_{O}-V_{O}}$   bond cluster cleavage reduced by the   $\mathrm{V_{O^{-}}V_{O}}$  bond breakage at the key location.

## II.  S IMULATION  M ETHOD 

RRAM cell with TiN/TEL/HfO x /TiN stack is investigated  using KMC method [2, 6]. During conductive filament  evolution in the resistive switching layer, two microscopic  process take place, including oxygen vacancy generation and  migration. The event probability is proportional to the  expression    $e^{-(E_{a}-\Delta\varphi)/k T}$  , where  E a  is the barrier energy,  ∆𝜑 is the barrier decrease due to the local electric field. The  thickness of   $\mathrm{HfO_{x}}$   and thermal enhanced layer (TEL) are  accordingly 5 nm and   $60\ \mathrm{nm}$  , the size of filament region is  limited in  $5\:\mathrm{nm}\times5$   nm region. The simulation flow begins with  initial   $\mathrm{V_{O}}$   distribution, the oxygen and oxygen vacancy bonds  form a random resistor network. The electric potential  distribution is obtained from the Kirchhoff equation, and the  temperature distribution is given by the Fourier heat  conductance equation with Joule heating [7, 8]. Based on the  electric potential distribution and the local temperature  distribution, the probability of V O  generation and migration is  calculated. Successively V O  generation and migration are both  considered, V O  distribution is then updated. The simulation  parameters are listed in the Table  . We assumed electron  transport along the   $\mathrm{V_{O}-V_{O}}$   bond obeys metallic-like ohmic  behavior, whereas O-O bond and   $\mathrm{V_{O-O}}$   bond obey the  tunneling behavior.

TABLE I.     Summary of Parameters

|Parameter|Value|
|---|---|
|Generation barrier of V O|0.8 eV|
|Migration barrier of V O|0.85 eV|
|Oxygen lattice distance|0.25 nm|
|Thermal conductivity of HfO X|5 W/(K*m)|
|Thermal conductivity of TEL|50 W/(K*m)|
|Conductance of V O -V O  bond|5 mS|
|Conductance of V O -O bond|0.05 mS|
|Conductance of O-O bond|1 μS|
|Resistivity of TEL|0.7 mΩ ∙cm|


## III. R ESULTS AND  D ISCUSSION 

Due to the lower thermal conductivity of TEL, higher local  temperature is achieved in  $\mathrm{HfO_{x}}$   layer, oxygen vacancies could  be distributed uniformly [1]. The device exhibits good analog  switching behavior under identical SET pulse as shown in Fig.  1, and severe conductance fluctuation accompanies with the  conductance dynamic growth.

![20.0u  Vset=1.0V Vset=1.1V Vset=1.3v 15.0u 10.01 5.0元 0.0 10:0  150  200 Pulse number ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/19845e64-1368-44eb-a966-f5b01358807b/19845e64-1368-44eb-a966-f5b01358807b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215681%3B1743219281&q-key-time=1743215681%3B1743219281&q-header-list=host&q-url-param-list=&q-signature=1f30e2e93e80c477a87763e4c76f3bcfaeb64eea)
Fig. 1 Conductance of RRAM device changes with identical SET pulses.

The KMC simulation was implemented to study the  conductance fluctuation mechanism. During SET process,  rectangular pulses with constant amplitude of 1.3 V are applied  to stimulate filament formation, and small read pulses with  amplitude of   $0.15~\mathrm{V}$   are applied between programming pulses  to acquire device conductance. The KMC simulation result  shows the same trend with the measurement data of the RRAM  device as shown in Fig. 2. One can observe that as the  conductance grows, obvious fluctuation accompanies with  conductance tuning process.

![45.0μ  14.0  -Conductance  40.0M   - The maximum cluster size  20  35.0μ  10HO  30.0μ  oue  25.0u  20.0u  15.0u  1 010   20-0   300   400   500  Pulse number  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/718ac3e7-2287-45dc-9a86-6f72d863c96b/718ac3e7-2287-45dc-9a86-6f72d863c96b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215681%3B1743219281&q-key-time=1743215681%3B1743219281&q-header-list=host&q-url-param-list=&q-signature=95cda4be847462aedd9ab66f589e11cafef87355)
Fig. 2 Conductance changes under identical read pulses and the statistic of the  maximum cluster size.

To elucidate conductance fluctuation mechanism, we  introduce the maximum cluster size, which is composed of V O - V O  bond. From percolation theory, resistive switching can be  treated as bond percolation process [9, 10]. The cluster size is  defined as the bonds number it contains [11]. The maximum  cluster contributes to the conductance most significantly. Fig.  3 shows the cluster growth with   $\mathrm{V_{O}}$   generation and migration.  Initially, only several random   $\mathrm{V_{O}}$   bonds occupy in the lattice  under thermal fluctuation effect. When voltage stress is applied  to the device, with more   $\mathrm{V_{O}}$   generation, the clusters begin  growing. On the other hand, under electric field, V O  migration  induces the neighboring clusters merging together to form a  larger cluster. When the maximum cluster extends to both  electrodes, the resistive switching occurs.

![Cluster  growth growth          Cluster  Cluster    merge  merge  Resistive  switch         ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1c04d728-3f8c-4024-aca4-af3692bba21b/1c04d728-3f8c-4024-aca4-af3692bba21b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215681%3B1743219281&q-key-time=1743215681%3B1743219281&q-header-list=host&q-url-param-list=&q-signature=712044c649572a0936b1b48175e5f3e6b849b3d5)
Fig. 3 The cluster grows with the V O  generation and migration. The red, blue,  black lines denote the different bond with conductance in descending order.

From Fig. 2, it is found that conductance growth trend is  similar with the maximum cluster size. The fluctuation occurs  synchronously in the growth of conductance and the maximum  cluster size. We choose two moments t1 and t2 when  fluctuation occurs to investigate the Vo distribution and the  $\mathrm{V_{O}}$  -  $\mathrm{V_{O}}$   bond cluster morphology. At the t1 moment, as the V O migration in the vertical direction to the electric field, the  cluster cleaves and results in the percolation path breaking as  shown in Fig. 4 and Fig. 5.

![a   力  Fig. 4 The Vo distribution at the tl moment. (a) Before the Vo migration. (b)  Fig. 4 The   distribution at the t1 moment. (a) Before the   migration. (b)  After the After the Vo migration. The golden cell denotes a Vo site.   migration. The golden cell denotes a   site.       ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/05c94426-9295-49fb-b042-606786d23a31/05c94426-9295-49fb-b042-606786d23a31.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215681%3B1743219281&q-key-time=1743215681%3B1743219281&q-header-list=host&q-url-param-list=&q-signature=91d1b842cc70d4cb47ba62caf022cd74b6f40883)
Fig. 5 The cluster morphology at the t1 moment. (a) Before the  $\mathrm{V_{O}}$   migration.  (b) After the  $\mathrm{V_{O}}$   migration.

Similarly at the t2 moment, the   $\mathrm{V_{O}}$   migration brings the  maximum cluster to divide as shown in Fig. 6 and Fig. 7.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b5509805-b904-4409-ad57-81dfea4b5151/b5509805-b904-4409-ad57-81dfea4b5151.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215681%3B1743219281&q-key-time=1743215681%3B1743219281&q-header-list=host&q-url-param-list=&q-signature=9a23f96de67b78af088a674298e27e03a95c3d40)
Fig. 6 The  $\mathrm{V_{O}}$   distribution at the t2 moment. (a) Before the  $\mathrm{V_{O}}$   migration. (b)  After the  $\mathrm{V_{O}}$   migration. The golden cell denotes a   $\mathrm{V_{O}}$   site.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bda953d9-7db8-40ed-b078-65806986de57/bda953d9-7db8-40ed-b078-65806986de57.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215681%3B1743219281&q-key-time=1743215681%3B1743219281&q-header-list=host&q-url-param-list=&q-signature=6fb4d91b83616d4656c5b47fe06963163b5a4140)
Fig. 7 The cluster morphology at the t2 moment. (a) Before the V O  migration.  (b) After the  $\mathrm{V_{O}}$   migration.

One thing to point out is that the clusters in Fig. 3 is formed  under the stimulating pulses of 1.3V, so the morphology is  different from the clusters in the Fig. 5, Fig. 7 under the read  pulses of 0.15V.

## IV.   C ONCLUSION 

Based on KMC simulation, the conductance fluctuation  mechanism was investigated. We found that the conductance  fluctuation is related to the maximum   $\mathrm{V_{O}-V_{O}}$   bond cluster  division induced by the V O  migration at the key location.

## R EFERENCES 

[8]    F. Pan and V. Subramanian, “A Kinetic Monte Carlo study on the  dynamic switching properties of electrochemical metallization RRAMs  during the SET process,” in  Int. Conf. on Simulation of Semiconductor  Processes & Devices (SISPAD) , pp. 19-22, September 2010.    [9]    D. Islamov, V. Gritsenko, C. Cheng and A. Chin, “Percolation  Conductivity in Hafnium sub-Oxides,”  Appl. Phys. Lett.,   vol.   105, pp.  262903, December 2014.     [10]   H.Yoo, S. Lee, J. Lee, S. Chang, M. Yoon, Y. Kim, B. Kang, M. Lee, C.  Kim, B. Kahng and T. Noh, “Conversion From Unipolar to Bipolar  Resistance Switching by Inserting  $\mathrm{Ta}_{2}\mathrm{O}_{5}$    Layer in  $\mathrm{Pt/TaO_{x}/P t}$   Cells,”  Appl.  Phys. Lett.,  vol. 98, pp. 183507, May 2011.     [11]   J. Hoshen, P. Klymko and R. Kopelman, “Percolation and Cluster  Distribution. III. Algorithms for the Site-Bond Problem,”  Journal of  Statistical Physics,  vol. 21, no. 5, pp. 583-600, May 1979.    [1]    W. Wu ,  H. Wu, B. Gao, N. Deng, S. Yu and H. Qian, “Improving Analog  Switching in  $\mathrm{HfO_{X}}$  -Based Resistive Memory With a Thermal Enhanced  Layer,”  IEEE Electron Device Lett.,  vol. 38,   pp. 1019-1022, August 2017.    [2]    B. Gao, H. Wu, W. Wu, X. Wang, P. Yao, Y. Xi, W. Zhang, N. Deng, P.  Huang, X. Liu, J. Kang, H. Chen, S. Yu and H. Qian ,  “Modeling Disorder  Effect of the Oxygen Vacancy Distribution in Filamentary Analog RRAM  for Neuromorphic Computing,”   in  IEDM Tech. Dig.,  pp. 91-94,  December 2017.    [3]    K. Moon ,  M. Kwak, J. Park, D. Lee and H. Hwang, “Improved  Conductance Linearity and Conductance Ratio of 1T2R Synapse Device  for Neuromorphic Systems,”  IEEE Electron Device Lett.,  vol. 38, pp.  1023-1026, August 2017.    [4]    D. Stauffer and A. Aharony,  Introduction to Percolation Theory.  Taylor &  Francis, 2003, ch. 2, pp. 15.     [5]    R. Zallen,  The Physics of Amorphous Solids.  A Wiley-Interscience  Publication, 1983, ch. 4.     [6]    A. Padovani, L. Larcher, O. Pirrotta, L. Vandelli and G. Bersuker, “Micro  Modeling of   $\mathrm{HfO_{x}}$    RRAM Operations: From Forming to Switching,”  IEEE Trans. Electron Devices,  vol. 62, no. 6, pp. 1998-2006, June 2015.    [7]    P. Huang, B. Gao, B. Chen, F. Zhang, L. Liu, G. Du, J. Kang and X. Liu,  “Stochastic Simulation of Forming, SET and RESET Process for  Transition Metal Oxide-based Resistive Switching Memory,” in  Proc.  SISPAD,  pp. 312-315, September 2012.

