---
title: "253_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_4032640a5a3e8fae2b965bf12840e2167295230462135641
file_size: 868945
---

## Soft Defect Localization (SDL) of Temperature  Dependent Failure using NI-PXI Test Platform in  DALS System   

Jed Paolo Deligente   Failure Analysis Department, Maxim Integrated, Gateway Business Park, Javalera, General Trias, Cavite, Philippines  \* Phone: +63-902-2000 local 2766   Email: jed.deligente@maximintegrated.com

Abstract-   Temperature dependent failures have always presented  challenges in failure analysis of advanced mixed signal integrated  circuits. Soft defect localization (SDL) has been proven a reliable  fault isolation technique however, reliable capture of pass/fail  signal conditions, temperature characterization and laser  synchronization are vital in having an effective SDL result. This  paper presents a case study which demonstrates how NI-PXI  system was utilized as a test and synchronization platform with  DALS module of Hamamatsu iPHEMOS.

Keywords  –  Failure Analysis, Soft Defect Localization, SDL,  DALS, PXI

## I. I NTRODUCTION 

Vast improvements in semiconductor process technology has  created faster and smaller integrated circuit devices. The result  of smaller geometries is an increased occurrence of soft defects,  which often impose challenges during failure analysis. Devices  with soft defects often exhibit intermittent or marginal failure  symptoms depending on certain test conditions like temperature  and length of operation. [1, 2]

The Soft Defect Localization (SDL) technique was  developed to quickly locate soft defects in integrated circuits  [2]. SDL is categorized under Dynamic Analysis by Laser  Stimulation (DALS) which evaluates functional pass/fail status  of the DUT under 1.3 um laser stimulation [3]. SDL is often  done using an LSI tester or ATE test equipment to evaluate  functional pass/fail condition [1, 4]. Recent studies have also  shown different techniques using discrete equipment like  oscilloscopes and functional generators to evaluate a pass/fail  signal and create synchronization to the laser system [3, 5 – 8].

In this study, a PXI (Pci eXtension for Instruments) system  developed by National Instruments (NI) was used as test  platform [9]. The NI-PXI platform together with the developed  LabVIEW program [10], integrated different modular and  bench top instruments into a single test system. This created a  more customized and portable test platform and avoided the  need for complete ATE test system. The developed test  platform was used to characterize the failure mode of the unit  over-temperature. Then it was used to evaluate the pass/fail  condition of the DUT, create a trigger and test signal input to  the DALS module of the Hamamatsu iPHEMOS.

## II.   EXPERIMENTS   AND   METHODOLOGY  

In this case study, the device under test (DUT) failed ATE

test at room (25C) temperature while it passed at hot (125C)  temperature. Electrical verification at bench confirmed that the  DUT exhibited delayed VCC output turn-on upon power-up.  Fig. 1 and 2 shows the VCC output response of the DUT at  room and hot temperatures respectively.

![Iek Stop   NoiseFilterOif  5.00V  5.00”   5.00V   2.005   :3231  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5f88e11b-295c-4400-b9c3-4c13f6868f6c/5f88e11b-295c-4400-b9c3-4c13f6868f6c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215674%3B1743219274&q-key-time=1743215674%3B1743219274&q-header-list=host&q-url-param-list=&q-signature=05901c86d75c631117f7d66fdafc5c800dd396f2)
Fig. 1 Output Response of the DUT at Room Temperature

![Tekstop   NoiseFilterOff  ESYNC/EN  CC  10.0   5.00   5.00   5.00   2.00 s   400m   09:12:07  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/89266de9-b8ef-47f8-8455-51c51e92a158/89266de9-b8ef-47f8-8455-51c51e92a158.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215674%3B1743219274&q-key-time=1743215674%3B1743219274&q-header-list=host&q-url-param-list=&q-signature=8f096dc2e77dddbe71a002fe110548b9f6b04736)
Fig. 2 Output Response of the DUT at Hot Temperature

To better understand the DUT performance over  temperature, an automated test setup using LabVIEW program  and benchtop instruments was developed. The program  automated the monitoring of the VCC turn-on response while  the temperature was slowly increased from 20C to 100C. Fig.3  shows the software flow of the temperature automation test  setup and Fig. 4 shows the software GUI. The DUT started  exhibiting normal VCC turn-on response at around 65C as  shown in Fig. 5.

In order to capture the failing mode of the DUT and create a  pass/fail signal as input to the DALS system, a different  automated test setup using LabVIEW program and NI-PXI  platform, was developed. Fig. 6 shows the software flow of the  test setup and Fig. 7 shows the software GUI of the LabVIEW  program used in DALS.

![ Initialize   Go to Min   Turn on Power    Initialize  Supply  Temperature   Temperature    Smus and   Chamber    (In, syNC/en,   Multimeter  FB)  Soak    Measure  VcC  Set MIN and  Output   MAX Temp, Soak  Times and   Go to MAx  Number of Cycles   Temperature  LogVcC and  Temperature  Soak  cmpcrature  TurnOFF  Cycle.   Power   Supplies  NuTotar of   ND   TestLo  Temperature  Cyclesdone  YES  Close All   END  Equipment   PROGRAM  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f7c291ea-d439-4774-a7f3-1de353374230/f7c291ea-d439-4774-a7f3-1de353374230.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215674%3B1743219274&q-key-time=1743215674%3B1743219274&q-header-list=host&q-url-param-list=&q-signature=5f26036d6c634be5ba0de5580ad2d2b2a682a1f2)
Fig. 3 – Software Flow of Automated Temperature Cycle Test Setup

![TemperatureChamber  PowerSupplySettings  INSupply   Settings  EN and FB Supply   Set WatlowAddress   Meter  GPIBAddress   22.00  Loop Iteration  Multimiter Settings   0  VCCMultimeter   MinTe  Output File Settings   125  MinTemp Soak Time(s)   MaxTemp   Time（s)  Output File Header Info   360  Temperature   VCCVoltaqe  Sampling Time (s)  FileName   END of Temp Cycle  STOP  C:DoC   nith\Desktop   STOP  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1a46b0ee-1101-4b8f-8c6e-ce3a2f690fdd/1a46b0ee-1101-4b8f-8c6e-ce3a2f690fdd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215674%3B1743219274&q-key-time=1743215674%3B1743219274&q-header-list=host&q-url-param-list=&q-signature=d59a6d15cb6bfb59701f06ed9c9b6946dd6dc91a)
Fig. 4 – GUI of Automated Temperature Cycle Test Program

![VCCvs.Temperature  5_S  2S  1-5  OS  20253035404550556065707580859095100  Ternpealure(°C)  DUT  KGU  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/52a7f03a-db91-44fa-9496-1e1f7666a969/52a7f03a-db91-44fa-9496-1e1f7666a969.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215674%3B1743219274&q-key-time=1743215674%3B1743219274&q-header-list=host&q-url-param-list=&q-signature=b42a348aa7e76aede3432bf70f7e2f983ae0b4df)
Fig. 5 – VCC Measurement vs. Tempeature Result

![Send  InitializePower  PASS/FAIL   Supplies and  signal to  Multimeter  iPHEMOS  otal   YES  Number   CloseAll  SendEndof  Turn on Supply    Test Trigger   ofPnels   Equipment  ofDUT   Signal to  iPHEMOS  NO   ENDOF  CheckifvcC   Turn OFF   PROGRAM  Outputis   Power  High/Low   Supplies  Fig. 6 - Software Flow of LabVIEW Test Setup Integrated to DALS  Fig. 6 – Software Flow of LabVIEW Test Setup Integrated to DALS  ModuleofiPHEMOS  Module of iPHEMOS   IN VISA  6PxMSIotB   Loop Number  Channel Name   Voltage Level  12.0000  ENVISA  PxnSlot9   PF  Channe Name   Voltag= Level  Measurement  3.00000  0.00000  FB:NTSA  Px11Slot14  Channel Name   Voltage Level  5.00000  Loop Trigger VISA  PxnSlot12  Stop Button  Tester Signal VISA   Trigger Level  PxMSlot3   025  Number of Pixels   Stop  072000  Multimeter  PxnSlot_05  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a9b4ea48-60b1-4584-9620-d5d8b6174f5d/a9b4ea48-60b1-4584-9620-d5d8b6174f5d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215674%3B1743219274&q-key-time=1743215674%3B1743219274&q-header-list=host&q-url-param-list=&q-signature=6278dccb72a1cfe4ccc2dc9993d63fc854a9e554)
Fig. 7 – GUI of LabVIEW Test Setup Integrated to DALS Module of

iPHEMOS

For each loop of the test flow, the input power supplies to  the DUT will be turned ON. After 50ms, the VCC regulator  output of the DUT will be measured with multimeter of the  NI-PXI and a Pass/Fail trigger pulse will be sent to the DALS  system of the iPHEMOS. The input power supplies will be  turned off, which marks the end of one test loop. Each test flow  loop will correspond to one pixel in the laser scan area of the  DALS system. For a 256x256 pixel laser scan image resolution,  total number of test loop or pixels is approximately   ${>}65536$  .  72000 was used as the number of test loop to ensure all image  and header pixels will covered by the test. Fig. 8 shows the  overall block diagram of the DALS system developed with  NI-PXI platform, while Fig. 9 shows the NI-PXI platform  hardware configuration. Fig. 10 shows the sequence of the  power supplies and loop trigger signal from the NI-PXI system.

![IN,EN,   iPHEMOS  SMU  FB   Lasei  DUT  DNN   WCC  NI-PXI   DALS  SNU   Tester Signal  Pass/Fail  SMU   Loop Trigger  Fig. 8 - DALS System using NI-PXI Platform  Fig. 8 – DALS System using NI-PXI Platform  NATIONCAL  INSTRUMENTS  PXIIPXIPXI  PXIPXI  NPX0e-8125  Embedded   DMM   DUTPower   TestLoop  Controller   Supplies   SignalTrigger    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/42ee3e83-bef5-4323-b16a-2aa3a077f5a7/42ee3e83-bef5-4323-b16a-2aa3a077f5a7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215674%3B1743219274&q-key-time=1743215674%3B1743219274&q-header-list=host&q-url-param-list=&q-signature=0262ffb3177bbfce5652448ddde77e8649b05616)
Fig. 9 – NI-PXI Platform Module Configuration

![TekRun   Tigd   NoiseFilter Off  ESYNC/EN  LOOP_TRIG  [20.0ms   80.5200ms  1/400mV   19.9991 Hz  10.0   2  5.00   1Freq   19.86 Hz   1Period   50.35ms  5.00   5.00   1+Width   24.34ms   11:45:40  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3f4043b3-2ace-41b7-9c17-2974835b455f/3f4043b3-2ace-41b7-9c17-2974835b455f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215674%3B1743219274&q-key-time=1743215674%3B1743219274&q-header-list=host&q-url-param-list=&q-signature=c7c1a8759a214dc7bfab0d3e45f1208402655ccb)
Fig. 10 – NI-PXI Output Signal Sequence

## III. R ESULTS AND DISCUSSION   

In preparation for the fault isolation using DALS, the  backside of the DUT was exposed. The DUT was scanned  pixel-by-pixel with 1.3um laser using the NI-PXI synchronized  DALS system. Laser power was set to   $30\%$  , which was enough  to stimulate pass/fail transition of the DUT. The laser scan  image resolution was set to   $128\mathbf{x}128$   to acquire the fastest scan  time with the most accurate results. The acquired DALS laser  scan result was superimposed to the laser image and the  temperature sensitive locations was determined.

Two distinct temperature sensitive locations were identified  on the unit. Increasing the laser image resolution to   $256x256$    and slowing the scan time produced a cleaner DALS image at  100X magnification. Fig. 11 shows the DALS superimposed

![20x  100X  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/35338c03-9177-48ee-b964-8681db4ef222/35338c03-9177-48ee-b964-8681db4ef222.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215674%3B1743219274&q-key-time=1743215674%3B1743219274&q-header-list=host&q-url-param-list=&q-signature=513450bd419e2372b981e48dc76bce6f54b67a53)
Fig. 11 – Superimposed DALS Image Result

In-circuit I/V curve probing was done on the circuit of  DALS temperature sensitive areas. Resistive short I/V curve  response, as shown in Fig. 12, was observed on the gate of one  of the MOSFETs with respect to the IN positive supply rail of  the circuit.

![1-V 5OUA Reject Good SOuA 12N  400 mV/div. ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/995597b4-0f31-43e8-8fde-905ad6996579/995597b4-0f31-43e8-8fde-905ad6996579.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215674%3B1743219274&q-key-time=1743215674%3B1743219274&q-header-list=host&q-url-param-list=&q-signature=73747bc6f0b775af9bd9b39141d7c506ac52d4f7)
F ig. 12 – I/V Curve Test at Gate of Temperature Sensitive MOSFET

Further fault isolation was done on the affected circuit block  using Optical Beam Induced Resistance Change (OBIRCH) by  biasing the resistive nodes. Fig. 13 shows distinct OBIRCH  spot observed on capacitor connected to IN supply rail and gate  of MOSFET.

Physical failure analysis was performed. Cross-section  using Focused-Ion Beam (FIB) was done on the capacitor. Fig.  14 shows particle defect and oxide dielectric breakdown  between the plates of the capacitor.

![DALSSpot  OBIRCHSpO  20X   100X  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a9d340cb-56a5-47f0-b0c2-8144d2fbdaec/a9d340cb-56a5-47f0-b0c2-8144d2fbdaec.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215674%3B1743219274&q-key-time=1743215674%3B1743219274&q-header-list=host&q-url-param-list=&q-signature=a295c9aa45a74dc31cd5239e02978fccfce6c04e)
Fig. 13 – Superimposed OBIRCH Image Result

![SEM Image  Particle  Defect  Oxide  Breakdown  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/53a4a5ab-3041-4549-b9f6-ad973045cb25/53a4a5ab-3041-4549-b9f6-ad973045cb25.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215674%3B1743219274&q-key-time=1743215674%3B1743219274&q-header-list=host&q-url-param-list=&q-signature=f52d8c6b49943443116756ceef258e9fdc610fff)
Fig. 14 – SEM Image after FIB cross-section on the Capacitor

Fig. 15 shows that the observed defective capacitor is directly  connected to one of the temperature sensitive transistors from  the DALS fault isolation. The resistive short signature of the  failing capacitor to the positive supply rail implies that the gate  voltage of the PMOS is higher than normal. This resulted to the  source to gate voltage (V SG ) to be lower and the PMOS will not  be functional. When temperature is increased by laser  stimulation from the DALS system, the threshold voltage  $\mathrm{(V_{TH})}$    of the sensitive PMOS will be lower. The lower  $\mathrm{V}_{\mathrm{TH}}$   will enable  the PMOS to turn-on and the circuit will exhibit normal  function.

![Defective  Capacitor  DVCC  Temperature  sensitive areas    Fig. 15 - Schematic showing defective capacitor and DALS  Fig. 15 – Schematic showing defective capacitor and DALS  temperature sensitive transistors  temperature sensitive transistors     ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5b700440-01aa-4d0f-8863-4c0af35d0afe/5b700440-01aa-4d0f-8863-4c0af35d0afe.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215674%3B1743219274&q-key-time=1743215674%3B1743219274&q-header-list=host&q-url-param-list=&q-signature=348f42402da42630784909e6e38e6ffe99e525ce)
## IV. C ONCLUSION 

This failure analysis case study presented challenges in fault  localization of failures exhibiting sensitivity in temperature and  length of operation. The NI-PXI test platform was effective in

characterizing the failure mode of the DUT over temperature  and synchronize its test sequence with laser scan of the DALS  system. The developed SDL test system together with in-circuit  fault isolation was proven successful in localization of the  failure and the identification of the temperature dependent  failure mechanism.

## A CKNOWLEDGMENT 

The author would like to thank Maxim Integrated Philippines  Failure Analysis FIB team for preforming circuit edit and  cross-section, Cinzia Cicchilliti for design engineering support  and Camille Garcia for guidance in the failure analysis flow.  The author would also like to thank Jerome Escobedo and  Zhiyong Wang for their support in this failure analysis case.

## R EFERENCES 

[1]    V. K. Ravikumar, S. L. Phoa, V. Narang and J. M. Chin, "Understanding  Soft Defect Localization set-points for reducing cause-not-founds in  integrated circuits,"  2008 15th International Symposium on the Physical  and Failure Analysis of Integrated Circuits , Singapore, 2008, pp. 1-4.    [2]    M. Bruce V. Bruce D. Eppes J. Wilcox E. Cole P. Tangyuanyong C.  Hawkins "Soft Defect Localization (SDL) on ICs". Proc.28 International  Symposium for Testing &amp; Failure Analysis 2002 pp. 21-27     [3]    C. He, D. Fan and G. Song, "SDL analysis in temperature sensitive  failure based on DALS system," 2017 IEEE 24th International  Symposium on the Physical and Failure Analysis of Integrated Circuits  (IPFA), Chengdu, 2017, pp. 1-4.    [4]    A. Deyine et al., "Full Dynamic Laser simulation set up," 2009 16th  IEEE International Symposium on the Physical and Failure Analysis of  Integrated Circuits, Suzhou, Jiangsu, 2009, pp. 213-217    [5]    C. Wu et al., "A novel and low-cost method to detect delay variation by  dynamic thermal laser stimulation," 2011 International Reliability  Physics Symposium, Monterey, CA, 2011, pp. FA.1.1-FA.1.5    [6]    G. Wen  et.al , "SDL(Soft Defect Location) technical in analysing the  laser beam wavelength and temperature sensitive failures in VLSI  failure analysis,"  2015 IEEE 22nd International Symposium on the  Physical and Failure Analysis of Integrated Circuits , Hsinchu, 2015, pp.  223-226.    [7]    Jinglong Li and Chunlei Wu, "Soft Defect Localization (SDL) applied  on analog and mixed-mode ICs failure analysis,"  2012 IEEE  International Reliability Physics Symposium (IRPS) , Anaheim, CA,  2012, pp. FA.6.1-FA.6.5.    [8]    P. H. P. Llamcra, C. J. G. Garcia-Awitan and K. K. P. Domantay, "Soft  Defect Localization of Hot Failure by Dynamic Analysis by Laser  Stimulation using Hamamatsu iPhemos," 2018 IEEE International  Symposium on the Physical and Failure Analysis of Integrated Circuits  (IPFA), Singapore, 2018, pp. 1-5.    [9]    L. Gutterman, "PXI: the future of test," Proceedings, IEEE  AUTOTESTCON, Huntsville, AL, USA, 2002, pp. 205-214.    [10]    "LabVIEW Professional Development System ver", 2012 National  Instruments Corporation.

