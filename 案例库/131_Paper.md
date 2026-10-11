---
title: "131_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_1650ca8e1641f0c9ba4ec2535cdf00ae7295230462135641
file_size: 620677
---

## Analysis of SEE modes in ferroelectric random access  memory using heavy ions  

Jia-Nan Wei 1,2, Hong-Xia Guo  ${}^{2,3^{*}}$  , Feng-Qi Zhang 3, Gang Guo 4, and Chao-Hui He 1 \*   1 School of Nuclear Science and Technology, Xi′an Jiaotong University, Xi′an, 710049, China.    2 Key Laboratory for Low Dimensional Materials and Application Technology of Ministry of Education, Xiangtan University,  Xiangtan, 411105, China.    3 State Key Laboratory of Intense Pulsed Irradiation Simulation and Effect, Northwest Institute of Nuclear Technology, Xi′an,  710024, China.  4 National Innovation Center of Radiation Application, China Institute of Atomic Energy, Beijing, 102413, China.    \*  Email:  weijianan93@163.com  (Jia-Nan Wei),  guohxnint@126.com  (Hong-Xia Guo),  hechaohui@xjtu.edu.cn  (Chao-Hui He)

Abstract-   The single event effects (SEE) in ferroelectric random  access memories (FRAM) are investigated and the error modes  are analyzed using heavy ions. Under the irradiation of heavy ions  with high linear energy transfer (LET) values, data upsets are  dominated by “0” to “1” upsets of which the cross section is larger  than that of “1” to “0” upsets by an order of magnitude and most  upsets are detected in addresses with the all “1” error pattern  (FFFFH). In addition, most of the upsets occur in events that  involve several consecutively accessed addresses. With the  increase of ion LET, the percentage of the data upsets in events  involving more than 10 consecutively accessed addresses increases  monotonically.

Keywords  – Ferroelectric random access memory, Single event  effect, Heavy ion .

## I. I NTRODUCTION 

Ferroelectric random access memory (FRAM) is a type of  non-volatile memory which is widely used in metering,  automotive electronics and industrial control. It uses  ferroelectric materials such as lead zirconate titanate (PZT) and  barium strontium titanate (BST) as its storage medium [1].  Compared with conventional non-volatile technologies such as  Flash and EEPROM, FRAM features high read/write speed,  unlimited endurance cycles and low power consumption [2].  Besides, FRAM represents a promising candidate for space  applications because ferroelectric materials have built-in  tolerance to total ionizing dose (TID) and high-energy ions  [3]-[7].

In recent years, micro/nano satellites employ more and more  commercial-off-the-shelf (COTS) components to cut down the  cost and improve the performance, which makes the reliability  of FRAM in harsh space radiation environment a hot topic.  Although the ferroelectric capacitor which is the key  component has good resistance to radiation, the peripheral  circuits fabricated based on standard complementary metal  oxide semiconductor (CMOS) process such as the address  decoder and sense amplifier are susceptible to single event  effects (SEE) [8]. A previous report has shown that the data  upsets in FRAM all originate from the peripheral circuits under  the irradiation of Bi ions with a maximum effective linear  energy transfer (LET) of   $99.3\,\,\mathrm{MeV}\!\cdot\!\mathrm{cm}^{2}\!\cdot\!\mathrm{mg}^{\!-\!1}[9]$  . The single  event upset (SEU) threshold is also very low. Heavy ions with

LET of   $1.8\;\;\mathrm{MeV}\!\cdot\!\mathrm{cm}^{2}\!\cdot\!\mathrm{mg}^{-1}$   are able to cause upsets in the  FRAM based on 130 nm technology [10]. Moreover, the errors  induced by heavy ions have various patterns and many  mechanisms can be involved, making the failure analysis more  complicated [11]. However, up to now, information concerning  the percentages of different error categories and their  relationship with ion LET is not enough and there is still a lot of  work to do.

In this work, heavy ions are used to investigate SEE in 4 Mbit  COTS FRAMs manufactured by Cypress. Cross sections,  including total upset cross sections, “0” to “1” upset cross  sections, “1” to “0” upset cross sections and event cross  sections at different ion LETs are given. Characteristics of the  different error categories and their relationships with ion LET  are summarized and analyzed.

## II.   E XPERIMENTAL  D ETAILS 

The devices under test (DUT) are 4 Mbit FRAMs (FM22L16)  with 16 bits per cell. The memory cell of FM22L16 is based on  the advanced high-reliability ferroelectric process while the  peripheral circuit is based on 130 nm CMOS technology. The  memory array is logically organized as   $262{,}144{\times}16$   and is  accessed using an industry standard parallel interface. The  262,144 addresses are organized as 8 blocks, each block has  8,192 rows and each row has 4 column locations. More detailed  features of the DUT are listed in TABLE I.

TABLE I - Detailed features of FM22L16

|Bias (V)|Access time (ns)|Active current (mA)|Standby current (μA)|Package|
|---|---|---|---|---|
|3.3|55|18|150|TSOP|


Heavy ion experiment was performed at the HI-13 Tandem  Accelerator in China Institute of Atomic Energy, Beijing. Ti, Br  and I ions were used to investigate the SEE response of the  DUTs under different LETs. The detailed information of the  ions is listed in TABLE II. Fig. 1 is the diagram of experimental  setup. The irradiation board on which DUTs were soldered was  mounted on a sample holder. The sample holder sits on a  three-axis motorized stage so that DUTs at different positions  can be aligned to the ion beam. The SEE digital tester  implemented through FPGA was mounted on the back of the

sample holder to avoid being struck by the ions and was  connected to the irradiation board through ribbon cable. The  irradiation board and the SEE tester were put in the vacuum  chamber to eliminate the attenuation of ion energy by air. The  host computer outside the chamber communicated with the SEE  tester through network cable. The experiment was performed at  room temperature and all ions were at normal incidence. The  spot size of the ion beam was about   $2\,\mathrm{cm}{\times}2$   cm. Before test, the  plastic package of all DUTs was removed using phosphoric  acid corrosion from front side to expose the die. The thickness  of the overlayers (metallization and passivation) on the top of  the die is about  $5~{\upmu\mathrm{m}}$   [9]. TABLE III shows SRIM calculation  results of ranges of the ions in the pure materials used in these  layers respectively. Denser materials such as W and Sn are not  considered here because they are used in very small amounts.  Based on the results in TABLE III, we can estimate the  attenuation caused by these overlayers to be minor and the ions  have enough ability to deposit energy in the sensitive region  since the depth of the sensitive volume of 130 nm technology is  less than 400 nm [12].

TABLE II - Summary of heavy ion information.

|Ion type|Energy (MeV)|LET (MeV·cm 2 ·mg -1 )|Flux (cm -2 ·s -1 )|Fluence (cm -2 )|
|---|---|---|---|---|
|Ti|185|21.3|5×10 3|1×10 6|
|Br|240|41.8|4.9×10 3|1×10 6|
|I|284|65.6|1×10 4|2×10 6|


![Vacuumchamber  DOT  Ionbeam  Digital  tester  Three-axis   Sample  motorized   holder  stage  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bb6e51e7-1c49-47a2-9105-ebbbfa98dcf1/bb6e51e7-1c49-47a2-9105-ebbbfa98dcf1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=7f4659abdb4167b8c36faba437ddc2369f0721cc)
Fig. 1  Diagram of the experimental setup for heavy ion irradiation.

TABLE III - Ranges of used heavy ions in materials.

|Material|Density (g.cm -3 )|Range (μm)|Range (μm)|Range (μm)|
|---|---|---|---|---|
|Material|Density (g.cm -3 )|Ti|Br|I|
|Si|2.32|37.9|32.4|30.1|
|SiO 2|2.2|37.3|31.8|29.4|
|Cu|8.9|14.7|12.9|12.2|
|Al|2.7|33.2|28.6|26.6|
|Si 3 N 4|3.44|23.7|20.2|18.7|


Before irradiation, 5555H was written into the DUTs. During  irradiation, the DUTs operated in dynamic mode. Data was read  back cyclically and compared with the initial data to obtain

error information such as the error bit, error address and error  type (  $"0"$   to “1” or “1” to  $"0"$  ). In a single read out of the DUTs,  the 262,144 addresses were accessed sequentially.

## III.   R ESULTS AND  A NALYSES 

During the heavy ion experiment, no typical single event  latch-up (SEL) event with a dramatic increase of supply current  was observed. Fig. 2 shows the upset cross sections as a  function of ion LET. For each data point, the standard deviation  has been calculated and reported. The total upset cross section  (σ t ) under Ti ions is about   $1.1{\times}10^{-4}~\mathrm{cm}^{-2}$   and it increases to   $3.9{\times}10^{-4}~\mathrm{cm}^{-2}$   under the irradiation of Br ions.   $\upsigma_{\mathrm{t}}$   caused by I  ions have similar values to that caused by Br ions, indicating  that the cross section has reached saturation.   $"0"$   to “1” and “1”  to   $"0"$   upset cross sections are calculated and are termed   $\upsigma_{0\rightarrow1}$    and  $\upsigma_{1\rightarrow0}$   respectively. Under Ti irradiation,  $\upsigma_{0\rightarrow1}$   is only slightly  larger than   $\upsigma_{1\rightarrow0}$  . While under the irradiation of Br and I ions,   $\upsigma_{0\rightarrow1}$    is larger than  $\upsigma_{1\rightarrow0}$   by an order of magnitude. That is to say,  the increase of   $\upsigma_{\mathrm{t}}$   should be mostly attributed to the increase of   $\upsigma_{0\rightarrow1}$  .

![4.0E-4- 3.0E-4 2.0E-4 tas  1.0E- 20  30  60 LET(MeV·cm²·mg-1) ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d61b3485-c82f-4409-a04f-72d9f593957c/d61b3485-c82f-4409-a04f-72d9f593957c.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=ec9c0d831aca29f8f6412dd8619a055c91ac5f72)
Fig. 2  Upset cross sections as a function of ion LET.

According to the log files of the SEE tester, the huge disparity  between  $\upsigma_{0\rightarrow1}$   and  $\upsigma_{0\rightarrow1}$    under Br and I ions is because that many  upsets occur with the data from 5555H to FFFFH, the all “1”   pattern. Fig. 3 shows the percentage   $\mathrm{(P_{a})}$   of the error addresses  with a FFFFH pattern in all error addresses and the percentage   $(\mathrm{P_{u}})$   of upset bits in these FFFFH addresses in all upset bits. It is  obvious that   $\mathrm{P_{a}}$   and   $\mathrm{P_{u}}$  increase monotonically with ion LET.  Under the irradiation of Br and I ions, addresses with the  FFFFH error pattern make up more than  $55\%$   of the whole error  addresses and the upsets at these addresses make up more than   $70\%$   of the whole upsets. However, this contribution is much  smaller when the DUT is irradiated by Ti ions, indicating that  the occurrence of FFFFH errors is related to the LET of incident  ions. The frequently occurred FFFFH upsets suggest that the  upset mode is not random and an abnormal condition that  affects the access of all the memory cells in an address may  occur in the peripheral circuits. A reasonable hypothesis is the  charging of the bit line (BL). Fig. 4 shows the schematic of the  1T-1C ferroelectric memory cell. It consists of a ferroelectric  capacitor (C FE ) that is connected to the plate line (PL) at one end  and to BL via an access NMOS at the other end. The gate of the  NMOS is connected to the word line (WL).   $\mathrm{C_{BL}}$  is the parasitic

capacitance of BL. According to the operating principles of  capacitor-type FRAM, the readout of a memory cell is driven  by a positive voltage applied on PL. Then the polarization  reversal current conducted to BL will be sensed by the  amplifier. This is a destructive operation because the  polarization state of the ferroelectric capacitor has changed.  Therefore, a write back operation is necessary to restore the  data on BL to the memory cell. However, if BL is wrongly  charged by ion-induced high current events such as  micro-latch-ups, the input of the sense amplifier will always be  high so that the output will always be “1”. In addition, the write  back operation will restore the capacitors with all “1”. As a  result, the output will also be “1” in the following read cycles.  Of cause, it seems impossible that all the 16 bits could always  be disturbed together. There are also some addresses with data  bits that are partially flipped from “0” to “1”.  These addresses  have error patterns such as FFFDH and 7FFFH.

![100  80  20  Er  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/8601ddbe-e04c-4a56-aa69-84d951bd5cdf/8601ddbe-e04c-4a56-aa69-84d951bd5cdf.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=2497da07d90a25334e7a199361ef38983cebc615)
Fig. 3  Percentage of addresses and upsets from 5555H to FFFFH.

![EL  L  EL  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/2fa00d3b-dace-4464-bf93-1479d10d49ab/2fa00d3b-dace-4464-bf93-1479d10d49ab.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=a474cbef8f797dc14a7c567b27cc45098b71ea01)
Fig. 4  Schematic of 1T-1C ferroelectric memory cell.

Another noteworthy phenomenon is that most upsets occur in  events that involve several consecutively accessed addresses.  Fig. 5 shows the event cross section   $(\upsigma_{\mathrm{e}})$   as a function of ion  LET. Compared with the results in Fig. 2,   $\upsigma_{\mathrm{e}}$   is smaller than   $\upsigma_{\mathrm{t}}$  by an order of magnitude, indicating that many upsets occur  synchronously in a single event. The observed upset events are  categorized into the four types listed in TABLE IV according to  the length of addresses they cover. Noting that though we use  SCU (single-cell upsets) and MCU (multiple-cell upsets) to

depict these upsets, they are totally different in mechanism  from the commonly called SCU and MCU which are caused by  incident particles directly in the memory array. For FRAM, the  SEE originates from the peripheral circuits, though the final  response of the DUT is also the upset of data. Fig. 6 shows the  percentage of each event category under different ions. SCU,  MCU-I and MCU-II make up no less than  $80\%$   of the events for  all the three ion types. However, this does not mean that the  impact of MCU- III events is minor. On the contrary, those few  MCU-III events may lead to huge amounts of upsets due to the  length of addresses they can cover, especially under the  irradiation of Br and I ions. Fig. 7 shows the percentage of  upsets caused by each category of event. Under the irradiation  of Ti ions, only  $24.4\%$   of the upsets occur in the form of SCU,  while   $56.4\%$   of the upsets occur in the form of MCU-I that  involves 2-5 consecutively accessed addresses. With elevated  LET, the percentage of SCU decreases gradually. At the same  time, a sharp increase can be found in the percentage of upsets  that occur in the form of MCU-III event that involves more than  10 consecutively accessed addresses. Under I ions, only   $10~\%$  upsets are SCU while   $74\%$   of them belong to MCU-III.   Moreover, the distribution of the addresses with the FFFFH  pattern shows a similar trend, as is shown in Fig. 8. As the ion  LET increases, more and more FFFFH error patterns tend to  occur in MCU-III events. Under I ions, the percentage can  reach   $87.0\%$  . This means that the disturbances caused by single  ions may last quite a long time. In the previous publication, the  supply current transients caused by micro-latch-up can last  several microseconds [13]. While the cycle time for a single  address is about   $0.5~\upmu\mathrm{s}$   in this work, it is unexpected that more  and more consecutively accessed addresses are corrupted.

![2.5E-5  2.0E-5  1.5E-5  1.0E-5  5.0E-6  20   30   40   60   60  LET(MeV·cm²·mg-1)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/726c591e-d889-4f7f-a3e0-c8b4713e396e/726c591e-d889-4f7f-a3e0-c8b4713e396e.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=9801760a4823b2c3342c407ebba7305612cdcdbf)
Fig. 5  Event cross section as a function of ion LET.

TABLE IV - Summary of upset event categories.

|Category|
|---|
|SCU|
|MCU-I|
|MCU-II|
|MCU-III|


![100  MCU-III  MCU-II  MCU-I  80  IsCU  60  40  20  Br  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f23a7fec-4d31-4929-a6eb-afdb6e31f104/f23a7fec-4d31-4929-a6eb-afdb6e31f104.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=570218afa55140ae8e508784d007e70b112406c4)
Fig. 6  Percentages of different categories of events.

![100-  MCU-III  MCU-II  MCU-I  80-  SCU  60  20  Br  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d9571c0b-fa02-4c26-beec-ddb18f6df4f4/d9571c0b-fa02-4c26-beec-ddb18f6df4f4.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=0148f69fadc31f7a906bff9cd7eac94be17ef1a6)
Fig. 7  Percentages of upset bits caused by different categories of events.

![MCU-III  100  MCU-II  MCU-I  SCU  80-  60.  20  Er  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f9900b9f-3f9b-4117-9a07-6cbee51a8f6a/f9900b9f-3f9b-4117-9a07-6cbee51a8f6a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=56af07fd62d5a0abe0a22a233401d763edfba454)
Fig. 8  Distribution of FFFFH pattern in different categories of events.

Besides, some violent disturbances were recorded during the  irradiation. These disturbances occurred only in one read cycle  of the DUT and recovered spontaneously in the next read cycles,  influencing hundreds to even thousands of consecutively  accessed addresses. The error patterns of the addresses in a  certain event tend to be same. Here we call these disturbances  transient upsets because of the difference from the upsets  mentioned above which are stable and can persist unless the  DUT is reconfigured. Fig. 9 shows the number of upsets  obtained in typical runs of heavy ion test with varied LETs,  each column represents the upset number of a single readout of  the DUT. It can be found that the number of upsets in the  transient upset events is much larger than that of the stable  upsets. In addition, the transient upset events occur more  frequently during Br and I irradiation than during Ti irradiation.  Since the transient upsets can recover spontaneously, the  ferroelectric cells are not corrupted. Therefore, this kind of

errors could be metastable states caused by micro-latch-up  events in the readout circuits or data buffer [14]. When the  metastable state recovers, the DUT could work normally.

![60000  50000   EBr  40000  30000  Typicaltransientupsets  10000  Typicalstableupsets  5000  50   100   150   200  Time (s)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b925160f-823b-4c34-9d03-d942bafc0e8b/b925160f-823b-4c34-9d03-d942bafc0e8b.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215631%3B1743219231&q-key-time=1743215631%3B1743219231&q-header-list=host&q-url-param-list=&q-signature=6919e6c137022512b495343c1bf1506d56703319)
Fig. 9  Upsets recorded in a typical run of heavy ion test.

## IV. C ONCLUSION 

The 4 Mbit COTS FRAMs are irradiated with heavy ions to  investigate their SEE responses. The data upsets are dominated  by “0” to “1” upsets under irradiation of ions with high LET and  data in most upset addresses is FFFFH. In addition, the  percentage of upsets that occur in events involving more than  10 consecutively accessed addresses increases monotonically  with ion LET and so does the upsets with FFFFH pattern. The  charging of BL caused by micro-latch-up events may be the  reason. Meanwhile, transient events which involve hundreds to  thousands of consecutively-accessed addresses were also  recorded. These upsets can be attributed to the metastable states  caused by micro-latch-up events in the readout circuits or data  buffer since they do not affect the data in the memory cell. This  phenomenon reminds the researchers that it is risky to focus  only on the stable upsets when evaluating the sensitivity of  COTS FRAMs to high-energy particles. It is necessary to pay  attention to the disturbances during irradiation since they may  also lead to serious reliability issues.

## A CKNOWLEDGMENT 

This work was supported by the National Natural Science  Foundation of China (Grant No. 11775167). The authors would  like to thank Dr. Rong-Mei Chen of Tsinghua University for the  help in heavy ion experiment.

## R EFERENCES 

[1]    T. Eshita, T. Tamura, and Y. Arimoto, “Ferroelectric random access  memory (FRAM) devices,”  in Advances in Non-Volatile Memory and  Storage Technology,  pp. 434-454, 2014.    [2]    H. Ishiwara. “Ferroelectric random access memories,”  J. Nanosci.  Nanotechnol.  Vol. 12, pp. 7619–7627, October 2012.    [3]    Z. Wang, W. Jiang, S.X. Li, and J.S. Tong, “Effects of  60 Co γ-ray  irradiation on microstructure and ferroelectric properties of   $\mathrm{Bi}_{3.25}\mathrm{La}_{0.75}\mathrm{Ti}$     $_3\mathrm{O}_{12}$   thin films,”   Nucl. Instr. Meth. Phys. Res. B  vol.366, pp. 1-5, January  2016.    [4]    Q. Shi, Y. Ma, Y. Li, and Y. Zhou, “Drastic reduction of leakage current  in ferroelectric  $\mathrm{Bi}_{3.15}\mathrm{Ad}_{0.85}\mathrm{Ti}_{3}\mathrm{O}_{12}$   films by ionizing radiation,”  Nucl. Instr.  Meth. Phys. Res. B,  vol. 269, pp. 452-454, February 2011.    [5]    R. Bittner, K. Humer, H.W. Weber, M. Tyunina, L. Cakare, A. Sternelerg,  D.V. Kulikov, and Y.V. Trushin, “Dielectric properties of reactor  irradiated ferroelectric thin films,” Integr. Ferroelectr. Vol. 37, pp.  275-283, January 2001.    [6]    J.R. Schwank, R.D. Nasby, S.L. Miller, M.S. Rodgers, and P.V.  Dressendorfer, “Total-dose radiation-induced degradation of thin film  ferroelectric capacitors,”  IEEE Trans. Nucl. Sci.,  vol. 37, pp. 1703–1712,  December 1990.    [7]    B. Angadi, P. Victor, V.M. Jali, M.T. Lagare, R. Kumar, and S.B.  Krupanidhi, “High energy Li ion irradiation effects in ferroelectric PZT  and SBT thin films,”  Thin Solid Films,  vol. 434, pp. 40-48,  June 2003.    [8]    T. Nuns, S. Duzellier, J. Bertrand, G. Hubert, V. Pouget, F. Darracq, J.P.  David, and S. Soonckindt, “Evaluation of recent technologies of  nonvolatile RAM,”  IEEE Trans. Nucl. Sci.,  vol. 55, pp. 1982-1991,  September 2009.    [9]    Z. Zhang, Z. Lei, Z. Yang, X. Wang, B. Wang, J. Liu, Y. En, H. Chen, and  B. Li, “Single event effects in COTS ferroelectric RAM technologies, “  in  Radiation Effects Data Workshop (REDW),  pp. 1-5, December 2015.    [10]   V. Gupta, A. Bosser, G. Tsiligiannis, A. Zadeh, A. Javanainen, A.  Virtanen, H. Puchner, F. Saigne, F. Wrobel, and L. Dilillo, “Heavy-ion  radiation impact on a 4 Mb FRAM under different test modes and  conditions,”  IEEE Trans. Nucl. Sci.,  vol. 63, pp. 2010–2015, August  2016.     [11]   A.L. Bosser, V. Gupta, A. Javanainen, G. Tsiligiannis,  S.D.  LaLumondiere, D. Brewe, V. Ferlet-Cavrois, H. Puchner, H. Kettunen, T.  Gil, F. Wrobel, F. Saigné, A. Virtanen, and L. Dilillo, “Single-event  effects in the peripheral circuitry of a commercial ferroelectric  random-access memory,”  IEEE Trans. Nucl. Sci.,  vol. 65, pp. 1708-1714,  August 2018.    [12]   C. Inguimbert, R. Ecoffet, and D. Falguère, “Electron Induced SEUs:  Microdosimetry in Nanometric Volumes,”   IEEE Trans. Nucl. Sci.,  vol.  62, pp. 2846-2852, December 2015.    [13]   A.A. Ju, H.X. Guo, F.Q. Zhang, W.X. Guo, X.P. Ouyang, J.N. Wei, Y.H.  Luo, X.L. Zhong, B. Li, and L. Qin, “Experimental study about single  event functional interrupt of ferroelectric random access memory induced  by 30-90 MeV proton,”  Acta Phys. Sin.,  vol. 67, pp. 237803,  December  2018.    [14]   G. Tsiligiannis, L. Dilillo, A. Bosio, P. Girard, S. Pravossoudovitch, A.  Todri, A. Virazel, H. Puchner, C. Frost, F. Wrobel, and F. Saigné,  “Multiple cell upset classification in commercial SRAMs,”  IEEE Trans.  Nucl. Sci.,  vol. 61, pp. 1747-1754, August 2014.

