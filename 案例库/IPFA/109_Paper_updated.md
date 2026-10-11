---
title: "109_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_cae66de08a8b71c225b2d2e06d66585d7295230462135641
file_size: 1539149
---

## Study on Loop Circuit Function Failure Isolation  Method on Mix Signals IC  

Jon Ren \* , Jacky Wen, Fay Liu, Hairong Di   Product Quality Center, NXP semiconductor, Tianjin, China  \*Phone: +86-19922419738  Email: jun.ren@nxp.com

Abstract —With the increasing integration of IC chips, their  functions are becoming more complex. Apart from processing  input and output signals, these chips also possess self-protection  capabilities. In cases where chips have self-protecting circuits, a  loop circuit is formed by the protection circuit and other blocks.  Analyzing failures in loop circuits is a challenging process. This  paper proposes the application of external stimulus to simplify  the analysis procedure. This method not only reduces extensive  microprobe analysis work and failure analysis time but also  enhances the success rate of IC chip failure analysis

Keywords—Loop Circuit, Mix signals IC, Failure Isolation,  external stimulus.

## I.    I NTRODUCTION 

With advancements in IC manufacturing technology,  particularly the implementation of novel lithography  techniques, there has been an increase in the integration  density of metal-oxide-semiconductor field-effect transistors  (MOSFET) per unit area [1]. The functionality of IC chips is  becoming more intricate, enabling intelligent chips to monitor  and process feedback signals while executing appropriate  adjustment actions to maintain desired output status.  Additionally, these chips possess robust self-protection  capabilities.

It is a common form of self-protection for a chip equipped  with various protective measures, including over current (OC)  protection, over voltage protection (OV), over temperature  (OT) protection, and under voltage (UV) protection. The  chip's self-protection function primarily consists of two  blocks: the sensor block and the logic operation block. The  sensor block converts abnormal input and output signals (such  as excessively low or high voltage or current) or abnormal  working conditions (extremely low or high chip temperature)  into electrical signals. These signals are then processed by the  logic operation block to control the shutdown of the chip's  main function.

The input signals of most sensor blocks, particularly for  OV, OC, and UV function circuits, are sense signals derived  from the main output signals. However, after processing the  input signal of a sensor block, the logic operation block  sequentially controls the chip's output signal. Therefore, a  general self-protection circuit operates as a loop circuit. For  loop circuit function failure analysis, Photo Emission  Microscope (PEM) has been widely employed to identify  abnormal device states. This is followed by combining layout  and schematic analysis with microprobe or Electrical Optical  Probe (EOP) analysis to isolate each failure step [2]-[5]. This  conventional process requires a long analysis time and would  bring uncertainty to the analysis results.

In this paper, we propose the application of external  stimulus to simplify the analysis process [6]. This method can  significantly reduce the amount of microprobe analysis  required and shorten failure analysis time. We present three

case studies to demonstrate how external stimulus can aid in  analyzing loop circuit function failures.

## II.    EXTERNAL STIMULUS METHOD INTRUDUCTION   

The key of loop circuit failure analysis is to eliminate the  interaction between signals. If an abnormal signal input to a  block, it will inevitably affect the state of its output signal.  External stimulus means forcing a DC voltage, DC current or  waveform to a loop circuit to break the loop and eliminate the  influence between the loop circuit signals.

For instance, presented here is a loop circuit comprising  four blocks A, B, C, and D that interact with each other  through their respective output signals a, b, c, and d (Fig. 1).  These blocks and signals within the loop circuit exhibit  abnormal behavior. External stimulus method means force a  signal   ${}^{\bullet}\flat^{+}{}^{\bullet}$   to block B in order to restore it to its normal state.  This method effectively breaks down the entire loop circuit,  facilitating quick isolation of the failure for analysts.

![BlockA  Signald   Signala  Force"b+"on  block B  Block D   Block B  KSignalc   Signalb  Block C  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7d0f853a-061f-4c8c-8c71-1dd9f89fda65/7d0f853a-061f-4c8c-8c71-1dd9f89fda65.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215822%3B1743219422&q-key-time=1743215822%3B1743219422&q-header-list=host&q-url-param-list=&q-signature=87a6fe66d27c7f5e4c31e4158dd369b12f5b6c6e)
Fig. 1.   Schematic diagram of external stimulus

External stimulus also has the following advantages,  which can help the analyst to quickly isolate the failure.

The external stimulus has a stronger load capacity for  some functional failures caused by leakage issue.  Abnormal spots can be more easily captured by PEM  if external stimulus applied on failed signals.        The external stimulus will change the working state of  some failed modules, and the PEM analysis with  different working states will also provide more clues  for the analyst.

## III.   E XPERIMENT  AND  RESULTS 

## A.   Case 1  

One analog digital mixed signals IC chip was failed on  fail-monitor (FMON) block’s all output signals (Fig. 2).  FMON block detects the key signals of the chip starting up. If  the key signals were abnormal, FMON block will make the

chip shut down in time to avoid damage to other hardware.  FMON block contains some analog blocks and one embedded  logic block which can’t be covered by ATE scan test.

![MDOFF1A  MDOFF1A  MDOFF1A  MDOFF1A   MDOFF1B  MDOFF1B   A1l FMON MDOFF1B  All FMON  MDOFF1B  output drop   MDOFF2A  MDOFF2A  MDOFF2A  DFE2   MDOFF2B  MDOFF2B  MDOFF2B  MDOFF2B  Failed part  Failed part    Reference part  Reference part  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d528b5b3-9403-427a-ba4a-b0687585638e/d528b5b3-9403-427a-ba4a-b0687585638e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215822%3B1743219422&q-key-time=1743215822%3B1743219422&q-header-list=host&q-url-param-list=&q-signature=bccb13207230a01c57d583de16de2e78cdb0cc6d)
Fig. 2.   Failed part was failed on  $2^{\mathrm{nd}}$   pulse checking, reference part was  normal starting after   $6^{\mathrm{th}}$   pulse checking

There was no abnormal spots highlighted by PEM analysis  based on FMON function failure. Microprobe analysis  showed lots of abnormal signals. Deep schematic analysis  found analog block, failed signals and embedded logic block  formed a loop circuit (Fig. 3). For this loop circuit especially  include embedded logic block. The failure hardly to be  isolated by microprobe analysis if there was no obviously  guidance. Meanwhile, the designer's simulation was also  difficult to accurately located failure since such embedded  logic blocks can’t be covered by scan test.

![FSCK  Vcca_oy  Vcca_uy  VCCA monitor block  sha_i  MDOFF1A  sha_vok  MDOFF1B  Embedded logic  block   MDOFF2A  COV  MDOFF2B  xuv  Otherkeysignalsmonitor  blocks  x_vok  FMONblock  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4d983230-569d-47e4-83b9-226b25d18e7c/4d983230-569d-47e4-83b9-226b25d18e7c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215822%3B1743219422&q-key-time=1743215822%3B1743219422&q-header-list=host&q-url-param-list=&q-signature=7ecdbcb615bfc8e8079c0cbb93203221b3c45156)
Fig. 3.   FMON block schematic diagram

External stimulus can’t be applied on failed signal since  those signals have a specific frequency and the external signal  clock is difficult to synchronize the clock of the embedded  logic block.

![ Enter to   VCCAOV  Power on  normal mode   check  FSCK 1st pulse  Return to    Return to   normal mode    normal mode  FSCK 2nd pulse  FSCK 6thpulse  Othersignals    Return to   VCCA UV  check   normal mode   check  FSCK5th pulse   FSCK 4th pulse   FSCK 3rd pulse  nununun   nUnUn  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/507fdb50-63c5-459c-9cb0-ba216559764e/507fdb50-63c5-459c-9cb0-ba216559764e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215822%3B1743219422&q-key-time=1743215822%3B1743219422&q-header-list=host&q-url-param-list=&q-signature=e4f5aedc6b5eb41e9f2d48710dd35aad51eaa151)
Fig. 4.   State machine diagram

Based on FMON output signals waveform that all outputs  signals would be shutdown, the state machine of FMON block  was studied. Result showed FMON was controlled by signal  FSCK which generated by evaluation board (EVB), and  FSCK is FMON embedded logic block clock signal. After  check failed part waveform time sequences, the chip failed on  VCCA under voltage checking step. And this step was  triggered by the 3rd FSCK clock signal (Fig.4).

When VCCA UV checking was failed, failed part would  shut down all FMON outputs and enter sleep mode. However,  VCCA UV checking time was too short (less than 1us) and  that was not enough to do further analysis. To prolong the time  of fail status to perform further analysis. FSCK which  generated by EVB was bypassed. A multiple single-trigger  pulses was forced on FSCK from external. State machine  study indicated FSCK 3rd single-trigger pulse would make  FMON keep on VCCA UV checking step and remain in this  step until next FSCK pulse arrived. Bench tested result  showed, when FSCK 3rd pulse was sent to failed part from  external, all FMON output signals were keep high voltage  (Fig.5).

![MDOFFxX  MDOFFxx   MDOFFxx  MDOFFxx  FMON output was set as high  FMON output was set as high  after 3"d FSCK pulse  after 3 rd   FSCK pulse  FSCK  FSCK   FSCK  FSCK  Failed part  Failed part    Reference part  Reference part  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/51c285d9-0c37-4119-ac19-aa95abe2e6cd/51c285d9-0c37-4119-ac19-aa95abe2e6cd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215822%3B1743219422&q-key-time=1743215822%3B1743219422&q-header-list=host&q-url-param-list=&q-signature=0baf6f8078b66f1a23fa6f1c4ed8b8d5cd57340f)
Fig. 5.   External FSCK 3rd pulse stimulus result

PEM analysis based on FSCK 3rd pulse forcing result was  tried again. And an abnormal spot was detected on embedded  logic block. Based on PEM analysis result, microprobe  analysis detected leakage failure between signal vdig to N_21.  The defective N_21 was an intermediate level signal because  it was activated by both vdig and GND. For the embedded  logic circuit, the intermediate level signal may be recognized  as 1 or 0. For this case, when the FSCK 3rd pulse was sent,  defective N_21 was identified as 0, so the failed part FMON  outputs behaves exactly same as reference part.

![400  Failed part  Failedpart  Abnormal PEM   100   leakage  leakage  spot   V1 0v)   1.00/div  PEM analysis lens 20X  PEM analysis lens 20X   Vdig to N_21 I-V  Vdig to N_21 I-V    silicon damage &  silicon damage &  silicide missing  silicide missing  Probe needle  OBIRCH hot  spot,  location  t. 1oca  same as PEM  spot  OBIRCH analysis lens 100X  OBIRCH analysis lens 100X   Physical analysis  Physical analysis  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5e7cae33-0b57-4c3a-bfd8-9e2c94ef1137/5e7cae33-0b57-4c3a-bfd8-9e2c94ef1137.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215822%3B1743219422&q-key-time=1743215822%3B1743219422&q-header-list=host&q-url-param-list=&q-signature=0e69eb5ae23859b7f3cb6b2ef24db44e311c868a)
Fig. 6.   PEM, OBIRCH and physical analysis result

Then Optical Beam Induced Resistance Change  (OBIRCH) analysis was applied on failed part. Hot spot was  detected on one NMOS FET of embedded block which same  as the location of PEM abnormal spot. Deprocess and Focused  ion beam (FIB) cross section indicated silicon damage and  silicide missing on NMOS FET (Fig.6).

## B.   Case 2  

One mixed signal IC chip which contained analog and  logic block was analyzed. ATE data log showed IC chip was  failed on output pin D2H and internal signal overtemp_2.  Signal overtemp_2 was generated by overtemp block and it’s  also input signal of main_logic block. Schematic analysis  found abnormal overtemp_2 would lead to D2H abnormal,  meanwhile, overtemp_2 and several blocks and signals made  up a loop circuit (Fig. 7).

![Switch  Output_2   D2H  Driver_2  block  Block  Main_logic  Block  Trip2_1   0t2_1  Trip2_2   Overtemp.   0t2_2   Overtemp  Trip2_3  detectblock   ot2_3   block  Overtemp_2  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b8f5b5ae-3aec-4e3d-8cf3-a9e4bf421234/b8f5b5ae-3aec-4e3d-8cf3-a9e4bf421234.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215822%3B1743219422&q-key-time=1743215822%3B1743219422&q-header-list=host&q-url-param-list=&q-signature=1bc5c0f39f9f81fa5602bec95d69c40d627e82c0)
Fig. 7.   Schematic diagram

Abnormal overtempt_2 signal led abnormal D2H was  confirmed by external stimulus. A good voltage (Good  overtempt_  $2{=}0\mathrm{V}$  , failed part overtempt_  $_{ Ḋ }2 Ḍ=\!2.5\mathrm{V}$  ) was forced  on overtempt_2, then D2H returned to normal. But when D2H  forced a good voltage, signal overtemp_2 keep abnormal. That  means, abnormal overtempt_2 signal could lead abnormal  D2H.

checked. Forcing result showed trip2_3 pull down current was  abnormal (Table II).

TABLE II.     FAILED   PINS   TESTED   RESULT

|Signal|REF part pull down current|Failed part down current|
|---|---|---|
|Trip2_1|17uA|15uA|
|Trip2_2|20uA|18uA|
|Trip2_3|19uA|168uA|


TABLE I.     E XTERNAL STIMULUS RESULT

|Signal|REF part no forced|Failed part no forced|Failed part overtempt_2 forced|
|---|---|---|---|
|Trip2_1|2.5V|0V|2.5V|
|Trip2_2|2.5V|0V|2.5V|
|Trip2_3|2.5V|0V|2.5V|
|Ot2_1|0V|2.5V|0V|
|Ot2_2|0V|2.5V|1.4V|
|Ot2_3|0V|2.5V|0V|


Based on pull down current tested result, function  OBIRCH was applied on failed part. Function OBIRCH  means using OBIRCH to provided forcing voltage then to  perform OBIRCH analysis in functional mode. In this case,  2.5V voltage was provided by OBIRCH and it was forced on  trip2_3. Result showed there was a hot spot on a MOSFET of  abnormal chip (Fig. 8).

It’s hardly to find the root cause just by microprobe  analysis for this loop circuit. Therefore, external stimulus  provided a high effective way for this loop circuit which was  formed by main_logic, overtemp_detect and overtemp block.  Signal overtemp_2 was forced a good voltage, then other  signals were checked. Result showed that only ot2_2 keep fail  when overtemp_2 was forced a good voltage (Table I).

Based on the above external stimulus result, the failure  could be isolated in overtemp_detect block. Therefore, further  study should be focused on failed signal ot2_2 to perform  microprobe analysis. But external stimulus provided some  new setup configurations. Then overtemp_2 was forced a  good voltage, then PEM analysis was performed, but no  abnormal spots were found. Secondly, the input signals of  overtemp_detect block were forced with good voltage (Good  voltag  $\mathord{\leftmoon}=\!2.5\mathrm{V}$  ) respectively and pull down current was

![OBIRCH  OBIRCH  analysis hot spot  analysis hot spot   ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6aa239a2-fbeb-42d6-89b4-8690e91413e8/6aa239a2-fbeb-42d6-89b4-8690e91413e8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215822%3B1743219422&q-key-time=1743215822%3B1743219422&q-header-list=host&q-url-param-list=&q-signature=6b78d291a3c298301f6ceb7e3e025208b3fa94d6)
Fig. 8.   Function OBIRCH analysis result

Layout and schematic analysis showed OBIRCH hot spot  located on one NMOS FET. This MOSFET abnormality  would cause all function failure. Deprocess and scanning  electron microscopy (SEM) analysis showed electrical  induced physical damage (EIPD) on NMOS FET (Fig. 9).

![Optical image Optical image    NMOS FET NMOSFET    EIPD  EIPD  EIPD  OW  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9a62a507-ea57-43d3-9ec7-822a444469e6/9a62a507-ea57-43d3-9ec7-822a444469e6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215822%3B1743219422&q-key-time=1743215822%3B1743219422&q-header-list=host&q-url-param-list=&q-signature=98e689157d5296ad7bf70d093839968558304bf9)
Fig. 9.   PFA analysis result

## C.   Case 3  

One function failure case of mixed signal IC chip was  analyzed. The IC chip was failed on one of the four outputs.  Out3 voltage of failed part was 0V, while the one of  reference  part was 12V.

PEM analysis didn’t find any abnormal spots on failed  part. Microprobe analysis found several abnormal signals on  failed part, meanwhile, all the failed signals and related blocks  formed a loop circuit (Fig. 10).

![Output   Dir3   OUT3  Output Block  Driver Block  Em3   Out3_C  OC3   Overcurrent  Logic Block  Block  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5e6214e4-ce54-4151-aead-82eeba1d4968/5e6214e4-ce54-4151-aead-82eeba1d4968.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215822%3B1743219422&q-key-time=1743215822%3B1743219422&q-header-list=host&q-url-param-list=&q-signature=3254885aa7e23dca9b330532c4bc68892e3569c6)
Fig. 10.   Failed signals and blocks formed a loop circuit

For this case, follow-up normal handle procedure was  deeper microprobe analysis or deeper circuit analysis from  design aspect. This would spend a lot of analysis time. To  reduce the analysis time, external stimulus was applied. Due  to signal Out3_c was copied from OUT3, OUT3 was forced a  good voltage (12V), then other signals were tested (Table III).

TABLE III.     FAILED   PINS   TESTED   RESULT

||REF|OUT3 no forced|OUT3 forced|
|---|---|---|---|
|Out3_c|12V|0V|12V|
|OC3|0V|2.5V|2.5V|
|En3|2.5V|0V|0V|
|Dir3|5V|0V|0V|


External stimulus analysis showed signal OC3 was still  failed when out3_c was normal. Therefore, overcurrent block  abnormal was high suspected. To verify this conclusion,  external stimulus was applied on signal OC3 that it was forced  a good voltage 0V, result showed other signals would return  to normal (Table IV).

TABLE IV.     FAILED   PINS   TESTED   RESULT

||REF|OC3 no forced|OC3 forced|
|---|---|---|---|
|Out3_c|12V|0V|12V|
|En3|2.5V|0V|2.5V|
|Dir3|5V|0V|5V|


After above analysis, logic block, output driver block and  output block function normal was confirmed, and function  failure could be isolated in overcurrent block. Based on  external stimulus result, PEM analysis with different setup  configuration was tried. Firstly, OUT3 was forced a good  voltage. Then, PEM analysis was performed, but no abnormal  spot was found. The external stimulus was applied on signal  out3_c, and abnormal spot was found on one capacitor of  overcurrent block. This abnormal capacitor could lead to final  function fail. Deprocess and SEM analysis found scratch on  the capacitor (Fig. 11).

![Abnormal emission  Abnormal emission  spotoncapacitor  spot on capacitor  Abnormal chip PEM analysis result Abnormal chip PEM analysis result    Scratch  Scratch  SEM image revealed scratch on the PEM spot  SEM image revealed scratch on the PEM spot  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2dc57593-ff4c-4f1b-9837-a2146cbc0285/2dc57593-ff4c-4f1b-9837-a2146cbc0285.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215822%3B1743219422&q-key-time=1743215822%3B1743219422&q-header-list=host&q-url-param-list=&q-signature=6627615a8c65b8555eab06944070d3419b190390)
Fig. 11.   PEM analysis and physical analysis result

## IV.   C ONCLUSION   

With complexity of a IC chip function increasing, loop  circuit becomes the most common type of circuit structure. It  makes failure analysis more complicated and need consume  long analysis time. External stimulus would isolate the failure  to abnormal block from many blocks quickly. In the  meantime, external stimulus will provide many different setup  configuration, this will provide much useful information to  find the root cause when combined with OBIRCH and PEM  analysis. External stimulus will reduce the IC chip failure  analysis time and increasing the success rate.

## A CKNOWLEDGMENTS 

Thanks PFA team of NXP Tianjin PDQC lab for their  great efforts in cases analysis. Also, thanks to other colleagues  of EFA team of NXP Tianjin PDQC lab who gave much  assistance.

## R EFERENCES   

[1]    Bruning, J.H.: ‘Optical lithography … 40 years and holding’, Proc.  SPIE, pp. 652004:1–652004:13, 2007    [2]    Gaojie Wen, Xiaocui Li, Li Tian, Jon Ren, “Dynamic Current  Monitoring and Probe Laser Simulation Strategy to Analyse  Complicated Functional Failure on Mixed Signal Integrated Circuit”,  IPFA2017, pp128-132    [3]    Haus Zhang, Power Tian, Xuejian Qian, Winter Wang, “Electro  Optical Probing / Frequency Mapping (EOP/EOFM) Application in  Failure Isolation of Advanced Analogue Devices”, IPFA2017, pp.602- 607    [4]    Gaojie Wen, Li Tian, Diwei Fan, Jingrong Song, Jon Ren, Dong Wang,  Xiaocui Li, “Simulation Assisting PEM Technical to Locate Defect on  Capacitor in Integrated Circuit Failure Analysis”, IPFA2016, pp.227- 230    [5]    Gaojie Wen, Binghai Liu, Winter Wang, “Failure Isolation Using FIB  Assist Photon Emission Microscopy Analysis and Microprobe  Analysis”, IPFA2011, pp.140-143.    [6]    Jon Ren, Gaojie Wen, Bird Fan, Winter Wang, Xiaocui Li, “Study on  Multiple-pins Function Failure Isolation Method”, IPFA2018, pp.1-4.

