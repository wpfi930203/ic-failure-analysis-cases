---
title: "208_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_bd5ae7871b233f5f94b2572d3b0991487295230462135641
file_size: 1562677
---

## 3D System-in-package Failure Analysis by Highresolution Time-domain Reflectometry  

Yang Shang 1 , Makoto Shinohara 2 , Masaichi Hashimoto 2 , Thiam Kim Chuah 3 , Mei-Fern Lim 4 , Meng-Chi Pun 4 , King-Long Teoh 4  1 ADVANTEST (Singapore) Pte. Ltd, 10 Ang Mo Kio Street 65, #04-11 Techpoint, Singapore  2 ADVANTEST Corporation, 1-5 Shintone, Kazo, Saitama, 349-1158, Japan  3 ADVANTEST Sales and Support Sdn. Bhd.   L2-5A, Penang SME Centre, Hilir Sungai Kluang 5,11900 Bayan Lepas, Penang, Malaysia  4 Avago Technologies Malaysia Sdn Bhd (Broadcom), Free Industrial Zone,11900 Bayan Lepas, Penang, Malaysia  Phone : (65) 63473873, Email :  Yang.Shang@advantest.com

Abstract — The rise of 3D high-bandwidth-memory (HBM)  technology has boosted System-in-Package (SiP) storage density  and energy efficiency. However, this advancement poses  significant challenges in pinpointing defects within HBMs  during package-level failure analysis. Although electro-optic  sampling-based time-domain reflectometry (EOS-TDR) offers  high resolution for defect isolation in packages, its effectiveness  diminishes within HBMs due to reduced signal amplitude and  manufacturing tolerances. To enhance EOS-TDR's efficiency in  analyzing HBM failures, this study explores two waveform  analysis techniques: normalization and near-die correction.  Normalization extracts abnormal reflections caused by defects  within the die, while near-die correction refines normalization  results by minimizing sample-to-sample variations within the  chip package. Results demonstrate that employing both  normalization and near-die correction techniques effectively  identifies open defects within HBMs.

Keywords— HBM, non-invasive, failure analysis, EOS-TDR

## I.    INTRODUCTION  

Driven by the advancements in high-performance  computing (HPC) and artificial intelligence (AI), high  bandwidth memory (HBM) has emerged as the most  promising DRAM solution, offering a combination of high  data rates and low power consumption. Fig. 1 shows a systemin-package integrated with HBM. Leveraging advanced  packaging technologies, 3D-stacked HBM layers are directly  connected with the logic SOC through Through-Silicon Vias  (TSV) and µbumps and the interposer, bypassing any ESD  protection pads. This arrangement allows a significantly larger  number of memory chips to be accessed simultaneously over  a very short distance, resulting in a substantial reduction in  both data transfer latency and power consumption per bit.

The 3D-stacked architecture of HBM presents a  significant increase in I/O density and a notable reduction in  feature size. This poses a considerable challenge in packagelevel failure analysis. To address this challenge, employing a  high-resolution electro-optic sampling-based time domain  reflectometry (EOS-TDR) system has become crucial in  pinpointing defect locations [1-7] before undertaking  subsequent analyses such as X-ray, C-SAM, SEM. Fig. 2  illustrates the operational schematic of an EOS-TDR  (ADVANTEST TS9001). Unlike conventional TDR systems  where time resolution is confined by the sampling frequency,  EOS-TDR detects the reflected signal by shifting the delay  between two optical pulses. This approach significantly  enhances time resolution. When translated into distance  resolution, EOS-TDR offers a distance resolution that  surpasses traditional oscilloscope-based TDR by 20 to 30  times.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/277fdbdc-969c-4303-a45a-7d8c950af6cd/277fdbdc-969c-4303-a45a-7d8c950af6cd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=8fef7e59d06bbb470e39ad4efea867b4454bc6d5)
Fig. 1. A System-in-package (SiP) with HBM [1]

![Opticalpulse  AD   Amplitude  Femtosecond  Distance to Pad  fiber Laser  Electricalpulse  (Laser1)  Tinme  Frequency   Delay  Photodiode   PCS   Probe   DeviceUnderTest  Reference   Shifter  PLL.   Femtosecond  fiberLaser   Optical pulse  (Laser2)  f=f-△f  Oscilloscopebased Conventional TDR   ADVANTESTTS9001TDR  Distance Resolution   \~100μm   <5μm  Signal waveform   StepWave   PulseWave  Rise time   >13ps   < 10 ps (TYP)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/232df806-b46b-4ca2-982a-a3acc12b20ce/232df806-b46b-4ca2-982a-a3acc12b20ce.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=1796ee71464cc655c6b3921f30d82713139dc6ad)
Fig. 2. Functional diagram of a high-resolution TDR system

The detectability of defects using EOS-TDR is determined  by analysing the ratio between the reflected signal's amplitude  and the variation observed from sample to sample. In  traditional packaging, the connections that are prone to defects  can be readily identified through EOS-TDR. These  interconnections, situated outside the die, allow the  transmitted electrical pulse by TDR to pass through them  without experiencing significant attenuation. However, in  comparison to conventional packaging methods like flip-chip  or wire-bonded chips, the reflected signal's amplitude from  HBMs (High Bandwidth Memory) is notably smaller. This is  due to the ESD protection circuitry beneath each pad, which  typically possesses a decoupling capacitance of 0.5 to 1 pF,  significantly reducing the amplitudes of both the incoming  and reflected pulses [8, 9]. Therefore, more advanced  analysing techniques must be deployed to improve defect  detectability.

In this work, the EOS-TDR analysis to the open defects  inside the HBMs has been explored using two techniques:  defect dependent reflection (DDR) extraction [5] through  normalization and reduction of sample-to-sample variation by  near-die correction. Ideally, the TDR waveform of a DUT

![BMlayers  TDRRFProbe  Die  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a860ff53-e229-48b0-a42e-5e62e67ecdd8/a860ff53-e229-48b0-a42e-5e62e67ecdd8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=65e9c8131575527545771f6b68ae059ffe623f7d)
Fig. 3. Chip circuit diagram with HBMs

with defects inside HBMs can be normalized by a Good unit  one to extract the DDR. However, because of tolerance in the  chip package manufacturing, the extracted waveform includes  not only DDR, but also slight reflection deviations caused by  package differences among the same type of chips. These  deviations become non-negligible to the analysis of defects  within HBMs.

## II.   HBM S  A NALYSIS BY  N ORMALIZATION 

Fig. 3 shows a simplified circuit diagram of a signal trace  connecting through all HBMs. To simplify analysis, it is  assumed that each HBM layer is modeled by the transmission  line with same length (L) of  $200\,\upmu\mathrm{m}$   and effective permittivity  of 50. The circuit has been simulated using method proposed  in [5].

Fig.4a shows the simulated TDR waveforms of one Good  sample and four defective samples with opening at various  location. If the opening is outside the die like Open@Bump,  the defect location is clearly indicated by the positive peak at  160 ps in the TDR waveform. But if the opening is inside the  die like opening at locations  $\textcircled{2}$  ,  $\widehat{\left.\left(4\right)\right.}$   and   $\textcircled{6}$  , the positive peaks  are hardly identified in the waveforms because of the large  negative peaks at around 159.7ps induced by the ESD  capacitance. The magnitude of both incident and reflected  pulses will be largely attenuated when bypassing this ESD  capacitance. Knowing that the reflections generated by ESD  capacitance is not defect dependent, it can be normalized by  the waveform of a Good sample.

Fig. 4b shows the waveforms of in-die opening after  normalized by the Good sample. Three positive peaks are  clearly identified at 194.2 ps, 221.9 ps and 243.4 ps for  openings at locations   $\textcircled{2}$  ,   $\widehat{\left.\left(4\right)\right.}$   and   $\textcircled{6}$   respectively. The  normalized waveform consists of not only the first reflection  caused by the defect, but also the sequent multiple reflections  generated between the ESD pad and defect point. Take  Open  $@({\widehat{\boldsymbol{2}}})$   for example, the 2nd peak is at 227 ps, which is  32.8-ps away from the 1st peak. And subsequent peaks occur  around every 32.8 ps. Similarly, the peaks intervals for  Open@ ④  and Open  $@({\overline{{6}}})$   are 64.2 ps and 98.4 ps, respectively.  This peak-to-peak internal is proportional to the trace length  between the ESD pad and defect point. However, if the defect  point is too close to the ESD pad, the reflection peak caused  by the open defect may become non-detectable due to the  overlapping of multiple peaks.

Fig. 5a shows the simulated TDR waveforms of the same  set of samples after reducing the length of transmission line in

![0.8  Open@②  200   300   100   5-00  Time(ps)  a  (a) 0.2  Normalized Open@④  0.15  07  0.05  10O   200   300   400   50  Time (ps)  Cb  (b)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8f7b08e2-5532-4620-816b-dfb95c07f511/8f7b08e2-5532-4620-816b-dfb95c07f511.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=aec4c696b8a1ed90d510a7a055646e8aa048e8fb)
Fig. 4. Simulated TDR waveform of samples with openings inside HBM   $(\mathrm{L}\!=\!200\mathrm{um})$  : (a) TDR waveforms; (b) normalized waveforms.

![0.8  Good  oper  0.6  0.4  Q2  -0.4  10O   200   300   400   5-0-0  Time (ps)  a  (a)  02  n@BUMP（Scs  1Open@④  0.15  200   300   SOO  Time(ps)  (b)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/684e9031-de02-474b-b489-4eaac785c26e/684e9031-de02-474b-b489-4eaac785c26e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=78cfc7d0050581abd8189d4184cd2dabb1c03258)
Fig. 5. Simulated TDR waveform of samples with openings inside HBM   $(\mathrm{L}\mathrm{=}\,50\mathrm{um})$  : (a) TDR waveforms; (b) normalized waveforms.

![0.14  0.12  0.1  Open@BUMP(Scale:0.1)  0.08   Normalized Open@②  Normalized Open@④  Normalized Open@i6  0.06  0.04  0.02  140   150   160   170   180   190   200   210   220  Time(ps)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/09217304-c8bd-49d1-95db-836299b6610e/09217304-c8bd-49d1-95db-836299b6610e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=a67079d1fbf795f5d7817416dd6d6b221d1ecd83)
Fig. 6. A enlarged view of normalized TDR waveform of samples with  openings inside HBM   $(\mathrm{L}\mathrm{=}\,50\mathrm{um})$  .

each HBM layer to 50um. The waveform, such as  Open@Bump, remains the same if the open point is outside  the die. The waveforms generated by the in-die opens at   $\textcircled{2}$  ,   $\widehat{\left.\left(4\right)\right.}$   and   $\textcircled{6}$  , requires normalization analysis to eliminate the  impact of ESD-pad. Fig. 5b shows the normalized TDR  waveforms of these samples. We can observe the peak of  Open  $@({\widehat{\boldsymbol{2}}})$    is no longer representing the actual open location as  its peak time falls between   $\widehat{\mathcal{A}})$   and   $\textcircled{6}$  . In this case, the defect  location should be identified from the rising edge of the  normalized waveform, where the influence from 2nd and  subsequent peaks are minimized.  Fig. 6 shows an enlarged  view of the waveform between 140ps and 220ps. We can see  the time of the initial rising edges at 0.04V are still  proportional to the trace length between the ESD pad and  defect point.

## III.   N EAR -D IE  C ORRECTION  

If considering sample-to-sample variation between solder  ball and µbump (P1-P2 as shown in Fig. 3), normalization  method cannot be directly used to find the defects inside the  HBMs, the reflection deviation among different samples could  be higher than the signal reflected from the defect point. This  work proposed a near-die correction method to minimize the  impact of sample-to-sample variation to the inner die  reflections. Assuming the defect location is inside the die, the  reflections caused by known good region (KGR) outside the  die becomes a good reference to correct the path loss and time  delay between P1 and P2. The accuracy of in-die defect  analysis will be largely improved by the corrected waveforms.

Assuming reflection time of die interface is   $t_{d}$  ,   the  interested waveforms of DUT and Good sample becomes    $F_{t,\ t\geq t_{d}}$      and   $G_{t,\ t\geq t_{d}}$  , respectively. The KGR is defined as   $\left[\,t_{1},t_{2}\,\right]$   that   $t_{2}<t_{d}$  . To avoid the influence of probing  variations,   $t_{1}$   can be after the probing reflection   $\left(t_{1}>0\right)$    where   $g(t_{1})$   is approaching zero;  $t_{2}$   must be ahead of   $t_{d}$   to  avoid the influence of unknown inner die defects. We can  have:

$$t_{2}=t_{d}-\frac{\mathrm{t_{r}}}{2}$$
(1)

where  $\mathtt{t}_{\mathrm{r}}$   is the rise time of the pulse that injected into the die.  Assuming the ESD capacitance at the Die interface is large  enough,  $\mathtt{t}_{\mathrm{r}}$   can be approximated by the falling time of the  TDR reflection cause by this capacitance.

The corrected TDR waveform of DUT can be represented as

![HBM6 HBM4 ubump Interposer F一一一一一  C Substrate ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5ff88d83-fc4c-4d8e-b562-8c536f443d5c/5ff88d83-fc4c-4d8e-b562-8c536f443d5c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=01c83a5de90e784b6362bfda6be5ed867d0c1d38)
Fig. 7. Structure diagram of SiP with 3D stacked 8-layer HBMs

![0.5 —Good 0.4 KGR  -C4 ubump 0.3  HBM4 HBM6 0.2  HBM4（fit) --HBM6（fit) -0.2 -0.3 -0.4 -0.5 -50  C  50  100  150  200  250 Time(ps) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b5ea5a17-358b-4487-a86f-39a067ca5a6e/b5ea5a17-358b-4487-a86f-39a067ca5a6e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=f19f70f5406011f81026f33a73f3ab02e73ca074)
Fig. 8. Measurement results of SiP chip samples and the corrected results of  HBM4 and HBM6. (KGR: 50\~126 ps)

$$F^{\prime}{}_{t,\ t\geq t_{1}}=\ \delta F_{t+\tau,\ t\geq t_{1}}+\ \mu$$
(2)

where  $\delta$   is the amplitude correction;  $\tau$   is the delay correction;   $\mu$   is the dc offset correction. A least square curve fitting  method can be used to obtain the correction factors that meet  the objective function:

$$m i n\sum_{\mathrm{~x~}}^{t_{2}}[F_{\;i}^{\prime}-G_{i}]^{2}$$
(3)

where   $x=[\delta,\tau,\mu]$   . The resulting correction factor   $x_{0}=$   $[\delta_{0},\tau_{0},\mu_{0}]$    will generate a corrected DUT waveform   ${F^{\prime}}_{t,\textit{t}\geq t_{1}}(x_{0})$  . The corrected DUT waveform needs to be  normalized by   $G_{t,\ t\geq t_{d}}$   to eliminate the unwanted reflections  by die pad capacitance.

$$N_{t,\ t\geq t_{1}}\ \ =\ F^{\prime}{}_{t,\ t\geq t_{1}}(x_{0})-G_{t,\ t\geq t_{1}}$$
(4)

The defects inside HBMs will be revealed in  $N_{t,\ t\geq t_{d}}$

## IV.   E XPERIMENTS   

The proposed method is further verified with experiments  on a SiP chip with 3D HBMs. Fig. 7 shows the cross-section  view of the SiP chip. Five samples are measured, including  one good sample and four reference samples opening at C4,  µbump, HBM4 and HBM6, respectively. Advantest TS9001  TDR system was used for measurements. A RF probed with   $600{\mathrm{-}}\upmu\mathrm{m}$   pitch is used to probe at the BGA balls on the back  side the chip. The traces of the probed signal pins are wired  through all HBM layers.

Fig. 8 shows the measurement results of SiP chip all  samples. Since the openings of C4 and µbump are outside the

die, their measurement waveforms show clear positive peaks  at 142.9 ps and 156.2 ps, respectively. In contrast, the  openings of HBM4 and HBM6 are inside the die, we could  hardly observe a significant waveform difference from the  original waveforms as compared with Good. Their near-die  corrected waveforms are also shown in Fig. 8 as HBM4(fit)  and HBM6(fit). The KGR is selected as 50\~126 ps, within  which the waveforms of HBM4 and HBM6 are maximumly  fit to the Good one by scaling in the amplitude and shifting in  time delay.

Fig.9a shows the normalized results of HBM4 and HBM6  without any correction. The first peaks of “Norm HBM4” and  “Norm HBM6” are 159.7 ps and 154.4 ps, respectively. The  154.4 ps of HBM6 is clearly incorrectly as it is early than that  of µbump. Fig.9b shows the normalized results of HBM4 and  HBM6 after near-die correction. The first peaks of “Norm  HBM4(fit)” and “Norm HBM6(fit)” become 160ps and  170.1ps, respectively. The robustness of near-die correction  method is also confirmed. Fig. 10a and 10b shows the  normalized measurement results of HBM4 and HBM6 after  near-die correction when KGR is 75\~126 ps and 100\~126ps  respectively.

## V.   C ONCLUSION 

This study delved into utilizing EOS-TDR for the failure  analysis of 3D SiP featuring HBMs. This involved employing  normalization   and   near-die   correction   techniques.  Normalization aids in isolating abnormal reflections  stemming from defects within the die, while near-die  correction   contributes   to   refining   the   accuracy   of  normalization outcomes by reducing sample-to-sample  variations within the chip package. The measurements  revealed that employing both normalization and near-die  correction techniques distinctly identified open defects within  HBMs.

## R EFERENCES 

[1]    M. Hashimoto, et. al. “Failure analysis of LSI interconnection by  terahertz time-domain reflectometry”, IEEE International Symposium  on the Physical and Failure Analysis of Integrated Circuits (IPFA),  2016.    [2]    M. Hashimoto, M. Shinohara, Y. Shang, A. Mohan, B. Zee, “2.5D Chip  TSV Open Failure Analysis by High Resolution Time-domain  Reflectometry”, IEEE Electronics Packaging Technology Conference  (EPTC), 2017    [3]    Y. Shang, M. Shinohara, R. B. Radhamony, J. Kiljan, A. Wu, “Highresolution Time-domain Reflectometry Analysis in Back-end-of-line  (BEOL) by Recursive Circuit Modelling”, IEEE Electronics Packaging  Technology Conference (EPTC), 2018    [4]    Y. Shang, M. Shinohara, W. Qiu and B. Zee, "2.5D Package Modelling  for Short Circuit Failure Analysis by High-Resolution Time-domain  Reflectometry," IEEE International Symposium on the Physical and  Failure Analysis of Integrated Circuits (IPFA), 2018.    [5]    Y. Shang, M. Shinohara, E. Kato and M. Hashimoto, "Defect  Identification in Branched Traces by High-resolution Time-domain  Reflectometry," IEEE International Symposium on the Physical and  Failure Analysis of Integrated Circuits (IPFA), 2022.    [6]    L. Saku, R. B. Radhamony, A. Soriano, G. Tan and Y. Shang, "TimeDomain Refl  ectometry Analysis on Low Impedance Marginal Failure  and multi-chip Modules," Electronics Packaging Technology  Conference (EPTC), 2022    [7]    Y. Shang, M. Shinohara, M. Hashimoto, C.-Y. Lee, M. Xue " A  Preliminary Study on the Soft Defects Modeling and Measurement  Method Using Time domain Reflectometry," IEEE International  Symposium on the Physical and Failure Analysis of Integrated Circuits  (IPFA), 2023.    [8]    N. Khurana, T. Maloney and W. Yeh, "ESD on CHMOS Devices -  Equivalent Circuits, Physical Models and Failure Mechanisms," 23rd  International Reliability Physics Symposium (IRPS), 1985.    [9]    M. I. Natarajan et al., "RFCMOS ESD protection and reliability,"  International Symposium on the Physical and Failure Analysis of  Integrated Circuits (IPFA), 2005.

![0.06  0.06 C4 (scale: 0.1)  C4 (scale: 0.1) μbump (scale: 0.1)  μbump(scale:0.1) 0.05  0.05 Norm HB M4  Norm HB M4(fit) Norm HBM6  Norm HBM6(fit) 0.04  0.04 （） 0_01  0_01 -0_01  -0_01 10-0  1.50  200  250  100  150  200  250 Time (ps)  Time (ps)             (a)                                                       (b) （a)  CD ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9fa4f752-5459-4d00-885d-ae37639b4c10/9fa4f752-5459-4d00-885d-ae37639b4c10.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=84947b4313159aca6c3eaedb6de94587b07b2913)
Fig. 9. Normalized measurement results of of HBM4 and HBM6: (a) before  correction, (b) after near-die correction. (KGR: 50\~126 ps)

![0.06   0.06  C4 (scale: 0.1)   C4 (scale:0.1)  μbump(scale:0.1)   —μbump(scale:0.1)  0.05   0.05  Norm HBM4(fit)   —Norm HBM4(fit)  Norm HBM6(fit)   —Norm HBM6(fit)  0_04   0.04  00   00  0_01   0_01  -0_01   -0_01  10-O   1.50   200   250   10-O   150   200   250  Time (ps)   Time (ps)              (a)                                                       (b)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/98bfff12-6cd1-433d-b780-d5bcbd6a4af7/98bfff12-6cd1-433d-b780-d5bcbd6a4af7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215890%3B1743219490&q-key-time=1743215890%3B1743219490&q-header-list=host&q-url-param-list=&q-signature=243699d8c61cf4317fab02bf12b97d7d2d21f0e1)
Fig. 10. Normalized measurement results of of HBM4 and HBM6 after  near-die correction: (a) KGR is 75\~126 ps, (b) KGR is 100\~126 ps

