---
title: "217_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_e8a9f1f88e2cde26dc91cdbf7b4bc9237295230462135641
file_size: 584347
---

## Case Study on Precise Boron Quantification of Mixed  Matrix  

Kian Kok Ong\*, Yun Wang, Han Wei Teo, Ramesh Rao Nistala and Zhi Qiang Mo  1 Department QRA-PFA, GLOBALFOUNDRIES Singapore Pte Ltd, 60 Woodlands Industrial Park D, Street 2, Singapore 738406.  \* Phone: +65 6670 1532 Fax: +65 6360 4370 \*Email: kenny.ong@globalfoundries.com

Abstract-   Material characterization tool, Secondary Ion Mass  Spectrometry (SIMS) with its high precision and reproducibility is  widely used to capture any abnormality in the dopant profile of  the implanted species caused by drift in implant processes or  equipment. The characterization usually is performed on setup  test wafer with a single matrix substrate (usually silicon  substrate). However, this quantification approach is not suitable  for a mixed matrix of the silicon substrate and silicon dioxide  (physical segregation structure). In this paper, it is shown that  accurate dosage quantification can be obtained using the proposed  numerical method.

Keywords  –  Quantification, Secondary Ion Mass Spectrometry,  Mixed matrix .

## I. I NTRODUCTION 

For Autonomous Vehicle Driving with full automation level  5 (driverless vehicle) [1], all the semiconductor components in  the vehicle need to meet stringent safety demands. Any failure  part in the vehicle poses a life-threatening situation and hence,  the automotive industry aims for zero-excursions zero-defect in  a wafer manufacturing plant. Semiconductor products inside  the automotive subsystem such as stability control, power train,  dashboard instrumentation, battery management, and engine  controls must be AEC-Q100 qualified that is built to bear the  extended grade temperatures under the hood which is either  Grade 0 (-40 C to  $+150~\textperthousand$  ) or Grade 1 (-40 C to  $+125\;\texttop\mathbf{C}$    [2].

The implant process, one of the many processes in wafer  manufacturing, the variations tolerance control become very  tight with zero margin error to meet the above automotive  industry requirement. This is because dopant fluctuation can  cause ineffective channel L, Vt shift, I On  / I Off  variation, and  many other device level issues. Periodically, a product wafer  after boron implantation followed by thermal annealing is  tested for any dopant profile abnormality which is highly  critical to ensure the subsequent process step going smoothly.

Material characterization tool, Secondary Ion Mass  Spectrometry   (SIMS)   with   its   high   precision   and  reproducibility is widely used to capture any abnormality in the  dopant profile of the implanted species caused by drift in  implant processes or equipment [3]. This characterization  usually was performed on a setup test wafer with a single matrix  substrate   (usually   silicon   substrate).   Accurate   dosage  quantifications are important for process control that meets or  exceeds the voice of customers (VOC). Many efforts have been  done by the SIMS community to obtain accurate dosage which

is straightforward when matrix-matched standards are available.  In such cases, the relative sensitivity factor (RSF) is used for  quantification, which is calculated using an ion implantation  sample with a known dose [3] [4]. The dosage in the implanted  sample is estimated using companion techniques, such as  double-crystal X-ray diffraction and Rutherford backscattering  spectrometry (RBS).

Mixed matrices often involve two different species or more,  for example, silicon germanium (SiGe), aluminium gallium  nitride (AlGaN), aluminium gallium arsenide (AlGaAs), and  many others. Accurate quantification can be obtained using  RSF as mentioned above with known-dose matrix-matched  implanted standards [5].

However, the RSF method does not apply to the cases where  there is a physical segregation structure of matrix components  such as silicon substrate and silicon dioxide as shown in Figure  1, which consists of a repeated pattern of the shaded area  corresponding to silicon dioxide and non-shaded area of silicon  substrate. The implanted dosage quantification for such  structure is difficult due to different ion yield enhancement  effect of secondary ions at oxide and non-oxide region.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/48e1bf99-415e-439c-9f25-93118d509826/48e1bf99-415e-439c-9f25-93118d509826.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215664%3B1743219264&q-key-time=1743215664%3B1743219264&q-header-list=host&q-url-param-list=&q-signature=c6842e3e444a2ba3aa02a49a723071d77a39d73c)
Fig. 1 Area of interest with the size of   $150\upmu\mathrm{m}\,\mathrm{x}\,150\upmu\mathrm{m}$   with shaded area silicon  dioxide (a %) and non-shaded area silicon substrate   $(\mathsf{b}\,\%)$  .

Some studies showed that high dynamic range of arsenic  profile is required to address the low concentration arsenic in  SiGe matrix by using AsSi -  cluster ions [6]. However, this  approach for quantifying arsenic in SiGe matrix suffered severe  mass interference to As -  and AsSi -  and therefore numerical

approach is used to eliminate the effect of mass interference.  The solution for the mass interference is to subtract the mass  interference based on the related intensity ratio using the  recombination model of the cluster ions formation [7]. The  correct intensity of AsSi -  can be calculated by subtracting the  mass interference from the intensity I 103   $\mathrm{^{74}G e^{29}S i^{-}}$  ,   $^{73}\mathrm{Ge}^{30}\mathrm{Si}^{-}$  ,   $^{74}\mathrm{Ge}^{28}\mathrm{Si}^{1}\mathrm{H}^{,}$  ,   $^{73}\mathrm{Ge}^{29}\mathrm{Si}^{1}\mathrm{H}^{,}$  ,   $^{72}\mathrm{Ge}^{30}\mathrm{Si}^{1}\mathrm{H}^{\cdot})$   after obtaining the  intensity ratio from an undoped SiGe standard sample; hence  accurate arsenic dosage can be obtained.

In this paper, the accurate dosage quantification is obtained  with reference to the application of the concept as mentioned  above. The relative contribution from the shaded area silicon  dioxide and non-shaded area silicon substrate to the ion signal  is considered based on relative area and the relationship of  silicon ion signal intensity at the oxide and non-oxide regions.

## II.   EXPERIMENTS  

A patterned wafer implanted with boron species followed by  thermal annealing is tested for any abnormality for the implant  process. SIMS analysis was performed using the impact energy  of   $5\mathrm{keV}$   (positive mode, oxygen ions as primary bombardment  ions) on the area of interest with the size of   $150\,\upmu\mathrm{m}\,\mathrm{x}\;150\,\upmu\mathrm{m}$   as  shown in Figure 1. The sputtering area and analysis area were   $150\upmu\mathrm{m}{\times}150\upmu\mathrm{m}$   and   $52\upmu\mathrm{m}$   in diameter, respectively to address  the crater effect. The shaded area is silicon dioxide structure  with   $(\mathrm{a}\%$   area) and the non-shaded area is silicon substrate  structure (  $\mathbf{\a}\mathbf{b}\mathbf{\%}$   area) where   $\mathtt{b}>>\mathtt{a}$  . Natural stable abundance  isotope   of   silicon   exist   with    $(^{28}\mathrm{Si}{\cdot}^{29}\mathrm{Si}{\cdot}^{30}\mathrm{Si})$     \~   $(92.2\%;4.7\%;3.1\%)$  . The detected secondary ions were   $^{30}\mathrm{Si}$   as  matrix reference isotope with respect to   $^{11}\mathbf{B}$   as species of  interest for dosage calculation. Ions were detected on electron  multiplier (EM) detector, in the range   $[10^{-1}\,:\,10^{6}]\,\mathrm{~c/s~}$   and  Faraday cup for range  $\scriptstyle[>10^{6}]\,\mathrm{c/s}$  . The primary ion beam current,  aperture, energy slits, etc. were adjusted to the condition that  when scanned over an area of interest, the secondary ions were  extracted from the area with electronic gating “ON” within EM  detector. Due to high ions yield enhancement from silicon  dioxide structure area,   $^{30}\mathrm{Si}$   being the lowest natural stable  abundance as matrix reference isotope is still detected on  Faraday cup while   $^{11}\mathrm{B}$   was detected in EM. However, this  would not affect the dosage calculation using RSF method with   $^{30}\mathrm{Si}$   as matrix reference isotope as it is generally known that a  linear transfer function relationship between EM and Faraday  cup typically existed. Moreover, calibration for this linear  relationship was done periodically.

## III. R ESULTS AND DISCUSSION 

Most of the boron is implanted on the non-shaded silicon  substrate structure   $({\mathfrak{b}}\%$   area) in this case. Implantation on  shaded silicon dioxide structure   $(\mathbf{a}\%$   area) is dependent on the  product requirements and often with different ion implantation  dosage and energy. Through the analysis performed on the  11 B-implanted silicon standard sample    $(100\mathrm{keV}$  , 1E14  atom/cm 2 ) [4] as shown in Figure 2, we had obtained the  relative sensitivity factor (RSF) value of  $x$   atom/cm 3  using   $^{30}\mathrm{Si}$    as a reference by point to point normalization. Both   $^{11}\mathbf{B}$   and   $^{30}\mathrm{Si}$    signal intensity is detected within the EM detector. A similar

analysis is also performed on   $^{11}\mathbf{B}$  -implanted on silicon dioxide  standard sample (  $.100\mathrm{keV}$  , 1E14 atom/cm 2 ) and the RSF values  are tabulated as Table 1. The   $^{11}\mathbf{B}$   signal intensity is detected on  the EM detector and   $^{30}\mathrm{Si}$   signal intensity is detected on the  Faraday cup detector.

Table. 1 RSF value comparison between silicon substrate and silicon dioxide.

|11B Implanted|Silicon Substrate Matrix|Silicon Dioxide Matrix|
|---|---|---|
|RSF [atom/cm3]|x|1.2x|


For SIMS analysis at the area of interest with mixed matrix,  when matrix effect is neglected and assumed as a single matrix,  the RSF value for a single matrix will be directly applied and  the calculated concentration profile is shown in Figure 3 (before  numerical calculation). Above method is valid if:

i.    Shaded area or non-shaded area is very small, which  almost negligible ion yield enhancement effect of  secondary ions.    ii.    The difference of ion signal intensity obtained from  the non-shaded area and the shaded area is very small.

However, the assumptions as mentioned earlier are not valid  when the shaded area (silicon oxide) cannot be neglected and  the effect of ion yield enhancement in a shaded area (silicon  oxide) is significant compared with that non-shaded area  (silicon substrate). Therefore, we proposed two scenarios for  accurate dosage quantification using numerical calculation.

![1.E+21   1.E+O7  1.E+06  1.E+20  1.E+O5  1.E+19  1.E+04  1.E+18   30Si   1.E+O3  1.E+O2  1.E+17  1.E+O1  1.E+16  1.E+OO  1.E+15   1.E-O1  500   1000  Depth(nm)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a6116fd8-4e21-4c0e-ac91-d5b5b62cf78c/a6116fd8-4e21-4c0e-ac91-d5b5b62cf78c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215664%3B1743219264&q-key-time=1743215664%3B1743219264&q-header-list=host&q-url-param-list=&q-signature=a5b5e01070456a9e78ffb8c0621f3616b38a9804)
Fig. 2 SIMS profile obtained from   $\overline{{{}^{11}\mathbf{B}}}$  -implanted silicon standard sample  (100keV, 1E14 atom/cm 2 ) using   $^{30}\mathrm{Si}$   as matrix reference isotope. Both   $^{11}\mathrm{B}$   and   $^{30}\mathrm{Si}$   signal intensity is detected on the same EM detector.

![2.50E+19  2.50E+18  Beforeanynumerical  2.50E+17   correction  2.50E+16  2.50E+15  2.50E+14  50   100   150   200   250   300  Depth（nm)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3964bbdd-6a1c-4e5c-84ed-b9bb106ce6dd/3964bbdd-6a1c-4e5c-84ed-b9bb106ce6dd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215664%3B1743219264&q-key-time=1743215664%3B1743219264&q-header-list=host&q-url-param-list=&q-signature=21aead71785f53f75ef31dd851ac4d87d6d7b5e7)
Fig. 3 SIMS profile obtained from the area of interest using   $\overline{{{}^{30}{\mathrm{Si}}}}$   as matrix  reference isotope. Boron dosage obtained = y  $[\mathrm{atom}/\mathrm{cm}^{2}]$   dosage. The  $^{11}\mathbf{B}$   signal  intensity is detected on the EM detector and  $\mathrm{^{30}S i}$   signal intensity is detected on  the Faraday cup detector.

Scenario-1: No boron implantation on shaded area silicon  dioxide of   $\mathbf{a}\%$  . The solution for this scenario is to subtract the   $^{30}\mathrm{Si}$   signal intensity interference from shaded area silicon  dioxide (a %) as there is no boron implantation on it. A  reference sample with a thin layer of  $\mathrm{SiO}_{2}$   (125Ǻ) was analyzed  and the ratio of intensity for   $^{30}\mathrm{Si}$   in silicon substrate:   $^{30}\mathrm{Si}$   in  silicon dioxide is  $\sim1\colon16$   as shown in Figure 4. The   $^{30}\mathrm{Si}$   signal  intensity detected on same the EM detector for both silicon  dioxide and the silicon substrate. With this information, the new  reference   $^{30}\mathrm{Si}$   signal intensity is calculated with the following  equation:

$$\begin{array}{r}{I_{n e w}=\frac{b*1}{b*1+a*16}*I_{30S i}}\end{array}$$
(1)

This new reference   $^{30}\mathrm{Si}$   intensity will be used with the  existing RSF value of  $x$   atom/cm 3  for the calculation of the new  boron dosage   $[\mathrm{atom}/\mathrm{cm}^{2}]$  . When boron signal intensity in the  mixed matrix is normalized by corrected  $^{30}\mathrm{Si}$   intensity (point to  point normalization), a more accurate boron dosage values are  tabulated in Table 2 and corrected depth profile is plotted as  shown in Figure 5.

This method showed three times   $y $  dosage   $[\mathrm{atom}/\mathrm{cm}^{2}]$  compared with that before numerical correction. The dosage  after numerical correction is also in close agreement with the  given process parameter.

Table. 2 Boron dosage value obtained with a comparison between before  numerical correction and after numerical correction for scenario-1.

|11B Implanted|Before numerical correction|After numerical correction|
|---|---|---|
|Dosage obtained [atom/cm2]|y|3y|


![5.E+05  Silicon dioxide  Silicon dioxide  (s/)   Silicon substrate  Silicon substrate  5.E+04  30si(Y)  5.E+03  10   15   20   25   30  Depth（nm）  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3779e8fb-0414-4435-9400-7f15d42dcae2/3779e8fb-0414-4435-9400-7f15d42dcae2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215664%3B1743219264&q-key-time=1743215664%3B1743219264&q-header-list=host&q-url-param-list=&q-signature=8ab4d6822966990a31c4c0cef78418fadc2abe48)
Fig. 4 SIMS profile obtained using  $^{30}\mathrm{Si}$   as matrix reference isotope of a thin  layer of 125Å oxide reference sample with ratio ion signal intensity at silicon  substrate and silicon dioxide 1:16. The  $^{30}\mathrm{Si}$   signal intensity detected on same the  EM detector for both silicon dioxide and the silicon substrate.

![2.50E+19  2.50E+18   Beforeanynumerical  correction  2.50E+17   -Afternumerical  correction  2.50E+16  2.50E+15  2.50E+14  SO   100   150   200   250   300  Depth(nm)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2ae323f5-a5cb-40a5-af3f-5ac80fd13f43/2ae323f5-a5cb-40a5-af3f-5ac80fd13f43.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215664%3B1743219264&q-key-time=1743215664%3B1743219264&q-header-list=host&q-url-param-list=&q-signature=e4472d70b5b563c416369ef522ab892070bf350c)
Fig. 5 SIMS profile obtained from the area of interest using  $^{30}\mathrm{Si}$   as matrix  reference isotope for scenario 1 (point to point normalization and comparison of  “before numerical calculation” and “after numerical calculation”). Corrected  boron dosage obtained  $=3y$   [atom/cm 2 ] dosage.

Scenario-2: There is boron ion implantation on the shaded  area of silicon dioxide   $\mathbf{a\%}$  . Straightforward subtraction is not  applicable and the solution is a mixed matrix RSF applied for  precise quantification of boron dosage. Using the information  for the ratio of intensity for   $^{30}\mathrm{Si}$   in silicon substrate:   $^{30}\mathrm{Si}$   in  silicon dioxide  $\sim1{:}16$   and the RSF relationship between silicon  substrate and silicon dioxide standard sample \~ 1:1.2, the mixed  matrix RSF is calculated with the following equation:

$$\begin{array}{r}{\Big(1-\frac{b*1}{b*1+a*16}\Big)*R S F_{S i O x}+\Big(1-\frac{a*16}{b*1+a*16}\Big)*R S F_{S i}}\end{array}$$
(2)

Substituting  $x$   into  ${\mathrm{RSF}}_{S i}$   and   $l.2x$   into  ${\mathrm R S F}_{S i O x}$

$$\begin{array}{r}{{R S F}_{m i x}=\left(\frac{b+19.2a}{b+16a}\right)x}\end{array}$$
(3)

This new RSF for mixed matrix will be used with the existing  RSF value of   $x$   atom/cm 3  for the calculation of the new boron  dosage [atom/cm 2 ] and tabulated in Table 3. The boron dosage  is two and half times more than before numerical correction  dosage value which is in close agreement with the given  process parameter. However, the precise boron dopant profile  obtained is the combination of both boron in silicon dioxide and  silicon substrate. The ion implantation energy is neglected.

Table. 3 Boron dosage value obtained with a comparison between before  numerical correction and after numerical correction for scenario-2.

|11B Implanted|Before numerical correction|After numerical correction|
|---|---|---|
|Dosage obtained [atom/cm2]|z|2.5z|


## IV. C ONCLUSION 

In this paper, we discussed how to obtain the accurate dosage  for the physical segregation structure of mixed matrix  components of a silicon substrate and silicon dioxide. For such  a structure, the commonly used RSF method is not applicable  due to different ion yield enhancement effect of secondary ions  at the oxide and non-oxide regions.

With the proposed numerical calculation, one can obtain  precise boron dosage quantification for the two different  condition scenarios using the re-calculation of the new   $^{30}\mathrm{Si}$  signal intensity as matrix reference isotope and calculation of  mixed matrix RSF.

Through the numerical method for scenario-2, one can obtain  precise dosage quantification but not the real individual profile  with different ion implantation energy on silicon oxide and  silicon substrate.

## A CKNOWLEDGEMENT 

The authors gratefully acknowledged Chengdong XU from  Process   Integration   &   Yield,   GLOBALFOUNDRIES  Singapore Private Limited for the technical discussions.

## R EFERENCES 

[1]    Taxonomy and Definitions for Terms Related to Driving Automation  Systems   for   On-Road   Motor   Vehicles,   SAE   International  (J3016_201806).     [2]    The Automotive Electronics Council, AEC - Q100: Failure Mechanism  Based Stress Test Qualification for Integrated Circuits.     [3]    Surface Analysis – The Principal Techniques, 2nd Edition. Edited by John  C. Vickerman and Ian S. Gilmore . © 2009 John Wiley & Sons, Ltd. ISBN:  978-0-470-01763-0 .    [4]    D. Gui, Z.X. Xing, Y.H. Huang, Z.Q. Mo, Y.N. Hua, S.P. Zhao and L.Z.  Cha, “Long-term Reproducibility of Relative Sensitivity Factors Obtained  with CAMECA Wf”  in Applied Surface Science, 2008, Volume 255, Issue  4 .     [5]    F.A. Stevie, D.P. Griffis, “Quantification in dynamic SIMS: Current  status and future needs”  in Applied Surface Science, 2008, Volume 255,  Issue 4, Pages 1364-1367.     [6]    D. Gui, Y.H. Huang, R. R. Nistala, Z.X. Xing, Z.Q. Mo and Y.N. Hua,  “Numerical Approach to Resolve Mass Interference in Depth Profiling As  in SiGe,”  Surface and Interface Analysis, 01/2011, Volume 43, Issue 12 .    [7]    H.M. Urbassek and W.O. Hofer, “Fundamental Processing Sputtering of  Atoms and Molecules in P. Sigmund (Ed)”, SPUT92, p.97.

