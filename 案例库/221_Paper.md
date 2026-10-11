---
title: "221_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_a4e112a197db0e30da2f29770eaeb3fd7295230462135641
file_size: 763440
---

## SELECTIVE MECHANICAL BACKSIDE  GRINDING OF CSP-BGA AND SOIC-CAV  DEVICES IN PREPARATION FOR BACKSIDE  FAILURE ANALYSIS  

Melissa Caseria, Dennis Madrinan    1 Global Failure Analysis, Analog Devices Inc., Gateway Business Park, Javalera, Gen. Trias, Cavite, 4107, Philippines    2 Global Failure Analysis, Analog Devices Inc., Gateway Business Park, Javalera, Gen. Trias, Cavite, 4107, Philippines  \* Phone: +63-2-867 7030 Email: melissa.caseria@analog.com, dennis.madrinan@analog.com

Abstract-   Failure Analysis is the process of determining the cause  of failure, collecting and analyzing data, and developing  conclusions to eliminate the failure mechanism causing specific  device or system failure. 1    Semiconductor failure analysis initially  involves pinpointing the nature of the failure. The initial phase of  semiconductor failure analysis calls for the failure verification in  which the failure is identified and categorized. The next phase of  analysis seeks to localize the exact origin and causes of the failure.  To localize the exact origin and causes of the failure, the device  will be subjected to various forms of failure analysis, some  non-destructive, and others destructive.  As one of the failure  analysis rules, all possible non-destructive analyses should be  performed first before the destructive analyses.  Moving on to the  destructive FA techniques can render the device not suitable for  further electrical analysis.   This paper proposes a selective  backside mechanical grinding on a previously opened device  without damaging solder bumps and electrical connections linked  to the electrical fault and mechanical grinding of a device with  sensitive package constructions (sensors, beams) for a successful  backside fault isolation and further electrical analysis.

## I. I NTRODUCTION 

Failure analysis and characterization are relatively simple at the  wafer and die level where chip access is straightforward.  However, analysis and characterization of packaged parts or  components encapsulated with covers, caps, etc. may be more  cumbersome and lead to problems in assessing the root cause of  failure.

Backside fault isolation is a method to get optimum  transmission and a localized failure site. Fault site isolation is  the step in which various techniques are employed to localize  the defect area on the failed die. It is the most critical step in the  failure analysis process because it greatly reduces the area  required for failure analysis.  Topside fault isolation sometimes  may lead to inaccuracy in determining the failure mechanism  site. The reason is that the emission site can be underneath a  wire or the emission is blocked by thicker metallization and is  causing an inaccurate emission spot. As an example, after  decapsulation, an emission was seen underneath a wire.  However, if the failing device recovered after removing the  wire, then it is difficult to identify the emission site since the  wire was already removed.

For a CSP-BGA (Chip Scale Package - Ball Grid Array)  decapsulated device, performing backside isolation will subject  the die and the wires to damage, including the solder bumps  where backside grinding will be performed.  Further electrical  analysis will not be possible.

For an SOIC_CAV (Small Outline Integrated Circuit in Cavity)  device with sensors, performing backside grinding in  preparation for backside fault isolation can damage device  construction (that involves mechanically sensitive parts like  sensors), rendering it again unsuitable for further electrical  analysis.

## PROJECT DESCRIPTION  

For the CSP-BGA device, the device had been decapsulated for  die surface inspection. Doing backside fault isolation will  damage the die and wires during device mounting and will  damage the solder bumps during backside grinding.  The  opened area during decapsulation will be covered with a  thermoplastic cement to protect the die and wires during  mounting and mechanical grinding.  Analysis of the  connections will enable the analyst to choose an area where  connections will still be intact after mechanical grinding and  thus can render the device for a further electrical analysis.

For the SOIC_CAV device, to prevent damage on the sensitive  parts of the device, mechanical grinding will be done using the  slowest Analog Selected Area Preparation system (ASAP)  settings.  Further polishing of the backside of die cannot be  done since only the gel coat supports the die and wires.  A  partial chemical etching involving nitric acid will be done to  soften the die attach material.  Manual removal with plastic  tweezer will be done to totally remove the die attach.  Electrical  tests will then be done to check the device post backside  grinding if the device still exhibits the same responses prior to  mechanical grinding.

There are three (3) CSP-BGA units that came from the third  batch of burn-in evaluation units.   SN1, endorsed with a failed  I_Vp_PU failure in the submitted data log, was reported to have  data log measurement clamped at 2mA, and DC30 alarm on the   $\mathrm{V}+$   pin.  SN2 failed on OS_VPLUS_ANODE parameter. And,  while SN3 had I_Vp_PU measurements within limits, it was  datalogged as a failure on the same parameter due to an alarm  on the DC30 instrument for the AVCC and DVCC pins.

Based on the curve trace results, SN1 was endorsed back to the  Test Engineering Group for re-testing. The unit passed all  parameters including  $\mathrm{V}+$   current at power up (I_Vp_PU).

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8f16c2de-6160-4fff-83d7-8890cca3102b/8f16c2de-6160-4fff-83d7-8890cca3102b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=52a031b77e052acd5071a0ccc3cca72380a93678)
Figure 1.  No curve trace anomaly on  $\mathrm{V}+$   wrt GND on SN1

Bench testing for SN3 showed current measurements  comparable to a known good unit and within limits and showed  operational functionality for all 32 channel outputs.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2827d7c5-b589-4a75-8589-888329a46955/2827d7c5-b589-4a75-8589-888329a46955.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=2a001de0db9a80424c45b467b7f1fc629d778208)
Figure 2.  No curve trace anomaly on  $\mathrm{V}+$  , AVCC, and DVCC  for SN3

The short between V+ (K1/K2) and GND for SN2 needed to be  verified by opening the package and verifying the topside of the  die for any sign of die-related defects.

![1.36mA@100mV  SN2  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cafbf2b4-5460-4845-9b32-6e130bec08ce/cafbf2b4-5460-4845-9b32-6e130bec08ce.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=f34c99062bb5dd6ac91dc31899cf82b13c3a0fa9)
Figure 3.  Curve trace anomaly on   $\mathrm{V}+$   (K1/K2) and GND for  SN2

Optical Inspection post decapsulation of the top of the die of  SN2 showed no obvious die-related anomaly.

![DIEE  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bba5df57-dda3-4f76-a2f3-767e671eced5/bba5df57-dda3-4f76-a2f3-767e671eced5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=be65dab9de5d07060f032354deaea1fcec924eed)
Figure 4. Optical photos for the exposed HV dice of SN2

Optical Beam Induced Resistance Change (OBIRCH) identifies  the failure location by scanning the surface of the die using an  infrared laser and then detecting any changes in resistance value  caused by the laser. Extremely small changes in resistance can  be observed due to localized heating caused by the laser.  While  biasing the   $\mathrm{V}+$   to GND short on the unit, an anomalous  resistance changing site was observed on die 3.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3ed67291-1d79-47aa-a5cb-dbb2c39325aa/3ed67291-1d79-47aa-a5cb-dbb2c39325aa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=8d0a027da650ee5e4fa5cfb790ee6c0c35bd4241)
## 1.2 Second Case Study – SOIC_CAV  

A unit of Inverted Plastic Cavity Package (SOIC_CAV), was  submitted for failure analysis. The unit, reported as Production  Line reject, was submitted with the following failure  description: “Gyro offset failed.”

The unit was tested using an ADI evaluation board for   SOIC_CAV device.   Bench testing results showed a failing  gyroscope offset response while the X and Y accelerometer  offset responses remained within limits as shown in  Table 1 and Figure 6.

Table 1.  Bench Test Results

| Test Name|Initial|After Tap|        Lower                Limit      |Upper Limit|
|---|---|---|---|---|
|VSA,VSD (V)|3.290|3.290|3.15V|5.25W|
|CP5,V|30.17|30.17||Typ =31V|
|        Zero-rate Offset                (Gyroscope), deg/s      |41.809|41.900|-5 deg/s|+5 deg/s|
|        X-Offset                (Accelerometer), mg      |||-30 mg| +30 mg|
|        Y-offset                (Accelerometer), mg      |12.75|12.75|-30 mg|+30 mg |


![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7e0c36c7-fd96-4875-8e4e-a31e0750d885/7e0c36c7-fd96-4875-8e4e-a31e0750d885.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=04b3595552b9af497df82fe47e12b027ac4b4851)
Fig.6. Snapshot during bench testing showing good  accelerometer offset and failing gyroscope (yaw) offset  responses

The unit was electrically tested on the Automatic Test  Equipment (ATE) using the standard production test program.  Results at ambient   $(25^{\circ}\mathrm{C})$  , hot   $(105^{\circ}\mathrm{C})$  , and cold   $(-40^{\circ}\mathrm{C})$    temperature settings showed failing gyroscope offset,  gyroscope sensitivity, Continuous Self-Test (CST) and  Gyroscope   On-Demand   Self-Test   (ODST)   parameters.  Multiple failing Coriolis Signal Path – Sigma Delta Modulator  (CSP_SDM) parameters were also observed.

The unit was subjected to test modes centered on the circuitry  within the Coriolis Signal Path (CSP) block.  Results showed a  very low gain response on the Sigma-Delta-Modulator. See  Figures 7 to 12.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/769c77ed-61fd-40d6-ab94-f36161356eb5/769c77ed-61fd-40d6-ab94-f36161356eb5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=9556c1ee74945b3d53d122f547763133b0f6553a)
Fig.7. Graphs showing good Gyroscope Modulator Clock  output

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d668697c-0ced-4837-bad9-22a77a5170cf/d668697c-0ced-4837-bad9-22a77a5170cf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=f275b975cd5ab3d896c056cec295a902ae571562)
Fig.8. Graphs showing good Ampdet reference levels

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d72b1809-0ff1-4e62-876f-581d1b07cec8/d72b1809-0ff1-4e62-876f-581d1b07cec8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=a1709564e3777a16b8e11c06294ca0fcf788a583)
Fig.9. CSP Check [smdref   $=$  ampdet | sdmin = BPF o/p]  showing anomalous response on the returned unit

![  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f4c6d2d9-c76c-40c9-ac8b-87b0cf31802c/f4c6d2d9-c76c-40c9-ac8b-87b0cf31802c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=76d285cf2997b0292d293f4d6b359e3e8f93f5d7)
Figure 10. CSP Bias [AVDD/AVSS | Vcm]

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/23291281-fa43-4c8f-b417-ebdd12752b7e/23291281-fa43-4c8f-b417-ebdd12752b7e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=31ee737e80d157df3dc690d148503485a1030d53)
Figure 11. Graphs during CSP Power Down Test Mode  showing good response on the returned unit

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ca1733c6-436e-43fd-817a-4c0fd8bb2831/ca1733c6-436e-43fd-817a-4c0fd8bb2831.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=9093138a4a9acbd50964264b0640cc122e274a22)
Fig.12 Graphs during CSP signal path check showing good  response on the returned unit.

Backside grinding needed to be done on the unit for further  electrical analysis.

## II.   EXPERIMENTS  

## 2.1 Materials   

1.    Hot Plate    2.    Thermoplastic cement    3.    Analog Selected Area Preparation (ASAP) system    4.    Infrared (IR) Infrared Microscope    5.    OBIRCH system    6.    Light Emission Microscopy (LEM) system    7.    Nitric acid    8.    Plastic tweezers

## 2.2 Procedure  

2.2.1. Backside Grinding of the CSP_BGA device

1.    Based on the die layout review, the area of interest at  the back of the die was selected.  The area to be exposed should  not damage any solder bumps and electrical connections linked  to the electrical fault found during curve tracing/bench testing  analysis.

![LEGEND:  Area tobe  exposed  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e852f78e-3cc4-4418-8551-931e05e1cd37/e852f78e-3cc4-4418-8551-931e05e1cd37.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=1a6e9de5b3d4bb41a789d828023698e093cfcb9b)
Figure 13. Sample image showing an area to be exposed  without damaging the  $\mathrm{V}+$   and GND connections

2.    The top of the device was covered with thermo plastic  cement in preparation to mounting in the ASAP plate since the  top of the device was already opened and the dice and wire  bonds are already exposed.

![o00000000  ermoplastic cement  000000000  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fa776943-e999-4cb3-9792-9f673267fe20/fa776943-e999-4cb3-9792-9f673267fe20.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=47b7f02b8d974e6c2e9a6a7580028f7b95857bbd)
Figure 14.  Actual optical photo of SN2 (right) and sample  representation of thermoplastic covering (left)

3.    Device was mounted top down on the ASAP plate  using thermoplastic cement in preparation to backside grinding.

![HOTSURFACE    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d5da4e9d-e3e2-4459-a85e-50296daeaaa8/d5da4e9d-e3e2-4459-a85e-50296daeaaa8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=2818b72544e63d1f993a658e1afc419da8a935ad)
Figure 15. Device mounting (right) and side view  representation of a mounted device (left)

4.    The backside of the device was milled based on the  anomalous resistance seen during OBIRCH analysis.  The  solder balls and laminate were milled using a coarse milling

tool.  The copper layer was milled using a milling tool.  The  back of the die was exposed using a fine milling tool.

![  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/81fa1341-2249-4a9d-87de-200f91db9794/81fa1341-2249-4a9d-87de-200f91db9794.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=7439d4734459028d0e39f7d97db07e8157b05d0b)
Figure 16.  Backside mechanical grinding using ASAP system

5.    The device was demounted from the plate and  backside of the device and was inspected in IR microscope.  6.    The unit was checked post-back grinding in OBIRCH  system to check if device can still be electrically stimulated

## 2.2.1. Backside Grinding of the SOIC_CAV device  

1.    The area of the back of the die for back grinding using  X-ray was checked.

![    Area to be exposed  Area to be exposed  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0e9c49e2-6cb6-4b30-9b38-ed1def8a0825/0e9c49e2-6cb6-4b30-9b38-ed1def8a0825.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=4a6fd4993a9d7808044a59507b10975c656dbef9)
Figure 17.  X-ray images of the SOIC-CAV device showing the  die of interest

2.    The device was mounted metal-plate-cover down on  the ASAP plate using thermoplastic cement in preparation for  backside grinding.

![  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8d46f3c5-d907-4c92-90ee-126edef399a1/8d46f3c5-d907-4c92-90ee-126edef399a1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=4c7e7e675a0f13c50f58609f868c5d113a7a0bd1)
Figure 18.  Representation of device when mounted in the  ASAP plate

3.     The backside of the device was milled based on the  X-ray image.  The package was milled using a fine milling tool  until the die attach of the device was exposed.  Minimum table  speed and tool speed was used to prevent damage on some parts  of the device during mechanical grinding.

![AAPI  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bfe8c95f-9dd6-4af2-9281-3a3034a22e4d/bfe8c95f-9dd6-4af2-9281-3a3034a22e4d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=777cfd28a146adfaf551cc3a23071206263f4e50)
Figure 19. ASAP table speed set to 1 and Tool speed is set to 1.

![  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cd32a118-5635-4146-adf2-ba8aa2e54ad8/cd32a118-5635-4146-adf2-ba8aa2e54ad8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=f8704b6c037b5ac2313f69be21030df569057854)
Figure 20.   Backside mechanical grinding using ASAP system

4.     After the die attach of the target die was exposed, the  exposed area was partially treated with Nitric acid to soften the  die attach.    Note:  Further polishing in the ASAP system will not be  possible since only the gel coat is supporting the die.    5.    Die attach was carefully scrape using plastic tweezers  until back of die was exposed.

## III.    RESULTS AND DISCUSSION  

## 3.1    CSP-BGA  

## 3.1.1 Covering of the decapsulated device  

The top of die and exposed wire bonds were successfully  covered by the thermoplastic cement.

Note:  Use of thermoplastic cement involves heating on a hot  plate at 150 degC.  This is not applicable to heat sensitive  devices.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ab5a825b-14ca-45e4-8eca-d0b1c64c3517/ab5a825b-14ca-45e4-8eca-d0b1c64c3517.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=1f495bd270d458a6567cbd88695be44a46a262ac)
Figure 21. Optical photo of the decapsulated device (left) and  the device after thermoplastic curing (left)

## 3.1.2     Backgrinding of device  

The back of the die where the anomalous emission was seen in  OBIRCH was successfully exposed without damaging the other  bumps and connections.

![  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e537c3ec-d90b-4cd3-8419-d9aa06832745/e537c3ec-d90b-4cd3-8419-d9aa06832745.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=639a452985dcbec88e4da45582d94de81f45121c)
Actual optical photos of the unit after backside grinding

## 3.1.3    Infrared Inspection  

The exposed area was inspected in the infra-red microscope.   The areas of interest were clearly seen via IR microscope.  IR  results showed the damage in the bypass capacitor.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c9968b00-a5ea-4530-abfe-d6c0291aa66e/c9968b00-a5ea-4530-abfe-d6c0291aa66e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=9227b065f4c920b34ba19f0099ac5945a1b57fe0)
Figure 23. IR images showing the damage in the bypass  capacitor

## 3.1.4    OBIRCH  

The exposed area was subjected to OBIRCH analysis. The  device can still be electrically stimulated post-backside  grinding. OBIRCH analysis isolated the damage in the  capacitor and showed the possible origin of damage.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e7478403-9a81-45c3-9af3-68dcb0174245/e7478403-9a81-45c3-9af3-68dcb0174245.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=c8eb2c1624ef99b8c368fec813155a845361c41a)
Figure 24. OBIRCH analysis on the back of the exposed die  possibly pointing to the damage

## 3.2    SOIC-CAV  

3.2.1    Backgrinding of device      The die attached of the target die was successfully exposed.

Bench testing was performed on the unit post backside  grinding. Results showed the unit consistently exhibited the  same failing responses prior to backside grinding.

## 3.2.2    Light Emission Microscopy (LEM)  

Light Emission Microscopy enables the location of sub layer  defects through detection of faint light levels emitted from  silicon device structures. These faint light levels arise from  recombinant radiation emitted from p-n junctions and from  oxides. Photon emission analysis was performed on the  backside of the ASIC die to further isolate the location of the  suspected defect, while biasing the unit in the failing state. An  anomalous emission was observed on the PMU block of the  unit as shown in Figure 27.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/54f5131d-0003-403a-b923-1eb7385eb8aa/54f5131d-0003-403a-b923-1eb7385eb8aa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=bd99ac5577c276e80bdb339b07862801f9d09833)
Figure 27.    Images of the ASIC die during backside LEM  analysis showing the anomalous emission on the PMU block of  the returned unit

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8c1a68c7-8522-4fd3-b96c-0a02c01b18ed/8c1a68c7-8522-4fd3-b96c-0a02c01b18ed.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=25ad2ad8290f6aab976416ed2e4f5476aabf1093)
Figure 25.  Representative optical photo after mechanical back  grinding

3.2.2    Partial chemical etching and die attach removal  The exposed die attach material was partially etched with nitric  acid.  The softened die attach material was carefully scraped.   The back of the target die was successfully exposed.

## IV.     CONCLUSION  

Mechanical grinding to expose the backside of an  opened/decapsulated CSP-BGA device to conduct backside  fault isolation is possible using the method described in this  paper.  The top of die and the exposed wire bonds are protected  during mechanical grinding and solder bumps and electrical  connections linked to the electrical fault are still intact after the  destructive analyses.  The method still rendered the device  electrically good for backside fault isolation.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b29c577e-d624-4d9a-a4c6-b93c6d90f425/b29c577e-d624-4d9a-a4c6-b93c6d90f425.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215660%3B1743219260&q-key-time=1743215660%3B1743219260&q-header-list=host&q-url-param-list=&q-signature=c1b8f98cd0460008947cc29b9c2e0813dd3828ab)
Figure 26. Representative optical photo showing the exposed  back of die

3.2.1    Bench Testing post back grinding

Mechanical grinding to expose the backside of a target die of an  SOIC-CAV device to conduct backside electrical analysis is  also possible using the method described in this paper.  The  back of the target die was exposed mechanically without  damaging the sensitive parts of the device.  Bench testing on the  unit post-backside grinding proved that the unit consistently  exhibited the same failing responses prior to backside grinding.

## V.      ACKNOWLEDGMENT  

The authors would like to acknowledge Cindy Cabezas, Arnold  Evangelista, Melanie Cajita and Augusto Andal for their  support in these technique development projects.

## VI.    REFERENCES  

1.    Perry Martin, Electronic Failure Analysis Handbook, Mc  Graw Hill, 1999, Chapter 1, pp 1.1.    2.     Lasers and Electro-Optics Society, 2003. LEOS 2003. The  16th Annual Meeting of the IEEE


## VII.    ABOUT THE AUTHORS  

Melissa O. Caseria graduated with a degree in Bachelor of  Science in Chemical Engineering from Saint Louis University,  Baguio City.  She is currently a Senior FA Engineering  Specialist in Global Failure Analysis in Analog Devices  General Trias, Inc.

Dennis R. Madriñan graduated from Mapua Institute of  Technology with a degree of Bachelor of Science in Electronics  and Communications Engineering. He is currently a Failure  Analysis Engineer for Global Failure Analysis in Analog  Devices General Trias, Inc.

