---
title: "187_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_76eae7fb5b65aef92d2ee185fa3ce3657295230462135641
file_size: 353646
---

## Analysis of a novel EOS failure due to stray voltage  during ICT testing  

Weiwei Zhang \* , Yi Zhang, and Yuanxin Lee  Failure Analysis Team, H3C Technologies Co., Limited, 446 Changhe Road, Hangzhou, China.  \* Phone: +86-571-86761878   Fax: +86-571-86762705   Email:  Weiwei_zhang@h3c.com

Abstract-   Damages from Electrical Overstress (EOS) are the  leading reason of returns of integrate circuits and systems that  have failed in PCB assembly or final field. While a wide variety of  root causes could result to EOS damage, it is difficult for analyzers  to find the real root cause and provide effective improvements  base on root cause identification [1]. This paper will discuss a  novel EOS failure during PCB Assembly due to stray voltage of  ICT testing. Finally, a new design of ICT program is proposed to  resolve the problem.

Keywords  –  EOS, stray voltage, ESD, ICT test .

## I. I NTRODUCTION 

For over four decades, EOS has been one of the top reasons  of returns for integrate circuits and systems. Base on a survey  on EOS done by JEDEC [1], the most common cause of EOS  events is powered handling. EOS events may also relate to  overstress-induced phenomena when power is turned on,  incorrect power supply sequence, electromagnetic interference  (EMI), or hot plugging [2-6].   Although it has been clearly  established that component ESD target levels are not related to  the rate of EOS damage, other forms of ESD have been  observed at the system level and reported to contribute to the  conditions causing EOS. These include charged board or  charged cable events, system level events, discharges from  charged devices, and ESD controls in manufacturing which are  not compliant with handling ESDS devices [7-10].

In this case, a serial of CPUs’ power pin was found low  resistance during ICT test after components mounted on the  PCB. Failure Analysis was proceeded immediately as the  urgency of main production. The PFA conformed low  resistance of the power pin on CPU both on the main board and  after detached. 3D X-ray was used to find the corresponding  bonding pad and then LC was executed to locate the abnormal  position. Anomaly was not found on surface of the die after  de-capsulation.  EOS spot was found at the locating point while  de-process to M1.

It was determined the ICT process should be the possible  source of EOS by production review as all CPU were tested to  be normal before ICT test but found power pin low resistance in  ICT or FT (Final test). Checked the ICT instrument, no  abnormal high voltage or electrostatic charge was found during  the test.

Referring to the electrical specification of the chip, the power  on ramp rate control is required to avoid falsely triggering the  ESD circuitry. It was supposed that some stray voltage on the

ICT equipment or the PCBA, result in EOS damage via the  non-linear ramp while ICT power on. To resolve this problem, a  new designed ICT test program was released to eliminate the  stray charge before test.

## II.   ANALYSIS  

There were hundreds of CPUs used and 5pcs were reported  failure. On board test showed that CPU_MVREF voltage was  only 0.4 volt while normal voltage is 0.75 volt. Resistance test  showed that CPU_MVREF to GND was 28.6 ohms while  normal resistance is 110 ohms. The Board level isolation shows  CPU CPU_MVREF pin low resistance. The CPU was detached  from PCBA to do physical analysis. No abnormal was found by  external inspection of the failed chip (shown in Fig. 1).  Electrical   test   confirmed   the   resistance   of   pin   R6  (CPU_MVREF) was lower than good chips.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6db51362-3eed-4d41-a74b-c065361c39bf/6db51362-3eed-4d41-a74b-c065361c39bf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215643%3B1743219243&q-key-time=1743215643%3B1743219243&q-header-list=host&q-url-param-list=&q-signature=f28f8eaa06b6360faa4008195dd30ea42950db85)
Fig. 1 (a) Top view and (b) bottom view of the failure chip. Red arrow shows  the low resistance pin R6.

Before destructive analysis, 3D X-ray was introduced to  non-destructively check the position of bonding pad of R6, as  shown in Fig. 2.

![L4-3D  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2cbafdc6-7ba0-45d2-a9cd-6816f687c862/2cbafdc6-7ba0-45d2-a9cd-6816f687c862.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215643%3B1743219243&q-key-time=1743215643%3B1743219243&q-header-list=host&q-url-param-list=&q-signature=8913084d9c7dcc830dfbb7bd5455ff719ca9f113)
![L13D  2DXrayimage  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0848fc99-7833-4066-9a32-d485893f6c58/0848fc99-7833-4066-9a32-d485893f6c58.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215643%3B1743219243&q-key-time=1743215643%3B1743219243&q-header-list=host&q-url-param-list=&q-signature=b3c80564395ef116dd04a303cae32dee09380d3c)
Fig. 2 3D X-ray combined with real-time X-ray inspection to reveal the  corresponding pad of ball R6.

De-capsulation was executed and no abnormal found on  surface of the die, as shown in Fig 3. No burn mark or metal  discoloration was found through the surface by optical  microscope inspection. Liquid crystal was introduced to isolate  the hot spot. The hot spot was precisely under the bonding pad  of the failure pin, as shown in Fig 4.

![Fig. 4 Liquid crystal hot spot isolation.  Fig. 4 Liquid crystal hot spot isolation.   ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bdf225f8-2601-4feb-af14-42b574ace1c0/bdf225f8-2601-4feb-af14-42b574ace1c0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215643%3B1743219243&q-key-time=1743215643%3B1743219243&q-header-list=host&q-url-param-list=&q-signature=517895112c291a4bab4569dcbc5af9f850e49bca)
Fig. 5   De-layer to M1, EOS burn mark was found.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/33469641-fb55-4fdb-9181-6ea7329531eb/33469641-fb55-4fdb-9181-6ea7329531eb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215643%3B1743219243&q-key-time=1743215643%3B1743219243&q-header-list=host&q-url-param-list=&q-signature=fb2133bd6040e6fb72f7b2db673e7fb5f0fea6ac)
Fig. 3 Optical inspection image after de-capsulation.

Layer by layer analysis was introduced to found the defect  point. EOS burn mark was found after delayer to M1, as shown  in Fig 5.

## III. R ESULTS AND DISCUSSION 

As physical analysis verified EOS to be the root cause, the  origin identification of the EOS became the key point to solve  the problem. A small-lot production was released to verify the  ICT station. It was confirmed by AVO meter measurement that  all PCBAs’ resistance was normal after the chip soldering on  the PCB before ICT station. These PCBAs were sent to ICT test  and few of them showed CPU_MVREF to GND low resistance.  No abnormal high voltage or electrostatic charge was found on  ICT instruments during the production.

The CPU specification check showed that the power-on ramp  rate for voltage supplies was specified as linear ramp from 10 to   $90\%$   and the maximum changing rate is limited as TABLE I.  The ramp rate from 200 to  $500\:\mathrm{mV}$   is most critical as this range  might falsely trigger the ESD circuitry.

The schematic of ICT test setup in this case is shown in Fig 6.  In order to prove that the damage was caused by ICT test, many

investigations and simulations were carried out. Finally, it was  verified that EOS event often happens on the first testing after  changing probe station.

Some stray voltage might be on the ICT equipment or the  PCBA, result in EOS damage via the non-linear ramp while  ICT power on. A new designed ICT test program was proposed  to eliminate the stray charge before ICT power on. Small-lot  production was released to verify the correcting method. No  low resistance issue was reported after the new ICT program  change.

TABLE I.

P OWER SUPPLY RAMP RATE REQUIREMENT OF THE  C HIP

|Parameter|Min|Max|Unit|Notes|
|---|---|---|---|---|
|Required ramp rate for voltage supplies.|-|36000|Volts/Sec|1,2|
|1. Ramp rate is specified as a linear ramp from 10 to 90%. If non-linear (e.g. exponential), the maximum rate of change is critical as this change might falsely trigger the ESD circuitry. 2. Over full recommended operating temperature range.|1. Ramp rate is specified as a linear ramp from 10 to 90%. If non-linear (e.g. exponential), the maximum rate of change is critical as this change might falsely trigger the ESD circuitry. 2. Over full recommended operating temperature range.|1. Ramp rate is specified as a linear ramp from 10 to 90%. If non-linear (e.g. exponential), the maximum rate of change is critical as this change might falsely trigger the ESD circuitry. 2. Over full recommended operating temperature range.|1. Ramp rate is specified as a linear ramp from 10 to 90%. If non-linear (e.g. exponential), the maximum rate of change is critical as this change might falsely trigger the ESD circuitry. 2. Over full recommended operating temperature range.|1. Ramp rate is specified as a linear ramp from 10 to 90%. If non-linear (e.g. exponential), the maximum rate of change is critical as this change might falsely trigger the ESD circuitry. 2. Over full recommended operating temperature range.|


![Fixture Top  pueo  Probe station  DUT  Fixture Bottom  Control Card  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c10521c5-d584-4671-9aac-b04c42014897/c10521c5-d584-4671-9aac-b04c42014897.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215643%3B1743219243&q-key-time=1743215643%3B1743219243&q-header-list=host&q-url-param-list=&q-signature=8382dca8e4dcfd739438a7a96635e0c95517a5ad)
Fig. 6   schematic of ICT test setup in PCBA test.   IV. C ONCLUSION

[6]    K.T. Kaschani, Texas Instruments; R. Gaertner, Infineon Technologies  AG, “The Impact of Electrical Overstress on the Design, Handling, and  Application of Integrated Circuits”, EOS/ESD Symposium, 2011.     [7]    S. Ruth, M. Stockinger, J. Miller, V. Whitney, M. Kearney, S. Ngo, “A  CDM Robust 5V Distributed ESD Clamp Network Leveraging Both  Active MOS and Lateral NPN Conduction,” EOS/ESD Symposium  Proceedings, pp. 7-15, 2011.    [8]    A. Olney, B. Gifford, J. Guravage, A. Righter, “Real-World Charged  Board Model (CBM) Failures”, EOS/ESD Symposium Proceedings, pp.  34-43, 2003.     [9]    Noel, P.H., Dreibelbis, D.H., IBM Corporation, “EOS or ESD: Can  Failure Analysis Tell the Difference?”, EOS/ESD Symposium, 1983.    [10]   C H Tung, etal., “Physical FA to Distinguish EOS & ESD Failures”, IPFA  2002, pp. 65-69.

A serial of CPUs power pin was found low resistance during  ICT test after components mounted on the PCB. Physical  analysis identified EOS to be the root cause.  ICT process was  determined to be the source of EOS by production process  review. IC specification check found that the power on ramp  rate control is required to avoid falsely triggering the ESD  circuitry. Stray voltage on the ICT equipment or the PCBA  result in EOS damage via the non-linear ramp while ICT power  on. A new designed ICT test program was released to eliminate  the stray charge before test and the problem was resolved.

## R EFERENCES 

[1]    JEDEC Publication No. 174, Understanding Electrical Overstress - EOS,  pp. 15-33, 2016.     [2]    A. Righter, E. wolfe, J-J Hajjar, “Non-EOS Root Causes of EOS-Like  Damage,”  EOS/ESD Symposium Proceedings,  pp.312-317, 2014.     [3]    W. Farwell, K. Hein, and D. Ching, “EOS from Solder Irons Connected to  Faulty 120VAC Receptacles,”  EOS/ESD Symposium , 2005.    [4]    N. Peachy, R. Gauthier, R. Phelps, and E. Gebreselasie, “Transient  Latch-up of Switching Arrays in power management Circuits,”  EOS/ESD  Symposium Proceedings,  pp.152-160, 2012.     [5]    Richard Wong, Shi-Jie Wen, Rita Fung, and Paul Le, “System Level EOS  Case Studies not due to Excessive Voltages”, EOS/ESD Symposium,  2013.

