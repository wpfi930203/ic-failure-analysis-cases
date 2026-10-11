---
title: "tut-6.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_43c89bdf447f638defce998e282afd377295230462135641
file_size: 9332479
---

## Emerging Memory Technologies Reliability 

Cristian Zambelli

Università degli Studi di Ferrara

![13   9  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/785c35cd-d7b9-44a5-84b1-550fc7c16df9/785c35cd-d7b9-44a5-84b1-550fc7c16df9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=7e0aca160523eac37f939696226c552ca32684c1)
Universita degli Studi di Ferrara

## Objective 

▪  Discuss the operation and the reliability issues of emerging NVM

▪  Phase Change Memories (PCM) ▪  Resistive-switching Memories (RRAM) ▪  Magnetic Memories (MRAM)

▪  Understanding the limitations in the applications enabled by them

▪  Improving the application abstraction level  ▪  With a proper knowledge of the device reliability features

## Outline 

▪ Introduction   ▪ Phase Change Memories (PCM)   ▪ Resistive switching Memories (RRAM)   ▪ Magnetic Memories (MRAM)   ▪ Conclusion

## Outline 

## ▪ Introduction 

▪ Phase Change Memories (PCM) ▪ Resistive switching Memories (RRAM) ▪ Magnetic Memories (MRAM) ▪ Conclusion

## Introduction 

![Storage type - Latency  CPU   Registers - 100ps  Cache  SRAM - 1 to 10 ns   Storage capacity   memory  Main memory   DRAM - 10 t0 100 ns  Non-volatile storage   Flash - 10 to 100 μs  Mass storage   SSD - 100 μs to 1 ms  Bulk storage   HDD- >10 ms  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4f55d0b7-5112-4163-a7bf-9a726b5b12ac/4f55d0b7-5112-4163-a7bf-9a726b5b12ac.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=9bdd03c77bd0c8472bec0beaa391018dbc156eed)
▪  In computer architecture instruction/data storage follows hierarchy ▪  Traditional hierarchy encompasses a mix of memory technologies (DRAM, Flash, etc.) ▪  The closer to the processing element, the faster we are!

[1] C. Zambelli,  IRPS Tutorial  (2023)

## Data movement in the memory hierarchy 

![25pJ   6pJ   Control   70PJ  I-CacheAccess   RegisterFile   Add  Access  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/740d3695-6879-4668-b195-1ad412037d32/740d3695-6879-4668-b195-1ad412037d32.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=0186c9604ce4c6a47a563e4f01eeb44487697cea)
![Operation   EtPJJ   Relative Energy Cost  8bAdd   0.03  16bAdd   0.05  32bAdd   0.1  16bFPAdd   0.4  32bFPAdd   0.9  8bMultiply   0.２  32bMultiply   3.1  16b FP Multiply  32bFPMultiply   31  32bSRAMRead (8KB)  32bDRAMRead   640  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/eca1d98e-0a56-4ade-b92f-3bbe4630a6e1/eca1d98e-0a56-4ade-b92f-3bbe4630a6e1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=b4eadde6128b8a8065f71257d8d7926e60035989)
▪  Moving data from different hierarchy levels

▪  Requires a lot of energy! ▪  Think about moving data from DRAM to NVM…

Key issues to tackle in future architectures

▪  Reduce energy/latency/capacity ▪  Increase bandwidth ▪  Enable computation close to data if possible

▪  What about reliability???

[2] M. Horowitz,  IEEE ISSCC  (2014) DOI. 10.1109/ISSCC.2014.6757323 [3] S. Perri et al.,  presented at IEEE RAW Conference  (2024)

## Time to revise the memory hierarchy 

![ImageSearch  VoiceSearch   Elapsed  Translator  Time [ns]  Data analysis  Neuromorphic  1010   Tape data read  OL）    In Memory   Braininspired  circuits,Spike  Computing   109  neural networks..  Deep Neural Networks,   108   Data storage/Archival  NearMemory   ConvolutionalNeural   NAND Flash block erase / HDD read-write   Computing   Networks   107  von   Tensor Processing   106   NAND Flash page write  Neumann   Unit...  105  CPU   NAND Flash read (without ECC)  104  Computation   103   S-class/M-classScM write  SCN  102   DRAM read/ M-classSCM read  Host system memory  1O:1   CPU cache (SRAM)  Energy efficiency (ToPs/W)   100   CPU clock @ 1 GHz  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/314827de-7c61-402b-bbeb-6c224f8a46cb/314827de-7c61-402b-bbeb-6c224f8a46cb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=c66656a05944dac95401a2fae8150be1101647aa)
▪  A new breed of Storage Class Memories (SCM) is needed! ▪  New set of applications envisioned

[4] G. Molas et al.,  App. Sciences , 11, 11254 (2021) DOI. 10.3390/app112311254 (CC-BY 4.0) [5] C. Zambelli et al.,  Proc. IEEE , 105(9), 1790 (2017) DOI. 10.1109/JPROC.2017.2710217

## Emerging SCMs to disrupt the hierarchy 

![PCM   RRAM   MRAM  TE   TE   FreeLayer  Chalcogenide  layer   Insulator  Tunnel  Active   Layer  region   Layer  BE   BE   Pinned  Layer  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/423e2812-878f-40af-a772-7777a53a216b/423e2812-878f-40af-a772-7777a53a216b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=a78a699ce91999168f90fede251bfac3c1d0685e)
▪  Creating storage using resistive-based devices    ▪  Sensing data controlling  R  rather than  Q  as in SRAM/DRAM/Flash   ▪  Unifying the SRAM/DRAM/Flash benefits

[6] P. Mannocci et al.,  APL Mach. Learn. , 1, 010902 (2023) DOI. 10.1063/5.0136403 (CC-BY 4.0)

## Outline 

## ▪ Introduction 

▪ Phase Change Memories (PCM) ▪  Operation principles and materials for integration ▪  Reliability issues (Endurance, Retention, Drift, Instabilities) ▪  PCM advantages and shortcomings in applications   ▪ Resistive switching Memories (RRAM)   ▪ Magnetic Memories (MRAM)   ▪ Conclusion

## Phase Change Memory (PCM) concept 

![Long low  current pulse   · Write time is = 1 μs  ▪  Write time is ≈ 1 µs (SET)  High resistance   Low resistance  ▪  Read time is ≈ 100 ns  Read time is ≈ 100 ns TE  Crystalline  Short high  current pulse   ▪  Programming through voltage  Programming through voltage SAmorphous  Time   (RESET)  ▪ · Reading through resistance  Reading through resistance BE  · Phase switch (SET/RESET)  ▪  Phase switch (SET/RESET) Time  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5c3c06e8-c9f0-4122-b738-1fa223cb54b9/5c3c06e8-c9f0-4122-b738-1fa223cb54b9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=7836e35583444abba34ac1fa253df438faa0722c)
▪  A nanometric volume of phase change material between two electrodes…

▪

…with a heather element (as we are relying on a Joule effect)

[7] M. Le Gallo et al.,  J. Phys. D: Appl. Phys. , 53, 213002 (2020) DOI. 10.1088/1361-6463/ab7794 (CC-BY 4.0)

## Materials for PCM integration – the GST! 

![Ge   T×(C)  0.0^1.0  310  290  0.2   0.8   270  712-   250  512-   230   storage-oriented  0.4   0.6  highstabiey   412   312GeTe   228   automobileapplications  0.6   212   0.4   170  8211   150  paad   326  1225  0.8   0.2  124  147  1.0   Sb2Te3！   0.0   memory-oriented  Sb 0.0   0.2   0.4   0.6   0.8   1.0Te   computingapplications  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2f199290-470c-46ab-95d1-b0ab80dae68d/2f199290-470c-46ab-95d1-b0ab80dae68d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=0f7eba427565ae925a2a16e09a11e9ce5fdc1cca)
▪  The active material in a PCM cell is a chalcogenide ▪  GeSbTe (GST) layer between confined electrodes   $(\mathsf{G e}_{2}\mathsf{S b}_{2}\mathsf{T e}_{5}$   usually)

[8] L. Sun et al.,  npj Comp. Mat. , 7, 29 (2021) DOI. 10.1038/s41524-021-00496-7 (CC-BY 4.0)

## Activating the PC switching 

𝐸

𝑎

𝑅= 𝑅

𝐵

0

𝑒

𝑘

𝑇

![+30  +20  1O  [n'e]  T=150°℃  T=90°C  T=30°C  20  T=-30°C   1O  30  100   101   102   103   104   25   30   35   4O   45   SO  R[a.u.]   1/KT  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/84ffbc31-877f-40d3-a3c3-996a26ac3f00/84ffbc31-877f-40d3-a3c3-996a26ac3f00.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=191ae143355caa8f62f9aaddf6cc534529ec27a2)
▪  In the pristine state immediately after the fabrication

▪  The chalcogenide material is mostly poly-crystalline ▪  Grains with different elemental content and properties

▪  A forming step could be required for GST activation

[9] M. Baldo et al.,  IEEE IEDM  (2020) DOI. 10.1109/IEDM13553.2020.9372089

## Quasi-static and pulsed characteristics 

![10  [ un   10   Set state  (crystalline)  1C  Reset state  10   (amorphous)  10  0.0   0.5   1.0   1.5  Voltage [V]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/850a00e3-6626-4515-b79d-7778b14146aa/850a00e3-6626-4515-b79d-7778b14146aa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=0570613c86788202e5bd8c41be08715313777fcc)
![100   200300400500600700800900  Programmingcurrent[uA]  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2ef4228c-029e-4b63-b87d-68faabca9cd8/2ef4228c-029e-4b63-b87d-68faabca9cd8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=2748d799107cca18f445bfe2702d58652c6c53f4)
▪  Unipolar device based on threshold switch (see quasi-static I/V) ▪  The pulsed characteristics shows that there is an operation window

[10] N. Ciocchini et al.,  Sci. Rep. , 6, 29162 (2016) DOI. 10.1038/srep29162 (CC-BY 4.0) [11] A. Redaelli et al.,  IEEE EDL , 25(10), 684 (2004) DOI. 10.1109/LED.2004.836032

## Examples of PCM cells with selectors 

![Transistor Transistor   Diode Diode  Bit-line  GST  Metal-2  storage  Element  Word-line  PNDIode  N+B8se  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e2ccfb92-6526-4169-8c34-6ae306402864/e2ccfb92-6526-4169-8c34-6ae306402864.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=79a0d578ad79740c6eb842013713249780ccc437)
▪  PCM cells integrated in array structures  ▪  Need a mechanism for addressing them during read/write ▪  Since passive they need a device to provide SET/RESET current  [12] F. Bedeschi et al.,  IEEE JSSC , 44(1), 617 (2009) DOI. 10.1109/JSSC.2008.2006439 [13] J.H. Oh et al.,  IEDM  (2006) DOI. 10.1109/IEDM.2006.346905

## Endurance of PCM technology 

![1.E+10  1.E+09    Stuck Set   Stuck   UpperElectrode   Stuck  Upper Electrode  1.E+08   ■Stuck Reset   set   GST   reset  1.E+07   Ge   GST  1.E+06   depletion   Void  1.E+05   Heater  1.E+04   Insulator  BEC  1.E+03   50nm  1.E+02  1.E+01   1.E+03   1.E+05   1.E+07   1.E+09   1.E+11  Number of Cycles  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9ade9e2d-d9d3-4bfb-ad6b-49ab20030162/9ade9e2d-d9d3-4bfb-ad6b-49ab20030162.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=258445114f7b1dffde637c1fbd3beff2088844ea)
▪

PCM devices exhibit an endurance up to 10

10

cycles

▪

Between DRAM

and Flash technology (1

at best) for sure!

▪  PCM endurance fails manifest as stuck-bits usually

[14] Kim et al.,  IEEE IRPS  (2005) DOI. 10.1109/RELPHY.2005.1493077

## Not only GST for PCM… 

![10  Cu-GST/CuO/SiO/BE   CBRAM  OXRAM  6106   Cu/Ta2O5/Pt  PCRAM  Ag/GeS/HfO2  Mopui   Cu/PSE/Ru  1O   TilTaSiO/Ru   GST-O  GST-N  TaN/GeTe/Cy   GST-Sb  buiuu   GST/CuO/SiO/BE  102  TaON  Ta2O5/TaOx  ox  10  10   102   10\~   10   109   1011  Endurance N.[#]  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2aebeffe-f6cf-4f5f-b686-9a3780d2ffc1/2aebeffe-f6cf-4f5f-b686-9a3780d2ffc1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=326ad92492cd3a420cabba086904ce4f0c80e82c)
▪  PCM material impacts the memory window ▪  Best endurance reported is after GST doping or enrichment

[15] L. Perniola et al.,  IEEE IMW  (2016) DOI. 10.1109/IMW.2016.7495295

## SET/RESET energy role in endurance 

![1.0E+13  1.0E+12  1.0E+11  1.0E+10  1.0E+09  1.0E+08  1.0E+07  1.0EH06  1.0E+05  1.0E+04  1.0E+03  10   10010  Fneroy pei  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8cd93479-d6d6-4298-a16b-f9ecc4a5d80c/8cd93479-d6d6-4298-a16b-f9ecc4a5d80c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=bba625945bb995e6f09104406bc41bec78583ab4)
▪  SET and RESET pulse energy impacts endurance ▪  The higher the energy the lower is the endurance

[16] S. Lai,  IEEE IEDM  (2003) DOI. 10.1109/IEDM.2003.1269271

## Seasoning and structural modifications 

![Seasoning during cycling  S0  I=MKMM  pea.   100K  Voltage Applied [V]  Before   After  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2d20065b-16c4-4c15-af5a-5816eb7945ae/2d20065b-16c4-4c15-af5a-5816eb7945ae.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=23a24c6bffd76efbb88f33223870f2bbb81deb3f)
▪  SET/RESET cycling leads to GST composition modifications ▪  Defined as seasoning or structural changes

[17] C. Zambelli et al.,  IEEE IMW  (2010) DOI. 10.1109/IMW.2010.5488326   [18] B. Rajendran et al.,  VLSI Tech. Dig.  (2008) DOI. 10.1109/VLSIT.2008.4588576

## PCM can be used in SSD products 

||DRAIM|PCIM|NAND Flash|
|---|---|---|---|
|Non-Volatile|10|res|Yes|
|Bit-alterable|yes|Yes|140|
|Software complexity|Simple|Simple|Complex|
|Read Time|~20-50 ns|50-100 ns|25-125 μs|
|Read Energy|～ 0.1 nJ/b|||


|Application layer|
|---|
|        Operating system                Filesystem      |
|        Operating system                Filesystem      |
|Blockdevicelayer|
|Hybrid SSD      SATA, SAS, PCI_e ..|


▪  PCM are bit-alterable (data in-place update)

▪  More Write per Day (WPD) allowed in Solid State Drives (SSDs)

[5] C. Zambelli et al.,  Proc. IEEE , 105(9), 1790 (2017) DOI. 10.1109/JPROC.2017.2710217   [19] C. Sun et al.,  IEEE TCAS-I , 61(8), 2360 (2014) DOI. 10.1109/TCSI.2014.2309780

## Read and Program disturbs in arrays 

![一1   +1  10Years  10°   MaxDisturbCurrent  +1   10°10°10410²10°10²1010°10°1010  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3eacff4a-9053-40a0-91ea-152773f0b2c5/3eacff4a-9053-40a0-91ea-152773f0b2c5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=e90769e2b507f3d1811de985ff5a654f3853f5ec)
▪  Repetitive readout of a PCM cell in RESET state

▪  May provide a modification of its phase

▪  Program degradation of the PCM resistance

![RESET  C   -(I-1,J-1)  ○—(l-1,J)  —口一(1,J-1)  O—(1+1,J-1)  SET   一(1+1,J)  10°10′10²10°1041010°10′10°10°101°10  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7ea31960-8a31-4010-a7b6-8d34cbf2459d/7ea31960-8a31-4010-a7b6-8d34cbf2459d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=32370f7a0f5cf0270acf03f4bd2ef56ebf96300d)
▪  Thermal cross-talk between adjacent bits

[20] A. Pirovano et al.,  IEEE TDMR , 4(3), 422 (2004) DOI. 10.1109/TDMR.2004.836724

## Retention in PCM 

![T[²C]  growwth  300   250   200   150  125  100   80   driven  10  T=190°C  108   10years   10   211090   nucleation  +growth  Retention   106   errhaniuation   2090  failure   =118°C   OurGST  10  I   105  104   130°0  10  nucleation  10  102   Data   driven  Retention   Calculated   1-0  Liifetime  10100   1020   25   ③0   35   1-0  101   102   103   104   10-3   10   10   10   102   102   10  Time [s]   1/kT[ev-]]   Normalized1  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c17a114a-8d0f-4615-a463-1f0ab47369dd/c17a114a-8d0f-4615-a463-1f0ab47369dd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=ea15601b044e13905460dad98ab981dceab4aac1)
▪  Improving the stability of the RESET state (major challenge in PCM)

▪  Thermal stability is challenged by nucleation/growth

▪

Leading to the crystallization of amorphous phase

[21] A.S. Spinelli et al.,  ESREF tutorial  (2010) [22] U. Russo et al.,  IEEE TED , 54(10), 2769 (2007) DOI. 10.1109/TED.2007.904976

## Using PCM in automotive MCUs 

![Serise amp   Viain  PCM   1O   HTDR  array   GST+O  [su] awi iis  10   "Golden”   NGST  GST+Ge+N  Stacked  Ga-Sb-Ge  contactsin  GeTe+N  4MBPCMarray   4MBPCMarral   logic/SRAM  eSDNe  10   GST  GST  GST  GST+Sb  10  ThinSifilm   Speed  Thinburied oxide  Handle substrate  8101   160   ２4０   3２0  PcMarray   Logicarea  Retention Temperature [°℃]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0b421576-17ae-49ef-b2f8-a7c304e0821e/0b421576-17ae-49ef-b2f8-a7c304e0821e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=7d23dd3e4da892fa8390032c683b56c327af8bc4)
▪  Embedded applications (MCU) integrating PCM

▪  Require thermal stability!!! Critical in automotive

▪  Playing with materials can help though trading-off performance

[23] F. Arnaud et al.,  IEEE IEDM  (2018) DOI. 10.1109/IEDM.2018.8614595   [15] L. Perniola et al.,  IEEE IMW  (2016) DOI. 10.1109/IMW.2016.7495295

## Increasing storage density with MLC 

![RESETVerify   SETVerify  0.75 State   State   State   State  Preprogram  toSET   Preprogram  toRESET   0.5   O1   10   TT   VP  RESET   SET   0297.9%979%968%100%  0.125  PulseI   PulseI  0.05  Read   Done   ReadDone  Passtarget   Pass target  RESET   SET  PulseI+△I   PulseI+△I   0.01   d  0.005  Read   CDone   ReadDone   1.5   2.5   35   4.5  Pass target   L Pass target   Resistance (log10(Kohm))  Waveform Time [us]  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bb23b49b-341e-434a-bd20-9c1ff5f095d1/bb23b49b-341e-434a-bd20-9c1ff5f095d1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=b29b16900b9297fbb5ac6f106bbbb078c2560781)
▪  Multi-level capability of PCM technology is an asset ▪  SSD applications and innovative Analog Storage scenario   ▪  SET/RESET algorithms are developed for multi-level ▪  Implemented in array products and optimized

[24] T. Nirschl et al.,  IEEE IEDM  (2007) DOI. 10.1109/IEDM.2007.4418973   [25] C. Zambelli et al.,  ESSDERC  (2009) DOI. 10.1109/ESSDERC.2009.5331471

## Analog PCM storage for Deep Learning 

![1I   412  421   422  431   432.   OLTBA   Ac=b  G21  0PCM chip  x 4x4-bit fixed-point  G12R   322   G32  Exact bvalue  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/90fa1430-6a92-4e6b-9921-936dc84140e7/90fa1430-6a92-4e6b-9921-936dc84140e7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=fe750d26fe1280c3e20cf316143bd290b387a8ec)
▪  In Deep Learning we usually calculate Matrix-Vector Multiplications ▪  The simplest way is to implement a PCM crossbar array ▪  This will calculate Multiplications and Accumulates in one clock cycle!

[26] A. Sebastian et al.,  J. App. Phys. , 124, 111101 (2018) DOI. 10.1063/1.5042413 (CC-BY 4.0) 24

## Resistance drift – The biggest issue 

![0.95  T=25°C 0.9 厦0.85 0.8  R = r。  1-.t0 0.75 0.7 10°  101  102  103 ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9bf160fa-a229-4fb9-ac94-8818e4934c77/9bf160fa-a229-4fb9-ac94-8818e4934c77.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=62b26cfd3b314589d4c14b27519ecc5bacd0cce1)
![0.4  a)  EA0.2  言(b)  ] a  CO  1-5E  m=40 mV dec1  0.5E   n = 30 mV dec   Data-State A  Calculation- State B  10101010410-1021010°1010²1010  DelayTime[s]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/525b163e-e74b-4a9b-a7ed-1f3d86232dd5/525b163e-e74b-4a9b-a7ed-1f3d86232dd5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=f097465dabc606601ae277fbbb44e0b5c27f3023)
▪  The resistance of PCM increases over time referred to as resistance drift ▪  Resistance drift makes it difficult to detect the different states of PCM ▪  Drift is seen as a relaxation over time of  R

[27] D. Ielmini et al.,  IEEE TED , 56(5), 1070 (2009) DOI. 10.1109/TED.2009.2016397   [28] N. Ciocchini et al.,  IEEE IMW  (2012) DOI. 10.1109/IMW.2012.6213673

## Mitigating drift at runtime 

![15-20kQ   25-50kQ   >100kQ  LTPPCM  Spikingpre-synapticNeurons(Input)  ITP   1=ULTP-   Spiking post-synapticNeuron(Output)     (%)  10080  60  D  devices  40  TD  LTDPCM  20  devices   TLEC  PhaseChange Layer  WPiug  45   5,5  Log(Resistance)  BEC  EquivalentSynapse  NoDriftregion   Driftregion  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/dd1f8954-9d13-48df-8693-ba513dc350de/dd1f8954-9d13-48df-8693-ba513dc350de.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=a0377f7ec7b417f5a8e61fff2865bdbaef248f73)
▪  Drift is mitigated at runtime in design-phase ▪  Dummy PCM cells subtracts from drift-affected cells

[29] M. Suri et al.,  IEEE/ACM NANOARCH  (2013) DOI. 10.1109/NanoArch.2013.6623059

## Stochasticity of PCM devices 

![100   0.4.   1_0 -   150ns  Pulse width: 50 ns   2.0u  10  80   0_8   100 ns  0.3  Simulation  60   loe   Gaussian fit   Simulation  Gaussian fit   50ns  mue   0.2  40   40 ns  106   1.8"  04  30 ms  20   20 ns  0.2  Pulse amplitude: 1.8 V  105   0.0-   40-_0=  20   ¥60   ¥80   100120140   8   12   16   20   -8.5   -8.0   -7.5  -7.0-6.5   -6.0   10   15   20   25  Time (ns)   Number of pulses   Log (delay time (s))   Number of pulses  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b399a938-32c5-4903-936b-2957e634ffde/b399a938-32c5-4903-936b-2957e634ffde.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=8d04cae2738769f88317bad6cb506d2d8828739f)
▪

Stochasticity of PCM is observed

▪  Devices switch at different threshold switching voltages

▪  Devices switch with a different number of pulses

[30] M. Le Gallo et al.,  ESSDERC  (2016) DOI. 10.1109/ESSDERC.2016.7599664

## Random Telegraph Noise in PCM 

![△I[uA]  1  8.00   0.05   0.10   0.15  Time [s]   Cycle  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/48075073-694f-4347-a3a7-2fae8fcf5d60/48075073-694f-4347-a3a7-2fae8fcf5d60.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=7ad739084c9b1e86736d66aa9336e2a3651c00bf)
▪

RTN instability is present in PCM in all states

▪  1/f-like spectral behavior

▪  RTN-like behavior is observed during cycling

[31] D. Fugazza et al.,  IEEE IRPS  (2010) DOI. 10.1109/IRPS.2010.5488741   [32] C. Zambelli et al.,  IEEE TED , 59(3), 813 (2012) DOI. 10.1109/TED.2011.2179047

## Outline 

▪ Introduction   ▪ Phase Change Memories (PCM)   ▪ Resistive switching Memories (RRAM) ▪  Operation principles and materials for integration ▪  Reliability issues (Endurance, Retention, Drift, Instabilities) ▪  RRAM advantages and shortcomings in applications   ▪ Magnetic Memories (MRAM)   ▪ Conclusion

## Resistive switching Memories (RRAM) 

![Resistive Switching  Tunneling  Ferroelectric   Eleetrostatic   Memory  Phase Change   Memory Effect  Thermochemical   Memory Effect  Redox-based   Memory Effect  Electrochemical   Switching Effects  Molecular   Memory Effects  Magnetoresistive   Memory  Nanomechanical  Thermo- and electro  chemical switching  PCRAM   phenomena in oxides   MRAM  RRAM  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1c3f6319-7eb3-4d56-b23b-dcbd02e41647/1c3f6319-7eb3-4d56-b23b-dcbd02e41647.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=daa755b73f4dbc062cc78b3fbd61f2272b9d972a)
▪  Many RRAM flavors! Depending on the oxide switching mechanisms ▪  In this tutorial we will focus on Redox-based RRAM

[33] R. Waser et al.,  IEEE   IEDM  (2008) DOI. 10.1109/IEDM.2008.4796675

## HfO-based RRAM cell concept 

![VFORMINg  ▪  RRAM is made by  RRAM is made by  · A dielectric material (HfO considered here)  ▪  A dielectric material (HfO considered here) Pristine   Current   LRS   VRESET  VSET   · An oxide scavenging layer (Ti)  ▪  An oxide scavenging layer (Ti) Set (3)   HRS  ▪ · Two electrodes (TE and BE - TiN)  Two electrodes (TE and BE – TiN)  Forming(1)  Reset (2)   Voltage   Oxygen   ▪  Works on Oxygen vacancy migration  Works on Oxygen vacancy migration Vacancies  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/916e0bf7-9d7b-4115-bb8c-fee39e9aadc9/916e0bf7-9d7b-4115-bb8c-fee39e9aadc9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=44df76f8349c2a5e5a158a44eec26b13ebf87a85)
▪  In pristine state RRAM are in high resistance state (HRS) ▪  By applying a positive forming voltage at the TE (conductive filament growth) ▪  Resulting in low resistance state (LRS)   ▪  HRS is retrieved with a reset voltage

[34] A. Grossi,  Ph.D. dissertation  (2017)

## Integration in array architectures 

![BE  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8fbfe78a-9fd8-4c89-8f58-6588a61ca027/8fbfe78a-9fd8-4c89-8f58-6588a61ca027.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=16491a1bea1aa576a315beea7de0cacb2766ff19)
![VBL  Wss   Voltage Selection(Mode)  A_cols  X-AddressDecoder  Ax[5:0]  BLO   B1.1   BL63  VWL   vss   Vss   WsS  T  WsS   WsS   WSS  A_rows  4kCellMatrix  Ay[5:0]-→  Din-Mode   Wss.   Vss   Vss  RD  Select  WR  VSL   Voltage Selection(Mode)  WsS  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4b8715a3-9687-40ab-b4e1-8da2089a1439/4b8715a3-9687-40ab-b4e1-8da2089a1439.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=9cbf9de77ae91ee48695b5175eb41c0c9914f1a4)
▪  Raw cross-point arrays

▪  Lowest integration footprint (4F 2 ) but issues with sneak-paths

▪  1T1R arrays in embedded applications

[35] S. Ricci,  Adv. Intell. Syst.  (2022) DOI. 10.1002/aisy.202200053 (CC-BY 4.0) [36] C. Zambelli et al.,  ICMTS  (2014) DOI. 10.1109/ICMTS.2014.6841463

## Forming operation – DC versus pulsed 

![99.9  999  Oo Pre-Forming  9Q   — Pulse Forming  G  Pulse Retry #1  Pulse Retry #3  --Pulse Retry #5  DC Sweep Retry  DC-Sweep Forming  10  UAT  READ  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/36513280-2fbd-42a1-8776-e21c9e37d36f/36513280-2fbd-42a1-8776-e21c9e37d36f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=b027ef3f467920640cbb5329521281d9e4ee9cc4)
![一  10nm, amorphous 一  10nm. poly-cryst. 5nm, amorphous    5nm. poly-cryst. 10nmHfo 5nmHfo Crossbar Area, A [nm ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bd37a219-2da3-4e5e-b617-07d8f3987318/bd37a219-2da3-4e5e-b617-07d8f3987318.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=feb98279447563fb53bf9a4a47b884a8b59ff205)
▪  Forming operation enables resistive switching in RRAM

▪  A good uniformity can be evidenced with DC-sweep ▪  However un-optimized energy control reduces yield

▪  Pulse-based forming requires a high energy amount [37] A. Grossi et al.,  IEEE TED , 62(8), 2502 (2015) DOI. 10.1109/TED.2015.2442412 [38] B. Govoreanu et al.,  IEEE IEDM  (2011) DOI. 10.1109/IEDM.2011.6131652

## Set/Reset operations basics 

![100   V.>0   VA0   1-40-011   o.  50   c = 80 μA  stop   reset  set   0  30  50  CD  reset  -100  -1.5-1.0-0.50.00.5  ¥1.0   1.5   Reset   VPUSE=3.5V   DCSWEEP  TPULsE=50μs  Voltage [V]   transition   transition   VPULSE=3V  TPULSE  2.5V   Tpu1sE=10μs  =IS:  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/733d8e8c-9b97-45d3-99af-46fbf21c2101/733d8e8c-9b97-45d3-99af-46fbf21c2101.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=f4d37a0a84fd62c4a8ad29ecd9e2a6580a68521e)
▪  Set and Reset operations create and disrupt the filament ▪  A compliance current I C  is required ▪  Set/Reset energy determine switching reliability (…and variability)

[39] S. Ambrogio et al.,  IEEE TED , 61(8), 2192 (2014) DOI. 10.1109/TED.2014.2330200   [40] C. Zambelli et al.,  IEEE IMW  (2014) DOI. 10.1109/IMW.2014.6849387

## The role of the materials (dielectric) 

![(a）   100   100   100  80   80   80  6   60   60  )  4O   ()  AO   )  4O  20   -·-pHfO   20   -pHfO   20   -·-pHfO  -aHfO   aHfO   aHfO  ·-HfAIO   -HfAIO   -HfAIO  C   C  Forming Voltage (V)   Reset Voltage (V)   Set Voltage (V)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/04d3fd0a-b99f-4b43-9c05-ab17fcdde104/04d3fd0a-b99f-4b43-9c05-ab17fcdde104.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=089f0ab95a930825967722c36396fa25d5732ec6)
▪  Poly-crystalline HfO (pHfO) has a lower forming voltage ▪  …but difficult Set/Reset control ▪  Amorphous HfO (aHfO) is generally used in integration ▪  Doping HfO with Al (HfAlO) improves the operation control [41] V. Milo et al.,  APL-M , 7, 081120 (2019) DOI. 10.1063/1.5108650 (CC-BY 4.0)

## The role of the materials (deposition) 

|Proc.|Precursor|Tdep (°C)|Carbon content|Oxygen content|Microstructure|
|---|---|---|---|---|---|
||THLA|300|0.396|5896|poly-crystalline|
||HLA|150|0.496|5696|amorphous|
||110|300|796|4996|amorphous|
||11O|150|996|4196|amorphous|


![[] Aeq   20  Forming  00007005040302010   ABC   Seset  FORM  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a961f0d6-2e52-405b-987f-c3b065887e8f/a961f0d6-2e52-405b-987f-c3b065887e8f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=50137aa4884e23d3f012a99cd6f6b5e9443f426a)
▪  Metal-Organic precursor (MO)  ▪  High carbon content means low Forming voltage and RW   ▪  Halide precursor (HA) achieves best performance ▪  Benefit for the read window (LRS/HRS read current ratio)

[42] A. Grossi et al.,  Sci.Rep. , 8, 11160 (2018) DOI. 10.1038/s41598-018-29548-7 (CC-BY 4.0)

## RRAM endurance characteristics 

![CBRAM:  This work:  [1]LiuESSDERC2009  Median  [2]TadaIEDM 2010  Median±20   [3]TadaIEDM 2012  [4]BarciIMW2015  [5]BelmonteIMW2013  [6]VianelloIEDM2012  OOxRAM:  [7]KimVLSI2011  TestSetupLimit  [8]FantiniVLSI2014  [9]KawaharaISSCC2013  [10]VianelloIEDM2014  [11]ChenVLSI2014  [12] Goux VLSI2014  6  111  121  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1431fbfc-2731-4a06-a7f4-44f36885ac15/1431fbfc-2731-4a06-a7f4-44f36885ac15.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=565e852438e3ede62d1f736640261e2cf22de18b)
![Test Setup Limit  OResetIcc=2mA  Reset I=2.2mA  Reset Icc=2.5mA  Reset Icc=4mA  10   10   10  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/683e889d-12b2-4bc6-9d6c-b2b65871c6e4/683e889d-12b2-4bc6-9d6c-b2b65871c6e4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=773472763d85ba94169ec7d3e4437f8b04bef82f)
▪  The achievable switching cycles count (Set/Reset) ▪  Is a function of the operating conditions  →  Reset-dependent   ▪  Different RRAM technologies expose a trend ▪  High switching cycle count  →  Lower resistance ratio

[43] A. Grossi et al.,  IEEE IEDM  (2016) DOI. 10.1109/IEDM.2016.7838348

## Explaining the endurance wear in RRAM 

![overSET   electrode  LRS  RESET   HRS   cFgap  HRS  LRS  CF  SET  electrode  0   10   OverSET   OverRESET  Endurance  Cvcle  overRESET   MoreVo  Recombined   Increased  cFgap  HRS  RS   Original  CF  AccumulatedVo  10   10   CF:conductivefilamentVo:oxygenvacancy  Endurancecycle  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/495fddac-8812-487d-a4d7-e803a850c824/495fddac-8812-487d-a4d7-e803a850c824.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=869b521f4c04158a85f98adb9bcfab580e65170a)
▪  “Over-SET” due to oxygen vacancies (V O ) ▪  Generation during Set operation  ▪  “Over-RESET” from V O  and ion   $(\mathsf{O}_{2\cdot})$   recombination

[44] P. Huang et al.,  IEEE IEDM  (2013) DOI. 10.1109/IEDM.2013.6724685

## Retention of RRAM devices 

![10H   endurance cycles  ELRS   -a-Forming  TE   TE  Oxygen   -1 cycle  \*10 cycles  scavenginglayer   100r  HRS   TTH   \*100 cycles  Oxygen   ono  10r   LRS-250℃   e0  300K   Reset   0-10K cycles  1K cycles  HfO   Hfo   -LRS_150C   itsIs   +100K cycles  Ov   -HRS_250°CFM/SET   set   1M cycles  BETiN   BETiN   100p   HRS_200℃C CC 40μA  10M cycles  Oxygendiffusion from Hf TE   N   V。 diffusion out of   10p-HRS_150℃ 40nm.cell   30   100M cycles  0.01   0.1   100   1000   10-4 10-3 10-2 10-1.10° 101 102 103  the filament  Retention time [hours]   Time (hour)  ta  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2f8fe4c9-2027-4abc-a411-c4cb28618e7e/2f8fe4c9-2027-4abc-a411-c4cb28618e7e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=495f3a57f1e17c59c793f1769b5fb37641c99ef6)
▪  The principal mechanism for retention loss ▪  An out-diffusion of the vacancies in the conductive filament   ▪  Low Temperature Data Retention (LTDR) is a function of endurance   ▪  High Temperature Data Retention (HTDR) have limitations in cycled device

[45] Y.Y. Chen et al.,  IEEE IEDM  (2013) DOI. 10.1109/IEDM.2013.6724598   [46] H. Yamanazawa et al.,  SNW , 2014 DOI. 10.1109/SNW.2014.7348598

## RRAM in automotive scenario 

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/014b5e6a-5b89-4862-b2d0-5da4ba04ac2f/014b5e6a-5b89-4862-b2d0-5da4ba04ac2f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=028c2aa74f527ccb1d2422ce3b73a05b56e67fde)
![0.999999999  0.9999999  0.999999   HRS initial  0.99999  HRSafter6h175°C  0.9999  0.999   -..-LRSinitial  0.99   ----LRSafter 6h 175°C  0.9   --readlevel  O.5.  0.1  0.01  0.001  0.0001  0.00001  0.000001  0.0000001  0.000000001  Cell current(a.u.)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/17b0d754-21c7-4f92-970d-380716431f90/17b0d754-21c7-4f92-970d-380716431f90.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=13f5981c818320249472daa8efbf9fabac5a792d)
▪  28 nm RRAM test vehicle integrated in MCUs is currently under study

## System-level mitigation of RRAM wear 

![ap   Chipfloorplan   Main Memory (RRAM)  (systemwithon-chipRRAM)  e.g., 512 bits per word  Main memory:   (corresponds to a cache line)  on-chip RRAM (1T-1R)  Memory controller   Address  Data in Data out  Interconnect   Record  WRITER  Address   Mechanism (c)  Computing   ENDURER  elements   Mechanism (b)  Shared SRAM memory  Address  Data in Data out  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/47728166-7056-44d6-9308-a92ac47b8ac6/47728166-7056-44d6-9308-a92ac47b8ac6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=3d3ce7804f92110c6d4a9334d35fa2542471c515)
![Address   Datain   Dataou  一一  Fullly  Address   associative  Periodicremappi   checker   SRAMbuffer  PRNG  Offset  Timer  Reg  Ck   Address   Datain   Databut  (C)_WRITER   Connections to RRAM main memory  Error correctiontable (ECT)   Address  Datain   Dataout  Multiple records (e.g., 2-3)  perEcTentry    Data read register  Drdto   Recordwrite   Priority  XOR  ECT   registe  ECT  inmVali bir from   Recordread  record   decoder   XOR  ECT   registe  Faulty bit location   Address  word in main memory)  (e.g., 9 bits for 512-bit  toECT   Address register   Data write register  Address   Data in   Dataout  con   sfromENDURER  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5bb3c8e4-60bb-4008-b966-58a1fc91ad0f/5bb3c8e4-60bb-4008-b966-58a1fc91ad0f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=e7250b40c7fdf28cec11b0a8649fd789c8a53a9f)
(b)ENDURER Connections toWRITER and RRAM mainmemory

▪  Using a similar approach as in Flash memory ▪  Periodically re-mapping the content of the RRAM

[48] A. Grossi et al.,  IEEE TED , 66(3), 1281 (2019) DOI. 10.1109/TED.2019.2894387

## MLC capabilities of RRAM devices 

![<D>  150  250   250   250  100   IGVVA-100   OIGVVA-10  200   200   200  150   150   150  0   100   C   OO  Set  -50  S0   50  100  Reset  -150   0-5   0.5   0.5   1.5  -2-1.5-1-0.50 0.5 11.5 2   VTE[V]   Vsv]   Vev]  Voltage [V]   2   (D)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b288dae5-20ca-4de9-8ac9-1cea3f800f41/b288dae5-20ca-4de9-8ac9-1cea3f800f41.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=11f275b4e76feed9b75e9d68ede3fe38ae0dea6b)
▪  Multi-level in RRAM is an asset for many scenario

▪  Mainly through IC modulation  1.41  ▪  Using either ISPVA or IGVVA program and verify algo. ▪  Gradual tuning of  R(G)  to reach analog storage!!!

![VTE  VTE  1.61  ISPVA   IGVVA  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/72ed45f5-7d04-4e44-8dee-a11c820bfad3/72ed45f5-7d04-4e44-8dee-a11c820bfad3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=0f05e9f4e20cd83192121a664e3ea66cd3f6f6c6)
[49] V. Milo et al.,  IEEE IRPS  (2021) DOI. 10.1109/IRPS46558.2021.9405119   [50] V. Milo et al.,  IEEE TED , 68(8), 3832 (2021) DOI. 10.1109/TED.2021.3089995

## Variability of RRAM – The big hurdle! 

![R<1/G。  R>1/G。 1D TN  TN 1/G。 N° of defects 10S  10 follows a Poisson Law 10  Forming data  10  Fig. 10 (a), Set Icc≤1mA Fig. 10 (b) PotentialBarrier  103  =VG,e-αR1.5  10  Fig. 10 (c), Tset≤200ns Fig. 10 (d), Reset ICc≤3mA  Fig. 10 (e) 101   α 01ccR2  10  1/G。 Fig. 10 (f), TR  ≤10s 10 10  104  10S  106  102  104  I0S  1D TN  TN  ● Oxygen ions  Median R [Q]  Median R [Q] ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d7e0a362-85bd-43a5-89e2-904228013437/d7e0a362-85bd-43a5-89e2-904228013437.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=8c10bb20649cabab8e18d4bf7265537c0f647dbc)
▪  RRAM devices suffer from large variability   ▪  R < 1/G 0  (G 0  = 1/12.9 kΩ)  →  σ defined by dispersion of IC at Set   ▪  R > 1/G 0    →  σ defined by σ HRS  law

[43] A. Grossi et al., IEEE IEDM (2016) DOI. 10.1109/IEDM.2016.7838348

## Intra- and Inter-cell RRAM variability 

||R|
|---|---|


![1 cell,4k cycles  4kcells,1 cycle Set=50uA Set=200uA  米 Set=400μA Reset=2mA IG Median R [Q] ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0ae4f1ff-b421-4299-ae0b-05b6ae81926c/0ae4f1ff-b421-4299-ae0b-05b6ae81926c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=d632cdb28989ab0fe687927207c1360162c92b2a)
▪  Cell-to-cell usually defined as D2D (Device) ▪  Cycle-to-cycle usually defined as C2C

[43] A. Grossi et al., IEEE IEDM (2016) DOI. 10.1109/IEDM.2016.7838348

## Variability impact in RRAM-based circuits 

![nput-sta   MUx-stage  3.5  （a)  BIN   Vdd =1V,T=25°C   Vdd=1 V,T=25°C  0.6   LRS1   fclk = 10 MHz    3.0   ILRS1    fcLk = 10 MHz  miie   Tiie   Tiie   LRS2   LRS2  0.5   LRS3   0=1.3ps   2.5   ILRS3  μ = 27.91 ps  CMOS   CMOS  0.4   W2.0   =0.97 ps   =0.26aJ  P0.3   0=1.02ps  μ=19.39ps   1.5   μ=3.46aJ  =0.25aJ  μ=20.53ps   μ=3.68aJ  0.2   1.0  0=1.01ps   =0.26aJ  u=22.41ps   μ=3.95aJ  niie   Tiie   0.1   0.5   = 0.21 aJ  μ=3.06aJ  12   16   20   24   28   32   0.95   2.5   3.5   4.5  Delay [ps]   Energy Consumption [aJ]   ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2636083e-1f68-4ee4-8e3a-54bd19a8989c/2636083e-1f68-4ee4-8e3a-54bd19a8989c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=91f5db48ca8eade82fc5f0837c9246a7ae3be134)
▪  RRAM-based FPGAs are delay-sensitive by the resistance variability ▪  Reducing energy-consumption with LRS modulation ▪  …produces unwanted energy increase at run-time

[51] T. Rizzi et al.,  IEEE IIRW  (2022) DOI. 10.1109/IIRW56459.2022.10032753

## Read disturb in RRAM 

![State2  State1  V.=0.1V  V=0.1V  Symbol:Data   V,=0.2V   Line: Trend  V,=0.2V  V=0.3V   Symbol: Data  V=0.3 V  20   10   60   80   1010   201   210   601   28:10   1-0101  Read Time (s)   Read Time (s)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/15637ed6-94fb-425b-a99e-96157cd541ab/15637ed6-94fb-425b-a99e-96157cd541ab.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=72621d19dbda58e8544c13d4f195d622bf540c69)
▪  Read disturb is present in RRAM technology   ▪  High resistance states are the most affected   ▪  There is a dependency on the programmed level and read voltage

[52] L. Wu et al.,  IEEE JEDS , vol. 9, pp. 1257-1261 (2021) DOI. 10.1109/JEDS.2021.3110877 (CC-BY 4.0)

## Resistance drift in RRAM devices 

![0.9999   0.9999  0.999   0.999   ③  0.99   0.99  0.9   0.9  0.5   0.5  EA  1T  0.1   AS   O.1  24h  EA  0.011   0.01   72h  V  0.001   0.001   168h  0.00011   0.00011  50   100   150   200   250   300   25   50   25   100   125 150 175  Conductance [uS]   Conductance [uS  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fcf65a69-3a1c-4043-8ce2-332f9642f987/fcf65a69-3a1c-4043-8ce2-332f9642f987.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=3088c6a6e6cfc8c8fcdde5db6f94fa4e60d778ff)
▪  Drift of the resistance (conductance) distributions

▪  Low conductive states are the most affected

▪  Occurring even during the multi-level program algorithm

▪  Drift is highly temperature dependent

[53] A. Baroni et al.,  IEEE IIRW  (2021) DOI. 10.1109/IIRW53245.2021.9635613

## Drift mitigation at device-level 

![Change   ML-SetML-HybridBoth   22  RRAM   0.9999   L2L3L4L5L6L7L8L9  Selectthe   201   Increase VG   device   0.999   L1S  first RRAM  andapply   0.99   18   L2s  device   O!Oi IGVVA Set  RESET pulse   L3S  NO   0.9   16   000   @168h  CD  Apply   Apply1st   LRS   ast   0.5   L1B  SET(L8)   YES   YES   L2B  SET   target   RRAM   G12  L3R  pulse   0.1  Apply1st   101   L4R   日日日   IGVVARese  @168h  RESET   NO   YES   0.01  pulse   IncreaseVTE   0.001  EndML-Set  andapply   0.0001   8  SETpulse   255075100125150175200225250  -Set operations   End ML-Hybrid   Conductance[μS]  -Hybrid operations   10   100   10   10<   103  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/162cabb6-88ee-4954-97e8-4bcc3773add5/162cabb6-88ee-4954-97e8-4bcc3773add5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=4536974bc583b9c175a7a0edefa5f4fbf30c52bb)
▪  Drift can be mitigated through algorithms optimization ▪  Hybrid program and verify algorithms proposed ▪  Initial Set to high conductance and successive gradual Reset

[54] A. Baroni et al.,  Fron. Neurosci. , 16 (2022) DOI. 10.3389/fnins.2022.932270   [53] A. Baroni et al.,  IEEE IIRW  (2021) DOI. 10.1109/IIRW53245.2021.9635613

## Drift mitigation at application-level 

![RRAM Measurements  Q: 2590   ：25\*0   5:25°0  0.9  E: AS   or: oh   @1: 24h  M   0.8  4: 8540   4: 85+0   4: 85\*0  Q: 48h   Q: 72h   8: 16ah   Extractlon  F: Set   Senpt   0.6  0.5  .1  RRAM Interface  0.3  System Simulation  CtH  0.2  Mapping   Suant.  Imputs  DSP   DMAC   Voltage Stimull  syBiaM   Guant.   Decomp.   Mapplng  L1,L2,L3,L4   L1,L2,L3,L4   L1,L3,L5,L7   L1,L3,L5,L7  DSPyProgran   Conductances  25', Set, LcRM   25°, Set, HCRM   25", Set, LcRM   25°, Set, HcRM  OSP   ADC  Mapping and   Quantization   Cutput  CuP.   Recomposition   oh   2h   48h72h   168h   Reference  Curments  ▪  Simulation RRAM engines can help in exploring drift-mitigation states mapping 0+   DDAN  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/83ed3860-0d8b-403f-87c3-a1d18d376533/83ed3860-0d8b-403f-87c3-a1d18d376533.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=49d2f8f34a71f83547484e6d7e0fce4ceb4722f1)
[55] D. Reiser et al.,  IEEE NEWCAS  (2023) DOI. 10.1109/NEWCAS57931.2023.10198076

## Random Telegraph Noise in RRAM 

![Ca   LRS  2400-  50  2200   50  2000   LRS   pee    pea\~ d-d   suo= d-d    n  30  1800-  1403   20   HRS  00000040020   a  10   10：   TE   TE  HRS   de-activated  510 15 20 25 30 0.000.050.10   traps  1012141618202224262830   Time[s]   RelativeFrequency   d-d   Activated  Time [s]   traps  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c5afa2e8-2175-4e96-9f8c-9b1cd1267caa/c5afa2e8-2175-4e96-9f8c-9b1cd1267caa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=11addda0037532e01ffed5d7ba1d5000ec13c07a)
▪  RTN affects the current through the RRAM device

▪  It is attributed to the mechanism of activation/deactivation of the electron traps

[56] D. Veksler et al.,  IEEE IRPS  (2013) DOI. 10.1109/IRPS.2013.6532101

## Outline 

▪ Introduction

▪ Phase Change Memories (PCM)

▪ Resistive switching Memories (RRAM)

▪ Magnetic Memories (MRAM)

▪  Operation principles and materials for integration ▪  Reliability issues (Endurance, Retention, and Disturbs)  ▪  MRAM advantages and shortcomings in applications

## ▪ Conclusion 

## The concept of Magnetic RAM (MRAM) 

![BB  Exchange  splitting  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/5c6caa86-9ffb-4326-b8c3-ee946c088a33/5c6caa86-9ffb-4326-b8c3-ee946c088a33.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=ef10fbecc259f5be57fbc22a09c9988d8082bb4f)
Good band matching. high current, lowresistance

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e970b72e-29d0-4afd-b901-8f4937d3a144/e970b72e-29d0-4afd-b901-8f4937d3a144.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=4cab2832baf21d2c9816566b3e20e3639872820e)
▪  Magnetoresistance effect exploited ▪  Parallel configuration R low   ▪  Anti-Parallel configuration R high ▪  MR = (R high /R low -1)\*100% ▪  RA = R low  \* Area ▪  State of bit detected as a  R  change ▪  In MRAM the data is stored in magnetic polarization ▪  Assuming a Storage (Free) layer and a Reference layer

[57] D. Apalkov et al.,  Proc. IEEE , 104(10), 1796 (2016) DOI. 10.1109/JPROC.2016.2590142 52

## Many MRAM versions available 

![Magnetoresistance   Spin Manipulation  Device Applications  (read-out technology)   (writing technology)  MR ratio at RT & low H  Year   HDD read head   Oersted field  AMR effect  1857   (since 1820)  MR=1-2%   Inductive  head  1985  GMR effect  MR=5-15%  1990  MR head  TMR effect with  1995  amorphous Al-O barier  MR=20-70%  GMR head   Spin-transfer  Non-volatile  Torque(STT)[6-8]  2000   memory  GlantTMRefect[1-]  TMR head  with MgO(001) barrier  2005   Toggle MRAM[5]  MR=100-600%  (in-plane M)  MgO-TMR  head[4]   Voltage-induced  2010  Novel   toraue [18-20]  STT-MRAMI9,10]   devices  (in-plane M)  2015  STO[23].STD[24]  STT-MRAM[11-13]  (perpendicularM  Spin Dice [26]  Voltage-torque  MRAM (?)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2cacf573-5a41-4c69-afba-0bbdc6cbfaf3/2cacf573-5a41-4c69-afba-0bbdc6cbfaf3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=c5f2e3bdc71e5e609e31663e7a982bf03389d416)
▪  In Different MRAM concepts integrated

▪  (a) Field Write   ▪  (b) Thermally Assisted Switching (TAS)   ▪  (c) Planar Spin Transfer Torque (STT)   ▪  (d) Perpendicular STT (pSTT)   ▪  (e) Double barrier pSTT   ▪  (f) Domain-wall propagation   ▪  (g) Spin Orbit Torque (SOT)

▪  In this tutorial we will focus on STT-MRAM

## The interest in STT-MRAM devices 

![Spin-polarized  current（llMRL)  Polarizer   Outgoing  Spin-polarized(l|M)  Incoming  STAE  current   VIR   current  a   D  1.0  Prec  danp   SZ   danp  prec   0.51   TP  P   STT  STI  0.0  1  -0.5  1.0  -1.0  -1.0  0.5  -0.5  00  0.0  OORL   -0.5  V   0.5  10-1.0  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/498b999e-1cdf-4335-bd01-c7192f80e108/498b999e-1cdf-4335-bd01-c7192f80e108.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=a0010874016fd3aafdb3840f6b7501e74fb02ab9)
▪  Current between two ferromagnetic layers  ▪  Separated by a non-magnetic spacer ▪  Exerts a torque on the magnetization   ▪  Development of CoFeB-based free layers ▪  With MgO insulator    ▪  With synthetic antiferromagnet (SAF)    ▪  Landau-Lifshitz-Gilbert (LLG) model   ▪  Explains the magnetization dynamics

[57] D. Apalkov et al.,  Proc. IEEE , 104(10), 1796 (2016) DOI. 10.1109/JPROC.2016.2590142

## MRAM array integration on products 

![SL  RATJ   WL-WL-   T  S   BL-High ->Low   Low -> High  ▪  The 1T-1MTJ structure  The 1T-1MTJ structure · Uses one transistor as a select device  ▪  Uses one transistor as a select device ▪  Magnetic Tunnel Junction (MTJ)  Magnetic Tunnel Junction (MTJ)  · Area footprint like DRAM  ▪  Area footprint like DRAM · Integrated between metal layers  ▪  Integrated between metal layers · MTJ connected directly to Bitline  ▪  MTJ connected directly to Bitline ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/981826cb-5609-4e43-b385-633899e0dbef/981826cb-5609-4e43-b385-633899e0dbef.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=f39fa49148d45764f2f0110569807607e5d9cb06)
[59] D. Shum et al.,  Symp. VLSI Tech.  (2017) DOI. 10.23919/VLSIT.2017.7998174   [60] T. Andre et al.,  IEEE IMW  (2017) DOI. 10.1109/IMW.2017.7939104

## Write operation principles in STT–MRAM 

![Writing"o"   Writing“1"   800  600  → AP switching  400  200  十十丰  -200  C2   ON  400  AP → P switching  -600  -800  10-9   10-8   10-7   10-6   10-5   10-4   10-3  Write pulse width t (s)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b869fcfc-5977-44af-8b09-559fdd9fe285/b869fcfc-5977-44af-8b09-559fdd9fe285.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=248759daebe549572390d3962d248fd024343a7e)
▪  To write the parallel configuration ▪  Current flow of density  $>$   Jc is sent through the MTJ ▪  From the storage layer to the reference layer

▪  KuV anisotropy energy ▪  τ 0  \~ 1 ns ▪  k B T thermal factor ▪  J c0  critical current ▪  Write speed 1 – 10 ns

▪  To write the antiparallel magnetic configuration reverse the polarity [5] C. Zambelli et al.,  Proc. IEEE , 105(9), 1790 (2017) DOI. 10.1109/JPROC.2017.2710217

## Stochastic switching in STT–MRAM 

![Tnpu   No input  No input  No input  08  LIF neuron  1.13Vo   Lane 0Lane 1  Lane2  Lane   Lane4  Lane5  1.26V  LIH' neuron  1.41Vo  1.6Vo  Ｓ   67   8910  Programming Pulse Duration △t (ns)  · STT-MRAM switching mechanism of MTJ  ▪  STT-MRAM switching mechanism of MTJ  · Has been revealed intrinsically stochastic  ▪  Has been revealed intrinsically stochastic State:  · Which results from thermal fluctuations  ▪  Which results from thermal fluctuations  LAP  CP  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e2786343-a3ef-4cca-ba48-62880a7c2d41/e2786343-a3ef-4cca-ba48-62880a7c2d41.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=cbf4d1bc769eea98b652717f7773b1bd8cf321c2)
▪

Analog behavior can be emulated

[61] A. Vincent et al.,  IEEE TBIOCAS , 9(2), 166 (2015) DOI. 10.1109/TBCAS.2015.2414423

## Voltage distribution in STT-MRAM 

![VRead   Wwrite   Breakdown  10-1  10-2  10-3  10-4  10-5  e   10-6  10-7  0_4   0.8   1.2   1.6  Voltage(V)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fa0b79a9-68ca-4d42-b541-7017f3b23f7c/fa0b79a9-68ca-4d42-b541-7017f3b23f7c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=2abe99b1e6867f177d72d11bb2c18b9c9e3ff987)
▪  Write and read current paths are the same

▪  To avoid write disturbance during read

▪  The read voltage must be lower than the critical write voltage

▪  Each write event exposes tunneling barrier to stress [5] C. Zambelli et al.,  Proc. IEEE , 105(9), 1790 (2017) DOI. 10.1109/JPROC.2017.2710217

## The STT-MRAM manufacturing process 

![Staticrepeatability   Staticrepeatability  a   RA vs.OBM Thickness   TMR vs.OBM Thickness   MgO（x20）   CoFeB(x20)  10.10   20.10  16   190   10.08   20.08   （6）  10.06   20.06  20.04  (wm-)   185   28-88  19.98  180  19.96  10   99   19.94  190   175   9.92   19.92  170  150   170   Dynamicrepeatability   Dynamicrepeatability  130   9.49.69.8  1010.2 10.4 10.6   9.49.69.8  1010.2 10.4 10.6   MgO（x10)   CoFeB(x10)  10.6   20.6  118   OBM Thickness (A)   OBM Thickness (A)   10.4   C   20.4   d  10_2   20.2  50   100   150   200   10.0   20.0  Annealtime at 400°C(min)   98   19.8  196  ▪  The fabrication of nanopillars  The fabrication of nanopillars  19.4  Radius1Radius2Radius3  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bc99776e-722f-440a-a4af-ce4353e2b4d6/bc99776e-722f-440a-a4af-ce4353e2b4d6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=95ded079bbc648ec4e1925aec6aa6c166c61de8d)
▪

Critical down to 20 nm since MTJ involves mat. insulators, magnetic, non-magnetic

▪  Two commonly used methods

▪  Reactive Ion Etching (RIE) and Ion Beam Etching (IBE)

[62] R. Whig et al.,  IEEE IMW  (2019) DOI. 10.1109/IMW.2019.8739745

## Switching probability – Bit Error Rate 

![1e+0  (a)  1e-1   a  1e-2  1e-31  Eqs.(1-2)  1e-41  Eqs. (2-4)  1e-5   otp=40ns  m1e-61   otp=150 ns   10  1e-71   otp=500ns  1e-81   O   otp=1μS  1e-91   10   tp=10μS   10  1e-101  Reset  1e-111  -0.5-0.4-0.3-0.2-0.1   0.10.20.30.40.50.6   10-0.5   -0.4   -0.3   0.③   0.4   0510  VC(TJ)   Voltage[V]   Voltage[v]  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cc189012-085c-4594-8656-b5c15e18c1ea/cc189012-085c-4594-8656-b5c15e18c1ea.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=cbbbc37f2a4dd40e40263fd28a23b9820b2cebd9)
▪  With the Jc at a given pulse width we implied

▪  Average switching current density   $(50\%$   of switching prob.)

▪  For a successful memory product is not enough

▪

Full memory must be repeatedly written with very low Bit Error Rate (BER)

[63] J. J. Nowak et al.,  IEEE Magn. Lett. , 2 (2011) DOI. 10.1109/LMAG.2011.2155625   [64] R. Carboni et al.,  IEEE TED , 66(10), 4176 (2019) DOI. 10.1109/TED.2019.2933315

## Read disturb in STT-MRAM 

![660   80   1-010  Thormal Stability Factor (A)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/751a4138-d5f9-4b06-8740-ba21b6057fa8/751a4138-d5f9-4b06-8740-ba21b6057fa8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=aab1812888a90ba38c4a2e099542d45c3554d789)
$$\begin{array}{r}{F_{c h i p}=1-\exp\Bigl[-N\frac{\tau}{\tau_{0}}\mathrm{exp}\Bigl(-\varDelta\Bigl(1-\frac{I_{R}}{I_{C O}}\Bigr)\Bigr)\Bigr]}\end{array}$$
F chip  is the failure probability ▪  N number of bits to read  ▪  I R  read current ▪  I C0  critical switching current ▪  Δ thermal stability factor

▪  Read operations in STT-MRAM drive soft errors  ▪  As the read current can erroneously change the stored data ▪  A higher Δ is needed to avoid failures (read disturb level usually 10 -9 )

[65] N. Sayed et al.,  IEEE TVLSI , 27(6), 1329 (2019) DOI. 10.1109/TVLSI.2019.2903592

## Endurance of STT-MRAM 

![(G-[)u7-)u7  1O  12  t+ar   4a   s+at   94a1  cycles/bit  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f37ce773-f7a1-4357-aca6-f5dde127c4e4/f37ce773-f7a1-4357-aca6-f5dde127c4e4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=2e59eb2be1913ae2cfa4f9ab9004a6465fcc1e5f)
▪  Endurance in STT-MRAM is measured

▪  At increased voltage and projected to operating voltage

▪  For a given voltage, a cell is constantly written and read until it breaks down

[60] T. Andre et al.,  IEEE IMW  (2017) DOI. 10.1109/IMW.2017.7939104

## Explaining the endurance wear 

![(d>  applied  （a   （D>   CC   CD>  EE   BE  mgo  CoFeBFreelayer   107  MgO  Calc.  Defect   Defect   t=100ns  CoFeBPinnedlayer   (1)generation   (2) activation   tp=1μs  tp=10μs  R。 ～eαV+   R。\~ eβIV-1   tp=100μs   /=0.8  10  04   0.6   08  10  Voltage[V]  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/737795ee-49ab-4eca-9bdd-8b8b4eb3d093/737795ee-49ab-4eca-9bdd-8b8b4eb3d093.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=7f733190550fce6c5fd60e93baf40c04fea589a3)
▪

Endurance in STT-MRAM is limited

▪

By dielectric breakdown of the MTJ in the MgO

▪

Endurance wear can be modeled as function of

▪

Stress pulse width and voltage and device area

[66] R. Carboni et al.,  IEEE TED , 65(6), 2470 (2018) DOI. 10.1109/TED.2018.2822343

## STT-MRAM used as cache memories 

|        Example Use                Case      |        MEMORY SIZE                (MB)      |Assumptions|        10 Year Endurance                Requirement      |
|---|---|---|---|
|L2 Cache||108 access/sec, 40% write traffic|7.7 × 1011|
|L3 Cache||107 access/sec, 40% write traffic|1.3 × 1010|
|Unified eNVM||        1.6 GBps, 64-bit I/O, constant write                traffic      |1.6 × 1010|
|IOT Unified||400 MBps, 64-bit I/O, 1% duty cycle|1.3 × 109|
|R.A.A.|N/A| 50 ns attack period, 100% duty cycle|6.3 × 1015|


$100\;\%$

![1.E+13 1.E+12 1.E+11 --·---L2SRAM（256KB) 1.E+10  ---L2MRAM（1024KB） ·-L3SRAM（1.5MB） -L3MRAM（6MB） 1.E+09 20  4O  80  100 Millionsofcacheaccessespercorepersecond ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/73783ace-0b5d-4748-853d-ec0a5286ea0f/73783ace-0b5d-4748-853d-ec0a5286ea0f.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=56ec4cad4c294d7d741866f7462cf55b08e78415)
▪  System-level workload characterizations

▪  Suggest that the endurance of STT-MRAM is “unlimited” ▪  Exceeding the requirements of various memory use cases

▪  STT-MRAM can be used as non-volatile caches

[67] J.J. Kan et al.,  IEEE TED , 64(9), 3639 (2017) DOI. 10.1109/TED.2017.2731959

## STT-MRAM used in SSDs 

![Complete DRAM replacement   DRAM complement  FTLCode  MappingTable   Mapping Table   STT-MRAM  Datacache  FTLMetadata   FTLMetadata   Data cache  Hotdata  STT-MRAM  一一一一  Mapping Table   Datacache  FTL Metadata   FTLCode  Data  DRAM  FileSystemData  Data  NANDFlash  NANDFlash  File System Data  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f1ea9d3b-776c-4be6-8d3b-2d00fed0714e/f1ea9d3b-776c-4be6-8d3b-2d00fed0714e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=483bcb4dedfc7f46852625a831bfe09532d81344)
▪  STT-MRAM brings non-volatility with high endurance ▪  Unlocking the full SCM potential for SSDs ▪  STT-MRAM enables Hybrid SSD architectures

[5] C. Zambelli et al.,  Proc. IEEE , 105(9), 1790 (2017) DOI. 10.1109/JPROC.2017.2710217

## Retention of STT-MRAM 

![S   4%Switched@60min   4kbitafterbaking   Y]  D   △=56@85°CfprSCM  6   9%Switched@10min   =51@150°CforAutomotive  SO   9=51@85°CforConsumer  35%Switched@5min  53% Switched@2min   38@260°Cfor\$oldering  87%Switched@2min   =36@85°Cfor  97%Switched@2min   ForCacheApplication  10ns   mn  0  140   300   180   20K0   220   240   260   10101010°1010101010  IDO  BakingTemperature[°C]   Retention Time[s]  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4bc29fb7-9ea5-423c-aa76-20f21cb5d7b2/4bc29fb7-9ea5-423c-aa76-20f21cb5d7b2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=378595a9e80bb85dd45f216cce7305a2d241b885)
▪  In STT-MRAM the information may get corrupted

▪  By an unintended switch in the magnetization due to thermal fluctuations

▪

Different thermal stability factors required

▪  Depending on the application target

[68] L. Tillie et al.,  IEEE IEDM  (2016) DOI. 10.1109/IEDM.2016.7838492

## Retention modeling of STT-MRAM 

▪  At a temperature  T , the characteristic thermallyactivated switching time is given by:

$$\tau=\tau_{0}\cdot e x p\left(\frac{\Delta E}{k_{B}T}\right)$$
▪  For  N  bits, the probability of not experiencing any  switching event after a time  t  is:

$$P_{n o s w i t c h}^{N}(t)\propto e x p(-N t/\tau)$$
▪  The probability of having experienced at least one  switching event after a time  t :

$$F(t)=1-e x p(-N t/\tau)=1-e x p\left[\frac{-N t}{\tau_{0}}e x p\left(-\frac{\Delta E}{k_{B}T}\right)\right]$$
![10-2  1bit   32Mbit   1Gbit  1FIT  10-4  △=49  10-6  10-8  10-10  30   5060   O   80   90  AE/KBT  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/00d04a4a-54e4-4060-bfff-0c36ec5f683d/00d04a4a-54e4-4060-bfff-0c36ec5f683d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=15341481f776400658a5dbbe2f7853c125c89a26)
[5] C. Zambelli et al.,  Proc. IEEE , 105(9), 1790 (2017) DOI. 10.1109/JPROC.2017.2710217

## External field-induced magnetic coupling 

![(y) ( o da e   HField[0e]  25°℃   2864e+002  80  -55℃   Topshield   8.5729e+002  1E-3  105℃   .1457  1E-4   Poxy  125℃   1E-5   7186e  1ppm  150℃   1E-6  1E-7  1E-8  1min  1E-9  1-10   -0-20 mins   a  1E-11   10years  出1E-12  40  1000   2000   3000   500 1000 150020002500300035004000  100%  (a)   Hext (Oe)   （b）   Hext (Oe)   (oo)  909  ▪  External magnetic fields on STT-MRAM  External magnetic fields on STT-MRAM  80%   O-BGA package  -QFPpackage   STT-MRAM width axis (nm)  700  · Can affect effective energy barrier  ▪  Can affect effective energy barrier   609  500   1000  15002000  b）   The thickness of shield (nm)   （C)   STT-MRAM  ▪  Both in the standby and active modes  Both in the standby and active modes ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2ffcd85a-8b24-4932-8819-735c56f07704/2ffcd85a-8b24-4932-8819-735c56f07704.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=67cd249d196c9a46a023a0e10b9bb1d829673d7f)
▪  Magnetic shields required to enhance immunity

[69] G. Zhang et al.,  AIP Adv. , 13, 025232 (2023) DOI. 10.1063/9.0000521 (CC-BY 4.0)

## What about MLC in STT-MRAM? 

![mpu  mnal  C3:F.  红工工   input   32×32  IBe   Free layer  Tunneling barl  →Reference laye  conw  Mode Controller (logic/full-add)  write logic “1” write logic “0”   Binaryinp   Binary weights  ST  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ec6b2352-6f35-4381-8028-b1e404b15dc8/ec6b2352-6f35-4381-8028-b1e404b15dc8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215830%3B1743219430&q-key-time=1743215830%3B1743219430&q-header-list=host&q-url-param-list=&q-signature=34058adcb4d870cd2ba7b8882aaa7ee68530e8bf)
▪

Increasing MTJ tunnel magneto-resistance(TMR) ratio

▪

Inspires the development of multi-level cell (MLC)

▪

Two types of multi-level STT-RAM cells

▪

Parallel MLC and series MLC

||        STTMRAM                SCM/                DRAM      |        MRAM                embedded      |        SOH                Cache      |        PCMstand                alone      |        PCM                embedded      |        RRAM stand                alone      |        RRAM                embedded      |
|---|---|---|---|---|---|---|---|
||>1Gb|10-100Mb|>1Nb|Gb|10-100Mb|        Gb                targetted      |1-10Mb|
|        Capacity                Scalability      |Medium|Medium|Poor|Good|Good|Medium|Good|
|DLC||？0||||||
|        3D                integration      ||||Possible|Possible|        Possible in                theony      |        Possible in                theory      |
||xbar|20||Yes|Yes|Yes|Yes|
|        Architecture                Retention      |110°C|xbar|        3terminals                85-100°C      |xbar|1T1R|Xbar|1T1R|
|||        Automotive                150°C10ys      ||85-100°C|Automotive|10ys 85°C|10ys>85°C|
|Latency|10ns|10ns|              |100ns|100ns|100ns|100ns|
|Power|        pJ/bit                1010      |pj/bit|f/bit|10pj/bit|        10pj/bit                >200μA      |1-10pj/bit|        1-10pj/bit                ~100PA      |
|Endurance||>106|>1010|10|106|HOV|106|
|Variability|                DRAM1      |                NW1      |                Cache      |Issue (drift)|Issue (drift)|        Ilssue                (variability,                noise)      |        Issue                (variability,                noise)      |
|        Space                Maturity,                exampleof                products      |||No product|        SC                (storage,                memory)                Products:                Intel/                Micron,                Intel      |MPU, MCU|        SCII                (storage,                memory)      |        MPU,MCU                Products:                Panasonic,                Dialog.                TSIMC      |
||        Products:                Everspin,                Avalanche                (persistent                SRAIM)      |        Product:                Avalanche,                TSMC                (offers STT-                MRAM)      |||        Product                sampling:ST                Microelectr                onics      |No product||


[4] G. Molas et al.,  App. Sciences , 11, 11254 (2021) DOI. 10.3390/app112311254 (CC-BY 4.0)

## Conclusion 

▪  Emerging memories represent a disruption opportunity ▪  The memory hierarchy in computer architectures can change   ▪  PCM, RRAM, and MRAM enable a set of new applications   ▪  Different technologies raise peculiar reliability threats  ▪  Linked to their unique operating characteristics   ▪  Understanding the major limitations allow designing  ▪  Efficient device- and system-level mitigation techniques ▪  To further improve the application quality of service

▪  …

