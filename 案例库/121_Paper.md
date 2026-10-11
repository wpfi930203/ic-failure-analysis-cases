---
title: "121_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_f1ed785e39cb2c113abde5dbb38dac2e7295230462135641
file_size: 737846
---

## Cycle-Shift Scan Chain Failure Analysis Using Single Pulse Test Pattern  

Paulraj Eric\*, Chwee-Lin Choong, Yiang Won Chai

Intel Technology Sdn. Bhd., Bayan Lepas Free Industrial Zone, 11900 Penang, Malaysia  Phone: +60 42539516 \*Email:eric.paulraj@intel.com

## Abstract 

Conventional scan chain test pattern of “0011” repeating data is widely used to tackle scan chain failures such as stuck-at and  transition failures using Laser Voltage Imaging’s (LVI) fundamental and second harmonic frequency approaches.  However, this  “0011” scan chain test pattern when combined with LVI technique is ineffective in isolating cycle-shift scan chain failures even  with the integration of a lock-in amplifier which is also known as phase LVI. This is because phase LVI isolation technique  requires detailed understanding of the scan chain design and fault isolation for all types of cycle-shift scan chain failing signatures  is not possible using this technique. In this paper, we propose a technique to effectively isolate the failing flop for an entire range  of cycle-shift scan chain failures using a novel single pulse chain test pattern paired with Laser Voltage Probing (LVP) that  overcomes the challenges faced by phase LVI.

## Introduction  

Scan chain fault isolation is a process of identifying one or  more defective scan cells in a design-for-test (DFT) scan chain  [1]. Among the most commonly used chain test patterns, all-0s  and all-1s test patterns are restricted to detecting stuck-at-1 and  stuck-at-0 scan chain failures, respectively. On the other hand,  chain tests that consist of repetitive “0011” pattern has been  proven robust for detecting stuck-at failures, and all types of  transition failures including slow-to-fall, slow-to-rise, fast-tofall and fast-to-rise [2]-[4].

For stuck-at or transition scan chain failures, binary search  through the scan chain using LVI with fundamental or second  harmonic frequency can effectively isolate the failing scan cell  using a  $"0011"$   test pattern [4]. The LVI tool utilizes a spectrum  analyzer with tunable central frequency to filter signals with a  specific narrow band frequency. This results in an image of the  circuit activity at the specified frequency whereas transistors  switching at other frequencies (e.g. faulty transistors) will not  be detected and mapped [5].

However, the LVI method for cycle-shift failures is not  effective, as the failing scan cell holds the same “0011” shiftout data as a healthy scan cell. Cycle-shift failures may occur  due to manufacturing defects (e.g. bridging) or timing  violations (e.g. clock skew, long traces). The entire range of  cycle-shift scan chain failing signatures is as shown below:

Expected:    “11001100”    Fail Data:   “01100110” or               “00110011” or          “10011001” or          “11001100” (Note: Shifted by 4 cycles)

Conventional debug method for cycle-shift failure is by  isolating the failing scan cell using sequential LVP waveform  acquisition starting from the first scan cell until the failing scan  cell is identified. DCG Systems [6] has applied the “0011” test  pattern for this method of isolation. Their approach is time  consuming as LVP waveform acquisition needs to be  performed on each and every scan cell along the scan chain  until a mismatch of data shift cycle is observed on a particular  scan cell.

Phase LVI has been introduced to debug cycle-shift failures  more effectively by analyzing the relative phases between scan  cells using a high-speed digitized lock-in amplifier or a vector  analyzer [7]. However, phase LVI has not been well accepted  because: (1) phase LVI analysis can get complicated when  there are inverters, buffers and lock-up latches between scan  cells, which will change the relative phase delay between the  cells, (2) of the inability to debug cycle-shift failures with a  phase delay of  $360^{\circ}$   such as the aforementioned 4 cycles shifted  fail data, and (3) it requires the tester to drive a stable clock  signal to the LVI tool, which is vulnerable to jitter [7].

In this paper, we demonstrate that LVP isolation using a  single pulse chain test pattern proves to be an effective method  to debug cycle-shift scan chain failures.

## Single Pulse Chain Test Pattern  

Single pulse pattern, as in the conventional “0011” pattern,  is an Embedded Deterministic Test (EDT) bypass pattern. This  allows predictable data to be shifted onto the cycle-shift faulty  scan chain, bypassing the EDT decompressor.

The length of the proposed single pulse test pattern is based  on the length of the failing scan chain  $(n)$  , which is the number  of scan cells on the failing chain. A single pulse test pattern can  be constructed from one data cycle of '1' and the remaining data  cycles of   $\mathbf{\epsilon}_{0},$   or vice versa. When one data cycle of   $^\bullet1^{\bullet}$   is  employed, the length of data  $"0"$   can be derived from Eq. (1).

$$L e n g t h\:o f\:d a t a\:\mathrm{{'0'}}\:=\:n\textrm{-}1$$
This equation is to ensure that a single pulse is observed  throughout the entire length of the failing scan chain during  LVP acquisition.

## LVP with Single Pulse Test Pattern  

The LVP tool acquires waveforms from active transistors  directly based on principles of the Franz-Keldysh effect. The  photon detection is based on the change of logic state in  transistors that modulates the reflected laser beam from the  transistors’ space-charge region. A photodetector is used to  convert the optical signal to electrical signal, which then gets  amplified. In the end, an oscilloscope is employed to

reconstruct the original transitions from the transistors [8].

While performing LVP waveform acquisition with the  single pulse pattern, we are able to observe the single pulse  being shifted following the sequence of scan cells on the chain  as seen in Fig. 1. The scan cell numbering convention here is  in reverse order wherein the first scan cell is scan cell   $(n-1)$    and the last scan cell is scan cell 0.

![Scan Clock  Scan Cell (n-1)  Scan Cell (n - 2)  Scan Cell (n - 3)  Scan Cell (n - 4)     ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/29ebaeb9-37c5-43b2-9af1-f9218022959d/29ebaeb9-37c5-43b2-9af1-f9218022959d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215625%3B1743219225&q-key-time=1743215625%3B1743219225&q-header-list=host&q-url-param-list=&q-signature=0ce4ad14ed7498dbd70bd8cbcfb4b541a83d12c1)
Fig. 1 Shift sequence of single pulse data on a scan chain.

Based on this algorithm, the single pulse data cycle of the  probed scan cell can be anticipated. This will allow us to  perform binary search or sampling LVP on selective scan cells  instead of performing sequential LVP [5] or phase LVI [6].

As illustrated in Fig 2, for a failing scan chain that has a  total of 20 scan cells ( ݊ ), isolation can be done using a single  pulse chain test pattern with a data length of 20 (e.g.: “1000  0000 0000 0000 0000” or “0111 1111 1111 1111 1111”), as  derived from Eq. (1).

Binary Search Method : Firstly, probe the first scan cell (e.g.  scan cell 19) to determine the single pulse data cycle (e.g. at  clock cycle 1), then divide the chain length by two to get the  next cell (e.g. scan cell 10) that needs to be probed. This  determines whether the failing cell is located within the first  half or second half of the chain. For the given example, the  failure is located within the second half (e.g. scan cell 10 to 0)  of the chain. Then, continue binary search from scan cell 10 to  0 (e.g. scan cell 5 then 3) to isolate the failing cell (e.g. scan  cell 4) as shown in Fig. 2(a), where the expected single pulse  data was observed at clock cycle 6 instead of 16.

![Clock Cycle  1234567891011121314151617181920  Scan Cell19  ScanCell10  ScanCell5  ScanCell3  ScanCell4   Probed Passin  Probed Failn  Expected Pssing  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ff94c699-4ca3-4e5d-80f3-c92bb69bb04c/ff94c699-4ca3-4e5d-80f3-c92bb69bb04c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215625%3B1743219225&q-key-time=1743215625%3B1743219225&q-header-list=host&q-url-param-list=&q-signature=7ebf1e57a2895ad19455344cba725cd3e894269f)
Fig. 2(a) LVP waveform acquisition using Binary Search Method on  single pulse test pattern.

Sampling Method : Firstly, probe the first scan cell (e.g. scan  cell 19) to determine the single pulse data cycle, then probe on  every 5 or more scan cells sequentially, depending on the scan  chain length. For this given example, sampling of every 5 scan  cells is used (e.g. scan cell 15, 10, 5 and 0). If the pulse does  not occur at the expected scan clock cycle (e.g. scan cell 0),

move backwards to determine which scan cell has the wrong  pulse data (e.g. scan cell 4) as illustrated in Fig 2(b).

When a single pulse chain test pattern is applied, the  number of LVP waveform acquired can be significantly  reduced because sampling and binary search methods can be  used to search through the cycle-shift faulty scan chain to  isolate the failing scan cell. As demonstrated in the example  shown, binary search method requires 5 times of LVP  waveform acquisition while sampling method requires 6. It  should be noted that both binary search and sampling methods  are equally efficient to isolate cycle-shift failing scan cell,  hence readers can opt for either method based on their own  preference for fault isolation.

![ClockCycle  1234567891011121314151617181920  Scan Cell19  Scan Cell 15  Scan Cell 10  Scan Cell5  Scan Cello  ScanCell4   Probed Passing " Probed Failing  Expected Passing  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/38ab9aea-e0b9-48e9-9310-20e424c75481/38ab9aea-e0b9-48e9-9310-20e424c75481.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215625%3B1743219225&q-key-time=1743215625%3B1743219225&q-header-list=host&q-url-param-list=&q-signature=79adfac2b5e35a3c0ef8ab64eb0f7457f5c21aff)
Fig. 2(b) LVP waveform acquisition using Sampling Method on  single pulse test pattern.

## Scan Chain Debug on Cycle-Shift Failure  

The flow diagram in Fig. 3 outlines three types of scan  chain failures: (1) stuck-at, (2) transition and (3) cycle-shift  together with their corresponding fault isolation methods.  Nevertheless, this work focuses solely on cycle-shift scan  chain failure. The flow highlighted in blue is a novel fault  isolation technique proposed in this work to isolate a cycleshift failing scan cell. We demonstrate using a case study how  such failures can be root-caused using this fault isolation flow,  starting from Operation 3(a) to 3(h).

![3（a)  Scan ChainFailure  3（D)  RunSoftwareBasedDiagosistsolatFainghan&  3（C)  Use0011DataPatternPerformLVI/LVPonFailingChainOutput  VerifytheFailureType  3（d)  LVI:NoDataModulation   LVP/LVI   LVI:WithDataModulation  LVP:0000/1111   Result   LVP:0011/1100  LVI:WithDataModulation  LVP:1000/1110  3(e)  Stuck-atFailure   TransitionFailure   Cycle-Shiftfailure  3（f）  Change Shift in Data  RemainShift in Data   RemainShift inData  Pattern toSingle pulse  Pattern0011   Pattern0011  Pattern  3（9)  LVIBinarySearchUsing   LVI BinarysearchUsing   LVPUsingBinary Search  orSamplingMethod  Frequency   Frequency  3（h)  FailingScan Cell Isolated  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1bb6f20c-f45f-46fa-9625-b0680037f678/1bb6f20c-f45f-46fa-9625-b0680037f678.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215625%3B1743219225&q-key-time=1743215625%3B1743219225&q-header-list=host&q-url-param-list=&q-signature=9a7f34f6b69d011256a244e46f4c84f49593e90c)
Fig. 3 Scan chain fault isolation methods and flows.

## Case Study  

This case study focuses on a scan chain failure (Operation  3(a)) that was reported from High Volume Manufacturing  (HVM) test flow. In reference to software-based scan chain  diagnosis, scan chain 15 was reported failing, but the fault type  was “Indeterminate” (Operation 3(b)). The reported failing  chain has a total of 138 scan cells. At Operation 3(c), LVP and  LVI experiments were carried out using a  $"0011"$   test pattern  to determine the failure type. However, both LVP and LVI  experiments could not isolate the faulty scan cell as a healthy  looking data similar to the shifted in “0011” pattern was  observed on the last cell of the failing chain as shown in Fig. 4  (Operation 3(d)). In this instance, both stuck-at and transition  failures can be ruled out, thus it can be concluded that the  failure type is a cycle-shift failure (Operation 3(e)).

![  ScanCellO  Clock   Chain18  ScanCello   ScanCello  Chain15   Chain15  0.020.040.060.080.100.120.14>t(us)    (a)   Cb  (b)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b0cace4d-712b-4302-bf97-9e64318b4838/b0cace4d-712b-4302-bf97-9e64318b4838.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215625%3B1743219225&q-key-time=1743215625%3B1743219225&q-header-list=host&q-url-param-list=&q-signature=7c7adce461b4a9767ca1f123a6d5906f17c13b03)
Fig. 4 (a) LVP on output node of cell 0 of chain 15, and (b) First  harmonic data (12.5 MHz) LVI image on cell 0 of chain 15 showing a  healthy data modulation when compared to healthy scan cell 0 of  chain 18.

At Operation 3(f), a single pulse test pattern was  constructed (single pulse out of 138 shift data cycles) as  derived from Eq. (1) where the length of the failing scan chain,   $n=138$  . This was followed by Operation 3(g), where LVP  waveform acquisition was carried out for every 10 scan cells  via sampling method to isolate the failing scan cell boundary  within the range of scan cell 110 to scan cell 100. This is  because the single pulse for scan cell 100 was expected to be  observed only after 10 clock cycles from scan cell 110,  however it was observed much earlier at the third clock cycle  as shown in Fig. 5.

![10ClockCycles   Expected10,ClockCycles  Clock  ScanCell137  ScanCell130  ScanCell120  ScanCell110  ScanCell100  >t（us)  0.000.050.10   0.150.20   0.25   D.30   0.350.40  BCloe  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/07ea025c-0acc-4f48-b819-1da259600773/07ea025c-0acc-4f48-b819-1da259600773.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215625%3B1743219225&q-key-time=1743215625%3B1743219225&q-header-list=host&q-url-param-list=&q-signature=1795f14ecd7d34c49d1eaae84b329e0dcf96c35b)
Fig. 5 Failing scan cell boundary isolation using single pulse pattern  with LVP.

As showed in Fig.6, LVP experiment was continued by  acquiring waveform for every scan cell within the isolated

boundary (scan cell 110 to 100) and at last, the failing cell (scan  cell 106) was isolated (Operation 3(h)).

![clock  ScanCell108  ScanCell107  Scan Cell106W  ScanCell105  ScanCell104  ScanCell103  >t（us)  0.100.150.200.250.300.350.400.450.500.550.60  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/57dafdfe-15eb-429f-b3b2-b3ff17589318/57dafdfe-15eb-429f-b3b2-b3ff17589318.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215625%3B1743219225&q-key-time=1743215625%3B1743219225&q-header-list=host&q-url-param-list=&q-signature=0e46e646551e1bf2a933ebfcd755ea361a22d0fd)
Fig. 6 Failing scan cell isolation using single pulse pattern with LVP.

Subsequent   Scanning   Electron   Microscopy   (SEM)  inspection revealed a metal-to-metal short between signal A of  scan cell 106 and signal C of an adjacent device that is located  on a different scan chain path (Fig. 7). Therefore, the rootcause of the failure is due to an electrical “short” defect  between two chain paths.

![signalA   signalc  (Scan Cell 106)   (Neighboring device)  metal-to-metalbridging  3005.0kV   300nm  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d3f12506-eadb-47b2-91b8-6f3312a4b050/d3f12506-eadb-47b2-91b8-6f3312a4b050.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215625%3B1743219225&q-key-time=1743215625%3B1743219225&q-header-list=host&q-url-param-list=&q-signature=65286f49ae36e32d4e70f0b89a2be0893f89caf1)
Fig. 7 SEM image showing a metal-to-metal bridging between Signal  A of scan cell 106 and Signal C of a neighboring device.

## Discussion 

In this case study, sampling method was employed first to  isolate the failing scan cell boundary, followed by sequential  LVP to isolate the defective scan cell. It should be noted that  binary method is equivalently powerful to perform such  isolation. For this case study, sampling method was presented  merely because the authors find that sampling method provides  readers a better view of the progression of the single pulse  along the failing scan chain.

Introduction of single pulse test pattern allows binary  searching or sampling scan cells through the cycle-shift failing  scan chain using LVP. This significantly reduces the number  of LVP waveform acquisition needed to isolate the failing scan  cell. For instance, the presented case study shows that LVP  waveform was acquired 9 times when single pulse test pattern  is used with sampling approach.

In contrast, a conventional “0011” test pattern is ineffective  in isolating cycle-shift failure because: (1) both LVI and LVP  show “healthy” “0011” data; and (2) neither binary search nor

sampling method can be applied when searching through the  cycle-shift failing scan chain using LVP.

When a conventional “0011” test pattern is used [6], 32  times of sequential LVP waveform acquisition is required on  each and every scan cell from the first scan cell (e.g. scan cell  137) up to the defective scan cell (e.g. scan cell 106), which is  more than triple the effort of LVP waveform acquisition  compared to the proposed approach. Note that a more intense  level of LVP waveform acquisition may be required if the  failing scan cell is further away from the first scan cell.

## Conclusion 

In this work, we introduced a novel fault isolation  technique to identify a cycle-shift scan chain failure and isolate  the respective failing scan cell. The scan chain debug involves  shifting a single pulse test pattern onto the failing scan chain  during LVP waveform acquisition to detect the cycle-shift  defective scan cell. We have demonstrated the practicality and  efficiency of the presented isolation technique in root-causing  a fab-induced cycle-shift scan chain failure.

The proposed single pulse chain test pattern is proven to be  much more efficient than the conventional “0011” test pattern  which hinders sampling or binary search through the cycleshift faulty scan chain during LVP waveform acquisition [6].  The proposed isolation approach is also proven superior to the  phase LVI approach [7], as it does not require design  information to determine the expected phase data.

In conclusion, the presented fault isolation approach using  a single pulse chain test pattern for LVP-based isolation is both  simple and efficient in covering the entire range of scan chain  cycle-shift failures caused by either defect or design hold time  issue.

## Acknowledgments 

The authors would like to thank the Intel FAFI Team for  their assistance in FAFI data collection and analysis presented  in this paper.

## References 

[1]    E. Auvray, P. Armagnat, L. Saury, M. Jothi, M. Brügel, “Effective scan  chain failure analysis method,”  Microelectronics Reliability , 76-77,  2017, pp.201-213.    [2]    S.Y. Liu  et al ., "Laser voltage imaging and probing, efficient techniques  for scan chain verification in advanced node,"  2017 IEEE 24th  International Symposium on the Physical and Failure Analysis of  Integrated Circuits (IPFA) , Chengdu, 2017, pp. 1-4.    [3]    A. Oberai, J.S. Yuan, “Efﬁcient Fault Localization and Failure Analysis  Techniques for Improving IC Yield,”  Electronics , 7(3), 2018, p.28.    [4]    S. Kasapi, W. Lo, J. Liao, B. Cory and H. Marks, "Advanced scan chain  failure analysis using laser modulation mapping and continuous wave  probing,"  2012 19th IEEE International Symposium on the Physical  and Failure Analysis of Integrated Circuits , Singapore, 2012, pp. 12- 17.    [5]    J. Y. Liao, S. Kasapi, B. Cory, H. L. Marks, Y. S. Ng, “Scan Chain  Failure Analysis Using Laser Voltage Imaging.”  Microelectronics  Reliability,  50.9, 2010, pp 1422-1426.    [6]    DCG systems “Breakthrough in Electrical Fault Isolation and Yield  Ramp-Up: LVx-Enabled Shift Isolation” Technical Update, September  2012.    [7]    G. Ranganathan, V.K. Ravikumar, S.L. Phoa, C. Nemirow, N. Leslie,  “Debugging Signal Corruption in Scan Chain using Phase Laser  Voltage Imaging,”  Proceedings from the    $\mathcal{4}\mathcal{3}^{r d}$   International Symposium  for Testing and Failure Analysis, ISTFA 2017. , 2017, pp. 171- 175    [8]    V. K. Ravikumar, R. Wampler, M. Y. Ho, J. Christensen, S. L. Phoa,  “Laser voltage probing in failure analysis of advanced integrated  circuits on SOI.”  2012   $I^{g^{t h}}$   IEEE International Symposium on the  Physical and Failure Analysis of Integrated Circuits , Singapore, 2012,  pp 1-4.

