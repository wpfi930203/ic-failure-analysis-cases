---
title: "ISTFA-2015_compressed.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_6fb1bbc746a97c1328f8526b460062427295230462135641
file_size: 45536292
---

Proposed Methodology


Current Situation


SDL and LADA are commonly employed to reveal circuit  speed paths or device limiters that respond to laser stimulation  and result in a change of pass-fail test status. SDL uses a cw  1340nm thermal laser while LADA uses a cw 1064nm  photocurrent inducing laser (with slight thermal effect) to  temporarily alter transistor characteristics in the active region. The position of the scanning laser is correlated to the change  in electrical characteristics of the device for signal image  acquisition. Based on current applications of both techniques, there is one limitation and that is the constraint to debug on  soft failures.


Pulsed LADA


Although pulsed lasers are also commonly used in timeresolved LADA, delay variation mapping and other similar  derivatives [12-17], the application in their respective context  centers around soft failures and should not be confused with  the purpose in this work which will be discussed in this subsection. Figure 1 presents LADA signals obtained from a  random active logic region on a good device which is  exercised by a 100 MHz scan test pattern. Comparing the  signals induced by cw and pulsed laser at 10 kHz, 50 s pulse  width as shown in Fig. 1(a) and 1(b) respectively, enhancements in terms of the number of stimulated sites by  LADA in the latter is obvious. The cw average laser power is


approximately 600 mW and the pulsed peak power is in the  same range.  The peak power is calculated using equation 1.


cycle


Duty


/


)


(


,


(Js P


power,


1


-1








Js


P


power


Average


Peak


(1) It should be noted that the average power is measured using a  power meter from output fiber for relative reference and not  meant to indicate the exact power interacting with the device. The LADA signals are acquired using a refractive solid  immersion lens which presents an optical resolution of around  240 nm and the device under test is processed on 28 nm  technology.


The findings from this experiment demonstrate that a pulse  width in the range of tens of s and slow pulse frequency of  few kHz is sufficient to reduce the effect of high induced  substrate current that affects the ability to stimulate more sites  in the active circuitry. This enhancement from pulsed laser is  expected to become more critical at more advanced  technology nodes as the laser spot size does not shrink as fast  as the device.  To prove the limitation of cw laser, the laser  power is increased to the point of permanent device damage. No additional signal to Fig. 1(a) is observed. A further  experiment is conducted using a femtosecond pulsed laser  with picosecond (ps) pulse width and the results as shown in  Fig. 1(c). It is apparent that the signals are significantly  stronger likely due to possibly 2pLADA effects [12]. An  interesting point to highlight is the similarity in the locations  of stimulated sites between the s and ps pulsed laser. It  suggests that s pulsing could be sufficient, at least for the  next few technology nodes. However, further zoom-in analysis  is beyond the scope of this work and is not conducted to  validate this claim further.


In a further experiment, the pulsed laser beam is fixed at  location X (see FIG 1(b)) and the minimum average power  required to observe the LADA signal at various duty cycle is  recorded. The graph as shown in Fig 2 summarizes the result. As duty cycle reduces from a smaller pulse width with respect  to the period, the minimum average power required also  reduces but peak power remains approximately constant. This  proves that peak power determines whether the threshold for  the soft error upset is achieved, not the average power and this  result also demonstrates the advantage of pulsed laser beam in  reducing thermal build up from high incidence power which  can subsequently damage ‘healthy transistors’ permanently.


(a)


(b)


(c)


Figure 1: (a) cw-LADA, pulsed-LADA at (b) 10 kHz, 50 s


pulse width and (c) femtosecond frequency, ps pulse width


based on 1064 nm laser stimulation on a logic active region.


Figure 2: Minimum average and peak power required to


induce a state change on test at X (see Fig. 1(b)) under


conditions of varying duty cycle using 10 kHz pulsed 1064 nm  wavelength laser (537mW output power from fiber).


EeLADA Concept


We proposed a new fault localization method called EeLADA  that extends pulsed-LADA to debug device hard failures. Figure 3 depicts the block diagram of the concept. A tester is  docked to a scanning optical microscopy (SOM) system  similar to a custom LADA setup. Prior to fault localization on  a logic hard failure, the fail log (referred to as prior fail log in  the block diagram) is obtained from sort test. This fail log  describes the failure signature in terms of fail pin names and  cycle numbers. Figure 4 shows a very simplified illustration of  a test pattern with expected logic states. A failure signature  consisting of 3 error bits is highlighted. During fault  localization, the tester activates a good device using the fail  test pattern of interest with the test operating point set at the  margin of the passing window. A synchronized pulsed  scanning laser beam stimulates the logic active region of  interest and outputs a failure signature, if it exists, for every  pixel. This is compared against the prior fail log on the fly  using a comparator module. In the event of a match, a pulse is  triggered to register the location of the laser beam for signal  image acquisition. A signal spot on the screen thus represents  a potential defect or weakpoint on the bad die which  corresponds to the failure signature of interest. In this way, the  suspected locations of the hard defect can be electrically  filtered and identified for further trace analysis. Several  schemes of comparison based on different combinations of fail  pin names and fail cycles is possible; the most stringent being  all output fail pin names/ cycle numbers matched to the failure  signature. Since the success of this technique relies heavily on  the ability of the laser beam to stimulate as many ‘healthy


transistors’ as possible for electrical test filtering, this explains  the need for pulsed laser, especially in advanced technology.


Figure 3: Electrically-enhanced LADA (EeLADA) system  block diagram.


||Pin_A|Pin_B|Pin_C|Pin_D|Pin_E|Pin_F|
|---|---|---|---|---|---|---|

|1|H|L|L|L|H|H|

|2|H|L|H|H|H|L|

|3|L|L|H|H|L|L|

|4|H|H|L|H|L|H|

|5|L|L|H|H|H|L|

|6 7|L H|H L|H L|L H|L H|H H|

Figure 4: Simplified illustration of a test pattern consisting of  pin names and cycle numbers.


Error number|Cycle number


Pinname 67292BPI_BUS7


H


通 Expected dataReceived data


67294


BPI BUS7


2


67293


BPI_BUS2


汪


山67296


BPI_BUS7


67295


n


Experimental Results


567298


BPI_BU57


67299


067300


H H 2


67297


BFI_BUS7


67301


In a general product yield ramp, embedded memories and


67302


8


9


logic failures are 2 commonly encountered yield detractors. When software-based fault isolation tools such as bitmapping  or scan diagnosis are not available, investigation becomes a  challenge and dynamic EFI are usually explored. This section  presents data based on a 28 nm technology device to


乔


demonstrate the feasibility and limitations of using EeLADA  to address these challenges


Memory Fault Isolation


Figure 5(a) shows the error log from memory built-in-self-test (BIST) testing. The failure signature which comprises of the  fail pin name, cycle number and fail state information are  detailed. There are close to 100 embedded memory arrays in  the core of interest and EeLADA successfully localizes the  failure array by matching the exact failure signature using a  good die. The signal image is as shown in FIG 5(b). Figure  5(c) shows the signal overlay to an optical laser image. In this  case, EeLADA is only able to narrow down the failure to array  level and is unable to pinpoint to the defective cell. This is  expected because any defective memory bit fails in this array  will give rise to the same electrical failure signature on test, typical of BIST. Hence, the precision of EeLADA is  electrically-limited. A direct access memory test methodology


is the only way that EeLADA is able to pinpoint to a defective  cell. Nevertheless, this EFI result has demonstrated the  feasibility of EeLADA application on memory hard failure  fault localization to guide physical failure analysis in the  absence of bitmapping. The identified memory array is sent


Prior Fail Log


for subsequent physical failure analysis. Figure 6 shows the


Comparator


Fail


scanning electron microscopy (SEM) image at polysilicon


Automatic Testlog.


layer after contact (CA) removal to reveal the CA footprint.


Equipment


Locations A and B highlight the presence of very marginal CA


Match


Probe stack


Trigger


footprint and the failure mechanism is suspected to be likely  due to unlanded CA issues. Further analysis on inline defect


Good Die


inspection using electron beam found similar concerns and a


Laser Scanning


Stage


new mask fixes this issue.


Microscopy Tool中 Pulsed


Scanner


Image


Laser


ProcessorCRT


Logic Fault Isolation


On another device of similar technology, a programmed defect


Photodetector


(PD) is created on a known good die using 1340nm cw laser at  a logic active region as indicated by the crosshair in the  reflected laser image in Fig 7. The die is verified to be a hard  fail on scan testing and the error log is as shown in Fig. 8. There are 1 fail cycle and 4 failing pins. In the first  experiment, a less stringent condition is chosen by matching  the electrical failure pin signature. Stimulated signal images  from pulsed- LADA and EeLADA acquired from the entire  die are compared. It takes a total of 24 frames at 20x objective  to complete the inspection die, out of which 8 reveals  differences. Figure 9 shows results from 2 of the locations. Figure 9(a) and 9(c) shows the pulsed-LADA signals at these  2 locations and Fig. 9 (b) and


266958


JTMS


25


2000m


200ur


Figure 5: (a) Error test log from MBIST test, (b) EeLADA  signal image and (c) signal overlay to reflected laser image.


9(d) show the corresponding EeLADA signal images. The  pulse frequency is 10 kHz and the pulse width is 50 s. The  missing signals from EeLADA are encircled. These missing


signals represent locations of “healthy transistors” which when


perturbed, give rise to a fail signature that matches the 4  failing pin names.


500nm


Figure 6: Scanning Electron Microscope (SEM) photograph  at polysilicon layer after contact (CA) removal.


One of these missing signals is the location of the defect. In  this relaxed scheme of comparison, it is expected that the  missing signal is not localized because it does not take into  consideration the failing cycle. Figure 10(a) and 10(b) compare the pulsed-LADA and EeLADA signal images at the  known location of PD respectively. The crosshair indicates the  position of laser damage and it is observed to be part of the  missing EeLADA signals. In the second experiment, the most  stringent electrical failure signature matching is applied and  results as shown in Fig. 11. Figure 11(a) shows the EeLADA  signal image in the region of interest and Fig. 11(b) shows the  signal overlay to reflected laser image. EeLADA successfully  pinpoints the PD location.


Figure 7: Reflected laser image on logic active where PD is  created. The crosshair indicates the PD locality.


50 μm


chip_top_0_new_laser:69531171059 69532L.....H


LL..


Figure 8: Error test log from scan testing.


Conclusion


In this paper, we introduce EeLADA as a new approach to  extend conventional LADA’s capability to investigate  integrated circuits hard functional failures. In the first part, we  demonstrate the enhancements of pulsed-LADA as compared  to cw LADA and found that more LADA signals can be


100um


100ur


160um


(d)


Figure 9: (a), (c) Pulsed-LADA and (b), (d) corresponding  EeLADA signals based on 10kHz, 50s pulse width laser and  fail pin matching, at 2 different logic regions. Missing signals  from EeLADA encircled.


PPPPPPPPPPPPPPPPPPPPPPPPPPPPPPPPP AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA56 DDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDD


Figure 10: (a) Pulsed-LADA and (b) EeLADA signals based


STTTIITTTTTTEEEEEEEIIIIIIIILIIS5L


on 10kHz, 50s pulse width laser and fail pin matching. PD


MSSSSSSSS5SSJJJJJJJ22222222222PPE 95598859959DDD CDCDSVCTTTDRT


ITD


location marked with a crosshair.


17654321078005NDKSOKINTSUNNUUUUUUUU


CTTZUSB


_UN元SOCMWMSSSSBT KCSUDDDDC


Vechddr


RptCat Vaenaddr Cycle


KT 123K TTTIIITTOI 1100QD0000FF


Figure 11: (a) EeLADA signal based on 10kHz, 50s pulse  width laser and fail signature matching and (b) signal overlay  to reflected laser image.


stimulated using pulse width in the range of tens of s and  kHz frequency. Though ps pulse width laser at femtosecond  frequency presents more signals as expected, through an  analysis on the locations of stimulated sites at low  magnification, the s pulsed laser beam suggests being good  enough to gain the benefits of pulsed- LADA. We then  introduce EeLADA which utilizes a pulsed laser beam to


stimulate ‘healthy’ transistors on a good device and


electrically filters the pulsed-LADA signals to derive a signal  image that indicates the possible defect locations to guide  subsequent layout analysis or physical failure analysis. The  feasibility of EeLADA is demonstrated experimentally on a  real product embedded memory and logic device. EeLADA  seeks to compliment dynamic photon emission as broad area  FI approach to interrogate product hard failures. This work  also opens up a new and unconventional perspective in FI by  the use of good dies to pinpoint potential failure locations.


References


[1] MR Bruce et al., “Soft Defect Localization (SDL) in  Integrated Circuits using Laser Scanning Microscopy”, The 16th Annual Meeting of the IEE, Oct 2003, pp. 662-663.


[2] JA Rowlette JA and ME Travis, “Critical timing analysis  in microprocessors using near-IR laser assisted device  alteration (LADA).” IEEE International Test Conference (ITC), IEEE Computer Society.2003, pp. 264-264.


[3] ZL Qian, C Brillert, Burmer C, Y Yokoyama, “Differential and lockin imaging of dynamic photon  emission and applications in failure analysis”, Proc Int’l  Symp for Testing and Failure Analysis, 2010, pp. 373- 377


[4] S Kasapi et al., “Volume Electrical Failure Analysis for  Product- Specific Yield Enhancement”, Proc Int’l Symp  for Testing and Failure Analysis, 2010, pp. 38- 48.


[5] SH Goh, WY Lau, BL Yeoh, HW Ho, GF You, Hu Hao, Jeffrey L, “Debugging Phase-Locked Loop Failures in  Integrated Circuit Products”, Proc Int’l Symp for Testing  and Failure Analysis, 2014, pp. 465.


[6] U Kindereit, G Woods, J Tian, U Kerst, R Leihkauf, C  Boit, “Quantitative Investigation of Laser Beam  Modulation in Electrically Active Devices as Used in  Laser Voltage Probing”, Device and Matl Rel, IEEE, Vol  7, Issue 1, 2007, pp. 19-30.


[7] SH Goh, et al., “Effectiveness of frequency mapping on  28nm device broken scan chain failures”, Rev Sci  Instrum, Vol 83, Issue 2 (2012), 023702


[8] G Celi, et al., “Thermal Frequency Imaging: A new  application of Laser Voltage Imaging applied on 40nm  technology” Proc Int’l Symp for Testing and Failure  Analysis, 2011, pp. 19.


[9] SH Goh, et al., “Advanced CMOS device fault isolation  using frequency mapping on passive structures”, Proc  Int’l Symp for Testing and Failure Analysis, 2013, pp.


420.


[10] SH Goh, et al., “Debugging Phase-Locked Loop Failures  in Integrated Circuit Products”, Proc Int’l Symp for  Testing and Failure Analysis, 2014, pp. 465.


[11] VK Ravikumar, R Wampler, MY Ho, J Christensen, SL  Phoa, “Laser Voltage Probing in Failure Analysis of  Advanced Integrated Circuits on SOI”, Proc Int’l Symp  for Testing and Failure Analysis, 2012, pp. 1.


[12] KA Serrels, N Leslie, TR Lundquist, P Vedagarbha, , “Two Photon-Absorption-Enhanced Laser Assisted  Device Alteration and Single-Event Upsets in 28nm  Silicon Integrated Circuits”, Proc 39th Int’l Symp for  Testing and Failure Analysis, November 2013, pp. 173-181.


[13] J Shaw, M Christopher, SN Yin, B Felix, “Dual Port  RAM MBIST Failure Analysis using Time Resolved  Dynamic Laser Stimulation”, Proc 34th Int’l Symp for  Testing and Failure Analysis, November 2008, pp. 188–


191.


[14] K Eringon, J Asquith, D Bodoh, “Software enhanced time  resolved laser assisted device alteration with a non-pulsed  laser source”, Proc 35th Int’l Symp for Testing and  Failure Analysis, November 2009, pp. 43.


[15] D Bodoh, K Erington, “Improving the DLS Workflow”, Proc 38th Int’l Symp for Testing and Failure Analysis, November 2012, pp. 183.


[16] D Bodoh, K Erington, K Dickson, “Root Cause Analysis  Techniques Using Picosecond Time Resolved LADA”, Proc 40th Int’l Symp for Testing and Failure Analysis, November 2014, pp. 82–86.


[17] KB Erington, JE Asquith, “Time Resolved Radiation  Assisted Device Alteration”, U.S. Patent 0261840 A1, Oct 22, 2009.


ISTFA 2015: Conference Proceedings from the


Copyright © 2015 ASM International®


41st International Symposium for Testing and Failure Analysis


All rights reserved.


November 1–5, 2015, Portland, Oregon, USA


asminternational.org


Visible Light LVP on Bulk Silicon Devices


Joshua Beutler, V. Carter Hodges, J. Joseph Clement, Jeffery Stevens, and Edward I. Cole Jr.


Sandia National Laboratories, Albuquerque, NM, USA


Scott Silverman and Robert Chivas


Varioscale Incorporated, San Marcos, CA, USA


Abstract


Visible light laser voltage probing (LVP) for improved  backside optical spatial resolution is demonstrated on ultrathinned bulk Si samples.  A prototype system for data  acquisition, a method to produce ultra-thinned bulk samples as  well as LVP signal, imaging, and waveform acquisition are  described on bulk Si devices.  Spatial resolution and signal  comparison with conventional, infrared LVP analysis is  discussed.


Introduction


Laser Voltage Probing (LVP) is a key backside tool for  modern failure analysis and real time logic debugging of  signals propagating at operational speeds through integrated  circuits (ICs).  Conventional LVP systems rely on free carrier  generation and optical absorption within the transistor  channels to create a modulated reflected light intensity.  Infrared wavelengths are used to take advantage of Si’s  relative transparency for backside probing.  The incident light  is reflected back, captured, detected, and amplified.  The small  modulations in reflected intensity resulting from free carrier  density changes with electric field are used to determine local  transistor logic states as a function of time.  This is a powerful  tool for failure analysis and device debugging/characterization [1-2].


With the continual IC feature size reduction, backside, laserbased failure analysis tools are limited in spatial resolution by  the refraction limits of light and the relatively long  wavelengths required for through-silicon probing.  Even with  state-of-the-art Solid Immersion Lenses (SILs), modern 22 nm  devices are past the limit of smallest feature resolution.


To help address this spatial resolution limit, we developed and  demonstrated the effectiveness of applying LVP with shorter, visible wavelengths on silicon-on-insulator (SOI) devices [3].  Here we demonstrate the approach on bulk Si devices using  ultra-thinning.  Functionality is maintained as devices are


thinned sufficiently so that shorter, visible wavelengths can be  used for LVP analysis, thus enabling better spatial resolution  and enhanced LVP signals.


Visible light LVP on bulk Si devices brings with it new  complexities in sample preparation.  Bulk Si devices proved  significantly more difficult and time intensive than SOI  sample preparation.  This is primarily due to the absence of a  buried oxide layer which acts as an etch stop for Si etching of  the substrate.  In the absence of a built-in etch stop, several  other methods of ultra-thinning were used to achieve a usable  sample.  Note that the efforts in sample preparation  development produced discoveries in metrology, advanced  milling, and selective Si removal tools that greatly reduce the  guess work initially involved in ultra-thinning to generate a  final sample suitable for visible light LVP.  These techniques  will be discussed throughout the paper.


System and Sample Description


We demonstrate LVP using visible light (633 nm) on locally, ultra-thinned regions within bulk Si devices by incorporating  advanced deprocessing techniques to ultra-thin localized areas  and achieve a packaged, functionality-maintained IC.  These  techniques include, Laser Assisted Chemical Etch (LACE), Pulsed Laser Assisted Chemical Etch (PLACE) [4], conformal  mechanical milling and polishing, and Reactive Ion Etching (RIE).


A modified LSM 310 scanning laser microscope was used to  demonstrate LVP using visible light.  In order to effectively  probe the transistor, a high gain, low noise Avalanche  Photodiode (APD) is used as the detector of the LVP signal (Figure 1).


Our earlier work described the motivation for examining ultrathinning and using visible light microscopy to significantly  enhance spatial resolution with air gap and oil immersion  lenses [3].  The examples shown in this paper are for bulk Si  technologies at the 90 nm and 40 nm technology nodes.


Figure 1: Schematic diagram of a modified LSM 310 with an  APD detector and multiple wavelength sources for visible  light LVP analysis.


LACE and PLACE


Laser microchemical etching and deposition processes were  studied extensively in the early 1980s. Continuous wave (CW) laser induced melting of Si in a gaseous Cl environment can  result in a high spatial resolution etch [5].  This pyrolytic  technique is now commonly known as Laser Assisted  Chemical Etching (LACE) and is extensively used to prepare  active devices for focused ion beam circuit edit.  In addition to  the LACE method, pulsed lasers have also been used to  photolytically etch Si while in a Cl gas environment [6-10].  Both photolytic and pyrolytic methods using pulsed rather  than CW lasers are now referred to as Pulsed Laser Assisted  Chemical Etching (PLACE).


PLACE offers a significant advantage compared to LACE for  ultra-thinning over functional device layers.  The shape of the  Si melt zone for LACE is hemispherical with a melt depth  approximately equal to the radius of the laser beam spot  diameter [11].  However, the shape of the melt zone for  nanosecond PLACE resembles that of a thin disk due to short  pulse thermal confinement. The melt depth to first order is  proportional to the fluence (i.e. energy per unit area) of each  laser pulse and at 532 nm is as shallow as 100 nm. Further, since each pulse operates independently, the thermal load on  the device may be set by adjusting the pulse repetition rate. Thermal load control while maintaining etching above melt  threshold is especially important when processing large, ultrathin membranes while maintaining device functionality.


For PLACE ultra-thinning, we used a VarioEdit™, which was  modified for the specific purpose of laser assisted chemical  etching of Si.  The modifications included retrofitting the  VarioEdit™ with a JDS Uniphase Q-series diode pumped, pulsed laser.  The JDS Uniphase laser outputs a wavelength of  532 nm with a variable repetition rate and corresponding  variable pulse width.  This work was accomplished using a


200 kHz repetition rate and corresponding pulse width of 380  nanoseconds.  The selected energy varied from approximately


0.5 µJ to 1.5 µJ (100 mW to 300 mW average power).  When  combined with spot size and scan rate, this resulted in removal  rates of < 50 nm to 500 nm per total area scanned.


90 nm Bulk Si Example Results


As a proof of concept, a bulk Si, 90 nm Xilinx Virtex 4 FPGA  was prepared with a 250 µm x 250 µm region of interest.  The  region of interest covered an implementation of a shift register  operating at 12.5 MHz with a core voltage of 1.2 V.   Deprocessing the region of interest consisted of backside Si  removal over the entire die by lapping to 100 µm.  The region  of interest created using LACE and PLACE to a Remaining  Silicon Thickness (RST) of ~ 3 µm.  At this point a series of  isotropic RIE Si etches were performed to remove more Si  until roughly 1 µm RST within the thinnest portions of the  region of interest remained.


Figure 2: Reflected light image (top left) and 12.5 MHz  frequency map (top right) of the shift register on a  conventional LVP system using 1320 nm light and 20x  objective to create the reflected light image.  When the laser is  pointed at a region of operation indicated by the black dots in  the LVI image, the LVP signal is indicated by a spectral peak  at the operational frequency (bottom).


A conventional, backside, 1320 nm LVP system was used to  show functionality of the shift register as well as derive an  understanding of the overall conventional LVP signal for the  example shown in Figure 2.


On the ultra-thinned bulk Si device a visible light source is  applied for LVP probing.  This laser is a 5 mW, 633 nm  HeNe, with approximately 500 µW of power on the sample  with the 10x objective.  The shift register was clocked by an  onboard crystal oscillator.  Figure 3 illustrates visible light  Laser Voltage Imaging (LVI) [12] of the shift register, “zero  spanning” the spectrum analyzer on the operational frequency (12.5 MHz).  The analyzer’s video output is used to modulate  the image contrast as the 633 nm laser is scanned across the  device.  In this example the frequency map is slightly offset  due to the scan speed and latencies within the spectrum  analyzer.  This is similar to conventional LVI, but shown here  to work at a visible wavelength on an ultra-thinned bulk Si  device.


When spotting the laser on a region of LVI activity, the APD  reflected light response to the shift register operational  frequency is 15 dBm above the noise floor (Figure 3).


Figure 3:  Backside, 633 nm, 10x objective reflected light  image (top left) and LVI image (top right) of the ROI  containing a shift register operating at 12.5 MHz.  When a  633 nm laser is pointed at a region of operation indicated by  the white dots in the LVI image, the LVP signal is indicated by  a spectral peak at the operational frequency (bottom).


The Visible Light LVI image in Figure 3 can be compared  with the conventional LVI image in Figure 2 to highlight  several factors that influence the strength and uniformity of  Visible Light LVI.  One factor is wavelength resolutionn.  Due  to the improved resolution of the 633 nm laser, the LVI  regions are more sharply defined.  In contrast, the Si at the  bottom of the ultra thinned region is not perfectly flat.  This is  observed by the Visible Light LVI signal falling off as the Si  thickness increases near the edge of the trench.  As the Si


continues to get thicker the LVP signal is fully obscured.  The  1320 nm LVI image shows no such issues.  The turn-key 1320  LVI also uses an auto contrasting, histogram stretching  algorithm and 16 bit images to enhance  all regions operating  at the zero span frequency.  This type of an algorithm does not  exist on in the Zeiss LSM 310 software and is applied in post  processing on an 8 bit image.  Lastly, it should be noted that  differences between the two LVI images may be due to  different photon/carrier interactions between the 633 nm and  1320 nm laser with the CMOS logic.


Figure 4 shows LVP waveforms for the 633 nm and 1320 nm  LVP systems from spotting the laser at an active region of the  Virtex 4 shift register implementation. For this example the  output of the amplifed APD signal is displayed directly with a  Tektronix 70000 series fast acquisition oscilloscope. The  sinusoidal nature of the 633 nm LVP signal is due to the 25  MHz, 3dB bandwidth limits of the detector system.


1320 nm 20x Air Gap


633 nm 10x Air Gap


To RsdivRef 0.00 d8m


0.0200.on400.0n600.on800.0n1.op


Seconds (s)


Figure 4:  12.5 MHz shift register waveforms with  conventional (1320 nm) and visible light (633 nm) LVP.


M


A Span 10.00KMz


Res BW 91Hz


40 nm Bulk Si Example Results


To further extend the proof of concept visible light LVP to a  more advanced technology node, a bulk Si, 40 nm Xilinx  Virtex 6 FPGA was ultra-thinned over a 250 µm x 250 µm  region in a manner similar to the Virtex 4 previously  described.  In this case the region of interest was over a 4  MHz clock governing the operation of a shift register with a  core voltage of 1 V.


A conventional, backside, 1320 nm LVP system was used to  show functionality of the clock as well as derive an  understanding of the overall conventional LVP signal.  These  1320 nm tests were performed on the ultra-thinned bulk Si  device and are shown using a 16 mW probe power and a 20x  objective in Figure 5.   The comparison visible light LVP on  the same ultra-thinned bulk Si device is shown in Figure 6,


Figure 5 Reflected light image (top left), LVI image (top right) of clock on SR using 1320 nm laser and LVP signal of the 4


ISTFA  2015


Conference Proceedings from the 41st International Symposium for


Testing and Failure Analysis


November 1–5, 2015


Oregon Convention Center Portland, Oregon, USA


TM


Organized by


Published by


ASM International


Materials Park, Ohio 44073-0002


®


ASM INTERNATIONAL


asminternational.org/istfa


EDFAS Electronic Device Failure Analysis Society


5INTERNATIONALASM


Copyright  2015


by


ASM International® All rights reserved


No part of this book may be reproduced, stored in a retrieval system, or transmitted, in any form or by any  means, electronic, mechanical, photocopying, recording, or otherwise, without the written permission of the  copyright owner.


Great care is taken in the compilation and production of this book, but it should be made clear that NO  WARRANTIES, EXPRESS OR IMPLIED, INCLUDING, WITHOUT LIMITATION, WARRANTIES OF  MERCHANTABILITY OR FITNESS FOR A PARTICULAR PURPOSE, ARE GIVEN IN CONNECTION WITH  THIS PUBLICATION. Although this information is believed to be accurate by ASM, ASM cannot guarantee  that favorable results will be obtained from the use of this publication alone. This publication is intended for  use by persons having technical skill, at their sole discretion and risk. Since the conditions of product or material  use are outside of ASM's control, ASM assumes no liability or obligation in connection with any use of this  information. No claim of any kind, whether as to products or information in this publication, and whether or not  based on negligence, shall be greater in amount than the purchase price of this product or publication in respect  of which damages are claimed. THE REMEDY HEREBY PROVIDED SHALL BE THE EXCLUSIVE AND  SOLE REMEDY OF BUYER, AND IN NO EVENT SHALL EITHER PARTY BE LIABLE FOR  SPECIAL, INDIRECT OR CONSEQUENTIAL DAMAGES WHETHER OR NOT CAUSED BY OR  RESULTING FROM THE NEGLIGENCE OF SUCH PARTY. As with any material, evaluation of the material  under end-use conditions prior to specification is essential. Therefore, specific testing under actual conditions is  recommended.


Nothing contained in this book shall be construed as a grant of any right of manufacture, sale, use, or  reproduction, in connection with any method, process, apparatus, product, composition, or system, whether or  not covered by letters patent, copyright, or trademark, and nothing contained in this book shall be construed as a  defense against any alleged infringement of letters patent, copyright, or trademark, or as a defense against liability  for such infringement.


Comments, criticisms, and suggestions are invited, and should be forwarded to ASM International.


ISBN-13: 978-1-62708-102-3   ISBN-10: 1-62708-102-X                                                                                                        EISBN: 978-1-62708-103-0                                                                                                   SAN: 204-7586


ASM International®


Materials Park, OH 44073-0002  www.asminternational.org


EDFAS 2015‐2016 BOARD OF DIRECTORS 


EDFAS President 


Ms. Cheryl Hartfield 


Oxford Instruments Company 


EDFAS Vice President 


Mr. Zhiyong Wang Maxim Integrated 


EDFAS Board Members 


Position 


Affiliation 


President 


Mr. Zhiyong Wang 


Vice President 


Maxim Integrated 


Dr. William E. Vanderlinde 


Secretary 


IARPA 


Mr. Christopher L. Henderson 


Financial Officer 


Semitracks, Inc. 


Mr. Jeremy A. Walraven 


Past President 


Sandia National Laboratories 


Mr. Terry F. Mosier 


Associate Managing Director  ASM International 


Mr. Nicholas Antoniou 


Member at Large 


Revera Inc. 


Dr. Martin Keim 


Mentor Graphics 


Dr. Lee Knauss 


Booz Allen Hamilton 


Ms. Sandra Delgado 


Nanolab Technologies 


Ms. Susan Li 


Spansion Inc. 


Mr. David Su 


TSMC 


Board Committees 


Mr. Jon D. Tirpak 


ASM BOT Liaison 


SCRA Applied R&D 


Dr. Felix Beaudoin 


EDFA Chair 


Global Foundries 


Dr. Mayue Xie 


Education Chair 


Intel Corp. 


Dr. James J. Demarest 


Events Chair 


IBM 


Dr. Thomas Moore 


Membership Chair 


Waviks, Inc. 


Nominating Chair 


Dr. David Su 


International Growth 


iii


2015 ORGANIZING COMMITTEE 


Dr. Sam Subramanian 


General Chair 


Vice‐General Chair 


Technical Program Chair


Tutorial & Short Course Chair   


Freescale Semiconductor


Spansion, Inc. 


Mr. Dan Bodoh 


Immediate Past General Chair 


Freescale Semiconductor 


ACTIVITIES CHAIRS 


Nicholas Antoniou 


User Group Chair 


Felix Beaudoin 


Attendee Chair 


Lihong Cao 


International Chair 


Jan Olaf Gaudestad 


Expo Chair 


David Grosjean 


Panel Chair 


Becky Holdford 


AV Chair 


Rick Livengood 


Local Arrangements 


Efrat Moyal 


Expo Co‐Chair 


Rose Ring 


User Group Vice Chair and Movie Chair 


David Su 


International Co‐Chair 


Kendall Scott Wills 


Panel Vice Chair 


Mayue Xie 


Tutorial & Short Course Vice Chair 


iv


   ISTFA 2015 TECHNICAL PROGRAM COMMITTEE   


ISTFA 2015 Technical Program Chair Dr. Sam Subramanian 


SESSION CHAIRS 


3D Device Failure Analysis 


Frank Altmann, Fraunhofer Institute for    Mechanics of Materials 


Yan Li, Intel 


Board and System Level FA 


Victoria Bruce, Qualcomm Incorporated Ted Kolasa, Orbital Sciences Corporation  


Case Studies and the FA Process 


Zhigang Song, GlobalFoundries 


Rose Ring, GlobalFoundries Malta 


Detecting Counterfeit Microelectronics 


Robert Champaign, Raytheon Network Centric   Systems 


Joe Colangelo, Raytheon Network Centric  


  Systems 


Device Failure Analysis 


Diagnostic Testing, Scanning and Debug 


Geir Eide, Mentor Graphics 


Mark E. Kimball, Maxim Integrated Products,    Inc. 


Electrical and Yield 


Gregory M. Johnson, GlobalFoundries Jenny Ma, Intel 


Emerging FA Techniques and Concepts 


Terence Kane, IBM 


Phil Kaszuba, GlobalFoundries 


FA Lab Management 


Rose Ring, GlobalFoundries Malta Zhigang Song, GlobalFoundries 


Fault Isolation 


Michael Bruce, Consultant 


Paiboon Tangyunyong, Sandia National    Laboratories 


FIB Circuit Analysis and Edit 


Jason Benz, GlobalFoundries 


Michael DiBattista, Qualcomm, Inc. 


FIB Sample Preparation 


Carl Nail, Evans Analytical Group 


Tom Schamp, Hitachi High Technology    America Inc. 


Metrology and In‐Line Device    Characterization 


Bryan Tracy, Evans Analytical Group Huimeng Wu, Carl Zeiss Microscopy 


Microscopy 


Tom Schamp, Hitachi High Technology America  Inc. 


Nanoprobing and Electrical Characterization 


Kent Erington, Freescale Semiconductor Randal E. Mulder, Silicon Labs 


Package and Physical Analysis Challenges   Tutorial 


Susan Li, Cypress Semiconductor 


Chris Richardson, Allied High Tech Products 


Packaging and Assembly Level FA 


Lihong Cao, Advanced Micro Devices 


Bhanu P. Sood, CALCE, University of Maryland 


Sample Preparation and Device Deprocessing 


Roger Alvis, FEI Company 


Jake E. Klein, Texas Instruments 


Scanning Probe Analysis 


Technology Specific FA Tutorial 


Mark Jenkins, Sandia National Laboratories Corey Senowitz, Qualcomm Technologies 


v


vi


Contents


IPFA Best Paper


Fault Isolation Using Electrically-Enhanced LADA (EeLADA) ..........................................1


S.H. Goh1, B.L. Yeoh1, G.F. You1, H. Hao1, W.L. Sio1, J. Lam1, and C.M. Chua2


(1) GlobalFoundries


(2) Semicaps Pte. Ltd.


Emerging Failure Analysis Techniques and Concepts


Visible Light LVP on Bulk Silicon Devices ..................................................................... 6


J. Beutler1, V.C. Hodges1, J.J. Clement1, J. Stevens1, E.I. Cole, Jr.1,  S. Silverman2, and R. Chivas2


(1) Sandia National Laboratories


(2) Varioscale Incorporated


Electrically-Enhanced LADA (EeLADA) Technique ....................................................... 14


Laser Logic State Imaging Using Transient Voltage Collapse Circuits ........................... 21


G. Baek, J. Keane, and M. von Haartman Intel Corporation


Fault Isolation


Pulsed Laser Stimulation Coupled with Optical Failure Analysis Technique—


A Methodology to Help Space Application Electrical Designers  ................................... 25


G. Bascoul1, K. Sanchez2, G. Perez2, F. Bezerra2, and H. Chauvin3


(1) Intraspec Technologies


(2) Centre National d’Etudes Spatiales


(3) Thales Communication and Security


Soft Defect Localization on Analog and Mixed-Signal ICs Using an OBIRCH Tool ............ 31


C. Wu, X. Li, and Y. Che


Freescale Semiconductor (China) Limited


Combinational Logic Analysis Using Laser Voltage Probing......................................... 35


V.K. Ravikumar, W. Lua, S.Y. Xuan, G. Ranganathan, and A. Phoa Advanced Micro Devices


Comparison of Photon and Thermal Emission Microscopy for Dynamic Fault Isolation .. 42


S.H. Goh, G.F. You, A. Tan, C.V. Bharadwaj, H. Hao, B.L. Yeoh, and J. Lam GlobalFoundries


vii


Unique Approaches to Isolate Nanoscale Defect in Snake-Comb Test Structure ............ 47


S. Xie, N. Wang, C. Chen, and Q. Wu Maxim Integrated


Optical Fault Isolation and Nanoprobing Techniques for the


10 nm Technology Node and Beyond ......................................................................... 52


M. von Haartman, S. Rahman, S. Ganguly, J. Verma, A. Umair, and T. Deborde Intel


Device Ioff Mapping—Analysis of Ring Oscillator by Optical Beam Induced


Resistance Change .................................................................................................. 57


G.M. Johnson, Z. Xu, and C. D’Aleo GlobalFoundries


Focused Ion Beam Sample Preparation


Vacuum Assisted Ex Situ Lift Out for Manipulation of FIB Prepared Specimens ............. 61


L.A. Giannuzzi1, D. Hess2, and T. Clark2


(1) EXpressLO LLC


(2) The Pennsylvania State University


How Xe and Ga FIB Differ in Inducing Lateral Damage on TEM Samples ........................ 65


T. Hrnčíř1, J.V. Oboňa1, M. Petrenec1, J. Michalička2, and C. Lang3


(1) TESCAN Brno


(2) TESCAN ORSAY Holding


(3) Oxford Instruments Nanoanalysis


Turning Sample Into (Re)Solution—Focused Ion Beam


Shaped Solid Immersion Lenses  .............................................................................. 71


P. Scholz1, M. Sadowski1, C. Boit1, S. Kupijai1, M. Henniges1, C. Theiss1, S. Meister1,  D. Stolarek2, H.H. Richter2, and M. Boostandoost3


(1) Berlin University of Technology


(2) IHP


(3) Dialog Semiconductor


Scanning Probe Analysis


Near Field EMC Scanning Method Based on an E-Field Collapse  .................................. 76


J. Dunnihoo1, P. Tamminen2, and T. Viheriäkoski3


(1) Pragma Design, Inc.


(2) Microsoft


(3) Cascade Metrology


Extending Electrical Scanning Probe Microscopy Measurements of


Semiconductor Devices Using Microwave Impedance Microscopy   .............................. 82


B. Drevniok1, S. Dixon-Warren1, O. Amster2, S.L. Friedman2, and Y. Yang2


(1) Chipworks Inc.


(2) Prime Nano Inc.


viii


Focused Ion Beam Circuit Analysis and Edit


Alleviating Sample Charging during FIB Operation .................................................... 87


Q. Liu, H.B. Kor, Y.W. Siah, and C.L. Gan Nanyang Technological University


Circuit Tracing on Integrated Circuit Using  FIB Passive Voltage Contrast Effect   .......... 92


A. Sorkin1, C. Pawlowicz1, A. Krechmer1, and M.W. Phaneuf2


(1) TechInsights


(2) FIBICS


An Infrared Microscope for Use on a Focused Ion Beam for Circuit Edit and


Backside Edit Applications  ...................................................................................... 97


A. Richards1, M. Weschler1, and M. Durller2


(1) Technical Sales Solutions LLC


(2) Battelle


Board and System Level Failure Analysis


Time Domain Reflectometry—Case Studies in Electrical Failure Isolation  ..................104


J. Wheeler and S. Fasolino


Raytheon Space and Airborne Systems


Failure Analysis of Yellow Banding on Optically Bonded Touch Screen   ......................108


Q. Gu, J. Lewis, and D. Xu Microsoft Corporation


Microscopy


Detection and Measurement of Intermetallic Thin Films Using EDX Line Scanning  ......114


C. Nail, EAG


Quantitative SiGe TEM Elemental Analysis in FinFET Test Structures ..........................120


J. Demarest and J. Bruley IBM


3D Devices Failure Analysis


Failure and Stress Analysis of Cu TSVs Using GHz-Scanning


Acoustic Microscopy and Scanning Infrared Polariscopy ............................................124


I. De Wolf1, A. Khaled1, M. Herms2, M. Wagner2, T. Djuric3, P. Czurratis3, and S. Brand4


(1) Imec


(2) PVA Metrology & Plasma Solutions GmbH


(3) PVA TePla Analytical Systems GmbH


(4) Fraunhofer Institute for Mechanics of Materials IWM


ix


Fast Feature Based Non-Destructive Fault Isolation in 3D IC Packages


Utilizing Virtual Known Good Device  .......................................................................131


K.C. Lee 1, J. Alton1, M. Igarashi1, and S. Barbeau2


(1) TeraView Limited


(2) IBM Systems


Failure Analysis Strategies for Multistacked Memory Devices with


TSV Interconnects  .................................................................................................135


F. Altmann1, C. Grosse1, F. Naumann1, J. Beyersdorfer1, and T. Veches2


(1) Fraunhofer Institute for Mechanics of Materials IWM,


(2) Micron Technology, Inc.


3D Integrated Power—A Discrete Perspective  ..........................................................141


I. Kearney and S. Brink Texas Instruments


Analysis of Integrated Current Sense in Multiphase Buck Converters ..........................147


I. Kearney, Texas Instruments


Detecting Counterfeit Microelectronics


Update on Draft SAE AS6171 Standard—Tools and Techniques for Detection and


Mitigation of Counterfeit Electronics  ......................................................................152


W.E. Vanderlinde1 and B.P. Sood2


(1) Intelligence Advanced Research Projects Activity


(2) University of Maryland


Analyzing the Impact of X-Ray Tomography on the  Reliability of Integrated Circuits ...154


H. Dogan1, M.M. Alam2, N. Asadizanjani2, D. Forte2, M. Tehranipoor2, and S. Shahbazmohamadi3


(1) University of Connecticut


(2) University of Florida


(3) Manhattan College


Non-Destructive PCB Reverse Engineering Using  X-Ray


Micro Computed Tomography .................................................................................164


N. Asadizanjani1, M. Tehranipoor1, D. Forte1, and S. Shahbazmohamadi2


(1) University of Florida


(2) Manhattan College


2015 ISTFA Presentation #1: 2010–2015—The Evolving Counterfeit Machine   ............173


T. Sharpe, SMT Corp.


Functional Electronic Clones—The Most Dangerous New Counterfeit Threat


Facing the Entire Electronics Industry Today   ..........................................................177


Techniques for Reverse Engineering and Functionality Extraction of


Mixed-Signal ICs for Security Applications  ...............................................................179


F. Stellari, C.-C. Lin, L. Gignac, R. Robertazzi, A. Weger, and P. Song IBM T.J. Watson Research Center


x


WISE and ICARUS—New X-Ray Algorithms to Improve the Detection of


Counterfeit Components   .......................................................................................189


B. Cardoso, Creative Electron, Inc.


Materials Analyses for Parts Validation ....................................................................199


W.J. Wolfgong and J. Izzo Raytheon Company


Metrology and In-Line Device Characterization


In-Line Detection of Deep Trench Moat Underetch Defects Using eBeam Inspection .....205


R.F. Hafer1, B. Messenger1, M.T. Dekker1, O.D. Patterson1, Y. Feng1, S.-C. Lei2, and X. Tang2


(2) Hermes Microvision Inc.


SIMS Quantitative Analysis and Optimization for Ion Implantation Angle Deviation  ....211


J.B. Shi, W.T. Chien, Q.H. Zhang, A.M. Li, and C.J. Liu


Semiconductor Manufacturing International (Tianjin) Corporation


Posters


Magneto-Optical Frequency Mapping System for Very Low Resistance Short Circuit


Failure Imaging ......................................................................................................217


T. Nakamura, Hamamatsu Photonics K.K.


Magnetic Current Imaging Power Short Localization .................................................222


J. Gaudestad1, F. Rusli1, A. Orozco1, and M.C. Pun2


(1) Neocera


(2) Avago


A Case Study of Failure Analysis on ESD-Induced Degradation of 405 nm LD ................227


H. Liu, Z. Li, Z. Weng, H. Jiang, and Y. Shen Chinese Academy of Sciences


Failure Analysis of Embedded Non-Volatile Memory with Nano- and


Micro-Probing Techniques ......................................................................................230


X.-D. Wang, A. Yazzie, J. Buchert, L. Will, P. Wang, and S. Guisinger Freescale Semiconductor, Inc.


Analysis of Write Recovery Time Degradation Caused by


Adjacent Storage Node Data in DRAM .......................................................................234


K. Lee, I. Nam, D. Kim, H. Hwang, S. Rhee, K. Cho, and G. Jin Samsung Electronics Co., Ltd.


Failure Analysis Induced by Bit Line Sense Amplifier Noise in High Density DRAM  .......237


M. Lee, S. Ko, D. Bae, H. Hong, H. Hwang, S. Rhee, K. Cho, and G. Jin Samsung Electronics Co., Ltd.


xi


Laser Stimulation Effect on FinFET and Case Study  ..................................................241


K. Jin, S. Lee, K. Kim, Y. Lee, and Y. Kim Samsung Electronics Co., Ltd.


Implementation of a Visual System to Manage and


Improve Failure Analysis Work Flow ........................................................................245


J.M. Benz, K.A. Distelhurst, D.B. Hunt, and R. Kontra GlobalFoundries


IR Thermography for Temperature Measurements and Fault Location on


AlGaN/GaN HEMTs and MMICs .................................................................................253


L. Baczkowski1, F. Vouzelaud1, D. Carisetti2, N. Sarazin2, J.-C. Clément2, J.-C. Jacquet3,  C. Gaquiére4, B. Lambert5, and L. Brunel5


(1) Thales Systèmes Aéroportés


(2) Thales Research and Technology


(3) III-V Lab


(4) IEMN


(5) United Monolithic Semiconductors


Comparison of Magnetic Field Imaging and Thermal Laser Stimulation for


Detecting Electrically Shorting Defects within a Die BEOL .........................................258


K.A. Distelhurst, GlobalFoundries


Isolating Electrically Open Laminate Defects Using


Space Domain Reflectometry with a Superconducting


Quantum Interference Device .................................................................................261


Symptom or Cause? A Case Study ............................................................................264


A. Swaminathan, J. Liao, and H. Marks NVIDIA


Logic LIVA Fault Isolation in Synthesized Logic  ........................................................267


T. Pifer and T.M. Eiles Intel Corporation


How to Locate Resistance VIA by Analysing Schematic Combined with


EMMI Result on Integrated Circuit Failed at Cold Temperature  ..................................270


G. Wen, L. Tian, J. Li, C. Qi, and D. Wang PA Lab of Freescale Semiconductor


A Combination Continuous Wave and Pulse Laser Assisted


Chemical Etching Processes through Encapsulated IC Packaging ...............................274


M.M. Mulholland1 and S. Silverman2


(1) Intel Corporation


(2) VarioScale Inc.


Failure Mechanism Studies and Elimination of Galvanic Corrosion (Al-Cu Cell) on


Microchip Aluminum Bondpads in Copper Process ....................................................278


H. Younan, C. Yixin, F. Chao, and L. Xiaomin WinTech Nano-Technology Services Pte. Ltd.


xii


Non-Destructive Contamination Detection in Thick and


Extremely Thin SOI Wafers Using Optical Second Harmonic Generation  .....................282


M.C. Kryger1, J.P. Changala1, and M.L. Alles2


(1) FemtoMetrix, Inc.


(2) Vanderbilt University


A Study of How Different FIB Beam Current Intensities Locate Possible Defects ...........290


W.C. Shu and Y.H. Shu


United Microelectronics Corporation, Ltd.


Studies on a Qualification Method (OSSD) for Microchip Al Bondpads  ........................295


H. Younan, S. Yue, C. Yixin, F. Chao, and L. Xiaomin WinTech Nano-Technology Services Pte. Ltd.


Application of Scanning Acoustic Microscopy for Micro Delamination Detection   .........298


H. Kim, S. Lee, H. Kim, and S. Kim QRT Inc.


Selective Etching of Heavily-Boron-Doped Si Substrate Using


Lightly-Boron-Doped Si Epi as an Etch Stop Layer   ...................................................306


V. Korchnoy, Intel Israel


A More Rapid Approach in Revealing the Physical Status of Polyfuses and


Thin Film Fuses in a Multilayer Integrated Circuit   ....................................................314


J.H. Lagar, R.A. Sia, and M.S. Cajita Analog Devices Gen. Trias, Inc.


TEM Sample Preparation Tricks for Advanced DRAMs ................................................318


C.S. Sung, H.T. Lee, and J.S. Luo Inotera Memories, Inc.


Case Study—Doping Profile Analysis for 30 nm DRAM Devices


Using SCM and SSRM  .............................................................................................323


H.-P. Chen1, J.-S. Luo1, C.-S. Sung1, C.-K. Wei1, K.-L. Chiang1, C.-M. Yang2,  H.-C. Liao2, J. Suo3, and S. Lu3


(1) Inotera Memories, Inc.


(2) Chang Gung University


(3) Micron Technology, Inc.


Carrier Redistribution Analysis of Gate-Biased SiC Power-MOSFET


Using Super-Higher-Order Scanning Nonlinear Dielectric Microscopy  ........................329


N. Chinone and Y. Cho Tohoku University


Observation of Polarization and Two-Dimensional Electron Gas in


AlGaN/GaN Heterostructure Using Scanning Nonlinear Dielectric Microscopy  .............333


K. Hirose, N. Chinone, and Y. Cho Tohoku University


xiii


Environmental Control Scanning Nonlinear Dielectric Microscopy Measurements of


p-n Structures, epi-Si Wafers, and SiC Crystal Defects  ..............................................336


J.-J. Yu1, T. Yamaoka2, S. Hasumura2, R. Hirose2, K. Ando2, and K. Mizuguchi2


(1) Hitachi High Technologies America, Inc.


(2) Hitachi High-Tech Science Corporation


Diagnostic Testing, Scanning, and Debug


Tester Assisted Multiple Emission Microscopy  ..........................................................344


C. Hollerith, G. Borgmann, W. Schaller, C. Burmer, and C. Brillert Infineon Technologies AG


FASTKIT—A Software Tool for Easy Design Visibility and


Diagnostic Enhancement for Failure Analysis  ...........................................................349


E. Auvray and P. Armagnat STMicroelectronics


Strategies to Address Low DPPM Failure Mechanisms on


Automotive Grade Wi-Fi Radio Frequency Devices .....................................................358


K. Wang, S. Lone, C. Thomas, and R. Weaver  QualcommTecyhnologies International, Ltd.


Device Failure Analysis


A Case Study—Improving FIB Passive Voltage Contrast Imaging for


Deep N-Well Circuits  ..............................................................................................364


R. Mulder, Silicon Laboratories, Inc.


Fault Isolation and TEM Study in State-of-Art Thin-Film Transistors  ..........................374


Y. Zhou, S.L. Lee, C. Fu, Y. Hua, and X. Li


WinTech Nano-Technology Services Pte. Ltd.


Analysis Approach on DMOS Transistor Vth Mismatch Due to  Trapped Charges ...........378


H. Ismail1, A.C. Keow1, and K.G.C. Siong2


(1) Infineon Technologies (Kulim) Sdn Bhd


(2) Infineon Technologies AG


Nanoprobing and Electrical Characterization


High Resolution Electron Beam Induced Resistance Change for


Fault Isolation with 100 nm2 Localization  ................................................................382


B.A. Buchea, C.S. Butler, H.J. Ryu, W.-H Chuang, M. von Haartman, and T. Tong Intel


xiv


Plasma FIB DualBeam Delayering for Atomic Force NanoProbing of


14 nm FinFET Devices in an SRAM Array  ...................................................................388


R. Alvis1, T. Landin1, C. Rue1, P. Carleson1, O. Sidorov1, A. Erickson2, S. Zumwalt2, S. Dixon-Warren3,  W.-Y. Liu4, S.H. Chang4, T.-F. Chang4, C.-H. Yen4, P.-S. Kuo4, and C.-H. Chu4


(1) FEI Company,


(2) Multiprobe Inc.


(3) Chipworks


(4) Materials Analysis Technology


Nanoprobing Applications with Capacitance-Voltage and


Pulsed Current-Voltage Measurements for Device Failure Analysis   ............................401


L.L. Lai1, N. Li1, Q. Zhang1, T. Bao2, and R. Newton2


(1) Semiconductor Manufacturing International Corp. (SMIC)


(2) DCG Systems


Advanced Failure Analysis of Junction Profile Defect by Using EBAC/EBIC  ..................409


J.H. Lee, J.Y. Lee, D.W. Kim, K.W. Jung, and S.Y. Son SK Hynix Semiconductor


Non-Visible Defect Analysis by the Nanoprobing Methodology  ..................................414


C.Q. Chen, G.B. Ang, P.T. Ng, A.C.T. Quah, H.P. Ng, A. Teo, J. Lam, and Z.H. Mai GlobalFoundries Singapore Pte. Ltd.


Packaging and Assembly Level Failure Analysis


Corrosion Mechanisms of Cu Bond Wires on AlSi Pads  ...............................................418


W. Qin, H. Anderson, T. Anderson, G. Chang, and D. Barrientos ON Semiconductor


Failure Modes Associated with Plastic Packages and Copper Bond Wires  ....................424


K. Berger1 and S.A. Lilani2


(1) Analytical Solutions


(2) Integra Technologies LLC


X-Ray Microscopy and Root Cause Analysis in Electronic Packaging   ..........................430


L. Mirkarimi1, A. Gu1, L. Hunter1, G. Guevara2, M. Huynh2, and R. Katkar2


(1) Carl Zeiss X-Ray Microscopy,


(2) Invensas Corporation


Acid Decapsulation for Silver Wire Bonded Package  .................................................436


S. Suzuki and M. Yamaguchi


What Happens to Electrostatic Sensitive Devices in Case of


Direct ESD from Plastics? ........................................................................................441


P. Jacob, EMPA Swiss Fed Labs for Materials Testing and Research


Root Cause Analysis of a Connector Time-Delayed Fracture  ......................................451


P. Singh1, Y. Yu1, and R.E. Davis2


(1) IBM Corporation


(2) GlobalFoundries


xv


Sample Preparation and Device Deprocessing


A Simple Method to Fabricate a Tunable In Situ SIL ...................................................455


M. Kimball, Maxim Integrated


Adaptive Grinding and Polishing of Silicon Integrated Circuits to


Ultra-Thin Remaining Thickness   ............................................................................460


R. Chivas1, S. Silverman1, and M. DiBattista2


(1) Varioscale Incorporated


(2) Qualcomm Incorporated


The Changing Role of Advanced Sample Preparation in


X-Ray Inspection Supporting 2.5D and 3D Sample Failure Analysis   ...........................466


R.M. LaVoy1, F. Babian1, M. Mulholland2, and S. Silverman3


(1) SVXR Inc.


(2) Intel Corporation


(3) Varioscale Inc.


LASER Combined with Plasma—Will It Be the Future’s Green and


Safe IC Decapsulation Method .................................................................................474


P. Poirier and M. Obein Digit Concept


Decapsulation of Multichip BOAC Devices with Exposed Copper Metallization  Using


Atmospheric Pressure Microwave Induced Plasma ....................................................480


J. Tang1, K.D. Staller2, and K. Beenakker3


(1) JIACO Instruments B.V.


(2) Texas Instruments


(3) Delft University of Technology


Repeatable Method for Automated Decapsulation of Silver Alloy Wire Packages .........491


M. Lefevre1, E. Noraz2, and D. Veychard2


(1) JP Kummer SAS


(2) STMicroelectronics


Case Studies and Failure Analysis Process


Resistive Contrast Imaging—The Tool, Technique, and Applications on


Leading-Edge Semiconductor Technology Devices   ...................................................496


R.M. Ring1, R. Newkirk1, K. Davidson1, J. Capriola1, J. Russell1, A. Rummel2, and E.C. Carper3


(2) Kleindiek Nanotechnik GmbH


(3) FEI Company


Failure Analysis Methodology on Circular Patch Functional Failure Due to


Device Parametric Drift   .........................................................................................503


A.C.T. Quah, C.Q. Chen, G.B Ang, D. Nagalingam, H.P. Ng, P.T. Ng, S.J. Moon,A. Teo, K.H. Yip, J. Lam, and Z.H. Mai


GlobalFoundries Singapore Pte. Ltd.


xvi


Failure Analysis of ILD Delamination—Uncovering Multiple Root Causes  ...................507


M. Castignolles1, T. Zirilli1, E. Cattey2, J. Lewenstein2, S. Schauer2, W. Liu2, J. Chen2,  J. Hammett2, and S. Subramanian2


(1) Freescale Semiconductor


(2) Freescale Semiconductor, Inc.


Invisible Defect Root Cause Identification with Electrical and Chemical Analyses  .......513


Z. Song, Y. Wang, and S. Pendyala GlobalFoundries


Author Index .........................................................................................................519


Fault Isolation using Electrically-enhanced LADA (EeLADA)


SH Goh, BL Yeoh, GF You, Hu Hao, WL Sio, Jeffrey Lam


GLOBALFOUNDRIES, Technology Development, Product Test and Failure Analysis, Singapore


CM Chua


Semicaps Pte Ltd


Email: SzuHuat.Goh@globalfoundries.com


Pulsed-LADA is found to play an important role in the  advancement of next-generation LADA and it is reported that  tens of s pulses with 10 kHz frequency is sufficient to  observe enhancements in carrier injection. Electricallyenhanced LADA (EeLADA), based on pulsed-LADA, is  introduced as a new fault localization method capable to  overcome current limitation of Laser Assisted Device  Alteration (LADA) application on soft failure and extends it to  hard failure debug. We present the EeLADA methodology and  experimental data to demonstrate its feasibility.


A fast product yield ramp in a foundry depends largely on the  ability to localize defects in the shortest possible time. This is  the pre-requisite to identify a failure root cause before any  process or reliability fix plan can be formulated. As  technology scales and chip design gets more complicated, defect localization becomes more challenging. Static electrical  fault isolation (EFI) using few pins bias has been shown to be  less effective to activate functional fail-related defects. This  explains the heightened interest in dynamic EFI which uses a  tester to configure the device into the failure mode during fault  localization.


Currently, a variety of baseline dynamic EFI techniques are  available and their applications are well discussed in literature. In principle, hard and soft device failures are 2 main groups of  fails, requiring distinctly different dynamic EFI approach. Unlike hard failures, a device suffering soft failure is able to  pass under certain test corners. Soft Defect Localization (SDL) and Laser Assisted Voltage Alteration (LADA) are wellknown FI techniques to debug a soft failure [1,2].


For hard failures, the first go-to technique is usually dynamic  photon emission microscopy (PEM) because of its simplicity  and speed in execution [3-5]. However, this approach is  limited to failures that give rise to abnormal emission  hotspots. Consider the case that no emission spots are  observed on a bad device, either due to non-leakage failures or  weak signals beyond detection sensitivity from reducing  voltage levels in advanced technologies, the next logical  option is to explore laser-based techniques. Currently, the only  laser technique to diagnose hard failures is frequency mapping


[6]; however, it is limited to frequency-related failures like


scan chain shift [7,8], toggling I/O pins [9] or phase-locked  loop (PLL) fails [10]. It does not apply to product logic hard  failures in the absence of periodic switching states. Although  laser probing technique which utilises the same low noise  1300nm continuous wave (cw) wavelength laser as frequency  mapping can be employed to examine the transients from logic  capture cycles, prior suspects and design inputs are prerequisites [11]. However, they are usually not readily available  in a foundry debug or EFI service environment. Therefore, the  technical challenge remains in the lack of a laser-based FI  technique to complement dynamic PEM for general large area  fault localization.


This paper presents a potential solution to address this  challenge. We first define pulsed-LADA and show its  enhancements before introducing the EeLADA concept. Experimental data based on memory and logic failures will be  presented to demonstrate its feasibility.


Block Diagram


Figure 11 depicts the block diagram of the EeLADA  methodology. Prior to debug, the fail log of the targeted fail  die is acquired. This is referred as the reference failure  signature. The components bounded by dashed lines are part  of a standard laser scanning microscopy tool and will not be  described. We employ a wafer level microscopy system in this  work [21]. The other elements in the EeLADA setup involve  the automatic test equipment, also commonly called tester  which activates the die via a test probe stack. As laser scans  the die, a fail log is generated in the event of a positive circuit  response to laser stimulation. The comparator module parses  this fail log and compares against the reference failure  signature on-the-fly. This is achieved by synchronizing the test  run with comparison. Whenever a match to failure signature  occurs, a trigger pulse is generated and sent to the image  grabber to locate the circuit.


Figure 11: Electrically-enhanced LADA (EeLADA) system  block diagram.


The essence of EeLADA lies in the comparison procedure. It  can be visualized as an electrical filter that only allows LADA  signals that corresponds to the failure signature in question to  be selected. In this way, the failure-relevant signal can be  derived. In principle, various comparison schemes are  possible. The criterion can be pre-determined to match just the  fail pins, fail cycles, a subset or the exact combination of fail  pins and fail cycles according to the actual fail log. The latter  is the most stringent. In general, EeLADA can be applied to  both soft and hard failures debug. However, unlike soft  failures, a good die is analyzed when a hard failure is  investigated. Finally, although pulsed-LADA is one prerequisite, technically, a cw laser can also be used, but it might  not be effective for advanced technology node device.


The next two subsections discusses the capabilities of  EeLADA using test cases.


MHz clock (bottom).  Data was taken with a 16 mW beam  power and a 20x objective.


10 udiy


10.0


1kRef-20.00 dBm


Ref 0.00 dBm


|using a 633 nm HeNe laser and a 10x objective with approximately 500 µW of power on the sample.  When spotting the laser on the probe site of the UTLVI image, the primary harmonic of the 4 MHz clock is seen in the spectrum analyzer at roughly 15 dBm above the noise floor. |尔||
|---|---|---|

Nm


Center 3.999990 MHz Res BW 91 Hz


Span 10.00 kHz


N


Figure 6: Reflected light image (top left), LVI image of the  shift register (top right) clock using a 633 nm laser, and LVP  signal of the 4 MHz clock (bottom).  Data was taken with a


Center 4.000000 MHz


#Res BW 91 Hz


200 µW beam power and a 10x objective.


Probing and acquisition of the waveforms with 50x objectives  is shown in Figure 7.  While the two waveforms sufficiently  manifest waveform timing, there are notable differences


between the two waveforms. The overall waveform health of  the visible light waveform indicates RC rise and fall issues.


0.0500.0n


1.oμ1.5p


2.0μ


Figure 7:  4 MHz shift register waveforms from the ultra-thin  regions shown in Figures 5 and 6.  These waveforms were  taken using a 20x objective, 16 mW, 1320 nm probe and 10x  objective, 500 µW, 633 nm probe.


Hyper-Resolution on 40 nm Bulk Si


Hyper-resolution or use of objectives with an NA (Numerical  Aperture) of greater than 1 showed relatively comparable  results between the conventional LVP with a 2.6 NA SIL on a  100 µm thick Si sample and the visible light LVP with a 1.4  NA oil imerrsion lens on an ultra-thin target.  The results are  shown for the Virtex 6 shift registers comparing and  contrasting the trade-offs between ultrathin visible and  conventional IR LVP.


to geldiy


-.


700


to gevicdy8dPm


街0


100


s


Span 10.00kHz


Res BW 91 Hz


Figure 8: Reflected light image (top left), LVI image (top  right) of the shift register clock using a 1320 nm laser, and  LVP signal of a 4 MHz clock (bottom).  All data was taken  with a 6 mW beam and a 300x, 2.6 NA SIL.


1320nm 2.6 NA SIL机向楼按的


Figures 8 and 9 show the differences between hyper-resolution  techniques that are commercially available for IR and visible


yAR'Hmpu


LVP systems.  The difference in contrast between the  refelected light images of the two sources is primarily due to


633nm 1.4 NA Oil


the differences in absorption of the two light sources on the  integrated circuit.  The LVI images, though similar, show


壹壹


differences as well.  These are likely due to different  photon/carrier interactions between the 633 nm and 1320 nm  laser within the CMOS logic.  The big difference between the  hyper-resolution images is the presence of fringes in the ultrathin sample.  This will be covered in the next section.


0.0500.0n1.0μ


1.5μ


The waveforms acquired by the two using hyper-resolution


optics are shown in Figure 10.  These waveforms show similar  timing with significant overshoot on the visible light  waveform.  The reason for this is not fully understood and  may also be due to the visible probe interaction with the  CMOS logic or an artifact of the measurment system.


Figure 9: Reflected light image (top left), LVI image (top


Span 10.00 KHz


right) of the shift register clock using a 633 nm laser, and LVP


signal of 4 MHz clock (bottom).  All data was taken with a ~200 µW beam power and a 63x, 1.4 NA oil immersion  objective.


Seconds (S)


Figure 10: LVP waveforms of the 4 MHz clock taken from


the same regions and using the same parameters


described in Figure 9.


Ultra-Thin Metrology and Non-Uniformity


The presence of fringes in the ultra-thin reflected light images  is caused by non-uniformity in the ultra-thin Si membrane.  This phenomomon, commonly called Newton rings, is created  when reflected light from the membrane surface and device  surface interfere in a constructive or destructive manner.  These fringes were not observed when doing visible light LVP  on SOI devices because the device layer was uniform in  thickness and much thinner than the wavelength of the probing  laser. In the case of our bulk Si samples, the Si is thinnest  where the rings are most concentric and gradually thicker  moving toward the sidewalls of the trench.  We expect that  further developments in the LACE and PLACE processes as  well as developments in supporting techniques will improve  the uniformity of the Si membrane and thereby reduce the  fringing effect.


Of primary importance in ultra-thinning is a metrology tool  capable of measuring ultra-thin Si membranes with submicron accuracy.  Conventional, backside, infrared metrology  tools fall short of this goal due to their inability to measure  thin film Si with an RST < ~5 µm.  This can be overcome by  using a visible light metrology tool.  This tool can be used to  characterize RIE etches on ultra-thin Si to stay within the  narrow window of visible light transparency and device  functionality.  A 60 µm wide by 120 µm long thickness


Final ThicknessSurvey, Mean 5.1 um, Range 1.4 um


uniformity histogram and plot of the center region shown in


1.6


70


1.8


Figure 5 is shown below in Figure 11.


1.4"


60 50


1.2n只


12


30


0.8e


10-


0.6


20


0.4


8-


10


0.2


Count


pr u"90.764.855


4 6


0


u 10


心40


1d6 10


Value


cleta


5.6


4000


5.4


Thldoes Unformib: Ma*13on;Ras*23onRange*1.0am


是


2.6


5.2


Ara-01mm


习


4.6


是2000


4.8


00 mm; ex=00mm


18


-30002000-10000100020003000


X(um):Min =-3.8 mm;Max=3.8mm;Range= 7.6mm


6000


4.2


0AN03CUP) 8


4.4


2.4


5


Figure 11: Thickness uniformity histogram (top)  and contour  plot (bottom) of 11 X 11 measurements in a 60 x 120  µm  region of the Virtex 6 sample shown in Figure 5 using a  Varioscale visible light metrology tool.


Another method of ultra-thinning involves mechanical milling  of Si die.  This method is superior to conventional lapping  provided the mill can remove the substrate to ensure that the  overall remaining silicon is relatively thin and uniformly thick. In such a scenario an isotropic RIE etch can be performed on  the remaining substrate to create a Si membrane suitable for  visible light LVP.  This sample prep scenario is subsequently  illustrated.  A combination of milling and mill based polishing  was used to thin a Virtex 6 die to ~ 5 µm uniform thickness  with a range of 1.4 µm.  The thickness uniformity map and  survey are shown below in Figure 12. While the complete  functionality of the FPGA was not verified, it was able to load  and run the shift register implementation in the same manner  as other Virtex 6 devices used in this study.  Reactive Ion  Etching was then used to selectively thin a region of ~ 2.5 mm  x 3.5 mm to a membrane thickness of ~ 1µm.  A white light  microscope image and thickness uniformity map of the region  is shown in Figure 13.  A thickness uniformity map of the  silicon membrane after etching is shown in Figure 14. After  the etch, this part remained functional long enough for some  conventional LVP results to be obtained before is began  failing POST tests and would no longer load the shift register  routine.  The reason for the part failure remains unknown.  A  reflected light image and corresponding LVI image of the shift  register clock prior to failure are shown in Figure 15.


Bin


121819 192020 212.22.22.32.42.5


5.8


Thickness Uniformity; Min = 4.3um; Max= 5.7um; Range= 1.4um


1B


工商


to9


Figure 12: Thickness uniformity histogram (top) and contour  plot measurement (bottom) across an entire Xylinx Virtex 6  die with a target thickness of 5 µm RST.


Figure 13:  Backside white light image of a 40 nm Xylinx  Virtex 6 FPGA prepared for Visible Light LVP by thinning the  region of interest to roughly 1 micron remaining silicon  thickness.


X (um):Min =-0.8 mm;Max=0.8mm;Range=1.6mm


Figure 14: Thickness uniformity histogram (top) and contour  plot (bottom) of a region of the silicon membrane shown in  Figure 13.


Figure 15: Reflected light image (left) and corresponding LVI  image (right) of a shift register clock using a 1320nm laser on  the ultra-thin region shown in Figure 13. Data acquired with  a 10 mW beam  and a 50x objective.


Conclusions


LVP using visible light is for the first time demonstrated on


Thickness of Lever 1


bulk Si devices.  Sample preparation methods are described,


140


limitations are discussed, and solutions to several of these


120-


limitations are offered.  Side-by-side visible light LVP and  conventional IR LVP examples showing spectral acquisition,


frequency mapping and waveform generation are performed


to


on 90 nm and 40 nm bulk Si devices using air gap and hyperCount


resolution objectives.


古


Acknowledgements


Sandia National Laboratories is a multi-program laboratory


122is is


managed and operated by Sandia Corporation, a wholly owned


Thickness Uniformity:Min =0.9um;Max=2.0wm;Range =1.1um


subsidiary of Lockheed Martin Corporation, for the U.S.


2.2


Department of Energy's National Nuclear Security


注


dota


003


Administration under contract DE-AC04-94AL85000.


。


高


爸


The authors express their thanks to Doug Greth for


customizing and executing the Reactive Ion Etching shown in


w


this work.


1.4


-500


"


1.2


1000


0.8


-800-600-4002000200400600800


[1] Kindereit et al., “Quantitative Investigation of Laser  Beam Modulation in Electrically Active Devices as  Used in Laser Voltage Probing”, IEEE Transactions  on Device and Materials Reliability, Vol. 7, No. 1, (2007).


[2] Ravikumar, V. K. et al., “Laser Voltage Probing in     Failure Analysis of Advanced Integrated Circuits on  SOI”, 19th International Symposium on the Physical  and Failure Analysis of Integrated Circuits, Singapore, July 2012 pp. 1-4.


[3] Beutler et al., “Visible Light LVP on Ultra-Thinned  Substrates”, Proceedings of the 40th International


Symposium for Testing and Failure Analysis, Houston, TX, November 2014,  pp. 110-114.


[4] Chivas et al., “Preparation of Wafer Level Packaged  Integrated Circuits using Pulsed Laser Assisted  Chemical Etching”, Proceedings of the 38th  International Symposium for Testing and Failure  Analysis, Phoenix, AZ, November 2012, pp. 491-497.


[5] D.J. Ehrlich, R.M. Osgood, Jr. and T.F. Deutsch, “Laser chemical technique for rapid direct writing of  surface relief in silicon”, App. Phys. Lett 38 (1981) 1018


[6] C. Paulsen-Boaz, W. L. O’Brien and T.N. Rhodin, “Pulsed ultraviolet laser stimulated chlorination  mechanisms for Si(111)”, J. Vac. Sci. Technol. B  Vol. 10, No. 1 (1992), pp 216-220.


[7] T.N. Rhodin, C. Paulsen-Boaz and W.L. O’Brien, “Dynamics of pulsed ultraviolet laser enhancement of  the chlorine-Si(111) reaction”, Surf. Sci., Vol. 283


(1993) pp. 109-116.


[8] T.S. Baller and J. Dieleman, “Nanosecond excimer  laser-enhanced chemical etching”, Appl. Surf. Sci., Vol. 43 (1989), pp. 409-415.


[9] F. Foulon and M. Green, “Projection-patterned  etching of silicon in chlorine atmosphere with a KrF  excimer laser”, Appl. Phys. A Vol. 61, No. 6 (1995), pp. 655-661.


[10] R. Kullmer and D. Bӓuerle, “Laser-induced chemical  etching of silicon in chlorine atmosphere”, Appl. Phys. A, Vol. 43, No. 3 (1987), pp. 227-232.


[11]  J.Y. Tsao and D.J. Ehrlich “Surface and gas  processes in photo-deposition in small zones,” Proc. SPIE 0459, June 1984.


[12]  Ng et al., “Laser Voltage Imaging: A new  Perspective of Laser Voltage Probing”, Proceedings  of the 36th International Symposium for Testing and  Failure Analysis, Dallas, TX, November 2010, pp. 5-13.


Electrically-enhanced LADA (EeLADA) Technique


A modulated laser beam in the form of a continuous pulse  train is explored on Laser Assisted Device Alteration (LADA). We term this pulsed-LADA to differentiate from conventional  continuous wave (cw)-LADA. It is found that a duty cycle of  less than 0.9 at low frequency above 1 kHz is sufficient to  experience significant enhancements in laser stimulation. Following this, a new derivative of LADA technique called  Electrically-enhanced LADA (EeLADA) is developed. Experimental results to demonstrate its capability in  improving diagnostic resolution and potential application to  hard failure debug will be presented.


Laser assisted device alteration (LADA) is a common failure  analysis (FA) lab technique that is used for both  characterization and localization of sensitive speed paths in  integrated circuits (IC). It is based on photoelectric laser  stimulation effect. Photocurrent generated induces timing  shifts in critical signal paths resulting in a temporary flip of IC  test state from pass-fail or vice versa [1, 2, 3]. By custom  practice, a 1064 nm continuous wave (cw) laser beam rasters  the region of interest (ROI) through the backside of silicon die  to generate electron hole pairs while a complete test run is  executed at least once per pixel. The test condition can be  fixed at either side of the pass-fail margin and the position of  the scanning laser correlates to the change in electrical test  state for signal image acquisition.


Several works to characterize and model the effects of  photocurrent in p-n junctions, diodes and field effect  transistors (FETs) under the influence of cw laser and varying  bias conditions have been discussed extensively [4, 5, 6]. The  different effects of cw and pulsed laser systems on scan cells  are also studied [7]. Recently, pulsed photoelectric laser  stimulation is gaining some traction especially in the  understanding of single event upsets (SEU) testing on FETs  and memory cells [8, 9, 10], as well as obtaining temporal  information from speed-limiting circuit paths using timeresolved LADA (TR-LADA) technique [11, 12, 13]. However, pulsed laser system has never been reduced to practice for  typical LADA application. It could be due to a misconception  that a small pulse width (PW) in the range of ns to ps is


required to achieve a high peak power and it is not economical  to implement, or simply, it has no value add.


In this work, we demonstrate the enhancements and  significance of a pulsed laser system for conventional LADA  applications using modulated lasers. Although we make use of  transistor-transistor logic (TTL) modulated laser beam in this  work, we adopt pulsed-LADA as a general term since in  reality, similar phenomenon can be experienced by pulse  trains generated using gain (Q) switching or mode-lock lasers. Unlike most studies, instead of characterizing the influence of  laser stimulation on elementary devices, we approach from a  macroscopic viewpoint by analyzing the electrical test  response from the output strobe pins.


Building up on these enhancements on pulsed-LADA, we  develop an improved LADA technique called Electricallyenhanced LADA (EeLADA) which is capable to assess the  criticality of LADA signals and enhance diagnostic resolution. Potentially, this technique could also overcome the current  limitation of LADA technique [14] in soft failures debug and  complement existing dynamic fault isolation (FI) techniques  like photon emission [15, 16], frequency mapping [17, 18] and  laser voltage probing (LVP) [19] in debugging hard failures  that cannot be accessed by static means.


This paper is organized as follows: Section 2 compares the  stimulation ability of pulsed and cw laser beam. The concept  of EeLADA is described in section 3. Under both sections, experimental data based on 28 nm process technology devices  will be presented. Section 4 briefly discusses the limitation of  EeLADA. The findings are summarized in the concluding  section 5.


Synchronized Pulsed-LADA


LADA Signal Enhancements


Since pulsed-LADA is commonly associated for works  relating to TR-LADA, Fig. 1 clarifies the definition of pulsedLADA in this context. Technically, both techniques are  similar in the way that they involve a pulsed laser system  synchronized to the test pattern. However, the mode of pulsing  is markedly different. TR-LADA uses a small pulse duration  to enhance the optical beam induced current (OBIC) and is  employed primarily to acquire temporal information on critical  device or sensitive paths of interest.


Figure 1: Different laser scan modes for LADA applications.


One pulse is normally triggered at a pre-determined test cycle  within a complete test loop per pixel. In this context, pulsedLADA refers to laser stimulation using a periodic pulse train  which is applied in a similar manner to conventional LADA. However, 2 runs are required in the case of pulsed-LADA  with a 180-degree phase shift between the pulse trains. This is  represented by the 1010 and 0101 modulated waveforms as  illustrated in Fig. 1. This is to ensure complete laser  stimulation on the entire test pattern. For all the laser scan  modes, the inception of laser scanning is synchronized to the  tester clock.


Figure 2(a) shows a shmoo plot analysis from a good  reference device tested on memory built-in-self-test (MBIST). It describes the test results graphically under varying  conditions of vdd and test frequency (1/period). By assigning  the test operating point to be close to the margin in the pass  window, conventional cw-LADA is performed and the signal  image as shown in Fig. 2(b). The signals are acquired using  5X objective lens. The laser power measured from the fiber  output is 450 mW.  Pulsed-LADA is performed on the same  region of interest (ROI) using both 1010 and 0101  modulations and the signal images as shown in Fig. 3(a) and  Fig. 3(b) respectively. The PW is 30 s and the frequency  equals 10 kHz.  Fig. 3(c) shows the technical signal image for  pulsed-LADA combining (a) and (b). There are slight  differences in signals between 1010 and 0101 modulations and  it is observed that cw-LADA signals are a subset of pulsedLADA. This result hints at a relatively weaker stimulation  power using cw laser beam.


This finding reinforces the results from a previous experiment  conducted using a femtosecond pulsed laser with picosecond (ps) PW. The results are as shown in Fig. 4. Figure 4(a) shows  the signals obtained on cw-LADA. Figure 4(b) and (c) show  the signals obtained from pulsed-LADA at 10 kHz, 50 s PW  and femtosecond frequency, ps PW, respectively. It is  apparent that the signals from the ps pulsed laser are  significantly stronger as compared to the s one, likely due to  extreme high peak power and some extent of 2pLADA effect. An interesting point to highlight is the similarity in the  locations of stimulated sites. It suggests that s pulsing could  be sufficient, at least for the next technology nodes. The


results from these two experiments reveal the limitation of cw  laser.


Analysis on Minimum Average and Peak Power


At the location indicated X in Fig. 4(b), the s pulsed laser  beam is fixed in position using spot mode. The output laser  from the fiber is approximately 537 mW in continuous wave  and the minimum PW to observe a change in test state at  varying frequency of 4 kHz to 1 kHz is obtained. The duty  cycle is calculated from the ratio of PW over pulse period. The  average power of the modulation is measured from the fiber  output using a power meter. From the measured pulsed  average power and calculated duty cycle, the pulsed peak  power can be calculated. It should be noted that this is not the  delivery power to the sensitive circuits and are meant for  relative comparison purpose. The graph as shown in Fig 5  summarizes the result. There are three conclusions that can be  drawn from this analysis.


Figure 2: (a) Shmoo plot of analysis and (b) cw-LADA signal  image acquired from a good reference die.


Figure 3: Pulsed-LADA signal image acquired using (a)


1010 and (b) 0101 modulating laser beam using 5X objective  lens. (c) Technical signal image combining (a) and (b).


sirw


5 μm


Figure 4: (a) cw-LADA, pulsed-LADA at (b) 10 kHz, 50 s


EINT2


Laser OFF


pulse width and (c) femtosecond frequency, ps pulse width.


cw laser


First, as duty cycle reduces, the minimum peak power stays  almost constant, except for a slight insignificant increase. This  reveals the presence of a minimum peak power threshold


5Ius PW puled-laer


needed to cause a soft error. Second, the pulsed average power  is observed to be significantly reduced while still fulfilling this  threshold. In this way, the pulsed laser beam is able to mitigate


60 μs PW pulsed-laser


thermal build up from high incidence continuous stimulation  which can subsequently cause permanent damage to “healthy  transistors”. Lastly, based on the calculated minimum peak


90 us PW pulsed-laser


powers, there is clear evidence that very high peak power in


Cycles44144


44149


44153


the range of W or even MW as reported [20] is not the bottomline to experience enhancements from pulsed laser beam. The  enhancement from pulsed-LADA (pass-fail state transition) could be explained by the possible activation of parasitic  bipolars in pulsed laser beam stimulation on FETs [4, 6, 10] which is not happening when using cw.


Duty Cycle


Figure 5: Minimum average and peak power required to


induce a state change on test at location X indicated in Fig. 4(b) under conditions of varying duty cycle.


Effects of Pulse duty cycle on Output Pin Response


Pulsed-LADA signals in the logic areas that are absent in cwLADA are encircled in Fig. 3(c). Figure 6(a) shows the signals  when observed under 50X objective lens. The laser beam is


fixed in position using spot mode at the location marked with  a crosshair while the response of the output pin EINT2 is


examined using the tester’s waveform debugging tool. Figure


6(b) presents the output pin signal response between test


5μm


zoni


Figure 6: (a)Pulsed-LADA signal image acquired using 50X  objective lens on logic region encircled in Fig. 3(c) .(b)


Output pin waveforms for selected fail test cycles of interest  under varying PW at 10 kHz.


600


cycles 44144 and 44153. The response is evaluated to


500


determine the pass/fail state at the end of each cycle. A ‘1’ refers to an expected high and ‘X’ indicates that the pin is not


营Average power


strobed in that cycle for pass/fail. From Fig. 6, it is evident


Peak power


that when the laser is switched off, the pin passes because the  signal maintains above voltage output high (VOH) level up till


Power (Js1)200兰


44149, satisfying the expected states from these cycles. In the  case of a cw laser beam, it is apparent that transistors are not  stimulated sufficiently to affect the behavior of the signal


Wavelength:1064 nm


Power(measured before obj. lens):537 mW


response from the output pin.


0.10.20.30.40.50.60.70.8


This explains the absence of the LADA signals in Fig. 2(b). The signal response under varying PW modulation at 10 kHz (period 100 s) is next analyzed. It is observed that a pulsed  laser beam of 50 s and 60 s PW is capable of altering the  signal response and the test fails after cycle 44146. As PW  increases closer to cw condition at 0.9 duty cycle, the  stimulation effect weakens. The signal fluctuates around the  VOH level. Next, we maintain the duty cycle at 0.5 and  evaluate the signal response to 3 different modulation  frequencies of 2 kHz, 5 kHz and 10 kHz. From the results as


Figure 7: Output pin waveforms for selected fail test cycles  of interest under varying modulation frequency.


Figure 8: Output pin waveforms for selected fail test cycles


44144


ebi2_s_d_0


1740


ebi2_lcd_cs_nebi2_Icden_w_nebi2_cs_n_1ebi2_lb_nebi2_lcdrs_adv_nebi2_a_d_3ebi2_mem_clk


ebi2_a_s_0ebi2_lcd_cs_nebi2_lcden_w_nebi2_cs_n_1ebi2_lb_nebi2_lccirs_adv_nebi2_a_c_3ebi2_mem_clk


ebi2_a_d_D


ebi2_lcden_w_


ebi2_lod_cs_nnebi2_cs_n_1ebi2_lb_nebi2_lodrs_adv_nebi2_a_d_3ebi2_mem_clk


of interest under varying PW at 2 kHz.


1741


1742


sous PW pulsed-laser


1744


1748


1746


1747


1749


btcbtt工


1751


cw lasr


Cycles。71568


71573


71577


1755


1754


1753


1752


1752 1751


1750


1745


1743


1756


Figure 9: Output pin waveforms from pulsed and cw laser


1758


1757


stimulations  for selected fail test cycles of interest.


1759


shown in Fig. 7, it can be concluded that frequency of laser  modulation is not critical. Further experimental results as  shown in Fig. 8 substantiate the finding that duty cycle is the  critical parameter. The modulation frequency is fixed at 2 kHz  while the PW increases. Similar to results obtained from 10  kHz, as PW approaches cw condition, the stimulation power  weakens.


Finally, a strong signal X as indicated in Fig. 2(c), which  exists in both cw and pulsed-LADA, is analyzed for  completeness and results are presented in Fig. 9. The same  output pin is evaluated between test cycles 71568 and 71577. Although the cw laser beam is able to induce a failure after  cycle 71570, it is as stable compared to pulsed laser beam. These experimental results clearly reveal that pulsed laser  beam can affect LADA phenomenon. These enhancements  establish the foundation for EeLADA development which will  be discussed next.


Electrically-Enhanced LADA Concept


Intrinsically, a conventional LADA signal represents the  location of a circuit whose performance is altered sufficiently


2 kHz/ 250μs PW


to flip the test state, regardless of the fail cycles and pins. As a  result, in some cases, besides the critical circuitry of interest, there could be other signals- either from ‘healthy’ transistors


5 kH:/100sPW


with low threshold that are stimulated or there could be more  than one speed path circuitries within the test coverage. We  refer to such signals as LADA artifacts because they are not


10 khz/ 50s PW


related to the failure signature of the fail die under analysis. Figure 10 shows excerpts of error maps which illustrate the


failure signatures in the form of a two-dimensional matrix of  test cycle against failure pin names corresponding to three  different random logic regions stimulated under spot mode. This shows that it is possible to induce LADA signals


250μs PWpulsed-lasr


representing different failure signatures observed on test.


EeLADA technique is able to assess the criticality of all


375μs FN puled-lasr


LADA signals and sift out the relevant signals. There are two


pre-requisites: a) high laser stimulation ability and b) prior  knowledge of failure signature. The former can be fulfilled by  adopting pulsed-LADA and the latter can be obtained from a


typical tester fail log belonging to the fail device.


00μsPW pulsed-laer


Cycles


1760


Figure 10: Excerpt of error maps showing the unique failure  signatures that arise from laser stimulation at three random  logic locations.


Diagnostic Resolution Enhancement


Intuitively, the selection procedure of EeLADA has the ability  to reduce the number of artifacts to reveal only the critical  LADA signals; in other words, it enhances the diagnostic  resolution. We demonstrate this experimentally.


The first test case is a soft MBIST fail at high voltage  minimum (Vmin). The fail log is collected. Cw-LADA is  compared against pulsed-LADA and EeLADA using the  MBIST test pattern and 5X objective lens at 450 mW laser  fiber output power. The pulse frequency is 10 kHz and PW  equals 50 s. The test is set at the margin of passing window


100m


and the entire die is characterized. Figure 12(a) and 12(b) show the signals from cw and pulsed-LADA. Only the  memory signals can be observed from cw laser beam  stimulation. However, two different groups of logic signals are  present in the case of pulsed-LADA. After EeLADA  application, from the results as shown in Fig. 12(c), only the  memory cells and one group of logic signals remain matched  to the soft failure signature. Fig. 12(d) shows the EeLADA  signal overlay to reflected laser image.


The second test case is a simple illustration of the diagnostic  resolution improvement that can be expected from EeLADA. Using the same modulated laser beam conditions, a good  device is characterized on pulsed-LADA and EeLADA on a  logic test pattern using 20X objective lens. Figure 13(a) shows


one of the pulsed LADA signal and Fig. 13(b) shows the  signal to reflected laser overlay image. The laser beam is then  fixed using spot mode at the edge of the signal spot and the  failure signature corresponding to the laser stimulus is  recorded for EeLADA application. Following EeLADA, it is  found that the signal reduces as shown in Fig. 13(c).  This  proves that pulsed-LADA signal comprises of different fail  signatures and EeLADA is able to filter the artifacts.


Figure 12: (a) cw-LADA, (b) pulsed-LADA and (c) EeLADA  signal images acquired using 5X objective. (d) EeLADA


signal overlay to reflected laser image.


Figure 13: (a) pulsed-LADA and (c) EeLADA signal images  acquired using 20X objective. (b) pulsed-LADA signal


overlay to reflected laser image.


Application to Hard Defect Isolation


EeLADA also has the potential for hard defect localization  and we performed a simple experiment as a proof of concept. A programmed defect (PD) is created on a known good die  using 1340nm cw laser at a designated logic region. The die is  verified to fail hard on scan logic testing and the error log  acquired as reference failure signature. In a previous report, we demonstrate the feasibility of obtaining EeLADA signal  corresponding to the exact PD location based on the most  stringent comparison scheme. In this experiment, we make use  of a subset of the original failure signature and found  EeLADA signals to be within 10 m of the expected PD  location. Figure 14(a) and Fig. 14(b) show EeLADA signal  overlay to reflected laser image based on two different  reduced comparison schemes. The black dot indicates the  location of PD and the yellow arrow points to the EeLADA  signal. This result shows that it is possible to simplify the  comparison complexity and obtain reasonable signals close to  the defect for physical failure analysis. In practice, we have  also experienced that it is easier to obtain signals under a  reduced comparison scheme.


Figure 14(a)(b): EeLADA signal s acquired using two


different reference fail log overlay to reflected laser image


Limitations of EeLADA


Test Resolution determines Diagnostic Resolution


The precision of EeLADA in localizing critical circuits  depends entirely on the uniqueness of the failure signature  upon a successful laser stimulus. A very good example is  memory testing using a BIST engine architecture. Every  memory cell within an array will give rise to the same test  response when it fails. Although the response varies for  different memory arrays, the diagnosis resolution is array level  at best. We have experienced worse cases where the test  response is similar for all embedded memories within an IP  block. In contrary, should memory cells be tested using direct  access test method, in other words, the tester is able to address  every single bit of memory; the possibility for a cell-level  diagnosis is higher. Therefore, the precision of EeLADA is  limited by chip design, hence test resolution.


Effect of Optical Resolution


Although the last test case demonstrates the potential of  EeLADA on hard logic defects localization, in practice, it is


observed that the most stringent match condition is  challenging to yield a signal spot. A simple experiment is  performed by fixing the pulsed laser beam on a spot and  collecting fail signatures for 60 loops. We show an excerpt of  the results from the 50th to 56th loops in Fig. 15. It is evident  that the failure signature at the 50th loop is a subset of the  response in all the loops. This experiment uses a high  resolution 50X objective lens with an NA of 0.6. One probable  explanation is the larger laser spot diameter with respect to the  device transistor dimensions at 28 nm process technology. Based on experience, this observation does not happen in an  MBIST test. This is because it is limited by test resolution  instead of optical resolution. A memory array size is definitely  larger than the laser spot size. For cases limited by optical  resolution, like in some logic analysis, the other less stringent  matching schemes as described earlier become useful. More  experimentation is in progress to characterize using a solid  immersion lens and different pulse laser modulations.


Figure 15: Excerpt of a fail log file acquired using pulsedLADA point scan on a random logic.


In this work, pulsed-LADA implemented using a TTL  modulated laser at low frequency is explored. The presented  results suggest that custom cw-LADA could be limited soon. The inferiority of cw to pulsed laser beam stimulation is  manifested as missing signals in the former. It is found that a  TTL modulated laser with less than 0.9 duty cycle and greater  than 1 kHz is sufficient to experience enhancements and does  not require much modifications to a typical laser scanning  microscopy tool. These enhancements can be explained by the  different stimulation effect between a cw and pulsed beam. Further enhancements can be achieved by reducing the PW  using mode-locked lasers to provide higher peak power for


stimulation. Following pulsed-LADA, we develop a new  derivative of LADA technique called EeLADA. EeLADA  significantly improves the quality of signal image by ‘filtering’ only signals relevant to the failure mode by  analyzing the electrical test response from the output pins. This enhancement is demonstrated experimentally on soft  memory failures. We also present, as a proof of concept, on  the application of EeLADA on a good device for hard failures  defect localization using programmed defects. It offers new  dimension to explore LADA-based techniques. Finally, we  discuss briefly on the impact of test and optical resolution  constraints in the application of EeLADA.


[1] M Bruce et al., “Soft Defect Localization (SDL) on ICs,” Proc Int Symp for Testing and Failure Analysis, 2002, pp. 21-27.


[2] C Burmer, C Brillert, ZL Qian, “Soft Defects: Challenge  and Chance for Failure Analysis,” Proc Int Symp for  Physical and Failure Analysis 2007, pp. 235-239.


[3] S Lee, K Kim, Y Lee, E Lee, Y Kim, I Kapilevich, “Marginal Failure Diagnosed with LADA: Case Studies”, Proc Int Symp for Testing and Failure Analysis, 2014, pp.


367.


[4] AM Glowacki, SK Brahma, H Suzuki, C Boit, “Systematic characterization of integrated circuit standard  components as stimulated by scanning laser beam”,  Device and Materials Reliability, IEEE Transactions, 7(1), 2007, pp. 31-49.


[5] A Sarafianos, R Llido, JM Dutertre, O Gagliano, V  Serradeil, M Lisart, D Lewis, “Building the electrical  model of the Photoelectric Laser Stimulation of a PMOS  transistor in 90nm technology”, Microelectronics  Reliability, 52(9), 2012, pp. 2035-2038.


[6] A Sarafianos, R Llido, JM Dutertre, O Gagliano, V  Serradeil, M Lisart, D Lewis, “Building the electrical  model of the Photoelectric Laser Stimulation of a NMOS  transistor in 90nm technology”, Proc Int Symp for Testing  and Failure Analysis, 2012, pp. 143-150.


[7] T Kiyan, C Brillert, C Boit, “Timing analysis of scan  design integrated circuits using stimulation by an infrared  diode laser in externally triggered pulsing condition”,  Microelectronics Reliability, 48(8), 2008, pp. 1327-1332.


[8] V Pouget, P Fouillat, D Lewis, H Lapuyade, L Sarger, FM Roche, R Ecoffet, “An overview of the applications  of a pulsed laser system for SEU testing”, IEEE ioltw, 2000, pp. 52.


[9] Douin, A., Pouget, V., Darracq, F., Lewis, D., Fouillat, P., & Perdu, P. (2006). Influence of laser pulse duration in  single event upset testing. IEEE transactions on nuclear  science, 53(4), 1799-1805.


[10] A Sarafianos, O Gagliano, V Serradeil, M Lisart, JM  Dutertre, A Tria, “Building the electrical model of the  pulsed photoelectric laser stimulation of an NMOS  transistor in 90nm technology”, Int Rel Phy Symp, 2012


[11] K Eringon, J Asquith, D Bodoh, “Software enhanced time  resolved laser assisted device alteration with a non-pulsed


laser source”, Proc 35th Int’l Symp for Testing and  Failure Analysis, November 2009, pp. 43.


[12] D Bodoh, K Erington, “Improving the DLS Workflow”, Proc 38th Int’l Symp for Testing and Failure Analysis, November 2012, pp. 183.


[13] D Bodoh, K Erington, K Dickson, “Root Cause Analysis  Techniques Using Picosecond Time Resolved LADA”, Proc 40th Int’l Symp for Testing and Failure Analysis, November 2014, pp. 82–86.


[14] MR Bruce et al., “Soft defect localization (SDL) in  integrated circuits using laser scanning microscopy”, Lasers and Electro-Optics Society, 2003. LEOS 2003. The 16th Annual Meeting of the IEEE, Vol 2, pg 662- 663, 2003.


[15] ZL Qian, C Brillert, Burmer C, Y Yokoyama, “Differential and lockin imaging of dynamic photon  emission and applications in failure analysis”, Proc Int’l  Symp for Testing and Failure Analysis, 2010, pp. 373- 377.


[16] SH Goh, WY Lau, BL Yeoh, HW Ho, GF You, Hu Hao, Jeffrey L, “Debugging Phase-Locked Loop Failures in  Integrated Circuit Products”, Proc Int’l Symp for Testing  and Failure Analysis . 2014, pp. 465.


[17] SH Goh et al., “Effectiveness of frequency mapping on  28nm device broken scan chain failures”, Rev Sci  Instrum, Vol 83, Issue 2, 023702, 2012.


[18] SH Goh et al. "An effective broken scan chain diagnosis  flow combining software and hardware solutions for  systematic failures." Proc Int Symp on the Physical and  Failure Analysis of Integrated Circuits (IPFA), 2012.


[19] VK Ravikumar, R Wampler, MY Ho, J Christensen, SL  Phoa, “Laser voltage probing in failure analysis of  advanced integrated circuits on SOI” Proc Int Symp for  Testing and Failure Analysis, 2012, pp. 1.


[20] KA Serrels, N Leslie, TR Lundquist, P Vedagarbha, “Two  Photon-Absorption-Enhanced Laser Assisted Device  Alteration and Single-Event Upsets in 28nm Silicon  Integrated Circuits”, Proc 39th Int’l Symp for Testing and  Failure Analysis, November 2013, pp. 173-181.


[21] SH Goh et al., “Evolution of Wafer Level Tester-Based  Diagnostic System: More Than Just a Dynamic Electrical  Fault Isolation Tool”, Proc Int Symp for Testing and  Failure Analysis, 2013.


Laser Logic State Imaging Using Transient Voltage Collapse Circuits


Gwanghyeon Baek1, John Keane2 and Martin von Haartman1


1Low Yield Analysis, Logic Technology Development, Intel Corporation, Hillsboro, Oregon, United States  2Advanced Design, Logic Technology Development, Intel Corporation, Hillsboro, Oregon, United States


gwang.hyeon.baek@intel.com


A laser based logic state imaging (LLSI) by activating  transient voltage collapse (TVC) circuits of SRAM blocks is  demonstrated. In order to induce a voltage modulation on a  power rail, significant numbers of TVC units are activated. The image quality of LLSI strongly depends on a number of  activated TVC circuits. From this experiment, it is concluded  that an additional circuit or experimental setup is not  necessary for LLSI.


electron density  modulation


Vcc(AC)


惬←Laser斋


off


Logic state imaging (LSI) of operating devices  using infra-red


L


Modulation


(IR) emission, which is also known as infra-red emission


offH


offH*


microscopy (IREM), has been one of the most critical  techniques of fault isolation and failure analysis. The quality


个


个个


of IR based LSI (IR-LSI) images strongly depends on both the  operating voltage (Vcc) and an off-state leakage current


flowing through the transistors. [1] With continuous device  scaling, the features size of transistors is becoming smaller  and its operating voltage is decreasing in order to not increase  the electrical field applied on the transistors and also to reduce


Vcc(ac)


the power consumption. For instance, Intel’s state of arts  process technology, as of the year 2015, in mass production


Vcc(DC)


uses the feature size of ~ 14 nm and its operating voltage is


time


smaller than 1 V. Furthermore, the introduction of the tri-gate (or FinFET) device delivered superior immunity on short


channel effects and suppression in a leakage current, relative  to bulk planar devices. [2]


Unfortunately, with these advanced process technologies, the  IR-LSI signal has become very weak, leading to a poor signalto-noise ratio in the collected IR-LSI data. Furthermore, the  spatial resolution of IR-LSI is limited by the broadband nature  of the photon emission process inside of silicon. Therefore, fault isolation using IR-LSI is becoming increasingly difficult  with device scaling. In order to overcome these challenges of  the IR-LSI technique, a laser-based LSI (LLSI) technique has  been proposed. [3]


Laser Logic State Imaging


The LLSI technique is based on modulating the internal power  rail, which is supplying Vcc on a device under test (DUT). Figures 1(a) and (b) explain LLSI of simple inverter circuits. These inverters are frozen at a particular logic state (frozen at  output logic states: (a)high / (b)low). Vcc is then modulated, Vcc(AC), by about 100~200 mV as drawn in Figure 1(c).


Figure 1: laser logic state imaging; (a) output high (b) output  low (c) AC modulation on VCC rail


When the output logic state is High, the PMOS transistor is in  a saturation regime while the NMOS transistor is off-state. The modulating Vcc will change the electron density in the  channel of the PMOS, which will cause a modulation in the  intensity of the reflected laser beam. In the case of logic state  Low, the gate voltage of NMOS is modulated by the previous  inverter, whereas PMOS is off-state. Consequently, the  intensity of the reflected laser is modulating in the NMOS area. We expect to distinguish the different logic states from the


modulation of the reflected laser. The spatial resolution of  LLSI is predominantly related to the wavelength of laser, not  the photon emission process. [4] Hence, the spatial resolution  could be enhanced by choosing a short-wavelength laser.


It is worthwhile to compare with IR-LSI signatures. NMOS  shows IR-emission when the output is high due to the voltage  applied in between the source and drain that accelerates the  carriers. Similarly, PMOS has IR-emission when the output is  low. [5] Therefore, we can assume that LLSI and IR-LSI have  inverted images for the same logic state. These comparisons  are summarized in Table 1. As shown, both NMOS and  PMOS give exclusive signals for different logic states, allowing the logic states of the inverters to be correctly  determined.


Table 1: Comparison: IR-LSI vs LLSI


|Logic State |IR-LSI (IREM) |LLSI |
|---|---|---|

|Output High |Emission on NMOS |Laser beam modulation on PMOS |

|Output Low |Emission on PMOS |Laser beam modulation on NMOS |

There have been several methods published to introduce AC  modulated Vcc:


1.


AC Power Supply with accurate voltage control


2.


On Package Droop Inducer (OPDI) [6]


3.


On Die Droop Inducer (ODDI) [3]


These three approaches all require an additional debug setup. For example, AC power supply and OPDI methods require a


Vcc,SRAM


specialized packaging to minimize a decoupling capacitor. Moreover, an additional circuit design is required for both  OPDI and ODDI methods. In this paper, we propose utilizing  a transient-voltage-collapse (TVC) circuit to induce Vcc


Programmable


Vcc,cell


modulation instead. Since modern SOC or CPU products are


Pulse Generation


SRAM


already integrated with TVC in their SRAM blocks, we expect


Circuit


array


no additional circuit or debug setup will be required.


↓


Figure 2: Six-transistors SRAM architecture


Transient Voltage Collapse Circuit


Supply-voltage (Vcc) scaling or reduction has been a key  approach to achieve low-power SOCs or CPUs. However, voltage-scaling in SRAM is challenging because the read, write, and hold stability of SRAM are influenced by increased  voltage variations at lowered Vcc. The transient voltage  collapse (TVC) technique has been introduced for modern  SRAM architecture to achieve low-voltage operation and high  density SRAM cell. [6]


Reducing the SRAM cell supply voltage (Vcc,cell) during  write operations has been proposed to reduce competition  between transistors M4 and M6 (or M2 and M1) in 6-transistor SRAM structures (Figure 2). In order to achieve  secure write-ability, M2 and M4 should be weaker than M1  and M6, respectively. Lowering Vcc,cell below the threshold  voltage of M2 and M4 makes these transistors completely  off/weak. Consequently, the write-stability becomes less  sensitive to the process variation and/or Vcc variation at low  Vcc. Therefore, the TVC circuit is directly connected to  Vcc,cell and briefly collapses the Vcc,cell near 0 V during  write operation. This idea is widely adapted in modern SOCs  or CPUs, which are currently available on the market.


Figure 3 shows a circuit diagram of the TVC circuit which  generates a transient Vcc,cell droop with varying durations  through a programmable pulse generator. Oscilloscope  waveforms of the programmable pulse generator are captured  in Figure 4.


TVC


Figure 3: Schematic diagram of transient voltage collapse


WL


(TVC) circuit


M20


M4


M1


M6


The purpose of TVC is basically the same as that of the droop


nO


n1


inducers, as noted in the previous section. The only difference


is that TVC is only designed to induce a local Vcc droop on a


BL


M3


M5BL


few numbers of SRAM cells (Vcc,cell), rather than an entire


文支▽:Cn1


Vcc power rail. However, if large numbers of TVCs operate at  the same time, the locally induced Vcc droop would propagate  into a Vcc rail, but the amplitude of modulation would be  reduced. The reduced amplitude of the modulation results


from the parasitic resistance between the Vcc,rail and  Vcc,SRAM, and the capacitance of decoupling capacitors. This  situation is illustrated in Figure 5.


In modern SOCs or CPUs, it has been reported that SRAM  blocks occupy around 30 to 50% of the total die area. Moreover, it is expected that SRAM will occupy up to 80 % of


HN


m*..**


.*...29I/O Circuits--


the total die area by the year 2017. [7] Thus, inducing the  drooping on the entire Vcc power rail might be feasible by  activating significant numbers of TVCs at the same time.


D


HDC SRAM可


Fuse


LVC SRAM


BIST


Figure 4: Oscilloscope waveform of programmable pulse


PLL


generator; (blue) shortest pulse mode (purple) longest pulse  mode. The longest pulse is used in this experiment for  maximum Vcc modulation.


HDC SRAM SRAMLVC


Discussion


Figure 6 shows a die micrograph of Intel’s 14 nm test vehicle  with SRAM arrays. The size of the die is about 8,000 µm by  8,000 µm. We have activated TVC circuits in both block 1 and  block 2. One block corresponds to 14 Mega-bit SRAM cells. Logic state images have been taken at the location of “D” in  Figure 6, which is the edge of the circuit block. Figure 7  shows the logic state images of IR-LSI (i.e. IREM) and LaserLSI (LLSI) at “D”. The longest pulse mode in Figure 4 is  selected in this experiment. The silicon solid-immersion-lens (SIL) is used for the imaging, and the laser with 1319 nm  wavelength is used.


As we expected from Table 1, at the logic state Low, PMOS


has an emission in IR-LSI, but NMOS has the intensity  modulation of the reflected laser in LLSI. An opposite  statement holds for the logic state High. From this result, we  can clearly conclude that LLSI using TVCs is a feasible  approach in fault isolation.


Figure 6: Microscopic image of Intel’s 14 nm Test Vehicle (all  TVCs in blocks 1 and 2 are activated for LLSI). Image credit  from the reference [8].One block includes 14 Mb SRAMs.


If the activated TVCs are not enough to modulate the Vcc,rail, we are not able to determine a logic state from collected LLSI. In other words, the image quality of LLSI is strongly  dependent on the number of activated TVC circuits. The LLSI  images depending on different numbers of activated TVCs are  compared in Figure 8. In the case of block-1 activation, the  image degrades as the distance from the activated TVCs  increases (from A to D). This result implies that only VCC rails  near activated TVCs (block-1) is modulating, while the VCC  rail on the chip edge is still in a static state/condition. In  contrast, the image degradation is negligible when the TVCs


Vcc,rail


工UT


VCC,SRAM


占


Vcc,logic


A0,09|


A00'08|


Vcc.cell


saVN


sawIV


saww


eujeK


eueA


eu.eK


70513


LAJ


JUTFUUCNIL


de-cap


Programmable Pulse Generation Circuit


Figure 5: Simultaneously activated large numbers of TVCs induce Vcc,rail modulation, but amplitude of modulation is reduced.


in blocks 1 and 2 are activated. In all locations (A to D), we  were able to collect LLSI images of similar quality.


Figure 7: Collected LLSI image and its comparison to IR-LSI; the collected images are consistent with Table 1.


Figure 8: LLSI images taken from different locations (A, B, C  and D on Figure 6) of the die when TVCs of block-1 or 1&2  are activated.


In this study, we successfully demonstrated laser based logic  state imaging by activating TVCs of SRAM blocks. Since  modern SOCs or CPUs are already integrated with TVC  circuits in its SRAM blocks, the additional circuit or  experimental setup, such as droop inducers or an accurate AC  power supply, is no longer necessary for LLSI. However, since TVC is originally intended for local Vcc drooping, the  simultaneous activation of large numbers of TVCs was  required to modulate the entire Vcc power rail. We confirmed  that the image quality of LLSI depends on the amount of the  activated TVCs. Since the spatial resolution in LLSI is related  to the wavelength of laser, we expect a spatial resolution  enhancement with the choice of a short-wavelength laser.


Acknowledgement


The authors would like to thank Priyanka Gadde from the  advanced design group, Intel, Hillsboro, Oregon for her  assistance in preparing test vectors for activating different  numbers of TVCs.


[1] Bockelman, D. R. et al. “Infrared Emission-Based Static  Logic State Imaging on Advanced Silicon Technologies,” Int’l Symposium for Testing and Failure Analysis, pp. 531-537, 2001


[2] Jan, C.-H. et al. “A 22nm SoC Platform Technology  Featuring 3-D Tri-Gate and High-k/Metal Gate, Optimized  for Ultra Low Power, High Performance and High Density  SoC Applications,” IEEE Int’l Electron Devices Meeting (IEDM), pp. 3.1.1 - 3.1.4, 2012


[3] Baohua Niu et al., “Laser Logic State Imaging (LLSI)” Int’l Symposium for Testing and Failure Analysis, pp. 65, 2014


[4] J. Beutler et al., “Visible Light LVP on Ultra-Thinned  Substrates,” Int’l Symposium for Testing and Failure  Analysis, pp. 110, 2014


[5] Y-C Steven Chen, et al. “Backside Infrared Emission  Microscopy (IREM) Based Silicon Debug Methodology,” Intel Design and Test Technology Conference (DTTC), 2000


[6] Omer Vikinski et al., “Enhancing Circuits and Systems  Supply Noise Sensitivity Characterization Using OnPackage Droop Inducer,” Int’l SoC Design Conference (ISOCC), 2011, pp.397, 400, 17-18 Nov. 2011


[7] Zvi Or-Bach, “The most expensive SRAM in the world –


2.0,” Solid State Technology, 2014


[8] Eric Karl et al., “17.1 A 0.6 V 1.5 GHz 84Mb SRAM  design in 14 nm FinFET CMOS technology,” Solid-State  Circuits Conference - (ISSCC), 2015 IEEE International, pp.1,3, 22-26 Feb. 2015


* Corresponding author: guillaume.bascoul@intraspectechnologies.com Tel : +33 561 28 14 50      Fax : +33 561 27 47 32


Pulsed laser stimulation coupled with optical failure analysis  technique: a methodology to help space application electrical  designers


G. Bascoula*, K. Sanchezb, G. Perezb, F. Bezerrab, H. Chauvinc


a Intraspec Technologies, 4 avenue Didier Daurat, 31400 Toulouse, France


b Centre National d’Etudes Spatiales, 18 avenue Edouard Belin, 31401 Toulouse, France  c Thales Communication and Security, 18 avenue Edouard Belin, 31401 Toulouse, France


Pulsed laser for radiation sensitivity evaluation has become a common tool used in research and industrial  laboratory. This paper aims to highlight an approach to understand weaknesses of a component under radiation  environment using a short pulsed width laser beam coupled to thermography technique, heavy ions test inputs and  physical analysis. This paper is based on a study of a PWM device embedded on voltage converter.


1 Introduction


Pulsed laser stimulations have been used since the  beginning of the 1990s in research laboratories, and then  industry, to evaluate the sensitivity of microelectronics  devices submitted to radiative environment like in space. Under specific properties light radiations are in fact able  to trigger same electrical phenomenon as heavy ion (HI) particles [1], [2] such as single event latch-up (SEL), single event upset (SEU) [3], [4], Single Event Transient (SET), or single event functional interruption (SEFI). Light properties required to induce this phenomenon are  directly linked to the device under test characteristics [5]. Substrate type, doping and thickness are the most  important parameters which determine the laser  properties required [6].


On the other hand, the induced single event effect types  depend on the technology under test. For example CMOS  technology is very susceptible to single event latch-up  because of its own internal structure based on NPN and  PNP doped areas. An incoming energetic particle passing  through such biased structures is able to trigger electrical  phenomenon named latch-up implying a current  overconsumption [7], [8]. If this critical malfunction is  not stopped by removing the power supply, the device  may be subjected to damage [9]. Most of single event  effects are not responsible of physical damage like SEL  but are able to disturb the device functionality  temporarily or for longer time. Susceptibility  characterization of a given device to those effects is an  important work for space application and other field of  activity which need to support radiative environment.


Pulsed laser testing guides the selection of devices and


helps designers to select the appropriate embedded  corrective watchdog or protection system. Pulsed laser  testing is also an important tool for integrated circuit  manufacturers who want to develop and propose radtolerant or rad-hard devices [10], [11]. Heavy ion test sets  the susceptibility as a function of the deposited energy,while laser testing is able to give more information about  physical sensitive area localization and timing behaviour  of sensitive areas from devices [12], [13].


Moreover, since there is neither radioactive risk nor  vacuum chamber necessity, the operating cost and  infrastructure of a pulsed laser installation is much  smaller than an energetic particles accelerator.


The laser also allows a certain flexibility regarding test  board configuration and the possibility to use advanced  device test feature which are not easily transportable to a  particle-beam test laboratory.


2 Methodology


The methodology developed in this paper intends to show  how a study of the device behaviour under pulse laser  stimulation is able to help the design of electronic  systems dedicated to space application.


The study will give relevant elements to electrical  designers in order to optimize the implementation of the  device in their application and assure the reliability of the  complete system for a given space mission profile. Getting a better understanding of potential failure  mechanism involved around a component is mandatory  to be able to find parameters that can be tuned to avoid  the failure.


Origin of the study


The initiative of this study came from tests that have been  done during a heavy ion campaign on 5 PWM (Pulse  Width Modulator) mounted on a voltage converter  prototyping board. Results obtained were very critical  because all components were destroyed during this test, 4 directly after the first event and 1 after a single event  transient (SET).


As shown on the Figure 1 the current/voltage  characteristics (I/V curves) of the output pin for each  defective device has a more or less important resistive  output characteristic with values variation between 108   and 344 .


2E-04--lc(REF)


108 Ohm


lc(U1-2)


344 Ohm


1E-04


-Ic(U1-3)


5E-05


、


1u


1210E+00


REF


EHT=2.00kVVD=4.7mm


2μm


Grand.= 5.54 XXSignalA*SE2


Date:28Aur 2016


Figure 1 – Current/Voltage characteristics between


OUT/GND pins for components failed after heavy ions test. Inset: PWM device test under heavy ions


The goal of the study was first to locate the defect area in  order to understand the occurrence of the destruction  implying such ohmic characteristics. A lock-in  thermography analysis of all chips was done and  resulting by the presence of a defect on one interdigital  output transistor for each device (Figure 2).


2um


EHT =2.00KVWD=3.6mm Grand.= 4.35XX


SignalA= SE2


Date:13 Fev2015


Figure 2 – Thermography imaging of one of defective devices


EHT = 2.00KV


IVD* 3.6mm


Grand.= 4.76XXSignalA*SE2


Date:13 F6v2015


(5X). Inset: Full device image with thermographic spots, only  the bottom one is a defect signature.


The defect has been identified and located on several


devices damaged under heavy ion and under pulsed laser  stimulation. The physical signature of defective parts is  identical after heavy ion and pulsed laser test as  illustrated on the followed SEM images acquired on three  representative cases.


Figure 3 – SEM view of the typical defect observed between


-5E-05


the source and the drain at substrate level of the output  transistor after heavy ion stress.


-1E-04


-2E-04-0,1-0,08-0,06-0,04-0.0200.020,040,060,080,1 Volatge bias between OuT and GND (V)


Figure 4 – SEM view of the typical defect observed between


Figure 5 – SEM view of the typical defect observed between


the source and the drain at substrate level of the output  transistor after pulsed laser stimulation.


On Figure 3 and Figure 4 we can observe a defect at  substrate level induced by heavy ion stress. Previously a  wet deprocessing (dip HF) was done in order to observe  the poly-gate which shows some cracks at the substrate  level. The Figure 5 shows also the defect at substrate  level after pulsed laser stimulation and with the same  delayering steps. Some design signatures due to the shape  of contact at drain/source level can be seen but with no  significant impact on the whole melting zone including  the channel.


According to these results the typical defect signature is  a drain / source short circuit propagating through the  polysilicon gate and the channel causing a melting of  contacts.


From the electrical point of view, next step is to find the  conditions leading to this destructive phenomenon and to  determine which parameter plays a positive or negative  role.


Different parameters we chose to tune are the spatial and  the temporal location of particle impact on the die, the  biasing conditions and the external electrical  configuration.


3 Experimental setup


The laboratory is equipped with a 1064 nm, 7.9 ps pulsed  laser with a 80 MHz repetition rate. It gives the  possibility to work on integrated circuit based on silicon  by the front side and by the backside through the silicon  substrate. The spot diameter at the focalisation point is  about 5,5 μm diameter with the lower magnification lens  used for this study (2,5X). Smaller spot size can be set by  using à 50X lens, 1μm can be achieved. The pulse  repetition rate can be modulated thanks a pulse picker  module allowing to decrease this rate down to hertz or  single shoot. The laser is embedded on a tuned failure  localisation platform with a confocal laser scanner and a  CCD camera (Meridian LSM from DCG Systems).


4 Experimentation and Results  Pulse laser location dependency


In order to locate the sensitive area able to trigger the  destructive effect on the output transistor several laser  scans of the die were realized on the same setup  previously used for heavy ions test. This step is also  mandatory to adjust the laser energy required to induce  the different effects (SET and failure in this case). A low  repetition rate of 10 KHz maximum has been used for  these experiments in order to avoid cumulative effects; laser pulses can trigger non representative effects  compared to heavy ions impacts if they are too close in  time. This frequency is fastest than a standard flux  applied in radiation chamber (about 1 ion per 10 minutes  on 30μm²) in order to speed up the test and having a better  coverage of the die. Nevertheless the delay between two  consecutive pulses lets the electrical charges and  temperature to be dissipated into the bulk. The scanning  of the die from front-side is achieved starting with low


energy and increasing progressively. First, SET effect  appears on specific areas, then from 500 pJ per pulse the  destructive effect is happening (Figure 6).


Figure 6 - SET snapshot, Blue curve is PWM output when red


colour shows the signal after low pass filter (2ms/div).


The experiment has been reproduced on a tens of parts, then I/V curves analysis shown the same ohmic profile  than heavy ions experiments on the devices output (Figure 7).


Figure 7 – I/V curves traced between OUT/GND pins for  components failed after laser stimulation tests.


All parts became defective during the scanning of the  output MOS transistor where the hot spot is observed  thanks to lock-in thermography imaging on Figure 8. To  verify the destructive effect is well induced by pulsed  laser and not induced by die reliability-loss made by  previous scan, we limit the scan area to this MOS  structure and notice again the failure of the device (Figure  9).


It shows that defect appears exactly at the place where  the laser has been targeted. The opposite experiment has  been done by scanning all the die excluding this MOS  transistor and no destructive effect appears (SET are  observed and responsible areas are identified). This  information is definitively crucial to extract an  occurrence probability of such defect according to the  MOS/die surface ratio (die surface is 3.06 mm² when  MOS surface is 0.3 mm²).


Figure 8 – Thermography image of one component failed  under laser.


PWM Clock In Laser


马


PWM Output Pulse


Figure 9 – Thermography image on the defective MOS


produce by a direct exposition to pulse laser beam of 500 pJ. Inset: Locations of the laser scan area.


Pulse laser temporal dependency


To go further on the investigation, the laser system is able  to synchronize the pulse on the sequence of the device. This allows triggering a pulse only during the given state  of the output MOS transistor. First experiment is setup  for testing MOS off-state: Duty cycle is set to 50%, the  PWM clock period set to 500 KHz, the laser pulse to 1  KHz, laser power set to 500 pJ and only the output MOS  is scanned. The one-shot laser pulse signal  synchronization is assured by the same generator giving  the PWM clock In. Pulse picker driver receives this  signal and commands the pulse-picker opening at the  moment of the laser pulse generation. The minimum  delay of this operation is 12 ns without cable delay.


PWM


Clock In


Pulse


Output


Figure 10 – Screenshot of the behaviour of the output during  off-state stimulation (1μs/div)


As shown on Figure 10, no effect was observed on the  MOS even after 10s of laser stimulation.


The same experiment has been done during the on-state  of the MOS.


Figure 11 - Screenshot of the behaviour of the output during  on-state stimulation (2μs/div)


As shown on Figure 11, the laser pulse immediately trigs  a defective behaviour on the output signal and stops  working after 5 clock periods.


The experiment has been repeated for a lower frequency (clock at 100 KHz) and one-shot laser pulse with the  same result in the end. This implies the duty cycle is one  of key parameters regarding the occurring probability in  time.


Biasing dependency


Experiments shown that the decrease of the voltage on  VCC limits the occurrence of the destructive effect. Indeed no destructive effect was observed for biasing  lower than 10V, some component are destroyed between  10V and 12V after more than 1 laser scan and all parts  are defective other 12V biasing. The nominal biasing  value is 12V according to the datasheet. However the “turn on threshold” of this component is set to 12.5V and  voltage bias higher than 12V is possible for short period  of time.


External electrical configuration dependency


Pulse width modulator devices can be used to command  directly power MOSFET. In this situation a decoupling  capacitor in μF range is recommended on the PWM  supply to quickly bring the energy required for the power  MOSFET switching. During these experiments we have  also covered the influence of decoupling capacitor value: If decoupling capacitor value increases the voltage level  responsible of the defect decreases. Safe operating area  is identified with voltage level lower or equal to 10V and  decoupling capacitor at 1μF maximum (when decoupling


capacitor value increases safe operating voltage  decreases). However, once destructive effect is activated  the external electrical configuration will also change the  profile of the ohmic characteristic, bringing more or less  energy to the defect according to the size and the position  of external capacitors.


5 Discussion


All results obtained following different experiments  achieved on the chip incriminate a weakness in the output  MOS transistor. According to the size ratio of this output  MOS compared to the whole die surface, 7.5% of the  surface can be sensitive to destructive effect under heavy  ion strike (die surface is 3.06mm² and MOS surface is


0.3mm²). Moreover, such component works in a nominal  configuration with a duty cycle between 15% and 25%. Therefore, the probability damaging the chip is relatively  low considering the temporal aspect (Destructive  phenomena appear only when output is at high level).


Experiments confirm that decreasing voltage polarization  allows protecting the device against destruction; however  the susceptibility regarding SET is increasing with low  voltage.


The SET aspect has also been studied by making  sensitivity cartography as shown on Figure 12. An  important area of the die is susceptible to induce these  temporal interruption phenomena that decrease the  availability of the component along the mission. This  information can be very relevant according to the mission  profile.


6 Conclusion


In this paper, we have demonstrated that we can use a  localisation tool dedicated to microelectronic failure  analysis in order to highlight weaknesses of a device  embedded in space application. This analysis step  reinforces knowledge of the component behaviour to  adapt the electrical designs according to the mission  profile (orbit constraints, time of availability of the  application …). If this component is selected for space  application in spite of knowing potential weaknesses, electrical designers need to take into account the  consideration exposed by preliminary heavy ions and  pulsed laser test. Otherwise specific heavy ion test in the  final architecture is recommended.


As shown in this paper pulsed laser tests can be  advantageously integrated in the heavy ion robustness  flow for dedicated devices or COTS evaluation. Fine  electrical parameters affecting sensitivity to heavy ions  can be identified and characterised. By taking into  account those parameters a more accurate probability of  events in flight can be evaluated.


Figure 12 – Sensitivity cartography of SET by pulsed laser


7 Acknowledgments


The authors would like to thanks Antoine Reverdy from  Sector technologies for his help on the development of  the pulsed laser tool used along this study.


8 References


[1] A. H. Johnston, “Charge generation and  collection in p-n junctions excited with pulsed  infrared lasers,” IEEE Transactions on Nuclear  Science, vol. 40, no. 6, pp. 1694–1702, 1993.


[2] S. C. Moss, S. D. LaLumondiere, J. R. Scarpulla, K. P. MacWilliams, W. R. Crain, and R. Koga, “Correlation of picosecond laser-induced latchup  and energetic particle-induced latchup in CMOS  test structures,” IEEE Transactions on Nuclear  Science, vol. 42, no. 6, pp. 1948–1956, 1995.


[3] S. Buchner, K. Kang, W. J. Stapor, A. B. Campbell, A. R. Knudson, P. McDonald, and S. Rivet, “Pulsed laser-induced SEU in integrated  circuits: a practical method for hardness  assurance testing,” IEEE Transactions on  Nuclear Science, vol. 37, no. 6, pp. 1825–1831,


1990.


[4] A. H. Johnston and M. P. Baze, “Experimental  Methods for Determining Latchup Paths in  Integrated Circuits,” IEEE Transactions on  Nuclear Science, vol. 32, no. 6, pp. 4260–4265,


1985.


[5] E. Faraud, V. Pouget, K. Shao, C. Larue, F. Darracq, D. Lewis, A. Samaras, F. Bezerra, E. Lorfevre, and R. Ecoffet, “Investigation on the  SEL Sensitive Depth of an SRAM Using Linear  and Two-Photon Absorption Laser Testing,” IEEE Transactions on Nuclear Science, vol. 58, no. 6, pp. 2637–2643, Dec. 2011.


[6] J. S. Melinger, S. Buchner, D. McMorrow, W. J. Stapor, T. R. Weatherford, A. B. Campbell, and  H. Eisen, “Critical evaluation of the pulsed laser  method for single event effects testing and  fundamental studies,” IEEE Transactions on  Nuclear Science, vol. 41, no. 6, pp. 2574–2584, Dec. 1994.


[7] R. R. Troutman, Latchup in CMOS Technology: The Problem and Its Cure. Springer, 1986, p.


242.


[8] N. A. Dodds, N. C. Hooten, R. A. Reed, R. D. Schrimpf, J. H. Warner, N. J.-H. Roche, D. McMorrow, S. Buchner, S. Jordan, J. A. Pellish, N. J. Gaspard, and M. P. King, “SEL-Sensitive  Area Mapping and the Effects of Reflection and  Diffraction From Metal Lines on Laser SEE  Testing,” IEEE Transactions on Nuclear  Science, vol. 60, no. 4, pp. 2550–2558, Aug.


2013.


[9] Y. Moreau, H. de la Rochette, G. Bruguier, J. Gasiot, F. Pelanchon, C. Sudre, and R. Ecoffet, “The latchup risk of CMOS-technology in  space,” IEEE Transactions on Nuclear Science, vol. 40, no. 6, pp. 1831–1837, 1993.


[10] D. McMorrow, J. S. Melinger, S. Buchner, T. Scott, R. D. Brown, and N. F. Haddad, “Application of a pulsed laser for evaluation and  optimization of SEU-hard designs [CMOS],” IEEE Transactions on Nuclear Science, vol. 47, no. 3, pp. 559–565, Jun. 2000.


[11] D. Mcmorrow, S. Buchner, M. Baze, B. Bartholet, R. Katz, M. O’Bryan, C. Poivey, K. A. Label, R. Ladbury, M. Maher, and F. W. Sexton, “Laser-Induced Latchup Screening and  Mitigation in CMOS Devices,” IEEE  Transactions on Nuclear Science, vol. 53, no. 4, pp. 1819–1824, Aug. 2006.


[12] J. Ferrigno, R. Desplats, P. Perdu, K. Sanchez, F. Beaudoin, and D. Lewis, “Dynamic Optical  Techniques for IC Debug and Failure Analysis,” in 13th International Symposium on the Physical  and Failure Analysis of Integrated Circuits, 2006, pp. 320–326.


[13] K. Sanchez, P. Perdu, K. Melendez, and T. Nakamura, “Comparison of C.W. Electro Optical  Probing and Light Emission Techniques,” ISTFA  2013: Conference Proceedings from the 39th  International Symposium for Testing and Failure  Analysis (ASM International), pp. 329 – 335,


Soft defect Localization on Analog and Mixed-signal ICs Using an OBIRCH Tool


Chunlei Wu1, Xiaocui Li2, Yi Che2


1Analog and Sonser Group, Freescale Semiconductor (China) Limited, Tianjin 300385, China  2Product Analysis Laboratory, Freescale Semiconductor (China) Limited, Tianjin 300385, China  Tel: +86-159-2212-7484, E-mail: b09059@freescale.com


It is difficult to localize the soft defect on analog and mixedsignal ICs only by OBIRCH, because OBIRCH laser scanning  module could not synchronize with the IC under functional  test, and the failure modes on analog and mixed-signal ICs are  complicated. In this paper, a dynamic synchronization method  is proposed to localize the soft defect precisely only with an  OBIRCH tool on analog and mixed-signal ICs. The  methodology and system configuration are presented. A case is  studied successfully on an analog and mixed-signal IC using  this method.


More and more functional failure cases are induced by the soft  defects along with more and more advanced semiconductor  technology. Soft defects have been one of the most difficult  types of defects to isolate, as they are often subtle and "nonvisual" in nature. Generally, they can’t be detected by ordinary  defect localization techniques, such as Photon emission  microscopy (PEM [1]). In this case, the dynamic thermal laser  stimulation (D-TLS) techniques can localize them effectively. The D-TLS techniques include Resistive Interconnect  Localization (RIL) [2], Soft Defect Localization (SDL) [3] and  Delay Variation Mapping (DVM) [4] et al. As one of the DTLS techniques, SDL is a method that directly locates the soft  defects from the front side and backside of ICs. Information  about the SDL technique was first published and presented at  ISTFA in 2002 by M.R. Bruce et al. Their paper introduced  the concept that as a laser scans across a die pixel by pixel, the  localized heat changes the pass/fail state of an electrical test  result to identify a soft defect’s physical location on the die. Only the D-TLS technique can be performed to do that.


In fact, not all failure analysis (FA) laboratories have a normal  SDL equipment to localize soft defects but the OBIRCH [5] tool is employed generally in many laboratories. In our FA  laboratory, there is no normal SDL equipment but only an  OBIRCH tool. Generally, OBIRCH, as a Static Thermal Laser  Stimulation (S-TLS) technique, is used for detecting parameter  failures on failing ICs that are under a static state without  running any dynamic function. The OBIRCH tool does not  detect soft defects directly as it could not synchronize with an  IC under test.


In this paper, a dynamic synchronization method is presented  to realize soft defect localization only with an OBIRCH tool  on analog and mixed-signal ICs. It can dynamically  synchronize the IC under test to the laser scanning module of  OBIRCH. It is a new and low-cost way to achieve SDL  technique only by OBIRCH equipment and localize soft  defects precisely if there is no normal SDL equipment on hand  but OBIRCH equipment on hand. The methodology will be  elaborated and a case is studied successfully on an analog and  mixed-signal IC using this method.


The dynamic synchronization method on analog


and mixed-signal ICs


Generally, a soft defect is sensitive to temperature which  results in the pass/fail test result also depending on the  temperature. OBIRCH monitors the current variation while the  laser was heating every pixel of the circuit. The effect of laser  heating when performing OBIRCH could change the test result  from either a failing state to a passing state or vice versa by  heating the whole die pixel by pixel. For pinpointing the  position of the soft defect precisely, the key is how to  synchronize the dynamic IC under test to the OBIRCH laser  scanning module. However, OBIRCH does not have this kind  of synchronization capability to do that. For resolving this  issue, a dynamic synchronization method is proposed: given  the worst condition, the smallest pixel dwell time (PDT) of  laser should be twice as much as the test period. The whole  test period includes the time of test result identification and the  time of the pass/fail flag. This is a guarantee that the failing IC  is tested at least once while the laser is heating a pixel  regardless of the start time of a new test period. A valid pass or  fail result is determined at least once for each pixel. This also  insures that the SDL mark on the die image is just at the right  site of the soft defect. Figure 1 shows the sketch of SDL  system and the operating process is demonstrated in the  flowing.


Figure 1: The sketch of SDL system.


In the whole testing process the OBIRCH amplifier forces a  constant DC voltage (5V) at the “BIAS” port, and a 20KΩ  resistance is in series between the “BIAS” port and the test  result flag port for limiting the current in an appropriate scope. When the laser is located over the failing location, the heat  from the laser changes the test result either from a failing state  to a passing state or vice versa. Therefore, at each pixel  location the OBIRCH amplifier receives a digital pass/fail flag  from the test result flag port of the IC test system. If a pass flag  is assigned a digital value of “1” (5V) and a fail flag is  assigned the digital value “0” (0V), the OBIRCH signal should  mark the pixel dark (green in its overlay image) if the test  result is pass, as the current in the 20KΩ resistance decreases, and mark the pixel bright (red in its overlay image) if the test  result is fail, as the current in the 20KΩ resistance increases. So the location of the soft defect is located precisely by the  bright (red) mark (spot) as long as the smallest PDT is twice as  much as the test period. The mark result is vice versa if the  pass and fail digital assignments are reversed.


For the analog and mixed-signal ICs, it is hard to program a  pass/fail flag for revealing the state of the test result as there is  no CPU module in the analog and mixed-signal ICs. Generally, their failure modes are not digital and various, such  as pulse width failure, voltage amplitude (current) failure, delay time failure, and so on. Thus, the variation of the test  result under laser heating is not digital, too, and it could not be  forced into the OBIRCH amplifier directly as the case for a  digital IC. It is difficult to detect the variation of the test result  directly by the OBIRCH. However, all these variations of test  results on analog and mixed-signal ICs could be transformed  to a digital pass/fail flag through a signal processing system  which only includes an oscilloscope and a function generator. Figure 2 shows the sketch of SDL system for the analog and  mixed-signal ICs, and the operating process is demonstrated in  the flowing.


Analog failure signals input


Figure 2: The sketch of SDL system configuration on the


GND.


analog and mixed-signal ICs.


There are many trigger modes in an oscilloscope. They could  be used for detecting the variations of analog and mixed-signal  failure signals. Once the variation matches a trigger threshold  condition of the oscilloscope, the waveform is captured in a “normal/single” mode. Simultaneously, a rising edge is output  via the “Trigger Out Port” (usually in rear panel) of the  oscilloscope. However, the rising edge is not suitable as a  pass/fail flag because a pass/fail flag is time limited , thus, a  function generator triggered by the rising edge is employed to  produce a time limited pass/fail flag. The function generator is  able to output a programmable pulse with a special definition (voltage amplitude and time width). The time of pulse width  and test result identification should also match the requirement  of the dynamic synchronization method.


As Figure 2 shows, the OBIRCH system is applied to detect  the pass/fail flag by sending the flag to the “BIAS” port of the  OBIRCH amplifier. The current through the 20 kΩ resistance  is changed due to the variation of the pass/fail flag, given a  constant DC voltage is set by the OBIRCH amplifier through  the “BIAS” port. For example, the OBIRCH amplifier outputs  5V via the “BIAS” port. The function generator outputs 5V  signifying a “pass” flag and 0V with 20µs pulse width  signifying a fail flag.


Case study


This analog and mixed signal IC is a 4 channels DSI bus IC. The functional failure mode for this IC was: the DSI bus  signals of the channel 0 (D0H and D0L) were normal at 25°C, but they were abnormal at 115°C (Figure 3). Thus, it is the soft  defect resulted in the failure, because the failure mode was  temperature dependent.


Function Generator


Laser scan


"pass/fail" flag-OBIRCH


-


OBIRCH Amplifier


20KO


7r


8les


--


PFPOutput a pass/fail flag


一


Test result


Defect,I/O portww+


+AI,


Amplifier.OBIRCHID


Imaging system.--


↑


古failure modes


variation of the analog


GND


threshold to capture the


Set the trigger event


I-


Oscilloscope


BIAS.


PFP.


rigger signal


IC test system


Figure 3: The failure mode at 115°C.


OBIRCH was tried to employ to locate the soft defect using  the dynamic synchronization method proposed in this paper. First, we studied how to convert the abnormal variation of  D0H/D0L signal to a digital pass/fail flag. The normal pulse  width time of D0L was 129µs at 25°C if the high level voltage  threshold was set to 8V, but it decreased dramatically along  with the temperature raising. There was no pulse higher than  8V on D0L signal finally when the temperature reached to  115°C. Thus, the “pulse width” in an oscilloscope was chosen  as a trigger mode to monitor the abnormal variation of D0L  signal. In the “pulse width” trigger mode, the trigger threshold  condition was that the time of 8V pulse width was less than  125 µs. If the 8V pulse width time on D0L was less than 125 µs, a trigger event happened and a rising edge was output via  the “Trigger Out Port” of the oscilloscope to the Function  Generator, and then the Function Generator output a 20 µs 0V  pulse which represented a digital fail flag to the “Bias” port of  OBIRCH; If the 8V pulse width time on D0L was greater than  125 µs, the trigger event did not happen and no rising edge  was sent to the Function Generator, so the Function Generator  output 5V which represented a digital pass flag to the “Bias” port of OBIRCH. See Figure 4. Thus, the abnormal variation  of D0H/D0L signal was converted to a digital pass/fail flag in  this way. By the way, for converting the pass/fail test result to  the current variation, OBIRCH amplifier output 5V via “Bias” port in the whole test process.


Figure 4: The D0H/D0L signal at 25°C and 110°C. And the


pass/fail flag and trigger signal when D0H/D0L failed.


The D0H/D0L signal period was about 130 µs, and the time of  the pass/fail flag was 20 µs, so the whole test period was about  150 µs. For realizing dynamic synchronization between the  OBIRCH laser scanning module and IC under test, the smallest  PDT of laser should be 300 µs. In this case, 2182 µs PDT was  chosen to do soft defect localization for dynamic  synchronization and enough heating. Figure 5 shows the  experimental result with 200 and 1000 magnification. The  green signal revealed a passing state test result as laser heating  was not at the soft defect location, and the red signal revealed  a failing state test result as laser heating was just at the soft  defect location. Therefore, the red signal pointed out the soft  defect location. Physical analysis revealed a particle just at the  red signal location (Figure 6).So in this case, the soft defect  was a particle.


8V pulse width on D0L was 129µs  at 25°C, Pass


sogree5Skpn


ocing


Ew LimitFne


invers00q


Agilant Technologies


0019 00$


Agilaat Tachnologies


LN0A0 6089180□


8V pulse width on D0L was 112µs


at 110°C, Fail


Trigger signal


LS8=802868Hz


Fail flag “0”


EE


+SourceSlope


Mode


ManualDS008XL


12:-15.1900V


Cursora


122010


Pass flag “1”


Abnormal


THUOCT 3014:21:33 2014


L3N 0A050896N68 01F


D0H


D0L


The Ref IC


The Failed IC


OVY


SAa**5C.


WVUN 200224上0


2]


AX=129.200008


1/AX=7.7399kHz AY21=231900V


Figure 5: The soft defect localization result only using  OBIRCH.


Figure 6: The particle images at the red signal location.


In this paper, a dynamic synchronization method is proposed  to synchronize the dynamic analog and mixed-signal IC under  test to the OBIRCH laser scanning module. The abnormal  variation of the test result on analog and mixed-signal IC can  be converted to a digital pass/fail flag easily through a signal  processing system which only includes an oscilloscope and a  function generator. It is a new and low-cost way to achieve  SDL technique only with an OBIRCH tool and localize soft


defects precisely on analog and mixed-signal ICs, if there is no  normal SDL equipment on hand but OBIRCH equipment on  hand. The experimental result shows the dynamic  synchronization method is an effective way to locate the soft  defect precisely only with an OBIRCH tool.


In this paper, we do not consider the response time of the  oscilloscope and function generator. Generally, the response  time of the oscilloscope and function generator is very short (negligible) compared with the test period of the analog and  mixed-signal IC, so the oscilloscope does not miss the failing  event. However, if the test period is very short in some special  case, the response time of the oscilloscope and function  generator should be considered to make sure every failing  event could be caught.


LVP waveform is a function of the free carrier absorption. More carriers under the laser spot, more the modulation. When  2 PMOS transistors are turned on, they both affect the  modulation which now is twice as much as when only 1  transistor is on. The logic state is 1 as long as any one PMOS  is ON. The modulation however depends on the number of  PMOS that is ON. When both PMOS are ON in a 2-Input  NAND gate, we see a 1+ state where the modulation is at its  maximum


90nmLaser spot size~270nmNMOSLaser spot location on


Figure 4: LVP waveforms from 2-input NAND gate. PMOS  curves on the top and NMOS with inverted logic on the  bottom. The white arrows on the PMOS output waveform  show extra amplitude when both inputs are 0


Another interesting observation is that while it is important  that the laser spot is on both PMOS transistors, it does not  matter whether the transistors are connected in series or in  parallel. This is because the channels are modulated primarily  by the gate and creation of free carriers in the channel region  depend more on the gate voltage than the source/drain.


On the NAND, the NMOS transistors are in series. When  either transistor is OFF, it is essentially an open circuit to  ground. However, we still observe higher amplitude when 1  input is ON at the yellow arrows.  Since the transistors are in  series, this state is in between the minimum and the maximum  amplitude. The minimum state occurs when both transistors  are ON and the maximum when both transistors are OFF.  Note that we denote the minimum as logic 1 as the convention  for NMOS and to correlate the truth table


The physical placement of the laser probe spot affects which  of the inputs modulate the waveform more. In case we have a  large drive NAND gate which is made up of multiple fingers, the user might place the laser on the channel that is being  dominantly controlled by 1 input instead of both. If the laser  spot does not cover the entire active region of the output, the  modulation might be affected accordingly.


2-Input NOR Gate


The 2-input NOR gate has two PMOS transistors in series and  two NMOS in parallel, the layout and truth table shown in  figure 5. As per the truth table, Z will always be logical 0  unless both inputs A and B are 0, where both PA and PB are  ON


90nmLaser spotsize~270mm


NMOS


Figure 5: truth table and physical layout of 2-Input NOR gate


The LVP waveforms in Figure 6 are collected from the input  and output nets of the NOR gate. When both PMOS transistors  are OFF, we observe a third state in the waveform collected on  the output Z as indicated by the arrows.


|INPUT|INPUT|INPUT|A|A|
|---|---|---|---|---|

|I TM|PI||||

|OUTP|OUTP|UTZ|||

|1|1||T||

|||1|T H||

|N PU|N PU|N PU|N PU||

|0|0|0|TPUT Z|TPUT Z|

|1|1|1|||

|1|1|1|1|1|

Inputs waveforms collected from PMOS active


INPUT A


主


INPJTB


OUTPUT Z PMOS


INPUTA


o


INPUT B


OUTPUT Z


OUTPUT Z NMOS


PMOS0


1 0 1 Figure 8.a


s0


Figure 6: LVP waveforms of 2-input NOR gate


The third state lies below the “0” state of this output when we  compare the waveforms to the truth table of the NOR gate. This again is explained by free carrier absorption mechanism


INPUT


surrounding the probe placement point. While the logical state


per truth table is 0 when just 1 PMOS transistor is OFF, a


channel still exists in the PMOS transistor whose gate is ON  causing some amplitude modulation. When both the transistors  are off, we get the least modulation state, or a trough that is  lower than the logical 0.


Through both NAND and NOR we see that it doesn’t matter  whether the waveforms are generated from the NMOS or the  PMOS. We are able to map the logic state of the standard cell. We observe in both cases that it doesn’t matter whether the  transistors are in series or in parallel, as long as the gate is  toggled and the channel is created, we seem to be able to  observe the laser modulation.


VDDA


Z


2-Input AND, XOR, OR gates


NAND, NOR and NOT are the standard building blocks for


|Input A|Input  B|Output  Z|
|---|---|---|

|0|0|1|

|0|1|0|

|1|0|0|

|1|1|0|

PMOS


B


other standard cells. Cells AND, OR and XOR are generally  built using a combination of NAND, NOR and NOT.


614*14****3


13133


11654996635441


1555344144444


Metal 1Contact


A


ZA


NAND


NOR


■Active容Laser spot location onB


VSS


GatePMOS


2-Input AND


2-Input OR


Laser spot location on


Figure 7: Building 2 input AND and 2 input OR gates


Therefore, when we study Figure 8a, which is collected from a  2 input NAND gate and Figure 8b collected from the 2-input  OR gate, we only observe a 0 or a 1. We don’t have a third  state because the output of the standard cell in either case is  driven by an inverter which has only 2 states.


1ORN


Figure8.b


INPUTA1


INPUTB


OUTPUTZ1bD1


。1


1111


P0


Figure 8.a LVP waveforms of 2-input AND gate and


Figure 8.b LVP waveforms of 2-input OR gate


On Figure 9, we can observe the waveforms out of a 2-input  XOR gate along with its schematics and the truth table right  below.


OUTPUTZ0110


00M


Input B


Figure 9: LVP waveforms, schematic and truth table of 2-input XOR gate


Even though the XOR is built using NAND gates, we are  unable to see the third state at the output. The reason behind  this behavior can be understood from the truth table. A NAND  gate’s output reaches 1+ only when both of its inputs are 0. The  design does not allow for a 0 on both inputs (M and N) thereby


Cycle: 12345678


preventing the appearance of the 1+ state.


We have presented multiple 2-input standard cells and 0 explained how to build the truth table. In similar manner we 1 could approach more complex logic gates. Knowing what


waveforms to expect from logic gates is essential to fault 0 isolation.


Case Studies


We can use combinational logic analysis to debug scan logic


OUTPUTZONAG6ODUN0


failures. Since we are able to observe all the combinations of


1 0


the truth table, the analysis time is quite fast and we can  confidently assess the reported failing circuitry.


2-Input NAND failing scan logic


In this first case study on 28nm bulk silicon IC failing gross to


OUTPUTZ ON THE FAILING UNIT


scan logic, the diagnostics reported suspect to be a 2-input  NAND with either a dominant bridging or open mechanism.


## Case Studies


The suspect NAND has a large (4 fingers wide) fan out as seen  in the layout on figure 10. The red circle represents the laser  spot used during LVP probing. As you can see, the spot does  not cover the entire active, but only a portion of the active


1INPUTA


driving the output. We performed combinational logic analysis  by identifying a window within the load cycle where we could


P0AXOR F


see all the 4 combination of inputs as in Figure 11.


MINPUT B。0EXOR P s1


OUTPUT Z 0


Input A


INPUT A01


INPUT B00101


Output Z


5noWD


Figure 10: layout of reported 2-input NAND gate


|A|B|L|M|N z||
|---|---|---|---|---|---|

|0|0|1|1|1 0||

|0|1|1|1|0 1||

|1|0|1|0|1 1||

|1|1|0|1|1 0||

While the input A is collected from an inverter, input B is an  output of a NAND and shows “tri-state” at cycle 3 which from  our library know it to be logic 1. From the initial discussion we  should expect 3 states, 0, 1 and 1+ depending on the input, but  we observed 4 states. The pink arrows on the reference  waveform at cycles 3 and 4 show that when only input B is 1, the waveform is modulated a lot more than when only input A  is 1. This is an aberration created by laser placement as it is  placed on top of the active that is controlled by input B more  than input A. The truth table does not offer any difference in  logic so both states are 1 though there appears to be an  obvious transition.


Figure 11: LVP waveforms from the failing and reference 2-input NAND gate


The red waveform does not look obviously wrong, states are Aflat and the transitions are sharp.  It would have been very hard


to conclude that the signal is incorrect. The only observation


that causes suspicion is the absence of extra states when B


compared to library NAND waveforms especially when both


CL+尔22Q=AXOR(BXOR C)


inputs are low.


Not understanding the good signal clearly could cause further  confusion. The transitions indicated by pink arrows are not  indicating any change in logic state but only a switch between  the inputs B and A turning on. The LVP is modulated a lot  more by input B than A because of probe placement. The  failing and reference waveforms look conclusively different  only in the transition between cycles 6 and 7 (marked by the  red arrow) where we couldn’t see the third state.


We built the truth table from the waveforms in Figure 12.


|AB||cycle|Expected|observed|
|---|---|---|---|---|

||00|5|1+|1|

||01|2|1|1|

||10|1|1|0|

||11|7|0|0|

Figure 12: Building truth table with waveforms indicates input  B is stuck at 1


As long as input B is 1, the observed and expected states  match. But they don’t match when input B is 0. This means the  input B is likely stuck at 1. Since the signal at the active of  input B looked normal it suggests that the defect could be in  the interconnects of net B, or within the logic gate itself. Physical analysis confirmed metal short between net B and  VDD.


BX


This case study proved that unless we observe all combination  of inputs, we may not be able to ensure the functionality of the  standard cell. Secondly, when comparing the bad signal with a  reference good signal there could be situations where we have  a “false” toggle, like in cycle 3-4, where the truth table does  not expect any state change, but the reference waveform shows  1 because of the laser placement. This could mask the real  failing signature. An exhaustive truth table construct really  helped us to identify the cycle at which the signal clearly does  not match expectations.


3-Input XOR with 1 input stuck


In this last case study, we perform fault isolation on a 3 input  XOR. The scan diagnostics reported that the flop is failing  open but was unable to identify which net caused it to fail. Figure 13 shows the schematic of the 3 input XOR.  It is made  of 2 XOR gates, with inputs B and C being XOR first and the  resultant signal is BXORC. The second XOR gate performs  the same operation between A and BXORC to generate Q


BXORC


Figure 13: Schematic of 3 input XOR


The inputs and the internal nets are probed to perform  combinational logic analysis in Figure 14.


|Cycle:  1 A 0|||||||10|11|1213|14|15|16|
|---|---|---|---|---|---|---|---|---|---|---|---|---|

|Cycle:  1 A 0|B 0||||||||||||

|1|B 0||||||||||||

|1|0||||||||||||

|BXORC 0-|0||||||||||||

|BXORC 0-|0 A:||||||||||||

|BXORC 0-|0 A:||||d|||||||1 1|

|B:|||||||||||||

|C:|||||||||||||

|ORC: 0|1||||||||1||||

|Q: 0|1 1|||1|1||||1|1 1 1|1 1|1 1|

|QEXPECTED:  1|1 1|||1|1||||1|1 1 1|1 1|1 1|

Figure 14: combinational logic analysis on failing XOR


The waveform on internal node BXORC showed that the  operation was correct and matches our library. BXORC  became high when only 1 of the inputs B or C was 1 and the  other 0 as in cycles 1, 3 and 4. Q, on the other hand, did not  match the expected output on certain cycles and indicated by  red. In close examination of the constructed table, Q does not  match whenever input A is high indicating one possibility is  that net A could be stuck at 0. It could also mean an internal  bridging or open within the 2nd XOR.


Since the active driving input A showed good LVP signals, the  PFA was focused on the interconnects of net A and internal  nets of the 2nd XOR.   Physical analysis was performed and  M2 bridging was observed within the second XOR gate as in  figure 15.


Figure 15: STEM analysis of M2 bridging


In this case study, the output Q does toggle to both 0 and 1, so  it would have been harder to isolate in the traditional way. Using combinational logic analysis we were able to identify  the failing net much faster and with increased accuracy, speeding up the overall analysis.


We first introduced combinational logic analysis, which is a  great way to ensure the functionality of standard cells. It  involves identifying the right time window within the load  cycles of a scan pattern that injects all combinations of inputs  into the suspect standard cell and in building a truth table using  the waveforms generated from its output.


We then described our LVP library building process and  showed how the output signals may have multiple states  depending on the transistors being probed. We explained how  an identical looking waveform could indicate different logic  states depending on the combinational gate of interest. For  example, the middle state in the waveform for NAND is a  logic 1 but the same state is a logic 0 for NOR.


[1] Bruce MR, Bruce VJ, ABCs of Photon Emission  Microscopy, Electronic Device Failure Analysis, Vol. 5, pp.13-20, 2003.


[2] E.I. Cole Jr., Paiboon Tangyunyong, Charles F. Hawkins, Michael R. Bruce, Victoria J. Bruce, Rosalinda M. Ring  et al., Resistive Interconnection Localization, ISTFA  2001, pp. 43–57.


[3] M.R. Bruce et al., Soft Defect localization (SDL), ISTFA  2002, pp.21-27.


[4] Kevin Sanchez, Romain Deplats, Felix Beaudoin, philippe  Perdu, Dean Lewis, Praveen Vedagarbha et al., Delay  variation mapping induced by dynamic laser stimulation, IRPS 2005, pp. 305–311.


[5] K. Nikawa, S. Tozaki, Novel OBIC observation method  for detecting defects in Al stripes under current stressing, ISTFA 1993, pp. 303–310.


A particle at the red  signal location


The cross section image at the  particle location


Abnormal metal profile


induced by the particle


Metal bridged induced by the particle


Fail: Red signal


Pass: Green signal


200 Mag


1000 Mag


## Combinational Logic Analysis using Laser Voltage Probing


Combinational Logic Analysis using Laser Voltage Probing


## Venkat Krishnan Ravikumar, Winson Lua, Seah Yi Xuan, Gopinath Ranganathan, Angeline Phoa


Venkat Krishnan Ravikumar, Winson Lua, Seah Yi Xuan, Gopinath Ranganathan, Angeline Phoa


## Device Analysis Laboratory, Advanced Micro Devices, Singapore


Device Analysis Laboratory, Advanced Micro Devices, Singapore   Venkat-krishnan.ravikumar@amd.com


Laser Voltage Probing (LVP) using continuous-wave near  infra-red lasers are popular for failure analysis, design and test  debug. LVP waveforms provide information on the logic state  of the circuitry. This paper aims to explain the waveforms  observed from combinational circuitries and use it to rebuild  the truth table.


## 1. Introduction


Background


Continuous wave Laser Voltage Probing (LVP) is a technique  that has been successfully employed for design and test debug  as well as Electrical Fault Isolation (EFI) of integrated circuits  in recent times [1, 2]. The tool is used to study activity within  transistors while the tests are being run by observing optical  modulations on an incident laser [3]. It is especially useful in  identifying when exactly the switching event takes place.


Laser Voltage Imaging (LVI) and LVP for scan chain failures  is an established practice where we inject a periodic signal into  the chain and use to system to observe the frequency within  silicon [4, 5 and 6]. LVI is useful when we observe periodic  signals and can be exploited for debug of any chain like scan, JTAG, or even daisy chains as long as we are able to inject a  periodic signal. However, LVI has very limited applications in  circuitry that don’t normally toggle with a periodic frequency  which restricts its application for functional or scan (not chain) failure.


In case of fault isolation on scan logic or a functional failure, we resort to LVP. Here, we attempt to identify an exact toggle  event during the test [7]. Since probing is performed on 1  transistor at a time within a specific time window, the analysis  takes more time to complete. While interpretation of  waveforms from inverters is simple, waveforms generated on


LOADING CYCLESCAPTURE


UNLOADING CYCLES


combinational logic often show extra peaks or troughs that are


CLK


harder to interpret


A=1->0


Objectives


In this paper, we introduce combinational logic analysis, with  which we perform a comprehensive diagnosis of a standard


B=1->1


cell by observing LVP waveforms on the outputs of the cell


during the load cycles and building its truth table.


2=1->0


We will also attempt to explain why the waveforms measured


at the output nets of a combinational logic are often complex. This deeper understanding of the waveforms enables us to  make use of them to check the full functionality of the cell and  significantly speed up the turn-around-time.


## Venkat-krishnan.ravikumar@amd.com


## Abstract


2. Scan logic and Laser Voltage Probing


Scan is a fundamental DFT used extensively in testing most of  the logic elements and interconnections in the Silicon on chip. The tester loads the test vectors through the scan chains by  scan shifts. Once the scan cells are loaded with the right logic, they sensitize the inputs of the circuitry of interest with a  particular logic combination. The data are propagated through  the circuitry of interest and its outputs captured by other scan  flops. Finally the captured data are unloaded through scan  shifts in the chain that captured the output and is compared to  what is expected by the test. A simple circuit like a 2-input  NAND gate will need at least 4 patterns (combinations of 0  and 1 on either input) to test its functionality completely. Based on the test results of an exhaustive pattern list, a scan  diagnostics tool analyses the outcomes and predicts the failing  nets.


Fault isolation on scan logic failures usually start with the  diagnostics results. The callouts often contain 1 or more logic  elements which form a cone of logic and can explain one  symptom of the failure. The more elements there are in this  cone, it indicates that there are not enough scan nodes to inject  inputs or receive outputs directly limiting the resolution of the  test. Very often, users have to perform advanced diagnostics  combined with patterns modifications to have better control  over the toggles in the area of interest and make it debug  friendly [8]


Figure 1 describes how the diagnostic tool looks at a standard  cell. During load or unload cycles, the inputs and the outputs  are non-deterministic. Only at the last load cycle, the entire test  vector has completed loading and each output node of the scan  flops is deterministic.


Figure 1: scan logic test on a standard cell with 2 inputs A  and B and its output Z


Since these nodes connect to the inputs of the standard cell, the  capture cycle is entirely deterministic and the result is  observed at the capture flops for unloading. Once the pattern  begins unloading, the nodes of the standard cell are no longer  deterministic.


As the resolution of the diagnostic tool is restricted, EFI is  performed to identify the exact failing net within the cone of  failing logic. Depending on the test conditions and the failing  signature, we may have to perform LVP to identify if an  individual logic element in the failing cone observed the  correct transition at the scan capture cycle. To perform that, the failing pattern is loaded into the scan chains and the LVP  observation window is opened to observe toggles from the last  few load cycles, the capture cycle and the first few unload  cycles.


3. Combinational Logic Analysis Procedure


LVP on a scan logic failure can become complicated because  of the following reasons:


(1) LVP waveforms from standard cells do not have just  2-states 0 and 1. Some cells exhibit multiple states  that make understanding the waveforms difficult.


(2) During the capture cycle, there is just 1 transition at  the input and output nets. For some patterns, there  might not be any transition on a particular net like in  input B on Figure1. This makes it harder to confirm  correct activity on the net being probed.


(3) 1 correct transition on the pattern being tested does  not guarantee that the standard cell is entirely  functional, it could fail for certain input combinations  that can only be tested with another vector making the  entire process very time consuming.


To overcome these challenges and to improve the turn-aroundtime of LVP, we introduce combinational logic analysis which


A: output of inverter I


in essence has the following steps:


Signal collected from PMOSA active of net A


(1) Observe the load/unload cycles where there is plenty  of toggling activity on the inputs of the standard cell.


While the activity of standard cells during  load/unload cycles are non-deterministic for the  diagnostic tool, LVP can be used to observe the


7


7. outputof inven ten I


inputs for each cycle thereby making every cycle


active of net ∠


Signal collectedfrom PMOS


deterministic.


(2) Study and build a library of standard cell responses  by including all combinations of inputs. For a 2 input  cell, we only need 4 combinations of inputs.


(3) Observe a specific window of a load cycle where the  complete truth table can be built. Since the toggles  during the load cycles are caused by loading of vector  into the scan chain which is an arbitrary string, it is


## 3. Combinational Logic Analysis Procedure


easy to find a time window that has all the elements  of the truth table.


(4) Compare the observed response to the library  response.


4. Building the LVP library


The next section is a discussion on how we build the LVP  library to perform this analysis. An important part of building  the library rests on the laser placement. Since the output of  standard cells are a combination of multiple transistors, both  the laser placement and the size of each transistor matters. If  multiple actives are below the laser spot, the resultant is a  convoluted waveform. If the laser spot is unable to cover the  entire net, or is closer to one of the inputs than the other, the  resulting waveform could look distorted.


Most standard cells have complementary NMOS and PMOS  transistors, either of them can describe the logic state of the  cell. As the waveform collected look inverted from each other, we observe a convention where the signals from PMOS  describes the actual logic state and the NMOS has the signals  inverted


Laser Voltage Probing on inverter


Nets usually originate at the source/drain of a NMOS/PMOS  transistor and feeds into the gate of one or more transistors. Throughout the paper we follow a convention of naming and  probing the transistor whose source/drain feeds the net of  interest. Interpretation of LVP waveforms on simple elements  like an inverter is straightforward. For example, in Figure 2, we have waveforms collected from PMOS transistors of 2  cascaded inverters I and II. While the signal toggles from low  to high on net A, it toggles from high to low on net Z as  expected.


Figure 2: LVP on 2 cascaded inverters


While we haven’t shown here, the NMOS will show a falling  transition on the net A and raising transition on Z


2-Input NAND Gate


The level of complexity increases when we probe on  combinational logic elements like 2-input NAND gate. In an  ideal situation, LVP is performed on an individual transistor.


A logic state of a net (say output) is a combination of  responses from multiple transistors, both NMOS and PMOS. A gate with 2 or more inputs needs additional assessment on  which location would be better to probe


Figure 3 is the truth table and the physical layout of a 2-input  NAND gate with inputs A and B and output Z. As per the truth  table, Z will always be logic 1 unless both inputs A and B are  logic 1. On the left of Figure 2, we can see the physical layout. The Z net’s driver on the PMOS side is a combination of  transistors PA and PB. Either PA or PB needs to be a 0 to


conduct charges from the power supply through to the Z.


When we look at the NMOS side, we draw a parallel analogy.


Only when both NA and NB are 1, charges conduct from the


ground to the Z.


a 0ND


VDDAZ


1+


OUTPUTZ PMOS


0OUTPUT Z NMOS 1


NMOS1*ND


INPUT B011p


ActiveLaser spot location on


OUTPUTZ1


1#1


INPUT A1


|Input A|Input B|Output Z|
|---|---|---|

|0|1|1|

|1|0|1|

PMOS 1


P INPUTB


Figure 3: truth table, physical layout of 2-Input NAND gate


The red/yellow stars in Figure 3 show the laser probe  placement when LVP waveforms are collected from the  PMOS/NMOS of net Z respectively. Let us observe the LVP  response from both PMOS and the NMOS when the laser is  placed on the Z net on Figure 4. Signals from inputs A and B  are taken from actives of inverters feeding into the NAND  inputs.


We are able to rebuild the truth table using the waveforms on  either the NMOS transistors or the PMOS transistors of inputs  A, B and Z. Since we follow the convention to name the  PMOS waveforms as positive logic, the lower level of the  waveform is “0” and the higher level is “1”. Since A and B  waveforms only have 2 levels, we are able to assign a 0 or a 1  easily.


However, on Z, we have an interesting observation. Marked by  white arrows, certain cycles show a third state of higher than  normal amplitude. The difficult part proceeding to this work  has been in explaining what causes tri-stating signals on the  output because a digital device can only have a 0 or a 1 as its  output. Comparing against the truth table, we observe that the  third state (white arrow) occurs only when both inputs A and B  are 0 (i.e. both the transistors PA and PB are ON). When this  happens, there is a difference between logical state described  by the truth table and the observed state using LVP.


Finally, we showed two case studies and in both cases, there  were “normal” looking waveforms from the output of the  standard cell, but in close inspection of the built truth table, we  observed deviances in certain input combinations with which  we had a better isolation of the defect location.


In conclusion, using combinational logic analysis significantly  improves the success rate and reduces analysis time of LVP  when debugging standard cells.


Acknowledgments


Authors would like to thank AMD management and Rod  Wampler from AMD Austin who advised this work


## Conclusions


## Acknowledgments


## Authors would like to thank AMD management and Rod Wampler from AMD Austin who advised this work


## References


[1] Jiann Min Chin et al., “Fault isolation in semiconductor  product, process, physical and package failure analysis: Importance and overview,” Microelectronics Reliability 2011


[2] V.K. Ravikumar et.al, “Laser Voltage Probing in Failure  Analysis of Advanced Integrated Circuits on SOI” IPFA 2011


[3] Ulrike Kindereit, “Fundamentals and Future Applications  of Laser Voltage Probing,” IEEE-IRPS 2014


[4] Yin S Ng et al., “Laser Voltage Imaging: A new  Perspective of Laser Voltage Probing,” ISTFA 2010


[5] Yin S. Ng, et al, “Scan-Shift Debug using LVI Phase  Mapping” ISTFA 2013


[6] T. Parrassin et al “Laser Voltage Imaging and Its  Derivatives, Efficient Techniques to Address Defect On 28nm  Technology” ISTFA 2013


[7] SH Lee et al.  “Case Study: Failure Analysis of Functional  Shmoo Hole with Laser Voltage Probing” ISTFA 2009


[8] Christian Burmer et al. “Timing Failure Debug using  Debug-Friendly Scan Patterns and TRE” ISTFA 2008


[9] Jayashree Saxena et al. “Scan-based transition fault testing


- implementation and low cost test challenges” ITC 2002


Comparison of Photon and Thermal Emission microscopy for Dynamic Fault  Isolation


SH Goh, GF You, Alan Tan, CV Bharadwaj, Hu Hao, BL Yeoh, Jeffrey Lam


Unlike photon emission microscopy which is usually the first  go-to technique in tester-based or dynamic electrical fault  localization, infrared thermal microscopy does not play a  similar routine role despite its comparable ease in application. While thermal emission lacks in optical resolution, we  demonstrate superior sensitivity and accuracy over photon  emission on dynamic fault localization of backend-of-line  short defects.


In static fault localization, photon emission microscopy is well  known to be ineffective against backend-of-line (BEOL)-related defects, in particularly shorts, unless they occur in the  device layer. Laser stimulation technique such as ThermallyInduced Voltage Alteration (TIVA) and Optical Beam Induced  Resistance Change (OBIRCH) [1, 2] is the mainstream  solution to address interconnection defects in integrated  circuits (ICs). In dynamic fault localization which typically  involve running a set of test vectors to exercise logic circuits  to access the defect, significant fluctuations in supply current  could pose a challenge in the deployment of similar  techniques. Typical averaging procedures or lock-in  enhancements [3, 4] is not sufficient to achieve a reasonable  signal to noise for fault localization. Although there are  reports of success in the application of OBIRCH to functional  failures in analog mixed signal IC [4], it usually involves a  reasonably stable current in the interested supply. Furthermore, for systems on a chip, the circumstances might  not be as ideal. Figure 1(a) illustrates the dynamic current  measured on two different digital power supplies (DPS) while  executing a scan test pattern on a reference die. It can be  observed that the current changes drastically throughout the  entire test pattern. In a previous report, we showed that  although the test clock can be halted at a specific cycle where  the current is stable and a common ground be implemented  between the tester and scanning optical microscope to manage  ground loop noises, it remains a tedious process in localization  without prior information on the fail cycle of interest [5]. In  the worst case, the number of localization iterations is  equivalent to the total of test cycles. This workflow is not  realistic. Even if the fail cycle of interest is identified, a  second potential challenge exists in the application of such  technique. From Fig. 1(b), it is apparent based on the dynamic  current from a typical functional test comparing three bad and  two reference dies that few tens of mA current fluctuation is  common. This affects the detection of weak signals. Hence,


from these challenges, pseudo-dynamic laser stimulation  techniques are not as successful as their predecessors (static  bias) in the localization of interconnection shorts that lead to  functional failures.


Currently, because of its ease in application, photon emission  remains a popular choice for dynamic fault localization in  spite of its low success rate on interconnection short defects. Although thermal microscopy has been proven effective  before on microprocessor and scan chain failures from legacy  process technology devices greater than 90 nm [6, 7], it is not  widely accepted as a routine tool due to its poor optical  resolution. We advocate thermal microscopy as a  complementary tool to photon emission to bridge the gap in  dynamic fault localization of interconnection defects. This  work seeks to demonstrate the superiority of thermal  microscopy in terms of its accuracy and sensitivity on an  advanced process technology node device.


This paper is organized as follows: Section 2 describes the test  vehicle used in this work. The analog voltage controlled delay  line was selected because it is a simple logic test structure and  easy to observe the functionality using an oscilloscope. Experimental results comparing photon and thermal  emissions’ signal strength and the accuracy of hotspots  location with respect to a known programmed defect will be  presented. The main points will be summarized in the  concluding section 3.


Test Cycle Number(b)


Figure 1: Dynamic current measured from (a) two different  digital power supplies and (b) three bad and two reference  dies.


Clkretckso


niuCIK360


Test Sample


A multi-stage analog voltage-controlled delay line (VCDL) fabricated on 28 nm process technology is used for the  experiment. A simplified schematic is depicted in Fig. 2. The  VCDL comprises of multiple cascaded variable delay stages  with buffers connected to each stage. A control signal C  determines whether the signal from the buffer can be observed  on an output pin. There are 5 observation points namely pinout  1 to 5. The phase shifts with respect to CLKref is indicated in  the figure. The magnitude of signals equal the voltage control  Vctrl. To create the test sample, we damage the buffer at the  first cascaded output buffer permanently using spot mode laser  at 1340 nm wavelength laser from the silicon backside. The  other stages are not affected. To prove this, the circuit is  powered up and pre-conditioned using a national instrument  PXI bench tester and pinouts of the second (Clk90) and last  stage (Clk360) are observed on an oscilloscope. Figure 3 shows  the waveforms with respect to CLKref. It is evident that the


25 μm


signals can be observed as expected and the outcome of the


programmed defect is achieved. In this case, the laser is likely


to have caused a localized short failure at first metal layer.


Figure 4(a) and (b) show the reflected laser image at 50X


objective digital zoom 4 of the VCDL circuit before and after


laser-induced damage, respectively. The damage site also Ref


BD


referred to as the programmed defect location is indicated in  Fig. 4(b).


Signal Accuracy


Figure 5 presents the photon emission signals acquired while  exercising the VCDL. The photon emission camera is a liquidnitrogen (LN2)-cooled system that comes with an Indium  Gallium Arsenide (InGaAs) focal plane array. It is a common  standard in most EFA laboratories. Comparing the emissions  of a good unit as shown in Fig. 5(a), it is obvious that there are  anomalies around the damage region on the bad unit signal  image as shown in Fig. 5(b). Reflected laser image overlay


with good and bad unit signals in the region marked with


□


dotted lines are shown in Fig. 5(c) and (d) respectively. Figure


1.0


Thermal microscopy utilizing an indium antimonide (InSb) focal plane array is applied next and the thermal signal image


0.9


114


boB0BD▲RBDR


is shown in Fig. 6.


1.12


08


1.10


1.08


CIkret


CIK


1.00


0.6 -▲


Current (A)Core VDD


1.04


后


0.5


109池中


wig tnsing


buf


20000 60000 80000 80000 100000 120000 140000180000


c


pinout 1


pinout 2pinout 3pinout 4pinout 5


020000 400006000080000 100000 120000 140000 160000


bufbufbufbufbuf


ghgpmn


Vectrl


CIk O°


CIk 90°Clk 180°Clk 270°CIk 360°Figure 2: Schematic of a simple multi-stage analog voltage  controlled delay line.


DOC0-- 8m


Figure 3: Comparison of output waveform between Clkref, Clk90 and Clk360.


Figure 4: 50X digital zoom 4 optical image a) before and b) after laser damage at location indicated by arrow.


Figure 5: Dynamic photon emission signals of (a) reference  and (b) bad unit. Emission overlaid on reflected laser images  of (c) reference and (d) bad unit.


Figure 6: Infrared thermography (a) signal image and (b)


signal overlay with layout image. Crosshair indicates


location of abnormal signal.


Figure 7: Reflected laser overlay with layout image


indicating thermal hotspot and emission locations.


1μm


Figure 8: Bridging at first metal layer at PD locality.


Figure 6(a) indicates the location of the abnormal signal and  Fig. 6(b) illustrates the signal overlay with layout. The  crosshair identifies the location of the thermal hotspot on  layout. It should be added that the contrast of the thermal  image is stretched to reveal the background device features


that arises by virtue of the emissivity differences of different  materials to achieve the overlay.


A detailed analysis using layout overlay reveals that the  abnormal photon emission signals is approximately 10 m  away from the programmed defect (laser mark) as shown in  Fig. 7. However, the thermal hotspot is very close, if not at the


50um


exact spot of the programmed defect with reference to Fig. 6(b). A delayer PFA is performed at the location of thermal  hotspot location and the laser damage site is found at the first  metal layer, causing a bridge defect as shown in Fig. 8. We  explain the relationship between the bridge defect and the  observed emissions next.


First, let’s analyze the photon emissions on a good VCDL. The region marked by dotted lines in Fig. 5(a) is magnified as  shown in Fig. 9(a). The 5 brightest signal spots correspond to


以*


the buf block that outputs that observable pinout signals. Spot


盖地


1 (Clk0) is further magnified as depicted by the inset in the  figure. The signals are sub-divided into 3 sections, namely 1.1,


港"我


1.2 and 1.3. The transistors in each section are identified in the  schematic of the buf block as shown in Fig. 9(b). The states at


50μm


nodes A and B are 0 and 1 respectively. Node C toggles  according to the input which is the delay line driven by  CLKref. This explains the presence of the signals on a good  device since all the transistors in the 3 sections are turned on. Similarly, for the damaged unit, the region marked by dotted  lines in Fig. 5(b) is magnified as shown in Fig. 10(a). It can be  observed that section 1.1 shows a bright signal and some


Photon Emission


Laser mark*


signals are missing in the other sections. Figure 10(b) depicts  the schematic of the buf block which includes the location of  the shorted internal net caused by PD. This causes the drain of  the PMOS transistor in section 1.1 to be directly connected to  ground, resulting in an increased current leakage. Therefore, the intensity of emission signal increases. In section 1.3, only  the PMOS of the inverters is activated, hence explaining the  comparatively weaker signals compared to reference. NMOS


transistors in section 1.2 are also turned off. In this simple  experiment, neither the brightest nor the missing signals  indicate the defect location. This demonstrates the poor  accuracy of photon emissions as compared to thermal  emissions.


运


1.1


CSDSA


1.2 13


Figure 9: (a) Emission signals within the dotted region in  Fig. 5(a). (b) Schematic analysis of buf block as labeled in  Fig. 2.


40


Figure 10: (a) Emission signals within the dotted region in 0


Fig. 5(b). (b) Schematic analysis of buf block as labeled in


0102030405060 Fig. 2 showing the shorted path.


Pixel number


■0.4s


Signal Sensitivity


1s


The acquisition time for photon and thermal emissions are


◆2s


varied and studied in this section. The results are presented in "


▼4s


Fig. 11. From Fig. 11(a), it can be observed that at 2s, the


10s鹏


abnormal signals are barely visible and become apparent at 5s g of exposure. On the contrary, thermal hotspot can be observed


after 1s of exposure as shown in Fig. 11(b). In fact, a very


台 faint signal is barely discernable as low as 0.4s as indicated by


arrow. The sensitivity can be better understood using line


abitraryIntensity ( unit)吕 profile analysis.


2s


10's


020406080100120140 Pixel number


0.4s


input


4s


Buffer pinout


bias


Figure 11: Dynamic (a) photon emission and (b) thermal  emission at varying acquisition time.


Line profile analyzes are performed on the signals spots across  AA’ and BB’ for photon and thermal hotspots. Figure 12  presents the line profiles. The different plots represent varying  acquisition time and are intentionally offset in intensity for the  purpose of comparison. Figure 12(a) clearly shows that at 5s  exposure time, the photon emission signal peak is beginning to


be distinguishable from the noise level. Unlike photon  emission, at 1s acquisition time, the thermal emission signal is  obvious. At 0.4s, a nascent peak can be observed. This  analysis proves the higher sensitivity of thermal microscopy. Although this is not a complicated functional device, this  experiment demonstrates the potential of thermal microscopy  once again in the detection of BEOL-related short defects.


260


qnf


■ 2s


!udni


2205s 200◆10s


160


88988888品100120140◆ 30s▼20s 240


Figure 12: Line profile across a) AA’ and (b) BB’ as defined  in Fig. 11.


As we encounter more logic functional failures in leading edge  technology devices yield ramp, it is necessary to review  current dynamic fault localization approaches against defect  detection coverage and effectiveness. One current industry  challenge is in BEOL-related defects, especially internal short  or open nets in logic which do not emanate photon emissions. Thermal microscopy is effective in this respect but has not  been widely employed as a routine dynamic fault localization  method mainly because of its limitation in optical spatial  resolution. Many are still not convinced even though thermal  solid immersion lens has been proven. Using a simple analog  circuit, we heightened the awareness experimentally on the  merits of thermal microscopy in terms of localization accuracy  and sensitivity to BEOL short defects, to complement photon  emission microscopy as go-to dynamic techniques for global  defect localization. The former is able to pinpoint the exact  location of defect and can be potentially 2 times more  sensitive than photon emission.


[1] JCH Phang et al., “A Review of Laser Induced  Techniques for Microelectronic Failure Analysis”, Proc  Int Symp Physical & Failure Analysis of Integrated  Circuits, 2004, pp. 255-261.


[2] E Cole, P Tangyunyong, DL Barton, “Backside  localization of open and shorted IC interconnections”, Proc Rel Phy Symp, 1998, pp. 129-136.


[3] ACT Quah, JCH  Phang, LS Koh, SH Tan, CM Chua, “Enhanced detection sensitivity with pulsed laser digital  signal integration algorithm”, Proc Int symp for testing  and failure analysis, 2006, pp. 234.


[4] C Wu, S Yao, “Realizing Dynamic Thermal Laser  Stimulation by Lock-in IR-OBIRCH Assisted with a  Current Detection Probe Head”,  Proc Int symp for testing  and failure analysis, 2013, pp. 357.


[5] SH Goh et. al., “Tester-Driven Dynamic Laser  Stimulation for Hard Functional Failure”, Proc Int’l Symp  for Testing and Failure Analysis, 2010, pp. 332.


[6] LT Hoe, YW Mun, CY Yan, “Characterization and  application of highly sensitive infra-red emission  microscopy for microprocessor backside failure analysis”, Proc Int’l Symp Phy and Failure Analy of Int Circuits, 1999, pp. 108-112..


[7] L Forli, B Picart, A Reverdy, R Schlangen, “Scan chain  debug using Dynamic Lock-In Thermography”, Proc Int’l  Symp for Testing and Failure Analysis, 2011, pp.153-157.


Unique Approaches to Isolate Nano-scale Defect in Snake-Comb Test  Structure


Sujing Xie, Nathan Wang, Chaoying Chen, Qindi Wu


Maxim Integrated, 160 Rio Robles, San Jose, CA, USA


Multiple techniques including electrical resistance  measurement plus calculation, cross-sectional  view of passive voltage contrast (XPVC) sequential searching, planar and cross-section  STEM are successfully used to isolate a nanoscale defect, single metallic stringer in a snakecomb test structure. The defect could not be found  by traditional failure analysis methods or  procedures. The unique approach presented here, expands failure analysis capabilities to the  detection of nanometer-scale defects and the  identification of their root causes. With  continuous shrinking feature sizes, the need of  such techniques becomes more vital to failure  analysis and root cause identification, and  therefore yield enhancement in fabrication.


In existing IC fabrication, yield is typically  limited by defects generated in the manufacturing  process. In fact, yield often shows a good  correlation with the type and density of the defect. As a result, understanding the root causes of  failure is essential for yield improvement [1].


Test structures such as via or contact chains, snakes and combs are commonly used to detect  defects. Comb/snake structures usually cover a  large area (up to mm2 scale) and have high density of metal/poly lines. As process technology goes to  deeper submicron geometries and feature sizes  continue to shrink, it is becoming increasing  difficult to identify the defective sites. Common  fault isolation methodologies, such as optical  beam induced resistance change (OBIRCH) and  photoemission microscope (EMMI) do not always


work efficiently because, defects are more prone  to be damaged during failure analysis since they  are so small. When the low-level voltage is  applied, the signal cannot localize the defect, as  shown in Fig.1 (a) for the current case. The level  of current/voltage required to isolate defects by  OBIRCH and EMMI, can easily destroy subtle  defects (the snake-comb structure recovers in this  case, which means no short any more, at certain  voltage depending on the resistivity of the short). It makes root cause identification impossible.


This paper will discuss the combination of  multiple methods used to localize defects and  determine root cause. The first technique applies  low-voltage (less than 2V) to perform electrical  resistance measurements and then calculate the  approximate defect location; followed by FIB


Fig.1. A 20X OBIRCH image obtained at  low-voltage (1V) shows no specific defect  location – a region of the snakes light up.


XPVC to localize a short path. The second  technique utilizes planar STEM (P-STEM) to find  the defect site and feature using top-down view; then, cross-section STEM (X-STEM) on the PSTEM sample to get cross-sectional view of the  nanometer-scale defect, as single metallic stringer. To avoid the damage from SEM/FIB beam, the  low energy is selected for cutting and imaging. In  addition, the snake-comb structure is grounded by  graphite paint at the pad, and by Pt in P-STEM  and X-STEM procedures. The combination of the  multiple techniques is shown to enable a novel  way to identify nano-scale defects.


Experiments


2.1 Materials


The test vehicles used in the industry to obtain  defect characterization for BEOL are  predominantly snake and comb structures. The  schematic drawing in Figure 2 shows a snakecomb test structure. The spacing between comb  and snake is equal to the minimum acceptable  distance allowed by the design rules of chosen


sample. This structure can be used to detect shorts  in the metal or polysilicon layers. It should also be  noted that the multiple metal layers over the largearea test structure creates extra difficulties in top48


side defect isolation and uniform exposure of the  structure by parallel-lapping.


2.2 Procedures


Micro-probing is first performed between the  terminals of the snake and the comb to confirm  short/leakage state. Electrical resistances on  terminals of the test structure are measured by  applying a low-voltage (< 2V). The resistance  between the terminals 1 and 2 of the test structure  gives the total resistance R12 of the snake  structure, while the resistance between the snake  terminal (1 or 2) and comb terminal (3 or 4) gives  the total resistance of snake terminal to the short  defect R1S and the short defect to comb terminal  RS3. The relationship of these resistances can be  expressed by equation (1).


)1(


..........


3


23


13


S


R


⇒








+


=


Based on the resistance measurements and  calculations, the defect region can be narrowed


P a d


down to less than 1% of the total area. After


electrical fault isolation has been successfully


c o m b


S h o r t ↓ d e f e c t 0 m n _ 1


completed, the sample is mechanically polished to  remove the dummy metal layers over the snakecomb structure. Next, XPVC technique is used to  further narrow down the failing area. After  grounding comb pads 3 and 4, a defect search  procedure, as shown in Figure 3, was used. The 1st FIB cut is performed in the middle of the comb


s n a k e _


1 」 U L U


2  P a d


structure to determine whether the short path falls


to the top or the bottom of the cut area using


4


XPVC. This narrows down the investigation area  by fifty percent. Assuming the abnormal XPVC is  observed in the top half, the defect search  continues to 2nd, 3rd … FIB cut (with ~ 20 µm interval between neighboring cut), until the  abnormal PVC is isolated to a 20x5 µm2 area,which is the region with the short path.


Fig.2. A schematic diagram showing the snakecomb test structure for defect identification.


Once the long failing path to the small area is


localized, further high resolution localization with


P-STEM and final X-STEM to close in on the


defect is carried out by FEI Strata 400 Dual-beam


system. A combination X-STEM and P-STEM Rough rectangular mark to showRough makto indicate permits three-dimensional (3-D) characterization the area was narrowed down bytheisolatedsmalaea electricalmeasurement.


byX-PVC.


of the defect. A 3-D STEM technique has been  developed for such a purpose [2].


3Ground


comb


Comb terminalgrounded


→N* FIB


by graphite paint


+209 FIB  15 FIB


Results and discussion


3.1 Electrical Resistance Measurements


For sample #1 with a copper metal snake-comb  structure, the total length of the snake is ~1,300,000 µm with ~1000 µm per column, as  shown in Fig. 4.


The resistance measurements are as follows.


R12 ~ 873 kΩ


R13 ~ 325 kΩ


R23 ~ 548 kΩ


Ground


Substituting these values into equation (1), R1S  and R2S are obtained. The resulting values indicate  that the short defect is ~ 483,963 µm away from  the snake terminal 1, corresponding to the region  of column #483 ~ #485 (as roughly marked in Fig. 4). Considering the typical variation in probecontact


resistance


during


resistance  measurements, this calculated value only  determines the rough location of the defect.


3.2 Binary Search by Cross-section View PVC


To further narrow down the failing area, crosssection view PVC is performed by FIB cutting  and search after the top dummy metal layer is  removed by parallel-lapping. Since the test  structure covers about 1 mm2 area, it is very challenging to uniformly remove multiple metal  layers of the whole area without damaging the test  structure. After narrowing down the defect to  several


columns


resistance  measurements/calculations, the suspected defect  area is < 1% of the whole test structure. An area  that is much easier to uniformly expose without  breaking the metal lines in snake-comb structure. In addition, better grounding on the suspected  columns can be obtained for XPVC. Figure 4 is a


Fig.4. Overview of the snake-comb test


snake


structure with dummy metal over it.


comb -


Fig.3. A schematic diagram shows the defect  search procedure by XPVC. The 1st FIB cut is made in the middle of comb structure. From  this point, the interval of the following cut is  about 20 µm, until the abnormal PVC is  isolated to a 20x5 µm2 area.


typical XPVC SEM image. Principally, a  grounded metal line will appear to be very bright  whereas oxide surface or floating metal line will  appear to be dark. This is because when a metal is  grounded or connected to other conductive paths, the positive ions/electrons will be trapped on the  sample surface and these trapped charges will  build up a potential barrier above the sample  preventing low energy secondary electrons from  reaching the detector [3, 4]. To isolate the short  defect, the comb terminal is grounded by graphite  paint before loading the sample into FIB/SEM  dual system, as shown in Fig. 4. Therefore, the  abnormal PVC marked in Fig. 5 indicates that the  snake is shorted with the neighboring comb and  the defect is in the top half of the cut area. The  defect search procedure continues, as described in  Fig. 3, until a short site was isolated to a 20x5 µm2 area (as roughly marked in Fig.4).


Bottom Comb


300 nm


Top Comb


3.3 Planar and cross-section STEM


After the defect is isolated to the 20x5 µm2 area,P-STEM analysis is used to pin point the exact  failing spot. The reason to select P-STEM instead  of conventional physical failure analysis  techniques (such as polishing or plasma etching) is that conventional techniques miss subtle defects  and damage the sample. In order to avoid the


damage from SEM/FIB beam, the low energy  beam is selected for cutting and imaging and the  area of interest (STEM sample) was well  grounded by Pt in our procedures. Fig. 6 is an  example of planar SEM image after plasma  etching. It can be seen that the plasma etch leaves  a rough and uneven floor uniformity which makes  it difficult to find the root cause. The process of  removing material by FIB cleaning cross-section  can greatly enhance the quality and avoid the  contamination and confusion.


Figure 7 is a plan-view bright-field STEM image  obtained after FIB cleaning cross-section. The  short defect (marked by the red circle) exhibits  light grey contrast, which is invisible by  conventional physical failure analysis. In order to  better understand the root cause of the short  defect, a X-STEM analysis is performed. The  cross-section bright-field STEM image in Fig. 8  corresponds to the red-circled short defect region  of Fig. 7. The planar and cross-section STEM  results reveal the root cause of the failure to be a  metallic stringer which shorts the metal 1 snake to  the adjacent comb structure. The metallic stringer  consists of remaining tungsten material left by  unsufficient CMP polishing. The yield for this  process has been enhanced by slightly increasing  CMP time to avoid this kind of defect.


Fig.5. A typical XPVC SEM image showing  the short defect in the top of the cut area.


Fig.6. An example of planar SEM image of


Abnormal pC on snake


snake-comb test structure after plasma etching


This combined approach is one of the best  techniques that can discover nanometer-scale  defects such as metallic stringers. It can also be  applied to reveal any potential short/leakage  between two metal lines.


Metal combDielectricMetal Snake


Summary


The clever use of electrical resistance  measurement and calculation, defect search by  FIB XPVC observation, P-STEM for further  isolation and X-STEM successfully found a nanoscale defect, single metallic stringer in a snakecomb test structure. The approach described in  this paper have proved their capability in finding  nano-scale defects with reliable results. These  techniques expand the failure analysis world to  the role of defect localization and root cause  identification. With the increasing degree of  integration and scaling, the need of such  techniques has become more prominent in the


500nmfailure analysis world.


1. Khare J.B, Maly W, Thomas M.E, “Extraction of defect size distributions in an IC layer using Test Structure Data”, Dept. of Electr. &


Computer Eng., Carnegie Mellon Univ.,Pittsburgh,


PA,


Semiconductor Manufacturing, IEEE Transactions on


On, pp.354-368, Aug 1994.


2. Nathan Wang and Susan Li, “Application of


Metal stringer


3-D Transmission Electron Microscopy in Semiconductor Device Analysis, 1.2. EDFAAO (2008) 1:12-16,


3. David Su, et al, Microelectronic Failure


400 nm


Analysis: Desk Reference: 2001 Supplement,ASM International published, pp.85-95.


4. Oliver D. Patterson, Horatio Wildman, Doron Gal, Kevin Wu, “Detection of resistive shorts and opens using voltage contrast inspection”in IEEE/SEMI Advanced Semiconductor Manufacturing Conference, 2006, 327-333.


Fig.7. A plan-view Bright-Field STEM image  obtained after FIB cleaning cross-section. The  short defect is marked with red circle.


Fig.8. Cross-section bright-field STEM image  clearly reveals the metallic stringers at the  bottom of the snake-comb structure. This  image corresponds to the red-circled short  defect region in Fig. 7.


Optical Fault Isolation and Nanoprobing Techniques for the 10nm Technology  Node and Beyond


Martin von Haartman, Samia Rahman, Satyaki Ganguly, Jai Verma, Ahmad Umair, Tristan Deborde  Intel, Hillsboro, Oregon, USA


Resolution of optical fault isolation (FI) and nanoprobing tools  needs to keep pace with the device downscaling to be effective  for semiconductor process development. In this paper we  present and discuss state-of-the-art FI and nanoprobing  techniques evaluated on Intel test-chips fabricated on next  generation process technology. Promising results were obtained  but further improvements are necessary for the 7nm node and  beyond.


The continuous downscaling of the dimensions of electronic  devices for next generation semiconductor technologies is a  challenge for the electronics industry. Fault Isolation (FI) and  Failure Analysis (FA) teams have a key role in the process  development to find root cause to process and reliability  defects. Smaller device sizes result in process sensitivity to  even smaller defects, which is more challenging to electrically  isolate and characterize in FI/FA. Many FI tools rely on being  able to determine logic states or switching behavior of  individual transistors using optical techniques. This means that  the resolution of these techniques needs to roughly scale with  the same pace as the downscaling of the device dimensions: Moore’s Law. Currently, ICs based on 14nm technology is in  production at Intel [1]. This paper will discuss the recent  evolution and development of FI techniques, at Intel and  elsewhere, and present conclusions obtained from work on  Intel’s next generation process technology.


As the defects that can cause a malfunctioning transistor or  interconnect become smaller and smaller, further electrical and  physical isolation is necessary to be able to perform successful  physical failure analysis. The fault isolation process typically  starts with electrical testing, followed by optical fault isolation. If the region of interest is not sufficiently small, nanoprobing is  called for to electrically isolate the defect to a single electrical  node and determine the electrical defect type (normally short or  open). The end result of this work could typically be an open in  an interconnect stack or a short between two nodes. Our work  here is focused on the optical FI techniques as well as the  nanoprobing techniques developed to electrically isolate  defects on next generation process technologies.


The paper is outlined as follows. We will describe the key  optical FI techniques for 10nm technologies and beyond, which


includes infrared emission microscopy (IREM) and  Continuous-Wave Laser Scanning Microscope based Signal  imaging and Probing (CW-SIP) in the next section. We will  then discuss nanoprobing techniques, including SEM-based  nanoprobing techniques and atomic force probing techniques, followed by a conclusion of our work.


Optical FI techniques for 10nm and beyond


According to the well-known equation for diffraction limited  resolution of an aberration free optical system the image  resolution  can be written as


   =


0.61  


            (1)


where  is the wavelength and NA is the numerical aperture of  the lens (Rayleigh criterion). For an IREM system the  wavelength of the emissions cannot easily be reduced given the  constraints in supply voltage for modern semiconductor  circuits. However, one can improve the resolution by applying  short-pass filters (suitable range could be 1200nm to 1300nm), though at the expense of reduced signal-to-noise ratio. The  numerical aperture of the lens has increased from the aircoupled lenses to around 3.3 today on state-of-the-art solidimmersion lenses (SIL). Table 1 gives on overview of how the  numerical aperture, optical resolution and FI capabilities have  evolved over the last four technology nodes.


Table 1: Evolution of lens numerical aperture, optical  resolution, contacted gate pitch, and FI capability on  technology nodes from 32nm to 7nm.


||Technology node|Technology node|Technology node|Technology node|Technology node|
|---|---|---|---|---|---|

||32nm |22nm |14nm |10nm |7nm |

|Lens NA |1.4 (LIO) |2.6 (SIL) |3.0 (SIL) |3.3 |TBD |

|Optical resolution @  = 1500 nm |654 nm |352 nm |305 nm |277 nm |TBD – new solution needed |

|@  = 1064 nm |464 nm |250 nm |216 nm |197 nm |TBD |

|Contacted gate pitch |112.5 |90 nm [3] |70 nm [1] |~64 nm [4] |~50 nm [4] |

|Contacted gate pitch |nm [2] |90 nm [3] |70 nm [1] |~64 nm [4] |~50 nm [4] |

|FI capability |Fair |Very good |Good |Fair |TBD |

Technology node


(SIL)


The optical resolution at = 1500nm should be representative  of infrared (IR) emission from devices at the technology nodes  studied here, which will be further discussed below. The optical  resolution at  = 1064 nm is the best resolution that can be  obtained from state-of-the-art laser scanning microscopes  today. Note that although the optical resolution with the Liquid  Immersion Lens (LIO) on the 32nm technology only gave a fair  level of fault isolation, the defects were larger and easier to  detect in physical FA. For a similar level of capability on the  10nm node, more resources have to be spent to localize a defect (such as utilizing nanoprobing).


The following techniques have been developed for state-of-theart IREM tools:


i)


Differential polarization imaging and probing [5]


ii)


Short pass filters to improve resolution on (strong) emissions


iii)


SIL lenses with higher numerical aperture (up to  around 3.3 today)


iv)


Camera types with higher bandwidth than the  InGaAs camera that is standard in most systems  today. The higher bandwidth allows for higher  signal-to-noise ratio (though at the expense of  lower resolution), detection of IR emissions at  lower voltages, and being able to see emissions  due to other mechanisms than hot carriers (such  as thermal emissions). A good recent summary of  IR emission mechanisms can be found here [6].


The IREM technique has been successfully used in debugging  failures on Intel’s next-generation technology, including using  logic-state imaging (see Figure 1). This example shows  emissions from transistors with a fin-count of two. Note that  emissions from PMOS were significantly stronger than the  NMOS emission in this case which can depend on process  skews. By utilizing a 1300nm short pass filter the full width at  half maximum (FWHM) of the IR emission spots reduces by a  factor of ~0.8 compared to the unfiltered IR emission from the  InGaAs camera (upper wavelength limit around 1600nm) as  demonstrated in Fig. 1(g). This can be expected from Eq. (1) if  the IR spectrum is dominated by emissions near 1600nm. Earlier studies showed IR emissions from hot carrier effects in  MOSFETs are peaking above 1400nm [7] and are expected to  be further shifted to higher wavelengths as supply voltages  decrease with device downscaling. The downside is a reduction  of the emission intensity by a factor of three in this case when  using the 1300nm short pass filter, weaker emissions may not  be easy to detect anymore. As can be observed in Fig. 1(d) some  emission spots are below the noise floor after filtering.


However, fault isolation with IREM is getting more and more  challenging and an improvement in resolution is needed to be  able to use the technique effectively on future technology nodes (7nm and beyond). Further resolution scaling and being able to  detect and resolve emissions in minimum-sized devices is a  concern for coming technology nodes.


Figure 1: (a, b) IR emissions from inverters (predominantly  from PMOS) obtained on Intel test-chips using InGaAs camera  without filter. The change in state can be seen as the input is  changed from 0 to 1 and vice versa. (c, d) IR emissions from the  same inverters as in (a, b) but with a 1300nm short pass filter  applied in the detection path. (e) Abnormal high intensity  emission seen in IREM when the signal is shorted to Vcc and  the state is being forced to 0. (f) No emission observed for the  signal when state is 1. (g) Emission intensity profile taken at the  dashed lines in (b) and (d).


0.8 1


Normalized Intensity1.2


Pixel


1600 nm 1300 nm


0 0


Emission from


PMOS of inverter


Input short to Vcc, abnormal emission  when 0 forced.


Input short to Vcc, no  abnormal  emission  when 1 forced.


0 1


(f)


(e)


(g)


PO


h3-3


6b


:


Figure 2: (a, b) CW-SIP technique showing capability to isolate  faults on Intel’s next-generation technology at low bias (here


0.5V) where IREM is ineffective (1064nm laser was used). The  missing toggling suggests an open input to the inverter. (b) Missing toggling on a circuit from Intel’s 14nm technology  isolates the fail boundary. (c, d) A typical example where the  toggling of both NMOS and PMOS of a 2-fin inverter geometry (next generation technology node) has been successfully  resolved using a 1319nm (c) and 1064nm (d) laser. (e) Signal  modulation profiles across NMOS and PMOS in (c,d) as shown  with the dashed lines. The image with the 1064nm laser is  crisper with less signal overlap between devices (same power  level at DUT was used).


A key advantage with the CW-SIP technique (other common  names for this technique is LTM, LTP, LVI and LVP) over  IREM is that the signal level, here the modulation in the  reflected laser beam, scales roughly linearly with the voltage (due to dependence on the carrier density in the channel) whereas hot-carrier effects that generate IR emissions have an  exponential dependence on voltage [8],[9]. Thus, for low  voltage debug IREM may not generate any useful data as  emissions are typically below the noise floor, whereas CW-SIP  can give useful data with a supply voltage around 0.5V as  illustrated in Fig. 2(a). As shown in Fig. 2(b), a weak signal was  observed in the inverter near the fail boundary whereas no  logic-state emission or abnormal emission was detected in  IREM in this case. Fig. 2(c,d) depicts the ability to resolve both  NMOS and PMOS devices with next-generation features sizes  using CW-SIP. In contrast with IREM, the wavelength of the  laser beam used for probing with the CW-SIP technique can be  reduced. A 1064nm low-noise laser is standard in many CWSIP systems today, although lasers with slightly higher  wavelength potentially can give better results due to higher  signal-to-noise ratio. CW-SIP data using 1064nm and 1319nm  lasers are compared in Fig. 2(c,d). The 1064nm laser produces  better resolving modulation maps with less signal overlap  perpendicular to the fins, as expected, which is illustrated in  Fig. 2(e). A resolution improvement of 14% can be seen in this  image which matches reasonably well with the predicted 19%. Along the fins the resolution enhancement is less clear in this  example.


There are opportunities to reduce the wavelength even further  into the visible regime if one prepares ultra-thin samples as  outlined in the paper by Buetler et al [10]. Various polarization  imaging and probing techniques can also be applied on CW-SIP  systems to improve resolution. Also note that the SIL design for  narrowband CW-SIP systems could be simplified with an  aplanatic design compared to the broadband IREMs which


Intensity (a.u.)


could allow for higher NA. As demonstrated recently, CW-SIP  offers a solution to replace the logic-state-imaging capability of


-1319nm


IREM that can be scalable to future nodes: laser logic state


-1064nm


imaging [11]. The technique relies on being able to introduce a  fluctuation in the power supply voltage within the chip.


Wu


However, it’s inevitable that optical fault isolation techniques  eventually could run out of steam if Moore’s law continues for


another decade, even if shorter wavelengths into the visible  regime are used or advanced computational corrections and  analytics are applied. In another paper at this conference we  present how an e-beam can be used to produce a resistance  change much like the well-known optical OBIRCH technique. We could show a resolution of approximately 10nm for defect  isolation. Utilizing novel e-beam techniques could open up a  new era for fault isolation.


Nanoprobing techniques for 10nm and beyond


Nanoprobing has an integral role in the FI/FA flow today. Analysis of defects using a transmission electron microscope (TEM) requires a sample thickness in tens of nm, which sets a  requirement for how well some defects need to be isolated in


Toggling


missing


at 1st inverter:


Input open


Missing Toggling:


Fail boundary


Reference chain


Failing chain


Vss Vss  Vcc Vcc


Vss


Vss  Vcc Vcc


SMI intensity profiles


order to be successfully analyzed and characterized in physical  failure analysis. Thus, nanoprobing is many times performed  after optical fault isolation to further electrically localize the  defect. However, with the shrinking dimensions it becomes  increasingly difficult to position the probe tips on the contacts  and maintain good electrical connection through a  measurement. Moreover, the transistors also potentially get  more susceptible to damage such as electron beam irradiation.


The probing capability, including the abovementioned effects, was investigated on samples from Intel’s next-generation  technology. The transistors can be routinely probed with  negligible threshold voltage shifts at 500eV using advanced  SEM-based nanoprobing systems. By reducing drift in the  systems and optimizing sample preparation more than 5  minutes of stable electrical connection could regularly be  achieved when probing a transistor with minimum-sized  contacts as demonstrated in Fig. 3. The probes on the individual  contacts could sometimes stay in contact for tens of minutes. Probing techniques on AFM-based probing systems were also  developed. Figure 4 shows a conductive AFM scan of a lowlevel interconnect layer. The different contacts can clearly be  resolved and a leaky contact belonging to a gate could be  identified in the image. Conductive AFM maps continue to be  an important technique to quickly identify a suspected electrical  defect. Common for both probing techniques is the importance  of a sharp enough and durable probe tip with sufficiently low  resistance for the device under test. A good sample preparation  is also of utmost importance to achieve good results. However, further details on probe tips or sample preparation will not be  presented here.


Figure 3: Transistor measurements (Id-Vg) at two different Vds  taken over 5 minutes are shown. The measurement was  repeated with one minute interval and plotted in the graph.


Figure 4: A conductive AFM scan is shown. A leaky contact was  identified (red circle).


Both SEM- and AFM-based nanoprobing systems could  successfully be used to measure transistors and other structures  on Intel’s next generation technology. The choice between  these two probing techniques depends on the application. The  SEM-based probing systems have an advantage of direct visual  feedback of the sample surface, probe tips, and region of  interest. The DCG Systems nProberII incorporates built-in  cleaning solutions to maintain clean probe tips and sample  surface. Probe tip and stage drift is becoming a bigger concern  as contact sizes are scaled down. The drift can easily be  observed real time in an SEM-based probing system and is  therefore intuitively easier to compensate for. Sample quality is  also a bigger concern as the contact area for the probe tips is  getting smaller, which in turn requires probe tips with a smaller  radius. A built-in cleaning tool can save valuable time if the  sample and/or probe tips need cleaning prior to completion of  the probing. The main strength with an AFM-based system is  the ability to scan larger areas such as to collect conductive  maps, in which case drift is less of a concern.


As the resolution enhancements of optical fault isolation  techniques have lagged behind the downscaling for the last two  nodes, the uncertainty of the fault isolation increases resulting  in relatively larger region of interests for FA (i.e. they may  contain more transistors although the area may be smaller). This  puts an increased burden on nanoprobing teams to electrically  isolate the defect, which can be a laborious task. Techniques for  fast isolation of shorts and opens are of key importance to  deliver timely findings of defects to support process  development. Conductive AFM scan is one such method that  works well for some types of defects. Beam-based isolation  techniques such as Voltage Contrast and Electron Beam  Absorbed Current (EBAC) have also been used for a long time  but generally have more success for isolating opens [12,13]. A  new e-beam technique primarily used for isolating shorts was  recently developed and is reported in another paper at the  conference. This solved an important technical gap and gives  the fault isolation engineers a new method for faster isolation  of shorts. Further research into techniques not only for


resolution enhancement but with the goal in mind to produce  faster isolation of defects is encouraged.


State-of-the-art optical fault isolation and nanoprobing  techniques were developed and evaluated on novel Intel testchips fabricated on next-generation process technology. Promising results were obtained showing sufficient FI/FA  capability, but further resolution enhancement is necessary to  maintain high success rate and efficiency on future technology  nodes. This is an active research area with a diverse approach  into developing novel nanoprobing, optical, and e-beam  systems for next-generation fault isolation techniques.


The authors greatly acknowledge the support and contributions  to this work from our colleagues at Intel, no one mentioned, no  one forgotten.


[1] S. Natarajan et al, “A 14nm Logic Technology Featuring


2nd-Generation FinFET , Air-Gapped Interconnects, SelfAligned Double Patterning and a 0.0588 m2 SRAM cell size,” IEDM Tech. Dig. p. 71, 2014.


[2] P. Packan et al, “High Performance 32nm Logic Technology  Featuring 2nd Generation High-k + Metal Gate Transistors,” IEDM Tech. Dig. p. 659, 2009.


[3] C. Auth et al, “A 22nm High Performance and Low-Power  CMOS Technology Featuring Fully-Depleted Tri-Gate  Transistors, Self-Aligned Contacts and High Density MIM  capacitors,” Symp. VLSI Tech. Dig. p. 131, 2012.


[4] International Technology Roadmap for Semiconductors (ITRS), 2013 Edition, http://www.itrs.net.


[5] B. Niu, M. von Haartman, P. Pardy, and Mitch Sacks, “Differential Polarization Imaging and Probing [DPIP]: Seeing  and Probing the “Invisible”,” in Proc. ISTFA 2012, p. 190.


[6] T. Parrassin, S. Dudit, M. Vallet, A. Reverdy, and H. Deslandes, “Introduction of Spectral Mapping through  Transmission Grating, Derivative Technique of Photon  Emission,” in Proc. ISTFA 2014, p. 115.


[7] J. A. Rowlette, E. B. Varner, S. Seidel, and M. Bailon, ”Hot  Carrier Emission from 50 nm n- and p-Channel MOSFET  devices,” in Proc. IEEE LEOS Conf. 2003, p. 740.


[8] M. Gurfinkel, M. Borenshtein, A. Margulis, S. Sade, Y. Fefer, Y. Weizman, and Y. Shapira, “Study of hot-carrier  induced photon emission from 90nm Si MOSFETs,” Appl. Surf. Sci., vol. 248, p. 62, 2005.


[9] U. Kindereit, G. Woods, J. Tian, U. Kerst, R. Leihkauf, and  C. Boit, “Quantitative Investigation of Laser Beam Modulation  in Electrically Active Devices as Used in Laser Voltage  Probing,” IEEE Trans. Device Mater. Rel., vol. 7, no. 1, p. 19,


2007.


[10] J. Beutler, J. J. Clement, M. A. Miller, J. Stevens, and E. I. Cole, Jr, “Visible Light LVP on Ultra-Thinned Substrates,“ in  Proc. ISTFA 2014, p. 110.


[11] B. Niu, G. M. E. Khoo, Y.-C. S. Chen, and F. Chapman, “Laser Logic State Imaging (LLSI),” in Proc. ISTFA 2014, p.


65.


[12] “Beam-Based Defect Localization Methods,” E.I. Cole, Jr. in Microelectronics Failure Analysis: Desk Reference, 5th  Edition, ASM International pp. 406-416, 2004.


[13] K. Mizukoshi, T. Oyamada, A. Shimase, Y. Matsumoto, S. Yorisaki, and T. Majima, “Fault location using electron beam  current absorbed in LSI interconnects,” in Proc. Int. Meeting  Future Electron Devices 2004, p. 31.


Device Ioff Mapping: Analysis of Ring Oscillator   by Optical Beam Induced Resistance Change


Greg M. Johnson, Ziyan Xu, and Christopher D’Aleo


GLOBALFOUNDRIES, Hopewell Junction, NY, USA   gregory.johnson@globalfoundries.com


The ring oscillator is an important tool for inline monitoring  during technology development, as it contains the most  important front end of line technology features, is testable at  first metal, and generally shows a good correlation to SRAM  yield.  This work explores various failure analysis techniques  for the ring oscillator, during the development of 14 nm FinFET  technology.  OBIRCH, which is typically a DC technique, was  operated with voltages as low as 0.15 V to find multiple defect  mechanisms affecting the yield of ring oscillators, which  operate at a frequencies in the GHz range. In contrast to typical  photon emission analysis of ring oscillators, examines the  devices which are flipping on, it is here proposed that the  OBIRCH spots which are generated are indications of the Ioff, or the leakage of devices in the inverter stages across the ring. The results from this failure analysis approach enabled a rapid  improvement in yield not only of the ring oscillator itself but of  the SRAM.


With product-like layout design and high speed operating  conditions, the AC characteristics of the ring oscillator (RO) make it a more effective tool for assessment of technology  performance and process variations than isolated single FET  structures which are tested under DC conditions. The RO-based  test structure is therefore extensively employed during  technology learning cycles. The active and quiescent currents (Idda and Iddq) together with its frequency are the key  parametrics to provide RO electrical property and establish  power and performance benchmark.


Aggressive lithographic dimension shrinking, and the complex  integration scheme of FinFET technology, made 14 nm yield  development unprecedentedly challenging. In the early stage of  technology development, numerous defect mechanisms had to  be rapidly identified and corrected, long before an integrated  wafer made it to final or SRAM test. Thus a yield metric based  on measurement of a RO with 100 stages was a key measure of  program progress. The RO yield also is affected by issues of  design reliability, device centering and test accuracy.  Figure 1  shows a comparison of RO to SRAM yield for a series of


wafers. The comparison shows an excellent “envelope plot”


response, in which no wafer can get good SRAM yield without  accomplishing a critical RO yield.


Figure 1: Comparison, for 188 wafers, of ring oscillator yield  at Metal 1 to the SRAM yield at Metal 4.


Failure Analysis Approaches


Much of the literature regarding failure analysis of ring  oscillators involves photon emission microscopy (PEM).


Kash and Tang [1] introduced picosecond current imaging, a  movie with sub-nanosecond resolution, of photon emission, which has been used in characterization of ring Oscillators/  Ferrigno et al. [2] also utilized some static PEM, but showed  that dynamic PEM was required to see many defects.  Stellari, et al.  [3] showed that it was possible to detect gate delays, while  Shehata [4] recently were able to generate useful data as low as


0.4 V


Many of these techniques use detection methods that look for  the flipping inverters as the signal runs around the inverter. Our  early interest in the program, however, was specifically worried  about sources of leakage. It was discovered that for some of our  early hardware, a simple I-V sweep between the ground and  Vdd pads of the RO resulted in a curve that looked like that of  a leaky diode.  An intuitive approach was to stress a chip with  negative bias on the Vdd pad, and ground on the ground, and to  perform PEM under static conditions with no oscillation. This  technique was very successful at finding defects in the early  stage of the program.  Figure 2 shows an example of our  detecting a case of silicide encroachment using PEM at -2.2 V  with a charge-coupled device (CCD) camera. The PEM image  on the left of Figure 2 shows one inverter lighting up very  strongly, and the topdown delayered SEM image on the right  shows a case of silicide encroachment in a FinFET channel.  Typical results with this camera showed very little signal below


1.2 V, a voltage higher than the Vdd of the technology. Performing failure analysis at a voltage so much higher than the  technology voltage may not always be a good practice, raising


concerns about defects created or exacerbated during the test. Thus, we looked for low-voltage techniques to find fails in ROs.


Figure 2. a) PEM response @ 2.2 V with CCD camera of


PFET


defective RO.  b) delayered SEM view showing encroachment.


SEM


NFET


OBIRCH


As the yield improved, it was often the case that good and bad  chips would have the same I-V curve in the 2-point probe test. It was also evident from the curve shape that the field effects


that made for a PEM signal detectable by a CCD camera were  unlikely to be present. Laser-based techniques such as XIVA


(eXternally Induced Voltage Alteration) and OBIRCH (Optical  Beam Resistance Change) were utilized. Both of these


0.15 VOBIRCH IMAGE


techniques involve measuring changes in impedance of a circuit  while it is scanned by a laser scanning microscope.  The system  records pixels where resistance changed.  Figure 3 shows XIVA  response overlaid on top of a laser reflected image, for a case of  a gross short between two test pads.


Figure 3: Schematic view of XIVA localization technique.


Even though some preliminary results yielded useful data with  XIVA, the bulk of this study was based on OBIRCH, given the  greater sensitivity of the technique.  It is known that Sanchez et  al [5] were able to use OBIRCH in Dynamic Thermal Laser  Stimulation to OBIRCH to find dynamic and resistive defects, but this study was interested in continuing with a static  approach. It was discovered that with OBIRCH, we were able


to generate useful patterns at very low voltages, as low as 150  mV.  This is much lower than the voltages required to generate


DelayeredSEM view


PEM with the CCD camera available to us.  OBIRCH also has  the benefit of detecting defects unrelated switching  mechanisms, or affecting RO yield which were outside the bank  of 100 inverters. High-resolution OBIRCH scans demonstrate  that we can image all 100 stages, the enable NAND, and output  inverters in the ring oscillator.  By careful comparison of the XPEM@-2.2V


Y positions of NFET versus PFET devices in the inverter to the  spots in an OBIRCH scan we can see whether a particular  inverter were exhibiting a hotspot on its nFET or pFET side.  Figure 4 compares the SEM view with the typical hotspots seen  in OBIRCH scans on a good chip.


Figure 4: Comparison of SEM, OBIRCH, and overlaid images  showing the devices that have lit up during a static 0.15 V


OBIRCH analysis.


Defect Isolation Learning


Area which is partAreas not part of circuit path:


of circuit path:Often great changeNo change in R


This technique of low-voltage OBIRCH on ring oscillators was  used to uncover a number of yield-detracting defects in program  development of a finFET technology. Figure 5 shows one such  example.  On the left side of Figure 5, we see a few very large  spots, in contrast to the regular array of spots seen in the good  chip of Figure 4.  Topdown delayered inspection of the largest  spot revealed a case of CA (local tungsten interconnect) to PC (gate conductor) overlay problem. It is believed the short  caused not only the active device but also a large section of  surrounding “dummy” PC and CA lines to be electrically  active. Not only the device but also several nearby dummy  devices around it were part of the structure which was now  activated by OBIRCH. Hence a larger spot.


Delayered SEM view


Figure 5: Comparison of OBIRCH image to delayered SEM  view of a chip with gross misalignment.


Figure 6 shows the opposite problem—the OBIRCH pattern is


0.15 V OBIRCH IMAGEt


D2a日dsEMVI0w


missing a spot for a particular device. TEM cross section of this  spot showed a case of local underetch in the CA. With an open (or more highly resistive) contact, these devices did not carry as  much current as they should have and thus gave a greatly  diminished OBIRCH signal.


Figure 6: Comparison of OBIRCH pattern with missing device  spot and TEM section showing underetched contact.


Figure 7 demonstrates yet another problem— a large OBIRCH  spot completely outside of the array. In this case, a substrate  short was observed not in the main array of inverters, but  outside in a protect diode.  It’s unlikely that this defect would  have shown up in a photon emission scan of the RO.


Ring Oscillator Yield


Figure 7: Comparison of OBIRCH pattern with large spot  outside of the array with substrate short in supporting


Month


structure. .


In still other cases, the OBIRCH results indicated that all of the  PFET devices were lit up, and the spots are larger than normal, as depicted in Figure 8. Topdown delayered inspection of one  of the larger spots showed that there was silicide encroachment  in the channel. Due to process conditions, the silicide  encroachment only showed up in the PFET channels. It’s also  believed that the larger spot may be an indication of greater  temperature sensitivity, in that the OBIRCH effect was detected  by the system turned on while the laser beam was further away  than in the control sites.  Detection from further away leads to  a larger OBIRCH spot.


TEM Section


Figure 8: Comparison of OBIRCH pattern with only PFETs lit  up, and larger, with delayered inspection showing silicide


0.15 V OBIRCH IMAGE


encroachment.


lamella in a backside orientation to reduce the curtaining effect  on its surface.


Figure 1: SEM image of the part of the lamella prepared  inside Xe plasma FIB-SEM instrument immediately after the  final polishing of the lamella. STEM – bright field detector  was used for the imaging.


Measurement of the sample thickness by LayerProbe


Figure 2 is showing a typical thickness map, obtained by EDS  LayerProbe software module on another and much thicker (400 nm) TEM lamella, fabricated from the clean silicon  sample.  Such thick TEM lamella was fabricated to check the  quality of results from EDS LayerProbe software, mainly to  compare the lamella thickness measured by SEM to the  lamella thickness calculated by LayerProbe software from  EDS signal. The calculated thickness was around 400 nm too, which agrees well with the thickness measured by SEM when  viewing the lamella side on. The advantage of the thick lamella  is increased EDS signal and better uniformity of the thickness, but for the real applications in IC failure analysis the lamella  thickness has to be reduced significantly in order to be able to  see the lamella in TEM and to isolate small-size IC devices.


Measurement of Xe beam damage by LayerProbe


Figure 3 compares EDS spectra acquired on silicon part of the  400 nm thick lamella and the platinum protection layer. The  difference in the Xe content between the Pt layer and the rest  of the lamella is shown in the Table 1. While there is a  significant amount of Xe detected in the Pt protection layer, there is negligible amount of Xe detected in the Si part of the  lamella. This difference can be explained by the fact that for  deposition of Pt, (CH3)3(CH3C5H4)Pt gas was injected and  decomposed by a perpendicularly incident Xe beam. However, during the preparation of the lamella, the Xe beam  was nearly parallel to the lamella side walls and Xe ions were  deflected off the sides rather than being implanted (i.e.


200 nm


si


sidewall milling resulting in deflection of Xe ions compared to  the implantation for perpendicular milling). The negligible  presence of Xe in the silicon part of the lamella is of great  interest to our study, as for Ga FIB prepared lamellas, the  amount of the beam material detected by EDS is significantly  higher [8]. Therefore TEM lamella preparation by Xe plasma  FIB looks to be a very promising method in terms of reducing  the lateral damage of the lamella by Xe implantation and  lamella amorphization. When we compare this to our previous  studies on Ga ion beam induced deposition [10], where 16


Pt


at.% of Ga was measured in the deposit, it looks that the level  of Xe implanted in the protection layer is much lower (see 3  at.% of Xe in Table 1). The concentration of Ga, Pt and C in  Ga beam deposited Pt varies significantly for different authors  and process conditions [11], however significantly lower  concentration of Xe when compared to Ga is noticeable. The  concentration of Xe in the lamella itself is below the detection  limit of EDS technique (see Figure 3 and Table 1).


Table 1: Comparison of the atomic concentration of Xe and  other elements in the platinum protection layer and in the  silicon part of the lamella. Cu and Al stray signals from the  sample holder were not included.


|Element |Pt protection layer [atomic %] |Si lamella [atomic %] ||
|---|---|---|---|

|Pt |18 |0 ||

|C |79 |0 ||

|Si |0 |100 ||

|Xe |3 |0 ||

Figure 2: A thickness map of the thicker lamella, obtained by  EDS LayerProbe, where thickness around 400 nm was  measured by SEM. The thickness of the lamella was obviously  quite uniform. The left thicker part of the lamella was not  thinned by FIB.


10 kev


Figure 3: Two X-ray spectra are from (1 - gray) the Pt rich  protection layer and (2 - red) from an area just below IC  layers containing Si only, measured on 400 nm thick lamella  to maximize EDS signal. The Cu and Al peaks are stray X-rays  from the sample holder and grid post.


Measurement of Xe beam damage by TEM


Program Results


A stream of regular OBIRCH analyses on ROs identified many  yield detractors. Over time, we saw a steady increase in RO  yield, as depicted in Figure 9. Once the SRAM yield improved  to a subsequent point, it was clear that process changes were  needed to optimize yield for the SRAM, which in turn  exacerbated some problems in the RO. The process changes  account for the turndown in the red curve in the diagram.


Cross section


Ring Oscillator Yield progress by month


Figure 9: Progress in yield across month of program.


Understanding the spot pattern


In this paper, we propose that the OBIRCH spots are an  indication of the off-current leakage of each device in the RO. At first we assumed that the OBIRCH signal was merely  showing us which devices were on, but the new hypothesis was  reached after considering several key facts: 1) We know that  our OBIRCH resolution is good enough to detect in the X  dimension, whether the NFET or PFET side of any particular  inverter were showing a spot. 2) The pattern of devices which  should be "on" for our static test conditions is easily determined  under conditions of either static enabled, or static-enable pin  floating. This was confirmed by additional analyses with a  negative bias on the VDD pin, resulting in imaging of all the  PFET devices. 3) The actual spot pattern for on/off FETs  matches those FETs which would be off.  4) It is well known  that the Ioff for devices is often more temperature sensitive than  that of the Ion. 5) Some of our defect cases (Figure 7) showed  strong spots in the PFET devices which were leaking. 6)


Current should not continue to flow from the Vdd to GND pads  under static conditions. Therefore, we believe that our current  path is measuring leakage of the off devices.


This conclusion may better be understood by taking a closer  look at Figure 10.  In this diagram, we have (orange/green) a  view of four inverters in a row, running from left to right.  On  the top half of the diagram are four PFETS, and on the bottom  half, four NFETS.  If we carefully consider the wiring and the  behavior of a FET, we can determine which devices would be


on or off in our view here.  The green square and “on” denote


that one would have the first NFET on, then the second PFET  on, next NFET, next PFET.   The red blobs on the image are the  result of overlaying the actual OBIRCH pattern on top of these  devices (area sampled from red triangle below). We can see that  the pattern of OBIRCH spots lines up with the off devices.  Thus, this test finds leakage of off devices.


Figure 10: OBIRCH spots (red) overlaid on top of the diagram  for a particular inverter, demonstrating that the PFET spots are  much larger.  The diagram is also overlaid with the images  showing which devices would be on and off.


We have used a novel method for investigation of defect  mechanisms in RO process development. OBIRCH at 0.15 V  under static or DC conditions was able to find multiple defect  mechanisms. Furthermore, our explanation of the nature of the  spot generation mechanism shows that he have uncovered a  technique which may enable further characterizations of


screening a ring oscillator for device variability in Ioff current. Future work will investigate this relationship in detecting issues  like NFET vs. PFET strength.   Defects wrecking the yield of  AC constructs may sometimes be detected with DC localization  techniques.


[1] Kash, J.A.; Tsang, J.C., "Dynamic internal testing of  CMOS circuits using hot luminescence," in Electron  Device Letters, IEEE , vol.18, no.7, pp.330-332, July 1997


[2] Ferrigno, J.; Desplats, R.; Perdu, P.; Sanchez, K.; Beaudoin, F.; Lewis, D., "Dynamic Optical Techniques for  IC Debug and Failure Analysis," in Physical and Failure  Analysis of Integrated Circuits, 2006. 13th International  Symposium on the , vol., no., pp.320-326, 3-7 July 2006


[3] Stellari, F.; Zappa, F.; Cova, S.; Porta, C.; Tsang, James C., "High-speed CMOS circuit testing by 50 ps time-resolved


|||||cotu|
|---|---|---|---|---|

|VDD pad|PFET|PFET|PFET|PFET|

||SPOT|on|SPOT|on|

||on|SPOT|on|SPOT|

|GND pad|NFET|NFET|NFET|NFET|

luminescence measurements," in Electron Devices, IEEE  Transactions on , vol.48, no.12, pp.2830-2835, Dec 2001.


[4] A. Bahgat Shehata, F. Stellari, A. Weger, P. Song, H.


+ve


Deslandes, E. Ramsay, and T. Lundquist, "Novel NIR  camera with extended sensitivity and low noise for photon  emission microscopy of VLSI circuits", Proc. of  International Symposium for Testing and Failure Analysis (ISTFA), Houston, TX, 2014, pp. 6-11.


[5] Sanchez, K.; Desplats, R.; Beaudoin, F.; Perdu, P.; Dudit, S.; Valletc, M.; Lewis, D., "Dynamic Thermal Laser  Stimulation Theory and Applications," in Reliability  Physics Symposium Proceedings, 2006. 44th Annual., IEEE International , vol., no., pp.574-584, 26-30 March  2006


Vacuum Assisted ex situ Lift Out for Manipulation of FIB Prepared Specimens


Lucille A. Giannuzzi


EXpressLO LLC, Lehigh Acres, FL 33971 USA


Dustin Hess and Trevor Clark


The Pennsylvania State University, University Park, PA 16802 USA


Conventional ex situ lift out (EXLO) relies on adhesion forces  to pick up a specimen with a solid probe tip and place it on a  suitable carrier [1-3]. EXLO is performed outside of the FIB  instrument on a system basically consisting of a light optical  microscope, stage, and manipulator. The specimen is usually  picked from within the FIB trenches with adhesion forces  using a solid glass probe secured to a hydraulic manipulator. For scanning/transmission electron microscope (S/TEM) characterization, the specimen may be placed on a thin film  coated TEM grid [1]. The lift out and manipulation process  takes only a couple of minutes [2]. Known advantages to  EXLO include ease of use, high throughput and high > 90% success rates [2].


Recent developments in ex situ lift out include a new grid  carrier design and methods which allow fast and easy  manipulation of specimens without the need for a thin film  support [3-8]. A half grid with open slots allows specimens to  be manipulated to the grid itself. This allows for a better heat  sink and electrical path to ground. Since a carbon film may  inhibit certain S/TEM techniques such as high resolution  microscopy, energy filtered imaging, electron energy loss  spectroscopy or electron holography, the absence of this thin  film allows all S/TEM techniques to be performed. More  importantly, since no thin film support is needed, the specimen  can be further processed after manipulation. Once manipulated  to this new grid design, the specimen may be further processed  via FIB, broad beam ion milling, or plasma cleaning. In  addition, a thick specimen can be quickly and easily  manipulated to the slotted grid into a backside orientation, and  then FIB milled to a suitable thickness for S/TEM without  producing curtaining artifacts [3,4,8]. EXLO may also be used  to lift out very large specimens prepared using plasma FIB  instruments [3,7,8].


Vacuum micropipetting techniques using hollow probes have  been used for years in cell physiology and micro-robotics [9-11]. The shape of these vacuum grippers may be beveled, bent, or angled to optimize the surface orientation of the  micropipette with respect to the target [9-11]. The opening of  the pipette should be ~ 25-50% of the specimen face  dimension to be manipulated. The glass pipette may be sputter  coated with metal or a metal tip may be used to minimize the  electrostatic adhesion forces between the specimen and probe. Rai et al. [12] showed that vacuum-assisted ex situ lift out  could be used to pick up a FIB prepared specimen that was not


FIB milled free prior to manipulation to a 3 mm carbon-coated  TEM grid. Below, we combine a vacuum micropipetting  module with an ex situ lift out station, making use of both  suction vacuum forces and adhesion forces for the pick and  place of a FIB milled free specimen onto a slotted  EXpressLO™ grid [13,14].


Experimental Methods


Specimens from an InGaAs wafer were prepared for EXLO  using an FEI Quanta 3D FIB/SEM instrument. The specimens  were FIB milled free using 30 keV Ga+ ions for all steps with  final dimensions of ~ 15 m long x 5 m deep x 1 m thick.  Probes were pulled to a tip diameter of about 1m using  hollow glass rods with a one-step pull operation. The probes  were then beveled to an angle of 45o using mechanical  polishing to a long diameter of ~ 2-3 m. Debris from the  mechanical polishing was removed by dipping the probe tip in  ethanol in an ultrasonic cleaner for up to ~ 10 s. Alternatively, the bevel angle may also be produced by FIB milling the ends  of the probe tips. The probe was then mounted in a probe  holder at 45o and rotated to position the surface of the beveled  probe parallel or nearly parallel to the vertical FIB milled  specimen face. Fig. 1 shows a schematic diagram of the  correct orientation of the probe as well as both wrong and  incorrect orientations of the probe. When properly tilted and  rotated, the end of the beveled surface will appear as a straight  edge since the light optical microscope top down view will be  parallel to the beveled surface. Conversely, any combination  of an incorrect tilt or incorrect rotation of the probe will  produce an elliptical view of the beveled tip since the glass  probe is optically transparent. The end of the probe holder was  attached via a small diameter hose to a computerized vacuum  and air valve controller. In this way each valve may be opened  and closed quickly and without excessive vibrations from  manual valve operation.


Figure 1: Schematic diagram of hollow probe set up with  correct and incorrect orientation.


Results and Discussion


20 μm


Fig. 2 shows light optical microscope images obtained with


the EXLO system. In Fig. 2a, the hollow beveled probe


approaches the FIB milled free specimen and at this point the


vacuum valve is opened. The probe is centered with respect to


the specimen and as it nears the FIB milled free specimen, it is


pulled flat against the beveled probe face using the vacuum


suction as in Fig. 2b. The lift out or pick of the specimen is


achieved very easily and quickly in only a few seconds. This


geometry for manipulation to EXpressLO™ grids is detailed


below.


The specimen is lowered just above the EXpressLO™ grid. At


this point the vacuum valve is closed and the air valve is


opened to release the pressure to atmosphere using only


adhesion forces to hold the specimen in place. Alternatively, 20μmthe specimen may be exposed to flowing air (or nitrogen) to help release the specimen from the probe.  In Fig. 3, the specimen is placed on an EXpressLO™ grid in a bbackside orientation by leaning the specimen to the desired


geometry and manipulating the probe through the open slot of


the grid, allowing the specimen to stick to the grid surface via


adhesion forces. The extra tab of material indicating the top of


the specimen is evident in Fig. 3a showing that the specimen


is oriented in the backside geometry [3,5]. In Fig. 3b the probe


is lowered through the slot opening and the specimen comes to


rest and is placed on the grid support structure. After correct


placement, the specimen reflects brightly in the light optical 20 μmimage as per Fig. 3b. Thus, the Pick&Place™ is completed  and this specimen may be further FIB milled as shown below.


01


side viewLIJX


Light optical


microscope


(top down)


correct orientation


wrong orientation


view


b


Figure 2: Vacuum lift out of a FIB milled free specimen. (a) Vacuum valve opens. (b) Suction helps specimen adhere to  grid for lift out at optimum geometry.


Figure 3: Manipulation to the EXpressLO™ grid. (a) Center  the specimen above the open slot and lean to appropriate  orientation. (b) Probe slides through open slot.


It helps to lean the specimen into the desired orientation with  the probe prior to manipulating the probe through the open  slot as shown in the schematic diagrams displaying the grid  support area in Fig. 4. Since the specimen is approximately  centered on the probe, it is then easy to maneuver the probe  through the slot (see Fig’s 4a,b,c). In addition, the grid can be  rotated 180o and/or the probe angle can be changed after lift  out for manipulation and placement of the specimen into the  backside (or convention) orientation as per Fig. 4c.


45°


Figure 4: Schematic diagrams of manipulation to  EXpressLO™ grid support area. (a) probe with specimen  approaches grid. (b) probe leans specimen into a backside  orientation as it slides through open grid slot. (c) grid is  rotated with probe angle change after lift out.


Fig. 5 shows an SEM image of the same specimen in Fig. 3b  after secured by ion beam assisted deposition and then further  FIB milled. The specimen is now ready for TEM analysis. The  vacuum assisted lift out optimizes specimen positioning for  easy placement on the new EXpressLO™ grid.


Figure 5: SEM image of specimen in Fig. 3b after further  FIB milling.


Vacuum-assisted ex situ lift out of FIB milled free specimens  can be used to optimize geometry needed for manipulation to  new EXpressLO grids. Once on the new grid, an electron  transparent specimen may be analyzed directly by S/TEM or  other analytical technical. The specimen on these new grids  can also be further FIB milled or processed prior to analysis.


20°


[1]  L.A. Giannuzzi et al., “Focused Ion Beam Milling and  Micromanipulation Lift-Out for Site Specific CrossSection TEM Specimen Preparation,” Mat. Res. Soc. Symp. Proc. Vol. 480 (1997), MRS, pp. 19-27.


[2]  L.A. Giannuzzi and F.A. Stevie (eds.) Introduction to  Focused Ion Beams, Springer (New York 2005) pp. 201-228.


[3] Lucille A. Giannuzzi, Zhiyang Yu, Denise Yin, Martin  P. Harmer, Qiang Xu, Noel S. Smith, Lisa Chan, Jon  Hiller, Dustin Hess, and Trevor Clark, Microsc. Microanal. “Theory and New Applications of Ex Situ  Lift Out,” 21, (2015) pp. 1034-1048.


[4] L.A. Giannuzzi, “EXpressLO™ for Fast and Versatile  FIB Specimen Preparation,” Microsc. Microanal. Vol. 18, S2 (2012) pp. 632-633.


[5]  L.A. Giannuzzi, “Routine Backside FIB Milling With  EXpressLO™,” Proc. ISTFA (2012) pp. 388-390.


[6]  L.A. Giannuzzi, “Enhancing Ex-Situ Lift-Out with


EXpressLO,” Microsc. Microanal. Vol. 19, S2 (2013) pp. 906-907.


[7]  L.A. Giannuzzi and N.S. Smith, “ex situ Lift Out of  Plasma Focused Ion Beam Prepared Site Specific  Specimens,” Microsc. Microanal. 20 (S3) (2014) pp. 340-341.


[8]  Lisa Chan, Jon H. Hiller, Lucille A. Giannuzzi., “ex  situ Lift Out of Plasma Focused Ion Beam Prepared  Site Specific Specimens,” Proc. ISTFA (2014) pp. 283-286.


[9]  K.T. Brown and D.G. Flaming D.G., (eds) (1986) Advanced Micropipette Techniques for Cell  Physiology, Chichester, John Wiley & Sons, Ltd. pp. 132-133.


[10]  Wolfgang Zesch, Markus Brunner, Ariel Weber, “Vacuum Tool for Handling Microobjectswith a  Nanorobot,” IEEE Intl. Conf. on Robotics and  Automation, 2 (1997) pp. 1761-1766.


[11]  Dragan Petrovic, Gordana Popovic, Elias  Chatzitheodoridis, Oscar Del Medico, Ana Almansa, Franz Sümecz, Werner Brenner, Helmut Detter “Gripping Tools for Handling and Assembly of  Microcomponents,” 23rd Intl. Conf. on  Microelectronics, IEEE, 1 (2002) pp. 247-250


[12] Raghaw Rai, Eric Chen, Yu Zhang, Donald Nedeau,


Yandong Chen, Wayne Zhao, Seng Keat Lim, ZhiHong Mai, and Jeffery Lam, “Automated TEM Sample  Preparation from Smaller Device Structure Regions of  Semiconductor ICs using Inline Dual-Beam CLM+ and  TEMLink 150,” 19 (Suppl 2) Microsc. Microanal.


(2013) pp. 900-901.


[13] EXpressLO grids and lift out method are covered by


U.S. Patents 8,740,209 and 8,789,826.


How Xe and Ga FIB differ in inducing lateral damage on TEM samples


Tomáš Hrnčíř, Jozef Vincenc Oboňa, Martin Petrenec


TESCAN Brno, Libušina třída 1, Brno, Czech Republic


tomas.hrncir@tescan.cz, Tel. +420 530353468


Jan Michalička


TESCAN ORSAY HOLDING, Libušina třída 21, Brno, Czech Republic


Christian Lang


Oxford Instruments Nanoanalysis, Halifax Road, High Wycombe, UK


Reducing FIB induced damage on TEM samples is very  important in order to preserve the sample structure, especially  on modern semiconductor devices. We have compared the  damage caused by Ga ion beam to our measurements of the  damage caused by Xe ion beam and came to the conclusion  that Xe ion beam induced damage is significantly lower at  30 keV beam energy. This has been proven by several  independent analytical methods. Our results show that TEM  sample preparation by Xe ion beam causes less amorphous  damage and increase the quality of the lamella and in many  cases it will allow to prepare the lamella by finishing it even at  30 keV, without the final cleaning step at the low beam energy. Final polishing step by Xe beam at beam energy 3 keV further  reduces the amorphous layer, but the difference against Ga  beam is not so significant like at 30 keV.


The critical dimensions of semiconductor devices are now so  small that Transmission Electron Microscopy (TEM) is  routinely used for precise failure analysis. To be able to  investigate structures on the nanometer and sub-nanometer  scale by TEM, ultrathin TEM samples (lamellae) have to be  prepared that contain the fault in question. Optimal thickness  of the lamella depends on the energy of TEM beam and the  size of the analyzed structures. For the latest technology nodes  a final thickness of less than 20 nm is frequently required by  failure analysts at present. This requires very precise, sitespecific techniques and workflows for TEM lamella  preparation. Focused Ion Beam (FIB) combined with Scanning  Electron Microscope (SEM) fulfils the demanding criteria of  device failure analysis and therefore has become the standard  tool for the preparation of TEM lamellae in this field. However, TEM lamella preparation by FIB induces significant  artifacts, not present in the original sample, which can make  failure analysis on such samples more difficult or even  impossible. These artifacts include surface amorphization, implantation of the beam ions into the lamella surface or  creation of intermetallic compounds with Ga+ ions [1]. While


these effects are very well understood for Ga FIB now, there is  not sufficient knowledge about use of Xe+ ion beam for TEM  lamella preparation.


Xe+ ion beam offers two potential advantages for TEM sample  preparation. The first one is the milling rate. The milling rates  achievable in most Ga+ FIBs restrict the maximum TEM  lamella dimensions in both width and height to tens of  microns. Novel plasma FIB-SEMs enable milling rate more  than 50 times faster than conventional Ga+ FIBs [2]. Therefore  lamellae can be prepared rapidly with dimensions of hundreds  of microns [3], saving time in isolating defects. The second  advantage of Xe+ ion beam is the potential for less lateral  damage of the lamella surface. While one may expect higher  milling rates to induce greater damage, in actual fact  a reduction of the surface amorphization by approximately  25% on the silicon sample has been shown [4]. Furthermore, formation of intermetallic compounds does not occur with a  Xe+ ion beam due to non-metallic, inert character of the ions. Xe+ ion beam implantation can be reduced too, due to the  bigger size of Xe+ ions when compared to Ga+ ions. In order to  establish whether these potential advantages can indeed be  realized for TEM lamella preparation, this work focuses on the  comparison of TEM lamella sidewall damage by both beams. As a significant amount of data already exist for the  amorphous damage on Si by using Ga+ ion beam based  preparation [5, 6, 7], we will focus here on Xe+ ion beam and  draw comparisons to the published results. The amorphization  of the surface as well as implantation of Xe+ ions is studied by  SEM and TEM imaging and complemented by materials  analysis using Energy Dispersive X-ray Spectroscopy (EDS) and High Resolution TEM (HR-TEM) analysis of amorphous  layers. The consequences for TEM lamella preparation will be  discussed and practical workflows for TEM sample  preparation inside plasma FIB-SEM will be outlined.


The lamella quality is critical in order to obtain good quality  TEM images. Artifacts created during the preparation process  need to be understood and eliminated as far as possible. Here  we investigate lamellae prepared in TESCAN FERA3 and  XEIA3 plasma FIB-SEM instruments. The HR-TEM analyses  have been performed on a Carl Zeiss LIBRA 200FE TEM


microscope at beam energy 200 keV. In order to accurately  characterize the lamella thickness and implantation of beam  ions during the preparation process, we use in-situ EDS  analysis in combination with special software to calculate the  lamella thickness (AZtec LayerProbe, Oxford Instruments). This method has been shown to give accurate results for Ga+ prepared lamellae of a range of materials [8]. The LayerProbe  software refines a starting model of the sample structure  against the EDS spectra to calculate the film thickness and  composition of the layers. This technique can also be used to  detect the presence of beam ions in the lamella surface and  calculate the thickness of such a damage layer, assuming that  the concentration of the implanted beam ions is higher than the  detection limit of the method (~0.1 wt%). As this technique  has already been proven on Ga FIB [8], its application to  samples created by Xe FIB is a logical next step.


The measurement of FIB induced lateral damage in silicon was  traditionally measured by using TEM [5, 6, 7] or by using  Scanning Probe Microscopy (SPM), while still comparing  results to TEM [9]. While these methods offer a possibility to  perform very precise lateral damage measurement, their big  disadvantages are that they are by their very nature destructive. It is therefore impossible to perform any corrective action on  the sample after the measurement to mitigate the damage. This  requires the measurement of the lateral damage inside FIBSEM instrument during TEM lamella preparation process. The  use of a readily available EDS detector in combination with  the LayerProbe software offers a straightforward way to assess  the lamella quality in-situ and in a non-destructive way. To  prove the quality of the measurement by EDS method, the  comparison of results measured by EDS and by TEM will be  shown.


An example of lamella from IC sample


An example of a prepared TEM lamella is shown on Figure 1. The lamella was prepared by using a well established in-situ  lift-out procedure. Before welding the lamella to the TEM grid  it was rotated into the backside orientation to reduce the  curtaining effect during the final thinning and polishing  process steps. The whole milling, in-situ lift-out and final  polishing procedure has been performed by using Xe plasma  FIB at the beam energy 30 keV. The lamella was polished at  FIB beam current 100 pA. The thickness of the silicon part of  the lamella in the area above IC layers was approximately  100 nm, when measured by SEM, and 96 nm when measured  by LayerProbe software, which gives the excellent agreement  between these independent methods. We show that even  though the lamella was polished at Xe FIB beam energy  30 keV, the damage of the surface is still acceptable for  observation of IC layers. This may not be the case when using  Ga FIB at the same beam energy, where the final polishing is  usually carried out at considerably lower energies. The layer at  the bottom is the Pt protection layer, which was located on the  sample surface prior to FIB milling and before polishing the


Beyond TLP and IEC gun simulators, it is possible to use other  methods to generate transient pulses that may more readily  represent specific conditions under study, such as charged  board events (CBE). In this paper we present a novel way to  use field collapse event (FCE) test method for a pulse


generation [4]. When this field rapidly changes, the transient  current pulse travels through the DUT ground connection. At  the same time, this will create current flow along the PWB.


In this study we apply the electrostatic field collapse charging  and discharging principle into the automated EMC scanning  technology. The main benefit here is that the ESD source is  just a simple charged metallic induction plate, and the  discharge is made by grounding the induction plate by using a  relay switching. Thereby, the setup is simpler than when using  ESD gun, considerably less expensive than a TLP system, is  more easily interfaced to an arbitrary DUT/PCB/Enclosure, and the shape of the pulse can be adjusted to more closely  resemble a realistic test scenario. Additionally, the groundreferenced DUT can be in operation during the measurements  without concern for pulse generator ground loops and  impedance mismatches.


In this paper we present the experimental test setup in Chapter  II, an operation principle of the method and show example  measurement results in Chapter III


Measurement Method


A. Test setup


The measurement setup used in this study is presented in  Figure 1. The DUT is above an induction plate with a size of  255 x 150 mm and the plate is connected to a high voltage


supply through a 1 MΩ resistor. The DUT is separated with


thin 0.127 mm thick dielectric from the induction plate and the  induction plate is separated with 2.718 mm thick dielectric  from the ground.


The induction plate is grounded via a relay switch which is  turning on and off based on the relay control signal. Each time  the relay closes, the induction plate will discharge into the  electrical ground and the changing E-field pulls current  through the DUT ground connection. When the relay is open  the high voltage supply charges both the induction plate and  DUT in few milliseconds period.


Parallel to the pulsing a near field probe is moved with small  incremental steps in a grid above the DUT and an oscilloscope


is used to record field densities in each position. The


.tran 0 200n 0 10p


R_IndC_DUTPULSE(500 0 0 0.1p 1200n)


oscilloscope is triggered by a current probe measuring the


{R_Ind}{Cdut}.step param Cdut list 100p 200p


relay signal or the discharge current from the induction plate.


.param Lind 50n


Two sets of scans is made with 150 points each, one with the


Clnd


{Cind}{Lind}{Ldut}.param R_DUT 2.param R_Ind 102L_IndL_DUT_wire.param Ldut 50n


H-probe in the "X" orientation and one in the "Y” orientation. With this array of X/Y orientations of an H-Probe on the 2D


R_DUT_wire.param Cind 50p


grid over the PCB, this scope data can be used to compile a


V1{R_DUT}


real-time animation of current flows in the system due to the  contrived event.


The measured current values in each step position can be post  processed with computer to construct a Fast Fourier Transform (FFT) information. The FFT information provides signal  power spectrum information. This data can be useful with  system level EMC analysis.


The amplitude of the ESD current pulse is controlled by  adjusting the induction plate charging potential. At the same  time it is necessarily to verify that the RC time constant of the  induction plate is at least three-four times shorter than the relay  switching period. This is also affected by the PWB ground  contact, and a high impedance ground contact would slow  down the pulse stepping speed.


E- and H-fields can be measured with different probe types  based on the frequency range and directional information  required.  Omnidirectional E-field probes can be used to map  charged areas of interest, such as isolated stackup areas which  may store charge for secondary breakdown events. Shielded  H-field loop probes can be used to extrapolate current flow  from vector direction calculations.


B. Equivalent circuit


An equivalent circuit of the FCE simulation setup is presented  in Figure 2 [4]. There are two RLC circuits affecting the  realized DUT stress current waveform. However, the DUT  follows the voltage induced by the induction plate, and  thereby, the inductance and resistance of the induction plate  ground connection affects also on the DUT stress waveform. In addition, the capacitance of the induction plate defines the  amount of charge stored in the test setup.


00Oscilloscope


m


Eor H field probe


Relay


control


Dielectric


InaxYZrobot


hDielectricPCB七RHV supply


Figure 1:  Measurement setup (with Spectrum Analyzer, or  Oscilloscope capture device)


Figure 2: An equivalent circuit used to construct and simulate  the DUT current stress waveforms.


Simulations are an essential tool to fine tune test setup  parameters. For example, the capacitance, resistance and  inductance values can be estimated based on the simulations. Here the target can be to find a test setup producing similar  stress waveform as observed in a real world ESD stress event. Table 1 presents the main test setup parameters shown in  Figure 2 and explains at a general level how those affect the  DUT current waveform. RC circuits define the pulse rise time  and oscillation frequencies, whereas resistance values will  mostly effect on the amplitude and damping factor of the  current waveforms.


The simulated ESD current waveforms through the DUT  ground wire are presented in Figure 3 based on the Figure 2  equivalent circuit parameters. Here the capacitance of the  DUT changes between 100 pF and 200 pF, and the stress  waveform varies based on the capacitances. In this case the  total charge moving through the DUT ground contact is 61 nC  in the first run and 100 nC in the second run. Similarly, the  peak current increases from 16 A up to 19 A when the  capacitance increases.


Table 1. FCE parameters


|R_ind and |Low values make waveforms to oscillate and increases the current amplitude. |
|---|---|

|R_DUT_wire |High values create damped pulses and decreases the current amplitude. |

|C_DUT |High values increases the current |

|C_DUT |amplitude and decreases the oscillation |

|C_DUT |frequency. |

|C_ind |High values may decrease the current |

|C_ind |amplitude and decreases the oscillation |

|C_ind |frequency. |

|L_ind and L_DUT_wire |High values decreases the current |

|L_ind and L_DUT_wire |amplitude and decreases the oscillation |

|L_ind and L_DUT_wire |frequency. |

|L_ind and L_DUT_wire |Low values increases the current |

|L_ind and L_DUT_wire |amplitude and oscillation frequency. |

Ground platePCB Ground connection


sonsor Current


Figure 3. Simulated example DUT current waveforms during  an FCE discharge.


C. An experimental measurement setup


The basic experimental test setup is presented in Figure 4 for a  simple DIMM memory module. This configuration differs  only slightly from an existing current reconstruction scanner in  that the injection control of firing the TLP is replaced by a  simple relay to ground the induction plate. The choice of  trigger point for the oscilloscope is critical for assembling  meaningful video frames of the FCE.  In the time domain the  scope cannot be triggered from the probe response, because  the flight time of pulses vary geographically on the DUT with  respect to the ground point.   Likewise the scope should not be  triggered from the control signal to the relay as the mechanical  closing time and bouncing may be unrepeatable. A current  probe on the DUT grounding point, or on the relay discharge  contacts may provide an apparatus-independent trigger timing  that is actually related to the discharge activity on the DUT, and is reasonably independent of fixturing and probe position.


In Figure 4 a CT1 current probe along the DUT ground wire is  used to trigger the measurement. With higher stress levels the  probe should be moved on the ground plate to prevent EMI  coupling. Again, an advantage of the ground referenced nature  of this methodology allows the use of low cost resistor shunt  current probes on the relay contacts and/or DUT ground  connection.


The DUT ground point can be selected based on the stress  scenario. For example, the ground point can be an external


interface signal pin where the efficiency of an EMC/ESD filter  is tested. In this example case the DUT ground point is an  arbitrary pin of the DIMM module where a charged board  might make contact with an external circuit or tool.


Figure 4: A basic experimental measurement setup showing  the DUT and DIMM DUT ground wire with a CT1 current  probe. The H-field probe is above the DIMM module.


Measurement Results


An example measurement result is presented in Figure 5 for  the DIMM module. The figure contains peak H-field values  with color and the field direction information with arrows. The  ground point is on the top side middle of the module and the  highest field strength is observed at that point. The measured  field values are higher on the left side of the module, whereas  fields stay low at the right lower corner area which indicates a  meaningful difference in the conduction and coupling paths of  the different areas.


On top of the peak field values, it is possible to reconstruct  field details in each time step by post processing the measured  time domain data. Thereby, field values can be presented as a  video record showing similar data as shown in Figure 4. That  helps to resolve possible EMC problems due to the disturbance  signal reflections inside DUT during a transient event.


sepd ntSSI SOWL


t


5dars.


813


A3 4 5


|6|1 。|5|10|XSteps|15|20  Kce 0M Demo & 126V|25|
|---|---|---|---|---|---|---|---|

3 510


1P


Figure 5: Measured strength and direction of H-fields on a  DIMM memory module.


Another test case considers the more complex behavior of a  phone LCD panel “face down” on a ground plane (See Figure  6), much as would be seen when a smartphone is placed “display down” on the IEC61000-4-2 HCP and zapped  through the case/chassis.   This is a very challenging test as the  large surface area of the display and the very thin dielectric  creates a high capacitance and potentially large displacement  currents through the display.


0.0110


61080EO40


60


an TPFO,


0.0055


Figure 6: LCD Panel on SFCE Platform


ReconmosePRAGMA


0,0000


DESIGN


0.220


Unfortunately, full implementation details of the display and


0.165


zho


F-HTE00A673-090-0291-2 560 ms


touch panel (layout, stackup, conductivity of traces, etc.) may


0.110


not be readily available to the system designer for full 3D


0.055


simulation, and the computing power required is substantial.


1 25


0.000


-0.055


In this configuration the Field Plate is charged as before, and


the LCD Flex GND return is grounded to the ground plane.   5


-0.110


Hx and Hy are again imputed by the right-hand rule at the v


a S0oren


102030405060-0.165


surface of the scan plane to reflect the currents flowing in the


-0.220


flex conductors and the LCD traces, while Hz detects fields  flowing perpendicular to the scan plane.


Figure 7 shows one particular instant of Hxy scans during an  FCE event where the DUT pulse current is traveling through  the flex circuit (top left, direction down).   In the Hz plot (Figure 7, bottom) two circles highlight field densities of


opposite polarity approximately at either end of the chip-onglass LCD row/column driver chip resides.   Analyzing these  fields over time (via animation of each time-sampled frame) can assist the ESD protection designer confront the resulting  aggressor pulses and resonances actually seen by the chips.


Interestingly, while the implied current flow measured by the  Hx and Hy pair in the flex circuit (top left) are obvious, and  supported by the right-hand rule cross section seen as expected  in the same area on the Hz plot, the Hz fields observed  between the LCD conductors and the ground plane are not  readily apparent on the Hx/Hy plots.   It is not clear if this is  indicative of the nature of the displacement currents in the  panel, or a characteristic of the coupling between the LCD  conductor sheet resistances, flex copper traces, and the two  different Hx/Hy and Hz probes.


0.0495


XY PLOR20150706-0k02Fbx4-1z3501060-028 #151:t4-2.5m


0.0440


0.0385


0.0330


蒙5 10


0.0220


0.0165


0.0275


Figure 7: Phone LCD Hxy and Hz scans


While the FCE pulse shape can be adjusted with stack-up and  discharge network parameters to emulate real discharge  conditions of such a configuration, TLP and other 50-Ohm


pulsers have also been utilized in current reconstruction


1100TE


applications, injecting a fast rise time into the point of interest,


SET


with-respect-to the ground plane underneath.


!"


Reconfiguring the scanner for TLP requires connecting the


center-conductor of the pulser to the DUT injection point (again, using the flex circuit ground) and the shield of the  pulser to the ground plane directly underneath the DUT


日


(previously the Field Plate.)


--HEP 1572 mO+TLP-S24 412 8)1-069


Even with dramatically different aggressor pulses applied, the


inherent resonances and couplings within the DUT and to the  adjacent metal plane are readily apparent in the scanning.


!'s to


Consider the snapshots below extracted from two critical  peaks in the same LCD DUT, but one using FCE (Figure 8) and one using a modified 10ns TLP [1] (Figure 9). Note that  the layout features and discharge paths are remarkably similar.


X560zs


FPTSu3 20Lom mnrLs-oe32 z--


Figure 8: 300V FCE Hz scan at pulse peak (red z-up, blue z2s


down)


Aka Gom ChOmey 2 PLOT:20150728-NoKGIsFIX5-Hz300VTLP-024-022#236:tm 1.709


Scwedps2025008062542atage306.06c5tings,283odues 500stune


is


2030


5o


FT 2200d-00-2522 30 182


15


102030405060


x500m


Figure 9: 300V modified TLP Hz scan at pulse peak (red z-up,


0 so


blue z-down)


The time domain capture samples for each point in the scan  grid can be used to calculate an FFT for the point, and then  construct a series of plots that show relative spectral  distribution at frequencies of interest.    Figure 10 shows a  comparison of the relative intensity (in arbitrary dBmV  sensed) between the same FCE (top) and TLP (bottom) scans  showing relative local excitation at 40MHz.


Figure 10: Hz FFT comparison at 40MHz (300V FCE top,


NoHa em 30CE


cametaom 3050106oncapsetage 300 Ou SetngsM0mmhum,Seuhune a Casa CNOres Z PLOT:20150706-NokGlsFix4-Hz300VFCE-048-022@201:t= 0.0ns


300V TLP bottom)


The similarities at this low frequency using dramatically


different aggressor pulses  suggests that the patterns are  indicative of natural resonances in the DUT, which helps


。15


validate design decisions.


10 5


Figure 11 shows dramatically different contours at 620MHz, owing to the higher spectral content of the fast rise time of the


TLP pulser, and potential impedance mismatch ringing.


Figure 11: Hz FFT comparison at 620MHz (300V FCE top, 300V TLP bottom)


In reality, an actual discharge event will be defined by the  system configuration under test.  FCE provides a flexible  method for such inherent emulation.


E- and H-fields on the DUT can be measured with a near field  scanning method to identify possible EMC immunity and  emission challenges. These fields can be measured from an  operating system during normal operations and also by using  external noise or transient pulse generators such as TLP  systems or IEC guns.


In this paper we present a novel way to generate transient  external pulses with an electrostatic field collapse principle. The main benefit here is that the test setup is simple to  construct with very low cost tools and that the DUT can be  fully operational during the transient events. The only special  RF tool required is an oscilloscope or a spectrum analyzer and  EMC scanning servos with E- and/or H-field probes. However, in this study we apply the field collapse method to existing  fully automated near field scanning equipment without the  need for expensive TLP generators and precision inductive  current probes.


In this paper we present an experimental near field  measurement setup and sample measurement results for a  DIMM memory module and for a mobile phone display  module. Based on the measurement results the method is  capable to show transient current paths on a DUT during


different phases of the stress waveform. This information  enable system EMC designers to analyze and improve system  level designs.


[1] Wei Huang; Dunnihoo, J.; Pommerenke, D., "Effects of  TVS integration on system level ESD robustness," Electrical Overstress/ Electrostatic Discharge Symposium (EOS/ESD), 2010 32nd, vol., no., pp.1,6, 3-8 Oct. 2010


[2] W. Huang, D. Pommerenke, J. Xiao, D. Liu, J. Ming, G.


Muchaidze, S. Kwon, “A Measurement Technique for


ESD Current Spreading on A PCB using Near Field


Scanning”, Present on 2009 IEEE International  Symposium on EMC, Austin, Texas, Aug. 17 – 21.


[3] M. Giorgi, W. Huang, M. Jin, P. Shao, D. James, D. Pommerenke, “Automated Near-Field Scanning to  Identify Resonances”, EMC Europe 2008, Hamburg, Germany, Sep. 8-12.


[4] P. Tamminen, T. Viheriäkoski, T. Reinvuo, L.  Sydänheimo, L.  Ukkonen,”Field Collapse Event ESD  Test Method”, paper 2B.2, EOS/ESD Symposium, Tucson  USA, Sep 2014.


Extending Electrical Scanning Probe Microscopy Measurements of  Semiconductor Devices Using Microwave Impedance Microscopy


Benedict Drevniok, St.John Dixon-Warren


Chipworks Inc, Ottawa, Ontario, K2H 5B7 Canada  bdrevniok@chipworks.com


Oskar Amster, Stuart L Friedman, Yongliang Yang


Prime Nano Inc., Palo Alto, CA 94306, U.S.A


Scanning microwave impedance microscopy was used to  analyze a CMOS image sensor sample to reveal details of the  dopant profiling in planar and cross-sectional samples. Sitespecific capacitance-voltage spectroscopy was performed on  different regions of the samples.


Continued advancement of semiconductor manufacturing  drives development and refinement of analysis techniques  used in the failure analysis community. Scanning Probe  Microscope (SPM) based electrical measurement techniques  such as Scanning Capacitance Microscopy (SCM), which has  existed for more than three decades and is based on a sensor  orginally developed by RCA for video disk applications [1], have shown value in many circumstances, but suffers from  limitations including non-monotonic response to the dopant  level stemming from the requirement to measure differential  capacitance.


Scanning Microwave Impedance Microscopy (sMIM), which  directly measures the real (sMIM-R) and imaginary parts (sMIM-C) of the impedance of the SPM tip and sample  interface, adds significant electrical measurement capability  over existing techniques while simultaneously producing  dC/dV measurements similar to conventional SCM. At the  same time, sMIM’s direct measure of sMIM-C and sMIM-R  provide (i) a more systematic dependence on doping  concentrations in the range of 1015 cm-3  to 1019 cm-3 ii) information on linear regions of the sample, such as oxides, metals and polysilicon structures. Examples of these  capabilities are illustrated in this paper with planar and crosssectional measurements in the photocathode region of an  image sensor device using some of the imaging channels  available when using sMIM.


Figure 1: Diagram of a Scanning Microwave Impedance  system and the output signals. Of chief importance in this  paper are the sMIM-C and dC/dV signals


Scanning Microwave Impedance Microscopy couples 3 GHz  microwave signals to the apex of the sMIM probe via a microfabricated coaxial transmission line in a custom-designed, shielded, metal sMIM probe (Fig. 1). The sample is scanned  using contact-mode AFM and the reflected microwave signal  from the tip-sample interface is measured by the sMIM  electronics. Two signals corresponding to the in-phase and  out-of-phase reflection are collected to form images. When  properly configured, one signal is dominated by the  capacitance of the tip sample interface and the other signal is  dominated by the resistance of the tip-sample interface, hence  the images are labeled sMIM-C and sMIM-R. For linear  samples, these signals vary with the local conductivity and  permittivity of the sample respectively. For doped  semiconductors, the depletion or inversion layer depth  contributes to the signal. By modulating a bias voltage applied  between the tip and sample, dR/dV and dC/dV signals can be  measured using lock-in techniques. The dR/dV and dC/dV  signals are only non-zero in regions of the sample where nonlinear materials, such as a doped semiconductor, produce  voltage dependent changes in the R and C channels of the tipsample interface.


Sample Details


A front-side illuminated global-shutter CMOS image sensor  was used to illustrate monotonic sensitivity to a broad range of  doping concentrations as well as contrast from linear regions  such as shallow trench isolation, polysilicon and dielectrics. The basic device structure of a CMOS image sensor using a


pinned photodiode has been described in a recent review [2].  SEM images of the commercial device are presented in Fig. 2. The sample features 3 µm pitch pixels. The cross-sectional  SEM image in Fig. 2(B) is taken along a 45 degree angle as  illustrated on the planar SEM image in Fig. 2(A). Key features  of the structure are labeled on the images.


Figure 2: SEM images of the area of interest: A) A planar  composite image at two different layers of the sample. The  polysilicon layer on the left merges into the diffusion layer on  the right. B) A cross-sectional view of the samples taken along  the line indicated in (A).


The photocathode region of CMOS image sensor devices  contain doped features that exhibit a large dynamic range in  dopant concentrations. It is known that a large dynamic range  in dopant concentration can lead to non-monotonic behavior in  SCM [3]. Using sMIM-C we see monotonic behavior over the  whole range of concentrations [4]. In this paper, three  channels of information are presented: sMIM-C, dC/dV  amplitude and dC/dV phase. SMIM-C is proportional to the  capacitance of the area beneath the tip, dC/dV amplitude is  related to the concentration of carriers in the sample and  dC/dV phase is related to the carrier type, with N and P-type  material giving a response of opposite sign [1]. In the  following two examples of sMIM data we illustrate sMIM-C  data that provide information absent from traditional SCM  while simultaneously providing the data generated by typical  SCM.


Measurement Details


The image sensor used in this paper is from a recent  commercial device. It is a front-side illuminated global-shutter  CMOS image sensor with 3µm x 3µm pixels. Cross-sectional  and planar samples were prepared using diamond lapping  films of decreasing grit and finishing with colloidal silica  slurry. The samples are then conductively epoxied to a sample  holder to allow grounding the sample. The RMS roughness of  the samples is less than 1 nm.


Measurements were performed on two different AFM systems  with the PrimeNano Scanwave system integrated on both  systems to provide sMIM capabilities. Images are recorded in  contact mode with feedback maintaining a constant tip-sample  force. Five channels (sMIM-C, sMIM-R, dC/dV amplitude  and dC/dV phase) were recorded along with the AFM  topography. Only three channels: sMIM-C, dC/dV amplitude  and dC/dV are presented in this paper. The tip can be biased  with respect to the sample using 1V amplitude, 20 kHz  modulation signal with a DC offset.


Capacitance vs. voltage curves were recorded by moving the  sMIM tip to a location of interest, and then recording the  sMIM-C signal while sweeping the DC bias voltage. No AC  modulation is used when recording C-V curves. Curves are  averaged over 5 sweeps from -2V to 2V.


Planar Dopant Analysis


Fig. 3 shows simultaneously recorded (A) dC/dV phase, (B) dC/dV amplitude and (C) sMIM-C images of a planar sample  similar in location to Fig. 2(A). The relationship between  carrier concentration and dC/dV amplitude is challenging to  interpret: it is non-linear and can be non-monotonic. The  monotonic nature as a function of dopant level of sMIM-C  provides for a simpler interpretation of the data.


The dC/dV phase image in Fig. 3(A) appears as expected in  standard SCM imaging. N-type regions and p-type regions  within a certain dopant concentration range are differentiated, whereas all other areas appear with a random phase centered  on 0.


Figure 3: Multiple channels of data acquired simultaneously  from sMIM on a planar sample polished to just below the  polysilicon layer: A) dC/dV-phase, B) dC/dV-amplitude, and  C) sMIM-C.


Figure 3(B) dC/dV amplitude and (C) sMIM-C appear as very  similar images. A central photocathode and storage diffusion  look similar while the surrounding substrate appears brighter  around them. Other features, like shallow trench isolation fill  much of the remaining image as a dark background. Additional analysis presented below will illustrate important


differences in information content not easily seen in this  figure. As dC/dV phase data in Fig. 3(A) remains available  during the sMIM measurement, it is still possible to ascertain  the carrier type of each location. This is an important part of  the dC/dV measurement. In areas where it is possible to  determine carrier type, then the carrier type is known. In areas  where dC/dV provides no information sMIM-C is still capable  of providing physical insight. The combination of sMIM-C  and dC/dV phase therefore provides a combination of  information not available with conventional SCM.


Figure 4: A) dC/dV amplitude image of the CMOS image  sensor. B) Horizontal line profile plots through A) and C).The  location of the line profile is represented by the dashed white  line on each image. The white ellipses in B) ( i, ii, iii) indicate  regions of interest. C) sMIM-C image of the CMOS image  sensor.


Figure 4 presents a higher-resolution view of the same planar  sample from Fig. 3. The dC/dV amplitude and sMIM-C  images were collected simultaneously. The line profile data in  Fig. 4(B) is shifted to allow each to have a minimum at 0 and  then scaled by dividing by their respective maximum values. This is done for clarity.


Two TEM lamellae were prepared to measure the amorphous  damage of Si sample by Xe beam during the sidewall  polishing. The lamellae were prepared from Si sample surface  polished tangentially by Xe ions at the beam energy 30 keV  and 3 kV, respectively. The probe current was 100 pA at both  energies. In both cases, the surface of polished Si was covered  by Pt protection layer, firstly by the focused electron beam  induced deposition (FEBID), to avoid the damage of the thin  amorphous layer, then by the focused ion beam induced  deposition (FIBID), to grow faster the protection layer with  sufficient thickness. After that, two TEM lamellae  perpendicular to the surface were extracted and thinned by Xe  beam on the copper grid. These lamellae were immediately  transferred into the TEM and the thickness of the damaged Si  layer was measured there using HR-TEM technique. The  results are shown in Figure 4 (beam energy 30 keV) and  Figure 5 (beam energy 3 keV).


In both cases, the orientation of Si crystals was accurately


900


aligned to in-pole position at zone axes (110). The TEM


800


alignment was set up to allow the phase contrast, i.e., no


z [nm]500


objective aperture and a sufficient defocus was used.


400


300


From Fig. 4 and 5 thickness of the damaged layer was


200


measured. It was 13 nm at the beam energy 30 keV and 3.0 nm


at the beam energy 3 keV, respectively. Precision of the  measurement of the damage layer is slightly limited by the  unclear interface between the damaged layer and the


Y[μm]


protection layer (B-C intefrace on Fig. 4 and 5). The measured


x[μm]8 99 10


Xe+ ion beam damage can now be directly compared to  previous studies where Ga+ ion beam damage was measured. Regarding Ga+ ion beam damage at 30 keV, the reference [5] nicely summarizes data from several authors, who have  presented both calculated and experimentally measured values. For experimentally measured values at beam energy 30 keV, the values vary between 17 and 30 nm, which suggests that the  precision of the measurement is limited for Ga+ ion beam due  to the same reason. 28 nm were measured in [6] and 20 nm in


[7], so both values are still in the same interval like in [5].


However we have measured 13 nm for Xe+ ion beam at the  same beam energy, which means the damage is significantly  less for Xe+ ion beam, the difference is between 24 and 57%.


20nm


20 nm


Figure 4: TEM image of the amorphous damage of Si surface  after polishing it tangentially by Xe+ ion beam at the beam  energy 30 keV and probe current 100 pA. 4a – lower  magnification, 4b – higher magnification is shown. A – Si  lattice, B – the amorphous layer created by Xe+ ion beam  milling, C – Pt FEBID and FIBID protection layers. The  measured thickness of the damaged layer is 13 nm.


Regarding the ion beam damage at the low beam energy they  have measured 2-3 nm for 5 keV Ga+ beam in [12], which is  surprisingly lower number than our measurement at 3 keV. At  2 keV, they have measured 0.5–1.5 nm [12]. To compare it  with different authors, in [7] they have measured the


Figure 5: TEM image of the amorphous damage of Si surface   after polishing it tangentially by Xe+ ion beam at the beam  energy 3 keV and probe current 100 pA. 5a – lower  magnification, 5b – higher magnification is shown. A – Si  lattice, B – the amorphous layer created by Xe+ ion beam  milling, C – Pt FEBID and FIBID protection layers. The  measured thickness of the damaged layer is 3.0 nm.


dependence of the amorphous layer thickness on the beam  energy and it was linear between energies 10 and 40 keV. The  value measured at 30 keV was 20 nm and at 10 keV it was


9.4 nm. Their results were also in good agreement with  theoretical simulations. Following the same approach we


A  B  C


nm


10nm


C


4a


5b


4b


5a


interpolate the amorphous layer thickness to the beam energy  3 keV, we obtain an amorphous damage thickness of 5.7 nm  which looks to be more realistic than 2-3 nm at 5 keV  measured in [12]. To summarize, at the low beam energy  3 keV the Xe+ ion beam and the Ga+ ion beam, seem to be  quite comparable. More detailed studies incorporating  modeling may reveal further subtle differences.


HR-TEM images of lamella from IC sample


An example of HR-TEM imaging of the lamella created from


the modern semiconductor sample by Xe plasma FIB at the


beam energy 30 keV is shown in Figures 6-8. Figure 6 is


showing the overview image of the lamella and Figure 7 is


showing the high resolution detail of the transistor layer.


Obviously the silicon parts of the lamella are still crystalline,


without the significant amorphous damage visible (see the high


magnification detail in Figure 8). This seems to confirm our


general conclusion about the reduced amorphous damage of


TEM lamellas prepared by Xe ion beam, when compared to 100nmGa FIB preparation at the beam energy 30 keV.


Figure 6: TEM image overview of the lamella. The silicon


area is at the top, the layer at the bottom is Pt protection cap.  20nm


Between 24-57% less amorphous damage was measured at the  beam energy 30 keV for Xe ion beam in comparison to Ga ion  beam. This has been confirmed by EDS analytical method (no  Xe was detected in the amorphous layer, while for Ga beam  damage there was a significant amount of Ga detected). The  lamella prepared at FIB beam energy 30 keV from IC sample  was also visually showing less surface damage in HR-TEM  than typical lamellae prepared by using Ga FIB at the same  beam energy.


Figure 7: HR-TEM image of the lamella prepared by Xe  plasma FIB at the beam energy 30 keV, showing the high  resolution image of the transistor layer.


Figure 8: HR-TEM image of the lamella prepared by Xe  plasma FIB at the beam energy 30 keV, showing the  crystalline character of silicon areas with negligible influence  of the amorphous damage layer.


The research has been supported by the Technological Agency  of Czech Republic *TE 01020233 (AmiSpec).


[1] L. A. Giannuzzi, F. A. Stevie, Introduction to Focused Ion  Beams (2010).


[2] T. Hrnčíř et al., ISTFA 2012: Conference Proceedings  from the 38th International Symposium for Testing and Failure  Analysis (2012), pp. 26.


[3] A. Delobbe et al., Microscopy and Microanalysis, Vol. 20 (2014), pp. 298.


[4] L. Kwakman et al., ISTFA 2013: Conference Proceedings  from the 39th International Symposium for Testing and Failure  Analysis (2013), pp. 17.


[5] N. I. Kato, Journal of Electron Microscopy, Vol. 53, No. 5 (2004), pp. 451.


[6] S. Rubanov and P. R. Munroe, Journal of Microscopy, Vol. 214 (2004), pp. 213.


[7] Z. Wang et al., Appl. Surf. Sci. Vol. 241 (2005), pp. 80.


[8] C. Lang et al., Microelectronics Reliability, Vol. 54 (2014), pp. 1790.


[9] M. Rommel et al., J. Vac. Sci. Technol. B, Vol. 28 (2010), p. 595.


[10] C. Lang et al., Microscopy and Microanalysis Vol. 18


(2012), p. 620.


[11] I. Utke, P. Hoffmann, J. Melngailis, J. Vac. Sci. Technol. B, Vol. 26 (2008), pp. 1197.


[12] J. Mayer et al., MRS Bulletin Vol. 32 (2007), pp. 400.


Turning sample into (re)solution:


Focused Ion Beam shaped Solid Immersion Lenses


Philipp Scholz1, Michael Sadowski1, Sebastian Kupijai2, Marvin Henniges2, Christoph Theiss2,3, Stefan Meister2,3, David Stolarek4, Harald H. Richter4, Mahyar Boostandoost5 and Christian Boit1


1Semiconductor Devices, Berlin University of Technology, Einsteinufer 19, 10587 Berlin, Germany


2Institut für Optik und Atomare Physik, Berlin University of Technology, Straße des 17. Juni 135, 10587 Berlin, Germany  3Sicoya GmbH, c/o Berlin University of Technology, Straße des 17. Juni 135, 10587 Berlin, Germany


4IHP, Im Technologiepark 25, 15236 Frankfurt (Oder), Germany


5Dialog Semiconductor, Neue Str. 95, 73230 Kirchheim unter Teck, Germany


Phone: +49 (0)30 314 26803  Email: philipp.scholz@tu-berlin.de


This work is a unique solution for enhancing optical failure  analysis and optical signal transmission. Optical failure  analysis remains to be a vital part of the analysis process, despite shrinking feature sizes and challenging package  technologies. The presented optical signal transmission  supports the development of photonic integrated circuits.


The key component is a Focused Ion Beam (FIB) process  which shapes optical lenses out of the sample material leading  to an improvement in lateral resolution and signal transmission. Two cases are shown that demonstrate these  improvements. The first case is an optical backside analysis in  a spatially confined opening of a package where other Solid  Immersion Lens (SIL) systems could not be applied. It offers  an improvement in spatial resolution by a factor of 2, down to  a FWHM of 387 nm. The second case is a novel application  for FIB shaped lenses aiming at photonic integrated circuits. This lens is created out of the isolating frontside and improves  the grating coupler efficiency by a factor of 4.1.


While Focused Ion Beam (FIB) tools, with their ability to  precisely remove and deposit material, are commonly used for  cross sectioning, TEM sample preparation and circuit edit [1],


[2], this work uses a FIB for shaping lens elements directly out  of the material of a sample (Fig. 1).


Figure 1: Basic concept of this work: shaping a lens out of the  sample material using a focused ion beam and assisting  chemistry.


Essential components of the presented technique are the  bitmap mode, which controls the movement of the ion beam in  pixel values corresponding to dwell times, and the selfcalibrating algorithm (Fig. 2) developed by the authors [3]. In  addition, an assisting etch chemistry is used for efficient  processing and to avoid lens degradation due to implanted  ions.


Figure 2: Simplified concept of the self-calibrating FIB SIL  creation algorithm. Main components are: (a) calculated  target profile, (b) measured profile from draft shape based on  approximation of target, (c) grayscale (GS) bitmap which  controls ion beam and created “b”, (d) resulting new  grayscale bitmap for 2nd step / next iteration.


Two cases are demonstrated where this technique significantly  extends the possibilities of the corresponding fields of  application: One is a Solid Immersion Lens (SIL) [4] shaped  with a FIB out of silicon substrate material for optical  backside analysis [5] inside a commercial Quad Flat No leads (QFN) package (merely 4x4mm² opening), in which case “external” SIL systems could not be applied. The other is a  lens shaped out of the isolating frontside of a chip for


developing photonic integrated circuits, and thereby


a)


b)


c)


successfully enhancing the transferred optical signal with an


objective


improvement of the grating coupler efficiency. Figures  corresponding to one of these cases are indicated in the


SIL


following by “sample 1” or “sample 2”.


M  tilted sampleuneven


particle


polishing


edge of package平出业


h


FIB shaped SIL for optical backside analysis


The basic principle of round, refractive SILs can be illustrated  by optical ray tracing (Fig. 3, [6]). A SIL used in a central  setup can preserve a large opening angle inside a higher  density material and thereby improve numerical aperture (NA) and spatial resolution. A remarkable difference between  common “external” SIL systems and the presented FIB shaped  SILs is the reduced surface area needed for the same opening  angle (Fig. 4).


Though becoming part of the sample, FIB shaped SILs can be  completely removed by slight polishing of 5-10 µm, if  necessary. Furthermore, SILs created out of the sample itself  do not face the same challenges like external SILs (Fig. 5), i.e. image degradation due to a tilted sample, uneven polishing, or  particles underneath the SIL, and the critical condition where  SIL analysis is not possible close to the edge of the package  opening.


ES OF LURUBUS JNUM


(a)                                                      b)


Figure 3: Optical ray tracing analysis without (a) and with (b) SIL illustrates the optical benefit of a SIL: preserving a large  opening angle inside higher density materials and thereby  leading to higher spatial resolution. Notice that for the central  refractive SIL setup used in this work only a small segment of  the SIL is needed to improve e.g. a 0.76 NA objective. Ray  tracing was done with [6].


sample


Figure 4: Application example: Backside analysis with  external SIL (a) and SIL in sample substrate material (b). “b” requires significantly less surface area, but offers the same  opening angle θ. Sample and SIL material need to match in “a”.


Figure 5: Challenges for external SIL applications which can  be solved by creating a SIL from sample material: Imaging  can be degraded by air gaps from a tilted sample (a), uneven  polishing and particles (b), and become impractical near the  edge of the package opening (c).


Especially the last aspect is addressed in the presented case for  an optical backside analysis of a silicon sample inside an  opened QFN package allowing only a 4x4mm² opening (Fig. 6). While the cavity in the package is very shallow and  doesn’t restrict the optical opening angle of a FIB shaped lens, it is deep and small enough to hinder the placement of an  external SIL. External SILs with a cone-shaped base [7] might  partially help, but only for a central spot of the sample. Therefore a FIB shaped SIL segment with a radius of  curvature of 62 µm and a width of 50 µm was created in the  silicon substrate with an assisting iodine-based chemistry. A  central SIL setup was chosen over an aplanatic / super SIL  setup, due to better tolerance in sample thickness.


Figure 6: A die inside an opened QFN package (4x4mm²) on  which a FIB SIL analysis is performed where other SIL  systems could not be applied (sample 1).


The previously mentioned self-calibrating algorithm (Fig. 2)


[3] produced a SIL matching the ideal shape (Fig. 7). Over its


full opening angle of 26° the SIL deviates by only ±220 nm


from its designed radius of curvature of 62 µm. Over the inner


FIB created


possiblySILconnected0


22° it even deviates by merely ±120 nm (Fig. 8). This  indicates an optically working SIL for infrared (IR) imaging


to objective中


through silicon with NA = 3.5 sin 26° = 1.5, doubling the  resolving capabilities of the microscope available to the  authors. Laser scanning images taken at 1300 nm wavelength  illustrate this by making smallest details below wavelength  dimensions visible and by enhancing the edge contrast (Fig. 9, Fig. 10).


Posilion in μm


Figure 7: Cross section of the FIB shaped SIL inside the  narrow QFN package opening (axes scaled differently). The  self-calibrating algorithm created a suitable SIL shape, which  offers a numerical aperture (NA) of 1.5 (sample 1).


Posilion in um


Figure 8: The radial deviation of the presented FIB shaped


0-6-0-4一日


SIL in silicon is only ±220 nm over the entire 26° opening


0.0


angle and close to merely ±120 nm for the inner 22°. This 0200400600800100012001400 indicates an optically working SIL with NA 1.5 (sample 1).


2μml1


乙dUL


e


u0.6FWHM without SIL 8


829 nm


1t


(a)                                                      (b)


u 6 S0.4


FWHM with SIL


Figure 9: 1300 nm laser scanning images using a 50x


387 nm


objective (NA 0.76) of a less than 60 µm thick silicon sample,


without (a) and with (b) the FIB shaped SIL. Magnification  was adjusted so show the same image features (sample 1).


050010001500200025003000


1μm H


Figure 10: Detail of Fig. 9: 1300 nm laser scanning images  using a 50x objective (NA 0.76) of a silicon sample, without


(a) and with (b) the FIB shaped SIL. The improvement in  resolution with SIL by a factor of 2 makes additional image  features visible and enhances edge contrast (sample 1).


In addition to the previous visual comparison (Fig. 9, Fig. 10), a series of line scans of an edge was analyzed to quantitatively  verify the improvement in spatial resolution. The scans were  performed over the same image feature without and with SIL. The Houston criterion [8] was applied, which connects the


um inHeight


-ideal shapa


spatial resolution to the Full Width at Half Maximum


--FIB SIL in Si


(FWHM) of a Gaussian Point Spread Function (PSF). The


-6-32.5-24.375 -16.25 -8.12508.12516.2524.37532.5


dashed line in Fig. 11 is the integral of the fitted PSF with SIL. It closely matches the experimental data, indicating a proper  fit of the calculated Gaussian profile (see [9], [10] for more  applications of this methodology). The resulting FWHM with  SIL is 387 nm. This value was compared to the FWHM  without SIL (829 nm) in Fig. 12 verifying the expected  improvement in resolution by a factor of 2.


1.0>measured data


- fitted Gaussian PSF-- integral of PSF


'n


8 u0.6


-200.


e u


Rarial davialionn nm from iddeal i-25-18.75-12.5-8.2508.2512.518.7525


6 s0.4


只FWHM with SIL


>。60


Position in nm


Figure 11: Spatial resolution measurement with SIL over the  edge of an image feature from Fig. 10. The acquired data


properly corresponds to the integral of a fitted Gaussian  profile, which shows a FWHM of 387 nm (sample 1).


-fitted PSF without SIL


- fitted PSF with SIL


Figure 12: Comparing the Full Width at Half Maximum (FWHM) without and with FIB shaped SIL verifies the  expected improvement in resolution by a factor of 2 (sample 1).


FIB shaped lens for optical signal transmission


The second presented case of a FIB shaped lens is entirely  different from the first, though it uses the same technique (Fig. 2, [3]). While the first was applied to the backside of a  chip (see Fig. 4) by working on the silicon substrate with a  FIB and an assisting iodine-based chemistry, the second is the  creation of a lens in the frontside of a chip (Fig. 13) by  shaping the isolating SiO2 with a FIB and XeF2.


The terms “backside” and “frontside” are explicitly used to  differentiate the two cases. Note that the second case can also  be referred to as “back end lens” derived from the back end of  line (BEOL). The BEOL includes the production of metal  layers leading up to the frontside. It thereby connects the  devices which are created in the front end of line (FEOL) at  transistor level (Fig. 13) [11].


This second case is used for developing and analyzing  photonic integrated circuits. The basic idea is the signal  enhancement of a laser, which is coupled through the chip’s


mi


frontside into a grating coupler at the transistor level (Fig. 13). The laser diode is currently the only part, which is not yet


spheric / aspheric lens


Fresnel lens


fully integrated. It is placed on the chip and shines divergently


through the surface of the frontside (Fig. 14). Any metal layers WTLUWWEL HNand fill shapes were omitted by design in the path of light  towards the grating coupler.


single-level


multi-level


u


Transistor Level


d


(a)                                                             (b)


6 Figure 13: Concept without (a) and with (b) lens created by 40


-ideal shape---FIB SIL in SiO2


FIB in the chip’s frontside: The optical signal from a laser  diode (placed on the chip) is enhanced by the FIB created lens


-6-18-13.5-9-4.504.5913.518


(b) increasing the grating coupler efficiency. Metal layers and  fill shapes in the path of light were omitted by design (sample 2).


Laser diode


曾


台


hapc in nm s idealDeviation from-12.5-9.375-8.25-60-3.12503.1256.259.37512.5


Figure 14: Only the laser of the presented chip for photonic  integrated circuits is not yet fully integrated. It is placed on  the chip and couples light into the grating coupler through the  presented FIB created lens (sample 2).


The FIB shaped lens will undergo different stages in the  ongoing development: From an aspheric shape to a multi-level  Fresnel phase plate - a combination of a Fresnel lens and a  single-level Fresnel phase plate [12], [13] (Fig. 15). Just like a  FIB circuit edit, this FIB shaping of lenses is the preparation  for integrating the final result into the lithography process. Particular attention has to be paid to the isolating behavior of  the SiO2. A thin layer of gold needs to be applied prior to FIB  processing to avoid drift and punch-throughs. This layer does


not have an optical influence in this case, because it is only  deposited in the areas of FIB processing and is instantly  removed where FIB lenses are created. For the presented stage  of the development, an aspheric lens was shaped with the  aforementioned self-calibrating algorithm (Fig. 2) and  assisting XeF2 chemistry. The resulting lens shape is in  exceptionally good agreement with the ideal shape (Fig. 16) and shows deviations of only ±50 nm (Fig. 17).


Fresnel phase plate


LaserFrontsideLight


Light Laser


Figure 15: The presented lens is an aspheric one, while


SiO2


several approximations are possible. The future goal is a  multi-level Fresnel phase plate which is to be created during  chip production by the lithography process (sample 2).


Grating Couplerm


Grating CouplerSi


nf


Position in um


Figure 16: Cross section of the lens shaped by FIB into the  SiO2 frontside of the sample for developing photonic


Area for FIB created Lens


integrated circuits (axes scaled differently). The lens is in  exceptionally good agreement with the ideal shape (sample 2).


Figure 17: The lens created by FIB in the SiO2 frontside  shows only minor deviations in the range of ±50 nm compared  to the ideal shape (sample 2).


In order to investigate the improvement in beam profile and  grating coupler efficiency with the FIB shaped lens, a 2.5 µm  wide spot of a tapered fiber was used as a divergent light  source. Infrared light at 1550 nm wavelength was coupled  through the frontside into the grating coupler at the transistor  level without and with lens. The coupling efficiency was  measured spatially resolved by scanning an area of 20 µm by  20 µm with a resolution of 1 µm. Fig. 18 shows corresponding  normalized 2D scans, comparing the conditions without and


with lens. While the measurement without lens shows a  divergent behavior, the measurement with the lens shows a  strong focusing effect. The final result of the comparison is  that the grating coupler efficiency is improved by a factor of


4.1 (6.1 dB).


(a)                                                        (b)


Figure 18: The investigation of the beam profile without (a) and with (b) lens in the chip’s frontside confirms the focusing  effect of the lens, leading to an improvement in grating  coupler efficiency by a factor of 4.1 (6.1 dB) (sample 2).


The two demonstrated cases of FIB shaped lens applications  show unique solutions only achievable with the presented  technique. The FIB shaped SIL offering a numerical aperture  of 1.5 doubles the resolution capability for optical infrared  backside analysis and shows a FWHM of 387 nm. The FIB  shaped lens in the SiO2 frontside improves the grating coupler  efficiency in a chip for developing and analyzing photonic  integrated circuits by a factor of 4.1.


Thanks go to Andreas Eckert (TU Berlin) and Ultra Tec for  sample preparation support. Further thanks go to Heiko  Lohrke (TU Berlin) for ray tracing support and SIL  discussions.


[1]


J. Orloff, L. Swanson, and M. W. Utlaut, High resolution  focused ion beams: FIB and its applications: the physics of  liquid metal ion sources and ion optics and their application  to focused ion beam technology. Springer, 2003.


[2]


T. Malik, R. K. Jain, R. Nicholson, and T. Lundquist, “Role  of Circuit Edit in Post-Silicon Debug and Diagnosis,” in 2nd


IEEE Silicon Debug & Diagnosis, 2005.


S10


[3]


P. Scholz, N. Herfurth, M. Sadowski, T. Lundquist, U. Kerst, and C. Boit, “Efficient and flexible Focused Ion Beam


micromachining of Solid Immersion Lenses in various bulk  semiconductor materials – An adaptive calibration


algorithm,” Microelectron. Reliab., pp. 7–10, Aug. 2014.


05101520051015 20


[4]


G. S. Kino, “Solid immersion lens,” Proc. SPIE, vol. 3740, no. June, pp. 2–5, 1999.


[5]


K. Vigil, Y. Lu, A. Yurt, T. B. Cilingiroglu, T. G. Bifano, M. S. Ünlü, and B. B. Goldberg, “Backside FA with SILs  Integrated Circuit Super-Resolution Failure Analysis with  Solid Immersion Lenses,” Electron. Device Fail. Anal., vol. 16, no. 2, pp. 26–32, 2014.


[6]


P. Lutus, “OpticalRayTracer.” [Online]. Available: http://arachnoid.com/OpticalRayTracer/.


[7]


O. Breitenstein, F. Altmann, T. Riediger, D. Karg, and V. Gottschalk, “Lock-in thermal IR imaging using a solid  immersion lens,” Microelectron. Reliab., vol. 46, no. 9–11, pp. 1508–1513, Sep. 2006.


[8]


W. V Houston, “A compound interferometer for fine  structure work,” Phys. Rev., vol. 29, pp. 478–485, 1927.


[9]


F. Köklü, J. Quesnel, A. Vamivakas, S. Ippolito, B. B. Goldberg, and M. Ünlü, “Widefield subsurface microscopy  of integrated circuits,” Opt. Express, vol. 16, no. 13, pp. 9501–9506, 2008.


[10] K. Serrels, E. Ramsay, R. J. Warburton, and D. T. Reid, “Nanoscale optical microscopy in the vectorial focusing  regime,” Nat. Photonics, vol. 2, no. 5, pp. 311–314, Mar.


2008.


[11] K. Reinhardt and W. Kern, Handbook of Silicon Wafer  Cleaning Technology (Second Edition). Elsevier, 2008, p.


15.


[12] Z. Jakšić, Micro and Nanophotonics for Semiconductor  Infrared Detectors, 1st ed. Cham: Springer International  Publishing, 2014, p. 67.


[13] P. Scholz, U. Kerst, C. Boit, T. Kujawa, and T. R. Lundquist, “Instant Solid Immersion Lens creation in silicon  with a Focused Ion Beam - comparing refractive and  diffractive methods,” in Proceedings of ISTFA 2011, 2011, pp. 46–53.


Near field EMC scanning method based on an E-field collapse


Jeff Dunnihoo


Pragma Design, Inc. Austin, Texas


jeffhoo@pragma-design.com, (512) 965-0071


Pasi Tamminen


Microsoft, Tampere, Finland


Toni Viheriäkoski


Cascade Metrology, Lohja, Finland


In this study we present a novel method to use a field collapse  method together with fully automated near field scanning  equipment to construct E- and H-field information of a system  during transient ESD events. This inexpensive method  provides an alternative way for system designers to validate  and analyze the EMC/ESD capability of electronic systems  without TLP pulsers, ESD simulators, or precision inductive  current probes.


Electromagnetic fields around an electronic system can be  measured with non-contact electrical and magnetic near field  probes by using a spectrometer [1,2,3]. These measurements  can be done manually by moving the probe close to the surface  of the device under test (DUT), or by using an automated  scanning system with x-y-z axis control and simultaneously  recording the near E- and H-field density and location  information.


For EMI analysis, measured fields may originate from the  normal operation of the equipment.  Alternately, the source of  the field may be an externally injected aggressor pulse to  simulate EMC compatibility testing. Commonly, a fast high  current transient electrostatic discharge (ESD) pulse is utilized  in scanning systems created by using Transmission Line Pulse (TLP) or IEC610004-2 ESD gun generators [1]. In this case  the purpose of the field scanning is to study for example how  well different EMC/ESD protection components filter and  clamp electromagnetic interference (EMI) on a printed wiring  board (PWB) area.  Meaningful visualization of such scanning  requires tight synchronization of the field measurement and  pulse scanning system to accurately capture the short transient  pulses.


Method details:


The IC die sample was deprocessed from the back side [3] to  the metal 1 level. An externally grounded conductive line was  deposited by FIB on the die above a dielectric (SiO2) patch,


and then connected to the input node of the ‘starting point’ buffer while keeping the rest of the IC electrically floating


(Figure 4 Bottom). The M1 structure corresponding to the


output node of the next buffer upstream in the chain was


now visible with high contrast when compared to the


surrounding M1 structures (Figure 6). Using FIB conductive  deposition, the output and input nodes of this buffer were  shorted together (Figure 4 Top), moving the high contrast of  the grounded signal to the next buffer in the chain. The


output node of this buffer was then identified using the FIB  PVC technique (Figure 6), and the buffer bypass process was


repeated again ‘jumping’ to the next buffer.


Figure 4. a) Grounded ‘bright’ external line connected to  the buffer input node, b) bypassing the buffer’s in & out  nodes moves the ‘bright’ grounded signal to the next


buffer in line.


Figure 5. Tracing control signal back toward  controller.


Results Discussion:


After 82 ‘jumps’ along the buffer chain the final ‘jump’ went  past the boundary of the core and ‘lit up’ a device (Figure 7  Top) different from the typical buffers in the buffer chain. It


，


was concluded that the Power Management Controller block  was successfully identified and localized (Figure 7 Bottom).


Conventional imaging/reverse engineering could then be


applied to the found Power Management block.


A comparison of key metrics was made between two


approaches- traditional Reverse Engineering (RE) and FIB PVC.


Significant improvements were observed in throughput time,


equipment time and operator resourcing.  In particular the


FIB PVC saved >20,000 SEM images and >300 hours of SEM


time as well as >200 hours of engineering time.


Figure 6. Buffer output node is recognized using FIB


3※


PVC technique.


Figure 7. Final jump is not to a typical buffer (Top).   Buffer path toward Power Management Controller (Bottom).


Conclusions:


FIB PVC phenomena is well known in FA and has traditionally  been used to identify breakage in conductors. Based on the


phenomena, a new method for circuit tracing and circuit


analysis was developed.


Using this patented technique titled “Circuit tracing using a


focused ion beam” [4], specific circuits and functional blocks  can be localized in a reasonably short amount of time with a  more accurate estimate of the time needed to complete


circuit read-back and/or circuit analysis projects. Previously


cost-prohibitive or high risk projects can now be successfully  completed at reduced time and cost.


Acknowledgements:


The authors would like to acknowledge and thank the


Techinsights Ottawa Lab team for helping with sample


preparation, and would like to extend an appreciable thank


you to the FIBICS team for their help and for the facilities they  provided for the experiments and the process development.


References:


[1] Chun-Sheng Liu, Chih-Rong Chen and Yong-Fen Hsieh


United Microelectronics Corporation (UMC) “Identification of  Processing Defects by Focused Ion Beam (FIB) Induced


Voltage Contrast” Proceedings of 7th IPFA ‘99, Singapore.


[2] Method of registering and aligning multiple images (US


patent 7693348 B2) Inventors: Vyacheslav Zavadsky, Jason


Abt, Mark Braverman, Edward Keyes, Vladimir Martincevic.


[3] Failure Analysis from the Back Side of a Die


Silke Liebert, Philips Semiconductors. Conference Proceedings  of the 26th International Symposium for Testing and Failure  Analysis; pages 177-185


[4] Circuit tracing using a focused ion beam US 8791436 B1


Inventors: Chris Pawlowicz, Alexander Sorkin, Michael W.


Phaneuf, Alexander Krechmer, Ken G. Lagarec


An Infrared Microscope for use on a Focused Ion Beam for Circuit Edit and Backside  Edit Applications


Alexander Richards, and Matthew Weschler*


Technical Sales Solutions LLC, 15201 NW Greenbrier Parkway, Beaverton OR 97006 *Matt@TechnicalSalesSolutions.com


Michael Durller


Battelle, 505 King Ave, Columbus OH 43201


As micro-circuitry design nodes continue to become smaller, in rough accordance with “Moore's Law”, the challenges


presented to failure analysis and process development labs


continue to grow.  Often, regions and features of interest are


buried beneath layers of passivation, metal interconnect, or


silicon that makes Focused Ion Beam (FIB) or Scanning


Electron Microscope (SEM) imaging difficult and tedious.


Use of a FIB or SEM allows only shallow visual penetration


into the surface and often makes actions on deeper sub-surface  features a “shot-in-the-dark”.  As a result, researchers' ability  to meet time, quality, and budget demands become


increasingly stressed.


Frequently within the failure analysis or development lab


context, one may wish to perform a circuit edit (CE) or cut a


cross-section on a sample of interest [1].  If there are no


visible surface features that can be utilized as references, and  in cases where there are no Computer Aided Design (CAD)


layouts readily available for navigational use, the actions of


CE, cross-sectioning, and sample preparation can become


difficult to the point of impeding productivity and the quality  of data obtained from such procedures.  In this instance, the


microscopist is essentially “flying blind”.  A microscopist is


already working in a small unknown world and he or she must  have all the tools on hand that can possibly assist to make


actions, interpretations, and experiments a success on this


nanoscale.


To help solve this navigational problem, i.e., being able to


successfully locate a circuit for probing or editing without


destroying chip functionality, a near-infrared (NIR), nearultraviolet (NUV), and visible spectrum camera system was


developed that attaches to most FIB or SEM vacuum


chambers.  We believe some elements of this design to be


unique in the marketplace.


To date, this camera system has been fitted to an FEI FIB 200  ion beam platform.  Because flexibility of the system


hardware was a design priority, this camera can also be fitted  onto FIB or SEM platforms by other vendors.


With proper consideration and selection of illumination type


and wavelength in conjunction with the associated microscope


optics, small features buried in bulk silicon can be effectively  visualized for purposes of identification and navigation.  With  our hardware, this capability has been demonstrated on small  features buried over 200um deep within the substrate.  The


camera can be used in real time, as an end point detection


methodology while milling, i.e., it is possible to image directly  upon the milling process while the ion beam is performing its  function.


This paper will review further details of the design and


implementation of the NIR/NUV camera system, as


instantiated upon the FEI FIB 200, with a particular focus on  its use for the visualization of buried structures, and also for


non-destructive real time area of interest (AOI) location and


end point detection.  This paper will specifically consider the  use of the micro-optical camera system for its benefit in


assisting with CE, as well as other typical FIB milling


activities.


Development of the Microscope


The optical column was developed with flexibility in mind,


both for applications usage and platforms onto which it could  be integrated. The Olympus XM10 NIR CCD camera and


most of the optics exist outside of the vacuum chamber on the  host microscope, thus making it easily transportable and able  to be used on most FIB, SEM, and FIB-SEM. The camera and  the optical path connect to the chamber in such a manner that  the camera is coincident with the FIB at the eucentric point,


much like a traditional two-beam system with FIB and SEM  columns. While this design may change, the current


implementation of the camera is such that the FIB is


orthogonal to the sample at 0 degrees stage tilt.  At 65 degrees  stage tilt, the optical column image shows the sample topdown.  Figure 1 depicts the geometries of the FIB and optical  columns.


Figure 1: The optical column of the IR camera views top down  on the sample at a stage tilt of 65 degrees.


The collection camera is driven using the open source MicroManager microscopy software. This software was originally


intended for biological applications, but allows histogram


brightness-contrast curve adjustment for NIR viewing through  silicon, and digital zoom capability that is quite useful [2]. The  camera collects via a coated MT-L tube lens with a 200mm


NIR tube lens with metallurgical long working distance


apochromatic NIR objective lens compounded at 50x


magnification at just over 0.4NA. The camera connects to a


PC via USB interface and runs next to the FIB PC. Köhler


thru-the-lens fiber launched illumination provides the NUV,


visible, and IR light needed to image through silicon. Discrete  wavelengths are selectable across a range of 390nm to


1064nm, providing a narrower illumination spectra band than  a traditional tungsten visible “lighthouse” source, although


one could still be used. Figure 2 and Fig. 3 give an overview  of the electromagnetic spectrum and the wavelengths that can  be selected in this on-FIB NIR camera. To even further narrow  the bandwidth of illumination, laser light sources have been


discussed but not pursued because of the speckling effect


commonly seen when viewing laser-illuminated objects [3].


gamma ray


X-rayvisible


microwave


higher frequency*shorter wavelength  higher energy


Figure 2: The Electromagnetic Spectrum


Figure 3: The discrete wavelengths that are used in this


experiment via the epi-illuminated Köhler thru-the-lens fiber  launched LED illumination system.


The camera was installed on an FEI FIB200 platform with


prelens FIB column. During selected edit processes, tungsten  deposition and xenon difluoride etch (Insulator Enhanced


Etch) were utilized. Gases are compatible with our IR camera. The Circuit Edit Application: Frontside Edit


One of the key applications for this camera is the CE


application. The CE application is one that saves industry


money because it reduces the number of mask sets that have to  be created in a process development [4]. CE often involves the  use of a gallium FIB to physically edit a chip, which can be a


difficult process. One must be able to navigate and perform


FIB functions on areas of interest, without destroying the chip  functionality or creating additional problems when performing  the CE [4]. Add on the complexity created by having the CE  region of interest buried underneath tens or even hundreds of  microns of material layers – and the CE process becomes one  not for the easily frustrated.


With proper selection of illumination type, wavelength, and


microscope optics, small features buried in greater than 300um  of bulk silicon can be visualized. Our NIR optical system can  also be used in real time for end point detection while milling, and for visualization of milled structures during the FIB


process.  Some of the challenges related to real-time viewing  during FIB milling will be discussed below.


The use of IR imaging for frontside CE and sectioning also


has great benefit. By being able to visualize layers down


below the surface one can ensure that the AOI is accurately


located and action taken on it, and not on neighboring


features.


An edit was performed on a two metal layer device at the


ultravioletintrared


radio


90nm node using aluminum metallization and typical


semiconductor passivation and dielectrics. The deprocessed  package sample was mounted on a stub and placed into the


longer wavelength lower frequency


FIB200 for IR imaging and FIB milling.


lower energy


For completeness and to compare and contrast different


imaging techniques, Figure 4 shows an optical image acquired  of the sample using a Nikon Epiphot 300 inverted microscope  with a 100x 0.95CF objective, relay lens, and Nikon DSLR


cope  with a 100x 0.95CF objective, relay lens, and Nikon DSLR


|Wavelength	  (nm)	   |Spectral	  Region ||
|---|---|---|

|390	   |NUV ||

|525	   |VIS ||

|810	   |NIR ||

|870	   |NIR ||

|1060	   |NIR ||

D7000 capture camera. The approximate magnification of this  image is 1000X as printed with a horizontal field width


(HFW) of about 90um. In the optical image, which appears in  color, one is able to see the top metal layer (running


horizontally) and the top metal minus one layer running


vertically.


Figure 4: Optical image near the region of the frontside edit  described in detail below. HFW of this image is 90um.


In comparison, this same region was imaged using the IR  camera. Contrast on a sample of this thickness, ~ 20um,


seemed to be optimized when using the NUV (390nm) LED  for illumination. Noticeably, the aluminum interconnect


appears dark in the image, while the nitride passivation layer  transmits the 390nm light, but the bulk silicon interface


reflects it. As you can see in Fig. 5, it is quite easy to see the  buried layer (running vertically) and is accomplished with


high contrast.


To show the performance of the NIR camera, a region of 7um  x 4um was exposed. In this area, there was no top metal and  only metal one layer below, underneath a few microns of


passivation. Figure 5 shows an image on the left from the FIB  and an image on the right from the NUV at 390nm. These two  images are aligned with the Image-to-Image registration


feature of the FEI xP software, and was used to mill based on  placement of the milling pattern on the NUV image side.


Note, it is possible to mill and optically image in real time


with our setup, but milling must be preformed off axis at 65  degrees to optical column orthogonality.


Figure 5: NUV image taken at 390nm before any edits are  done on the sample. One notes excellent contrast and


resolution. The approximate field of view (HFW) of the IR  image when matched to the FIB image is 75um.


Figure 6: Left image is a traditional gallium FIB image, the  right image is a NUV 390nm image showing the subsurface  buried features.  HFW of the FIB image is 76um.


The 7um x 4um box was milled at 150pA to expose the lower  metal layer. The images shown below are of this region at


different wavelengths of illumination. It is instructive to


compare the quality of the images at different illumination


wavelengths. In general, the 525nm illumination is an “allaround” best wavelength for most samples. This visible green  light provides the best overall contrast on most samples and  still allows for good resolution, and provides some metal


morphology visible. While the NUV 390nm wavelength


provides better overall resolution, the contrast is sometimes  not as visually appealing as the green 525nm. See Fig. 7 and  Fig. 8 for comparison of these two key wavelengths.


Figure 7: 525nm illumination of the edit area. The image


shows good contrast and clear visualization of the top and


lower metal lines.  The HFW is 50um.


Figure 8: 390nm illumination of the edit area.  The HFW of  this image is ~ 75um.


It is also interesting to compare the resolution of the different  wavelengths. Theoretically, the resolution of an optical


imaging system that uses a single aperture is 2.0I, where I is  the wavelength of illumination. This increases to 1.0I in a


system with two apertures [5]. In a single aperture system,


some stray light can lead to degradation of the effective


resolution, thus the improvement in resolution by use of the  double aperture. The system utilized for this experiment has a


single aperture. Therefore, one might expect the resolution at  390nm to be approximately 800nm and at 525m illumination  one might expect the resolution to be greater than 1um. To


validate this, during one of the edits we utilized an exposed


feature and measured it in the FIB and then validated we could  clearly discern it from dark space in the IR image. A box 1um  square was milled and metal exposed. The exposed metal


measures 0.4um square. We can show that the IR image


resolution certainly meets the Rayleigh criterion [6] and


validates the resolution of the IR camera is less than 0.5um


even at 525nm. Figure 9 shows the FIB image of a small


exposed metal area in the upper left quadrant and Fig. 10,


shows the corresponding IR image at 525nm.


a


Figure 9: FIB image. To validate the resolution of the IR


camera, we measured the exposed dot highlighted near the


arrow. Contrast in this image is elevated to show the small dot  in the upper left quadrant. The HFW of this image is ~25um.


Figure 10: Optical image at 525nm showing the 1um feature. This bright 1um square dot is clearly seen in the IR image.


To complete the edit, a tungsten trace was added to connect


the two metal lines (top metal and top metal minus one). The  tungsten trace that was deposited was nominally 13um long by


0.4um wide. Cleanup of the tungsten overspray was done


using the ion beam. This metal trace is clearly visible in Fig. 10 and Fig. 12, thus again validating the resolution of at least


0.5um at 525nm and further improved resolution at 390nm. Figure 13 shows the final optical image taken on the Epiphot  inverted microscope.


Figure 11: Visible green image at 525nm showing the 0.4um  wide tungsten deposited interconnect. The HFW of this image  is ~ 50um.


Figure 12: NUV image at 390nm showing the 0.4um wide


tungsten deposited interconnect. As one would expect the


resolution at 390nm is even better than 525nm.  HFW is


~35um.


Figure 13: Color Optical inverted microscope imaging of the  final edit, showing the tungsten trace. (note: image is inverted  relative to FIB and IR images). HFW is approximately 35um.


The Circuit Edit Application: Backside Edits


The IR camera can prove especially useful for backside circuit  edits or investigations on planarized devices where no top


surface features are visible. For thicker samples like


unpolished samples, a longer wavelength is required to see


through the silicon. In most experiments we conducted, we


utilized either 1064nm or 910nm light.


A common way to perform alignments on planarized samples  is to do a rough alignment with an IR microscope and then


create FIB marks on the sample for more accurate alignments


[7]. Furthermore, CAD navigation can be useful followed by  small area local milling to expose alignment marks [8]. We


have found, however, that with any typical type mechanical


polishing or de-capping there will be residual polishing


material and particulate matter that can be used to roughly


align the sample for coarse milling. Figure 14 shows how


particulate matter on the top surface of the sample can be


focused upon with the IR camera and used for fiducial


alignment of the FIB and IR images. This enables accurate


enough placement of the larger bulk removal FIB mills.


Subsequent exposure of smaller regions of interest could be


done if more accurate alignment is needed, or one desires to


correlate sub-surface features with CAD layout.


Figure 14: FIB image on the left and 1064nm IR image on the  right showing how particles are used for alignment and


placement of mill boxes. The red arrows mark the location of  the same particle in the FIB and IR images.


FIB deprocessing was performed on a planarized sample with  silicon on the order of 25um final thickness. This sample was  polished from a bulk thickness of over 150um silicon to 25um  using an Ultra Tech ASAP-1 CNC polisher. Polishing from


bulk levels to the 25um region is not difficult for an


experienced operator and can save a lot of FIB milling time


and decrease the overall time to data. Another possible way to  decrease gallium FIB milling time is to utilize a Reactive Ion  Etcher to further thin the bulk silicon. A reactive ion etcher


can be useful for bulk milling operations with or without prior  mechanical polishing, but will not be discussed in detail in this  paper. Similarly, an Inductively Coupled Plasma (ICP) FIB


could be used for bulk milling operations [9].


Backside editing is complicated by the issue of doped bulk


silicon absorbing NIR light. The more heavily it is doped, the  more light it absorbs. Unfortunately, gallium is also a silicon  p-type dopant and as the FIB milling operation progresses, the  image becomes less and less transparent to NIR light in the


1060nm range. Some manufacturers choose to dope their bulk  silicon, and some do not. An InGaAs or mercury cadmium


telluride imager would be required to extend the NIR optical  spectra out to 1.2um for imaging on heavily doped silicon


[10]. It has also been noted that the use of gas chemistry is


critical to the IR imaging success [11]. In a gas-depleted mill, it is suggested that gallium implantation becomes more of a


factor in decreasing the effectiveness of IR viewing and IR


imaging becomes difficult or impossible. With the use of


improved silicon based removal gas chemistries one can


improve the camera’s imaging and surmount the effects of


gallium implantation.  These experiments are in progress at


the time of the writing of this manuscript.


In Fig. 15, we see 1064nm light viewing through bulk silicon  before any milling is done.  As milling commences, in Fig. 16  we see that the region of the mill becomes opaque to 1064nm  light and even opaque to lower wavelength light, as shown in  Fig. 17.  This obscures any endpointing advantage and makes  it impossible to see the buried circuitry.  When the sample was  thinned below a few microns, the image became visible at


wavelengths below 1064nm.   As noted, further applications


development needs to occur with the use of gas chemistry and  our IR camera setup to make the backside technique viable.  One interesting effect is that NUV optical views become more  reflective when remaining nitride has been etched away, and  this could potentially become an important endpoint


indication.  Future exploration will involve the use of varying  beam dose and gas chemistry flux to optimize the milling and  minimize the gallium implantation, thus possibly improving  the real-time IR image that is achieved.


Figure 15: IR image viewing through ~200um silicon. 1064nm  light was used.  HFW is 150um.


Figure 16: 1064nm image during backside trenching of a


50um x 50um box. One can see that the box becomes opaque, because of gallium implantation and suspected lack of gas


flux.  HFW is ~150um.


Figure 17: 525nm image taken during the backside trenching. The mirror effect is very noticeable when using the 525nm


light, even more so than 1064nm (Fig. 15).


Future Developments


The IR imaging system as it is developed today is quite


functional and provides excellent sub-surface imaging data all  the way from the NUV to visible and NIR regions of the


spectrum. As the camera is integrated onto different platforms, other design improvements may be made. This might include  on-axis imaging such that top down viewing could be done


simultaneously with the FIB and the IR camera with no


intermediate tilt action, thus making operation of the camera  and FIB even more facile and functional. In addition, we may  consider different illumination techniques to further improve  and broaden the range of wavelengths that could be utilized


thus making the camera apparatus useful for an even larger


applications space. The use of other cameras could push the


spectra further into the infrared band, and it would be


interesting to note the difference in doped silicon absorption


for backside edit applications. Another possibility for future


work is in synthetic image reconstruction, as it may be a


possibility even when the optical image is off axis.


The IR camera system substantially improves the ease of use  and applications range of the FIB. By using the optical column  one can see buried structures all but invisible to a SEM or FIB  beam, and increase the success rate of frontside and backside  CE, as well as other related FIB operations with no charging  effects. The flexibility and operational advantages of the


optical column can make it a worthy addition to many FIB and  FIB-SEM platforms. By using easily selectable illumination


wavelengths, one can optimize the image for layer visibility, contrast, and resolution. The quality of the image obtained by  the IR camera rivals or exceeds traditional optical based


imaging microscopy techniques, due to its apochromatic


objective system. Since the system uses a high magnification  objective, the microscope can also be used to estimate depth of  a subsurface feature with the depth of field by shifting focus


from surface to subsurface image views. Backside edit could  benefit from a camera that could image longer wavelengths


than a silicon CCD due to ion implantation and the associate  loss of NIR transparency.


This work was performed by Battelle (Battelle.org) and TSS


(TechnicalSalesSolutions.com) at Battelle’s microelectronics  research facility in Columbus, Ohio. Special recognition goes  to Michael Frome of TSS for mechanical engineering


expertise and technical support. Steve Herschbein of Global


Foundries provided key information on the effects of gallium  implantation and use of gas chemistry for backside


visualization.


References and Notes


[1] Lee, R., Antoniou, N., “FIB Microsurgery on Flip-Chips


from the Backside,” Proc 24th International Symposium for


Testing and Failure Analysis, Dallas, TX, November 1998, pp. 455-459.


[2] Arthur D Edelstein, Mark A Tsuchida, Nenad Amodaj,


Henry Pinkard, Ronald D Vale, and Nico Stuurman (2014),


Advanced methods of microscope control using µManager


software. Journal of Biological Methods 2014 1(2).


[3] J. C. Dainty, Laser Speckle and Related Phenomena,


Springer, Berlin (1975).


[4] K.N. Hooghan, K.S. Wills, P.A. Rodriguez, S.J.


O’Connell, “IC Device Repair using a FIB System: Tips,


Tricks and Strategies”, ISTFA 1999 Proceedings, pp. 247-255.


[5] Nunn, S., “How to Optimize Spatial Resolution in IR


Microscopy and Imaging,” R&D Magazine, Aug. 16, 2004.


[6] Lasch, P., Naumann, D., “Spatial Resolution in Infrared


Microspectroscopic Imaging of Tissues,” Biochimica et


Biophysica Acta (BBA), Vol 1758, Issue 7, July 2006, Pages  814-829.


[7] Rue, C., Herschbein, S., Scrudato, C., “Backside Circuit


Edit on Full-Thickness Silicon Devices,” ISTFA 2008, pg.


141-150.


[8] R.H. Livengood, V.R. Rao, “FIB Techniques to Debug


Flip Chip Integrated Circuits”, Semiconductor International, March 1998, pp. 111-116.


[9] Tesch, P., Smith, N., Martin, N., Kinion, D., “Nanoscale to  Millimeter Scale Milling with a Focused Ion Beam


Instrument,” EIPBN Conference, Portland, Oregon, USA.


May 2008.


[10] R.A. Falk “Near IR Absorption in Heavily Doped Silicon – An Empirical Approach”, Proceedings of the 26th ISTFA,


2000.


[11] Herschbein, S. Personal communications, July 2015.


Along the line profiles indicated by white horizontal dashed  lines in Fig. 4(A) and (C) clear differences between the two  channels exist on some areas of the sample. In the highlighted  region (i), a transition from occurs from insulating STI to a  contact that has been polished away sitting on a p-doped area. The dC/dV profile remains completely flat in region (i), whereas the sMIM-C profile contains a shoulder related to the  change in material in this region. Region (ii) contains the ndoped storage well and region (iii) contains insulating STI. The contrast difference between ii and iii for the dC/dV profile  is small, whereas sMIM-C shows an obvious difference.


Cross-Sectional Dopant Profiling


In addition to semiconductors, sMIM can also provide  physical information on non-doped materials. Whereas SCM  is generally limited to semiconductor materials with doping  levels of 1015 to 1019 cm-3, sMIM provides information for  insulators, semiconductors and metallic regions of the surface.


Figure 5: Cross-sectional images of the photocathode region  of the image sensor. The A) dC/dV-phase, B) dC/dV-amplitude  and C) sMIM-C images were acquired simultaneously. Note  here that features such as the metal layer and polysilicon  gates are visible in the sMIM-C and not in dC/dV-Amplitude.


Figure 5 contains (A) dC/dV phase, (B) dC/dV amplitude and (C) sMIM-C phase images of the area in Fig. 2(A). In dC/dV  amplitude the highly-doped polysilicon gates give a null  signal, and appear similar to the dielectric layers which


surround the gate. Additionally, the STI appears similar to


both the gate and the dielectric layers. In the sMIM-C case, the  polysilicon gates, along with the photocathode and STI are all  differentiated.


We expect the dopant concentration in the labeled areas in Fig. 5 to proceed from greatest to least as: polysilicon gates, p-type  pinning layer, p-type substrate, followed by n-well. While this  is not obvious from examining the images at a single bias  voltage, in the following section it will be demonstrated that  sMIM is sensitive to these differences in concentration.


Site-Specific Capacitance-Voltage Spectroscopy


Site-specific capacitance voltage curves were recorded by  placing the AFM tip at a location on the sample and then  ramping the DC bias voltage while recording the sMIM-C  signal. Figure 6(B) presents curves from obvious n-type and ptype regions on a planar sample. The curve at location 1 has  the expected behavior (positive slope) of an n-type region  under standard MOS C-V testing [5]. The same holds true for  the p-type region at location 2.


Figure 6: Site-specific capacitance - voltage curves taken at  locations 1 and 2 showing n-type and p-type response..


C-V measurements at three different locations on a crosssectional sample were performed. The three locations were:


(1) p-type pinning layer, (2) n-type photocathode, (3) p-type  substrate as indicated in Fig. 7. Clear differences between the  n, p and p+ regions are evident from the C-V curves. Being  able to map out the region with a sMIM-C image at a single  fixed bias and sampling different regions with a C-V curve  allows for a thorough understanding of the device under test.


While the situation may be more complex than a simple MOS  capacitor, being able measure CV curves using sMIM presents  a great advantage. One can use these curves to reveal  differences between a known good location and a failing  location on a die. The curve is more informative than a single  image at a fixed bias.


Figure 7: C-V measurements on a cross-sectional sample in  three different locations, each with different dopant


concentrations.


A CMOS image sensor was analyzed using two different  models of scanning microwave impedance microscopes, both  capable of simultaneous sMIM and dC/dV imaging. It was  demonstrated that the sMIM-C channel provides new  information, not available via the SCM dC/dV amplitude and  phase measurements. SMIM-C provides contrast in insulating  and conductive or very highly doped regions of the sample  that is not available from dC/dV measurements. Yet, being  able to simply access the dC/dV channel is still advantageous  for determining carrier type.


Site specific C-V measurements were taken using the same  microscope system and used to reveal differences in dopant  concentrations and type. This provides an attractive possible  route towards quantitative dopant profiling in modern  semiconductor devices.


[1] J. R. Matey and J. Blanc, “Scanning Capacitance  Microscopy,” J. Appl. Phys., Vol. 57, p. 1437, 1985.


[2] E. Fossum, D. Hondongwa, “A Review of the Pinned  Photodiode for CCD and CMOS Image Sensors” IEEE  Journal of the Electron Devices Society, Vol. 2, No.3, p.33,


2014.


[3] R. Stephenson, A. Verhulst, P. De Wolf, M. Caymax, and  W. Vandervorst, “Nonmonotonic Behavior of the Scanning


Capacitance Microscope for Large Dynamic Range Samples,”


J. Vac. Sci. Technol. B., Vol. 18, p. 405, 2000.


[4] W. Kundhikanjana, K. Lai, M. A. Kelly, and Z.-X. Shen, “Cryogenic microwave imaging of metal-insulator transition  in doped silicon.” Rev. Sci. Instrum., Vol. 82, p. 033705,


2011.


[5] S. Pendyala, D. Albert, K. Hawkins, M. Tenney, “dC/dV  and CV Characterization of Gate Resistance Defects in  eDRAM Circuits”, ISTFA 2013: Proceedings from the 39th  International Symposium for Testing and Failure Analysis, p. 255, 2013.


Alleviating Sample Charging during FIB Operation


Q. Liu1, H. B. Kor1, Y. W. Siah1,2, C. L. Gan1,2


1Nanyang Technological University, Temasek Laboratories@NTU, 9th Storey, BorderX Block, Research Techno Plaza  50 Nanyang Drive, Singapore 637553.


2Nanyang Technological University, School of Materials Science & Engineering,


50 Nanyang Avenue, Singapore 639798.


liuqing@ntu.edu.sg, +65-6592 3725


Dual-beam focused ion beam (DB-FIB) system is widely used  in the semiconductor industry to prepare cross-sections and  transmission electron microscopy (TEM) lamellae, modify  semiconductor devices and verify layout. One of the factors  that limits its success rate is sample charging, which is     caused by a lack of conductive path to discharge the  accumulated charges. In this paper, an approach using an insitu micromanipulator was investigated to alleviate the  charging effects. With this approach, a simple front side  semiconductor device modification was carried out and the  corresponding stage current was monitored to correlate to the  milling process.


DB-FIB is a versatile and prevalent tool in many areas of  science and engineering [1-6]. However, one of the issues that  affect the performance is that charges from the ions and  electrons can accumulate on the sample if the sample does not  have adequate conductivity. As a result, the charged samples  would drift during operation or even lead to electrostatic  discharge (ESD) failures [7]. Many approaches have been  reported to alleviate the charging effects, such as coating the  sample with thin conductive films [7]. In most cases, the  deposited thin conductive films are carbon, gold or some    metal alloy. However, coating the sample surface with a thin  conductive layer may shield the real surface information, resulting in non-accurate surface characterization. After  characterization, additional removal process is also required  before carrying out further electrical tests of the sample. Another approach used is applying low operating voltages    and this method is usually used to characterize organic  samples [8]. Nevertheless, low operation voltages may  sacrifice the image quality and prolong the milling process.    In this study, an alternative and simple approach using in-situ  micromanipulator was explored to reduce and even eliminate  the charging effects.


Experimental Details


In this investigation, a commercial quad flat package was


used. The top passivation layer of the chip is approximately


3.5 µm in thickness. The package was first decapsulated with                                                                                                                    a Nippon Scientific PS103S system. The ion milling and


imaging were carried out using FEI Nova Nanolab 600i DBFIB system integrated with in-situ Omniprobe  micromanipulator. All the experiments were conducted on the  same sample at locations with the same structure and the  sample was not taken out of the FIB system. Moreover, the  rest of the parameters (0.28 nA beam current, contact window  size, working distance etc.) were kept the same during the  experiment.


Figure 1(a) shows the ion beam image of the chip after milling


a contact without in-situ micromanipulator probing.             The yellow square indicates the intended contact via location.


It is at a lower position as compared with the actual milled


contact window. Cross-sectional scanning electron


microscope (SEM) imaging was carried out with FIB to


obtain the profile of the milled contact and the SEM image is


shown in Figure 1(b). The cross-sectional cutting direction is


indicated in Figure 1(a) by a green line. In Figure 1(b), the


desired contact location is indicated by the blue box. Metal


line A is desired to be connected and probed later. Due to the


image drifting during the milling process, the contact hole


that was milled extended onto the adjacent metal line B. As a


result, metal lines A and B will be shorted (indicated with red


circle) if metal deposition is carried out.


2 µm


Cross-section


Figure 1: (a) Ion beam and (b) cross-sectional SEM images of  a micro-chip after opening a contact window without in-situ  micromanipulator probing


During the contact window milling, the stage grounding  current, which is known as end point detection (EPD), is  plotted as a function of milling time and the result is shown in  Figure 2. Segments A, B, C, D and E indicated in Figure 2 are  the stage grounding currents obtained during milling of  Si3N4 , Si3N4/SiO2 interface (A-B), SiO2, SiO2/Al interface (B-C) and Al layer (C-D), respectively. Although drifting  occurred during the milling, all the layers could be detected.


Figure 2: Stage grounding current during milling


In order to mill the contact opening at the desired location and  to prevent short circuit between adjacent lines, an in-situ  micromanipulator probe tip was used to discharge the  accumulated localized surface charges. Figure 3(a) shows the  schematic diagram of the probing and milling set-up. During  the milling process, the probe tip was placed near the milling  position, typically 1 to 2 µm away. The surface charges can be  discharged immediately. An ion beam image of the chip after  milling a contact with in-situ micromanipulator probing is  shown in Figure 3(b). No drifting was detected and the  intended square contact was obtained at the desired location. The cross-section of the milled contact was characterized with  FIB and shown in Figure 3(c). The contact was opened above  metal line A.


50


150


Milling Time (s)


Figure 3: (a) Schematic diagram of probing and milling setup, (b) ion beam and (c) cross-sectional SEM images of a  micro-chip after opening the contact window with in-situ  micromanipulator probing


The stage grounding current and the circuit to capture the  current are shown in Figure 4. In Figure 4(a), Rpassivation and  Rprobe are the resistances of the passivation layer and probe tip, respectively. Rsubstrate is the resistance of metal lines and silicon  substrate. Thus, with the in-situ micromanipulator probing, the  stage grounding current can be described by Equation (1):


probe


emmision


beam


stage


I


(1)


In the above equation, stageI is the stage grounding current,


I  is related to the incident beam current, emmisionI  is the  emitted electrons and ions current when the incident beam  interacts with the sample and probeI is the current that is due to


1 µm


8.0x10-11


1.6x10


E


2.4x10 Stage Current (A)3.2x10


4.0x10-10


-10


End Point Detection


Ion Beam Probe


Passivation


Substrate


the charges that flow through the in-situ probe tip to the probe  grounding.


During segments A, B and C in Figure 4(b), the resistance of  the passivation layer is much larger than that at the probe tip, thus most of the charges are discharged through the probe tip. As a result, the stage grounding current is constantly close to


0. Note that Si3N4 and SiO2 layers in the passivation cannot be


differentiated clearly.


At segments D and E, the passivation was removed and the top


metallization layer on the chip was exposed. The resistance of  the discharge path through the substrate is comparable with  that through the probe tip. Thus, the stage grounding current  can be detected.


币


777


Stage currentA


8.0x10 a1.6x10


6


Rprobe


2.4x10


U


-11


Figure 4: (a) Stage grounding current circuit and (b) stage  grounding current during patterning with in-situ


micromanipulator probing


In order to detect the different layers in the passivation, the  charges that are discharged through the probe tip should be  monitored instead. Hence, a modified stage grounding current  circuit was implemented. In this modified circuit, the probe tip  was connected to the stage, such that some of the charges  discharged through the probe tip will go through the stage to  the stage grounding. Before milling the micro-chip, verification on the functionality of the modified circuit was  conducted. Figure 5(a) shows the schematic diagram of the  experiment. Only the probe tip indicated by the black box was


milled to keep the circuit simple. Figure 5(b) shows the  standard circuit of the stage grounding current without  connecting the probe tip to the stage, and Figure 5(c) is the  modified circuit.


Rpassivation


Rsubstrate


nRprobe


办T77(b)


3.2x10


V


市17(c)


Figure 5: (a) Schematic diagram of probing and milling setup. Stage grounding current circuit with (b) standard and (c) modified in-situ micromanipulator probing


Figure 6 shows the stage grounding currents detected with  standard and modified in-situ micromanipulator probing. It can  be observed that, with the standard probing, the stage  grounding current is close to 0. With the modified circuit, the  stage grounding current is constantly close to 125 pA. This  implies that the stage grounding current could be monitored  with the modified circuit. Not all the charges were discharged  through the probe tip to probe grounding.


Figure 6: Stage grounding current during milling of probe tip  with standard and modified in-situ micromanipulator probing


Detection of different layers in the passivation could be  achieved with the circuit modification discussed above. Figures 7(a) and (b) show the modified schematic diagram and  circuit of milling the micro-chip, respectively. In the modified  circuit, probeI  can be further described by Equation (2):


'


(2)


In the above equation,


is the current due to charges  flowing through the in-situ probe.


is the current that


discharges the accumulated surface charges through the in-situ


3.2x10-10


probe and to the stage grounding. Thus, Equation (1) can be V further described by Equation (3):


a2.4x10 u


艹





''


(3) 0a1.6x10 6


8.0x10


药1.0x10-10


市177


5.0x10-11


Figure 7: (a) Schematic diagram of the probing and milling


16


24


set-up and (b) stage grounding current circuit with modified


in-situ micromanipulator probing


The stage grounding current during milling of the micro-chip  is shown in Figure 8. During milling of the passivation layer (segments A, B and C), the resistance of passivation layer is  much larger than the probe tip and all the accumulated charges  were discharged through the probe tip. From the probe tip, the  charges were further discharged through both stage and probe  grounding. Thus, any changes in the discharging current due to  milling of different passivation layers (Si3N4 and SiO2) can be  captured by this set-up. During milling of metallization layer (segments D and E), the accumulated charges can also be  discharged through both stage and probe grounding. Note that  all the measured currents are less than those in Figure 2.


Ion BeamProbe


Figure 8: Stage grounding current during patterning with  modified in-situ micromanipulator probing


Besides the application in device modification, this approach


can be applied to capture SEM images with improved quality. Figures 9(a) and (b) show the cross-sectional SEM images of  the micro-chip without and with in-situ micromanipulator  probing, respectively. It can be observed that the charging  effect was much reduced when the in-situ micromanipulator  was applied. The image captured also has less distortion.


1.5x10-10


2.5x10


3.0x10


3.5x10


Isolating probe and stage


Rsubstratew√


2.0x10-10


Connecting probe to stage


Figure 9: Cross-sectional SEM images of the micro-chip (a)


without and (b) with in-situ micromanipulator probing,


captured at 5kV, 0.4nA


In conclusion, the capability of the DB-FIB was improved with  the in-situ micromanipulator probe. Charging of samples could  be eliminated by discharging the charges through the probe tip. Precise milling of contact vias at desired location can thus be  performed. Si3N4 and SiO2 layers in the passivation can also be  detected and captured if the probe is electrically connected to  the stage. Furthermore, enhanced SEM images with reduced  charging and distortion can be obtained with this approach. However, the probe tip should be placed close to the region of  interest to make this approach successful, typically within a  few microns.


[1]          D. Donnet, O. Sidorov, P. Carleson, C. Rue, R. Alvis, and S. Madala, “Localized FIB Delayering on


Advanced Process Technologies”, Proc. 21st IPFA, Singapore, July 2014, pp. 146-149


[2]          S. Tan, R. Livengood, Y. Greenzweig, Y. Drezner, R. Hallstein, and C. Scheffler, “Characterization of Ion  Beam Current Distribution Influences on


Nanomachining”, Proc. 38th ISTFA, Phoenix, AZ,


Nov. 2012 , pp. 436-439


[3]          H.B. Chong, B.V. Leer, V. Narang, and M.Y. Ho,


“Sideways FIB TEM Sample Preparation for


Improved Construction Analysis in TEM”, Proc. 19th  IPFA, Singapore, July 2012, pp. 303-306


[4]          P.K. Lee, B.Y. Choi, and M.J. Kang, “Assessment of  mobility and bio-availability of heavy metals in dry  depositions of Asian dust and implications for


environmental risk”, Chemosphere, 2015, pp.1411-


1421


[5]          Y. Huang and D. Cockayne, “Control of


nanostructures induced by ion sputtering”,


Nanotechnology, vol. 18, 2007


[6]          F.A. Stevie and L.A. Giannuzzi, “FIB Applications: A Historical Perspective”, Microscopy and


Microanalysis, vol. 20, 2014, pp. 294-295


[7]          V. Ray, “Elimination ESD damage during FIB


operation”, FIB User Group Meeting  40th ISTFA,


Huston TX, Nov 2014


[8]          D.A.M.De. Winter, C.T.W.M. Schneijdenberg, M.N. Lebbink, B. Lich, A.J. Verkleij, M.R. Drury and


B.M. Humbel, “Tomography of insulating biological  and geological materials using focused ion beam


(FIB) sectioning and low-kV BSE imaging”, Journal  of Microscopy, vol. 233, 2009, pp. 372-383


Circuit Tracing on Integrated Circuit Using  FIB Passive Voltage Contrast Effect


Alexander Sorkin, Chris Pawlowicz, Alex Krechmer


TechInsights 3000 Solandt Road, Ottawa, ON, K2K2X2, Canada.


Michael W. Phaneuf


FIBICS 1431 Merivale Rd #100, Ottawa, ON, K2E0B9, Canada.


Competitive circuit analysis of Integrated Circuits (ICs) is one  of the most challenging types of analysis. It involves multiple  complex IC die de-processing/de-layering steps while keeping  precise planarity from metal layer to metal layer. Each step is  followed by Scanning Electron Microscope (SEM) imaging


together with mosaicking that subsequently passes through


an image recognition and Graphic Database System (GDS)


conversion process. This conventional procedure is quite time  and resource consuming. The current paper discusses and


demonstrates a new inventive methodology of circuit tracing  on an IC using known FIB Passive Voltage Contrast (PVC)


effects [1]. This technique provides significant savings in time  and resources.


The conventional approach in the circuit analysis process flow  is shown in Figure 1. Starting from an IC diffusion level sample  study, identification of different IC blocks and their


functionality is estimated. A Region of Interest (ROI) is


defined, following by IC die delayering into individual metal


layer sets. Large mosaics of images are acquired by SEM of


the ROI with high magnification and high resolution for each  of the IC metal layers [2]. A significant number of images of


the IC die layers are collected and then passed through an


automated process of image recognition and GDS extraction. Layout circuitry is then analyzed by IC engineers. The entire


process is highly time and resource consuming.


To add to the complexity, sometimes the signal of interest


goes ‘outside’ of the ROI boundaries, and the entire process  must be repeated after a new ROI is defined. This signal


‘chasing’ process might need to be repeated multiple times. Duration, cost and effort can be significant (and prohibitive). The project time and effort estimates become less


predictable. Imaging the entire die is generally not feasible – on a modern device it is too expensive and time consuming.


Figure 1. Conventional IC circuit competitive  analysis process flow.


The principal of FIB PVC


In Figure 3, Ga Ions charge floating structures to a positive


potential. The secondary electrons generated when the Ion


beam strikes this sample are attracted back by the strong


positive electrical field. Very few of them reach the Secondary  Electron Detector (SED); therefore, the structure appears


black on the FIB image. Likewise, grounded structures


transfer the charge to the ground and so do not accumulate  any positive charge thus allowing secondary electrons to


easily escape the grounded structure.  The secondary


electrons leaving the grounded structure easily reach the


SED. As a result, the grounded structures appear bright in the  FIB image with higher contrast compared to the floating


structures.


FIB PVC is a well-known method for Failure Analysis (FA)


investigation of signal continuity [1].


In the following case study, the PVC technique is used to


trace a particular signal on an IC. Using Back Side (BS) sample  preparation methods, the entire bulk Si is removed from the


IC keeping all the metal interconnects intact [3]. The metal  interconnects are then further analyzed with the PVC


technique.


To incorporate a dynamic approach, an externally grounded  probe tip (Figure 2) is introduced into the FIB chamber.


External manipulator control allows dynamic grounding of


any signal of interest to investigate its propagation. Another  option allowing an externally grounded signal to be brought  onto an IC is to use FIB to deposit a conductive layer above a  dielectric patch of SiO2 deposited in advance (Figure 4


Bottom).


Gnd


Ga+


e-


Secondary electrons  easily escape


grounded trace


toward detector


(bright white)


Secondary


electrons cannot  escape from


positively charged  surface (dark)


(Bulk Si is removed)


CELLU XICmDpe e c2m0rov.60 m


trags Mide Emchron


Figure 3. PVC concept (Top). FIB image showing the


resulting PVC effect (Bottom).


Grounded  probe tip


(Metal 1 Level)


SL


Figure 2. External ground concept (Top). FIB image of  grounded probe tip contacting transistor node (Bottom).


Case study: Signal tracing ‘up-stream’ to localize the


Location


controller circuitry


Unknown


Search Direction


Start PointKnown


In this case study, numerous Power Switch Transistors (PST) are distributed inside an IC’s functional block (Core). The


Controller


PST’s control signal is distributed by long buffer chains (Figure  5). The power control circuitry is at the origin of the control


Buffer82


Buffer 2


Buffer I


signal buffer chain, but its specific location is not known. The  project goal was to identify and localize the controller


李孝平


0000李宾常HH


circuitry block.


Method concept:


四☑


☑


所


An externally grounded signal is connected by FIB conductive  deposition to one of the buffer Input nodes.  The FIB PVC


凹


回


technique is then used to identify the previous buffer output  node (Figure 6). By shorting the input and output nodes of


the found buffer (Figure 4 Top), the ‘bright’ ground signal is


闻


内日


transferred further upstream to the next buffer in the chain. By making ‘jumps’ from the buffer’s input to a previous


中


buffer’s output, one can trace the power switch control signal


菌月日□


□司


InOut-InOut


580


upstream toward the controller circuit (Figure 5).


Analysis:  The enable signal is generated by an FPGA and is  output to the J1 and P2 connectors through a zero ohm resistor  pack (Z5).  Therefore, the short could be related to the solder  joints (connectors, resistor pack, BGA joints, etc.), within the  FPGA (die or interposer), or internal to the PCB.


Figure 1: Overall block diagram of assembly with critical  components highlighted.


Location A - Transition from L10 to L6.


Location B - Transition from L6 to L4.


Location C - Transition from L4 to L5.  The characteristic  impedance was pulled to GND at this location, indicating the  short was in close proximity to this PTH.


AB


ZS


PCB Pad


Cap


Termination


C15


Figure 2: Composite image of assembly depicting the enable signal’s  routing through the PCB.  The different internal layers are  represented by different colors.  Locations A, B, and C highlight the  layer transitions through the plated through holes (PTHs).


|Eile Edt yew Setup Uibios Applcabions Hep 17575 Waredarm Baktreaty _x Run/Slop AcqMode [AverageTrigIntenalClock[200kHz □ ASS A?|Eile Edt yew Setup Uibios Applcabions Hep 17575 Waredarm Baktreaty _x Run/Slop AcqMode [AverageTrigIntenalClock[200kHz □ ASS A?|Eile Edt yew Setup Uibios Applcabions Hep 17575 Waredarm Baktreaty _x Run/Slop AcqMode [AverageTrigIntenalClock[200kHz □ ASS A?|
|---|---|---|

|Pulte|Ampitude 财|Hcasurement|

4.Ovs 01几


70.09176%


5Mean C1A


43.197960


MinC1A


4.9235140


PRPK CT 入


75.07721Ω


Wovelrrm


C1 10.00QAV


R1 10.000Aly


R2 10.00QAiv


Cursers(Mn R1)d17.52696m d2 7.97455m


ad 447.596mm ad/2 223.798mm


R2


R210.000AC351PM 9/13/2013


Figure 3: TDR plot showing characteristic impedance (y-axis, 20Ω/div) versus time (x-axis, 500ps/div) of a good assembly (blue) and a failing assembly (purple).  Based on the PCB stack-up, the  signal layer transitions at the plated through holes could be roughly  determined due to their relative spacing to the GND plane on layer 7, which directly affects characteristic impedance.


In a subsequent X-ray inspection at this PTH (not visible  optically), it was noted that the C15 capacitor termination  extended past the PCB solder pad region and appears to  contact the unprotected via (no solder mask).  Reference  figure 4.


A dimensional evaluation confirmed that the critical  termination spacing for the capacitor case code presented  opportunities for the capacitor to short to the adjacent plated  through holes once installed.  TDR facilitated quick fault  isolation of the short to an obscure via located under a  capacitor that was unrelated to the circuit of interest and not  visible upon optical inspection.


Figure 4: X-ray image depicting the location of the short between the  PTH and C15 cap termination, as indicated by the red box.


000


Figure 5: Overall image of PCB pads with C15 removed.  The L4 to  L5 via is indicated by the left arrow.


Case Study 2


Program X Communication Issue


The Problem


The customer reported communication failures that were  isolated to cable assemblies while retrofitting a fielded system.  Additional troubleshooting revealed the suspect cable’s  Ethernet interfaces could connect at 10 Mbps but not at  100Mbps.


Analysis


Preliminary investigation revealed no obvious defects: continuity was verified through the cable, no contamination on  the contacts, no mechanical damage to the assembly, etc.  Because of the high data rates involved at the system level, TDR was utilized to evaluate the signal integrity of the  Ethernet transmit (TX) and receive (RX) pairs.  A distinct  characteristic impedance discrepancy was noted when  comparing twisted pairs of passing and failing assemblies – passing assemblies measured 75Ω and failing assemblies


measured 110Ω.  Additionally, it was noted that correct  characteristic impedance values could be obtained on the  failing assemblies when crossing the pairs (i.e. TX+ to RXand TX- to RX+) – an indicator the assemblies were  manufactured with split pairs.  Destructive analysis was  performed and provided conclusive evidence that the cable’s  Ethernet lines were manufactured incorrectly.


R4▲20.002/d西00002蔺12:02PM 12/7/2011


v2 34.89Q AV 4.324Q


Figure 6: TDR plot of failing cable assembly highlighting the  characteristic impedance difference between a twisted pair and a  split pair.  (Y-axis – 20Ω/div, X-axis – 2ns/div)


TX+


R3


Figure 7: Correct twisted pair configuration per the drawing


|Ble bok w 200||woices|applicaions tao Inggored||Bokdoay 出管 x|
|---|---|---|---|---|---|

|0|||AcqMede |AverageTigIrternel Clock 国|200KHz|□ ?|

|Pulse|Ampitude||**||后 附园 Waveform|

TXR15.000ΩMiy


RX+


Measunement


RXWrong (Split Pair)


Cursnrc(Min R1)30f


R25.000QAIV


V149.05412 4299'02606


Figure 8: Ethernet configuration on failing cable assemblies


di182919km d21.62920km Ad 6.01005mm 95k8bO


Ad/2 3.40042mm


Conclusion:  The “twisted pairs” on failing cable assemblies  were not configured per the drawing.  This induced cross-talk  on the transmit and receive signals, affecting the system's  immunity to common mode noise.  TDR facilitated quick  characterization of the transmission environment to determine


81▲5.0000M0.00


肆中日.℃3139PM 4/18/2013


root cause non-destructively.


Case Study 3


Cable Voltage Standing Wave Ratio (VSWR) failure


Three initial build semi-rigid cable assemblies marginally  failed VSWR testing using a Vector Network Analyzer (VNA).  The cables have a BMA (Blind Mate - A) and SMA (SubMiniature - A) connector on opposite ends.


|Be Edt yow Salip Liites Appications|10783 Waveloims|Tektronjic|河区|
|---|---|---|---|

|Run/ Stop|AcqMode[AvoragoTriglrternalClock200KHz|□|hpp k?|

|Pu se ▼ Amplitude|职产照期|职产照期||

|178.80|||Lursors (Mn C1)|

V150.87150


TDR was utilized to evaluate characteristic impedance across


v2198.3682&v -147.4970


the length of the cable.  A large impedance discontinuity and


d111.7679m


subsequent ringing in the time domain were observed at the


d216.9557m


Rx+ to RxAd2 2.59440m&d 5.18881m


SMA connector end.


Measurement


|Be sar 白势力|n0|Bun/Skip Acq Mode Average|Tig lntenel Clock|日 200KHz|□|?|
|---|---|---|---|---|---|---|

|Pulse|AmpRtude|wm*|||E M间 Waveform|▲柒|

yot


Of


jeo yhites Applestonsp lnggerod


Toktroatyx


Waveform


Tx+ to RxR4 20.000/div


R15.000ΩMiv R25.000QMV


Twisted Pair


R35.0000MV Measurement


R4D


Corsors(to R1)


21202


9130.562 301


C120.00QASN


TX83-5.000QA0.69


1℃11:23.AM 4/18/2013


Figure 9: TDR plot at BMA connector (left) with SMA (right)


RXCorrect


terminated with an ideal 50Ω termination.  Y-axis – 5Ω/div, X-axis – 500ps/div.


Figure 10:  Higher magnification image of failing cable at the SMA  connector.  Blue curve represents a non-terminated SMA and purple  represents a 50Ω terminated SMA.  An impedance discontinuity (5Ω  delta) is apparent just prior to the contact points at the termination,


suggesting the impedance discontinuity is within the SMA shell.


Figure 11: X-ray evaluation at SMA connector - There were no  indications of solder wetting to the top of the connector's solder well.  This feature correlates well with an increase in characteristic  impedance for the length of this anomaly.


The failures were isolated to within the SMA connector and  were related to incomplete solder fill in the solder well due to  an inadequate solder process.  Rework of the connector solder  joints allowed proper solder joint formation, and subsequent  VSWR tests were within specification. The program elected to  replace the connector type to one with a shorter solder well, which was more suitable for the supplier’s soldering  processes.


Limitations of TDR


As with any analysis technique, there are limitations.  TDR is  typically not useful in troubleshooting power plane to ground  shorts due to the presence of decoupling capacitors, which  present a low impedance to the instrument at high frequencies.  In addition, the TDR is equipped with SMA terminations and  intended to operate in a 50Ω controlled impedance  environment.  In reality, not all of the boards or cables  manufactured at Raytheon are equipped with these interfaces; therefore, some level of improvisation is often needed to  achieve an acceptable connection to device under test.  Often, this can degrade the edge rate of the TDR pulse, significantly  affecting bandwidth and spatial resolution.  This is largely a  function of the physical layout of the unit under test and needs  to be evaluated on a case by case basis.


[1]  Tektronix, TDR Impedance Measurements: A Foundation  for Signal Integrity. Application Note. www.tektronix.com


Failure Analysis of Yellow Banding On Optically Bonded Touch Screen


Qing Gu, J Lewis, Danhua Xu


Microsoft Corporation, Redmond, WA, 98052, USA


Yellow banding is a phenomenon occurring at an edge(s) in an  electronic optical touch screen when the display module emits  certain background light. Although it is commonly recognized  that the discoloration turns yellowish due to display liquid  crystal (LC) cell gap change, the mechanism to create the color  change can be different depending on the display designs. This  paper discusses an approach to investigate a particular  mechanism of forming yellow banding caused by uncured edge  fill UV adhesive.


Touch displays typically use either air gap bonding or optical  bonding for touch panel attachment. Optical bonding applies  optically clear adhesive (OCA) over entire surface between  liquid crystal module (LCM) and touch sensor panel (TSP), while air gap bonding applies a pressure sensitive adhesive (PSA) at the perimeter of inactive area. OCA can be either dry  film or in a form of liquid or semi-liquid. Each design has its  own advantages and drawbacks, such as difference in optical  performance [1]. However, yellow banding and yellow spots as  cosmetic display defects have been reported regardless of  bonding methods used. This paper discusses an approach to  investigate the mechanism of forming yellow band after  application of dry film OCA to bond a touch screen.


For a dry OCA film bonded display, yellowing phenomenon  can be classified into following categories:


a) Interference of TDM and rest of the device, such as high  profile components/shields pushing onto the bottom of the


TDM module, or FPC/FFC being pinched into the bonding  between TDM and enclosure, or stress exerted to the TDM  due to enclosure warpage/twist.


b) OCA related yellowing, which could be caused by OCA  lamination, or the mechanism discussed in this paper.


c) LCM issues, such as out of spec LC cell gap or LC panel  seal damage.


In order to determine the cause of yellowing in display screen, some general practices below can be followed:


1. Debond TDM from enclosure, and relax the TDM for  couple days. If yellowing disappears, it’s due to  interference problem, and if yellowing persists, then  proceed to Step #2.


2. Debond TSP from LCM. If yellowing disappears, it is  OCA related problem, otherwise the problem is in LCM.


This paper discusses a failure related to uncured edge fill  adhesive. The failure mechanism has been investigated and  experiments have been performed. Solutions are also proposed  to mitigate the problem in this study.


Dry Film OCA Bonded Display


With Edge Fill Adhesive


Figure 1 shows layer structure of a dry film OCA bonded  display and some critical dimensions in alignment of features  in stacks of TDM, OCA, and LC modules with edge fill  adhesive.


3.3mm2mmBlack


ITO


Black


0.8mm


Mask


Glass


Edge fill


OCA


0.7mm


fill


Polarizer


Tape


Glass 1


CoG


LC Glass 2


Tape Edge


Left side of screen


right side of screen


Figure 1: OCA bonded touch screen structure


Viewed from landscape oriented screen, asymmetric stacking  can be seen between left and right region as shown in Figure 1.  Chip on Glass (CoG) drivers embedded at same stacking layer  of LC can be placed on either side of the screen depending on  design. The edge with drivers is recognized as long edge while  the edge without drivers is noted as short edge. In this case the  left edge becomes the long edge.


When the touch display edge is not balanced, touching at the  edge can produce water ripple like visual effect known as edge  pooling. To reduce edge pooling effect, edge filled adhesive, usually an UV cure adhesive, is often used to fill into the gap  between TSP and LCM to fulfill geometric requirement. With


Figure 2: Yellow banding at left side edge


presence of driver(s), the depth of the edge fill requires much  deeper penetration at long edge than at short edge.


Because of physical limitation of such asymmetric layout, yellow banding is often found along left side of the screen in  such cases. For example, a yellow strip about 5mm wide  appears along the entire edge by the black mask and optically  most recognizable with gray background as demonstrated in  Figure 2. After removing TSP, yellow banding disappeared as  shown in Figure 3, which indicates that occurrence of yellow  band on long edge is associated with adhesion between TSP, OCA and LCM.


Profile Measurement of OCA


After removing TSP, optical line-profiling across yellow band  region is performed by using Cyber Technology GmBH noncontact optical profilometer CT-350T. Line scan demonstrates  a measurable surface topographic height of several micrometers  on yellow banding units, while such geographic feature is not  shown in non-yellow banding units as shown in Figure 4.


This geometric feature has been consistently recognized in  several different sample groups with and without yellow band  phenomenon. Because OCA is in dry film formation, the  change of OCA profile at yellow band region leads to the  investigation of all material in contact with OCA.


Figure 3: Yellow Banding disappeared When TSP Removed


What’s Under the Bump?


By zooming and focusing on the long edge at left side of display  module, shown in Figure 1, many components neighboring the  OCA are noted - black mask, touch display media as indium tin  oxide (ITO), edge filler, and polarizer. After an effort to  precisely remove the OCA film and the material underneath is  exposed, Fourier Transform Infrared (FTIR) Spectroscopy, using ThermoFisher Scientific Continuum Microscope with  Nicolet 6700 Analytical Spectrometer, is used to survey  materials as indicated and the results are shown in Figure 5. Clearly, edge fill adhesive is found under the bump with  mixture of OCA component and edge filler chemistry.


Edge Fill Adhesive


Since the edge fill adhesive is UV cured, deeper adhesive in the  long edge may not be fully cured. Again, non-cured edge fill  adhesive at long edge (left side) is confirmed by FTIR as shown  in Figure 6.


By comparing the FTIR spectra sampled from locations  adjacent to yellow banding, it is clearly shown that the  difference in IR absorption at 2930 cm-1 and 1636 cm-1, corresponds to a change in methylene group and diminishing  C=C bond, respectively. These changes reflect the chemical  state of cured and uncured chemistry of the edge fill adhesive  under UV exposure.


Yellow banding unit left side OCA top surface profile (line scan)Normal unit left side OCA top surface profile (line scan)Black mask


Black mask


10mm


品


版Lm1mhism


tooe


usm10*=品sin


to8mG1/


OCA. .


Figure 4: OCA surface profile


0 .0022Failed unit #1 location1


0.0000


0 0020Failed unit #1 location268000


OCA pried open and material


£ 000sFailed unit #2 location1


stick to the polarizer is analyzed


6A0Q0Failed unit #2 location2 C8010


e800


***4 *00 c


. . . .


8002 49000


4.9062


uesial


A DOGA


onlyonly


A*


* 0 * * * 1 6 * 6


14版


1M80tais5420120强1a***11345


"n


0*08


OCAEdge fill


CWOE1£ 8000


-A mix of OCA & edge fill


Figure 5: Edge fill adhesive under OCA


Ip


uncured


cued


cured


Figure 6: Un-cured edge fill adhesive at left side


Failure Mechanism


Without completion of curing due to insufficiency of UV  penetration, the edge fill adhesive maintains mostly low  viscosity, and migrates in between the OCA and LCM  polarizer, due to a combination of display warpage, heat, and  humidity. When uncured adhesive reaches the distance of nonblack-mask area, it is exposed to visible light and is cured and  hardened, forming a strip of bump. The bump is under the OCA  and sandwiched in between TSP and LCM. As a result, the  bump exerts stress to the liquid crystal (LC) layer, enlarges LC  cell gap of the nearby area, and causes yellow banding near the  bump. The described failure mechanism is illustrated in Figure


7.


Experiment


In order to verify the failure hypothesis, several experiments  are carried out to demonstrate the failure mechanism. Units


built through normal manufacturing process but well cured


edge fill adhesive by additional edge curing process were used  as control group. Experimental group was built with purposely  uncured edge fill adhesive. Both groups were sent to


temperature/humidity (TH) test along with UV exposure.


Yellow banding was reproduced from experimental group


while none of the units in control group shows yellow banding  as shown in Figure 8.


Solutions


Several solutions can be proposed to minimize or eliminate the  cosmetic defect in dry film OCA design for display  applications. One of the prominent solutions is to apply oversized OCA sheet further out at the long edge, which can  minimize spacing for edge filler to migrate underneath of OCA. With reduced depth and amount of adhesive needed to fill the  edge shown, as in Figure 9, the edge filler can be fully cured  and unable to migrate under OCA, similar to the one in short  edge.


Different designs can have different root causes of display  yellowing phenomenon, and for each specific design, many  factors can play different roles to create discoloration in the  form of yellowing phenomena. Some general steps can be  followed to find the root cause(s) of the problem, based on the  understanding that stress exerted to the LCM can enlarge the  LC cell gap and cause yellowing.


Authors sincerely thank Frank Huang, Paul Li, Garrett Bowen, Ramji Dhakal and To Lam for their valuable contributions.


[1] Birendra Bahadur, James D. Sampica, Joseph L. Tchon, Alyssa Butterfield, “Direct Dry Film Optical Bonding – A


Low Cost, Robust and Scalable Display Lamination


Technology”, Journal of the Society for Information Display, Volume 19, Issue 11, pages 732–740, November 2011.


OCA Polarizer Glass 1


LC Glass 2 a Light


Polarizer Glass 1


309


Stress


LC gap


Figure 7: Yellow banding failure mechanism


强国'nti


DUT


Reference


I week 55/85 TH+


1 week 55/85 TH+


10min UV+


I week 55/85 TH


1 week 55/85 TH


Figure 8: Yellow banding reproduced from experiment


Cured edge fillUncured edge fill


Figure 9: Extending OCA to make sure edge fill adhesive fully cured


Detection and Measurement of Intermetallic Thin Films Using EDX Line  Scanning


Carl Nail


EAG, Irvine, California, United States  cnail@eaglabs.com


Elementally characterizing intermetallic compounds (IMCs) to identify phases has routinely required relatively expensive  transmission electron microscopy (TEM) analysis. A study  was done characterizing IMCs using less expensive energydispersive x-ray (EDX) spectroscopy tools to investigate it as  a practical alternative to TEM. The study found that EDX line  scanning can differentiate phases by tracking changes in count  rate as the electron beam of a scanning electron microscope (SEM) passes from one phase to another.


Intermetallic compounds (IMCs) can form when at least two  dissimilar metals inter-diffuse at an adjoining interface. If the  inter-diffused metals can form an ordered compound with a  predictable stoichiometry at a given temperature, then they will  tend to form when the thermodynamic conditions are  favorable. IMCs are extremely important in assembly of  microelectronic components – they are the ‘glue’ that hold  assembled dissimilar metal joints together, such as in wirebonds on integrated circuits and in solder on contact pads. The  ordered lattices for IMCs result in precise stoichiometries, rather than the amorphous or gradient concentrations for  metals that do not form IMCs. Some of the more common  IMCs found in assembly applications are shown in Table 1 [1]. However, IMCs can also be a potential failure mechanism if  the IMCs become unacceptably thick or if particularly brittle  IMCs form at the bond lines. When this happens, the brittle  interfaces can allow cracking to occur under routine shear  loading encountered in typical service conditions. An early  example of this was the discovery that operating aluminum  pad, gold-wirebonded integrated circuits (ICs) at service  temperatures above 150˚C caused the formation of a brittle  AuAl2 IMC. Its purple appearance in optical microscopy gives  us the term still used for this phenomenon – "purple plague"


[2]. More recently, the use of "lead-free" solders has resulted  in reliability concerns with soldered joints [3, 4], prompting  investigation into which tin-based phases form in the highertemperature reflow conditions required for these higher  melting point solders.


Table 1: Examples of Intermetallic Phases


Time Domain Reflectometry: Case Studies in Electrical Failure Isolation


Jason Wheeler, Stephen Fasolino


Raytheon Space and Airborne Systems, McKinney, Texas U.S.A


Component Engineering Department - Failure Analysis Lab


Time Domain Reflectometry (TDR) is an analysis technique for  characterizing a transmission environment (PCB traces, cable  assemblies, etc.) and identifying the physical location of defects  or impedance discontinuities which can quickly narrow the focus  of an investigation.  This paper introduces the capability and  presents several case studies spanning different applications  where TDR was useful as a non-destructive analysis technique.


In the evolving electronics industry, signal integrity is an  essential aspect of every successful design.  As such, there are  many different tools available to an engineer to assist in  characterizing the electrical performance of a system.  Often, expensive Vector Network Analyzers (VNAs) are useful in  evaluating network parameters (most commonly Sparameters) over frequency; however, these systems fall short  in their ability to isolate and further characterize a failure.


In contrast, Time Domain Reflectometry (TDR) is a powerful  tool for characterizing a transmission environment (printed  circuit board (PCB) traces, cable assemblies, connectors, etc.) and identifying the physical location of defects or impedance  discontinuities; this can facilitate a more thorough  investigation using other analysis techniques.  The focus of  this article is to highlight this technology capability and  present case studies where TDR was useful as a nondestructive troubleshooting tool.


How it Works


TDR uses a sampling module to provide a fast edge step  response (with significant frequency content) to a unit under  test.  Voltage reflections occur at deviations from a standard  impedance (50Ω) and are displayed in the time domain with a  high-powered oscilloscope [1].  This information can be  processed using software that determines the differences in  characteristic impedance where these voltage reflections  occur.  Coupled with the dielectric constant of the material(s) involved, the physical location of these impedance aberrations  can be conclusively determined.


Case Study 1


Assembly Communication Issue


The Problem:  A CCA failed BIT test for video issues due to a  failure to establish communication (“hand-shaking”) between  two counterpart assemblies.  The issue was isolated to a small  subset of signals which could contribute to this condition.  Preliminary curve trace analysis revealed a low ohmic short (0.1Ω) between an FPGA’s enable signal and digital ground, which explained the observed failure mode.


Figure  1: SEM pictures of different samples showing voids of  different sizes and located at different positions (depth) in the  Cu-TSV. These samples were processed on purpose to study  the detection sensitivity of the investigated techniques.


The stress induced by TSVs in silicon can, if high, result in  local delamination of the vertical sidewalls. In addition, it will  affect the electrical properties of nearby transistors through the  piezoelectric effect of silicon. It is of high interest to industry  to determine the keep-out-zone, i.e. the zone around a TSV  where transistors are impacted by stress from the TSV. This  stress is most often studied by micro-Raman spectroscopy, sometimes combined with finite element models [2], and its


impact on transistors is investigated by electrical  measurements of drain current changes with distance from the  TSVs [3]. However, both experimental methods only give  local information. Raman spectroscopy can be used to make  maps of the stress field near a TSV, but this takes a long  measuring time and the sensitivity is at best about 10 MPa. There is need for a technique that can give this information  faster, covering a larger surface, and with a higher sensitivity. Polariscopy is a possible candidate for this purpose, with stress  sensitivity in Si in the kPa range. An additional advantage of  such a technique would be its use for failure analysis. Indeed, any defect that will affect the stress field near a TSV, such as  delamination or large voids, can possibly be detected with a  stress-sensitive technique. The aim of this paper is to explore  both techniques, GHz-SAM and IR polariscopy, for analysis of  TSVs.


Techniques: GHz-SAM


GHz-SAM is similar to a traditional SAM [4], but the  development of novel ultrasonic transducers has enabled the  fabrication of acoustic resonators reaching GHz frequencies. Extending the frequency to the GHz domain promises a higher  spatial resolution, but also a smaller penetration depth, making  it possible to detect issues in thinned wafers. In the system used  for the experiments discussed in this paper (PVA TePla  Analytical Systems GmbH), the transducer is mounted on a 3  axis scanning stage and, instead of immersing the sample fully  in water, as is traditionally done in SAM, only a drop of water  is used. A focused acoustic beam is generated by an acoustic  lens at 1GHz frequency. Fig. 2 shows a photograph of the setup.


Figure 2: Photograph of the GHz-SAM system


Techniques: SIREX


Polariscopy is based on the discovery of David Brewster [5] that when observing polarised light transmitted through a  stressed piece of glass, a color pattern is seen.  This resulted in  the ‘photoelastic stress measurement technique’ [6]. The  principle is based on the fact that stress makes a crystal such  as  Si optically anisotropic and thus birefringent. SIREX





G  2C 2


(Scanning Infrared Stress Explorer) is a so-called plane  polarimeter using linearly polarized laser light for probing. Due to the birefringence the beam splits of into two parts (ordinary and extraordinary) which are linearly and  perpendicularly polarized to each other and turned by the angle  between the initial polarization direction and that of the  ordinary beam. Furthermore, both parts are shifted by the


phase  to each other:


 =(2d/) C (xx -yy) =(2h/) C 


with d the thickness of the sample, xx and yy are the in-plane  principal stress components, and C is the photoelastic  constant of the material the light passes through.


The application of stress-induced birefringence for the  characterization of semiconductor materials and devices has  been the topic of many publications [7-10]. In particular, mono-crystalline silicon is a very good sample to study, because the unstressed crystal is nearly non-birefringent. This  means that, in principle, any stress in silicon wafers and  devices can be detected and visualized by photoelastic imaging  techniques. SIREX is a reflection-based polarimeter developed


Figure 3: Measurement principle of the SIREX system


by PVA (former JenaWave GmbH) [7]. Its principle is shown  in Fig. 3. The use of near-infrared laser diodes as scanning  probes allows a mapping with a lateral resolution of a few  microns. The sensitivity for stresses down to 1 kPa is nearly  unrivaled in comparison to other methods such as Raman  spectroscopy (~10 MPa sensitivity in Si).


SIREX provides two images: one of reflection given by R = (P + P‖)/P0 and one of depolarization given by the  depolarization D = 2P / (P + P‖). The R-image is helpful for  navigation and to separate non-birefringent-related effects. D  can be converted in the so called shear stress equivalent, G  which is given by:


4d 2sin


and which is directly related to the phase change  and thus the  shear stress .  For imaging  and n (optical anisotropy) a  procedure of variation of  and fit of sin(2), respectively, is  necessary which can be accomplished by measuring  independent G-maps. The results here presented were gained  from the backside (face-down configuration).


Results


GHz SAM


It was shown in [1] that GHz SAM is able to detect voids in  TSVs. After removing the Cu overburden on these samples, new GHz-SAM images were made. The images revealed a  fringe pattern near the TSVs. A typical example of such a  pattern observed in a normal TSV (no delamination or voids) is shown in Fig. 4, left. The GHz-SAM image of a TSV where


on purpose ‘delamination’ is made, by a FIB cut around the


TSV, is also shown in Fig. 4 (right).


Figure 4: GHz-SAM image of a normal (left) and ‘defective’ (right) TSV. The TSV diameter is 5 m, the depth 50 m. The ‘defective’ TSV was fabricated by making a circular FIB cut (few microns deep) around the TSV, mimicking delamination.


The fringes are much more pronounced in this image. This  indicates that they might be used to detect vertical  delamination. To further investigate this fringe effect, TSVs  with a smaller diameter (3 m) and even empty TSVs were  investigated. All show fringes in the image (Fig. 5, left and  right). A line cut using the FIB was also detected as a fringe  pattern (Fig. 6). The vertical cut width is around 1µm while the  horizontal cut width is under 500nm. These images show that  fringes in GHz-SAM have the potential to be used in detecting  fine cracks and delamination.


Figure 5: GHz-SAM images of a TSV with 3 m diameter (left), of empty TSVs (no Cu) with 5 m diameter (centre) and of a  TSV and a FIB cut (right).


The origin of the fringes lies in Rayleigh waves [11]. The  aperture of the GHz-SAM acoustic lens is such that not only  bulk waves, but also Rayleigh surface waves are generated in  the Si, as shown in Fig. 7. Fig. 8 shows the fringe intensity in  function of distance from the TSV, measured along a line  crossing the TSV. The distance between the minima is about  half the Rayleigh wavelength in Si. This is caused by reflection


of the Rayleigh waves, generated by the acoustic lens at the Si  surface, from the TSV edges. Interaction with the incident  waves results in a standing wave, and thus the observed fringe  pattern, with half the Rayleigh wavelength.


One can notice that the distance between the fringes seems to  increase further away from the TSV. A possible cause is stress  induced by the TSV in the Si. In order to study this, first FIB  circular holes with different depths (~ 2, 4, 6 and 8 m) were  cut beside a TSV to allow direct comparison between a hole  and a TSV filled with Cu and thus studying the effect of stress  on fringe behaviour. Fig. 9 shows that the fringes near the holes  are very regular and more pronounced than the ones from the  TSV. The intensities of the fringes from one hole (~2 m deep) measured in a narrow 5o region (see wedge in Fig. 10 left) are  plotted in Fig. 10, right. The bold line shows the average of the  region. The distance between the fringes is irregular. This  experiment does not confirm the stress effect. However, the  results are highly impacted by vibration induced noise, resulting in an irregular image making it difficult to measure  the exact distance between the fringes.


Figure 6: GHz-SAM image a cross-like FIB cut where the  near horizontal cut is 500nm wide and the vertical one 1000  nm; and (inset) corresponding SEM image.


Figure 7: Schematic drawing explaining the origin of  Rayleigh waves in GHz-SAM images.


Figure 8: Intensity of the fringes observed in a GHz-SAM  image (in-set) of a TSV. The intensity was calculated along  the white line shown in the in-set image. The distance between  minima is indicated. The wavelength corresponds to the  Rayleigh wavelength in Si.


Figure 9: SEM image of a TSV surrounded by 4 FIB circular  cuts with different depths (left). The corresponding GHz-SAM  image showing fringes beside the TSV and the empty FIB cuts (right).


Figure 10: Left: Zoom-in on the left FIB cut hole from Fig. 9  and definition of the area (wedge) where the intensity of the  fringe image is measured. Right: Fringe intensity in function  of distance from TSV, measured along different radial lines  inside the wedge defined in the left image, and mean value (bold line).


In another experiment, Fig. 11, the fringes near a TSV  containing Cu are compared in detail to the ones near an empty  TSV with same dimensions (but different sample). The fringe  distance seems different, which is confirmed by the intensity  analysis shown in Fig. 11 right. The distance between fringes  from the empty TSV is clearly larger and closer to the one


expected for stress-free Si (half the Rayleigh wavelength). For  this reason, this difference could be a stress effect. However,  system optimization (noise reduction) is required to further  investigate this effect.  In addition, the fringes are not entirely  circular, which could be related to the anisotropy of the  mechanical properties of Si. Additional research is required to  further investigate this.


Figure 11: Fringes near an Cu-TSV (left top) and an empty  TSV (left-bottom) and measured fringe intensity (right) from  the triangular region indicated in the left pictures.


The fringes near TSVs with many voids are clearly different  than the ones near good TSVs, as is for example shown in Fig.


12. While the good sample shows uniform fringe patterns, the  defective samples show varying and distorted images and  intensity patterns, a clear sign for defects. This confirms that  GHz-SAM indeed can be used to detect defective TSVs. The  exact sensitivity and resolution of the technique still has to be  investigated.


Figure 12: GHz-SAM images of good TSVs (left) and TSVs  with many voids (right).


SIREX


Because polariscopy is so sensitive to stress, we investigated  its possible application to detect stress fields near TSVs [12]. The technique proved to be very sensitive. Fig. 13 shows a  depolarization contrast map (G@ 0o) of part of a fully  processed chip (i.e. containing transistors (FETs) and TSVs). The colors indicate local shear stress fields. A zoom-in on a  stress field measured around a 6x6 array of 5 m diameter/50 m depth Cu-TSVs, located on this chip (see square marking  this place, Fig. 13, left) is shown in Fig. 13, bottom right. Also  shown (top right image) is a map of the (shear) stress field near


a group of 5 TSVs which location on the chip is indicated by  the small square in Fig. 13, left. The overlapping stresses  clearly generate a larger stress field, i.e. a larger keep-out-zone. This demonstrates the unique stress mapping properties of this  technique.


Figure 13: Left: SIREX map of the shear stress equivalent of  part of a chip with two regions indicated by squares. Right, bottom: Zoom-in on the left region, an array of 5 m  diameter, 50 m depth Cu-TSVs. Right, top: Zoom-in on a  group of 5 TSVs (configuration as in Fig. 16, left).


Figure 14: Left and right: SIREX map indicating the shear  stress equivalent caused by TSVs in Si samples. Left for a  sample with normal TSVs (D22), right for a sample with  empty TSVs (D23). The layout of the regions inside the  rectangular on the maps is shown at the bottom. It contains  fields without (0), with 1 or with an array (6x6) TSVs (A). TSV  diameter is 5 m, depth is 50 m.


To ensure that the SIREX maps are indeed related to stress in  Si caused by the Cu-TSVs, a map of a sample containing CuTSVs (sample D22) was compared at the same position with a  map of a sample with empty TSVs (sample D23). The region  contained a module with blocks of FET-arrays, some of which  were without TSV, some with one, and some with an array of


3x3 TSVs. The results are shown in Fig. 14. In the sample with  Cu-filled TSVs, the typical butterfly pattern, caused by the  stresses around the TSV, is very clear near the blocks  containing an array of TSVs, and it is also present in the blocks  with one TSV. It is not visible in the sample with empty TSVs.


The stress at the positions with only one TSV, was also  investigated using micro-Raman spectroscopy for a sample  before TSV opening (D24), after TSV etching (D23), and after  Cu filling (D22). The probing laser was 633 nm. The shift of  the Si Raman peak frequency from the stress free value (), measured along a line crossing the TSV on the three samples, is shown in Fig. 15 together with optical images of the position  where the measurement is done (small red line crossing the  center). At the position of the TSV (sample D22 and D23) no  Raman signal is obtained. The results clearly show that only  the TSV filling step introduces large stresses in the Si. The  sample with Cu in the TSV shows a large change of near  the TSV, indicating mechanical stress only in that sample. A  TSV typically induces tensile radial stress in the Si, and  compressive circumferential and axial stress. The measured  Raman frequency shift is positive, because the compressive  axial stress component dominates the Raman spectroscopy  results [13]. The SIREX results show the TSVs as tensile stress  monopoles, indicating that this technique is more sensitive to  the tensile radial stress which is also the main component  affecting nearby transistors [3].


Figure 15: Top: Raman frequency shift from the stress free  value () measured along a line across the position (cfr  optical images at the bottom) where a TSV will be processed (before etching, bottom left, D24), across a TSV etched hole (bottom center, D23) and across a TSV filled with Cu (bottom  right, D22). TSV diameter is 5 m, depth is 50 m.


These SIREX and Raman spectroscopy measurement results  confirm that the SIREX technique, in fact, does detect stress  and should thus be sensitive to anything affecting this stress, such as large voids in the TSVs, or delamination between the  TSV and the silicon.


To verify this statement, in a next experiment, a sample with  good TSVs (no voids) was compared with a sample with voids (2nd sample from the left in Fig. 1). Both samples have 10 m  diameter TSVs with a depth of 100 m. The reflection, G@0o  and n images obtained on an array of groups of 5 TSVs  obtained on the sample without voids are shown in Fig. 16. The  images around all TSV-groups are very similar, showing no  indication of failure. Measurement results taken on a similar  array of groups of 5-TSVs on the sample with voids are shown  in Fig. 17. Here only the n results are shown, obtained at 3  different positions on the array (called matrix 1, 2 and 3). In  each of the three locations deviating groups can be seen, showing more yellow and red colors, indicating a different  stress field.


Figure 16: SIREX results from a control sample (no voids), measured on an array of groups of 5 TSVs (see drawing at the  left). TSV diameter is 10 m, depth is 100 m.


Figure 17: SIREX results from a sample with large voids in  some TSVs near the top (2nd sample from left in Fig. 1), measured on an array of groups of 5 TSVs (see drawing at the  left of Fig. 16). TSV diameter is 10 m, depth is 100 m.


To quantify the results, first the stress difference  obtained  from these measurements at a line scan through the TSVs  indicated by circles on the images of Fig. 16 and 17 is plotted  in Fig. 18. The result from Fig. 16 (reference) is compared with  line scans across some images from the defective TSVs of  matrix 2 of Fig. 17. The numbering of the TSV-groups is done  by counting from top-left to bottom-right. At the position of  the TSVs, the signal is noisy because the reflection of the  probing beam from the TSV bottom (face-down configuration) is irregular. In Fig. 17, matrix 2, one can clearly observe two  deviating TSVs (more red and yellow colors), i.e. numbers 2  and 9. In Fig. 18 these TSVs also deviate from the others and  from the reference, showing higher strain in the Si close to the  TSV. Notice the kPa stress sensitivity.


Figure 18: Comparison of the stress  calculated along a line  crossing the TSVs indicated by circles in Fig. 16 (reference) and Fig. 17 (nr. 2, 9, 10 and 12 from matrix 2).


Fig. 19 shows an histogram of the calculated  stress in the full  matrix image, i.e. not taking a line scan at some places but  counting all data. This shows that the defective sample clearly  deviates from the reference, void free sample. More places  with higher stress are revealed and also at low stresses the  histograms clearly differ. Although further verification is  required, for example by doing FIB-cuts at the positions  indicated by the circles in Fig. 16 and 17, the results are very  promising. They indicate that Scanning Infrared Polaroscopy  could be used not only to detect deviations in complete regions (histogram) but even to pinpoint the deviating TSVs. This  technique shows promises both as stress measurement  technique and as failure analysis and process control  technique.


Figure 19: Comparison of the histogram of stress  calculated in the matrices shown in Fig. 16 (reference sample) and 17 (defective sample).


Two new techniques to study stress and defects near TSVs are  presented: GHz-SAM and SIREX. It is shown that both are  very promising for failure analysis in 3D technology.


It is shown that GHz-SAM can image standing Rayleigh waves  in the Si surface, caused by reflection at boundaries. We  investigated for the first time whether these fringes can be used  for failure- and stress analysis near TSVs.  The results indicate  that this might be possible, but further improvement of the  technique (noise reduction) and additional research is required. It is demonstrated that GHz-SAM allows detection of  discontinuities in the Si surface (TSV edge, FIB cut, crack), at  least for 500nm wide cracks, and confirmed that it can detect  differences between TSVs with and without voids.


It is demonstrated that polariscopy can detect shear stress fields  near TSVs and TSV-arrays, with an extreme sensitivity of 10  kPa. First results indicate that the technique can detect TSV  failures (voids) affecting this stress: SIREX shows clear  differences between good samples and defective samples.


Both techniques require further research to understand their  sensitivity and limitations. The techniques are also promising  for other domains where failure analysis is required, for  example chip-package-induced (CPI) induced problems (delamination, cracks) in the back-end-of-line.


The authors would like to thank the imec partners of the  Industrial Affiliation Programs on 3D integration and the  imec 3D team.


[1]  Phommahaxay, A., De Wolf, I., Hoffrogge, P., Brand, S., Czurratis, P., Philipsen, H., Civale, Y., Vandersmissen, K., Halder, S., Beyer, G., Swinnen, B., Miller, A., Beyne, E. “High frequency scanning acoustic microscopy applied  to 3D integrated process: Void detection in Through  Silicon Vias,” Proc. Electronic Components and  Technology Conference (ECTC) 2013, pp. 227-231.


[2] De Wolf, I., Simons, V., Cherman, V., Labie, R., Vandevelde, B. and Beyne, E., “In-depth Raman  spectroscopy analysis of various parameters affecting the  mechanical stress near the surface and bulk of Cu-TSVs,” Proc. Electronic Components and Technology Conference (ECTC), 2012, pp. 331-337.


[3] Guo, W., Van der Plas, G., Ivankovic, A., Eneman, G., Cherman, V., De Wachter, B., Mercha, A., Gonzalez, M., Civale, Y., Redolfi, A., Buisson, T., Jourdan, A., Vandevelde, B., Rebibis, K.J., De Wolf, I., La Manna, A., Beyer, G., Beyne, E. and Swinnen, B. ,”3D chip package  interaction thermo-mechanical challenges: Proximity  effects of Through Silicon vias and μ-bumps,” Proc. IEEE  IC Design & Technology conference (ICICDT), 2012, pp.


1-4.


[4] Brand, S., Petzold, M., Czurratis, P., Reed, J.D., Lueck, M., Gregory, C., Huffman, A., Lennon, J.M., Temple, D.S.,  Acoustic inspection of high-density-interconnects for 3Dintegration Proc. IEEE Ultrasonics Symposium (IUS), 2011, pp. 1076-1079.


[5] Brewster, D., “On the effects of simple pressure in  producing that species of crystallization which forms two  oppositely polarized images and exhibits the  complementary colurs by polarized light”,  Phil. Trans. A. (London) (1815), Vol. 105, pp. 60-64.


[6] Timoshenko, S. and Goodier, J. N., Theory of elasticity. United Engineering Trusties, Inc, (McGraw-Hill Book  Campany, 1951), pp. 131-145.


[7] Geiler, H. D., Karge H., Wagner M., Eichler St., Jurisch  M., Kretzer U. and Scheffer-Czygan M. “Photoelastic  characterization of residual stress in GaAs wafers. Materials Science in Semiconductor Processing (2006), Vol. 9, pp. 345-350.


[8] Lederhandler, S. R., “Infrared studied of birefringence in  silicon,” J. Appl. Phys. Vol. 30 (1959), pp. 1631.


[9] DeNicola, R.O. and Tauber, R. N., “Effect of growth  parameters on the residual stress and dislocation density  of Czochralski-grown silicon crystals,” J. Appl. Phys. Vol. 42, No. 11 (1971), pp. 4262-4270.


[10]Yamada, M., “High-sensitivity computer-controlled  infrared polariscope,” Rev. Sci. Instrum. Vol. 64, (1993), pp. 1815-1821.


[11] Briggs, A., Kolosov, O., Acoustic Microscopy (Oxford  University Press, 2010).


[12] Herms, M., Wagner, M., Lin, P., De Wolf, I. and Zhao, M., “Materials characterization and device analysis for  evaluation of semiconductor processes by highlysophisticated photoelastic stress measurement technique” Physica Status Solidi C (2015) doi: 10.1002/pssc.


201400356.


[13] De Wolf, I. “Relation between Raman frequency and  triaxial stress in Si for surface and cross-section  experiments in microelectronics components,” J. Appl. Phys. Vol. 118, 053101(2015) doi: 10.1063/1.4927133


Fast Feature Based Non-Destructive Fault Isolation in 3D IC Packages Utilizing Virtual Known Good Device


K.C. Lee∗, J. Alton, M. Igarashi


TeraView Limited, Cambridge, CB4 0DS, United Kingdom


∗Email: kc@teraview.com


S. Barbeau


IBM Systems, Bromont, QC, Canada


We combine Electro Optical Terahertz Pulse Reﬂectometry (EOTPR), with full three dimensional device-under-test(DUT) modeling utilizing virtual known good device to quickly and non-destructively isolate faults in advanced 3D IC packages. Computation power required for modeling can quickly become prohibitive with the design complexities of modern IC packages. In this study we adopt a piecemeal modeling approach that bypasses this exponential requirement. A PFA study veriﬁes the accuracy of our model. This shows that feature-based fault analysis with a distance-to-defect accuracy of less than 10 µm can be readily attained through the combination of these techniques.


Three dimensional IC package designs have become ubiquitous in recent years due to their abilities to incorporate ever more logical circuits within the same footprint as their traditional, two dimensional counterparts. However, the step up in circuit complexity poses new challenges for the failure analysis community. Traditionally, Time Domain Reﬂectometry(TDR) measurements offer a convenient means of defect prelocalization. In a typical TDR workﬂow, measurement from a failed device is compared to a reference Known Good Device (KGD), where the fault location is deduced from the timing information embedded in these measurements. The scale up in circuit complexity has increased the difﬁculties in producing golden KGDs for the comparative study, as well as the difﬁculty in interpreting the measurement results based on time-based information alone.


Electro Optical Terahertz Pulse Reﬂectometry (EOTPR) is an implementation of the TDR technique at terahertz frequencies, proven to improve fault isolation accuracy to less than 10 µm [1, 2, 3, 4]. This is achieved through a step reduction in measurement jitter noise and increase in temporal resolution [1]. During operation, electrical pulses are launched into the device-under-test (DUT) via a high frequency circuit probe. Reﬂections from device structures and faults are recorded as a voltage-time waveform by a fast photoconductive switch (PCS).


Figure 1: Model of the 3D package consisting of a substrate and (inset) an interposer structure.


In a recent study [5], a commercial 3D electromagnetic simulation software was used to generate a Virtual Known Good Device (VKGD). Simulation of the EOTPR measurement process then resulted in a reference waveform that was virtually identical to one measured from a physical KGD. By monitoring the real time pulse propagation in the simulation, the authors were able to correlate waveform features with key structures in DUT. Combining the spatial information gained from the simulation with highly accurate EOTPR measurements,feature based fault isolation with an accuracy level of less than 10 µm can readily be achieved [5, 6] in modern package substrates. Here, we extend this fault isolation technique on a complex 3D package (Fig. 1) consisting of a substrate and die,where the physical dimensions traces in the constituents vary by more than an order of magnitude.


An EOTPR system comprises two PCSs, one functioning as an electrical pulse source and the other as an instantaneous current detector activated by a mode-locked near infrared laser.


The emitted pulse is coupled into the DUT through a co-axial cable and a high frequency probe, while the reﬂected pulse is directed into the PCS detector. A translation stage in the detector beam path sweeps the relative delay between the emission and detection timings (Fig. 2), generating a continuous


Figure 2: (a) Schematic of an EOTPR system; (b) Typical raw EOTPR waveform from the open end of a high frequency probe.


voltage-time waveform for the user (Fig. 2b shows an example waveform from an open probe).


To enable meaningful comparison with a model generated reference waveform, we deconvolve the system response from the measured waveform by applying a post-processing procedure as in [5].


Model


To capture accurately the electromagnetic (EM) response of the DUT, we use a commercially available EM simulation tool which employs the ﬁnite difference time domain (FDTD)method [7] to calculate the transient EM behaviors through Maxwell’s equations. This approach bypasses the need for phenomenological quantities such as capacitance and inductance, and all inter-conductor couplings behaviors arise naturally as a result.


Fig. 1 displays a section of a model of a 3D package generated directly from the DUT design ﬁle. This particular package is a state-of-art design that is currently being developed. The trace shown in Fig. 1 consists of a ball grid array (BGA) connected to a via column on the substrate side. The signal path continues into the interposer structure through a C4 bump, where a through silicon via (TSV) connects to a top level trace that is terminated by an open pad for a microbump. Substrate side traces in this design are 60 µm wide, contrasting with the 3 µm wide traces in the interposer.


The modeling process consists of two iterations in this instance: a VKGD for the bare substrate is ﬁrst created using the procedures given in [5]; this is followed by creating a VKGD for the entire package, using values derived from the bare substrate model. To run the second model accurately and within reasonable time, the substrate and die are simulated separately.


Fig. 1 inset shows the split plane where the propagating pulse is extracted from the substrate side model and inserted into the equivalent point of the interposer model.


The importance of this failure mechanism has, for many years, generated significant interest in tools that can elementally  characterize them. The tools of choice have traditionally been  energy-dispersive x-ray (EDX) and wavelength-dispersive xray (WDX) spectroscopy in the scanning electron microscope (SEM) and transmission electron microscope (TEM). More  recently, electron energy loss spectroscopy (EELS) has also  become popular in TEM instruments. TEM and its associated  elemental analysis tools are particularly popular because TEM  inspection can also provide crystallographic data that provides  a second confirming data point for phase analysis – especially  important when small analytical volumes make spectral  analysis problematic.


The single greatest drawback for TEM analysis is not  technical, but financial. TEM instruments are not available in  many failure analysis (FA) laboratories due to the capital  outlay required both for the instrument and for the trained  operator/analyst such an instrument requires, not to mention  the focused ion beam (FIB) work required to create a TEMready sample lamella. Using outside laboratories for these  services is often more cost-effective, but not inexpensive; moreover, these expenses can grow significantly when  business conditions require rapid turnaround times on the  System


Aluminum


-Copper


-Gold


SilverTin


Copper-Tin


Abbrev. Al-Cu


||Al (κ) |Al |Ag |Cu (α) |
|---|---|---|---|---|

|(Symbol) |Al2Cu (θ) |Al2Au |Ag3Sn (ε) |Cu3Sn (ε) |

||AlCu (η) |AlAu |Sn (β) |Cu6Sn5 (η) |

||Al4Cu9 (γ) |βAlAu2 ||Sn (βSn) |

||Cu (α) |Al2Au5 ||Sn (αSn) |

|||AlAu4 |||

|||Au |||

Al-Au


Ag-Sn


Cu-Sn


Phase


analyses, over which the customer has less than complete  control.


On the other hand, most FA laboratories do have both SEM  and EDX tools that can support at least some level of IMC  characterization. The greatest drawback for these tools is their  limited resolution. The electron beam penetration depth and  the associated interactive volume of the SEM probe can result


do s


in probe spaces on the order of microns, as shown in Fig. 1


[5]. This does not compare well with a TEM lamella often a  tenth of a micron in thickness, giving the TEM yet another  edge over the SEM.


Figure 1: Diagram of typical excited volume in a sample  under SEM inspection. Depth approximation was added by  this author; approximation is typical for metals at a beam  energy of 15 kilovolts (kV).


The question then becomes whether there are any techniques  available that would make SEM/EDX analysis more  competitive with TEM analysis of IMC structures.


One possibility uses the rastering nature of the SEM electron  beam to take a series of spectral "snapshots" of how fast x-rays  of a given energy are being detected (in counts per second, or  CPS) at a particular spot. These "snapshots" are then  assembled graphically into a line matching the raster pattern of  the electron beam. When the x-ray energies are matched with  an element known to generate them, then these graphs can  show whether or not an element is present and, if so, then how  much the concentration of that element is changing with  respect to various points on the rastering beam from which  they were obtained. An analysis like this is referred to as an  EDX line scan.


Figure 2 shows a diagram of what happens during such a line  scan. At each point interrogated by the software, the rate at  which counts are received for a given x-ray energy is recorded, if that energy is assigned to an element of interest. In this  example, only five samplings are shown, though the samplings  in a given line typically number in the thousands. The more


that a given element is present, the higher will be the rate that  counts are received for it, and vice versa.


Distance


Tin


51


Nickel


Sample


e beam


backscattered


electronseelectrons X-rays


~1to 2μm


secondary


Surface


Direction of scan


Nickel Nickel1u


Figure 2: Schematic diagram of line scan process. As the  excited volume progresses to the right, progressively greater  volumes of tin are included, followed by decreasing volumes. These translate to increasing, then decreasing count rates for  tin. The opposite happens for nickel detection in the sample.


An example of a line scan obtained for two relatively pure  metal films is shown in Fig. 3. The copper and tungsten films  in the scan show a distinct location in the scan that matches  their locations as observed in the matching SEM image. Typically the SEM and line scan data are saved and presented  together to correlate the location of particular observed  structures to their relevant elemental data. Because the excited  volumes pick up elements of interest before they have fully  entered a film and before they completely leave, the interface  between films is nominally assigned at the point where two  elemental lines cross, also called the "crossover" point.


One encouraging characteristic of line scanning is also shown  in this figure. The copper and tungsten films analyzed are both  close to 100 nanometers in thickness. This line scan had no  difficulty resolving these films against each other and the  thicker bulk metallizations, suggesting that this technique can  have practical use in evaluating sub-micron pure metal films.


lvIB auauqs


120


Al Kal


90


Ni Kal


a60


Cula1 2 W Mal


30 0


µm


0.20.40.60.8


1.21.41.61.822.22.4


Figure 3: Line scan of tungsten (W) and copper (Cu) process layers separating bulk aluminum (Al) and nickel (Ni) die bump  metallization. The line traversed is shown by the horizontal line on the SEM image. Aluminum count rates are off this scale until the  raster begins to pass into the nickel layer. Crossover points and leftmost point of the tungsten layer are shown at vertical dashed lines.


The use of this technique for IMC films is not as  straightforward as it is for pure metal films. Binary IMC  systems (those composed of only two elements) by definition


Gold (Au)


will have unique atomic percentages in each intermetallic  phase, but these percentage changes will not cause the same  sharp line slope changes shown in Fig. 3. Instead, the element


Au4 Al


abundance will go from a nearly pure elemental phase to one  somewhat less pure, possibly followed by one or more  progressively less pure phases, and ending with a phase that is  dominated by the other element in the binary system. An  example of such a distribution for the aluminum-gold system is


Au5Al2


shown in Fig. 4 [6]. Elemental abundance due to phase  changes, therefore, is not marked by rapid changes in the line  scan of an element from near zero to a quick maximum, followed by an equally rapid drop. Instead, abundance changes  from phase to phase in binary systems are marked by often  subtle changes in slope of the trace for the two elements  involved.


Au2Ai


A representative example of this is shown in Fig. 5. This line  scan examines changes in elemental abundance for the tinsilver system. When using tin-silver-copper (SAC) solders in


AuAi


electronic assemblies, one phase that can form is the plate-like


Au Al2


Ag3Sn phase, an example of which is circled in the image. The  line scans for silver and tin are shallow compared to those in  Fig. 3, which would be nearly vertical at this scale. Because of  this, tracking phase changes in line scans involves noting


Aluminium (AI)


changes in slope of the lines of the elements of interest. This  complication is compensated in part by the fixed stoichiometry  of IMCs. The changes from phase to phase are abrupt, causing  the resultant lines to be straight (assuming the surface under  analysis is free of pitting or similar artifacts).


Figure 4: Diagram of the aluminum-gold binary IMC system. Five different IMC phases can be found in such a diffusion  couple, depending on the thermal history of the joint. Small  objects in the Au4Al-to-Au5A2 interface are Kirkendall voids.


All Elements


12D


Sn Lai


60 90


Ag Lal


µm 2021222324 252627 2829'3031323334 35


Figure 5: Line scan of one Ag3Sn intermetallic plate (circled in image). Only Sn and Ag traces are shown in legend for clarity. Ag  content steadily increases as its fraction of the excited volume increases, until the excited volume is completely within the particle (line is flat). As the excited volume passes the particle, the Ag content decreases to background levels. Note that the opposite is true  for the Sn line trace.


Experimental Procedure


Two IMC systems were selected for this study. The first is the  copper-tin system and the second is the aluminum-gold system. For the first, a lead-free solder joint to a copper pad was crosssectioned; for the second, a set of gold wire ball bonds thermosonically bonded to aluminum pads on an integrated circuit die  were cross sectioned. The parts were inspected using a JEOL  6700f SEM equipped with an Oxford X-Max 50 EDX  detector, supported by Oxford AZtec EDX analysis software. All analyses were conducted at 15 KeV at a working distance  of 15 millimeters. The SEM stage was not tilted during any  acquisition. Areas that appear in the Results section appear in  Fig. 6 and Fig. 7.


Figure 6: Lead-free solder at a copper pad on a printed  circuit board. Boxed region indicates portion of line scan  appearing in the Results section.


Figure 7: Gold wire ball bond at an aluminum pad on an  integrated circuit die. Boxed region indicates portion of line  scan appearing in the Results section.


An example of a line scan result for the copper-tin system is  shown in Fig. 8. The copper-tin IMCs traditionally found in  such joints include the "light" (as illuminated by the SEM) and  relatively abundant Cu6Sn5 phase adjacent to the bulk solder, and the darker Cu3Sn phase, usually a thin film that is  conformal to the bulk copper. The distinctive appearance of  the two phases contributed to their selection for this study, as  this would facilitate a quick "sanity check" of the line scan  findings against SEM observations. This example was the  clearest of the results in the copper-tin portion of this study; the other experimental results proved to be less conclusive  than this one. This suggests that line scanning, while feasible, does not produce results that are reliable enough to substitute  for TEM in this system.


Al| Elements


180


Sn La1 Cu La1_2


d120


345678910111213 14 15 16 17 18192021n


Figure 8: Example of line scan results for the copper-tin binary IMC system. Vertical dotted lines indicate the approximate location of  the Cu3Sn phase, approximately 500 nanometers thick. Inflection points in both the copper and tin traces appear at each dotted line, suggesting the slope of these two line segments represent the same phase (estimated by the leftmost dashed line at each trace). The  Cu6Sn5 phase to the right of the Cu3Sn phase is approximately three microns thick, thus it shows an altered slope (estimated by the  rightmost dashed line at each trace) for approximately 1.5 microns, followed by a flat trace as the excited volume completely  penetrates the phase. The final change in slope occurs as the excited volume crosses into the bulk tin solder, after which both traces  flatten as the excited volume passes completely into the solder.


1500


All Koil


Au Mal


Si Ka1 Cu Lai_2


00.20.40.60.8112141.61.8 22.2


Figure 9: Example of line scan results for the aluminum-gold binary IMC system. Vertical dotted lines indicate the approximate  location of the suspected AuAl2 phase, approximately 200 nanometers thick. Possible inflection points in both the aluminum and gold  traces appear at each dotted line, however, the absence of a sharp inflection renders this assessment questionable. This may be due in  part to the irregular appearance of the phase, which appears to have also contributed to a delayed aluminum-gold crossover. Irregularities in the prepared surface may also have contributed to observed inflection changes elsewhere on the two traces, making  any further conclusions about the phase distribution impossible.


Figure 9 (shown on the previous page) is a best-case result for  the aluminum-gold system – all other experimental results  were less conclusive than the one shown. At least three distinct  IMC phases were visible during SEM inspection. However, only one (the AuAl2 phase) gave any indication of trace  inflections consistent with the observed location of this dark  phase. This phase is particularly irregular and amorphous, causing more blending of the gold and aluminum signal than  would occur in a uniform film. Much of the difficulty here also  rests with the inherent difficulty of preparing gold IMCs  metallographically to a surface finish that will permit effective  line scan analysis at the magnifications required. While this  can be substantially mitigated with focused ion beam  polishing, this is not routinely available in all labs and, as with  the copper-tin system, is unlikely to be competitive with TEM  analysis.


The evidence in this study of line scan analyses of two IMC  systems suggests that, while sub-micron resolution may be  possible in certain cases, it cannot be counted on to reliably  produce phase identification in the absence of phase contrast  SEM data. TEM analysis appears to be a better option for  phase identification in most circumstances.


I thank Gwen Nail, Dave Susnitzky at Apple, and Tom  Schamp at Hitachi HTA for their help with editing.


[1] ASM Handbook, Vol 3: Alloy Phase Diagrams (Materials  Park, OH 1992.


[2] Philofsky, E., “Purple Plague Revisited”, Proc. 8th IEEE  Reliability Physics Symp., Las Vegas, NV, April 1970, p.


177.


[3] Angral, A., “Life Prediction in Leadfree Solder Joint and  PCB Metallization Under Shock and Vibration”, Auburn  University (Auburn, 2011), p. 99.


[4] Lead-Free Solder Joints” IVF Industrial Research and  Development Corporation (Mölndal, Sweden, 2006), p. 8.


[5] Vanderlinde, W., “Energy Dispersive X-Ray Analysis,” Microelectronics Failure Analysis Desk Reference, 5th ed., p. 632 (Materials Park, OH 2004).


[6] Jones, J. A., "Gold Aluminum Intermetallics - Current and  Future Considerations", Proc. 3rd ESA Electronic  Components Conf., Noordwijk, Netherlands, April, 1997, p. 411.


Quantitative SiGe TEM Elemental Analysis in FinFET Test Structures


James Demarest


IBM, Albany, NY USA   jjdemar@us.ibm.com


John Bruley


IBM, Yorktown Heights, NY USA


Quantitative elemental analysis by transmission electron  microscopy (TEM) has been a widely understood and studied  aspect of electron microscopy for many decades. Two of the  primary quantitative elemental analysis techniques are energy  dispersive X-ray spectroscopy (EDX) [1] and electron energy  loss spectroscopy (EELS) [1&2]. However, routine  application of these techniques can prove to be difficult as  they work ideally when internal references exist within the  sample being analyzed. As semiconductor device scaling  continues to reduce the structure size, device geometries are  also changing to three dimensional (3D) structures such as  finFETs, and the materials which compose the devices are also  evolving to obtain additional device performance gains. The  material change this paper studies is the introduction of silicon  germanium (SiGe) into the electrically active region of a  finFET test structure.


With the introduction of single crystalline SiGe into device  structures, it becomes necessary to monitor the atomic  concentration of Si and Ge to ensure the proper electrical  properties of the material are maintained throughout the  device fabrication process. X-ray diffraction (XRD) techniques are an excellent in-fab methodology to employ as  they are non destructive. However, XRD techniques have a  spatial resolution on the order of a millimeter with a chemical  sensitivity around 0.01 atomic percent (at%). A single fin in  cross section can occupy an area less than 25 by 100nm. This  small feature size makes TEM analytical techniques preferred  for nanoscale analysis as quantitative information can be  obtained with sub nanometer spatial resolution and a chemical  sensitivity on the order of a few at% with today’s state-of-theart TEMs.


There are two principal TEM analytical techniques used for  performing chemical analysis: EDX and EELS [1&2]. Briefly, EDX analysis examines the X-rays which are generated from  inelastically scattered incident electron-sample interactions. The incident electron interacts with an inner shell electron of  an atom within the sample and transmits energy to it, thus  promoting the electron to a higher energy state.  This leaves a  hole in the atomic electron configuration which is filled by a  higher energy electron.  The higher energy electron needs to


lose energy and does so by emitting an X-ray photon. These  photons are then detected and can be related back to where  they were generated on the sample.


Quantitative EDX, the main topic of this paper, utilizes the  Cliff-Lorimer equation which relates the ratio of the  concentrations (CA and CB) of two elements in a system to the  ratio of X-ray intensities of those elements (IA and IB) in the  spectrum times an instrument dependent sensitivity factor kAB or CA/CB=kAB IA/IB [1]. This equation is for a binary system  where CA + CB = 1.


EELS analysis is performed on inelastically scattered incident  electrons which have lost a characteristic energy when  interacting with an inner shell electron of an atom in the  sample [1&2].  The incident electron continues on through the  sample and is passed through a magnetic prism to obtain an  energy distribution. This allows characteristic elemental  energy information to be collected and related back to where it  was generated within the sample.


Experimental determination of kSiGe


Blanket SiGe wafers at three different Ge concentrations were  fabricated and characterized through XRD. The average Ge  concentration for the three wafers was 25.4, 50.25, and 84.14  at% Ge. A TEM sample was prepared from the 50at% Ge  sample by dual beam focused ion beam (DBFIB) with an  approximate thickness of 100nm following the process  described in [3]. Fifteen EDX spectra were obtained in a  200kV TEM across the blanket film. Three background  windows were defined for data processing (Figure 1). These  same microscope parameters and background windows were  used for all subsequent quantitative analysis. The spectrum  which was closest to representing the average value of the  fifteen uncalibrated data points was used to calculate the kSiGe factor for the instrument using the vendor software and the  known XRD concentration value.  kSiGe was determined to be


1.568 which is consistent with the range of potential values  found in the literature [1]. With kSiGe determined, quantitative  analysis was then applied to the entire data set and an average  value of 51.8 at% Ge was observed with a standard deviation  of 1.46.  This was found to be in good agreement with the  XRD data of 50.25 at% Ge. Additional samples from the two  other blanket films were prepared in an identical manner in the  DBFIB. Quantitative EDX analysis was applied to those films


as well using kSiGe of 1.568. The 25.4 at% Ge film was found  to be 25.5 at% Ge by TEM EDX with a standard deviation of


1.57 over 25 data points within the blanket film. The 84.1 at% Ge film was found to be 85.3 at% Ge with a standard  deviation of 1.58 over 50 data points taken within the blanket


*086 s6 dwel


film. These values are summarized in Table 1. Based upon


Ge 1 sec dwell●06.0.5 sec dwel


these results quantitative EDX by TEM was determined to be


28-


●Ge 3 sec dwel


accurate within two standard deviations or ±3 at% Ge.


26-


250


■EDX Spectrum profie


200-


22


150si


Ge


Courds


营


00


场


#0


Position (nril


Figure 1: EDX spectrum of SiGe blanket film showing  background window definition.


26


Table 1: Blanket Film Calibration Data


|Ge concentration |XRD at% |TEM at% |Standard Deviation |Number of Data Points |
|---|---|---|---|---|

|Low |25.4 |25.5 |1.57 |25 |

|Medium |50.3 |51.8 |1.46 |15 |

|High |84.1 |85.3 |1.58 |50 |

Variation of experimental parameters


With the demonstration of a consistent quantitative process, it  was of interest to explore changing some experimental  instrument acquisition parameters to determine if they have a  significant impact upon the analysis. The first of the  parameters which were studied was the effect of probe dwell  time at each analysis point in a uniform blanket film of about  25 at% Ge composition. The probe size of the instrument  which was used in this study was less than 1nm. As can be  seen in Figure 2, varying the dwell time from 0.5 to 6 seconds  has little to no impact upon the quantified composition. Lower  dwell times (0.5 and 1 second) trend with a slightly lower at% (~22.5 at%) while higher dwell times (3 and 6 seconds) trend  with slightly higher at% Ge (~26.5). The observed variation is  within the estimated error of the technique of ±3 at% Ge.


The effect of changing step size with a fixed dwell time was  also explored (Figure 3). In this experiment the dwell time was  set at 3 seconds—a typical acquisition time to ensure decent  spectra statistics—while the step size of each data point was  varied from 0.5-5nm. The data here shows a fairly consistent  average value for all step sizes of about 25 at% Ge, which is  the known value of the film. It should be pointed out that the  1nm step size data trended lower than the other conditions by  about 1 at% Ge. Over the typical dwell time and step size  parameters used for analyzing these structures the quantitative


results are consistent within the specified error of the  technique.


Figure 2: Effect of changing dwell time with 5nm step size.


●Oe £.5nm step


Oe Tnm stop


Energy (keV)


●Ge frm step●Ge2nm stop


Position (nri)


Figure 3: Effect of changing step size with 3 second dwell  time.


Early in the development process for a finFET program, an  electrical parameter was observed to be out of specification. One possible explanation for this shift in electrical behavior  was an increased Ge concentration beyond the expected value. Cross sectional BF TEM imaging demonstrated reasonably  good physical structure (Figure 4).  Figure 5 shows the same  sample in a high angle annular dark field (HAADF) image.  In  this imaging mode, irregularities on the upper fin surface can  be observed. Further, quantitative EDX elemental analysis was  performed vertically along the fin height and showed  significantly higher Ge concentration in the upper fin region  than was expected.  This difference was on the order of 10-15  arbitrary units (AU) (Figures 6 & 7). An independent  quantitative EELS analysis on a sister wafer which received  similar processing verified the EDX results (Figure 7). The  EELS analysis indicated a difference between the observed  and anticipated concentration of about 15-20 AU. These two  data sets were plotted together along with the expected  concentration in Figure 7. Given the sensitivity of the two  quantitative techniques, the fact they were performed on  different instrumentation, with different sample preparation  tools, and analyzed by different microscopists, they are in very  good agreement with each other and thus offer credence to the  results.


Figure 4: BF TEM image of finFET structure in fin cross  section


Figure 5: HAADF STEM image of finFET structure with fins  in cross section showing damage to the upper fin surface.


Figure 6: Quantitative EDX line scan location along fin  height.


Figure 7: Quantitative EDX, quantitative EELS, and expected  values as a function of position. The vertical axis is in  arbitrary units of concentration. The horizontal axis is in  arbitrary units of length. The left side of the plot is at the fin  top, while the right side of the plot is at the fin bottom.


In conclusion, a quantitative EDX TEM technique has been  demonstrated through the use of blanket film calibration  samples of known concentration characterized by XRD. The  accuracy of the EDX analysis is ±3 at% Ge (twice the  observed standard deviation of the data). The effect of  changing dwell time and step size were studied and showed  minimal impact (less than the error of the technique) on the  quantified data. The technique was used to identify a test  structure issue which could only be diagnosed with a  technique having nanometer spatial resolution and atomic  percent sensitivity.  Further the results of the test structure  analysis were independently verified by the complementary  TEM EELS technique. Based in part on these analyses, process actions were put in place to correct the observed  issues.


[1] Williams, D. B and C. B. Carter, Transmission Electron  Microscopy, Plenum Press (New York, 1996).


[2] Egerton, R. F. Electron Energy-Loss Spectroscopy in the  Electron Microscope, Plenum Press (New York, 1996).


[3] Demarest and DeSouza. “Start Up and Evolution of a FEI  DA 300 DBFIB for Automatic STEM Sample  Preparation,” Proc 33rd International Symposium for  Testing and Failure Analysis, San Jose, CA, November  2009, pp. 334-338.


Failure and Stress Analysis of Cu TSVs using GHzScanning Acoustic Microscopy and Scanning Infrared  Polariscopy


Ingrid De Wolf and Ahmad Khaled


Imec, Kapeldreef 75, B-3001 Leuven, Belgium   and Dept. Materials Engineering, KU Leuven, Belgium  ingrid.dewolf@imec.be


Martin Herms and Matthias Wagner


PVA Metrology & Plasma Solutions GmbH, Am Naßtal 6/8, D-07751 Jena-Maua, Germany


Tatjana Djuric and Peter Czurratis


PVA TePla Analytical Systems GmbH, Deutschordenstraße 38, D-73463, Westhausen, Germany


Sebastian Brand


Fraunhofer Institute for Mechanics of Materials IWM (CAM), Walter-Hülse-Straße 1 I 06120 Halle (Saale), Germany


This paper discusses the application of two different  techniques for failure analysis of Cu through-silicon vias (TSVs), used in 3D stacked-IC technology. The first  technique is GHz Scanning Acoustic Microscopy (GHzSAM), which not only allows detection of defects like voids, cracks and delamination, but also the visualization of Rayleigh  waves. GHz-SAM can provide information on voids, delamination and possibly stress near the TSVs. The second is  a reflection-based photoelastic technique (SIREX), which is  shown to be very sensitive to stress anisotropy in the Si near  TSVs and as such also to any defect affecting this stress, such  as delamination and large voids.


Through Si Vias (TSVs)


In order to enable a continuous improvement of the  performance of electronic systems, in addition to the classical  device scaling, 3D-system integration is under development. In this innovative and challenging technology, silicon dies are  thinned and stacked on top of each other. They are electrically  interconnected by Cu nails through the silicon (called through  silicon vias, TSVs) and micro-bumps. This technology brings  new failure mechanisms requiring new failure analysis  techniques. In this paper we focus on two detection problems  associated with the TSVs. One is the detection of voids and  delamination of the TSVs, a second one is the detection of the  stress field near the TSVs.


During processing, voids may be present in the TSVs (see for  example Fig. 1). These voids can be large or small, and located


near the top or bottom of the TSV. Industry is looking for  techniques to detect these voids as early as possible in the  processing sequence. The samples shown in Fig. 1 were made  on purpose with voids, to test various techniques. It was  demonstrated that GHz scanning acoustic microscopy (GHzSAM) is a possible candidate for this detection [1]. In this  paper, we will show that the technique offers additional  features that might be of interest for TSV failure analysis.


In a complex structure such as the one modeled in this study,signiﬁcant cross-coupling occur between the signal trace and its nearest neighboring line. The propagating pulse must therefore be recorded across both parallel traces as it crosses the model split boundary. For each portion of the model, ‘scattering’ S parameters were derived for coupling along the signal line, as well as cross-coupling into the adjacent neighboring lines. These are then combined during post-processing with the equivalent S parameters from the other model portion to generate the VKGD model waveform for the entire stacked package.


Fig. 3 shows the measured and simulated EOTPR waveforms for the signal trace in: (a) the bare substrate device, and (b) the full package; in (c) the red arrows denote the reﬂection mechanism responsible for producing the ﬁrst order, primary waveform features, annotated in red in (a), whereas the secondary


Figure 3: Comparison of simulated and measured EOTPR waveforms in the (a) bare substrate; (b) full package. The red and blue curves show the measured and simulated waveforms in both cases. The pale grey and green curves in (b) are the measured and simulated waveforms for a failed package.


Comparison of the waveform peaks against the brown dotted alignment lines in the two plots clearly indicate that the open fault in the package lies just after the C4 bump. (c) Illustrates the propagation paths of primary reﬂections (red) vs. an example of a secondary reﬂection (green).


Figure 4: SEM images showing the region around the TSV in:


(a) A good reference device; (b) the failed device showing the open fault failure at the top of the TSV; (c) close up of the same device around the open failure.


‘mid trace’ waveform feature in (a) (annotated in green) is produced by a secondary reﬂection mechanism shown in green in (c). In practise, only the primary reﬂection features are needed for fault isolation since, for instance, if an open fault were to exist in front of the mid trace feature, the secondary reﬂection path (green) illustrated in Fig. 3c would not occur,thereby suppressing the corresponding feature annotated in green in Fig. 3a. Good agreements are obtained between the measured (red curve) and simulated (blue curve) waveforms enabling key device design features to be identiﬁed. This is especially true for the primary waveform features, and the small deviations in the secondary waveform features in Fig. 3a represent differences between the modeled and manufactured samples, resulting from sample-to-sample variations, manufacturing tolerances etc. The close correspondence between the measured and simulated results in Fig. 3a signiﬁes that the substrate VKGD is correctly set up. Subsequent VKGD creation of the full package followed the procedures as in [5], with only the die side requiring further attention. Pulse propagation velocity between key device structures can be extracted from the simulation and used to locate faults in a measured device with a simple time-of-ﬂight calculation.


To verify the technique, we tested the simulation results against a failed device. The grey curve in Fig. 3b shows the measured EOTPR waveform from a failed package device.


This waveform clearly deviates from the reference device, with a notable peak at ∼ 125 ps, indicating an open fault at a sig-niﬁcant distance before the microbump. Calculations based on the pulse propagation velocity from the simulation suggests that the waveform peak is a reﬂection originating from just after the TSV within the interposer, around 5 mm into the DUT,from the BGA. A subsequent model with a virtual open circuit created at the suggested location is then simulated, producing the resulting green waveform in Fig. 3b. The good agreement with the grey waveform conﬁrms the accuracy of the simulation technique. Having established the open fault location relative to the TSV, the sample is subsequently subjected to a Physical Failure Analysis (PFA). During PFA, the DUT was mechanically grounded from the BGA plane upwards to the top substrate layer, with periodic manual probing of the DUT to conﬁrm the continual presence of the fault. The DUT is then cross-sectioned along the TSV, exposing the open fault for optical, and ﬁnally, SEM inspection (Fig. 4). This ﬁnal, high resolution image conﬁrmed the location of the open fault to indeed be at the top of the TSV, corroborating with the EOTPR modeling analysis. In general, the EOTPR tool is capable of revealing faults at 100+ mm into the sample.


In summary, we have shown that by combining EOTPR with three dimensional DUT modeling, it is possible to correlate key device design elements with EOTPR waveform features.


In addition, we have shown how DUT simulations can be used with EOTPR to identify faults in advanced IC packages without having a physical reference device.


[1] Y. Cai, Z. Wang, R. Dias, and D. Goyal, “Electro Optical Terahertz Pulse Reﬂectometry - An innovative fault isolation tool,”in Proceedings - Electronic Components and Technology Conference, Jun. 2010, pp. 1309–1315.


[2] M. Y. Tay, L. Cao, M. Venkata, L. Tran, W. Donna, W. Qiu, J. Alton, P. F. Taday, and M. Lin, “Advanced fault isolation technique using electro-optical terahertz pulse reﬂectometry,” in Physical and Failure Analysis of Integrated Circuits (IPFA), 2012 19th


IEEE International Symposium on the, Jul. 2012, pp. 1–5.


[3] L. Cao, M. Venkata, M. Y. Tay, W. Qiu, J. Alton, P. F. Taday, and M. Igarashi, “Advanced Fault Isolation Technique using Electro-optical Terahertz Pulse Reﬂectometry ( EOTPR ) for 2D and 2.5D Flip-chip Package,” in Proceedings of the 38th International Symposium for Testing and Failure Analysis (ISTFA),2012, pp. 21–25.


[4] S. Barbeau, J. Alton, and M. Igarashi, “Electro Optical Terahertz Pulse Reﬂectometry - a fast and highly accurate non-destructive fault isolation technique for 3D Flip Chip Packages,” in Proceedings of the 39th International Symposium for Testing and Failure


Analysis (ISTFA), 2013, p. 264.


[5] K. C. Lee, J. Alton, M. Igarashi, and S. Barbeau, “Feature Based Non-Destructive Fault Isolation in Advanced IC Packages,” in Proceedings of the 40th International Symposium for Testing and


Failure Analysis (ISTFA), 2014, p. 214.


[6] E. Kowalczuk, A. Bhattacharya, K. C. Lee, J. Alton, M. Igarashi,and S. Barbeau, “Fault Localisation of defects using Electro Optical Terahertz Pulse Reﬂectometry and 3D EM modelling with Virtual Known Good Device,” in Proceedings of the IEEE 3D System Integration Conference 2014, 2014.


[7] K. Yee, “Numerical solution of initial boundary value problems involving maxwell’s equations in isotropic media,” Antennas and Propagation, IEEE Transactions on, vol. 14, no. 3, pp. 302–307,May 1966.


Failure analysis strategies for multi-stacked memory devices with TSV  interconnects


Frank Altmann1, Christian Grosse1, Falk Naumann1, Jens Beyersdorfer1, Tony Veches2


1Fraunhofer Institute for Mechanics of Materials IWM,


Center for Applied Microstructure Diagnostics, 06120 Halle, Germany  2Micron Technology, Inc., Boise, USA


frank.altmann@iwmh.fraunhofer.de


In this paper we will demonstrate new approaches for failure  analysis of memory devices with multiple stacked dies and  TSV interconnects. Therefore, TSV specific failure modes are  studied on daisy chain test samples. Two analysis flows for  defect localization implementing Electron Beam Induced  Current (EBAC) imaging and Lock-in-Thermography (LIT) as  well as adapted Focused Ion Beam (FIB) preparation and  defect characterization by electron microscopy will be  discussed. The most challenging failure mode is an electrical  short at the TSV sidewall isolation with sub-micrometer  dimensions. It is shown that the leakage path to a certain TSV  within the stack can firstly be located by applying LIT to a  metallographic cross section and secondly pinpointing by  FIB/SEM cross-sectioning. In order to evaluate the potential  of non-destructive determination of the lateral defect position, as well as the defect depth from only one LIT measurement, 2D thermal simulations of TSV stacks with artificial leakages  are performed calculating the phase shift values per die level.


Today’s package developments including System in Package (SiP) approaches, Wafer Level Packaging, Chip Embedding  and 3D heterogeneous integration are continuously pushing  innovations for microelectronics. In the previous years, in  particular Through Silicon Via (TSV) technologies have been  attracting rapidly increasing attention for high density vertical  system integration approaches [1]. Recently, several new  DRAM memory architectures based on multi-stacked die and  TSV have been announced for mass production. But, many  challenges associated with cost, process integration and device  reliability still have to be solved. Failure analysis provides an  important basis for process step optimization in order to  achieve and secure high quality and manufacturing yield  during industrial manufacturing [2]. The main types of  interconnection failures are short circuits or opens. For 3D  packages with multilevel dies and interconnects only a few  analysis techniques exist that allow localizing electrical  defects.


In particular, scanning magnetic field imaging (MFI) methods   provide direct information about the spatial location of  interconnect failures by visualization of electrical current


paths based on a highly sensitive detection of the related local  magnetic field. First results of visualization of current paths  within stacked die devices with TSV interconnects have  already been demonstrated [3-4]. Alternative technique to  isolate electrical defects within the internal wiring is based on  time domain reflectometry (TDR) that provides failure  localization information from electrical “echo” signal data  which has already been shown for TSV defect localization [5-7]. Another promising candidate for electrical defect  localization is microscopic Lock-in Thermography (LIT). This  technique is suitable for localizing resistive opens and  electrical shorts within packaged devices by detecting and  imaging of related hot spots generated by the small amount of  electrical power they dissipate. Gaining depth information of  the hot spots is possible through a quantitative phase shift  analysis based on the time delay between electrical stimulation  and thermal response that is measured at the device surface [8-9]. A new multi harmonics analysis approach was currently  shown to further improve the phase shift analysis in terms of  frequency range and measuring time [10].


Last but not least, Electron Beam Absorbed Current Imaging  Technique (EBAC) based on scanning electron microscopy  can be applied in special cases for precise open and short  localization. One example on open TSV interconnects is  shown here [11].


In order to understand the root causes of faulty functional  behavior, high-resolution material analysis based on scanning  and transmission electron microscopy and other analysis  techniques is essential.  For site specific cross sectioning of  TSV and micro-bump interconnects, standard mechanical  cross sectioning techniques are often limited. As an  alternative, focused ion beam (FIB) systems with novel  inductive plasma sources can achieve suitable milling rates  and are very useful to get access to single defects [12].  For  device level preparation the milling process can further be  enhanced by combining precise short pulse laser ablation for  rough milling and combined Plasma-FIB for finishing [13].


In this paper we will demonstrate strategies for the localization  of electrical defects by EBAC, LIT and FIB/SEM defect  screening followed by Plasma-FIB cross sectioning and  Standard-FIB TEM lamella preparation for physical defect  analysis on Cu filled TSV stacks at Hybrid Memory Cubed (HMC) test structures.


Sample Description


Microns´ HMC package consists of a highly complex stack of  one controller die and up to 8 DRAM dies, integrated with  advanced circuit board technology, as shown in figure 1. Each  die is about 60 μm thick and thousands of Cu filled TSVs with <10 μm diameters, are inserted through each die and  connected together using Cu-Sn pillars. This allows extremely  high performance and low loss interconnect paths. The TSVs  are filled with Cu metallization with nm-scale diffusion  barriers. The TSV metallization is isolated by a thin silicon  oxide layer to the Si-substrate.


Figure 1: Mechanically cross section of the TSV test sample


For TSV process development and reliability testing specific  daisy chains are used with multiple connected TSVs over the  whole stack. So called “short chains” consist of 160 serially  connected TSVs over 4 stacks and are used to check for opens  within the TSV wiring, figure 2 left.


Figure 2: Schematic of the wiring of TSV test structures of “short chain” (left) and “open chain” (right)


“Open chains” are used to check for TSV shorts to the Si  substrate and shorts between pillars consisting of electrically  separated 5 stacked TSV columns which are tested to an  adjacent stacked TSV row.


A HMC test device contains multiple TSV daisy chains of all  together several thousand interconnect for electrical testing.


Failure Analysis of open TSVs


As a first example the localization and cross section analysis  of opens within the “short chain” are demonstrated. To get  access to the TSV structures from the top of the die stack the  lids of the HMC test devices were removed. The defective  daisy chain was contacted at the outer TSVs applying tungsten  needles by using a piezo driven nanoprober system within a  scanning electron microscope (SEM). Then EBAC imaging  was performed to locate the open within the daisy chain, figure 3.


Figure 3: Probing of the “short chain“ (left), EBAC imaging  of the TSV chain shows clearly defect position (right)


Knowing the exact defect position a local cross section of the  defective TSV stack was prepared by Plasma-FIB milling. As  a result one TSV with insufficient Cu filling was found which  caused the electrical open within the daisy chain, figure 4.


Figure 4: Overview of Plasma-FIB cross sectioning at the  defect position (left), detail of TSV open caused by insufficient  Cu filling (right)


Analysis strategy for TSV side wall shorts


TSV sidewall leakage defects typically scale with the  thickness of the isolation layer and therefore have dimensions  below 100 nm.  To understand the origin of such defects, physical root cause analysis by high resolution TEM is  required.  To be able to prepare an electron transparent sample  of such a defect, knowing its exact position within the three  dimensional TSV stack is essential. In the following section a  localization strategy including nanoprobing, LIT and  FIB/SEM screening is demonstrated on a 5 stack HMC test


logic  DRAM #2  DRAM #3


DRAM #1  DRAM #4


device with single TSVs shorted to Si-substrate. The die level  of the TSV short cannot be determined by electrical testing  here, thus 3D defect localization is crucial.


Nanoprobing and top view LIT


As a first step, a defective HMC test device was opened  removing the lid cover. Then, with optical access to the upper  TSVs of the device, the defective “open chain” test structure  was identified by comparison to the data map from electrical  testing. In order to detect single shorted TSVs each of the 12  TSV columns were probed and electrically measured to each  other to verify the defect positions from the data map. The  measurements were performed by SEM in-situ nanoprobing. As a result, electrical shorts were measured at two adjacent  shorted TSV columns with 6.4 MOhm resistance, figure 5.


Fig. 5:  Stepwise electrical characterization of adjacent TSV  columns to identify leakages, SEM insitu nanoprobing of TSVs (left) and U-V characteristics of leakaged TSVs


As a first trial to locate the position of the leakage at the  sidewall of the TSV column, top view LIT measurements  were performed. For this experiment, the upper Cu pad of the  TSVs was removed by chemical-mechanical polishing. TSV  columns should not be probed directly to avoid shadowing  caused by the relative large prober needles. Therefore, each  defective TSV column was contacted by Plasma-FIB  deposited Pt lines. Additional Pt pads were deposited to  simplify probing for the following LIT measurements.


Fig. 6:  LIT top view of shorted TSV columns probed by  Tungsten-needles, overlay of amplitude and topography image (left), phase image (right)


The TSV columns were electrically stimulated by 40 V and  90 μA which mean 3.6 mW dissipation power. Measurements  were done at different lock-in frequencies. Figure 6 shows the  amplitude and topography as well as the phase image result  after 1.5 hour at 0.5 Hz. It can be seen, that the signal to noise  is quite low and the heat is spread over several tens of microns  around the TSV column. A local hot spot indicating the defect  position was not found. The extreme low thermal signal and  large thermal spreading is caused by the Cu-filling and Si with  high thermal conductivity.


LIT at metallographic cross section


To exactly pinpoint the short within the TSV column an  alternative approach was used to apply LIT at metallographic  cross section. For this experiment, a site specific cross section  of the device was made by stepwise grinding and polishing. Optical navigation was possible by gluing the sample to a  glass plate, thus allowing visual inspection from the top site. The cross sectioning was stopped about 10 μm before the  defective TSV columns. Then, the FIB deposited Pt lines were  used to electrically stimulate the TSV columns for the  following LIT measurements.


Fig.7: Removed upper Cu-pad by CMP polishing (upper left), Plasma-FIB deposition of Pt lines and pads (upper right),  LIT


at un-coated mechanically cross section (lower left) and


located defect site at same cross section after black painting (lower right)


LIT measurement was done at 30 V and 80 μA (2.4 mW  dissipation power) applying a lock in frequency of 22.9 Hz in  order to minimize thermal spreading and achieve high lateral  resolution. The IR transparency of the Si substrate allows a  direct view to the Cu filling of the TSVs.


In a first LIT measurement for about nearly 1 hour, a thermal  signal was detected which unexpectedly was not at a Cu-TSV  but at the organic under-filler between the dies, figure 7 left. Because the thermal signal is located above and underneath  die #2 it was assumed, that the origin of the hot spot would be  situated at the TSV of die #2, but it could not be detected  because of the low emissivity of Cu and Si. Therefore, the  sample was locally covered by a thin layer of black paint to  maximize the emissivity. The second LIT measurement at  30 V with 40 μA leakage current showed the expected hot  spot at the Cu-TSV after 1 hour measuring time, figure 7 right.  The defect was located at the upper part of the TSV at  memory die 2#. It can be seen that the thermal signal is


DRAM #4


DRAM #2  DRAM #1


logic


DRAM #1  DRAM #2  DRAM #4


smeared in a relatively large area of several 10 μm due to the  thermal spreading within the Cu. Thus, the origin of the hot  spot could not be located more precisely than about ±10 μm.


SEM/FIB screening of the located defect area


As last step for defect localization, the area of the hot spot was  screened for any visible defects by combined FIB crosssectioning and SEM imaging. A first cross section of about  60 μm width and several 10 μm depth was made by PlasmaFIB at the center of TSV at memory die #2. From this  position, a continuous Ga-FIB and SEM observation of the  TSV structure was started. The milling was stopped  immediately when the defect appeared at the TSV side wall, figure 8.


Fig. 8: Continuous FIB / SEM screening of TSV at the hot spot  position (left), SEM detail of the found breakdown defect in  TSV isolation (right)


As a result, a defect < 1 μm in diameter could be found within  the TSV sidewall near the top of the TSV filling.


Physical failure analysis of the TSV sidewall defect


Because of the small dimension of the located defect at the  TSV sidewall isolation additional analysis by transmission  electron microscopy (TEM) and energy dispersive X-Ray  spectroscopy (EDS) was performed. For this an electron  transparent lamella was made from the defect site by FIB  milling from the opposite side to the defect. The TEM lamella  was cut out by FIB and then transferred by a piezo driven  micro gripper into a clamp holder, figure 9 [14].


Fig. 9: FIB-preparation of a TEM lamella (left), In-situ lift out  by microgripper (right)


TEM imaging and EDS mapping were done in a FEI TITAN  microscope equipped with high sensitive SuperX EDS  detector. As a result, Cu migration from the TSV filling into  the sidewall isolation could be analyzed, figure 10.


Fig.10:  TEM image of the TSV structure with sidewall defect (above), STEM image (lower left) and EDS maps (lower  middle and right) of the short defect at the TSV isolation, Cu  migration into the oxide could be proved


Evaluation of top view LIT for non-destructive  defect localization


In order to evaluate the sensitivity of the defect depth  localization of multi-stacked dies by LIT, Finite Element  Analysis of the lock-in process was performed and the  expected phase shift values were calculated. This is needed to  define a suitable frequency range for measurement, i.e. the  frequency where the separation of different dies is possible  and thermal damping of the Lock-in signal is reduced. Simple  1D calculation by the analytical solution is not expedient  because of the 3D structure of the TSV wiring.


Therefore, a 2D-axialsysmetric model of the multi stacked  device including one TSV structure was prepared. The  simulation was performed using ANSYS®15.0. During  transient solution of the model, a square wave shaped heat  flow (periodic to the lock-in frequency) is introduced into the  die by a point source at the FEA-model. During thermal  excitation the heat propagation to the model surface and with  that, the resulting phase shift is calculated [10]. Figure 11  shows the extrapolated 2D-model demonstrating the model  setup and considered memory dies. In addition to the transient  calculation, the local temperature distribution under steady  thermal conditions is exemplarily shown of an assumed defect  at the DRAM#1 stack. The thermal plot demonstrates the  reason for a poor signal-to-noise ratio during LITinvestigation, where the major heat flux into the Si-die occurs  and only a small amount of the heat for LIT-investigation  reaches the device surface. The estimated phase behavior of a  LIT-frequency of 5 Hz (dashed line) and 22.9 Hz (solid line) is shown in figure 12 for different defect depths at the stacked  memory device. The estimated phase shift at the defect  localization was set to zero for model calibration and


simplification of the heat source geometry. As a result, an  increase of the phase shift can be observed for larger distance  to the heat source depending on the used LIT-frequency, while  the highest gradient of the phase shift can be found at the Sn  layer of the TSV. The estimated phase difference to  distinguish defect locations between two adjacent dies can be  found in the range of 15° till 50° (for 5 and 22.9 Hz), depending on the actual defect depth and used LIT-frequency  as shown in figure 13.


Fig.11:  FEA-Model: left – extrapolated 2D-FEA model of the  multi-stacked memory devices with one TSV interconnect; right – temperature profile at the steady- state with a assumed  defect at the DRAM#1 stack


Fig.12:  FEA-Result of the calculated phase shift of different  defect depths at f=5 Hz (dashed lines) and f=22.9 Hz (solid  lines)


As a result of the FEA-simulation of the multi-stacked die, the  minimum frequency for defect localization can be estimated  and compared to the experimental restrictions from thermal  damping.


In the next step, the absolute values of the FEA-simulation  have to be compared with defined measurement of different  stacks by LIT measurements, which are currently not  concluded in the required extent.


Fig.13:  Estimated phase shift difference between two stacked  dies at f=5 Hz (light blue) and f=22.9 Hz (dark blue)


Conclusion and Outlook


Today’s trends in 3D integration and packaging lead to  distinct challenges for  the required failure analysis techniques  and work flows due to the high design complexity of multichips. As an example, electrical defects within stacked TSV  interconnects were investigated and adapted failure analysis  approaches for defect localization and site specific preparation  evaluated. It was shown that electrical opens within TSV daisy  chains can easily be located by top view EBAC imaging. Fast  cross sectioning by Plasma-FIB can be used to verify and  characterize those defects. For sub-μm sidewall defects, cross  sectional LIT combined with further FIB/SEM screening was  successful in pinpointing the defect within the TSV column. This procedure might be shortened in time by combined  Plasma-FIB cross sectioning and SEM observation screening  the whole TSV stack. The challenge here is to check all TSV  sidewalls at the column by high resolution SEM during  continuous or stepwise milling and to avoid any curtaining  especially at the TSV isolation. The problem will be mitigated  if the first top view LIT measurement could also provide the  defect depth localization by phase shift analysis. By thermal  simulation it was shown that thermal spreading is high and  therefore, the gained signal to noise ratio low. On the other  hand, each TSV level should clearly be distinguishable. But, further LIT measurements have to be done to verify the  thermal modeling.


The authors thank AUDI AG for financial support of this work  in particular Wolfgang Froehlich for many valuable  discussions.


P.S. Andry et al., “Fabrication and Characterization of  Robust Through-Silicon Vias for Silicon-Carrier  Applications,” IBM Journal of Research and  Development, Vol. 52, No. 6, (2008), pp. 571-581


F. Altmann et.al.: Characterization and failure analysis of  3D integrated semiconductor devices novel tools for fault  isolation, target preparation and high resolution material  analysis, Proceedings from the 36th International  Symposium for Testing and Failure Analysis November  14–18, 2010, Addison, Texas, USA


A. Orozco et. al.: “3D IC/Stacked device Fault Isolation  using 3D Magnetic Field Imaging” Proc. of the 40th  International Symposium for Testing and Failure Analysis (ISTFA), 2014 33-37


J. Gaudestad et. al.: “Failure Analysis Work Flow for  Electrical Shorts in Triple Stacked 3D TSV Daisy  Chains”, Proc. of the 40th International Symposium for  Testing and Failure Analysis (ISTFA), 2014 38-42


K. Matsumoto et. al: “Identification of Through Silicon  Via (TSV) Failure Points Using Time Domain  Reflectometry (TDR) Method”, Transactions of The  Japan Institute of Electronics Packaging  01/2013; 6(1) 57-62.


W. Qiu et. al.: “Non-destructive Open Fault Isolation in  Flip-Chip Devices with Space-domain Reflectometry”; Proc. of the 39th International Symposium for Testing  and Failure Analysis (ISTFA), 2013 1-6


K-C. Lee et.al. : “Feature Based Non-Destructive Fault  Isolation in Advanced IC Packages” Proc. of the 40th


International Symposium for Testing and Failure Analysis (ISTFA), 2014 214-217


R. Schlangen et al:  “Use of Lock-In Thermography for  Non-Destructive 3D Defect Localization on System in  Package and Stacked-Die Technology”, proceedings of  ISTFA 2011, p68-73


C. Schmidt, F. Altmann: “Quantitative Phase Shift  Analysis for 3D Defect Localization Using Lock-in  Thermography”, proceedings of ISTFA 2011, p 74-80


F. Naumann et. al.: “Efficient non-destructive 3D Defect  Localization by Lock-in-Thermography utilizing Multi  Harmonics analysis” Proc. of the 40th International  Symposium for Testing and Failure Analysis (ISTFA), 2014 130-135


F. Altmann et. al.: “Enhanced Failure Analysis on open  TSV interconnects” Proc. of the 38th International  Symposium for Testing and Failure Analysis (ISTFA), 2012 55-60


L. Kwakman et.al. : Sample Preparation Strategies for  Fast and Effective Failure Analysis of 3D Devices, Proc. of the 39th International Symposium for Testing and  Failure Analysis (ISTFA), 2013 17-26


M. Krause et. al.: “microPREPTM – A New Laser Tool  for High-Throughput Sample Preparation” Proc. of the  40th International Symposium for Testing and Failure  Analysis (ISTFA), 2014 270-276


M. Simon-Najasek et. al.: “ Advanced FIB sample  preparation techniques for high resolution TEM  investigations of HEMT structures”, Microelectronics  Reliability 54 (2014), 1785-1789


3D Integrated Power – A Discrete Perspective


Ian Kearney


Texas Instruments, Lehigh Valley Device Analysis Operations Laboratory  116 Research Drive, Bethlehem, PA 18015


iankearney@ti.com


Stephen Brink


Texas Instruments, High Power Solutions  50 Phillippe Cote St, Manchester, NH 03101  stephen.brink@ti.com


The shift in power conversion and power management  applications to thick copper clip technologies and thinner  silicon dies enable high-current connections (overcoming  limitations of common wire bond) and enhance the heat  dissipation properties of System-in-Package solutions. Powerstage innovation integrates enhanced gate drivers with  two MOSFETs combining vertical current flow with a lateral  power MOSFET. It provides a low on-resistance and requires  an extremely low gate charge with industry-standard package  outlines - a combination not previously possible with existing  silicon platforms.


These advancements in both silicon and 3D Multi-ChipModule packaging complexity present multifaceted challenges  to the failure analyst. The various height levels and assembly  interfaces can be difficult to deprocess while maintaining all  the critical evidence. Further complicating failure isolation  within the system is the integration of multiple chips, which  can lead to false positives. Most importantly, the discrete  MOSFET all too often gets overlooked as just a simple threeterminal device leading to incorrect deductions in determining  true root cause.


This paper presents the discrete power MOSFET perspective  amidst the competing forces of the system-to-board-level  failure analysis. It underlines the requirement for diligent  analysis at every step and the importance as an analyst to  contest the conflicting assumptions of challenging customers. Automatic Test Equipment (ATE) data-logs reported elevated  power MOSFET leakage. Initial assumptions believed a  MOSFET silicon process issue existed. Through methodical  anamnesis and systematic analysis, the true failure was  correctly isolated and the power MOSFET vindicated. The  authors emphasize the importance of investigating all  available evidence, from a macro to micro 3D package  perspective, to achieve the bona fide path forward and true  root cause.


The system in a package (SIP) approach takes a step toward  creating an ideal switch by reducing the device parasitics thus  dramatically improving its performance. In order to maximize


the performance of a typical synchronous Buck converter [1],


[2] the parasitic inductances and resistances in the power  circuit formed by the two MOSFETs is minimized (Figure 1). Through an innovative packaging approach in the multi-chip  module (MCM) this is accomplished where the MOSFETs are  actually stacked on a grounded lead frame with two copper  clips (Figure 2). The package also includes the IC controller  providing a further level of integration. The resulting power  stage 3D package has characteristics that make it unique in the  power electronics industry. The integrated package hosts the  controller, gate driver, control and sync power MOSFETs.


Figure 1: System Block Diagram of a Power System Design. The inductor current is controlled by both FET switches.


Figure 2: Illustration of a 3D stacked-die integrated package.


The 3D package construction consists of a low-side die (syncFET) attached to the main lead frame pad serving as the  ground connection of the MOSFET pair as shown in Figure 2. The syncFET die also integrates a small senseFET for  resistance monitoring. The syncFET drain connects to the


outside through a thick copper clip that is the device’s


switching node (SW or bottom clip). The switch node is the  point where the FET switches and inductor are joined. On top  of the thick copper clip, the high-side MOSFET (controlFET) is solder die attached. Another thick copper clip connects the  high-side drain (VIN or top clip) to the device’s external pins.


This paper discusses packages manifesting soft low-side FET  breakdown voltage at ATE testing. The test forced 100mA  into the switch node (SW) with both FETs turned off.


The customer presented the following observations: On a  correctly functioning part, the SW node voltage immediately  jumps up to the breakdown voltage of the FET, then abruptly  stops rising when the FET starts conducting in breakdown. On  a failing unit, the SW node voltage quickly raised to just over  8V, then the slope changed abruptly, and it slowly rose up to  the normal breakdown voltage over the course of tens of  milliseconds.


Initial assumptions by the customer suspected (i) marginal  FET lots due to poor final test yield, (ii)  physical, electrical or  contamination induced damage to the primary FET, sense FET  and/or Controller, (iii) mechanical or physical degradation in  the interconnects (FET gate wire, sense FET wires, clips, die  attach (DA) and/or Controller DA, wires).


Analysis and Discussion


Initial verification testing ran with stop-on-fail settings in  order to protect ATE hardware. It highlighted the VDD supply  was drawing excess current (Figure 3, pin 29) identifying  excess leakage current and soft breakdown in the Low Side  FET (pins 8-12) of the 3D package, as well as current sense  amp functional failure, and a high VDD supply current high in  the order of 2-3 mA, as summarized in Table 1. Turning stopon-fail off provided additional failure signature clues:-


1. SW leakage and soft breakdown voltage (BVDSS)


2. Current sense amp functional failure, OCF trip low and elevated power supply current (IVDD)


3. Oscillator parametric failure and dead-time tests


4. BP regulation error


For the failures, the “IVDD” power supply current was 2-3mA  higher than normal with the output enabled and FB (pin 34) pulled high (compared to a control). The curve tracer response  of the syncFET drain (pins 8-12) to 100mA current steps  tested the breakdown voltage of the syncFET. The response  looked like a “soft breakdown” at just over 8V, Figure 4. Figure 5 confirmed the excess leakage current. Other  observations were mechanical and high temperature bake  sensitivity where failing units appeared to recover.


To clearly understand all failure signatures a cross-functional  team from controller and power MOSFET development teams  worked in unison through external and internal package


inspection, package level probe, partial decapsulation and  visual inspection, internal micro-probing focusing on  connectivity and parametric specifications. Initial package  bench verification confirmed the customer’s syncFET  observations.


Figure 3: Package pin-out relevant to this analysis. Table 1: ATE summary observations.


Failures


Comment


Group 1


5 IVDD, 2 BP


Group 2


All IVDD


Group 3 All IVDD, all pass with pogo contactor  tightening


Group 4


Figure 4: External curve trace sweep (voltage Vs. Time) of  syncFET BVDSS. Failing units showed a “soft breakdown”.


Figure 5: DC Sweep of syncFET on typical failing unit  verified the excess leakage current. Good units exhibited less  than 100uA at 12V and 18V.


Control


Failure


Switch Node Voltage (V)


Time (ms)


Power MOSFET Analysis: CSAM analysis identified slightly  abnormal regions of package delamination when compared to  control units. This delamination (Figure 6) was present over  the exposed corners of the LSFET (gate side) and to a lesser  extent at pin 26 and 38 of the lead-frame. This did not  logically explain the syncFET electrical waveforms. Internal  inspection by x-ray (Figure 7) showed normal assembly.


Figure 6: CSAM analysis of Control Vs. DUT highlighted  some regions of delamination on failing units.


Figure 7: Typical package xray image.


Temperature profiling of the syncFET leakage had the  following conditions on a thermal hot chuck: VIN=VDD=5V; CNTL=Pgrnd; monitor syncFET leakage at 5V on VDS. The  test group contained Control, ATE pass and ATE syncFET  leakage failures. ATE Pass units tracked control units with  leakage values under 20 A, Table 2. The syncFET failures  got worse in some cases but returned close to their initial  values after cooling to room temperature. Cooling packages  with freeze spray had little effect. The “leaky” syncFET had a  strong temperature dependence supporting the reported  mechanical sensitivity.


Table 2: syncFET Temperature Dependence.


Units 4, 5, 8 and 9 were partial decapsulated and micro-probed  between the SW and Pgrnd pins (Figure 8). The U4 syncFET  leakage recovered while U5 deteriorated. Units 8 and 9 (ATE  pass) did not change. The interconnect wire resistance values  linking the syncFET and Controller die were in the normal  four milli-ohm range. Pseudo mechanical wire-pull testing  confirmed normal wire fracture response.


Figure 8: Partial chemical decapsulation allowed access to  the syncFET-controller wire interconnects for micro-probing.


The syncFETs were next electrically isolated from the  controller and characterized to datasheet limits. All devices  met specification confirming no intrinsic leakage (Table 3) was present in the primary syncFET silicon die. If the power  MOSFET were the true source of ATE leakage current, recovery would not occur after partial decapsulation.


Table 3: DC characterization of Sync Power MOSFETs after  isolation from the controller confirmed full recovery.


An important side observation noted the small-integrated  senseFET did exhibit unexpected leakage levels (Figure 9) that was characteristic of charge injection with a “channeling” appearance. This leakage recovered with the application of a  negative gate bias and/or appropriate temperature anneal.


Figure 9: SenseFET leakage recoverable with negative VGS.


Pin 38


Pin 26


Partial Decap Exposed ROI


Probe Socket


CONTROL


FAILURES


Wire Voltage (V)


The external package switching operation demonstrated  switch node behavior consistent with a floating LSFET gate. How could a floating gate scenario arise for the syncFET or  integrated senseFET if the gate-controller interconnects were  electrically robust? Next the analysis shifted to the IC  controller.


IC Controller Analysis: With each ground pin encapsulated  pin 26 and 38 were curve traced to all other pins at hot and  cold temperatures to see if any ground to pin characteristic  changed – especially looking for evidence of an open circuit. No significant curve trace changes anomalies noted.


To further investigate the CSAM abnormal delamination (Figure 10) the remaining epoxy mold compound (EMC) was  chemically removed (Figure 11) and exposed packages  inspected focusing on pin 26 and 38. Under low and high  optical magnification, all GND bonds and bond wires  appeared normal at pin 26 and 38.


Figure 10: CSAM delamination overlaid with package optical  micrograph after partial and full decapsulation.


Figure 11: Typical pin 26 lead-frame and IC wire bonds.


Initial SEM inspection showed intact wire bonds with no  evidence of cracks or damage (Figure 12).


Figure 12: Pin 26 & 38 SEM image of lead-frame wire bonds.


After SEM inspection, each pin 38 AGND wire was microprobed from the pin-pad to the controller die bond-pad (Figure  13 and Table 4). Certain wires had high resistance with some  exhibiting intermittently or completely open behavior. Lightly  touching the wire with a micro probe confirmed that the ball  bond readily lifted from the Pin 38 fused lead-frame. Repeating this procedure on Pgrnd pin 26 confirmed similar  random electrical opens for wire 1, 2, or 3.


Table 4: Example pin 38 (Agrnd) wire resistance analysis.


Figure 13: Optical inspection of fused lead frame at pin 26  appeared normal. SEM inset showed no anomaly either.


The Figure 13 failure was not due to Kirkendall voiding since  this was gold wire bonded to silver-nickel. Inspection by SEM  did not identify any residual intermetallics or raised features  under the ball bond [3]. The poor wire “stickiness” was solely  a result of low bonding pressure.


Further wire resistance measurements (Figure 14) also  confirmed unstable wire resistance behavior for both ATE  passing and failing devices while virgin units were within  specification.


Group Unit Resistance (mΩ)


Fail U4


OVLD


Fail U5 350, unstable


Pass U7 FA Look-ahead  Pass U8 689, unstable


Pass U9 OVLD, same as U4  Virgin Ctrl1


Virgin Ctrl2


Figure 14: Curve trace results confirmed unstable wires.


U4 Agrnd:   W3        W2    W1


Applied Voltage (V)


A second but related open circuit fail-mode condition  identified intact ball bonds but overly thin stitches on bump or  sharp bump landing of the stitch due to HIGH BQM settings  causing broken stitches, Figure 15.


Figure 15: Thin stitches on bump or sharp bump landing.


The final section discusses the analog and digital wire bond  observations with regard to explaining root cause of the four  ATE failure signatures.


Root Cause and Optimization


The syncFET leakage: was indicative of a sub-threshold  channel current, consistent with the LDRV signal floating  above the FET’s PGND. The BVDSS curve also indicated a  floating gate - capacitive coupling across the gate to drain (CGD) pulled the gate up as the drain started to slew, it  clamped and then discharged when the dv/dt on the drain  reduced.


Current sense amp functional failure, OCF trip low and  elevated VDD current: As PGND floats, its voltage became  higher than SW. As a result, the differential input seen by the  current sense amplifier (Figure 16) was large, causing the  current sense amplifier to rail high. This caused OCF to trip  low, and the current sense amplifier to draw extra VDD current.


Figure 16: Illustration of current sense amp circuit.


Oscillator parametric failure and dead-time tests: The floating  PGND caused cross-conduction because the LSFET did not  actually turn off, which resulted in failure of the dead-time  test, as well as some distortion of the SW node waveform on  the ATE during the test of the oscillator, causing the extracted  frequency to be incorrect.


BP regulation error: The regulators are referenced to their  local grounds. When one or both of the local grounds are open  due to cracked wire bonds or lifted AGND ball bonds, the  regulation error will occur, measured with respect to the  external true ground.


Bench measurements of the syncFET gate drive signal  replicated the fail-mode. Evidence of the ground for this signal (PGND) ground reference floating was captured on an  oscilloscope confirming the wire-bond theory. Figure 17  shows the Unit repeatedly shutting down and restarting due to  open-circuit events. In between the starts, the LDRV slowly  discharges because its ground return is floating.


Figure 17: Measurement of gate drive signals confirmed the  observations from the discrete MOSFET characterization.


The impedance of the LDRV signal was measured by pulling  the signal up through a 100 Ohm resistor in the measurement  configuration illustrated in Figure 18. This experiment verified  that the LDRV signal was floating, and only clamps when it  reached a voltage of 1.5V or higher (Figure 19), which is the  forward bias voltage of the two ESD protection diodes.


Figure 18: Configuration for measurement of LDRV  impedance. The voltage source is varied and the current into  the LDRV terminal is measured.


Figure 19: Measured characteristic of LDRV pulled up  through a 100-Ohm resistor. The zero current below 1.2V  shows that the LDRV was floating due to PGND floating.


BP3


PGND


The bond stitch on ball (BSOB) process involved multi-steps. First, a ball was created on the lead frame, and then a ball  bond (1st bond) on the IC followed by stitch bonding (2nd  bond) onto the ball initially created. This analysis identified  failures at step one and step three at the second bond.


A thin or sharp landing stitch on the bump induced stitch bond  cracking on top of the ball bond. In cases, the final wedge  shape was undesirable. The effective elimination of this  package failure mode was achieved by adjusting package  structure to prevent excessive mechanical stress and by  optimizing bond parameters to ensure strong stitch bonds.


Figure 20: Process improvement illustration.


A low contact force caused failure of the first ball (step 1). Contact and bond time may also have influenced the poor ball  adhesion.


The root cause of the ATE and bench failures was a floating  gate driver ground return and current sense amplifier positive  input due to PGND stitch bonds becoming open circuit, and an  induced ground differential between BP6 and BP3 due to the  AGND stitch bonds also entering an electrically open state.


The latent failures manifested generally after certain stresses  like load switching or temperature cycling. The mechanical  and temperature annealing device recovery further supported  this theory. Marginally connected bond wires re-connected  either from (a) the application of pressure to the package or (b) relative motion induced by temperature making the failing  signature recover.


The true root-cause disproved the initial and incorrect  assumption that the discrete MOSFET was inherently the  culprit.


The author wishes to express gratitude to LVDAO analysts B  Wolfe for CSAM analysis and D Yencho for detailed SEM  imaging. MDAO colleagues M Foley and S Holman for crossfunctional failure analysis support. Finally, S Brink for  application, design and bench testing discussions and insights.


[1] Texas Instruments Power Management Guide 2015, http://www.ti.com/lsds/ti/analog/powermanagement/techn ical-documents.


[2] Power Electronic Packaging: Design, Assembly Process, Reliability and Modeling, 2012, 609 pages, Yong Liu, 1461410533, 9781461410539, Springer, 2012 pp642.


[3] Electronic Device Failure Analysis, August 2015, Volume  17, Issue 3 pp 33.


Analysis of Integrated Current Sense in Multiphase Buck Converters


Accurate and lossless current sensing is vital for high  performance multiphase buck converters used in the latest  voltage regulation modules (VRMs). A synchronous FET onstate resistance based approach is an alternative topology to  DCR based sensing and is compatible with any controller, which requires inductor current information. The MOSFET  driver has built-in sense circuitry, which when co-packaged  with the MOSFETs reduces total footprint and ease of design. The Powerstage embodiment virtually eliminates the parasitic  inductance and resistance between Control and Synchronous  power MOSFETS; and using thick copper clips substantially  reduce the parasitics associated with the input supply voltage (VIN) and the switch node output voltage (VSW) connections  when compared to wire-bonded solutions.


This paper presents a novel investigation into a contradictory  low on-resistance paradox in a stacked 3D configuration. Through analysis, characterization and simulation the author  deciphered the conundrum leading to a root cause explained  by a mismatch of internal gain and referenced on-resistance. Building on previous metrology improvements the innovative  insights drove analysis toward root-cause.


Power MOSFET transistors [1], [2] are widely used in  synchronous buck DC-DC converters for the advantages of  small gate charge, low specific on-resistance, and large  breakdown voltage. A digital power solution may consist of  several interleaved synchronous buck converters [3] controlled  by a single microprocessor (Figure 1).


Figure 1: A Block Diagram of a typical six-phase buck system  and 3D Integrated Power package.


Accurate and lossless current sensing is necessary for high  performance multiphase buck converters used in the latest  voltage regulation modules (VRMs). An integrated current  sense technique improves accuracy and reduces solution  footprint [4]. This provides an alternative to thermistor based  temperature and DCR sensing (Figure 2). This synchronous  buck converter uses on-state resistance sensing of the sync  FET to derive an emulated signal proportional to the inductor  current rather than the common DCR sensing technique.


Figure 2: System architecture, proposed scheme with  integrated current sensing (left) vs. traditional DCR sensing  with external temperature sensing thermistor (right).


This integrated current sense technique is temperature  compensated, co-packaged with the FETs and trimmed to  achieve consistent high accuracy despite normal process  variation of the FETs. However, manufacturing tolerance  introduces significant variation in the on-state resistance of  individual FETs. This is normally accounted for using postpackage trimming. Co-packaging ensures that once paired the  driver will always remain with the specific FETs in the  package. Adjusting the current sense amplifier gain after  packaging ensures the desired gain accuracy of the device.


This work presents a theoretical yet paradoxical failure of a  multi-finger sync FET in an advanced 3D integrated power  package. Devices only failed the coarse trimming process due  to an internal post gain trim and syncFET BootR resistance  mismatch. Development engineering assumed an inherent flaw  existed in the gate driver design.


The package illustration in Figure 3 describes the stacking  topology, which compliments the source down silicon  technology enabling the high-side (top die or controlFET) MOSFET to be stacked above the low-side (bottom die or


syncFET) transistor to implement a synchronous buck  converter topology in a very simple and cost-effective manner. The pin-out is shown in Figure 3 for reference.


Figure 3: 3-D integrated synchronous buck converter.


Attaching the low-side die to the main pad of the lead frame  provides the ground connection of the MOSFET pair. The  low-side drain connects to the outside through a thick copper


RDS(O n)


Test


Coarse


clip that constitutes the device’s switching node (VSW or


Name


Code


6 to 13


8 to 13


bottom clip). On top of the thick copper clip the high-side


External


Internal


Pin#


MOSFET is solder die attached, which also uses a source


ITEST


20A


down technology. Finally, another thick copper clip connects


Normailzed Normailzed % Delta


the high-side drain (VIN of the buck converter) to the device’s


Unitsto RDS(On)MAXto RDS(On)MAXVs. Pin 6 Serial #


external pins. Internal connections are Au wire bonds. The


0.97


0.63


-58%


bootstrap capacitor, connected to Boot and BootR pins,


0.99


0.65


provides the charge to turn on the control FET. BootR


0.57


-63%


provides the return path (Figure 4) for the HS gate driver and


0.91


0.76


-46%


connects to VSW internally.


0.92


0.71


-50%


0.96


-33%


% Delta


9%


43%


Figure 4: Buck-converter resistance sense circuit as in [4].


Refer to [4] for a detailed description of Figure 4 and circuit  operation. Equation 1 describes the approximation of the  syncFET on-time inductor current.


     =     


    (  −    ℃)      (    ),    ℃


Equation 1


The current sense amplifier gain is represented by GS, VDS is  the syncFET drain to source voltage, GT the FET technology  temperature coefficient and RDS(ON),25C the syncFET on-state  resistance at 250C as measured by the internal driver. Postpackage trimming matches the co-packaged driver and FETs  to overcome variations in individual FET RDS(ON) values. The  GS gain is set, depending on RDS(ON)  value sensed, to maintain  the current sense amplifier output at the desired gain of 5  mV/A of inductor current.


This analysis reports the theoretical effect of a short trim range  with limited coarse coding (CC) and sensed RDS(ON) variation  from a failure analysis perspective.


Table 1 summarizes the normalized external and internal  package ATE RDS(ON) values and the percentage resistance  deltas. The internal package values significantly varied from  each other and contradictorily compared to external values. Bench verification confirmed ATE values. The initial gain  value was set from a coarse code look-up table. For trim range  1, device one to three were out of specification and failed the  trim and hard EPROM coding process. Analysis focused on  why for a given external package resistance the internal  RDS(ON) values failed to track controls. Secondly, why were the  internal RDS(ON) values so low?


Table 1: Normalized external and internal ATE RDS(ON) values. Coarse code E was outside the gain code specification, GS  could not be to maintain 5mV/A during test.


Proceeding through the FA process flow, no obvious  anomalies were evident from external package inspection. Non-destructive internal observation by CSAM and XRAY  techniques (Figure 5 and Figure 6) identified limited single  and cumulative solder voiding but these should only increase  resistance. External RDS(ON) values indicated no abnormal  resistance increase. There was no sensitivity to either ground  sense position either.


Decapsulation and physical cross-section (Figure 7) further  confirmed the void observations. Resistance measurements  from the BootR pad were 18% to 37% lower than expected. All wire and clip resistances were normal. Could solder  voiding produce a resistance decrease?


Figure 5: CSAM 50 MHz Pulse Echo, DUT Vs. Control.


FAILURE


Figure 6: Internal package x-ray inspection comparing DUT  Vs. control.


Figure 7: Post decapsulation solder profiles and SEM of  horizontal and diagonal cross-section directions.


By mounting units to replicate true stacked die current flow  micro-probe analysis enabled detailed resistance mapping and  isolation of the low 150-300µΩ resistances. The multi-finger  power MOSFET is essentially a 3D distributed resistor  network. Toggling the syncFET on/off with different current  force paths enabled the study of the vertical and lateral current  flow effects on the distributed resistance values (Figure 8).


Figure 8: Illustration of 3D distributed resistor network in a  multi-fingered power MOSFET and summary µprobing data.


Micro-probing measurements, Figure 8, confirmed beyond  argument that subtle voiding at a specific location would  paradoxically produce a low resistance value. The suspected  failure mechanism was next validated through silicon device  simulation.


Optimization and Verification


R3D simulations were conducted which convert layout files  into metal and vias. Metal is shown as potential and lateral  current distribution; vias are the vertical current distribution. Model parameters were 1mΩ.cm substrate, spreading  resistance (rsp) = 4.8mΩ.mm2 at 4.5 VGS, metal sheet  resistance 9.3mΩ/sq. To mimic FET on state a bias of 0.1  volts was applied to the drain with the source grounded.


This first pass simulation study (Figure 9 and Figure 10) confirmed the FA observations. Lateral spreading resistance  and non-uniform current distribution had an effect on BootR  resistance sensing.


Drain potential was maximized under clip-solder regions. With optimal solder coverage, the potential rolls-off by almost  15% from the clip edge to BootR.


Separating the clip edge & BootR with a theoretical 20% solder void produced an approximate 50% potential gradient. When current flows through metal it produces a voltage drop. A longer path (theoretical solder void) increases the lateral  resistance & the associated voltage drop.


Figure 9: R3D potential gradient simulations.


Figure 10: R3D lateral and vertical current simulations.


Underneath the clip, lateral current flow was a minimum. Immediately adjacent the clip-solder region the current density  is largest. There is a current density gradient toward die edges. Underneath the clip, vertical current flow is maximized. At  edges adjacent the sense pad it is significantly reduced due to  lateral spreading resistance affects. Our theoretical study


identified how solder voiding adjacent a sense pad aggravates  this (simulated 1.4E-5A/µm2 V’s 8E-6A/µm2).


tests evaluation methods and will correlate them to the  tomography parameters.


B. Electrical Tests


In our experiments, we tested two types of device: flash  memories and FPGAs. We have developed different electrical  test procedures for each type as shown in Fig. 5. The details of  each type will be discussed in the following subsections.


Figure 5: Electrical test procedure for (a) Flash memories  and (b) FPGAs


Figure 11: The wire bond diagram highlighting BootR virtual  sense point and solder dispense pattern.


The reported failures were from a theoretical study using a  non-optimal gain code specification confined to two coarse  codes and modified solder dispense pattern (Figure 11). Using  full trim range eliminates any risk of violating the gain code  specification and ensures the GS value is adequately set to  maintain the 5mV/A target and compensate for any  abnormally low sensed RDS(ON)_25C relating to Equation 1. Stringent solder coverage tolerances combined with in-line  single and cumulative voiding inspection are further process  controls. Finally, the ATE final test strategy is such that  checks are in place to screen any potential inspection  escapees.


This innovative analysis identified a unique trim code failure  mechanism caused by solder voids producing a paradoxically  low on-resistance (RDS(ON)) scenario due to deviations  introduced in lateral and vertical current flows.


Simulation confirmed bench measurements in that for a given  test current BootR inherently sensed less voltage. Analysis  reported how a specific type of solder void actually reduced  the voltage, and consequently the sensed resistance confirming  the low ATE on-resistance phenomenon.


Die current flow was proven to be non-uniform especially  adjacent the sense pad. This further reduced the virtually  sensed on-resistance.


The author wishes to express gratitude to D Yencho for SEM  analysis, N Otta for CSAM interpretation, K Thomas for final  test and EPROM coding discussions, and T Ramann for  device design and R3D simulation discussion.


[1] “History of FET Technology and the move to NexFET”, Jacek Korec and Chris Bull, Bodo’s Power Systems, May


2009.


[2] “Next Generation of Power MOSFETs,” Jacek Korec and  Shuming Xu, Power Electronics Europe, May 2009: http://www.powermag.com/pdf/issuearchive/29.pdf.


[3] Case Study: Texas Instruments Digital Power Solutions; D Alter; EDN Network August 03, 2006.


[4] “An Integrated Current Sense Technique for Multiphase  Buck Converters to Improve Accuracy and Reduce  Solution Footprint”, E Reutzal, Rengeng Chen, Scott  Ragona and David Jauregui, APEC 2013.


## Update on Draft SAE AS6171 Standard - Tools and Techniques for Detection and Mitigation of Counterfeit Electronics


Update on Draft SAE AS6171 Standard - Tools and Techniques for Detection and  Mitigation of Counterfeit Electronics


## William E. Vanderlinde


William E. Vanderlinde


Intelligence Advanced Research Projects Activity, Washington, DC, USA


Bhanu P. Sood


Mechanical Engineering, CALCE, University of Maryland, College Park, MD, USA


In recent years, the prevalence of counterfeit electronic parts  has greatly increased, with reports of parts discovered in  critical applications such as medical systems, military  electronics, and process control equipment. This increased risk  has not only focused the spotlight on counterfeit component  detection methods, but the ability of these techniques to  uncover suspect parts that are produced using sophisticated  counterfeit creation techniques. The Society of Aerospace  Engineers (SAE) AS6171 Aerospace Standard standardizes  the test and inspection procedures, workmanship criteria, and  minimum training and certification requirements to detect  counterfeit electrical, electronic, and electromechanical (EEE) parts. The standard comes in response to a significant and  increasing volume of counterfeit electrical, electronic, and  electromechanical parts entering the supply chain. This short  manuscript and accompanying talk will update the audience  on the risk based methodology for detecting potential  counterfeiting related defects.


The SAE AS6171 Standard was created in response to a  significant and increasing volume of suspect/counterfeit EEE  parts entering the supply chain, posing significant  performance, reliability, and safety risks. The standard was  created to provide uniform requirements, practices and  methods for testing EEE parts to mitigate the risks of  receiving or using such parts. Since the approach is risk-based, the document includes a standardized methodology for  assessing risk, and a means by which cognizant engineers can  link technical assessments with tools to guide actions and  adaptively manage the identified risk through incremental  testing for more critical risk assessments, and monitoring and  feedback through the test evaluation process.


The AS6171 document classifies all counterfeit devices into  seven categories. These include devices that are produced by  recycling parts that are reclaimed from systems (recycled), devices that originated from an authorized manufacturer, but  have been replaced with a forged marking (remarked), illegally manufactured devices (overproduced), defective  devices (out-of-specification), a part that has been reproduced


## Bhanu P. Sood


without permission from the original manufacturer (cloned), parts with forged documentation, and tampered devices.


The target audience of the standard includes independent  testing facilities, distributors and original equipment  manufacturers that have in-house testing capability, and also  OEMs, system integrators or end-users that plan on flowing  down the requirements to sub-tier supply sources. The  Standard includes required certification and training of  personnel to address proficiency requirements specified in  each of the test method document. The Standard, which is  applicable to a wide range of active semiconductor devices, discretes, passives and electro-mechanical devices, further  specifies the requirements for a minimum level of inspection  and testing using various techniques and a sampling plan that  is based on tier level of accepted risk, level of confidence  required, and acceptable reject criteria. An example of the  sampling plan for complex active parts in risk tiers ranging  from Very Low to Critical is shown in Table 1.


The test and inspection slash sheets of the standard for  different classes of parts are written with the intention of  certifying test laboratories and ensuring that competent  individuals perform the inspection as per the techniques  specified in the slash sheets. The test techniques incorporated  into the Standard are indicated in the first column on Table 1. The risk model that determines which tests must be used for  parts depends on their source and their intended use. As an  example, the suggested flow as per Table 1 very low risk part  includes external visual inspection (EVI) (general), EVI  remarking, x-ray fluorescence (XRF) lead finish and 2-D  radiological (X-ray) inspection. EVI, XRF, and X-ray are thus  critical techniques because they are the only inspections  required for all parts per the AS6171, and will likely be the  only inspections that most parts will witness. EVI is used to  detect indications of possible counterfeiting such as nonuniform leads, re-plated leads, bent, damaged, corroded or  missing pins, discolored or damaged solder balls, non-standard  package markings, and unusual surface textures which may  indicate resurfacing. EVI remarking techniques include  chemical and mechanic methods to destructively remove  resurfacing material known as blacktop. Many examples of  suspect parts detected by external visual inspection will be  shown during the presentation.


Table 1: Examples of test sequences to achieve the overall defect coverage threshold for five risk tier levels (very low to critical) – as  applicable to complex active parts.


Physical/Environmental/Electrical  Inspections/Tests


Critical  Risk


High  Risk


Moderate


Risk


Low  Risk


Very Low


Ex 1 Ex 1 Ex 2 Ex 1 Ex 2 Ex 1 Ex 2 Ex 1 Ex 2


EVI, General (Full Lot)


X


EVI, Detailed (Sample)


EVI, Remarking


EVI, Resurfacing


EVI, Part Dimensions


EVI, SEM


XRF, Lead Finish Analysis


XRF, Lead Finish Thickness


XRF, Material Composition


DDPA, Internal Inspection


DDPA, Bond Pull


DDPA, Die Attach


Radiological, 2D


Radiological, 3D, Incremental


Radiological, 3D, Independent  AM, PEMS – External only


AM, PEMS - External, Internal & Material (Incremental)


Electrical, Curve Trace, at ambient temp.


Electrical, DC Test at ambient temp.


Electrical, Key Parameters (AC, Switching, Functional) at ambient temp.


Electrical, DC Test and Key Parameters (AC, Switching, Functional), over temp.


Electrical, Burn-In with Pre- and PostElectrical Tests


Electrical, Temperature Cycling with Pre- and  Post-Electrical Tests


Electrical, Seal (hermetic devices)


Raman


FTIR


TGA


Design Recovery, Level 1: Simple manual  comparison


Design Recovery, Level 2: Layout comparison


Design Recovery, Level 3: Selective


functional comparison


Design Recovery, Level 4: Full microcircuit


comparison


Note: X: Test is to be performed


User/Requester designates any inspections and/or tests that may have been invoked in the contractual language by the User or Requester


The AS6171 slash sheet pertaining to radiography defines the  methodology for suspect parts inspection using radiological  inspection. The purpose of radiology for suspect counterfeit  part inspection is to detect deliberate misrepresentation of a  part, either at the part distributor or OEM level. Radiological  inspection can also potentially detect unintentional damage to  the part resulting from improper removal of part from  assemblies, which may include, but not limited to, prolonged  elevated temperature exposure during de-soldering operations  or mechanical stresses during removal. The techniques that are  discusses in this slash sheet include film radiography and  filmless radiography such as digital radiography (DR), real  time radiography (RTR), and computed tomography (CT). The  analysis is performed on parts to verify that the internal  package or die construction is consistent with an exemplar  item. In case an exemplar item is not available, the document


recommends that comparisons be made within a homogenous  sample population using the technical data available for that  item.


SAE AS6171 is expected to be approved for release by the end  of calendar year 2015. AS6171 will provide the counterfeit  detection community with standardized test and inspection  procedures, workmanship criteria, and minimum training and  certification requirements to detect counterfeit electrical, electronic, and electromechanical parts. This will enable endusers a measure of confidence in parts that have been tested by  laboratories adhering to the published standard.


Analyzing the Impact of X-ray Tomography on the   Reliability of Integrated Circuits


Halit Dogan1, Md Mahbub Alam2, Navid Asadizanjani2, Sina Shahbazmohamadi3, Domenic Forte2 and Mark Tehranipoor2


1Electrical and Computer Engineering, University of Connecticut, Storrs, CT, USA  3Mechanical Engineering, Manhattan College, Riverdale, NY, USA


2Electrical and Computer Engineering, University of Florida, Gainesville, FL, USA  Email: {dforte, tehranipoor}@ece.ufl.edu


X-ray tomography is a promising technique that can provide  micron level, internal structure, and three dimensional (3D) information of an integrated circuit (IC) component without  the need for serial sectioning or decapsulation. This is  especially useful for counterfeit IC detection as demonstrated  by recent work. Although the components remain physically  intact during tomography, the effect of radiation on the  electrical functionality is not yet fully investigated. In this  paper we analyze the impact of X-ray tomography on the  reliability of ICs with different fabrication technologies. We  perform a 3D imaging using an advanced X-ray machine on  Intel flash memories, Macronix flash memories, Xilinx Spartan  3 and Spartan 6 FPGAs. Electrical functionalities are then  tested in a systematic procedure after each round of  tomography to estimate the impact of X-ray on Flash erase  time, read margin, and program operation, and the frequencies  of ring oscillators in the FPGAs. A major finding is that erase  times for flash memories of older technology are significantly  degraded when exposed to tomography, eventually resulting in  failure. However, the flash and Xilinx FPGAs of newer  technologies seem less sensitive to tomography, as only minor  degradations are observed. Further, we did not identify  permanent failures for any chips in the time needed to perform  tomography for counterfeit detection (approximately 2 hours).


The problem of counterfeit electronic components continues to  grow given the increased complexity of the supply chain and  the lack of appropriate countermeasures and detection  schemes. Counterfeit components do not possess the exact  same specifications as genuine parts, and can impose  significant vulnerabilities and threats to the systems in which  they are placed. If such parts end up in critical applications (defense, medical, aerospace, transportation, etc.), catastrophic  scenarios that result in mission failures, health and safety  hazards, and jeopardize national security can occur. Thus, it  has become imperative that manufacturers, distributors, and  users of electronic components inspect all electronic  components for authentication. In addition, counterfeit parts


have a negative impact on corporate identity and reputation  which can trigger massive revenue losses.


Several test methods have been developed to distinguish  counterfeit parts from authentic components. The most  common detection methods employed by test labs are physical  inspection methods which include incoming inspection, exterior test, interior test, and material analysis. Recently, Xray Microscopy (XRM) and tomography have distinguished  themselves as promising approaches to detect counterfeit ICs  due to their ability to unveil the obscured features and details  of parts in a nondestructive fashion [1–3]. Although limited  information can be extracted from a two dimensional (2D) Xray images such as bond wire configuration, die orientation, or  lead frame, they lack critical information compared to 3D  images such as presence of cracks in the die, die face  delamination, reworked bond wires, and bond wires  configuration in a chip. 3D images, reconstructed from a series  of 2D X-ray projections obtained at various rotation angles  reveal more information on both interior and exterior of  samples. This technique opens up new possibilities for  physical inspection procedures and may contribute in a faster  and lower cost detection of counterfeit parts [2–5].


Unlike 2D real-time X-ray imaging, a device undergoing  tomography is exposed to irradiation for long time. In other  words, higher X-ray power and/or longer scanning is needed in  order to obtain high resolution images that are free from  artifacts. Even though X-Ray tomography is deemed to be  non-destructive, it has been reported to affect several IC  parameters [6, 7]. While there have been some efforts to show  the effect of X-ray on integrated circuits [8–11], none have  explicitly investigated the effect of tomography.


This paper attempt to answer many questions related to the  concerns on the reliability of X-ray tomography, which is one  of the most advanced and effective detection techniques for  counterfeit electronic components.


In this work, we examine the effects of X-ray tomography on  two types of integrated circuits with different process  technologies: (i) flash memories (400 nm and 150 nm) and (ii) FPGAs (90 nm and 45 nm). For both the flash memories and  FPGAs, test setups and procedures are designed to capture the


parameter shifts and failures caused by repeated X-ray  exposure. The effect of X-ray studied in this work is total  ionized dose (TID). This is selected due to the fact the devices  are not powered up when inspecting the ICs for counterfeit  detection with X-ray tomography [6].


The rest of the paper is organized as follows: In Section 2, we  elaborate the radiation-induced failure mechanism in CMOS, flash memory and FPGAs. The experimental set up and test  procedures are described in Section 3. Section 4 presents the  experimental results and its analysis. We conclude the paper in  Section 5.


Preliminaries


In this section, we provide background on the sources of  failure from irradiation in basic CMOS circuits, flash memory, and FPGAs. For FPGAs, we shall focus our discussion on ring  oscillator (RO) circuits which will be used later to capture the  degradation in our experiments.


A. Impact of Radiation on CMOS


Radiation damage in CMOS electronics based on TID effect  has been described in several earlier works [6, 8, 10–12] . Xray interacts with the atoms of the matter through photoelectric  effect and scattering effect. Electron hole pairs are generated  from these interactions.


The ionization process due to radiation is depicted in Fig. 1. The physical process started from initial deposition of energy  can be described as follows:


1. The process is initiated with the generation of  electron hole pair by energy deposited on gate oxide. The density of generated pairs depends on the  strength of the radiated energy. With electrons having  higher mobility than holes, a fraction of the electrons  are swept out quickly from the oxide.


2. Simultaneously some fraction of electrons recombine  with holes as a function of the energy of incident  particles [12].


3. The remaining holes move to the oxide/Si interface  through the states of the oxides via hopping transport. Portions of these holes fall into deep traps in the  oxide or near the interface. These trapped holes  create positive charges and are known as oxide  trapped charge. The amount of oxide trapped charge  is proportional to the thickness of the oxide.


4. Another major contribution of TID effect is the  radiation-induced buildup of interface traps at  oxide/Si interface. The trapped hole defects at  interface may exchange charge with bulk Si via  electron tunneling and can create interface tapped  charge. The reactions between holes and hydrogen  containing defects or dopants also help to form the  interface traps [7, 13]. These traps are localized states  with energy levels in the Si band-gap.


Oxide trapped charge can have a significant impact on  electrical parameters of integrated circuits such as shift in  threshold voltage, and change in switching speed of the  devices. The radiation-induced buildup of oxide trapped  charges shifts the gate to source bias point in the negative  direction. This leads to a reduction in threshold voltage and an  increase in off state and drive current in NMOS. In PMOS, the  threshold voltage becomes more negative and the off state and  drive current are reduced [6, 7].


Interface trap charge affects the subthreshold swing of a  CMOS device. This causes an increase in threshold voltage in  NMOS and a decrease in threshold voltage in PMOS. It also  increases the flicker or 1/f noise in CMOS devices [6].


B. Flash Memory


Flash memories have been the subject of few studies regarding  TID effect [11, 14–17]. Ionization effect in complex control  circuitry such as floating gate transistors and charge pump  degrades the performance of flash memory. These are  discussed in more detail below.


A floating gate transistor (FG) is the basic storage element in  flash and is used to store one or more bits of data (see Fig. 2). There are three sources of degradation in the FG due TID  effects.


1. Induced trapped charges are generated in the oxide  due to TID effect. The trapped generation mechanism  is similar to the trapped charge generation in CMOS  oxide. Note that due to the thick tunnel oxide region  between ﬂoating gate and the channel, ﬂash memory  in older technologies should intuitively be more  susceptible to the oxide trapped charges.


2. A fraction of surviving holes generated in the oxide  may drift toward the floating gate and recombine with  electrons. This process leads to a reduction of  electrons in floating gate.


3. Floating gate transistor can also lose charge due to  photoelectric effect, i.e., impinging radiation provides  enough energy for electrons to jump over the oxide. The transistor programmed in the high threshold


Figure 1: Total ionization dose (TID) effect in CMOS.


voltage moves toward a lower value after irradiation. Conversely, devices programmed in lower threshold  state experience an increase in threshold voltage, that  is, a positive charge loss from FG [11]. The shift in  threshold voltage may corrupt the stored data and/or  reduce the retention of the data.


Figure 2: Cross section of a standard floating gate memory  cell.


Flash memories often utilize a charge pump (multi-stage  circuit) to convert the supply voltage (VDD) to a higher voltage  that is generally required for an erase operation. Charge pump  circuits share a basic design as illustrated in Fig. 3. The  common characteristics of a charge pump that has m number  of stages can be described by following equation:


 (m  1) (V DD  V )


out


r


where, the threshold voltage of each of the MOS is denoted by  Vr. The generated output voltage is directly proportional to the  number of charge pump stages and, therefore, can be generated  even at a very low supply voltage. Output voltage strongly  depends on threshold voltage of the MOS.


Figure 3: m stage Dickson Charge pump circuit with MOS  diodes [18].


As we mentioned in earlier section, the degradation due to TID  effect can cause changes in the threshold voltage of the  transistors. As a result of this deviation, the output voltage of  the charge pump might alter as well, which can create  unexpected behavior in flash memory operations.


C. Ring Oscillator (RO)


In the FPGAs under evaluation, Ring Oscillators (ROs) will be  created to evaluate the performance of FPGAs. A ring  oscillator is a circuit that consists of an odd number of delay  stages connected in series to form a closed loop chain. An  example where each delay stage consists of an inverter is  shown in Fig. 4.


Figure 4: Ring Oscillator with odd number of inverters


The oscillation period is twice the sum of the delays of all  elements that compose the loop. Thus, the oscillation  frequency of n stage inverters can be expressed as:


fo n


2d ,i i1


where, d,i delay of ith delay element.


It is already mentioned that oxide trapped charges and  interface trapped charges are generated due to TID effects. It  results in a drift in threshold voltage of the MOS transistor. Since the drain current of each transistor is a function of its  threshold voltage, the drain current shifts. It causes a change in  delay of the circuit.


In this experiment, ROs are mapped on FPGAs using Look-up  Tables (LUTs). Even though the implementation of ROs in  FPGAs is different than ROs implemented by inverters, the  change in the DC characteristics is expected to be similar after  the X-ray radiation as both implementations consist of MOS  transistors. For the FPGA implementation, however, the  changes drastically depend on the architecture of the FPGA, which could be either NMOS dominant or PMOS dominant.


Experimental Setup and Test Procedure


In the following subsection, we discuss the experimental  setups, the devices that were used in our experiments, the Xray tomography procedure, and the electrical tests used to test  the ﬂash memories and FPGAs before/after exposure.


A. X-ray Tomography Parameters


There are many parameters such as exposure time, source  power, etc. that must be tuned carefully during a general X-ray  tomography in order to achieve successful imaging process. Optimized values of such parameters have been investigated  previously by the authors for different purposes including  reverse engineering of Printed Circuit Boards (PCBs) [19] and  Thermal Barrier Coatings (TBC) [20]. For counterfeit IC  detection, however, even greater care in parameters is needed. First, the imaging must be good enough to capture the defects


within a counterfeit IC with high conﬁdence. At the same time,


however, too much exposure may damage the chip under test (degrading its performance or leading to failure). Thus, the  trade-off between imaging (counterfeit detection) and  component failure must be carefully managed.


The impact of the X-ray tomography parameters on the ICs is  better to be tracked in a systematical way which has not been


investigated before. A Design of Experiments (DOE) table is  prepared for this purpose. There are also four different types  of semiconductor device fabrication technologies selected, based on their availability, in order to see the trend of the  imposed effects on newer technologies and compare to older  ones.


The X-ray exposure tests are performed using the Zeiss Versa  510 machine which is equipped with Resolution at a Distance (RaaD) system. Compared with the traditional conventional  tomography, the X-rays are better focused in this new  generation of the machines. This results in better quality of  images and sharper edges. The source distance and the ﬁlter  are selected based on the limited publications available in the  literature on the X-ray impact on ﬂash memories. Although  there are general understandings about the X-ray impact on  such devices, details regarding the maximum time and power  of the exposure are not well understood, especially with  respect to 3D imaging. The DOE is presented in the Table I.


Table 1: X-ray Exposure Settings


Tomography parameters


Source distance from sample(mm)


110


Exposure time (Hrs)


0.25-0.50-1.0-2.0-4.0 [Source voltage (kV), power (W)] [60,7] [80,8] [100,9] [120,10]


Filter


Al – 1mm


In this experiment the distance between the source and the  sample is kept constant at 110 mm for all the tests. Source  voltage and power are the two parameters directly related to  the energy of the electrons bombarding the target metal in the  x-ray source. Higher power results in photons with higher  energy, which will result in better X-ray transmission through  the material and less signal to noise ratio. In order to reduce  the effect of hard X-rays on the chips, we have used a 1 mm  aluminum ﬁlter right in front of the source, which will protect  the chips from defects due to the characteristic X-ray emission.


The quality of the image and time of tomography are the two  important parameters directly related to the source power and  exposure time. Increasing the exposure time will result in  higher number of received X-ray counts by the objector, which  increases the signal-to-noise ratio for images. An increase in  source power will result in higher transmission rate, better  resolution, and faster tomography for high Z material. On the  other hand, the contrast for low Z material will be decreased. Given that high Z material is used in electronic chips, higher  power seems to be the obvious choice, but those same  parameters are also responsible for creating defects in ICs. Depending on the size of the chips and the required image  resolution, one can extract the 3D information about the lead  frame, die rotation, bound wire conﬁguration, and the overall  internal structure from a 1-2 hour of X-ray tomography. In  Section 4, we will quantify the defects using the electronic


B. Discussion of Flash Memory Results


As the results clearly show, there can be large change in the  erase time. This can be explained as follows. The erase  operation in NOR flash is described by Fowler Nordheim  injection shown in following equation [15, 22].


A 


 S TUN  E TUN  exp( B


FN


TUN


i


(4)


ETUN is the electrical field through the thin oxide. STUN is the  injecting area under the floating gate, A and B are the FowlerNordheim parameters. From above relation it is obvious that  the most important parameter affecting the total charge  injection or erase time of a ﬂoating gate transistor is the  electric ﬁeld in the tunnel oxide. The electric ﬁeld is directly  proportional with the erase speed so when the electric ﬁeld  goes up, the erase speed goes up as well. The electric ﬁeld  itself is also directly proportional with the source power [23]. Based on these we have two explanations for the degradation.


First, the failures may be a result of degradation in the charge  pump unit of the ﬂash memory. Charge pump degradation due  to X-ray tomography can be understood from output voltage (see Equation (1)). Since ionizing dose effect shifts the  threshold voltage Vr, the output voltage of the charge pump is  reduced. Any increase in stage-to-stage leakage might also  reduce the output voltage. The reduced output voltage of  charge pump is responsible for slowing down the erasing and it  can fail the erasing operation. Our explanation is partially  supported by the above results. When the device failed to  complete the erase operation with charge pump (5V), it was  later erased successfully with 12V. Erase time of second set of  Intel flash without charge pump, i.e., with 12V has also been  measured in each tomography cycle and it showed the same  increase trend with a longer erasing time (see Fig. 9). This  observation concluded that charge pump degradation is not the  only unit responsible for the change in erase speed.


Second, radiation-induced defects may be created in the tunnel  oxide as described Section 2A. Oxide trapped charges and  interface trapped charges can affect the electric ﬁeld across the


tunnel oxide, and therefore cause the increase in erase time. In  addition, both interface and oxide traps increases  monotonically with radiation dose [7]. Therefore with the  increase of time, the number of defects increases. This leads to  higher erase time and eventually failure. In addition, higher  energy radiation enhances the ionization process and makes  the failure process faster.


Figure 9: Change in the erase time due to X-ray tomography  for Set-2 Intel ﬂash memories with 12V.


The above-mentioned effects are a strong function of the  thickness of the oxide. The number of defects in oxide is  reduced with the thickness of the oxide. Charge pump  degradation is expected to be lower in new technology with a  thinner oxide as well. Hence, it can be anticipated that newer  technology is more resistant to X-ray tomography. As we see  from Macronix flash memory result (Fig. 8), radiation effect  has little impact, if any, on erase time. This supports our  earlier anticipation.


It has been observed that 2 hours of X-ray scan with high  source power such as 120 kV can ensure high-resolution  images with enough information that can detect counterfeit IC. If the source power decreases, the scan time should be kept  longer to maintain the quality. It has been seen that the erase  time went up to 9.5 seconds (initially 3.17) and 5.4 seconds (initially 3.5) for sample 1 and sample 5, respectively after 3  hours and 45 minutes of tomography at 60KV source power. This number goes up with higher source power. These  numbers are less than the datasheet speciﬁcations. However, as  degradation is observed, it might not be safe to use X-ray  tomography for this speciﬁc ﬂash memory. On the other hand, tomography seems to be safer when carried out for  comparatively newer technology flash because of their  resistive nature to long term radiation.


C. FPGA Results


For the FPGA experiments, two Spartan 3 and two Spartan 6  FPGAs were tested. Our aim was to utilize as many CLBs in  both FPGA types as possible to get a uniform distribution of  change in the frequency of the ROs. The test procedure  mentioned in earlier section was applied to the FPGAs. Since  FPGAs were not powered on, we only expected to observe


total ionizing doze effects, which could change the DC  characteristics of the transistors [6].


Figure 10: Percentage change in the frequency in Spartan 3  and Spartan 6 FPGAs due to X-ray tomography.


1. Spartan 3: The results of tomography cycles for Spartan 3  and Spartan 6 FPGAs have been illustrated in Fig. 10. Tomography time is represented in the x axis and the y axis  corresponds to percentage change in ring oscillator’s  frequency. Average RO frequency increases with tomography  time for both Spartan 3 FPGAs. Both of them showed an  identical trend. Maximum variation was found at 19 hours and  45 minutes of tomography. As it is mentioned earlier that each  frequency value of FPGAs were calculated by taking averages  of all the ring oscillator frequencies, we checked the  consistency of the standard deviation of each data points. Standard deviation are within 2288 ± 3 and 1923± 4 for  sample 1 and 2 respectively. This justifies the consistency of  the data.


2) Spartan 6: Unlike Spartan 3, Spartan 6 results are less  consistent. For the ﬁrst sample, there was no change until the ﬁrst 4 hours of tomography. After the 4 hours of tomography, the frequency of the ROs decreased a little but it recovered  after that cycle. The second sample experienced an increase in  the frequencies of ROs but it did not have the same trend as in  Spartan 3 FPGAs. Percentage frequency change in sample 1 at


7.75 hours tomography exhibited a large discrimination. This  might come from measurement noise (imprecision of  equipment, environmental temperature, etc.) or variations in  the text procedure (e.g., more recovery time between exposure  and measurements). While standard deviation of other data  points of sample 1 is around 720, this particular data point has  standard deviation of 697. Thus, this point is inconsistent with  others.


D. Discussion of FPGA Results


It is observed that both Spartan 3 FPGAs experienced an  increase in their average RO frequencies. Since we do not have  access to the proprietary architectural details of the Spartan 3  FPGA, it is difficult to give a deﬁnitive explanation to the  results. One possible reason of frequency degradation can be  obtained considering total ionization dose effect. It is already


mentioned that oxide trapped charges leads to reduction in the  NMOS transistor threshold voltage and negatively increases  the PMOS transistor threshold voltage [6]. The delay of a  MOS transistor is inversely proportional to the overdrive  voltage. A lower threshold voltage results in a decrease of  delay of the circuit and thus increases oscillation frequency. Following increasing trend of average frequency it seems that  Spartan 3 FPGAs might be NMOS dominant.


Spartan 6 FPGAs are newer technology so the gate oxide is  thinner. Thus, it is expected to have less oxide trapped charges  due to TID. Instead of oxide trapped charges, border charges  and interface traps are expected to be more dominant. It is  known that these defects leads to an increase of noise in the  transistors, so that the frequencies of ROs might be noisier. This may be partially responsible for the observed  inconsistency.


We should note here again that 2 hours of tomography with  120 kV provides very detailed 3D image for the counterfeit IC  detection. Therefore, we are mostly interested in the results up  to the cycle with 2 hours of tomography which is in total 3  hours and 45 minutes of tomography in this experiment. We  can see from Fig. 10 that before the ﬁrst 4 hours of  tomography, the percentage change in RO frequencies are  insignificant. While we cannot directly conclude that it is safe  to use X-ray but it is obvious that there is little impact on the  performance or DC characteristics of the FPGAs.


E. Summary of Major Findings


We summarize the major results of this section as follows:


 High resolution 3D imaging of ICs require 2 hours of  tomography at 120KV source power. The Intel flash  memory failed the erase operation with charge pump  after 3 hours and 45 minutes, and 5 hours 45 minutes  of tomography for sets 1 and 2 respectively. While  the Imaging process by tomography may degrade the  performances of ICs, it seems that counterfeit ICs can  be detected without failing the device.


 Some parameters and devices were not impacted  much by tomography. The tomography process did  not corrupt the read and write operation of either  flash memory. It also has little impact on the  switching characteristics of the FPGAs.


 New technology devices are friendlier to the  tomography imaging process. Electrical  characteristics of 150 nm Macronix flash memory, 90  nm and 45 nm FPGAs used in this work did not  change by much. Hence, it may be safe to perform  tomography on new chips. However, we stress that  more experimentation should be performed on many  different chips of different technologies, especially  regarding the time-to-failure between exposed and  unexposed devices.


Future Work


Silicon based integrated circuits are vulnerable to low energy  x-rays. X-ray filter is used to remove that undesirable part of  the x-ray spectrum. Thus, the choice of appropriate filter is  important in x-ray tomography to get good image with  minimum damage of IC. The vulnerability of integrated  circuits in terms of x-ray filter materials will be investigated in  author’s future research.


In this experiment, sets of applied voltage (KV) and power  were applied to control the amount of dose absorbed by IC. Along with filtration and energy the absorbed dose also varies  with source-to-sample distance and beam current. Future  research based on these parameters will be carried out.


In this work we presented the impact of X-ray tomography on  two different types of ICs. Our results suggest that the FPGAs  are more resilient to TID effect and there is not much change


in the monitored parameter up to the ﬁrst 2 hours of


tomography cycle. However, we observed some degradation in  the erase speed of the ﬂash memories even with 60 kV source  power after 2 hours of tomography. With the scaling of the  devices this effect is reducing in both cases. It is clearly unsafe  to use X-ray tomography for old technology devices. Although  there is little observable impact on new technology devices  from our experiments, the overall reliability and time-to-failure  should also be investigated in future work.


The authors would like to acknowledge the support from  National Science Foundation (grants CCF-1423282).


K. A. M. Ahmood, P. E. L. A. C. Armona, S. I. N. A. S. Hahbazmohamadi, F. I. P. La, and B. A. J. Avidi, “Real-time  automated counterfeit integrated circuit detection using xray microscopy,” Appl. Opt., vol. 54, no. 13, pp. D25–D32,


2015.


S. Shahbazmohamadi, D. Forte, and M. Tehranipoor,


“Advanced Physical Inspection Methods for Counterfeit IC  Detection,” in 40th International Symposium for Testing  and Failure Analysis, 2014, pp. 55–64.


S. Bord, A. Clement, J. C. Lecomte, and J. C. Marmeggi, “An X-ray tomography facility for I.C. industry at  STMicroelectronics Grenoble,” Microelectron. Eng., vol. 61–62, pp. 1069–1075, 2002.


U. Guin, D. DiMase, and M. Tehranipoor, “A


Comprehensive Framework for Counterfeit Defect Coverage  Analysis and Detection Assessment,” J. Electron. Test., vol. 30, no. 1, pp. 25–40, Jan. 2014.


M. M. Tehranipoor, U. Guin, and D. Forte, “Counterfeit  Integrated Circuits: Detection and Avoidance,” Springer, 2015, pp. 133–151.


H. J. Barnaby, “Total-ionizing-dose effects in modern  CMOS technologies,” IEEE Trans. Nucl. Sci., vol. 53, no. 6, pp. 3103–3121, 2006.


P. V. Ma, T.P. and Dressendorfer, “Ionizing Radiation  Effects in MOS Devices and Circuits,” in John Wiley & Sons, 1989, pp. 35–43.


M. Bagatin, G. Cellere, S. Gerardin, A. Paccagnella, A.


Visconti, and S. Beltrami, “TID sensitivity of NAND Flash  memory building blocks,” IEEE Trans. Nucl. Sci., vol. 56, no. 4, pp. 1909–1913, 2009.


D. M. Fleetwood, P. S. Winokur, and J. R. Schwank, “Using  laboratory X-ray and Cobalt-60 irradiations to predict  CMOS device response in strategic and space  environments,” IEEE Trans. Nucl. Sci., vol. 35, no. 6 pt 1, pp. 1497–1505, 1988.


[10] X. Yao, N. Hindman, L. T. Clark, K. E. Holbert, D. R. Alexander, and W. M. Shedd, “The impact of total ionizing  dose on unhardened SRAM cell margins,” IEEE Trans. Nucl. Sci., vol. 55, no. 6, pp. 3280–3287, 2008.


[11] G. Cellere, A. Paccagnella, A. Visconti, M. Bonanomi, S. Beltrami, J. R. Schwank, M. R. Shaneyfelt, and P. Paillet, “Total ionizing dose effects in NOR and NAND flash  memories,” IEEE Trans. Nucl. Sci., vol. 54, no. 4, pp. 1066–1070, 2007.


[12] T. R. Oldham and F. B. McLean, “Total ionizing dose  effects in MOS oxides and devices,” IEEE Trans. Nucl. Sci., vol. 50, no. 3, pp. 483–499, Jun. 2003.


[13] L. Tsetseris, R. D. Schrimpf, D. M. Fleetwood, R. L. Pease, and S. T. Pantelides, “Common origin for enhanced lowdose-rate sensitivity and bias temperature instability under  negative bias,” IEEE Trans. Nucl. Sci., vol. 52, no. 6, pp. 2265–2271, Dec. 2005.


[14] M. Bagatin, G. Cellere, S. Gerardin, A. Paccagnella, A. Visconti, and S. Beltrami, “TID Sensitivity of NAND Flash  Memory Building Blocks,” IEEE Trans. Nucl. Sci., vol. 56, no. 4, pp. 1909–1913, Aug. 2009.


[15] D. N. Nguyen, S. M. Guertin, G. M. Swift, and A. H. Johnston, “Radiation effects on advanced flash memories,” IEEE Trans. Nucl. Sci., vol. 46, no. 6, pp. 1744–1750, 1999.


[16] S. Gerardin and A. Paccagnella, “Present and Future NonVolatile Memories for Space,” IEEE Trans. Nucl. Sci., vol. 57, no. 6, pp. 3016–3039, Dec. 2010.


[17] T. R. Oldham, R. L. Ladbury, M. Friendlich, H. S. Kim, M. D. Berg, T. L. Irwin, C. Seidleck, and K. A. LaBel, “SEE  and TID Characterization of an Advanced Commercial  2Gbit NAND Flash Nonvolatile Memory,” IEEE Trans. Nucl. Sci., vol. 53, no. 6, pp. 3217–3222, Dec. 2006.


[18] G. Palumbo and D. Pappalardo, “Charge Pump Circuits: An  Overview on Design Strategies and Topologies,” IEEE  Circuits Syst. Mag., vol. 10, no. 1, pp. 31–45, 2010.


[19] Quadir S.E and Chen J. and Forte D. and Asadizanjani N. and Shahbazmohamadi S. and Wang L. and Chandy J. and  Tehranipoor M., “A survey on chip to system reverse  engineering,” ACM J. Emerg. Technol. copmuting Syst. (accepted for Publication), 2015.


[20] Asadizanjani N. and Shahbazmohamadi S. and Jordan E.H., “Investigation of Surface Geometry Change in Thermal  Barrier Coatings Using Computed X-ray Tomography,” Dev. Strateg. Mater. Comput. Des. V Ceram. Eng. Sci. Proc., vol. 35, no. 8, 2015.


[21] K. Xiao, X. Zhang, and M. Tehranipoor, “A Clock  Sweeping Technique for Detecting Hardware Trojans  Impacting Circuits Delay,” IEEE Des. Test Comput., vol. 30, no. 2, pp. 26–34, 2013.


[22] P. Canet, V. Bouquet, F. Lalande, J. Devin, and B. Leconte, “Fowler-nordheim erasing time prediction in flash memory,” in Symposium Non-Volatile Memory Technology 2005., pp. 15–18.


[23] P. Cappelletti, C. Golla, P. Olivo, and E. Zanoni, Flash  Memories, Springer, 1999.


Non-destructive PCB Reverse Engineering Using   X-ray Micro Computed Tomography


Navid Asadizanjani1, Sina Shahbazmohamadi2, Mark Tehranipoor1 and Domenic Forte1  1Electrical and Computer Engineering Department, University of Florida


2Mechanical Engineering Department, Manhattan College


Reverse engineering of electronics systems is performed for  various reasons ranging from honest ones such as failure  analysis, fault isolation, trustworthiness verification, obsolescence management, etc. to dishonest ones such as  cloning, counterfeiting, identification of vulnerabilities, development of attacks, etc. Regardless of the goal, it is  imperative that the research community understands the  requirements, complexities, and limitations of reverse  engineering. Until recently, the reverse engineering was  considered as destructive, time consuming, and prohibitively  expensive, thereby restricting its application to a few remote  cases. However, the advents of advanced characterization and  imaging tools and software have counteracted this point of  view. In this paper, we show how X-ray micro-tomography  imaging can be combined with advanced 3D image processing  and analysis to facilitate the automation of reverse  engineering, and thereby lowering the associated time and  cost. In this paper, we demonstrate our proposed process on  two different printed circuit boards (PCBs).  The first PCB is  a four-layer custom designed board while the latter is a more  complex commercial system. Lessons learned from this effort  can be used to both develop advanced countermeasures and  establish a more efficient workflow for instances where  reverse engineering is deemed necessary.


Keywords: Printed circuit boards, non-destructive  imaging, X-ray tomography, reverse engineering.


Reverse engineering is a process where the goal is to  reproduce, duplicate, or enhance chips and systems based on  the study of an original object/system. For electronic systems, reverse engineering (RE) could be performed at chip, board, and system levels. Since such electronics typically consist of  multiple layers, reverse engineering involves obtaining the  internal structure and connections of all layers through either  a destructive process of delayering or non-destructive  processes. In a destructive process, delayering is followed  with imaging of every layer before the next round of material  removal. On the other hand, a non-destructive process consists  of imaging tomography, which can be used to image the whole  system or board without delayering. In either case, the  analysis can be automated or manual and ultimately results in  a netlist [1] that can be used to reproduce the system.


Reverse engineering can be performed by groups with


“honest” intentions or “dishonest” intentions. “Honest”


intentions include verification of a design for the purposes of  quality control, fault and failure analysis, analysis of the  features of a competitor’s product, counterfeit detection, Trojan detection, confirmation of intellectual property, approved redesign of an obsolete product, and education


[2][16][17]. In many countries, reverse engineering is even  legal as long as patents and design copyrights are not violated


[3]. When reverse engineering is performed with the intention  of performing cloning, piracy, Trojan insertion, or  counterfeiting, the intention is “dishonest”. If RE results in a  working copy of the system, it is called a cloning attempt [4]. “Dishonest” parties could sell large amounts of cloned or  counterfeit products without incurring the same development  costs as the IP owner [5]. Beyond cloning, RE of electronic  systems could also become a major motivation for Trojan  insertion. Since a dishonest party is cloning an electronic  system, he/she will have the capability of adding malicious  circuitries or firmware to the system as well.


Figure 1: (a) Four layer custom board, (b) Commercial  Xilinx Spartan-6 starter board.


In this paper, we focus on board-level reverse engineering  since a printed circuit board (PCB) is the fundamental  component of any electronic system. A PCB is a laminated  non-conductive material that connects electronic components  via conductive copper traces. Electronic components and  chips are mounted on the board and are electrically  interconnected with these traces. The board might be single or  multi- layered depending on the complexity of the system. A  RE team could analyze the outer layers of an authentic board  to find the components mounted on it, its traces, and its ports. After that, they could delayer the multi-layered board to reveal  the connectivity, traces, and vias within its internal layers.


We use a Zeiss Versa 510 X-ray machine to demonstrate how  easy it is today to perform RE on PCBs with suitable  equipment and expertise. Our process is both fast (4.23


scan/hour) and partially non-destructive. Although we might  need to remove the components from the board to reduce the  noise level in the images, comparing with traditional  destructive methods where serial sectioning had to be done, this method can be considered as one that is faster and easily  repeatable. In other words, it is more amenable to automation  from start to finish. We illustrate our technique on a small  custom PCB first (see Fig. 1 (a)) as a proof of concept. Next, the same scanning process is applied to a 6 layer commercial  Xilinx Spartan-6 starter board as shown in Fig. 1(b). The  entire process consists of optimizing parameters for X-ray, performing X-ray imaging, and performing image processing. These steps are discussed in detail along with the results and  potential countermeasures in the remainder of the paper.


X-ray source


Transmission value


Detector


Energy


( Must be


Objective


X-ray Imaging


maintained


between 20-35%)


Tomography is a non-invasive imaging technique that makes


Position of


it possible to visualize the internal structure of an object


source and


without interference of over- and under-layer structures. In


X-ray counts


X-ray Filter


this paper, micro X-ray computed tomography is performed


(Must be


using the Zeiss Versa 510, which has a maximum power of


maintained above


160 KV for its source, to acquire the structural information of  different PCBs. X-ray tomography gives us the opportunity to


5000 and below


extract the geometrical information of traces, via holes and


geometry


60000)


Exposure time


connections on PCB layers. Note that all PCB layers (front, back, and internal) be captured in a single imaging session.


Optimizing Image Acquisition Parameters


The principle of tomography is to acquire a stack of two  dimensional (2D) images and then use mathematical  algorithms such as direct Fourier transform and center slice  theory [6] to reconstruct the three dimensional (3D) image. These 2D projections are collected from many different angles  depending on the quality needed for the final image. The  object properties, such as its dimension and material density, are important to consider in selection of the tomography  process parameters which include:


 Source power: correlated to the X-ray energy and amount  of penetration


1) Flash Memory: NOR type parallel ﬂash memories from  Intel (28F400B5) and Macronix (MX29F400C) with different  process technology of 400 nm and 150 nm respectively have  been used in this work. Experiments were performed on a total  of 12 flash memories, 8 of them are from Intel (28F400B5) and the rest are from Macronix (MX29F400C). Since Intel (28F400B5) flash memory is obsolete, there are many  counterfeits in the market. Therefore, Intel flash memories are  good candidate for our experiment. On the contrary, Macronix  flash memory is parallel NOR type flash memory like Intel


Flash but it has relatively newer process technology. That  allows us to compare the impact of X-Ray tomography on  flash memories with different process technologies. We have  done X-ray tomography using the X-ray device described in  earlier section on ﬂash memories using 60 kV, 80 kV, 100 kV  and 120 kV source voltages. We divided 8 Intel (28F400B5) samples into two sets, Set-1 and Set-2. Set-1 contains samples  1, 2, 3, and 4 while Set-2 contains samples 5, 6, 7, and 8. We  used 60 kV for Samples 1 and 5, 80 kV for Samples 2 and 6, 100 kV for Samples 3 and 7, and 120 kV for Samples 4 and 8. We formed a single set of 4 samples of Macronix (MX29F400C) flash for each of the source voltages. The  tomography was applied in the following time increments for  each ﬂash memory: 15 minutes, 30 minutes, 1 hour, 2 hours  and it continued with an additional 2 hours of tomography  until the devices failed to complete any of the basic operations (read, program, or erase).


For testing the flash memories after each tomography cycle, a  setup was created deploying a Digilent Atlys Board, which  includes a Xilinx Spartan 6 FPGA. A flash memory controller  was written in VHDL to control the basic operations of the  flash memory and perform the required tests. The operations  that the controller can handle are read, program and chip  erase operations. Read and program operations are in byte  mode. In addition to the basic operations, erase timing is also  measured using the controller. Along with the memory  controller, a UART module is used to send the read data to a  PC for analysis. The read margin of the flash memories was  also measured using a clock sweeping method [21]. Clock  sweeping involves applying a pattern at different clock  frequencies from a lower speed to higher speeds. Some paths  sensitized by the pattern which are longer than the current  clock period start to fail when the clock speed increases. The  obtained start-to-fail clock frequency can indicate the delays of  the paths sensitized by the patterns.


The test procedure for flash memories is shown in Fig. 5(a). The procedure was repeated for each tomography time period (15 minutes, 30 minutes, and so forth) and it can be described  as follows:


1. Program the ﬂash memory (i.e., change the data  stored in each cell to ‘0’) and perform the  tomography for the speciﬁed time.


2. Execute a read operation on whole chip after  tomography. If there are any bit ﬂips from ‘0’ to ‘1’, record the number and store the associated locations.


3. Apply an erase operation on whole chip (i.e., change  the data stored in each cell to ‘1’) and then a read  operation to detect any ‘1’ to ‘0’ transition failures.


4. Program the entire memory again and repeat steps 2  and 3 to determine whether any failures are  permanent or temporary. This process is repeated for  10 times.


5. Measure the erase time to obtain any deviation from  the initial value.


6. Employ clock sweeping on read operation and record  read margin information.


The Intel ﬂash memory (28F400B5) has a pin for


erase/program voltage. Either 5V or 12V can be applied to the  pin. If 5V is applied, an internal charge pump boosts the  voltage to the appropriate erase/program voltage. If the pin is  driven with 12V, this voltage is given to the ﬂash cells with an  internal voltage control unit. In some steps of the test, we used  12V to see if the failure is due to charge pump or not. In  contrast, Macronix (MX29F400C) is a single voltage flash. It  needs 5V to read, program and erase operation and always  uses an internal charge pump to boost the supply voltage to a  higher voltage.


2) FPGAs: We have investigated the effects of X-ray for two  different types of FPGA families: Xilinx Spartan 3 (Digilent  Spartan-3 Starter Board) and Spartan 6 (Digilent Atlys Board). The technologies of these two FPGAs are 90 nm and 45 nm  respectively. The boards contain different components other  than FPGAs, so a custom holder was designed to hold both  board types, one at a time during tomography. In addition, by  using a lead sheet, we shielded the cage to protect other parts  of the boards from irradiation effects. Hence, only the FPGA  chip on the board was exposed to X-ray and we could fairly  evaluate the effect of X-ray on FPGAs. In FPGA experiments, we started our tests with low energy power, but according to  the small changes seen in the electronic test results we decided  to conduct tests using just high energy power (120kV) for all  the reporting tests.


FPGAs are difﬁcult to test in the sense that there are billions of  possible logic functions that can be implemented. Thus it is not  possible to test all the functional blocks in an FPGA. In  addition, in counterfeit IC detection, X-ray is used when the IC  is unbiased. So, the effect of X-ray is limited to total ionizing  dose (TID), which mainly affects the threshold voltage of  CMOS transistors and their switching speeds. Therefore, in  our tests, we focused on observing the change in the speed of  the FPGA. Speciﬁcally, ring oscillators (ROs) were placed into  the FPGA and measured to get the delay information of the  FPGA Conﬁgurable Logic Blocks (CLBs). CLBs might have  different number of logic primitives and Look-up Tables (LUTs) depending on the device family. In Spartan 3, each  CLB contains 8 Look-up Tables (LUTs), so we placed 7-stage  RO to each CLB and covered every CLB. In Spartan 6, because the CLBs have 16 LUTs, 15-stage ROs were created  which covered almost all the CLBs in the FPGA. We created  hardmacros for RO designs to make sure that internal routing  of each RO in every part of the FPGA was exactly same.


The FPGA tests procedure is illustrated in Fig. 5(b) and can be  described in the following steps:


1. All the RO frequencies were measured before X-ray  tomography.


2. Tomography was performed for the predeﬁned period  of time.


3. The frequency of each RO in the FPGA was  measured after the tomography and stored in a PC.


4. Deviations from the initial measurement for each RO  were calculated according to the following equation:


 fi ,tn 100  (


)                                     (3)


where, fi,to is the initial frequency of ith RO in the  FPGA, and fi,tn is the frequency of the ith RO after  the nth tomography cycle. Finally, fi,tn is the  percentage deviation from the initial frequency for  the ith RO at time tn. Positive and negative fi,tn  denote RO speed-up and slow-down respectively.


The above steps were repeated for additional rounds of  tomography on both FPGAs. The frequency of each ring  oscillator was measured 10 times in every step. Each  frequency value is the average of these 10 measurements. There were 1728 and 1476 ROs in Spartan 3 and Spartan 6  FPGAs respectively. The frequency of each FPGA is  calculated by averaging the frequency of all the ring oscillators  placed in that FPGA.


A. Flash Memory Results


Using the devices and the setup described in experimental  setup and test procedure section, the tomography and test  cycles were executed. In this section, we summarize our results  from each tomography cycle. After ﬁnishing all the  tomography cycles for both Intel (28F400B5) and Macronix (MX29F400C), the following operations and parameters were  unaffected. First, we did not observe any bit ﬂips in any  tomography cycle in any sample. This can be explained by the  fact that the difference between erased state and programmed  state threshold values of the ﬂash memory cells are large  enough to prevent being ﬂipped by X-ray high energy photons. Second, there was no change in the read margin of any sample  after applying the clock sweeping on read operation. This  suggests that the read operation was not affected from  tomography in these speciﬁc ﬂash memories.


1. Intel Flash: We found that several parameters degraded for  the Intel flash (older technology). First, the chip erase time  increased exponentially with the exposure time of tomography. Figure 6 and 7 show the change in the erase time for Set-1 and  Set-2 respectively. In the ﬁgures, the x-axis represents the  exposure cycles and y axis corresponds to erase time. As  shown in Fig. 6, sample 1 exposed by 60KV did not fail to  perform any of the operations after 7 hours and 45 minutes of  tomography in total. However, erase time increased by one  order of magnitude. Other samples failed in different cycles. For example, samples 2 and 3 which are exposed by 80 and  100KV source failed to erase and write after the third 2 hours  of tomography. As one would expect, higher source power had  larger effect on the devices. Hence, 120 kV caused the Sample  4 to fail earlier than others. Sample 4 failed to erase one of the  main blocks in the ﬁrst 2 hours tomography cycle, but this  failure was temporary. After erasing with external 12V (see  Section 3.B.1), it recovered and then operated normally.


However, after another 2 hours of tomography it failed to erase


f i , tn fi ,to


and write whether 5V or 12V was applied to it.


fi ,to


It can be seen from Fig. 7 that the second set of samples also  follow very similar trends. Sample 8 failed earlier than others  due to higher source power 120KV as expected. Similar to  Set-1, samples 6 (80KV) and sample 7 (100KV) failed later  than sample 8. Sample 5, which was only exposed to 60 kV


did not fail at all similar to ﬁrst set. There were only two major


differences to report between the two sets. The devices in the  second set lasted 2 hours more compared their counterparts in  the ﬁrst set. In addition, the erase time of sample 5 increased  less than that of the sample 1 which was exposed to same  source power.


2. Macronix Flash: Erase time of a newer technology (0.15m) Macronix (MX29F400C) flash after X-ray  tomography is shown in Fig. 8. Here, the erase time varied  very little over 7 hours and 45 minutes of tomography. Even  120KV source power could not make a significant impact on  erase time.


Figure 7: Change in the erase time due to X-ray tomography  for Set-2 Intel ﬂash memories.


Figure 6: Change in the erase time due to X-ray tomography


for Set-1 Intel ﬂash memories.


Figure 8: Change in the erase time due to X-ray tomography  for Macronix ﬂash memories.


 Detector objective: determines the field of view and  resolution range


 Filtering: controls the dose which allows higher energy  X-rays to penetrate


 Distance of source and detector from sample: inversely  proportional to number of counts


 Number of X-ray projections: identifies the angular  increment for each rotation for sample during  tomography


 Exposure Time: linearly related to counts and determines  the total time and, consequently, the cost of scanning.


These parameters can affect the pixel size and signal-to-noise  ratio, which must be optimized based on the region-of165


interest. Internal and external structure can be analyzed when  the 3D image is reconstructed, which needs center shift and  beam hardening tuning. [7].


Trade-off between Pixel Size and X-ray Counts


The most critical parameter for defining the quality of 3D  reconstructed images is the pixel size. Based on it, many other  parameters such as distance of source and detector from the  sample (geometric magnification) and detector objective (similar to optical magnification) will be tuned.


Figure 2: a) Effecting parameters on X-ray imaging b) Xray counts relation with respect to the distance between  source and detector


To use both magnifications effectively, one has to optimize all  the parameters simultaneously. Thanks to a near-ideal point  source used in the cited system, we are given the opportunity  to move the detector and source towards or away from one  another to change the pixel size while still maintaining the  resolution. Geometrical magnification can help to decrease  pixel size by a factor of 10 in addition to the magnification  offered by the detector which is yet another option to be tuned.


Normalized Distance between source and  detector


Combining the two magnification types, one can choose any  value between 0.3 to 62 microns for the pixel size. Each  detector in turn has a specific number of pixels (an array of  about 1000 by 1000) which defines the field of view for  imaging. However, there is a trade-off. Smaller pixel size  demands the detector to be positioned relatively far from the  source, thus reducing the number of X-ray counts detected by  the detector. Based on the principles of wave propagation, wave power is inversely proportional to square of distance  from wave source. In order to get a clear image, one has to  obtain 2D projections with more than 5000 X-ray counts. Therefore, to maintain such X-ray count values, the exposure  time and total scanning time must be increased.  In addition, the window size decreases with smaller pixel size.


The same concept applies here. The diagram in Fig. 2(a), shows the effecting items on the imaging parameters and Fig. 2(b) shows the relation between the measured detector  distance and X-ray counts as it moves back. The values for  distance and X-ray counts are normalized based on the  maximum value for each to better show the dependent  behavior of these two parameters.


A four layer custom board is first used as a proof of concept  for our tomography on PCBs and then the same process will  be used to do reverse engineering on a commercial Xilinx  Spartan-6 starter board. Both PCBs are shown in Fig. 1(a) and  Fig. 1(b) respectively.


To make sure that we can see our features on the board, we  have selected a fine pixel size which gives us enough image  quality. After several rounds of optimization for tomography  parameters the values presented in Table I are selected. Tomography window size has a direct relation with the pixel  size. The detectors on Versa 510 are an array of 1000 by 1000  pixels. This will give us an area of about 5 by 5 cm for each  tomography set with the parameters in Table I. In order to do  a complete tomography on the custom board (10 by 15 cm) in  one session, a raster scan is performed on 6 different areas to  cover the entire board. The process is completely automated  after setting the parameters, and can be performed without the  need for oversight. Note that the same process and a very  similar set of parameters should be widely applicable to most  PCBs.


Custom Board Tomography


For the four layer custom board (Fig. 1(a)), all traces, connections, and via holes are clearly captured. In order to  check the effectiveness of the tomography the results are  compared with the board design files previously used to print


it. The board includes a front side, backside, and two internal  layers. The internal layers correspond to power and ground. The via holes are connecting the traces on two sides of the  board and are also connected to either power or ground layers. This is presented in the design layout in Fig. 3.


Table I. X-ray Tomography Parameters for PCB


Tomography parameters Scan  Pixel size (µm)


49.2


Window size (µm)


49520


4X


Source distance (mm)


204.2


Detector distance (mm)


80.1


Exposure time (s)


1.2-7.2


Number of projections


3201  Total tomography time (hr) 4.23


The 3D image of the board is reconstructed using a  combination of thousands of virtual 2D slices. These slices  can be viewed and analyzed separately. The thickness of each  of them is same as the pixel size (approximately 50 micron). In Fig. 4, one slice is demonstrated which shows the  information of the internal power layer. Obviously, a better  resolution or smaller pixel size will give us better image  quality which can result in an easier image processing effort. However, one also has to consider that a better image will  increase the costly X-ray scanning time and data size. These  two parameters are considered as the controlling factors for  the final PCB reverse engineering process.


Comparing the tomography results and the design layout of  the board (in Figs. 3 and 4), one can see a clear difference  between the via holes that are connected and those which are  not connected to the internal layer. The soldering material, which provides connection of the via holes has high density  and results in white contrast for the pixels. On the other hand, when there is no soldering material and no connection the  isolating material between the via hole and the layer has lower  density and results in dark contrast for the pixels. The same  principle will let us detect the traces on the side layers of the  board due to the attendance of copper on the traces as is shown  in Fig. 5.


Xilinx Commercial Board Tomography


The imaging process described above clarifies the accuracy of  non-destructive X-ray imaging to acquire structural  information of a PCB. In the next step a commercial PCB, Xilinx Spartan 6 is chosen to be scanned and reverse  engineered. This a 6 layer PCB with a complicated map of


Figure 3: Layout of an internal layer.


Figure 4: Virtual slicing of internal layer. Figure 5: Reconstructed (a) top and (b) bottom layers


traces and joint connections on different layers. The same  tomography parameters have been used for this PC. In our first  imaging attempt, the board was scanned with all the  components mounted on it. Most of the components such as  resistors, plastic switches and ports are low Z material in the  periodic table which does not cause any effect during the  scanning process. However, there were also some of the  components such as the soldering material and the metal ports  which created artifacts in the reconstructed images. These  effects appear as noise in the image, which can make it  difficult to set up an automated reconstruction process. In  order to solve this problem, we detached the components from  the board using a hot air gun. The soldering material will also  be melted down during this process. Then, imaging was  performed again with improved results.


Image Stitching and Total Board  Reconstruction


The entire width and length of a PCB board is much larger  than the field of view of a single tomography.  Yet, multiple  imaging sessions not only increases the time and cost  associated with imaging, but also creates errors associated  with mounting and alignment. In our approach, X-ray imaging  was done in one session as follows. Coordinates of each  scanning region were preprogrammed and the scanning was  then performed at each region of the board in order. At the  end, the data from each region was stitched together to form  the complete PCB.


Firstly, in order to ensure enough information is available for  alignment, scanning was performed with 15-20% overlap  between neighboring areas. This portion was then used to  align surfaces together. The alignment process is based on  Iterative Closest Point (ICP) algorithm [15].  This algorithm  operates in the following iterative fashion:


1. Corresponding points in the neighboring scans are  associated together based on the nearest neighbor criteria.


2. A transformation is estimated to minimize the mean  square distance between the reference point cloud and the  target one.


3. This transformation function (combination of translation  and rotation) will be iteratively revised to best match the  target cloud to the reference.


4. As a result of the previous step, there may still be some  artifacts as a result of different histograms for each scan  having different global minima and maxima. Some of the  parameters, such as room temperature, accuracy of source  power, etc., can cause the contrast or histogram changes  during the tomography on different areas. For example, since the tomography is automated and will be run  through the day and night, the temperature in the room  will change accordingly. The contrast for every image has  to be adjusted based on the other one during the stitching


process. This will help to get a similar histogram for the  images for each and every separate scan. A scaling  process is then applied on all the areas by imposing a  global minimum and maximum intensity value for the  entire data set. These values are obtained by choosing the  smallest minimum and largest maximum value among all  stitched scans.


Image Segmentation


Although reconstructed 3D images contain valuable  information, they cannot be used directly for fabrication or  elaborate quantified inspection. A series of image processing  steps are necessary to transform the image to a computeraided design (CAD) system file which is a prerequisite for  fabrication. In particular, to print circuits on the board, Gerber  files are generated for each layer which are 2D binary CAD  files containing geometric information.


The most critical step for the transition from a 3D X-ray image  to a Gerber file, is image segmentation, that is assigning labels  to each pixel ( or in the case of 3D, each voxel) to extract point  cloud (x, y, z) information. Efforts have been made in the past  to perform image processing on images of PCBs for the  purpose of inspection or reverse engineering of PCBs. [8-10]. In [8], defect characterization in PCBs have been achieved  using subtraction and elimination process. The technique is  limited to simple defects and physical fixtures are used for  alignment purposes. In [9], series of morphological operations  such as erosion, dilation, etc. are utilized for segmentation but  lacks automation and after the proposed process the images  are not converted to CAD files for recreation.  C. Koutsougeras et al. [10] applied an automatic Verilog HDL  Model Generator, which includes 2D image processing  technique that is used to identify the components and their  connections at much lower resolution and lacks information  of the internal layers.


Here we propose an automated step-by-step algorithm (shown  in Fig. 6) which can be utilized for any 3D data of the boards  regardless of the imaging modality, board feature complexity, and number of layers.


Figure 6.  Image processing algorithm


Image  Sampling


•Data Size reducation of factor of  8 using  binning of 2


Image  Filtering


•Obtaining gradient of the image for edge  detection and smoothing


Image  Labeling


•Assigning values to pixels belonging to  vias and traces


The first step, image sampling, is deemed critical when the  data size is relatively large as in this case with X-ray  tomography data. For instance, the complete data set of the  Xilinx board has a file size exceeding 60 GB. Sampling  shrinks the dimensions of the original image grid by merging  neighboring pixels. Though images may lose sharpness, using  a binning of 2 can reduce the file size by a factor 23=8 which  make the data more manageable for further processing. This  process has only been used if the consequent blurring of the  image doesn’t make accurate segmentation impossible.


Figure 7. Image binning 2 (a) and 4 (b)


Fig. 7 shows the effect of binning on the quality of data for  extraction information on vias and traces. Fig. 7(a) is image  with binning 2 where traces and vias are still kept at very high  quality for feature extraction. On the other binning 4, shown  in Fig. 7(b) clearly shows loss of clear ages and pixilation of  the image.


Figure 8. X-ray images (a) before and after (b)


application of 3D Sobel operator


The next step is filtering the images to remove different  inevitable artifacts in the 3D data. For example, due to the  presence of materials with radically different X-ray absorption  coefficients there are several location with saturated  illumination (as illustrated in Fig. 8 (a)) Also, as the X-ray  penetrates through the sample, it loses some of its energy. This


phenomenon is known as beam hardening. Beam hardening  can insert false image contrast within a same material making  the process of labeling difficult. We have used a Sobel  Algorithm to highlight the edges corresponding to traces and  vias while smoothing the rest of the image. The Sobel-Filter  is an edge detection filter which estimates the gradient of an  image using central difference. It convolutes the image with a  3 by 3 by 3 kernel (equations 1a and 1b) in all proper  directions.


[


−1 −3 −1


−3 −6 −3−1 −3 −1


] , [


0 0 0 0 0 0 0 0 0


1 3 1 3 6 3 1 3 1


]


Eq. 1a


X-1


X+1


        =


  (   + 1) −   (   − 1)2


Eq. 1b


Note that the kernel in X direction has been provided above as  an example. The Y and Z kernels can be simply obtained by  rotating the kernel in the appropriate direction.


The filtered images are finally ready to be labeled. There are  different techniques that can be used to segment/label  including TopHat [11], watershed, thresholding [12-13], and  several others [14].  Simple binary thresholding merely  replaces each pixel on an image with a 0 or 1 (black or white) depending on the logical operation on the intensity of the  image (i.e., if intensity < predefined threshold replace with 0, else replace with 1.) However, this simple method cannot be  used for the 3D data of the boards as locations belonging to  traces and via have different image intensity at different  location of the image. This issue is further compounded by  stitching, which adds more segments to the image with  different intensity values of the same material. Therefore, we  have used localized thresholding where image is broken into  different segments which are not overlapped. In each segment, a limited range of the histogram will be selected locally. This  will be according to the pixels contrast of the via and traces. Once the histogram range is selected, only the trace and via  will be selected from the image when a brushing tool paints  the pixel (assign values to pixels) as it scans all over the  image.


Fig. 9 shows the outcome of the process on all layers of the  board. Although some of the details are not clear in the  presented figures, this is due to limitations of image quality as  a snap shot from a CAD file and to stay in the size limit of the  total file size. The original CAD files indeed present all the  details as one zooms in.


Layer 1


Layer 2


Layer 3


Layer 4


Layer 5


Layer 6


Figure 9.  Segmented layout (point cluster) of six layers of PCB.


Lessons Learned to Develop Countermeasures


The proposed approach can significantly reduce the time, cost, and manual effort associated with reverse engineering. Though further efforts have to be made to duplicate  functionality (firmware and software), the described method  provides us with the entire geometry and 3D internal structure. Although very beneficial for honest reverse engineering  obsolete designs where data sheets are no longer available, the  portability of this technique is alarming. Here are the lessons  learned from this research:


1. Non-destructive and fast imaging of multi-layered PCB  systems are possible using X-ray computed tomography.


2. Although X-ray can penetrate through most materials  used in PCB systems, there is always a challenge in  feature recognition once a low density material is located  next to high density material.


3. X-ray is in fact the emission of high energy photons. Although one has to note in case electrical components  are on the board during the tomography, long X-ray  exposure might cause damage or ionization on some of  the chips. This can be also used as an external source to  harvest energy to create a countermeasure structure.


We introduce concepts from the lessons learned above, to  prevent reverse engineering in critical applications.


The first class of countermeasures is application of X-ray  sensors that can react to X-ray exposure. This class of  countermeasures have two subcategories of indirect and direct  methods.


1) Indirect: Materials such Zinc sulfide are sensitive to Xray and emit light upon exposure to X-ray or electron  beam. Light sensitive films can also detect the light and  generate current in very small scale values. Using the  combination of Zinc sulfide and photodiode, one can  implement an X-ray sensor in the system to store the  history of the devices exposure to high energy X-ray  photons and/or react destructively when the exposure  exceeds a certain limit. This allows for limited X-ray  inspection as a common practice for authentication, but  negates the chance of thorough reconstruction.


2) Direct: In direct mode, X-ray photons are directly  converted to electrical charge which can be used to alter  information in the device. These type of sensors are  fabricated from solid state material such as silicon [18]. The amount of exposure and the X-ray power defines the  output of the sensor. Depending on the amount of energy  harvested from the sensor, one can use that to store  exposure information in the device or use it as an antireverse engineering sensor as stated above.


Although sensors will help to see whether or not the device  has been attacked, they may not prevent the entire information  piracy. The second class of countermeasures addresses this  issue through materials that have excessively large X-ray  attenuating coefficient. X-ray can penetrate easily through the


general PCB material and create clear 3D images with high  signal-to-noise-ratio. Adding high density material such as  Zirconia powder, which has a very high X-ray attenuation  coefficient, will reduce the X-ray transmission amount  through PCB and will result in much lower signal-to-noiseratio. This can be used in a specific pattern in between several  layers. Thus, indeterminate information will make the  transition to a CAD file almost entirely impossible.


Conclusion and Future Work


In this paper, we have presented non-destructive reverse  engineering by x-ray imaging of a simple, custom PCB and  another, more complex commercial Xilinx Spartan-6 starter  board. The netlist of components and connections were  extracted as a point cluster with xyz information from the  images using advanced image processing techniques. These  type of files can be directly converted to DXF or GERBER  files which are compatible with circuit printing machines. We  will continue the study to develop a software where the X-ray  images are imported and the final netlist is generated as output  in a completely automated fashion. Since RE could lead to IP  theft, piracy, cloning, etc. of PCB products, we have also  proposed countermeasures which might mitigate the threat of  the proposed technique. We hope that this paper raises  awareness of the current-state-of-the-art techniques and  provides motivation for the development of additional lowcost and robust anti-RE techniques.


[1] R. Torrance and D. James, “The state-of-the-art in ic


reverse engineering,” in Cryptographic Hardware and


Embedded Systems-CHES 2009. Springer, 2009, pp. 363–


381.


[2] C. Bao, D. Forte, and A. Srivastava, “On application of


one-class svm to reverse engineering-based hardware


trojan detection,” in Quality Electronic Design (ISQED),


2014 15th International Symposium on. IEEE, 2014, pp.


47–54.


[3] T. J. Biggerstaff, “Design recovery for maintenance and


reuse,” Computer, vol. 22, no. 7, pp. 36–49, 1989.


[4] S.E Quadir, J. Chen, D. Forte, N. Asadizanjani, S.


Shahbazmohamadi, L. Wang, J. Chandy, M. Tehranipoor,


“A survey on chip to system reverse engineering” ACM


journal on emerging technologies in computing systems


(JETC), 2015.


[5] U. Guin, D. DiMase, and M. Tehranipoor, “Counterfeit


integrated circuits: Detection, avoidance, and the


challenges ahead,” Journal of Electronic Testing, vol. 30,


no. 1, pp. 9–23, 2014.


[6] X. Pan, “Unified reconstruction theory for diffraction


tomography, with consideration of noise control,” JOSA


A, vol. 15, no. 9, pp. 2312–2326, 1998.


[7] N. Asadizanjani, S. Shahbazmohamadi, and E. H. Jordan,


“Investigation of surface geometry change in thermal


barrier coatings using computed x-ray tomography,” in


38th Int’l Conf and Expo on Advanced Ceramics and


Composites, ICACC 2014.


[8] W.-Y. Wu, M.-J. J. Wang, and C.-M. Liu, “Automated


inspection of printed circuit boards through machine


vision,” Computers in industry, vol. 28, no. 2, pp. 103–


111, 1996.


[9] R. C. Mat, S. Azmi, R. Daud, A. N. Zulkifli, and F. K.


Ahmad, “Morphological operation on printed circuit board


(pcb) reverse engineering using matlab.”


[10] C. Koutsougeras, N. Bourbakis, and V. J. Gallardo,


“Reverse engineering of real pcb level design using verilog


hdl,” International Journal of Engineering Intelligent


Systems for Electrical Engineering and Communications,


vol. 10, no. 2, pp. 63–68, 2002.


[11] C. Ting, Q. H. Wu, R. Rahmani-Torkaman, and J.


Hughes. "A pseudo top-hat mathematical morphological


approach to edge detection in dark regions." Pattern


Recognition 35, no. 1, pp.  199-210, 2002.


[12] M. Susanta, and B. Chanda. "Multi-scale morphological


segmentation of gray-scale images." Image Processing,


IEEE Transactions on 12, no. 5, pp. 533-549, 2003.


[13] M. Sonka, H. Vaclav, and R. Boyle. “Image processing,


analysis, and machine vision.” Cengage Learning, 2014.


[14] R. Unnikrishnan, P. Caroline, and M. Hebert. "Toward


objective evaluation of image segmentation


algorithms." Pattern Analysis and Machine Intelligence,


IEEE Transactions on 29, no. 6, pp- 929-944, 2007.


[15] M. Tehranipoor and F. Koushanfar, “A Survey of


Hardware Trojan Taxonomy and Detection,” IEEE Design


and Test, 2010.


[16] Tehranipoor and C. Wang, Introduction to Hardware


Security and Trust, Springer, 2011.


[17] S. I. Parker, C. J. , Kenney, & J. Segal, (1997). 3D—A


proposed new architecture for solid-state radiation


detectors. Nuclear Instruments and Methods in Physics


Research Section A: Accelerators, Spectrometers,


Detectors and Associated Equipment, 395(3), 328-343.


2015 ISTFA Presentation#1: 2010-2015: The Evolving Counterfeit Machine


Thomas Sharpe


SMT Corp, Sandy Hook, Connecticut   tsharpe@smtcorp.com, +1-203-270-4705


This presentation will be chronologically-progressive to my  ISTFA Keynote given in 2010: “Counterfeiters’ Techniques: Constantly Improving to Avoid Detection – National Security  Depends on Us to Keep Up”. Over the 4+ years since that  presentation was given SMT’s labs have watched the  refinement of the counterfeiters craft evolve at a pace  exceeding industries ability to keep up. As quickly as SMT  shared newly-identified counterfeiting methods along with the  test and inspection mitigation processes to reliably detect  them, the counterfeiter seemingly responded within months  with a revised process specifically designed to defeat these  newly published mitigation efforts.


I will share, in detail, the forensic test methodologies utilized  by SMT and ultimately our research breakthroughs which gave  our labs crystal-clear insight into the counterfeiters specific  step-by-step rework process. This clarity allowed us to recreate each process, and in doing so, identify each tell-tale  inspection “red-flag” along the way.


This presentation will include all forensic work utilized in  exposing the “Micro-blast” & “Flat-Lap” counterfeit processes  identified at SMT labs during 2011, as well as unpublished  new process threats and refinements identified in 2013 &


2014. I will also cover the counterfeit mitigation work SMT  supported with the GAO and Senate Armed Services  Committee investigation into counterfeits within DoD supply  chains during the 2011-2012 time period. This presentation  will set the stage for my 2nd presentation on the cloned-device  threats.


Micro-Blasting


With black top coatings (both old and newer varieties) becoming a much more easily detected counterfeit process by  both US-industry quality inspectors and Customs and Border  Protection (CBP) agents, the counterfeiter needed to furtherevolve his craft to processes not requiring blacktop coatings be  utilized to cover their tracks. SMT identified 2 of these newer  processes during 2011. In June of 2011 SMT released our  forensic report to government and the defense/ aerospace  industry on Micro-Blasting.


In this process the counterfeiter utilized a small hand-held  stylus to blow abrasive dust within a controllable compressed  air stream against ink-based part markings on various types of  component surfaces. In this case the process is re-created on a  Plastic Encapsulated Microcircuit (PEM) device. Total time  required to completely remove the part marking was less than  15 seconds.


The high-velocity particle impact of micro-blasting leaves no  directional sanding marks and very little visual evidence  depending on the abrasive medium utilized and amount of time  required to completely obliterate the ink mark.


Figure 1:


Figure 2:


Utilizing Scanning Electron Microscopy (SEM) at 16,000x we  could see artifacts of fine abrasive dust from the milled walnut  shell – a commonly available abrasive utilized for many  industry applications.


Figure 3:


Figure 4:


When the process was applied to a ceramic package the results  were more concerning as the abrasive micro-blast not only  removed the original part marking but also all light scratches  and other cosmetic blemishes leaving the device surface  appearing factory-new. There was also no noticeable edgeprofile degradation which is a common red-flag condition  caused by traditional sanding processes on ceramic devices.


Figure 5:


Again, this entire process took less than 15 seconds to  perform. The most likely abrasive material utilized here is a  finely-milled plastic in a range of specific densities.


Figure 6:


Metal-can packages proved to be equally as concerning since  like ceramic packages, the micro-blast process easily remove  cosmetic blemishes - thus “refreshing” the surface while  simultaneously removing any ink-markings present.


Figure 7:


The abrasive most likely utilized here would have been a 20-50 micron glass-bead type material, which leaves an even,


consistent “fresh” metallic surface behind for counterfeit


remarking.


Figure 8:


Flat-Lapping


In November of 2011 SMT released our forensic report to  government and the defense/ aerospace industry on FlatLapping. Lapping is defined as an abrasive process utilizing a  rotating lap charged with a loose slurry which removes very  small amounts of material from flat metallic or non-mettallic  surfaces. The electronics counterfeiter use lapping is being  performed on both metallic and ceramic top component  surfaces to remove both ink and laser-etch part markings and  logos put on by the Original Component Manufacturers (OCM’s).


The automated lapping process, properly performed, leaves no  directional sanding marks on the component surface and can  only be detected consistently with high magnification digital


microscopy or SEM at 2500-5000x. Luckily however, a lapped  ceramic surface is easy to spot at these magnifications due to  the tell-tale “peanut-brittle” surface charasterisic left behind by  the lapping process.


Figure 9:


The natural ceramic surface of an OCM device not modified  by the lapping process has a very recognizable pebbly, granular or mosaic surface characteristic with distinct particle  separation. Again, this is only easily and consistently seen at  high magnifications to ensure an accurate assessment of the  device.


Figure 10:


An automated lapping machine consists of a slowly rotating


main wheel or “tool” with a number of separate “control rings”


positioned on the main tool. The control rings spin  independently of the main tool in a “figure-8” fashion which  has a polishing effect on the surface being lapped – and thus  eliminating any directional marks from the work surface. The  list of available abrasive materials on the market varies greatly  to accommodate every surface material type and finish. With  very little trial and error on the part of the counterfeiter the  perfect slurry “recipe” of abrasive material(s) can be  determined to closely replicate any desired OCM surface  finish for a specific electronic part package type.


Figure 11:


Table 1:


Industry Bio on Tom Sharpe


Tom is Executive Vice President of SMT Corporation which  maintains the largest inventory of obsolete & DMS-type  electronic components as well as in-house testing services  within the Independent Distribution sector.


SMT’s labs are credited with the initial identification and


industry-sharing of several counterfeit processes over the past  several years as well as developing the required mitigation  inspections to reliably detect these new counterfeiting  methods. In 2011 Tom was requested to provide subjectmatter-expert (SME) testimony before the formal Senate  Armed Services Committee (SASC) hearings on counterfeit  electronic components within DoD supply chains. As part of


this investigation the GAO chose SMT’s lab facilities to


provide all authentication and forensic analysis on behalf of  the SASC investigation.


Functional Electronic Clones – the most dangerous NEW counterfeit threat  facing the ENTIRE Electronics Industry today


The entire electronics industry is now facing a much more  insidious counterfeit threat than at any time in the past. The  existence of cloned electronic components bearing the


markings of major component manufacturers in today’s global  supply chains has been clearly established within SMT’s labs  over the past 3 years. The most worrisome aspect of these “made from scratch” fakes is their ability to easily pass current  Industry-Standard counterfeit inspection processes and  electrical testing to the manufacturers’ data sheet.


My presentation will focus on several actual examples of this  most concerning advanced counterfeiter capability and some  of the processes utilized by SMT as an obsolescence  component supplier and testing lab to mitigate this new and  growing threat from making it to our OEM & CM customers.


Clone devices are undoubtedly the counterfeiters response to a  significant increase by industry in the detection of traditional


“modified or reworked” OCM devices. In March of 2012 SMT


released our forensic report to government on the growing  clone threat. Today, over 3 years later, we are witnessing the  clone threat growing in pandemic proportions.


The increased threat begins with reproduced manufacture  packaging and fake paperwork being generated for clone


material which closely resembles that of the OCM. The  exterior package dimensions of all clones we have inspected to  date falls within the manufacturers data-sheet specification.


The increased threat begins with reproduced manufacture  packaging and fake paperwork being generated for clone  material which closely resembles that of the OCM. The  exterior package dimensions of all clones we have inspected to  date falls within the manufacturers data-sheet specification.


The most concerning aspect of clone devices is their A/C & D/C functional characteristics; many clones we have studied  have functional / performance characteristics which test closer  to the manufacturers spec than the corresponding authentic  devices.


industry-sharing of several counterfeit processes over the past  several years as well as developing the required mitigation  inspections to reliably detect these new counterfeiting  methods. In 2011 Tom was requested to provide subjectmatter-expert (SME) testimony before the formal Senate  Armed Services Committee (SASC) hearings on counterfeit  electronic components within DoD supply chains. As part of  this investigation the GAO chose SMT’s lab facilities to  provide all authentication and forensic analysis on behalf of  the SASC investigation.


Tom is very active on the Electronics Industry speaking tour  and has become the leading voice from the independent sector  in the fight against counterfeit components in the electronics  industry. Tom’s presentations serve to educate all sectors of  the electronics industry about the growing dangers of  counterfeits in today’s market and best practices to reliably  detect and mitigate these constantly evolving dangers.


Techniques for Reverse Engineering and Functionality Extraction  of Mixed-Signal ICs for Security Applications


Franco Stellari, Chung-Ching Lin, Lynne Gignac, Raphael Robertazzi, Alan Weger, and Peilin Song


IBM T.J. Watson Research Center, 1101 Kitchawan Rd, Yorktown Heights, NY - stellari@us.ibm.com, 914-945-3223


In this paper, we discuss a set of techniques and analysis  methodologies for the reverse engineering and functionality  extraction of complex mixed-signal ICs with a special focus for  security applications. Front and back side reflected light pattern  images at different magnifications are used to identify circuit  blocks. Time-integrated and time-resolved photon emission  data is used to identify gate logic states, sequences of events, and specific functional activity. Backscattered electron and  scanning transmission electron images mosaics are used to  reverse engineer individual gates and observe local  interconnects. Thermal imaging is used to aid in the functional  block identification and analog gates analysis. Different  advanced methodologies for tool automation, focusing, mapping, and image processing are also discussed in the  context of our proposed electro-optical tester based technique.


Today’s globalization trend of IC design and fabrication has  pushed more companies to use a fabless model to reduce overall  IC cost, thus introducing a higher risk of potential hardware  security vulnerabilities. For this reason, the development of  new detection methods aimed at improving ICs security has  attracted a lot of attention [1-7]. Nowadays, the destructive  reverse engineering of ICs is still a common practice that allows  one to discover the implementation of a particular device at the  transistor and metal levels. Many companies provide this type  of service. As the term suggests, these techniques often involve  destroying the device by delayering it and analyzing its  workings in detail using SEM inspections, TEM cross sections, etc. However, these techniques are very time consuming (therefore they can be applied only to small batches of  fabricated chips), and most importantly they are destructive  inspection methods (limiting the inspection to samples that  exclude the actual chip that will be used for real applications). Our group has first proposed a non-destructive method to detect  chip alterations using a combination of optical diagnostics and  electrical tests [8]. This technique takes advantage of the fact  that every FET on an IC emits light when it is simply biased or  switched. The methodology was later extended to help identify  the attack point in digital ICs [9]. For these applications, the  optical tool of choice is the 2D Picosecond Imaging Circuit  Analysis (PICA) that was originally developed for diagnosing  time-critical ICs failures [10]. This tool can measure timeresolved emission from switching gates, as well as timeintegrated and time-resolved emission from gates in a fixed


logic state, also known as Light Emission from Off-State  Leakage Current (LEOSLC) [11]. The first type of emission is  generated by the energized carriers when current is flowing in  the FET channel, while the latter is a direct consequence of the  off-state leakage current trickling through the transistor channel  in the off state (with the gate grounded and the drain at the  supply voltage).


In this work, we have used a multitude of different approaches  and techniques to develop a methodology for the destructive  and non-destructive reverse engineering of mixed-signal chips, with particular focus to the identification of functional blocks. Most of the techniques being discussed require back side access  to the chip, which is usually achieved by thinning the silicon  substrate to about 100 µm so that it becomes transparent to light  and possibly high-energy electrons. Even after thinning, the  chip remains functional and, in most cases, it could be later  repackaged for use in real life application. In our approach we  try to leverage the capabilities of each individual technique and  combine their information in both the reverse engineering and  functional extraction tasks. In particular, we have used:


 Low magnification front and back side pattern measurements


using reflected-light optical tools or laser scanning


microscopy (LSM) to identify key components such as I/O


pins, top level metal interconnects, as well as groups of FEOL


logic that may highlight functional blocks.


 Back-Scattered Electron (BSE) imaging to perform back side


Front End Of Line (FEOL) gate mapping with ultimate


spatial resolution as well as to detect local interconnects at


the lower levels of the metal stack [12-16].


 Near InfraRed (NIR) emission measurements (both timeintegrated and time-resolved) to confirm the type and identify


the logic state of gates mapped with BSE, as well as to further


identify functional activity and functional blocks [8,17-18].  Thermal imaging to support the NIR emission data for


detecting activity in passive elements and analog gates that


do not commonly emit in the NIR spectral region.


 Advanced image processing techniques for improving image


quality to increase sensitivity and resolution, managing large


datasets by registering and stitching the images [16,19,20],


detecting small changes and recognizing common patterns. In this paper, we apply these techniques to an unknown-to-us  mixed-signal waveform synthesizer chip fabricated in 90 nm  bulk technology. In the following sections, we will show that  using these techniques we can readily identify key functional  blocks, such as the DAC, memory, PLL, I/O and RTL logic. Furthermore, emission allows one to discover that only one  quadrant of the chip is functioning. By using emission and BSE  images combined, we can reverse engineer the digital


component of the DAC and show that functional behavior can  be extracted. Low and high magnification emission data is also  used to localize the chip Serial Peripheral Interface (SPI) register controller, down to the gate level. Furthermore, by  applying via (CA) detection and feature recognition techniques  on BSE maps, we can automatically reverse engineer the FEOL  gates of large areas of synthesized logic blocks.


Device Under Test (DUT)


The work discussed in this paper was performed on a thirdparty custom designed high-performance 10 Bit, 2.5 GSPS, RF  Digital-to-Analog Converter (DAC) capable of synthesizing  signals from DC up to 1.25 GHz. The flip-chip was  manufactured on an ASIC 90 nm SF CMOS process by a third  party and provided to us with only the limited information that  would be available from a commercial source. Fig. 1 shows the  block diagram information available in the standard  manufacturer datasheet. A four pin Serial Peripheral Interface (SPI) is used to program the chip and load an arbitrary  waveform into a 4x1024x10-bit dual-port synchronous RAM  memory. The on-chip clock can either be generated by an onboard 2.5 GHz Phase-Locked Loop (PLL) or provided  externally through a differential high-speed reference clock  signal. The provided datasheet information details the different  modes of operation including, initialization of the chip, memory  write, memory read, and waveform generation through the onchip high-speed 10-bit Digital to Analog Converter (DAC). The  DSP engine is based on a memory read-out or play-back  architecture. Samples of the desired waveform to be generated  are written onto the memory at a low rate using the SPI. The  memory play-back is based on two modes of operation: Arbitrary Waveform Generator (AWG) or Direct Digital  Frequency Synthesis (DDFS). In AWG mode, the memory is  sequentially addressed at the clock rate to synthesize any  arbitrary waveform.


The third party samples were provided to us as naked fullthickness chips with C4s, individual Ball Grid Array (BGA) flip-chip packaged modules, and attached to a standard test  board as shown in Fig. 2. For reflected light imaging and back  side BSE imaging, the unpackaged dies were selected to reduce


the device preparation cost and time. For back side timeintegrated and time-resolved emission measurements, individual BGA modules were de-capsulated and the silicon  substrate was thinned to ~100 µm, compatible with our Solid  Immersion Lens (SIL). To perform measurements with the chip  powered on and functional, the provided test board was reworked to replace the existing BGA module with a thinned  module that exposed the Si back side to the microscope lenses. This, although invasive, is a nondestructive technique because, after the procedure, the module is still fully functional and can  be operated electrically during the emission measurements. It  should also be noted that full silicon thickness SILs are  available from a variety of manufactures and could be used on  the chip after simply de-packaging and polishing without the  need of thinning the substrate, thus significantly reducing the  preparation effort.


To exercise the main functionality of the chip, a custom  interface and test patterns were developed to replace the  provided FPGA based test environment with an Advantest  93000 tester. This solution was chosen to enable more  flexibility in the programming of the chip through the SPI. Furthermore, in all the experiments discussed in this paper, the  chip was always clocked externally with the on-chip PLL  turned off. This allows an easier sweep of the frequency and  synchronization with emission-based techniques such as PICA.


Key techniques and methodologies


Several key techniques and tools were developed as part of this  project, including tool control, complex instrument setup  automation, large image dataset acquisition, autofocusing, image processing and stitching, etc.


An underlying component was to create generic software  interfaces to the analytical tools so that key capabilities , such  as stage movement, instrument setup, and data collection, could  be operated in a programmatic way from other dedicated  software packages or from different tools involved in the  experiment. These interfaces are generic, do not require  software API from the tool vendor, and, although coded with  one particular programming language, can be easily addressed  using other software and programming languages. In addition, network connectivity is easily allowed so that the overall  acquisition system may be run over the network, thus


Fig. 1: Block diagram of the mixed-signal DUT obtained from  the manufacturer datasheet.


Fig. 2: A mixed signal DUT with the back side exposed and  thinned to ~100 µm is mounted on a test board.


permitting the interaction among multiple tools in a virtual lab  environment such as the one discussed in [16].


Identifying the correct/best focus for a measurement is often  very challenging during automated data acquisition from large  areas of a chip. This problem becomes even worse when one  needs to maintain good focus from one SIL landing position to  the next one. In fact, most SIL objectives on the market rely on  some sort of spring loading between the SIL tip and a backing  air-gap objective. The distance between the SIL tip and the  objective is changed to achieve the best focus, while the spring  mechanism applies the desired pressure to guarantee a good  solid contact between the tip and the silicon substrate. Due to  the difficulty of reproducing the same conditions reliably, in  conjunction with small variations in silicon substrate thickness  and surface preparation quality, the best focal Z position may  change from one position to the next. Over several years we  have developed autofocusing algorithms that rely either on  reflected light pattern images or directly on emission data [19,20].


In [18], we first discussed how chip functionality can be  successfully analyzed by combining the concepts in [8] with the  tester-based optical diagnostic system [21] that we have  developed to verify chips in a more general case. In particular, we would like to use the concept of tester-based optical  methodology to localize and extract functional blocks from a  chip of unknown design. In conventional test and diagnostic  applications, the response of a DUT is measured under certain  operating conditions to verify its functionality against a set of  expected behaviors/patterns or failing hypothesis [21]. Examples of stimuli include voltage bias conditions, clock  frequencies, initialization test patterns, functional test patterns, chip operating temperature and cooling conditions, etc. Usually, the specific operation is selected to exercise the chip  in a desirable and known condition so that it expresses a certain  behavior that may be used to confirm or rule out a failing  hypothesis. The diagram in Fig. 3 describes the key elements of  the proposed methodology. The DUT is exercised with a set of  different stimuli, one at a time. For each one, one or more  measurements of the chip are collected using analytical tools, such as emission and thermal tools. In this case, different types  of stimuli are devised to exercise the DUT in slightly different  ways, thus introducing detectable changes in the measured


images. The set of measurements is subsequently analyzed  together, not individually, based on the specific knowledge of  the set of stimuli used. Subsequent image analysis and postprocessing techniques allow to identify the portions of the  circuit that are affected by the specific set of stimuli for  functional block localization. For example, clock exercisers at  different frequencies may be used to target the localization of  the clock distribution network. Targeted logic state changes in  a particular circuit performing a certain function may be used  to separate it from surrounding logic gates. Switching activity (using time-resolved measurements) may also be used to  highlight gates being used by a certain functional exerciser. By  combining the knowledge of the characteristics of the different  stimuli with the observed effect of each stimulus in the set of  measurements, one can extract additional information that  would not be available from a single stimulus and  measurement. This process can be automated by adding a  feedback loop for adjusting the stimuli generation based on the  results of the analytical tool measurements.


Reflected-light pattern imaging


For the purpose of functional extraction and reverse  engineering, optical tools can be used for two primary  activities: acquire pattern images of the chip from both the front  and back side of the chip, as well as acquire spontaneous Near  InfraRed (NIR) emission from the active circuits in both static  and dynamic conditions. Both techniques are non-destructive. By acquiring the reflected light pattern image from the front  side of the chip we can identify pins (in this case C4 contacts) as well as high level Back End Of Line (BEOL) interconnects  that use the top metal levels as show in Fig. 4. The dark circles  in the image represent the location of the C4 contacts. Since the  datasheet provides the role of each C4 (such as ground and Vdd  contacts), one can identify the top main metal levels that are  connected with each C4 and trace part of the signal path. For  example, red lines in Fig. 4 highlight Vdd busses while blue  lines indicate ground contacts.


On the other hand, pattern images acquired through the back  side of the chip allow the recognition of major functional blocks


Fig. 3: Block diagram of the tester-based methodology [18].


Fig. 4: Block diagram of the mixed-signal DUT obtained from  the manufacturer datasheet.


by the identification of local Front End Of Line (FEOL) interconnect and circuit blocks: transistor diffusions produce a  clear contrast to empty silicon areas. By leveraging the  information provided in the datasheet (e.g., pin names, assignment, and proximity), along with the information  extracted from the front side pattern images, one can start to  infer the function of the sub-blocks identified in the back side  images. Later on, emission data due to specific functional  activity can be used to corroborate these hypotheses. For  example, by comparing the high magnification back side  pattern image in Fig. 5(a) to the front side pattern image with  C4 contact functions highlighted (Fig. 5(b)), one can identify  several key elements of the circuit including Vdd/gnd I/O  circuits (red boxes), RF/high frequency pads (purple boxes), low speed SPI digital I/Os (green boxes), DAC sub-circuit (orange box), memory arrays (light blue boxes), and PLL subcircuit (dark blue box). Additional major areas with synthesized  logic gates are identified by the darker regions located between  the memory arrays and the DAC. Further details of these high  level functional blocks can be extracted by using higher  resolution techniques, including Solid Immersion Lens (SIL), and BSE beams.


Back-Scattered Electron (BSE) imaging


Although pattern emission images are very effective in  covering large field of views (FOVs) and provide an indication  of the location and distributions of key functional blocks, their  lateral spatial resolution is often insufficient to reverse engineer  individual gates and macros. For this purpose, a high energy (300-400 keV) BSE imaging technique was developed [14] to  image key interconnect structures on the chip. BSEs are  electrons that are produced when an incident electron beam  scatters with the nucleus of atoms near the surface of a sample  and are then emitted back out of the sample. BSE images are  obtained when the BSEs are collected by a detector sitting  above the sample. If the incident beam energy is high, electrons  can be scattered and re-emitted from large depths (several µm) in the sample below the surface. Materials with a high atomic  number (Z) backscatter electrons more efficiently than low Z  materials so BSE images highlight materials with varied Z (Z  contrast). An IC chip with multilevel Cu interconnects (high Z)


embedded in SiO2 dielectrics (low Z) is an ideal sample to  detect multiple interconnect levels from different depths with  one high energy BSE image [14-16]. By performing a detailed  study of the back side BSE image quality as a function of the  remaining chip substrate thickness, we have been able to show  that <2 µm of remaining silicon substrate is desirable to achieve  sharp image quality for the Cu interconnects. Although, this  requirements is much stronger than the one for a SIL (~90 µm  for our tip), it may still allow the chip to operate for some  applications. This requirement could be relaxed if only vias (which have high Z) are mapped for gate recognition purpose. However, it should be noted that, for convenience (chip  preparation was outside the scope of this work), the entire  silicon substrate was removed with XeF2 for the images  presented here, thus making it a destructive technique.


For this work, the chips were imaged with a JEOL 3000F  Transmission Electron Microscope (TEM)/Scanning TEM (STEM). This system has a Schottky field emission electron  source, a maximum incident beam energy of 300 keV and  micro-channel plate BSE/Secondary Electron (SE), Bright  Field (BF) STEM and Annular Dark Field (ADF) STEM  detectors. Contrary to initial expectations, good resolution  images of the interconnect structure on the thick test chip (~8.5 µm thick with 10 interconnect levels) could be obtained  by 300 keV BF STEM.


Fig. 6 compares images of the same region of the back side of  a test chip taken with different microscopes and detectors: 300 keV images from the JEOL 3000F (a) BSE and (b) BFSTEM (red line marks the cross-section shown in Fig. 8) and  28 keV images from the FEI Helios 400s dual beam focused ion


Fig. 5: Key circuit elements are identified in the back side  pattern image (a) using C4 locations (b).


Fig. 6: Images taken from the back side of the chip in the  JEOL 3000F at 300 keV (a) BSE and (b) BF-STEM and in the  Helios 400s at 28 keV (c) SE and (d) BSE. The red line in (a) and (b) marks the location of the cross-section TEM sample.


beam (DB-FIB) (c) SE, and (d) BSE. The BSE mode on the  micro-channel plate detector in the JEOL 3000F captures BSEs  and a significant number of SEs. The SE component of the  image provides information about the surface detail such as  rectangular silicon etched out regions and balls of surface  debris. The BSEs in the image provide sub-surface, atomic  number (Z) contrast information such as the circular W contact  vias and several Cu interconnect layers. The BSE images can  be used to identify gates since the RX diffusion (etched out Si) and CA contact vias are recorded. The BF-STEM image shows  Z contrast and sub-surface features without the interference of  the surface detail that is seen in the BSE image. The BF-STEM  image has inverted contrast from the BSE image since high Z  components scatter electrons out of the BF-STEM detector  creating dark contrast in BF-STEM images but have higher  BSE yield and brighter contrast in BSE images. The 28 keV SE  and BSE images in Fig. 6(c) and (d) respectively were taken  with the through-the-lens Everhart-Thornley detector in the FEI  Helios 400s DB-FIB and are examples of information that can  be obtained in a typical scanning electron microscope (SEM) with a maximum incident beam energy of 30 keV. These  images show similar surface details but less sub-surface  information than Fig. 6(a) demonstrating the need for higher  energy BSE imaging capability.


In the JEOL 3000F, BF-STEM and BSE images were  automatically collected as the stage moved the sample in x and  y directions. Specialized software to automatically stitch  together the images was developed [16]. Fig. 7 shows a stitched  image of the DAC consisting of 7 image sets containing a total  of 1476 individual BSE frames. Some of the dataset do not  perfectly overlap leaving small portions of the DAC unmapped.


A destructive analysis of one of the test chips was performed to  gather reference information about the fabrication technology  and help understand how many layers of interconnects were  visible in the BSE and BF-STEM images. In particular, Fig. 8  shows a TEM cross-section of the DUT: the BEOL interconnect  is 8.5 µm thick and consists of W contact vias (CA) to silicon  or poly-Si, eight levels of Cu interconnects and one Al  interconnect level. The TEM section in Fig. 8 was taken from  the location in the BSE and BF-STEM images in Fig. 6(a)-(b), respectively, marked with a red line. The BSE and BF-STEM  images show sub-surface Cu lines down to the M8 level which  is 5 m below the back side surface.


Photon emission imaging


It is well known in the diagnostic and failure analysis  communities that any FEOL gate emits light when power is  applied to it [10,11]. Such emission is intrinsic to the device  operation in both transient and stationary conditions. This faint  near-infrared light may be detected from the back side of the  chip, thanks to decades of development in emission tools for  demanding failure analysis applications. This inspection is  mostly non-invasive and non-destructive for the DUT that  operates in its normal operating conditions during test and  characterization. In this paper, we thinned the silicon substrate  down to 100 µm to be compatible with our SIL tip leaving the  device fully operational. Alternative lenses are also available to  work with full-thickness chips.


The authors would like to thank C. Breslin, J. Bruley, K. Jenkins, B. Linder, J. Stathis, K. Stawiasz, E. Ray, E. Yashchin, J. Salimeno, M. Taubenblatt, and M. Soyuer from IBM.


The authors would also like to acknowledge H Iida, S. Kim. T. Nakamura, K. Atsuko and others from Hamamatsu Photonics  for the support in the development, installation and  maintenance of the tool used in these experiments.


This work was supported by the Defense Advanced Research  Projects Agency (DARPA) under SSC Pacific contract  HR0011-11-C-0060. The views, opinions, and/or findings  contained in this article/presentation are those of the  author(s)/presenter(s) and should not be interpreted as  representing the official views or policies of the Department of  Defense or the U.S Government.


[1] Defense Advanced Research Projects Agency, “Integrity and Reliability  of Integrated Circuits (IRIS),” http://www.darpa.mil/Our_Work/MTO /Programs/Integrity_and_Reliability_of_Integrated_Circuits_%28IRIS%


29.aspx


[2] D. Agrawal et al., “Trojan Detection using IC Fingerprinting”, IEEE  Symposium on Security and Privacy, 2007, pp. 296-310.


[3] R. Rad et al., “Sensitivity Analysis of Power Signal Methods for  Detecting Hardware Trojans Under Real Process and Environmental  Conditions”, IEEE Trans. on Very Large Scale Integration (VLSI) Systems, vol.18, no. 12, 2010, pp. 1735-1744


[4] S. Narasimhan et al., “Multiple-parameter side-channel analysis: A noninvasive hardware Trojan detection approach,” IEEE Int. Workshop on  Hardware-Oriented Security and Trust, 2010t, pp. 13-18.


[5] Y. Jin and Y. Makris, “Hardware Trojan detection using path delay  fingerprint”, IEEE Int. Workshop on Hardware-Oriented Security and  Trust, 2008, pp. 51-57.


[6] High  Performance  Microchip  Supply, http://www.acq.osd.mil/dsb/ reports/ADA435563.pdf


[7] X. Wang et al., “Detecting  malicious  inclusions  in  secure  hardware: challenges and solutions”, IEEE Int. Symp. on Hardware-Oriented  Sesurity and Trust (HOST), 2008, pp. 15-19.


[8] P. Song et al., “Malicious alteration recognition and verification by  emission of light”, IEEE Int. Symp. on Hardware-Oriented Security and  Trust (HOST), 2011.


[9] D. Nedospasov et al., “Functional integrated circuit analysis” ”, IEEE Int. Symp. on Hardware-Oriented Security and Trust (HOST), 2012, pp. 102-107.


[10] J.A. Kash and J.C. Tsang, “Dynamic internal testing of CMOS circuits  using hot luminescence”, IEEE Electron Dev. Let., vol. 18, no. 7, 1997, pp. 330-332.


[11] F. Stellari et al., “Testing and diagnostics of CMOS circuits using Light  Emission from Off-State Leakage Current”, IEEE Trans. on Electron  Devices, vol. 51, no. 9, 2004, pp. 1455-1462.


[12] L.M. Gignac et al., “Imaging and analysis of subsurface Cu interconnects  by detecting backscattered electrons in the scanning electron  microscope”, J. Appl. Phys., 97, 114506-14 (2005).


[13] L.M. Gignac et al., “High energy backscattered electron imaging of  subsurface Cu interconnects”, JEOL News, 40(1), 13-17 (2005).


[14] L.M. Gignac et al., “A method to reverse engineer semiconductor chips  using high energy backscattered electron (BSE) imaging from the top and  back sides of the chip”, Int. Conf. on Science for Defense and Security,


2012.


[15] L.M. Gignac et al., “High energy BSE/SE/STEM imaging of 8 um thick  semiconductor interconnects,” Microscopy & Microanalysis, 2014.


[16] C.C. Lin et al., “Automatic registering and stitching of TEM/STEM  image mosaics", Int. Symp. for Testing and Failure Analysis (ISTFA), San  Jose, CA, 2013.


[17] F. Stellari et al., “Verification of untrusted chips using trusted layout and  emission measurements”, IEEE Int. Symp. on Hardware-Oriented  Security and Trust (HOST), Arlington, VA, 2014, pp. 19-24.


[18] F. Stellari et al., “Functional block extraction for hardware security  detection using time-integrated and time-resolved emission  measurements”, VLSI Test Symp. (VTS), Napa, CA, 2014, pp. 1-6.


[19] F. Stellari and P. Song, “Advanced methods and software for enhancing  analytical tools capabilities during chip diagnostic and characterization”, Int. Symp. for Testing and Failure Analysis (ISTFA), Phoenix, AZ, 2012. [20] C-C Lin and F. Stellari, “Automated mapping of very large areas of VLSI  circuit using SIL”, Int. Symp. for Testing and Failure Analysis (ISTFA), Houston, TX, 2014, pp. 12-18.


[21] P. Song and F. Stellari, “Tester-based optical and electrical diagnostic  system and techniques”, VLSI Test Symposium (VTS), 2012, pp. 209-214.


WISE%and%ICARUS:%New%X2Ray%Algorithms%to%Improve%the%Detection%of%Counterfeit%Components%


Dr.$Bill$Cardoso$$


Creative(Electron,(Inc.(


info@creativeelectron.com,(+1(760.752.1192(((


((((


The drive towards miniaturization has created increasing  challenges to the overall failure analysis and quality inspection  of electronic devices. This trend has equally challenged the  image quality of x-ray inspection systems – engineers need to  see more details in each inspection. Image quality is  paramount to the ability of making actionable decisions on the  information acquired from an x-ray machine. Previous  generations of x-ray technologies have focused on hardware  improvements – better x-ray sources and better x-ray sensors. Although further improvements can still be achieved in  hardware, our focus will be on the latest wave of technology  breakthroughs and innovation in radiography systems: algorithms.


The success of our global economy relies on the free flow of  information and products across multiple geographical  boundaries. In a networked society, markets transcend  political borders to reach every corner of the globe. With such  connectivity come serious challenges to protect the homeland  from foreign and domestic threats. The influx of counterfeit  electronic components in our supply chain is an everincreasing threat to our economy. The latest report issued by  the US Department of Commerce states that the number of  counterfeit incidents almost tripled between 2005 and 2008. The US is especially vulnerable to the threat of counterfeit  electronic components. The task of controlling the influx of  products into our 327 ports, with over 10 million containers  and almost 31 million entries every year, is daunting. Moreover, the focus of our Department Homeland Security  officials is in counterterrorism, border security, readiness  against natural disasters, immigration, and cybersecurity. As a  result, the more than 50,000 people employed by the  Department of Homeland Security is busy looking for  different threats to the homeland, and despite recent efforts, the search for counterfeit components is not always on the top  of their list. Therefore, it becomes the users and suppliers’ responsibility to assure that the supply chain is free of  counterfeit electronic components.


Algorithms have been paramount in enabling the inspection of  challenging electronics assemblies. From computed  tomography to dual energy algorithms, these special pieces of  software may be the difference between finding or not finding


an issue with your sample.  In this presentation we will go  behind the curtains and see how these algorithms are designed. The examples presented will illustrate real life situations that  show the extent of the use of algorithms in radiography for  failure analysis and quality control.


Image Comparison Algorithms for Radiography  Unified Software (ICARUS)


The Image Comparison Algorithms for Radiography Unified  Software – ICARUS – is the convergence of over a decade of  algorithm development into a unified software platform. ICARUS combines several image comparison algorithms  under one umbrella to determine the exact location in the xray images that differ from a reference image. These  algorithms work in tandem to find the optimal answer to the  question: is this image similar to the reference image?


ICARUS uses a nonlinear optimization algorithm since both  objective and constraint functions are nonlinear. In order to  estimate the optimal similarity kernel that will give us the best  match between reference and acquired image, an objective  function is defined as the mean squared difference between the  image


!(#)


and the reference image


[1]. The error  between the image and reference image, or the similarity  between them, is given by:


Er = ŝ(n)− s(n)( )2


n=0


N−1


∑


!


The goal of the optimization is to generate a kernel based on  the acquired image that is as similar as possible to the  reference image. Figure 1 shows a block diagram of the  objective function.


(n


Er


Optimization kernel


ˆ ns


( )∑ − 2)()(ˆ nsns


Figure 1 – ICARUS optimization objective function


The solution for the optimization kernel that minimizes the  objective function can be described as:


( )


1,0


.


ˆ


min


−


∑∑


k


δ


Where M is the finite impulse response (FIR) filter length, h(n) are the coefficients of the FIR filter, and δ(n) is the Dirac  delta function. The above equation sets the condition for  perfect reconstruction. Although this is an important  requirement in the solution of an optimization kernel, there are  other issues that affect the performance of the kernel in  representing data.


To find the solution to this problem, numerical methods using  Lagrange multipliers were used to evaluate the optimization  function. The Lagrange algorithm simplifies the calculation of  nonlinear constrained optimization problems since it does not  require the explicit solution of the conditions. The Lagrangian  function can be written as:


( ) ∑ ∑= =


"""#$


%%%&'


λ


Where λi is the set of Lagrange multipliers. The necessary  conditions so that h* is a local minimizer of the mean squared  error function are stated as follows [Nas96]


definite


semi


positive


xx


T


∇


*


Where Z(h*) is a null-space matrix for the Jacobian matrix of  the constraint function. The necessary conditions to satisfy the  minimization problem so that h* is a strict minimizer are


λ∇


To better illustrate how these algorithms that compose  ICARUS work, Figure 2 shows a typical space of the problem  we are trying to solve. The mesh in this figure has several  peaks and valleys – some higher or lower than others. The key  to finding the best match, and the optimal differences between  two images, is to find the lower valley in this mesh. As you  can see it is not an easy problem, and that’s why we need all


the before mentioned math to help us. The challenge here is  that the algorithm can get stuck in one of the local minima, and as a result miss the global minimum (or the minimum of  the minima).


Figure 2 – ICARUS minimization space


To visualize ICARUS working on a real case, the following  example shows two images with small differences between  them. The reference image on the left shows a module without  any defects. The acquired image on the center presents a  couple of subtle defects: a broken wire bond and a damaged  solder ball. ICARUS correctly identified these defects in the  right image.


Figure 3 – ICARUS example. Left: reference image, sample without defects. Center: acquired image to be  compared to the reference image using ICARUS. Right:


ICARUS result image showing differences between


reference and acquired images


Wavelet Image Spectral Enhancement  Algorithm (WISE)


The analysis, storage, and transmission of x-ray data can  benefit from sharpening and noise suppression algorithms. The data augmentation performance of the discrete wavelet  transform (DWT), the discrete Fourier transform (DFT), and  the discrete cosine transform (DCT) are examined when  applied to simulated and experimental x-ray data. An adaptive  threshold is applied to remove the smaller coefficients of the  frequency domains to achieve data filtering. Then, the signals  are reconstructed from the remaining coefficients.  The mean  square errors of these techniques are analyzed for filtering and  compression ratios of up to 90%. For higher ratios, the


continuous wavelet transform (CWT) is also investigated in  this section. The CWT performs the correlation of a kernel  wavelet with the radiographic signal. A modified version of  the Morlet wavelet is used as the kernel wavelet to estimate  the signal parameters. Upon the determination of these  parameters, high data improvement and denoising can be  obtained. The CWT is applied to both simulated and  experimental data, and the results are presented here.


Thresholding Techniques


Subband transform (DWT) and transform coding techniques (DCT and DFT) provide a representation of the input signal  into separate frequency bands. Data filtering is therefore  achieved by selecting portions of the frequency domain where  the signal is expected. Energy in the frequency domain outside  the bandwidth of the signal is usually due to noise. This  method is most effective for bandwidth limited signals with  uncorrelated noise.


DWT, DFT, and DCT


The filter bank representation of the DWT is shown in Figure


4. The lowpass h0(n) and the highpass h1(n) filters are analysis  filters, while g0(n) and g1(n) are lowpass and highpass  synthesis filters [2].


h0(n) h1(n)


g0(n) g1(n)


2  2


WT


IWT


Figure 4 – Discrete Wavelet Transform


The analysis filters h0(n) and h1(n) can be selected as  quadrature mirror filters (QMF). In such configuration g0(n) and g1(n) are the time reversed versions of h1(n) and h0(n) respectively. In order to recover the input signal from the  DWT coefficients, h0(n) and h1(n) have to satisfy the  following condition:


,)


(1) The DFT of a signal f(n) (or fN in a vector representation) of  length N is defined in Equation (2). The frequency domain  signal FN is a linear combination of the time domain signal fN  with the kernel WN.


f


W


F


(2) In the above equation WN is an N×N symmetric matrix defined  as:


,...,1,0


,1


exp


"#$


%&' −


kn


j


π


The inverse DFT (IDFT) is shown in Equation (3).


1−


Referring to the case of a simple complementary inverter, when  the output of the gate is at logic “1”, the n-FET produces Light  Emission from Off-State Leakage Current (LEOSLC) [11], while the p-FET is not emitting any light. When the output of


Fig. 7: 300 keV BSE mosaic of 1476 images of the DAC


acquired from the back side of the chip with silicon removed.


Fig. 8: Cross-section TEM image of the BEOL stack. Sample  sectioned along the red line shown in Fig. 6(a)-(b).


the gate is at static logic “0”, the p-FET emits light with the  n-FET being dark. If the gate is toggled, short bursts of hotcarrier luminescence will also be emitted by either the n-FET  or the p-FET. Based on this understanding, both time-integrated  and time-resolved emission measurements can be used to  identify logic gate types and switching activity, etc.


High magnification (up to SIL) emission maps were acquired  using our automated data acquisition software, image  processing, and stitching algorithms. For functional block  identification we have used and extended our tester-based  optical-electrical methodology (Fig. 3). Different types of  stimuli are devised to exercise the DUT in slightly different  ways, thus introducing detectable changes in the measured  images [18]. The measurements are subsequently analyzed  together to identify the portions of the circuit that are affected  by the specific set of stimuli for functional block localization. For example, clock exercisers at different frequencies may be  used to target the localization of the clock distribution network. Targeted logic state changes in a particular circuit performing a  certain function may be used to separate it from surrounding  logic gates. Switching activity (using time-resolved  measurements) may also be used to highlight gates being used  by a certain functional exerciser.


For the DUT, low magnification emission images were  acquired with the DAC generating an arbitrary waveform stored  in the on-chip memory (Fig. 9(a)) and the DAC halted in a  quiescent state (Fig. 9(b)). By performing a differential  analysis, it was possible to highlight that only the top-right  quadrant of the chip was involved in the functional exerciser (Fig. 9(c)). This indicated that most of the chip memory arrays (left and bottom quadrants) previously observed in the back side  pattern are actually not being used. Each one of the blocks in  Fig. 9(c) corresponds to one of the four memory blocks  described in the datasheet. Additionally, Fig. 9(c) clearly shows  the “arrow” shaped data path inside the block of synthesized retiming logic from the memory blocks to the DAC positioned in  the center. By looking at the original images (a) and (b), one  can also observe several bright spots in the unused digital logic  areas as well as the DAC area. Based on our experience, the  first type of bright spots corresponds to gates with their input  left floating that may ultimately lead to a partial activation of  the gates due to noise and leakage into a conductive, and  therefore bright state. This may be the result of disabling three


of the four memory quadrants. These spots are also observed by  the thermal camera as described later in the paper.


Higher magnification static and dynamic images were also  acquired from selected regions inside the digital logic areas to  identify the local clock buffers by running the clock without any  functional exerciser activated. Fig. 10 shows a comparison of  clock buffers with and without a clock applied: differential  imaging can again easily point out the gates of interest. Further  analysis using 2D PICA data separates the main clock buffer  from the dependent local clock buffer by measuring the  sequence of switching events in time: a ~60 ps signal delay is  observed (Fig. 10(c)).


A high magnification analysis of portions of the digital logic  was also performed using the developed SIL mapping  methodology [20]. To the best of our knowledge, this is the first  time that such a technique has been demonstrated on a real chip. Thousands of images have been acquired from the test chip and  were used to create mosaics of more than 25 x 25 images  covering a total area of approximately 400 x 400 µm2. In  particular, this technique was used to localize the SPI functional  block that programs the chip operation and loads the arbitrary  waveforms into memory. For this purpose, low magnification  differential images were first acquired while repeatedly  programming the SPI interface through an Advantest 93000


Fig. 9: Time-integrated emission acquired when the DAC is (a) running, (b) quiescent, and (c) after differential analysis.


Fig. 10: Time-integrated emission images of several clock  buffers in (a) quiescent and (b) running state. (c) 2D PICA  show propagation delays and identify the signal sequence.


tester. This analysis pointed to a small portion of logic above  the isolated memory array on the right hand side of the PLL (see  Fig. 5(a)). Once the general area was localized, several 10 x 10  SIL maps were acquired by running different types of patterns. For example, Fig. 11 compares a SIL emission map of the SPI  area acquired while preforming (a) an exhaustive test of the SPI  register to (b) a quiescent emission image. The difference (c) highlights the increase (red) and decrease (blue) of emission  due to the logic state changes of the individual gates in the SPI  digital logic.


A detailed analysis of the DAC sub-circuit was also performed  by setting up the chip to generate different square waveforms  loaded into the on-chip memory. Each waveform was designed  to have a different amplitude so that different levels of the DAC


would be exercised. Differential emission images were then  acquired to identify the DAC bits (e.g., most and least  significant). Unfortunately, due to a known chip design issue, it  was not possible to reliably control the data streams from the  memory to the DAC. Therefore, only qualitative changes could  be demonstrated using the emission. Fig. 12 shows three  emission images acquired with the DAC in (a) a quiescent state (not generating any waveform), as well as while generating a  square waveform of (b) 128 and (c) 512 amplitude (note that  the 10 bit DAC allows for a maximum 1023 amplitude). By  differentiating the measured images, it is possible to highlight  which portion of the DAC is involved in generating the required  output levels. In particular, one can notice that to generate the  larger 512 level, a 4X bigger portion of the DAC is being  exercised compared to the smaller 128 level waveform.


Fig. 11: Emission from the SPI logic is acquired during (a) an exhaustive register test, (b) a quiescent state. The difference (c)


highlights the gate involved in the test operation.


Fig. 12: Emission images of the DAC acquired in (a) quiescent state, and while generating square waveforms of (b) 128 and (c) 512  amplitude. Differential images (d,e) show the portion of the DAC activated by the patterns.


Thermal imaging


Like NIR photon emission imaging, thermal imaging uses  longer wavelength (usually 3 to 5 µm) infrared detectors to  produce images of light emitted from the chip. The most  popular detectors in scientific applications are made of Indium  Antimonide (InSb) material, cooled to around 77 K, that have a  wide spectral sensitivity thanks to their low band gap (~7 µm). While hot-electron emission is produced within FETs and is  primarily confined to the silicon channel and the drain, the heat (and therefore the thermal emission) are easily spread out by  silicon substrate and metal wiring, thanks to their good thermal  conductivity. In addition, the longer wavelength used by  thermal cameras intrinsically reduces the lateral spatial  resolution. Furthermore, while hot-carrier emission is basically  an instantaneous process that tracks the FETs activity with great  fidelity, thermal emission is affected by a thermal time constant  that is orders of magnitude slower. It should also be noted that  the different materials used in modern ICs have a different  thermal emissivity that may strongly modulate the thermal  signal and therefore make the analysis rather complicated. On  the other hand, thermal emission measurements have two key  advantages over photon emission. First, we can detect a thermal  signals from passive and BEOL elements, such as wires  carrying elevated current. Second, the thermal emission signal  is a linear function of the power density while the hot-carrier  photon emission is an exponential function of the supply  voltage. For this reason, activity in analog circuits, which  usually divide the available supply voltage across several FETs, may be studied better using thermal emission signals.


Fig. 13(a) shows a low magnification thermal image of the  entire chip without emissivity correction applied. The image  easily reveal key circuit structures that can be used for  navigation and registration, similarly to reflected light pattern  images. Fig. 13(b) shows an emissivity corrected image of the  top center portion of the chip containing the DAC and digital  logic areas when the DAC is programmed to generate a square  waveforms with a 1 GHz external clock. Several “hot spots” are  immediately apparent in both images.


Fig. 13(b) shows also that the thermal gradients across this chip  is quite modest, except for the 6 specific “hot spots” locations  that are several degrees hotter than their surroundings. Some of


the hot-spot match well the location of the bright emission spots  in the static emission measurements that were attributed to  floating gates in the unused portions of the chip. Additional  locations inside the DAC and clock network are also identified.


Image processing and analysis


Mainly, three types of images were registered, overlaid, and  used during the reverse engineering process:


 BSE mosaics to image W via (CA) locations and RX


diffusions that were used to identify gates;


 BF-STEM mosaics of M1/M2 metal layers that were used to


extract local gate interconnects;


 Back side emission images to identify the emission signature


of the gate (type and logic state) and circuit activity.


In particular, we develop an automated method to identify  standard cells in (stitched) BSE/BF-STEM mosaics. Tungsten (W) CA vias are a crucial element in ICs because they create  the gate, drain, and source contacts of any FET. Due to the high  atomic number of W, they also produce a strong signal in  BSE/BF-STEM images. For this reason, CA constellations can  provide important and reliable information for automatic  reverse engineering of individual gates. Our method detects  CAs and uses their locations to identify standard cells. First we  use the general Hough transform to detect circular shapes (characteristic of CAs) in the BSE/BF-STEM stitched image. The detected circles are used to create a CA constellation after  noise reduction and edge enhancement are applied on the image  to improve CA detecting performance. In order to identify the  standard cells, a set of golden CA maps is created using the  standard cell library or from manually reverse engineering a  small portion of the FOV. Each golden CA map is used to  compare against the CA constellations that are automatically  extracted from the BSE/BF-STEM mosaics. Four orientations  are compared for each golden cell. To tolerate CA detection  error, detection bias, and stitching error, the comparison is map  to map. This method uses oversampling to tolerate small errors  and bias. A measure of CA and standard cell identification  performance was also developed.


As an example, a 12 x 12 BSE mosaic of a region with digital  logic circuits is analyzed by our algorithm to detect ~12,000  CAs. About 4,800 (38%) of the CAs can easily be recognized


Fig. 13: (a) Lower and (b) higher magnification thermal  image (a) without and (b) with emissivity correction.


Fig. 14: CA vias and standard cells are automatically  identified in the BF-STEM image using our algorithm.


to be VDD and GND contacts due to their layout in organized  rows. By using a small library of about 21 golden standard cells, about 43% of the remaining 7,800 CAs can be grouped into  known sub-circuits of different sizes. Fig. 14 shows the  detection results for the example above. The red dots highlight  the detected CAs while the rectangular boxes show the detected  standard cells with 100% (green) and 80% (red) confidence. Different line styles of the boxes represent different orientations  of the standard cell. One can note that the confidence reduction  is mostly due to missing CAs.


A nonlinear Support Vector Machine (SVM) with Gaussian  Radial Basis Function (RBF) kernel was also used to develop  and train a classifier capable of identifying certain gates from  both static photon emission images and reflected light pattern  images. In this paper, the algorithm was trained to recognize  certain types of large buffers that are spread across the digital  logic regions that were mapped using a SIL (pattern image  mosaic in Fig. 15(a)) and a 100X air gap lens (photon emission  image mosaic in Fig. 15(b)). The buffer locations are  highlighted by red colored marks in both images in Fig. 15. The  precision and recall of the buffer detection on the pattern image  are 74% and 80%, respectively. The precision and recall of the  buffer detection on the emission image are 88% and 76%. Besides the obvious reverse engineering application, the


identified buffers can be effectively used as registration  markers between the two types of images that are otherwise  incoherent and at different magnification scales. This technique  enables one to correlate the logic state information from the  emission images with physical parameters from BSE/BFSTEM or pattern images as shown in Fig. 16 example.


Fig. 17 shows an example where a partial layout was extracted  from the BSE/BF-STEM image combination. First the CA  algorithm in combination with the golden set of standard cell  signatures can be used to identify and reverse engineer the basic  gates of the circuit from the BSE mosaic. Then M1/M2 metal  layer information, included in the BF-STEM images, is used to  extract the local gate interconnects: orange lines are M1  connections to VDD/gnd, green are gate fingers, blue are M1  connection between gates, red are CA input contacts to the next  gate, and yellow lines are higher level metal connections. Based  on the partial layout, a reverse engineered schematic of the  portion of the chip can be extracted with the gate connections  shown in Fig. 17. Finally, photon emission data, registered and  overlaid onto the BSE/BF-STEM images, can be used in  combination with the tester-based methodology to extrapolate  the logic state of the gates under different working conditions.


Fig. 15: Classifier algorithm identifies buffers (red) in both


(a) pattern and (b) emission mosaics.


Fig. 16: Static emission image is overlaid onto back side (a) BSE and (b) BF images to identify the logic state of the gate.


Fig. 17: Partial layout extracted from (a) BSE and


(b) BF-STEM images and (c) reverse engineered schematic.


In this paper, we have discussed a set of techniques and analysis  methodologies for the non-destructive and partially-destructive  reverse engineering and functionality extraction of complex  mixed-signal ICs with a special focus for security applications. Different advanced methodologies for tool automation, focusing, mapping, and image processing are also discussed in  the context of our proposed electro-optical tester-based  technique to significantly enhance the capabilities of existing  tools currently used to test, diagnostics, and failure analysis of  ICs. In particular we have proposed the use of front and back  side reflected light pattern images at different magnifications to  roughly identify circuit blocks. Time-integrated and timeresolved photon emission data was used to identify logic states  of individual gates, critical sequences of events, and functional  activity associated to specific test pattern and exercisers. Back  side plane view BSE and BF-STEM image mosaics were used  to reverse engineer individual gates and observe local metal  interconnects. Thermal imaging was used to aid in the  functional block identification and analog gates analysis that do  not show bright emission due to the reduced supply voltage.


Radiography (or x-ray inspection) is a ubiquitous technique to  all recent and upcoming counterfeit detection standards, including IDEA 1010A/B, CCAP-101, AS5553, AS6081, and  AS6171. X-ray inspection gives the user the unique ability to “see” what is inside an electronic component without  damaging it. To illustrate how x-ray images represent an  electronic component, Figure 11 (top) shows a simplified side  view diagram of a typical plastic molded part. The top view xray of a real plastic molded component is shown in Figure 11 (bottom). The dark regions in the x-ray image represent dense  areas in the component. Conversely, the light areas represent  less dense in the field of view. For this reason the area around  the component is represented in white. The x-rays traveling  through the different density areas of the component under  inspection cast a shadow onto the x-ray sensor. Thus this x-ray  imaging technique is also known as a shadowgram.


Figure 11 – Top: Cross section (side view) diagram.


Bottom: Top view x-ray image of epoxy mold compound  encapsulated electronic component


The following sections will describe the key features to look  for in the x-ray image when looking for counterfeit electronic  components. It is clear that prior to x-ray inspection we must  first assure that the markings on the components under  inspection show the same part number, place of manufacture, lot number, date code, and manufacturer. If at least one of  these identification descriptors is not homogenous throughout  the lot of parts, further investigation is needed to determine the  origin of the components.


Empty Package


One of the simplest – yet effective – techniques to make  counterfeit components is to start with an empty package  identical to the target. Obtaining such empty package is easy, as they are readily available in the market. Then, the proper  marking is applied to the top of these empty parts. To reduce  the chance of being detected, some criminal enterprises mix  the counterfeited parts with good ones, as seen in Figure 12. Another dangerous source of empty packages are component  fabrication facilities. There have been reports of “ghost” shifts  producing empty components with original markings on the  package – but with no active parts inside.


Figure 12 - Even though they look identical in the outside,


sometimes components are empty in the inside. These  images are 3D renderings of the internal structures of 2  components in the same lot. Left: Image showing


leadframe with parts inside. Right: Empty package


Lot Anomalies


The major challenge in the determination of a counterfeit  component is the usual lack of an exemplar that can be used as  a basis of comparison. For this reason, the most common  strategy used to assess the authenticity of an electronic  component is to perform the comparison within parts of the  same lot, as seen in Figure 13. This in-lot comparison is very  powerful because all parts within the same lot must be  identical. However, often time counterfeiters remark different  parts (that do not have identical x-ray images) to fulfill an  order. Even if you do have an exemplar available, it is also  common to find counterfeit components mixed with good  parts. That is the counterfeiters’ attempt to circumvent  detection by customers doing tests of just a few parts in the  lot. For this reason it is imperative to test all parts to assure  homogeneity within a lot. Until not long ago testing thousands  of components was cost prohibitive. However, recent  breakthroughs in the automation of radiography inspection  systems have made it possible the systematized inspection of  thousands of parts in trays, tubes, or reels in a cost effective  manner.


Figure 13 – Flow chart diagram on x-ray inspection for  component counterfeit detection


Figure 14 shows an example of lot anomalies. The x-ray  images on the top of Figure 14 are paired with the photograph  of the components on the bottom. It is clear in this example  that the fourth component from the left is empty.


Figure 14 - It is critical to inspect 100% of the parts – so  you don’t get fooled by criminals who mix bad parts with  the good ones. Can you tell which one doesn’t belong?


Differences from Known Good Sample


A common technique used to identify counterfeit components  using x-rays is to utilize an exemplar as a basis of comparison. The exemplar samples can be obtained in different ways. The  usual method includes the comparison to components in  previous lots that were obtained from trusted suppliers. In the  event that such a priori information is not available, you can  compare the part to another one currently in use. In this case, it is often necessary to x-ray the printed circuit board with the  assembled component. Both options, if available, must be used  carefully, as manufacturers can change the leadframe  structure, die size, and wire bonding schemes without notice. Therefore, it is imperative for the user to seek more  information on the part before judging it a suspect counterfeit.


Good Component Counterfeited Component


Figure 15 – Finding a counterfeit component becomes easy


if you have a known good sample to use as a reference


part. Check how different these two parts – found in the


same lot – look from each other. Good part on the left, counterfeited part on the right


Datasheet Discrepancies


This is a powerful technique because it can be applied to a  single component – no need to compare to the whole lot or to  compare to a known good sample. The check against the  datasheet can provide powerful insights about a component, as  we see in this example.


The layout of the lead frame and the wire bond diagram can  tell a lot about a component. To visualize this point, see the  component in Figure 16. On the left, you can tell where VDD, GND, and no connect (NC) pins are located. VDD and GND


have double wirebonds and connection to the lead pad, respectively. The NC pin is not connected anywhere in the die. Now check how they differ when overlaid with the part’s real  pinout (on the right). Instead of a GND connection on the  bottom right of the component, the datasheet points to a DQ3  connection. VDD instead VPP, and most telling, our NC  turned out to be the location for VDD. These anomalies cast a  big shadow of doubt on this component. Note that we were  able to perform this analysis with a single x-ray image of the  component.


Figure 16 – Left: best guess of the location of critical pins, like power and no connects. Right: Overlay of the


datasheet pinout onto the x-ray of the component showing  critical discrepancies


Missing Wire Bonds


Missing wire bonds are another critical sign of a counterfeited  component. Figure 17 (left) shows an example of a component  with missing wire bonds. However, at this point, we must  caution that aluminum wirebonds are not visible in the x-ray  image. For this reason, before assessing the authenticity of a  component based on the lack of wirebonds, first check with  the manufacturer if the part has aluminum wirebonds.


Figure 17 – Left: Suspect component without wirebonds. Right: Component with exposed wire bonds, showing  aluminum wires that are not visible in the x-ray image.


Internal Defects


This is a topic on the border of counterfeit detection and  failure analysis. In other words, are those defects present  because the component was counterfeited or because of  failures during the manufacturing process? The best answer to  this question lies on the definition of a counterfeit component: misrepresentation. The following example illustrates this  point. In Figure 18 we can see that one of the wirebonds in the  package is missing. This wirebond can be seen in the image on  the left, lying on top of a trace inside the leadframe. There is a  chance that this defect was caused during manufacturing, but  most likely it is a result of improper handling or storage of the  device. For this reason, although this information is  insufficient to assess the part’s authenticity, this defect should  raise many red flags.


Figure 18 – Suspect counterfeit components showing  internal damage to wirebonds


External Defects


Unlike the previous section, external defects are easier to point  to improper handling of a component. The example in Figure  19 shows a ball grid array (BGA) component with damaged  solder balls. This type of damage is common when  components are not packaged in the original tray, tube, or reel  provided by the original manufacturer. Even if the component  is deemed good by other tests, the fact that the parts are in the  wrong package makes them suspect counterfeit.


Figure 19 – BGA with damaged solder balls due to  improper storage


Consider that, for the parts to end up in this different package, they were removed from the original package and placed in  the non-conforming package. How to assure this process was  done following the proper procedures against electrostatic  discharge? How to assure these components were properly  stored while outside the original package? The fact we can’t  answer any of these questions leads us to classifying them as  suspect counterfeits.


Excessive BGA Voids


A profitable way to commercialize counterfeited components  is to pull them out of old boards, clean them, and then to resell  them as new. That’s exactly what happened to the electrolytic  capacitor example later in this paper. However, when  criminals pull ball grid array (BGA) components from boards, they need to have the parts re-balled.


The re-balling process is not trivial. The metallurgic interface  between the component and the new balls is no longer pristine (as it was when the first balls were applied onto the virgin  pads of the component). For this reason, it is common to find


counterfeited BGA components with excessive surface voids. As seen in Figure 20, the bare component shows a large  amount of voiding that indicates a part that was pulled and reballed. It is also important to note the abnormal shape of the  solder balls, which further validates the conclusion that this  part has been re-balled.


Figure 20 – BGA inspection analysis of bare BGA


component showing excessive voiding, a typical


characteristic of components that have been re-balled


Bent Pins


Another indication of improper storage of components is the  presence of bent pins, as seen in Figure 21. This x-ray  inspection can be done while the components are still inside  the tray, so they don’t need to be removed from the package  for a suspect counterfeit determination to be issued. Furthermore, not only trays of the wrong size are often used, sometimes the trays with the wrong material are used. In these  cases, instead of using the proper material to deal with ESD, counterfeiters replace it with lower cost options. These lower  cost option materials, unfortunately, can damage the parts.


Figure 21 - Components inside trays, tubes, and tape have  to be perfect. Suspect components with bent pins – that  usually means they have been handled outside the original  package


Excessive Die Attach Voiding


Electronic component manufacturers invest heavily in the  consistency of the products they sell. If you find a few of the  components within a lot with anomalous die attach voiding, like the one in Figure 22, suspect the overall quality of the part  and the lot. It may have been the result of an operation that  removed the die from the proper package to place it in another  package, thus creating an excessive amount of voiding.


Figure 22 – Component with excessive die attach voiding. The die is the rectangular object in the figure, while the  dark areas represent the location of the attach material


The assessment of the authenticity of an electronic component  must always be done with caution. Remember that inspection  techniques – like radiography, microscopy, and XRF – can  determine if a part is non-conforming. However, these  inspection techniques can’t determine that a component is  authentic.


For example, sometimes components with the same part  number are found to have different leadframes. Market  globalization led to the distributed manufacturing of electronic  components. Therefore, it is common for original component  manufacturers (OCM) to fabricate the same part number in  their multiple facilities. It is entirely possible that these  different locations procure different leadframes due to  relationships to their suppliers. It is also possible for a  manufacturing plant to change leadframes at a certain point in  time based on design and/or supplier changes. Unfortunately, most OCMs are not forthcoming with detailed information  about changes applied to their manufacturing process.


Another case we see often is to find components with the same  part number but with different die size. “Die shrink” is a term  often used in the semiconductor industry to refer to the  continuous miniaturization of integrated circuits. This means  that the same circuit can be implemented in a fraction of the  size of the previous generation of semiconductors. Thus, die  shrink is a natural consequence of the evolution of electronics  industry.  What it means to you is that it is possible to find  legitimate components with different lot numbers, date codes, and die sizes. The wire bonding diagram of these parts is  usually the same, but not necessary always identical.


Lastly, we may sometimes find good components with the  same part number that have different wire bonding diagram. As a consequence of die shrink, the power and signal  characteristics of different generations of the same component  can change. For example, it is possible that the earlier  generation of a part needed more power to bias larger  transistors. Thus, the multiple wire bonds needed to carry the  necessary current to bias an earlier version of the die may not  be necessary for the lower power later versions of the same  circuit.


The following examples illustrate that the determination of the  legitimacy of a component should not be done lightly. As we  discussed earlier, if the x-ray inspection shows that the parts  have different die sizes and/or leadframe structures and the  same date code and lot number, you can reject them as highly  suspect. However, if the date codes and lot numbers are


different, it does not mean that you are ready to assert their  legitimacy. Instead, this situation requires more research to  verify the traceability of the parts under scrutiny. The  following examples will help you identify when to call a  component non-conforming. These examples are not  comprehensive, but should assist you in the difficult task of  finding counterfeit components.


Samsung CMOS SRAM


The following example in Figure 23 shows the x-ray image of  a section of a reel of Samsung K6X1008C2D CMOS SRAM  with mixed leadframes and die sizes. This is a clear example  of a reel where good and bad parts have been mixed together  in an attempt to deceive a user doing sample testing of the lot.


Figure 23 –Top: Photo of a section of the reel, all


components show identical part number, date code, and  part number. Bottom: Overlaid x-ray image onto photo  showing mixed components


This is one example where the components went through a die  shrink, and as a result, the leadframe and die size changed. In  this example, all parts passed electrical tests. That’s because  they are essentially the same part. If left unchanged, these  components could be used in the field. However, counterfeiters adulterated the top of these parts to show the  same part number, date code, and lot number. To make things  worse, the criminals mixed all parts into the same reel of  components.


Tantalum Capacitors


The recent shortages of passive components (namely  capacitors, inductors, and resistors), led to a substantial  increase of their market value. The result of a higher market  value is a larger incentive for counterfeiters to enter the


market. Passive components, especially surface mount  devices, are particularly easy to counterfeit. Low tolerance  parts can be substituted by a lower cost part with the same  value. For example, a 1% 47nF capacitor can be replaced by a  lower cost 20% 47nF capacitor that looks almost identical to  its expensive counterpart. Furthermore, these parts often do  not have markings or any other types of mechanical  differentiators. In these cases, however, radiography can be  very useful.


Similar to the previous example, Figure 24 shows the x-ray  image of the section of a reel of tantalum low ESR capacitors  that have been remarked and mixed with standard tantalum  capacitors. In this example the x-ray image of the individual  capacitors was overlaid on top of the optical image of the  same parts. The inconsistency of the x-ray images, despite the  identical markings on the top of the parts, clearly shows the  presence of counterfeited parts.


Figure 24 – X-ray images of tantalum capacitors overlaid  onto photograph of reel of parts


The change in the value of a capacitor can have insignificant  impact on the functionality of the board. However, a change in  voltage tolerance can have catastrophic consequences, as we  see in the next example.


Electrolytic Capacitors


One of our customers, a large military original equipment  manufacturer (OEM) sent us a video of an electrolytic  capacitor exploding in one of their boards. We replicated two  frames of this video in Figure 25. This video was captured  after some of these boards failed during burn-in in the same  way. For this reason one of the engineers decided to document  the event by filming the explosion.


Figure 25 – Frames of a video showing the electrolytic


capacitors exploding while in use. Left: Frame right before  the explosion. Right: Frame showing the flames created  during the explosion


So how could we determine this was not some other quality  issue, and that indeed it was a counterfeit problem? First, this  was a mature design, which rules out a design issue. Second, they were able to correlate the explosion problem to a batch of  capacitors they bought from an independent distributor (ID). It  was the first (and likely the last) time the OEM bought parts  from this ID. Third, we were able to compare the counterfeit  capacitors with good capacitors mixed in the same lot of parts  acquired from the ID.


The photos in Figure 26 show the electrolytic capacitors in  question. A careful visual inspection of 100% of the parts in  the lot did not present any inconsistencies. Since they all look  identical from the outside, we were not able to determine the  legitimacy of these components using visual inspection.


Figure 26 – Visual inspection of electrolytic capacitors. No


anomalies encountered in these packaged components.


Left: A batch of counterfeited capacitors. Right: Single  counterfeited capacitor


The next step we took was to perform a 100% x-ray  inspection. On the left of Figure 27 you can see the reference  component capacitor – a component from a previous lot that is  a known good. The x-ray image on the right shows significant  structural differences from the one in the left.


Figure 27 – Left: Reference component. Right:


Counterfeited component.


The conclusive proof that these components were  counterfeited was determined when we found welding lines on  the leads of the suspect capacitors. The following high  magnification images in Figure 28 show the location of this  welding line. This feature was not detected in the visual  inspection because it is too close to package of the capacitor, and in some instances inside the plastic package. This is a  typical finding in components that have been pulled from  discarded boards. These parts have short leads since they have  been mounted on a board, soldered, and trimmed. As a result, when counterfeiters want to commercialize used parts pulled  from old board, they weld new leads to the stubs of the pulled  component. After that, they apply a layer a tin solder (process  also called re-tinning) to give the component a homogeneous


shiny finish. That’s the reason why the visual inspection did  not find any issues with these parts, but the x-ray inspection  was able to clearly find them.


Figure 28 – High magnification images showing the welded


leads of the counterfeited component. Left: Reference


component. Right: Counterfeited component.


The cost of repairing the boards that failed during burn in is  minimal when compared to the cost of replacing the boards in  the field. Unfortunately, the cost of replacing deployed boards  usually comes with other associated costs - costs that go far  beyond the monetary liability and include the damage to  reputation and the potential loss of lives. Those can lead to the  demise of an otherwise reputable corporation.


The continuous miniaturization of electronic components has  created increasing challenges to the overall failure analysis  and quality inspection of such devices. In this paper we  reviewed state-of-the-art algorithms to improve the resolution  of x-ray images (WISE) and to compare x-ray images (ICARUS). These algorithms, when used in tandem, are  powerful tools to detect counterfeit electronic components. The case studies presented show how x-ray inspection, when  assisted by the correct techniques and algorithms, can be an  efficient method in failure analysis, quality inspection, and  counterfeit detection of electronic components.


[1]! K. Sayood, Introduction to Data Compression, Morgan  Kaufmann, 2000.


[2]! P. P. Vaidyanathan, Multirate Systems and Filter Banks, Prentice Hall, 1993.


[3]! Donoho, D., et al. “Density Estimation by Wavelet  Thresholding”, Technical Report, Dept. of Statistics, Stanford University, 1992.


Materials analyses for parts validation


W. John Wolfgong, James Izzo


Raytheon Company,


Space and Airborne Systems, McKinney, TX, U.S.A. wolfgong@raytheon.com, 972 952-3158


The most common methodologies for determining  whether a component should be judged suspect counterfeit, or  not, rely on visual examination, electrical test, and X-ray  examinations. While these are commonly sufficient at such  determinations, more thorough examinations may be pursued - in particular materials characterizations.  In this paper, examples are given in which such “non-standard” methods are  employed.  Additionally, the results of an investigation as to  the applicability of such methods towards detection of surface  alteration to facilitate repackaging are described.


The passing of counterfeit goods as legitimate is  obviously a well-known and very profitable practice. In many  cases, such as production of currency and increasingly during  pharmaceutical production [1], steps are taken to thwart  counterfeiting before products make it to market. Additionally, in such cases, it is common that manufacturers build in  markers for counterfeit detection such as the use of metal  bands in US paper monies. While there has been increasing  discussion of designing electronic components with such  counterfeit avoidance technologies [2], most all materials  currently in the market place have no such built in safe-guards. Additionally, such methods could prove cost prohibitive for  inexpensive components.


(3)


The DCT and its inverse (IDCT) are defined in Equations (4) and (5) respectively.


(5)


)5.0


)(5.0


cos


%&'


Data filtering of a given signal f(n) is successful when the  redundant and noise components of f(n) are reduced or  removed in the frequency domain. The signal )(ˆ nf  is the  filtered representation of f(n). The following section describes  how thresholding for data compression and noise suppression  can be applied to the frequency coefficients of the original  radiographic signal.


DFT, DWT,  or DCT


ˆ nf


IDFT, IDWT, or IDCT


Figure 5 – Thresholding of frequency coefficients


Adaptive Threshold


For the case of a signal corrupted by additive white Gaussian  noise (AWGN) with variance σ2, reference has shown that the  optimal threshold is given by:


)1


ln(


.2 −


σ


τ


(6) This “universal” threshold τ is applied to radiographic data  corrupted by WGN. In the threshold approach all transform  coefficients smaller than τ are set to zero. All coefficients  greater than τ are kept the same:


...0


),


,0


"#"$%


≥


<


(7)


This approach is referred to as a hard thresholding technique. In the above equation


W f represents the frequency  coefficients of the radiographic signal f(n), while


ˆ nW f  is the  set of frequency coefficients used in the IDWT, IDCT, and  IDFT. Figure 6 shows the input/output mapping for the hard  thresholding case.


-1 -0.8 -0.6 -0.4 -0.2 0 0.2 0.4 0.6 0.8 1  -1


-0.5


−τ


ˆ nW f


( n


W f


Figure 6 – Hard thresholding rule.


Parameter Estimation Technique


The parameter estimation method is based on the CWT to  estimate the parameters of the x-ray signals. The CWT  performs a correlation of the kernel wavelet with the input  signal [3]. The CWT is defined in Equation (8).


∫


dt


).


ψ


(8) In WISE a modified wavelet kernel is introduced to closely  match the shape of the radiographic signals.


This kernel includes several parameters that are optimized to  maximize the correlation between the radiographic signal and  the wavelet kernel. This algorithm allows better correlation, and consequently improves parameter estimation.


The performance of the thresholding technique applied to the  DWT, DFT, and DCT coefficients is shown in Figure 7. This  figure shows the relative energy compression ratio  performance in radiographic experimental data. Since the  DWT kernel resembles the x-ray signals, it offers better data  compression compared to the DCT and DFT.


Figure 7 – Compression ratio performance with  experimental data


The parameter estimation technique is applied to the noisy  version of image in Figure 8 (left), while the reconstructed  image is shown in Figure 8 (right).


Figure 8 – Before and after of WISE. Left: original image. Right: reconstructed image with WISE.


The signal-to-noise ratio (SNR) of the signal is 6dB. In this  example the parameter estimation technique is able to  correctly isolate the x-ray signals of the radiographic image. A  total of 35 coefficients are necessary to reconstruct the original  signal with a SNR of 36dB.


Another example of the level of image improvement achieved  with WISE is seen in Figures 9 and 10. Figure 9 is the original  x-ray image of a semiconductor, while Figure 10 shows  several of the details that were not clearly visible in the  original image in Figure 9.


Figure 9 – Original X-ray image of semiconductor


Figure 10 – X-ray image of semiconductor in Figure 9  after WISE


Detection of Counterfeit Components


The recent escalation of electronic parts counterfeiting on the  world stage comes in tandem with a sharp increase in the  technical sophistication of this criminal enterprise. This  escalation has also increased the demand for counterfeit  detection techniques at each and every point in the supply  chain. The resulting paradigm shift led to a higher aggregated


value of the distribution chain. As a result, a suite of  inspection techniques has replaced the once appropriate and  sufficient visual attribute analysis practiced a decade ago. The  information contained in this section provides independent  distributors, contract manufacturers, authorized distributors, original equipment manufacturers, original component  manufacturers, and government agencies with an overview on  the use of radiography in the detection of counterfeit  components. The positives and pitfalls of this powerful  inspection technique will be reviewed. Instead of pursuing an  in-depth view of radiography, the focus of this work is the  overall strategy utilized in the identification of counterfeited  parts.


In the formulation of this strategy, it is important to note that  radiography is one of several tools needed in the arsenal  against counterfeit components. Among the other techniques  needed in the search for fake parts are visual inspection, resistance to solvent immersion, decapsulation, x-ray  fluorescence (XRF), and electrical testing. None of these  techniques alone can tell you that a part is authentic. As a  matter of fact, these are not authentication techniques. Instead, they are anomaly detection techniques. That’s a subtle but  crucial difference to keep in mind. However, these different  tests and techniques independently create “lines of defense” that can tell you if a component is a suspect counterfeit. In  order of effectiveness, we recommend starting with visual  inspection, then x-ray, decapsulation, XRF, and if needed, electrical testing.


Other advanced techniques have been explored, and include  ultrasound, scanning electron microscopy, thermogravimetric  analysis, differential scanning calorimetry, and thermomechanical analysis. Although not routinely used in the  detection of counterfeit components, these advanced  techniques have shown to be useful in challenging cases of  component authenticity assessment.


Currently, “state of the art” detection methodologies  rely primarily on visual examination, X-ray examination, and  electrical test. While fully sufficient in most cases, these  methods may still fail to identify counterfeit components. In  such cases, use of additional techniques can be utilized to  further characterize components for counterfeit detection [3]. For example, with mission critical, high risk, and/or high cost  components such extra investigations may be warranted.  Of  such possible applications, materials analyses for parts  verification or alteration comprise the remainder of this paper.  Only a few of the more common methodologies are discussed  and examples are given.


Identification of the construction materials which  comprise electronic components is an attractive target to help  identify suspect counterfeits. Such identifications can be used, for example, to identify if the materials used to construct a  part are consistent with an authentic component. They may  also be used to determine if a part has been altered by  remarking (e.g.  identifying different inks than those originally  present).


In such cases information concerning the material  compositions of authentic parts must be known. Such  information can be gained from parts specifications, discussions with manufacturers (particularly when a part is  suspected of being counterfeit), and comparison to known  authentic parts – so called golden standards. When identifying  that a material is different than specified, or even from a  known authentic part, care must be taken to ensure such  differences are not accounted for by acceptable manufacturing  changes. This highlights the often complicated interpretation  of data generated in general and not just from materials  identifications, during suspect counterfeit investigations.


In addition to analyses for construction materials  identifications, such methods may be employed to determine if  parts have been altered by detection of constituents such as  sand-blasting media, residual cleaners, and others.


There are a number of analytical techniques for  materials identifications and the choice of such methodologies  will commonly result from several factors such as: cost, the  ability to provide sufficient data for a specific need, simple  availability (does the analytical lab happen to have the  requisite equipment?), sample considerations such as  destructiveness (will the testing result in alteration of the part  or will it damage a part is some way?), and a host of others. In  the following examples, only more common methodologies  are discussed.


Procedure


A tale of two parts:


During a “non-franchised” parts investigation the lab  was presented with two components which had very detailed  materials specifications in the part drawings (nominal amounts  of various construction materials were listed). One of the  devices had the composition values listed as shown in Table 1 ,Part 1 column, while the second had those shown in Part 2  column.


Table 1 – Construction Material.


Construction


material


Part 1


Part 2


Bond wire


100% Au


>99.99% Au


Die


attach


adhesive


epoxy


(14.6%), silver filler(85.4%)


epoxy(15%), silver  filler(82%)


Lead frame


Cu(97.5%),Fe(2.3%), Zn(0.15%)


Cu(97.4%),Fe(2.3%)


Zn(0.17%)


Mold compound Sb(asSb2O3)(1.9%), Br(0.85%),


silica(75%),


resin(22.2%)


Sb(as Sb2O3)(1.5%), carbon black(0.3%), bromophenol


phenolic(2.5%),


silica


(80.7%), phenolic(5%),


epoxy resin(10%)


Lead


frame


plating


Pb(15.1%),Sn(84.9%)


>99.99% Sn


Semiconductor  device


Si(100%)


Most of the requirements listed in the table can be  addressed using Scanning Electron Microscopy/Energy  Dispersive Spectroscopy (SEM/EDS) and was the method of  choice for characterizing many of the materials. Quantitative  analyses were performed using a 20 kV electron beam and the  system was calibrated to copper.


Part 1 was found to be consistent with the specified  composition as listed in Table 1. For example the mold  compound was found from EDS quantitative analyses to be  composed of 73.6% silica, 1.2% antimony trioxide, 0.49% bromine, and resin as the remainder (Figure 1). Note that these  determined values are low when compared to those of the  nominal specifications (Table 1). However, such findings were  deemed acceptable because of the nature of the analysis. For  example, the following rationale was applied: the specified  values are nominal only, EDS analyses of inhomogeneous  materials such as this produce poor quantitative results, the  value of oxygen was erroneously high which is typical of such  EDS analyses and results from adsorbed waters lowering  overall levels of other detected elements, qualitatively  identifying that the specified materials were present while  quantitatively showing  they were “in the ballpark” is all that  could be expected and more intensive quantitative analyses  would have represented significant added costs not deemed  necessary with these low risk parts.


Figure 1 – Area of analysis and elemental spectrum of  package molding.


Note that the specifications require a nominal  concentration of bromine of 0.85%. Bromine is commonly  added to molding in the form of appending bromine atoms to  the backbone of epoxy resin molecules as well as addition of  organic bromine containing compounds [4]. Detection of  bromine using EDS methods can be complicated by an  inconvenient overlap of the primary aluminum band at the  same approximate energy.  While there are methods to resolve  this ambiguity, it is accomplished with less confidence when  these elements are detected at low levels as was the case here. As a result, and to further characterize the molding compound, pyrolysis Gas Chromatography/Mass Spectrometry (GC/MS) was also employed.


By exposing a sample of the encapsulant to  pyrolyzing conditions, 3 mg - 750C for 20 seconds, unambiguous identification of bromine containing compounds  is possible. Additionally analysis of the types of compounds  detected can yield insights into the molding compound  chemical structure.


For this example detection of hydrogen bromide was  deemed sufficient to establish the presence of bromine in the  encapsulant. As this compound entered the MS from the GC at  the same time as many other small molecules, high resolution  exact mass methods were employed to unambiguously assign  bromine as present in the sample.


Figure 2 - Mass spectrum collected at 1.21 minutes after  introducing the sample into the MS.


As shown in Figure 2, a number of masses are


present that are close to 79, 80, 81, and 82 amu; this results


from the complex nature of the materials introduced into the


mass spectrometer. However, only those with the exact masses


listed can be assigned to bromine and simple compounds


thereof. The following tabulated data compares the observed


masses to theoretical –


Table 2 – Exact mass determinations showing that the molding


is brominated.


Measured      % Base    Formula                            Calculated


Mass                                                                          Mass       (Error, mmu


from calculated)


78.91479       68.5%    Br                                          78.91833      -3.5


79.92149       23.1%    HBr                                        79.92616      -4.7


80.91388       60.8%    81Br                                     80.91629      -2.4


81.92325       29.3%    H81Br                                  81.92412      -0.9


While the molding compound specified only “resin”,


the material listed for the die attach was more specific


indicating generically that the binder be composed of an


epoxy. EDS analyses showed that the silver content was


approximately 82% which is in good agreement with the


specifications. However, EDS analysis cannot determine that


the binder is in fact an epoxy. A more molecular information


rich method is necessary. Fourier Transform Infrared (FTIR)


spectroscopy was chosen for this part of the investigation and


a spectrum was easily recorded using reflectance methods


employing a microscope spectrometer attachment.  The


infrared spectrum, displayed in Figure 3, is fully consistent


with an epoxy resin indicating that the component is in


compliance with nominal materials specifications.


Figure 3 – Die attach binder.


All other materials were shown to be consistent with  the nominal materials specifications using SEM/EDS methods.


Comparison of the specifications listed in Table 1  show that the two are quite similar (these are not “exotic  parts” and such compositions are in fact common). However, during parallel analyses, using the same methodologies as  described in the previous sections, two distinct nonconforming materials were identified; in particular the  molding compound and the lead finish.


Figure 4 - Elemental spectrum of molding compound, part  two.


As shown in Figure 4, only carbon (C) oxygen (O) and silicon (Si) were detected in the elemental spectrum of the  molding compound of part 2. Conspicuous by their absence  are peaks indicating the presence of antimony (Sb) or bromine (Br).  This indicates that the molding does not contain the  brominated phenolics or antimony trioxide as specified. In  addition to this EDS analysis, the sample was also subjected to  the same pyrolysis GC/MS methods as were applied to sample


1. Detection of bromine and its compounds were not  accomplished, which unambiguously shows that the molding  does not meet the specifications as stated in Table 1.


In addition to the molding compound not meeting  specifications, the lead frame plating was also shown  deficient; it is composed of a tin/lead finish and not pure tin.


Figure 5 – Lead finish of part 2 area analyzed and  corresponding spectrum.


Quantitative analysis showed that in this case the lead  content was about 16% actually making it a good match for  specifications of part 1.


These two examples were chosen to show that  materials analyses can be employed as part of suspect  counterfeit investigations in cases which details of  construction materials are known and to highlight common  laboratory techniques to these ends. When materials  mismatches are found the likelihood of a component being a  counterfeit is heightened and further investigation is typically  warranted such as determining if these differences are due to  acceptable materials changes.


Part II – evaluation of methods to detect part alteration.


Evaluations of methods aimed at detecting if parts  have been sand-blasted, this is a common technique to  facilitate repackaging, have been performed by the SAE G-19  counterfeit electronic parts committee of which the authors  participated. In these experiments multiple techniques were  evaluated including physical inspection methods to discern if a  package had been altered via sand-blasting.  The goal was to  evaluate the application of Raman and FTIR spectroscopies to  the detection of residual blasting materials which may remain  embedded on the package surface.


A number of part types, such as typical ICs and metal  can devices, were blasted with a variety of common blasting  materials including alumina, walnut shells, glass beads, sodium carbonate, and plastic beads. While there was  difficulty in identifying impregnated blasting material


remnants, it was discovered that in many cases traces of the  materials remain in package crevices such as at the base of  leads. Additionally, residuals of inks originally on the  packages could be identified.


FTIR methods proved cumbersome and hindered by  sampling limitations of the method. However, the application  of Raman spectroscopy was shown a viable technique in many  cases.


Raman spectroscopy has long been applied to  detection of counterfeits with regards to the art world [5]. This  results largely from the method’s unique capabilities to  characterize paint pigments. It has been shown that this  approach is also applicable to detection of pigments of inks  applied to electronic components [3]. The challenge in this  case was to show its applicability to the detection of residual  blasting materials.


Figure 6 – Particles concentrated at base of leads.


Figure 7 – Glass beads retained after blasting.


Figure 8 – plastic blasting beads impregnated into lead  package interface.


Figures 6 – 8 show that blasting materials may be  retained by a component after blasting. It can be surprising  how tenacious these particles could be with remnants retained, in some cases, even after post-blast cleaning.


Raman spectroscopy proved effective at identifying   glass, alumina, plastic, and sodium carbonate blasting  materials used for these experiments “as is” on the parts  without manipulation – that is bead remnant samples were not  removed from the parts. Of the part types, metal cans proved  the most difficult; however, in a few cases retained particles  could be detected. Finally, in some cases remnants of inks  supposedly removed during the blasting procedure were also  detectable.


2000  2500  3000  3500  4000  4500  5000  5500  6000  6500  7000  7500  8000  8500  9000  9500  10000  10500  11000  11500


2000


2500


3000


3500


cm-1


Figure 9 - Raman spectrum of residual ink.


The spectrum in Figure 9 shows that a titanium  dioxide filled epoxy ink was on the package prior to blasting  and detectable levels remained. In cases of determination if  packages were remarked, detection of such barely perceptible  inks (these were obvious only under high magnification in the  Raman microscope) could indicate remarking; particularly if a  second dissimilar ink is present as the new marking media.


1.5


2.0


2.5


3.0


3.5


4.0


4.5


5.0


Figure 10 – Raman spectrum of alumina particles (collected  using a 532 nm laser).


As displayed in Figure 10, alumina produces a  particularly strong response when probed using a 532 nm  laser. As such it is easily detected.


1200  1400  1600  1800  2000  2200  2400  2600  2800  3000  3200  3400  3600


Figure  11 – Raman spectrum of glass beads.


As opposed to alumina, glass does not produce a  particularly strong Raman response; however, as shown, Figure 11, it can be detected when present as residual blasting  beads.


18000  20000  22000  24000  26000  28000  30000  32000  34000  36000  38000  40000  42000  44000  46000  48000  50000  52000  54000  56000  58000  60000


Figure 12 – Polymer beads remnants were easily detected.


Figure 12 shows that the polymer beads were easily  characterized using Raman methods.


-4000-3000-2000-1000  0  1000  2000  3000  4000  5000  6000  7000  8000  9000  10000  11000


Figure 13 – Raman spectrum of carbonate salt.


The carbonate blasting remnants were detectable but  proved difficult as evidenced by the poor signal to noise in the  spectrum displayed in Figure 13. Additionally, of all the  materials tested, this salt is the only one that is water soluble  and could conceivably be easily removed using simple water  rinses.


The experiment using walnut shells did not result in  quality spectra when analyzed using Raman methods. This  resulted from the materials poor Raman response. However, in  this case FTIR spectroscopy was shown to be an effective  method.


The data presented here show that materials analyses  can play a role in counterfeit component detection. While the  methods presented are certainly not exhaustive, with a host of  other approaches also applicable, they are certainly capable of  addressing many materials characterization applications for  suspect counterfeit detection.


[1.] L. Walet, "Fighting Fake Drugs" Chem.  Eng. News, 93 (8), 28 - 29 (2015)


[2.] L. Greenmeier, "Shorted Circuits: Pentagon Looks to  DNA from Plants to Foil Electronic Component  Counterfeiters, Scientific American, April 18 2012


[3.] W. Wolfgong, J. Izzo, M. Depriest, Detection of  Counterfeit Components",  Circuits Assembly, March 2012


[4.] E. Weil, S. Levchik, "A Review of Current Flame  Retardant Systems for Epoxy  Resins", Journal of Fire  Sciences, 22 (1), 25 - 40 (2004)


[5.] P. Vandenabeele, L. Moens, H.  Edwards, R. Dams, "Raman spectroscopic database of azo pigments and  application to modern art studies" J. of Raman Spectroscopy, 31 (6), 509 - 517, (2000)


In-Line Detection of Deep Trench Moat Underetch Defects Using eBeam Inspection


Richard F. Hafer, Xiaohu Tang*, Brian Messenger, Mark T. Dekker, Oliver D. Patterson Shuen-Cheng Lei*, Yi Feng


GlobalFoundries


2070 Route 52


Hopewell Junction, NY 12533, USA *Hermes Microvision Inc.


1762 Automation Pkwy


San Jose, CA 95131 USA


I. INTRODUCTION


E-beam Inspection (EBI) is commonly used for in-line  detection of defects in semiconductor manufacturing. EBI  historically has been used mostly in the voltage contrast mode, but recently due to resolution limitations with other inspection  techniques and improvements in EBI capability, physical  defect inspection mode applications have grown in popularity [1, 2]. The superior resolution of EBI enables (1) detection of  very small physical defects as well as (2) sufficient quality  defect images for automatic defect classification, to separate  out defects of interest (DOI) from nuisance defects. This  allows the inspection to be run at low signal-to-noise so that  more real DOI can be captured.


Voltage Contrast (VC) inspection is characterized by high  throughput using large pixel sizes and capability to scan large  areas, up to and including a whole 300 mm wafer in less than  75 minutes [3, 4]. On the other hand, physical defect  inspection is characterized by small pixels and low throughput  due to much lower signal-to-noise ratios. Physical EBI is used  in situations where a defect of interest is not easily detected  with other inspection techniques and will not cause a VC  signal. The ability for EBI to detect physical defects has  further improved with the introduction of high-energy  columns (5 keV and above), previously limited to 3 keV [5, 6]. This extends EBI’s capability to detect buried defects, provides a sharper image for many physical defects, and can  help in cases where wafer charging is a factor.


This paper highlights a physical defect mode application  where traditional defect inspection techniques, such as broadband plasma (BBP) and dark field inspection were ineffective  in finding the DOI. In this application, the device is built on  Silicon on Insulator (SOI) substrates. While processing with  SOI substrates is more complicated, benefits include higher  performance due to reduced junction capacitance, lower  operating voltage, denser layout, and the availability of highdensity memory in the form of DRAM embedded in the same  substrate as the processor, called Embedded-DRAM (eDRAM).


GlobalFoundries (previously IBM Microelectronics) implements eDRAM using deep trench capacitors. Holes  called deep trenches (DT’s) are etched through the SOI, then  through the buried oxide (BOX), and finally deep into the  substrate. These are filled with a dielectric and then a


conductor which becomes the top plate of the capacitor.  An  N+ doped silicon region underneath the BOX forms the  bottom or buried plate. The N+ doped silicon underneath the  BOX starts out as one large electrical node, but can be broken  up into multiple nodes using a feature called a DT MOAT or  MOAT to isolate the cathodes of the DTs from each other. They are formed by etching a rectangular trench that extends  through the BOX and the buried plate into the P- doped  substrate. This rectangular trench is filled with dielectric and  conductor similar to the DTs. A SEM cross-section, top down  physical schematic, and cross-section electrical schematic are  shown in Figures 1a-1c.


Figure 1a:  SEM cross-section of MOAT structure.


Figure 1b: Top down schematic of a MOAT


Figure 1c: Cross-section schematic of MOAT isolation (not correct aspect ratio)


Sometimes the MOAT etch does not etch properly through the  BOX, resulting in a shallow moat, causing high leakage from  the inner buried plate to the outer buried plate as shown in  Figure 2.  Riso should be in the Gohms range, but is much  lower when one of these defects is present.  This leakage may  kill the circuitry for certain products.  A characteristic of these  defects is that the BOX near the wafer surface is narrower than  desired, shown in Figure 2, causing the MOAT to be more  shallow in that particular location. This narrowing is visible  from the wafer surface using a very small inspection pixel  size.  This defect type was of primary interest for a recent  GlobalFoundries/IBM technology.


Figure 2: Schematic of shallow MOAT, defined as a  defect (not correct aspect ratio)


The problem of leakage across the MOAT isolation was first  detected at Module Test, which occurs many, many process  steps after MOAT etch. Failure Analysis found that failing  structures had under-etched locations in the MOATs.


The eDRAM and MOAT modules are the first modules in the  semiconductor process whereas Module Test occurs after the  semiconductor processing is complete. Feedback on the  existence of these defects was on the order of 6 months.  This  large delay presented an unacceptable risk to work in progress (WIP). An in-line electrical test (ILT) was then implemented  after metal 1 which reduced this delay by 50%.  This  improvement was helpful, but real implementation of an inline inspection was necessary to reduce the delay to an  acceptable level.  The reduction in Mean-Time-To-Detect (MTTD) between root cause and detection point is important  in three ways:


1. The amount of defective WIP involved in an  excursion is reduced.


2. Customer deliveries are far more predictable.


3. Cycle time of experimental learning intended to fix  the problem is far faster.


Unfortunately, both BPP and dark field inspection techniques  were not particularly effective in detecting the shallow  MOAT. In one deep-dive comparison of techniques for this  defect, EBI identified 95% of defective die, whereas darkfield identified 40%.  While 40% sounds reasonable, it would  not provide nearly as strong of a correlation to ILT.  This is  also a best case number after a lot of recipe work, and for a  routine inspection there would be a significant proportion of  nuisance defects.  This would require SEM review sampling, which would further reduce capture rate and increase cycle  time.


The explanation for this difficulty rests on the geometry and  spot size for the darkfield inspection.  The laser is incident  from an oblique angle to the wafer, and scattered light from a  defect or other source is detected.  Because the darkfield  source meets the wafer at an oblique angle, the DOI most  effectively scatters light when the laser is parallel with the  trench.  The trench that is perpendicular to the incident laser


‘hides’ any defects.  This reduces sensitivity for this geometry


of MOAT, and so to maximize sensitivity it would require 2  scans (increasing throughput).  EBI incident electron beam is  perpendicular to the wafer, and so does not have a geometry  sensitivity, and so can inspect in one scan.


The second contribution is the signal to noise ratio.  The pixel  size for the EBI scan is 25 nm, and thus 12 pixels cover the  width of the MOAT which is approximately 300nm.  The  details of the darkfield signal to noise are outside the scope of  this paper, but the contribution from the larger pixel size, scattering from both the defect and trench, and scattering from  the surrounding structures all contribute to a very difficult  inspection with high nuisance rate.


An EBI inspection was then developed for this purpose.  This  reduced the time to detect to approximately 5 days.  Section II  describes the inspection setup and verification with failure  analysis.  Section III describes application of the technique.


II. INSPECTION SETUP AND FA VERIFICATION


During the EBI inspection, images of subject die are  compared to two adjacent die. If a significant difference is  detected, the location is recorded as a possible DOI. An  example of the MOAT defect is shown in Figure 3. This  inspection uses 25nm pixel size and multiple pixel averages  to achieve the resolution necessary to detect this defect type.


The inspection conditions are 1 keV landing energy, and 0 V  extraction voltage, at a 25nm pixel size.  The 1keV landing  energy was found to be optimal by comparing imaging on a  particular DOI.  The comparison of different landing energies  versus DOI contrast is shown in Figures 3a-3d.


A more positive extraction field would generally be used for  better contrast, but because the defect is below the surface  plane of the wafer the contrast difference between the surface


and DOI was not improved.  The brightness/contrast is set to  make the trench edge as bright as possible to highlight the  DOI.


A 25nm pixel size was used because it was found to be the  largest usable pixel size (to increase throughout) while still  maintaining sensitivity to the DOI.  We found no helpful  effect for the inspection from prescan charging on this SOI  product.


Figure 3a:  300 eV landing energy; defect barely visible.


Figure 3b:  500 eV landing energy; defect visible.


Figure 3c:  1000 eV landing energy; defect more visible.


Figure 3d:  2500 eV landing energy; defect visible.


The width of a nominal trench is approximately 300 nm.  With a 25nm pixel size, we have 12 pixels to characterize the  trench.  The field of view (FOV) is 2000 pixels.  For our


MOAT structures we use approximately 10 FOV’s per


structure, see Figure 4.  Note that the Care Area is only the  MOAT and everything else in the FOV is filtered out (the  Care Area is defined as the area of interest where defects are  to be reported; Don’t-Care Areas may be in the FOV but  defects are not reported from these areas).


Figure 4:  Step and Scan pattern over the MOAT.


After the inspection is complete (Figure 5a), a high resolution  image of the defect is captured for disposition as shown in  Figure 5b.


Figure 5a: (Top) In-line, top-down inspection image of  defect, (Bottom) inspection image of reference.


Figure 5b: HR EBI image of the DOI.


The throughput of this physical-mode inspection is limited  because of the resolution requirements, but fortunately just  the actual MOATs need to be scanned. If the critical  ~100  um by ~300 um MOAT structure is scanned, the inspection  time is on the order of 30 minutes per wafer. In a recent case, this equates to ~1,000 fields of view. For a review SEM or  manual SEM, the operator input would have to inspect 1,000  images (or a sample thereof).  Finding the DOI on a wafer  manually using a review SEM would take many more hours  with a high probability of missing a defect.


Failure analysis was used to verify that the defects detected  with EBI correspond to the MOAT under-etch which had  caused the module electrical failure. Figure 6 shows FIB  cross sections of bad (Figure 6a) and good (Figure 6b) MOATs as they transition through the BOX.


The SOI and BOX, and Silicon Substrate are labeled and are  part of the final device.  The layer above the SOI is a etch  hardmask, which is part of the process but not part of the final  device, and the MOAT liner is also shown.  Additionally, there is an analysis film decorating the MOAT which is part  of the Failure Analysis process and not part of the standard  process.


The immediate area of the MOAT opening through the box is  shown in Figures 6a and 6b. The opening in the BOX is much  narrower for the defective site and translates into a narrower  MOAT. This in turn limits the MOAT etch so that the MOAT  is also much shallower at this location and does not reach the  bottom of the N+ buried plate region.


Figure 6a: Cross section SEM. Defective site. The MOAT  penetrates ~2 um into the substrate (not shown)


Figure 6b: Cross section SEM. Good site.  The MOAT


penetrates ~5 um into the substrate (not shown)


III. PROCESS MONITORING AND EXPERIMENTAL


This inspection was implemented as a process monitor to  detect excursions.  Initially, the amount of process “ON” time  after an etch-chamber parts change (“conditioning”) was  identified as the main factor in MOAT defectivity. This was  found by correlation to Module Test, but the trend was  duplicated with the EBI inspection but with a much faster  MTTD. Defectivity was high immediately after a parts  change, but decreased with processing time, see Figure 7. Thus initially the EBI inspection was used to qualify a


“conditioned” etch chamber. However, in a manufacturing


environment this sometimes unpredictable and wasteful  waiting time needed to be reduced.


Figure 7:  Chamber defectivity before and after parts  change.


Therefore, EBI inspection was used to study ways to eliminate  high yield loss immediately after parts changes.  In one  experiment, wafers were split between a known-good “Reference” chamber, a known-bad chamber with the “POR  Process”, and an “Improved Process” in a known bad  chamber.  The results are shown in Figure 8.  This plot also  includes the ILT results which were collected later to show the  good correlation between these metrics.  The ILT MOATLeakage Yield is a binary pass/fail metric based upon several  parameters but is largely influenced by MOAT leakage. As  can be seen, the “Improved Process” has much higher yield  than the POR Process, mitigating the effect of the chamber  conditioning.


Figure 8: EBI Predicted Yield versus ILT Yield.


Defective Etch  through SOI


Figure 9: Presence of defect versus Maximum Leakage


The correlation between EBI defect detection and leakage at


ILT was further investigated by looking at each individual die


and the leakage associated with the MOAT only, see Figure 9.


For each die, the presence of a defect is plotted on the x-axis


and the maximum leakage (with compliance at 1000) is


plotted on the y-axis.


As can be seen, the data fall into 3 categories. First, the True


Negative (927 die), where no defect is observed and the ILT


leakage is low. Second, The True Positive (83 die), where a


defect is observed and correctly predicts high leakage at ILT.


The 83 data-points are all stacked at the compliance limit of


1000.  Third, the False Negative, where no defects were


detected but the leakage was increased (58 die, 55 of which


were at compliance). The increased leakage in the Third group


could be due to (a) another process factor further in the process


than MOAT etch, or (b) a MOAT defect that was missed


during the EBI inspection.  Note that there is no occurrence of


a false positive, where hypothetically EBI predicted a defect


but ILT did not see a defect.


The fast EBI inspection was also used as a line monitor, to


catch excursions and to predict ILT Yield. Figure 10 shows


120 days of production wafers and experiments that had both


EBI and ILT data (111 data points). The correlation between


EBI Predicted Yield and ILT leakage-yield is very good,        R2 = 0.95.


Figure 10: Correlation of EBI defect detection and ILT  Yield for 120 days of volume production.


IV. CONCLUSIONS


This paper presents a case-study that shows EBI can be used  for in-line detection of very challenging physical defects. This  inspection can be used for rapid evaluation of hardware. Previously this defect type could only be monitored at module  test, which occurs many days later in the process sequence. Ebeam inspection enables much earlier detection of excursions  as well as faster evaluation of split experiments. Defects that  were captured were verified with cross sections as well as  correlation to ILT results.


V. ACKNOWLEDGMENT


This work was performed as part of the IBM Microelectronics, Semiconductor Research & Development Center, Hopewell  Junction, NY 12533. Thanks to S Darling for Failure Analysis  work and Ryan Kelly, for in-line electrical test data and  expertise.


VI. REFERENCES


[1] O. D. Patterson, J. Lee, D. Salvador, S. C. C. Lei, X. Tang “Detection  of Sub-Design Rule Physical Defects using E-Beam Inspection”, IEEE  Trans on Semiconductor Manufacturing, Nov 2013.


[2] O. D. Patterson, D. A. Ryan, X. Tang, S. C. Lei, “Rapid Failure  Analysis of Low-Yielding Electrical Test Structures Using E-beam  Physical and Voltage Contrast Inspection”, Proceedings of ISTFA, Nov 2013.


[3] R.F. Hafer, O.D. Patterson, R. Hahn, H. Xiao “Full-Wafer Voltage  Contrast Inspection for Detection of BEOL Defects”, IEEE Trans on  Semiconductor Manufacturing, To Be Published Nov 2015.


[4] B. Donovan, O. D. Patterson, W. Chang, N. Arnold, B. Messenger, O. J. Kwon, J. Liu, R. Hahn, “Early Detection of Electrical Defects in  Deep Trench Capacitors using Voltage Contrast Inspection” Proceedings of ASMC, May 2013, pp. 301-306.


[5] O.D. Patterson, R.F. Hafer, X. Tang, C. Lei “The Merits of High  Landing Energy for E- Beam Inspection”, American Semiconductor  Manufacturing Conference, May 2015.


[6] M. Lei, K.Wu, H. Nguyen, M. King, “Application of Backscattered  Electron Imaging for Process Development in Advanced Technology  Nodes”, American Semiconductor Manufacturing Conference, May


SIMS Quantitative Analysis and Optimization for Ion Implantation Angle Deviation


JiangBei Shi, WeiTing Chien, QiHua Zhang, AiMin Li, ChuanJun Liu


Failure Analysis Laboratory /19 Xing Hua Avenue, Xi Qing Economic Development Area, P. R. China, 300385  Email: ANDY_SHI@SMICS.COM   Phone: (86-22)23700252.   Fax: (86-22)23700555


The accuracy of ion implantation is very important in  semiconductor manufacturing and will directly affect the  performance of the individual devices and even the whole chip. The deviation  of ion implantation energy, dose and angle often  result from abnormality of implant equipment or process design  limit. The information of ion implantation energy, dose and  angle can be qualitatively and quantitatively analyzed by SIMS (Secondary Ion Mass Spectrometry) [1], which provides a way  to diagnose ion implanter issue. Based on SIMS analysis results, we can judge whether ion implanter meets the requirements and  whether the process design achieves the expected goal. In this  paper, we report a SIMS data analysis method determine the  deviation of ion implantation angle. A term of deviation rate is  defined and a related calculation method was introduced, which  is proportional to the deviation angles of the ion implanter. Then, a statistical analysis on a large number of data of deviation rates  and ion implantation angles showed that the sampling data  followed normal distribution, and thus the corresponding 3  sigma could be obtained. Using the determined 3 sigma range of  the deviation rates, we can define the acceptable range for  deviation rate. Further, we can use the actual deviation rate to  judge if the implant equipment needs maintenance or not, or  suggest the direction for improvement. Finally, we set up an  oriented and quantitative optimization method of angle  deviation by the full mapping of SIMS depth profiles, which can  directly set the relationship between the angle deviation and the  adjustment parameters of ion implantation disk ( alpha,


beta). The equipment’s maintenance time and cost can thus be  minimized. This method can be used as early detection to the  abnormity of ion implant equipment.


SIMS is a method that applies spectrometry to detect and  analyze the secondary ions generated from the target sample  sputtered by the primary ion beam, as shown in figure 1. SIMS  can analyze all elements even including hydrogen, and provide


isotopic information. SIMS’s detecting sensitivity can reach


PPM or even PPB level [1, 3]. SIMS is primarily used for  analyzing the existing process and can provide the statistical  data base for the development of more advanced process in the  semiconductor manufacturing industry.


In semiconductor manufacturing, the accuracy of ion  implantation (IMP) will impact the performance of many


electrical parameters. But the IMP may be occasionally  abnormal in terms of energy, dosage or angle due to the  equipment or design issues. With the progress of advanced  technology, the relative sizes of semiconductor devices are  indeed becoming smaller and smaller, requiring a corresponding  high accuracy and precision during SIMS analysis.


Figure 1: SIMS analysis theory


Theoretical Background of SIMS Qualitative and  Quantitative Analysis


The SIMS depth profile can directly reflect the distribution of  ion concentration along the implant depth [1]. Thus, when the  ions are implanted at control wafer, SIMS analysis and results  comparison can be performed between the control wafer and the  reference sample. The comparison results will indicate whether  there is abnormality.


The abnormality of ion implantation often occurs on energy, dose or angle. The traditional SIMS analysis usually focuses on  defining the acceptable deviation range of energy or dosage. But  the judgment on the variance of SIMS profiles, caused by the  implanter angle deviation, is predicated upon the experience of  the respective analyst. There was no an exact analytical  judgment method pertaining to this phenomenon and also no  quantitative reference data is accessible to help the improvement  of implanter. Moreover, the SIMS data with minor anomalies  cannot be fully affirmed if there is an abnormality from the ion  implanter. As figure 2 shown, when SIMS profiles showed  significant abnormality the implantation machine might have  failed and the electrical parameters of semiconductor device can  also be affected, even resulting in irreparable damage, and need  more time and energy to recover.


Figure 2: SIMS profile comparison


SIMS Analysis Method of Ion Implantation Angle  Deviation


As already mentioned in the theory of background technology, the present SIMS comparison analysis method is not  satisfactory. Effective and reliable results cannot be achieved  due to the SIMS profile mismatching caused by ion implantation  angle deviation. In our study, the mismatching fluctuation of  SIMS profiles is acceptable in a certain range. Further study  found that there is a fixed relationship between the ion  implantation angle deviation and the profile matching degree, called deviation rate, denoted as K. This paper presents the  calculation process of K value and the detailed results. In order  to optimize the SIMS analysis process for inconsistent profiles;


this paper applies statistical methods to analyze the significance  and define the scope of K value. Because K value is directly  proportional to the ion implantation angle deviation, analyst can  effectively judge whether the result is acceptable or not when  the minor anomaly of SIMS profile appeared. The K value not  only can be referred for the further adjustment of equipment  performance, but also can eliminate a lot of repetitive SIMS  experiments, save raw material, and reduce the diagnosis time   and down time of equipment.


Implementation Steps of Angle Deviation and  Application on Ion Implantation Equipment  Optimization


The SIMS analysis steps for ion implantation angle deviation  can be described as figure 3.


Figure 3: SIMS analysis of IMP angle deviation


Next, we will report the details of the analysis steps. Figure 4  presents the SIMS results of two samples (sample 1 and sample  2) which are under the same SIMS analysis conditions and are  integrated into one coordinate system. Doing point to point  division for sample 1 and sample 2 will form a curve as curve 3  shown in figure 5. Obviously, curve 3 has too much noise, and  the values are poor for use. Then, we apply Gaussian smoothing


[4] on curve 1 and 2 in figure 4, which is to ensure the area (i.e. the area surrounded by the coordinate axis and the SIMS curve) and the curvature invariant, and do point to point divisions again. After theses data processing, we get the curve 4 as shown in  figure 6. For figure 5 & 6, the abscissa is the implantation depth  with the unit of micron (um), and the ordinate is the ratio of test


sample 1 to reference sample 2 in ion concentration. For  comparison purpose, curve 4 is also drawn in figure 5.


Depth


Figure 4: SIMS results of the test and reference samples


Figure 5: Fitting curves with (curve 4) and without (curve  3) Gaussian smoothing on the raw curves


Figure 6: Fitting curve after Gaussian smoothing


To choose the effective data in fitting curve 4, firstly, we need to  eliminate the biggest noise region from the integration area, as  region 6 shown in figure 7; Secondly, the region 5 must be  included because it is the region with the largest difference in  concentration; Thirdly the available area must include at least  95% dosage of the ion implantation. In combination with the  above three conditions, the available area of fitting curve can be  preliminarily determined from curve 4. Moreover,  to ensure the  reasonability and reliability of the used data in figure 6, a


suitable ordinate (i.e. the ion concentration ratio between the test  sample1 and the reference sample2) interval should be set, which can be determined by analyst based on the practical  experiment. In this paper, the available range of ordinate values  is 0.55~1.45, which is shown in figure 8. And the available area  is composed of y1=1.45, y2=0.55, and lines L1, L2.


Figure 7: The selection of the data region


Figure 8: Available region of the fitting curve


Next, as indicated in figure 9, the available area is trisected  along the abscissa, and the average coordinates A x1 y1


B x2 y2 C x3 y3 of three regions a, b, c can be calculated  respectively. Based on a & b coordinates the beeline slop value  K1 can be calculated; and based on b & c coordinates, the  beeline slop value K2 can be calculated. The deviation rate is the  maximum absolute value of K1 and K2.


Figure 9:  The definition of the region coordinates


In addition, the region coordinates A, B and C in the available  area can also be obtained as following method: point B can be  set as the average of multiple points (e.g., 50 points) that the  y-axis equals 1 or is close to 1, or be set according to the actual  situation. Then the average coordinates of the points to the left  of region b can be used to calculate point A, and the average  coordinates of the points to the right of region b can be used to  calculate point C. This method is equivalent to trisection one  when there are large amount of points in the available area. The  trisection method is preferred when there are enough points  because of the simple calculation process. If there are few points, the above mentioned method is preferred for it is more  dependable.


After obtaining the deviation rates, a large amount of  experiments and analysis were performed to verify the  relationship between the deviation rate and the angle shift of ion  implantation. The results are shown in figure 10, which indicate  that the deviation rate is directly proportional to the ion  implantation angle shift. A statistical analysis of a large number  of data on deviation rates and ion implantation angles showed  that the sampling data followed normal distribution [5] on the  whole, and thus the corresponding 3 sigma could be obtained, as  shown in figure 11. Using the determined 3 sigma range of the  deviation rates, we can define the acceptable range for deviation  rate. The K acceptable range should be less than 1.15.


Figure 10: Correlation between K value and ion  implantation tilt shift


Figure 11: Statistical analysis on the data of ion implant  deviation rates


It is needed to say, the best matching of SIMS profiles is the  depth profiles fully superposition. However, considering the  actual situation, the normal range of deviation rate can be  defined and optimized by the technical staff according to the  long-term monitoring based on the proposed SIMS profile  comparison and analysis method.


If the deviation rate exceeds of the corresponding specification, the full mapping analysis of SIMS depth profile is needed. Then  the corresponding full mapping deviation rates are obtained as  shown in figure 12.


Figure 12: Full mapping K value of test wafer


The key is to find out the smallest deviation rate Kmin from the  full mapping of K value curved surface; Kmin represents the  sampling point that best matches the reference sample. That  means the Kmin location of the point on the wafer (X0, Y0) indicate the most accurate point with least offset distance to the  wafer center (i.e., normally the wafer center is the optimal  position of IMP, however if angle deviation exists, it will result  in offset (X0, Y0)). And by establishing the corresponding  relationship between the offset (X0, Y0) and the adjusting  parameters ( alpha, ±beta ) of ion implantation machine disk (wafer bearing plate as shown in figure 13), ( alpha, beta) can be easily obtained to quantitatively correct and optimize the  ion implanter angle.


Figure 13: Ion implantation machine batch disk


According to the characteristics of ion implantation process as  below A, B and C introduced, we can establish the relationship  between  (X0, Y0) and ( alpha, ±beta ):


A: Alpha controls the vertical slope angle of the disk, i.e., the  vertical slope angle that the ion beams pass through the wafers  these on the disk plate.


B: Beta controls the horizontal slope angle of the disk, i.e., the  horizontal slope angle that the ion beams pass through the  wafers these on the disk plate.


C: Notch always points to the disk center.


At this point the experimental verification is performed. The  standard  (alpha, beta) of the machine is set to ( 1, 0) ( 0.5, 0) (0, 0.5) (0, 1). By doing SIMS full mapping depth profile  test, recording the location of Kmin in wafer, and further  regressive analysis, the coordinate relationship can be obtained  as shown in figure 14.


Figure 14: Coordinate relationship of (X0, Y0) to (±alpha, ±beta)


It must be pointed out that the implantation machine usually has  two models disk (batch and single wafer disk). Based on the  parameters relationship between batch and single wafer disk as  shown in figure 15, this method is also applicable to single  wafer disk parameter (tilt, twist) adjustment.


Figure 15: IMP disk angle parameters relationship


In addition, the regressive analysis result of the coordinate  relationship of (X0, Y0) to ( alpha, ±beta ) can be different with  the ion implantation recipes change. Using this method, we can  bring Kmin into the regressive analysis results, and get (∆alpha, ∆beta) directly, which can avoid multiple repeatable tests for  equipment optimization.


SIMS quantitative analysis and optimization for ion  implantation angle deviation not only can quantitatively  evaluate the deviation of ion implantation angle, but also give a  directional and quantitative parameter for implantation angle  optimization. For example, when the shift of ion implantation  dose is within limit but the SIMS depth profile matching is not  fully satisfied, it is difficult to judge whether or not to continue  production with the assumed risks if there is no angle deviation  value as reference data. On the other hand, stopping equipment  to check issue or conducting repeated SIMS experiments for  verification will also waste time and materials, which is taboo in  mass production. According to this paper, the quantitative  expression of deviation rate and specification definition can  clearly indicate whether there is an abnormality from the  implanter. It enables one to find out the problem in the early  detection stages. Consequently, it will be an accessible and  identifiable approach which can guide the technical personnel to  establish corresponding solutions to avoid accidents from ion  implantation angle deviation.


In addition, to keep the monitor program efficiency, the required  resource including full mapping analytical SIMS equipment (i.e., IMS -WF), statistical analytical software (i.e., SAS or JMP) and  The K calculate modularization (i.e., a programed Excel). With  above primary preparation, the deviation rate specification limit  will be fixed for ion implantation recipes. Then the analyst just  needs input SIMS data will directly get the fine tuning  parameters of the ion implantation angle deviation.


[1] Chen Yu Fan, and Chuizhen., “The quantitative SIMS


analysis of Ion Implant sample,” Journal of Chinese Mass


spectrometry society, vol. 13, no. 1, pp.14–22, Jan. 1992.


[2] Yin Hui-Ting, and Wang Jie., “SIMS Analysis Technology


and the Applied Research,” Chinese Journal of Spectroscopy


Laboratory, vol. 25, no. 2, pp.180–184, Mar. 2008.


[3] Bennighoven A, Rudenauer FG, Werner HW., “Secondary


ion mass spectrometry”. Wiley, New York, 1987.


[4] Zhong Wenfeng, Zhou Shumin., “The Application Research


and Implementation of Smoothing in Spectrum Analysis,”


Intelligent Computer and Application, vol. 3, no. 3,


pp.72–74, Jun. 2008.


[5] Fu Huimin, and Liang Chaohu., “Confidence Test Method


for Normal Distribution,” Journal of Aerospace Power, vol.


18, no. 3, pp.305–312, Jun. 2003.


MOFM : Magneto-Optical Frequency Mapping system   for very low resistance short circuit failure imaging


Tomonori Nakamura


Hamamatsu Photonics K.K., 812 Joko-cho, Hamamatsu City, Shizuoka, Japan  t-nakamura@sys.hpk.co.jp


Magnetic field imaging (MFI) has been an excellent tool for a  low resistance failure localization in LSI devices. A  Superconducting Quantum Interference Device (SQUID) and  a Giant Magneto Resistive (GMR) sensor are well known in  this field. A SQUID has extremely high magnetic sensitivity (500 nA, <40 pT/ Hz)[1], but the spatial resolution is  somewhat problematic due to the clearance that is needed for  cooling and vacuuming mechanism. A GMR sensor has higher  resolution but lower sensitivity (50 uA, <10 nT/ Hz)[1] and, they have less flexibility because the sensor/stage has to be  scanned during operation.


In this paper, we present a new current imaging method called  Magneto-Optical (MO) Frequency Mapping (MOFM). The  imaging is based on a laser beam scanning, which allows  flexibility and ease of use. The MO signal intensity is  inversely proportional to the distance between the sensor and  the current path to be detected. Since it can be 10 um or less, i.e., one half of the MO crystal thickness, it practically makes  the MOFM’s system sensitivity is 10 uA, it only 20 times  lower than a SQUID method, even though the intrinsic  sensitivity may be about 250 times or so lower. It can also  achieve high special resolution as with the GMR sensor  because of the short distance or clearance needed to sense the  current. These characteristics are verified with a TEG sample  and we present a case in which it is applied for the short  circuit failure localization.


Failure Analysis (FA) for semiconductor devices is important  for cost reduction and yield management. Optical FA tools: OBIRCH and thermal emission microscopy are utilized widely  for the isolation of short circuit failures. However, very low  resistance short circuit failures are hard to detect with those  techniques because of low resistivity changes with laser  stimulation and, no localized thermal emissions from failure  point.


To detect low resistance failure, MFI is widely used. MFI  localizes the current path with a SQUID or GMR sensor [2]. Shorted points are identified with the detected current path and  the CAD data. And this method can be adopted in FA for leak  failure in 2.5D and 3D LSI [3]. But SQUID needs cryo-cooler  system, vacuum chamber and magnetic shields. These  structures make impossible the reduction of the distance  between DUT and the detector. GMR sensor needs sensor  head scanning too. However, head scanning near sample needs  precise alignment to avoid touching the sensor head to DUT  surface and bonding wires. We present a new MFI method  named MOFM system based on laser scan microscopy and  Faraday effects. MOFM has LSM flexibility, high resolution  like GMR sensor and enough high sensitivity of magnet field.


Principle:MOFM


MOFM leverages Faraday Effects. When polarized light beam  is illuminated on the MO crystal, the polarized axis is rotated  depends on magnetic field in MO crystal, not depends on light  direction. Fig.1 shows MO (Faraday’s effect) principle of the  operation. Magnetic fields are induced by the current around  the wiring. The magnetic field direction obeys on the  right-handed screw rule. When MO crystal is placed on the  wiring as shown in Fig.1, the magnetic field direction in  left-side of current pass is through the MO crystal from  bottom to top, and from top to bottom at the right side. The  polarization axis is rotated in MO crystal opposite direction in  each area.


Setup:MOFM


Fig.2 shows optical setup for MOFM. This is based on Laser  Scan Microscopy. Light source is 1.3 um polarized optical  beam. Input light beam is rotated 22.5 degree with Faraday  Rotator (FR). MO crystal is placed on the DUT and light beam  spot is scanned on it. The polarization of refracted light  through MO crystal is rotated by the MO crystal. This MO  crystal is deposited on the 500 um glass wafer and coated with


1.3 um refraction layer. This refraction layer has transparency


on 1.1 um for pattern observation. And it has almost 100% refraction ratio on 1.3 um light for MO measurement.


Hundreds of kHz modulated current is fed to the testing net  from the pulse generator through current amplifier. The  refracted light goes back through the 22.5 degree FR again, and the rotation becomes 45±  degree. Finally, polarized beam  splitter (PBS) separate S and P of refracted light, the  modulation signal is detected by photo detector. The amplitude  and phase of signals are extracted by lock-in amplifier or  spectrum analyzer.


Figure 1: MO FM optics principle


Figure 2: MOFM optics


Basic characteristics of MOFM


Fig.3 shows TEG structure for MOFM and the measurement  conditions. The TEG surface around wiring is removed till  120um depth by end mill. It has 2 mm square loop and 300 um  pitch parallel wiring. The wiring width is 100 um and the  space is 200 um. Rectangular wave is applied to the TEG from  pulse generator. 51 ohm resistance is applied for termination  and total TEG resistance is 53 ohm.  The measurement  results are shown in Fig.4. In our system, 3 different data are


measured simultaneously; Amplitude, Phase, and IQ. I means  In-Phase signal, Q means Quadrate-Phase signal.


The current path is shown as black line in white area in  amplitude image, as boundary of opposite phase in phase  image, and as boundary of white area and black area in IQ  image.


Fig.3 TEG for MOFM


Fig.4 MOFM measurement results of TEG


(a)The amplitude image (A) shows z axis magnetic field  intensity. (b)The phase image ( ) shows magnetic fields  switching timing based on reference signal. (c) The IQ image  shows Acos( + offset).


Fig.5 (a) shows signal intensity and S/N ratio of MOFM. The  measurement frequency is 10 MHz. The measurement band  width is 1 kHz and it is equal to time constant 1 ms. In this  measurement, the minimum sensitivity is better than 0.1mA as  shown in Fig.5(c)(d). There is no signal in amplitude image  Fig.5 (b) but a little signal can be observed in phase image (c) and IQ image (d). The converted sensitivity limit is estimated  better than 3.3 uA with time constant 1 s. Currently, minimum  setting bandwidth of this system is 100 Hz and the sensitivity  limit is 33 uA (0.1 mA/ (1kHz/100Hz) ) at 30 um distance: half of metal thickness + half of MO crystal thickness. The  estimated sensitivity limit with thin wiring (less than 10 um  distance) will be 10 uA: more than 3 times better than this  result.


TEG


Wire width      100 um  Pitch


300 um  Rope size        2 mm  Depth


120 um


Metal thickness    40 um


Measurement condition


View size       512 512


Measurement time  5min


Time constant     1 ms/pixel


Objective        2.5x


Distance        0 um


Current ave.      10 mA (Duty 50 %) Frequency      10 MHz 0-1 V


Resistance      53


bandwidth      1 kHz


Polarized  Light


PBS


FR22.5


GM


Objective  Lens


MO crystal


Generator


Photo  senso


Spectrum Analyzer/Lock-in amp


Current  Amp


Refraction surface MO crystal


Polarizationrotation


Fig.5 (a) MOFM signal intensity depends on current (b)(c)(d)TEG measurement results with 0.1 mA. Bandwidth  1kHz@10MHz, distance 20 um. (b) Amplitude image, (c) Phase image, (d) IQ image.


Characteristics of MOFM: Frequency dependency


Fig.6 MOFM signal intensity depends on frequency


Fig.7 Incoherent light source S/N ratio for MOFM


In this work, the embedded NVM is fabricated with 0.18um  split gate flash (SGF) technology. Figure 2 shows the schematic  of a SGF bit. It consists of a single MOSFET with a floating  gate under control gate. Manipulation of the gate is  accomplished by charging and discharging of the floating gate  with high electrical field pulse. In programming operation, the  source is biased high (~10.5V) and drain is at low (0.6V), while  the control gate is positively biased (Vg=~2.1V). The hot  carriers created by high source bias are injected into the floating  gate while being swept from drain to source. The charge  increases Vt significantly enough that the transistor is turned off  during read condition (Vg=2.5V). During erase operation, the  control gate is biased high (~13V) while source and drain are at  ground. The electrons in the floating gate are discharged by the  high electric field created at the tip of the floating gate, thus  reducing Vt. In the erase state, the transistor is on in read  condition.


Figure 2: Schematic diagram of SGF cell in x-section view.


The memory array layout is shown in Fig. 3. A column consists  of bits on a continuous silicon active area; all the drains on the  same column are connected together with metal-1 line, while  all the bits in a row are controlled by a continuous poly gate (Word Line) throughout the array.


Figure 3: layout of SGF array. (black hollow - active, green - control gate poly, red - contact, orange - metal-1 line)


Case-I: Column-column Leakage


Wafer level test shows excessive yield loss related to entire  column failure in pairs, which suggest that column to column  leakage is a possible cause. To verify the hypothesis, the failed  die was deprocessed to the level where the two columns were  electrically isolated.  AFP was then used to measure I-V  characteristics between two neighboring columns. Figure 4  shows a typical curve.


Figure 4: I-V curves of a column-column pair with leakage.


The I-V curves are almost linear with resistance ranging from  10’s to 100’s of kΩ for most failed column pairs. It was also  noticed that the leakage would disappear with moderate  increase of bias, suggesting a very thin current path that could  be burnt out. Since the column is over 600um long, further  isolation of the defect is necessary before any physical analysis, such as TEM or FIB x-section can be attempted. To access the  area of interest with diagnosis tool, such as OBIRCH, two  micro-probing pads were fabricated with FIB deposition, on a  nitride isolation layer deposited in-house.


Figure 5 shows an OBIRCH image. The defect site is then  determined by overlaying the OBIRCH image with the layout. For physical analysis, we elected FIB slice and view to allow  3D survey of the defect site. Figure 6 is a SEM image of FIB xsection, where it is revealed that a residual silicide stringer is  bridging S/D of the neighboring columns.


Poly (WL)


Drain contact


A Bit cell


Source


Column


Figure 5: OBIRCH image and overlay with layout (insert).


Figure 6: SEM image of FIB x-section at defect site. A residual  layer of metal/silicide is bridging drains around contact area.


Based on the FA results, the FAB resolved the issue by  modifying the cobalt silicide pre-sputtering process.


Case-II: Single bit erase failure


Another type of high failure rate we encountered was single bit  low read current after erase test. For normal bits, the drain  current at read condition is typically in the 40-50 uA range. In  contrast, the failed bits have drain current between 20-30uA. They also show higher Vt than normal bits. To verify the  results, the dice were deprocessed down to contact level and  Vg-Id curves were taken with AFP. Figure 7 shows Vg-Id  characteristics of as-received dice. Indeed, all the failed bits we


probed showed lower current consistent with wafer test data. It  was also noticed that they have higher Vt.


Figure 7: Vg-Id curves of as received single bit in typical read  conditions. The failed bit shows low drain current and higher  Vt.


After confirmation of the failure, the bits went through  program/erase cycle to capture the details of the failure  behavior. After program, all the bits show Vt much higher than  gate bias at read state. At gate bias for read condition, the drain  current is negligible. The bits were then erased. Surprisingly, all the failed bits recovered to within normal range. Figure 8  shows Vg-Id characteristics after erase. The failed bit shows  similar current and the sub-threshold I-V slope is also very  close to reference bits. The results indicate that the failure  mechanism no longer exists upon repeated program/erase cycle. One of the possibilities could be that the failed bits require  longer than normal discharge time. At contact level, during  erase cycle, the high field on poly is only applied to a single  row, while at die level, during the same amount of erase time, the high field is applied to the entire array, which has 512  columns. To verify the hypothesis, the dependence of erase time  on Vt is measured, as shown in figure 8, where Vg-Id curves  were plotted with erase time from 4us to 20ms. There is little  difference noticed in Vt, which indicates that the low current in  failed bits was not due to insufficient erase time.


Figure 8: Vg-Id curves of failed and reference bits after  program/erase cycle with various erase time.


Residual  layer


STI


Active


Based on the results, repeated program/erase cycles were  performed at tester. Indeed, most of those single bit failures  recovered. Since the failure mechanism is removed upon first  program/erase cycle, its nature remains an open question.


In conclusion, the nano-probing techniques allow us to  electrically isolate defects in NVM arrays that would otherwise  be difficult to determine. Individual bits were probed to verify  and characterize failure signatures. It should be noted that  sample planar deprocessing is critical for the success of probing  NVM arrays. In the first case, it is shown that silicide residual  could cause column to column leakage by creating electrical  path between active areas of adjacent columns. In the second  case, it is shown that single bit failures due to low erase current  can be recovered with repeated program/erase cycle.


The authors would like to acknowledge support from Freescale  Semiconductor New Product & Technology Diagnostic Center  and Physical Analysis Lab (Arizona).


[1] Seungbum Hong, S., Auciello, O., Wouters, D. “Emerging  Non-Volatile Memories”, Springer(2014).


[2] Nishi, Y., “Challenges and opportunities for future nonvolatile memory technology”, Current Applied Physics, Vol. 11, No.  2 Supplement (2011), pp. e101–e103.


[3] Pawlowicz, C., “Delayering Tutorial-Fundamental to  Advanced Techniques”, 38rd Int’l Symp for Testing and  Failure Analysis, Phoenix, AZ, November 2012,


[4] H. G. Ong, H. G. and Gan, C. L., “Alternative Lapping  Method to Reduce Edge Rounding Effect,” Proc 38rd Int’l  Symp for Testing and Failure Analysis, Phoenix, AZ, November 2012, pp. 462-464.


[5] Hahn, J., “Masking Technique to Enable Multiple Site  Defect Analysis on a Microchip”, Proc 33rd Int’l  Symposium for Testing and Failure Analysis, San Jose, CA, November 2007, pp. 165-167.


[6] Weldy, M. E. and Serrano L., “Increasing Planarity for  Failure Analysis Using Blocked Reactive Ion Etching  Combined with Planar Polish”, Proc 31rd Int’l Symposium  for Testing and Failure Analysis, San Jose, CA, November  2005, pp. 206-208.


[7] Wills, K. S., “Planar Deprocessing Of Advanced VLSI  Devices”, Proc 32rd Int’l Symposium for Testing and  Failure Analysis, Austin, TX, November 2006, pp. 393-397.


[8] Moor, T., Malyanker, E., Raz-Moyal, E. “Single Die „Hands-Free‟ Layer-by-Layer Mechanical Deprocessing  for Failure Analysis or Reverse Engineering”, Proc 34rd  Int’l Symposium for Testing and Failure Analysis, Portland, OR, November 2008, pp. 363-367.


[9] Carlson, P., Donnet, D., Sidorov, O., Rue, C., “Delayering  on Advanced Process Technologies Using FIB”, Proc 40rd  Int’l Symposium for Testing and Failure Analysis, Houston, TX, November 2014, pp. 430-433.


Analysis of Write Recovery Time Degradation Caused by   Adjacent Storage Node Data in DRAM


Kwangwon Lee, Incheol Nam,  Daesun Kim, Hongsun Hwang, Sangjae Rhee, Kangyong Cho, Gyoyoung Jin


DRAM Product Engineering Team, Memory Division, Samsung Electronics Co.,Ltd  1-1, Samsungjeonja-ro, Hwaseong City, Gyeonggi-do, 445-330, Republic of Korea  E-mail) leekone@gmail.com


As microelectronic feature sizes are scaled down, the  characteristics and distribution of DRAM data retention time  and write recovery time are getting worse.  This degradation is  due to the increases in the leakage current and resistance of the  cell node and the decrease of cell capacitance in DRAM  devices. As the physical distance between storage nodes  decreases, node potential is increasingly affected by small  potential changes in adjacent storage nodes. In this paper, we  will show that the one of the most dominant contributors to  failure is the adjacent storage node level, and we will  demonstrate how node level affects write time delay. The  effect of the adjacent storage node level can be correlated with  a change in threshold voltage, much like the MOSFET body  effect. We define this phenomenon as the lateral body effect, and propose a model for adjacent potential effect using the  Buried Cell Array Transistor (BCAT) structure in sub 20nm  DRAM.


The scaling of dynamic random access memory (DRAM) creates a number of challenges such as decreased cell  capacitance, increased body effect (BE), increased variation in  threshold voltage (Vth), and bridge failures at signal lines  between the inter and intra layers[1][2][3]. The most important  characteristics for gigabit DRAM are the write time (tWR) and  the data retention time (tREF) which are related to cell


inta


capacitance and resistance [4][5].


l





cell


bV


ΔV(


Figure 1. Redundancy use rate for tREF and tWR versus  Technology node in DRAM. (A.U.=Arbitrary Unit)


Figure1 shows the physical distance between cell nodes (“Technology node”) versus redundancy use rate for tREF and  tWR. The redundancy is the spare elements such as s rows and  columns used as logical substitution for defective cells, and the  increase of redundancy use rate corresponds to an increased  chance of failure. A sharp increase in the parametric failure  rate for both characteristics is observed at Technology node  sizes less than the critical distance [6].


Although the single bit failures resulting from tWR and  tREF variations can be corrected with error correcting code (ECC) techniques, understanding of the failure mechanism  must be achieved through electrical and physical analysis. Figure 1 shows that the increase in tWR caused by higher total  effective resistance is the one of the major factors reducing  yield and product quality [7].


Failure Analysis & Modeling


The DRAM basic unit cell consists of a capacitor to store  one bit of data as electrical charge and a transistor to transfer  that data. The capacitor can be either charged (data-1, 1.2V) or  discharged (data-0, 0V). To determine the binary level 1 or 0, the small voltage changes in the bit line level (Vbl=Vinta/2) are  detected after the cell capacitance (Cs) charge is shared and the  bit line capacitance (Cbl) is amplified using a bit line sense  amplifier (BLSA). Vinta is defined as Internal Array Voltage.  The ∆ Vbl detected after this charge sharing is given by  Equation (1).


blCCs


Maintaining a stable ∆ Vbl is important for avoiding single  bit failures. After the design rule and supply voltage are  established, Cbl, Cs, Vbl are constant. So the charged voltage of  the cell capacitor (Vcell) becomes the dominant factor in  achieving the desired DRAM operating characteristics, and the  parameter tWR is critical in determining the voltage (Vcell) in  the cell capacitor [8]. Write time (tWR) is the time during  which the data in the write buffer can be written safely into the  DRAM cell capacitor. If there is insufficient tWR, the  resulting Vcell will be low and the intended charge is not fully  stored in the DRAM cell.  This can ultimately result in a read  failure at the bit cell.


Figure 2. Equivalent circuit to write data into storage cell.


Figure 2 shows a simple equivalent circuit of a DRAM cell.  It shows the write operation and illustrates the dependence of  the write time upon applied voltage (Vinta). Furthermore, the  write time decides the final value of Vcell because it depends on  the RC time constant of the write path.  This, in turn, depends  on parameters such as bit line resistance (Rbl), buried cell  contact resistance (Rbc), cell capacitance (Cs), and the  threshold voltage (Vth).


With the shrink of feature sizes in newer Technology Nodes, the effects of the surrounding circuitry (including adjacent  nodes, storage cells, and transistors) are increased. In  particular, the storage level of DRAM cells can be affected by  the action of adjacent cell transistors, significantly increasing  the possibility of read errors in the billions of storage cells in a  typical DRAM array.


The failures induced by adjacent data are analyzed by  monitoring the tWR characteristic while changing the six  storage node voltages in the cells immediately surrounding the  failing cell. Figures 3(a) and (b) show a top view of the  DRAM cell array cell topology with adjacent cells holding the  data-1 state and the data-0 state, respectively.


(a)                                              (b)


Figure 3. Top view of the DRAM cell array.  Thick circles  delineate the storage node in failure, and thin circles  delineate the adjacent cells surrounding the failing cell. View


(a) shows data-1 in the dominant adjacent cell, and view (b) shows data-0 in the dominant adjacent cell.


The tWR parameter is measured in each cell condition using  electrical analysis equipment. The difference of tWR each data  state is about 5.2ns at a supply voltage level of 1.5V. This  shows a considerable difference of 35% in write time. This  causes the tWR of cells with adjacent Data-1 states in excess


of the Joint Electron Device Engineering Council (JEDEC) tWR specification of 15ns maximum [9]. The tWR values  versus supply voltage for each adjacent cell data state are  shown in Figure 4.


Figure 4. The tWR versus supply voltage for each adjacent  cell data state.


Since the tWR parameter derives from an RC charging  characteristic, the resistance value can be extracted from  Figure 4 assuming a constant cell capacitance. Results show  that the tWR 5.2ns difference correlates to an apparent  resistance of 350kΩ, which is a 49% increase over the  apparent resistance of the adjacent Data-0 case. Since there is  no change in the physical resistance of the circuit  interconnects, the increase in apparent resistance stems from a  change in transistor operating characteristics between the two  adjacent data states.


Figure 5 shows the change in Vth versus adjacent cell  voltage level. Results show that the Vth of the cell transistor  increases with decreasing adjacent cell voltage. Therefore, tWR is delayed with the adjacent cell data-0 condition due to  increase in equivalent resistance of cell transistor operating in  the linear region. Results also show the nonlinearity between  adjacent cell level and change in threshold voltage.


Figure 5. The change of the transistor Vth in DRAM Cell Array  increases with the adjacent cell charge level


A simple body effect model is employed to explain the  nonlinear relationship between threshold voltage and adjacent  cell data level as follows,


Body Effect =





f ( bs





bs  2  B ) 


Lateral Body Effect =  f


cell


VAdj


( )3


Body Effect in DRAM Cell Array =  V )


) ( 4


bs


Adj





f (


where γ is body effect coefficient, ΨB is surface potential, Vbs


is the source to body substrate bias, β is lateral body effect


coefficient.


Equation (2) shows the body effect term in the threshold  voltage equation for a conventional MOSFET. A decrease in  body voltage (Vbs) increases threshold voltage. Based on Eqn. (2), a nonlinear change in the threshold voltage due to the  adjacent cell level is modeled by Eqn. (3). Consequently, the  body effect in a DRAM cell is expressed as Eqn. (4). Herein, we named Eqn. (3) as lateral body effect (LBE). The lateral  body effect is shown to be directly proportional to the square  of the adjacent cell voltage as shown in Figure 5.


Figure 6. The Vth change of transistor versus BCAT Depth  while varying the adjacent cell level Data 0 or 1.


Figure 6 shows changes in threshold voltage according to  BCAT depth with adjacent data-0 and data-1. Considerable  difference in Vth is observed with large BCAT depth. As the  BCAT depth increases, the gate region grows away from the  silicon surface. Thus, adjacent cell controllability increases  due to the decrease in the gate controllability by surface  potential. Therefore, same electric field induced from an  adjacent cell level affects Vth differently. This phenomenon  can be explained with increase in the LBE of the adjacent cell.


We analyzed the degradation of write recovery time, the  primary factors restricting the yield and quality in gigabit  DRAM. With no increase in the interconnect resistances, deterioration in write time was observed according to the state


of the adjacent cell data. The Lateral Body Effect model was  proposed to explain the nonlinearity between adjacent cell  level and change in write time. Results showed that the  threshold voltage of a cell transistor was changed by the  adjacent storage node level much like a body effect within the  BCAT structure in sub 20nm DRAM. Moreover, the threshold  voltage change according to adjacent data with large BCAT  depth can be explained easily. Our proposed lateral body  effect (LBE) model is useful for describing the shift in tWR  associated with the adjacent data state in this structure.


[1] Kinam Kim, Chang-Gyu Hwang, Jong Gil Lee “DRAM  Technology Perspective for Gigabit Era”, IEEE Transactions  on Electron Devices, Vol. 45, p598-608, 1998


[2] K. Kim and G. Jeong, “Memory technology for sub-40 nm  node,” in IEDM Tech. Dig., 2007, pp. 27–30.


[3] Kim, K., "From the future Si technology perspective: Challenges and opportunities", Technical DigestInternational  Electron Devices Meeting (IEDM), 1-9 (2010)


[4] K. Itoh and H. Sunami, “High density one-device dynamic  MOS memory cells,” IEE Proc., vol. 130, pt. I, pp. 127-135,


1983.


[5] K. Roy, S. Mukhopadhyay, and H. Mahmoodi-Meimand, “Leakage current mechanism and leakage reduction techniques  in deep-submicrometer CMOS circuits”, Pmc. Of  IEEE, vol. 91, pp. 305-327, Feb. 2003


[6] Kinam Kim et al., “Memory technologies in Nanoera:Challenges and Opportunities,”(invited) ISSCC Dig. Tech. Papers, pp. 576-577 ,2005.


[7] J. D. Plummer and P. B. Griffin, “Material and process  limits in silicon VLSI technology,” Proc. IEEE, vol. 89, pp. 240–258, Mar. 2001.


[8]http://www.samsung.com/global/business/semiconductor/fil e/product/tWR-0.pdf


[9] The computing DDR3 DRAM Specification (data sheet)


Failure Analysis Induced by Bit Line Sense Amplifier Noise   in High Density DRAM


Myungjae Lee, Sanghoon Ko,  Daegi Bae, Heeil Hong, Hongsun Hwang, Sangjae Rhee, Kangyong Cho, Gyoyoung Jin


DRAM Product Engineering Team, Memory Division, Samsung Electronics Co., Ltd  1-1, Samsungjeonja-ro, Hwaseong City, Gyeonggi-do, 445-330, Republic of Korea  E-mail:  mj524.lee@samsung.com, Phone: (82)-31-8037-0653


The open bit line architecture scheme is an effective method  to achieve higher density memory devices. With the scaling of  DRAM, we have adopted a bit line sense amplifier (BLSA) design using a shared local power line for reducing the circuit  layout dimensions. As a result of this new design, the write  time of the memory cell was sometimes degraded because of an  increase in initial sensing noise. This paper gives a detailed  analysis of the problem caused by the initial sensing noise by  examination of the behaviour of the opposite data portion of  the cell array matrix when the word line is not activated. Finally, we propose a design improvement to reduce the  magnitude of noise peaks and the results of this improvement  when implemented in the test vehicle.


In order to achieve higher memory cell density, the open bit  line architecture has been recently adopted in DRAM  technology. In this architecture, the conventional bit line sense  amplifier is tied to a common power supply node to minimize  the layout area. However, this structure is vulnerable to  sensing noise that is dependent on data pattern polarity during  DRAM operation [1-4]. In particular, capacitive coupling  between the signal lines and the shared power bus as well as  bulk well noise have significant impact upon the initial sensing  operation [5, 6]. This phenomenon is continuously intensifying  as the decreasing feature sizes reduce the distance between the  adjacent data signal lines while simultaneously increasing of the  number of shared supply power nodes in the sense amplifier  region. Moreover, the initial sensing margin is emerging as a  critical issue through design rule changes to obtain higher  device densities. It is becoming progressively more difficult to  ensure stable quality and yields in mass production, a problem  that is expressed by write time degradation (tWR). In this  paper, we show how we found the sensing noise failure  mechanism by focusing on the initial sensing time. Our  investigation was partially based on the electrical analysis and  the simulation.


Experiments & Modeling


It is well known that the early sensing characteristics of the  cross-coupled differential bit-line sense amplifier (BLSA) make  it more difficult to obtain sufficient sensing margin at reduced  feature sizes due to a decrease in the ratio of the cell  capacitance to the bit line capacitance. This ratio is determined  the initial successful operation of the sense amplifier. Moreover, performance of the BLSA is degraded through  increase of the level of opposite data during the charge sharing  period between word line (WL) enabling and the sense  initiation point. This phenomenon is represented by an increase  in the delay parameter “to Write Time” (tWR). The DRAM  cell array consists of uniformly sized repeating unit blocks that  may have an indeterminate data polarity. The performance of  each unit block is determined by monitoring the write time (tWR) degradation caused by increasing the amount of inverse  polarity in the opposite data during the charge sharing period.


Figure 1: Write time degradation versus opposite data block  portion and measured Sensing Noise versus Failing Cell block  position.


Figure 1 shows that the measured sensing noise increases  sharply at the point where the block data changes polarity. The  degradation of tWR occurs in three characteristic regions.


Region A, which is the largest sensing noise block including  the fail cell, shows rapid increases for each change of data  polarity within the block. When the word line is activated, the  charge of cell capacitor data flows to the bit line so the  resulting BL node becomes biased to a known state. Figure 2  shows the case where a memory cell holding a low logic level (Data 0) has transferred its state to the BL node.  During  charge sharing, the BL node has a current path to the shared  power bus ground node through the nMOSFET transistor N3. At the same time, the voltage levels of the BLB lines  associated with to the cells holding the high logic level (Data 1) and sharing the same word line are increased.  This is caused  by an increasing amount of charge caused with the N2 and N6  nMOSFET transistors tied to the same shared power bus  ground line.  We refer to the amount of charge contributed by


each of these oppositely polarized bit lines as a “block” of


charge.  Hence, the initial jump in sensing noise is relatively  large because local ground power line is shared in the sense  amplifier regions.


For Region B, the increase the sensing noise is reduced as  successively fewer opposite polarity cells are present, so write  time (tWR) degradation rate has increased more slowly from  twelve percent to eighteen percent despite a reduction of five  opposite polarity data blocks from the word line.


Finally, there is Region-C where most of the bitlines now hold  Data 0. In this region the tWR degradation is less than two  percent as the last few bit lines in the word line transition to  hold Data 0.


Figure 2: Schematic diagram showing Current paths (red) at  the Sensing start point


We designed an experiment to observe the initial sensing  noise behaviour according to the proportion of the data cell


array blocks holding a Data 0 polarity. Two test cases were  constructed; the first where the cell array uses a shared local  ground line and the second where the local sense amplifier  ground lines are isolated from one another, as shown in Figure


3. By comparison of the two cases it is possible to determine  how noise is delivered from the region including failed cell into  other blocks.


Figure 3: The bit line sense amplifier schematic diagram for  testing in initial sensing behavior: (a) Local ground power  line sharing case and (b) Isolated local ground power line  case.


Nano-probing techniques, such as atomic force probe (AFP) used in this study, allow us to access individual devices at  contact or via levels and characterize the details as much as  possible before a decision can be made for physical analysis. They have been widely used in failure analysis communities. However, for it to be applied to NVM, it is not trivial to develop  a deprocessing procedure to achieve planar surface throughout  the array, as most NVM arrays are very large, up to a few  millimeters across. Within the array, the control gate (poly line) and active areas in a column are electrically continuous.  Planar  deprocessing down to contact level is necessary to keep the  whole array intact [3-9]. They have some advantages as well as  disadvantages. Some require special equipments that are not  commonly available in many FA labs [4, 8, 9]; others would not  be able to achieve large enough planar area required for our  applications [5-7]. Furthermore, the solution to local non-planar  issue caused by variation in tungsten via density was not  properly addressed, without causing side effects (such as  scratches).


In this paper, we report the application of AFP to characterize  each individual bit at contact level, or individual column at via1  level. By applying program/erase cycle to each individual bit, we were able to capture each individual's failure characteristics. Based on the information, further diagnostic and physical  analysis techniques, such as optical beam induced resistance  change (OBIRCH) and focus ion beam (FIB) x-section, were  used to find the failure mechanisms.


Sample deprocessing is critical for probing NVM devices, as  gate poly and column active area are continuous across the  entire array. To achieve planar deprocessing, we approach the  issue with a combination of reactive ion etch (RIE), wet  chemical etch, and finger polishing with colloidal silica and  diamond slurry. Many of the techniques used here are reported  in the references [3-9]. The benefits and disadvantages of each  technique are considered based on equipments and settings  available in our lab and to best fit to our specific back-end  stacks and layout. The top nitride passivation layer is removed  with RIE while the top metal layer (aluminum) is removed with  wet etch in HCl acid. Compared to finger polishing, these two  steps greatly improve flatness of the final target surface. The  remaining layers are removed by a combination of RIE (for  dielectric layer), wet etch (metal layer), and finger polishing  alternatively with colloidal silica and diamond slurry (for  removing barrier layer and smoothing out dielectric/metal  regions). Colloidal silica and diamond slurry have quite  different polishing rates on different materials. The former is  fast on dielectric but not so fast on tungsten and other metals, while the later is just the opposite. By alternating those two  polishing materials, we were able to achieve the required  flatness at contact level.  Figure 1 shows the die at contact level. The NVM array is 600um x 1500um large. The surface is planar  across several arrays.


Figure 1: NVM array deprocessed to contact level.


NVM principle


Fig.6 shows frequency depended sensitivity curve of MOFM  that is calculated from IQ signal intensity. The lower  frequency is limited by amplifier of photo detector. The  amplifier band width is from 10 kHz to 3 GHz. This system  can be used between 20 kHz and 10 MHz. The S/N ratio is  limited by light source RIN. The light source: High-power  Incoherent Light-source (HIL) noise ratio is shown in Fig.7. In  the case of the laser light source, there are fringe pattern that is  caused by the interference between several optical surfaces, optical lens, sample surfaces and glass substrate of MO. And  the vibration of optics modulates the fringe patterns and it  generates noise in low frequency. When in use of incoherent  light source, there are no fringe patterns and the noise. The  sensitivity in higher frequency region is limited by magnetic  loss of MO crystal. S/N ratio of MOFM can be improved by  RIN reduction of light source and MO crystal sensitivity  improvement.


Characteristics of MOFM: distance dependency


Magnetic field imaging can be used for depth measurement. The z axis magnetic field intensity around a current is shown  in equation (1).


Bz


∝


(1) The current is on y axis at origin of x-z plane, current distance  from MO crystal is d as shown in Fig.8(a) . This equation has  peak value at the position as shown in equation (2). But, if the  d was smaller than wire width, the peak value position is shift. If the wire effective width is 2a, the peak value position is  shown as equation (3).


x ±=


2 d


±


Fig.8 Depth measurement with magnetic field


x,d


wiring


MO cristal


Effective width 2a


The equation (3) shows, wiring width is needed to calculate  distance between current path and MO crystal.


The TEG Bz IQ measurement result with MO crystal contact  condition is shown in Fig.8 (c). Wiring width is 100 um and  the thickness is 40 um. MO crystal thickness is around 10 um.


Fig.9 Depth measurement with magnetic field. The horizontal  axis shows physical distance from wiring to MO crystal  surface. Signal intensity is measured at loop area and parallel  wiring area. Distance 1 and distance 2 shows result with  equation (3).


The depth data is calculated at the top edge of TEG loop  position as shown in Fig.8. The measured depth of current is  shown in Fig.9. It shows signal intensity and the distance. To  change the distance, there are SIM between TEG and MO  crystal.


In Fig.9 “distance1” shows depth calculation results with wire  effective width 100 um. In this case, initial distance (depth) is  0 um by equation (3). However, physical distance should be  more than half thickness of wiring, and the line graph is not  straight. To rectify the line graph and calculate true distance, it  is needed to add new parameter, effective width of wiring. The  rectified line graph “distance2” shows 80 um and the depth is  30 um. The depth 30 um is total amount of the half of wiring  thickness and half of MO crystal thickness. Effective width is  depends on roughness of wiring side wall.


Sensitivity of MOFM


MO crystal magnetic sensitivity can be calculated from the  peak distance 50 um shown in Fig.8 and current depth from  MO crystal 30 um shown in Fig.9. Minimum current can be  detected is 0.1 mA with measurement band width 1 kHz at 10  MHz, shown in Fig.5. Then, the peak signal intensity position  from center of current is 58 um. And the magnetic field  intensity is 345 nT, calculated by Biot-Savart law. If the 345  nT with bandwidth 1kHz was the limit, the sensitivity is 10.9  nT/ Hz @ 10 MHz. This MO sensitivity is almost same as  GMR sensor. The difference between sensitivity limit 50 uA  of GMR sensor and 10 uA of MOFM is estimated by  depending on measurement time constant, visibility of phase  image and sensor distance from DUT.


Result


Fig.10 shows MOFM measurement images of low resistance  short device in package. Sample design rule is 40nm and chip  size is 5 mm by 5 mm. The mold thickness is 500 um. Short  failure is located between Vdd line and Vss line. The  resistance is 95 ohm. The bias voltage is square waveform  0-1.5 V 200 kHz, the duty is 50 % and the average leak  current is 15 mA. Fig.10(a) shows amplitude image, (b) shows  phase image, (c) shows I/Q image of MOFM. Black line in the  amplitude image shows current path. Upper part of line is Vdd  lead frame and lower one shows Vss. In the phase image, current path is also shown with boundary of reversed phase. Phase signal relation shows current direction. In this figure, the right side of current is yellow and the left side is blue. As  shown in Fig.3(d) leak current is go through Vdd line till the  short failure point and spread into ground net. The current path  is shown more clearly than thermal emission image Fig. 11.


(a) Amplitude image


(b) Phase image


(c) I/Q image


(d) Phase image and Current direction


Fig.10 MOFM current measurement with x1 lens (13 mm by  13 mm) 0-15 mA 200 kHz modulation


Fig.11 Thermal emission image of DUT (phase image) bias  from different pin.


180°


-180°


0°


360°


Vdd


Chip size


Short


position


In this work, we proposed new MFI method “MOFM”. This  method can provide 0.1 mA current with contact condition in 1  ms and around 10 mA current images from outside of a 500  um mold package. The sensitivity and the resolution are easily  increased by reducing the mold thickness. MOFM have  applicability to isolate most of low resistance short failure.


We would like to thank RENESAS engineering Services Co., Ltd for the support and the samples providing.


[1] http://www.neocera.com/magma/Products.html


[2] J. Gaudestad et. al., “Short Localization in 2.5D Microchip  with Interposer using Magnetic Current Imaging”,


Proceedings from the 40th International Symposium for Testing  and Failure Analysis (ISTFA) 2014, 43-48


[3] D. Vallett et.al., “High-Resolution Backside GMR  Magnetic Current Imaging on a Contour-Milled Globally  Ultrathin Die”, Proceedings from the 40th International  Symposium for Testing and Failure Analysis (ISTFA) 2014, 23-27


Magnetic Current Imaging Power Short Localization


J. Gaudestad *, F. Rusli, A. Orozco


Neocera, 10000 Virginia Manor Road, Beltsville, MD, 20705, USA  M. C. Pun


Avago, Bayan Lepas Free Industrial Zone, 11900 Penang, Malaysia


A Flip Chip sample failed short between power and ground. The reference unit had 418Ω and the  failed unit with the short had 16.4Ω. Multiple fault isolation techniques were used in an attempt to find  the failure with thermal imaging and Magnetic Current Imaging being the only techniques capable of  localizing the defect. To physically verify the defect location, the die was detached from the substrate  and a die cracked was seen using a visible optical microscope.


Complicating failure analysis is the semiconductor industry’s trend toward complex packaging such as Multi-Chip Modules (MCMs) and  flip chip packages. This requires that nondestructive measurements be made through thick  layers of insulation or conductors. One of the  most common failure modes in complex packages is the power-to-ground short. Many techniques, such as infrared thermography [1], are  either not able to locate power-to-ground shorts  or are inhibited in their effectiveness by multiple  metal layers technology or flip-chip type packaging [2].


2. Magnetic Field Imaging (MFI)


Magnetic Field Imaging (MFI), as applied to  failure analysis (FA) in the semiconductor industry, is based on mapping the magnetic field produced by a current injected into the failing structure of the device under test (DUT). Unlike optical of infrared radiation employed by Failure  Analysis (FA) techniques such as thermal and  optical emission [3, 4, 5], the magnetic field has  the advantage of passing unperturbed through  virtually any materials used in semiconductor  manufacturing. The obtained magnetic field image of the DUT is then converted into current  density image by using a Fourier Transform inversion technique [6, 7]. In order to determine  fault location, the current density image is superimposed onto an optical image.


MFI has two major implementations: Magnetic Current Imaging (MCI) for localization of  shorts and leakages [8] and Space Domain  Reflectometry (SDR) for localization of open  defects [9].


The current case study discussion pertains to  the short circuit search with MCI technique. For


MCI applications, magnetic field is imaged by  either a Superconducting Quantum Interference  Device (SQUID) or Giant Magneto Resistive (GMR) sensors. The SQUID sensor is mostly  applicable for package level devices with working distances beyond 100μm and/or when low  current setup is required. Measurements are  made with Alternating Currents (AC) signal of  2-15 kHz range applied to a sample referenced  using a lock-in amplifier to provide for noise  reduction. The GMR sensor is used for the front  side wafer/die level high resolution (submicron) imaging using AC sampling currents at 95 kHz [10].


SQUID and GMR sensors differ in both sensitivity and spatial resolution. SQUID is the most  sensitive magnetic sensor known [6], and for  electronic fault isolation (EFI) it can detect signals as low as


at a working distance of several hundred microns between  the current path and sensor. The SQUID sensor  is kept in vacuum at cryogenic temperature, while the DUT is raster-scanned at room temperature and separated from the SQUID sensor  enclosure by a thin diamond window. This setup  allows localizing currents to within ±3 microns. For 2.5D applications the SQUID sensor will be  used.


3. Power Short in Flip Chip sample


The sample to be investigated was a 4.6mm ×


4.6mm flip chip silicon device with full thickness 725μm on top of an organic 13mm × 13mm  substrate (Figure 1).


Figure 1. Samples front and back


The reference unit has normally a resistance  between Vdd (power) and Vss (ground) of 418Ω  when measured close to zero volts. The failing  sample showed a Vdd-to-Vss resistive short of


16.4Ω when measured at the same test voltage.


Figure 2. IV curve of reference unit (red) and  shorted unit (blue)


The failed unit Vdd-to-Vss curve trace is  shorted as compared to a reference unit Vdd-toVss diode-like curve trace (Figure 2). When current can pass through both a reference sample  and a failing sample, both reference and failing  samples are needed for direct current path comparison to find the deviating current path.


4. Experimental setup


The sample was attached inside the MCI system  to an XYZ stage for raster scanning under the  SQUID sensor. The SQUID sensor enclosure was  brought to within 100 μm of the sample surface (top of the silicon, backside of the die) to get the  highest possible resolution (resolution is dependent  on distance to failure site only, not the material in  between). Micro probers were used to inject current through the solder balls and thus allow for  retaining device integrity and possibility of further  return of the sample to the automated test equipment (ATE) (Figure 2). Since the short failure location was unknown, a current image was acquired  from the entire sample.


Figure 3. Sample setup for Scanning SQUID  Microscope (SSM) used for package MCI.


Both failing sample and a reference sample  were scanned using the same scan parameters  and then the signals were compared side by side (Figure 4a, 4b).


5. Fault Isolation using MCI


AC current of 5.333kHz frequency and


3.5m


amplitude was injected  through backside micro probers into the Vdd  solder bal connection L1 with respect to ground  reference on Vss solder ball A1, and then global  MCI was performed.


Reference  Unit


MCI Electronics


Vacuum chamber  with cryo cooler  for SQUID


sensor


XYZ stage


L13 (VDD)


A1 (VSS)


Failed  Unit


Figure 4a. The current paths, between power  contact Vdd (L13) and ground Vss (A1), superimposed on the top view of the Reference (Left) and failed (Right) sample.


Failed


Unit


Figure 4b. The same cur-rent paths are overlaid


on “top view” optical images of both samples


(each optical image of the backside of the BGAs  was rotated and flipped to simulate a top view  layout of the BGAs).


Since MCI is imaging current density, a  stronger signal will always be detected from a  metal line rather than in a metal plane. To reduce  noise and to filter out the weaker current density  image from the plane, “thresholding” was used,


which explains why only the feeding signals and  the shorting sites are visible in Figures above.


By comparing the reference sample and the  failing sample current maps (Figures 4a and 4b) overlaid on the layout, the short location in the  failing part was identified between contact solder balls L11 (Vdd) and M11 (Vss).


6. OBIRCH, Thermal Imaging and X-Ray


OBIRCH (Optical Beam Induced Resistance  Change) a Laser Scanning Microscope (LSM) technique, was used to image the entire die area  that revealed a die crack (Figure 5). LSM can  only find failures at the die level and if the failure was in the substrate area LSM would not be  useful. Also, OBIRCH usually cannot detect any  resistance changes in case of a power short, as  the power and ground planes are in the lower  metal layers (as seen from the backside/top of  the die) and the laser beam struggles to penetrate  the metal layers in the die.


Figure 5. A subtle die crack was seen in the  OBIRCH image.


L11 (VDD)M11 (VSS)


Thermal Imaging was used to inspect the  failed through the backside of the silicon, which  revealed the subtle crack. This almost opaque  crack can be seen in Figure 6.


Figure 6. IR imaging of the die reveals the crack


X-ray imaging was also used to isolate the defect, but neither crack nor the short were visible  in the X-ray image (Figure 7).


Figure 7. X-ray did not reveal any defects between L11 and M11.


7. Physical FA (PFA)


Using the information from fault isolation, the  sample was sent to physical examination for  failure verification. The die was then removed  from the substrate and the die crack was localized using an optical microscope (Figure 8).


Figure 8. Optical microscopic imaging of the die  reveals the crack


8. Conclusion


The short was found to be caused by a crack  in the die. Usually cracks tend to cause opens or  leakages but not shorts, making this a very interesting case. Only MCI was capable of seeing the  current path in this substrate, which is caused by  power shorts generating few to none hot spots  for thermal or laser scanning techniques to detect.  Both OBIRCH and Thermal Imaging, which are techniques used to find shorts, were  not able to localize the short by using current or  hot spots through standard analysis techniques. Instead they were used in a passive mode as an  imaging tool with longer wavelengths to see  through doped silicon.


1. M. Foremny and S. Trivedi, “Thermography testing of P.C. Boards”, ISTFA 1983, pp. 219-221


2. W.E. Vanderlinde, M.E. Cheney, Microelectronics


Research Laboratory, E.B. McDaniel, K.L. Skinner,


University Research Foundation,L.A. Knauss, B.M.


Frazier, H.M. Christen, Neocera, “Localizing Power to Ground Shorts in a Chips-First MCM by Scanning


SQUID Microscopy”, IRPS 2000


3. Breitenstein, O., et al, “Microscopic lock-in thermography investigation of leakage sites in integrated circuits”, Rev. Sci. Instrum. 71, 4155 (2000).


4. A. Glowacki, C. Boit, Berlin University of Technology-German and P. Perdu, CNES – France, “Optimum Si thickness for backside detection of photon emission using Si-CCD” ESREF Proceedings 2012.


5. T. Sun, G. L. Woods, M. F. Duarte, K. Kelly, C. Li,


and Y. Zhang, Rice University, Houston, TX, USA


“OBIC Measurements without Lasers or RasterScanning Based on Compressive Sensing “ ISTFA


Proceedings 2009


6. J. P. Wikswo, “SQUID sensors: Fundamentals, Fabrication and Applications, Chapter The Magnetic Inverse Problem for NDE”, pp. 629-695, Kluwer Academic Publishers, The Netherlands, 1996.


Crack Line


Pin A1


7. E. F. Fleet, et al., “HTS scanning Microscopy of Active Circuits”, IEEE Transactions on Applied Superconductivity, 9 (2): 4103 (1999).


8. David P. Vallett, “A Comparison of Lock-in Thermography and Magnetic Current Imaging for Localizing


Buried Short-Circuits”, ISTFA proceedings, 2011.


9. J. Gaudestad, V. Talanov, P. C. Huang, “ Space Domain Reflectometry for Opens Detection in StackedDie Packages”, Electronic Device Failure Analysis


Society (EDFAS) Magazine, August 2012, pp. 22-28


10. L. A. Knauss, et al., “Current Imaging using Magnetic Field Sensors”, Microelectronics Failure Analysis


Desk Reference 5th Ed., pp. 303-311 (2004).


A Case Study of Failure Analysis on ESD-induced Degradation of 405nm LD


Hongmin Liu†, Zhe Li,  Zheng Weng


National Space Science Center, Chinese Academy of Sciences


No.1, Zhongguancun Nanertiao, Haidian District. Beijing 100190, China  Hao Jiang, Yuanting Shen


Shanghai Institute of Technology Physics, Chinese Academy of Sciences  No.500, Yutian Road, Hongkou District. Shanghai 200083,China


A field failing Ondax’s 405nm Laser Diode (LD) was under  failure analysis. The failure analysis (FA) results showed that  the LD was very sensitive to ESD and the degradation was  ESD induced. Some mechanism explanation is also given in  this paper.


## I. Introduction


I. Introduction


Ondax’s 405nm Laser diode (LD) [1], which was single mode  with collimated single frequency, was selected as the high  quality light source in a space-born quantum communication  system. Performance degradation of an Ondax’s 405nm LD  was reported after assembled in PCB, and the failing device  was submitted to failure analysis (FA). The FA included 5  steps: (1) electronic parameter test, (2) visual and mechanical  inspection of the LD die, (3) SEM inspection of the burn out  dots, (4)ESD sensitivity test of the LD, and (5) some  mechanism interpretations. The FA was conducted in the clean  room with controlled temperature, humidity and ESD-protected. All the FA instruments and tools were calibrated.


Failure analysis showed that the Ondax’s 405nm LD was very  sensitive to ESD and the damage was ESD-induced. Further  analysis revealed that the ESD with reverse polarity broke  down the pin structure. The detailed processes of the failure  analysis are described in this paper, and some mechanism  explanation is also given.


## II. Processes of Failure Analysis


II. Processes of Failure Analysis


### (1) Electronic-optical  parameter test


(1) Electronic-optical  parameter test


The electronic-optical specification summary of Ondax’s  405nm LD is listed in table1. The test equipment include a  precision power supply, an optical power meter, an Newport  integrating sphere, and a transistor output characteristics curve  tracer.


### (2) Internal visual and mechanical inspection


Table 1:  Electronic-optical parameter summary


First, forward biased voltage was applied on the failing LD  with current compliance at Max. Iop to observe laseremission. With the power on, the LD worked as a LED, instead of a LD, and the output light power was about 10%of the rated power  under certain bias. Second, a transistor output characteristics  curve tracer was used to obtain the forward and reverse I-V  curves of the LD[2], as shown in figure1.TheseI-V curves of  the LD looked more like the I-V curves of a resistor, instead of  atypical diode. The unusual output light power and I-V curves  indicated the electronic function failure of the LD.


Figure1:I-V curves of LD


(2) Internal visual and mechanical inspection


The LD was carefully decapped and cleaned, including the outlayer metal-can, the optical parts and the inner-layer metal. The  internal visual and mechanical inspections were performed  according to MIL-STD-883F, methods2013.1, 2011.7 and


2019.7, to check the structure integrity of the die body, wire  bonding and die attachment.Figure2 shows the mechanical  structure overview of the facet of laser emitting. Figure 3  shows two black dots on the surface of anode and the


magnified photo of one of them. During the visual inspection, no defect listed in the methods 2013.1 was founded, except two  black dots. In the mechanical test, the results of bonding  strength and die shearing test [2]met the requirements of MILSTD-883. From the internal visual inspection and mechanical  tests, we can conclude that no mechanical structure defects or  contamination lead to the electronic malfunction.


Two black dots found on the surface of the anode was zoomed  in at 60X magnification, as shown in right of figure 3. They  were likely burn out dots. Thus electrical overstress might lead  to the burn out in these dots. To figure out what the dots were  and what caused them, SEM inspection was conducted.


Figure 2:Mechanical structure and laser emission facet


Figure3:Burn outdots on the anode surface


(3) SEM inspection of the burn out point


Optical microscope has limitation in depth of field and  component identification. So a scanning electron  microscope(SEM) is used to look at the detailed structure of the  burn out dots as well as to obtain the EDX spectrum of it. The  SEM inspection was conducted according to MIL-STD-883F  and method 2018.4. Figure 4 is the SEM[2] photo of one of the  burn out dots. Figure 5 shows the EDX spectrum and Table 2  lists its chemical components. Figure 4shows that the burn out  dot actually was a punch hole. No melt was found surrounding  the punch hole. So it was suspected that an electro static  discharge event with high voltage and limited current happened  on the die, resulting in the punch holes. EDX spectrum shown  in Figure 5 indicated that there were Au and Ga atoms in the  punch holes, as listed in Table 2. Au is the material of anode  and Ga is the inner material of the die body. It meant that the  inner material Ga was pushed up to the anode surface when the  discharge happened, indicating the ESD must be a reverse  polarity one.


From SEM inspection, we concluded that a reverse electrostatic  discharge event happened in the LD die and broke it down, resulting in the punch hole. The energy of the electrostatic  discharge was not enough to burn it completely, causing a short  circuit.


Figure 4: SEM photo of one of the punch holes


Figure 5: SEM spectrum of the punch hole


Table 2:Componentanalysis


Element Weight% Atomic% Ga K


58.75


80.10


Au M


41.25


19.90


Totals 100.00


(4) ESD sensitivity test


From failure analysis steps (1), (2) and (3), we knew that a  reverse polarity ESD event happened on the LD, but its energy  was limited. The bias circuit was carefully designed with surge  absorption function and the LD was stored in ESD protecting  material. Thus the ESD event should come from the handling  process. If the LD is very sensitive to ESD, it could be  damaged easily in an improper handling process. An ESD test  was carried out to classify the ESD sensitivity of the LD. The  ESD test was performed with the HBM method and circuit(see  figure6) as described in MIL-STD-883F and method 3015.7, which enabled the stimulation of the HBM ESD[2]. The ESD  test started at 50V, and increased with interval of 50V each  time until the LD showed sign of degradation. Leakage current  and light output power were measured after each ESD test. A


brief description of the ESD test result is shown in table3. From  table3, 5 samples of Ondax’s 405nm LD were under ESD test, and degradation was observed when the voltage reached 200V  or 250V. It indicated that the 405nm LD was very sensitive to  ESD and could be damaged easily if handled without careful  ESD protection. In our case, in the manufacturer instruction of  LD, the ESD sensitivity and protection are actually emphasized.


Figure6:  ESD classification test circuit(HBM)


Table 3:  ESD test results


Samples


Degradation at voltage


50V 100V 150V 200V 250V


#1 × × × √


#2 × × × × √


#3 × × × × √


#4 × × × √


#5 × × × × √


An extensive study on ESD effects on GaN-based commercial  470nm and 570nm LEDs[3] revealed that the breakdown  discharge voltage on GaN-based LEDs is from 200 volts to 250  volts.  From SEM spectrum of LD, we knew that Ondax’s  405nm Laser diode was GaN or InGaN based, so the  breakdown discharge voltage of LD should bein the same range  as GaN-based LED. This is helpful to understand the ESD test  results of Ondax’s 405nm LD.


III. Some Mechanism Explanations


The ESD-induced degradation has been investigated and the  mechanism has been studied for a long time.  Although there  are differences in types and structures, considering the  threshold of current density, gain and efficiency, the thickness  of all LD or LED active layer is so thin as about hundreds of  nanometer. So all the laser diodes are sensitive to ESD due to  their very thin active layer[4-7].


Ondax’s 405nm Laser diode was based on InGaN or GaN  technology and the detailed structure of LD die was unknown. But its schematic representation is shown in Figure 7. The  active layer is under the ridge region with width of several um  and depth of several um from the anode surface, hence its  resistance to reverse electrostatic discharge is the weakest


## III. Some Mechanism Explanations


point of the whole anode surface area. This is why we  observed two punch holes lied in a nearly 4um width straight  metallization line, where the active layer located, comparing  the two pictures in Figure 7.


Figure 7:  Schematic diagram of 405nm LD structure


## IV. Conclusion


IV. Conclusion


Performance degradation of an Ondax’s 405nm LD was  reported after assembled in PCB and failure analysis was  performed on it. I-V curves indicated that the LD lost the  electronic and laser emission function. Internal visual  inspection and mechanical test indicated an electrical overstress  might happen on the LD. Follow-up SEM inspection revealed  that it was an ESD event with limited energy, that broke down  the LD, but not competed burnt out it to short. Subsequent ESD  test indicated that the LD was very sensitive to ESD. Combining the information of above tests, bias circuit design  and the storage environment, we reached a conclusion that the  degradation was caused by a reverse polarity ESD event on the  LD. Some mechanism explanations are given to understand the  ESD-induced degradation and it was consist with the  observation of the ESD-induced punch holes.


### References


[1] Ondax 405nm, 12/25/40mW wavelength stabilized lasers, Rev.9


[2] MIL-STD-883 Rev.F


[3] M.Dal lago et al., “ESD on GaN-based LEDS: An analysis based on dynamic electroluminescence measurements and current waveforms”, Microelectronics Reliability 54(2014) 2138-2141.


[4] F. Magistrali et al., “ESD induced degradation mechanisms ofInGaAsP/InP lasers”, Quality and Reliability Eng. Int. 8, 287 (1992).


[5] Y. Twu et al., “Semiconductor laser damage due to human-bodymodelelectrostatic discharge”, J. Appl. Phys. 74, 1510 (1993).


[6] H. Ichikawa et al., “Analysis on reverse electrostatic dischargeinduced degradation of GaInAsP/InP laser diodes”, IndiumPhosphide and Related Materials, TuB-1-3 (2005).


[7] J. Wallon et al., “Sensitivity to electrostatic discharges of low-cost1.3 μm laser diodes”, Materials Science and Eng. B28, 314 (1994).


Failure Analysis of Embedded Non-Volatile Memory with Nano- and   Micro-Probing Techniques


Xiang-Dong Wang, Arnold Yazzie, John Buchert, Laurel Will, Ping Wang and Scott Guisinger


Freescale Semiconductor, Inc., Chandler, AZ  xiang-dong.wang@freescale.com


Embedded non-volatile memory (NVM) technologies are used  in almost all areas of semiconductor chip applications, as it  becomes increasingly vital to retain information when the  electronics power is off [1, 2]. While embedded NVM provides  much needed integrated solution for miniaturization and faster  data retrieving, it creates some unique challenges for failure  analysis. When a die is rejected by a test program in a wafer  prober, the failure characteristics are very limited. In a  conventional failure analysis approach, failed bits may only be  verified and characterized when the circuit is still functional. In  such case, the diagnosis setup in a FA lab could get complicated  by the interaction of the whole circuitry.


Figure 4: Write time degradation versus opposite data portion  for the shared ground line (black) and isolated ground line (red) configurations.


Figure 4 illustrates that the isolated ground line  configuration and the shared ground line configuration show  similar behaviour in Region A, which is the case with only one  Data 0 polarity cell.  However, the isolated ground case  showed reduced noise compared to the shared ground case.


The write time degradation is reduced from around 0.9 AU (arbitrary units) to 0.2 AU as the number of opposite (Data 0) polarity cells increases. The difference between the two cases  gives us insight into the origin of the sensing noise.  It also  drove us to propose use of a local ground line configuration to  solve the initial sensing failure caused by oppositely polarized  data cells inducing ground noise on a common word line.


A secondary source of noise is the power noise in the cell  array which is used the cell capacitor plate and bulk well and is  caused by sharing of the power mesh.  DRAM memory devices  require that the cell capacitor plate voltage and well bias  voltage in the cell array region are stable.  However, the in a  DRAM memory device the power nets are connected to each  other within common blocks of memory cells. Figure 5 shows  the correlation between distance of the noise source from the  oppositely polarized cell and tWR degradation. In order to  explain this relationship, we observed tWR is gradually  reduced while the oppositely polarized data group is gradually  increased in distance from the noise source. It was observed  that the influence of the noise source flattens out when the  oppositely polarized cell is positioned further than a  predetermined distance away from the failing cell position. This  phenomenon shows that there is a noise source which is caused  by sharing power in the DRAM cell array whose magnitude  varies with the distance from the source.


Figure 5: The illustration for oppositely polarized data group  position diagram (a). Write time degradation versus opposite  data group position (b).


Figure 6 shows the simulation results for two cases of data  pattern polarity. Case 1 is the solid data pattern which has  uniform data polarity of Data 0 in the word line activated. Case  2 has a pattern where most of the bits hold Data 1, with only  one cell holding the Data 0 state. The measured initial sensing  delta voltage revealed that the read time (tRD) increased 24% from the solid pattern case (all Data 0) to the opposite data  pattern case (one Data 0). This result shows that initial sensing  level is reduced by the portion of the opposite data polarity in  the cell array when the one word line is activated.


Figure 6: The simulated sensing voltage result of data pattern  polarity case.


A performance issue was identified after adoption of the  open bit line DRAM architecture for mass production when  tWR parameters degradation was observed.  We have shown  how write time degradation is caused by initial sensing noise  resulting from opposite data polarity memory cells.  This noise  results from use of a shared local ground line in the sense  amplifier region of the memory cells. It is clear that the noise  arising from cells holding oppositely polarized data is  composed of the sum of several mechanisms. The effects of the  noise can be overcome by using the separated local ground line  in the sense amplifier regions.


[1] Nak-jin Son, et al., “A Unique Dual-Poly Gate Technology  for 1.2V Mobile DRAM with Simple In-situ n+ -Doped  Polysilicon,” IEEE Transactions on Electron Devices, vol. 51, pp. 1644–1651, 2004.


[2] K. Itoh, et al., “Limitation and challenges of multigigabit  DRAM chip design,” IEEE J. Solid-State Circuits, vol. 32, no. 5, pp. 624–634, May 1997.


[3] Kinam Kim, et al., “DRAM Technology Perspective for  Gigabit Era”, IEEE Transactions on Electron Devices, Vol. 45, p598-608, 1998


[4] K. Kim and D. Park, “The future outlook of memory  devices,” Solid State Device Res. Conf. 2007, Sepember. 2007, pp. 47–147.


[5] K.Saino, et al., “Impact of gate-induced drain leakage  current on the tail distribution of DRAM data retention  time,” IEDM Technical Digest, pp 837-840, 2000


[6] C.-G. Hwang., “Semiconductor memories for IT era,” in  IEEE ISSCC Dig. Tech. Papers, 2002, pp. 24–27.


[7] T. Sekiguchi, et al., “A low-impedance open-bitline array  for multigigabit DRAM,” Solid-State Circuits, IEEE  Journal of, vol. 37, pp. 487-498, April. 2012.


[8] T. Takahashi, et. al., “A multigigabit DRAM technology  with 6F2 open-bitline cell, distributed overdriven sensing, and stacked-flash fuse,”


Laser Stimulation Effect on FinFET and Case Study


Kyeongju Jin, Sukho Lee, Keonil Kim, Yunwoo Lee, Yojoung Kim


Samsung Electronics Co. Ltd., Hwaseong-si, South Korea  kyeongju.jin@samsung.com


In the case of conventional planar FET, Dynamic Laser  Stimulation (DLS) is a very effective method to isolate  marginal failure. Depending on laser sources, DLS is divided  by Soft Defect Localization (SDL) and Laser Assisted Device  Alteration (LADA). SDL uses 1320nm wavelength laser  source in order to induce localized heat. On the other hand, LADA uses 1064nm wavelength laser source to generate  photo carriers. But for the FinFET the effect of laser  stimulation is not clear yet.


This paper introduces the effect of laser stimulation on  FinFET transistors based on wavelength, the so called LADA  and two-photon LADA. The experimental data show changes  in Vth and Idsat with different character for a single FinFET  transistor. A case study further explains this laser stimulation  effect via scan chain LVcc marginal failure analysis localized  with 1320nm CW laser stimulation and nano-probing analysis.


It is generally accepted that there are two types of DLS  applications[1], [2]based on the wavelength of the light source. LADA(1064nm) is generally appropriate for failures related to  transistor performance by affected by photo current effect  while SDL(1320nm) is more suitable for soft defects related to  metal or via open/short due to local heating effects. Recently  another stimulation effect has been reported – the so called  two-photon LADA.[3], [4]


This paper introduces experimental data illustrating how  single FinFET transistor characteristics are changed by  1064nm and 1320nm laser beam injection. This result  indicates which characteristic is the most significant to change  the pass/fail results of the marginal failure. A case study is  provided to expand the understanding of the laser stimulation  effect from a single transistor into a functional failure analysis.


Laser stimulation Experiment


For this experiment, we used an isolated single transistor  with probe pads to enable manual probing in the scribe lane  area. The laser beam was injected with a Meridian WS which  has both a 1064nm and a 1320nm laser source. An HP4156C  was also used for electrical biasing and measurement.


Figure 1 Vg-Id curve trace results with 1320nm laser.


Figure 2 Vg-Id curve trace results with 1064nm laser.


Figures 1 and 2 show Vg-Id curve trace results with 1320nm  and 1064nm laser stimulation. In the case of PMOS with  1064nm laser source, we immediately observed unstable and  abnormally high Id current when laser power is above 50mV. We can assume that this current was from electron hole pair  generation between N-well and P-sub.


Figures 3, 4, and 5 show Vth, Idsat, and Idoff shift  respectively according to laser power. We recognize that there  is considerable Vth change with both 1320nm and 1064nm  laser source, but the values of Pmos Vth shift and Idoff shift  are also unstable with 1064nm laser. Therefore, we believe the  1320nm laser provides a more stable and predictable Vth shift. For Idsat shift, the 1320nm laser provides little effect to either  NMOS or PMOS while the1064nm laser gives Idsat gain to  PMOS.


Figure 3 Vth shift according to Laser power.


Figure 4 Idsat shift according to Laser power.


Figure 5 Idoff shift according to Laser power.


Figure 6 and 7 show Vd-Id curve trace results of a junction  diode with the 1320nm and 1064nm laser. As we can see in  Figure 2 in the case of Nwell/P-sub with 1064nm laser source, abnormally high Id current is observed when laser power is  above 20mW in the reverse bias region.


Figure 6 Junction leakage shift according to Laser power (1320nm laser source).


Figure 7 Junction leakage shift according to Laser power (1064nm laser source).


The gap of junction leakage induced by each laser source of  1064nm and 1320nm is obvious in the reverse bias region. Figure8 shows this clearly. The Nwell/Psub leakage shift as a  function of laser power with 1064nm laser source is extremely  high. Based on this result, we can be sure that abnormally high  Idoff of PMOS with 1064nm laser stimulation results from  Nwell/Psub junction leakage.


Figure 8 Junction leakage shift according to Laser power.


From this experiment, the laser stimulation analysis  technique provides a good solution for Vth concerns. Since  only 1064nm stimulation creates a substantial effect on PMOS, it should apply only to failures related to Idsat.


Case Study: Scan Chain Low Voltage marginal  fail


Scan chain failure analysis is one of the most important for  logic yield enhancement. As a result, a great deal of FA efforts  is focused on scan chain debug in the early stage of process  development. For hard failures, LVI/LVP is a good technique  for fault isolation, but it is time-consuming and limited due to  probing signal at small features. For marginal failures, we can  use LVI, but DLS saves time and indicates the exact fault  location.


Figure 9 Shmoo plot for a fail and a reference sample.


The shmoo plot of a fail sample shows over 100mV lack of  low voltage margin compared to a reference sample as shown  in Figure 9. The output data of scan chain is “0011” at pass  voltage but the data changed to “0111” at fail voltage. This is  commonly known as hold violation failure because the  following data is changed 1 cycle faster. Hold violation is  simply expressed as “fast data” or “slow clock”.


Figure 10 Laser stimulation result with 1320nm Laser.


Figure 11 F/F schematic.


Figure10 is DLS result using 1320nm laser source by  scanning the fail candidate region and the green spot shows  the area on the device where laser stimulation is causing the  test result to change from fail to pass. In other words, there is  sufficient device alteration to change the test result at this  localized area. The voltage margin critical node found by DLS  is the NMOS region of the clock driver and the clock is  critical for hold violation. Generally, a slow clock signal  generates a hold violation fault, so it is also possible that slow  NMOS clock driver performance induced poor low voltage  margin.


Figure 12 Shmoo plot with laser stimulation on failing F/F.


To confirm the laser effect on the location, shmoo plots (Figure 12) show 100mV margin improvement with laser on  and off. This suggests that the clock driver is the only unique  timing critical node which is available to improve low voltage  margin up to 100mV.


Figure 13 Nano-probing results at clock Nmos.


Electrical characteristic analysis with nano-probing  confirmed the NMOS at the failure location is 60mV slower  than its neighbor. This confirms the laser stimulation effect at  a single transistor is related to functional voltage marginal  failure.


In this paper, we evaluated transistor characteristic shift by  1064nm and 1320nm laser beam injection and found reliable  Vth shift for both NMOS and PMOS with a 1320nm laser. This knowledge was adapted to root cause scan chain low  voltage marginal failure analysis and used to identify the  timing critical location as the clock NMOS driver in the flipflop. Finally, this slow Vth compare to a neighboring site was  confirmed electrically with nano-probing analysis.


Laser stimulation techniques provide a powerful solution by  isolating the fault location with sensitivity to the timing  critical node.


[1] Jeremy A. Rowlette, Travis M. Eiles, “Critical Timing  Analysis in Microprocessors UsingNear-IR Laser Assisted  Device Alteration (LADA)”, ITC2003, p. 264.


[2] P. Perdu, “Fault Localization by Dynamic  LaserStimulationExtended Testing”, IPFA2009, p. 182.


[3] Kent Erington, Dan Bodoh, Kris Dickson, George  Lange,“The Role of Free Carrier Absorption in  LADA”,ISTFA2014, p.73.


[4] K.A. Serrels, N. Leslie, T.R. Lundquist, P. Vedagarbha, K. Erington, D. Bodoh,C. Farrell, D.T. Reid, “Two-PhotonAbsorption-Enhanced Laser-Assisted Device Alteration  andSingle-Event Upsets in 28 nm Silicon Integrated Circuits”, ISTFA2013, p.173.


[5] Sukho Lee, Keonil Kim, Yunwoo Lee, Euncheol Lee, Yojoung Kim, Izak Kapilevich, “Marginal Failure Diagnosed  with LADA-Case Studies”, ISTFA2014, p.367.


[6] SH Lee, YW Lee, KT Lee, CY Choi, “Case Study: Failure  analysis of functional shmoo hole with Laser Voltage  Probing”, ISTFA2009, p.193.


[7] Suk Ho Lee, Yun Woo Lee, Moo Jong Hong, Sung Jun  Yun, Eun Cheol Lee, Kyu Shik Hong, “New Failure Analysis  Method for Laser Voltage Probing (LVP)Utilizing System  Evaluation Board and Software.”, ISTFA2011, p.439.


Implementation of a Visual System to Manage and Improve   Failure Analysis Work Flow


Jason M Benz, Kevin A Distelhurst, Douglas B Hunt, and Rick Kontra


Global Foundries 1000 River Rd, Essex Jct. VT 05403


jason.benz@globalfoundries.com, 802-769-5941


Many articles and books have been written that discuss and  study the techniques of lean thinking and methodologies.  The  applications of these methodologies have included such  industries as manufacturing, health care, and information  technology.  Application to analytical laboratories has been  rare or non-existent due to the inability to apply lean


methodologies to a process with ‘unique’ analytical work


flows as well as a lack of a direct connection to the  manufacturing value stream.  The following paper describes  the work done in a semiconductor failure analysis laboratory to  visualize work flow, design a forecasting model, and create a  management system.  The result of which has been sustained  and improved quality, resource utilization, and delivery of  actionable root cause failure analysis.


The mission of the Physical Failure Analysis (PFA) laboratory  discussed in this paper encompasses many techniques within  fault isolation (PEM, LSM, MFI, XRT), mechanical  preparation, electrical isolation (NanoProbe, AFP), and  advanced materials characterization (SEM, FIB, SPM, TEM, Auger).  Analytical requests from internal customers (representing technology/product qualifications, reliability  monitoring, OEM, and Foundry products) flow into the PFA  process.  The individual laboratories that performed the  analyses in the PFA process operated as ‘islands of  functionality’ with no visibility of the entire end-to-end  process.  This has resulted in a process with high variability  with respect to cycle time, report content, quality of the data, etc.  From the customer’s point of view, PFA was a ‘black  box’ process lacking the infrastructure to provide job tracking  and scheduling, a single point-of-contact for the analysis, submission guidelines for enablement, and the ability to  communicate interim status and a final report.


In order to improve the PFA process the team employed Think  Process First (TPF), a concept that provides a methodology for  taking highly variable processes, achieving process stability, and mindfully improving the process.  By developing a process  that makes deviations, actual versus expected, visible and is  able to act and remove the root cause of the deviation, the  process and subsequently the results will continue to improve.


Visualize the PFA Process


The first step was to make the PFA process visible using a  Value Stream Mapping (VSM) technique [1, 2]. Once the  process was visible, the team established initial metrics to  monitor the PFA process.  In order to reduce variability and  achieve a stable PFA process an 8-step structured problem  solving methodology [3] was used which addressed problems  related to job scheduling, job tracking, and communications  both internal and external.  The problem solving teams  improved and resolved many of the customer issues.  The  specific methodologies used and actions implemented to  achieve improvements are discussed in more detail in  subsequent sections.


Elements of a Daily Management System


In order to sustain and continue to improve the process, a  Daily Management System (DMS) [4] was established.  The  team focused on four characteristics to implement a working  DMS in the failure analysis laboratory.  The first was to create  a visual control board, where engineers, technicians, and  managers could gather and easily visualize the workflow  currently in the laboratory.  The second was to clearly define  the responsibilities of the failure analysis team leaders for  tracking the work as it flows through the lab.  Thirdly, a daily  standup meeting of 15 minutes or less was established with the  team leaders, managers, and other key personnel to review the  workflow.  Finally, a continuous improvement system was  implemented to record and aggregate excursions, allowing the  team to use structured problem solving techniques to address  them.  These characteristics provided the framework for a  DMS that drives continuous improvement in the PFA process.


Establishing a Visual Control System


Mapping the Failure Analysis process


In order to create a visual representation of the failure analysis  process, the entire process needed to be mapped.  A structured  problem solving team was assembled to create a Value Stream  Map (VSM) for the process [1].  This team was immediately  confronted with the assumption that every job was unique and  could go through any number of failure analysis steps in any  order.  An overview map was created which grouped the steps  into areas of expertise, or ‘sectors’ as shown in Fig 1.  Then  representative fail types were selected (e.g. memory cell fail, logic fail, I/O fail) and mapped through the process.


Figure 1 (above): Value Stream Map of the overall failure analysis process. Areas of expertise are highlighted showing where indepth value stream maps were created.


It was found that while some fail types would skip various  steps, the order of all the steps was generally the same end-toend.


To further understand the process flow, the team went to visit  each sector, beginning with the last step which is the final  report.  By working backwards, problems could be tracked  upstream and more clearly understood.  Process flow, data  flow, cycle time, throughput, and places where queues develop  were also recorded as shown in Fig 2.  The purpose of figure 2  is to illustrate the use of value stream mapping as a tool to  show material and data flow.  The intent is to show the  complex nature of the process and the amount of work that  went into the analysis.  The details of the method and the  resulting map are not critical for the rest of the discussion.


Finally, the end-to-end process was divided into 11 steps that  represented a combination of various tools, techniques, and  most importantly where handoffs were being made to create  the framework for a visual control board as shown in Table 1  on the next page.  The steps were selected to be representative  of every process a failure analysis job could possibly go


through in a linear format, recognizing that not every job will  use all of the steps.


Figure 2: Example of an in-depth value stream map of the  TEM lab process.  Starbursts represent problems that get in  the way of doing the analysis.


Step Step Name


Included Processes


1 Engineering  Prep


Data review, preparing working aids, nondestructive electrical verification


2 Prep/Fault  Isolation


Package analysis (CSAM, X-Ray, MFI), liquid  crystal, sample prep needed for PEM


3 PEM Lab


PEM, LSM techniques


4 Data Review


Review fault isolation results, designer input, etc.


5 De-package / Delayer


Typical de-packaging and delayering of a part, bench probing if needed


6 Nano-probe / De-process


Nano-probing (SEM probes, AFP) and additional  deprocessing for probing at multiple levels


7 Advanced Data  Review


Review of electrical data, additional SEM work, decision point for advanced analysis (FIB, SPM, or TEM)


8 FIB Analysis


FIB Cross-section


9 SPM Lab


Various SPM techniques


10 TEM Lab


TEM cross-section or plan-view


11 Final Report/Job  Close


Inter-lock with customer and write final report


Table 1: List of failure analysis steps used to track the failure  analysis process.


Tier II Value Stream Meeting


Having the VSM of the PFA process provided the building  blocks required to understand the main avenues of job flow.  The next step was to observe jobs flowing through this value  stream.  Figure 3 is a modified embodiment of the VSM which  the team calls a value stream (VS) board.  All 11 steps span  across the top while several rows represent different demand  classes of jobs (e.g. RMAs, Qualifications, etc.).


A stand-up meeting, termed “Tier II VS Meeting”, is  performed several times a week in front of the VS board as  shown in Figure 4 with an allotted 15 minute time limit. The


engineering and management team members that decide the  movement of jobs are present at this meeting where the host  uses a script to lead a discussion.  The meetings are used to  discuss the priority of the jobs, buildup, and flow of jobs.  Actions items are set that would make sure priority is  communicated, sectors are prepared for excess work and that  jobs don’t fall behind from the lack of focus.  When jobs do  fall behind a prescribed schedule, provided by the forecasting  model, they are highlighted to the team such that the  appropriate business decisions can be made.


Figure 4:  Photo of value stream board and team members  during a daily standup meeting.


Figure 3: Modified VS board with all 11 steps (see Table 1) which are also called sectors across the top and example demand class  lanes (see Table 2) identified on the left.  Job tickets are placed on this type of board and moved accordingly.


Utilizing the System


Forecasting Model


The ability to predict the aggregate cycle-time of an analysis at  the time when the job was submitted into the value stream was  previously considered too complex.  The goals of the modeling  team were to reduce complexity and use existing cycle-time  data to produce a forecasting model that yielded target cycle  times with confidence bounds.


Some of the complexity factors often encountered were  differences in node-technology (e.g., 65 nm vs 22 nm), fail  type (e.g., logic, memory, etc.), analytical goals, priority, and  analytical path dependence on upstream results.  The  complexity factors were challenged using actual data from ~300 completed analyses during 1H2014.  The cycle time (Ct) data was segmented into three demand classes: product returns (RMA), product/technology qualifications, and ongoing  reliability monitoring (ORM) for manufacturing quality.  The  data clearly showed Ct (RMA) < Ct (Qualifications) < Ct (ORM) and was a good reflection of the overall mission  priorities.  Excluding the RMA demand class, where Ct was a  function of the JEDEC standard, there was minimal node  technology differences observed in the qualification and ORM  demand classes.  Another complexity factor was predicting the  analytical path, the techniques used to produce a root-cause  finding.  After interviewing the principle engineers, it was  determined that they could predict the analytical path based on  the analytical goals and fail type with high degree of  confidence during job submission.


The next step was to establish the key drivers of job  complexity and cycle-time.  Using demand class segmented  data, it was observed that node technology and priority factors  were not significant.  Assuming high confidence in the  analytical path chosen, fail type was found to be the only  additional key driver shown in Table 2.


Demand Class Fail Type


RMA


Qualifications


Mfg Reliability  Monitoring


Analog/HSS - IP macro or core typically involving  HSS (High-speed serial ) or PLL (Phase-lock loop) cores


I/O Open/Short - Severe pin leakage or resistance


I/O Parametric - Spec fail on an I/O pin typically  involving smaller amounts of leakage or resistance


Logic - Fail in the internal logic of the chip typically  requiring a significant amount of isolation


Memory SCF - Single Cell Fail (SCF) inside a  memory array.  For example a 6 transistor SRAM cell  Memory Pattern - Multi-cell (ie column, or word-line) fail inside a memory array.  May also include array  logic or block fails


Probe Protect/Iddq - Large chip Iddq or power failure  Other - Miscellaneous bucket for non-standard fails or  jobs submitted through non-standard processes


Table 2: Key Drivers for Predicative Cycle Time Model


The resultant forecasting model only has two key drivers, demand class and fail type, to predict cycle time. The main  reason for minimizing the number of key driver combinations  was the finite ability of this system to generate sufficient data  for the approximately 600 jobs/year in order to yield accurate  forecasting targets. Forecasting targets were established for  each analytical step in the process from Table 1 using a set of  tiered conditional queries designed to balance the key drivers ‘Level of Detail’ and the data population statistics as shown in  Table 3.


Condition Level of Detail Minimum


Population


Maximum  Population


Step/DC/Fail


Step/DC


Step


n/a


Table 3. Algorithm Conditional Queries


The algorithm will try condition 1, if that’s not successful it  will use condition 2, and if necessary default to condition 3  using the following rules for a particular analytical step:


Condition 1 - Use the Demand Class and Fail Type


a. Must have at least 10 data points


b. Target Ct is based on the 75th percentile job  based on a maximum of 20 data points


Condition 2 - Use the Demand Class & All Fail Types


c. Must have at least 4 data points


d. Ct is based on the 75th percentile job based on a  maximum of 50 data points


Condition 3 - All Demand Classes & Fail Types


e. Ct is based on the 75th percentile job based on a  maximum of 50 data points


When the minimum population criteria is met, the cycle time  for the 75th percentile job, by population, is written to the  database for that particular analytical step, demand class, and  fail type.  Currently the model update frequency is weekly and  contains approximately 11 months of data.  The model  population data for each step in the value stream as a function  of Demand Class is shown in Figure 5.


Figure 5: Value stream population matrix segmented by  Demand Class and Fail Type. The data block colors of green, yellow, or red indicate whether condition 1, 2, or 3 was met (i.e. pass vs. fail) respectively.


This matrix helps the team monitor the statistics behind the  TAT model for each step in PFA value stream as a function of  demand class and fail type. This data readily shows where the  highest population (i.e., workload) is throughout the value  stream and the level of detail used for the target cycle time (Ct) calculations for Table 3.


The TAT model algorithm provides a target cycle time for  each step in the analytical path of an analysis.  The summation  of target cycle time along the analytical path yields an  estimated completion date for the analysis.  The target cycle  time is compared to actual cycle time for each step in the  analytical path.  When actual cycle time exceeds target cycle


time the deviation is documented as a ‘miss’.  These  documented ‘misses’ are fed into a continuous improvement  process for further investigation.


Continuous Process Improvement (CPI)


A ‘miss’ is essentially a deviation from an expected target or


performance due to a process inhibitor.  The above sections  detail some of the visual aids and processes that are used to  capture, collect, and review some of these deviations.  For  example, one type of a miss encountered by the team included


Figure 1: Cross-section representation of the laminate used. Note that the trace through the laminate is just below the  copper power plane.


On one side of the sample denoted side 1, the copper power  plane is removed using surgical blades. Optical inspection  revealed little damage to the insulation above the traces and no  disturbance to the underlying traces. The other side of the  sample denoted side 2 only has the copper power plane  exposed. This is done so design features in the copper plane  are visible for alignment of CAD images if necessary. Mechanical abrasion is used to expose a portion of the copper  power plane above the area the net will be cut. Both nets were  electrically measured for further verification that no defects  were introduced.


Next, a cut is made in each net using a laser cutting system. An arbitrary location was chosen halfway along the side 1 net. Exposed vias that connected to the removed copper power  plane were used to navigate and ensure the cut was made in  the appropriate location. Likewise, clearance features in the  copper plane were used to navigate to a portion of the net and  ensure the cut was made in the appropriate location on side 2. The resulting cuts for side 1 and side 2 appear in Figure 2(a) and Figure 2(b), respectively.


Figure 2: Optical images of the cuts on side 1 and side 2. (a) The cut made in side 1. The vias that connected to the removed  power plane are visible. The underlying net that was cut is  partially visible through the insulator. (b) The cut made in  side 2. Features in the copper power plane are visible. Black  wax was added to both cuts after they were confirmed  electrically open.


The formation of the holes were monitored optically with a  camera system accompanying the laser head. The underlying  traces appeared as the cuts were being made and allowed the  status of the cut to be monitored. An electrical open was  confirmed on both sides after the lines appeared cut. Black  wax was subsequently filled into the holes to insulate the  exposed traces from conductive debris.


The part containing both sides was placed into the MFI tool. A  single probe contacted the BGA connecting to the side 1 net. Several SDR scans using the SQUID were performed. The  initial, low res scan (100µm) of the area around entire length  of the net observed the magnetic field up-until the cut after  which the signal began to drop off. The scan size was reduced  and the resolution set to 25µm. Figure 3(a) provides the CDM  of this scan and Figure 3(b) provides the infrared image (IR) image of the same area. Note the beginning of the copper  power plane near the left edge of Figure 3(b). An initial glance


of the CDM may indicate that no open exists. However, the  RF signal formed by the standing wave along the  superimposed line in Figure 3(a) is plotted with respect to  distance. Likewise to [4], the plot reveals a reduction in RF  signal over distance until it reaches a minimum. The linear fit  of the decay of this line is then used to find at what distance  the current drop may indicate an open. A cross in Figure 3  indicates this location.


Figure 3: (a) CDM with the superimposed line indicating the  distance plotted with respect to RF current. The  cross  indicates the location the current reaches the first minimum.


(b) The IR image of the scan area with the  cross translated  from (a).


Comparison of the cross location with the IR image of the cut  reveals an offset. Further, higher resolution SDR scans of  about 5µm are performed in an effort to reduce the offset. The  same linear fit is performed on the CDM and the probable  defect location is marked on an IR image of the scan area. The  IR image with the cross is overlaid with a CAD image in  Figure 4. The location of the cut in the net of interest is  highlighted by an arrow. The overlay reveals that the higher  resolution scan provided a closer approximation of the open.  In many cases, this approximation and even a lower resolution  approximation is sufficient to begin destructive analysis or  closer indirect inspection with techniques such as XRT.


Figure 4: IR image of side 1 with a cross indicating calculated  location of the open defect. The image is overlaid with a CAD  image to visualize the accuracy and the location of the open  along the net. The arrow indicates the location of the  manufactured open.


An SDR scan of side 2 is then performed. Likewise to side 1, a  lower resolution scan of the entire net is obtained followed by  higher resolution (2µm), small area scan to reduce the offset. Even with the copper power plane above the net, a signal is  still observed. The signal strength is reduced but the data is  sufficient in providing the approximate location of the open. An IR and CAD image overlay is provided in Figure 5.


Figure 5: IR image of side 2 with a  cross indicating calculated  location of the open defect. The image is overlaid with a CAD  image to visualize the accuracy and the location of the open  along the net. The arrow indicates the location of the  manufactured open.


Low resolution SDR scans of an open manufactured along a  net using a laser cutting system provides a reasonable  approximation of the defect spatial location. Higher resolution  scans reduce the offset which could be useful in applications  were more accurate results are needed (e.g. finding subtle  defects). A net buried under a copper power plane which may  act as an RF shield is also analyzed. Although a reduction in  signal is observed, accurate results are still obtained and useful  for further analysis. Further experimentation on thicker  laminates with more copper planes and different materials is  still needed to understand the viability of this method in more  diverse applications. However, this technique is capable of  locating open defects even with certain obstacles.


[1]  D. P. Vallet, D. A. Bader, V. V. Talanov, J. Guadestad, N.


Gagliolo and A. Orozco, "Localization of Dead Open in a


Solder Bump by Space Domain Reflectomery," ISTFA


2012: Conference proceedings from the 38th International


Symposium for Testing and Failure Analysis, p. 4, 2012.


[2]  J. Gaudestad, A. Orozco, M. Kimball, K. Gopinadhan and


T. Venkatesan, "Short Localization in a Multi Chip BGA


Package," IEEE 21st International Symposium on the


Physical and Failure Analysis of Integrated Circuits, p.


74, 2014.


[3]  J. Gaudestad, N. Gagliolo and V. V. Talanov, "High


Resolution Magnetic Current Imaging for Die Level Short


Localization," 20th IEEE Internaional Symposium on the


Physical and Failure Analysis of Intergrated Circuits


(ITSFA), p. 355, 2013.


[4]  J. Gaudestad, V. Talanov, N. Gagliolo and A. Orozco,


"Space Domain Reflectometry for Open Failure


Localization," 19th International Symposium Physical &


Failure Analysis of Integrated Circuits, p. 1, 2012.


Symptom or Cause? A Case Study


Anuradha Swaminathan, Joy Liao and Howard Marks


NVIDIA, 2701 San Tomas Expressway, Santa Clara, CA 95050 USA


Contact:aswaminathan@nvidia.com


Although we have at our disposal many advanced technologies  and techniques for silicon diagnostics, effective failure  analysis to root cause is getting increasingly challenging, as  very often the electrical failure analysis (EFA) data would  point to a symptom that is the result of the defect rather than  the actual location of the defect.  Therefore, we often employ a  combination of multiple techniques so that we can further  observe sensitivity of ‘the cause of the problem’ and  understand why certain effects are better defect indicators than  others.  This work compiles successful analysis with the aid of  Continuous Wave Laser Voltage Probing (CW-LVP) [1] and  Soft Defect Localization (SDL) [2] techniques. Three cases  presented in this paper are voltage-sensitive (VMIN) fails.


Case Study #1. Voltage sensitive at-speed failure.


The first case study is a 28 nm device which failed at-speed  scan. Software diagnostics pointed to multiple callouts of  which ‘capture flop’ was one of the candidates. Continuous  Wave Laser Voltage Probing (CW-LVP) [1] was performed  while executing the failing pattern in a loop. Simulating the  failing pattern for the cone of logic under investigation, we  compared the CW-LVP [1] results to the simulation and  identified the faulty node. The ‘capture flop’ was observed to  be faulty.


To further isolate the voltage-sensitive defect, SDL with  1340nm laser was performed and revealed a fail-to-pass site  within the flop.  Figure1 shows the results of simulation, CWLVP, and SDL of the ‘capture flop’.


Physical failure analysis (PFA) recommendation was to target  the fail-to-pass location within the flop. PFA showed a highresistance contact (that was under-etched) at the exact location  of the fail-to-pass site.


Figure 1. CW-LVP at ‘capture flop’ location and comparison  with simulation (top).  Fail-to-pass site observed with SDL (1340nm laser) at the failing flop (bottom right).


Case Study #2. High Vmin RAM register BIST fail.


The second case study is a 28 nm device failing RAM register  BIST with high Vmin. Bitmap identified 2 adjacent columns  failing.


To study the laser effect on the failure, we parked the 1064nm  laser at two different sites inside the region which contains the  2 failing columns, and performed shmoo on ATE.


(a) Shmoo with laser parked at site A (red circle) of the  failing region.  Passing region started at  VDD~0.735V.


(b) Shmoo with laser parked at site B (red circle) of the  failing region.  Passing regions started at  VDD~0.875V.


(c) Shmoo with no laser (SIL landed on the failing  region.)  Passing region started at VDD~0.88V.


Figure 2. Shmoo plots showing sensitivity with laser at the site  sensitive to laser (a) and the site insensitive to laser (b).  Vmin  shifted almost 0.14V.  (c) Reference Shmoo with SIL  contacting the failing region without laser. SDL was performed  using the MBIST pattern. A fail-to-pass site was observed at  the sense-amp area (Figure 3). SDL comes in handy for BIST  failures with unstructured patterns where CW-LVP looping is  not possible.


Figure 3. Fail-to-pass site with SDL [2] (1064nm)


Case Study #3.  Scan shift failure exhibiting transition  behavior


The third case study is a scan shift failure in a <28nm device.


A binary search using laser modulation mapping at the 2nd  harmonic [1] of the data frequency revealed that the output  was a transition fault: data patterns changing from  11001100… to 10001000… Probing of the Q output of flop  C143 confirmed that the output data was 10001000…


Figure 4. Second harmonic modulation mapping showing   second harmonic throughout flop C143 but normal passing  flop signature for flops C144 and C145.


Soft defect localization at the suspect flop area showed a failto-pass site and a pass-to-fail site at flop C144, the flop  preceding C143. Laser effect on C144 pushed the failure to  pass; therefore, Modulation mapping using second harmonic  and CW-LVP could not isolate C144 as the failing flop.


Figure 5. CW-Laser Voltage Probing at C145,C144, and  C143. C144 did not exhibit failure due to laser effect.


C144/Q


Passing- not


exhibiting transition  due to laser effect


C144


C145  C143


Figure 6. 1340nm LSM image showing C144 (red) and C143 (yellow).  SDL results -Fail-to-pass site (left, green spot) and  pass-to-fail site (right, red spot) appear at C144 (red).


PFA confirmed failure at the fail-to-pass site within flop C144.


SDL Technique- Synchronous mode


Soft defect localization can be enabled in two modes. This  case study uses SDL in synchronous mode [3], using two  trigger signals: one for pixel clock to move the LSM scan pixel  by pixel and another for the pass-fail signal from the  test/tester.


This setup is illustrated in Figure 7a. A timing diagram (Figure  7b) showing the signals involved summarizes this mode. This  is a case where the device under test is set up in a mostly  failing voltage and laser interaction causes the fail to pass.


Figure 7.(a) SDL Technique- Synchronous mode  setup , (b) Timing diagram


Soft defect localization for voltage sensitive fails has proven to  be efficient for isolating the cause of the failure. PFA results  confirm that the laser stimulated fail-to-pass sites are defect  indicators.  In the cases when laser interaction is strong enough  to cause the CW-LVP signal to look correct (pushing to pass), SDL comes in very handy.


Thanks to Roy Ng for successful bring-up of SDL at NVIDIA.


[1] Steven Kasapi et al., “Advanced Scan Chain Failure  Analysis Using Laser Modulation Mapping and Continuous  Wave Probing”, ISTFA 2011


[2] M.R. Bruce et al., “Soft Defect Localization”, ISTFA 2002


[3] Izak Kapi Kapilevich, DCG Systems Inc., CA, Application  notes for SDL.


Logic LIVA Fault Isolation in Synthesized Logic


T. Pifer and T. M. Eiles


Intel Corporation, Technology Manufacturing Group Labs, 2501 NW 229th Ave, Hillsboro, OR 97124. Tim.j.pifer@intel.com, travis.eiles@intel.com


InfraRed Emission Microscopy (IREM) is often the simplest  and fastest Fault Isolation (FI) technique. But with the reduction  of leakage in advanced technologies, transistors emit fewer  photons, particularly at low power supply voltage levels.  It is  also more difficult to gain the needed spatial resolution to  identify emitting devices.  These factors reduce the number of  cases in which IREM can adequately localize the defect, requiring additional effort in nano-probing and physical failure  analysis.


In contrast to emission microscopy, laser-based techniques such  as TIVA (thermally induced voltage alteration) and LIVA (light  induced voltage alteration) are not as dependent on leakage or  the specific voltage of the defect to provide localization, but are  able to observe variations in the defective current drawn by the  defect. For this reason, variations of these techniques can  provide additional information when IREM does not provide a  satisfactory localization. Applying LIVA to logic devices on the  main power plane can complement IREM.  Additionally, these  techniques are able to differentiate between open and short  circuits by measuring the change in power supply current. For  a transistor driving into a short, the laser can increase the drive  strength, which increases the overall current the DUT is  consuming.  On the other hand, transistors that have an  indeterminate voltage level on the gate (due to an open, for  example) may reduce the current drive due to a shift in the  threshold with the presence of the laser. While performing this


technique, one can also observe the thermal effects of the laser  which can be seen as the increase


in resistance at a short, resulting in a reduction in the total  current.


This paper describes a method of applying LIVA to synthesized  logic connected to large-scale power plane by controlling the  amount of decoupling capacitance on the power supply.  This  has proven to provide very useful fault isolation beyond what is  possible with emission microscopy.


Methods


The basic physical setup for Logic LIVA has the same hardware  requirements as standard TIVA or LIVA, the difference is in  the electrical connection. We will use LIVA to refer to both  standard TIVA and LIVA as the hardware setup is similar.  For  Logic LIVA, we use the LIVA supply to power the entire logic  plane where the failure is expected based on electrical data, as  shown in Figure 1. The LIVA supply drives the voltage  required to power and run the logic in the failing state.  Once  the integrated circuit is in the appropriate failing state, in this  case the internal net is set to zero; the laser will stimulate a small  change in the current drawn by the defective device. The  primary difference between this technique and standard LIVA  is that the defective device will only contribute a minor portion  of the total current driven by the supply. Standard LIVA, on the  other hand, is often applied to IO pins which do not normally  draw much current; that is, the majority of the current supplied


Figure 1. Basic Logic LIVA schematic. LIVA supply is connected to the Logic power plane. Variations of current in


the transistor driving a current are observed on the supply.


to the circuit is passing directly through the defect. Logic LIVA  is therefore a more subtle effect, but even using the standard  hardware, we are able to observe small variations in current in  one transistor while it is connected to millions of others in  parallel.


However, we have encountered limitations on the ability to  observe signals at higher power supply currents in large logic  blocks. The LIVA supply we are using is able to source 100 mA  of current, but we are not able to reliably observe signals when  the DC current is above 30 mA; the technique has proven most  successful below 10 mA. To observe some of the more subtle  signals, it is often necessary to average the image 50 times or  more and some signals have not become obvious until hundreds  of images are averaged.


Logic LIVA relies on the laser causing variations in the current  on the power supply. However, large amounts of capacitance  are often added to the test motherboard to prevent such current  variations and to ensure a steady voltage level.  In turn, this  capacitance degrades the LIVA signals as it filter out rapid  current changes that create the signal.  This effect is illustrated  in Figure 2, which shows several LIVA images taken with  increase amounts of capacitance added to the power supply rail.  One can see that even with a strong signal a relatively small  capacitance of 100uF drastically diminishes the signal and  470uF almost entirely eliminate it. Board power supplies, especially in a test environment, can have a high quantity of  capacitance, even into the tens of millifarads; hundreds of times  greater than the acceptable capacitance.


This board capacitance is added to provide stability to the  power supply while running. During reset and while the device  is clocked the capacitance prevents the voltage from drooping  during current spikes. If the capacitance is not present while the  clock is running these droops will cause a loss of state and one  will not be able to exercise the defect.


To enable logic LIVA, while avoiding power droops during  reset, we use a relay-based circuit to provide a switchover from  a power plane with added capacitance to a low-capacitance  plane for LIVA. Good board design practices place the  capacitors as close to the DUT as possible to minimize the  impedance. The switching mechanism for connecting the  capacitors needs to be given the same considerations, so a relay  near the DUT is the best way to minimize the wiring distance. Figure 3 provides an example of the relay based switchover  circuit, where the capacitive board supply can be connected  through the relay on the left and the LIVA supply can be  connected by activating the relay on the right. To ensure the  device stays powered up we perform the following procedure. First, attach the capacitive plane, power up the device and reset  it and apply the pattern to get the device to the defective static  state. Then, following a “make-then-break” procedure, the  LIVA supply is connected while the capacitive supply is  disconnected.


We collected data using a system equipped with1064 nm and  1319 nm lasers and a solid immersion lens. Logic LIVA images  were collected using the 1319 nm laser. Our first case study is  a 40 nm process technology sample with a failing array, but no


Figure 3. Schematic showing relay switchover board. Left side relay connects the DUT to the capacitive board  supply, while the relay on the right connects to the LIVA supply.


Figure 2. LIVA response of a device driving into a short for various amounts of capacitance added to the power plane.


further test data. Figure 4 presents the overlay of an IREM  image in blue with a logic LIVA image in red.  Each emission  seen in the IREM image has a matching LIVA signal. The  LIVA result allows us to differentiate the transistors that are  driving current, which show up as dark at the bottom, from the  transistors that are receiving a poor logic level input which  show up as bright red.


Our second case is also a 40 nm sample which was submitted  to FA with a bit-line to word-line short but, translation to a  physical location was not available for this device. Initially, the  sample was imaged using IREM which identified a large  emission in the array and the shorted bit-line, but it could not  identify the word-line. The logic LIVA result shown in Figure


5 allowed us to determine the locations of the two emissions  seen in the IREM image as well as the word-line driver. This  result provides a complete picture of the failure the exact wordline driver simplified physical failure analysis.


On low-current power planes, Logic LIVA can be used to  elaborate on initial IREM results and provide further distinction  between shorted and open nets. The large capacitance built into  load-boards currently prevents the use of this technique for  many IC devices, but a relay-based modification is used to  enable Logic LIVA. In real world cases, this technique has  proved useful in providing a more complete picture of the  failure while the device is intact, reducing the need to localize  it using more invasive means such as nano-probing.


Figure 4. 40 nm sample with a defect in SRAM logic. Emissions  are shown in blue, while the LIVA signal is shown in red. Dark  LIVA locations indicate an increase in current and bright spots  indicate a decrease in current.


Figure 5. 40 nm SRAM array in LIVA where blue indicates  increased current consumption and green indicates reduced  consumption. A) Word-line driver signal B) location of short. C) Bit-line signal


How to Locate Resistance VIA by Analysing Schematic Combined with EMMI Result on  Integrated Circuit Failed at Cold Temperature


Gaojie Wen, Li Tian, Jinglong Li, Changyan Qi, Dong Wang


PA Lab of Freescale Semiconductor, TianJin, China  B16245@freescale.com, 86-22-85684205


Due to the decreasing metal line size on complicated integrated  circuit, non-destructive analysis strategy such as EMMI (Emission Microscope) is very significant to failure analysis, especially when special cold temperature failures are  encountered. When combined with efficient schematic and  layout analysis, the real defect can be localized without much  microprobe work.


Since the characteristic dimensions of integrated circuit (IC) is decreasing all the time and functions becoming increasingly  complex, failure analysis is facing more challenges than ever  before to find the root cause efficiently. This is especially when  met with special functional failures which only happened at cold  temperature. Under these conditions, the effective application of  non-destructive analysis methods can be challenging to failure  analysis.


As modern ICs need to operate under harsh conditions, for  instance, cold or high temperature, increased moisture and  electronic noise, more uncommon functional failures happened, such as hot and cold temperature failures are expected. Cold  temperature failure is challenging as it is difficult to manage  potential moisture accumulation or handle complicated cold  temperature equipment. Performing microprobe work on cold  temperature failed samples could lead to potential damage risk  caused by conductive moisture. In this work, the cold  temperature environment is achieved using a custom-built  cooling unit which comprises of a thermal cooler within an  isolation box where the evaluation board reside in. The cooling  unit has a small window on top side to allow access by light or  laser beam. There are also two openings to maintain a constant  air flow using a fan and moisture is unable to settle on the die  surfaces and left to freeze. In this way, cold temperature failures  ICs can be analysed. For many ICs which only failed at cold  temperature, resistive VIA or contact was the main issue on


0.25m technology integrated circuit. EMMI analysis is a  well-known non-destructive method in analysing functional  failure ICs. When the integrated circuit is configured in such  cold fail mode, more electron hole pairs would recombine and  emit photons which can be detected by CCD or InGaAs camera. This can be displayed on screen. Having acquired the hot spots, familiarity with the fundamentals of EMMI and the  interpretation of signal shape will determine the success in  isolating the most critical and abnormal spot. The ability to


analyse the isolated abnormal emitted spot with layout and  schematic would greatly affect the success in revealing the root  cause accurately in subsequent failure analysis step.


Two real cases will be presented in this paper to demonstrate  the effectiveness of analysing EMMI result at room temperature  and cold temperature, in combination with schematic and layout  study to reveal resistive VIA defects successfully.


Experiments and Results (Case1)


One mixed signal IC which comprises of both analog and  digital circuits was returned by customer due to abnormal  RESET signal at cold temperature (CT) (0°C) test. The failure  would disappear and pass the Auto Test Equipment (ATE) at  room temperature (RT) (25°C), and high temperature (120°C). It was a cold temperature RESET failure (Fig.1). The failure  mechanism should be related to signal metal line conducting  issue, rather than hard defects like resistance short or leakages.


After decapsulation, EMMI analysis was performed first at  room temperature and no abnormal emitted spot was found.   EMMI was performed again at cold temperature (0°C) and this  time, several abnormal emission spots were detected in the logic  module (Fig.2). This suggests that the abnormal emitted spots in  logic directly related to the failure at cold temperature. Schematic analysis revealed that the failed RESET signal was  controlled by logic module directly and a logic failure can  explain the RESET failure well. However, the defect is still  indeterminate at this step. It was always difficult to analyse the  logic due to the complicated logic control and feedback effect. Using micro probing directly in logic regions is not feasible  because it would take a long time.


Abnormal no wave


Normal


Figure 1: RESET signal was normal at room temperature (25°C) and failed at cold temperature (0°C).


RT


CT


RESET  VDD


Detailed analysis on the schematic and layout focused on the  vicinity of the abnormal emitted spots. There were 10 abnormal  emitted spots in total- 9 emitted spots in D flip flops, and 1 in an  inverter—U1274_L7_I8, all of which related to one signal  named CLK_L7. It can be hypothesize that the 9 abnormal  emitted spots in D flip flops were a result of abnormal CLK_L7  signal as this explains 9 defects in the 9 D flip flops (Fig.3). The  next step was to isolate the real defect location along the entire  suspected path through CLK_L7. The answer is clear from  schematic analysis.


The input signal to the abnormal emitted inverter was  CLK_L6. It also connects to another inverter—U1274_L7_I7  cell. Should CLK_L6 signal failed, there should be another  abnormal saturated emitted spot in U1274_L7_I7 inverter cell, but there does not exist. This indicates the path from CLK_L6  signal to the U1274_L7_I7 inverter is normal. For the abnormal  emitted spot in U1274_L7_I8 inverter cell, it was more a  saturated emitted spot than a real defect location. The real defect  emitted spot is always a single and cycle spot on part POLY  Gate of a MOSFET, not the whole POLY. Combined with past  experience on cold temperature failure mechanism that it is  likely related to VIA or contact conductive issue, the suspected  path should be on CLK_L6 signal to the Gate of  inverter—U1274_L7_I8 cell. Layout was checked based on the  CLK_L6 signal metal line, and suspected VIA2, VIA1 and  contact were located near the U1274_L7_I8 cell (Fig.4). They  were vertical when viewed from the top on layout and it was  easy to see the whole interconnecting stack which includes  VIA2, VIA1 and contact on one cross section cut. This approach  combining schematic and layout analysis based on the EMMI  result and past experience successfully isolates the failure on the  VIA without much probe work. Much analysis time is saved.


a situation where a technician working in the TEM lab was  preparing a sample for use in a FIB tool.  Based on knowledge  and experience the technician might expect the job to be  completed by the end of the shift.  However, due to some tool  errors the job was delayed and did not complete until the next  shift.


Historically problems that prevented individuals from  performing their daily tasks were generally tolerated, not  communicated, and constantly worked around.  The typical  situation with organizations that do not focus on continuous  improvement is that these temporary work-around solutions or  fire-fighting techniques never resolve the root cause.  Hard  working, well-meaning individuals then spend a lot of time and  effort solving the same problem over and over again [5].  In  the above example, the VS boards and processes help identify  and communicate that particular tool issue to the larger group, where in the past it was largely ignored.


The simple act of recording, communicating, and discussing  the misses in a larger group was a significant step towards  improvement.  However, what happens with all that data?  Are  any actions being taken to address the root-cause of the miss or


process inhibitor to ensure that it doesn’t happen again?  Was


the miss a one-time event or does it appear to be systematic?  Is there a larger more complex issue that could be resolved and  help improve efficiency?


Figure 6, which looked at the number of misses by the steps in  the VS, illustrates an example of how some of the data was  visualized in an attempt to look for systematics, or majority  mechanisms.


The data in figure 6, as an example, suggests a large portion of  the misses fell in the TEM step of the VS.  An investigation  into those misses revealed that the TEM analyses performed  were more complex due to a subtle defect mechanism and the  additional sample preparation required for such an analysis.


The next and most difficult phase for the CPI process was to  now attempt to drive improvements based on the data  observed.  As in the TEM example, the opportunity to learn  that these particular types of samples take longer allows the  team to potentially adjust resources and/or document the  process that was used.  Therefore, resources or process  development time is not wasted when these types of fails are  observed in the future.


Figure 6: Bar chart showing the number of misses the team  cataloged over a month separated by the steps in the valuesteam map (VSM).


One of the most challenging aspects with attempting to resolve  identified issues often revolves around resource and the overall  business culture.  The culture or the business has to have the  ambition and drive to focus on continuous improvement and  provide people with time to work on such activities.  Convincing people that there is a problem generally is not an  issue.  Asking people to find the time from their daily activities  and pressures to spend time on continuous improvement can  often be very difficult.


The team has taken the first step towards changing and  improving our culture by first publicly recognizing and  identifying opportunities for improvement.  There will  constantly be challenges from the business to provide  opportunities to focus on complex root cause fixes, but with  some emphasis on continued improvement there is an  expectation that it will start to come naturally.


Case Studies and Examples


Decrease PFA Cycle Time and Variability


If we look back at the past 12 months and compare the PFA  average cycle time for the various demand classes the trend  shows less cycle time variability and lower average cycle time  as shown in Figure 7.  This has allowed mindful and proactive  job prioritization commensurate with the needs of the business.


The typical communication churn addressing “Where is my  sample?  When is it going to be done?” have been reduced


significantly.  The PFA system can now handle more jobs  which impacts qualification schedules, yields, etc.  How is this  possible? What components of the Visual Management System  drove these improvements?


Figure 7: Average cycle-times over a 12-month period as a  function of demand class. The data shows decreasing cycletime variability and average cycle time.


The most important part of the management system was the  daily 15-minute standup meeting that was attended by  managers and engineers representing most areas of the value  stream. This allowed for rapid communication and includes  some of the following discussion points:


1. Jobs that changed status (green to yellow to red)


2. Jobs that are idle (no resources available)


3. Priority calls between jobs


4. Proactive awareness for the need to move resource to  another step in the value stream in the future


5. Tool status and scheduled preventative maintenance


6. Accountability for TAT target misses


Forecast-based Proactive Resource Utilization


The ability to move resource when and where it is most needed  is an ongoing improvement activity that relies on an effective  cross-training program. The cross-training program was  initiated based on data from the management system that  showed current TEM sample output was not sufficient to meet  projected input from the Qualifications demand class as shown  in Figure 8.


If the TEM laboratory could not increase output by 1.2  samples per week, significant overtime would have been  required to mitigate an approximately 15 sample deficit.


This would have impacted the product qualification schedules  and analyses from other demand classes.


The TEM team was challenged with reducing cycle time and  training additional resources to perform basic mechanical and  FIB sample preparation.  Cross training consisted of two  phases, learning the skills followed by an ongoing skills  maintenance plan that ensured the individual could perform the  skill when needed.


Figure 8: 2014 forecasted demand for TEM analysis by  quarter. The forecast showed that demand would be much  greater than capacity for Q3.


The cross-training skills are managed by separate visual  system.  The visuals clearly show cross-training maintenance  requirements for all trained individuals.  The Tier II board  helps to identify additional areas for cross training.


The ability to “see” how jobs flow through the value stream


and calculate the overall step utilization, such as what  percentage of qualifications fails utilize TEM, was paramount  to forecasting future resource demands.


Priority Calls


Prior to establishing a daily management system, priority calls  were handled haphazardly.  Team leaders would have to make  calls based on their own customer input, without a larger  picture of the business.  Sector leaders were often making calls  based on past history, knowing which products got the most  attention in the past.   Management might make calls based on  phone calls they received, without having visibility to the  entire workflow in the lab.  As a result, jobs that were


legitimately important, but didn’t have a champion, would


often languish.  Also, a routine analysis would often get outprioritized at various steps along the process over and over, as  there would always be a higher priority job ahead of them, leading to unacceptably long turnaround times.


After establishing the daily management system, priority calls  can now be handled with everyone present at the daily standup  meeting.  At every meeting team leaders are questioned if any  jobs need a priority call.  If so, other team leaders can speak  up if it looks like the call would affect their jobs adversely, and  management can confirm if the call is needed.  Sector leaders  are present, so they can prepare to handle the job if it is headed  their way while still maintaining routine analysis.


Ironically, since establishing this system, the number of jobs  identified as needing priority have gone down.  Having a daily  standup meeting has allowed everyone to visualize the entire  workload and exchange information so priority calls can be  made sparingly and with full visibility.


Ebbs and Flows Throughout the PFA Process


Although the visibility of jobs throughout the PFA process has  improved, there still exists a certain degree of unpredictable  behavior.  Some of this behavior stems from the timing of jobs  externally entering the PFA process.  This is further  exacerbated by nuances in the job such as difficulty in fault  analysis, insufficient data, and variability in preparation.  This  can lead to a build-up of jobs within a sector causing a  bottleneck for jobs upstream.


The addition of the VS (value stream) board clearly shows the  build-up of jobs in real time.  Prior to the VS board, build-ups  were not immediately visible to the entire PFA community.  Once a bottleneck was detected, a reactionary environment  was created and lasted long after the bubble was alleviated.  Some examples of this environment included excessive  overtime, forcing different techniques or tools, and escalation  battles which diverted scarce energy and resources.  Conversely, the VS board would visually show a depletion of  jobs in a sector.  This can and often indicated underutilized  staff assigned to that sector.


These observations led to a formalization of the cross-training  program.  This program was expanded beyond the crosstraining discussed earlier for TEM to include probe, and delayer skills.  The result of creating this dynamic workforce has  allowed for staff members to expand their skill sets, which led  to increased morale, and the ability to redeploy resources up  and down the value stream.


Figure 9: Modified VS similar to fig 3 with job tickets rearranged to visually show how a buildup in step 6 (probe  sector) is readily observable.


Figure 9 is a representation based on observed data showing  how quickly a person can walk up to the board and identify a  buildup where almost half of all the jobs are currently located  in step 6.  The goal of the team is to prevent such a buildup  from occuring, but if buildup does occur it is readily  observable by the entire team.  Armed with that knowledge,


the team can then make smart and quick decisions to help  ensure the buildup is handled effectively.


The cultural transformation process from a fire-fighting results  based organization to a process focused Lean driven  organization is a long and difficult journey.  This paper  describes some of the Lean activities and tools used to start  this cultural transformation in a semiconductor failure analysis  laboratory.  This transformation is a continuous process that  requires rigor, discipline, and the openness to making  problems visible.  The results to date have shown  improvements in process variability, data quality, cycle-time, and resource utilization.  There is significantly less time  expended on wasteful communications such as emails, phone  calls, meetings, etc.  The teams described in this paper have  made tremendous strides in reaching their goals.  However, the  transition is far from over as the teams continue to look ahead  and continue to push the culture and improve their processes to  meet future target conditions.


The authors would like to thank all the lean teams that  contributed to this effort including our facilitator and coach  Otto Funke, our team members Rob Calderoni, James Raboin, Bill Bentley, Phil Kaszuba, Greg Tomczyk, Mark Weymouth, Michael Pearce, Nick Pizzuti, Eric Marz, Alyssa Bawgus, Ron  Whitmore, Mike Coster, Doug Benoit, Joe Myers, Mike  Harris, James Salimeno III, Erik McCullen, and Daminda  Dahanayaka, and our sponsors and management for their  support including Connie Dollinger, Linda Miller, and Tami  Vize.  Of course a management system only represents the  efforts of the larger team and their accomplishments, all  without whom this would not be possible.


[1] Rother, Mike, and John Shook. Learning to See: Value


Stream Mapping to Create Value and Eliminate Muda.


Version 1.3. ed. Brookline, MA: Lean Enterprise Institute,


2003.


[2] Toast Value Stream Mapping. GBMP, 2009. DVD.


[3] Sobek, Durward K., and Art Smalley. Understanding A3  Thinking: A Critical Component of Toyota's PDCA


Management System. Boca Raton: CRC Press, 2008.


[4] Mann, David. Creating a Lean Culture: Tools to Sustain  Lean Conversions. New York: Productivity Press, 2005.


[5] Spear, Steven J. The High-Velocity Edge: How Market


Leaders Leverage Operational Excellence to Beat the


Competition. 2nd ed. New York: McGraw-Hill, 2009.


41st International Symposium for Testing and Failure Analysis  November 1–5, 2015, Portland, Oregon, USA


Copyright © 2015 ASM International® All rights reserved. asminternational.org


Comparison of Magnetic Field Imaging and Thermal Laser Stimulation for  Detecting Electrically Shorting Defects within a Die BEOL


Kevin A. Distelhurst


GLOBALFOUNDRIES, Essex Junction, VT, USA  kevin.distelhurst@globalfoundries.com


Magnetic Field Imaging (MFI) and Thermal Laser Stimulation (TLS) failure analysis (FA) techniques (e.g. OBIRCH, XIVA, ect.) both have advantages and disadvantages. The obstacles  encountered from these techniques may hinder further fault  isolation (FI), lengthen turn-around-time and/or detract from  actionable results. MFI using a Giant Magneto Resistance (GMR) sensor is compared to TLS techniques to understand  the capability of the MFI technique at finding shorting defects. A short within a capacitor bank is successfully isolated using  both techniques.


Having a variety of tools for die level FI and analysis provides  administrative options since no single technique can provide  universal coverage for all types of applications. For TLS  techniques, two criteria are required to detect the defects: the  sensitivity of defects to laser stimulation and adequate path for  the laser energy to reach the defects. MFI with a GMR is  capable of overcoming the TLS obstacles that may hinder  detection. However, certain criteria are also needed to detect a  defect with the MFI/GMR technique: sufficient current (>50uA) passing through the defect,  no obstruction by  ferromagnetic material, and the proximity of GMR within  roughly 10µm z-direction of the current. Using a  Superconducting Quantum Inference Device (SQUID), which  is also an MFI technique, can overcome most of the obstacles  presented by the GMR at the cost of reduced resolution. The  SQUID has demonstrated the ability to localize shorting  defects within TSV [1], on multichip packages [2] and on die


[3]. A comparison of both MFI and TLS is needed to  determine the feasibility of seamlessly interchanging which  technique is used.


MFI with a GMR sensor is capable of isolating electrically  shorting defects on a die [4], [5]. An example of a typical  GMR sensor setup is found and described in [4]. This setup is  used to map the current density, which is derived from the  magnetic field map, through a verified shorting defect on the  BEOL of an experimental die. An overlay and comparison of  the current density map (CDM) with the IR/NIR image in  combination with a CAD image of the die reveals the location  of the defect. TLS is also used to identify the location of the  defect by mapping the locations on a die sensitive to laser


energy. Likewise, overlay and comparison with the IR/NIR  and CAD image of the die localize the defect.


In this paper, a comparison between TLS and MFI with a  GMR is presented. In both cases, each technique is sufficient  in isolating the defect to a desirable area of interest (AOI). MFI is a useful technique as an alternative to TLS and when  TLS is not capable of isolating the defect.


Figure 1: (a) CAD image of the capacitor bank. The blue  represents the upper capacitor plate conductor in the BEOL  stack and the green represents the lower capacitor plate  conductor. The plates are separated by a dielectric and  connected to probe pads off image. Note that the entire bank is  not represented in this image. (b) XIVA signal (arrow) overlaid with the IR image. Fill patterns exist above the  capacitor bank and have no impact to this particular analysis.


Setup and Results using TLS


The sample used for analysis consists of various test  structures, one of which is a capacitor bank. A CAD image of  the capacitor bank is in Fig.1a. The bank consists of numerous  capacitors in parallel with one another. Each plate of each  capacitor is tied together and directly connected to a pad for  probe contact. The bank is localized to the first few levels of  the BEOL; that is, the furthest metallization levels from the  FEOL.


Figure 2: (a)Overlay of the CDM and CAD image; the scan lasted less than 30 minutes and has an XY spatial resolution of 4 µm. (b)An overlay of the CAD image and peak localization of the same scan as 2a. It provides a more defined path of the current. (c)Overlay of the CDM and CAD image; the scan lasted about 12 hours and has an XY spatial resolution of 0.3µm. (d)An overlay of  the CAD image and peak localization of the same scan as 2c. It provides a more defined path of the current.


Electrical 2-point DC measurement by contacting the two pads  with micromanipulator probes indicated an electrical short  when an electrical open is expected.


The sample was provided as a diced, die-level piece. The top  level passivation was removed prior to analysis using a dry  etch recipe. Several other samples with similar failures existed  and were used to identify the defect mechanism which was a  broken-down capacitor dielectric. The sample was loaded into  a laser scanning microscope setup for TLS. A pair of  micromanipulator probes contacted the pads connecting  between upper and lower plates of the capacitor bank. A slight  bias of 15 mV was applied which achieved about 600µA of  current.


The biasing readout also confirmed the electrical short still  existed. A 1340 nm laser was used to both image and  stimulate the defect. A reflected light image was first captured  to provide a structural (optical) image of the capacitor bank. Subsequently, XIVA imaging was performed and then  overlaid with the NIR structural image. The overlaid image  shows that one of the capacitors in the bank is sensitive to the  laser energy. The results are provided in Fig. 1b. The defect is  likely in the nearest adjacent capacitor, highlighted by a box in  Fig. 1a.


Setup and Results using MFI


The sample was then transferred to the MFI system.  A pair of  micromanipulator probes contacted the pads of the capacitor  bank. An AC bias of about 0.8 Vp-p was applied with about  450µA peak-to-peak current. Since the probes have about a


1300 Ω resistor in series with this setup, a higher bias voltage  was used. In all magnetic scans the sensor was approximately  1µm above the die surface observed in Fig. 1b. An initial low  resolution scan of 20 µm of the entire capacitor bank was  performed. A CDM was derived from the magnetic field map  and used to isolate and focus upon the AOI. A quick scan of  about 30 minutes at the AOI with a resolution of 4 µm showed  a strong current flow through one of the capacitors in the  bank. The higher resolution CDM was then overlaid with the  CAD image as shown in Fig. 2a. A peak localization of the  CDM was also obtained and overlaid with the CAD image in  Fig. 2b. A longer, 12-hour scan was performed with a  resolution of 0.3 µm. Likewise, the CDM was overlaid with  the CAD image resulting in Fig. 2c with a peak localization  shown in Fig. 2d. Although the longer scan provided a higher  resolution CDM, no significant differences between defect  localization was observed in the varying resolutions; a longer  scan was not required to provide accurate results. Both scans  localized the defect.


The CDM was compared to the CAD drawing to predict the  location of the defect by observing at what point the current  density crosses an unexpected boundary. In this case, a defect  was likely bridging the upper capacitor plate to the lower at  the point marked by an arrow in Fig. 2. The bridge was likely  through the dielectric as indicated in similar samples. An  overlay of the TLS NIR/XIVA image and the MFI peak  localization was produced and provided in Fig. 3 to further  illustrate this point.


The current density in both Fig. 2 and Fig. 3 doesn’t  completely align with the expected metal traces. The current


density appears to exist in a non-conducting region. This is  due to the magnetic fields from the upper and lower plate  interacting and shifting the apparent location of the current. The close proximity of the conducting traces and their 3D  separation should be considered during analysis.


Figure 3: Overlay of the MFI peak localization illustrating the  current flow through the defective capacitor and the TLS  NIR/XIVA image illustrating the location of laser sensitivity.


Both TLS and MFI techniques were capable of isolating the  defect to a single capacitor in the bank. MFI is capable of  isolating defects on the die using a GMR sensor. In certain  cases, MFI would be able to find the defect when TLS could  not. For example, when obstacles are blocking the defect from  laser energy, the CDM can be aligned with a CAD image to  achieve fault isolation. MFI also has the added benefit of  mapping the current density thus providing deeper insight into  how a defect may be altering the state of the circuit. In this  experiment, the current was shown to flow directly down one  path through the distributed upper plates of the bank, through  the defect, then directly back to the probe attached to the  lower plates.


Further work may identify unique instances when TLS fails to  isolate the defect. For instance, MFI can reveal the circuits  that should be the primary area of focus in cases where a  regional defect insensitive to TLS is causing abnormally large  current demands. MFI provides the analysis another technique  to isolate the diverse variety of defects for a successful, actionable analysis.


[1]  J. Gaudestad, A. Orozco, I. D. Wold, T. Wang, T.


Webers, R. Kelley, T. Morrison and S. Madala, "Failure


Analysis Work Flow for Electrical Shorts in Triple


Stacked 3D TSV Daisy Chains," ISTFA 2014:


Proceedings of the 40th International Symposium for


Testing and Failure Analysis, p. 5, 2014.


[2]  J. Gaudestad, A. Orozco, M. Kimball, K. Gopinadhan


and T. Venkatesan, "Short Localization in a Multi Chip


BGA Package," IEEE 21st International Symposium on


the Physical and Failure Analysis of Integrated Circuits,


p. 4, 2014.


[3]  D. P. Vallett, "Scanning SQUID Microscopy for Die


Level Fault Isolation," Proceedings from the 28th


International Symposium for Testing and Failure


Analysis, 2002.


[4]  J. Gaudestad, N. Gagliolo, V. V. Talanov, R. H. Yeh and


C. J. Ma, "High Resolution Mangetic Current Imaging


for Die Level Short Localization," 20th IEEE


International Symposium on the Physical and Failure


Analysis of Integrated Circuits (IPFA), p. 4, 2013.


[5]  D. Vallett, J. Gaudestad and C. Richardson, "HighResolution Backside GMR Magnetic Current imaging on


a Contour-Milled Globally Ultrathin Die," ASM


International, p. 5, 2014.


Isolating Electrically Open Laminate Defects Using Space Domain Reflectometry (SDR) with a Superconducting Quantum Interference Device (SQUID)


GLOBALFOUNDRIES, Essex Junction VT, USA  kevin.distelhurst@globalfoundries.com


An electrically open defect on a laminate may not always be  found timely or successfully due to the lack of fault isolation  techniques for this type of defect. This is partly due to needing  high frequency techniques to isolate the location of the open. Magnetic field imaging (MFI) using a Superconducting  Quantum Interference Device (SQUID) is a technique that  maps, in this case, an RF signal through a trace, up until the  open defect boundary. Several obstacles are introduced when  using an RF signal, one of which is the shielding of the signal  from the external world. Despite this obstacle, analysis of an  open in an arbitrary location along a laminate under a copper  plane is proven successful using this technique.


Several examples of electrically open defects that can be  found within a laminate include a break in a signal trace, via  or the laminate-die interface (e.g. wirebond). There is no  direct way to view these defects without destructive analysis  due to the opaque material that the traces are typically  embedded within. XRAY computed tomography (XRT) is one  method of indirectly observing the defect by taking series of  2D XRAY images and reconstructing them into a 3D render. XRAY 2D imaging may be sufficient in detecting catastrophic  opens and even some less obvious breaks in a signal trace or  via. However, without sufficient isolation, the XRAY imaging  technique may not provide timely results. Several iterations of  XRT may be needed throughout the laminate to analyze all  stretches of the electrically open trace. In some cases, the  defect may be too subtle to detect. Techniques have been  developed, such as Time Domain Reflectometry (TDR), to  help isolate the defect [1] but XRAY imaging may still be  needed to confirm or further isolate the defect before  destructive, more direct analysis is performed.


MFI has been successful in isolating shorts in both laminate


[2] and die [3]. Typically, an AC signal is applied to the  shorting defect and the resulting magnetic field generated  from the current path is observed using a SQUID or Giant  Magnetoresistance (GMR). The technique has been extended  to using an RF signal. The signal is applied to the defective  trace and the resulting standing wave magnetic field is mapped


up until the open boundary which reflects the incoming RF  signal. This technique is called space domain reflectometry (SDR). The resulting map of the magnetic field is used to  generate a current density map (CDM).  Further descriptions  of the setup are found in [1] & [4]. Destructive, direct analysis  of the defect can be performed after MFI provides the  approximate location of the fault, circumventing the need for  lengthy XRT and electrical isolation.


SDR has been successful [1], [4] in finding opens in the  laminate. This work extends the concept by including an open  along a signal trace within the laminate, buried under a single  copper plane. The buried defect is of interest because it is one  example of the obstacles encountered when dealing with RF  signals (e.g. shielding, coupling, ect.). Analysis of a buried  defect compared to an open without a copper power plane  above reveals the magnetic field strength at the SQUID sensor  is impacted by the planes.


Setup of Laminate


A non-defective laminate is used as the device under test. The  laminate consists of a ball grid array (BGA) followed by  several layers of copper traces and power planes up until the  laminate-die interface to the silicon flip chip. An arbitrary net  is chosen in two corners of the laminate opposite one another. Both nets start at a ball near the edge of the laminate on the  bottom (opposite the flipped die) and eventually transverse  most of the distance near the top (closest to die) of the  laminate. The top most portion of the laminate above the top  level trace has a power plane covering the nets. See


Figure 1 for a representation of the nets.


Experimental, Results & Discussion


In this case, a NSOP issue was reported during assembly and  some failed die-samples were sent for analysis. The main  purpose is to understand the failure mechanism and possible


## Introduction


root cause and whether the NSOP problem was due to wafer


## Email:Younan@wintech-nano.com


fabrication or assembly.


Figure 1. A NSOP case was reported during assembly. Optical inspection found discoloration and pinholes on the  Al bondpads, especially at the edge, which might have  caused the NSOP issue.


Failure analysis showed that galvanic corrosion resulted in  pinhole defects on the Al bondpads (Figure 1). From Figure


1, one can see discoloration and pinholes on the Al bondpads, especially at the edge. Moreover, comparing to the previous  cases studied [1-2], we found that the pinhole defects formed  were more serious.


FIB/TEM analysis was done on a pinhole at the bondpad  edge. The TEM results showed that the pinhole defect formed  in the Cu process was more serious (Figure 2) than it formed  in the Al process (previous case) (Figure 3).


Figure 2. TEM micrograph shows that the pinhole defect  formed in the Cu process (current case) was more serious. At the defect area, all Al had been corroded.


Figure 3. TEM micrograph shows that the pinhole defect  formed in the Al process (previous case). At the defect area, Al layer was partially corroded on the Al bondpad at the site  circled.


From Figure 2 (current case with the Cu process), one can see  that the Al at the pinhole had been fully corrosive and almost  no  Al  was  left. However, from Figure 3 (previous  case with


## Galvanic Corrosion


the  Al  process),  Al  at   the  pinhole  area   had   been   also   corrosive, but Al (about 50%) was still left.  Why the pinhole  defect formed in the Cu process (Figure 2) was more serious  comparing to that formed in the Al process (Figure 3)? We  conducted further investigation and studies in the following  section.


Studies of Failure Mechanism


Galvanic Corrosion


Galvanic corrosion is also known as two-metal corrosion. A  complete corrosion cell consists of an anode and a cathode in  which the less resistant metal becomes anodic and the more  resistant metal cathodic.  In the authors’ previous studies, a  failure mode of galvanic corrosion has been proposed [1-2], in which, Al is anodic & Cu is cathodic:


Anodic      Al  Al+3  + 3e     - 1.662 V      (1)


Cathodic   Cu +2 + 2e  Cu    + 0.337 V     (2)


If a bondpad is exposed to moisture, corrosion may occur. The anodic aluminum surrounding exposed cathodic Cu is  corroded to form hydrated aluminum hydroxide corrosion  product:


O2 + 2H2O + 4e  4 OH-            (3)


4Al + 3O2 + 6H2O  4Al+3 + 12OH-  4Al(OH)3↓  (4)


The hole apparently continues until the Al2Cu nucleus is  isolated electrically and physically from the aluminum  matrix. Therefore, there is a nucleus centered inside most  holes due to galvanic corrosion [1-2]. However, in this case, the Al2Cu nucleus had been washed away during the cleaning  process.


After studying, we understood that the root cause of galvanic  corrosion in the Al process is only one way that Al-Cu cell is  from Al alloy (Al + 0.5%Cu). However, in the Cu process (0.13um and below) it may be from two ways as Al-Cu cell  can be from both Al alloy (Al + 0.5% Cu) and underneath Cu  layer when the barrier metal Ta is with weak points (pinholes). As such, the pinhole defect formed might be more  serious in the Cu process.


One can further understand from the diagrams (Figure 4-5). This is because of only with one way Al-Cu cell galvanic  corrosion in the Al process (Figure 4), but with two ways of  Al-Cu cell galvanic corrosion in the Cu process (Figure 5). As such, the pinhole defect formed in the Cu process might  be more serious comparing to that in the Al process.


Identification of Root Cause


To identify the root cause and fully understand the failure  mechanism, cross sectional TEM was performed at the  bondpad edge (the no pinhole area).


Figure 4. Schematic cross section shows the pinhole defect  formed in the Al process: only one way (as shown as the  arrow) Al-Cu cell galvanic corrosion, which is from the Al  metal (Al alloy with 0.5% Cu).


Figure 5. Schematic cross section shows the pinhole formed  in the Cu process: two ways (shown with arrows) Al-Cu cell  galvanic corrosion, which are from both Al metal and  underneath Cu layer when the barrier metal Ta has a weakpoint.


TEM results showed that Cu diffused into the Al layer on the  bondpad and Al was also diffused into the Cu layer (Figure  6). The Cu-Al and Al-Cu materials formed could form some  new Al-Cu cells and contribute to galvanic corrosion. This  might have made galvanic corrosion more serious in the Cu  process.


It is well known that there is a barrier metal layer (Ta) between the Cu layer and the bondpad Al layer so as to  prevent Al and Cu diffusion to form the Al-Cu or Cu-Al   phases. However, in the current case, TEM result showed that


Al and Cu diffused into each other to form Cu-Al and Al-Cu  phases as shown by the arrows in Figure 6. Based on the  TEM results, we suspected that the barrier metal Ta had weak  points or pinholes.


Figure 6. TEM micrograph showed that Cu diffused to the  Al layer on the bondpad and Al was also diffused to the Cu  metal layer. These materials would form some new Al-Cu  cells and contribute to galvanic corrosion


To prove our suspicion, we did further TEM analysis. Based  on the TEM results, we found the barrier metal Ta layer with  weak point or pinhole, which is shown in Figure 7 at the area  circled. The close-up TEM result is shown in Figure 8.


From the TEM results (Figures 7-8), one can see that the Ta  barrier metal has a weak point/pinhole, which caused Cu to  diffuse into the Al layer on the bondpad and Al to diffuse into  the Cu metal layer.


Figure 7. Z contrast TEM micrograph showed that the  barrier metal Ta with weak point (pinhole) at the area  circled. One can also see Cu-Al phase due to diffusion.


Figure 8. Z contrast TEM micrograph showed the barrier  metal with a weak point (pinhole), which caused Cu  diffusion to the Al layer on the bondpad and Al was also  diffused to the Cu metal layer.


In this paper, the authors have further studied the failure  mechanism of galvanic corrosion (Al-Cu cell）on microchip  Al bondpads in the Cu process (0.13um and below) with Ta  barrier metal.


Based on our study, the root cause of galvanic corrosion in  the Al process (0.18un and above) is only one way that Al-Cu  cell is from Al alloy (Al + 0.5%Cu). However, in the Cu  process (0.13um and below) it may be from two ways that AlCu cell can be from both Al alloy (Al + 0.5%Cu) on the  bondpad and underneath Cu metal layer when the barrier  metal Ta is with weak points or pinholes. As such, the  pinhole defects on the bondpad caused by galvanic corrosion (Al-Cu cell) in the Cu process might be more serious than  that in the Al process. The failure mechanism in the Cu  process could be:


1) The barrier metal (Ta) has weak points or pinholes;


2) Al on bondpad diffused to the Cu metal layer and the Cu  in the Cu metal layer also diffused out to the Al bondpad; 3) Formed Cu-Al and Al-Cu compounds and more Al-Cu  cells;


4) Caused galvanic corrosion (Al-Cu cell);


5) Formed the worst pinhole defects on Al bpndpads;


6) Resulted in NSOP during assembly bonding process.


The authors would like to thank colleagues from WintechNano for their technical support and contributions to this  technical paper.


[1] Hua Younan, A Study on Discolored Bondpads & Galvanic Corrosion. ISTFA 1998, 15-19 Nov, Hyatt  Regency, DFW-East Tower, Dallas, Texas, USA, 269-272 (1998).


[2] Hua Younan et al, Failure Analysis and Elimination of  Galvanic Corrosion on Bondpads during Wafer Sawing. ISTFA 2000, 12-16 Nov, Meydenbauer Convention  Center, Bellevue (Seattle), Washington, USA, 369-372 (2000).


[3] Simon Thomas and Howard M. Berg, Micro-corrosion of  Al-Cu Bonding Pads, p153-158, IEEE/IRPS (1985)


Non-Destructive Contamination Detection in Thick and Extremely-Thin SOI  Wafers Using Optical Second Harmonic Generation


M.C. Kryger and J.P. Changala


FemtoMetrix, Inc., Santa Ana, California, US  info@femtometrix.com


M. L. Alles


Dept. of EECS, School of Engineering  Vanderbilt University


Nashville, Tennessee, USA


michael.alles@vanderbilt.edu


Non-destructive optical second harmonic generation (SHG) is  shown to be an effective method for detecting interfacial  surface and subsurface non-visual defects in commercial thick  and extremely-thin (ET) SOI wafers. A method is demonstrated  for removing contributions (noise) from layer thickness  variations observed in thick SOI, increasing the sensitivity and  enabling detection of trace surface metal contamination. Subsurface contamination, otherwise missed by the standard flow  of non-destructive characterization methods, is shown to be  detected by SHG.


Introduction and Background


Optical Second Harmonic Generation (SHG) is a  nondestructive, contactless technique for characterizing  surfaces, interfaces, thin-films and bulk properties of materials. SHG originates from areas where symmetry in the material is  broken, such as surfaces, interfaces, crystal defects, and the  bulk of non-centrosymmetric materials.  This allows SHG to be  highly interface specific in centrosymmetric materials like  silicon and Silicon-on-Insulator (SOI), and effectively probe  the bulk of materials such as Ge and III-V.  Novel layered  materials necessary to continue meeting the exacting  performance needs of device fabricators, such as SOI, are  excellent candidates for characterization with SHG [1-5].


SOI, because of its wide range of potential applications and  benefits, is available in many thickness configurations. The  basic structure of SOI consists of a silicon film on a buried  oxide layer, supported by a silicon substrate.   Figure 1  demonstrates a sampling of the various thicknesses and related  applications [6].


Thick SOI has long been used for high voltage, power, and RF  devices, requiring electrical isolation, and increasingly in Micro  Electro Mechanical Systems (MEMS), where the BOX layer  serves as an etch stop for creating 3D MEMS structures. Layer  thicknesses in these applications are on the order of  micrometers [6].


Figure 1: An example of the varieties of SOI types and  applications from SunEdison Semi, a major manufacturer of  SOI wafers, PerfectSOI = thin and PowerSOI = thick.


Thin film SOI, such as FD-SOI (Fully Depleted Silicon-onInsulator) and PerfectSOI, are a high potential substrate that  provides solutions for the scaling, leakage, and variability  issues inherent in advanced CMOS technology. These wafers  consist of a top silicon layer of ~8-25nm, on a buried oxide (BOX) layer, supported by the bulk silicon substrate. Thin SOI  fabrication processes have significant advantages over bulk  processes such as fewer processing steps, no need for pocket  implants and easier STI formation [1]. ST Microelectronics has  commercialized a 28 nm FDSOI CMOS process that has been  licensed to Samsung [7], and GLOBALFOUNDRIES have  recently announced a 22 nm FDSOI technology having a 14 nm  FEOL and 28 nm BEOL [8]. The latter is targeted specifically  for more cost-sensitive applications desiring a performance  gain of scaling below 28 nm CMOS, while achieving a lower  cost point than 14 nm bulk FinFETS.


A significant plurality of reliability, yield, and variability  concerns in SOI are due to charge traps and associated defects


at the Device/BOX and BOX/Bulk interfaces [2,3]. Charge  traps in the near-interfacial regions of the BOX layer in FD-SOI  substrates (Dit) can lead to significant bias temperature  instabilities, especially in fully-depleted transistors [2,4]. Hot  carrier stress due to trapping at the back gate is also known to  have detrimental impact on FD-SOI transistor reliability [5]. Other key yield concerns such as 1/f - or "flicker" - noise are  additionally attributable to Dit complications [9]. One source of  excessive charge traps is buried trace metal contamination [10]. The effect of metal contamination may also be compounded  during production by the failure of traditional metal gettering  techniques in FD-SOI [11]. In addition, normal methods of  monitoring metal contamination in bulk silicon are not effective  for FD-SOI [12], resulting in defective wafers being processed  as seen in Figure 2 below.


Figure 2: Wafer fabrication path


Cu is considered more dangerous than iron due to its diffusive  properties, and when located on the backside of an SOI wafer  can easily penetrate into the BOX during standard processing. Once Cu is introduced into the buried interfaces of an SOI wafer  it will diffuse throughout the wafer [13].


The extremely thin layers employed by FDSOI introduce new  metrology challenges requiring characterization of the  electrical parameters of BOX interfaces where conventional  techniques have limitations [14]. Figure 3 summarizes in-line  and subsurface capabilities of relevant characterization tools.


Figure 3: Utility comparison of available metrology  techniques.


As shown, alternative techniques fail to provide a highthroughput in-line solution for subsurface electrical  characterization. Group 1 and 2 techniques (ICP-MS, SIMS, GD-OES, Ψ-MOS and DLTS) are able to characterize limited  aspects of the subsurface of FD-SOI substrates, but fail to


provide the comprehensive non-destructive ability necessary  for in-line production. Group 3 techniques are non-destructive  but lack needed utility for FD-SOI due to limited throughput  and depth profiling capacities [15].


The destructive nature of Ψ-MOS prevents its use for nondestructive, in-line inspection [16]. ST Microelectronics has  expressed that Ψ-MOS loses accuracy for ultra-thin SOI [17] and Soitec has stated that Ψ-MOS cannot effectively  characterize the bulk/BOX interface [14].


The FemtoMetrix Harmonic F1x® Wafer Inspection System  utilizes optical Second Harmonic Generation (SHG) to provide  in-line electrical characterization of the surface and BOX  interfaces. SHG is a non-destructive, contactless technique for  characterizing surfaces, interfaces, thin-films and bulk  properties of materials. SHG is the only in-line method able to  comprehensively characterize the quality of BOX interfaces in  FD-SOI substrates, due to its high throughput and high  sensitivity to disturbances in the electric field at the interfaces  of multilayered materials [18,19]. As an industrial tool, SHG  offers distinct yield and net cost advantages to manufacturers.  SHG was first proposed as a versatile tool for SOI material  characterization in the 1990's [20]. Work since then has  uncovered a wide range of applications, including the probing  of Si/SiO2 interface roughness [21], and most recently the  detection of trace metal contamination at both BOX/Substrate


[22] and Device/BOX [23] interfaces. Advanced development  has demonstrated the utility of SHG as "optical Ψ-MOS" that is  rapid, non-destructive, and sensitive to concerns at both BOX  interfaces [24]. SHG is uniquely capable of identifying trapped  charges and other deleterious concerns at the Device/BOX  interface in a cost-effective and high-throughput manner.


Samples, Preparation, and Measurements


Eight SOI wafers, comprising two sets of four, were provided  by a leading semiconductor industry firm for the evaluation of  the Harmonic F1x.  Each set of four contained a distinct type of  SOI, thick (1500/1000 nm) and thin (12/25 nm.)


The four thick film 200 mm SOI wafers, 1500 nm top silicon  on 1000 nm buried oxide, were intentionally contaminated with  copper to study the sensitivity of SHG to surface contamination. All four of the wafers were measured nondestructively (SHG, Spectroscopic Reflectometry) and destructively (VPDICPMS). One wafer was held as a control, and not intentionally  contaminated.  The remaining three were spincoat with Cu in  doses on the orders of 1010, 1011, and 1012 at/cm2.  Contamination was verified by VPD-ICPMS, the results of  which are shown below in Table 1.


Table 1: 1500/1000 nm SOI wafer contamination levels, verified via VPD-ICPMS.


Wafer 1 (Control)


Wafer 2 (1010 Cu)


Wafer 3 (1011 Cu)


Wafer 4 (1012 Cu)


VPD


Measured  Cu


Measured Cu


(no


treatment)


1.7x1010  at/cm2


1.4x1011  at/cm2


1.6x1012


at/cm2


The four thin film 300 mm SOI wafers, consisting of a 12 nm  silicon film on 25 nm of BOX, were measured via SHG as  delivered to inspect for non-visual defects that influence yield. Of the four thin wafers there were two pairs of two, each having  a distinct manufacturing process. These wafers were measured  non-destructively (SHG, Spectroscopic Ellipsometry, Surfscan), and destructively (VPD-ICPMS, LA-ICPMS). The  four wafers were characterized using optical Second Harmonic  Generation (SHG) alongside complementary optical nondestructive characterization techniques.  Two paired wafers (one from each process technology lot) were also tested with  VPD-ICPMS.


SHG Measurement Methodology


SHG measurements were carried out on the samples described  above by irradiating the samples at 45° incident angle with ppolarized ~85 fs optical pulses (350 mW average power, 50  MHz repetition rate, wavelength λ = 780 nm) from a mode  locked ultrashort pulse laser focused to a w0 ≈ 50 µm radius  spot on the surface of the sample. A dichroic long wave pass  filter was placed in the incident beam to remove parasitic  second harmonic generation from elements along the path. The  p-polarized SH signal was spectrally filtered from the reflected  fundamental beam and measured with an integrated  photomultiplier element and photon counter as a function of  time to collect the SHG signal. The SHG data from the  measured points was then used to create wafer maps as a  function of discrete X-Y coordinates, displaying specific  parameters of the signal. The thick film wafers were mapped  using 643 spatial points, while the thin film wafers were  mapped using 1095 spatial points. For both wafer sets, these  points were arranged in a rectilinear grid across the surface of  the wafer.


For the thick film wafers, additional data and processing was  needed to separate material optical properties contributions to  the SHG and increase sensitivity to electrically active impurity  related defect. A breakdown of these SHG signal contributions  is shown in Figure 4.


Layer thickness variations in the top silicon film were found to  introduce a baseline signal that limited the sensitivity on the  thick SOI wafers. We developed an approach to remove this  signal and improve the sensitivity to the electrically active  defect (contamination) contributions to the SHG signal. To  remove the thin film interference effects, a phenomenological  model was constructed to describe the desired SHG parameter  as a function of top silicon film thickness for the ‘clean’, uncontaminated control wafer. This model was applied to  normalize the SHG response for variations in layer thickness  for the whole set of wafers. With the film thickness variation  effects removed from the SHG signal, the remaining variations  in SHG response are be primarily due to electrically-relevant  parameters such as metal contamination. This process is  summarized in Figure 5.


Figure 5: Parsing layer thickness from SHG data to enhance  electrical defect maps.


1500/1000 nm SOI: Initial SHG Results


Initial results from the three intentionally contaminated samples  did not indicate a stark contrast versus control as expected.  Within wafer variation was high, and there was not an obvious  relationship between Cu dose and SHG response.  Figure 6  below shows the initial (raw data) SHG response maps from the  four wafers.


Figure 4: Contributions to SHG signal.


TEM analysis was performed directly focused on the  suspected resistive VIA and contact and abnormal VIA2 was  found. There was abnormal Oxygen element at the interface of  Ti and W on VIA2. It can cause the resistive VIA and suffered  conductive issue at cold temperature (Fig.5). This kind of VIA  defect explains the cold temperature failure well.


Experiments and Results (Case2)


One 0.25m mixed signal IC which provide Local  Interconnect Network (LIN) communication failed on 3.5V  enable function. The signal on Lx pin is unable to recover the  sample from sleep mode at cold temperature (-10°C). The  failure didn’t appear at room temperature and high temperature.  It was also a failure that happened at cold temperature (Table 1). After decapsulation from the front side, the wakeup issue was  confirmed to exist.


Abnormal emitted  spots


X200


Figure 2: EMMI result at RT (Room Temperature) 25°C


and CT (Cold Temperature) 0°C on failed sample.


EDX line scan


O element


Interface


area


Figure 5: STEM image revealed abnormal VIA defect on  VIA2 and EDX line scan detected abnormal O element on  the interface area of VIA2.


VIA defect


Via2


Via1


Contact  Metal2


Metal1


Poly


Metal3


CLK_L7 signal  CLK_L6 signal


Emitted spots


U1274_L7_I8 cell


U1274_L7_I7 cell


D flip  flops


Figure 4: Schematic of the abnormal emitted spots and the  control logic.


Figure 3: Abnormal emitted spots and its corresponding  layout location.


X1000


emitted spots


CLK_L7 signal


Abnormal VIA


location


Table 1: Lx signal can’t wake up the IC from sleep mode on  failed sample.


VSUP=9V


Reference:


Failed IC:


Lx (wake up  voltage at -10°C)


3.5V


Can’t wake up


even Lx rising to


5V


EMMI was performed firstly at room temperature with no  failure condition, no abnormal emitted spot was found when  compared with reference. EMMI was performed again at cold  temperature (-10°C) and abnormal missing emitted spots were  detected on failed sample (Fig.6). The emissions at these  locations are normal at room temperature and may be directly  related to the cold temperature failure. Since this kind of cold  temperature failure was seldom caused by short or resistance  leakage which was hard defect-induced, the EMMI result was a  precious guidance to the root cause.


Layout and schematic was studied based on the abnormal  missing emitted spots at cold temperature. It was found that they  were located on two series Zener diodes (DZ5 and DZ4) which  are involved in wake up module. A defect in this module can  explain the wakeup issue well. When performing EMMI  analysis, the Zener diode would emitted normally if there was  higher voltage between the N node (the signal was VB1) and P  node. The missing emitted spots on two diodes at cold  temperature imply that voltage between N node and P node of  diode is not high enough. If the VB1 signal was low voltage or  0V, the two diodes would not emit. As short or resistance  leakage between VB1 and GND can not possibly happen due to  the cold temperature failure characteristic, conductive issue was  highly suspected. Schematic analysis indicated that the VB1  signal was a divided voltage from VSUP through some resistors. Since the VSUP signal was provided by external power supply  directly, it meant that the VB1 signal was failed after VSUP  through some resistors.


As there were many VIAs on the VSUP signal metal line to  VB1 signal, it was difficult to determine which VIA was the  prime suspect. A further measurement is required. Based on the  EMMI analysis result, necessary in-depth failure isolation  method to measure the IV curve between VB1 and VSUP is  required to double confirm that the wire line conduct failure is  caused by resistance VIA. An open failure was finally  confirmed between VSUP and VB1 on failed sample at cold  temperature (Fig.7). Optical Beam Induced Resistance Change


(OBIRCH) was used to locate the abnormal VIA precisely. Fortunately, the problematic VIA2 was successfully found by  OBIRCH (Fig.8). It was located on the VSUP wire line between  metal 3 and metal 2.


TEM was performed directly on the isolated VIA and  abnormal oxide layer was found at the bottom of VIA2. This  leads to the conductive issue at cold temperature (Fig.9).


Figure9: TEM image on the abnormal VIA revealed


abnormal interface on the bottom of VIA2.


Figure 8: Abnormal resistance change spot was captured


on VIA2 of VSUP wire line and its layout location.


X1000  Abnormal resistance


change spot on VIA


VS1 metal 3


VSUP


Failed: open Ref: 3.1Mohm


VB1


Missing emitted spots on  DZ5 and DZ4


Abnormal VIA2 location


3.1Mohm


Lx Control  module


Figure 7: Abnormal open between VSUP and VB1 on failed  IC and resistive VIA location in schematic control module.


Figure 6: EMMI result at RT (Room Temperature) 25°C  and CT (Cold Temperature) -10°C on failed sample.


Abnormal missing


Abnormal interface on VIA2


Abnormal VIA2  VS1 metal 2


EMMI is demonstrated to be effective to distinguish abnormal  emission spots by comparing between room and cold  temperature conditions. Applying past experience on  interpreting the shape of abnormal emission spots, fundamental  of EMMI and combing detail schematic and layout analysis, resistive VIA defects causing cold temperature failures on ICs  can be revealed. Analysis cycle time is saved on micro-probing. Furthermore, the success rate of this approach is high to debug  cold temperature functional fail cases.


Thanks Jinglong Li for his cold temperature equipment to  duplicate the cold temperature failure. Also thanks my  electronic failure analysis team and physical failure analysis  team for their great help on case analysis.


[1] Edward I. Cole Jr., Paiboon Tangyunyong, “Resistive    Interconnection Localization”, ISTFA 2001, 15-21.


[2] Jinglong Li, Chunlei Wu, “Soft Defect Localization(SDL) Applied on Analog and Mixed-mode ICs Failure Analysis”, IRPS2012, FA.6.1-FA.6.5.


[3] Christian Burmer, Christof Brillert, Zhongling Qian, “Soft  Defects: Challenge and Chance for Failure Analysis”, IPFA  2007, 235-239.


[4] Christian Burmer, Christof Brillert, Zhongling Qian, “Soft  Defects: Challenge and Chance for Failure Analysis”, IPFA


2007, 235-239.


[5] Xuanlong Chen; Xianjun Kuang; Guangning Xu,


“Application of EMMI contrast method in failure analysis”


IPFA2013, 504-507.


A Combination Continuous Wave and Pulse Laser Assisted Chemical Etching  Processes through Encapsulated IC Packaging


Matthew M. Mulholland,


Intel Corporation, Santa Clara, CA 95054 USA


matthew.m.mulholland@intel.com, Tel: 408-765-7870


Scott Silverman


VarioScale Inc. 1782 La Costa Meadows Dr. #103, San Marcos, CA 92078 USA  agman@varioscale.com, Tel: 760-402-2640


Post silicon validation techniques specifically Focused Ion  Beam (FIB) circuit editing and Failure Analysis (FA) require  backside sample preparation on Integrated Circuits (IC). Although these preparation techniques are typically done  globally across the encapsulated and silicon packaging  materials, in some scenarios with tight boundary conditions, only a local approach can be attempted for the analysis.  This  local approach to access the underlying features, such as  circuits, solder bumps, and electrical traces will typically use  conventional Laser Chemical Etching (LCE) platforms.  The  focus of this analysis will be to investigate and conjoin  previously published techniques to this local preparation by  using a combination of laser sources.   A Continuous Wave (CW) and Pulse laser will be used at various processing stages  to de-process IC packaging materials silicon and mold  compound encapsulation.


Post silicon validation techniques specifically Focused Ion  Beam (FIB) circuit editing require backside sample preparation  done by local silicon machining to access the active circuits. Conventional methods such as Laser Chemical Etching (LCE) platforms are commonly used.  This paper will investigate and  conjoin previously published techniques to this local silicon  preparation by using a combination of laser sources to deprocess IC packaging materials including silicon and mold  compound encapsulation.  These techniques work by using both  a Continuous Wave (CW) and Pulse laser depending on the  material to be removed.  Although the CW laser processing of  silicon is well understood, some parameters such as optical  objective, laser power, scan speed, and line spacing were  modulated to recover rough surfaces produced from ablation. Most of the work here revolves around pulse laser ablation of  mold compound and silicon.  An overview of the encapsulated


IC package materials stack-up and localized prep region is  shown below (Fig. 1).


Figure 1: Cross section of trenching concept showing localized  prep region through encapsulated mold compound and silicon.


There have been previous studies of pulse laser ablation of  different materials and laser sources [1].  These comprehensive  studies took a mechanistic approach to understanding the pulse  laser wavelength and width parameters against the material  removal performance.  It has also been studied that the laser  parameters used in this ablation process are important in  keeping the integrity of the device [2].


This paper will build upon these previous studies, but will  introduce a comprehensive local machining approach and  solution through different materials split into four main areas. The first will target Mold Compound Pulse Laser Ablation (MCPLA) and discuss the mold compound removal rate and  silicon layer endpoint detection.  The second will discuss and  use previous developed techniques of Chemical Assisted Pulse  Laser Ablation (CAPLA) [3] and ways to recover the surface  quality for further FIB and FA applications.  The third will  briefly outline some well-known continuous wave laser  chemical etching (CWLCE) parameters.  Finally, the fourth  area will discuss previously developed extreme thin silicon  membranes by Pulse Laser Assisted Chemical Etch (PLACE) [4, 5, 6].  These combined processing techniques provide a  comprehensive local preparation solution for device failure


analysis.  The labelled x-section of the trenching concept and  material stack is shown (Fig. 2).


Figure 2: Cross section of trenching concept showing laser  processing and material layer stack-up


Experimental Set-up


For the experimental set-up, an existing Laser Etching  VarioEditTM platform was used that has both a 532nm  wavelength CW and Pulse lasers integrated.  The CW laser  parameters such as input power (W), raster scan speed (um/sec), and line spacing (um) can be modulated to achieve selected etch  rates.  The Pulse laser parameters of energy per pulse (uJ), repetition rate (kHz), scan speed (um/sec), and line spacing (um) can also be modulated to achieve different etch rates.  The  Pulse laser input current (Amp) was fixed based on the  calibrated laser source.


The encapsulated IC sample used in this study consisted of a  stack-up of 100um thickness mold compound and 250um  silicon thickness for a total of 350um of material available for  removal as shown in figure 2.  The starting local machining  trench size was 1mm2 (1x1mm) in area and tapers to a final


0.09mm2 (300x300um) floor above the circuits.


For the first processing phase, mold compound pulse laser  ablation (MCPLA) was tested.  The starting surface optical  image and laser processing GUI screen shots are shown in  figure 3.  The interaction mechanism used here was not  chemically dependent, but rather relied solely on the laser to  material interaction.  The sample was placed in the work  chamber under 100mT operating pressure with continuous  vacuum flow.  This continuous flow helps to control material  contamination and collection by pumping particles out of the  chamber.  The energy per pulse was modulated for resulting  etch rates as shown in figure 7.  The repetition rate (50 kHz), scan speed (60,000 um/sec), input current (17 amp), and 1um  line spacing was kept constant.  Typically, a high energy per  pulse is used with subsequent lower energies as the mold  compound to silicon transition is approached and the final  resulting surface becomes visible.  The end point mechanism  can be detected in two ways: first, through depth of focus with  a known material thickness and second, optical inspection, as  silicon will visually have a brighter contrasting appearance.  The processing time through 100um of mold compound  thickness can be done in just a few minutes for a 1x1mm size  trench and stepping down energy per pulse per scan pass.  The


etch rate curve fit for MCPLA is shown in figure 7.  The energy  per pulse multiplied by the constant repetition rate used here  will result in average power applied to the sample.  This chart  shows a logarithmic scale of 1um up to 80um depth of material  removal is possible for mold compound material.


Figure 3: Mold compound ablation (MCPLA) GUI processing  images for subsequent pulse energies (uJ) and silicon layer  endpoint


For the second processing phase, once the mold compound  layer is completely removed and silicon layer has been exposed, chemical assisted pulse laser ablation (CAPLA) is used to etch  at a very high rate.  This enables large volumes of material to  be removed to save processing time as the silicon thickness in  this case is fairly thick at 250um.  The downside to this  technique is a resulting rough silicon surface that will ultimately  need to be recovered in subsequent processing steps which will  be discussed later.  Here 400T pressure of chlorine is used with  energy per pulse modulated for resulting etch rates again shown  in figure 7.   The depth per pass possible in this case ranged  from 4um up to 10um.  The repetition rate (50 kHz), scan speed (60,000um/sec), input current (17 Amp), and 1um line spacing  was kept constant.  Again, typically a high energy per pulse is  used with subsequent lower energies as silicon thickness  decreases.  The end point mechanism used in this case relied  solely on the depth of focus with a known material thickness.  An end point target of 100um remaining silicon thickness was  used in order to have enough remaining material to etch and  recover the rough surface using the CW laser, as shown in  figure 4.


Figure 4: Silicon ablation (CAPLA) GUI processing images for  subsequent pulse energy (uJ), remaining silicon thickness (um), and silicon end point


The third processing phase focused on typical CW laser  chemical etching to recover the previous rough surface  produced from the ablation phase.  In this phase, 400T pressure  of chlorine with high CW power of 6 watts is used with typical  scan speed of 20,000 um/s and 1um line spacing parameters.  In  comparison, CW will have much higher average power applied  to the sample as opposed to pulse mode shown in figure 7. Figure 5 shows the process photos and typical surface qualities  produced during this step.  The silicon will be etched from  100um remaining to a target of 10um above the active circuit  layer.  Over this processing phase, the trench floor size will  typically be decreased and scan direction alternated.  Visually, the trench floor roughness will appear smoother and acceptable  for further FIB and FA processing.


Figure 5: Silicon etching (CWLCE) GUI processing images for  subsequent continuous wave power (W), remaining silicon  thickness (um), and silicon end point target 10um


The final phase will switch back to the pulse laser assisted  chemical etching (PLACE) processing mode and modulate to  very low energies per pulse to achieve just a few hundred  nanometers per pass etch rates.  It will be these low energies or  average power that allows silicon etching to an extreme  remaining silicon thickness of 2um without exposing the circuit  layer below (Fig. 6).  By using this process for bulk silicon  removal, significant FIB processing time will be saved by  allowing closer access to the circuits.


Figure 6: Silicon ablation (PLACE) GUI images for starting  surface 10um to final target surface 2um remaining silicon  thickness (um)


These four processing phases and resulting etch rates as a  function of power (mW) were plotted together on the  logarithmic scale to show the versatility of etch rates available  between these two laser sources, process chemistry, and  working material stacks.


Figure 7: Logarithmic scale chart displaying etch rates versus  power for processing phases 1) MCPLA, 2) CAPLA, 3) CWLCE, and 4) PLACE


In summary, a versatile laser assisted etching platform with  both a CW and Pulse mode operations can handle the multilayer stack-up of materials and thicknesses.  The evolution of  these process steps are shown with the final optical image in  figure 8.


Figure 8: An optical image of the evolution of the process steps  through mold compound and silicon.


The pulse laser mode without chemical assisted etching works  well for mold compound ablation.  The pulse laser can also be  used with chemical assist chlorine and produce a wide range of  etch rates depending on energies used.  A very high energy of  8uJ can etch 20um/pass in an ablation state whereas a much  lower 0.5uJ can etch 0.5um/pass under the ablation threshold to  achieve a 2um trench remaining silicon thickness.  The standard  CW laser mode can act as a bridge between the high and low  pulse mode energy processes.  This laser and process versatility  allows one platform to de-process multiple materials enabling a  localized area to be exposed for further Circuit Edit (FIB) or  Failure Analysis (FA) applications.


[1] Stefan Martens, Walter Mack, Frederic Courtade, Philippe  Perdu, Juergen Wilde, Friedemann Voelklein, “Laser-Based  Target Preparation in 3D Integrated Electronic Packages” Journal of Electronic Packaging Vol. 131 Pg. 031006-1 (2009)


[2] Yeoh Lai Seng, Yeoh Joon Chai, Chong Kok Cheng, Susan  Li, “Case Studies of Laser Ablation Effects on Flash Memory  Devices”


[3] Robert Chivas, Scott Silverman, Niru Dandekar, “LaserAssisted Chemical Polishing of Silicon (112) Wafers” Journal  of Electronic Materials, Vol. 41 Pg. 2790 (2012)


[4] M. H. Hong, Z. H. Mai, G. X. Chen, T. Thiam, W.D. Song, Y. F Lu, C. E. Soh, T. C. Chong, “Pulsed Laser Ablation of IC  Packages for the Device Failure Analyses” Proceedings from  SPIE Vol. 4637 Pg. 445 (2002)


[5] Robert Chivas, Scott Silverman, Niru Dandekar, “Pulsed  Laser Assisted Chemical Etch for Analytic Surface  Preparations” Proceedings from Reliability Physics  Symposium (IRPS) Pg. 2D.6.1 (2012)


[6] Robert Chivas, Scott Silverman, Niru Dandekar, “Preparation of Wafer Level Packaged Integrated Circuits using  Pulse Laser Assisted Chemical Etching” Proceedings from  International Symposium for Testing and Failure Analysis (ISTFA) Pg. 491 (2012)


Failure Mechanism Studies and Elimination of Galvanic Corrosion  (Al-Cu Cell）on Microchip Aluminum Bondpads in Copper Process


## Hua Younan, Chen Yixin, Fu Chao and Li Xiaomin


Hua Younan, Chen Yixin, Fu Chao and Li Xiaomin


10 Science Park Road, #03-26 & #03-28, The Alpha Building  Singapore Science Park II, Singapore 117684


Email:Younan@wintech-nano.com


In the authors’ previous papers, the failure mechanism and  elimination solutions of galvanic corrosion （Al-Cu cell） on  microchip Al bondpads in the Al process (0.18un and above) have been studied [1-2]. In this paper, the authors will further  study the failure mechanism and root cause of galvanic  corrosion (Al-Cu cell) on microchip Al bondpads in the Cu  process (0.13um and below) with Ta barrier metal. Based on  our results, the root cause of galvanic corrosion (Al-Cu cell) in the Al process is only one way and Al-Cu cell is  from Al  alloy (Al + 0.5%Cu) on Al bondpads. However, in the Cu  process it may be from two ways and Al-Cu cell can be from  both Al alloy (Al + 0.5%Cu) on Al bondpads and the Cu  metal layer below the barrier metal Ta when Ta has weak  points or pinhole. As such, the pinhole defects on Al bondpad  caused by galvanic corrosion (Al-Cu cell) in the Cu process  might be more serious than that in the Al process. In this  paper, TEM is used for root cause identification. Based on the  TEM results, galvanic corrosion was due to the weak point/ pinhole at the Ta barrier metal layer and Al-Cu diffusion.


In wafer fabrication for metallization materials of bondpads, copper is added to Al or Al-Si to enhance the  electromigration performance of the conductor, and the  control grain size of the metal film on the bondpads. However, the addition of Cu to Al metallization is not without  drawbacks. The increased susceptibility of Al-Cu thin film to  corrosion is generally recognized [3]. In this paper, the  authors will further study the failure mechanism and the root  cause of galvanic corrosion on microchip Al bondpads in the  Cu process (0.13um and below) with Ta barrier metal.

