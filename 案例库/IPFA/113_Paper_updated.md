---
title: "113_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_3e5824d6eedaa678e94d3456c14ed3257295230462135641
file_size: 2985779
---

## Dual-Side Electrical Fault Isolation Workflow:  Enhanced Defect Site Determination In  Microcontroller Devices and Case Studies  

Azizul Hakem Zulkifli \*1 , Foo Loke Sheng 1 , Mohd Suhaimi Ab Ttaleb 1   Thianchai Phianpan 2 , Anusorn Khuankaew 2 , Weeraphong Koetkhwamsuk 2    1 Product Diagnostic and Quality Centre Kuala Lumpur, NXP Semiconductors,   2, Jalan SS 8/2, Sungai Way Free Trade Industrial Zone, 47300 Petaling Jaya, Malaysia  2 Product Diagnostic and Quality Center - Bangkok, NXP Semiconductor (Thailand) Co., Ltd.,   Changwattana Rd., Bangkok, Thailand  \* Phone : (+60)376692000, Email:  azizulhakem.zulkifli@nxp.com

Abstract  – In general, Electrical Fault Isolation (EFI)  techniques such as Photon Emission Microscopy (PEM),  Optical Beam Induced Resistance Change (OBIRCH), Laserassisted Device Alteration (LADA)/Soft Defect Localization  (SDL), in combination with probing activities, are critical to  isolate and localize the most possible fault location prior to  nanoprobing and physical analysis in the failure analysis (FA)  workflow. Depending on the wafer technology complexity, EFI  analysis can be performed either from the frontside of the die  or the backside of the die. This paper explores the idea of  combining the EFI techniques from the dual-side (frontside  and backside of the die) to acquire more valuable EFI data for  a concise conclusion in fault isolation followed by actual case  studies discussion to demonstrate the benefit of the dual EFI  methodology which pinpoint the defect region successfully.

Keywords—Frontside Electrical Fault Isolation, Backside  Electrical Fault Isolation

I.    I NTRODUCTION :   F AILURE  A NALYSIS IN  D EFECT  F INDING

The success of the defect finding highly depends on the  accuracy and precision results from the electrical fault  isolation (EFI) which help to pinpoint to suspected fault  location in the smallest resolution. The success of the failure  analysis (FA) finding will help to improve the quality of the  devices and to reduce the Part Per Million (PPM) return  levels. The typical EFI includes optical global fault isolation  such as Photon Emission Microscopy (PEM), Optical Beam  Induced Resistance Change (OBIRCH), Laser-assisted  Device Alteration (LADA)/Soft Defect Localization (SDL),  with combination of the signals investigation through  probing analysis, either from frontside micro-probing or  backside laser interaction of Laser Voltage Probing  (LVP)/Electro Optical Probing (EOP). The probing activities  help to backtrace the faulty signals to the originated faulty  node and narrow down the proximity area of the fault  location, which enhances the success of defect finding in  subsequent physical analysis.

![23  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/af75c2a8-1dee-4644-b1a4-59f12bdb37fa/af75c2a8-1dee-4644-b1a4-59f12bdb37fa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=a27348798fd0e1bc99738d33ee732a49c227c26b)
Fig. 1.   Micro-probing analysis able to reveal the voltage level, polarity  and signal response over the probing time span

The frontside micro-probing enables the analyst to  understand the voltage level, polarity and capable of  capturing the signal sequence until milli-seconds (ms)  ranges. It is very useful especially in analog circuity studies  in which the voltage level and the signal response during  device execution are critical to understand the behaviours of  the analog module (Fig. 1).  The backside probing such as  EOP/LVP can help to overcome the limitation of the  frontside Focus Ion Beam (FIB) probe point deposition due  to dense metallization, or due to package limitation, for  example flip-chip package devices.

The flip-chip package, is strongly emerging as a  promising choice for high density integration applications.  Key advantages of this advanced package are good electrical  performance and excellent thermal characteristics [1]. The  topside of the die is directly connected to the substrate  through the bump. This structure will inhibit any topside  analysis to be performed on the flip-chip package device  since any opening on the topside will make the unit cease to  operate. This will be a challenge to apply this flow for this  kind of package.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/dc327f2b-a5df-4560-b42b-5cafd921c746/dc327f2b-a5df-4560-b42b-5cafd921c746.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=3a07fac19c60882cfcb68d33d9453db6bf69d114)
Fig. 2.   Backside probing through the EOP/LVP can investigate the  switching activities of the transistors but is unable to identify the voltage  level and polarity.

Unlike frontside micro-probing, LVP/EOP activities  only capture the switching activities of the transistor. The  voltage amplitude only represents the measured reflected  laser /light source, but not the actual voltage level or polarity  (Fig. 2). In addition, the time span for LVP and EOP is  preferable in micro-second (µs) ranges [2], thus limiting the  analysis for the failure occurred after reset or after lengthy  pre-conditioning setup.

II.   C ONCEPT OF  D UAL -S IDE  E LECTRICAL  F AULT  I SOLATION

## A.   Concept Origination  

The idea of dual-side EFI originated from the flash  failure analysis. There was an FA support request for the  charge pump failure which induced the flash erase issue. The

front-side FA approach was selected to investigate the charge  pump behaviours. Frontside PEM by continuously looping  the erase cycle or during power up did not observe any  abnormal emission spots. Active micro-probing analysis  revealed that the charge pump failure was due to missing  clock activities at the clock generator module inside the flash  region (Fig. 3).

Although the frontside analysis was able to confirm the  charge pump failure due to missing clock activities, it was  still unable to identify the origin of the failing node.  The  frontside active micro-probing to back-trace the missing  clock activities was limited by the accessibility of the FIB  probe pad deposition due to dense metallization. Hence the  frontside analysis was halted at this juncture with the missing  clocks conclusion.

![0000000  Good ClockA  BadClockA  GoodClockB  Bad Clock B  Good ClockC  Bad ClockC    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8927d5c0-a6a2-4744-924d-b7dd566a48ad/8927d5c0-a6a2-4744-924d-b7dd566a48ad.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=fe204fb826581da6714394924ca74b18526d35db)
Fig. 3.   Micro-probing analysis observed missing clock activities

A circuitry study based on the frontside analysis  suggested that the power domain for the clock generator is  supplied by VDD_FLASH. Further fault isolation can be  continued through backside Electro-Optical Frequency  Mapping (EOFM) by modulating the VDD_FLASH to  understand the other clock activities which were not able to  be probed from the frontside. EOFM is capable of  identifying the missing clock activities inside some clock  drivers (Fig. 4). By overlaying the layout with a combination  of circuitry studies, the failure was suspected due to open  routing at the VDD_FLASH signal. Subsequent physical  analysis confirmed the failure due to Electrical Induced  Physical Damage (EIPD) at the suspected open routing (Fig.  5)

![Missing Activitie  Missing Activities       Badunit  Bad unit   Good Unit  Good Unit  \*EOFMIQ SuperimposeImage  \*EOFM I Q Superimpose Image    \*EOFM I Q Superimpose Image  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e9b46373-f02f-48e6-a736-ce4da700f565/e9b46373-f02f-48e6-a736-ce4da700f565.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=984e08ccdd8c44c55ecb8163f7533def420a1804)
Fig. 4.   EOFM observed missing clock activities inside the clock drivers

![  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0195a9fb-81db-4b83-920b-c97e1ec3f831/0195a9fb-81db-4b83-920b-c97e1ec3f831.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=7404224e187171c1333d83bf120b022a262f2d8f)
Fig. 5.   Scanning Electron Microscopy (SEM) inspection revealed signs of  EIPD at metal 2

## B.   Potential Fan-Out for Dual-Side Electrical Fault  Isolation   

The success of the FA in charge pump issue inspires the  idea and concept of dual-side EFI implementation in the  typical FA workflow. The dual-side EFI has the potential to  provide a concise conclusion in defect localization by  collecting sufficient EFI data from frontside and backside  fault isolation. In addition, microcontrollers nowadays are  designed to integrate the processor with communication  protocol modules, flash and memory modules, radar  modules, etc. into one single die for faster and higher  performance (Fig. 6). Although the current typical FA flow  and EFI tools in the market are leaning towards backside  approach, the investigation of the voltage level and voltage  responses of a signal during die  execution  from the  frontside EFI is still critical to understand the module  functionality and behaviours (Fig. 7)  especially if the failure  is analog related, for example, Voltage Regulator issue,  Analog-to-Digital   Conversion   (ADC)/Digital-to-Analog  Conversion (DAC) issue, Flash issue, etc.

To have more functional modules embedded inside a  powerful processor, smaller technology wafer nodes and  multi-layer metallization are needed in the integrated circuit  design consideration [4]. Not all signals are capable of being  probed from frontside of the die due to FIB edit limitation. In  addition, the multi-layer metallization can absorb the  emission of the photon from layers beneath [5], and also  limit the laser interaction at the target region. Hence the  analysis from the frontside especially for analog-related  failure may not be able to isolate to suspected location for  subsequent nanoprobing and physical defect finding. Hence,  the concept of the dual-side EFI FA workflow has the  potential to overcome this limitation and improve the  resolution of the defect location isolation, especially in  microcontroller devices.

![520  1_40  292  140  3.00  200     i.Micro probing on the regular module to understand the voltage level.  i.Micro probing on the regular module to understand the voltage level.  3.60    ii. Micro probing on internal ADC ground to understand the noise level  ii. Micro probing on internal ADC ground to understand the noise level  during conversion.  during conversion.  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f9cc034a-4bf4-47ce-9b58-4ce94d0be365/f9cc034a-4bf4-47ce-9b58-4ce94d0be365.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=b5557039d87e20f8cf58700bf097eb5ccbe913ae)
Fig. 6.   Micro-probing analysis able to reveal the voltage level, polarity  and response over the analysis time span.

The   following   case   studies   will   discuss   the  implementation of the dual-side EFI in the FA workflow and  demonstrate the success in defect finding. The case studies  will discuss the frontside EFI followed by backside EFI  workflow in the analog failure and followed by dual-side EFI  in digital-related failure in which the FA approach starts  from the backside and continues to further isolate the fault  location in the frontside of the die.

## III.   C ASE  S TUDIES 

A.   From Frontside Electrical Fault Isolation to Backside  Electrical Fault Isolation

The first 2 case studies demonstrate the FA workflow in  real-time cases based on the concept discussed above. The  first two cases discussed in flowing prove how dual-side EFI  starts from frontside EFI and is followed by signal  modulation to further isolate the defect region using backside  EFI before physical analysis.

Case Study 1

![  SN1  SN1                                 Good unit  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/30a799d0-d81c-4cce-9775-393e01cb5c96/30a799d0-d81c-4cce-9775-393e01cb5c96.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=a1539bf545d1aab8a4b1f870a9c1b07f8caf6834)
Fig. 7.   Distorted Digital-to-Analog Converter (DAC) waveform reflected  on DAC output pins.

SN1 fails Digital to Analog Converter (DAC). One of the  register modules was failing and this was reflected through  the distorted output signal (Fig. 8). The SN1 was  decapsulated from the frontside to access the circuitry for  fault isolation analysis and active micro-probing purposes.

![   ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b4c2f7b4-5b53-458b-b70b-246b33f0aab9/b4c2f7b4-5b53-458b-b70b-246b33f0aab9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=81b1b7940f1a014ce243308a4ddf386ad6dbf24b)
Fig. 8.   Photon Emission Microscopy (PEM) did not reveal any anomalies.

PEM was performed by continuously looping the DAC  conversion, but no anomalous emissions were observed (Fig.  9). Area of interest is inside the red box. Frontside active  micro-probing observed that Signal A was faulty. The  investigation then focuses on the internal signal inside the  suspected module. However, those signals cannot be  accessed via frontside active micro-probing since covered by  power/ground routing from the top. Any FIB edit on that  power/ground layer will alter the state of the devices.

![This module cannot be  accessedfromfrontside  Module A   Module B   Module C  SignalA  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3258961c-a923-4a8c-b6b7-581eefaab763/3258961c-a923-4a8c-b6b7-581eefaab763.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=7c395a9a43cd84bb3e07da0ee3efb788f7cc72e9)
Fig. 9.   Frontside active micro-probing observed Signal A was faulty.

Since frontside active micro-probing concluded that  Signal A was faulty, code modification was performed to  modulate Signal A. Active micro-probing from the frontside  after code modification confirmed that Signal A for the good  unit was able to be toggled which met the criteria for  subsequent backside EOP or EOFM (Fig. 11) with a period

of 6.4µs (156.3KHz). For SN1, the Signal A was stuck at  high.

![Vidiv  alAstuckatH  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1d8bdfc4-829d-4469-8de1-dccd55222b56/1d8bdfc4-829d-4469-8de1-dccd55222b56.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=023d8cb75dbb9a08dc5792d1d4238b44b36ba0f6)
Fig. 10.   Frontside micro-probing after code modification.

SN1 was repackaged to facilitate backside analysis.  Backside PEM was performed by continuously toggling  Signal A. One abnormal spot was observed at the NMOS of  the driver for Signal A and an abnormal spot at the NMOS  site of the faulty module (Fig. 12). To have a better  understanding of the PEM result, backside EOFM was  performed to observe any additional activities of the  transistors. EOFM amplitude image observed abnormal  transistor switching activities at the NMOS and PMOS sites  inside the register module (Fig. 13).

![SI  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b481ab92-f2e3-4703-9c45-a07dafed9654/b481ab92-f2e3-4703-9c45-a07dafed9654.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=3f25041d4b9c21eb024181952e22fed511cab943)
Fig. 11.   Backside Photon Emission Microscopy (PEM) observed  anomalous emission as indicated.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/00bc1c4c-5fc1-4c15-9634-642d7c10c09a/00bc1c4c-5fc1-4c15-9634-642d7c10c09a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=64416e2c32225a0db09f06e090a49ef0d1e74600)
Fig. 12.   Backside Electro-Optical Frequency Mapping (EOFM) observed  abnormal transistor switching.

Both backside PEM and EOFM images were overlayed  with the die layout using Avalon software. Circuitry analysis  showed the anomalous PEM spot coincided with one of the  EOFM spots at the NMOS of the driver for Signal A. For the  remaining EOFM spots, abnormal switching activities were  observed at the internal clock (Clk & Clkb) regions (Fig. 14).  EOP was performed and observed high signal-to-noise ratio  (SNR) which indicates a short [6] at the Clkb driver inside  the register module B (Fig. 15).

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/11dcac95-0e7a-4af8-8280-6c8823085348/11dcac95-0e7a-4af8-8280-6c8823085348.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=c8399c36907a557c460977c9d1f967af611669b1)
Fig. 13.   Simplified circuitry inside the register module B with the location  of  EOFM and PEM spots observation region

![300.0μVIc  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/77993db5-276a-41d5-ab8c-81a6f0f186be/77993db5-276a-41d5-ab8c-81a6f0f186be.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=bfcff95b29e3bd57bef5aff5a61dc4b1b4273c65)
Fig. 14.   Electro-optical probing (EOP)  at the Clkb driver revealed  abnormal switching activities.

Since dual-side EFI successfully pinpointed the fault  location at the clock driver, SN1 was delayered to Metal 1  layer and nanoprobing analysis successfully identified one of  the faulty NMOS (source-drain short). Cross-sectional  Transmission Electron Microscopy (TEM) successfully  observed the source of the failing NMOS was burst and  shorted to the drain and gate (Fig, 16).

![  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d3694b32-d66f-4dec-9d07-5c19961245a1/d3694b32-d66f-4dec-9d07-5c19961245a1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=03dbc9e42d332b21fc0942acffce5e92800c2ea5)
Fig. 15.   Transmission Electron Microscopy (TEM) image observed the  defect at the failing NMOS.

## Case Study 2 

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f342970c-07df-42cb-976c-dbe18abd74be/f342970c-07df-42cb-976c-dbe18abd74be.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=47f1435bcccf1f40df4c42bab3ba58613b8c0803)
Fig. 16.   DAC_Output signal did not ramp out properly during DAC clock  startup and DAC pin setup.

SN2 is a device that failed DAC however the failure is  not as specific as Case Study 1 since there is no specific  failing sub-module detected during bench verification. The  DAC_Output did not ramp up properly during DAC Clock  startup and DAC pins setup (Fig. 17). The period of the  failing code was about 18.7ms (53.5Hz) which was not  suitable for backside EOP/LVP or EOFM/LVI. SN2 was  decapsulated from the frontside and PEM was performed

while running the DAC startup and conversion with missing  PEM emission spots observed (Fig. 18). Circuitry analysis  identified the missing spots are related to the fan-outs from  the DAC_ClkB signal (Fig. 19). Hence the Signal A,  DCA_ClkA and DAC_ClkB were selected for probing  analysis.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3cccbdc4-357e-4436-9471-499ac700684e/3cccbdc4-357e-4436-9471-499ac700684e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=c6676480197a3f071eea38b605375367698671d4)
Fig. 17.   Frontside Photon Emission Microscopy (PEM) observed missing  emission spots as indicated.

Frontside active micro-probing revealed that Signal A  controlled the DAC_ClkB and was unable to pull low during  the signal assertion and thus caused the DAC_ClkB to stuck  at high (Fig. 20). The active probing results correlated with  the PEM result where missing emission spots were observed  due to missing DAC_ClkB. After identifying that Signal A  was faulty, code modification was performed to modulate  Signal A with a   $75.3\upmu\mathrm{s}$   (14.2KHz) period to enable  subsequent backside frequency mapping and backside  probing analysis (Fig. 21).

![SignalA  Level   DAC_CIKB  ShifterA  DAC_CIKA    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3e8cdc1d-89d6-4924-8ef2-584c4716c879/3e8cdc1d-89d6-4924-8ef2-584c4716c879.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=3fe40c7015ca2b4ea2f65f90b6ab602712e6cf00)
Fig. 18.   Circuitry study revealed the missing PEM spots region.

![GoodSignalA  Good ClkA  oodClkB  DAC_CIkBstuck  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d1a8db79-2e20-4c86-a582-e40b1977524d/d1a8db79-2e20-4c86-a582-e40b1977524d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=5c69d618914dd3e9b4e040d3cb0790ecd88b3ff4)
Fig. 19.   Frontside Active micro-probing observed DAC_ClkB was stuck  with Signal A and was unable to pull low.

![ Good Sync  Bad Sync   Good Signal A  Bad Signal A     ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0513b07b-9baa-4f41-a674-8c08b629d161/0513b07b-9baa-4f41-a674-8c08b629d161.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=3652dbfefc4eee4e33ae3390d2bf8d9db48bc5b8)
Fig. 20.   Code modification enables Signal A to be toggled in micro-seconds  (µs) ranges.

The unit was repackaged and backside PEM was  performed by modulating Signal A under a Solid Immersion  Lens (SIL) and observed an anomalous spot at the subInstance A inside the level shifter B of the DAC module  (Fig. 22). Backside EOFM analysis was also observed  anomalous transistor switching activities inside the subInstance A (Fig. 23).

![000000000000000000  □□□□□  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/94d4aac4-65d4-4279-9388-673841f102af/94d4aac4-65d4-4279-9388-673841f102af.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=86ae9b7d5643bf9ff60cfdbf297edb55c8a0a4d3)
Fig. 21.   Backside PEM observed abnormal emission at inside sub-Instance  A inside the level shifter B

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/417d7c2e-5cf7-4439-a4e8-d09e64d180fd/417d7c2e-5cf7-4439-a4e8-d09e64d180fd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=c5e187b6d3dee34c8ef00acff86b63768fa247b2)
Fig. 22.   Backside EOFM observed abnormal switching activities at subInstance A inside the level shifter B.

Circuitry analysis revealed the PEM and EOFM anomalies  originated inside the Sub-Instance A of the level shifter B  (Fig. 24). EOP analysis was performed on the driver of  signal A and observed high Signal-to-Noise Ratio (SNR)  which indicated shorts within the sub-instance circuitry (Fig.  25). Since the sub-instance A was controlled by Signal B,  Signal C, and Signal D, hence it was suspected these controls  signals may faulty or short which case the Signal A unable to  pull low.

![Input   SignalB   SignalA  Signalc  SignalD  Sub-Instance A  Level ShifterB  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7a27a38b-56b3-41df-82af-59a6bb460541/7a27a38b-56b3-41df-82af-59a6bb460541.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=f4b65a1a258a6e57d2be71ba7ffd90fefd207813)
Fig. 23.   Partial simplified circuitry shows the EOFM and PEM anomalies at  the sub-instance A

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4a285c58-d2ae-45dc-97fa-244bc694035c/4a285c58-d2ae-45dc-97fa-244bc694035c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=0fd7f755000f23bd80eb58d598a6b469f4adc79c)
Fig. 24.   EOP analysis reveals high SNR at the driver of signal A.

The physical analysis for SN2 was further analyzed by  the wafer foundry lab. The unit was delayered and at each  layer, inspection was performed via Scanning Electron  Microscopy (SEM). No gross anomaly was observed until

the Metal 2 layer. A metal defect that shorted Signal B and  Signal C with respect to the ground was observed (Fig. 26).

![etal  Metal  Defect  Defect  SignalB  Signal B  Signal C  Signal  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cd9bece0-115a-4f74-8497-ecf61b26f914/cd9bece0-115a-4f74-8497-ecf61b26f914.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=cd07088956b9670b14ae11bea5e6863a257af8f3)
Fig. 25.   Illustration of the failure mechanism using Avalon software.

B.   From Backside Electrical Fault Isolation to Frontside  Electrical Fault Isolation

Besides starting the FA approach from the frontside  followed by the backside as discussed in Case Study 1 and  Case Study 2, the concept of the dual side EFI can be  implemented for digital analysis where the FA approach  starts from the backside. The following case studies  demonstrate how the concept of dual-site EFI further  enhances the localization of the defect region starting from  backside EFI to frontside EFI.

![SignalA  SignalB  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/24707a22-fe61-4b50-b2bf-897b8f70c79d/24707a22-fe61-4b50-b2bf-897b8f70c79d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=956700609e96bef8b97cb8e01886f52f30b65648)
Fig. 26.   Electro-Optical Probing (EOP) suggested that Signal A and Signal  B were shorting to each other

SN3 was failing general-purpose I/O in which one of the  pins was unable to pull low. Backside global fault isolation  by continuously looping the failing patterns observed  abnormal emission spots The abnormal emission spots  suggested unexpected toggling in one of the signals B. EOP  analysis suggested possible short in between the control  signal A with the adjacent signal B (Fig. 27).

![     ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a96c208c-3532-4958-875e-4a596027cb66/a96c208c-3532-4958-875e-4a596027cb66.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=134d6db449a51a7eb915403a0f9dff3bd85ba01c)
Fig. 27.   Frontside static fault isolation confirms the short and OBIRCH  observed the abnormal spot.

To confirm the hypothesis of adjacent signal shorts, SN3  was decapsulated from the top and followed by FIB-edit for  probe pad deposition at both signals. Passive probing  confirmed the short and subsequent topside ORBICH  analysis by biasing the faulty signals and observed 1  abnormal spot (Fig. 28). Subsequent FIB cross-sectioning  analysis revealed a metal defect that shorted the faulty  signals at the OBIRCH spots region (Fig. 29).

![     ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b2c13959-06fe-43aa-a8e1-ec1e490525f1/b2c13959-06fe-43aa-a8e1-ec1e490525f1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=3d60997015864bef6b512196548464fba34b34d1)
Fig. 28.   Sign of metal defect at the OBIRCH region for unit SN3 during  FIB cross-sectioning.

## Case Study 4  

Case Study 1 and Case Study 2 revealed that from the  frontside active micro-probing, the signals of interest can be  identified.   Modulation   of   the   signals   with   coding  modification helps to reduce the looping length into microsecond (µs) ranges to enable backside EOP/LVP and  EOFM/LVI purposes. For Case Study 3, the backside EOP  confirmed the suspected failing signals and static voltage  biases were applied to the suspected signals for OBIRCH  analysis. For the following Case Study 4, instead of static  voltage biases, a periodical external dynamic stimulus was  applied on the suspected faulty signal from frontside after  being isolated from the backside analysis and performed  EOFM from the backside simultaneously [7].

To perform the frequency mapping or other fault  isolation from the backside with external stimulus from the  top, a special setup or prober is needed. The probe station  needs to have a CCD camera from the bottom side for microprobing navigation purposes and an inverted probe card for  needle landing. Case study 4 was performed under this setup  (Fig, 30).

![Enun  Signalinjection       (Toptical imaDUT)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1efe6c92-d20e-4b67-92c2-ce4f85fa2541/1efe6c92-d20e-4b67-92c2-ce4f85fa2541.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=0d729fd89863ade9eceb972e225922b9a23f0561)
Fig. 29.   Back side EOFM with frontside micro-probing assisted for signal  direct injection.

EOFM analysis can detect signals which coupling  through capacitors. An external stimulus can be injected into  the suspected open net without any power supplies to the  Device Under Test (DUT) and use EOFM to detect  switching activities at fan-out branches. EOFM signal is  expected at the gate-bulk of NMOS (which is bulk connected  to GND) of the interested net under normal conditions (Fig.  31).

![Driver   out#  Signalinjection  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/62da0b8a-f78e-4060-9ca1-fbb984168f32/62da0b8a-f78e-4060-9ca1-fbb984168f32.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=abf8da139699b98189d9d39e42ecf548a997c796)
Fig. 30.   Schematic diagram shows the expected EOFM signal at gate-bulk  at NMOS transistors of the interested net

SN4 is a device with a communication issue. Backside  PEM was performed and one abnormal emission spot (Fig.  21) was observed. Layout study revealed that the extra  emission spot was originated from the NMOS transistor  inside an inverter which gated by Signal A (Fig. 32).

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6450398c-0d7b-413f-a432-5a919bf1bd3e/6450398c-0d7b-413f-a432-5a919bf1bd3e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=078b5a557e9c49987b7fec7b2a1899248d556d6c)
Fig. 31.   Frontside PEM observed 1 abnormal emission spot as indicated  while looping the failing coding

![MP2  Driver   Fanout#1  SignalA  Signal A  MN1   +PEM  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/96d82c8f-f117-490f-a2c7-8466f02e49a4/96d82c8f-f117-490f-a2c7-8466f02e49a4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=cfea1eba36af82f8c0f7606a3c6c6fff598a3f8d)
Fig. 32.   The extra PEM spot was observed at the NMOS transistor inside an  inverter which was driven by Signal A.

SN4 was then decapsulated on the topside and one FIB  probe pad was deposited at Signal A for micro probing  purposes. Unpowered passive probing was performed on  Signal A with respect to Vdd and Vss respectively but no  abnormal diode curve characteristics were observed.  Frontside active micro-probing by looping the failing code  observed different timing responses during code execution  with no sign of voltage level degradation or sign of crosstalk  (Fig. 34).

![Good  GOOC  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e87ddcc9-eb97-4fe6-a3eb-a7dde106be35/e87ddcc9-eb97-4fe6-a3eb-a7dde106be35.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=651ed064e87b2dfce17f2059598749d8a9210eb2)
![SN4  SN4  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/213e8b52-d5c4-4d4c-921c-0536fefbecd2/213e8b52-d5c4-4d4c-921c-0536fefbecd2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=07c23aacb0829ea37c58a254802c778adb23b841)
Fig. 33.   Frontside active probing at Signal A revealed different timing or  periods of the signal responses during code execution.

After circuit and layout analysis based on frontside  micro-probing electrical behavior and PEM result, an open  circuit at Signal A was suspected. To prove this hypothesis,  an external periodic stimulus was injected into Signal A  through a frontside probe, and backside EOFM analysis was  performed simultaneously. Since Signal A was unable to be  modulated using coding, hence an external stimulus signal  was needed for EOFM purposes. EOFM result showed  missing switching activities on the fanout of the suspected  net which confirmed that Signal A was open (Fig. 35).

![SN4  SNA  Good  Downstreamedfanout  GOO   Fanout   SN4  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6cb018e8-e762-4d77-a31f-e29ef32c2115/6cb018e8-e762-4d77-a31f-e29ef32c2115.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=f5653cb0a05beb6ae96838e2006720d981c95f99)
Fig. 34.   EOFM result showed missing switching activity on the failed  device.

FIB cross-section was performed at the suspected open  location. The result revealed a high ohmic contact structure  at VIA3 between the Metal 4 and Metal 3 layers (Fig. 36)

![NE3    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/24df5905-45fd-4c29-b165-056a1c11a6e7/24df5905-45fd-4c29-b165-056a1c11a6e7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=7d061673dcdd6d4696a69e82695127fe0ec21b49)
Fig. 35.   FIB cross section showed open VIA3 for Signal A.

The similar dual EFI techniques in Case Study 4 can be  expanded to the faulty signal with multiple fan-outs.  Backside EOFM/LVI by signal injection from frontside on  the identified open signal would easily help to identify the  open branches visually instead of backside EOP /LVP in  each fan-out (Fig 37).

![river   anout#1√  ut#2  LnunE   oper  nout#4√  Signal injection    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9d13518a-d421-4f2a-b5b8-362a4298c3ef/9d13518a-d421-4f2a-b5b8-362a4298c3ef.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=937123e5dd810dfb1647dd033562f524c59fc045)
Fig. 36.   EOFM with signal injection on the multiple fanouts net which  might point to the failed fanout in single EOFM scanning as an alternative  solution of using EOP to trace each net one by one.

## IV.   I MPLEMENTATION OF THE  D UAL  S IDE  E LECTRICAL  F AULT  I SOLATION    

FA engineers need to perform multiple fault isolation  techniques to localize the fault location before subsequent  nanoprobing and defect finding through physical analysis.  The case studies shared in this paper demonstrate the  success of dual-side EFI in localizing the fault location and  thus help the success in subsequent failure mechanism  determination.  Due to the FA success, the dual-side EFI  concept has been implemented in the FA workflow to  enhance the fault location and increase the defect finding  success rate (Fig. 38). The implementation of the dual-side  EFI into FA workflow will help the analysts to maximize  the coverage of fault isolation in dual-side and help to  conclude the suspected fault location in smallest resolution  which enhance the success for defect finding.

![fonalFailureCasesSubmissior  res  to trace orfailure  res  ical fault isolation on  stimulus to further  Physical analysis  noprobing  suspected sign  Yes  Physical analysiswith Nanoprobing     ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ef105b6f-b7c8-4b57-951f-b11ac9241dcb/ef105b6f-b7c8-4b57-951f-b11ac9241dcb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215826%3B1743219426&q-key-time=1743215826%3B1743219426&q-header-list=host&q-url-param-list=&q-signature=8e36835fb4448b92a5e063410b8c6fe3a054ddf3)
Fig. 37.   Dual-Side Electrical Fault Isolation workflow

However, the dual-side EFI workflow does not apply to  any Flip-Chip devices due to the design or structure of the  package is impossible for front-side analysis [8]. Else for  other packages, such as LQFP or BGA devices, are capable  of utilizing the dual-side EFI methodology as long as the  devices can be chemically decapsulated for frontside analysis  and have the repackaging and sample preparation readiness  for backside failure analysis purposes. In terms of the EFI  techniques, there is no limitation to the techniques used in

either the frontside or backside. The key concept of the dual  side EFI is that the signals of interest need to be identified  either from frontside or backside by using any EFI  techniques, and these signals of interest can be used for  further isolation from the opposite side to localize the suspect  fault location in smallest resolution.

## A CKNOWLEDGMENT  

The author would like to express his special thanks for  the effort of collaboration between NXP Product Quality  Labs in Malaysia and Thailand. In addition, the author would  like to appreciate the Physical Failure Analysis team in both  labs for further isolating the fault location using nanoprobing  and continuing the defect finding using FIB cross-section  and TEM. Furthermore, appreciation also dedicated to  Product Engineering team NXP Malaysia and Thailand in the  failure mode verification and program code modification.

## R EFERENCES 

[1]    X. Wenjun, C. Yusheng and Y. Quanbin, "Flip chip CBGA package  design and simulation," 2013 14th International Conference on  Electronic Packaging Technology, Dalian, China, 2013, pp. 555-558,  doi: 10.1109/ICEPT.2013.6756533. keywords: {Electronic packaging  thermal   management;Flip-chip   devices;Resistance;Heat  sinks;Inductance;Software;Capacitance;CBGA;electrical and thermal  simulation;Flip chip package},    [2]    KA Serrels, U Ganesh, T Gandhi, “Laser Voltage Probing of  Integrated Circuits: Implementation and Impact”, Microelectronics  Failure Analysis: Desk Reference, 244-261.    [3]    L. C. Lu, "Semiconductor Evolution for Chip and System Design-From 2D Scaling to 3D Heterogeneous Integration," 2022  International Symposium on VLSI Design, Automation and Test  (VLSI-DAT), Hsinchu, Taiwan, 2022, pp. 1-1, doi: 10.1109/VLSIDAT54769.2022.9768086.    [4]    Lucien Diego Laude, Konstantin Kolev, Claudio Dicara, Catherine  Dupas-Bruzek, "Laser metallization for microelectronics and bioapplications,"   Proc.   SPIE   4977,   Photon   Processing   in  Microelectronics and Photonics II, (17 October 2003.     [5]    Ryan Xiao, William Wang,Ang Li, Shengqiu Xu,Binghai Liu, “Case  Study of Electro-Optical Probing Signal with High Signal-Noise  Ratio[C]”, ISTFA 2019       [6]    Damrong Korbsrisawat, Foo Loke Sheng, “Signal toggling in  EOFM/EOP application as a novel bulk localization technique for  analog devices failure localization,” 2017 IEEE 24th IPFA, Chengdu,  China.    [7]    M. Paniccia, T. Eiles, V.R.M. Rao, and W.M. Yee, “Novel Optical  Waveform   Probing   Technique   for   Flip   Chip   Packaged  Microprocessors,” Proceedings International Test Conference, pp.  740, 1998.

