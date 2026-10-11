---
title: "228_Paper.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_3360bdf795693b04bec1ca7f90d619567295230462135641
file_size: 424036
---

# N+


N+


# III. OPTIMIZATION AND SIMULATION VERIFICATIONS


III. OPTIMIZATION AND SIMULATION VERIFICATIONS


In order to suppress the degradations under repetitive avalanche stress, the structure with one step gate oxide above JFET region was firstly proposed, as shown in Fig.  5 (a) .


The optimized parameters of the structure with one step oxide are determined. The distance (D) between the edges of the original oxide and the one step oxide is 1.7μm, and the thickness (Th1) of the one step oxide is 50nm. Fig.  8  shows the perpendicular electric field and I.I. of the optimized structure under avalanche condition. Unfortunately, two additional electric field peaks are introduced by the sharp corners of the step gate oxide. Fig.  6  (a) and (b) respectively show Ron and BV versus the width and the thickness of two additional step gate oxides. When the width is 0.45μm, the Ron and the BV remain unchanged, meanwhile the perpendicular electric field and I.I can also be effectively reduced. However, the thickness should be designed more carefully, or the perpendicular electric field and I.I. peaks can also be introduced due to the sharp corners of two additional step gate oxides, just as shown in Fig.  7 . Combined with the device electrical performances, the optimized thickness is determined to be 50nm. The comparison of three structures is shown in Fig.  8 .It can be apparently observed that the peaks of perpendicular electric field and I.I. of the targeted novel structure are respectively reduced by 10% and 51%. It helps reduce the injection of hot holes into the gate oxide interface above the JFET region, which can effectively suppress the degradation of Rdson and Cgd.


# IV. CONCLUSION


IV. CONCLUSION


In this work, it is demonstrated that the main degradation mechanism of 4H-SiC power MOSFET under repetitive avalanche stress is the injection of hot holes into the gate oxide interface above the JFET region, which leads to the decrease of Rdson and the increase of Cgd. Based on the degradation mechanisms, an improved structure with two additional step gate oxides is proposed. Then the optimized width and thickness of two additional step gate oxides are determined. The perpendicular electric field and I.I. can be effectively reduced by the optimized structure so as to enhance the high avalanche reliability.


# ACKNOWLEDGMENT


ACKNOWLEDGMENT


## References


-                                                                                                                                                                                                                                                                                                                                                                                                                                      


EN_PAPER

# Repetitive-avalanche-induced Electrical Degradation and Optimization for 1.2kV 4H-SiC MOSFETs


Repetitive-avalanche-induced Electrical Degradation and Optimization for 1.2kV 4H-SiC MOSFETs


## Authors


-                                                                                                   


## Keywords


4H-SiC power mosfets, Repetitive avalanche stress, Degradation, Optimization, Two additional step gate oxides


## Abstract


Repetitive avalanche stress results in the injection of hot holes into the gate oxide interface, which leads to the degradations of electrical parameters, attracting wide attentions on improving the avalanche reliability of SiC power MOSFETs. A high avalanche reliability structure with two additional step gate oxides is then proposed in this work. With the help of Silvaco TCAD simulations, the optimized width and thickness of the additional oxides are determined. When compared with the conventional device structure, it is found that the peaks of perpendicular electric field and impact ionization rate of the improved structure under avalanche status are respectively reduced by 10% and 51%. Meanwhile, the breakdown voltage and the on-state resistance of the device are almost unchanged. Therefore, the improved device structure can effectively suppress the degradations caused by avalanche stress.


# I. INTRODUCTION


Silicon carbide (SiC) power metal-oxide-semiconductor field-effect transistor (MOSFET) is considered as a promising candidate for applications in the high power and high temperature fields  [1]  -  [8] , because of the advantages of high breakdown voltage (BV), low switching loss and high operating temperature. However, it is accompanied with reliability problems as a result of the existence of interface states  [9]  -  [13] . Because the 4H-SiC power MOSFETs are often used in the fast switching conditions and there are a large variety of parasitic inductance in the practical application, so the failure caused by unclamped-inductive-switching impact under repetitive avalanche stress is one of the most concerned reliability issues. When the 4H-SiC power MOSFETs are during on-state to off-state transient , a large current induced by parasitic or load inductance will surge from the drain to the source, and the drain-source voltage (Vds) will be clamped at the breakdown voltage at the same time, which can arise the impact of avalanche shock and cause both high current state and high voltage state to appear simultaneously. Under normal operating conditions, this usually does not cause the direct failure of the 4H-SiC power MOSFETS but rather the long-term degradation of electrical characteristics. Some studies have reported the degradation phenomena and mechanism under repetitive avalanche stress  [14]  -  [22] . However, only few improved device structures are proposed  [23, 24] . Therefore, combined with the repetitive avalanche stress experiment and the simulation, the main degraded parameter and mechanism are comprehensively investigated in this work. Then based on the analysis of the dominant degradation mechanism of the device under repetitive avalanche stress, an improved structure for SiC power MOSFETs with two additional step gate oxides is proposed. The optimized parameters are carefully designed to effectively suppress the degradations of electrical parameters caused by repetitive avalanche stress.


# II. EXPERIMENTAL RESULTS AND ANALYSIS


II. EXPERIMENTAL RESULTS AND ANALYSIS


For the sake of investigating the electrical parameters degradation in practice, a commercial 4H-SiC power MOSFET product (C2M0160120D) fabricated by Cree with over 1.2kV BV is used. The schematic cross section of the device structure is shown in Fig.  1 . This device is fabricated on a 12μm-thick n-type epitaxial layer with 0.5μm-long channel, 5μm-long and 0.5μm-thick gate oxide layer. It is designed to sustain over 1200V breakdown voltage. Fig.  2  shows the measured Vgs, Vds and Ids waveforms for the 4H-SiC power MOSFET under avalanche stress. During charging stage, the gate driving voltage (Vgs) is 15V while the direct-current (DC) power supply voltage (VDD) is 100V. A 1mH inductor is used to charge the load current (Iload) to reach a peak value (Ipeak) of 18A before the Vgs returns back to 0V. When the device turns off, the energy stored in the inductance during on-time is released. A high breakdown voltage, approximately 1640V, is then generated on the drain, meanwhile, the Iload flows from the drain to the source, which leads to the avalanche status. Large current and high voltage exist simultaneously until the energy stored (about 172.5 mJ) in the inductance is fully released, which can cause the failure and degradation of the 4H-SiC power MOSFET. As shown in Fig.  3  (a), with the increase of stress cycles, Vth remains almost unchanged, some other electrical parameters, such as the forward turn-on voltage of the body diode(Vf) and breakdown voltage(BV) also remain unchanged, which indicates that the channel region and the body diode of the device are almost not affected by the stress. Meanwhile, it is observed that the Rdson of the 4H-SiC power MOSFETs has a slight decrease, which indicates that there are positive charges caused by the stress at the SiC/SiO2 interface above JFET region. The obvious right shifts of Cgd-Vds curves can also verify this point, just as shown in Fig.  3 (b) . With the increase of stress cycles, the gate-drain capacitance (Cgd) increases, while the gate-source capacitance (Cgs) and the drain-source capacitance (Cds) remain unchanged. In order to deeply illustrate it, a simulation is carried out with the help of Silvaco. Fig.  4  shows that the peaks of perpendicular electric field and the impact ionization rate (I.I.) along the gate oxide interface under avalanche condition both exist in the JFET region, which contributes to the injection of hot holes into the gate oxide interface above the JFET region. The injected holes can restrain the extension of the depletion layer in the JFET region, resulting in the increase of the Cgd, without affecting the Cgs and the Cds. Meanwhile, the electrons attracted by the injected holes can accumulate on the surface of the JFET region, causing the decrease of Rdson. Therefore, combined with the experimental measurements and simulation results, it is demonstrated that the main degradation mechanism is the injection of hot holes into the gate oxide interface above the JFET region.

