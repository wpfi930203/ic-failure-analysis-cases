---
title: "149_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_da52648f0b18da216ae41ed2c2fc83407295230462135641
file_size: 1214172
---

## Logical Data Extraction of a STT-MRAM:  Backside FIB Preparation and ConductiveAFM Measurements  

Louise DUMAS  1, 2, 3 , Guillaume BASCOUL  1 , François MARC  2 , Hélène FREMONT  2 ,   Christina VILLENEUVE-FAURE  3 , Christophe GUERIN  4   1  Laboratoire d’Expertise, Centre National d’Etudes Spatiales (CNES), Toulouse, France  2  IMS Laboratory, University of Bordeaux, UMR 5218, 33405 Talence, France  3  LAPLACE (Laboratoire Plasma et Conversion d’Energie), Université de Toulouse, CNRS, UPS, INPT, Toulouse, France   4  Direction Générale de l’Armement Maîtrise de l’information (DGA MI), Bruz, France  Email: louise.dumas@cnes.fr

Abstract – The reading of the memory state (i.e.,  whether a bit is at   $\mathbf{\cdot0}^{\bullet}$   or ‘1’) on an individual magnetic  tunnel junction (MTJ) in a commercial spin-transfer  torque magnetic random access memory (STT-MRAM) is  still a challenging task. This is mainly due to the nanoscale  size of the memory cell. This paper proposes a probing  approach, based on atomic force microscopy (AFM),  aiming at monitoring the resistance value of the MTJ,  thereby determining its memory state.

To achieve this objective, the 40 nm MRAM device  must undergo preparation to establish electrical access on  both sides of the MTJs. The appropriate methodology,  developed in this paper, involves backside preparation,  creating access to the bottom side of the MTJs through  vias, and to the top side through bitlines primarily using a  focused ion beam (FIB).

Following the MRAM preparation process, the  paper delves into MTJ resistance probing using AFM in a  conductive mode. Consequently, it becomes possible to  measure the current flowing through the MTJs and assess  their resistance. Results emphasize that   $\mathbf{\epsilon}_{\mathbf{0}},$   and ‘1’ bits  exhibit a resistance of   ${\bf8.5+/-~0.1~k\Omega}$   and   $\mathbf{3.9+/-~0.2~k}\Omega$    respectively which is in agreement with literature. This  allows the first reading of a STT-MRAM.

Keywords – MRAM, MTJ memory cell, FIB, AFM,  Methodology

## I.    I NTRODUCTION 

The integrity of data stored in a magnetic random  access memory (MRAM) stands as a critical concern for  electronics manufacturers. Furthermore, regardless of  the application (whether it be for civilian, space, or  military purposes) ensuring the confidentiality of data  remains of utmost importance. Because of those security  considerations, conducting electrical operations on the  data stored in embedded memories is extremely  complex. Usually, to prevent any abnormal activities,  standard memory access is restricted and triggering data  erasure is activated when an unauthorized read operation  occurs. The goal of this paper is to read the data content  without resorting to its electrical access, hence by  bypassing these safety protocols.

One approach to accessing the data involves  exploring the physical properties of the technology to  unveil the data contents. Nanoprobing, conductive

atomic force microscopy (C-AFM) and electron beam  absorbed current (EBAC), are standard techniques  needing destructive preparation, to characterize the  electrical behaviour of real-world devices to precisely  locate defects [1]. These techniques have already been  used on static RAM (SRAM) for a soft fail analysis [2],  [3] and on embedded non-volatile memories (eNVM) to  characterize leakage current in inter-poly dielectric and  to identify the spatial localization of the failure [4]. CAFM has also been used to read emerging NVM such as  resistive RAM (RRAM) [5] but also to read the bit state  of a magnetic tunnel junction (MTJ) nanopillar when a  magnetic field is applied [6].

A methodology to extract logical data has already  been developed on a Toggle MRAM with a high  technology node of 140 nm [7], [8]. In those papers, the  use of a bevel in a backside preparation allows the  application of a DC bias voltage on the bitlines and the  collection of a current on the MTJ. Hence, the two states  are discriminated by their resistance values thanks to the  AFM modes SSRM (scanning spreading resistance  microscopy) and C-AFM, and also with Nanoprobing.

This methodology is adapted in this paper to  investigate a spin-transfer torque MRAM (STTMRAM). This new challenge is related to a smaller  technology node (40 nm) and architectural differences.  In this context, the approach developed in this paper,  proposes a methodology to collect information,  contained at bit-cell level in the MTJ and integrated in  commercial memories, using AFM probing. To reach  this goal, a dedicated backside sample preparation  including a chemical opening, a chemical-mechanical  polishing (CMP) and focused ion beam (FIB) etching  and deposition is developed. Compared to our previous  papers, the addition of the FIB allows a better control of  the etching and so the adaptation of our procedure to  smaller technology nodes.

## II.    STT-MRAM  CONSTRUCTION ANALYSIS   

## A.    MRAM operation  

In a MRAM, the data is stored in the MTJ as  different electrical resistance levels which are created by  different polarization orientations in the magnetic stack.  Indeed, the MTJ stack is magneto-resistive, meaning

1

that its magnetic orientation and resistance can be  modified by a magnetic field or in this case, by a spin  current. The MTJ can be described as in-plane (iMTJ) or  perpendicular (pMTJ) depending on the orientation of  the stored magnetic polarization [9].

For a write operation, the bit value selected by  the word line (WL) is changed by applying a positive  voltage on a bitline (BL) or a source line (SL) [10].  Indeed, when a current goes from the BL to the SL  (purple arrow in Fig. 1), the state ‘0’ switches to ‘1’. On  the other hand, when a current goes from the SL to the  BL (brown arrow in Fig. 1), ‘1’ changes to   $\mathbf{\epsilon}^{\bullet}0^{\bullet}$  .

For a reading operation, the bit value selected by  the WL is read by applying a negative voltage on the BL.  This makes a current go through the MTJ (pink arrow in  Fig. 1) which is then compared to a reference cell thanks  to a current sense amplifier that allows a deduction of  the value of the electrical resistance.

![BipolarGenerator  Reading  Readbias/Writepulse  Current  Sense  IReading   Iwriting \*0"   Amplifier  Iwriting\*1"  S  NTJ   Ref  Bit"O"   Bit‘1”  Access  transistor  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c138d14b-3240-4527-a2de-4da30df82703/c138d14b-3240-4527-a2de-4da30df82703.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215858%3B1743219458&q-key-time=1743215858%3B1743219458&q-header-list=host&q-url-param-list=&q-signature=0529ae9c197d6d673463e645f86adf57f2555d52)
Fig. 1. Schematic of the STT-MRAM memory point with a pMTJ.

## B.    Construction analysis  

The commercial device used for this study is a  Renesas M3004204 memory with a 16Mb capacity. It is  based on a   $40\;\mathrm{\nm}$   pMTJ technology. This MRAM  consists of a chip resting on a leadframe in an organic  thin small outline package (TSOP).

The die is made of 96 memory blocks, as shown  in Fig. 2, where one is circled in pink.

The first step to investigate the Renesas memory  is to identify the localization of the MTJ in the metal  stack and to understand the internal organization. To  reach this goal, the MRAM was analysed in crosssection using two micro sections made in the two  perpendicular directions of the device (i.e. along X- and  Y- directions on Fig. 2). Fig. 3a and Fig. 3b represent a  scanning electron microscope (SEM) image of a MRAM  cross-section. The MTJ was identified under the  metallization levels M1, so quite at the bottom of the  metal stack, in one column over two.

Since the bitlines and source lines are on the  same metallization level (M2), Fig. 3c was established  to show the different planes, made possible thanks to a  delayering analysis. As we can see, the MTJ (present in  the first and third XZ-planes) is connected to a BL  through metal C1 and via D1, and to the access transistor  through via A1. The other side of the transistor is  connected to the source line (in the second plane)  through the vias A2 and B2 (in the first plane), metal C2  (which is a strip, present in the three planes) and via D2  (in the second plane). On the other hand, the WL is  perpendicular to them at the transistor level.

![500pm   3.2mm  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/1b59301a-5465-4044-989a-4c650861cab5/1b59301a-5465-4044-989a-4c650861cab5.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215858%3B1743219458&q-key-time=1743215858%3B1743219458&q-header-list=host&q-url-param-list=&q-signature=3d81cd16462a6e627aea4af00613afdc5d089769)
Fig. 2. SEM image of the entire die, after a backside opening and  silicon removal, showing one memory block (pink rectangle).

![3rdplane   BL  2ndplane   SI  1stplane   8L  VX   2  22   81  MMTJ  D1   D2  2  1   CT   C2  VAE   82  NTJ  1  1m   100nm  C  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a40a2054-4f99-4c7d-bed6-3a9765977390/a40a2054-4f99-4c7d-bed6-3a9765977390.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215858%3B1743219458&q-key-time=1743215858%3B1743219458&q-header-list=host&q-url-param-list=&q-signature=671bd81b810bc03a123b051f9b9aae1f3440bd91)
Fig. 3. SEM image of the cross section of the die showing the localization of the MTJ between M1 and M2 (a.), SEM image of the cross section in the  first plane with the identification of the organization of the die (b.) and Schematic of the different elements across three different planes : first plane in  black connected to a BL, second plane in grey connected to a SL and third plane in brown connected to a BL (c.).

2

Thanks to this identification, it is now possible to  know what critical levels surround the MTJ. Indeed, the  MTJ is located above the transistor and wordline level  (which appearance is shown in the blue rectangle in Fig.  5c) ; the bitlines and source lines metallization level is  located just above a level composed of alternating vias  and lines (which appearance is shown in the red  rectangle in Fig. 5b).

## III.    P REPARATION TECHNIQUE 

## A.    Goal  

The goal of this preparation method is to access  two different levels in the chip (shown as two blue dot  lines in Fig. 4) to be able to probe the current going  through the MTJ. The first access between M1 and M2  will allow the application of a DC bias voltage on the  bitlines while the second access above the transistor will  allow the collection of the current to determine the  resistance value of the MTJ. These steps represent a  challenge as the thickness difference between the two  planes is only 350 nm wide. As such, a bevel made with  polishing is not possible and the two steps will be  created by FIB etching.

Moreover, as the memory block only has a length  of   $85~\ensuremath{\upmu\mathrm{m}}$   in the direction of the bitline (M2), which is  the path used for the current (red arrow in Fig. 4), the  preparation technique must be precise (in depth and  form) as not to damage the path.

## B.    Preparation methodology  

The first step is to uncap the package without  damaging the chip. Nitric acid is used to dissolve the  plastic package and the leadframe, leaving only the chip.  Then, the silicon is polished by CMP from the backside  of the die leaving only a thin silicon layer so that it is  see-through. Once the thickness of the remaining layer

of silicon is ranging from 0 to   $5~\ensuremath{\,\upmu\mathrm{m}}$  , the next step  consists in creating an access to the memory block using  FIB editing.

The process to perform this access is illustrated  in Fig.  5 a to c, and follows these five steps:  1) Localization of the memory block by utilizing the  transparency of the silicon (pink rectangle in Fig.  5 a)  2) Determination of the silicon cap thickness thanks to a  cross-section by FIB etching, made on the side of the  memory block (beige-yellow rectangle in Fig.  5 b)  3) Creation of an access to the vias under M2 by FIB  etching (orange rectangle in Fig.  5 b and higher dotted  line in Fig.  4 )  4) Creation of the electrical contact on M1 to apply a DC  bias by depositing two platinum layers by FIB

First deposit for a good electrical contacting of  the vias (green rectangle in Fig.  5 c)       Second deposit to cover a larger area (brown  rectangle in Fig.  5 c)

5) Creation of an access to the vias under the MTJs for  AFM measurements by FIB etching (purple rectangle in  Fig.  5 c and lower dotted line in Fig.  4 )

![2   3L  NI  NTJ   350nm  DCBias  200nm  AFMScan  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/94d4c2e1-0b3c-4a38-a126-aeb3d9e59466/94d4c2e1-0b3c-4a38-a126-aeb3d9e59466.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215858%3B1743219458&q-key-time=1743215858%3B1743219458&q-header-list=host&q-url-param-list=&q-signature=238bf8cd34ffd8ff20da60c024eb8dd65d3894cc)
Fig. 4. SEM image of the cross-section showing the BL (which is  also the metallization level M2), the MTJ and the WL but also the  schematic of the two planes of vias to get access to (blue dot lines)  and the wanted current flow (red arrows) between the two tips (one  applying a DC bias and one collecting a current in C-AFM).

![60mm  1pm  85pm  A1or A2  BLorientation  Boun   5oonm  100pm   10pm   5opm  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/e320a28d-32e2-4a7c-86aa-d07c5f0f5eb8/e320a28d-32e2-4a7c-86aa-d07c5f0f5eb8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215858%3B1743219458&q-key-time=1743215858%3B1743219458&q-header-list=host&q-url-param-list=&q-signature=924abb37081ab2a0686cebe307ca85e6e8150ef0)
Fig. 5. SEM image f the backside of the die showing the memory block (pink rectangle) and orientation of the BL (burgundy arrow) (a.),   SEM image of the backside of the die, after a cross-section (beige-yellow rectangle) and a FIB etching (orange rectangle), showing the vias under the  bitlines and source lines (zoom in red rectangle) (b.)   Optical microscopy image of the finished preparation showing the first platinum deposit (green rectangle), the second deposit (brown rectangle) and  the second etched area of vias under the MTJs (purple rectangle) with a zoom on the vias which will be studied in C-AFM (blue rectangle) (c.).

3

## C.    Preparation notes  

The sample is handled easily through all this  process thanks to the aluminium stub is it glued onto  (with epoxy). It is stored in a nitrogen chamber between  polishing and the FIB editing as none of the area of  interest are exposed. Then between the FIB editing and  the AFM imaging, it is stored in a vacuum chamber as  not to contaminate the exposed vias area.

The second step of the preparation methodology  is not mandatory but allows the validation of the position  of the memory block. Moreover, the silicon thickness  measurement allows the determination of the most  suitable etching speed.

The contact of the bitlines through the platinum  pad allows the application of a DC bias voltage on  several bitlines at a time, here around 300. That way, the  current can be collected on all the exposed vias with the  AFM, without moving the probing tip.

## D.    FIB parameters  

The etching of the silicon layer is done by  imaging (in real time and not by an automated process  with a predetermined duration) at   $30\,\mathrm{keV}$   and 15 nA for  2 minutes. Then, the etching of the metallization layers  is done by imaging at  $30\,\mathrm{keV}$   and either at 4 nA for fast  etching or at 1 nA for slow etching. This etching process  stops when the vias, which are just under the bitlines and  source lines, are reached as shown in the red rectangle  in Fig. 5b. This image over the vias area highlights that  the sample is perfectly clean and suitable for creating  reliable electrical contact.

This was done by depositing a platinum layer by  FIB in two steps: a first deposit with low current (8 keV   $-\,0.62\;\mathrm{nA})$  ) on the exposed vias  (green rectangle in Fig.  6) and then a larger deposit (brown rectangle in Fig. 5c)  at a higher current   $(8\;\mathrm{keV}-2\;\mathrm{nA})$   on top of it to ensure  an easy contacting of the tip. This second deposit usually  spreads some platinum on the neighbouring area of the  deposit but this does not present a problem for our  preparation since the area of interest (i.e. the vias just  under the MTJs) is still protected by the silicon layer.

The second etching process reveals an area of  vias under the MTJ (blue rectangle in Fig. 5c) that is also  perfectly clean. That is why the sample is stored in high  vacuum conditions before AFM probing.

## IV.    C ONDUCTIVE -AFM  

## A.    Set-up  

Near-field probe measurements were performed  on an AFM (Bruker ICON) setup. The MRAM memory  block of   $85\;\upmu\mathrm{m}$   width with randomly distributed   $\mathbf{\epsilon}^{\bullet}0^{\bullet}$   and  ‘1’ bits is used but the area to be investigated by the  AFM is reduced to   $15~\ensuremath{\upmu\mathrm{m}}$   width over   $60~\ensuremath{\upmu\mathrm{m}}$   (purple  rectangle in Fig. 5c).

The C-AFM setup applies a DC bias voltage  between two tips : a probing tip (left tip in Fig. 6 and in

Fig. 7) which applies a DC bias voltage on the platinum  FIB pad, while the AFM tip  (right tip in Fig. 6 and in  Fig. 7) scans the surface and collects the current on the  vias plane. With this setup, the current goes through the  BL, an MTJ (or a via in one row over two), and a via  before being collected. For this measurement, a silicon  tip with a doped diamond coating (DDESP-V2 from  Bruker) is used and the current is collected in C-AFM  mode (contact force of   $1.1~\upmu\mathrm{N}$  ).

![Current   AFMController  Amplifier  TipSignal  ProbingTip   AFMTip  DCBiasVoltage  FIBPad   via  SampleHolder   MRAM  SampleStage  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/9ca481a8-d4f2-4b10-ba05-2882ff4a1706/9ca481a8-d4f2-4b10-ba05-2882ff4a1706.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215858%3B1743219458&q-key-time=1743215858%3B1743219458&q-header-list=host&q-url-param-list=&q-signature=0696f76c2e5c65d4dbd41f2a491d27d7fdd54bf0)
Fig. 6. Schematic view of the setup for the C-AFM experiment.

The contact between the probing tip and the  surface was made manually with the optical binocular of  the AFM as shown in Fig. 7. This comes as a challenge  since the two tips are in the same vicinity (separated by  less than   $100\;\upmu\mathrm{m})$  ).

![AFMTip  100pm  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/200a5328-f03b-4984-82fb-0029e55f8a18/200a5328-f03b-4984-82fb-0029e55f8a18.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215858%3B1743219458&q-key-time=1743215858%3B1743219458&q-header-list=host&q-url-param-list=&q-signature=060bae21239bcd4674408ae340c7f80991ac1f8e)
Fig. 7. Optical view of the AFM showing the close distance between  the two tips.

## B.    Experiment  

Fig. 8 compares surface topography (Fig. 8a) and  current cartography (Fig. 8b) probed in C-AFM when 4  mV is applied by a probing tip on the FIB pad.

In Fig. 8a, the vias are identified as bright spots.  Fig.  8 b highlights that the current is not uniform on the  surface. Indeed, no current is collected on insulating  parts between vias while a current, saturating the  amplifier, is collected on vias that are not over a MTJ  (one row over two). This can be explained by the fact  that those vias are directly connected to the applied  voltage through the source line, which is short-circuited  by the FIB pad along with the bitlines.

4

![1.2μm   NTJ   vias  Section  Profile  1.1μm   OnA  600nA  1.16μm   400nA  1.15μm  200nA  1.14μm   OnA  Om   a.Topography   2m   Om   b.Current   2m  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/deecf0ad-c166-4307-8dd6-188ac9a838b0/deecf0ad-c166-4307-8dd6-188ac9a838b0.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215858%3B1743219458&q-key-time=1743215858%3B1743219458&q-header-list=host&q-url-param-list=&q-signature=444a67fc3994839efa0653b4fbc7228341a15d41)
Fig. 8. C-AFM topography (a.) and current (b.) map obtained by applying a polarization of   $4\,\mathrm{mV}$   and a contact force of   $1.1~\upmu\mathrm{N}.$

However, the current collected over a MTJ is not  saturating, showing that a non-negligible resistance was  encountered on the current path. This allows a direct  identification of the bits by imaging: the two states are  discriminated on an image with two current values  (brown around 300 nA or beige around 500 nA).

A separate analysis of a memory programmed  only with   $\mathbf{\epsilon}_{0},$   and another only with ‘1’ was conducted  in parallel of this experiment. Thanks to which, we can  identify the brown vias, which presented a lower current  and so a higher resistance as the bit   $^{\bullet}0^{\bullet}$  . In comparison,  the beige vias, which presented a higher current and so  a lower resistance, are identified as ‘1’.

The two states are discriminated on an image  with two current values, corresponding to two resistance  values:

$$R(0)_{s c a n}=R(h i g h)_{s c a n}=\frac{4\;m V}{300\;n A}=13.3\;k\Omega$$
$$R(1)_{s c a n}=R(l o w)_{s c a n}=\frac{4\:m V}{500\:n A}=8\:k\Omega$$
To improve the accuracy on the MTJ resistance  measurement, forty-one current I versus voltage V (i.e.  I-V) curves are plotted on forty-one vias (Fig. 9) with a  higher contact force and a longer plotting time  (frequency of   $0.1~\mathrm{Hz}$  ). The curves are well separated in  two groups according to the colour of the vias (brown or  beige in Fig.  8 ). Moreover, the current increases linearly  with the applied voltage, which allows us to extract a  MTJ’s resistance from the slope of the curves.

The plateau at higher applied voltage is related to  current sensor saturation. The staircase-shaped slope  indicates that the AFM bias generator is not precise  enough to plot 256 points over   $16\,\mathrm{mV}$  , corresponding to  a  $62.5\;\upmu\mathrm{V}$   step. It is not correlated to the MRAM.

![6.0E-07  3.0E-07  0.0E+00  -8.0E-03   -4.0E-03   0.0E+00   4.0E-03   8.0E-03  -6.0E-07  Voltage(V)  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/80b2b14e-d370-44ca-ab4b-b0a8179cce80/80b2b14e-d370-44ca-ab4b-b0a8179cce80.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215858%3B1743219458&q-key-time=1743215858%3B1743219458&q-header-list=host&q-url-param-list=&q-signature=63968149d9cc3b14a1aacf45e6ee898666d92170)
Fig. 9. Current versus Voltage curves over 41 vias obtained in CAFM by ranging from -8 mV to   $8\;\mathrm{mV}$   at  $0.1\:\mathrm{Hz}$  .

Fig. 10 represents the average I-V curves for each  resistance group for which the saturation part was  excluded. The yellow curve corresponds to the high  resistance value as its current measurement is lower than  the one of the green curve (corresponding to the low  resistance value) at the same voltage value.

5

The resistance values defined by the fitting  curves are:

ܴ(0) ௧

= ܴ(ℎ݅݃ℎ) ௧

= 8.54 ± 0.05 ݇Ω

ܴ(1) ௧

= ܴ(݈ݓ) ௧

= 3.90 ± 0.21 ݇Ω

These values are in agreement with the literature  since a MTJ (on wafer) of this diameter (85 nm) is  supposed to have resistance values between   $8\textrm{-}12\ \mathrm{k}\Omega$    (for a 80 nm MTJ) and   $4\textrm{-}6\ \mathrm{k}\Omega$   (for a 100 nm MTJ)  [11].

![6.0E-07  y=2.6\*10-4x-1.4\*10-8  3.0E-07  y=1.2\*104x-8.6\*10-9  0.0E+00  -2.0E-03   -1.0E-03   0.DE+00   1.0E-03   2.0E-03  -3.0E-07  R(high)  R(low)  -6.0E-07  Voltage(V)  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b3715395-faf0-4422-b2d1-62f55491e159/b3715395-faf0-4422-b2d1-62f55491e159.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215858%3B1743219458&q-key-time=1743215858%3B1743219458&q-header-list=host&q-url-param-list=&q-signature=3a9e459b6988e8386d35180d290f0172e78cefcb)
Fig. 10. Mean I-V curves of the two states, based on the previous 41  I-V curves, with their fitting curves and equations.

The parameters used for this study (memory,  AFM and output) can be found in the Annex (Fig. 11).

## V.    D ISCUSSION 

The AFM tip has a high tip radius (around 100  nm) so it was not our first choice resolution-wise since  the vias are 90 nm-wide. The silicon tip with a platinum  coating (SCM-PtSi from Bruker) had a lower curvature  tip radius (25 nm) but collected the current poorly in the  long run, probably due to a coating wear out. Hence, the  diamond tip was chosen to get the best current collecting  measurement compared to the best topography image,  which is still sufficient.

It is possible to notice that some dots are present  next to the vias at the top right of the image (topography  and current map). Theses dots and vias broadening on  the current map could be related either to a convolution  phenomenon linked to AFM tip with large curvature  radius, or to the impact of a previous scan with the AFM  tip that damages the surface and mostly enlarges the  vias.

C-AFM is an effective way to probe a current  trough an MTJ. The probing of the vias is easy thanks to  the automated descent. Moreover, the control of the  contact force and the minimization of the tip  deterioration makes C-AFM the ideal choice of probing.  However, it is quite difficult to add another probe next  to the AFM tip due to the size of the tip holder.

Moreover, the AFM technique is timeconsuming so it is hard to imagine applying it on the  whole array. Since this technology is quite small, the  size of the scan can go up to   $5~\mathrm{~\textmu m}$  while still  distinguishing both resistance values; that covers around  360 bits at a time. So, for only one memory block, it  would take a couple of days to connect all the bitlines  with FIB etching and deposition. Moreover, it is not  possible to automate the process mainly for the FIB  etching, as the imaging time to etch the silicon depends  on the silicon layer that is left from polishing. I do not  consider it possible unless a perfect polishing planarity  is obtained.  Then it would take a day or two to expose  the vias just under the MTJ. It is noteworthy that with  this technique not every data can be recovered as some  is lost in the connection of the bitlines. It would be  possible to expose an area of   $50\,\upmu\mathrm{m}$   width over  $430\;\upmu\mathrm{m}$  ,  the length of a memory block, which amounts to about  300 000 bits. Finally, the AFM scan of all the exposed  vias is what would take the longest time, probably  around two weeks or more, plus the time to analyse the  data.

The Fast-scan mode was developed by Bruker on  the AFM Icon to schedule the scanning of different areas  beforehand and to save images as they are acquired  (around an image by minute). This mode has not been  tested here to map the memory block, as we do not have  it, but it could theoretically be suitable for such an  electrical analysis.

The only unfixable issue is the stepping of the  bias generator. A replacement by a source measurement  unit (SMU) was tried unsuccessfully as the tip and the  sample need to be connected on the same ground value.

## VI.    C ONCLUSION 

Results reported in this study demonstrated the  possibility to probe a current flowing through the MTJs  of a commercial 40 nm STT-MRAM with probing-AFM  with the final goal of being able to read them (i.e. to  discriminate a “0” from a “1”). A resistance of around 4   $-\textsl{8}\,\mathrm{k}\Omega$   for the two states is obtained for the entire  electrical path composed by FIB pad, BL, MTJ and vias.

These values, comparable to those reported in the  literature, and their difference (i.e. few kΩ) demonstrate  that the two states can be discriminated thanks to the  resistance. Hence, it is possible to extract the logical  content of a STT MRAM with a thorough methodology  and an AFM.

This work has its limitations. It cannot be applied  to the whole array with the standard AFM mode as it  time-consuming and not automatable. Hence, the data is  read locally and as we know, the logical address of a bit  is not its physical one. A future work will be to do the  descrambling of this MRAM, firstly to be sure that what  we read is what is written, and secondly to read data and  not only independent bits.

6

## A CKNOWLEDGMENTS 

This work is funded by a grant of the French  Innovation Defence Lab and the French space agency  (CNES).

## A NNEX   

Fig. 11. Table summarizing the parameters of the studied memory, of  the AFM experiment and of the output.

|Parameters|Parameters|Parameters|
|---|---|---|
|Memory|Type|MRAM|
|Memory|Capacity|16Mb|
|Memory|Technology node|40nm|
|AFN|Probe|        Silicon tip with a                doped-diamond coating      |
|AFN|Voltage|4mv|
|AFN|Contact force|1.1 μN|
|Output|        Content                demonstrated      |4Hm²|
|Output| Possible scan area|25μm²|
|Output|Speed|8 minutes / scan|


## R EFERENCES 

[1]   L. Tian  et al. , “The Application of Advanced Nano-Techniques  in Failure Analysis for Different Failure Mechanism,” in  International Symposium on the Physical and Failure Analysis  of   Integrated   Circuits   (IPFA) ,   2018,   pp.   1–5.   doi:  10.1109/IPFA.2018.8452560.    [2]   L. Lai, N. Li, O. Zhang, and T. Bao, “The demonstrations and  discussion   for   static/read/write   noise   margin  (SNM/RNM/WNM)   via   Nanoprobing   to   SRAM   FA  applications,” in  International Symposium on the Physical and  Failure Analysis of Integrated Circuits (IPFA) , 2015, pp. 26–30.  doi: 10.1109/IPFA.2015.7224324.    [3]   Y. J. Chen, S. C. Chan, R. Liu, S. L. Toh, and R. Ji, “Nanoelectric studies on advanced semiconductor devices by  conductive AFM,” in  International Symposium on the Physical  and Failure Analysis of Integrated Circuits (IPFA) , 2017, pp. 1– 4. doi: 10.1109/IPFA.2017.8060085.    [4]   F. Rivai  et al. , “A Systematic Approach to Localize NVM InterPoly Defects using Nanoprobing Techniques,” in  International  Symposium on the Physical and Failure Analysis of Integrated  Circuits   (IPFA) ,   2020,   pp.   1–5.   doi:  10.1109/IPFA49335.2020.9261045.    [5]   J. Y. Tay, J. Cheah, S. Chef, X. M. Zeng, Q. Liu, and C. L. Gan,  “Investigation on Data Retrieval in Emerging Non-Volatile  Memory Devices Using Conductive Probe Atomic Force  Microscopy,” in  International Symposium on the Physical and  Failure Analysis of Integrated Circuits (IPFA) , 2023, pp. 1–6.  doi: 10.1109/IPFA58228.2023.10249197.    [6]   S. Piotrowski  et al. , “Conductive Atomic Force Microscopy of  Small Magnetic Tunnel Junctions With Interface Anisotropy,”  in  IEEE Transactions on Magnetics , 2015, pp. 1–4. doi:  10.1109/TMAG.2015.2434798.    [7]   L. Dumas, C. Villeneuve-Faure, F. Marc, H. Fremont, C.  Guerin, and G. Bascoul, “Methodology of backside preparation  applied on a MRAM to lead a logical investigation with a nearfield probe,”  Microelectronics Reliability , vol. 150, p. 115102,  2023, doi: 10.1016/j.microrel.2023.115102.    [8]   L. Dumas, G. Bascoul, C. Villeneuve-Faure, F. Marc, H.  Fremont, and C. Guerin, “Nanoprobing on an MRAM Cell,  Following a Backside Opening, to Extract Logical Data,” in  International Symposium for Testing and Failure Analysis  (ISTFA) ,   2023,   pp.   411–419.   doi:  10.31399/asm.cp.istfa2023p0411.    [9]   T. Kawahara, K. Ito, R. Takemura, and H. Ohno, “Spin-transfer  torque   RAM   technology:   Review   and   prospect,”  Microelectronics Reliability , vol. 52, no. 4, pp. 613–627, Apr.  2012, doi: 10.1016/j.microrel.2011.09.028.    [10] M. Hosomi  et al. , “A Novel Nonvolatile Memory with Spin  Torque Transfer Magnetization Switching: Spin-RAM,” in  IEEE International Electron Devices Meeting , 2005, pp. 459– 462. doi: 10.1109/IEDM.2005.1609379.    [11] N. Yazigy  et al. , “Real-Time Switching Dynamics in STTMRAM,”  IEEE Journal of the Electron Devices Society , vol. 10,  pp. 490–494, 2022, doi: 10.1109/JEDS.2022.3185324.

7

