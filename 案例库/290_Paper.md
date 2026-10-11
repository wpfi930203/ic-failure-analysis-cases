---
title: "290_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_1e5cd1ba51975ac660611560ae9772e67295230462135641
file_size: 948044
---

## Study of Front-Side Approach to Retrieve Stored Data in Non-Volatile Memory  Devices Using Scanning Capacitance Microscopy   

J.Y. Tay 1 , J. Cheah 1 , Q. Liu 1 , and C.L Gan 1,2,\*

1 Temasek Laboratories@NTU, Nanyang Technological University, 50 Nanyang Drive, Singapore 637553    2   School of Materials Science and Engineering, Nanyang Technological University, 50 Nanyang Drive, Singapore 639798  Email: CLGan@ntu.edu.sg \*

Abstract-  Data are stored as electrical charges in floating gates of  the transistors in Non-Volatile Memory (NVM) devices. Reading  back this stored data will help in understanding how memory is  organized which is important in the digital forensics field. Sample  preparation from back-side approach had been attempted and  scanning capacitance microscopy (SCM) can be used to probe the  charges stored in the floating gate transistors directly. However,  it is challenging to attain a uniform surface across the memory  device using mechanical polishing and also difficult to read back  the full data. In this paper, front-side sample preparation will be  discussed for data retrieval with SCM probing method. The  application has been demonstrated on 8-bit microcontroller with  16 KB ISP flash memory and 512 bytes EEPROM.

Keywords – Non-Volatile Memory, front-side sample preparation,  scanning capacitance microscopy, data retrieval

## I. I NTRODUCTION 

Non-Volatile Memory (NVM) devices are used in many  different fields of applications such as cache in mobile devices  and high-end processors, artificial intelligence, transportation  and consumer electronics [1, 2]. Understanding how the  memory is organized and reading back the stored content inside  the memory is useful for failure analysis and digital forensics  [3, 4]. There are many types of NVM devices such as  EEPROM, flash memory, RRAM, etc. Some of these devices  store the content in the form of electrical charges [5]. Scanning  capacitance microscopy (SCM) is one of the methods that can  be used to characterize these stored charges. SCM reading of  stored data has been proved to be non-destructive to the data  and repeatable [6-9].

Some researchers have demonstrated the technique by  polishing to the tunnel oxide from the back-side approach. The  charges stored inside the floating gate can be measured through  this tunnel oxide [6-9]. In their studies, the samples must be  deprocessed to less than 300 nm from the interface to make the  near field electrical measurements. This is because for the SCM  approach to work, the SCM tip has to probe the charge density  located at the floating gate transistor (FGT) channels directly.  An example of a FGT is shown in Fig 1. However, the studies  only demonstrated content extraction in a localized region as it  is challenging to obtain a uniform surface through polishing  from the back-side. Hence it is not able to read back the full  data stored in the memory block. In this study, a uniform  surface of the NVM memory was obtained with precise control  from the front-side approach and the stored data from the  memory block was retrieved through the SCM technique.

![Control Gate    Gate Oxide  TunnelOxide   Floating Gate  Source   Channel   Drain  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/10edd794-39d8-4e81-b86a-a6ce9f72e25c/10edd794-39d8-4e81-b86a-a6ce9f72e25c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=ad798b37d5deafca1589137b184259cd9812dead)
Fig. 1 Example of a floating gate transistor.

## II. EXPERIMENTS  

## A.    Study of device   

In our study, a 8-bit microcontroller of 250 nm technology  node with embedded 512 B EEPROM and 16 KB Flash was  investigated. The embedded EEPROM and Flash memory  blocks are boxed in red and yellow as shown in Fig. 2,  respectively. The flash memory block consists of 16 rows while  the EEPROM has 3 rows of memory cells.

![.63  EEPROM  FIASH  2.63mm  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9a63b238-2336-4003-9a4b-c1b2fe7d7b18/9a63b238-2336-4003-9a4b-c1b2fe7d7b18.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=ebdaec7d75187a32eb8554cd00a7088295550d99)
Fig. 2 Exposed sample die before deprocessing steps. EEPROM  (box in red) and flash memory (box in yellow) are identified.

A FIB cross-section cut was performed at the memory cell  and the floating gate structure consists of Poly 2 layer wrapping  over Poly 1 layer as shown in Fig 3.

![a   Metal2  FGI  Poly 2control gate  Oxidelaye  Poly1 floatinggate  Tunnel oxide  5.0kV6m0000×52°4.9m   DNT  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/295e5324-e198-484e-98dd-88fecbd5e6c8/295e5324-e198-484e-98dd-88fecbd5e6c8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=1d4dda3db728f4f02ab699fd25765243762aade5)
Fig. 3 SEM image of (a) sample cross-section and (b) zoom-in of  FGT.

## B.    Sample Preparation 

Three of the same devices were programmed with 3 different  hexadecimal codes [Hex 55 (0101 0101), Hex AA (1010 1010)  and Hex 00 (0000 0000)]. The codes were written to both the  flash memory and EEPROM of the samples. This is to verify  that the distinct patterns of the different hexadecimal codes can  be observed in the returned SCM scan data.

The three programmed samples were then soaked in fuming  nitric acid to remove the epoxy molding compound (Fig. 4(a)).  Exposure of the oxide layer above the Poly 1 (floating gate)  was achieved by removing the passivation layer, metallization  layers and Poly 2 layer (control gate). This allows the SCM tip  to probe the oxide layer above the floating gate directly by  measuring the change of capacitance of its stored charges.  Extra care was taken during the sample preparation to avoid  perturbing the stored charges.

During the sample preparation, conventional physical failure  analysis techniques such as RIE and chemical etching were  used to remove the different layers in the studied chip. RIE was  only used to remove the top passivation layer as it was reported  that both SEM inspections and Reactive Ion Etching (RIE) are  not recommended during sample preparation. This is to avoid  charging the oxides and disturbing the real floating gate  potentials as reported by Nardi  et   al  [10]. In our case, the  floating gate is embedded far away from the top passivation  layer, thus the chance of affecting the stored data is low.  Keeping the surface clean is also important for SCM charge  measurement. Thus, cleaning has to be conducted when  necessary during the sample preparation.

Additionally, with the front-side approach of the sample  preparation, a global uniformity of the memory area was  achieved as shown in Fig. 4(c). Subsequently, memory content  access is feasible with the SCM technique. Fig. 5(a)-(f) are the  zoom-in optical images captured at the six sites of the memory  area indicated in Fig. 4(c).

![a  200L  6  200um  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/36bd8357-69f1-4717-be47-3052798c3f2d/36bd8357-69f1-4717-be47-3052798c3f2d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=8bd9f8a1fc97d306310742ddc471a04fba1c8557)
Fig. 4 Planar view of sample under optical microscope. (a) Before  deprocessing steps. (b) Poly 2 layer. (c) Poly 1 layer after TMAH step.  (d) Zoom-in of EEPROM top row with 8 memory cells in a column.

## A.    Sample Preparation 

It is critical not to cause over-etch or under-etch during the  buffered oxide etch (BOE) steps. Long BOE etching time will  often cause over-etching. As the deprocessing proceeds nearer  to Poly 2 layer, BOE can etch both the gate structure side-wall  and region below Poly 1, which might lead to the Tetramethyl-ammonium hydroxide (TMAH) etching Poly 1 [10] in the later  stages. For this sample, since the Poly 2 is wrapped over Poly 1,  it provides some protection to Poly 1 against the BOE and  TMAH over-etching Poly 1. Precision control over BOE time  will be needed for other floating gate structures such as stacked  floating gates.

From Fig. 4(c) and Fig 5(a)-(f), it shows the surface  uniformity of the memory block after the TMAH step. Zooming  in at the memory cells of the EEPROM memory array, 8  memory cells in a column can be seen clearly in Fig. 4(d).  Stored data can be read out from these memory cells.

![C   d  e  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/56f4f440-ae11-4aab-ac1a-8a998ed13dd4/56f4f440-ae11-4aab-ac1a-8a998ed13dd4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=cfd402126ea318b6fdf5f98c38f747fc0bb4ca93)
Fig. 5 Zoom-in images of the six sites indicated in Fig. 4(c): (a) Site 1,  (b) Site 2, (c) Site 3 (d) Site 4, (e) Site 5 and (f) Site 6.

Programming different hexadecimal codes into the same  memory block of different samples will allow the  understanding of how data are stored in the actual cell location  and the memory address being used. In such scenario, uniform  sample preparation will be very critical in order to obtain the  whole memory content.

## B.    Scanning Capacitance Microscopy  

The prepared samples were measured using Parks System  NX20 AFM. The SCM scan was conducted on all 3 rows of  EEPROM and some parts of the FLASH memory of samples to  demonstrate the uniformity of the sample preparation and the  retrieval of their data. SCM detects differential capacitance at  fixed DC and AC bias voltages as the AFM tip scans the sample  surface and simultaneous images of both topography and  differential capacitance are obtained. The SCM scan  parameters used were 4 to 5 V DC bias applied to the substrate,  6 to 7 V AC bias applied to the tip and   $+90^{\mathrm{o}}$   phase. The  parameters of the AFM set-up have to be optimized in order to  acquire meaningful signals, especially the applied voltages

used. Higher AC voltage will give higher changes in  capacitance but results in larger depletion volume and lower  spatial resolution [11]. It was also recommended to maintain  DC and AC voltages at the lower range, away from program  erasable voltages for flash devices [6].

Hex 55, Hex AA and Hex 00 hexadecimal codes were read  back from the scan data of the three samples respectively as  shown in Fig. 6. Fig. 6(a), (c) and (e) show the SCM  topography of the same corner of each sample, and Fig. 6(b), (d)  and (f) show the amplitude signals appearing as bright and dark  spots. Bits   $\mathbf{\epsilon}_{0},$   will appear as bright spots while Bits ‘1’ will  appear as darker spots in SCM amplitude scan for this device.  We can conclude that the front-side deprocessing method is  able to successfully delayer till oxide layer with the electrical  charges preserved and SCM is able to read back stored data in  the floating gate.

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/48f23e28-e574-4364-bb23-5c0365238714/48f23e28-e574-4364-bb23-5c0365238714.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=edae793face8ac90ec1eeb1e0a8357a55622de40)
Fig. 6 SCM (a), (c) and (e) topography and (b), (d) and (f) amplitude  scan images at the left corner of Row 3 of the EEPROM of the  samples with Hex 55, Hex AA and Hex 00 hexadecimal codes,  respectively.

With uniform sample preparation, the stored data over the  memory block can be read back. From Fig. 7, it shows the SCM  scans on six sites of the memory blocks of the sample  programmed with Hex 00 hexadecimal codes as a  representative. Site 1 to 4 are the four corners of EEPROM  memory block and Site 5 and 6 are the top 2 corners of FLASH  memory block as shown in Fig 7(a). Hexadecimal codes of  “0000 0000” were read back from the scan data of memory  block, thus demonstrating the uniformity of the sample  preparation.

In Fig. 8(b), it shows the line profile of the memory cells with  the width measured  ${\sim}1~{\upmu\mathrm{m}}$   and depth measured \~117 nm from  the sidewall to oxide layer above Poly 1. The AFM tip has a  radius curvature better than 25 nm and height of   $15\;\upmu\mathrm{m}$  , hence  the tip is able to probe into this trench size. However, the AFM  tip can get worn out during the large area scan where there is a

big difference in height topography since the SCM scan is in  contact mode. This can be observed in Fig. 7(b) and Fig. 7(h) as  the topography features in Fig. 7(b) look sharper as compared  to Fig. 7(h). The image in Fig. 7(h) was the last image scanned  in the EEPROM as compared to Fig. 7(b), which was the first  image scanned. Frequent checking of the image quality is  required during the scanning of large area as there might be a  need to change a new tip. The image quality will be greatly  affected by the tip condition and surface cleanliness.

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/0c85b6cf-8984-4668-b3e8-a29fefed29ce/0c85b6cf-8984-4668-b3e8-a29fefed29ce.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=d559e57544546fdc3731a846d6093d192608023f)
Fig. 7 (a) Sample programmed with Hex 00 hexadecimal code as a  representative showing SCM scan data of six sites circled in white.  SCM topography and amplitude scan images of: (b) & (c) Site 1, (d)  & (e) Site 2, (f) & (g) Site 3, (h) & (i) Site 4, (j) & (k) Site 5, (l) & (m)  Site 6.

![Line Prcfile:Red  CUFSOE   Angle[deg)  DRed   0.905   -0.117   7363  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c518530f-71b3-43e8-9edf-fb71c734685e/c518530f-71b3-43e8-9edf-fb71c734685e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215687%3B1743219287&q-key-time=1743215687%3B1743219287&q-header-list=host&q-url-param-list=&q-signature=096c0e659689cda5900f348e5a0b801f8cad4a67)
Fig. 8 Top left corner of EEPROM of the sample with Hex 00  hexadecimal codes. (a) SCM topography with a red line cutting across  the columns of memory cells and (b) showing the line profile  indicating the width and depth of the memory cells.

## IV. CONCLUSION  

In this paper, repeatable SCM sample preparation to the  oxide layer above the Poly 1 FG of both EEPROM and flash  has been successfully demonstrated on a 8-bit microcontroller of   $250\,\mathrm{\nm}$   technology node. Front-side sample preparation  approach through chemical methods can provide better  uniformity than back-side approach. With precisely control  sample preparation and AFM setup, programmed data can be  retrieved through the SCM scanned data for digital forensics.

## REFERENCES  

[1]    J.S. Meena  et al , “Overview of Emerging Non-volatile Memory  Technologies”,   Nanoscale Research Letters , Vol. 9, pp. 1-33, 2014    [2]    K.Baker, “Embedded Nonvolatile Memory technology”,  IEEE  International Conference on IC Design and Technology , 2381-3555,  2009    [3]    B.J. Jones, A.J. Kenyon, “Retention of Data in Heat- Damaged SIM  Cards and Potential Recovery Methods”,  Forensic Science  International , Vol. 177, pp. 42-46, 2008    [4]    D I Konopinski, A J Kenyon. “Data Recovery from Damaged Electronic  Memory Devices”. Retrieved from:  https://www.researchgate.net/publication/254814425_Data_recovery_ from_damaged_electronic_memory_devices    [5]    S.P. Skorobogatov, “Data Remanence in Flash Memory Devices”,  Cryptographic Hardware and Embedded Systems – CHES 2005.  Lecture Notes in Computer Science , Vol. 3659, 2005    [6]    Rudra S. Dhar  et al.,  “Direct Charge Measurements to Read Back  Stored Data in Nonvolatile Memory Devices Using Scanning  Capacitance Microscopy”,  Journal of Vacuum Science & Technology B,  Vol. 31, 061801, 2013    [7]    Rudra S. Dhar  et al.,  “Read Back of Stored Data in Non Volatile  Memory Devices by Scanning Capacitance Microscopy”,  Materials  Research Society Proc.,  Vol. 1527, 2013    [8]    C.D.Nardi  et al.,  “Direct Measurements of Charge in Floating Gate  Transistor Channels of Flash Memories Using Scanning Capacitance  Microscopy”,   Proceedings of the  $32^{n d}$  International Symposium  Testing and Failure Analysis(ISTFA),  P. 86, 2006    [9]    C.D.Nardi  et al.,  “Descrambling and Data Reading Techniques for  Flash-EEPROM Memories. Application to Smart Cards.”,   Microelectron. Reliab.,  Vol. 46, pp. 1569- 1574, 2006       [10]    C.D.Nardi  et al.,  “Oxide Charge Measurements in EEPROM Devices”,  Microelectron. Reliab.,  Vol. 45, pp. 1514- 1519, 2005       [11]    J.J. Kopanski, “Scanning Capacitance Microscopy for Electrical  Characterization of Semiconductors and Dielectrics”,  Scanning Probe  Microscopy , pp. 88- 112, 2007

