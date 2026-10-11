---
title: "149_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_7e72e180fa0964ebac1cd302a2c1597e7295230462135641
file_size: 327624
---

## Design and Verification of SRAM Self-Detection  Repair Based on ECC and BISR Circuit  

Yanqing Zhang, Yinghun Piao, Mingxue Huo, Tianqi Wang, Guoliang Ma,   Chaoming Liu, Jianning Ma, Kairui Guo   and Chunhua Qi \*   Harbin Institute of Technology, No. 2, Xidazhi Street, Harbin, Heilongjiang Province.  Phone: +86 13904656920 \*Email: qchunh@126.com

Abstract -  In the space radiation environment, the chip in the  spacecraft   is susceptible to radiation effects, which leading to the  errors of the device. Therefore, the detection and repair of the  errors is particularly important. Aiming at the soft and hard  errors of memory cell caused by single event effect in space  radiation environment, a memory architecture based on ECC  circuit and BISR circuit is proposed to detect errors online,  distinguish between soft and hard errors and repair them, so as  to reduce the accumulation of errors. And the memory structure  uses repair circuit and redundant memory to repair soft errors  and hard errors respectively. The simulation results show that in  normal read-write mode, the proposed memory structure not only  can repair soft errors, but also can repair hard errors, and can  detect unrepairable hard errors. It means that the proposed  method is effective.   when the memory size is   $\mathbf{39\,x\,64K}$  , the area of  the ECC and the BIRA circuit is about   $\mathbf{13.95\%}$   of the entire  memory chip.

Keywords – Single event effect, ECC, Soft error, Hard error,  BISR.

## I. I NTRODUCTION  

Integrated circuit chips are exposed to various unfavorable  radiation environments in space. Radiated particles can lead to  several types of errors in devices, which will affect the overall  function of the circuit [1]. In the integrated circuit chips, the  area of memory usually accounts for more than  $60\%$   of the total  area, so the fault diagnosis and repair of memory is particularly  important. Chip faults in radiation environment are mainly  affected by single event effect [2, 3], including soft errors and  hard errors. For soft errors, Error Correction Codes (ECC) [4 -  6] technique is widely used in SRAM circuits, which can greatly  improve the fault tolerance of memory by encoding input data  and adding additional redundant storage bits in memory [7, 8].  As for hard errors, built-in self-test (BIST) technology [9, 10]  is the mainstream of memory testing technology, with which  built-in self-repair (BISR) technology emerges to deal with the  repair of hard errors [11, 12]. ECC circuit and BISR circuit are  conventionally used for repairing soft errors and hard errors  respectively [13]. In this paper, we proposed an on-line SRAM  detection and repair circuit based on ECC circuit and BISR  circuit according to the two kinds of errors characteristics in  order to improve the reliability of memory. In read-write mode,  this memory structure not only can repair soft errors, but also  can repair hard errors, and when the all redundant memory is  used, it can detect unrepairable hard errors. It is suitable for  dealing with the single event effect in the process of reading and  writing.

## II. S OFT  E RROR  R EPAIR  B ASED  O N  E CC 

Single event effects can cause soft and hard errors in memory  cells. Soft errors are temporary while hard errors are permanent.

In order to cope with the errors caused by the single-event effect  in the radiation environment, the classical ECCs for memory  error correction are Hamming codes, which require a small  number of check bits, and the syndromes calculated by  comparing the decoding one by one. The relationship with the  error mode can correct any single error in the data or detect two  random errors. However, the traditional ECC memory can only  correct the output data, but can’t repair the error data in the  memory, so the error is always kept in the memory. If the single  event effect occurs again, the corrective ability of Hamming  code is not enough to correct the data with two errors.  According to the characteristics of different errors, in order to  reduce the accumulation of errors, it is necessary to repair soft  errors and detect hard errors in the memory. When reading data,  the ECC circuit based on Hamming code can be used to detect  and modify the error data in memory, write back and re-detect  the modified data, so as to determine the error type. If there are  no errors after re-detection, the data will be read out, indicating  that the soft error is corrected. Otherwise, the address will be a  hard error and send out a hard error signal. The structure of ECC  circuit and SRAM memory is shown in Fig. 1.

![Data_out  Data_out DetectionCorrector  Detection_Corrector Read Q(F)  Read Q(F) Datain  Data_in  Error(F  Error(F)  State_  State_  ReadQ'(S)  Read Q´(S)  Decoder  Decoder transformer  transformer SRAM  SRAM Encoder  Encoder  Errorflag(S)  Error_flag(S) WritebackQ  Write back Q ’ ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b8f29d86-8563-4de2-936e-ffa4f34047c2/b8f29d86-8563-4de2-936e-ffa4f34047c2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=fd34e8955aa259c03d0bb5982055621077d52f0f)
Fig. 1 SRAM Architecture for Soft Error Repair.

As shown in Fig 1, there are Encoder, SRAM memory and  Dectection_Corrector   consisting   of   Decoder   and  State_transformer. F means the first time; S means the second  time. When writing data, input data first enters the encoder,  which encodes the received data and stores the generated  supervisory code in SRAM together; when reading data, the  first read data Q detects whether there is an error through the  detector. When there is no error, the data Q is output directly;  when Q is wrong, the data Q is corrected by Decoder, and then  the data Q is written back to the original address and read out  the address again. Q’ is judged by the Decoder again whether  data of the address error is a correctable soft error. If there is no  error, soft error of the address is corrected and the data Q is read  out. Otherwise, the address error can’t be corrected through  writing back, the Decoder sends an error signal, informing the  system that the current address has an irreparable error.

The State_transformer is implemented by finite state machine.  According to the error condition, it is divided into three states,  namely   DETECTION_ERROR,   WRITE_ORIGIN   and  DETECTION_TYPE. The transition between States mainly  depends on the checking signal S which is sent by the Decoder.  The error detection state transition diagram is shown in Fig.2.

![WRITE  WRITE_ S != 0   ORIGIN  ORIGIN S == 0  DETECTION DETECTION   DETECTION  DETECTION _ERROR ERROR   _TYPE _TYPE  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/799fc938-6057-4c4f-a020-469e22cc867c/799fc938-6057-4c4f-a020-469e22cc867c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=aca2213c52f5c19dbc4e2537c2a78f8d2a0abc0c)
Fig. 2 Error Detection State Transition Diagram.

As shown in Fig. 2, S is the detect signal. According to the  structure in Fig. 1, in the  DETECTION_ERROR  state, the  data Q is detected. If there is no error, read the data Q out. If  there is an error, jump to the WRITE_ORIGIN state, wait for  the data to be written back to original address; jump to the  DETECTION_TYPE  state after writing back, and check out  the second read-out data Q'. If there is no error, output the  correct data Q'; otherwise, an Error_flag is output to indicate  that there is a hard error in the current address.

## III. B ISR  C IRCUIT  A ND  O VERALL  A RCHITECTURE 

The repair of hard error is mainly realized by BISR circuit.  BISR module includes BIST module and BIRA module. The  whole circuit is divided into test mode and normal read-write  mode. The specific BISR structure is shown in Fig. 3.

![Testin  Test_in Bistin  Bist_in  Test_out  Test_out BIST  BIST SRAM  SRAM Faultaddress  Fault_address Nomal  Nomal  address  address address  address BIRA  BIRA Mapping  Mapping  address  address Redundant SRAM  Redundant SRAM ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b561960e-0f7d-4f06-8e0e-e7e53a471b89/b561960e-0f7d-4f06-8e0e-e7e53a471b89.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=923e544d6bae64ff4d3e255e2f0820fa82afcac6)
Fig. 3 Architecture of BISR.

As shown in Fig. 3, the overall structure is mainly divided  into two working modes: test mode and normal reading and  writing mode. The test mode mainly depends on the BIST  circuit. When the BIST_en signal is valid, the BIST circuit  detects the SRAM memory and stores the fault address in the  BIRA (Built in Redundancy Analysis) module. The normal  reading and writing mode mainly depend on the BIRA module,  whose function is to map fault addresses to redundant  addresses. In the normal read-write mode, the address first  enters the BIRA module to detect whether it is a fault address,  if not, the original address is output; if so, the fault address is  mapped to a redundant address to isolate the fault address. Based on the function of BIRA address mapping, this paper  designs a BIRA module which can store fault address and map  address in read-write mode. Detailed BIRA module is shown in

Fig. 4.

![BIRA  BIRA change_addr  change_addr_  Redundant  Redundant   ready  ready  flags  flags addr adcr   Mapper  Mapper  addr_map addrmap-FaultAddress  Fault Address  Memory  Memory ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/82276a92-1ec5-428b-b25c-9bb29551223a/82276a92-1ec5-428b-b25c-9bb29551223a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=9fdc7d03462d14d03748861ef5429d696c7a756f)
Fig. 4 Architecture of BIRA.

As shown in Fig. 4, in the normal read-write mode, the BIRA  module is used to map the fault address to redundant address.  The change_addr_ready signal set 1 when a hard error is found,  and store the current address into the fault address memory to  map it to the corresponding redundant address. When the  address is selected next time, it is mapped directly to the  redundant address, thus isolating the original hard error  addresses. Therefore, in the read-write mode, based on this hard  error isolation mechanism, and according to the way of  detecting hard errors in the previous section, when the ECC  circuit detects hard errors, the hard error isolation can be  completed by   BIRA module.

According to the repairing scheme of soft and hard errors,  ECC circuit and BISR circuit can be combined to deal with  these two errors. Based on the ECC circuit, the fault type is  judged, and different repair methods are selected according to  the fault type. In the normal read-write mode, the BIST circuit  is bypassed. The overall structure is shown in Fig. 4.

![CLK-  CLK  DATA_READY DATAREADY  -RST_EN  RST_EN  DATA_OUT  DATA_OUT —DATA_IN  DATA_IN  Encoder  Dectection_Corrector Dectection_Correcto  Main  Main DecoderError(F)State  Error(F)  State_  SRAM  SRAM  Decoder transformer  transformer Error(S)  Error(S) WEN WEN-   Redun  Redun SRAM  SRAM ADDR ADDR   BIRA  BIRA CHANGE_FAIL  CHANGE_FAIL CEN CEN-   Write back Q tebackQ  ’ ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5ec83c79-811e-4355-807f-a9bb42e16ce0/5ec83c79-811e-4355-807f-a9bb42e16ce0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=31fb4ca3877a993269470f57b06572aee5282eab)
Fig. 5 SRAM Architecture for Soft and Hard Error Repair.

The main signal in Fig 5 is shown in TABLE 1.

|Signal|Type|Description|
|---|---|---|
|CLK|Input|clock|
|RST_EN|Input|Reset signal, active LOW|
|DATA_IN [31:0]|Input|data inputs|
|WEN|Input|write enable, active LOW|
|CEN|Input|chip enable, active LOW|
|ADDR|Input|addresses|
|DATA_READY|Output|data ready signal, active HIGH|


|Signal|Type|Description|
|---|---|---|
|DATA_OUT [31:0]|Output|data outputs|
|CHANGE_FAIL|Output|change fail signal, active HIGH|


As shown in Fig. 4, according to the workflow of the ECC  circuit mentioned above, in the normal read-write mode, When  reading data(CEN is 0 and WEN is 1), when the detector detects  the error of the second read-out data by using the corrector, the  detector will send a hard error signal indicating that the current  address has a hard error. The error signal will be sent to the  BIRA module, which stores the current address in the fault  address memory and maps it to the fault-free redundant address.  Then, the corrector writes the correct data to the redundant  address and reads the data again. At this time, the  DATA_READY is set to 1, indicating that the current data is  valid, thus completing the repair of the hard error. Next time the  hard fault address is selected, the BIRA module maps the  address to the corresponding address and outputs the data of the  redundant address. If the redundant address is used up and a  hard error is detected, the CHANGE_FAIL will be changed to  1 to inform the system that current address has an irreparable  hard error.

The state of the decoder also needs to be changed. The  detailed state machine is shown in Fig 6.

![WRITE  WRITE_ S != 0   ORIGIN  ORIGIN S == 0  DETECTION  DETECTION  S==0  S == 0  DETECTION  DETECTION _ERROR ERROR   _TYPE _TYPE  S != 0  STORAGE  STORAGE_ OUTPUT  OUTPUT_ HEADDR  HEADDR DATA  DATA WRITE  WRITE_ REDUN  REDUN_ MAP  MAP ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/91f626e6-9942-4b79-a05a-b29c9a2cd74e/91f626e6-9942-4b79-a05a-b29c9a2cd74e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=9751512f6e48e4a17ed89e94ce92404c6a6d5fd9)
Fig. 6 Soft and Hard Error Repair State Diagram.

The whole state is performed while reading the memory. As  shown in Figure 6, S is the detection signal. According to the  structure of Fig. 5, In state of DETECTION_ERROR, detect  the first output data Q. If there are no errors, read the data Q. If  there is an error, the error is corrected by Corrector and state is  jumping to the WRITE_ORIGIN to write back correct data to  original address. Waiting for the data to be written back and  jump to the DETECTION_TYPE state, Detector detect the  second read data Q'. If there are no errors, it will jump to the  initial state, and output the correct data Q'; if data is still wrong,  jump to STORAGE_HEAADR state, The BIRA module stores  current fault address. The corrected data is written to the  redundant address in state of WRITE_REDUN_MAP. The last  output the data in OUTPUT_DATA state.   Through this process,  the repair of soft and hard errors and the detection of  irreparable hard errors have been completed. Soft error repair  requires two clock cycles, and hard error repair requires five  clock cycles of delay. Only when errors are detected, the  mechanism will be activated, which reduces the impact on the

system.

## IV. R ESULT 

ECC circuit and BISR circuit are designed by Verilog HDL.  39x4k main memory and 39x64 redundant memory are  generated by Memory Compiler. In order to verify the  correctness of the circuit function, the AHB slave interface was  designed and combined with circuit, installed on the AHB bus  for system level verification. The memory output is injected  fault to complete the overall simulation verification in  ModelSim. The whole fault injection platform is shown in Fig  7.

![HSEI  HSEL  DATA_READY  DATA_READY  IP core  IP core HADDR  HADDR  DATA_OUT  DATA_OUT HWRITE  HWRITE HTRANS  HTRANS[1:0] CLK-  CLK  Injection  Injection  HSIZE[2  HSIZE[2:0]  fault  RST_EN  RST_EN  fault HBURST  HBURST[2:0] 2:01  -DATA]  DATA_IN  Encoder HWDATA[31:0] HWDATA   10   AHB AHB   Main  Main  Dectection  Dectection BFM BFN  interface interface   SRAM  SRAM  _Corrector Corrector  HMASTER  HMASTER[3:0] CHANGE_FAIL  Idrmap  ErrorSignal  Error Signal HMASTI  HMASTLOCK HREAD  HREADY  WEN WENH   Redun  Redun HRESP[1  HRESP[1:0]  SRAM  SRAM ADDR ADDR   BIRA  BIRA HCLK  HCLK  CEN CEN-   Write back Q’  Write back Q ’ HRESET  HRESETn ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/69d22efc-b210-4f27-a288-fe002ecdbe96/69d22efc-b210-4f27-a288-fe002ecdbe96.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=1f92080cd27c02a13bc316ad1b90793220f29df1)
Fig. 7 System-level Verification Platform.

Based on the fault injection point shown in Fig 7, when the  system reads the data, the fault is injected into the memory  output data data_sram_out signal of the slave. First, verify the  case of soft errors. In order to simulate soft errors, only keep it  until the correct data is written back.   The specific case of soft  error injection is shown in Fig. 8.

Fig. 8 Soft Error Repair for System-Level Verification.

|        hcik                hsel      |        1*h1                1*h1      ||||||||
|---|---|---|---|---|---|---|---|---|
|        hcik                hsel      |        1*h1                1*h1      |hsel|||||||
|        hcik                hsel      |        1*h1                1*h1      |hsel|||||||
|        hcik                hsel      |        1*h1                1*h1      |hsel|        hsel                hsel_m                hmaster      ||||||
|        16h0004                4*h1      |||        hsel                hsel_m                hmaster      ||||||
|htrans|htrans|2*h2|2*h2||||||
|haddr|haddr|32'h00000010|32'h00000010|32'h00000010|32'h00000010||||
|hwrite|hwrite||||||||
||||||||||
||||||||||
|hwdata|hwdata|        32'h00000000                1*hG      |||||||
|hready|hready|        32'h00000000                1*hG      |||||||
|hresp|hresp|2*h0|2*h0|2*h0|2*h0||||
|        hrdata                data_ready                state      |        32h11111111                1*hG                3h0      |32h11111111|32h11111111||||||
|        hrdata                data_ready                state      |        32h11111111                1*hG                3h0      ||||||||
|data_sram_out|data_sram_out|39h0444404449|39h0444404449|39h0444404449|39h0444404449|39h0444404449|||
|        CEN                VEN      |        39h0444444449                1hC                1h1                12'h010                39h0000000000      ||||||||
|        CEN                VEN      |        39h0444444449                1hC                1h1                12'h010                39h0000000000      ||||||||
|        CEN                VEN      |        39h0444444449                1hC                1h1                12'h010                39h0000000000      ||||||||
|        CEN                VEN      |        39h0444444449                1hC                1h1                12'h010                39h0000000000      ||||||||


As can be seen from Fig. 8, when current address is 12'h010,  the injection error data is 39'h0444404449. In state of  DETECTION_ERROR the decoder finds the error, it set  data_ready signal to 0. The master receives data_ready signal  of the slave which is 0, it waits and keeps the original address.  Decoder writes the correct data back to the original address  12'h010 in the next state (WRITE_ORIGIN). After writing  back, data will be output when decoder detect read-out data  39’h0444444449 has no error. data_ready is valid, indicating  that the data in memory has been corrected, and the current data  is valid.

The second is to verify the repair of hard errors, which,  unlike soft errors, doesn’t change the memory data even if it is  written back. Therefore, it is necessary to keep the fault until it  is written back to the redundant address, so as to simulate the

case of hard errors. The injection of hard errors is shown in Fig.    9.

|        hcik                hsel                hsel_m      ||||||||||||
|---|---|---|---|---|---|---|---|---|---|---|---|
|        hcik                hsel                hsel_m      |        hcik                hsel                hsel_m                hmaster                htrans                haddr                hwrite                hwdata                hready                hresp                hrdata                data_ready                state      |        11*h1                1-h1                16*h0004                4h1                2*h2                32'h00000014                1*hG                32h00000000                1*hO                2*h0                32h22222222                1-hG                3-h0      ||||||||||
|        hcik                hsel                hsel_m      |        hcik                hsel                hsel_m                hmaster                htrans                haddr                hwrite                hwdata                hready                hresp                hrdata                data_ready                state      |        11*h1                1-h1                16*h0004                4h1                2*h2                32'h00000014                1*hG                32h00000000                1*hO                2*h0                32h22222222                1-hG                3-h0      ||||||||||
||        hcik                hsel                hsel_m                hmaster                htrans                haddr                hwrite                hwdata                hready                hresp                hrdata                data_ready                state      |        11*h1                1-h1                16*h0004                4h1                2*h2                32'h00000014                1*hG                32h00000000                1*hO                2*h0                32h22222222                1-hG                3-h0      |16h0004||||||||16h0002|
|pho|        hcik                hsel                hsel_m                hmaster                htrans                haddr                hwrite                hwdata                hready                hresp                hrdata                data_ready                state      |        11*h1                1-h1                16*h0004                4h1                2*h2                32'h00000014                1*hG                32h00000000                1*hO                2*h0                32h22222222                1-hG                3-h0      |12*h2||||||||12h0|
||        hcik                hsel                hsel_m                hmaster                htrans                haddr                hwrite                hwdata                hready                hresp                hrdata                data_ready                state      |        11*h1                1-h1                16*h0004                4h1                2*h2                32'h00000014                1*hG                32h00000000                1*hO                2*h0                32h22222222                1-hG                3-h0      ||||||||||
|B2'h00b00ood|        hcik                hsel                hsel_m                hmaster                htrans                haddr                hwrite                hwdata                hready                hresp                hrdata                data_ready                state      |        11*h1                1-h1                16*h0004                4h1                2*h2                32'h00000014                1*hG                32h00000000                1*hO                2*h0                32h22222222                1-hG                3-h0      ||||||||||
||        hcik                hsel                hsel_m                hmaster                htrans                haddr                hwrite                hwdata                hready                hresp                hrdata                data_ready                state      |        11*h1                1-h1                16*h0004                4h1                2*h2                32'h00000014                1*hG                32h00000000                1*hO                2*h0                32h22222222                1-hG                3-h0      ||||||||||
||        hcik                hsel                hsel_m                hmaster                htrans                haddr                hwrite                hwdata                hready                hresp                hrdata                data_ready                state      |        11*h1                1-h1                16*h0004                4h1                2*h2                32'h00000014                1*hG                32h00000000                1*hO                2*h0                32h22222222                1-hG                3-h0      ||||||||||
||        hcik                hsel                hsel_m                hmaster                htrans                haddr                hwrite                hwdata                hready                hresp                hrdata                data_ready                state      |        11*h1                1-h1                16*h0004                4h1                2*h2                32'h00000014                1*hG                32h00000000                1*hO                2*h0                32h22222222                1-hG                3-h0      ||||||||||
|||||||||||||
|        CEN                YEN                Main      |        39h48888888b8                1-hO                1*h1                12*h014                39'h0000000000                39hxxxxxxxxxx                1-h1                1-h1                6-h14                39'h0000000000      |||||||||||
|        CEN                YEN                Main      |        39h48888888b8                1-hO                1*h1                12*h014                39'h0000000000                39hxxxxxxxxxx                1-h1                1-h1                6-h14                39'h0000000000      |||||||||||
|        CEN                YEN                Main      |        39h48888888b8                1-hO                1*h1                12*h014                39'h0000000000                39hxxxxxxxxxx                1-h1                1-h1                6-h14                39'h0000000000      |||||||||||
|        CEN                EN                Redundant      |        39h48888888b8                1-hO                1*h1                12*h014                39'h0000000000                39hxxxxxxxxxx                1-h1                1-h1                6-h14                39'h0000000000      |||||||||||
|        CEN                EN                Redundant      |        39h48888888b8                1-hO                1*h1                12*h014                39'h0000000000                39hxxxxxxxxxx                1-h1                1-h1                6-h14                39'h0000000000      |||||||||||
|        CEN                EN                Redundant      |        39h48888888b8                1-hO                1*h1                12*h014                39'h0000000000                39hxxxxxxxxxx                1-h1                1-h1                6-h14                39'h0000000000      |||||||||||


Fig. 9 Hard Error Repair for System-Level Verification.

As shown in Fig. 9, when the address is  $12\%14$  , the hard error  data 39'h48888c88b8 is injected. In the DETECTION_TYPE  state, the read-out data also has an error, the current address is  stored in the STORAGE_HEAADR state, and in the  WRITE_REDUN_MAP state, the address is mapped to the  redundant address 6'h00 and the correct data is written to it.  Finally, the correct data is output and the data_ready signal is  active. The overall repair process requires five clock cycles of  delay, but the next time the address is selected, the data of the  redundant address will be output directly without delay, thus  reducing the impact on the system.

Through fault injection, the fault conditions under various  states are simulated, and the simulation results are analyzed.  The results are shown in TABLE II below.

TABLE II.     S IMULATION  R ESULTS

|Mode|Fault Address|Fault Type|Memory Location|Correction Method|
|---|---|---|---|---|
|Read/Write|N|None||None|
|Read/Write|Y|None||Map to Redundant Address|
|Read|N|Soft|Main|ECC Correction|
|Read|Y|Soft|Redundant|ECC Correction|
|Read|N|Hard|Main|Stores Fault Address and Maps to Redundant Address|
|Read|Y|Hard|Redundant|Stores Fault Address and Maps to New Redundant Address|


As can be seen from Table  II , for soft errors, the memory can  be corrected by ECC circuit in the normal reading process. For  hard errors, the memory can be repaired by ECC circuit  detection and BIRA circuit mapping in the normal reading  mode.

We have implemented logic synthesize of the whole design  on Desgin Compiler platform with SMIC65 process library.  Then, based on formula 1, the hardware overhead ratio of the  Encoder, Dectection_Corrector and the BIRA module in the  overall design is analyzed under 39bits of different memory

sizes and the same redundancy ratio.   The area ratio is shown  in Fig. 10.

Hardware_Overhead_ratio（）

ECC+BIRA

(1)

Total

![Hardware Overhead Ratio  16.5  16  15.5  14.5  14  13_5  14   16  MemorySize/x4k  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3ce32908-c57f-4872-bb2e-82a4aa41a967/3ce32908-c57f-4872-bb2e-82a4aa41a967.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215635%3B1743219235&q-key-time=1743215635%3B1743219235&q-header-list=host&q-url-param-list=&q-signature=4dc4254edd233d2875fad373da22b9dca1dc847b)
Fig. 10 Hardware Overhead Ratio of Other Circuit.

As can be seen from Fig. 10, with the increase of memory  size, the ratio of Encoder, Dectection_Corrector and BIRA  modules in the overall area gradually decreases. When the  memory size is  $39\,\mathrm{x}\,64\mathrm{k}$  , the area ratio is about   $13.95\%$  .

## IV. C ONCLUSION 

We propose an integrated structure of   SRAM based on ECC  circuit and BISR circuit, which can detect and repair soft errors  and hard errors caused by space radiation. In normal read-write  mode, soft errors can be corrected by ECC circuit in normal  read-write mode ;  hard errors can be corrected by ECC circuit  detection and BISR circuit mapping, thereby reducing the  accumulation of errors in the memory. Because of its selfdetecting and repairing characteristics, it can better deal with  the errors caused by single event effect in space radiation  environment, and improve the reliability of memory.

## A CKNOWLEDGMENT 

Fund project: This work was supported by the National  Natural Science Foundation of China (Grant Nos. 61704039,  61771167, 11775061, 11805045), the Natural Science  Foundation of Heilongjiang Province (Grant No. QC2017073),  the Science and Technology Innovation Foundation of Harbin  (Grant No. 2016RAQXJ068), the Fundamental Research Funds  for the Central Universities (Grant No. HIT. NSRIF. 2018.09)  and the “111 project” (Grant No. B18017).

## R EFERENCES 

[1]   R. D. Schrimpf and D. M. Fleetwood, Radiation Effects and Soft Errors  in Integrated Circuits and Electronic Devices. Singapore:  World  Scientific , 2004.  [2]   Wang T Q, Xiao L Y, Zhou B, et al. Analysis of process variations impact  on the single-event transient quenching in 65 nm CMOS combinational  circuits. Sci China Tech Sci, 2014, 57: 322-331, doi: 10.1007/s11431-   013-5441-9.   [3]   Huo M X, Ma G L, Zhou B, et al. Single-event upset prediction in static  random access memory cell account for parameter variations. Sci China  Inf Sci, 2019, 62(6): 069404, https://doi.org/10.1007/s11432-018-9561-   9  [4]   Bentuotuo Y. A Real Time EDAC System for Applications Onboard

Earth Observation Small Satellites.  IEEE Transactions on Aerospace &

Electronics Systems , pp. 648-657, 2012.     [5]   Blaum M, Goodman R, Mceliece R,  et al . The reliability of single-error  protected computer memories.  Computers IEEE Transactions on ,   pp.  114-119, 1988.    [6]   Saiz-Adalid L J, Reviriego P, Gil P,  et al . MCU Tolerance in SRAMs  Through Low-Redundancy Triple Adjacent Error Correction.  IEEE  Transactions on Very Large Scale Integration Systems , pp. 2332-2336,  2015    [7]   Reviriego P, Pontarelli S, Evans A,  et al . A Class of SEC-DED-DAEC  Codes Derived From Orthogonal Latin Square Codes.   IEEE  Transactions on Very Large Scale Integration Systems , pp. 968-972,  2015    [8]   Mary Francy Joseph, Anith Mohan,  et al . Improved Architecture for Tag  Matching in Cache Memory Coded with Error Correcting Codes.  Procedia Technology , pp. 544-551, 2016.     [9]   Syc. Cz. What is the BIST system.  Przeglad Telekom unikacynjy . pp.  174-178, 1979.    [10] Preethy K John, Rony Antony P,  et al . BIST Architecture for Multiple  RAMs in SoC,  7th International Conference on Advances in Computing  & Communications , pp. 159-165, 2017.     [11] Wooheon-Kang, Hyungjun Cho, Joohwan Lee, Sungho, Kang,  et al . “A  BIRA for Memories With an Optimal Repair Rate Using Spare Memories  for Area Reduction,”  IEEE Trans. VLSI systems , vol. 22, no. 11, pp. 2336  - 2349, Nov.2014.     [12] A. S. Nair, P. L. Bonifus,  et al . An efficient built-in self-repair scheme  for multiple RAMs, 2017 2nd IEEE International Conference on Recent  Trends in Electronics,  Information & Communication Technology  (RTEICT), Bangalore , pp. 2076-2080, 2017.    [13] Shyue-Kung Lu, Cheng-Ju Tsai, and Masaki Hashizume,  et al .  Integration of Hard Repair Techniques with ECC for Enhancing  Fabrication Yield and Reliability of Embedded Memories.  IEEE 24th  Asian Test Symposium , pp.49-54, 2015.

