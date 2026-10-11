---
title: "170_Paper.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_7481d1d0e155b871b32ad4bf77be80777295230462135641
file_size: 3706819
---

## Combining Electrical Fault Isolation and Physical  Failure Analysis inside an SEM to locate and  characterize gate leakages on a 3 nm device  

Andreas Rummel 1 , Matthias Kemmler 1 , Klaus Schock 1  Andrew Smith 1 , Stephan Kleindiek 1  1 Kleindiek Nanotechnik GmbH, Aspenhaustr. 25, 72770 Reutlingen, Germany  Phone: (+49)7121-345395-0, Email:  andreas.rummel@kleindiek.com

Abstract —This work employs an easy-to-use method to  quickly find and characterize leakage currents on a  semiconductor sample by combining electrical fault isolation  and physical failure analysis. By using a simple add-on for a  probing system’s tip holders, a prober is transformed into a  scanning device that measures currents through a sample’s  surface and visualizes the currents in a 2D color map that can  be superimposed onto the SE image. As a case study, an area of   $1.5~\ensuremath{\upmu\mathrm{m}\mathrm{~\bf~x~}}1.5~\ensuremath{\upmu\mathrm{m}}$   of a   $\pmb{3}\ \mathbf{nm}$  device was scanned while the  current through the contacts was measured and visualized with  Current Imaging (CI) and gate currents were characterized.  One leaking gate could be identified and the position of the  failure localized using Electron Beam Induced Resistance  CHange (EBIRCH) imaging. This technique also avoids any  damage caused by electron beam irradiation as the beam can  be switched off during scanning.

Keywords—Current Imaging, Probing, Leakage, EBIRCH,  EBAC, EBIC, EFI, PFA

## I.    I NTRODUCTION 

Physical failure analysis is an essential task in the  integrated circuit (IC) manufacturing industry over the past  decades [1][2]. As the distances between structures on a  semiconductor device continuously shrink leakages between  two structures or contacts occur more and more frequently.  These leakages have to be characterized and, in case of a  failure, have to be located.

Leakage analyses can be performed using cAFM  (Conductive Atomic Force Microscopy) [3] or probing  systems that utilize AFM cantilevers [4], however, these  methods are limited in their use to atmospheric conditions.  Instead, we have used a new scanning head that can be  plugged into a nanoprober’s tip holder without the  requirement for any permanent modification to the probing  system. The tip holder provides the means to attach a  conductive AFM cantilever to the nanoprober. By scanning  the (biased) AFM tip over the area of interest, a 2D color  map of the measured current flowing through the sample can  be obtained. We call this method Current Imaging (CI). The  resulting setup can be used in (but is not limited to) an SEM  (Scanning Electron Microscope) or FIB (Focused Ion Beam)  microscope.

This is an ideal combination as CI is used for both  electrical fault isolation and physical failure analysis: it scans  an area and locates the failure within that area as well as  measures the absolute currents between the scanning tip and  the sample’s substrate. Combining it with the probing system  along with other methods that are used for non-destructive  analyses in current technology nodes, like EBIC (Electron  Beam Induced Current) [5], EBAC (Electron Beam  Absorbed Current) [6] and EBIRCH [7][8], provides  an

even more detailed physical and electrical failure location  and analysis to investigate the root cause of a failure:  electrical probing can distinguish whether a direct leakage to  the substrate, or a leakage to drain or source is present. After  having identified the leakage path, EBIRCH can locate the  exact position of the short.

In addition, a high gain Current Imaging mode can be  used to characterize gain leakages over an area of about   $1.5~\mathrm{~\upmum~x~}\,1.5~\mathrm{{\upmum}}$   containing between 40 and 50 insulated  pass gates within some minutes by visualizing leakage  currents with sub-pA resolution.

## II.   M ETHODOLOGY 

An SRAM memory area of a device manufactured in  3 nm technology by TSMC was investigated using a  Kleindiek Nanotechnik PS8 nanoprobing system equipped  with an xyz-substage and a Current Imaging module. The CI  module was used to locate the failure while the Kleindiek  Nanotechnik EBIC amplifier and the Keithley 4200-SCS  were used to investigate the root cause of the failure and to  contact and characterize the transistors. The PS8 Prober  Shuttle was loaded into a Zeiss GeminiSEM 300 for  visualizing the sample during the course of the experiments.

A CI module was attached to one of the eight probe  needle holders and used to pick up the currents from the  sample (Fig. 1). The xyz-substage was used to scan the  sample and to apply a voltage (Fig. 2).

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/7f5d1b80-232f-4bc2-9840-4266ac8adf50/7f5d1b80-232f-4bc2-9840-4266ac8adf50.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215864%3B1743219464&q-key-time=1743215864%3B1743219464&q-header-list=host&q-url-param-list=&q-signature=a3ffbb2c0050684ac4b8db6b55504638714afab2)
Fig. 1.   PS8 prober Shuttle with Current Imaging module

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/dd022c0f-8fd3-40de-87ed-b52b3d91f1a1/dd022c0f-8fd3-40de-87ed-b52b3d91f1a1.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215864%3B1743219464&q-key-time=1743215864%3B1743219464&q-header-list=host&q-url-param-list=&q-signature=983cc4b6f07de701d8ab252f710fb95d69666123)
Fig. 2.   CI measurement during sample scanning.

## III.   M EASUREMENTS 

## A.   Failure location with Current Imaging  

At first, an overview scan was done over an area of   $1.5\;\upmu\mathrm{m}$   x   $1.5\;\upmu\mathrm{m}$  . One gate contact exhibits a high leakage  current of several nA (Fig. 3) while applying a voltage of   $+1\;\mathrm{V}$  . The dynamic range comprises nine orders of  magnitude and can be used to quantify both high leakage  currents and leakages in the sub pA range.

![S  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/a25d348c-a3cd-4ff4-85c7-2cccfd41738a/a25d348c-a3cd-4ff4-85c7-2cccfd41738a.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215864%3B1743219464&q-key-time=1743215864%3B1743219464&q-header-list=host&q-url-param-list=&q-signature=4ecc8819f0d24801b44a699499a5141a6cd53cb4)
Fig. 3.   Current Imaging result, overview, leaking gate marked with a  white arrow.

![89E-12  .SE-11  leaking  gate  1000  800   600   4OKO   200   -600   8001   -995  IA7.3E-7m  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/211b5c48-e739-4762-b084-ddc0785168a7/211b5c48-e739-4762-b084-ddc0785168a7.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215864%3B1743219464&q-key-time=1743215864%3B1743219464&q-header-list=host&q-url-param-list=&q-signature=ea9aec9e603adbba750190d001a77cf28fe5acff)
Fig. 4.   Current Imaging result of gate currents at a high gain, the defective  gate is indicated with a white arrow, the location marked with a green line  between start and stop is analyzed.

## B.   Leakage Characterization with Current Imaging  

While the leaking gate contact is saturated at high  amplifications (see Fig. 44), all other pass gates can be seen  and small changes in the gate leakage can be visualized. A  line plot along the green line is plotted in Fig. 5.

![Measured currents across two gates  E-12  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/fe929ad1-7b92-4935-aa63-85192db5c607/fe929ad1-7b92-4935-aa63-85192db5c607.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215864%3B1743219464&q-key-time=1743215864%3B1743219464&q-header-list=host&q-url-param-list=&q-signature=070b901d9ba32e7c9c21c37490918456bdfa7d07)
Fig. 5.   Current Imaging result of gate currents at a high gain, the defective  gate is indicated with a white arrow, the location marked with a green line  between start and stop is analyzed.

The measured currents are plotted as a sliding average  with an average of five values. While the measured current  of the gate on the right hand side can be seen clearly in both  the CI image and the line plot, the gate on the left hand side  can still be resolved in the line plot showing a current of less  than 1 pA difference with respect to the noise level.

## C.   Resistance Measurements  

Both a transistor characterization (section D.) and  resistance measurements were performed in order to find out  the root cause of the failure.

The resistance measurements show that part of the  current leaking through the gate flows to the substrate and  part of it flows to the pass gate transistor’s drain.

![100.00  ApertureSize=30.00μr   iseReducti  ](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/63ea6f2d-6d29-4a76-96a1-ca2fa11f4e22/63ea6f2d-6d29-4a76-96a1-ca2fa11f4e22.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215864%3B1743219464&q-key-time=1743215864%3B1743219464&q-header-list=host&q-url-param-list=&q-signature=2ef31c665e108cc24016eca7c861433d11c66d1a)
Fig. 6.   Measurement of the Gate – substrate current

![](https://venus-trag-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/c83f9cb4-a3f8-4f2a-941b-18cbf992ab4d/c83f9cb4-a3f8-4f2a-941b-18cbf992ab4d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215864%3B1743219464&q-key-time=1743215864%3B1743219464&q-header-list=host&q-url-param-list=&q-signature=69ae8fcbe17aac85e532cf0a4d5cf65954ce5235)
Fig. 7.   Measurement of the gate – substrate current - result

![](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/ac58a919-27b5-40c2-94ae-fb420068035d/ac58a919-27b5-40c2-94ae-fb420068035d.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215864%3B1743219464&q-key-time=1743215864%3B1743219464&q-header-list=host&q-url-param-list=&q-signature=6861808a2ff0f32c9130483b0a257e39b8c3936d)
Fig. 8.   Measurement of the gate – drain current, result

The resistance measurements show that only a small part  of the current flows directly to the substrate, the larger  fraction flows to the drain of the pass gate transistor.

While the gate to substrate current plot is a smooth  curve, the gate to drain curve shows unstable behavior  starting at around   $1\ \upmu\mathrm{A}$   current.

## D.   Transistor Measurements   

For the sake of completeness, we compared the  transistor curves of both the leaking and a healthy pass gate  transistor. Three probe needles were used to contact gate,  source and drain (Fig. 9), respectively, and the gate and  drain curves were measured (Fig. 10).

![WHT3100KV  MadeT1mo00KXSe ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/6710cdff-c44a-4404-bbab-8a8ba0684161/6710cdff-c44a-4404-bbab-8a8ba0684161.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215864%3B1743219464&q-key-time=1743215864%3B1743219464&q-header-list=host&q-url-param-list=&q-signature=f37f8c98a8ce59e21d63e8aa2bf97ff028621e3f)
Fig. 9.   Transistor Measurement – SEM image

![   V-lFailingTransistor   V-lFailingTransistor  GateVoltage inV  V-l,ReferenceTransistor   V-l,ReferenceTransistor  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/f6bc5198-1abc-4fff-8aa3-9db2641c0d96/f6bc5198-1abc-4fff-8aa3-9db2641c0d96.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215864%3B1743219464&q-key-time=1743215864%3B1743219464&q-header-list=host&q-url-param-list=&q-signature=32d2e3200641dad99ddadc46995f2d86cae16141)
Fig. 10.   Transistor Vd-Id (left) and   $\mathrm{Vg}$  -Id (right) measurements of the  leaking gate (top) and the reference gate (bottom)

In contrast to the measurements of the reference  transistor, where the threshold voltage is clearly defined, the  gate curves of the leaking transistor show an increase of the  drain voltage in the sub-threshold region and a calculation  of the threshold voltage is not possible.

Although the CI analysis detects a failure between the  gate and the substrate, the electrical measurements reveal a  larger leakage between gate and drain. This short is usually  located below but close to the surface and the exact location  can be detected by an EBIRCH analysis.

## E.   EBIRCH Measurement   

For the EBIRCH measurement two probe needles were  used and drain and gate were contacted. At a voltage of  0.5 V across the failure the resistance of the failure changed  at the moment when the electron beam was scanned over it  and resulted in a higher current which was measured.

After superimposing the EBIRCH image with the  Secondary Electron (SE) image the failure could be located  (Fig. 11).

![0.100pm  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/019299f8-563d-4de2-9650-8f5358854837/019299f8-563d-4de2-9650-8f5358854837.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215864%3B1743219464&q-key-time=1743215864%3B1743219464&q-header-list=host&q-url-param-list=&q-signature=49e654a438c3f79c460945352645f41cc80b0cb9)
Fig. 11.   EBIRCH result superimposed on the SE image

It should be noted that during the exposure with the  electron beam at a high beam current (  $60~\upmu\mathrm{m}$   aperture) and a  high magnification of usually 100.000x small particles start  to appear. The EBIRCH image also shows damage to the  drain and gate contact after extensive probing over the  course of several hours.

## F.   Sample Damage from Current Imaging  

As the scanning process is done open loop, the sample  and the cantilever tip may be damaged in case the contact  force between the tip and the sample is too high. This force  is determined by the tip holder’s spring constant, the  cantilever’s stiffness, the size of the scanning tip, and the  homogeneity and hardness of the materials at the sample’s  surface. A low spring constant oriented perpendicularly to  the sample surface is thus crucial for reducing any damage.  Fig. 12 shows the observed changes to the sample surface  after ten scans.

![EHT = 0.500 kV   Mag=50.00KX   Signal A = InLens   300nm  WD = 3.7 mm   Cycle Time = 40.5 Secs   System Vacuum = 9.44e-07 mbar  GSEM300   Aperture Size = 30.00 μm   Noise Reduction = Pixel Avg   Date:30 Nov 2023  Time:12:30:23  ](https://venus-llm-1258344701.cos-internal.ap-guangzhou.tencentcos.cn/userUpload/is-62e36cd9/2025-03-29/b0182524-89c2-4e3a-9c5c-b45b937c99e8/b0182524-89c2-4e3a-9c5c-b45b937c99e8.jpg?q-sign-algorithm=sha1&q-ak=AKID61g5D5fy1TjiRv84nEOHtFJ8gyzjCPL0&q-sign-time=1743215864%3B1743219464&q-key-time=1743215864%3B1743219464&q-header-list=host&q-url-param-list=&q-signature=b26fd370f73b76b23f42f15519c10a836969572b)
Fig. 12.   SRAM surface after 10 CI scans. A slight change in contrast can be  observed near the center of the image. This is the area that was scanned  using CI.

## IV.   D ISCUSSION AND  C ONCLUSION 

We have investigated a new Current Imaging holder and  its use for physical failure analysis and failure location.  With a single scan we measured the electrical current  between a probe tip and a sample manufactured in 3 nm  technology by applying a voltage and could identify a  leaking gate.

One big advantage of this method is its ease of use. The  CI holder is attached to the standard tip holder without any  tools and any further hardware change.

In addition to locating and quantitatively characterizing  the failure we characterized up to 50 pass gates in their  corresponding leakage currents using a single scan with sub  pA resolution.

In order to prove the damage to the located gate,  electrical probing was employed tp determine that the root  cause was a short between gate and drain. Consequently, the  leakage current flowed through the short from the gate to the  drain and then to the substrate.

The exact location could finally be determined using  EBIRCH which shows a typical spot at the boundary  between the gate and the drain.

Even at the smallest currently commercially available  semiconductor technology the damage to both tip and  sample caused by the scanning setup is negligible.

Furthermore, during the scan the electron beam is  paused or can even be switched off to avoid any damage  caused by the electron beam. This is required especially at  the current and future technology nodes where electron  beam voltages of 200 V and less are needed.

## R EFERENCES   

[1]    Zschech, Ehrenfried & Langer, E. & Meyer, A.M. & Engelmann,  Hans-Juergen & Stegmann, Heiko & Geisler, Holm & Tracyand, B. &  Schneider, Gerd. (2004). Physical failure analysis in semiconductor  industry - Challenges to microscopy. Design and Nature. 6. 487-495.    [2]    Song, Hoseok & Seo, Heejeong & Lee, Kiwon & Lee, Yongjae.  (2022). Fault Isolation and Physical Failure Analysis of IC-Embedded  OLED   Display   Device’s   Failure.   78-80.  10.31399/asm.cp.istfa2022p0078.    [3]    Murrell, M.P., Welland, M.E., O’Shea, S.J., Wong, T.M.H., Barnes,  J.R., McKinnon, A.W., Heyns, M., and Verhaverbeke, S. (1993)  Spatially resolved electrical measurements of SiO2 gate oxides using  atomic force microscopy. Appl. Phys. Lett., 62, 786.    [4]    Tong, Tom & Erickson, A. (2004). Current Image Atomic Force  Microscopy (CI-AFM) combined with Atomic Force Probing (AFP)  for location and characterization of advanced technology node.  Proceedings of the 30th International Symposium for Testing and  Failure Analysis, ISTFA 2004.    [5]    A. Rummel, G. Johnson and M. Kemmler, "Low-voltage EBIC  investigation of EBIC fails,"  IPFA,  2021.     [6]    M. Simon-Najasek, J. Jatzkowsk, C. Große and F. Altmann, "A New  Technique for Non-Invasive Short-Localisation in Thin Dielectric  Layers by Electron Beam Absorbed Current (EBAC) Imaging,"  ISTFA,  2012.     [7]    B. Buchea, H. Ryu, M. v. Haartman, C. Butler and T. Tong, "High  Resolution Electron Beam Induced Resistance Change for Fault  Isolation with 100nm2 Localization," ISTFA, 2016.    [8]    G. Johnson, C. D’Aleo, Z. Xu, U. Kwon, H. Berman, Y. Feng, S.  Darling, B. Yates, Y. Wang, M. Kagerer and R. Newton, "Electron  Beam Induced Resistance Change for Device Characterization and  Defect Localization," ISTFA, 2016.

