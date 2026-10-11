---
title: "128_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_610d8b3a88ac787be5e0ca61cfe308c87295230462135641
file_size: 1536204
---

## Fault localization on Test Coverage and Functional  Issue for SoC Product with Combining Bench and  Pattern Test   

Li Tian 1 , Nan Xiao 1 , Ang Li 1 , Shijun Zheng 1 , Haijiao Bian 1 , Jianli Yang 1  1 Product Diagnostic & Quality Center in NXP Semiconductor, Tianjin, China  Email :  power.tian@nxp.com

Abstract —With the rapid development of System on Chip  (SoC) products, the structures and functions have become  increasingly complex. Failure analysis is crucial for discovering  design bugs and enhancing the quality of SoC products[1]. To  improve yield and screen out the defects, Automatic Test  Equipment (ATE) was particularly key tool to complete test.  Automatic Test Pattern Generation(ATPG) and functional  pattern on ATE were the most important test method for SoC  products to confirm whether the circuit has manufacturing  defects or not. In the meanwhile, the FA team often receives  failed products returned from customers with test coverage  issues, so that functional failure could only be duplicated on  evaluation board (EVB) platform in bench level. The failure  configuration is usually more flexible for debugging and  modification on EVB compared to the ATE tester. Based on  internal signal testability of ATPG pattern and configuration  flexibility of EVB test, in this paper novel failure analysis (FA)  workflow was proposed that combined bench and pattern  testing to complete failure investigation and fault localization  for test coverage and functional issues. And three real cases  were presented to demonstrate the effectiveness of this  workflow, that was beneficial in overcoming challenges,  improving the success rate and reducing analysis time for  complicated cases in FA.

Keywords—EVB, ATPG, Functional pattern, Test coverage,  Failure analysis

I.    B ENCH AND  P ATTERN  T EST  I NTRODUCTION

## A.   Bench Test with EVB  

The EVB is a specialized hardware platform that is  designed to evaluate the performance and functionality of a  particular chip. It typically includes all the necessary  interfaces and peripherals required to interact with the chip  being evaluated. The engineers in IC manufacturer often use  EVB to develop and debug own product, as it provide a  standardized platform for testing and evaluating new  technologies or products. Sometimes EVB allow engineers to  test components or systems quickly and easily without the  need for building a entire application system. Meanwhile  bench test with EVB is significant method to complete FA  when functional test coverage issue need to be localized root  cause for further wafer process or test improvement.

Some of the key features of EVB test include:

1. Standardized interfaces: EVB often have standardized  and user-friendly interfaces such as USB, HDMI, Ethernet,  DDR, UART, etc., which allow them to connect to various  components and systems.

2. Flexibility of function configuration: various specific  functional test setup can be flexibly changed with EVB in  failure debugging and investigation, for example bench code  customization based on FA requirement.

3. Full coverage of functional test: bench test with EVB  match to real application more closely, no matter one  specific module or system level test.

## B.   ATPG Pattern on Tester  

ATPG is a method used to detect manufacturing defects  in integrated circuits (ICs). It generates test patterns that are  designed to stress the circuit and reveal any latent defects.  These patterns use various techniques, such as random  pattern generation, fault simulation, and deterministic pattern  generation, to identify and classify faults based on their  testability and detectability[2].

Detectable characteristic is a measurement that a fault  can be observed on external scan output pins. Detectability is  influenced by the DFT circuit design, the fault model used,  the test patterns generated, and the observation mechanisms  implemented in the testing process. High detectability is  important to ensure that faults are accurately identified on  tester.

Testable characteristic refers to an internal signal or  circuit that can be tested by using test pattern. Testability is  an essential to generate appropriate ATPG pattern with high  coverage. If a net is testable, it means that both high(H) and  low(L) value can be transmitted and toggled to this net. Even  though one fault can be testable, and it still maybe not  detectable externally.

To improve the efficiency and accuracy for defect  detection, usually DFT design not only requires testability  for internal signal as much as possible, but also aims to  enhance detectability for these tests. As we known, once the  evidence from scan diagnosis or photo emission microscope  (PEM) / optical beam introduce resistor change (OBIRCH)  are available[3], FA engineer mainly perform further  analysis with advanced fault localization technique on  internal instance/device, for example electro-optical probing  (EOP) or electro-optical frequency mapping (EOFM).  Typically, FA team pay more attention to confirm the  testability on target signals during testing, regardless of its  detectability. Thus, it is sufficient to complete EOP  measurement if the target signals are merely testable, and the  detectability of fault on target signal is unnecessary.

## C.   Fucntion Pattern on Tester  

Function pattern in IC testing is a methodology to verify  functional characteristic of device under test (DUT). This  approach involves the application of specific patterns or  sequences of inputs to stimulate the device, then its  corresponding outputs or pass/fail flags were observed  externally. Any deviations or unexpected behaviours indicate  potential issues or failures in the IC's functionality. The goal  is to ensure the IC performs as designed and fulfil its

functional parameters. The function patterns are typically  designed in accordance with specifications and requirements  of the IC. These patterns may include sequences of digital  signals, analog stimulus, or combinations of both, depending  on IC circuit or subsystem design.

During function pattern testing, a set of predefined test  cases is developed, each representing a unique functional  scenario or operational mode of the IC. These test cases are  carefully crafted to cover all critical functionalities and edge  cases, ensuring thorough testing.

However, it is generally challenging to accurately narrow  down suspects using functional patterns, unlike with ATPG  patterns. In essence, functional pattern in IC testing is similar  to bench test, differing in the test platform utilized.

## II.   M AIN  S TRATEGY TO  C OMBINE  B ENCH AND  P ATTERN  T EST 

Traditionally bench test was only one solution to  complete FA for addressing test coverage issues, because all  test items can be passed on ATE, and it was flexible and easy  to configurate various setup by FA engineer based on  analysis requirement. However, the code execution was too  long to perform EOP waveform acquisition on internal cells  or signals sometimes. The longer loop period led longer time  in EOP waveform acquisition, meanwhile mechanical  vibration would seriously influence the measurement  accuracy within a long time, especially for advanced process  node or high-speed signals.

To overcome this challenge, a novel FA workflow was  proposed. Primarily bench test was utilized to investigate  failures for fault isolation in block level, and then  PEM/OBIRCH analysis was conducted to inspect abnormal  spots[4]. After abnormal spots were located on layout/  schematic and suspected signals/cells were traced, FA  engineer collaborated closely with the DFT team to simulate  waveform of relevant ATPG pattens in gate level to check  suspected signals/cells testable or not, regardless of the  availability of fault detectability.

If the appropriate ATPG pattern was available to toggle  suspects, it would be utilized to perform further EOP  analysis to isolate fault accurately. Since EOP setting could  be shortened effortlessly with ATPG pattern, target  signals/cells could be measured EOP waveforms efficiently  by using auxiliary ATPG pattern test on FA tester.  Additionally,   the   shorter   loop   cycle   enabled   the  observation for rise/fall edge issues more easily on highspeed signals. The flowchart in Fig. 1 provided a summary of  analysis approach for test coverage issues.

Furthermore, failed part was screened out by functional  patterns on ATE in manufacturing, which need FA team to  trace root cause. For this kind of failure primarily fault was  narrowed down into block or cell level with basic and  advanced FA techniques based on functional test pattern,  including PEM, OBIRCH, EOFM or DALS. When applying  functional patterns for fault localization, it was quite limited  to change various configurations for failure study due to poor  readability and flexibility of functional test pattern, it  sometimes necessitated support from test engineer to modify  or customize test pattern with long time. And it was  necessary to loop all vectors in the functional pattern to  ensure the component enter the normal state for waveform  measurement, so that it was difficult to complete EOP  waveform acquisition difficulty with long loop period.

![Test coverage failure  Test coverage failure    Auxiliary test  Auxiliary test  DFT simulate signal testable  DFT simulate signal testable  Primary test  Primary test  in which ATPG pattern  in which  ATPG pattern  Failure investigation and  Failure investigation and  narrow down with EVB  narrow down with EVB  EOP measurement with  EOP measurement with  specific ATPG pattern  specific ATPG pattern  Primary FA analysis by EVB  Primary FA analysis by EVB   (PEM, OBIRCH, DALS)  (PEM, OBIRCH, DALS)   Nanoprobing test  Nanoprobing test  Hotspot study on  Hotspot study on  layout/schematic  layout/schematic    Physical analysis  Physical analysis  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/eabde62d-25bd-4681-9efa-f3cf4d507f69/eabde62d-25bd-4681-9efa-f3cf4d507f69.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=3c06a328c8144504a899ecd85e364e69fe14468e)
Fig. 1.   Analysis flow for test coverage issue

To solve this issue, FA engineer employed auxiliary  bench test to setup flexible configurations or shorten test to   investigate failure and enable stimulation and measurement  of target signals within logical circuit. This approach  provided FA engineer with more electrical evidence to  localize faults accurately and facilitate effective analysis. The  analysis workflow for functional pattern failure was  summarized in Fig. 2, outlining the steps involved in this  approach.

![Functional Failure with  Functional Failure with   Auxiliary test  Auxiliary test  pattern test  pattern test  Functional setup on bench to  Functional setup on bench to  Primary test  Primary test   toggletarget signals/circuits  toggle target signals/circuits  Failure verification and  Failure verification and  investigation on FA tester  investigation on FA tester   EOP measurement with  EOP measurement with  various configuration   various configuration  Basic FA technology (PEM  Basic FA technology (PEM  &OBIRCH)  & OBIRCH)  Data analysis  Data analysis   Advanced FA technology  Advanced FA technology  (EOFM/DALS)  (EOFM/DALS)   Nanoprobing test  Nanoprobing test  Hotspot sutdy to isolate  Hotspot sutdy to isolate   Physical analysis  Physical analysis  suspicion  suspicion  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/45059cbb-1e35-4421-b3dc-d2b8a92fdade/45059cbb-1e35-4421-b3dc-d2b8a92fdade.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=e767310795e14ac56b94b2b53f8e5967b9c7a680)
Fig. 2.   Analysis flow for function pattern failure

In summary, FA engineers could maximize the benefits  of both bench and pattern testing in fault localization. By  leveraging the flexibility of the evaluation board setup  and  the testability of ATPG patterns, both the success rate and  analysis cycle time would be improved significantly. With  applying bench and pattern test partially on different failure  modes and test platforms, FA engineers could achieve  successful fault localization to trace root cause more  efficiently and accurately for meeting customer satisfaction  and enhancing quality.

## III.   C ASES  S TUDY 

## A.   Primary Bench Test and Auxiliary Pattern Test   

In first case the part failed double data rate (DDR) stress  test on bench, but it passed all test items at tri-temperature on  ATE. Product engineer (PE) and FA member duplicated  failure in FA laboratory by using DDR stress tool. It was  found that software hang occurred in reading operation.

In NXP FA there was the electrical localization  equipment PHEMOS-100 produced by Hamamatsu company,  that was equipped with an InGaAs camera, a 1340nm HLD  and a 1064nm HIL laser source, meanwhile solid immersion  lens (SIL) was used on 71X objective lens to observe the  semiconductor from backside with a high resolution,  enhancing maximum optical magnification to 250X. Main  techniques in electrical failure analysis (EFA) were enabled  within PHEMOS-1000, such as PEM, OBIRCH, EOP,  EOFM, and DALS.

In this case PEM analysis revealed one abnormal PEM  site with focusing interested DDR subsystem in SoC when  running function with bench setup, see the result in Fig. 3.  After checking power supply of PEM site static OBIRCH  analysis was performed with biasing relevant power supply.  As a result, two abnormal impedance change sites could be  identified, one of them (OBIRCH site2) was same location  as PEM evidence, while the other (OBIRCH site1) was the  upstream buffer of OBIRCH site2, hotspots were shown in  Fig. 4. By overlapping spot on layout and schematic, it was  determined the fail signal related to read response flag in  Advanced eXtensible Interface (AXI) bus of DDR subsystem.

![Abnormal PEM site  Mag:20X   Mag:250X  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/25fa682d-8c92-413c-bd9b-c8dbf94e021d/25fa682d-8c92-413c-bd9b-c8dbf94e021d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=4d34295cc528f1c1e329c4a47034e0f5b9e7ddf8)
Fig. 3.   PEM superimposed image, Condition: intialized DDR, run script  for DDR calibration and training, write and read data on specific address.

![OBIRCH  OBIRCH stie1   OBIRCH stie2  Abnor   hotspot   Abnormal hotspot   OBIRCH mag: 250X   OBIR   250X  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fb6dae0a-e2c2-4e8e-8c16-1afffd3b3767/fb6dae0a-e2c2-4e8e-8c16-1afffd3b3767.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=74c1271253e32472b3efcaa453f209b132d32e9f)
Fig. 4.   Static OBIRCH superimposed image, OBIRCH stie2 was same  location as PEM site, OBIRCH site1 was upstream buffer of OBIRCH  site2. Condition: bias AXI supply with 1V, VSS=0V.

Based on discussion with designer it was challenging to  toggle response flag signal to measure EOP waveform by  bench code or EVB configuration. Consequently, FA team  collaborated with design for test (DFT) team to perform gatelevel simulation on several ATPG scan patterns to detect  toggling on suspected signal. Fortunately, the toggling was  observed on target signal in specific vectors of one DCscan  pattern. Subsequently, EOP measurement confirmed that the  toggling on fail part disappeared on the buffers highlighted

by PEM and OBIRCH sites. The schematic and EOP  waveform were shown in Fig. 5.

![REF_buffer2  REF_buffer1  REF_buffero  RJT_buffer  RJT_buffer  RJT_buffer  2μs/div  (a) EOP waveform, no toggling on fail part  (a)   EOP waveform, no toggling on fail part  OBIRCHsitel   OBIRCHsite2  Responseflag  Buffer2  Buffer2   Bufferl  Buffer1   BufferO  Buffer0  EOPnormal    EOP abnormal   +PEM   ★OBIRCH  (b)   EFA result marked on schematic  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/88f0a1de-b75b-43a9-8e67-e27b9916bba7/88f0a1de-b75b-43a9-8e67-e27b9916bba7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=c0d17ce822392fd58c8c45b8e405bc1c9e51ceae)
Fig. 5.   (a) EOP measurement, (b) EFA result on detail schematic

After EFA completion the fail part was sent to perform  nanoprobing test to narrow down defective location  furtherly in physical. In our lab nanoprobing equipment was  nProbeII produced by Thermofisher Scientific, its main  function included DC measurement, C-V characterization,  Electron Beam Absorbance Current (EBAC), Electron  Beam Introduce Current (EBIC), Electron Beam Introduce  Resistor Change (EBIRCH), and Pulsing test. Open issue  was identified by invertor function test (sweep   $\mathrm{H->L}$   or L ${>}\mathrm{H}$  on input of buffer1, monitor output of cell), the curve  depicted in Fig. 6(a) shown buffer1 didn’t work normally.  Then an abnormal EBAC signal in Fig. 6(b) indicated the  precise location of the defect on metal2 line. Post removing  metal3 layer, metal open defect on metal2 layer was  observed on target signal (input of buffer1) with SEM  inspection eventually in Fig. 7.

![1.2  08  RJTL->H  %0.4  Wuffe roimvae   RJT_H->L  REFL->H  02  REEH->I  0.2  -0.5   D.s  (a) Nanoprobing invertor Function  (a) Nanoprobing invertor Function   (b)EBAC result indicated  (b) EBAC result indicated  test  confirmed  suspected buffer  test confirmed suspected buffer    accurate open defect location  accurate open defect location  worked abnormally  worked abnormally   on metal2 layer  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a66134e4-9ca5-4c96-9151-6862606fb4c1/a66134e4-9ca5-4c96-9151-6862606fb4c1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=40c703e9fdeed7300bfb99443664e7704a6cbd21)
Fig. 6.   Nanorpobing analysis, (a) invertor function test, (b) EBAC result  on target signal

![Metal2 oper  200nm 200mm    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f585c328-75ad-4399-9811-0d928ee9086d/f585c328-75ad-4399-9811-0d928ee9086d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=3ba5434ce14dd4072ffe456e504733ae8a2c57f5)
Fig. 7.   Physical analysis, open metal2 line was inspected by SEM

In second case the fail part was returned to FA lab to  investigate root cause due to DDR issue, which was the test  coverage issue. During failure verification unexpected data  was found in DDR stress test on bench level, meanwhile  calibration error also was detected with functional setup  provided by PE team. Then the failure was narrowed down  on internal interface between MUX and PHY for most  significant bit (MSB) 32-bits in DDR subsystem, as all test  could be completed normally with configuring low  significant bit (LSB) 32-bits data bus only. Verified and  investigated result was detailed in Table 1.

TABLE I.

F AILURE  V ERIFICATION AND  I NVESTIGATION

|Verification|DDR stress test|Calibration test|
|---|---|---|
|32bit data bus|Passed|Passed|
|64bit data bus|Failed|Failed|


After inserting infinite loop into bench test, the abnormal  PEM and OBIRCH sites were captured on three buffers in  suspected internal interface, detail result was presented in  Fig. 8. Three abnormal sites highlighted by PEM/OBIRCH  were located on three adjacent invertors in one buffer chain.  In this case there were two major challenges in blocking  EOP setting for further fault isolation with bench setup. First  was long loop cycle in bench coding that would result in  extending analysis cycle time and potential inaccuracies in  EOP measurements; second was unclear link between  external setting and internal target signals.

Therefore, DFT designer had to assist FA team to check  the toggling on target signals/cells by running gate-level  simulation on ATPG scan pattern. As a result, waveform  revealed the toggling on target signals in specific vectors of  one DCscan pattern. Then, distorted waveforms were  measured on suspected buffers by using EOP technique with  shortened ATPG pattern, the waveform result was shown in  Fig. 9. The electrical result information was annotated in  schematic shown in Fig. 10.

![bnorma  (a) （ap     Three unexpected PEM sites on adjacent invertors in one buffer  Three unexpected PEM sites on adjacent invertors in one buffer  chain, Condition: loop write and read one data on specific DDR  chain, Condition: loop write and read one data on specific DDR  address  Abnormal hotspot  Site2   Sites  Mag:20X  (b）Abnormal OBIRCH sites on same location as PEM sites,  (b) Abnormal OBIRCH sites on same location as PEM sites,  Condition: bias the internal interface supply with 0.9V, VSS=0V  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1fd588cc-1b5f-406d-8e2d-2fb58f3b5d5f/1fd588cc-1b5f-406d-8e2d-2fb58f3b5d5f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=1089f6a4816648f664b4c8ffcf25d313f61b212c)
Fig. 8.   Primary analysis, (a)PEM result, (b)static OBIRCH result

To   localize   defect   with   greater   precision,   I-V  characteristic measurement was performed on input signal  of site3 on upper metal layer during nanoprobing analysis,  which revealed open issue on target signal between probed

point close to site3 input and the driver of target signal.  Meanwhile open defect location was indicated accurately by  EBAC technique. Detail nanoprobing result was shown in  Fig. 11. Finally scan transmission electron microscope  (STEM) analysis observed metal line open in Fig. 12.

![REF input buffer  REF site3  REF_sitel  RJT_inputbuffer  RJTsite3  RJTsite2  RJTsitel  200ns  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5bf91fe1-9e4f-496a-b936-4fb6585bc1d4/5bf91fe1-9e4f-496a-b936-4fb6585bc1d4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=1b2d26023c92ae306f9860ed1c06666a5177fb39)
Fig. 9.   EOP result, abnormal waveform on three suspected invertors

![Site  EOPnormal   EOPAbnormal   OBIRCH site   PEMsite  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4bb98c96-208a-4241-8392-068a32036803/4bb98c96-208a-4241-8392-068a32036803.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=7a234fbca43f20f84976ee3cfd3b4faf52177f5e)
Fig. 10.   EFA result on schematic, three adjacent invertors highlighted by  PEM/OBIRCH and abnormal EOP waveform on them

![Abnormal EBAC signal  Abnormal EBAC signal  indicated defect location  indicated defect location  RTT  e1  Openo  1e-13  le-14  0.60.8  Voltage(V)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/dec0f01e-2d7d-4c9f-a6f3-0472c9d089fe/dec0f01e-2d7d-4c9f-a6f3-0472c9d089fe.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=54b2e961f4337376cfb9970f4511449bdba4a3de)
Fig. 11.   Nanoprobing result, (a) I-V characteristic measurement, (b)   EBAC  analysis

(a) 2points IV curve between site3  input and vdd/vss, sweep voltage:   -1\~1V, clamp current:100 uA

(b) abnormal EBAC signal  disappeared from one via4,  open issue suspect on via4 or  metal5 line

![STEM image-BF  Pt coating  T16  M5 defect  M4  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ac0cdbf3-0957-418d-b02b-36cb3f0f0fe4/ac0cdbf3-0957-418d-b02b-36cb3f0f0fe4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=f88b842ed81612d26ff4034233ae3038062a3520)
Fig. 12.   Physical analysis, metal defect induced by random particle caused  open issue

B.   Primary Pattern Test and Auxiliary Bench Test

In the third case General Purpose Input/Output (GPIO)  functional failure was screened out through pattern test on  ATE and it was duplicated on FA tester, the fail log was  shown GPIO output error on four pins in Fig. 13. No  abnormal shmoo boundary was observed when sweeping  supply voltage and test period in functional pattern test.  During PEM analysis several abnormal emission sites were  captured in circuit related to GPIO function, which were  associated with different GPIO pins in Fig. 14(a), and  abnormal OBIRCH sites were detected on nearly same  locations as PEM result with biasing supply in Fig. 14(b).  With the study and alignment in cross team, failure on  ESAI0_SCKT was suitable candidate for further analysis,  since the error on this pin was reported by customer.

![Cycle   Timing   Failing Pins  Failed GPIO  Failed GPIO  386538   40991   TS1_EQNSET_10   pNOXTALS Repeat   ESAIO_FST:L  386986   40999   TS1EQNSET10  _pNOXTALS Repeat   ESAIO_SCKT:L  387434   41007   TS1EQNSET 10  PNOXTALS Repeat   ESAIO TX1:L  387882   41015   TS1_EQNSET_10   pNOXTALS Repeat   ESAI0_TX3_RX2:I  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ae0567d6-d097-4393-95a7-2fd5ca3217d7/ae0567d6-d097-4393-95a7-2fd5ca3217d7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=2160bb33d8c096e4ae73323a4696eb93c6fa5c70)
Fig. 13.   Faillog of function pattern test, GPIO output failure on four pins

At the start of test pattern, tester loaded source code  (named Coremark code in NXP) into tightly-coupled  memory (TCM) within system controller unit (SCU) on SoC,  then move pointer to execute functional test. When  configuring a loop test in pattern for EOP measurement, the  loop cycle was too long to complete EOP waveform  acquisition because test sequence must include RAM  loading step for Coremark code, that caused test loop period  was quite long. Thus, FA engineer considered to toggle  suspected buffers with modified code on bench level.

![Abnormal PEM sites  Mag:20X  (a) （a)     Several abnormal PEM sites related to different GPIO pins,  Several abnormal PEM sites related to different GPIO pins,  Condition: in function pattern set GPIO as output, write 0  Condition: in function pattern set GPIO as output, write 0  & 1 in data register, then output data to GPIO pins  & 1 in data register, then output data to GPIO pins  Abnormal OBIRCH sites  Mag:20X  (b) Several OBIRCH sites nearly same as PEM result. Condition:  (b) Several OBIRCH sites nearly same as PEM result. Condition:  bias supplywith 1.1V,VSS=0V  bias supply with 1.1V, VSS=0V  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0ede4405-5d86-478c-a434-ac903512e090/0ede4405-5d86-478c-a434-ac903512e090.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=4820c6c760f107d6f5bda6d361cea1a4c627c090)
Fig. 14.   Primary analysis, (a)PEM result, (b) static OBIRCH result

Based on code customization in bench test the target  signals were stimulated properly and loop trigger was  generated successfully. EOP analysis revealed no data or  pulse on target signal efficiently by customized bare-metal  code with about 13.9us loop period. It was significant to  reduce time consumption on functional pattern debugging  and EOP analysis. The EOP result and detail schematic were  shown in Fig. 15 & Fig. 16 respectively.

After conducting a physical failure analysis SEM image  shown open issue on target signal and metal defect affecting  adjacent signals on metal5 layer in Fig. 17. With further  study these impacted signals were related to all four pins  failed on ATE and highlighted by PEM/OBIRCH, so the  metal defect on metal5 was the root cause to explain all  evidences in EFA step regarding GPIO output failure.

![One test loop  One test loop   One test loop  One test loop   One test loop  One test loop  REF Buffer1  REF_Buffer_2  REFBuffer  (a)  REF_Buffer_4  2μs/div  RJT_Buffer_1  RJT_Buffer_2  RJT_Buffer_3  RJTBuffer4   No toggling  2μs/div    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/75e1e9dc-d324-4349-98eb-0b6c5278a8e5/75e1e9dc-d324-4349-98eb-0b6c5278a8e5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=0d6c1b0aa810259f291ff743ca8cf2756fb0c2a3)
Fig. 15.   EOP result, abnormal waveform on the suspected invertor and  downstream buffer.

![Buffer_1   Buffer_2   Buffer_3   Buffer_4  EOP Normal   EOP Abnormal   OBIRCH site   PEMsite    ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c87863df-8391-432a-96da-5e42404e0d28/c87863df-8391-432a-96da-5e42404e0d28.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=5dbb76c1aa690caa69b73fae65bb6a5b410954e1)
Fig. 16.   EFA   result   on   schematic,   one   invertor   highlighted   by  PEM/OBIRCH and abnormal EOP waveform on it

![target signal open  Abnormal metal profile around targetsignal,  whichlinkedtotheanomalityonotherGPIOs  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/26bf90c3-28c3-4382-968b-3d7f89688117/26bf90c3-28c3-4382-968b-3d7f89688117.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215835%3B1743219435&q-key-time=1743215835%3B1743219435&q-header-list=host&q-url-param-list=&q-signature=aa4cba66bea2b7ab77c58cca5c0c424e9b967f79)
Fig. 17.   PFA result, metal defect on metal5 by SEM inspection

## IV.   S UMMARY  

In this paper novel FA workflow was proposed to  overcome the challenge in test coverage and functional  failure issues, that combined bench and pattern test in  different EFA phase.

1.    For test coverage issue, suspected signals or cells  were located by using bench test primarily, then  apply pattern test as auxiliary test method to isolate  defective site quickly and effectively.     2.    For functional pattern failure, PEM/OBIRCH/DALS  analysis served as the primary test to initially  identify the analysis direction, then bench test was  probably   auxiliary   method   to   build  appropriate configuration flexibly to stimulate target  signal/cell or facilitate a shorten test loop.


Three real cases sharing (two cases for test coverage  issue, one case for functional pattern failure) illustrated this  FA workflow was effective to localize fault accurately and  quickly, meanwhile success rate and cycle time could be  improved. In additional it provided alternative approach for  solving complex issue by combining different test platform  or method in the future.

## A CKNOWLEDGMENT 

For this work and study, I would like to thank for bench  test support by Nan Hong, Xiaodong Bai and Xin Fang from  business line, FA technical discussion with Nan Xiao and  Ang Li, Nanoprobing & PFA support by Shijun Zheng,  Haijiao Bian and Jianli Yang. Meanwhile I sincerely  appreciate my colleagues in cross team of NXP  semiconductor to provide helpful information.

## R EFERENCES 

[1]    S.  Boubezari, J. Chhabria, “Failure and Root Cause Analysis for a  System-on-Chip: An Industrial Case Study,”   $9^{\mathrm{th}}$   International Design  and Test Symposium, 2014    [2]    Mentor Graphics, “Tessent® Shell Reference Manual,”    [3]    A. Machouat, G. Haller, V. Goubier, D. Lewis, V. Pouget, P. Fouilla,  F. Essel, P. Perdu, “Scan-Based ATPG Diagnostic and Optical  Techniques Combination: A New Approach to Improve Accuracy of  Defect Isolation in Functional Logic Failure,”   $15^{\mathrm{th}}$   International  Symposium on the Physical and Failure Analysis of Integrated  Circuits, 2008.    [4]    K.Q Ouyang, X.X Wei, X.Y Lin, D. Yang, N. Mei, T.B Sun, “Fault  Localization of Functional Failure by using Dynamic EMMI Analysis  Technique,”    $23^{\mathrm{rd}}$   International Conference on Electronic Packaging  Technology, 2022

