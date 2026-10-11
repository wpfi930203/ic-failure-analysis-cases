---
title: "114_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_9ec9d140aa2eddbcc378a8c1a6583b677295230462135641
file_size: 1323296
---

## Integrating NI LabVIEW in Soft Defect Localization  of Temperature Dependent Voltage Failure  

Paul Hubert P. Llamera 1 , Camille Joyce G. Garcia-Awitan 2 ,  Febus Reidj Cruz 3 , and Glenn Magwili 4   Maxim Integrated – Failure Analysis Department, Gateway Business Park, General Trias, Cavite, Philippines  School of Electrical, Electronics, and Computer Engineering, Mapua University, Manila, Philippines  Phone: +632 902 2000 local 2396;   Email:  1 Paul.Llamera@maximintegrated.com,  2 Camille.Garcia@maximintegrated.com,    3 reidjcruz@gmail.com,  4 gvmagwili@yahoo.com

Abstract-   One of the challenges in the field of failure analysis is the  effective failure characterization and fault isolation of devices  which only fail on specified region of temperature, frequency, and  voltage. Soft defect localization is used for the failure localization  of such cases. In this paper, a LabVIEW program was utilized and  developed for failure characterization and localization to help in  the soft defect localization of two devices with output voltage  temperature   dependency   failure   during   hot   and   cold  temperatures. Moreover, the Dynamic Analysis by Laser  Stimulation (DALS) capability of Hamamatsu iPhemos was  utilized in performing the soft defect localization process.

Keywords – Soft Defect Localization (SDL), Dynamic Analysis by  Laser Stimulation (DALS), NI LabVIEW, Temperature Dependent  Failure, Hamamatsu iPhemos.

## II.   I NTRODUCTION 

Failure analysis is a comprehensive and systematic  investigation to determine failure mechanisms and root causes  of how and why devices are failing. The determination of root  cause helps in preventing reoccurrence of this failure  mechanisms. The key to successful failure analysis depends on  the comprehensive failure verification and characterization and  effective fault isolation technique to pinpoint root cause of  failure by providing the physical manifestation of defect.

Different industries demand for devices and products that can  withstand applications over a wide range of temperature.  Consequently, the need for support in devices that failed in  customer application over temperature changes pose new  challenges in the current techniques used in failure analysis due  to devices which fail only at certain temperatures. This type of  failure is called soft defect. [1]

Soft defects are subtle defects that causes a device to be only  partially functional and will not operate under certain conditions  which may or may not be within normal limits. [2] It is difficult  to detect this type of defect using conventional failure analysis  techniques. [3] To address these cases, Soft Defect Localization  (SDL) was introduced. [4] SDL is a collection of various laser  scanning fault isolation techniques such as Resistive  Interconnection Localization (RIL) [6], Laser Assisted Device  Alteration (LADA) [7] and Dynamic Analysis by Laser  Stimulation (DALS) [8] that evaluates the pass/fail condition of

a device under test (DUT). SDL is considered as an effective  way to localize soft defects. [1, 5]

## 1.1 NI LabVIEW  

If a device is reported to fail at a specified temperature,  datalogging of failing parameter versus temperature is needed  to verify the failure. Automation in data gathering for such cases  can be performed by using Laboratory Virtual Instrument  Engineering Workbench more commonly known as LabVIEW.  LabVIEW is an engineering software that can be used for data  gathering, controls and automation for different applications.

LabVIEW offers an extensive support for interfacing devices  and equipment by creating a user interface to hardware  communication for control and automation.

In this study, LabVIEW was integrated for failure  characterization and localization on two devices that failed on  output voltage parameter during hot and cold temperatures.

## 1.2 Dynamic Analysis by Laser Stimulation (DALS)  

The Hamamatsu iPhemos is one equipment that can be used  for several fault isolation techniques such as Optical Beam  Induced Resistance Change (OBIRCH), Photo Emission  Microscopy (PEM) and the Dynamic Analysis by Laser  Stimulation (DALS).

DALS is an SDL technique that uses the principle of laser  stimulation where the die is scanned with laser and observed its  operating status change (pass/fail). Fig. 1 shows the DALS  concept used in Hamamatsu iPhemos where the DUT is  stimulated using a   $1.3\upmu\mathrm{m}$   laser while it is operating under  normal condition. The laser scanning produces photoelectric  and photothermal effects on the die resulting to thermal energy  production (heat) that creates electrical variation on the DUT  resulting to a change in its operating status (pass/fail). Hence,  when an area sensitive to temperature is scanned with laser, a  change in the DUT’s operating status will occur resulting to a  pulse generation that is fed into the DALS system. The pulse  collected by the DALS system is then expressed into image  pattern defined by difference in pixel color. Superimposition of  the pattern generated on the image system to the die pattern will  determine the location of areas sensitive to temperature. [5]

![LASER（1.3μm）  Pass/Fail map  correspondingtolaserscan  LSltester  TestPattern   Image  formation  Pass/Failstatus  ExPass=High  DUT  FaBLV  Failurelocation  Change in status in reaction to  Status changes due to  thelaser=failurelocation  laserheat  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/39073e76-b702-4493-b402-70d4a34383b8/39073e76-b702-4493-b402-70d4a34383b8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=e98c2442b06715ad595255d30fcefad360d482a9)
Fig. 1.  DALS Concept using Hamamatsu iPhemos

In this study, DALS was utilized to determine the location of  the defect on the two devices with output voltage temperature  dependency failure during hot and cold temperatures. The  scanning time and resolution of laser scan were varied to get the  best result.

## II.   R EVIEW OF  R ELATED  L ITERATURE 

In 2012, Dynamic Laser Stimulation (DLS) was used by A.  Deyine, et al to determine the failing component of a device that  only fails at low temperature and low voltage. A specific  transistor was found to be the sensitive area in the device. An  anomaly on the electrical behaviour on the component was  observed after microprobing. [9] Same technique was utilized  by P. Llamera, et al in fault localization of a device that fails  only at hot temperature. A process defect was observed on a  bipolar junction transistor (BJT) during FIB cross-section and  STEM analysis. [10]

In a study conducted by Chi He, et al, the process of capturing  the location on the soft defect was further enhanced by adding  a pulse generator. The pulse generator would transmit a  narrower pulse to the DALS system before its integration with  the image system. A more localized DALS image was captured.  The success of the SDL analysis using DALS was confirmed  after doing physical failure analysis (PFA). [5]

Hat, Sabate and Yusof conducted a study to compare several  heat generators (thermal module, heat gun and thermostream)  which aided in the analysis of hot failures. [11]

In a study conducted by Szabó, Gontean and Lie, LabVIEW  program was successfully used to automate a temperature  chamber with RS-232 interface. Several applications of the  automated temperature chamber were also presented. [12]  Ahmad, Nordin, Saaid, et al also used LabVIEW to create  virtual instrumentation in 2017. [13]

## III. M ETHODOLOGY 

Fig. 2 presents the failure analysis (FA) process methodology  that was followed in this study. The DUTs were tested on bench  by monitoring the failing output voltage parameter over  temperature. When the temperature dependency of failure of the  DUTs was confirmed, further electrical characterization using a  LabVIEW-based program to log the output voltage parameter  while temperature is increased from minimum to maximum

specified operating temperature range of the DUTs was  performed. This was done to analyse the behaviour of the DUTs  over temperature that would help in performing DALS. An NI  LabVIEW program was developed when the failing parameter  cannot be fed directly to the DALS system.

The DUTs were decapsulated to expose the die. Bench re-test  was performed to observe any change in the behaviour of the  DUTs after decapsulation. The device was scanned using the  laser of Hamamatsu iPhemos to determine if a change in its  operating status (pass/fail signal) can be generated. The output  voltage parameter of the DUTs were monitored using  oscilloscope, and the laser power was gradually increased until  a change in the DUTs’ operating status was observed. When a  change in state of the failing parameter was confirmed, the  failing parameter was fed into the DALS system and DALS in  Analog mode was performed on the DUTs.

![START  BENCH  TEST  TEMP  DEPENDENT  FAILURE?  YES  FAILURE  NILABVIEW  CHARACTERIZATION  INTEGRATION  (NI LABVIEW)  NEED   YES   NILABVIEW  <PROGRAMFOR   PROGRAM  DALS?   DEVELOPMENT  20  BENCH RE-TEST  DECAPSULATION   USING NI LABVIEW  PROGRAM  BENCH RE-TEST  USING NI LABVIEW  PROGRAM  FAILURE   DALS (SDL)  CHARACTERIZATION  IN HAMAMATSU  FAULT   N工  ISOLATION   LABVIEW  (DALS)   PROGRAM  PHYSICAL  FAILURE  ANALYSIS  END    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5c15d85c-d61e-4485-92ae-8c556e5d8f3b/5c15d85c-d61e-4485-92ae-8c556e5d8f3b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=69f720a06c18a0c2366aa95f93fa4d3b8df49997)
Fig. 1. FA Process Methodology

Fig. 3 shows the DALS mode: Analog process where a  continuous test pattern is applied on the DUT and observed the  resulting integral tester signal (failing parameter) per loop  trigger in every pixel scan. The voltage levels of the tester signal

are translated to equivalent image data.  In performing DALS,  the unit is scanned pixel by pixel using a   $1.3\upmu\mathrm{m}$   laser while the  DUT is operating under normal condition. The laser power was  set high enough to cause a change in the DUT’s operating status  while varying the scanning time and resolution of laser scan to  get the best result. The generated DALS image (PASS/FAIL  image) was superimposed to the infrared (IR) image to locate  and identify the areas sensitive to heat.

![Test pattern  Looptrigger  Pixelclock  Testersignal  (-5<V<5)  Resei  Imagedata  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4e531c39-e0b8-440d-94c2-d3de4bc4fb08/4e531c39-e0b8-440d-94c2-d3de4bc4fb08.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=1fd60b6ef26199b572bc2b24cced41bd417815fe)
Fig. 3.  DALS Mode: Analog

The identified localized sensitive area was then subjected to  optical inspection using high magnification microscope.  Microprobing and circuit analysis for further electrical  verification was also performed. Focused ion beam (FIB) crosssection and Scanning transmission electron microscopy  (STEM) imaging was performed to observe the physical  manifestation of the defect should no obvious defect is seen  during high magnification optical inspection.

## IV. R ESULTS AND  D ISCUSSION 

## NI LabVIEW Failure Characterization Program  

An existing LabVIEW program was used for failure  characterization thru bench test automation on the two devices  with output voltage temperature dependency failure. Fig. 4  shows the flowchart of the LabVIEW program where the DUTs  were automatically operated on their specified minimum and  maximum operating temperature range and their failing  parameter is measured per temperature increase. Results were  logged on an excel file.

![Initialize   Measure   Measure   Log   Ramp  Equipment   Temperature   Parameter   Data   Temperature  Excel  Set Min and  File  Max Temp  2O   LOoP  Finish?  Set Sampling  Time  TESTLOOP  YES  Turn On   Close   End  Supply   Equipment   Program  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b6e9c1fb-02fa-48e3-9569-deb56cc7d07e/b6e9c1fb-02fa-48e3-9569-deb56cc7d07e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=82b4899eb4caf330bfd68066e33137e436686286)
Fig. 4.  Bench Test Automation LabVIEW Program Flowchart

## Case 1: Hot Temperature Failure  

An undervoltage/overvoltage (UVLO/ OVLO) device was  confirmed to fail on comparator output voltages at hot  temperature during bench test using typical operating circuit.  Failure characterization using the LabVIEW program showed  that the comparator output voltages fail at temperature above   $33^{\circ}\mathrm{C}$   as shown in Fig. 5.

![25.3   32   65.9   87.4   106.6   122.8  Temperature(°C)  DUTOUTE   KGUOUTA  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1f21949b-5cd9-44b5-8db9-6cafd8a4246c/1f21949b-5cd9-44b5-8db9-6cafd8a4246c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=5f9ec3c2cd119abb18ab4f9333abd78fb6326ef9)
Fig. 5.  Comparator Output Voltage vs Temperature

Failure characterization in Hamamatsu iPhemos showed that  a   $30\%\cdot40\%$   laser power is enough to make the DUT fail. Fig.  6 shows an oscilloscope shot of the comparator output voltage  when the DUT was scanned with laser.

![Pass  Pass   Pass  Pass  rai  Fail  2Me   12%  3920  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ce9af24d-a94e-44a5-b2b0-ecd8c284bcc2/ce9af24d-a94e-44a5-b2b0-ecd8c284bcc2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=7d597d64f35d82e9c19693d94e6cb3681e57d9b7)
Fig. 6.  Comparator Output Voltage Scopeshot when scanned with laser

Fig. 7 shows the set-up used in performing DALS on the  DUT. The output voltage of the DUT is fed into the DALS  system of Hamamatsu iPhemos while being monitored using  oscilloscope. The change on the DUT’s operating status from  PASS to FAIL was stimulated using a   $30\%–40\%$   laser power  while varying scanning resolution and time to get best result the  least time possible.

![Power  Supply   Supply   LASER  DUT   IPHEMOS  Output   Tester  Voltage   Oscilloscope   Signal  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9ed18f04-4a30-4b3a-b98e-eae3cc956a20/9ed18f04-4a30-4b3a-b98e-eae3cc956a20.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=7421c5df143e57b77cb904e0c65e6896b12cb28b)
Fig. 7.  Case 1 Hot Temperature Voltage failure DALS Set-up

Fig. 8 (a) shows the DALS image generated during fault  localization. Gray and/or white pixels correspond to PASS  while black pixels correspond to FAIL. In Fig. 8 (b) the  superimposed image   $(\mathrm{IR\mathrm{~+~}D A L S})$  ) shows that the fail signal  (temperature sensitive area) is on a bipolar junction transistor  (BJT) inside the power management circuit block of the DUT.

![  (a)     (b)   b  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/23ebc88b-9662-4a46-b994-7b275795dc5d/23ebc88b-9662-4a46-b994-7b275795dc5d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=d4c6c2024727441aea3242bd14e3062645a5ca5c)
Fig. 8.  (a) DALS image and (b) superimposed DALS image on IR image

Optical inspection on the BJT using high magnification  microscope failed to show anomaly. However, microprobing  thru curve trace testing, revealed an I/V curve anomaly between  the collector-base and emitter terminal of the BJT. In Fig. 9,  curve trace test showed an open connection in the reverse bias  region between the collector-base and emitter terminal of the  transistor.

![   a  (a)     (b)   b  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f9458391-ae27-4cf1-863e-fd4a56fb8c64/f9458391-ae27-4cf1-863e-fd4a56fb8c64.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=0445987ccef083cd31ae8ca1755874522f253fdd)
Fig. 9.  Collector-base and emitter terminal I/V curve on a (a) DUT (b) KGU

The BJT was subjected to FIB cross-section and STEM  imaging. Fig. 10 shows anomalous contact formation and void  underneath the contact of the emitter terminal of the BJT. A  particle remnant was observed on top of the void.

![125/201d17.50kD      a  (a)     (b)   Cb  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fb7a5a1a-3d9d-4f12-8b18-d79eee2138ab/fb7a5a1a-3d9d-4f12-8b18-d79eee2138ab.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=0bb718b1ad227eef6e9d2b557a23528d7024bee4)
Fig. 10. (a) SEM image and (b)STEM image

Fig. 11 shows that the failing BJT forms a current mirror with  Q2 transistor that controls the current flowing through the  internal UVOUT net. For a current mirror to work properly, the  two transistors formed must be matched and should be identical  at same temperature. The electrical signature of the defect  suggests that at hot temperature the defect creates a mismatch  between the Q1 and Q2 transistors of the current mirror. The

mismatch between the two transistors causes lower pull-down  current on the UVOUT net which results to UVOUT asserted  high and comparator output voltages low.

![COMIP_OUT  Failing BJT  Failing BJT  JVLO  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a5953e39-ebaf-43ed-96fb-921b51958c19/a5953e39-ebaf-43ed-96fb-921b51958c19.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=38c3ae2b584f54a3603f8883486a3022390f260f)
Fig. 11. Simplified Schematic showing failing BJT

## Case 1: Cold Temperature Failure  

A led driver device was confirmed to fail on output switching  signal at room and cold temperature during bench test   using  ATE test set-up on oscillation frequency. Fig. 12 shows that the  DUT exhibits low duty cycle at room temperature while stuck  low output switching signal at cold temperature and good output  switching signal at hot temperature. However, fault isolation  thru emission microscopy at room temperature failed to show  distinct emission sites on the unit in reference to a good unit  even if the DUT is already failing.

![（a  (a)  1Frec     Cb  (b)    C  (c)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7f4d97aa-4c2d-4ce7-b6ab-3a041e170870/7f4d97aa-4c2d-4ce7-b6ab-3a041e170870.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=4a1610c9c0782660e01636a06edef0016c964c23)
Fig. 12. Output Switching Signal Oscilloscope at (a) room (b) cold and (c) hot

The existing LabVIEW program was modified to measure the  frequency   of   the   output   switching   signal.   Failure  characterization using the modified LabVIEW program showed  that the output switching signal fails on switching frequency at  temperature below   $-25^{\circ}\mathrm{C}$   as shown in Fig. 13.

![700000.000  600000.000  500000.000  0000.000  100000.000  0.000  124122  Temperature(°C)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8f118c50-afd3-4c3b-94ee-dd85da5f47e6/8f118c50-afd3-4c3b-94ee-dd85da5f47e6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=b0b7853cffb8437d325d0c4590793b691fa7f023)
Fig. 13. Output Switching Signal Frequency vs Temperature

The failing parameter is a switching signal that cannot be fed  directly to the DALS system of Hamamatsu iPhemos. Fig. 14  shows the new LabVIEW program flowchart developed  converting the switching signal to its mean DC equivalent.

![Initialize   TurnOn   ConvertSwitching   Checkif  Equipment   Supply   Signal to DC   PASS/FAIL  20  scan   TestSignal   Send  Complete?   iPHEMOS   Signal  TESTLOOP  YES  Close   End  Equipment   Program  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/509f8f9e-b10e-41fb-8f0f-6a821c201468/509f8f9e-b10e-41fb-8f0f-6a821c201468.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=e12e42e5c007e27ebeb3250b91c34395df4e8c9c)
Fig. 14. LabVIEW Program Flowchart

Failure characterization in Hamamatsu iPhemos using the  developed LabVIEW program showed that a   $15\%\cdot20\%$   laser  power is enough to make the DUT pass. Fig. 15 shows the  oscilloscope shot of the output switching signal when the DUT  was scanned with laser.

![  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4808e6b0-bd7f-4442-9bf7-79f1191169f5/4808e6b0-bd7f-4442-9bf7-79f1191169f5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=cb0bc3737e305ae848449d1f11a57e0fa62829b9)
Fig. 15. Output Switching Signal Scopeshot when scanned with laser

Fig. 16 shows the set-up used in performing DALS on the  DUT. The DUT was powered up using the SMUs of the NI PXI

module and the output switching signal was fed into the module.  The mean DC equivalent of the output switching signal is  outputted on one of the NI PXI’s SMUs and fed into the DALS  system of Hamamatsu iPhemos. The change on the DUT’s  operating status from FAIL to PASS was stimulated using a   $15\%{-}20\%$   laser power while varying scanning resolution and  time to get best result the least time possible.

![SMU   Supply  LASER  Output  H/O   Oscilloscop   Switching Sign  NI PXI   DUT   IPHEMOS  SMU   Tester  Signal  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/32f6a288-3e00-4df2-bd3d-5b3ef7db5d47/32f6a288-3e00-4df2-bd3d-5b3ef7db5d47.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=82c05d12ea52afffb2a5efb39d24bf75445b1437)
Fig. 16. Case 2 Cold Temperature Voltage failure DALS Set-up

Fig. 17 (a) shows the DALS image generated during fault  localization using DALS. Gray and/or white pixels correspond  to FAIL while the black pixels correspond to PASS. In Fig. 17  (b) the superimposed image (IR + DALS) shows that the pass  signal (localized sensitive area) is on a MOS transistor inside  the bias circuit block of the DUT.

![  Ca  (a)     (b)   CD  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/48630d67-5c32-4fd5-a5a0-0b085a55b1b6/48630d67-5c32-4fd5-a5a0-0b085a55b1b6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=14f91be6ede5412aa39a80466ada0431ddb047b1)
Fig. 17.  (a) DALS image and (b) superimposed DALS image on IR image

Optical inspection on the MOS transistor using high  magnification microscope failed to show anomaly. However,  defect was observed on a capacitor that is connected to the gate  of the MOS transistor where DALS signal was observed as  shown in Fig. 18.

![Poly2 Poly2 Poly1 Poly1  (a)  （a）   (b)  CD1 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e42f1299-51dc-4caf-8295-2af411f80d88/e42f1299-51dc-4caf-8295-2af411f80d88.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=22be5974660607b2de194093653fa821208713e6)
Fig. 18. (a) Dark Field optical and (b) FIB image showing defect on capacitor

Fig. 19 shows that the faulty capacitor is connected to gate of  the MOS transistor where DALS signal is observed. The failing  capacitor caused abnormal bias current to the PWM circuit  block of the unit resulting to faulty output switching signal.

![PTATCurrent  BiasCurrenttoPWM  RT  DALS Signal  DALS Signal   NN3   NN2   NN4.  Failing Cap  Failing Cap  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f21085a6-5b7a-47b1-ac24-84c73b0b9c91/f21085a6-5b7a-47b1-ac24-84c73b0b9c91.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215624%3B1743219224&q-key-time=1743215624%3B1743219224&q-header-list=host&q-url-param-list=&q-signature=3af4294561492194da38468bc55298552d67ba22)
Fig. 19. Simplified Schematic showing Failing Capacitor

## V.   C ONCLUSION 

With the increasing difficulties and challenges in failure  verification and fault isolation on devices that failed only at  specified conditions, a comprehensive and systematic failure  analysis must be done. In this study, NI LabVIEW was  successfully integrated in the soft defect localization on the two  devices with temperature dependent output voltage failure. A  LabVIEW program was successfully developed for failure  characterization thru bench test automation and for converting  a switching signal to its mean DC equivalent to able to perform  DALS.

Moreover, the DALS capability of Hamamatsu iPhemos was  successfully utilized and proven to be an effective fault isolation  method for localizing and identifying defects of two devices  with temperature dependent output voltage failure. The  scanning time and resolution of laser scan were varied to get the  best result.

## VI.   R ECOMMENDATION 

The current study is only limited to bench test automation  monitoring a single parameter over temperature which only  gives a part of the total functional behaviour of the device. To  further understand and for an in-depth analysis of the functional  behaviour of a DUT over temperature changes, future  researchers may consider the development of Shmoo Plot of the  DUT. Shmoo plot may be used to understand the behaviour of  the device over operating voltage and temperature changes,  observing at what combination of voltage and temperature will  the DUT fail. Hence, making the failure localization process  easier.

While bench test provides actual behaviour of the DUT over  temperature, the characterization during laser scanning provides  behaviour of the DUT over laser power. Hence, creating a gap  and misalignment between the results of the two failure analysis  processes. Future researchers may consider studying the  effective equivalent temperature induced by the applied laser  power thus correlating bench test characterization result to  failure localization process during laser scanning.

## VII.   A CKNOWLEDGMENT 

The authors would like to thank Camille Garcia-Awitan and  Jed Paolo Deligente for the LabVIEW program used during  bench test automation and characterization, Febus Reidj Cruz  and Glenn Magwili who served as academe advisers, FA FIB  team for performing the FIB cross-section, Fritz Christian  Awitan for carrying out STEM imaging and Jerome Escobedo  for supporting and making this project happen.

## VIII.   R EFERENCES 

[1]    J. Li, L. Zhai, et. al, 18th IEEE International Symposium on the Physical  and FailureAnalysis of Integrated Circuits (IPFA), 2011, 1–4.    [2]    M. R. Bruce, V. J. Bruce, et. al, The 16th Annual Meeting of the IEEE  Lasers and Electro-Optics Society, 2, 2003, 662–663.    [3]    V. K. Ravikumar, S. L. Phoa, et. al, 2008 15th International Symposium  on the Physical and Failure analysis of Integrated Circuits, 2008, 1–4.    [4]    M. R. Bruce, V. J. Bruce, et al, Proceedings of the 28th International  Symposium for Testing and Failure Analysis (ISTFA), 2002, 21-27    [5]    C. He, D. Fan, et. al, 2017 IEEE 24th International Symposium on the  Physical and Failure Analysis of Integrated Circuits (IPFA), 2017, 1–4.    [6]    E. Cole, P. Tangyuanyong, et. al, Proceedings of the 9th International  Symposium on the Physical and Failure Analysis of Integrated Circuits,  2002, 15–21.    [7]    J. Rowlette, T. Eiles,” International Test Conference 2003 Proceedings, 1,  2003, 264–273.    [8]    F. Beaudoin, K. Sanchez, et. al, Microelectronics Reliability, 47, 2007,  1517–1522.    [9]    A. Deyine, E. Doche, et. al, Microelectronics Reliability, 52, 2012, 2068– 2072.     [10]   P. H. P. Llamera, C. J. G. Garcia-Awitan and K. K. P. Domantay, "Soft  Defect Localization of Hot Failure by Dynamic Analysis by Laser  Stimulation using Hamamatsu iPhemos," 2018 IEEE International  Symposium on the Physical and Failure Analysis of Integrated Circuits  (IPFA), Singapore, 2018, pp. 1-5.    [11]   N. Hat, A. Sabate, et al., Proceedings of the 20th IEEE International  Symposium on the Physical and Failure Analysis of Integrated Circuits  (IPFA), 2013, 563–568.    [12]   R. Szabó, A. Gontean, et al., 2011 IEEE 12th International Symposium on  Computational Intelligence and Informatics (CINTI), 2011, 155–159.    [13]   A. Ahmad, M.K. Nordin, et al., 2017 IEEE 9th International Conference  on Engineering Education (ICEED), 2017, 206–211.

