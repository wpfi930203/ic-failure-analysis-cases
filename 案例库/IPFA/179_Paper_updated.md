---
title: "179_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_d8902cf756a968ee5e88531656eed15b7295230462135641
file_size: 1769919
---

## How to Enable Electro-Optical Frequency  Mapping/Probing(EOFM/EOP) by Customized Test  Configure in Mix-signal Device  

Haus Zhang, Jianli Yang, Winter Wang   NXP Semiconductor (China) Limited, No.15 Xinghua Avenue, Xiqing Economic Develop Area, Tianjin, China  Phone : (86)18622967755, Email :  haus.zhang@nxp.com

Abstract —Electro-optical   Frequency   Mapping/Probing  (EOFM/EOP) are dynamic technology commonly applied to  digital design debug, but rarely used in mix-signal integrated  circuit failure isolation. In this paper, the feasibility of Electrooptical Frequency Mapping/Probing(EOFM/EOP) usage in  mix-signal integrated circuit devices was explored by test  configure debug. This paper then presented one real case of  customer   return   in   which   Electro-optical   Frequency  Mapping/Probing (EOFM/EOP) was successfully applied by  changing bench test configure

Keywords—Electro-optical   Frequency   Mapping(EOFM),  Electro-optical Probing(EOP), customized test configure debug

## I.    I NTRODUCTION 

With the increasing of the interconnect layers and shrinking of  wafer fab process , successful electrical failure isolation is  facing more and more challenges from front side. Meanwhile,  the fast increase of soft defect and timing issue in advanced  integrated circuits have pushed backside dynamic optical  techniques: EOFM (Electro Optical Frequency Mapping) [1]  and EOP (Electro Optical Probing) [2].

EOP/EOFM techniques are laser based optical tools that are  able to check the electrical activity of the devices from  backside silicon, without contacting the inner node of the  device directly. The EOP/EOFM techniques uses a 1340 nm  infrared laser to probe the waveforms non-destructively in an  integrated circuits internally. The laser is focused directly at  the level of the active areas of the device through the backside.  The voltage at a particular node of the device influences the  reflected light intensity in the parts-per-million range. With a  sensitive detection system, this signal can be extracted, and  semi-quantitative voltage information can be recovered [3].

In this paper, we present one customer CQC return case of  failure isolation using EOP/EOFM techniques. At first, the  failure was trigger by a constant voltage, and calculate the  mean value. In such a situation, EOP/EOFM was not suitable  due to lack of looping trigger signal. Then, bench setup  configuration was changed by looping the trigger signal with  a high/low switch on/off period, so that it can be applied to  EOP/EOFM   analysis.   Using   the   new   bench   setup  configuration, the defect location was highlighted, the final  defect was successfully identified with following analysis.

## II.   EOFM/EOP   T HEORY 

Electro Optical Probing/Electro Optical Frequency Mapping  (EOP/EOFM) is a laser-based voltage and timing waveform  acquisition system which can be used to perform failure  analysis on integrated circuits chip.

The drain voltage of a MOS (Metal-Oxide-Semiconductor)  transistor will vary with the switching operation of a trigger

signal, the electric filed distribution of the drain boundary will  also change correspondingly. This induces a change of  refractive index and absorption coefficient due to the electrooptical effect of different kind of material. When irradiating a  drain by a light beam through the silicon substrate, the  intensity of reflected light varies corresponding to the voltage  level. A laser beam interacts with a device through several  mechanisms. At the wavelength of 1340nm, the main effects  are absorption and refraction due to free carriers [4][5].

The EOP/EOFM function can observe the reflected light  which expresses the status of a transistor, and then measures  transistors switching at a specific frequency and images them.  The reflected light from a drain has the power spectrum  distribution. The EOFM picks up the intensity of signal under  certain frequency from the distribution and visualize it as an  image. By operating transistors in a specific region under  certain frequency, it is possible to observe if the circuits are  correctly switching or not [6]. The HAMAMATSU Phemos1000 system hardware setting requires a higher than 1.0V and  period larger than 20ns trigger signal (Fig.1), hence, the key  to use EOFM/EOP technique was how to appropriate trigger  signal.

![Signalseparator  windowopenedinfrontpanel  REF IN   SIGIN1   SIGIN2   SIGIN3  Not used in this system  Connectortype:SMA  (cableisbundledwiththesystem.)  Triggersignal  >20ns  >1.0V  Specificationoftriggersignal  (Risingedge/fallingedge:bothavailable)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cc6fcc43-ef72-49d7-b169-6711fbd462d7/cc6fcc43-ef72-49d7-b169-6711fbd462d7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215874%3B1743219474&q-key-time=1743215874%3B1743219474&q-header-list=host&q-url-param-list=&q-signature=235e1056ce289109d612bb92d971327385618121)
## III.   E XPERIMENT AND RESULT 

One NXP SMOS8 MV 250nm technology mix-signal chip  was returned from customer for root cause investigation due  to abnormality in a value of average output voltage of VIP pinAvip. Bench test in PA lab confirmed Avip cannot meet low  standard, the result was illustrated in TABLE I, no matter the  POUT was forced at high level 3.6V or forced at low level of  2.4V, the VIP output voltage was always lower than reference  part, hence, the customer required average voltage of VIP  cannot be high enough.

Setup condition:

ROTINIG=FRSET=MSBFE=LGCRSTB=WD=0(c  onnect   to   GND).   FDTSET0=FDTSET1=5V  (connect to VS)       TEST0=TEST1=0, TEST2  $2{=}35\mathrm{V}$   (TEST_30V force   35V; TEST0_J&TEST1_J on the left, TEST2_J on   the right)       Supply VCC=VCCR=VSP=16V, VS=5V @100mA       Supply  $_\mathrm{VL}{=}5.1\mathrm{V}$  , COM=3.6V       Force POUT=3.6V, measure VIP voltage as V1       Force POUT=2.4V, measure VIP voltage as V2       Calculate Avip=(V2-V1)/1.2V

Result:

TABLE I.     B ENCH VERFICATION RESULT

||V1|V2|Avip|
|---|---|---|---|
|Reference part|2.38 V|3.57 V|0.99 V|
|CQC part|2.29 V|1.74 V|0.46 V|


Photon emission analysis was performed with both POUT  input voltage configs, as the result illustrated in Fig.2, there  were several extra emitting spots and also missing PEM spots  highlighted on the CQC part (red dot square area) compared  with the reference part (white dot square area).

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6f2a9cac-66aa-4dbc-aed1-b7cfd96ebe8d/6f2a9cac-66aa-4dbc-aed1-b7cfd96ebe8d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215874%3B1743219474&q-key-time=1743215874%3B1743219474&q-header-list=host&q-url-param-list=&q-signature=869e4cd6ab2c2007e8ad0247bc6f473933d5a1a5)
PEM result of reference part

![extra and missing spots  PEM result of CQC part  PEM result of CQC part  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/72290145-0c5d-4d4f-8d07-2a8b9552d6dd/72290145-0c5d-4d4f-8d07-2a8b9552d6dd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215874%3B1743219474&q-key-time=1743215874%3B1743219474&q-header-list=host&q-url-param-list=&q-signature=56389239b7847447895d55413c9162873c8d927f)
Fig. 2. Photon emission result.

After detailed layout and schematic studying, all of the  extra emitting spots and missing spots were shown in the  schematic extraction in Fig.3, all of the extra missing spots are  saturation spots as the malfunctional node, rather than  defective spot, the real defective component was still not  visible at this PEM analysis.

![ssingspot  extra spot  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7c5d8b34-4603-43e1-8d02-1b64bda00325/7c5d8b34-4603-43e1-8d02-1b64bda00325.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215874%3B1743219474&q-key-time=1743215874%3B1743219474&q-header-list=host&q-url-param-list=&q-signature=424eedffe3ab72a03830c527990c34cdce2ff79d)
Fig. 3. Schematic extraction illustrate the PEM spot location.

Then new configure was developed by toggling the trigger  input signal POUT with 1K Hz frequency, the result was as  Fig. 4, the VIP output voltage level cannot be as high as the  reference sample, meanwhile, there was a 180 degree phase  delay on the CQC sample compared with reference unit.

![POUT  POUT  VIP abnormal phase andvoltage leve  VIP abnormal phase and voltage level  VIP  ectHodoff   ctHoldoff  Reference part  Reference part   CQC part  cQCpart  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/72c7a48f-dc55-4d1c-b2d7-8453c4b99a58/72c7a48f-dc55-4d1c-b2d7-8453c4b99a58.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215874%3B1743219474&q-key-time=1743215874%3B1743219474&q-header-list=host&q-url-param-list=&q-signature=c3b47bb5ce786ba7798911d50e8fff767f2cfb28)
Fig. 4. new-changed test setup configuration and bench result.

Since both amplitude and phase of the VIP output  waveform were failed on the CQC sample with the new test  configure, EOFM was tried by applying 50K Hz toggling

frequency on POUT input, as Fig. 5 illustrated, EOFM amp  image highlighted the amplitude deviation with a suspect  abnormal spot on one component inside the target block area,   also EOFM phase image pointed out a similar abnormal spot  due to the abnormal phase of VIP output waveform, the  EOFM phase spot location was exactly same location as  EOFM amp image, combining both amp image and phase  image, the final defective spot was localized on the EOFM I/Q  image (the computing result combining amp image and phase  image).

![REF_pattern_20.0x(2x)  REFai P_20.0x（2x REF_1/Q_20.0x(2x）  REFR  se_20.0x（2x） EOFMresultofreferencepart EOFM result of reference part CQC_amp_20.0x(2x CQC_1/Q_20.0x(2x)  CQC_phase_20.0x(2x) EOFM result of CQC part ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9326d618-54bb-425c-9206-e345a44146d1/9326d618-54bb-425c-9206-e345a44146d1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215874%3B1743219474&q-key-time=1743215874%3B1743219474&q-header-list=host&q-url-param-list=&q-signature=1e9b0e1a3759887c65bae965b40a58eb93885f36)
Fig. 5. EOFM image using the new test setup configure.

In order to characterize the on/off status of the EOFM  highlighted components, EOP analysis was followed using the  same frequency, as results in Fig. 6 illustrated, distortion EOP  waveform was captured on the EOFM spot component, while  the other components EOP waveform were all normal as  reference sample. The distortion EOP waveform on failing  component also validated that this component was real failed.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/26266dd1-e327-4415-955e-face76c97623/26266dd1-e327-4415-955e-face76c97623.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215874%3B1743219474&q-key-time=1743215874%3B1743219474&q-header-list=host&q-url-param-list=&q-signature=9cfe1c6b62c46170f1cfae5b76dd6b8ce332465f)
Fig. 6. EOP waveform of   ${\bf M}58{<}0{:}3{>}$   showing abnormal at EOFM spot site.

Using EOFM/EOP, the suspect failing component was  successfully localized in the target block, then the CQC  sample was decapsulated from front side, after that, detail  optical microscope visual inspection didn’t reveal any visible  abnormal focus on the suspect component block area.  Following that, 2 FIB pads were deposited on metal2 layer on  the CQC return sample, and passive microprobe checked the  IV curve of the suspect defective component, as a result,  resistive short was confirmed between vp_int and in_plus,  which corresponding to gate and drain of the failing   ${\bf M}58{<}0{:}3{>}$  device, the result was in Fig. 7.

![vp_intvsin_plus  Resistiveshort  30  20  REF  Voltage(v)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7a96be2e-fb37-48d1-9ce9-5a996f262654/7a96be2e-fb37-48d1-9ce9-5a996f262654.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215874%3B1743219474&q-key-time=1743215874%3B1743219474&q-header-list=host&q-url-param-list=&q-signature=81247d83a7f51fcb1ee27463c94683aa01fae1cf)
Fig. 7. Passive microprobe IV measurement.

IR-OBIRCH analysis was performed with the abnormal  resistive short IV curve between vp_int and in_plus, as a result  in Fig. 8 left shown, the abnormal resistance change spot was  captured at the same location on   ${\bf M}58{<}0{:}3{>}$  , which correlated  with the EOFM result in Fig. 8 right illustrated.

![OBIRCh spot  OBIRCh spot   EOFM spot  EOFM spot  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c121adec-bb25-4fc1-b688-f10751a7d0a5/c121adec-bb25-4fc1-b688-f10751a7d0a5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215874%3B1743219474&q-key-time=1743215874%3B1743219474&q-header-list=host&q-url-param-list=&q-signature=9f06d327efc2deb82b9112cdc2bab9c7520376f4)
Fig. 8. OBIRCH analysis using the short IV curve.

As the schematic extraction illustrated in Fig. 9, the  defective component was on   ${\bf M}58{<}0{:}3{>}$  , which was fail to  emission during PEM analysis, ie, the DC setup config. But  this component was highlighted by EOFM/EOP with new test  configure.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8c87c8bf-f848-4ae5-90e4-2705e95fca33/8c87c8bf-f848-4ae5-90e4-2705e95fca33.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215874%3B1743219474&q-key-time=1743215874%3B1743219474&q-header-list=host&q-url-param-list=&q-signature=36c9d5aef2e460e6c71d09373a84478811930442)
Fig. 9. Schematic analysis showing the defect device location.

FIB cross section was then carried out carefully focus on  the IR-OBIRCH spot location, and finally poly defect was  found at the defect location of   ${\bf M}58{<}0{:}3{>}$   device, in Fig. 10  extra poly extended to contact and induced leakage path  between gate and drain of   ${\bf M}58{<}0{:}3{>}$  device, the correct  profile should be as the GDS cartoon illustrated in Fig.10.

![SEM image  Mletall  Comtact  Poly defect  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9c3038fe-2fb6-499f-9a59-d82d279a932f/9c3038fe-2fb6-499f-9a59-d82d279a932f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215874%3B1743219474&q-key-time=1743215874%3B1743219474&q-header-list=host&q-url-param-list=&q-signature=f8b3d0d87742274bfd443171b40de8b722847473)
FIB cross section result of defect

![GDS cross section cartoon of defect device  GDS cross section cartoon of defect device  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/afb0fd4c-3df5-45a7-9306-9007835a2e45/afb0fd4c-3df5-45a7-9306-9007835a2e45.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215874%3B1743219474&q-key-time=1743215874%3B1743219474&q-header-list=host&q-url-param-list=&q-signature=17c8957df9557da603cff12af18402ad102f1b52)
Fig. 10. FIB cross section at the defect location.

## Conclusion 

The case study and experiment above proved that  EOP/EOFM techniques can be realized in mix-signal circuit  with customized test configuration. With the help of the  EOP/EOFM techniques, the block failure localization on  mix-signal integrated circuit can be fast and efficient. EOFM  provides switching activities and timing information on path  and localize the defect site out of the active area of MOS  transistor. EOP could easily probe and check the signal in the  target area. With this technique, the failure isolation and  failing block/component determining time could be greatly  reduced.

## Acknowledgments 

The author would like to thank all the efforts of PQC_TJN  physical analysis team of NXP semiconductor for their  professional physical analysis support in completing this  paper.

## References 

[1]    Ng, Y. S., Lundquist, T., Skvortsov, D., Liao, J., Kasapi, S., & Marks,  H. (2010). Laser voltage imaging: A new perspective of laser voltage  probing. In  ISTFA  (pp. 5-13).      [2]    Siva Kolachina, “Introduction to Laser Voltage Probing (LVP) of  Integrated Circuits”,  Microelectronis Failure Analysis: Desk Reference  Fifth Edition , pp.426-430, Texas Instruments Inc., Stafford, Tex.,  USA.     [3]    Kindereit, U., et al. "Quantitative Investigation of Laser Beam  Modulation in Electrically Active Devices as Used in Laser Voltage  Probing."  Device & Materials Reliability IEEE Transactions  on  7.1(2007):19-30.     [4]    R. A. Soref and B. R. Bennett, “Electro-optical effects in silicon,”   IEEE  J. Quantum Electron.,   vol. QE-23, no. 1, pp. 123–129, Jan. 1987.     [5]    M. Bruce et al., “Waveform acquisition from the backside of  silicon  using electro-optical probing,”  in Proc.   $25^{t h}$   ISTFA , Santa Clara, CA,  1999, pp. 19-25.     [6]    H. Zhang, P. Tian, X. Qian and W. Wang, "Electro optical probing /  frequency mapping (EOP/EOFM) application in failure isolation of  advanced   analogue   devices,"  2017   IEEE   24th   International  Symposium on the Physical and Failure Analysis of Integrated Circuits  (IPFA) , Chengdu, 2017, pp. 1-5.

