---
title: "309_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_68f3c96c419ba4e37ebe14cab874198f7295230462135641
file_size: 2206703
---

## Innovative Methodology for Short Circuit Failure  Localization by OBIRCH Analysis  

Ooi Yong Khai, Jack Ng Yi Jie  Device Failure Analysis, Intel Microelectronics (Malaysia),   Plot 6, Bayan Lepas Technoplex, Medan Bayan Lepas 11900 Penang, Malaysia.  \*   Phone: +60 1114425710 \*Email: yong.khai.ooi@intel.com

Abstract-   Lock-in thermography (LIT) is a commonly used FA  technique to perform fault isolation for parametric short failures  in microelectronic devices as compared with Optical Beam  Induced Resistance Change (OBIRCH). This is because the  OBIRCH technique becomes significantly less sensitive for direct  hard short circuit parametric failure. This paper presents a simple  yet innovative and effective methodology to increase resistance  variances during OBIRCH analysis in hard short failures to  improve the fault isolation success rate.

Keywords  –  OBIRCH, short circuit failure (Short), increase  resistance variances

## I. I NTRODUCTION 

OBIRCH analysis is a widely used failure analysis  methodology in the semiconductor industry for locating a  leakage related defect. Typical OBIRCH investigated defects  are leakage in polysilicon, gate oxide pinholes, void in metal  track, and drain/source shorts. It is useful for field failures as  well as the failures in the manufacturing processes in both the  development and mass-production phase. In principle, a laser  beam with a wavelength of   $1.3\mathrm{{um}}$   is stimulated on a device to  induce a thermal effect, then the thermal generation heats up a  defective area and causes resistance changes which will then  induce current alteration ∆I, which will be detected by the  OBIRCH amplifier and imprinted on the screen as abnormal  spots. The current variation, ∆I can be given by   $\Delta\mathrm{I}{=}_{-}(\Delta\mathrm{R}/\mathrm{V})\mathrm{I}^{2}$    (Fig. 1)[1].

![Laser:=1.3μm   Laser(frontside)   Leakage CurrentPath  A1  Heated   △I（△R/V）P  Si-sub.  △T,TCR  Laser(backside)   Dependsondefectsandmaterials  1:Currentbeforelaserirradiation  DefectsinMetal Line  V:Appliedvoltage  I:Current change dueto laser irradiation(whenconstantvoltageisapplied)  △R:Resistanceincreasewiththetemperatureincreaseduetolaserirradiation  △T:Temperatureincreaseduetolaserirradiation  TCR:Temperaturecoefficientofresistance  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9b2b4bb0-21c6-4f3a-b6c0-e2319e0ec5aa/9b2b4bb0-21c6-4f3a-b6c0-e2319e0ec5aa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215707%3B1743219307&q-key-time=1743215707%3B1743219307&q-header-list=host&q-url-param-list=&q-signature=060e041e24a34396611b45e2c0503bba62921498)
Fig. 1 Principle of OBIRCH

OBIRCH proved to be very effective and precise in  parametric current leakage isolation. Fig. 2 shows an example  of OBIRCH analysis between the Vcc to Gnd pins for an early  turn on failure, where OBIRCH analysis detected an abnormal  OBIRCH spot at the die level which correlated with the failing  circuitry.

![Vcc w.r.tVss  一 OBIRCHSpot  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fddf2e83-5756-4287-92f3-f752da5e46bd/fddf2e83-5756-4287-92f3-f752da5e46bd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215707%3B1743219307&q-key-time=1743215707%3B1743219307&q-header-list=host&q-url-param-list=&q-signature=3d04c1dee92ade405016722b351e462aff6c9423)
Fig. 2 OBIRCH result with biased VCC w.r.t Vss

However, it becomes less sensitive for a hard short circuit  failure model as ∆I is not significant due to the low ohmic  characteristic of the failure. The limitation is due to mA range  current clamp limit of the OBIRCH tool. As an I-V example in  Fig. 3 below, when a device failed short with a resistance of 6  ohm, voltage supply into the DUT during OBIRCH analysis is  only workable for not more than 0.05V, otherwise the OBIRCH  signal will be distorted as the current in the DUT exceeds the  OBIRCH system clamp’s limit. Thus, a new methodology was  implemented to improve OBIRCH signal sensitivity for hard  short failures. An external resistor (Re) is being added serially  between the biased failing pin and the positive input terminal of  the OBIRCH system to create a higher ohmic path so current in  the DUT will not exceed the OBIRCH system clamp limit as  shown in blue and brown colour I-V curves in Fig. 3. It helps to  improve ∆I detection during failure analysis of a short as  current alteration will be well below the clamp limit in the  OBIRCH system. Fig.4 shows the setup of an external  resistance (Re) in the OBIRCH system.

![I-VCharacteristics  30  20  20  0.05V  30  -1.5   -1_0   -0.5   0_0   0.5   1.5  Voltage,V  VCC w.r.t Vss (Original)   VCCw.r.tVss(+500ohm)  VCCw.r.tVss（+100ohm）  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c8f54f93-642d-48db-81bd-47b1ce104b75/c8f54f93-642d-48db-81bd-47b1ce104b75.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215707%3B1743219307&q-key-time=1743215707%3B1743219307&q-header-list=host&q-url-param-list=&q-signature=13efdbd858fad66eedf938302368769582a6d60e)
Fig. 3 Electrical behavior of DUT circuitry after implementation of External  Resistance (Re).

![Laser:=1.3um  Laser(frontside)   LeakageCurrentPath  RRe  A1  -(△R/V)P  Si-sub  △T,TCR  Laser(backside)   dson defectsand mate  1:Currentbeforelaserirradiation   DefectsinMetal Line  V：Appliedvoltage  I:Current change dueto laser irradiation(when constantvoltage is applied)  △R:Resistance increasewiththe temperatureincrease duetolaserirradiation  T:Temperature increase due to laser iradiation  TCR:Temperaturecoefficientofresistance  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5673f395-0356-4dda-b0f6-07d53998a08c/5673f395-0356-4dda-b0f6-07d53998a08c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215707%3B1743219307&q-key-time=1743215707%3B1743219307&q-header-list=host&q-url-param-list=&q-signature=e4456ecef42b23d4f701a78c8b46c692de285722)
Fig. 4 Setup of External Resistance in OBIRCH system.

## II.   EXPERIMENTS  

Several experiments were done to investigate the effectiveness  of this methodology. In the experiment, we did not use the Lock  In feature in the OBIRCH system but only normal continuous  signal capturing. Constant voltage OBIRCH amplifier under  Hamamatsu iPhemos SD A8755 series was used in first and  second experiments, whereas ASP-2000 model from  Checkpoint Technologies was used in third and fourth  experiments.

First experiment was conducted to investigate the effectiveness  of the new methodology. Three different test cases were set up  which were: resistor free, 430ohm resistor added and 820ohm  resistor added. Initial resistance Ri was measured after the DUT  was connected to the OBIRCH system with 1V biased at the  failing pin at room temperature. During this measurement, no  external resistance Re was connected in between the DUT and  the OBIRCH system.

The second experiment was conducted with the objective of  finding the optimal resistance value for the most sensitive spot.  Twelve test cases were set up for this purpose. Constant voltage  of 2.5V was biased to the failing path, with twelve different  resistance values tested respectively. The initial resistance Ri  was measured after the DUT was connected to the OBIRCH  system with 2.5V biased at the failing pin at room temperature.  During this measurement, no external resistance Re was  connected in between the DUT and the OBIRCH system.

The third experiment was conducted to measure effectiveness  of the external resistance to the total current alteration in the  OBIRCH system. Constant voltage of 0.5V was biased to the  failing path, with eleven different resistance values tested  respectively. The initial resistance Ri with value of 523.0 ohm  was measured after the DUT was connected to the OBIRCH  system with 0.5V biased at the failing pin at room temperature.  During this measurement, no external resistance Re was  connected in between the DUT and the OBIRCH system.

The fourth experiment was conducted to measure effectiveness  of the external resistance to enable laser irradiation in the  OBIRCH system during hard short circuitry analysis. One short

sample with only 3.6 ohms of initial Resistance Ri was selected  to perform experiments.

## III. R ESULTS AND DISCUSSION 

First experimental results clearly showed that the OBIRCH  spot sensitivity improves with the external resistance being  added to the failing DUT circuitry. Fig. 5 below shows the  sensitivity of the OBIRCH spot improved with additional  resistance injected into the failing path.

![Original   +430ohm   +820ohm  Nondsagnacduieto   Noinesagnacaueto   None sagnacatieto  Actual OBIRCH signal at   Actual OBIRCH signal at  defectlocation   defectlocation.  Capturemore  OBIRCHSi   sistanceReintoDuTcircuit  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/542aa52f-6764-49ea-a469-54d337e87797/542aa52f-6764-49ea-a469-54d337e87797.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215707%3B1743219307&q-key-time=1743215707%3B1743219307&q-header-list=host&q-url-param-list=&q-signature=d751f7732a9006d1ab251f6af1b29ceea10b7674)
Fig. 5 Experimental results showed OBIRCH spot sensitivity improved with  external resistance (Re) injected into the failing path.

When no external resistance is added into the DUT circuitry,  the OBIRCH system only detected a noise signal at the bond  pad of failing pin. After external resistance (Re) was added into  the DUT circuitry, the OBIRCH system successfully detected a  signal at the defective location. This finding also increased the  subsequent success rate for the die de-processing step in  physical failure analysis.

![=902.88  2-50  Conage   1.90m  Colane  2.511  Voltage-2.51   Voltage=2.50V  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a73bd9e2-72b0-4ba0-b59d-9a9cb45c1a8a/a73bd9e2-72b0-4ba0-b59d-9a9cb45c1a8a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215707%3B1743219307&q-key-time=1743215707%3B1743219307&q-header-list=host&q-url-param-list=&q-signature=3effdb296d09341d4578d7c9d825e8fe86371db4)
Fig. 6 Experimental results show the OBIRCH spot sensitivity difference at  various resistance levels.

For the second experiment, the results showed that the  OBIRCH spot was dispersed and not significant when there was  no additional resistance being added, while it became most  sensitive when the total resistance was close to 2500 ohm,  where the current value was 1mA. See Fig. 6 and Fig. 7 for  more information. This experiment showed that the additional  resistance injected into the DUT circuitry managed to affect  signal detection in the OBIRCH system.

|NO-|Voltage (V)|        Initial Resistance,                Ri(ohm)      |        Add-on Resistance,                Re(ohm)      |        Current                (mA)      |Signal|
|---|---|---|---|---|---|
||2.5|902.88||2.78|Min|
||2-5|902.88|100|2.32|Min|
||2-5|902.88|360|1.90|Min|
||2.5|902.88|820|1.39|Medium|
||2.5|902.88|1500|1.04|Max|
||2-5|902.88|2000|0.86|Max|
||2.5|902.88|2400|0.74|Max|
||2.5|902.88|6000|0.37|Medium|
||2-5|902.88|7500|0.31|Medium|
|10|2-5|902.88|8200|0.28|Medium|
||2.5|902.88|24000|0-11|Min|
|12|2.5|902.88|240000|0.01|2O|


Fig. 7 The OBIRCH spot is most sensitive when the total resistance is close to  2500ohm, where the current value is 1mA.

![DefectROI&OBIRCH signal   Defect ROI&OBIRCH signal  confidential circuitry  1x magnification (Original )   1xmagnification(+2kohm)  5x  anificationview  DefectROl&OBIRCHsignal  confidential circuitry  5xmagnification(Original)   5x magnification (+2k ohm)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b662853d-e9e6-4969-9aac-53017769d60d/b662853d-e9e6-4969-9aac-53017769d60d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215707%3B1743219307&q-key-time=1743215707%3B1743219307&q-header-list=host&q-url-param-list=&q-signature=b957776f32f71b26dff52802a8adcfbca078378f)
Fig. 8 Comparison between 1x & 5x magnification OBIRCH signal with &  without Re in DUT.

Fig. 8 shows OBIRCH analysis with 5x magnification  performed at the suspected failing region-of-interest (ROI) in  the second experiment, which demonstrates the effectiveness of  the external resistance Re implementation.

![Original   +500ohm  Background   OBIRCH Spot No.3  noise signal  OBIRCH Spot No.2  NoiseSignal  fromfailing   OBIRCH Spot No.1  pn  Magnification:5X  Voltage bias=0.5V   SpotA   SpotBSpot C  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c003829f-fe9d-4303-a754-ae37443f341e/c003829f-fe9d-4303-a754-ae37443f341e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215707%3B1743219307&q-key-time=1743215707%3B1743219307&q-header-list=host&q-url-param-list=&q-signature=4bfded322b47718a56c6fb4603c5e2cca1db6e37)
Fig. 9 Experimental results show the changes in OBIRCH spot pattern after  external resistance is added.

For the third experiment, the results showed that the three  OBIRCH spots were dispersed and surrounded by noise signal  when there was no additional resistance being added. After  external resistance (Re) with 500 ohm was added into the DUT  circuitry, all three OBIRCH spots became more concentrated  and solid as showed in Fig. 9.  Profile plot analysis was applied  at OBIRCH spot No.1 location to further analyze the  effectiveness of the external resistance to the total current  changes in the OBIRCH system. The profile plot is a cross  section on the line across the OBIRCH spot No.1. The Y axis is  total current changes due to laser irradiation and measured in  value of   $\upmu\mathrm{A}$  and X axis is pixel position measured in value of   $\upmu\mathrm{m}$  . Noise Boundary level is calculated with approximately   $45\%$   of total captured signal in every profile plot analysis at the  OBIRCH spot location. The current changes due to laser  irradiation is calculated with reduction of the background noise  from the profile plot results.

![Profile Plot analysis  Original  Background  noiselevel  45%oftotal  signalcapture  798.8HA  Background noise  boundary level)  Aldueto  laser  Ium irradiation  Pixel position, μm  DBIRCH SpotNo.  SpotA   SpotB   Spotc  +500ohm  Background  noiselevel  45%oftotal  signalcapture  11004.69uA  Background noise  boundarylevel)  △ldueto  laser  μm irradiation  OBIRCHS  SpotA   SpotB   SpotC  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5cfc2fea-3445-4d00-88c0-ba5f06ca0ac5/5cfc2fea-3445-4d00-88c0-ba5f06ca0ac5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215707%3B1743219307&q-key-time=1743215707%3B1743219307&q-header-list=host&q-url-param-list=&q-signature=4559071945460b1c03f3be4739faaa480065fefd)
Fig. 10 Profile plot results at OBIRCH spot No.1 without Re & with 500 Ω in  DUT.

Fig. 10 compares the profile plot results at the OBIRCH spot  location No.1 between with and without Re in DUT. This  experiment showed that when no Re is added into the DUT  circuitry, the OBIRCH system only detect the highest current  changes in Spot B whereas lower current changes in the Spot A  & Spot C. After external resistance (Re) with 500 ohm was

added into the DUT circuitry, the current changes at the Spot A,  Spot B and Spot C were decreased in value.

|NO.|        Add-On                Resistance,Re                （ohm)      |        OBIRCH                SPOTA,                A      |        OBIRCH                SPOTB,                A      |        OBIRCH                SPOTC,      |        Boundary level for                Background Noise,      |        lat                OBIRCH                SpotA,      |        lat                OBIRCH                Spot B,                A      |        Alat                OBIRCH                SpotC,      |
|---|---|---|---|---|---|---|---|---|
|||790|186.3|631.8|798.835|8.835|612.535|167.035|
||100|885.9|591.7|847.1|926.265|40.365|334.565|79.165|
||200|928.5|751.2|859.2|943.04|14.54|191.84|83.84|
||300|937.1|841.9|903.1|983.855|46.755|141.955|80.755|
||400|957.6|979.9|931.6|1024.22|66.62|44.32|92.62|
|6|500|968.9|919.1|888.2|1004.69|35.79|85.59|116.49|
||600|872|925.6|934.2|997.4|125.4|71.8|63.2|
||700|670.4|404.6|461.9|952.07|281.67|547.47|490.17|
||800|551.9|385.8|206.4|862.88|310.98|477.08|656.48|
|10|900|754.5|493.9|458.9|866.505|112.005|372.605|407.605|
||1000|988.7|981.8|988.7|1046.81|58.11|65.01|58.11|


Fig. 11 Table above show the results of total current changes at the Spot A, B  and C at various Re values.

![700  600  500  400  HO   300  200  100  200   400   600   800   1000   1200  Add-onResistance,Re(ohm)  =OBIRCHspotA  =OBIRCH spotB  OBIRCHspotC  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/298a5e1e-0512-477f-8830-7523139a068a/298a5e1e-0512-477f-8830-7523139a068a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215707%3B1743219307&q-key-time=1743215707%3B1743219307&q-header-list=host&q-url-param-list=&q-signature=c38900961e8c14ed1540e22d03d68bcd44989b82)
Fig. 12 Relationship between Re resistance value with total ∆I due to laser  irradiation at the OBIRCH spot A, B and C.

From the graph Fig. 12 above, it shows that the different Re  value added into the DUT can affect the total value of current  changes at each OBIRCH spot locations. The experimental  results clearly show that why only Spot B detectable when Re  value is  $\leq200$   ohm added into the DUT circuitry, it is because  the OBIRCH signal at Spot B is too strong and exploited to  observe signals came from the Spot A and Spot C. In this case,  when the Re value with range of   $400~\mathrm{ohm}\leq\mathrm{Re}\leq600$   ohm, is  added into the DUT circuitry, fault isolation at transistor level  based on OBIRCH signal can be analyzed more precisely due to  the small and concentrated OBIRCH spot size. The  experimental results also showed that OBIRCH user was able to  manipulate the signal detection in the OBIRCH system by  implementing an external resistance (Re) into the DUT  circuitry.

The fourth experience was conducted on one shorted sample  with only 3.6 ohm resistance. The biasing voltage supply could  only go up to 0.052V with the current clamping at 20mA for  this sample. The experimental results showed that higher

voltage input could be used with this methodology, which  provided a solution for insensitivity of the OBIRCH analysis  due to a voltage input limitation.

![Original   + Re =10 ohm   + Re = 20 ohm  Ri=3.60Q   Ri + Re = 13.5 Q   Ri + Re = 23.5 Q  Vmaxbias=0.052V   Vmax bias = 0.2V   Vmax bias = 0.42V  OBIRCH spot   OBIRCH spot   OBIRCH spot  Limt 30 0   Limt30.0   17.9m  57.0m   420.0mV  1Oso   2   23.50hm  Vmax Bias = 0.052V   VmaxBias=0.2V   VmaxBias=0.42V  o511   03H [51KH   DentDC   Dument:DC   CumontDC  CmsntC  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/07e43c0a-66da-49ac-9e6b-d2a0be08978a/07e43c0a-66da-49ac-9e6b-d2a0be08978a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215707%3B1743219307&q-key-time=1743215707%3B1743219307&q-header-list=host&q-url-param-list=&q-signature=b090da728d90c3db39282afaeeee71503dde89e4)
Fig. 9 Image above shows the value for maximum voltage bias into the DUT  circuit, which increases after external resistance is added.

As result, we could express current change (dI) or relative  current change (dI/I) function of Ri (internal resistance), Re  (external resistance) and dR (defect resistance variation under  laser stimulation) to appreciate the interest of Re. When no laser  stimulation on device,   $\mathrm{I}0=\mathrm{V}/\left(\mathrm{Ri\Omega+Re}\right)$  . When laser stimulation  on device,   $\mathrm{I}=\mathrm{V}/$     $(\mathrm{Ri\mathrm{~+~}R e\mathrm{~+~}d R})$  ). Therefore, current change  detected by the OBIRCH machine is   $\mathrm{{d}I=I-I0=V}$   (  $.1/(\mathrm{Ri}+\mathrm{Re}$     $+\ \mathrm{d}\mathrm{R})-1/(\mathrm{Ri}+\mathrm{Re}))$   and with usual approximations,

$\mathrm{d}\mathrm{I}={\tt-}\,(\mathrm{V}/(\mathrm{Ri}+\mathrm{Re}))\mathrm{dR}/$     $\left(\operatorname{Ri+Re}\right)$   and   $\mathrm{{d}I/I=\mathrm{{d}R/\left(R i+R e\right)}}$  .

In general, adding an external resistance to the failing DUT  circuitry did not change the behavior of the defective part as the  defect heated by the laser will have the same resistance change.  Therefore, the improvement noticed in the experiments was  from current alteration detection of the OBIRCH system.

## IV. C ONCLUSION 

The experimental results clearly showed that the OBIRCH  spot sensitivity improved with the additional resistance being  added to the target path. These findings validated the hypothesis  and proved to be effective in enhancing the success rate of short  circuit failure localization by OBIRCH. There are some  improvements planned on this methodology which are still  work in progress. One investigation of interest is to understand  why external resistance only takes effect when it is connected to  the positive terminal of the OBIRCH system but no effect was  observed when connected to the negative terminal of the  OBIRCH system.

## A CKNOWLEDGMENT 

The authors would like to thank Intel PSG & PG 7 FA team  members for their motivation and support.

## R EFERENCES 

[1]    K. Nikawa, “Optical beam induced resistance change (OBIRCH):  overview and recent results” IEEE Trans. Electron Devices, vol. 2,  pp. 742-743, October 2003.    [2]    https://hamamatsu.com/resources/pdf/sys/SSM0003E_PHEMOS10 00.pdf    [3]    Falk, R.A, "Advanced LIVA/TIVA Techniques", Proceedings of the  27th International Symposium for Testing and Failure Analysis,  Materials Park, Ohio: ASM International: 59–65, 200.    [4]    Nikawa, K; Tozaki, S, "Principles Novel OBIC Observation Method  for Detecting Defects in Al Stripes Under Current Stressing",  Proceedings of the 19th International Symposium for Testing and  Failure Analysis, Materials Park, Ohio: ASM International:  303–310, 1993.    [5]    K. Nikawa, S. Inoue, K. Morimoto, S. Sone, "Failure analysis case  studies using the IR-OBIRCH (infrared optical beam induced  resistance change) method", Proceedings of 1999 Asian Test  Symposium (ATS'99).

