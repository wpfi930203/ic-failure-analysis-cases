---
title: "192_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_72d4efa8908b5dc9202af20b3d9dc5877295230462135641
file_size: 4980263
---

## Fault localization of Cold-temperature Scan failures  by integrating Soft Defect Localization and ElectroOptical Probing  

Imran Arif Abdul Jamil 1 , Foo Loke Sheng 1 , Alwi Pawet 1 , Chew Jun Jie 1  ,Siow Cheng Liang 1 ,Tan Hui Hui 1 , Benjamin Lo Yuen Sum 2   1 Failure Analysis Lab, NXP Semiconductor Sdn. Bhd.,   Sungai Way Free Trade Industrial Zone, 47300 Petaling Jaya, Malaysia  2 Failure Analysis Lab, Taiwan NXP Semiconductor Co., Ltd, No.10, Jingwu Rd, Nanzih District, Kaohsiung City, Taiwan 811

Phone : (+60)182777067, Email:  imran.abduljamil_1@nxp.com

Abstract —Scan testing has been the main method for testing  in the semiconductor industry due to its extremely high test  coverage and high reliability in determining the suspected  region of failure. Scan test failures typically fail solidly across  voltage, frequency, and temperature. However, there are scan  failures that would only fail at cold temperatures and are  classified as temperature-dependent scan failures. ElectroOptical Probing (EOP) analysis is usually performed when the  part fails to observe abnormal transistor switching activity.  However, The main challenge behind cold temperature scan  failures is the inability to perform EOP at very cold  temperatures mainly due to tool limitations with conventional  tool setup. This paper will further discuss a new approach by  performing EOP at room temperature on three different types  of scan failures (Stuck-at, Time-delay, and Chain) that would  still yield tangible fault isolation results by referencing the Soft  Defect Localization (SDL) hotspot performed at cold  temperature.

Keywords—Scan, Soft Defect Localization (SDL), Cold, fault  isolation, Electro-Optical Probing (EOP)

## I.    I NTRODUCTION 

## A.   Scan Diagnosis Testing in Microelectronic Devices  

As time progresses, smaller technology nodes are being  developed in the microelectronic industry mainly due to their  increased performance in the overall system on chip (SOC).  However, the ever-decreasing size of technology nodes would  bring disadvantages, which are the cost increase in fabrication,  increased complexity in testing, lower yield during  fabrication, and increased difficulty in fault isolation. Due to  this, scan diagnosis is essential in ensuring successful fault  isolation for defective units [1-3].

![ScanIn#1  ScanOut#1  ScanIn#2  ScanOut#2  ScanIn#3  ScanOut#3  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/810b9bd9-5936-4273-9520-fcf713f295a0/810b9bd9-5936-4273-9520-fcf713f295a0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=05cef66139cc6185c62f29eb54959610fc56db31)
Fig. 1.   Block diagram of a scan chain architecture

Scan Test Insertion is carried out by replacing the  sequential state cells such as a flip-flop or a latch with scan  cells. The main difference between a scan cell and a flipflop/latch, is the ability to connect from one scan cell to the

next to create a chain of scan cells which are commonly called  scan chains visualized in Fig. 1. When scan chains are  connected in a chain, test vectors are able to be shifted into  each scan cells through the Scan Data In (SDI). With the  appropriate test vectors in place in each scan cell, there is a  pre-determined expected output at Scan Data Out (SDO) at the  end of the test [1]. Fig. 2 shows the typical scan cell  configuration, depending on the state of logic shift and logic  capture, the SI or D is chosen respectively, controlled by the  Scan Enable (SE) signal.

![Logic   Logic  Cloud   Cloud  Primany   Primay  Inputs   Outputs  CLK  scan  Patns  ObservationPoint  ControlPoint  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7d25ff1f-07c2-4a72-ae29-eb8d265aa3d7/7d25ff1f-07c2-4a72-ae29-eb8d265aa3d7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=b639d91ee16732434ffe08979e52db26ab99f437)
Fig. 2.   Scan chain schematic

There are several types of scan tests which are the Stuckat (SA) Transition-Delay (TD), and Chain type of scan pattern.  Depending on the pattern, the mechanism behind capturing  the test pattern response would be different. For TD scan  pattern, a launch and capture clock exists where the launch  clock is responsible for initiating the change in logic, creating  a 0-1 or 1-0 transition. Subsequently, the capture clock is  responsible in latching the logic launched by the launch clock.  Ultimately, TD scan patterns is sufficient to observe any slowto-rise or slow-to-fall type of faults within the scan path. For  SA, similar to TD, it possesses a capture clock but no launch  clocks, essentially testing whether a node is stuck at one logic  and does not test the speed in its transition. Finally, scan Chain  tests checks on the integrity of the scan chain itself by  verifying the scan in data is successfully shifted in and shifted  out of the DUT. Fig. 3 depicts a typical launch, capture and  shift cycle of SA, TD and Chain scan tests.

![ShiftIN   Capture   ShiftOUT  SACLK  TDCUK  ChainCLK  ScanEnable  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/46ff4da1-88ec-4051-990b-ffdf7eaf7d0b/46ff4da1-88ec-4051-990b-ffdf7eaf7d0b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=5d0642c8c02cf1575ab4c6ce043fc57e3fdefd0d)
Fig. 3.   Clock Timing Diagram for SA, TD and Chain Scan tests

By comparing the actual and expected result of the scan  test, the diagnostic tool can list down the possible defective  signals within the logic sea pictured in Fig. 4. Although the  suspect has been identified by the diagnostic tool, further  electrical fault isolation (EFA) is required to electrically  characterize the failure. In this paper, two major tools were  utilized the Soft Defect Localization (SDL) and ElectroOptical Probing (EOP).

![fail   tchtype   value  netpathnamelayout_status  100.   SIUCK   NTD Signal 1 INPUT_PIN_FAULT  100   STUCK   NTD Signal 2 INPUT_PIN_FAULT  #potential_open_segments=7l,#total_segments=84,   #potential_bridge_aggressors=0,#total_neighbors=  suspect  score fail_match pass_mismatch type   value location layout_layer critical_area  2.1   100   CELL   NTD Signal3  2.2   10O   OPEN   BS VIAO   1.38E-02  7.98E-04  1.93E-03  B4VIA0   1.38E-02  7.98E-04  VIA1   1.93E-03  5.64E-02  VIA2   1.29E-03  3   3.00E-02  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/96dc1b04-a4a0-47a2-9068-f224e6c8552d/96dc1b04-a4a0-47a2-9068-f224e6c8552d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=f33f729b778913a750fda05751819cd2892fcf9a)
Fig. 4.   Example of diagnostic suspects

## B.   Soft Defect Localization  

Soft defects are failures that are temperature, voltage, or  frequency dependent. For Soft defects, the DUT can be  configured so that the DUT is consistently failing and fault  isolation can proceed with conventional techniques.  However, by configuring the DUT to its critical state where  it passes and fails at the same rate, the Soft Defect  Localization (SDL) technique can be utilized for fault  localization purposes.

The SDL technique is a subset of Dynamic Analysis by  Laser Stimulation (DALS) that utilizes laser stimulation  where the silicon die is scanned using a laser while observing  the pass/fail status of the DUT. The laser scanning introduces  photoelectric/thermal effects through the heat generated by  the laser which alters the electrical properties of the DUT.  This would result in a change in the rate of the pass/fail when  the laser scans the defective site. The information would then  be mapped into a   $512\,\mathrm{~x~}\,512$  -pixel image frame where the  thermally sensitive area would be highlighted with a colored  pixel illustrated in Fig. 5.[6-8].

![Laserscan  Stimulus  DUT   Tester   Signal mappin  Pass/Fail Signal  Failure Location   Reaction to laser =failure location  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/911f2f2b-9495-48df-bfb5-50d8d034b114/911f2f2b-9495-48df-bfb5-50d8d034b114.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=1c1d5ff5068925076ac1dbdbafd56d160f0b4093)
Fig. 5.   Soft-Defect Localization working principle

In this paper, the SDL technique is a critical step in  isolating the fault. However, SDL alone is not enough to  isolate the failure as the anomalous spot revealed by SDL  may not be able to characterize which exact transistor is  failing if the spot size is too large, especially when the DUT  is of a smaller technology node. Hence, EOP analysis is a  critical step to further characterize the failure to proceed with  the appropriate plan for Physical Failing Analysis (PFA).

## C.   Electro-Optical Probing  

Electro-Optical Probing (EOP) analysis utilizes 1.3um or  1.064um laser radiated to the backside of a microelectronic  device whereby the reflected light would be measured to  observe transistor operation activity. EOP is a powerful tool  whereby the data interpretation is simple and logic failures are  easily identified. Therefore, EOP analysis is essential to  observe any type of stuck-at or transition delay faults [9,10].

EOP is currently an essential failure analysis technique  that may be utilized in conjunction with other failure analysis  techniques such as Soft Defect Localization (SDL), Optical  beam Induced Resistance Change (OBIRCH), and Photon  Emission Microscopy (PEM) [11].

## D.   Challenges in Cold Scan Failures  

Conventionally, EOP is carried out with continuous test  stimulation to the DUT where it would consistently fail  throughout the test in order to observe the anomalous  waveform during probing. With the integration of SDL  analysis, the conventional method of performing EOP would  surely make the fault isolation efforts for a defective part  quicker and increase the odds of finding the physical defect  during physical analysis [11].

However, for cold scan failures, the DUT would only fail  the scan test at cold temperature. Although SDL analysis can  be carried out by varying the temperature, most fault isolation  tools may have limitations when performing EOP at cold  temperatures as cooling the DUT may introduce unwanted  vibrations due to the cold air flowing through the DUT  without using a more sophisticated and expensive setup. The  micro-level vibrations may hinder the quality of the  acquisition of waveforms.

Although there are solutions currently in the market where  a mechanism could cool the DUT without  introducing severe  vibrations which enables EOP analysis, the tool may be  expensive and the frequency of cold failures may not be as  frequent to invest in an expensive tool. Hence, EOP analysis  can only be carried out at room temperature whereby the cold  scan failure would be passing with conventional tool setup.  This paper discusses the result of carrying out EOP analysis at  room temperature where the DUT would pass the scan test and  was still able to collect tangible fault isolation results that  would help in the PFA plan.

## II.   M ETHODOLOGY 

## A.   Proposed Flow  

In this paper, several case studies will be discussed where  the DUT was subjected to a proposed flow depicted in Fig. 6.  First, the scan failure would first be characterized to determine  the critical temperature where the test would start to fail as  well as to ensure the failure can be reproduced reliably. The  scanning diagnostic would then need to be ascertained and the  suspects' call-outs need to be of good quality (high-scoring  suspects, minimal amount of suspects, suspects that are  interconnected with each other). If needed, the sample would  then go through necessary sample preparation prior to SDL  analysis at cold temperature. The SDL analysis at cold  temperature is a critical step in the analysis as the subsequent  EOP analysis will be carried out about the SDL result. Lastly,  EOP analysis at room temperature would then be carried out.  At the end of the EOP analysis with sufficient circuitry study,  sufficient EFA information would meet the criteria for a  successful PFA plan.

## B.   Cold SDL Configuration  

The cold SDL configuration utilizes a temperature-forcing  system that delivers clean dry air of varying temperatures. In  this paper,   $-40^{\circ}\mathrm{C}$   of clean dry air was blown onto the unit  gradually. A piece of hard plastic cover was used to enclose  the cool air and an air hose was directed towards the die  backside. By connecting a thermocouple to the temperature  forcing system, the surrounding temperature of the DUT can  be controlled to a desired temperature consistently. The clean  dry air was able to flow into the enclosure with the air hose  from the side opening of the enclosure depicted in Fig. 7.

As the cool dry air is blown onto the backside of the die,  the setup was then brought under the Hamamatsu lens to  facilitate SDL analysis depicted in Fig. 8. During the cooling  process, low air pressure was used to minimize the amount of  vibration which may hinder the image acquisition of  Hamamatsu during LSM (Laser Scanning Microscopy).

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ac645778-9913-41e4-aad2-9848dd615365/ac645778-9913-41e4-aad2-9848dd615365.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=1c29aedefd569f8bd101b768ba3f528ae9d1305c)
Fig. 7.   Air hose routed to aim towards the backside of the die

![Start  Failure characterization  Scan Diagnostic   Sample Preperation  SDL at critical temperature   EOP at room temperature  EFA End  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3fb49c4a-5d0f-4c3d-b2a9-ffbde38b2ddf/3fb49c4a-5d0f-4c3d-b2a9-ffbde38b2ddf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=31790462c1980b6095a3cb5c3153f4e7f17fbfe2)
Fig. 6.   Proposed workflow for cold-temp scan cases

## III.   C ASE  S TUDY 

## A.   Case Study 1  

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/71cba26d-5ddc-4980-9816-4b405f1f6e79/71cba26d-5ddc-4980-9816-4b405f1f6e79.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=ee5aa9a60682f3faba695b81301d0787b91d88b9)
Fig. 8.   Cool air able to flow to the DUT backside while performing SDL  analysis

The first case study would be on a 16nm technology device  that failed the time transition scan test starting at   $-30^{\circ}\mathrm{C}$  . The  failure was further characterized by shmoo analysis and  revealed the pass/fail boundary in Fig. 9 which will be used as  the test point during SDL analysis. Scan diagnostic was  performed and revealed 5 signal suspects of 100 score that are  interconnected with each other in Fig. 10. One of the suspects  is also one of the inputs to a scan cell that can be used to probe  with EOP later on.

![1v  -30°C 0.96V 0.92V PassRegion 0.88V Test 0.84v d0.8V 0.76V 0.72V 0.68v 0.64V 0.6v 90n82n74n66n58n50n42n34n26n18n10 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/96e314c0-da1b-45a5-88fc-8851976b001d/96e314c0-da1b-45a5-88fc-8851976b001d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=7e9d8c6eb1a0f49357cd6cca3bd122f8474b9052)
Fig. 9.   Shmoo plot at  $-30^{\circ}\mathrm{C}$   revealed pass/fail boundary

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e37c8028-a596-44c5-bc39-b7c45c732381/e37c8028-a596-44c5-bc39-b7c45c732381.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=897e04f8f663dd687b7ec46269ab4033a54179f7)
Fig. 10.   Several diagnostic suspects are interconnected with one another.

SDL analysis was performed at the designated test point while  cooling the unit to   $-30^{\circ}\mathrm{C}$   and one SDL spot was identified  depicted in Fig. 11. Further overlay study revealed the SDL  spot coincide with the scan diagnostic suspect and located at  the driver of net 1398.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3a0ee06d-3918-4492-8572-c8eef1d7c000/3a0ee06d-3918-4492-8572-c8eef1d7c000.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=ce9be5cf79dde3f6bdb783deecd37246814f4fd3)
Fig. 11.   SDL spot located at the driver of one of the diagnostic suspect

The unit was then heated to room temperature to facilitate  EOP analysis. Several waveforms were collected along the  suspects and observed time delay characteristics. Probing  results in Fig. 12 revealed there was a 800ps delay between  Probe locations 1 and 2 and the delay was then propagated to  Probe 3 and 4. Probe 5 which is the output of the scan cell was  able to shift out the correct logic and no gross anomaly was  observed as expected as the scan test was at passing condition.

![63.0H  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8bec312c-8831-40ce-ac8f-ae72997aab51/8bec312c-8831-40ce-ac8f-ae72997aab51.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=367218027177fa4ddcaf7c9acc22b88d97ad6e29)
Fig. 12.   EOP analysis revealed a marginal delay observed between probe 1  and probe 2

At this juncture, it was suspected that the delay was marginal  during room temperature where the scan test would not fail.  However, at  $-40^{\circ}\mathrm{C}$   where the scan test was failing, the delay  would have been worsened and managed to fail the scan test  whereby the incorrect logic was captured during the capture  clock. Further probing was then performed to characterize the  delay to isolate the region of failure further in Fig. 13. The  driver of the inverter where the SDL was located was probed  and the fall/rise time between Probe 6 and Probe 1 revealed an

anomalous slow rise exhibited by the inverter at probe  Circuitry study would then reveal a potential resistive open  path or a defective PMOS transistor that explains the slow rise  exhibited visualized in Fig. 14.

![SDLSpot  Fan  Risex  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c08fdd3f-a326-4aed-9616-1aaf568bc112/c08fdd3f-a326-4aed-9616-1aaf568bc112.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=5610cae430433ea9c658f7a08c38c8f6a5accc7d)
Fig. 13.   Slower rise time and normal fall time observed

![vdd   wdd  Fal  Wss   Wss  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/662daf6f-45fa-4f25-a33f-ee10fef0d650/662daf6f-45fa-4f25-a33f-ee10fef0d650.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=63c46bf4cb262d06d1956e3e7eda6f8971862651)
Fig. 14.   Suspected PMOS that caused the slow fall time

Further physical analysis which includes nanoprobing (Fig.  15) and cross-section TEM would then reveal a resistive via  that connects the source of the PMOS transistor to the VDD  with a higher concentration of cobalt between the via and  metal interface in Fig. 16. The resistive path from the source  to VDD would explain the slow rise exhibited at the output of  the inverter.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d7605ef1-4a1c-4e95-9efa-2534f224c6ac/d7605ef1-4a1c-4e95-9efa-2534f224c6ac.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=9a0751eccdaad648e6f0ffe096fd4efc016b8ba6)
Fig. 15.   Nanoprobing IdVg analysis revealed a lower current draw when the  PMOS transistor is ON.

![Referenc  Reference  dd-   vdd-BadRi  oodFal  wss  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a6e31794-cd5b-40ab-8c28-1f5269b807d6/a6e31794-cd5b-40ab-8c28-1f5269b807d6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=6685279afa0c2b968760b395cba648ad64e40bee)
Fig. 16.   Resistive Open towards VDD power rail that caused the slow rise

## B.   Case Study 2   

The second case study would be on a 16nm technology device  that failed the stuck-at-scan test at    $-40^{\circ}\mathrm{C}$  . Shmoo  characterization revealed a pass/fail boundary in Fig. 17. The  test point was then set at the boundary to facilitate SDL  analysis. Diagnostic results of the scan test revealed 1 signal  suspect with a 100 score. This net was then revealed to be the  reset signal of several scan cells based on Fig. 18.

![0.796V  0.776V  0.756V-0.737V  0.717V  d0.698V  0.678v  0.658V-0.639V  0.619V  0.6  147.2n   119.76n   92.32n 78.6n 64.88n51.16n37.44n23.72n10n  freg  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cce5a8f8-8704-45ab-959b-c38eb6049fb1/cce5a8f8-8704-45ab-959b-c38eb6049fb1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=2448b4d596d473237a3ec9ccaacd95fe3aecd111)
Fig. 17.   Shmoo plot at  $-40^{\circ}\mathrm{C}$   revealed pass/fail boundary

![  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/870c73b6-ce54-49c2-b51a-4909899975b8/870c73b6-ce54-49c2-b51a-4909899975b8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=ddf2bfa1e74411e9c77f548bf9e1fcb6e5266cf2)
Fig. 18.   One diagnostic suspect revealed to be the reset signal of the scan cell

SDL analysis was performed at the critical test point where the  unit is passing/failing at a  $50\%$   rate at   $-40^{\circ}\mathrm{C}$   and revealed one  anomalous spot at one of the fan outs of the signal suspect  which was located at a scan cell visualized in Fig. 19.

![SDLSpot    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/79e8ea2b-4a12-421a-b44f-4d6f989114d3/79e8ea2b-4a12-421a-b44f-4d6f989114d3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=eedfa49016acff801cdb7a9c2389ec0c689e1f17)
Fig. 19.   SDL spot located at one of the fan outs of the diagnostic suspect

The unit was then re-heated to room temp for EOP analysis.  The input and output signals of the scan cell were collected for  both the failing unit and a correlation unit. It was noted that  the output of the scan cell exhibited a delay of 24 ns when  compared to the good unit illustrated in Fig. 20.

![SDLSpot    Bad_Probe 1  GoodPro  Delay  B-A=24.125nS  Bad_Pr  Good_Probe2    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/16dee0d0-e64b-4ff0-9f0d-c2cfeda5bc97/16dee0d0-e64b-4ff0-9f0d-c2cfeda5bc97.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=26639869fced9432380b9c872e138c9e76664cec)
Fig. 20.   EOP analysis observed delay between probe 2 and probe 1

The circuitry study in Fig. 21 of the scan cell revealed that the  reset signal was responsible for forcing a logic 0 at the output  of the scan cell regardless of the other inputs.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/aa7c0707-47f0-4650-af86-ca182eebecde/aa7c0707-47f0-4650-af86-ca182eebecde.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=dfeaf8838307fd7e70f06b911390fe692de14adc)
Fig. 21.   Scan cell study revealed reset signal would force a change of logic  to the output.

It was then hypothesized that at room temp, as long as the  logic was able to toggle to the correct logic, the scan-test  would pass although a delay was observed. Therefore, it was  suspected there was a resistive open to the gate of the reset  signal whereby at cold temperature the open would be more  gross which could cause the output would not toggle to the  correct logic. This may explain why the stuck-at scan test  would fail at   $-40^{\circ}\mathrm{C}$  . Further probing was performed for other  scan cells that share the same reset signal and revealed the  other scan cells observed no delay at their respective outputs  visualized in Fig. 22.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8f07a595-84ee-4ed2-af44-3760730a7b8d/8f07a595-84ee-4ed2-af44-3760730a7b8d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=6bcd5ffb608c1be9812021521406136b980d1de2)
Fig. 22.   Probing revealed only the suspected scan cell experienced the delay  in its output.

Based on the EOP analysis, sufficient electrical fault isolation  data was collected and isolated to only one fan out of the reset  signal. Due to similar symptoms exhibited by this case study  to the previous one, no physical analysis was pursued for this  unit.

## C.   Case Study 3  

The last case study would be on another 16nm technology  device that failed the scan chain test at  $-40^{\circ}\mathrm{C}$  . Shmoo analysis  revealed a pass/fail boundary in Fig. 23 that will be used as  the test point during SDL analysis. A scan diagnostic was  performed on the failing scan chain pattern and revealed one  faulty chain in Fig. 24.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ffff0dc8-484d-4cee-8127-ff5cd5e9cf63/ffff0dc8-484d-4cee-8127-ff5cd5e9cf63.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=dc3e30c48deb9b451ffd12b196aa0521bcb4e57c)
Fig. 23.   Shmoo plot at   $-40^{\circ}\mathrm{C}$   revealed pass/fail boundary

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b4acaaa6-0db1-4173-9cc0-d694ff850ea7/b4acaaa6-0db1-4173-9cc0-d694ff850ea7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=6c8561c4ee23d0fc2b2023ba7cfaa789f2b7af45)
Fig. 24.   Scan chain diagnostic revealed one failing scan chain where  several scan cells and their scan paths highlighted

SDL analysis was performed at designated test point at   $-40^{\circ}\mathrm{C}$    and one SDL spot was identified overlaying the SDL image to  die layout revealed the spot coincided with a scan module  within the failing scan chain in Fig. 25.  Further circuit study  revealed scan modules consists of 4 scan cells in series  pictured in Fig. 26. It was noted that these scan cells share  several signals such as Scan Enable (SE), Reset (R) and Clock  while having separate functional logical inputs (D).

![  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ed67f5cd-409f-4dc4-a320-a3bbebb51b70/ed67f5cd-409f-4dc4-a320-a3bbebb51b70.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=d53c6886cc9c34358d741115d965178c9f53de0c)
Fig. 25.   SDL spot located at one of the scan modules within the failing scan  chain

![Scanmodule    Functional Logic  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5911fc84-5b87-41e9-8d58-17dd48dac6f1/5911fc84-5b87-41e9-8d58-17dd48dac6f1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=a1664dd3c7128258b413f82b5c816727b95ea61f)
Fig. 26.   SDL spot located within one scan module (in red) which comprises  4 scan cells

The unit was then heated to room temperature for subsequent  EOP analysis. As scan chain failures do not utilize the  functional logical input (D input) of a scan cell, several  waveforms were collected primarily at the Q output and the  Scan Input (SI) of the scan cells and observed time delay  characteristic for the SI signal (Probe 2) of the suspected  major scan cell. The time delay was a slow rise/fall time at  approximately 7.625ns in Fig. 27. As the DUT is currently at  a passing state, it was expected that the subsequent Q (Probe  3 & 4) observed shifted logic by 1 clock cycle correctly.

![Functional Logic  645.25ns   53ns  Shift_Clock  15.0uV/div  15.0uV/div  10.0μv/d  Probe3  40.0μV/div  Probe  40.0μV/div     ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9dd6e41d-cb35-4cd2-8ab1-944fd60a0223/9dd6e41d-cb35-4cd2-8ab1-944fd60a0223.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=759033f4e593d0ef9c6c6374e9ba1a67f962ac7e)
Fig. 27.   Slow rise/fall observed at the SI input (Probe 2) of the scan cell with  correct logic shifted at the subsequent output (Probe 3 & 4)

Similar to previous case studies, it can be hypothesized  that the delay observed would have been worse at  $-40^{\circ}\mathrm{C}$  . The  delay would eventually lead to the wrong logic being shifted  into the scan cell through SI ultimately leading to the scan  chain failure. Further probing was performed for the other  fanouts of the SI signal and observed no such delay for the  other fan outs in Fig. 28. Based on all the EOP data collected,  it was highly suspected there is a resistive open towards the  gate of the failing SI signal of the scan cell visualized in Fig.  29.

![SDLSpot  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1920e8ae-38d8-40cb-bbe4-2794cc67aab1/1920e8ae-38d8-40cb-bbe4-2794cc67aab1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=b3a7327f8c9d7f806f13b5f27ea67cb43762e0c5)
Fig. 28.   Further probing revealed only the suspected SI fan-out experienced  the slow rise/fall characteristic.

![Functional Logic  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3826d0a1-1e8d-46cf-b337-b5c228c23ee6/3826d0a1-1e8d-46cf-b337-b5c228c23ee6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=10c29d11aaf833f76f0813dabc8f73d1063d356b)
Fig. 29.   Suspected resistive open towards the gate of the SI input

Subsequent physical failure analysis would then reveal a  resistive via of the failing SI signal in Fig. 30 which would  make the signal open towards the gate whereby the resistive  path would explain the slow rise/fall characteristic during  probing.

![Reference  20nm   20.n  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8dd0faf8-8291-4eb4-adcb-1b1e9a11357f/8dd0faf8-8291-4eb4-adcb-1b1e9a11357f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215885%3B1743219485&q-key-time=1743215885%3B1743219485&q-header-list=host&q-url-param-list=&q-signature=3557ffd02b9f0165d3b4db0b5f1ce648242c77a2)
Fig. 30.   Resistive interface between Via1 and M1 that caused the slow  rise/fall SI signal

## C ONCLUSION 

With the integration of SDL analysis at cold temperature  and EOP analysis in the room, although the DUT is passing,  minor delays can still be observed. With the electrical fault  isolation efforts collected at room temp, hypotheses were able  to be made on how the unit would have failed at cold  temperatures. However, this can only be confirmed with an  advanced tool setup where the unit is properly cooled so it  would fail and EOP would be carried out at this state. By  characterizing the delay sufficiently, sufficient electrical fault  isolation data was enough to proceed with physical fault  isolation and would have revealed the physical defect.

## A CKNOWLEDGMENT 

The author would like to acknowledge the Physical Failure  Analysis team which includes Mugilan Ganesan, Au Yin Fun,  Siow Cheng Liang, and Benjamin Lo mainly for their fault  isolation efforts including Nanoprobing, FIB cross-sectioning,  and TEM analysis. Additionally, special thanks to the Failure  analysis Technicians which are Yasser, Izam, Faizol,  Mahassan, Rusdi, and Hafiz who prepared the sample for EFA  and PFA. This paper could not have been written without their  tremendous help. Lastly, the author would like to appreciate  his wife, Iwana for moral support throughout the writing of  this paper.

## R EFERENCES 

[1]    Z. G. Song, S. P. Neo, T. Tun, C. K. Oh, and K. F. Lo, "Diagnosis and  failure analysis for scan failure," Proceedings of the 12th International  Symposium on the Physical and Failure Analysis of Integrated Circuits,  2005.   IPFA   2005.,   Singapore,   2005,   pp.   181-184,   doi:  10.1109/IPFA.2005.1469157.    [2]    S. J. Moon, D. Nagalingam, Y. T. Ngow, and A. C. T. Quah,  “Combining Enhanced Diagnostic-Driven Analysis Scheme and Static  Near Infrared Photon Emission Microscopy for Effective Scan Failure  Debug,” in  2022 IEEE International Symposium on the Physical and  Failure Analysis of Integrated Circuits (IPFA) , Singapore, Singapore:  IEEE, Jul. 2022, pp. 1–6. doi:  10.1109/IPFA55383.2022.9915727 .    [3]    E.B. Eichelberger and T. W. Williams, “A Logic Design Structure for  Testability”, Proceedings, DAC, P. 462-468 (1977).    [4]    Anysilicon, “How to optimize IC test time,” AnySilicon,  https://anysilicon.com/how-to-optimize-ic-test-time/ (accessed Dec.  29, 2023).     [5]    S. Sherma, “Scan Chains: PNR Outlook,” Design And Reuse,  https://www.design-reuse.com/articles/48331/scan-chains-pnroutlook.html     [6]    M.R. Bruce, V.J. Bruce, D.H. Eppes, J. Wilcox, "Soft defect  localization on ICs," ISTFA 2002, p. 21-2    [7]    V.K. Ravikumar; S.L. Phoa; V. Narang; J.M. Chin, “Understanding  Soft Defect Localization set-points for reducing cause-not-founds in  integrated circuits”, IPFA, 2008    [8]    Hamamtsu Photonics, “Phemos 1000 emission microscope”,  https://www.hamamatsu.com/resources/pdf/sys/SSMS0003E_PHEM  OS1000.pdf.    [9]    H. Zhang, P. Tian, X. Qian, and W. Wang, “Electro optical probing /  frequency mapping (EOP/EOFM) application in failure isolation of  advanced analogue devices,” in  2017 IEEE 24th International  Symposium on the Physical and Failure Analysis of Integrated Circuits  (IPFA) , Chengdu, China: IEEE, Jul. 2017, pp. 1–5. doi:  10.1109/IPFA.2017.8060131 .    [10]   Damrong Korbsrisawat, Foo Loke Sheng, “Signal toggling in  EOFM/EOP application as a novel bulk localization technique for  analog devices failure localization”, IPFA 2017.    [11]   F. L. Sheng, C. Thin Wei, T. L. Teng, L. Chik Hooi, and A. Pawet,  “Integration of Soft Defect Localization (SDL) and Electro-Optical  Probing (EOP) in Root Cause Investigation for Time Delay Related  Issue,” in  2023 IEEE International Symposium on the Physical and  Failure Analysis of Integrated Circuits (IPFA) , Pulau Pinang,  Malaysia:   IEEE,   Jul.   2023,   pp.   1–6.   doi:  10.1109/IPFA58228.2023.10249051

