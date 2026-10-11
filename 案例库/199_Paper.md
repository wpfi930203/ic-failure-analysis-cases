---
title: "199_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_39b2d272fb04107a881a07d76762cefd7295230462135641
file_size: 307615
---

## How To Determine Fluorine Contamination Level   On A Normal Al Bondpad?  

Hua Younan   WinTech Nano-Technology Services Pte. Ltd.    10 Science Park Road, #03-26, The Alpha, Singapore Science Park II, Singapore 117684    \* Phone: +65-6-77773-54   Fax: +65-6-77724-62   Email:  Younan@wintech-nano.com

Abstract-   IN our previous paper, we discussed the differences  between EDS and AES and concluded that EDS couldn’t be used  to determine F level on A Normal Al bondpad. In this paper, we  will discuss how we can determine fluorine contamination level on  a normal Al bondpad and propose to use AES/XPS to analyse  fluorine level on a normal Al bondpad in wafer fabrication.

Keywords – Fluorine Contamination and Monitoring, Al  Bondpad,  Auger Electron Spectroscopy.

## I. I NTRODUCTION 

In semiconductor wafer fabrication, fluorine-related gases  (such as   $\mathrm{CF_{4}}$  ,   $\mathrm{SF_{6}}$  , etc.) are used in the etching process of Al  bondpads. Therefore, even after a series of strict cleaning  processes, there will be a certain amount of fluoride  contamination on a normal Al bondpad. The quality of wafers  may not be affected if the amount of fluoride contamination on  the Al bondpad is controlled at a lower value (commonly  referred to as the baseline or background value). However, if  the amount of fluoride contamination exceeds a certain value,  the quality of wafers will be affected, which will lead to the Al  corrosion of Al bondpads and the formation of Al fluoride  defects, and which will then cause the discoloration of Al  bondpads and NSOP problem.

In order to control F level on Al bondpads in wafer fab,  scanning electron microscope (SEM) and energy dispersive  X-ray spectroscopy (EDS), Auger electron spectroscopy (AES)  and X-ray photoelectron spectroscopy  (XPS) analysis   techniques are widely used. In our previous paper titled as “Can  We Use EDS To Determine Fluorine Contamination Level on  A Normal Al Bondpad?” [1], we discussed the differences  between these analysis technologies and analysed the data with  some practical examples. We mentioned that EDS results  couldn’t directly compare with AES or XPS results. This is  because EDS is a bulk analysis and the penetration depth   $(0.3{\cdot}8.5\upmu\mathrm{m})$   of analysis is much deeper than that of AES and  XPS (  $\mathopen{}\mathclose\bgroup\mathopen{}\mathclose\bgroup\mathopen{}\mathclose\bgroup\mathopen{}\mathclose\bgroup\mathopen{}\mathclose\bgroup\mathopen{}\mathclose\bgroup\mathopen{}\mathclose\bgroup\left[10\!\!-\!\!20\upmu\!\!\left[\bgroup\egroup\aftergroup\egroup\aftergroup\egroup\aftergroup\egroup\aftergroup\egroup\aftergroup\egroup\aftergroup\egroup\aftergroup\egroup\aftergroup\egroup\aftergroup\egroup\right]\right]$  ), which are showed in Figure 1.

We suggested that EDS couldn’t be used to determine Fluorine  contamination level on a normal Al bondpad.

In this paper, we will further study and discuss how to  determine fluorine contamination level on a normal Al  bondpad? Following the practical description of "EDS clean is  not clean and Auger clean is clean" ， we will propose to use AES  or XPS to determine fluorine contamination level on a normal  Al bondpad. For sample surface contamination analysis, if no  abnormal element is detected using EDS analysis, we still can’t

immediately conclude that the sample surface is clean. And  then we have to use surface analysis methods such as AES or  XPS to do further analysis. If no abnormal element is detected  using AES or XPS analysis, then we could conclude that the  sample surface is clean. In this paper, we will present details of  AES or XPS to determine fluorine level on a normal Al  bondpad in wafer fabrication. Moreover, we will propose and  discuss a monitoring scheme by using AES (or XPS) analysis  method and instrument parameters, quantitative calculation of  data, also monitoring frequency, selection and preparation of  wafer samples, setting of Control/Spec Limits and OOC/OOS  quality control actions, etc. will be discussed. This will provide  a perfected AES (or XPS) monitoring scheme for eliminating  and overcoming fluorine contamination in the semiconductor  industry and wafer fabrication/packaging test production.

![EDS→BulkAnalysis   AES/XPS→Surface Analysis  (0.3-8.5μm deep)   (10-20A deep)  AES/XPSsurfaceanalysis  EDSanalysisvolume    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c8b2940d-e174-4b4e-80d3-d019bf186457/c8b2940d-e174-4b4e-80d3-d019bf186457.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=5f94290060179135df1b952276c6e006fdc59796)
Fig.1 EDS is a bulk /volume analysis technique and the penetration depth is  much deeper to 0.3-8.5um. But AES is a surface analysis technique and the  penetration depth is only   $10{-}20\mathrm{~\AA~}$  .

## II.   FLUORINE   CORROSION  

In the previous studies, we reported the chemical reaction  mechanism of fluorine contamination and fluorine corrosion on  Al bondpads. The failure mechanism proposed [2,3] is as  follow: Fluorine contamination   [F] corrosion   [OH]  corrosion  $\Rightarrow$   Al bondpad surface serious damage  $\Rightarrow$   Al bondpad  discoloration or NSOP (non-stick on pad).

##  [F] Corrosion:   

Fluorine and Al on the Al bondpads will have a chemical  reaction to formation of Al fluoride:

$$\mathrm{Al+xF^{\cdot}\Rightarrow[A l F_{x}]^{\Gamma(x-3)}=}$$
(1)

In general, x may be 3 or 6, and then

(2)

$$\begin{array}{r l}&{\mathrm{Al+3F^{\cdot}\rightrightarrows[A l F_{3}]}}\\ &{\mathrm{Al+6F^{\cdot}\rightrightarrows[A l F_{6}]^{3-}}}\end{array}$$
(3)

## 【 OH 】 Corrosion:   

Air and moisture/water vapor will enhance corrosion during the  production and wafer storage to cause [OH] corrosion. The OH - ion produced by the chemical reaction will react further with  Al:

$$\begin{array}{c}{{\mathrm{O}_{2}+2\mathrm{H}_{2}\mathrm{O}\rightarrow4\mathrm{OH}^{-}}}\\ {{+\qquad\qquad\qquad\qquad-\mathrm{H}_{2}\mathrm{O}}}\\ {{\mathrm{Al}\rightarrow\,\mathrm{Al}(\mathrm{OH})_{3}\,\rightarrow\mathrm{Al}_{2}\mathrm{O}_{3}}}\end{array}$$
Therefore, to eliminate and overcome the fluorine corrosion on  Al bondpads, it is necessary to reduce fluoride contamination  level and avoid contact with air and moisture/water in the  processes and wafer storage. Moreover, wafer vacuum  packaging and nitrogen   $\left(\mathbf{N}_{2}\right)$  ) environment for wafer storage are  used in wafer fab and assembly house to prevent [OH]  corrosion. Besides these, a fluorine contamination monitoring  scheme should be set up and AES (or XPS) is recommended to  monitor the fluorine contamination level on a normal Al  bondpad in wafer fab.

## III.   AES   ( OR  XPS)   ANALYSIS  

## AES  

Auger electron spectroscopy (AES) is a surface analysis  technique. The e-beam/sample interaction area is same as the  spot size and the penetration depth of AES is only 10-20 Å.   AES is sensitivity to low atom Z elements (such as C, O, F etc.).  Its detection limit is similar to EDS’s about   $0.1{\cdot}1.0\ \mathrm{at\%}$   level.   In this study  ， PHI710 field emission Auger electron  spectrometer from PHI Company is used. The instrument is  equipped with ion gun and can be used for longitudinal  sputtering analysis of the sample. The acceleration voltage and  beam distribution are 10kV and 10nA. In order to obtain a good  Auger signal, the inclination angle of the sample is   $30^{\mathrm{o}}$  . The ion  gun voltage is  $2\;\mathrm{kV}$   and the beam density is  $3\;\mathrm{mA}\,/\mathrm{cm}^{2}$  . The gas  used is argon (Ar purity   $99.9\%$  ).

The basis of AES quantitative analysis is derived from the  relative intensity of Auger differential spectrum peak and the  sensitivity factor of analytical elements, that is, the main Auger  transition peak of each element is the signal intensity, divided  by the relative sensitivity factor of each element. The relative  contents of each element on the surface of the sample can be  obtained by normalization treatment. The expressions are as  follows:

$$\mathrm{C_{i}}{=}(\mathrm{I_{i}}/\mathrm{S_{i}})/\mathrm{{\sum}^{n}}_{(\mathrm{i=1})}\mathrm{I_{i}}/\mathrm{S_{i}}$$
The   $\mathrm{I_{i}}$  - element I is peak-peak in the spectrum; The atomic  sensitivity factor and   $\mathrm{C_{i}}$   - unit of   $\mathrm{S_{i}}$  - element I are relative  atomic percent content. The AES data processing software  MultiPak, which is equipped with PHI710 instrument, can  qualitatively and quantitatively analyse the analysed spectral  lines. The relative atomic percentage and weight percentage of  each element can be obtained.

## XPS  

In this study, we also applied the XPS technology to analyse the  fluorine contamination on Al bondpad of wafers. The model  used for XPS analysis is Scanning XPS Microscope PHI  Quanta II, which is using Aluminium source at 1486.6 eV.

## IV. MONITORING SCHEME  

## Control Limit (CL)/Spec Limit  

Control Limit (CL) is related to wafer manufacturing process. If  the optimized wafer back-end process (including etching, PRS,  cleaning processes, etc.) is used, the level of fluoride  contamination on the Al bondpads should be limited to a lower  level. However, if the back-end process of the wafer is not  optimized, the level of fluoride contamination on the Al  bondpads might be higher. We use Auger analysis to analyse  and study fluorine contamination level on a normal Al bondpad.

A large number of samples were analysed, and then the control  limits were calculated based on 3 Sigma calculation methods.

The control limits of fluorine contamination on Al bondpads:   (a) Control Limit:   $3.0{-}5.0\;\mathrm{at}\%$   (as received) and   (b) Control Limit:  $0.0\;\mathrm{at}\%$   (after 5nm sputtering).

The Spec Limits of fluorine contamination on Al bondpads:  (a) Spec Limit:  $6.0\;\mathrm{at}\%$   (as received) and   (b) Spec Limit:   $0.0\;\mathrm{at}\%$   (after 5nm sputtering).

Only when both results from "As received" and "After 5nm  sputtering" are within the control limits, the Al bondpad is  qualified and passed the monitoring. Conversely, if the result  from the "As received” are within the control limit, but the  result from the "After 5nm sputtering" run Out Of Control  (OOC), the Al bondpad is still not qualified and considered as  "failed" the monitoring.

The Specification (Spec) Limits does not depend on wafer  manufacturing process, but only depends on the quality impact  of Al bondpads. In the previous studies [4], a series of  experimental studies have been carried out, and it is determined  that the industrial Spec Limits of fluoride contamination on Al  bondpads are   $6.0\;\mathrm{at}\%$   ("As received") and   $0.0\;\mathrm{at}\%$   ("After 5nm  sputtering").

## Monitoring Frequency and Sample Source   

Monitoring frequency is critical because Auger monitoring  requires additional costs depending on the performance of  Auger machines. If the Auger machine can analyse the  complete wafer without cutting, and the wafer is still available

to use, then the monitoring frequency can be increased.  However, if the Auger machine cannot analyse a whole wafer  and then the wafer has to be cut into the small sample and the  monitoring frequency should be reduced.

A typical frequency of Auger monitoring is recommended once  a week. The monitoring sample source may be from: (a). If the  Auger machine is able to analyse of the whole wafer, the  samples can come from both good production wafer (because it  can still be used after analysis) and scrapped wafer; (b). If the  Auger machine is unable to analyse of the whole wafer, then the  scrapped wafer (due to other failures) should be used, such as  the selection of those wafers that fail due to electrical  measurements but whose Al bondpads have to be as normal.

## Wafer Lifetime  

The shelf life of wafers is also critical. From the theoretical  discussion above, we know that   $\mathrm{O}_{2}$   and   $\mathrm{H}_{2}\mathrm{O}$   could enhance the  corrosion of fluorine and lead to the formation of corrosion  defects in Al bondpads during the wafer storage process.  Therefore, for Auger monitoring, the wafer samples should not  only be representative, but also should be fresh wafers. It is  suggested that the lifetime of wafers should be less than one  week.

## Analysis Points  

Auger monitoring analysis points and methods set up in the  analysis scheme proposed: (a). In general, 6" wafer needs 2-  point Auger analysis (centre and edge); (b). 8" wafer needs 3-  point Auger analysis (centre, middle and edge); (c). 12" wafer  need 5-point Auger analysis (centre, 4 edges).

## Elements Monitored and Methods  

Analysis methods suggested are: (a). To monitor the surface  contamination on Al bondpads, the elements of C, N, O, F, Al,  Si, Ti are analysed. Two steps of the "As received" and "After  5nm sputtering" need to be analysed. (b). If the surface  contamination on the Al bondpads and the thickness of the Al  oxide layer are monitored at the same time, then we suggest to  carry out step analysis by 5nm till the pure Al. For most cases, it  may reach to the pure Al after sputtering to   $15\mathrm{nm}{-20}\mathrm{nm}$  .

## OOC/OOS Procedure  

During AES (or XPS) monitoring, it is suggested that the  monitoring elements should include elements of C, N, O, F, Al,  Si and Ti. The analysis results must be within the Control/Spec  Limits, including both "As received" and "After 5nm  sputtering", and then the wafer product monitored is qualified.  If analysis results are out of the Control Limit (OOC) and the  Spec Limit (OOS), we have to take actions as the wafer product  is not qualified. The production and engineering team at the  wafer fab should be alerted immediately.

The quality team should do OOC actions/procedures: (a).  Check or verify the analysis results of AES (or XPS) analysis. If  possible, it is best to redo the AES (or XPS) analysis to confirm  the OOC. (b). Check the history of wafer monitored. Is wafer  monitored correct? Is the wafer lifetime within a week? If

possible, another wafer should be retested to confirm OOC. (c).  If OOC is confirmed after the taking actions, the production and  engineering teams should take immediate actions to investigate  and find out the root causes of OOC. (d). The production and  engineering teams should also take corrective/preventive  actions to eliminate fluoride contamination, including  improvements of production processes. (e). After the process  are improved, if the new process is implemented, a new wafer  sample must be sent for AES (or XPS) analysis to confirm that  the level of fluorine contamination is within the control limit.  (f). If the analysis results exceed the industrial Spec Limit (F 6.   $0\ \ \mathrm{at}\%$  ), the wafer production line should be shut down  immediately. (g). The impact wafers should be reworked. (h).  The wafer production line can be restored only when the  fluorine contamination level is reduced to within the control  limit.

## Vt Shift Concern  

The results show that AES analysis can affect the threshold  voltage performance of semiconductor devices. The Bondpad  connected to the transistor gate was exposed for an average of  2.5 minutes at different beam energies (0, 3, 5, 10, 15 and 20  keV). Vt measurements were collected once before exposure  and three times after exposure. The results showed that, in AES  analysis, the transistor Vt was impacted and moved by electron  beams at different energy levels (0, 3, 5, 10, 15 and   $20~\mathrm{keV}$  ).   Therefore, it is not recommended to carry out AES monitoring  analysis on production wafers to be shipped to customers. It is  best to use wafers rather than intended shipments for AES  monitoring. Another way, if necessary, AES analysis is  recommended to do on incomplete edge die of the wafer to  prevent the Vt migration from being exposed to electron beam  during AES analysis.

## V. APPLICATIONS   

## Case-Study-1: Process Improvement  

In this application case, AES monitoring was using for process  improvement. In Figure 2, AES monitoring results showed that  F level on Al bondpads. From the data, we could know that for  the old process, F level on Al bondpads were scattered about   $1.0{-}5.50\;\mathrm{at}^{0}\%$   and some points were OOC.

![Surface F at.%  8Q  Oldprocess   Newprocess  CL5.0at.%  %  40  20  ③④  ew-   dt-c   AeW-   inr-9   6nv-g   100-9   AON-S  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/37858c9e-9ebd-414d-98c6-26cbef2a748f/37858c9e-9ebd-414d-98c6-26cbef2a748f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=002d9307254bf4f492075dd8422dc656d8f6c346)
Figure 2. AES monitoring results showed that for the old process, F level on Al  bondpads were scattered about  $1.0{-}5.0\;\mathrm{at}\%$   and some points were OOC.  However, after process improvement, the F level had been reduced for new  process comparing to the old process and all points were within CL.

As such, the process has to be improved so as to reduce F level  on Al bondpads.

After process improvement, the F level had been reduced for  new process comparing to the old process and all points were  within the control limit.

## VI. C ONCLUSION 

In this paper, we propose a complete AES (or XPS) monitoring  system for Al bondpads for semiconductor wafer fab, including  AES (or XPS) analysis methods and instrument parameters,  quantitative calculation of data, monitoring frequency,  selection and preparation of wafer samples. control/spec limits  settings and OOC quality control procedures and so on. It  provides a useful monitoring scheme for eliminating and  overcoming fluorine contamination in semiconductor industry  during wafer fabrication/packaging test production. In this  paper, we also reported a case-study for wafer fab process  improvement.

## A CKNOWLEDGMENT 

The author would like to thank Surface FA Division,  Wintech-Nano for their support of this technical paper.

## R EFERENCES 

[1]    Hua Younan,  Can We Use EDX To Determine Fluorine Contamination  Level on A Normal Al Bondpad?  The Proceedings of the   $25^{\mathrm{th}}$  International Physics and Failure Analysis (IPFA2018), July 2018,  Singapore (2018).    [2]    Hua Younan et. al., A Study on Non-Stick Aluminium Bondpads due to  Fluorine Contamination using SEM, EDX, TEM, IC, Auger, XPS &  TOF-SIMS Techniques. The proceedings from the 28 th  International  Symposium for Testing & Failure Analysis (ISTFA'2002), 3-7 Nov,  Phoenix Civic Plaza, Phoenix, Arizona, USA p495-504 (2002).    [3]    Hua Younan et. al., A Study on Fluorine-Induced Corrosion on Microchip  Aluminium Bondpads. The proceedings from the   $29^{\mathrm{th}}$   International  Symposium for Testing & Failure Analysis (ISTFA'2003), 2-6 Nov. 2003,  Santa Clara, California, USA, p249-255 (2003).    [4]    Hua   Younan,   Nistala   Ramesh   Rao,   Simulation   Studies   of  Fluorine-induced Corrosion and Defects on Microchip Al Bondpads In  Wafer Fabrication. The Proceedings of the  $36^{\mathrm{th}}$   International Symposium  for Testing and Failure Analysis (ISTFA 2010), Nov 14-18, in Dallas,  Texas, USA (2010).

