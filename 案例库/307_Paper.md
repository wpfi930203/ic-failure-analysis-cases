---
title: "307_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_b2e6238eb25f4d6e2b07880e054375837295230462135641
file_size: 629204
---

## EOFM for contactless parameter extraction of low k  dielectric MIS structures  

N. Herfurth a,c,\* , E. Amini d , A.Beyreuther a,c, , T. Nakamura b , S. Keil c , C. Boit a     a Semiconductor Devices, Berlin University of Technology (TUB), Einsteinufer 19, 10587 Berlin, Germany    b Hamamatsu Photonics KK, 325-6, Sunayama-cho, Naka-ku, Hamamatsu, Shizuoka Pref., 430-8587 Japan    c Sensuators and Actuators, Berlin University of Technology (TUB), Einsteinufer 19, 10587 Berlin, Germany  d Security in Telecommunications, (TUB), Sekr. TEL16, Ernst-Reuter-Platz 7, 10587 Berlin, Germany  \* Phone: +49 1734849904, \*Email:  norbert.herfurth@tu-berlin.de

Abstract-    This paper investigates electro-optical frequency  mapping   (EOFM)   characteristics   of   metal   insulator  semiconductor (MIS) capacitor test structures. The EOFM  characteristic describes the EOFM signal intensity dependence to  the device under test (DUT) input signal amplitude. We can  monitor the gradual increase of charge per voltage in  accumulation and in strong inversion. We show that the device  parameters flat band voltage and the threshold voltage can be  extracted from a series of EOFM measurements. This parameter  extraction is linked to a low k dielectric degradation experiment.  Changing of the extracted parameters during a degradation  process allows contactless monitoring of the device properties and  their degradation under electrical stress.

Keywords  –  EOFM, low k, parameter extration, Soft breakdown,  Hard breakdown .

## I. I NTRODUCTION 

Metal insulator semiconductor (MIS) structures are an  important part in the front end of line (FEOL) as well as in the  back end of line (BEOL) in integrated circuit (IC) technology.  The ongoing development of insulating BEOL materials is  necessary to ensure the capacitive load of the BEOL is not  limiting the IC switching characteristics. Consequently,  materials with low k values are required for the BEOL. These  materials are often coupled with mechanical and electrical  reliability problems [1, 2]. The reliability community often  address these problems with electrical measurements and  statistical modelling to predict a time to failure. However,  physical fault isolation of defective sites would give a more  complete picture of the degradation process. The statistical  nature of the low k degradation process makes it crucial to  validate the representativity of single physical fault isolations to  the degradation characteristic of the test structure.

Photon emission microscopy and thermal laser stimulation  have been presented being capable to isolate low degradation  states of low k dielectrics [3]. For these techniques the device  under test (DUT) needs to be stressed during the localisation  measurements. Thus, a further degradation during the  localisation measurement cannot be excluded. In this paper we  show that electro-optical frequency mapping (EOFM) is also  capable of detecting the degradation in low k material MIS test  structures. However, the low voltage levels required to measure  EOFM signals are likely to small to force further degradation.

EOFM is a contactless and destruction-free method that allows  to acquire signals that are related to the optical properties of a  dynamically operated DUT and thus providing insight into the  dynamic state of the device [4, 5]. Sweeping the DUT input  amplitude allows us to measure an EOFM characteristic. This  characteristic is measured and analysed for different states of  degradation of the DUT. From these characteristics the change  of device parameters like the flat band voltage can be extracted  and monitored over the degradation.

## II.   SAMPLES  

In comparison to metal insulator metal (MIM) structures,  MIS structures are a good alternativity to characterise insulating  materials [6–8]. Whereas a MIM structure does reflect the  device application. Dedicated MIM and MIS structures with  copper metallisation and porous low k material show similar  degradation characteristics. In terms of failure analysis, the  infrared transparent backside of MIS structures is advantageous,  allowing direct optical access to the material that needs to be  characterised.

Figure 1 shows a schematic drawing of the test structures  used. The backside aluminium contact is locally removed to  enable optical access to the formed capacitive test structure. The  n-doped bulk silicon is covered by a native oxide, isolating the  low k layer from the substrate. The low k material is a SiOCH  type dielectric with OSG 2.0   $(\mathrm{k}{=}2.0)$  ,   $45\%$   porosity and 40nm  thickness. A 4nm Ta/TaN diffusion barrier prevents the copper  from diffusing into the low k material. For this work we are  using  2ߤ݉ ݔ 2ߤ݉  structures.

![Probepad  SiM  Formed capacitor  Formed capacitor Diffusion  Diffusion  barrier  barrier   SiOz  Backside contact  Backside contact S  Native oxide  Native oxide ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bccf8abd-3e55-4249-bf46-58ec1a1f0d58/bccf8abd-3e55-4249-bf46-58ec1a1f0d58.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=819ef5812622deb13f94aa6c9c81ae53ea9930fd)
Figure 1: Schematic drawing of the MIS structures used

![Degradation of a low k BEOL test structure  Degradation of a low k BEOL test structure  under CVS  under CVS leakage current over time @26.5V CVS  leakage current over time @26.5V CVS 1E-04  1E-04  trap  trap   Hard breakdown  Hard breakdown charging  charging = 1E-06  Current [A] 1E-06  defect  defect 1E-08  1E-08  nukleation  nukleation 1E-10  1E-10 O1E-12  1E-12  Soft breakdown  Soft breakdown 1E-14 1E-14  0  1,000  1,000  2,000  2,000 Time [s]  Time [s] ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/be838b58-bb4a-408c-aa17-4f88e0cb64e9/be838b58-bb4a-408c-aa17-4f88e0cb64e9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=2b867bf0717f72142ebe7889e9cc3ff2a4666dbb)
Figure 2: Characteristic constant voltage stress degradation curve of a  2ߤ݉ ݔ 2ߤ݉  MIS structure with typical low k dielectric degradation phases

In Figure 2 a characteristic I-t degradation curve of this  structure type can be seen. Four, for low k dielectric  degradation, typical domains can be identified. Starting with the  defect charging phase which is characterised by a reduced  leakage current over time. The defect nucleation phase, where  the leakage current is nearly, constant is following. The soft  breakdown (SBD) phase is characterised by a constantly  increasing leakage current. Ending in a current peak during the  hard breakdown (HBD). The leakage current is a mean to  monitor the degradation. In this work we show that EOFM  measurements can be used to monitor the degradation process

## III.   EXPERIMENTAL   SETUP  

EOFM is an optical analysing technique that maps frequency  dependent changes in the index of refraction of the analysed  material stack. These frequency dependent changes in the index  of refraction are stimulated by applying an input frequency to  the DUT. In our case we are using a function generator with a  square wave pulse with  $50\%$   duty cycle and 1 MHz frequency.  The EOFM measurements is performed with the Hamamatsu  Phemos 1000 in EOFM mode (1400nm laser) and a 50x  magnification lens with a numerical aperture of 0.71.

To bring the DUT into a controlled state of degradation, we  use the Keithley SC4200 to apply electrical stress to the devices.  The front side of the test structures have been bonded to contact  the metal front side and an extensive area backside aluminium  contact is used to contact the n-doped silicon substrate. Locally  removed aluminium allows to get optical access to the infrared  transparent backside of the test-structure.

## IV.   EOFM   CHARACTERISTIC  

For measuring an EOFM characteristic, the DUT stimulating  signal amplitude is varied. In this work we are measuring a MIS  structure and vary the stimulation amplitude form -10V to  $+10\mathrm{V}$    in 2V steps. This modifies the bulk charge carrier density at the  silicon-insulator interface.

A series of EOFM measurements with varying input  amplitudes of a single non-stressed MIS structure can be seen  in figure 3. To extract the EOFM characteristic from these

![Formed  Formed  capacitor  capacitor   Bond pad  Bond pad  50μm 50pm    （a)  (a)  -10V  -10V   -6V  -6W   -1A←  -1V   +1←  +1V   6  +6V   +10V  +10V  (b)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/34bc2e11-4e30-4a72-9429-919cf66c12e6/34bc2e11-4e30-4a72-9429-919cf66c12e6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=2ddf7ea505dc8235cb56dd1e32f9e867b83f81a0)
Figure 3: (a) Backside pattern image of a  $2\mu m\,x\,2\mu m$   BEOL MIS test  structure; (b) part of a series of EOFM measurements with varying  stimulation amplitudes

measurements we analyse the raw sensor data that correspond  to the images presented in Figure 3. From every analysed data  set we determine the maximum EOFM signal amplitude. This  value together with the stimulating input amplitude generates a  single data point in the EOFM characteristic. A full EOFM  characteristic of a single non stressed MIS structure can be seen  in figure 4.

In forward bias a linear dependency between the EOFM  signal intensity and the DUT input amplitude can be seen. In  addition, the signal intensity in forward bias is higher compared  to the signal intensity in reverse bias.

![EOFM signal intensity [a.u.]  8000  8000 6000 6000  4000  4000 2000 2000  0 -10 -10-8-6-4-20  -8  -6  -4  -2  0  2  4  6  8  10 DUT input amplitude [V]  DUT input amplitude [V] ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a329fad8-19bb-43cb-a547-a233dc1effa0/a329fad8-19bb-43cb-a547-a233dc1effa0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=bf9c6fbec970c5d898226d7b707654f3182d0914)
Figure 4: EOFM characteristic of a non-stressed low  $\mathbf{k}$   dielectric MIS structure

In forward bias, the silicon at the silicon-insulator interface is  in accumulation whereas in reverse bias we expect a strong  inversion.

## V. EOFM   CHARACTERISTIC   -   DISCUSSION  

EOFM is sensitive for changes in the index of refraction. In  our context the charge carrier density at the silicon-insulator  interface is modulated by the applied stimulation voltage.

One of the key factors that modifies the optical properties of  silicon is the charge carrier density. For a voltage biased MIS  system, the charge carrier concentration in respect to the silicon  band bending   $(\Psi_{\mathrm{Si}})$   is given by:

$Q_{S i}=$  $$\begin{array}{r l}&{\mathrel{\mathop{\vee}}_{S i}-}\\ &{\pm\sqrt{2\varepsilon_{s i}k T N_{A}\left[\left(e^{-\frac{e\Psi_{s i}}{k T}}+\frac{e\Psi_{s i}}{k T}-1\right)+\frac{n_{i}^{2}}{N_{A}^{2}}\left(e^{\frac{e\Psi_{s i}}{k T}}-\frac{e\Psi_{S i}}{k T}-1\right)\right]}}\end{array}$$
This relation is plotted in figure 5. From this plot we can  extract the flat band voltage   $\left(U_{F B}\right)$   as well as the threshold  voltage   $(U_{T H})$  . In strong inversion and in accumulation we can  see an exponential slope of   $e^{-\frac{e}{k T}}$   and   $e^{\frac{e}{k T}}$   respectively. In  depletion and inversion, the accumulated charge changes linear  in respect to  $\Psi_{\mathrm{Si}}$  .  This allows us to extract   $U_{F B}$   at the starting  point of the positive exponential slope and   $U_{T H}$   at the end of the  negative exponential slope.

The curve presented in figure 4 shows a much lower absolute  slope in reverse bias than in forward bias. Consequentially, the  changing charge carrier density in reverse bias must be lower  compared to the changing charge carrier density in positive bias.  For reverse bias we bring the system into strong inversion which  is a minority carrier accumulation at the insulator-silicon  interface. In a MIS system the time to accumulate minority  carriers is limited by the intrinsic charge carrier generation rate,  typically a few   $100\mathrm{kHz}$  . Whereas for a MIS system with  adjacent source and drain diffusion regions minority carriers  can be delivered with nearly no delay from these diffusions.  This circumstance is well known from MIS capacitance  characteristics as shown in figure 6. For high frequencies in  reverse bias the MIS capacitance remains in deep depletion.  Thus, the system can store less charge compared to the same  system that is measured with the same voltage at lower

![100 increasing input  increasing input  10  frequency  frequency      accumulation  accumulation 1  strong Inversion strong Inversion  ) [As] 0.1 depletion and  depletion and  Si  inversion   0.01  inversion  log (Q 0.001  ܷ TH  ்ு    ܷ UFB  ி 0.0001 -0.8 -0.8   -0.6 -0.6   -0.4 -0.4   -0.2  -0.2  0  0.2  0.2  0.4  0.4 Band bending Ysi [eV]  Band bending   [eV] ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d44092b8-9845-4641-b64a-9318f6fd9852/d44092b8-9845-4641-b64a-9318f6fd9852.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=9492bed302590f8ab115a60d1891f862f277ac01)
Figure 5: Free carrier density in a MIS system with n substrate in relation to  band bending

![C02     શ Isi=  ܁ܑ ൌ      1,0 1D    low frequency  low frequency    -0,8  0,8   Ysi= 2ΦB  શ  ൌ    શ Ys：=史  ൌ      ܁ܑ  ۰  ܁ܑ  0,6  0,6   / mmim    -0,4  0,4   Cmim  ᇱ   0,2  0,2    high frequency  high frequency  0   0   −← —U      →  →+U    V-VFB  −   ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e1a1306b-85dd-498c-82fc-e217196b5924/e1a1306b-85dd-498c-82fc-e217196b5924.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=fb413ada7c75e671ab3b3431f18897edcdc354ce)
Figure 6: C-V Characteristic of a MIS system with n substrate [8]

frequencies. The EOFM characteristic shown in figure 4 shows  a lower signal intensity in reverse bias than in forward bias  which is likely caused by a lower charge carrier density in  reverse bias compared to forward bias. A 1MHz stimulation  frequency that is used to measure the EOFM characteristic is  too high to allow sufficiently enough minority carriers to  generate in time to fully develop the strong inversion.

## VI. CASE   STUDY  

We measured EOFM characteristics for different levels of  degradation of a low k dielectric MIS test structure. The EOFM  characteristic of a non-stressed structure is shown in figure 4  and was discussed earlier in this work. To evaluate the influence  of the degradation of a MIS structure on the EOFM  characteristic, a controlled degradation has been performed on  the structure that was used to measure the characteristic of  figure 4. For the degradation we used a voltage ramp. A current  compliance (CC) is used to limit the degradation. Whereas the  current level determines the level of degradation. The series of  voltage ramps with different CCs can be seen in figure 7. The  degradation process from ramp #1 to ramp #3 can be identified

![12000 2000  EOFM signal intensity [a.u.]  noStress  no Stress 10000 10000  8000 8000   O,1nA  0,1nA leakage  leakage 6000 6000   current  current -10nA  10nA 4000 -000   leakage  leakage current  current 2000 2000   1000nA  1000nA leakage  leakage current  current 0 -10 -8 -6 -4 -2 -10-8-6-4-20246810  0  2  4  6  8 10 DUT input amplitude [V] DUT input amplitude [V]  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b96556aa-a0d1-4815-8de6-db64ccad9949/b96556aa-a0d1-4815-8de6-db64ccad9949.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=21b5f81e13dca5e09e10d22ecc50a5414ebf8903)
Figure 8: EOFM characteristics of a low k dielectric MIS structure in different  states of degradation

by the increased leakage current at a constant voltage. Using a  maximum of 10V stimulating amplitude to measure the EOFM  characteristics, we ensure to not further degrade the structure  during the measurement.

## VI. CASE   STUDY   -   DISCUSSION  

In figure 8 we can see a clear trend in the EOFM  characteristics of BEOL test structures under different levels of  degradation. Extending the linear part of the positive bias of the  graph, we can see a shift of the flat band voltage. The flat band  voltage shift for the different levels of degradation are  summarised in table 1. The flat band voltage is reduced with  increasing degradation if the structure is still in SBD. With a  current compliance of   $1\upmu\mathrm{A}$   the structure is driven into HBD  where it usually comes to significant morphological material  changes due to high current densities. In reverse bias we see the  high frequency behaviour of the charge carrier density shown in  figure 5, making it difficult to extract the threshold voltage from  this specific curve. Nevertheless, we can see an increase of the  EOFM signal intensity with ongoing degradation. With ongoing  degradation, due to the increased leakage current, minority  carriers can be transported faster into the substrate via the  insulating layer. This enables to build up the inversion charge  faster with ongoing degradation, resulting in a more vertical  slope.

![1E-6 1E-6  Leakage current [A]  100E-9 100E-9  10E-9  10E-9  −−−       ramp #3  ramp#3  (1μA CC)  (1µA CC)  1E-9 1E-9  −⋅−⋅   ramp #2   ramp#2  100E-12 100E-12     (10nA CC)  (10nA CC)  10E-12 10E-12  1E-12  1E-12  −⋅⋅−⋅ ramp #1    ramp #1  100E-15 100E-15      (100pA CC)  （100pACC  10E-15 10E-15  0510152025303540  0  5  10 15 20 25 30 35 40 Voltage [V] Voltage[V]  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2c2da301-05af-474b-aa99-a4ebc71bf37c/2c2da301-05af-474b-aa99-a4ebc71bf37c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215701%3B1743219301&q-key-time=1743215701%3B1743219301&q-header-list=host&q-url-param-list=&q-signature=afdd50c830e3b57ca28bee0205bf2f56a928304d)
Figure 7: Voltage ramp with current compliance (CC) to bring the structure in  a controlled degradation state

|Degradation level|ઢࢁ ࡲ࡮||
|---|---|---|
|No Stress|0|SBD|
|100pA|-0.65|SBD|
|10nA|-1.4|SBD / HBD|
|1μA|-1.05|HBD|


Table 1: Flat band voltage shift for different states of degradation

## VII. SUMMARY  

A series of EOFM measurements can be brought together to  measure an EOFM characteristic. These characteristic of MIS  structures can be used to obtain insight into the charge carrier  density of the semiconductor. Furthermore, we can easily  extract the flat band voltage shift from these measurements.  Making it easy to monitor the flat band voltage change of a  degrading device. Measurements with low input frequencies  also allow to extract and monitor the threshold voltage. We have  presented a use case were the monitoring of the flat band shift  can be used to monitor the degradation of a low k dielectric MIS  structure.

## VIII. CONCLUSION AND OUTLOOK  

EOFM allows to visualise and monitor the charge carrier  density in MIS systems. Similar to a CV measurement we can  extract the flat band voltage and the threshold voltage from  EOFM characteristics. In addition, with a series of EOFM  characteristics we can directly monitor the relative charge  carrier density change as well as a 2D information about the  relative charge carrier density distribution. Performing the  presented measurements on a system with better optical  resolution to localise an early defect development though a  locally changing charge carrier density would be interesting,  especially for BEOL SBD analysis. The capability of detecting  a SBD with EOFM have been presented in this work. If no 2D  information is desired, electro optical probing (EOP) represents  an alternative to EOFM. Performing EOP measurements can be  performed faster. Analysing the measured EOP waveform can  be beneficial to obtain more specified information about the  device at a single measurement point. However, for monitoring  a device degradation it can be difficult to ensure that the EOP  measured spot size includes the defect. Thus, especially for  larger BEOL test structures the 2D information from EOFM  measurements are essential.

## ACKNOWLEDGMENT  

The authors would like to thank Andreas Eckert from TU  Berlin for sample preparation and they are grateful to imec  Belgium for providing test structures and additional help.

## REFERENCES  

[1]   Y. Li  et al.,  “Influence of absorbed water components on  SiOCH low-k reliability,”  J. Appl. Phys. , vol. 104, no. 3,  p. 34113, 2008.    [2]   G. Wang, C. Merrill, J.-H. Zhao, S. K. Groothuis, and P.  S. Ho, “Packaging effects on reliability of cu/low-k  interconnects,”  IEEE Trans. Device Mater. Relib. , vol. 3,  no. 4, pp. 119–128, 2003.    [3]   N. Herfurth  et al.,  “Non-invasive soft breakdown  localisation in low k dielectrics using photon emission  microscopy and thermal laser stimulation,”  Microelectronics Reliability , vol. 92, pp. 73–78, 2019.    [4]   P. Perdu, G. Bascoul, S. Chef, G. Celi, and K. Sanchez,  “Optical probing (EOFM / TRI): A large set of  complementary applications for ultimate VLSI,” in  2013  20th IEEE International Symposium on the Physical and  Failure Analysis of Integrated Circuits (IPFA): 15-19  July 2013, Suzhou, China , Suzhou, China, 2013, pp.  119–126.    [5]   U. Kindereit, “Fundamentals and future applications of  Laser Voltage Probing,” in  2014 IEEE International  Reliability Physics Symposium (IRPS 2014): 1-5 June  2014, Waikoloa, HI , Waikoloa, HI, USA, 2014, 3F.1.1- 3F.1.11.    [6]   L. Zhao  et al.,  “Role of copper in time dependent  dielectric breakdown of porous organo-silicate glass lowk materials,” p. 222110.    [7]   C. Wu, “In-depth understanding of low-k dielectric  reliability in interconnect system,” Dissertation, 2016.    [8]   C. Wu, Y. Li, M. R. Baklanov, and K. Croes, “Electrical  Reliability Challenges of Advanced Low-k Dielectrics,”  ECS Journal of Solid State Science and Technology , vol.  4, no. 1, N3065-N3070, 2015.    [9]   Y. Taur and T. H. Ning,  Fundamentals of modern VLSI  devices,  2nd ed. Cambridge: Cambridge Univ. Press,  2013.

