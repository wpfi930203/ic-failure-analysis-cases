---
title: "196_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_c2ca54266877673d738a776807d28ab57295230462135641
file_size: 1276841
---

## Advanced Method to Locate The Defect on Zener  Diode to Avoid Cutting The Circuit in  Failure Analysis  

Xuejian Qian, Li Tian, Gaojie Wen, Hao Zhang, Xiaocui Li  Product Analysis Laboratory of Quality Department in Freescale Semiconductor(China) Limited  Phone: 86-22-85684376. Email:Xuejian.qian@nxp.com

Abstract-  Due to metal layers coverage, many signals  couldn’t be measured by mechanical probe test to perform electrical isolation. And usually EMMI [1]   (Emission Microscope) or OBIRCH [2]   (Optical Beam Induced  Resistor Change) analysis can’t directly highlight the  real defect for function failure. It’s difficult to isolate  Zener diode failure because the current path which  through others device. We can’t test the Zener diode  leakage directly unless to cut the circuit to isolate the  Zener diode alone. In the paper we proposed one novel  and effective method for locating Zener diode defect on  device level to avoid the irreversible destructive test.  The main idea was that if there is a defect on Zener  diode in spite we can’t find a leakage effected by others  circuit but we can find the voltage is abnormal. Then we  can use the function EMMI [3]  to location the defect instead of cut the circuit to isolate the Zener diode alone.  After PFA (Physical Failure Analysis), the defect was  found. Thus, we believe the advantage measurement  method is novel, effective and save cycle time. It was  beneficial to our FA for Zener diode on device level in  electrical failure isolation.

Keywords – Zener diode,No Leakage,Voltage high,  Function EMMI.

## I.   I NTRODUCTION 

In this paper we proposed one new method to  confirm and locate defect on Zener diode on device  level. The main idea was that if there is a defect on  Zener diode although we can’t find the leakage because others circuit effect but we can find the voltage  is abnormal. Then we can use the function EMMI to  location the defect instead of cutting the circuit to  isolate the Zener diode alone. After PFA (Physical  Failure Analysis), the defect was found. Thus, we  believed the advantages measurement method were  novel, effective and save cycle time. It was beneficial  to our FA for Zener diode fail on device level in electrical failure isolation.

## II. EXPERIMENTS  

The Zener diode in order to stabilize voltage it is usually connected in parallel with other circuits. Although there is a leakage, it impossible to detect directly due to the influence of other circuits.

So we summary three steps to confirmed the defect  on Zener diode.

Isolated the fail on correlation circuit of Zener diode and confirm the signal voltage abnormal higher than reference.

IV curve [4]  test can’t find any leakage.       Function EMMI was performed that add the  work voltage on the both ends of Zener diode.

## III. Simplified circuit Mode  

For complex circuits we can simplify to the following  circuit diagram.

![Vpower  Other  circuits  DZ  Other  circuits  Failsignal  GND  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e854e2d5-7cf7-4f79-86a7-009286146fec/e854e2d5-7cf7-4f79-86a7-009286146fec.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=e864b6f5690b63367746313b1cbcc4624b95a495)
IV. Real Case Analysis

According main idea of function EMMI, we applied  this method on real case successfully.

A.

First case

In this case functional failure was vdd5_oc fail on  CQC part. After decapsulation, EMMI analysis was  performed and the result revealed one block didn’t  work normally due to vdd5_oc fail. And then failure  isolated was continued by micro-probing test and root  cause was confirmed in one block with two normal  input signals(pref and senseref) and one abnormal  output signal(ilim_indicator). Test result as table1.  The zoom in partial circuit was showed in Fig.2.

||lim_indicator|pref|senseref|
|---|---|---|---|
|REF||4.7|5.7Wr|
|CRC|2.8V|4.70|5.7W|


Table1. Microprobe test internal signals result  of case

Ⅰ

![<vim  senseref  DZ  Ilim indicator.  gnd  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2a56601c-9185-41d0-95d4-ca261fa22cbf/2a56601c-9185-41d0-95d4-ca261fa22cbf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=772ba6da66ac6c406139f440222816d5052768a8)
Fig.2 Zoom in partial circuit of case Ⅰ

IV curve test ilim_indication to vin reveal normal.    Pictures were showed in Fig.3 and Fig.4.

![50u  A!Pfno'OT  40u  30u  20u  10u  -10u   Same to REF  SametoREF  （】TI  -30u  40u  -50u  V1（vD   1.00/div  Fig.3 Show IV curve of CQC part of case I  Fig.3 Show IV curve of CQC part of case Ⅰ     Sou  A!P/ nO'OT  40  30u  10 u  -10u  -20U  [】TI  -30u  40U  -50u  V1（v)   1.00/div  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1bd2bf77-f65c-4584-84e2-4aa7ddd3b3b4/1bd2bf77-f65c-4584-84e2-4aa7ddd3b3b4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=a0d73ecc3a0d401c26cb6367f24e41fd4c59256a)
Fig.4 Show IV curve of REF part of case Ⅰ

For the case, fellow up normal handle procedure only  is cut the circuit to isolated the DZ(Zener diode)  alone then test IV curve to check the leakage. For this  procedure will damage the unit and it is unrecoverable for going ahead function analysis. In the condition, we can use function EMMI [4]  that forced 2.8V  between vin and gnd to test. Result showed in Fig.5  that one abnormal emission spot was found on DZ  device.

![ abnormal emission spot  abnormal emission spot  Msg:1000x Msg:1000x  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/048a14e3-0e26-4edc-b7c6-8307d5cdcce1/048a14e3-0e26-4edc-b7c6-8307d5cdcce1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=ea0a25710b7ad3c487a80ca9a6c19da07b17e5b0)
Fig.5 Function EMMI test 1000X picture of case Ⅰ

Based on EMMI result, physical analysis was performed and  dislocation was found on DZ (Zener diode).  Result was  showed in Fig.6.

![dislocation  dislocation  D   node  5.00kV86pA3.8m  m150000xTLD SE     Fig.6 Physical result of case I  Fig.6 Physical result of case Ⅰ     SILBLR   LLBLK  Dislocation   DPN  location   HVNW  NWELL   NHVt.  NWELL  TRENCH  NBE  Pepi-1  Crosssectionimaqe   P++ Substrate  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/228dc260-6bc2-4ab3-bc2f-506a4d117144/228dc260-6bc2-4ab3-bc2f-506a4d117144.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=ce33c5b6634caaf33f3ab8e5ffd91facbaa73ed6)
Fig.7 Cartoon picture of defect location

B.    Second case

For second case functional failure was v2p5 low failure. In  EMMI analysis there were many missing spots, but no abnormal spot was found on Zener diode, see Fig.8.

![no emission spot  emission spot  Msg:1000x  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/87b6a833-29d6-48ef-a4da-a01955b8a4b7/87b6a833-29d6-48ef-a4da-a01955b8a4b7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=743731a02b9a2bd12988207f12243a3c5c262aa0)
Fig.8 Normal EMMI test 1000X picture of case Ⅱ

Then by a series of microprobe test, the fail was isolated to v2p5 regulatorcore block and found the signal  ‘net584’ abnormal high. Test result as table2. Zoom in  partial circuit was showed in Fig.9.

Table2. Microprobe test internal signals result of case  Ⅱ

||met584|met1006|
|---|---|---|
|REF||4.7|
|COTC|2.8wr|4.7W|


![ESS4  met1006  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2c5b5526-7c9d-46c5-80c9-f81ced0dbd1b/2c5b5526-7c9d-46c5-80c9-f81ced0dbd1b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=5fa22e443bbf450d7036bdc7d310a0a077160646)
Fig.9 Zoom in partial circuit of case  Ⅱ

IV curve test vddramp to net584 show normal. Pictures were showed in Fig.10 and Fig.11.

![S0:u  APno'o  0  川  -10u   Same to REF  Same to REF -20u  -30u  -40u  -50u  V1   1.00/div     ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/be83324b-b98f-4b2a-aa03-2d8c98243b76/be83324b-b98f-4b2a-aa03-2d8c98243b76.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=aaccfa9fc79a1d4210ac7a248b756980a8160bc5)
Fig.10 Show IV curve of CQC part of case Ⅱ

![sou 40u noo1  ¥30０ 20０ 100 -10u -200 -300 40U -50u V1（v）  1.00/div   ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/88d297ab-a02d-48c0-a86b-439f2fb9796a/88d297ab-a02d-48c0-a86b-439f2fb9796a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=f5b05524daaa90d61b989f3c2999b7beb6664d3e)
Fig.11 Show IV curve of REF part of case Ⅱ

In the condition, we used function EMMI that forced 2.3V between vddramp and net584 to test. Result was showed in Fig.12  that one abnormal emission spot was found on DZsoft device  instead of cutting the circuit.

![abnormal emission spot  abnormal emission spo  Msg:1000x  Msg:1000x    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a02c3b86-9e26-410e-acf0-3ef556211f5c/a02c3b86-9e26-410e-acf0-3ef556211f5c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=3f57c6e522276a166f1517a6c66bcbe4b012a048)
Fig.12 Function EMMI test 1000X picture of case Ⅱ

Based on EMMI result, physical analysis was performed and dislocation was found on DZsoft (Zener  diode). Result was showed in Fig.12.

![  Dislocation  SEMinspection  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f6eebe9b-4c20-4ffb-b943-c1ae6941b621/f6eebe9b-4c20-4ffb-b943-c1ae6941b621.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=6d6708b9578936b5aaf75c9e1af6dbbbb3323398)
Fig.13 Physical result of case Ⅱ

![SILBLK   SILBLK  Dislocation   DPN  location   HVNW  HV+  NWELL   NHV+  NWELL  TRENCH  NBL  Pepi-1  Crosssectionimaqe   P++Substrate    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/53508d88-38e1-4ca2-b844-579fbb41bd3f/53508d88-38e1-4ca2-b844-579fbb41bd3f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215651%3B1743219251&q-key-time=1743215651%3B1743219251&q-header-list=host&q-url-param-list=&q-signature=2388e1f57a2a994d9704305cbc0e0fa9e3b420c2)
Fig.14 Cartoon picture of defect location

## Ⅴ . SUMMARY  

For the new method it is efficient and successful for isolated to Zener diode failure cases instead of cutting the circuits to avoid damaged the chip and saving the cycle time.

## ACKNOWLEDGMENT  

For this work, I would like to thank for cooperation with    Power Tian, Haus Zhang,Jacky Wen and Xiaocui Li and the  support from PFA colleagues.

## REFERENCES  

[1] JCH Phang1,2, DSH Chan1, SL Tan1, WB Len1,  KH Yim1, LS Koh2, CM Chua2, LJ Balk3 “A Review  of Near Infrared Photon Emission Microscopy and  Spectroscopy”.

[2] JCH Phar\~g’.\~D,S H Chanl. M Palaniappanl.2,  JM Chin’.’, B Davis’, M Bruce’, J Wilcox’, G  Gilfeather’, CM Chua4, LS Koh4, HY Ng4, SH Tan4  “A Review of Laser Induced Techniques for Microelectronic Failure Analysis”.

[3] Li Tian, Kuibo Lan, Gaojie Wen, Xiaocui Li,  Dong Wang, ”Application of Voltage and Waveform  Forcing Method for Electrical Isolation of Complex  and Loop Circuit in Failure Analysis”.

[4] Li Tian, Xuejian Qian, Gaojie Wen, Jinrong Song,  Hao Zhang, Diwei Fan, Dong Wang, ”Application of  MOSFET Characteristic Measurement for Electrical  Isolation of Open Defect on Device Level in Failure  Analysis”.

