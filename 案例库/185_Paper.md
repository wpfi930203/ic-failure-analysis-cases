---
title: "185_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_a91e579e82a1251e8d4ef6204ccc09447295230462135641
file_size: 3832220
---

## Increased Fault Isolation Efficiency by Using Scan  Cell Visualizer for Scan Chain Failures  

Peter Chua Thin Wei \*1 , Foo Loke Sheng 1 , Ng Kim Choo 1 , Keith A. Serrels 2 , Kuyt   $\mathrm{Ku}^{3}$  , Curt Lin 3 , Tang Chih-yi 3  1 NXP Semiconductor Sdn. Bhd., 2, Jalan SS 8/2, Free Industrial Zone Sungei Way, 47300 Petaling Jaya, Selangor, Malaysia.  2 NXP Semiconductors, 6501 West William Cannon Drive, Austin, TX 78735, USA.  3 NXP Semiconductors, 10, Jing 5th Road, N.E.P.Z., Kaohsiung 81170, Taiwan, R.O.C.  \* Phone: +603-7669-2407   Email: peter.chua@nxp.com

Abstract-   Scan design, being part of the most commonly practiced  form of Design for Testability (DFT) has been developed to enable  software based diagnosis for scan chain failures. Tessent Diagnosis  helps to narrow down the reported failures to a suspected failing  chain [1] - [5].  Unfortunately, scan chains can consist of hundreds  to thousands of individual latches that can represent potential  defect candidates and are typically distributed across the entire  chip. Implementing global fault isolation techniques, which  includes Photon Emission Microscopy (PEM) analysis, can lead to  a collection of numerous anomalous emission spots. Cross  mapping both the PEM results and the hundreds to thousands of  individual scan cells to the CAD layout is both time-consuming  and labor intensive. Moreover, selective cross mapping does not  reveal the scan latches in chronological order, which is important  for any scan chain analysis.  One possible solution is to spatially  map the scan latch list from the diagnosis file to the CAD layout to  visualize the scan latch distribution quickly.  This paper describes  the use of this Scan Cell Visualizer through the use of case studies  to demonstrate improved layout mapping efficiency and reduced  overall failure analysis cycle time.

Keywords  –  Scan Chain, Scan Cell Visualizer, Fault Isolation,  Tessent Diagnosis .

## I. I NTRODUCTION 

Integrated Circuit (IC) design has advanced rapidly in recent  years with increasing complexity and shrinking transistors  geometries, where in all aspects has led to complexities for  Failure Analysis (FA). Scan-based DFT has become the  standard in the semiconductor industry to tackle the increase in  advanced technologies. Scan-based DFT is designed to enable  software based diagnosis to assist in localizing and therefore  narrowing down the suspected failure. [1] - [5]

Scan cells in scan chains have been increasing with the  advance in technology to improve fault coverage; therefore,  scan chains often consist of hundreds to thousands of scan cells.  Tessent Diagnosis comes into play in narrowing down the  suspected failing node, but at times it does not provide good  diagnosis results [1] - [5]. As a result, implementing global fault  isolation techniques, such as PEM analysis, can help to isolate  the suspected failing sites. When no anomalous spots are  identified however, a binary search of the individual scan cells  is required to narrow down the suspected failing sites [6]. In  order to perform this binary search, one must first start by  mapping hundreds to thousands of scan cells manually across  the layout. This step is very time consuming and labor  intensive.

To address this limitation, a Scan Cell Visualizer script from  Synopsys was employed to map all the scan cells within the  scan chain in chronological order. This provides a rapid spatial  overview of all the scan cells located across the die within a  specific chain. By generating this scan cell map, an analyst can  easily identify the area to focus on with increased accuracy, as  compared to the laborious task of manual mapping. As a result,  by having access to both the spatial distribution and the  sequential latch order of a suspect scan chain, the process of  performing a binary search is significantly reduced. [7]

In addition to the spatial distribution and sequential latch  order, each scan cell map is detailed with path name. Thus  increase the efficiency in identifying the modules during  analysis.

All case studies presented herein were extracted from FA  performed on test vehicles for yield learning.

## II.   C ASE  S TUDY AND  D ISCUSSION  I  

Device 1 was failing a stuck-at scan chain pattern. Tessent  Diagnosis identified the failure to occur within 2 chains,  chain117  and  chain118 . These 2 chains have hundreds of scan  cells each, where  chain117  consists of 312 scan cells and  chain118  consists of 317 scan cells. Using the Scan Cell  Visualizer, these scan cells were mapped to the CAD layout and  are shown in Fig.1 and Fig. 2.

![Chain117  Scancells  Scan cells  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e5ed703a-0c87-4f3a-aef7-e92e78f7b700/e5ed703a-0c87-4f3a-aef7-e92e78f7b700.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=37a65bac02699584d9bb1e7995cfc741e23335c3)
Fig. 1 - Scan Cell Visualization of  Chain117  (highlighted in white).

![Chain 118  Scan cells  Scancells  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d38cf4ca-f1bd-4909-91a0-2ec93c08c0d0/d38cf4ca-f1bd-4909-91a0-2ec93c08c0d0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=bdecfc9b43f68ee23e76ecc9584329951fa9a219)
Fig. 2 - Scan Cell Visualization of  Chain118  (highlighted in yellow).

By utilizing the Scan Cell Visualizer in Fig. 1 and Fig. 2, it  was easily identified that the scan cells are not contained in one  area but instead occupy 2 different areas for each chain.  Therefore, when performing global fault isolation, the prime  focus will naturally be these 2 specific areas.

Backside PEM analysis was performed and 2 anomalous  emission spots were observed while looping the stuck-at scan  chain pattern, as shown in Fig. 3 and Fig. 4.

![  Good Device  Good Device    Failing Device  Failing Device   ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ab16848f-6081-4b87-bad6-31ba51bb22d9/ab16848f-6081-4b87-bad6-31ba51bb22d9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=22132b61d4168970350b8f06b09de5cb6ec291af)
Fig. 3 - PEM analysis observed anomalous spots (circled in red).

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/986154cf-0a2d-4ad7-aeac-0b004a5cdca8/986154cf-0a2d-4ad7-aeac-0b004a5cdca8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=fbd1d2652f1c4940d02a80deeea3e64d038368bc)
Fig. 4 - PEM analysis with higher magnification observed 2 anomalous spots  (pointed with red arrows).

Layout and circuit analysis performed on the 2 emission sites  localized their origin to 2 inverters. These 2 inverters are driven  by a buffer with signal routing  Reset A  (highlighted in green  trace) (Please see Fig. 5).

![Reset A  ResetA  ResetB  Reset B  Reset C  ResetC  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/de54d763-1839-492f-a3c1-257fb536a11d/de54d763-1839-492f-a3c1-257fb536a11d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=6213701f13be63fb0f5d8520dae3c91483f31726)
Fig. 5 - Partial schematic showing the routings to the emission sites.

Further layout and circuit mapping observed that the 2  inverters with anomalous spots are driving signal  Reset B  and  Reset C . These 2 signals drive part of the scan cells within the 2  scan chain identified earlier -  chain117  and  chain118 . By  mapping signal  Reset B  (highlighted in magenta trace), we see  that the signal shows global routing that is not only a fan-out to  chain117  (highlighted in white boxes in Fig. 6) but also to  chain118  (highlighted in yellow boxes in Fig. 7). A similar  observation is identified on signal  Reset C  (highlighted in blue  trace), where it is a global routing that fans-out to both  chain117  and  chain118 .

![Emission spot observed  ission spotobsery  atinvcrter  at inverter.  Emission spot observed  Ispot  at inverter.  at inverter  ResetA  Reset A  Reset B  Reset B       Reset C  Reset C  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/25f7b927-ff0b-4599-9691-f77e6bf7950d/25f7b927-ff0b-4599-9691-f77e6bf7950d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=bcf99d79fb1d799f087c92bad5c7cd8592c60790)
Fig. 6 - Partial layout showing the routings to scan cells of  chain117

![Emissionspotobserved  atinverter  Emissionspotobserved  atinverter  ResetA  Reset A  Reset B  Reset B    Reset C  Reset C  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/364133f5-841f-4c3f-a10d-cbe58d093bbb/364133f5-841f-4c3f-a10d-cbe58d093bbb.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=1051834d177974f2e95500a7589b868f35d6ff5a)
Fig. 7 - Partial layout showing the routings to scan cells of  chain118

With the use of Scan Cell Visualizer, one can summarize that  the signal  Reset A  is driving the inverters with the anomalous  emission spots that eventually fan-out to scan cells on both  chain117  and  chain118 .

Further analysis using Electro-Optical Probing (EOP) also  benefited from the Scan Cell Visualizer. It can identify the  sequence of scan cells and distinguish which potential latch is  faulty. EOP was first performed at the driver of signal  Reset A   and its fan-out inverters, which drive the signal  Reset B  and  Reset C  (anomalous emission sites). Please see Fig. 5. EOP  results acquired at the driver for  Reset A  are comparable to a  correlation unit; however, the fan-out inverters are abnormal  (Please see Fig. 8). This shows that the signal  Reset A  is already  faulty while routing to both inverters.

![  DriverReset  Driver Reset  A           DriverReset  Driver Reset  E  B        DriverReset  Driver Reset  C  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/69f3473d-a09e-4872-b884-0ced3a7c3bdc/69f3473d-a09e-4872-b884-0ced3a7c3bdc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=290a44ab91e55862dc6903225ff96266d246637b)
Fig. 8 - EOP result of driver and fan-out of signal  Reset A .

Further EOP analysis was performed on several scan cells  from  chain118  to investigate the propagation of the failure  observed in Fig. 8. Using the Scan Cell Visualizer, together  with layout and schematic analysis, one could confirm that the  best candidates to check from the sequence of latches were  from Latch 309 to Latch 301. This is because only Latch 307 to  Latch 303 are being driven by signal  Reset B  (Fig. 9). From this,  we can identify the disparity between affected scan cells and  those that are not affected, along scan chain  chain118 .

|        DataLocator/KEdit                Select AllPath of sean chain 117file.      |
|---|


EOP analysis was performed on Latch 309 until Latch 301.   An abnormal chain shift signal is seen on Latch 307 until Latch  303. Latches prior to Latch 307 and after Latch 303 are  observed to return the normal chain shift signal (Fig. 10). This  confirms that the affected latches correlate to the signal routing  of  Reset B  that is affected by failing signal  Reset A .

![Reset B  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/570c54cb-c1be-41a4-b219-59d67fe04a04/570c54cb-c1be-41a4-b219-59d67fe04a04.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=8c5cd611c5b50eb21538f4a6b9589021e48566e8)
Fig. 10 - EOP result of Latch 309 until Latch 301.

The information from PEM and EOP analysis were then  drawn to a hypothesis of potential discontinuity along signal  Reset A  that causes subsequent  chain117  and  chain118  to fail.  Physical analysis focusing at signal  Reset A  with the help of  Passive Voltage Contrast (PVC) at every metal layer localized  the root cause of this failure to a metal void defect at Metal 4  routing (Fig. 11 and Fig. 12).

![12/10/2018  25.OkV LEI   SEM   WD5.1mr  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/011bfba6-2b44-4da1-9c96-bd854afb0fb9/011bfba6-2b44-4da1-9c96-bd854afb0fb9.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=955233250969edcf5ff7d7c83b733337a700eb8e)
Fig. 11 - High kV SEM inspection observed metal void as highlighted in red  box.

![4  ResetA  Reset A  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e65bd5f4-37a6-4fe8-9303-9a672a19cdc8/e65bd5f4-37a6-4fe8-9303-9a672a19cdc8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=ee2283d852b20bb283b1ff2346f192d1c54bac2c)
Fig. 12 - Cross section view of the metal void defect.

III. C ASE  S TUDY AND  D ISCUSSION  II

Device 2 failed a stuck-at scan chain pattern. Tessent  Diagnosis suggested the failure occurs within the scan latches  of   chain228 .  This chain consists of 536 scan cells, which were  mapped out into the CAD layout using Scan Cell Visualizer  (Fig. 13). The area of focus was then identified for subsequent  analysis.

![HEPE   22229  Scan cells  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9de913b9-cda6-489a-8381-ef3746b9c851/9de913b9-cda6-489a-8381-ef3746b9c851.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=ebcb1abb7fa27636a795bb5c68aebaea77ff40d4)
Fig. 13 - Scan Cell Visualization of  Chain228  (highlighted in white).

Backside PEM was performed by exercising the stuck-at scan  chain pattern. Multiple anomalous emission spots were  observed with 2 different setups, which are shown in Fig. 14.  The first setup was performed by looping the stuck-at scan  chain pattern and the second was performed by pausing the  stuck-at scan chain pattern at a certain vector.

![  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/02b60054-ef89-4e8a-a417-eb127726b8c0/02b60054-ef89-4e8a-a417-eb127726b8c0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=b07300fa29fd75c71c328a8148e1bceeeaae9197)
Fig. 14 - PEM analysis observed multiple anomalous emission spots (pointed to  with red arrows) with 2 different setups (Left – looping pattern; Right – paused  pattern).

The PEM results were then overlaid in the layout with the  Scan Cell Visualizer result. The result from both setups showed  that the emission spots emanated from the same signal routing,  which was the Scan Enable (SE) input for each scan cell. As an  enabler signal, it is usually routed to several scan cells.  Although it is only linked to tens of scan cells, manual mapping  of the scan cell’s chronological sequence would require careful  concentration to compare them to the scan chain list, which is

also time consuming. Using the Scan Cell Visualizer, it reduce  the effort required for both manual mapping and in identifying  the scan cell’s sequence. Fig. 15 shows the mapped scan cells  using Scan Cell Visualizer that can identify the scan cells  related to the SE’s routing and PEM results, together with other  scan cells related to  chain228 .

![  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d43fc255-81e3-48d3-9b91-40f187424d44/d43fc255-81e3-48d3-9b91-40f187424d44.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=cd5d294f255571c3ed43a789b8a4d9a34bfd5491)
Fig. 15 - Partial layout showing the routing of SE overlayed with PEM result of  both setups (Left – looping pattern; Right – paused pattern) and scan cells of  chain228 .

The Scan Cell Visualizer shows that the SE signal is routed to  multiple scan cells that are not in chronological order, as shown  in Fig. 16. This information will then assist in subsequent  analysis when identifying the sequence of scan cells related to  SE signal routing.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0f526285-d2a5-4fb7-b39a-815b4e0eab31/0f526285-d2a5-4fb7-b39a-815b4e0eab31.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=0152c3d782d90445efa0c6a9b0c1611671887333)
Fig. 16 - Partial layout showing the routing of SE signal in  Chain228

.

With the use of Scan Cell Visualizer, together with CAD  layout, 2 sets of latches were identified to check the propagation  of the failure.  The 2 sets of latches identified are ranging from  Latch 524 to Latch 521 and from Latch 515 to Latch 508. An  abnormal chain shift signal is seen on Latch 523 until Latch 522  and on Latch 510 until Latch 508. Latches other than these  ranges are observed to return normal chain shift signals   (Fig.  17). This shows that the affected latches correlates to the shared  signal routing of SE signal.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1528ad32-e631-4155-a458-694170335a9d/1528ad32-e631-4155-a458-694170335a9d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=385662981f73e44035db4be496b5d7b84acdd54f)
Fig. 17 – EOP result of Latch 523 until Latch 522 and Latch 510 until Latch  508.

The data from PEM and EOP confirmed that the SE signal  was faulty. Further EOP analysis led to a hypothesis of a  potential discontinuity along the SE signal.  Physical analysis  focusing at the SE signal with the help of PVC at every metal  layer isolated the root cause of this failure to a metal void defect  at Metal 3 routing (Fig. 18 and Fig. 19).

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/486e37c2-a110-41d7-b949-8cf3c114f654/486e37c2-a110-41d7-b949-8cf3c114f654.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=b48972acefe263e0b8ca6d7a118f553fc4557e81)
Fig. 18 - High kV SEM inspection observed metal void as highlighted in red  box.

![M13  212  NXPPQCKL  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d9d3f98e-01b0-4a0e-9d23-d41656635f15/d9d3f98e-01b0-4a0e-9d23-d41656635f15.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=bf64aac724c130181ea6d8a04ef1c63161dbec5c)
Fig. 19 - FIB cross section view of the metal void defect.

## IV. C ASE  S TUDY AND  D ISCUSSION  III  

Device 3 failed a stuck-at scan chain pattern. Tessent  Diagnosis suggested the failure occurred within the scan latches  of   chain152 . Using the Scan Cell Visualizer, the PEM spots  were found to reside within the scan chain path prior to  Latch147. EOP analysis was performed and incorrect data  shifting was observed at Latch 147. Further EOP observed  abnormal transistor switching activity at intermediate inverters  between Latch148 and Latch 147 (Fig. 20 and Fig. 21).

![SDLatch147gno  SO  SDLatch148gnd  ydd  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9e41d956-3689-4c76-a262-c4a25fbb045b/9e41d956-3689-4c76-a262-c4a25fbb045b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=f6d6e854863aa28ad85cc38c9ea09aca2e3fd36d)
Fig. 20 - Partial Schematic showing Latch 148 to Latch 147 route of  chain152 .

![E3  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ea6098f7-b8ac-460f-a7a2-84a7aa6bbabf/ea6098f7-b8ac-460f-a7a2-84a7aa6bbabf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=f3bcac0af54a42dfde5ff34a5516b64fef0e6a27)
Fig. 21 - EOP result observed abnormal transistor switching activities at site B  and site C.

Both PEM and EOP result identified a potential discontinuity  along  signal_a  routing. Since routing length was long, a binary  search via passive probing using Focused Ion Beam (FIB)  probe pads was conducted. This approach successfully  identified the potential open site and physical analysis  confirmed a metal void defect at Metal 4 routing (Fig. 22 and  Fig. 23).

![x18,000   10.OKV LED   SEM   4.1  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e927f534-409f-4ef2-8f7f-eb507aeae165/e927f534-409f-4ef2-8f7f-eb507aeae165.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=43dcc3577d77d32cfd3ce5e7a0695755653a3840)
Fig. 22 - High kV SEM inspection observed metal void as highlighted in yellow  circle.

![2.00kV50pA3.8mm1.66μm250000xTLDBSE   NXPPQCK  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/155bcc04-c963-4e6f-be08-fcb3bd7fa4ff/155bcc04-c963-4e6f-be08-fcb3bd7fa4ff.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=79b2c17d1487dbf4354f1f93648bb145463c117e)
Fig. 23 - FIB cross section view of the metal void defect.

## V. C ASE  S TUDY AND  D ISCUSSION  IV  

Device 4 failed a stuck-at scan chain pattern intermittently  during verification. Further analysis had caused device 4 to  recover, and further global fault isolation techniques from the  backside did not reveal any positive results. Tessent Diagnosis  suggested the failure occurred within the scan latches of chain14 . This chain consists of 1465 scan cells, which were  mapped out into the CAD layout using the Scan Cell Visualizer  (Fig. 24). The area of focus was then identified for subsequent  analysis.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/efedc880-2c82-4380-849c-904af353d372/efedc880-2c82-4380-849c-904af353d372.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=a8759561c95bc931576fede637de610dae6844ef)
Fig. 24 - Scan Cell Visualization of  Chain14  (highlighted in yellow)

Further analysis by performing optical inspection from the  frontside at the site of interest revealed anomalous passivation  (Fig. 25). Using the Scan Cell Visualizer together with CAD  layout, the anomaly occurred at the Scan in path towards latch  977 (Fig. 26).

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/88f72764-418a-4247-ab63-c43f526b1dda/88f72764-418a-4247-ab63-c43f526b1dda.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=6519d0e75688a334cbccd8ebe9450ef4b384d9e8)
Fig. 25 - Optical inspection revealed anomalous passivation.

![Scan-outpath  Scan in  Scan in  path  path  Latch977  Latch 977  FiBcross  isection  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/57d6ca06-eb24-4681-b46d-1c7d25464c66/57d6ca06-eb24-4681-b46d-1c7d25464c66.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=e48fbe474f36fe3a47c4b9f9a72cd6bdb4afaab8)
Fig. 26 - Partial layout showing the defect location occurred at scan in path  towards latch 977.

SEM inspections and FIB cross-sections revealed a  “volcano” defect at the scan in path towards latch 977 (please  see Fig. 27 & 28).

![volcano defect  8/31/2018HVHFWmag口WD   10um  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/19c2da6c-a6d3-4289-bac8-60139f4f22b8/19c2da6c-a6d3-4289-bac8-60139f4f22b8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=2ea8afd9f956a8ff722ef6b5a6a0fd663b16b768)
Fig. 27 - SEM imaging revealed volcano defect.

![Volcano defect occurred above scan in path of  Volcano defect occurred above scan in path of  latch977  latch 977  8/31/2018   H   HFWmag口   spm  2:20:08PM1.30kV171Um15000  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6c51dabd-62a3-4f07-808c-bc2fe66966fa/6c51dabd-62a3-4f07-808c-bc2fe66966fa.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=7f51ce373ee8f38fca2dfdc140282596aef50204)
Fig. 28 - FIB cross section view of the volcano defect.

## VI. C ASE  S TUDY AND  D ISCUSSION  V  

Device 5 failed a stuck-at scan chain pattern. Tessent  Diagnosis suggested the failure occurred within the scan latches  of   chain1 . This chain consists of 2066 scan cells. Optical  inspection observed anomalous passivation on die surface, and  using the Scan Cell Visualizer together with CAD layout, the  anomaly was identified to be occurred in the vicinity of latch  1202 and latch 1203 (Fig. 29).

![Latch 1202  Latch 1202  Latch1203  Latch 1203  Anomalous passivation  Anomalous passivation  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a80b2a85-53c4-499b-9f31-40dda249ba78/a80b2a85-53c4-499b-9f31-40dda249ba78.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=c6fc6ba7652eefa1cb54617e1bc11a9e3442e623)
Fig. 29 - Scan Cell Visualizer together with CAD layout revealed the  anomalous passivation occurred at latch 1202 and latch 1203.

SEM inspection and FIB cross-sections revealed a “volcano”  defect at vicinity of latch 1202 and latch 1203 (Fig. 30 & 31).  The VDD was routed to latch 1202 and latch 1203.

![volcano  FB cross section direction  SEMtopview  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ee664630-43a4-4421-8217-83693f1bc27e/ee664630-43a4-4421-8217-83693f1bc27e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=b948186ff9f13ea180dd863d011ae858abcb6856)
Fig. 30 - SEM imaging revealed volcano defect.

![ALCAP  volcano  VDD routing to latch 1202 & 1203  VDDrouting to latch 1202& 1203  Abnormalmetallza  Crosssectionview  4/1/2019HVHFW|mag口WD   2um  4:13:02PM1.30kV7.31μm|35000x3.8mm  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/4a7df66a-6c5f-4e24-af9c-c60cd3b63f1d/4a7df66a-6c5f-4e24-af9c-c60cd3b63f1d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215645%3B1743219245&q-key-time=1743215645%3B1743219245&q-header-list=host&q-url-param-list=&q-signature=243e9805e6d19ece5408d43891330029158ba896)
Fig 31 - FIB cross section view of the volcano defect.

## VII. C ONCLUSION 

The implementation of a Scan Cell Visualizer can assist  Tessent Diagnosis in providing a good analysis of suspected  failing nodes for scan chain failure. By utilizing a Scan Cell  Visualizer, is one option in providing increased fault isolation  efficiency when hundreds to thousands of individual scan cells  are required to be spatially mapped. As IC design has been  advancing rapidly, it drives an increase in device complexity  along with a shrinking in transistor feature sizes. Therefore,

there exists a great challenge to every analyst to narrow down  the failure quickly. The introduction of a Scan Cell Visualizer  into the FA flow will reduce both the time and effort required to  map out all the scan cells to quickly provide an overview of  specific areas of interest for further analysis.

## A CKNOWLEDGMENT 

The authors would like to sincerely thank Min Xia of  Synopsys for providing the initial visualizer script and both  Kris Dickson and John Sanchez from the NXP Product  Diagnostic Center in Austin, TX for their help in enabling the  use of Scan Cell Visualizer.

## R EFERENCES 

[1]   Z.G. Song, S.P. Neo, T. Tun, C.K. Oh, K.F. Lo,  “Diagnosis and failure  analysis for scan failure” ,  proceedings of the 12th International  Symposium on the Physical and Failure Analysis of Integrated Circuits ,  2005, IPFA, 2005.     [2]   Yu H., Reifeng G., Wu-Tung C., James C.,  “Survey of scan chain  Diagnosis” ,  IEEE Design & Test of Computers , Vol. 25, pp. 240-248,  2008    [3]   Huajun C., Zichu Q., Lin W., Chao X.,  “A scan chain optimization  method for diagnosis” ,  33rd IEEE International Conference on  Computer Design (ICCD) , 2015    [4]    Ruifeng G., S. Venkataraman,  “A technique for fault diagnosis of  defects in scan chains”, proceedings International Test Conference ,  2001    [5]   Yu H., Will H., Yuan-Shih C., Wu-Tung C., Ruifeng G., Albert M.,  “Diagnose compound scan chain and system logic defects”, IEEE  International Test Conference , 2007    [6]   Seiichi N., Hiroji N.,  “Binary Search Revisited: Another Advantage of  Fibonacci Search” ,   IEEE Transactions on Computers , Vol. C-36, pp.  1132-1135, 1987    [7]   M.Grützner, C.Burmer, C.Brillert,  “Ultra-fast CAD scan chain  highlighting for failure analysis assistance” ,   Microelectronics  Reliability , Vol. 50, Issues 9-11, pp 1494-1498, 2010

