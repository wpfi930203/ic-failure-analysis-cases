---
title: "191_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_397b4d8c1d1645bee726871f9e9c22037295230462135641
file_size: 1500265
---

## Root Cause Analysis on Analog Circuit Using TR-LADA 

Lua Winson 1 , Phoa Angeline 1 , Gopinath Ranganathan 1 , AS Girish 1 , Ravikumar Venkat Krishnan 1,2   1. AMD Inc. 2. Singapore University of Technology and Design, Singapore;   Correspondence email:  winson.lua@amd.com

Abstract  -  Analog circuits are traditionally harder to debug  using light assisted device alteration (LADA) also known as  dynamic laser stimulation (DLS), as the circuitry are too  sensitive to carrier generations. This paper showcases a  successful post-silicon debug on analog circuitries (start-up  circuit) using nanosecond pulse-on-demand laser to perform  DLS leading into root cause identification on a marginality  issue in a sub-20nm FinFET technology device.

## I.    INTRODUCTION 

Dynamic Laser Stimulation (DLS) is a dynamic fault  isolation technique used on marginal failures. DLS employs  continuous wave (CW) near infrared (NIR) lasers with photon  energies larger than the Silicon bandgap such as   $1064\mathrm{nm}$   to  alter the drive strength of transistors and helps expose  bottlenecks in the circuitry tested. The technique requires the  chip to be biased such that there is an equal probability of the  device to pass or fail under a specific test condition [1]. The test  is constantly looped and its status monitored while the laser is  raster scanned across a field of view containing sensitive  circuitry. The pass/fail result is mapped to each pixel where the  laser is momentarily positioned at while evaluating the test.  When the laser hits sensitive circuitry, the pass/fail ratio  changes dramatically and is observed as a cluster of passing or  failing sites. When overlaid with the laser reflected image, this  cluster shows the location of the sensitive circuitry which can  be examined further.

While DLS is great for failure analysis and timing analysis, it  has practical limitations when debugging analog circuits.  Unlike digital circuits, the functionality of an analog circuit  often  depends on relative drive strength of the devices in the  circuit. This means that intrusions such as carrier injections  during DLS in an analog circuitry can cause fatal errors and  result in false failures. Sometimes, the testing is not recoverable  until a hard reset.

Time resolved LADA (TR-LADA) has been introduced as an  enhancement technique to obtain timing information of the  observed DLS site [2]. Instead of a continuous beam as is  conventionally used, laser is pulsed such that photons interact  with the transistor at just the right moment in time that is critical  to the test. Since this reduces the spread of carriers in the  connected active devices, it helps reduce the spatial spread of  the DLS site. References [2] and [3] demonstrate situations  where TR-LADA provided useful information related to the  exact time that triggered the failure. Additionally, as TR-LADA  allows the laser to be pulsed in short discrete bursts, it  minimizes the average laser power reducing the potential for  laser induced damage.

TR-LADA can be implemented in several ways depending on  the timing precision, time resolution (pulse width) and peak

optical power of the laser desired. Depending on the laser  source, it may be necessary to add more electro-optic  components to control the timing parameters and to sync the  laser pulse with the critical test instructions [4]. Figure 1  summarizes the 4 different TR-LADA methods that were  considered for the specific implementation used in this paper.

The transistor-transistor logic (TTL) as it is commonly  known, is the input of a regular laser source, that allows it to be  powered on and off. Sending a pulse into this input, therefore,  allows generation of a laser pulse, but the generated pulse width  being greater than 5us is too wide to arrest carrier migration in  the well. The electro-optic modulator (EOM) allows for a better  time resolution, but reduces the peak laser power of the system,  reducing the intrusive effect of the laser. The femto-second  pulsed laser provides a pulse that is several thousandth of a test  cycle (typically 10ns-100ns). Such a pulse width would not  allow adequate coverage within a test cycle.

Figure 1: Comparison of laser sources.

|TYPE|TTL|EOM||        ns Pulse                on-demand      |        fsPulse                on-demand      |
|---|---|---|---|---|---|
|Time resolution|>5 HS |>50ns|>50ns|>1 ns|>100 fs|
|||||||
|Average Power|High|Medium||LOW|Low|
|Peak Power|High|LO||High|Very High|
|        Large time                window search      |yes|yes||Yes|70|
|Cost|Cheap|        Moderate-                Expensive      |        Moderate-                Expensive      |Moderate|Expensive|


In the specific implementation highlighted in this paper, the  abilities to pulse the laser at will, vary the laser pulse width  widely with adequate laser power, and at the right wavelength;  and be economical were all desired. The pulse-on-demand  nanosecond 1063nm laser satisfied all these requirements.

This paper showcases the use of the nanosecond pulse-ondemand laser to localize a design-process marginality within an  analog circuitry, where the failure only appeared in specific  power ramp condition and caused some IO pads to be stuck at  a wrong state.

## II.    EXPERIMENT SETUP  

The hardware setup for TR-LADA with pulse-on-demand  laser [4] is described in Figure 2. The conventional DLS system  requires the tester and scanning optical microscope (SOM). ( 1 )   The tester exercises the DUT at the pass-fail boundary of shmoo  and ( 2 ) returns the results to the SOM. ( 3 ) The SOM performs

raster scans of NIR laser at the area of interest and ( 4 ) creates a  DLS image.

For TR-LADA setup, we have added the pulsed laser source  which needs an additional signal to trigger the pulse. ( 5 ) The  tester triggers a delay module with which ( 6 ) a precise and  calibrated delay is added to the trigger as input to the pulsed  laser.  Finally, ( 7 ) the pulsed laser is coupled into the scanner to  allow raster scanning.

This setup also allows the use of pulsed laser in free running  mode without tester synchronization.

![TESTER  5. Tester triggers module  1. Tester exercises Device  TriggerDelay   2. Tester sends test  module   evaluations to SOM   Device  Scanning Optical Microscope  6. Module triggers   (SOM)  lasersource  3. Laser intrusions  onDevice  Pulsed laser  source  Pulsed  4.SOMcreates theLADA overlay  laser  TR-LADA overlay image  toSOM  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/26675a14-550e-4ee6-bc25-f8a69ad324c1/26675a14-550e-4ee6-bc25-f8a69ad324c1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215647%3B1743219247&q-key-time=1743215647%3B1743219247&q-header-list=host&q-url-param-list=&q-signature=f11990cf6e2858bd44f0472aa0f25af7aa7175de)
Figure 2: TR-LADA hardware setup.

## III.    PROBLEM STATEMENT 

Several input/output (IO) pads were reported as stuck-at-high  fails after booting up. Further debug showed that while booting  up, adjusting ramp rates or adding delays to two internal power  supplies, VA and VB, caused some IO pads output to become  stuck at high state unexpectedly. Readjustment of the ramp  rates with different delay setting would fix the anomalous  behavior.

Figure 3. shows screenshots from an oscilloscope monitoring  the ramp of power rails and the voltages on the affected IO pads.  In Figure 3.a, both power rails VA and VB are ramped together,  with the same ramp rate and no delay between the rails. The  monitored pad (green trace) is pulled to high anomalously. In  Figure 3.b, the same power rails are ramped with slightly  different ramp rates. Here, the monitored trace stays low, as  expected.

![(a)Samerampratefor  VAandVB  2.25y  I0 pad stuck  athigh  (b)Differentramprate  for VAand VB  I0padstaylow  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/aa936ed2-7e88-40cc-b320-30aae023b682/aa936ed2-7e88-40cc-b320-30aae023b682.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215647%3B1743219247&q-key-time=1743215647%3B1743219247&q-header-list=host&q-url-param-list=&q-signature=876353a20d1c3af3072814dc7c9cb1a6d2687c84)
Figure 3: (a) IO pad (green) is stuck at wrong high state when  ramping VA (blue) and VB (yellow) power rails together. (b) By  changing the ramp rate for both power rails, the IO pad  remains in Low state.

Fault isolation was performed using the static setup with  breakout board and power supplies.  By adjusting ramp rates  and delays between the supplies, the failure was replicated.

Photon Emission Microscopy (PEM) was first conducted to  study differences in emission between good and bad conditions.   One abnormal PEM site was observed on the failing pad at  stuck-at-high state, but further investigation indicates the  observed PEM site was the consequence of the failure rather  than the actual defect. The anomalous emission occurred  because the IO pad was a dummy that has been grounded in the  package. Since the pin was pulled to a high state, it resulted in  a contention between the output driver of the dummy pad and  VSS resulting in a strong emission. The PEM technique was not  useful in narrowing down the defect location.

![(a) Pass condition    (b) Fail condition    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f8009cda-5904-42f2-951c-9c4e889b3a56/f8009cda-5904-42f2-951c-9c4e889b3a56.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215647%3B1743219247&q-key-time=1743215647%3B1743219247&q-header-list=host&q-url-param-list=&q-signature=141d6fc00b24ea4356f456d65d1755de2afe6205)
Figure 4: Abnormal PEM site was observed at the failing  condition, but it was because of a contention created by the fail  and did not point to the cause of the failure.

The device was subsequently setup for DLS. The power  supplies were made to ramp up and down simultaneously with  precise ramp rates. The monitored pad provided pass/fail results  based on whether the pin was pulled high or not. The settings  were tuned in such a manner that the failing behavior could be  observed with a   $50\%$   probability. To minimize the voltage  fluctuation from the pad due to VA and VB switching, the pad  is connected to another trigger module which allows the output  signal to be triggered at discrete High or Low state to SOM.

Conventional DLS with 1064nm CW laser was performed  but due to the sensitivity of the analog circuitries to the NIR  laser, the entire IOs area was covered by DLS sites as shown in  Figure 5.a even with the minimum laser power of   $0.1\mathrm{mW}$  .  There was no site with 1340nm laser stimulation either. This  made DLS ineffective.

The CW laser was switched with the 1063nm pulse-ondemand laser diode and set to produce 100ns laser pulses with  repetition of 1us pulse rate. This resulted in a significant fault  localization   improvement.   The   pulse   widths   were  systematically dropped until the most sensitive circuitry was  uncovered as shown in Figures 5.b, 5.c, and 5.d.

![(a)1064nm DLS  CWlaser  2560um  380um  (b)1063nmTR-LADA  Pulsewidth=100ns  810um  380um  (c)1063nmTR-LADA  Pulse width =4.5ns  480um  360um  (d) 1063nm TR-LADA  Pulsewidth=3.4ns  220um  170um  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b449d68a-3a63-4f15-8ee4-0fd550aa88c8/b449d68a-3a63-4f15-8ee4-0fd550aa88c8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215647%3B1743219247&q-key-time=1743215647%3B1743219247&q-header-list=host&q-url-param-list=&q-signature=af7acaf5b391b4777ba6e22e57b7802714ee5709)
Figure 5 : Comparison between DLS and TR-LADA site under  5X magnification. (a) CW laser shows huge site across the  entire IO pads with an area of   $\ \ \ 0.97m m^{2}$  . (b) TR-LADA with  100ns pulse width reduces the spot size to   $0.3m m^{2}$  . (c) Smaller  pulse width improves the localization size. (d) 3.4ns pulse width  provides 0.04mm 2 . Note the TR-LADA site can be reduced  further with higher magnification lens.

Higher resolution TR-LADA with solid immersion lens (SIL)  further isolated the observed single low mag site into a few finer  sites as shown in Figure 6, allowing the design debug on the  circuit of interests.

![270X  2DLSsitesatControlCircuit  270X  4DLSsitesatIOpad  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1461585f-70db-4944-a60a-583d65c5017d/1461585f-70db-4944-a60a-583d65c5017d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215647%3B1743219247&q-key-time=1743215647%3B1743219247&q-header-list=host&q-url-param-list=&q-signature=cf9ade0014c52395222785c2055ce5cae3ebfc3f)
Figure 6 : 1063nm pulse-on-demand laser uncovered more  distinct sites under 270X magnification. DLS site A and B are  located at the Control circuitry, DLS site C to site F are located  at the failing pad.

The observed TR-LADA sites are located at 3 main design  blocks; one at the Control_Sync circuitry inside the Control  Block, while the other two are Sel_A and Sel_B circuitries  which acts as a master control for the level shifter. All three  circuities are inputs to a multi input AND gate, which feeds to  a SR latch.

Figure 7 shows that the minimum pulse width needed is more  than 3.3ns as the ultra-short pulse width of 3.3ns did not  produce any TR-LADA site, likely because the peak power  from the laser source began to drop below 4ns pulse width.

![(a)3.3ns pulse width  No TR-LADA site  (b) 3.5ns pulse width  WithTR-LADAsite  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2f2ef22c-3df7-429d-8e48-b4fed2799d20/2f2ef22c-3df7-429d-8e48-b4fed2799d20.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215647%3B1743219247&q-key-time=1743215647%3B1743219247&q-header-list=host&q-url-param-list=&q-signature=b7b532ad96eff42628e7fef7089297f9f2639eb8)
Figure7 : (a) 3.3ns pulse width with less than 150mW peak  power insufficient to alter the device performance. (b) 3.5ns  pulse width observed TR-LADA sites at the area of interest.

Design verification confirmed that the AND gate output  should remain LOW throughout the operation, that any High at  AND gate output could cause the SR latch to output a 0V.  This  subsequently turns on the Pad PMOS driver and pull up the pad  to a high state. A block diagram for the mentioned circuitries  relationship are shown in Figure 8.

![A   B  3.3W  SigA  SelA  PadgoHigl  Control   SR  Input  Sync   Latch  AND  SigB  SelB  LevelShifters   Pre-Driver   Driver  Control Circuit   IOPad  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2726982b-b534-4341-be86-b3e95a7b81ec/2726982b-b534-4341-be86-b3e95a7b81ec.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215647%3B1743219247&q-key-time=1743215647%3B1743219247&q-header-list=host&q-url-param-list=&q-signature=f1755e7701ba0407b4723e2ebdd8b848393969cc)
Figure 8 : A hypothesis suggested that the pad could pull to high when the SR latch output a 0V, and only happened when the multi  input AND gate output goes high at the same time, where all the inputs observed the TR-LADA pass sites.

Detailed analysis was performed on the Control_Sync  signal as this signal is the primary input to the level shifters  and therefore the AND gate. Monte Carlo simulations were  performed with various ramp rates and delays in between to  check the maximum glitch at the Control_Sync output. The  results show when both VA and VB are ramped together at  faster ramp rate, a large voltage glitch  appeared on the  Control_Sync. A glitch that is   $28\%$   worse than the passing  condition is able to  trigger the level shifters to output a High  state, exacerbating the pad to stuck-at-high.

The failure was subsequently root-caused to an extreme  threshold voltage variation in the circuitry. To ensure the  glitch does not reoccur, it was fixed by a minor design  alteration to minimize the glitch on Control_Sync signal.

## IV.    CONCLUSION 

PEM is useful for localizing the physical defect but might  not work well with the failure that non-defect-related. As  analog circuitry is sensitive to the laser intrusions and  sometimes causing false results, CW laser is unsuccessful  in exposing the defect.

The results clearly show that nanoseconds pulse-ondemand laser or similar highly controllable pulsed lasers  can help to distinguish actual TR- LADA sites that matter  to the failure by eliminating byproduct DLS sites caused by  CW NIR laser in the analog circuitry. By optimizing the  pulse width and laser power of pulse laser, we have  successfully isolated the TR-LADA sites further and root  caused the issue by analyzing the design blocks and  replicated the fails with Monte Carlo simulations.

## ACKNOWLEDGMENT 

Authors would like to thank AMD management for  sponsoring this work. Also, authors would like to express  their gratitude to Cheng, Yee-Ling and Chen, Wei-wen for  their valuable inputs.

$\copyright$   2019 Advanced Micro Devices, Inc. All rights  reserved. AMD, the AMD Arrow logo, and combinations  thereof are trademarks of Advanced Micro Devices, Inc.   Other product names used in this publication are for  identification purposes only and may be trademarks of their  respective companies.

## REFERENCES 

[1]   Rowlette, J; Eiles, T, "Critical Timing Analysis in  Microprocessors Using Near-IR Laser Assisted Device  Alteration (LADA)",  International Test Conference  2003 Proceedings

[2]   D Bodoh et al., “Root Cause analysis techniques using  pico-second time resolved LADA”,  ISTFA 2014

[3]   K. Erington et al., “Measuring Propagation Delays of  Critical Paths Using Time-Resolved LADA”  IRPS  2014    [4]   VK Ravikumar et al, “Implementing Time Resolved  Laser Assisted Device Alteration using Pulse-ondemand nanosecond Laser Diode ”,  ISTFA 2016

