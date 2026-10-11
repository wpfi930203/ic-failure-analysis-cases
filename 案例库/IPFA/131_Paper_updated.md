---
title: "131_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_c70d98771643abfe29f3a30942bbe5cd7295230462135641
file_size: 1952801
---

## Nano-probing Technique for   Flip-Flop Circuit with Diffusion Defect   

Lai-Seng Yeoh 1 , Kok-Cheng Chong 1 , Susan Li 2   1   Infineon Technologies Memory Solutions Malaysia Sdn. Bhd.                                   Phase 2, Bayan Lepas Free Industrial Zone, 11900 Penang, Malaysia.    2   Infineon Technologies Inc., 198 Champion Court, San Jose, California, 95134 USA.  Phone: (604)8882201, Email:  LaiSeng.Yeoh@infineon.com

Abstract —Electron Beam Absorbed Current (EBAC) is an  omnipresent technique in nano-probing field commonly utilized  for local electrical fault isolation at die level. It complements the  conventional global electrical fault isolation techniques of  photon and thermal emission analyses as well as OBIRCH  (Optical Beam Induced Resistance Change) analysis. In this  paper, we develop an inclusive procedure for analyzing flip-flop  circuits in memory devices impaired with read functional  failures, which has not been reported in any other literature. We  also elaborate on deep-dive physical analysis at the isolated  defective sites   to reveal subtle Silicon diffusion defects which  have caused the read failures.

Keywords—Nano-probing, EBAC, flip-flop, diffusion defect

## I. I NTRODUCTION 

Flip-flop is the basic building block of most sequential  circuits, which are constructed from various electronic  components such as logic gates, transistors, integrated  circuits (ICs), and programmable logic devices (PLDs).  Having the capability of “flipping” or “flopping” between  two stable states (usually   $"0"$  and “1”), a flip-flop is able to  store and recall a single bit (binary digit) of information. A  clock signal triggers an event by latching and changing a  value, assisting the flip-flop to store data over time. Flip-flop  is also the fundamental of digital memory. Memory which  uses capacitor is called Dynamic Random-Access Memory  (DRAM), while memory which engages flip-flip is known as  Static Random-Access Memory (SRAM). The most basic  type is SR (set/reset) flip-flop (Fig. 1 and Fig. 2). It possesses  a bistable multivibrator that can store state information. Flipflop has one or more control inputs where signals are applied.  The processed signals will be exported to its outputs with  change of states. The output of a gate can also drive the input  of other gate, thus forming a feedback loop. This is the  fundamental concept of storage in sequential logic circuits.  Flip-flop is widely used in communication and computing  systems. Besides storing state information, flip-flop also  takes part in clock synchronization, digital counting, and  logic control. Flip-flop has advantages of bistability, precise  synchronous operation and excellent state retention.  Nevertheless, it does have some disadvantages like  complexity, propagation delay and power consumption [1-4].

![CLK  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7e4566a0-8564-4f32-a100-54e0b36a5934/7e4566a0-8564-4f32-a100-54e0b36a5934.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=9644dc65a1cc15d9f0d6dc10ddc7f14363a91fc9)
Fig. 1.   Schematic diagram of SR flip-flop.

Fig. 2.   Truth table of S-R flip-flop.

|CUK|||||
|---|---|---|---|---|
||||Memorystate|Memorystate|
||||Memorystate|Memorystate|
||||||
||||||
||||Invalidstate|Invalidstate|


In 1965, Gordon Moore postulated a log-linear  relationship between the complexity of device against the  time scale. As the number of transistors in ICs doubles-up  every two years, the transistor dimension miniaturizes  proportionally [5-6]. This poses a greater challenge for failure  analysts in discovering physical defects that exist in submicron or even nano-scale. In this situation, the use of nanoprobing is inevitably vital for high-accuracy local fault  isolation. During nano-probing work, a Scanning Electron  Microscope (SEM) is needed for real-time probing and highresolution navigation, while a parametric analyzer is required  to   enable   electrical   measurement   on   the   device’s  characteristics. Depending on the number of nodes, a  minimum of four tungsten probe needles are necessary for  probing the interconnect or contact of a specific transistor  which consists of gate, drain, source and bulk.

A diversity of nano-probing techniques can be applied to  fault isolate malfunctioned circuit that contains short, leakage  or open failure, including Electron Beam Absorbed Current  (EBAC), Electron Beam Induced Current (EBIC), Electron  Beam Induced Voltage (EBIV), Electron Beam Induced  Resistance Change (EBIRCH), and Resistive Contrast  Imaging (RCI). In olden days without nano-probing system,  we had never success in finding the cause of read failure in  flip-flop circuit. Emission technique and even scan chain  diagnosis were not working for this soft failure. With the  recent development of nano-probing assisted EBAC  operation, we had established an unique procedure to resolve  this prolonged quality issue. EBAC is helpful for electrical  and physical fault isolation at metal level. In order to initiate  the EBAC operation, we irradiated electron beam generated  from the SEM tool onto the area of interest. We probed the  targeted metal line and let electron beam current to be  absorbed by all lines which were in connection to the probing  point. The external amplifier system constructed a current  map in the vicinity of the probing area and displayed it on the  SEM. By interpreting the current map, any defect related to  metal open/short or even the underlying poly/diffusion defect  can be effectively screened out (Fig. 3) [7-11].

![electron  oprobe  ampiener  mnetal  nsutatiar  resistive defect  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f1f689d9-b458-4e5a-8e67-938b01c88cf7/f1f689d9-b458-4e5a-8e67-938b01c88cf7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=9beac30f0eb45c8acfbc667891acb49b93eb1dd6)
Fig. 3.   EBAC operation during nano-probing.

## II.   E XPERIMENTAL  T ECHNIQUES  

International standard failure analysis flow was applied in  two case studies consisting of two memory products with  65nm technology node. A variety of equipment were  involved, including memory tester, optical microscope,  scanning acoustic microscope (SAM), X-ray radiator, acid  decapper, reactive ion etcher, thermal/photon emission  microscopes, polisher-grinder, dual-beam focus ion beam  (DBFIB)   machine,   (scanning)   transmission   electron  microscope (S)TEM, energy dispersive X-ray (EDX), etc. As  for nano-probing work, a Kleindiek PS8 probing tool with  XYZ substage attached to a ZEISS Gemini560 SEM was  engaged. Four pieces of Mesoscope CR20 nm probe needles  were used for probing. On the other hand, electrical  characterization was carried out by a Keithley 4200-SCS(A)  parametric analyzer. EBAC test was conducted at each flipflop by probing its Vcc and Vss metal plates. Vcc was  connected to Kleindiek amplifier while Vss was grounded.  Next, Id-Vd data was collected from every diffusion structure  in respective flip-flop. Drain was swept from 0V to 3V and  the corresponding current was gauged at a compliance of 500   $\upmu\mathrm{A}$  . Gate, source and bulk were grounded.

## III.   R ESULTS AND  D ISCUSSIONS  

## A. Case Study 1   

A customer returned memory device demonstrated a read  failure. The failure mode showed a dependency that the  device only failed when using the read command. It failed  block read (different number of bytes 1, 2, 4, 8, 16, 32) and  linear read with no power down between the tests. When this  read failure occurred, the device tended to read at the wrong  address. The circuit designer performed diagnosis and  suspected four possible faulty flip-flop (FF) circuitries which  could contribute to the read failure (Fig. 4).

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/914862b5-b341-45b3-8220-11e01d8af424/914862b5-b341-45b3-8220-11e01d8af424.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=29d49e79fd6370b79b48a4eaa64af91a4b157f36)
Fig. 4.   Four problematic flip-flop circuitries suspected by designer.

Physical failure analysis was started with package level  analysis. Optical, X-ray and SAM inspection revealed no  package related issue. After decapsulation, no any thermal or  photon emission was produced in the suspected area on the  die. A reactive ion etcher was used to etch-off the passivation  layer. Next, a series of parallel lapping processes were done  to remove metal-5 layer down to metal-1 layer. After that, the  area of interest of the specimen was examined at 1keV in  SEM to make sure that the metal-1 layer was fully exposed to  enable nano-probing. Then, the sample was subjected to  plasma cleaning for about 5 min to acquire clean contact  needed for nano-probing work.

EBAC analysis work was initiated for each suspected flipflop circuitry using two probe tips. One probe was landed on  Vcc and hooked up to the external amplifier, while the other  probe was landed on Vss and connected to ground. A  distinctive leakage spot was detected in the diffusion area of  suspected flip-flops #3 and #4 (Fig. 5).

![Flip-flop #1   Flip-flop#2  VcC  vcc  wss  Flip-flop #3   Flip-flop#4     ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/52c4a9fd-b052-46fb-96f4-bd45f262391b/52c4a9fd-b052-46fb-96f4-bd45f262391b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=fdb43f0b05f32243f6b32e0a3813710d3e23d9aa)
Fig. 5.   EBAC test isolated leakage spot in flip-flops #3 and #4 (9.5kx,  10keV).

The next action was to measure the diffusion  characteristic of the defective flip-flops #3 and #4. This nanoprobing work required 3 probe tips to probe at gate, drain and  source of each transistor to measure its Id-Vd characteristic.  Flip-flop #3 contained four p-type diffusions (PDIFF) and  four n-type diffusions (NDIFF) (Fig. 6). The measurement  result indicated that all PDIFF had normal I-V behavior (Fig.  7), but one out of four NDIFF was shorted (Fig. 8).

![PDIFF  Part of the circ    ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a09a3664-9e21-4655-a2e1-afe826b8829d/a09a3664-9e21-4655-a2e1-afe826b8829d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=869531463690dd83056883f7cca972792a895354)
Fig. 6.   Circuit layout of flip-flop #3 containing four PDIFF and four NDIFF.

![PDIFF1        PDIFF2      PDIFF3      PDIFF4      ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9952ae10-1506-4e33-bf2c-e9a61c8064ef/9952ae10-1506-4e33-bf2c-e9a61c8064ef.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=8529e507a1bad2d37319dd2172c3674d3b370747)
Fig. 7.   Nano-probing result of the four PDIFF in flip-flop #3 – all had normal  Id-Vd curve (13kx, 2keV).

![NDIFF1         NDIFF2      ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e2b5bd71-ad61-4963-9ab1-6e6a762c4cd2/e2b5bd71-ad61-4963-9ab1-6e6a762c4cd2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=2735c5e5881b414518aae3ecfe65e9882b4470af)
![NDIFF3      NDIFF4      ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7f3ef5bd-294b-40f3-8b40-d225758c2b12/7f3ef5bd-294b-40f3-8b40-d225758c2b12.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=7f6a19bf8b7ca3f6aa1d8f774cc6890d954cd255)
Fig. 8.   Nano-probing result of the four NDIFF in flip-flop #3 – NDIFF3 was  shorted in its Id-Vd curve (13kx, 2keV).

Similar nano-probing approach was applied to flip-flop #4  which comprised of two NDIFF and three PDIFF (Fig. 9).  The measurement result showed normal I-V curve at all  PDIFF, while one of the two NDIFF, i.e. NDIFF2 displayed  a hard short (Fig. 10). These electrical measurement results  validated the detected EBAC spots at flip-flops #3 and #4.

In order to understand the failure cause, FIB cross section  was carried out at the EBAC spot on both flip-flops #3 and  #4. FIB results showed a suspicious drain diffusion anomaly  at both sites (Fig. 11 and Fig. 12). STEM analysis was then  performed for better defect characterization. Since these two  anomalous sites were located close to each other, so Lamellar  sample preparation could be done only at one site. Flip-flop  #4 was selected for Lamellar sample preparation to extract a  thin film with thickness of approximately 60nm out from its  EBAC spot. STEM inspection confirmed a ring-like physical  defect buried under the drain diffusion (Fig. 13). EDX line  scanning across the defect proved that its content was Cobaltrich (Fig. 14). It was a sign of Cobalt migration!

![Part of the circuit layout  PDIFF1   PDIFEE  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b466cd68-34b6-49de-89e5-4d71f4b7f5f8/b466cd68-34b6-49de-89e5-4d71f4b7f5f8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=7c916c35a5bb20cd2cc6a3566bebc75904570ded)
Fig. 9.   Circuit layout of flip-flop #4 containing two NDIFF and three PDIFF.

![NDIFF1      ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/75d27c76-7599-43c6-a70b-a7a55e4f9e4a/75d27c76-7599-43c6-a70b-a7a55e4f9e4a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=843e12099fcec024d448968838353decea8fb713)
![NDIFF2      PDIFF      PDIFF2      PDIFF3      ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/65405d07-a589-4adb-8c84-3002c011cabd/65405d07-a589-4adb-8c84-3002c011cabd.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=055c23d0b3e0c181efde5eb3a6f9e0234f3db274)
Fig. 10.   Nano-probing result of the five diffusions – NDIFF2 was shorted  in its Id-Vd curve (13kx, 2keV).

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bae45cd1-edb6-4cf4-9167-44adea0114d1/bae45cd1-edb6-4cf4-9167-44adea0114d1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=04121bb3accfdc1d406c143ebb4e60a20ffb87e3)
Fig. 11.   FIB cut detected a suspicious anomaly in NDIFF3 of flop-flop #3  (200kx, 10keV).

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c12f2a28-c783-4fa8-9ae9-80beb4bc8c79/c12f2a28-c783-4fa8-9ae9-80beb4bc8c79.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=418bad73b270422bd1efc308d3729f3fdd3f914a)
Fig. 12.   FIB cut detected a suspicious anomaly in NDIFF2 of flop-flop #4  (250kx, 10keV).

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/db58fb9a-894f-47bb-b208-805572413a16/db58fb9a-894f-47bb-b208-805572413a16.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=f9e0ee080ebc9756d86054e8ac2a69a8f75055b1)
Fig. 13.   STEM image confirmed a ring-like diffusion defect in NDIFF2 of  flop-flop #4 (500kx, 30keV).

![Cobalt diffusion  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b5970654-815d-4fde-8a91-b7b3eeb59be5/b5970654-815d-4fde-8a91-b7b3eeb59be5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=557c4f58ce1dd95483a6033ae29777d6cca2596a)
Fig. 14.   EDX line scan gave an indication of Cobalt diffusion at the defect  site.

## B. Case Study 2   

A memory device failed at our customer board assembly  line. The customer claimed that the device showed abnormal  data content at  $-35~^{\circ}\mathrm{C}$  . Our full electrical test indicated that it  suffered from read failure at left bank, sectors 6&7, IO 3&4.  Circuit designer diagnosed the device and suspected a  potential defective flip-flop circuit (Fig. 15).

![Partofthecircuit layoutviewismaskedout  forintellectualpropertyprotection  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/cbff3a8c-59a0-4be1-877c-9c332aacf505/cbff3a8c-59a0-4be1-877c-9c332aacf505.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=5358701c0628181ebb67e1f80b93399989b180cc)
Fig. 15.   Circuit layout of the problematic flip-flop suspected by designer.

Package level analysis comprising of optical, X-ray and  SAM inspection showed no package anomaly. Die surface  inspection upon decapsulation revealed no sign of physical  damage at the failing sectors 6 and 7. Both photon and  thermal emission analyses did not manage to generate  emission signal related to the read failure. The passivation  structure of the die was removed in reactive ion etching.  Then, the die was subjected to planar polishing to lap-off  metal-5 down to metal-1 in order to expose the area of interest  pinpointed by circuit designer. It was plasma-cleaned about 5  min.

The affected flip-flop circuit contained six pairs of PMOS  and NMOS transistors. Nano-probing was carried out using 3  probes to land on gate, drain and source of each transistor to  check its Id-Vd behavior. The measurement result showed  that the first transistor pair (PMOS1 and NMOS1) was  electrically shorted (Fig. 16 and Fig. 17).

![PMOS1      PMOS2      PMOS3      PMOS4       PMOS5      ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/672458b0-9d51-4eac-a8fd-4f4e333831d2/672458b0-9d51-4eac-a8fd-4f4e333831d2.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=9a6416b1dae57438ff447fb33de7824924daa665)
![AE  PMOS6      ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0fbdd190-9a82-4d38-92b5-2f3e4c7ac381/0fbdd190-9a82-4d38-92b5-2f3e4c7ac381.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=591b45386b787dd7a5144f6995131db8a125998a)
Fig. 16.  Nano-probing result of the six PMOS transistors – PMOS1 was  shorted in its Id-Vd curve (13kx, 2keV).

![S  NMOS1      NMOS2      NMOS3      NMOS4      NMOS5      ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2ca672ef-cce9-4a71-a0dd-f64588fd4dd8/2ca672ef-cce9-4a71-a0dd-f64588fd4dd8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=cb51363af40174cc810364d60d611c8cc62a70d1)
![NMOS6      ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/3cd82361-7b59-4415-b1c5-0c8985205c34/3cd82361-7b59-4415-b1c5-0c8985205c34.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=f57ad5e13909648fca88cff42bc4f65c2614d1c1)
Fig. 17.   Nano-probing result of the six NMOS transistors – NMOS1 was  shorted in its Id-Vd curve (13kx, 2keV).

Next, EBAC fault isolation analysis was conducted to  determine if PMOS1 or NMOS1 was defective. The EBAC  approach applied in case study 1 was attempted but  unsuccessful to detect any spot. Therefore, an alternative  method was engaged by landing a probe tip on the drain of  NMOS1 and hooking it up to the external amplifier. The gate  and source of NMOS1 were also probed and were grounded.  At the moment the amplifier was turned-on, excessive EBAC  signal was observed at NMOS1. This implied an occurrence  of unusual electron-hole pairs activity in the diffusion region  of NMOS1. In contrast, EBAC signal at PMOS1 appeared to  be normal (Fig. 18).

![NMOS1  PMOS1  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d44a6fd3-ac92-4863-ad14-829387d11c41/d44a6fd3-ac92-4863-ad14-829387d11c41.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=83bbc1a12c2e7e128ab9d5cbd35d59a1a5cbd87d)
Fig. 18.   EBAC test at NMOS1 transistor detected over-clouding of signal  at NMOS1 (13kx, 10keV).

No any anomality was sighted under high-kV SEM  inspection at the EBAC site of NMOS1. Since the EBAC  signal spread over a wide area, sequential FIB cross section  was carried out starting from the edge of circuitry and  gradually moved into the inner part of the diffusion to look  for signs of abnormal transition. Eventually, a suspicious  anomaly was discovered at the hillside of the diffusion  adjacent to a drain contact (Fig. 19). For better illustration, a  50nm-thick Lamellar thin film was lifted off from the  defective area. High-resolution of STEM and TEM imaging  proved that it was an etch block defect (Fig. 20 & Fig. 21).  EDX mapping verified that the defect composition was rich  in silicon (Fig. 22).

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7621e206-0096-4135-a9ce-92a5b7f0cb35/7621e206-0096-4135-a9ce-92a5b7f0cb35.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=9583834db4836223ba3b071dad30c2d7ce2c5aea)
Fig. 19.   FIB cut showed a suspicious diffusion anomaly in NMOS1 (100kx,  10keV).

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1f61f05b-e475-490b-98e1-4ee79a130a26/1f61f05b-e475-490b-98e1-4ee79a130a26.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=016c8e5c297d07d7528d2ebdafac8127812e6862)
Fig. 20.   STEM imaging confirmed presence of an etch block defect in  NMOS1 (200kx, 30keV).

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e8ce32cf-6cb5-4aa3-9154-06f82162c0c6/e8ce32cf-6cb5-4aa3-9154-06f82162c0c6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=b3df399b87a79bdcc5b5468abd3a762229de58f0)
Fig. 21.   TEM imaging confirmed presence of an etch block defect in  NMOS1 (200kx, 300keV).

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/54834dcd-5c20-484b-a232-e15d5f8ba6ca/54834dcd-5c20-484b-a232-e15d5f8ba6ca.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215843%3B1743219443&q-key-time=1743215843%3B1743219443&q-header-list=host&q-url-param-list=&q-signature=8e21ee2b7f0f993a2426a957657ed6298354054e)
Fig. 22.   EDX mapping indicated that the etch block defect composition  was Silicon-riched: yellow – Si, blue – O, green – N, red – Co.

## IV.   C ONCLUSION  

Our team founded an effective and efficient nano-probing  method for successful fault isolation of read failure involving  several flip-flop circuitries in two types of memory product.  Further physical failure analysis precisely discovered  miniscule diffusion defects that were detrimental to the  catastrophic read failure. These fascinating findings not only  enabled the fab foundry to implement apt corrective action to  streamline the semiconductor process and remedy the quality  issue, but also established an useful guideline for future work  using a similar methodology demonstrated in this paper to  enhance the failure analysis success rate.

## A CKNOWLEDGMENT 

We would like to acknowledge DE, EFA and PFA teams  from Infineon Technologies for their contribution to the  success of this technical paper. Special thanks to Infineon  Material Characterization Lab particularly Max Sidorov for  his engineering aid on TEM work. Appreciation is also  dedicated to MC Lim and Jens Haertel on their endless  motivating management support.

## R EFERENCES 

[1]    Adel S. Sedra and Kenneth C. Smith, “Microelectronic Circuits,”  Oxford University Press Inc.,  $5^{\mathrm{th}}$   Ed. 2004.     [2]    Jan M. Rabaey, Anantha Chandrakasan and Borivoje Nikolic, “Digital  Integrated Circuits - A Design Perspective,” Prentice Hall Inc.,   $2^{\mathrm{nd}}$   Ed.  2003.      [3]    John F. Wakerly, “Digital Design, Principles & Pratices,” Prentice Hall  Inc. 3 rd  Ed. 2002.     [4]    “Flip Flop Basics – Types, Truth Table, Circuit, and Applications,”  Electronicsforu.com, 2023.     [5]    Gordon E. Moore, “Cramming More Components onto Integrated  Circuits,” Electronics, Volume 38, Number 8, April 19, 1965.    [6]    Bob Schaller, “The Origin, Nature, and Implications of Moore’s Law,”  Microsoft, 1996.    [7]    S. Kleindiek and A. Rummel, “Nano-probing (Failure Analysis),”  Technical Notes, Kleindiek Nanotechnik.    [8]    P. K. Tan, M. K. Dawood, G. R. Low, H. H. Yap, R. He, et al.,  “Nanoprobing EBAC Technique to Reveal the Failure Root Cause of  Gate Oxide Reliability Issues of an IC Process,” IEEE International  Integrated Reliability Workshop 2014.    [9]    S. Wei, S. H. Lim, M. Zulkifli, Syahirah, and D. Khatri, “Optimization  and Application of Electron Beam Absorbed Current Technique,”  IPFA2015.    [10]   S. Kleindiek, K. Schock, A. Rummel, M. Zschornack, P. Limbecker, A.  Meyer, and M. Kemmler, "Combining Current Imaging, EBIC/EBAC,  and Electrical Probing for fast and reliable in situ Electrical Fault  Isolation," IEEE   $23^{\mathrm{rd}}$   International Symposium on the Physical and  Failure Analysis of Integrated Circuits (IPFA), 2016.    [11]   L.S. Yeoh, K.C. Chong, and Susan Li, “Novel Nano-probing Technique  for Column Short Failure in Flash Memory Devices,” IEEE   $30^{\mathrm{{th}}}$    International Symposium on the Physical and Failure Analysis of  Integrated Circuits (IPFA), 2023.

