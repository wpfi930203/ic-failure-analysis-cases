---
title: "256_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_158daec435c2c4dbd9cb88e8bd2247f07295230462135641
file_size: 437963
---

## Characterization of 1122nm Laser for Laser Based  Fault Isolation Applications  

Vasanth Somasundaram 1 , Seah Yi Xuan 1 , Angeline Phoa 1 , Winson Lua 1 , Chua Choon Meng 2

Venkat Krishnan Ravikumar 1,3

1. Device Analysis, AMD Singapore;

2. Semicaps Pte Ltd

3. Singapore University of Technology and Design, Singapore


Correspondence email: vasanth.somasundaram@amd.com

Abstract-   As the technology node shrinks, the choice of laser  for performing fault isolation becomes critical. The  conventionally used 1319nm laser has spatial resolution  constraint at smaller geometries. The 1064nm laser provides  resolution improvement at the cost of reduced signal strength  especially for thicker or heavily doped substrates. This paper  explores the possibilities of using a low noise 1122nm laser in  Electrical Fault isolation analyses.

## I. I NTRODUCTION 

Electrical Fault Isolation (EFI) is an initial step in failure  analysis. Conventional EFI techniques include Photon Emission  microscopy (PEM), Soft Defect Localization (SDL), Frequency  Mapping (FM), and Laser Probing (LP) [1].

When the device under test (DUT) is constantly exercised, it can  affect optical properties like absorption coefficient and refractive  index change, causing amplitude and phase modulation of the  reflected laser. FM and LP require lasers reflected off transistors  to be monitored continuously when the DUT is being exercised.  The reflected laser is demodulated with the help of the spectrum  analyzer to map the transistor switching frequency whereas an  oscilloscope is used to obtain transistor switching information.

FM is an excellent technique to debug functional chain failures  [2]. A break in the chain can be identified by FM and further  fault isolation can be performed. LP, as a complimentary  technique, is useful for logic analysis and timing violations  debug.

SDL is a fault isolation technique where the DUT is stimulated  by laser while it is operated at pass-fail boundary. This technique  is used when the devices fail intermittently, the device is  generally sensitive to voltage, frequency, and temperature of the  test [3].

## II.   P ROBLEM STATEMENT 

Two conventionally used laser wavelengths in the industry for  fault isolation for sub 20nm FinFET devices are   $1319\mathrm{nm}$  and   $1064\mathrm{nm}$  . In accordance with the Rayleigh’s criteria, the  resolving power of a microscope improves with shorter  wavelength, which means the 1064nm resolve better than the   $1319\mathrm{nm}$  . This makes 1064nm more suitable for advanced nodes  [4].  However, 1064nm photons possess higher energy than the  silicon bandgap and can introduce electron-hole pairs into the  devices being probed. This results in alterations of laser probing  waveforms, affecting signal interpretation. As a further  challenge, the laser is absorbed a lot more in silicon, thereby  reducing the signal strength for a given laser power. This  problem is exacerbated when aplanatic silicon solid immersion  lenses are used. To overcome these losses, a laser with higher  resolving power than a 1319nm laser but with a photon energy  near to, but not exceeding the Si bandgap is desired.

## III. E XPERIMENTAL SETUP 

In this work, we introduce a low noise 1122nm laser as a  potential alternative to   $1064\mathrm{nm}$   and 1319nm lasers for dynamic  fault isolation applications. This paper draws a comparison in FI  results between a   $1319\mathrm{nm}$  , 1064nm and   $1122\mathrm{nm}$   low noise  lasers. Previous work using 1122nm lasers were limited to SDL  applications [5] as the laser was not low noise.

FM and LP were performed on sub-20nm FinFET devices using  both the lasers (1319nm and   $1122\mathrm{nm})$   under identical test  conditions. The LP detector used was a 1GHz, low noise  detector, and instead of an oscilloscope, a digitizer was used to  collect the waveform. This setup limited our scope to qualitative  comparisons, and we were unable to assess effect of laser on  rising edges of laser waveforms.

Key parameters such as Signal to Noise ratio, Peak signal  strength, Normalized Signal Strength and the Frequency  mapping images were recorded for the lasers. To quantify  resolution, simulations were conducted and compared with  frequency map results.

SDL Analyses were performed on the same device using  1064nm, 1122nm, and 1319nm lasers.

## IV. R ESULTS AND DISCUSSION 

Frequency Mapping : Frequency mapping was performed on  different circuits using both lasers and the images are shown  below.

![1 um 1 umm     1 um unn             1122nm @ 8.2mW  1122nm @ 8.2mW                          1319nm @ 1.84mW  1319nm @ 1.84mW  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d86a950b-caa3-4734-a36e-a4337d17c891/d86a950b-caa3-4734-a36e-a4337d17c891.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=fbe57f9a86af22fbbcd4551c9e53482439bbe962)
Figure 1 – FM on circuit 1 at 50MHz .

From Figure 1, it is observed that the resolution of both the  lasers, 1122nm on the left and 1319nm on the right is similar for  a buffer circuitry.

To understand the resolution differences, FM was performed on  a 3-stage inverter circuitry on a sub 20nm FinFET device and the  layout of the circuitry is shown in Figure 2. Figure 3 and Figure  4 show the FM images on   $1319\mathrm{nm}$   and   $1122\mathrm{nm} $  lasers  respectively.

![一 200nm ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7832c887-6444-47c4-89cc-96c2c4f1d0e0/7832c887-6444-47c4-89cc-96c2c4f1d0e0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=a18a36192feeba8d90a426fbbba9a3b682297239)
Figure 2 – Layout of a 3 stage Inverter.

The Gaussian Full Width to Half Maximum [FWHM] was used  to determine the resolution under both the lasers, the calculations  of the resolution were based on [6].

$$\mathrm{FWHM}=0.87\,\lambda\,/\,\mathrm{NA}$$
Where   $\uplambda$   is the wavelength of the laser, NA is the numerical  aperture of the Solid Immersion Lens. NA of the Solid  immersion lens was 3.3. Hence the FWHM for 1319nm laser is  approximately 348nm and FWHM for 1122nm is 296nm

Laser’s Interaction with device was simulated, the laser probe  was modelled using the electro-optic model discussed   in [6],  Figure 3 shows a comparison between simulated FM image and  the actual FM image on  $1319\mathrm{nm}$   laser

![100 nm  100 nm                     Actual FM                                 Simulated FM  ActualFM   SimulatedFM  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c2ee75e0-3cf0-4622-bb5b-2d597e4da8be/c2ee75e0-3cf0-4622-bb5b-2d597e4da8be.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=38309b3f8305e0168f5a37151dd0efc31932c94b)
Figure 3 – 1319nm, Actual FM versus Simulated FM.

Figure 4 shows a comparison between simulated FM image and  the actual FM image on   $1122\mathrm{nm}$  laser.

![100 nm  100 nm                  Actual FM                            Simulated FM  Actual FM   Simulated FM  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/29238235-d59a-4c79-ac5b-7f7f98bfb569/29238235-d59a-4c79-ac5b-7f7f98bfb569.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=a6cb6f12503e2e106d1b504279f25cc7b251bea5)
Figure 4 – 1122nm, Actual FM versus Simulated FM.

The 2p transistor is visible on   $1122\mathrm{nm}$  whereas it is not visible  on   $1319\mathrm{nm}$   laser.

The simulated FM images closely resemble the actual images  and thus based on the FWHM calculation for this experimental  setup,   $1122\mathrm{nm}$   laser offers close to   $50\mathrm{nm}$  reduction in spot size  and therefore in resolution as well.

Laser Probing:  Laser Probing was performed while exercising  the device by a tester at 50MHz frequency.

![1122nm  1122nm       1319nm  1319nm  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/60fabb8f-c41e-4682-b436-04a7828770b9/60fabb8f-c41e-4682-b436-04a7828770b9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=d4acab4a4296753e43f9688e09d8cb2b91bebd42)
Figure 5 – Laser voltage probing on the same circuit.

Figure 5 shows a snippet of waveform acquisition using both the  lasers. It was observed that the signal strength of the 1319nm  laser was higher than the   $1122\mathrm{nm}$  laser.

The signal to noise ratio (SNR) was calculated using the formula  below

SNR=(Peak Signal Strength)/(Standard Deviation of Noise)

SNR versus Laser power graphs in Figure 6 and Figure 7 below  show that while the SNR increases proportionally with power,  1319nm laser shows a much larger signal strength than 1122nm,  before and after normalizing the power to the absorption within  the aplanatic SIL. This is probably because of differences in the  quantum efficiency for the two lasers in the detector as well as  unaccounted losses within the device.

![120  120 Signal to Noise Ratio 100  100 80  80 60 40 20 20  0 0  2  4  6  6  8  1O  10 Laser Power(mW) Laser Power(mw)  1319nm  1319nm  1122nm  1122nm ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/eda9c16e-6c48-4859-a58e-edf067126dd3/eda9c16e-6c48-4859-a58e-edf067126dd3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=b506f08f29a078c986130c83b6c642b50145f12b)
Figure 6 – SNR versus Laser Power.

![4000  3000  leusy  2000  1000  1O  LaserPower(mw)  1319nm   1122nm  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7b403f0c-b585-4560-a1e5-303d2367acf1/7b403f0c-b585-4560-a1e5-303d2367acf1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=e50d34e11064801d2bc1da83c6ae723d7b71c136)
Figure 7 – Signal strength versus Laser Power.

In conclusion, for laser voltage probing,   $1319\mathrm{nm}$  laser provides  a superior signal strength and SNR as compared to   $1122\mathrm{nm}$   laser

Soft Defect Localization:  Soft defect localization was  performed on a sub 20nm FinFET device using   $1064\mathrm{nm}$  ,  1122nm and 1319nm lasers.

Figure 8 shows a comparison of SDL images on 1064nm versus  1122nm. Figure 9 shows a comparison of SDL images on  1319nm laser versus   $1122\mathrm{nm}$   laser.

![300nm  300 nm   300nm  300 nm              1064nm @ 0.1mW 1064nm @ 0.1mW               1122nm @ 0.81mW 1122nm@0.81mW  Figure 8 - SDL on 1064nm versus 1122nm.  Figure 8 – SDL on 1064nm versus 1122nm.  300 nm  300 nm  300 nm  300nm            1319nm @ 1mW 1319nm @ 1mW               1122nm @ 0.81mW  1122nm @ 0.81mW ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/23266204-6708-49c9-9cf7-37dbf2288dee/23266204-6708-49c9-9cf7-37dbf2288dee.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=21eb2ad00b13b1e6abd0c8ec92c1b5e3bf904df2)
Figure 9 – SDL on   $1319\mathrm{nm}$   versus   $1122\mathrm{nm}$  .

Figure 8 shows a high-resolution image of SDL analysis using   $1064\mathrm{nm}$   at   $0.1\mathrm{mW}$   and 1122nm laser at   $0.84\mathrm{mW}$  , it can be  observed that for   $1064\mathrm{nm}$  laser, at a very low laser power of   $0.1\mathrm{mW}$  , the SDL site is dispersed. This could be attributed to the  intrusive effect of 1064nm laser. At higher laser power, the SDL  encompassed the entire cell thereby rendering the SDL analysis  obsolete. There could be circuitries which are extremely  sensitive to   $1064\mathrm{nm}$   laser even at low laser powers.

Figure 9 shows a high-resolution image of SDL analysis using   $1319\mathrm{nm}$   laser at 1mW and   $1122\mathrm{nm}$   laser at   $0.81\mathrm{mW}$  , The SDL  site at   $1319\mathrm{nm}$  laser is stronger probably because a higher laser  power of 1mW was used as compared to   $0.84\mathrm{mw}$   on   $1122\mathrm{nm}$    laser. Adjusting for the increased laser power in 1319nm laser, it  can be interpreted that the 1319nm SDL image is comparable to  1122nm SDL image

As observed from Figure 8 and Figure 9, 1122 laser performs  better than   $1064\mathrm{nm}$  laser for fault isolation in this case and is  comparable to 1319nm laser in terms of defect localization.

SDL Analysis helped in identifying the suspected defect location  Physical failure analysis was performed on the suspected SDL  site (Figure 9). Top down de-processing of the device showed no  significant anomaly till lower metal layer. Nano Probing  revealed short between gate and active (Figure 10)

![Ivcurve  IV curve 1.2 1-2  1 Current (µA) 0.8  0.8 0.6  0.6 0.4  0.4 0.Ｚ  0.2 0 0  0.2  0.2  0.4  0.4  0.6  0.6  0.8  0.8  1  1.2  1.2 Voltage(v)  Voltage(V) ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/35d63fa6-9a08-494d-aca3-77524842a59b/35d63fa6-9a08-494d-aca3-77524842a59b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=83ff00b5e34fd6b1212a93d2a02ce2b8c19e6fb8)
Figure 10 – Nano probing showed a short between gate and  active.

FIB cross section followed by TEM inspection along the SDL  site area showed (shown in Figure 11) a short between gate and  active

![50 nm  50 nm  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/eca139ca-1ae2-4db8-b7b5-522232473036/eca139ca-1ae2-4db8-b7b5-522232473036.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215673%3B1743219273&q-key-time=1743215673%3B1743219273&q-header-list=host&q-url-param-list=&q-signature=db92bad1d2e83156ea0f787aac861729de007fb0)
Figure 11 – TEM result indicating a short.

5 0  n m

SGP DALAB

Thus, from the case study above, it can be concluded that SDL  analysis at   $1122\mathrm{nm}$   laser helps to isolate the fault at a better  precision than 1064nm laser while offering image resolution  improvement as compared to 1319nm laser. This allows better  CAD alignment at   $1122\mathrm{nm}$  , without compromising a spread in  the SDL site.

## V. C ONCLUSION 

This paper draws comparisons between 1122nm, 1319nm and  1064nm low noise lasers for fault isolation. Frequency mapping  showed that based on Gaussian FWHM, the 1122nm laser offers  a better resolution than   $1319\mathrm{nm}$   laser. Laser probing showed  that 1319 nm has a superior signal strength and Signal to noise  ratio as compared to   $1122\mathrm{nm}$   laser.  SDL analysis was  performed on   $1064\mathrm{nm}$  ,   $1122\mathrm{nm}$   and   $1319\mathrm{nm}$   laser and the

results were compared. 1122nm and   $1319\mathrm{nm} $  laser was  observed to localize faults better than   $1064\mathrm{nm}$  .

Despite a loss in the signal strength, the resolution  improvements add value for the use of   $1122\mathrm{nm}$   laser with Si-aplanatic SIL. Due to the superior transmission to   $1064\mathrm{nm}$   the  laser can potentially be used for full silicon laser probing as well.  Therefore,   $1122\mathrm{nm}$   laser serves as an alternative to the  conventional 1319nm and 1064nm lasers by bring the desirable  properties of each laser into its arsenal.

## A CKNOWLEDGMENT 

Authors would like to thank AMD Singapore and Semicaps  Singapore for sponsoring this work.

$\copyright$  2019 Advanced Micro Devices, Inc. All rights reserved.  AMD, the AMD Arrow logo, and combinations thereof are  trademarks of Advanced Micro Devices, Inc.  Other product  names used in this publication are for identification purposes  only and may be trademarks of their respective companies.

## R EFERENCES 

[1]    Jiann Min Chin  et al ., “Fault isolation in semiconductor  product, process, physical and package failure analysis:  Importance and overview,” Microelectronics Reliability  (September 2011), 51 (9-11), pp. 1440-1448.

[2] Ulrike Kindereit, “Fundamentals and Future Applications  of Laser Voltage Probing,” IEEE-IRPS 2014 section 3F.1 (11  pp.) 978-1-4799-3317-4/14/\$31.00 ©2014 IEEE

[3] Michael R. Bruce, Victoria J. Bruce, David H. Eppes, Jacob  Wilcox, Edward I. Cole Jr., Paiboon Tangyunyong, Charles F.  Hawkins, “Soft Defect Localization (SDL) on ICs” 28th  International Symposium for Testing and Failure Analysis,  November 2002.

[4] Venkat-Krishnan Ravikumar  et al ., “Continuous- wave  1064nm laser for Laser Voltage Imaging and Probing  Applications,” Proceedings from 40th International Symposium  for Testing and Failure Analysis 2014, pp. 344-348.

[5] SH Goh  et al ., “Experimental Demonstration of the Effects  of Laser Pulse Duration on SEU and LADA in CMOS Devices,”  Proceedings from the 42nd International Symposium for  Testing and Failure Analysis, pp. 559-566.

[6] Venkat Krishnan Ravikumar,  et al ., “Understanding spatial  resolution of laser voltage imaging”, Microelectronics  Reliability, Volumes 88–90, 2018, pp. 255-261, ISSN 0026- 2714

