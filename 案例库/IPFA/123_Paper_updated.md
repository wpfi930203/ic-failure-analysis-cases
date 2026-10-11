---
title: "123_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_50efa88edc30cc92953dc9d099e1849f7295230462135641
file_size: 2765393
---

## Analysis of Failure Mechanisms Occuring at  Breakdown Voltage in power p-GaN HEMT  

Lucien Ghizzo 1,2,3 , David Trémouilles 2 , Gérald Guibaud 1 , Christophe de Nardi 1 , Vanessa Chazal 1 , Hélène Chauvin 1 , François Jamin 1 ,  Frédéric Richardeau 3   1 THALES SIX France SAS, Toulouse, France  2 LAAS-CNRS, Toulouse, France   3 LAPLACE, Toulouse, France   Phone : (+33) 0627608983, Email: lucien.ghizzo@gmail.com

Abstract — This   study   focuses   on   the   drain-source  breakdown voltage (V BR ) of 100 V commercial p-GaN  transistors. By presenting V BR  values, showcasing device  dispersion, and employing failure analysis (FA), we explore  various physical degradation mechanisms. Investigating the  degradation process from origin to defect manifestation  enhances our understanding of GaN transistor limitations.   Additionally, the paper highlights the adaptation of FA  methodology based on defect nature, providing valuable insights  for semiconductor device reliability improvement.

Keywords—voltage breakdown, reliability, failure mechanism,  GaN power transistors.

## I.    D EVICES USED AND STRESS APPLIED   

The devices under test (DUT) are commercial,   $100\;\mathrm{V}$  ,  90 A, 7 mΩ packaged p-GaN gate AlGaN/GaN HEMT of part  number 1 (devices δa to δi in Table I) and 100 V, 36 A 16 mΩ  packaged p-GaN gate AlGaN/GaN HEMT from the same  manufacturer and called part number 2 (devices ωa to ωd in  Table II). The ε devices are from another manufacturer  their  ratings are unpackaged naked die with solder bumps of ratings  100 V, 16 A, 7 mΩ.

The drain-source voltage (V DS ) and the gate-source  voltage (V GS ) are applied with a Keysight  B1505A power  device analyzer/curve tracer connected with probe needles  landed on the package electrodes.

V DS  is sweeped up until the breakdown voltage value  (V BR ) is reached which is the V DS  value when the drain  leakage current  $\mathrm{I_{dss}}$    increases abruptly (see Fig. 1).

T ABLE  I.           T ABLE OF BREAKDOWN VOLTAGE VALUES PART  NUMBER  1:   100   V,   90   A,   7  M Ω

|Part Num.1  device n. :|Setup|V DS = V BR|Expected degradation|
|---|---|---|---|
|δa|V GS  = 0 V|154.6 V|DS leakage FP|
|δb|V GS  = 0 V|123.8 V|DS leakage FP|
|δc|V GS  = 0 V|144.5 V|DS leakage FP|
|δd δe|V GS  = 0 V|165.9 V 161.6 V|DS leakage FP DS leakage epitaxy|
|δf|V GS  = 0 V|158 V|DS leakage epitaxy|
|δg|V GS  = 0 V|150.4 V|DS leakage epitaxy|
|δh|V GS  = 0 V|162.7 V|DS leakage epitaxy|
|δi|V GS  = 0 V|157.9 V|DS leakage epitaxy|


## II.   T WO TYPES OF DEGRADATIONS 

The δ devices tested in drain source voltage have two  different electrical breakdown signatures. One is a complete  failure of the device, immediate and not recoverable, the  device after the breakdown voltage measurement cannot be

used in an application due to very high leakage current at low  voltage bias. The other one is only degraded (not severely  damaged) after V BR , a second and even more other breakdown  voltage measurement can be performed on the device. The  leakage current of these device only change for high drain  voltage (above 120 V).

## A.   Immediate degradation, complete failure  

The δ devices that failed entirely at first attempt are the  devices a to d. The V DS  limits in the same range of value ie  between   $123~\mathrm{V}$   and   $166~\mathrm{V}$   as visible in table I. δa was less  degraded thanks to the use of a serial resistance that limits the  default current after V BR  (max of  $500\,\upmu\mathrm{A})$   and δb,c and d were  more degraded due to a higher current limit after breakdown  voltage (8 mA) and the removal of the serial resistance.

The breakdown corresponds to an increase of the DS  leakage current.  For these four devices the V BR  measurement  leads to a complete failure of the device in a single sweep.  When the drain voltage sweep is done again (V BR  2) on the  same device the resistance of the device is severely reduced  and therefore the current leakage is significantly increased as  it can be seen on the dashed lines of Fig. 1. The backward  sweep of the hysteresis of device δa shows a significant  reduction of the resistance of the device too.

![10-3  10-5  SSD  10-7  6a1   5b2  5b1   6c2  10-9  Sc1   8d2  od1  50   100   150   200  VDs(V)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/878f2758-e24b-4ed5-9d03-72d9ad2f5b0c/878f2758-e24b-4ed5-9d03-72d9ad2f5b0c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=815867e9162df24453d119cb56213136e8d4ef32)
Fig. 1.  Electrical signatures of the V BR  for devices δa,b,c and d. The drain  current leakage increases abruptly at the  $\mathrm{V_{BR}}$   reached at at 154.6 V, 123.8 V,  144.5 V and 165.9 V for the respective device. The dashed lines show the  signature after  $\mathrm{V_{BR}}\,1$  . The blue curve of device a shows with the hysteresis a  change of leakage current on the forward sweep (increase by two orders of  magnitude). The increase in drain leakage current is expected to be a drain  source leakage current.

## B.   Degradation occurring at higher drain voltage    

The other devices of the same part number in the same  stress conditions (current limit at 8 mA, no serial resistor), δe  to δi did not lead to complete failure after performing a first  V BR  measurement.

As it can be observed for transistor δe in Fig. 2a,b the  curves of   $\mathrm{V_{BR}}\ 2.4$   overlap with the curve of V BR  1 under   $\mathrm{V_{DS}}{=}120\;\mathrm{V}$  . Nevertheless a degradation has appeared after

V BR  1 as the increased of leakage current can be seen at a  smaller voltage in the next V BR  measurements. A leakage path  has then been formed after  $\mathrm{V_{BR}\,1}$  , the resistance of the leakage  changes in the subsequent V BR  measurements (particularly  between V BR  2 and V BR  3 respectively in pink and orange in  Fig. 2a above 140 V) due to the addition of other leakage path  in the device that will be showed later.

The devices δf-i (Fig. 2c) showed the same degradation  behavior that δe. The gate current during V BR  did not change  at all, the gate stack nor the gate region seem affected in this  case, a degradation is expected to be located in the drain  region of the device. The device characteristics is still in the  ratings, still operate correctly and could be used in a power  application according to the manufacturer datasheet despite a  change of V BR  curve showing a degradation of the device.

![oe1  2.00  se1 10—4  6e2  1.75  6e2 6e3  6e3 1.50 6e4  6e4 10-6  1.25 1.00 SSD LO  \$0.75 0.50 10-10  0.25 a  0.00 50  100  150  200  100120140160180200 VDS(V)  VDS(V) 10-3 10-3 1O一 1O-  SSpI 1O Cd 6f1 10- 1O一 591 妈b1  wb2 6h1 JC1 10-11  C  61 Jd2 SO  10O  150  200  SO  10O  L50  200 VDs(V) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/20d73973-2b91-4f85-af95-18d276d2550b/20d73973-2b91-4f85-af95-18d276d2550b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=2bf9642c01f26215d0648200a695ec1746afeb52)
Fig. 2. Electrical signature of the repeated V BR  (1,2,3 and 4) for devices δe,  other V BR  measurements were performed after the first one to study the  propagation and evolution of the V BR  defect. No degradation was noticed  after the first attempt like the devices on Fig. 1 (a) log display, (b) linear  display, (c) Electrical signature of the first   $\mathrm{V_{BR}}$  of the devices δf to δi, (d)  Electrical signatures of the ω devices.

The other part number devices (ωa to ωd) did not fail  entirely as well after   $\mathrm{V_{BR}}\ 1$   like δf-i, the   $\mathrm{V_{BR}}$   is in the same  range than δ devices (δe to δi), see Table II. However, a steep  increase of leakage current occurred at a smaller V DS  voltage  (see Fig. 2d: 90 V for   $\mathrm{V}_{\mathrm{BR}}\,2$   instead of   $150~\mathrm{V}$   for  $\mathrm{V_{BR}\,1}$  ). None  of the device of this part number showed degradation  mechanisms presented in section A with  $\mathrm{VGS}=0~\mathrm{V}$     (gate-drain  leakage current).

T ABLE  II.         T ABLE OF BREAKDOWN VOLTAGE VALUES FOR  PART NUMBER  2:   100   V,    36   A,   16  M Ω

|Part Num.2 device n. :|Setup|V DS = V BR|Expected degradation|
|---|---|---|---|
|ωa|V GS  = 0 V|146.2 V|DS leakage epitaxy|
|ωb|V GS  = 0 V|146.9 V|DS leakage epitaxy|
|ωc|V GS  = 0 V|165.1 V|DS leakage epitaxy|
|ωd|V GS  = 0 V|141.8 V|DS leakage epitaxy|


![ 10-3  1O一 Reversible chargeeffect 1O一  1O一 \$10-  %10- eai  Ea4 10-6  10- a2  Ea5  ∈b1 ea3  Ea6  ∈b2 10- 10- 50  100  150  200  50  100  150 VDS(V) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/522547fd-5108-47cb-a344-2b8e9d4d71d0/522547fd-5108-47cb-a344-2b8e9d4d71d0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=69c0136857ed4e1b5eb2f94e41268950fca53239)
Fig. 3. (a) Electrical signatures of the drain leakage current at high polarization  when looking for the V BR  of ε devices. No change can be observed after the  repetition of the high polarization.  The power is limited by the tracer SMU to  reach a flagrant degradation. (b) Example of charge leak out at high  polarization that generate a shift of the leakage increase knee. The  phenomenon does not seem to be related to a degradation as it is reversible.

The other manufacturer's devices (devices ε, 6 devices  tested in total) did not fail as the devices of section IIA, the  leakage increase knee is stable and does not seem to be  affected with the reproduction of the V BR  measurement stress  (Fig. 3a).

However, some instabilities of the operating point were  observed in the increased leakage current part near   $180~\mathrm{V}$   as  visible in Fig. 3b. As the current increased, some reversible  voltage reduction was observed, indicating an avalanche-like  phenomenon that is expected to be related to the charge  trapping/detrapping effect.

The leakage current is expected to be related to  dislocations and as explained in [3], the additional leakage  current resulting from trapping/detrapping effects may come  from ionized carbon acceptors in nitrogen sites which may  favor Poole-Frenkel emission process. The emission process  can lead to the discharge of stored charges in the buffer, which  add up to the leakage current that goes through dislocation  defects.

The energy of the B1505A's Source Measurement Units  (SMUs) is not sufficient to produce visible degradation on the  device, as compliance is reached very quickly once the  leakage rise knee is reached. A higher power current  controlled SMU was used to reach the true breakdown  voltage. This experiment is performed while measuring the  photons emitted with Photon Emission Microscopy (PEM).

The operating point to reach the drain voltage limit of the  device is controlled by the current value, which is increased  step by step. A first emission spot appears in zone 1 in Fig. 4,  which means that the leakage current at high voltage observed  in Fig. 3 is more intense locally in the structure.

After increasing the current and then the power in the  structure, this spot disappears and another one appears in the  lower right corner of the device (zone 2 in Fig. 4b). A defect  is now visible in zone 1 near the bump and the whole structure  can still be polarized with high voltage (195 V).

The increase in leakage current controlled by the SMU  resulted in a complete failure near 20 mA. After this step, high  polarization is no longer possible as a few volts resulted in a  very high leakage current, indicating the formation of an  electrical short within the structure.

![Before failure at  199V,5mA  Leakage zone 1  Previous  leakage zone 1  eakage zon  After failure at 195 V, 10 mA  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e0228441-7dab-4caa-8522-f9c173754689/e0228441-7dab-4caa-8522-f9c173754689.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=055dfd50fde85551075946d024d6e1f846c3e574)
Fig. 4. PEM in frontside during the V BR  measurement of ε devices. A first  emission spot is visible in zone 1 a the top right corner of the device and a  second one appeared at the bottom right corner of the device with the  increase of the leakage current after the first one disappeared.

Devices (both δ and ω) stressed with   $\mathrm{V}_{\mathrm{GS}}{=}{3}\ \mathrm{V}$   have the  degradation mechanism of section A which is a gate drain  leakage current in the gate area. These stress conditions are  interesting to study as this gate voltage is advised in  application by the manufacturer at off-state.

## III.   N ATURE OF DEFECTS   

## A.   Electrical short in the passivation region  

For the device δa, a backside approach was performed as  described in [1]. A focused ion beam (FIB) cross-section  (Fig. 5) revealed a metallic shunt that electrically short the  drain (the 2DEG) and the source (field plate metal). The  melting of the field plate metal is induced by the high electric  field, which generates a metal filament.

Fig. 6 shows the consequence of an up to V BR  sweep for  a device were the limiting serial resistance is removed (δd),  which is the situation that will be encountered in a real  application. The FP melted on a much larger area due to the  higher energy. The consequence is that all electrodes are then  shorted together.

![#8a   defect  metal filament  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/130f0c89-adf1-4d75-a7d6-7bab66e42c9c/130f0c89-adf1-4d75-a7d6-7bab66e42c9c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=d7f869aa7ef6747925500f85fbff2736d4557a83)
Fig 5. FIB cross-section in the defect region of device δa (breakdown energy  limited with the serial resistor). The drain source electrical short seems to  originate from the melting of the metal field plate that reached the drain  electrode through the 2DEG.

![ca   C   C  cracks  Drainmetal   molten fielc   plate  pheric)  fieldplat  Zoneof  hotspot  Sourcemetal  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/862dae67-a09e-45e0-a2d5-6675f71c8d9f/862dae67-a09e-45e0-a2d5-6675f71c8d9f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=6ff74b4f36c449663439814179e8eb359b6fbace)
Fig. 6. (a) IR LIT Localization of defect of device δd (no serial resistance  during V BR ). A hotspot is visible on the field plate metal area near the drain.  A black spot start from this point and expand above it which shows the  propagation of the defect. (b) Zoom of the defect zone. The metal structure  is visible from the backside through the GaN layers. The short led to the  melting of the field plate metal.

## B.   Failure expected to be caused by dislocations issues  

##       δ device: leakage through dislocations   

![a   ab  CCD  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/08a15fd8-707a-4b64-91fe-a25ddbc15d43/08a15fd8-707a-4b64-91fe-a25ddbc15d43.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=6d706fa963c775e3053f245e8c22ca83c7a6b9ea)
Fig. 7. (a) Defect localization for device δe. A spot is visible between the  field plate metal and the drain metallization. (b) IR 71x zoom camera of the  defect zone. A black spot is visible on the drain metallization (above the drain  contact, probably in the GaN layer as it is a backside observation). (c) Defect  localization with 10x magnification of device δe, four emission spots are  visible on the edges of the active zones.

The devices that did not break after V BR  1 (δe to δi ; ωa to  ωd and ε devices) are suspected to have experienced vertical  leakage current degradation through the GaN layer near the  drain metal. The failure in the epitaxy compared to the  previous case in SiN is attributed to differences in the random  layer process quality that selects the stress weak spots within  the structure (either SiN or GaN).

Photon emission microscopy (PEM) localization was used  to identify the areas of leakage current. The number of  observed spots appears to increase with the number of V BR   sweeps carried out on a device, particularly with the number  of shape changes in the leakage current. A significant change  in resistance between two V BR  at a certain V DS , such as at   $140~\mathrm{V}$   in Fig. 2b, is expected to generate a new leakage path  and spot within the device (Fig. 7d). Devices that underwent  only one V BR  sweep have only one spot.

The first defect produced by V BR  1 does not seem to evolve  at V BR  2 or the subsequent ones. Indeed, this defect's is a  leakage current and it is still possible to increase the electric  field throughout the device and lead to new defects elsewhere  in the transistor. This explains Fig. 7c and the four emission  spots instead of only one spot that is getting bigger after  performing again V BR  sweep.

A dark spot is visible with IR microscopy at each emission  spot location (see Fig. 7b for δe). A big defect could be  expected as the defect is visible at this step, however this spot

is not visible with other microscopes that have a different focal  length.

The defect is within the GaN layers and does not seem to  affect the metals of the active zone, as observed by changing  the focus distance. The defect's electrical signature, previously  observed under different stress conditions [1], suggests that  the leakage path may be caused by dislocations generated by  a sufficient electric field [4].

The observed leakage current is likely due to a TimeDependent Dielectric Breakdown mechanism [2,3]. The dark  spots observed (on IR microscopy images) indicate a visible  evolution of the transistor. There may be a change in  crystalline properties due to an increase in the concentration  of another element such as aluminum for instance near the  leakage path.

![100Lm  Aboallylagtchpits  located onlyhere onthedevic  Etch pit type  located  Previous Drain location   everywhere  on the whole  surface  Previous Source location  EHT=2.00kV   SignalA=SE2   Vit.Balayage=9   Date:23Nov2023  WD=5.5mm   Grand.=2.00KX  1Sonde=244pA  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/041cc27c-782c-4b67-b5ec-7b8dcd170473/041cc27c-782c-4b67-b5ec-7b8dcd170473.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=de6be27931e2d80a9f9650226f3ee6eede78bf9e)
Fig. 8. (a) Optical view of the surface of the transistor after chemical etching  with ortho phosphoric acid  $\mathrm{(H_{3}P O_{4})}$  , the small black dots on the whole surface  are etch pits of revealed dislocations. On the left of the picture the bigger etch  pits aligned of (b) are visible. (b) SEM observation of the GaN layer in  frontside circle in red in Fig. 7a. Etch pits of some the dislocations are visible  on all the surface (yellow arrows), however on one border of the active zone,  the pits are larger and aligned on the edge of the previous drain metal location  (white arrows).

In our previous study in [1] we did obtain a similar  electrical signature of degradation for a switching voltage  stress. We found in this paper that the density of dislocations  seemed to increase due to the stress with the observation of  TEM lamellae and conductive Atomic Force Microscopy  (AFM) experiments. However this paper was inconclusive as  many dislocation are already present before stress and  differentiate them with stress produced one is complicated.

This paper investigates a less expensive and timeconsuming approach to observe defects in the metal location.  The device was studied by removing the varnish and the first  layer of copper with nitric acid from the front side. The  process began with a dip in hydrofluoric acid etching (dip HF)  to remove the metal and oxide layers, leaving only the silicon  substrate, the GaN buffer, the AlGaN barrier, and the p-GaN  cap.

Next, the sample was revealed with heated H 3 PO 4  at   $130\,^{\circ}\mathrm{C}$   for 10-20 minutes to remove the p-GaN and AlGaN  layers. The surface of the GaN buffer revealed some of the  dislocations through etch pits that were uniformly observed.

However, a different pattern is observed on the stressed  device (device δd that was stressed under the same conditions  as δe). The etch pits are aligned on the border of a drain metal  edge localization on the border of the active area of the device  where the emission spots are often observed (see Fig. 7c). The  pits are larger than the others (2 to   $3~{\upmu\mathrm{m}}$   versus   $1\;\upmu\mathrm{m}$  , as  shown in the SEM image in Fig. 8).

The line of different etch pits was observed only on  stressed devices and not on pristine ones. The chemical  conditions are difficult to maintain as the chemical revelation  is a very unstable and variable process. Only a third of the  stressed devices tested show this pattern and none of the  pristine ones.   $\mathrm{VGS}\,{=}\,0~\mathrm{V}$

The larger aligned pits may correspond to conductive  dislocations. The larger size of dislocations may be attributed  to the presence of aluminum impurities brought by Cottrell  clouds, which accelerate the etching process locally [6]. The  presence of aluminum impurities can reduce the electrical  isolation of the buffer layer. Furthermore, deeper dislocations  may cause more significant etching [7], resulting in a thinner  electric isolation layer and increased leakage current at high  voltage drain values.

## εa device: high energy defect 

The other manufacturer's devices (ε devices) do not lead  to the defect presented in Sections IIA and IIIA thanks to a  different design choice. In fact, the drain-source electrical  isolation is mainly done in two regions inside the structure,  under the field plate edge on the drain side and the GaN buffer  layer. The electrical isolation varies with the thickness of the  materials used, the doping, the type and the doping  concentration of the device.

While the voltage boundaries of these two regions are  quite close for δ devices, resulting in two distinct failure  modes, the addition of a second field plate (FP2 in Fig. 9)  further from the channel results in a unique failure mode for ε  devices. This failure is in the GaN layer below the drain metal.

![Drain  Source  FP2(S)  FP1  Gate  WHT-3.8mmV   Sianai A =4S:020 K X   VitoBalayag244 pA   Date :19 Mars 2024  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2f868001-36d1-499b-bc7d-77bedeb2c6b3/2f868001-36d1-499b-bc7d-77bedeb2c6b3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=3456cdc6582c34df299b44dd6150fdba17888343)
Fig. 9. SEM image of the cross section of the gate region of ε devices .  The  second field FP2 improve the electrical isolation drain source between the  field plate FP1 and the channel region.

The current leakage through the GaN layer is expected to  be related to dislocations in the structure, as explained for the

δ devices of B. The appearance of the second emission spot in  fig.4 could be the generation of a new leakage path and  perhaps new dislocations, as in the case of the δ devices.

The increase of the current in the vertical path originating  from dislocations in GaN (new here before stress) can  generate an evolution of the defect and could give an idea of  the aging of these crystal defects in an application.

The disappearance of the emission spot of Fig. 4b is  expected to be the generation of a metallic short in the GaN  layer near the current path and caused by the increase in  temperature and current coupled to the electromigration  phenomenon. The presence of the metal could affect the  charge recombination process that makes the spot in PEM.  The high current leakage and temperature could cause a local  melting of the drain metal as can go through the GaN layer.

The high polarization is possible if this filament does hold  the thermal and electric field stress.

Increasing the leakage current caused melting of the drain  metal and the filament to propagate through the GaN buffer  and reach the AlGaN connected to the source potential. The  melting caused by the high energy then propagates to the  upper metal level of the structure. An optical front-side view  is shown in Fig. 10. Many cracks are visible on the structure  metal in the defect in zone 1.

The defect visible with the IR camera in Fig. 6 is expected  to be an optical effect caused by the change of the polyimide  after being at high temperature.

![Cracks  Bump  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2f3de95e-acf2-40b5-87db-b5ca4a9ff2a9/2f3de95e-acf2-40b5-87db-b5ca4a9ff2a9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=3526c9b4e26037426566d99e2e3a91cf84aab163)
Fig. 10. Optical view of the defect zone (zone 1 in Fig. 4a). Some cracks on  the metal are visible.

A FIB cross section in Fig. 11 was performed in the defect  zone of this device to verify the failure hypothesis of the GaN  layer. The image in Fig. 11 is the FIB Slice&View image  when the defect is most significant.

The drain metal has disappeared with the melt propagating  to the metal above. However, it can be seen that the void  caused by the melting is just below the drain metal and is  contained in the GaN layer. The boundary of the void is the  AlGaN layer of the buffer superlattice, which is electrically  connected to the source.

![Previous drain  metal  GaMN  A1GaN  AIT  Si  88326   ATLD10000   Helios G3 LadyGaN/E  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0162ce21-aa50-47e8-8788-5cbba7cb035b/0162ce21-aa50-47e8-8788-5cbba7cb035b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=d5ccc64048e7482678021ee56178c4c4033b39b0)
Fig. 11. SEM image of the cross-section of the defect of the ε damaged device  a void is expected to be the consequence of the melting of a metal filament  under the drain metal where the electrical leakage path was. The image shows  that the leakage observed at high   $\mathrm{V_{DS}}$  polarization is vertical and in the GaN  layer, the defect stops at the AlGaN layer connected to the source.

The SEM image of Fig. 11 shows the evolution of the  leakage path through the GaN layer and related to crystal  defects. The study of both the δ devices of IIIB and the εa  device allows to show the origin of the defect and its evolution  to a complete failure.

The local high leakage current can come from existing  conductive dislocations induced by the manufacturing or the  hypothetical dislocations generated by the electric field and  the displacement of metal elements in the vicinity of the  dislocations, which locally reduce the electrical insulation and  create the leakage path in the GaN buffer.

Once the electrical path is in the structure, the high energy  can cause it to evolve into a metal percolation with melting of  the drain metal above the leakage path. Once this second step  has occurred, the device has reached total failure and the drain  and source electrodes are electrically shorted. The drain metal  melt propagates with the drain via to the upper level of metal  connected to the drain and then to the level of metal above  conneced to the source and creates a drain source electrical  short as visible in Fig. 12.

![Electrical short through  the dielectric layer  dielectric layer  Drain vias  3/2  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0bb43e00-99c3-415a-b407-67adf723addd/0bb43e00-99c3-415a-b407-67adf723addd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=3c7b05e33d1540a5cdeff9c7428a9b3349ca6ce9)
Fig. 11. SEM image of the cross-section of the defect of the ε damaged device.  The propagation of the melting of the drain metal to the drain via and then to  the upper levels of metal shows the electrical short that traduces the complete  failure of the device.

## C ONCLUSION 

The experiment on breakdown voltage revealed two types  of defects depending on the location of the weakest spot  within the device regarding the choices of design. The first  type is located under the field plate metal. The failure analysis  is relatively simple, and metallic shunts are expected. The

second type is a defect in the GaN buffer layer that appears to  be related to dislocations. The failure analysis at this step is  much more complicated because the device is degraded but  not severely, and the defect is difficult to observe. Some  experiments, such as chemical revelation, can provide  additional information to understand this second failure  mechanism. The increase of the energy in this type of  cristalline defects can produce a complete failure of the  device. The crystalline defect becomes a metallic defect in the  GaN layer due to the melting of the drain metal.

## R EFERENCES 

[1]    L. Ghizzo, G. Guibaud, C. De Nardi, F. Jamin, V. Chazal, D.  Trémouilles, R. Monflier, F. Richardeau, G. Bascoul, M. González;  November 12–16, 2023. "Backside Fault Localization and Defect  Physical Analysis of Degraded Power HEMT p-GaN Transistors  Stressed in DC and AC Switching Modes." Proceedings of the ISTFA  2023. ISTFA 2023: Conference Proceedings from the 49th  International Symposium for Testing and Failure Analysis. Phoenix,  Arizona,   USA. (pp.   pp.   491-499).   ASM.  https://doi.org/10.31399/asm.cp.istfa2023p0491.     [2]    M. Meneghini et al., "Power GaN HEMT degradation: from timedependent breakdown to hot-electron effects," 2018 IEEE International  Electron Devices Meeting (IEDM), San Francisco, CA, USA, 2018, pp.  30.5.1-30.5.4, doi: 10.1109/IEDM.2018.8614605.    [3]    M. Borga et al., "Evidence of Time-Dependent Vertical Breakdown in  GaN-on-Si HEMTs," in IEEE Transactions on Electron Devices, vol.  64, no. 9, pp. 3616-3621, Sept. 2017, doi: 10.1109/TED.2017.2726440.    [4]    Sven Besendörfer et al, Statistical of dislocation induced leakage  current paths in AlGaN/GaN HEMT structures on Si and the impact of  growth conditions, Applied Physics Express 15, 095502 (2022),  https://doi.org/10.35848/1882 -0786/ac8639     [5]    Takashi  Yokoyama, Yasushi  Kamimura, Keiichi  Edagawa, Ichiro   Yonenaga, Local current conduction due to edge dislocations in  deformed GaN studied by scanning spreading resistance microscopy,  Eur.   Phys.   J.   Appl.   Phys.   61   (1)   10102   (2013),  10.1051/epjap/2012120318    [6]    Kazanowska, Barbara Anna, Sapkota, Keshab Raj, Gunning, Brendan  Patrick, Jones, Kevin C, and Wang, George T. Crystallographic  Phosphoric Acid etching of GaN AlGaN and AlN Nanostructures..   United States: N. p., 2020. Web.     [7]    G. Kamler, J. Borysiuk, J. L. Weyher, A. Presz, M. Woźniak and I.  Grzegory, Application of orthodox defect-selective etching for  studying GaN single crystals, epitaxial layers and device structures,  Eur.   Phys.   J.   Appl.   Phys.,   27   1-3   (2004)   247-249,  10.1051/epjap:2004103.

