---
title: "119_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_2e5185b4c62cc10439b10f07c4616fb07295230462135641
file_size: 1203732
---

## Fault Localization on ICs by Function Based  OBIRCH Method  

Xuanlong Chen 1,2 , Junjun  $\mathrm{{Nu}}^{1}$  , Jiahao Liu 1 , Shengzong  $\mathrm{He^{l}}$  , Xiaoling Lin 1 , Gaoming Shi 1,2  1   China Electronic Product Reliability and Environmental Testing Research Institute, Guangzhou 511370, China  2   Reliability Research and Analysis Centre, China CEPREI Laboratory, Guangzhou 511370, China  Phone : (86-20) 32147640   Fax: (86-20)87237185, Email :  shigm@ceprei.com

Abstract —OBIRCH is commonly utilized in failure analysis  of integrated circuit as an electrical fault analysis method, it’s  based on static electrical test, mainly anomaly from  I - V   characteristics curve. For functional failures, OBIRCH is  supposed to be limited since the bias of function failures is  complicated, it’s hard to find a leakage current path by single  OBIRCH source. Function based OBIRCH is proposed to solve  functional failures and soft defects, the IC is electrically biased  by external power source, I/O signal and embedded source of  OBIRCH. The external source and I/O signal provide a testable  leakage path, and the leakage is detected by OBIRCH amplifier.  Results demonstrate function based OBIRCH is efficient in fault  localization of oxide defects or breakdown, even soft defect  sensitive to temperature.

Keywords—OBIRCH, fault localization, failure analysis,  integrated circuit, reliability

## I.    I NTRODUCTION 

Integrated Circuit (IC) is developing very fast in the past  few decades with scaling down. The failures are more difficult  to be observed, especially failures as subtle metallization  defects [1], gate oxide defects beneath polysilicon, foreign  materials, soft defect, and etc., the defects dramatically  decrease IC reliability. Some of these failures may result in  leakage current, which is supposed to be detected by  I - V   characteristic curve test, while most failures are functional  issues. Failure analysis (FA) is an efficient method to find the  root cause and improve the reliability of ICs, in which fault  localization is a crucial step [2].

Many static fault localization techniques have been  developed, such as Optical Beam Induced Resistance Change  (OBIRCH), Photon Emission Microscope (PEM), Lock-in  Thermography (LIT), etc. OBIRCH is typically performed  when leakage current was detected between two I/Os based on  the principle, it’s believed not suitable for function failure  analysis. Function failure is mostly started with PEM analysis  since the sample can be driven dynamically in various  electrical conditions or temperature [3]. However, as the  layers of metallization increase, the weak photon emission  might not reach the surface to be detected, some failures like  metal bridge might not emit photons, which makes PEM  limited in certain cases. To solve this problem, backside  analysis or dynamic analysis with testers is proposed, the die  substrate is exposed under PEM. Backside analysis needs  sample preparation, it might be complicated for some of the  advanced packages, such as wire bond ball grid array, ceramic  packaging, etc. Dynamic drive with automatic test equipment  (ATE) or evaluation board (EVB) is not always an FA tool  interface for laboratory environment lacking the ability,  therefore, it’s necessary to utilize the function failure analysis  method.

Since laser can penetrate several layers of metallization,  and OBIRCH can provide a power source, the source can also  act as one of the biases or signals in function failures or  dynamic situations. Therefore, frontside analysis for function

failures is possible by optimizing the OBIRCH technique with  a combination of external power source, I/O signal and  embedded source of OBIRCH. In view of the abovementioned facts, function based OBIRCH is proposed.

## II.   P RINCIPLES AND  M ETHODOLOGY 

Most of the defects would result in leakage current,  sometimes it’s easy to be detected only by  I - V  curve  characteristic curve test, as shown in Fig. 1, D1 represents  electrostatic discharge unit. In this situation, the leakage of D1  should be detected and OBIRCH is performed to narrow down  the failure.

![OBIRCHBias  Corecircuit  D1  Leakage  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e4f42371-6859-4296-be5d-b9a2187a6888/e4f42371-6859-4296-be5d-b9a2187a6888.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215828%3B1743219428&q-key-time=1743215828%3B1743219428&q-header-list=host&q-url-param-list=&q-signature=646a4b5dff9660c2fac10110e6188d46cd7c20b0)
Fig. 1.   Typical OBIRCH analysis bias method.

If the leakage current located in the core circuit, OBIRCH  analysis becomes difficult by single electrical drive. The core  circuit should be driven dynamically to find an abnormal  current path. Usually, the core circuit should be biased at the  failed mode by pausing the device at each test vector of the  failing functional pattern and measuring the voltage or current.  In general, there are three classical bias methods described as  follows and the method is known as function based OBIRCH  analysis.

## A.   Function based OBIRCH method  

(1) OBIRCH detecting power consumption is the first  application scenario. For a typical logic circuit consists of  inverters, as shown in Fig. 2, only if the core circuit is  correctly driven and transistor N1 is in the On-state, then the  leakage current of P1 can be detected by OBIRCH. The  OBIRCH bias should be between Vcc and GND, and  stimulate the device at a point of abnormal current  consumption. Leakage of N1 can be detected by the same  method as P1 is turned on, these two failure modes are similar  to each other.

![WCC  OBIRCH  bias  Biasedcorecircuitand   eakage  N1MOSFETisintheOn-State  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0072e62d-f539-4633-b21e-b192aa63a6b6/0072e62d-f539-4633-b21e-b192aa63a6b6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215828%3B1743219428&q-key-time=1743215828%3B1743219428&q-header-list=host&q-url-param-list=&q-signature=e414ac7248f55861e49a566eae6d28fbb576062d)
(2) I/O signal variation failures can be also detected by  OBIRCH technology. Some failures will change the output or  input voltage of ICs, resulting from a leakage current path  from output/input to VCC or GND. OBIRCH analysis should  be performed by creating a current loop with biased MOSFET  N1, as Fig. 3 shows.

![OBIRCHbias  across the output  Biasedcorecircuit and  N1MOSFETisintheOn-State  E1  T1  Leakage  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a31d5496-656b-43d5-bd0e-c127c14d87d2/a31d5496-656b-43d5-bd0e-c127c14d87d2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215828%3B1743219428&q-key-time=1743215828%3B1743219428&q-header-list=host&q-url-param-list=&q-signature=41416a94929413ba5c7530974d18e750f15ed055)
Fig. 3.   OBIRCH detecting I/O signal variation.

(3) Soft defect is another kind of failure modes, which is  affected by temperature, voltage, frequency and etc. [4, 5]. It’s  generally recognized that dynamic laser stimulation is suitable  for soft defect localization (SDL) and OBIRCH is a static  failure analysis method [6], however, some of the soft failures  will change the output or input voltage/current under high  temperature test, which makes it possible for OBIRCH  analysis for SDL. The change of input or output voltage would  transfer to the change of current, then the OBIRCH current  amplifier would detect the current alteration, and the  temperature sensitive area is marked. Basically, any kind of  parameter delivering some current or voltage change (e.g.  tester pass/fail outputs) should work with OBIRCH. Fig. 4  describes one of the failed situation applied to soft defect  localization, tester drives the device and the output is Vcc, as  the laser heat the failed area, output will drop from Vcc to  GND, and the current alteration is Vcc/R, the failed area is  marked. An example for such a failure will be shown in the  following chapter.

![ISM  Output  Biasl  Bias2  OBIRCH  Bias3   Amplifier  DUT  Tester  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/178b10e2-1721-4d09-859e-d5f037d0e544/178b10e2-1721-4d09-859e-d5f037d0e544.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215828%3B1743219428&q-key-time=1743215828%3B1743219428&q-header-list=host&q-url-param-list=&q-signature=2376d04704c7fbb9506300ec04484d6c4cc8c023)
Fig. 4.    Soft defect localization  setup.

## B.   Experimental setup   

The OBIRCH image was collected on a Hamamatsu  PHEMOS-1000, sample preparation and SEM images  recording were conducted on a Thermofisher Helios G4 CX  dual beam focus ion beam (DB-FIB) and Hitachi S-4300.

## III.   C ASE  S TUDY AND  D ISSCUSIONS 

A.   Case Study 1:Oxide defect induced power comsumption

The first case study was on a gate oxide defect of a CMOS  inverter input. The output voltage of the 16 bit A/D converter  was drop to GND for whatever analog input. No obvious  I - V   characteristic curve was found, and static photon emission  microscopy was performed under functional setup from front

side of die, no anomaly was found between failed and good  device. Then a setup of bias voltage according to the failed  mode was employed, as shown in Fig. 5, the pins which are  related to the control logic are biased either to GND or 5V.  The power consumption of failed device increased about 3mA  and OBIRCH was performed. The current amplifier was  connected to power (VDD and Vout) and ground. The  OBIRCH result demonstrated a control logic area related to  the failure phenomenon as compared with good reference,  shown in Fig. 6.

![5  50  GNDAVCCVDDGNDD   VoUT GNDD  DB6  DB8\~DB10  GNDA  DB14  VREFA/B/C   Cs  R  GNDA  EOC  FREE   STA-STCC  WB  GNDA   H/Ssel(  RANGE  V11-V16  D3\~\~D5  DT  D11\~D13  GNDA   D 15   VREFB  DO\~D2  GNDA  VREFC  SyPs  GNDA  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/23e41b86-d545-40ed-ad77-3cfc1bbaf389/23e41b86-d545-40ed-ad77-3cfc1bbaf389.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215828%3B1743219428&q-key-time=1743215828%3B1743219428&q-header-list=host&q-url-param-list=&q-signature=b3776249fc4d5198d70a1ddd79f4f3831a3a5e18)
Fig. 5.   Supply current consumption increased as the control logic circuit  was biased.

![  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5e11de3a-7ca1-4739-bf48-ae3b5b470f7f/5e11de3a-7ca1-4739-bf48-ae3b5b470f7f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215828%3B1743219428&q-key-time=1743215828%3B1743219428&q-header-list=host&q-url-param-list=&q-signature=8a71818917590673582e8d5d5bcb2d8cee613b1e)
Fig. 6.   OBIRCH result of failed device.

Physical failure analysis was performed to trace the defect.  The dielectric and interlayer metallization were removed until  contact, since no abnormal optical defect was observed,  passive voltage contrast (PVC) was carried out to examine the  leakage. Fig. 7 showed a bright poly connecting the gates of  three transistors, which suggests the leakage current is located  in gate oxide. Focus ion beam (FIB) was performed on the  three suspected transistors, the result showed that the gate  oxide was not homogeneous and oxide   void was observed (Fig.  8).

![mag口HV   cunr   ND   modedet   10pm  6500x1.00kV0.34nA4.1mmSE   ETD   Apreo2  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1a1d0021-9433-4136-af1c-a26afb98f4d3/1a1d0021-9433-4136-af1c-a26afb98f4d3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215828%3B1743219428&q-key-time=1743215828%3B1743219428&q-header-list=host&q-url-param-list=&q-signature=41ea5e41ecc3ccebbfb90e5407f9301eb00ff95d)
Fig. 7.   PVC result of the OBIRCH area.

![mag  OHV   curr   WD   modedet   300nm  200000x5.00kV0.34nA4.0mmSE   TLD   Apreo2     ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/27ec6264-d56c-4f83-853b-e2dc65c352b9/27ec6264-d56c-4f83-853b-e2dc65c352b9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215828%3B1743219428&q-key-time=1743215828%3B1743219428&q-header-list=host&q-url-param-list=&q-signature=cdcc6ae01abcc448afaf821973b3f992fe4aa29e)
Fig. 8.   Gate oxide defect of MOSFET.

B.   Case Study 2: Oxide breakdonw induced I/O variation

This case involves an eight channel analog multiplexers, it  failed for the output voltage is higher than expected, which is  close to the supply voltage, while the output voltage of the  good reference is 0V. Since no anomaly was found in   $I{\mathrm{-}}V$  characteristic test, a functional setup with various bias should  be consider priority. The abnormal output voltage is from  power supply, therefore, there must be a leakage from power  to output. OBIRCH can sense the current path, it’s necessary  to create a current loop. The designed test circuit is shown as  Fig. 9, a   $5.6~\mathrm{k}\Omega$   load gave a current path for OBIRCH. The  OBIRCH result demonstrated a leakage of gate oxide (Fig. 10).  After the polysilicon and oxide was removed, breakdown of  the channel was observed (Fig. 11).

A review of layout and schematic of failed area  demonstrates that the leakage is across gate and channel (with  bulk connected to -15V), not drain (output) to source of  NMOSFET. The gate is connected to internal control logic,  only when internal logic drive the NMOSFET, the leakage can  be detected.

![5Vor0V   Output  15W  DUT  OBIRCH  Amplifier   5.6kQ2  GND  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1e728426-3723-45b3-bab1-08617047044d/1e728426-3723-45b3-bab1-08617047044d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215828%3B1743219428&q-key-time=1743215828%3B1743219428&q-header-list=host&q-url-param-list=&q-signature=db190781bb08ab3ff642954b7dcd4053b528d622)
Fig. 9.   OBIRCH detecting I/O signal variation.

![  Fig. 10.OBIRCH result.  Fig. 10.   OBIRCH result.  SE   WD15.8mm10.0kVx20k   2UE  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c4ce50e8-59b3-4280-863b-e15bcd092c62/c4ce50e8-59b3-4280-863b-e15bcd092c62.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215828%3B1743219428&q-key-time=1743215828%3B1743219428&q-header-list=host&q-url-param-list=&q-signature=afd6526c6924024fcfca498244ee42638fb537fa)
Fig. 11.   Gate oxide breakdown.

## C.   Case Study 3: Soft defect of contact  

This case is a dual low-side MOSFET gate driver. The  delay time increased to 93ns at room temperature, while the  typical time is 23ns, as temperature rises, the delay time would  decrease to the typical value, it’s a typical soft failure. The test  results of the failed device at room temperature and high  temperature   $(50\ \ {}^{\circ}\mathrm{C})$   are shown in Fig. 12. At room  temperature tests, the delay time is longer. If the duty cycle  increased, the output voltage of the failed device would be  stuck at high. With slightly heating, the output voltage should  drop. We define that output stay high is failure, and output  drop to GND is pass, therefore, the heat causes fail to pass (F  to P), the issue can be transfer to soft defect localization (SDL).  The designed circuit is shown in Fig. 13. The period is 345s  and duty cycle is   $78\%$  , The output bias of OBIRCH was  equivalent with the device output (close to power supply), and  5.6k ohm resistor is to limit the current as a protect for  amplifier, as the laser heat reached temperature sensitive

circuit, it would alter the output voltage and OBIRCH system  would detect a current change.

![(a) 4.5V 6.0V 黎摄周期 →155.6000ns 最小值  最大值 2M0G次/秒 标椎差  18:1月42 3频率 (b)  168.4000ns  4.640y 4.5V +ST  △40.00000ns  △4.320V 6.0V 6:0 G次/秒 55.6000r  18：4月42022 最小值  最大值  标准差 3步  这现周其 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/de35b89e-4146-4e30-a03d-fe0c62dda520/de35b89e-4146-4e30-a03d-fe0c62dda520.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215828%3B1743219428&q-key-time=1743215828%3B1743219428&q-header-list=host&q-url-param-list=&q-signature=302c5fa59fc58beb94eb909339dabb2c7b284a79)
Fig. 12.   The yellow waveform is input and the purple waveform is output:  (a) room temperature, (b) high temperature.

![6.0  NCNC   9  INAOUTA  OBIRCH  GNDVs   FPE  H4  INBOUTB5  5.6kQ  4.5 V 345ns square wave  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e72a5373-71e7-46b6-89f3-1cda7c466df2/e72a5373-71e7-46b6-89f3-1cda7c466df2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215828%3B1743219428&q-key-time=1743215828%3B1743219428&q-header-list=host&q-url-param-list=&q-signature=342097dfe22f8633c482d6e34831975210197ae0)
Fig. 13.   Function based OBIRCH setup for soft defect localization.

OBIRCH results demonstrate that temperature sensitive  area is a contact, in which there is a sudden change of the  current alteration as laser heating (Fig. 14).

![(a)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7daccdf7-9f3d-4ca5-b2c9-9b65208ad47f/7daccdf7-9f3d-4ca5-b2c9-9b65208ad47f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215828%3B1743219428&q-key-time=1743215828%3B1743219428&q-header-list=host&q-url-param-list=&q-signature=f12ad3b048efc15ad8e13ddc9049dd7875d432f1)
![Cb  (b)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/13d2205b-3b3a-47fb-80a8-2d20e5ea0bc6/13d2205b-3b3a-47fb-80a8-2d20e5ea0bc6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215828%3B1743219428&q-key-time=1743215828%3B1743219428&q-header-list=host&q-url-param-list=&q-signature=7ae0366b0bded8b4dec428abf87b56c48f4101ee)
Fig. 14.    OBIRCH result for localizaiotn of contact.

## IV.   C ONCLUSION   

Function based OBIRCH method is proposed for fault  localization of functional failure and soft defect. The bias  based on external power source and I/O signal provide a  testable leakage current path, which makes OBIRCH possible  for fault localization in three typical application scenarios:  abnormal supply current consumption, IO voltage/current  variation and soft defect sensitive to temperature. Case study  demonstrates that gate oxide defect could be detected by  increased power consumption, and soft defect results in output  voltage drop is also detectable by OBIRCH.

## A CKNOWLEDGMENT  

The authors would like to appreciate failure analysis team  in China CEPREI Laboratory for support on root cause  finding. This work was supported in part by the Key-Area  Research and Development Program of Guangdong Province  under Grant 2022B0701180002, and CEPREI Innovation and  Development Fund No. 22Z04, which were acknowledged.

## R EFERENCES 

[1]    A.C.T. Quah, D. Nagalingam, S. Moon, et al., “Static fault localization  of subtle metallization defects using near infrared photon emission  microscopy,” Microelectron. Rel., vol. 73, pp. 76–91, 2017.     [2]    C. Hartmann, M. Wieberneit, “Layout analysis as supporting tool for  failure localization: Basic principles and case studies,” Microelectron.  Rel., vol. 48, pp. 1343–1348, 2008.    [3]    C. L. Wu, “Failure analysis of faulty vias or contacts in mixed-signal  integrated circuits,” Trans. Device Mat. Rel., pp. 568-573. 2018.    [4]    C. L. Wu, Z Linda, M Masuda, et al., “A novel method to realize soft  defect localization techniques without a synchronization signal for  failure analysis,” 16th IEEE Int. Symp. Phys. Failure Anal. Integr.  Circuits (IPFA), Suzhou, China, Jul. 06-10, 2009.    [5]    M. R. Bruce et al., “Soft defect localization (SDL) on ICs,” in Proc.  Conf. 28th Int. Symp. Test. Failure Anal., Phoenix, AZ, USA, Nov.  2002, pp. 21–27.    [6]    F. Beaudoin, K. Sanchez, P. Perdu. “Dynamic laser stimulation  techniques for advanced failure analysis and design debug applications,”  Microelectron. Rel., vol.47, pp. 1517-1522.

