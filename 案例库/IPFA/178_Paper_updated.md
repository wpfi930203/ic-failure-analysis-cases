---
title: "178_Paper_updated.pdf"
source: IMA知识库/IC失效分析/IPFA
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_13de63dcac5f834d6072ccb8c27fd2c87295230462135641
file_size: 980183
---

EN_PAPER

# Total-Ionizing-Dose Radiation Induced Off-state Current Degradation in p-GaN Gate HEMTs


Total-Ionizing-Dose Radiation Induced Off-state Current Degradation in p-GaN Gate HEMTs


## Authors


-                                                                                                                    


## Keywords


TID, p-GaN, HEMTs, Off-state, holes, trap, Ioff, increase


## Abstract


In this work, the impact of total-ionizing-dose (TID) radiation on the off-state characteristic in p-GaN gate HEMTs is studied. A significant increase in the off-state current (Ioff) is observed after irradiation and the underlying physical mechanism is revealed. Irradiation-induced holes are trapped at GaN channel under the gate region, which would lower energy barrier for electron injection and increase Ioff. Off-state drain leakage current (Ioff), gate-drain capacitance (CGD) and threshold voltage (VTH) are tested to verify the mechanisms. Leakage current test results show irradiation-induced hole trapping could anneal with time.


In space radiation environment, electronic equipment has to suffer from severe radiation effects. Total-ionizing-dose (TID) effect is one of the most significant radiation effects. In Si power devices, electron-hole pairs are generated in the oxide layer under gamma ray radiation, and electrons are swept out rapidly. Holes will transport through the oxide toward the Si/SiO2 interface by hopping through localized states in the oxide and then trapped at the Si/SiO2 interface, forming a positive oxide-trap charge, which causes the degradation of the electrical characteristics of the devices  [10] [11] [12] [13] [14] [15] [16] . In GaN power devices, due to the immaturity of material growth and technology, there are many defects in the GaN and AlGaN materials and its interface, which could trap holes. Electron-hole pairs are generated in the GaN layer under gamma ray radiation, and electrons are swept out rapidly.


Holes will transport through the GaN layer and trapped at GaN channel under the gate because of the potential well for holes, which could degrade the electrical characteristics of the devices. Due to wide band gap (about 3.4 eV), GaN HEMTs have larger ionization energy and threshold energy for defect formation than that for Si devices, resulting in intrinsic better TID tolerance  [17] [18] .


However, conflicting results of TID's effect on GaN HEMTs suggest that some mechanisms are still confused, and its impact on the off-state current (Ioff) of p-GaN gate HEMTs is still absent. In power switching applications, Ioff is important to assess the quality and performance of devices, which is related to the power consumption in the system and could impact the device reliability. Therefore, it is necessary to study the degradation of Ioff in p-GaN gate HEMTs devices induced by TID effect.


In this paper, the impact of TID radiation on the off-state characteristic in p-GaN gate HEMTs is studied. A significant increase in the Ioff is observed after irradiation. The underlying physical mechanisms are found to be related to holes trapped at the GaN channel, which is verified by off-state drain leakage current (Ioff), gate-drain capacitance (CGD) and threshold voltage (VTH) tests. TCAD simulation software is also used to verify the above mechanisms in this paper.


# II. EXPERIMENTAL RESULTS AND ANALYSIS


II. EXPERIMENTAL RESULTS AND ANALYSIS


Fig.  1  shows schematic of TID radiation experiment setup for p-GaN gate HEMTs. The devices are available commercial 650-V/7.5-A p-GaN gate HEMTs with a Schottky-type contact by GaN Systems and the threshold voltage of the devices is about 1.3 V. TID radiation experiment is carried out by using 60 Co γ radiation source with 70 rad (Si)/s dose rate at room temperature. In the experiment, a total of 15 devices were used with drain electrode biased at 50/100/200V and other electrodes grounded. Ioff, VTH and CGD are monitored at 0.5/1.0/1.5 Mrad by Keithley 4200 semiconductor analysis and testing system within 100 s after the end of irradiation to ensure that the devices are not annealed. In Fig.  2 (b), the device is irradiated for the same time. When VDS is stressed at 50 V, Ioff increases about 7 times than that for the fresh state. And when VDS is stressed at 200 V, Ioff increases about 16 times that for the fresh state. Fig.  3  shows schematic irradiation damage mechanism of p-GaN gate region. During gamma ray irradiation, a large number of electron-hole pairs are ionized in the GaN buffer layer. The generated electrons will be swept out rapidly by the drain electrode under off-state bias and some fraction will recombine with holes. Those holes which escape initial recombination will transport through the GaN layer. However, due to the low mobility and the existence of hole potential wells under the gate, holes will accumulate and be trapped at the GaN channel under the gate, which would lower the energy barrier for electron injection from source electrode to drain electrode, leading to the increase of off-state current Ioff. And with the increase of TID, more and more holes will accumulate and trap under the gate, Ioff will increase further. Fig.  4  shows measured transfer I-V characteristic with drain electrode biased at 200 V. In the fresh state, VTH is 1.23 V. After irradiation, VTH shifts from 1.23 V to 1.05 V negatively at TID = 1.5 Mrad, which indicates that holes are trapped at the GaN channel under the gate. However, for devices stressed at off-state bias without irradiation for 6 hours, VTHshifts from 1.23 V to 1.80 V positively, which indicates electrons are also trapped during off-state stress because of deep acceptors (such as carbon or Fe) in GaN buffer. Besides, there is a significant increase in drain to source leakage in subthreshold region of the devices, which also indicates that holes are trapped at the GaN channel under the gate.


In Fig.  5 , increased CGD after irradiation at the same VD also provides an understanding for the holes trapped at the GaN channel under the gate in contrast to devices stressed at off-state bias without irradiation for 6 hours. The metal/p-GaN/AlGaN/GaN gate-stack of GaN devices can be modeled as two back-to-back diodes in series: the metal/p-GaN Schottky junction and p-GaN/AlGaN/GaN (p-i-n) heterojunction. Because the Schottky junction is forward-biased when devices are under off-state stress, its capacitance is small that it can be ignored, CGD mainly depends on the reverse-biased p-i-n heterojunction. Holes trapped at the GaN channel under the gate could increase electron concentration under the gate, which could shrink the depletion region of the p-i-n heterojunction and increase CGD.


# B. ID,str test with gate current stress


B. ID,str test with gate current stress


To further confirm the existence of holes trapped at the GaN channel under the gate, optical pumping effect induced by gate-injected holes is used to verify the mechanism, and ID,str test with gate current stress is also conducted as shown in Fig.  6 [19] . The optical pumping effect shows that the gateinjected holes could combine with 2DEG and emit photons which could pump out electrons or holes in the traps. Before measuring Ioff, the gate is under constant gate current stress (IG,str) for a period of time. The IG,str is set to a fixed value to make sure that the injected holes to the GaN channel from the p-GaN gate keep the same. After gate current stress, ID,str is monitored at VDS = 20 V. Fig.  7  shows extracted ID,str as a function of the gate stress time. It is indicated that ID,str increases gradually with the increase of gate stress time until it reaches saturation. After irradiation, ID,str becomes larger at the initial stage, but smaller when it reaches saturation and ID,str decreases with the increase of TID.


Before irradiation, holes are injected into the GaN channel from the p-GaN under the constant IG,str, which would recombine with 2DEG. And then, photons are emitted which could pump out electrons trapped at acceptor traps under the gate. Negative space charges under the gate are reduced by optical pumping as shown in Fig.  8 (a)  [20] . As a result, the energy barrier of the GaN channel from source to drain is lower, which leads to ID,str increasing. As gate stress time increases, injected holes from the gate increase and more electrons would be pumped out, then ID,str keeps increasing. ID,str does not increase any more when protons pumping out electrons and acceptors trapping electrons are in balance.


After irradiation, holes trapped at the GaN channel under the p-GaN gate lead to the increase of ID,str at the early stage. During gate stress, the number of emitted photons is the same as IG,str is set to a fixed value. The generated photons can pump out electrons, which makes energy barrier lower. Moreover, photons can also pump out holes, which makes energy barrier higher. It means that the number of electrons pumped out by photons would decrease because partial photons are pumping out holes as shown in Fig.  8(b) . And thus, the energy barrier of the GaN channel is higher than the fresh state after gate stress, leading to the decrease of ID,str. As TID increase, holes trapped at the GaN channel under the gate increase and more holes would be pumped out by the photons, the energy barrier is higher, then ID,str keeps decreasing. Fig.  9  shows ID as a function of VD after ID,str test with gate current stress and after 168 hours annealing at room temperature. After irradiation, off-state current ID increases significantly due to holes trapped at the GaN channel under the gate. It is indicated that ID decreases apparently after gate injection, which is ascribed to decreased holes by optical pumping. After 168 hours annealing, ID shows a substantial recovery, and becomes very similar to those measured before irradiation. During the annealing process, holes are released gradually, and the energy barrier of the GaN channel from source to drain is recovering. As a result, off-state current ID will recover with time.


Simulation is also carried out to verify the mechanisms of TID radiation experiment. Fig.  10  shows simulated transfer I-V curve after irradiation. It is indicated that holes trapped at the GaN channel under the gate results in threshold voltage negative shift, and trapped electrons results in threshold voltage positive shift. Fig.  11  shows simulated ID as a function   of VD after irradiation. The holes trapped at the GaN channel under the gate lower the energy barrier for electron injection from source to drain, leading to the Ioff increase. Fig.  12  shows simulated energy barrier from source to drain after irradiation. The holes trapped at the GaN channel under the gate makes the energy barrier lower than that in the fresh state.


# III. CONCLUSION


III. CONCLUSION


In this paper, TID radiation effect induced off-state current Ioff degradation in p-GaN gate HEMTs is presented. The mechanism underlying the increase of Ioff is revealed. A large number of electron-hole pairs are ionized in the GaN buffer layer during irradiation. Electrons will be swept out rapidly by the drain under off-state bias and some fraction will recombine with holes. Holes will transport through the GaN layer and be trapped at the GaN channel under the gate, which lowers the energy barrier for electrons injection from source to drain, leading to the increase of Ioff. Threshold voltage negative shift and increased CGD are also indicated the holes trapping. Besides, the ID,str test with gate current stress is also proposed to verify the existence of holes trapped at the GaN channel under the gate. This work provides an understanding of radiation impact on GaN channel, supporting to assess channel reliability for utilization of power GaN HEMT devices in space application.


# ACKNOWLEDGMENT


ACKNOWLEDGMENT


## References


-                                                                                                                                                                                                                                                                                                                                                                  

