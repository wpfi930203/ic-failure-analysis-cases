---
title: "286_Paper.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_758c42ec901a63719c41e04820baf51f7295230462135641
file_size: 329447
---

## Failure Analysis of the Effect of Hydrogen on  GaAs Device  

Chao Duan, Zhimin Ding, Zhaoxi Wu, Xiaoqing Wang, Chao Li, Xu Wang  1 Center of Failure Analysis Affiliation, China Academy of Space Technology, Beijing, China.  \* Phone: +86-135-817-36381   Fax: +86-10-6874-6312   Email:  super_duan@126.com

Abstract —In this paper, we analyzed the reduction of the  signal-to-noise ratio of the signal received by the system caused  by the failure of a GaAs device. By the means of fault tree, it  can be concluded that the failure is in that the operating point  of the GaAs device was not selected at the appropriate gate  voltage bias position, and at the same time the device gain  decreased under the hydrogen effect. Finally, it led to the  systematic function failure. A large number of contrast tests  concerning the failure components and the samples were  designed and implemented during the analysis. The suitable  working bias voltage was determined. The degradation impact  caused by the hydrogen effect on the GaAs device performance  was analyzed. It provides reference for controlling the failure  mode of the device during its subsequent production and  application.

Keywords-GaAs;Failure; Hydrogen Effect

## I.      I NTRODUCTION  

The GaAs is an important semiconductor material. It is of  high electron mobility and therefore is widely applied to the  field of wireless communication in high-frequency machines,  such as microwave devices and high-speed digital circuits.  The semiconductor devices made of the GaAs shows good  performances in high frequency and under high and low  temperatures; they also produce low noise and high radiation  resistance. With the wide application of GaAs devices, their  failure problems grow more and more complex. Some new  failure mechanisms have also emerged, i.e., the hydrogen  effect. That is to say, the hydrogen may slowly leak out from  the   encapsulating   material,   degenerating   devices’  performance and affecting their normal function.

By constructing a fault tree, this paper analyzed the  maximum possible event for the failure of the malfunction  component and localized the fault point with high efficiency  and accuracy. The cause of failure of the component was  demonstrated through tests and its mechanism was analyzed.

## II.    P ROBLEM  O VERVIEW 

The signal-to-noise ratio of the signal received by a  module decreased; the losing lock is widely appeared in  signals. The fault is positioned at the final radio frequency  amplifier through troubleshooting. In order to further  determine the cause of the fault, the fault tree method was  then adopted to analyze and troubleshoot the possible cause  of the gain reduction of the final radio frequency amplifier.

![Final Radio Frequency Amplifier Failure  Final Radio Frequency Amplifier Failure Using Problem  Using Problem X1:The  X1:The  Problem  Problem  inside the Device  inside the Device Electrical  Electrical   Environment  Environment  X2:Difference  X2:Difference   Overstress  Overstress  Problems  Problems from Operating  from Operating  Point Selection  Point Selection X3:se1f-  X3:selfexcitation of  excitation of  the amplifier  the amplifier X4-2:  X4-2: X4-1:  X4-1: Hydrogen  Hydrogen  Moisture  Moisture Effects  Effects ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/bdf487c4-2693-40e1-af72-6d86a8a548a6/bdf487c4-2693-40e1-af72-6d86a8a548a6.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215688%3B1743219288&q-key-time=1743215688%3B1743219288&q-header-list=host&q-url-param-list=&q-signature=1ab7f0cfc2ef961e4c41f799cac83d07be1852a0)
Figure 1.    Fault Tree for Abnormal Module

## A.    X1 - The Problem inside the Device  

•    A total of 50 devices from the same batch were  selected, from which 10 devices were selected for  tests of temperature cycling, constant acceleration,  steady-state life   $(175\,^{\circ}\mathrm{C}$  ,   $\mathrm{{Idd}=250m A}$  ,   $\mathrm{V}\mathrm{d}\mathrm{d}{=}\ \mathrm{V}\mathrm{d}\mathrm{d}{=}$    5V, 1000h), high and low temperature, SEM and  bonding strength, shear force, etc. and no failure was  observed among all the 10 devices.  •    The focused ion beam (FIB) test and the scanning  electron microscope (SEM) test were respectively  carried out on the failure components and the normal  chips from the same batch. Ti, Pt and Au of the  metal system had a thickness of   $404\mathrm{nm}$   (for failure  components) and   $402\mathrm{nm}$   (for samples), respectively.  The test results were normal. The results are shown  in Figure 2 & 3.

![rSTt  SgAm   Date29Dec2D16  WD-39mm   Mag\*3571Kx   212  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/55d98466-b2f5-4ced-bd5a-bae5d6a2b631/55d98466-b2f5-4ced-bd5a-bae5d6a2b631.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215688%3B1743219288&q-key-time=1743215688%3B1743219288&q-header-list=host&q-url-param-list=&q-signature=b8f4ec836a84160aa58cc09d0d3eb708eca29eb4)
Figure 2.    FIB Results of Failure Components

![20   EHT=5.00WV   SgniA=Lems   Date:29Dec2016  WD=3.5mm   Mag-35.00Kx   Time:54:26:33  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/d3d9db7d-1ca9-4e10-b7b9-cc73b7bbe3d3/d3d9db7d-1ca9-4e10-b7b9-cc73b7bbe3d3.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215688%3B1743219288&q-key-time=1743215688%3B1743219288&q-header-list=host&q-url-param-list=&q-signature=8e1b06680f36ffd1ac79fde37590c0aa5f7f64a9)
Figure 3.    FIB Results of Samples

•    Another 5 samples were reassembled and subject to  the dynamical aging (input -12dBm, -0.8V,   $+5\mathrm{V}$  ,  125) for 26 hours together with samples having  been subject to static aging (125, 1000h). No  significant change in gain was observed among 7  chips. After those tests, the gate voltage of the  above-mentioned 7 samples was adjusted to -1.2V.  The remaining testing conditions were unchanged.  After 115 hours of dynamic aging, 7 chips showed  no significant change in gain.

Base on above, the assumption that the problem inside the  chip may cause the device failure was ruled out due to the  analysis of the chip quality assurance process, the FIB test  results, the aging test results of chips from the same batch  and the chips subject to the evaluation.

## B.    X2 - Difference from Operating Point Selection   

In the actual circuit design, the set DC operating point is  about   $150\mathrm{mA}$   (the gate voltage was -1.2V.) and the grid  voltage deviation data of the failure components tested are  shown in the figure below.

![samples  failure components  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/713a24a6-2a3d-49a8-9343-00438f8d46fc/713a24a6-2a3d-49a8-9343-00438f8d46fc.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215688%3B1743219288&q-key-time=1743215688%3B1743219288&q-header-list=host&q-url-param-list=&q-signature=4c9e96e2e8eded7fe9c7bb83d9626413e6424fbe)
Figure 4.    Test Diagram for Gain Contrast Energized & Gate Voltage  (Samples vs Failure Components)

In the image, the three curves represented:  Blue: sample test curve  Orange: the first time test of failure module curve  Green: after  $85\,^{\circ}\mathrm{C}$  , 48h, failure module curve

The gate voltage bias during the first test for failure  components was -1.2V, which decreased by 13.28dB when  comparing with the gains of samples. However, after the test,  when the gate voltage bias of the failure component was set  to be -0.8V, its gain decreased by 2.74dB when comparing  with the gains of samples. After the aging for 48 hours under   $85\mathrm{^\circC},$   the gain under 1.2V of gate voltage decreased by  21.72dB and the gain under the 0.8 V of gate voltage  decreased by 3.43dB.

Before and after the aging test, when the gate voltage  bias of the failure components was -1.2V, the changes in  gain fluctuated dramatically; when the gate voltage bias was  -0.8 V, the gain remained almost unchanged. The above  testing data show that the changes in gain vary with the  operating points of the gate voltage. However, the gain  changes of the gate voltage (-1.2V) selected in the actual  circuit design were more dramatical than that of the gate  voltage (-0.8V) after the fault occurs. Therefore, the reason  cannot be ruled out that the difference in operating point  selection has caused the component failure.

## C.    X3 - The self-excitation of the amplifier causes a  decreased stability in cascade.  

The output end of the failure module is directly  connected to the filter. If the filter is abnormal, it may cause  damage to the final amplifier inside the module. Therefore,  the stability of the failure module and of the filter after  cascade was analyzed.

•    The standing wave deflection test and the antimismatching test were carried out on normal  components and there was no self-excitation after  those tests.

The standing wave deflection test and the antimismatching test were carried out on normal module  to verify the module stability.

The test conducted the current and the spectrum  monitoring for standing waves of 2:1, 3:1, 4:1, 5:1  and 10:1, respectively. During the test, the working  current was stable, no self-excitation signal was

observed by the spectrometer and the module was in  normal operation.

•    The high temperature baking test without electricity  was conducted to rule out the external electric stress.

The high temperature baking test without  electricity was carried out on the modules with the  same model but different batches under   $125\,\sqsupset$   and   $150\perp$   for 48 hours, respectively. Then, the testing  results of those modules showed that the gain  decreased by about 16dB under the -1.2V of gate  voltage and the gain decreases by 2.7dB under -0.8V  of gate voltage. The external electric stress then  could be ruled out.

Based on the above analysis, the possibility could  be ruled out that the reduction of the cascade  stability was caused by a self-excited amplifier.

## D.    X4 - External Environment - Moisture & Hydrogen  Effects  

A gas composition was conducted on failure components.  The content of moisture was  $4.84\%$  , which met the standard.  The content of hydrogen was   $1.7\%$  . A hydrogen effect will  cause the threshold voltage drift and the leakage current drop  of GaAs PHEMT devices.

The failure module had not been dehydrogenated during  tube and shell processing. In order to verify the effect of  hydrogen on the module, five contrast tests were conducted,  as shown in table 1.

TABLE I.     F IVE  C ONTRAST  T ESTS ON  H YDROGEN  E FFECT

|Serial Number|Testing Items|Testing Conditions|TestingData|Testing Conclusions|
|---|---|---|---|---|
||        Dynamic Aging                Failure Components      |        Dynamic Aging under 85 °C and.                1.2 V of Gate Voltage for 48h      |The gain slowly decreases by 8.7dB.|        Prove that the gain decrease occurs when the                module is im sealing state. tlthe internal                atmosphere of the cuting module is related to                the gain change and the gain will not continue                decreasing when the cap is removed.      |
||        Dynamic Aging                Failure Components      |        The cap was femoved to conduct                atmosphere analysis.      |        The content of vapor in the module was 4.84%                (it was required to be less than 0.5%) and the                content of hydrogen was 1.7%.      |        Prove that the gain decrease occurs when the                module is im sealing state. tlthe internal                atmosphere of the cuting module is related to                the gain change and the gain will not continue                decreasing when the cap is removed.      |
||        Dynamic Aging                Failure Components      |        Dynamical Aging under +85 °C and                -1.2 V of Gate Voltage for 48h with                a Removed Cap      |There was no significant change in gain.|        Prove that the gain decrease occurs when the                module is im sealing state. tlthe internal                atmosphere of the cuting module is related to                the gain change and the gain will not continue                decreasing when the cap is removed.      |
||        5 chips from the same                batch and 2 chips tested                wele   adopted  fo1                assembly test.      |        Dynamic Aging under +125°C and                10.8V of Gate Voltage for 26h      |        All 7 chips experienced significant changes in                gain.      |        Prove that no gain decrease would occur under                0.8 V and -1.2 V of gate voltage in unsealed                state.      |
||        5 chips from the same                batch and 2 chips tested                wele   adopted  fo1                assembly test.      |        Dynamic Aging under +125°C and                1.2V of Gate Voltage for 115h      |        All 7 chips experienced significant changes in                gain.      |        Prove that no gain decrease would occur under                0.8 V and -1.2 V of gate voltage in unsealed                state.      |
||        Verification Tests for                Modules from Different                Batches      |        Dynamic Aging under +125°C and -                1.2V of Gate Voltage for 8h      |        The gain began to decrease by 5dB since the                thirteenth hour.      |        Prove that no gain decrease would occur under -                0.8 V and -1.2 V of gate voltage in sealed state.      |
||        Verification Tests for                Modules from Different                Batches      |        Dynamic Aging under +125-C and -                0.8 V of Gate Voltage for 60h      |        The gain decreased by 1dB slowiy under 0.8 V                of gate voltage within 23h and then it remained                stabie.      |        Prove that no gain decrease would occur under -                0.8 V and -1.2 V of gate voltage in sealed state.      |
||        Verification Tests for                Modules from Different                Batches      |        Dynamic Aging under +125°C and.                1.2V of Gate Voltage for 20h      |        The gain remained stable. There was                decrease of 23dB versus the iniial stage of the                test; there was a difference of 33dB versus a                operating condition of-0.8 V of gate voltage.      |        Prove that no gain decrease would occur under -                0.8 V and -1.2 V of gate voltage in sealed state.      |
||        Verification Tests for High Temperature Baking without                Modules from Different Electricity under 150°C for 48h                Batches      |        High Temperature Baking without                Electricity under 125 °℃ for 48h      |        tNo significant change was observed in gain                after baking.      |        Prove that the gain decrease in sealing state was                irrlevant to the electricity but the hydrogen in                the module is relevant to the gain change while                the vapor is irrlevant to the gain change.      |
||        Verification Tests for High Temperature Baking without                Modules from Different Electricity under 150°C for 48h                Batches      |        Verification Tests for High Temperature Baking without                Modules from Different Electricity under 150°C for 48h      |        The gain decreased after baking. The gain                decreased by 2.7dB under the -1 under the -1.2                V of and -0.8 V of the testing gate voltage.                respectively.      |        Prove that the gain decrease in sealing state was                irrlevant to the electricity but the hydrogen in                the module is relevant to the gain change while                the vapor is irrlevant to the gain change.      |
||        Verification Tests for High Temperature Baking without                Modules from Different Electricity under 150°C for 48h                Batches      |        The cap was removed to conduct                atmosphere analysis.      |        The hydrogen content in the module was                2.52% and the vapor content im the module                was 2.03%, respectively.      |        Prove that the gain decrease in sealing state was                irrlevant to the electricity but the hydrogen in                the module is relevant to the gain change while                the vapor is irrlevant to the gain change.      |
||        1 Chip from Samples                 Iodule Chip  fom                Different Batches      |        The   sub-threshold   swimgT                characteristics of the chip were                (S factor indicates if there is an                interface state.)      |        The peak value of S parameter of the chipProve that the interface state was generated due                inside the module increases to 3.75 times than to the hydrogen effect of the module chip.                that of the normal chip and the interface statewhich eventually leads to degradation of device                imcreases.      |        The peak value of S parameter of the chipProve that the interface state was generated due                inside the module increases to 3.75 times than to the hydrogen effect of the module chip.                that of the normal chip and the interface statewhich eventually leads to degradation of device                parameters.      |


Through the contrasting analysis of the above tests, the  gains of the module under different gate voltage biases  experience no obvious change in the unsealed state and the  gain decreases when the module (the hydrogen content is  more than   $1.7\%$  ) is in the sealed state. Through the  contrasting test on sub-threshold swing characteristics, it can  be found that the interface state increases and therefore the  possibility cannot be ruled out that the module failure is  caused by hydrogen effect.

After the above troubleshooting, the analysis shows that  the problem of the module’s reduced signal-to-noise ratio  lies in that the device operating point was not selected at the  appropriate gate voltage, and at the same time, the gain  decreases under the hydrogen effect, which eventually leads  to the module’s malfunction.

## IV.    M ECHANISM ANALYSIS ON HYDROGEN EFFECT 

In general, the failure of electronic components can be  divided into fatal and non-fatal. The fatal failure is to  completely disable a device while the non-fatal failure leads  a device to degraded parameters and confined performance.  The hydrogen effect refers to the degradation effect on GaAs  device performance induced by hydrogen, which belongs to  non-fatal failure.

The existence of hydrogen effect has been confirmed. It has  been shown by tests that Si is inhibited when it is mixed with  GaAs and exposed to an ionic environment like hydrogen.  Infrared scanning data has also confirmed the existence of  (SiAs3) As-H complex [1] . a degradation of DC and RF  parameters occurs in PHEMT devices tested in sealed  encapsulation environment or hydrogen environment. The

fundamental reason for the degradation is the hydrogen  released from encapsulating material such as Kovar alloy  and electroplated metal  [2-3] .

The exact reason for device degradation caused by  hydrogen remains unknown and is being researched. At  present, two representative theories have been proposed. One  theory is that the hydrogen reduces the number of carriers in  the device channel. This theory suggests that the hydrogen is  dissociated into atomic hydrogen in the Pt layer due to Pt  catalysis; then, the atomic hydrogen diffuses into the device  channel and forms Si-H which further inhibits the donor  impurity Si in the channel; the inhibition of the donor will  reduce the concentration of the channel carrier, thus reducing  drain current, transconductance and gain [4] . For example,  when the non-encapsulated GaAs FET is exposed to   $100\%$    hydrogen environment and the temperature is set to be   $150\perp$    for 4 hours (which is referred to as “standard hydrogen  exposure”),   the   transconductance   will   experience   a  significant attenuation as shown in figure 6  [5] .

![after  Before  2D  -0.S   -1S   2S  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/331e4bda-dfb2-4316-9044-c3f082adea56/331e4bda-dfb2-4316-9044-c3f082adea56.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215688%3B1743219288&q-key-time=1743215688%3B1743219288&q-header-list=host&q-url-param-list=&q-signature=81053c61aa535fc2ed90aa95410d5702fd964c68)
Figure 5.    Degradation of Device Energized by DC after Hydrogen  Exposure

Another theory is that the hydrogen affects the self-built  potential removed by Schottky. According to this theory, the  principle that the effect of the hydrogen on the inter-phase  characteristics is that the atomic hydrogen’s entrance into the  interface between the metal gate and the semiconductor will  affect the interface state and then change the self-built  potential removed by the metal gate and the semiconductor.   [6]

There are still no effective preventive measures against  hydrogen effect now. Therefore, metals that do not react with  hydrogen can be adopted as the gate material to deal with the  hydrogen effect on metal in GaAs devices, such as gate  materials containing no Pt, Ti, or Pt/Ti structures.

## V.    C ONCLUSION 

Through the above analysis on failure cases and the study  on test results, it is confirmed that the device failure is due to  the improper selection of bias voltage at the operating point,  causing a decreased signal-to-noise ratio in the system under  the hydrogen effect.

The   hydrogen   leaking   from   the   sealed   metal  encapsulation will affect the gas composition inside the  device, which has a severely harmful impact on the devices,  especially the GaAs devices. The hydrogen slowly leaking  out from the encapsulating material can react with the gate

metal of the device and lead to the drift of threshold voltage.  The hydrogen may also affect the internal and interface state  of the semiconductor and degrade the device’s electrical  performance. The slow but continuous release of hydrogen in  metal materials will affect the long-term reliability of  components. Therefore, such phenomena shall be given  special attentions and be prevented from happening during  device research and manufacturing.

The current microwave semiconductor device commonly  used metal ceramic package, hydrogen release from the  metal casing or the surface coating. To ensure the reliability  of the device used, we make the following recommendations.

For metal package at least 24 hours of high temperature  baking at  $200\,^{\circ}\mathrm{C}$   was needed, in order to promote the release  of internal hydrogen. Because of the sensitivity of the device  on the hydrogen effect is determined by the device structure  and process, the sensitive level of hydrogen effect of device  should to evaluated. By means of both, can effectively  reduce the hydrogen effect when microwave GaAs devices  were used.

## A CKNOWLEDGMENT 

First of all, I would like to extend my sincere gratitude to  my dear colleague, Ms. Zhimin Ding, for her instructive  advice and useful suggestions on this paper. I am deeply  grateful of her help in the completion of this paper.   High tribute shall be paid to Mr. Zhaoxi Wu, who has helped  me a lot in this failure analysis.

Last my thanks would go to my lovely family for their  great confidence in me. I also owe my sincere gratitude to  my friends who gave me help and time in listening to me and  helping work out my problems during the difficult point  during the failure analysis.

## R EFERENCES 

[1]    JALIL A, CHEVALLIER J, PESANT J, et al. Infrared Sepctroscopic  Ebidence of Silicon Related Hydrogen Complexes in Hydrogenated  n-Type   GaAs   Doped   with   Silicon[J].   Appl.   Phys.   Lett,  1987,50(8):439.    [2]    LIU Shanghe, WEI Guanghui, LIU Zhicheng, et al. Electrostatic  theory and protection[M]. Beijing, China: Weapons Industry Press,  1999:22-24.    [3]    Zhenyu Zhu. The harm of ESD to microwave module and its  protection.[A] Reliability and Environmental Test of Electronic  Products, 2013,31(3):19-24.    [4]    YANG Jie, LIU Shanghe, YUAN Qingyun, et al . Square-wave EMP  damage of microwave low-noise silicon transistors[J] High Voltage  Engineering, 2007, 33(7):111-114.    [5]    Baohua Shi, Xinzhang Jia, Desheng Zhang. Reliability of  Microelectronic Devices[M].Xi’an: Xidian University Press,1999.    [6]    EVELOY V, HWANG Y C, PECHT M G. The effect of electrostatic  discharge on electrical overstress susceptibility in a gallium arsenide  MESFET-based device[J].IEEE Transactions on Device and  Materials Reliability, 2007,7(1):200-208.

[7]    G. Eason, B. Noble, and I. N. Sneddon, “On certain integrals of  Lipschitz-Hankel type involving products of Bessel functions,” Phil.  Trans. Roy. Soc. London, vol. A247, pp. 529–551, April 1955.  (references)

[8]    J. Clerk Maxwell, A Treatise on Electricity and Magnetism, 3rd ed.,  vol. 2. Oxford: Clarendon, 1892, pp.68–73.    [9]    I. S. Jacobs and C. P. Bean, “Fine particles, thin films and exchange  anisotropy,” in Magnetism, vol. III, G. T. Rado and H. Suhl, Eds.  New York: Academic, 1963, pp. 271–350.    [10]   K. Elissa, “Title of paper if known,” unpublished.    [11]   minutes    [12]   R. Nicole, “Title of paper with only first word capitalized,” J. Name  Stand. Abbrev., in press.    [13]   Y. Yorozu, M. Hirano, K. Oka, and Y. Tagawa, “Electron  spectroscopy studies on magneto-optical media and plastic substrate  interface,” ASME Transl. J. Magn. Japan, vol. 2, pp. 740–741,  August 1987 [Digests 9th Annual Conf. Magnetics Japan, p. 301,  1982].    [14]   M. Young, The Technical Writer’s Handbook. Mill Valley, CA:  University Science, 1989.    [15]   Electronic Publication: Digital Object Identifiers (DOIs):  Article in a journal:    [16]   D. Kornack and P. Rakic, “Cell Proliferation without Neurogenesis in  Adult Primate Neocortex,” Science, vol. 294, Dec. 2001, pp. 2127- 2130, doi:10.1126/science.1065467.  Article in a conference proceedings:    [17]   H. Goto, Y. Hasegawa, and M. Tanaka, “Efficient Scheduling  Focusing on the Duality of MPL Representatives,” Proc. ASME  Symp. Computational Intelligence in Scheduling (SCIS 07), ASME  Press, Dec. 2007, pp. 57-64, doi:10.1109/SCIS.2007.357670.

