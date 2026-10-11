---
title: "ISTFA-2014.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_a5e68f118f9b859bff09b8773c2518017295230462135641
file_size: 60634802
---

ISTFA  2014


Conference Proceedings from the 40th International Symposium for


Testing and Failure Analysis


November 9–13, 2014


George R. Brown Convention Center Houston, Texas, USA


TM


asminternational.org


Organized by


Published by


ASM International


Materials Park, Ohio 44073-0002


®


ASM INTERNATONAL


asminternational.org/istfa


OEDFAS Electronic Device Failure Analysis Society


4INTERNATIONALASM


Copyright  © 2014


by


ASM International®


All rights reserved


No part of this book may be reproduced, stored in a retrieval system, or transmitted, in any form or  by any means, electronic, mechanical, photocopying, recording, or otherwise, without the written  permission of the copyright owner.


First printing, November 2014


Great care is taken in the compilation and production of this Volume, but it should be made clear  that NO WARRANTIES, EXPRESS OR IMPLIED, INCLUDING, WITHOUT LIMITATION, WARRANTIES OF  MERCHANTABILITY OR FITNESS FOR A PARTICULAR PURPOSE, ARE GIVEN IN CONNECTION WITH THIS  PUBLICATION. Although this information is believed to be accurate by ASM, ASM cannot guarantee  that favorable results will be obtained from the use of this publication alone. This publication is  intended for use by persons having technical skill, at their sole discretion and risk. Since the  conditions of product or material use are outside of ASM's control, ASM assumes no liability or  obligation in connection with any use of this information. No claim of any kind, whether as to  products or information in this publication, and whether or not based on negligence, shall be greater  in amount than the purchase price of this product or publication in respect of which damages are  claimed. THE REMEDY HEREBY PROVIDED SHALL BE THE EXCLUSIVE AND SOLE REMEDY OF BUYER, AND IN NO EVENT SHALL EITHER PARTY BE LIABLE FOR SPECIAL, INDIRECT OR CONSEQUENTIAL  DAMAGES WHETHER OR NOT CAUSED BY OR RESULTING FROM THE NEGLIGENCE OF SUCH PARTY. As  with any material, evaluation of the material under end-use conditions prior to specification is  essential. Therefore, specific testing under actual conditions is recommended.


Nothing contained in this book shall be construed as a grant of any right of manufacture, sale, use, or  reproduction, in connection with any method, process, apparatus, product, composition, or system, whether or not covered by letters patent, copyright, or trademark, and nothing contained in this  book shall be construed as a defense against any alleged infringement of letters patent, copyright, or  trademark, or as a defense against liability for such infringement.


Comments, criticisms, and suggestions are invited, and should be forwarded to ASM International.


ISBN-13: 978-1-62708-074-3


ISBN-10: 1-62708-074-0


SAN: 204-7586


Materials Park, OH 44073-0002


Printed in the United States of America


iii


EDFAS 2014-2015 BOARD OF DIRECTORS


EDFAS President


Ms. Cheryl Hartfield


Oxford Instruments Company 


EDFAS Vice President


Mr. Zhiyong Wang  Maxim Integrated 


EDFAS Board Members


Position


Affiliation


President


Oxford Instruments Company


Mr. Zhiyong Wang


Vice President


Maxim Integrated


Dr. William E. Vanderlinde


Secretary


Laboratory for Physical Sciences


Mr. Christopher L. Henderson


Financial Officer


Semitracks, Inc.


Mr. Jeremy A. Walraven


Past President


Sandia National Laboratories


Mr. Michael O' Toole


Executive Director


EDFAS


Mr. Nicholas Antoniou


Member at Large


Revera Inc.


Mr. Dan Bodoh


Freescale Semiconductor


Dr. Lee Knauss


Booz Allen Hamilton


Ms. Sandra Delgado


Nanolab Technologies


Ms. Susan Li


Spansion Inc.


Mr. David Su


TSMC


Board Committees


Dr. Kathryn Dannemann


ASM BOT Liaison


Southwest Research Institute


Dr. Felix Beaudoin


EDFA Chair


Global Foundries


Education Chair


Dr. James Demarest


Events Chair


IBM


Dr. Thomas Moore


Membership Chair


Waviks, Inc.


Mr. Jeremy A, Walraven


Nominating Chair


Dr. Philippe Perdu


International Growth


CNES


iv


2014 ORGANIZING COMMITTEE


Dr. James J. Demarest


Dr. Martin Keim


Ms. Becky Holdford


General Chair


Vice General Chair


Technical Program Chair


Tutorial and Short Course Chair


Mentor Graphics


Texas Instruments, Inc.


Dr. Zhiyong Wang


Immediate Past General Chair  Maxim Integrated


ACTIVITIES CHAIRS


Expo Chair


Mr. David Grosjean  Panel Vice Chair


Qualcomm


Ms. Efrat Moyal


Publicity Chair


LatticeGear LLC


Mr. Kendall Scott Wills  Local Arrangements Chair  Consultant


Panel Chair


Tutorial & Short Course


Vice Chair, Spansion Inc.


Ms. Rose Ring


Vice Chair, Movie Vice Chair,  Global Foundries


Dr. Mayue Xie


Movie Chair & User Group   Vice Chair, Intel


Dr. Lihong Cao


International Chair


AMD


Mr. Rick Livengood  User Group Chair


Intel


Dr. Sam Subramanian  AV Chair


40TH INTERNATIONAL SYMPOSIUM F。R TESTING AND FAILURE ANALY5IS NOVEMBER 9-13 2014


v


ISTFA 2014 TECHNICAL PROGRAM COMMITTEE


ISTFA 2014


Technical Program Chair  Dr. Martin Keim


|SESSION CHAIRS |SESSION CHAIRS |SESSION CHAIRS |
|---|---|---|

|3D Packages Case Studies and the Electrical Characterization and |3D Packages Case Studies and the Electrical Characterization and |3D Packages Case Studies and the Electrical Characterization and |

|Frank Altmann, Fraunhofer Institute for |Failure Analysis Process |Nanoprobing |

|Mechanics of Materials |Peter Jacob, EMPA Duebendorf |Stefan B. Kaemmer, Multiprobe |

|Yan Li, Intel |Zhigang Song, IBM |Izak Kapilevich, DCG Systems |

|Defect Characterization and Metrology |Detecting Counterfeit Devices |Novel Research-Level Techniques and |

|Terence Kane, IBM |Zhigang Song, IBM |Concepts |

|Phil Kaszuba, IBM ||Michael Bruce, Consultant |

||Microscopy |Huimeng Wu, Carl Zeiss Microscopy, LLC |

|Emerging Concepts and Techniques |Carl Nail, Evans Analytical Group, LLC ||

|Michael Bruce, Consultant ||Photon-Based Techniques |

|Huimeng Wu, Carl Zeiss Microscopy, LLC |Panel Discussion |Herve Deslandes, DCG Systems |

||Philippe Perdu, CNES |Frank Zachariasse, NXP Semiconductors |

|Packaging and Assembly Analysis |||

|Lihong Cao, Advanced Micro Devices |Sample Preparation and Device Deprocessing |Sample Preparation and Device Deprocessing |

|Posters |Roger Alvis, FEI Company |Roger Alvis, FEI Company |

|David Grosjean, Qualcomm |Bryan Tracy, Spansion, Inc. |Bryan Tracy, Spansion, Inc. |

|Martin Versen, University of Applied |||

|Sciences Rosenheim |Circuit Edit Michael DiBattista, Qualcomm, Inc. |Circuit Edit Michael DiBattista, Qualcomm, Inc. |

||Dane Scott, Intel Corporation |Dane Scott, Intel Corporation |

vii


Contents


IPFA and ESREF Paper Exchange


Defect Localization Enhancement Using Light Induced CI-AFP  ............................................... 1


N. Dayanand, A.C.T. Quah, C.Q.Chen, S.P. Neo, G.B. Ang, M. Gunawardana, Z.H. Mai, and J.C. Lam  GlobalFoundries, Singapore


Detectability of Automotive Power MOSFET On-Resistance Failure at


High Current Induced by Wafer Fab Process Excursion  .......................................................... 5


Yann Weber, Julien Goxe, and Maris Castignolles; Freescale Semiconducteurs France SAS


Emerging Concepts and Techniques


Novel NIR Camera with Extended Sensitivity and Low Noise for


Photon Emission Microscopy of VLSI Circuits  ........................................................................ 6


Andrea Bahgat Shehata1, Franco Stellari1, Alan Weger1, Peilin Song1,  Herve Deslandes2, Ted Lundquist2, Euan Ramsay2


(1) IBM T.J. Watson Research Center, Yorktown Heights, NY, USA


(2) DCG Systems, Fremont, CA, USA


Automated Mapping of Very Large Areas of VLSI Circuit Using SIL  ........................................ 12


Chung-Ching Lin and Franco Stellari


IBM T.J. Watson Research Center, Yorktown Heights, NY, USA


Routine Device-Level Atom Probe Analysis  ......................................................................... 19


D.F. Lawrence, R.M. Ulfig, D.J. Larson, D.P. Olson, D.A. Reinhard, I.Y. Martin,  S. Strennen, and P.H. Clifton


CAMECA Instruments Inc., Madison, WI, USA


Novel Research-Level Techniques and Concepts


High-Resolution Backside GMR Magnetic Current Imaging on a


Contour-Milled Globally Ultrathin Die  ................................................................................ 23


D. Vallett1, J. Gaudestad2, and C. Richardson3


(1) PeakSource Analytical, LLC, Fairfax, VT, USA


(2) Neocera, LLC, Beltsville, MD, USA


(3) Allied High Tech Products, Inc., Rancho Dominguez, CA, USA


viii


Resolution Improvement through Sparse Image Reconstruction Techniques for


Dark Field Subsurface Microscopy of Integrated Circuits  ..................................................... 28


T. Berkin Cilingiroglu, W. Clem Karl, Janusz Konrad, Michael D.W. Grogan,


Abdulkadir Yurt, Ahmet Tuysuzoglu, Bennett B. Goldberg, and M. Selim Unlu  Boston University, Boston, MA, USA


3D Packages I


3D IC/Stacked Device Fault Isolation Using 3D Magnetic Field Imaging  ................................. 33


A. Orozco1, N.E. Gagliolo1, C. Rowlett1, E. Wong1, A. Moghe1, J. Gaudestad1,  V. Talanov1, A. Jeffers2, K. Torkashvan2, F.C. Wellstood2, Stephan Dobritz3,  Mathias Boettcher3, A.B. Cawthorne4, and F. Infante5


(1) Neocera, LLC, Beltsville, MD, USA


(2)University of Maryland, College Park MD, USA


(3) Fraunhofer IZM-ASSID, Moritzburg, Germany


(4)Trevecca Nazarene University, Nashville, TN, USA


(5) Intraspec Technologies, Toulouse, France


Failure Analysis Work Flow for Electrical Shorts in


Triple Stacked 3D TSV Daisy Chains  ................................................................................... 38


J. Gaudestad1, A. Orozco1, I. De Wolf 2 , T. Wang2, T. Webers2, R. Kelley3,  T. Morrison3, and S. Madala3


(1) Neocera, Beltsville, MD, USA


(2) IMEC, Leuven, Belgium


(3) FEI, Hillsboro, OR, USA


Short Localization in 2.5D Microchip with


Interposer Using Magnetic Current Imaging  ....................................................................... 43


J. Gaudestad1, D. Nuez 2 , and P. Tan2


(2) Xilinx, San Jose, CA, USA


Applying Innovative Techniques for Solving FA Challenges of


3D IC Failures Utilizing Conventional Equipment  ................................................................ 49


Phoumra Tan, Kenny Ng, Eric Thorne, S.Y. Pai, Doug Hamilton, and Dan Nuez  Xilinx, Inc., San Jose, CA, USA


Detecting Counterfeit Devices


Advanced Physical Inspection Methods for Counterfeit IC Detection  .................................... 55


Sina Shahbazmohamadi, Domenic Forte, and Mark Tehranipoor  University of Connecticut, Storrs, CT, USA


ix


Photon-Based Techniques I


Laser Logic State Imaging (LLSI)  ........................................................................................ 65


Baohua Niu, Grace Mei Ee Khoo, Yuan-Chuan Steven Chen, Fernando Chapman,  Dan Bockelman, and Tom Tong


Intel Corporation, Hillsboro, OR, USA


The Role of Free Carrier Absorption in LADA  ....................................................................... 73


Kent Erington, Dan Bodoh, Kris Dickson, and George Lange  Freescale Semiconductor, Inc., Austin, TX, USA


Root Cause Analysis Techniques Using Picosecond Time Resolved LADA ................................ 82


Dan Bodoh1, Kent Erington1, Kris Dickson1, George Lange1,  Carey Wu1, and Tom Crawford2


(1) Freescale Semiconductor, Inc., Austin, TX, USA


(2) DCG Systems, Inc., Fremont, CA, USA


Packaging and Assembly Analysis I


Comparative Study on Decapsulation for Copper and


Silver Wire-Bonded Devices  ............................................................................................... 87


François Kerisit 1 , Bernadette Domenges1, and Michael Obein2


(1) LaMIPS, CRISMAT-NXP semiconductors-Presto Engineering, Caen, France


(2) Digit Concept, Secqueville en Bessin, France


Laser Focus Depth Adaptation for Decapsulation of Copper Wirebonded Devices  .................. 94


H.B. Kor, Q. Liu, Y.W. Siah, and C.L. Gan; Nanyang Technological University, Singapore


A Sample Preparation on Decapsulation Methodology for


Effective Failure Analysis on Thin Small Leadless (TSLP) Flip Chip Package with


Copper Pillar (CuP) Bump Interconnect Technology  .......................................................... 100


Gwee Hoon Yen and Ng Kiong Kay, Infineon Technologies, Melaka, Malaysia


Photon-Based Techniques II


Improved Lock-in Phase Mapping of Modulated Reflectance with SIL  ................................. 105


Zhongling Qian, Christof Brillert, and Christian Burmer  Infineon Technologies AG, Munich, Germany


Visible Light LVP on Ultra-Thinned Substrates  .................................................................. 110


Joshua Beutler, J. Joseph Clement, Mary A. Miller, Jeffery Stevens, and Edward I. Cole, Jr. Sandia National Laboratories, Albuquerque, NM, USA


x


Introduction of Spectral Mapping through Transmission Grating, Derivative


Technique of Photon Emission  ........................................................................................ 115


Thierry Parrassin1, Sylvain Dudit1, Michel Vallet1, Antoine Reverdy2, and Hervé Deslandes3


(1) STMicroelectronics, Crolles, France


(2) Sector Technologies, Gières, France


(3) DCG Systems Inc., Fremont, CA, USA


3D Packages II


SAM Assisted Contour Milling  .......................................................................................... 125


Christian Hollerith1, Bernd Krüger1, Stefan Waginger1, Doris Plabst1, and Matthias Fritz2


(1) Infineon Technologies, Neubiberg, Germany


(2) Kern Microtechnik, Eschenlohe, Germany


Efficient Nondestructive 3D Defect Localization by Lock-in Thermography


Utilizing Multi-Harmonics Analysis  .................................................................................. 130


Falk Naumann, Frank Altmann, Christian Grosse, and Rolf Herold


Fraunhofer Institute for Mechanics of Materials IWM, Halle, Germany


Advances in FIB-SEM Analysis of TSV and Solder Bumps—


Approaching Higher Precision, Throughput, and Comprehensiveness  ................................ 136


Tomáš Hrnčíř1, Jiří Dluhoš1, Lukáš Hladík2, Efrat Moyal3,  Janet Teshima3, and Jaromír Kopeček4


(1) Tescan Brno, Brno, Czech Republic


(2) Tescan Orsay Holding, Brno, Czech Republic


(3) LatticeGear, LLC, Beaverton, OR, USA


(4) Institute of Physics ASCR, Prague, Czech Republic


The Physical Isolation of a Die in a Stacked-Die Configuration  ........................................... 143


Vivian Jang and Ken Sias, Texas Instruments, Dallas, TX, USA


Microscopy I


Evaluation of TEM-Lamella Oxidation  .............................................................................. 148


Thomas Haber1 and Christian Gspan2


(1) ams AG, Unterpremstaetten, Austria


(2) Graz University of Technology, Austria


Spectrum Sharpening on Rotation Averaged TEM Nano Beam


Electron Diffraction Patterns  .......................................................................................... 152


Yongkai Zhou, Younan Hua, and Xiaomin Li


WinTech Nano-Technology Services Pte. Ltd., Singapore


xi


Automated Defect Analysis in Solar Cells Using EBIC  ......................................................... 156


Grigore Moldovan1, Shark Lotharukpong2, and Peter Wilshaw2


(1) Oxford Instruments NanoAnalysis, High Wycombe, UK


(2) University of Oxford, Oxford, UK


Packaging and Assembly Analysis II


Reballing/Rebumping Ultra-Fine Pitch Packages


Less Than 0.5 mm Pitch for FA  ......................................................................................... 160


Bob Wettermann, Best Inc., Rolling Meadows, IL, USA


A Comprehensive Investigation of the Galvanic Corrosion Induced Ag-Al


Bond Degradation in Microelectronic Packaging Using Argon Ion Milling,


SEM, Dual Beam FIB-SEM, STEM-EDS, and TOF-SIMS  .......................................................... 166


Yixin Chen, Emmanuel Simon, Bing Sheng Khoo, Esther Lee, Meailing Chooi,  Meng Hao, Jingjing Shao, Younan Hua, and Xiaomin Li


Correlation of Thin Film Measurement Techniques for Device Packaging


Processes  ...................................................................................................................... 172


J. Walter1, W. Mack1, C.Y. Lee2, and C. Gspan3


(1) Infineon Technologies AG, Regensburg, Germany


(2) Infineon Technologies Sdn. Bhd., Malacca, Malaysia


(3) Center for Electron Microscopy (ZFE), Graz, Austria


Case Studies on Application of 3D Real Time X-ray for Flip Chip C4 Package  ........................ 178


Lihong Cao, Wallace Donna, Loc Tran, and Lynda Tuttle  Advanced Micro Devices, Inc., Austin, TX, USA


Analysis of Two Electrical Failures Caused by


Die Attach of Exposed Pad Package  ................................................................................. 184


Jinglong Li, Motohiko Masuda, Yi Che, and Miao Wu


Freescale Semiconductor (China) Limited, Tianjin, China


Electrical Characterization and Nanoprobing


Analysis of InGaAs Epi Defects by Conductive AFM  ............................................................ 189


Aaron Cordes1, Tom Dyer1, and Sean Hand2


(1) Sematech, Albany, NY, USA


(2) Bruker Nano Surfaces, Santa Barbara, CA, USA


xii


Utilizing Nanoprobing and Circuit Diagnostics to Identify


Key Failure Mechanism of Otherwise Nonvisible Defects in


20 nm Logic Devices  ....................................................................................................... 196


M.K. Dawood, C. Chen, P.K. Tan, S. James, P.S. Limin, H. Tan, H.H. Yap,  G.R. Low, J. Lam, and Z.H. Mai


GlobalFoundries Singapore Pte. Ltd., Singapore


Failure Analysis of Bit Line to SNC Leakage Fail in


2x nm DRAM Using Nano-Probing Technique  .................................................................... 202


Jaeho Won, Jundong Kim, Jina Kim, Jihye Shin, Jihoon Kim, Kyungrim Lee, Miae Yoon, Jonghak Lee, Jaeyoon Lee, Weonjoon Suh, and Hyeonsoo Kim


SK Hynix Semiconductor, Gyeoggi-do, Korea


Analysis of an Anomalous CMOS Transistor Exhibiting Drain to


Source Leakage—Its Model and Cause  .............................................................................. 205


Yuk L. Tsang1, Alex VanVianen2, Xiang D. Wang3, and N. David Theodore3


(1) Freescale Semiconductor Inc., Austin, TX, USA


(2) Freescale Semiconductor Inc., Tempe, AZ, USA


(3) Freescale Semiconductor Inc., Chandler, AZ, USA


Packaging and Assembly Analysis III


Feature Based Nondestructive Fault Isolation in Advanced IC Packages  ............................. 210


K.C. Lee1, J. Alton1, M. Igarashi1, and S. Barbeau2


(1) TeraView Limited, Cambridge, UK


(2) IBM Microelectronics, Bromont, QC, Canada


Failure Mechanism Studies and Root Cause Identification of Nonstick on


Pad on Microchip Al Bondpads  ........................................................................................ 215


Hua Younan, Zhou Yongkai, Chen Yixin, Fu Chao, and Li Xiaomin  WinTech Nano-Technology Services Pte. Ltd., Singapore


Failure Localization of Intermittent Short Failures Caused by


Vertical Conductive Anodic Filament Formation  ............................................................... 218


Daniel Nuez and Phoumra Tan;  Xilinx, San Jose, CA, USA


Case Studies and the Failure Analysis Process I


Understanding the Cu Void Formation by TEM Failure Analysis  .......................................... 227


Binghai Liu, Jie Zhu, Changqing Chen, Eddie Er, Siping Zhao, Jeffrey Lam,  Sebastian Elizabeth, and Chen Ye


xiii


Failure Analysis Methodology on Systematic Missing Cu in


RAM Due to Cu CMP  ........................................................................................................ 231


Ghim Boon Ang, Changqing Chen, Hui Peng Ng, Alfred Quah, Angela Teo,  Kim Hong Yip, Soh Ping Neo, Jeffrey Lam, and Zhihong Mai


GlobalFoundries Singapore Pte.Ltd., Singapore


Identification of Subtle Defect by Means of


High Kev SEM Passive Voltage Contrast  ............................................................................ 236


Sujing Xie, Chaoying Chen, Nathan Wang, Andrew Komrowski,  Qindi Wu, and Saunil Shah


Maxim Integrated, San Jose, CA, USA


In-Line Defects Overlaying with Functional Failures and Characterization for


Fast Defect Learning and Fast Yield Improvement  ............................................................ 241


Zhigang Song, Oliver D. Patterson, and Qian Xu


IBM Systems and Technology, Hopewell Junction, NY, USA


Observation of Channel Strain Release in pMOS Device with


Low Idsat Using Energy-Filtered Nano-Beam Diffraction Technique .................................... 246


Jie Zhu, An Yan Du, Bing Hai Liu, Eddie Er, Si Ping Zhao, and Jeffrey Lam  GlobalFoundries, Singapore


Sample Preparation and Device Deprocessing I


Effective and Efficient FEOL Defects Localization/ Inspection by


Selective Mechanical/Chemical Deprocessing  ................................................................... 250


Ng Hui Peng, Teo Angela, Ang Ghim Boon, Yip Kim Hong, Chang Qing Chen,  Alfred Quah, Tam Yong Seng, Jeffrey Lam, and Zhi Hong Mai


GlobalFoundries Singapore Pte. Ltd.,Singapore


Site-Specific, Wide Field-of-View Cross-Sectional Sample Preparation,


Imaging and Analysis in a Plasma Ion Source Helios DualBeam™ Microscope  ...................... 255


Roger Alvis and Ron Kelley


FEI Company, Hillsboro, OR, USA


MicroPREP—A New Laser Tool for High-Throughput Sample Preparation  ........................... 261


Michael Krause1, Martin Ebert1, Thomas Höche1, and Uwe Wagner 2


(1) Fraunhofer CAM, Halle, Germany


(2) 3D-Micromac AG, Chemnitz, Germany


Application of Fast Laser Deprocessing Techniques in


Physical Failure Analysis on SRAM Memory of Advance Technology  .................................... 268


H.H. Yap, P.K. Tan, G.R. Low, M.K. Dawood, H. Feng, Y.Z. Zhao, Y. Zhou, R. He, H. Tan, Y.M. Huang, D.D. Wang, Y. Zhou, P.S. Limin, S. James, J. Lam, and Z.H. Mai


xiv


Ex-Situ Lift Out of Plasma Focused Ion Beam Prepared Site Specific Specimens  .................. 274


Lisa Chan1, Jon M. Hiller1, and Lucille A. Giannuzzi2


(1) Tescan USA, Cranberry Township, PA, USA


(2) EXpressLO LLC, Lehigh Acres, FL, USA


Circuit Edit


Using Energy Dispersive Spectroscopy (EDS) to Determine the Resistance of


FIB Jumpers for Circuit Edit  ............................................................................................ 278


Michael DiBattista1, Corey Senowitz1, Hasan Faraby2, and Prabhakar Bandaru2


(1) Qualcomm Incorporated, San Diego, CA, USA


(2)University of California, San Diego, La Jolla, CA, USA


New Ion Source for High Precision FIB Nanomachining and Circuit Edit  .............................. 284


Adam V. Steele1, Brenton Knuffman1, and Jabez J. McClelland2


(1) zeroK NanoTech Corporation, Montgomery Village, MD, USA


(2) National Institute of Standards and Technology, Gaithersburg, MD, USA


Microscopy II


Evaluation of Power SiC-MOSFET Using Super-Higher-Order Scanning


Nonlinear Dielectric Microscopy—Imaging of Carrier Distribution and


Depletion Layer  ............................................................................................................. 289


N. Chinone1, Y. Cho1, and T. Nakamura2


(1) Tohoku University, Sendai, Miyagi, Japan


(2) ROHM Ltd. Co., Kyoto, Kyoto, Japan


Imaging Performance of aSIL Microscopy on


Subsurface Imaging of SOI Chips  ..................................................................................... 293


Aydan Uyar, Abdulkadir Yurt, T. Berkin Cilingiroglu,  Bennett B. Goldberg, and M. Selim Ünlü


Boston University, Boston, MA, USA


Methods to Reconstruct SEM and Optical Probe Tips Using a FIB Tool  ................................. 296


Walter Lepuschenko and David Goulet, IBM, Essex Junction, VT, USA


Near-Field Scanning Optical Microscopy for Through-Silicon Imaging and


Fault Isolation of Integrated Circuits  ............................................................................... 299


R. Giridharagopal, T.M. Eiles, and B. Niu, Intel Corporation, Hillsboro, OR, USA


xv


Posters


Defect Localization and Root Cause Analysis on e-Fuse Read Reliability Failure  .................. 304


Hung Chin Chen, Chih Yang Tsai, Shih Yuan Liu, Yu Pang Chang, and Jian Chang Lin  United Microelectronics Corporation, Tainan, Taiwan, ROC


Application of Soft Defect Localization Technique for


SRAM Soft Failure Debug  ................................................................................................. 307


Moon Seung Je, Yeoh Boon Lian, Goh Szu Huat, Shaalini Chithambaram,  A.C.T Quah, and Jeffrey Lam


GlobalFoundries, Singapore


Applications and Techniques for 2D Picosecond Imaging for Circuit Analysis  ...................... 312


Franco Stellari, Peilin Song, and Alan J. Weger


Applications of AFP Nanoprobing for Localization of Implant Related Issues  ....................... 318


N. Dayanand, K.H. Yip, A.C.T. Quah, S.P. Neo, H.P. Ng, G.B. Ang, J.C. Lam, and Z.H. Mai  GlobalFoundries, Singapore


Automatic Emission Spots Identification in Static and Dynamic Imaging by


Research of Local Maxima  ............................................................................................... 322


A. Boscaro1, S. Chef 1 , S. Jacquir1, K. Sanchez 2 , P. Perdu2, and S. Binczak1


(1) Le2i, Dijon, France


(2) Centre National d’ Etudes Spatiales, Toulouse, France


Auto-Metrology on TEM Images of FinFET  ......................................................................... 327


Sajal Biring, Materials Analysis Technology Inc., Hsinchu City, Taiwan, R.O.C.


Characterization and Simulation of a Body Biased Structure in


Triple-Well Technology under Pulsed Photoelectric Laser Stimulation  ............................... 330


N. Borrel1, C. Champeix1, M. Lisart1, A. Sarafianos1, E. Kussener 2 ,


I. INTRODUCTION


As technology node shrinks, traditional SEM based  Passive Voltage Contrast (PVC) technique has become less  effective to pick up front-end of line defects as junction  leakages and resistive open defects become more subtle. Thus, marginal PVC contrast difference between good and bad  samples requires further verification and Current Imaging – Atomic Force Probing (CI-AFP) [1] has become an effective  technique used at tungsten contact level to localize and  characterize transistor level defects. CI-AFP is typically  performed at contact mode with tip biased at a small positive  or negative voltage and a scanned current image is created by  measuring the leakage current flowing from the tip to sample  or sample to tip. The measured current image reflects the  source/drain/well junction leakage and gate oxide leakage at a  particular biased voltage.


Conventional current imaging was done in the dark to  minimize the interferences of the junction leakage current  with the photo-generated current. This technique has been  very effective in localizing memory and logic hard failures  such as high resistance contact, junction leakage, gate-S/D  short, bridge between NMOS and PMOS transistors, [1], [2] for devices in bulk process. However, there are certain defects  that are not easily detectable by conventional CI-AFP.  One  such failure mode is a bridge between two or more similar  type junctions (p+/nwell - p+/nwell or n+/pwell - n+/pwell). In this paper, we described 2 case studies on the use of light  induced effects to improve the effectiveness of localizing a  short between 2 similar junction types in the memory array  and also a case study where light induced effects help to


V 8


distinguish between gated and non-gated diode in a logic gate


3 0。


to S/D short scenario.


In this paper, the CI-AFP analysis and nanoprobing  measurements were conducted using Multiprobe AFP MPIIb  system. Fig.1 shows a snapshot of the AFP DUT stage, 2 out  of a total of 4 probe heads in position and a 40X optical lens


[3]. The DUT stage is able to rotate and move in X, Y and Z


directions. The DUT stage is also fixed onto a precision snap  stage for precise sample movement within +/- 200um in X & Y directions. The 40X optical lens with 100X digital zoom is  mounted above the stage for gross tip to tip positioning and  also for navigation to the region of interest (ROI). The optical  lens is illuminated with a tungsten light source which is turned  off during current imaging or nanoprobing for accurate  junction leakage and transistor characterization. However, in  this work, the light source is deliberately turned on during  current imaging to generate photo-carriers for fault  localization.


Fig.1 AFP stage and housing.


II. RESULTS AND DISCUSSION


SCENARIO1: SRAM Pull-Up Gate–S/D leakage detection  using PV effect.


Scenario 1 illustrates two cases where light induced CIAFP was used to effectively localize SRAM Pull-Up (PU) transistors Gate-Source/Drain short which is otherwise not  easily detectable with conventional current imaging analysis. Fig.2 shows the layout of a single 6T SRAM cell which is  commonly used in advanced technology node memory array. While the NMOS pull-down (PD) and pass-gate (PG) transistors have isolated S/D contacts, the PU transistors have  rectangular contacts (CAREC) to locally connect the gate of  one PU to the drain of the other PU transistor. Thus, gate of  the PU exhibits a P+/N diode junction characteristic.


Fig.2. 6T SRAM cell layout


Stage


Probe Head


40X Optical Lens


PU18V 3


3PU2


VDD


PD2


PD1 PG1


PG2 VSS


VSS BL


BLB


WL


– Active


– Poly


– Contacts


SRAM single bit failure was identified on a 40nm device  and physical failure analysis was performed at the failed  bitmap address. Both SEM inspection at via1/metal1 and PVC  analysis at via 1 and contact levels, as shown in fig 3(b), observed no anomaly. Conventional CI-AFP was employed  and Fig 4(a) and 4(b) shows the current image with a small  positive and negative bias to the tip (±0.5V) respectively. In  the positive bias scan, PU S/D junctions are forward biased  resulting in diffusion current flowing from tip to sample  denoted by white contrast as shown in fig 4(a). The PD & PG  S/D contacts were in reverse bias with very small leakage  current. For the negative biased scan in fig 4(b), the NMOS  S/D junctions were in turn forward biased resulting in current  flow from sample to tip denoted by black contrast. From these  results, one could deduce that there is no resistive active  contacts and CARECs, no NMOS gate-S/D short, no gate  oxide breakdown and no junction leakages. However, we  could not identify if there was a bridge among PU contacts, resistive open on PG gate contact, transistor S/D bridge or if  the failure is due to transistor mismatch. Thus, conventionally, an extensive 6 transistors characterization, which is time  consuming, would usually have to be performed to further  localize the defect location.


明申


(a)


(b)


Fig.4 CI-AFP with +0.5V (a) and –0.5V bias (b). Failed  cell is highlighted in red box


On the other hand, Light induced CI-AFP was used with  tip at -0.5V negative bias as shown in fig 5(a). It was observed  that the 2 PU CARECs are showing a darker contrast, indicating a larger reverse bias leakage as compared to the  CARECs from neighboring good cells. A simple two point  nanoprobing between the two CARECs indeed revealed an  electrical short, as shown in fig 5(b), that would cause the cell  to fail. Further SEM inspection after wet etch observed a  silcided polysilicon residue at the STI region resulting in a  bridge between the 2 CARECs as shown in fig 6.


Fig.5 Light induced CI-AFP at -0.5V (a) showed distinct


contrast at 2CAREC. Nanoprobing confirmed short (b).


Fig.6 SEM image showing silicided polysilicon residue in STI  region causing bridge between 2 CARECs.


The same light induced current imaging was applied on  another similar SRAM failure where no abnormal contrast  was observed at contact level from conventional CI-AFP  analysis. Fig 7 showed the light induced CI-AFP scan with  small negative bias to the tip. It was evident that there was a  distinct darker contrast observed on both the CAREC and  VDD node as compared with other PU contacts. Further 2  point nano-probing verified CAREC-VDD short and SEM  inspection at poly and active layer revealed a minute poly  residue shorted the poly that was connected to the abnormal  CAREC to the VDD contact as shown in fig.8.


|(a) (b) ||
|---|---|

|Fig.3 SRAM layout (a) and Contact PVC image (b) failed cell (highlighted in red box). |of the |

要


甲0


*


中G宁


看


市


第可 of甲管警年


0


申中


号


Fig.7 Light induced CI-AFP at -0.5V showed distinct contrast  between CAREC and VDD


Fig.8 Poly residue resulting  in short between CAREC  and VDD.


The mechanism behind the contrast difference can be  attributed to the difference in the photovoltaic effect on the  shorted and non-shorted junctions. Fig.9 showed the current  density vs voltage (J-V) characteristics of a p-n junction in the  dark (black curve) and under illumination (blue curve) [4]. As  visible light impinges on the p-n junction, electron-hole pairs (E-H) are generated. These minority carriers flow across the  depletion region, resulting in open circuit potential difference, VOC, built up between the junction where p-type electrode is  positively charged while the n-type electrode is negatively  charged. The short circuit current density, JSC, can be


measured during AFP scanning when the tip comes in contact  with the junction and closes the circuit. Effectively, the  illuminated J-V characteristic of the junction is shifted down  by photo-generated current density, JPh, given by eqn (1) [5]


)


(


p


n


Ph


L


W


qG


J


+


=


(1) Where, G is the E-H pair generation rate dependent on the  light intensity, Ln and Lp is the minority carrier diffusion  length for electrons and holes respectively and W is the width  of the depletion region.


Fig.9 J-V characteristics of shorted and non shorted junction  with and without illumination


For the 2 memory failure cases described above, the bridge  due to the conductive defects would result in parallel  connections between 2 p+/nwell junctions as illustrated in  schematic diagram in fig 10.


Fig.10 Schematic of 2 p+/nwell junctions in parallel.


In typical reverse biased current imaging, the reverse  saturation current, 2Jo, at a small reverse biased voltage of the  shorted junctions remain too small to be detectable by the  system. In the forward bias scan, the large diffusion current


Contact


could easily mask out the difference between shorted and nonshorted junctions.  Thus, by comparing the difference in the  photo-generated current in the reverse bias condition, the


Poly


|Fig.14. Light induced CI- |Fig.15. STEM image |
|---|---|

|AFP at zero bias surfaced out |showing Poly shorted to |

|the leaky S/D node |contact |

contrast difference between shorted and non-shorted p+/nwell  junctions can be easily observed from the additional JPh on the  contacts of the shorted p+/nwell junctions as shown by the red  curve in fig 9 . This methodology can also be applied to logic  array but one has to take note of the complications from the  irregularities of the junction widths.


SCENARIO2: PV effect on gated and non-gated diode to  precisely localize logic Gate – S/D short


Following is a 28nm case where light induced CI-AFP  precisely localized gate – S/D short in a transistor array  structure. Electrical fault isolation identified an exclusive spot  at a transistor array in SRAM decoder which is shown in  fig11.


Fig.11 EMMI image showing spot at SRAM decoder.


Standard PFA approach was carried out with layer by layer  de-processing with SEM inspection and PVC analysis at CA  level, however no anomaly was observed.  The EMMI spot  was identified to be on a PMOS array and hence conventional  CI-AFP was performed with a positive bias (+0.5V ~ +1V) to  the AFP tip. Strong gate leakage was observed at the structure, shown in fig.13; however the leaky S/D had to be identified  through nano-probing. Light induced CI-AFP scan at zero bias  surfaced out the leaky S/D with distinctive contrast as shown  in fig.14. Further two point nano-probing between gate and  leaky node confirmed short. STEM image of a defect in core  logic with similar failure mode is shown in fig.15.


Fig.12. PMOS Transistor


array structure


Fig.13. CI-AFP showing  leaky gate at +0.5V bias.


Illuminated  PN Junction


o


SC


ph


oJ


J +


2


o J


Illuminated & shorted  PN Junction


Dark PN Junction


OCV√


Jo


▽立2Jo


Bridge:W_


Leaky Gate


Leaky S/D


The contrast difference between shorted and non-shorted  nodes can be achieved due to photovoltaic effect on gated and  non-gated junction. When visible light is illuminated on the  sample, E-H pairs are generated in both p+/nwell and nwell-psub junctions. Since the area of nwell–psub junction is bigger  than p+/nwell junction, the excess carrier(light induced  carrier) will be decided by nwell-psub junction. Therefore, excess electron will be induced in the nwell region. p+/well  junction can be treated as normal junction. While performing  an AFP scan across a normal S/D contact, it creates a path for  the excess electron to diffuse from nwell to p+ active as  shown in fig.16(a). This photo-generated current is reflected  as white contrast in current image.


Alternatively for a gated junction (gate-S/D short), the  ionized impurities in the nwell underneath the gate, will be  shared between p+ active and gate. This causes some field  lines from the nwell to terminate on the ionized P+ Active and  some to terminate on the gate, thereby reducing the junction  barrier [7]. While performing AFP scan on such a gated  junction, the amount of excess electron diffusing from nwell  to p+ active will increase in this region due to reduced  junction barrier as shown in fig.16(b). Therefore contrast  difference is achieved due the difference in amount of  electrons diffusion between a gated and non-gated junction.


Fig.16 Electron diffusion in an ordinary junction (a) and gated  junction (b)


Although the case study describes the scenario of single  poly gate transistor, we believe that the same method could be  used on multiple finger transistors, commonly found in logic  circuitry as shown in fig.17, to distinguish the defective gated  junction without going through tedious nanoprobing process.


Fig.17 Typical Transistor Array structure in logic circuitry  III CONCLUSION


The effectiveness of light induced CI-AFP to enhance  defect localization had been demonstrated in two different  scenarios where leakages could not be initially detected or  precisely localized through conventional CI-AFP. With the


results in hand, a successful effort was made to theoretically  understand the mechanism involved in achieving a significant  contrast difference at the leaky nodes with CI-AFP. A detailed  explanation on the mechanisms has been illustrated for each  case.


ACKNOWLEDGMENT


The authors would like to thank Product, Test and Failure  Analysis group for the constant support and encouragement to  experiment the technique with real time samples and actively  participate in results discussion to understand the mechanism. REFERENCES


1. Tom X. Tong et al, “Current Image Atomic Force  Microscopy (CI-AFM) combined with Atomic Force  Probing (AFP) for location and characterization of  advanced technology node”, Proc Int Symp Testing & Failure Analysis (ISTFA), pp 42-46, 2004.


2. C.Q. Chen et al, “Application of AFP on failure analysis  of 65nm technology SRAM”, Proc. Intl. Symp. Physical & Failure Analysis of Integrated Circuits (IPFA), pp148-151, 2011.


3. Multiprobe Inc., AFP Manual, P-EM-05 V4.0, July 2008.


4. Purnomo Sidi Priambodo et al, “Electric Energy  Management and Engineering in Solar Cell System, Solar  Cells - Research and Application Perspectives”,


244


4。


5. P. Würfel, “Physics of Solar Cells: From Principles to  New Concepts”, Wiley-WCH, Weinheim, 2005.


6. Roy. K et al, “Leakage current mechanisms and leakage  reduction techniques in deep-submicrometer CMOS  circuits”, Proc. of the IEEE, Vol.91, No.2 (2003), pp305-327.


7. Badih El-Kareh et al, “Silicon Devices and Process  Integration-Deep Submicron and Nano-Scale  Technologies”, pp277-286.


N-Well


P-sub


P+


ee-eeLight


ee-ee-e-eLight


e-e- Increased diffusion  due to reduced  junction barrier


“Detectability of automotive power MOSFET on-resistance failure at high current induced by Wafer Fab  process excursion”


Yann WEBER, Julien GOXE, Maris CASTIGNOLLES, Freescale Semiconducteurs France SAS, Toulouse


Product Analysis Lab, 134 avenue du Général Eisenhower, B.P. 72329, 31023 Toulouse Cedex, France


W. Rahajandraibe2, and J-M. Dutertre3


(1) STMicroelectronics, Rousset, France


(2) Aix-Marseille University Marseille, France


(3) Ecole Nationale Supérieure des Mines de St-Etienne, Gardanne, France


Continuous-Wave 1064 nm Laser for


Laser Voltage Imaging and Probing Applications  .............................................................. 335


Venkat-Krishnan Ravikumar1, Angeline Phoa1, Prasad Sabbineni2,  Dmitry Skvortsov2, and Ted Lundquist2


(1) Device Analysis Laboratory, Singapore


(2) DCG Systems Inc., Fremont, CA, USA


xvi


Development of DPA (Destructive Physical Analysis) Method for


Cu Wire Device  ............................................................................................................... 340


Hirohumi Tateyama, Wataru Shimizu, Hidehisa Kubota, Daisuke Murahara,  Tamiko Hattori, Naoki Ootani, Yujiro Yasuda, and Kazuhiro Yabe


Oki Engineering Co., Ltd., Japan


Failure Analysis Methodology on Resistive Open Defects  ................................................... 345


A.C.T. Quah, G.B. Ang, D. Nagalingam, C.Q. Chen, H.P. Ng, S.P. Neo,  J. Lam, and Z.H. Mai


Integrated ESD Robustness through Device Analysis of


Ultra-Small Low Voltage Power MOSFETs  ......................................................................... 350


Ian Kearney1 and Hank Sung2


(1) Texas Instruments, Bethlehem, PA, USA


(2) Texas Instruments, Dallas, TX, USA


Marginal Failure Diagnosed with LADA—Case Studies  ........................................................ 358


Sukho Lee1, Keonil Kim1, Yunwoo Lee1, Euncheol Lee1, Yojoung Kim1, and Izak Kapilevich 2


(1) Samsung Electronics Co. Ltd., Ki-hung, South Korea


Memory Address Verification Using NIR Laser  ................................................................... 365


Wilson Lee Cheng Hoe, Leena Saku, Ong Wei Kok, Yau Moi Kian, and Felix Yue Ren  Qualcomm Global Trading Pte. Ltd., Singapore


Metal Bridge Defects Localization by a Tiny Leakage between One of


Bridged Signals and VDD (GND)  ....................................................................................... 370


Chunlei Wu and Suying Yao, Tianjin University, Tianjin, China


Quantitative Analysis of Heterogeneous Materials by SEM/EDS by


Use of Rapid Phase Decomposition  .................................................................................. 374


John Konopka, Thermo Fisher Scientific, Madison, WI, USA


Safe Decapsulation Techniques Using Viton Caulk  ............................................................ 378


Kristopher D. Staller, Texas Instruments, Tucson, AZ, USA


Sample Preparation for High Numerical Aperture


Solid Immersion Lens Laser Imaging  ................................................................................ 383


M.S. Wei1, H.B. Chong1, S.H. Lim1, and C. Richardson2


(1) Advanced Micro Devices (Singapore) Pte. Ltd., Singapore


(2) Allied High Tech Products Inc., CA, USA


Static Fault Isolation on the Functional Failure Analysis  .................................................... 388


C.Q. Chen, Z.H. Mai, G.B. Ang, B.H. Liu, P.T. Ng, K.H. Yip, D. Khalid, and J. Lam  GlobalFoundries Singapore Pte. Ltd., Singapore


xvii


TDR Analysis on Short Transmission Lines  ........................................................................ 391


Nicholas Konkol, Intel Corporation, Hillsboro, OR, USA


Test Circuit Conditioning for Soft Defect Localization  ....................................................... 396


Kristopher D. Staller1 and Corey Goodrich2


(1) Texas Instruments, Tucson, AZ, USA


To Eliminate Curtain Effect of FIB TEM Samples by a Combination of


Sample Dicing and Backside Milling  ................................................................................. 400


Jian-Shing Luo and Hsiu Ting Lee; Inotera Memories, Inc., Taiwan, Republic of China


Ultra-Low Voltage Time-Resolved Emission Measurements from


32 nm SOI CMOS Integrated Circuits  ................................................................................ 416


Andrea Bahgat Shehata1, Franco Stellari1, Alan Weger1, Peilin Song1, Vikas Anant2,  Kristen Sunter3, Karl K. Berggren3, Ted Lundquist4, and Euan Ramsay4


(2) Photon Spot Inc., Monrovia, CA, USA


(3) Massachusetts Institute of Technology, Cambridge, MA, USA


(4) DCG Systems, Fremont, CA, USA


Sample Preparation and Device Deprocessing II


Application of Automated FIB for TEM Sample Preparation in


Semiconductor Failure Analysis  ...................................................................................... 413


Jie Zhu1, Soo Sien Seah1, Irene Tee1, Bing Hai Liu1, Eddie Er1, Si Ping Zhao1,  Jeffrey Lam1, Mark Najarian2, and Valerie Brogden2


(1) GlobalFoundries, Singapore


(2) FEI Company, Hillsboro, OR, USA


Productive Polishing TEM Sample Preparation Methodology Development  ........................ 420


Huisheng Yu, Shuqing Duan, Ming Li, Qihua Zhang, and Wei-Ting Kary Chien


Semiconductor Manufacturing International (Shanghai) Corp., Shanghai, China


Optimization of TEM Sample Preparation to Reduce the


Overlapping of TEM Images  ............................................................................................. 425


Shuqing Duan, Summer Chen, Paul Yu, Ming Li, Mark Zhang, and Kary Chien


Delayering on Advanced Process Technologies Using FIB ................................................... 430


Pete Carleson, David Donnet, Oleg Sidorov, and Chad Rue  FEI Company, Hillsboro, OR, USA


xviii


Case Studies and the Failure Analysis Process II


Failure Analysis Enhancement by Incorporating a


Compact Scan Diagnosis System  ..................................................................................... 436


Rommel Estores1, Pascal Vercruysse1, Karl Villareal1, Eric Barbian2,  Ralph Sanchez3, and Rich Ackerman3


(1) ON Semiconductor, Oudenaarde, Belgium


(2) ON Semiconductor, Phoenix, AZ, USA


(3) Teseda Corporation, Portland, OR, USA


Determination of the Source of an Electrical Overstress Event to a


Digital Variable Gain Amplifier Module  ............................................................................. 446


Thiri Htun and Steve Brockett, TriQuint Semiconductor, San Jose, CA, USA


Temperature-Dependent Logic Failure in a


GaAs Power Amplifier-Duplexer Module Caused by a


Subtle Parasitic Schottky Diode ....................................................................................... 450


Rose Emergo, Steve Brockett, and Pat Hamilton, TriQuint, Hillsboro, OR, USA


Debugging Phase-Locked Loop Failures in Integrated Circuit Products  ............................... 456


S.H. Goh, Wendy Lau, B.L. Yeoh, H.W. Ho, G.F. You, Hu Hao, Y.E. Koh, and Jeffrey Lam  GlobalFoundries, Singapore


Sample Preparation and Device Deprocessing III


A Novel Method for the Specified Site Planar View TEM Sample Preparation  ....................... 462


Shuqing Duan, Yanli Zhao, and Ming Li


Investigation of Protection Layer Materials for Ex-Situ Lift-Out


TEM Sample Preparation with FIB for 14 nm FinFET  .......................................................... 469


H. Feng, G.R. Low, P.K. Tan, Y.Z. Zhao, H.H. Yap, M.K. Dawood,


Y. Zhou, A.Y. Du, C.Q. Chen, H. Tan, Y.M. Huang, D.D. Wang, J. Lam, and Z.H. Mai  GlobalFoundries Singapore Pte. Ltd., Singapore


Application of Passive Voltage Contrast (PVC) to


Dual Beam Focused Ion Beam (FIB) Based Sample Preparation for the


Scanning/Transmission Electron Microscope (S/TEM)  ........................................................ 474


Corey Senowitz, Hieu Nguyen, Ruby Vollrath, Caiwen Yuan, Fati Rassolzadeh,  Theresa Graupera, Don Lyons, and Michael DiBattista


Qualcomm Incorporated, San Diego, CA, USA


Tri-Directional TEM Failure Analysis on Sample Prepared by


In-Situ Lift-Out FIB and Flipstage  .................................................................................... 480


xix


Will Tomorrow’s Failure Analysis Lab Operate More Like Today’s Fab?  ............................... 485


Todd Templeton and Valerie Brogden, FEI Company, Hillsboro, OR, USA


Defect Characterization and Metrology


Localization of Weak Points in Thin Dielectric Layers by


Electron Beam Absorbed Current (EBAC) Imaging  ............................................................. 491


Jörg Jatzkowski, Michél Simon-Najasek, and Frank Altmann


Fraunhofer Institute for Mechanics of Materials, Halle, Germany


Al-Cu Alloy Films Characterization and Studies Using TOF-SIMS,


XPS, AFM, EBSD and TEM ................................................................................................. 496


J.J. Shao, Y.Q. Shen, Y. Shen, Y.K. Zhou, K. Li, S.Y. Chou, Y.F. Liu, M. Hao,  W.W. An, Y.N. Hua, Z.X. Xing, and X.M. Li


Advanced Failure Analysis on Silicon Pipeline Defects and


Dislocations in Mixed-Mode Devices  ................................................................................. 502


Y. Weber1, J. Goxe1, S. Alves1, T. Zirilli1, M. Castignolles1, S. Subramanian2,  Y. Tsang2, and K. Harber2


(1) Freescale Semiconducteurs France SAS, Toulouse, France


(2) Freescale Semiconductor Inc., Austin, TX, USA


Foil Capacitor Characterization and Failure Analysis with


Special Respect to Noise Filter Applications  ..................................................................... 508


Peter Jacob


EMPA Swiss Federal Labs for Materials Testing and Research, Duebendorf, Switzerland


Sample Preparation and Device Deprocessing IV


TEM Sample Preparation Methods for MEMS Floating Structure Analysis  ............................ 515


Huisheng Yu, Shuqing Duan, and Ming Li


Cross-Section Sample Preparation Method for


Imaging Dopant Related Anomalies Using


Scanning Probe Microscopy Techniques  ........................................................................... 519


Swaminathan Subramanian, Khiem Ly, and Tony Chrastecky  Freescale Semiconductor, Austin, TX, USA


xx


Software-Based Techniques, Test, Diagnosis, and Yield


Design Debug for Intermittent Power up Failure in


Analog/ Mixed Signal Devices  .......................................................................................... 525


Sagar Karki, Oladele Sule, and You Zhihong  Texas Instruments Inc., DDAO, Dallas, TX, USA


A Case Study on the Benefits of Functional Memory Access during


ATE Test and Electrical Fault Isolation Techniques for Embedded SRAM  ............................. 528


Corey Goodrich, Texas Instruments, Inc., Dallas, TX, USA


Introduction to Verification and Test Using a 4-Bit Arithmetic Logic Unit


Including a Failure Module in a Xilinx XC9572XL CPLD  ....................................................... 533


Martin Versen and Michael Hayn


University of Applied Sciences Rosenheim, Rosenheim, Germany


Author Index  .................................................................................................................. 537


Defect Localization Enhancement using Light Induced CI-AFP


N. Dayanand, A.C.T Quah, C.Q.Chen, S.P.Neo, G.B.Ang, M. Gunawardana, Z.H.Mai, J.C.Lam  Product, Test, Failure Analysis Group, GLOBALFOUNDRIES Singapore


60 Woodlands Industrial Park D, Street 2, Singapore 738406


Phone No:(65) 6670-1508, Email: Dayanand.NAGALINGAM@globalfoundries.com


Abstract


This paper describes the effectiveness of using light  induced Current Imaging – Atomic Force Microscopy (CIAFP) to localize defects that are not easily detected through  conventional CI-AFP. Defect localization enhancement for  both memory and logic failures has been demonstrated. For  advanced technology nodes memory failures, current imaging  from photovoltaic effects enhanced the detection of bridging  between similar types of junctions. Light induced effects also  helped to improve the distinction between gated and nongated diode, as a result enhanced localization of gate to  source/drain short.


This paper presents the meaningful consequence of a minor Wafer Fab process variability, generating on-resistance (RDSon) drift on low voltage vertical power N-MOSFETs dedicated to microhybrid automotive application. The research challenge concerned the fact that failure was not detected  in production but at customer level; therefore, it was determinant to understand the root cause of this  failure mode to drive corrective actions in order to secure customer by detecting and delivering correct  parts. The originality of that paper concerns the necessity to use complementary Failure Analysis (FA) investigations, needed to determine the origin of the failure without any possibilities to perform any  fault localization. First, assembly investigations are presented to discriminate if the failure was coming  from customer or provider. Then, electrical characterizations at high current confirmed the RDSon  failure. Thus, strategic physical destructive FA approaches were combined in order to discriminate all  potential root causes, using physical step-by-step deprocessing, FIB milling cross-sections and TEM  analysis. Finally, a nanometric layer of oxide residue was identified as the origin of the failure and  corresponded to a wafer Fab process defect, induced by a lack of oxide overetch at spacer definition  process step. These results allowed implementing corrections and improving test screening to protect  customer.


Pulse generator and power supply


DUT


DBX


Meridian IV


Figure 1: Experimental setup used to characterize the new  DiamondBack eXtended (DBX) camera prototype in a  Meridian-IV system. DUT = Device Under Test.


Novel NIR camera with extended sensitivity and low noise  for photon emission microscopy of VLSI circuits


Andrea Bahgat Shehata, Franco Stellari, Alan Weger, and Peilin Song


IBM T.J. Watson Research Center, 1101 Kitchawan Rd, Yorktown Heights, NY 10598   abahgat@us.ibm.com, 914-945-2820


Herve Deslandes, Ted Lundquist, Euan Ramsay


DCG Systems, 3400 West Warren Avenue, Fremont, CA 94538


This work presents a new photon emission microscopy  camera prototype for the acquisition of intrinsic light emitted  from VLSI circuits during their normal operation. This novel  camera was designed to be sensitive to longer wavelengths in  order to maximize the signal intensities from modern VLSI  chips which are characterized by a red shift in the intrinsic  emission spectrum. In this paper, we will characterize the  performance of the camera using 32 nm and 22 nm SOI  chips. The novel camera is able to collect emission images  with the circuit under test operating at a supply voltage down  to 0.5 V, exceeding the performance of a state-of-the-art  InGaAs camera.


Introduction


Backside Photon Emission Microscopy (PEM) is commonly  used for circuit diagnostics and analysis of VLSI chips. Time-integrated emission images may be used for many  different applications: to localize anomalous emission spots  associated with failure mechanisms, to acquire logic state  maps for circuit debugging [1], to characterize chip  variability for yield improvement [2], to measure power  supply voltage droops [3], and more recently for circuit  security applications [4]. One of the main advantages of PEM  technique is the fact that it is a completely non-invasive  technique: it does not alter or damage the circuit under test.


However, with the continuous shrinking of integrated circuits, both in terms of power supply voltage and feature size, the  detection of the intrinsic photon emission is becoming  challenging. Reducing the operating voltage of the circuitry  leads to much fainter signal intensities in time-integrated


Meridian


emission images, that decreases as the exponential of the  reciprocal applied voltage [3][5]. Moreover, recent work  showed a red-shift of the emission spectrum towards longer  wavelengths [6]. Therefore, conventional detectors used for  emission microscopy, such as Si-CCDs or even InGaAs  cameras, are no longer a good option, given that they are not  able to detect a significant portion of the emission spectrum  due to their low cutoff wavelengths.


This paper presents the characterization of a new  time-integrated detector prototype with extended sensitivity  and low noise. This allows one to acquire time-integrated  images even at very low voltages – i.e. Vdd = 0.5 V – within a  few minutes. Performances of this new camera are compared  with those of a state-of-the-art liquid nitrogen (LN2) cooled  InGaAs camera, showing superior capabilities that can be  exploited to test future technologies of integrated circuits.


Experimental Setup


Fig. 1 shows our experimental setup with the novel PEM  camera (DiamondBack eXtended [7], DBX, developed by  DCG Systems) mounted on a Meridian-IV tool. The  1024 x 1024 pixel focal plane array is made of an extended  infrared material with sensitivity up to 2000 nm. This allows  the detection of the significant part of the VLSI circuits


SP 1600 nm


SP 1800 nm


SP 2000 nm


18000


9000


2 µm


9000、


12000


6000


Figure 2: Dependence of the detected intrinsic emission intensity from the chip on the cutoff wavelength of the short-pass filter used  in combination with the DBX camera and the SIL lens. 2D images, 3D plot, and emission profile along the dashed white lined and  gray planes are shown in the first, second and third row respectively.


emission spectrum that other cameras – e.g. InGaAs detectors


with λcutoff < 1600 nm – missed. The DBX camera is  cryogenically cooled with LN2 (~77 K) to reduce noise and  provide an adequate thermal shield. Inside the dewar, a set of  Short-Pass (SP) filters with different cutoff wavelengths λcutoff  can be used to set an upper limit to the incoming light  spectrum. Different lenses can also be used according to the  resolution desired for the PEM image: starting from a macro  1X lens, passing through 20X and 50X, to a 350X Solid  Immersion Lens (SIL). The board with the Device Under Test (DUT) is mounted on top of the Meridian-IV stage and  connected to power supplies and pulse generator.


DBX Characterization


The new camera was first tested in combination with the  different short-pass filters in order to optimize the cutoff  wavelength and obtain the best SNR in time-integrated  images acquired from VLSI circuits. Furthermore, we were  able to demonstrate that the camera is sensitive to emission  signals for circuit power supply voltages down to 0.5 V using  a 32 nm SOI testchip. We also directly compared the  performance of the new camera with that of a state-of-the-art  InGaAs camera. Finally we showed that, with this PEM  camera a nice emission image can be acquired from a 22 nm  SOI chip in only 10 seconds.


Time-integrated images with different short-pass filters


As a first characterization we checked that the emission  signal intensity acquired with PEM cameras gets stronger


when the sensitivity of the detector is extended to longer  wavelengths. To prove that, we used the DBX camera in  combination with the different short-pass filters and acquired  2D images from a 32 nm SOI testchip using the high  Numerical Aperture (NA) SIL. In particular, the DUT had an  inverter chain consisting of 7 stages, with 5 x 650 nm n-FETs (bottom inverter chain in Fig. 3). Time-integrated emission  images were acquired for Tacq = 30 s from the chip switching  at f = 100 MHz. Fig. 2 shows the 2D images (first row), together with the 3D plot (second row) of the emission  intensity and the profile along the n-FETs of the inverter  chain (third row). Note that the first emission spot  corresponds to a device in the driver section (see Fig. 3). As  expected, the signal intensity increases when the extended  spectral sensitivity of the DBX camera is exploited. One can  also observe a significant change of emission intensity  depending on the particular gate along the inverter line. This  is due to random process variations affecting the transistor  thresholds in this early version of the testchip, and such small  variations are amplified in emission images given the  exponential dependence of the emission intensity on the  voltage.


Sensitivity at very low voltage


The same testchip, consisting of inverter chains with FETs of  different sizes and spacing (Fig. 3a), was used to test the  sensitivity of the new camera down to very low voltages. To  this aim we used the SP filter that optimizes the SNR, i.e. the  one with λcutoff = 1800 nm (more details on SNR optimization  in the following section), and acquired the emission from the  chip running at a very low power supply voltage Vdd = 0.5 V  using the SIL for 10 minutes. Note from Fig. 3b how we are


0 200 400 600


1月5捌EP倒中


800 1000


Drivers


Inverter chains


1 2


9 10


a)


b)


Figure 3: a) Layout of the 32 nm SOI testchip used for DBX characterization, consisting of 10 inverter chains with different FETs’ dimensions and spacing between one inverter stage and the following one. b) PEM image acquired from the testchip running at  Vdd = 0.5 V, with only the two top and bottom inverter chains powered on, using the DBX camera in combination with the 1800 nm  short-pass filter. The image was acquired using the SIL for Tacq = 600 s. Note how emisison can be detected also from the smaller  devices.


2000 4000 6000 8000 10000


Emission ROI


Noise ROI


Figure 4: Example of PEM image acquired for the camera  comparison and definition of the Regions Of Interst (ROIs) for emission and noise for signal-to-noise ratio calculation.


able to detect the emission even from the smaller devices (single finger FETs 208 nm wide) in the testchip.


DBX vs. InGaAs camera comparison


The new camera performances were also compared to those of  a state-of-the-art InGaAs camera by acquiring emission  images from the testchip in Fig. 3a, running at different  operating voltages (i.e. from 1.2 V down to 0.5 V). To obtain  a fair comparison of the two cameras, we used the same  Meridian-IV optical system and the PEM images were  acquired through the same SIL.


For the purpose of this analysis, we define SNR as the ratio  between the emission intensity signal and the noise of the  measurement. In particular, the signal was defined as the  mean of the emission intensity collected by the camera pixels  from the second of the 7 n-FETs of the inverter chain (Fig. 4) minus the mean of the intensity in the noise area. The noise  was defined as the standard deviation of the pixel intensities  in an area of the same size of the previous one, but at a  location far from the Region Of Interest (ROI) defined for the  emission, where no emission is detected (Fig. 4).


Fig. 5 shows the results in terms of emission intensity signal (a), noise (b) and SNR (c) for the DBX camera, at different  voltages and with different short-pass filters. All the images


were acquired using a fixed acquisition time of 60 seconds to  simplify the comparison and rule out any acquisition time  non-linearity. As already shown in Fig. 2, the emission signal  intensity detected by the DBX camera improves when its


0.5 0.6 0.7 0.8 0.9 1 1.1 1.2


101 10


u(a.Noise std .)


Emissionean,E signal mM(a.u.)EAN


stdSNR=EMEAN/noise


103 104


Power supply voltage, VDD (V)


DBX, SP1600, TACQ = 60 s


DBX, SP1800, TACQ = 60 s DBX, SP1900, TACQ = 60 s DBX, SP2000, TACQ = 60 s


101


Power supply voltage, VDD (V)DBX, SP1600, TACQ = 60 s


100 101 102 103


Signal


Noise


SNR


Increasing λcutoff


a )                                                                    b)                                                                      c)


Figure 5: Emission intensity signal (a), noise standard deviation (b) and resulting signal-to-noise ratio (c) obtained with the DBX  camera and the SIL lens at different Vdd and using the different short-pass filters. Both the signal and the noise increase using  longer wavelength filters, but the SNR shows an optimum when the SP1800 filter is used. All the measurements were acquired using  Tacq = 60 s.


101 102 Emission sean, Eu.)ignal mMa.E(AN103 104


InGaAs, T ACQ = 60 s


InGaAs, T ACQ = 300 s InGaAs, T ACQ = 600 s


Noise std (a.u.)101


100 101 SNR=EMEAN/noise std102 103


Increasing Tacq


Figure 6: Emission intensity signal (a), noise standard deviation (b) and resulting signal to noise ratio (c) obtained with the InGaAs  camera and the SIL lens at different Vdd and using different acquisition times. Signal, noise and SNR increase using longer  acquisition times. At high Vdd the camera saturates if the acquisition time is too long.


sensitivity to longer wavelengths photons is exploited


(Fig. 5a). However, at longer wavelengths the camera is also  sensitive to thermal and blackbody radiation, and, as a  consequence, the noise level of the measurement increases  with λcutoff of the short-pass filter used (Fig. 5b). As a result, by progressively increasing the cutoff wavelength the  signal-to-noise ratio (Fig. 5c) initially starts to improve – due  to the increased emission signal detected – but then rolls off  due to the increased background noise. From this  characterization one can note how the SP1800 filter is the one  that optimizes the SNR of acquired PEM images. It should be  noted that higher power chip may reach a higher operating  temperature that would significantly increase the background


noise compared to the ambient. This may therefore affect the  best SNR conditions. On the other hand, using devices made  in a smaller technology node and with lower Vdd would push  the optimum SNR to longer wavelengths.


We used the same experimental setup to characterize an LN2  cooled InGaAs camera in the same experiment conditions. Such camera has an intrinsically lower cutoff wavelength (< 1600 nm) than the DBX due to the higher bandgap of the  III-V alloy used for the detector. Different acquisition times  were investigated, namely 60 s (in order to directly compare  the performances with those obtained with the DBX), 300 s  and 600 s. The results obtained with the InGaAs camera in


0.5 0.6 0.7 0.8 0.9 0.70.80.911 1.1 1.2


101 102 Emission sial mean, E.u.)gnMaEAN (103 104


DBX, SP1800, TACQ = 60 s InGaAs, TACQ = 60 s


InGaAs, TACQ = 300 s


InGaAs, TACQ = 600 s


DBX, SP1600, TACQ = 60 s，


一DBX, SP1800, TACQ = 60 s


InGaAs, TACQ = 60 s


InGaAs, T


Noise std (a.u.)


ACQ = 300 s InGaAs, T ACQ = 600 s


100 101/noise std102 103


Power supply voltage, VDD (V)DBX, SP1600, T


SNR =EANEM


ACQ = 60 s


DBX, SP1800, T


%


ACQ = 60 s InGaAs, TACQ = 60 s


Figure 7: Comparison of emission intensity signal (a), noise standard deviation (b) and resulting signal to noise ratio (c) obtained  using the DBX (solid lines) and InGaAs (dashed lines) cameras with the solid immersion lens. The DBX camera with the SP1600  leads a 2X SNR compared to the InGaAs camera with the same acquisition time (green dashed line) or to the same SNR 5X faster (compare black solid line and blue dashed line). The DBX with SP1800 allows to achieve even better performances in terms of SNR.


Table 1: Values of the signal-to-noise ratio for the InGaAs and DBX cameras. The improvement factor in SNR of the DBX with


respect to the InGaAs camera is also highlighted.


|Vdd (V) |Vdd (V) |Vdd (V) |0.6 |0.7 |0.8 |0.9 |1.0 |1.1 |1.2 |
|---|---|---|---|---|---|---|---|---|---|

|-.-|InGaAs, Tacq = 60 s |SNR |0.6 |3.7 |12.5 |34.7 |84.3 |191.2 |411.1 |

|---|InGaAs, Tacq = 300 s |SNR |1.7 |8.0 |27.5 |87.3 |192.3 |418.0 |624.3 |

||DBX, SP1600, Tacq = 60 s |SNR |1.4 |7.3 |21.9 |94.1 |161.6 |390.8 |972.2 |

||DBX, SP1600, Tacq = 60 s |Improvement factor wrt. InGaAs, Tacq = 60 s |2.3 |2.0 |1.7 |2.7 |1.9 |2.0 |2.4 |

||DBX, SP1800, Tacq = 60 s |SNR |8.0 |25.4 |73.1 |198.1 |367.2 |629.1 |1366.1 |

||DBX, SP1800, Tacq = 60 s |Improvement factor wrt. InGaAs, Tacq = 60 s |13.5 |6.9 |5.8 |5.7 |4.3 |3.3 |3.3 |

terms of emission signal, noise and SNR are summarized in  Fig. 6a, 6b and 6c, respectively. As expected, all these  quantities scale with the acquisition time. Note also how the  acquisition time is limited by the saturation of the camera at  high voltages (Fig. 6a).


Fig. 7 shows a comparison of the performances achieved with  the new DBX and the InGaAs camera. Here we show only the  results obtained with the DBX with two of the four short-pass  filters, i.e. SP1600 and SP1800. The former is the one that  mimics the InGaAs cutoff, while the latter is the one that  optimizes the SNR.


The DBX with SP1600 (black solid line in Fig. 7) is less  sensitive than the InGaAs camera with the same acquisition


time (green dashed line in Fig. 7), also because of reduced  transmission caused by the presence of the filter in front of  the DBX camera. However, the significantly lower noise of  the DBX allows for an SNR which is about 2 times better  than that of the InGaAs camera over the entire Vdd range (see  Table 1). The SNR achieved with the DBX combined with the  1600 nm short-pass filter is actually comparable with that  obtained with the InGaAs camera at Tacq = 300 s (blue dashed  line in Fig. 7), thus achieving the same SNR five times faster. If, instead, we compare the best performances obtained with  the DBX – i.e. with the SP1800 (purple solid line in Fig. 7) – with those obtained with the InGaAs camera, the SNR  improvement in comparison to the InGaAs measurement with  the same acquisition time (green dashed line in Fig. 7) is even


Figure 8: Emission image acquired from a 22 nm SOI chip  running at Vdd = 1 V. The image was acquired using the DBX  through the 20X lens and with an acquisition time of only  10 s.


better, being a factor 3 to 14 times higher depending on Vdd (see Table 1).


PEM images from a 22 nm chip


Time-integrated images were also acquired from a 22 nm SOI  chip operated at Vdd = 1 V. The PEM image in Fig. 8 was  acquired through the 20X lens with the DBX camera in only  10 seconds. It can be noted how, notwithstanding the short  acquisition time of only 10 seconds, a nice emission image  was obtained.


Conclusions


In this work we characterized the performances of a new  PEM camera prototype integrated in a Meridian-IV tool. The  extended spectral sensitivity of this novel camera allows the  detection of the longer wavelength portion of the chip  emission spectrum that other cameras – e.g. InGaAs cameras – are not able to collect. Thus the new camera is capable of  acquiring time-integrated images also at very low voltages (Vdd = 0.5 V) within 10 minutes. Through an extensive  characterization at different chip operating voltages we  compared the performances achievable with the new DBX  camera with those of a state-of-the-art InGaAs camera. Such  comparison shows that, thanks to the reduced noise of the  new camera, we are able to achieve the same SNR of an  InGaAs camera 5 times faster (i.e. with a 5X shorter  acquisition time) when we mimic the InGaAs cutoff using the


1600 nm short-pass filter. Results are even better when we  use the SP1800 that optimizes the SNR, obtaining a 14X  improvement at lower Vdd.


Acknowledgments


The authors would like to acknowledge and thank many other  people from IBM T.J. Watson Research Center and DCG   Systems for useful discussions, suggestions, and support, including: Herschel Ainspan, Seongwon Kim, Christian  Baks, Marc Taubenblatt, Mehmet Soyuer, Tom Kujawa, Dave  Schleh.


The project is supported by the Intelligence Advanced  Research Projects Activity (IARPA) via Air Force Research  Laboratory (AFRL) contract number FA8650-11-C_7105. The U.S. Government is authorized to reproduce and  distribute reprints for Governmental purposes  notwithstanding any copyright annotation thereon.


Disclaimer: The views and conclusions contained herein are  those of the authors and should not be interpreted as  necessarily representing the official policies or endorsements, either expressed or implied, of IARPA, AFRL, or the U.S. Government.


References


[1] F. Stellari et al., “Testing and diagnostics of CMOS  circuits using Light Emission from Off-State Leakage  Current”, IEEE Trans. on Electron Dev., vol. 51, no. 9, 2004, pp. 1455-1462.


[2] S. Polonsky et al., “Photon emission microscopy of  inter/intra chip device performance variations”, ESREF, 2005, pp. 1471-1475.


[3] S. Rusu et al., “Backside infrared probing for static  voltage drop and dynamic timing measurements”, ISSCC, 2001, pp. 276-277.


[4] P. Song et al., “MARVEL - Malicious Alteration  Recognitionn and Verification by Emission of Light”, HOST, 2011, pp. 117-121.


[5] A. Tosi et al., “Hot-carrier photoemission in scaled  CMOS technologies: a challenge for emission based  testing and diagnostics”, IRPS, 2006, pp. 595-601.


[6] U. Kindereit et al., “Near-infrared photon emission  spectroscopy trends in scaled SOI technologies”, ISTFA, 2012, pp. 128-134.


[7] N. Khurana et al., U.S. Patent 6825978.


Automated Mapping of Very Large Areas of VLSI Circuit using SIL


IBM T.J. Watson Research Center, 1101 Kitchawan Rd, Yorktown Heights, NY  stellari@us.ibm.com, 914-945-3223


In this paper, we present a novel system and method for the  automated mapping of pattern and spontaneous photon  emission from very large areas of VLSI circuit using Solid  Immersion Lens (SIL). To the best of our knowledge, this is the  first time that such a technique has been developed and  demonstrated on a real chip. The system being presented  includes an automation software Application Programming  Interface (API) to control the microscope used to acquire the  images, an acquisition software that allows to automatically  navigate the chip, move (hop) the SIL to the desired location, focus the image after the SIL landing, register the acquired  images, and stitch them together to create a high resolution  mosaic. In this paper, we will present, for the first time, a real  life example involving thousands of images acquired from a  90 nm bulk technology test chip that were used to create a  mosaic of more than 25 x 25 images covering a total area of  approximately 400 x 400 µm2.


For many types of applications, such as mapping systematic and  random process variations using Light Emission from Off-State  Leakage Current (LEOSLC) [1], security and reverse  engineering applications [2,3], images of large areas of the chip  may be necessary for extracting important information. However, the aggressive scaling of transistor dimensions as  well as the increase in chip size pose a challenge to these types  of emission acquisition. Since cameras have a limited number  of pixels, the spatial resolution is inversely proportional to the  Field Of View (FOV) of the optical system. In specific, if the  magnification of the optical system is increased to obtain a  suitable spatial resolution, the FOV is inevitably reduced as a  side effect. In performing diagnostics of high end products, we  have reached the point that the emission from the entire chip  cannot be acquired with a single acquisition even at the lowest  possible magnification offered by most optical microscopes [4]. To solve the previous issue in [4], we have developed for the  first time a method for automatically acquiring large sets of  images from different positions of a chip and then  mathematically stitching them together to create a highresolution image with a very large FOV. In the proposed  method, a set of overlapping images are acquired using air-gap  lenses following, for example, a raster scanning pattern. Adjacent images (in the X or Y direction) are acquired so that a  partial overlap is achieved. Obviously the overlap size needs to


be carefully selected to be large enough to guarantee accurate  registration of the images across the entire region of interest but  also small enough to reduce wasted overhead. For this reason, adaptive methodologies were considered: the overlap size is  adjusted during the image acquisition process to take into  account the content of current emission image (i-th) before the  stage is moved to the next ((i+1)th) partial overlapping image. After acquiring all the images, individual frames are stitched  together to form the final mosaic image.


In this paper, we present a significant extension of this  methodology to the use of Solid Immersion Lens (SIL) instead  of air-gap lenses. At best of our knowledge, this is the first time  that such a capability has been presented in a paper. The  capability of creating pattern and emission maps of very large  FOV with the ultimate lateral spatial resolution and coupling  efficiency of the SIL allows the monitoring of changes caused  by process variations, the identification of security threads, and  the reverse engineering at the gate and transistor level. Using  the SIL generates several very specific challenges that must be  overcome in order to control the landing and to obtain  overlapping frames (see next sections). Furthermore, a more  advanced image stitching algorithm had to be developed to deal  with high unpredictability of the stage movement during the  raster scanning. In the next sections, we will present the key  ideas of our method along with real life test cases acquired from  a 90 nm bulk test chip.


SIL mapping challenges


The most difficult challenges in creating mosaics using air-gap  lenses are mainly related to tracking the focus of the  microscope, guaranteeing a sufficient overlap between  neighboring images for registration, and stitching algorithms. In most cases, the focus challenge may be often overcome by  tilting the stage, when possible [4], or by implementing a Z  tracking interpolation with polynomial functions. In [1] and [4] we have also shown that simple first neighbor cross correlation  methods may be used to achieve good stitching results for an  area of up to about 1 in x 1 in when emission images are being  acquired.


The use of SIL intrinsically brings key additional challenges; some of which may be obvious to the typical user even during  manual operation. First, the accuracy of the landing position of  the SIL is, in general, not very good, especially when landing  the SIL from a lower magnification air-gap objective for the  first time. This particular problem makes “hopping” the SIL  from one position to the next following, for example, a raster


scanning pattern very imprecise so that the overlap of  neighboring images significantly changes from one step to the  next. Additionally, SIL “sticking” and stage drift may  contribute to create systematic, and sometimes difficult to  predict, deformation of the final area being scanned.


A second issue, related to the previous one, is maintaining good  focus from one SIL landing position to the next one. In fact, the  large majority of SIL objectives on the market rely on some sort  of spring loading between the SIL tip and a backing air-gap  objective. The distance between the SIL tip and the objective is  changed to achieve the best focus, while the spring mechanism  applies the desired pressure to guarantee a good solid contact  between the tip and the Silicon substrate. Due to the difficulty  of reproducing the same conditions reliably, in conjunction with  small variations in Silicon substrate thickness and surface  preparation quality, the best focal Z position may change from  one position to the next, along the raster scanning path. Thanks  to the large number of SIL images acquired using our proposed  system; we have found that, in most cases, a slow smooth trend  may be observed.


A third problem category relates to image distortion across the  FOV of the SIL that reduces the quality, resolution, and  coupling efficiency from the axis of the SIL towards the  periphery of the acquired image. Therefore simply stitching  neighboring images may lead to significant variations in the  quality of the final mosaic from one position to the next. As an  additional complication to this image quality problem, it should  be noted that the brightness and contrast of a measured pattern  images may also change significantly from one frame to the  next depending on the quality of the solid contact between the  SIL tip and the chip Silicon substrate.


Finally, we have found that more advanced image preprocessing, registration, and stitching algorithms were needed  to effectively deal with some of the aforementioned challenges, which could not be completely overcome by hardware  improvements, microscope control, and feedback.


In the next sections, we will present an overview of our  proposed method with a specific focus on the steps and  techniques involved in both precise microscope control and  automation, and image processing.


Microscope control and automation


Fig. 1 shows a diagram of the SIL mapping system. First, lower  magnification air-gap lenses are used to identify the area of  interest to be mapped using the SIL. In particular, the X and Y  range of coordinates is defined. Based on the knowledge of the  SIL FOV and requirements of neighboring image overlap for  stitching purpose, the number of images in X and Y directions  are calculated. A best strategy for covering the entire area is  defined, for example in a raster scan fashion as shown in Fig. 2. In most cases, an overlap of about 20%-30% between  consecutive neighboring images is recommended in order to  guarantee an acceptable number of correspondence points for  registration and enough image cropping to remove most of the  distortions introduce by the SIL across its FOV.


Depending on the specific microscope used, “hopping” the SIL


↓


from one position to the next may simply be achieved by  entering new coordinates into the stage controller. In our case,


the only way of moving the SIL is by using the mouse to point  to a new location, followed by a menu activation and


subsequent commands. Since a software API from the vendor  is also not available, we have developed the custom software


interface shown in Fig. 3, which runs in background and  interacts with the microscope controller by injecting custom


Fig. 1. Automated SIL mapping procedure.


Fig. 2. Example of raster scanning sequence for the SIL.


Fig. 3. Diagram of the automation layer, including the custom  tool interfaces and high level functions [4].


Identify region of interest using lower mag. lenses


Land SIL


Define map parameters


“Hop” and land the SIL


Improve contact with sample↓


Focus the SIL


Acquire pattern and/or


emission images


Map completed?


Process images


Register images


Stitch mosaic


No


Yes


1


3


Y


X


4


5


6


7


Analytical tools


Instrumentation


Custom interface


Layout browser


Autofocus Chip navigation


Automation layerExtensive data collectionand mappingLayout registration and advanced


data interpretation


1User input


个Requirements


Experiment


1conditions


commands into the controller message queue similar to what is  discussed in [4].


Once the tool automatic landing procedure has completed, but  before acquiring any pattern or emission image, the SIL is  adjusted to achieve a good solid contact. This reduces lateral  shift during the following automated focusing procedure and  delivers better quality images. In some cases, this can be  achieved by vibrating the SIL after it has made contact with the  chip. In other cases, the stage may be repeatedly moved up and  down, without loosing contact with the chip, to release any  lateral force accumulated during the SIL landing.


From a practical point of view, it is well known by users that  the Z stage position after landing the SIL may not yield the best  focus conditions, notwithstanding good chip planarity and  small lateral movement. In order to overcome this problem, which becomes more significant with larger area being scanned, an automated focusing procedure was developed. In [4] we first  proposed the use of a Figure Of Merit (FOM) based on the 2D  gradient to evaluate the focus quality of emission images. In this  case we further refined the algorithm to work with the specific  SIL image conditions and both reflected light and LSM pattern  images. In particular, the image acquired by the SIL has to be  pre-cropped to remove the perimeter that is most strongly  affected by distortion, which may cause undesirable bias of the  FOM. Furthermore, during our experiments we have found that  a preconditioning of the images may be useful to remove  artifacts such as bad camera pixels, cosmic rays (alpha  particles), etc that may end up in the image. Typically a disk or  Gaussian shaped low pass filter works well, leading to a  smoother FOM dependence on the stage Z position. In some  cased, the 2D gradient of the center portion of the image is  averaged to compute a single measurable parameter, in other  cases, the FOM may be calculated only inside specific subregions of the image where structures are present. Fig. 4 shows  a set of frames acquired at different Z focal position. For each  image, the FOM, measuring the focus quality is calculated as  shown in the graph. The best focus is chosen as the Z position  that yields the maximum value of the FOM.


After the best focus has been determined, the pattern image  corresponding to the best focus is saved for future stitching. If  needed, the emission image corresponding to the best focus  may also be acquired by first moving the stage back to the best  Z position and then acquiring and saving the emission image (it  should be noted that other types of analytical images may also


be acquired). Once all data has been collected for a particular  site of interest, the stage is moved to an adjacent site by “hopping” the SIL by an amount that allows a 20-30% overlay  with the starting location (significantly less overlap would be  necessary if the periphery of the acquired SIL image did not  have such a significant distortion). Fig. 5 shows two  consecutive sites where selected corresponding points have  been manually highlighted.


In our current implementation, all the images are saved locally  in a measurement folder on the controller computer and are  subsequently transferred to a secondary processing computer  that performs the image processing, registration, and stitching  as described in detail in the next section. In fact, we have found  that the use of separate computers does not slow down the  microscope controller and allows for much faster stitching  times. Depending on the stitching algorithm being used, a  partial stitching of the images could be performed after each  image to identify possible corrections in the SIL “hopping” steps sizes, as well as to perform feature recognition capable of  aiding the SIL navigation.


Using this custom API we have been able to acquire several  maps from VLSI chips consisting of several thousand’s of  separate locations with good results.


Image processing and stitching


After the dataset is acquired, we want to create a mosaic  combining all the individual frame into a single larger image. This is a challenging task since the images are not like normal  life pictures that have very distinct feature points. In our  previous work [5], we have shown a new method to generate a  mosaic for Transmission Electron Microscope (TEM) images


Z = 473 µm  FOM = 154.4


Z = 471 µm  FOM = 173.1


Z = 469 µm  FOM =  161.0


Z = 467 µm  FOM =  133.0


Z = 465 µm  FOM =  105.6


Fig. 4. Sequence of reflected light pattern images acquired during the automated SIL focusing. For each image, the focus quality is  measured using a figure of merit so that the stage Z position corresponding to the best focus may be identified.


X = 168 µm


X = 183 µm


Fig. 5. Example of consecutive measurement sites showing a  partial overlap and some corresponding points highlighted.


of VLSI circuits. In particular, the procedure to generate a  mosaic includes: finding corresponded points between adjacent  image tiles, refining corresponded points, estimating tile  configurations, and merging all images. However, this method  does not work very well for the SIL pattern images acquired in  this work. One major problem relates to the fact that some of  the images in the dataset do not contain circuit shapes. In fact, some images just show filler shapes consisting of many  identical and repetitive structures. These repetitive structures  create a lot of false positives during the process of finding the  corresponded points, as well as create missing corresponding  points that cannot be found. Ultimately, this causes an error  during the estimation of the stitching parameters, thus seriously  deteriorating the mosaic quality.


Based on the previous observation, it is easy to understand how  it is better to use only the correspondence points around the  circuit areas. In this way, more reliable positive  correspondences can be found. In order to achieve this goal, we  developed a selective analysis method to generate a salient map  for every frame in the dataset. First, the salient map highlights  the most important areas (in this case circuit structures) and  then only the correspondences on the important selected areas  are used to estimate stitching parameters using the method  described in [5].


The goal of the salient map is to identify non-repetitive  structures in the image, thus excluding the very repetitive filler  shapes. In particular, the process of creating a salient map  includes the steps listed in Fig. 6: calculating the gradient, generating the normalized Histogram of Gradient (HoG), finding correlations between adjacent normalized HoG, building a correlation map using mean and variance, and finally  creating the salient map representation.


The gradient of the image is used to analyze the repetitive  structure. To reduce the effect of random noise, a Gaussian filter  is applied before calculating the gradient of the image. The  angle and the magnitude of the gradient value are then used to  generate a normalized HoG with a number of bins Nb for every  pixel within a defined analysis window. To get the correlation  between the pixels, the HoG of every pixel is compared with


the HoG of its neighbor pixels, both horizontally and vertically. We use the following equation to calculate the correlation of  HoG R(s):


푅푥(푠) = ϑ(s푥,푦 , k)푁푏


푘=0ϑ(s푥−1,푦,


9(Sx-1jy,k)


k)


(1)


푅푦(푠) = ϑ(s푥,푦, k)푁푏


푘=0ϑ(s푥,푦−1, k)


(2)


푅(푠) = 푅 (푠) + 푅 (푠)


(3) where Rx is the horizontal correlation, Ry is the vertical  correlation, s is pixel position, the function θ is the normalized HoG, and k is an integer index used to scan the bin in the  analysis area. The mean and the standard deviation of the  correlation are then used to create a correlation map γ(s):


훾(푠) = 푒


( )


R(s)-R


(4)


where


푅


is the mean value of R(s), and σ is the standard  deviation of R(s). The correlation map is subsequently  convoluted with a disk filter to generate a new intermediate  function ψ(s). Finally, a threshold τ is applied to log(ψ(s)) to  generate a new map that undergoes dilation (a morphological  operation) to finally generate the salient map.


Examples


Fig. 7 shows a dataset of SIL images overlaid with the  corresponded salient map generated with the method above. The red color highlights show the salient areas containing  distinctive circuit shapes. This is in accordance with the  purpose of the salient map to indicate important (circuit) areas. Based on Fig. 7, we can see that all the circuit areas are  highlighted with the red color, thus validating our method. Only  a few salient maps show inaccurate estimations in empty areas. Only the corresponded points that are detected inside the salient  map are then used in the bundle adjustment algorithm to  estimate stitching parameters [5]. The remaining corresponded  points outside of the salient map are discarded. This allows to  weight more and use the corresponded point of regions of the  circuit that have more importance. In our experiment, we have  found that optimal values are Nb = 9, an analysis area equal to  16, and τ = 0.5.


Fig. 8 shows the stitching result (a) without using the salient  map and (b) with salient maps. One can notice that the result  obtained without using the salient map is distorted by the


Fig. 6. Salient map generation procedure.


Fig. 7. Image dataset with corresponded salient maps (red).


Image dataset


→


Calculate gradient


Generate normalized


histogram of gradients (HoG)↓


Find correlations between adjacent HoG


3.80


会


Create salient map representation


3 3 34


inaccurate stitching result. For example, the edges of  rectangular circuits on the left hand side and in the middle are  not straight. Instead, stitching results using our proposed  method shows a better fidelity without strong distortions.


Pattern example


Fig. 9 shows a low resolution (20X) reflected light pattern  image of a region of the chip containing a circuit of interest  spanning about 300 µm x 150 µm. In order to perform a detailed  analysis of the circuit, a map of the pattern at the highest  possible spatial resolution was needed. For this reason, multiple  SIL maps relying on our new proposed method were acquired  to achieve a full coverage (see colored rectangles in Fig. 9). Given the large number of images to acquire, the area was  broken down in four sub regions to reduce the risk of failed  maps and optimize the coverage for the circuit with uneven  shape.


The data in maps 1, 3, and 4 were used to create the large highresolution mosaic in Fig. 10. The image consists of more than  1,300 individual frames that cover an area of approximately  450 µm x 400 µm. The empty area on the left-middle region of  the mosaic is caused by the absence of circuit features in that  region. Since no corresponded points were detected in that area, no stitching parameters were estimated for the tiles on the area. Therefore, the empty area does not contain important  information. The high resolution image can provide a global  view of the circuit as well as fine details of the circuit gates.


Emission example


Although most of the examples and analysis so far presented  have been focused on stitching pattern images, our technique is  also effective for creating large mosaics of photon emission


*道20x(


口


Mapt


Fig. 8. Stitching result (a) without and (b) with salient maps.


Mupz "


Fig. 9. Low resolution (20X) reflected light pattern image of a  region of chip. Colored box indicate different SIL maps that  have been used to achieve full coverage.


Fig. 10. High resolution stitched mosaic consisting of >1,300  images covering an area approximately 450 µm x 400 µm.


Fig. 11. Zoom in detail of the mosaic in Fig. 10 gate level  resolution.


images and other types of data, including laser stimulation  images and Laser Voltage Imaging (LVI). In one  implementation of our method, both pattern and analytical data (e.g., spontaneous photon emission) are acquired concurrently. Typically, pattern images are used to focus the SIL at each  landing position due to their shorter acquisition time. Then the  emission image is acquired at the best focus position and stored  for later stitching. In some cases, the pattern images are first  used to register the individual frames and calculate the stitching  parameters, similarly to what was described before; then the  emission data is stitched into a mosaic using the same  parameters. In other cases, the emission data may be used  directly (especially if a pattern dataset is not acquired) to  calculate the stitching parameters. It should be noted that in this  last case, we do not need to use the salient map since the  emission is intrinsically limited to the active circuitry. However, median filters and background emission image  subtraction are often used to improve the image quality before  finding the corresponded points.


Fig. 12 shows a stitched emission image result consisting of  10 x 9 individual frames covering an area of approximately  150 µm x 150 µm.


Future work


Work is still ongoing to further improve the SIL mapping  system. In particular, live focusing using either pattern or  emission images is being considered as a replacement of the  current methodology that requires saving images at multiple Z  location in order to determine the best focus. While the new  method may allow the speed up of the focusing process, mostly  limited by the tool controller software, it may also reduce the  possibility of recovering, in case the focus is misjudged due to  corrupted images returned by the controller.


In general, one of the biggest challenges for the custom API  relates with handling unexpected behaviors of microscope as  well as errors in the controller software. For this reason, several  layers of error checking are required during each operation in  order to guarantee the smooth control of the tool and reduce the  risk of undesirable operations, especially when using the  delicate SIL tip. An optimization of these error checking  procedures should also lead to a faster mapping of the desired  area. Ultimately, we have found that the speed bottleneck  relates to the tool controller software and microscope lack of  speed and response time. In fact, one has to consider that it was  designed for human use corresponding to tens of SIL landing a  day, not hundreds of landing a day in a continuous fashion.


Two main areas of additional interest are related to stage drift  correction during SIL “hopping” as well as the use of this  technique to enabled automated probing by positioning a  certain feature of interest in the center of the FOV. In both  cases, a live analysis of the images will have to be incorporated  with feature recognition algorithms and automated layout to  pattern registration based on the small available FOV of the  SIL. The SIL tip used in our experiments has a special mounting  that allows it to conform to the chip tilt and tip up to about 2  degrees. Additionally, the automatic focusing of the SIL allows  to correct for slow bowing of the chip as well as tip and tilt  across the region of interest. During our experiments, we never  experienced any issue with the SIL crashing thanks to the fact  that the “hopping”, landing, and focusing of the SIL does not  bypass the internal safety features of the analytical tool.


In this paper, we have presented a novel system and method for  automated mapping of pattern and spontaneous photon


Fig. 12. Example of stitched emission mosaic consisting of 900 individual frames.


emission from very large areas of VLSI circuit using Solid  Immersion Lens (SIL). To the best of our knowledge, this is the  first time that such a technique has been developed and  demonstrated on a real chip. The system being presented  includes an automation software API to control the microscope  used to acquire the images, an acquisition software that allows  to automatically navigate the chip, move (hop) the SIL to the  desired location, focus the image after the SIL landing, register  the acquired images, and stitch them together to create the final  mosaic.


This technique allows us to acquire reflected light pattern  images, LSM frames, and spontaneous time-integrated or timeresolved photon emission from VLSI chips. It has been used to  automatically land and focus the SIL more than 4,000 times  acquiring more than 16,000 images that were composed into  stitched mosaics of several hundred images each.


Acknowledgements


The authors would like to acknowledge and thank P. Song, A.J. Weger, M. Taubenblatt, and M. Soyuer from IBM T.J. Watson  Research Center for useful discussions, suggestions, and  support.


This work supported by the Defense Advanced Research  Projects Agency (DARPA) under SSC Pacific contract  HR0011-11-C-0060. Any opinions, findings, and conclusions  or recommendations expressed in this publication are those of  the authors and do not necessarily reflect the views of the  DARPA or U.S. Government.


[1] F. Stellari et al., “Mapping systematic and random process  variations using Light Emission from Off-State Leakage”, Int. Symp. on Physics and Reliability (IRPS), 2009, pp. 640-649.


[2] P. Song et al., “Malicious alteration recognition and verification  by emission of light”, IEEE Int. Symp. on Hardware-Oriented  Security and Trust (HOST), 2011, pp. 117-121.


[3] F. Stellari et al., “Functional block extraction for hardware  security detection using time-integrated and time-resolved  emission measurements", VLSI Test Symposium (VTS), 2014, pp. 1-6.


[4] F. Stellari and P. Song, “Advanced methods and software for  enhancing analytical tools capabilities during chip diagnostic and  characterization”, Int. Symp. for Testing and Failure Analysis (ISTFA), 2012, pp. 273-280.


[5] C.-C. Lin et al, “Automatic Registering and Stitching of  TEM/STEM Image Mosaics”, Int. Symp. for testing and Failure  analysis (ISTFA), 2013, pp. 152-158.


Routine Device-Level Atom Probe Analysis


D.F. Lawrence, R.M. Ulfig, D.J. Larson, D.P. Olson, D.A. Reinhard, I.Y. Martin, S. Strennen, and P.H. Clifton


CAMECA Instruments Inc., 5500 Nobel Drive, Madison, WI USA


Continuing advances in Atom Probe Tomography and Focused  Ion Beam Scanning Electron Microscope technologies along  with the development of new specimen preparation approaches  have resulted in reliable methods for acquiring 3D subnanometer compositional data from device structures.  The  routine procedure is demonstrated here by the analysis of the  silicon-germanium source-drain region of a field effect


transistor from a de-packaged off-the-shelf 28 nm design rule  graphics chip. The center of the silicon-germanium sourcedrain region was found to have approximately 180 ppm of  boron and the silicide contact was found to contain both  titanium and platinum.


20 um


2um


Atom Probe Tomography (APT) has seen recent expanding (c)


(d)


interest and deployment in the area of semiconductor device


analysis [1-4]. Ever smaller device technology nodes and


yield/performance requirements have resulted in increasing


demand for the type of data that the atom probe can provide:


3D distribution of isotopic species at the atomic scale with


high detector efficiency (>75% of atoms identified in 3D) and


high sensitivity. This analysis performance is achieved by 500 nm


500 nm


preparing the sample in a sharp needle geometry, applying a  positive voltage on it such that atoms at the tip ionize and are  collected by a position sensitive single atom time-of-flight  detector [5].  The data is then reconstructed into a 3D atom  map that can be analyzed with any number of visualization or  numerical routines.  APT analyses of particular interest include  dopant distribution in the source/drain, extension, and  interfacial and channel regions of actual devices where other  common analysis techniques lack sufficient spatial or  compositional resolution [6].


Although APT is now being broadly deployed by seven of the  top ten semiconductor manufacturers in the world, it formerly  had been used primarily in a research and development role on  model devices, test structures, or unpatterned, blanket wafers


[8]. Analysis of a single, targeted device, such as a failure  analysis of a transistor with APT, has been rarely done  historically due to the complicated sample preparation  required and the relatively low data collection success rate on  complex 3D structures with many interfaces, particularly for  device specific analyses. Continuing advances in APT and  Focused Ion Beam (FIB) Scanning Electron Microscope


(SEM) technologies, along with the development of APT  hardware, software and advanced APT data collection  techniques have resulted in reliable methods for acquiring 3D  sub-nanometer compositional data on specific devices [2].


Figure 1 represents a modern standard specimen preparation  approach that has been employed to capture data from a  device.


Figure 1.  Illustration of the basic steps involved in standard  FIB-based preparation. (a) The first three FIB milling cuts  produce a wedge-shaped cantilever of material for attachment  to a micromanipulator. (b) A piece of the wedge shown in (a) has been attached to a silicon microtip using Pt. (c) and (d) show selected shapes of the specimen during the annular  milling process used to sharpen the specimen.


APT analysis of layered structures has been performed in a “top-down” orientation, where each layer is evaporated in  series. The major issues associated with this method are the  poor thermal conductivity and the various evaporation field  between the layers, which may result in sample fracture at the  transition.


Another method, called cross-sectional orientation method for  preparation of APT samples has been developed. First, a  standard, normal orientation lift-out wedge is transferred and  mounted to a microtip post. The wedge is then carefully  thinned to <30 nm using standard TEM lamella preparation  techniques described elsewhere [7]. The captured devices of  interest are clearly visible in cross-section. The microtip array  carrying the thinned wedge is then removed from the FIB and


capped with ~300 nm of conformal CVD polysilicon to 2a)


2b)


provide a buffer material for FIB APT tip preparation. The  encapsulated lamella is then returned to the FIB. Sections of  the lamella are next transferred to microtip posts.  Finally,


行联


each mounted section is sharpened with an annular milling  pattern so that the specimen tip is <200 nm at the region of  interest (ROI) [7]. This method results in evaporation of the


1um


5 um


layers in parallel, rather than in series, which is helpful in  thermal dissipation of heat during APT analysis,


2c)


2d)


The challenge for both above methods is the amount of time  required to complete each, and their lack of site specificity. It  normally takes weeks to complete a device analysis (from  sample preparation to APT analysis). Here we report a new  method of site specific sample preparation for APT utilizing a


10 um


novel backside ROI targeting method. Combining this new  sample preparation methodology along with the latest  hardware and software in Atom Probe Tomography, we can  improve test efficiency and enable true failure analysis work  with an APT system within days.


Technique


To demonstrate the new single-device sample preparation and


analysis technique, a 28 nm technology node device (AMD


Radeon™ R7 graphics card) was purchased from a retail outlet


and analyzed. The chip was de-packaged and processed in the 3a)


3b)


FIB SEM.  In this case, the specimen was analyzed from the  substrate side (backside), but the device specific marking was  done while still being able to identify features with the metal  mask above the ROI.  By conducting the APT analysis from  the substrate side of the device, complicated and weak  interfaces are kept outside the high stress region at the tip. This new approach significantly improves analysis success  rates.


5um


3c)


3d)


Figure 2a shows the de-processed wafer at M2 level.  A single  device was chosen to target for analysis, but it is important to  note that any device visible in the figure could be chosen with  this technique (e.g. those identified to be of interest by  electrical or other testing technique).  Fiducial holes cut with  the FIB around the ROI and are then refilled.  The holes will  provide high contrast to the silicon substrate as the sample  preparation procedure progresses.  Figure 2b shows the thick


250nm


layer (approximately 3 microns) deposited directly over the  fiducials and the ROI.  This layer is used later as the  attachment handle to the carrier for sample to be introduced  into the atom probe.  Figures 2c and 2d show standard wedge  creation and lift-out performed with an in-situ  micromanipulator [5], followed by wedge transfer to a  manipulator stage with rotation capability.


Figure 2.  (a) De-processed wafer at M2 level, with fiducial  holes cut with the FIB around the ROI, (b) ~3 m Pt  deposition (this will become the base region of the removed  wedge, once rotated 180 degrees), (c) the wedge extraction  cut, (d) handing the plucked wedge over to a secondary, axialrotation manipulator.


After transfer to the micromanipulator, the wedge is rotated 90  degrees followed by FIB low angle milling to reveal the four  fiducial markers that were created from the de-processed M2  side, as shown in Figure 3a.


Figure 3.  (a) rotated 90 degrees, backside milling reveals the  backside of the fiducial holes , (b)e-beam Pt deposition marks  the ROI, protecting it from subsequent mounting (c) and final  annular milling and finishing (d).


Figure 3b shows the ROI as marked with a FIB deposited  platinum cap which will be the tip of the sharpened APT  specimen.  The wedge is rotated again for a total of 180  degrees to orient the substrate pointing up and is shaped in the  FIB such that a wedge is created that will be put in contact  with a silicon microtip post (Figure 3c) which can be inserted  into the APT using a standard spring clip stub.  Standard  annular milling is then used to reduce the radius of the tip  under 100 nm such that sufficient electric field can be


generated to cause field evaporation of the transistor in the  atom probe. The finished tip is illustrated in Figure 3d.


The specimen was analyzed in a LEAP 5000 XR system from


123


CAMECA instruments Inc. using the latest control software  that improves laser targeting and field evaporation control and  thus improves the ability to collect data from a complicated  device reliably.  This in combination with the site specific  backside sample preparation technique outlined above has  allowed for a 60% yield improvement, where the region of  interest is successfully analyzed with sufficient data quality to  provide valuable feedback.


20 nm


Data Analysis


Figure 4 shows a cross-section SEM image of the test device.


Si Ge Ni Ti Pt


The region of interest is marked in red square. Using our site  specific backside ROI targeting method, described above, we  prepared the APT sample.  The APT data were reconstructed  using IVAS 3.6.8™ and simple inspection of one of the  resultant images in Figure 5 reveals the target region was  successfully analyzed and contains a SiGe source-drain region  as well as both titanium and platinum in the nickel-silicide  contact.


Figure 4.  A cross-section SEM image example of the target  region analyzed, outlined in red.


Figure 5.  A view of the SiGe region of the device (the channel  region is to the right).  Sub-volume analysis was done on the  SiGe region, the interface of the SiGe to the channel, and the  channel.


Figure 5 also shows the APT dataset, with three sub-volumes  and related spectra shown in Figures 6 and 7. The APT data  indicates that the area in the center of the source/drain contains  180 ppm boron concentration, the area spanning the silicongermanium and the channel contains 50 ppm boron  concentration, and the area under the channel has a  concentration of boron which is below the detection limit for  the chosen sub-volume size.


Si


1e3


Count高sub-volume


1e1?C


aldanduhdal mn10.0 10.5 11.0 11.5 12.0 12.513013519014515.0 15.5


Mass-to-Charge-State Ratio (Da)


hold


visible for this


B: no peak


1e4


Figure 6.  Mass spectra of the channel region (Region 3 from  Figure 5) demonstrating the presence of carbon, but no  detection of B above the detection limit.


Figure 7.  Mass spectra of the SiGe (Regions 1 and 2 from  Figure 5) and the SiGe-channel interface demonstrating the  clear detection of B in the SiGe region.


New sample preparation techniques and the latest hardware  and software in FIB SEM and APT systems improve time to  knowledge and enable true failure analysis work with an APT  system.  Prior to site specific backside ROI targeting methods, single specific device analysis generally took weeks to  achieve. It is now possible to complete this type of analysis  within days.


The authors would like to thank all of our colleagues at  CAMECA Instruments Inc. who assisted in assembling the  materials presented in this manuscript, especially J. Bunton, D. Lenz, T. Payne, E. Oltman, and J. Watson.


Region 1


[1] Kelly, T.F., et al., "Atom Probe Tomography of


B:0.018%


Electronic Materials", Annual Review of Materials


untCoB180ppm


Research, 37 (2007),  pp. 681-727.


[2] Lauhon, L.J., et al., "Atom-Probe Tomography of  Semiconductor Materials and Device Structures", MRS  Bulletin, 34(10) (2009),  pp. 738-743.


1e0


10.0 10.5 11.0 11.5 12.0 12.5 13.0 13.5 14.0 14.5 15.0 15.5


[3] Larson, D.J., et al., Atom Probe Tomography for


Microelectronics, in Handbook of Instrumentation and  Techniques for Semiconductor Nanostructure


Region 2


Characterization, R. Haight, F. Ross, and J. Hannon, Editors. (World Scientific Publishing/Imperial College  Press, 2011): London.


untCo1e21


50ppm


B:0.005%


[4] Mutas, S., et al., "Investigation of the analysis parameters  and background subtraction for high-k materials with


B


atom probe tomography ", Ultramicroscopy, 111 (2011),


1e0m也山


pp. 546-551.


[5] Larson, D. J. et al., Local Electrode Atom Probe


15.0 15.5


Tomography, Springer, (New York, 2013) pp. 318.


[6] Vandervorst, W., “Dopant/carrier Profiling for 3DStructures,” Phys. Status Solidi C, Vol. 11, No. 1 (2014), pp. 121-129.


[7] Larson, D. J. et al. From the Store Shelf to Device-Level  Atom Probe Analysis:  An Exercise in Feasibility. in 189–197 (ASM International, 2011).


[8] McClean Report, IC insights 17 (2013).


High-Resolution Backside GMR Magnetic Current Imaging                              on a Contour-Milled Globally Ultrathin Die


D. Vallett


PeakSource Analytical, LLC, 287 Buck Hollow Road, Fairfax, VT  05454, USA


J. Gaudestad


Neocera, LLC, 10000 Virginia Manor Road, Beltsville, MD  20705, USA


C. Richardson


Allied High Tech Products, Inc., 2376 East Pacifica Place, Rancho Dominguez, CA  90220, USA


Magnetic current imaging (MCI) using superconducting  quantum interference device (SQUID) and giant-magnetoresistive (GMR) sensors is an effective method for localizing  defects and current paths [1]. The spatial resolution (and  sensitivity) of MCI is improved significantly when the sensor is  as close as possible to the current paths and associated magnetic  fields of interest. This is accomplished in part by nondestructive removal of any intervening passive layers (e.g. silicon) in the sample.


This paper will present a die backside contour-milling process  resulting in an edge-to-edge remaining silicon thickness (RST) of < 5 microns, followed by a backside GMR-based MCI  measurement performed directly on the ultra-thin silicon  surface. The dramatic improvement in resolving current paths  in an ESD protect circuit is shown as is nanometer scale  resolution of a current density peak due to a power supply shortcircuit defect at the edge of a flip-chip packaged die.


Fault isolation continues to be an increasingly critical step in  the debug and failure analysis of complex ICs and devices [2]. Starting as a method of localizing only short circuits, MCI has  evolved into a versatile suite of techniques for isolating also  leakage currents, resistive opens, and complete opens in 2, 2.5, and 3D assemblies, as well as imaging current paths for design  validation and counterfeit detection [3]. As with any technique  however the need for improved spatial resolution is constant as  circuit dimensions and defects continue to shrink in size and  devices grow in thickness and complexity [4].


A unique attribute of MCI compared with other image-based  fault isolation methods is that magnetic fields from sub-surface  defects and current paths deep within a device pass to the  surface unperturbed. Properties of materials commonly used in  microelectronics like absorption, thermal conductivity, diffraction, doping, dielectric constant, etc. that adversely  impact transmission of other energy forms (i.e. light, heat, electric field, and electron/ion beam) do not affect passing  magnetic fields from conductors buried within and beneath (while these materials do possess finite magnetic permeability, their magnitude is close enough to the free-space constant as to  be comparable with air or vacuum and are thus negligible).


As such, MCI is among the small number of fault isolation  methods capable of non-destructive image-based electrical fault  isolation of deeply buried defects and current paths. For 2.5 and  3D packaged components, discretes, and PCBs specifically, where thick opaque films render other techniques ineffective, MCI is one of only two tractable image-based fault isolation  methods (the other being lock-in thermography or LIT).


While magnetic signals are easily imaged through thick films  there is a resolution penalty imposed by the separation distance  between the current and the sensor [5]. Both peak resolution (the ability to localize the center of a point-source current  density signal) and spatial resolution (the ability to differentiate  neighboring current paths) are affected by this distance. There  are two components to the sensor-current separation: a) the  sensor to surface scanning height; and b) the current depth  below the surface. The sensor to surface height is minimized by  precise automated scanning of the SQUID or GMR sensor over  the sample and is fixed by the magnetic microscope system. So  reducing the surface to current depth by non-destructive  removal of passive materials above magnetic field sources  enables closer scanning and, therefore, improves resolution (and sensitivity).


The resulting resolution improvements of such close-proximity  scanning using a GMR sensor from the frontside of a die have  been shown previously [6]. During backside examination of a  flip-chip packaged die the substrate silicon is essentially a  passive film. The benefits of full or partial-area backside silicon  thinning and removal are well known [7, 8]. A key concern in  silicon thinning, however, is the in-situ die deformation caused  by inherent stresses in the package [9]. This often results in die  curvature at the start of, and/or during, the thinning process as  increasing removal of silicon allows stress relief and possible  device damage. As such, a precise and automated non-planar, edge-to-edge silicon thinning and removal process is highly  desirable to provide a smooth surface with little to no remaining  silicon for the closest possible non-destructive scanning of a  proximal probe sensor such as a GMR [4].


Prior work in this area has examined the effects of thinning by  mechanical polishing to random, incidental silicon thicknesses (i.e. not intentional edge-to-edge removal of silicon to a  specified target thickness) on MCI’s ability to resolve current  paths in the die and its interposer [10].  This paper will show  the dramatic resolution improvements after silicon removal by  edge-to-edge contour-milling in: a) resolving current paths over


a relatively large area in an ESD protect circuit; and b) in  localizing an intentionally created point-source power short.


A 2-Ampere over-current was introduced into a power supply  pin of a standard BGA packaged, 265 micron thick, 65 nm  technology node flip-chip device with a 4.8 ohm short circuit  defect resulting. SQUID-based MCI was then performed over  the full-thickness silicon backside while supplying 35 uA  ACRMS to the short (5.9 nW effective heating value dissipated  power) and also with 600 uA ACRMS to a random forwardbiased ESD protect circuit. All MCI measurements were carried  out on a Neocera Magma C30 system.


The backside silicon was subsequently thinned using an Allied  High Tech X-Prep and X-Prep Vision using a two-step process    to achieve < 5 microns RST uniformity across the entire die (Fig. 1). Non-planar contours are commonplace in the die  surface and obviate the use of planar milling or polishing  techniques as the center of the die tends to be destroyed prior to  the edges achieving desired thickness. To accomplish full-die  uniform thinning the backside device contours were first  measured on the milling system to create a contour map for the  machining tool to follow.  This is enabled by following a  predefined grid determined by a combination of the die and tool  diameter. The physical device profile is then visualized offline  for reference. The bulk silicon removal was next performed  with a “flat-top” grinding methodology followed by the contour  re-introduction with a fine grit diamond bonded milling tool to  within 65 µm of the desired RST target [11]. Stopping within  65 µm of the final target thickness ensured there was enough  silicon left for device relaxation correction and polishing to the  desired final surface finish.


Figure 1: Two-step silicon contour milling process.


A new RST profile was collected on the same grid that was  defined from the measurement of the original physical contour, thus providing data on how the device relaxed during the bulk  thinning process. Correction software was used to modify the  original physical milling profile map to reflect the changes due  to die/package relaxation. The corrected profile was then used


to mill within 25 microns of the final target thickness. The final  25 microns of material removal was accomplished with a  sequential process of decreasing diamond polishing  compounds, polishing cloths, polishing patterns and calibrated  low forces to achieve a mirror finish sufficient for throughsilicon imaging (also compatible with a solid immersion lens or  SIL). With the backside silicon thus removed, the active  circuitry is exposed immediately below the surface for repeat  MCI using a GMR sensor that scans directly on the smooth  silicon (Fig. 2).


For GMR scanning a current of 600 uA ACRMS was driven to  the ESD circuit with 48 uA ACRMS (11 nW) supplied to the  power short. MCI images using the SQUID sensor pre-thinning  were then compared with GMR images taken post-thinning.


Measure Starting Physical Contour


Results and Discussion


Remove Bulk Material


Mill to Corrected Contour


The initial SQUID-based MCI measurement of the ESD protect


Within 50μmNo


Within 25 μmNo


circuit through the full-thickness silicon substrate shows widely


of final target?


dispersed current to a relatively large area with no distinct  features visible (Fig. 3). It should be noted that while the 600


?Yes


uA ACRMS supplied divides over a large region for a lower


Measure RST


Polish To Desired Mirror Finish


overall current density, the high-sensitivity SQUID has plenty  of signal with negligible background noise to detect the lower


Create CorrectedContour Map


Final targetNo


magnitude localized currents. The signal however is lacking in


(X-Correct)


thickness?


业


detail owing to > 400 µm current-to-sensor separation


↓Yes


component imposed largely by the intervening silicon.


*Indicates optional step


Validate RST Measurement *


Pre-thinning SQUID measurements of the power supply short  through the full-thickness silicon do show a well-localized  current-density near the edge of the die (Fig. 4). While the peak  signal is quickly and easily pinpointed well above any noise, it  is lacking in detail, also because of the > 400 µm separation  distance between the SQUID and the current. Still, under these  conditions the peak can be localized to +/- 3 µm as referenced  to the optical image.


Figure 2: Final contour-milled die surface thinned to < 5  microns RST.


Repeat MCI measurement of the ESD protect circuit now using  the GMR sensor scanned on the ultrathin silicon surface shows  much greater detail (Fig. 5). Individual current paths are clearly  visible highlighting topology beneath the surface that was not  discernible using the SQUID through the full-thickness  substrate.


Post-thinning MCI of the power supply short using the GMR


8.9 mm


also shows significantly greater definition (Fig. 6). The much  smaller GMR sensor active area (~ 50 nm vs. ~ 30 um for the  SQUID), its ability to scan in very close proximity to the  sample, and increased scanning precision enable conductive  paths sourcing and sinking current to and from the defect, respectively, to be resolved with still only 48 uA ACRMS of  current supplied (11 nW dissipated power). More importantly it  is now possible to localize the peak current density signal to a  diameter of approximately 250 nm.


Figure 4: SQUID-based MCI image of power supply short  with surface profile (inset) of current density signal.


Figure 5: GMR-based MCI image of current density in the


900 X(μm)


ESD protect circuit from the ultrathin silicon surface (top)


1800


with SQUID reference image (inset); and surface profile (bottom).


1.0 mm


556


Figure 3: SQUID-based MCI image of current density in an


1.0mm


< 287


ESD protect circuit through full thickness silicon.


Z(au)


Y(μm)


900


84


Conclusions and Future Work


Backside SQUID-based MCI was performed through a fullthickness silicon flip-chip die to image current in a relatively  large-area forward biased ESD protect circuit and to localize a  low-resistance point-source power supply short circuit. MCI  was repeated with a GMR sensor scanned directly on the


surface of the same device after silicon removal to < 5 microns  RST using global contour-milling.


The work shows the advantages of a non-destructive edge-toedge silicon removal process which accounts for varying stressinduced warpage and resulting contours in multilayer devices. It also highlights the significant improvements in MCI  resolution gained by non-destructively exposing active circuitry  immediately below the surface for GMR scanning. Of particular  importance is the simultaneous demonstration of approximately  250 nm peak resolution with nano-Watt sensitivity achieved by  combining magnetic current imaging with contour milling.


Previous publications have analyzed MCI vs. other common  fault isolation techniques (i.e. PEM, LSM/TIVA, LIT, and  liquid crystal) [12-14]. These results however are dated and/or  limited in scope, examining only SQUID-based MCI and


Q


looking at specific defect types in just a few different sample  form-factors. Updated comparisons using the significant new  capabilities announced here will advance the body of


knowledge of the application, limitation, and performance of  image-based fault isolation techniques.


[1] Knauss, L., et al., “Scanning SQUID Microscopy for  Current Imaging,” Microelectronics Reliability, 2001, 41


250 nm


(8), pp. 1211-1229, Elsevier Ltd.


>*-


[2] Chin, J.M., et al., “Recent Advances in Fault Isolation for  Semiconductor Industry,” Proceedings of the 20th Int. Symp. on the Physical and Failure Analysis of Integrated  Circuits (IPFA), July, 2013, IEEE.


[3] Vallett, D., “Magnetic Current Imaging Revisited,” Electronic Device Failure Analysis (EDFA), 2014, 16 (4), (to be published) ASM International.


[4] Vallett, D., “Fault Isolation Challenges and Opportunities  for Proximal-probe Imaging,” Proceedings of the 19th Int. Symp. on the Physical and Failure Analysis of Integrated  Circuits (IPFA), July, 2012, IEEE.


[5] Chatraphorn, S., et al., “Noise and spatial resolution in  SQUID microscopy,” IEEE Trans. Appl. Super-cond.,


4um


vol.11, no.1, pp.234–237, March 2001.


[6] Gaudestad, J., et al., “High resolution Magnetic Current  Imaging for Die Level Short Localization,” Proceedings of  the 20th Int. Symp. on the Physical and Failure Analysis of  Integrated Circuits (IPFA), July, 2013, IEEE.


[7]  Perdu, P., et al., “Comparative Study of Sample  Preparation Techniques for Backside Analysis,” Proceedings 26th Int. Symp. Test. and Failure Analysis (ISTFA), 2000, ASM International.


[8]  Boit, C., et al., “Physical Techniques for Chip-Backside IC  Debug in Nanotechnologies,” IEEE Design & Test of  Computers - Special Issue on Silicon Debug and Diagnosis, 250-257, 2008, IEEE.


[9] Richardson, et al., “Contoured Device Sample Preparation  Technique for +/- 5 µm Remaining Silicon Thicknesses that  Meets Solid Immersion Lens Requirements,” Microelectronics Reliability, 53(9-11); 2013, Elsevier Ltd.


Figure 6: GMR-based MCI image of power supply short  current density from ultrathin silicon surface (top) and  SQUID reference image (inset); with thresholded peak  signal (bottom).


[10] Hechtl, M., “Backside GMR Magnetic Microscopy for Flip  Chip and Related Microelectronic Devices”, Proceedings of  the 15th Int. Symp. on the Physical and Failure Analysis of  Integrated Circuits (IPFA), July, 2008, IEEE.


[11] Richardson, C., et. al., “Putting the Die Contour Back - Methods in Advanced Sample Preparation for 3-D and FlipChip Devices,” Proceedings of the 20th Int. Symp. on the  Physical and Failure Analysis of Integrated Circuits (IPFA), July, 2013, IEEE.


[12] Vallett, D., “Scanning SQUID Microscopy for Die Level  Fault Isolation”, Proceedings 28th Int. Symp. Test. and  Failure Analysis (ISTFA), 2002, ASM International.


[13] Vallett, D., “A Comparison of Lock-in Thermography and  Magnetic Current Imaging for Localizing Buried ShortCircuits,” Proceedings 37th Int. Symp. Test. and Failure  Analysis (ISTFA), 2011, ASM International.


[14] Schmidt, C, et. al., “Enhanced Comparison of Lock-In  Thermography and Magnetic Microscopy for 3D Defect  Localization of System in Packages,” Proceedings 38th Int. Symp. Test. and Failure Analysis (ISTFA), 2012, ASM  International.


Resolution Improvement through Sparse Image Reconstruction Techniques for Dark  Field Subsurface Microscopy of Integrated Circuits


T. Berkin Cilingiroglu, W. Clem Karl, Janusz Konrad, Michael D. W. Grogan, Abdulkadir Yurt, Ahmet Tuysuzoglu, Bennett B. Goldberg, and M. Selim Unlu


Departments of Electrical and Computer Engineering, Materials Science and Engineering, Physics Boston University, 8 St. Mary's  Street, Boston, Massachusetts, 02215, USA


Back-side fault isolation and failure analysis of Integrated  Circuits (ICs) must meet the challenges of increasing  component density and smaller length scales [1]. The highest  possible resolution is achieved by imaging through silicon  substrate using aplanatic solid immersion lenses (aSILs) with  effective numerical apertures (NA) approaching the index of  the substrate (NA ~ 3.5) [2]. In order to accurately understand  the behavior of tightly focused light in such high NA systems, we need to move beyond a scalar model and consider the  vector nature of light [3]. In high NA condition, the ref  reflected light from the silicon-dielectric interface is high in  magnitude due to total internal reflection. Additionally, the  magnitude of scattered light from objects in the dielectric  medium scales with the sixth power of the radius of the  objects, resulting in low magnitudes for small objects. Therefore, in high NA is that the reflected light from the  silicon-dielectric interface is comparable in magnitude to the  scattered light from small objects in the dielectric medium, resulting in low contrast images. In order to increase the  contrast of images, a polarization-sensitive dark-field  microscopy is proposed and modeled that successfully  suppresses the strong background reflection and increases both  contrast and resolution [4].


Sparse image reconstruction techniques have been previously  used to recover high frequency information lost during  acquisition process in different imaging domains, such as  ultrasound [5], synthetic aperture radar [6], optical microscopy


GM0=o1=LP


[7], and astronomical and microscopic imaging [8]. We have  proposed frameworks applying these techniques to high NA  microscopy images in [9,10]. These frameworks combine


det↓↑


←☑二QWP


prior knowledge about ICs with physics-based optical forward  model and recover high frequency information, which is  typically lost in low-resolution observations. In this work, we


一


propose a signal processing framework in order to estimate the  Point Spread Function (PSF) of the dark-field subsurface


pinholecollimated


beamresolution target


aSIL &


microscopy system from observation data. We incorporate this  PSF into an image reconstruction framework, which can be  formulated with two different image reconstruction  techniques, regularized image reconstruction and dictionarybased image reconstruction. Both of these techniques take  advantage of prior knowledge about ICs. We demonstrate on  experimental data that dictionary-based image reconstruction  provides better image enhancement and higher resolution.


Dark Field Subsurface Microscopy for  Integrated Circuits:


The goal of dark-field subsurface microscopy is to increase  resolution and contrast by suppressing the strong background  reflection. We modify an aSIL confocal microscope by adding  a linear polarizer and a quarter wave plate prior to the  objective lens to allow us to selectively filter the background  light that has specularly reflected from the dielectric interface  of silicon and low-index medium (see Fig. 1). This simple  implementation of the polarization sensitive optics allows us  suppress the background creating a dark-field image. Fig 2  shows a comparison from a typical confocal and our dark-field  subsurface confocal microscope images of aluminum lines  fabricated on a double-side polished silicon wafer. In the  typical case, there is a strong reflection from the background, which diminishes the visibility of the features significantly as  shown in Fig. 2a. In the dark-field case, the specularly  reflected circularly polarized light is filtered after traversing  the quarter wave plate and the linear polarizer. The resulting  image is largely free of background and the visibility of the  small features is enhanced significantly. The technical details  of this method can be found in [4]. In this work, we apply  image reconstruction frameworks on such background filtered  subsurface images of ICs in order to improve resolution.


Fig. 1 The confocal microscope setup. (Collimated beam from  1310 nm laser; GM – galvanometric mirror; LP – linear  polarizer; QWP – quarter-wave plate; aSIL – aplanatic solid  immersion lens; pinhole is 10 µm.)


Image Reconstruction Framework:


The image reconstruction framework is composed of two  steps. The first step involves the estimation of the PSF of the  system from observed images. In the second step, we  formulate an image reconstruction framework using the  estimated PSF in a linear forward model. In this framework, we apply regularization terms in order to incorporate prior  information about the features of interest.


We propose two different formulations for image  reconstruction, they differ in how prior knowledge about the  integrated circuits is incorporated into image reconstruction  framework. The first formulation assumes that IC images are  sparse and they are composed of piecewise constant regions. This assumption relies on ICs being composed of small lines  and small rectangular structures. We can incorporate this  information into reconstruction framework while using nonquadratic regularization functionals in the image  reconstruction formulation. Therefore, we can preserve the  sparsity and the edges of the underlying features. This type of  image reconstruction for IC Imaging has been previously  proposed [9]. Our second approach uses the computer aided  design (CAD) layouts in order to build an overcomplete set of  dictionary of rectangular building blocks, which vary in their  size and in their location. Then, this dictionary can be  incorporated into a sparse image reconstruction framework. A  dictionary–based image reconstruction framework for IC  imaging is proposed in [10].


Fig. 2. (a) Metal lines separated by 252 nm, 282 nm on a  resolution target, imaged using 1310 nm circular polarization  with no linear polarizer in the return path. (b) The same set of  metal lines imaged with the linear polarizer and quarter wave  plate in place. (c) The intensity profile corresponding to  dashed lines in (a) and (b). The red line is with circular  polarized illumination from (a), and the black line is with  Dark Field Microscopy from (b)


PSF Estimation and Observation Model:


When the PSF of the system is unknown, blind deconvolution


[11] is used as the conventional image reconstruction  technique. In blind deconvolution, both the PSF and the  reconstruction are estimated from observation data iteratively. Another approach is to predict a sharp version of the blurry  image and to use the two images to solve for a PSF [12]. In  this section, we explain how we estimate the PSF of the  optical system and how we employ this PSF in order to  formulate an optical forward model. The cross sections (examples of cross section locations can be seen in Fig. 3) along the lines from the center part can be used in order to  estimate the Line Spread Function of the system. We collect  multiple cross sections from different lines in the observation  and we fit a spline to the average of these cross sections using  a least squares spline approximation. The derivative of this  estimated function will give us the estimated Line Spread  Function of the system. However, since the lines are thin, boundary effects result in spurious artifacts in the waist of the  estimated LSF. In order to filter these imperfections, we  approximate the LSF with an airy disk. We assume that this is  the estimated 1D PSF and since the system can be assumed to  be isotropic, this airy disk can be rotated to obtain the 2D PSF  of the system. Hence, the assumed linear observation model of  the system becomes:


g(x, y) = ĥ(x, y)* f (x, y) ,


(1) where g x, y( )  is the observed intensity,


€


f x,y( )  is the


intensity of the underlying object, * denotes the convolution  operation, and ĥ x, y( )  is the estimated PSF of the optical  system.


In practice, the data we collect is discretized in spatial  coordinates on a uniformly spaced grid and Eq. 1 becomes:


g = Ĥf,


where g is the vectorized discrete observation data, f is the  discrete underlying object image,  Ĥ  is the Toeplitz matrix  that implements convolution as a matrix operation based on  the estimated PSF.


.s


0.4


0.3


月


0.2


01


a


204060o100


140150110200


shaes


Fig. 3. How cross sections are taken in order to estimate the  LSF of the system


sO 8


(c)


Regularized Image Reconstruction:


The underlying features in ICs have smooth, homogeneous  and sparse structure. This preliminary knowledge can be  incorporated in the reconstruction by employing non-quadratic  regularization functionals. The regularized reconstruction can  be formulated as the following optimization problem:


f̂ = argmin


f


J f( ),


(3)


where,


J f( ) = Ĥf − g22+ λ1 Df1+ λ2 f1,  (4)


and D is the discrete approximation to the gradient operator  that computes first-order image differences in horizontal and  vertical directions. The second and third terms in Eq. 4 are  regularizers that favor sparsity in the edge field of the  reconstructed image and the sparsity in the reconstructed  image, respectively. The optimization problem in Eq. 4 is  solved using the quasi-Newton method, which has been  explained in detail previously [6,9].


Dictionary-based Image Reconstruction:


The structures in ICs consist of flat regions consisting of  horizontal and vertical lines of constrained and varying width  and length. The width and length of these lines are easily  derivable from CAD layouts. Therefore, the application of  overcomplete dictionaries in an image reconstruction  framework becomes particularly suitable for IC imaging  domain. We can construct an overcomplete dictionary from  building blocks derived from CAD layouts. These building  blocks are rectangles of varying width and length and all  possible locations of these rectangles are included into the  dictionary. More detail about how to build this dictionary is  explained in [10].


Then, the unknown underlying scene f can be represented as: f = Φα,


(5)


where Φ is the appropriate overcomplete dictionary and α is  the vector of representation coefficients. Now, we can  estimate the underlying IC scene by solving the following  optimization problem:


α̂ = argminαĤΦα − g22+ λ α1,


(6)


where λ is a regularization parameter that determines the  overall level of problem sparsity. We are using the interior  point algorithm [13] in order to solve the optimization  problem. The estimated underlying scene will be:


f̂ = Φα̂.


(7)


Fig.4. (a) The dark field subsurface microscopy image (b) SEM image of metal aluminum lines separated by 252 nm, 224  nm and fabricated on a double-side polished silicon wafer


Fig. 5.(a) Average of cross sections from the center of lines  and Least-squares spline approximation to this average (b) The estimated LSF which is the derivative of the least-squares  spline approximation and the airy disk fit to this estimated  LSF


Fig. 6. The estimated PSF of the system


(b)(b)


−100 −50


50


100


0.1


0.5


0.6


0.7


pixels


Average of cross sections


Least−squares spline approximation


Normalized Intensity


0.8 1


Airy disk fit


Estimated LSF


Experimental Results:


In Fig. 4, the dark field subsurface microscopy image of a  resolution target and its corresponding Scanning Electron  Microscope (SEM) image are shown. The resolution target is  composed of metal aluminum lines separated by 252 nm and  224 nm, and fabricated on a double-side polished silicon  wafer. The average of cross sections from center parts of lines  and the least-squares approximation of this average are shown  in Fig 5(a). The derivative of this approximation gives us the  estimated LSF of the system, which is shown in Fig. 5(b). However, since the lines are thin, at the end of the lines we  observe boundary effects and this causes errors at the waist of  the LSF. Therefore, we fit an airy disk to this estimated LSF (Fig. 5(b). The estimated PSF of the system, which is obtained  rotating this airy disk, is shown in Fig. 6.


The next step is to incorporate this PSF into two image  reconstruction formulations in order to improve the resolution  and quality of the observed image. In Figures 7,8 and 9, we  show the observation and the results of two image  reconstruction techniques for 252 nm spaced vertical lines, for  224 nm spaced vertical lines and for 224 nm spaced horizontal  lines, respectively. Both techniques improve the resolution of  observation data. In the case of 252 nm spaced lines, there are


10 lines, although we can count these 10 lines in observation, they are sharper and clearer in reconstruction results. In the  case of 224 nm spaced lines, there are 12 lines and we cannot  count them in the observation. In the reconstruction results of  224 nm spaced vertical lines, we can clearly count 12 lines. This shows that we improve not only edge resolution, but we  also improve isolation. We can see in the SEM data that there  are some fabrication imperfections in 224 nm spaced  horizontal lines. For this reason, we could not recover all 12  lines after image reconstruction of 224 nm spaced horizontal  lines. However, the location of the fabrication default actually  corresponds to blurred region in the dictionary-based image  reconstruction of 224 nm spaced horizontal lines. One of the  resolution metrics used for IC Imaging is a sparrow resolution  criterion. The Sparrow criterion defines the resolution as the  distance between the peaks of the two point sources when the  midpoint just becomes visible. Similarly, we can evaluate if a  resolution structure is resolved or not, in other words, if a  structure is localized or not, depending on whether we observe  a peak. We are able to observe exact number of peaks in lines  with 224 nm spacing after resolution improvement while exact  number of peaks was observed in lines with 252 nm spacing  for experimental data. This shows at least 12 % resolution  improvement.


Fig. 7. Vertical lines with 252 nm spacing (a) Observation (b) Regularized Image Reconstruction (c) Dictionary-based Image  Reconstruction


Fig. 8. Vertical lines with 224 nm spacing (a) Observation (b) Regularized Image Reconstruction (c) Dictionary-based Image  Reconstruction


0.8


0.9(b)1


0.5 1


1.5 2


2.5 3


3.5 4


4.5


1.2


1.4


1.6


(a)(a)


(c)(c)


0.9


2.5


1.8


Fig. 9. Horizontal lines with 224 nm spacing (a) Observation (b) Regularized Image Reconstruction (c) Dictionary-based Image  Reconstruction


In this work, we proposed an image reconstruction framework  in order to improve the resolution of dark-field subsurface  microscopy. Within this framework, we applied two different  sparse image reconstruction techniques with different levels of  assumed prior knowledge - regularized image reconstruction  and dictionary based image reconstruction. Both techniques  provide at least 12 % resolution improvement; we are able to  localize lines with 224 nm spacing after resolution  improvement while lines with 252 nm spacing are at the limit  of localization in experimental data. However, dictionarybased image reconstruction provides higher edge resolution  and maintains the homogeneity of the intensity within the  structures.


The work presented in this paper was supported by the  Intelligence Advanced Research Projects Activity (IARPA) via Air Force Research Laboratory (AFRL) contract number: FA8650-11-C- 7102.


[1] K. A. Serrels, E. Ramsay, R. J. Warburthon and D.T Reid, “Nanoscale optical microscopy in the vectorial focusing  regime,” Nature Photonics. 2, 311-314 (2008).


[2] F. H. Koklu, J. I. Quesnel, A. N. Vamivakas, S. B. Ippolito, B. B. Goldberg, and M. S. Unlu, “Widefield  subsurface microscopy of integrated circuits,” Opt. Exp., 16(13), 9501, (2008).


[3] L. Novotny & B. Hecht, “Principals of Nano-Optics,” Cambridge University Press (2006).


[4] A. Yurt, “subsurface optical microscopy of semiconductor  integrated circuits,” Ph.D. dissertation, Boston University, Boston, USA, 2014.


[5] A. Tuysuzoglu, J. M. Kracht, R. O. Cleveland, M. Cetin, and W. C. Karl, “Sparsity driven ultrasound imaging,” The Journal of the Acoustical Society of America, vol. 131, no. 2, pp. 1271–1281, 2012.


[6] M. Cetin, et al, “Feature-enhanced Synthetic Aperture  Radar Image Formation based on Nonquadratic  Regularization,” IEEE Transactions on Image  Processing, Vol. 10, No. 4 (2001), pp. 623-631.


[7] S. Gazit, A. Szameit, Y. C. Eldar, and M. Segev, “Superresolution and reconstruction of sparse sub- wavelength  images,” Opt. Express, vol. 17, no. 26, pp. 23 920–23  946, Dec 2009.


[8] E.F. Hom, F. Marchis, T.K. Lee, S. Haase, D.A. Agard,


and J.W. Sedat, "AIDA: an adaptive image deconvolution  algorithm with application to multi-frame and threedimensional data," J Opt Soc Am A Opt Image Sci Vis.


2007, 24(6), 1580-600.


[9] T. B. Cilingiroglu, F. H. Koklu, E. Ramsay, Y. Lu, A. Yurt, W. C. Karl, J. Konrad, B B. Goldberg, M. S. Unlu, “Image Reconstruction Techniques for High Numerical  Aperture Integrated Circuit Imaging,” ISTFA 2012.


[10] T. B. Cilingiroglu, A. Tuysuzoglu, W. C. Karl, J. Konrad, B B. Goldberg, M. S. Unlu, “Dictionary-based  Image Enhancement for Integrated Circuit Imaging,” IEEE International Conference in Acoustics, Speech and  Signal Processing (ICASSP), May 2013.


[11]  Q. Shan, J. Jia, and A. Agarwala, “High-quality motion  deblurring from a single image,” ACM Trans. Graph., 27 (3), 2008


[12]  N. Joshi, R. Szeliski, and D. J. Kriegman, “PSF  estimation using sharp edge prediction,” IEEE  Conference on Computer Vision and Pattern Recognition (CVPR), 2008


[13] S.-J. Kim, K. Koh, M. Lustig, S. Boyd, and D. Gorinevsky, “An Interior-Point method for large-scale l1-Regularized Least Squares,” IEEE Journal on Selected  Topics in Signal Processing, vol. 1, no 4,pages 606–617,


2007.


1.5


3.5(c)


3D IC/Stacked device Fault Isolation using 3D Magnetic Field Imaging


A. Orozco*, N. E. Gagliolo, C. Rowlett, E. Wong, A. Moghe,  J. Gaudestad, V. Talanov


Neocera, LLC, 10000 Virginia Manor Road, Beltsville, MD, 20705, USA


A. Jeffers, K. Torkashvan, F. C. Wellstood


Center for Nanophysics and Advanced Materials, Department of Physics, University of Maryland, College Park MD,20742


Stephan Dobritz and Mathias Boettcher


Fraunhofer IZM-ASSID, Ringstr. 12 01468 Moritzburg, Germany


A. B. Cawthorne


Department of Science and Mathematics, Trevecca Nazarene University, Nashville, TN 37210


F. Infante


Intraspec Technologies, 3 avenue Didier Daurat, 31400 Toulouse, France


The  need  to  increase  transistor  packing  density  beyond Moore's Law and the need for expanding functionality, realestate  management  and  faster  connections  has  pushed  the industry to  develop  complex  3D package technology which includes  System-in-Package  (SiP),  wafer-level  packaging,through-silicon-vias (TSV), stacked-die and flex packages.


These  stacks  of  microchips,  metal  layers  and  transistors have caused major challenges for existing Fault Isolation (FI)techniques and require novel non-destructive, true 3D Failure Localization techniques. We describe in this paper innovations in  Magnetic  Field  Imaging  for  FI  that  allow  current  3D mapping  and  extraction  of  geometrical  information  about current  location  for  non-destructive  fault  isolation  at  every chip level in a 3D stack.


As a way to keep packing transistors in ever reducing space,the Semiconductor industry has started stacking transistors in 3D, the so called “More than Moore” (MtM) [1]. In addition,the need to expand functionality, real-estate management and faster connections has pushed the industry to develop complex 3D  package  technology,  which  includes  System-in-Package(SiP), wafer-level packaging, through-silicon-vias (TSV), and stacked-die and flex packages among others. This complex 3D geometry, with abundance of opaque layers and interconnects presents a great challenge for fault isolation (FI) and failure analysis (FA) [2].


The challenges that 3D integration present to FA require the development  of  new  FI  techniques  that  allow  for  nondestructive, true 3D failure localization.


3D Magnetic Field Imaging (MFI)


Magnetic Field Imaging (MFI), the mapping of current in devices  by detecting  the  magnetic  field  they  generate,  was


introduced  in  1998  using  a  Superconducting  Quantum Interference Device (SQUID) [3].From its early application to detect short circuit failures, it has grown to a full capable tool for  detection  of  all  static  failures:  shorts,  leakages,  high resistance and open circuit failures [4]. Giant-magnetoresistive sensors have been added to complement the SQUID allowing high resolution capability for die-level FI.


The  signal  injected  (DC  and  AC  of  few  kHz  for shorts/leakages detection or RF up to few 100 MHz for open failure  detection)  in  the  circuit(s)  under  study  generates  a magnetic  field.  This  magnetic  field  is  detected  by a  sensor positioned above the device. The sample is raster scanned and its magnetic field is acquired at multiple predetermined steps providing an  image of  the  magnetic  field  distribution.  This magnetic  field  data  is  typically  processed  using  a  standard inversion technique [5, 6] to obtain a current density map of the device.  The resulting current map can then be analyzed,compared to a circuit diagram, an optical/infrared image, or a non-failing part to determine the fault location. A description of the technique and the applications to FA can be found in the literature,  including  extensive  discussion  and  tests  of  its capabilities and limitations [7-14].


Magnetic field imaging is a natural candidate for 3D FI of complex 3D interconnected devices. This is because the lowfrequency magnetic field generated by the currents in the DUT is unaffected through the vast  majority of materials used in device  fabrication  as  they  are  non-ferrous;  the  presence  of multiple metal layers, dies or other opaque layers do not have any impact on the magnetic field signal.


A serious limitation with the standard inversion technique is that,  in order to compute the current  based on the acquired magnetic data, it is assumed that all currents are confined to a single plane [5,  17].  Although this is  a  good assumption in many  situations,  this  is  a  2D  technique  and  the  vertical information  is  lost.  Nonetheless,  it  has  been  successfully applied to 3D devices in some situations [3, 15-17].


Generalizing  this  to  a  3D  problem  is,  unfortunately  not possible.  It  can  be  easily  demonstrated  that  there  are  an


infinite number of possible solutions to the generic 3D inverse problem. Details about the limitations of the 3D capability of the standard technique can be found in the literature [5, 6, 17].


By  imposing  reasonable  constraints  on  the  current  paths compatible with typical device fabrication and after exhaustive analysis  of  the  magnetic  field  signal,  it  was  proved  by  us[18,19] that it is  possible to extract the 3D current path based on acquired magnetic field images of metal structures using a new  solver  rather  than  the  standard  inverse  method.  To summarize,  we  have  developed  an  algorithm  capable  of successfully  reconstructing  a  3D  current  path  based  on  an acquired  magnetic  field  image.  The  generally  intractable problem  has  been  reduced  to  a  manageable  problem  by carefully constraining the search.


Two main questions remained:  first  what are the ultimate practical  limits  of  this  technology and  second,  how does  it handle  real  devices.  In  this  paper,  we  examine  these  two questions and present results on 3D Magnetic Field Imaging to real 3-die TSV and multi-layered structures.


Magnetic Field 3D Solver resolution capability


3D MFI capability can be quantified in terms of vertical and


Optical Scan (top of sample)


lateral resolution. How the resolution is affected by the depth of the device needs to be addressed as well. To do this, we need  devices,  ideally  3D  IC  consisting  of  at  least  4 interconnected dies, each one at most 10  m thick. As these


devices do not exist  yet,  we fabricated a device resembling these geometries by constructing 3D metallization structures


--layer 1#


Magnetic Scan


on top of passivation blocks. The devices where fabricated by


→- layer 2


3DiS Technologies.


layer 4=


回


zCurrent path cross-section


-layer 3


Figure  1. 3D  multi-layered  structures  used  to  quantify resolution  capability  of  the  novel  3D  MFI  technique fabricated by 3DiS Technologies.


Fig.  1  shows  SEM  images  of  two  of  the  structures fabricated.  Pattern  1  (Fig.  1(a))  is  a  linear  via  chain  with current vertically meandering through the different layers as


shown in more detail in the insert. Fig. 1(b) shows pattern 4, a XYZ-meandering structure.  As seen in the inset, the current runs  through  all  4  layers  while  meandering  in  X  and  Y directions.  The  layer-to-layer  separation  is  5  m.


Manufacturing limitations at the time of fabrication restricted the minimum metal trace width to 20  m. Metallization was Cu/Au of total thickness around 1 m.


The  devices  were  scanned  in  a  3D-modified  commercial magnetic field imaging system. Fig. 2 shows the result of the scan  and  3D  analysis:  Top  Fig.  is  an  optical  scan  image showing the section of the linear via chain scanned. Different blocks visible correspond to different layers. Middle image is a magnetic scan image. Red and blue represent magnetic field coming  out  and  coming  into  the  scan  plane,  respectively.


Overlaid on this image, although barely noticeable, is the 3D current map obtained through the 3D solver. We use a color scheme to identify the different layers the current is located at,as shown on the inset to the left. Finally,  the bottom image shows a cross-section view of the 3D path along the via chain.


This image clearly shows that  the 3D solver can accurately assign different current sections to the corresponding layers.


+z


Figure  2.  (Top)  Optical  scan  from  top  of  the  sample.


(Middle) Magnetic scan with computed 3D path overlaid. A color scheme (inset at left) is used to designate the vertical


3DS Tahnoia0i6e-2013


layers for the current with layer 1 the closest to the sample


surface and the sensor. (Bottom) Cross-section view of the 3D  path  showing  the  proper  layering  structure  of  the current.


Fig. 3 shows a more clear representation of the 3D mapping results. Top two images refer to pattern 1, the linear via chain.


Top image  is  the  optical  image with each  segment  colored according to the layer location. Bottom image uses the same


0305 Technologies-2012


socum


optical image but the colors follow the results of the 3D solver layering assignment. It is ease to notice the accuracy in layer identification.  Besides,  lateral  positioning  of  the  current  is excellent and better than 3 m.


The two bottom images of Fig. 3 show similar results for pattern  4,  the  XYZ  meandering  path.  The  accuracy  in assigning  each  current  segment  to  the  correct  X,  Y and  Z


location is very good. Furthermore, lateral resolution analysis with different samples show that 3D MFI can provide lateral resolution better than 3 m.


Figure 3. 3D current layer assignment overlaid with optical image.


Finally, in addition to provide an accurate 3D current map,3D MFI can also provide critical geometrical parameters such


历


as current width, layer separation distance, and distance from sample top surface to currents.


|Table  1. structures. |Quantitative  Results  Summary  for  different |Quantitative  Results  Summary  for  different |Quantitative  Results  Summary  for  different |Quantitative  Results  Summary  for  different |
|---|---|---|---|---|

|Parameter|design value|3D Solver fit pattern 3|3D Solver fit pattern 2|3D Solver fit pattern 1|

|z(μm)|NA|6.8293|12.08|12.74|

|layer 1 to layer  2 (μm)|5|4.669|4.821|4,540|

|layer 2 to layer  3 (μm)|5|5.204|4.833|5.0895|

|layer 3 to layer  4 (μm)|5|5.364|5.788|5 (fixed)|

|wire width (μm)|20|21.27|20.67|20 (fixed)|

|current (mA)|1.0028|1.0028 (fixed)|1.0028 (fixed)|0.9978873 (fixed)|

Top de


125


Bottom die


Table 1 summarizes the quantitative results for 3 different patterned structures analyzed using 3D MFI.  It is remarkable that the layer separation estimated by the 3D MFI technique is


better  than  1  m  in  all  cases  and  that  the  wire  width  is accurate within 1 m as well.


3-die TSV IC devices


100010


For testing the 3D solver capability on real devices, we used 2 and  3-die  TSV devices  provided  by the  Fraunhofer  IZM


photo colorized with known layer heights


Institute (www.izm.fraunhofer.de). The devices,  IZM ASSID


le/aJ↓


ATC, are 2-die (TD) and 3-die (TD+SD) TSV connected dies.


eheJZ


These are test structures to qualify process. The basic reticle


lehaJ£


size is  22 x 22 mm2  with 25  m space width for  electrical


eha


contacts and micro-bumps (solder bumps and copper pillars)


00000000000


of about 25 m diameter. The chip construction is mother die


dyolos ndaudosapo u


(coupon), then top die for the 2-die configuration or mother


gasaujd eiulzom oeumipu[


die,  stacked die (intermediate) and top die in a chip-to-chip with micro-bump configuration. The bump pitch is 55 mm and


5o|ouzepd uoo


the die size is 10 mm2. The structure is a daisy chain. Fig. 4 shows a top view optical picture (left) of the device with the probe locations marked as “1” and “2”, with the feed-in traces


e/aJ↓


visible  until  they  reach  the  top  die.  The  top  segments


ehauz


connecting 2 TSV pairs are also visible on the top die. On the


bottom right  insert,  a  cross-section  sketch  shows  the  daisy


ehaJ7


chain structure. Top right insert shows a picture of the wafer


duo1os nda.dosapo u


piece and in red, the specific die used for scanning.


包


Top die


deuje|s ojnpaud eayz a) zou lououm !p1y(


Figure  4. Die  level  image  and  geometric  configuration sketch of the 2-die TD device.


The TD device daisy chain has approximately 36,000 TSVs with  an  expected  resistance  of  1.35k.  TD+SD  devices contain ~72,000 TSVs with expected resistance of 2k. The


measured resistances for both TD and TD+SD samples were as  expected.  We will  focus  on the  2-die  TD device  in  this study which two main goals are:


a) Determine the capability of the 3D solver to obtain the 3Dcurrent  path  on  this  complex  structure,  properly associating current segments to their respective die.


b) Determine the capability of the 3D solver to extract key geometrical information about the current distribution in the  device,  such  as  vertical  separation  (this  is,  layer separation)  or  trace  width  and  also  its  resolution


↓ 10 0 η m


capability (both lateral and vertical).


1 0 0


Figure  5.  (Left)  Optical  image  of  the  TSV  and  Layout.


(Right)  Magnetic  filed image (red/blue pattern represents magnetic  field  coming  out/in  of  the  plane  of  the  device respectively) and current path computed by the 3D solver.


Red:,  bottom  die  current  segments.  Green/blue:  top  die current segments.


Fig.  5  left  shows  an  NIR  image  of  a  section  of  the  die showing  the  in-feed  traces  and  part  of  the  daisy  chain structure.  Top  insert  shows  a  zoomed-in  image  with  some dimension on the top metal structures. Fig. 5 right shows the acquired magnetic data, with magnetic field coming out of the plane of the sample in red and blue for the opposite direction.


Overlaid on it it is the 3D path obtained from the 3D solver:red denotes current in the bottom die and green/blue current in the top die.


The  3D  solver  also  provides  information  about  the separation from top current to the sensor, ~11.8mm. The fact that  there are two colors  (green/blue)  for  the top current is


2 0 1 ↓ 0 6 R


2 0 0 g e d _ 白


because  the  3D solver  sometimes  opted  for  sitting  the  top layer 11.3m below the sensor but some other times 12.3m


1 8 0 ↓) r o d )


4 5 0


below the sensor. We estimated then an averaged distance of


11.8 m for the top current to sensor separation. This indicates


1 6 0↓)r a d ) 4 0 0


that the vertical resolution of the technique, at this point is ~


1 4 0 ↓) re d ) 3 5 0 _


1m.  In  addition,  the  3D  solver  computes  the  vertical separation  from  top-to-bottom  current,  to  be  125m,  in


1 2 0 ↓) r e d )


3 0 0 ↓ ^


excellent agreement with the expected distance according to the device dimensions: 100m die thickness plus 25m height


1 0 0 ) r e d )_


of connecting µ-bump.


8 0 ↓) r e d ) ^ _


6 0 ) r e d ) _


4 D ) r e d ) 1 ^ 0 ^


2 0 r e d ) _ E


1 ) N u e )


3 3 3 3 3 3 3 3  3 5 8 8 8 8 8 8 8 8 3 8 8 8 8 8


1 8 5 X 8 3 2 5 4 3 8 8 8 8 8 3 3


7 0 0 7 2 0 0 A 0 0 卡  1 0 ) 5 u e ) 2 0 b u s 3 0 ) H u e 4 0 ) 6 b c 5 0 ) o u e )


7 0 ) 0 1 0 ) 8 0 ) N u 8 7 o u e


1 5 0


Figure  6.  3D  Current  path  computed  by  the  3D  solver


superimposed onto optical image.


The 3D solver can, as well, provide us with the width of the current  carrying  element,  16m  in  this  case.  The  lateral


resolution in current position from the 3D solver is better than 3m as  it  can  be  noticed  in  Fig.  6  where  we  overlay  the


current path from the 3D solver on the NIR image. This was also confirmed by separate analysis.


Besides  this  important  3D  path  reconstruction  and geometrical information, magnetic field imaging allows in an easy  way  to  verify  circuit  design.  It  is  quick  and straightforward to obtain a magnetic image of the whole die as seen in Fig. 7 in which we show the current overlaid on the optical  image  for  the  whole  die,  showing  the  TSV  topconnection layout.


Figure 7.  Current superimposed onto the optical image of the whole top die showing the TSV top-connection layout.


It is clear from this image that current reaches the whole die,thus  ruling  out  any  short  circuit  which  would  show up  as missing lines  or  sections.  Also,  the  intensity of  the field is uniform across the die and thus, there is no current leaking.


Finally, each pair of TSVs connected at the top are visible in the image as red/blue dipoles, allowing us to count them and thus, count how many active components are visible. A quick count reveals that there are 87 in x and 204 in y of these topconnected  structures.  As  each  includes  2  TSVs,  the  total number  of  these  is  35,496 in  excellent  agreement  with  the intended number.


3D  Magnetic  Field  Imaging  is  a  new  non-destructive  fault isolation technique capable of mapping current in 3D IC and stacked devices  with vertical  resolution ~ 1  m and lateral resolution  of  ~  3  m.  It  can  provide  critical  geometrical


information about 3D current distribution in complex, multichip  devices,  among them the  current  to  sensor  separation,which  can  be  used  to  identify  the  layer  where  the  failure occurs, as well as the separation between layers of current..


Supported  by  the  Intelligence  Advanced  Research  Projects Activity (IARPA) via  Air Force Research Laboratory (AFRL)contract number FA8650-11-C-7101. The U.S. Government is authorized  to  reproduce  and  distribute  reprints  for Governmental  purposes  notwithstanding  any  copyright annotation thereon.  Disclaimer: The views and conclusions contained herein are those of the authors and should not be interpreted as necessarily representing the official policies or endorsements, either expressed or implied, of IARPA, AFRL,or the U.S. Government.


[1] W. Arden, M. Brillouët, P. Cogez, M. Graef, B. Huizing, R.


Mahnkopf, ITRS, “More than Moore White paper”, ITRS


2010.


[2] F. Infante, P. Perdu, D. Lewis,  “Magnetic microscopy for  3D devices: Defect localization with high resolution and  long working distance on complex system in package”,


ESREF 2009.


[3] L. A. Knauss, B. M. Frazier, H. M. Christen, S. D.


Silliman, K. S. Harshavardhan , E. F. Fleet, F. C. Wellstood, M. Mahanpour and A. Ghaemmaghami : “Detecting


Power Shorts from Front and Backside of IC Packages


Using Scanning SQUID Microscopy ”.


[4] S.I. Woods, L.A. Knauss, and A. Orozco: “Current Imaging Using Magnetic Field Sensors,” Microelectronics Failure  Analysis Desk Reference, Fifth Edition, ASM


International, 2005, pp. 303-11.


[5] J.P. Wikswo: “The Magnetic Inverse Problem for


NDE,”SQUID Sensors: Fundamentals, Fabrication and


Applications, Kluwer Academic Publishers, The


Netherlands, 1996, pp. 629-95.


[6] S. Chatraphorn, E. F. Fleet, F. C. Wellstood , L. A. Knauss  and T. M. Eiles : “Scanning SQUID microscopy of


integrated circuits ”, Appl. Phys, Lett., Vol. 76, (2000), pp. 2304-2306.


[7] R. Dias, L. Skoglund, Z. Wang, and D. Smith: “Integration  of SQUID Microscopy into FA Flow,” Proc. 27th Int.


Symp. Test. and Failure Analysis (ISTFA), 2001, pp. 77-


81.


[8] M. Pacheco and Z. Wang: “Scanning SQUID Microscopy  for New Package Technologies,” Proc. 30th Int. Symp.


Test. and Failure Analysis (ISTFA), 2004, pp. 67-72.


[9] T.T. Eng, H.E. Lwin, P. Muthu, and J.M. Chin: Proc. 12th  IPFA, 2005, pp. 110-13.


[10] A. Orozco et al.: Proc. 29th Int. Symp. Test. and Failure


Analysis (Santa Clara, CA), 2003, pp. 9-13.


[11] A. Orozco: Fault Isolation of Circuit Defects Using


Comparative Magnetic Field Imaging, U.S. Patent


7,019,521.


[12] O. Crepel, P. Descamps, P. Poirier, R. Desplants, P. Perdu, and A. Firiti: Proc. 30th Int. Symp. Test. and Failure


Analysis (Worcester, MA), 2004, pp. 29-31.


[13] M. Hechtl, G. Steckert, and C. Keller: “Localization of


Electrical Shorts in Dies and Packages Using Magnetic


Microscopy and Lock-In-IR Thermography,” Proc. 13th


Int. Symp. Phys. and Failure Analysis of Integr. Circuits


(IPFA), 2006.


[14]  F. Felt, L. Knauss, A. Orozco, A. Gilbertson, Neocera


“Construction of a 3-D Current Path Using Magnetic


Current Imaging”, ISTFA 2007.


[15] O. Crepel, P. Poirer, P. Descamps, LaMIP Philips


Semiconductor, “Magnetic Microscope for ICs Failure


Analysis: Comparative Case Studies using SQUID, GMR  and MTJ systems”, IPFA proceedings 2004.


[16] David P. Vallett, IBM Systems & Technology Group, Essex Junction, VT, USA, “A Comparison of Lock-in


Thermography and Magnetic Current Imaging for


Localizing Buried Short-Circuits”, ISTFA proceedings


2011.


[17] B.J. Roth, N.G. Sepulveda, and J.P. Wikswo, Vanderbilt


University, “Using a magnetometer to image twodimensional current distribution”, J. Appl. Phys., v. 65, n.1,p. 361 (1989).


[18] A. Orozco et al., “3D Magnetic Field Imaging for NonDestructive Fault Isolation”, Proc. 39th Int. Symp. Test.


And Failure Analysis (ISTFA), 2013.


[19] A. Orozco et al., “3D IC Analysis using Magnetic Field


Imaging”, Nano Testing Symposium 2013, pp. 183-188


Failure Analysis Work Flow for Electrical Shorts in Triple Stacked  3D TSV Daisy Chains


J. Gaudestad, A. Orozco


Neocera, 10000 Virginia Manor Road, Beltsville, MD, 20705, USA


I. De Wolf*, T. Wang, T. Webers


IMEC, Kapeldreef 75, B-3001 Leuven, Belgium


*Also at Dept. MTM, Fac. Engineering, KULeuven, Leuven, Belgium


R. Kelley, T. Morrison, S. Madala


FEI, 5350 NE Dawson Creek Drive, Hillsboro, Oregon 97124, USA


In this paper we show an efficient workflow that combines  Magnetic Field Imaging (MFI) and Dual Beam Plasma Focused Ion Beam (DB-PFIB) for fast and efficient Fault Isolation and root cause analysis in 2.5/3D devices. The work  proves MFI is the best method for Electric Fault Isolation (EFI) of short failures in 2.5/3D Through Silicon Via (TSV) triple stacked devices in a true non-destructive way by imaging the current path. To confirm the failing locations and to do  Physical Failure Analysis (PFA), a DB-PFIB system was used  for cross sectioning and volume analysis of the TSV structures  and high resolution imaging of the identified defects. With a  DB-PFIB, the fault is exposed and analyzed without any sample prep artifacts seen in mechanical polishing or laser preparation techniques and done in a considerably shorter amount of  time than that required when using a traditional Gallium Focused Ion Beam (FIB).


3D Integrated Circuits (IC) wafer level stacking is very cost  sensitive to global wafer yield. If the global yield of two wafers is 95% each, the global yield of the double stacked wafer  drops to 90%. Increasing the stacking level from two to eight  of such wafers further decreases the global yield to only 66%


[1]. This can be reduced by in-line electrical testing of the  wafers and dies before bonding and after each bonding step, using dedicated probes [2]. The stacking process itself (TSV  and micro-bump bonding) is an important contributor to yield  loss. Hence, to arrive at acceptable yields of the stacked devices, all yield loss mechanisms need to be well understood  and characterized to be able to optimize the marginal process  steps.


For this, Electric Fault Isolation (EFI) and Physical Failure  Analysis (PFA) are critical enablers but at the same time face  specific challenges related to the 3D nature of the stacked devices: EFI needs to be effective in each of the three dimensions and PFA requires a fast access to the failure location and  sufficient spatial resolution to detect the (sometimes nm scale)


physical defects without any sample preparation artifacts like  mechanical stress, delamination, scratches, curtaining and  thermal damage.


In this paper we introduce Magnetic Field Imaging (MFI) as  a unique solution for both short and leakage failures in 3D die  level EFI and Plasma Focused Ion Beam (PFIB) as an optimal  solution needed for PFA in a 3D TSV device (Fig. 1).


|Failure Analysis Workflow |Failure Analysis Workflow |
|---|---|

|Fault Isolation |Fault Validation |

|FIB/SEM Magnetic Field Imaging |Plasma |

|Figure 1. The followed workflow to detect and analyze stat- ic defects (Shorts and leakages) in a 3D device. |Figure 1. The followed workflow to detect and analyze stat- ic defects (Shorts and leakages) in a 3D device. |

Magnetic Field Imaging (MFI)


When a conductor such as a copper metal trace is carrying a  current, defined as a flow of electric charge, a magnetic field  is generated according to the Biot-Savart law [3]. Magnetic  Current Imaging (MCI) is a sub technique of MFI which has  been used by the semiconductor industry for more than a decade to find electrical shorts and leakage paths and which has  the capability to “look through” all materials typically used in  the semiconductor industry, allowing global imaging without  the need for physical de-processing [4, 5, 6]. MCI utilizes two  types of sensors: a Superconducting Quantum Interference  Device (SQUID) sensor for low current and large working  distances and a Giant Magneto Resistance (GMR) sensor for  sub micron resolution current imaging at wafer/die level [6].


Plasma Focused Ion Beam (DB-PFIB)


The PFIB system uses an Inductively Coupled Plasma (ICP) Xenon ion source with high angular intensity, making it  more suitable for high current, high speed operation that is  needed when large volumes of material have to be removed


[7].  The PFIB system extends the beam current to the µA  range and yields removal rates of ~ 20000 µm3/min, which is a


Chip 2


Chip 0 and Chip 1 Daisy chains between


gain of a factor 20-50 over classical Gallium FIB systems. As  shown in Fig. 2, PFIB is well suited for site-specific sample


Chip 1


preparation as beam spot sizes are ~ 1 um @ 1 µA (bulk millChip 0


ing conditions) and ~ 20 nm @ 10pA (imaging conditions).


Navigation to a defect location is possible using Computer


Aided Design (CAD) overlay or other imported image overlays from EFI equipment. De-processing and de-layering is


facilitated by the integrated Gas Injection System and proprietary chemistries for selective and non-selective chemically Chip 2


50µm


enhanced milling. Ultimate image resolution is achieved with  the integrated High Resolution Scanning Electron Microscope (HR SEM) column, allowing visualizing defects and device


10-12µm


structures with a spatial resolution of ~ 1 nm. The DB-PFIB


system is capable of sequentially milling and imaging (Slice &


View) 100s of um size areas of the Region-of-Interest in order Chip 1to locate the hidden nm size defects for faster root cause.


Figure 2. Image showing PFIB large volume removal of the  HVHPWbtdet


500μm


2.00RV 761μm 45.0* ETD


14 pairs of


TSV37


TSV1


TSV4


TSV43


Daisy Chains b1 and b2


TSV


Daisy Chains a1 and a2


three stack TSV sample with short.


Triple stacked TSV die


b1 and b2


The sample investigated in this work is a triple-layer stack,


chains


in which 2 layers of 50 µm thick test chip (Chip 1 and Chip 2


a1_V+ a2_V+ a1_V- a2_Vin Figure 3) were assembled on a 200 µm thick bottom chip (Chip 0 in Figure 3). The test chips were manufactured by  imec’s standard 65 nm CMOS Back End of Line (BEOL) process, 5×50 µm via-middle TSV technology [8], and fine pitch  micro bumping process [10]. Further details of the test vehicle  and assembly process can be found elsewhere [9].


The daisy chains between all the stacked chips can be  measured. In this paper, the focus is on a group of interwoven  daisy chains, named a1 and a2, between the bottom chip (Chip  0) and the first stacked top chip (Chip 1). The a1 and a2 chains have a group of neighboring interwoven chains called b1 and  b2 (Fig. 4). The designed current paths of these daisy chains  include probe pads on Chip 0, top BEOL layer of Chip 0, bump joints between Chip 0 and Chip 1, TSVs in Chip 1, and  bottom BEOL layer of Chip 1. TSV and µ bump pitch in these  daisy chains are 20 µm (Fig. 3).


Figure 3. Illustration of the investigated sample.


The a1 and a2 daisy chains had 43 TSV pairs each and were  located to the left (as seen in Fig. 4) of the b1 and b2 daisy  chains. To the very left (as seen in Fig. 4) there are 14 TSV  pairs that are not related to any daisy chains. The a1 and a2


81


daisy chains are built such that if a1_V+ and a1_V- are connected, they should show continuity, and the same is the case  with a2_V+ to a2_V-. However a1 should not be connected to  any a2 probe pads.


Figure 4. The 14 left TSV pairs (red) are not part of the  a1_a2 daisy chains. The next TSV pairs (marked orange) are the a1_a2 daisy chains that start on the right side (marked by the TSV1 arrow) and ends at the left side (marked by the TSV43 arrow). The left blue box highlights  the TSV chain where the a1-a2 daisy chain turns around  and the right blue box highlights the entry point for the  a1_a2 daisy chain with corresponding CAD layout. The  green box to the right is the b1_b2 daisy chain and is physically disconnected from the a1_a2 daisy chain, meaning no  current should be seen in the b1_b2 daisy chain when only  connecting the a1_a2 daisy chain.


Experimental setup


The sample had a short between daisy chain a1 and a2, which were supposed to be electrically separated. The probe


tests that was used for this experiment is shown in Table 1.


Table 1. MCI scans with probe pads


|Scan |Probe Pad 1 |Probe Pad 2 ||
|---|---|---|---|

|1 |a1_V+ |a1_V- ||

|2 |a2_V- |a2_V+ ||

|3 |a1_V- |a2_V- ||

|4 |a1_V+ |a2_V+ ||

a1_V+ ala1_Va2_V+ a2_VThe signal was injected into the respective daisy chains by  probing V+ to V- on the bottom chip. To send a signal between daisy chain a1 and a2 one could probe V- to V- and V+ to V+. The MCI scans were done using the GMR sensor only. The sample was attached to a vacuum chuck and raster  scanned (Fig. 5).


Figure 5. Image showing MFI scanning setup with the  GMR sensor raster scanning the entire sample.


The scan area included the entire a1_a2 and b1_b2 daisy  chains in addition to the extra 14 TSVs to the very left of the  a1_a2 daisy chains (Fig. 6 blue box area). The probe pads  were on the bottom die further away from the TSV structure (Fig. 6 yellow box area).


Figure 6. Yellow area shows the probing pads and the blue  area shows the scanning area.


Four scans were done to localize the short location using a


4.4mA, 5.333kHz AC current. The current images were overlaid the optical image and the results of the MCI data are disMCI Electronics


played in Fig. 7.


Scan 1


Current SourceSensor


Cantilever


Daisy chains between


Chip 0 and Chip 1


0、d0


Stage controlled by PC


Sensor  substrate


Scan 2


Scan 3


>bandbcb1 and b2 chainsn


Scan 4


a1 and a2 chains


Figure 7. Current images overlaid with the optical device


XYZ stage


images showing abnormal current patterns. Yellow current  color means the current is closer to the top surface while  darker orange color means current is further away from the  surface.


The bright yellow current seen in Fig. 7 is from surface current at the top of Chip 2, meaning that in these specific location, the current is coming up to the top surface of the chip  stack. However, from the layout, no current should be traveling in this TSV layer. Therefore we can make a pre conclusion  that there has to be at least one or more shorts where the signal  reaches the top surface (Chip 2) seen on the left of the data  scans in Fig. 7. Also, we see that the b1_b2 daisy chains also  have current, something that should not happen as these daisy  chains are not connected to a1_a2 daisy chains. For better understanding of the failure, high resolution scans were compared directly with the layout (Fig. 8).


HVHPW90det V29m0mD


||TSV 28 |23 |TSV |18 TSV |
|---|---|---|---|---|

|Scan |1 ||||

|Scan |2 ||||

|Scan 3 |Scan 3 |Scan 3 |Scan 3 ||

|Scan 4 |Scan 4 |Scan 4 |Scan 4 ||

|Figure 8. TSV pairs 18, 23 and 28 (counting from right as shown in Fig. 5) seems to be the shorted TSV pairs. |Figure 8. TSV pairs 18, 23 and 28 (counting from right as shown in Fig. 5) seems to be the shorted TSV pairs. |Figure 8. TSV pairs 18, 23 and 28 (counting from right as shown in Fig. 5) seems to be the shorted TSV pairs. |Figure 8. TSV pairs 18, 23 and 28 (counting from right as shown in Fig. 5) seems to be the shorted TSV pairs. |Figure 8. TSV pairs 18, 23 and 28 (counting from right as shown in Fig. 5) seems to be the shorted TSV pairs. |

From Fig. 8 one can see that the current enters the top layer (Chip 2) at TSV 18 and goes back down again to Chip 1 at  TSV 28. We expect to find at least 2 shorts at these two locations when using PFIB. In addition it was found that daisy  chains b also conducted current, indicating a short between  chains a and b.


Plasma FIB for PFA


Since the sample clearly has multiple shorts, the short located at TSV pair 23 was chosen for PFA using the PFIB. The  final large area cross-section is shown in Fig. 2 above.


Searching for a defect was performed using serial crosssections milled with the PFIB through chip 1 and chip 2 (90 µm x 135 µm). Coupled with SEM inspection and with 350  nm consecutive slice pitch, a defect was revealed as shown in  Fig. 9.


A short is found between the 2 BEOL layers of Chip 1, causing the current to leak into Chip 2. This result indicates a  potential issue in the BEOL process of the test wafers used in  this work. It may be related to a too thin metal layer which  resulted in a local etching of the low k material and consequent filling with Cu in the subsequent process step. The result  also suggests that the short measured at this location is not  caused by the assembly of this triple layer stack.


Figure 9. The short is in TSV Pair 23 between the BEOL  layers of Chip 1.


Conclusion


For any failure analysis to be successful a wide variety of  tools and techniques are employed by analysts. As 2.5/3D die  stacking technologies are being developed and adopted by the  industry, localization, exposure and analysis of defects in these novel devices and packages is becoming a critical step for  shorter development cycle and quicker root cause analysis. In  this paper, we have shown a workflow that successfully combines MFI for localization and Dual Beam Plasma FIB for  PFA to deliver high efficiency and throughput on short defects. Using the proposed tools and techniques delivers a nondestructive fault isolation of the ROI followed by high resolution physical analysis and root cause identification.


We would like to thank the Helios PFIB development team  at FEI for providing access to the tools and valuable consulta-


tion in performing the physical analysis of the defects. The  imec authors would also like to thank the support from all  partners and team members of imec 3D program. Last we  would like to thank the entire Magma team at Neocera for  great analysis work.


[1] European Commission Framework Programme 7 within  project eBrains (Project-no FP7-ICT-257488), “Yield of  3D IC Heterogeneous integration”, IMAPS 10th International Conference and Exhibition on Device Packaging


March 10-13, 2014, Scottsdale, Arizona, USA.


[2] Marinissen Erik Jan (2012). ‘Challenges and emerging  solutions in testing TSV-based 2.5D- and 3D-stacked  ICs’, In Proc. Design, Automation, and Testing in Europe (DATE’12), Dresden, Germany, March 2012, pp. 1277-


1282.


[3] Jackson, John David (1999). Classical Electrodynamics (3rd ed. ed.). New York: Wiley. Chapter 5


[4] Mai ZH et al., “Short Failure Analysis under Fault Isolation.” In Proc. of 8th IPFA, Singapore, 2001, pp. 202-


205.


[5] Steve K. Hsiung et al., “Failure analysis of Short Faults  on Advanced Wire Bond and Flip-chip Packages with  scanning SQUID Microscopy.” In Proc. of the 30th Int’l  Symp. on Testing and Failure analysis, pp. 73-81(2004).


[6] D.P Vallet, “Scanning SQUID Microscopy for Die Level  Fault Isolation.” In Proc. of the 28h Int’l Symp. on Testing and Failure Analysis, pp. 391-396, Phoenix, AZ, November 2002.


[7] L.F.Tz. Kwakman et al., “Sample Preparation Strategies  for Fast and Effective Failure Analysis of 3D Devices”,


ISTFA Proceedings, 2013


[8] A. Redolfi, D. Velenis, S. Thangaraju, P. Nolmans, P. Jaenen, M. Kostermans, U. Baier, E. Van Besien, H. Dekkers, T. Witters, N. Jourdan, A. Van Ammel, K. Vandersmissen, S. Rodet, H. G. G. Philipsen, A. Radisic,


N. Heylen, Y. Travaly, B. Swinnen, and E. Beyne, IMEC, “Implementation of an industry compliant, 5x50 µm, viamiddle TSV technology on 300mm wafers,” in Electronic  Components and Technology Conference (ECTC), 2011  IEEE 61st, 2011, pp. 1384–1388.


[9] T. Wang, R. Daily, G. Capuz, C. Gerets, K. J. Rebibis, A. Miller, G. Beyer, and E. Beyne, “Development of underfilling and thermo-compression bonding processes for  stacking multi-layer 3D ICs”, to be published in 5th Electronics System-Integration Technology Conference


(ESTC), Sept. 16-18, 2014, Helsinki, Finland.


[10] J. De Vos, L. Bogaerts, T. Buisson, C. Gerets, G. Jamieson, K. Vandersmissen, A. La Manna, E. Beyne, IMEC, “Key Elements for Sub-50μm Pitch Micro Bump


Processes”, in Electronic Components and Technology  Conference (ECTC), 2013, pp. 1122–1126.


Short Localization in 2.5D Microchip with Interposer using Magnetic Current Imaging


D. Nuez, P. Tan


Xilinx, 2100 Logic Drive, San Jose, CA  95124, USA


Interposers used in 2.5D technologies introduce new challenges for Electric Fault Isolation (EFI) due to the multiple  layers of silicon, metal layers, Through Silicon Vias (TSV), solder bumps and/or copper pillars making it hard for standard  EFI techniques, such as thermal and optical techniques, to  localize failures due to the opaqueness of these materials [1, 2, 3]. In this paper we show that shorts in 2.5D Integrated Circuits (IC) technologies can be localized accurately in x, y and  z-direction using Magnetic Current Imaging (MCI) while injecting a low power current and showing that the materials  used in 2.5D semiconductor manufacturing are fully transparent to magnetic fields.


Driven by strong demand for smart phones and tablets, the  semiconductor industry needs to increase data speed transfer  while preserving signal integrity between dies; all the while  consuming less power [4]. The solution to achieve this has  been to move towards 2.5D and 3D Integrated Circuits (IC), a  solution that will allow companies to create devices that far  exceed Moore’s Law [5].


2.5D IC is a System in Package (SiP) where the dies are  connected to the substrate through a passive silicon interposer (active-on-passive) with Through Silicon Vias (TSVs) connecting the metallization layers on its upper and lower surfaces [6]. 3D ICs, on the other hand, will stack two or more dies (active-on-active) on top of each other using TSV technology  by stacking the chips normally placed on a Printed Circuit  Board (PCB) in one device [5].


Field Programmable Gate Array (FPGA) manufacturers  have been early adopters of the 2.5D technology, which allows  the active die size to stay relatively small while connecting  multiple dies on a passive silicon interposer enabling high  bandwidth at low power die-to-die communication [7].


With thousands to tens of thousands of µ-bumps, each sized  45 µm or smaller, on a single interposer with multiple dies, static failures, such as shorts and opens, become much more  challenging to localize even with the latest Electric Fault Isolation (EFI) equipment [7].


In this paper, we will show a case study where both thermal  imaging and magnetic current imaging were used to localize a  short defect on a Virtex-7 FPGA from Xilinx. The two techniques will be compared in terms of injected power, resolution  in XY and depth (Z) accuracy.


Thermal Imaging


Thermal imaging has been used for decades by the Failure  Analysis (FA) industry to localize shorts and leakages in semiconductor ICs [8]. Thermal imaging is accomplished using an  Indium-Antimonide (InSb) infrared (IR) focal plane array


(FPA) detector covering the mid wave IR (MWIR) wavelength from 2-5.5µm [9]. When injecting a current into the


failed device, heat in the MWIR spectrum will be generated by  the short or leakage. Silicon is a very good waveguide for


MWIR and thus the thermal signal travels more or less unperturbed through it while metal layers will absorb most of the


thermal signal. This will cause signal spreading and thus lower  resolution experienced by the thermal detector array [10].


For accurate fault isolation, the thermal emission image is


superimposed onto an IR confocal laser image using a 1340nm (1.34µm) wavelength laser scanning microscope (LSM) [10].


Magnetic Field Imaging (MFI), as applied to failure analysis (FA) in the semiconductor industry, is based on mapping  the magnetic field produced by a current injected into the failing structure of the device under test (DUT). Unlike optical  radiation employed by EFI techniques such as thermal and  photon emission [1, 2, 3], the magnetic field has the advantage  of passing unperturbed through virtually any material used in  semiconductor manufacturing. The magnetic field image of  the DUT is converted into current density image by using a  Fourier Transform inversion technique [11, 12]. In order to  determine the fault location, the current image is superimposed onto an optical image usually acquired with a near infrared (NIR) camera at 1080nm (1.08µm).


MFI has two major implementations: Magnetic Current Imaging (MCI) for localization of shorts and leakages [13] and  Space Domain Reflectometry (SDR) for localization of open  defects [14]. For MCI applications, magnetic field is imaged  by either a Superconducting Quantum Interference Device (SQUID) or Giant Magneto Resistive (GMR) sensors. The  SQUID sensor is mostly applicable for package level devices  with working distances beyond 100µm and/or when low current is required. Alternating currents (AC) at 2-15 kHz provide  for noise reduction using a lock-in amplifier. The GMR sensor  is used for the front side wafer/die level high resolution (submicron) imaging using AC sampling currents at 95 kHz [15]. In SDR applications the SQUID detects a radio frequency (~40MHz) current forming a standing wave in the open trace


[16].


SQUID and GMR sensors differ in both sensitivity and spatial resolution. SQUID is the most sensitive magnetic sensor  known [11], and for electronic fault isolation it is typically  used to image AC sine currents as low as 500 n


(                   at 1Ω resistance) at a working distance of several hundred microns between the current path and  sensor (Converting sine AC peak to peak current to root mean  square (rms), the current needs to be divided by     ). The  SQUID sensor is kept in vacuum at cryogenic temperature, while the DUT is raster-scanned at room temperature and separated from the SQUID sensor enclosure by a thin diamond  window. This setup allows localizing currents to within ±3  microns.


Virtex-7; multiple die FPGA


The sample used in this case study was a Xilinx Virtex-7


InSb Detector


device that places four 500µm thick FPGA microchips on top  of a 100µm thick passive silicon interposer with TSV side-byand Laser


side on a passive silicon interposer [5]. The silicon area was ≈775    (≈25mm×31mm) with a total of 6.8 billion transistors [7]. The µ-bumps were 45µm tall and the C4 bumps were


Optics


0.5X, 5X


90µm tall (Fig. 1).


25mm


Scanning Laser 1.34µm


Thermal


for over view image


Emission


31mm


SQUID  electronics


Current Source


micro bumps Interposer


SQUID tip (inside  vacuum chamber)


C4 bumps


28nm FPGA         28nm FPGA         28nm FPGA          28nm FPGA


Package Substrate


****u


Silicon Interposer


BGA    Solder    Balls


XY stage


Figure 1. Shows the buildup of the FPGA stacked device on  top of the interposer [7].


The sample failed short with resistance 6.5Ω between power


and ground after 509 cycles of Temperature Cycling (TC) test  condition B, which cycles between temperatures of -55°C at  the low side and +125°C at the high side [17].


Electric Fault Isolation (EFI)


Two EFI techniques were used to localize the short defect; 1) a thermal imaging system using a liquid nitrogen (LN2)cooled 256 x 256 pixels at 45µm pixel size InSb IRFPA detector covering wavelengths from 2-5.5µm (Fig. 2 upper) [9], and  2) a MCI system using the cryo cooled (77K) Scanning SQUID Microscope (SSM) where the sample is raster scanned  with minimum pixel size of 1µm under the sensor to create the  current image (Fig. 2 lower).


Figure 2. Scan setup using the Thermal Emission system (upper) and the Scanning SQUID Microscope (SSM) using MCI (lower).


1. Thermal Imaging


The two shorted BGA solder bumps had wires soldered for  current injection of 120mA at 0.90V, which is 108mW of input power. The sample was placed under the InSb camera and  was imaged first using 0.5X magnification and then 5X magnification (Fig. 2) which makes each pixel size 90µm and 9µm  respectively (based on 45µm pixel in the InSb array).


-


With 0.5X magnification and 90µm pixel size one need 9  images to fully cover the entire chip area. The large signal  below the hot spot is an artifact from the input of the current  signal. With pixel size of 9µm and approximately 15-20 pixels  inside the hotspot, the defect location size was approximately  150µm large. Due to the optical laser scanning image (background image) using 1.34µm laser, few details can be seen in  metal layer 1 through the backside of the silicon (Fig. 3).


|0.5X |Lens 120mA |@ |0.90V |
|---|---|---|---|

|5X Lens |120mA |@ |0.90V |

|Figure 3. Thermal laser scanning tion and the lower seen in the 5X probe for X-ray |emission image. The image is magnification inspection. |spot superimposed upper image is 0.5X 5X magnification. image was used as |onto the magnifica The needle a landing |

2. Magnetic Current Imaging (MCI)


The two shorted pins were electrically connected using  backside probing. An AC current at 5.333kHz of


2.2m              (1.56m    ) on 6.5Ω, corresponding to


11.2µW of power (rms), was injected into the short location  through the shorted BGAs, and global MCI was performed (Fig. 4).


Figure 4. The red/orange shows the current path over3D Analysis Location


Short Location


laid the optical image. White arrows show the current direction while the green line shows the location where 3D  analysis will be performed. The blue box displays the area  where a high resolution scan was done.


The current (red/orange path in Fig. 4) overlaid to the NIR  image is the absolute value of the current             . Since    contains all information about the current in xdirection and    contains all information about the current  in y-direction, one can calculate the direction of the current (displayed by the white arrows in Fig. 4). All shorts act as  an “intersection” where current goes in and then out of the  failing location, which makes it easy to recognize a short  location versus the normal current path.


The next step was to acquire high resolution MCI image  to allow for only the short location current hot spot to be  visible and then superimpose onto an NIR image. This was  achieved by using “thresholding” on the current data image


to remove the weaker current signals and keeping the  stronger signals generated by the short locations. The distances in x and y from a visible feature (die corner) in the  NIR image is displayed in Fig. 5.


Figure 5. Current peak of short location visible in metal


545µm 645µm 735µm


MCI Estimate 560µm


200µm


layer 1 through the backside of the silicon using NIR.


3D Analysis


Since the 2.5D technology involves multiple layers, the location in z-direction is a critical parameter before choosing the  best fault validation technique. 3D analysis using thermal imaging with a high frequency InSb imaging array coupled with  a lockin amplifier was not successful in obtaining the distance  from the surface of the die to the failing location.


MFI can easily and fairly accurately calculate the z-distance  from the top of a sample to the current path, when a straight  current path is available. In the sample used for this analysis,


several ears of straight current paths can be found. The 3D  analysis is done by using that the two magnetic field max/min  locations found from a line cut across the current path is equal  to two times the total distance from sensor to the current path (Fig. 6) [18].


1.5-


1-


Magnetic Field-1--0.5-0-0.5-


Figure 6. Z-distance analysis of location 1 displayed in   ofArbitrary Units


2z = 1906µm


-1.5-


300003100032000330003400035000µm


y=719µm


Fig. 2.


x=951µm


A straight line current trace segment close to the short was  used for this analysis (see choice of location in Fig. 4). The  distance between the min/max locations of the magnetic field  was found to be 1906µm (Fig. 6). Dividing this number by  two and then subtracting the distance from the SQUID sensor  to the outer edge of the diamond window (193µm found by  calibration) and the distance between the outer edge of the  diamond window to the sample surface (200µm set by the user  and a calibrated touch probe) gave a distance from the sample  surface to the current path of 560µm (Fig. 7) [18].


个


Figure 7. Shows the z-dimensions in the Virtex-7 and the  MCI fault location estimate.


Using the known distances from the layout in Fig. 7 that the  die is 500µm, the µ-bump is 45µm, interposer is 100µm and  the C4 bump is 90µm one can find that the current path right  next to the short is calculated to be 15µm below the µ-bump. From this we can assume that the short is located in either the  metal traces on top of the interposer or at the very bottom of  the µ-bumps.


Fault Validation


X-ray validated the root cause of the short defect to be a  metallic ball of approximately the same size as a µ-bump in  between a power and a ground µ-bump that was sandwiched  in Z between the interposer and the FPGA (Fig. 8) at the XY  location indicated by both thermal imaging and MCI. Due to  the high number and density of µ-bumps, using X-ray alone  for fault isolation is close to impossible; however, X-ray was  highly useful in validating the defect location after electrical  fault isolation techniques had localized the failure to a smaller  and well defined location (Fig. 8 upper image).


Figure 8. X-ray images showing a metallic ball in between  two µ-bumps causing the short.


The distance from the top surface to the top of the interposer/micro bumps is 545µm, which means that the MCI calculated z-distance analysis was off by 15µm. This distance  should be accurate enough in this case study for the FA engineer to make the conclusion that the short was occurring in the µ-bumps or in the metal traces at the top of the interposer.


Thermal imaging and MCI techniques were both able to localize this short in XY, however only MCI provided information about the Z location of the short. The most visible difference between the two techniques is the power needed to detect a signal; thermal needed about three orders of magnitude  more power than MCI to localize signal from the short defect. The results have been summarized in Table 1.


Table 1. Comparison of thermal imaging and MCI results in  this particular case study


|Technique |XY resolution |Z resolution |Current (rms) |Power (rms) |
|---|---|---|---|---|

|Thermal Imaging |≈150µm |N/A |120mA |108mW |

|MCI |≈10µm |≈ ±40µm |1.56mA |11.2µW |

[1] O. Breitenstein, et al, “Microscopic lock-in thermography  investigation of leakage sites in integrated circuits”, Rev. Sci. Instrum. 71, 4155 (2000).


[2] A. Glowacki, C. Boit, Berlin University of TechnologyGerman and P. Perdu, CNES – France, “Optimum Si


thickness for backside detection of photon emission using  Si-CCD” ESREF Proceedings 2012.


[3] T. Sun, G. L. Woods, M. F. Duarte, K. Kelly, C. Li, and  Y. Zhang, Rice University, Houston, TX, USA “OBIC


Measurements without Lasers or Raster-Scanning Based  on Compressive Sensing “ ISTFA Proceedings 2009


[4] “Amkor Technology Reports Financial Results for the


Fourth Quarter and Full Year 2011,” Q4 and 2011 Amkor  Technology, Inc. Earnings Conference Call, February 9,


2012.


[5] M. Santarini, Xilinx, “2.5D ICs are more than a stepping  stone to 3D ICs” Published in EE Times 3/27/2012


In this study, we have utilized advanced image processing and  image analysis tools to establish a more consistent and  accurate image perception. In particular, we tackle the issue of  texture characterization. Improper texture and/or texture  inconsistency are deemed a defect often present in counterfeit  parts, but quantifying it in such way that one can distinguish  between the counterfeit and authentic parts, is a major  challenge. Also, optical methods can potentially misrepresent  texture variations due to light intensity and exposure which  can bias the detection process. By using multiple surface  parameters to quantify texture variation, we have been able to  distinguish more sophisticated blacktop-coated samples and  sanding issues, two of the most common phenomena in  counterfeit ICs.  We also use inconsistencies within the  samples and their defects as an alternative to having a golden  IC. However, the final decision has further been validated  using results from 5 known authentic samples.


Background


Counterfeit parts are classified into 7 main categories: Recycled, remarked, overproduced, defective, forged  documentation and tampered [2]-[5]. A detailed explanation of  each can be found in [2].


Physical Inspections


Mechanical


Incoming


Inspection


|Leads/Balls/ Columns|Package|Bond Wires|Die|
|---|---|---|---|

|M1:Dents|M10:Sanding/ ▲ Grinding Marks|→Wires M23:Missing|M29:Missing Die|

|M2:Re-tinned|M11:|→Connection M24:Poor|→M30:Wrong Die|

||Markings||M31:|

|Dimensions M3:Incorrect|M12:_Burned Markings|M25:Broken ▼ Wires|Delamination M32:Gross ◆ Cracks|

|Materials M4:Wrong|、M13:Ghost Markings|M26: Poor/ Inconsistent Lead Dress/|_M33:Improper Die Markings|

|M5:Color|M14 Color|Lead Frame|M34:Die Damage/|

|→Variations|▲ Variations/ Fade|M27:Re-|Extraneous|

|→Marks M6:Tooling|M15:Improper|→worked Wire Bonds|Markings|

||Textures|M28:Bond|M35:Poor/ Inconsistent Die|

|M7: Misaligned/|M16:Extraneous|Pull Strength|Attach|

|→ missing Balls/ Columns|Markings M17:Dirty Cavities|Markings M17:Dirty Cavities|Markings M17:Dirty Cavities|

|M8:Distorted/ → Non-uniform Balls/Columns|M18:Incorrect > Dimensions/ Weight|M18:Incorrect > Dimensions/ Weight|M18:Incorrect > Dimensions/ Weight|

|M9:Lead Re- →attachment|M19:High/Fine/ Gross Leak (Hermetic) M20:Package Mold|M19:High/Fine/ Gross Leak (Hermetic) M20:Package Mold|M19:High/Fine/ Gross Leak (Hermetic) M20:Package Mold|

||Variations M21:Package|Variations M21:Package|Variations M21:Package|

|Damage M22:Resurfacing/|Damage M22:Resurfacing/|Damage M22:Resurfacing/|Damage M22:Resurfacing/|

|blacktopping|blacktopping|blacktopping|blacktopping|

Low Power


Visual Inspection→Blacktop TestingOptical Inspection


+X-Ray Imaging*Microblast Analysis+Wire PullFourier Transform Package Confg. andDie Shear(Her-Infrared Spec.(FTIR)dimension Analysismetic Devices)Ion Chromatography Hermeticity Testing*Ball Shear(IO)


Scanning Acoustic


"Microscopy (SAM)


Scanning ElectronScanning ElectronEnergy Dispersive Microscopy (SEM)*Microscopy(SEM)Spectroscopy (EDs)Figure 1(b) - Physical inspection methods


After acquiring digital microscope images of all chips


using the cited instrument, the samples have been investigated by Scanning Electron Microscopy (SEM)and X-ray Microscopy. SEM analyses have been performed using FEI Quanta 250 under low vacuum mode with no sample preparation. Energy dispersive Spectroscopy (EDS) was performed in the same imaging session using an X-ray detector and EDAX software.


Images were taken at three tilt angles using eucentric tilting at the working distance in order to perform stereo


Figure 1(a) Taxonomy of Mechanical Defects


and further texture analysis. XRM analysis was performed The mechanical defects that are associated with theseusing Xradia Versa 510 (Pleasanton, CA) using large field counterfeit types can be seen in Fig. 1(a) which is the target of


physical inspection methods. The defects include both


Proposed Method


geometric abnormalities and compositional discrepancies and


inconsistencies. Such variety of defects demands utilization of4-Dimensional Scanning Electron Microscopy (SEM)


various test methods as shown in Fig. 1(b) which demand


SEMs are extensively used in counterfeit detection as a defect more than 19 instruments. It must be noted that some of thesecharacterization tool.SEMmicrographshave beendefects are also associated with quality issues.qualitatively used to characterize the surface and /or texture of the electronic parts. The large depth of field of SEM makes it Preliminaries


a much more appropriate tool for texture inconsistency analysis comparing to optical microscope [11]. However,


Five Intel flash memory ICs have been analyzed for


SEM images remain to be two-dimensional lacking quantified


counterfeit detection without prior knowledge of them being counterfeit or authentic. Sample image of the chip using a VHX2000 Keyence digital microscope (Itasca, IL)


Z66T③®高


Figure 3- Two images of the exact same location of the same


Figure 2- Sample Digital Microscope Image of the ICs investigated


Texture variation is not always readily seen using microscopy techniques. Figure 3 shows two SEM images of the exact IC with different imaging parameters


has been provided in Fig. 2.


depth information.


of view (LFOV) and 4X magnification objectives.


photogrammetry for 3D surface geometry reconstruction Microscopy (SAM)*SpectroscopyScanning Acoustic_Raman


(XRF)X-Ray Fluorescence Exterior TestsInterior TestsMaterial Analysis


same location acquired by different acquisition parameters. As  it can be seen the variation in the texture is almost entirely  invisible while it can be easily recognized in the left image. Another issue is such images always require an SME to  interpret the data as it lacks quantified information and is not  suitable for automation.


In order to obtain 3D images of the surface of the inspected  ICs, we have used stereo-photogrammetry, a well-established  technique in aerial imaging which has been developed with


|SEM for 3D reconstruction. This technique consists of 3 stages: [12] |SEM for 3D reconstruction. This technique consists of 3 stages: [12] |
|---|---|

|1) |Image Acquisition: Taking images of the same area from different perspectives. |

|2) |Matching Algorithm:  A computer algorithm to find homologue points, i.e. points belonging to the same location |

|3) |Extracting depth information; Using projective geometry and Piazzesi Algorithm [8] to find three dimensional coordinates and reconstruct digital elevation model (DEM) |

Figures 4(a) and (b) demonstrate the acquired images on a  dimple (mold cavity) of the ICs taken at two tilting angles of  positive and negative ten degrees. The working distance and  the angle have been optimized using guidelines elaborated in  reference [12]. Figure 4(c) shows the 3D reconstructed image  with the color map corresponding to height values.


In order to extend the information to the 4th dimension, EDS  mapping has been used on the exact same area and the images  are reconstructed in color to show any variations in material  composition. Figure 5 demonstrates a similar image to that of  Fig. 4 (a) and (b) in terms of location, however in this figure  color represents material composition and shows the presence  of different material on the wall of the dimple.


Figure 5 Compositional Map on the Dimple, where green  represents Carbon and blue, red and yellow are Si, Ti and V  respectively


Presence of inorganic materials on the package of these chips  is an anomaly. Further analysis has shown the same material  composition, that is (Ti and V), on the markings of the chip. The presence of Si in the image is also an indication of  sanding. This analysis can help us to not only distinguish the  defect but also find out the process of counterfeiting which  can contribute to further counterfeit detection and prevention. In this case, it appears that the previous marking on the chip  has been removed using SiC paper sanding and then remarked. Combining Fig. 4(c) and 5 can provide us with four  dimensional information on the sample which can greatly  facilitate the counterfeit detection. This is shown in Fig. 6.


合


2696mm


Mioroship


册10.5409 mm


200 wn


M福聘


Figure 4 Tilted (a) and (b) and reconstructed 3D (c) images


Figure 6- four-dimensional image of a Dimple, with colors  represent sample material as Fig. 5.


Dual Energy 3D X-ray Microscopy


2D radiological X-rays is a well-established technique to  examine the interior attributes of the chip without  decapsulation.[14] By taking multiple 2D X-ray projections


HH


and then reconstructing them, one can obtain the three  dimensional information of the interior and the exterior image  of the imaged object. This technique is commonly known as  X-ray Tomography scan. Researches have used the 3D X-ray  Tomography for studying electronic parts, however there have  always been some issues: [15], [16]


High Resolution Lens-based detector


Dimple Investigation: Height, Relative Positioning and Sanding (a


Sample


filled dimple) Investigation


X-ray Source


Energy Filter


Lens


Scintillator


CED


Figure 7 Schematic of the X-ray Microscope structure


1. Many electronic parts and in this particular case, the flash  memory chips have high aspect ratio, which result in the  obligation to have a sufficiently large working distance  during tomography to avoid collision of the sample with


5000 Microns


the source and detector. However, conventional CT loses  resolution significantly as the distance to the source is


Investigation of black top coating


increased. The number of X-ray counts also decrease  greatly resulting in a much worse signal to noise ratio.


2. In many cases such as the ICs studied in this work, samples are made of materials with radically different Xray absorption coefficients. For example, the package is  commonly made out of Carbon with a very low X-ray  attenuation coefficient while the leads are made of Tin (Sn) which is a metal with a much higher attenuation  coefficient. This entails problems associated with  choosing the right X-ray source energy.


3. The process of tomography is believed to be time  consuming and inefficient for everyday counterfeit  detection application.


Die and Bond wires investigation


Lead Frame


Investigation


Lead Investigation


Figure 8- XCT images of ICs using low (bottom) and High


(top) energy


In order to overcome these challenges, two tomographies have  been performed at two different energy levels focusing on the  package for the low energy ones and investigating leads with a  higher energy. Use of dual energy can help us to identify both  exterior and interior defects. Also the cited X-ray  Microscope’s architecture and use of a scintillator allows a  much better resolution to be achieved at higher working  distances. Figure 7 provides a schematic of the X-ray (a)


microscopy with Resolution at a distance (Raad) propriety  capability.


Also to capture the most defects in a single imaging session, the large field of view detector has been used where the entire  sample can be imaged at once. Figure 8 shows a sample 3D  rendered image at both high (a) and low (b) energies and the  investigations that have been facilitated using the proposed  technique.


Texture analysis


The data density and three dimensional information associated  with 3D SEM allows performing a more detailed texture  analysis. Table 1 shows the surface parameters that are  extracted from the surface of the chips to quantitatively  address inconsistencies. In the table, “Z” denotes the height  information that can be extracted through the entire  rectangular surface with the length M and width N.


Table 1- Surface Parameters for Texture Analysis


8


|Parameter |Definition |Formulation |Formulation |Formulation |
|---|---|---|---|---|

|Sa: Average Roughness |Arithmetic mean of absolute height values of the area |1 |∑ |  (  ,   ) |

|Sa: Average Roughness |Arithmetic mean of absolute height values of the area |     |||

|Sa: Average Roughness |Arithmetic mean of absolute height values of the area |1≤    ≤    |1≤    ≤    |1≤    ≤    |

|Sa: Average Roughness |Arithmetic mean of absolute height values of the area |1≤  ≤   |1≤  ≤   |1≤  ≤   |

|Sq: RMS Roughness |Root mean square |√ 1      ∑   2(  ,   ) 1≤    ≤    1≤  ≤   |√ 1      ∑   2(  ,   ) 1≤    ≤    1≤  ≤   |√ 1      ∑   2(  ,   ) 1≤    ≤    1≤  ≤   |

|Sq: RMS Roughness |value of the height of the area |√ 1      ∑   2(  ,   ) 1≤    ≤    1≤  ≤   |√ 1      ∑   2(  ,   ) 1≤    ≤    1≤  ≤   |√ 1      ∑   2(  ,   ) 1≤    ≤    1≤  ≤   |

|Sp: Peak |Largest Height of the area |max |max |  (  ,   ) |

|Sp: Peak |Largest Height of the area |1≤    ≤   |1≤    ≤   ||

|Sp: Peak |Largest Height of the area |1<  <   |1<  <   ||

|Sv: Valley |Minimum Height of the area |min 1≤    ≤   1<  <     (  ,   ) |min 1≤    ≤   1<  <     (  ,   ) |min 1≤    ≤   1<  <     (  ,   ) |

|Sku: Peakedness |Kurtosis of the area |1         4 ∑   4(  ,   ) 1≤    ≤    1≤  ≤   |1         4 ∑   4(  ,   ) 1≤    ≤    1≤  ≤   |1         4 ∑   4(  ,   ) 1≤    ≤    1≤  ≤   |

+/-3%


品


2 8


/-1%


√


的


1%Sa


0。


svSPsq■Sv Sa


■Sp■Sq


Roughness parameters such as Average and RMS allow us to  have a better understanding of texture variations. Height  parameters can help us analyze the dimple height variations  independent of the reference plane and finally kurtosis, as a  measure of pointiness of the surface allows us to find sanding  marks and removed markings based on the texture  information. Figure 9 shows the surface parameters extracted  from the 5 ICs showing that using any single parameter alone  cannot show the discrepancy among the surfaces however as  more surface parameters are used. The inconsistencies among  the samples are better identified.


It can be seen at roughness level (Sa and Sq), only sample 5 is  showing major discrepancy. Moving to height information we  can see that sample 1 and sample 3 share different values than  those of 2 and 4. This takes us to our fifth measure, Kurtosis


which has been kept out the Fig. 9 for scaling issues. The  kurtosis values for the 5 samples are 0.98, 1.5131, 1.3048,


1.5461, and 1.358.


This suggests that the value is substantially lower for sample 1  which can be attributed to sanding. The 4-dimensional image  shown in Fig. 6 also showed sanding residual materials which  can further prove the process of counterfeiting.


Such characterization allows us to quantitatively prove  sanding which can facilitate the process of automation. In  addition, as only inconsistencies within the 5 samples are used  for detection, the analysis does not require a “golden IC”. However, we have included the information about the  authentic samples for validation purposes. As one can  determine:


1) Whether such variations also appear different


authentic samples


2) Whether the samples have different surface parameter  values than the golden IC.


Figure 9- Surface parameters extracted from a dimple for the  5 samples in study (all values are in microns)


The authentic sample bars in Fig, 9 have a number above them  showing their variations among 5 samples in percent. It is  clear that the variations between the authentic samples are  much smaller than that seen among the 5 studied ICs. Also we  can see roughness parameters are less effective measure  comparing to height parameters and Kurtosis values.


Additional texture analysis using 3D SEM data is calculated  by the areal autocorrelation function (AACF) of the surface to  obtain the texture directionality: [12]-[15]


  (     ,     ) =


(  −  )(  −  )


∑ ∑   (     ,  −    =    −    =1     )  (    +   ,     +  )  (1)


   = 0,1, … .    <   ;     = 0,1, … .    <   ;      =   . ∆  ;      =   . ∆   Figure 10 shows the AACF of each of the surfaces where the  value of autocorrelation ranges from -1 (no correlation in  pink) to 1(maximum correlation in red). Additional  information on AACF can be found in references [17-22]


Sample 1


Sample 2


Sample 3


Sample 4


Sample 5


Authentic Sample


Figure 10-AACF of all samples showing different texture direction


The ideal uniform direction in sample 1 also proves the  sanding case. In addition further discrepancies were recorded  between samples that initially had relatively similar roughness  parameters.


To further investigate if similar cases can be identified in  authentic samples, similar studies were conducted on 5  authentic samples.  All figures and exact values have been  excluded for brevity and only one has been shown in Fig. 10     as an example. All the authentic samples shared a similar  ACCF. This further proves that discrepancies in the AACF  can be used as another quantitative metric for counterfeit  detection.


3D X-ray Results


2D X-rays can help distinguishing defects such as a wrong  die/ wrong die orientation. Such study is shown for all chips in  Fig. 11. It can be seen that sample 3 has a totally different die  which has a different orientation and size. The other 4 samples  look very similar and even comparing to the authentic sample  doesn’t yield conclusive evidence though it does show a small  difference in bond wire patterning. This study proves that  extending the information to the third dimension is inevitable


Figure 12 shows 3D images of samples 1 and 2 where one can  see signs of  die face delamination on sample 1(top left) and


not in 2 (top right). Additional investigation of virtual slices  shows clear images of the die face delamination in all corners. (Bottom left and right). The die face delamination can be the  result of recycling and is a great reliability concern. After  hours of operation, such delamination can grow to the point of  breaking the bond wires. Similar images revealed same results  for sample5.


Results Summary


Combining the results from the two techniques, we have been  able to identify all the 5 ICs as counterfeits. Results were  discussed and confirmed with our SMEs at Honeywell who  performed all the tests on the parts and obtained similar  information.


All the defects identified using the techniques described are  summarized in Table 2. Other common techniques or  instruments utilized for detection of such defects are also  provided in the last column. It can be seen that using our  proposed technique can successfully detect all defects  nondestructively.


82868 2n w


8801.04 um


Figure 11- 2D X-rays of samples


6435.75 um


6435.17 um


8319


6477.57 um


8838.91 um


8807.75 um


Authentic


6435.73 um


6416.24 um


Figure 12- Top: 3D images of the die in samples 1 and 2- Showing die face delamination in sample 1   Bottom: Virtual 2D slices of sample 1 illustrating die face delamination in all corners


Sample 1-Virtual slice


Table 2 - Summary of results


|OBSERVATION |INSTRUMENT |OTHER COMMON METHODS |
|---|---|---|

|Residue on leads |SEM/X-ray |X-ray Fluorescence (XRF), Optical Microcopy |

|Sanding marks |SEM/EDS |Optical Microscopy, XRF |

|Coated/filled dimples |SEM/X-ray |LSM, Optical profilometry |

|Dimple depth variation |SEM/X-ray |LSM, Optical Profilometry |

|Incorrect lead plating (Sn vs. Sn/Pb) |SEM/EDS |XRF |

|No exposed lead base metal |SEM |XRF,Optical Methods |

|Bent leads |SEM/X-ray |Optical Methods |

|Metal shavings and/or tin whiskers on leads |SEM |SEM, Optical Microscopy |

|Different die sizes |X-ray |Decapsulation, Scanning Acoustic Microscopy (SAM) |

|Different lead frames |X-ray |Decapsulation |

|Wire bond pattern variations |X-ray |Decapsulation, SAM |

|No barrier metal under pure Sn lead finish |SEM |XRF, Optical Microscopy |

|Blacktopping (top and bottom surfaces) |SEM/X-ray |Destructive Liquid Testing |

Two novel imaging techniques have been introduced and  applied as a powerful tool for detecting defects associated


with counterfeit electronic parts. The techniques are entirely  non-destructive and don’t require any sample preparation. In addition, all information can be obtained in a single  imaging session which can greatly contribute to the time  and cost of counterfeit detection procedures. Quantitative


analysis has also been proposed for the first time for texture  analysis which has been in an issue of controversy. It has  been shown that three dimensional characterization of the  dimples along with compositional analysis can help us better  identify counterfeit parts as well as to understand the process


which can be used for further counterfeit detection and  prevention purposes. The 3D X-ray analysis has also been  used as an effective way to access the interior properties of  the ICs and proved to be necessary in cases where 2D X-ray  doesn’t provide sufficient geometry. It has been shown the


observed defects in counterfeit parts are not present in the  authentic samples. However, one doesn’t necessarily require a  so-called golden IC to check for several defects discussed in


this paper. Although the authors have taken the preliminary  steps of automation in counterfeit detection by providing


quantitative metrics, more work has to be done to establish a  rigorous algorithm for such effort. The authors seek to  develop such algorithms in their future work while improving  the quality of the proposed methods. It must be noted that  current study requires a more detailed statistical analysis to


prove if the detection is consistent.


This work was supported in part by the National Science  Foundation under grant CCF-1423282 and grants from  Honeywell and the Missile Defense Agency (MDA). The


authors would also like to thank Daniel DiMase and Steve  Walters for providing the samples and their comments as  SMEs.


[1] J. Cassell, “Reports of Counterfeit Parts Quadruple Since  2009, Challenging US Defense Industry and National Security,” Apr. 2012.


[2] U. Guin, K. Huang, D. DiMase, J. M. Carulli Jr., M. Tehranipoor, and Y. Makris, “Counterfeit Integrated Circuits: A  Rising Threat in the Global Semiconductor Supply Chain,” Proceedings of the IEEE, 2014


[3] U. Guin, D. DiMase, and M. Tehranipoor, “Counterfeit  Integrated Circuits: Detection, Avoidance, and the Challenges  Ahead,” Journal of Electronic Testing: Theory and Applications (JETTA), 2014.


[4] Guin U., D. Forte and M. Tehranipoor, “Anti-Counterfeit :


Techniques: From Design to Resign,” Microprocessor Test and  Verification (MTV), 2013.


[5] U. Guin, M. Tehranipoor, D. DiMase and M. Megrdichian, “Counterfeit IC Detection and Challenges Ahead,” ACM SIGDA,


2013.


[6] IHS iSuppli, “Top 5 Most Counterfeited Parts Represent a $169 Billion Potential Challenge for Global Semiconductor  Market,” 2011.


[7] CHASE, “ARO/CHASE Special Workshop on Counterfeit


Electronics,” January 2013,


http://www.chase.uconn.edu/arochase-special-workshop-oncounterfeit-electronics.php.


[8] CHASE, “CHASE Workshop on Secure/Trustworthy Systems  and Supply Chain Assurance,” April 2014,


https://www.chase.uconn.edu/chase-workshop-2014.php.


[9] U. Guin, D. DiMase, and M. Tehranipoor, “A Comprehensive  Framework for Counterfeit Defect Coverage Analysis and  Detection Assessment,” Journal of Electronic Testing: Theory  and Applications (JETTA), 2014.


[10] U. Guin and M. Tehranipoor, "On Selection of Counterfeit  IC Detection Methods," IEEE North Atlantic Test Workshop (NATW), 2013.


[11] J. Goldstein, Scanning Electron Microscopy and X-Ray  Microanalysis, Springer, 2003.


[12] S. Shahbazmohamadi and E. H. Jordan, "Optimizing an  SEM-based 3D Surface Imaging Technique for Recording Bond  Coat Surface Geometry in Thermal Barrier Coatings," Measurement Science and Technology, vol. 23, no. 12, pp. 125601-125601, 2012.


[13] Piazzesi G., "Photogrammetry with the Scanning Electron  Microscope," Journal of Physics E: Scientific Instruments, vol. 6, no. 4, pp. 392-296, 1973.


[14] "AS6171/IV (WIP) Method IV - TECHNIQUES FOR  SUSPECT/COUNTERFEIT EEE PARTS DETECTION BY


RADIOLOGICAL TEST METHODS - SAE International," 2014. [Online].Available: http://standards.sae.org/wip/as6171/iv/.


[15] M. Cason and R. Estrada, "Application of X-Ray Micro CT  for non-destructive failure analysis and package construction  characterization," in Physical and Failure Analysis of Integrated  Circuits (IPFA), 2011 18th IEEE International Symposium on  the, pp. 1-6, 2011.


[16] M. Cason and R. Estrada, "Physical and Failure Analysis of  1


Integrated Circuits (IPFA), 2011 18th IEEE International  Symposium on the,” 2011 18th IEEE International Symposium on  the, pp. 1-6, 2011.


[17]Dong W, Sullivan P, Stout K.  ‘Comprehensive Study of  Parameters for Characterizations Three-dimensional Surface  Topography. I’, Wear 1992; 159:161-171.


[18] Dong W, Sullivan P, Stout K.  ‘Comprehensive Study of  Parameters for Characterizations Three-dimensional Surface  Topography. II’, Wear 1993; 167:9-21.


[19] Dong W, Sullivan P, Stout K.  ‘Comprehensive Study of  Parameters for Characterizations Three-dimensional Surface  Topography. III’, Wear 1994; 178:45-60.


[20] Dong W, Sullivan P, Stout K.  ‘Comprehensive Study of  Parameters for Characterizations Three-dimensional Surface  Topography. IV’, Wear 1994; 178:29-43.


[21] De Chiffre, Leonardo, et al. "Quantitative characterization of  surface texture. "CIRP Annals-Manufacturing Technology 49.2 (2000): 635-652.


[22] Lonardo, P. M., H. Trumpold, and Leonardo De Chiffre. "Progress in 3D surface microtopography characterization." CIRP  Annals-Manufacturing Technology45.2 (1996): 589-598.


Laser Logic State Imaging (LLSI)


Baohua Niu, Grace Mei Ee Khoo, Yuan-Chuan Steven Chen, Fernando Chapman, Dan Bockelman, Tom Tong


Intel Corporation, 2501 NW 229th Avenue, Hillsboro, OR 97124  Corresponding author: Baohua.Niu@intel.com


[6] C. Maxfield, “2D vs. 2.5D vs. 3D ICs 101”, Published in  EE Times 4/8/2012.


[7] V. Tong, Senior Vice President, Xilinx, “3D in the Deep  Submicron Era”, Key Note presentation at Semicon West


[8] J.B. Colvin, FA Instruments, “Moiré Stabilized Thermal  Imaging”, Proc. 12th IPFA (2005), pp. 163-166


[9] Product details for InfraScope II


oc


http://mntl.illinois.edu/equipment/Infrascope.htm


[10] Themos 1000 Brochure.


http://www.hamamatsu.com/us/en/product/category/5002/5012/THEMOS-1000/index.html


[11] J. P. Wikswo, “SQUID sensors: Fundamentals, Fabrication and Applications, Chapter The Magnetic Inverse


Problem for NDE”, pp. 629-695, Kluwer Academic Publishers, The Netherlands, 1996.


[12] E. F. Fleet, et al., “HTS scanning Microscopy of Active  Circuits”, IEEE Transactions on Applied Superconductivity, 9 (2): 4103 (1999).


[13] D. P. Vallett, “A Comparison of Lock-in Thermography  and Magnetic Current Imaging for Localizing Buried


Short-Circuits”, ISTFA proceedings, 2011.


[14] J. Gaudestad, V. Talanov, P. C. Huang, “ Space Domain  Reflectometry for Opens Detection in Stacked-Die Packages”, Electronic Device Failure Analysis Society (EDFAS) Magazine, August 2012, pp. 22-28


[15] L. A. Knauss, et al., “Current Imaging using Magnetic


Field Sensors”, Microelectronics Failure Analysis Desk  Reference 5th Ed., pp. 303-311 (2004).


[16] J. Gaudestad, V. Talanov, N. Gagliolo, and A. Orozco,


“Space Domain Reflectometry for open failure localization”, Proc. 19th International Symposium Physical &


Failure Analysis of Integrated Circuits (ISTFA) 2012.


[17] JEDEC STANDARD document for Temperature Cycling  JESD22-A104D of March 2009 (Revision of JESD22-


A104C, May 2005).


[18] J. Gaudestad, A. Orozco, V. Talanov, Neocera, P. C.


Huang, TSMC, “Open Failure Detection in 3D Device


non destructively”,  LSI Testing Symposium 2012.


Applying Innovative Techniques for Solving  FA Challenges of 3D IC Failures Utilizing  Conventional Equipment


Phoumra Tan, Kenny Ng, Eric Thorne, S.Y. Pai, Doug Hamilton, Dan Nuez


Xilinx, Inc


Phone: (408)879-4797; Fax: (408)879-4727; Email: Phoumra@xilinx.com


Abstract –  With the advent of three-dimensional stacked integrated-circuit (3D IC), the functionality, performance and  power of semiconductor devices has been elevated to a new level. At the same time, the analytical techniques used in the  evaluation of 3D IC must also advance in capability. Some new methodologies, based on FPGA products, have been


developed to analyze 3D IC failures, all using conventional FA equipment and innovative techniques to achieve a short  turn-around time and high success rate. A few case studies will be presented to show the effectiveness of the


methodologies.


Traditionally, the scaling of semiconductor chips has  been used to improve signal speed, increase functionality, decrease power consumption, and improve overall  performance.  Until now, the scaling has depended on Moore’s Law to deliver nearly twice the logic capacity with  each new process generation [1].  However, the growing  demands of today’s high-end markets require more  capacity and performance beyond what Moore’s Law  scaling can provide. 3D IC packaging was developed to  overcome the limitations of lithography scaling by stacking  multiple dies in a 3D fashion inside a single package. Xilinx has adopted Stacked Silicon Interconnect  technology (SSI) for the new generation of FPGAs, which  uses a passive silicon interposer, microbumps, and throughsilicon vias (TSV) to achieve higher capacities, performance, and power savings that would not be possible  using the traditional monolithic approach [2, 3, 4, 5].  Since  the active dies are stacked on top of the passive interposer  in a face-to-face fashion, it becomes very challenging for  fault isolation and subsequent physical failure analysis with  the present available analytical tools with very limited 3D  capability [6] (Figure 1). To overcome this challenge, new  and innovative techniques and methodologies have been  developed that primarily focus on all 3D interconnect  related fault failures while using conventional FA  equipment.  Combining with existing FPGA die fault  isolation techniques, this provides us a full FA capability to  analyze the 3D packaged device failures. Three case studies  will be presented to show these new FA methodologies and  approaches for analyzing and debugging defects in the 3D  packaged devices using conventional lab tools:


1) Investigation of die-to-die interconnect fault failures(for High-bandwidth, low-latency connections).  This  demonstrates the use of a basic scan methodology for


electrical fault isolation to locate the microbump defects and interposer metal interconnect defects.


2) Analysis of IO parametric failures with utilization of the parasitic diode built in CMOS process and using crosssectional micro-probing in conjunction with Kelvin  resistance measurement technique. This enables us to  analyze the microbump interface high resistance problem.


3) Analyzing the high Icc failures with an innovated interposer de-processing technique using selective silicon  etch KOH. This enables us to pinpoint the interposer  bottom delamination and solder extrusion problem in a ceramic package substrate.


Figure1. Schematic cross section of the Stacked Silicon Interconnect  Technology (left), and an actual SSIT device cross section (right)


II. INVESTIGATIONS OF DIE-TO-DIE INTERCONNECT FAULT FAILURES


Fault isolation of internal interconnect fault failures from  FPGA slice to FPGA slice is challenging because there is  no direct access to the interposer from the external BGA  balls.   For this reason, Xilinx has developed an innovative  interposer testing methodology to pin-point the exact  failing locations.


Testing of the passive interconnect interposer and  microbumps connecting FPGA to FPGA slices uses a basic  scan methodology.  One FPGA side acts as a driver of the  connections from the FPGA through the interposer to the  receiver FPGA.  Test patterns are shifted in (scan clock), then clocked across the interposer (equivalent of a


“functional clock”), and finally scanned out and compared.


See Figure 2.  Diagnostics are very simple, as each failing  vector is easily mapped back to an observation flop, and the


“electrical node” under test between the scan chains is  presumed faulty.   In this case, the “electrical node” is


made up of the wire on the interposer, the two microbump


Interposer Open Failure


connections on each end of that wire, and the wires in the


inpul


input


FPGA plus their drivers.  The FPGA are tested before  integration with the interposer (Known Good Die), so the  driver and FPGA wires are presumed good and only the


output


cutput


interposer is under suspicion of failure.


Interposer failures can be classified as opens or shorts  based on their failing signatures.  Opens are seen as stuck6


M


at-high from the scan test, on the receiver output only.


Corr


Open Failure


Failures are classified as shorts if a stuck-at-low is  observed, or if a stuck-at-high is seen on both the receiver  and driver scan chain.  Node-to-node shorts which translate


Interposer Short (Two Node Short)


physically to microbump to microbump shorts can also be  observed using the correct patterns over multiple vectors.


input1


Input1-0


Node-to-node shorts on the interposer itself are unlikely, as


cutput1


output1


by design all wires are shielded with either power or


Input2=0


irput2


ground, so wire-to-wire shorts on the interposer will always  be observed as stuck-at-high or stuck-at-low.


output2


ostput2


Figure 2.  Diagram for Interposer Testing Methodology (Open Testing)


Electrical isolation to physical mapping can be taken care  of any number of ways, but we use the failing pin and cycle


to map to the test configuration’s net, that net to map to the


device model tile and wire resources, and then finally  device model resource to physical layout and its associated  microbump location on the FPGA.  That location is then  mapped to the interposer based on the failing FPGA  location on the interposer and then the wire of interest can  be traced to reveal the interposer wire and both microbump  locations in the layout.   There is a small database that  contains all of these mappings, precompiled for each  interposer product, and a script to do the lookups on  individual die failures for quick turnaround times.


The interposer testing concept and interpretation were  then verified for the interposer open and short failures by  using FPGA resources to reroute the failing nodes to the


external BGA balls.  The input signal was clocked into the  failing node and the output signal was monitored using an  oscilloscope. Figure 3 shows a waveform of an open  circuit. The output signal reveals that it is stuck-at-high,which confirms the correct interpretation of an open net. Similarly, the graph of the interposer short (two nodes  shorted) is shown in Figure 4.  In this example, the  waveform of output2 tracks the waveform of output1, or  vice versa regardless of the inputs. This characteristic  implies that the two microbumps are shorted to each other.


Figure 3. Waveforms of a good net vs. an open net


Figure 4. Waveforms of two nodes short


Figure 5 shows an example of the fault isolation and  physical FA of the metal interposer open failure utilizing  the interposer testing methodology to quickly identify the  failing location.  The ATE failing net was first translated  into x-y coordinates of the failing microbump pairs.  In this  example, there were two failing pairs with open signature. The failing pairs were then mapped onto the physical  layout locations as shown in Figure 5a.  Once the location  of the suspected failing microbumps had been identified by  physical counting, subsequent cross section was then  performed by targeting the two failing microbumps (one  pair) at the same time.  The PFA result showed that the  open failure was due to non-wet microbump as shown in  Figure 5c.


“Functional” Path


Or


Interposer wire


FPGA Driver FPGA or IP


Reciever


open


6111


Scan Path


net1=100MHz,net2=0


net1=0,net2=100MHz


Die3


(b


Figure 5. Analysis of microbump open failures.  a) CAD layout mapping


showing two pairs of failing microbumps,  b) magnified view of the


microbump, and c) and cross section result showing non-wet microbump.


Mecal Dafec


计第


The metal interposer short failure is also demonstrated in  the example below. This device failed for short on two


(e1290.500.471.87)


Die4


(+1000.503-9567.00)+1000.5038460.02)


pairs of the adjacent nets as shown in the layout in Figure 6.


The short could happen either at the microbump pair on


O


Die1 or on Die2.  Using X-ray imaging, a metallic particle  defect was found between the failing microbumps on Die2. Subsequent physical FA by cross section confirmed the  solder particle short between the two failing microbumps. See Figure  7.


Figure 6. CAD Layout and mapping of the metal interposer  short failure locations


Figure 7.  X-ray image showing metallic particle between the  microbumps (a) and SEM cross section image showing solder  particle shorting between the two microbumps (b).


The two previous examples showed the failures at the  microbumps.  However, the interposer testing methodology  also works for interposer metal interconnect failures, as  shown in Figure 8.  Based on the pattern of the failing  microbumps (alternating between good, bad, good, bad), the defect is most likely at the interposer metal traces rather  than at the microbumps.  The physical FA was focused on


the interposer metal traces by parallel lapping off the top  metal layer of the interposer to expose the metal 3 layer  beneath. A metal masking defect was found at the  interposer metal 3 causing multiple open traces as shown in  Figure 8c, which exactly matched the failing nodes in


pee


Figure 8b.


pair


74902


210 pair


Figure 8.  CAD Layout of the metal interposer open failures (a &b) and PFA result showing  metal defect at interposer Metal 3 layer (c).


III.


INVESTIGATIONS OF IO PARAMETRIC FAILURES


Die1


sq


Interface issues pose significant challenges for the


(+4318 5 +9485 2)


physical FA because they are often difficult to see even


(+4318.5 +6855.b


with high resolution FE-SEM and FIB cross section.  Some


Die2


cases require the use of advance tools and techniques.  For  this second case study, we will investigate a low yield/REL  issue for Voh/Vol failures in the 3D IC devices. We will


discuss the problems and the struggles we encountered with  this type of failure.  We will also describe the use of cross  sectional microprobing technique in conjunction with the


Kelvin resistance technique to successfully isolate the  failure location followed by FIB cross section to confirm  the defect at the interface of the failing microbump [5].


Voh/Vol is a parametric test that measures the output  high and output low for an IO pin.  Any high resistance


he2


path from a BGA ball through the package substrate, C4  bump, interposer, and to the die metallization and vias  could be the cause of this failure.


This type of failure took significant amount of time to  analyze.  Several initial attempts were unsuccessful and  inconclusive because no obvious anomalies were observed,even after extensive PFA. What made this case especially  challenging was that the failures were marginal and  sometimes could be recovered during unpowered curve tracing by just increasing DC sweeping voltage (i.e. from  1V to 2V).  See Figure 9.


Figure 9. IV curve of  Voh/Vol failing pin (red curve) showing  marginally high resistance at negative side of diode.  Positive side also  showed similar high resistance but less obvious.


up Uites Appications Heb 5946Woveloms


Tektronby-x ABun/StopAcqMode [Average Tog|Interal Clock200MHz?PulseArpihude▼产期me 4216m8


C350.00mV/dy R150.00mWv R250.00mVdv R350.00mWtliv Sulistrate who die


P450.00mVAy Waveform


Figure 10 .  TDR result of the failing pin (red) indicating high


impedance path, possibly at the microbump or C4 region


Using the existing non-destructive tools and techniques (curve trace, TDR, C-SAM, and X-ray), the fault location  was narrowed down to either the microbump region or in  the die (Figures 9 and 10).   Since the die had already been  wafer sorted and presumed good, a defect was more likely  to be at the microbump region.  Therefore, the physical FA  focus was on the microbump. However, subsequent  mechanical and FIB cross sections of several failing  microbumps did not reveal any obvious defects.  Many  attempts had been made to analyze several similar Voh/Vol  failures, but the results were inconclusive without further  Rel stress and fault isolation.


Based on the initial results, it was believed that the  microbump had an interface issue such as oxidation or a contamination layer which would make it very difficult to  see.  To make the interface issue more visible, it was  decided to subject a few failed units to Temp Cycle.  Time  0 only showed 7 failing pins, but after 75 cycles 177 pins  were failing.  Additional fault isolation showed that the  new failures had the same failing signature as the original  failures. At this point, we expected the failures to be more  obvious. The same PFA techniques were used, but this time  Kelvin resistance measurement technique was also  employed to electrically identify which interface of the  microbump had high resistance.


3V6S8120


|Pro 0 points|Bad pin A24|Good pin|
|---|---|---|

|ato a1|46.mQ|48 mQ|

|a to b|23,070 mQ|52 mΩ|

|btoc|56 mQ|50 mΩ|

|c to C4 bump|75mQ|71 mΩ|

110*0062DR2012


Horiz/Div (V)50m


vert/Dw (A)500


10.5


exdosap/ ap


-sen


Peak Puwer (W)


-roen


.080


0-)


Peak Voltage (V)


-tsen


058


w*w*W


-2000


Collector Polarity-Fulwave


+250


To C4 Sump


Comments


Forcing 1mA constant current using


-300u


SNLG-Pr A24Ro GND after


Microprobing of the failing microbump interface


TOB 266X


shows high resistance of -23 Q. Note that only


3900


Red-Bod FinA24


-1/5 of the microbump exposed to prevent


to measure voltage drop using Kelvin


smearing at the interface, which would make the


+0o


Geen-GoodpinA2e


failure recovered.


setup.R=VII


(bga ball)GND


micro-probing across each intortace


Keithley 2400 SourceMeter, and


(bga ball)


太 10substrateC4interposeru-bump w-Senne+TMA


Collector Supply (9%)


uopeeu oy


-o


Figure 11.  Cross sectional microprobing and 4-wire Resistance  measurement technique of the failing microbump.  The interface between


-500u050403020.1


microbump Al pad and the copper pillar shows high resistance


Ref Open


RS 50.00mWtiy


Substrate + Interposer


Figure 12.  FIB cross section images of high resistance microbump showing


Measteeiment


separation between Al pad and the UBM interface of the microbump


PkPk C3八


125.0114m9


SN16-Pin A24


The 4-wire resistance measurement setup and the results


Gaod Unll Pin A24


are shown in Figure 11. However, landing 4 probes on a


High resistance


single microbump with approximately 40 um feature size  was quite challenging.  A creative approach was developed  by using one of the GND BGA balls to replace one of the


-29.00knd


70.00per


probes by utilizing the parasitic diode built in CMOS


RS▲[50.0c0mvi品QQ700004410℃11:07AM2/17/2012


process, and replacing a second probe by using the BGA  ball of the failed IO pin.  Then use the first and second  probes as the Sense+ and Sense- to probe and measure the  voltage drop across different interfaces.  The Forcing  current (1mA) was injected into the GND BGA ball  through the forward bias diode of the die.  The resistance  values were calculated by dividing the voltage drop by the  current (R=V/I).


This resistance measurement was a crucial step in isolating the failure because the interface issue such as  oxidation or contamination are often very difficult to see  even after FIB cross section.   Using the microprobing and  resistance measurement on this Voh/Vol failure, the high  resistance interface was isolated to be between top die  Aluminum pad (Figure 11 point-a) and the UBM interface  of the microbump (point-b). Note that although a 2-point  resistance measurement would have been possible to use, there were measurement errors due to fixture setup  and  contact resistance between each metal probe and the  semiconductor material. Using four-wire Kelvin  measurement eliminates these measurement errors [7].


After the suspect location was identified by the 4-wire  measurements, FIB cross sectioned was then performed at  the microbump interface. The innovative technique of  performing FIB cross section perpendicular to the original  mechanical cross section surface revealed delamination at  the interface of the microbump UBM layer and the top die  aluminum pad caused by weak interface.   See Figure 12.


After further investigation the root cause was due to  organic PBO residue on the microbump Al pad.


IV.


INVESTIGATION OF HIGH ICC FAILURES


For this third case study, we will discuss a technique to  deprocess the silicon interposer die using KOH [8] to  investigate a Power to GND short failure due to solder  extrusion at the C4 interface to the interposer. This device  failed after Level 4 preconditioning for high Icc failure. This type of failure is difficult to analyze because the Vcc  routing is global and fault isolation has to cover a large area  of the die.  In addition, the 3D stacking of the dies adds  more complexity to the analysis.  The defect could be either  on the die, interposer, or at the microbump, C4 bump, or in  the package substrate. TDR analysis would not be able to  provide useful information because of its limitation to  localize the power to GND short.  Thermal emission was  first utilized to identify the location of the short.  Although  a hot spot was detected, it only provided the x and y  location but not the z-depth information [9].  See Figure 13.


Reflowed solder bridging


Figure 13. Thermal hot spot of Vcc to GND short


Eoer


Since the device was initially good and the short  happened only after the precondition, it was strongly  suspected that the short could be due to reflowed solder  bridging.  Therefore, the most likely place that the short  could happen would be at the C4 bump or at the  microbump.  One of the physical FA approaches was to use  parallel polishing to thin down the silicon substrate and  then etch off the remaining silicon using KOH at both the  die level and interposer level.  The purpose of using the  KOH etch in combination with polishing was to obtain  uniformity across the entire surface area for global  inspection. Cross section approach would have been  possible but it would be difficult to hit the exact short  location if you can’t see it.


Since this device was assembled in a ceramic package, it  would have been very difficult to parallel polish off the  package from the BGA ball side. Therefore, the best  approach was to polish from the die side.  This technique  started by thinning down the die silicon to about 40 um and  using KOH solution (125C on a hot plate for ~ 1 hour) to  etch off the remaining silicon and then continue polishing  off the die metal and dielectric layers to expose the top of  the microbumps.  Careful examination of the u-bump layer  did not show any anomalies.  The PFA was then continued  to the second suspected location at the C4 bump region by


polishing off the microbumps and thinning down interposer  substrate.  KOH was used again to etch off the remaining  silicon to expose the C4 bump layer.  Subsequent optical  inspection revealed solder bridging between the failing Vcc  and GND C4 bumps at the hot spot location (Figures 14, 15). The technique of using KOH to dissolve the  remaining interposer silicon allowed us to inspect the entire  C4 area and locate the shorted bumps. The suspect C4  bump was subsequently cross sectioned and reflowed  solder was confirmed (Figure 15).


The cause of this solder bridging was due to underfill  delamination between the SiN passivation layer and C4  underfill caused by high TCE mismatch between the silicon  interposer (TCE=2.6) and the HiCTE ceramic package (TCE=12.3), especially at the die corners where the stress  is the greatest.  This delamination issue was resolved by  optimizing the underfill.


Figure 14.  Overview optical images of the C4 bump region after the KOH  etch showing reflowed solder bridging between VCC and GND bumps


Figure 15.  High magnification image of solder bridging after KOH etch.  The x-section image shows the interfaces where delamination happened.


V.


CONCLUSION


Fault isolation and physical failure analysis of 3D IC  devices is far more complex and challenging than  traditional monolithic devices.  With 3D IC devices, the  chance of not finding the failure mechanism is high due to  the multitude of potential failure locations between the die, silicon interposer and package substrate.  However, with a  creative thinking and applying innovative techniques and  methodologies using existing lab equipment, successful FA  results were achieved with high success rate (>90%) and  short turn-around time.  This paper has shown how die-todie interconnect shorts and opens, die–to-interposer high  resistances, and Power–to-GND shorts in a 3D IC devices  can be analyzed by using existing lab tools in a novel  way  to achieve the desired results.


The authors would like to thank their Xilinx FA team (Violeta Cabacungan and Joy Tarayao) for their PFA supports.  The authors would also like express gratitude to  the REL/FA management for their encouragement and  support.


REFERENCES


1. Scott Thompson, et al., “MOS Scaling:  Transistor


Challenges for the 21th Century”, Intel Technology


Journal Q3’98


2. Xilinx Inc White Paper, “Xilinx Stacked Silicon Interconnect Technology Delivers Breakthrough FPGA Capacity, Bandwidth, and Power Efficiency”,December 11, 2012


3. M. Santarini, Xilinx  “2.5D ICs Are More Than a


Stepping Stone to 3D ICs”, Published in EE/Times


3/27/2012


4. Raghunandan Chaware, et al., “Assembly and Reliability Challenges in 3D Integration of 28nm FPGA Die on a Large High Density 65nm Passive Interposer”, ECTC 2012.


5. C. Maxfield, “2D vs. 2.5D vs. 3D ICs 101”, Published


in EE Times 4/8/2012.


6. Eric Beyne, Ingrid De Wolf. “Failure Analysis for 3D TSV Systems” Product Level Reliability Workshop,IMEC  July 14, 2011.


7. Dale Cigoy, Senior Applications Engineer, Keithley Instruments, Inc. “Accurate Low-Resistance Measurements Start with Identifying Sources of Error”. Keithley White Paper


8. Yuanjing (Jane) Li, nVidia. “Advanced Physical Analysis Methodology for Yield and Reliability of 28-nm, Bulk-Si, Flip-Chip ICs Using SEM and Backside Deprocessing” ISTFA 2012.


9. C. Schmidt et al.  “Non-destructive defect depth determination at fully packaged and stacked die devices using Lock-in Thermography”  17th IEEE International Symposium on the Physical and Failure Analysis of Integrated Circuits (IPFA), Singapore,2010, pp 1-5.


Advanced Physical Inspection Methods for Counterfeit IC Detection


Sina Shahbazmohamadi, and Domenic Forte, and Mark Tehranipoor


Center for Hardware Assurance, Security, and Engineering (CHASE) University of Connecticut, Storrs, CT, USA


Email: {sina, forte, tehrani}@engr.uconn.edu


The remarkable increase in counterfeit parts (a factor of 4  since 2009) [1] is a huge reliability and security concern in  various industries ranging from automotive electronics to  sensitive military applications increasing the possibility of  premature failure in critical systems [2-5]. Counterfeit parts  can also incur a great financial loss to legitimate electronics  companies [6]. The issue is even more alarming as the  counterfeiters use more sophisticated methods making  counterfeit detection a much harder task [7-8]. Therefore, it is  reasonable to develop more advanced counterfeit detection  methods targeting a more efficient detection of sophisticated  counterfeited parts.


Possible methods for counterfeit electronic parts detection can  be classified into two main categories: physical inspection and  electrical testing [3, 5, 9, and 10]. The physical inspection  techniques can potentially be extended to different integrated  circuit (IC) types (analog, digital, mixed-signal, FPGAs, and  memories.). However there are some challenges:  First, there  is no specific equipment or test technique that can target all  the defects associated with counterfeit ICs. Previous efforts  have shown the possibility of more than 60 [9-10] different  exterior, interior and compositional defect types making it  difficult for any single instrument to detect all. Therefore, one  has to resort to utilizing different instruments ranging from  optical microscopes to high-tech Scanning and Transmission  electron microscopes (SEMS and TEMs) making physical  detection a costly and time-consuming process. Second, most  methods require a subject matter expert (SME) to interpret the  test results which in turn leads to additional cost, inefficiency  and inconsistency and prevents us from automating the  process. Third, the issue associated with physical inspections  is the destructive nature of most tests. Having access to the  interior features is inevitable for complete counterfeit  detection tests which usually entails decapsulation of the part, which is inherently destructive method. The common practice  for detecting remarked and black-top coated parts is also based  on chemical or mechanical destructive tests. In terms of using  microscopy and spectroscopy techniques, one has to do the  imaging and analysis on various locations which entails  multiple sessions of imaging which further adds to the cost  and time in addition to the likelihood of damaging the chip  while handling. Finally, counterfeit detection usually requires  having a known authentic sample (commonly referred to as


the “golden IC”) for comparison. This can raise issues where  such a golden IC may not exist or difficult to be obtained.


The major contribution of this paper is to tackle these issues  by introducing and optimizing two novel three and four  dimensional imaging techniques that can provide us with the  necessary information on interior and exterior geometry along  with the material composition for the parts under test: FourDimensional Scanning Electron Microscopy and Dual Energy  3D X-ray Microscopy. It will be shown that by applying the  proposed modifications, we can successfully detect all the  defects associated with different counterfeit parts through a  single-imaging session. This could significantly reduce the  cost and time of implementing physical inspections. The  proposed methods are also totally non-destructive, causing no  damage to the part under test while successfully detecting the  interior defects. Finally, the presence of quantitative results as  opposed to qualitative images can potentially eliminate the  need of the SMEs’ interpretation and expertise which can  further reduce the associated cost and improve the detection  accuracy.


Logic State Imaging (LSI) using Infra-Red Emission  Microscopy (IREM) [1-4] has been an indispensable  technology for silicon CMOS process development and  product debug applications. Its main limitations are relatively  poor spatial resolution due to the broadband near-infrared  photons emitted, and poor Signal to Noise Ratio (SNR) with  low voltage and low leakage processes and products. Continuous-Wave Laser Scanning Microscope (CW-LSM) based Signal Imaging and Probing (CW-SIP) [5-9] technology  is also widely used. It features inherently better spatial  resolution than IREM, due to the use of monochromatic  1319nm or 1064nm laser light, and high SNR due to its  weaker dependence on voltage and leakage, and, for signal  imaging applications, the use of narrow band detection to  reduce noise. However, CW-SIP can only detect modulating  signals, so it couldn’t previously be applied to LSI. In this  paper, we introduce an innovative approach that overcomes  this limitation to enable Laser Logic State Imaging (LLSI). Actual fault isolation and design debug cases using this  technology are presented to show its advantages in terms of  resolution (>50% better), SNR (>2X better) and throughput  time improvement, especially at low voltages (down to  500mV).


IREM based LSI [1-4] has been an indispensable technique for  Intel’s process development and product debug since its  introduction in 2001. Besides providing details of the nodal  logic states when the device clock is stopped, IREM LSI can  be used to find the locations of process defects. This technique  is illustrated in Fig. 1. It takes advantage of the fact that when  silicon based CMOS transistors are in the off-state, with  leakage resulting from the strong electric field across the  source and drain regions, they emit detectable near infrared  photons.


Our state-of-the-art IREM systems use a sensitive liquid  nitrogen cooled InGaAs Focal Plane Array (FPA) detector  with high quantum efficiency and SNR over the 1100nm ~ 1600nm wavelength range. A silicon Solid Immersion Lens (SIL) with Numerical Aperture (NA) approaching 3.3 over the  same wavelength range provides high resolution imaging and  high photon collection efficiency.


The quality of IREM LSI images depends strongly on both the  operating Vcc and the small amount of off-state leakage current  flowing through the CMOS transistors. Unfortunately, with  continued process scaling leading to lower operating Vcc (< 0.65V) and ultra-low leakage transistor architectures, the  IREM signal has gotten very weak, leading to poor SNR of the  LSI data. In addition, the spatial resolution of IREM-LSI is  limited by the broad-band nature of the CMOS photon  emission process. With continued shrinking of dimensions in  advanced silicon process technologies, now reaching a  minimum feature size of ~ 15nm, this limitation definitely  imposes significant challenges for pinpointing defect locations  and determining nodal logic states within the ~ 100nm  accuracy required for process development, design verification  and power debug (i.e., identifying circuits which draw excess  power).


Figure 1. “OFF” state leakage current (under strong field) produces infrared emission image (middle) showing the logic  state of each inverter’s output.


CW-SIP technology [5-9] has been in use at Intel for CMOS  process technology development and post silicon circuit debug  since 2010. CW-SIP takes advantage of the fact that when  CMOS circuits are actively switching, both the local electric  field and the local free carrier density modulates, leading to a  small modulation of the local refractive index and photon  absorption coefficient (on the order of a few hundred parts per  million). As a result, a continuous wave laser beam (typically  1064nm or 1319nm wavelength) scanned over a region of  interest (ROI) in the device under test (DUT) will have its  reflected phase and intensity modulated when it is incident on  the modulating/switching nodes. An example of signal  imaging using CW-SIP is shown in Fig. 2. As can be seen in  the middle image, only the actively modulating/switching  nodes are detected. As a result, traditional CW-SIP


methodologies cannot be used for LSI, where the chip is held  in a static state.


Figure 2. Top: LSM reflected light image. Middle: signal  image showing only the actively switching/signaling devices. Bottom: overlay of the top and middle images, which enables  us to quickly pinpoint and probe the active devices for fault  isolation and design debug applications.


For CW-SIP, a high speed and high sensitivity Avalanche  Photo Diode (APD) is used to detect the modulating reflected  laser beam. The APD output is electrically amplified using


one or more wideband microwave amplifiers, then split and  input to both a spectrum analyzer and an oscilloscope. The  spectrum analyzer, set to low resolution bandwidth (typically ≤1kHz) for noise rejection, and tuned to the switching  frequency of interest, is used for signal imaging. Its output is  digitized simultaneously with the normal reflected light signal  used to form the LSM image, as the laser is raster scanned  across the ROI. The high-bandwidth, real-time sampling  oscilloscope provides timing waveforms, which can be  acquired when the laser beam is statically ‘parked’ on an  active node.


The advantages of CW-SIP are: 1) Superior spatial resolution (>50% improvement over IREM) due to a combination of the  relatively short wavelength, monochromatic laser light used  and the confocal imaging of the LSM, and 2) High sensitivity  and SNR due to its relatively weak dependence on voltage,


者古


and on the fact that the signal does not depend on the absolute  value of Vcc, but rather on the magnitude of its modulation. Results show that CW-SIP can detect Vcc modulations as


888be0


small as 50mV. For signal imaging, the use of a spectrum  analyzer, set to a low resolution bandwidth centered on the  known and fixed frequency of interest, enhances the SNR  tremendously.


In this paper, we introduce an innovative extension of CW-SIP


800


to enable its application to LSI. This new Laser Logic State


xa


Imaging (LLSI) technique is based on modulating the internal


888


power rails supplying the DUT’s circuits of interest. LLSI has


00G.


been found to be superior to IREM-LSI in terms of resolution, SNR, and scalability to lower Vcc, ultra low leakage devices,


"


and process nodes beyond 14nm.


E


In the following sections of this paper, we will compare  IREM-LSI to LLSI, briefly describe the equipment used, and  discuss the setup and test procedures. Some examples will be


081-


presented, including a few successful LLSI defect


688085--


localizations and design debug cases where IREM-LSI was


.


not successful.  At the end, a summary will be given,


8ESHSF38


highlighting possible future developments and deployment of  this new technology.


83 888


Experiment Setup and Procedures for LLSI


雷台


The CW-SIP tool used for this study is LSM based, but the


是告


system also incorporates IREM capabilities. Figure 3  highlights the functional blocks of the optical column, as  configured for CW-SIP operation. For IREM, the components  in the dashed box are moved out of the beam path to allow  photons emitted by the DUT to be collected by the camera. The camera is a liquid nitrogen cooled, InGaAs FPA). Both  the traditional IREM and CW-SIP techniques (which also goes  by various other names) have been well documented in the  literature [1-9].


Figure 3. Block diagram of the CW-SIP tool that enables  LLSI. 1) Device under Test and Tester. 2-3) Solid Immersion  Lens. 4 – 7) various waveplate, beam splitter and mirrors/scan  mirrors. 8) collection lens for return laser signal. 9) detector


Function"Modulated"


and 10) collimation lens for input laser beam. Components


Power Supply


shown in dashed box can be removed from the beam path to


Generator


allow IREM acquisitions using the camera.


、0


Oscilloscope


To perform LLSI, the supply rail connected to the circuits of


interest in the DUT must be modulated, as illustrated in Fig. 4.


Power SupplyLoadboardHigh Current


Multiple ways to achieve this were tried and evaluated. One


Tester


proven approach is to take advantage of on-die Design For  Debug (DFD) features, such as the On-Die Droop Inducer (ODDI) that are available on Intel SOC  microprocessors [10-13].  The ODDI circuitry allows users to  locally modulate the internal voltage level on a power rail at a  fixed and known frequency. Another method we investigated  successfully is to directly drive a small Vcc modulation  externally to the appropriate power pins of the DUT. A third  method is to make use of Fully Integrated Voltage Regulator (FIVR) technology [14,15]. Here, a small, periodic voltage  signal is injected into the sense line of the FIVR’s feedback  loop, causing the FIVR to ‘compensate’ by modulating the  local Vcc power rail.


Figure 4. Illustration showing the ‘injection’ of a small Vcc  modulation into a power plane of a DUT. Typical Vcc is ~550mV to 1.0V, depending on the failure/fault signature, while typical Vmod is ~100mV, peak-to-peak.


All three methods allow a small Vcc modulation to be injected  into the power rails of interests. We characterize each DUT, measuring both the frequency response and the Vcc modulation


amplitude on the targeted power rails that can be tolerated. To  maintain the DUT’s nodal state during LLSI, the Vcc


□


Laser Logic State Image


modulation amplitude must be kept below the switching  threshold. At the same time, the amplitude needs to high  enough to be detectable by CW-SIP. Peak-to-peak Vcc  modulations of about 50mV ~ 100mV have been successfully


☑


used, with Vcc static levels ranging from about 500mV to


1.0V, dependent on the DUT fault conditions.


For DUT that do not have the ODDI or FIVR features (or do  not have them on the power rails of interest) we use the setup  illustrated in figure 5 to generate a Vcc modulation. The DUT


Laser Scauming Microscope Inage


is powered on and exercised normally using the High Current


10


Power Supply (HCPS) connected to the Vcc power rail of  interest. The Modulated Power Supply (MPS) output is  connected to the DUT’s Vcc sense line to inject ‘noise’ into the  HCPS’s feedback loop.  The HCPS reacts to this ‘noise’ by  modulating its output.


Figure 5. Block diagram of setup used to inject a small Vcc  modulation for DUTs without ODDI or FIVR features on the  power plane of interest.


Since each particular DUT setup and Vcc power rail has its  own frequency response and maximum tolerable modulation  level, both must be characterized. The frequency response of a  setup is found by ‘freezing’ the DUT at a particular state, then  sweeping the frequency of the function generator driving the  MPS while monitoring the DUT’s response. An oscilloscope  is used to monitor the MPS’s output to see both the peak-topeak value and the shape of the waveform being input to the  DUT’s Vcc sense line. The DUT’s Vcc sense line is


0.1Vmod9州


simultaneously monitored to observe the DUT’s response.


<Vccfub1


This process allows us to determine the input Vcc modulation


+VccfubO


CORE is


-Vcclfub2


frequency that provides good DUT Vcc response while being  high enough to avoid the low frequency noise of the CW-SIP  system. The maximum tolerable modulation level is


<Vccfub3


determined by setting the function generator to the selected


↓0.9vcc22nm/14nm Devices


modulation frequency, then increasing the MPS’s output level  while looping the DUT test pattern and observing its pass/fail  status.  For best LLSI sensitivity, the external function  generator and the MPS are set to the selected frequency and  highest tolerable Vcc modulation level.


The procedures for setting up the tester/DUT and CW-SIP tool  to acquire normal IREM-LSI and LLSI is outline in Fig. 6. With traditional IREM based LSI, a test pattern is first run on  the DUT to exercise the desired ROI. Then the clock signal  that drives the test pattern is ‘frozen’ at a particular clock


cycle to set the devices within the ROI to the desired logic


states. An IREM image is taken. Then the test pattern is re-run


and the clock cycle at which the test pattern is frozen is 本4AAadvanced to set the devices within the ROI to different logic T公L.PMOSstates. A second IREM image is taken. Both images are then 。b compared to see which devices change state. Failing devices


。L


Inverter 1


either fail to change state when they are supposed to, or will


Inverter 2


give no emission at all. This enables both defect localization  for process development and yield improvement, and design


NMOS


off


debug to locate the circuits/devices that are not operating as  expected.


|Dock the DUT on Tool|Dock DUT on Tool|
|---|---|

|↓|↓ Cotnect "MPS" to selected power plane -setse line ↓|

|Turn on all control/power on the DUT|Turn on all control/power on the DUT|

|↓|↓|

|Run desired test pattern|Run desired test pattern|

||→|

|Freeze clock afinterested cycle|Freeze clock at interested cycle|

|↓ ↓↑ Inject Vmd to selected power plane Collect LLSI data|↓ ↓↑ Inject Vmd to selected power plane Collect LLSI data|

|Collect IREM-LSI Image-Data||

Figure 6. Block diagram of the IREM-LSI flow (left) and new  LLSI flow (right).


In LLSI, additional steps in the procedure are required. First, setup the device and test pattern just like regular IREM-LSI. Then, freeze the clock at the desired cycle number in the test  pattern. With the clock frozen, use one of the three methods  described above to modulate Vcc at a pre-characterized  frequency, with amplitude below the pre-characterized  threshold at which the DUT switches states. The CW-SIP  system is then tuned to the Vcc modulation frequency and a  frequency map of the ROI is acquired. This is repeated at a


lnverder 1DEo


different clock cycle, just like IREM-LSI, and the two images


compared. With the DUT frozen at the desired logic state, the


Inverter 290


frequency map highlights those devices that are ‘connected’ to  the modulating Vcc.


Figure 7 shows a LLSI of two inverters on an Intel 14nm test  chip. These inverters were frozen at a particular logic state  using the pattern/clock control of the DUT stimulus with static  Vcc of about 650mV. Vcc was then modulated by about 100mV  and the inverters imaged using the CW-SIP tool. As shown, both nFETs and pFETs give clear signatures when they are in  the on-state, allowing the logic states of the inverters to be  correctly determined.


Inveqte/ 2


Figure 7. LLSI of two back-to-back inverters. As shown, only  the on-state transistors give a strong CW-SIP signal, which  allows the logic state of the inverters to be correctly  determined.


Results and Discussions


Figure 8 compares the IREM-LSI (left) and LLSI (right) sightings of a defect localization and fault isolation case on an  Intel 14nm MPU. This is one situation where we were able to  acquire both IREM-LSI and LLSI data. Each image data set  shown consists of an overlay of two separate images acquired  at two different clock cycles of the test pattern. One image in  each data set is colored red and the other is colored green. In  both data sets shown, yellow (= red + green) indicates no  difference in the acquired data between the two clock cycles, i.e., no change of state. Within the red boxes, green indicates a  logic state of ‘1’, while red indicates a logic state of ‘0’.


Figure 8. IREM-LSI (left) and LLSI (right) data from a 14nm  test device. Yellow indicates no change of state. Within the red  boxes, green indicates a logic state of ‘1’ and red indicates a  logic state of ‘0’.


In Fig. 8, the IREM-LSI data (left) shows that the inverters  within the red boxes did not change state as expected, since no  red ‘dots’ are observed. On the other hand, the LLSI data (right) does shows the expected logic state change. In this  case, clearly the IREM-LSI data is not giving us the correct  logic state information. The reason is a combination of low  SNR and poor spatial resolution. In practice, the LLSI spatial  resolution is found to be more than 50% better than IREMLSI. This is due to the fact that the 1319nm laser used for  LLSI has about 25% shorter wavelength than the longest  emission wavelength, ~1600nm, detected by the IREM-LSI


camera. In addition, the confocal imaging capability of the  LSM used for LLSI improves the resolution by ~40% over  normal wide-field imaging, such as used for IREM-LSI.


The low SNR for IREM-LSI is a result of the very different  nMOS and pMOS photon emission intensities under similar  Vcc bias conditions, and the exponential dependence of  emission intensity on Vcc. LLSI signal strength, on the other  hand, does not depend on the static Vcc value, but only on the  modulation level. LLSI thus better maintains its SNR at low  voltages. In addition, the detected signal strengths between  nMOS and pMOS are very similar for LLSI.


Figure 9 shows an IREM-LSI image of the logic area of an ondie cache in a 14nm MPU. Images taken at both the READ ‘1’ and READ ‘0’ states are identical. This means that, once  again, the expected activity is not properly captured. Indeed, some of the active devices in the ROI do not show any  emission at all, regardless of their logic state.


Figure 9.  IREM-LSI image of the logic area of the on-die  cache of a 14nm MPU. No distinguishable logic-state  emission or changes in the circuits of interest were found.


Figure 10 shows LLSI images of the same area on the same  DUT, taken with Vcc at about 850mV and Vcc modulation  amplitude of ~ 75mV, peak-to-peak. The LLSI data clearly  captures the expected changes in the devices’ logic state, even  for those weaker devices that showed no emission signal at all  in the IREM-LSI data. This example again highlights the  superior SNR of LLSI over EMMI-LSI.


和


Figure 10. LLSI images of the same region in the same DUT  as Fig. 9. (A) READ ‘1’ state, (B) READ ‘0’ state, and (C) image showing (A) and (B) overlaid. In (C) yellow regions  indicate devices that do not change states.


Figures 11 is shown to point out a unique feature of LLSI- the  ability to capture data on passive devices such as decoupling  capacitors, along with the normal logic state data. The yellow  boxes in the upper image enclose several active ‘bits’ that  changed logic state under the control of the test pattern. These  show up as red and green regions. Bit 0 is yellow, as it does  not change state. The dotted white box shows some of the


A


C


decoupling capacitors in the field of view. Since they are  passive devices which do not change state, they are also  colored yellow.


Figure 11. LLSI data highlighting the ability to capture  modulation of passive devices such as decoupling capacitors. Top: Overlay of two LLSI acquisitions taken at different clock  cycles. The yellow boxes show some of the cells that actively  changed logic states (red and green regions). The white  rectangle shows some of the decoupling capacitors that are  captured in the LLSI data. Bottom: CAD overlay on one of the  LLSI images showing how the decoupling capacitors (red  rectangle) can be used to aide CAD overlay alignment.


Passive devices, like decoupling capacitors, normally don’t  emit and won’t show up in IREM-LSI data. However, since  each capacitor is connected across Vcc and Vss, the small Vcc  modulation used for LLSI will modulate their electric field  and charge density, allowing  them to be ‘imaged’ using LLSI. They are clearly visible in Figs. 8, 10 and 11. The ability to  capture these passive devices using LLSI helps to speed up  CAD overlay alignment considerably (Fig. 11, bottom) and  allows precise alignment to be easily achieved.


Figure 12 shows another example of the ability to capture both  active and passive devices using LLSI. This data was acquired  on a 22nm System On a Chip (SOC) product. IREM-LSI  images (not shown) failed to capture any features of interest. The reflected LSM image is shown on the left. The LLSI  image on the right was captured concurrently with the LSM  image. The LLSI image clearly shows the logic states of the  active devices (see Fig. 13) and also highlights many passive  devices. The well defined active and passive devices in the  LLSI image can speed up CAD overlay alignment compared  to using the LSM image alone.


Bit 0 0-0


Bit 5 0-1


B批310


Bit 2 0-1


Bit 7 1-0


骨 份份 费 烧 9991 烧 100 普 贷


Figure 12. 22nm SOC reflected LSM image (left) using  1319nm, and LLSI image (right) collected concurrently with  the LSM-image. The well defined active and passive devices in  the LLSI image can be used to speed up CAD alignment.


Figure 13 shows a zoomed-in view of the same SOC as  Fig. 12. The left image shows an LLSI image overlaid with  CAD layout. The right side shows a zoomed in view of the  LLSI image. The three pairs of rectangles highlight cells that  are at three different logic states, as controlled by the tester  patterns as designed. The clear differences in the LLSI pattern  for the cells at different logic states provides yet another  demonstration of the ability of LLSI to capture logic state  information.


Figure 13. SOC-LLSI with CAD overlay on the left, and  zoomed in to those cells of interest on the right. Clear  differences in the LLSI of the cells within the rectangles  further demonstrate the ability of LLSI to capture logic state  differences.


Figures 14-16 show LLSI of a circuit with 3 bit cells on an  Intel 14nm MPU. The logic state of each bit was changed by  freezing the test pattern at two different clock cycles. LLSI  was acquired at the two frozen states (Figs. 15 and 16). In this  case,  there is no IREM-LSI equivalent images as there was no  emission detected at all.


Figure 14. 1319nm LLSI image with CAD overlay of three bit  cells and their control logic.


With these images, we demonstrate that both 1319nm LLSI (Fig. 15) and 1064nm LLSI (Fig. 16) give the correct logic  state of the bit cells, as can be seen from the embedded truth


VOUB


table in the figures. This result shows that an additional ~20% improvement in optical resolution for LLSI is available. Note  the interesting, but not yet fully understood, differences in the  details of the LLSI data between the two different laser  wavelengths. One difference is the abnormal 1064nm LLSI  signal, indicated by the arrows in Fig. 16. This ‘spot’ does not  appear in the 1319nm LLSI data.


There is another aspect of the LLSI base technology that we  did not explore here, but is widely utilized: Laser Voltage  Probing. With the same CW-SIP tool, we can park the laser  beam at selected individual devices and get waveforms that


220390220392


Bit 01


220390


220392


Bit 110


Bit 210


0ngn Figure 15. 1319nm LLSI image overlaid on LSM reflected light image for two different logic states of the three bit cells (rectangular  boxes) shown in Fig. 14.


Abnormal LLSI


Bit 110 Bit 210


ZZ0E6Z


Figure 16. 1064nm LLSI of the same region as Fig. 15, demonstrating the ability to capture the correct logic state using the shorter  laser wavelength. Differences in the details between 1064nm and 1319nm exist, including the capture of an anomalous LLSI signal  with 1064nm, but not with 1319nm.


show dynamic timing and logic state information, without  changing the DUT and test setups. With the LLSI technology, the failure analysis and design debug engineers effectively has  both the traditional IREM-LSI technology and the added CWSIP technology in one setup. This gives the engineer new  capabilities and flexibilities to solve the increasingly difficult  and challenging failures and faults seen in modern CMOS-IC.


Logic State Imaging is a powerful tool and technology in  CMOS IC process development and circuit design debug. With the increasingly challenging environment of smaller  circuit feature sizes, lower Vcc operation for low power  devices and ultra low leakage transistor technology, the  traditional IREM based LSI is facing nearly insurmountable  hurdles on two fronts: feature size resolution and SNR. LLSI  technology overcomes those two hurdles. It has enabled Intel  to continue using the LSI technology for our 22nm and 14nm  process development and product debug successfully. To the  authors’ knowledge, this is the first time we were able to take  advantages of some of the latest DFT and DFD feature in  modern MPU and SOC products to enable LLSI. We  successfully expanded CW-SIP technology to include LSI  capabilities, and thereby extended LSI to the 22nm and 14nm  technology nodes. With LLSI, we can, in fact, not only get  static logic states information –like traditional IREM LSI, except with much improved spatial resolution and better SNR, but also dynamic circuit logic states information. We expect  LLSI to continue to scale and be able to support the next  generations of process node development and product debug  in the foreseeable future.


We would like to acknowledge many engineers in Intel’s  process development and product design and validation labs  for their support and contributions to enable LLSI at Intel. Specifically, LTD design group’s Fabrice Paillet, Loc Mai and  Gerhard Schrom for their help with the FIVR DFT features. PTD LYA lab’s Aamir Zia and Rajesh Duggirala for their  support with both tool time and available resources for many  of the experiments carried out in their Lab. TMG lab’s  Zhiyong Ma, Travis Eiles, Rajiv Giridharagopal, Mitch Sacks, Tony Peterson for many helpful discussions. TMG Lab’s  FATD team at Intel Penang, especially Choon Yan Teh, Him  Eng Yeoh and Seong Leong Lim for their support on the  system board design-manufacturing and debug to enable  LLSI. PEG/MDO JF debug lab’s Pat Pardy and his team for  their support on data collected in the JF-Debug lab. Shane  Pollard of Intel Fab32 LYA group is acknowledged for his  contribution to the LLSI working group at Intel. The authors  greatly appreciate inputs and edits the reviewer and mentor


provided to the manuscript. The inputs and edits from the  reviewer/mentor greatly improved the manuscript’s clarity and  readabilities.


[1] Y-C Steven Chen, et al. “Backside Infrared Emission  Microscopy (IREM) Based Silicon Debug  Methodology”, Intel Design and Test Technology  Conference, 2000.


[2] D.R. Bockelman, “Infrared Emission-Based Static Logic  State Imaging on Advanced Silicon Technologies”, ISTFA, 2002


[3] Dan Bockelman, et al. “Multi-Point Probing on 65nm  Silicon Technology Using Static IREM-Based  Methodology”, International Symposium for Test and  Failure Analysis, 2005.


[4] Stas Polonsky, et al. “Off-state luminescence in metaloxide-semiconductor field-effect transistors and its use  as on-chip voltage probe”, APL 85, 2390(2004)


[5] Baohua Niu, et al. “Continuous Wave 1319nm Signal  Imaging and Probing”, Intel Design and Test  Technology Conference, 2012


[6] Ying S Ng, et al “Laser Voltage Imaging: A new  Perspective of Laser Voltage Probing”, ISTFA 2010.


[7] Joy Y Liao, et al, “Scan Chain Failure analysis using  laser voltage imaging”, Microelectronics Reliability, Vol. 50, pp 1422-1426, 2010


[8] R. Nicholson, et al, “Laser Voltage Imaging: Setting a  New Baseline for Circuit Analysis”, EDFAS Vol 13, Issue 3, 2011.


[9] G. Celi et al, “Thermal Frequency Imaging: A new  application of Laser Voltage Imaging applied on 40nm  technology”, ISTFA, 2011.


[10] A. Muhtaroglu et al, “On-Die Droop Detector for Analog  Sensing of Power Supply Noise”, IEEE J. Solid-State  Circuits, Vol.39, No.4, April, 2004.


[11] R. Petersen, et al, “Real Time Voltage Measurement and  Droop Induction for Debug on Tukwila”, Intel Design  and Test Technology Conference, 2008.


1064nm  Laser Irradiance (mW/µm


Enable-d


0道


10**x15202530*2)


Figure 3.  With a 28nm nMOS transistor in its off state, (VGS=0V), we measured the 1340nm OBIC at both


0Q


VDS=1.015V and VDS=0.894V in the typical LADA laser


IA


irradiance range.  The induced current is linear with laser  irradiance.


SDFFRFO


寿


4. Characterization of LADA Failure Rate


Figure 4 shows a typical LADA analysis using both 1064nm  and 1340nm lasers.  Both lasers identify the same devices with  the 1340nm laser producing a more localized spot.  The better  localization with the 1340nm laser occurs primarily because  there is no nWell interaction.  In order to determine the  relationship between laser power and LADA effect a selected  LADA site was illuminated in spot mode and the change in  failure rate was measured at several different laser powers for   both the 1340nm and 1064nm lasers.  Figure 5 shows that both  lasers cause a change in failure rate that is linear with respect  to laser power.  Again, the data indicates that there is a linear  mechanism occurring that produces laser induced current and  LADA effects when using the CW 1340nm laser, not the  quadratic relationship of 2pLADA


1340nm


Figure 4. Colorized LADA images superimposed on reflected  image showing several LADA passing sites detected at  1064nm and 1340nm lasers.  The site on the right was  analyzed in spot mode to produce the failure rate curves  shown in Figure 5.


70


1.2E-03


--1064nm


O0.7V=VDS


Failure Rate Delta (in %)10


---Laser ON


2.0E-04


0 2台古 50


-1340nm


60


Drain Current (in A)


-Laser OFF


00


O0.1V=VDS


004


8.0E-04


()0.3V=Vos


1.0E-03


0.5V=VDS


0.9V=VDS


0123456789


0.0E+00


0.0V=VDS


Laser Irradiance (in mW/μm^2)


Gate Voltage (in Volts)


0.10.20.30.40.50.60.70.80.9


Figure 5. The site on the right in Figure 4 was illuminated in  spot mode and the induced failure rate change versus laser  irradiance is nearly identical linear relationship for 1340nm  and 1064nm lasers.  Note: “Failure Rate Delta” was  calculated as “Fail% with laser off” minus “Fail% with laser  on”.


5. 1340nm Laser-Induced Current vs. VGS and VDS


An on chip 28nm metal gate high-K dielectric nMOS test


transistor was characterized through the back side using a laser


scanning microscope lens with a 0.4 NA (spot size of


~1.5um).  The spot size is approximately the size of the entire


nMOS device that is shown in Figure 6.  Also shown in Figure


6 are the ID vs VGS curves taken from that device.


To better understand the 1340nm laser interaction with a


transistor during normal operation, consider the circuit


implementation of an nMOS device in a CMOS inverter. The


output node of the inverter is discharged by having its input


gate signal ramped from 0V to VDD. During this transitional 4 period, due to the receiver’s capacitance, for a short time VDS


is nearly constant at ~VDD.  In order to accurately describe


laser effects at various times throughout the ramp behavior,


investigative VGS and VDS bias points for the nMOS transistor


were defined and are shown as red circles in Figure 6.


As the output node is discharged the VDS falls from VDD to 0V.


in Current (in μA)Difference in Dra山Laser ON - Laser OFF。PNw


These additional bias points are shown as green circles within  the same figure. All of the bias points described in Figure 6  can be used as reference throughout this paper. A blue arrow  seen in Figure 6 shows the progression of bias points from left  to right as the output node is discharged through the nMOS


-2


0.00.10.20.30.40.50.6 0.7 0.80.9


device


Figure 6.  VGS sweep of a 28nm-node nMOS with investigative  bias points during CMOS inverter operation.  The layout  shows the transistor with a drawn gate length of 30nm and a  width of 1.3um.  The source (left) and drain nodes (right) are  both approximately 0.45um x 1.3um.


Note that Figure 6 shows curves for laser ON and OFF, and  that the difference between the two cases is a small percentage  of the overall current (and at this scale the two curves appear  superimposed).  What is important for understanding LADA is  to characterize the induced current from the laser.  Figure 7  shows the induced current from the laser by plotting the  difference of the two data sets (ON vs OFF) of Figure 6.  This  data shows that through most bias points of the VGS sweep the  net effect of the laser is an increase the drain current.


The 1340nm laser effect was characterized at different power  levels.  The data of Figure 8 shows that the amount of laser  induced current is linear with respect to laser power.  Again, as in the case of the laser-induced off current, the linearity is  inconsistent with 2pLADA.


Figure 7.  Difference in current measured as I-drain (laser on) minus I-drain (laser off).  This plot has five curves with VDS  biases of 0.1, 0.3, 0.5, 0.7, and 0.9 volts.  The blue line traces  the bias points of the nMOS in an inverter, as shown in Figure


6.


Measured at Vgs=400mV; Vds=100mV


VG=0.25Vand VD=0.9V


2.0


RR R只


1.0


. . 0


0.0 △ Laser0nm134 (in μA) induced Current0


1015


20


SourceDrain


Laser Power mW


8。


。


R。


Figure 8.  Laser induced current versus laser power shows a  linear relationship.


6. High Spatial Resolution 1320nm Laser Effects


Source Edge


To obtain a more complete understanding of CW ~1300nm


VG=0.9V and VD=0.7V


LADA, the isolated nMOS transistor shown in the inset of  Figure 6 was analyzed at several different gate and drain bias  conditions.  A laser induced current image was generated  using a current amplifier to produce a video input voltage  level proportional to the laser induced current. This data was  acquired with a 2.45NA SIL and a 1320nm CW laser  irradiation.


Figure 9 shows two examples of the acquired laser induced  drain current images, and the CAD overlay that was  performed to identify the source and drain region.  The full  data set is shown in Figure 10.  The images in Figure 10 show  the spatial dependence of laser induced current at the typical  CMOS bias points shown in Figure 6.  A bright site in the  images of Figure 10 indicates a positive laser induced drain  current, and a dark site indicates a negative laser induced drain  current.


The images in Figure 10 show that at low VGS values (less  than 0.7V) there is a large positive induced current detected at


A9=06A


the transistor.  At VGS greater than 0.7V the source node


VD


remains bright while the drain switches to a negative induced


0'6A0.8V0.7V0.6V0.5V


current.


Figure 9 (Top Image) Composite image with the CAD active, gate, contact layers and laser induced drain current image at  VGS=0.25V and VDS=0.9V. (Bottom Image) A second bias  condition of VGS=0.9V and VDS=0.7V showing drain signature  of lower current.  The source (yellow) and drain (pink) regions were determined from this overlay as well as the  source edge (blue).  These regions were then used in Figure  10 to extract current from the source, drain, and source edge  regions.


||VD=0.9V|VD=0.9V|VD=0.9V|VD=0.9V|
|---|---|---|---|---|

|||VG|||

|0.0V|0.25V|0.5V|0.7V|0.8V|

Figure 10.  1320nm laser induced drain current images for the  nMOS device of Figure 6, acquired with a 2.45NA SIL.  The  top row of images is taken at a VDS=0.9V and VGS of 0, 0.25,


0.5, 0.7 and 0.8 volts.  The bottom row of images is acquired  at a VGS=0.9V and VDS of 0.9, 0.8, 0.7, 0.6, and 0.5 volts. These images have different contrast settings to enhance the  image.


In order to quantify the induced current effects based on laser  position within a device of interest, current values were  extracted from the raw gray scale levels in the images of  Figure 10 and plotted versus various bias conditions.  The


locations analyzed are shown in Figure 9 as: source


2.E-05


9


Global Thermal Heating Effect


illumination (yellow rectangle), drain illumination (pink  rectangle), and because we observed a high sensitivity site  near the edge of the transistor, we labeled that region as source


1.E-05


edge illumination (blue circle).  Note that this is the same test  device as discussed in Figure 6. Figure 11 shows the laser  induced current at several bias conditions for the three spatial


0E+00


regions.   The data in Figure 11 shows that the source and  source edge locations have a net positive current for all bias  conditions.  The data also shows that the drain node has


1E05


positive current as the gate voltage is swept but then has  negative current when VGS reaches 0.9 volts


n Amp in Drain(is)  CurrentChange


-2.E-05


0.00.10.20.30.40.50.60.70.80.9


Figure 11.  Laser induced current values obtained at the


three regions shown in Figure 10 at the following bias points: (VGS=0, 0.25, 0.5, 0.6, 0.7, 0.8, 0.9 volts with VDS held


n μA) inChange(i  Current DrainN


constant at 0.9V) are shown as red filled data markers and


(VDS=0.5, 0.6, 0.7, and 0.8 with VGS held constant at 0.9V) are 0 shown as green filled data markers. All bias points result in


Temperature (in degrees C)


positive current for source illumination while the drain  illumination has both positive and negative induced current  depending on bias conditions.


7. Global Heating Effects


4.E-06


Next we compare the laser effects on measured transistor


d3.E-06 S


ω


curves to that of global heating of the transistor in Figure 6.  V


Figure 12 shows the heat induced current of a 17 C


u2.E-06


temperature increase caused by forced air heating of the


u


81.E-06


sample. Several temperatures were characterized and the


increase in current versus temperature was found to be linear, 00.E+00


as shown in Figure 13.


e-1.E-06a-Measured Laser Induced Drain Current Delta----Spice Simulation of Thermal Effectu In Figure 14, we show that the laser effects shown in Figure 7


-2.E-06-Global Thermal Heating Effect


can be approximated by a 4C increase in temperature.


3 e-3.E-06 However, there are differences between global heating and 0U


laser interaction.  Most significantly, the laser induced current


-4.E-06


switches negative at a higher VGS than the thermal current.


Secondly, there is significant OFF current generated by the


laser (VGS=0) which is not seen from the bulk thermal  stimulation.


VDs=900mV


Figure 12.  Temperature induced current difference at VDS


biases of 0.1, 0.3, 0.5, 0.7, and 0.9 volts. The current


台


500mV VDS


difference is calculated by subtracted 48C measurements from


600mV


65C measurements.


700mV 800mV 900mV


无


DBmV


良


2020V


(in Current InducedLaser μA)-1.0


→-Source Drain Source-Edge


co


00.1 0.2 0.3 0.4 0.5 0.6 0.7 0.8 0.9 Gate Voltage (in Volts)


an


Figure 13.  Plot showing that drain current (measured at  maximum increase on the VDS=0.1V curve) increases linearly  with temperature at about 300nA per degree C.


Figure 14.  Comparison of laser and thermal induced current  measurements at various drain voltages (0.1V-0.9V).  The  data in Figure 14 was scaled to a 4C difference to overlay  these curves. Also shown here are the predicted effects of the  spice transistor model for the same 4C temperature difference.


8. Response Time of LADA Failure Rate


In order to obtain an estimate of time of the interaction we  used a pulsed 1340nm laser with a 120ns rise time to  characterize the response time of a LADA interaction.  Figure  15 shows the failure rate versus time for a pulsed laser  interaction.  Since the critical signal with which the laser  interacts with is ~100ps, the resulting failure rate graph is  simply a measure of the much longer laser pulse itself [6].  A  photodiode with <175ps rise and fall time was also used to  characterize the laser directly and the two plots are overlaid  for comparison.  The conclusion of this figure is that the  response time of the 1340nm LADA signal is << 100ns.


Figure 15.  Pulsed 1340nm laser induced failure rate response  versus time during spot mode illumination of a LADA site with  an interaction window of ~100ps.  The resulting plot is  equivalent to the laser pulse itself (shown in black) indicating  that the LADA response time is much faster than the laser  pulse used for this experiment.


9. Discussion


Linear Response to Laser Power


The data presented in Figures 3, 5 and 8 all show a linear  relationship of the induced current and the LADA fail rate to  laser power.  Figures 13 and 14 demonstrate that the laser  induced current is linear and is likely due to the heating of the  device, as discussed in [5]. The change in drain current  approximates both the measured and simulated effects of  globally heating the device 4 degrees C. Two competing  effects drive the induced current change: mobility reduction  and Vt lowering (about 1mV/deg C [7]), each of which  dominate at different bias conditions.


Free Carrier Absorption


At the dimensions of a 28nm-node transistor, there are two  local materials that can convert the IR irradiation to heat via  free carrier absorption (FCA) -- the heavily doped source and  drain regions [5, 8] and the silicide on those regions.   The ，absorption coefficient for ~1300nm FCA in the heavily doped  source and drain regions is about 70 cm-1 [8], similar to the  1064nm electron-hole pair absorption coefficient of 100cm-1


[8] that is used for conventional LADA.


The Role of FCA in the Transistor Off Current


The positive current seen in Figure 3, and Figures 7 and 10  when VDS=0.9V and VGS=0V, is neither explained in [5] nor  by global thermal heating in Figure 14.  We propose that this  difference is due to free carrier absorption in the highly doped  source region of the transistor, giving the carriers enough  energy to surmount the source-channel barrier and be  collected in the drain.


The free carrier absorption effect was utilized in [9] and [10] where it is shown that an efficient IR detector can be built in  silicon using a three-layer structure designed with the  asymmetrical band diagram shown in Figure 16. In such a  structure, an IR photon interacts with a free carrier, giving it  enough energy to surmount the barrier and get collected at the  other node.  Free carrier absorption creates a current through


the structure.


Short channel MOSFETs exhibit drain induced barrier


-Photodiode Detection


lowering (DIBL) with high VDS and VGS=0.  The DIBL band


of Laser Pulse


员


Failure Rate Detection


structure [11] is very similar to the band structure of the IR


detectors, where the IR-sensitive region A is the transistor


and


source, the barrier B is at the gate/source end of the channel  and the collection region C is the drain.  The high doping in


the transistor source allows it to be a significant source of free


ized Failure RateNormal


carriers [8].  In other words, an off-state transistor in modern  CMOS circuits is biased similar to an IR detector and can


PulsePhotodiode detection of Laser


produce leakage current in the presence of infrared


-0.2


illumination at the source terminal.


500


1,000


Time (in ns)


FCA in the highly doped source region is a plausible  explanation as to the interaction responsible for the laserinduced off current we observed, by giving source electrons  energy to overcome the energy barrier between the source and  the channel.  The additional energy in these hot carriers  effectively increases transistor off current.


Figure 16.  In [13] and [14], silicon-based IR detectors with this  band diagram are described.  An IR photon interacts with a free  carrier in region A of the device, giving it enough energy to surmount  the barrier in region B and move into region C


The Source Signature Associated with FCA


Differentiating the response of the source and drain on 28nmnode transistors is difficult, since even a high numerical  aperture SIL lens has a spot size (~260nm) much greater than  the gate length (~30nm).  The relatively large source and drain


CB


VB


eIR Photon 4


nodes of the test transistor did allow a distinction at some bias  conditions as can be seen in Figure 10.


Figure 11 illustrates that the largest induced current occurs  when illuminating the transistor source region.  Illuminating  the drain causes the lowest induced current and a reduced  current for higher VGS bias conditions.


We propose four explanations for the difference between the  drain and source (i.e. the source signature):


1. The “IR detector” effect described in the previous section can happen only at the transistor source.


2. An increased temperature of the source node will lower the Vt by about 1mV/deg C [7].


3. An increased temperature of the drain node due to FCA will lower the saturation velocity of the carriers at the drain-channel region and will reduce the current [7].


4. A Seebeck effect may exist between the source/drain regions of the transistor due to increased diffusion currents caused by non-uniform heating of carriers[5, 12].


Response Time Measurements Support FCA


Based upon [13] the response time of free carriers in silicon is  less than a picosecond and the time for the hot carrier to  transfer its heat to the surrounding lattice is on the order of  picoseconds.


The local silicide (within ~100nm) heating due to free carrier  absorption is also very fast, with literature sources providing a  range of estimates.  Based on [14, 15] the Seebeck effect  response times for FCA heating in this scale of structure are  likely on the order of nanoseconds.  Given the dimensions of  28nm node transistors and by using the modeling results of


[16], thermal heating of the local silicide (and contact) may  conduct heat to the transistor within tens of picoseconds.


The conclusion based on Figure 15 is that the response time of  the FC-LADA signal is << 100ns which is consistent with a  free carrier absorption mechanisms close to the transistor.  It  implies that heating of the interconnect metallization, which is  significantly farther away, does not significantly contribute to  induced currents in the transistor.  The images in Figure 10, and the LADA images in the next section also show no  evidence of interactions with the metal interconnect.


Free Carrier LADA


Given the detailed analysis in [5] and the analysis in this paper  on 28nm-node devices, we believe that the LADA effect  observed with CW ~1300nm irradiation is primarily due to  free carrier absorption in the transistor source and drains.  We  have termed this technique Free Carrier LADA (FC-LADA). In the next section, we will discuss FC-LADA images within  the context of the data presented.


10. FC-LADA Image Analysis


As we begin to review LADA sites there should be two main  differences between FC-LADA and traditional LADA.


1. FC-LADA should have no nWell or pWell interaction because the band structure shown in Figure 16 that is


needed for significant current generation is not present  in a reverse biased well junction.  The lack of well  response is shown in Figure 4.


2. The source signature discussed in section 9 should be observable: the origin of the FC-LADA interaction should be stronger at the source node and weaker at the drain node.


Observing the stronger source node interaction is not  straightforward as discussed in Section 9.     In looking at  many FC-LADA sites, however, we observed that gates with  devices in series such as NOR gates do in fact show a source  signature consistent with FC-LADA.


Figure 17 is a grayscale FC-LADA image where lower failure  rates are shown as darker pixels and higher failure rates are  shown as brighter pixels.  The FC-LADA image of Figure 17  shows a two-input NOR gate and its LADA signature.  In this  case the gate is transitioning from LOW to HIGH and its  output from HIGH to LOW.  The FC-LADA site shows a  failing signal at the series pMOS device due to the higher  current from the pMOS slowing down the output.  However it  can be seen that the drain of the pMOS is actually helping the  transition by inducing less current.  This is the same effect  observed in the laser induced current of the transistor in Figure


10.


Figure 17.  (Left Image) SIL based LADA grayscale image at  NOR gate of the LADA site of Figure 4.  (Right Image) The  active, gate, and output node (yellow) are shown.


Figure 18(a) shows an FC-LADA site obtained at the 8-fingered PMOS transistor pair of a two-input NOR gate in a  speed-limiting path.  The laser interacts at the transistor source  regions rather than the drain regions to speed up a rising edge  on the NOR output. If the effect were due to electron-hole pair  interaction, the brightest LADA contrast would be evident at  the drain region [1].


Free Carrier Effects with 1064nm LADA


Figure 18(b) shows a 1064nm LADA signature at the same  NOR gate under identical conditions.  Surprisingly, this data  indicates that the 1064nm LADA has a source signature  consistent with FC-LADA, and not a drain signature that  would indicate electron-hole pair interaction.  Note that FCA  is also present with 1064nm irradiation.  The absorption  coefficient scales with the square of wavelength, so FCA at  1064nm is about 63% of that at ~1300nm.


Based on this data it appears that free carrier absorption  effects are the dominant mechanism in this 1064nm LADA  image. Initial follow-up investigations indicate that a ~50ps  pulsed 1064nm laser as used in [17] produces source  signatures nearly identical to that of Figure 18(b) indicating


that the FC-LADA mechanism likely has a response time on  the order of ~100ps or less.


Figure 18.  (a) This FC-LADA image of an 8-fingered PMOS  transistor pair in a NOR gate illustrates that the laser interacts with  the transistor source regions (marked S) rather than the drain  regions (marked D).  Gates are outlined in green and the solid cyan  is the metal-1 drain connection.  This image was obtained with a


2.45NA SIL and a 1320nm CW laser. (b) A 1064nm LADA image of  the same 8-fingered PMOS transistor pair indicating a source  signature similar to that of the 1320nm laser.


FC-LADA at Other Circuit Structures


Although not shown here, focusing the 1320nm laser into the  nWell junction showed no nWell interaction, further  indicating that the mechanism is not related to electron-hole  pair creation.  However, FC-LADA does have a signature at  the n+ well tie as shown in Figure 19.  This figure shows a  passing site induced at the n+ well tie near the NOR gate of  Figure 18.  This passing site is believed to be due to the  Seebeck effect at the well tie structure resulting in a lowering  of the local nWELL voltage which will lower the VT of the  PMOS NOR gate transistor and results in a passing LADA  site.


Figure 19.  A 1320nm FC-LADA image of the NOR gate of  Fig. 18.  This image was acquired at slightly different  background failure rate and laser conditions to produce a  larger passing signature.  Note that the n+ well tie is detected (left dark site) but not the entire nWell signature.  This is  believed to be the Seebeck effect occurring due to free carrier  absorption at the n+ well tie.


Summary and Conclusions


The results presented in this paper show that the mechanism


(a)1340nm


responsible for CW ~1300nm LADA is linear and is not  consistent with 2-photon absorption, although we did observe  2-photon absorption in a diode structure.


We attribute the CW ~1300nm LADA effect to free carrier  absorption in the heavily doped regions of the transistor, as


SDSDSDSDS


well as absorption in the silicided regions.  The free carriers  both heat the transistor, and as hot carriers themselves can act  as a source of current.  We call this technique free-carrier  LADA (FC-LADA) to distinguish it from SDL, normally used  for locating defects in metal interconnect.


We presented evidence that even 1064nm LADA on 28nmnode transistors is related more to free carrier absorption in the  transistor than to electron-hole pair creation at the junctions.


FC-LADA is a complementary tool to traditional LADA and


(b) 1064nm


has several advantages. The absence of large nWELL  interactions help to improve spatial resolution and eliminate  possible cases of latch up during analysis.  Spatial resolution  will be on the order of the optical spot size of the laser since  minority carrier diffusion lengths do not limit resolution.


Future Work


In this work we tackled a difficult topic using only production  IC material.  We used on chip test structures and a number of  functional root cause analysis jobs to extract a reasonable  understanding of the ~1300nm FC-LADA interaction.  Future  work could be aimed at using faster ~1300nm pulsed lasers to  determine more precise response times.  We were surprised by  the 1064nm FC-LADA result and the fast (~100ps) response  time and are planning further experimentation into that area. We encourage others to identify better test structures and test  cases to continue to refine the understanding of the FC-LADA  effect.


1.


Rowlette, Jeremy A., and Travis M. Eiles. "Critical timing analysis in microprocessors using near-IR laser


n+ nWell Tie


assisted device alteration (LADA)." In 2013 IEEE International Test Conference (ITC), pp. 264-264.


IEEE Computer Society, 2003.


2.


Bruce, Michael, Victoria Bruce, David Eppes, Jacob


NOR GATE pMOS


Wilcox, Ed Cole, Paiboon Tangyunyong, and Charles Hawkins “Soft Defect Localization (SDL) on ICs”,


Proceedings of the 28th International Symposium for Testing and Failure Analysis, pp. 21-27, ASM International, 2002


3.


Niu, Baohua, Pat Pardy, Joe Davis, Mel Ortega, and Travis Eiles. "Two-Photon Absorption Laser Assisted Device Alteration Using 1340nm CW Laser: Critical Timing Fault Isolation & Localization for 32nm MPU and Beyond." In Proceedings from the 36th International Symposium for Testing and Failure Analysis, p. 224. ASM International, 2010.


4.


Niu, Baohua, Patrick Pardy, Jerry Fortier, Mel Ortega,and Travis Eiles. "Two-photon absorption laser


assisted device alteration using continuous wave 1,340  nm laser." Journal of Materials Science: Materials in  Electronics 22, no. 10 (2011): 1542-1552.


5.


Glowacki, Arkadiusz M., Sanjib Kumar Brahma,Hiroyoshi Suzuki, and Christian Boit. "Systematic characterization of integrated circuit standard components as stimulated by scanning laser beam."


Device and Materials Reliability, IEEE Transactions on 7, no. 1 (2007): 31-49.


Bodoh, Dan, and Kent Erington. "Improving the DLS Workflow." In Proceedings from the 38th International Symposium for Testing and Failure Analysis p. 183. ASM International, 2012.


7.


Wolpert, David and Paul Ampadu, “Temperature Effects in Semiconductors” in Managing Temperature Effects in Nanoscale Adaptive Systems (2012)


8.


Falk, R. Aaron. "Near IR absorption in heavily doped silicon-an empirical approach." In Proceedings from the 26th International Symposium for Testing and Failure Analysis, pp. 121-128. ASM International;


2000.


9.


Tohyama, Shigeru, Nobukazu Teranishi, Kazuo Konuma, Miyo Nishimura, Kouichi Arai, and Eiji Oda. "A new concept silicon homojunction infrared sensor." IEEE Transactions on Electron Devices 38,no. 5 (1991): 1136-1140


10. Ariyawansa, G., M. B. M. Rinzan, S. G. Matsik, G.


Hastings, A. G. U. Perera, H. C. Liu, Margaret Buchanan, G. I. Sproule, V. I. Gavrilenko, and V. P.


Kuznetsov. "Characteristics of a Si dual-band detector responding in both near-and very-long-wavelengthinfrared regions." Applied Physics Letters 89, no. 6(2006): 061112.


11. Mutlu, Ayhan A., and Mahmud Rahman. "Twodimensional analytical model for drain induced barrier lowering (DIBL) in short channel MOSFETs." In Southeastcon 2000. Proceedings of the IEEE, pp. 340-344. IEEE, 2000.


12. Wolfe, Charles, Nick Holonyak, Jr., Gregory Stillman.


Physical Properties of Semiconductors (1989)


13. Downer, M. C., and C. V. Shank. "Ultrafast heating of silicon on sapphire by femtosecond optical pulses."Physical review letters 56, no. 7 (1986): 761.


14. Xiaofang, Zhou, Jiang Zuimin, Lin Jianhui, Tang Xiaodong, Chen Qingming, Zhang Hui, and Zhang Pengxiang. "Thermoelectric signals from Si/SiGe superlattices." Journal of Physics D: Applied Physics 42, no. 22 (2009): 225303


15. Renk, Karl Friedrich, J. Betz, S. Zeuner, Hans Lengfellner, and Wilhelm Prettl. "Thermopile effect due to laser radiation heating in thin films of high-Tc materials." Physica C: Superconductivity 235 (1994):37-40.


16. Wang, Xinwei, and Xianfan Xu. "Thermoelastic wave in metal induced by ultrafast laser pulses." Journal of thermal stresses 25, no. 5 (2002): 457-473.


17. Erington, K., D. Bodoh, K. A. Serrels, C. Nemirow, N.


Leslie, T. R. Lundquist, P. Vedagarbha, C. Farrell, and D. T. Reid. "Measuring propagation delays of critical paths using time-resolved LADA." In Reliability Physics Symposium, 2014 IEEE International, pp. 3F4. IEEE, 2014.


Root Cause Analysis Techniques Using Picosecond Time Resolved LADA


Dan Bodoh, Kent Erington, Kris Dickson, George Lange, Carey Wu


Freescale Semiconductor, Inc, 6501 West William Cannon Drive, Austin, Texas 78735, USA  Tom Crawford


DCG Systems, Inc, 3400 W Warren Ave, Fremont, CA 94538, USA


Laser-assisted device alteration (LADA) is an established  technique used to identify critical speed paths in integrated  circuits [1].  With this technique, the critical path is identified  and interaction sites are mapped to specific transistors; then a  schematic analysis is performed to reveal speed path details.


LADA can reveal the physical     location of a speed path, but  not the timing of the speed path. Several researchers have


Vsource


Vb


reported on time resolved LADA (TR-LADA).  The concept


n-well tie 2


PMOS


n-well tie1


was introduced in [2] using an electro-optic modulator with ~15ns rise time to modulate a 1064nm continuous wave (CW)


TR3R1VBLocal2 n+


回可


n+


laser.  In [3], we describe a methodology to achieve  microsecond resolution without the need for laser modulation. As a follow-up in [4], we demonstrate TR-LADA by


Cawell


N well


manipulating the TTL control input on a 1064nm diode  pumped solid state laser to achieve 100ns resolution, and we  detail the software to acquire single-site TR-LADA


P substrate


waveforms.  In [5], Serrels, et al. describe time resolution of <10ps with the mode-locked 1280nm femtosecond laser


Laser beam


necessary for two-photon LADA.


In this paper, we will describe the root cause analysis benefits  of 1064nm TR-LADA with a picosecond laser.   Introduced in


[6], we will show several examples of how picosecond TRLADA has complemented the existing fault isolation toolset  and has allowed us quicker resolution of design and  manufacturing issues.


The TR-LADA System


The TR-LADA system consists of a 1064nm fiber amplified  pulsed diode laser, capable of a 50ps pulse width.  The laser is  connected to a laser scanning microscope containing air gap  lenses.   Similar to our previous work described in [4], the  system integrates with a tester using custom hardware and  software.  TR-LADA waveforms can be acquired at one site, or the entire field of view can be scanned while laser pulses  are synchronized to the test loop.  The synchronization of the  laser pulse to the tester was straightforward because the laser  can be triggered at any frequency from 50Hz to 80MHz, allowing for a single pulse per test loop for typical loop


LADA


periods.   The system also contains 1064nm and 1340nm CW  diode pumped solid state lasers.


TR-LADA


The Analysis Benefits of this System


Increasing the localization resolution by reducing the well  interaction. LADA sites at PMOS transistors, especially with  lower-NA lenses, are dominated by the laser interaction with  the n-well.  As described in [1] and shown in Figure 1, CW  illumination creates a photocurrent at the n-well/p-substrate  junction which is divided between the nearest n-well ties.  The  resistance of the n-well, R1 and R2, creates a voltage divider  that reduces the local n-well voltage, VbLocal, of any transistors  between the n-well and the illumination site.  The reduced nwell voltage effectively decreases the Vt of the transistor  allowing it to speed up. Large cigar-shaped LADA sites along  the well are the result, reducing the localization resolution.  The n-well interaction depends on the relative values of R1, R2  and R3, and therefore on the physical relationship between the  n-well ties and the transistor in the critical path.


Figure 1.  Simplified schematic of the n-well photocurrent injection.


With a 50ps laser pulse, however, the well capacitance, Cwell, becomes important – the decrease in VbLocal lags the  photocurrent injection due to the RC delay of the well.  A laser  pulse timed to occur just before the critical event arrives at the  transistor will cause the VbLocal perturbation to occur after the  event, eliminating the n-well interaction.


Figure 2 illustrates the cigar-shaped LADA sites from CW  illumination with an air gap lens.  Each of the dark LADA  sites encompass most of the n-well containing a transistor in  the critical signal path.  The TR-LADA image in Figure 2  shows the same three sites, with the laser pulse synchronized  to arrive just before the signal arrives at the left site.  The nwell response is eliminated at the left site, and reduced at the  two other downstream sites.     The localization resolution of  the left TR-LADA site is limited only by the optical resolution  of the system.


Figure 2.   LADA and TR-LADA images of a critical signal propagating  through three gates from left to right on a 28nm-node device, using a 0.9NA air gap lens.    In the TR-LADA image, the laser pulse  is synchronized to arrive at the left site just before the signal  arrives, eliminating the n-well response.  In the images in this  paper, dark sites indicate a low fail rate.


The smaller spot size possible when using a SIL increases the  contrast between the transistor response and the n-well


response in some cases.  However, if the n-well ties are far  away from the transistor of interest, the n-well interaction  creates the same haze along the n-well, as shown in Figure 3.  SIL-based TR-LADA improves the localization resolution and  reveals complementary signals from the two inverters in the  clock buffer.


201e 4 1


Figure 3.  LADA and TR-LADA images of a critical signal in a clock


Figure 3. LADA and TR-LADA images of a critical signal in a clock 704 He


buffer on a 28-nm node device, using a 2.45NA SIL on a commercial  optical fault isolation tool.  In the TR-LADA image, the laser pulse is  synchronized to arrive just before the rising edge of the clock signal


synchronized to arrive just before the rising edge of the clock signal


at the input of the clock buffer.  The OD (active) layer from CAD is  shown for reference.


shown for reference.


LADA Image


Typically, the n-well responds a few nanoseconds before the  critical event, as shown in Figure 4.  The n-well interaction


critical event, as shown in Figure 4. The n-well interaction


builds to a maximum at about 2ns prior to the event.   The


The


most localized site is achieved by synchronizing the laser at


the time of the trailing edge of the TR-LADA waveform,


the time of the trailing edge of the TR-LADA waveform, where the pulse is close to the actual critical event.


Figure 4. TR-LADA waveform of a typical 28nm-node passing site, with the 50ps laser pulse and a 0.9NA lens.  The n-well interaction  reaches its maximum about 2ns before the event at time A.    The  most localized site is achieved by synchronizing the laser pulse at  time B, the rising edge of the TR-LADA waveform.  As described in


[4], a TR-LADA waveform is taken by spot-illuminating a LADA site, and has average fail rate on the y-axis and time relative to the  beginning of the test loop on the x-axis.


Resolving the time of the LADA-sensitive event.   LADA  locates sensitive circuits on the die but does not offer any  information on the timing of the sensitive event in the circuit. Often, further analysis, such as laser voltage probing (LVP) or logic simulation, is required to understand the nature of the  critical path.   The lack of timing information is especially  problematic for laser voltage probing long functional patterns. Finding the timing of a LADA event with LVP alone is an  intractable needle-in-the-haystack problem in most situations.


Figure 5 shows the workflow of an analysis of a shmoo stripe  issue.  LADA analysis revealed sites leading to a clock mux. Waveforms were necessary to understand the nature of the  failure, because the issue did not appear to be a typical setup  or hold time issue at a flip flop.  A picosecond TR-LADA  waveform was acquired at one of the passing LADA sites. The waveform showed that the critical event occurred at


6.328837ms after the beginning of the 7.38ms test loop.  This


timing was used to set the delay for LVP analysis, which  showed a 150ps glitch in the clock signal at the output of the  mux.


Without TR-LADA, finding a 150ps glitch in a 7.38ms pattern  would have been impossible.  The LVP system is limited to  1000 points in the waveform, which is a 2.4ns window at the  timing resolution shown in Figure 5.  Searching from the end


of the pattern with 2.4ns windows would require 437,985  waveforms.  With TR-LADA, we enabled the use of LVP  where it would have been difficult, leading to a faster  resolution to the problem.


Figure 5.  Illustration of the workflow that TR-LADA enables to get  waveforms of a timing issue.    The sites were localized with LADA.  Picosecond TR-LADA was performed at one of the passing sites to  temporally localize the fault, which is indicated by the trailing, rising edge of in the TR-LADA waveform.  The timing was used to  set the delay for LVP analysis, which revealed  a 150ps glitch in the


clock signal.Horiz: 500ps/divVert:


clock signal.


Visualizing the direction of signal propagation in the  critical path.  The ability to take many TR-LADA images  with the laser pulse synchronized at different times in the test  allows the analyst to make a “movie” of the signal propagation  along the critical path.  As shown in Figure 6, the signal  propagation is evident by when the site disappears.


Physically viewing the path of signal propagation has two  advantages.   First, the end of the critical path is known prior  to any netlist analysis.  It’s often the end of the path that is  important for further LVP analysis, so knowing the end  eliminates the need for analysis of the other sites.


Second, one of the more challenging tasks in LADA analysis  is to correlate the sites with the path of logic gates. Uncertainty in the CAD overlay leads to many possible gates  at each site.   Knowing the direction of propagation can  eliminate some of the possibilities and aid in extracting the  critical path schematic.


Measuring the logic transition value and the propagation  delay along the critical path.  As we show in [6], it is  possible to determine the logic values of the transitions along  the critical path, and to measure the propagation delay  between gates (see Figure 7).   TR-LADA can be used as a  complementary technique to LVP.  Because only transistors in  the critical path create a signal, there is no crosstalk from  neighboring signals.  However, for that same reason, it is not  possible to probe signals that control the critical path but are  not directly part of the race.


to+100ps


LVP Buffer B


Figure 6.  In this sequence of TR-LADA images, the 50ps laser pulse  was synchronized at the specified time relative to the beginning of  the test loop.  The direction of propagation of the critical signal is  evident by recording the time each site disappears.  The small sites  in the circled area are flip flop single-event upsets [7], unrelated to  the path observed by LADA.  These images are acquired with a


0.9NA air gap lens.


Resolving multiple events occurring at the same site.  In  some cases, multiple critical timing events occur at the same  site.  LADA averages the responses of the multiple events, leading to misinterpretation.


In one example, LADA results showed sites on a clock path  starting at the PLL and ending at a capture flip flop.  A racing  data path was not evident, as is typically seen in a LADA  critical timing analysis.  Netlist inspection revealed that the  capture flip flop was directly fed from a launch flip flop, driven by the same clock.  This implied that the failure must  be caused by an inability to store data into the capture flop.


In Figure 8, time resolved LADA on the last clock buffer in  the path shows two separate interactions: one at the falling  edge of the launch clock pulse, and a second interaction at the  rising edge of the capture clock pulse.  The n-well interaction  at the clock buffer starts as a pass (darker) site, because the  falling edge of the first clock pulse is sped up, increasing the  clock low time.  Later in time, as the laser pulse approaches  the rising edge of the second clock pulse, the n-well  interaction reduces the clock low time and the clock buffer site


to


transitions to a fail site.   The detailed analysis of the TRLADA waveforms from two clock buffers on this device  allowed us to conclude prior to LVP analysis that the clock  duty cycle was degraded as it progressed from the PLL  towards the capture flip flop. The low portion of the clock  pulse was being shortened on its path towards the flop. The  LVP analysis shown in Figure 7 confirmed our TR-LADA


to+20ps


200 ps/div


LVP Buffer A


to+60ps


Spot Mode TR-LADAFailure Rate vs.Time measurements.


|TR-LADA|100 ps/div||
|---|---|---|

|Buffer A||TR-LADA|

|||Buffer B|

Figure 7.  TR-LADA and LVP waveforms taken at two clock buffers – Buffer A near the PLL, and Buffer B downstream in the clock tree  near a flip flop.  The TR-LADA waveforms are scaled to match the  time/division of the LVP waveforms.   Note that the A-to-B  propagation delay measured via TR-LADA closely matches the LVP  measurement.  Similarly, the width of the low clock pulse as  measured by TR-LADA is in close agreement with LVP.  TR-LADA  was able to show, prior to LVP analysis, that the failure was caused  by a degradation of the clock duty cycle.


Figure 8. These CW LADA and TR-LADA images illustrate that  multiple events at a site can be separated with TR-LADA.  The clock  buffer is the left site. The clock duty cycle was degraded, so the low  time was too short.  Images were taken at several times during the


clock cycle.


:


Case Study: Using Time Resolved LADA to  Locate a Defect


The use of LADA is often associated with finding critical  paths that have not been timed correctly in the design. However, it is also useful to locate manufacturing defects.


to+200ps


Many defects can be very sensitive to laser illumination, limiting the localization resolution.  The short pulse of  picosecond TR-LADA, however, reduces the effect of the


to+600ps


laser illumination and can improve localization.


Several 28nm-node devices were submitted to the lab which  had a reduced maximum frequency for a specific memory  array test (see Figure 9).   LADA analysis revealed sites in the  read/write circuit of the tested array, as shown in Figure 10. One site in particular (circled) was more sensitive to the laser  illumination and too large to isolate to a single transistor.


A sequence of TR-LADA images was acquired with the laser  pulse synchronized 100ps later for each image.  A subset of  those images is shown in Figure 10.  At time t0+200ps,   the  circled site of interest appears as a very small localized site, and later grows larger.  When overlaid in the CAD layout, the  TR-LADA site implicated a two-fingered transistor in the  sense amp.


Figure 11 shows that nanoprobing of the gate resistance  showed an open contact to one of the two fingers.   TEM  analysis, not shown, confirmed that the contact was open.


ClockFlip


13ery11#mvBufferFlop


nWell interaction


CWspeeds up both edges


1017.5mV1937.50V375mrd-Failing Unit


0xZ.5wV12.500v


BNV-


parod


pencid 20m1562isans025020m 3750VPassing Unit


Figure 9.  Shmoo of a part failing a memory BIST test showed that


it was slow relative to a passing unit.  For LADA analysis, the part  was biased at the pass/fail boundary at 987mV, such that the  average test loop fail rate was approximately 50%.


<


Figure 10.  This montage of images shows the LADA and TR-LADA  analysis.  The LADA analysis revealed several sites, including the  circled asymmetric site.  TR-LADA images taken at 100ps steps  showed that this site starts out very small at t0+200ps and grows  larger.  The t0+200ps image was overlaid with CAD layout, implicating a two-fingered transistor in a sense amp in the memory  array.  The fingers are labeled “A” and “B” for reference in Figure


11. Polysilicon is green and contact is yellow in the CAD layout.


Images were acquired with a 0.9NA air gap lens.


Figure 11.  The resistance of each of the polysilicon fingers to the  driving transistor was measured with the nanoprobing tool. Finger  B had a very high resistance contact.


Summary


In this paper, we have demonstrated a practical TR-LADA  system that enhances traditional CW LADA.   TR-LADA  complements the existing toolset, enabling faster resolution of  issues.  Specifically, we have shown how TR-LADA


1. Increases the LADA localization resolution be eliminating the well interaction,


2. Provides the timing of the event detected by LADA,


3. Indicates the propagation direction of the critical signals detected by LADA,


4. Allows the analyst to infer the logic values of the critical signals, and


5. Separates multiple interactions occurring at the same site for better understanding of the critical signals


1. Rowlette, Jeremy A., and Travis M. Eiles. "Critical timing analysis in microprocessors using near-IR laser assisted device alteration (LADA)." In 2013 IEEE International Test Conference (ITC), pp. 264-264. IEEE Computer Society, 2003


2. Shaw, Jonathan, Christopher McMahon, Yin Shyang Ng,and Felix Beaudoin, “Dual Port RAM MBIST Failure Analysis using Time Resolved Dynamic Laser Stimulation” In Proceedings of the 34th International Symposium for Testing and Failure Analysis”,  pp. 188-191, ASM 2008


3. Erington, Kent, John Asquith, and Dan Bodoh. "Software enhanced time resolved laser assisted device alteration with a non-pulsed laser source." In Proceedings from the 35th International Symposium for Testing and Failure Analysis, p. 43. ASM International, 2009.


4. Bodoh, Dan, and Kent Erington. "Improving the DLS Workflow." In Proceedings from the 38th International


Symposium for Testing and Failure Analysis p. 183. ASM  International, 2012.


5. Serrels, Keith A., Kent Erington, Dan Bodoh, Carl Farrell,Neel Leslie, Theodore R. Lundquist, Praveen Vedagarbha, and Derryck T. Reid. "Two-photon laserassisted device alteration in silicon integrated-circuits."Optics Express 21, no. 24 (2013): 29083-29089.


6. Erington, Kent, Dan Bodoh, Keith Serrels, Chris Nemirow, Neel Leslie, Theodore Lundquist, Praveen Vedagarbha, Carl Farrell and Derryck T. Reid,“Measuring Propagation Delays of Critical Paths Using Time-Resolved LADA” International Reliability Physics Symposium 2014


7. Serrels, K, N. Leslie, T. R. Lundquist, P. Vedagarbha, K.


Erington, D. Bodoh, C. Farrell and D. T. Reid, “TwoPhoton-Absorption-Enhanced Laser-Assisted Device Alteration and Single-Event Upsets in 28nm Silicon Integrated Circuits”  In Proceedings from the 39th International Symposium for Testing and Failure Analysis.


ASM


International


Comparative Study on Decapsulation for Copper and Silver Wire-Bonded  Devices


François KERISIT and Bernadette DOMENGES


LaMIPS, CRISMAT-NXP semiconductors-Presto Engineering joint laboratory,


CNRS-UMR 6508, ENSICAEN, UCBN, Presto-Engineering Europe, 2 rue de la Girafe, 14000 Caen, France   f.kerisit@digit-concept.com, +33 2 31 354 354


Michael OBEIN


Digit Concept, Chemin de St Sulpice, 14740 Secqueville en Bessin, France


[12] M.S.A. Holtz et al, “On Die CMOS droop detection and  dynamic compensation” Proceedings of the 19th ACM  Great Lakes Symposium on VLSI, pp 35-40, 2008


[13] R. Petersen, et al “Voltage Transient Detection and  Induction for Debug and Test”, paper 8.2, IEEE- ITC


2009.


[14] E.A. Burton, et al “FIVR-Fully Integrated Voltage  Regulators on 4th Generation Intel® CoreTM SoCs”, IEEE-APEC, 2014, page 432-439.


[15] P. Hammarlund, et al “Haswell: The Fourth-Generation  Intel Core Processor”, IEEE-Micro, March/April, 2014, pp6-20


The Role of Free Carrier Absorption in LADA


Kent Erington, Dan Bodoh, Kris Dickson, and George Lange


Freescale Semiconductor, Inc., 6501 West William Cannon Drive, Austin, Texas 78735, USA


1. Introduction


The technique of soft defect localization (SDL) [2] uses a  detection and imaging scheme similar to LADA, but it  employs a continuous wave (CW) ~1300nm laser, a  wavelength longer than the intrinsic absorption edge of  silicon.  SDL has been primarily used to locate defects in  metallization rather than identifying critical speed paths. However, in [2] the authors note that SDL can slow a ring  oscillator and attribute the effect to carrier mobility being  reduced by heating.


Subsequently, it has been observed that ~1300nm irradiation  can also speed up transistors, which is inconsistent with  reduced carrier mobility.  In [3] and [4], the authors suggest  that the device interaction with ~1300nm irradiation is due to  two photon absorption LADA (2pLADA).


In sections 2-4 of this paper, characterization of CW 1340nm  laser induced currents and the LADA failure rate will show  that a two photon absorption explanation for the LADA effect


OBIC in a Diode


is not plausible.


0****


Extensive work on 10µm gate length transistors in [5]


-100


△1064nmOBIC0**


characterized the effects of a ~1300nm laser on MOS


口 u


X1340nmOBIC4口


-200


transistor current.  Several effects were described, each


u-3004


0*


dominating at different bias regions.


dd n 3


-500


y=-0.033x2


39


-400


In sections 5 and 6 of this paper, we confirm the results in [5]


p U-600


p25x


on a 28nm-node nMOS transistor using a 2.45NA solid


-700


0102030


immersion lens (SIL).  In section 7, we compare the effects of


-800


global heating to that of local laser heating.    In section 8, we


-900


show that the LADA response time to ~1300nm irradiation is


051015202530


<< 100ns.


Given the data in [5], and our characterization of 28nm CMOS  laser induced transistor current and LADA response time, we  introduce in section 9 an explanation for LADA at ~1300nm – free carrier absorption in the silicon and in the local silicide  layers.


In section 10, selected 1320nm LADA images on 28nm-node  devices are presented and shown to have characteristics that  support our discussion in section 9.  We will show 1064nm  LADA images on the same structure that indicate that 1064nm


interaction with transistors is likely related to free carrier  absorption, rather than electron-hole pair creation.


Throughout this work two LSM systems were used.  Both an  air gap lens LSM system with a 1340nm laser and a solid  immersion lens (SIL) LSM system with a 1320nm laser were  used.  We have indicated each wavelength in the data, but we  assume in this paper that the wavelengths are equivalent.


2. Two-Photon Absorption in a Diode under CW 1340nm Irradiation


Figure 1 confirms the observation in [3] that CW 1340nm  irradiation of a diode structure does induce a current that is  consistent with two-photon absorption, and that the current is  2-3 orders of magnitude lower than CW 1064nm optical beam  induced current (OBIC).  Note that during these measurements  the laser spot was oriented so that it did not irradiate metal  layers or heavily doped silicon regions in order to eliminate  any free carrier absorption and Seebeck effects.   Confirming  these results, however, did not answer how the small twophoton current could have induced LADA.  Because LADA is  based on laser interaction with transistors, on-chip test  structure transistors were characterized next.


Figure 1.  Using a thermal diode on a 28nm-node test structure, we  show in these graphs that both 1064nm and 1340nm irradiation  induce current in a diode biased at 0 volts.  However, the 1340nm  optical beam induced current (OBIC) is 2-3 orders of magnitude  smaller than the 1064nm OBIC.  As the inset shows, the smaller  1340nm OBIC has a quadratic relationship to the laser irradiance, consistent with two-photon OBIC (2pOBIC) as discussed in [2].


Laser Irradiance (mW/µm2)


3. 1340nm Laser-Induced Transistor Off Current


1400


To study the effect of 1340nm irradiation on transistors in a


十nMOSLeakage, Vds=1.015V


CMOS circuit, a leakage test structure on a 28nm bulk CMOS


1200


XnMOS Leakage, Vds=0.894V


IC was used.  The circuit, illustrated in Figure 2, allowed the  leakage in the nMOS of a CMOS inverter to be measured


1000


1064nm Diode OBIC X1340mm Diode OBIC


while it was illuminated by a CW 1340nm laser through ~100


8800


microns of silicon.


P6008 n


VA


p400


200 0


Figure 2.  This leakage structure was used to study the effect  of 1340nm irradiation on a CMOS gate.  Biases of 1.015V and


0.894V were applied to VA while Q and Enable were both  held low.  The nMOS off current in the inverter with 1340nm  illumination was then measured as IA.


As shown in Figure 3, the nMOS exhibits leakage current that  is linearly related to the 1340nm laser irradiance.  In order to  compare current magnitudes we have also included the diode  current measurements of Figure 1.  The 1340nm induced  nMOS leakage current is much larger than the 1340nm  2pOBIC diode current, and is on the same order as the  1064nm diode OBIC. The linearity of the 1340nm induced  current, its magnitude, and the fact that the laser induced  current is detected as IA (source current) on an nMOS device  with VGS=0V are all inconsistent with two-photon absorption.


Figure 1: SEM picture of undamaged silver wires after  laser ablation, exhibiting one crater (arrow).


Based on our experience of copper wired ICs, we know that  low temperature (10 °C) decapsulation is efficient to preserve  wires, as the activity of the acid on the wires is lowered, while  still etching the EMC [4]. At 10°C, we use 100% fuming nitric  acid and fuming sulfuric acid with 20% SO3, with nitric to  sulfuric ratios ranging from 2:1 up to 5:1.


Dry chemistry was performed with a RF plasma chamber  running on three gases at 13.56 MHz (SesamePLASMADcap)


[6]. In order to preserve the package mechanical integrity, the  device is wrapped with copper tape [7]. But plasma still finds  its way around and etches the protected part of the package, thus making the device fragile or non-testable. Therefore we  use green silicone paste (originally meant for dental  impressions) to protect the package around the pins, pads or  balls.


In these case studies, we used oxygen and fluorinated gas CF4  to etch the EMC away. As the epoxy turns into ashes, a silica  filler layer builds up and prevents the plasma attack. Therefore  the equipment is fitted with a CO2 blast to remove these fillers  between each 10 minutes-long cycle and start again plasma


1mm


attack on a clean surface. Plasma generation raises the  temperature of the whole chamber, therefore the tray and  sample holder can be cooled down from 80°C down to 25°C. The working pressure in the chamber has to remain around  4000 mTorr to allow proper RF tuning between the generator  and the chamber. The RF power can be set up to 300 W, but  we will use it in the 50-100 W range as too much power would  damage the parts.


Looking for any damage on the wires and/or chips, the  decapsulated samples were controlled with optical microscopy  and Scanning Electron Microscopy (SEM). Energy Dispersive  X-ray spectrometry analyses were also performed to evaluate  the composition of the Ag-based wires and characterize the  observed residues if any.


Results


Copper wire – type #1


This case study shows wet and dry chemistry decapsulation on  a copper wire-bonded device, with wire diameter of 20 µm. Front-side opening was necessary in order to realize  photoemission microscopy on the die and should not affect the  electrical functionality of the opened ICs.


Copper wire – acid decapsulation


Low temperature acid decapsulation was proven to work on  copper wire. Gold-wired package allows multi-step opening


with wet chemistry, as the acids only etch the EMC away. It is  possible to under-etch the package, rinse it and run a second  step. Regarding copper wires, we observed that it is better to  do a one-shot decapsulation, based on bonding quality and  coating material around the wires. Below is an example of an  opened device in two 600 s-step process with a 2:1 ratio  chemical at 10°C, followed with several rinse baths, acetone to  stop the acid attack, hot water and finally alcohol to remove  water traces [4]. Broken wires are observed after this two steps


process (Figure 2). But this phenomenon is not seen by using  one-step process, where the sample is kept in the equipment  under pressurized nitrogen, and broken wires in two step  process may be due to oxygen or air humidity exposure  between the two steps.


To open gold based ICs, one step etching times can be reduced  about 10 to 20% of total time from those of the multi-step  decapsulation in order to avoid over-etching. Thus, using the  same parameters with 1000 s process, we could expose the die  and preserve the wires, though the wire surface is slightly  attacked (Figure 3 and 4).


Indeed, copper is not as forgiving as gold and requires special  care. Most often, sacrificial samples should be etched first to  establish the right conditions based on the package type and  die size. This is not possible for critical analysis. Plasma  decapsulation appeared to be an interesting route to open such  devices.


Figure 3: Acid decapsulation on device in a single step of  1000 s.


Figure 2: Acid decapsulation of a device in two steps of


600 s, total of 1200 s, which shows broken wires (red  arrows).


Copper wire - plasma decapsulation


So, we tested plasma decapsulation along with acid  decapsulation. Samples have been processed in the plasma  chamber. Dry chemistry parameters are 40% CF4, 60% O2, 50 W power and low temperature of 25°C with a CO2 blast  between each cycle. When the passivation is visible, we then  reduce the amount of CF4 down to 10% to avoid damaging the  nitride passivation of the die. Total etching time for those  samples is between 3 to 4 hours. A final acetone rinse in  ultrasonic bath was needed to remove residues on the surface  of the die.


Table 2: Plasma parameters


Process Temp. (°C) %CF4


%O2


Fast


25


40


Slow


90


As seen on Figure 5 and 6, ball-bond and wire surface are  much more preserved with plasma etching than with acid


etching. Furthermore, the electrical functionality of the opened  devices was also checked before the photoemission  microscopy analysis which could be successfully performed.


Silver wires, type #2


This case study shows wet and dry chemistry decapsulation on  a silver-alloy wire-bonded device, with wire diameter of  15 µm. The aim was to demonstrate feasibility of the  decapsulation technique with silver wire.


Silver type #2 – acid decapsulation


Several experiments of acid etching were performed with  different acid ratios at low temperature on different type of  silver-based ICs. All were unsuccessful. We will only detail  here results for type #2 IC. We used a 2:1 ratio at 10°C for  120 s. It confirmed, unfortunately, that the Ag wires are more  sensitive to acid attack than the Cu ones. All wires are  attacked, severely thinned and/or broken (Figure 7).


Figure 7: SEM image of thinned and broken silver wires  after acid decapsulation, type #2


Figure 6: SEM picture of ball-bond after 230 min of


plasma etching.


Figure 5: Plasma decapsulation on device showing  slightly bent wires probably due to direct CO2 blast.


Figure 4: SEM picture of ball bond after acid


decapsulation in a single step of 1000 s.


Silver type #2 – plasma decapsulation


Samples have been processed with the mixture 40% of CF4, 60% of O2, variable power and temperature of 80°C, following  the plasma chamber manufacturer's advices.


First plasma trial was done at 100 W of RF power. This  plasma appears too reactive as all wires exhibit strong surface  modifications, some of them being completely broken (Figure  8). Therefore, the power has been reduced down to 50 W (Figure 9). There still is surface modification, but only one cut  wire.


In order to increase selectivity between wire and resin, we  lowered the temperature of the chiller down to 25°C. This  decrease in temperature also makes the plasma less reactive  and then reduce the resin etch rate. A total etch time of 200  minutes was necessary to completely expose the die. On one  hand, it is a very long duration for a single sample. On the  other hand, this allows a step by step procedure with a precise  control over the etching. Table 3 summarizes etch times for  acid and plasma etching, showing that a lower reactivity  induces a longer etch time but better results.


Table 3: Measured wire diameter, type #2 IC


Mean   Dia. (µm)


Diameter   Range


Etch time (min)


Laser*


16.0


15.5 – 17.0


Acid


n/a


P. 80°C 100W


17.2**


15.8 – 20.0


P. 80°C, 50W


19.2**


16.2 – 21.4


P. 25°C, 50W


14.8


14.1 – 15.3


200


* laser ablation pre-opening on all samples ** most wires are still embedded in resin


SEM observation shows that none of the wire is broken (Figure 10). The surface appears to be slightly modified, but  the overall result is good. Small spheres remain on the wires  after etching (Figure 11). EDXS-SEM showed it was silicon.


Wire diameters have been measured showing that once EMC  is completely removed, the wires are etched, and their  diameter decreases (Table 3). A reference value of wire


Figure 10: SEM image of slightly attacked wires after  plasma decapsulation at 50 W and 25°C, type #2 IC.


Figure 9: SEM images after plasma decapsulation at


50 W and 80°C, type #2 IC. a) wires are still embedded  in resin, b) only one single broken wire.


Figure 8: SEM image after plasma decapsulation at  100 W, type #2 IC; broken wires and some wires are still  embedded in resin (arrow).


diameter was obtained after laser ablation, while wires are  partially exposed.


Silver wire: type #3, Stacked die


Same gas mixture was tried on a device with wires containing  Ag 90% and Au 10%, which is less silver than in the previous  package type. The device contains 4 memory dice and a  smaller top die, confined in an eMMC package. The sample  was processed at 50 W and 80°C also. All wires are attacked, but none is broken. We observed cracks on the balls and  passivation damages when trying to fully expose the pads of  the top die (Figure 12).


Decapsulation at 25°C seems to be less corrosive with fewer  cracks on the balls and less damage on the wire, but there is  still a strong surface modification (Figure 13).


Same SEM observations were obtained on the connections  between the stacked memory dice (Figure 14 and 15).


Figure 15: SEM image showing surface modification on  the wire, type #3 IC, 50 W 25°C, stacked die


Figure 14: SEM image showing a crack on the wire, type


#3 IC, 50 W 80°C, stacked die


Figure 13: SEM picture showing fewer cracks on the ball


with surface modification on the wire, type #3, 50 W 25°C, top die


Figure 12: SEM image showing cracks on the ball, type #3 #3 IC, 50 W 80°C, top die


Figure 11: SEM close-up image of wires with remaining


silica fillers after decapsulation at 50 W and 25°C, type #2 IC.


Silver wire : type #4


This device contains Ag 97% and Au 3%, it has the highest  Ag percentage of all sample types. The sample was processed  at 50 W and 80°C. We were not able to even partially expose  the die without breaking all the wires (Figure 16).


At 25°C, we were able to almost fully expose the die, but we  observed strong surface modifications and at least one broken  wire (Figure 17).


Silver wire: type #5, crystal artifact


The type #5 silver (unknown composition) wire-bonded  device was processed at 50 W and 25°C. After the plasma  decapsulation, we observed needle-like crystals, very unstable  under the electron beam (Figure 18). EDXS-SEM analysis  showed, it contained Si, F, O, N and C elements and no trace  of Ag metal (Figure 19). The Si EDXS signal may be due to  the true presence of Si in these crystals, as a result of  contamination by the protective silicone paste used for plasma


experiments, which more precisely is polyvinyl siloxane or  reaction with the SiO2 fillers. As we did not observe these  needles in the other silver ICs, the Si EDXS signal is most  probably due to X-ray fluorescence artifact because of the  surrounding SiO2 silica fillers. Furthermore, as the analysed  crystals collapsed under the electron beam during the EDXS  spectrum acquisition, it was very difficult to keep manually  the beam on them and avoid the interference with surrounding  EMC. The strong F EDXS signal shows that fluorine is the  main component of the crystals, coming from the CF4 gas used  for plasma etching.


Discussion


Analysis before and after plasma etching, IC type #3


In order to understand the impact of the plasma etching on the  silver-based wires, EDXS analysis has been performed first  after the laser ablation and second after plasma etching.


The EDXS spectra are superimposed on Figure 20. EDX  spectrum of the wire after laser ablation (green graph) shows  proportions of Ag and Au matching the ones given by the  supplier for type #3 IC. Besides, traces of palladium were  detected though they were not given in the manufacturer  specifications. After plasma etching, the central area of the


Figure 19: EDXS-Spectrum of crystal, showing Si, F, O, N and C signals (40 s, 5 kV).


Figure 18: SEM picture of non-conductive crystal on wire.


Figure 17: SEM image of attacked and broken wires, 50 W  25°C, type #4


Figure 16:SEM image of attacked and broken wires 50 W


80°C, type #4


wire (red graph) shows a higher peak of Au compared to Ag (red arrow) and the Pd peak also increases. It means that the  plasma etches the Ag away. In the area of the wire closest to  the top surface of the device and thus to the neighboring  remaining EMC (top wire, purple graph), EDXS analysis  shows that the wire composition is similar to the composition  found after laser ablation. This part of the wire has been  plasma etched for little time, but we observed crystals in the  same area (Figure 21). The light blue graph of the crystal  analysis shows Si, O (silica filler), Ag but neither Au, nor Pd  anymore.


This might explain how the Ag is taken away from the wire. The plasma reacts with the silver leading to the formation of  Ag-based crystals, which are further destroyed by the plasma, or removed by the CO2 blast. This plasma composition should  be adapted to silver-based devices.


This study showed that both acid and plasma decapsulation  can be successful with copper wire packages. Wet chemistry  at low temperature provides a relatively quick decapsulation  mean, yet consuming a lot of acid for large packages or hard  EMCs and offering less control on the endpoint of the  opening. Plasma decapsulation seems to offer more latitude  regarding EMC etching and preservation of the wires, yet etch  time is long. Regarding silver wires, our experiments show  acid etching at low temperature does not work, but plasma  could be a solution, even though it slowly consumes the silver  in the wire and may lead to breaking of the wires which  depends on the wire composition. Thus, further experiments  should be performed at low temperature and with different  plasma compositions to study the selectivity and sensitivity on  silver wires.


Acknowledgment


Thanks to Presto-Engineering FA team and especially to  Christophe Pistis for his helpful advices and to the ANRT for  financial support.


[1] Kai, L.J. et al, "Silver alloy wire bonding," 62nd Electronic


Components and Technology Conference, 2012 IEEE


62nd, San Diego, CA, May 2012, pp.1163-1168.


[2] Chen, Q.J. et al, "Cu wire and beyond - Ag wire an


alternative to Cu?," 12th Electronics Packaging


Technology Conference, Singapore, Dec. 2010, pp. 591-


596


[3] Lan, A. et al, “Interconnection Challenge of wire bonding


– Ag alloy wire,” Proc. 15th  Electronics Packaging


Technology Conference, Singapore, Dec. 2013.


[4] Lefevre, M. et al, “New method for decapsulation of


copper wire devices using LASER and sub-ambient


temperature chemical etch,” Proc. 37th International


Symposium for Testing and Failure Analysis, San Jose,


CA,  Nov. 2011, pp. 248–255.


[5] Murali, S.; Srikanth, N., "Acid Decapsulation of Epoxy


Molded IC Packages With Copper Wire


Bonds," Electronics Packaging Manufacturing, IEEE


Transactions on , vol.29, no.3, pp.179,183, July 2006.


[6] Aubert, A. et al., "New Front Side Access Approach for


Low-k Dielectric / Cu Technologies in Plastic Package


New decapsulation technique description" Proc. 37th


International Symposium for Testing and Failure Analysis,


San Jose, CA,  Nov. 2011, pp.  256–261.


[7] Staller, K, “Low Temperature Plasma Decapsulation of


Copper-Wire-Bonded and Exposed Copper Metallization


Devices”. Proc. 36th International Symposium for Testing


and Failure Analysis, Addison, TX, Nov. 2010, pp. 127–


132.


Figure 21: SEM image of type #3 IC after plasma  decapsulation. Colored squares show regions of interest  for EDXS analyses near the top end of the exposed wire.


Figure 20: EDXS spectra of a type #3 sample after laser


ablation only, and after laser and plasma etching on 3  different spots of the wire (30 s, 10 kV).


Laser Focus Depth Adaptation for Decapsulation of Copper Wirebonded Devices


H. B. Kor1, Q. Liu1, Y. W. Siah1,2, C. L. Gan1,2


1Nanyang Technological University, Temasek Laboratories@NTU, 9th Storey, BorderX Block, Research Techno Plaza  50 Nanyang Drive, Singapore 637553.


2Nanyang Technological University, School of Materials Science & Engineering,


50 Nanyang Avenue, Singapore 639798.


hbkor@ntu.edu.sg, +65-6592 3725


Although pre-laser decapsulation reduces the time to acid  exposure for subsequent chemical decapsulation of copper  wirebonded devices, it can result in severely damaged or  broken copper wirebonds if carried out at a focused depth  followed by chemical decapsulation. Thin quad flat packages (TQFPs) of dimensions 22 mm × 22 mm, with copper  wirebonds were pre-laser decapped (Nd:YAG laser, 1064 nm) at three depths of focus, at focus, (z-0.5) mm and (z-1) mm. Reducing the laser focus depth by 1 mm, followed by  subsequent chemical decapsulation, resulted in the least  damage to copper wirebonds. Average percentage reduction in  copper wirebond diameter after complete (laser and chemical) decapsulation is about 2.30%.


Copper wires are replacing gold wires in microelectronic  packaging due to their relatively lower cost and superior  properties in terms of electrical and thermal conductivities and  mechanical strength. It can be found from literature that  various recipes or combination of recipes in terms of plasma (dry), laser and chemical decapsulation have been developed  for the successful decapsulation of copper wirebonds. Some of  these are related to the chemical etching temperature, mixed  acid ratios and concentration, etc. [1-7].


Pre-laser decapsulation is often carried out prior to chemical  decapsulation during the opening of copper wirebonded  packages to reduce the time to acid exposure for copper  wirebonds. However, a focused laser depth during pre-laser  decapsulation followed by subsequent chemical decapsulation  could result in severely damaged or broken copper wirebonds. The aim of this paper is to study the effects of defocussing  laser during pre-laser decapsulation of copper wirebonded  devices, while maintaining the integrity of the copper  wirebonds for further failure analysis.


Experimental Details


Thin quad flat packages (TQFPs) of dimensions 22 mm × 22  mm, with copper wirebonds consisting of 97.28% of copper,


2.70% of palladium and 0.02% of impurities were predecapped by laser (with Sesame 1000 laser decapsulation  system), followed by chemical (using Nippon Scientific


PS103S system). The copper wires were examined under both  the optical microscope and scanning electron microscope (SEM).


The copper wirebond diameters were measured after pre-laser  decapsulation and after complete (laser and chemical) decapsulation. Table 1 shows the laser decapsulation  parameters used for the pre-laser decapsulation of the copper  wirebonded TQFPs.


Table 1: Laser decapsulation parameters used for the prelaser decapsulation of copper wirebonded TQFPs


Laser power (%)


Frequency (kHz)


16


Duty cycle (%)


95


The depth of focus of the laser was varied at focus, (z-0.5) mm  and (z-1) mm. The samples were chemically decapped using  fuming HNO3 and concentrated H2SO4 (10:1), at 22°C, for a  duration of 1 min 30 s, followed by cleaning using IPA, acetone and water.


Figure 1 shows the SEM images of the copper wirebonds after  pre-laser decapsulation and after complete decapsulation, at a  focused laser depth, while Fig. 2 shows the overview optical  image after complete decapsulation.


Figure 1: SEM images of copper wirebonds (a) after pre-laser  decapsulation, (b) diameter measurement of copper wire after  complete (laser and chemical) decapsulation, (c) broken wires  and (d) debonded wires, laser depth at focus


Figure 2: Optical image of TQFP after complete (laser and  chemical) decapsulation, laser depth at focus


It can be observed from Fig. 1(a) that when the laser depth is  at focus, burn marks formed on the surface of the copper  wirebonds. This can be explained by the relationship between  the laser intensity and the beam spot size in the following  paragraphs.


The design of the laser machine can be found in Fig. 3, where  the laser galvo head consists of the laser with the galvanometer  and focusing lens.


Figure 3:Schematic of laser galvo head design (Sesame 1000)


[8]


Assuming that the laser beam is a point source and there is no  energy absorption or scattering by the medium through which  it propagates, the laser intensity is a function of the power over  the beam area. This relationship can be described in Eq. (1) –


(3) [9].


 





d


I


P


where P is the net power irradiated, I is the intensity as a  function of position, and d A is a differential element of a  closed surface containing the source. Performing integration  over a spherical surface of uniform intensity I, Eq. (1) becomes:


surf


4 w








(2) where I is the intensity at the surface of the sphere and w is the  radius of the sphere. Rearranging Eq. (2) gives:


The Gaussian function in Eq. (4) can be used to represent the  transverse profile of the laser intensity of the beam with a  power P [9]:


 ,








where r is the  radial distance from the centre axis of the beam, z is the axial distance from the beam’s narrowest point, w(z) is  the beam radius, the distance from the beam axis at which the  intensity of the beam drops to 1/e2 of the maximum value [9, 10]. This is illustrated in detail in Fig.4.


Figure 4: Irradiance vs distance plot of a Gaussian beam [10] With a fully focused laser beam, the laser beam spot size is  reduced, resulting in peak laser intensity on the copper  wirebonds, which can be described by Eq. (5) [9]:


P





The laser heats the surface of the copper wirebonds and finally  melts it [11], leaving behind striation marks. Subsequently, after complete decapsulation, besides the severe shrinkage of  the copper wirebonds (Fig. 1(b)), some copper wirebonds  broke (Fig. 1(c)), while some stitch bonds debonded from the  leadframe (Fig. 1(d)).


The severe shrinkage of the copper wirebonds after complete  decapsulation could be due to the chemical interaction of the  mixed acids with the palladium on the copper wirebond  surface. Palladium reacts slowly with fuming nitric acid and  concentrated sulphuric acid, forming palladium nitrate, palladium sulphate and hydrogen gas, respectively, as shown


I P


in Eq. (6) and (7):


Asurf


4 w


Pd(s) + 2HNO3(aq)   Pd(NO3)2(aq) + H2(g)





Pd(s) + H2SO4(aq) PdSO4(aq) + H2(g)


(7) Without the protective layer of palladium on the surface of the  copper wirebonds, copper wirebonds are readily attacked by





r2


the mixed acids, resulting in corrosion on the surfaces, as





zw P


z


r


2 2/


exp


 zw 2


explained in Eq. (8) and (9):


Cu(s) + 4HNO3(aq)Cu (NO3)2(aq) + 2NO2(g) + 2H2O(l) (8) Cu(s) + 2H2SO4(aq)CuSO4(aq) + SO2(g) + 2H2O(l) (9) The corrosion could be a result of the combined effects from  the laser peak intensity, as well as the chemical reactions  between the mixed acids with the copper wirebonds. Pre-laser  decapsulation at laser focus depth of (z-0.5) mm was carried  out next to see the effects.


Figure 5 shows the SEM images of the copper wirebonds after  pre-laser decapsulation and after complete decapsulation, at  laser focus depth of (z-0.5) mm, while Fig. 6 shows the  overview optical image after complete decapsulation.


2/2w


Figure 5: SEM images of copper wirebonds (a) after pre-laser  decapsulation, (b) after complete (laser and chemical)


decapsulation and (c) diameter measurement of copper wire  after complete decapsulation, at laser focus depth of (z-0.5) mm


Figure 6: Optical image of TQFP after complete (laser and  chemical) decapsulation, at laser focus depth of (z-0.5) mm


It can be observed from Fig. 5(a) that when the depth of focus  of the laser is (z-0.5) mm, there is still some damage in the  form of burn marks on the surface of the copper wirebonds. With a slightly defocused laser beam, the laser beam spot size  is increased, resulting in a reduction in laser intensity on the  copper wirebonds. Subsequently, after complete decapsulation (Fig. 5(b)), although pits formed on the surface of the copper  wirebonds, the damage to the palladium coated copper  wirebonds is reduced. The copper wirebonds are slightly  deformed and there is still shrinkage in wire diameter, but  there were no broken or debonded wires. Thus, the pre-laser  decapsulation was next carried out at (z-1) mm to verify if the  damage could be reduced further.


The introduction of silver as bonding material led to new  failure analysis issues. This study compares the efficiency of  wet and dry chemistries for decapsulation on Cu and Ag-based  alloy wires. It is shown that dry chemistry allows better  control and selectivity on the EMC/ Cu and Ag-based bond  wires.


For the past decade, developments to switch wire bonding  material from gold to copper have been done regarding  process, reliability and failure analysis. More recently, new  silver alloy bonding wires have been developed and raised  specific problems due to silver alloy properties. Whereas this  new type of wiring material seemed to fulfill most challenges, like physical properties and reliability [1,2], it was suggested  that specific Epoxy Molding Compound (EMC) should be  adopted in order to ease decapsulation [3]. With the move  from gold to copper, the failure analysis community had had  to come up with new decapsulation techniques [4,5]. As well, the introduction of silver alloys raised new problems of  decapsulation. Furthermore, failure analysts do not always  have all required information on the type of EMC and the true


Acc.VSpot MagnDetWD


50 μm


composition of the bonding wires.


5.00 kV 3.0500xSE5.32013/09/27 Ag wire


Two major techniques of decapsulation regarding wire-bonded  devices are known: wet (acid) and dry etching (plasma); LASER ablation or mechanical milling being used for preopening. This study will compare the capabilities of these  techniques on Cu wiring and four types of Ag-based wiring  integrated circuits (IC) (Table 1).


Table 1: Wire diameter and composition for each IC type (supplier data).


|IC # |Dia. (µm) |Composition ||
|---|---|---|---|

|1 |20 |Cu 100% ||

|2 |15 |Ag 95%, Au 0.5%, Pd 4.5% ||

|3 |15 |Ag 90%, Au 10% ||

|4 |18 |Ag 97%, Au 3% ||

|5 |20 |Ag based ||

Experimental


All samples were pre-opened using an infra-red pulsed laser  system (SesameLASER) to reduce the process time and  exposure time for both wet and dry chemistry. This preopening step, which is most often stopped just before reaching  the bonding wires, must not alter the wire integrity, as shown  on Figure 1.


Wet chemistry was performed with automated equipment  running on nitric and sulfuric acid (SesameACIDCu). This  common method for plastic package decapsulation uses  mixture of nitric and fuming (f) or non-fuming (nf) sulfuric  acids. This removes EMC efficiently while preserving Au  wires. But copper and silver are attacked by nitric and sulfuric  acids, see reactions (1) to (4).


Cu + 4 HNO3 → Cu(NO3)2 + 2 NO2 + 2H2O


Cu + H2SO4 → CuSO4 + SO2 + 2 H2O (2) 3 Ag + 4 HNO3 → 3 AgNO3 + 2 H2O + NO


2 Ag + H2SO4 → Ag2SO4 + H2


In Fig.7, apparent MR “ghost” images (red circles) were  observed along the both edges of active region. The change of  laser scanning direction did not show any change of such a  ghost effect.  If it is an artifact, it should be very small und  uncorrelated with the reference signal. However, just as  shown in Fig.6, to our surprise, the point measurements  showed that the MR amplitude at such edge regions is 6 times  larger than the normal signal at corresponding active regions. The lock-in phase MR result (left) shows also both of them  have stable but different phases. Therefore they should not  have the same physical origin. The large “ghost” signal poses  a great challenge to the probing of inner signal in advanced  logic products.


Fig.7. Left:  Lockin MR mapping phase image, Right: Lockin  MR mapping amplitude image. The amplitude and phase  signals were measured in the active region and neighboring  STI region in the red circles.


These spots are located at the boundaries of active regions, where a large laser reflection from M1 layer is expected. Since  in this area no free carrier exists, it cannot be ascribed to the  carrier effect.  One reasonable explanation is the electro  optical reflection due to vertical electrical field between  source/drain and the substrate at the end of a FET. The electro  optical coefficient due to external electrical field is normally  smaller than the contribution from carriers [19], but the


reflection is much stronger in these regions than in active  regions, i.e. the detection laser power is stronger.


In order to confirm such an origin, more detailed experiments  should be done. This point is very crucial, particularly to laser  voltage probing. It was observed that the probing signal has an  extreme dependence on the probing position, and the shift of  one or two pixels will lead to a large change of the MR signal! On the other hand, it can be helpful in voltage probing if the  signal is too weak in the active region.


The lockin phase mapping of modulated reflectance with SIL  is discussed in detail. With SIL, the improved spatial  resolution leads to a clear observation of MR phenomena, particularly the so-called ghost in the MRM amplitude  imaging.  The different lockin phase between active regions  and ghost regions showed clearly that both of them have  different physical origins. The pattern of MR phase mapping  in a reference cell can be utilized as a rapid tool to find the  failed cell. Furthermore, the phase transition in FF or subblocks in operating states leads to a sharp edge between  neighboring active regions of FETs and provides an  enhancement of spatial resolution for a precise localization of  defective FET in scan cell and sub blocks in advanced  technologies.


[1] R.A. Falk, “Advanced LIVA/TIVA techniques” , ISTFA  2001


[2] C. Boit, “Fundamentals of Photon Emission (PEM) in  Silicon-Electroluminescence for Analysis of Electronic  Circuit and Device functionality”, Desktop Reference of  Failure Analysis, 2005


[3] D.Vallett, “Picosecond Imaging Circuit Analysis –PICA”,  Desktop Reference of Failure Analysis, 2005


[4] M.R. Bruce et al., “Soft Defect Localization (SDL)”, ISTFA, 21-27 (2002)


[5] F. Beaudoin et al, “Lock-In Amplification Applied to  Thermal Laser Stimulation”,  2nd European Workshop on  Photonics Failure Analysis, Munich (2002)


[6] Z.-L. Qian et al. “LIA-SDL and its Application in Scanshift problems”, ISTFA 2005


[7] C. Brillert, Z.-L. Qian and C. Burmer, “Laser assisted  Lock-in Phase & Spectral Analysis Techniques at  advanced IC Failure Analysis with application to Jitter  and Soft-Defects”, ISTFA 2007


[8] Z.-L. Qian, C. Brillert and C. Burmer, “Mixed Frequency  Detection of Thermal Laser Stimulation and its  application in failure analysis”, ISTFA 2008


[9] Z.-L. Qian et al. “Differential and Lockin Imaging of


Dynamical Photon Emission and Applications in Failure  Analysis”, ISTFA 2010


[10] R.A.Soref, and B.R. Bennett, “Electro-optical Effects


in Silicon”, IEEE J. Quant. Electron., Vol QE-23, p.123,1987


[11] U. Kindereit, C. Boit  et al, “Quantitative  Investigation of Laser Beam Modulation in Electrically  active Devices as Used in Laser Voltage Probing”, IEEE  Transactions on Device and Materials Reliability, vol. 7, NO.1, March 2007


[12] F. Zacharisasse et al. “Laser modulation mapping on  an unmodified laser scanning microscope”, ESREF 2010


[13] C. Pagano, C. Boit and Y. Yokoyama, “ Detecting  Laser Beam Reflectance Modulated by Electronic Device  Operation with a Simple Setup”, IRPS 2011


[14] J. Teo, C. Chua, L.S.Koh, and J.C.H. Phang, “Nchannel metal-oxide-semiconductor characterization with  static and dynamic backside laser reflectance modulation  techniques”, Applied Physics Letters  99,094105, 2011


[15] S. Kasapi, W- Lo, J.Liao et al: “Advanced Scan  Chain Failure Analysis Using Laser Modulation Mapping  and Continuous Wave Probing”, IFTFA 2011


[16] S.H. Goh et al. “Effectiveness of frequency mapping  on 28nm device broken scan chain failures”,  Rev. of  Sci. Instr. 83, 023702(2012)


[17] J. Fine et al “optical Probing of FinFETs”, IPFA  2013


[18] Y.S. Ng et al., “Scan-Shift Debug using LVI Phase  Mapping”, ISTFA  2013


[19] Z.-L. Qian, C. Brillert and C. Burmer, “Lock-in  Phase Mapping of Modulated Reflectance in Dynamically  Operating Mixed-Signal IC Devices”, ISTFA 2012


Dr. Zhongling Qian*


Infineon Technologies AG


IFAG OP QM FA2


Am Campeon 1-12,


D-85579 Neubiberg


Tel.: 0049/89-234-26366


Fax: 0049/89-234-23497


Email: zhongling.qian@infineon.com


Visible Light LVP on Ultra-Thinned Substrates


Joshua Beutler, J. Joseph Clement, Mary A. Miller, Jeffery Stevens, and Edward I. Cole Jr.


Sandia National Laboratories, Albuquerque, NM, 87185, USA


ABSTRACT — Visible light laser voltage probing (LVP) for  improved backside optical spatial resolution is  demonstrated on ultra-thinned samples.  A prototype  system for data acquisition, a method to produce ultrathinned SOI samples, and LVP signal, imaging, and  waveform acquisition are described on early and  advanced SOI technology nodes.  Spatial resolution and  signal comparison with conventional, infrared LVP  analysis is discussed.


INTRODUCTION


Laser Voltage Probing (LVP) is a key backside optical tool  for modern failure analysis and real time logic debugging of  signals propagating at operational speeds through integrated  circuits (ICs).  Conventional LVP systems rely on free carrier  generation and optical absorption within the channel of  CMOS transistors to modulate reflected light intensity.  Infrared wavelengths are used to take advantage of silicon’s  relative transparency for backside probing.  The incident light  is reflected back, captured, detected, and amplified.  The  small modulations in reflected intensity resulting from free  carrier density changes with electric field are used to  determine local transistor logic states as a function of time.  This is a powerful tool for failure analysis and device  debugging/characterization [1-2].


With the continual reduction of IC feature sizes, backside, laser-based failure analysis tools are limited in spatial  resolution by the refraction limits of light and the relatively  long wavelengths required for through-silicon probing.  Even  with state of the art Solid Immersion Lenses (SILs), modern  22 nm devices are at and past the limit of practical resolution.   To address this spatial resolution limit, we developed and  demonstrate here the effectiveness of applying LVP with  shorter, visible wavelengths.  This is accomplished using  backside ultra-thinning of Silicon on Insulator (SOI) devices.  The devices are thinned sufficiently that shorter, visible  wavelengths can be used for LVP analysis, thus enabling  better spatial resolution and enhanced LVP signals.


SYSTEM AND SAMPLE DESCRIPTION


We demonstrate LVP using visible light (633-640 nm) on  locally ultra-thinned regions within SOI devices.  Creation of  an improved resolution reflected light image from the


backside through die thinning and shorter wavelength light  has been accomplished previously [3].  Our present work goes  further by using advanced deprocessing techniques to ultrathin localized areas on SOI devices to achieve a packaged, functionality-maintained IC.  These techniques include, gasassisted Focused Ion Beam (FIB) and XeF2 etching.


A modified LSM 310 scanning laser microscope was used to  demonstrate LVP using visible light.  In order to effectively  probe the transistor, a high gain, low noise Avalanche  Photodiode (APD) is used as the detector of the LVP signal (Figure 1).


Figure 1: Schematic diagram of a modified LSM 310 with an APD  detector and multiple wavelength sources for visible light LVP  analysis.


MOTIVATION AND BACKGROUND


Ultra-thinning and visible light microscopy significantly  enhances the resolution that can be achieved when using an air  gap lens.  This can be further enhanced to be roughly  comparable with advanced solid immersion microscopy using  infrared light when oil immersion microscopy is incorporated  with visible light.


Rayleigh criterion in Equation 1 equates the minimum  resolution limit of two points, D, to wavelength, λ, and


numerical aperture, NA, of the microscope objective. As  shown in Table 1 below, an oil immersion lens using visible  light to image ultra-thinned silicon will render ballpark  resolution performance to state of the art solid immersion  lenses imaging through bulk samples using infrared light.


Table 1


Lens Type


λ (nm)


NA


D (nm)


3.0 SIL


1320


3.0


270


1064


216


1.4 Oil


633


276


532


232


Air Gap


429


361


While these resolution enhancements do not surpass a state of  the art SIL, they do provide an alternative when SILs are not  an option. This technique gives significant enhancements, to  those working on SOI samples with thick Buried Oxide (BOX) layers which can be ineffective for use with SILs.  It  also gives another option to failure analysts that are not  equipped with state of the art imaging technology, but may  find it plausible to ultra-thin devices.  For SOI devices, this  technique also appears to enhance the sensitivity of the LVP  signal.  This is likely accomplished by reducing the loss  factors which occur when probing through many microns on  thick samples.


Figure 2:  Round-trip transmission of visible light through different  thicknesses of undoped silicon.  Data to create the curves was from


[5].


Visible light loss through doped silicon is high.  Despite high  losses, adequately thinned silicon, even at visible  wavelengths, provides sufficient reflected light to create an


image and capture an LVP signal.  The extent to which the  silicon must be thinned is shown in Figure 2.  In all cases  where the substrate is doped, losses will be higher.  Heavily  doped silicon will create substantially higher losses.


The examples shown in this paper are for SOI technologies.  Demonstration of the approach on bulk silicon devices will be  the subject of future work.


EXAMPLE RESULTS


Example 1: 350 nm SOI


As a proof of concept, an SOI device was prepared with a  region of interest consisting of a buffer amplifier (Figure 3) on  a 350 nm technology operating at 3.3 V.  The deprocessing  consisted of backside silicon FIB removal in the region of  interest.  FIB milling stopped shortly before the BOX layer.  The remaining residual silicon was removed by etch gasses  resulting in a clean, glass-like viewport to the areas of interest. A conventional, backside, 1320 nm LVP system was used to  show functionality of the buffer as well as derive an  understanding of the overall LVP signal for a given intensity  laser.


Figure 3: Reflected light image of the buffer on a traditional LVP  system using 1320 nm light to create the reflected light image and  the 1 MHz frequency map.


The visible light used to do LVP probing was a 5 mW, 633  nm HeNe laser, with approximately 100 W of power on the  sample.  The buffer amplifier was clocked with a square wave, the output of the detector amplified, and the signal observed  using a spectrum analyzer (Agilent EXA N9010A).  When  spotting the laser on the probe site, the primary harmonic from  the amplifier is seen in the spectrum analyzer at roughly 15  dBm above the noise floor (Figure 4).


Figure 4:  (Left image) Backside, 633 nm, reflected light image of a  buffer amplifier clocked at roughly 1 MHz.  When a 633 nm laser is  pointed at the transistor (red cross) and the reflected light captured  by the APD, the LVP signal is indicated by a spectral peak at the  periodic clocked frequency (right image).  The left image has better  resolution but poorer contrast than an IR image.  However, enhanced  resolution is the objective, and lack of contrast is of secondary  concern.


Figure 5 illustrates Laser Voltage Imaging (LVI) [4] of the  clocked buffer amplifier.  This is done by setting the spectrum  analyzer to a zero span at the frequency of the observed peak (1MHz).  The analyzer’s video output is used to modulate the  image contrast as the 633 nm laser is scanned across the  device.  In this example the frequency map is slightly offset  due to the scan speed and latencies within the spectrum  analyzer.  This is similar to conventional LVI, but shown here  to work at a visible wavelength.


Figure 5: When the buffer amplifier is scanned with the 633 nm  laser, the reflected light is collected by the APD and the resulting  signal fed into the spectrum analyzer zero spanned at the clock  frequency.  The video out option from the spectrum analyzer can  then be used to create a frequency map or LVI image of the buffer, highlighting operation at the clock frequency.


Figure 6 demonstrates that by spotting the visible laser at the  clocked buffer amplifer, a waveform of the amplifier’s logic  state with time can be acquired.  For this example the output  of the amplifed APD signal is displayed directly with  averaging on an oscilloscope.


Figure 6: By spotting the laser on the buffer (red cross in Figure 4), the output of the APD can be averaged to show the clocked  waveform. The yellow waveform is the averaged, clocked APD  signal. The green waveform is the trigger output from the periodic  clock.


In subsequent examples we demonstrate the possibility of  visible light LVP on advanced SOI technology nodes.


Example 2: 45 nm SOI


To further show the extent to which this technique is useful, we demonstrate ultra-thinned LVP on a more recent, 45 nm  SOI technology.  In this case, the region of interest, a simple  test inverter, was thinned using a XeF2 etch that stopped on  the BOX layer. Once this occurred, the region of interest was  viewable through the glass-like BOX region with visible  wavelengths.  This test inverter was clocked using an external  function generator at 1 MHz.  The inverter LVI and LVP  signals were then tested on a conventional 1320 nm LVP  system with a 50x objective and 5 mW probe power.  The  reflected light image and corresponding LVI image is shown  in Figure 7.


This sample was then tested on the visible light LVP system  with a 50x objective (Figure 8) and a 63x 1.4 NA oil  immersion lens (Figure 9).  The laser probe power though the  50x lens was 100 µW and 150 µW for the immersion lens.


Figure 7: Reflected light image and corresponding LVI image of a  45 nm inverter using a 1320 nm conventional LVP and 50x  objective.


Figure 8: Reflected light image and corresponding LVI image of a


45 nm inverter using a 633 nm laser and 50x objective on a visible


light system.


Figure 9: Enhanced resolution of the reflected light image and  corresponding LVI map using a 63x 1.4 NA oil immersion lens.


Not only does the oil immersion lens improve the resolution, it drastically improves the locality of the frequency map and  consequently enhances the intensity of the LVP signal.  This is  most easily seen by examining the plot in Figure 10 which  shows LVP spectral signals for a 50x, 633 nm laser and the  63x oil immersion, 633 nm LVP signal.  Figure 10 shows  LVP signal for the same region of interest increases by more  than 10 dBm when using the oil immersion lens.


Using the 63x oil immersion objective, the frequency map  from Figure 9 was used as an aide in probing the inverter.  The output of the inverter, LVP waveform, and clock trigger  are shown in Figure 11.


Figure 10:  Two spectral peaks that represent the LVP signal from  Figure 8 and Figure 9 in the frequency domain.  The peaks are offset  from their true frequency to illustrate the difference in signal  strength between a 50x 0.5 NA air gap objective and a 63x 1.4 NA  oil immersion objective.  In each case, the 633 nm probe laser was  pointed in the same region of LVP signal activity.


Figure 11:  A waveform capture from probing an active area shown  in Figure 9.  The top (magenta) is the electrical waveform measured  by the scope.  The middle waveform (yellow) is the averaged LVP  signal.  The bottom (green) waveform is from the clock trigger  output.


SUMMARY


The motivation for improved spatial resolution of LVP  analysis, a means to achieve improvement by the use of  shorter wavelength illumination on ultra-thinned SOI samples, a prototype system to analyze such devices, and examples of  using the visible light LVP system on SOI have been  described.  We demonstrate this method on advanced  technology node SOI devices, comparing the spatial  resolution and LVP signals achieved at visible wavelength  with a conventional, infrared LVP system.


ACKNOWLEDGEMENTS


Sandia National Laboratories is a multi-program laboratory  managed and operated by Sandia Corporation, a wholly  owned subsidiary of Lockheed Martin Corporation, for the  U.S. Department of Energy's National Nuclear Security  Administration under contract DE-AC04-94AL85000.


[1] Kindereit et al., “Quantitative Investigation of Laser


Beam Modulation in Electrically Active Devices as Used


in Laser Voltage Probing”, IEEE Transactions on Device


and Materials Reliability, Vol. 7, No. 1, March 2007.


[2] Ravikumar, V. K. et al., “Laser Voltage Probing in     Failure Analysis of Advanced Integrated Circuits on


SOI”, Physical and Failure Analysis of Integrated Circuits


(2012) 1-4.


[3] Tan et al., “VIS-NIR LED Illumination in Backside


Circuit Edit and Optical Probing Applications”,


International Symposium for Testing and Failure


Analysis, (2012) 505-508.


[4]  Ng et al., “Laser Voltage Imaging: A new Perspective of


Laser Voltage Probing”, International Symposium for


Testing and Failure Analysis, (2010) 5-13.


[5]  PVEDUCATION.ORG – Optical Properties of Silicon


http://www.pveducation.org/pvcdrom/materials/opticalproperties-of-silicon


Introduction of spectral mapping through transmission grating, derivative  technique of photon emission


Thierry Parrassin, Sylvain Dudit, Michel Vallet


STMicroelectronics, 850 rue Jean Monnet, 38920 Crolles, France


thierry.parrassin@st.com, sylvain.dudit@st.com, michel.vallet@st.com


Antoine Reverdy


Sector Technologies, 2 avenue de Vignate, 38610 Gières, France   antoine.reverdy@sector-technologies.com


Hervé Deslandes


DCG Systems Inc., 3400 W Warren Avenue, Fremont CA 94538, USA  herve_deslandes@dcgsystems.com


By adding a transmission grating into the optical path of our  photon emission system and after calibration, we have  completed several failure analysis case studies. In some cases, additional information on the emission sites is provided, as  well as understanding of the behavior of transistors that are  associated to the fail site. The main application of the setup is  used for finding and differentiating easily related emission  spots without advance knowledge in light emission  mechanisms in integrated circuits.


Photon emission microscopy is widely used in Integrated  Circuit (IC) failure analysis to find defects, but in acquisitions  showing a sea of emission spots it is sometimes hard to locate  the faulty one of interest. Past experiences have demonstrated  a potential benefit in analyzing the spectral composition of the  emitting source. The photon emission from ICs has been  analyzed through light intensity [1] or through the light  spectra sampled by optical filters [2], [3], [4], by prism [5], [6] or transmission grating [7], with the objective to understand  the photon-emission mechanisms or to find defects.


Using a transmission grating demonstrates an extension to  photon emission microscopy in order to provide more insights  to emission spots in the field of view. This will allow the  faulty transistor to be recognized easily and quickly in a sea of  spots.


The transmission grating introduced in the optical path of our  Meridian IV system allows the spectral display of each  emission spot in the field of view. From a typical emission  image (Figure 1 left) we do not have a way to differentiate the  signatures of the spots. If now a diffraction grating is  introduced we get the same image as the one before but with


addition of the spectral response of each individual spot (Figure 1 right)


Figure 1: Left: typical 20x photon emission acquisition  obtained on CMOS40nm. Right: same field of view while  using the diffraction grating.


It is also possible to finely analyze the spectral response of  each spot with the information clarified by a virtual crosssection or profile of the diffraction pattern. Our goal is to use  the spectral analysis of the photon emission spots for fast  recognition and localization of defects. The focus of this paper  is mainly on an approximate analysis of the spectra on real  cases instead of doing the fine analysis of the spectral profiles.


In a first part, we detail the setup of our spectrometer: why we  chose a transmission grating, how we lay out the installation  and how we calibrate it.


Then we validate the spectrometer on known ICs including  standalone devices such as MOSFETs, resistors, and standard  cells in order to learn basic spectral signatures that we can  compare to real cases.


The main part of this paper goes through the results obtained  on real case analysis in various silicon technology nodes  showing multiple photon emission spots that can be quickly  differentiated thanks to the diffraction grating.


Finally we discuss the benefit of using the spectral analysis in  the failure analysis flow before concluding.


Spectrometer Setup


Choice of the spectrometer


The choice of a transmission grating was mainly motivated by  the specifications of our Meridian IV system. We wanted an  installation with proper resolution that can be set up easily in  the optical path of the Meridian and fast to use. Spectral  profiles have to be displayed and analyzed on our 1024x1024  pixel InGaAs camera with good enough resolution.


According to these specifications, a spectrometer based on an  optical filter wheel acquires discrete measurements and needs  several acquisitions to get a full spectral analysis: resolution is  low and acquisitions are long. A spectrometer based on a  prism has good resolution with continuous spectral  acquisition, it needs only one acquisition to get the results, but  a prism is difficult to insert in the optical path of the  equipment due to the volume taken by it. Further, a prism does  not show the original emission position and the spectra at the  same time.


The transmission grating is the best compromise for Meridian  because the device is flat, easy to insert into the optical path, and provides registration between the original emission spots  and the acquisitions, which are continuous spectral  distributions directly diffracted onto the InGaAs camera.


Dimensioning


The grating specifications as well as its location are chosen  based on the user’s desired dispersion. Choosing the correct  grating depends on several parameters.


Some parameters are linked to the material: the grating has to  be used in the range of the spectral response of the InGaAs  camera; the substrate of the grating must have the maximum  transmission in the used spectral range and has to be  transparent in the near infrared domain. A grating with a  blazed angle is the best choice to increase the diffraction  efficiency into one order.


Other parameters are linked to the dimensioning:


There is a compromise between spectral resolution and signal  strength. It depends on the distance of the grating to the  InGaAs camera, the azimuthal angle of the grating with  respect to the camera coordinates, the resolution of spectral  acquisition we need, and the sensitivity we need. Indeed, a  grating with a low spatial frequency allows a good sensitivity, reducing the acquisition time but at the cost of the resolution. Conversely, a high spatial frequency grating will increase the  resolution but the acquisition time will take longer.


The specifications of the grating are solved thanks to the  transmission diffraction grating equation


mλ =a.(sinθm –sini)                   (I)


where m is the order of the diffraction peak, λ is the  wavelength, a is the grating period or the distance between 2


slits, i is the angle of the incident beam of light to the grating, θm is the angle of diffraction at the m order.


Figure 2: Transmission grating and diffracted orders inserted  in the optical path of the system.


By using some trigonometry formulae, it is possible to  simulate and to solve the grating parameters like the grating to  camera distance or the spectral spreading, expressed in camera  pixels or directly in wavelength after calibration.


Typically with the grating we have selected, we get the full  spectrum (≈800nm-1600nm) on our LN2 cooled InGaAs  camera over the range of about 300 pixels, giving a resolution  of about 2.2nm of wavelength per pixel. We have to pay  attention to use the first order of the blaze angle of the  diffracted spectrum since we will get more intensity compared  to the opposite diffracted order. The 0 order (Figure 2) is the  integrated emission, similar to a standard emission image and  can be used as the reference point for calibrating the  spectrometer. A spectral mapping image will contain all the  orders but we typically use only the 0 order and the first order (


Figure 7 shows the SEM images of the copper wirebonds after  pre-laser decapsulation and after complete (laser and  chemical) decapsulation, at laser focus depth of (z-1) mm.


Figure 7: SEM images of copper wirebonds (a) after pre-laser  decapsulation, (b) after complete (laser and chemical)


decapsulation and (c) diameter measurement of copper wire  after complete decapsulation, at laser focus depth of (z-1) mm (defocused)


It can be observed from Fig. 7(a) that when the depth of the  laser is defocused at (z-1) mm, the laser does not cause much  damage in the form of burn marks on the surface of the copper  wirebonds due to much lower laser intensity with an increase  in laser beam spot size. After complete decapsulation, although pits still result on the surface of the copper wirebonds (Fig. 7(b)), the damage to the palladium coated copper  wirebonds is reduced significantly. The copper wirebonds are  no longer deformed and shrinkage in wire diameter is minimal. The overview optical image of the TQFP after complete  decapsulation is shown in Fig. 8.


Figure 8: Optical image of TQFP after complete (laser and


chemical) decapsulation, at laser focus depth of (z-1) mm


(defocused)


Table 2 summarizes the measured average diameters of the  copper wirebonds after pre-laser decapsulation, and after  complete decapsulation, as well as the average percentage  reduction in wire diameters after complete decapsulation, at  the various laser focus depths studied.


Table 2: Average diameters of copper wirebonds after prelaser decapsulation and complete (laser and chemical) decapsulation


Laser  focus  depth,


(mm)


Average


copper


wirebond  diameter after


pre-laser


decapsulation (µm)


Average copper


wirebond


diameter after


complete


decapsulation


(laser and


chemical) (µm)


percentage  reduction in  wire diameter  after complete  decapsulation (%)


At  focus


21.7 ± 2


0 – 14.7


Severely


damaged,


broken and  debonded wires


(z-0.5)


14.5 – 18.5


24.0


(z-1)


20.4 – 22.0


2.30


From the results, it can be observed that carrying out pre-laser  decapsulation at a defocused depth of (z-1) mm preserves the  integrity of copper wirebonds, compared to (z-0.5) mm or at  focus depth which resulted in broken and debonded copper  wirebonds.


When the laser beam is focused, the spot size is reduced, resulting in greater laser intensity on the surface of the copper  wirebonds. However, with a defocused laser beam, the spot  size is increased, thus the laser intensity on the surface of the  copper wirebonds is lowered, and damage to the copper  wirebonds is minimized. Although the average copper  wirebonds diameter after pre-laser decapsulation is similar for  laser focus depths at focus, (z-0.5) mm and (z-1) mm, the  damage to the surface of the copper wirebonds is more at a  fully focused depth, compared to defocused depth. The  palladium protection layer will also be less at focused laser  depth. Subsequently, during chemical decapsulation, this  damage will be even greater, as the mixed acids can easily  access and etch the already damaged copper wires from the  pre-laser decapsulation step.


The pre-laser decapsulation step in the decapsulation of copper  wirebonded devices is crucial in preserving the integrity of  copper wirebonds. If copper wirebonds are already severely  damaged at this step, subsequent chemical decapsulation will  exacerbate the damage. It is recommended to carry out prelaser decapsulation with a defocused laser depth to reduce the  amount of damage on copper wires.


[1]


S. W. Ng, H. B. Zhang, K. N. Liew, W. Lee, and R. D. Lin, "Copper wirebond package decapsulation


technique using mixed acid chemistry," in 19th IEEE  International Symposium on the Physical and Failure  Analysis of Integrated Circuits (IPFA), 2012, p. 5 pp.


[2]


H. Wu, A. Chiang, D. Le, and W. Pratchayakun, "Failure Analysis on Power Trench MOSFET


Devices with Copper Wire Bonds," in 37th


International Symposium for Testing and Failure  Analysis (ISTFA), 2011, pp. 223-229.


[3]


M. J. Lefevre, F. Beauquis, J. Yang, M. Obein, P.


Gounet, and S. Barberan, "New method for


decapsulation of copper wire devices using LASER  and sub-ambient temperature chemical etch," in IEEE  13th Electronics Packaging Technology Conference (EPTC), 2011, pp. 769-773.


[4]


Y. H. Chen, M. Hsiao, and C. E. Tseng, "The


properties comparison between Au and Cu wires


bond in DRAM component," in 18th IEEE


International Symposium on the Physical and Failure  Analysis of Integrated Circuits (IPFA), 2011, pp.


207-210.


[5]


J. EKlein and L. Copeland, "Decapsulation of copper  bonded plastic encapsulated integrated circuits


utilizing laser ablation and mixed acid chemistry," in


36th International Symposium for Testing and Failure  Analysis (ISTFA), 2010, pp. 133-136.


[6]


K. D. Staller, "Low temperature plasma decapsulation  of copper-wire-bonded and exposed copper


metallization devices," in 36th International


Symposium for Testing and Failure Analysis (ISTFA), 2010, pp. 127-132.


[7]


S. Murali and N. Srikanth, "Acid decapsulation of


epoxy molded IC packages with copper wire bonds,"


IEEE Transactions on Electronics Packaging  Manufacturing, vol. 29, pp. 179-183, 2006.


"Manual: Machine Design and Description of


Functions," ed: Baublys Control Laser, 2007, p. 3.


[9]


R. Paschotta, Optical intensity, Gaussian beams. RP  Photonics. Encyclopedia of Laser Physics and


Technology vol. 2, N-Z: Wiley-VCH, 2008.


[10] A. Laboratories. (2014). Laser beam divergence and  spot size. Available:


http://amrita.vlab.co.in/?sub=1&brch=189&sim=342&cnt=1


[11] P. E. B. Paranal, "Localized die metallization damage  induced during laser-marking of a semiconductor


package," in 33rd International Symposium for


Testing and Failure Analysis (ISTFA), 2007, pp. 226-230.


A Sample Preparation on Decapsulation Methodology for Effective Failure  Analysis on Thin Small Leadless (TSLP) Flip Chip Package with Copper Pillar (CuP) Bump Interconnect Technology


Gwee Hoon Yen, Ng Kiong Kay


Infineon Technologies, Free Trade Zone, Batu Berendam, 75350 Melaka, Malaysia


hoonyen.gwee@infineon.com; kiongkay.ng@infineon.com, phone; +606-2873715, fax: +606-2325069


Today, failure analysis involving flip chip [1] with copper  pillar bump packaging technologies would be the major  challenges faced by analysts. Most often, handling on the chips  after destructive chemical decapsulation is extremely critical  as there are several failure analysis steps to be continued such  as chip level fault localization, chip micro probing for fault  isolation, parallel lapping [2, 3, 4] and passive voltage  contrast. Therefore, quality of sample preparation is critical. This paper discussed and demonstrated a quick, reliable and  cost effective methodology to decapsulate the thin small  leadless (TSLP) flip chip package with copper pillar (CuP) bump interconnect technology.


The crux of today’s packaging innovations continues to be  driven by silicon node reduction and its corresponding


die shrinking, coupled with increased functionality and higher  bandwidth requirements. Smart phones and tablets comprise  two of the fastest moving, highest volume, and most  competitive markets in the world with form, fit and function  evolving at an unprecedented rate. Consequently, the necessity  of managing costs, design complexity, and manufacturability  results in continual innovation to meet the dynamic demands  of the market. The semiconductor manufacturing responds to  this challenge with similar innovation in the development of  new packaging methods and with the speedy assembly of  copper pillar bump flip chip packaging technologies as  illustrate in figure 1.


It is not only in high volume production for mobile electronics, but is also a transformative technology for next generation flip  chip interconnects which offers advantages in many designs  while meeting current and future requirements. It is an  excellent interconnects choice for applications such as  transceivers, embedded processors, application processors, power management, baseband and ASICs where some  combination of ROHS/Green compliance, low cost and electro  migration performance are required.


Figure 1: Overall views of SEM image on flip chip with  copper pillar bump packaged from backend manufacturing  after die attach process. Die surface facing downwards.


Meanwhile, failure analysis dealing with such packaging  technologies is getting more and more challenging. Traditional  package chemical decapsulation method, window  decapsulation no longer works as the size of the silicon chip is  almost similar to the package dimension. Total decapsulation  by immersed the whole device into fresh fuming nitric acid (HNO3) will end up with left only the bare die. In other words, handling the silicon bare die is risky and it could be accidently  lost. Therefore, a sample preparation on decapsulation  methodology has being proposed to overcome the highlighted  issues associated with other, traditional package decapsulation  methods.


Sample Preparation and Decapsulation Method


A DPDT (Dual-Pole/ Double-Throw) differential RF switch  used in smart phones are assembled under Thin Small Leadless (TSLP) flip chip package with copper pillar bump as  interconnections. The silicon chip consists of ten pads and the  pad itself was connected to external lead using copper pillar  bump. This device was used as a test device (DUT) to  demonstrate the proposed sample preparation on decapsulation  method. Low power optical image illustrated the top package


view while bottom and side views were illustrated by drawing (figure 2).


The proposed method required scrapped silicon wafers in  pieces form that used as a platform to support the devices as  illustrated in figure 3. Epoxy Bond 110 was used to bond the  product onto the piece of silicon wafer. The two-part epoxy  mixture was prepared according to the manufacturer’s  recommendations (figure 4).


(2a)


(2b)


(2c)


Figure 2. Low power optical microscope image and package  drawing on device under test (DUT): (2a) Package top view; (2b) Package bottom view; (2c) Package cross sectional side  view.


Figure 3: Optical image showing the scrapped silicon wafer  in square shape after cut with diamond pen.


(4a)


External Pad


Silicon


Resin


Hardener


(4b)


Figure 4. (4a) Epoxy Bond 110 from Allied is a hard, fast  curing and chemical resistant epoxy adhesive; (4b) Two part  formula were mixed 10 (10 drops from Resin) to 1 (1 drop  from Hardener) using mixing cup. Wood stick was used to  stir the chemical to ensure two part formula completely  mixed.


At this stage, the DUT can be subjected to laser ablation to  remove the mold compound until the silicon chip backside is  visible as illustrate in figure 5. After that, the cotton swab was  used to distribute epoxy bond evenly on the silicon wafer as  shown in figure 6. Figure 7 showed that the DUT was then  placed on the epoxy bond to bond the silicon chip backside to  silicon.


Finally, the epoxy of DUT assembly was cured at 150 °C for 5  minutes as shown in figure 8. It could notice that the epoxy  became dry and changed to dark brown color after curing. The  DUT was firmly attached on silicon and the bonding force was  strong, and chemically resistant. Subsequent heating at high  temperature did not melt the epoxy and there was practically  no risk of silicon chip drop off after subjected to chemical  decapsulation [5].


Figure 9 shows that the DUT assembly is now immersed into  the 100% fuming nitric acid to remove the mold compound.  Once it is completely removed, the DUT is then rinsed with  acetone for cleaning. Figures 9(b) illustrates the DUT  condition after removing the mold compound left over the  pillar and external pad still connected to silicon die.   Then  followed by immersed again, the DUT was put into 65% nitric  acid to remove the external pad and copper pillar as illustrate  in figure 10.


(5a)


(5b)


Figure 5. (5a) Cross section schematic showing before and  after laser ablation; (5b) Optical image of DUT after mold  compound removal.


Figure 6. Optical image showing a tiny drop of epoxy bond  distribute evenly on silicon.


(7a)


Epoxy Bond 110 (Mixture of part A and B) Mixing Cup


Wood Stick


Si Chip Backside


Mold Compound


Mixture of Epoxy Bond 110


(7b)


(7c)


Figure 7. (7a-7b) Cross section and optical view showing  DUT bond to silicon; (7c) Overall view of DUT assembly on  silicon.


Figure 8. Optical image showing epoxy bond has changed to  dark brown colour after 150 °C cured.


(9a)


(9b)


Figure 9. (9a) Optical image showing DUT assembly  immersed into 100% fuming nitric acid to remove the mold  compound; (9b) Cross sectional view showing DUT assembly  condition after removing the mold compound.


Epoxy Bond


CuP Flip Chip


Tweezer


Hot Plate


Nitric Acid (HNO3) 100%


DUT  assembly


(10a)


(10b)


Figure 10. (10a) Optical image showing DUT assembly  immersed into 65% nitric acid to etch away the external pad  and copper pillar; (10b) Cross sectional view showing DUT  assembly has been completely chemical decapsulated.


It can be noticed that external pad and copper pillar are  completely etched away, leaving a clean and zero handling risk  silicon chip for next step failure analysis. Chemical  decapsulation process is considered complete at this step. The  silicon chip is then rinsed with acetone for final cleaning  follow by blowing with air gun to dry the chip surface. Figure  11 shows overview of unique and innovative methodology to  decapsulate Thin Small Leadless (TSLP) flip chip packages  with CuP bump technology.


Figure 11. Optical image showing final result of DUT  assembly after chemical etching steps completed.


A method using silicon combined with epoxy bond 110 from  Allied to decapsulate the Thin Small Leadless Package (TSLP) with copper pillar (CuP) bump technology flip chip packaged  was presented. The proposed decapsulation methodology  enables the excellent handling mechanism to allow failure  analysis to be performed more efficiently and reliably  especially on CuP flip chip packaged IC devices. Besides, it  eliminates the handling risk that may induce externally to the  chip that could cause the chip to fatal and it provides the  flexibility and possibility to offer various type of failure  analysis step to be performed.


[1] J. Lau, “Flip Chip Technologies”, McGraw-Hill, 1996.


[2] H.Y. Gwee, K.K. Ng, “Alternative Sample Preparation  Technique for Die Level Parallel Lapping Analysis,” Proc  39th Int’l Symp for Testing and Failure Analysis, Proceeding, 576-581.


[3] Wills, K.S. “Planar Deprocessing of Advanced VLSI  Decices,” Proc 32nd Int’l Symp for Testing and Failure  Analysis, Austin, Texas, November 2006, pp. 393-397.


[4] Moor, T., “Single Die Hands Free Layer-by-Layer  Mechanical Deprocessing for Failure Analysis or Reverse  Engineering,” Proc 34th Int’l Symp for Testing and  Failure Analysis, Portland, Oregon, November 2008, pp. 363-367.


[5] J. E. Klein and L. Copeland, “Decapsulation of Copper  Bonded Encapsulated Integrated Circuits Utilizing Laser  Ablation and Mixed Acid Chemistry,” 2010 ISTFA, pp. 133-136


Nitric Acid 65% (HNO3)


Chip


Improved Lock-in Phase Mapping of Modulated Reflectance with SIL


Zhongling Qian*, Christof Brillert and Christian Burmer   Infineon Technologies AG, Munich, Germany


The application of lockin phase mapping of modulated  reflectance with SIL is discussed in detail, particularly the socalled ghost mapping signal in STI neighboring to active  regions. The different lockin phase between active regions and  ghost regions showed clearly that both of them have different  physical origins. The phase transition between active regions  provides an enhancement of spatial resolution for defect  localization in scan cell and sub blocks.


With shrinking feature size of VLSI circuits and decreasing  power supply voltage, the traditional global localization tools  in failure analysis (FA), such as photon emission microscopy (PEM) and thermal laser stimulation (TLS), have met a great  challenge [1-4]. The lockin assisted TLS techniques, such as  lockin TIVA, LIA-SDL and mixing frequency TLS etc., extend its usage range in FA daily jobs [5-8]. Lockin  technique has also been successfully applied into dynamical  PEM for global localization of failed FFs in a broken scan  chain and to enhance weak emission spots correlated to a  single power domain [9].


The recent application of lockin technique is found in the FET  activity mapping technique called laser modulation mapping (LMM), or modulated reflectance mapping (MRM), or  frequency mapping (FM) [10-18]. Its mechanisms include  electro-optical effects, and thermo-optical effects generated by  modulated electrical field [10-14].  Absorption and refraction  due to free carriers are regarded as the main effect with a  detection laser at 1319nm [10]. The drawback of MR mapping  using real-time spectrum analyzer is that the detection  frequency must be tuned accurately to obtain a higher SNR.  It  makes it very difficult to apply such a technique in the device  whose inner clock frequency is not required to be very stable  and with a larger jitter. However, in lock-in technique, the  external reference signal can follow such a change of the  operating frequency rapidly. Lock-in phase mapping of  modulated reflectance demonstrated its unique advantage in  comparison with amplitude particularly in dynamically  operating mixed signal or power IC devices [19].


In FA of advanced IC devices, the solid immersion lens (SIL) provides an enhanced spatial resolution and plays an


important role for a fine localization in order to find the root  cause rapidly.  With its help, the detailed MRM can be  realized in a single FF or a logic sub-block for a finer  localization at transistor level. To our knowledge, there is still  no report on the lock-in phase MRM by using SIL directly. The usage of vector analyzer instead of lockin amplifier was  reported to obtain the phase mapping of single scan cell but  with a limit of a rough phase resolution of 90° [18].


It is well known that the MR signal is extremely weak in the  order between 40 and 70ppm at a bias of 1.2V [10-14]. In a  typical inverter, pFET and nFET showed opposite MR phase, i.e. 180° phase difference, but their MR amplitudes own a  relatively small difference. Such a huge phase difference can  be used to enhance the spatial resolution in a FF or small subblock to obtain a fine MRM pattern at transistor level, although laser spot size may cover two or more FETs.


Setup


The self-made Lockin MR setup is based on a modulated  reflectance mapping (MRM) system in combination with a  high frequency lock-in amplifier. The thermal laser (1340nm) is used as a detection optical source with a maximum output  power of 20mW.  The best lateral and axial spatial resolution  can be realized with a GaAs solid immersion lens (NA=2.63, 350x). Such a SIL has also a higher tolerance to silicon die  thickness: about 50µm.


Fig.1. The Lock-in amplitude and phase signal on a reference  device depend on the detection laser power.


The system shows a very stable result in both amplitude and  phase at point mode with laser power larger than 1mW, shown  in Fig.1.  The MR amplitude shows a linear dependence on  the laser power, so we can exclude any nonlinear optical  effects, such as two-photon absorption (TPA) etc.  The phase  is very stable with the laser power larger than 1mW.  Its  accuracy is about ±1°.


Fig.2. (Top) Pattern image – darker contrast at the lower  right corner. (Middle) Lock-in MR amplitude pseudo color  image overlaid with pattern image - weaker signal at the  lower right corner. (Bottom) Lock-in MR phase pseudo color  image overlaid with pattern image – homogenous in the whole  image, although there is a lower contrast of laser reflection at  the lower right corner.


In order to compare both the amplitude and phase mapping  techniques of modulated reflectance clearly, one device with  full scan design in 110nm technology was used. In the test, the  bypass mode of scan chain was used in order to activate every


scan chain separately.  The test clock is 20MHz. The scan  input is “1010”.  The pattern was modified for looped run.


Homogenous MR phase mapping


Just shown in [19], the advantage of lockin phase mapping is  that it is independent of the reflection intensity of detection  laser.  Variation in local reflectivity or inhomogeneous  lighting is very apparent to be excluded from the formula  below:


θ= arctan(Y/X)


where θ is the phase of the MR signal, and X and Y are its inphase and out-of-phase components. Both X and Y  components of the MR signal are proportional to the reflection  intensity of a detection laser. The DC reflectivity R shows a  very large difference depending on materials (Cu, Al, Si, Poly  and so on), layer thickness and doping dose in an advanced IC  device. This difference in reflectivity prevents normal  amplitude mapping, using spectrometer or lockin amplifier, from showing the real MR signal. The real MR signal can be  obtained only by using ∆R/R, where ∆R is the reflectivity  variation.


In Fig.2, inhomogeneous pattern image (top) was observed  due to inhomogeneous lighting with SIL lens, particularly at  the lower right corner. It makes the corresponding lock-in  amplitude mapping (middle) inhomogeneous too. But that is  not the case in the phase mapping (bottom).  The phase  mapping signal is strong and homogeneous throughout the  image.  Just as shown in Fig.1, the incident laser power must  be larger than1mW in order to obtain a stable phase signal.


Fig.3. The overlay image of lock-in MR phase (upper) and  layout (lower, only poly layer and FF blocks) of FFs in a scan  chain.


Fine flip-flop/inverter pattern in MR phase mapping


The fine details of a lock-in phase mapping in a single flipflop (FF) block can also be detected with SIL, as shown in Fig


3. The clear phase variation image in every nFET and pFET of  one reference FF cell can be used to determine rapidly the  defective FET if the affected FF doesn’t work well. In Fig.3, FF460 and FF484 showed the same phase mapping pattern. On one side, both of them are the identical FF type with the  same orientation in the layout (below in Fig.3). On the other  hand, it indicates also that they work synchronously with the  same scan clock during scan chain test. It is not the case at FF  477 since it is out of phase due to “0101” scan input pattern.


The lockin phase mapping at the bottom of Fig.4 shows  clearly 4 different phases of MRM signals in color. The  inverter chain showed clearly 180° difference phase at n and p  FETs in the same stage, shown as the yellow/brown pair  colors on the left side of the bottom image. The variation  between two inverter stages was also observed to be  correlated with the time delay between them, shown as  yellow/light yellow contrast between left and right sides of the  bottom image. It is clear that on the middle of Fig.4, the MRM  amplitude image shows no information about time delay and  phase difference not only in the same inverter stage and also  in the following inverters.


Fig. 4: Typical MRM result of inverter chain in SIL.  Top: pattern image, Middle: overlay of Lock-in amplitude mapping  and Bottom: overlay of lock-in phase mapping. The clear  phase variation pattern was observed in the lock-in phase MR  image.


Enhanced spatial resolution in MR phase mapping


The sharpest edge of lock-in MR phase image is observed on  such sites where the phase transition happens. The comparison  of the line profiles in the optical pattern image, MRM  amplitude and phase images in Fig.5 clearly confirms it.  This  can be helpful for recognizing fine structure spatially, particularly in advanced technologies. The clear pattern in the  phase image will also provide precise localization allowing  identification of a single defective FET in FFs or sub-blocks.


Fig.5 The corresponding line profiles (red guiding lines) are  shown through two inverters in pattern (upper), lockin MR  amplitude mapping (middle) and lockin MR phase mapping (lower).  Grey images showed clearly the sharpest edge in  lock-in phase image where phase transition happens.


“Ghost” signal in modulated reflectance mapping


Fig. 6 Typical MRM signal using real-time spectrum analyzer  in an inverter chain. Red arrows point to the so-called ghost  signal. The inset showed the probing result at such a ghost  point (yellow: input signal).


The ghost phenomena was at first observed in the normal  MRM system using real-time spectrum analyzer in a test 90nm  bypass inverter chain running at 50MHz. The normal MR  signal was observed in active regions in both n- and p- FETs  in an inverter, just as expected to be the contribution from free  carriers. However, stronger MRM signals were also observed


at neighboring STI regions around the active region (red  arrows in Fig. 6).   The probing result on one of such ghost  points confirmed a stable periodic signal; see the inset in Fig.


It is difficult to understand the origins of such ghost signals, since they are not located in active regions. It is worth  pointing out that all these spots showed a larger DC reflection  from polys and metal layers on the top of STI. All of them  belong to the boundaries of source regions to STI.


Such a ghost phenomenon was not only observed in the test  inverter chain but also in the product ICs. Since the lock-in  method can strongly reduce uncorrelated signal, so the lockin  MRM was used to study such ghost points.


Figure 3). An image cross section along the diffraction axis  will give the raw emission spectrum as displayed by


Figure 4.


Figure 3: Detail of the spectral mapping image: emission and  spectrum of a NMOS in saturation in blue, forward biased  diode in red.


Figure 4: Profile of the red highlight of Figure3.


Calibration


The calibration provides conversion of pixels of the InGaAs  camera into wavelength. We used a monochromator in order  to acquire the calibrated spectra at different wavelengths (Figure 5). Then we measure on each profile the distance in  pixel of the first order from the reference emission spot (Figure 6).


Figure 5: Spectral mapping obtained during calibration. Left  is the zero order, right is the diffracted 1st order spectra for  each wavelength.


Figure 6: Profiles of all 1st order spectral mapping in pixels. Distance for each wavelength measured (zero order has been  cropped) leading to the calibration curve for the pixel to  wavelength conversion.


The model obtained by the transmission diffraction grating  equation is finally fitted with the resulting wavelength versus  pixel calibration curve. Solving the fit by the mean square  error reduction methodology gives a very good matching with  a correlation score of  0,9998 .


Validation on stand-alone devices


This paper is mainly based on the spectral mapping and the  shapes of the signatures. The calibration of the spectrometer is  only done for the X-axis (wavelength) and not done in  amplitude. In practice we are doing relative comparison  between the spectra of different spots so the full calibration is  not required. This might be a future improvement.


The validation of the spectrometer installation on known  devices allows learning basic spectral signatures that we will  be able to recognize easily in real cases. Results obtained are  on various devices such as stand-alone MOSFETs, resistance, diodes and also on controlled defects such as gate breakdown, electromigration and bridge defects drawn in the design.


Figure 7 below shows an example of a cell which can emulate  various photon emission mechanisms: impact ionization when  the NMOS is saturated, photon emission when the gate is in  an intermediate state or when the MOS is commutating, and  light emission when the diodes are forward biased or reverse  biased. It is also possible to over stress the gate leading to  tunneling emission or gate oxide breakdown.


Figure 7: Device included in a chip dedicated for failure  analysis: stand-alone NMOS with protection diodes on the  gate net. It allows the emulation of various photon-emission  mechanisms.


The spectral mapping of the device acquired with the Solid  Immersion Lens (SIL) 220x objective is shown in Figure 8.


2 NMOS devices as described in Figure 7 are biased to  emulate different emission mechanisms in real FA cases. On  the first device, we set the NMOS in saturation and one of the  diodes is forward biased (yellow and red highlight). In the 2nd  device we set the gate at Vdd/2 for emulating an intermediate  state. It is interesting to notice that a switching NMOS gives  the same spectral mapping as the NMOS set in this partiallyon state.


The used diffraction grating is very dispersive and the spectral  mapping can sometimes diffract outside the camera field of  view. In order to gain some pixels, we can set the grating with  a rotation of 45°. Another advantage is the possibility to  separate 2 spectral signatures by rotating the grating if we  acquire overlaid signatures due to an alignment on the same  axis of two emission spots.


Figure 8: Spectral mapping showing different spectral  signatures depending on the photon emission mechanism. 3  mechanisms are highlighted: the diode in forward bias gives a ‘water drop shape’ signature, the saturated NMOS gives a ‘comet shape’ and the NMOS with the gate in intermediate  state gives a flat spectrum.


We performed several trials on devices designed in different  technologies and emulated with various electrical conditions. Generally, the spectral shape of tested devices is strongly  dependent on the electrical conditions and slightly on the  technology node (this point will be characterized in a further  work on a large range of technologies). Finally we were able  to categorize some generic spectral shapes (Figure 9) and  spectral profiles (Figure 10) related to specific photon  emission mechanism or defects.


Figure 9: Spectral mapping obtained on specific photon  emission mechanisms, these mappings seem to be generic  more to the emission mechanism than the technology node (assumption to be characterized)


Figure 10: Profiles measurement of the basic shapes  described in Figure 9 with forward diode, NMOS with the  gate in intermediate state and NMOS in saturation measured  in Figure 8. Thermal measurement gathered from acquisition  seen in Figure 11.  Profiles are normalized in order to focus  on the position of the maximum of intensity.


The shape of the spectral mapping image is similar between  the thermal emission and the NMOS in saturation. The  difference is that the thermal emission is apparently  exponential with increasing wavelengths.


Real case analysis


CMOS40 thermal characterization of a 12 Ohms copper  resistance


The first real case analysis is a characterization for  temperature model. The device is a copper resistance (100 x 1 µm) designed in metal1 layer. 80mA is applied  through this resistance in order to reach a temperature limit  where the black body radiation can be captured in the range of  our InGaAs camera (≈900nm-1600nm). The light emitted by  the resistance is captured through the backside of the circuit  with the 220x SIL objective.


The original EMMI signature shows a homogenous intensity  distribution along the resistance except for the extremities (Figure 11, left). The spectral mapping obtained with the  grating is translating the intensity into wavelength and reveals  that the temperature is not homogenous (Figure 11, right). A  hot area at the center of the resistance and some cold spots are  observed. A virtual cross-section of the spectral mapping, which is useful for fine analysis, shows the difference in the  captured black body radiation along the resistance (Figure 12).


Figure 11: Left, Backside illuminated image of the copper  resistance overlaid with emission, using 220x SIL.


Right: spectral mapping diffracted with the grating. Original  EMMI shows homogenous intensity while the spectral  mapping reveals some hotter area (plot3) and colder points (plot 4).


Figure 12: Profile of the spectral mapping (black body  radiation) obtained in


Figure 11, showing plot1 colder than plot3.


This analysis is still in progress in order to understand the  source of the cold spots revealed by the grating. Ageing stress  is now being applied in order to observe drifts in the spectral  mapping. One of the hypotheses of the cold spots is linked to  the grain texture of the copper resistance and will be analyzed  later.


The root cause of the cold spots is outside the scope of this  paper, where we focus more on the feasibility to perform the  characterization of temperature distribution, expressed in  wavelength with a very good resolution (InGaAs camera with  220x SIL) which is not observable in EMMI without the  diffraction grating.


CMOS28nm Bridge defect on metal 3 layer


This case study has been already presented using techniques  based on the laser reflection and especially Thermal  Frequency Imaging [8]. We were interested to see if the  spectral mapping technique can work also on this case for the  defect localization.


The defect is a bridge between two nets in metal3 due to an  OPC issue (


Figure 13).


Figure 13: SEM image of deprocessed device (down to  metal3) showing the bridge defect.


The failure mechanism induces a leakage between the nets if  the current flows from VDD, through the PMOS1 of net1, then through the bridge, then through the NMOS2 of net2 and  finally to GND with IN1 at 0 and IN2 at 1 (Figure 14). In this  case analysis we focus more on the NMOS emission rather  than the PMOS because it is much easier to detect the NMOS  emission. When the resistance of the defect is very low, the  NMOS2 is in saturation and emits light. The NMOS of the  cells driven by the failing nets are also emitting light because  the voltage drop on the gates induced by the defect set the  driven transistors in intermediate tri-state.


Figure 14: Schematic of nets with the resistive bridge defect. NMOS2 emits light because it is saturated; NMOS3 and  NMOS4 emit light because the cells are in intermediate state.


According to the results obtained during the validation phase  on stand-alone devices, the diffraction grating is able to  differentiate the saturated NMOS (comet shape) with an  intermediate state NMOS (flat shape). As shown by Figure15  we can clearly distinguish a different unique spectral shape on  the spectral signatures (right side). The spectral mapping


combined with other techniques capable also to differentiate a  signature in a sea of spots, such as TFI, is a very powerful  combination to focus directly on the defect without the help of  the CAD. One can argue that the spectral mapping maybe not  necessary in this case because the original photon emission  spot of the saturated transistor related to the defect is brighter  than the other spots, but this is not always the case.


Figure 15: Left side: original photon emission (order 0). Right  side: 1st order spectral mapping revealing the saturated  NMOS (comet shape) related to the bridge defect versus the  consequence light emission from others NMOS in  intermediate state (flat shape).


CMOS40nm Poly bridge


The photon emission of the 2nd bridge defect case study was  performed in dynamic mode with a clock signal applied to the  failing path. In this case the brightest spot is not the one  related to the fail. Spectral mapping reveals 2 comet shapes  which correspond to the saturated NMOS related to the fail (Figure 16 and Figure 17). The other flat shape signatures are  emitted by the NMOS set in intermediate state due to the  defect (the 2 strongest spots) or by the gates commutating  because the acquisition was done with a clock applied to the  tested path. It is difficult to differentiate  MOS in intermediate  state from commutating MOS by the spectral mapping which  are almost the same. Only the intensity of the spots gives clues  about the light emission mechanism. Nevertheless, saturated  MOS are clearly differentiated thanks to the spectral signature.


Figure 16: Spectral mapping of a poly bridge defect. Saturated MOS (left arrows)  due to the bridge are identified  by their comet shape (circles) versus commutating or  intermediate state emissions which have flat shapes. The  spectral mapping can reveal the hidden spot highlighted by  the bottom arrow (in between 2 very bright ones) when the  contrast/brightness of the image is not well adjusted.


Figure 17: Same image as the previous one but in false color  with contrast/brightness adjustment showing the hidden spot.


Flash40nm Oxide breakdown


The next case deals with an overconsumption in a Flash  memory designed in Flash 40nm technology.


The original photon emission acquisition shows several spots  in a poly resistance area driven by high voltage (>5V) and  surrounded by active filler cells (Figure 18).


Figure 18: Layout of the poly resistor in red surrounded by  the active dummies in green.


In this area, there are no transistors, only resistance. So the  expected spectral signature of the EMMI acquisition is a  thermal one (comet shape), but the spectral mapping shows  spectra with water drop shaped signatures related to forward  biased diodes instead (Figure 19).


Figure 19: Spectral mapping in the resistor area, signatures  look like forward biased diodes.


The physical analysis explains the failure mechanism. The  FIB/SEM cross-section observation shows a DRM (Design  Rules Manual) violation with an active dummy touching the  poly resistor (Figure 20). The high voltage applied in the poly  resistor reaches the voltage breakdown limit of the oxide  interface and leads to the oxide breakdown. The parasitic  defect generated is a Poly/Si diode emitting in forward, as  captured by spectral mapping.


In this case, the spectral mapping enforces the reliability of the  fault diagnosis and allows understanding of the correct failure  mechanism.


Figure 20: Dummy active touching Poly resistance (DRM  issue). Oxide breakdown occurs when the breakdown voltage  is reached.


CMOS28nm short poly contact


The next analysis is a short poly contact found in the logic  glue of a CMOS28nm circuit. The original photon emission  acquired in static at nominal voltage (1.0V) shows a sea of  more than 50 spots (Figure 21).


Figure 21: Photon-emission acquired in the area of interest of  the short poly contact (using the SIL)


After the insertion of the grating in the optical path, the  spectral mapping highlights only 2 comet shapes  corresponding to the MOS corrupted by the defect (Figure  22). These signatures have been confirmed by the profile  measurements. This case is a very good example  demonstrating the best usage of the spectral mapping  application for finding quickly and easily the spots related to  the defect.


Figure 22: Spectral mapping. The 2 NMOS in saturation are  revealed with the grating rotated at 45° in order to avoid the  overlay of the signatures.


Finally the short poly contact was located and observed in  FIB/SEM X-section (Figure 23)


Figure 23. FIB/SEM cross section of the defect


CMOS28 FDSOI massive EOS


The last analysis is an example where the grating was not  useful to differentiate the EMMI spots in a sea of signatures. The spectral mapping result is a mix of comet shapes and flat  shapes which are not easily differentiable (Figure 24)


Figure 24: Sea of EMMI spots diffracted by the grating. The  result is a mix of not differentiable comet shapes and flat  shapes.


This analysis shows that the spectral mapping used for the  signature differentiation is not working on all cases and we  still need complementary techniques as laser mapping or  others to explain the failure mechanism and to localize the  defects.


In this case, a massive electrical over stress was observed in  FIB/SEM cross section (Figure 25). We were not able to find  the root cause of this massive destruction.


Figure 25: Massive EOS observed in FIB/SEM cross section


Advantages


The advantages of the transmission grating spectrometer have  been demonstrated throughout a few examples. It is easy to  use and provides additional information on the emission sites, without the CAD information. It sometimes can pinpoint  directly to the defect


Limitations


The 2 limitations of this spectrometer installation are the  spectral range detection and the resolution.


The main spectral range detection limitation is due to the  InGaAs camera used for the acquisitions which is sensitive  from 800nm to 1600nm. For light detection on silicon  technologies a solution with a CCD camera (visible to ~1µm  spectral range) coupled to a MCT camera (800nm to ~2500nm) greatly increases the spectral range that can be  acquired. Most of the acquisitions are performed through the  backside of the dice through a silicon thickness set at 100µm  in order to use the SIL 220x: the transmitted light through the  silicon is strongly attenuated for wavelengths below 800nm. In this case spectral mapping acquisitions works better from  the front side of the die if there is a direct access to the light  emitter or through an ultrathin silicon film sample preparation  from the backside.


The limitation due to the resolution is linked to the grating  parameters. The need of resolution depends on the application  of the spectrometer. If the objective is to differentiate an  abnormal emission in a sea of spots, a high resolution grating  with a high capability of diffraction is not mandatory. In this  case the analyst just wants to display a large number of  spectral signatures in the field of view of the camera. But for  fine analysis and profile characterization for mechanism of  light emission study, the highest resolution is mandatory.


In order to perform both spectral mapping and profiles  analysis, a good compromise is to use a set of different  gratings mounted on a wheel.


Our spectrometer installation is a convenient and  complementary tool that can be easily included in the failure  analysis work flow in order to improve the reliability of the  diagnosis and the fault localization.


The goal of this installation was to set up a system for  performing fast acquisitions that can be used by any  technician in our laboratory without advance knowledge on  photon emission mechanisms. In this way, good practice with  the spectrometer is to quickly target abnormal emission spots  related to the fail through a sea of emission spots.


It is also possible to analyze finely the profile of each spectral  signature in order to study the behavior of the photon  emission mechanisms. Light emission in silicon is dependent  on too many parameters such as technology node size, voltage  biasing, nature of defect, etc… Some studies of these  mechanisms have already been published [4, 6, 9, 10] but  have to be characterized for each new technology node. Nevertheless we were able to sort some basic spectral  mapping shapes such as forward diode signature (water drop  shape), saturated NMOS / thermal (comet shape) and  intermediate state or commutating NMOS (flat shape) that we  believe can be used for several technology modes.


The resolution of the spectral signature can be easily adjusted  using several gratings or by changing the distance to the  camera, but these operations need calibration in order to  analyze quantitatively the results. The calibration is not  mandatory for performing only spectral mapping.


Further work


Our next work will be the calibration in amplitude of the  system in order to try to perform quantitative thermal  measurement on the resistance characterized in the first  analysis case. Also we will study some basic light emission  mechanisms versus the technology node and electrical setup in  order to extrapolate signatures of photon emission microscopy  for the next technologies.


The authors would like to acknowledge and thank engineers  from DCG Systems for the prototyped mechanical support for  the grating which is compatible with the SIL 220x on the STCrolles Meridian IV system. Thanks also to Sector  Technologies engineers for the installation of the  spectrometer. Last, thanks to all contributors working on light  spectral analysis based on photon emission microscopy.


[1] A. Tosi, F. Stellari, A. Pigozzi, G. Marchesi, and F. Zappa, “Hot-carrier photoemission in scaled CMOS  technologies: a challenge for emission based testing and  diagnostics” proc IRPS 2006 , pp. 595-601.


[2] G. Faggion, P. Sardin, S. Dudit, M. Vallet, H. Deslandes, J.-P. Roux, H. Koike and T. Kuki, “Effect of IC  Geometry Shrink on Photon Emission Spectrum”, LSI  Testing Symposium Japan, 2007.


[3] U. Kindereit et al., “Near-infrared photon emission  spectroscopy trends in scaled SOI technologies”, Proc   Int’l Symp for Testing and Failure Analysis ISTFA, San  Jose, CA, 2012, pp. 128-134.


[4] J.Kölzer, C.Boit, A Dallmann, G. Deboy, J.Otto, D.Weinmann, “Quantitative emission microscopy”, Journal of Applied Physics, Volume71, R23, June 1992


[5] M. Rasras, I. DeWolf, H. Maes, “Spectroscopic  identification of light emitted from defects in silicon  devices”, Journal of Applied Physics, Volume89, Number1, January 2001


[6] A. Glowacki, C. Boit, P. Perdu and Y. Yokoyama, “Electron temperature - the parameter to be extracted  from backside spectral photon emission”, IEEE 2013, pp5B.6.1-6.7


[7] S. Rusu, S. Seidel, G. Woods, D. Grannes, H. Muljono, J. Rowlette, K Petrosky, “Backside infrared probing for  static voltage drop and dynamic timing measurements”, IEEE 2001, pp 276, 277, 454.


[8] T. Parrassin, E. Petit, G. Celi, Y. Mousseau, and S. Dudit, “Scan Chain Bridge Defect on a 28 nm Technology Node  Circuit, Localization Using Dynamic Power Supplies”, ISTFA 2012 poster session, p. 587


[9] Herzog M, Koch M, “Hot Carrier Light Emission from  Silicon Metal-Oxide-Semiconductor Devices”, Appl Phys  Lett, Vol 53, No 26, pg 2620-2622, 1988


[10]  SL Tan et al., “Near-Infrared Spectroscopic Photon  Emission Microscopy of 0.13 μm Silicon nMOSFETs and  pMOSFETs”, International Symposium on the Physical  and Failure Analysis, 2008


SAM assisted Contour Milling


Christian Hollerith, Bernd Krüger, Stefan Waginger, Doris Plabst,


Infineon Technologies, Neubiberg, Germany


christian.hollerith@infineon.com, Tel. +498923422785


Matthias Fritz


Kern Microtechnik, Eschenlohe, Germany


Contour milling by high precision CNC-milling offers the  possibility to delayer precisely into warped and tilted package  interfaces e.g. to expose the die backside. The needed data  about the warpage of the surface of interest is in this case  derived from SAM time of flight- measurements. The  combination of these two approaches solves emerging  challenges for backside preparation process.


Advanced package technology often includes very thin dies in  thin packages. The reason for this trend is better heat  conductivity and lower resistance for the package, which leads  to better performance of the whole device. But the thin  construction makes these packages prone to warpage. These  two effects lead to the fact that the warpage of the dies can  easily be in the same dimension as the thickness of the die. Backside preparation for electrical localization of these  devices therefore becomes more and more difficult. So, new  approaches are needed such as milling with electrical endpoint  detection as described in [1]. The current paper shows a  different approach. A SAM time-of-flight measurement is  used to determine interface warpage as shown e.g. in [2]. This  data is used as input for contour-conform CNC-milling. A  process-flow for this method is shown at figure 1.


Figure 1: Process Flow


CNC-Milling-Machine


To accomplish contour milling a KERN CNC milling  machine is used with spherical millers in the range of 100 µm  to 500 µm diameter for this purpose, see figure 2. The same  CNC-machine already showed very good results for circuit  modification application in packages [3]. This tool is specified  with a position accuracy and repeatability of less than 1 µm in  all 3 axis directions. The maximum rotational frequency is  40000 rpm. Vibration of the machine is very low, so that  mechanical damage to Silicon is avoided as good as possible. The milling machine is controlled by a Heidenhain TNC  426PB CNC-control that can be programmed by Heidenhain  compatible CNC code. It offers a serial connection to an  external PC. So the code can be generated offline and then  transferred to the CNC-machine for the desired milling  process.


Figure 2: KERN CNC Milling Machine


SAM-Tool


The SAM used in this work is a Sonoscan Gen5, which offers the possibility to save the A-scan into a binary  file, which is subsequent processed by a Matlab routine. The  SAM images are generated with a 230 MHz-transducer that  has a focal length of 0.25 inch. The usage of high frequency  transducers enables very good lateral resolution as well as a  very good resolution of the reflected echo which enables a  precise determination of the peak maximum.


Matlab-Software


The calculation of the warpage in the die area, the  correction of defective pixels in this measurement and the  generation of Heidenhain CNC code is done with the help of  Matlab routines. The warpage is calculated in a standalone  GUI, the post processing is currently done in scripts, but will  be also integrated in the GUI soon. The output of the Matlab  routines is a Heidenhain CNC-code file (*.h) that can be  transferred to the milling machine for the intended milling  process.


Device-Sample


As a test device to demonstrate the new approach, a  laminate based package was used. In this kind of package the  die below the Cu-heat sink is often extremely warped. This is  especially the case after stress tests like temperature cycling. The warpage can be in the same order as the die thickness. But  the higher the warpage of the die is the higher is the risk that  the sample is destroyed if prepared for backside preparation by  plan-parallel polishing. It will be shown that contour conform  milling can overcome this problem. At beginning of the  preparation of the device, the upper layers of the package are  removed by plan-parallel milling. In this state the warpage can  then be determined by SAM measurement and then these data  can be used to control the local milling process


SAM Warpage Measurement


SAM is a well-known method at semiconductor industry, as it  is highly important to detect interface delaminations [4]. At  standard SAM measurement, the images are created from the  amplitude and phase of the reflected signal. An example of an  A-scan can be seen in figure 3.


Figure 3: Example of SAM-signal


In this signal two echoes are visible, the first from the surface  and the second from the first interface within the package. From these two echoes amplitude and phase are derived and  plotted into graphs, to identify changes in the acoustic  properties of the interface of interest. Delamination in the  package shows up as deviations in these images. But also the  time of flight between the different echoes, which can be seen  in figure 3, can be used as source for a 2D-Graph which gives  a hint about warpage. Therefore only the positions of the  maxima of the two echoes have to be determined. In our case  the time of flight between package surface and the warped  interface (die backside) is determined over the whole area of  interest. The surface of the sample is plan-parallel to the  reference plane of the CNC-machine, because the surface has  been pre-prepared by the milling machine and remains on the  sample holder. So from the time of flight (t), the distance  between the reference surface and the warped interface (d) is  calculated with knowledge of the velocity of sound (v) in the  materials between the two interfaces:


Figure 12: Time resolved thermal response for POI 1 at a Lock-in  frequency of 5 Hz


In addition, for the lock-in frequency of 5 Hz the introduced  power and measured response is significantly higher compared  to the 0.5 Hz excitation. Therefore, Figure 13 compares the  spectral intensity measured by the Lock-in system for 0.5 Hz  and 5 Hz using a log scale. It is clearly shown, that the spectral  intensity of the 5 Hz measurement is about factor ten higher  than the intensity of 0.5 Hz.


Figure 13: Spectral analysis of the measured thermal response (POI 1) of the LIT system with 0.5 Hz and 5 Hz using the MultiHarmonic approach


In summary, for each POI of the investigated active device the  same information about the frequency dependent phase shift  behavior till a frequency of 25 Hz could be extracted by two  instead of eleven single measurements by using the MultiHarmonic approach. For all POIs a good correlation between  both analysis approaches is shown.


A new post processing approach for non-destructive 3D  Lock-in defect localization is presented allowing a reduction  of measurement time by the factor 5-10 in comparison to  multiple single measurements. The theoretical background of  the approach was illustrated and its feasibility and capability  were demonstrated at a homogeneous opaque Ti-sample using  an external heat excitation source. Furthermore, the approach  was demonstrated at different hot spot positions of a packaged  hall sensor device. This test sample considers the real case  with IR-transparent Si die and mold compound with  inhomogeneous structure. For all investigated POIs with  different phase behavior the functionality of the method was  demonstrated. Thus, the presented new post processing  approach can also be applied to 3D-failure analyses. As a  consequence, the time expenditure for failure localization can  be significantly reduced supporting further upcoming defect  analysis steps or to increase the signal-to noise-ratio by longer  measurement times and reduced frequencies. In addition, the  method allows the prediction of the highest usable lock-in  frequency - with a sufficient signal-to-noise ratio - by only a  few measurements, which was demonstrated in the case study. As next step this approach has to be applied at more complex  devices e.g. multi-stacked dies.


The work presented in this paper was done in cooperation and  under partial funding of DCG Systems. We are grateful for the  provided samples by the company MICRONAS.


[1] O. Breitenstein: “ Lock-in Thermography – Basic Use for  Evaluating Electronic Devices and Materials, 255 pages,


Springer, 2010


[2] C. Schmidt et al., “Lock-in-Thermography for 3-dimensional localization of electrical defects inside


complex packaged devices”, proceedings of ISTFA 2008, p 102-107


[3] C. Schmidt et al., “Non-destructive defect depth  determination at fully packaged and stacked die devices  using Lock-in Thermography”, proceedings of IPFA  2010, p 1-5


[4] R. Schlangen et al., “Through Package Defect  Localization by Lock-In Thermography”, proceedings of  IMAPS 2010, p 312-316


[5] R. Schlangen et al:  “Use of Lock-In Thermography for  Non-Destructive 3D Defect Localization on System in


Package and Stacked-Die Technology”, proceedings of  ISTFA 2011, p68-73


[6] C. Schmidt, F. Altmann: “Quantitative Phase Shift  Analysis for 3D Defect Localization Using Lock-in


Thermography”, proceedings of ISTFA 2011, p 74-80


[7] Data sheet, MICRONAS HAL 1820 (July 2009)


Tomáš Hrn í  and Ji í Dluhoš


TESCAN Brno, Libušina t ída 1, Brno, Czech Republic


tomas.hrncir@tescan.cz, Tel. +420 530353468


Lukáš Hladík


TESCAN ORSAY HOLDING, Libušina t ída 21, Brno, Czech Republic


Efrat Moyal and Janet Teshima


LatticeGear, LLC, 1500 NW Bethany Blvd. Suite 200, Beaverton OR, USA


Jaromír Kope ek


Institute of Physics ASCR, Na Slovance 1999/2, Prague 8, Czech Republic


Cross sections of large Through Silicon Vias (TSV) and solder  bumps are often prepared using the Focused Ion Beam (FIB).  The high current Xe plasma ion source allows fast and precise  target preparation of TSV with small diameter. Solder bumps  can be accessed due to the high milling rate too. However, the  high current milling by plasma FIB causes the worsening of  the milled surface quality. An optimized FIB scanning strategy  accompanied with the novel rocking stage for the sample  tilting during the milling has been developed for the plasma  FIB. Whole milling process is observed by the Scanning  Electron Microscopy (SEM).  Time to prepare a cross section  is accelerated and the excellent quality is suitable for  subsequent failure analysis. Also important is proper sample  cleaving before FIB milling. Using an accurate method to  cleave the sample prior to FIB preparation further reduces the  overall sample preparation time. The high quality cross  sections prepared using this new method are ready not only for  SEM but also for EDX and EBSD analysis, either 2D or 3D, when combined with FIB slicing. Broadening the analysis to  these techniques increases the obtainable information, allowing    the arrangement of materials and their crystalline  structure to be studied in a detail.


FIB and SEM are essential techniques for failure analysis. FIB  is used for cross-sectioning the sample by ion milling or, when  accompanied by the Gas Injection System (GIS), for creating  protection layers by the deposition; SEM is used for imaging  of resulting cross sections at the high resolution, for charge  compensation, or as a source of electrons for other analytical  techniques. Two parameters of the cross section are crucial – the fast milling rate and the high quality of the surface, with  no damage or artifacts obstructing the failure analysis process.


This work is focused on recent advances in TSV and solder  bump cross-sectioning with FIB-SEM. In the past TSV have  been investigated by FIB cross-sectioning [1-4]. Bender et al.


[1] have performed a combination of the sample cleaving and  Ga FIB cross-sectioning and found ways to get rid of  curtaining artifacts by milling from the correct direction of the  ion beam towards TSV. The highest quality cross sections  were obtained when milling from the perpendicular direction, where the length of the ion beam path on the cross-sectioned  TSV was minimized. They have also performed FIB-SEM 3D  tomography of TSV by Ga FIB, which however appeared to  be very time-consuming process, so the necessity of the Xe  plasma FIB [2], that has much faster milling rates, for TSV  analysis has been suggested. 3D tomography of TSV with the  significantly increased throughput by using the high current  plasma FIB slicing was shown later [3]. The main problem of  the plasma FIB is the generation of curtaining artifacts, which  are more significant in comparison to Ga FIB due to the  increased beam diameter. Altmann et al. [4] have studied these  curtaining artifacts by atomic force microscopy (AFM). They  have minimized these artifacts by FIB polishing from two  different directions [4]. However, without SEM observation, this method makes cross-sectioning more difficult and less  accurate, as it requires pausing FIB polishing process and  changing the stage position to check the cross section quality  from time to time. This makes it difficult to stop the milling  when the desired point/structure is reached at small structures  and to minimize the curtaining artifacts. That is why the  research described in [4] was focused primarily to TSV with  large diameter of 50 μm. Here we are showing the new  method utilizing the novel rocking stage, which overcomes  these drawbacks.


Cross-sectioning of solder bumps by conventional mechanical  methods is limited by artifacts like smearing of the soft  material into the cracks and bump delamination, which makes  it difficult to determine the real defects and failure


mechanisms. These drawbacks can be overcome by using FIB  cross-sectioning [5]. However, due to the common size of  solder bumps being in the order of hundreds of μm, crosssectioning time using Ga FIB is time prohibitive for practical  work. Milling time for large bumps can approach several tens  of hours or even several days. Therefore it is a huge advantage  to use the high current Xe plasma FIB to reduce the milling  time [2, 6]. Plasma FIB is able to perform simple cross section  of the bump and when accompanied by SEM with several  detectors it can be also utilized for more complex 3D  tomography data acquisition [3, 7].


Even when using the high current plasma FIB milling, the  milling time can still be longer than acceptable for the  practical work, especially for big cross sections and for feature  size approaching 1 mm. Generally there are two simple and  straightforward methods to minimize the milling time with the  given FIB instrument (regardless if it is Ga or Xe plasma ion  source). The first method is the optimization of the beam  scanning strategy, by taking advantage of the angular  dependence of FIB sputtering yield. Figure 1 is showing this  dependence for several common materials. Obviously, the  maximum milling rate might be increased dramatically when  milling approximately tangentially to the sample surface, compared to the perpendicular FIB incident angle.


Figure 1: Dependence of FIB sputtering yield on the beam  incidence angle (measured from surface normal) for several  common materials [8].


The second method is to accurately cleave the sample such  that the feature of interest is already positioned close to the  edge of the sample. This has many advantages that reduce  sample preparation time and improve the cross section quality. Accurate cleaving produces a 90 degree cross section, eliminates redeposition effects, saves time as less material  needs to be removed and because the cleave follows the  crystal plane it produces a clean cross section face with many  repeating structures available for final polishing. In addition, Energy Dispersive X-ray Spectroscopy (EDX) and Electron  Backscatter Diffraction (EBSD), signal collection is optimized  using this type of cross section.


To obtain the highest throughput and most analysis flexibility  on a wide variety of samples, the cross-sectioning process can


be optimized by using the combination of accurate sample  cleaving, optimized scanning strategy and sample tilting in the  cross section plane while imaging it simultaneously with the  SEM. Of course there are more ways to speed up FIB analysis  for a given sample (gas-assisted etching, laser ablation,...) but  these methods are limited to a certain type of samples, some  processes are lengthy or require another complex (and  expensive) instrument for the sample preparation.


To obtain really comprehensive information about structures  like TSV or solder bumps, sometimes it is not enough to  utilize SEM and FIB imaging only. The complete information  about the material composition and structure can be obtained  by performing FIB-SEM 3D tomography [1, 3, 7] or by including other analytical methods like EDX and EBSD. These methods were traditionally used for obtaining 2D  information from the analyzed cross section only (Fig. 3), but  now these can be expanded to 3D space too. The plasma FIB  allows fast slicing of structures and each slice can be analyzed  by EDX or EBSD. The first 3D EDX (Fig. 4) and 3D EBSD (Fig. 5) results obtained on TSV and solder bumps by using  plasma FIB for the gradual slicing of the sample will be  presented. 3D EDX on solder bumps gives detailed  information about the solder structure and it can reveal  elemental or phase distribution like formation of dendritic  structures in the solder or diffusion processes between the  solder and substrate. The 3D EBSD on TSV offers thorough  information about the crystal structure of TSV copper filling  material. Data acquired by both 3D EDX and 3D EBSD also  provide necessary analytical information for precise  simulation of thermal or mechanical properties of the  structure.


The first experiments with automated 3D EDX and 3D EBSD  as analytical method, using the Ga based FIBs, were introduced in 2006 [9, 10].  Due to low milling rates of Ga  based FIB the method was limited only to certain microstructured materials. The maximum dimensions of several tens  of micrometers was leading to enormous acquisition times  easily extending several days, limited by both FIB milling and  EDX/EBSD acquisition speed. With the recent large area, high  speed EDX and EBSD analyzers a high resolution maps can  be acquired in few minutes. The introduction of plasma FIB  extends these techniques to a more metallurgical point of  view, allowing study of objects with dimensions of several  hundreds of micrometers in few hours [11].


For TSV with the lower diameter and for the detection of  small failures or features in general, the novel method is  introduced here, which allows changing of FIB milling  direction during the polishing process easily, while observing  the cross section placement and quality by SEM imaging. Commonly used eucentric sample stages allow the tilting only  around the axis perpendicular to both FIB and SEM columns.


The novel multi-tilt sample stage (called “rocking stage”) allows an additional tilting also in the plane of the cross  section. Unlike the solution described e.g. in [4], where the  eucentric stage was used, the proposed method allows to  control the whole milling/tilting process by SEM imaging (Figure 2), which is essential for the precise end-point  detection. The range of tilting is 10º in all directions, which is  enough to reduce the curtaining effect [4]. Greatly improved  results were obtained on TSV with the diameter 5 μm and  length 50 μm, where it is important to stop FIB polishing in  the middle of TSV row and at the same time to minimize the  curtaining effect at the cross section (Figure 3).


Figure 2: Principle of the novel multi-tilt sample stage, which  allows SEM observation during FIB milling process, in a case  the sample requires milling from multiple directions to reduce  the curtaining effect.


Figure 3: a) Cross section of six TSVs, each one 50 μm long, preparation time 30 min. BSE imaging at SEM beam energy  30 keV. b) Demonstration of the sample tilting in the cross  section plane during FIB polishing, while imaging the  polishing process with SEM.


The main advantage of the novel rocking stage is the  possibility to perform fast and precise FIB milling from  multiple directions and detailed SEM observation together, which simplifies the cross-sectioning process, allows the  precise end-point detection on small structures and improves


the final polishing quality, as the operator can stop the  polishing process at the point when the curtaining effect is  minimized according to SEM imaging performed during FIB  processing simultaneously.


An optimized scanning strategy for the cross section is  important to increase the throughput, mainly because of the  strong angular dependence of FIB sputtering yield (Figure 1). To obtain the minimum time for a given depth of the cross  section, it is necessary to keep the slope of the sample surface  under the ion beam close to the maximum sputtering yield  condition. Apart from increasing the sputtering yield, it is also  necessary to reduce the redeposition artifacts to avoid  obstacles limiting the effective depth (Figure 4). The effect of  the redeposition on the shape of the cross section was  modelled [12]. According to the obtained shape, it is necessary  to correct the scanning strategy in order to remove the  redeposition artifacts and to have a flat bottom surface of the  cross section, without any obstacles to following SEM  observation. Therefore we have combined two changes of the  scanning strategy, the first one to increase the milling rate, the  second one for compensation of the redeposited artifacts  blocking the attainable depth of the cross section, which could  be observable by SEM.


Figure 4: Example of redeposition artifacts on a cross section  object. (a) Milling without shape correction, where the  effective depth for SEM observation is reduced by the  redeposited material. (b) Milling with the use of the shape  correction, where there are no obstacles originated by the  redeposited material.


b


The resulting cross section shape is greatly improved and  around 2.5 times deeper when compared to the classical stair  shape and much nicer when compared to the shape obtained  by one-pass polishing method. The obtainable depth of the  cross section in dependence on the scanning strategy is shown  on Figure 5. The cross-sectioning rate has been increased 2.5  times. This approach shortens the cross section preparation  time significantly, independently on what type of the focused  ion beam is used.


Figure 5: Increasing cross-sectioning rate by optimizing the  scanning strategy. Milling time 2 min, cross section area  10x10 μm2, Ga FIB at 12 nA, 30 keV.


A) Classical stair strategy, which gives a nice shape but it is  slow (depth 5 μm).


B) One-pass polishing, where the shape is corrupted by redeposition artifacts, reducing the obtainable depth (8 μm).


C) Novel optimized strategy, with the nicest shape and the  highest depth of the cross section (depth 13 μm).


High accuracy cleaving [13] is a simple method that can be  used prior to FIB milling to position the feature of interest  close to the cross section face. Figure 6 shows how cleaving is  integrated into the workflow for cross section sample  preparation. There are two paths, single-tool and multi-tool


[14]. In the single-tool case samples flow directly from  cleaving to the SEM. This yields the fastest cycle time. The  cleaving tool shown is the patent pending LatticeAx and can  achieve up to 10 μm targeting accuracy with a 5 minute cycle


time. Samples needing higher accuracy or additional surface  preparation follow the multi-tool path. In this case, FIB or  other methods are used to finalize the cross section. Copper  filled samples such as the TSVs and solder bumps follow the  multi-tool workflow while front end and etched samples  typically follow the single tool path.


Figure 6: Workflow for cross-sections prepared by high  accuracy cleaving.


The cleaving step has several values. First and foremost, it is  fast and provides the accuracy and quality needed to reduce  FIB time. Figure 7 shows a cleave through copper filled  5x50 μm TSV test structures. The LatticeGear LatticeAx300 was used for sample cleaving. The sample was cleaved cleanly  and perpendicular to the sample surface producing multiple  sites for the cross section. The FIB was used to quickly (30  min) finalize the cross-section, which could take up to 1 hour  without performing the cleaving step (rough milling of the  cross section is not necessary on the cleaved sample).


Figure 7:  Cross-section of Copper filled TSVs prepared using  the multi-tool workflow.


The cleaving apparatus (Figure 8) is integrated with a highmagnification vision (5 μm resolution) hardware and software  to allow the user to view the area of interest (AOI) and  position the indentation precisely aligned with it.  Using the


100 μm


software provided, the user draws a line that begins at the


sample edge and extends through the target.  The indenter is  then positioned over the line using the micrometer (step size = 5 μm) resulting in high quality cross sections from the top to  the bottom of the TSV and accuracy of ±10 μm.


Figure 8: High Accuracy Cleaving Apparatus.


Solder bumps are prepared using a 2-step multi-tool workflow. The indent-and-cleaving process takes 5-min and positions the  bump on the edge of the cross-section.  Using the plasma FIB  for the final polishing step results in artifact-free cross sections  of the solder bump/s at a total preparation time of less than 20  min per bump. The time to cross section scales to hours or  days if bulk milling is required.


It should also be noted that images of cleaved cross sections  result in accurate critical dimension measurements because  they allow the image surface to be normal to the SEM electron  beam (geometrical corrections are not required).


New methods for TSV and solder bump analysis


3D EDX on the solder bump and 3D EBSD on TSV have been  performed for the first time. 3D methods applied on such  features usually require either lift-out of the block of the  sample containing the analyzed structures [3] or to mill a  trench around the analyzed volume by FIB, to allow the beam  access to the volume, to minimize the redeposition artifacts  and to have more uniform signal on each of the analyzed  slices. Here the proper cleaving of the sample allows  removing these preparation steps. These steps can usually take  a significant amount of time, do the big advantage of the


cleaving is the considerable reduction of the total analysis  time. Cleaving does not help only in a case the features are  protruding above the surface and are well accessible by SEM  and FIB beams, e.g. for solder bumps which are protruding  above the surface of the sample.


3D EDX of a Solder Bump


Cross section of the whole bump imaged by SEM is shown on  Figure 9. The bump diameter was 100 μm, time to get cross  section by plasma FIB was approximately 20 min. The 3D  EDX acquisition was done in a static position on a noncleaved sample. A 10 μm thick Pt layer was deposited using  the GIS to protect the sample edge and to crop the EDX signal  on the bump surface.  For the slicing the TESCAN FERA3  with Xe FIB current of 120 nA at 30 keV was used.  For the  EDX acquisition a 60 mm2 silicon drift detector EDAX  Apollo 60 was used. The electron currents for EDX  acquisition were 30 nA at the beam energy 15 kV, which leads  to about 900 kcps input count rate of X-Ray and detector dead  time about 34%.


Figure 9: Cross section of Pb/Sn solder bump with the  diameter 100 μm, imaged by SEM using the backscattered  electron detector. Pb/Sn material contrast is clearly  resolvable.


For the acquisition resolution of 500 nm in all three  dimensions was used. The time per slice was 22 s for FIB  milling and 1 min 20 s for EDX map acquisition. Total  volume of 180 slices was acquired in about 5 hours. EDX  detector was protected by the automated motorized shutter  during FIB milling, the shutter was moved out during EDX  mapping process. The mapping was done with full spectra  acquisition in each point. The individual 3D maps were  extracted from this hyper-spectral data cube for each element  individually as a spectrum ROIs: Sn Lα1 (3364 – 3520eV) +Lα2 (3616– 3730 eV), Pb-Mα (2302-2405), Cu Kα (7960-8122 eV), Ni Kα (7392–7550 eV). The individual 3D channels  were visualized (Figure 10) using ORS Visual software [15].


Figure 10: Visualization of 3D EDX elemental maps a solder  bump. X-Ray lines of Sn L 1 (green), Pb M 1 (red), Cu K(blue) and Ni K  (purple) were used for map extraction. Dendritic structure of a rapidly solidified Pb rich -phase and  diffusion of Cu into Sn is observed.


From the 3D distribution of individual elements or phases we  can easily evaluate the thermal history of the solder e.g. creation of dendritic structures is a typical result of rapid  solidification of a hypoeutectic solder [16].


The typical EBSD map on TSV sample is shown on Figure 11. By preparing a set of slices like this we can make 3D  reconstruction of TSV volume. These 3D EBSD results were  acquired on a sample cleaved about 20 μm from the 5x50 μm  TSV to save the sample preparation time. Without cleaving  the sample before the analysis, it would be necessary to  perform a lift-out of the block containing several TSVs [3], so  the cleaving step saved at least 1 hour of FIB operation time.


A triangular side trenches were prepared using 2 μA ion  current using Xe plasma FIB in about 45 min. For 3D EBSD  acquisition FIB current of 300 nA at 30 keV was used. For  EBSD acquisition electron beam current of 30 nA at 20 kV  was applied. For ultra-fast EBSD mapping a high speed EBSD  camera EDAX Hikari with binning 5x5 was used, reaching  acquisition speed of about 100 patterns/s. In such  configuration it was possible to reach slice time about 6 min (13 s FIB milling, 5 min 42 s EBSD acquisition).  The overall  acquisition of 250 slices with lateral map resolution of 100 nm  and slice thickness of 200 nm was performed in approximately  25 hours. In case of using binning 6x6 the camera frame rate  was 300 patterns/s, which leads to about 5x faster acquisition (1.2 min per slice, total acquisition time 6 hours).


The 3D EBSD was acquired using the EDAX TEAM Software  API, for the postprocessing EDAX 3D OIM software was  used. The visualizations (Figure 12) were done in Fiji [17].


Figure 11: A set 4x50 μm TSVs polished by plasma FIB to  EBSD quality. EBSD map shows SEM SE image with  overlaying IPF orientation map.


Figure 12: 3D EBSD reconstruction of a single 5x50μm  copper TSV, EBSD mapped using IPF-Z orientation coloring  mode. a) Visualization of TSV surface, b) virtual cross section  in an arbitrary angle.


Characterization of large semiconductor structures such as  TSV and solder bumps by Ga FIB has been limited by the  prohibitively long sample preparation times (hours to days). The Xe plasma FIB, with novel scanning and stage rocking  capabilities, coupled with accurate cleaving prior to FIB have  been shown to be an effective way to reduce sample


preparation time. This is achieved in less than an hour without  compromising quality.


The results from 3D EDX of a solder bump and 3D EBSD of  TSV show that using the Xe plasma FIB it is possible to reach  a high quality 3D Tomography together with important  analytical information like elemental distribution or crystal  orientation. The time requirements for such an analysis are  close to acceptable routine analytical times.


The research has been supported by the Technological Agency  of Czech Republic *TE 01020233 (AmiSpec) and by the Academy of Sciences of Czech Republic, project FUNBIO: CZ.2.16/3.1.00/21568.


1. H. Bender et al., “Structural characterization of through  silicon vias”, J. Mater. Sci. Vol. 47 (2012), pp. 6497.


2. T. Hrnčíř et al., “Novel plasma FIB/SEM for high speed  failure analysis and real time imaging of large volume  removal”, ISTFA: Conference Proceedings from the 38th  International Symposium for Testing and Failure Analysis (2012), pp. 26.


3. T. Hrnčíř and L. Hladík, “Fast and Precise 3D  Tomography of TSV by Using Xe Plasma FIB”, ISTFA: Conference Proceedings from the 39th International  Symposium for Testing and Failure Analysis (2013), pp.


27.


4. F. Altmann, J. Beyersdorfer, J. Schischka, M. Krause, G. Franz and L. Kwakman, “Cross Section Analysis of Cu Filled TSVs Based On High Throughput Plasma-FIB  Milling”, ISTFA: Conference Proceedings from the 38th  International Symposium for Testing and Failure Analysis (2012), pp. 39.


5. L. Cao, L. Tran, W. Donna, “Failure Analysis of Flip  Chip C4 Package Using Focused Ion Beam Milling  Technique”, ISTFA: Conference Proceedings from the  37th International Symposium for Testing and Failure  Analysis (2011), pp. 81.


6. P. P. Tesch, N. S. Smith, N. P. Martin, D. Kinion, “High  current focused ion beam instrument for destructive physical analysis applications”, ISTFA: Conference  Proceedings from the 34th International Symposium for  Testing and Failure Analysis (2008), pp. 7.


7. T. Hrnčíř, L. Hladík and M. Zadražil, “Fast 3D  Tomography at package level by using Xe Plasma  Focused Ion Beam”, 20th IEEE International Symposium  on the Physical and Failure Analysis of Integrated  Circuits (IPFA) (2013), pp. 112.


8. B. I. Prenitzer et al., “The Correlation between Ion  Beam/Material Interactions and Practical FIB Specimen  Preparation”, Microsc. Microanal. Vol. 9 (2003), p. 216.


9. M. Schaffer, J. Wagner, B. Schaffer, M. Schmied, H. Mulders, “Automated three-dimensional X-ray  analysis using a dual-beam FIB”, Ultramicroscopy 107 (2006), pp. 487.


10. J. Konrad, S. Zaefferer, D. Raabe, “Investigation of  orientation gradients around a hard Laves particle in a  warm-rolled Fe3Al based alloy using a 3D EBSD–FIB  technique”, Acta Mater, Vol. 54 (2006), pp. 1369.


11. J. Dluhoš et al., “Ultra-Fast Three Dimensional  Microanalysis Using the Scanning Electron Microscope  Equipped with Xenon Plasma Focused Ion Beam”, Conference Proceedings from the 18th International  Microscopy Congress (2014), pp. 1143.


12. H. B. Kim, G. Hobler, “Simulation of Focused Ion Beam  Milling”, Nanofabrication Using Focused Ion and  Electron Beams, Oxford University Press (2012), pp. 226.


13. E. Moyal, E. Brandstädt, “Cleaving Breakthrough: A New  Method Removes Old Limitations”, EDFAAO Vol. 3 (2014), pp 26.


14. J. Teshima, E. Moyal, J.J. Clarke, “Streamlining Sample  Preparation of Semiconductor Materials with a New Sitespecific Cleaving Technology”, Microscopy Today (2013) pp. 56.


15. ORS Visual, http://www.theobjects.com


16. J. F. Roeder, M. R. Notis and H. J. Frost, “Physical  Metallurgy of Solder Systems”,  Solder Mechanics – A State of the Art Assessment, The Minerals, Metals & Materials Society (1991), Chapter I, pp.4


17. Fiji Image Processing Package, http://www.fiji.sc


The Physical Isolation of a Die in a Stacked-Die Configuration


Vivian Jang, Ken Sias


Texas Instruments 12500 TI Blvd. Dallas, Texas USA  vijang@ti.com, ksias@ti.com


This paper will illustrate the procedures to physically isolate  one die in a stacked-die configuration. This highly reliable, systematic method allows for failure analysis engineers of all  levels to successfully isolate the die of interest for further  investigation.


The price of real estate on semiconductor chips has been  steadily increasing as the trend for smaller consumer products  continues to dominate the market space. To meet this demand  arose the stacked-die configuration that creates a component  solution to existing technologies [1]. This strategy allows for  the elimination of multiple devices by presenting one packaged  product, which leads to reduced board space in addition to  faster operating speeds [2].


The warpage of the die can be determined in the order of some µm, especially if high frequency transducers are used. The  measurements are done in our case in a Sonoscan Gen5 and  stored to hard disk with help of Sonoscan VRM mode. Then  the data is processed in a standalone Matlab GUI that was  developed for warpage calculations of the surface and buried  interfaces. This GUI can also export warpage data for further  processing in Matlab. Figure 4 shows an example of this  measurement. A thin die in a complex multi-chip package  shows a warpage of about 15µm between one die corner and  the center of the die. In general also warpage larger than the  die thickness can occur. Parallel grinding of such a kind of  package for backside preparation purpose would destroy the  die and any further electrical defect localization would be  impossible. Therefore the backside preparation has to be done  in this case in a way that follows the contour of a warped  interface.


Figure 4: Warpage measurement of die surface


The SAM warpage measurement offers very precise and  reliable results. To ensure the correctness of the measurement  method, different comparisons with other methods have been  done. These comparisons are sometimes difficult for this  package because warpage may change due to processing of the  sample. So a good mechanical stabilization of the sample is  necessary that warpage cannot change during process and  results of different methods are comparable. At least for line  scans of the warpage measurement this can be achieved by  comparison with mechanical cross-sections. To accomplish  this comparison at first the SAM warpage measurement was  done of the die backside of one device, see figure 5. SAM was  done through Cu-heat sink. Calculation was done with a speed  speed of sound 4.7 µm/ns for Cu.


Figure 5: Warpage measurement of die backside with position  of cross-section plane (figure 6) marked (black dots)


From this measurement a linescan along the black line was  extracted, see figure 6. The start of the linescan is on the lower  left side of the black line and it is headed to the minimum of  the die near the upper right corner.


Figure 6: From Figure 5 extracted linescan (along black line)


The difference in thickness between the two sides is 42 µm.


Then this sample was mechanically cross-sectioned along the  black line. The optical microscopy image has been expanded  along the vertical axis by a factor of 4, see figure 7.


Figure 7: Cross-section along line specified in figure 5; plot  has been expanded in vertical direction by a factor of 4


The cross-section is aligned in the same direction as the SAMlinescan. The Cu layer of interest can be seen on the top side  of the image, the die is soldered below of it. The thickness  measurements between both sides in the mechanical crosssection vary by 42 µm. This is the same value as determined  in SAM warpage measurement.


Additional verification for the precision of SAM warpage  measurement was done with a tilted die soldered on a lead. The SAM-measurement was done through the lead and die  and focused on the die front side. This warpage measurement  with leveled lead surface can be seen in figure 8. It was done  with a sound velocity for solder of 2.7 µm/ns, which was  determined by the use of a calibration sample.


Figure 8: Warpage measurement of die backside through lead  and solder with position of cross-section plane marked (black  solid line)


Figure 9 shows a cross-section that was extracted from figure


8. It is marked in figure 8 with black dots. The statistical error  of the measurement along the line is below 1 µm.


Figure 9: SAM-Cross-section along black-dotted line in  warpage measurement (figure 8)


As comparison X-ray tomography was done and a crosssection was extracted along the same line as the cross-section  extracted from the warpage measurement (figure 9). In the  SAM cross section a tilt of about 11 µm can be measured from  edge to edge. From X-ray cross sections in figure 10 the same  difference (11µm) between the two edges was determined.


Figure 10: X-ray Tomography Cross-section through tilted die  seen in figure 8


So the method can detect tilts and warpage with the precision  of approximately one micrometer. This is absolutely sufficient  to provide information for the milling process.


Creation of CNC-code


We have developed a Matlab routine that allows transferring  contour data in Haidenhain-CNC-code used by our CNCmachine. The CNC-machine then mills from pixel to pixel  into the interface of interest.  Profile data of a SAM  measurement as shown in figure 4 can be used as input. But  before this data can be transferred to CNC-code, preprocessing  steps are necessary to eliminate outliers, because considering  of these pixels could lead to destruction of the sample in the


milling process, if the milling tool would go through the front  side of the die due to defective pixels. A second step is to bin  the pixel for increased accuracy. As first step the distribution  of the heights within the die area is calculated. The  distribution clearly shows the outliers and also minimum and  maximum of the warped interface. So, if necessary, all outliers  that are below the minimum and above the maximum can be  marked and excluded from further processing. Then the  number of pixels is decreased by 5x5 pixel averaging. This  leads to increased accuracy for each pixel. This does not affect  the lateral accuracy of the milling process because the reduced  pixel size is still much smaller than the used milling tool.  So  from fig. 4 a profile is extracted for contour milling (shown in  fig. 11).


Figure 11: Warpage measurement of die surface with  decreased pixel resolution


The larger die in figure 11 shows no more deviant pixels  originating from die front side structure and also the statistical  fluctuations between the pixels are sufficiently low. The  adapted data of the die area is then transferred to CNC-code. This code describes the milling process from pixel to pixel in  meanders over the whole die area.


Contour Milling


The generated CNC-code is finally transferred to the milling  machine. In this case plan-parallel milling was applied to thin  the Cu layer further. The remaining Cu had a thickness of  about 10µm. Then the profile as shown in figure 11 was  milled successively with increasing milling depth until the die  was exposed. To get a smoother transition between the pixels  a spherical milling tool was used. But this kind of milling tool  still creates grooves along the meander line. To remove this  and to get a really smooth surface the meander structure was  repeatedly milled with small offsets of about 25 µm in the  meander direction. So only small relicts of the grooves  remained and after an additional polishing step the backside  surface quality was sufficiently to inspect the front side of the  die by IR-microscopy from the backside. Figure 12 shows an


L / pixels


Cu-Leadframe


Solder


Die


image of the decapsulated device processed by contour milling  ready for localization.


Figure 12: Decapsulated die ready for electrical localization  A cross section along the longer package side shows a  difference of die thickness of about 1,5 µm, see figure 13. So  the die thickness is nearly constant, although the die showed  original a warpage of 15 µm within the package. Also no  mechanical damage due to milling could be found in the crosssection. Further backside preparation and electrical  localization will therefore be enabled with this method.


Figure 13: Comparison of die thickness between center of die (upper picture) and die edge (lower picture)


It was shown, that the combination of SAM warpage  measurement and accurate CNC milling makes it possible to  prepare surface conform into warped interfaces. This  application will become more and more important as package  complexity increases and layer thicknesses (especially die  thickness) decreases causing warpage. The effort for one  sample is currently 5 hours but with further software  integration this time can be reduced.


In this paper SAM was used to determine the die warpage. But  also other methods could be used to derive this data, e.g. optical profiler for surfaces or 3d-X-ray tomography. It would  only be necessary to transfer the contour information into  CNC-code to enable the contour milling process.


We would like to thank Dr. Richard Neumann for providing a  set of measurement samples and also Klaus Lidl for  performing the very good cross-sections shown in this paper. Additionally we want to thank the Zecha HartmetallWerkzeugfabrikation GmbH for advice in milling tools.


[1] J. Colvin, “FemtoFarad/TeraOhm Endpoint Detection for  Microsurgery of Integrated Circuit Devices”, Proc. ISTFA, 2012


[2] http://www.pvaanalyticalsystems.com/produkte/samnalysissoftware/pva/samnalysis-software/3d-surface-imaging


[3] C. Hollerith, “Advanced Package Circuit Modification by µMilling”, Proc. IPFA, 2014


[4] Kessler, L. W., "Acoustic Microscopy",


Nondestructive Evaluation and Quality Control;


Metals Handbook, Volume 17, 9th Edition, ASM


International, 1989, p 465-482.


Efficient non-destructive 3D Defect Localization by Lock-in Thermography  utilizing Multi Harmonics Analysis


Falk Naumann, Frank Altmann, Christian Grosse, Rolf Herold


Fraunhofer Institute for Mechanics of Materials IWM,


Center for Applied Microstructure Diagnostics, 06120 Halle, Germany


Falk.Naumann@iwmh.fraunhofer.de


Lock-in Thermography in combination with spectral phase  shift analysis provides a capability for non-destructive 3D  localization of resistive defects in packaged and multi stacked  die devices. In this paper a novel post processing approach  will be presented allowing a significant reduction of  measurement time by factor >5 in comparison to the standard  measurement routine. The feasibility of the approach is  demonstrated on a specific test specimen made from ideal  homogenous and opaque material and furthermore on a  packaged hall sensor device. Within the case studies the  results of multiple single LIT measurements were compared  with the new multi harmonics data analysis approach.


It was already shown in [2]-[6], that the method of Lock-in  Thermography (LIT) is able to identify electrical resistive  defects in packaged devices and locate it in all three  dimensions. Up to now multiple LIT measurements are  required to determine the phase shift to frequency  characteristic of hot spots used to pinpoint the defect site in  relation to the interconnect or die level.


Figure 1: Simplified sketch of a stacked die device. The phase shift to  frequency characteristic is calculated and measured enabling a  fingerprinting of defect site related to the die level [6]


The general approach for 3D hot spot localization is  demonstrated on a packaged stacked die device in [6]. As a  result of the thermal heat diffusion through the die attach tapes (DAT) and the package material, a difference of the phase  shift value can be measured for each die level. Because the  measured phase shift depends on the used lock-in frequency  itself, multiple measurements at different single frequencies  are required to determine the phase shift to frequency graph  which is representative for each die level. Therefore, the  common measuring process could be very time consuming. Especially for defects within packaged devices with low heat  dissipation the whole measurement can take many hours. As a  drawback of this approach, typically defects within packaged  devices can only be measured at low lock-in frequencies in  order to achieve an acceptable signal-to-noise ratio for phase  shift determination limiting the identification of the phase shift  to frequency characteristic. Furthermore, at low lock-in  frequencies the lateral resolution for hot spot localization is  reduced, caused by increased heat dissipation within the  device.


To overcome these limitations we have developed a new post  processing approach allowing to extract an advanced phase  shift to frequency characteristic from only one LIT  measurement utilizing Fourier analysis of the time-dependent  thermal signal shape. This approach allows a significant  reduction of the required excitation frequencies for the lock-in  process without loss of measurement information.


Principle of 3D Lock-in Thermography


The operational principle of Lock-in Thermography is well  described in [1] and can be applied for 3D defect depth  localization utilizing time-dependent heat propagation. After  periodic stimulation of a heat source which is covered by one  or multiple material layers, the heat can propagate through the  several layers and is measured as a local temperature increase  on the device surface. The time delay between heat generation  at the defect site and the thermal response measured at the  device surface determines the phase shift signal, which can be  extracted by two phase LIT. The thermal diffusion process is a  function of time, the applied lock-in frequency and the thermal  properties of the layer system above the defect position. The  one dimensional analytical calculation of thermal wave  propagation gives a square root characteristic of the phase  shift to frequency behavior and is in most cases a good  approximation for measurements at packaged devices. Related  experimental results are shown in [3]-[6].


Using the standard approach, the calculation of the phase shift  of the thermal response is realized by a harmonic oscillator at  constant excitation frequency and can be described by  equation (1).


Thus, the estimation of the resulting phase by the Lock-in  process is realized, using two different weighing functions (sin/-cos). This allows splitting the thermal response in two  parts (S0, S90 image) and the integration over all periods of  the measurement time occurs. The resulting phase φ is  calculated from the S0– image and 90° phase shifted S90– image using equation (2). The complete mathematical  description can be found in [1].


Caused by the low intensity of the measurable temperature  signal during investigation, the effort of time for phase  measurements at multiple frequencies is relatively high. Hence, the major benefit of this approach is given by the fact  that over the total measurement time only the integrated and  averaged signal has to be stored for each pixel and the  resulting measurement data can be reduced significantly.


The new approach is based on the capability to store the total  temperature versus time behavior of a selected couple of  points of interests (POIs). These data are averaged over all  periods of the whole measurement time allowing further signal  processing. Depending on the defect type the signal shape of  the thermal excitation can be assumed as a nearly rectangular  or square-wave function. Because of the excitation bandwidth  of the function the thermal heat generation consists of a  fundamental mode at the lock-in frequency and further  additional harmonics at higher frequencies.


These higher harmonics - which are influenced by the thermal  dampening characteristics of the investigated sample - can  also be analyzed from the measured thermal response shape. Thus, correlating the stored and averaged time resolved signal  y(t) with the input signal x(t) at the frequency domain, the  transfer function H(jω) can be estimated from the Fourier  transformations (X(jω)),Y(jω)) by equation (3).


From this function the phase shift  of the fundamental and  each calculated higher harmonic frequency ω can be  determined using equation (4).


As a result, a high range of LIT frequencies correlated with  the phase shift response can be calculated by only one  measurement significantly reducing the overall measurement  time.


Evaluation of the Multi Harmonics Signal  Analysis on Homogeneous Test Samples


For practical evaluation LIT measurements were carried out at  reference samples to correlate the Multi Harmonics approach  with conventional experimental results. As reference a  homogenous and ideal opaque sample made of titanium with a  thickness of 1 mm was investigated. This sample was  stimulated on the backside by needle probing (biased with  1 V) - simulating a hot spot generated by a point like defect - and analyzed by LIT from the front side. The resulting time  resolved signal was recorded for phase shift estimation at  different lock-in frequencies in the center of the hot spot. Figure 2 shows the waveforms of the applied voltage and the  resulting temperature at the sample surface exemplary at a  Lock-in frequency of 0.5 Hz (green). As a result from the  thermal dampening the measured signal output (red) shows a  distorted waveform with small phase delay from excitation.


Figure 2: Waveform of the applied voltage and the resulting  temperature at the sample surface at 0.5 Hz


The calculated amplitude distribution from this thermal signal  at the frequency domain is shown in Figure 3. In addition to  the excitation (green) the measured temperature signal  response (red) shows also terms higher order up to a frequency  of about 25 Hz which are stimulated by the bandwidth of the  square wave signal.


Figure 3: Amplitude of the electrical excitation and the thermal  response at the surface at 0.5 Hz


After calculating the phase shift by equation (4) for each  higher harmonic signal, the phase delay as a function of  frequency can be determined and is shown in Figure 4, calculated from only one measurement at a lock-in frequency  of 0.5 Hz.


Figure 4: Comparison of the phase shift values of the LIT  measurement in comparison to the Multi Harmonics analysis at


0.5 Hz


In addition, the graph shows nine separate measurements at  different lock-in frequencies (black) - using the common  approach (equation 2) for phase shift estimation - showing a  similar behavior up to about 25 Hz in comparison to the  calculated phase shift from only one single measurement at


0.5 Hz using the Multi Harmonic approach. Only at the  frequency range above 15 Hz a slight scatter of the phase shift  calculated by Multi Harmonic approach can be observed, resulting from the increased signal-to-noise ratio caused by the  reduced excitation magnitude and higher thermal dampening  at enhanced frequencies (see Figure 3). Considering the  frequency range up to 15 Hz were scattering occurs, a  reduction from 8 to 1 measurement could be achieved by the  Multi Harmonic approach at the idealized test sample.


Evaluation of the Multi Harmonics Signal  Analysis on a Hall Sensor Device


Since no devices with real defects are implicitly needed for  demonstration of usability of the Multi Harmonics method, the  LIT measurements were carried out on a magnetic field sensor  device HAL 1820 manufactured by MICRONAS in a small  leaded package TO92UA [7]. For the investigations the device  was operated under normal working conditions, meaning with  a bias of 5 V and a current consumption of approximately  6 mA.


In contrast to the previous investigation of a homogenous and  opaque material, the sample consists of a Si-die embedded in  molding compound (MC) representing an inhomogeneous  material and contacted by Au wire bonding to the lead frame. After a first test measurement @ 22.52 Hz (see Fig. 5) three  POIs related to thermal active areas were defined. At these  POIs, the phase shift to frequency characteristics was  determined by multiple LIT measurements following the


common approach and in addition the thermal waveform was  measured and analyzed by Multi Harmonics.


Figure 5: Overlay of amplitude and topography image @22.52 Hz (left) and position of the POIs (right)


Figure 6 shows a mechanical cross section through a similar  device. As can be seen by comparison between Figure 5 and 6, the POIs were chosen at the position of local hot spots at the  MC (POI 1 & 2) and the lead frame (POI 3) maximizing the  usable signal-to-noise ratio.


Figure 6: Cross section of a similar device with highlighted positions  of the measured POIs


Caused by the SiO2 filler particles in the MC the heat transfer  occurs through a material composition with different thermal  diffusion properties, multiple thermal interfaces and potential


heat transfer by radiation through the SiO2 filler.


The three POIs differ in th


e thickness of the MC the thermal wave has to pass to reach  the surface and in the case of POI 2 and 3 the addition lateral  spreading of the thermal wave. In the case of POI 1 the  thermal wave has to spread out through ≈ 394 μm MC to reach  the surface. The thickness of the MC at POI 2 is ≈ 270 μm and  POI 3 ensures a direct optical approach to the lead frame  because the Si die is IR transperant. Thus, the phase shift at  POI 3 is only influenced by the lateral heat transfer within the


Cu leadframe.


Although the Multi-Harmonic approach just presents an  alternative for the phase calculation in the first case, the  frequency behavior of the phase shift is influenced by the heat  propagation parameters, the frequency dependent heat transfer  coefficients between different material layers and the phase  delay of active stimulated components, where a superposition  of these effects cannot be precluded. As a consequence, the


analysis of the phase shift information of the 3D Lock-in  analysis becomes much more complex and the principle  functionality of the post processing approach should be  demonstrated for these three sample conditions compared to  the common approach.


LIT investigations


During LIT investigations, the device was analyzed at 11  different lock-in frequencies in the range from 0.5 Hz up to


22.5 Hz. A measurement time for each frequency of about one  hour was used in order to reach a sufficient signal-to-noise  ratio. The resulting phase shift versus the lock-in frequency of  these measurements is shown in Figure 7.


Figure 7: Phase shift results of the LIT measurements for the  different POIs


Caused by the thermal properties of the materials, in which the  heat wave is spreading out and the thermal propagation  distance to reach the surface, all POIs are showing a different  phase shift to lock-in frequency behavior.


It is clearly shown that POI 3(without MC layer) and 2 (with  reduced thickness of the MC layer) has a reduced phase shift  in comparison to POI 1 at the surface. Therefore, independent  from the cause of thermal phase delay, three different hotspots  with different frequency dependent behavior are available to  investigate the capability of Multi-Harmonics approach.


Comparison between results of LIT measurement and  Multi Harmonics Analyses


After the LIT investigations the results of the measurements  with a Lock-in frequency of 0.5 Hz has been analyzed using  the Multi Harmonics approach. The results of these analyses  and the comparison to the LIT measurements are shown in the  following Figure 8.


Figure 8: Comparison of the results of the single LIT measurements  and the Multi Harmonics analyses @0.5 Hz for POI 1-3


All POIs are showing a very good correlation between the  single measurements and the Multi Harmonic approach until a  lock-in frequency of about 15 Hz. At this frequency, the  measured signal-to-noise ratio leads to some scatter of the  calculated phase behavior.


Figure 9: Time resolved thermal response for POI 1 at a Lock-in  frequency of 0.5 Hz


The corresponding recorded and averaged time signal for


0.5 Hz of POI 1 is shown in Figure 9. The signal behavior  shows a saw-tooth shape resulting from the thermal  dampening of the initial square wave signal during heat  propagation. From the signal behavior it becomes obvious, that the periodical signal must be a superposition of multiple  sine-functions at higher frequencies. Therefore, the Figure 10  shows the spectral analysis of the time resolved response of al  POIs investigated. In this graph POI 1 shows the lowest  thermal response at higher frequencies over approximately  10 Hz. This is caused by the thicker MC the thermal wave has  to pass and hence at POI 1 the thermal wave is more damped (especially at higher frequencies) till it reaches the surface of  the device in this area.


Figure 10: Spectral analysis of the measured thermal response of the  LIT system with 0.5 Hz of all POIs using the Multi-Harmonic  approach


In a second step the LIT measurement results of POI 1, 2 and  3 with a lock-in frequency of 5 Hz were analyzed using Multi  Harmonics (see Figure 11). With the use of these  measurement data a good correlation between LIT  measurement and Multi Harmonics analyses could be realized  till a lock-in frequency of about 25 Hz.


Figure 11: Comparison of the results of the LIT measurements and  the Multi Harmonics analyses @5 Hz for POI 1, 2 and 3


The recorded time signal for 5 Hz is shown in Figure 12. In  contrast to the 0.5 Hz signal behavior the dampening of the  higher frequency is so high, that only the basic harmonic  signal and two higher harmonic frequencies can be measured. In this case, additional analyses with Multi-Harmonics cannot  yield in further information >25 Hz.


With the advent of stacked-die architecture came novel  challenges for failure analysis engineers. Before analysis could  begin, the failure now had to first be isolated to one die. Afterwards, options were limited by the fact that nodal  analysis and top-side global isolation were reserved for the top  die while back-side analysis was only available for the bottom  die. Even after the analysis reached a point in which the  investigation was to continue on one die, existing techniques  proved insufficient since the dies did not readily separate with  chemicals or heat and was built very thin and was prone to  shattering [3].


These challenges in failure analysis created a need for a more  reliable, systematic method to ensure the physical isolation of  a die for further investigation. Following experimentation  across two different stacked-die devices with disparate  technologies and package types, a reliable set of procedures  were created that allowed for the isolation of the top or bottom  die.  In this paper, the procedures for physically isolating the  top die will be detailed first, then a modified method will be  introduced to successfully isolate the bottom die. Note that  illustrations and optical images of the two devices are detailed  of each step in order to aid the reader’s understanding. Afterwards, limitations of the existing technique will be  disclosed and possible future applications illustrated before  closing.


Figure 1: Decapsulated device images of ‘A’ (top) and ‘B’ (bottom).


Figure 2: Profile-view x-ray images of ‘A’ (top) and ‘B’ (bottom).


Top-Die Isolation


Once electrical testing isolates the location of failure to the top  die, the bottom die may need to be removed with the use of  chemicals to be able to secure the top die for further  examination. Before the use of chemicals, however, the bulk  silicon of the bottom die has to first be exposed. Note here that  the rest of the package should be kept intact to ensure that the  top die will be protected by the mold compound throughout  the following steps. The method to expose the bulk silicon of  the bottom die may involve parallel lapping or laser ablation  depending on the package type, tool availability and analyst  preference.


Following the exposure of the back-side of the bottom die, a  wet chemical etch consisting of hydrofluoric acid (HF) and  fuming nitric acid can be used to etch away the bulk silicon. The analyst can use a pipette to apply a few drops of this  mixture to cover the bulk silicon of the bottom die at room  temperature. A bubbling reaction will take place as soon as the  mixed acid makes contact with the silicon. This should only  last several seconds, and the sample should be rinsed off using  an acetone squirt bottle and dried before applying more of the  chemical etch. This process should be repeated until no silicon  remains. An optical microscope can be utilized here to observe  the progress. Experimentation has shown that this step takes  between 5 to 10 minutes depending on the bulk silicon  thickness. Note that the metal and oxides that remain of the  bottom die act to protect the top die from the wet chemical  etch and the analyst should note the technology node (presence  of dummy metal, number of metal layers and density of the  lines) to avoid the chemical from reaching the top die.


Once the bulk silicon of the bottom die is removed, the rest of  the sample can be placed in a fuming nitric acid bath at 80°C. This will remove the mold compound of the package as well as  the remaining metal and oxides that remain of the bottom die, leaving only the top die to be retrieved for further failure  analysis. Refer to figure 3 for illustrations and optical images  of this process.


Figure 3: Illustration (top) and optical images of ‘A’ (left) and ‘B’ (right) at every step of the procedure to physically isolate  the top die.


Figure 4: Illustration and optical images of ‘A’ (left) and ‘B’ (right) at every step of the procedure to physically isolate the  bottom die.


Bottom-Die Isolation


If the failure was instead electrically isolated to the bottom die  of the stack-die package, a modified procedure can be  employed to extract the bottom die. The revised method uses a  combination of parallel polishing and chemicals to  systematically strip away the top die as illustrated in figure 4.  First, the sample must be polished from the top side of the  device to expose the bulk silicon of the top die. Many methods  are possible to achieve this, but in this particular case study, the sample was encapsulated and parallel-lapped to accomplish  this step. For ease of handling, ensure that the sample is  encapsulated in a thick layer of epoxy. Note that  experimentation showed a clear trade-off in time between this  step and the next, so it is important for the analyst to gauge  his/her parallel lapping skills to determine the time to be spent  on each step.


Once only a thin layer of the bulk silicon of the top die  remains, a chemical mixture consisting of HF, fuming nitric  acid and acetic acid can be used to etch away the silicon. Note  that the sample should be freshly lapped before proceeding to  this chemical step in order to prevent native oxide growth on  the device. The analyst should be warned about the destructive  nature of this wet chemical silicon etch since it has been  observed that the glass fillers in the mold compound, die attach  and passivation layer of the bottom die was eventually etched  away with time. Once the bulk silicon of the top die is etched  away, transparent die attach may act as a window to show part  of the bottom die.  Note that the mold compound covering the  bottom die acts as a barrier to protect it from this chemical  step.


After only the bottom die and mold compound of the device  remains in the encapsulation, the sample can be placed in a  fuming nitric acid bath at 80°C to remove the rest of the  package. It is highly recommended that any excess  encapsulation be removed before the acid bath using a saw to  expedite this process.


Despite the reliable nature of the process described, there are  several limiting factors of the procedures to be discussed. As  evident, this method can only physically isolate one die at the  cost of the other. Hence, it can only be applied to situations in  which the failure has already been narrowed down to one of  two dies. For this reason, it is imperative for the test solution  of the device to have the capability to narrow down the failure  to one of the die in the multi-chip module.


Another limitation of these procedures is the destructive nature  of the mixed-acid silicon etch recipes. Experimentation has  found that the mixture will eventually attack the glass fillers in  the mold compound, the transparent die attach, oxides and the  passivation layer of a die. For example, if the etch was  intended for etching away the bulk silicon of the bottom die to


physically isolated the top die, depending on the technology  node (presence of dummy metal, number of metal layers and  metal density), the silicon etch may eventually etch away the  ILO (Inter-Level Oxide) and passivation layer of the bottom  die to reach the backside of the top die. In addition, it must be  noted that the wet chemical etch consisting of HF, fuming  nitric acid and acetic acid may not be suited for dies with SOI (Silicon On Insulator) processes since the formula is not  optimized to etch oxides.  To prevent unintended damage, the  silicon etch formulas should be experimented on several  devices before proceeding with the actual failing device of  interest.


Future Applications


With the successful application of two-die stacked-die  packages in the semiconductor industry, came configurations  with three or more stacked-die in a package. Due to its  systematic nature, the presented methodologies should  theoretically allow for the physical isolation of any one of the  dies on any future products. To demonstrate, the application of  the procedures on a three-die stacked-die package will be  presented below.


If the top die needed to be physically isolated from the threedie stacked-die package, the sample has to first be  encapsulated and parallel polished from the back-side until the  bulk silicon of the middle die is exposed. At this step, a wet  chemical silicon etch (HF and fuming nitric acid) can be used  to etch away the bulk silicon of the middle die, leaving only  the metal lines and oxides. Afterwards, the rest of the sample  can be placed in a fuming nitric acid bath at 80°C to retrieve  the top die.


If the die of interest was, instead, the bottom die, the device  can once again be encapsulated and parallel lapped from the  top-side until only a thin layer of the bulk silicon of the middle  die remains. Then, a wet chemical silicon etch (HF, fuming  nitric acid and acetic acid) can be utilized to etch the  remaining bulk silicon away from the middle die and the  sample can be placed in a 80°C fuming nitric acid bath to  recover the bottom die.


The trickier situation is the one in which the middle die has to  be extracted. However, due to the systematic nature of the  methods developed, the combination of the first and second  procedures should theoretically allow for the extraction of the  middle die as well. The first step is to expose the bulk silicon  of the bottom die and use a silicon etch mixture (HF and  fuming nitric acid) to etch away the bulk silicon. Then, the  sample can be encapsulated and parallel polished from the topside of the device until only a thin layer of the bulk silicon of  the top die remains. Again, a wet chemical etch (HF, fuming  nitric acid and acetic acid) can be utilized in this step to etch  away the rest of the bulk silicon. Then the rest of the sample  can be dropped in a 80°C fuming nitric acid bath to boil away  the rest of the package and the remainder of the other two dies  to retrieve the middle die.


As illustrated above, in theory, the procedures drawn in this  paper can be directly applied to extract any one of the dies in  future stacked-die configurations that may include three or  more die. Due to the reliable, systematic nature of the  methodology developed, it will prove to be relevant in years to  come.


The prevalence of stacked-die packages created a novel  challenge for failure analysis engineers. To tackle the  difficulties of physically isolating the die of interest, a set of  procedures were developed to reliably retrieve the top or  bottom die of the package. Several limitations were addressed  for the benefit of the reader and the relevance of the  methodologies to future products described in theory. Because  of the reliable, systematic nature of the process, the procedures  should remain relevant with future renditions of the  configuration to come.


The authors would like to thank Texas Instruments for  providing the environment in which to pursue our research.


[1] Vardaman, E.J.; Matthew, L., "New developments in  stacked die CSPs," High Density Microsystem Design and  Packaging and Component Failure Analysis, 2004. HDP '04. Proceeding of the Sixth IEEE CPMT Conference on , vol., no., pp.29,30, 30 June-3 July 2004.


[2] Black, B.; Annavaram, M.; Brekelbaum, N.; DeVale, J.; Lei Jiang; Loh, G.H.; McCauley, D.; Morrow, P.; Nelson, D.W.; Pantuso, D.; Reed, P.; Rupley, J.; Sadasivan Shankar; Shen, J.; Webb, C., "Die Stacking (3D) Microarchitecture,"Microarchitecture, 2006. MICRO-39. 39th  Annual IEEE/ACM International Symposium on , vol., no., pp.469,479, Dec. 2006.


[3] Malachowski, K.; Gonzales, D.; Miller, R. A; Schnegg, F.; Arzberger, A; Hajdarevic, Z.; LaManna, A, "An investigation  into damage-free thin die pick and place for 3D  stacking," Electronics Packaging Technology Conference (EPTC), 2011 IEEE 13th , vol., no., pp.819,823, 7-9 Dec.


Evaluation of TEM-Lamella Oxidation


Thomas Haber


ams AG, Unterpremstaetten, Austria


Thomas.Haber@ams.com, +43313650032228


Christian Gspan


Institute for Electron Microscopy and Nanoanalysis, Graz University of Technology, Austria   christian.gspan@felmi-zfe.at, +433168738324


This study investigated the origin of detrimental high ohmic  behavior of contacts by means of analytical electron  microscopy. The root cause for the high resistivity could be  identified as delamination of the contact bottom in the  nanometer range. Based on the results, we were able to  establish a method to identify thin oxide layers using analytical  methods without being able to spatially resolve them in a  combined focused ion beam instrument and scanning electron  microscope.


High ohmic contacts are a significant problem for  semiconductor devices. Such contacts are typically  investigated using a dual-beam focused ion beam and scanning  electron microscope instrument (FIB/SEM, referred to as FIB  in the following) for lamella preparation [1] followed by  analytical transmission electron microscopy (TEM) [2, 3] to  obtain high resolution images accompanied by chemical  information from the bottom contact interface which is a stack  of tungsten plugs (contact material), TiN/Ti (liner) and  TiSi2/Si (substrate). An unexpected detrimental oxide layer  between the contact and the silicon is regularly observed when  analyzing high ohmic contacts. This oxide layer is believed to  cause the high resistivity. However, the question of the root  cause cannot be answered, since the observed layer can be  explained by two competing theories. Either this is an oxide  layer evolving during the manufacturing process in the wafer  fabrication facility (the FAB) or it is an oxidation of a  delamination that takes place during the transport of the TEM  lamella to the microscope.


The following experiment was set up to answer this question. A FIB equipped with a scanning TEM (STEM) option and an  energy dispersive x-ray spectrometer (EDXS) was used to  perform analytical measurements in-situ, thus avoiding the  exposure of the lamella to air and therefore preventing  oxidation. If an oxide layer is identified with this  measurement, then it can be attributed to evolution during the  FAB process.


However, not detecting this layer is not equivalent to its  absence. Since the dimensions of the regions of interest are in  the nanometer range it is not clear if the instrument detection  limits have been reached. Thus, a present oxide layer simply  may not be detectable with the FIB.


Assuming that no oxide layer is observed in the in-situ  experiment with the FIB, the lamella was to be further  investigated with a dedicated STEM equipped with an electron  energy loss spectrometer (EELS), allowing for quantitative  chemical composition analyses. With the latter, even the  numbers of atoms under the beam can be calculated. With this  information the lamella was to be transferred back to the FIB  where the initial in-situ measurements would be repeated. If  the oxide layer can be detected at this stage, it can then be  ascribed to oxidation of the lamella. Together with the  quantitative results, conclusions can be drawn as to whether  the observed oxidation is surface oxidation of the lamella or  oxidation through the lamella appearing as the suspicious  oxide layer. In the case where the oxide layer can be detected  after the exposure to air, but is not observable in the in-situ  measurement, the root cause for the high ohmic contact can be  identified as delamination rather than oxidation during  fabrication. As a convenient side effect, the detection limits for  the EDXS used in this FIB can be estimated.


FEI NanoLab 650 FIB operated at an electron energy of 30  keV (for STEM) equipped with an Oxford 80 mm² EDXS  system. This system was also used for the lamella preparation. FEI Titan STEM operated at 300 keV equipped with a SuperX EDXS detector and a GATAN imaging filter Quantum with  ultra-fast shutter allowing for dual energy range EELS (DualEELSTM) measurements in STEM mode.


For EELS quantification the software DigitalMicrographTM by  GATAN, Inc. was applied.


Experiments


Test structures with single contacts were prepared allowing for  resistance measurements for each individual contact. Some  contacts showed a significantly higher resistance than others.


TEM lamellas of these contacts were prepared as seen in Fig. 1  which is a superposition of a FIB image and the layout. The  red squares represent contacts, while the metal lines and the  active area are represented by bright green lines and a dark  green square, respectively. Typically the lamellas were thinned  from the substrate side down to several tens of nanometers  which is required for reasonable EELS measurements later on.


Figure 1: Superposition of a FIB image and the layout of the  test structure in small red boxes (contacts), bright green lines (metal 1) and dark green box (active).


The specimens were investigated in-situ in the FIB directly  after preparation using STEM and EDXS. A STEM image  from the FIB is shown in Fig. 2, where the tungsten contact  appears on the left side (black) and the substrate on the right  side. No suspicious details can be identified and, due to the  limited spatial resolution of the equipment, the interface  cannot be resolved.


Figure 2: STEM image taken in-situ in the FIB; the white line  indicates the line scan across the interface from the contact (black) to the substrate.


Nevertheless, EDXS line scans were performed across the  interface as indicated by the white line in Fig. 2. Results are  presented in Fig. 3, showing the intensity changes of the


individual characteristic peaks along the line scan. Although  the spatial resolution of the titanium layers is not possible, they  are clearly identified by the EDXS measurements (pink line in  Fig. 3). Furthermore, there is no distinct rise in the oxygen  intensity observed. This means that an oxide layer cannot be  identified with in-situ measurements; not proving its absence, though, as explained above.


Figure 3: EDXS line scan across the contact-substrate  interface as indicated in Fig. 2. The relevant elements are  plotted according to the counts of the EDXS signal.


Both the good and the bad contacts give the same results, not  allowing for any conclusions. Therefore, the samples were  further investigated using a high resolution STEM, as shown in  Fig. 4.


Figure 4: a) STEM image of a high ohmic contact and b) a  zoom in the contact-substrate interface. An unexpected bright  layer is observed (indicated by a red arrow) which is located  between the Ti and TiSi2 layers.


A stack of layers at the bottom interface was observed. The  stack is identified as tungsten (top, dark), TiN, Ti, an  unidentified bright line, TiSi2 and crystalline silicon with its  atomic structure. According to the fabrication process the  suspicious bright layer (red arrow in Fig. 4b) cannot be  explained. Furthermore, this layer is only observed with  respect to high ohmic contacts and is not observed at good  ones. Therefore, the high resistance is reasonably attributed to  this layer.


Figure 5: EELS line scan data (edge intensities) for titanium (blue, top), nitrogen (green, middle left) and oxygen (red, center.)


The layer stack was analyzed with STEM/EELS line scan  measurements as shown in Fig. 5. The line scan is performed  from the contact on the left side to the substrate on the right  side and confirms the expected layers (TiN, Ti, TiSi2) accompanied by an additional oxide layer as seen from the  intensity profile of the oxygen edge (red line). This layer  correlates with the bright layer as it is located between Ti and  TiSi2.


For quantification, EELS spectra are drift corrected, background subtracted, and multiple scattering deconvoluted. For this purpose the line scan was performed in dual EELS  mode, allowing for recording the high loss and the low loss (zero loss) spectra simultaneously. Spectra of TiN, TiSi2 and  Ti of the measurement above are shown in Fig. 6 in green (top  right), red (bottom right) and blue (middle right), respectively. The layers can clearly be distinguished based on their spectral  finger print.


Figure 6: Obtained EELS spectra of the individual layers after  post processing.


Based on these results, spectra from each point of the line scan  are taken for quantification. The results are presented in Fig. 7  showing the layers TiN, Ti, TiO2 and TiSi2. The suspicious  layer is located where the detected dark field intensity (DF) is  low whereas the oxygen content is high. The oxide content at  other areas than the gap is ascribed to lamella surface  oxidation. However, it is clearly observed that the oxygen  content in the gap is higher than in the direct vicinity, thus  exceeding the amount of lamella surface oxidation, proving the  presence of an oxide layer.


Figure 7: Relative composition along the line scan  superimposed with the dark field detector signal (grey). Lines  are nitrogen (green, middle left), oxygen (red, top center), and  titanium (blue, bottom center).


Fig. 8 presents the calculated areal density which is dependent  on the atoms*nm-2. The knowledge of the zero-loss intensity  for each recorded high-loss spectrum allows for the calculation  of the atoms*nm-2 we are looking at. The number of atoms at  the maximum of the oxygen content was calculated to be 5000  atoms*nm-2, though with an estimated error of 50 %.


Figure 8: Obtained EELS spectra of the individual layers after  post processing. Lines are nitrogen (green, middle left), oxygen (red, top center), and titanium (blue, bottom center).


Figure 9: EDXS spectra of the interfacial area recorded in the  FIB; yellow: in-situ measurement; blue: after exposure to air.


With these results the lamellas are again investigated in the  FIB to get comparable results to the in-situ measurements. First, an EDXS scan of an area as shown in Fig. 4b was  performed and compared to the same measurement recorded  in-situ, directly after preparation. This is presented in Fig. 9, where the oxidation of the lamella is clearly identified by the  rise of the oxygen peak after exposure to air (blue spectrum).


Figure 10: EDXS line scan across the contact-substrate  interface as indicated on the top image. The relevant elements  are plotted according to the counts of the EDXS signal.


To be able to distinguish between lamella surface oxidation  and the oxide layer an EDXS line scan was performed that is  shown in Fig. 10. In contrast to the in-situ measurement, there  is a clear increase of the oxygen signal observed at the position  of the gap. This increase is detected although the layer cannot  be spatially resolved in the FIB.


The analytical quantitative results obtained from the in-situ  results (Fig.3) when contrasted with the subsequently recorded  EDXS results as shown in Fig. 10 suggest that for single point  measurements in the FIB the detection limit is below 5000  atoms*nm-2, as this is the number from the EELS analysis. This number clearly exceeds the number expected for pure  surface oxidation of the lamella. More importantly, the spatial  rise of the oxygen content shows that the oxygenated layer is  detectable and can be identified using FIB measurements only. As this layer cannot be detected during in-situ measurements, it is clear that the high ohmic behavior of the contact can be  assigned to a delamination between Ti and TiSi2.


This conclusion is corroborated by the fact that the relative  oxygen content exceeds the stoichiometric content of TiO2 at  the interface to TiSi2, as can be seen in Fig. 7. This suggests  that there are dangling oxygen atoms from a TiO2 surface  pointing into the gap. These dangling atoms are typical for an  oxidized Ti surface, thus leading to the same conclusion that  the initial gap is oxidized during lamella exposure to air.


With this experiment the high ohmic behaviour can be  assigned to a delamination of the contact bottom taking place  between the Ti and the TiSi2 layer. The observed oxide layer  can be attributed to the sample preparation and the following  exposure to air.


Furthermore, the detection limit for our FIB was determined to  be less than 5000 atoms*nm-2. This enables the detection of  layers down to 1 nm with the EDXS system even if they  cannot be resolved spatially. Based on this information  suspicious interfaces will be investigated routinely by EDXS  prior to air exposure and subsequent investigations.


The Authors want to thank Prof. Ferdinand Hofer, head of the  Institute for Electron Microscopy and Nanoanalysis, for  granting us access to the ASTEM to perform the  investigations.


[1] Giannuzzi, L.A. and Stevie, F.A., Introduction to Focused  Ion Beams, Springer (Cambridge, U.K. 2004).


[2] Williams D.B., Carter C.B., Transmission Electron  Microscopy, Plenum Press (New York 1996)


[3] Egerton R.F., Electron Energy-Loss Spectroscopy in the  Electron Microscope, 2nd ed. Plenum Press, (New York  1996)


Spectrum Sharpening on Rotation Averaged TEM Nano Beam  Electron Diffraction Patterns


Yongkai Zhou*, Younan Hua and Xiaomin Li


WinTech Nano-Technology Services Pte. Ltd., The Alpha Singapore Science Park II, Singapore 117684   Email: yongkai@wintech-nano.com


The Rotation Averaged Spectrum of TEM diffraction patterns  can be sharpened by a Maximum-Likelihood deconvolution  algorithm. The sharpened spectrum will help to improve the  precision of TEM diffraction-based techniques, e.g.: phase  identification and strain analysis.


TEM diffraction is a commonly used method for material  structure analysis. When it comes to nano-scale structure  analysis; e.g. nano-sized phase identification or nano scale  strain analysis, the traditional Selected Area Diffraction  Pattern (SADP) method is no longer working, because the  spatial resolution of SADP is limited by the smallest aperture  size, which is about 300nm in many TEM machines. On the  other hand, TEM Nano Beam Electron Diffraction (NBED) has obtained superior spatial resolution for material structure  analysis and phase identification. The NBED uses a slightly  converged electron microprobe to achieve about 3nm spatial  resolution. In some state-of-art TEM machines; e.g., the FEI  Titan TEM, the convergence angle of the electron microprobe  can be as low as 0.23 mrads. With such small convergence  angle, the size of the diffraction spot is almost as sharp as the  parallel beam diffraction method; e.g., SADP. However, for  lower-end TEM machines; e.g., the FEI Tecnai TEM, the  electron microprobe convergence angle could be as large as 2  mrads, which makes the diffraction spots into small disks  instead of sharp points (see Fig. 1 (a) and (b)). This would  affect the precision of the structure analysis. In this work, we  have developed a new method to sharpen the NBED patterns  obtained by the Tecnai TEM. This study could give  researchers the opportunity to do some advanced analyses  using “cheaper” TEM machines.


Experimental Procedure


TEM lamellas were prepared by Focused Ion Beam (FIB) milling in a FEI Helios 600i machine at a 30 kV ion beam  voltage. NBED analysis was performed under Scanning-TEM (STEM) mode using an FEI Tecnai F20 TEM equipped with a  Schottky FEG source. The beam setting was switched to  Microprobe mode instead of the Nanoprobe mode that was  used for normal STEM. Gun lens 6 and spot size 7 were


adopted in the Microprobe STEM. A 10um diameter  Condenser 2 aperture was used to get a nearly-parallel electron  probe of small semi-convergence angle, which is estimated to  be around 2mrad. The method of estimating the convergence  angle has been described elsewhere [1]. The NBED pattern  was converted into a Rotation Averaged Spectrum (RAS) using the DiffTools plug-in package [2] in  DigitalMicrographTM.


Figure 1: Diffraction patterns of single crystal silicon viewed  along the <011> zone axis: (a) Selected Area Electron  Diffraction (SAED), and (b) Nano-Beam Electron Diffraction (NBED).


The final trials used a non-contact solder excavation combined  with semi automated ball placement.  Excavation (Figure 13) was performed using the VJ Electronix Micra rework system. A thermal cycle was chosen which adequately melted the  solder yet maintained a peak package temperature below 250° C. The BGA was placed into a fixture with the solder balls  facing up.  The solder scavenger was positioned 0.12 mm  above the BGA body using the systems height sensor, and was  traverse in a “S” shaped pattern to remove the solder. (Figure  12).


Figure 12 – Solder Excavation Thermal Parameters


Figure 13- Solder scavenging method after deballing


Once the solder was removed, the semi automated reballing  process was performed as previously described.


Results and analysis  Design of Experiments Results


There were three different deballing methods investigated in  order to determine the temperature of the BGA die. These  methods were the: non-contact solder excavation, solder  fountain (miniature wave) and a soldering iron and desoldering  braid methods. Small 5mil ball end thermocouples were  embedded in to the die in order to determine if a thermal


excursion had been experienced by the component. Both the  solder excavation (peak average 240ºC) and the solder  fountain methods (peak average 230ºC) triggered a  temperature which was above that a reflow temperature with  the solder excavation process having the highest peak  temperature (260ºC) for the longest period of time of the  methods investigated. In the case of the solder wick method  the reflow temperature was not reached with the average peak  temperature being 190ºC. (Note: Due to difficulties in  fixturing, the solder fountain method was not used in the final  reballing study).


After deballing and cleaning there were a few visual anomalies  noted  on the reballed parts.


X-ray Inspection


In the same manner, there were a few anomalies observed  during x-ray inspection. The parts were inspected with an  automated BGA analysis routine using a VJ Electronix Vertex  140kV plate voltage x-ray system. The analysis was executed  on the x-ray tool to look for typical parameters including  solder ball area, circularity, and voiding.  The BGA was  divided into nine regions of interest (Figure 14) to provide  adequate magnification.


Figure 14 - X-ray image of BGA (low magnification) highlighting


one of five regions of interest.


Several parts were examined via x-ray both pre and post  reballing. Figure 15 is one of the images seen prior to


Figure 15- Image of BGA prior to solder ball removal


reballing. There were no anomalies noted on this as well as  other images prior to reballing. After reballing the parts were  again x-ray inspected. Figure 16 below is typical of some of  the images generated during this investigation. Using the  integrated x-ray software the ball diameters of the reballed  components were measured as were the voiding percentages. The results are summarized in Table 17.


Figure 16- Image shows two minor voids (<10%) post reballing


Baseline


WickManual Wick-Auto


ScavengeAuto


Area


0.0228


0.0240


0.0244


0.0236


Area Std Dev


0.0010


0.0012


0.0011


0.0013


% Deviation


2.99


3.74


4.21


4.26


Circularity


1.19


1.21


1.20


% Void


0.00%


0.24%


0.26%


0.07%


Max Void %


9.17


10.55


2.92


Figure 17- XRAY Results after Deballing


Shear Strength Comparison


A ball shear test was performed on samples from each of the  three methods using a Keller Technology Corp model


Bondtest 30 (Figure 18 and 19).  Balls were sheared at a speed  of 0.42 mm/sec (Slow speed per JEDEC JESD22B117A).


The shear test data shows very consistent range (standard  deviation) with the control sample and all methods (Figure 20) 100% of balls tested exhibited the desired ductile fracture (fracture occurs above the interface within the bulk of the  solder sphere).  There were no cases of the undesired  pad or  ball lifting or interfacial breaking.


The mean shear strength varied slightly between methods with  the solder wick/ manual reball method yielding the greatest  strength.


Figure 18- Ball Shear Test Instrument


Figure 19- Ball Shear Test Instrument – force transducer


Figure 20- Shear Test Results


All methods investigated in this study, both for deballing and  ball re-attachment are viable process options for manual  reballing of smaller packages.  Tests indicate minor variations  in consistency via coplanarity, ball diameter and mechanical  integrity of the solder joint via shear testing.


For the deballing of these uBGA packages (2) of the (3) solder  excavation methods drove the devices in to a thermal  excursion. Only the soldering iron and wick method did not  send the device above this temperature threshold. This may  lead to higher reliability of devices deballed in this manner. When using the solder wick deballing process and the semiautomated BGA reballing process, a greater volume of flux  and a 10 degree increment in reflow profile was required when  compared with the solder excavation deballing process. This  increased temperature may lessen the reliability of the die.


The reballing process resulted in addition of very minor  voiding as evidenced in x-ray measurements.  The excavation  and semi-automated ball reattachment process resulted in less  voiding, which we attributed to the reduced flux application  required in the Nitrogen environment. While the sample size  of the various reballing techniques investigated was limited, there were no noted yield detractors, one method versus  another.


This shallow dive in to the reballing of ultra fine-pitched  package processes indicated that there are numerous methods  available to users for ultra fine pitch manual reballing. The  fastest deballing technique was the solder fountain technique  with the caveat being the potential to dissolve the copper if the  fountain is too hot or the immersion time too long. The ball  reattachment technique with the fastest cycle time was the  manual solder preform technique.  The choice of process  should be made on access to automated equipment, the  skill  level of technicians and the total cost inclusive of time and  materials.


We would like to thank the following individuals and  organizations for their contributions:


Don Naugler and Adam Brooks – VJ Electronix Engineering  Technicial – Micra System profile generation and operation


Custom Analytical Solutions, 50a Northwestern Drive, Salem  NH 603-898-7074 (Ball Shear tesing)


Tammy Grefkowicz and Hung Hoang of BEST for their work  on processing the devices and taking the pictures


[1] Meschter, S.J., McKeown, et el , “BGA Re-Balling from  PB-Free to Sn-Pb Mettalurgy”, SMTAI 2010 Proceedings


[2] Nie L, Osterman M, Pect M, Somg F ete el, “Solder Ball  Attachment Assessment of Reballed Plastic Ball Grid Array  Packages, IEEE Trans . Components and Packaging  Technology, Vol 32, N0 4, December 2009, pp 901-908.


[3] Robert Kinyanjui and Quyen Chu, “The Pb-free SnAgCU  Ball Grid Array (BGA) Components in SnPb Assembly  Process”, Proceedings of Apex 2008, S15-02, Las Vegas, NV


2008.


[4] I Chatterji, “Backward Compatibility, Are We Ready-A  Case Study,” Proceedings of SMTAI, Chicago, IL 2006.


[5] Coyle, R, Meilunas, M., Popwich, R., et el “Interconnection Reliability of Interposer and Reballing  Options for Ball Grid Aray Backward Compatability”, Proceedings of SMTAI, Dallas, TX 2010.


A comprehensive investigation of the galvanic corrosion induced Ag-Al bond  degradation in microelectronic packaging using Argon Ion Milling, SEM, Dual  Beam FIB-SEM, STEM-EDS and TOF-SIMS


Yixin Chen, Emmanuel Simon, Bing Sheng Khoo, Esther Lee, Meailing Chooi, Meng Hao, Jingjing Shao, Younan Hua and Xiaomin Li


WinTech Nano-Technology Services Pte. Ltd.


10 Science Park Road, #03-26 & #03-28, The Alpha, Singapore Science Park II, 117684, Singapore  yixin@wintech-nano.com, (65) 81817526


It is known that Ag-Al bonds have strong tendency to degrade  due to excessive interdiffusion and to oxidize in the presence  of contaminants such as the moisture and corrosive ions, hence  form a risk for both the bonding quality and the reliability of  microelectronic devices [1]. However, people seldom carry out  an in-depth analysis of the microstructural and the chemical  information in the degraded Ag-Al bond and investigate the  bond degradation mechanism in a packaging module. In this  study, a comprehensive investigation of the Ag-Al bond  degradation mechanism in an electrically failed module using  the Argon Ion Milling, Scanning Electron Microscopy (SEM), Dual Beam Focused Ion Beam-Scanning Electron Microscopy (FIB-SEM), Scanning Transmission Electron MicroscopyEnergy Dispersive X-ray Spectroscopy (STEM-EDS) and  Time-of-Flight Secondary Ion Mass Spectrometry (TOFSIMS) is reported. It is found that the bond degradation is due  to the galvanic corrosion in the Ag-Al bonding area. Specific  attention is given to the information of microstructures, elements and corrosive ions in the degraded bond. Moreover, since obvious micro-delaminations were observed between the  moulding compound and the Ag plated lead frames at the edge  of the fresh module without any bond degradation, it is  suspected that the micro-delamination acts as a potential path  allowing the moisture and the corrosive ion Cl- to seep in and  attack the bonding area, leading to the galvanic corrosion in  the Ag-Al bonding area. Eventually, the bond was detached  due to the Cl- accelerated galvanic corrosion. Comparing the  analytical results at two lead locations in the same packaging  module, it is believed that the bond degradation is highly  related to the packaging designs.


An electrically failed microelectronic packaging module  showing an open failure and a fresh module without any  failure, which has exactly the same structure as the failed one, were investigated and compared. A schematic illustration of  the module is shown in Fig 1. Al wires bonded to Ag plated  lead frames are used in the packaging module.


After laser decapsulation, bond detachment in all wires on  lead1 has been found in the failed module. For comparison, bond 1, bond 2 in the failed module and bond 1 in the fresh  module were comprehensively characterized using the Argon


Ion Milling, SEM, Dual Beam FIB-SEM and STEM-EDS. Furthermore, the possible low concentration of corrosive ions  at the bonding interface in the failed module after laser  decapsulation was studied using the TOF-SIMS surface  analysis.


Figure 1: A schematic illustration of a part of the module in  which Al wires bonded to Ag plated lead frames are used. The  Al wire and lead frames are pointed out by red arrows. In this  study, the two bond locations of interest (bond 1 and bond 2) are marked by red circles while corresponding leads (lead1  and lead 2) and pins (pin 1 and pin 2) are indicated.


Argon Ion Milling sample preparation and SEM Imaging. An  overview of the bonding was investigated by the SEM imaging  on the Argon Ion Milling prepared samples. The ion milling  has been treated as an alternative to Focused Ion Beam (FIB) for studying wide area cross sections of intermetallics (IMCs)


[2]. In addition, avoiding any artefacts such as scratches, smearing, wash out and delamination induced by the  mechanical polishing technique, the ion milling could be the  best method for preparing cross sectional samples having the  potential bond degradation. The low energy and wide area  Argon Ion Milling was used to obtain the large cross sections  of the whole bonding area for bond 1 in the fresh module, bond 1 in the failed module and bond 2 in the failed module. The overview cross sectional SEM image of bond 1 in the  fresh module, bond 1 in the failed module and bond 2 in the  failed module are shown in Fig 2 a, b and c (The SEM is  operated at 15kev). In the failed module, the delamination  between the Ag layer and the Al wire/moulding compound was  found, while abnormal features at the bonding interface  indicating the possible corrosion behaviour were observed.


Figure 2: The cross sectional SEM images of a) bond 1 in the  fresh module b) bond 1 in the failed module; c) bond 2 in the  failed module.  The sample was prepared by the wide area  Argon Ion Milling.


In order to check the bonding quality of the three bonds, zoom  in cross sectional SEM images around the centre of the  bonding area for bond 1 in the fresh module, bond 1 in the  failed module and bond 2 in the failed module were taken (Fig  3a, b and c). For both bond 1 in the fresh module and bond 2  in the failed module, the IMCs were well formed. No bond  degradation was observed for bond 2 in the failed module, whereas for bond 1 in the failed module, an obvious bond  degradation was observed.


Al


Cu


Ag


IMCs


delamination


Al wire


Ag plated Cu lead frame  moulding compound


Ag plated Cu lead frame


moulding compound


c)


Figure 3: Zoom in cross sectional SEM images around the  centre of the bonding area for a) bond 1 in the fresh module b) bond 1 in the failed module; c) bond 2 in the failed module. All three samples were prepared by the wide area Argon Ion  Milling.


Dual Beam FIB-SEM sample preparation, STEM Imaging  and STEM-EDS Analysis


Detailed microstructures and elemental information were  obtained from the Dual Beam FIB-SEM prepared lamella  samples using the STEM imaging and STEM-EDS analysis.


Since the spatial resolution of the SEM is limited by the  electron spot size and the interaction volume, in order to give  an in-depth microstructure and element information in the  bonding area, the STEM operated at 200kev was used to reach  a higher resolution. One cross sectional STEM lamella was  prepared around the centre location shown in Fig. 4a of the  bonding area for bond 1 in the fresh module and two cross  sectional STEM lamellas were prepare at two locations shown  in Fig. 5a in the delamination area of the failed module using  the in situ lift-out method in the Dual Beam FIB-SEM. Then, the STEM imaging and STEM-EDS analysis were used to  analyse the details in the bonding area. Based on the STEM  observation and EDS line profile analysis shown in Fig 4b, for  bond 1 in the fresh module, stable phases of the Ag-Al IMCs  were formed, indicating a good quality of the Ag-Al bond. Whereas, based on the STEM observation and STEM-EDS  mapping analysis shown in Fig 5b and c, for bond 1 in the  failed module, a delamination was observed in the bonding  area. The Al in the bonding area was oxidized and swollen, forming a porous structure, while Ag precipitates were  separated from the IMCs and nearly no more IMCs were  observed. All these observations indicate that the severe  galvanic corrosion occurred in the bonding area.


Figure 4: a) The cross sectional SEM image around the centre  of the bonding area for bond 1 in the fresh module with the  TEM sample preparation location indicated. b) The STEM  image and STEM-EDS line profile of the IMCs for bond 1 in  the fresh module. The STEM lamella was prepared by the in  situ lift-out method using the Dual Beam FIB-SEM.


IMC


EDS line  profile  location


TEM  location


Figure 5: a) The cross sectional SEM image around the centre  of the bonding area for bond 1 in the failed module with two  TEM sample preparation locations indicated. b) The STEM  image and STEM-EDS mapping result at location 1. c) The  STEM image and STEM-EDS mapping result at location 2.


TOF-SIMS Surface Analysis


Since the concentration of some corrosive ions could be below  the STEM-EDS detection limit and STEM sample area is too  localized to detect all information in the wide bonding area, the TOF-SIMS surface analysis, which provides a superior  detection limit (in the range of ppb-ppm),  is used to detect any  possible corrosive ions which might lead to the galvanic  corrosion. Although extensive studies have been done on  corrosion of bond pads using the TOF-SIMS surface analysis


[3], this technique is rarely used for studying the corrosion  behaviour in the bonding area of a packaging module.


The Al wire of bond 1 in the failed module after laser  decapsulation was mechanically pulled off just before the  TOF-SIMS surface analysis to ensure uncontaminated surfaces  of the lead frame and the wire. The TOF-SIMS surface study  using a Bi+ gun under the condition of 25Kev and 1.0pA has  been carried out on the surfaces of the lead, the wire and a  good area (an uncontaminated surface on a fresh module for  reference). As shown in Fig 6, the TOF-SIMS surface spectra  and ion intensities comparison charts show higher level of Cland K+ ions on the surfaces of the lead and the wire, compared  to those of the good area. The Cl- can act as a catalyst for the  galvanic corrosion. Hence, the existence of the Cl- could


TEM


location


location 2


EDS


mapping  location


accelerate the galvanic corrosion in the presence of the  moisture.


Figure 6: TOF-SIMS surface a) ion mass spectra and b) ion  intensities comparison charts for Cl- and K+ ions on the  surfaces of the lead, the wire and a good area (an  uncontaminated surface on a fresh module for reference) for  bond 1 of the failed module. The module has been laser  decapsulated and the Al wire was mechanically pulled off just  before the TOF-SIMS surface analysis to ensure  uncontaminated surfaces.


SEM Imaging on the Micro-delaminations


For investigating a possible path allowing the moisture and  ions to get in, low energy wide area Argon Ion Milling was  used again to obtain a relatively large cross section near to the  edge of lead 1 and lead 2 in the fresh module.  Microdelaminations were observed between the moulding compound  and the Ag plated lead frames at the edge of the module for  both leads.  Zoom in SEM images of the micro-delaminations  were shown in Fig 7a and b. It is supposed that the microdelamination could act as a micro path allowing the moisture  and Cl-   to seep in and gradually attack the bonding area, thus  leading to the galvanic corrosion in the Ag-Al bonding area. Eventually, the bond was detached due to the severe galvanic  corrosion, resulting in an open failure in the module.


Figure 7: Zoom in cross sectional SEM images at the edge of  the fresh module for a) lead 1 and b) lead 2. The sample was  prepared by the wide area Argon Ion Milling. Microdelaminations were observed between the moulding  compound and the Ag plated lead frames at the edge of the  module for both leads.


In summary, the Ag-Al bond degradation mechanism has been  comprehensively investigated using the Argon Ion Milling, SEM, Dual Beam FIB-SEM, STEM-EDS and TOF-SIMS. It is  found that the bond degradation is due to the Cl-   accelerated  galvanic corrosion in the Ag-Al bonding area. Microdelaminations were observed between the moulding compound  and the Ag plated lead frames at the edge of the module for  both lead1 and lead 2 in the fresh module without any failure. The micro-delamination could be a potential micro path  allowing the moisture and Cl- to seep in and gradually attack


micro-delamination


the bonding area, leading to the galvanic corrosion in the AgAl bonding area.  It is notable that there is no bond  degradation observed for bond 2 in the same failed module  although a micro-delamination was observed at the edge of the  fresh module for lead 2. The reason why different results were  obtained from bond 1 and bond 2 in the same module could be  as follows: A) The travel distance for the moisture and ions  between the module edge and the bonding location of bond 2  is longer than that between the module edge and bond 1; B) Compared to the regularly shaped lead 1, the irregular shape of  lead 2 could help to prevent the extension of the microdelamination at certain locations. In this study, it is believed  that the Ag-Al bond degradation is highly related to the  packaging designs.


The authors would like to thank all colleagues who contributed  to this work and the ISTFA 2014 committee members for their  great support.


[1] Michael Pecht  et al., Electronic Packaging Materials and  Their Properties (CRC Press, 1998) pp. 41-42.


[2] Roger Stierman, et al., “Ion Milling as an Alternative to  Focused ion Beam for Cross-Section Intermetallic  Analyses,” Pan Pacific Symposium 2006 Proceedings, Kuala Lumpur, Malaysia, July 2006.


[3] Hua Younan, et al., “A Study on Fluorine-Induced  Corrosion on Microchip Aluminum Bondpads,” Proc29th   Int’l Symp for Testing and Failure Analysis, Kuala  Lumpur, Malaysia, Santa Clara, California, USA, November 2003,  pp. 249-255.


Correlation of Thin Film Measurement Techniques for Device Packaging  Processes


J. Walter*, W. Mack


Infineon Technologies AG, Regensburg, Germany  Juergen.walter@infineon.com


C. Y. Lee


Infineon Technologies Sdn. Bhd., Malacca, Malaysia


C. Gspan


Center for Electron Microscopy (ZFE), Graz, Austria


The analysis of thin layers in semiconductor components  represents a central point in the quality control of  semiconductor companies. Not only to control production  processes, but to successfully operate also reverse engineering, reliable thin-film measurement methods are essential.


In this work, non-destructive thin film EDX (energy dispersive  X-ray micro analysis) software and µXRF (micro x-ray  fluorescence analysis) were compared with TEM analysis. These methods ensure a high lateral resolution which is  essential in the analysis of semiconductor structures.


As an example, four different, for the semiconductor industry  interesting, very thin coating systems in the nanometer range  have been tested.


In the individual cases best TEM detector contrast settings  could be found, as well as optimum fluorescence lines settings  on the EDX to minimize the errors. The TEM measurements, in thickness and composition, were compared to the thin film  EDX software and the µXRF method results to determine their  accuracy.


It turns out that depending on the layer system recalibration  with multilayer standards or at least with elemental standards  is recommended.


It could be shown that with µXRF and thin film EDX a  reliable, rapid and non-destructive layer analysis is possible.


The goal of this work was to establish new alternative  analytical methods for very thin film measurement in package  applications, in terms of high lateral resolution, measurement


capability, accuracy and deviations. The field of interest  contains on the one hand thin layers for refining or doping  metal surfaces, like plating layers, and on the other hand the  control of oxidization of ignoble surfaces.


Two different analytical methods have been established  and compared:


 A new thin film EDX (energy dispersive x-ray micro


analysis) software module for characterization of thin


films. The spectra are taken with a standard EDX detector


attached at a SEM (scanning electron microscopy). The


lateral resolution is therefore in the hundreds of


nanometers, depending on material and electron energy.


 µXRF (micro X-ray fluorescence) with a multilayer


software option and a precisely focused beam spot of 30µm


diameter by a poly-capillary optics. The range of detectable


elements is from Na to U, means that oxides cannot be


detected by µXRF.


The advantage of these two methods compared to conventional  analytical methods like TEM (transmission electron  microscopy) or AES (Auger electron spectroscopy) are the fact  of non-destructiveness, the ease of analysis from layer top and  multiple positions, low analysis time below 60 seconds and  high throughput.


Both systems are installed at Infineon, whereas the thin film  EDX software is a EDX signal processing software with  potential for non-destructive thickness measurement of various  thin layers or layer systems in the range of few to some  hundreds of nanometers. The software allows a variety of  elemental fluorescence lines which have to be selected and  checked for meaningful results. The issue and restrictions are  well described in [1] to [3].


Sample setup


216 cm-1 Cu2O


A careful selection of different test samples was done, covering four fields of relevant layer types in the device  packaging technology. The achieved results should  demonstrate the accuracy of the two methods over a wide  range of materials and thicknesses. Following layer stacks


299 cm-1 (CuO)


were chosen:


1. Copper oxide on copper, for controlling the oxidation


2. Ultra thin aluminium oxide on copper, for controlling


oxidation of ignoble materials


3. Ultra thin leadfree plating, with a silver-gold mix layer on


Points


400


600


1600


palladium, on nickel, on copper leadframe material


K:\FELMI-ZFE\A12270\Cuoxid1_473nm_DS_0D_17.spc


11/10/18


4. Palladium coating on copper wires for advanced copper


K:\FELMI-ZFE\A12270\Cuoxid2_473nm_DS_0D_16.spc


wire bonding


Each sample was prepared carefully in advance for precise  position finding and comparison, by marking the regions of


CuO/Cu2O


interest with micro indentation.


Each reference thickness at the same position was obtained by  TEM analysis at Infineon in Kulim, Malaysia, and the ZFE


0.06


(Center for Electron Microscopy, Graz, Austria), at which  different detector contrasts have been tested.


0.05


0.04


Thin Film Measurement


Methods @ IFX Methods @


Methods


Regensburg


IFX Kulim


Methods @ ZFE Graz


Test Topic


Object


thin film SEM/µXRF FIB TEM FIB TEM/STEM-Raman


0.03


EDX EDX


EDX HAADF


software


or  EELS


0.02


1 Cu oxide oxide type,  done


done done done done


thickness


0.01


2 Al oxide


done


done done


0.00


Cu wire


Figure 1: Overview of samples and analysis combinations


1. Copper oxide on copper


Three different layer thicknesses of copper oxide have been  prepared by annealing copper pads on silicon. The annealing  results in different single layer thickness of the two stable  oxides CuO and Cu2O, lying on each other.


To determine the Cu2O/CuO ratio, Raman spectroscopy was  done at ZFE Graz and peak intensities were calculated, see  figure 2 and 3.


K:\FELMI-ZFE\A12270\Cuoxid3_473nm_DS_0D_18.spc


Seite 1 von 1


Figure 2: highlighted bands of CuO and Cu2O in Raman  spectra


Oxid1


Oxid2


Oxid3


3 ultra thin thickness,


platingconcentrationdone done done


Probe


Figure 3: calculated Raman bands intensity ratio CuO/Cu2O


4 Pd coated thickness


Due to the low ratio of CuO of circa 1/20 and below a  weighted approach in the thin film EDX software was not  necessary. The layer was calculated as pure Cu2O and the  accepted failure is shown to be well within the detected point  to point variation of EDX and TEM.


Unfortunately there was no possibility to visualize the thinnest  copper oxide layer by TEM and EELS (electron energy loss  spectroscopy).


During TEM investigation, it was found out that EFTEM (energy filtered TEM) contrast delivers more reliable thickness  values of copper oxide than the STEM-HAADF (Scanning  TEM high-angle annular dark field) contrast. Figure 4 shows  an example of the EFTEM elemental map of sample “oxid2”.


Figure 4: EFTEM elemental map of copper oxide layer and  integrated intensity profile


The thin film EDX standard less analysis was done at 15kV


Aluminium Oxide Correlation


and the setup of the relevant fluorescence lines has to be


manually optimized by lowering the relative errors of the kfactors. This is realized by ignoring the substrate excitation


fluorescence and only calculating with the oxygen signal. With


this setup an accurate thickness determination with low


variation was possible and could be compared to the TEM  reference values. The densities of the materials were taken


from published bulk densities from relevant tables.


Sharpening Process


The first step of the sharpening method is to convert the  NBED pattern into a Rotation Averaged Spectrum (RAS) using the DiffTools plug-in package in DigitalMicrographTM. The RAS has some similarity to the EELS spectrum, which  inspired us to apply the EELS spectrum sharpening method on  the RAS. The Maximum-Likelihood (ML) deconvolution is an  effective method for EELS spectrum sharpening [3]. The  theory and details of the ML deconvolution were explained  elsewhere in ref [4, 5]. In this work, the ML deconvolution  program was revised to be suitable for RAS sharpening and  was re-programmed in Python. One of the major challenges to  sharpen the RAS is to find a suitable Point-Spread-Function (PSF). In EELS spectrum sharpening, the Zero-Loss-Peak (ZLP) can be extracted from the EELS spectrum as a PSF; however, in RAS, the center spot only forms a half peak in the  RAS (see Fig. 2 (a)). To get a full Center-Spot-Peak (CSP), the half peak was mirror-flipped against the zero location, as  shown in Fig. 2 (b). A Gaussian peak that fits the full CSP was  used as the PSF for the RAS sharpening. In principle, the  Gaussian peak fits other peaks in the RAS and can also be  used as the PSF. Converting the CSP into a full peak also


reduces artifacts during ML deconvolution. Using a Si (011) diffraction pattern as an example, the SADP, NBED and  sharpened NBED RAS are put together for comparison. As we  can see in Fig. 3, after sharpening by the program, all NBED  RAS peaks are sharpened and some peak widths (e.g., the Si


(111) peak) can match the width of SADP peaks. It clearly  shows that this method is effective in sharpening and  improving the precision of the NBED RAS peaks. It should  also be noted that, similar to EELS spectrum sharpening, the  ML deconvolution will induce some artifacts around major  peaks. The sharpened spectrum has to be compared with the  original spectrum to make sure that the peaks are really from  the diffraction spots.


Figure 2: (a) The Rotation Averaged Spectrum of the NBED  pattern in Figure 1 (b). (b) The Center Spot Peak. The blue  curve (right half) is the original half peak, while the red curve (left half) is the mirror curve of the blue one to form a full  peak.


Phase Identification


The first case study demonstrates the capability of this method  to identify the IMC phases in the Al-Cu bonding system. The  IMC phase at the Al side near the Cu wire – Al pad bonding  interface were investigated. The location in the Al-rich IMC


phase on which we performed EDX and NBED analyses for  the case study is shown in Fig. 4. TEM and EDX analysis  showed that the Cu-Al atomic ratio is close to 1:2. However, the Cu:Al=1:2 phase can be the θ-CuAl2 phase (space group: I4/mcm), the CuAl2 phase (F/mmm), or the θ’- CuAl2 phase (I4m 2). A previous study [6] tilted the sample until the IMC phase aligned to certain zone axis and then acquired the diffraction pattern by NBED.


Figure 3: Comparison of Rotation Averaged Spectra (RAS) obtained from SADP and NBD diffraction patterns. The green  curve is the sharpened spectrum of the NBD RAS. Some  artifacts in the green curve have been pointed out.


Figure 4: STEM image at the Cu-Al interface. The location in  the Al-rich IMC phase for the EDX and NBED analyses is  shown by the red dot.


The phase identification relies on comparing the diffraction  pattern to simulated diffraction patterns. Both the sample  tilting for such small-sized phase and computer simulations  are both challenging and time-consuming. However, using the  peak sharpening method demonstrated in this work, the peak  location would be determined more precisely and confidently.


The phase identification can be done by simply measuring the  peak location in a randomly oriented NBED pattern, an  analysis that is much easier and faster to do. The RAS and  sharpened RAS of the NBED pattern in the Al-rich IMC phase  are shown in Fig. 5. The peak sharpening indeed improves the  precision of peak locations (e.g., the (330) and (422) peaks). All peaks agree with the d values of the θ-CuAl2 phase (I4/mcm), as shown in Table 1. The IMC phase can then be  identified as the θ-CuAl2 phase.


Figure 5: The Rotation Averaged Spectrum (RAS) and its  original NBED pattern (inset) in the Al-rich IMC phase. The  peaks that match the d values of the θ-CuAl2 phase are  labelled on the spectrum.


Figure 6. The illustration of the transistor that was used for  the strain analysis. The NBED strain analysis was performed  along the line in the arrow-indicated direction.


Strain analysis


The NBED strain analysis was performed in a PMOS  transistor with an e-SiGe Source / Drain. Only a schematic  illustration of the transistor structure is provided in Fig. 6 due  to confidentiality concerns.


To get an idea of the precision improvement of the NBED  strain analysis, 100-point NBED patterns were collected in the


Si substrate far below the transistors. Those areas are  supposed to be strain-free. Without sharpening the RAS of  NBED patterns, as shown in Fig. 7(a), the standard deviation  of the strain values is about 0.1%. After spectrum sharpening, the standard deviation is reduced to about 0.08%. Therefore, the spectrum sharpening can give a 20% improvement of the  precision.


Table 1: Comparison of the plan distance d values between  the literature data and the measurements from NBED of this  work. The d values obtained experimentally that match the  literature data are highlighted in red italics.


hkl


d (ref. [7]) / Å d (this work) / Å


110


4.287


3.032


002


2.436


211


2.369


2.360


220


2.144


112


2.118


310


1.917


202


1.899


222


1.609


1.618


321


1.590


1.516


312


1.507


330


1.429


1.433


411


1.408


213


1.393


420


1.356


402


1.287


332


1.233


1.218


422


1.185


1.187


431


1.177


114


1.172


The NBED strain analysis was then performed in the PMOS  channel region. The NBED line scan was performed along the  line under the gate as shown in Fig. 6. The NBED patterns  were collected from the channel region all the way down to  the substrate (strain-free) area. The measured strain profile (Fig. 7(b)) clearly shows compressive strain in the channel  induced by the e-SiGe Source / Drain. The measurement using  the sharpened RAS has less data variation and provides a  better representation of the strain profile.


In summary, the method of Maximum-Likelihood  deconvolution used for EELS spectrum sharpening can also be  used for sharpening rotation averaged diffraction pattern  spectra. The location of diffraction spot peaks can be more  precisely determined after peak sharpening. In the first case  study, this method is proved to be able to simplify the NBED  phase identification analysis.


Figure 7. The comparison of NBED strain analysis results  between the no sharpening RAS and sharpened RAS: a) the  strain analysis in the Si substrate far below the transistors; b) the strain variation along the orange line as shown in Figure


The through-put of nano-scale phase identification can be  improved. In the second case study, we have demonstrated  that the precision of the NBED strain analysis can be  improved 20% by applying spectrum sharpening. The two


cases studies support the conclusion that this spectrum  sharpening method is a cost effective way to improve the  precision of NBED analyses.


The authors would like to thank the management of WinTech  Nano-Technology Services Pte Ltd for their support.


[1] A. Armigliato, “Electron Diffraction with Ten Nanometer  Beam Size for Strain Analysis of Nanodevices”, Applied  Physics Letters, Vol. 93 (2008). pp. 161906 - 161906-3.


[2] Mitchell, D.R.G., "DiffTools: Electron Diffraction  Software


Tools


for


DigitalMicrographTM", MICROSCOPY RESEARCH AND TECHNIQUES, Vol. 71 (2008), pp. 588–593


[3] Zhou, YongKai, et al., "EELS Chemical Bond  Characterization of Process Induced Damages in Low-k  Dielectric Films", IPFA2012 Proceedings, Session 08.01 (2012).


[4] R.F. Egerton, Electron Energy-Loss Spectroscopy in the  Electron Microscope, 3rd ed., Springer, (New York, 2011), Appendix B.6.


[5] R.F. Egerton, et al., “Fourier-Ratio Deconvolution and its  Bayesian Equivalent,” Micron, Vol. 39 (2008), pp. 642-647.


[6] Bae, In-Tae, et al., Intermetallic Compound Formation at  Cu-Al Wire Bond Interfaces, Journal of Applied Physics, Vol. 112 (2012), pp. 123501-8.


[7] Havinga, E.E., et al., Less-Common Met., Vol. 27 (1972)  p. 169


Automated Defect Analysis in Solar Cells Using EBIC


Dr. Grigore Moldovan


Oxford Instruments NanoAnalysis, High Wycombe, United Kingdom   grigore.moldovan@oxinst.com


Shark Lotharukpong and Prof. Peter Wilshaw


Department of Materials, University of Oxford, Oxford, United Kingdom


Electron Beam Induced Current (EBIC) characterization is  unique in its ability to provide quantitative high-resolution  imaging of electrical defects in solar cells. In particular, EBIC  makes it possible to image electrical activity of single  dislocations in a Dual-Beam Focused Ion Beam (FIB) Scanning Electron Microscope (SEM), to cut and lift out a  micro-specimen containing a particular dislocation, and then  transfer it for further structural or chemical analysis. As typical  solar cell material presents a complex array of defects, it is  important to observe statistical variations within a sample and  select key sites for analysis.


This paper describes a method for automated defect  identification and characterization, and shows an application to  multi-crystalline silicon (mc-Si) solar cell wafers selected from  different heights along the manufactured ingot. Information  presented here includes the experimental setup for data  acquisition, as well as the basic algorithms used for  identification and extraction of dislocation contrast.


Electron Beam Induced Current (EBIC) is a well-established  method for characterization of electrical defects in  semiconductor materials in electron microscopy, in particular  for characterization of dislocations and grain boundaries [1-2]. It has been applied extensively to Si materials, as well as many  compound semiconductors, such as GaAs or GaN [3-4]. As  EBIC provides the key ability to observe electrical activity  with high spatial resolution, an array of methods has been  developed for particular characterization needs, of which the  most popular are measurement of recombination strength and  quantification of diffusion length of minority carriers [5-6].


Increasingly, EBIC is providing the unique ability to identify  and measure recombination activity of single dislocations in  preparation for more advanced characterization, such as Atom  Probe or Transmission Electron Microscopy. For example, use  of EBIC on Dual-Beam Focused Ion Beam – Scanning  Electron Microscopes (FIB-SEM) allows for identification and  preparation of relevant sites for lift-out.


Solar cells, in particular, display a complex array of defects, including single dislocations, grain boundaries and inclusions, and therefore assistance is required to guide preparation of  valuable micro-specimens and to provide direct correlation of  composition and structure with electrical activity. This  complex array of defects generates the need for automated  identification and analysis, as described below.


Method


To provide raw data for testing, mc-Si solar cell wafers were  selected from the bottom, middle and top of an ingot. Bottom  and top wafers were selected from parts of the ingot that are  not generally used for manufacture of solar cells, as they  exhibit short minority carrier lifetimes. However, the  distribution of defects along the height of the ingot provides an  essential insight into the formation of the solar cell material, and constitutes a good test for automated analysis methods.


For electron microscopy, smaller 1cm2 samples were cut and  cleaned from these wafers, then a 3mm diameter, ~20nm thick  Al round pad was deposited by e-beam evaporation to form a  top contact, and the resultant device was attached to a standard  SEM stub using conductive Ag-loaded epoxy to form a bottom  contact. The top Schottky contact provides the electrical field  required for EBIC characterization, and the bottom ohmic  contact gives the second terminal of the device.


Experimental Set-Up


Solar cell devices mounted on SEM stubs were loaded on the  stage of a Tescan Mira SEM, which provided electrical  connection to the bottom terminals. Devices were probed in  turn with an OmniProbe OP100.7 nanomanipulator equipped  with a coaxial shaft, which provided electrical connection to  the top of each device (see Fig. 1).


For initial work, the probed solar cell devices were connected  to a Keithley 428 current amplifier, and the output signal was  captured by the scanning system in sync with the beam  scanning control. Finally, for quantitative acquisition and  current-voltage (I-V) characterization, the probed solar cell


devices were connected to an Oxford Instruments e-amp using  E3 acquisition software.


A number of solar cell devices were loaded into the SEM at  the same time, and mounted on an electrically-connected stage.


Each device was connected in-situ, in turn, by means of the  electrical probe, and I-V characteristics were recorded to  confirm successful electrical probing and the diode behavior of  the solar cell device (see Fig. 2).


Figure 1:  Experimental setup, showing electrical probing of  solar cell devices in SEM for EBIC.


-1 0 1 2 3 4 5


-1,000


VOLTAGE (mV)  Figure 2:  Typical current voltage (I-V) characterization of  solar cell, showing good contacts and diode behavior.


Figure 3: Typical 2,048 x 2,048 EBIC image of a 3mm circular Al pad on mc-Si; wafer from top of the ingot.


AMPLIFIER


SCANNING SYSTEM


TO SCAN


CONTROL


MANIPULATOR


DEVICES


TOP


TERMINAL


STAGE  ELECTRON


MICROSCOPE


BOTTOM


FEEDTHROUGH


Live EBIC imaging was used to monitor probe touchdown, as  the immediate appearance of the EBIC signal proved more  sensitive than conventional probe shadow or deflection-based  methods. Typical EBIC images recorded at 20kV acceleration  voltage (see Fig. 3) show single dislocations and grain  boundaries in the mc-Si wafers as dark features, as well as the  tip of the nanomanipulator and contamination particles on the  surface of the device.


A higher magnification image (see Fig. 4) provides an  improved view of the dislocations, but also highlights  impurities on the surface of the device. Since the electron  beam is absorbed in the W tip, no current is induced into the  device underneath it and therefore this area has been used to  establish the dark (0 A) level for each image analyzed.


Analysis Method


A new image analysis method was designed to automatically  identify dislocations, in particular for images captured at about  1,000x magnification. Identification may be used under a very  wide range of magnifications; however, a lower magnification  allows for analysis of many more dislocations in the larger  field of view, and thus provides improved statistics. A limit at  very low magnifications is imposed by the sampling required  to image single dislocations; a limit at very high  magnifications is given by the need to record signal away from  the dislocation capture radius.


Criteria for automated identification of single dislocations  include


• an intensity in the middle of the dislocation core area  that is smaller than the average background area  intensity by significantly more than the background


standard deviation,


• a minimum circularity parameter when segmented by  intensity, and


• no significant annular variation in intensity of the  background area.


This approach (illustrated in Fig. 4) is designed to provide a  natural feature segmentation for typical EBIC images, and thus  to distinguish between single dislocations, grain boundaries  and shadow of the tip. Further, the algorithm will reject from  analysis dislocations partially obscured by the tip, or too close  together.


Once dislocations have been identified, dislocation contrast C  was calculated using the standard formula


C = (Ibackground – Icore) / Ibackground (1)


where Icore is minimum signal at the dislocation core and  Ibackground is the mean background signal; both of which are  corrected for the true zero in current in the absence of electron  beam illumination. Note that the calculated dislocation  contrast is independent of the SEM contrast and brightness  settings.


The criteria described above have shown excellent  discrimination of image features arising from recombination at  dislocation sites and other contrast mechanisms, including  grain boundaries, surface contamination and tip shadowing. Significant changes in background intensity have been  observed between grains, and use of local background  intensity has been found to be essential.


It has been found that a minority of dislocation sites are  excluded from analysis, depending on the particular search  values used in the automated algorithm. In particular, dislocations that are in close proximity to each other do not  allow for adequate reading of the background intensity, and  were excluded from the final analysis. However, the algorithm  allows for identification of the large majority of dislocations.


Figure 4: Typical 1kX magnification EBIC, showing  dislocations and variation in background intensity across the  device.


Figure 5:  Schematic diagram of areas used for automated  identification and analysis of dislocations.


BACKGROUND AREA


DISLOCATION


CORE AREA


RADIAL DIRECTION


ANNULAR DIRECTION


The smallest measureable contrast value for this experiment  was 0.01, which may be improved with longer acquisition  times or reduced acceleration voltage. This level of contrast  provides excellent discrimination for the purpose of this study.  The distribution of dislocation contrast has been measured for  wafers from the bottom, middle and top of the ingot, respectively, and show a clear gradual shift in activity at  dislocation sites as the ingot is solidified (see Fig. 7). Dislocation contrast average value is decreasing from 0.12 for  the bottom wafer, to 0.10 for the middle wafer and finally to


0.08 for the top wafer. Overlapping distributions highlight here


the importance of statistical analysis.


Discussion and Conclusions


Automated analysis of dislocation contrast on solar cell wafers  revealed that the EBIC contrast of dislocations is shifting from


0.12 at the bottom of the ingot to 0.08 at the top of the ingot. This shift in dislocation contrast may be assigned to the  different total times available for dislocations to collect  impurities, where dislocations at the bottom of the ingot have  more time compared with those at the top.


However, this may also be attributed to the different densities  of dislocations along the height of the ingot, where impurities  at the bottom of the ingot are spread between a reduced  number of dislocations, as compared with those at the top.


As highlighted by the overlapping distributions, such analysis  and observation can only be provided by statistical analysis of  dislocations, where automated identification is key. This study  has proposed and demonstrated one such algorithm for  automated defect identification.


[1] Orton J.W. and Blood P., The Electrical Characterization  of Semiconductors: Measurement of Minority Carrier  Properties, Academic Press (London, 1990).


[2] Donolato C., Optik, Vol. 52, No. 19 (1978).


[3] Yakimov E.B., Journal of Physics: Condensed Matter  Vol. 14 (2002), pp. 13069-13077


[4] Moldovan G. et al., Ultramicroscopy Vol. 107 (2007), pp. 382-389


[5] Fell T.S. and Wilshaw P.R., Journal of Physics IV  France, Vol. 01 (1991), pp. C6-211-C6-216


[6] Ong V.K.S et al., Journal of Applied Physics, Vol. 100 (2005), pp. 114501


Figure 6: Typical segmented image during analysis (area is  also shown in Fig. 4), showing identified dislocations and  discrimination from tip shadow and grain boundaries.


0.10


0.20


0.30


0.40


0.14


0.18


0.22


DISLOCATION  CONTRAST


MIDDLE BOTTOM


Figure 7:  Distributions of dislocation contrast for wafers from the top, middle and bottom of the ingot.


Reballing/Rebumping Ultra Fine Pitch Packages Less Than 0.5mm pitch for FA


Bob Wettermann


BEST Inc, Rolling Meadows, IL USA   bwet@solder.net


As the pitch and package sizes of semiconductor devices have  shrunk and their complexity has increased, the manual  methods by which the packages can be re-bumped or reballed  for failure analysis have not kept up with this miniaturization.  There are some changes in the types of reballing preforms  used in these manual methods along with solder excavation  techniques required for packages with pitches as fine as


0.3mm. This paper will describe the shortcomings of the  previous methods, explain the newer methods and materials  and demonstrate their robustness through yield, mechanical  solder joint strength and x-ray analysis.


Figure 1 Shows a Non-Contact Solder Excavation Example


There are several methods which will be discussed both for  deballing, subsequent site excavation and reballing. This paper  will review the deballing methods used most commonly  including non-contact solder excavation (Figure 1) solder  wicking and solder fountains. Machine-based reballing  methods including solder “jetting” (Figure 2) are not included  in the scope of this work as does not fall under the manual  methods category. Mechanical fixturing and solder preform  reballing techniques will be compared and methods discussed.  The repeatability, speed and yields for ultra fine pitch devices  using these different manual methods along with their  processing conditions and process photos will be presented.


Figure 2 Depicts a Reballing using “jetting” technique


The focus of this paper is several fold. The first issue  investigated was insuring that a practical and cost effective  process of reballing can be carried out on small, ultra fine  pitch uBGAs, WLPs and MEMs.  This work analyzed the  mechanical strength of the solder joint, pre- versus postreballing and final ball diameters and voids of the reballed  BGAs in order to analyze the factors which may impact the  reliability of a reballed device.


Reballing of BGAs, CSPs, MEMs and WLPs has been taking  place in order to allow semiconductor device vendors to  perform failure analysis after devices have been returned from  the field, from the packaging house or from other sources. With ever decreasing package sizes and complexity and the  associated smaller ball diameters and pitches, the same  methods which have heretofore been used for reballing larger  packages have been become increasingly challenging to use. These smaller package sizes have made it difficult to create  tools for the solder fountain or miniature wave deballing  machines as the packages get more difficult to fixture. In  addition, the solder balls are hard to pour in to metal reballing  fixtures as the various forces acting on the balls-relative to  their weight become significant. Older paper reballing  preforms, since they rely on mechanical punches to “hole out” the apertures to hold the solder spheres, cannot be fabricated at  these ultra fine pitch sizes.


Figure 3- Device with integral passives and solder spheres


For this experiment ultra fine pitch BGA “dummy parts” were  used. The pattern used is seen in Figure 4, below, and it  consists of a 0.3mm pitch BGA, 8 mil solder balls in a 4.2 x


4.2mm package. SAC305 solder balls were used during these  trials.


Figure 4- Outline dimensions of test vehicle


The total number of devices used in this experiment were (29) in number. Each of them was laser scribed (Figure 5) with a  designator in order to keep track of the different parts for this  experiment.


There were 3 deballing methods compared namely the solder  fountain, the solder wick and the non-contact solder  excavation methods. A 5 mil (0.005 inch, 0.127mm) balled  thermocouple was embedded in to 3 parts for each of the 3  methods in order to determine the temperature profile at the  die using each of the various deballing methods.


Figure 5- Laser inscribed parts for tracking


The first of these methods was the use of a soldering iron, flux  and desoldering braid. In this method the part was fixtured (Figure 6) and held in place as the size and mass of the part is  such that it tends to move around without this fixturing. The  parts were placed in to a laser inscribed stainless steel fixture  to hold the parts. Other areas of the fixture were prevented  from having the flux and flux residue contaminate each of the  pockets by taping them off with Kapton™ tape.  After  application of paste flux, a very small blade tip was used along  with 0.1mm wide solder wick to move vertically “up and  down” onto the pads. Movement along the surface of the part  is not recommended as it can scratch or damage the mask or  lift pads. The second method shown in (Figure 8) is the solder


fountain technique. Alternatively the part can move on either a  conveyorized or mechanical motion system on order to bring  the part in to the miniaturized wave solder system for a similar  effect.


Figures 7 and 9 are the respective deballing method reflow  profiles (MegaMole 20) using a soldering iron/wick and a  solder fountain.


A third common deballing method relies on the non-contact  solder excavation (Figure 1) of the solder balls from the  package.


Figure 6- uBGA were fixtured and held in place during deballing


Figure 7- Deballing profile time (s) vs temp (°C) using solder  iron/wick method


Figure 8- Deballing profile using solder iron/wick method


Figure 9- Deballing profile time(s) vs temp (°C) using solder fountain  method


A third thermocouple was used to develop the semi-automated  reballing profile (Figure 10). In this case a 5 mil tape  thermocouple was attached to the BGA body (post solder  removal) prior to placement of the solder ball preform.  The  reflow cycle was developed to achieve a peak temperature of  240°C at the solder joint, while minimizing the package and  die temperature (Figure 8).


Figure 10- Semi-automated preform placement method


Figure 11- Reballing preform for micro packages


In terms of the reattachment of solder balls there are numerous  methods. Some of the more common methods include the use  of solder preforms (Figure 11) and the use of various  mechanical fixturing techniques for selective replacement of  the solder balls. In the case of the preforms, a preloaded


plastic substrate with adhesive backing has the matching array  of replacement balls corresponding to the package ball pattern. The deballed and site dressed package is placed on to the  preform, the assembly sent through the reflow process, and the  preform pulled off leaving the solder balls attached to the  bottom of the package. In the fixturing approach the package is  held in a fixture, and through the use of a variety of stencils, solder balls are placed onto selective pad locations. Once the  balls are on the pads, the device is reflowed, cleaned and  inspected prior to use.


The many benefits of the reballing process lead to many  concerns in the reliability of the reworked components. These  concerns include the formation of a thicker intermetallic, anomalies and defects developed as a result of the reballing  process. The most common concerns of a reballed device is  the mechanical strength of the newly formed solder joint.  Shear testing of the solder joint allows for the mechanical  strength of the newly formed solder joints to be investigated.


The focus of this paper is several fold. The first issue  investigated was insuring that a practical and cost effective  process of reballing can be carried out on small, ultra fine  pitch uBGAs.  Finally, this work analyzed the mechanical  strength of the solder joint, pre- versus post-reballing and final  ball diameters of the reballed BGAs in order to analyze the  factors which may affect the reliability or placement of a  reballed uBGAs.


Each of the parts was inspected both before and after the  deballing and site preparation with anomalies noted and  visually recorded. A combination of deballing and ball reattachment techniques was investigated.


In the first trial, the parts were deballed using the manual wick  and soldering iron deballing method. A single operator applied  paste flux, applied a soldering iron and solder braid to deball  and site prep the uBGA packages. A water soluble Alpha WS809 tacky flux was used during the reballing process.  The  plastic preforms with an adhesive backing were placed, preform side down with the component placed manually on to  the preform. After alignment, the parts were reflowed and the  preform removed. Finally the BGA was cleaned and inspected.  In terms of the cycle time for deballing these small packages, the solder fountain technique was 2-3 seconds in length, the  manual solder wick method 15 seconds and solder excavation  process 25 seconds respectively.


In the second trail grouping, parts were also deballed using a  soldering iron and solder wick.  In this case the BGAs were  reballed using a semi automated reballing preform placement  technique with the VJ Electronix Micra rework system  performing this function. In this technique the parts are held in  a machine fixture as a semi-automated rework station picks the  preform from a pocket, dips the solder balls into flux, and  places it onto the pads of the BGA.


Methods @ IFX Regensburg


ID Topic Object Elements TEM meanTEM Thin film Thin film µXRF µXRF  std.dev.


EDX


EDX meanstd.dev.


[all in nm]


meanstd.dev.


TEM 3kV 5kV 10kV 15kV 20kV


oxid1 Cu oxide type,  Cu2O


not detectable


16.8


2.8


oxid3


Cu2O


48.4


5.2


76.8


4.3


Figure 5: Overview of copper oxide samples and thickness  results


Figure 6: Correlation of thin film EDX and TEM thickness


Figure 5 and 6 show each sample result and the correlation  plot. The correlation shows a high stability index, but quite  high deviation of the thin film EDX values. This is expected  because of the light oxygen element, with atomic number Z =


8, which could lead to failures if lying on a heavier matrix like  Cu and quantified standard less. For such cases the software  allows standardization by intensity correction, which is  recommended to implement.


2. Ultra thin aluminium oxide on copper


An atomic layer deposition was performed to deposit the ultra  thin aluminium oxide on copper. The composition was initially  Al2O3 and the thickness determination was done by TEM at  Infineon Kulim to 3.95±0.35nm.


The thin film EDX standard less analysis was done over a  range of energy from 3 to 20kV, see figure 7.


oxid2 oxidethicknessCu2O


24.5


6.5


33.1


3.4


EDX energy


Figure 7: Correlation of TEM and thin film EDX thickness  over EDX energy


The setup of the relevant fluorescence lines has to be manually


Copper Oxide Correlation


optimized to decrease the relative errors of the k-factors. This  is again realized by ignoring the substrate excitation


fluorescence and only calculating with the oxygen signal.


R² = 0.9727


80


It is obvious that higher EDX energy increases the error in the


standard less quantification case. This is again due to the


matrix effect of light oxygen on heavier aluminium.


With this setup an accurate standard less thickness


determination with relative low variation was possible to up to  10kV. If higher excitation energies get necessary, e.g. due to


30


layer thickness, a standardization by intensity correction in the


software is recommended.


Thin film EDX mean


Linear (Thin film EDX mean)


3. Ultra thin leadfree plating


Three layer stacks have been chosen with different thicknesses


and Ag-Au concentration over a wide range.


Copper oxide, TEM thickness [nm]


During TEM investigation, it was found out that STEMHAADF contrast delivers more reliable thickness values of the  layers than the TEM-BF (TEM bright field) contrast. Figures 8  and 9 show an example of the layer stack on the copper  leadframe of sample “µPPF1”


Correlation: AgAu thickness


120


R² = 0.9984


R² = 0.9772


R² = 0.9889


Figure 8: schematic overview of layer stack


60 40


Correlation: Au concentration


Figure 9 left: TEM image of Ni, right: zoomed into AgAu/Pd


65


layer top


R² = 0.9835


µXRF mean


µXRF mean, with recalibration


R² = 0.846


The ThinFilm EDX standard less analysis was done at 7, 20


55


and 25kV to investigate the capability over a wide range. Eight  different software setups in energy and relevant fluorescence


lines were compared in terms of lowest relative errors of the k45


factors, as recommended, low deviation to TEM results and


R² = 0.9399


ability to measure a nickel thickness above 1000nm. These


requirements could be best fulfilled by using 25kV, Au_M,


35


Ag_L, Pd_L, Ni_K and Cu_K fluorescence lines for the  analysis. The densities of the materials were taken from


45


published bulk densities from relevant tables and a mean  density of 13.6g/cm³ was taken for the Ag-Au mix layer on  top.


The µXRF measurements are carried out with 30µm spot size  and are referred to bulk elemental standards by intensity


Correlation: Pd thickness


correction at first. After seeing significant errors of the µXRF  results, a recalibration with the multilayer stacks was applied,


to consider matrix and self absorption effects. Thus the error


R² = 0.9995


could be reduced significantly, see figure 10. Three single


R² = 0.9782


measures per sample have been done in all cases.


Sample Topic Object Elements TEM meanTEM Thin film Thin film µXRF µXRF µXRF mean, µXRF


R² = 0.9726


ID


std.dev.


with


recalibration


µPPF1 ultra thickness,AgAu


14.3


13.1


12.6


15


thin Au conc.


Pd


7.1


5.6


4.9


6.9


platingin AgAu


Ni


136.0


11.4


140.0


263.8


149.3


Au wt.%


52.8


2.9


43.4


2.4


40.0


53.2


1.3


µPPF2


AgAu


17.0


3.2


1.1


19.7


18.9


12.0


0.0


13.4


12.5


12.4


1166.7


56.7


1378.9


7.8


968.5


1179.5


1.7


57.9


4.0


55.0


47.4


56.9


µPPF3


93.2


12.2


87.6


78.3


92.5


30.5


2.6


28.1


25.8


30.8


10 15 20 25 30 35


305.0


19.4


308.6


402.2


278.8


42.5


37.1


32.7


43.3


Figure 10: Overview of samples and results


AgAu, TEM thickness [nm]


Figure 11: individual thickness results of Ag-Au mix layer


Au, TEM concentration [wt.%]


Figure 12: individual Au concentration results of Ag-Au mix  layer


Pd, TEM thickness [nm]


Figure 13: individual Pd thickness results


600 400 200


0 200 400 600 800 1000 1200 1400


Ni, TEM thickness [nm]


R² = 0.9968


Correlation: Ni thickness


1400 1200


R² = 0.9985


1000 800


R² = 0.8493


Figure 14: individual Ni thickness results


Figures 11 to 14 show the individual sample and layer results  and the correlation plots. The correlations show mostly a high  stability index, but some errors of the thin film EDX software  and µXRF values.


All standard less EDX results are within 20% error except one  outlier value, which demonstrates the excellent capability of  the software. The EDX accuracy can even be improved by  applying an intensity correction with the standardization  routine.


The µXRF nickel results a depth dependent deviation which  indicates a necessary recalibration with the available foil  standards.


The µXRF shows unexpected high deviations despite  elemental bulk calibration. However this can be brought below  10% for all measured values by a recalibration with the  multilayer standards.


4. Palladium coating on copper wires


A palladium coated copper wire with 20µm diameter for  highly integrated wire bonding pads was chosen. The Pd  coating thickness is normally below 100nm and applied to  improve material properties and oxidation behaviour of the  wire.


Best TEM contrast of the Pd layer was obtained in STEMHAADF mode.


The thin film EDX standard less analysis was done at 10 and


Topic Object Elements TEM meanTEM Thin film Thin film µXRF µXRF


17kV to investigate the capability over this energy range.


std.dev.EDX


The µXRF analysis is not possible due to the limited spot size


Pd thicknessPd (10kV)


68.3


32.3


64.5


11.2


minimum of 30µm.


Figure 15 and 16 illustrate the bond wire surface and the crosssection through the Pd coating layer


Figure 15: SEM image on wire top


Figure 16: TEM cross-section image


The EDX energy shows no significant influence and the error  of measured standard less thickness is within 6 percent, which  is again an excellent result for standard less analysis, see figure


17.


coating


Pd (17kV)


67.0


Figure 17: Overview of sample and thickness results


The used fluorescence lines were once more manually reduced  to only Pd_L, without substrate information, to minimize the  relative errors of the k-factors.


In this work non-destructive thin film EDX software and µXRF were established and compared and calibrated with  TEM analysis results.


As an example four different, for the semiconductor industry  interesting, very thin coating systems in the nanometer range  have been tested.


In the individual cases best TEM detector contrast settings  could be found.


The EDX software required manual fluorescence lines settings  to minimize the systematic errors and to reduce point to point  variation.


The EDX software is able to get excellent standard less results  on ultra thin metal layers with errors lower than 20%. On  metal oxides the deviation is quite higher, most probably due  to matrix effects. But accuracy can be improved with  standardization, done by intensity correction. Errors below  10% are reproducible possible, from experience.


The µXRF needs calibration with elemental bulk standards  from beginning on, to reach errors below 35% on metal layers. For further improvement to errors lower 10% recalibration  with multilayer foil standards is necessary to include matrix  effects.


It turns out that thin film EDX is able to measure accurate over  a wide range of layers in “plug and play” mode, but restricted  in maximum layer thickness.


Whereas the µXRF is limited on heavier elements and needs  more intensive recalibration effort, but with the ability to a  larger thickness range.


A part of this work has been performed in the project ESiP, in  which the partners are funded by the German BMBF and the  ENIAC Joint Undertaking.


[1] Sempf K., Herrmann M., Bauer F., “First results in thin  film analysis based on a new EDS software to determine  composition and/or thickness of thin layers on substrates”, EMC 2008 14th European Microscopy Congress, Aachen, Germany, September 2008, pp. 751-752


[2] Eggert F., "Principles and problems of quantitative  analysis by EDX“, Deutsche Gesellschaft Kristallografie /AG Elektronenmikroskopie, Kiel, Germany, March 2002, www.mikroanalytik.de


[3] Haschke M., Eggert F.; „Standard less quantification for µXRF spectroscopy“, Colloqium of BAM at Berlin, Germany, March 2004, www.mikroanalytik.de


Case Studies on Application of 3D Real Time X-ray                              for Flip Chip C4 Package


Lihong Cao, Wallace Donna, Loc Tran and Lynda Tuttle


Advanced Micro Devices, InC  Austin, Texas, USA


This article describes how 3D Real Time X-Ray (RTX) technique enhances the capability of packagelevel failure analysis of a flip-chip package. 3D RTX  was successful in detecting different failure  signatures. This paper outlines detailed applications  of 3D RTX with case studies.


1. Introduction:


IC packages are becoming increasingly complex due  to the growing size, I/O numbers and application of  integrated packages such as MCM (multi-chip  modules), POP (package on package) and 3D stacked


die package. Package level failure analysis has  become very challenging.  Efficiently detecting  failure signatures and finding the root cause has  become very critical. Conventional 2D RTX  techniques are the most common methodology for


package level failure analysis. However, the typical  problem of 2D RTX is the limitation of vertical Z  determination of the defects. Thus, it is difficult to  effectively determine the failure signatures.


3D RTX technique has dramatically increased the  application in the semiconductor industry. Nanofocus  and microfocus 3D RTX have been successfully  applied to copper bond wires, microvias, flip chip  interconnections,  copper filled through silicon vias


(TSV), as well as for 50-60μm microvias of an  embedded chip package [1] [2] [3].


In this paper, case studies by using 3D RTX  techniques are discussed and followed by studies of  the impact of key parameters of 3D RTX on the


image resolution for flip chip package.


2. Working Principle of 3D RTX


Compared to the conventional 2D RTX, there are  three steps to acquire the 3D image, which are image  acquisition, reconstruction and visualization. The  computerized tomography (CT) scans were carried


out with superior and sub-micron feature recognition  2D X-ray images, to produce the best CT models for  3D sample analysis, virtual micro-sectioning and  internal dimensional measurements. The system  acquires a series of two dimensional X-ray images


while progressively rotating the sample step by step  through a full 360° rotation at a certain increments. More steps and images will provide a better CT  model, but more time will be consumed. Very intense  mathematical geometric processing is used to


generate a 3D virtual model of the object using this  series of individual 2-D x-ray images. The resolution  of the reconstructed 3D matrix is defined in terms of  volume pixels or voxels. CT models typically have  256 x 256 x 256 voxels, 512 x 512 x 512 voxels and


1024 x 1024 x 1024 voxels. Modern CT system uses  dedicated hardware (high processing power) for the  number crunching and a high quality CT model is  ready minutes after the acquisition. Reconstruction  can be carried out in parallel with the acquisition.


The geometric magnification M of the image is the  ratio of focus-detector distance (FDD) and focusobject distance (FOD), where M is equal to  FDD/FOD.  Therefore, the smaller the focal spot, the  greater the resolution.  In our studies, the resolution


of the 3D system used is approximately 0.25um. Fig.1 and Fig.2 show the schematic working principle  for 2D RTX and 3D RTX, respectively.


Fig. 1 Schematic for 2D RTX


Fig. 2 Schematic for 3D RTX


3. Case study on resistive open


A DUT (device under test) sample with resistive  open failure was analyzed. Curve trace on the failing  pin confirmed a resistive I-V curve. Comparative  Time Domain Reflectometry (TDR) was performed  on the failing unit to determine at what point the


impedance profile of the failing unit differed from the  known good unit. Fig.3 showed TDR waveform by  comparing a good unit, bare substrate and DUT. It  showed a slight difference in the impedance profile  of the good device.


2D RTX was performed on DUT and the result was  shown in Fig.4.  From the 2D RTX result, an  abnormality on the failing C4 bump was observed. However, it could not determine the failure clearly.


Therefore, 3D RTX was further performed on the  same failed C4 bump by progressively rotating the  sample step by step through a full 360° rotation at  increments of less than 1° per step under 110KV. The  result was shown in Fig.5 after 15 minutes fast scan.


It clearly showed that the C4 bump was not fully  connected and thus caused the resist open. Physical  deprocess analysis was further performed on the  defective C4 bump and the result was shown in Fig.6. The root cause was due to the C4 bump not wetting


during the assembly process (CNW).


Fig.3 TDR showing resistive open near C4 bump.               Fig.4 2D RTX image showing protrusion of C4 bump


Fig. 5 3D RTX images on the defective C4 bump (Connect Non-Wetting)


Fig.6 Non-contact bump seen in mechanical cross-section


4. Case study on resistive short


A Sample was reported as a short failure from  automated test results. 2D RTX was performed and  Fig.7 showed the 2D RTX results. It showed the C4


bumps deformed and reflowed.


In order to find out whether the failure mechanism  was at the Si die side or at the substrate side, the  defect in z direction needed to be further investigated.


3D RTX was applied on the DUT. As the defective  AOI (area of interest) is quite large, the sample with  40mm X 40mm dimension was put into the 3D RTX  chamber. The resolution of 3D RTX is significantly  affected by the geometric magnification, power,


detector configuration, focal spot size and sample


size. Under the selected operation parameters such as  voltage/power and focal spot size, the sample size is  very critical in order to achieve a high resolution. A  small sample size enables sample to be closer to the  X-ray source and get a high magnification, thus to


achieve a high resolution. Compared to previous case  study on one C4 bump, the sample for this case study  is much larger. Therefore, a high power 140Kv and  long acquisition time with 45 minutes were applied  for 3D imaging. The result was shown in Fig.8. It


clearly showed that the solder reflow occurred at the  substrate interface. The root cause was further  identified due to the underfill to solder mask interface  delamination.


Defective C4


Fig.7 2D RTX showing C4 bump reflowed


Fig. 8 3D RTX showing the C4 reflowed at substrate side.


5. Case study on non-destructive


analysis in organic substrate


3D RTX can also be used for non-destructive


inspection in the substrate for both 2D package and  3D packages. It is an especially effective tool to  inspect 3D packages. An example is given here for  one of the non-destructive applications of 3D RTX. A  POP (package on package) sample was requested for


inspection of BGA solder balls and PTH (Pin  Through Holes).  3D RTX was performed under  140Kv with 30 minutes acquisition. Fig.9 showed the  3D RTX imaging after volumetric reconstruction.  In  Figure 9(A), the top view only showed voids in BGA


solder joints. However, it was unable to distinguish


the solder voids either from the top BGA balls or  bottom BGA balls in a POP package. In Figure 9(B), the slice X-section 3D RTX view clearly showed two  layers of BGA balls and the solder voids inside two  layers of BGA balls. Fig. 10 showed the overview of


3D volumetric image of PTH inside the POP sample.  In Fig.10 (A), the top view showed an abnormality in  one of the PTHs. Further slice X-section view was  shown in Fig.10 (B) and (C). It clearly showed the  defect embedded inside the PTH between the two


BGA layers. The defect was suggested to be a high  atomic number material with high absorption of Xray. The feedback was given to the customer and  further investigation will be conducted by the  customer.


Reflowed  C4  bump


Reflowed  C4 bump


Fig. 9 (A) 3D RTX top view image                                    Fig.9 (B) 3D slice X-section view image


Fig. 10 (A) 3D RTX top view image


Fig. 10 (B) 3D RTX slice X-direction view                 Fig. 10 (C) 3D RTX slice Y-direction view


1 2 3  void


s


1  2  3


void s


defect


direction


PTH defect


X direction


PTH defect  Y direction


6. Conclusions


3D RTX has successfully demonstrated its  implementation with high resolution in package level  analyses. It improves the limitation of vertical Z for  2D RTX technique to help to determine the root  cause of the failing mechanism.


7. References


[1] T. Braun, K.-F. Becker, S. Voges, T. Thomas, R. Kahle, V. Bader J. Bauer,K. Piefke, R. Krüger, R. Aschenbrenner and K.-D. Lang, “Through Mold Vias  for Stacking of Mold Embedded Packages”, ECTC  2011, Lake Buena Vista


[2] H. Roth, Z. He and T.Paul, “Inspection of  Miniaturised Interconnections in IC Packages with  Nanofocus X-Ray Tubes and NanoCT”, 10th  Electronics  Packaging Technology Conference, Singapore 2008


[3] K.-J. Wolter, Martin Oppermann and Thomas  Zerna “Nano Packaging – A Challenge for Nondestructive Testing”, 10th Electronics Packaging


Technology Conference, Singapore 2008


Analysis of Two Electrical Failures Caused by Die Attach of Exposed Pad  Package


Jinglong Li; Motohiko Masuda; Yi Che; Miao Wu


Product analysis Laboratory, Freescale Semiconductor (China) limited, Tianjin, China


Die attach is well known in die bonding process. Its electrical  character is simple. But some failures caused by die attach are  not so simple. And it is not proper to analyze by a generic  analysis flow. The analysis of two failures caused by die attach  are presented in this paper.


Die bonding is a mature process.  Die attach is well known in  die bonding process.  It could experience various physical  defects such as void, delamination, lead contamination, bridge  and so on [1-2]. These defects induce electrical failures such  as open, short or leakage. Most of these defects and failures  are able to be analyzed effectively and successfully by  traditional package FA techniques with a generic analysis flow


[3].


Exposed Pad (EP) is appeared in Quad Flat No-Lead (QFN) package as heat spreader.  And EP is also possibly connected  to the outer circuit (for example, as power supply pin).  So the  electrical quality of the die attach become important.  However  the electrical failure analysis is not so simple to localize the  defect in the broad die attach area in some cases.


In this paper, two failure cases caused by die attach are  discussed. The electrical failure isolation approaches are also  demonstrated.


Case 1 study


Device information and failure description


It was a Customer Quality Incident (CQI). The CQI unit is in  QFN48 package. As shown in Fig.1a, there are a couple of  VDD and VSS pins.   The center is an EP for heat spreader.  Although the die is placed on the EP with electrically  conductive die attach, this EP does not short to VDD or to  VSS.


Several CQI units were VDD and VSS short on customer’s  application boards.  However the returned CQI units were  passed final test and no short was found between any VDD  pins and VSS pins. Considering that EP was tied to VDD


plane on customer’s circuit board, then it was found that EP (but not VDD pin) was resistive short to VSS pin (I-V  character shown in Fig.1b).


Figure 1: (a) Backside view of the QFN48 package with VDD  and VSS pins assignment; (b) EP-VSS I-V curves of a  reference and the CQI unit.


Failure isolation


No defect or damage was observed by package level  inspection (optical microscope, C-SAM and X-ray). A little  difference was noticed on the dark area (marked by arrows) of  each die side by X-ray photo (Fig.2).  The area was wider and  darker in CQI unit than that of reference unit.   It means more  excess die attach in CQI unit.


Figure 2:  X-ray photos. (a) CQI unit; (b) Reference unit.  The  dark areas of each die side means excess die attach of CQI  unit.


The next step was to isolate the defect point. First, EP was  mechanically removed, and the die attach remained (Fig.3a).  As confirmed, the electrically conductive die attach was  resistive short to VSS at this step.  Then some portion of die  attach was scratched out by knife manually, and separated in 5  PIN1


EP


VSS


VDD  VSS


PIN1


divisions, 4 edges and 1 die bottom as shown in Fig.3b. They  were electrically isolated each other (as confirmed by I-V  curve tracer).  Then I-V curve between each division and VSS  was measured.  The die attach at edge1 to VSS was resistive  short (Fig.3c).  Other divisions were open to VSS (Fig.3d).  Notably, there was no VSS die pad, wire, or pin at edge1 side.


Figure 3:  (a) EP removed and die attach remained; (b) die  attach separated into 5 divisions, 4 edges and 1 die bottom;


(c) I-V curve of die attach at edge 1 to VSS;(d) I-V curve of  die attach at edge 2,3,4 or die bottom to VSS.


Backside IR-OBIRCH analysis


Infra Red Optical Beam Induced Resistance Change (IROBIRCH) is an effective method to localize a current path.  It  was applied on the EP removed unit from backside. One probe  needle contacted die attach at edge1 and connected to ground.  Another needle contacted VSS pin and biased at 0.07V (0.07V  was chosen for not turning on any p-n junction). The results  were shown in Fig.4.  Several green, red spots (Green means  current decrease by laser heating, red means current increase) were observed along edge1 side. They were not in inner circuit  but in Scribe-Grid Process Control (SGPC) area.


Based on the IR-OBIRCH result, a hypothesis came out. The  excess die attach at edge 1 climbed up the die sidewall and  touched some structures in SGPC area, connecting to VSS. To  confirm this hypothesis, the next analysis was performed from  front side.


Figure 4: Backside IR-OBIRCH and superimposed images. A  couple of green, red spots were observed in SGPC area of  edge1


Physical finding


The CQI unit was de-capsulated (chemically) and die surface  was inspected by optical microscope. There were a series of  exposed test pads (half remained) along die edge1. And no  such pattern was found at other edges.


Figure 5: A series of test pads in the SGPC along edge1 was  found. No such pattern was found at other edges.


In the other hand, SEM inspection on edge1 confirmed that die  attach climbed up sidewall to the die surface.  It did not touch  any die pad or bonding wire. But it did touch the exposed


SGPC test pads (Fig.6) at edge1.


SGPC   test pad


Backside IR-OBIRCH image


Edge1


SGPC


attach  Die


attach


bottom


PIN1  EP removed


Die attach


remained


(d) (b)


Objective lens: 5x


Objective lens: 20x


Figure 6: SEM photos confirmed die attach climbed up  sidewall. Although it did not cross SGPC to the inner circuit  area, it did touch the exposed test pad in the SGPC area.


SGPC pattern inspection


The next was to understand how test pads in SGPC connecting  to VSS. All the bonding wires were removed. SGPC test pads  and inner VSS bonding pads were manually probed to trace IV curve. As shown in Fig.7, these pads (all of the pads in  SGPC area of edge1) were resistive short to inner VSS pads. According to the SGPC information, these test pads were  connected to P type substrate.


Unless otherwise noted DDESP-FM-10 probes were used for  all scans that appear in this presentation.  These are Sb-doped  Silicon probes with a 100nm thick conductive diamond  coating.  The diamond coating significantly enhances the  probe lifetime.  Nominal tip radius is 150nm.  In addition to  DDESP-FM-10s we also tested both platinum-iridium coated  doped silicon probes and solid platinum probes, both with  similar cantilever specifications to the DDESP-FM-10.  Both  were found to produce almost identical measurement  performance to the DDESP-FM-10 at the same settings and  bias with the primary difference being probe lifetime:  platinum-coated probes had noticeably faster wear rates than  diamond-coated probes, while solid platinum probe lifetimes  were significantly higher.


Specifically, while Platinum-Iridium coated probes decayed  noticeably and continuously we could usually maintain enough  sensitivity to complete a few 1x1um scans while still getting  some recognizable signal from defects; by contrast diamond  coated probes usually lasted in the low to high tens of scans  depending on the amount of topographic roughness in the  sample.  Platinum probes showed no scan-to-scan loss of  sensitivity, but would sometimes show a sudden loss of signal.  Based on checks with a tip shape check standard, these events  seem most likely to correspond to the appearance of a foreign  object on the probe.  It is likely that these events are not  exclusive to the platinum probes, but more noticeable where  there is otherwise no loss of sensitivity over time.


Table 1 – table showing the material, coatings, nominal  spring constant and resonant frequency for the probes  discussed in this work.


To provide supporting reference metrology data, TEM  samples were prepared for all samples used in this work.  Both  cross-section and plan-view TEM samples were prepared.  Cross-section samples were prepared using focused ion beam  milling in a scanning electron microscope (FIB-SEM), while  plan view samples were prepared using an etched pits method.  TEM images were taken in dark field and high resolution using  an FEI high-base Titan 80-300 at 300keV.


Defects in III/V on Si


Two main types of crystalline defects were found in the IIIVon silicon materials:  dislocation tangles and stacking faults.  Dislocation tangles (DTs) are one-dimensional and appear as  points where they intersect the surface [8].  Stacking faults (SFs) are planar defects that propagate in a preferred  crystalline axis.  Where they intersect the surface they appear  as a straight line [9].  They frequently have no discernable  impact on surface topography.


If these defects are conductive, both of these defect types can  serve as potentially killer leakage pathways.


Case 1:  Blanket InGaAs with Pits


This sample from early in process development was covered in  small bumps.  Cross-section TEM revealed that many, but not  all, of the bumps were associated with clusters of dislocations.  However, the area between the pits was relatively free of  dislocations, though occasional stacking faults were observed.  With the relatively small surface area TEM could interrogate, however, it was difficult to determine how many of the pits  were decorated with dislocation tangles.


In first testing conductive AFM on this sample, there were a  number of questions we wanted to address.  First, would we be  able to measure the defects at all through the numerous buffer  layers?  Second, would the measurement change the defects  substantially?  Third, would we have sufficient sensitivity to  detect all types of defects present in the TEM data?


Fig 2 – cross-section dark field TEM showing two surface pits  from sample 1, one with dislocations and one without.  Note  also the stacking fault visible in the center of the image.


Scanning the sample in conductive AFM revealed an  extremely high leakage from most of the pits.  Only about 10% of the pits showed no leakage behavior.  Leakage currents in  the pits reached as high as 10 nA.


Fig. 3 – height and current signals from decorated pit in  sample 1.


Stacking faults, though invisible in the topographic image, were also easily detectable from the C-AFM current image.  Leakage current from the stacking faults was much lower, on  the order of 5 to 40 pA when scanned at the normal contact  force


Fig 4 – Topographic image shows two pits and an open area  in the upper right.  The current image revealed a stacking  fault visible as linear area of leakage in the upper right of the  lower image.  Both pits were also decorated.  Current scale  has been adjusted to make it easier to see the stacking fault.


To test if the technique modified the defect in the process of  measurement, a series of static repeatability tests, measuring  one hundred times on each of several sites.  We used a  platinum probe for this test.  From this we found that, using the  above settings, we could consistently scan a single site fifteen  times without substantial loss of signal or observable  topographic damage.


As a result of these initial tests, we found we could detect  conductive defects through the buffer layers, measure signal  strength quite strongly against the background current, and do  so repeatedly and nondestructively.


Case 2:  InGaAs with Scattered DTs


Sample 2 is from later in the development process.  The large  pits no longer appeared in this split.  This particular sample  had relatively weak buffering so that the number of buried  dislocations and surface dislocations were similar.  While this  lead to a very high surface defect density, it meant that HRXRD could be used relatively reliably for reference metrology  as to surface defect density.  Surface defect density for this  sample was measured at 2.5x109 dislocations per cm2 from  modeled HR-XRD peak broadening.


-14000 -12000 -10000


-8000


-6000


-4000


OMEGA-2THETA  (arcsec)


Fig. 5 – HR-XRD spectrum from sample 2.  The central peak  is from the InGaAs, the left from a buried buffer layer, and the  right peak is Si.  From peak broadening, a defect density of


2.5x109 per centimeter was predicted.


This was consistent with the densities visible in plan view  TEM.


Fig. 6 – plan view TEM image from sample 2, showing large  numbers of dislocations in the InGaAs layer.


This distribution of dislocations at the surface, though quite  high, is much closer to types of defects we expect in a mature  process.  Combined with the HR-XRD data this made it useful  for testing how accurate C-AFM detection would be on a more  device-like surface.


Conductive AFM scans on sample 2 showed a random  distribution of point-like leakage sites.  These showed no


correlation to topographic features.  Leakage currents were  comparable to those from stacking faults on sample 1, ranging  from 5 to 25 pA.


Fig. 7 – topographic and current map from the same scan on  a 1x1um area of sample 2.  The dislocations appear elongated  due to the contribution of the tip shape.  Single-pixel current  spikes into the defect leakage range are treated as noise for  purpose of calculating defect density.


After scanning over several hundred cumulative square  microns of the sample surface, we calculated an estimate of the  observed defect density in order to compare to the HR-XRD  and TEM data.  We calculated the estimate by first applying a  threshold filter to the image based on filtering out areas less  than 5x below the peak-to-peak background noise, then using  an Image-J based particle analysis macro to count the number  of localized leakage centers remaining.  Using this method we  estimated an average defect density of 1.4x109 defects per  square centimeter, which agrees fairly well with the HR-XRD  and TEM data.


Using this estimation methodology on several other samples  from different splits has given us results that consistently track  changes in the defect density as measured by TEM and HRXRD.


Similar static repeatability tests were performed on this sample  as on sample 1, and as with sample 1, we found we could scan  at least 15 times on a site without significant loss of signal or  topographic damage.


Case 3:  Aspect Ratio Trap (ART)


As an alternative to or in combination with buffer layers, another method that can be used to reduce some III-V defect  densities is aspect ratio traps (ART).  This involves growing  the III-V material within STI trenches.  Dislocations tend to  terminate in the sidewalls of the trap.  However, the additional  constraint the STI imposes on the III-V material can itself be a  significant


source


of


defects.


Fig 8 - Image from a cross-section SEM showing III-V  material grown within an ART.  Image taken post-CMP.


Aspect ratio trapping is capable of filtering out large numbers  of dislocation tangles.  However, the strain imposed by the  constraint of the crystal can easily cause the formation of large  numbers of stacking faults, as revealed in darkfield TEM:


Fig. 9 – Plan view (upper) and cross section (lower) darkfield  TEM images from InP grown in ART.  The dark bands in the  plan view image are stacking faults visible via diffraction  contrast. They correspond to the lines rising up at an angle in  the cross section image.


Though we grow III-V in ART using many compositions, including InGaAs, the data shown here is InP, not InGaAs. This is because InP was the earliest sample for which we had  post-CMP surfaces of acceptable quality.  TEM and other  results available for InGaAs in ART so far mirror the situation  in InGaAs, so it is our best source of comparison so far.


The density of stacking faults based on the plan-view TEM  data was 8.9x108 per square centimeter, or 3.4x104 per  centimeter if counted linearly along the ART lines.  Scanning  the post-CMP ART with conductive AFM reveals scattered  regions of leakage current, always aligned with the III-V  trenches:


Fig. 10 – topographic and current map from a single scan on  a post-CMP InP ART wafer.  The CMP process at this stage  was still under development:  the STI lines are about 1nm  lower than the InP and some holes appear where InP has been  dislodged.  Areas of bright current appear periodically in the  InP lines but not in the STI.


The current measured the leakage sites visible in the InP is on  the order of 10pA at 1V bias, comparable to that measured  from DTs in InGaAs.


We used a methodology similar to the one described in case 2  to estimate the number of discrete leakage centers above the  noise, with the caveat that we used the noise threshold along  the ART structure only to set the filtration level.  For the  sample shown here, this method estimated 4.2x104 leakage  centers per centimeter of ART.  Estimations made in this  manner have generally scaled with densities measured from  TEM data between samples.


Understanding the effects of defectivity on device performance  is critical for adoption of III-V materials for advanced node


manufacturing.   These defects may be both topographical  and/or electrical and may be either benign or a device killer. Taking a queue from HVM on silicon devices the defectivity  of 3 process steps is investigated using three different  metrology techniques: C-AFM, HR-XRD and TEM. The  results of the three techniques are compared and have shown  good correlation and complementarity.


On case 1, blanket InGaAs with pitting, the cross section TEM  shows both pits decorated by dislocations and undecorated  pits.  The C-AFM shows that about 10% of the pits measured  show no leakage behavior.  These pits correspond to the  undecorated pits whereas those pits that show a strong leakage  signal correspond to those pits decorated with dislocation  defects.


The wide area distribution of dislocation tangles was measured  with plan view TEM, HR-XRD and C-AFM for case 2.  Case  2 represents a later step in the process. The density of these  defects correlated well between the three techniques at  approximately 109 cm-2.


Lastly, the density of stacking faults induced by the aspect  ratio trapping structures used to contain the dislocation tangles  was measured by both C-AFM and plan view TEM for case 3. Again here, the location and densities of the stacking faults as  measured by both techniques is similar.


Table 2: Summary of Results


The results of this work demonstrate that the three techniques  used here provide excellent complimentary metrology  techniques for defect identification and characterization for  III-V semiconductors.


The authors wish to acknowledge Kathleen Dunn of the SUNY  College of Nanoscale Science and Engineering for assistance  with TEM reference metrology and interpretation, PY Hung of  SEMATECH for assistance with HR-XRD, Tommaso Orzali  and Tom Dyer for assistance with sample preparation and  references.


[1]   Oktyabrsky, S., et al., Fundamentals of III-V  Semiconductor MOSFETs, Springer (New York, 2010), pp. 1-27


[2]  Hopkinson, M., et al., “III-V semiconductor devices  integrated with silicon” Semicond. Sci. Technol., vol. 28 (2013) 090301, pp. 1


[3]   Jesus A. del Alamo, “Nanometre-scale electronics with  III-V compound semiconductors,” Nature, Vol. 479, (2011), pp. 317-323


[4]  Quitoriano, N., and Fitzgerald, E., “Relaxed, high-quality  InP on GaAs by using InGaAs and InGaP graded buffers to  avoid phase separation,” J. Apl. Phy., Vol. 102, 033511 (2007)


[5]   Ferrari, C, et al., “Misfit dislocation and threading  dislocation distributions in InGaAs and GeSi/Si partially  relaxed heterostructures,” Materials Science & Engineering B, Vol. 91/92, (2002), pp. 437-441


[6]   Liu, J., et al, “High-resolution X-ray diffraction analysis  on HVPE-grown thick GaN layers,” J. Crystal Growth, Vol. 311, (2009), pp. 3080-3084


Figure 7: After all bonding wires removed, the I-V curves of  SGPC test pads and VSS inner pad were short


Failure mechanism


Based on the above analysis, the current path is described. The  excess die attach touched the half remained test pads in SGPC  region.  These pads in SGPC contacted to the P type substrate, as same as the VSS die pads in inner circuit region. So SGPC  pads were resistive short to inner VSS pads in die region. Since the excess die attach touched the SGPC pads. Then on  customer board, VDD was resistive shorted to VSS through  the current path shown in Fig.8.


Figure 8: The electrical failure was induced by the current  path “VDD-EP-excess die attach-SGPC test pad-P type  substrate-inner VSS pad-VSS”.


Based on the FA result, the assembly team analyzed the excess  die attach control issue and corrected the process parameter.


Case 2 study


This was a process qualification failure. The failed unit is in an  Enhance Small Outline Integrated Circuit (ESOIC) package. Inside package, two dies (digital die + MOSFET die) are  attached on the single EP.  To be functional, the substrate of  MOSFET die (drain) must be biased at the positive voltage  that provided by external power supply (connected to EP). To  minimize RDS(ON) of the MOSFET, the die was attached with  well conductive die attach. In the other hand, the digital die’s  substrate is GND level.  So the digital die is attached with  electrically insulating (but heat conductive) die attach.


Figure 9: Structure of the device in ESOIC32 package. Two  dies on the single EP. Conductive die attach for MOSFET die  and electrically insulating die attach for digital die.


The failure was resistive short between EP (VPWR) and GND. The problem was observed on the evaluation unit with only  digital die encapsulated.


The first step was to figure out the failure was within die  region or package. The failed unit was manually de-capsulated  from front side and the digital die surface was exposed. No  anomaly was observed by optical inspection. For isolation, all  the bonding wires including VPWR and GND were removed. One probe needle contacted to the GND die pad. Then I-V  curve of EP to the GND die pad was traced.  The resistive  short was observed, as shown in Fig.10b. Considering the  GND die pad connection to high dope p type substrate (low  resistance contact), the short though the electrically insulating  die attach was suspected.


Conductive  die attach  Electrically


insulating die attach


SGPC pad


All bonding wires removed


SGPC pad - SGPC pad


SGPC Pad - VSS


Die attach climb up to  the die surface


Inner circuit area


Die attach touched test  pad (half remained) in  SGPC area


Figure 10: (a) Failure isolation method and DC microprobe;


(b) EP (VPWR) - GND (die bonding pad) I-V curve result of  the failed unit; (c) I-V curve result of a reference.


Front side grinding for IR-OBIRCH


Localization of the short point in the broad die attach area was  the next step. IR-OBIRCH was an effective tool to localize a  current path in a die [4]. But in this case, IR-laser could not  stimulate die attach due to metal layers from top side or thick  EP metal from backside.


Figure 11: (a) The problem to apply IR-OBIRCH; (b) The  front side grinding approach to remove metal layers and  circuits; (c) Microprobe needles to contact EP and silicon for  DC bias applying.


To do IR-OBIRCH, a process which is for backside unit  preparation was applied in this case from front side. A  packaged unit was mechanically grinded from front side until  all metal layers and circuits were removed (only bulk silicon  remained) as shown in Fig.11b.  The high dope P type  substrate of digital die and the metal nodes of EP were  exposed. Then one probe needle contacted the upper (inner) side of the EP (VPWR) plate. Another probe needle was  contacted to the remained silicon surface (GND). The tungsten  needle got a reliable ohmic contact on high doped P type  silicon. IR-OBIRCH was performed by applying 0.1V voltage  on VPWR to GND. As shown in Fig.12, an abnormal  resistance change spot was observed successfully.


Figure 12: An abnormal resistance changed spot was  observed in the IR-OBIRCH image and Superimposed images.


Physical analysis and failure mechanism


Mechanical cross section was performed at the IR-OBIRCH  spot. A particle was found in the die attach. Energy Dispersive  X-ray spectroscopy (EDX) detected silver atoms in the particle (Fig.13).


Figure 13: (a) SEM image of the particle inside the  electrically insulating die attach; (b) EDX result indicated  that silver element in the particle.


Based on this FA result, the assembly process was studied.  The nozzle of die attach is used both conductive and  electrically insulating die attach, alternatively.  It was found  that insufficient cleaning after conductive die attach (Ag paste)


Ohmic contact to  substrate


Package


Bulk silicon remained after


front side grinding


EP metal node


needle


(c)  (b)


caused Ag contamination in electrically insulating die attach.


This paper presented two die attach FA cases. Both of the  failures were the resistive short caused by the die attach.  However, the electrical analysis was not so simple. Comparing  to a generic package FA flow, particular unit handling  approaches are effective to reveal the defects in these two  cases.


In case1, die attach isolation approach and backside IROBIRCH were critical to understand how the excess die attach  touched SGPC pads and induced the EP-VSS short.


In case2, the front side grinding approach allowed the laser to  stimulate the defect effectively. Then the conductive particle  inside electrically insulating die attach was localized by IROBIRCH. Both of the FA results help assembly team to find  the root cause in assembly process and execute the process  parameter correction.


The authors would like to thank the support and  encouragement from quality managers Jason Xu, Helen Zhu  and customer quality engineer Zhong Liu for case1 study. We  also thank product engineer Bin Zhou and Nathan Xu in TSO  team who provided valuable data and supported case2 study.


[1] Chin Lap Sin, et al., "Epoxy Die Attach Challenges in  Miniature and Compact DFN / QFN Packages," Electronics Packaging Technology Conference (EPTC), 2008, Pages: 475 – 480.


[2] Lee Yee Sinn, Tan Chee Eng, “Comprehensive Study of  Epoxy Die Attach Process to Achieve Zero Reject  Performance,” Electronics Manufacturing and  Technology, 31st International Conference (IEMT), 2006, Pages: 230-235.


[3] Rajen Dias, “Failure Analysis Flow for Package Failures,” Desk Reference of Microelectrionics Failure Analysis, 6th  Edition, 2011, Pages: 34-37.


[4] Nikawa, Kiyishi, et al., “Failure analysis case studies  using IR-OBIRCH (infrared optical beam induced  resistance change) method,” Test Symposium (ATS’99) Proceedings,


1999,


Pages:


394-399.


Analysis of InGaAs Epi Defects by Conductive AFM


Aaron Cordes, Tom Dyer


SEMATECH, Albany, NY, USA


aaron.cordes@sematech.org; 518.649.1001


Sean Hand


Bruker Nano Surfaces, Santa Barbara, CA, USA  Sean.Hand@bruker-nano.com;


As the semiconductor industry continues to push the  boundaries of Moore’s law, new device structures and  materials are being introduced to increase device speed and  lower power consumption. This work uses InGaAs as  representative samples to investigate the capability of  conductive AFM to image and characterize electrical defects  in thin films.  As the AFM is a non-destructive technique, the  defects may be re-located by complimentary reference  metrology techniques.  Once the capability of defect detection  and characterization of AFM is demonstrated with respect to  the reference metrology techniques, conductive AFM is used  to characterize the defect density of a set of InGaAs samples  grown under varying process stressed epitaxial conditions.


To date, virtually all manufacturing for large-scale integration  semiconductor devices has been done using silicon as the  active semiconductor material.  Interest within the industry has  steadily increased in switching to III-V semiconductors, such  as GaAs, InP, and others for use in the channel area.  Due to  much higher electron mobility III-V semiconductors promise  to allow designers to drastically lower Vdd without sacrificing  device performance.  This is particularly important for the fastgrowing mobile applications market, where a large reduction  in power consumption and corresponding increase in battery  lifetime would have the most impact [1,2,3].


However, as heterogeneous semiconductors, III-V  semiconductors also introduce new challenges.  They are  considerably more vulnerable to various forms of crystalline  defects, such as dislocations and stacking faults, than  homogeneous semiconductors like silicon.  Furthermore, due  to cost and availability of suitable processing equipment, it is  highly likely that at least the first generations of III-V devices  will be built on silicon. This leads to a lattice mismatch  responsible for a large numbers of new defects near the critical  device area, which cannot easily be gettered away, meaning  they must be filtered by buffering, geometric trapping, or other  screening methods [4, 5].


### Analysis of InGaAs Epi Defects by Conductive AFM


New sources of defects near the device layer and the resultant  need to introduce filtration mechanisms introduces new  challenges for the device integrator. Crystalline defects are  invisible to many metrology techniques introducing new  challenges.  These defects may also be either electrically  active or inactive.  Electrically active defects that form leakage  pathways through the channel will greatly reduce performance  at best, and will kill the device at worst.  Electrically inactive  defects or defects that do not form leakage pathways are  benign, but if their benign status cannot be determined, may  lead to misdiagnosis of failure and/or to expensive, wasted  efforts that have no impact on yield.


As a result, there is high need for a device that can search for  and find critical defects on any developmental III-V device  while discriminating them from non-critical defects.  Ideally, it  should be usable on full wafers mid-process and be nondestructive.  As part of SEMATECH’s III-V on silicon  pathway exploration program, several potential metrology  pathways for dealing with the challenge of III-V crystalline  defects have been evaluated.  As a result of these efforts, conductive AFM, backed up with reference metrology from  TEM and HR-XRD, is the most effective way to monitor and  analyze these defects and discriminate their impact.


Samples


III-V test samples were grown on prime 300mm Si (1 0 0) wafers in an AIXTRON MOCVD chamber.  InGaAs samples  appearing in this paper are grown as blankets.  Because the  primary source of most crystalline defects in these samples is  the lattice mismatch between the underlying silicon and the IIIV material, a variety of buffer layers were inserted into each  with the objective of preventing defects from reaching the  intended InGaAs device layer at the surface.  Most wafers  produced were run as parts of splits designed to test the effects  of varying buffer conditions.


Fig. 1 – a TEM cross-section image of several buffer layers in  a III-V on silicon wafer.  Note the very large number of  defects originating at the bottom layer (Si) and the  progressively lower concentrations moving up through the  stack.


Samples presented here are numbered to indicate different  buffer layers or filtering schemes, which in turn correspond to  different surface defectivity conditions.  These surface features  are the defects that are ultimately of interest to us.


Measurements


Test wafers emerging from the MOCVD chamber were prescreened for surface topography in a full-wafer AFM and for  bulk defectivity by full-wafer HR-XRD.  Numerous samples  were run to test diverse buffer combinations and many were  scrapped due to AFM and/or HR-XRD data showing gross  problems.


HR-XRD provides a fast method to measure surface  defectivity but, because it penetrates deep into the buffer  layers, does not necessarily reflect defectivity at the surface.  It  also measures only a general level of crystalline defectivity  due to peak broadening, giving no direct information on  electrical impact [6].


Samples identified as being of interest after pre-screening as  above were then diced for distribution to various surface  defect measurement technologies, of which the most successful  so far has been conductive AFM.  . Conductive AFM  measurements were made on a Bruker Dimension Icon AFM, using conventional C-AFM mode. Measurements were  performed on both intact 300mm wafers and on diced  coupons.


Conventional conductive AFM (C-AFM) operates by scanning  the tip in contact mode, applying a bias from the tip through  the sample, and measuring the current.  Measurements were  made with a 100nN force and 1.5V bias.  The force was  calculated using a spring constant calibrated using a thermal  tune method, and the deflection sensitivity calibrated using a


sapphire standard sample.  The technique is described in detail  elsewhere.  [7]


[4] R. E. Stallcup II, Z. Cross, W. James, P. Ngo, “Measuring  Static Noise Margin of 65nm Node SRAMs using 7-point  SEM Nanoprobing Technique,” Proc. of 33rd ISTFA 2007, pp  223-225.


[5] M. K. Dawood, T. H. Ng, P. K. Tan, H. Tan, S. James, P. S. Limin, Y. Huang, J. Lam, Z. H. Mai, “Study of Static Noise  Margin and Circuit Analysis on Advanced Technology Node  SRAM Devices By Nanoprobing.” Proc. of 39th ISTFA 2013, pp 505-510.


[6] G. Nagatani, K. Yu, An. Del Rosario, M. Sidorov, R. E. Stallup II, J-A. Gray, “Fault Isolation of Sub-surface Leakage  Defects Using Electron Beam Induced Current  Characterization in Next-Generation Flash Memory  Technology Development,” Proc. of 36th ISTFA 2010, pp 62-65.


### Failure analysis of bit line to SNC leakage fail in 2xnm DRAM using Nano- Probing technique


Failure analysis of bit line to SNC leakage fail in 2xnm DRAM using NanoProbing technique


Jaeho Won, Jundong Kim, Jina Kim, Jihye Shin, Jihoon Kim, Kyungrim Lee, Miae Yoon,  Jonghak Lee*, Jaeyoon Lee*, Weonjoon Suh, Hyeonsoo Kim


R&D Division, *DRAM Development Division, SK Hynix Semiconductor, Ichon-si, Gyeoggi-do, Korea


Leakage current from bit line to SNC (Storage Node Contact) is one of the most critical issues in DRAM operation. Such  failure becomes more difficult to visualize as the device  shrinks. In this study, bit line to SNC leakage fail was analyzed  using nano-probing tool in 2xnm DRAM technology.


DRAM (Dynamic Random Access Memory) has various  leakage current issues. Numerous reports have been published  on leakage current issues such as junction leakage, GIDL (Gate Induced Drain Leakage), subthreshold leakage and oxide  tunneling current [1]. DRAM consists of periodic cell array. Fig.1 show diagrams of DRAM cell that consists of one  transistor and one capacitor (a) and cell array (b). Leakage  current of cell array is considered as an important issue  because it is the reason for various failures. Bit line to SNC  leakage, SN (Storage Node) leakage current and word line to  bit line leakage seem to be majority [2][3][4]. These kinds of  failures are called “marginal fail”. Such marginal failure is not  found easily by conventional physical failure analysis  methodology.


Fig. 1: Circuit diagram of a single DRAM cell (a) and cell  array with sense amp (S/A) and sub-word line driver (SWD) (b).


Bit line to SNC leakage failure is a major factor in yield loss. It is caused by physical short between BLC (Bit Line Contact) and SNC. As device scales down, failure analysis using TEM (Transmission Electron Microscopy) cross section image has  limitations which makes it difficult to find the reason of bit  line to SNC leakage failure. Thus, new failure analysis  methods are required to define the leakage current path in the  cell.


In this study, we measured electrical behavior of bit line to  SNC leakage failure by indirectly probing contact in cell array  in 2xnm DRAM technology.


Electrical Test


In this process of electrical test, we could keep track of exact  addresses of the failed cells in a DRAM tester (MOSAID  MS4205). The general test procedure of bit line to SNC  leakage is as follows:


1) Data of „0‟ is written to all cells.


2) High voltage is applied to all bit lines, then it is paused for 1 second.


3) Read the data of previously written cells to judge whether the cells keep the „0‟ data or not. Failed cells show data of „1‟ instead of „0‟ due to bit line to SNC leakage.


The test procedure is described in Fig. 2.


Fig. 2: Electrical test process to find bit line to SNC leakage.


Experimental Conditions


Sample was prepared to probe by mechanical polishing. In  order to separate bit line and gate from interaction of  transistors on S/A and SWD, metal lines were cut using FIB (Focused Ion Beam). Fig. 3 shows SEM images of S/A and  SWD after etching.


Depending on the gate bias, the gate could be turned on as a  result floating SNC bias is changed by the swing bias of  selected bit line. At this state, we can measure leakage current  between neighboring bit line and SNC without probing on  SNC as shown in Fig. 4.


Bit line voltage was varied from 0V to 5V, in step of 0.02V  at the different gate bias levels (0V/ 3V/ 3.5V/ 4V). Well bias  was -0.8V and neighboring bit line bias was connected to  ground level. This measurement was carried out at room  temperature.


Fig. 3. SEM images of prepared sample to test bit line to  SNC leakage.


Fig. 4. Schematic diagram of bit line to SNC leakage  sample for nano-probing analysis. (a) Simplified memory cell  structure (b) circuit diagram of a cell array


Fig. 5 shows I-V curves of the failed and the normal cells, as  the gate bias increased from 0 to 4V. Where I is the selected  bit line current and V is the selected bit line voltage. In Fig.5 (a), the current is low when no charge injected into the failed  SNC (gate voltage = 0) from the bit line. Current increase by  charge injection at high gate voltage (>3V). However current  of normal cell does not vary by increasing gate voltage from 0  to 4V ( Fig. 5(b)).


The currents are constant, as can be seen on the I-V curve  region 1 because probe tips do not contact the SNC directly.  In fig. 5, source of leakage current is not physical short but a  dielectric leakage between bit line and SNC. This indicates  that the failed cell has some marginal weak structure or  material properties. Generally, dielectric leakage current can  be explained by carrier transport. We assumed that the bit line  to SNC leakage current was induced by conduction processes  through insulators like MIS (Metal Insulator Semiconductor) capacitor. The possible causes of this leakage are as follows: Tunneling, Thermionic emission, Frenkel-Poole emission,


Ohmic conduction, Ionic conduction and Space-charge-limited


Fig..5. I-V curves for failed (a) and normal cell (b)


In the 2xnm DRAM, the spacer between bit line and SNC is  very thin (usually < 20nm). We assumed that conduction  through insulator would be tunneling current which depended  on the electric field, insulator thickness and barrier height.


Tunneling current can be subdivided into direct tunneling and  Fowler-Nordheim(F-N) tunneling. F-N tunneling occurs when  the applied voltage V>(b-E0)/q and direct tunneling  phenomena dominate when V<(b-E0)/q. From Fig.5 (a), region 2 (bit line voltage < 3V) can be explained by direct  tunneling current mechanism.


On the other hand, the F-N tunneling phenomena is dominant  at high voltage as can be seen on the I-V curve plot region 3 (Bit line Voltage >3V) [6].


To verify the leaky point, the failed cell was examined using  TEM. TEM observation results were shown in Fig. 6. Thinning of the nitride spacer between BLC and SNC was  found at the failed cell. The nitride spacer thickness of failed  cell is almost half of the spacer thickness in a normal cell. Overlap dimension of BLC with active area of failed cell was


also misaligned. These misalignment led to under-etch of  BLC, and thinning of nitride spacer. Decrease of nitride spacer  thickness resulted in the increase of electric field leakage  through the nitride spacer.


Fig. 6. Cross-section TEM image of failing and normal cell.


The current through the nitride layer is controlled by direct  tunneling. The direct tunneling current calculation is derived  from an earlier study by Simmons [7] on tunneling current  through thin insulating films [8]. This result is similar to the  graph from theoretical result of previous studies [7] [9].


In this conductive mechanism, the current density (Ji) of  insulator for the low field range is given by [6]


V


q


m





)]


[


/


eff


m








0 (1)


Where meff is the electron effective mass, d is the insulator  thickness, V is the applied voltage, b is the barrier height. The  barrier height and electron effective mass of Si3N4 is 2.1eV  and 0.50m0, respectively [8].


The electric field is determined by [5]


s


i 


E s


Where i and s are the electric fields in the insulator and the  semiconductor, respectively, and i and s are the  corresponding permittivity.


The tunneling current is estimated by the sum of Eq. (1) and  Eq. (2)


i


exp(


bd


aE





    


Where a and b is constant.


In other words, current density is proportional to electric  field, insulator thickness and barrier height. If it is difficult to  increase thickness of insulator, an alternative is replacement of  insulating material with higher barrier.


With the continuous scaling down of DRAM devices, bit line  to SNC leakage current has a major impact on yield. In the  case presented here this failure appears as a “marginal fail”. In  this study, we measured the leakage current in 2xnm DRAM  using nano-probing without contacting the cell. This leakage  current measurement method in the cell is a good reference for  DRAM or similar circuit design. In addition to this electrical  measurement will be useful to clarify failure in sub-2xnm  DRAM.


[1] Kaushik Roy, Saibal Mukhopadhyay, Hamid MahmoodiMeimand, “Leakage current Mechanisms and Leakage  reduction Techniques in Deep-submicrometer CMOS  Circuits”, Proceedings of the IEEE, Vol.91, No. 2, FEB


2003.


[2] Martin Versen, “DRAM Failure Analysis and Defect  Localization Techniques”, Microelectronic Failure  Analysis Desk Reference, 6th Edition, pp. 104-110, 2011


[3] Yu-Ching Yeh, Chia-Lung Lin, Bi-Jen Chen, Yuan-Wei  Tseng, Jeremy D. Russell, “Application of Atomic Force  Probing on 90nm DRAM Cell Failure Analysis”, Proceeding of 13th IPFA, pp340-343, 2006.


J i


2d





exp


d


[4] Bonggu Sung, Daejung Kim, Yongjik Park, Joo-Sun Choi,











“A new approach for screening retention time failure bits  in DRAM device”, Proc 39rd  Int’l Symp for Testing and  Failure Analysis, San Jose, California, pp403-406, Nov. 2013


[5] S. M. Sze, Kwok K. Ng, “Physics of semiconductor  device, 3rd Edition, New York: Wiley, Ch. 4.


[6] G. Chakraborty, S. Chattopadhyay, and C. K. Sarkar, C. Pramanik, “Tunneling current at the interface of silicon  and silicon dioxide partly embedded with silicon


id


nanocrystals in metal oxide semiconductor structures”, J. Appl. Phys., 101, 024315, 2007


[7] J.G. Simmnos, “Generalized formula for the electric  tunnel effect between similar electrodes separated by a  thin insulating film”, J. Appl. Phys., vol. 34, no. 6, 1793-1803, 1963.


[8] Yee Chia Yeo, Qiang Lu, Wen Chin Lee, Tsu-Jae King, Chenming Hu, Xiewen Wang, Xin Guo, T.P. Ma, “Direct  tunneling gate leakage current in transistors with ultrathin  silicon nitride gate dielectric”, IEEE Electron Device  Letters, Vol. 21, No. 11, 540-542, 2000.


[9] Xin Guo, “Tunneling leakage current in oxynitride: dependence on oxygen/nitrogen content”, IEEE Electron  Device Letters, Vol. 19, No. 6, 207-209. 1998


Analysis of an Anomalous CMOS Transistor Exhibiting Drain to  Source Leakage – Its Model and Cause


Yuk L. Tsang1*, Alex VanVianen2, Xiang D. Wang3, N. David Theodore3


1Freescale Semiconductor Inc., Austin, TX  2Freescale Semiconductor Inc., Tempe, AZ  3Freescale Semiconductor Inc., Chandler, AZ


* Now with Globalfoundries, yuk.tsang@Globalfoundries.com


In this paper, we report a device model that has  successfully described the characteristics of an  anomalous CMOS NFET and led to the identification  of a non-visual defect. The model was based on  detailed electrical characterization of a transistor  exhibiting a threshold voltage (Vt) of about 120mv  lower than normal and also exhibiting source to drain  leakage. Using a simple graphical simulation, we  predicted that the anomalous device was a transistor in  parallel with a resistor. It was proposed that the resistor  was due to a counter doping defect. This was  confirmed using Scanning Capacitance Microscopy (SCM). The dopant defect was shown by TEM imaging  to be caused by a crystalline silicon dislocation.


With ever shrinking device dimensions of CMOS  integrated circuit technology, the critical size for  defects that cause circuit failure is becoming ever  smaller. This size reduction trend and process  complexity has made failure analysis extremely  difficult.  Dopant related failures, in particular, in a  single device remains a challenging non-visual defect (NVD) for even ultra high resolution microscopy  techniques such as SCM [1, 2], SMM [3], TEM  holography [4, 5], and SSRM [6, 7]. Complicated  sample preparation and imaging optimization are some  of the obstacles, although a handful of such successful  analyses have been reported on both single crystalline  silicon and poly silicon [8, 9, 10, 11]. Once a precise  fault isolation is achieved, a good knowledge of what  to investigate next before deploying any of these  advanced techniques is essential.  To meet this  requirement and to increase the success rate of any  physical analysis, particularly for subtle NVD types, a  detailed electrical analysis to pinpoint exactly where  and what to look for in the sample is critical. As a


### Analysis of an Anomalous CMOS Transistor Exhibiting Drain to Source Leakage – Its Model and Cause


result of an accurate model based on this electrical  analysis, and with its guidance, appropriate methods  can be effectively utilized to find the defect. This quick  turnaround feedback is important for wafer fabrication  lines, test or design teams to make corrective actions to  address critical yield issues. In this work, detailed  electrical analysis using an Atomic Force Nanoprober (AFP) had led to an accurate physical model. This  model had guided the selection of the dopant mapping  technique to bring out the NVD. In previous work [12], a counter doping defect was identified based on a dual  Vt transistor model for another anomalous transistor.  This time, the counter doping magnitude is of a much  larger extent due to a different cause, resulting in a  different device model. The two models and their  associated defects will be compared. The work  presented demonstrates the importance and usefulness  of accurate modeling of failing devices to achieve  successful failure analysis.


Experiments and model


(1) Electrical characterization


The unit was a customer return found later to be a test  escape. Global isolation pointed to an NFET exhibiting  source to drain leakage. The failing NFET and an  adjacent good NFET are shown in Figure 1. These two  transistors were electrically characterized at the contact  level using atomic force probing (AFP) and compared. The source-drain leakage was confirmed as shown in  Figure 2. The electrical characteristics behaved like a  resistive short. The transistor was then fully  characterized to help understand the failure  mechanism. The gate and source/drain to Pwell  junctions were measured to be normal as shown in  Figure 3.


Figure 1  Optical image of NFET devices that were  AFP probed at the contact level. The device in the red  circle was the fail, yellow was a good for reference.


Figure 2  Two terminal Id-Vd plot showing a resistive  short between Drain and Source in the Fail. The gate  and Well were floating. Ref=good.


Figure 3  Gate (top) and Source/drain junction (bottom) leakages were normal.


The transistor Id-Vg curves were measured at Vd=0.1V, Vs and Vwell=0V and plotted as shown in Figure 4. A  residual current was observed in the failing device.  The  magnitude of this current was about the same as the  Drain to Source current at 0.1V shown in Figure 2. This


current shifted the normal channel current upward  resulting in an apparent Vt delta of about 120mV. At


Reference


Vd=1V, the residual current increased as shown in  Figure 5.


Fail


Figure 4  Id-Vg plots in linear scale showing a residual  current in the failing device. Vd=0.1V, Vs=Vwell=0V.


Figure 5 Id-Vg plots in semilog scale showing a residual  current in the fail. Vd=0.1V and 1V, Vs=Vwell=0V.


(2) Model


Based on the device electrical behavior observed, it  appears that there was a resistor in parallel with the  transistor. To assess this possibility, the resistance was  first determined in the off state as shown in Figure 6. The failing transistor shows a low and reasonably stable  resistance of about 80k-95k ohms in the off state at Vg  below 0.3V while the good transistor (Ref) was  essentially non-conducting. The calculated resistance  and a good transistor were then combined in a parallel  configuration for the resultant effect. The resultant IdVg curve was compared with the failing curve. It was  found that this model had accurately predicted the  failing transistor characteristics as shown in Figure 7.


-1.5E-05-1.0E-05-5.0E-06-2.0E-19


5.0E-06


1.0E-05


-1 -0.6 -0.2 0.2 0.6 1


Vd (V)


Fail Ref


1.0E-14


1.0E-11


[7]   Kremmer, S., et. al, “Modification and characterization of  thin silicon gate oxides using conducting atomic force  microscopy,” Materials Science & Engineering B, Vol. 102, Issue 1-3, (2003), pp. 88


[8]  Kui, J., et al, “Misfit dislocation generation mechanisms in  InGaAs/GaAs heterosctructures,” J. Appl. Phys,. Vol. 76, No. 12, (1994), pp. 7829-7832


[9]   Kimura, Y. et al, “Generation of misfit dislocations and  stacking faults in supercritical thicknesses strained Si/SiGe  heterosctructures,” Appl. Phys. Letters, Vol 88, No. 031912, (2006)


Utilizing Nanoprobing and Circuit Diagnostics to Identify Key Failure Mechanism of  Otherwise Non-Visible Defects in 20nm Logic Devices


M. K. Dawood, C. Chen, P. K. Tan, S. James, P. S. Limin, H. Tan, H. H. Yap, G. R. Low, J. Lam and Z. H. Mai


GLOBALFOUNDRIES Singapore Pte. Ltd.


60 Woodlands Industrial Park D Street 2


Singapore 738406


In this work, we present two case studies on the utilization of  advanced nanoprobing on 20nm logic devices at contact layer  to identify the root cause of scan logic failures. In both cases, conventional failure analysis followed by inspection of passive  voltage contrast (PVC) failed to identify any abnormality in  the devices. Technology advancement makes identifying  failure mechanisms increasingly more challenging using  conventional methods of physical failure analysis (PFA). Almost all PFA cases for 20nm technology node devices and  beyond require Transmission Electron Microscopy (TEM) analysis. Before TEM analysis can be performed, fault  isolation is required to correctly determine the precise failing  location. Isolated transistor probing was performed on the  suspected logic NMOS and PMOS transistors to identify the  failing transistors for TEM analysis. In this paper, nanoprobing was used to isolate the failing transistor of a logic  cell. Nanoprobing revealed anomalies between the drain and  bulk junction which was found to be due to contact gouging of  different severities.


Nanoprobing has become an important and key tool for  electrical failure analysis (FA) in current FA metrology for  fault isolation.[1,2] A typical nanoprobing system comprises  of a Scanning Electron Microscope (SEM), integrated with up  to 8 nano-manipulators with tungsten nanotips, which are  connected to a parametric analyzer. A system with a minimum  of 4 probes is capable of direct transistor characterization at  the contact level, while a state-of-the-art system with 8 probes  allows further on-chip circuit analysis such as studying static  noise margins (SNM) in SRAM cells.[3,4,5] Current systems  may also come equipped with Electron Beam Current (EBC) analysis capabilities which are able to perform Electron Beam  Induced Current (EBIC) and Electron Beam Absorbed Current (EBAC) analysis.[6]


As transistor scaling progresses, fault isolation via  conventional PFA methods such as inspection by passive  voltage contrast (PVC) in an SEM becomes increasingly  difficult to identify abnormalities due to limits with the SEM  and the specific layout design at the region of interest. Such  PFA cases are a key concern for a foundry where rapid fault  isolation and identification is critical for process development  and yield improvement.


In this work, we demonstrate two cases studies on the  utilization of nanoprobing on 20nm logic devices at contact  layer to identify the root cause of the otherwise “non-visible” failures.


Two 20nm technology node scan logic failures, on two  different failed dies were deprocessed layer by layer followed  by SEM inspection using conventional techniques. The failing  cell and its corresponding connections were provided by the  customer. Both samples showed no abnormal PVC on vias and  metals at back end of line (BEOL). PFA was continued until  the front end of line (FEOL) layers were reached. The SEM  PVC technique was unable to determine any abnormalities due  to the way the devices were designed. The samples were  loaded into a DCG nProber system that has 8 nanopositioners. To minimize e-beam induced damages to the transistors, nanoprobing was carried out at a low acceleration voltage of  500eV.[3]


Case 1: 20nm scan chain failure due to severe contact  gouging


Figure 1a shows the schematic diagram of the scan logic cell  of interest. There are three types of contact architecture on this  technology node; the first is the contact which lands on the  silicon, (TS), the second is the contact on the TS layer which  provides connection (CA) and the third is the contact that  lands only on the gate (CB). Silicon is referred to as RX. All  the transistors at TS layer showed no abnormal PVC except  for the two connected NMOS and PMOS devices as shown in  Figure 1b.  This is due to the presence of the dummy gate and  the CB connection between both PMOS and NMOS devices. The scan chain failure was expected to be localized to two  pairs of NMOS and PMOS devices (transistor pair 1 and  transistor pair 2).


Figure 1a: Schematic diagram of the layout of the bad PMOS  and NMOS transistors (Transistor pair 1 and 2) and the  location of a known good device for reference.


Figure 1b: SEM image of the failing location showing no  abnormal PVC.


Nanoprobing was performed on the individual NMOS and  PMOS devices for electrical characterization based on the  following biasing conditions:


Id-Vd: Sweep Vd from 0V to 0.9V. Step Vg from 0.9V by


0.1V. Vs = Vb = 0V.


Id-Vg: Sweep Vg from 0V to 0.9V. Vd = 0.85V and 0.9V. Vs = Vb = 0V.


To determine any abnormalities between the source and drain  junctions, a source sweep was also performed, whereby the  drain and source voltages are reversed. In addition, a  neighboring pair of NMOS and PMOS transistors was  nanoprobed for reference.


Figure 2a and 2b shows the I-V curves of the reference PMOS  and NMOS transistors while Figure 2c and 2d shows the I-V  curves of the bad PMOS transistors. Both NMOS devices  showed no abnormal characteristics.


Figure 2a: Id-Vg and Id-Vd of the Reference PMOS. (Top) shows drain sweep and (bottom) shows source sweep.


Figure 2b: Id-Vg and Id-Vd of the Reference NMOS. (Top) shows drain sweep and (bottom) shows source sweep.


Figure 2c: Id-Vg and Id-Vd of the Bad PMOS1. (Top) shows  drain sweep and (bottom) shows source sweep.


Figure 2d: Id-Vg and Id-Vd of the Bad PMOS2. (Top) shows  drain sweep and (bottom) shows source sweep.


Figure 2e: SEM image of nanoprobing and the respective  probe assignment on Bad PMOS1.


Abnormal transistor behavior was observed for both PMOS  transistors. Diode like I-V curves were observed at the drain  terminal during drain sweep for both devices. In addition, an  abnormally high bulk (n-well) current was observed at both  PMOS transistors. Transistor-like behavior was observed  during source sweep. The results seem to suggest that the  cause of failure may be due to the common drain terminal  between the two PMOS devices. Bulk current on the order of  10-7A was measured at both PMOS transistors compared to 10-10A at the reference PMOS location as shown in Figure 3.


Figure 3: I-V curve of bulk current vs drain voltage for (left) the bad PMOS device and (right) the reference PMOS device. Figure 4 shows TEM analysis which was performed across the  bad PMOS devices. The TEM images show an over-etched  CB which resulted in a drain to substrate short. This explains  the diode-like I-V curve during the drain sweep and the high  drain to bulk current. During the source sweep, both drain and  bulk are grounded and normal transistor curves are obtained. As a comparison, Figure 5 shows the TEM image of a known


good device showing no CB gouge.


Figure 4: TEM images across the PMOS devices showing a  severely over etched CB which resulted in a short to the  substrate. The bottom image is a dark filed image while the  top images are bright field.


Figure 5: TEM images of a known good die showing no CB  gouge as comparison. The bottom image is a dark filed image  while the top images are bright field.


Case 2: 20nm scan chain failure due to less severe contact  gouging


Figure 6 shows the I-V plots of the reference NMOS and the  bad NMOS devices of the second failed die. Unlike the first  die, no abnormality was observed at the PMOS transistors.


Figure 6a: Id-Vg and Id-Vd of the Reference NMOS. (Top) shows drain sweep and (bottom) shows source sweep.


Figure 6b: Id-Vg and Id-Vd of the Reference PMOS. (Top) shows drain sweep and (bottom) shows source sweep.


Figure 6c: Id-Vg and Id-Vd of the Bad NMOS1. (Top) shows  drain sweep and (bottom) shows source sweep.


Figure 6d: Id-Vg and Id-Vd of the Bad NMOS2. (Top) shows  drain sweep and (bottom) shows source sweep.


Figure 6e: SEM image of nanoprobing and the respective  probe assignment on Bad NMOS1.


Though both NMOS devices show normal transistor  characteristics, a closer examination of the bulk current  showed a higher bulk current in both bad NMOS devices  compared to the reference NMOS as shown in Figure 7.


Figure 7: Plot of bulk current vs drain voltage of the respective  NMOS devices.


TEM was then performed across the NMOS devices. Figure 8  shows the resulting TEM images. In this case, a less severe  CB gouging was observed. The gouging was not severe  enough to cause a drain to bulk short however it might account  for the drain to substrate leakage.


Figure 8: TEM images across the bad NMOS devices showing  less severe CB gouging. The bottom image is a dark filed  image while the top images are bright field.


In summary, this work demonstrates the reliance and  importance of nanoprobing for fault isolation especially in  advanced technology nodes where “visible” failures become  increasingly difficult to identify with conventional PFA


techniques. A better understanding of the cause of failure can  be determined by studying the device or circuit behavior  during nanoprobing. In this work we presented two case  studies whereby the severity of contact gouging results in  different electrical behavior; a direct short between drain and  substrate when contact gouging is severe and a high leakage  current when contact gouging is less severe.


We would like to thank the Failure Analysis Department (Singapore) of GLOBALFOUNDRIES for their kind support  in TEM and EDX works.


[1] C-M Shen, T-C Chuang, S-C Lin, L-F Wen, C-M Huang, “Combining the Nano-probing Technique with Mathematics  to model and identify Non-Visual Failures” Proc of 33rd  ISTFA 2007, pp 214-218.


[2] S. L. Toh, Z.H. Mai, P.K. Tan, E. Hendarto, H. Tan, Q.F. Wang, J.L Cai, Q. Deng, T.H. Ng, Y.W. Goh, J. lam, L.C.


Hsia, “Use of nanoprobing as the diagnostic tool for  nanoscaled devices,” Proc. 14th IPFA, 2007, pp.53-58.


[3] T. H. Ng, M. K. Dawood, P. K. Tan, H. Tan, C. K. Oh, J. C. Lam, Z. H. Mai, “Study of Static Noise Margin, Cell  Stability and Influence of Electron Beam on sub-30nm SRAM  Using SEM-based Nanoprobing with 8 Nanoprobes” Proc. of  38th ISTFA 2012, pp112-117.


1.0E-08


1.0E-02


-2 -1.5 -1 -0.5 0 0.5 1 1.5 2


Vg (V)


1.0E-12


1.0E-10


1.0E-06


1.0E-04


-1 -0.5 0 0.5 1 1.5 2


Vactive (V)


S/W -Fail D/W -Fail S/W -Ref D/W -Ref


1.5E-05


2.0E-05


GATE DRAIN


2.5E-05


ISO


BODY


SOURCE


3.0E-05


-0.5 0


Ref Fail


1.0E-13


1.0E-09


1.0E-07


-0.5-0.1 0.3 0.7 1.1 1.5 1.9 2.3


Fail Vd=0.1v Ref Vd=0.1v Fail Vd=1v Ref Vd=1v


Figure 6  Channel resistance as a function of gate bias. The Fail shows a low and reasonably stable resistance  in the off state while the Ref is essentially nonconducting.


Figure 7 Model and measured Id-Vg (Vd=0.1V) data


Height profile


comparison showing excellent match. Linear (top),


2.5mm


semilog (bottom) and R is the resistor Id.


Defect identification


The model suggested that a possible cause could be  counter doping on part of the channel linking the  source and drain. This hypothesis can be evaluated  using Scanning Capacitance Microscopy (SCM) analysis. Another possibility is a continuous  conducting stringer linking source and drain. Top-view  SEM imaging after progressive delayering to bare  silicon did not find any stringer. SCM analysis was


next performed on the bare silicon sample. The planar  view SCM dopant mapping image indeed revealed  counter doping across the entire channel length  bridging source and drain as shown in Figure 8.


Figure 8 Planar view SCM dopant mapping images at  various bias conditions. An n-type band (circled in red) across the p-type device channel, bridging Source and  Drain, is observed. (n-type = brown contrast, p-type = bright contrast)


Topography image also revealed a step height of about


0.8nm at the n-type band as shown in Figure 9.


Figure 9 Topography image of the SCM area revealed  a step of 0.8nm high at the n-type band as indicated by  the red arrows. The height profile represents the  section through the dark dashed line. The step  occurred along the red dashed line.


It was therefore suspected that this counter doped band  was the result of enhanced dopant diffusion along a  silicon crystalline defect. Planar TEM analysis was  further performed for additional insight about the  defect. At the step height where the n-type counter


1.0E+00


1.0E+02


1.0E+04


1.0E+06


1.0E+08


1.0E+10


1.0E+12


-1.5 -1.1 -0.7 -0.3 0.1 0.5 0.9 1.3


Active area


Active area below below silicide


-0.5 -0.1 0.3 0.7 1.1 1.5 1.9 2.3


below silicidegate oxide


block


2.50


R


Ref


R+Ref (Model)Fail


5.0mm


1.25


~0.8nm high step


R+ref (Model)


Reference  device


Failed  device


Vb = -0.5V


Vb = 0V


Vb = 0.5V


Source  Channel  Drain


5mm 0


5mm


doping band occurred, a silicon dislocation line  traversing the entire channel length was indeed  revealed as shown in Figure 10. This crystalline silicon  defect will allow for enhanced diffusion [13] from the  heavy n-type source and drain dopant. As a result, the  counter doped band was formed creating the leakage  path.


Figure 10 Planar view TEM images of the failing  transistor channel region. The low magnification  image (top) encompassed the entire channel. The high  magnification image (bottom) revealed a silicon  dislocation line across the entire channel length at the  step height where the n-type counter dopant band  occurred.


At this point, we firmly established the validity of the  model for the failing transistor behavior and the root  cause of the defect.


Comparison with previous work


Counter doping defect was reported in ISTFA 2012


[12] for another anomalous transistor. The proposed


device model was two transistors in parallel having two  different Vt’s. One of the transistor’s Vt was low while  the other was normal.  The cause was due to counter  doping of a portion of the channel length that resulted  from implant penetration. The present model for  another anomalous transistor was a transistor in parallel  with a resistor also caused by counter doping, but  across the entire channel length due to a silicon  crystalline dislocation. The two models and defect root  causes are summarized in Table 1.


Table1 Model and defect comparison


A MOSFET exhibiting excessive source to drain  leakage was successfully modeled as a device formed  by a transistor and a resistor in parallel. The hypothesis  of a channel counter doping defect as one of the two


most likely causes, based on electrical characterization  data, was verified by SCM dopant mapping technique  that revealed an n-type counter doped band linking  source and drain. TEM analysis showed that a silicon  dislocation was the root cause. Comparisons with


previous work indicated that the device model is  dependent on the magnitude of the counter doping in  the channel due to different root causes.


The authors would like to thank the Freescale  Semiconductor Product Analysis Labs for technical  support.


[1] C. C. Williams, “Two-Dimensional Dopant Profiling  by Scanning Capacitance Microscopy” Annual Review  of Materials Science, 29, 471-504(1999) Capacitance


Previous work [12]


Present work


Model


Two transistors in  parallel, Vt’s being  different


A resistor in  parallel with a  transistor


Defect


Counter doping of a  portion of the channel  length


Counter doping  across entire


channel length


Root  cause


Ion implant through  large poly grain


boundary


Crystalline silicon  dislocation


Microscopy” Annual Review of Materials Science, 29, 471-504 (1999)


[2] F. Giannazzo, D. Goghero, V. Raineri, S. Mirabella, F. Priolo, “Scanning Capacitance Microscopy on Ultra  narrow Doping Profiles in Si”, Applied Physics Letters, 83(13), 2659 (2003).


[3] W. Han, “Introduction to Scanning Microwave  Microscopy Application”, Agilent Application Note, June 16, 2008


[4] W. D. Rau, P. Schwander, F. H. Baumann, W. Höppner, and A. Ourmazd, “Two-Dimensional Mapping  of the Electrostatic Potential in Transistors by Electron  Holography”, Phys. Rev. Lett. 82, 2614 (1999).


[5] M. A. Gribelyuk, M. R. McCartney, Jing Li, C. S. Murthy, P. Ronsheim, B. Doris, J. S. McMurray, S. Hegde, and David J. Smith, “Mapping of Electrostatic


Potential in Deep Submicron CMOS Devices by  Electron Holography”, Phys. Rev. Lett. 89, 25502 (2002)


[6] P. Eyben, S. Vemula, T. Noda and W. Vandervorst,


“Two-dimensional Carrier Profiling with Sub-nm  Resolution Using SSRM: From Basic Concept to TCAD  Calibration and Device Tuning”, Ext. Abs. the 9th  International Workshop on Junction Technology 2009, p24-28.


[7] L. Zhang, K. Ohuchi, K. Adachi, K. Ishimaru, M. Takayanagi, A. Nishiyama, “High-resolution  characterization of ultra shallow junctions by measuring


in vacuum with scanning spreading resistance  microscopy”, Applied Physics Letters, 90(19), 192103 (2007)


[8] K. Jarausch, J. F. Richards, L. Denney, and A. Guichard, “Site specific 2-D implant profiling using FIB  assisted SCM”, Proceedings of the 28th International  Symposium for Testing and Failure Analysis, p467, Phoenix, Arizona, 2002.


[9] D. K. Fillmore, and S. Wang, “Investigation of LowEnergy Focused Ion Beam Milling for Scanning  Capacitance Microscopy Sample Preparation”, Conference Proceedings from the 30th International


Symposium for Testing and Failure Analysis, p350, Worcester, Massachusetts, 2004.


[10] Xiang-Dong Wang, Yuk Tsang, and Clifford  Howard “X-sectional Scanning Capacitance Microscopy (SCM) Applications”, Conference Proceedings from the  36th International Symposium for Testing and Failure  Analysis, p 98, Dallas, TX, 2010


[11] Yuk Tsang, Xiang-Dong Wang, Michael


Mendicino, Andrew Blankenship, “A case study: Observation of counter doping of gate poly and its  validation in high density 90nm CMOS SRAM Bitcell”, Conference Proceedings from the 36th International  Symposium for Testing and Failure Analysis, p 66,


Dallas, TX, 2010


[12] Yuk Tsang, Xiang-Dong Wang, Reyhan Ricklefs, Jason Goertz, “Analysis of an anomalous transistor  exhibiting dual-Vt characteristics and its cause in a


90nm node CMOS technology”, Conference  Proceedings from the 38th International Symposium for  Testing and Failure Analysis, p106, Phoenix, AZ, 2012


[13] G. H. Plantinga, “Influence of dislocations on  properties of shallow diffused transistors”, IEEE  Transactions on Electron Devices, Vol. 16 (No. 4), 394 – 400 (1969).


### Feature Based Non-Destructive Fault Isolation in Advanced IC Packages


Feature Based Non-Destructive Fault Isolation in Advanced IC Packages


K.C. Lee, J. Alton, M. Igarashi


TeraView Limited, Cambridge, CB4 0DS, United Kingdom   Email: kc@teraview.com; Tel: (44) 1223 435380


S. Barbeau


IBM Microelectronics, Bromont, QC, Canada


Traditional time domain reflectometry (TDR) techniques  employ time-based information to locate faults within  packages with minimal references to internal structures. Here, we combine a novel and innovative technique, electro optical  terahertz pulse reflectometry (EOTPR) [1], with full 3D  device-under-test (DUT) modelling to quickly and nondestructively perform feature-based analysis. We demonstrate  fault isolation to an accuracy of 10 µm or better with respect to  device features in an advanced integrated circuit (IC) package.


The challenges within IC failure analysis are increasing with  the continued miniaturization and greater complexity of  advanced devices. Key among these challenges is the nondestructive localization of electrical failures, prior to the  destructive investigation. Defect pre-localization has become  increasingly important in new generation products, such as 3D  packages where the package geometry is both highly complex  and fragile. Until recently, an accuracy of around 1 mm was  acceptable for most defect localization in IC package FA.  However, this is no longer the case for the new generation of  products. Consider the typical stacked dies of a 3D package,


the whole chip stack height can be less than 1 mm, and the  distance between two interconnects can be less than 20 µm in a  silicon interposer package with TSV technology. Thus, nondestructive fault isolation techniques with an accuracy of much  less than 20 µm are required [2-5].


EOTPR is a proven technique for localizing defects to within  10 µm accuracy [1-5]. During operation, electrical pulses are  launched into the DUT via a high frequency circuit probe (Figure 1b). Reflections from device structures and faults are  recorded as a voltage-time signal, known as an EOTPR  waveform, by a fast photoconductive switch. Deviations of the  DUT waveform from a reference waveform indicates the  presence of a fault. In previous studies, the velocity factor  calculated from a measured reference device converts the  voltage-time DUT waveform into a voltage-distance signal for  fault isolation. This broadband technique has an extremely low  time base jitter and high temporal resolution [1].


Here, we use a commercially available electromagnetic (EM) simulation package to run a full 3D analysis to generate the  reference EOTPR waveform (Figure 1a). Through the  simulation, EOTPR pulse propagation can be monitored in  virtual real time, and allows accurate correlation of reference  EOTPR waveform features to key design elements in the DUT.  This enables faults to be located accurately with respect to  device structures, taking full account of the varying pulse


Figure 1: (a) Top-down and (b) bottom-up views of a combined substrate/probe 3D model.


propagation velocities in different parts of the DUT. This


approach improves on the constant propagation velocity  approximation of the measurement-based reference generation  and allows accurate fault isolation in devices of arbitrary  complexity.


Measurement


An EOTPR system comprises two photoconductive switches (PCS), one functioning as an electrical pulse source and the  other as an instantaneous current detector activated by a mode-


EOTPR pulse reflected from open probe tip


locked near infrared laser. The emitted pulse is coupled into  the DUT through a co-axial cable and a high frequency probe, while the reflected pulse is directed into the PCS detector. A


translation stage in the detector beam path sweeps the relative  delay between the emission and detection timings (Figure 2a), generating a continuous voltage-time waveform for the user


(Figure 2b shows an example waveform from an open probe).


To enable meaningful comparison with a model generated  reference waveform, we minimize the effect of system


300


response on the measured waveform by applying a postTime (ps)


processing procedure. The detail of the post-processing, involving the generation of a deconvolution function from the  probe open/short waveforms, can be found in the Appendix.


To capture accurately the electromagnetic response of the  DUT, we use a commercially available EM simulation tool  which employs the finite difference time domain method (FDTD) [6] to calculate the transient EM behaviors through  Maxwell’s equations. This approach bypasses the need for  phenomenological quantities such as capacitance and  inductance, and all inter-conductor couplings behaviors arise  naturally as a result.


In this study, we model a signal trace (designated BR300) in a


Figure 2: (a) Schematic of an EOTPR system; (b)


Typical raw EOTPR waveform from the open end of


a high frequency probe.


Figure 3: Cross section image of a sub-volume of the  package substrate model after it has been set up for  simulation. Grey lines indicate the mesh grid; conductors are in green; dielectric regions are in pink.


Figure 4: Zoomed-in view of the BGA side of package. 'r' is  the transverse radius of the BGA; 'h' the vertical separation  between package surface and probe tip.


typical flip chip package substrate. The 3D structure is built  directly from the 2D design files. After importing the design, we add the dielectric coatings, ball grid array (BGA) and a  high frequency probe to form the structure shown in Figure 1a. The combined probe-package model is spanned by around 32  million mesh cells and is bounded by perfectly matched layers (PMLs) on all sides. The mesh settings have been set  sufficiently high to resolve all of the fine features in the  device, and the PMLs absorb all stray EM fields (Figure 3). We import the structure with a greater than 1 mm buffer  around the BR300 trace to ensure that the PML boundaries  have no impact on the electrical impedance of the signal path. Further, we extrude all structure faces touching the model  boundaries by 100 µm to ensure perfect absorption at the PML  interface. Virtual voltage monitors placed at regular intervals  along the signal trace provide a convenient method for in-situ  monitoring of the propagating pulse. A pulse is injected from  the high frequency probe and the back reflections are recorded  as the raw DUT waveform.


Once the structure is created we perform a least square  optimization to match the simulated waveform from the  BR300 trace to a measured reference device. We utilize a  principle component analysis optimization algorithm to  dynamically adjust:


i. BGA solder ball radius (r in Figure 4),


ii. The normal separation between package surface and  probe tips (h in Figure 4),


iii. The dielectric permittivities in the package.


By varying the permittivities, we compensate for surface  roughness in the conductors and other deviations in the  manufactured device from the nominal design parameters. Further, separate models of open- and short-terminated probes  are created and these waveforms are used to deconvolve the  raw DUT waveform. The optimization procedure compares the  deconvolved simulated and measured waveforms since these  are broadly independent of the injected pulse profile.


This optimization procedure should be performed once for  each new device type, and once complete allows accurate  simulations of other traces in the device to be obtained using  the optimized parameters.


Figure 5 shows the transient voltage signals detected by  voltage monitors placed at some of the key points in the  optimized model (as labelled in Figure 1a). Here, the pulse  propagates clearly to the end of the substrate trace, which has  an open C4 termination. These voltage signals provide crucial  time of arrival information that can be used to unambiguously  identify features in the reflected EOTPR waveforms as well as  calculating the velocity factors for the pulse in different parts  of the package.


Figure 6a compares the deconvolved, measured, and simulated  EOTPR waveforms for the reference BR300 trace. A clear  open reflection is observed from the C4 termination, and is  consistent with the equivalent voltage monitor signal. The  near-complete level of agreement between the model and  measured data reflects the accuracy of the FDTD modelling  approach.


Figure 6: (a) Comparison of a measured reference BR300  trace (red) to the optimized model waveform (blue); (b) zoomed-in views around the C4 reflection. Superposed are the  measured (yellow) and model (green) waveforms of a faulty  device.


Figure 5: Transient voltage signals extracted from monitors  placed at key points in the optimized BR300 model. Monitor  placement labels correspond to the indicated locations in  Figure 1a.


Following the completion of the EOTPR model optimization, we then introduced an open fault 3 mm before the C4  termination in the physical sample and obtained a new  waveform. As shown by the yellow trace in Figure 6b, the  pulse is now reflected at the open fault rather than the C4, consequently we see a forward shift in time in the termination  peak from 200 ps (red) to 160 ps. By applying the velocity  factors derived from Figure 5, we infer the location for where  the open fault lies, created a virtual cut at the same point in the  model (shown in Figure 7) and ran the new simulation without  further changes. As illustrated by the green waveform in  Figure 6b, the resulting open reflection matches well with the  measured waveform of the failed device, and act as a further  demonstration of the modelling capabilities.


In this study, we have demonstrated a new fault analysis  workflow combining a high precision EOTPR tool with the  construction of a virtual known good device (KGD) or golden  device through an electromagnetic simulation package. The  resulting near-perfect correlation between measurement and  simulation establishes both the accuracy of the hardware as  well as the simulation technique.


The modelling also enables a new level of understanding of the  EOTPR waveforms. Previously, an accurate fault location was  calculated by measuring the flight of time of EOTPR pulses  and converting this to a distance by applying various velocity  factors. By knowing the nearest major feature locations, users  can now analyze the EOTPR waveforms based on features in  the DUT. Moving from time-based analysis to feature-based  analysis of the EOTPR waveforms, users can shorten the  analysis time and improve the accuracy of their analysis.


The fault isolation capabilities of the modelling is  demonstrated through a test study of an artificially created  open fault, and subsequently verified by physical  measurement. The methodology employed here is suitable for  use in highly complex 3D IC packaging structures which  contain small features such as microbumps and TSVs, and


expands the capabilities of the EOTPR toolkit in an easily  assessable manner.


[1] Y. Cai, Z. Wang, R. Dias, and D. Goyal, "Electro Optical  Terahertz Pulse Reflectometry - an Innovative Fault  Isolation Tool", Proceedings of the 60th Electronic  Components and Technology Conference (ECTC), Las  Vegas, Nevada, USA, June 1-4, pp. 1309-1315, 2010.


[2] S. Barbeau, J. Alton, M. Igarashi, “Electro Optical  Terahertz Pulse Reflectometry - a fast and highly accurate  non-destructive fault isolation technique for 3D Flip Chip  Packages”, Proceedings from the 39th International  Symposium for Testing and Failure Analysis, 2013, San  Jose, California, USA, November 3–7, pp. 264 – 269.


[3] M. Y. Tay, L. Cao, M. Venkata, L. Tran, W. Donna, W. Qiu, J. Alton, P. F. Taday, and M. Lin, "Advanced Fault  Isolation Technique Using Electro-optical Terahertz Pulse  Reflectometry", Proceedings of the 19th International  Symposium on the Physical and Failure Analysis of  Integrated Circuits (IPFA), Singapore, July 2-6, 2012.


[4] L. Cao, M. Venkata, M. Y. Tay, W. Qiu, J. Alton, P. F. Taday, and M. Igarashi, "Advanced Fault Isolation  Technique Using Electro-optical Terahertz Pulse  Reflectometry (EOTPR) for 2D and 2.5D Flip-chip  Package", Proceedings of the 38th International  Symposium for Testing and Failure Analysis (ISTFA), Phoenix, Arizona, USA, November 11-15, pp. 21-25,


[5] Alton, J. and Igarashi, M., “Non-Destructive Fault  localization in Advanced IC Packages Using Electro  Optical Terahertz Pulse Reflectometry,” IEEE  Microelectronics Packaging Conference (EMPC), 2013  European, Grenoble, September 2013, pp. 1-4.


[6] Yee, K., “Numerical Solution of Initial Boundary Value  Problems Involving Maxwell’s Equations in Isotropic  Media,” IEEE Transactions on Antennas and  Propagations, Vol. 14, No. 3 (1966), pp. 302-307.


Appendix


Post-processing algorithm


The measured waveform from an EOTPR is a function of the  pulse shape that enters the DUT. Here, we obtain the signal  function at the probe tip using linear combination of the  measured open- (o(t)) and short-terminated (s(t)) probe  waveforms (t represents time). The algorithm is as follows:


r(t) = (o(t) - s(t))/2


b(t) = (o(t) + s(t))/2


Figure 7: Model of package with a simulated open fault.


r(t) and b(t) are the ‘reference’ and ‘baseline’ signals and they  represent the input pulse shape and reflections from elsewhere  in the system.


For ease of computation, we perform the following  deconvolution in frequency (f) space. Let D(f) represents the  Fourier transformed raw DUT waveform, then the post  processed waveform is given by the inverse Fourier transform  of A(f), where:


A(f) = (D(f) – B(f))/R(f)×G(f)


B(f) and R(f) are the Fourier transforms of b(t), r(t) respectively. G(f) is a Gaussian function in frequency space  and acts as a frequency filter.


A(f) is a function that depends on the DUT and the timedomain version of the waveform a(t) is used for comparison  with simulation results in this study (also post-processed as  outlined here).


Failure Mechanism Studies and Root Cause Identification of   Non-Stick on Pad on Microchip Al Bondpads


Hua Younan, Zhou Yongkai, Chen Yixin, Fu Chao and Li Xiaomin


10 Science Park Road, #03-26 & #03-28, The Alpha Building  Singapore Science Park II, Singapore 117684


Email:Younan@wintech-nano.com


It is well-known that underetch material, contamination, particle, pinholes and corrosion-induced defects on microchip  Al bondpads will cause non-stick on pads (NSOP) issues.  In  this paper, the authors will further study NSOP problem and  introduce one more NSOP failure mechanism due to Cu  diffusion caused by poor Ta barrier metal. Based on our  failure analysis results, the NSOP issue was not due to the  assembly process, but due to the wafer fabrication. The failure  mechanism might be that the barrier metal Ta was with  pinholes, which caused Cu diffused out to the top Al layer, and then formed the “Bump-like” Cu defects and resulted in  NSOP on Al bondpads during assembly process.


In wafer fabrication and microchip assembly process, it is  well-known that underetch material, contamination, particle, pinholes and corrosion-induced defects on microchip Al  bondpads will cause non-stick on pads (NSOP) issues at  assembly process. In the authors’ previous studies, some  NSOP cases due to TiN underetch [1], galvanic corrosion [2-3] and fluorine-induced corrosion [4-6] have been studied. In  this paper, we will further study NSOP problem and introduce  one more NSOP failure mechanism due to Cu diffusion  caused by poor Ta barrier metal.


Experimental, Results & Discussion


In this case, based on customer’s feedback, the NSOP issue  was found during their assembly process and some failure  samples were sent to us for failure analysis. The main purpose  is to understand the failure mechanism and possible root  cause and identify whether the NSOP problem was due to  assembly process or wafer fabrication so as to make  improvement at manufactory/assembly line.


Optical and SEM inspections were carried on the failed die  and found NSOP pad which are shown in Figure 1 and 2. In  order to identify the possible root cause, Auger analysis was  conducted on 3 pads (non-bonded pad, NSOP pad and bonded  pad, which are shown in Figure 2) to check if there is any  contamination. However, Auger surface and depth analysis by  sputtering   results  showed   that  no  abnormal  element was


Figure 1.  Optical inspection found NSOP pad on the affected  dies.


Figure 2. SEM inspections found NSOP pad on the affected  dies (From left: non-bonded pad, NSOP pad and bonded  pad).


detected. Based on Auger results, we ruled out the possibility  that the NSOP was due to contamination (such as C and F  etc.) and underetch material (such as TiN & Si, etc.).


For root cause identification, we further did SEM/EDX  analysis and found presence of Cu material on Al bondpads. In wafer fabrication, we know that for microchip bondpad  metallization, Al alloy (0.5% Cu) is currently used. However, based on our experience and common knowledge, this level of  Cu (only 0.5%) is unable to be detected by EDX analysis  technique due to its high detection limit. Therefore we  suspected that the Cu material might be from underneath Cu  diffusion. Then we did further FA using chemical  deprocessing and TEM analysis techniques.


HCl acid was used for deprocessing on the die sample to  remove Al metal on bondpads:


HCl  + Al  AlCl3


HCl  + Cu  No reaction


Optical and SEM inspection on non-bonded pads found some “Bump-like” defects at the bondpad edge (Figure 3). EDX  analysis detected high Cu peak on the “Bump-like” defect (Figure 4).  In the EDX spectrum (Figure 4), Cl detected was  from deprocessing chemicals HCl and Au detected was from  sample preparation by gold sputtering.


Figure 3. After HCl chemical deprocessing to remove Al  metal, SEM inspection found some “Bump-like” defects at  the pad edges.


Figure 4 EDX analysis detected high Cu peak on the “Bumplike” defect (in the spectrum, Cl was from deprocessing  chemicals HCl and Au was from sample preparation by gold  sputtering).


Based on such high amount of Cu material showed in Figure  3, we highly suspected that Cu material was more likely from   underneath Cu diffusion. To identify the root cause and  failure mechanism, cross sectional TEM was performed at the  pad edge. TEM results confirmed that Cu was diffused into  the Al layer on the bondpad and Al was also diffused into the  Cu layer (Figure 5).


Moreover, based on TEM result, we found the barrier metal  Ta layer with the weak point (pinhole) at the area circled in  Figure 6. Close-up TEM result are showed in Figure 7. From  the TEM result, one can see that the Ta barrier metal was  with a pinhole, which had caused Cu to diffuse into the Al  layer on the bondpad and Al to diffuse into the Cu layer.


Figure 5. TEM micrograph showed that Cu was diffused to  the Al layer on the bondpad and Al was also diffused to the  Cu layer.


Fig. 6 TEM micrograph showed that the barrier metal Ta  with weak point at the area circled.


Figure 7. Close-up TEM micrograph showed the barrier  metal was with a pinhole, which might have caused Cu  diffusion to the Al layer and Al was also diffused to the Cu  layer.


In this paper, we further study NSOP problem, introduced one  more bondpad failure model of NSOP, studied failure  mechanism and identified the possible root cause. Based on  the failure analysis results, the NSOP issue was not due to the


assembly process, but due to the wafer fabrication. The failure  mechanism might be that the barrier metal Ta was with  pinholes, which caused Cu diffused out to the top Al layer, and then formed the “Bump-like” Cu defects and resulted in  NSOP on Al bondpads during assembly process.


The authors would like to thank Mr Richard Xing and Miss  Sun Fangda for their technical support and contributions to  this technical paper.


[1] Hua Younan, Failure Analysis of Discolored Bondpads in  Wafer Fabrication. ISTFA 1999, 14-18 Nov, Santa Clara  Convention Center, Santa Clara, California, USA,149-159  (1999).


[2] Hua Younan, A Study on Discolored Bondpads & Galvanic Corrosion. ISTFA 1998, 15-19 Nov, Hyatt  Regency, DFW-East Tower, Dallas, Texas, USA, 269-272 (1998).


[3] Hua Younan et al, Failure Analysis and Elimination of  Galvanic Corrosion on Bondpads during Wafer Sawing. ISTFA 2000, 12-16 Nov, Meydenbauer Convention  Center, Bellevue (Seattle), Washington, USA, 369-372 (2000).


[4] Hua Younan et al, A Study on Non-Stick Aluminum  Bondpads due to Fluorine Contamination using SEM, EDX, TEM, IC, Auger, XPS & TOF-SIMS Techniques. ISTFA 2002, 3-7 Nov, Phoenix Civic Plaza, Phoenix, Arizona, USA p495-504 (2002).


[5] Hua Younan et al, A Study on Fluorine-Induced  Corrosion on Microchip Aluminium Bondpads. ISTFA  2003, 2-6 Nov. 2003, Santa Clara, California, USA, p249-255 (2003).


[6] Hua Younan, Xing Zhen Xiang and Li Xiaomin, Characterization Studies of Fluorine-induced Corrosion  Crystal Defects on Microchip Al Bondpads using X-ray  Photoelectron Spectroscopy. The Proceedings of the 21st  International Physics and Failure Analysis (IPFA’2014), 30 June – 4 July 2014, Singapore, p17 – 088 (2014).


Failure Localization of Intermittent Short Failures Caused


by Vertical Conductive Anodic Filament Formation


Daniel Nuez and Phoumra Tan


Xilinx 2100 Logic Drive San Jose, CA 95124


Phone: (408) 879-6572; Emails: dnuez@xilinx.com ; phoumra@xilinx.com


Abstract – Conductive anodic filament (CAF) formation is a mechanism caused by an electrochemical migration of metals  from a metal trace in ICs or in PCBs.  This is commonly caused by the moisture build-up in the affected metal terminals in an  IC package or PC board caused by critical temperature, high humidity and high voltage gradients conditions.  This  phenomenon is known to have caused catastrophic field failures on various OEMs electronic components in the past [1,7].   Most published articles on CAF described the formation of the filament in a lateral formation through the glass fiber  interfaces between two adjacent metal planes [1-6, 8-12].  One common example is the CAF formation seen between PTH (Plated through Hole) in the laminated substrate with two different potentials causing shorts [1-6, 8-12].   In this paper, the  Cu filament grows in a vertical fashion (z-axis formation) creating a vertical plane shorts between the upper and lower metal  terminals in a laminated IC package substrate.  The copper growth migration does not follow the fiber strands laterally or  vertically through them.  Instead, it grows through the stress created gaps between the impregnated carbon epoxy fillers from  the upper metal trace to the lower metal trace with two different potentials, between the glass fibers.  This vertical CAF  mechanism creates a low resistive short that was sometimes found to be intermittent in nature.  This paper presents some  successful failure analysis approaches used to isolate and detect the failure locations for this type of failing devices.  This  paper also exposes the unique physical appearance of the vertical CAF formation.


I. Introduction:


There had been a growing level of concerns on conductive


anodic filament type of failures in both the semiconductor


industry and the printed circuit board manufacturers.  The


advent of smaller and thinner hand held devices such as cell


phones, tablets and other PDAs, made the issue even a


greater concern for the IC manufacturers and their vendors


who are directly affected by the demands for high


performance and high density ICs in a smaller, thinner and


light weight packages [4, 7,12].   In this article the main


concern is the laminated package substrate which consisted


of closely spaced metal traces between thin inter-woven


glass fiber interfaces and carbon epoxy fillers with solder


mask laminate (FR-4) at the exterior layer.  We first


observed the vertical CAF formation at our facility during


the earlier assessments of various package types with a


variety of package piece parts combination from different


vendors.  One combination set had shown significant


failures during HAST stress.  The failing samples are from


wire bonded package BGA, 17mm X 17mm. The reliability


stress introduced on the samples is HAST (110°C/85%RH)


with an extended duration beyond the JEDEC required


hours.  The failure modes observed from the ATE tester are:  Resistive shorts (~1 to ~200 ohms) and IIL leakage failures  in which both are intermittent in nature and can easily  recover from handling and testing. The intermittent short  can sometimes recover with a slight mechanical pressure  applied to the package and after repeated attempts of  electrical testing on the same failing pins.  The short was  also found to be bake- recoverable. Testing this type of  failure at a slightly higher than normal voltage / current  settings can also make some of them recover.   During the  initial analysis of the earlier failing units using conventional  FA approach, some of the failing devices would recover or  showed no evidence of failure on their suspected failing  locations.  Realizing these challenges helped us formulate  some techniques in isolating and analysing these sensitive  and subtle intermittent short failures.   The vertical CAFs  observed in this article is copper–containing corrosion byproducts that had emanated from the positively charge  anode terminal metal traces toward the grounded metal pad  terminals- cathode.


II. Failure Isolation & Detection Methods:


a) Curve tracer test:  During I-V curve tracer testing for  confirmation of failures on the failing pins, it is highly  recommended to use low voltage /current range settings on  the curve tracer (100mV/div. and 10uA/div.).  Some failure  devices tend to recover between 300uA – 1mA at ~ 100mV


- ~200mV.   In most cases, once the device fully recovered, they can no longer fail again unless they are subjected to  additional HAST stress.  This was realized after a few units  had recovered during the initial analysis of this type of  failures.  There were also some cases in which the failing  pins of the devices would fully recover a few hours after  curve tracer testing.  Therefore it is highly recommended to  immediately move on to the next sequence of failure  analysis technique while the short is still present in the  device.  The curve tracer images below show the duration  when the short failure was first observed in the curve tracer  until fully recovering after 4 hours.  This was one of the  challenges in doing failure analysis of these units.


b) Time Domain Reflectometry:  TDR analysis was then  utilized to determine whether the failure mechanism lies in  the package substrate or in the die.  It also helps determine  how far the short is from the solder ball.  The TDR results  on two failing devices revealed that the location of their  shorts are within the package substrate near the area of the  solder ball (lower metal layer).  Using this information, an  analyst can then make a better decision for performing the  appropriate PFA (Physical Failure Analysis).  One  disadvantage with using this equipment is that the device  had to be held down firmly in the TDR socket in order to  obtain a good waveform signal of the failing pin through  the device.  The pressure applied on top of the package  causes slight mechanical flexing that can sometimes be  enough to make the device recover.  So it is important to  handle the device carefully in the TDR socket by applying a  slight pressure just enough to get a good signal on the  failing pin in order to preserve the short failure of the  device.


Fig. 4:  TDR analysis revealed the short lies in the package substrate near the solder ball (red arrow). 


Figure 1:   < 1 Hr. after ATE test         (IO pin   vs. VCCO = 1Ω short) 


Figure 2:  2 Hrs. after test                     (IO pin vs. VCCO = 9KΩ short) 


 Figure 3:  4 Hrs. after test                             (IO pin vs. VCCO ~2MΩ) ‐ Device had fully recovered.  


c) Thermal Emission Microscopy:   A thermal emission  microscope with an InSb IR camera was used to isolate the  location of the resistive short failure on some of the  devices.  Using this hot spot detection approach, several  devices had recovered during the initial analysis of these  units.  By using the reference TDR data (failure near the  solder ball), one device was probed from the solder ball  side of the package between the shorted I/O pin and supply.  A hot spot was successfully detected emanating from one  side of the failing I/O solder ball at the opposite area of the  probe point. This hot spot was accomplished by applying  very low voltage / current ratings (50mV - 100mV / 50uA100uA) to the device. The disadvantage of using this  equipment is similar to the curve tracer.  This sensitive  short failure would easily recover if higher voltage / current  were applied.


III. Physical Failure Analysis


a)  Mechanical Package Cross-section: After reviewing the  package CAD layout, it was determined that lateral short  would not be possible at this hot spot location.  The short  was most likely happened between the two overlaying  metal planes.   The device was mechanically crosssectioned to examine the hot spot area in the package  substrate.   We labelled this unit #1. The cross-section  revealed a vertical CAF formation directly underneath the  hot spot area causing a direct short between the Vcco - upper metal trace to the grounded I/O pin – lower metal  trace.   The images of the cross-section are shown through a  dark field lens (Fig. 7 – Fig. 8).  It was found that using  dark field lens and drop of water on the sample helped  make this vertical CAF formation more visible in the  optical microscope.  The subsequent SEM images of the  same cross-sectioned area of unit #1 showed some of the  exposed portion of the CAF filament (Fig. 9 – Fig. 10).


Fig. 5:  Micro‐probing and thermal emission detected the hot spot area near the solder ball. Mag. = 0.5X  


Fig. 6:  A higher magnification view of the hot spot area emanating from the bottom side of the failing solder ball pin.   Mag. = 5X 


Fig. 7:  Unit #1 cross‐section view of the package substrate show the vertical CAF formation between layer 3 (VCCO) and layer 4 (Failing IO) metal traces using a dark field lens.   Mag. 100X 


Vcco


Grounded (I/O) Pin 


CAF


b) EDS Elemental Analysis:  Energy dispersive x-ray  analysis detected the presence of Cu elements in the  impregnated epoxy fillers at the CAF migration path  between the metal 3 and metal 4 layers (Fig. 11).  The EDS  validated the Cu conductive anodic filament formation in  the impregnated epoxy filler area.


Fig. 11:  EDS elemental analysis  result confirmed that the exposed filament is Cu.   


Fig. 8:  Unit #1 High magnification view of the vertical CAF formation.   Mag. 500X 


Fig. 9:  Unit #1 ‐ SEM image of the CAF formation in the epoxy filler area.  Due to the nature of the CAF formation embedded in the epoxy filler, the SEM can only reveal the exposed portion of the CAF.          Mag. 1500X 


Fig. 10:  Unit #1 ‐ High magnification SEM image of the exposed Cu filaments in the epoxy filler area.     Mag. 4500X 


CAF formation


To confirm that the failure mechanism is the same for all  the failures, a second cross-sectioned sample was prepared:  Unit #2 also failed for low resistive short failing between an  IO pin and supply.  The CAF migration path was observed  from the VCCO (3.3V) trace to the failing grounded I/O  pads connected to the solder balls.  These failing pins  resided directly underneath and VCCO trace.   The result of  the second cross-sectioned sample was identical to the first  one where a clear evidence of vertical CAF formation was  observed through the dark field lens.  Light deflection  technique through water and dark field lens helped reveal  embedded Cu growth in the impregnated epoxy filler area.  For this particular sample #2, the failing pin had already  recovered.  Despite its recovery, the failure mechanism  remained evident in the area as shown through the dark  field lens in Fig. 12 and 13.


c)  Parallel Polish (Unit #3):  A third unit was prepared by  grinding off the solder balls and polishing off the solder  mask and the lower metal 4 layer to expose the impregnated  g. epoxy filler material and interwoven glass fiber.  The  circled area is where the hot spot (for unit #3, not shown in  this article) was detected between the interwoven glass  fibers.


Fig. 12:  Unit #2 cross‐section view of the package substrate show a vertical CAF formation between layer 3 (VCCO) and layer 4 (Failing IO) grounded metal trace and solder ball.   Mag. 100X 


Fig. 13:  Unit #2 higher magnification cross‐section 


view of the vertical CAF formation.  Mag. 500X 


Fig. 14:  Unit #3 ‐ Lower magnification SEM image of the fail site (circled) after the removal of the solder mask and M4 layer.    This image exposes the inter‐woven glass fibers between the impregnated epoxy fillers.   


Planar view:  Low mag. SEM Image of location of CAF


CAF formation  Vcco plane 


Grounded (I/O) Pin


d) EDS X-Ray Mapping:   To further validate the findings


in unit #3, EDS elemental mapping of the CAF formation


on the impregnated epoxy filler was performed.  The EDS


map confirmed the exposed shiny material in the epoxy


filler area is composed of Cu elements (blue).  Please note  that the Al particle (yellow) is remnant from the alumina


powder that was used during sample preparation (polishing).


Fig. 16:  Unit #3 – The optical photo shows the anomaly observed at metal 3 layer of the hot spot location.  The anomaly became evident after the removal of the M4 layer.  The optical image is shown using dark field lens.  


Fig. 17:  Unit #3 – A higher magnification optical photo of the CAF formation (circled) after the removal of the solder mask and M4 layer (bottom side of package).   The image is shown using dark field lens. 


Fig. 15:  Unit #3 ‐ Higher magnification SEM image of the fail site (circled) after lapping the solder mask and M4 layer (bottom side of package).  The shiny particles (circled area) are the tips of the Cu CAF formation.   


Fig. 18:  Unit #3 – The EDS x‐ray mapping revealed the tip of the Cu CAF formation in the epoxy filler highlighted in blue.    


Planar view:  Optical Dark Field Image of CAF location Planar view: High mag. SEM Image of CAF formation


e) FIB Cross-section:   Precision FIB cross-section was  performed in the affected area to view the underlying CAF  formation on unit #3.  The FIB cross-section revealed the  cracking in the epoxy filler area where the path of the Cu  migration occurred. This epoxy filler material breaks down  between the inter-woven glass fibers. As expected, the EDS  analysis of the underlying particles in the epoxy filler  between the cracks is composed of Cu elements (Fig. 19).


f) 2D and 3D X-ray Tomography Imaging:   Another FA  approach to show the Cu CAF formation in the substrate is  with the use of the 2D and 3D CT x-ray tomography.   The  2D and 3D x-ray images revealed the CAF formation in the  impregnated epoxy filler from the M3 Cu metal trace in the  substrate.   Please see the images below.


FIB cut ‐ Partially exposed CAF  


Fig. 20:  Unit #4 – 2D x‐ray revealed the Cu loss in the Cu metal trace of VCCO (red arrow) where the vertical CAF short  


formation occurred. 


Fig. 21:  Unit #4 – A virtual cross‐section x‐ray tomography image showing the Cu loss (yellow arrow) and the vertical CAF filament formation in the epoxy filler area (red arrow).   


Cracks in the epoxy filler 


Top view 2D x‐ray image of the Cu loss at Vcco metal trace


CAF formation 


Cu loss at Vcco metal trace Virtual Cross‐section x‐ray tomography  


Fig. 19:  Unit #3 – The FIB cross‐section and EDS analysis of the exposed filament validated that the filament formation is Cu.   


IV. CAF Formation Mechanism:


Earlier research by Bell Laboratories provided the two step  model that causes the mechanism for typical CAF  formation and growth [5].   The first is the breakdown or  degradation of the epoxy/glass fiber interface when the  absorption of moisture occurs between the two materials.   An aqueous medium is then created between the


epoxy/glass fiber interfaces which provide an electrolytic  pathway for corrosion by-products. The next step is the  creation of the electrochemical corrosion reactions that  cause a loss of insulation resistance.   With continued  moisture build up between the conductors, any electrical  bias to the affected conductors can then produce an  electrochemical process in which copper ions dissolve from  the anode and migrate to cathode through epoxy resin/glass  fiber interface [3, 6, 8].   However, in this particular case, the electrolytic migration path is a vertical pathway through  the cracks of the moisture weakened impregnated carbon  epoxy filler material in the substrate which is the spacing  between the interwoven glass fibers as shown in Fig. 14  and Fig. 15.  The insulation resistance drops as the carbon  epoxy filler barrier breaks down then the vertical CAF  phenomenon will start to occur.


Electrochemical Equation for Cu CAF Formation:


V. Conclusion:


As the demand for high performance smaller feature size  packages increases in the IC industry, the chance of having  catastrophic failures also increases as the package design  becomes more complex combined with a variety of choices  of materials and piece parts that may be susceptible to CAF  formation type of failure [1,4,7,12].  The type of vertical  CAF formation presented in this paper follows the typical  electrochemical CAF growth model but with a different  pattern formation and location of the growth path.  This  vertical CAF formation was made possible due to moisture  weakened impregnated epoxy fillers from the excessive  reliability stress introduced to the devices, which is above  the JEDEC standards.   This paper introduced a vertical  CAF formation mechanism that is different from the typical  lateral CAF formation seen between PTH.  The mechanism  can be easily overlooked or missed during PFA due to its  physical characteristics, intermittent nature and  recoverability of the short failure. The successful FA  methods described in this paper can be a useful reference  whenever a similar type of failure mechanism is  encountered.


Fig. 22:  Unit #4 – The 3D CT volumetric x‐ray tomography 


showed a tilted view of the CAF formation in the substrate at the metal 3 layer (circled).  In this image the solder balls and bottom M4 layer had been removed to help expose the vertical CAF formation clearly. 


Fig. 23:  Unit #4 – The 3D CT volumetric x‐ray tomography 


showed a higher magnification view of the vertical CAF 


formation.  


VI. References:


[1] Yung, K.C., HKPCA Journal Issue 21, Conductive


Anodic Filament : Mechanism and Affecting Factors.


[2] Turbini, J. L., Ready, W., Smith, B., Georgia Institute of


Technology, Conductive Anodic Filament Formation:


A Potentially Reliability Problem for Fine Line Circuits


[3] Brewin A., Zou L., Hunt C. “Susceptibility of Glass


Epoxy Laminates to Conductive Anodic Filamentation”


[4] Karavakis K., Bertling S. “Conductive Anodic Filament:


The  Threat to Miniaturization of the Electronics  Industry”,  Meptec Report, Quarter Four, 2004


[5] Lando D.J., Mitchell J.P., Welsher T.L. “Conductive


Anodic Filaments in Reinforced Polymeric Dielectrics:


Formation and Prevention”, International Reliability


Physics Symposium, 1979


[6] Rudra B., Jennings D., “Failure-Mechanism Models for


Conductive-Filament Formation”.  IEEE Transactions  on  Reliability, Tutorial Vol. 43, No. 3 September 1994


[7] Amkor Technology Reports Financial Results for the


Fourth Quarter and Full Year 2011,” Q4 and 2011  Amkor Technology, Inc. Earnings Conference Call, February 9, 2012


[8] Kohman G.T, Hermance H.W., Downes G.H.,


“Silver Migration in Electrical Insulation” n2e Bell


Systems Technical J., November 1995


[9] Ready W.J., Stock S.R., Freeman G.B., Dollar L.L. and


Turbini L.J., “Microstructure of Conductive Anodic


Filaments Formed during Accelerated Testing of


Printed Wiring Boards”, Circuit World, July, 1995


[10] Ready W.J. and Turbini L.J., “The effect of Flux


Chemistry, Applied Voltage, Conductor Spacing, and


Temperature on Conductive Anodic Filament  Formation”, Journal of Electronic Materials, Vol. 31, No. 11, 2002


[11] Amla Tarun, “Conductive Anodic Filament Growth


Failure”, IPC Expo, 2002


[12] Cohn C., Kimbara H.  “Via to Via Isolation vs. Quality  of Via Formation in Organic Substrates”, 9th Electronics


Packaging Technology Conference, 2007


VII. Acknowledgements:


The authors would like to thank Dean Tsaggaris the REL  engineer at Xilinx who helped with the REL testing of the  samples used.  We also would also like to thank S.Y. Pai, our director, for his continued support to broaden the  technical capabilities in the FA Lab at Xilinx.  Finally, we  would like to thank Jack Kasahara, Naomi Kotwal and  Allen Gu of Carl Zeiss/Xradia for their support with the xray inspection and for providing the 3D X-ray tomography  images of the anomaly using the Xradia 510 Versa.


Understanding the Cu Void Formation by TEM Failure Analysis


### Understanding the Cu Void Formation by TEM Failure Analysis


Binghai Liu, Jie Zhu, Changqing Chen, Eddie Er, Siping Zhao, Jeffrey Lam, Sebastian Elizabeth, Chen Ye


Failure Analysis,  Product, test and failure analysis Dept. (PTF Singapore) GLOBALFOUNDRIES Singapore Pte Ltd 60 Woodlands  Industrial Park D, Street 2, Singapore 738406


* Correspondent: Binghai.liu@globalfoundries.com


In this work, we present TEM failure analysis of two typical  failure cases related to metal voiding in Cu BEOL processes. To understand the root cause behind the Cu void formation, we performed detailed TEM failure analysis for the phase  and microstructure characterization by various TEM  techniques such as EDX, EELS mapping and electron  diffraction analysis. In the failure case study I, the Cu void  formation was found to be due to the oxidation of the Cu  seed layer which led to the incomplete Cu plating and thus  voiding at the via bottom. While in failure case study II, the  voiding at Cu metal surface was related to Cu CMP process  drift and surface oxidation of Cu metal at alkaline condition  during the final CMP process.


Introducing Cu as the metal interconnects meets the  demands for fast signal transport in modern semiconductor  devices. However, the integration of Cu into manufacturing  processes is always challenging due to the complexity of Cu  BEOL processes. Among these challenges, inline defect  generation, and processing integrity of dual-damascene  processes, and associated microstructure/properties of Cu  materials are critical concerns for high-quality metal  interconnect and high yield/reliability performance. Cu voids  of various size and morphologies are most commonly  observed defects in Cu BEOL processes. The presence of  these Cu voids may either result in direct device failure such  as open or high-resistance, or exist as imperfection which  may have potential reliability concerns and/or finally induces  reliability failure. Recent researches have shown that void  defects of Cu thin films are mainly yield killers and seriously  degrade interconnect reliability.[1]


The formation of Cu voids can occur at various process steps, such as dual-damascene processes, reliability test and wafer  sort/testing, etc. Cu voids could be due to imperfect ECP


filling, or organic additives introduced during ECP [2], or  stress migration during heat treatment after ECP [3], or  hydrogen embrittlement effects [4], or electromigration  during reliability test.[5] , or thermal stress concentration [6]. Under either case, the Cu void as formed can be associated  with some characteristic physical signatures which can be  linked to certain process steps. Therefore, the  characterization of these physical signatures is the key for  understanding the root-cause of the Cu void formation, and  thus associated processes drift.


In this work, we will report two typical case studies on Cu  void formation in semiconductor manufacturing processes of  advanced technology nodes. We demonstrated the  importance of TEM failure analysis techniques in  understanding the root-cause of the Cu void formation with  detailed phase, composition and microstructure analysis.


For the TEM FA for both case studies, to facilitate possible  carbon related contamination issue analysis, we used in-situ  lift out FIB sample preparation technique in order to avoid  carbon signal from the carbon film on Cu grids. The TEM  sample preparation was performed by using FEI Helios 400S  Nanolab FIB. TEM imaging was done by using FEI Titan  TEM (80~300kV) at 300kV with STEM EDX for elemental  analysis. EELS mapping was performed by using Gatan GIF  Tridem system at 300kV.


Case I: Cu void formation due to Cu seed oxidation


The case as reported was related to wafer edge scan failure  with 2~4% wfr level hit rate. Prior to the physical failure  analysis, detailed electrical fault isolation by EMMI was  performed and an exclusive spot was observed.  FIB  slice/view was performed before TEM sample preparation  according to emission spot location.


Figure 1 (a)-(b) Bright-field TEM images and (c) STEM Z-contrast  image shows the void at Via1 bottom


As shown in Fig.1(a) and (b), TEM failure analysis revealed  a typical void at via1 bottom.  STEM z-contrast image in  Fig.1(c) indicated that the Ta/TaN liner remained good  conformity and coverage at the bottom of the defective via.


Figure 2 STEM-EDX line scan analysis revealed the presence of Cu, Ta, O and N in the via 1 void


To understand the materials inside the void, STEM-EDX line  scan was performed across the defective via1 bottom, and the  results are shown in Fig.2.


As indicated by Fig.2, Ta, Cu, O, N were detected in the  voiding region. No carbon was detected across the voiding  area, indicating that the Cu void formation was not due to  polymer/carbon contamination issue related to etch and postetch cleaning processes. The presence of Ta and N is easily  understood since the Ta/TaN linear remain good conformity  and coverage at the defective via1 bottom. However, Cu  signal from the voiding area needs careful interpretation if  considering the small CD of via1 bottom, which is less than  100nm. Therefore, Cu signal may arise from M1 in front  of/behind the via1. On the other hand, Cu signal from Cu  grids may also be possible, which makes the interpretation of  Cu presence more difficult. As far as O-rich materials present  in void is concerned, there also might be several possible  sources: (i) oxide residue at the via bottom introduced before  ECP process; (ii) oxidation of Ta linear due to line issue; (iii) Cu seed oxidation before ECP process; (iv) oxide redeposition during FIB sample preparation. Therefore, the  presence of O in via1 void could be correlated with either of  them. Therefore, further detailed TEM analysis is needed in  order to understand the root cause of the void formation.


Figure 3 EFTEM-EELS mapping: (a) C-map; (b) Cu-map; (c) Omap; and (d) Ta map


Fig.3 (a)~(d) showed the results of  EFTEM-EELS mapping. Carbon map in Fig.3 (a) confirmed that there was no carbon  contamination at the via1 bottom. The Cu map in Fig.3 (b) indicated that there might be Cu partial filling in the voiding  area. If the Cu signal was purely from either front-side or  back-side of M1, the Cu counts as detected should show the  uniform contrast in the EELS map. The discontinuity in Cu  contrast in voiding area may suggest that Cu was partially


filled in the via1 bottom. The presence of Ta and O in the via  void were further confirmed by the EELS mapping as shown  in Fig3. (c) and (d), which is consistent with the results of the  EDX line scan analysis shown in Fig. 2.


To further understand the presence of O in the via1 void, we  performed nanobeam electron diffraction (NBD) to study the  phases presented in the voiding area. The diffraction patterns  from 2 points inside the void were selected for detailed index  analysis, as shown in Fig.4 (a). The NBD patterns in Fig.4 (b) and (c) showed typical polycrystalline nature. The NBD in  Fig.4 (b) was taken from Ta-linear. Detailed indexing of the  patterns indicated the presence of both metallic Ta and TaO2  phases, and TaO2 has BCC structure with -11-5 zone axis. The results indicated that Ta linear was oxidized, which is  consistent with EDX line scan analysis shown in Fig.2 (d). The rotational intensity average technique was employed for  the phase identification in Fig.4 (c).  As seen from Fig.4 (c), TaO2 and Cu2O phases were identified, indicating the  oxidation of both Ta linear and Cu/ Cu seeds in the void.


Figure 4  Nano-beam electron diffraction (NBD) on Cu void region, revealed the presence of Cu2O and TaO2 and Ta phases.


The above results indicated that, before ECP process, it is  highly possible that both Ta linear and Cu seed layer were  oxidized. With Cu seeds oxidation, it is easily understood  that partial Cu filling at the defective via1 bottom which in  turn directly resulted in partial filling Cu and thus the voiding  at the via bottom. The results also well agreed with the fab  inline investigation. Lot history and tool commonality  analysis showed the affected lots/wfrs the abnormally long  timeline between Cu seed PVD process and the subsequent  ECP processes, which may account for the oxidation of Cu  seed layer and thus underneath Ta layer.


Case II: Cu void formation during Cu CMP process


The case reported was related to an inline defect issue. YDD  after Cu CMP caught high-density of Cu micro-void defects  on Cu metal surface.Fig.5 showed typical surface SEM  images of the Cu voids formed on the Cu metal surface with  difference sizes. Close view indicated that these voids  normally had sharp edges/corners, instead of round shape.


Figure 5 SEM images showing the voids of different sizes on Cu  metal surface


Figure 6 (a) Bright-field TEM and (b) STEM-Z contrast images of  Cu micro-void formed after Cu CMP process


The wafer submitted for TEM FA was covered with NBLK  layer to facilitate TEM failure analysis in order to keep native  structures associated with the voiding defects.   Fig.5 (a) and


(b) show respectively the bright-field and STEM images of  the void on Cu surface. As seen from them, the void had  sharp corners, just like the left-over with a grain peeling off  from the metal.


Further STEM-EDX line scan analysis was performed across  the Cu void in order to understand any residue materials  inside the void. As shown in Fig.7, EDX analysis showed the  presence of Al, Si and O inside the void. The source of Al  and Si may be Cu CMP slurry. As it is well known, Cu CMP


is a multiple process with Al2O3 as the slurry for the primary  CMP process, while silica as the slurry for final CMP process. The presence of Al and Si inside the Cu void may suggest  that the void was formed during CMP processes, but not  related to other effects like stress voiding. With void  formation during the CMP processes, the slurry particles  were trapped inside the void. This also well explained the  presence of O inside the void.


Figure 7 STEM-EDX line scan analysis, showing the presence of


Al-oxide and Si-oxide inside the Cu void


Figure 8  Nanobeam diffraction showed the presence of Cu2O phase  at the edge of the void, indicating oxidation of Cu metal


As shown in Fig.7 (a) and Fig.8 (a), relatively dark contrast  was observed at the boundary in between the void and the  remaining Cu metal. The contrast could arise from thickness  and/or diffraction effects, and maybe also  Z contrast, e.g. the  oxidation of Cu metal at the void boundary.   Therefore, we  performed further electron diffraction analysis, as shown in  Fig.8. The NBD from a point in the suspected edge region (Point-2 in Fig.8 (b)) showed the presence of Cu2O, indicating there was really Cu oxidation associated with the  Cu void formation.


The Cu oxidation could occur either during CMP processes  or after the void formation with trapping of oxide slurry in  the void. Although both possibilities exist, the former one  might be an important signature that deserves further  investigation of any abnormal process shift during CMP  processes. Through detailed inline investigation, it was found  the affected slots/wafers ever went through CMP rework due  to process drift with using the new CMP slurry. The Cu void  formation was related to the surface oxidation of Cu metal at  relatively higher alkaline condition with the new slurry in the  final Cu CMP stage.  As it is well know, in pH>7 alkaline  condition, Cu can be oxidized to CuO or Cu2O during CMP  process. Furthermore, in case of any large CMP process drift  which leads to  abnormally large Cu protrusion with  respected to IMD in between metal lines, Cu oxidation in the  final CMP stage together with large shear stress by CMP, the  Cu oxide as formed could be easily peeled off, leaving voids  in the Cu surface. Normally the oxidation is preferred along  Cu grain boundaries due to the presence of defects and large  surface energy, and therefore, the peeling occurs along the  Cu grain boundaries, resulting in the sharp and smooth  boundaries of voids, as what we observed in Fig. 5 ~ Fig.8.


In this work, we presented two typical case studies related to  Cu void formation by TEM failure analysis. With detailed  phase and microstructure analysis, we identified key physical  failure signatures, and correlated them to the fab inline  investigations for root cause understanding. The void  formation in the first case was due to (i) the oxidation of Cu  seed layer due to abnormal time between Cu seed PVD and  Cu ECP processes. Void formation in the second case was  caused by using new CMP slurry during rework due to Cu  surface oxidation process drift with Cu surface oxidation.


[1]  H.P. Feng, M.Y. Cheng, Y.L. Wang, S.C. Chang, Y.Y. Wang, C.C. Wan, Thin Solid Films, 498 (2006) 56 – 59


[2]  Shinya Konishi, Miki Moriyama and Masanori


Murakami, Materials Transactions, 43 (2002) 1624-1628


[ 3]  J. A. Nucci, R. R. Keller, D. P. Field, Y. ShachamDiamand, Appl. Phys. Lett. 70 (1997) 1242-1244


[4] M. Koiwa, A. Yamanaka, M. Arita and H. Numakura, Mater. Trans JIM 30(1989) 991-998


[5] Nam-Hoon Kim, Sang-Yong Kim, Woo-Sun Lee, EuiGoo Chang,  Microelectronic Engineering, 84 (2007) 2663–2668


[6] A. Sekiguchi,  J. Koike, S. Kamiya and M. Saka, K.


Maruyama,  Appl. Phys. Lett., 79 (2001) 1264-1266


Failure Analysis Methodology on Systematic Missing Cu in RAM due to Cu CMP


Ang Ghim Boon, Chen Changqing, Ng Hui Peng, Alfred Quah, Teo Angela,  Yip Kim Hong, Neo Soh Ping, Lam Jeffrey, Mai Zhihong


Product, Test and Failure Analysis group,  GLOBALFOUNDRIES Singapore Pte Ltd  Email: GhimBoon.Ang@globalfoundries.com


This paper places a strong emphasis on the importance of  applying Systematic Problem Solving approach and use of  appropriate FA methods and tools to understand the “real” failure root cause. A case of wafer center cluster RAM fail due  to systematic missing Cu was studied. It was through a strong “inquisitive” mindset coupled with deep dive problem solving  that lead to uncover the actual root cause of large Cu voids. The missing Cu was due to large Cu void induced by galvanic  effects from the faster removal rate during Cu CMP and  subsequently resulted in missing Cu. This highlights that the  FA analyst’s mission is not simply to find defects but also play  a catalyst role in root cause/failure mechanism understanding  by providing supporting FA evidence (electrically/ physically) to Fab.


In wafer fabrication, quick root cause identification and  process fix are always critical to resolve low yield issues. The  role of FA analyst is no longer restricted to finding defects but  more importantly provide value-added information that can  help the Fab to establish root cause understanding and  mechanism. This is achieved through in-depth analysis of the  issue with close collaboration with Fab Yield Engineering (YE), Process Integration (PI) and Product Engineering (PE). The FA analyst can then self-propose any follow up FA that  can help to verify or revise the hypothesis even after the defect  is found.


FA engineers in the wafer foundry industry are required to  work on limited information and test support. “Inquisitive” mindset and problem solving skillset are particularly important  when working on systematic issues [1], [2],[3].


Result and Discussion


A low yield case that suffered from wafer center cluster RAM  fail was reported in wafer fabrication. Unfortunately, there is  NO bitmap capability available. Such scenario is often seen  particularly in wafer foundry due to the fact that there is often  minimal available data provided to the analyst.


1st level analysis: Successfully identified the defect


Bench testing based on different combination of power to  GND showed comparable IV. Nevertheless, Static EFA by  backside TIVA was performed and managed to shed some  lights with an exclusive TIVA signal. (Figure 1)


Figure 1: Static EFA by backside TIVA showed exclusive spot


The overlay of the TIVA spot with the GDS layout clearly  showed identical type of structure in the circuitry (Figure 2)


Figure 2: Identical type of structure seen from the TIVA spot


Subsequent top down PFA showed obvious Missing Cu (Figure 3). Alternatively, another approach was taken by  performing high beam SEM inspection to identify missing Cu  site with dielectric intact followed by XTEM. It further  revealed abnormal nitride layer at the missing Cu region (Figure 4). Random SEM inspection also revealed presence of  Cu voids that “seems” to be larger than the typical surface  voids (Figure 5).


Figure 3: Top down PFA showed obvious Missing Cu


Figure 4: XTEM revealed abnormal nitride layer at the  missing Cu region


Figure 5: Random SEM inspection also revealed presence of  Cu voids that “seems” to be larger than the typical surface  voids


2nd level Analysis: In-depth FA leading to root cause


understanding


Although the defect is found, the analysis is FAR from  Completion. Why??


 What is the cause of the missing Cu?


 Why the missing Cu is ALWAYS besides Via?


 Why such structure is more prone to missing Cu?


 How is the center patch correlated to the defect signature?  Is presence of “larger than typical” Cu void a “coincidence” or correlated to the missing Cu?


 Which process step is the culprit for creating such large  missing Cu?


With no further Fab suspect such as equipment commonality  provided, more in-depth FA finding with quick and effective  approach is critical for root cause understanding and  preventing more lots in the line from being impacted.


Initial Fab Hypothesis:


How FA data/evidence served as a supporting role to help  in confirming or overrule it


More Cu hillock resulted in thinning nitride NBLK and caused  problem if Cu hillock is directly at the Via site (resulted Via  punch-through and thinned NBlk). However, FA data  suggested this scenario to be of low possibility and over-ruled  it for the following reasons:


 The defective structure has only 2 Vias intact. Large  metal with more Via should hit more frequently based on  probability of occurrence


 Generally, Cu hillock should be observed at those large  Cu plates


Missing Cu


Value added FA contributed to root cause understanding  through systematic problem solving approach


Revisit the Symptom of Cu void


The larger than usual Cu voids as seen in Figure 5 may NOT  be a coincidental event. For validation, high beam SEM  inspection approach was engaged to search for more obvious  Cu void with dielectric intact. Subsequently XTEM along  metal showed signs of missing nitride at the Cu void site (Figure 6).


Figure 6: XTEM along metal showed signs of missing nitride  at Cu void site


Further XTEM was then performed across metal to another  inspection view. It confirmed the missing /damage nitride at  the Cu void site. The Cu void is also much larger than typical  surface Cu voids (Figure 7).


Figure 7: XTEM done across metal confirmed the missing


/damage nitride at the Cu void site. The Cu void is also much  larger than typical Cu voids


Revisit the Symptom of Systematic Missing Cu structure


The Camelot software from Synopsys was used in this  analysis phase due to its automatic layout tracing capability. This analysis is critical to understand how the circuitry  connected to this missing Cu metal line. It was observed that  all the missing Cu structure as well as those metal lines  with large Cu voids ALWAYS connected to N+/PW (Figure  8).


Figure 8: Camelot layout tracing showed all the missing Cu  structure as well as those metal lines with large Cu voids  ALWAYS connected to N+/PW


Consolidating all the key Symptoms Together  Induction  and hypothesis


The stage is much clearly now. Large Cu voids MUST be  present first. It resulted in missing/Damaged nitride at Cu void  site. If these voids falls underneath Via, it will result in Via


Center  Patch


Missing  Cu


Random  Large Cu


voids


Missing /Damage  Nitride at the Cu  void site


structure & metal  lines with large Cu  voids connected to  N+/PW


Presence of Via


besides the


punch-through and subsequent process steps (Via/Metal trench  etch/clean) will enhance the void to create a fully broken  metal (Missing Cu).  Since all the missing Cu structures and  metal lines with large Cu voids  are always connected to  N+/PW, it implies there is some form of galvanic effects  taking place during M1 CMP.


Further Fab Investigation and Failure Mechanism


100        80 60 40 20


0-20-40-60-80-100


Figure 9: Higher Center Removal rate correlated to the center  Fail patch


A close Fab investigation based on the FA confirmed that the  culprit was due to Cu CMP. There is a faster removal rate in  the wafer center. As seen in Figure 9, the higher center  removal rate correlated well to the center fail patch. Besides, the temperature was observed to be higher than usual. This  higher in temperature will reduce the efficiency of the  chemicals in the slurry that act as corrosion inhibitor. Thus, a  combination of faster center removal rate and higher  temperature will accelerate the galvanic effect to take place  during M1 CMP particularly on those metal lines with barrier  M1 removed and are connected to N+/PW that are of higher  build in potential. This also explained why the missing Cu  structures and metal lines with large Cu voids are always  connected to N+/PW. These Cu voids will result in nonuniform coverage of the CVD SiN. Subsequent steps (via etch, via scrub and metal trench etch/clean) enhance the void to  create a fully voided or broken metal line causing yield loss at  time zero (Figure 10).


Contour Plot for Cu Removal Rate


Cu Removal Rate<= 1.12e+4


<= 1.1375e+4<= 1.155e+4<= 1.1725e+4<= 1.19e+4


<= 1.2075e+4<= 1.225e+4<= 1.2425e+4<= 1.26e+4


> 1.26e+4


Figure 10: Large Cu voids are formed due to galvanic effects  and these Cu voids will result in non-uniform coverage of the  CVD SiN. Subsequent steps (via etch, via scrub and metal  trench etch/clean) enhance the void to create broken metal


A case of wafer center cluster RAM fail due to systematic  missing Cu was studied. After finding the missing Cu, further  in-depth study showed that actual root cause of large Cu voids  was induced by galvanic effects from the faster removal rate  during Cu CMP and subsequently resulted in missing Cu. This  paper placed a strong emphasis on the importance of applying  Systematic Problem Solving approach, deep dive and use of  appropriate FA approach/tools to understand the “real” root  cause. It stresses the importance of FA analyst not simply  finding defect but playing a catalyst role in root cause/failure  mechanism understanding by providing supporting FA  evidence (electrically / physically) to Fab.


Acknowledgement


The authors would like to thank the EFA/XTEM/Fab  counterparts for the FA data and failure mechanism  discussion.


[1] Ang Ghim Boon, Chen Changqing, Alfred Quah, Magdeliza, INDAHWAN Jony, Lee Mern Tat, David Zhu, After Via1 Scrub etch


After Trench Etch + Clean


After Cu CMP and SiN Dep


After Via1 etch


After M2 ECP


Neo Soh Ping “Failure Analysis Methodology on Systematic  defect in ADC_PLL Ring Pattern due to Plasma De-chuck  Process” ISTFA 2010


[2] Ang Ghim Boon, Chen Changqing, Zhao Si Ping, Ng Hui  Peng, Neo Soh Ping, Magdeliza G, Indahwan Jony, Lee Mern  Tat “Failure Analysis Methodology on Systematic defect in  N+ poly/NWELL Varactor in RF Analog_PLL due to  Implanter charging issue ” ISTFA 2012


[3] Ang Ghim Boon, Quah Alfred, Chen Changqing, Zhao Si  Ping, NAGALINGAM Dayanand, Li Yan, Neo Soh Ping, Shailesh Redkar “Device Characterization using AFP  Nanoprobing for the Localization of  New product Design  Weakness” ISTFA 2013


Identification of subtle defect by means of high KeV SEM passive  voltage contrast


Sujing Xie, Chaoying Chen, Nathan Wang, Andrew Komrowski, Qindi Wu, Saunil Shah


Maxim Integrated, 160 Rio Robles, San Jose, CA, USA


This paper presents two cases utilizing high KeV Passive  Voltage Contrast (PVC) for defect localization that is  impossible with other techniques. The first case is thin layer  resistor of CrSi. De-processing or polishing to expose the  defective layer may damage it. High KeV PVC combined with  FIB etch allows for a clear top view and x-section image. The  second case involves a beam sensitive via chain. In order to  avoid ion-beam-caused-damage, carbon paste was used to  ground the sample. A high KeV electron beam was used to  localize the defective via. This paper also discusses the way to  avoid beam caused sample damage and how to apply it for  further grounding and FIB cross sectioning to reveal the  defect.


PVC has been used for semiconductor fault isolation for  more than 20 years and it is very useful in detecting  open/leakage cases [1]. The traditional PVC procedure is:


1. Polish or deprocess to expose the conductive node, poly  or metal line;


2. Apply FIB or low KeV SEM to image the area of interest  to find contrast difference to get defect location.


Ion beam or low KeV E-beam is used most commonly for  PVC because the ion beam has stronger electron yield than  that of E-beam. Low KeV e-beam yields the better PVC result  over high KeV(see Figure 1 and 2 from [2]). However, in the  real world, ion beam or low KV e-beam does not always work. The following are some examples where ion beam or low KeV  SEM does not work. In these cases, high KeV e-beam is useful  for fault isolation.


Met1


CT


CrSi resistor


Case Study #1: CrSi resistor open


Bench test result points to open CrSi resistor as  the root cause of yield loss. The structure of the resistor  contains only two contacts and the snake shape of resistor  itself. FIB cross-sectioning is performed and indicates  both contacts are good (Fig.3). This suggests the electrical  open is in the snake shape of the thin CrSi resistor.


Fig3: STEM image showing good contacts to the  CrSi layer.


Fig. 1 Comparison of Charging in FIB and SEM from


[2].


Fig. 2 Influence of the beam energy to the emission yield  in SEM from [2]. The threshold voltage E1 and E2  depend on sample, sample material and SEM  configuration like beam current, chuck to ground  resistance, vacuum, etc.


The obstacle now is how to localize the defect  location. If the resistor were a thick poly resistor, deprocessing and then PVC observation would be the  ideal technique.  However, this CrSi is less than 30nm  thick and any procedure to expose it, such as parallel  lapping or deprocessing, without damaging the thin layer  is impossible. To avoid such issue, high KeV electron  beam PVC was considered. It is well know that SEM  beams penetrate deeper with higher accelerate voltage [3]. The tear drop shape of the effective volume is shown in  Fig. 4.


It gave us a hint that with high KeV beam, SEM can  reach the node that is covered with a layer of dielectric.   Our approach is as follows:


a) Polish the sample to remove other dummy layers on  top of the snake CrSi resistor;


b)  Ground a contact of the resistor by using FIB  depositing;


c) Observe the area of interest by using high KeV  electron beam.


The defect location is successfully isolated, as shown in  Fig. 5.


Use of the FIB to locally thin the dielectric on top in  the region where the defect was localized revealed a clear  SEM top down image of the defect as shown in Fig. 6. Since this resistor has wide band structure, this top –down  image shows the detail about the defect shape. Until this  moment, the sample is still covered with a thin dielectric  layer on top of the resistor. Next, cross section was  performed and the STEM image of the opening of the  resistor is shown in Fig. 7.


The both top and cross section view of the defect  provide more information about the defect than regular  FIB cross section. Using this technique to get such 3-D  information is very helpful for process engineer to figure  out defect root cause.


X-section cut(Fig. 3)


Case Study #2: Beam sensitive via chain open


1) Sample background


The second case study involves the technology with 4  layer of metal line and all metal layers are copper. Copper  as metal line has been used in semiconductor device for


Fig. 5 High KeV PVC reveals the defect location of  CrSi resistor.


Fig. 7 Cross-section view STEM image of the  open CrSi resistor.


Fig. 6 Top-down view SEM image of the defect.


Fig. 4 The effective interaction volume of SEM from


more than a dozen years [4] but via void is still a main  issue in such device failure. In order to distinguish such  defects from others, long via chain modules are designed  and produced to aid in process development.


In our experiment, the module has a snake structure  that contains one million vias between 2 probe pads. Its  structure is shown in Fig. 8.


After micro-probing the resistance between the two  pads, via open was confirmed.  Then the sample was put  in plasma etching to remove a covering dielectric layer to  expose the metal line. Next, it was put in FIB/SEM dual  beam system for fault localization by means of passive  voltage contrast.


2) First PVC attempt


Grounding one end of the snake to stage and leaving  another one floating is a necessary step to gain PVC [2]. The normal procedure is digging a deep hole on or near  the pad to be grounded to reach Si substrate and deposit


OBIRCH spot


Pt or W to connect the Pad to the substrate through the  FIB hole. In this way, Si substrate gets connected to the  pad. According to PVC theory, applying a  negative/positive charge on via chain may reveal the  location of the open because the floating part of the


PVC location


sample will be charged and the grounding part will not. The separation part is the defect location.


However, in our experiment, there is no clear PVC  shown under ion beam. Occasionally, one spot was seen  under low magnification and it disappeared when  zooming-in. And then it appears in the other place when  zoom-out.


Retest of the sample in bench shows the previous “open” becomes “high resistive”. In the other words, its  resistance change from larger than 1×109 Ohm to less  than or equal to 5×107 Ohm. It indicates the sample  recovered after PVC observation with FIB.  This result  suggests sample is ion beam sensitive.


3) FIB free sample grounding


Since the sample is ion beam sensitive, we need to  find FIB free procedure for defect localization. Laser  zapping is a good method for pad grounding.  Unfortunately, there is no laser machine in our lab. The  pad is 75 micron meter square in size and its metal is  exposed. Such characteristic allow directly hand painting  conductive material to a pad. The successful FIB free  grounding method is: fasten the sample to stage with  sticky copper tape and then carefully paint with graphite  paste from via chain pad to the copper tape.


4) Other Fault localization methods


Since FIB caused sample recovery, low KeV SEM is  used for passive voltage contrast. However, in our case  the PVC is still intermittent. Such sample seems very easy  to get contaminated under low KeV SEM. While zooming  in for detail location, contamination accumulates rapidly. OBIRCH (Optical Beam Induced Resistance CHange) is  also a popular fault isolation method, although it is not as  precise as PVC. In order to get more information, OBIRCH analysis was also performed on several samples. One sample had PVC in the very beginning observation, but it disappears upon ion beam inspection at high  magnification. Subsequent electrical measurement reveals  a resistance change in the sample-- it recovered after FIB  observation. This sample had no OBIRCH spot before  sample recovery; It had OBIRCH spot but it is not the  original PVC location.


This result suggests:


a) OBIRCH spot only appeared in a certain resistance


range (102 < R < 108 ohm from our experiments).


b) There are multiple via voids in the sample.


OBIRCH spot is about few micrometer sizes that  involves more than one snake lines. This fault localization  is not precise enough for further sample cross sectioning.


5) High KeV PVC for copper


Ideally, we would like to isolate the defect location  on one specific metal line/via segment for FIB cross  sectioning. The bottle neck is how to get one. Copper  metal line has the following characteristics: a). it easily  gets oxidized after it exposed in air; b) it reacts with O2  that is left over in the FIB chamber. Also, the image gets  degraded when observing the sample at high  magnification due to accumulation of hydro-carbon. Such  problems can be resolved by leaving a thin layer of  dielectric on top of copper line.  Copper won’t get  oxidized so the copper lines won’t short to each other. Beam caused contamination may still occur but it can be  ignored if high KV electron beam is used for observation. The result with 10 KeV observations is shown in Fig. 10.


Fig. 9 OBIRCH (left) and PVC (right) images of the  same sample showing the OBIRCH spot location  different from the original PVC location.


Fig. 8 Schematic drawing of Via chain structure


6) Advanced electrical testing


Normal DMM and SMU test systems cannot provide  the current measurement as accurate as pico-amp. In order  to get the detail about in which resistance PVC is  available, more precise electric measurement was  performed using picometer and carefully control the  ramping slope of the applied voltage (1V). A systematic  study suggests minimum resistance of 4GOhm (500pA @2V) is required to get PVC in our experiment. That is, if  resistance is lower than 4×109 ohm, PVC cannot identify  the defect location.


7) Influence of dielectric thickness to PVC


How does thickness of the dielectric layer influence  PVC is also an interesting topic. In our experiment, we  selected a sample that has about 850nm thick oxide on the  top and then thin it with plasma etcher.  This sample was  observed in SEM with variable KeV. The result is shown  in Fig.11. The oxide thickness varies at 830nm, 480nm  and 190nm.  It was found that the thickness does not  affect PVC much; although, it is necessary to adjust  accelerate voltage accordingly. The thinner the dielectric  layer is, the lower kV to get PVC. The lowest KV to show  PVC is 4kv,3kv and 2 kv for thickness of 830nm,480nm  and 190nm. With 30 KV, PVC is shown when the sample  is 830nm, but not when the thickness is less than 480nm.


8) Cross section results


FIB cross sectioning was performed after defect  localization. Three different kinds of opening were seen  as shown in Figure 12, 13 and 14.


The sample in Fig.12 has resistance is 106 ohm range, localized with OBIRCH spot; the one in Fig. 13 has  resistance range 109 ohm range, in which high kV PVC  can barely get the location. Its mass contrast in STEM


Fig. 10 10KeV SEM image with PVC showing defect  location.


Fig. 11 Effect of oxide thickness on PVC: top row  oxide thickness 830 nm, center row 480 nm, and  bottom row 190 nm.


Fig. 12 Cross-section STEM image of via defect (with resistance ~ 106 ohm) isolated by OBIRCH.


Fig. 13 Cross-section STEM image of via defect (with resistance ~ 109 ohm) isolated by high KeV  PVC.


Fig. 14 Cross-section STEM image of complete  open via defect by high KeV PVC.


image indicates the shadow is diffused metal, because it is  heavier than SiO2. The sample in Fig. 14 is an example of  a complete electrical open via chain sample. Cross-section  image is the clue leading to defect root cause. The Fig. 14  clear tells us Via etching is the issue. However, the one in  Fig. 12 did not provide clear information as in Fig.14 due  to damage occurred. It would be ideal to avoid beam  caused sample damage.


9) Prepare charge-free sample


The previous sample was prepared with FIB and ion  beam causes damage to the sample, especially at the weak  spot, such as voids. The shadow kind of damage is most  likely caused due to ion beam damage. The key to avoid  FIB caused damage is to dissipate charges.


The following is our procedure to get rid of ion  charging problem:


a) Use Carbon paste to ground sample


b) E- beam PVC to find location


c) Mark the location with e-beam deposition


d) Apply carbon paste to ground both pads that  connect via chain. In this way, there is no  potential near the void.


e) Coat the sample with gold to avoid surface  charging.


f) Perform FIB-section.


Fig. 15 is the cross-section STEM image of charge free  sample with via defect.


10) Discussion


For a sensitive via structure, ion beam can result in  damage at a weak spot. In this way, the original “open” sample (resistance>10-9ohm) becomes high resistive (resistance 10-6 ohm). E-beam PVC is the good method  to localize the defect. Electron beam does not cause  damage because electron can easily dissipate.  However, low KeV e-beam is not as effective because copper easily  get oxidized and contaminated.


High KV e-beam with passivated sample works very  well in this case. This method also avoids sample


preparation that saves time and avoids possible sample  damage.


From two case studies, we learned that high KeV  electron beam can be very useful in certain cases  especially for very thin conductive layer and/or copper  metal lines. Electron beam can be used to deal with ion  beam sensitive sample because charge dissipates easier.


1. Mehrdad Mahanpour, “Emission microscope and  passive voltage contrast: Solving a problem quickly”, III-Vs Review, Volume 9, Issue 6, December 1996, Pages 46–47, 49–50.


2. Ruediger Rosenkranz, ‘Failure localization with  active and passive voltage contrast


in FIB and SEM”, J Mater Sci: Mater Electron (2011) 22:1523–1535


3. Dr Aïcha Hessler-Wyser, Scanning Electron  Microscopy,


p22. http://cime.epfl.ch/files/content/sites/cime2/files/shar ed/Files/Teaching/MSE_603_2011_spring/Chapter%203%20-%20SEM.pdf.


4. David Su, et al, Microelectronic Failure Analysis: Desk Reference: 2001 Supplement, ASM  International published, pp.85-95.


Fig. 15 Cross-section STEM image of a charge free  sample with via defect.


In-line Defects Overlaying with Functional Failures and Characterization for Fast  Defect Learning and Fast Yield Improvement


Zhigang Song1, Oliver D. Patterson and Qian Xu


IBM Systems and Technology, 2070 Route 52, Hopewell Junction, NY, USA


1. Email: zsong@us.ibm.com; Tel: 845-892-1691; Fax: 845-892-6094


Process defects, either random or systematic, are often the top  killers of any semiconductor device. Process defect learning  and reduction are the main focuses in both technology  development stage and product manufacturing yield ramp  stage. In order to achieve fast defect learning, in-line defect  inspection is implemented in critical layers during wafer  manufacturing. In-line defect inspection is able to detect  defects. However, in-line defect inspection alone cannot  predict the impact of defects on device functional yield. Failure analysis is an effective method of finding the defects  which really cause device functional failures. However, often, the defects found by failure analysis are very different from the  original defects, making it difficult to understand the root  cause. This paper will describe a methodology how to combine  in-line defect inspection and failure analysis together to found  the top killer defects and accelerate their root cause  identification for fast defect learning and yield improvement.


Process defects, either random or systematic, are often the top  killers of any semiconductor device. Process defect learning  and reduction are the main focuses during both technology  development and product manufacturing yield ramp. It is  common practice to use in-line defect inspection to capture  defects at their source layer for multiple critical layers during  wafer manufacturing. In-line defect inspection techniques, such as bright field, dark field of optical inspection and  Electron Beam (EB) inspection [1-4], are capable of detecting  defects. However, in-line defect inspection technique alone  cannot measure the impact of these detected in-line defects on  device functional yield. Current advanced semiconductor  technology has become so tremendously complicated that even  forming a single layer requires many process steps. Some inline defects look catastrophic at their beginning, but they may  be removed or remedied by subsequent processes and become  non-killer defects, while other tiny in-line defects may be  exacerbated by subsequent processes and become catastrophic. In order to achieve fast defect learning and yield improvement  under this situation with so many types of in-line defects and  limited resources, it is important to deploy the limited  resources to focus on the defects with the greatest yield


impact. Failure analysis is an effective method of determining  which defects really cause functional failures [5-7]. However, sometimes the defects found by failure analysis have been  substantially transformed from the original defects by  processing. Thus identification of the source layer and source  process step for such defects is still difficult and may take one  or two months. Overlaying in-line defects with functional  failures and subsequent characterization of these defects via  physical failure analysis, not only identify the top killer defects  for integration and unit process communities to work on, but  also provide understanding of how the original defect  transformed to the final defect. This additional information  helps the integration and unit process communities resolve  these defects for fast yield improvement.


In-line Defects Overlaying with Functional  Failures and Characterization Methodology


In-line defect inspection is an important step for defect  learning. However, in-line inspection alone often cannot  predict the impact that defects will have on device functional  yield. To understand whether an in-line defect is a yield killer, the in-line defects are overlaid with functional test failures. If a  defect matches a functional failure, the defect is classified as a  killer defect. If not, it is not a killer defect. Often, whether a  type of defect causes a functional failure depends on its size  and location. In this case, the kill ratio of this defect type can  be calculated by dividing the number of defects matching with  a functional failure by the total overlaid defects. After this  overlay analysis is completed, physical failure analysis is  performed to understand how some defects cause a functional  failure or why other defects do not cause any failure. This  information establishes the kill ratio for in-line inspection  defects. It can be used to more effectively predict yield and  illustrates the failure mechanism so that the integration team  can best address it.


Figure 1 shows the flowchart of the “In-line Defects  Overlaying with Functional Failures and Characterization  Methodology” used in this paper. During wafer manufacturing, in-line defect inspection is performed at several critical layers  and the defect types and locations are stored in a file. The  wafer is continuously processed to certain layer and a  functional macro, such as Static Random Access Memory


Wafer


Manufacturing


Inline Defect  inspection


Wafer Manufacturing


to certain layer


Inline


functional test


Defect types  and locations


Failure types  and locations


Layout viewer


Set an offset radius


Match


Killer defect


Non-match


Non -killer defect


Physical failure analysis


Figure 1: The flowchart of in-line defects overlaying with  functional failures and characterization methodology.


EBI, Dark contact


VPF


Figure 2: An example of an in-line defect overlaid with a  functional failure using a layout viewer.


(SRAM), is tested. The functional test failure types and  locations are recorded. Both in-line defect types and locations  and functional failure types and locations are loaded into a  layout viewer. It is often found that an in-line defect and the  SRAM bitcell failure caused by it are not at the same locations  exactly. This is due to the alignment and movement accuracy  of the inspection tools. To compensate for this, a constant  offset (R) is assumed for a particular in-line inspection tool  and a circle with radius R is drawn from each of the in-line  defects detected by the inspection tool. As long as a functional  failure falls within the circle with radius R centered at an inline defect, the in-line defect is considered to match the  functional failure. Thus the defect is believed to have caused  the functional failure. Figure 2 is an example of an in-line  defect overlaid with a functional failure using a layout viewer. The in-line defect is a dark contact detected by EBI; the  functional failure is vertical pair bit failure.  The offset R in  this case was 2um. If there is not any functional failure falling


into the circle, this in-line defect is a non killer defect. For  both cases, follow-up physical failure analysis is performed to  understand how an in-line defect causes a functional failure or  why a defect does not cause any functional failure.


Case Studies


In this section, five in-line defects were overlaid with  functional test failures employing the methodology described  in the previous section. Figure 3 shows the calculated kill  ratios for these five in-line defects based on the overlay results. The prior layer defect had zero hits; In other words, it was a  non-killer defect; the kill ratios of Replaced Metal Gate (RMG) metal voiding and poly Si residue in RMG were 40% and 70% respectively; and poly spacer voiding and EBI dark  contact had 100% kill ratios.  Subsequent physical failure  analysis was performed to characterize the non-killer priorlayer defect, and the killer poly spacer voiding and poly Si  residue in RMG to understand why the prior-level defect did  not cause any functional failure and how, on the other hand, a  tiny poly spacer void and poly Si residue in RMG caused  functional failures.


It is worthy to mentioning that except EBI dark contact  detected by In-line E-beam inspection using passive voltage  contrast mode [8], RMG voiding, poly Si residue in RMG and  poly spacer voiding were captured by in-line E-beam  inspection using physical inspection mode. In the last several  years, E-beam inspection has become popular for physical  defect detection because of significant improvements in  inspection resolution and also because many critical defects  are now at the edge of optical inspection detection capability. E-beam inspection provides superior detection capability for  these gate level defect types because of higher resolution  compared to optical inspection.  This higher resolution enables  to achieve a much greater detection rate and the ability to  automatically bin defects [9].  The drawback in using E-beam  inspection continues to be throughput and so generally it is  used in complement to optical inspection for tricky levels.


Prior-layer defect


RMG Voiding Poly Si residue in RMG


Poly Spacer


voding


EBI dark contact


Defects


Figure 3: Kill ratios for five different in-line defects.


A.  Prior-Layer Defect


In-line optical inspection after M3 CMP found a type of  defect, which was not observed with Scanning Electron  Microscope (SEM) review (see Figure 4). Thus, the defect was  not at the M3 layer and therefore assumed to be from a prior  layer. However, in-line inspection at prior layers did not show  any defect at the same location. To understand the mystery of  this defect formation and source layer, after SRAM functional  test which occurred at M6 layer, several of these prior-layer  defects were overlaid with the functional failures in this wafer  and it was found that none of these defects matched with any  functional failure, indicating this prior-layer defect is not a  killer defect. Figure 5 is an example of a prior-layer defect  overlaid with the functional failures for a particular chip.


Figure 4: The optical bright field image of an in-line defect at  right side. SEM review image at left side did not show any  defect.


Figure 5: Overlay of a prior defect with the function test  results for this chip found that the defect did not match any  functional failure.


It shows that the segment containing the prior-layer defect was  perfect. Since the prior-layer defect location in a chip was  located with the layout viewer, referring to Figure 5, the chip  was de-processed to the M3 layer and top down SEM  inspection was performed. No abnormalities were found at the  reported in-line defect location (see Figure 6). Then the  sample was submitted to Focused Ion Beam (FIB) crosssection. The FIB X-section image, shown in Figure 7, discovered delamination between the metal cap layer and M1


at the in-line defect location. So, it is believed that there was  certain contamination after M1 CMP, which was not  detectable by in-line inspection. When the wafer was  processed to M3 layer, the contamination site delaminated due  to thermal stress variation during subsequent processing. The  delaminating caused a pop-up shape, which scattered the  inspection light beam, making it be detected as a defect. Obviously, this delaminating did not cause any functional  failure at time zero, but it still was a concern for reliability.


Figure 6: SEM image after deprocessing to the M3 layer did  not show abnormalities at the reported in-line defect location.


Figure 7: FIB x-section showing delamination between the  metal cap layer and M1.


B.  Poly Spacer Voiding


In-line E-beam inspection showed a type of defect called poly  spacer voiding after poly spacer formation. Overlaying some  of the poly spacer voiding defects with functional failures


Figure 8: In-line E-beam inspection image of a poly spacer  voiding defect.


Figure 9: SEM image showing contact W filling pass-gate and  local gate lines and the active area between these two poly  lines.


showed that this type of defect had a 100% kill ratio and  caused different functional failures, such as horizontal pair bit  failures (HPF), quad cell failures (QCF), and single cell  failures (SCF), depending on defect size and location. In this  case study, a tiny poly spacer void (see Figure 8) matched with  a HPF. To understand how this tiny poly spacer void caused a  HPF, the chip was de-processed to the poly level and SEM  inspection was performed at the location of the HPF. The SEM  image in Figure 9 shows contact W filling a pass-gate poly, a


local poly and the active area between these two poly lines. Since the pass-gate poly, which was shared by two cells in  row, was damaged, it was understood that a HPF was caused.


How was a tiny spacer void transformed to such a big  catastrophic defect causing a HPF? Here is the scenario. During poly Si removal for RMG, the chemical used for  etching the poly Si seeped through the poly spacer void and  attacked the active Si, leaving a big void in the active and a  portion of the void under the poly lines. Then the big void and  the poly were filled with RMG materials. When the wafer was  processed to the silicide and contact formation steps, the  chemical used for removal of un-reactive silicide metal etched  away the RMG materials in the void and the adjacent poly  lines and then the contact W re-filled the void and adjacent  poly, creating a big defect as shown in Figure 9. In this case, if  the defect was found based on failure analysis for a functional  failure without knowing about the poly spacer void detected by  in-line inspection, identification of the root cause of this defect  would be very difficult.


C.  Poly Si Residue in RMG


Another type of in-line defect, called poly Si residue in RMG, was detected by in-line E-beam inspection after poly Si  removal. Overlaying several defects of this type with  functional failures showed that poly Si residue in RMG has a  70% kill ratio, mainly causing SCF and HPF. Some small poly  Si residue defects in the portion of poly over Shallow Trench  Isolation (STI) areas do not cause functional failures. Figure  10 shows an image of a typical poly Si residue defect in RMG, which matched with a SCF. To establish the link between this  poly Si residue and the SCF, the chip was de-processed to the  poly layer and SEM inspection was performed.


Figure 10: In-line E-beam inspection image of a poly Si  residue in RMG.


Figure 11 is the SEM image of the SCF at the poly layer. It  shows missing RMG metal, pointed out by an arrow, at a pulldown transistor of the SCF. As the sacrificial poly Si was not  totally removed, the subsequent high K gate dielectrics and  RMG metal did not fill the poly at the pull-down transistor, leading to a failing pull-down transistor, which was  responsible for the SCF. Once again, knowing the in-line  defect was very helpful to understand the root cause of the  missing RMG metal defect which caused a SCF.


Figure 11: SEM image showing RMG metal is missing within  a pull-down transistor, pointed by a black arrow.  The right  image is the zoom-in image of the defect.


In-line defect inspection is an important step for defect  learning.  However, in-line defect inspection alone cannot  predict the impact of defects on device functional yield. Failure analysis is an effective method of finding the defects  which really cause device functional failures. However, often, the defects found by failure analysis are very different from the  original defects, making it difficult to understand the root  cause. Overlaying in-line defects with functional failures and  then applying physical failure analysis to characterize these  defects can establish the kill ratio for in-line inspection  defects, prioritize which defects integration and unit process  communities should work on, and also make it much easier to  understand the root cause. Following this methodology enables  the integration and unit process communities to achieve faster  defect learning as well as yield improvement.


This work was performed at Semiconductor Research & Development Center, IBM Microelectronics Division, Hopewell Junction, New York 12533. The authors also  appreciate Thuy Su and Aaron Shore for their help in physical  failure analysis and FIB cross-section.


[1] X. Ouyang, D. Riggs, I. Ahsan, O. D. Patterson, D. Lea, B. Ebersman, K. Hawkins, S. Fox, and J. Rice, “Yield  learning methodology in early technology development,” ASMC 2007 Proceedings, P.333 (2007).


[2] N.G. Shankar and Z.W. Zhong, “Defect detection on  semiconductor wafer surfaces”, Microelectronic  Engineering, vol. 77, P. 337 (2005).


[3] O. D. Patterson, K. Wu, D. Mocuta and K. Nafisi, “Voltage Contrast Inspection Methodology for In-line  Detection of Missing Spacer and Other Nonvisual  Defects”, IEEE Transactions on Semiconductor  Manufacturing, Vol. 21, No. 3, P. 322 (2008).


[4] O. D. Patterson, D. A. Ryan, M. D. Monkowski, D. Nguyen-ngoc, B. Morgenfeld, C. Lee, C. Liu, C. Chen, S. Chen, “Early Detection of Systematic Patterning Problems  for a 22nm SOI Technology using E-Beam Hot Spot  Inspection”, ASMC 2013 Proceedings, P. 295 (2013).


[5] Z. G. Song, J. Y. Dai, S. Ansari, C. K. Oh and S. Redkar, “Front-end Processing Defect Localization by Contactlevel Passive Voltage Contrast Technique and Root Cause  Analysis”, IPFA’ 2002 Proceedings, P. 97 (2002).


[6] R. Desineni, Z. Berndlmaier, J. Winslow, A. Blauberg, and B. R. Chu, “The Grand Pareto: A methodology for  identifying and quantifying yield detractors in volume  semiconductor manufacturing,” IEEE Trans. Semiconductor Manufacturing, Vol. 20, P. 87 (2007).


[7] E. Zschech, E. Langer, H.-J. Engelmann, and K. Dittmar, “Physical failure analysis in semiconductor industry—challenges of the copper interconnect process,” Materials  Science in Semiconductor Processing, Vol. 5, P. 457 (2002).


[8] O. D. Patterson, J. L. Drown, B. D. Crevasse, A. Salah, K. K. Harris, “Real Time Fault Site Isolation of Front-end  Defects in ULSI-ESRAM Utilizing In-Line Passive  Voltage Contrast Analysis”, ISTFA’ 2002 Proceedings, P. 591 (2002).


[9] O. D. Patterson, J. Lee, D. Salvador, S. C. C. Lei, X. Tang “Detection of Sub-Design Rule Physical Defects using EBeam Inspection”, IEEE Trans on Semiconductor  Manufacturing, Vol. 26, Issue 4, P. 476 (2013).


Observation of Channel Strain Release in pMOS Device with Low Idsat using  Energy-filtered Nano-beam Diffraction Technique


Jie Zhu, An Yan Du, Bing Hai Liu, Eddie Er, Si Ping Zhao and Jeffrey Lam


GLOBALFOUNDRIES, 60 Woodlands Industrial Park D, Street 2, Singapore 738406  Phone: (+65) 66701539.   Fax: (+65) 6362-2938.   Email: JIE.ZHU@globalfoundries.com


In this work, energy-filtered TEM nano-beam diffraction (NBD) technique was used to evaluate channel strain profile  in pMOS transistors suffering low Idsat issue. TEM and EDX  analysis showed nickel deep diffusion into embedded SiGe  source/drain. Such defect not only led to leakage current from  S/D to substrate but might also reduce compressive strain  induced to channel by eSiGe. Comparison of channeldirection strain between bad and good samples using NBD  confirmed strain relaxation in bad sample which explained  low Idsat as a result of reduced holes mobility.


Strain engineering is one of the predominant techniques used  in advanced semiconductor devices to boost performance of  MOSFETs. Increase in electron and hole mobility is  attributed to conduction and valence energy band structure  change when material is being stressed [1]. Among all strain  engineering techniques, epitaxial growth of embedded SiGe (eSiGe) in transistor’s source/drain is very cost-effective for  pMOSFETs hole mobility enhancement. Large compressive  strain along channel direction and tensile strain  perpendicular to the wafer surface can be introduced to the  channel region due to lattice mismatch between SiGe and Si, depending on the physical structure and Ge concentration of  eSiGe. This technique has been used since sub-100 nm  devices and has now been extended to 32 nm technology and  even below. Several strain measurement results on MOSFETs  have been reported using different analysis techniques such as  nano-beam diffraction (NBD), dark-field off-axis holography  strain mapping (DFOH), and convergent-beam electron  diffraction (CBED) techniques [2,3]. In this work, energyfiltered NBD technique was applied to evaluate strain profile  of pMOS transistors suffering low Idsat issue. With energy  filter, root-mean square deviation of NBD strain analysis was


0.05% based on measurement on Si substrate. Si channel  strain relaxation was found in transistors with deep nickel  diffusion into eSiGe source/drain. To the best of our  knowledge, this is the first time failure analysis observation of  device performance degradation related to strain relaxation.


Electrical Fault Isolation


A combination of TIVA and AFP techniques were used to  isolate failure location on target die. TIVA spots were  detected at several locations in SRAM blocks of failed device  with low Idsat. AFP technique observed gross pMOS to  nMOS leakage. Subsequent IC curve tracing on this location  confirmed characteristic leakage (VDD Vs. VSS core).


TEM Sample Preparation and Analysis


Upon electrical fault isolation, sample was analyzed by TEM  in order to find out physical defect signature. Focused-ion  beam milling was used to prepare TEM lamella on pMOS  transistors with channel along -220 of Si crystallographic  direction. 300kV TEM (Titan) equipped with EDX detector  was used to perform physical and chemical characterizations.


NBD Strain Measurement


Nano-beam diffraction was performed under STEM µm-probe  mode using smallest condenser aperture in order to achieve  nearly-parallel electron beam. Semi-convergence angle of  electron probe was measured to be 0.24 mrad. Gatan energy  filter with energy slit width of 10 eV was used to partially  filter out inelastic scattering electrons and increase signal to  noise ratio. Fig. 1 shows schematic drawing of electron  diffraction geometry in TEM. It can be deduced that lattice  plane distance is related to other parameters by equation:





 Ld


where, R is the distance measured from the center of direct  beam (O’) to the center of diffraction beam (G’), d is the  lattice plane distance, L and λ are the cameral length and  wavelength of electron beam, respectively. Strain value can  therefore be calculated as follow:





Figure 1: Schematic drawing of TEM diffraction shows  geometric correlation between parameters including camera  length (L), electron wave length (λ), lattice plane distance (d), and distance from direct beam O’ to diffraction beam G’ (R).


Figure 2: Energy-filtered NBD pattern from Si substrate. Device channel is along -220 diffraction beam direction.


where, εi is the strain, d0, R0 and di, Ri are the values obtained  from diffraction patterns corresponding to the reference and  strained location, respectively. In order to improve NBD  measurement accuracy, a large camera length (L) was used so  that -220 and 2-20 diffraction beams spanned the whole CCD


Figure 3: NBD strain plot on strain-free Si substrate. The  root-mean square (RMS) deviation was measured to be


0.05%.


area (2K x 2K pixel size) as much as possible. One typical  NBD diffraction pattern taken on Si substrate was shown in  Fig. 2 and (-220) diffraction beam corresponded to the  channel direction of transistor. All diffraction patterns were  analyzed using public domain software “ImageJ” by batch  data refinement. NBD strain value was measured on strainfree Si substrate area and root-mean square deviation was  measured to be 0.05% (Fig. 3).


TEM images of pMOSFETs from TIVA spot and reference  locations are shown in Fig. 4. It was observed that nickel  might diffuse deep into eSiGe source/drain in failure sample. In good sample, Ni silicide depth was much shallower as  compared with bad sample. Deep nickel diffusion into eSiGe  was further confirmed by EDX line scan as indicated by  extended Ni signal tail beyond normal silicide depth, as  shown in Fig. 5. EDX line scan of nickel silicide from good  sample is given in Fig. 6 for comparison. Deep nickel  diffusion into eSiGe correlated with electrical test which  showed source/drain to substrate current leakage. Another


Figure 4: TEM images of pMOS transistors of (a) good and


(b) bad samples. Deep Ni diffusion into eSiGe was observed  in bad sample.


Figure 5: TEM EDX line scan on bad sample. Ni diffusion  into eSiGe was indicated by Ni signal tail in EDX line  profile.


Figure 6: TEM EDX line scan on good sample. No abnormal  Ni diffusion was observed.


electrical failure signature was that the Idsat value of  pMOSFETs from bad unit was ~15% lower comparing with  good unit. Saturation current (Idsat) of MOSFET is given by:


Id


)( VVtg2


 


ox


sat


L2m


where, µeff is the effective mobility of charge carrier, Cox is  gate oxide capacitance, W and L are channel width and  length of transistor, Vg and Vt are gate voltage and threshold  voltage, and m is related to the sub-threshold slope and body  effect. In equation 3, there is a linear relation between  saturation current and effective mobility of charge carriers. The mobility of carriers is linearly proportional to the channel  strain according to the classic piezoresistance model at  relatively low stress region. Since eSiGe strain engineering  technique was used in this device and deep Ni diffusion into  eSiGe was observed, it was most likely that lower Idsat value  was caused by reduced hole mobility resulting from channel  strain release. In the next step of failure analysis, TEM  energy-filtered nano-beam diffraction technique was used to  measure channel strain profile on both failure and good  samples. As shown in Fig. 7, channel direction strain (ε-220) was measured in each sample along a line starting at a depth  of ~ 8 nm below the gate oxide. From NBD strain plots in  Fig. 7, it shows that there is obvious channel strain difference  between failure and good samples. In good sample, relatively  large compressive strain (~ -0.3%) was measured in channel  area and strain decreases to zero at a depth of ~ 65 nm.


However in failure sample, it was observed that the  compressive strain in channel area was only ~ -0.1%. Fig. 8  shows NBD strain (ε-220) measured on a horizontal line at  depth of ~ 30 nm below the gate oxide. Again from NBD  strain plots, it is observed that there is clear strain release in  failure sample. The average compressive strain measured  from good sample was -0.27% while the strain was nearly  zero in failure sample (Fig. 8). From NBD strain analysis, we  showed that the lower Idsat value of failure sample was  related to strain release in channel area.


Figure 7: Energy-filtered NBD strain plot from both good  and bad samples. Relatively large compressive strain (-220  direction) was observed in good sample while strain release  was observed in bad sample in channel area.


Figure 8: Energy-filtered NBD strain plot from both good  and bad samples. Measurement region is ~ 30 nm below gate  oxide.


In summary, TEM energy-filtered nano-beam diffraction  technique was used to measure channel strain of pMOSFETs  suffering source/drain to substrate leakage and low Idsat  issue. Deep Ni diffusion into eSiGe was observed by TEM  analysis which introduced S/D to substrate current leakage.  NBD strain analysis was used to show large strain release in  channel area and thus it was believed that the low Idsat was  most likely due to reduction in hole mobility because of strain  relaxation.


Authors would like to thank GLOBALFOUNDRIES  Singapore TD EFA group for performing electrical failure  analysis on failed device. We also appreciate encouragement  and support from management team during this project  development.


[1]  M. Chu, Y. K. Sun, A. Umamaheswari and S. E. Thompson, “Strain: A Solution for Higher Carrier  Mobility in Nanoscale MOSFETs”, Annual Review of  Materials Research. Vol. 39 (2009), pp. 203-239.


[2] K. Usuda, T. Numata and S. Takagi, “Strain Evaluation  of Strained-Si Layers on SiGe by the Nano-beam  Electron Eiffraction (NBD) Method”, Materials Science  in Semiconductor Processing, Vol. 8 (2005), pp. 155-159.


[3] M. Hÿtch, F. Houdellier, F. Hüe and E. Snoeck, “Nanoscale Holographic Interferometry for Strain  Measurements in Electronic Devices”, Nature, Vol. 453 (2008), pp. 1086-1089.


Effective and Efficient FEOL Defects Localization/ Inspection by Selective  Mechanical/Chemical deprocessing


Ng Hui Peng, Teo Angela, Ang Ghim Boon, Yip Kim Hong, Dr Chen Chang Qing, Dr Quah Alfred, Tam Yong Seng, Dr Jeffrey Lam, Dr Mai Zhi Hong


Product, Test and Failure Analysis group, GLOBALFOUNDRIES Singapore Pte Ltd


Email: HuiPeng.NG@globalfoundries.com


[4] R. Young, S. Henstra, J. Chmelik, T. Dingle, A. Mangnus, G. van Veen, I. Gestmann, XHR SEM: enabling  extreme high resolution scanning electron microscopy, Proc. SPIE 7378, pp. 737803, 2009.   doi:10.1117/12.824749


[5] Alvis, R. et al., High-Throughput, Site-Specific Sample  Prep of Ultra-Thin TEM Lamella for Process  Metrology and Failure Analysis, ISTFA 2012: Conference Proceedings from the 38th International  Symposium for Testing and Failure Analysis (ASM  International), November 11-15, 2012, Phoenix  Arizona.


[6] http://www.fei.com/Products/ExSolve/


(accessed 2014-0721)


[7] Altmann, F., Young, R., J. Micro/Nanolith. MEMS  MOEMS 13(1), 011202 (Jan–Mar 2014)


[8] http://www.fei.com/products/fib/vion-plasma/?ind=el


[9] Donnet, et al, Delayering on Advanced Process  Technologies using FIB, elsewhere in the ISTFA 2014: Conference Proceedings from the 40th International  Symposium for Testing and Failure Analysis


[10] Helios PFIB reference


[11] http://www.chipworks.com/en/technical-competitiveanalysis/resources/blog/samsung-amoled-in-the-galaxys4-moves-the-needle/?lang=en&Itemid=815y (accessed  2014-0721)


[12] http://informationdisplay.org/IDArchive/2013


/MarchApril/DisplayMarketplaceAMOLEDProduction.


aspx (accessed 2014-0721)


[13] see for example, http://www.stuff-review.com/2012-04/samsung-is-ready-to-mass-produce-flexibleunbreakable-and-lighter-amoled-displays-called-youm/ (accessed 2014-0907)


[14] see for example, http://www.extremetech.com/computing /170970-igzo-display-tech-finally-makes-it-to-massmarket-ipad-air-now-high-res-laptops-and-desktopsnext (accessed 2014-0907)


[15] http://www.anandtech.com/show/7743/the-pixel-densityrace-and-its-technical-merits (accessed 2014-0907)


[16] see for example, http://www.androidcentral.com/quickdisplay-comparison-samsung-galaxy-s4-versuscompetition (accessed 2014-0907)


[17] http://blog.samsungdisplay.com/731 (accessed 2014-0721)


[18] http://www.fei.com/products/dualbeam/helios-nanolab/  (accessed 2014-0721)


[19] http://www.fei.com/products/FIB/Vion/ (accessed 2014-0721). Helios PFIB DualBeam product announced at  2014 Microscopy and Microanalysis Meeting


[20] see for example, http://www.tedpella.com/grids_html/


4510half.htm (accessed 2014-0728)


[21] http://www.fei.com/software/maps/ (accessed 2014-0728)


[22] Sylvain Lefebvre and Hugues Hoppe, Compressed


Random-Access Trees for Spatially Coherent Data  Eurographics Symposium on Rendering (2007),  downloaded from http://research.microsoft.com/enus/um/people/ hoppe/ratrees.pdf (accessed 2014-0908)


[23] http://research.microsoft.com/en-us/um/redmond/groups /ivm/HDView/ (accessed 2014-0908)


### microPREPTM - A New Laser Tool for High-Throughput Sample Preparation


microPREPTM - A New Laser Tool for High-Throughput Sample Preparation


Michael Krause, Martin Ebert, Thomas Höche


Fraunhofer CAM, Fraunhofer Institute for Mechanics of Materials IWM, Walter-Huelse-Strasse 1, 06120 Halle, Germany  thomas.hoeche@iwmh.fraunhofer.de


Uwe Wagner


3D-Micromac AG, Technologie-Campus 8, 09125 Chemnitz, Germany


Over the past fifty year, lasers have found many, often  groundbreaking applications in science and technology. The  most important features of lasers are that photons are  inherently free of contamination, extremely high energy  densities can be focused in very small areas and the laser beam  can be precisely positioned using deflection mirrors. By  reducing pulse lengths from a few nanoseconds down to the  picosecond or femtosecond range, material ablation is  becoming increasingly “athermal”, i.e. structure damage by  local heating is reduced to well below a few microns. In view  of these outstanding characteristics of lasers, it is very  surprising that sample preparation for microstructure  diagnostics did not derive the advantages from laser micromachining.


microPREPTM, is a new laser-micromachining tool developed  by 3D-Micromac capable of making fast, clean, and efficient  laser ablation available for the preparation of samples for  transmission electron microscopy (TEM). The workflow  follows a three-stage approach. First, a supporting basic  structure is cut from the feedstock. Second, the supported  structure is laser-thinned down to a few microns and third, the  supported and laser-thinned structure is thinned using a  focused ion beam or an ion broad beam.


The examples presented in this paper support this approach  and show it is ready to be applied in different areas of  microstructure diagnostics and has very high potential for  failure diagnostics.


Lasers as reliable tools for micromachining


Being commercially available for many decades, lasers have  become indispensable and extremely reliable tools in many  areas of life, including the automotive industry (welding, drilling, and measuring), thin-film processing (scribing, patterning), and even esthetic surgery (dermabrasive ablation, LASIK).


In consideration of the fact that the application of lasers is so  wide spread, it is most surprising that the preparation of  samples for microstructure diagnostics has so far made only  little use of laser micromachining. Things are getting even  more incomprehensible when considering the favorable


properties of lasers. Laser radiation can, sufficiently high  power (or more precisely: fluences, i.e. area densities) provided, ablate all kind of materials. Using ultrashort pulses  and/or very high pulse energies, ablation is based on multiphoton absorption, enabling the machining of transparent-atthe-wavelength materials. The ablation rate of laser micromachining is about six orders of magnitude larger than that of  a Ga+-FIB and roughly three orders of magnitude higher than  the milling rate of a Xe+-Plasma-FIB.


Beyond the aforementioned advantages, lasers can be precisely  delivered and straight-forwardly focused using standard  optical elements like galvanometer scanners. Since laser  radiation consists of photons (it is not a corpuscular radiation  like ion beam that may tend to unwanted implantation effects), laser micromachining is very clean in terms of contamination.


Lasers meet preparation needs


There is an increasing demand for preparation techniques for  microstructure diagnostics that need to be fast, reliable, cost  effective, artifact-free, and targeted on the micron scale or  below. Besides traditional mechanical preparation, focusedion-beam micromachining is currently dominating the field. While the former is accompanied by high costs for skillful  personnel, the latter is characterized by very high costs of  ownership.


Figure 1: 3D-Micromac’s microPREP™ tool is a compact  desktop instrument.


In this contribution, we present the capabilities of a new tool  for laser-based preparation illustrated by a number of  examples. Based on several patents (e.g. by [1,2]), 3DMicromac’s microPREP™ tool (Figure 1) has a basic


functionality that consists of laser cutting of a base structure  followed by local laser thinning in an almost entirely  automated fashion. Making use of a rugged, ultrashort-pulse  laser source, the process is characterized by very low running  costs, suitability for semiconductors, metals, ceramics, as well  as compounds thereof, and a high targeted precision on the  micron scale.


Heat-Affected Zone (HAZ)


Widespread use of laser micromachining for the preparation of  microstructure-diagnostics samples has been hampered by  concerns regarding thermal damage to the samples. A few  points need to be considered in order to understand this effect. The interaction of short-pulsed (not ultrashort-pulsed) visiblerange laser radiation with matter is dominated by the formation  of a melt and expelling the latter from the location of  machining. This is because the electromagnetic wave couples  to the phononic system, and the excitation of phonons leads to  a local increase of temperature.


For ultra-short pulsed lasers, however, due to non-linear  optical effects, the excitation is attained via the electronic band  structure of the materials, leading to much reduced heat  effects. Ablation is not entirely non-thermal, but it proved to  be restricted to less than a few 100 nm [3, 4, 5]. Moreover, the  extent of this heat-affected zone (HAZ) can become larger  when the basic principles of laser micromachining are not  obeyed. For examples, too low feed rates and too high pulse  energies are to be avoided. Ultimately, one has to face the fact  that there is (and will always be) a certain layer of material on  a laser-machined surface that will contain structural damage. Similar effects are by the way known for the mechanical  grinding of metals and in Ga+ milling one has to accept  implantation and amorphization effects as well (although on a  much smaller length scale). For the ultrashort pulsed green  laser used in microPREPTM (wavelength: 532 nm), a typical  example of laser-micromachined silicon is depicted in Figure


2. In this case, the recrystallized layer is less than 400 nm thick  and no other indications of structural damage can be discerned. However, considering the melting temperature of silicon to be  1,410 °C, it is obvious that close to the recrystallized layer, the  substrate has seen elevated temperatures as well.


The thermal penetration depth, Lth, being dependent on the  pulse length τ and the thermal diffusivity of the laser-machined  substrate κ according to


results in a finite penetration of heat into the substrate during  on-time of the laser pulse. For ultrashort pulses, the thermal  penetration depth can be estimated to be clearly less than 500  nm (assuming a thermal diffusivity of 92·10-6 m²/s, [6]).


Therefore, suitable process conditions given, 10 µm apart from  the location of laser impact, there is no noteworthy  temperature increase to be expected.


Figure 2: TEM cross-section of the flanks of lasermicromachined silicon showing the extent of recrystallized  slabs to be limited to less than about 0.4 µm.


The example discussed above, however, is not the worst case  as a notch in a surface allows heat flow in a quarter space if  not a semi-infinite solid. Therefore, the pillars shown in Figure  3 were laser machined to have a look at structural damage to  their tips, where heat flow is much more limited along the  pillar axis. These structures by the way are geometrically very  close to what local electrode atom probe samples should look  like prior to sharpening them using FIB.


Figure 3: SEM micrograph of three pillars laser-machined  into silicon.


In order to assess the structural damage, the pillar experienced, a TEM lamella was prepared by standard Ga+ FIB from one of  the tips. As shown in Figure 4, in TEM micrographs recorded  in an FEI TITAN³ G2 80-300, the topmost end of the tip  contains a high density of higher-dimensional crystal defects. Figure 5 reveals that further down the pillar, the damaged layer


is not thicker than found in Figure 2, amounting no more than  a few 100 nm.


Figure 4: TEM overview of the tip end of one of the pillars  shown in Fig. 3 after preparation of a FIB lamella.


From the HRTEM micrograph depicted in Figure 6, it is  evident that below the damaged layer, the silicon is single  crystalline.


Figure 5: TEM close-up of the tips sidewall shown in Fig. 3.


As already mentioned, laser micromachining of pillars defines  a worst case scenario in terms of structural damage. The defect  densities of such structures cannot be found for typical TEMspecific geometries due to the much better heat flow and the  lack of beam overlap unavoidable when micromachining  structures smaller than the spot size of the laser beam. However, even in case of pillars prepared for local electrode  atom probe, the high defect density within the tip area might  be uncritical due do the fact, that more than 90% of the laserprepared structure have to be removed by FIB in order to meet  the specific geometrical requirements of the technique. Moreover, additional protective layers can be deposited on the  surface prior laser machining to place the heat effect zone  within.


Figure 6: HRTEM close-up of the tips sidewall.


Basic Workflow


The basic workflow detailed below was developed for bulk  samples. Beyond this, there will be extensions towards the  processing of cross-sections of IC structures, tomography and  atom-probe pillars, micromechanics test samples, etc.


The basic workflow consists of six steps:


1) Plane-parallel thinning to 100-150 µm


2) Assembling the plate on a flat mount


3) Laser cutting of the base structure


4) Transferring the base structure to a clamping jig


5) Local laser thinning of preselected areas (single- or both-sided), leaving a several micron thick bar


6) Final, single- or both-sided thinning with Ar+ ion beam (either using an focused or a broad ion beam)


In the final step, structural damage in the HAZ is removed  leaving an electron-transparent sample. This is achieved by  ion-beam thinning (either with a “broad” beam of about a  millimeter diameter or using a focused ion beam) a few micron  of the damaged material on either side, leaving an unaltered  sample volume for inspection.


Damaged layer


Single-crystalline silicon


Silicon pillar


In steps 3 and 5, one can make use of a huge variety of laser  trajectories. Regard the laser as a tool of about 12 µm diameter  that can cut out any imaginable structure, like those illustrated  in Figure 7. It is not just that you can design and cut a  supporting structure to exactly fit the needs for successive  characterization of the microstructure (like tips, bars, etc.), also the second step of the laser-based preparation (the  thinning of the supported structure) offers purpose-made  patterns.


The samples obtained are similar to H bar samples [7], but do  not necessarily have to be glued onto a half ring (due to being  self-supported) and can be much more than just one “H”. It  can be multiple “H”s, or other shapes.


Figure 7: Illustration a few selected basic structures that can  be machined with the laser. Besides circular TEM standard  samples, one can make any given geometry fitting into  standard samples holders. Beyond this, stabilizing bars and  marking for sample tracing are readily made.


Followed by ion-beam thinning, electron transparent sections  cannot just be made at one but multiple positions (illustration  in Figure 8), allowing for high-throughput screening of the  microstructure. This feature is particularly valuable for  gradient materials or if the homogeneity of a given  microstructure needs to become evaluated.


Figure 8: CAD sketch of a local thinning scheme used to  probe multiple positions in one sample in order to attain highthroughput screening of e.g. a series of through silicon vias.


Results & Discussion


Laser Micromachining of Silicon


In Figure 9, a supported bar (marked with figure “2”) is shown  after step 4 of the workflow, while in Figure 10, a scanningelectron micrograph of a tomographic basic structure is  depicted.


Figure 9: SEM micrograph of a supported-bar basic  structure laser-machined into silicon.


Figure 10: SEM micrograph of a tomographic basic  structure laser-machined into silicon in a standard SEM grid  holder.


In Figs. 11, 12, and 13, local thinning is demonstrated for the  supported-bar basic structure shown in Figure 5.


Figure 11: SEM micrograph of a H-bar basic structure in  silicon after local thinning in a box-like manner.


opening


Figure 12: SEM micrograph of a H-bar basic structure in  silicon after local thinning in a finger-like manner.


Figure 13: SEM micrograph of a H-bar basic structure in  silicon after local thinning in an open-box manner.


Laser Micromachining of Copper


In order to test laser-based cutting and thinning of copper, the  result shown in Figure 14 was achieved: a very smooth flank, free of curtaining.


Figure 14: SEM micrograph of a H-bar basic structure in  copper after local thinning in an open-box manner.


In the real world, it is not sufficient to be able to precisely  machine silicon or copper substrates. But the ability to  machine the aforementioned substrates individually is a  necessary precondition to machine heterogeneous systems. Therefore, we prepared a linear arrangement of copper-filled  through-silicon vias for inspection of the quality of their  fillings.


Laser Micromachining of Through Silicon Vias (TSVs)


In order to illustrate the high potential of laser based  preparation for failure diagnostics in microelectronic devices, TSVs (blind vias with 50 µm diameter and 150 µm depth) were prepared using the microPREP™ workflow and  investigated using transmission electron microscopy with  special emphasis on the interfaces formed between silicon, the  insulating layers, and copper. The samples under investigation  have been produced by deep reactive ion etching (DRIE) followed by subsequent thermal oxidation of the sidewalls and  silicon nitride deposition using a low stress LPCVD process. Prior to copper electroplating using Enthone’s MICROFAB  DVF200 chemistry, highly conformal copper seed layers were  deposited by MOCVD. In a last step, copper CMP was used to  remove the plating overburden and planarize the TSVs on the  front of the wafer. Annealing tests were conducted in order to  characterize the Cu TSV protrusion effect and related Cu  microstructure changes (samples were heat treated at 400°C  for 2 hours under N2 atmosphere.


As shown in Figure 15, a top view of the Cu-filled TSV  sample, local thinning along the TVS long axis can be  precisely controlled by optical means. Figure 16 shows a SEM  micrograph after both-sided laser thinning of all three TSVs, while in Figure 17, one of the latter is depicted in an SEM  micrograph after Plasma FIB thinning that may easily replace  broad-beam ion thinning.


Figure 15: Light-optical micrograph of a bar containing  three TSVs where one of them is already laser thinned from  one side.


Figure 16: SEM micrograph of a bar containing three TSV  structures thinned from both sides with the laser.


With standard (Ga+) FIB machining, one is (due to the  relatively low ablation rates) limited to more superficial areas, as shown in Figure 18. In this REM micrograph, the TSV  neighboring the one shown in Fig. 17 is depicted. Subsequent  TEM and STEM imaging (Figures 19, 20, and 21) confirmed  that the removal of about 7 microns from both sides fully  removes the thin layers containing structural damage due to the  laser micromachining.


TEM investigations reveal conformal adhesion between the  entire layer stack. Within the copper plug, small voids  randomly distributed over the electron transparent area have  been found, which is reasonable considering the mass transport  during annealing. Some of the grains are characterized by a  high defect density due to geometrical constrains during  recrystallization. The presence of these defects presents an  additional proof of the “athermal” ablation regime where  sample areas not directly exposed to the laser stay unaffected. Otherwise, heat-induced healing of lattice defects would have  been


apparent.


Figure 17: SEM micrograph of the laser-thinned, triple-H  bar containing TSV structures (Fig. 16) after PFIB  polishing.


Figure 18: SEM micrograph of the laser-thinned, triple-H  bar containing TSV structures (Figure 16) after Ga+FIB  polishing.


Figure 19: STEM micrograph of the Ga+FIB polishing TSV  contained in the laser-thinned, triple-H bar (Figure 16).


Figure 20: TEM montage of the Ga+FIB polishing TSV  contained in the laser-thinned, triple-H bar (Figure 16).


Figure 21: TEM close-up of the Ga+FIB polishing TSV  contained in the laser-thinned, triple-H bar (Figure 16).


Laser-based sample preparation is opening up new approaches  for fast, cost-effective, and site-specific preparation of samples  for TEM inspection and other microstructure diagnostic  techniques.


Using ultrashort laser pulses and employing appropriate  machining schemes, the extent of the very narrow, but omnipresent heat-affected zone can be limited such that final ionbeam thinning can readily remove any modified volume.


Dean Malta, RTI International, is gratefully acknowledged for  providing TSV samples. The authors are indebted to Dr. Christian Patzig for TEM imaging and Andrea Böbenroth for  her support during preparation.


[1] Th. Höche, PCT Patent Application WO 2013/026707 A1


[2] M. Krause and Th. Höche, EP Patent Application EP 13  16 2360.


[3] Th. Höche, D. Ruthe, and T. Petsch, "Femtosecond-Laser  Interaction with Mo/Si Multilayer Stack at Low Fluence," Appl. Phys. A, 79[4-6] (2004) 961-963.


[4] Th. Höche, D. Ruthe, F. Frost, and T. Petsch, “Nanostructural Investigations on Ripples Prepared by FemtoSecond Laser Treatment of Silicon,” Proc. 2nd  International Congress on Applications of Lasers & Electro Optics (ICALEO), Jacksonville, FL, October


[5] D. Ruthe, K. Zimmer, and Th. Höche, "Etching of  CuInSe2 Thin Films - Comparison of Femtosecond and  Picosecond Laser Ablation," Appl. Surf. Sci., 247 (2005) 447-452.


[6] S. Martens, M. Fink, W. Mack, F. Voelklein, J. Wilde, „Simulation-Based Analysis of the Heat-Affected Zone  during Target Preparation by Pulsed-Laser Ablation  through Stacked Silicon Dies in 3D Integrated System-inPackages,” 11th Int. Conf. on Thermal, Mechanical and  Multiphysics Simulation and Experiments in MicroElectronics and Micro-Systems, EuroSimE, 2010.


[7] L.A. Giannuzzi and F.A. Stevie, “A review of focused ion  beam milling techniques for TEM specimen preparation,” Micron, 30 (1999) 197-204.


Application of Fast Laser Deprocessing Techniques in Physical Failure Analysis  on SRAM Memory of Advance Technology


H.H. Yap, P.K. Tan, G.R.  Low, M.K. Dawood, H. Feng, Y.Z. Zhao, Y. Zhou, R. He, H. Tan,  Y.M. Huang, D.D. Wang, Y. Zhou, P.S. Limin, S. James, J. Lam, Z.H. Mai


Globalfoundries Singapore Pte. Ltd.


E-mail: HueiHao.YAP@globalfoundries.com, Tel: +65-66702905


With technology scaling of semiconductor devices and further  growth of the integrated circuit (IC) design and function  complexity, it is necessary to increase the number of  transistors in IC’s chip, layer stacks, and process steps. The  last few metal layers of Back End Of Line (BEOL) are usually  very thick metal lines (>4µm thickness) and protected with  hard Silicon Dioxide (SiO2) material that is formed from (TetraEthyl OrthoSilicate) TEOS as Inter-Metal Dielectric (IMD). In order to perform physical failure analysis (PFA) on  the logic or memory, the top thick metal layers must be  removed. It is time-consuming to deprocess those thick metal  and IMD layers using conventional PFA workflows. In this  paper, the Fast Laser Deprocessing Technique (FLDT) is  proposed to remove the BEOL thick and stubborn metal layers  for memory PFA. The proposed FLDT is a cost-effective and  quick way to deprocess a sample for defect identification in  PFA.


With continuous CMOS device dimension scaling, deprocessing Physical Failure Analysis (PFA) has become  more challenging and time consuming. In order to fulfill the  sophisticated circuit design and functions, it is necessary to  increase the number of transistors and layer stacks. Hence, layer by layer deprocessing for PFA is becoming increasingly  challenging and time consuming, especially to remove those  last few thick and stubborn metal layers of BEOL. E.g. the  delayering steps for 7 metal layers BEOL as follow:-


1. RIE to remove the passivation layer.


2. Immersed the die into the chemical to remove the metal 7, Aluminum layer.


3. Polished away the barrier layer with slurry.


4. RIE again to remove the TEOS layer and exposed the  metal 6, Cu layer.


5. Then polish with slurry to clear all the metal 6 and the  barrier layer.


6. Repeat the similar step 4 & 5 until the desired layer  exposed and only perform the SEM inspection.


Figure 1(a) & 1(b) show cross-sectional Scanning Electron  Microscope (SEM) images of a 28nm product chip (8 metal  layers) and 20nm (10 metal layers) test chip respectively. The  typical thickness of thick top metal layers is 4.0µm to 5.5µm. By using the conventional parallel lapping methodology, 1 to  2 hours will be required to remove the top thick metal layers


[1].


The Laser Deprocessing Technique (LDT) has been  introduced to 1) flatten unevenness issue of PFA and 2)


removed unwanted metal layers (especially top three layers) for Transmission Electron Microscopy (TEM) sample  preparation previously [2]. In this paper, we explore extending  LDT to remove the top five metal layers (apply LDT to expose  until V3/M3 layer) and ILD layers in memory such as Static  Random Access Memory (SRAM); therefore, the  deprocessing time for memory can be shortened. The  experimental SRAM PFA used in this paper is known as Fast  Laser Deprocess Technique (FLDT), whereby multiple laser  pulses are used to remove the top thick metal layers, so that  the SRAM PFA delayering time can be shortened from a  couple of hours to several minutes. FLDT is simple, cost-effective, quick, and provides uniform material removal  and surface evenness of an interest area. This technique is  especially important and useful for deprocessing of diced die  or packaged die.


Figure 1(a) Cross-sectional SEM images of a 28nm prototype  chip, and 1(b) Cross sectional SEM images of a 20nm  prototype chip.


1(a)


1(b)


FA Technique and Experiment


This experiment was performed on a 55nm (7 metal layers), 28nm (8 metal layers) & 20nm (10 metal layers) technology  node prototype chip that integrated SRAM. After the wafer  sort, a data log provides the GDS coordinate of the failing  bit/bits. Once verified and aligned the target, FLDT is then  performed at the failing location that is obtained from GDS  layout.


A laser marking system from New Wave Research model  Ezlaze3 was used in the experiment. The laser has a  wavelength of 532nm and was integrated into a model PM5  Cascade probe station. The laser pulse has a controllable  energy from 0 to 0.5mJ and fixed pulse width of 5ns.


In the previous paper, the effect of laser burst power upon a  number of layers deprocessed or removed is reported [2]. This  paper studies the relationship between how many layer is  removed as a function of the number of (constant power) laser  pulses. The laser energy used in this experiment is 0.5mJ with  a 20X objective lens and laser opening window size of  130µmx130µm. The following sequence describes a typical  FLDT workflow, as shown in Fig. 2:


1. Attempt to remove material that can be possibly removed  by chemical or Reactive Ion Etcher (RIE), such as solder  ball, polyimide etc. For example: die sample’s (cut out  from wafer) Polyimide can be removed by dipping into  Hydrofluoric Acid (HF), usually a 10s dip will be able to  separate polyimide layer from Passivation layer as shown  in Fig. 2.


2. Remove SiO2-based passivation layer (mainly SiO2 that  formed by TEOS) by RIE.


3. Top metal Aluminum (Al) layer can be removed by  Hydrochloric Acid (HCl). The result after chemical  removal is shown in Fig. 2(a). It is improper to remove  the Copper (Cu) metal layers by acid, because it will etch  the next layer Cu metal through the vias and cause  unevenness to the sample.


4. Apply FLDT laser burst, followed by slurry polish to  clean out debris arising from the laser blast. Where the  top metal layers had been remove by the laser blast.


5. Continues to delayer sample with slurry to the desire  inspection layer.


6. Layer by layer deprocessing with slurry to remove the  layer and RIE to expose next metal layer. Then perform  SEM inspection with conventional SEM Passive Voltage  Contrast (PVC) PFA technique [3-5] at the desire layer.


This basic workflow was applied to 7 metal layers (55nm), 8  metal layers (28nm) and 10 metal layers (20nm) prototype  chips in nanometer technology nodes respectively.


Figure 2 Schematic of the FLDT experiment steps.


Experiment Results and Discussion


Figure 3 shows SEM images of a 7 metal layers 55nm  prototype reference chip that was subjected to multiple laser  pulse bursts. Laser pulse burst of 4 pulses, 6 pulses, 8 pulses, and 10 pulses were used in this experiment. The results show  that with four laser pulse, it can controllably remove 2 top  thick Cu layer in total ~4.5µm plus 3 subsequent thin Cu  layers (~ 1µm) to the desired SRAM inspection V2 layer. The  subsequent laser blast (6, 8 & 10 laser bursts) will further  remove and reach Via1 (V1) or Metal 1 (M1) and below, which is past the target PFA inspection layer. The subsequent  laser blast is not as efficient as the first four blasts, because the  debris from the first four laser pulses block the subsequent  laser bursts from reaching the underlying layers. Another  reason could be due to the objective lenses focus point is at die  top layer (M7 barrier layer/M6). Hence the laser penetration  power is getting weaker and inconsistent once the objective  lenses working distance is getting further.


With the rapid development of semiconductor manufacturing  technologies, IC devices evolve to smaller feature sizes and  higher densities, and thus the task of performing successful  failure analysis (FA) is becoming increasingly difficult. Device  miniaturization often requires high spatial resolution fault  isolation and physical analysis [1]. To cater to the shrinking of  devices, extensive process improvements have been conducted  at the front-end-of-line (FEOL) structures. As a result, among  the numerous types of defects leading to chip failure, FEOL  defects are becoming more common for devices of advanced  tech nodes [2]. Therefore, it becomes more complexity and  difficulty on searching the physical defect.


Sample preparation is a key activity in material and failure  analysis. In order to image small structures or defects it is  often necessary to remove excess material or layers hiding the  feature of interest.


Removing selected layers to isolate a structure is called  delayering. It can be accomplished by chemical etching using  liquid or plasma chemistry, or by mechanical means, by  polishing off each unwanted layer.


This paper highlights the essence and importance of physical  deprocessing work that is particularly critical in resolving  some difficult yield problem in wafer fabrication. Without such  sample preparation skillset embodies in the FA analyst, purely  depending on advanced FA tools from fault localization and  AFP nanoprobing, will not be able to find the defect and  understand the true root cause behind.


Three case studies are discussed here with a different methods  and technique on how chemical/mechanical parallel polishing  or chemical etching can be applied to successfully identify  physical evidences on localized spacer defect on thin poly lines  and pinhole on Gate Oxide breakdown, floating gate failure in  EEPROM and FEOL defect with large LI interconnect  structure issue.


Case study 1: Gate oxide failure defect


Localized Spacer defect on ET structure with thin Poly  lines


A test wafer suffered from GOI Failure. Generally, there are  dummy metal lines on top of the structure as seen in Figure 1. From the spot seen from Front side EMMI/TIVA is difficult to  localize the exact failure site. Alternatively, backside  EMMI/TIVA approach can be adopted. However, it is still  extremely difficult for precise localization as fault localization  resolution is generally difficult to see which poly lines having  the problem. Thus, failure site localized indications such as  EMMI/TIVA have insufficient capability to provide such  precise position for physical analysis especially for small  defects.


Figure 1: Spot seen from Front side EMMI/TIVA is difficult  to localize the exact failure site


Instead, for solving this issue, perform TIVA/EMMI on full  processed wafer first. Subsequently, mechanical polish away  all the layers till M1 is still electrically intact. Subsequently, performing the TIVA/EMMI at M1 layer again, a precise  overlay with Metal1 lines to increase the success rate of  identifying defect. Once the defect is localized, further  deprocessing to poly layer (with presence of partial ILD) followed by high beam KV SEM inspection revealed spacer  anomaly at the poly lines. The anomaly has resulted in poly  shorted/leaked to S/D active (Fig 2).


Without a good physical sample methodology, the likelihood to  identify such small defect as current fault localization  resolution is many times larger than the defect size.


Figure 2: Precise spot on Metal 1 layer (upper) and high  beam SEM inspection revealed spacer anomaly at the poly  lines (Lower). The anomaly has resulted in poly  shorted/leaked to S/D active.


Is Gate oxide pinhole in bulk or at the edge of capacitor  structure?


Another Gate oxide sample preparation will be reviewed in  this paper also. In wafer fabrication, the exact location of the  gate oxide anomaly is particularly important to process  engineer. Example: Pinhole at bulk, it excludes possibility of  poly/spacer etch, gate oxide thinning at Edge/STI corner. In  this case study, fault localization by TIVA shows that the  defect is in the capacitor region. AFP current imaging found a  poly gate leak to substrate, suggesting the failure of gate oxide  breakdown issue. However, the exact location of the defect is  difficult to be determined by conventional physical analysis  with top down SEM. When the problem arises due to gate  oxide, punch through or pinhole can be determined by using  alternative sample preparation method as proposed. We used  mechanical parallel polishing to remove the ILD layer and  expose poly surface. Then, poly-Si gate was selectively etched  by chemical (e.g. mixture of HNO3, HF and H2O), as shown  in Figure 3. The location of gate oxide defect can be readily  inspected by SEM, as shown in Figure 4. This method enables  quick and accurate localization of gate oxide defects. The  location of the defect can assist the trouble-shooting of  equipment to find the root cause of gate oxide breakdown  failure.


Metal


Drain


Source


GOX defect


Well


Substrate


Delayer till poly


STI


Gate oxide


Pin hole defect


Figure 3:  A schematic view of sample preparation structure  for gate oxide defect localization.


Figure 4: AFP current imaging at contact level found leaky  poly contact in which pinhole defect was found at the edge of  gate.


Case study 2: Floating gate defect in EEPROM


Generally, for EEPROM, as seen in Fig 5, analyst normally is  able to identify the problematic node labeled A. However, if  the node is leaky, does it imply the cause is due to ONO or  tunnel oxide issue? Not an easy answer without a much  detailed electrical characterization.


However, the isolation of floating gate from adjacent  conductive layers results in difficulties in identifying possible  defects related to tunnel oxide, and thus many test  methodology and test algorithms have been studied to enable  the detection of tunnel oxide defects in an efficient manner. If  both bitmap location information and AFP nanoprobing  capability are available, it is possible to identify the tunnel  oxide failure by probing the failed memory bit and checking  any anomaly in its function. However, the functional test  requires accurate probing on the source, drain, select gate and  control gate as well as appropriate bias conditions. The  localization of the failed memory bit and appropriate contacts  for probing are time-consuming.


In this case study, initial failure analysis on the failed memory  bit by passive voltage contrast (PVC) and AFP current imaging  did not show any anomaly, and thus it is suspected that the  memory failure is caused by defects related to floating gate or  tunnel oxide. Mechanical parallel polishing was performed to  selectively remove the layers of control gate and ONO layer, as  shown in Fig 6. After the removal, the floating gate patterns  were exposed, enabling further analysis on the floating gates. As shown in the PVC analysis result of Figure 7, it was found  that the floating gate at the failed bit location showed  abnormal bright contrast. By this method, the identification of  whether it is ONO or tunnel oxide issue can be found in a  much easier way.


\


Figure 5: Leaky node seen at “A” of the EEPROM


Apply mixture of  HNO₃, HF & H₂O


Leaky poly contact


Figure 6: Mechanical parallel polishing was performed to  selectively remove the layers of control gate and ONO layer.


Figure 7: Leaky contrast seen at floating gate suggesting of  tunnel oxide issue.


Case study 3: Sample preparation in SRAM with  Local interconnect (LI)


Conventional de-processing of SRAM devices includes  removing metal and inter-metal dielectric (IMD) layers  followed by wet-etching by HF-based chemicals to expose poly  and active-Si layer. However, it is difficult to locate and  inspect FEOL defects for SRAM devices with localinterconnect (LI) layer. The LI layer is essential for decreasing  of overall size of SRAM devices. It is under the first metal  layer and provides electrical paths to which gate may be  electrically connected to other portions of the SRAM device  without the need of multiple interconnect. Typical LI layers are  made of tungsten which is inert to common wet etchants used  in de-processing. As a result, LI layers remain on the sample  after poly and active layers are exposed by HF-based wetetchant, as shown in Figure 8(a). Due to the large size of LI  layers, it is highly possible that FEOL defects are blocked by  LI layers, making the subsequent defect inspection difficult.


In this case study, failure analysis was done on a single bit  failure of SRAM with local-interconnect (LI) layer. After the  sample was de-processed to contact/LI layer, AFP nanoprobing  analysis found symptoms of LI short to LI and LI short to  active. However, the exact location of the defect and what the  defect causing the failure is still unclear.


Wet etching by H2O2 was done to selectively remove the LI  layer and expose the structure beneath the LI layers. Surface  SEM inspection found poly-Si residues which cause the short, as shown in Figure 8(b) which clearly found after the LI  removal.


Figure 8(a): SEM pictures of SRAM with LI layers after poly  and active are exposed. The LI patterns blocking possible  defects beneath.


Figure 8(b) After the LI patterns were removed, poly residue  defects were found.


Sample preparation in failure analysis is a very importance  analysis step which helps us to identify the physical defect for  further root cause and mechanism understanding of the issue. Throughout the 3 FEOL case studies presented in this paper, we have clearly demonstrated how the causes of these failures  are being identified through a good sample preparation  methodology. Without a good physical sample methodology, the likelihood to identify small FEOL defects such as spacer  defect, gate oxide pinhole and poly residue underneath the  local interconnect will be extremely low.


[1] K. Li, P. Liu, J. Teong, M. Lee*, and H. L. Yap*, “A  Logical Problem Solving Process for High Via Resistance  Root Cause Analysis”, ISTFA 2008, pp.70-74.


[2] S. Chen, L. Li, A. Du, Y. N. Hua, “Study of Si crystal  defects by chemical preferential etching and its application  on Si dislocation defects caused by Laser Spike Annealing (LSA)”,  ISTFA 2012, pp.293-296.


Site-Specific, Wide Field-of-View Cross-Sectional Sample Preparation, Imaging  and Analysis in a Plasma Ion Source Helios DualBeam™ Microscope


Roger Alvis, Ron Kelley


FEI Company, Hillsboro, Oregon USA  roger.alvis@fei.com


A Plasma-source focused ion beam (Helios PFIB) DualBeam™ microscope with sub-nanometer 1kV SEM  resolution was used to investigate the structure of a state-ofthe-art organic light-emitting diode (OLED) display. The  capability of the Helios PFIB to produce and manipulate  millimeter-scale samples for wide field-of-view crosssectional SEM analyses was demonstrated by lifting out a  570µm long by 40µm wide x 10µm deep and mounting it on a  copper half-grid. An angled face was cut into the chunk and  high-resolution back-scattered SEM tiles across the entire  exposed face were automatically acquired within a modular  automated processing system (MAPS).


Historically, shrinking transistor technologies have pushed  electron microscopes to ever higher imaging performance in  terms of resolution and magnification ranges. Cross-sectional  Scanning Electron Microscopy (SEM) of densely packed, small geometry devices demands that a microscope provides  high surface sensitivity and high spatial resolution [1-3]. At  low-kV, secondary and back-scattered electron signals are  obtained from the near-surface region [4].  Minimizing  chromatic aberration enables extremely high-resolution  imaging at relatively low landing energies (“XHR-SEM” conditions), as evidenced by a 1kV SEM image of a 22nm  finFET sample shown in figure 1. To meet the demands of  site-specific sample preparation and analysis applications, the  combination of a monochromated field-emission gun (FEG) and a gallium focused ion beam (Ga-FIB) in a DualBeam™ microscope enables FIB-exposed structures to be imaged with  sub-nanometer resolution. For site-specific sample preparation  of XHR SEM, or even TEM samples, a typical FIB cut  dimensions is on the order of 10-20 micrometers wide and 5-10 micrometers deep [5,6].


Relatively recently, the advancement of multi-chip packaging  structures such as through-silicon-vias (TSV) and interposers, has pushed FIB to support site-specific sample prep of features  of tens-to-hundreds of microns in size which may be buried  under hundreds of microns of substrate or packaging material


[7]. To support this application space, a plasma-based FIB (PFIB) source was developed, providing imaging currents as  low as 1.5pA and milling current greater than 1µA [8]. Figure  2 shows an example of a package-level cross-section enabled  by a PFIB. The 270µm x 330µm cross-section was made in  less than 2 hours by bulk milling with 1.3µA beam current and  final polishing with 470nA.


Figure 1: 3kV XHR SEM view of a commercially available  22nm finFET inverter from an SRAM array.


Figure 2: PFIB images of a package-level structure,  333µm field-of-view overview image (left) showing bondpad, TSV, and inter-die micro-bumps, and a 118µm fieldof-view zoomed-in image (right) showing the structure of  the micro-bumps


As the traditional lines between packaging (back-end) interlayer metallization, and (front-end) devices blur, a new  application space is emerging for simultaneous site-specific, large area cross-section sample prep and XHR-SEM imaging. Besides cross-section imaging and analyses, wide-field-ofview (WFOV) application space includes package-level and  die-level circuit editing, as well as delayering for fault  isolation-to-physical failure analysis workflows [9]. Within  this WFOV application space, requirements for SEM  resolution and acuity for imaging and analysis of active  microstructures remain practically unchanged from those of  conventional field-of-view analyses.  To this end, the 20X  increased milling rate of a plasma-source FIB (PFIB) combined with a monochromated SEM column offers a  promising solution to the emerging demand for WFOV XHR  SEM imaging and analysis [10].


An interesting example of the challenges inherent in WFOV  sample preparation is found in mobile displays. Like  semiconductor structures, liquid crystal displays and organic  light-emitting diode displays (LCD and OLED, respectively), are made up of elements from across the periodic table, incorporating both extremely hard materials (molybdenum and  titanium nitride, for example) and extremely soft materials (silver alloys, for example) [11, 12]. SEM analyses of this  class of structure are further complicated by the use of glass (or plastic) substrates, organic interlayers, and integral touch  screens.


The construction of a typical display device [13, 14] suggests  that the volume of material that would need to be removed by  FIB in order to explore display structures could place  extraordinary demands on a gallium FIB sample preparation in  terms of instrument loading, depending on the purpose of the  analysis.  While it is feasible that a single FIB cut a couple of  tens of micrometers wide and as small as five micrometers  deep could satisfy the requirements of a basic cross-section  image of a thin-film transistor (TFT), a cut through across the  entire length of a single-color pixel, (so-called “sub-pixel”) might require a FIB cut greater than 50 micrometers and as  deep as 15micrometers. Further, a FIB cut through the full  extent of a red-green-blue (RGB) pixel’s TFT array could be  over one hundred micrometers in length [15]. A failure  analysis or reverse-engineering analysis of an entire RGBpixel TFT array with sequential milling and imaging (120µm  in X by 120µm in Y by 15µm in Z, with 25-50nm slices for  example) could take several tens of hours, to even days on a  Ga-FIB.


In this paper, we explore a WFOV application of reverseengineering and structure analysis of a TFT circuit found in a  commercially available OLED display. Our approach is to  extract a 3D portion of the layout and layers by using the  plasma FIB to prepare a long sample (<800um) for XHR-SEM  and to demonstrate the ability to thin a specific area to electron  transparency for STEM imaging and EDS analysis.


Experimental Methodology and  Discussion of Results


AMOLED Sample Details


A Samsung Galaxy S4 mobile phone (model number SGHI337) was purchased on the internet. The Galaxy S4 display  features an Full-HD compatible (1080p) active-matrix organic  light emitting diode (AM-OLED) display specifies a  1920×1080 pixel count on a 5-inch display (440 pixels/inch) [16, 17]. Samsung Display Company arranged the green pixels  on a square grid, with alternating red and blue positioned in  the center of each green sub-pixel square (figure 3), resulting  in 58micrometer RGB pixels.


Figure 3: Samsung Display Company marketing image of  the Samsung Galaxy S4 OLED display. Blue and red subpixels are laid out on diagonal lines, alternating positions  with green sub-pixels, giving the appearance of diamond  shaped pixels (adapted from ref 17).


The S4 was disassembled and after being separated from the  touchscreen, the display was cracked and a small piece of the  display was separated from the display assembly (figure 4).


Figure 4: Samsung Galaxy S4 disassembled, with the  OLED display separated from touch screen. A sample of  the display is being held by tweezers.


With the display sample on a glass slide, bright field reflected  and transmitted optical images of the S4 display were captured  from a clean portion of the display using a 50X MPlan FLN  objective lens on an Olympus BX51 inverted microscope (figures 5a and 5b).


Figure 5a, b: Optical micrographs of the Samsung Galaxy  S4 display, showing an area equivalent to that in figure 3, a) reflected light view and b) transmitted light view. Black (opaque) regions in b) reveal AMOLED metallization  layers, while light pink regions are inter-layer dielectrics  and dark pink lines correspond to TFT active layers.


Sub-Pixel Sample Preparation


After capturing optical images, a specimen from the display  was mounted on a standard SEM stub and was coated with  approximately 100nm of evaporated carbon (Cressington  Carbon Cater, Model 208 Carbon, 155A, approximately 60s) as a precaution against damaging the top layer(s) of the S4


display during the initial exposure to FIB processing. To  enable the orientation of the SEM images to match that of the  previously acquired optical microscope images, the sample  was imaged with the Everhart-Thornley detector (ETD) at 20  and 30kV in an FEI Helios Plasma FIB DualBeam™ microscope to reveal the subsurface metal power lines and the  sub-pixel anode layer (figures 6a and 6b) [18].


Figure 6a, b: 20kV and 30kV SEM (ETD) images of the  carbon-coated OLED display surface revealing sub-pixel  features at the surface, and sub-surface metal lines. The “+” corresponds to an intersection of opaque and  translucent features, suspected to be the TFT gate  controlling the power to the adjacent blue sub-pixel.


A)


B)


The intersection of an opaque line and a translucent line  visible in both the transmitted light optical micrographs (marked with an “+”) adjacent to the contact is suspected to be  the transistor that controls the power to the pixel (brightness  level). This feature and surrounding structures in a green subpixel were targeted for detailed XHR-SEM analysis.


Analysis of TFT Layout


Volume analyses of the TFT circuitry and low-kV STEM  analyses were done using a Helios PFIB [19]. A 900  micrometer long by 105 micrometer wide by nominally two  micron deep ion beam platinum and carbon films were  deposited across a span of 15 green sub-pixels (at 180nA, approximately 50 minutes in total). Trenches were cut on  either side of the chunk at -8° stage tilt using a 1.3µA with  880µm x 40µm rectangular milling pattern to undercut the  region of interest, approximately 70 micrometers of substrate  was removed on each side (1.3µA, approximately 300 minutes  total). Figure 7 shows top down and oblique views of the  cantilevered chunk. Large curtains, typical of high-current  milling on glass materials, are evident in the end-on view of  the chunk.


Figure 7a, b: SEM (ETD) overviews of the region of  interest a) top-down and b) tilted and viewed end-on, after  chunking in the Helios PFIB DualBeam™ microscope.


The chunk was lifted out from the substrate, inverted, and  mounted to a standard TEM half-grid [20] for further sample  preparation and imaging. Immediately prior to mounting while  the chunk was still attached to the EZ Lift micro-manipulator,


Figure 8a-c: Overview and detailed images of the lift-out  and attach process, a) EX Lift needle and platinum GIS  inserted before lifting out (SEM ETD), b) inverted chunk  attached to the TEM half-grid (SEM ETD), and c) detailed  view of the ion beam Pt attach to the grid (PFIB ICE).


C)


needle, two of the four posts on the grid were milled away in  the Helios PFIB using a 1.3µA cleaning cross-section pattern (approximately 10 minutes per post). Figures 8a-c show  selected SEM (ETD) and PFIB images of the lift-out and  attach process.


After the wedge-shaped chunk was securely attached to the  grid on both ends, additional ion beam platinum was deposited  on the substrate-side of the chunk (top of the now-inverted  sample).  The edge of the sample was cut (at 52° stage tilt) with cleaning cross-section (CCS) patterns placed on the far  sides of both ends of the sample to set a nominally neutral  milling angle for subsequent angled milling into the ROI (figure 9). Identical structures at each end of the chunk were  exposed to optimize milling for subsequent imaging of the  green sub-pixel across the entire face of the ~900µm chunk.


Figure 9: ROI cut strategy overlaid on the top-down view  of the chunk (from figure 6a). Two CCS cuts, ~12µm from  the first edge (green overlay)--one at each end of the  sample, into a distinct feature in the green sub-pixels TFT  circuitry, are to be made to determine the neutral milling  angle. A subsequent angled CCS cut across the entire  chunk (1.3°, red overlay) will expose the AMOLED TFT  structure around one of the green OLED contacts.


The face of the sample was prepared for SEM imaging with a  CCS pattern (775µm (X) by 12 µm (Y) by 10µm deep with  180nA at 30kV. After the face was prepared sample was  removed from the specimen preparation stage and re-oriented  for imaging normal to the cut face. The imaging conditions  were optimized for XHR-SEM (BSE) imaging (2kV and  100pA at 3mm WD).


The correlative microscopy software package MAPS [21] was  used to automatically step the stage, capture and stitch a total  of 38 images (6k pixel resolution at 10% overlap) to create a  high resolution montage image of the cross-sectioned face. The montage of the tapered cut was saved in a pyramid data  structure [22] through the circuit was imported into the  Microsoft HD View Internet Explorer plug-in [23]. The  structure of the OLED TFT array was explored by panning  through the data set and screenshots at different levels of  zoom were exported from HD View (figures 10a-e).  Figure  10a is a low-resolution (down-sampled) overview of the entire  extent of the 773µm MAPS data set. Detailed images from the  left, center, and right of the prepared face were exported from  HD view (indicated in figure 10a by the dashed circles labeled  detail 1, detail 2a, and detail 3, respectively). Detail 2b is an  even higher magnification image attained by zooming further  into the detail 2a HD dataset. The location of detail 2b is


indicated in detail 2a by the dashed-line circle in the upperright of the image (figure 10c).


Detail 1 (from the leftmost part of the MAPS overview) shows  the intersection of a metal line section passing over a long  semiconducting layer, most likely part of a transistor structure. Detail 2a shows a more complex patterned structure consisting  of two short metal line sections, a second conducting line  contacting the left part of a semiconducting line and  connecting to the bottom of the long bright line that extends  across the entire field of view. This detail captures the  AMOLED array at the thinnest part of the stack, the lightemitting portion of the green sub-pixel. Detail 2b shows the  green OLED stack sandwiched between the continuous anode  line and the cathode layer that appears to consist of discreet  nano-particles, rather than a continuous layer. In each of the  metallization layers, crystallographic contrast in the BSE  signal is evident. Dark contrast in the layer(s) above the TFA  array is likely organic filler material.


Figure 10a-e: 2kV TLD-BSE images, showing an ultra-low  magnification overview and detailed images extracted  from the b) left, c) center, and e) right region of the  770x35µm MAPS dataset.  The microstructures of the  various AMOLED conductive and insulating layers, as  well as TFT devices are clearly revealed. The OLED  cathode (top layer, detail B2) appears to be made up  entirely of discreet nano-particles, as seen in figure 10d.


A Plasma-source focused ion beam DualBeam™ (Helios  PFIB) microscope with sub-nanometer 1kV SEM resolution  was used to investigate the structure of a state-of-the-art  organic light-emitting diode display. The capability of the  Helios PFIB to produce and manipulate millimeter-scale  samples for wide field-of-view cross-sectional SEM analyses  was demonstrated by lifting out an 800µm long by 100µm  wide x 50µm deep sample and mounting it on a copper halfgrid. An angled face was cut into the chunk and highresolution 2kV SEM (TLD-BSE) images across the entire  exposed face were automatically acquired, tiled, and stitched  within the MAPS imaging environment. Using MAPS data  throughout the available magnification range, detailed analysis  of the thin-film transistor construction was straightforward, with distinct microstructures revealed in the conducting, semiconducting, and insulating layers comprising the active matrix  circuitry driving the display. The angled cross-section  technique applied to the wide filed-of-view methodology  made possible with the Helios PFIB, hold promise for  tomography


The authors would like to thank Trevan Landin and Allen  Hunter (FEI Hillsboro NanoPort), Anthony Burgess and David  Donnet (FEI Acht NanoPort), Suri Madala (FEI Product  Marketing) and Kenny Mani (FEI Product Development) for  their kind and diligent support of this project.


[1] http://download.intel.com/newsroom/kits/22nm/pdfs/22


nm-details_presentation.pdf (accessed 2014-0721)


[2] L. Y. Roussel, D. J. Stokes, I. Gestmann, M. Darus, R. J. Young, Extreme high resolution scanning electron  microscopy (XHR SEM) and beyond, Proc. SPIE 7378, pp. 73780W, 2009.   doi:10.1117/12.821826


[3] Ugurlu, O., et al, High-volume process monitoring of  FEOL 22nm FinFET structures using an automated  STEM, Proc. SPIE 8681, Metrology, Inspection, and  Process Control for Microlithography XXVII, 868107 (18 April 2013); doi:10.1117/12.2011594


Passive Voltage Contrast for Failure Localization”, ISTFA


2007, Proceeding, pp. 331-336.


[5] P.K. Tan, Z.H. Mai, Y.W. Goh, L. Zhu, S.L. Toh, Q. Deng,


R. He, H. Tan,H.L. Li, Q.F. Wang, Y.Z. Ma, W.Y. Lee,


G.R. Low, Jeffrey Lam, “Fault Isolation on High


Resistance Failure of 45nm ET Via Chains Using


Combined Technique of SEM PVC and Nanoprobing”,


ISTFA 2010, Proceeding, 239-242.


ex situ Lift Out of Plasma Focused Ion Beam Prepared Site Specific Specimens


Lisa Chan and Jon M. Hiller


Tescan USA, 508 Thomson Park Dr., Cranberry Township, PA 16066


Lucille A. Giannuzzi


EXpressLO LLC, 5483 Lee St, Unit 12, Lehigh Acres, FL 33971


ex situ lift out (EXLO) was historically the first lift out  technique to be developed for site specific removal and  manipulation of focused ion beam (FIB) prepared specimens  to a suitable carrier [1].  Early publications simply refer to this  technique as “lift out” since further specification was not  necessary.  EXLO was later coined to distinguish it from lift  out methods performed inside the FIB instrument.


EXLO is performed outside of the FIB instrument on a unit  basically consisting of a light optical microscope and  manipulator.The specimen is usually picked from within the  FIB trenches with adhesion forces using a glass probe  manipulator.  For scanning/transmission electron microscope (S/TEM) characterization, the specimen is then placed on a  thin film coated TEM grid [1].  The lift out and manipulation  process takes only a couple of minutes [2].  Known  advantages to EXLO include ease of use, high throughput and  high > 90% success rates [2].


Recently developed methods negate the need for a thin film  coated TEM grid [3-8].  A slotted half grid allows specimens  to be manipulated to the grid itself.  This allows for a better  heat sink and electrical path to ground.  Since a carbon film  may inhibit certain S/TEM techniques such as energy filtered  imaging, electron energy loss spectroscopy or electron  holography, the absence of this thin film allows all S/TEM  techniques to be performed.  More importantly, since no thin  film support is needed, the specimen can be further processed  after manipulation.  In addition, a thick specimen can be easily  manipulated to the slotted grid into a backside orientation, and  then FIB milled to a suitable thickness for S/TEM without  producing curtaining artifacts [4,8].


EXLO was developed in the age of Ga+ FIB columns with ~ 50 nm beam sizes.  The modern Xe+ plasma FIB (PFIB) column operates at about this same 50 nm beam resolution or  better.  Therefore, it is no surprise that the Xe+ PFIB is  capable of preparing electron transparent specimens for  S/TEM [9].  In addition, the PFIB offers inert or other ions of  choice for specific applications.  Since the PFIB can operate at  much higher beam currents (with a smaller probe size) than a  Ga+ FIB, the PFIB’s strength is large volume material removal [10,11], which can be exploited for TEM EXpressLO methods


[12].  The requirement of producing large lift out specimens  increases the FIB time dramatically [13].  For example, it took ~ 4 hours to prepare > 100 m long TEM specimens prepared


via in situ lift out via Ga+ FIB [14].  Thus, in this paper, we  combine fast PFIB preparation of large S/TEM specimens  with fast conventional EXLO and EXpressLO “pick and  place” solutions.  The combination of large material removal  rates with PFIB and EXLO allows for efficiency and high  throughput of FIB lift out specimens.


Experimental Methods


Specimens from a patterned Si wafer were prepared for EXLO  and EXpressLO using a Tescan FERA3 Xe+ PFIB operating at  30 keV.  PFIB W deposition marked the region of interest.  Each large specimen measured 40 m x 15 m x 1 m and  was prepared in well under 30 minutes using successively  smaller beam currents of 100 nA, 30 nA, and 10 nA.  An  example of a final PFIB prepared specimen is shown in the  scanning electron microscope (SEM) image in figure 1.  Lift  out success rates improve dramatically when the specimen is  completely FIB milled free (or nearly free as in figure 1).  EXLO and EXpressLO examples were performed on an  EXpressLO LLC lift out station as shown below in figures 2  and 3.


Figure 1: SEM image of PFIB prepared specimen.


Figure 2: Sequence of EXLO steps for a PFIB prepared


specimen from lift out to manipulation to a formvar coated  Cu TEM grid. The PFIB specimen length is 40 m.


Figure 3: Pick&Place sequence of EXpressLO steps for a  PFIB prepared specimen from lift out and manipulation to a  slotted Cu TEM grid [8]. The PFIB specimen is 40 m long.


Conventional EXLO


Figure 2 shows a sequence of images during the EXLO of a  PFIB specimen and manipulation to a formvar coated Cu  TEM grid.  The time stamp from the video acquisition is noted  on each image.  As shown, the entire process takes just over a  couple of minutes.  Figure 2a shows the PFIB specimen  secured on the probe tip in under 10 s.  Figure 2b shows a low  magnification image of the specimen attached to the probe tip. In figure 2c the grid has been centered and the specimen has  been lowered close to the desired grid square.  In figure 2d, the probe tip gently touches the top of the specimen, to ensure  it is flat and secure.  The probe tip is raised and the specimen  transfer is completed in figure 2e in just over 2 minutes.


EXpressLO Pick&Place


Figure 3 shows a sequence of images during EXpressLO of a  PFIB specimen and manipulation to a slotted Cu TEM grid.  The time stamp from the video acquisition in figure 3 shows  the elapsed time after the specimen has been picked out of the  trench.  As shown above, the specimen “pick” generally takes ~ 10s if the specimen is completely FIB milled free.  The  entire “place” process to the slotted grid after the specimen “pick” in figure 3 takes just under 3 minutes.


Figure 3a shows the PFIB specimen positioned on top of the  probe tip and just above the EXpressLO Cu grid.  If the “pick” does not result in this preferred orientation of the specimen for  the EXpressLO process, the probe can be easily rotated to  orient the specimen on top of the probe.  Figure 3b shows the  specimen and grid close to the same focal plane.  When the  probe and grid both start to appear in focus as in figure 3b, the  probe is very close to the grid surface.  At this point, the probe  with the specimen is centered over the slot opening in the  EXpressLO grid.  In figure 3c the probe is lowered and  manipulated through the slot opening such that the specimen  comes to rest and is “placed” on the grid support structure.  The probe then gently touches the specimen to ensure it is flat  and secured to the grid (figure 3d).  After correct placement, the specimen reflects brightly in the light optical image as per  figure 3d.  The probe is raised and the specimen “place” is  finished completing the “Pick&Place” procedure as per figure  3e.


Figure 4 shows an SEM image of the specimen placed on the  EXpressLO grid after ion beam assisted W deposition (indicated by the arrow) was used to further secure one side of  the specimen.  Certainly, this W deposition step is not needed  for careful handling as the adhesion forces are sufficiently  large to successfully transfer the specimen attached to the grid  from the lift out station in ambient conditions into the  FIB/SEM vacuum (figure 4).  Indeed, electron transparent  specimens manipulated to an EXpressLO grid have been  transferred directly to a TEM for analysis (without further  deposition to secure the specimen) [3].  This added W  deposition is performed as a precautionary measure to secure  the specimen during further FIB milling.  At this point, it is


not known if this added W deposition step is absolutely  necessary prior to further FIB milling, however, the added  time required for the W deposition step is minimal compared  to the alternative scenario of having to re-FIB mill another lift  out specimen.


Figure 4: SEM image of the Pick&Place specimen. The  arrow indicates PFIB deposited W.


At this point the specimen in figure 4 can be directly analyzed  via SEM or other technique.  In addition, this specimen can be  further thinned to electron transparency for S/TEM via  standard Ga+ FIB methods or via Xe+ PFIB methods [9,13].  Indeed, very large > 100 m specimens have been prepared  via in situ lift out and thinned to electron transparency via Ga+ FIB, albeit at times ~ 4 hours [14].  More recently, very large > 100 m specimens were thinned to electron transparency via  Xe+ PFIB [13].  Thus, once a specimen is manipulated to a  suitable grid as in figure 4, thinning to electron transparency is  routine via established methods described above.


Large (40 m) PFIB prepared site specific specimens were  milled, lifted out (“picked”) and manipulated (“placed”) quickly for direct characterization using EXLO.  With  conventional EXLO, thick or electron transparent specimens  can be picked and placed on thin film coated grids or other  appropriate supports for either S/TEM or other  characterization.  Pick&Place of specimens directly to  EXpressLO grids enable further FIB or other processing prior  to S/TEM or alternative technique.  The combination of PFIB  milling and EXLO increases throughput for specimen  preparation.


[1] L.A. Giannuzzi et al., “Focused Ion Beam Milling and  Micromanipulation Lift-Out for Site Specific CrossSection TEM Specimen Preparation,” Mat. Res. Soc. Symp. Proc. Vol. 480 (1997), MRS, pp. 19-27.


[2]  L.A. Giannuzzi and F.A. Stevie (eds.) Introduction to  Focused Ion Beams, Springer (New York 2005) pp. 201-228.


[3]  L.A. Giannuzzi, “EXpressLO™ for Fast and Versatile  FIB Specimen Preparation,” Microsc. Microanal. Vol. 18, S2 (2012) pp. 632-633.


[4]  L.A. Giannuzzi, “Routine Backside FIB Milling With  EXpressLO™,” Proc. ISTFA  (2012)  pp. 388.


[5] L.A. Giannuzzi, “Enhancing Ex-Situ Lift-Out with  EXpressLO,” Microsc. Microanal. Vol. 19, S2 (2013) pp. 906-907.


[6]  N. Bassim, K. Scott, and L.A. Giannuzzi, “Recent  advances in focused ion beam technology and  applications,” MRS Bulletin Vol. 39, No. 04 (2014) pp  317-325.


[7]  F.A. Stevie and L.A. Giannuzzi, “FIB Applications: A  Historical Perspective,” to be published, Microsc. Microanal. Vol. 20, S2, (2014)


[8] Lucille A. Giannuzzi, U.S. Patents 8,740,209 and  8,789,826.


[9] L. Giannuzzi and N. Smith, “TEM Specimen  Preparation with Plasma FIB Xe+ Ions,” Microsc. Microanal. Vol. 17, S2, (2011) pp 646-647.


[10]  N.S. Smith, W. P. Skoczylas, S. M. Kellogg, D. E. Kinion, P. P. Tesch, O. Sutherland, A. Aanesland and  R. W. Boswell, “High brightness inductively coupled  plasma source for high current focused ion beam  applications,” J. Vac. Sci. Technol. B Vol. 24, No. 6, (2006) pp. 2902-2906.


[11] Paul Tesch, Noel Smith, Noel Martin, Doug Kinion, Proc. ISTFA, (2008) pp.7-13.


[12] Lucille A. Giannuzzi and Noel S. Smith, “ex situ lift  out of PFIB prepared TEM Specimens,” to be  published Microsc. Microanal. Vol. 20, S2, (2014).


[13]  A Delobbe, O Salord, P Sudraud, T Hrncir, F Lopour, and A David, “High Speed TEM Sample Preparation  by Xe FIB,” to be published, Microsc. Microanal, Vol. 20, S2, (2014).


[14] S.M. Schwarz, B.W. Kempshall, L.A. Giannuzzi, “Effects of diffusion induced recrystallization on  volume diffusion in the copper-nickel system,” Acta  Materialia Vol. 51 (2003) pp. 2765–2776.


Using Energy Dispersive Spectroscopy (EDS) to Determine the   Resistance of FIB Jumpers for Circuit Edit


Michael DiBattista and Corey Senowitz


Qualcomm Incorporated, San Diego, California  92121, USA   mdibatti@qti.qualcomm.com


Hasan Faraby1and Prabhakar Bandaru2


### Using Energy Dispersive Spectroscopy (EDS) to Determine the Resistance of FIB Jumpers for Circuit Edit


1Department of Electrical and Computer Engineering, University of California, San Diego, La Jolla, California  92093, USA  2Department of Mechanical Engineering, Materials Science Program, University of California, San Diego, La Jolla,


California  92093, USA


A key capability of focused ion beam (FIB) tools is the ability  to deposit conductive materials by introducing organometallic  precursors such as tungsten hexacarbonyl [W(CO)6] or (methylcyclopentadienl)trimethyl platinum [C9H17Pt].  The  FIB deposited metal is often used in applications such as the  modification of integrated circuits (ICs) by creating new  electrical connection on the device.  The electrical properties  of the FIB material are of particular concern to high speed  digital and radio frequency (RF) circuit designers because the  resistivity of the FIB deposited metal is orders of magnitude  higher in value than the near bulk resistivity value of the  metals used in IC manufacturing.  In this paper, we developed  a correlation between the chemical composition of the FIB  deposited metal and the electrical resistivity using an effective  media theory (EMT) model.  Analysis shows that gallium  from the ion beam is the dominant contributor to lowering the  resistivity of the jumper.  The results of this work and model  allow us to understand the role the chemical elements play in  the electrical resistance of the FIB electrical jumper and to  estimate the FIB metal resistance from energy dispersive  spectroscopy (EDS) analysis and the geometry.


FIB Metal Deposition


A significant range of chemistries can be employed to deposit  conductive materials using either an electron or ion beam.  Published examples include gold [1,2], copper [3,4], cobalt


[5], tungsten [6-8] and platinum [9-10]. In the analysis of  semiconductor processing for yield enhancement and design  debug, FIB deposited tungsten and platinum are the two most  common materials deposited for sample cross sectioning, transmission electron microscopy (TEM) sample preparation, and circuit modification (circuit edit).  Circuit edit  traditionally has relied on ion beam deposition of material  over the electron beam because a lower resistance material has  been consistently achieved with organic precursors.[11]


Circuit edit on semiconductor devices faces unique challenges  with FIB deposited metals because the resistivity values of the


deposited material are orders of magnitude higher than the  metal interconnect layers of the device.  This is a particular  concern to VLSI designers of high speed digital circuits and  RF designers.  These circuit edit requests are of significant  importance to the overall performance of the device, and  therefore particularly important use cases for the failure  analysis laboratory.


FIB tungsten from tungsten hexacarbonyl falls in the range of  180-250 -cm [12] and FIB platinum mainly from (methylcyclopentadienl)trimethyl platinum generally has a  higher resistivity in the range of 400-1000 -cm [13] in  published literature. FIB deposited materials have been used  for more than 10 years to successfully modify circuits and  semiconductor devices [14-16], but the reasons why the FIB  deposited materials have such high resistivity is still unknown  even though the values of the electrical properties of platinum  and tungsten have been published and are very reproducible  across the industry.  The presence of carbon from the organic  precursors act as an insulator or contaminate has often been  mentioned as the most likely cause [17], but even with this  material present, the resistance values are often too high for  FIB depositions with sixty atomic percent metal.


Effective Media Theory (EMT)


We have formulated a model to understand and predict the  overall resistivity of FIB deposited materials using effective  media theory. EMT is a well developed field that has been  used to understand and predict the electrical, optical, and  mechanical properties of complex materials such as resistivity


[18], index of refraction [19], and bulk modulus [20].


Figure 1.   A conceptual model of a complex material composed of  different constituents with different properties can be modeled as a  single material with aggregate properties of the matrix.


As shown in Figure 1, EMT uses the properties of the  individual constituents of the material such as each of the  component’s known resistivity values to create an effective  medium with an electrical resistivity that is based on the  ensemble of the individual components. For this work, the  theoretical resistivity of the FIB deposited materials were  estimated through McLachlan’s [21-23] general effective  medium (GEM) based formulations [24]. For this model  implementation, we made assumptions that the FIB material  was mixture of only two components - a low resistivity (lo) component and a high resistivity (hi) component.


φ [(  m)1t -(  lo)1t ](  m)


t + [1-φcφc] (  lo)1t+


(1-φ) [(  m)1t -(  hi)1t ](  m)


t + [1-φcφc] (  hi)1t=0


lo= resistivity of the low resisitivity component (ohm-cm) hi= resistivity of the high resistivity component (ohm-cm) m= resistivity of the medium (ohm-cm)


= atomic percentage of the low resistivity component c= critical percentage of low resistivity component


t = critical exponent


The resistivity of the overall FIB material (m) can measured  electrically and determined from the physical geometry of the  line/jumper.  The atomic percentage of the low resistivity  component () is determined from chemical analysis using  energy dispersive spectroscopy (EDS). The remaining  variables from the formula for the critical percentage of the  low resistivity component (c) and the critical exponent (t) are  fit parameters that are determined based on the fit of the model  output to the data collection.  Further explanation of the model  analysis has been published here [25].


Electrical Resistance Measurements


In this paper, we have conducted a series of FIB metal  depositions for both platinum and tungsten jumpers on four  point probe resistance structures.  Figure 2 shows a typical  example of a FIB deposition on the structure.


Figure 2. An example of a FIB metal deposition on the four point  probe structure, with physical measurements labeled to be used for  the resistivity calculation.


This structure and technique allows the resistance of the FIB  material to be measured directly and negates the external  contact resistance of the electrical probes placed on the pads.  The physical dimensions of the FIB metal deposition were  also determined by measurement in a dual beam FIB.  From  these measurements the resistivity of the material can be  determined. The electrical resistivity (ρ) of the material was  determined through four-probe measurements of the resistance (R) of the deposited metal lines (using a HP 34401A  multimeter and a commercial probe station). The length (l) along with the width (w) and the height (h) of the metal lines  were estimated from scanning electron microscope (SEM) imaging and FIB cross sectioning


m = R (w x h) /L


m= resistivity value (ohm-cm)


R= Resistance value (ohms)


L = deposition length (cm)


w= deposition width(cm)


h = deposition height (cm)


Key deposition parameters such as the ion beam current, precursor temperature, beam spot overlap, and lens defocus  were varied in the design of experiments to create a range of  resistance values in the FIB depositions [7]. This work was  done was done with beam currents from 80pA to 2.5nA for  platinum and 80pA to 9.5nA tungsten.  The overlap beam spot  values were investigated in a range  from zero percent to a -150 percent while the defocus value of the ion beam was  changed from a value of zero to a value of 150ums for the  beam spread.  Lastly, the gas injection system (GIS) precursor  delivery temperature started at a value of 42 oC and was  increased up to 54 oC for platinum and from 41 oC to 68 oC for  tungsten.


Chemical Analysis with EDS


Energy dispersive spectroscopy (EDS) was used to determine  the chemical composition of each of the FIB deposited  lines/jumpers.  A typical example of this analysis on a selected  FIB platinum line is shown in Figure 3.


Figure 3.  A representative EDS spectrum of a FIB deposited  platinum line after resistance measurements on the four point probe  structure.  The relative concentration of Gallium, Platinum, Carbon, and Oxygen are shown.


This analytical technique allowed the determination of the  relative concentration of each element in the line.  In all the  analysis, four major elements could be measured in the FIB  deposited material.  Primarily carbon, oxygen, gallium, and  the metal component (platinum or tungsten) were found to be  present.  Using a standard less correlation, the relative atomic  percentage of each element could be calculated.


In addition, transmission electron microscopy (TEM) of  selected FIB deposited platinum and tungsten samples was  performed to examine the structure of the materials as shown  in Figure 4.  Chemical mapping with EDS on the TEM


samples was also done to examine the chemical distribution of  the platinum depostions.  The EDS maps show aggregation of


Pt


the platinum and carbon in the granular structure.  The gallium


104


was present uniformly across the samples (not shown).  The  TEM images of the FIB deposited tungsten also show fine  granular structure, but at a much finer structural level.


Figure 4.  TEM and EDS Maps of FIB Platinum(a &b) and


Tungsten(c) material showning the granular structure of depositions  with different resistivity values.


To determine which chemical elements in the FIB material


play a direct role in  the resistivity of the jumper, the elemental


data from EDS analysis was plotted against the electrical data  examine the relationship. Figure 5 shows a graph of the


Pt, lit.


electrical resistivity of the FIB jumper versus the atomic metal  percentage measured by EDS in each of the FIB deposited  lines. Surprisingly, the graph shows a poor correlation  between the resistivity of the material and the metal atomic  percentage.  The expected relationship should reveal that with  increasing concentration of metal present in the material, the  overall resistivity of the material would correspondingly


102


decrease.  The data in Figure 5, does not show this direct  relationship.  For example, the platinum data point at 42%


75


metal concentration has a measured resistivity greater than  20000-cm, but there are numerous data points for FIB  deposited platinum at a metal concentration near 17% that  have measured resistivities in the range of 800 to 1000-cm.


In addition, the graph shows a FIB tungsten jumper with 17% metal has a lower resistivity than a FIB tungsten jumper with  approximately 73%.   There are also cases in the both the FIB  platinum and tungsten data, where data points have the  electrical resistivity value, but different amounts of metal  present.  For example, platinum data points at 18% and 30% both have resistivity values of 950-cm, and tungsten data  points near 35% and 47% also have nearly identical values of ~350-cm.


Figure 3 shows the result of laser pulse on a Via 6 (V6) layer  surface of 55nm sample. a.) 10x burst: Poly/active exposed, b.) 8x burst: Metal 1 (M1) exposed, c.) 6x burst: Via 1 (V1) exposed, d.) 4x burst: Via 2(V2) exposed.


55nm SRAM Prototype Chip with Cluster Defect


For the first work out on defect chip, FLDT was tested on a 7  metal layers 55nm 32Mb SRAM chip with cluster and  multiple partial column failures. The defect chip shows from  the wafer sort bitmap of the cluster failure. Referring to device  layout studies, the suspect layer is at Via2 (V2) and Metal2 (M2). FLDT using four laser pulses burst was performed on  the cluster failure location to expose V2/M2. The sample was  then performed conventional delayering by slurry polishing to  clear the debris arising from the laser blast and flattens up the  FLDT area. PVC in the SEM image of the V2 layer exposed


by FLDT revealed a patch of abnormally dark vias at M2 (Figure 4).


Figure 4 Bitmap of 32Mb 55nm SRAM chip. The failing mode  is classified as cluster with multiple partial column failure. The cluster location is the suspect location that causes the  failure.


The defect chip was continued deprocess by slurry polishing  to reveal Via1 (V1) and perform PVC inspection, then RIE to  expose Metal1 (M1) to go through PVC again. Similar patch  of irregular dark V1/M1 still remain. The sample was then  performed slurry polishing again to delayer until the contact  layer exposed. From the SEM result, anomalous PVC contrast  propagating all the way to the source/drain contacts (figure 5ad).


The area showing dark PVC, suggesting open contacts to passgate source-drains, was sent for TEM analysis.


Figure 5(a-d) SEM PVC results after layer by layer  deprocessing and inspection on 55nm SRAM chip that have  cluster failure with FLDT.


TEM results were revealing an abnormal profile of the contact  to the active (Rx) area which shown in figure 6. Here, the  contact and nickel silicide (NiSi) did not land on active silicon (Si) due to Shallow Trench Isolation (STI) not being fully  removed by CMP. This caused Polysilicon (PC) residue form  on top of it. The root cause of this failure is related to (STI) CMP issue.


Figure 6 TEM PVC results after layer by layer deprocessing  and inspection on 55nm SRAM chip that failed cluster failure  with FLDT.


28nm SRAM Prototype Chip with Pair Bit  Failure


The following experiment is PFA on 28nm prototype chip  with FLDT. From prior experiments studying the relationship  between laser pulses and material removal on this (top metal  level, M8) test structure, four laser bursts, were found to  remove the top four metal layers (M8 barrier-M4) and expose  Via3 (V3)/Metal3 (M3). Five laser bursts were observed to  expose and damage the Rx layer.


Figure 7 Cross sectional SEM image with FIB after FLDT, (a) after 4x laser burst, and (b) after 5x laser burst.


The SRAM of a 28nm prototype chip with SRAM block was  analyzed by bit map and found to exhibit a pair bit failure  mechanism. SEM images at the failing bit location show dark  PVC at the failing bits’ location after applied FLDT down to  V3/M3 & slurry delayering to the V2 level (figure 8). TEM  revealed broken Metal 2 (M2) to be the cause of the dark PVC  V2 as well as to be the root cause of the PB failure.


Figure 8 SEM and TEM results for a 28nm dual port SRAM  prototype chip with FLDT. Results show that the pair bit  failure is caused by broken M2.


20nm SRAM Prototype Chip with Single Bit  Failure


FLDT was finally applied to a 10-metal layer 20nm with highk metal gate SRAM layout. The same four laser pulse FLDT  protocols as previously described were used, followed by  layer-by-layer slurry and RIE deprocessing and SEM  inspection to identify the root cause of the failure. The last  case is single bit failure which identified by bitmap wafer sort.


Figure 9 shows the FLDT and PFA result on the single bit  failure. FLDT successfully removed the top thick metal layers  to M2 layer. After using slurry deprocessing to Via0 (V0) layer and PVC inspection, an abnormal bright PVC was  observed at the failing bit down to V0 level.


A 10kV ebeam scan at the failing V0 bit revealed a bright  PVC metal gate below the surface of the exposed polish layer.


Figure 9 SEM results for a 20nm SRAM test chip with FLDT. Bright PVC observed at failed single bit. A bright PVC metal  gate observed under 10kV SEM inspection.


Figure 10 shows TEM and EDX result at the abnormal bright  PVC metal gate as shown in Fig. 9. Root cause was  determined to be an irregular metal gate, caused by Tungsten (W) from Contact (CA) diffusing/filling into the metal gate  causing the bit failed.


Figure 10 Bright and dark field TEM and corresponding EDX  results from the defect region shown in figure 9, showing  Tungsten (W) from Contact (CA) diffused/filled into the metal  gate causing the bit failed.


Applications of Fast Laser Deprocessing Technique (FLDT) on SRAM for different technology node were experimented. The technique successfully demonstrated a quick, cost-effective, and convenient way for SRAM PFA. This  technique can remove last few thick metal layers with a simple  few laser pulse burst. Conventional polishing technique may  require several hours’ times, but with FLDT, those stubborn  thick metal layers could be removed within few minutes  including locating time. In this paper, compared to the  conventional delayering method, the experiments managed to  shrink down the total time cycle into half. With this new  methodology, it helps to increase the PFA through put on  SRAM device. FLDT also demonstrated suitability for  applying on the different technology node, including 20nm  advance technology.


The authors would like to thank Globalfoundries Singapore  Pte. Ltd. TEM team and product team of Technology  Development New Technology Prototyping Division for their  great support.


[1] Kendall Scott Wills, Srikanth Perungulam, ISTFA 2007


tutorial ‘Delayering Techniques: Dry processes, wet


chemical, parallel lapping’.


[2] H.H. Yap, P.K. Tan, J. Lam, T.H. Ng, G.R.  Low, R. He,


H. Feng, Y.Z. Zhao, M.K. Dawood, H. Tan, Y.M. Huang,


D.D. Wang,  Z.H. Mai, “Application of Laser


Deprocessing Techniques in Physical Failure Analysis”,


ISTFA 2013, Proceeding, 563-568.


[3] V. Liang, H. Sur, S. Bothra, “Passive Voltage Contrast


Technique for Rapid In-line Characterization and Failure


Isolation During Development of Deep-Submiscron ASIC


CMOS Technology”, ISTFA 1998, Proceedings, pp. 221-


225.


[4] R. Rosenkranz, W. Werner, “Comparison of Active and


Metal %


Figure 5.  A graph of the FIB metal resistivity values plotted with the  the atomic percentage of metal measured by EDS.  Values for both  tungsten and platinum lines are shown.


A stronger correlation and increased understanding can be  shown by including the FIB metal and gallium from the ion  beam in combination. Figure 6 shows the FIB material  resistivity data versus the FIB metal and gallium atomic  percentage in the jumper. A wide dispersion of the platinum  data points continues to exist, but the correlation of the FIB  tungsten data has improved slightly.  The graph shows the  material with the highest concentration of tungsten and  gallium had the lowest resistivity.  The data points for both  platinum and tungsten in the also tend to indicated a trend  toward decreasing resistivity with increasing concentrations of  metallic components.


(Metal+Ga)%


Figure 6.  An improved correlation between the measured resistivity  of the FIB jumpers and the total measured atomic percentage of FIB  metal and gallium from the ion beam.

