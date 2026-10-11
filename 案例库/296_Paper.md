---
title: "296_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_7c74c8364043fa2fb79ca5e33cf535c97295230462135641
file_size: 4568134
---

## Practical Dynamic Laser Stimulation Technique and  Code Modification: A Soft Defect Localization  Approach for Microcontroller Self-Test Failures  

Kevin Joshua S. Cala, Junald C. Saludares, and Wendel A. Basbas \*   1 Microchip Technology Inc., 102 Accuracy Drive cor. Excellence Ave. Carmelray Industrial Park 1, Calamba, 4028, Philippines.  \* Phone: (049) 549-0563   Fax:   (049) 536 2171  Email:  kevinjoshua.cala@microchip.com,   junald.saludares@microchip.com,  wendel.basbas@microchip.com

Abstract-   A practical alternative for soft defect localization (SDL)  and fault isolation of dynamic failures is presented. The approach  utilizes an existing optical beam induced resistance change  (OBIRCH) hardware without a dynamic laser stimulation (DLS)  add-on kit, coupled with an exhaustive electrical sample prep step  which involves code modification. The technique was proven  effective in localizing failures pertaining to resistive interconnects  which are rather difficult to analyze using conventional static  techniques.

Keywords  –  Soft-defect localization, Fault isolation, Dynamic  failures, Self-test code, Dynamic laser stimulation .

## I. I NTRODUCTION 

Defect localization is a critical step in failure analysis (FA). It  is a make or break step for the succeeding physical analysis  steps. With the variety of available defect localization  techniques, analysts must determine which techniques are  appropriate based on failure mode and defect classification.

Conventional static laser stimulation (SLS) techniques such  as optical beam induced resistance change (OBIRCH) and  emission microscopy (EMMI) are largely successful in  pinpointing defect sites for static failure modes [1]. For  dynamic failure modes with soft defects, soft defect localization  (SDL) techniques such as dynamic laser stimulation (DLS) are  applied [2] – [3].

An ideal setup for DLS of microcontroller self-tests failures  uses complex test systems interfaced and synchronized with an  SLS equipment with a DLS add-on kit [4]. The test system  typically involved is an automated test equipment (ATE) tester.  In the case that the DLS add-on kit and the ATE tester are  unavailable, a practical alternative approach is proposed in this  paper with minimal equipment needed.  This approach utilizes  existing SLS equipment and with the aid of self-test code  modification realizes it usage for DLS. Finally, to prove the  effectiveness of this approach, actual FA cases are discussed.

## A.  Laser Stimulation and its Effects  

Laser stimulation results in either photoelectric or  photo-thermal effects induced to a device under test (DUT),  depending upon the laser wavelength used. Laser techniques  based on photoelectric effect make use of a laser wavelength  around the silicon bandgap region,   $1.064~\mathrm{~um}$   in popular  systems. Active structures are excited and measured for shifts

in order to localize faults pertaining to junction issues, open or  latch up sensitivity. For dynamic applications, laser assisted  device alteration (LADA) had also been introduced.

On the other hand, photo-thermal techniques rely on the fact  that changing the temperature of a given material changes its  electrical properties. For example, heating up a metal structure  changes its resistance, thereby producing a corresponding  voltage or current variation which can be used to track down a  defect. To ensure that only thermal effects are introduced, a  higher wavelength is used, typically 1.34 um. This is the  working principle of the OBIRCH which is a widely used static  technique to isolate leakage and resistive failures. However,  such technique is ineffectual when it comes to localizing  dynamic failures and mechanisms pertaining to soft defects.

![PHEMOS1000  Laser   Scan  Controller  Immage  Acquisition  Microscope  Card  Photodiode  imput  IC-Driver   LaserSource  DUT  DALS Kit  output  Amplifier  Measurement  Umit  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d1c4e609-6060-4efa-9f6a-b19445e31e2d/d1c4e609-6060-4efa-9f6a-b19445e31e2d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=4b93b961b5f484eaaf8b795e3c8eaa3fb9200162)
Fig. 1 Block diagram of HAMAMATSU PHEMOS 1000 laser stimulation  system with DALS kit.

A laser stimulation system from Hamamatsu is shown in Fig.  1. The Laser Scan Controller scans the beam onto the DUT’s  surface pixel by pixel both to stimulate the DUT and to acquire  the reflected image.

During static analysis, the weak current or voltage changes  caused by laser stimulation are fed to an amplifier whose output  serves as input to the Image Acquisition Card (IAC) for data  processing.

Dynamic analysis is realized with the use of the Dynamic  Analysis by Laser Stimulation (DALS) kit. This kit can accept a  pass/fail (P/F) trigger from a tester or evaluate an output signal  (analog or digital) coming from the DUT itself. A change from  pass to fail and vice versa, as well as change in the DUT’s  output signal characteristics such as amplitude, frequency and  duty cycle are processed by the kit and sends that information to  the IAC. Moreover, the DALS kit can modulate the laser scan  function by accepting external synchronization signals from a  tester.

## C.    Fault Isolation Challenges related to Dynamic Tests  

One dilemma of using a dynamic test like the self-test “as-is”  is that they may result in extra emissions not related to the true  failure. The self-test code is a collection of instructions hence,  the device executes numerous other instructions in the test aside  from the failing instruction, which is the root of the self-test  failure. On a classic liquid crystal technique, the CPU (Central  Processing Unit) would have generated a lot of heat and made  the liquid crystal less sensitive to the heat generated by the  failing instruction [6].

From an emission microscopy perspective, instructions  before the failing instruction may produce pockets of transistor  emissions. The same is true for instructions after the failing  instruction, but instead of just introducing emissions un-related  to the failure, these emissions could be due to a dependency  from that failing instruction thus, secondary emissions.

For a practical DLS method to work, it is critical that only the  vital lines of the code are running, and that the P/F trigger is  sent immediately after the failing instruction, otherwise there  will be an offset on the localization result. Hence, there is a  need to debug and minimize the self-test code, if possible, down  to the very first failing instruction in order to minimize the  inspection volume and maximize localization rate.

## II.   EXPERIMENTS  

The experiment starts with the characterization of the failing  self-test and identification of DLS P/F trigger point by  performing shmoo plotting. With a deep dive into the self-test  assembly code, the specific failing instruction is determined  through debugging. Self-test code is then minimized with only  the vital instructions running. Lastly, practical DLS is  performed with the minimized code.

![Failure mode  characterization   Practical DLS  Self-test code  and   with minimized  modification  identification of   code  P/F trigger point  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b16b12ba-292e-48aa-96ca-83b3bd1e7d7f/b16b12ba-292e-48aa-96ca-83b3bd1e7d7f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=b743aeab723de9c56d2a3b0be738ed3e0c5138fb)
Fig. 2 Summary of steps for the methodology.

An open-top or open-bottom bench board is used for the  DUT with the addition of the following materials and  equipment per step as seen from Table I.

Table I - Parameters used in 2-D simulations

|Steps||Materials and equipment|
|---|---|---|
|        Failure mode characterization and                identification of P/F trigger point      |||
|        Failure mode characterization and                identification of P/F trigger point      ||        Temperature forcing system                or heat gun      |
|Self-test code modification||        Programmer/debugger                Laptop/Desktop      |
|Self-test code modification|||
|Practical DLS with minimized code||        HAMAMATSUPHEMOS                1000 without DALS kit                OBIRCH DLS diode-resistor      |
|Practical DLS with minimized code||        OBIRCH DLS diode-resistor                network      |
|Practical DLS with minimized code||Clock source|
|||Variable power supply|
|||Programmer/Debugger|


A.

Failure mode characterization and identification of P/F

trigger point

The main target of self-tests are to capture functional failures  within dense, internal circuit blocks, and peripherals of the  microcontroller. The first step is to check whether the self-test  failure is not due to some other parametric failure. This can be  done by a thorough review of the ATE datalog. Once proven  that it is a genuine self-test failure, it is then checked if the unit  passes on specific conditions of voltage and frequency, i.e. if it  is having a soft defect characteristic. If this is the case, then the  sample is a good candidate for the practical DLS. A shmoo plot  is then generated in order to know P/F boundaries. A shmoo  plot at room that is significantly shifted versus a known good  plot may indicate suitable bias points for a DUT be it hot or cold  temperature failure. A certain point on the P/F boundary is then  selected for bias conditions. Then a quick check is done to  determine how the device reacts with temperature.

![0.5ns/Di  Going Good  GoingBad  failedpasse   0.05V/Di  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7dc01d85-99ec-4229-8350-afbd4b2fe611/7dc01d85-99ec-4229-8350-afbd4b2fe611.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=b0e2bde679414fe2ad6334dcf33663ccbaa65829)
Fig. 3 Example shmoo plot.

Depending upon the impacted circuit and nature of the defect,  the P/F boundary may shift. If the part is “going good” under  the influence of heat, the initial condition of the DUT on the  practical DLS set-up should be on the edge of the Failed region,  otherwise it should be biased on the edge of the Passed region.  When discernable, the final set-up should be at the operating  point most sensitive to temperature, which is usually at the  voltage and clock corners. This point will be the P/F trigger  point.

B.    Self-test code modification for fault validation

The focus of code debugging is to do fault validation and  isolation. Thus, replicate the failing ATE test results in bench  setup.

![Code  Compilation of   Measuring the  debugging and  self-test   execution time.  minimization  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e380d3e0-f7d4-417c-84e6-ed09f13bc805/e380d3e0-f7d4-417c-84e6-ed09f13bc805.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=57ad104d7ee8a70000e58f17bbe4bc3eeabd55ac)
Fig. 4 Basic process for self-test code modification.

The process starts with the compilation of the self-test. Once  compilation is successful, the extracted self-test is ready for  code debugging. It is advisable to run the compiled self-test  code first on a good sample to check the setup integrity. Once  setup is proven good, code debugging, and minimization is  done as shown in Fig. 5.

![Runthe  self-test  Stepinto  thecode  Stepinto  thecode  Anstruction  Passor   failing?   NO  fail?  Pass  yes  Fai  Minimized  thecode  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c95f6ef8-ebe8-4461-87d3-11f103bfbaa5/c95f6ef8-ebe8-4461-87d3-11f103bfbaa5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=75f1b2eb38495704d15a379edfc628b2d7c595ef)
Fig. 5 Flow chart for code debugging and minimization.

![ExampleMinimizedcode  Preconditioning instructions  Examplecode   Staxe  clr R16 clear register 16  c1rR17  1d1R16,   RE  1d1R17   RT  0x01toR18  DDRD,R18;PD0  Failing instruction  orR16，R17；e   dR16=  Compareinstruction  cpse rl6, rl7 ;compare then skip if equal  dRle  Pass/Fail Routine  jmp failure jump to failure routine  uccess ;jump to success routine  failure:  1d1 R18,0x01 ;fai1 signat  out PORTD，R18  rjmpstart  access:  ldiR18,   passsignatt  out PORTD，R18  rjmp start  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7d92fea7-6500-4b23-8e4c-9eb83e0f7795/7d92fea7-6500-4b23-8e4c-9eb83e0f7795.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=a8fb4a11876fbcd73d91231488d1ded1382001f5)
Fig. 6 Illustration of example self-test code vs minimized code.

The minimized code should only include the vital lines of the  code for better result in defect localization. The final step is to  measure the execution time of the minimized code. This is to  ensure that the DUT transitions from pass to fail or vice versa at  the exact moment that the laser raster on the defect site.

The execution time is the product of the code’s clock cycles  and clock period of the chosen pass/fail point.

$$t_{e x e c}=N_{c y c l e s}*P e r i o d$$
To ensure excitation of the defect and registration of the P/F  transition, the execution time must be less than minimum pixel  dwell time of the SLS equipment [7].

$$t_{e x e c}\leq P i x e l\;d w e l l\;t i m e$$
Table II – Example of different execution time for core self-test program

|Code size|1.0 MHz|8.0 MHz|16 MHz|
|---|---|---|---|
|Whole self-test program|6, 912 us|864 us|432 us|
|Failing self-test program|346 us|43.25 us|21.63 us|
|Minimized Failing self-test|14 us|1.75 us|0.88 us|


The Table II shows the simulated execution time of a sample  self-test program at different code size or modification levels  versus clock speeds. It shows how reducing the number of  instructions as well as increasing the clock speed reduces the  total execution time. This means that aside from minimizing the  code itself, larger or more complex self-test programs can run at  a higher clock speed in order to attain a lower execution time.  But there is a limit to the range of available clock speeds. The  clock speed chosen should still correspond to a trigger point  within the P/F boundary that transitions from pass to fail or vice  versa. Nevertheless, the lower the execution time relative to  pixel dwell time, the higher is the chance that P/F toggles  happen at the exact moment that the laser is scanning right at  the defect site, hence more accurate localization.

The visual representation shown on Fig. 7-9 depicts the  significance of the minimized code during laser stimulation.  Referring on the figures, the defect site was represented on  one-pixel area. Fig. 7 shows the effect of executing the code  beyond the laser pixel dwell time. In this case, the P/F routine of  the code runs after the laser excite the defect site thus no  OBIRCH signal found. This is a different scenario if the code is  minimized as shown on Fig. 8 and Fig. 9. For Fig. 8, the  minimized code P/F routine executes after approximately   $50\%$    of the dwell time happened. It would create an OBIRCH signal  since one P/F transition occurred within the point of laser  excitation. For Fig. 9, the P/F routine runs more often than the  previous minimized code. The more P/F transition loop within  the laser pixel dwell time, the better OBIRCH signal can be  obtained.

![Time(us)   No hotspot  Laserpixeldwelltime  Start of code  P/FRoutine      Fig. 7 Illustration of execution time of the whole self-test code vs laser pixel    Fig. 7 Ilustration of execution time of the whole self-test code vs laser pixel  dwelltime  dwell time  Time(us)  Laserpixel dwell time   Start of code  P/F Routine    Fig. 8 Illustration of execution time of the minimized self-test code (1) vs  Fig. 8 Illustration of execution time of the minimized self-test code (1) vs  laser pixel   dwell time  laserpixeldwelltime  Pixeldwelltime  Time(us  Laserpixel dwell time  Start of code  P/FRoutine    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a2ae681a-4d82-4edc-b2c8-e7486c7d6d8f/a2ae681a-4d82-4edc-b2c8-e7486c7d6d8f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=d8b2df7dacd37f0f31bdafa87f9f0605fce22903)
Fig. 9 Illustration of execution time of the minimized self-test code (2) vs  laser pixel   dwell time

The importance of minimizing the code may extend to  EMMI analysis. Fig. 10 and Fig. 11 show how the emission  sites were reduced just by removing certain instructions and  retaining the vital ones. It could also help to avoid some  masked emission due to unnecessary high intensity emission  sites.

![（b） ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f53b9cbc-4e11-4834-963f-a6a96d6da975/f53b9cbc-4e11-4834-963f-a6a96d6da975.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=7a1b44fe182be7dfdab22e3095a9947073854309)
Fig. 10 (a) Emission sites for minimized code and (b) emission site for whole  self-test codes.

![（b） ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/57bfc2b7-a4e8-4ef1-9731-ca1aa80a09db/57bfc2b7-a4e8-4ef1-9731-ca1aa80a09db.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=fa97fe6a850ecbbc03f0a25d900405587423953c)
Fig. 11 (a) Emission sites for minimized code and (b) emission site for whole  self-test codes.

## C.    Customized DLS Setup  

The practical solution presented in this paper is depicted in  Fig. 12.

![PHEMOS 1000  LaserScan  Controller  Image  Acquisition  Microscope  Cardl  Photodiode  imput  IC-Driver   Laser Source  DUT   NOt  DALSkit  Available  DLS  Network   Amplifier  Measurement  Umit  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/859e951f-cc0b-41c5-b410-13c13cc9e3ae/859e951f-cc0b-41c5-b410-13c13cc9e3ae.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=07f30f3132e952cea1b8e1cc195b135934903525)
Fig. 12 HAMAMATSU PHEMOS 1000 laser stimulation system without the  DALS kit customized for DLS analysis.

The PHEMOS 1000 was used but with a minor change. A  network between the DUT and the OBIRCH amplifier was  added. The DUT itself generates the P/F signal using  microcontroller’s CPU and I/O (input/output). Since the  introduced network will now become “part” of the DUT, any  current or voltage change due to P/F toggles will be sent to the  IAC by the amplifier itself. As can be seen, the practical DLS  set-up actually makes use of the static laser stimulation signal  chain in order to isolate a dynamic failure. Voltage mode of  DUT biasing was used, using a 1340 nm laser wavelength.

## D.    OBIRCH DLS Network Simulation Results  

The network introduced between the DUT and OBIRCH  amplifier is shown in Fig. 13, comprised of a current limiting  resistor and a blocking diode which prevents unwanted current  flow towards the OBIRCH amplifier. This diode also  standardizes the polarity of the current change registered by the  machine in order to avoid confusion. The other end of the  network connects to the I/O pin of the DUT which sends the P/F  trigger.

![TRIGGER  Open-top or  OBIRCH  Open-bottom   RCL  Bench Board GND   amplifier  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/577a2a15-d449-4d4e-a385-61118d9f4b27/577a2a15-d449-4d4e-a385-61118d9f4b27.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=e9335f6e06fb1d3ba44e73316287e9a32a37c3db)
Fig. 13 DLS network between DUT and OBIRCH amplifier.

Circuit simulation was performed in order to visualize the  effects of certain variables in and around the DLS network. For  the simulation results, refer to Fig. 14.

![R1  10k   1N4148  P/F_Signal   OBIRCH  PULSE(0 5 0 10n 10n 1m 2m 2)  .tran 0 4m 0 5n  -I(P/f_signal)  V(p/f_signal)  I (obirch)  V(obirch)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4bf88878-b0b8-446b-b871-62626beec08b/4bf88878-b0b8-446b-b871-62626beec08b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=5bef5bf9cc98f6037e14c2ab8408e88d26556eef)
Fig. 14 DLS network simulation results showing a reliable P/ F trigger  occurring when OBIRCH amplifier is set to logic high.

The following table of generalizations were then derived  from the simulation work.

Table III - Effects of OBIRCH Amplifier Bias Voltage and I/O Pin Logic State  Combinations to Current

|OBIRCH Amplifier Bias Voltage|I/O Pin Logic State|Current|
|---|---|---|
|Logic low voltage|Logic high|Negligible current; sink current stopped by protection diode|
|Logic low voltage|Logic low|No current reading|
|Logic high voltage|Logic high|No current reading|
|Logic high voltage|Logic low|Source current|


Basing on the table, to have a reliable P/F trigger, the  OBIRCH bias voltage should be on the high side, with logic  high voltage of the I/O pin as the optimum. A high-to-low  toggle on the I/O pin results in a change in the current, from  zero to maximum current. Conversely, a low-to-high toggle will  result to a change from maximum to zero current. Each of these  conditions will show the same OBIRCH site but with differing  colors due to different polarity in current change. Refer to Fig.  15.

![（b) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a6d396a4-3776-4d71-a2ee-42db1a00db08/a6d396a4-3776-4d71-a2ee-42db1a00db08.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=a1f008fbcef29624082ed06c6fbd216af6a48214)
Fig. 15 Laser image overlaid with (a) red OBIRCH site vs (b) green  OBIRCH site.

The current flowing around the network can be controlled by  setting the value of the resistor and/or OBIRCH bias voltage.

## E.    Practical DLS Procedure  

Fig. 16 shows a practical DLS setup for a microcontroller  self-test failure. The DUT is set to the P/F trigger point by  adjusting the clock source and power supply. The  programmer/debugger is used in case additional modifications  are needed on the code.

![a   CLK IN  Clock  Open-top or GND   Source  Programmer  Open-bottomVcc  /Debugger  DEBUGBenchBoard   Power  LINES  GND   Supply  GND   TRIGGER  DLS  Networki  OBIRCH  Amplifier    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/04fed4a8-1d44-4349-acd1-174d73babb96/04fed4a8-1d44-4349-acd1-174d73babb96.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=2ab2d47f12d4b6aef55febd675e8da4b53193d2b)
Fig. 16 (a) Block diagram representation of DLS set-up. (b) Sample actual DLS  set-up.

It is recommended that the bench board has onboard LEDs  through which the IO port is connected. The analyst can use one  of the LEDs to keep track of the P/F signature. An indication  that the DUT is set on the boundary of the shmoo is that the P/F  signature through the LED is continuously changing.

Once the DUT is set on the desired P/F point, the analyst can  now begin laser scanning. Several scan settings were  experimented on the cases in the results and discussion. The  settings that yield the best images, i.e. with highly localized  OBIRCH site, are low-speed high-resolution scans. Different  orientations for the scan could also be performed to add  confidence on the OBIRCH site location during layout analysis.

Table IV - Suggested DLS scan settings

|Scan Settings|Suggested DLS Settings|
|---|---|
|Laser (%)|20% - 40%|
|Scan Orientation|Horizontal (left to right) and Vertical (top to bottom)|
|Number of Frames|30 – 60 Frames|
|Scan Resolution|1024 x 1024|


In the HAMAMATSU PHEMOS 1000, an OBIRCH image  improvement tool can be used to further improve OBIRCH site  localization.

![<a）  （b） ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ef4ef084-f068-4b6b-bd54-24113c226d41/ef4ef084-f068-4b6b-bd54-24113c226d41.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=580770800ea370d686c6fbdbc42d8e2c9b92cba1)
Fig. 17 (a) Laser image overlaid with OBIRCH site vs (b) Laser image  overlaid with OBIRCH site with image enhancement.

III. R ESULTS AND DISCUSSION

Table V - FA Case no.1 – Register Write Failure

|Device|Failure Mode Type|Failure Symptoms|
|---|---|---|
|Product A|Functional Self-test failure|Register write failure at cold temperature|


Failure mode characterization and identification of  pass/fail trigger point:  Characterization of the unit shows that  its behavior on the self-test is worsening at cold temperature  and improving at hot temperature. The trigger point chosen is a  failing point just below the P/F boundary at room temperature  shmoo. This point will transition to a passing point with the  application of heat from the laser.

![ApplicationofheatoftheDUT  COLDSHMOO   ROOM SHMOO   HOT SHMOO  Failing at   Failingat   Passing at  trigger point  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/85935d4d-707c-435c-8c47-405dd605a2ed/85935d4d-707c-435c-8c47-405dd605a2ed.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=f77e442e64de0ade1e0069053313adbf165ca071)
Fig. 18 Changes on shmoo plot and trigger point state with the application of  heat.

Self-test code modification:  Unit is failing on ATE testing at  self-tests that performs register writes and reads. Further  debugging of the self-test reveals that the unit is failing when  writing on registers R6. Code is minimized to include vital  instructions that will excite the failure.

Practical DLS with the minimized code:  Practical DLS  showed an OBIRCH site on the core circuitry. The OBIRCH  site coincides with a via between top metal and metal 2.

Additional data from emission microscopy showed emitting  gates that are connected to the OBIRCH site-coincident via  through a single net.

![（aD ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5208ff08-5eb9-4dd5-9394-8eda36e39748/5208ff08-5eb9-4dd5-9394-8eda36e39748.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=93753b1415a3ba30927b406eb068bced774eacbb)
Fig. 19 (a) Net trace showing OBIRCH site-coincident via connected to (b)  emitting gates.

Physical   analysis:    TEM   (Transmission   Electron  Microscope) and EDX (Energy-Dispersive X-ray) was  performed on the suspected failing via. The via was observed to  be misaligned as compared to a good via and a gap exists  between the via and the top metal. Only a small alloyed bridge  connects the via to the top metal causing it to be resistive.

![HAADF   HAADF  #7152   #7153EM0G  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/37f2495d-0611-4923-941e-920949cd4fab/37f2495d-0611-4923-941e-920949cd4fab.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=a4fea4bad2660d009fa0d1fd486a923e20f413d7)
Fig. 20 (a) TEM image of failing via showing misalignment with the top  metal and malformed interlayer between via and metal and (b) TEM image of  reference via.

![HAADF OSiAI W TN   HAADFO   AWTN  7152  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/82eb23ae-dc13-4079-9be8-15145d286462/82eb23ae-dc13-4079-9be8-15145d286462.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=bed8b70af2e5ca53ab0b24fd85b51dd6fe06d848)
Fig. 21 (a) EDX image of failing via showing gap between the top metal and  the via with a small alloyed bridge connecting the via and the top metal and (b)  EDX image of reference via.

Table VI - FA Case no. 2 – Arithmetic Instruction Failure

|Device|Failure Mode Type|Failure Symptoms|
|---|---|---|
|Product B|Functional Self-test failure|Failure in executing a arithmetic instruction at room temperature|


Failure mode characterization and identification of  pass/fail trigger point:  Characterization of the unit shows that  its behavior on the self-test is failing during the application of  hot temperature. A trigger point at fail region was chosen to  transition from failing to passing point when heated by the  laser.

![ROOM SHMOO   HOT SHMOO  Failing at trigger point   Passing at trigger point  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e693f019-2f49-4dad-b3ec-20a048323f50/e693f019-2f49-4dad-b3ec-20a048323f50.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=563cde64a55c9333f6f1a8e453576abd857d27c2)
Fig. 22 Changes on shmoo plot and trigger point state with the application of  heat.

Self-test code modification:  The unit is failing at multiple  self-test. A self-test that test the multiplier for stuck-at faults  was chosen for the debugging. During debugging, it was  identified that the instruction ‘fmuls’ (Fractional Multiply  Signed) introduce intermittent result on the sample when being  executed.

Practical DLS with the minimized code:  Using the  practical DLS approach, OBIRCH site on the core circuitry was  captured that coincides on the net trace of all the abnormal  emission on the driven gates in which connected to a driver cell.

![DriverCell  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/131a1c9b-b615-4e43-9d00-dce81cd5be5d/131a1c9b-b615-4e43-9d00-dce81cd5be5d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=c5b15878f15af9e42c29eed7b56d61a84873943d)
Fig. 23 Net trace showing OBIRCH site connected to emitting gates.

Physical analysis:  Cross-section using FIB (Focused Ion  Beam) was performed on the suspected failing via. TEM and  EDX image shows unexpected high amount of nitrogen in  between the top metal and via. This insulating material induced  additional resistance on the via thus making it highly resistive.

![（b） HAADF 300nm HAADF MAG:79.0k ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6f2a0200-e6dc-4c27-bd96-d25509cf69b5/6f2a0200-e6dc-4c27-bd96-d25509cf69b5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215703%3B1743219303&q-key-time=1743215703%3B1743219303&q-header-list=host&q-url-param-list=&q-signature=f061df98b895415777521d3d02d83c8e6537a4c1)
Fig. 24 (a) TEM image showing insulating material between the top metal  and the via and (b) EDX image of the sample showing high amount of nitrogen  which acted as insulating material.

## IV. C ONCLUSION 

A practical DLS technique for microcontroller self-test  failures was presented in this study which requires the  following   electrical   sample   preparation   steps:   device  characterization and self-test code minimization. It was shown  that with a minor modification on a defect localization setup,  the static OBIRCH system can be used to isolate dynamic  failures and localize soft defects which are resistive  interconnects on the cases showcased in the results and  discussion section.

This setup is simpler, as it uses basic equipment readily  available on most FA laboratories. It is effective, as it was  successfully applied on several cases. Finally, it is economical,  as it allows FA laboratory to maximize the usage of its  equipment and still perform DLS for microcontroller self-test  failures even without expensive equipment.

The technique also dramatically reduces turnaround time of  an FA case for resistive interconnect defects as compared to  performing FIB cuts and microprobe measurements. The  electrical sample preparation steps will typically take only  around 4 hours and the DLS itself will take about 2 hours. In  about 6 hours, the FA can now submit the unit for TEM and  EDX on a defect site with very high probability of revealing a  defect.

## A CKNOWLEDGMENT 

The authors would like to thank the Microchip Philippines FA,  Colorado Springs FA, Norway Product Engineering, and  Tempe Lab teams.

Special thanks to the analysts of FA case no. 2, Celdrian Rei  Asilo and Maria Rosalina Reyes, and the co-inventors of the  technique, Tim Mcgrady, Andy Blemker and Tor Joerund  Sund.

## R EFERENCES 

[1]    F. Beaudoin, et al, “Principles of Thermal Laser Stimulation Techniques”,  Microelectronics Failure Analysis,   Materials Park, Ohio: ASM  International , pp 417-425, 2004.     [2]    P.H. Llamcra, et al, “Soft Defect Localization of Hot Failure by Dynamic  Analysis by Laser Stimulation using Hamamatsu iPhemos”,  2018 IEEE  International Symposium on the Physical and Failure Analysis of  Integrated Circuits (IPFA) , pp 1-5.K, 2018.    [3]    M.R. Bruce, et al, “Soft defect localization (SDL) in integrated circuits  using laser scanning microscopy”,  The 16th Annual Meeting of the IEEE  Lasers and Electro-Optics Society , pp 662-663, 2003.     [4]    K.Y. Chao, et al, “Laser Assisted Device Alteration, Efficient Application  for Soft Failure Localization on Advanced Node”,  2018 IEEE  International Symposium on the Physical and Failure Analysis of  Integrated Circuits (IPFA) , pp 1-4, 2018.    [5]    T. Kiyan, “Dynamic Analysis of Tester Operated Integrated Circuits  Stimulated by Infra-Red Lasers”,  Thesis dissertation , 2010.    [6]    Y.E. Hong et al, “An Overview of Advanced Failure Analysis Techniques  for Pentium and Pentium Pro Microprocessors, Intel Technology  Journal”, 1998.    [7]    W. Chunlei, et al, “A Novel Method to Realize Soft Defect Localization  Techniques without a Synchronization Signal for Failure Analysis”,  2009  16th IEEE International Symposium on the Physical and Failure Analysis  of Integrated Circuits , pp. 237-240, 2009.

