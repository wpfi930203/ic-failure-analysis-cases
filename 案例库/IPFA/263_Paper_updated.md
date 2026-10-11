---
title: "263_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_ded52f7974db44e650155376cbccefa27295230462135641
file_size: 864338
---

## Characterization of Threshold-Voltage Hysteresis  and Instability in 4H-SiC Power nMOSFETs  

Yi Li Goh 1,2 , Chun Wei Khor 2 , Yuan Gao 2 , Voon Cheng Ngwan 2  1  School of Electronics and Data Engineering, Singapore Institute of Technology, 10 Dover Dr, Singapore    2  Technology Development and Introduction, STMicroelectronics, 28 Ang Mo Kio Industrial Park 2, Singapore  Phone: (+65) 6427 7501, Email:  2001532@sit.singaporetech.edu.sg

Abstract — The interface between silicon carbide and gate  oxide has long been studied and found to contain higher  interface traps. The higher intrinsic material defects coupled  with a wide bandgap introduces a phenomenon known as  hysteresis which is barely observed in silicon. According to  recommendations from JEDEC, applying a pulse near the  maximum gate-source voltage rating of the device prior to  measurement is known to reduce the threshold voltage  hysteresis. In this work, we present an innovation known as SVC  that achieved a uniform distribution of hysteresis values.  The  study on hysteresis and BTI revealed that both phenomena are  uncorrelated, and likely to have originated from different  sources.

Keywords— SiC, interface states, hysteresis, BTI

## I.    I NTRODUCTION 

Silicon Carbide (SiC) is seen as the next breakthrough for  high power semiconductor materials. SiC based Metal Oxide  Semiconductor Field Effect Transistor (MOSFET) is  increasingly used in renewable energy applications such as  traction inverter in electric vehicles, power converter in solar  panels where the robustness of the device at high temperature  and operating conditions is imperative to the reliability of the  device. Compared to its counterpart silicon (Si), SiC faces  many testing and reliability challenges, such as threshold  voltage   $\mathrm{(V_{th})}$   hysteresis and bias temperature instability (BTI)  [1-3].

With regards to hysteresis, basically Vth hysteresis   $(\Delta\mathrm{V_{th}})$    effect causes a quasi-permanent shift in threshold voltage  when the bias is swept in the opposite polarity. The shift can  be observed as a positive(negative) shift dependent on the  trapping mechanism capturing(emission) of charge carriers  [4] shown in Fig. 1.

![ID(A)  Capturingof trapped  charges  Emissionoftrapped  charges  VG(V)  vth  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/900b8fd2-1119-4e18-a8fb-c1eda6459211/900b8fd2-1119-4e18-a8fb-c1eda6459211.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215781%3B1743219381&q-key-time=1743215781%3B1743219381&q-header-list=host&q-url-param-list=&q-signature=604b73dbfd804a21ae96484038befa650ebb93dd)
Fig. 1. Capturing of charges and emission of charges with corresponding  right and left  $\mathrm{V_{th}}$   shift respectively

Hysteresis can be caused by extrinsic and intrinsic defects.  Extrinsic defects refer to particle contamination that can  corrode the gate oxide quality during device fabrication.  Intrinsic defects is linked to the inherent properties of the  interface involving interface states   $\left(\mathrm{{Dit}\right)}$   which can evolve to  oxide or interface traps. Research studies have shown that the  shift is mainly attributed to interface and oxide trapped  charges [4]. The 2-order of magnitude higher   $\mathrm{Dit}$   render

hysteresis a more critical issue in SiC than Si, resulting in  reliability testing challenges [5, 6].

During a device operation lifetime, the turn-on and turnoff Vth should not deviate from the stipulated values in the  datasheet for long-term stability. BTI causes parallel shift in  the transfer characteristic of a MOSFET, which can result in  undesirable effects. Under positive-BTI (PBTI), electron  trapping causes a positive shift which reduces the drain current  when the device is in the ‘ON’ state. Under negative-BTI  (NBTI), hole trapping occurs which causes a negative shift  and lead to parasitic turn-on when the device is in the ‘OFF’  state [7]. Since SiC power devices are used in switching  applications, assessing Vth degradation from BTI stress is  important since both polarity represents the device ‘ON’ and  ‘OFF’ state respectively.

JEDEC (JEP184) recommends applying a conditioning  pulse at near maximum gate-source voltage for a stipulated  timing (10-100ms) to characterize the effect of BTI by  bringing the charges to a reproducible conditioning state [8].  With conditioning,   $\Delta\mathrm{V_{th}}$   is expected to stabilize and not  fluctuate during subsequent measurements.  In this work, we  propose a different conditioning method known as Stepwise  Voltage Conditioning (SVC) that performed better results in  terms of stabilizing  $\mathrm{V_{th}}$   drift compared to JEDEC’s.

## II.   E XPERIMENTAL 

We fabricated a 650V SiC planar n-channel power  MOSFET with a   $550\mathrm{\AA}$   oxide thickness as shown in Fig. 2.  Nitric oxide (NO) gas was used during post-oxidation  annealing after thin oxide layer deposition to reduce  $\mathrm{Dit}$  . Also,   $\mathrm{H}_{2}/\mathrm{N}_{2}$   forming gas was introduced after metallization to  passivate extrinsic surface defects. The key processes in gate  oxide growth is also shown.

![Source   Source  SourceMetallization  Epi-growth  GateOxide  Sacrificialoxide  7+T   7十   layer  Body   Depositgateoxide  P+T  AnnealinginN2/0  gas  Drift Region  RCAclean  7+   Substrate  DrainMetallization  Drain  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bfd64e5a-19ec-494d-82b5-37375538caa6/bfd64e5a-19ec-494d-82b5-37375538caa6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215781%3B1743219381&q-key-time=1743215781%3B1743219381&q-header-list=host&q-url-param-list=&q-signature=7a3d03e9ca2249b5fe816d118c111f2da46d560d)
Fig. 2. Schematic of Power MOSFET detailing key oxide growth steps.

The evaluation of hysteresis is done by sweeping the  measurement bias as a function of the gate voltage according  to the DUT ratings. The  $\mathrm{V_{th}}$   extracted from upsweep  $(\mathrm{V_{up}})$   and  downsweep (V down ) is used to defined   $\Delta\mathrm{V_{th}}$   as follows:

$$\Delta\mathrm{V_{th}}\,{=}\,\mathrm{V_{down}\,{-}\,V_{u p}}$$
(1)

It is observed that hysteresis is generally at the highest  when the DUT is swept at a pristine state and drops to  relatively stable values in subsequent measurement.  Therefore,   $\Delta\mathrm{V_{th}}$   will be taken from the second reading of  every measurement for a more comprehensive analysis.

![VG(V)  ID(A) eepBias ts】  VG(V) VnVa   ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/53bc433c-52ec-49cd-afb5-8d81461a3b76/53bc433c-52ec-49cd-afb5-8d81461a3b76.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215781%3B1743219381&q-key-time=1743215781%3B1743219381&q-header-list=host&q-url-param-list=&q-signature=54c4c31fe121ed741e76bec357b031ffde3a8e23)
Fig. 3. Gate bias staircase upward and downward sweep (left) with shifting  of  $\mathrm{V_{th}}$   due to hysteresis (right).

To alleviate   $\mathrm{V_{th}}$   hysteresis, according to JEDEC  recommendation, applying a high voltage pulse at the gate  can reduce   $\mathrm{Dit}$  , thereby minimizing the hysteresis effect. The  pulse retriggers the dormant interface states by supplying a  high enough potential energy, causing the traps to capture and  settle into an equilibrium state upon removal of stress [8].  Instead of using JEDEC method, a novel innovation known  as SVC is used to condition the DUT.

Contrary to JEDEC constant pulse, SVC utilizes a step-up  voltage from the device maximum operating range (18V) and  incrementing it by 2V until it reaches the absolute maximum  value (22V) for a duration of 100ms at each step. The method  and their implementation is figuratively shown in Fig. 4.

![VG(V)  JEDEC  VG(V)  sVC vgs_m 22w 201w L8W t（s）  t（s] 100ms  1ooms   ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/229bd313-a24c-44a9-9fb3-af5aecfe1c57/229bd313-a24c-44a9-9fb3-af5aecfe1c57.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215781%3B1743219381&q-key-time=1743215781%3B1743219381&q-header-list=host&q-url-param-list=&q-signature=b9e54fc63c8ab3a60ac06f491a035bfff379a43f)
Fig. 4. JEDEC constant pulse conditioning method (left). A novel method  known as SVC to condition DUT is proposed (right).

The PBTI phase (Fig. 5) includes a measure-stressmeasure (MSM) approach. First,   $\mathrm{V_{th}}$    of the DUT is measured  prior to stress. Next, SVC was applied to condition the DUT  to stabilize  $\mathrm{V_{th}}$   drift. PBTI is then performed by applying gate  voltage of 35V for 10ks following SVC conditioning. After  PBTI, the DUT is left at idle state for 10ks to see if drift  recovers to prestress value. Finally, negative recovery is done  at -5V for 10ks and the DUT is measured for its final   $\mathrm{V_{th}}$   drift  value. PBTI will be performed at room temperature and high  temperature to investigate the effect of temperature along with  high positive voltage on hysteresis and BTI.

![ApplySvo  eepovto   Sweepovto   weepovto   Sweepovto   sweepOvto  35V for 10ks stres  18Vtwo times  PBTI  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/183782a2-cca3-4196-84f0-6e74f149f75e/183782a2-cca3-4196-84f0-6e74f149f75e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215781%3B1743219381&q-key-time=1743215781%3B1743219381&q-header-list=host&q-url-param-list=&q-signature=40d9ce93e6c6a004fa197d64c4031665633a9f84)
Fig. 5. PBTI measurement procedure.

## III.   R ESULTS  &  DISCUSSION   

In the subsequent sections, we present our experimental  findings. The evaluation of SVC compared to JEDEC is  reported first, followed by the evaluation on hysteresis and  finally, PBTI analysis result.

## A.   Hysteresis  

Hysteresis was found to decrease after conditioning with  voltage pulse applied at the gate. The reduction in   $\Delta\mathrm{V_{th}}$   can  be done through SVC while the remaining   $\Delta\mathrm{V_{th}}$   is attributed  to permanent deep level traps. The impact of using SVC and  JEDEC as conditioning method is depicted in Fig. 6 and 7.

![140   △Vbeforeand afterJEDECconditioning  POSt  100  uu)  40  20  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4549eabc-b3c5-4063-be37-6cc06e331881/4549eabc-b3c5-4063-be37-6cc06e331881.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215781%3B1743219381&q-key-time=1743215781%3B1743219381&q-header-list=host&q-url-param-list=&q-signature=ea8b09bb5a45a1ddaed5a26a0a0818bd306d9a3a)
Fig. 6. ΔV th  measured pre and post JEDEC conditioning.

![140   △Vth before and after SVC conditioning  Pre  120   Post  100  80  60  40  20  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/addc3f47-f437-42fc-8418-0a02102bfc38/addc3f47-f437-42fc-8418-0a02102bfc38.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215781%3B1743219381&q-key-time=1743215781%3B1743219381&q-header-list=host&q-url-param-list=&q-signature=80cd85551fad9a3c20a124f085f7ff5d0f4d07f2)
Fig.  $7.\,\Delta\mathrm{V_{th}}$   measured pre and post SVC conditioning.

It is evident that both methods reduced the similar amount  in terms of   $\Delta\mathrm{V_{th}}$   but a notable distinction was that SVC led to  stabilization of  $\Delta\mathrm{V_{th}}$   values,whereas JEDEC standard method  created considerable variation in   $\Delta\mathrm{V_{th}}$   measurements. This  can easily be observed in the statistical chart shown in Fig. 8.

![StandardDev.ofAVtAfterConditioning  Pre  Post  (ne)  Ps  JEDEC   SVC  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fcc1f82b-c838-4c11-9eeb-1899cf382015/fcc1f82b-c838-4c11-9eeb-1899cf382015.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215781%3B1743219381&q-key-time=1743215781%3B1743219381&q-header-list=host&q-url-param-list=&q-signature=090b9903d80f5ed3fab96f69a9631fedccc4cc24)
Fig. 8. Standard deviation across statistical location after subjecting to  JEDEC and SVC conditioning respectively.

Defects in the lattice site can be classified according to  their energy level properties with regards to the bandgap;  either shallow traps or deep traps [9]. Shallow traps are  believed to be in localized clusters (near-interface traps,  interface traps etc.), while deep level traps (oxide traps/border  traps) are known to spread in unlocalized manner. The  presence of border and interface traps near the SiC/SiO 2 interface results in the formation of energy states within the  bandgap, which has significant implications for the  performance and reliability of SiC-based devices. Comparing  the bandgap of Si (1.12 eV) and SiC (3.3 eV), there is a higher  probability that interface states lie within the range in SiC due  to the wide bandgap nature of the material [10]. Coupled with  the high density of point defects in SiC, it exacerbates the issue  of threshold voltage variation even more so in SiC than Si.

The traps can cause variations in  $\Delta\mathrm{V_{th}},$  , due to releasing and  capturing of charge carriers associated with them (Fig. 1). A  decrease in   $\Delta\mathrm{V_{th}}$   is attributed to the emission of trapped  charges from traps, indicating an increased supply of charge  carriers that allows the formation of the inversion channel to  be achieved faster [11]. Conversely, capturing charges by  traps would reduce the supply of charge carriers in the  channel, thereby increasing   $\Delta\mathrm{V_{th}}$   since more time would be  required for the formation of inversion channel.

It can clearly be observed that SVC method has a smaller  spread post-conditioning as compared to JEDEC. The use of  SVC improves stability with std dev reducing by nearly   $70\%$  .  SVC works on the same principle as JEDEC in terms of  utilizing a voltage pulse applied at the gate to recondition  interface states and allow them to settle into a state of  equilibrium. However, the key difference is that SVC uses a  voltage ramp-up approach which allows charges to be settled  uniformly in an equilibrium manner [12]. This results in the  consistent  $\Delta\mathrm{V_{th}}$   which we observe post-SVC that is not found  in post-JEDEC.

![SiO2  SiC(n-type) an Oxidetraps/NITs Releasine nterfacetraps  E。=3.3eV Atequilibriumstate(nobiasappliedatgate） sio,  SiC(n-type) idetraps/NiTs ee otelectrons fhole Whenpo  atthegate ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4c5fe562-5152-49d0-92ae-bdccc912061a/4c5fe562-5152-49d0-92ae-bdccc912061a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215781%3B1743219381&q-key-time=1743215781%3B1743219381&q-header-list=host&q-url-param-list=&q-signature=5456e0f83afa6da6c82e594d36a5e98171411f66)
Fig. 9. Energy band diagram in relation to the oxide and n-type substrate  structure with traps activity and filled traps shown in black.

The model in Fig. 9. shows how trapping mechanism  works with respect to the energy properties of the Fermi level  (EF). At equilibrium state (no bias), capturing of charges  occurs when the energy level of the traps is lower than EF.

Conversely, emission of trapped charges happens when the  trap has a higher energy level than E F .

In our experiment, SVC stress caused band-bending which  resulted in accumulation of electrons near the interface layer  (Fig. 9 (b)). The application of incremental step-up stress bias  allowed interface states to release previously trapped charges  and stabilized  $\Delta\mathrm{V_{th}}$  value to produce repeatable results [8].

## B.   Positive Bias Temperature Instability (PBTI)  

We performed PBTI stress at room and high temperature  by stressing the DUT at the gate with a bias of 35V for 10ks.  Fig. 10. shows the   $\Delta\mathrm{V_{th}}$   comparison between room and high  temperature. It is observed that   $\Delta\mathrm{V_{th}}$   at room and high  temperature follows the similar trend while   $\Delta\mathrm{V_{th}}$   at high  temperature is generally lower than at room temperature.

![Vacrossdifferent temperatureprofile  25°C  100°C  PreStress   svC   PBT   zero   Negative  Recovery   Recovery  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/af246b85-10c1-4f3b-8e78-3f43576a7e56/af246b85-10c1-4f3b-8e78-3f43576a7e56.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215781%3B1743219381&q-key-time=1743215781%3B1743219381&q-header-list=host&q-url-param-list=&q-signature=c14e8fceb769e8979810c824c1e20f214360337b)
Fig. 10. ΔV th  measured across different phases of the measurement sequence  at different temperatures.

![SiOz   SiC(n-type)  citationot   Ec=3.2eV  electronsinto  Seneration  ewtraps  When positive bias applied at 373K     ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/51ba8354-de19-40d5-a646-1b87d5c403c3/51ba8354-de19-40d5-a646-1b87d5c403c3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215781%3B1743219381&q-key-time=1743215781%3B1743219381&q-header-list=host&q-url-param-list=&q-signature=c74efd4b81073c4f6d5597124ecc2d212a140094)
Fig. 11.   Generation of new traps along with electrons excitation at high  temperature and bandgap shrinkage.

With the application of thermal stress, it causes further  shrinking of the forbidden bandgap, along with excitation of  electrons from the valence band (E V ) into conduction band  (E C ) [13]. Thus, the increased supply of electrons lowers ΔV th ,  which is consistent with the mechanism in Fig. 1 and observed  in Fig. 10.

![PBTITestatRoomTemperature  10-  Prestressup  Prestress down  svcup  svcdown  PBTIup  PBTIdown  Zeroup  Zerodown  Negativeup  Negative down  14  l  20   21   2.2   2.3   2.4   2.5   2.6   27  GateVoltage  Vv)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/37ca53e0-a78c-4ed0-bd35-ddc8f8abd9c0/37ca53e0-a78c-4ed0-bd35-ddc8f8abd9c0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215781%3B1743219381&q-key-time=1743215781%3B1743219381&q-header-list=host&q-url-param-list=&q-signature=9a0e16bcc4c27a8548a2ce75d337603d223e9a6c)
Fig. 12.   Parallel shifting of   $\Delta\mathrm{V_{th}}$   at room temperature following PBTI stress  with   $\mathrm{V_{up}}$    (solid line) and   $\mathrm{V_{down}}$   (dash line) referenced at   $\mathrm{{ID}{=}210\upmu\mathrm{{A}}}$  .

Fig. 12. shows PBTI test result at room temperature swept  from 0V to 18V. Parallel shifting of the transfer characteristic  curve was observed both during after PBTI stress and recovery  phase. An analogous observation was also made for PBTI test  at high temperature. Thus, this implies that the BTI stress at  room or high temperature is not linked to the threshold voltage  hysteresis that is observed in the DUT due to the parallel  shifting of both  $\mathrm{V_{up}}$   and V down  after BTI stress and using SVC  as a precondition method.

## IV.   C ONCLUSION 

In the present study, we characterized threshold voltage   related behaviors, specifically hysteresis and PBTI, in SiC  power nMOSFETs. Our investigation into hysteresis  demonstrated that through the application of SVC  preconditioning, it is possible to further minimize hysteresis  effects. This preconditioning resulted in a more uniform  distribution of   $\mathrm{V_{th}}$   and a substantial reduction in the standard  deviation by up to   $70\%$  . These findings provide a solid  foundation for future research in the area of BTI phenomena.  The methodologies and insights gained from this study have  the potential to significantly influence subsequent BTI  investigations and to be integrated into advanced SiC power  nMOSFETs design strategies.

## A CKNOWLEDGMENT 

The authors would like to thank M. K. Teoh for device  fabrication, T.C. Lee and M. Castorina for project  sponsorship.

## R EFERENCES 

[1]    T. Okayama, S. D. Arthur, J. L. Garrett, and M. V. Rao, “Bias-stress  induced threshold voltage and drain current instability in 4H–SiC  DMOSFETs,”  Solid-State Electronics , vol. 52, no. 1, pp. 164–170, Jan.  2008, doi: 10.1016/j.sse.2007.07.031.     [2]    K. Matocha, “Challenges in SiC power MOSFET design,”  Solid-State  Electronics , vol. 52, no. 10, pp. 1631–1635, Oct. 2008, doi:  10.1016/j.sse.2008.06.034.     [3]    R. Arora  et al. , “Charge Trapping Properties of 3C- and 4H-SiC MOS  Capacitors With Nitrided Gate Oxides,”  IEEE Transactions on Nuclear  Science , vol. 56, no. 6, pp. 3185–3191, Dec. 2009, doi:  10.1109/tns.2009.2031604.     [4]    P. Fiorenza, F. Giannazzo, and F. Roccaforte, “Characterization of  SiO2/4H-SiC Interfaces in 4H-SiC MOSFETs: A Review,”  Energies ,  vol. 12, no. 12, p. 2310, Jun. 2019, doi: 10.3390/en12122310.     [5]    A. J. Lelis, R. Green, D. B. Habersat and M. El, "Basic Mechanisms of  Threshold-Voltage Instability and Implications for Reliability Testing  of SiC MOSFETs," IEEE Transactions on Electron Devices, vol. 62,  no. 2, pp. 316-323, 2015.    [6]    S. T. Pantelides, S. Wang, A. Franceschetti, R. Buczko, D. V. M., S.  N. Rashkeev, . L. Tsetseris and M. H. Evans, "Si/SiO2 and SiC/SiO2  Interfaces for MOSFETs –Challenges and Advances,"  Materials  Science Forum,  vol. 527, pp. 935-948, 2006.    [7]    T. Aichinger, G. Rescher and G. Pobegen, "Threshold voltage  peculiarities and bias temperature instabilities of SiC MOSFETs,"  Microelectronics Reliability, vol. 80, p. 6878, 2018.     [8]    JEDEC , "Conversion, Guideline for Evaluating Bias Temperature  Instability of Silicon Carbide MOS Devices for Power Electronic,"  JEP184, pp. 1-44, 2021    [9]    P. YU and M. Cardona,  Fundamentals of Semiconductors: Physics and  Materials Properties . Springer Science & Business Media, 2010.     [10]   D. M. Fleetwood  et al. , “Effects of oxide traps, interface traps, and  ‘“border traps”’ on metal-oxide-semiconductor devices,”  Journal of  Applied Physics , vol. 73, no. 10, pp. 5058–5074, May 1993, doi:  10.1063/1.353777.     [11]   B. Asllani, A. Castellazzi, O. A. Salvado, A. Fayyaz, H. Morel, and D.  Planson, “VTH-Hysteresis and Interface States Characterisation in SiC  Power MOSFETs with Planar and Trench Gate,” in  2019 IEEE  International Reliability Physics Symposium (IRPS) , Mar. 2019.  Accessed:   Mar.   26,   2024.   [Online].   Available:  http://dx.doi.org/10.1109/irps.2019.8720612     [12]   G. Rescher, G. Pobegen, T. Aichinger, and T. Grasser, “On the  subthreshold drain current sweep hysteresis of 4H-SiC nMOSFETs,”  in  2016 IEEE International Electron Devices Meeting (IEDM) , Dec.  2016.   Accessed:   Mar.   26,   2024.   [Online].   Available:  http://dx.doi.org/10.1109/iedm.2016.7838392     [13]   W. J. Choyke, “Optical Properties of Polytype of SiC: Interband  Absorption, And Luminescence of Nitrogen-Exciton Complexes,” in  Silicon Carbide–1968 , Elsevier, 1969, pp. S141–S152. Accessed: Mar.  26, 2024. [Online]. Available: http://dx.doi.org/10.1016/b978-0-08- 006768-1.50018-8

