---
title: "151_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_80700aa7a8687fc21ffff906f3999b687295230462135641
file_size: 405389
---

## Design of Radiation-Hardened Image Compressor  Based on Lossless JPEG-LS  

Chunhua Qi, Jianning Ma, Mingxue Huo, Tianqi Wang, Guoliang Ma,   Chaoming Liu, Yinghun Piao, Kairui Guo and Yanqing Zhang \*   Harbin Institute of Technology, No. 2, Xidazhi Street, Harbin, Heilongjiang Province.  \* Phone: +86 15304806698      Email:  zhangyanqingHIT@163.com

Abstract-    Image compressor in aerospace application is  susceptible to single event effect, causing encoder logic errors and  system errors. Therefore, the image compressor in aerospace  application must be specially designed to improve the reliability of  image information. Compression efficiency of JPEG-LS is higher  than JPEG2000 and compression effect is better than lossless  JPEG. Especially, JPEG-LS algorithm has the characteristics of  low complexity and easy hardware implementation, which will  save hardware resources of spaceborne system. An image  compressor based on lossless JPEG-LS algorithm is designed in  this paper, which can correctly compress   $\pmb{512}\times\pmb{512}$   8-bit wide  grayscale images. It is hardened by three-mode redundancy,  Hamming code, timeout detection, one-hot code, and   inter-process  independently.   The results point out that the error rate caused by  SEU is significantly reduced   ${\bf19.48\%}$   using the hardened  compressor in this paper.

Keywords  –  JPEG-LS, Image Compressor, Radiation-Harden ， soft errors .

## I. I NTRODUCTION 

The application scenarios of image information interaction  are more and more common in aerospace technology [1,2].  However, the onboard equipment resources are limited [3,4]. It  cannot meet the storage requirements of a large number of  image data. With limited onboard memory capacity and  application of existing communication bandwidth, image  compressor is necessary to exist.

Among many image compression algorithms, the JPEG-LS  is an algorithm for lossless or near lossless compression of  static continuous tone images in the new ISO/ITU standard [5],  and it is a compression method based on LOCO-I (Low  Complexity Lossless Compression for Image) proposed by HP  laboratory Weinberger et al [6]. Compression efficiency of  JPEG-LS is higher than JPEG2000, compression result is better  than lossless standard compression JPEG. JPEG-LS algorithm  has good applicability to various types of images, so it is widely  used in space image processing, medical and other fields.  Moreover, JPEG-LS is a predictive differential compression  algorithm [7]-[9]. The low memory demanded is one important  advantage over transform-based ones for it. But one drawback  is that a single soft error can corrupt part of a packed data block  [10]-[12].

In addition, there are many energetic charged particles from  cosmic rays, solar flares and other radiation sources in the space  environment.   When these energetic particles impact on devices  (e.g. RAM, microprocessor, image compressor, etc.), the  electron-hole pairs are generated in the sensitive areas of

devices.   Electron-hole pairs form signals that open connections.  These faults are collectively referred to single event effects  [13].   Due to ionization effect, a large number of electron-hole  pairs will cause soft errors in semiconductor devices and  transient errors in logic devices and memory. Single-Event  Upset (SEU) is one of the most common non-destructive errors  in single event effects [14]. Charge aggregation effect (funnel  effect) is one of the important theoretical models to explain the  single event upset.   The electron-hole pair can result the  redistribution of the electric field in the device. It causes the  change of the electrical performance of the device, which  results in the logic error of the logic device or circuit. Single  event upset is a soft error, which can be prevented by hardening  the device design.

Due to the harsh electromagnetic and radiation environment  in space, it is inevitable that the onboard image compression  system will be damaged by particle irradiation [15]. Therefore,  the image compressor must be hardened. Among the irradiation  effects, the SEU has serious impact on SRAM-Based FPGA  [16-17]. To ensure the accuracy and reliability of the image  compression process, radiation hardened methods must be  designed to reduce the effects of SEU. In this paper, an image  compressor based on lossless JPEG-LS algorithm is realized. It  can correctly compress   $512\!\times\!512$  8-bit wide grayscale images.  And the lossless JPEG-LS image compressor is hardened by  Hamming Error Detection and Correction (EDAC) technique,  timeout detection, inter-process independently ， one-hot code  and widespread TMR, which can reduce the error rate of image  compression results even if it is affected by the simulated SEU.

## II.   I MAGE COMPRESSOR BASED ON JPEG - LS 

The operation structure of JPEG-LS image compression  algorithm is shown in Fig. 1.

![Modeler  Modeler  Coder  Coder REGULAR REGULAR  context  context image  image  pred.errors,  pred.errors, samples  samples  Context  Context codelspec.  code spec.  Golomb  Golomb Modeler  Modeler  Coder  Coder Fixed  Fixed Gradient  Gradient Predictor  Predictor Calculation  Calculation Image  Image  · Source  Source Adaptive  Adaptive Flat  Flat  Correction  Correction  Predictor  Predictor Region  Region Yes Yes  compressed  compressed bitstream  bitstream runlengths  run lengths, 70  No  Run  Run  code'spec  code spec.  Rum  Run MODE  MODE   Counter  Counter  Coder  Coder RUN  RUN SELECT  SELECT ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/455d84bc-b6bb-41b4-9ba6-9d528bce8108/455d84bc-b6bb-41b4-9ba6-9d528bce8108.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=d81d08f63e3e2ac27a1025f4888f192908e60501)
Fig. 1 The operation structure of JPEG-LS algorithm [18]

It can be divided into three parts: mode selection module,  regular mode coding module, and run mode coding module.  Regular mode coding module outputs compressed bitstream  after prediction ,  context modeling and Golomb coding. Run  mode coding module outputs compressed bitstream after run  counter and run coder. The mode selection module detects  whether the pixel area belongs to a flat area (the local gradient  value is 0 or all NEAR) and decides which module the pixel  value will enter.

According to the operation structure of the algorithm, the  hardware structure based on the algorithm can be divided into  four parts: mode selector, regular mode coder, run mode coder  and result output device. They are all designed as shown in Fig.  2.

![Regular Mode Coder  Regular Mode Coder Regular       Mode        Update Result Result  Mode vlod  Uncompressed  Initia-  Compressed RAMa  RAMb  RAMc  RAMn  Output  Pixel Data  lization   Pixel Data Pixel Data   Selector Parameter Update Device Run          Mode        Update Run Mode Coder RunModeCoder  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9c07eb13-5886-4202-82fd-564c4e7ab85c/9c07eb13-5886-4202-82fd-564c4e7ab85c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=75061881d31f542cc59d0ce149d09af7e93ed6c2)
Fig. 2 Hardware Structure of Image Compressor

The mode selection module detects whether the pixel area  belongs to a flat area. If it is a flat area, pixel data will be  transmitted into the run length encoding module for encoding,  otherwise transmitted to the regular encoding module for  encoding. In the image compressor designed in this paper, the  mode selection module not only needs to judge whether the  pixel belongs to a flat area, but also has the function of  controlling image data direction. It is mainly controlled by the  state machine of 5 states, as shown in Fig. 3.

![Waiting  Waiting  DIE  IDLE to start  to start req_flag=0  req_flag=0 Start  Start  req_flag=0  req_flag=0 S0 Ra=Ix Ra=Rb=Rc=Rd req_flag=1 RC  S2  eqfa   RC  S1  Ra-Rb-Re=Rd Rax&regularisfec  Ra ≠ Ix & regular is free Ra   S3 Ra coRblctey Rdare not  cgual conpletely Rdarene   req_flag=0  req_flag=0 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e502b969-055e-478c-aa43-44a036393f7e/e502b969-055e-478c-aa43-44a036393f7e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=140e9297f8afeb43e188c1874a575dbe95857708)
Fig. 3 Mode selection module state machine

Req_flag is the request signal for the next module. When  the current pixel value is completed the compression process,  the signal is valid 1, otherwise 0; IDLE is the initial state,  waiting for the start signal of image compression. When the  start is valid, the state machine transits from IDLE to S0,  otherwise it waits all the time; S0 is a state that enters the mode  selection stage for the first time, in this state, it satisfies  different requirements. Conditional state machine jumps to

different states: when the pixel values Ra, Rb, Rc and Rd are  not completely equal and req_flag is valid, it enters the regular  mode coder S1 state; when Ra, Rb, Rc and Rd are completely  equal, Ra is equal to Ix and req_flag is valid, it enters the  run-mode coder S2 state; when Ra, Rb, Rc, Rd are completely  equal, Ra is not equal to Ix and req_flag is valid, it enters the  run-mode coder S3 state. Particular attention is paid to the fact  that in order to satisfy the final coding results of the two modes,  it is necessary to wait for the idle state of the current mode to  switch in the process of switching between run mode and  regular mode.

In the regular mode encoding module, according to the  characteristics of the sequential execution of each sub-module,  the JPEG-LS regular mode operation flow is divided into  four-stage pipeline, as shown in Fig. 4. This can greatly shorten  the regular encoding operation time and increase the data  throughput, so it can increase the clock frequency. In the design  of the run coding module, the function of the run encoding  operation is realized.

![pipeline1  pipeline1  pipeline2  pipeline2  pipeline3  pipeline3  pipeline4  pipeline4 Q  M  K  Me  G P  Pc  E  up c Q  M  K  Me  G P  Pc  E  up c ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e3d9d8b5-c21e-47f8-9053-5f2fbb10d23a/e3d9d8b5-c21e-47f8-9053-5f2fbb10d23a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=066a6aada896db4e74ecf5e73829b23b6223f825)
Fig. 4 Regular mode pipeline

Result output device needs to receive the compressed bit  stream output from the regular mode coder and the run mode  coder, and splices them in the output order to form a complete  output bit stream. However, due to the unpredictability of bits  stream bits received each time, it is difficult to implement  hardware. 64 bits shift register are used to solve this problem, as  shown in Fig. 5.

![RegularBit  Regular Bit   Run Bit  Run Bit   Regular  Regular   Rum  Run Number  Number  Number  Number  Bit Stream  Bit Stream  Bit Stream  Bit Stream BitStreamSplicer  Bit Stream Splicer Reg-address  Reg-address  Generator  Generator address ddre  64Bits Shift Register  64 Bits Shift Register Shift[0:3 1]  Shift [0:31] 32bits  32 bits Output-ready  Output-ready   output  outpu  OutputController  Output Controller Detector  Detector  enable  enable ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0e19a636-cfd2-4064-90bf-27f82646778e/0e19a636-cfd2-4064-90bf-27f82646778e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=436e336eff679c1532d6f6389896ea8030c3190b)
Fig. 5 Result output device

Bit stream splicer identifies the coded results from the  previous module and splices them with the last output, and then  places the results in the shift register. Reg-address generator

calculates the address bits of the registers based on the bit  numbers, and passes the addresses to the shift register.  Output-ready detector detects whether the address is greater  than 31, and if the address is greater than 31, the address  generator will be positioned and the output signal will be  enabled. The results are low 32 bits of 64 bits shift register.

## III. SEU PROTECTION AGAINST RADIATION EFFECTS

Image compressors are widely used in aerospace systems due  to the limit of the lot of image information. However, they are  susceptible to irradiation effects, especially single-event upset  (SEU). In this paper, several methods have been proposed to  improve the radiation hardened performance of image  compressor.

The work of the mode selector is mainly accomplished by the  5-state state machine. In the actual work process, the single  event upset is likely to cause the state machine jump state error.  One hot code is a code system with only one bit 1 and all other  bits 0, that is to say, there are as many bits as states. In the  aspect of SEU, the code spacing of state machine coded by one  hot code is longer than that of binary code and gray code. Even  if affected by single event upset, it will only cause state  machine state to jump to undefined state, and not cause state  machine to jump to wrong state. Three-mode redundancy is one  of the most widely used and most classical harden methods for  flip flops. So one hot code and three-mode redundancy is  adopted to harden the mode selector, as shown in Fig. 6.

![present state register  present state register (one hot code)  (one hot code) v secondary  secondary   o present state register  present state register generative  generative   t (one hot code)  (one hot code) 10gic  logic  e r present state register  present state register (one hot code)  (one hot code) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a52e4b0a-155e-4735-9c3b-afcfea8c2b12/a52e4b0a-155e-4735-9c3b-afcfea8c2b12.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=a9e30721f83a67e855b6bc211ff52988a3b025b2)
Fig. 6 Harden structure of mode selector

In the design of JPEG-LS image compressor, the important  parameters A [Q], B [Q], C [Q], N [Q] are all from RAM. The  completion of parameter update module is the read-write  operation of RAM. Once the parameter data in RAM is affected  by SEU, all the compression results of subsequent image pixels  will be wrong, and the decompressed original image will not be  recovered. In this paper, Hamming code is adopted to harden  RAM, as shown in Fig. 7.

In addition to mode selector and parameter update RAMs,  JPEG-LS image compressor also includes regular mode coder,  run mode coder and result output device. Redundancy is to  increase the anti-SEU ability of the system through multiple  backups and improve the reliability of the system. In the design  of digital circuits, the three-mode redundancy (TMR) is the  most classic way. The three-mode redundancy is to perform the  additional two replications of the designed functional modules,  and select the correct output through multiplexer. In this paper,  regular mode coder, run mode coder and result output device

are hardened by TMR. In addition, as mentioned in the previous  section, regular mode coder is pipelined for processing  acceleration. The clock cycle required for each module is fixed.  When the logic in the system is affected by SEU, the result of  the module may not be output on time. A detector is designed to  detect whether each sub-module of the regular mode coder  outputs the results on time. If they fail to output on time, it  shows that it is affected by SEU. At this time, the error flag is  valid, as shown in Fig. 8.

![Message  Message Message  Message   Error  Error  Code  Code  Corrector  Corrector Supervised  Supervised   Corrector  Corrector  bits Generator  bits Generator  Generator  Generator Integrator of  Integrator of  message bits and  message bits and   RAM  RAM  supervisedbits  supervised bits ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cb8a1191-0835-4444-a702-8f2e160a435c/cb8a1191-0835-4444-a702-8f2e160a435c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=51f46660ce1c4d9f87bd8fd4175c26dde07c61ee)
Fig. 7 Error Detection and Error Correction Structure of Hamming Code

![Regular Mode Coder  Regular Mode Coder Sub-module  Sub-module  Sub-module Sub-module   …  Sub-module Sub-module   Sub-module  Sub-module Time-  Time-  Time-  Time-  Time-  Time-  Time-  Time… detector  detector  detector  detector  detector  detector  detector  detector Error_out  Error_out ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0a0c4c0a-2093-41ea-8c6e-bcc500595bcd/0a0c4c0a-2093-41ea-8c6e-bcc500595bcd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=7b8241988aa7575d4d863708db12d0b3b9699af5)
Fig. 8 Timeout detection

In the process of image processing, the image compressor  processes the image frame by frame, that is, the compression  result of the previous frame has no effect on the next frame.  Using this characteristic of image processing, each frame of  image is processed independently, that is, before compressing  each frame, the compressor will reset the relevant parameters  and triggers in its own system. In this paper, synchronous resets  are adopted. Because it can result in less logic, fewer  restrictions on packing, and, often, faster circuits.  Furthermore,  it can avoid the influence of circuit logic.

## IV. R ESULTS 

In this paper, all RTL designs are comprehensive. And we  use comprehensive tools to synthesize. The device we choose is  VC707. After synthesis, the resource utilization rate is  obtained. The external clock is 200 MHz differential clock, so  we use 100MHz after frequency division as our actual working  clock.

Using designed image compressor, 8 international standard  test images were successfully compressed. When the clock  frequency is 100 MHz, the encoder running time, regular  module run times, run module run times and compression code  rate are shown in Table I. It can be seen that the image  compression time is almost fixed at 0.0265s, satisfying the  speed requirement of image compression. The run module  running times show whether the image flat area is rich, and the  more times, the more flat areas; the compression rate of

compressor is not fixed. This depends on whether the flat area  of the image is rich enough. If there are many flat areas, the  code rate is low, otherwise the code rate is high.

Table I – Result statistics

|Image name|Result data|Result data|Result data|Result data|
|---|---|---|---|---|
|Image name|Time|Regular|Run|Bit Per Pixel|
|aerial|0.0265s|260830|806|5.09|
|airplane|0.0270s|256909|2643|3.94|
|babbon|0.0262s|262116|25|6.04|
|figerprint|0.0263s|262022|102|5.41|
|lena|0.0264s|261429|491|4.34|
|yacht|0.0266s|260164|1259|3.97|
|tree|0.0263s|261925|122|5.59|
|peppers|0.0264s|261553|406|4.62|


At the same time, we list the comprehensive utilization rate of  resources before and after hardening compressor, as shown in  Table II.

Table II – Contrast of resource utilization rate

|Site Type|Unharden|Harden|
|---|---|---|
|Slice LUTs|3481|5962|
|Slice Registers|1316|2705|
|Block RAM|155.5|155.5|
|Bonded IOB|10|10|
|BUFG|2|2|
|MMCM|1|1|


The fault injection experiment of the image compressor is  carried out by using the fault injection tool in reference [19]. In  this paper, 100 fault injections are made for each signal. In  regular mode coder, the rate of timeout detect flag be valid is   $4.52\%$  , showing that the detector can detect SEU. The rate of  error when SEU occurs is obtained by injection faults into the  unhardened and hardened compressor, as shown in Fig. 9. The  result shows that the error rate caused by SEU is significantly  reduced   $19.48\%$   using the proposed method in this paper.

![32.24% 35.00% 30.00% 24.60% 25.00%  20.10%  20.16% 20.00% 15.00% 10.00% 3.70% 839% 5.00%  .88%  .68% 0.00% regular  nun  select  RAN  total errorrate(unharden）  errorrate(harden) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8aea28af-119a-4fde-aac7-0f23779d5bc6/8aea28af-119a-4fde-aac7-0f23779d5bc6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215636%3B1743219236&q-key-time=1743215636%3B1743219236&q-header-list=host&q-url-param-list=&q-signature=7f96c9093864ac517faa90fb3cc78631630efdd5)
## V. C ONCLUSION   

The image compressor based on JPEG-LS is designed in this  paper, which can correctly compress   $512{\times}512$   8-bit wide

grayscale images. The bit per pixel is roughly between 3-6.  When the clock is   $100\ \mathrm{MHz}$  , the average time of compressing  an image is 0.0265s. The error rate caused by SEU is  significantly reduced   $19.48\%$   using the hardened compressor in  this paper.

## A CKNOWLEDGMENT 

This work was supported by the National Natural Science  Foundation of China (Grant Nos. 61704039, 61771167,  11775061, 11805045), the Natural Science Foundation of  Heilongjiang Province (Grant No. QC2017073), the Science  and Technology Innovation Foundation of Harbin (Grant No.  2016RAQXJ068), the Fundamental Research Funds for the  Central Universities (Grant No. HIT. NSRIF. 2018.09) and the  “111 project” (Grant No. B18017).

## R EFERENCES 

[1]    Chen Z, Duan Z T, Sun Z Y.  et al.  Design and implement of high  resolution still image compression and storage system . International  Conference on Wavelet Analysis and Pattern Recognition , p. 4, 2010.    [2]    Salahova, S. Remote Sensing and GIS Application for Earth  Observation on the base of the Neural Networks in Aerospace Image  Classification.  Recent Advances in Space Technologies , p. 10, 2007    [3]    Lixin Zhang, Peipei Wang. An  Improved Compression Based On  JPEG-LS.  Proceedings of 2015 International Conference on Computer  Science and Information Engineering . pp. 6-8, 2015.    [4]    Kastensmidt F L, Sterpone L, Carro L,  et al.  On  the  optimal  design  of   triple  modular  redundancy  logic for SRAM-based FPGAs.  Proceedings of the conference on Design, Automation and Test IEEE  Computer Society,  p. 156, 2005.    [5]    ISO/IEC,   Information   technology-Lossless   and   near-lossless  compression of continuous-tone still images, International Standard  ISO/IEC 14495-1 and ITU Recommendation T.87, 1999.    [6]    Weinberger M J, Seroussi G, Sapiro G. LOCO-I: a low complexity,  context-based, lossless I mage compression algorithm.  Conference on  Data Compression. IEEE Computer Society , p. 140 1996.    [7]    Misou S G, Kefs, Chen S C. A  lossless  compression  methodfor   medical  image sequences  using  JPEG-LS  and  interframe  coding.  IEEE Trans.  Information  Technology  in Biomedicine.  pp,  818-821.2009.    [8]    Chen Yigang, Deng Jiaxian, Xie Kaiming. Image Compression  Encryption Algorithm Based on Compression Ratio Control of  JPEG-LS.  Journal of Computer Applications , pp. 93-98,2015.    [9]    Nazar F, Murugan S. Implementation of JPEG-LS compression  algorithm for real time applications.  International Conference on  Electrical, Electronics, and Optimization Techniques, IEEE . pp.  2772-2774, 2016.    [10]    Wang Z, Klaiber M, Gera Y, et al. Fast lossless image compression with  2D Golomb parameter adaptation based on JPEG-LS.  Signal Processing  Conference, IEEE . pp. 1920-1924, 2012.    [11]    Hairong Wang. FPGA Implementation of JPEG-LS Remote Sensing  Image Coding Algorithm.    $\mathcal{A}^{t h}$   International Conference on Machinery,  Materials and Computer,  2017.    [12]    Lihua Deng, Zhenghua Huang. The FPGA Design of JPEG-LS Image  Lossless Decompression IP Core.  Chinese Automation Congress , pp.  27-29, 2015.    [13]    Label, K. A. , et al. Single event effect proton and heavy ion test results  for candidate spacecraft electronics. 1994 IEEE Radiation Effects Data  Workshop, 1994:64-71.    [14]    Changhe Wang. Effect of Single Event Effect on Satellite Space  Operation Reliability. Semiconductor Information. 1998.    [15]    D. M. Fleetwood and P. V. Dressendorfer. A simple method to predict  irradiation and annealing biases that lead to worst-case CMOS static  RAM postirradiation response.  IEEE Trans. Nucl. Sci , col. 34, no.6, pp.  1408-1413, 1987.    [16]    C. Bernardeschi, L. Cassano, and A. Domenici, SRAM-Based FPGA  systems for safety-critical applications: A survey on design standards  and proposed methodologies.  J .Comput. Sci. Technol , vol. 30, no. 2, pp.  373-390, 2015.    [17]    H. Quinn, P. Graham, J. Krone, M. Caffrey, and S. Rezgui, Radiation  induced multi-bit upsets in SRAM-based FPGAs.  IEEE Trans. Nucl. Sci,  vol. 52, no. 6, pp. 2455-2461, 2005.    [18]    Weinberger, M. The LOCO-I lossless image compression algorithm  Principles and standardization into JPEG-LS.  IEEE Trans. Image  Process. 9(2000).    [19]    Anlong Li, Development and Application of RTL Fault Injection Tool,  Dissertation of Harbin Institute of Technology , 2017.

