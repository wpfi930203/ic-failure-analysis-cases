---
title: "222_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_36ec78d507dbed13647f928c5af7b7127295230462135641
file_size: 1024809
---

## The Application of Thermal Sensor to Locate IC  Defects in Failure Analysis  

Kuan-Chieh Huang, Yi-Chen Lin    Reliability & Failure Analysis Department, Powerchip Semiconductor Manufacturing Corp.  No. 12 Li-Hsin Rd. 1, Hsinchu Science Park, Hsinchu, Taiwan, R.O.C    Phone: 886-3-5795000 EXT.4864   Fax: 886-3-5792142   Email: rogerkc@powerchip.com

Abstract -  Precise defect positioning by EFA has become critically  important for yield improvement due to the reduction in CMOS  size and the increase in complexity. Some kind of leakage current  caused by metal defects could not be detected by conventional  Photo emission microscope (like InGaAs EMMI), because the  InGaAs detector responds to near-infrared light (NIR); therefore,  the Lock-in thermography (LIT) equipped with the InSb camera is  used for the detection of mid-infrared wavelength (MIR), and has  better sensitivity in the heat dissipation. The LIT system has been  proven to be very useful in 3D packaging or PCBs failure analysis.  In this article, we utilize the sensitivity of LIT system and compare  the emission differences between EMMI and LIT in three different  cases. By understanding the characteristics of the LIT system in IC  detection, we realized the emission differences it represents and  have succeeded in positioning the defect location and finding the  real reason for failure.

Keywords - EFA ； PEM ； LIT ； Leakage current

## I. Introduction  

In IC fault analysis, we often use Photo emission microscope  (InGaAs EMMI) or OBIRCH tool to locate the defect position.  In most cases, we can receive the defect signal and delayer it by  PFA skill to find the reason of failure. However, in some of the  function tests, the complexity in power condition for activating  the function circuit limits the use of the OBIRCH machine, and  leaves EMMI as the only option for EFA. But, in a short circuit  defect, using EMMI is not suitable for detecting the leakage  current induced by the metal, and might mislead the engineers to  false transistors activated by the leakage current. This only leads  to detecting abnormal AA damages caused by the leakage  current, but the main cause of the low yield remains unknown.

Therefore, in the absence of OBIRCH, we need another EFA  tool for detecting metal defects. Lock-in thermography (LIT)  has been widely used in 3D integration packaging for failure  analysis, ex: inter die crack, pin leakage, etc. Since its detector is  of InSb material, the corresponding quantum efficiency would  respond in the mid-infrared (MIR) ranges, which make it very  useful in detecting several millimeters thick of encapsulation die  fail, or in detecting the heat radiation emitted by the metal defect  in ICs.

In this article, we used Thermo Fisher ELITE system for LIT  and Hamamatsu InGaAs EMMI for PEM. LIT senses the  temperature difference caused by defects and operates similarly  to InGaAs EMMI. However, due to the differences in both  cameras, InSb camera can cover the same analysis sample with  different spectral response. Therefore, by discerning the EFA  results between PEM and LIT, we can successfully narrow

down the defect area. Below we will briefly introduce the  principles of PEM and LIT.

## II. Methodology and system configurations  

In general, after sample tests according to the Fail Bin, we  can wire up the failure pads for the following EFA analysis. The  commonly used PEM are CCD EMMI, which is made of Si  material, and InGaAs EMMI, which is made of InGaAs  compound. The material characteristics of the detectors will  determine its spectral response to the photons emitted by the  defect. For example, CCD EMMI has a spectral response in the  ranges of the 0.35um-1.1um wavelengths; while the InGaAs  EMMI has spectral response to   $0.9\mathrm{{um}{-}1.7\mathrm{{um}}}$   wavelengths.  Because Si energy gap   $(\mathrm{Eq}{=}1.12\mathrm{eV})$   is broader, it makes CCD  EMMI less sensitive in scaling down IC.

The LIT has a camera material of InSb, making its spectral  response in the 3um-5um wavelength ranges of MIR. Therefore,  it can sense different wavelengths by defects compared to PEM.  Figure 1 shows the quantum efficiency of InGaAs and InSb in  different wavelength regions.

![—InGaAs   InSb  100%  ()    80%6  6096  4096  2096  06  Wavelength (um)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ed9ade58-16d7-4388-8d11-94de57b025cc/ed9ade58-16d7-4388-8d11-94de57b025cc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215661%3B1743219261&q-key-time=1743215661%3B1743219261&q-header-list=host&q-url-param-list=&q-signature=dd4b0c9153a91608819bb42e169fb041e39539c1)
Fig.1: InGaAs and InSb Quantum Efficiency to Wavelength

In addition, one benefit of LIT is that OBIRCH uses external  laser power to activate the defect, and detects the changes in  resistance around the defect. Under the premise of adding laser,  the structure of the multi-layer metals prevent the laser power  from penetrating and reaching the layer of the defect position,  and thus limit the defect detection capability of OBIRCH. In the  application of LIT, for the defect hot spot is self-illuminated by  voltage, the heat can transmit to the IC surface and be detected

by the LIT system. As shown in Figure 2, on the left is the LIT  detection mode, and on the right is the OBIRCH Laser blocked  by upper metal.

![Insb   OBIRCH    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/33fbf0fd-5ab5-4e0c-9d4a-213d358dd32b/33fbf0fd-5ab5-4e0c-9d4a-213d358dd32b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215661%3B1743219261&q-key-time=1743215661%3B1743219261&q-header-list=host&q-url-param-list=&q-signature=ca30217479e1d6aaf1ca017ea78b7d45c04482f8)
Fig.2: Direct defect IR detected by LIT, and OBIRCH Laser blocked by metals

## III. Results and Discussion 

In the following cases, due to EFA functional test limitation,  we could only apply PEM and LIT without OBIRCH. However,  in past EFA experiences, we knew some PEM analysis results  would lead to AA damages discussed in [1] like Figure 3: the  damage was caused by the back end of line (BEOL) metal defect  during the EFA test. In order to find actual root cause, we  needed to trace the abnormal transistors back to each connecting  layer and inspect larger areas for PFA analysis. Therefore we  applied LIT in this situation and compared the EFA results  between PEM and LIT.

![AA damage  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/27551272-8bc9-420c-b6d3-3c4a19e04a54/27551272-8bc9-420c-b6d3-3c4a19e04a54.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215661%3B1743219261&q-key-time=1743215661%3B1743219261&q-header-list=host&q-url-param-list=&q-signature=0136ee4915d6018357c4569dfd29f6612ad55d74)
Fig.3: short circuit induced AA burn-out

## IV. Case 1: PEM multiple spots induced by short circuit  

In case 1, we measured the stand-by current of Reference  Die and Fail Die as shown in Table I. We found that Fail Die had  significant leakage current under power-on conditions, so we  performed PEM analysis.

Table I- Reference Die and Fail Die leakage current

|Sample|lovcc = 1.8V|VSP=5V|VSN=-5V|
|---|---|---|---|
|Reference Die|9mA|0.18uA|-100nA|
|FailDie|7.8mA|91mA|-1.7mA|


As shown in Fig.4, after the PEM measurement, we found  emission spots at point E, but when we zoomed in further to  point E, we found that it was consisted by multiple transistors in  different locations. We suspected that there were two  possibilities for the failure. The first one is, all those transistors

are abnormal; the second is, defects in the BEOL metal layer  cause those transistors to behave abnormally.

However, based on past experience, the possibility of all  transistors abnormal was rare, so we suspected that the main  cause of failure was the BEOL metal defect. For this kind of  PEM spots, in order to find out the suspicious metal layer,  engineers needed to perform metal tracing on the PEM spots to  find all possible metal routes that were connected to the  transistors.

![Point E  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b8f342b0-cf9e-427b-b863-15d9e430febf/b8f342b0-cf9e-427b-b863-15d9e430febf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215661%3B1743219261&q-key-time=1743215661%3B1743219261&q-header-list=host&q-url-param-list=&q-signature=f5a139864def5b788ada64708e4d71a687aa4787)
Fig.4: The multiple PEM spots at point E

The connected metal routes could be over several  millimeters, which would enlarge the PFA areas. Also, the PFA  location positioned by the rough layout tracing would result in a  high missing rate and prolong the PFA cycle. Therefore, in the  case where OBIRCH could not be applied, we used LIT to detect  the mid-infrared light emitted by BEOL metal defects. As a  result, the LIT hot spots shown in Figure 5 showed additional  spot information. Among them, Line_AB and Line_CD  represented heat paths, and point E had the same spot location in  LIT, same in PEM.

![LT  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/81a3317a-a9c7-461d-a7f7-64512f20c2b6/81a3317a-a9c7-461d-a7f7-64512f20c2b6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215661%3B1743219261&q-key-time=1743215661%3B1743219261&q-header-list=host&q-url-param-list=&q-signature=14b24a1087a8710cc46b3470c5004d25681cea26)
Fig.5: The LIT hot spots

By comparing the EFA results in both, we found that the LIT  system could sense additional hot spots along Line_AB and  Line_CD. Therefore, we performed PFA in the range of  Line_AB, Line_CD and point E; and the PFA result found 3M  short circuit respectively at endpoint B and endpoint D, as  shown in Figure 6 and Figure 7.

![PointB  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5cf2852f-c253-4e75-b8c3-5cd95b805756/5cf2852f-c253-4e75-b8c3-5cd95b805756.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215661%3B1743219261&q-key-time=1743215661%3B1743219261&q-header-list=host&q-url-param-list=&q-signature=f65f83603d95d425565b50e6ea930f09b1bd1780)
Fig.6: PFA found short circuit at endpoint B

![Point D    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b9d4d1ad-b1a7-41db-b728-cb0cd6de241c/b9d4d1ad-b1a7-41db-b728-cb0cd6de241c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215661%3B1743219261&q-key-time=1743215661%3B1743219261&q-header-list=host&q-url-param-list=&q-signature=7a96f0add7d03bc88b7c3d6e630504d7270c1321)
Fig.7: PFA found short circuit at endpoint D

For point E, no defect was found in 3M and, after a layer by  layer check, we only saw AA damages similar to the one in  Figure 3.

In this case, we combined different EFA tools to find out the  possible defect signals, which would help us to narrow down the  failure area and save us time from difficult layout tracing. We  also noticed two significant differences between LIT and PEM  hot spots. One was, the hot spot showed a linear path in LIT; and  the other was, the defect position was not at the brightest point.

We came up with an explanation by looking at the Line_AB  hot spot shown in Figure 8.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/24d521a2-2070-4e32-a9e5-cd01daafeabf/24d521a2-2070-4e32-a9e5-cd01daafeabf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215661%3B1743219261&q-key-time=1743215661%3B1743219261&q-header-list=host&q-url-param-list=&q-signature=688e0309e48b710c5bbeed5a66b7e08967303b2b)
Fig.8: 5X magnified LIT of the Line_AB hot spot

Normally, when we find the PEM spots, we could  reasonably narrow down the hot spot to the brightest location  and delayer it accordingly. However, in LIT system we observed  that in Line_AB, the hot spot of point A was brighter than that of  point B. Therefore, if the PFA delayer was narrowed down to the  brightest point of the LIT signals, only point A would remain  and the actual short circuit defect of point B would be missed.

Accordingly, in order to understand why we could not  narrow down the hot spots, we inferred from the following  mechanism, Figure 9. The original normal circuit can be  assumed as Logic_X, with serial transistors of resistance R1 and  supplied by voltage V, having current I1 (by ohm’s law).

![Loglc_x  2M\~1M  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7a3679d2-23ea-4b3d-88ec-700034c3c861/7a3679d2-23ea-4b3d-88ec-700034c3c861.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215661%3B1743219261&q-key-time=1743215661%3B1743219261&q-header-list=host&q-url-param-list=&q-signature=a53efe293ffc227e4aae4b6d96c8ede5c4fd9250)
Fig.9: Schematic diagram of a normal circuit

When short circuit occurred in Figure 10, the input voltage V  was not affected; but the short circuit would create a lower  resistance conducting path, which could be assumed as the

Logic_Y circuit with a resistance of R2. In this condition, we  could assume that Logic_X and Logic_Y were parallel  connected circuits and, because Logic_Y is induced by the metal  defect, the defect circuit of the resistance R2 would be smaller  than the resistance R1, connected with many transistors. In other  words, more currents would be distributed to Logic_Y, and that  would allow us to detect abnormal heat dissipation on the  Line_AB path. This explained why a linear heat path was seen  on the LIT results.

Next we wanted to know why endpoint B was the actual  defect location in Line_AB but was “NOT” the brightest point.

![3M short  Loglc_x  Loglc Y  2M\~1M   2M\~1M  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/73bb1166-72d0-4f59-8a26-ff25d7cdd5bc/73bb1166-72d0-4f59-8a26-ff25d7cdd5bc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215661%3B1743219261&q-key-time=1743215661%3B1743219261&q-header-list=host&q-url-param-list=&q-signature=d9184e848e563ce90e8a4cff79d5063cf9845e91)
Fig.10: Schematic diagram of the short circuit

We checked the 3M layout of endpoint A and endpoint B in  Figure 11. We observed that the brightest endpoint A,  corresponded to the structure with connecting via to 2M, while  endpoint B didn’t. From the view of power dissipation (Power   $\mathrm{=}\mathrm{I}^{2}\dot{\mathbf{R}})$  , we know that the resistivity of the Via_Tungsten is   $5.6\mathrm{E}{\cdot}8(\Omega^{*}\mathrm{m})$   which is larger than the resistivity of the  Metal_Aluminum,   $2.8\mathrm{E}{\cdot}8(\Omega^{\ast}\mathrm{m})$  . It would produce more heat  consumption in the tungsten via than to the metal line due to the  characteristics of the metal materials and the physical  dimensions. In the end, we found the brightest hot spot to be at  endpoint A, but it was irrelevant to the defect location.

![月月月月月月日月月月月 ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1392c01a-cf15-47f3-b40f-d4f4c47448f4/1392c01a-cf15-47f3-b40f-d4f4c47448f4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215661%3B1743219261&q-key-time=1743215661%3B1743219261&q-header-list=host&q-url-param-list=&q-signature=d5e402c67df0fc329cef540fce7d1d76061b886c)
Fig.11: Endponit A and B corresponding to upper vias

## V. Case 2: Abnormal PEM spots induced by IMD defect  

If the brightest hot spot was just caused by the resistance  difference in LIT results, could we pay attention only to the  endpoint of the linear EFA path? Case 2 is a good example to  explain another defect possibility.

In case 2, we measured the stand-by current of Fail Die  shown in Table II. Under the different leakage current between  Reference Die and Fail Die, we performed PEM analysis.

Table II- Reference Die and Fail Die leakage current

|Sample|lovcc = 1.8V|VSP=5V|VSN=-5V|
|---|---|---|---|
|Reference Die|2.1mA|0.2uA|-100nA|
|FailDie|17mA|0.3uA|-100nA|


As shown in Figure 12, we found two PEM spots in the  Logic area, and EFA results looked similar to case 1, so we used   LIT to check whether there was other suspicious point.

![PEM  Rd  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/61234b6d-9b8d-42d1-8d1a-c2befb0c1ab2/61234b6d-9b8d-42d1-8d1a-c2befb0c1ab2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215661%3B1743219261&q-key-time=1743215661%3B1743219261&q-header-list=host&q-url-param-list=&q-signature=8bb684b4aa002db1515f0a010324d2f906d3c1ab)
Fig.12: The PEM spots

The LIT results are shown in Figure 13. We found additional  points A and B around L point, which was the same in PEM, so  we performed PFA delayering at the endpoints A, B and L.

![LT  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/48db6ef1-cc65-4a00-94cb-6d8cc0d8f007/48db6ef1-cc65-4a00-94cb-6d8cc0d8f007.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215661%3B1743219261&q-key-time=1743215661%3B1743219261&q-header-list=host&q-url-param-list=&q-signature=3ad5a1c6c0ca93f2d323f6c99b61da055d5f653d)
Fig.13: The LIT hot spots

As shown in Figure 14, PFA found 1T IMD void at point A.  From the FIB cross section, we suspected that particles occurred  during the 1T oxide deposition and, after the subsequent photo  lithography and cleaning process, the particles were removed,  causing the following tungsten to fill into the particle void. The  abnormity of filled-in tungsten would result in poor isolation of  the surrounding oxide, and in LIT, the brightest hot spot was in  accordance to the filled-in tungsten defect.

![PFA  Cross section  2  IWDVO  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4782dc5e-213f-4cb1-837e-7896a1627480/4782dc5e-213f-4cb1-837e-7896a1627480.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215661%3B1743219261&q-key-time=1743215661%3B1743219261&q-header-list=host&q-url-param-list=&q-signature=da42c08238ecb1b702c742aef919dbb61a8af115)
Fig.14: PFA found IMD void at point A

In Case 2, as we have seen in PFA, the brightest hot spot was  caused by the tungsten defect. We could say that, in LIT results,  the hot spot intensity was related to the resistance changes or  different material characteristics in the defect circuit. Also, the  twisted heat path indicated that the poor IMD isolation was  weaken by the filled-in tungsten, and induced leakage current in  the surrounding areas.

In summary of the two cases of EFA and PFA results, we  understood some characteristics of the LIT application. Firstly,  if the defect occurred from a simple short circuit, it does not  necessarily appear at the brightest hot spot, and attention is  needed at the endpoint area. Secondly, if the defect is caused by  abnormal via issue, the hot spot can be detected as a twisted path.  By combining the EFA results of PEM and LIT, accurate defect  positioning can improve the hit rate.

## VI. Case 3: No signal detected by PEM  

The EFA positioning is very important for PFA delayering  because it provides a possible failure location to find the root  cause. However, if there is no valid PEM spot, the following  PFA can not proceed.

In case 3, there was a significant difference between the IV  curves in Figure 15. However, even though the leakage current  was so obvious; it was still unable to detect any abnormal hot  spots in PEM.

![7.E-02  Reference Die  6.E-02  FailDie  5.E-02  4.E-02  3.E-02  2.E-02  1.E-02  0.E+00  0.2   0.4   0.6   0.8   1.2   1.4   1.6  1.8  Voltage (V)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6f54ff7b-5de4-416a-9ea7-f4217ac76911/6f54ff7b-5de4-416a-9ea7-f4217ac76911.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215661%3B1743219261&q-key-time=1743215661%3B1743219261&q-header-list=host&q-url-param-list=&q-signature=6b280ff33fc5e35dbe98f90b05dc1b7b1a67af40)
Fig.15: Reference Die and Fail Die leakage current

No detectable signals in PEM bothered us, so we tried LIT  for a chance to find any possible hot spot. The result is shown in  Figure 16.

![LT  OX  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e4de78a0-839a-43b7-9ff4-cab148372075/e4de78a0-839a-43b7-9ff4-cab148372075.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215661%3B1743219261&q-key-time=1743215661%3B1743219261&q-header-list=host&q-url-param-list=&q-signature=cfcb281b6d60ed0ce92d062aab70bfcde959ec87)
Fig.16: The LIT results

In LIT, there was a suspicious hot spot so we performed PFA  at this area and found a 6M short circuit defect, Figure 17.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c6c55e12-934f-49a8-8a05-b4b95b8e28e8/c6c55e12-934f-49a8-8a05-b4b95b8e28e8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215661%3B1743219261&q-key-time=1743215661%3B1743219261&q-header-list=host&q-url-param-list=&q-signature=00b41a279285d4f107d1d4688f44920cd8149403)
Fig.17: PFA found 6M short circuit

In this case, the point of our attention was that, normally for  the short circuit defect, we could detect abnormal signals that  were induced by the leakage current in PEM. Once we had the  suspicious transistors, we could at least perform the layout  tracing and identify a possible area for PFA.

However, in case 3, no PEM signals could be found, so the  following PFA delayer could not continue. It meant that, in  some situations, LIT could play an important role in finding  abnormal signals due to its characteristic of the detector.

After finding the defect location, we examined the circuit  routing and noticed that the defect made a direct short circuit  from power line VDD to ground GND. By combining the results,  we could schematically illustrate the reason why there were no  signals detected in PEM.

The assumed original SRAM circuit is shown in Figure 18(a)  and the defect circuit is shown in Figure 18(b). For the  Reference Die in Figure 18(a), the voltage was biased at 1V and  the current was 43uA. Therefore, by ohm’s law   $\scriptstyle\mathrm{V=IR})$  , the  resistance of this SRAM circuit is roughly   $23\mathrm{K}\Omega$  . Under the  same conditions for the Fail Die, the leakage current was 11 mA  and the resistance of the defect circuit was roughly   $90\ \Omega$   in  Figure 18(b). As a result, in the event of defect, the defect could  produce an equivalent parallel resistance, which would make the  voltage consumption dissipate from the designed SRAM circuit  to the defect circuit. For the short circuit situation, since the  voltage consumption was mainly consumed at routing metal  lines, it would only produce heat dissipation in metal layers.  Eventually, for the high resistance SRAM region, there was no  enough power to drive the transistors on, and then induced a  detectable signal for PEM.

In this case, we learned that in short circuit situations, PEM  could not detect this kind of heat radiation and other solutions  were needed for the challenge.

![R1=23KQ   VDD   R1=23KQ   VDO  SRAM   SRAM  IR2=900  GND   GND  (a) Reference Dle   (b) Fail Die  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/db4f8914-7956-4b9b-9bb3-01edf52d0ee9/db4f8914-7956-4b9b-9bb3-01edf52d0ee9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215661%3B1743219261&q-key-time=1743215661%3B1743219261&q-header-list=host&q-url-param-list=&q-signature=3885665c7bc1e6bccebbf736aad6b483d055f6d6)
Fig.18: (a) schematic circuit of the normal SRAM (b) schematic circuit of the  short circuit loop

## VII. Conclusions  

In the increasingly complex circuit, a successful EFA is like  a guild map in telling us where the defect location is. However,  even for an obvious metal defect like case 3, PEM is unable to  detect this kind of failure mode and more options are needed for  this kind of situation. Through our studies, we have learned  more about LIT and can sum up the results into two conclusions.

1. For metal defect in LIT, the brightest hot spot does not  mean the actual defect location.

2. In LIT, the brightest hot spot is related to the characteristic  of the material.


By understanding the characteristics of LIT application, we  can easily find a possible defect location and skip the hard work  of the layout tracing in PEM.

In the future, we will learn more EFA differences between  LIT and PEM and, by knowing that, will build up EFA accuracy  and reduce our PFA cycle time.

## References  

[1] Ssu-Yu Wu, Yi-Chen Lin, Sheng-Min Chen, Shih-Hsuan Yang, “Failure  Modes Study of Active Area Damage with Two Identified Causes using  Multi-Analysis Methods”, IPFA. 2018.     [2] Jinglong Li; Gaojie Wen; Joe Yu; Grace Song, “Die-Level Leakage  Current Path Analysis Based on IR-OBIRCH Technology”, IPFA. 2012.    [3] D. Nagalingam, A.C.T. Quah, S. Moon, G.B. Ang, S.L. Ting, H.H. Ma, S.P.  Neo, Z.H. Mai, J.C. Lam,  “Defect Prediction Approach to enhance Static  Fault Localization of Functional Logic Failure Defects using NIR Photon  Emission Microscopy”,  IPFA. 2018.    [4] Wen Qiu., Bernice Zee, Brian Lai, Jim Vickers, David Tien, “Improved  Phase Data Acquisition for Thermal Emissions Analysis”, IPFA. 2018.

