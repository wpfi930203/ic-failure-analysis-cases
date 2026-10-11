---
title: "ISTFA-2008.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_b6f353f52a828f0aea7ffb6934a471147295230462135641
file_size: 83570523
---

ISTFA  2008 TM   Conference Proceedings from the


34th International Symposium


for Testing and Failure Analysis


November 2–6, 2008


Oregon Convention Center  Portland, Oregon, USA


Sponsored by


www.asminternational.org/istfa


www.asminternational.org


Published by


ASM International®


Materials Park, Ohio 44073-0002


Copyright  © 2008


by


All rights reserved


No part of this book may be reproduced, stored in a retrieval system, or transmitted, in any form or by any  means, electronic, mechanical, photocopying, recording, or otherwise, without the written permission of  the copyright owner.


First printing, November 2008


Great care is taken in the compilation and production of this Volume, but it should be made clear that NO  WARRANTIES, EXPRESS OR IMPLIED, INCLUDING, WITHOUT LIMITATION, WARRANTIES  OF MERCHANTABILITY OR FITNESS FOR A PARTICULAR PURPOSE, ARE GIVEN IN  CONNECTION WITH THIS PUBLICATION. Although this information is believed to be accurate by  ASM, ASM cannot guarantee that favorable results will be obtained from the use of this publication alone. This publication is intended for use by persons having technical skill, at their sole discretion and risk. Since  the conditions of product or material use are outside of ASM's control, ASM assumes no liability or  obligation in connection with any use of this information. No claim of any kind, whether as to products or  information in this publication, and whether or not based on negligence, shall be greater in amount than the  purchase price of this product or publication in respect of which damages are claimed. THE REMEDY  HEREBY PROVIDED SHALL BE THE EXCLUSIVE AND SOLE REMEDY OF BUYER, AND IN NO  EVENT SHALL EITHER PARTY BE LIABLE FOR SPECIAL, INDIRECT OR CONSEQUENTIAL  DAMAGES WHETHER OR NOT CAUSED BY OR RESULTING FROM THE NEGLIGENCE OF  SUCH PARTY. As with any material, evaluation of the material under end-use conditions prior to  specification is essential. Therefore, specific testing under actual conditions is recommended.


Nothing contained in this book shall be construed as a grant of any right of manufacture, sale, use, or  reproduction, in connection with any method, process, apparatus, product, composition, or system, whether  or not covered by letters patent, copyright, or trademark, and nothing contained in this book shall be  construed as a defense against any alleged infringement of letters patent, copyright, or trademark, or as a  defense against liability for such infringement.


Comments, criticisms, and suggestions are invited, and should be forwarded to ASM International.


ISBN-13:978-0-87170-714-7


ISBN-10: 0-87170-714-4


SAN: 204-7586


Materials Park, OH 44073-0002


Printed in the United States of America


Multiple copy reprints of individual articles available from Technical Department, ASM International.


iii


EDFAS 2008-2009 BOARD OF DIRECTORS


EDFAS President


EDFAS Vice President


Mr. Tracy D. Myers                                                                  Dr. Thomas Moore


ON Semiconductor


|Board Members |Board Members |Affiliation |
|---|---|---|

|Mr. Tracy D. Myers |EDFAS President |ON Semiconductor |

|Dr. Thomas Moore |EDFAS Vice President |OmniProbe |

|Mr. Jeremy A. Walraven |Secretary |Sandia National Laboratories |

|Dr. Lee Knauss |Finance Officer |Booz Allen Hamilton |

|Mr. Gary Shade |Past President |Insight Analytical Labs |

|Ms. Sandra Delgado |Member at Large |Nanolab Technologies |

|Mr. Thomas S. Passek |Executive Director |ASM International |

|Ms. Susan Li |Member at Large |Spansion |

|Dr. Philippe Perdu |Member at Large |CNES |

|Mr. Matthew Thayer |Member at Large |Advanced Micro Devices |

|Mr. David P. Vallett |Member at Large |IBM Systems and Technology |

|Board Committees |Board Committees |Affiliation |
|---|---|---|

|Dr. Charles A. Parker |ASM BOT Liaison |Honeywell Aerospace |

|Ms. Rosalinda M. Ring |EDFA Chair |SMSC Austin |

|Mr.Thomas Zanon |Education Chair |PDF Solutions Inc. |

|Mr. Nicholas Antoniou |Events Chair |Independent Consultant |

|Mr. John West |Membership Chair |Texas Instruments |

|Mr. Gary Shade |Nominating Chair |Insight Analytical Labs |

|Mr. Jeremy Walraven |Website Chair |Sandia National Laboratories |

OmniProbe


iv


ORGANIZING COMMITTEE


David P. Vallett


Nicholas Antoniou      William E. Vanderlinde    Jeremy Walraven         Philippe Perdu


General Chair                 Vice General Chair       Technical Chair            Tutorial Chair                 Tutorial Vice Chair  IBM Systems &


Consultant


Laboratory for


Sandia National Labs        CNES


Technology                                                                       Physical Sciences


Group


Chris Henderson


Immediate Past General Chair


SemiTracks, Inc.


Activities Chairs


Zhiyong Wang


User Groups Chair


Intel Corporation


Janet Teshima


Local Arrangements Chair


IBM


Marsha Abramo


Local Arrangements Vice-Chair


Dave Vallett


EDFAS Liaison


IBM Systems & Technology Group


Chris Richardson


Exposition Chair  LSI Corporation


Tracy Myers


Publicity Chair


Martin Keim


Publicity Vice-Chair   Mentor Graphics


Dan J. Bodoh


Audio/Visual Chair


Freescale Semiconductor


Tom Woods


Audio/Visual Vice-Chair  Biotronic


Ed Keyes


Panels Chair


Semiconductor Insights


v


ISTFA 2008 TUTORIAL COMMITTEE


ISTFA 2008


Tutorial Program Chair


Jeremy Walraven


Sandia National Labs


|Tutorial Committee Chair |Topic |Affiliation |
|---|---|---|

|Cosme Furlong |Fault Isolation, Failure Analysis Basics |Worcester Polytechnic Institute |

|James Griffin |Analog Device Failure Analysis |Analog Devices |

|Leo G. Henry |EOS/ESD, Failure Mechanisms |ESD-TLP Consulting & Testing |

|Becky Holdford |Packaging |Texas Instruments |

|Susan Li |Device and Memory FA |Spansion |

|Tracy Myers |Yield, Test and Logic Diagnostics |ON Semiconductor |

|Chris Richardson |Focused Ion Beam (FIB) |LSI Logic Corporation |

|Rose M. Ring |Device and Memory FA, Emerging Technologies |AMD |

|Kendall Scott Wills |Failure Analysis Basics |Independent Consultant |

|Sam Subramanian |Materials Characterization |Freescale Semiconductor, Inc. |

|Jeremy A. Walraven |MEMS Devices, Microscopy Tools |Sandia National Laboratories |

|Zhiyong Wang |Packaging, Lab Management |Intel Corporation |

vi


ISTFA 2008 SYMPOSIUM COMMITTEE


Technical Program Chair


William E. Vanderlinde


Physical Sciences


CIRCUIT EDIT


BOBBY HOOGHAN, CHAIR


Hooghan Consultancy & Services


STEVE HERSCHBEIN, CO-CHAIR


IBM Systems & Technology


Steve Herschbein, IBM


Mike Phaneuf, Fibics Inc.


EMERGING CONCEPTS


DAN BODOH, CHAIR


MICHAEL BRUCE, CO-CHAIR


AMD


Alex VanVianen, Freescale Semiconductor


Steve Kasapi, NVIDIA


FAILURE ANALYSIS PROCESS 1&2  DAVID BURGESS, CHAIR


Accelerated Analysis


Pete Carelson, FEI Company


Apek Mulay, Independent Consultant


Johnny Lee, X-Fab Texas


Randy Lee, Keithley Instruments Inc.


METROLOGY


JANET TESHIMA, CHAIR


FEI Company


JEREMY RUSSELL, CO-CHAIR


Inotera


Chas Archie, IBM


Roger Alvis, Imago


Loek Kwakman, FEI Company


Barbara Miner, Intel Corp.


Bart Rijpers, ASML


NANOPROBING


SHAWN DECKER, CHAIR


South Dakota School of Mines  TAYLOR CAVANAH, CO-CHAIR  Zyvex Instruments


Terrence Kane, IBM  Phil Kaszuba, IBM


PACKAGE  & ASSEMBLY LEVEL FA  1&2


DEEPAK GOYAL, CHAIR


ZEZHONG FU


Stephane Barbeau, IBM


J. Robert Crawford, DoD


Jessica Hoskins, The Aerospace Corp. on


Ted Kolasa, Freescale Semiconductor, Inc.


Andrew Mawer Freescale Semiconductor, Inc.                         Roger Stierman, Texas Instruments


PHOTON BASED TECHNIQUES 1    STEPHEN IPPOLITO, CHAIR


AARON FALK, CO-CHAIR


OptoMetrics, Inc.


PHOTON BASED TECHNIQUES 2  FELIX BEAUDOIN, CHAIR


PHILIPPE PERDU, CO-CHAIR


CNES


Frank Zachariasse, NXP Semiconductors


Alan Street, QUALCOMM, Inc


Jerome Touzel, Infineon Technologies


PHOTON BASED TECHNIQUES 3    STEPHEN IPPOLITO, CHAIR


KENDALL SCOTT WILLS, CHAIR


Independent Consultant


POSTERS


REENA CHANPURA, CO-CHAIR


Texas Instruments


SAMPLE PREPARATION  EFRAT RAZ-MOYAL, CHAIR  Gatan


Bernd Krüeger, Infineon Tech. Astrid Krehan


David Su, TSMC


David MacHahon, Micron


Arthur Rawers, Xilinx, Inc.


SPM


PHIL KAZUBA, CHAIR


TERRY KANE, CO-CHAIR  IBM


Ben Schrag, Micro-Magnetics  Jim Slinkman, IBM


Pai Tangyunyong, Sandia


SYSTEM LEVEL FA


JAMES DEMERST, CHAIR


JEFF HARTSELL, CO-CHAIR   Dell, Inc.


Ted Levin, IBM  Jeff Birdsley, Dell  Carol Boye, IBM  Ted Levin, IBM


TEST


BRADY BENWARE, CHAIR


Mentor Graphics


SHAWN BLANTON, CO-CHAIR  Carnegie Mellon University


Stephan Eichenberger, NXP


Ken Butler, Texas Instruments  John Carulli, Texas Instruments


YIELD ENHANCEMENT


SARMA GUNTURI, CHAIR


CATHY KARDACH, CO-CHAIR  DCG Systems


Alfredo Herrera, Spansion


Yi Feng, IBM


Cathy Kardach, DCG Systems


2009 FIRST ANNOUNCEMENT AND CALL FOR PAPERS


November 15-19, 2009


McEnery Convention Center San Jose, California USA


“It’s All About Resolution”


Natasha Erdman and Vern Robertson, JEOL USA


EDFASSM35th International


Electronic Device Failure Analysis SocietySymposium for Testing  An Affiliate Society of ASM Internationalb and Failure Analysis™


EDFAS 2008 Photo Contest Winner, First Place False Color: An EBSD (Electron Backscatter Diffraction) map of a wire bond, showing grain size and crystallographic grain orientation.


Submit your abstract today.  Go to www.istfa.org.


Abstract Submisson Deadline:


ISIFA/2009


April 3, 2009 Submisson Deadline:


ix


Contents


IPFA 07 Best Paper


Effect of Refractive Solid Immersion Lens Parameters on the


Enhancement of Laser Induced Fault Localization Techniques .................................... 1


S.H. Goh1, A.C.T. Quah1, C.J.R. Sheppard1, C.M. Chua2, L.S. Koh2, J.C.H. Phang1


(1) National University of Singapore, Singapore


(2) SEMICAPS Pte Ltd, Singapore


Session 1: Emerging Concepts


High Current Focused Ion Beam Instrument for


Destructive Physical Analysis Applications ..................................................................... 7


P. Tesch, N. Smith, N. Martin, D. Kinion   Oregon Physics LLC, Hillsboro, OR USA


Recent Developments in TEM Applications for the IC Industry .................................... 14


L.F. Fu, Y.C. Wang, B. Jiang, F. Shen, M. Strauss, B. Van Leer, C. Senowitz, A. Buxbaum  FEI Company, Hillsboro, OR, USA


Automated Serial-Section Polishing Tomography ......................................................... 21


J.A. Hunt1, P. Prasad1, E. Raz2


(1) Gatan Research & Development, Pleasanton, CA, USA;


(2) Gatan FA Products Division, Pleasanton, CA, USA


Applications of Scanning Near-Field Photon Emission Microscopy ............................ 25


D.V. Isakov1, B.W.M. Tan1, J.C.H. Phang1, Y.C. Yeo1, A.A.B. Tio2, Y. Zhang2,  T. Geinzer3, L.J. Balk3


(1) National University of Singapore, Singapore;


(2) Singapore Institute of Manufacturing Technologies, Singapore;


(3) University of Wuppertal, Germany


Session 2: Packaging and Assembly Level FA I


New Developments in High-Resolution X-ray Computed Tomography for


Non- Destructive Defect Detection in


Next Generation Package Technologies ........................................................................ 30


M. Pacheco, D. Goyal


Intel Corporation,Chandler, AZ, USA


x


Flip-Chip Bump Interface Failure Mechanisms In


Plastic BGA Packages and Failure Analysis Process Flow .......................................... 36


Z. Wang, Sr.


International Rectifier Corp., Temecula, CA, USA


PCB Pad Cratering – Characterization Techniques and Challenges ............................ 43


S. Parupalli1, K. Newman2, M. Ahmad3


(1) Intel Corporation, Hillsboro, OR, USA


(2) Sun Microsystems, Sunnyvale, CA, USA


(3) Cisco Systems, San Jose, CA, USA


Stitch-Bond-Shearing in Optoelectronic Devices,


Caused by Lead-Free-Wave- Soldering – Do We Need


Improved Wire-Bonding Methods? ................................................................................. 49


P. Jacob1, M. Rütsch2


(1) EMPA Swiss Federal Laboratories for Materials Testing and Research, Duebendorf, Switzerland,


(2) Vossloh-Kiepe GmbH, Duesseldorf, Germany


Lead-Free Solder/Gold Metallization Interdiffusion in


Electronic Interconnects – Challenges and their Control ............................................. 53


N. Asrar


Schlumberger Technology Center, Sugar Land, TX, USA


Thick Film Resistor Failures ............................................................................................ 59


A. Shrivastava1, A. Amin1, B. Sood1, M. Azarian1, M. Pecht1, M. Zagami2


(1) University of Maryland, College Park, MD, USA


(2) Fairchild Controls, Frederick, MD, USA


Session 3: Failure Analysis Process I


Active Voltage Contrast and Seebeck Effect Imaging as


Complementary Techniques for Localization of Resistive Interconnections .............. 65


I. Österreicher, U. Rossberg, S. Eckl


Infineon Technologies Dresden GmbH & Co., Dresden, Germany


A Logical Problem Solving Process for


High Via Resistance Root Cause Analysis ..................................................................... 70


K. Li, P. Liu, J. Teong, M. Lee, H.L. Yap


Chartered Semiconductor Manufacturing Ltd., Singapore, Singapore


Vdd Leakage Analysis by a Combination of


Various Failure Analysis Techniques .............................................................................75


Z.G. Song1, S.B. Ippolito1, P.J. McGinnis1, A. Shore1, B. Paulucci1, T. Kane1,  M.P. Tenney1, F.G. Trudeau1, A.W. Kozaczka2


(1) IBM Systems and Technology Group, New York, NY, USA


(2) IBM Systems and Technology Group, Essex Junction, VT, USA


xi


Physical Failure Analysis Techniques and Studies on


Vertical Short Issue of 65 nm Devices ............................................................................ 79


P.K. Tan, Z.H. Mai, S.L. Toh, E. Hendarto, Q. Deng, Y.W. Goh, J.L. Cai, Y.Z. Ma,  H.B. Lin, L. Zhu, J. Yu, H.L. Li, Q.F. Wang, R. He, H. Tan, J. Lam


Chartered Semiconductor Manufacturing Pte. Ltd.


Fast Root Cause Analysis Based on Electrical Defect Localization ............................ 85


M. Schmidt1, L. Dworkin1, C. Hess2, M. Squcciarini2, S. Yu2, J. Burrows2


(1) FEI Company, Hillsboro, OR, USA


(2) PDF Solutions Inc., San Jose, CA, USA


Failure Analysis for Gate Oxide Breakdown .................................................................. 88


X. Chen, M. Li, Q. Guo, K. Chien, Y.-B. Gao


Semiconductor Manufacturing International Company, Shanghai, P.R.China


Session 4: Package and Assembly Level FA II


Non Invasive Failure Analysis of Passive Electronic Devices in


Wireless Modules Using X-ray Micro Tomography (MicroCT) ...................................... 92


T. Pendleton1, L. Hunter2, S.H. Lau2


(1) RFMD, Greensboro, NC, USA


(2) Xradia, Inc., Concord, CA, USA


Scanning Acoustic Microscopy for


Solder Joint Failure Analysis and Design Improvements ............................................. 99


R. Varma, J. Bartolovitch, V. Brzozowski, C. Sokolowski


Northrop Grumman Electronic Systems, Baltimore, MD, USA


Lock-In-Thermography for 3- Dimensional Localization of


Electrical Defects inside Complex Packaged Devices ................................................ 102


C. Schmidt1, F. Altmann1, C. Grosse1, A. Lindner2, V. Gottschalk3,


(1) Fraunhofer Institute for Mechanics of Materials, Halle, Germany


(2) Micronas GmbH, Freiburg, Germany


(3) Elmos Semiconductor AG, Dortmund, Germany


An Analytical Technique to Assess the Risk of Laser Damage to


Encapsulated Integrated Circuits during Package Laser Marking ............................. 108


J. Patterson1, C. Schuring2


(1) Applied MicroCircuits Corporation, San Diego, CA, USA


(2) Quantum Focus Instruments, Vista, CA, USA


Techniques for Identification of Silver Migration in


Plastic Encapsulated Devices Assembled with


Molding Compound Containing Red Phosphorus Flame Retardant Material ........... 112


R.R. Hylton


Maxim Integrated Products, Hillsboro, OR, USA


xii


Emerging Techniques for the Characterization of


Nano-Mechanical Properties of Integrated Circuit Components ................................ 121


N. Randall, R.P. Nair


CSM Instruments, Needham MA, USA


Session 5: Circuit-Edit


Manufacturing In-Line Whole Wafer Focused Ion Beam (FIB)


Memory Address Descramble Verification ................................................................... 128


S.B. Herschbein, H.H. Kang, S.L. Jansen, A.S. Dalton


IBM Systems & Technology, Hopewell Junction, NY, USA


An Analysis of Tungsten FIB-Fabricated Via Resistance ............................................ 133


D.W. Niles1, J. Meyer1, R.W. Kee1, M. DiBattista2


(1) Avago Technologies, Fort Collins, CO, USA


(2) FEI Corporation, Hillsboro, OR, USA


Backside Circuit Edit on Full-Thickness Silicon Devices ............................................ 141


C. Rue1, S. Herschbein2, C. Scrudato2


(2) IBM Corporation, Hopewell Junction, NY, USA


Insulator Deposition for Through Conductor Editing .................................................. 151


C. Richardson1, M. Martin1, T. Malik2, J.P. Barone2


(1) LSI Corporation, Fort Collins, CO, USA


(2) DCG Systems, Fremont, CA, USA


Creation of Solid Immersion Lenses in Bulk Silicon Using


Focused Ion Beam Backside Editing Techniques ....................................................... 157


P. Scholz1, U. Kerst1, C. Boit1, C.-C. Tsao2, T. Lundquist2


(1) Berlin University of Technology, Berlin, Germany


Session 6: Sample Preparation I


S/D LDD Junction Stain/Delineation by


Electrochemical Displacement with Illumination ......................................................... 163


R.-L. Chiu, T. Chen, S. Chen


WaferTech LLC Camas, WA, USA


A New Method of Wafer Level Plan View TEM


Sample Preparation by DualBeam ................................................................................. 168


H.H. Kang1, M.A. Gribelyuk1, O.D. Patterson1, S.B. Herschbein1, C. Senowitz2


(1) IBM Microelectronics, Hopewell Junction, NY, USA


(2) FEI Company, Hillsboro, OR, USA


xiii


Embedded Gold Markers for Improved TEM/STEM


Tomography Reconstruction ......................................................................................... 172


J.-S. Luo, C.-C. Huang, J.D. Russell


Inotera Memories, Inc., Taoyuan, Taiwan, Republic of China


Session 7: Photon Based Techniques I


Timing Sensitivity Analysis of Logical Nodes in


Scan Design Integrated Circuits by Pulsed Diode Laser Stimulation ........................ 180


T. Kiyan1, C. Boit1, C. Brillert2


(2) Infineon Technologies, Munich, Germany


Dual Port RAM MBIST Failure Analysis Using


Time Resolved Dynamic Laser Stimulation ................................................................. 188


J. Shaw1, C. McMahon1, Y.S. Ng2, F. Beaudoi2


(2) DCG, Fremont, CA, USA


Mixed Frequency Detection of Thermal Laser Stimulation (MF-TLS) and


Its Application in Failure Analysis ................................................................................ 193


Z. Qian, C. Brillert, C. Burmer


(1) Infineon Technologies, Munich, Germany


Differentiation between Artifacts and True Defects in


45 nm BEOL Structures in M-TLS Technique .............................................................. 198


A. Reverdy1, P. Perdu3, M. de la Bardonnie1, H. Murray2, P. Poirier1, B. Domengès2


(1) NXP Semiconductors, Caen, France


(2) LaMIPS, Laboratoire commun NXP-CRISMAT, Caen, France


(3) CNES, Toulouse, France


Session 8: Scanned Probe Microscopy


Calibration of Nanoprobe Capacitance-Voltage Spectroscopy (NCVS) ..................... 204


T. Kane1, M.P. Tenney1, A. Erickson2, P. Harris2


(2) Multiprobe, Inc., Santa Barbara, CA, USA


Analysis of Deep Trench Node Leakage Depth by


Applying Current Imaging Technique at Silicon Level ................................................ 209


S. Doering, M. Seitz, U. Zimmermann, P. Rodger, W. Werner  Qimonda Dresden GmbH & Co. OHG, Dresden, Germany


xiv


Session 9: Photon Based Techniques II


Backside Failure Analysis by Electroluminescence on Microwave Devices ............. 214


M. Bouya1, D. Carisetti1, P. Delaqueze1, J.C. Clement1,  N. Malbert2, N. Labat2, P. Perdu3


(1) Thales Research and Technology, Palaiseau, France


(2) IMS Laboratory, Talence, France


(3) CNES Laboratory, Toulouse, France


Photon Emission Spectral Signatures of AlGaN/GaN HEMT for


Functional and Reliability Analysis ............................................................................... 220


A. Glowacki1, C. Boit1, R. Lossy2, J. Würfl2


(2) Ferdinand Braun Institut für Höchstfrequenztechnik, Berlin, Germany


Laser Scanning Localization Technique for


Fast Analysis of High Speed DRAM Devices ................................................................ 227


M. Versen1, A. Schramm1, J. Schnepp1, S. Hoch1, T. Vikas1, D. Diaconescu2


(1) Qimonda AG, Neubiberg, Germany


(2) Infineon AG, München, Germany


Novel Application of the OBIRCh Amplifier for


Timing Failure Localization ............................................................................................ 233


M. Sienkiewicz1, S. Brule2, P. Perdu1, A. Firiti2, O. Crepel2


(1) CNES - French Space Agency, Toulouse, France


(2) Freescale Semiconductor, Toulouse, France


Session 10: Posters


Novel Sample Preparation Technique for


Backside Analysis of Singulated Die ............................................................................238


S. Elliott, M. LaPierre, P. Plourde


Fairchild Semiconductor, South Portland, ME, USA


Innovative Method & Use of UV Technologies for


Dye Penetrant Sample Preparation ...............................................................................242


T.R. McDonald


Intel Corporation, Hillsboro OR, USA


The Failure Analysis of Specific Source-to-Drain Dislocation and


Case Study ...................................................................................................................... 245


C.H. Wang, S.W. Lai, C.Y. Wu, B.T. Chen, J.Y. Chiou, J.H. Chou


Taiwan Semiconductor Manufacture Company, Ltd., Taiwan, R.O.C.


Next Generation Laser Voltage Probing .......................................................................249


Y.S Ng, W. Lo, K. Wilsher


DCG Systems, Inc., Fremont, CA, USA


xv


A Study of the Photoelectric Effect Caused by a


Laser Beam Used in a Beam Bounce Technique in a C-AFM System ....................... 256


H.-S. Lin, M.-S. Wu


United Microelectronics Corporation, Ltd. Taiwan, R.O.C.


Applications of C-AFM and CBED Techniques to the Characterization of


Substrate Dislocations Causing SRAM Soft Single-Column Failure


Contained in a Wafer with (001) Plane/[100] Notch ..................................................... 260


H.-S. Lin, T.-H. Chen, W.-C. Shu


United Microelectronics Corporation, Ltd., Taiwan, R.O.C.


Electroluminescence Analysis by Precise Tilt Polish Technique of


Edge-Emitting Laser Diode ............................................................................................ 265


H. Ichikawa, K. Sasaki, K. Hamada, A. Yamaguchi  Sumitomo Electric Industries, Ltd., Japan


A Novel OBIRCH Fault Isolation Method to Locate the Leakage Failure Point ......... 269


C.-L. Huang ,Y.H. Shu


Case Study of High Temperature Failure Analyses


Using an On-Chip “Heater” ............................................................................................ 273


F. Zhang, C. Lewis, T. Duryea


Texas Instruments Inc., Dallas, TX, USA


Development of PECS Application for Sample Preparation ....................................... 277


X. Chen, M. Li, Q. Guo, W.T. Kary Chien


Semiconductor Manufacturing International Company, Shanghai, P.R. China


Automated Sample Preparation of Packaged Microelectronics for FESEM .............. 280


R.R. Cerchiara, P.E. Fischione, M.F. Boccabella, A.C. Robins   E. A. Fischione Instruments, Inc., Export, PA, USA


Studies of Fluorine-Induced Corrosion and Defects on


Microchip Al Bondpads and Elimination Solutions ..................................................... 285


H. Younan, N.R. Rao, T. Jennifer


Optimization of SEM Analytical Conditions for


Low K and Ultra Low K Dielectric Materials ................................................................. 291


L. Binghai, M. Zhiqiang, H. Younan, T. Jennifer   Chartered Semiconductor Mfg. Ltd., Singapore


Using Cross-Triggering in Oscilloscope for


Debugging Multiphase Converter Circuit of


Personal Computer (PC) Motherboard ......................................................................... 294


B. Nguyen, O. Diaz


Intel Corporation, Hillsboro, OR, USA


xvi


Doping Profile Measurements in a 65-nm Commercial Product Using


Atom Probe Tomography ............................................................................................... 297


L. Klibanov1, D. James1, D. Isheim2


(1) Chipworks Inc., Ottawa, Ontario, Canada


(2) Northwestern University Center for Atom-Probe Tomography (NUCAPT),  Evanston, IL, USA


Failure Analysis of Nitride-Trapping Memory Cell Failures ........................................ 301


W.-R. Chen, Y.-J. Chen, I.-C. Chang, H.-H. Chiang, L.-K. Kuo, S. Yin, C.-Y. Lu  Macronix International Co., Ltd., Hsinchu, Taiwan


Advanced Methodologies for Backside Circuit Edit .................................................... 305


E. O’Donnell1, D. Scott1, T. Malik2, R. Jain2, T. Lundquist2,  R. Schlangen3, U. Kerst3, C. Boit3


(1) Intel Corporation, Folsom, CA, USA


(3) Berlin University of Technology, Berlin, Germany


Physical Failure Analysis Techniques Using


3D Rotation Imaging Method by STEM ......................................................................... 315


T.-S. Back, J.-H. Kim, S.-J. Lee, J.-W. Jung, T.-O. Jung, H.-J. Kim, S.-Y. Lee   Hynix Semiconductor Inc., Ichon-si, Kyoungki-do, Korea


High Precision Ion Beam Milling with Time of Flight Compensation ......................... 317


T. Holtermann, A. Graupera, S. Rosenberg, M. DiBattista  FEI Company, Hillsboro, OR, USA


Applications of In-situ Sample Preparation and Modeling of


SEM-STEM Imaging ........................................................................................................ 320


R.J. Young1, A. Buxbaum1, B. Peterson1, R. Schampers2


(2) FEI Company, Eindhoven, The Netherlands


Sample Preparation Technique for


Bond Pad IMD (Inter-Metal Dielectric) Damage Observation ...................................... 328


Y.S. Huan, Y.L. Kuo, Y.T. Lin, J. Chen, K.Y. Lee


Taiwan Semiconductor Manufacture Company, Ltd. Hsinchu, R.O.C.


Session 11: System Level Failure Analysis


Dynamic Laser Stimulation Technique for Device Qualification Process ................. 332


A. Deyine-Barth1, P. Perdu1, G. Benetti1, K. Sanchez1, F. Battistella1, D. Lewis2


(1) CNES & THALES Laboratory, Toulouse Cedex France


(2) IMS, Talence Cedex, France


xvii


Lead Frame Metal Migration in an Encapsulated IC Package ..................................... 339


W. Eslinger


Boston Scientific, St. Paul, MN, USA


Latent Flash Single Bit and Multiple Bits Systematic Approach to


Failure Analysis .............................................................................................................. 344


H.-Y. To, D. Nguyen, C. Dunn, D. Davis


Texas Instruments Inc., Houston, TX, USA


Reliability for Pure CMOS One-Time Programmable Memory Using


Gate-Oxide Anti-Fuse (eFuse) ....................................................................................... 349


N. Wakai


Toshiba Corporation, Yokohama, Japan


Laser Failure Isolation Techniques Demonstrated On Test Structures ..................... 354


F.S. Arnold


Texas Instruments, Dallas, TX, USA


Session 12: Sample Preparation II


Single Die 'Hands-Free' Layer-by-Layer Mechanical Deprocessing for


Failure Analysis or Reverse Engineering ..................................................................... 363


T. Moor1, E. Malyanker2, E. Raz-Moyal2


(1) Datel Design and Development Ltd, Stone, Staffs, UK


(2) Gatan, Pleasanton, CA, USA


Characterization and Failure Analysis of Wafer Bonded Devices and


Unfilled Through-Silicon-Vias (TSVs) ........................................................................... 368


C. Cassidy1, J. Kraft1, G. Koppitsch1, E. Brandlhofer1, M. Steiner1, F. Schrank1,  D. Erwin2, E. Raz-Moyal2


(1) austriamicrosystems AG, Graz, Austria


(2) Gatan Inc., Pleasanton, CA, USA


Detection and Characterization of an Electrical Failure Induced during


Laser Ablation of Packages ........................................................................................... 375


P. Schwindenhammer, H. Murray, P. Descamps, P. Poirier  NXP Semiconductors, Caen, France


Session 13: Test


Timing Failure Debug Using Debug-Friendly Scan Patterns and TRE ....................... 383


C. Burmer1, R. Guo2, W.-T. Cheng2, X. Lin2, B. Benware2


(2) Mentor Graphics Corp., Wilsonville, OR, USA


xviii


Improving Fault Isolation Using Iterative Diagnosis .................................................... 390


K. Gearhardt1, C. Schuermyer2, R. Guo 2


(1) LSI Logic Corporation, Ft. Collins, CO, USA


(2) Mentor Graphics Corporation, Wilsonville, OR, USA


Deterministic Localization and Analysis of Scan Hold-Time Faults ........................... 396


J. Hwang1, D. Kim1, N. Seo1, E. Lee1, W. Choi1, Y. Jeong1, J. Orbon2, S. Cannon2


(1) Samsung Electronics Co., Ltd., Youngin-City, Gyeonggi-Do, Korea


(2) Verigy Inc – Inovys DfX Solutions, Pleasanton CA, USA


Session 14: Photon Based Techniques III


Combining Refractive Solid Immersion Lens and


Pulsed Laser Induced Techniques for


Effective Defect Localization on Microprocessors ...................................................... 402


A.C.T. Quah1, S.H. Goh1, V.K. Ravikumar2, S.L. Phoa2, V. Narang2, J.M. Chin2,  C.M. Chua3, J.C.H. Phang 3


(2) Advanced Micro Devices Pte. Ltd, Singapore


(3) SEMICAPS Pte. Ltd., Singapore


Evaluating PICA Capability for Future Low Voltage SOI Chips .................................. 407


F. Stellari1, P. Song1, J. Vickers2, C. Shaw2, S. Kasapi3, R. Ispasoiu4


(1) IBM T.J. Watson Research Center, Yorktown Heights, NY, USA


(3) NVIDIA Corp., Santa Clara, CA, USA


(4) Fairchild Imaging, Milpitas, CA, USA


Session 15: Nanoprobing


An Application of a Nanoprobe Technique in the Characterization of


Advanced SRAM Devices ............................................................................................... 417


H.-S. Lin, C.-M. Chen


Failure Analysis of Single Shared Column Fail in DRAM Using


Nano-Probing Technique ............................................................................................... 423


S.M. Kim, J.H. Lee, J.H. Lee, H.K. Kim, M.S. Chang, J.H. Lee, S.J. Hong  Hynix Semiconductor Inc., Kyoungki-do, Korea


Low Voltage, Low Current AFP Characterization of


Non-Visible Soft Transistor Defects .............................................................................. 428


R. Mulder, S. Subramanian, T. Chrastecky


Freescale Semiconductor, Inc., Austin, TX, USA


xix


Characterization and Analysis of 45nm Node SRAM Standby Leakage .................... 437


D.E. Albert, Z.G. Song, S.B. Ippolito, L. Fischer, M.P. Tenney  IBM, Hopewell Junction, NY, USA


Investigation on Focused Ion Beam Induced Damage on


Nanoscale SRAM by Nanoprobing ................................................................................ 445


E. Hendarto, S.L. Toh, P.K. Tan, Y.W. Goh, J.L. Cai, Y.Z. Ma, Z.H. Mai,  J. Lam, J. Sudijono


Chartered Semiconductor Manufacturing Ltd., Singapore


Session 16: Yield Enhancement


Oxidation of TiN ARC Layer as a Reliability Issue for ICs .......................................... 449


M. McVeigh1, A. Raz1, W.J. Kindt1, A. Gomes1, K.Y. Wong1, T. Inamine1, T.J. Bold2


(1) National Semiconductor, Santa Clara, CA, USA


(2) Bold Productions, Roanoke, TX, USA


Timing Problems Due to Spacer Bridging in a Sub-100 nm Product ......................... 459


J. van Hassel


NXP Semiconductors, Nijmegen, Netherlands


A Study of Pad Contamination Defect and Removal ................................................... 464


K.A. Mohammad, L.J. Liu, S.F. Liew, S.F. Chong, D.G. Lee, S.F. Lee and B.C. Lee  X-Fab Sarawak SDN. BHD., Kuching, Sarawak, Malaysia


A Study to Remove Heavy Polymer Remain on Thick Metal (> 3 micron)


Sidewall Profile after Metal Etch Solvent Clean Step .................................................. 468


S.F. Liew, K.A. Mohammad, L.J. Liu, S.F. Chong, D.G. Lee, S.F. Lee,  B.C. Lee  X-Fab Sarawak SDN. BHD., Kuching, Sarawak, Malaysia


Yield Enhancement Using a Combination of Wafer Level Failure Analysis and


Defect Isolation Software: Case Studies ...................................................................... 471


P. Simon1, M. Thétiot1, B. Picart1, C. Kardach2, H. Deslandes2,  F. Dudkiewicz3, J.-P. Roux4


(1) Atmel, Rousset, France


(2) DCG Systems, CA, USA


(3) Credence Systems Corporation, France


(4) Sector Technologies SAS, France


Session 17: Failure Analysis Process II


A Procedure for Identifying the Failure Mechanism Responsible for a


Pin-To-Pin Short Within Plastic Mold Compound Integrated Circuit Packages ........ 476


C. Nail, J. Rocha, L. Wong


National Semiconductor Corporation, Santa Clara, CA, USA


xx


Mis-identified Failures in FETs ...................................................................................... 481


M. Gores,


Hi-Rel Laboratories, Spokane, WA, USA


Frontside and Backside Analysis of Surface ESD ....................................................... 485


D. Daly, L. Grogan, F. Keating, Xilinx, Ireland


Intermittent Failures, Challenges and Strategies Involved with


Finding Root Cause ........................................................................................................ 490


N. Konkol


Transient Latch-Up Analysis of Power Control Device with


Combined Light Emission and Backside Transient


Interferometric Mapping Methods ................................................................................. 493


M. Heer1, D. Pogany1, M. Street2, I. Smith2, F. Riedlberger2, D. Bonfert3, H.A. Gieser3


(1) Vienna University of Technology, Vienna, Austria


(2) Diodes Incorporated, Oldham, United Kingdom


(3) PS ATIS Analysis & Test of Integrated Systems, Munich, Germany


Session 18: Metrology


3D STEM Tomography Based Failure Analysis of 45 nm CMOS Devices .................. 499


F. Lorut1, D. Delille2


(1) STMicroelectronics, Crolles, France


Dopant Analysis on Advanced CMOS Technologies ................................................... 505


F. Siegelin, A. Dübotzky, B. Danzfuss, S. Schömann  Infineon Technologies, Munich, Germany


SEM Si Dopant Contrast Enhancement Using Sample Charging ............................... 510


Y.-W. Hsieh, J.D. Russell, P.-Y. Chen


Inotera Memories, Inc., Taiwan, Republic of China


3-D Image Reconstruction in the Scanning Electron Microscope .............................. 515


W.E. Vanderlinde


Laboratory for Physical Sciences, College Park, MD, USA


Author Index .................................................................................................................... 525


ISTFA 2008: Proceedings from the 34th International Symposium for


Copyright © 2008 ASM International®


Testing and Failure Analysis


All rights reserved.


November 2-6, 2008, Portland, Oregon USA


DOI: 10.1361/cp2008istfa001


Effect of Refractive Solid Immersion Lens Parameters on the  Enhancement of Laser Induced Fault Localization Techniques


SH Goh1, ACT Quah1, CJR Sheppard2 , CM Chua3, LS Koh3, JCH Phang1, 3 1Centre for Integrated Circuit Failure Analysis and Reliability,


National University of Singapore, 10 Kent Ridge Crescent, Singapore 119260


2 Bioimaging Laboratory, Div of Bioengineering, National University of Singapore, Singapore 117574  3SEMICAPS Pte Ltd, 28 Ayer Rajah Crescent #03-01, Singapore 139959


Phone: +65-6516-3890 Fax: +65-6516-7912 Email: gohszuhuat@nus.edu.sg


Abstract


The effect of Refractive Solid Immersion Lens (RSIL)


parameters on the enhancement to laser induced fault


localization techniques are investigated. The experimental


results of the effect on a common laser induced technique,


namely Thermally Induced Voltage Alteration (TIVA), and


imaging are presented.  A signal enhancement in the peak


TIVA signal of close to 12 times has been achieved.


I. INTRODUCTION


Laser induced techniques are widely used for frontside


and backside fault localisation in semiconductor integrated


circuit (IC) failure analysis (FA) [1]. For backside thermal


stimulation, a 1340 nm wavelength laser is commonly used


to obtain high transmittance through the silicon substrate [2].


In far-field systems, the laser spot size at a numerical


aperture (NA) of 0.7 is diffraction limited to approximately


1 µm.  This resolution limit compromises the performance


for both backside optical imaging and the fault localization


precision of laser induced techniques especially as ICs scale


towards the 65nm and 45nm technology nodes. An effective


approach is to apply immersion lens technology. Solid [3]


and liquid [4] immersion lens technologies have been used


to extend the diffraction limit by increasing NA. The two


main types of solid immersion lens (SIL) technologies that


are applicable to backside FA are Refractive SIL (RSIL) [3]


and Diffractive SIL [5].


RSIL involves placing a truncated spherical silicon (Si)


lens on top of the back Si substrate [6]. The resolution


enhancement from RSIL leads to a smaller laser spot size


which will have a direct impact on Thermally Induced


Voltage Alteration (TIVA) signal [7] which is proportional


to laser power density. In practice, due to limitations in


common mechanical polishers, precise thinning of Si


substrate to fit an RSIL design may not be routinely


achievable. Furthermore, because of light bending, the


aperture angle in air (objective angle) changes when the


RSIL


laser is focused at different focal planes affecting the


Sample


objective NA.  The degree of enhancements from RSIL  depends strongly on these factors. In the worst case, enhancements may not be achieved under certain conditions.  Therefore, it is essential to understand these effects prior to  the application of RSIL to laser induced techniques.


In this paper, we investigate the effects of varying laser  focusing planes and objective NA on the enhancements of  TIVA with RSIL. These are the two main RSIL parameters. The focusing plane is varied by changing the RSIL design. The results provide information on the optimum conditions  and the effective objective NA required in combination with  the RSIL to maximize the enhancements. The latter is  termed objective NA matching in this paper.


II. BACKGROUND


A. Refractive Solid Immersion Lens (RSIL)


RSIL is a truncated spherical silicon (Si) lens which is  placed on the back surface of the Si substrate [6]. The  Centric RSIL involves imaging at the focal plane which is at  the centric position (point C) of the Si lens and is aberrationfree. This can be achieved by the combination of the Si lens  thickness and backside thickness so that the focal plane is at  the centric position of the Si lens as shown in Fig. 1(a).


The Centric RSIL reduces the laser spot size by  increasing the focusing aperture angle in Si. The aplanatic  RSIL further increase this angle through favourable light  bending at the spherical interface. The aplanatic focal point (point A) which is also aberration-free is at a distance of  equal to Si lens radius divided by the Si refractive index. The effect of refractive index mismatch between the Si lens  and doped Si backside is neglected since the real component  is close to 3.5 in the light wavelength concerned [8].


(a) Centric


(b) Aplanatic


Fig. 1. Laser focusing at Centric point (a) and Aplanatic point (b).


The resolution performance achievable by a centric and  aplanatic RSIL is comparable. However, the advantage of an  aplanatic configuration over the centric is the fact that it  requires a low backing objective NA to achieve a good  performance. A centric RSIL is usually limited by backing  NA. It is reported that a lateral spatial resolution of 0.23 µm  has been achieved using a 1.05 µm wavelength laser when  imaging close to aplanatic configuration. The objective NA  is 0.3 [9].


B. Thermally Induced Voltage Alteration


TIVA is a laser induced technique used for active fault  localisation based on thermal stimulation. This technique  involves using a scanned 1340 nm laser beam to localize  faults which are sensitive to thermal stimulation. It is based  on constant current bias and voltage detection configuration. The change in voltage during thermal stimulation is detected  by an ac-coupled amplifier, digitized and then mapped into a  TIVA image [1]. Subsequently, the TIVA image is overlaid  on the reflected laser image for fault localization. The  localization precision is dependent on the strength of TIVA  signal, signal spot size and spatial resolution of reflected  laser image.


The intensity of TIVA signal is proportional to the laser  power and laser spot size, i.e. the power density of the  incident laser beam. The laser spot size can be significantly  reduced by RSIL to enhance the TIVA signal and the TIVA  signal spot size. The reduction in beam resolution can also  give rise to a better resolved reflected laser image.


III. EXPERIMENTAL SETUP


Fig. 2 shows the schematic diagram of the experimental  setup on SEMICAPS SOM 1005 Analytical Scanning  Optical Microscope System. Mitutoyo 10X (0.26 NA), 20X (0.4 NA), 50X (0.42 NA) and 100X (0.5 NA) objectives are  used. It should be noted that the effective NA for the 10X  and 20X objectives are less than the designed values since  the objective back pupil is not filled completely by the laser  beam. The RSIL setup is in a decoupled configuration as  shown in Fig. 2. It is not attached to the objective lens. The  add-on components for the decoupled RSIL setup consist of  a mechanical aperture structure and a micromanipulator. The  truncated Si lens is placed on top of the device under test  and brought close to the area of interest. The mechanical  aperture is necessary to apply sufficient pressure between  the lens and sample interface for optical coupling [6] during  imaging by lowering the micromanipulator. The  micromanipulator is also used for fine movement of the  RSIL to align the RSIL to the optical axis of the objective  lens using a series of alignment steps. A thin layer of optical  fluid is used between the lens and sample to avoid scratching  the lens during RSIL movement as well as for better contact  to eliminate air gaps. In this work, the RSIL is fabricated  from a 1 mm diameter Si sphere which is doped in the range  of 1x1017-1x1018 cm-3 and polished to variable thicknesses.


Fig. 2. Decoupled RSIL experimental setup.


The test structure is a 0.5 m/0.9 m (line/space) polysilicon  serpentine structure on a substrate doped at 5x1015 cm-3. The  substrate thickness is kept constant at around 60 µm. The  mechanical structure has a clear aperture of 90-93% transparency.


IV. RESULTS AND DISCUSSION


A. TIVA Enhancements from RSIL


Fig. 3(a) shows the TIVA signal image using 1340 nm  laser with a 20X objective from voiding defects along the  serpentine tracks which is biased with a constant current of  10 µA. From the overlay image in Fig. 3(b), it is evident that  the defects cannot be precisely localized because the  serpentine tracks are not resolvable and the TIVA spots are  large. With the same sourcing current, laser power and  amplifier settings, the experiment is repeated with RSIL. Fig. 4(a) and 4(b) show the TIVA signal and overlay images  respectively.


The serpentine lines are clearly resolved and the defect  sites are localized precisely along the lines with stronger  TIVA signal. The reflected laser image also reveals the  magnification enhancement from RSIL.


(a)


(b)


Fig. 3. TIVA image (a) and overlay image (b) from a  polysilicon structure using Mitutoyo 20X objective.


Fig. 4. TIVA signal image (a) and overlay image (b) from a  polysilicon structure using Mitutoyo 20X objective and RSIL  application.


The middle signal is more enhanced than peripheral spots  because of increasing aberrations away from the lens optical  axis. To quantify the enhancements from RSIL, the line  profile AA’ is plotted across the middle defect for the case  of with and without RSIL as shown in Fig. 5(a).  The line  profiles are normalized to the same magnification to take  into account the increase in magnification due to RSIL.


Fig. 5(b) shows the peak TIVA signal enhancement of  close to 4.5 times with RSIL. In this case, the theoretical  laser spot size is enhanced by approximately 8 to 9 times. The peak TIVA signal is defined as the signal peak above  noise mean. It should be noted that the enhancement in  TIVA signal is not directly proportional to the spot size  enhancement because of laser power absorption from the  additional SIL thickness. The TIVA signal intensity could  also be affected by the nature of the defect and the effective  interaction area between the defect and laser spot size.


The lines profiles are normalized to signal intensity to  compare the Full Width Half Maximum (FWHM) of the  TIVA signal. Fig. 5(c) shows that the FWHM of TIVA  signal with and without RSIL is around 0.6 µm and 2 µm  respectively. The reduction of TIVA FWHM by about 3  times shows that with RSIL, the TIVA signal is reduced  close to the defect size of approximately 0.5 µm.


(c)


Fig. 5. Location of AA’ (a), line profile of AA’ (b) and


normalized intensity plot (c), across TIVA signal spot.


B. Power Loss from RSIL and Objective Lens


For backside RSIL application, additional laser power  losses can arise from reflections at the spherical interface of  RSIL, laser power absorption by SIL and power loss due to  laser beam truncation by the back pupil of objective lens. Fig. 6(a) shows a comparison between the TIVA line  profiles of the cases with selected RSIL designs and without  RSIL application. The same laser power of 26.4mW is used  and the objective is fixed at 20X. The power loss due to  reflections at spherical interface is assumed to be constant  for RSILs at different focal planes. Fig. 6(a) shows that  TIVA signal enhancement of 4.5 times is achieved at focal  planes, Z=13 µm and 135 µm. However at 164 µm, although  the laser spot is enhanced, there is no significant  enhancement in TIVA signal. This is because the power loss  by laser absorption through highly-doped thicker RSIL  compromises the increase of power density due to reduction  of laser spot size. This is the issue if the RSIL lens is highly  doped. The laser spot size enhancement is evident in Fig. 6(b) which shows that the FWHM of the TIVA spot are  similar and close to defect size.


4µm


Distance (μm)


260Objective Lens:20X(0.4 NA)0Without RSIL


260Amplifier gain: 500△


Laser power: 26.4 mW0


240.(w.r.t.20X objective)


Amplifier gain:500


With RSIL


220


(z=135 μm)g 0With RSIL


200


(z=164 μm)E


180


莒


曹


△0


160


TIVA Signal Intensity (a.u.)


TIVA) Intensity (a.u. Signal


1400


120


.000合


100000000


120-


00088


100


0.00.51.01.52.02.53.03.54.0


0.00.511.0152.02.5 0,od


140


△


(z=13 μm)


240


100X(0.5NA)


Distance from centric:13μm△△-0-50X(0.42 NA)20X(0.4NA)


Fig. 6. Line profile (a) and normalized intensity plot (b), across TIVA signal spot.


Fig. 7 illustrates the significance of laser beam truncation by  the back pupil of the objective lens. In this case, focal plane  is fixed at 13 µm below centric point and the same laser  power of 36 mW measured before objective lens is used. Fig. 7 shows that switching to higher NA objective lens  degrade TIVA signal strength in spite of reduction in laser  spot size as NA increases. This is because the power loss by  laser beam truncation is more significant than the reduction  in laser spot size, giving rise to an overall degradation in  power density.


1.0


70


The pupil diameter, PD [10] is defined as:


‘OO


--0-Collection angle


0.8


- 66


-0-NA


-68


NA


f


PD


*


2


=


(1)


8 p


Mechanical aperture opening:


90% transparency (w.r.t. SIL diameter)C64


8


60


b品


620


As NA increases with higher objectives, the objective focal


0


length f reduces faster, resulting in an eventual reduction in


e


人0.4


8en


N


8A0


PD. A smaller pupil diameter leads to a larger beam


10 3


truncation and power loss since the beam diameter is fixed.


q 0


0.2


52


0.23 NA


54(


This loss can be compensated by increasing the laser power.


Note: Calculation is based on paraxial rays0


(Geometrical optics)


0.002040608010012014018048Aplanatic location


6-50


Fig. 7. Degradations from objective lens.


1.0Laser power:26.4 mVWObjective Lens:20X(0.4 NA)


△-Without RSIL With RSIL


(w.r.t.20X objective)


(z=13 jμm)


C. Objective NA matching


8Amplifier gain:500


With RSIL(z=135 μm)With RSIL


The mechanical aperture structure plays an important


(z=164 μm)


role in RSIL. The collection angle decreases with increase in


品


focusing depths for a fixed clear aperture. Fig.8 shows the  corresponding objective NA required based on 90% clear


力


aperture. It is calculated from geometric optics and is an  approximation at the paraxial focus. At focusing depths,


8T


other than the centric and aplanatic location, focal shifts


180008oogga 99


exist. This can change the objective NA, especially at large


)Normalized TIVA signal intensity (a.u.0.0-


angles. Fig. 8 shows that at regions close to the centric  location, a high NA is required for optimum resolution. This


0.00.51.01.5202.53.03.54.0


requirement reduces at greater depths such that an NA as  small as 0.23 is sufficient at the aplanatic location.


Although this plot shows the minimum NA required for  collection, degradations can occur if excess NA is used for  laser delivery. Fig. 9(a) shows the case when the light rays  are converged by the objective lens to within the aperture  opening. On the contrary, if the NA is in excess of  requirement, as shown in Fig. 9(b), there is truncation of the  geometrical cone of laser beam which results in power loss   and degradation of the  TIVA signal and reflected image  contrast. Therefore, too much excess NA is undesirable. The  NA should preferably be matched close to the minimum  requirement for optimum laser delivery.


Distance from centric location (μm)


Fig. 8. NA requirement and collection angle at various focal  depths.


合0


>


1200


10X(0.26 NA 20X(0.4NA)


50X(0.42NA


g>


Laser power:10-11 mW


(measured from respective objective lens)


RSIL Sample


吕


With RSILWithout RSIL


Fig. 9. Laser beam geometrical cone, within mechanical


gain (a.u.) signalTIVA peak20


aperture (a) and larger than mechanical aperture (b).


0-------------------


6080100120140150


D. Effect of RSIL parameters on imaging and TIVA 02040 enhancement


The key enhancement and degradation factors on TIVA


signals have been identified. We investigate the tradeoffs


between the laser spot size variation, SIL absorption and 0.75


--4-10X(0.26 NA)


objective NA matching at different designed focusing


-20X(0.4NA)


depths. Degradation due to laser beam truncation by the


-100X(0.5 NA)


0.70


--G-50X(0.42 NA)


objective pupil is normalized by using variable power for 0.6510X/16μm


Resolution measured from azimuthal 0


10--0


different objective lens to make sure that the resultant laser


power measured after objective lens is approximately 10-11


mW. Fig. 10 shows the peak TIVA signal at increasing focal 0.55 depths, from centric to aplanatic, for selected objective lens.


en0.50


eo


ds


a0.4550X/16μm


t


In general, power absorption from RSIL increases with 8


increasing focusing depths as thicker Si is required. 00.40 However, the main effects from the variation in TIVA peak 10.35esignal with focusing depths comes from the spot size


-8


variation and objective NA matching. Fig. 11 shows the 0204060801001201401601802000.3050X/165μmexperimental spatial resolution in imaging. It should be  emphasized that the resolution values were quantified based


on FWHM resolution. It can be experimentally proven that


the experimental observable resolution can vary from as


much as 30-38%. Although there are some differences, the


reflected laser image resolution is expected to be close to


that of laser spot size.


In Fig. 10, at region close to centric location, the highest


TIVA signal is achieved by 50X and 100X due to their small


laser spot size compared to 10X and 20X. The signal for


10X is the worst. The contrast and sharpness of the image


for 10X is too poor in the image and not quantified. For


optimization in this region, the higher the NA, the better will


be the signal gain.


With increase in RSIL thickness to focus at larger


depths, TIVA signal degrades from 50X and 100X because


the power loss from lens absorption is more significant than


the resolution enhancement. On the contrary, the signal from


10X and 20X increases because the resolution enhancement


is more dominant. When the focal depth increases further to


about 90-100 µm below centric location, the NA required for


collection starts to reduce to around 0.5. Laser beam


Distance from centric location (um)


Fig. 10. Change in TIVA signal enhancements with varying  laser focusing planes and objective NA.


Fig. 11. Experimental spatial resolution at various imaging  planes.


from excess NA becomes an issue from this point onwards. This is seen from the increased gradient in signal  degradation for 50X and 100X which is especially worse for  100X. Both 10X and 20X continue to achieve increasingly  good signal gain from their enhanced resolutions.


At region close to 135 µm, there is a peak in TIVA signal  from 20X objective as the resolution is close to the  minimum. This is more significant than the slight laser beam  truncation. At this point, the 10X is still not at its optimum  resolution. The increase in signal from 50X and 100X is  insignificant due to high laser beam truncation. When  focusing depths increase further to 150 µm, there is another  signal peak from 10X objective because of its enhanced  resolution enhancement. This peak is higher than the  previous one from 20X although it does not have a minimum  resolution better than 20X objective. This is because its  beam is not truncated due to its low NA. After this point, TIVA signal degrades drastically for all objectives. Therefore, at regions close to the aplanatic location, it is


better to use low objectives of 10X and 20X for NA  matching reasons. This is also important for imaging as well. A comparison between the reflected laser images captured at  16 µm and 165 µm as shown by insets in Fig. 11, reveals  that beam truncation by mechanical aperture can reduce the  laser power to an extent that contrast is significantly  affected.


It is clear that TIVA performance with RSIL application  is highly dependent on various parameters.  The success of  TIVA localization technique also depends on the spatial  resolution of reflected laser image for overlay. Although it  might seem that 10X can provide the highest signal gain, it  should not be the design target because of resolution  tradeoff. A weak TIVA signal due to power loss can be  overcome by increasing laser power delivery. The results in  this work are also applicable to the case of RSIL which is  formed directly on Si substrate [11].


V. CONCLUSION


This RSIL parameters that affect TIVA and imaging  enhancements has been discussed. The results have  highlighted the importance of RSIL design to maximize  performance both in TIVA and imaging. There is no single  optimum condition when applying RSIL. For design close to  centric location, a high backing objective NA is necessary. On the contrary, a low backing NA is required at locations  close to aplanatic. A too high objective NA will result in  degradations from beam truncation by the mechanical  aperture of RSIL. Although a low NA will give rise to  optimum TIVA signal, it is undesirable because of optical  resolution tradeoffs, affecting precise defect localization.


ACKNOWLEDGEMENT


The authors, SH Goh and ACT Quah are supported  jointly under the National University of Singapore (NUS) research scholarships and Chartered Semiconductor  Manufacturing graduate program grant. We would like to  acknowledge Li Lijuan from NUS for helping with sample  preparation. We also wish to thank Frank Zachariasse from  NXP semiconductors for the valuable discussions.


REFERENCES


[1] Phang JCH, Chan DSH, Palaniappan M, Chin JM, Davis B, Bruce M, Wilcox J, Gilfeather G, Chua CM, Koh LS, Ng HY, Tan SH, “A Review of Laser Induced  Techniques for Microelectronic Failure Analysis”, Proc  Int Symp Physical & Failure Analysis of Integrated  Circuits (IPFA 2004), 5-8 Jul 04, Hsinchu, Taiwan, pg  255-261, 2004.


[2] Aw SE, Tan HS, Ong CK, "Optical Adsorption  Measurements of Band-gap Shrinkage in Moderately  and Heavily Doped Silicon", J Phys: Condens Matter, Vol 3, No 42, pg 8213-8223, 1991.


[3] Mansfield SM, Kino GS, "Solid Immersion  Microscope", Appl Phys Lett, Vol 57, No 24, pg 2615-2616, 1990.


[4] Eiles T, Pardy P, "Liquid Immersion Objective for  High-Resolution Optical Probing of Advanced  Microprocessors", Proc Int Symp Testing & Failure  Analysis (ISTFA 2001), 11-15 Nov 01, Santa Clara, California, USA, pg 167-170, 2001.


[5] Zachariasse F, Goossens M, "Diffractive Lenses for  High Resolution Laser Based Failure Analysis", Proc  Int Symp Testing & Failure Analysis (ISTFA 2005), 6-10 Nov 05, San Jose, California, USA, pg 1-7, 2005.


[6] Ippolito SB, Goldberg BB, Uenlue MS, "Theoretical  Analysis of Numerical Aperture Increasing Lens  Microscopy", J Appl Phys, Vol 97, pg 053105-1-12,


2005.


[7] de la Bardonnie M, Ross R, Ly K, Lorut F, Lamy M, Wyon C, Kwakman LFTz, "The Effectiveness of  OBIRCH Based Fault Isolation for Sub-90nm CMOS  Technologies", Proc Int Symp Testing & Failure  Analysis (ISTFA 2005), 6-10 Nov 05, San Jose, California, USA, pg 49-58, 2005.


[8] Barta E, "Optical Constants of Various Heavily Doped  p- and n-type Silicon Crystals Obtained by KramersKrong Analysis", Infrared Physics, Vol 17, pg 319-329,


1977.


[9] Ippolito SB, Goldberg BB, Ünlü MS, “High spatial  resolution subsurface microscopy”, Appl Phys Lett, Vol 78, No 26, pg 4071-4073, 2001.


[10] Mitutoyo Corporation, "Microscope Units, Objectives, Eyepieces and Accessories", Catalog No E4191-378


[11] Koyama T, Yoshida E, Komori J, Mashiko Y, Nakasuji  T, Katoh H, "High Resolution Backside Fault Isolation  Technique Using Directly Forming Si Substrate into  Solid Immersion Lens", Proc Int Rel Phys Symp (IRPS  2003), 30 Mar 03 – 4 Apr 03, Dallas, Texas, USA, pg  529 - 535, 2003.


DOI: 10.1361/cp2008istfa007


High Current Focused Ion Beam Instrument for Destructive Physical Analysis  Applications


Paul Tesch, Noel Smith, Noel Martin, Doug Kinion


Oregon Physics LLC, Hillsboro, OR  USA  p.tesch@oregon-physics.com


Introduction


Conventional focused ion beams (FIB) employing liquid metal  ion sources (LMIS) are commonly used to create site specific  cross-sections for viewing subsurface features and performing  3D metrology on subsurface structures[1]. These FIB tools are  typically used to remove material with volumes from 0.1 µm3  to  1x104 µm3 with  high  cross-section  edge  placement  accuracy.   These  tools  are  very  effective  at  creating  crosssections  for  failure  analysis  or  yield  improvement  on  structures with dimensions below 25µm. For instance, LMIS  FIB  tools  commonly  create  cross-sections  for  measuring  critical dimensions on magnetic hard drive heads to optimize  production yields. LMIS FIB tools are also used to create thin  lamella  cross-sections  for  Scanning  Transmission  Electron  Microscopy analysis.   In both these cases the cross-sections  are typically less than 10 microns in any dimension.


Figure 1 shows a schematic drawing of a multilayer structure  with a planar surface before and after a wedge shaped volume  of  material  is  removed  to  expose  a  cross-section  of  the  multilayer structure.


Figure 1:  Schematic drawing of  multilayer  structure before   and after a wedge shaped volume of material is removed to   expose a slice through the multilayer structure.  The wedge of   material  is  removed  to  expose  a  planar  cross-section  for   imaging or metrology. The cross-section face is located at the   left edge of the stripes area.


In this figure the top two images show a side view and a top  view of a multilayer structure before any milling. The bottom  two images show a side view and a top view of  a multilayer  structure  after  the  wedge  shaped  volume  of  material  is  removed to expose the cross-section. The volume of material  that is removed is determined by the width and depth of the  cross-section. The third dimension of the wedge (horizontal in  Figure 1) scales with the depth dimension to allow the crosssection  face  to  be  imaged  at  an  angle.  The  typical  wedge  volume removed   for a 45 degree viewing angle is given by


Volume=0 .5⋅Width⋅Depth2 .


In  some  cases  the  geometry  of  the  structure  to  be  crosssectioned allows for less material to be removed. For instance  if the area to be viewed protrudes from the sample or is near  the  edge  of  the  sample,  then  it  is  not  necessary  to  mill  a  complete wedge to view the cross-section.


Figure 2 shows the geometry that is typically used for milling  and imaging the cross-section.  The FIB column that removes  the material is typically oriented perpendicular to the surface  of  the  sample.  After  the wedge of  material  is  removed the  cross-section  face  can  be  viewed  with  an  imaging  device  positioned at an angle to the cross-section face.


Column


Position for FIB


Side view of multilayer structure


Milling the Cross-section


Position for Imaging the Cross-section


Top view showing the surface of the structure


Side view of multilayer structure with a wedge of material removed to expose a cross-section.


crosssection


width


Top view showing the surface with a wedge of material removed. The exposed cross-section face is at the left of the red stripe.


Cross-section Face


Figure 2: Schematic drawing of the geometry typically used  for milling the wedge shaped volume and imaging the crosssection.  The FIB milling column is oriented perpendicular to   the sample. The imaging column is at an angle to the crosssection face.


Structures that are larger than 25µm are typically difficult to  analyze with a conventional FIB because with a 10nA/30keV  gallium beam, the mill rate of silicon (normal incidence) is  only 2.7 µm3/s. At this rate mill volumes greater than 1x104 µm3 can take more than an hour.  For instance a 65µm x 65µm  x 65µm (2.7x105µm3) cross-section would take over 10 hours  to complete with a 10nA/30keV gallium beam. Micro-ElectroMechanical  Systems  (MEMS),  three  dimensional  integrated  circuits  (3D-ICs),  optical  components,  and  semiconductor  packaging materials often require large volumes of material (greater  than  1x106 µm3)  to  be  removed  for  sub-surface  material inspection or chemical analysis.


Oregon  Physics  has  developed  a  new  focused  ion  beam  instrument  capable  of  creating  cross-sections  as  large  as  1  millimeter  in  size.  In  this  instrument,  a  radio  frequency  plasma ion source with an electrostatic matching lens has been  integrated onto a commercially available two lens electrostatic  FIB column to create a new FIB tool that can mill structures  from less than 100 nanometers to over a millimeter in size. This FIB instrument has been operated with a variety of gases  including Xenon, Oxygen, Argon and Helium and can produce  probe  current  from  tens  of  picoamperes  to  over  2  microamperes.  With  Xenon  at  4  microamperes  the  volume  removal rate is approximately 2000 µm3 per second for silicon  at normal incidence. Mill rates approaching 6000 µm3  have  been achieved for creating cross-sections. This removal rate is  nearly a 100 times faster than a 65nA LMIS FIB without gas  chemistry etch enhancement.


This high mill rate enables this tool to be used for  destructive  physical  analysis  (DPA)  in  emerging  applications.  For  instance,  this  tool  is  capable  of  creating  cross-sections  of  multiple stacked wafers and through silicon vias (TSVs) used  in  3D-ICs  as  well  as  large  IC  packaging  or  interconnect  structures.  These  emerging  applications  incorporate  new  materials  as  well  as  large  structures  that  interface  to  decreasing IC dimensions and often require DPA for process  development, quality control, and yield enhancement.


In this paper we describe the new high current FIB instrument, compare  it  to  the  existing  LMIS  FIBs,  and  show  several  examples that illustrate the capabilities of this tool.


Discussion


Radio-frequency  inductively  coupled  plasma  (ICP)  ion  sources  have  been  used  for  various  scientific  applications  since  the  1950's  [2].   These  sources  are  quite  simple  in  principle consisting of a wire coil with several turns wrapped  around a ceramic or quartz tube containing a low pressure gas. Figure 3 shows a schematic drawing of this source.


Figure  3:  Schematic  drawing  of  an  inductively  coupled   plasma  ion  source  showing  the  main  components:  a  coil   antenna wrapped around a quartz or ceramic tube containing   a low pressure  gas, a source electrode with a aperture, an   extractor electrode, and a RF power supply connected to the   coil.


A  radio frequency (RF) power supply generates an alternating  current  in  the  coil  antenna  which  produces  a  time  varying  magnetic field in the low pressure gas. Through Faraday's law  of  induction,  a  time  varying  azimuthal  electric  field  is  produced  causing  an  azimuthal  current  in  the  low pressure  gas.  This  radio  frequency  electric  field  couples  energy  efficiently  into the plasma electrons but does  not accelerate  the ions because of the large mass difference between the ions  and electrons. The efficient coupling to the plasma electrons  produces  a  high  density  plasma  with  high  electron  thermal  energy but very low ion thermal energy. The combination of  the high plasma density and low thermal ion energy results in  a high brightness for ions extracted from the plasma.  Practical  inductively  coupled  ion  sources  are  typically  much  more  complex because they include shielding to reduce  capacitive  coupling between the coil and the plasma as well as insulation  so the RF electronics can be referenced to ground potential  instead of the source anode. Oregon Physics has developed a  RF ICP ion source (the HyperionTM source) that is specifically  designed  for  producing  micro  and  nano-probes  on  FIB  systems.


The performance of an ion source for forming probes at the  nanoscale and microscale is determined by the source's virtual  source  size,  angular  intensity,  and  axial  energy spread.  The  HyperionTM  source has much lower  virtual  source size and  axial  energy spread than other  common plasma ion sources  such as the Duoplasmatron and Penning sources allowing the  HyperionTM source  to  produce  much  higher  current  density  micro-probes and nano-probes than other plasma sources. The  HyperionTM source  has  much  larger  virtual  source  size  and  angular intensity than the Gallium LMIS. This results in the  LMIS having higher current density for nanoscale probes but  the  HyperionTM source has  much higher  current  density  for  microscale probes. Table 1. shows the key source parameters


for the  Xenon HyperionTM


source and two common sources


used for FIB milling.


Table 1: Source parameters for the Xenon HyperionTM source,  the Gallium LMIS , and the Argon Duoplasmatron source.


100000


||Xenon HyperionTM |Gallium LMIS |Argon Duoplasmatron |
|---|---|---|---|

|Virtual Source Size (microns) |13 |0.05 |50 |

|Angular Intensity (mA/ Steradian) |18 |0.02 |10 |

|Axial Energy |4-6 |5 |15 |

|Spread (eV) |4-6 |5 |15 |

|Source Brightness (A/m2/stera dian/V ) |13,000 |1,000,000 |1,100 |

Ga LMIS FIB


Xe Plasma FIBAr Duoplasmatron


10000


1000


(nm Size Probe100


10cccmlrcml--lCrorml-sal


0.010.11101001000 Probe Current (nA)


)


Focusing columns with electrostatic lenses are used to create  finely  focused  probes  for  milling  applications.  Ga  LMIS  columns  typically  utilize  two  electrostatic  lenses  to  create  probes  due  to  their  nanoscale  virtual  source  size.  While  plasma  sources  typically  use  three  lenses  in  order  the  demagnify  the  microscale  virtual  source  size  to  produce  optimized  probes  at  the  nanoscale.   Figure  4  shows  a  schematic drawing of the three lens focusing column used to  produce sub 50nm size probes with the HyperionTM source.


Figure 4: Schematic drawing of a three lens column used to   demagnify  the  microscale  virtual  source  of  the  HyperionTM  source  to  achieve  nanoscale  probes.  Typically  a   demagnification of ~400 is required to reach sub 50nm size  probes.  This  optics  configuration  produces  a  large  angular  magnification to produce the necessary demagnification of the   source object.


Figure 5 shows the simulated probe size versus current for the  three sources when operated on a 30 kV focusing column. The  column  has  three  lenses  for  the  Duoplasmatron  and  HyperionTM sources but only two lenses for the Ga LMIS to  run under optimized conditions.  Each focusing lens  has  the  same  aberration  coefficients  with  spherical  aberration  coefficient  (Cs)  of  900mm  and  chromatic  aberration  coefficient (Cc) of 105mm. The Ga LMIS has higher current  density for probes below 430nm in size. However at higher  current the performance of the Ga LMIS rapidly falls off from


spherical aberrations due to the low angular intensity of the  LMIS.  The  HyperionTM


source  outperforms  the  Duoplasmatron source at all currents and outperforms the Ga  LMIS for probe sizes above 430nm.


Figure 5: Simulated performance comparison for Ga LMIS,  Xenon  HyperionTM,  and  Ar  Duoplasmatron  sources  on  a   focusing  column  with  aberrations  of  Cs=900mm  and  Cc=105mm in each lens. The source parameters  from Table 1   were used in the simulation. This plot shows that the Ga LMIS  has the highest current density for probe sizes below 430nm  but the Xenon ICP source has superior performance at larger   probes sizes.


The performance of a FIB system for creating cross-sections  of a given size for destructive physical analysis applications  depends on the probe current density and the sputter rate of  the ion probe. The sputter rate (volume removed for a given  ion  dose)  is  much  higher  for  Xenon  than  Gallium.  For  instance,  the  silicon  sputter  rate  for  30kV  ions  is  0.43 µm3/nanoCoulomb  for  Xenon  but  only  0.27 µm3/nanoCoulomb for Gallium.


Oregon Physics has developed a focused ion beam instrument  where  the  HyperionTM ion  source  with  an  electrostatic  matching  lens  has  been  integrated  onto  a  commercially  available two lens electrostatic FIB column to create a new  FIB  tool  that  can  mill  structures  from  less  than  100  nanometers to over a millimeter in size. This FIB instrument  has been operated with a variety of gases including Xenon, Oxygen,  Argon and  Helium and can  produce probe current  from  tens  of  picoamperes  to  ~4  microamperes.   The  HyperionTM source  produces  over  ~20  microamperes  of  current with Xenon but the FIB column is limited to several  microamperes of current in its current configuration. This new  FIB tool  has  been used   to  create a  large variety  of  crosssections  for  destructive physical  analysis  applications.   The  high probe current density of this tool at high current makes it  well suited  for creating large cross-sections. Figure 6 shows  the rate at which a wedge shaped volume with equal width and  depth can be created as a function of the width/ depth for the  Xenon plasma FIB instrument and for a traditional  Gallium  FIB. The time required to mill the wedge in Silicon is plotted


as a function of the cross-section size taking into account how  the current scales with probe size and the sputter rate of the  different  ion species.   It  is  assumed that  the probe size  is  1/40th of  the  cross-section  width  for  each  of  the  different  widths on the graph.  Typically probe sizes of 1/25th to 1/100th  of the cross-section width are used to make a cross-section. Using  a  smaller  probe  size  typically  improves  the  surface  quality of the cross-section but increases the milling time. The  probe  size  was  calculated  using  the  same  parameters  and  assumptions as Figure 5. If a column with higher performance (lower aberrations) were used, it would reduce the mill time  but the improvement for both sources would be similar. Figure  6 shows two curves for each of the sources. One curve shows  the performance with currently available column technology. The  second  curve  which  is  labeled  “Extended”  shows  the  performance that could be achieved if the current is increased  to what can practically be achieved with the specified source  and column technology.


Figure  6:  Simulated  milling  time   as  a  function  of  crosssection size for a Gallium LMIS and a Xenon ICP  sources on  a  focusing  column  with  aberrations  of  Cs=900mm  and  Cc=105mm in each lens. The source parameters  from Table 1   were  used  in  the  simulation.  The  current  used  to  mill  the   different cross-section sizes is determined by the current in a   probe  size that is 1/40th of the cross-section width.


Figure  6 shows that  the  Ga LMIS FIB is  very  effective  at  making  cross-sections  below  10  microns  in  size.  However, cross-sections above ~12 microns are completed much faster  with the Xenon ICP FIB. The  Xenon  HyperionTM FIB can  remove  material  for   cross-sections   that  are  hundreds  of  microns in size in less  than an hour where it  would take a  Gallium FIB approximately 100 hours to complete the same  task.  The rate at which the Gallium LMIS FIB can mill large  cross-sections  is  limited by spherical  aberrations  due to  the  relatively low angular intensity of the LMIS.  For the largest  cross-sections, the Xenon plasma FIB is limited by the column  rather than the source. The existing column is limited to about  3  microAmperes  and  a  modified  column  design  could  accommodate  35  microAmperes.  This  extended  Xenon  HyperionTM FIB would be able to create 1mm cross-sections  in  less  than a work day where the extended Ga LMIS FIB  would take over 3000 hours.


The cross-sectioning rate was analyzed for the case where a  wedge is removed from a sample with a planar surface. Even  higher cross-section rates can be achieved if  the cross-section  location protrudes from the sample or is near the edge of the  sample. In these cases it  may not be necessary to remove a  wedge  to  view  the  cross-section  because  a  cut  shape  with  lower volume may allow the cross-section to be viewed with  an  imaging  column.   Also  the  sputter  rate  is  higher  near  sample  edges  or  with  protruding  samples  because  there  is  much less redeposition of sputtered material in the pattern area  for these geometries than with a wedge geometry. However, samples  with  protruding  structures  typically  accumulate  redeposited material on the surrounding structures outside the  pattern  area.  In  the  case  of  the  wedge,  some  material  is  redeposited into the  area being milled slowing the  removal  rate,  while  most  of  the removed material  is  sputtered away  from the sample.


10000-□- Gallium LMIS FIB (Max current 65 nanoA)


In  addition  to  having  a  higher  sputter  rate  than  Gallium,


-0-Xenon ICP FIB (Max current 3 microA)


Xenon has a number of other benefits for milling applications.


1000AExtended Xenon ICP FIB (Max current 35 microA)今Extended Gallium LMIS FIB (Max current 160nanoA)


Xenon  is  an  inert  gas  at  room  so  it  undergoes  very  little  chemical  reaction  with  the  sample.  Also  unlike  Gallium, Xenon deposited into the damage layer during the sputtering  process  does  not  substantially  change  the  sample's  conductivity.  Xenon has  lower penetration depth and lateral  range  than  Gallium  at  a  given  ion  energy  so  the  sample  damage layer from ion beam milling process is thinner with


Milling Time (Hours)古00


the  Xenon  beam.  Table  2  shows  the  results  of  a  SRIM


0.1


calculation [3] for the stopping range of Gallium and Xenon at  normal incidence in Silicon for 30 keV and 14 keV ion energy.


0.01


The  damage  layer  thickness  produced  by  the  ion  beam


1


10


depends on the angle of incidence but is  approximately the


Cross-section Size (Microns)


longitudinal  range  for  ions  at  normal  incidence.  The  ion  energy of 14 keV was chosen because the sputter yield of the  14 keV  Xe ion  is the same as the 30keV Ga ion.  The Xenon  ion  will  produce  a  damage  layer  approximately  half  the  thickness  of  Gallium when operating with the  same sputter  yield.


Table 2: Calculated ion range in silicon using SRIM at 30 keV   and 14 keV ion energy for Xenon and Gallium.


||Species |Longitudinal range( nm) |Radial  Range (nm) |Sputter Yield (atoms/ion) |
|---|---|---|---|---|

||30 keV Xe |23.7 |6.8 |2.9 |

||30 keV Ga |28.1 |10.2 |2.2 |

||14 keV Xe |15.1 |4.5 |2.2 |

||14 keV Ga |16.3 |6.2 |1.8 |

Example Applications


The high volume removal rate of the Xenon ICP FIB can be  applied for failure analysis and process evaluation in emerging  technologies such as 3D integrated circuits (3D-IC). In 3D-ICs  vertical die stacking is used to integrate different functional  layers  with  short  interconnect  lengths  to  improve    the  performance and allow for higher density.  Figure 7 shows a  cross-section of a  STMicroelectronics Real Time Clock that  has 2 stacked dies on a copper heat sink. This  900 micron by  300 micron cross-section would take days to complete on a Ga  LMIS FIB but was completed in less than 1 hour with a  3  microAmpere Xenon beam.


Figure 7: Image of a 300 micron by 900 micron cross-section   of a  STMicroelectronics Real Time Clock  device. The crosssection was created with a  3 microAmpere Xenon beam and  the  image was taken with a 100pA Xenon beam tilted at 45  degrees angle. This cross-section was created in less than one   hour.


This  cross-section  exposed  interfaces  between  the  different  layers that can be images at high resolution. Figure 8 shows  images taken at the interfaces.


Upper Die


Figure 8: Images of the interfaces exposed in a cross-section   of a STMicroelectronics Real Time Clock. The top left image  is  the  interface  between  the  two  wafer  dies.  The  top  right   image was taken at  the interface of  the bottom die and the   copper heat sink. The bottom center image was taken at the


Lower Die900μm


interface of the copper heat sink with the base substrate.


In the top left image of this figure it is possible to see small  structures  in  the  boundary  layer   between  the  two  stacked  wafer dies.  It is also possible to view the grains in the copper


Copper Heat Sink


heat sink and the base layer.


These 3D-ICs often use  large “through silicon vias” (TSVs) to interconnect the different dies. These TSVs can be several  hundred microns deep and are too time consuming to analyze  with a conventional Ga LMIS FIB. Figure 9 shows a Ga LMIS  FIB image  taken of a 100 micron by 20 micron  copper TSV  that was milled with the Xenon  ICP FIB.


I-BeamMagDetFWDPAHFWTit


20μm


30.0 kV1000 XCDM-E 16.5102152 μm0.0°


Figure 9. Ga FIB image of a 100micron by 20 micron TSV  that was course milled with a 1.5 microampere  Xenon beam  and fine milled with a 100 nanoAmpere  Xenon beam.


Figure 10 shows an image of a TSV that has an incomplete  copper fill. A large void can be seen near the top of the image  and the copper grain structure can be seen.


I-BearnMagDetFWDpAHFWTilt


10 μm


30.0 kV 2.50kX CDM.E 16.511160.8 μm00


Figure 10. Image of a TSV that has an incomplete copper fill.  A large void can be seen near the top and the copper grain   structure can be seen. This cross-section was milled with the   Xenon ICP FIB using a 1.5 microampere beam for the course  cut and a 100nA  beam for the final polish cut.


Figure 11 shows a backscattered secondary electron image of  the bottom section of the TSV shown in Figure 9.  This image  provides good contrast to view the small voids located near  the bottom of the TSV. In the previous image it was difficult  to  differentiate  the voids  and  the dark copper  grains  in  the  image. Scalloping on side walls from the Deep Reactive Ion  Etch process used to create the deep holes can be seen on the  edge of the TSV.


Figure 11. Backscattered secondary electron SEM  image of   the  TSV   shown  in  Figure  10.  This  image  provides  good   contrast to view small voids located at the bottom of the TSV.


A third example is the cross-section of a 750 micron solder  ball from a ball grid array of a RM7000-266T microprocessor  package shown in Fig 11.  This  cross-section  was milled  in  about 6 hours with a 1.7 microampere beam.


Figure 12.  Cross-section  image showing a 750 micron solder   ball from a ball grid array of a RM7000-266T microprocesser   package.  The  cross-section  was  milled  with  a  1.7  microampere Xenon beam while the image was taken at 45 degrees   of tilt with a 100 picoampere Xenon beam.


Even though a  high current was used for creating this crosssection,  fine  details  at  the base  of  the  cross-section  can be  seen. Figure 13 shows a close up of the  interface between the  solder ball and the under bump metallization pad. Submicron  features  can easily  be identified.  The Nickel  interface layer  between solder ball and the underlying copper can be seen as  well as a small gap between the solder ball and the package  passivation layer.


Sn-Pb~700nm


Passivation


Ni


Cu


Package


Figure 13. Image of the interface between the solder ball and


E39amMagDetFWD| SpotHFWTilt


the under bump metallization layer pad from the solder ball


5μm


5.00 kV6.50kX TLD-B 5.145423.4 μm52.0°Semion LLC


cross-section shown in Fig 12.


Conclusions


A new high current FIB instrument has been developed that is  capable  of  creating  large  cross-sections  for  destructive  physical analysis applications. An inductively coupled plasma  ion source was integrated onto a conventional FIB column to  create a tool that is useful for creating cross-sections from 10  microns to 1mm in size. The tool retains the benefits of the  conventional LMIS FIB such as high placement accuracy for  the  cross-section  location  and  the  ability  to  immediately  obtain  high  resolution  images  of   the  cross-section  face  without having to transfer it to another tool. However, this tool  is capable of creating very large cross-sections at a rate about  100 times faster than a conventional FIB. The cross-sections  created  with  this  tool  have  high  quality  and  enable  useful  imaging  for  DPA  applications.   Critical  dimensions  of  subsurface  features  can  be  accurately  measured.  Process  problems such as unwanted voids or poor adhesion between  layers  can  be  identified  from  these  cross-sections.  This  capability  has  the  potential  to  be  very  useful  in  emerging  technologies such as 3D-ICs that have large scale structures.


Acknowledgments


The  authors  would  like  to  acknowledge  Kevin  Filter  of  Semion LLC for his gracious support in providing several of  the  images used in this paper.


References


[1] Orloff,  J,  et  al,   High  Resolution  Focused  Ion  Beams, Kluwar  Academic/ Plenum Publishers (New York, 2003).


[2] Thonemann,  P.  C.,   Progress  in  Nuclear  Physics, Pergamon Press (London, 1953), pp. 219.


[3] Ziegler, J. F. et al, SRIM The Stopping and Range of Ions  in Matter, SRIM Co, (2008)


DOI: 10.1361/cp2008istfa014


Recent developments in TEM applications for the IC industry


L. F. Fu, Y. C. Wang, B. Jiang, F. Shen, M. Strauss, B. Van Leer, C. Senowitz, and A. Buxbaum


FEI Company, 5350 NE Dawson Creek Drive, Hillsboro, OR 97124, USA  Lianfeng.fu@fei.com


Recent developments in aberration-corrected transmission  electron microscopy have drawn much attention from the  semiconductor characterization community. Two new  developments in transmission electron microscopy, image  aberration correctors and probe aberration correctors, are  discussed in term of their applications in characterizing gate  oxide dielectrics for the IC industry.


Continuing device scaling reductions in integrated circuit (IC) industries, e.g. to 45nm node or beyond, require precise  determination of film thickness, interfacial roughness, and  chemical distribution. High resolution transmission electron  microscopy (HRTEM) has been considered as a fast and  reliable method to characterize the nanostructure of the IC  devices and measure individual thin film layer thickness [1-4]. However, due to the imperfection of magnetic lenses in the  electron microscope, e.g. the spherical aberration of the  objective lens, the interpretable spatial resolution in the  microscope is limited [5]. Moreover, the lens aberrations lead  to a blurring effect, referred to as contrast delocalization, for  non-periodic structures such as interfaces, edges, and defects


[6]. As a result, the image details of these structures are  displaced from their true locations. This problem limits the  accuracy of layer width measurement and becomes more  serious when the physical width of oxide gate dielectrics in IC  devices shrinks down to below 2nm. The new generation of  commercially available aberration corrected electron  microscopes reduce objective lens spherical aberrations and  therefore minimize delocalization. At the same time, the  correction of the spherical aberration moves the point  resolution to the information limit; therefore, it dramatically  improves usable image resolution. It thus becomes possible to  obtain directly interpretable and atomically sharp images with  sub-Angstrom resolution.


The modern transmission electron microscopy (TEM) tools  are also capable of scanning a small and focused electron  probe on the sample, using scanning transmission electron  microscopy (STEM) mode. A STEM microscope equipped  with a HAADF (high-angle annular dark field) detector allows  the acquisition of atomic resolution images where the contrast  is directly related to the atomic number Z. Systems with probe  aberration correctors are also commercially available. The  probe-corrected STEM system enhances not only the STEM  resolution but more significantly, increased the beam currents


[5]. The high beam current also benefits the atomic scale  analysis in terms of available signal.


In this paper, we first describe the physical background of  delocalization and the basic concept of an image corrector and  a probe corrector. Then, we present the microstructure  characterization results from the gate oxides in the current IC  industry on a conventional electron microscope. The results  are compared with the data obtained on an image aberrationcorrected microscope and a probe aberration-corrected  microscope to illustrate the benefits of aberration-correction.


Background  Contrast delocalization


Contrast delocalization means that image details are blurred  and displaced from their true locations in the specimen. Physically, it can be understood as the lateral displacement of  spatial frequencies in the image. This displacement increases  significantly with spatial frequency. It is rarely a problem on  LaB6 microscopes due to their limited coherence in  illumination. However, it is a prominent imaging artifact in  HRTEM images acquired from field emission gun (FEG) microscopes due to their high coherence which leads to a  strong contribution of the high spatial frequencies. This  blurring effect becomes most easily recognizable at nonperiodic structures in materials, such as interfaces, boundaries, edges, and defects. Depending on the spatial frequencies and  the selected defocus, the contrast delocalization can extend up  to several nanometers. Otten et al. and Lentzen et al. have  extensively studied this effect [7, 8] and given a mathematical  expression for the delocalization ∆R


∆R=λg (∆f+Csλ2g2),                                                              (1) where λ is the electron wavelength, g the spatial frequency, ∆f  the defocus and Cs the spherical aberration of the objective  lens.


Figures 1(a) and 1(b) show typical examples of such a blurring  effect on BaTiO3 thin films including multiple twin variants  viewed along the [110] direction, which was reported by Jia et  al. [9]. Both images were acquired on a Philips CM20 ST FEG  electron microscope (Cs=1.2mm). The image acquired at  smaller defocus (-137nm) shows less blurring at the twin  interface than the image acquired at larger defocus (-225nm). However, it is obvious that both images make contrast  interpretation and interface analysis impossible by eye. Image  simulation procedures based on these interfaces are extremely


difficult since the strong contrast delocalization prevents a  good guess at a structure model input for simulation.


Figure 1:  (a) HRTEM image of Σ3 twin boundaries in BaTiO3  at defocus of -137nm (adapted from reference [9]). The arrow  denotes the contrast delocalization (b) HRTEM image of Σ3  twin boundaries in BaTiO3 at defocus of -225nm. (c) HRTEM  image of a gate dielectric at defocus of -67nm. (d) HRTEM  image of a gate dielectric at defocus of -120nm.


More typical examples for IC applications are shown in Figs. 1(c) and 1(d). These two HRTEM images are acquired from a  65nm node technology gate oxide on a FEI TecnaiTM F20  electron microscope equipped with a S-Twin objective lens (Cs=1.2mm) at two defocus values, -67nm and -120nm. It is  clear that the left image which is focused close to Scherzer  defocus has a less blurred Si/SiO2 interface than the right one, meaning less delocalization. Scherzer defocus is given by ∆fsch=-1.2 λsC  and it allows one to image a wide band of  spatial frequencies at nearly the same phase shift. However, the point resolution obtained at this focus is still lower than the  information limit, which is limited by spatial and temporal  coherence of the electron source. Up to the point resolution, the delocalization at Scherzer defocus can be determined as ∆Rsch=38


1−


sch


g =384


3


16


3 λsC [8]. Using the wavelength at  200kV and Cs=1.2mm, the delocalization at Scherzer defocus  is about 0.65nm. This calculation indicates that even at  Scherzer defocus the amorphous SiO2 width of gate oxides  measured by conventional HRTEM can be estimated off by


0.65nm. This measurement offset can be worse with other  focus settings.


Over years, different methods of hardware correction and  software correction have been developed to minimize this  imaging artifact, e.g. correction of objective lens spherical  aberration using a corrector [5, 10], focal-series reconstruction


[1], and off-axis holography [11]. The latter two methods can  retrieve the exit-plane wave function of the specimen and  obtain a true image free from most imaging artifacts. However, in both cases, the increase of the radiation damage  to the specimen or time-consuming post-acquisition process  can be a concern for high through-put demands in IC  industries. In contrast, the hardware correction, aberration  corrector electron microscopes developed recently can  overcome this problem very efficiently. The method and its  importance are discussed in the next section.


Aberration Correctors


Since the invention of TEM by Knoll and Ruska 76 years ago, the aberrations in round electromagnetic lenses have been  studied intensively. Scherzer proposed in his 1936 paper that  the two major axial aberrations of electron lenses, chromatic  aberration and spherical aberration, could be corrected by a  combination of various corrected lenses [12]. Following his  proposal, many researchers have spent a substantial amount of  time in designing such a system in practice [5, 6, 10]. In the  last four years, TEM systems both suitable for and equipped  with correctors compensating for the aberrations have finally  become commercially available. Correctors are made for two  applications: one for the probe-forming (condenser) or  illumination system of the system, called a probe corrector, and another for the image forming (objective) part of the  system, called an image corrector. Double-corrected systems  with both image and probe correctors integrated in one column  have also been implemented. If we consider the rotational  symmetry of the multipole elements that the correctors use, there are two classes of aberration correctors available, the  hexapole-sextupole corrector and the quadrupole-octopole  corrector. For image correctors, the hexapole-sextupole design  is dominant in the market. For probe correctors, both classes  of corrector designs exist in the market and have been proven  successful in compensating for spherical aberration. Currently  there are designs for a chromatic aberration corrector, which  will be primarily based on a quadrupole-octopole corrector  according to Rose [10].


The FEI TitanTM 80-300 [Fig. 2(a)] is a versatile platform that  can accommodate either an image corrector or a probe  corrector or both, with its newly designed column for 80-300  kV operation, constant power and three-condenser system. FEI  closely collaborates with CEOS GmbH and adapts their dual  hexapole type spherical aberration Cs corrector for both image  and probe correctors. A schematic diagram is shown in Fig. 2(b) to show how correctors work. The image corrector is  placed between the lower pole piece of objective lens and  projection lenses. The first hexapole of the image corrector  deforms the beam. Then this deformed beam is projected into  a second hexapole that compensates for this deformation  leaving only a higher order effect. This effect acts as a  negative Cs so that the electron scattered farther away from


2nm


(d)


the center leaves the corrector in a way seemingly like coming  from a point source close to the center. In this way, the  positive Cs in the objective lens can be compensated. The  aberrations of the two components are simply added together; thus, the total Cs of the two modules can be tuned to desired  values, e.g. close to 0. From the equation (1), it is not difficult  to see that the contrast delocalization can be strongly reduced. At the right defocus, the delocalization can be theoretically  reduced to values less than one angstrom or even to 0.


Figure 2: (a) Image of a FEI TitanTM 80-300 TEM/STEM  microscope (b) Ray path through the hexapole Cs-corrector  consisting of two hexapoles. Figure courtesy of Dr. S. Uhlemann, CEOS GmbH. (c) 1D phase-contrast function  curve to show the benefit of an image-corrector Titan by  moving the point resolution (~1.9Å) to the information limit (~0.9Å).


In addition, the reduced objective lens aberration in the image  corrector moves the point resolution to the information limit  and thus the final directly interpretable resolution is  determined by the information limit [Fig. 2(c)]. As a result, it  dramatically improves usable HRTEM image resolution, only  if the information limit of the base system is suitably  excellent. The images of irregularities in a crystalline material  such as interfaces, boundaries, edges, and defects can be  imaged more clearly and be interpreted intuitively as a result. A typical example of Au nanotwins is shown in Fig. 3. For IC  applications, the α-SiO2 gate oxide width at the interface Si/αSiO2/poly-Si can therefore be measured more precisely.


The probe correctors work in a similar way. However, different from the image correctors, the probe correctors are


placed between the condenser lens and the upper pole piece of  the objective lens. The aim of the probe corrector design is to  improve the atomic scale STEM imaging and analysis which  require the smallest probe with the highest probe current for  good signal-to-noise ratio. The STEM resolution is primarily  determined by the probe size and current, and by beamspecimen interaction. For a thin sample, the latter is less  dominating in STEM resolution than the former two. The  probe size is principally determined by four factors: spherical  aberrations, chromatic aberrations, the source brightness, and  noise effects. The reduced spherical aberrations in the probeforming system can prominently reduce the probe size and  increase the size of the aberration-free sweet spot (the flat area  in the Ronchigram [13]) on the condenser aperture plane by a  large factor. The size of the aberration-free plane in the  Ronchigram limits the size of the largest usable condenser  aperture. Therefore, care should be taken to select the correct  aperture; otherwise probe aberrations will negatively affect  analytical cleanliness. An acceptable analytical probe is not  necessarily determined by the spots present in a fast Fourier  transform, and hence care must be taken when probe current  vs. probe size measurements are made.  The condenser  aperture limits the half convergence angle of an illumination  system. The probe current is given by


I=


4


/


2 απ sourcedB ,                                                            (2) where B is the source brightness, dsource the demagnified  source size, α the half convergence angle [14]. With the  increased usable half convergence angle in the aberrationcorrected illumination system, the probe current can be  increased at least four times better than an uncorrected  microscope. The reduced probe size and increased probe  current can greatly enhance the spatial resolution in atomic  scale STEM imaging with much better signal to noise ratio. This is exemplified by the clearly resolved Si [110] dumbbells  in Fig. 4. The inset FFT shows information in the image  extended to 0.96 angstrom.


Figure 3: Aberration-corrected HRTEM images showing the  atomically sharp details of twin-structures in Au  nanoparticles. Figure courtesy of Anna Carlsson, FEI  Nanoport Acht.


Figure 4: Aberration-corrected HR-STEM image of Si (110) showing the well separated Si dumbbells. The inset FFT  clearly shows the 0.96Å resolution (circled).


Results and discussions


Gate Oxide Characterization on an Uncorrected TEM


As the modern IC transistors scale down to below 65nm and  gate oxide thinner than 2nm, precise measurement of the gate  oxide width becomes more challenging. To obtain a high  quality HRTEM image, it is critical to obtain a suitably thin  and flat TEM specimen. Moreover, according to Akatsu and  Odomahari’s work [15], HRTEM images can make a rough  interface appear smooth when the film thickness exceeds the  roughness correlation length (typically 5-10 nm). Therefore, a  good TEM specimen is essential to ensure a precise  measurement of the gate oxide width.


tial to ensure a precise  measurement of the gate oxide width.


|2nm 2nm 2nm (a) (c) |2nm 2nm (b) (d) |
|---|---|

Figure 5: (a) HRTEM image of gate dielectrics with a 70nm  thickness (b) HRTEM image of a 40nm-thick sample. (c) HRTEM image of a 30nm-thick sample. (d) HRTEM image of  a 20nm-thick sample.


A series of TEM specimens of gate oxides with different  thicknesses were intentionally prepared using the focused ion  beam (FIB) milling method on a FEI HeliosTM NanoLab 400S  DualBeamTM system. Figures 5(a)-(d) show the series of  HRTEM images with different sample thickness acquired on  FEI TecnaiTM F20-ST. The specimen thickness was estimated  using energy filtered TEM techniques. As shown in (a)-(c), the  samples with a thickness larger than 20nm show an obvious “black band” along the gate oxide interface. Principe et al. [1] think that this black band occurs when the local sample  thickness is greater than the extinction distance. This artifact  should be overcome by making thinner samples in order to  achieve the required high quality HRTEM data. Figure 4(d) shows the sample with a thickness of 20nm after the surface  was polished with 2 keV Ga+ ions following the low energy  FIB milling approach reported by Giannuzzi et al. [16]. It can  be seen that the black band is substantially minimized and this  sample thickness is thin enough for high-resolution imaging of  this scale of structure.


Figure 6: (a) BF-TEM image of a 65nm-node technology logic  device (b) STEM image of the same region (c) HRTEM image  of the gate oxide. (d) HR-STEM image of the gate oxide.


Figures 6(a) and (b) show the Bright-field TEM and High  angle annular dark field (HAADF) STEM image of a 65nmnode technology logic device. The nickel silicide gate, source  and drain contacts show brighter contrast in the STEM image  due to higher atomic number relative to Si substrate or polySi. Figures 6(c) and (d) show the HRTEM and HR-STEM  images acquired at the gate oxide region with a transmission  thickness of 20-30nm for the gate oxide width measurement. HRTEM images were focused close to Scherzer defocus. The  dashed lines on the HRTEM image denote the interfaces used  for the width measurement. The dashed lines on the HRSTEM image denote the interfaces determined from inflection


2nm  50nm


1nm


points on the STEM intensity traces across the interfaces, following the approach of Diebold et al. and Muller’s work [3, 4]. Figures 7(a) and (b) show the statistic column diagrams of  the width measurement based on HRTEM and STEM. The  statistic analyses from HRTEM and STEM give the gate oxide  widths of 1.80nm±0.07nm, 1.82nm±0.06nm. Electron energy  loss spectroscope (EELS) and energy dispersive X-ray (EDX) line scans were performed simultaneously across the Si/αSiO2/poly-Si interfaces. EELS line profile analysis on oxygen  K edge and EDX analysis on oxygen K line, which are  calculated from full width at half maximum (FWHM), give  the gate oxide widths of 1.86nm±0.08nm and


1.90nm±0.10nm, respectively.


Gate Oxide Characterization on a Corrected TEM


The same gate oxide sample with similar transmission  thickness 20-30nm has been studied on an image-corrected  FEI Titan 80-300 microscope at 300kV. A typical aberrationcorrected HRTEM image of gate oxide is shown in Fig. 8(a). The thin area in the image is quite flat and clean. The lattice  image is sharp and clearly shows Si [110] dumbbells which  have a separation of 1.36 Angstroms. As the image shows, aberration correction greatly minimizes the contrast  delocalization and clearly reveals the atomic scale details of  the Si/α-SiO2/poly-Si interfaces. After all the artifacts from a  non-zero amount of aberration (Cs≠0) are removed or  minimized, the resulting HRTEM images can be used to get a  more precise gate oxide width measurement. Fig. 8(b) shows  the statistic column diagram of the width measurement based  on image-corrected images. The statistic analysis gives the  gate oxide width of 1.83nm±0.04nm.


Figure 7: (a) Column diagram of the gate oxide width  distribution measured by HRTEM. (b) Column diagram of the  gate oxide width distribution measured by HR-STEM.


As a comparison, the same gate oxide sample has been studied  in the STEM mode on a probe-corrected FEI Titan 80-300  microscope at 300kV. Using the unique spectrum imaging  acquisition mode whereby simultaneous image detail, EELS


and EDX line scans are taken across the Si/α-SiO2/poly-Si  interfaces, all the required data are obtained at once. Figure  9(a) shows a typical aberration-corrected HR-STEM image of  a gate oxide. The aberration-corrected probe is small enough  to resolve the Si [110] dumbbells. The inset FFT indicates  transfer of contrast out to d224=0.11 nm. The corresponding  column diagram from statistic analysis is shown in Fig. 9(b). The analysis result gives the gate oxide width of 1.84 nm±0.04  nm.


Figure 8: (a) Image-corrected HRTEM image of the gate  oxide sample. (b) Column diagram of the gate oxide width  distribution measured by HRTEM.


Discussions


The results presented above show that the improved resolution  after aberration correction can clearly reveal individual atom  column and therefore ensure more precise measurement of  gate oxide width. Besides the improved resolution, aberration  correction minimizes conventional FEG-TEM imaging


1.76


1.80


1.84


1.88


0 5 10 Number of measurements15 20


Width (nm)


1.65 1.70 1.75 1.80 1.85 1.90 1.95 0


measurementsNumber of5


15


20


25


W i d t h [ n m ]


1.74 1.76 1.78 1.80 1.82 1.84 1.86 1.88 1.90


0 Number of measurements5 10 15 20 25


Width [nm]


artifacts such as contrast delocalization. Therefore, image  corrected HRTEM imaging measurements surpass the  uncorrected image measurements of the gate oxide by 0.3nm  with a better statistical precision of 0.04nm. The uncorrected  STEM measurements are close to the probe-corrected STEM  measurements. The reason is that in STEM HAADF images  are amplitude images and not phase contrast images. They are  direct images of the crystal lattice and provide a one-to-one  correspondence between the atomic images and the position of  atomic columns. In addition, the contrast reversal problem  with defocus or thickness in TEM imaging does not occur in  STEM HAADF imaging. The recorded intensity in the STEM  image is a map of the atomic scattering factor and closely  related to the atomic number; which is why it is also referred  to as a Z-contrast image. High quality HAADF images require  a more precise specimen tilt than HRTEM images, and can  therefore reduce measurement errors from misalignment of the  crystal. Moreover, STEM HAADF images can tolerate a wide  range of sample transmission thickness and display no  dynamical diffraction contrasts. Furthermore, the probe  forming optics is before the specimen; therefore the postspecimen lenses defects, e.g. the chromatic blurring due to  energy loss after beam-specimen interactions, do not affect the  STEM spatial resolution as in HRTEM. Thus, STEM imaging  even on a microscope without aberration correction can  provide a relatively precise measurement of interface  thickness compared to the conventional HRTEM method.


Figure 9: (a) Probe-corrected HR-STEM image of the gate  oxide sample. The inset shows the FFT information of Si [110] transferring out to 0.11nm. (b) Column diagram of the gate  oxide width distribution measured by HR-STEM intensity  trace.


However, a STEM HAADF image can be degraded by many  factors, such as room temperature control, specimen drift, acoustic vibration, material radiation damage, and detector  noise since the image is acquired in a serial fashion [5, 13]. A  well-controlled environment is essential to ensure a scanning  distortion-free STEM image. Besides, an optimized STEM  probe with the correct convergence angle is the decisive factor  to achieve the best spatial resolution. Diebold et al. have  discussed how the convergence angle affects the contrast


transfer function and probe tails [3]. A 13-mrad aperture  instead of a 10-mrad aperture will not only lead to a noisier  image, but also will increase image delocalization. The  optimal convergence angle should be calculated according to  the diffraction blur and spherical aberration blur with the  source size. Experimentally, it should be selected by tuning  the condenser lens excitation and aperture size. In contrast, the  probe-corrected Titan microscope with a newly designed  column and constant power has been designed to reduce these  problems. The increased resolution, contrast, and signal to  noise ratio which benefits from aberration correction is clear  from the examples given.


The large discrepancy between uncorrected image  measurements and spectroscopic measurements could come  from the interfacial mixed state between the SiO2 and Si. The  larger statistical error in EDX results can be explained by the  fact that thin TEM specimens give only a low quantity of Xrays due to a small interaction volume and short acquisition  times. The uncorrected TEM EELS result is closer to either  image-corrected TEM or the probe-corrected STEM result. This is because EELS gives better detection ability for light  elements, e.g. C and O, than EDX. Besides, EELS has a  stronger signal to noise ratio than EDX at the 20nm sample  thickness that was used for spectroscopy analysis. The still  larger value of uncorrected TEM EELS result could be  explained that EELS is not only sensitive to nearest neighbor  environment changes but also second neighbor changes. Therefore, the measured electronic width of the interface is  always larger than the physical width, which is in agreement  with reference [4].


Aberration correction in an image corrector system can greatly  minimize the contrast delocalization and improve the usable  spatial resolution. Aberration correction in the condenser  system not only improves the STEM spatial resolution, but  also increases the signal to noise ratio. Thus, precise gate  oxide width measurement can be completed with a higher  degree of accuracy. Both new developments in electron  microscopy open a new era for structure characterization in IC  industries.


Acknowledgements


We thank FEI North America Nanoport and Ohio State  University (OSU) for providing the facilities in this work. Dr. L. A. Giannuzzi and Dr. J. Ringnalda are especially  acknowledged for helpful discussions. Dr. A. Genc at OSU is  also acknowledged for sample preparation.


[1] Principe, E. L. et al., "Advancements in the  Characterization of “Hyper-thin" Oxynitride Gate  Dielectrics through Exit Wave Reconstruction HRTEM


1.76 1.80 1.84 1.88 1.92


0 Number of measurements5


W    i    d    t    h   [  n    m   ]


and XPS”, Lawrence Berkeley National Laboratory, Paper LBNL-52151 (2002), pp. 1-11.


[2] H. Akatsu and I. Ohdomari, “HRTEM Observation of the  Si/SiO2 Interface”, Applied Surface Science, Vol. 41 (1989), pp. 357-364.


[3] Diebold A. C. et al., “Thin Dielectric Film Thickness  Determination by Advanced Transmission Electron  Microscopy”, Microscopy and Microanalysis, Vol. 9 (2003), pp. 493-508.


[4] Muller D. A., “Gate Dielectric Metrology Using  Advanced TEM Measurements”, Characterization and  Metrology for ULSI Technology: 2000 International  Conferences, edited by D. G. Seiler, et al.(2001), pp. 500-505.


[5] Stam M. et al., “A New Aberration-Corrected  Transmission Electron Microscope for a New Era”, Microscopy and Analysis, Vol. 19, No. 4 (2005), pp. 9-11.


[6] Urban K. et al., “A Way to Higher Resolution: Sphericalaberration Correction in a 200kV TEM”, Japanese Society  of Electron Microscopy”, Vol. 48 (1999), pp. 821-826.


[7] M. T. Otten and W. M. J. Coene, “High-resolution  Imaging on a Field Emission TEM”, Ultramicroscopy, Vol. 48 (1993), pp. 77-91.


[8] Lentzen M. et al., “High-resolution Imaging with an  Aberration-corrected Transmission Electron Microscope”, Ultramicroscopy Vol. 92 (2002), pp. 233-242.


[9] Jia C. L. et al., “Atomic Structure of a Σ=3, {111} Twinboundary Junction in a BaTiO3 Thin Film”, Philosophical  Magazine Letters, Vol. 79 (1999), pp. 99-106.


[10] Rose H., “Prospects for Aberration-free Electron  Microscopy”, Ultramicroscopy, Vol. 103 (2005), pp. 1-6.


[11] Lichte H., “ Optimum Focus for Taking Electron  Holograms”, Ultramicroscopy, Vol. 38 (1991), pp. 13-22.


[12] Scherzer O., “Theoretical Proof That Cs and Cc Are  Unavoidable with Round Electron Lenses”, Z. Physik, Vol. 101 (1936), pp.593-603.


[13] Cowley, J. M., “Electron Diffraction Phenomena  Observed with a High-Resolution STEM Instrument”, Journal of Electron Microscopy Technique, Vol. 3(1) (1986), pp. 25-44.


[14] Muller H. et al., “Advancing the Hexapole Cs-corrector  for the Scanning Transmission Electron Microscope”, Microscopy and Microanalysis, Vol. 12 (2006), pp. 442-455.


[15] H. Akatsu and I. Ohdomari, “HRTEM observation of the  Si/SiO2 interface”, Applied Surface Science Vol: 41-42 (1989), pp. 357-364.


[16] Giannuzzi L. A., et al., “2 keV Ga+ FIB Milling for  Reducing Amorphous Damage in Silicon”, Microscopy  and Microanalysis, Vol.11 (Suppl 2) (2005), pp. 828-829.


DOI: 10.1361/cp2008istfa021


Automated Serial-Section Polishing Tomography


J.A. Hunt, P. Prasad


Gatan Research & Development, Pleasanton, CA, USA 94588


E. Raz


Gatan FA Products Division, Pleasanton, CA, USA 94588


Tomographic reconstruction of a wide range of materials can  be accomplished via mechanical polishing serial-sectioning – alternately polishing away material and imaging the remaining  polished surface with optical (or electron) microscopy.  Under  computer control it is possible to acquire 2-D images of  hundreds of sections without user intervention and assemble  them for 3-D visualization and measurements.  In general, the  resulting 3-D images permit significantly better understanding  of the structure of complex systems than would be possible  with a few strategically acquired 2-D images at various  depths.  Herein we report what we believe is the first general  implementation of automated Serial-Section Polishing  Tomography (SSPT) and reconstruction using light  microscopy.


The SSPT technique discussed herein addresses the need to  derive accurate three-dimensional (3-D) reconstructions of  complex materials systems within the resolution range of light  microscopy.  The process described is based on the integration  of an optical microscope with a controlled material removal  technique and 3D reconstruction software. Although these  components have been available separately (e.g., [1]), the key  for routine use is an integrated system that produces accurate  3-D reconstructions with limited user involvement.


The SSPT technique is useful for imaging a wide range of  structures in the backend of the semiconductor fabrication  process including metallization, at the package level, and  printed circuits.  Outside of semiconductor failure analysis we  envision application in metallography such as 3-D grain shape  and orientation analysis, and in materials science general  imaging of structures in the 1-1000 µm range.  A wide range  of optical microscopy methods can be utilized which can  extend the technique to problems that cannot be adequately  imaged using x-ray methods, such as grain-boundary  reconstruction of homogeneous systems.


The SSPT technique is not applicable to systems that cannot  be mechanically polished to allow high-quality microscopy.  Automating the polishing technique with robotics does extend  the range of samples that can be polished over that which is  possible with a manual technique alone.  However, some  samples will be too delicate or too flexible such as


unsupported structures (e.g., bond wires) and structures that  smear rather than polish regardless of polishing recipe (e.g., unfixed biological samples and some polymer systems).  Until  implementation of an electron microscopy version of the  technique, it is not useful for applications requiring resolution  below the currently implemented optical microscopy  techniques.


Competing technologies for 3-D reconstruction in the micron  through ~10 mm range include x-ray microscopy [2] and FIB  dual-beam serial-sectioning [3].  There is an excellent  summary of a manual process described in [1].


System implementation


Automation of the serial-sectioning process is required to  make the SSPT practical. Specific challenges include: (1) high-speed material removal with resultant high surface  quality, (2) control over the repeatability of increments in Z (polishing depth), (3) ability to clean the sample after  polishing, (4) maintaining precise alignment of the sample in  XYZ, rotation and both tilt axes while the sample is translated  between polishing, cleaning, and imaging, and (5) imaging the  sample while retaining precise image focus after each  polishing step.  The Gatan Centar Frontier [4,5], a computercontrolled polishing system designed for cross-sectional and  plan-view specimen preparation, was straightforward to  modify for the purpose of SSPT.


The Centar system features a robotic arm that can precisely  control the polishing force and orientation of the sample onto  a mechanical polishing wheel.  Polishing rate and progress can  be monitored through closed-loop positional feedback on the  robotic arm and via light microscope observation.  The robotic  arm can rotate the polished sample surface from the polishing  wheel to the optical microscope and back with repeatability  below a micron and essentially no image field rotation.  Translation of the sample enables field stitching to extend the  field-of-view to the centimeter level.  Several optical  objectives are selectable under computer control allowing (1) tradeoff of resolution and single-image field-of-view and (2) optical microscopy contrast method.  Modifications to the  Centar system were primarily new software routines that  automated existing delayering and imaging functions in an  acquisition loop.  The SSPT workflow is summarized in Fig.


1.


Figure 1:  Serial-Section Polishing Tomography (SSPT) workflow. Shaded boxes indicate time-consuming steps that  can proceed without user involvement.


Sample preparation


SSPT sample preparation involves removing the smallest  practical volume of material that contains the area to be  imaged.  On the Centar there are maximum sample size  limitations for tomography samples of approximately 1 cm per  side.  It is advantageous from a polishing time and polishing  media expense perspective to minimize the area to be  polished.  The sample is mounted via wax or equivalent to the  Centar sample holder.


Setup


The tomography acquisition setup requires user input and  involves selecting XY imaging resolution and field-of-view (FOV), polishing depth per slice (∆Z) and number of sections (Z), and selection of polishing recipe optimized for speed  versus surface quality.  After setup the acquisition can proceed  without user intervention, although the system is designed to  allow the user to intervene in cases where polishing media  must be changed or if polishing parameters are to be refined.  Selection of polishing recipe is critical to achieving good  quality images with the minimum polishing time.  The current  SSPT implementation utilizes the delayering recipe system of  the Centar Frontier, which primarily involves choosing a  polishing media, polishing force, radial range of polishing  medium to utilize, and time or distance in Z to polish.


Recipes can in principle involve many polishing steps but we  have at present avoided changing polishing media between  steps to avoid the need for user intervention to change the  media.  It should be possible to extend the technique to  multiple polishing grits when papers are used by incorporating  a hybrid paper with different grits as a function of radius.  This adaptation would permit faster polishing times but at  present has not been incorporated.


Data acquisition


SetupAcquisitionReconstructionVisualization


Acquisition generally proceeds without user intervention  although polishing over long durations may require a media


Specify ROi and


Polish XY surface


Fine align image 1


View as slices in


sampling


ojs ewdjaq Av Z


in XY


XYIXZ.YZ


change.  It is a simple matter to interrupt the system at any


resolution in XYZ


罗


一


time for this purpose without affecting alignment.


零


dlaeus eudja


Correct image


Choose polishing


hw


artifacts


3D rendering


parameters and


media


After each polishing step, the sample must be adequately


2D.3D


weBaX Xs njeoa


Save data in 30


measurements


cleaned and dried prior to imaging.  This is a standard


m!nuu 3uosoodadataset


odgouegAs mpu


function of the Centar system, although small modifications to


undiay eips


air flow had to be made to improve sample drying for


Repeat for all:


牛


images


tomography.  If sample drying is insufficient then water


Save data


droplets will occasionally preferentially adhere to certain  structures generating image artifacts.


Repealuntil all Zimaged


Image stitching is required when the specified FOV is larger  than the microscope FOV.  Each microscope image acquired  takes 1-2 seconds for the acquisition and sample translation.  Image stitching is essentially instantaneous.  Stitch boundaries  on the current system are insignificant for all but the highest  magnifications – at the latter more work is needed to improve  image alignment (this is expected to be straightforward).


Multiple XY FOVs can be saved at each slice.  The data is  saved as a single image for each separate FOV at each slice, and is later combined into one 3D dataset for each FOV  during the reconstruction phase.


Reconstruction


Reconstruction of the acquired data is straightforward  provided alignment issues and polishing artifacts are  controlled.  The resulting 3-D datasets can be of large XY  areas (many mm2) with sub-micron resolution in XY or Z.


The ultimate reconstruction resolution is limited primarily by:


(1) resolution of the microscope (~0.5 µm for the light  microscope used here), (2) image pixel size, and (3) accuracy  of the alignment of the image sections.


Alignment of image sections is dependent on the system’s  ability to reproducibly return to a specific sample position in  between polishing steps.  This is both system and sample  dependent, but reproducibility of better than 1 µm (and no  measurable sample rotation) has been readily achievable.


Further improvement of alignment accuracy can be facilitated  via attaching fiducial markers along the sides of the sample  that serve as reference points for post-acquisition crosscorrelation and subsequent image alignment. We have  obtained good results working with 7 µm diameter alumina  fibers glued to the sample edge with an optically opaque  epoxy.  The fiber should be placed as parallel to the Z-axis as  is practical to ensure good vertical alignment for features with  large separation in Z.  Alignment with respect to fiber centers  of better than ¼ pixel are readily achievable.  The translational  repeatability of the Centar stages allow the fiducial markers to  be an arbitrary distance from the reconstructed volume.


Several imaging artifacts are typically encountered and must  be controlled to produce accurate image reconstructions, including: (1) polishing scratches, (2) polish debris remaining


on surface or in voids during imaging, and (3) microscopy  contrast mechanisms that confuses reconstruction such as  specular contrast from surface roughness.  In general these  artifacts do not significantly limit the capability of the  technique but in some cases does introduce the need for image  processing.


The most common artifact encountered to date are polishing  scratches which tend to affect only a single Z slice at a time.  We have treated these successfully by median filtering each  slice with the slice above and below it.  This does result in a  modest reduction in Z resolution that requires consideration  when selecting polishing depth between planes.


Another important imaging artifact is from the specular  contrast at the rough edge of a feature that is polished to  almost zero thickness.  This artifact is also reduced by median  filtering, but not as successfully as the removal of polishing  scratches.


As in most microscopy techniques, care must be taken to  avoid interpretation of artifacts as specimen features – this is  facilitated in the SSPT technique by allowing straightforward  switching from a feature-in-question in the 3-D view back to  the original 2-D dataset.


A typical reconstruction process involves (1) fine image  alignment via cross-correlation (typically skipped if pixel size  is >1 µm), (2) median filtering the aligned images, and (3) saving the aligned images to a 3D dataset.  After  reconstruction, the data can be viewed plane-by-plane, or as a  3-D volume.  The reconstruction and visualization of the data  are performed off-line in Gatan DigitalMicrograph plug-ins on  a separate computer system to permit more efficient utilization  of the Centar tool.  Approximately 10 minutes of  user/computer time is required for reconstruction before data  is ready for visualization and measurement.


Example


Figure 2 shows selected sections from a printed circuit board  reconstruction that was acquired with an XY pixel size of 3 µm, XY FOV of 1.4 mm x 3 mm, and 150 sections (Z) of 1.68 µm each.  Polishing used a 0.5 µm diamond paper and  required ~30 s per slice, in addition to a dead time of ~20 s per  slice for sample rotation to and from the microscope, cleaning, imaging and stitching 4 image fields to cover the whole FOV, and lowering the sample back to the polishing table.


After the sample was mounted, the total user time required for  setup and acquisition was ~30 minutes although in principle  could be less than 10 minutes.  The polishing and data  acquisition phase proceeded entirely under computer control  and without need for a user present – the portion of data  shown required ~3 hours.  It is expected that typical data  acquisition will require 2-10 hours of Centar time.


Section #14  Z = 24 m


Section #42  Z = 71 m


Section #124  Z = 209 m


Section #129  Z = 218 m


Section #139  Z = 234 m


Figure 2: Selected sections illustrating sectioning progress of  a 1.4 mm x 3.0 mm printed circuit board.  Arrow shows a  polishing artifact (scratch).


Tomography reconstruction involved identifying and  correcting image artifacts and aligning the images in XY.  For  the reconstruction of the printed circuit board in Figure 3, the  as-acquired data required no additional image alignment, but


some polishing scratches were removed using the  aforementioned median filter process.


Figure 3a: Reconstructed volume from data in Fig. 2 (first  150 Z slices shown). Intensities of fiberglass weave and epoxy  displayed. Individual 7-10 µm fibers clearly shown in all  orientations.


Figure 3b: Intensities of metal vias displayed with a lighting  and transparency scheme that highlights interfaces. The  arrows point to a band of contrast due to a specular artifact  from surface roughness at the epoxy-metal interface in  sections #139-140.


Extension to electron microscopy


An important limitation to this technology as demonstrated is  the ultimate resolution of light microscopy.  In principle the  extension to electron microscopy would require a method to  polish and clean under essentially atmospheric pressure, followed by a pump-down of the sample to an appropriate  vacuum level for SEM observation.  These adaptations would  allow approximately 2 orders of magnitude better resolution  than the current optical technique.  In many conditions it  would have faster slicing times than FIB dual-beam based


serial-sectioning methods as well as significantly greater  imaging area.


A general implementation of automated serial-section  polishing tomography is demonstrated and is expected to be  applicable to a wide range of problems relevant to  semiconductor backend processes and general materials  science.  This method proved to offer efficiency and quality  advantages over related prior methods in which a specimen  was repeatedly sectioned with much thicker slices, dismounted, photographed through a microscope, and  remounted on a fixture for the next cut.


Reconstructions can be viewed after less than one hour of user  time although 2-10 hours of additional Center tool time is  required for data acquisition.  As with most microscopy  techniques, some technique artifacts will remain even after  processing and analyst due-diligence is required to prevent  misinterpretation.  The resulting 3-D images permit  significantly better understanding of the structure of complex  systems than would be otherwise possible with only 2-D  sections.


[1] N. Chawla, , V. V. Ganesh and B. Wunsch, Scripta


Materialia, 51:2 (2004) 161.


[2] P.J. Withers, Materials Today, (2007) 10 (12) 26-34.


[3] B. J. Inkson,, T. Steer, G. Mobus, T. Wagner,  Journal of  Microscopy, 2001, vol. 201, issue 2, p 256.


[4] Sarfaty et al., Precision Polishing System, US Patent


#5,741,171.


[5] D.J. MacMahon and E. Raz-Moyal, Microscopy Today  15:6 (2007).


DOI: 10.1361/cp2008istfa025


APPLICATIONS OF SCANNING NEAR-FIELD PHOTON EMISSION MICROSCOPY


DV Isakov, BWM Tan, JCH Phang, YC Yeo


Centre for Integrated Circuit Failure Analysis and Reliability (CICFAR), National University of Singapore  dmitry_isakov@nus.edu.sg


AAB Tio, Y Zhang


Precision Measurements Group, Singapore Institute of Manufacturing Technologies, Singapore


T Geinzer, LJ Balk


Faculty of Electrical, Information and Media Engineering, University of Wuppertal, Germany


In this paper, the application of scanning near-field photon  emission microscopy for imaging photon emission sites is  demonstrated. Photon emissions generated by a Fin-FET test  structure with one metallization layer are imaged with spatial  resolution of 50 nm using scattering dialectic probe. The  potential applications and limitations of the technique are  discussed.


Current fault localization techniques have limited resolution  and sensitivity parameters, which are inadequate for the  current technology node whereby substantial searching is still  required for post-localization [1]. One of these techniques is  Photon Emission Microscopy (PEM), which is an important  tool for the localization of hot carrier sites and faults in silicon  based integrated circuits [2]. The spatial resolution of current  PEM tools, which are operated in the optical far-field, is  limited by optical diffraction. The theoretical spatial  resolution according to Rayleigh Criterion is about half the  wavelength used but the practical spatial resolution is closer to  one wavelength due to instrumentation constraints. For silicon  devices, the significant contribution of photon emission occurs  in the near-infrared (NIR) and the practical spatial resolution  of far-field NIR PEM systems is limited to about 1 µm. Recent developments in using solid immersion lenses in PEM  have improved the spatial resolution to around 230 nm [3]. However, for a critical defect size of 45 nm at the 90 nm  technology node [4], the desired spatial resolution should be  better than 50 nm.


In our earlier work, a Scanning Near-field Photon Emission  Microscope (SNPEM) was introduced [5]. It was used for  imaging photon emissions from silicon devices in the visible  spectral range from 400 to 900 nm [5]. SNPEM is based on a  collection mode of a Scanning Near-field Optical Microscope (SNOM). In SNOM, a sub-wavelength aperture is used for  near-field light detection and the dimension of the aperture  determines the resolution of the SNOM [6]. The method of


collecting photons in the near-field has been proposed [7], but  the technique has not been developed. A probable reason  could be the low sensitivity due to extreme attenuation of light  intensity [8]. Our SNPEM system avoids this limitation and  demonstrates a much higher sensitivity at a similar resolution. In our previous work, the improvement was achieved with a  protrusion type probe (PTP), which had a large base aperture


[5]. When such a probe is scanned 10-20 nm above the  surface, photons are scattered by the dielectric tip of the  protrusion. The resultant radiation is collected in the far-field  by the base aperture formed in the metal coating just above the  tip. However, the main problem with the PTP is the base  aperture formation during the fabrication process. The process  requires the removal of the metal coating from the tip with a  Focused Ion Beam (FIB). The repeatability of the process  depends heavily on the skill of the FIB operator and requires a  considerable amount of time for each probe.


A Scattering Dielectric Probe (SDP) has been proposed to  overcome this limitation [9]. For the SDP the coating is not  used and the base aperture is determined solely by the  geometry of the probe. As shown in Fig. 1, the SDP has a  cylindrical cross-section with a diameter of approximately 3 μm just before the final tip. The cylindrical part is formed  during the process of heating and simultaneous pulling of a  piece of a multi-mode fiber. The final tip is formed by front  illumination with the FIB. The tip formation is determined by  the difference in the etching rate between the edge and inner  parts of the cylindrical probe. The final taper has a cone angle  of 20o and the tip diameter is estimated to be below 50 nm. The process does not require any micromachining or fine  focusing and takes one minute per tip.


This paper describes the application of the SNPEM system  with the SDP for imaging photon emissions from test  structures with a single metal layer. As most of the photon  emissions from silicon devices have energy below the silicon  bandgap, a NIR photomultiplier with a wavelength range from  1000 nm to 1400 nm was used. Detailed description of the  detection unit can be found in [9].


Fig. 1. Scattering dielectric probe (SDP)


Application of SNPEM to test structures


SNPEM analysis requires direct access to the near-field of the  emission source. This requirement makes it impossible to use  conventional backside analysis with a silicon substrate thinned


ab


down to 50-100 µm. However, front-side analysis of test  structures with a minimum number of metallization layers  could be possible. For the demonstration of the capabilities of  the SNPEM system with the SDP, a Fin Field Effect  Transistor (FinFET) test structure [10] was investigated.


Fig. 2a shows the far-field PEM image of the FinFET device  for the wavelength range from 400 nm to 1100 nm overlaid on


2pm


the far-field reflection image. Following biasing conditions  were applied: drain voltage – 4V; gate voltage – 3V; drain  current – 15 µA. The image was recorded with a 100X


C


objective lens with numerical aperture of 0.55. The pixel size  of the digitally magnified image was equal to approximately  500 nm (Fig. 2a). The highest intensities of photon emissions  were localized at the drain metal contact.


a


b


200 mm


2μm


Fig. 2b shows the SEM image of the area, where the photon  emissions were localized by the far-field PEM in Fig. 2a. A  gap between the metal contact and gate material was  observed. This gap can serve as a window, guiding the


photons from the active area into the free space. The width of


base


the gap was estimated to be 200 nm.


aperture


The topography images of the FinFET at two different  magnifications are shown in Fig. 3a and 3b respectively. It can  be seen that these images are distorted. It should be noted that


far-field


the SDP was glued manually to the quartz tuning fork, which  was used for distance regulation [5], and hence, it was not  possible to perform final adjustments of an angle between the


near-field


probe and the sample. The presence of this angle can possibly  explain why the distortion of the metal contacts in the  topography images was not symmetrical. The recorded photon


2 μm


emission area shown in Fig. 3c and Fig 3d is approximately 2 μm in diameter. We believe that this emission area was  detected by the base aperture of the probe in the far-field and  roughly corresponded to the effective collection diameter of  the base aperture. High spatial frequencies in photon emission  distribution recorded on the background of this 2 μm spot may  be attributed to the interaction of the sharp tip in the nearfield.


metal


gate


Fig. 3. (a, b) Topography images and (c, d) SNPEM of Fincontactmateria


FET test structure at different magnifications


gap


The high magnification topography and SNPEM images of the


400mm


photon emission area are shown in Fig. 4a and 4b


3μm


respectively. The image size is 1 by 1 µm, which is equal to  the lowest wavelength of photons detectable in the current  SNPEM set-up. In the image, fine details of photon emission  distribution are revealed showing that the highest intensities  are concentrated at the metal contact.


Fig. 5 shows the corresponding line profiles across the  topography (line AA’) and SNPEM (line BB’) images. It is  evident that the highest 20% of the photon emission intensity, i.e. intensity above 0.8 level, are confined within 200 nm (Fig.


Fig. 2.  a) Far-field PEM image overlaid on reflected image of  FinFET; b) SEM image of the area with maximum photon  emission intensity in far-field PEM image


5), which should correspond to the gap between the metal  contact and the gate material (Fig. 2b). A clear  correspondence between the edge of the metal line and the  beginning of the sharp increase in photon emission intensity  can be used to estimate the optical resolution of the image. Following the knife-edge method, the resolution is estimated  at 50 nm (Fig. 5), which is at least 20 times smaller than the  wavelength of the detected photons. This value is dependent  on the exponential decrease of the near-field interaction with  the distance from the surface and might affect the  characterization of the SNPEM system resolution. Nevertheless this value can be used as an indicator of the  spatial resolution of the localization technique.


m


Fig. 4. High magnification (a) topography and (b) SNPEM  images of the photon emission area in Fig. 3


0 200 400 600 800 1000


0 Topography, nm100


300


400


500


- Topography


- PE intensity


Position, nm


0.0


"plMd


0.4a


0.6Sn


0.8n


50 nm


200 nm


Fig. 5. Topography and intensity profiles across lines AA’ and  BB’ respectively


In order to assess the actual near-field resolution capabilities  of the system, we considered the region with minimal  topographical variations. From the topography line profile in  Fig. 5, it can be seen that the region on the right of the metal  contact is fairly flat. Adopting the theoretical model developed  by Ohtsu and Kobayashi [11], this region was fitted with two  Gaussian curves representing near-field and far-field  interactions respectively (Fig. 6).


200mm


For the curve fitting procedure, the following assumptions  were made: a) area of interest from 500 nm to 1000 nm of the  linescan with minimum topography variation; b) only two  peaks corresponding to the far-field and near-field effects; c)


coinciding locations of the maxima of these two peaks.  During the curve fitting process, the number of peaks and  position of their maxima were fixed, while amplitudes and full  widths at half maximum (FWHM) were varied. The fitted  curve in Fig. 6a was reached within 20 iterations. The  resulting values of the FWHM for near-field (NF) and farfield (FF) curves are 80 ± 10 nm and 570 ± 10 nm  respectively (Fig. 6). The FWHM value of the far-field (FF) curve is approximately equal to half of the wavelength  corresponding to silicon bandgap energy. The value of 80 nm  should be treated as a sum of the system near-field optical  resolution and effective size of the emission source. These  results are an important indicator of the validity of the SDP  concept.


200 400 600 800 1000


200nm


Intensity,u a..


0.4


0.6


A


A’B


B'


--


- Exp. data


- NF


- FF


- NF+FF


570 nm 80 nm


Fig. 6. Curve fitting of the intensity profile in Fig. 5b with two  Gaussian curves corresponding to near-field and far-field  interactions of emission source and the probe.


t e


y


Using the results of the curve fitting, it is possible to ignore  photon emission intensities below 0.8 level of maximum


u


intensity because those photons are not related to the nearfield interaction. Hence, only the distribution of the highest  20% of photon emission intensities should be overlaid with  the topography image as shown in Fig. 7. This SNPEM image  clearly demonstrates higher spatial resolution in comparison  with the far-field PEM image in Fig. 2a.


Fig. 7. Highest 20%  of photon emission intensities was


overlaid with the topography image


Application to real devices


In the application of SNPEM to the test structures with one  metal layer, the above achievable resolution provides useful  information on the location of the maximum photon emission  intensity within a structure. For example, a SRAM cell  fabricated at the 65 nm technology node is confined to an area  smaller than 0.6 μm2 [12]. Hence, if one of the 6 transistors in  the cell is leaking, the far-field PEM system with resolution in  the order of 1 μm will not able to localize the faulty transistor. The SNPEM can clearly pinpoint the location of the leaking  transistor and correlate the topography image to the actual  layout of the cell.


The prerequisite condition of having only one or two metal  layers constrains the applicability of SNPEM. Sample  preparation techniques are required for accessing the nearfield of the photon emission source. For example, SNPEM can  be applied to devices based on Silicon-On-Insulator (SOI) technology since the Si substrate can be chemically removed  down to the buried oxide without affecting the electrical  functionality of the device [12]. Other techniques have been  successfully applied to devices prepared in this way [13, 14]. It is important that SOI devices with removed Si substrate are  topography-free to take full advantage of the enhanced spatial  resolution of SNPEM. For devices based on bulk silicon, FIBbased circuit edit can be used to bring the SNPEM probe to  distances within 400 nm from the emission source [16].


Even if the applicability of SNPEM might be limited due to  the near-field constraint, SNPEM provides an important  opportunity for non-destructive characterization of test  devices with resolution compatible with the current  technology node. This capability allows a clearer  understanding of multiple physical phenomena within a biased  device, which cannot be investigated with existing destructive  characterization techniques or computer simulations.


The enhanced spatial resolution of SNPEM, which is  compatible with the requirements of the current technology  node, was demonstrated. It was shown that in comparison  with far-field PEM, SNPEM can provide a better  understanding of the origin of photon emission generation. The analysis of photon emission distribution from a test  FinFET showed that most of the photons generated within the  device were radiated through the 200 nm gap between the  drain and gate contacts. The near-field and far-field  components of collected radiation by the SDP have been  determined through an analysis of the photon emission  intensity distribution. The requirements for any future  applications of SNPEM for failure analysis were discussed.


D Isakov is supported by a National University of Singapore (NUS) research scholarship. The project is collaboration  between NUS, Singapore Institute of Manufacturing and  Technology and University of Wuppertal, Germany. We  would also like to thank Center of Integrated Circuit Failure  Analysis and Reliability (CICFAR), National University of  Singapore, and SEMICAPS Pte Ltd, Singapore, for the kind  permission to use their facilities.


[1] Vallet DP: “Why waste time on roadmaps when we  don’t have cars?”, IEEE Transactions on Device and  Materials Reliability, Vol 7, No 1, (2007), pp. 5-10.


[2] Phang J.C.H. et al., “A review of near infrared photon  emission microscopy and spectroscopy”, Proc Int Symp  Physical & Failure Analysis of Integrated Circuits (IPFA) (2005), pp 275-281.


[3] Ippolito S. B. et al., "High spatial resolution subsurface  microscopy", Appl Phys Letts, Vol 78, No 26 (2001) pp. 4071-4073.


[4] Semiconductor Industry Association: "International  Technology Roadmap for Semiconductors", http://public.itrs.net/


[5] Isakov D. et al., “Scanning near-field photon emission  microscopy”, Proc  International Reliability Physics  Symposium (IRPS),  Phoenix, Arizona, USA, 27 Apr 08


- 1 May 08, pp. 575-579.


[6] Balk L.J. et al., “Characterization of electronic materials  and devices by scanning near-field microscopy”, Applied Physics A, Vol 87 (2007), pp. 443-449.


[7] Luo Z.: “Method and apparatus for isolating defects in  an integrated circuit near field scanning photon emission  microscopy”, Assignee: Texas Instruments Incorporated, US Patent References 5,235,400 (1999).


[8] Labeke D. V. et al., “Optical Characterization of  Nanosources Used in Scanning Near-field Optical  Microscopy”, Optical Society of America, Vol. 12 (1995), pp. 695-703.


[9] Isakov D et al., “Near-field detection of photon emission  from silicon with 30 nm spatial resolution”, 19th  European Symposium on Reliability of Electron  Devices, Failure Physics and Analysis (ESREF), Maastricht, Netherlands September  29th  - October 2nd  2008, accepted.


[10] Liow T.Y. et al., “Strained N-channel FinFETs with 25  nm gate length and silicon-carbon source/drain regions  for performance enhancement”, Symposium on VLSI  Technology, (2006), pp. 68-69.


[11] Ohtsu M., Kobayashi K., “Optical Near Fields: Introduction to Classical & Quantum Theories of  Electromagnetic Phenomena at the Nanoscale”, Springer, Ch 3-4 (2003), pp 25-76.


[12] Lamy M. et al., “How Effective Are Failure Analysis  Methods for the 65nm CMOS Technology Node?”, Proceedings IPFA, Singapore, 2005, pp. 32-37.


[13] Prejean S. et al., “CMOS Backside Deprocessing With  TMAH/IPA as a Sample Preparation Procedure for  Failure Analysis”, International Symposium for Testing  and Failure Analysis (ISTFA2002), pp. 317-323.


[14] Eng T.T. et al., “Backside Deprocessing Technique & Its  Novel Fault Isolation Application”, Proceedings IPFA,  Singapore, 2005, pp.110-113.


[15] Narang V. et al., “Development of Backside Scanning  Capacitance Microscopy Technique for Advanced SOI  Microprocessors”, International Symposium for Testing  and Failure Analysis (ISTFA2006), pp. 94-97.


[16] Boit C, et al., “Physical Techniques for Chip-Backside  IC Debug in Nanotechnologies”, IEEE Design & Test of  Computers, (2008), pp. 250-257.


image resolution better than 2 microns. This provides  conclusive information on whether there is physical contact or  not. Figure 8b shows the virtual cross section view of


potential area of physical contact. The two wirebonds appear  to be touching each other within the 2 micron resolution of the  virtual cross-section view. Once the exact location of the  physical contact was found, the unit was physically crosssectioned for correlation purposes only, figure 8c. As can be  seen, correlation between the virtual figure 8b and physical  figure 8c images is very clear.


Figure 8. x-ray CT results: (a) Virtual 3D  model clearly  showing physical contact between failing wirebonds, (b) virtual cross section of x-ray image at location of physical  contact, confirming information of virtual 3D model, and (c)


optical image of physical cross-section showing that it


correlates very well with virtual x-ray image.


C4 Bump Open Detection


In another interesting case study, a unit failed with C4 bump  open. A Time Domain Reflectometry (TDR) tool could not  isolate the defect location. 2D x-ray was also used to search  for potential defective C4 bumps without success. The unit  was scanned using x-ray CT to search for any defective C4  bump along the failing structure that could have caused the  open failure.


A routine was created to perform hi-resolution scanning in the  whole chain of C4 bumps, which required 10 scans. Each scan  took about 20 minutes, with a field of view of about 2mm  square. As can bee seen in figures 9a-b, the defect was  localized along the failing structure as low-volume solder that


could not be seen with 2D x-ray due to the presence of a  capacitor that blocked radiation thus masking-out the defect,


Figure 9a. The virtual plane view is shown in figure 9b, in  which the defect can be clearly seen. For comparison  purposes, figure 9a shows the top view of 2D x-ray image  indicating the area (solid yellow rectangle) where the low  volume solder bump was found. Note that it is not detectable  at all with 2D x-ray.


(b)Virtual Plane View


(a) 2D x-ray


Figure 9. (a) 2D x-ray image of area of interest, notice defect  cannot be seen, (b) Virtual planar grinding view, yellow circle  highlights defective C4 bump.


Figure 10a shows the virtual cross section of defective lowvolume and a passing solder bumps. The unit was physically  deprocessed for correlation purposes; figure 10b shows the  picture of the physical cross-section. Notice the good  correlation between virtual and physical images.


Figure 10. Comparison between (a) virtual and (b) physical


Virtual Cross"Section View"


cross section views of both failing low-volume and passing C4  bumps.


C4 Bump Cracking Detection


Cracks in C4 bumps could appear in units under thermal stress  for reliability evaluation. Electrical test cannot isolate partial  cracks but just full solder joint cracks and the isolation


resolution depends on the number of C4 bumps between test  points. Destructive techniques like Dye and Pull produce  artifacts and cannot be used in packages with underfill. Physical cross-sectioning is a tedious and time consuming  process that requires more than 3hrs for about ten C4 bumps. The objective of this application development is to establish a  non-destructive method to detect cracks in C4 bumps. Figure  11a and 11b show the virtual cross section and planar grinding  views of C4 bumps that were obtained for a sample size of ~6cm2, without any sample preparation required.


Figure 11. (a) Virtual cross section and (b) planar grinding of  corner C4 bumps. Yellow dotted line on plane view indicates  line of cross section.


Figure 12 show a comparison between virtual planar and cross  sectional views for both a failing C4 bump from the corner of  the die, and a passing C4 bump from the center of the die. As  can be seen in figure 12, x-ray CT can provide a clear finger  print of cracking issues, either using a virtual plane or a crosssectional view. In this slice the surface of a good solder joint  looks smooth and uniform; whereas the slice surface of a  failing bump looks uneven. A similar situation occurs with the  virtual cross-sectional views.


Low-volume solderPassing solder


Cracked joint


Good joint


Virtual Planar View


Figure 12. X-ray image comparison between a failing C4  bump (left images) and a passing C4 bump (right images): virtual planar views (top) and virtual cross sectional views (bottom).


Progressive Testing


One of the compelling capabilities of x-ray CT is the  possibility of performing defect inspection during reliability  testing to provide feedback to predictive reliability models, as  well as at different steps during process development. In order  to demonstrate progressive testing capability, C4 bump area of  a unit without underfill was imaged before and after thermal  stressing. The absence of underfill helped in cracking the C4  bumps during thermal stress. A routine was created to scan the  units with high resolution, with a data acquisition time of  about 90 minutes. Figure 13a shows the virtual planar view


image of the same C4 bump area obtained prior to thermal


21/2u


stress to verify that C4 bumps were not cracked, and figure  13b shows similar view after thermal stress showing that


Metallic


solder joints with finger print of bump cracking, according to


Socket


comparison of good joint and cracked joint show in figure 12.


Figure 13. Comparison between virtual planar view of C4  bumps (a) before and (a) after the applied thermal stress.


X-ray CT has several advantages over physical deprocessing. For instance, using physical cross sectioning, the analyst  usually gets information from about 10-20 bumps, with  limited information of a single cross-section, with a  throughput time of 3-4hrs. Whereas x-ray CT can obtain full  information of both virtual plane and cross sectional views of  60 to 100 C4 bumps (between 6-10 rows) in about 30 to 90  minutes, depending on how x-ray-absorbing the sample is. Table 1 summarizes a comparison between Physical and  Virtual methods for bump cracking applications.


|Comparison  Matrix Parameter Physical|XRay CT|Comparison  Matrix Parameter Physical|XRay CT|Comparison  Matrix Parameter Physical|XRay CT|
|---|---|---|

|Analyzed bumps|10-20|60-100|

|Number of rows|1|6-10|

|Xsections/bump|1|Multiple|

|Time-to-information|3-4|1-2h|

|Plane views|h Cannot|Multiple|

|Progressive test?|No|Yes|

Table 1. Comparison matrix between physical and x-ray CT  virtual methods for bump cracking detection.


BGA Micro Voiding


Figure 14(a) shows a metallic socket in which a nondestructive characterization of voiding in solder balls is


required. 2D x-ray imaging can provide some information  about voiding, however it is limited to a single top view with  overlapping details as shown in figure 14(b). This application  requires obtaining a 2D x-ray image of the whole sample to  select the solder balls to be inspected with x-ray CT. Once the


area of interest has been determined, higher resolution scans  can be performed in those areas to fully characterize voids as  indicated in figures 14(c-d). Figure 14(c) show a virtual cross  section view of a solder ball, indicating planes where voids  are formed. Virtual planar views can be obtained at any plane  level to detect its voiding, as can be seen in figures 14(d-f).. Typical data collection time is around 15 minutes per region  of interest of about 4mm2.


(e)


(f)


(a)Void to Crack(b)


Figure 14. (a) Board sample with metallic socket. (b) Best 2D  x-ray image of voids. (c) Virtual cross section of solder ball  and (d)-(f) virtual plane views of voids.


BGA Solder Joint Cracking Detection


Another compelling capability of x-ray CT is the detection of  solder ball cracking in the second level interconnects BGA  package. In this case, the typical sample dimensions are in the  range of 1-2 inches wide. Figure 15 shows a planar view  indicating solder ball cracking issues (a), and also a virtual  cross section confirming the existence of cracks and their  plane location. Scanning times for this application using a 4X  objective lens is around 30 to 60 minutes, with a field of view  of ~4mm2.


Figure 15. (a) Virtual plane view and (b) virtual cross section  view of solder balls corresponding to yellow-doted line after  thermal cycle stress testing, indicating typical finger print of  solder joint cracking.


This paper has demonstrated the successful development of  new applications in x-ray CT for the non-destructive isolation  of defects in next generation package technologies. C4 bump  cracking and “invisible” non-wetting analysis, BGA fatigue  and cracking, wirebond microcracking and shorting, BGA  voiding, are some of the critical applications in which the  capability of x-ray CT has been demonstrated. Further  development in x-ray CT technology roadmap should include  improving spatial resolution to sub-micron level, reducing  time-to-data to levels of 10 minutes of data acquisition, improving reconstruction algorithm to reduce data processing  time, increasing usability and customizing software for data  inspection automation.


We’d like to acknowledge Jeff Thomas, Lars Skoglund, Rajen  Dias, Betty Phillips, Zhiyong Wang, Andy Proctor, Frank  Thoth, Ranga Prasanna, Marty Bitsoi, Kaushik Muthur and  Joaquin Aguilar-Santillan from Intel Corporation for technical  discussions regarding applications development that were  presented in this paper. We’d like to also acknowledge  Hauyee Chang, Wenbing Yun and Fred Duewer from Xradia, Inc for technical discussions regarding x-ray tomography  system and applications development that are reported in this  paper.


1. D. Goyal, “X-Ray Tomography for Electronic  Packages”, ISTFA, 2000.


2. D. Goyal, Z. Fu, J. Thomas, “3D X-ray Computed  Tomography for Electronic Packages”, ISTFA, 2003.


3. Scott, F. Duewer, S. Kamath, A. Lyon, D. Trapp, S. Wang, W. Yun, “A Novel X-ray Microtomography  System with High Resolution and Throughput for  Non-Destructive 3D Imaging of Advanced  Packages”, ISTFA, 2004, pp. 94-98.


DOI: 10.1361/cp2008istfa036


Flip-Chip Bump Interface Failure Mechanisms In Plastic BGA  Packages And Failure Analysis Process Flow


Zhaofeng Wang,  Sr. FA Engineer, Failure Analysis Lab


International Rectifier Corp.


41915 Business Park Dr. Temecula, CA92590   Tel. (951)375-4270, e-mail zwang1@irf.com


The present paper studies several  failure mechanisms at both UBM and Cu  substrate side for flip-chip die open contact  failures in multi-chip-module plastic BGA-LGA  packages.


A unique failure analysis process  flow, starting from non-disturbance inspection  of x-ray, substrate and die level C-SAM, bump  x-section followed by a bump interface  integrity test including under-fill etching and  bump pull test and/or substrate etch has been  developed.


Four different types of failure  mechanism in multiple chip module that are  associated with open/intermittent contact, ranging from device layout design, UBM  forming process defect, to assembly related  bump-substrate interface delamination have  been identified.


The established FA process has been  proved to be efficient and accurate with  repeatable result. It has facilitated and  accelarated new product qualification  processes for  a line of high power MCM  modules.


Flip-chip BGA technology has been becoming  ever popular to meet the challenge of  enhancing electrical and thermal dissipation  capabilities, demanding design requirements  of densification, and manufacturing cost  reduction.


This paper focuses on failure analysis  procedure development and failure  mechanisms discovered during product  development of a flip-chip inside a multiple  chip power module (MCM) in plastic package  with multi-layer PCB substrate (Fig. 1).


Fig. 1:  Tilted top view of a module showing  plastic mold and PCB substrate (right side is  a partially de-capped module)


Analysis Procedure


1. Non-destructive Inspection


Real time x-ray inspection in analysis of these  plastic BGA modules allows quick survey of  general structural of all bumps, solder attach, substrate connections, etc.


Scanning acoustic microscope (C-SAM) on  the other hand, detects interface delamination in two modes:


(a) low frequency transducer overall  module scan


(b) high frequency transducer flipchip die bump interface scan


It detects die-bump delamination at UBM side (Fig. 2) as well as delamination between die  and under-fill.


Fig. 2:  die C-SAM of a normal die and a die  with two defective bump interfaces.


2. X-section Through Bumps


As it is used in other failure analysis field, cross-section is an indispensable means of  analysis tool on bump interfaces.  It gives a 3  dimensional view of the interface(s) of interest  in light of the information from electric test and  non-destructive inspection.


3. Module Components’ Isolation


The MCM module in discussion is constructed  in such a way that individual component can  only be (accessed) tested to a very limited  extend. In other words, In order to identify the  component at fault, non-disturbance isolation  of the components is necessary. Backside  preparation is employed to expose all the  electric contact without disturbance (Fig. 3).


Fig. 3:  Backside view of a module after all Cu  contact pads are exposed by parallel lapping.  Note: the blue box is where the flip-chip is  located


4. Bump Interface Integrity Test Method I


Die-level C-SAM is able to detect die-UBM  interface anomaly quite accurately. However  it is very difficult to discern from C-SAM image  bump-substrate side bond quality due to very  limited penetrating capability of high  frequency transducer.


Bench test found that probing on the Cu pads, with which bumps are bonded, may not be  able to detect an open or intermittent contact  because of the probing pressure acting on the  pad.


DOI: 10.1361/cp2008istfa030


New Developments in High-Resolution X-ray Computed Tomography for NonDestructive Defect Detection in Next Generation Package Technologies


Mario Pacheco and Deepak Goyal


Intel Corporation, 5000 W. Chandler Blvd., Chandler, AZ 85226 USA  mario.pacheco@intel.com (480)552-5772


The development of a next generation high-resolution x-ray  Computed Tomography (CT) tool and its applications are  reported in this paper. Some of the key features are region of  interest capability, improved time-to-data, improved usability, and data collection automation capability. We also discuss the  key technical challenges that are faced by x-ray CT  technology. Critical cases that are hard or not possible to  isolate by alternative methods are also discussed. Examples  include Controlled Collapse Chip Connection (C4) bump  cracking and “invisible” non-wetting analysis, ball grid array (BGA) solder joint cracking, and wirebond microcracking and


wirebond shorting, as well as demonstration of progressive


testing capability.


X-ray source


Rotating


The assembly package development roadmap has been


stage


increasing interconnect complexity, component density, the  number of stacked dice, material composition, while at the  same time reducing critical dimensions. As a result of these


Rotating sample


trends, the isolation and root cause analysis of defects has  become increasingly challenging for traditional analytical


→ P(θ)


.


tools and techniques. In addition, reduced time-to-information  and non-destructive approaches have become critical factors,


Detectorprojection Intensity


introducing more challenges into the analytical tools


at angle 0


development roadmap. One of these analytical capabilities is  2D x-ray imaging, which is also one of the more extensively  used tools in the semiconductor industry to isolate and analyze  defects in non-destructive fashion. Some of these capability  challenges are the detection of metal migration and dendrite  growth, C4 bump non-wetting, C4 bump cracking, BGA  solder fatigue and cracking, wirebonds and die cracking in  multi-stacked packages, etc. One of the x-ray techniques that  were identified as potentially feasible to fulfill these defect  detection gaps was x-ray CT [1,2]. However, the standard  assembly imaging techniques of x-ray CT had important  limitations in terms of defect detection capability and time-todata, and thus it needed to be extended into the next  generation. Key technical drivers for 3D x-ray computed  tomography are the need to non-destructively and quickly  detect micron and sub-micron sized defects.


In this paper, we review key technical challenges faced by xray CT technology, leading technical developments that have  overcome some of these challenges, as well as application  development for critical defect detection case studies.


X-ray Computed Tomography


The X-ray CT Operation Principle


Figure 1a shows a basic schematic of the x-ray CT operating  principle. This consists of an x-ray source, a rotating stage and  detector. The stage rotates the sample through 180o in equally  spaced angles, and the detectors collect a two dimensional  image at each angle. All 2D images are then mathematically  superimposed and processed to obtain a three dimensional  map of the sample, as it is shown schematically in Figure 1b. Information is typically displayed as a cross-section, slice  view and 3D model.


Detector


Figure 1: (a) Basic schematic of the x-ray CT setup consisting  of x-ray source, rotating stage and detector. (b) The


projections at each angle of the intensity of collected 2D x-ray  images are superimposed and mathematically processed to  generate the three dimensional image.


Technical Challenges


X-ray image resolution depends on several factors, however  geometric magnification, which is given by the ratio between  sample-to-source and sample-to-detector distances, is one of  the most critical ones. The total distance between x-ray source  and detector is fixed by tool setup dimensions, thus the  sample-to-source distance strongly limits system  magnification. Smaller sample-to-source distances provide  higher magnification and thus better spatial resolution.


One of the key technical challenges is the fact that in order to  obtain the highest possible resolution, the sample has to be  positioned very close to the x-ray source and since the sample  has to fully rotate for 2D images collection the sample hits the  x-ray source, as illustrated in figure 2. In order to avoid


sample to source collision, the sample has to be positioned far  enough from the source to freely rotate without hitting it, thus  limiting the achievable resolution. One simple solution is to  trim the sample under test so that it does not snag. However  such sample preparation consumes time, it is invasive and  non-practical in most cases.


Figure 2: The conventional x-ray system schematic faces  technical challenge: the sample has to freely rotate without  hitting the x-ray source, which limits the achievable


resolution.


Another technical challenge is the fact that x-ray CT is not a


Physical x-sections


2D x-ray image


real time imaging technique but requires many 2D images to  create tomographic information of the object consuming  several hours. In many cases this could be a show stopper. For  this reason, developing approaches to achieve data collection  and 3D image reconstruction times less than 10 minutes is


Non-wet failing bump


very important for x-ray CT technology to succeed in  integrated circuit (IC) packaging applications.


The MicroXCT 3D Tomographic X-ray Microscope


The results that are discussed in this paper were obtained  using some of the latest developments in x-ray CT technology,


Passing bump


specifically the 3D tomographic x-ray microscope, model  MicroXCT, manufactured by Xradia [3].


One of the key components of this system is a proprietary  efficient x-ray camera with pixel size ranging down to 0.65  microns, allowing high resolution in the range of 1.5 to 2   microns without the need of placing the sample close to the  source and thus allowing full sample rotation required for 3D  x-ray imaging, without sample-source collision for samples up  to 4 inches in diameter, figure 3.


X-rayBeam


scintillatorcollimator


Figure 3. Xradia Micro XCT tool configuration.


The system also uses an x-ray tube that has a maximum  voltage and power output of 150kV and 10W, respectively; this high voltage allows for effective penetration through  highly absorbing samples with features like solder balls and  C4 bumps.  Samples are mounted on highly stable, accurate  and repeatable stages, which is also important design factor  for high resolution imaging.


Results and Discussion


In this section we will review different applications in which  x-ray CT has demonstrated capability to detect defects that are  hard or not possible to detect by alternative methods.


Rotating sampleDetector


C4 Bump “Invisible” Non-Wet” Detection


Non-wet detection using 2D x-ray is based on the rounded


X-ray/9


shape of solder ball indicating non-wetting issues. When the


P(θ)


source


shape is such that it is difficult to differentiate between  passing and failing bumps due to 2D x-ray imaging  limitations, this type of non-wet is known as “invisible”.


D1D2


Figure 4 shows the physical cross section pictures of both  passing and non-wet failing solder bumps. This figure also  shows that the best 2D X-Ray image obtained using highmagnification at an oblique view angle cannot detect these  types


of


non-wet


solder


bumps.


Figure 4: On the left, physical cross section view of both a  non-wet failing C4 bump and a passing one. On the right, the  best 2D x-ray image of those two bumps indicating that they  cannot be detected.


It is possible to isolate the electrical structure that has non-wet  solder bump by electrical testing for either dead open or highresistance electric failure modes. The technical gap is to  further non-destructively isolate failing bump locations in the  failing electric structure.


X-ray


sourceRotating sampleDetector 0


Virtual 3D View


Virtual Planar view


Virtual X-Section View


Figure 5: Virtual 3D model, planar and cross section views of  a C4 bump non-wet that cannot be detected using


conventional 2D x-rays.


The objective of this application development was to establish  a fast solution to detect C4 bump non-wets along the failing  structures using x-ray CT. The results are shown in figure 5, where the non-wet is clearly visible using either virtual cross  section or planar grinding tomographic views. The typical  scanning time for C4 bump non-wet detection is 15-20  minutes per data set of 3.5mm2.


Wirebond Breaks in Multi-Stacked Packages


Wirebond breaks in multi-stacked packages are difficult to  detect with conventional 2D x-ray equipments due to both the  overlapping of wirebonds in the field of view as well as  resolution limitations. Figure 6a shows the best 2D x-ray  lateral image of a package, with several broken wirebonds. These breaks have different gaps, and the ones that are less  than 5 microns are very difficult to detect thus requiring the  development of a 3D x-ray imaging solution to image cracks  in the range of 3-5 microns.


Figure 6b and 6c show the results obtained with x-ray CT. The breaks are clearly seen using either virtual cross section (Figure 6b) or a rendered 3D image (Figure 6c). Typical  scanning time is in the range of 12 to 20 minutes, with a field  of view of 3.5mm2.


Figure 6. 6a  shows the best 2D x-ray image, unable to detect  the wire break. Figure 6b and 6c show the results obtained  with x-ray CT. The wire breaks are clearly seen using either  virtual cross section (Figure 6b) or 3D model view (Figure  6c).


。


Wirebond Shorting in Multi-Stacked Packages


Another case study involves electrical shorting caused by  wirebonds touching each other in either single die or multistacked packages. Figure 7a and 7b show the 2D x-ray  images, lateral and top views, of the suspected shorted  wirebonds from a two-dice stacked package. In this figure it is  clear that the wirebonds overlap in the x-ray image field of  view, but they do not provide conclusive data of actual  physical contact. Thus root cause analysis would typically  require a destructive analysis technique such as chemical  decapsulation, in order to get physical access to the failing  wirebonds. The main problem when using a physical deprocessing technique is the risk of releasing pressure that  could potentially hold the wirebonds together; thus root cause  key data could be lost. This was the case of the unit shown in  figure 7. It belonged to a group of units that failed with  electric shorts and recovered during failure analysis. Chemical  decapsulation and laser deprocessing were used without  success in keeping the failure mode intact.


Figure 7. 2D x-ray images showing overlapping wirebonds in  a dual-stacked package: (a) lateral view, and (b) top view.


A unit was scanned using x-ray CT. Figure 8a shows the  rendered 3D image of this unit; the yellow circle highlights  the clear physical contact between two wirebonds of the


failing electric structure. Once the tomography data is  reconstructed, the virtual rendered 3D image (model) can be


Best 2D x-ray


rotated 360o to any possible viewing angle with a spatial


image


Mechanical x-section on the other hand is still  an indispensable tool in these bump interface  analysis. It can cut through an entire row of  bumps, exposing a line of three dimensional  view of a bump contact. However, mechanical  x-section is not only time consuming to  examine bump interfaces, but also destructive  to the die under testy, wherefore preventing  the analysis from any further conduction of  die level analysis.


In order to meet the challenge of large sample  quantity with required thorough examination  of every bump interface in module reliability  test, a chemical etch approach is  experimented.


After the last layer of Cu pads (in PCB  substrate) is exposed (Fig. 3), bump under-fill (hereinafter as UF) is etched in hot sulfuric  acid. By choosing a proper temperature, UF  can be etched at a much higher rate than  mold plastic thus preserve the die and other  components from being undercut or over  etched (Fig. 4). A temp of 160oC, 90 seconds  is optimized for the particular plastic mold  compound and UF material in this particular  design.


mow2.am 20.nv x60"booin,"


Fig. 4:  Tilted view of a die after UF etch.


Fig. 5:  SEM tilted view showing comparison


of a good and failed die. These pictures


clearly demonstrate that the UF etching does  not induce artifact, even after half of the bump  is sectioned it still stands as long as its two


interfaces are intact, hence the result is


proved to be reliable and accurate.


sectioned surface


Any Cu pad or bump falling off manifests a  completely de-laminated bump-substrate or  bump-die interface.


The validity of this etching method is tested  and examined as following:


- x-section an edge row of bumps to  inspect both UBM and substrate  interface;


- de-cap the sectioned sample;


- perform the above mentioned UF etch   Fig. 5 compares the etching result of a failed  die and a good one. Both dice were xsectioned prior to UF etching.


Fig. 6: Top view of a die that showed


continuity failure under TMT (automated


electric tester), but probing at the Cu pad after  module backside preparation/isolation (refer  to section 3) is not able to detect any open  contact.


Upon UF etc, one Cu trace at its substrate


side fell off (marked by red circle). This


evidence clearly manifests bump-substrate  interface delamination on this particular bump


Note: Bottom picture of SEM tilted view


showing a smooth surface at the interface, whereby delamination took place.


Fig. 6a: Bump pull test on the same die


reveals another 3 weak interfaces at


substrate side (yellow circle).


Observation: both the shining reflection under  optical microscope and rough surface at the  left side of the SEM tilted view indicates that  the left side is the area still bonded, but it is  now torn due to pulling force.


5. Bump Interface Integrity Test Method II


An alternative approach to bump pull after UF  removal is to selectively etch Cu pads using  nitric acid, which preserves un-passivated Al  metal on the two power MOSFETs. By  controlling etch time, this etch can show  partially delaminated interface(s) without  being subject them to pulling force (Fig. 7).


Fig. 7:  Top view of a flip-chip die after UF and


partial Cu etch. Note: most of the Cu pad


bonded to bump is not etched.


Fig. 7a:  SEM tilted view of Fig. 7, i.e. after UF


and partial Cu etch.  Since every bump is  free-standing after the etc, any open bump  will fall off, and the interface whereby


separation occurs will be readily visible.


Fig. 7b:  Tilted SEM view of two examples of  defective bumps. The top one separated near  UBM due to solder fatigue; the bottom one


shows a partially delaminated interface at  substrate.


Failure Mechanisms Discovered


1. Bump fracture due to shear force from  substrate delamination.


This failure mechanism was encountered  during the initial stage of package design (Fig. 8). The root cause was diagnosed as  excessive thermo-mechanical stress due to  CTE (coefficient of thermal expansion) mismatch and inadequate substrate layout.


Fig. 8:  Overall module C-SAM image


showing substrate delamination (red colored  regions), and x-section view revealing a gross  crack that broke bumps in their bulk solder. Note: the light blue box marks the flip-chip  die.


2. Bump delamination at substrate or UBM


Fig. 9 is a section view of an open bump. It  clearly demonstrates that the bump is  separated from substrate. IMC (inter-metalliccompound) presence indicates that the  bonding was indeed formed at substrate side.  However, the significant difference in IMC  thickness (marked by yellow and blue arrows  in Fig. 9) and evidence of mold resin filled in  the gap (red arrows in Fig. 9) points that the  delamination took place during molding  process. It was later discovered that substrate  surface condition (Au plating thickness, contamination, etc) and inadequate dwelling  time in reflow process was the two  contributors to the failure. Similar  delamination is also found at UBM side.


The two pictures in Fig. 7 are tilted view of  two defective bumps: one delaminated at  UBM, the other at substrate. Both are  revealed by the Bump Interface Integrity Test


Method II discussed in the in the previous  session.


Fig. 9:  die-level C-SAM and x-section reveals  that a bump is delaminated at substrate side. The significant difference in IMC (intermetallic-compound) thickness and mold resin  filling the gap between solder and substrate  suggests that the bump was initially reflowed  and bonded to substrate, but separated  during molding process probably due to  surface condition variation, i.e. contamination.


3. Bump-UBM de-lamination or cratering


One type open bump failure was first  discovered as bump cratering damage at die  pad opening area (Fig. 10).


Fig. 10:  bump integrity test reveals what


appears to be an open bump with cratering  damage.


X-section of an open bump detected by CSAM (Fig. 11) observes that there is a line of  separation starting at both edge all the way  across the bump between UBM and pad


metal which agrees with the top view as the  result of bump interface integrity test in Fig.


10.


Fig. 11:  x-section view of a bump indicated  by C-SAM as delaminated. X-section shows  that the bump was laterally separated across  starting at both edges.


Fig. 11a:  Close-up examination shows that


the UBM interface broke at the M3 pad


opening and its nitride passivation step.


Thick IMC


Thin IMC


Mold resin


Close examination at the x-section picture of  a good bump discovers pad Al lateral  undercut under nitride passivation, with its  vacancy filled by Ni (part of UBM). The  interface between Ni and Al, TiN is  delaminated, and the TiN film is broken (Fig. 12).


This phenomenon is also observed on good  bumps by the same bumping process.


0000 5.0kV 8.7mm x45.0k


Fig. 12:  x-section view of a good bump


showing Al lateral undercut, Ni filling,


delamination and TiN film broken at both


bump edge. This is exactly the same location  where bump separation resulted in cratering  took place illustrated in Fig. 10, 11.


Feedback from FAB acknowledges that there  is Al lateral undercut or over etch due to the  nature of Al wet etch. This Al pad etch is the  first step in UBM metallization process: M3 Al  pad is etched from 0.6um to 0.4um, followed  by Zn deposition to activate the interface for  Ni plating.


Apparently, Zn was not able to reach the area  where Al lateral undercut took place. This  area is then filled with Ni which does not bond  to surface un-activated by Zn.


Consequently, this poorly bonded “ring” around the bump edge due to Al lateral


undercut becomes intrinsically weak spot of  the UBM interface.


Thus the root cause of this bump cratering  failure is identified. The bumping process is  then switched to another FAB equipped with  dry etch, whereby eliminating the failure as  such.


4. Pre-mature bump solder fatigue


Pre-mature solder fatigue that caused open  and/or intermittent contact is readily revealed  by the bump interface integrity test (Fig. 13).


DOum


Fig. 13:  Tilted SEM view of a device post  temperature cycle test. The bump integrity  test revels an open bump contact, as well as  some partial fatigued bumps.


Two probable contributors to the solder  fatigue are found: one is related to certain Cu  pad geometry, i.e. substrate layout design, which leads to higher stress on the particular  bump connected to it. The other is solder void  with irregular shape, which acts as the origin  of fatigue fracture (Fig. 14)


Al


Zn


TiN film broken


N3Si4


Al lateral over etch


Fig. 14:  X-section view of a fatigued bump. The fatigue fracture was probably originated


from the rough edge of a shown void.


Conclusion


A failure analysis process flow for flip-chip  bump interface inside multi-chip-module in  plastic package has been developed. It is a  combination of non-destructive x-ray and dielevel C-SAM inspection, x-section, component  isolation and wet etch. This analysis  procedure not only enables thorough analysis  of any specific bump having electrically  open/intermittent, but also allows examination  of every bump on the flip-chip.


Once a level of confidence in understanding  of the failure mechanisms involved in a  particular bumping/packaging process is  established, a sequential wet etch procedure  is employed, which allows quick and accurate  examination of all bump interfaces, including  partially delaminated and/or fatigued bumps. This effective and accurate sequential wet  etch is thus named “Bump Interface Integrity  Test”.


Four different bump interface failure  mechanisms, ranging from module substrate  layout design, wafer bumping process, and


assembly quality control, of flip-chip in MCM  module in plastic package are discovered.


Acknowledgement


The author would like to express sincere  appreciation to Mr. Mahmood Choudhry for  his management support. Special thanks are  due to Mr. Chuan Cheah in IR iPower  package design group for technical  discussions.


Reference


[1] Z. Wang, L. Wagner, C. Cheah “Plastic  BGA Failure Analysis Process Flow  Development”, ISTA ’01, Microelectronics  Failure Analysis Desk Reference Fifth Edition, pp-329-331


[2] Z.P. Xion, J.W. Osenbach, K.H. Chua, “Eutectic Sn/Pb Solder Bump Cracking Issue  of Large die Flip Chip BGA Package in  Electroless Ni/Immersi on Au (ENIG) Build-up  Substrate”, 2006 Electronics Packaging  Conference,pp- 196-202


[3] A. Bansal, Y. Li, D. Friyz “Reliability of  Large Organic Flip-Chip Packages For  Industrial Temperature Environments”, Online  source of Altera.com


[4] M. J. Heffes, H. F. Nied, “Analysis of


Interfacial Cracking in Flip Chip Packages


With Viscoplastic Solder Deformation”,


Journal of Electronic Packaging -- March


2004 -- Volume 126, Issue 1, pp. 135-141


DOI: 10.1361/cp2008istfa043


PCB Pad Cratering - Characterization Techniques and Challenges


Satish Parupalli


Intel Corporation, Hillsboro, Oregon, USA


Satish.parupalli@intel.com


Keith Newman


Sun Microsystems, Sunnyvale, California, USA  Mudasir Ahmad


Cisco Systems, San Jose, California, USA


INTRODUCTION


The transition to Pb-free materials has introduced  many Printed Circuit Board (PCB) interconnect  reliability challenges. New PCB laminate materials  have been introduced to survive the higher Pb-free  reflow temperatures. The increased stiffness of the  most common Pb-free solder alloy, SnAgCu (SAC), relative to SnPb, coupled with reduced interconnect  pitch and new laminate materials, have shifted the  primary failure mode in mechanical bend and shock  testing, from solder fractures to cratering underneath  the PCB pads [1, 2, 3]. Some standard  characterization techniques (solder ball pull, solder  ball shear, etc.) [4, 5] exist today for the assessment  of solder ball mechanical fracture strength; however, it isn’t clear if these test methods would also provide  characterization of PCB pad cratering susceptibility. This paper provides an overview of test methods  being investigated by a PCB pad crater industry  working group. This group was initiated during a  break-out session in the 2006 Intel/IPC Pb-free  symposium [6]. The scope of this industry working  group is two-fold:


a) Standardization of PCB pad crater crack  characterization and measurement methods


b) Development of a quantitative quality metric for  PCB pad cratering.


Based on an industry survey conducted within the  team, five PCB laminate materials with varying resin  chemistries (dicy, phenolic, non-dicy & non-phenolic) were chosen for the Phase1 study.  The test matrix  included the following test methods: cold ball pull (CBP), high-speed shear (HSS), and hot pin pull (HPP). In addition, a variety of other test variables


were also evaluated: pad design (metal defined & soldermask defined), pad diameter, and number of  reflow cycles (1X, 5X). Results of the Phase1  evaluation are detailed below. Correlations between  test methods and test parameters were derived from  the testing, to help identify the ideal test method that  could help characterize PCB pad cratering. Failure  analysis was also conducted to understand the failure  modes for the different test methods studied.


PCB pad crater crack characterization  metrologies


The initial focus of the working group was  development of a quantitative failure mode  assessment method to characterize PCB pad cratering. Conventional metrologies such as cross-sectioning  and dye penetrant testing are currently used to  identify PCB pad cratering; non-destructive methods (CSAM, X-ray) have proven less successful. Figures  1a & 1b show some typical PCB pad crater cracks  observed with the existing destructive metrologies.


7.6 mils


17.9 mils


CD


Figure 1: PCB pad crater in 1a) Cross-section 1b) Dye  penetrant test


Based on observations of pad crater cross-sections, the crack usually starts at one end of the pad and  progresses at an angle (around 45 degrees) into the


PCB laminate. Depending on the stress level, pad  design, and PCB construction, the crack may affect  the functionality of the component as shown in Figure


2.


fracture in the


BGA pad.


etchline to the


Figure 2: PCB pad crater resulting in trace open


The working group proposed the following methods  to quantify the damage due to a pad crater crack, as  shown in Figures 3a and 3b.


Figure 3: a) % pad crater = (x/y) * 100; b) % pad  crater = (L/D)*100


These quantitative methods, however, have  limitations associated with the destructive failure  mode metrologies:


a) Cross-sectioning – this is limited to a single  plane and cannot fully capture the overall  interconnect damage due to the pad crater.


b) Dye Penetrant test – the red colored dye  adheres better to solder, and does not  consistently adhere to the PCB laminate  material. Consequently, inspection of both  fracture surfaces is recommended.


Given these limitations, using both the above  mentioned techniques in parallel may improve  understanding of PCB pad cratering damage.


Development of Test Method


The second part of the Phase 1 study was to evaluate  various test methods to rank order the laminate  materials in terms of resistance to pad cratering. Table  1 below shows the various PCB laminate materials  along with other variables, i.e. test methods, test  speeds, PCB pad definition, PCB pad size, and  number of reflow cycles.


Table 1: List of factors/variables with respective  values for Phase 1 study


|Factors |Value / Type |Value / Type |
|---|---|---|

|Laminate Material |Dicy => A; Phenolic => B, C, D; Non-dicy & non-phenolic => E |Dicy => A; Phenolic => B, C, D; Non-dicy & non-phenolic => E |

|PCB pad size |10, 15, 20 mils |10, 15, 20 mils |

|Reflow condition |1X, 5X |1X, 5X |

|Metrology |Cold Ball Pull (CBP), Ball Shear & Hot Pin Pull (HPP) |Cold Ball Pull (CBP), Ball Shear & Hot Pin Pull (HPP) |

|Test Speed (mm / sec) |CBP => 5, |100, 500, |

|Test Speed (mm / sec) |1000 ||

|Test Speed (mm / sec) |Ball Shear => |5, 100, |

|Test Speed (mm / sec) |500, 1000, 2000 ||

|Test Speed (mm / sec) |HPP => 5, 15 ||

The test board used for the study was a 6 layer, 62 mil  thick PCB with 1080 prepreg material in the outer  layers & 7628 material for inner layers and the core. Figure 4 shows a schematic of the test board  construction. Test board measured 12 inch X 12 inch  with 16 individual test coupons on each board. Figure  5 below is the schematic of the test coupon layout  along with pad definition (SMD or MD). Sn 4.0 Ag


0.5 Cu (SAC 405) solder paste was printed onto the  pads using DEK Universal printing machine & SAC  405 solder spheres were placed on the individual pads  using a specially made ball placement fixture. Test  boards were sent through a Pb-free reflow profile (see  Figure 6) after ball placement & then individual test  coupons were cut out from the PCB.


D  L


PCB Pad


x Package


PCB


Figure 4: Schematic of PCB test board construction


5cm


Figure 5: Schematic of PCB test coupon layout & pad  definition (MD or SMD)


0心


00


0 D


台


TaCL


口


ahe0


品8


281


000


!..


21


0000000


SlimKIC


血


二


中


省梅南花回园8295号


时


s


Figure 6: Pb-free reflow profile used for Phase 1  study


00m100000D 8口眼


Test Procedure


Based on the factors/variables outlined above; a  Design of Experiment (DOE) was designed which  consisted of 30 legs in total & 3 samples per leg i.e. 90 samples for the study. Various legs of the DOE are  shown below in Table 2.


Table 2: DOE showing various legs studied in Phase


0 00------000中


0000 5 cr0000


000=0


0000


0000defined


Non Solder-mask 0SIder-mask defined 0


000------>20


1 study


|||[Laminate matl| Pad size (mils)||# of Reflows|Metrology|Test speed (mm/sec)|# of coupons|
|---|---|---|---|---|---|---|---|

||Leg1|226/402|。|杀|CBP|号||

||Leg2 Leg3|226/402 226/402|2|希 希|CBP CBP||m 3|

||Leg4|226/402||备 。||8 E|3|

||Leg5 Leg6|226/402 226/402|8 2||CBP|5|3|

||Leg7|226/402|10|器|CBP|E|3|

||LegB Leg9 Leg10|226/402|2||去密色|E|3 3|

||LegB Leg9 Leg10|370hr 370hr|2 0|备|去密色|o|3 3|

|||370hf|2|希|CBP||3 3|

||Leg11 Leg12||5 2|器|色|8 E|3 3|

||Leg13 Leg14 Leg15|370hr 370hr|10|益|强|1000|3|

||Leg1G Leg17||15|益 含|密 HSS HSS|500|3|

||Leg1G Leg17|370hr|15|益 含|密 HSS HSS|o|3|

||Leg1G Leg17||15|益 含|密 HSS HSS|8|3|

||Leg18||15||HSS||3|

||Leg19|370hr 370hr|15|爸|HSS HSS|1000|3 3|

||Leg19|370hr 370hr|15|爸|HSS HSS|2000|3 3|

||Leg20 Leg21|370hr|10|送|HPP|5|3|

||Leg22 Leg23||2|落 器|HPP CBP|15 5|3|

||Leg24|||||5|3|

||Leg25 Leg26||90|||8||

||Leg25 Leg26|Leg27 Leg28||2 15|爸 器 动|8||

||CBP|Leg27 Leg28||2 15|爸 器 动|88||

||Leg29 Leg30|370年|15|≤ 希|CBP CBP CBP|500 500|3 3|

||Leg29 Leg30|370hrx|15|≤ 希|CBP CBP CBP|500 500|3 3|

000e:0 10


CBP & Ball Shear tests were conducted according to  JESD22-B115 & JESD22-B117 respectively. Hot Pin  Pull (HPP) test (illustrated in Figure 7), which  involves soldering a copper pin to the pad & then  pulling the pin vertically upwards, was also explored  on one of the PCB laminate material. Once the tests  were complete; failure modes were classified based  on JEDEC test methods for CBP & Shear which are  outlined below in Table 3


Figure 7: Illustration of Hot Pin Pull (HPP) test  method


Table 3: Description of various possible failure modes  in CBP, Ball Shear, and HPP tests along with a grade  for each failure mode.


|CBP |CBP |Ball Shear & HPP |Ball Shear & HPP |
|---|---|---|---|

|Grade |Description |Grade |Description |

|1 |Ductile Failure |1 |Ball Shear |

|2 |Pad Lift |2 Pad |Lift |

|3 |Ball Lift |3 |Ball Lift |

|4 |Interfacial Break |4 Interfacial |Break |

|5 |Ball Extrusion |||

Results & Discussion


As explained in the test procedure section above; several test methods were performed on individual  pads. Figure 8 shows the pad crater % observed under  each leg of the DOE.


Var 100


|iability Chart  for Pad Crater %|iability Chart  for Pad Crater %|iability Chart  for Pad Crater %|iability Chart  for Pad Crater %|iability Chart  for Pad Crater %|iability Chart  for Pad Crater %|iability Chart  for Pad Crater %|iability Chart  for Pad Crater %|iability Chart  for Pad Crater %|iability Chart  for Pad Crater %|iability Chart  for Pad Crater %|iability Chart  for Pad Crater %|iability Chart  for Pad Crater %|iability Chart  for Pad Crater %|iability Chart  for Pad Crater %|iability Chart  for Pad Crater %|iability Chart  for Pad Crater %|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|

||-||-|and|-|- - - 一 - B E 5|- B 100||4|||1.|H||||

||-||-|and|-|- - - 一 - B E 5|- B 100|||-|-|||||*|

||-||-|and|-|- - - 一 - B E 5|- B 100|T||||1||-|T|- 1|

|-|-|-||||- - - 一 - B E 5|- B 100|8 E|86|0|0|8|6 8|||A C|

|A E A 0|A E A 0|A E A 0|A E A 0|0 E|E|- - - 一 - B E 5|- B 100|8 E|86|0|0|8|6 8|0 A|0 A|A C|

|5|5|5|400||1000|- - - 一 - B E 5|- B 100|400|1000|07|10|100|400|1002000|||5|

|||CBP tx|CBP tx|CBP tx|CBP tx|CBP 5x|CBP 5x|CBP 5x|CBP 5x|HSS|HSS|HSS|HSS||CBP 5X|CBP 5X|

罗 Pad Craber %占 20


Matertal ID


Test speed (mm/s)Metrology


g


# of Retous  Figure 8: Plot showing % of pad craters observed  across each leg of the DOE


Some of the key observations from the above plot are: a) test methods chosen were successful in  creating pad crater failure mode (see Figure  9); though it still remains a challenge to  choose/focus on the right test method


b) higher incidence of pad craters was observed  on samples made from ‘B” phenolic material  c) interestingly; no pad craters were observed on  samples made from ‘C” phenolic material  suggesting that other material properties (like  microhardness, modulus etc) would also have  an effect


d) number of reflows, test speed seem to NOT  effect the laminate’s pad crater susceptibility  e) Majority of soldermask defined pads exhibited  ductile fracture or interfacial break between  solder & intermetallic (see Figure 10)


Figure 9:  a) pad crater failure; b) pad crater failure  exposing glass fibers in the laminate


Figure 10: a) ductile failure; b) interfacial failure


Samples made from ‘C’ phenolic laminate material  did not exhibit pad crater & so would be excluded


from the graphs below. The main failure mode in this


material was either ductile or interfacial fracture.


Also; the effective output parameter (peak force,


energy) was normalized by the pad size in the


following graphs. Figures 11 to 14 show the 80020normalized peak force & energy values obtained from


the Cold Ball Pull & HSS tests in the DOE. As c0.010-


mentioned above; test speed & number of reflows did ap0.005-not have an impact on the test results in this study. "4


10.000-


Variability Chart for Normalized Force (g/mil2)


11-


+


10-


u0


K


6


15151515


un


10 02


0.71010040010002000Test Speed (mm/s)


1 u不↓~


、


-。


||AEA|B D|E|E|E|B|B E|B|E|A|A C|Material ID|
|---|---|---|---|---|---|---|---|---|---|---|---|---|

||5|400 1000|400 1000|400 1000|400 1000|400 1000|5|5|5|5|5|5|

|||CBP|CBP|CBP|CBP|CBP|CBP|CBP|CBP|CBP|CBP|CBP|

||1x|1x|1x|1x|5x|5x|5x|5x|5x|5x|5x|5x|

|Figure 11: Plot showing normalized peak force |Figure 11: Plot showing normalized peak force |Figure 11: Plot showing normalized peak force |Figure 11: Plot showing normalized peak force |Figure 11: Plot showing normalized peak force |Figure 11: Plot showing normalized peak force |Figure 11: Plot showing normalized peak force |Figure 11: Plot showing normalized peak force |Figure 11: Plot showing normalized peak force |Figure 11: Plot showing normalized peak force |Figure 11: Plot showing normalized peak force |Figure 11: Plot showing normalized peak force |Figure 11: Plot showing normalized peak force |

B


-


5x


# of Reflows 1515Pad Size (mils)


B(Phenolic)


B(Phenolic)Laminate Material Type


H


in


CBP test method


Figure 12: Plot showing normalized energy in CBP  test method


Figure 13: Plot showing normalized peak force in  HSS test method


Figure 14: Plot showing normalized energy in HSS  test method


Variability Chart for Normalized Total Energy (mJ/mil2)


mm (2 microns, Fig. 4a and b).


Material characterization of the cross-section of the end  cap of the capacitor identified Sn96 tinning with high  content of Ni, Cu, and Au (gold). This indicated that; (a) the Ni layer of the end cap was gold plated, and (b) considerable amount of Ni and Cu of the end cap  metallization have diffused into the tin layer (Figures 5a  and b). The cross-section of the soldered area of the  capacitor, where numerous whiskers had grown, identified layers of Sn-Ni-Cu and Sn-Ni-Au IMCs at the  end cap/solder interface. Chain of Kirkendall voids were  observed at the IMC/Solder interface. Islands of Sn-NiAu IMC were identified in the entire solder matrix also (Fig. 6a and b).


25x


1100x


Figure 5 (a) SEM picture showing cross-section of the capacitor. (b) Magnified view of the  marked area, shown in (a), showing elemental distribution on the end cap (in wt%).


Sn – 72  Ni – 23  Cu – 4  Au – 0.5  Ag – 0.9  Ni – 92


Cu – 6


2000 μm


20 μm


Cu – 76  Ni – 22


Figure 6 – (a) Cross-section of the capacitor. (b) Magnified view of the marked area shown in “a”. Note the layer of IMCs and chain of Kirkendall voids (block arrows) at the end cap/solder


interface. White island of Sn-Ni-Au IMC can also be seen in the solder matrix.


3.3 Discussion


A tin whisker is a conductive tin crystal that grows  spontaneously from tin-finished surfaces (in z-axis), often in needle like form, typically 1 – 3 micron in  diameter. No, single, widely accepted explanation of this  mechanism has been established, however, tin whisker  growth is primarily attributed to stresses in the tin solder.  Failure investigations of the components of the subject  PCB identified that the copper substrate, coated with Ni  and Au, was joined with Sn96 solder (96.5Sn/3.5Ag). The outermost Au-coated copper substrate serves to  protect the substrate from corrosion and oxidation, and  the Ni-coated layer provides a diffusion barrier that  inhibits detrimental growth of Cu-Sn intermetallics. However, in such combination of Sn-base solder and  Cu/Ni/Au metallization, temperature is a critical  parameter to be considered to avoid the interfacial  reactions. It seems that at the test temperature (175oC) an interfacial reaction between Sn-base solder and  Au/Ni/Cu metallization did occur, which resulted in the  formation of Sn-Au-Ni intermetallics (such as Sn4AuNi2) in the solder matrix.


There is a general agreement that compressive stress in  the tin solder is a key driving force behind the formation  of tin whiskers. Compressive stress in the tin solder may  be caused by; (a) IMC growth, (b) thermal induced  stress (such as thermal cycle), or (c) mechanically  induced stress. In this case diffusion of the end capmetallization into the solder material and formation of  intermetallics seems to be among the key contributing  factors for the formation of the tin whiskers. A  considerable compressive stress in the tin solder might


have been caused by the massive growth of the Sn-NiAu intermetallics. Diffusion of end-cap metallization from  high energy to low energy regions provides the atomic  mass transfer for whisker growth. The CTE mismatch  between the PCB and the capacitor induces mechanical  stresses in the solder joint and the capacitor body. Therefore, thermal cycle is also likely to contribute in  escalation of the compressive stress in the solder matrix. These findings contradict the speculation that high  temperature annealing may reduce the risk of tin whisker  growth.  Zhang et al. has postulated that high  temperature annealing could effect IMC formation  between tin and copper substrate [15].  It may be  because at present, factors regarding the time, temperature, type of solder material, substrate, and  barrier metals have not been adequately studied to  provide sufficient guidelines for applying annealing to  mitigate tin whisker formation. These findings have also  indicated that the application of conformal coating may  not be enough to contain whisker growth within the coat, as has been claimed in literature [16].


3.4 Conclusions and Recommendations


•


The tin whisker formation on the Sn96 solder  joints is attributed to compressive stress


generated in the solder material due to


excessive diffusion of the end-cap metals into  the solder matrix and formation of Sn-Ni-Au


intermetallics. Thermal cycling of the PCB is  also likely to escalet the compressive stress in  the tin solder matrix.


Sn – 66  Ni – 18  Cu – 11  Au – 3


22x


400X


Sn –77  Au - 17  Ni - 4


7


Sn-Ni-Au IMC


Considerable amount of gold was identified at  the end cap/solder interface.


High content of gold (up to 17 wt.%) could be  due to excessive gold plating of


the end-caps of the components. At the service  temperature diffusion of end-cap metallization  into the solder material resulted in formation of  Sn-Ni-Au


intermetallics in the entire matrix of the solder  and numerous “Kirkendall” void


formation at the end cap intermetallics/solder  interface.


Tin whiskers were straight (needle like), very  long (0.344mm), large in numbers


and they could come out of the SCC3 Conformal  coating. This shows that the


Conformal coating could not control the tin  whisker formation.


It seems that the end-cap metallization could not  resist the test temperature of 180oC. It is  therefore recommended that the interaction of  the end-cap metallization with the solder  material should be adequately studied at the test  temperature to avoid the intermetallics formation  in the solder matrix.


Thickness of gold plating, the nature of the  component substrate, and the solder volume in  the joint, all need to be considered carefully for  high temperature test of the PCB. Immersion  gold layers of 0.05 - 0.2 micron thicknesses are  adequate to offer solderability protection.  If the  gold layer is too thick, it is better to thin it before  soldering. This can be done with a hot-solder dip  procedure in which the molten solder is used to  wash away the gold-layer, replacing it with layer  of solder or tin.


[1] Darveaux et.al, Chapter 13 in Ball Grid Array  Technology, edited by John Lau, 1995.


[2] Zhong et.al. :Missing Solder Ball Failure  Mechanism in Plastic Ball Grid Array Packages:, ECTC 200, pp.151-159.


[3] Ferguson, M.E. et.al., “Manufacturing Concerns  When Soldering with Gold Plated Component  Leads or Circuit Board Pads”, IEEE Transaction  on Components, Packaging and Manufacturing  Technology – Part C, Vol. 20. No. 3, July 1997, pp. 186-193.


[4] Kramer, P.A. et. al.,  “The Effect of Low Au  Concentration on the Creep of Eutectic Sn-Pb


Joints”, Metallurgical and Materials Transactions  A, Vol. 25A, June 1994, pp. 1249-1255.


[5] KIM P.G. et.al., “Fast Soldering Reactions on Au  Foils”, Materials Research society, Symposium  Proceedings, Vol.445, 1997, pp. 131-136.


[6] Mei, Z. et. al., “Brittle Interfacial Fracture of PBGA  Packages soldered on Electroless Ni/Immersion  Gold”, Hewlett-Packard Company.


[7] Dunford, S.O. et. al., “Microstructural Evolution  and Damage Mechanisms in


Pb-free Solder Joints During Extended –40 to  125°C Thermal Cycles”, IPC 2002, New Orleans, LA, Nov 2-3, 2002.


[8] Meilunas, M. et. al., “Reliability and Failure  Analysis of Lead-Free Solder Joints,” IPC


2002, New Orleans, LA, Nov 2-3, 2002.


[9] Zeng, K. et. al., "Formation of Intermetallic  Compounds in Solder Joints and Its Effects


on Joint Reliability," Helsinki University of  Technology, report series HUT-EPT-2 2000, ISBN  951-22-4980-4.


[10] Dunford, S. et. al., “Metallurgical and Reliability  Aspects of Lead-free Mixed Technology


Electronic Assembly for Mobile Communication  Products,” IPC Works 2000, Miami, FL. Sept. 9-14,2000.


[11] Zheng, Y. et. al., “Intermetallic Growth on PWBs  Soldered with Sn3.8Ag0.7Cu,” Proceedings of  ECTC 2002, San Diego, CA., May 28-31, 2002.


[12] Zeng, K. et. al., "Six cases of reliability study of  Pb-free solder joints in electronic packaging  technology", Mater. Sci. Eng. Reports (invited), 2002, 38 (2), pp. 55-105.


[13] J. Brusse: “Tin Whisker Observations on Pure TinPlated Ceramic Chip Capacitors,” AESFSUR/FIN  Proceedings, June 24-27, 2002, pp 45-61.


[14] NASA Goddard Space Flight Center, Basic  Info/FAQ,


http://nepp.nasa.gov/whisker/background/


[15] Y. Zhang, C. Xu, J. Abys, and  A. Vysotskaya: “Understanding Whisker Phenomenon, Whisker  Index and Tin/Copper, Tin/Nickel Interface,” IPC, SMEMA Council APEX 2002.


[16] J. Kadeshch, and J. Brusse: “The Continuing  Dangers of Tin Whiskers and Attempt to Control  Them with Conformal Coating,” EEE Links, vol. 1, No. 2, July 2001.


DOI: 10.1361/cp2008istfa059


Thick Film Resistor Failures


Anshul Shrivastava, Ahmed Amin, Bhanu Sood, Michael Azarian, Michael Pecht


CALCE, Center for Life Cycle Engineering, University of Maryland, College Park, MD


Michael Zagami


Fairchild Controls, Frederick, MD


Resistors are passive electronic devices that impede the flow  of electric current in a circuit. Resistors are used in virtually  all electronic systems. Their purpose in a circuit varies. They  can be used to divide a voltage or to limit a current. There are  a variety of resistors ranging from conventional ceramic  elements, embedded resistors inside of a printed circuit board, thin film resistors, or thick film resistors. Figure 1 shows a  typical thick film resistor construction. Figure 2 shows the  thick film power resistor package that was investigated at  CALCE Test Services and Failure Analysis (TSFA) Lab. Thick film devices are “single or multilayer structures  fabricated by screen printing a layer of a specially formulated  paste on a substrate that can be made of ceramic, polymeric, or metallic material.”[2]. The paste thickness generally ranges  from a few microns to mils [1]. The material used in the  construction of a thick film power resistor include a ceramic  substrate, a resistive layer, a protective glass layer, heat sink, attach material to bond the substrate to the package heat sink, and mold compound to package the entire assembly. Figure 3  shows different layers present in a typical thick film power  resistor. Thick film resistors are widely used in consumer and  industrial products such as timers, motor controls and a broad  range of high performance electronic equipment. Thick film  resistors are commonly used in hybrid circuits, for current  sensing, power resistor or power conversion [5]. They are  used as damping resistors for pull-ups or pull-down resistors  for digital circuits [6]. Additionally, high-speed switching, snubbers, and RF systems use thick film resistors [5].


Reliability Tests


Reliability tests on resistors include temperature cycling, temperature humidity cycling, temperature humidity bias test, thermal shock test, HAST (Highly Accelerated Stress  Testing), and HALT (Highly Accelerated Life Testing).


Failure Modes & Mechanisms


Thick film resistors functionality is dependent on the electrical  circuit and environmental conditions under which they are  used.  For Panasonic thick film resistors for example, there are  very specific conditions under which the resistors will fail.  For example, they are not guaranteed to function outside of  temperature ranges of 5°C - 35°C and humidity ranges of 45 – 85% relative humidity for a given bias condition [4]. They


will not function correctly if exposed to direct sunlight or  placed in an environment of corrosive gasses such as sea  breeze, Cl2, H2S, NH3, SO2, or NO2.  These are typical  requirements for maintaining thick film resistor environmental  quality to prevent failures modes such as open or changes in  resistance values that result from mechanisms such as  substrate cracks or solder joint cracks.


Copper dendrite growth, silver migration, sulfur atmosphere  corrosion, and crack due to molding compound mechanisms  are discussed in detail in the following sections. Ultimately, these mechanisms contribute to three main failure modes, electrical open, electrical short and large changes in resistance  values.


These mechanisms are prominent when the temperature and  humidity are varied for long periods of time.  Time under  stress load condition seems to be one of the biggest factors  influencing the failure of thick film resistors.  Over time  resistors degrade after extensive use, changing their resistance  values, and eventual open circuit.  The resistive material itself, inside the resistor, may also experience degradation over time  causing a drift in resistance value.  Overloading the resistor  with too much voltage or current can also cause the resistor to  fail by changing its resistance value.


Electrode (Inner)


Protective Coating


Alumina Substrate


Electrode


(Between)


Electrode (Outer)


Thick Film Resistive  Element


Figure 1: Thick film chip resistor [3]


Figure 2: Investigated thick film power resistor


Figure 3: Different layers present in a typical thick film power  resistor, the leads are connected to the resistor internal metal  pads.


Crack due to molding compound


If the resistor is encapsulated with molding compound, the  protective-film over the resistive element may peel, delaminate, or splinter due to thermal stress or mechanical  stress as the compound hardens.  This may cause cracks in the  solder joint at the termination, and sometimes the cracks can  be filled with the molding compound itself.  This results in  increase in the resistance value or could result in an open  circuit. The crack generated in the solder joint by way of resin  mold induced stress is visualized in Figure 4.


4→R921-Untrimmed


-R921-Trimmed


-0.5


Normalized Percent Change in Resistance


101001000/10000100DOO


口一 N to


Figure 4: Disconnection by resin mold of chip resistors [4].


-1


Storage Time at 300℃ (hrs.)


Silver termination failure due to Sulfuration


When thick film resistors are exposed to a sulfurated  atmosphere, sulfur gas can seep in through the space between


the terminal plating and the resistive film. This sulfur gas can  react with the Ag present at the terminations thus causing  failure of terminations by open circuit. A sulfated atmosphere  is created through sulphur use in rubber vulcanization, sulphur


OMC/TCH


chlorination, or sulphur oil used in heated and high-humidity


3R9J


atmospheres.  The reaction velocity is highly influenced by


D1028E


sulfated gas density, temperature, and humidity [4]. The  equations that describe this destructive reaction are illustrated  below.


Ag  Ag+ + eS + 2e-  S2-


2Ag+ + S2-  Ag2S


Protective Glass Layer  Mold Compound


Resistive Layer


Substrate


Attach


Silver Migration


Failure due to silver migration occurs at the end terminations  of thick film resistors, and will be seen by the user as  electrical current leakage, dielectric breakdown, electrical  shorting, or changes in resistance value.  If the terminations of  the resistor are made out of palladium or silver, silver  migration may occur between the leads and the inner layers of  the resistor.


This phenomenon can occur when the resistors are placed in  an environment with high humidity and temperature, but it  was also observed in a normal environment when high  voltages were applied.  The common physical cause of this  type of failure is printing irregularities close to the resistor  terminals.  These irregularities concentrate electric fields  around the edges of the resistor, causing silver from the leads  to migrate into the resistor’s body.  Increased humidity, temperature, and applied voltage can all contribute to the  amount of silver that migrates and to the change of resistance  value.  A study that focused primarily on the effects of  increased storage temperature used the following formula to  graph the percent change of resistance as a function of time


[7]. Figure 5 shows the change in the resistance value over a  period of storage time at 300° C atmosphere.


%Change in Resistance = (RTIME – RINITIAL)/ RINITIAL *


Figure 5: Normalized change in resistance with storage time  at 300°C for unpowered, 100 Ohm/sq. thick film resistors. The  resistors were terminated with PdAg conductors [7].


Crack


Most thick film resistors are no more than 0.3 mm in width  and 1mm in length, and according to this same study, silver  atoms were detected as far as 100 μm from the electrodes on  either side.  The end results of this Ag migration, in addition  to changes in resistance value, are local crowding of current  density around the migrated silver, resulting in an increase of  noise, and a lower stability of the resistor’s characteristics  over time [8].


Copper Dendrites


Failure due to copper dendrites occurs primarily in thick film  resistors that have been trimmed to adjust their resistance to a  desired value. In this case copper dendrites, or branches of  copper, will form in the trimmed section of the resistor.


The copper dendrites are formed because the conductive gold  metallization layers of the thick film resistors contain trace  amounts of CuO to help bond the conductive material to the  substrate.  This copper reacts with other materials in the  resistors package to form branches across the trimmed section  of the resistor.  Copper on the surface of the resistor is more  likely to form dendrites because it is the closest to the reactive  elements in the resistor package.  This top layer of copper  causes the dendrites to form and results in electrical shorts  across the trim, which is seen by the user as incorrect  resistance values and as increase in leakage current values.


Two primary mechanisms have been attributed for this failure


[9]. The first is the migration of copper-laden molecules from  the surface of the resistor to the laser trim areas.  A chlorine  rich rinse is used as a solvent to wash the finished resistor, and  it is speculated that this chlorinated moisture could be the  medium through which the copper enters the thick film  resistor. This is especially true since CuO is soluble in  aqueous solutions.


20.0 kV 3.05052x| Lid SE 921 mm|110.0 Pa


Figure 6: SEM micrograph of dendrites.


The electrochemical reaction between the copper oxide and


0100200300400500-30


the chlorine is defined by the following chemical equation: CuO + 2 Cl-  CuCl2 + 0.5 O2


CuCl2 + electrical energy  Cu + Cl2


It can be described in three steps.  First, copper dissolves at  the thick film gold anode.  Then, as voltage is applied, these  copper ions traverse the gulf between the anode and the  cathode sides of the resistor.  The propagation of the copper is  dependent on suitable sites for growth in addition to the  availability of copper and chlorine ions.


The second mechanism is similar to the first except for the  fact that the copper comes directly from the resistor’s  packaging material itself, and is not transported by a  chlorinated rinse solution.  In this case the chlorine, ammonia, copper, and moisture from the package accumulates on the  edges of the laser trimmed region of the resistor.  The  dendrites form in a similar manner, with cupric ions being  carried between the two sides of the trim by electrical current.  This will cause decrease in the resistance values, since the  resistors are trimmed with very specifically shaped patterns to  give specific resistance values.


Temperature Failures


Thick film resistor failure is also a function of variation of  temperature.  The failure will result in varied resistance values  as temperature is varied.  At low temperatures, different types  of thick film resistors will behave differently, that is, some  may vary widely in their resistance values at low  temperatures, while some may experience no changes at all.  Thick film resistors tend to vary in resistance values as  temperature increases, as is shown in Figure 7.  If thick film  resistors are aged at extreme temperatures, these variances in  resistance values will be more pronounced.  However, for the  most part, thick film resistors seem to age well under many  different temperatures, and some may experience no failure at  all under lowered or elevated temperatures. The graph in  Figure 7, shows resistance change in percentage versus  temperature in degrees Celsius.  Up to 400°C, the resistance  change for most thick film resistors are no larger than 10  percent.


The primary variables associated with resistor failure due to  environmental temperature are the duration of time the resistor  is exposed to temperature and the humidity of the  environment.


HVSpot| MagDet SigWDPressure-10μmResistance change (%)-20102


Temperature (°C)


Figure 7: Thick film resistor behavior due to temperature  changes. [8] The red dashed lines show no more than 10% resistance change for most of the resisters.


Case Studies


Mold Compound


Protective Glass Layer Resistive Layer Substrate


CALCE TSFA lab recently investigated failures on thick film  power resistors that had gone through HALT testing. The  resistors were exhibiting electrical open. CALCE performed  an evaluation of the materials, manufacturing and assembly  processes and the testing environment to identify a set of  possible failure sites with associated failure modes and  mechanisms. A physical analysis plan was developed and  executed to investigate these sites of interest on asmanufactured (new) and failed thick film power resistors. The  analysis techniques included X-ray inspection, cross-


限BVWDSsooto.


sectioning, decapsulation, and optical and environmental  scanning electron microscopy (E-SEM) analysis.


Figure 8 and Figure 9 shows a cross-section performed at  CALCE TSFA lab showing image of different layers of a  similar good thick film power resistor. Figure 10 shows the  EDX elemental mapping of the different layers of the same  thick film resistor performed at CALCE TSFA lab.


X-ray inspection was performed on the failed resistor package  lying flat on the heat sink but it did not reveal any anomaly as  the heat sink was shadowing the internal structure of the  resistor. Finally the orientation as shown in Figure 11 was  used which revealed a vertical crack-like feature in the  resistive thick film. Figure 12 shows the x-ray image showing  the crack in the failed resistor. Similar X-ray image of a good  resistor as shown in Figure 13 reveals no crack was observed  in the good resistor.  Chemical decapsulation did not reveal  the crack. The crack found in the failed resistor was later  confirmed by cross-sectioning followed by optical imaging as  shown in Figure 14 which explains the open resistance  observance.


Figure 8: Optical image of a cross-section of a thick film  resistor showing different layers.


Figure 9: E-SEM micrograph of a cross-section of a thick film  resistor showing different layers.


Ti


Si


Sn


Ag


As


Sb


Figure 10: EDS elemental mapping shows different elements  present in different layers shown in previous E-SEM image.


Another study on similar failed thick film power resistors was  conducted. These failed resistors were exhibiting very high  resistance. Visual and X-ray inspection was performed which  did not reveal any anomaly. Cross-sectioning was performed  on the failed resistors to inspect the connection of the leads to  the thick film resistor element. In this study, the plane of  cross-sections was changed by 90 degrees, i.e. cross-sectioned  top down to expose the lead connections.  This revealed  thinning and discontinuities in the thick film conductor  metallization between the lead pad and the thick film resistive  layer as shown in Figure 15 which explains the high resistance  that the failed resistors were exhibiting. Cross-sections also  revealed that contact pad on the thick film metallization in the  failed packages were thin. Cross-sections of an asmanufactured package did not exhibit the thinning between  the lead pad and the thick film resistive layer that was  observed in the failed packages.


Mold Compound  Protective Layer  Resistive Layer  Substrate


Heat Sink


Trim


Direction of X-Rays


Figure 11: X-Ray orientation was from top to bottom at a  slight angle as shown in the figure above.


Figure 12: X-Ray image showing the vertical crack like  feature in the thick film of the failed resistor.


Figure 13: X-Ray image of a good resistor showing no crack  in the thick film at the similar location.


Figure 14: Image showing the irregular vertical crack


through the blue thick film on the cross-sectioned resistor, horizontal resistive trim is also observed.


Figure 15: Thinning between the lead pad and the thick film  resistive layer


Resistive layer


Area of Concern


Solder


Lead Pad


Grips


Top View


Although there are many mechanisms which can lead to the  failure of thick film resistors, there are only three main modes  by which users will detect these failures. These three modes  are open circuit, short circuit, and change in resistance values  as shown in


Table 1 Electrical opens and variation in resistance failure  modes were observed in case studies by CALCE TSFA..


Different failure modes and mechanisms for thick film  resistors are illustrated in Table 1.The table also lists the  potential application and manufacturing factors that cause  failure mechanisms, which then describe the failure modes.


No Crack


While changes in resistance value are more likely to occur  than a total electrical open circuit, literature shows more  failure mechanisms associated with the open and short circuit  failure mode.  Also, not all changes in resistance values will  lead to complete failure of thick film resistors.  Small changes  in resistance values might not even be noticed, especially after  some time has been spent in the field, at which point other  components on the printed circuit board will have started to  fail more catastrophically.  Even though thick film resistors  are not complicated components, they are necessary for the  functioning of any printed circuit board. By preventing their  failure, many printed circuit boards can be kept in service for  their full lifetime.


Table 1: Failure Modes and Mechanisms of Thick Film resistors


|Stresses |Failure Mechanism |Failure Mode |
|---|---|---|

|Manufacturing Factors |Silver Migration |Electrical open |

|Non-uniform thinning of electode film |Copper Dendrites |Electrical short |

|Chlorine rich rinse |Electrode crack |Variation in resistance value |

|Non-uniform thin Nickel layer |Solder crack ||

|Molding compound |Solder degradation ||

|Unsuitable soldering condition |Voltage induced breakdown ||

|Copper present in the resistor |Voltage induced degradation ||

|Poor laser trim quality |Transition of electrode material ||

|Unbalanced/excess quantity of solder |Electrode corrosion ||

|Application Factors |Crack in the resistive thick film ||

|Unsuitable pattern design |||

|Sulfur atmosphere exposure |||

|Over load causing temperature rise |||

|Voltage overload |||

|Current overload |||

|Low temperatures |||

|High temperatures |||

|Atmosphere of corrosive gases |||

[6] “Thick film resistor”: Resistor Network, KOA Speer  Electronics, Inc., Bradford, PA, USA, 7 Apr. 2005. <http://www.koaspeer.com/


[1] R.K. Ulrich (ed), L.W. Schaper (ed):  Integrated Passive  Component Technology, A John Wiley & Sons, Inc. Publication, USA, 2003


[7] J.E. Naefe, R.W. Johnson, R.R. Grzybowski: HighTemperature Storage and Thermal Cycling Studies of  Thick Film and Wirewound Resistors, IEEE Transactions  on Components and Packaging Technologies, Vol 25, No.1, March 2002


[2] M. Gargliardi: GB-280 Thick Film Devices, Processes  and Applications, Business Communications Company, Inc., Norwalk, Connecticut, USA, May 2005


[3] “Thick Film Chip Resistors”: Panasonic, Matsushita  Electric


Industrial


Co.,


Ltd.,


2008.<http://www.panasonic.com/industrial/components/pdf/AOA0000CE1.pdf>


[8] High-Temperature Electronics, ed. R. Kirschman, IEEE  Press, 1999


[9] J.B. Dixon, M.R. Northrup, D.T. Rooney: Failure  Analysis of a Hybrid Device Exhibiting Copper Dendrite  Growth on Thick Film Resistors, IEEE, 1991


[4] Surface Mount Resistors Technical Guide, Matsushita  Electronic Components Co. Ltd. LCR Device Company  Resistor Division, 1 Nov. 1999


[5] LTO 30/50/100, D2TO20, Thick Film Power Resistor: Vishay,


Accessed


9


July.


2008.


<


http://www.vishay.com/resistors-discrete/thick-film>


DOI: 10.1361/cp2008istfa065


Active Voltage Contrast and Seebeck Effect Imaging as Complementary  Techniques for Localization of Resistive Interconnections


Infineon Technologies Dresden GmbH & Co. OHG, Dresden, Germany  ingo.oesterreicher@infineon.com


Defective interconnections are a common issue in  semiconductor production and pose a problem with every new  technology generation. The usual way of monitoring process  stability and defect density is to utilize test structures in the  kerf or on special test chips. The diagnosis of the failure mode  first requires the localization of the failing via before the  visualization is performed. The exact localization is  challenging when the test array consists of several thousand  interconnections and is even more difficult when we have to  deal with contacts on active area due to leakage currents into  the substrate. Interconnections which are not open but just  show a higher resistance are also hard to find. In these cases  well known techniques like passive voltage contrast are not  successful. In our failure analysis flow we have introduced a  combination of Active Voltage Contrast (AVC) and Seebeck  Effect Imaging (SEI) to address this kind of failures.


|||||4 -|4 -|4 -|4 -|4 -|4 -|4 -|4 -|4 -||
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|

|||||- S|- S|- S|- S|- S|- S|- S|- S|- S||

|d|d|d|d|- -- --|- -- --|- -- --|- -- --|- -- --|- -- --|- -- --|- -- --|- -- --||

|-|-|-|-|||||||||||

|↓|↓||-|求||-|1||*|晰|-|||

|AE||A|BD E||E|BE|B|BE|B|E|A||AC|

||5||400||1000|5|100|400||1000|5||400|

|CBP 1x|CBP 1x|CBP 1x|CBP 1x|CBP 1x|CBP 1x||CBP|CBP|CBP|CBP|CBP 5X|CBP 5X|CBP 5X|

|CBP 1x|CBP 1x|CBP 1x|CBP 1x|CBP 1x|CBP 1x|5x|5x|5x|5x|5x|CBP 5X|CBP 5X|CBP 5X|

Pad crater is an emerging failure mode that needs  attention to avoid compromised products in the field. In this study the industry team completed the Phase 1  analysis with the main goal to evaluate the current test


言


methods at pad level with respect to pad cratering. Though the test methods were successful in creating


Material 10


Test Speed (mm/s)


pad craters; there wasn’t enough distinction between


Metrology a of Reflows


the various laminate material types based on the  output parameters. Based on the learnings from Phase  1 study & available literature; team is in the process  of completing the Phase 2 study which will be  reported out at a later stage. Phase 2 study involves


11古


selecting two test methods based on Phase 1 results & analyzing the output with respect to pad cratering  susceptibility. PCB material property correlation & tie  up with the reliability results (ex: bend, shock) would  also be part of the follow-on activities of this group.


Normalized Force (g/mil2)-00-00


H14十


40


The authors would like to give special thanks to Dage


日


no


mo


19


no dd 88


Instruments for their help to perform the tests,


151515151515Pad Size (mils)


members of pad crater industry team & Intel


management for their continuous support.


# of Reflows


References:


1. Impact of Cracking beneath Solder Pads in Printed


Circuit Boards on the Reliability of Ball Grid Array  Packages, Mukadam, M., Long, G., Butler, P., Vasudevan, V., Proc. Of SMTAi 2005


2. Lead Free Assembly Impacts on Laminate Material  Properties and “Pad Crater” Failures, Gary Long, Todd Embree, Muffadal Mukadam, Satish Parupalli, and Vasu Vasudevan, IPC EXPO 2007


3. Impact of Cracking Beneath Solder Pads in Printed  Circuit Boards on Reliability of Ball Grid Array


Packages; Muffadal Mukadam, Gary Long, Phil  Butler, and Vasu Vasudevan; Proc. Of SMTAi 2004


4. JEDEC Solder Ball Pull Test Method JESD22-B115, May 2007


5. JEDEC Solder Ball Shear Test Method JESD22-B117, October 2006


6. PCB pad craters, Gary Shade, Intel/IPC Pb-free  symposium,


March


2006


DOI: 10.1361/cp2008istfa049


Stitch-Bond-Shearing in Optoelectronic Devices, Caused by Lead-Free-WaveSoldering - Do We Need Improved Wire-Bonding Methods?


Peter Jacob, EMPA Swiss Federal Laboratories for Materials Testing and Research


CH-8600 Duebendorf, Switzerland,


Tel. +41-44-823-4288, Fax –4054, e-mail: peter.jacob@empa.ch )


Michael Rütsch, Vossloh-Kiepe GmbH


D-40599 Duesseldorf, Germany


Abstract:


This case study shows a typical example of  a manufactur-ingchain-induced reliability problem. All participants of the chain  do their work within specifications, but, looking at the system  level, severe reliability problems have been observed. In order  to get back into the system-level process window, several  corrective actions are possible. In this case, the most  promising approach is an improvement of the stitch bond  robustness, combined with a clear user specification.


Introduction:


In light railway electronics, galvanic isolation is needed  between the low power control electronics and the highpower/ high-voltage-part of the current converter circuitry, which performs the regulated vehicle motor power. In most  cases, such circuitry is designed by using either optocoupler  devices or glass-fibre-based solutions with separately mounted  optoelectronic transmitter (LED) and receiver devices. Since  the introduction of lead-free soldering on some of the control  PCBs, an increasing rate of field failures of optoelectronic  receiver devices has been observed. Each some of these  receivers are mounted together with some transmitter-LEDs in  a female sub-D-connector-frame. Statistical evaluations have  shown that some of those had been soldered manually, while  others had been automatically wave-soldered – and only the  wave-soldered failed. The devices are specified for lead-free  wave soldering at a temperature maximum peak of 260°C for  less than 3 sec. However, multiple measurements have shown  that the actual maximum temperature reached in several series  had been less than 240°C.


Physical analysis:


In order to avoid another thermal/ mechanical stress, the PCB  section around the sub-D-connector was sawn out


mechanically; thereafter, an electrical characterisation of the  failed receivers followed, using a curve tracer. The Vdd pin of  all failed parts was either open or intermittent. A mech-anical  polishing was performed in a manner, which left the pin  structure still completely embedded but it was already clearly  visible through the planar polished transparent mold (fig. 1). A  very small delamination was found between the transparent  plastic encapsulation and the voltage supply (Vdd) pin (fig.2). The same result appeared on a second sample, which has been


polished from the top instead of viewing from the side (fig. 3). Both other pins (GND and


output) were ok. More detailed investigations by optical  microscopy, SEM and FIB had shown that, electrically, the  Vdd pin intermittently became open by a broken wire bond  heel (fig. 2). If we take a look at the physics of gold wire  bonding, two substantial differences show up between the


Fig.1: Overview onto the side-polished optocomponent; left hand: ball bond onto the chip, right hand:


stitchbond onto the pin


Fig. 2: wire-bond heelcracking(dark arrow)  due to bad  bond quality and shearing force; the delamination to the  mold is indicated by the white arrow


device-side- and the pin-side-wire bonding: on the device, a  gold-ball and a steep loop is formed by the capillary wirebonding-tool, while at the pin-side, a very flat “loop” and only  a very weak wedge-like bonding are made in one step with  cutting-off the wire (fig. 6 at the end of this paper) [1]. This  setup makes the pin side wire bond extremely sensitive for  shearing, which, in fact happened systematically in case of  delaminated pins and generated the more or less completed  open. Fig.4 shows a wire bond, still connected, where the  potential shearing line is already visible (arrows).


Fig.4: Nearly cutted stitchbond on a pin. The potential  cracking line can be seen already along the small arrows


Result Discussion:


Glass Fibre Transmission Receivers and LED transmitters are  embedded in transparent plastics. The lead frame of such  devices is relatively simple, consisting of just 2-3 pins. However, the mechanical stability of these pins is weak, since  the thermal stability of the plastic encapsulation against  thermal stress from soldering is frequently at the limit, when  the enhanced temperatures of lead-free-soldering are applied. If, in addition, a mechanical pre-tension of some pins appears  due to the mechanical plugging of the sub-D into the PCB (before soldering), its relaxation is the natural consequence if


the plastic starts to melt. This is not only dangerous for the  pin-wire-bond-shearing but also performs access gaps for  humidity and external contaminations. Certainly, considering  the mechanical pre-tension, caused by the always existing  small geometrical mismatch of sub-D-pin- and PCB hole - pitch, this situation becomes more critical in such sub-D-setup  as described, compared to discrete mounted devices. Root  cause finding became more difficult even, because four parties  were involved in that case: the optocomponent manufacturer, the sub-D-assembler (who sold this product on his own, just  forwarding the solder recommendations of the discrete  optocomponent manufacturer), the PCB-manufacturer, applying the wave soldering – and – last but not least – the  final user (a manufacturer for electrical equipment of light  railways and trolleybuses), who uses this setup in a vibrationand humidity-critical environment. These components were  mounted on PCBs within current converter boxes on the roof  of such vehicles, where they are subject to extended  vibrations, weather attacks and salty fogs in winter time.


However, it should be mentioned that these devices have been  in use for many years without any problems. The problems  started with the process-conversion to lead-free soldering and  the resulting increase of the solder wave temperature to  260°C. Although both temperature, profile and time were  within specified values, the failure analysis results have shown  the obvious thermally-induced pre-damage (delamination of  plastics and pin), which later caused the wire-bond shearing, supported by operational vibration.


Improvement approaches:


In the case described here, the first approach was to increase  the geometrical distance between the soldering wave surface  and the bottom of the connector molding – such giving more  distance for both thermal and mechanical relaxation. Since  both Vout and GND pin didn’t show the effect at all, it was  proposed to redesign the lead frame geometry with respect to  improve mechanical stability and embedding into the plastics. Using a more extreme “S”-shape of the pin (fig. 5), it becomes  not only longer (=increased thermal capacitance and distance  between wire-bondpad and solder wave) but it also improves  the intensity of adhesion between mold and pin (decrease of  thermally-induced delamination risks). If useful from other  important physical characteristics and economical points-ofview, one should also consider to use plastics with a higher  melting point to avoid any delamination on future product. Furthermore, it seems to us of utmost importance to improve  the stitch bond stability and durability against vibration and  shearing stress. Of course, the best would be to have the ball  on the pin side instead of chip side. However, requirements of  economy, throughput and chip pad size limit the capabilities  of major changes. In order to improve potential and systeminduced heel cracks of stitch bonds from the beginning, we  propose to revise the bonding capillary tool geometry in a  manner, which makes the outer part looking like a microconical-cog-wheel. This would leave at least a small part of  the stitch bond uncompressed and would result in a more-orless true wedge-bond shape. The main benefit would be to  avoid the stitch-bond-typical “almost completed” pin-sideheel-cracks. Furthermore, the process-window for wirebonding parameters would be more tolerant, since within the  transient between the cog peaks and valleys of such a


Fig. 3: surface-view onto a topside-polished sample. The  delamination around the pin is clearly visible (arrow)


stitchbond tool, good bonded areas must exist in nearly any  reasonable process condition.


Fig. 5: Overall cross section. A stronger “S”-shape of the  critical pins would reduce the thermal criticality


Another approach with already some promising experimental  results has been made by using a specific new capillary tip  surface morphology, which helps to reduce the materialslipping [2].


From mechanical point-of-view, it would be furthermore  desirable to implement a (transparent) relaxation layer  between mold and pin surface, allowing more elasticity in case  of any movements of the pin, by whatever they should be  induced. If the bondpad is totally fixed by mold embedding, any harsh movement of the pin will later result in wire bond  heel-cracking or –shearing. Such potential reliability problem  increased with the implementation of the lead-free-solder  processes at higher temperatures than used before.


Similar considerations include the wirebond-loop. If it is too  flat and the embedding fixation very strong, the risk of  cracking and/ or shearing increases. This must not happen at  the pin side. Especially in case of “heavy weight”-components, like for example embedded induction-coils, minitransformers with ferrite cores etc, their big mass may result in  movements in case of vibration stress. In such cases, frequently wire-bond opens have been observed in various  analysis cases. Besides a reasonable packaging design for such  cases, good precautions would be for example a soft  embedding of the wirebond and a useful loop height.


Consequences in general for microelectronics and  customer-return F/A cases:


In parallel to the introduction of lead-free soldering, the  number of similar customer return cases in microelectronics  has increased, where the manufacturer’s retest could not  confirm the customer’s claim. Some analysis cases performed  later on normally molded (non-optical) devices confirmed the  existence of the same kind of failure. Since the decapsulation  of molded devices is done in most cases in a manner, where  only the chip-side-wire bonding is visible, while the leadframe (pin-) side wire bonds still remain mold-coated, such  failures were not discovered in many cases, yet. Since, in  addition, the wire open is only in the order-of-magnitude of  less than 1m, most 3D-X-ray equipments cannot discover  such problems.


In case of intermittent failures, or, if the retest of a customerreturn-device doesn’t show a failure, a pin-side inspection of  the wire-bond stability is strongly recommended as well as the  customer-side thermal& mechanical stress, e.g. during  soldering. Progress in latest X-ray technology, including highresolution X-ray tomography, today already allows useful Xray analysis in such cases, where the assumed or measured  open reaches at least 1um and more.open reaches at least 1m and more.


Besides the technical aspects, this case study has shown in a  very illustrative manner the various failure contributions of all  firms participating in the product manufacturing chain. As  already proposed in a former presentation at the German  power semiconductor discussion group with other case studies


[3], a general conclusion of this case is the need of an  intercompanial, end-product-related quality assurance team, of  which the reporting responsibility should clearly be oriented to  the product management team or –task force and not to each  participating company management. The tunnel-minded-view  and “limited-responsibility-feelings” of each participating  party just alone on their contribution to the product will not be  helpful for the solution of such complex problems in the  future.


Conclusion:


An unusual failure and failure context between stitch bonding  and lead-free soldering has been shown. As a consequence, in  principle, stitch bonding should be systematically improved by  a useful bonding tool redesign, including also a revision of the  extremely tolerant and vague quality criteria given in MIL883  for judging of stitch bond quality. The authors recommend a  capillary shape similar to a conical cog wheel. It has been  shown at a case study example that state-of –the-art stitch  bonding may become critical in case of the enhanced lead-free  soldering temperatures and in case of vibration stress. For  failure analysis, useful hints for the treatment of “recovered” defective devices (leadframe-bond-inspection and diagnosis  signature) were given.


[1] Dixit, V., Davis, H., Clark, M, “Wire Bonding  Considerations - Design Tips for Performance and  Reliability”, Advanced Packaging, July 2006 issue, PenWellCorp, Tulsa,OK


[2] Goh, K.S., Zhong, Z.W., “A new bonding-tool solution to  improve stitch bondability”, Microelectronic Engineer-ing, Vol. 84 Issue 1, Jan. 2007, p.173-179


[3] Jacob, P. Nicoletti, G., „Beispiele für  zuverlässigkeitskritische Konstruktionsschwachstellen in  Kleinleistungs-Hybriden und Halbleitern“, 31. Kolloquium  Halbleiter-Leistungsbauelemente und ihre systemtechnische  Integration, Freiburg i.B., 28-29. Oktober 2002 (this German  language presentation can be obtained on demand at the  corresponding author)


less than 1um, most 3D-X-ray equipments cannot discover


Pin-„S“


Connector  mold


Transparent  mold


a0


Stitch00


Melting the ball Bonding the ball


Stitchbond


wire-cut


□


Ultrasonic energy


Bonding force7


Clamp


Capillary目0 Gold wire


Pad


Fig. 6: Steps of the ball-/stitch- wire-bonding: Left: The wire is molten by an electric spark discharge; center left: The ball  is pressed onto the pad, forming the bond. Center right: The tool leaves the wire-bond, looping the wire towards the frame;


right: The capillary presses at the pin, and, by cutting ist, the stitchbond is performed. (Source: www.wikipedia.org)


DOI: 10.1361/cp2008istfa053


LEAD-FREE SOLDER/GOLD METALLIZATION INTERDIFFUSION IN ELECTRONIC  INTERCONNECTS - Challenges and their Control


Nausha Asrar


Failure Analysis and Materials Characterization Laboratory  Schlumberger Technology Center,  Sugar Land, TX-77478  E-mail: nasrar@slb.com


1.  INTRODUCTION


While most of the industries are striving very hard to  produce totally lead-free electronic products, many  concerns remain regarding lead-free solder joint  reliability. One major concern is the robustness of gold  metallization of the electronic components for lead-free  soldering. Most of the electronic components are plated  with thin gold flesh on Ni barrier layer to improve  wettability and corrosion resistance. During the soldering  process the gold readily dissolves into bulk solder. However, studies [1 and 2] of such solder joints have  shown that the gold precipitates back to the interface  after high temperature aging, forming a Au-Sn  intermetallic, AuSn4. This binary Au-Sn intermetallic is a  weak, brittle compound that degrades the thermal  fatigue life when present in high concentration in solder [3} and results in embrittlement and early failure in  electronic assemblies during thermal shocks or  mechanical shocks and/or bending. Therefore, information about the lead-free solder/gold metallization  interdiffusion at high temperature applications is very  important for controlling the technological processes for  the reliability of the electronic interconnects. A large  number of gold concentration in Pb-Sn solder have been  explored by several investigators [3-5]. According to  these works, gold has a propensity to embrittle solder  joints when present in a range of  concentrations that  extends from 2 to 7 wt.%. Other investigators [6] stated  that as a rule of thumb, gold concentration of more than  3 wt.% in a PbSn solder joint cause considerable  degradation.


While considerable amount of researches and  investigations have been made on lead-free solder joint  reliability [7-12], limited number of literatures are  available on the effect of gold content on lead-free solder  joint performance. The challenges of lead-free  solder/gold metallization interdiffusion during high  temperature application/test are; gold embrittlement, intermetallics growth, void formation, and also tinwhisker formation. Whiskers-related field failures, resulting in millions of dollars loss, have been reported  by the electronics industry since 1990 [13].  The major  failure risks are short circuits and current leakage due to  bridges. Several instances have been reported where tin  whiskers have caused system failures in both earth and


space-based applications [14]. This paper illustrates few  case histories of such challenges. These results  confirmed that the synergistic effects of void formation, IMCs formation due to the thick gold plating, and  coefficient of thermal expansion (CTE) mismatch  between organic and ceramic substrates resulted in  brittle fracture of the solder joint. The tin whisker  formation was attributed to the compressive stress in the  tin solder material, which was caused by diffusion of the  end-cap metallization, formation of intermetallics, and  thermal cycling of the soldered components.


2.  CASE HISTORY – I


2.1  Background


Electronic components soldered on a circuit board with  lead-free solder SN96 (Sn96.5, Ag3.5) failed after aging  at 155oC, 100-hours, and 100 thermal cycling at -40oC to  155oC. After the thermal cycle test the solder joint, between the Oscillator and the pad, fractured.


2.2  Failure Investigations and Results


Macroscopic examinations revealed that the solder joint  failed at the solder/PCB (printed circuit board) pad  interface. Numerous voids of irregular shape were  observed on the fractured surface (Fig. 1). Chemical  analysis of the solder by Energy Dispersive X-ray  Spectroscopy (EDS) determined high content of gold in  the solder, in the range of 9 - 12 wt.% (Fig. 1).  At higher  magnifications the solder was examined by Scanning  Electron Microscopy (SEM). SEM examinations  identified two different morphological phases, i.e. a  coarse dark  grey phase and a fine light gray phase, in  the Sn-rich matrix throughout the Sn96 solder joint (Fig. 2).  The elemental mapping indicated that the light grey  plate-like phase was rich in gold (Au) and the dark grey  phase was rich in silver (Ag). According to the Sn-Au  and Ag-Sn phase diagrams, these phases were  identified as AuSn4 and Ag3Sn intermetallic compounds (IMCs).


Figure 1 – (a) As-received Oscillator with fractured surface, (b and c) SEM picture – Note the numerous irregular shape  voids.  EDS analysis determined the high content of Au (in wt.%) in the solder.


48 x


1000 um


50 μm


990 x


Figure 2 – (a) SEM picture of the fractured surface of the solder (b) EDS analysis  determined Intermetallic Compounds (IMCs).


2.3 Discussion


The plating thickness is the most influential characteristic  of the gold deposit as it relates to the ultimate integrity of  the solder connections in regards to gold embrittlement. The criticality of gold embrittlement is ensuring uniform  dispersion of the gold in the melted solder and a final  weight percent that is less than 3-4 wt%. The thinner Au  deposits minimize Au-Sn intermetallic formation and its  concentration along the reaction interface. In situations  where thick Au deposits (>0.5 micron) are present, the  larger quantity of Au-Sn intermetallic that forms usually  segregates and cannot disperse uniformly through the  solder connection. The elevated concentrations of Sn-Au  IMCs in the areas of segregation greatly degrade the  integrity of the solder connections, especially where


cyclic thermal environments are encountered in service. This is especially critical in the confined spaces between  flat mating surfaces. In this situation, the Sn in the small  amount of remaining solder is easily consumed during  reaction with the Au, thereby resulting in a very soft, weak Ag-rich zone between very hard and brittle  intermetallic layers.


Irregular shaped voids are most common in the solder  joints of components with thick gold plating. As a results  of higher gold dissolution rate at higher temperature, the  fraction of AuSn4 in the lead-free solder joints is greater  than in Sn-3.5Ag solder. The presence of solid AuSn4  crystals increases the viscosity of the molten solder and  degrades its spreadability. The increased viscosity also


Au – 9.8


24x


2000 um


Ag3Sn


AuSn4


restricts the egress of gasses from solder during reflow, resulting in formation of numerous irregular shaped  voids, which deteriorates the mechanical strength of the  solder joints.


2.4 Conclusions and Recommendations


• The synergistic effects of void formation,


IMCs formation due to the thick gold plating,


and coefficient of thermal expansion (CTE)


mismatch between organic and ceramic


substrates seem to be the cause of brittle


fracture of the solder joint of the Oscillator.


Such failures of the lead-free solder joint


due to the formation of gold-rich IMCs is


called as the “gold embrittlement”.


• The gold embrittlement depends on the gold


content in a solder joint. With the same


thickness of gold finish, the smaller the


solder joint, the larger the possibility of Auembrittlement.  Therefore, for Au-plated


components, solder joint thickness is critical.


• Irregular shaped voids were identified on the


fractured surface of the solder.


• It is recommended that for gold plated


components, specifications for gold plating


thickness and solder joint thickness should


be developed. Based on the R&D work it


was reported that 0.05 - 0.2 micron


immersion gold layers are adequate to offer


solderability protection similar to the thicker


electroless and electrolytic plating (1.3-2.5


micron)1,2. If the gold layer is too thick, it is


better to thin it before soldering rather than


let it be dissolved into the solder joint during


soldering.


This can be done with a hot solder dip


procedure in which the molten


solder is used to wash away the Au layer ,


replacing it with layer of solder or tin.


• Thickness of gold plating, the nature of the  component substrate, and the solder volume  in the joint, all need to be considered before  accepting any qualified lead-free finish for  components.


CASE HISTORY - II


3.1 Background


During qualification test a printed circuit board (PCB) of  an electronic device of a drilling tool failed.  The circuit  board did not fail during the 120 hour aging at 180oC. However, during the subsequent thermal cycles, in the  temperature range of – 40oC to 180oC, it failed after 10  cycles (each cycle was of 2 h). During the inspection  numerous white whiskers were observed over the Sn96  solder joint surfaces of components. In addition to that, fracture of the wirebonds of a PCB-mounted chip were  observed, which caused the failure of the circuit board. In this paper likely causes of tin whisker formation have  been discussed.


3.2 Failure Investigations and Results


Firstly the SCC3 Conformal coated circuit board was  macroscopically examined under the stereomicroscope  at various magnifications (10x thru 40x). The details of  the morphology of the whiskers and solder joints were  examined under the scanning electron microscope (SEM). It was observed that the PCB was excessively  coated with SCC3 Conformal coating and the coating  was brown in color, which indicated thermal degradation  of the coating at the test temperature (Fig. 3a and b). Tin  whiskers were observed on all the solder joints of the  components. All of the whiskers were needle like and  came of the coating from the solder surface (Fig. 4a).


1234 5678 9100 THS


50 THS


123456789


Figure 3 – (a) As-received printed circuit board (PCB) coated with Conformal coating. (b) Close-up showing the whiskers on the solder joints.


48


1000 μm


100 μm


2.00 μm


X


530 x


Figure 4 – (a) SEM picture showing length of the tin whisker (0.344mm, formed within 140 hrs). (b) Close-up of the whiskers showing thickness (0.002 mm).


In order to characterize the composition of the whisker


and possible intermetallic compounds (IMCs) grown in


the matrix of the solder, the solder joints were crosssectioned and examined under SEM using the energy


dispersive spectrometry (EDS) technique. SEM/EDS


examination of the whiskers and the solder material


confirmed that the solder was Sn96 and the whiskers


were of pure tin. During the 140 hours of thermal cycle


test the whiskers had grown 0.344 mm (344 microns)


and the width of the whisker was determined to be 0.002


CO2 is often used in bond pad cleaning process and it is  generally believed that CO2 helps the formation of a more  uniform, but thinner oxide over the Al metal surface including  precipitated Cu and CuAl2, which are one of the elements for  Al Galvanic corrosion [2]. However, the effect of CO2 on via  bottom oxidation is an issue of argument. Dedicated  experiment was carried out to study the effect of CO2 on via  cleaning. Figure 4 shows the results just after via wet clean  and Ti was deposited to cap the via surface with the aim to  minimize surface oxidation and protect via bottom surface  during TEM sample preparation. The results show that there is  obvious oxidation at the via bottom of the sample cleaned  without CO2 (Fig. 4 (a)), as indicated by the arrow. For the  sample cleaned with two times the dose of normal CO2 (Fig. 4


(b)) there is no obvious oxidation. The observation supports  the statement that CO2 helps to reduce the oxide thickness on  Al surface.


Effect of plasma cleaning


A hypothesis is proposed through the analysis of the detailed  process steps. The hypothesis suggests that the introduction of  CO2 makes thinner oxide layer at via bottom, but the  following plasma sputtering cleaning step is not adjusted  accordingly and causes more damage to the Al at via bottom  as compared with the process without CO2. As a result, Al is  easier to intrude at high temperature CVD TiN step due to the  more damaged via bottom.


To simulate the combined effect of wet clean with CO2 and  plasma dry clean, an experiment was designed to evaluate the  effect of different plasma cleaning timing and different Ti  layer thickness with high CO2 dose.  It is found that Ti  thickness has no obvious effect on Al intrusion, as even 40% thinner Ti does not cause any issue. However, cleaning timing  plays a very important role. Samples with doubled plasma  cleaning show the same Al intrusion as observed in the failed  devices (Fig. 5 (a)). It is also noted that this only happened in  certain similar structures (single via on a big piece metal), and  did not occur in E-test structure. The reasons will be analyzed  later.


Figure 3 Relationship among via size, amount of Al  intrusion, poison of Al extrusion and TEM sample  location and size


TEM sample  Al intrusion


Figure 4 Effect of CO2 on via bottom oxidation (a) without CO2, and (b) with 2 times normal CO2 dose


Figure 5 Effect of 2 times sputtering clean, (a) full  process, and (b)just after IMP Ti and staying in CVD  TiN chamber for the same period of time as TiN  deposition, but without TiN deposition.


CVD TiN process step is a high temperature step and Al  intrusion is suspected to happen at this process step. The  situation was simulated by just putting the wafer (after IMP Ti  deposition) into the CVD TiN chamber for the same period of  time as normal TiN deposition, but without TiN deposition. TEM analysis also found the occurrence of Al intrusion on top  of IMP Ti (Fig. 5 (b)). Obviously Al intrusion happens in TiN  process.


Resistance consideration


As Al intrusion happens before or during TiN deposition, there is possibility that some kind of Al-N compound may be  formed. AlN is a wide band gap semiconductor and has very  high electrical resistivity (>1E+20µΩ⋅cm). The formation of  AlN will definitely cause high via resistance. However, based  on what reported in the literature [3-4], the formation Al-N  only happens at temperature more than 500 oC. But the  interaction between the TDMAT (Ti[N(CH3)2]4) precursor of  TiN and fresh Al at about 400 oC is not clear. A simulation  was performed by skipping the IMP Ti deposition, which  enabled the direct interaction between TDMAT and Al. The  E-test results showed that majority of the vias have a  resistance in the range of tens of thousands ohms. The results  indicate that there is chemical reaction between TDMAT and  Al at TiN deposition temperature to form high resistance Al-N  compound. Resistance in tens of thousands ohms range will  cause device failure.


Structure consideration


It is noted that the failed structures all belong to the type of “single via on top of a big piece of metal line” structure. The  simulation also showed that this structure is more susceptible  to Al intrusion than the E-Test structure which has a more


symmetrical layout and smaller piece of metal. This is  believed to be related to stress condition. According to Hook’s  law, the stress can be expressed as


L


E


F Δ⋅∝ ,


(1)   where E is Young’s modulus, and ΔL is elongation. ΔL can be  expressed as


L ⋅∝


Δ ε


(2)


where ε is coefficient of thermal expansion (CTE).  Al has a  CTE of about 2.1E-6, while high density plasma (HDP) oxide  has a CTE of about 0.3E-6, which is significantly smaller than  that of Al. Thermal stress is expected to build up after high  temperature process. According to Equation (2), the longer the  metal, the bigger the elongation will be.  As a result, thermal  stress will be higher in bigger metal line structure. For the via  structure, the stress at the longer metal line side will be bigger  than the stress at the shorter metal line side. This explains why  metal intrusion happens often from the longer metal line side, as indicated by the arrows in Fig. 6.


It is clear now that the introduction of CO2 into the via  cleaning process results in thinner oxide layer at via bottom, but the plasma via cleaning process is not adjusted  accordingly . Therefore it causes more damage at the via  bottom and makes the process more vulnerable to Al intrusion. As the location right above the heater has slightly higher  temperature, it becomes the preferred location for Al intrusion  to occur. The big metal structure has more astringent stress  condition, which narrows the process windows in terms of  temperature. As a result, the low yield  devices show failures  at the single via on big metal structure. From design point of  view, if the metal size can be reduced and /or more vias can be  added, the process margin will be improved.


The low yield issue is caused by the process mismatch  between wet via cleaning process with CO2 and dry plasma  via sputtering process. Higher temperature above CVD heaters  and big metal structure help the buildup of thermal stress and  result in the happening of Al intrusion at via bottom. The  failure analysis process clearly shows that a logical from big  picture to detail step-by-step approach is very important for  problem solving and root cause finding.


The authors would like to thank TEM Sample Preparation  Group of Physical Analysis, Chartered Semiconductor  Manufacturing Ltd. for the sample preparation and the  Electrical Failure Analysis Group, Chartered Semiconductor  Manufacturing Ltd. for useful discussions.


Figure 6 Correlation between intrusion direction and  metal profile: intrusion occurs from the longer side of  the metal.


[1] Dyos, G.T., and Farrell, T., Electrical Resistivity  Handbook, Institution of Electrical Engineers (1992), pp.64,


641.


[2] Scully, J.R. et al., “Localized Corrosion of Sputtered  Aluminum and Al-0.5 %Cu Alloy Thin Films in Aqueous HF  Solution  II Inhibition by CO2,” J. Electrochem. Soc. Vol 137, No. 5 (1990), pp.1373-1377.


[3] Okihara, M. et al, “Transmission Electron Microscopy


Observation of Interfacial Reactions in High Temperature


Sputtered Al Alloy/TiN System,” Appl. Phys. Lett., Vol. 66,


No.11 (1995), pp.1328-1330.


[4] Chun, J.S. et al., “Interfacial Reaction Pathways and


Kinetics during Annealing of Epitaxial Al/TiN (001) Model


Diffusion Barrier Systems,” Thin Solid Films, Vol. 391 (2001), pp. 69-80.


DOI: 10.1361/cp2008istfa075


Vdd Leakage Analysis by a Combination of Various Failure Analysis Techniques


Z. G. Song, S. B. Ippolito, P. J.  McGinnis, A. Shore, B. Paulucci, T. Kane, M. P. Tenney and F. G. Trudeau


IBM Systems and Technology Group, Hopewell Junction, New York, USA


A. W. Kozaczka


IBM Systems and Technology Group, Essex Junction, Vermont, USA


It is generally accepted that the fault isolation of Vdd short  and leakage can be globally addressed by liquid crystal  analysis (LCA), photoemission analysis and/or laser  stimulating techniques such as OBIRCH or TIVA. However, the hot spot detected by these techniques may be a secondary  effect, rather than the exact physical defect location. Further  electrical probing with knowledge of the circuit schematic and  layout may still be required to pinpoint the exact physical  defect location, so that a suitable physical analysis  methodology can be chosen to identify the root cause of the  failure. This paper has described a thorough analysis process  for Vdd leakage failure by a combination of various failure  analysis techniques and finally the root cause of the Vdd  leakage was identified.


Vdd short and leakage are common failure modes of  integrated circuits, which failure analysts routinely address. For this type of failure, liquid crystal analysis (LCA) [1], photoemission analysis [2] and laser stimulating techniques  such as OBIRCH or TIVA [3-5] are options for fault isolation. However, the hot spot detected by these techniques may be a  secondary effect, rather than the exact physical defect location. Sometimes, the exact physical defect location can be quite far  from the emission sites. To further pinpoint the exact physical  defect location based on the emission or laser stimulation  analysis, studying the circuit schematic and layout is necessary  and intensive electrical probing is also often needed. Then a  suitable physical analysis methodology can be chosen to  identify the root cause of the failure. This paper has described  a thorough analysis process for Vdd leakage failure by a  combination of various failure analysis techniques. First, backside laser stimulation analysis detected two hot spots; then intensive electrical probing identified a location with  open circuitry and finally, the carefully selected physical  analysis methodologies successfully revealed the root cause of  the Vdd leakage failure.


Failure Background and Characterization


Some blindly packaged chips of a test vehicle, manufactured  by 65nm silicon bulk technology, suffered VDD4 high leakage  failure. I-V curve tracing of one failing VDD4 versus ground  was performed for three bad units and one control unit. The IV curves, as shown in Fig. 1, manifested that the leakage was  diodic leakage rather than ohmic leakage. Zooming-in on the  low voltage portion of the I-V curves, as shown in Fig. 2, it  was found that (1) When VDD4 was below about +0.1V, bad  units and control unit showed the same current; (2) When  VDD4 increased beyond about +0.1V, the current for the  control unit decreased and maintained a low level, while the  current for bad units passed a peak and increased rapidly. All  bad units had the similar high leakage with the same signature. It indicated a systematic defect across all bad units.


Failure Analysis


As usual, the bad units were subject to backside thermal laser  stimulation analysis and it was found that two hot spots were  associated with one of the ESD protection circuits for VDD4, as shown in Fig. 3. Zooming-in further to the hot spot location  showed that the two hot spots were exactly at the two large  NFET transistors in parallel, as shown in Fig. 4. It indicated  that the high diodic leakage was from the two large NFET  transistors. However, based on the fact that the probability of  having defects at both of the two NFET transistors  simultaneously is very low, the two hot spots at the two NFET  transistors are believed to be secondary effect. This implies  that the high current at the two NFET transistors is due to a  defect at another location, rather than in the NFET transistors  themselves.


-6.0E-02-4.0E-02-2.0E-02


V


0.0E+00


2.0E-02


4.0E-02


6.0E-02


-2.0 -1.5 -1.0 -0.5 0.0


0.5


1.5


2.0


VDD4 (V)


I-VDD4 (B1)I-VDD4 (B2)I-VDD4 (B3)I-VDD4 (G)


Fig. 1 I-V curves of VDD4 versus VSS for three bad units and  one control unit showing that all bad units have similar high  diodic leakage.


-1.0E-06-8.0E-07-6.0E-07-4.0E-07-2.0E-07


2.0E-07


4.0E-07


6.0E-07


8.0E-07


1.0E-06


-0.5 -0.4 -0.3 -0.2 -0.1 0.0 0.1 0.2 0.3 0.4 0.5


I-VDD4 (B1)


V)


I-VDD4 (B2)I-VDD4 (B3)I-VDD4 (G)


Fig. 2 Zoom-in plot of the low voltage portion of Fig. 1  showing that there is a peak-point for all units at around +0.1V. After this point, the current for control unit decreases and  maintains at low level, while the current for bad units  continues increasing rapidly.


Fig. 3 Backside laser stimulation analysis showing two hot  spots associated with one of the ESD protection circuits.


Fig. 4 Zoom-in image of the two hot spots showing that they  associated with the two large NFET transistors of the ESD  protection circuit.


After backside laser stimulation analysis detected the hot spot  location, the sample was de-processed by parallel lap to metal  4, at which, all the ESD protection circuits with VDD4 are  separated each other and they are also disassociated with other  circuits. Electrical probing was performed at metal 4 for good  ESD protection circuit and the one with hot spot detected. I-V  curves, as shown in Fig. 5, clearly showed that the ESD  protection circuit with hot spot detected was defective and had  high diodic leakage of VDD4 to VSS, while the good one  showed low current. Fig. 6 is the zooming in plot on the low  voltage portion of Fig. 5. Comparing Fig. 5 with Fig. 2, it was  found that there was similar signature for the I-V curves of  good ESD protection circuit and control unit, namely, the  current initially increased until VDD4 is around +0.1V, then  decreased and maintained at low level, while for the defective  ESD protection circuit, the current continued increasing  without any peak-point, which was observed in the I-V curves  of bad units. It was understood that the peak-point appeared in  I-V curves of the bad units, but not in that of the defective  ESD protection circuit was the contribution of the good ESD  protection circuit to the total current of VDD4 to VSS for bad  units. Based on the electrical probing results, it was believed  that the defect should be below metal 4. At metal 3 level, the  same electrical probing was performed and the same results  were obtained. It further indicated that the defect should be  below metal 3.


0.00E+00


2.00E-04


4.00E-04


V6.00E-04


8.00E-04


1.00E-03


1.20E-03


0.00 0.20 0.40 0.60 0.80 1.00 1.20


I (Bad ESD Crt)I (Good ESD Crt)


Fig. 5 I-V curves probed at metal 4 showed that VDD4 has  high diodic leakage to VSS for the defective ESD protection  circuit.


1.00E-07


2.00E-07


王3.00E-07


4.00E-07


5.00E-07


6.00E-07


0.00


0.10


0.20


0.30


Fig. 6 The zooming-in plot of I-V curves at low voltage  portion of Fig. 5


The sample was further de-processed to metal 2, where all of  the components: the NFETs, Inverter, Resistor and Capacitor  of the ESD protection circuit, as shown in Fig. 7, are separated  from each other according to GDS layout. With reference to  the schematic of the ESD protection circuit, the NFET high  diodic leakage could be due to the following failure  mechanisms rather than the NFETs themselves (1) The  capacitor (C) is leaky, leading to turn on of the NFETs; (2) The Resistor (R) is open, resulting in loss control of the  NFETs, or (3) The Inverter (INV) is malfunction, like stacking  on “1” at the output.


VDD4


NFET


INV


R


非


Fig. 7 Schematic of the ESD protection circuit.


To verify all the suspected failure mechanisms, electrical  probing was performed at metal 2 to verify the function


I(V)


integrity of the Capacitor, the Inverter and the Resistor. The IV curve of the Capacitor, as shown in Fig. 8, shows diodetype curve at both negative and positive voltage sides, because  parasitic diodes exist. However, at the low voltage portion  between - 0.3 Vs to + 0.3Vs, no high leakage is observed. It  indicates that the Capacitor is in good function.


-1.00E-09-8.00E-10-6.00E-10-4.00E-10-2.00E-10


2.00E-10


4.00E-10


6.00E-10


8.00E-10


1.00E-09


-0.5 0


-0.4


-0.3 0


-0.2 0


-0.1 0


0.00 0.10 0.20 0.30 0.40 0.50


V (V)


Cap of Bad ESD Crt


Fig. 8 The I-V curve of the Capacitor.


Fig. 9 shows the input-output characteristic of the Inverter. It  clearly shows that when the input is low, the output becomes


high, vice versa, when the input is high, the output becomes  low. It manifests that the Inverter functions properly.


-0.40


0.40(A)0.80


1.20


1.60


2.00


30


Data point


0.40


0.80


!人


:


Vinput Voutput


Fig. 9 The input-output characteristic of the Inverter.


The I-V curves of the Resistor for good and bad ESD  protection circuits are showed in Fig. 10. It is found that for  the good ESD protection circuit, a linear portion of curve is  observed, indicating an Ohm resistor, while for the defective  one, the Resistor shows open circuitry. At the negative side of  the I-V curves beyond -0.1 V, the diodic leakage is due to  parasitic diode as observed in the I-V curve of the Capacitor.


-1.4E-05-1.2E-05-1.0E-05-8.0E-06-6.0E-06-4.0E-06-2.0E-06


2.0E-06


4.0E-06


-1.5


-1.0


Good ESD crt Bad ESD crt


Fig. 10 I-V curves of the Resistor (R) for good and bad ESD  protection circuits showing open circuitry for the bad one.


With the further fault isolation by electrical probing, the  sample was finally de-processed to the metal 1 level and SEM


inspection was focused on the Resistor path. It was found that  two defective via 1, which connected the Resistor to the  VDD4 line, as shown in Fig. 11, was open.  To further  understand the root cause of the via 1 open, a second sample  was analyzed by the same methodology and it was also  verified to be resistor open circuitry by electrical probing. For  the secondary sample, a Focused Ion Beam (FIB) tool was  employed to cross-section the suspected open via 1. Fig. 12  shows the FIB cross-section image of the open via 1. The  image shows poor liner metal coverage and Cu void in the  via1 and metal 2 layers. Thus, the root cause was believed to  be contamination during pre-clean of liner-deposition. The  contamination affected liner metal deposition, leading to poor  liner metal coverage. Poor liner coverage affected Cu seed


nucleation, which in turn affected Cu ECP, resulting in poor  Cu filling in via 1 and metal 2 layers. Poor Cu filling led to via  1 open.


Fig. 11 SEM image showing defective via 1 causing the open  circuitry for the first unit.


Fig. 12  FIB cross-section on the defective via1 for the second  unit showing poor Cu filling via 1 and metal 2.


Summary


Vdd leakage issues can be addressed by global fault isolation  with LCA, photoemission or laser stimulation techniques. However, the hot spot detected by these techniques may be a  secondary effect. To pinpoint the exact defective location, further local fault isolation may be required by electrical  probing. Once the defective location is identified, the  appropriate follow-on physical failure analysis technique can  be chosen for the root cause analysis. This paper has  demonstrated the methodology of Vdd leakage analysis by a  combination of various failure analysis techniques. In this case, the hot spot was detected at the two large NFET transistors of  an ESD protection circuit by backside laser stimulation  analysis, the via 1 open was finally identified associating with  the Resistor of the ESD protection circuit with extensive  electrical probing and follow-up physical analysis. The via 1  open causing loss control of the input of the Inverter of the  ESD protection circuit led to high current flowing in the two  large NFET transistors.


[1] K. A. Cooper and S. J. Schwartz, “A Novel Proactive  Failure Analysis Technique Using Liquid Crystals”, Proceedings, ISTFA, pp. 219-221 (1992).


[2] N. Khurana and C. L. Chiang, “Analysis of Product Hot  Electron Problem by Gated Emission Microscopy”, Proceedings, IRPS, pp. 189-194 (1986).


[3] K. Nikawa and S. Tozaki, “Novel OBIC Observation  Method for Detecting Defects in Al Stripes Under Current  Stressing”, Proceedings, ISTFA, pp. 303-310 (1993).


[4] E. I Cole Jr, P. Tangyunyong and D. L. Barton, “Backside  Localization of Open and Shorted IC Interconnections”, Proceedings, IRPS, pp. 129-136 (1998).


[5] R. Aaron Falk, “Advanced LIVA/TIVA Techniques”, Proceedings, ISTFA, pp.59-65 (2001).


DOI: 10.1361/cp2008istfa079


Physical Failure Analysis Techniques and Studies on Vertical Short  Issue of 65nm Devices


P.K. Tan, Z.H. Mai, S.L. Toh, E. Hendarto, Q. Deng, Y.W. Goh, J.L. Cai, Y.Z. Ma, H.B. Lin, L. Zhu, J. Yu, H.L. Li, Q.F. Wang, R. He, H. Tan, J. Lam


E-mail: tanpk@charteredsemi.com, Tel: +65-63604015


With the scaling down of semiconductor devices to  nanometer range, physical failure analysis (PFA) has become  more challenging. In this paper, a different method of  performing PFA to identify a physical vertical short of intermetal layer in nanoscale devices is discussed. The proposed  chemical etch and backside chemical etch PFA techniques  have the advantages of sample preparation evenness and  efficiency compared to conventional PFA. This technique  also offers a better understanding of the failure mechanism  and is easier to execute in identifying the vertical short issue.


Short and open issues are common back-end-of-line process (BEOL) in wafer foundry, especially as integrated circuit (IC) devices become smaller. This is induced by modification in  the process flow such as application of low k dielectric  material, thinner inter-metal-dielectric (IMD) layer and  lithography issue/optical proximity correction (OPC). In  order to locate the short location, techniques such as the use  of liquid crystal analysis (LCA), laser scanning microscopy (LSM), infrared thermal detection (ITD) method [1] and  focused ion beam (FIB) circuit edit (CE) are utilized. In older  technologies, the commonly seen physical short type is  horizontal such as metal bridging. Most horizontal shorts can  be easily observed under optical microscope (OM) or  scanning electron microscope (SEM), but for vertical short, the PFA methodology to identify the root cause is more  difficult. Vertical short is always covered by the overlaying  stacked metal structures. Very often, Passive Voltage  Contrast (PVC) technique is required to locate the defect area [2-3].


This paper focuses mainly on the different types of defect  localization and the unique PFA method to identify the root  cause of vertical short issue on 65nm IC devices. The vertical  short discussed in this paper is rarely seen, and is unable to  be captured by electrical test (ET) structure.


Analysis Flow before FA


Wafer lot was sorted after full wafer processing and the yield  loss was categorized into different bins. Wafer map was  plotted and ET data were studied in order to understand and


isolate the highest possible failing layers or issues. If this  could not be done, the wafer would be submitted for FA. Fault  isolation would be performed to identify failed location, followed by layout study for further PFA.


Two case studies with conventional PFA techniques and new  techniques were discussed in this paper.


Case study 1


In case study 1, conventional and non-conventional PFA  methods were discussed. This case study is base on 65nm  device in which, many Vdd and Input/Output (IO) pins were  shorted to Vss. More than 40% yield loss on this issue and no  failed ET were captured. Figure 1(a) shows the wafer map of  the short failing dies. Wafer at failing sites were microprobed  to verify on the short. Figure 1(b) shows the I-V measurement  of the failing die and passing die. The short resistance is  around 18ohm, so it is most likely a back end of line (BEOL) issue, in particular, metal short issue.


1001003456812345678


20000002000000


40m0030300222032oN220


6o207202503150320


2ON5。00


0602N00200


c220e 4口32□220  7ONCN21207202N2200  90032020900222000800N22008022N2220  10C02010002000


11


10110000


Figure 1: (a) Wafer map of short issue. (b) I-V measurement  of the short and passing die.


Wafer 3 POR


Wafer 8 CA/PC


Legend


3FailPass


• Bin 0 pass die


• Bin 1,2,3 failed short at different


pin such as IO pin/Vdd and etc.


-1.5E-04


-1.0E-04


-5.0E-05


∞0.0E+00*********---------..--5.0E-05


1.0E-04


1.5E-04


-0.02


0.08


0.18


0.28


0.38


Bad Die Good Die


LCA was carried out on a few dies, and hot spots were found  only at the probe pads area. LSM was used to identify defect  area because it has higher resolution than LCA. Backside  LSM was used due to the presence of dummy metals and  thick top metals that will prevent the laser beam from  reaching the layers below as shown in Figure 2(a) and 3(b). Backsides deprocessing of failed and good dies were thinned  down  to  around   300µm   for  backside  LSM  measurement.


VDDIO


PA range0(gpio) signal


Figure 2: (a) Cross sectional view of 7 metal layers structure  of sample. (b) Simple layout of the devices at failing pad.


Figure 3 shows the Optical Beam Induced Resistance Change (OBIRCH) image of the failed die from the backside of the die. The OBIRCH spot was found at the corner of the failing short  pin. Layout study was carried out based on both the spot  location and electrical data. According to the layout study in  Figure 2(b), the possible shorted layers are only between Via5 (V5) below and above Metal3 (M3). The possibility that short  occurred in other layers was very small, as there was large  metal (M) gap and also no related circuit presents. If the short  occurred horizontally, it could be observed by OM during  delayering.


The first OBIRCH sample was delayered using the  conventional PFA technique, parallel lapping and layer-bylayer inspection [4]. Figure 4(a) shows the SEM image of the  abnormal bright PVC after lapping away M5, but because of  the unevenness of sample, it is very difficult to identify  whether it is an artifact or real defect. The unevenness is  caused by the very thick and large top metal which reduces  suddenly to a very thin layer of metal with thin V4 IMD  thickness as shown in Figure 2(a). Sample unevenness is one  of the disadvantages of parallel lapping, especially for  technologies smaller than 90nm [5-6]. Figure 4(b) shows the  TEM image of the abnormal bright PVC spot, showing that Cu  from M5 filled the trench and shorted to M4. It was suspected  that this shorting was caused by plasma arching effect in the  process chamber when high voltage was applied. The plasma  arching is random and irregular in shape.


10mV_650uA


Emission spot location


M4 M5 RX


Figure 3: OBIRCH result from LSM, spot found near fail pad  edge area.


Al Bond pad


Metal7 (M7) , Cu


Via6 (V6), Cu


Metal6 (M6), Cu


Via5 (V5), Cu


Metal5 (M5), Cu  V4, Cu


Metal4 (M4), Cu  V3, Cu


Metal3 (M3), Cu   V2, Cu


Metal2 (M2), Cu  V1, Cu


Metal1 (M1), Cu


Contact (CA), Poly, Active


OBIRCH spot found  at pad corner


In order to view and verify the short profile efficiently, a nonconventional PFA method was adopted. This nonconventional PFA method can overcome the problem of  unevenness in parallel lapping. A failed sample was  deprocessed to V5 and then Reactive Ion Etch (RIE) was  used to expose M5, as illustrated in Figure 2(a) from black  dot line to black solid line with RIE (black arrow). The Cu  M5 was then etched away by nitric acid (HNO3). If there  were no short between M5 and M4, the Cu of M4 would not  be removed by HNO3. Figure 5(a) shows the optical image of  the failed short pad after M5 Cu was etched away by HNO3. A hole on the 4th M4 can be observed from optical  microscope. The hole got bigger as the etch time by HNO3  increased. It is obvious that M4 of the 4th Metal from top is  being etched away through the trench that shorted M5 and  M4. Figure 5(b) shows the SEM image of the abnormal  trench. The IMD collapsed due to the weak support after  removing portion of M4 Cu by HNO3. Figure 5(c) shows  Transmission Electron Microscopy (TEM) image of the  trench (labeled as 1) that shorted M5 and M4 with Cu  material already removed by HNO3. With this method, the  whole failed pad can be inspected thoroughly without facing  the unevenness problem. This new technique offer better  efficiency in deprocessing time and also flatness. The process  has been improved after feedback, and currently this device is  already in production with high yield.


Figure 4: (a) SEM image of bright PVC at OBIRCH spot  area after lapped away M5. (b) TEM image at PVC area.


After 120s Cu remove by HNO


Floating Ta barrier layer of Via5 after Cu material etched away


that short to Metal4


Abnormal trench


Figure 5: (a) Microscope image of failing pad after removal  of V5 and M5 Cu by HNO3. (b) SEM and (c) TEM image of the  abnormal trench that short M5 and M4.


Cu filled in the trench and  shorted Metal5 to Metal4


(b) (a)


Bright PVC observed  after lapping away


Metal5 at OBIRCH  spot area


TEM


M4 expose due to very  large pad size and


cause unevenness in  sample lapping


Low


Metal4


cover


by IMD


Remaining


M4 Cu


Floating Ta barrier of


V5 after Cu was  removed


The trench that


shorted M5 and M4.


IMD collapse due to bad support after  removing M4 Cu by using HNO3


The


remained  M4 Cu


after M5  remove by  HNO3


Cu of Metal4 etched away through  the trench that short to Metal5.


Case study 2


In case study 2, the sample preparation was more  complicated in order to truly identify the root cause of  vertical short. Case study 2 was a 65nm device from a  different customer process which had same pad short issue as  in case study 1. Both methods described in case study 1 were  used. Although both methods can locate the short defects, neither is able to explain how the short is formed.


Figures 6(a) and (b) show SEM and TEM images of using  both methods to find the short defects. Same as previous case, it is difficult to find defect in samples using normal parallel  lapping method (Fig. 6(a)) due to the unevenness of sample  preparation on large area. The chemical etch method (Fig. 6(b)) as described in case study 1 has the advantage of larger


inspection area, therefore abnormal trench that short to M4  can be found easily. TEM for both methods observed trench  that shorted M5 and M4. From both results, V5 was suspected  punch through and short to M4, because all defects that found  have almost similar size with V5, and have no sign of random  shape trench as mentioned in case study 1. The issue is not  solved after feedback. Unfortunately, the conventional PFA  method is only able to identify why it failed short but unable  to pinpoint how the short formed. A backside sample PFA was  proposed for this case. Backside PFA had been reported  earlier in literate, but it was mostly used for transistor level  inspection [4]. The new proposed PFA technique was backside  PFA with chemical etch method. The new techniques not only  identify the root cause, but also can overcome the unevenness  problem of parallel lapping, especially for technology smaller  than 90nm.


This paper shows that AVC and SEI are complementary  methods to localize defective interconnections in cases where  passive Voltage Contrast or other laser scanning techniques  fail.


Active Voltage Contrast


Voltage contrast is widely utilized as a localization method for  opens (or shorts) on circuits and test structures. However, if  used in a passive way without applying voltage to the circuit, this approach implies that a clear distinction between a  floating and a grounded part of the circuit is possible. When  this is prevented by design or defect type, passive voltage  contrast reaches its limits. For example, contact chains on por n-doped substrate are very hard to analyze since the whole  structure is not floating. Small leakage currents are running  from each contact into the substrate layer which makes  passive approaches impossible. The contact chain cannot be  charged by the electron beam and remains bright in the SEM  contrast even when the chain is interrupted by an open  contact. There are two ways to overcome this problem: One is  the recently developed Active Voltage Contrast [1]. We use a  probing system (Kammrath & Weiss) which is integrated into  a FEI dual beam tool. A bias is applied to one side of the  chain, and the other side is put on ground. With the applied  voltage the chain is charged on a level that compensates the  substrate leakages. This leads to a visible contrast in the SEM  image which can not be seen with passive techniques. The


point between the dark and bright areas marks the open  interconnection and allows direct x-sectioning and imaging in  the dual beam tool.


The same method is performed when interconnections on  higher metallization are to be analyzed. If a low ohmic defect  is suspected a direct active approach is preferred. Even if a  successful localization by passive voltage contrast is not  excluded prior to analysis and would be the easier way, it is  often skipped as the DUT is irreversibly modified: To enable  PVC one side of the structure is usually grounded by milling a  hole into the pad to connect it with substrate thus making  subsequent active biasing difficult.


Seebeck Effect Imaging


Seebeck Effect Imaging [2] has advantages over Active  Voltage Contrast when the failing structure is hidden under  several metal layers. Mechanical delayering to enable voltage  contrast can be difficult if the test structure is very large  because the required lateral uniformity is not always reached. The thermoelectric effect of local heating by an infrared laser  beam on the junctions is monitored at the pads that connect  the chain. The images presented below were taken with a  Hamamatsu Phemos1000 using an IR-laser.


Although the lateral resolution of SEI images is limited by the  laser wavelength it delivers additional information compared  to AVC. Not only open vias are localized, but small  differences in resistance between the interconnections can be  made visible yielding a two dimensional resistance mapping  of the test structure.


Via Localization Challenges


The test structures used for this paper are especially designed  to monitor the via defect rate in the manufacturing process  continuously so the quality and yield loss due to via problems  can be estimated. Some of them are placed in the kerf, but  most of the structures shown below are Characterization  Vehicle® test chips on dedicated wafers (designed by PDF  Solutions, Inc., 90 nm technology, see figure 2).


A via improvement strategy based on large test structures  requires the ability to localize all types of via defects for root  cause identification. Four cases can be distinguished, where  passive voltage contrast is ineffective:


• Contact chain on p- or n-substrate with hard open


• Contact chain with soft opens (increased resistance) at one


or more positions


• Contact chain with higher resistance but all contacts are


affected equally


• Via chains on higher metallization with increased


resistance


In these cases AVC and SEI are the only suitable localization  methods and complement each other.


O" SEI


Figure 1: Localization of high resistive interconnections


SEI: The laser energy is converted to a heat gradient resulting  in an SEI signal which is higher at a resistive via.


AVC: The electron beam generates secondary electrons that  are reflected towards the detector in the grounded part of the  chain, while being deflected by the applied potential in the  biased part.


Results


Contact chain on p- or n-substrate with hard opens


Due to the small feature size contact chains are more often  affected by defects than vias on higher metallization. A set of  contact chains with numerous hard opens is shown in figure 2. All of the chains are connected by the same ground pad. When Seebeck Effect Imaging is executed, one microprobe is  enough to contact all of the chains at the same time. The  opposite electrode is represented by the substrate and the  grounded chuck, respectively. In this setup not only unbiased  conditions can be used for localization, also OBIRCH/TIVA  could be chosen. The resulting contrast basically shows the  area that is electrically connected to the microprobe and thus  marks the point where the chain is interrupted. In figure 2, only the chain in the middle does not have a hard open. Additionally, areas with different intensity of the SEI signals  can be recognized (see the arrows in figure 2) indicating high  resistive contacts.


Two of the chains are enlarged in figures 3 and 4. In figure 3 a  contact chain on substrate with two opens is shown where  three areas with different contrast can be differentiated with  both methods. The position of the open contact is marked in  the SEI images by the alternating contrast. In figure 4 only


one open is detected, a small step in the border line can be  seen at the open position (arrow).


As already described above, active biasing of the contact  chain is needed for voltage contrast imaging to compensate  leakage currents into the substrate. In figures 3 and 4 the AVC  image is shown above the SEI image. It corresponds well to  the SEI image and allows the localization of the same open  contact.


AVC is able to localize the first open contact on the side that  has been electrically connected. A second open contact can be  made visible by contacting the other end of the structure.


electron beam


More opens in between can only be localized under certain


IR-laser


conditions: A voltage contrast difference is reached if the  areas between two opens are significantly different in size. In  this case these isolated areas vary in their sheet resistance and  thus in their discharge behavior. In figure 5 we found two  opens at the positions marked with the arrows, furthermore  another open contact was seen at the far left end of the chain (position outside of the image). The area on the right side is  bright because it’s actively connected to ground; the left area


ITIUIL


is grey because it is positioned between two opens and  isolated from the pads; the area in the lower middle is also


AVC


isolated by opens but is the darkest because it has the highest


。。


sheet resistance due to its small size and is charged the most  by the electron beam.


Figure 2: Overview of a set of contact chains that was used  for this study (SEI overlay image). All chains are contacted by  a common ground pad and show the position of several opens  at the break off point of the red SEI signal areas. Note also  the different shades of red in some of the chains indicating a  soft open (arrows). In the inset a typical defect is shown: The  left contact is not completely filled.


Figure 3: AVC and SEI image of a contact chain on substrate (two hard opens) with Si-NAIL. The chain (90nm technology) was connected at both sides so three regions with different  contrast were visible. The area in the middle between the two  opens is not directly connected to the pads.


In the lower image the superimposed SEI image with high  magnification with a NAIL is displayed (backside mode).


Compared with AVC, SEI has the disadvantage of lower  lateral resolution. This drawback can be reduced by  immersion lenses. In figure 3 SEI was performed in backside  mode to allow the usage of a Si-NAIL (Numerical Aperture  Increasing Lens [3]). As can be seen in the lower image, at  least the horizontal lines consisting of the contact bridges can  be resolved in 90 nm technology (compare fig. 5 for SEM  resolution).


Figure 4: AVC/SEI comparison on contact chain on substrate  with both soft and hard opens.


Upper image: Active Voltage Contrast image, lower image: Corresponding Seebeck Effect image. The structure is  contacted with two probe tips. AVC clearly shows the position  of the open, whereas SEI additionally marks numerous  contacts with increased resistance (bright and dark spots), thus allowing a two-dimensional resistance mapping.


Figure 5: AVC on contact chain with different shades of  contrast. Contrast depends on the area between the opens: The chain is darker between the two marked opens because  the area is much smaller than the rest of the chain on the left  side. The small area leads to a higher sheet resistance to  ground and stronger charging by the electron beam.


SEI AVC


opens


SEI with NAIL (superimposed)


SEI


Contact chain with soft opens (increased resistance) at one  or more positions


If the contact chain is not fully open but just a slightly higher  resistance is measured, we are able to retrieve a similar  voltage contrast as with hard opens. A little tuning of the  voltage is needed to reach a stable contrast condition. The SEI  image looks quite different, as no strong contrast is obtained. In figure 1 there are numerous „soft opens” found in addition  to the hard open. Additional dark and bright spots show up  pointing to contacts with slightly different resistance. The  structure is contacted by two microprobes, so the soft opens  are visible on both sides of the hard open. SEI provides a  resistance mapping image that shows the lateral distribution of  resistive contacts over the test structure and also correlates the  resistance magnitude with signal intensity (small spots in  figure 4).


In comparison, AVC will at least show the position of the  contact with the highest resistance. Other resistive contacts  can sometimes be localized by slowly increasing the applied  voltage, so the dark/bright frontier jumps to another position.  A detailed qualitative overview of the resistance distribution  can only be done with SEI, which has the higher electrical  resolution in this application.


Figure 6: Via chain between metal 1 and metal 2 with a  resistance value 1% above spec.


Exact localization with SEI down to an area of two  interconnections using a NAIL is possible (130nm  technology). Overlay with layout is shown in the lower image.


Contact chain with higher resistance but all contacts  affected equally


When all interconnections are affected in the same way, the  resistance of the chain may be similar to a chain with one  open interconnection only. This can’t be decided by the  electrical data. The localization with SEI or AVC in this case  does not show any contrast across the chain. A continuous  change from bright to dark between the two sides of the  structure will be observed with AVC, and a SEI image will be  uniform. This is also valuable information as it excludes e.g. a  defect density problem and points to a processing issue.


Via chains on higher metallization (without substrate  contact) with increased resistance


If the electrical path is not completely open, passive voltage  contrast will not give any results. This issue can be treated by  both AVC and SEI. A satisfying contrast can be reached in  AVC by applying a bias that compensates the small residual  current flow. With SEI we can localize the same defect even if  the chain is masked by upper metal layers.


The interesting question is the reachable sensitivity. In figure  6 a chain of interconnections between metal 1 and 2 is shown. The chain consists of 800 vias and is interconnected with three  identical chains in a bridge circuit allowing a four point  measurement. The chain exhibited a resistance merely 1% higher than that of its neighbors which translates to a  resistance increase of a factor of 15 for one via, assumed that  only a single via is affected. In a fab environment this case  represents the lowest resistance limit we have to deal with in  practice, as most via chains are much larger and the lowest  detectable resistance increase of a single via is accordingly  much higher. Moreover the electrical test structure parameters  are usually only measured with two probes and with lower  electrical sensitivity than in this example.


While we were not able to do successful localization with  AVC, Seebeck Effect Imaging showed a strong signal after  short integration time marking the suspicious area. With the  use of a NAIL and layout overlay (fig. 6), it was possible to  exactly localize the defect down to an area of two  interconnections. The analysis was performed in backside  mode through the substrate and poly layer.


Active Voltage Contrast allows localization of resistive  interconnections under conditions that have previously  prevented successful analysis, especially contacts on substrate  or chains with slightly increased resistance. Seebeck Effect  Imaging provides additional lateral resistance mapping in case  of soft opens and makes differences between the  interconnections visible with very high sensitivity.


Drawing on the example of test structures used for via quality  monitoring, we showed that the two physical approaches yield  different information and complement each other. AVC has  advantages in lateral resolution and speed as it allows  localization and direct cross sectioning in one step. While SEI  often overlaps with AVC, it makes resistance mapping of a  large area possible and is the method of choice for marginal


resistance increases with high sensitivity. To save time and  money, SEI is often used first in our FA flow to preselect the  chips for AVC as we can localize large structures and even  through metal layers.


Only the combination of AVC and SEI delivers the complete  view on resistive interconnection issues and covers the full  resistance range.


The authors wish to thank PDF Solutions, Inc. for their  cooperation and support with the CV® test chips.


We would also like to thank L. Bauer and M. Kawka for  numerous FIB and VC analyses and P. Klose for electrical  measurements.


[1] R. Rosenkranz, W. Werner, “Active Voltage Contrast for  Failure Localization in Test Structures,” Proc. of the 29th  International Symposium on Testing and Failure  Analysis, ASM International (2006), pp. 316-320


[2] E.I. Cole, P. Tangyunyong, C.F. Hawkins, M.R. Bruce, V. J. Bruce, R.M. Ring, W.L. Chong, “Resistive  Interconnection Localization,” Proc. of the 27th  International Symposium for Testing and Failure  Analysis (2001), pp 43-57


[3] S. B. Ippolito, B.B. Goldberg, M. S. Ünlu, “High spatial  resolution subsurface microscopy,” Applied Physics  Letters, Vol 87, No. 26 (2001), pp 4071-4073


DOI: 10.1361/cp2008istfa070


A Logical Problem Solving Process for High Via Resistance Root Cause Analysis


K. Li, P. Liu, J. Teong, M. Lee*, and H. L. Yap*


Failure Analysis, Quality Reliability and Assurance  * Fab 3


Chartered Semiconductor Manufacturing Ltd


60 Woodlands Industrial Park D, Street 2, Singapore 738406, Singapore


This paper presents a case study on via high resistance issue. A logical failure analysis process EDCA (Effect, Defect, Cause, and Action) is successfully applied to find out the  failure mechanism, pinpoint the root cause and solve the  problem. It sets up a very good example of how to do tough  failure analysis in a controllable way.


Failure analysis of modern semiconductor integrated circuit (IC) devices becomes more and more challenging as IC  devices shrink in dimension and get more complicated in  design and processing steps. Device miniaturization often  requires high spatial resolution fault isolation and physical  analysis. For contamination and implantation-related issues, high sensitivity (good detection limit) is also needed. Due to  the inherent resolution limitation of some of the analytical  techniques such as secondary ion mass spectrometry (SIMS), process simulation in larger structure has to done. The  complexity in process steps sometimes also makes design of  experiment (DOE) or simpler split experiment necessary.  Very often a combination of analytical techniques has to be  employed. More importantly, to tackle the major low yield and  field return  issues, an EDCA logical failure analysis  methodology has to be established first. Prior to intensive  detailed electrical and physical failure analysis looking first at  the big picture (effect), such as low yield category, low yield  location distribution (wafer map), lot history, tool  commonality, preventive maintenance schedule and time-link, helps to set up correct failure analysis direction, which can  significantly improve failure analysis resource utilization  efficiency, cycle time and success rate.


800-


In this paper, we report a case study of a low yield issue  related to high via resistance in a quarter micron device with


600-


aluminum backend. A logical step by step failure process was


0 Runo


applied here to resolve the issue.  The initial fault isolation


400-2


based on the failure mode and circuit design indicated that the


200-


problem was due to high via resistance in the range of tens of  thousands ohms per via. A thorough analysis was performed


0-


on affected lot time frame, tool commonality, process history,


Posibion (nm)


020406080100


and failure location distribution. Based on the information  obtained and analysis results from the failed units, the  suspected process step was narrowed down to pre W via


process modules with Via cleaning process and chemical  vapor deposition (CVD) of TiN barrier being most susceptible. A systematic simulation of the process steps was performed  and the failure observed phenomenon in the failed units was  successfully repeated. Based on the results the effect of Via  cleaning with CO2 was clear and the failure mechanism was  established. Further analysis of the common characteristics of  the failed locations suggests that design improvement can also  widen the process window.


Logical Failure Analysis Process  Initial Failure results


High failure rate was reported for several devices. Through  initial circuit analysis a via structure was suspected. Circuit  simulation indicated that the via would cause problem if its  resistance was in the range of tens of thousands ohms. TEM  analysis was performed on the suspected location of several  failed units, and the typical results were shown in Figure 1. The image contrast suggests that the via bottom is abnormal  and there might be Ti/Al intermixing. An EDX line scan was  performed across the via bottom (Fig. 1 (b)). It showed that  the Ti and Al signal overlaps and this confirms the occurrence  of intermixing or inter-diffusion of Al and Ti. As diffusion is a  thermally activated process, this anomaly was initially  suspected to be linked to process temperature, and most likely  to CVD TiN deposition temperature. Wafer map check shows  that the low yield dice fall into an annular zone, which  matches the heater position of the TiN CVD process very well. This further supports the idea that the problem is


Figure 1 (a) Abnormal via bottom profile, and (b) EDX  line scan across via bottom along the white line in (a).


AJ


temperature related. However, the temperature history chart  did not show any anomaly.


Another concern is whether Ti-Al intermixing is able to cause  device failure, as simulation shows that the device will fail  only when the resistance is in the tens of thousands ohm range. There are different forms of intermetallics between Al and Ti, and the two most common forms are TiAl3 and Ti3Al. The  resistivity of TiAl3 and Ti3Al are 26 and 210 µΩ⋅cm  respectively, while the resistivity of Al and Ti are 2.7 and 42 µΩ⋅cm respectively [1]. The resistance change based on the  thickness of the Ti-Al intermixing layer is about 0.1Ω  to


0.15Ω, as compared to the 1.3 Ω resistance of a normal via  without Ti-Al intermixing. Obvious the increase in via  resistance through the forming of Ti-Al intermetallics is not  big enough to cause the failure.


TEM analysis was continued on more failed units. A clearer  via bottom picture was finally obtained (Fig. 2 (a)), most  probably due to better TEM sample positioning. A white layer  is sandwiched in between the top W layer and another dark  layer on top of bulk Al. To understand better the materials  configuration, energy filtered TEM (EF-TEM) imaging  technique was applied for elemental mapping.  Ti mapping (Fig. 2(b)) clearly shows that the dark layer is Ti. There is also  faint contrast right underneath W, suggesting that Ti and TiN  might be separated. Moreover, Ti penetration into Al at the


right bottom corner is observed. N mapping (Fig. 2 (c)) further  suggests that TiN layer might be separated from Ti layer. Oxygen map shows the presence of O at the two via corners  and where Ti diffuses into Al.  Al mapping (Fig. 2 (d)) shows  clearly the intrusion of Al in between Ti and W (TiN).


To get a clearer picture, high spatial resolution (2 nm) electron  energy loss spectroscopy (EELS) line scan was performed  across the via bottom along the white line in Fig. 2 (a). EELS  has much better energy resolution (0.8 eV) than energy  dispersive x-ray (EDX) (~135 eV) and can resolve Ti and N  easily. The result shows two separated Ti peaks and one N  peak, which is at the same location as the first Ti peak. Obviously, the first Ti peak corresponds to TiN and the second  Ti peak corresponds to IMP (Ionized Metal Plasma) Ti. In  between is Al.


The reason why Fig. 1 looks differently might be due to the  fact the sample is not cut right on the extruded portion and the  Ti/TiN barrier forms the background. The scenario is depicted  in Fig. 3. The relative position between intruding Al and TEM  sample and the extent of Al intrusion affect the final TEM  image.


Now the question is why Al intrusion happens and whether it  happens right before TiN deposition or it happens after TiN  deposition. To answer these questions, a thorough analysis of


Figure 2 (a) Zero-loss image, (b) Ti map, (c) N map, (d) O map, and (e) EELS line scan across via bottom along  the line in (a)


lot time frame, tool commonality, change of process steps, wafer map characteristics, and etc. is needed


Commonality analysis


Analysis of the time frame of the affected lots showed that the  issue happened after CO2 was introduced into via clean  process. When CO2 was turned off, the issue disappeared; when CO2 turned on again, the issue reoccurred. There seems  to be some correlation with the introduction of CO2.


Wafer map check showed that the failure location was annular  shaped, matching the position of TiN heater quite well. However, temperature trend check did not show anomaly. The  location right above the heaters is expected to be of higher  temperature than the rest of the areas, therefore it is more  vulnerable to Al intrusion.


It is important to understand the effect of CO2 and its  correlation with Al intrusion. The correlation between Al  intrusion and via high resistance is also needed to be  understood.


Effect of introducing CO2 into via clean


Figure 1: This is a 3D model of an area within a module  with a suspected solder short. This type of view is an  excellent tool to show the location of a potential fail site.


Figure 2:  This 3D model (pseudo color) shows the  capacitor with a solder short on the top surface.


3D


Overview


Figure 3: This is a virtual cross sectional slice of the  solder short, capturing the defect in its entirety.  This  aspect of the XCT data is exceptional, since top  down polishing to expose package level defects is  rarely used.  The solder short was also measured  using the MicroXCT.  This short ranged from 12 um  to 247 um in width.


Top lapping or polishing to expose this defect would be


>1 3.3221139 CHz -1.7121 d0


0.000


09 532 Log Mag 10.o0d8/ Ref w4o.o0d8 [F3 08m]


difficult because of possible overshooting, or polishing  through the failure area.


-10.00


-20.00


-30.00


-40.00


-50.00


-60.00


-70.00


Figure 4: The physical cut would have to be made at this  exact location to capture the entire short, provided the  whiskers from the short are in a relatively straight line.


Example 2 – Failure Analysis of open connections in  an LC Filter


Open or short solder defects in LC filters  are also  common defects within wireless modules which  traditionally require tedious cross sectioning, but can  now be easily resolved using XCT. These defects are  often left undetected since RF probing is typically  needed to detect an open or a short.  Depending on the  defect, DC probing is useless as these devices normally  exhibited a DC open or short, depending on the filter  being used.


The surface mount device (SMD) filter was isolated from  the rest of the module using a precision laser cutting  system and it was verified as the source of the module  failure using a network analyzer (figure 5).  The network  analyzer data revealed an open on the output side of the  device.   2D X-ray imaging of the filter output area  revealed no definite fail site (figure 6).  An XCT scan of  the suspected region clearly shows an open solder  connection (figures 7 & 8). A physical cross section of  the filter was performed to verify the accuracy of the CT (figure 9).


-80.00


Figure 5: A network analyzer was used to verify the  failure. The forward transmission measurement showed  a possible open on the output side of the filter.  The bad  curve is compared to a passing unit in this log mag  chart.


Figure 6: This a 2D x-ray image of the output of the


failing filter.  There is no clear fail site shown from this


inspection.


Figure 7: This 3D view from the XCT data shows a  possible open solder connection


0.000513.323LSED CH24.0211 89


20.03


20.00


-40.00b


50.55


-00.20


Figure 8: This image shows an X-ray virtual cross  section of the open solder connection


-的


Figure 9; A physical cross section was performed to  verify the CT results and the findings were virtually  identical.


Another less common defect with these LC filters is  cracked via.  These via are imbedded within the ceramic  package and are also undetectable using DC curve  tracing and 2D x-ray.  As with the open circuit, the only  way to detect this type of failure would be to use RF  probing.  This particular LC filter failed after a  temperature cycle reliability test.  The S parameters  showed a potential mismatch (figure 10).  XCT was used  to analyze and inspect the filter (figure 11), showing  cracked via, which were also confirmed using physical  cross sectioning (figure 11, a, b).  The physical cross  sectioning verified the results of the XCT data but also  appeared to introduce additional damage to the metal, most likely due to the polishing process.  The XCT data  shows the area of interest without disturbing the cracked  region or introducing additional damage.  It also allows  the examination of several via on the same device  without additional physical manipulation.


Figure 10: This log mag chart shows the fail signature,


compared to a passing filter.


Figure 11: (a) CT Cross sections vs. physical cross  section and optical imaging of LC via (b), the latter  shows cracks as well as additional material loss, which  most likely occurred during the polishing process.


Example 3 – Failure Analysis of Inductors


>1 66.629517 MHz 1.0285 0 1.8771 n 4.4837 mH


A bad or shorted inductor can be difficult to troubleshoot  in an RF Module. This is primarily because most  package inductors exhibit no electrical signature when  using conventional DC curve tracing. When using DC to  probe an inductor, all that is shown is a short circuit.  Two common ways to verify the function of a package  level inductor is to us an LCR meter, or by using a single  port reflective measurement with a network analyzer.  The latter is the most useful since using an LCR meter  usually requires that the device under test be removed  from the package.  This could destroy any evidence of a  fail site.  The following images (12 & 13) show how XCT  was used in conjunction with an RF probe station to  expose a defect within an SMD inductor.  This is another  defect that would normally go unseen, but with XCT, the  defect is exposed and there have been no destructive  methods utilized.


Figure 12: This S11 measurement shows the inductor


value to be approximately 5.6 nH at 66.6 MHz.


This inductor came from a module that was verified to be  a passing device


Figure 13: This S11 measurement shows the inductor  value to be approximately 4.4 nH at 66.6 MHz.


This inductor came from the failed device and the  inductance is shifted approximately 1.2nH.


>1 66.629517 mz 857.98 ma 2.3309  5:5678 nem


This inductor was part of a matched output for a SAW  filter.  The device failed in the TX/RX band and the test  data was similar to that normally seen in a SAW failure.  The SAW was initially tested on the RF probe station  and it failed.  However, for verification, the matching  circuit was cut out and the SAW was tested again and it


passed.  This led to the testing of the individual RF  testing of the inductor, which was verified as a failure.  The device was then scanned using the XCT and the  results can be viewed on the following figures (14 &15).


Figure 14: This is a 3D model of the suspected failed


inductor (Psuedo color). A metal defect was seen in the  highlighted area


Good


Inductor


Failing  Inductor


seom 3


Figure 15: X-Ray cross sectioning was used to perform a  top down cross section, exposing the defect in its


entirety.  This defect changed the value of this inductor, causing the failure in the TX/RX parameter


Example 4 – Failure Analysis of SAW Filters a(80.201m 1131


91 1.7111186 0H2 21.788 0 -55:425 01 6780 pF


The Xradia MicroXCT has been invaluable for finding  defects in SAW filter packages within RF modules.  SAW  filters are like inductors when it comes to failure analysis.  Typical methods can not be used to efficiently  troubleshoot a SAW.  SAW filters must be tested using  an RF probe station and careful subsequent analysis  must be performed to expose a failure.  Some typical  failures seen in these filters are open solder  connections, solder extrusion, cracked die, open bumps  and the occasional assembly defect. Some examples of  these are shown in the following images.


Figure 16: (a) 3D Model of the area of the filter with an  open solder connection, (b) with an X-ray virtual cross


P


sectional view.


Figure 17: This is a top down virtual cross section of the  filter.  This slice shows where the solder is connected to  the laminate metal traces.  Notice that the open pad (at  the colored cross hair) has very little solder, as  compared to the metal traces around it.


1 Seament Sweep


Order Bese


p721 33 2a1n 04j 8te 1090[33


3 37311184 01 2 1844 0 -19 296 0 4-0102 F


1 segment Swp


Crer biee


Figure 18: These S parameters indicate a short in one of  the SAW filter outputs (b) compared to a normal plot (a).


Figure 19: This 3D model of the filter shows a possible  metal defect beneath the die.


Figure 20: X-ray virtual cross section shows the defect  between the output area of the die and a GND trace.


Figure 21: After the non destructive analysis was  performed, the substrate was removed and a thorough  optical inspection was performed, exposing a metal  defect that was shorting RFOUT to GND


In conclusion, we describe a non invasive FA technique  for RF modules and its passive components using a high  resolution and high contrast X-ray micro computed  tomography system. This technique has been shown to  dramatically improve our FA engineers’ chances of  identifying defects over conventional 2D x-rays, and  avoid the need for physical and tedious cross sectioning  of these devices.  Using the XCT helps eliminate


questions by personnel that may doubt the results of  destructive analysis based on possible induced or  removed damage or defects.  Using the machine allows  for positive use of the Analysts time, all of the data is  non destructive, and it is stored for unlimited retrieval for  reviews and for FA training for new engineers.


[1]    Johnson, J, et al.,: Virtual Histology of transgenic


Mouse Embryos for High-Throughput Phenotyping.,


PLoS Genet 2(4): e61 (2006)


[2] Bentz, D.P, et al., : Microstructure and transport


properties of porous building materials, II: 3D x-ray


tomographic studies, Materials and Structures,


33(227),147-153 ( 2000)


[4 [3] Levine, Z.H., et al.: Tomography reconstruction of


an integrated circuit interconnect, Applied Physics


Letters, 74(1), 150-152 (1999)


[4] Scott, D, et al.,: High Resolution 3D Tomography


for Advanced Package Failure Analysis, ISTFA


Proceedings


[5]  Lau., S.H, Non destructive characterization, inspection,    failure analysis of advanced components and sensors with a  high resolution and high contrast microCT, Proceedings, 25th  Army Science Conference, 2006


Ventony Fryar: RFMD Failure Analysis Technical


Supervisor


Bynum Ferguson:  RFMD Failure Analysis Engineer


Ben Wray:  RFMD Sr. Failure Analysis Technician


David Shuttleworth: Sr. Failure Analysis Engineer


Randy Love:  Sr. Failure Analysis Technician


Stephen J. Miller:  RFMD Engineering Manager


Michael Antonell, PhD: RFMD Senior Engineering


Manager


DOI: 10.1361/cp2008istfa099


Scanning Acoustic Microscopy for Solder Joint Failure Analysis  and Design Improvements


Ramesh Varma, Jeffrey Bartolovitch, Victor Brzozowski and Carl Sokolowski


Northrop Grumman Electronic Systems


7323 Aviation Boulevard, Baltimore, MD21240 Email: ramesh.varma@ngc.com


This paper reports using Scanning Acoustic Microscopy for  solder joint failure analysis and process and design  improvements.  There are reliability concerns associated with  solder voids or non-wetting of the solder to the bond pads  which is particularly important for higher electrical power or  temperature applications.  Defects in solder can also occur and  grow during operation and thermal cycling.  Sonoscan is an  attractive non-destructive test to characterize solder joints and  is often used to study the growth of defects during life test  simulations.  X-ray imaging cannot identify very small  defects, particularly non-wetting and delamination because of  poor resolution.  The instrument used in this study was a CSAM (C-Mode Scanning Acoustic Microscopy) operating in  reflection mode at 30-100 MHz.  We have identified voids  inherent in the solder layer as well as delamination at the  package to solder and solder to heat-sink interfaces.  C-SAM  results confirmed that the delamination was caused by CTE  mismatch of the materials as well as the mechanical stresses  caused by higher level package integration and module  assemblies.  Thermal cycling studies have shown that typically  the voids do not grow whereas delamination does.  These  results were used to improve thermal heat-sinking and product  reliability by minimizing defects in solder joint by changes in  process and mechanical designs.


Reliability of solder joints has been studied extensively, but  mostly using cross section and SEM/TEM analysis.  Effects of  intermetallic compounds [1] and CTE mismatch between  surface mount components and the PCB [2-4] on the thermal  fatigue of solder joints have been reported.  From a practical  point of view, a non-destructive technique is very useful for  continuous monitoring of product build and process controls.  X-ray imaging, Scanning Laser Acoustic Microscopy (SLAM), and C-SAM are typically being used in the industry  for inspecting board assemblies.  In our study, we have used  C-SAM to continuously characterize the defect growth in  solder joints as the assembly goes through higher levels of  assemblies and thermal cycling.


Experiment & Results


A schematic configuration of the package assembly is shown  in Figure-1.  A power transistor is attached to a heat-sink  using SnPb solder using standard reflow processing.  The Xray image (110kV, 40uA) of the assembly is shown in Figure2.  The voids in the solder joint can be seen clearly in the


X-ray image.


Fig-1:  Package schematic assembly


Fig-2:  X-ray Image


Figure-3 shows a C-SAM scan using a 30 MHz transducer and  the gated region including reflected signals from both  Interfaces A and B.  Interface A is between the heatsink and  solder whereas Interface-B is between solder and the package.  Though the voids seen using C-SAM are comparable with the


Transistor Package


Metal Heat-Sink


Solder  Joint


Interface-A


Interface-B


Void


X-ray, C-SAM shows additional features that are not seen in  the X-ray image.  Figure-4 and Figure-5 show C-SAM images  taken with reflections from interfaces A and B separately  using a narrower gate.


Fig-3:  C-SAM Image showing delamination


Fig-4:  C-SAM image


(Interface-A, Heatsink – Solder)


Fig-5:  C-SAM image


(Interface-B, Package – Solder)


The C-SAM image shows more features than X-ray indicating  that the defects in the solder interfaces are more complex.  The  red and yellow areas shown in C-SAM images indicate  delaminations or non-wetting areas that are not identified by  high resolution X-ray.  Red areas are clearly voids or  delaminations and yellow area may be initiation of  delamination. More importantly, using selective gating on reflection peaks we have been able to identify that the voids  and delaminations are located at the heat-sink Interface A.  This information is very important in understanding the root  cause of the defects and in eliminating them by improving the  assembly process.


One of the packages was separated from the heat-sink by  pulling it after heating the assembly very close to the solder  melting point.  Care was taken to make sure that the solder did  not melt to distort the interface signatures.  An example of this  is shown in Figure-6.  Optical image of the de-soldered  surface shows features indicating wetting and non-wetting  areas as well as voids similar to that observed in C-SAM  images.  Desoldering a package requires heating it close to the  solder melting point and hence the solder interface may not  give the true picture as it may be disturbed during the  mechanical removal of the package and therefore, this method  should not be used quantitatively.  Here the purpose of this  test is to show that delaminations are real and can be observed  by C-SAM which is often not detected by X-ray.


Fig-6:  De-soldered Package


We have analyzed the de-soldered surface at several spots  using EDS (Figure-7) which showed that this interface is  slightly Sn rich, most likely from the Sn plating on the heatsink.


Delamination


Fig-7:  EDS


The board assembly was thermal cycled and characterized by  C-SAM.  Figure-8 shows C-SAM image after 500 cycles.  Solder separation is clearly visible after 500 cycles and this  separation occurred mostly at the solder-heatsink Interface A.


10249


Fig-8:  C-SAM image after 500 Cycles


Figure-9 shows increase in solder separation with thermal  cycling.  The yellow areas generally change into red  confirming that this area is indeed a transition region and  further studies are required to understand this mechanism.  The un-bonded area was calculated using image processing  software.   Solder separation increases almost linearly with  cycling.  No defect saturation was observed even after 750  cycles.  Thermal modeling has shown a CTE mismatch  between the package and heatsink materials leading to a  redesign of the package assembly.  Figure-10 shows thermal  cycle data after assembly redesign and process optimization.  In Figure-10, the defect area did not grow as in Fig-9 and  saturated at about 10% compared to about 40% before process  optimization.


0 10 20 30 40 50


018_209_10 193-0210 -A3A1


600 8800


Cycles


Fig-9: Thermal Cycling before design change


0 10 20 30 40


% Unbonded Area


50


600


Fig-10: Thermal Cycling after design change


We have studied solder joint degradation using C-SAM and  identified the root cause due to CTE mismatch of materials.  By redesigning the package and optimizing the assembly  process, we have significantly reduced the solder joint  degradation and improved thermal heat-sinking and product  reliability.


[1] P.L.Tu and Y.C.Chan, Effect of intermetallic compounds  on the thermal fatigue of surface mount solder joints, IEEE  Trans. Comp., Packaging and Manuf. Tech., Part-B, Vol.20 (1), pp 87-93, Feb 2007.


[2] D.R.Frear, Thermomechanical fatigue of solder joint: A  new comprehensive test method, IEEE Trans. Comp., Hybrid, Manuf. Tech., Vol.12, pp 492-501, Apr. 1989.


[3] V.K.Garj, Reliability of surface mount solder joint, Proc. 4th Int. Microelectronics Systems’95 Conference, June 19-23,


1995.


[4] S.M.Lee et.al., Grain boundary sliding in surface mount  solders during thermal cycling, IEEE Trans. Comp., Hybrid, Manuf. Tech., Vol 14, pp. 628-633, Mar. 1991


Solder Separation


DOI: 10.1361/cp2008istfa102


Lock-in-Thermography for 3- dimensional localization of electrical defects inside  complex packaged devices


C. Schmidt, F. Altmann, C. Grosse


Fraunhofer Institute for Mechanics of Materials, Halle, Germany  fa@iwmh.fhg.de, phone: +49-345-5589170, fax: +49-345-5589101


A. Lindner


Micronas GmbH, Hans-Bunte-Str. 19, D-79108 Freiburg, Germany


Achim.Lindner@Micronas.com, phone: +49-761-5172359, fax: +49-761-5172174


V. Gottschalk


ELMOS Semiconductor AG, Dortmund, Germany


vgottschalk@elmos.de, phone: +49-231-7549295, fax: +49-231-7549189


It has been shown that microscopic Lock-in-Thermography (LiT) can be used for localization of electrical active defects  like shorts and resistive opens in integrated circuits. This paper  deals with the application of LiT for non-destructive failure  analysis of fully packaged single and multi chip devices. In  this case inner hot spots generated by the electrical defects  typically can not be imaged directly because the mold  compound or adhesives above are not IR transparent. Inner hot  spots can only be detected by measuring the corresponded  temperature field at the device surface. By means of failed and  test devices will be shown, that LiT is sensitive enough to  measure such temperature fields. In addition to the lateral  localization of inner hot spots its depth can also be determined  by measuring the phase shift between the electrical excitation  and the thermal response at the device surface. Furthermore, the influence of the lock-in-frequency and mold compound  thickness to lateral resolution and signal to noise ratio will be  discussed. Using real failed single chip and stacked die devices  two analysis flows were demonstrated to locate inner defects.


Modern system in package (SiP) or package on package (PoP) devices are getting more and more complex. Therefore, the  localization and analysis of electrical defects inside such a  complex three dimensional built up can be difficult and time  consuming. Especially for this kind of devices methods are  required which are able to detect defects in a non-destructive  way because every preparation step can effect the failure mode  or destroy the overall functionality of the device. Additionally, in multi chip devices electrical active structures, like ICs or


interconnects are often vertically stacked. Therefore defect  structures are covered by surrounded materials. Only the upper  chip level can be investigated using standard failure  localization techniques like OBIRCH [1], liquid crystal  thermography [2], or emission microscopy after removing the  mold compound by opening the device. Lower chip- or  interconnect levels can not be investigated by this methods in a  non-destructive way... Furthermore, assumed shorts between  bond wires could be removed by etching the mold compound. In such cases only non-destructive-testing methods are  necessary to localize defects. There are only several, very  specific methods known satisfying these requirements. Time  domain reflectometry (TDR) can be used finding the failure  site by measuring the delays of electrical signals. Magnetic  microscopy [3] uses the fact that every current flow generates  a local magnetic field, which is not affected by the surrounding  material. It will be shown that LiT can also be used for nondestructive testing, measuring the corresponding temperature  fields at the device surface caused by inner hot spots.


As shown in literature, the method of LiT is a sensitive and  easy to handle method for hot spot detection on chip level. [4],


[5], [6]. The defect is stimulated electrically by a periodically  pulsed supply voltage which produces a periodically thermal  response. This response is detected by a free-running IR  camera and is split into an in-phase-part and an out-of phasepart related to the excitation signal by using two correlation  functions.  From these basic signals the amplitude and the  phase signal of the thermal response can be calculated:


)²


(


phase


out


S


amplitude


−


= arctan


Using these two signals, the main advantage to the steady state  thermography can be seen clearly. Due to the periodically  pulsed excitation the heat spreading and therefore the thermal  blurring is lateral limited which is direct related to the lock-infrequency. In addition, due to the lock in amplifier principle  the detection limit is improved by the 3-4 orders compared to  the steady-state-thermography. Nevertheless, the phase signal  contains information about the time delay between electrical  stimulation and thermal response. This phase shift is  influenced by thermal spreading inside the mold compound or  adhesives and can be used for three-dimensional defect  localisation. the basic principle is explained in Figure 1.


Figure 1: Sketch of the heat expansion in an excited device. Depending on the depth of the defect a phase shift ∆Φ  between excitation and detection occurs due to heat  conduction through the layer system.


Typically, the mold compounds or adhesive materials are not  IR transparent. Therefore inner hot spots generated by  electrical defects can not be imaged directly. But inner hot  spots can be detected by corresponded temperature field at the  device surface. Heat flow is a time-depending process. Therefore, a phase shift ∆Φ between excitation and detection  of the local heating occurs depending on the depth of the  defect and the thermal behaviour of the material. Visa versa, by measuring the phase shift the depth of the defect can be  determined. The phase shift value depends mainly on heat  conduction, heat capacity and thickness of each layer above an  inner heat source at the defect site.


Experimental


1. Two dimensional defect localization in fully packaged  single chip device


A fully packaged single chip device with a local inner short  acting as a point heat source was used to demonstrate the  potential of the LiT for non-destructive failure localization. LIT measurements were done using supplied voltage of 0.4 V,


a current of 4.17mA and a measuring time over 5000 periods.  The lock-in-frequency was varied starting at 3 Hz up to 12 Hz. As it can be seen from figure 2, a relatively large hot spot at  the surface could be detected using a low excitation frequency (3Hz) due to thermal spreading. This spot size can be reduced  by increasing the lock-in-frequency.


Figure 2: Hot spot detection in a fully packaged device using  a lock-in-frequency of 3Hz. Phase and topography image were  overlaid. .


Increasing the lock-in-frequency to 6 Hz reduces the spot size  at the surface significantly and allows a better localization of  the hot spot (Fig.3). On the other hand, the signal-to-noiseratio is significantly reduced. Further increasing of the lock-infrequency leads to the point that the hot spot can not be  detected on the surface in relevant measuring times.


Figure 3: Hot spot detection in a fully packaged device using  a lock-in-frequency of 6Hz. Phase and topography image was  overlaid.


As a second way, in order to reduce thermal spreading, the  thickness of the mold compound above the failure can be  reduced. This could be done using a local grinding tool, Fig. 4. A second fully packaged single chip device with an inner short  was investigated by LiT. The inner hot spot was excited using  a supply voltage of 0.4 V at 2 Hz frequency leading to a


∆Φ1


∆Φ2


current of 2.61mA. It can be seen from figure 5 that a hot spot  was located outside of the chip. After reducing the thickness of  the mold compound a second LiT measurement was done  using a higher LiT frequency of 16.5 Hz. It can be seen from  figure 6 that this leads to the result that the hot spot size is  strongly reduced compared to the first measurement (Fig.5).


Figure 4: Reducing the thickness of the mold compound by  local mechanical grinding.


Figure 5: Hot spot detection by LiT at a fully packaged  device. Shown is the overlay of amplitude and topography  image.


Figure 6: Second LiT measurement after reducing the mold  thickness above the short defect. Shown is an overlay of  amplitude and topography image.


As a result of the reduced thickness and the resulting increase  of the spatial resolution the hot spot could be located between  two adjacent bond wires. After additional target preparation by


mechanical cross sectioning the root cause of short path could  be found as a metal splinter by light and scanning electron  microscopy investigations , seen in Fig. 7.


Figure 7: root cause after target cross sectioning: metal  splinter between adjacent bond wires


2. Three dimensional defect localization at a fully  packaged stacked die device


2-dimensional non-destructive failure localization at single  chip devices can be used to divide between chip- or  interconnect-defects, which is important for further failure  analysis steps. The 3-dimensional failure localization is  helpful, if separate chips were stacked on top of each other.  In  this case the non-destructive localization of the defect  allocated to the chip- or interconnect level can strongly reduce  failure analysis time.  An easy failure analysis flow at a  defective stacked die device is subsequently shown. The  multi  chip device contained two stacked ICs. The inner short was  excited by a supply voltage of 0.5V and a current of 8.02mA. The LiT was done using a lock-in-frequency of 2Hz. As it can  be seen from Figure 8 a hot spot in the area of the IC stack was  found.


Figure 8: LIT phase image of a fully packaged stacked die  device with inner short. The dotted line shows the position of   the linescan determining the phase shift.


Example # 1: Visualizing shorts within ceramic  capacitors


This is one of the most common defects in wireless  modules, the shorted capacitor. Most solder shorts  within a module are a result of delamination between the  mold compound and the laminate material, providing a  path for the solder to travel. Occasionally a solder short  can occur during reflow on the top or the bottom of the  device, without the aid of delamination.  As short  diameters within ceramics capacitors can be relatively  small ( 1 to 15 um ) and inherently have poor x-ray  absorption contrast, it is difficult to detect this class of  failure using conventional 2D x-ray systems and most  3D systems, due to lack of contrast &/or resolution.


The following figures (Fig 2 to 4) demonstrate the power  of how, with sufficient resolution and high contrast, the  XCT can visualize these types of defects non invasively.  This short was discovered at package level, and the  short was isolated to this capacitor using a combined  method of mechanical back lapping and DC curve  tracing.


Figure 6: SEM and TEM image of sample preparation using (a) common parallel lapping PFA method, and (b) using non-common PFA method as Case study 1.


M5


M4 almost  expose


Bright PVC


observed after  lapping away M5


M4  V5 punch thru short to M4


M5 lapped  away


M3


V3


M2


M4


M5 and V5 Cu etch


away by HNO3


V5 punch through


short to M4


TEM  Micro trench short


to lower M4


M4 under IMD


Firstly, the failed sample was secured on a dummy glass  substrate with epoxy or solidified with resin, and then its  backside Si substrate was thinned to around 100µm. The left  over Si material was removed by Potassium Hydroxide (KOH) to leave BEOL material, in order to have even surface for  further delayering. Figure 7 shows cross sectional view of the  sample. Sample continued to delayer away Nickel Salicide (NiSi) layer using parallel lapping (as gray dot line that  illustrated in Fig. 7). RIE was used to remove IMD and Ta  barrier layer leaving the Cu metal identified by the black dot  line as illustrated in Figure 7. M1 Cu metal was removed by  HNO3 to reach V1 level. M2 and V1 were protected from  reaction with HNO3 by Ta barrier layer. This method used the  thick Ta barrier layer processes to prevent HNO3 to react with  Cu metal, which can be seen from TEM result in Figure 6(b). By continuously using RIE and HNO3, every layer can be  removed and inspected evenly with good control of RIE  timing. Figure 8(a) shows the SEM PVC image after removing  M4. Abnormal bright PVC Via (V) observed. Figure 8(b) shows the TEM image at the punch through V5. It can be  clearly seen that V5 punch through M5 and short to M4. From  this TEM image, void can be seen at the punch thru V5, and  Ta barrier layer for V5 was actually deposited at the sidewall  of the M5. The TEM image explained that M5 actually  corroded and void was formed during V5 trench etch and  clean process as illustrated in Figure 9. Therefore during M6  trench etching, it will etch through corroded Cu or void of M5  and punch through to M4. Ta barrier layer and Cu fill will  cause the Cu filled to the empty areas and cause short between  M5 and M4. Some empty areas that cannot be filled  thoroughly remained as void. The whole short mechanism is  illustrated and explained in Figure 9.


Layer by layer inspection from the backside can be done using  this proposed PFA technique. Furthermore it also offers better  sample surface evenness and better understanding of the  failure mechanism. With this finding, the process yield was  improved and the prototype is transferred to fab for production.


B056


Figure 8: (a) SEM and (b) TEM image of sample preparation  using new proposed chemical etching methods from sample  backside delayering.


Figure 7: Cross sectional view of the layers.


IMD of M4


Bright PVC of punch


thru V5 that short to M4


Left over of M4 Cu  that not thoroughly  etch clean


V6


M6


V5


V5 punch through  short to M4


Metal Void that


from M5 corrosion


M4 etched away


by HNO3


Ta barrier layer that  deposited to empty  corroded M5 sidewall (refer Figure 9)


Si removed by KOH


RIE to expose M1


Followed by HNO3  to remove M1Cu  RIE to expose M2


Followed by HNO3  to remove M2 Cu


IMD


Ta barrier layer


CA


Cu Metal


M7, Cu


V6, Cu


M6, Cu


V5, Cu


M5, Cu


V4, Cu


M4, Cu


V3, Cu M3, Cu V2, Cu M2, Cu V1, Cu M1, Cu


Contact, Poly, Active


NiSi removed by  parallel lapping


NiSi


Si substrate


Direction  of


delayering


Two unusual vertical short examples of 65nm devices were  studied and discussed, and two different non-conventional  PFA methods to identify different types of vertical short issue  were presented. These two non-conventional PFA methods are  more efficient and easier to adopt in the identifying process of  vertical short issue in Cu process. These PFA techniques allow  for a deeper understanding rather than just finding the defects  only.


The authors would like to thank Chartered Semiconductor  Mfg. Ltd., Singapore TEM FA team and Product Engineering  team of Technology Development New Technology  Prototyping Division for their great support.


[1] Len W. B. Len, Y. Y. Liu, JCH. Pang, DSH. Chan, “Near


IR continuous wavelength spectroscopy of photon


emissions from semiconductor devices”, ISTFA 2003


proceedings, pp. 311-316.


[2] V. Liang, H. Sur, S. Bothra, “Passive Voltage Contrast


Technique for Rapid In-line Characterization and Failure


Isolation During Development of Deep-Submiscron ASIC


CMOS Technology”, ISTFA 1998, Proceedings, pp. 221-


225.


[3] R. Rosenkranz, W. Werner, “Comparison of Active and


Passive Voltage Contrast for Failure Localization”, ISTFA


2007, Proceeding, pp. 331-336.


[4] Kendall Scott Wills, Srikanth Perungulam, ISTFA 2007


tutorial  ‘Delayering Techniques : Dry processes, wet


chemical, parallel lapping’.


[5] M. Weldy, L. Serrano, “Increasing Planarity for Failure


Analysis Using Blocked Reactive Ion Etching Combined


with Planar Polish”, Proceeding of the 31st ISTFA


Conference, Nov. 2005, pp. 206-208.


[6] J. Hahn, “Enable Multiple Site Defect Analysis on a


Microchip”, Proceeding of 33rd ISTFA Conference, Nov.


2007, pp. 165-167.


V5 over etched into Nitrate block layer


Cu corrosion after M5 exposed


V5 punch through Cu void


during M6 trench etching


Ta barrier layer deposition


(formed at side wall of void)


M6 Cu filled in and shorted to M4 (some void at sidewall still remained)


Figure 9: Explanation of the M6 punch through shorted to  M4 mechanism.


DOI: 10.1361/cp2008istfa085


Fast Root Cause Analysis Based on Electrical Defect Localization


Michael Schmidt, Larry Dworkin


FEI Company, Hillsboro, Oregon 97124, USA  Michael.Schmidt@fei.com


Christopher Hess, Michele Squcciarini, Shia Yu, Jonathan Burrows


PDF Solutions Inc., San Jose, CA 95110, USA


The ability to rapidly perform root cause analysis (RCA) on  yield limiting defects is critical to a fab’s ramp. Here we  present two methodologies for RCA using specially designed  high density test structure arrays and a FIB/SEM DualBeam. These methodologies have been proven to identify the root  cause of both hard and soft electrical failures. Correlation  between electrical test results and the yield-impacting defects  are presented.


As devices shrink and become more complex, semiconductor  manufacturers are relying more on electrical test results, as  opposed to traditional optical inspection, to identify defects  that affect device performance. These electrical defects may  be ‘soft’ failures or ‘hard’ failures. Hard failures are present if  a structure’s measured resistance is many orders of magnitude  different than its expected value. Soft fails are present if a  structure’s measured resistance is as little as one order of  magnitude different than its expected value. Soft fails present  particular difficulty in being relocated by scanning electron  microscopy (SEM) or focused ion beam (FIB) imaging. This  may be due to the fact that soft fails are often transient and  disappear with multiple image acquisitions.


Here we present two methods for performing RCA on a high  density test structure array. The first method involves imaging  the entire DUT with the SEM operated at high beam energy. If  a hard failure is present this technique will often reveal its  precise location allowing for further FIB processing and RCA. The second technique employs what is traditionally known as  slice-and-view in a FIB/SEM DualBeam. The powerful  combination of specially designed DUTs, electrical test  results, and the two methods of performing RCA allow a fab  to determine the root cause of both hard and soft yield limiting


Test Structure Design


The high density test structures designed by PDF Solutions  incorporate many small DUT cells within a single array [1]. Figure 1 illustrates the layout of placing many small DUT’s in  a single array.


Figure 1


Each DUT is approximately 9 µm x 9 µm in size. In this  design, devices are shared among neighboring DUTs. This  cuts the number of required devices per DUT in half. Combinatorial decoder circuits are implemented to address a  particular DUT within the array.


Root Cause Analysis


Once the failing address has been electrically located the  physical analysis of the device can begin. The electrical fail  data allows for navigation to the row and column of the failing  DUT. A 300 mm full-wafer dual beam is used to perform the  failure analysis. The use of a dual beam FIB/SEM allows easy  automated or manual navigation by use of defect files and  CAD design files.


Once the failing cell has been located within the DUT in the  view of the SEM, several analysis techniques can be  employed. The method of analysis employed depends on the  fail type (Hard, soft, open, short….). High energy SEM back  scatter inspection from top down is employed to try and  isolate a possible point defect within the 9 µm X 9 µm region. This technique is most often successful in locating hard  electrical opens. If a defect is located using this technique a  FIB cross section can be immediately performed at the site of  interest. If nothing is observed further layout and circuit  analysis can be performed to potentially narrow down the  region where the defect might reside. In the worst case


Selection Devices and Routing   Selection Devices and Routing


Selection Devices and Routing


scenario, the dual beam can be used to slice all the way  through the 9 um X 9 um DUT while observing with SEM  between slices to look for anomalies. This technique is  commonly referred to as slice-and-view. This is the power of  using the high density test structure arrays. Normally DUTs  are too large, often on the order of hundreds of microns, to  employ a slice-and-view technique over the entire area. In the  absence of top-down defect localization, an FA engineer often  gives up on the site. With high density array test structures the  failure can often be located in a cross-section even if it is not  detected using top down SEM or FIB imaging.


Hard Fail Defect Detection


In this first example, a hard electrical open was detected after  electrical probing. An image of the DUT using high energy  backscatter electrons is shown in Figure 2. The entire 9 µm x  9 µm area can be seen in a single FOV. A sub-surface defect  is visible using this imaging technique. A red box has been  drawn around the defect.


Figure 2


In this case a quick cross section can be prepared with the FIB  since top-down fault isolation was achieved. The cross  sectional image (Figure 3) shows a missing contact. Although  high-energy backscatter electron imaging has been used in the  past to localize sub-surface defects, it is the use of highdensity test arrays that allows the engineer to localize the  defect in < 5 minutes. Often an FA engineer may spend hours  trying to localize a defect in a large DUT.


Figure 3


Soft Fail Defect Detection


When the defect can not be located top-down using high  energy backscatter electrons, as is often the case for soft  failures, then slice-and-view can be applied to the entire DUT. Slice-and-view involves repeatedly removing small amounts  of material with the FIB followed by a SEM image. Since the  electrical failure has already been localized to a 9 µm x 9 µm  array it is reasonable to perform a Slice-and-view process on  the entire DUT even if a defect is not visible top-down.


Top down high energy backscatter SEM imaging of this  failing location did not reveal any anomalies. Electrically, it  had a measured resistance of 39820Ω compared to a nominal  resistance of 25927Ω. Further analysis of the electrical data  pointed to a possible single contact type defect. This chain  type defect contains 156 contacts, as show in figure 4.


性


Figure 4


Since no observations were made in top down imaging, the  site was set up in the dual beam FIB to slice through all  contacts progressively and acquire SEM images between  slices. The site ran for approximately 3 hours. A missing  contact was observed in the structure as shown in figure 5.


Figure 5


This image clearly shows the defective contact. The region  where the W contact would normally be has been filled in  with Aluminum. It is nice also to make sure that the after the  defect has been located and characterized physically that it  matches up with the electrical failure signature. Since this is a  single point defect, it fits very well with the electrical test data  showing a soft open signature.


Another defect not observed via top down back scatter  followed. A slice-and-view was also performed on this DUT  as well. The contact resistance was 21720Ω as compared to a  nominal resistance of 25129Ω indicating a short was present. The defect was located, as shown in Figure 6, but would have  been nicer to see 90 degrees to how it was actually cut. It was  cut this way suspecting a short from the structure to the


periphery. What was observed here is an internal short to the  structure that excluded several vias during electrical  measurements.


Figure 6


Does this defect make sense?  Absolutely if you look at where  the short occurs and cut out the contacts. 108 total contacts, nominal value is 25129 ohms; this equals 195.6 ohms/contact. 14 contacts are eliminated by the short equaling a resistor of  about 2739 ohms pretty close!


Utilizing high density test structure arrays and a full wafer  FIB/SEM DualBeam enabled the detection and localization of  hard and soft electrical failures. Utilizing a two-pronged  solution for uncovering the root cause of the electrical failure  is a successful technique. The failing DUT is first imaged  using high energy backscatter electrons to see if the failure  can be localized even further within the DUT. If one is  detected then it can be immediately cross-sectioned. If one is  not detected then an automated slice-and-view can be  performed on the entire 9 µm x 9 µm DUT.


[1] Christopher Hess, et. al “High Density Test Structure  Array for Accurate Detection and Localization of Soft  Fails,” 2008 IEEE International Conference on  Microelectronic Test Structures


DOI: 10.1361/cp2008istfa088


Failure Analysis for Gate Oxide Breakdown


Xianfeng Chen, Ming Li, Qiang Guo, Kary Chien, YanBo Gao


Damage-free gate oxide is one of the important  factors to ensure device performance and  reliability. Compared with the Logic and  DRAM, SOC (system on chip) wafer needs  more careful process control to improve yield. In SOC wafer process, HV (high voltage) and  LV (low voltage) devices are integrated into  one system. More process steps are involved in  oxide formation. There are more than two  cycles oxide of deposition, oxide photo, oxide  strip and cleaning. The added steps introduce  more process risk. So, special WAT (wafer  accept test) test structures such as large size (i.e. 70um by 700um) MOS capacitor must be  laid on test line to monitor the oxide process  issue and process window. However, it brings  about many challenges to failure analysis  engineer. Firstly, burnout during the test  destroys evidence and thus prevents engineers  from analyzing the cause of original failure. Secondly, in the EFA procedure, it is difficult  to detect failure site by EMMI and OBIRCH  without capacitor burnout. It makes the root  cause difficult to identify. Finally, in the PFA  procedure, artifact such as silicon substrate pit  could be introduced during capacitor access. In  general, to access the oxide layer, polysilicon  is removed by HF based etchant, which could  attack silicon substrate if there would be a  pinhole in the oxide layer. It also couldn’t be  accessed by mechanical parallel lap down due  to the poor uniformity on sample surface  polished.


To overcome the EFA and PFA limitations, fresh samples were taken from the passed


wafer and the failed ones to identify the root  cause of VBD failure. In addition, new lapping  down method was used to access the capacitor  structure. Two VBD failure cases were studied  here.


1) Test structure


Test structure shown in Fig.1 is a capacitor  stacked with n-type silicon substrate, oxide  and poly capped with Ti-silicide.


Fig.1 Schematic of capacitor cross-section  view stacked with n-type silicon substrate, oxide and poly capped with Ti-silicide.


2) Fault Isolation and PFA


The I-V curve shown in Fig.2 of the failed  sample (Sample1) is linear. So, OBIRCH was  applied to detect hotspots as shown in Fig.3. After parallel lapping down to ILD (inter layer  dielectric), RIE (reactive ion etcher) was used  to remove the remaining dielectric and silicide. Dielectric was removed by Ar & CHF3 based  plasma and silicide was removed by Ar plasma  sputtering. Poly layer was observed by  scanning electron microscopy. No abnormality  was found. Per this analysis result, it is  concluded that the damaged sites could be in  the oxide or silicon substrate.


FIB milling was applied to find defect area.


Ti-silicide  HV oxide  LOCOS


Si-sub  Poly


Before FIB milling, Laser Marker marks the  failure site according to OBIRCH image. By  BD (Dual beam) FIB system, E-beam images  were taken step by step during I-beam milling. Milling stopped when capacitor damage was  observed by E-beam image. And then, TEM  sample was prepared at the defect area by FIB. Unfortunately, burnout was observed at the  failure site shown in Fig.4. And dislocation can  be observed in silicon substrate at the failure  site. The burnout could have happened during  WAT test or EFA and the dislocation could  result from the thermal stress when burnout  happens. To exclude the influence of WAT test  and EFA on the PFA result, two fresh samples  were taken from the VBD passed and failed  wafer respectively.


Fig.2 I-V curve of the sample 1 when voltage  was applied on the poly and silicon substrate  is grounded.


Chemical etching was used for dielectric layer  removing. Firstly, two samples were dipped in  49%HF. To accelerate the removing rate of  dielectric layer, the solution needs to be stirred  by a plastic stick until the poly layer was  exposed. Then, samples had been dipped in  10:1 BOE (Buffered Oxide Etch) for 12hours  to erode the oxide layer. Next, ultrasonic  vibrating was executed in fresh BOE for 20  seconds and in DI water for 10 seconds step by  step. During BOE dipped ultrasonic vibrating, sample was upside-down to remove poly  residue. Finally, samples were decorated by


dilute Wright Etcher (2mins). Plane view of  silicon substrate by SEM showed a  high-density of dislocations and significant  micro roughness on the silicon substrate  surface of the test structure as shown in Fig.5. But, there is no obvious dislocation observed  on the substrate surface of the passed sample  as shown on Fig.6.


Fig.3 Sample1 failure site detected by  OBIRCH.


Fig.4 Sample1 X-TEM view of the failure site, Burnout and dislocation can be observed.


Process engineers were interested in finding  the root cause of high-density dislocations and  micro roughness of the silicon substrate. In-line tool check and defect map analysis  showed that the passed wafer and the failed  wafer were run in different cleaning machines  after HV oxide strip. From this clue, it was


Poly


Oxide


Dislocation


suspected that the HF based cleaning solution  would induce under-cutting at the corner of  oxide film and damage the silicon substrate  surface when its concentration were out of  control. Fault isolation results provided more  evidence for that because all failure sites of the  failed samples were detected at the edge of test  structure shown on Fig.7 (a) & (b).


Fig.5 SE image of Silicon substrate surface of  the VBD failed sample. High-density  dislocation and micro roughness observed.


Fig.6 SE image of Silicon substrate surface of  the VBD passed sample.


Capacitor VBD failure analysis of the other  products also confirmed that poor cleaning  process damaged the silicon substrate and  induced VBD failures. As a matter of fact, no  VBD failure issue occurred after cleaning  recipe renewal.


The test structure is different from the previous  one. The capacitor is stacked with n-type  silicon substrate, oxide and poly1/poly2.


Fig. 7 (a) Sample2 failure site detected by  OBIRCH.


Fig.7 (b) Sample3 failure site detected by  OBIRCH.


2) Fault isolation and PFA


Fig.8 I-V curve of the failure sample.


From Fig.8, I-V curve of the failure sample, EMMI was chosen for fault isolation as shown  in Fig.9. Pits at the failure site can be observed


LOCOS area


Si-Sub


after poly layer removal. Pit top view is shown  in Fig.10 and X-TEM view is shown in Fig.11. EDX examination revealed higher oxygen  signal at the bottom of the pit shown in Fig.12. It is concluded that pits were formed before  oxide deposition. Just like the previous case, the failed sample was also taken from the  wafer, which ran in the same cleaning machine  before oxide deposition. The poor wet process  could damage the silicon substrate during  pre-oxide deposition cleaning when chemical  solution concentration is out of control.


Fig.9 Failure site detected by EMMI.


Fig.10 Plane view of oxide layer. The oxide  and silicon substrate were damaged.


Fig.11 X-TEM of the pit defect. Bright contrast  can be observed at the bottom of pit.


Fig.12 EDX result of the failure site, higher  density O signal was detected at the pit bottom.


Poor wet clean process was defined as the  cause of the silicon substrate surface damage  and crystalline defect. It induced poor oxide  deposition, which reduced breakdown voltage.  In addition, we demonstrated that 12hrs BOE  dip is an effective method for removing poly  and oxide layers from large MOS capacitors.


1. Frank S & Anton S., Dislocation Related  Leakage in Advanced CMOS Device, 31st  ISTFA, 2005 Nov.


2. J.C. Lin, Y.T. Hsu & C.K. Huang etc, Investigation of Substrate Dislocation induced  Bit Line Soft Failure, 30th ISTFA, 2004 Nov.


3. H. Uchida, S. Ikeda & N. Hirashida, An  Accurate Discrimination Method for Gate  Oxide Breakdown Positions by a New Test  Structure of MOS Capacitors, Proc, IEEE 2001, Int. Conference on Microelectronic Test  Structure, Vol 14, March 2001, P299.


4. Dat Nguyen & Frank Huang, Stacked  Polysilicon/Metal Capacitors Failure Analysis, 31st ISTFA, 2005 Nov.


pit


pt


oxide


DOI: 10.1361/cp2008istfa092


Non invasive Failure Analysis of Passive Electronic Devices in  Wireless Modules using X-ray Micro tomography (MicroCT)


Tyler Pendleton,


RFMD, 7907 Piedmont Triad Parkway, Greensboro, NC 27409


Luke Hunter, S H Lau


Xradia Inc, 5052 Commercial Circle, Concord, CA 94520


The electronics industry is continually evolving. Electronic devices are becoming smaller and the  technology is becoming increasingly complex.  With the  increased intricacy in device and package design the  difficulty in the failure analysis field increases as well.  Two of the major problems commonly encountered by  failure analyst engineers in wireless modules are issues  with solder reflow and open solder connections, many of  which are difficult to detect by conventional techniques, such as 2D X-ray imaging or even physical cross  section.  Along with the difficulty in finding some of these  failures, there are also problems that may arise in  exposing these failures using destructive analysis  techniques such as physical cross sectioning and  chemical decapsulation.  Both of these techniques may  induce damage, not relevant to the defect site, or  remove the evidence of a defect or damage site.  High  resolution 3D X-ray micro computed tomography (XCT) provides a powerful non invasive alternative solution for  these problems facing failure analysis engineers.


X-ray computed tomography (CT) or 3D X-ray imaging  has been used extensively in the medical community, where resolution in the range of mm to sub mm is  sufficient for imaging of human anatomy. With the  advent of microCTs, accompanied by better resolution in  the range of several microns to tens of microns, many  new applications in biomedical[1], industrial[2] and  microelectronics[3] were reported. However conventional  microCTs or 3D x-ray upgrades from existing 2D x-ray  systems have two major drawbacks when they are used  for failure analysis of advanced packages: Insufficient  resolution to image small (1 to 5 microns), and the lack  of imaging contrast to visualize cracks, whiskers, and  defects within low Z materials.


In this paper we are going to discuss some of the failure  analysis case studies of wireless modules using a novel  high resolution micro x-ray computed tomography (XCT).


Method


At RF Micro Devices, we recently acquired a novel  high resolution XCT, which seem to overcome some of  the drawbacks of conventional 3D x-ray systems. This  tool is currently being extensively used in our failure  analysis lab to help solve a number of difficult to detect  failures, complementing and gradually replacing some of  our traditional, destructive, methods. The results in this  study are based on the CT images obtained from the  MicroXCT from Xradia Inc (Concord, CA)[4 & 5] The  MicroXCT is capable of 1-2 micron resolution, even for  relatively large RF packages containing compound  semiconductor material such as gallium arsenide (GaAs) or gallium nitride (GaN). Using XCT, along with other  non destructive techniques, such as DC package level  curve tracing, RF probing and scanning acoustic  microscopy (SAM), it is possible to eliminate the routine  use of manual cross sectioning and/or decapsulation.  Such physical methods take hours of preparation and  render the device useless post analysis. The XCT has  proven to be invaluable in resolving various solder and  metal defects, by reducing the time to a FA solution and  maintaining the integrity of the original package.  In  addition, all data that is collected during XCT is saved  and can be retrieved at any time for review, or to  observe other areas of interest related to the device  under inspection, reducing the need for rework of a  sample.  Moreover, the tomography allows the region of  interest to be visualized in 3D or virtual cross sections to  be made at different planes without destroying the  sample.  The 3D visualization can be used specifically to  target customers who may not fully understand the  makeup of the inspected device


The most common failures in wireless modules typically  occur in the package, not at die level (microcircuits such  as the power amplifiers, silicon controllers and switching  circuits).  Most failure analysis engineers and  technicians have experienced projects with failures that


appear to be at die level based upon test data, or initial  non destructive analysis, such as DC package level  curve tracing where an abnormal electrical shorting is  observed. It is easy to overlook the passive devices  within the module and concentrate on possible damage  to the die, and thereby come up with no results because  the defect site was elsewhere within the module.  Since  these devices are exposed to corrosives, any defect in  the package could be destroyed, resulting in an  unresolved analytical case loads.  On the flip side of this  scenario, if there is a package level defect suspected, such as a solder short beneath a capacitor, a physical  cross section must be performed.  This process destroys  the package and no further analysis can be performed at  die level if need be.


The following examples show the value of high  resolution x-ray computed tomography as a new  approach to some common package level defects, including some interesting case examples, where we  have been able to uncover some failure mechanism we  could not have done otherwise, using conventional  means.


1.5 mm


3 mm


(1) Left end of  metal splinter


(2) Splinter, diving  down to the right


(3) Splinter, diving


up from the left


(4) Splinter, again diving


down to the right


grinded


After the first LIT measurement, the mold compound above  the upper chip was removed by local mechanical grinding and  chemical etching.  Then a second LiT-measurement was done. As it can be seen from Figure 9, the hot spot size is strongly  reduced. Due to the point that both stacked chips contain  electrical active structures in the area of the hot spot the short  could be located at the upper or lower chip.


Figure 9: LiTimage after removing the mold compound.


As a subsequent step, the upper chip level was de-contacted by  removing the bond wires. The following electrical and LiTmeasurements lead to same results. In conclusion the short  defect is situated on the lower chip level. Because of the IRtransparency of the chip material (mainly Si) the thermal  defect on the lower chip could be imaged through the upper  chip.


This procedure can be extended to multi chip stacks with  separately operating chips. More complicated is the case if the   chip functionality depends from each over or the defect occurs  at the interconnect level. Therefore, an all-encompassing  method to allocate the defect vertically is necessary. This  could be done in a non- destructive way using LiT and its  opportunity of measuring the phase shift generated by timedepending heat flow.


In order to demonstrate this, a linescan through the detected  hot shots in the phase image of the fully packaged device was  taken, which can be seen in figure 8. Figure 10 shows the  resulting graph of the linescan where two phase signals can be  regarded. The left one, marked black, comes from the contact  needles of the supply voltage and the other one, marked red, is  the phase shift occurring by the defect.


Figure 10: Graph of the linescan. The phase shift on the left  side (marked black) occurs from the electrical contact, the  phase shift marked red comes from the defect.


It has to be noticed that the phase has an amount of 360° at the  device surface and therefore the resulting phase is calculated  by:


°


Φ


∆Φ


360


measured


which leads to a phase shift of 30° for the contact needles and  140° for the defect. The difference between both is 110°. This  phase shift could be used to recalculate the defect site inside  the stacked die. To allow this, the relation between the  resulting phase shift and the penetrated layer thickness for  each layer material has to be known.


3. Phase shift between different stacked die layers


First experiments using mold compound dummies were done  determining the relationship between the penetrated mold  thickness and the resulting phase shifts [7].


Figure 11: Experiment and simulation results taken from [7] in order to determine the defect depth related to the measured  phase signal.


For further experiments a test sample with defined ohmic  resistance and geometry was used. It consists of a stacked die  built up with two identical meander-shaped test structures at  each chip layer, shown in figure 12 in a sideview. The lower  test structure is placed outside of the upper chip. In both cases  heat flow is transferred only through the mold compound to  the device surface.


Figure 12: Side view of the device under test. The expected  phase shift difference comes from the different depths of the  defects (red points).


460µm


655µm


The meander-shaped structures have the same electrical  behavior (R ~ 93 Ohm) and were excited using a supply  voltage of 0.18V. The current flow of 1.89mA leads to a  power dissipation of 0.34mW. In order to allocate the LiT  measurements the test sample was imaged by a X-ray  inspection tool.. Figure 13 shows the resulting X-ray image  and the position of the different chip layers from top side.


Figure 13: Top view of the test sample. The blue rectangle  marks the dimension of the upper chip, the red one the chip  below.


The heat generations of both test structures were measured  using a lock in--frequency of 2Hz. To obtain a minimum  required signal-to-noise-ratio the amount of measurement  periods was increased up to 36,000.


Figure 14: Overlay of X-ray and LiT-phase image of the  upper test structure measured with a lock-in-frequency of 2Hz.


Linescans over both hot spots were taken to determine the  phase signal. Own to the low signal- to-noise ratio both  linescans were smoothed by a moving average-function  allowing a determination of the required phase shift.


Figure 15: Linescan over hot spot occuring at the upper chip  level including  smoothing function.


Figure 16: Overlay of X-ray and LiT-phase image of the lower  test structure measured with a lock-in-frequency of 2Hz.


Figure 17: Linescan over hot spot occuring at the lower chip  level including  smoothing function.


For the upper chip level (Figure 15) a maximum phase of 273° was determined which is equivalent to a phase shift of 87°.  For the defect on the lower chip level (Figure 17) the phase  was measured with 239° which results in a phase shift of 121°. The phase shift difference caused by the known distance of  197µm between both chip levels amounts to 34°.


LiT can be used for non-destructive defect localization in fully  packaged devices. It was shown that inner hot spots occuring  by ohmic shorts can be visualized and allocated at the device  surface. In order to get an adequate signal to noise ratio at the  device surface the lock in frequency has to be reduced to  several Hz. Due to the low frequencies and the necessary heat  flow through the mold compound thermal spreading leads to a  reduction of lateral resolution of this method. For sinlge chip  devices or defects in the upper interconnect level of a multi  chip device this can be improved by reducing the mold  thickness above the defect by local grinding. For single chip  devices with inner short paths LiT can be used to differentiate  between chip- or interconnect-failures. Vertical localization of  the short defect is helpful, if the mold thickness should be  remained. For more complex multi chip devices vertically  allocation of the defect in a non-destructive way can reduce the  failure analysis flow significantly. and is one of only several  methods allow defect localization without annihilating the  overall functionality. For stacked die devices with separately  connected chips an analysis flow was found to allocate the  defect chip level.  An all-encompassing method to allocate the  defect vertically can by measuring the phase shift of the  thermal signal. It could be shown that the LiT is in principle  able to allocate the defective chip level by measuring the phase  shift. Additionally, the relationship between phase shift and  mold thickness above the hot spot was determined in a  previous work [7] and can be used to recalculate the defect  depth.


Outlook


The heat transfer through multi layer systems has to be  investigated to allow vertical defect allocation in complex  multi chip devices. Each material layer like mold compound or  die attach contributes a discrete value of phase shift which can  be used recalculating the failure depth. Furthermore, the  sensitivity of the LiT and analysis routines has to be improved  to allow phase shift detection with a higher accuracy. Nevertheless, thermal simulations can be used as a comparison  to experimental results and to predict the heat transfer through  device.


The authors are particularly grateful to Dr. Otwin Breitenstein  for providing his LiT set up and for a lot of fruitful  discussions. The authors also like to thank Dr. Schoemann and  his colleagues from Infineon Munich for making test samples  and Stephan Martens from Infineon Regensburg for his special  support.


The work is supported by the European project “PIDEA Full  control”.


[1] Reverdy,A.,et.al:“3-D Defect Localization by  Measurement and Modeling of the Dynamics of Heat  Transport in Deep Sub-Micron Devices, Proc 33rd  Int’l  Symp for Testing and Failure Analysis, San Jose, CA, November 2007


[2] Khandekar, S., et.al, Liquid Crystal Microscopye, Microelectronic Failure Analysis Desk Reference, Fourth  Ed., (EDFAS 2002), pp.739-44


[3] Hechtl, M. et. al. „Localization of Electrical Shorts in  Dies and Mold compounds using Magnetic Microscopy  and Lock-in-IR-Thermography”


[4] Breitenstein, O. et al., “Developments in IR Lock-in  Thermography”, Proc. 30th Int. Symp. for Testing and  Failure Analysis,  ASM Intern. Mat. Park, Ohio  November 2004, pp. 595-599


[5] Breitenstein, et al., "Lock-in IR Microscopy with 1.4 µm  Resolution by Using a Solid Immersion Lens", Electronic  Device Failure Analysis magazine 8, 2006, pp.4-13


[6] Breitenstein, O. et al., Microscopic lock in thermography  investigation of leakage sites in integrated circuits, Rev. of  Scientific Instruments, 71 (2000), 4155-4160


[7] Schmidt, et al., “ Application of Lock-in-Thermography  for 3d defect localization in defect devices” Proc 2nd  Electronics System-Integration Technology Conference, London, UK, September 2008, submitted


DOI: 10.1361/cp2008istfa108


An Analytical Technique to Assess the Risk of Laser Damage to Encapsulated  Integrated Circuits During Package Laser Marking


Joseph Patterson


Applied MicroCircuits Corporation


San Diego, California, USA


jpatters @amcc.com,  Phone: 858 535 3290


Cliff Schuring


Quantum Focus Instruments


Vista, California, USA


cliff@quantumfocus.com,  Phone:760 599 1122


Damage to encapsulated integrated circuits has recently been  reported due to Laser marking of the package. A method to  assess the risk of such damage is presented. The method is an  analytical technique using Thermally Induced Voltage  Alteration (XIVA) and Optical Beam Induced Current (OBIC) imaging.


Laser ablation of the epoxy mold compound for encapsulation  integrated circuits is one of the predominate methods to mark  devices with their identifying labels.  Damage to Integrated  Circuits encapsulated in Epoxy mold compound induced  during Laser package marking was reported at ISTFA in


2007.[1].  It was shown that the spherical glass filler particles  in the epoxy can line up vertically providing an optical path  for the laser energy to reach the die surface.  The risk of this  occurrence has increased as packages have become thinner, and will continue to increase as packages shrink further.


A means to study the susceptibility of any given specific  package to this mechanism has been developed and is  presented herein.  The damage reported in the Intel paper was  due to melted metal lines that resulted in shorts.  However, other types of degradation to integrated circuit structures have  been observed due to laser energy [2].   Low K dielectric can  delaminate and dopant diffusions can even be altered.  Thus  the issue of an initial yield loss due to shorts is not the only  concern.  The reliability of circuits exposed to laser energy  that can cause degradation other than shorts has to be  considered.  To do that, the likelihood and severity of the laser  event has to be assessed quantitatively.  Alternatively, the  package structure and the conditions during Laser marking  must be shown to be such that the likelihood of damage is  virtually zero.  OBIC and XIVA analysis can be performed at  laser energy well below the threshold of damage or  degradation yet still have the sensitivity to detect package  integrity.  An alternate approach could be to reformulate the


packaging materials so that the marking laser can not reach  the die surface, such as removing the glass spheres.  However, any change to the existing packaging methodology would  have a significant impact on the technology.  New material  and process development as well as requalification of any  changes represent a major effort.


Details of the Damage Mechanism


The conditions during Laser marking resulting in the laser  energy reaching the die surface are depicted in Figure 1. The  significant feature is the alignment of a few large glass  spheres vertically from the outside of the package to the die  surface.


Figure 1: Diagram of a cross section through a plastic  encapsulated integrated circuit showing the optical path of the  marking laser to the die surface.


The set up used during XIVA or OBIC characterization of the  optical paths through the epoxy mold compound to the die  surface is depicted in Figure 2.


Figure 2: Diagram of the set up used to detect the optical  paths through the epoxy mold compound to the die. It is the  same as the laser marking configuration except that the  detection amplifier is connected to the device leads and a  much low power laser is utilized.


A XIVA image of the top of the package of an encapsulated  integrated circuit is shown in Figure 3.  The device VCC and  ground pins were connected to the XIVA amplifier inputs. The red and green sites indicate the location of the optical  paths where the laser beam propagated through the glass  spheres in the mold compound and reached the die circuitry.  The top of the package was polished to remove a thickness  equal to the depth of ablation of the normal marking laser.  The laser wavelength for the XIVA image was 1340  nanometers.  Thus the red and green sites indicate locations  where the circuitry would change resistance due to heating of  the laser energy.


Imaging similar to that in figure 3 was performed on the same  device using a laser wavelength of 1064 nanometers.  The  OBIC technique was performed with the VCC and ground  pins of the device connected to the OBIC amplifier inputs.  The laser was scanned across the outside of the package over  the area of the encapsulated die.  The current detector and  amplifier were the same as what was used as for the XIVA  image.  The OBIC image is shown in figure 4.  The red and  green spots indicate locations where the laser reached sites on  the die that would generate electron-hole pairs in the silicon  near junctions.  Again, the laser revealed optical paths through  the glass spheres in the mold compound.


The locations of the XIVA sites on a given device are  different than the locations of the OBIC sites on the same  device because the integrated circuit elements have different  sensitivities to the two different stimuli.  The XIVA laser can  heat sites where it strikes metal.  However, that same site will  block the OBIC laser from reaching the silicon and it therefore  cannot generate electron–hole pairs.  Figure 5 shows a XIVA  image of the same device as in figures 3 and 4 after the mold  compound was completely removed above the die.  It  indicates all the possible XIVA response locations.


Figure 3: XIVA image of the circuit response (red and green  regions) to the laser energy that reached the die surface  through optical paths in the epoxy mold compound as the  laser is scanned across the outside of the package above the  die.  The white spots are the glass sphere and the dark areas  are the epoxy in the overlain reflected light image. (5X  objective lens).


Figure 4: OBIC image of the circuit response (green regions) to the laser energy that reached the die surface through  optical paths in the epoxy mold compound as the laser is  scanned across the outside of the package above the die.  The  white spots are the glass spheres and the dark areas are the  epoxy in the overlain reflected light image. (5X objective  lens).


Figure 5: XIVA image of the same sample as in figures 3 and  4 after all of the mold compound above the die was removed. This indicates all possible XIVA sites.  (5X objective lens.)


It was initially assumed that the locations of the optical paths  through the mold compound would be randomly distributed. And that the probability of the vertical alignment of several  large glass spheres would be determined by random statistics.  The distribution of particle sizes was examined over the area  of the die in the X-Y plane and at several vertical planes  above the die surface.  This revealed a non random  distribution.  Then a sample of the total thickness of mold  compound covering the die was prepared by removing the die  by parallel polishing from the backside of the package.  This  layer of isolated mold compound was examined for optical  transmission by observing it in a microscope in the back  lighted mode. This produced an image showing total light  transmission and distribution over the area of the die.  This  revealed greater optical transmission near the wires where  larger glass spheres collected.  Refer to figure 6.


Studies of size distribution of the glass spheres revealed that  the physical structures in the I.C. package act as filters to the  various sizes and large glass spheres can selectively collect at  specific locations.  For example, the loops in the wires that  extend above the die surface will allow particles smaller than  the wire pitch to pass between them, whereas the larger  particles are impeded from passing between them.  Therefore, large particles tend to collect near one side of the wires  depending on the direction of the flow of the mold compound  during injection into the mold.  This results in a much higher  probability of vertically aligned large glass spheres in these  locations.  Vertical alignment would not be expected at certain  locations if they were randomly distributed.


Figure 6: Light transmission image of the layer of mold  compound over the die observed in a microscope in the back  lighted mode.  The bottom of the package and die were  removed by parallel polishing.  The bright band at the bottom  is a region where larger glass spheres collected due to the  filtering action of the closely spaced bond wires. (10 X  magnification.)


This examination method can be an alternate to the OBIC and  XIVA methods, but it requires more sample preparation time  and is destructive.  However, because it does not require a  laser scanning microscope it can be useful for a laboratory that  is equipped with standard metallurgical equipment.


The conditions can sometimes exist where a thin layer of  epoxy is present between the glass spheres that will obscure  the OBIC laser.  Even the XIVA laser power may be  inadequate to ablate this layer, yet the marking laser may  ablate it and allow an optical path to the die.  This can result  in a false negative result for the OBIC/XIVA examination. However, since this is a statistically random phenomenon the  false negative events can be mitigated with an adequate  sample size.


For many products the last step in the manufacturing process  is laser marking of the package.  This means that final test is  usually conducted before laser marking, so there is no monitor  for laser marking damage.  Also, new integrated circuit  processes can be more sensitive to the laser marking energy.  Another case not addressed in this paper is the scenario where  the laser marking is performed directly on the back of the  silicon die.


It was mentioned earlier in this paper that package was  prepared for laser injection by polishing the top of the  package down to the depth of the normal laser marking  ablation.  This polishing produces a flat surface on many of  the glass spheres which does not represent the conditions  produced during laser marking where the glass particles  remain spherical.  So the polished samples afford a more  favorable optical coupling interface than a full thickness


package and thus can be considered to be a more conservative  model.  The laser acceptance angle of the spherical surface  with respect to a path that will reach the die surface is much  less.


The observations in the previous paragraph may provide  insight into a solution to reducing the likelihood of damage to  the die during marking.  That is, tilting the marking laser off  the normal axis should greatly reduce the amount of laser  energy reaching the die because the coupling between the top  most glass sphere and an underlying sphere would be greatly  reduced.


It has been shown that the techniques of XIVA and OBIC can  effectively detect the existence and location of optical paths  through the mold compound above the die surface for plastic  encapsulated packages.  These techniques are not 100% effective because not all locations on a given die produce a  response to those stimuli.  But if a reasonable sample size is  used and these techniques show no evidence of light  transmission to the die the confidence level can be considered  very high.


[1] Paranal, Paul Eric B., “Localized Die Metallization  Damage Induced during Laser-Marking of Semiconductor  Packages”, Proceedings of the International Symposium  for Testing and Failure Analysis, Nov. 4-8, 2007, p 226.


DOI: 10.1361/cp2008istfa112


Techniques for Identification of Silver Migration in Plastic Encapsulated  Devices Assembled with Molding Compound Containing


Red Phosphorus Flame Retardant Material


Ronald R. Hylton


Maxim Integrated Products, Hillsboro, Oregon, USA


This paper describes the electrical signatures and failure  analysis techniques used to identify plastic encapsulated  devices that have failed due to silver migration.  This  migration, which produces resistive leakages between adjacent  pins, has been associated with molding compounds that utilize  red phosphorous as a flame retardant material.  A description  of the failure mechanism is also presented.


System failure resulting from silver migration across an  insulating surface is not a new phenomenon, having been  observed in electromechanical telephone systems in the mid  1950’s [1].  The recent introduction of environmentally  friendly “green” molding compounds that have replaced  bromine and antimony oxide based flame retardant systems  have created a new failure mechanism in today’s plastic  encapsulated devices.  Specifically, those molding compounds  that use phosphorous based flame retardant materials have  been associated with silver migration.


This paper will describe the mechanism whereby silver  migration occurs and will describe in detail the techniques  used to isolate and accurately identify this failure mechanism.


Failure Mechanism Description


Phosphorous performs the flame retardant function by forming  a carbon layer or “char” on the plastic surface at the burning  zone that interferes with the transport of oxygen to the burning  zone.  This system requires a uniform distribution of flame  retardant particles in the molding compound to promote even  char layer formation during the burning process [2].


The phosphorous particles are coated with aluminum  hydroxide, Al(OH)3, to prevent a chemical reaction from  occurring under normal conditions.  If this coating is  defective, or if the coating is damaged when the device is  assembled onto the customer’s board, phosphorous can be  exposed.  Oxidation of the exposed phosphorous occurs, forming phosphorus pentoxide, P2O5.  This in turn reacts with  moisture in the package to form phosphoric acid, H3PO4.


Phosphorus pentoxide is hygroscopic, further compounding  the problem.  The phosphoric acid corrosively attacks the  silver plating or copper core of the lead frame.  With the  presence of an electric field and the phosphoric acid  electrolyte, the silver or copper migrates through an anodic  oxidation/cathodic reduction process.  Maxim has observed  this problem on devices with higher power dissipations, a  condition that might accelerate the oxidation of the  phosphorous.  Time to failure is dependent upon the  application and environment.  In practice, failures have been  observed after 3 months to 2 years of service.  Failure rates are  also dependent upon these same factors, and rates of  approximately 1% have been reported [3].


Maxim has observed silver migration failures both at the lead  frame fingers in the package body and between bond pads on  the die surface.  The phenomenon of migration at the die  surface is not completely understood, as no silver is present on  the die.  One theory is that the phosphoric acid electrolyte  wicks along slight delaminations in the package to the affected  bond pads.  Silver plating is used on the interior surface of  exposed paddle packages, providing a nearby source of silver  for this type of failure.  Maxim and other manufacturers have  associated this failure mechanism with the Sumitomo  EMExxxxU Series phosphorus based molding compound.  The total quantity of this material sold until shipment was  stopped in July 2002 is estimated at 1000 tons.  Assuming 1  gram of molding compound per device, nearly one billion  units could have been produced using this molding compound


[4].


Additional information about this failure mechanism that is  beyond the scope of this paper is available from the works of  Pecht and Deng of the CALCE Electronic Products and  Systems Center [5,6].


Analysis Techniques


The techniques that have proven to be effective in accurately  identifying the presence and location of silver migration will  now be described, beginning with electrical characterization  and followed by physical analysis methods.  All of the  techniques described in the following examples were  performed on TQFP-EP style packages, but the techniques can  easily be extended to other package styles.


Electrical Characterization


Silver migration can produce resistive paths between adjacent  pins that can range in resistance from a few ohms to 10’s of  kilo-ohms.  One method that works well to identify the  affected pins is to measure the DC voltage present on each pin  while power is applied to the failed device in the application.  The measured values can be compared to those from a good  device, looking for pins that are pulled higher or lower than  normal.  Next, verify that the observed DC voltage differences  correlate with the device malfunction.  A typical example of  two pins that might be resistive to one another would be an  input or output pin with a higher DC voltage than expected  that is immediately adjacent to a VCC pin.  Once a pair of  suspect pins has been identified, a curve tracer should be used  to examine the characteristics between the two pins.  Low  measurement currents in the microamp range should be used  to reduce the risk of fusing open the potentially fragile silver  migration path.  Instability in the leakage will often be  observed, with the measured resistance quickly fluctuating, even intermittently appearing as an open circuit.  If there is  other circuitry on the circuit board that makes this curve tracer  measurement difficult, one may consider mechanically  removing the connection to one or both of the pins.  Desoldering the failed unit from the device should be avoided  prior to analysis, as the heat and resulting thermal expansion  of the package from this operation can break the tenuous silver  migration path.  Days or even weeks of continuous bias might  be required to restore the leakage.  For this reason, Maxim  recommends that devices suspected of failure due to silver  migration should be returned for analysis while still mounted  on the circuit board [7].
The localized positioning capability of the Open Platform  system permits the placing of nanoindentations with submicron positioning accuracy. This is demonstrated in Fig. 6  which shows a line of 4 nanoindentations made along a  bonding pad connector of only 10 µm width which has been


coated with a diamond-like carbon (DLC) coating of thickness  2 µm. An example of a typical load-depth curve is shown in  Fig. 6(c), from which a hardness of 11.058 GPa and elastic  modulus of 135 GPa have been calculated for the coating. The  indentation depth was kept to approximately 10% of the  coating thickness (~ 200 nm) in order not to have any  influence from the underlying substrate on the mechanical  property values.


Some other examples of nanoindentations on small device  features are shown in Fig. 7, one on a circular bonding pad  and one on a gold connector strip. The residual impression, when viewed under an optical microscope can also give an  idea of the ductility of the material. For example, in Fig. 7(a) the residual indent has significant plastically deformed  material around it, and the edges of the imprint are “barreled” suggesting that the material is soft and ductile. In contrast, the  indent in Fig. 7(b) does not show such deformation because  the material (in this case gold) is more brittle as a result of the  deposition process.


Figure 7: Nanoindentations made in circular bonding pad (a) and along a gold connector (b) confirming the sub-micron  positioning capability of the system.


2. Solder Bumps


During IC fabrication solder bumps are subject to deformation  which can be modeled with a flat punch indenter. The surface  of individual solder bumps is prone to oxidation and  contamination, and if this hampers connectivity there may be  significant impacts on overall yield. Excessive damage to  solder bumps during fabrication of devices can lead to  planarity issues requiring additional process steps.


The switch from leaded solder to unleaded solder caused a lot  of contamination issues and led to development of a technique  for measuring the applied load at which a flat punch indenter (simulating the packaged device) makes electrical connectivity  with the solder bump. Fig. 8 shows a schematic of the solder  bump indentation test process, together with an optical  micrograph of a typical solder bump after testing up to 500  mN applied load. Results show that the load to achieve  continuity may exceed the load used for bonding. Such point  testing of solder bumps can be performed on any bump of  interest, without the need for costly probe cards and cleaning  solutions. The indentation test can also give valuable  information about the structural integrity of the solder bump.


Hardness, H = 11058 MPa


Elastic Modulus, E = 135 GPa


Figure 8: Schematic of the indentation technique for solder  bumps (a) and an optical micrograph of a typical bump (b) after testing to an applied load of 500 mN


A comparison between good and bad solder bumps is shown  in Fig. 9 where the effects of contamination are evident. A  corresponding load-depth cycle is also shown in Fig. 9(c) where the contact resistance is monitored simultaneously to  the load and depth data. This particular test cycle was  programmed to increase the applied load (FN) on the bump  until continuity occurs, this being characterized by a sudden  drop in the contact resistance (CR). The applied load required  to achieve continuity is often 50 – 80% higher in  contaminated bumps.


Figure 9: High quality solder bump (a) compared to a poor  solder bump which has significant contamination (b) after  loading up to 500 mN. Typical data in (c) shows the system  setup to increase load (FN) on the indenter until continuity  occurs, after which automatic unloading occurs. Contact  resistance (CR) and penetration depth (d) are monitored  throughout the test.


3. Wafer Probe Test


Probe tip damage (scrub mark) can be simulated in a  controlled way using the Microindentation Tester (MHT) with  a dedicated tip. The tungsten probe tip is mounted on to the tip  holder and isolated with epoxy as shown in Figure 10. This  allows a current to be applied or a resistance to be measured  via external connections as an indent is carried out with the  probe tip. This method is used to determine the effect of  contamination on the pad that can lead to an increase in  contact resistance. It is also useful in determining the applied  load required to make electrical contact.


Figure 10: Tungsten probe tip mounted as an indenter with  external connections


The advantage of using an actual probe tip (and not a diamond  indenter) is that the interaction between the probe test card  and the IC device can be investigated by simulating a single  probe tip interfacing with a bonding pad. This provides  valuable information about the integrity of the probe tip, a  measure of the applied load required to achieve continuity and  a quantitative image of the corresponding scrub mark created  on the bonding pad. Such tests have helped to optimize the  probe testing process and allow many more tests to be  performed before the probe test array has to be exchanged.


Figure 11: Typical load-depth curve for a multicycle probe  test (a) and the corresponding scrub mark (b) created by the  test in the bonding pad surface.


d


FN


CR


4. Adhesion of IC coatings


Several IC components are coated films that range in  thickness from a few nanometers to a micron with a variety of  material such as aluminum, copper, gold, titanium and  tungsten. Previous studies have shown the adhesion of a  coating to the substrate can be determined by scratch testing  using progressive loading. The technique involves generating  a controlled scratch with a tip on the sample. The tip, made of  diamond or hard metal, is drawn across the surface under  progressive load.  At a certain critical load, the material will  start to fail. The critical loads are determined by means of  investigation of optical observation, acoustic emission, frictional force, and penetration depth.  For example, Figure  12 shows a progressive load scratch using a Micro Scratch  Tester (MST) with a Rockwell diamond of 50µm radius on a  5µm thick coating of silicon dioxide on a silicon substrate. The critical load data is used to quantify the abrasionresistance of the coating or the adhesive properties of different  film-substrate combinations.


Figure 12: Progressive load scratch data for a SiO2 coating  on a Si substrate showing the critical failure point (dotted  line) at which the coating delaminates completely.


In this particular example, the SiO2 coating has failed by  delamination at an applied load of 1950 mN, this being shown  by a dotted line in Fig. 12. It can clearly be seen that the  failure is quantified by a sudden drop in the depth signal (PD) and by an increase in the friction signal (FT), these two  datasets being indicators of failure which can then be  correlated to the actual damage seen via optical microscopy. The residual depth (RD) is measured by passing the indenter  back along the scratch track with a very low load, in much the  same way as a stylus profilometer. This gives a measure of the  elastic recovery of the coating-substrate system after damage  and can be useful in quantifying the impact of the scratched  area on subsequent processes. As a general rule, a set of 3-5  scratches is usually performed on any given coating-substrate  system in order to investigate variations which can be due to  coating thickness, porosity in the coating, residual stresses  from the deposition process and variations in the substrate.


Figure 13: Progressive load scratch along a bonding pad  connector (a) which is coated with a diamond-like protective  coating. Zoomed image of the scratch (b) which confirmed a  coating failure load of 36 mN.


The localized positioning capability of the Open Platform  system permits the placing of a scratch test with sub-micron  positioning accuracy as demonstrated in Fig. 13. This shows a  progressive load scratch along a bonding pad connector which  is coated with a diamond-like protective coating. This  particular coating failed at an applied load of only 36 mN and  completely delaminated due to residual stresses from the  deposition process.


Development of new testing instruments and methods  illustrated in this paper has been driven by the need to produce  reliable ICs. Hardness, moduli, creep and fracture toughness  are determined through instrumented indentation. Adhesion, scratch resistance and visco-elastic recovery of coatings are  determined through scratch testing. Modifications to existing  instruments help simulate deformations and damages that may  occur during the fabrication process. These coupled with  surface roughness measurements with an AFM help  characterize the mechanical properties of IC components in a  true manufacturing environment. The initial work presented in  this paper is only the beginning of what will undoubtedly  become a very important part of future IC research and  development, encouraged by the next generation of testing  equipment.


(b)(a)


FT  RD


[1] W. C. Oliver and G. M. Pharr, “An improved technique  for determining hardness and elastic modulus using load  and displacement sensing indentation experiments”, J. Mater. Res. 7, pp. 1564-1583, 1992


[2] T. J. Bell, J. S. Field and M. V. Swain, “Stress-Strain  behaviour of thin films using a spherical tipped indenter”, Mat. Res. Soc. Symp. Proc. 239, pp. 331-336, 1992


[3] M. F. Doerner and W. D. Nix, “A method for interpreting  the data from depth-sensing indentation instruments”, J. Mater. Res. 1, pp. 601-609, 1986


[4] N. X. Randall, E. Hollander and C. Julia-Schmutz, “Characterisation if IC aluminium bonding pads by  nanoindentation and scanning force microscopy”, Surf. Coat. Tech. 99, pp. 111-117, 1998


[5] P. A. Steinmann and H. E. Hintermann, “A review of the  mechanical tests for assessment of thin-film adhesion”, J. Vac. Sci. Technol. A 7, pp. 2267-2272, 1989


[6] P. J. Burnett and D. S. Rickerby, “The scratch adhesion  test: an elastic-plastic indentation analysis”, Thin Solid  Films 157, pp. 233-254, 1988


[7] S. Bennett and A. Matthews, “Multi-function scratch  tester”, Surf. Coat. Tech. 74-75, pp. 869-876, 1995


[8] International Organization for Standardization ISO 14577  Part 4, Metallic materials – Instrumented indentation test  for hardness and materials parameters; test method for  metallic and non-metallic coatings (2007)


[9] ASTM E2546-07, Standard practice for instrumented  indentation testing (2007)


DOI: 10.1361/cp2008istfa128


Manufacturing In-Line Whole Wafer


Focused Ion Beam (FIB) Memory Address  Descramble Verification


Steven B. Herschbein, Hyoung H. Kang, Scott L. Jansen, Andrew S. Dalton


IBM Systems & Technology, Hopewell Junction, NY  USA


Test engineers and failure analyst familiar with random access  memory arrays have probably encountered the frustration of  dealing with address descrambling.  The resulting nonsequential internal bit cell counting scheme often means that  the location of the failing cell under investigation is nowhere  near where it is expected to be.  A logical to physical  algorithm for decoding the standard library block might have  been provided with the design, but is it still correct now that  the array has been halved and inverted to fit the available  space in a new processor chip?


Off-line labs have traditionally been tasked with array layout  verification.  In the past, hard and soft failures could be  induced on the frontside of finished product, then bitmapped  to see if the sites were in agreement.  As density tightened, flip-chip FIB techniques to induce a pattern of hard fails on  packaged devices came into practice.  While the backside FIB  edit method is effective, it is complex and expensive.


The installation of an in-line Dual Beam FIB created new  opportunities to move FA tasks out of the lab and into the  FAB.  Using a new edit procedure, selected wafers have an  extensive pattern of defects 'written' directly into the memory  array at an early process level.  Bitmapping of the RAM  blocks upon wafer completion is then used to verify  correlation between the physical damaged cells and the logical  sites called out in the test results.  This early feedback in-line  methodology has worked so well that it has almost entirely  displaced the complex laboratory procedure of backside FIB  memory array descramble verification.


In an ideal world, the layout of X and Y address decoders for  stand-alone and imbedded memory arrays would be arranged  from lowest to highest order, resulting in an progressive count  scheme. For a variety of reasons related to available layout  space, mirroring, interleaving, multiplexing, cross-talk  reduction, critical path length considerations, etc., this is often  not the case.  Row and column address lines may either go  thru a simple translation (swap) or be subject to a more


complex logic function that involves the elaborate  combination of two or more inputs.  The result is that  externally applied consecutive addresses may not yield  physically adjacent bits, but instead a seemingly random  distribution of data placement within the array.  In addition, the act of invoking redundancy can shift physical cell  distribution even further, possibly creating a unique case on  each and every device examined [1].   Data scrambling may  also take place, as bit and bit-bar mirroring by column or by  block is common.


Current generation microprocessors can have a dozen distinct  and independent memory arrays, including L1 & L2 cache, video, shift registers, instruction blocks, computational  storage, etc., executed in a number of different technologies.  SRAM (single and dual port), embedded DRAM, PROM and  Flash may all be represented.  Designers and layout teams  may create site specific arrays, but whenever possible will  choose from standard libraries of memory blocks.  Either way, they may have to customize them to provide the required data  width and depth, or fit the layout size and aspect ratio of the  available space.


Figure 1.  IBM POWER6 microprocessor showing better than  a dozen memory arrays banks.  Some are well documented, others may need independent verification.


Impact on Test and FA


The documentation available with many of the standard  library offerings typically includes logical to physical address  and data descramble information, as well as how to locate  redundancy replacement elements.  Verifying the accuracy of  the translations used in a given layout is important especially  if the array is modified to fit, as it can have a profound impact  on both test coverage and the failure analysis process itself.   Imagine if a test engineer intended to write a 'surround disturb' pattern to check for neighboring cell influence, but actually  scatter the data throughout the array!  Or more to the point for  the FA community, if the failing cell called out in a bit map  was physically nowhere near the suggested location, resulting  in continuous 'no defect found' analyses.  These issues are  further compounded by designs that do not allow direct access  to embedded arrays for test purposes, but require filtering thru  core logic.


Various schemes have been developed to enable tester pattern  generators to reorder, or ‘untwist’ the external bit stream to  produce a correct internal array address, but can they be  trusted [2]?  Too often in real-world applications, the provided  descramble algorithm is found to be wrong or needs ‘adjustment’ to function reliably.


Figure 2.  Example logic diagram showing address  descrambling.  A  sequentially applied external binary  address becomes convoluted, producing a very different  internal data distribution.


FA Lab Verification


Failure analysis labs have a long history of active participation  in memory array layout verification to ensure test data  accuracy.  Earliest work included the use of probe station  small spot high intensity light and later laser stimulation to 'flip' cells during active read/write cycling.  Some relaxed  layouts could be accessed by FIB or laser oblation from the  frontside to induce physical damage in a specified pattern (stuck cells) for map verification.


Eventually, when density, robustness and spatial resolution  precluded these simplistic methods, some labs turned to  physical damage through the backside silicon [3].  This is  typically done on finished devices using a flipchip style FIB  tool to induce fixed fails for bitmapping.


B/L W/L


64SPmem3


35


64SPmem1


538


1005


88C4mem0


4L1mem4


440


63


94C6mem2


539


54Q0mem11


27


215


18L2mem14


263


68


44Q1mem6


89


12L2mem1


Figure 3.  Access to multiple arrays on a modern  microprocessor can take extensive backside FIB tool time, patience and expertise.


SEGMENT


Figure 4.  Layout to backside validation.  Cells exposed for  viewing purposes only – region on a working device would  remain fully covered with the exception of the deleted cell.


While this is indeed a very effective method, it requires  waiting until functional packaged hardware becomes


available.  Plus, it necessitates the full procedure of backside  silicon excavation, blind targeting, and exacting single cell  deletion.  It becomes particularly time consuming and prone to  failure when multiple arrays need to be verified.  Not many  labs have the technology and capacity to support this on a  volume basis, especially if it involves processes based on bulk  rather than the easier to manipulate silicon-on-insulator  CMOS.  Clearly, a better methodology was needed to support  the high volume of new designs being introduced.


Lab to Fab Migration


The current trend in successful development operations is a  growing dependence on early feedback.  Design verification, validation of test coverage, and process yield learning can no  longer take place serially; all must advance in parallel in order  to achieve tight time-to-market targets.  Recognizing this  need, a few papers have been published on the value of the inline FIB as an early learning tool for construction analysis and  defect root-cause determination [4] [5] [6].


In 2004, the IBM 300mm wafer line in East Fishkill, NY  installed an FEI DA-300hp Dual Beam FIB tool.  This dual  FOUP-equipped full wafer system is capable of conventional  low keV SEM inspection along with die surface modification  using the gallium ion beam column.  Navigation across the  entire wafer to any selected defect site or array blocks can be  achieved using the KLARFF coordinate system, or by layout  design information.  The acquisition of this system opened up  the possibility of moving certain failure analysis tasks out of  the lab and into the fabrication environment.


Experiments were defined to determine the suitability of  returning wafers subjected to limited ion beam exposure to  their lots for subsequent processing.  Limited approval was  granted for engineering evaluation purposes.    Engineering  lots that have completed the basic transistor fabrication  process can be routed to the FIB for mid or back end wiring  changes, then returned to the line to complete the wafer build.   While we have successfully performed full logic changes inline (cuts and conductor deposition to correct errors), our most  extensive experience is in doing simple 'deletes' to simulate  memory array defects. In this procedure we ‘write’ a pattern  of defects directly into a memory array at an early mask level.  Electrical bit mapping of these sites upon wafer completion is  then used to verify correlation between logical and physical  addressing of the array [7].   This analysis has been done not  on just specially designed kerf or die test sites emulating array  designs, but on actual embedded memory on microprocessor  products.


The test plan called for a short hold on a wafer after tungsten  stud CMP level, prior to ILD and M1.  Memory arrays that  were of interest to the test community were easily identified, and a set of cells located using low voltage SEM imaging.


The ion beam was then used to mill a fine “F” shaped pattern  of discrete points into the surface, destroying a single contact  within each cell location.  The “F” was chosen because even if  rotated or mirrored, the pattern of zapped cells as displayed in  an array bitmap would be unique and recognizable.  If the  bitmap visual output resolves to an “F” and is in the proper  orientation, the descramble table is probably correct.  Rotation  or scattered bits suggests a problem warranting further study.


Figure 5.  Dual Beam FIB image of memory cell structure at  tungsten contact level selectively damaged in a unique “F” pattern, then run through the line until the point of full  memory test and failure bit map.


Figure 6.  Test results from memory bitmap testing (SRAM  array functional test) showing that the only failing cells in this  array block are those induced by the in-line FIB.


Depending on the block design, some memory arrays are fully  testable using a resident pad cage as early as metal level 4.  This is a huge advantage for early learning and yield  diagnostics, as it may save weeks of raw fab cycle and process  time.  It also means that full die functionality is not essential  for memory diagnostics, as the processor core and other  support architecture is most likely not being utilized in order


to access the embedded array.  Even if the initial wafer final  test yield is overall very low, we still stand a good chance of  obtaining usable logical to physical descramble verification  data.  With this advantage, only a few die on one to two  wafers need be subject to the FIB “F” treatment to verify each  new design.


Figure 7: Three die are selected from the ‘sweet spot’ region  of the wafer for verification.  Two of the three typically yield  useable bitmap data.


Large “F” shaped patterns made up of multiple smaller “F’s” were also performed.  Doing so increases our overall  confidence level, and allowed us to evaluate multiple array  blocks that were arranged ‘back to back’.  This is an important  step in checking on the impact of layout ‘mirroring’.


Figure 8: Multiple “F” patterns to check for array mirroring  and correct block addressing.


It is not uncommon to have a scattered failing bit or two in  other areas of the array, unrelated to the FIB induced sites.  Unfortunate, there is no way of predetermining if a chip will  be defect-free before selection, and redundancy cannot be  invoked without creating further confusion.  Doing a few sites  allows us to separate the random dead cells from an actual  decoder layout issue.


Figure 9:  Bit map shows that all nine “F” patterns were  successfully milled in the sub-array, and that the  descramble algorithm is correct in this case.


Incorrect address scrambling information can exact a high toll  on ATE test integrity and failure analysis results.  Laboratory  frontside methods of inducing single cell defects for bitmap  verification began to fail when line density precluded clear  access to the individual features of the bit.  Backside FIB  editing procedures certainly work, but are extremely difficult  and time consuming.


The advent of the in-line dual beam FIB opened up the  opportunity to modify partially processed wafers and return  them to the fab to complete the build cycle.  A known pattern  of damaged cells was induced just above the first level of  transistor interconnects, and the arrays bitmapped at the  earliest metal level that allowed full memory testing.  The  result has been a real breakthrough in early learning.  By  insuring correct descramble, the ‘no defect found’ rate on  reliability test failure submissions has been reduced, speeding  up the overall new product qualification process.


The authors wish to thank Brad Austin for preparing the  bitmap images used in this paper.


[1] M. Franklin, et al, “Testing reconfigured RAM's and  scrambled address RAM's for pattern sensitive faults,” IEEE Transactions on CAD of Integrated Ckts & Systems, Sept 1996, pp. 1081-1087.


[2] G. Lehmann, et al, USPTO 6601205 – Infineon/IBM – Method to Descramble the Data Mapping in Memory  Ckts, 7/29/03


[3] S. Herschbein, et al, “FIB Chip Repair: Improving  Success by Controlling Beam-Induced Damage and  Thermal/Mechanical Stress,” Proc. 30th ISTFA, Worcester, MA, Nov. 2004, pp. 166-171.


[4] R. Weiland, et al, “Wafer Conserving Full Range  Construction Analysis for IC Fabrication and Process  Development based on FIB / Dual Beam Inline  Application,” Proc. 26th ISTFA, Bellevue WA, Nov. 2000, pp. 393-396.


[5] G. Franco, et al, “An Initial Investigation into the use of  FIB Technology for In-line Process Control of Critical  Dimensions in the FAB,” Proc. Of ISSM 2005, San Jose, CA,  Sept. 2005, pp. 394-397.


[6] S. Blanc-Coquand, et al, “Automated Defect Crosssectioning with a In-line Dualbeam,” SPIE Metrology & Inspection Conference 2004, Santa Clara, CA,  Sept. 2005, pp. 819-896.


[7] S. Herschbein, et al, “FIB: A Design Repair, Fault  Isolation Tool,” ISTFA Tutorial Program, 33th ISTFA, San Jose, CA, Nov. 2007, slide 99.


DOI: 10.1361/cp2008istfa133


An Analysis of Tungsten FIB-Fabricated Via Resistance


David W. Niles, Jay Meyer, and Ronald W. Kee  Avago Technologies, Fort Collins, Colorado USA  david.niles@avagotech.com


Michael DiBattista


FEI Corporation, Hillsboro, Oregon USA


We present an analysis of tungsten vias fabricated by a  focused ion beam with regard to the understanding of circuit  editing strategies. The growth rate of W is ~10 times faster in  high aspect ratio vias than on flat surfaces, and W in vias has 4  at. % more C but only one-tenth the Ga of surface-deposited  W. We propose that vias act like small Faraday cups, trapping  the energy of the Ga+ ions and the reaction byproducts to  enhance the growth rate of W and to increase the C to W ratio  in vias compared to flat surfaces. The resistivity of W in the  vias determined by a least squares fit to resistance data is 250 µΩ-cm, unchanged from the resistivity of W deposited on a  flat surface. The resistances of the vias fabricated in a SiO2  layer to contact an underlying Al sheet layer fit well to either  of two models: 1) an effective area model that invokes  resistive via sidewalls that do not participate in conduction, and 2) an contact resistance model that invokes tapered vias  with a constricted W/Al contact area.


The resistance and resistivity of metal lines deposited in the  focused ion beam (FIB) environment has been studied in detail [1-5]. Tungsten and Platinum have emerged as standards for  FIB editing circuits in the industrial arena, showing good  performance and reliability [1,2]. With the downward scaling  of semiconductor layout geometries, the role of the vias in  FIB-deposited interconnect strategies has increased in  significance. Our experience is that effective FIB operators  should try to steer designers away from difficult FIB  procedures such as high aspect ratio (length to cross-sectional  area) vias, but may find some moderately high aspect ratio  vias unavoidable.


Figure 1: Example of a 7:1 aspect ratio (length to area) via in  90nm Cu technology.


As an example, Fig. 1 shows a high aspect ratio W via  fabricated in an FEI VectraVision on a 90 nm Copper  technology flip chip circuit. Because the via was not along the  edge of a chip, we made a stair-step cross section cut to allow  viewing in a scanning electron microscope (SEM) at a 45° angle. We delineated with a buffered oxide etch and coated  with a thin layer of AuPd to prevent charging. The apparent  gaps in the via along the sidewalls are a result of the buffered  oxide etch. The via spans four layers of Cu metal to make  contact to a metal 5 bus line, and a jumper connects the top of  the via to a neighboring metal 9 bus line. The 45° degree angle  belies the true aspect ratio of 7:1. Although the via clearly  makes good contact to the metal 5 bus line and shows no  presence of voids, the resistivity of the W comprising the via  is not known but rather assumed to equal to the resistivity of  W deposited on a flat surface.


For direct current electrical measurements, one can calculate


an expected value for the resistance of the via from the  resistivity of the W metal and the geometry using the  equation:


R = ρ*L/A,


where ρ is the resistivity of the deposited W metal (typically  250 µΩ-cm for flat surface W), L is the via length, and A is  the cross-sectional area [3,4]. The total resistance of a FIBdeposited connection between two metal traces such as the  example in Fig. 1 will comprise the resistance of the jumper  connecting the top of the via to the metal 9 bus line, the  resistance of the via, and the contact resistances of the  deposited W to both Cu metal lines [4]. The key difference  between a simple metal 9 to metal 9 jumper and the image in  Fig. 1 is the resistance of the via from the top of metal 9 down  to metal 5. The via’s contribution to resistance is important for  understanding voltage drops across connections and timing  delays for circuit edits on high frequency applied specific  integrated circuits.


As a function of its aspect ratio, a via may contain voids that  diminish conductivity, as discussed in Reference [4], or  simply be poorly filled with metal (hereafter, the fill factor). Another uncertainty is that the composition of the deposited  material in the via may differ from that deposited on a flat  surface depending on the ion beam and gas parameters during  the deposition, and the composition may vary along the length  of the via. For instance, the C and O content may be more or  less than expected depending on the ability of the C and O  containing byproducts to escape from the via during growth.


  A Dremel tool with a cutting disk  works well to separate the portion of the circuit board  containing the failed device from the rest of the board.  The  sensitivity to elevated temperatures can be used as an  additional diagnostic tool:  If briefly heating the failed device  with a heat gun causes the leakage to disappear, and a few  minutes of normal operating bias restores the leakage, then  another signature of silver migration has been identified.


While performing the electrical isolation, the analyst should  keep in mind that there are some failure locations that are not  obvious.  For instance, the lead frame tie bar that is electrically  connected to the die paddle and extends out between the  corner leads can act as one terminal of the migration cell.  This  tie bar will be at some potential, often at zero volts in the case  of an exposed paddle package where the paddle is soldered to  the circuit board ground plane.  Unbonded device pins that are  connected to ground on the circuit board could also become  part of the migration cell, as could pins that are labeled as “no  connects” but are bonded to the die for testing or diagnostic  purposes.  Silver migration has also been observed on the die  surface between adjacent bond pads.  A bond pad that is not  bonded to a lead finger but is internally biased to some  potential can also become part of a migration cell with an  adjacent bond pad.


Physical Analysis


X-ray analysis of the failed device should always be  performed.  Careful selection of exposure energy can reveal a


silver migration artifact between the package lead fingers in  some instances.  The successful resolution of the migrated  silver is dependent upon the quantity of silver involved.  Figure 1 shows one example of an area of silver migration that  was resolved using X-ray analysis.


Figure 1:  X-ray image showing location of silver migration  between lead frame fingers.


Surface or parallel polishing is the preferred method for  revealing the silver migration artifact.  The failed device  should be mounted to the sample holder using a two part  epoxy or some other adhesive medium that does not introduce  heat.  If the device is still mounted to a portion of circuit  board, this procedure still works well.  Maxim has designed  and fabricated a manual surface polish system for use in our  laboratory that is well suited to this type of parallel polish.  This system allows fine control over the polishing rate and  facilitates frequent visual inspections that are necessary to  avoid polishing through the artifact.  Figure 2 shows the  polishing system used at Maxim, while Figure 3 shows a  sample prepared for surface polish.


Figure 2:  Surface polishing system.


Figure 3:  Device mounted to stainless steel surface polish  puck, ready for polishing.


After the adhesive holding the device to the polishing puck is  well cured, the surface polish can begin.  Typically, the polish  is performed using 600 grit silicon carbide media.  The surface  polish removes material from the top side of the package.  By  polishing until the loops in the bond wires between the die and  lead fingers have been severed, the location of the migration  can be electrically isolated.  Microprobing the two wire ends  that connect to the lead fingers of the leaky pins, then the wire  ends that are bonded to the die, will isolate the leakage to  either of these two locations.  In those cases where x-ray  analysis revealed the location of the silver migration, this  provides additional confirmation.  Once the leakage is isolated  at the die or the package lead fingers, additional surface  polishing is required to expose the silver migration.  For 48  TQFP packages and larger, the surface polish can continue  with the 600 grit silicon carbide media.  The polishing rate of  the 600 grit media naturally drops as the media becomes  contaminated with package encapsulant particles.  Thus as the  die surface or lead frame is approached the polish rate will be  quite slow and controllable.  For packages smaller than 48  TQFP, a finer abrasive might be needed to insure sufficient  control when approaching the die or lead fingers.


Metal Migration Between Package Lead Fingers


If microprobe continuity measurements between adjacent  bond wires indicates leakage at the lead fingers, then surface  polishing can continue close to the plane of the lead fingers.  When approaching the plane of the lead fingers, frequent  iterative microscope inspections concentrating on the area  between the two leads of interest should be performed.  The  entire length between the two lead fingers should be carefully  inspected unless previous x-ray analysis revealed an anomaly  between the two fingers, in which case attention can be  focused on that area.  The silver migration is usually identified  through one or more of the glass filler particles in the molding  compound.  The filler particles can act like a lens, providing a  good view of the migration artifact.  An example of this is  shown in the light micrograph of Figure 4.


Figure 4:  Optical micrograph showing silver migration  artifact viewed through a glass filler particle in the molding  compound.


The silver migration can only occur through the plastic portion  of the encapsulant, not through the glass filler particles.  Thus  the migration occurs in three dimensions, weaving around the  glass particles.  After the migration artifact has been visually  detected through a filler particle, the polish can proceed  carefully until the artifact has been partially exposed.  Figure 5  is a light micrograph showing a migration “vein".


Figure 5:  Optical micrograph showing silver migration “vein” traveling through molding compound.


After the vein is exposed, EDX or WDX analysis can be  performed to verify the presence of silver or copper.  WDX  dot map analysis can provide a dramatic image of the path  taken by the migration.  Elemental analysis should also be


performed to check for the presence of phosphorus.  Many  times the amount of phosphorous is small and difficult to  detect using WDX or EDX analysis.  If the presence of  phosphorous can be detected and confirmed, it provides  additional confirmation that the root cause of the failure was  due to a phosphorus flame retardant particle.  Figure 6 shows  an SEM micrograph of the area of silver migration, while  Figure 7 is a WDX dot map for silver that correlates exactly to  the micrograph of Figure 6.


Figure 6:  SEM micrograph of silver migration “vein”.


Figure 7:  WDX dot map indicating the presence of silver.  This image correlates exactly to the silver vein shown in the  SEM image of Figure 6.


Another example of surface polish analysis is shown in  Figures 8 through 12.  In this case a much more severe  migration occurred, indicated by the silver colored “cloud” adjacent to the lead finger in the optical micrograph of Figure


8.


Figure 8:  Optical micrograph showing a “cloud” indicative  of severe silver migration between lead fingers.


An SEM micrograph of a portion of this area is shown in  Figure 9, while WDX dot map analysis results for silver and  phosphorous are shown in Figures 10 and 11, respectively.


Figure 9:  SEM micrograph of the area of the silver migration  artifact shown in the optical micrograph of Figure 8.  This  micrograph shows the area on which WDX analysis was  performed for silver and phosphorus as shown in Figures 10  and 11.


Figure 10:  WDX dot map indicating the presence of silver.  This image correlates exactly to the area shown in the SEM  image of Figure 9.


Figure 11:  WDX dot map analysis indicating the presence of  phosphorous.  This image also correlates to the area shown in  the SEM image of Figure 9.


The WDX dot map results of Figure 11 clearly show the  involvement of phosphorous in this failure.


Metal Migration Between Bond Pads on the Die


If microprobing the severed bond wires shows that the  resistive leakage is located on the die, two different methods  can be used to confirm the presence of silver migration.  In  both cases, the surface polish should continue until the  encapsulant above the area of interest is as thin as possible, on  the order of a few microns.  As was the case at the lead  fingers, a migration artifact between the bond pads should be  visible through the glass filler particles in the encapsulant.  The first technique to confirm metal migration uses a FIB to  mill a hole in the encapsulant over the suspected area of  migration.  Passive voltage contrast [8] provides a good means  of end point detection to indicate when the migrated silver has  been exposed.  EDX or WDX analysis can then be performed  in the milled hole to verify the presence of silver.  Good  success has been achieved with milled holes that were  approximately 10µm by 10µm in size.  Performing the milling  operation within the confines of a glass filler particle provides  more uniform milling, and dielectric etch gas hastens the  operation.  To prevent charging, the entire sample can be  sputter coated with gold, with additional FIB deposited  platinum in the area to be milled.  A FIB cross section can also  be performed to examine the structures in the area of the  migrated silver, as shown in Figure 12.


Figure 12:  SEM micrograph of FIB cross section of silver  migration between bond pads on die surface.


Another technique to examine and analyze the metal migration  between bond pads is to use a lift-off technique.  After the  encapsulant over the area of interest has been thinned as much  as possible, a xenon laser is used to cut the encapsulant around  the periphery of the two affected bond pads.  Ordinary  adhesive tape is then applied to the surface of the polished  sample and rubbed with a soft eraser to ensure good adhesion.  The tape is then removed, lifting the cut section of encapsulant  off of the die.  If the laser cut around the area of interest is  complete and the tape adhesion is good, the lift-off should be  successful without any additional steps.  This technique allows


encapsulant


silver


die


examination of both the die surface and the encapsulant that  was in contact with it.  Figures 13 and 14 show the SEM  image of the die surface and the corresponding WDX dot map  analysis for silver.


Figure 13:  SEM micrograph of die surface where thinned  encapsulant has been lifted-off with adhesive tape.


Figure 14:  WDX dot map analysis indicating the presence of  silver on the die surface.  This image correlates exactly to the  area shown in the SEM image of Figure 13.


Figures 15 and 16 show the SEM image of the encapsulant  above this area and its corresponding WDX dot map analysis.


Figure 15:  SEM micrograph of thinned encapsulant that was  lifted from the area shown in Figure 13.


Figure 16:  WDX dot map analysis indicating the presence of  silver on the underside of the encapsulant.  This image  correlates exactly to the area shown in the SEM image of  Figure 15.


Laser cut to define lift-off area


Replication of bond pad edge in encapsulant


Bond pad


If a large number of samples are available for analysis, another  technique has been used to expose silver migration that has  occurred on the die surface.  This technique consists of  mechanically decapsulating the package using a hobby knife  and hot plate.  Heating the failed device to approximately  200°C softens the encapsulant somewhat and allows the  package body to be separated from the die.  This technique is  risky since it can result in destruction of the sample, thus the  recommendation that a large number of samples be available.  Results of a mechanical decapsulation can be seen in the light  micrographs of Figures 17 and 18.  Figure 17 shows the silver  migration present on the die surface, and Figure 18 shows the  migration present on the mating encapsulant surface.


Figure 17:  Optical micrograph showing silver migration  between adjacent bond pads on the die surface after  mechanical decapsulation.


Figure 18:  Optical micrograph showing silver migration on  the package body after mechanical decapsulation.


Novel Analysis Techniques


In this section two additional techniques that have shown to be  useful in isolating and imaging the location of silver migration  are presented.


FIB Passive Voltage Contrast


A novel technique to observe the presence of the silver  migration during the course of the surface polish is the use of  FIB passive voltage contrast.  One or both of the suspected  leads must have a good connection to ground while in the FIB.  Also, since the migration travels in three dimensions, the  analyst must take care during surface polishing not to sever  the current path to the leads before imaging.  Figure 19 shows  a passive voltage contrast image where the location of the  migrated silver is very apparent.


Figure 19:  FIB passive voltage contrast image of silver  migration on surface polished sample.


SQUID Microscopy


In cases where the leakage path caused by the silver migration  is relatively stable, SQUID (Superconducting QUantum  Interference Device) microscopy has been successful in  determining the location of the migration.  Figure 20 is a  combination of current density and current density peak  profile maps that are superimposed on the optical image of a  48 TQFP device.  This analysis indicated that the location of  the leakage path between two adjacent pins was at the bond  pad area of the die.  Subsequent surface polishing of the  device confirmed that silver migration was present at this  location.


Others have also found SQUID microscopy to be an effective  technique to identify the location of leakage currents resulting  from metal migration associated with red phosphorus flame


lead finger


retardant.  More detailed information about this technique can  be found in their work [9].


Figure 20:  SQUID analysis showing location of leakage path  is between adjacent bond pads. Subsequent surface polish  confirmed this result.  (Image courtesy of Neocera, Inc.)


Analysis Flowchart


An analysis flowchart is shown in Figure 21 that summarizes  the analysis steps used to isolate silver migration in plastic  encapsulated devices.


The failure mechanism of silver migration associated with  phosphorus bearing molding compounds was described.  A  brief overview of the theory behind this mechanism was  discussed, as were observations of time to failure and  approximate observed failure rates.  Techniques were  presented to aid in the electrical diagnosis and isolation of the  migration artifact.  Physical analysis techniques were  described to identify and characterize migration that occurred  between bond pads on the die surface or at the lead fingers in  the package body.  Analytical techniques such as WDX were  used to confirm the presence of silver and phosphorus, helping  to confirm the root cause of failure.  A novel FIB passive  voltage contrast technique was also described to view silver  migration in the plastic encapsulant.


It is hoped that this paper will be instructive to the failure  analysis community in recognizing and analyzing devices that  could potentially suffer from this failure mechanism.  The  techniques described in this paper can be used to successfully  analyze devices with other failure mechanisms that result in  leakage currents or adjacent pin shorts.


Unit failed in field


Measure DC bias


voltage on all pins


with device in application


Measure suspicious adjacent


pins with curve tracer


Cut out portion of circuit board


containing unit


Prepare unit for surface polish


Surface polish until bond wire


loops are severed


Microprobe to determine if


short is located at die or lead fingers


If short is at die:


If short is at  lead fingers:


Continue surface polish


Iterative surface polish


to thin encapsulant over


and inspection.  Check


die to a few microns


for migration through  glass filler particles


Use FIB or lift-off


Continue polish to


technique to expose


expose migration


migration


Perform elemental


analysis to confirm


presence of silver


presence of silver and/or


and phosphorus


copper and phosphorus


Figure 21:  Silver migration analysis flowchart.


The author would like to thank Lawrence Benedict of Maxim  for his extensive electrical measurements and characterization  of failed devices, and Mark Kimball of Maxim for  development of the lift-off technique to analyze migration that  has occurred on the die surface.  Thanks also go to Norio  Yasui of Maxim Japan for translation of the article listed in  Reference 4, Joan Dwire of Maxim for extensive WDX  analysis work, and also to Neocera Inc., for SQUID analysis  and permission to use their analysis results.  Many individuals  too numerous to list also contributed to this project, particularly during the initial discovery phase of this failure  mechanism.  Thank you all.


[1] G.T. Kohman, H.W. Hermance, and G.H. Downes, “Silver Migration in Electrical Insulation,” The Bell  System Technical Journal, Vol. XXXIV, No. 6, 1115-1147 (1955)


[2] A. Gallo, “Green Molding Compounds,” Dexter  Technology Information Technical Paper (2000)


[3] “Failures Attributed to Phosphorus in Molding  Compounds,”


http://www.calce.umd.edu/whats_new/2002/Phosphorus_


020926.htm, September 26, 2002


[4] “What Caused the Troubles of Fujitsu-Made HDDs,” Nikkei Electronics, Issue No. 833, 99-119, October 21, 2002


[5] M. Pecht and Y. Deng, “Electronic Device Encapsulation  using Red Phosphorus Flame Retardants,” Microelectronics Reliability, Vol. 46, Issue 1, 53-62 (2006)


[6] Y. Deng and M. Pecht, “The Story Behind the Red  Phosphorus Mold Compound Device Failures,” The  Journal of the Reliability Information Analysis Center, http://www.theriac.org/DeskReference/PDFs/2006Q3.pdf, Third Quarter (2006)


[7] “Notice to Customers and Industry:  Field Failures  associated with Sumitomo EMExxxxU Series  phosphorus-based molding compound,” www.maximic.com (2002)


[8] S. Zhigang, L.S. Khim, and S. Redkar, “Passive Voltage  Contrast Application on Analysis of Gate Oxide Failure in


0.25µm Technology,” ISTFA Proceedings, 93-95 (2000)


[9] Y. Deng, M. Pecht, and K. Rogers, “Analysis of  Phosphorus Flame Retardant Induced Leakage Currents in  IC Packages Using Squid Microscopy,” IEEE  Transactions on Components and Packaging  Technologies, Vol. 29, No. 4, 804-808 (2006)


DOI: 10.1361/cp2008istfa121


Emerging Techniques for the Characterization of Nano-Mechanical Properties of  Integrated Circuit Components


Nicholas Randall and Rahul Premachandran Nair


CSM Instruments, Needham MA02132 USA


nicholas.randall@csm-instruments.com, 781-444-2250


With the growing complexity of integrated circuits (IC) comes  the issue of quality control during the manufacturing process. In order to avoid late realization of design flaws which could  be very expensive, the characterization of the mechanical  properties of the IC components needs to be carried out in a  more efficient and standardized manner. The effects of  changes in the manufacturing process and materials used on  the functioning and reliability of the final device also need to  be addressed. Initial work on accurately determining several  key mechanical properties of bonding pads, solder bumps and  coatings using a combination of different methods and  equipment has been summarized.


At present, the tools available to the Failure Analysis engineer  for characterizing the mechanical properties of a device, or  part of a device, have been limited to stand-alone instruments  which cannot be integrated into a production line or QC  process. In addition, such instruments are usually dedicated to  a single task and cannot easily be coupled with existing in-line  characterization tools for fast analysis both at the wafer and  component levels.


The development of Integrated Circuit (IC) and other  semiconductor devices has, in recent years, been more  focussed on the fabrication process than on issues concerning  reliability and the link to mechanical properties. Many issues  related to tribology, mechanics, surface chemistry and  materials science should be considered in the operation and  manufacture of many devices. At present, very few analytical  instruments are available for accurate characterisation of  localised properties and specific zones of interest.


The indentation method for assessing mechanical properties at  low loads and shallow depths is already well established for  the characterisation of thin films as well as bulk materials. The  depth-sensing indentation method (Fig. 1) produces a loaddisplacement curve from which quantitative property values  can be calculated using a variety of approaches1-3. Additionally, the indenter (of defined geometry) can be  accurately controlled in terms of load, depth and speed of  application. Provided that the indenter can be accurately  positioned on a site of interest, then the technique can be used


to probe the local mechanical properties of different  structures, either with single or more complicated loading  cycles. Previous work has already shown the application of  indentation at the nanometer scale for characterising the  properties of extremely small structures such as integrated  circuit bonding pads4.


Figure 1: Principle of the instrumented indentation method  where an indenter penetrates into the sample (a) whilst  simultaneously recording a load vs. depth curve (b).


In addition to the quasi-static indentation method, where an  indenter is moving solely in the vertical direction, the simple  addition of an accurate displacement stage enables the sample  to be moved horizontally, thus enabling a scratching function. In conventional scratch testing (Fig. 2), a diamond stylus is  drawn across the sample under either constant or  progressively increasing load. Elastic and/or plastic  deformation occurs at specific points along the scratch path, such critical points being observed by optical microscopy or  by variations in acoustic emission and frictional force5-7. In  many cases, the scratch test has now become accepted as a  versatile tool for assessing the mechanical integrity of a  surface, whether bulk or coated, and has found application in  many different fields of materials research8-9. The driving  forces for the failure of a coating-substrate system in the  scratch test are a combination of elastic-plastic indentation  stresses, frictional stresses and the residual internal stress  present in the coating. The normal load at which failure occurs  is called the critical load, Lc. When a progressive load scratch  is performed, a number of consecutive coating failure events  may be observed as the load is increased, the final event  corresponding usually to total delamination. The critical load  depends on coating adhesion, but also on several other  parameters; some are directly related to the test itself (intrinsic  parameters) whereas others are related to the coating-substrate  combination (extrinsic parameters).


Figure 2: Principle of the scratch test for measuring the  adhesion of coatings. The indenter passes across the surface  with increasing applied load, whilst recording the penetration  depth, tangential force and acoustic emission.


A large proportion of modern semiconductor devices are made  of silicon using complex manufacturing processes. As the  applications of such devices increase, it is anticipated that all  classes of materials (metals, ceramics, polymers, composites) will become important. There are certain unique features of  the mechanical properties of each class that require the testing  procedures to vary from one to another. The properties  considered to be important for the design of IC devices  include the strength (yield, ultimate, fatigue), moduli, toughness, friction, adhesion, damping, Poisson’s ratio and  residual stresses. From a manufacturing point-of-view, mechanical properties such as strength, hardness, scratch  resistance and chemical-mechanical behaviour are important. The effect of the manufacturing procedure on the device  properties also needs to be addressed. Properties such as crack  propagation, friction, wear, fatigue, adhesion and property  changes due to corrosion/oxidation/erosion during service will  determine the lifetime of a device. Additionally, there is a  growing demand for mechanical testing to be combined with  electrical testing in the same platform so that a defined stress  can be correlated to a change in electrical signal.


This paper presents a new and fully automated test platform  which is dedicated to measuring the mechanical properties of  highly localized areas of a system, whether discrete or as part  of a wafer containing many thousands of devices. A wide  choice of indenter geometries and test methods (indentation, scratch, tribology), coupled with suitable imaging methods (AFM, confocal, optical) make this modular solution the ideal  choice for in-line characterization. The utilization of such an  automated test platform on an IC production line allows a fast  and efficient way of probing mechanical properties in a highly  reproducible manner and in conformance with up-to-date  ASTM standards8-9. A wide range of test examples are shown  in the form of case studies, such as the mechanical properties  of bonding pads, solder bumps, metallization layers and probe  test needles.


The instrument used for all tests was a CSM Instruments Open  PlatformTM mounted with 4 modules as follows:


• Nanoindentation Tester: automated indentation head  with maximum applied load of 500 mN and a  Berkovich (3-sided) pyramidal indenter


• Nano Scratch Tester: ultra low load scratch testing  head with a 10 µm radius spherical diamond  indenter. Maximum applied load of 1000 mN


• Atomic Force Microscope (AFM): three-dimensional  imaging up to a maximum image size of 80 µm x 80 µm.


• Video Optical Microscope: allows standard optical  microscopy which enables exact positioning of the  site to be tested.


The sample is mounted on a displacement stage capable of  moving in XY (horizontal) and Z (vertical) axes, the former  for displacing the sample under either of the 4 test modules, the latter for automated approach of the sample under any  given module. The horizontal displacement resolution (0.25 µm in each axis) allows even the smallest feature on the  device to be selected for an indentation or scratch test. The  complete system is shown in Fig. 3 and can be integrated into  a production line for automated quality control testing.


Figure 3: Fully automated Open Platform for wafer level  testing with XYZ sample positioning and four test modules, from left to right: Nano Scratch, Nanoindentation, Atomic  Force Microscope (AFM) and Video Optical Microscope.


Full software control allows the user to programme any  number of coordinates for testing, after which the system  automatically translates to each site and makes a test (to preselected parameters) with a small retraction and approach  phase between each site. This platform can accommodate  wafers of any size up to 12” diameter. A large range of  indenter geometries can be used, including spherical, pyramidal and flat punch.


1. Bonding Pads


The hardness of bonding pads can be characterized using a  Nanoindentation Tester (NHT) combined with an optical  microscope. Figure 4 shows aluminum bonding pads that were  tested for hardness by performing instrumented indentation  with a Vickers tip using the NHT. Ten indents were carried  out precisely on the chosen bonding pad as shown in Figure  4(b) by using the positional synchronization capability  between the optical microscope and the indentation head.


Figure 4: Optical micrograph of a typical IC layout, together  with a zoomed image of a single bonding pad where 10  nanoindentations (white arrows) have been made with max. load 5 mN


Another important function of the bonding pad is to provide a  platform onto which connecting wires can be attached. During  the thermosonic bonding process one end of the gold wire is  attached to the pad by pressing the wire against the pad and  using ultrasonic motion and the other using tailless ball  bonding. The transfer of the energy during the ultrasonic  motion depends on optimum surface roughness of both the  capillary and the pad and thus determines the quality of the  bond.


An Atomic Force Microscope (AFM) can be used to derive  the root mean square (RMS) roughness of the surface as  shown on the AFM image of an indent on a bonding pad in  Figure 5(a). The micrograph in Fig. 5(b) shows a mounted and  polished section through a gold wire thermosonic bond onto  an aluminum bonding pad. A line of nanoindentations has  been made across the boundary between the Si substrate, the  Al bonding pad (a coating of thickness 3 µm) and the gold  bonded ball.


Nanoindentation is often used to measure the effects of the  thermosonic bonding process on the gold bonding wire. This  wire can often suffer from work-hardening effects as a result  of bending, as well as softening in some areas due to localized  annealing of the material. The wire can be mounted and  polished and then indented in different regions to measure the  localized hardness. An example of such results is shown in  Fig. 5(c) where hardness values have been plotted as a  function of position along the wire, and compared with the


hardness of the actual bonding pad onto which the gold wire  has been attached. The ball, neck and wire areas of the wire  are shown in Fig. 5(b) for reference. It is interesting to note  that the hardness is highest in the ball section, this being due  to work-hardening of the gold when it is bonded under  pressure to the pad. The subsequent cooling takes place too  rapidly for the gold to anneal and soften. This interface has  been found to be the cause of numerous bond failures in IC  devices, often exacerbated by contamination from preceding  processes.


Figure 5: SFM image of a nanoindentation on an aluminum  bond pad (a) from which the roughness can be calculated and  correlated to ease-of-bonding. A sectioned ball bond is shown  in (b) with a line of nanoindentations through the Si substrate, Al coating and Au ball. A hardness comparison between the  pad and the gold ball, neck and wire is shown in (c).


0 500 1000 1500 2000 2500 3000 3500 4000


5


Indentation number Ball


Neck


Wire


Ball


Figure 6: Line of 4 nanoindentations (max load 5 mN) along a  bonding pad connector (a) which is coated with a diamondlike protective coating. Zoomed image of the tested connector


(b) and corresponding load-depth curve and calculated  coating hardness/modulus values (c).


The purpose of these experiments was to try to fabricate good  vias of moderately high aspect ratio to understand their  contribution to total interconnect resistance. Since voids will  clearly decrease conductivity, we targeted the fabrication for  good fill factors in all cases rather than allow poorly filled vias  that would not be amenable to circuit edits. We focused on the  compositions of the vias and the resistance in an effort to  understand how they would impact circuit editing decisions at  the 90 nm Cu node and beyond.


In these experiments, we used an FEI VectraVision FIB to  create vias in test wafers for analysis. The test wafers, made in  the Avago IC wafer fab in Fort Collins, comprised 2.5 µm of  SiO2 on top of 2.5 µm of Al on a Si wafer substrate. Two  square holes between 0.25 µm and 1.25 µm (depending on the  desired aspect ratio) were etched with a 23 to 121 pA Ga+ beam enhanced with XeF2 through the SiO2 layer to make  contact with the Al. The separation between the two holes was  fixed to 100 µm. The via holes were filled with W using a 13  pA beam, and a 50x50 µm W pad was deposited onto each  via. Fig. 2 is a structural representation of the circuit and via  geometry. A microprobe station (used in both 4-point and 2-point modes) with an Agilent 4156C Parametric Analyzer and  a Keithley 2602 Sourcemeter was used to measure the  resistances of the vias.  The measured resistance includes  contributions from the W pads, the W vias, and the Al layer. The contribution of the Al sheet to the total resistance was  measured to be ~5 Ω as determined by transmission line  methodology and was subtracted from the data [6].


Figure 2: Structural presentation of via measurement  geometry.


By making W pads 3 microns thick and by varying the  positions of the probe tips on the W pads, we determined that  the W pad resistance was negligible. A comparison of 2-point  and 4-point modes proved that contact resistance to the pads  was small and ignorable to within the accuracy of the  experiments. Due to the length of time necessary to make W  pads and the difficulty of probing them with W probe tips, we  initiated a second round of experiments with a new wafer


design. This wafer comprised a 5.5µm SiO2 layer sandwiched  between two 2.5 µm Al layers. We created W vias in the SiO2  between the two Al layers, and cut Al pads surrounding the  vias, to isolated them and allow for measurement of the via  resistance.


Measuring the resistances of the vias is challenging. The small  vias (~1 µm2) made in these experiments cannot carry much  current. To determine the maximum current density a W via  could carry, we used a light bulb filament, measured the  filament diameter, and ramped the current in air until it failed. We determined that the maximum current density a 50 µm  diameter W wire could carry in air is ~20 µA/µm2. Even  though this maximum current density is less than reported  values, we found experimentally that the Al/SiO2/Al wafer had  poor reliability and would fail if we exceeded this value, but  that the SiO2/Al wafer with W pads could handle ~104 µA/µm2  [2,3]. Typical measurement parameters for a 1 µm2  via were ~10 µA of forced current and, assuming ρ = 2.5 Ω-µm and a length of 2.5 µm, a resistance of about 6 Ω and a  voltage drop of  ~100 µV.


The VectraVision FIB used W(CO)6 to make conductive W  lines and vias. The usual deposition rate for W on a flat  surface in our FIB is 0.17±0.01 µm/(nC/µm2), independent of  beam current. For example, with a 23 pA beam, a pixel  spacing of 0.03 µm, and a dwell time of 0.5 µs, our system  deposits a dose of 1 nC/µm2 over an area 1 x 2 µm in 3.5  minutes to make a W jumper 0.17 µm thick. We have never  measured a deviation from this rate for W deposited on a flat  surface, although we have noticed that vias fill much faster  than 0.17 µm per nC/µm2. The typically measured  stoichiometry of our W metal is 65 at. % W, 8 at. % Ga, 5 at. % O, and 22 at. % C as determined with a Quantum 2000  Electron Spectroscopy for Chemical Analysis (ESCA) system [1,3,5]. The resistivity of jumpers drawn on a SiO2 surface  measured 250 µΩ-cm, in good agreement with the accepted  value [1,3,5]. Pure W has a resistivity of 5.3 µΩ-cm [7].


We used a Hitachi 4700 SEM equipped with a Noran Vantage  energy dispersive spectrometer (EDS) to look at the vias in  cross-section, to estimate the degree of voiding, and to  measure the average via material composition. In all cases, we  deposited W slowly in the vias using a 13 pA Ga+ beam in an  effort to avoid voiding since we were interested in good via  contacts, not a study of via voids against deposition  conditions.


We augmented the EDS compositional data with Auger  electron spectroscopy (AES) data from a Phi 680 Scanning  Auger Microscope to avoid uncertainties in the EDS excitation  volume and overlap between the Si K and W M lines. The Phi  680 has SEM imaging capabilities with ~10 nm spatial  resolution and compositional accuracy of several atomic  percent. After making test vias along the edge of a piece of the  test wafers, we used the Ga+ beam in the VectraVision to slice  down the middle of the vias. We sputtered lightly (2 nm) in  the Phi 680 to remove surface contamination from transport in  air, using a low sputter voltage (2kV) to avoid preferential  sputtering of C atoms over W atoms, and then made  compositional measurements on the cross-sections.


Figure 3: Three vias, each filled with W at a dose of 1  nC/µm2.


Fig. 3 is a SEM cross-section of W deposited at 1 nC/µm2 on


the SiO2 surface (far left), and three vias each filled with a  dose of 1 nC/µm2 of W. The SEM image was taken  perpendicularly to the cross section to insure a true image of  the aspect ratio.


The specific parameters used in all cases were a 13 pA beam, a pixel spacing of 0.026 µm, a dwell time of 0.5 µs, and a dose  of 1 nC/µm2. The deposition rate is 0.18 µm per (nC/µm2) on  the surface (far left) as expected for our FIB system. For the  same 1 nC/µm2 dose, the W at the bottom of the 2.5 µm via is  already to 0.25 µm thick, evidencing an increase in the W  deposition rate at the bottom of the via from 0.17 to 0.25 µm  per nC/µm2. The 1.25 µm via has already filled to 1.4 µm for  the same 1 nC/µm2 dose, and the 0.5 µm via has filled to 2.1 µm.


Converting the deposition rate of 0.17 µm per nC/µm2 into W  atoms per Ga+ ion, we determine that each Ga+ ion results in


1.1 atoms of W in a surface film, a value less than the 3.5 W  atoms per incident Ga+ ion reported in the literature [3]. The


0.5 µm via shows a twelve-fold increase in the conversion  rate, from 1.1 to 12.3 W atoms per incident Ga+ ion. This data  clearly shows that the via fill rate is a strong function of the  via geometry, that high aspect ratio vias fill faster than low  aspect ratio vias, and that the deposition rate in a via can be an  order of magnitude higher than the deposition rate on a flat  surface for identical beam conditions.


A model to understand the observed increase in deposition rate  in a via compared to a flat surface invokes an increase in the  effective precursor-to-beam ratio in a via. The W(CO)6  precursor must line both the walls and the bottom of the via. The 1.25 µm via, for instance, has ~11.5 µm2 of surface area  along the walls and 1.5 µm2 surface area on the bottom. The  incoming Ga+ ions see approximately eight times (11.5/1.5) the number of precursor molecules in the via than on a flat  surface of the same area, manifested as an increase in the  effective gas-to-beam ratio. This model works well for rough  surfaces.


An alternative model for understanding the enhanced  deposition rate begins with the assumption that the vias  behave like Faraday cups, capturing the Ga+ ions that would  otherwise have backscattered into the vacuum. The captured  Ga+ backscattered ions would then collide with and crack  other W(CO)6 molecules in the Faraday cup, increasing  deposition rate to more than 1.1 W atoms per incident Ga+ ion. Ga+ ions that strike W(CO) 6 precursor molecules on one of  the walls may scatter to the bottom with sufficient energy to  decomposition precursor molecules along the base. Similarly, Ga+ ions that backscatter off of the bottom may strike one of  the walls with sufficient energy for precursor decomposition.


Figure 4: SEM image of three test vias.


In all three vias shown in Fig. 3, we completed the W  deposition by decreasing the size of the deposition box by ~20% from the size of the etching box. For instance, we made  the 1.25 µm via by etching a 1.25 x 1.25 µm area, but we  filled by depositing over a 1.0 x 1.0 µm area. The deposition  along the walls must result from Ga+ ions that have already  scattered off the bottom of the via. The extra deposition along  the via bottom compared to a flat surface may be from Ga+ ions that have scattered a second time off the via walls.


These two models, 1) the effective precursor-to-beam model  and 2) the Faraday cup model, are not different but really just  two ways of viewing the same phenomenon. The effect of the


via is to concentrate the precursor and the beam energy to  increase the conversion of W(CO)6 precursor to W metal.


Fig. 4 shows a SEM cross section of three vias made in close  proximity to study the composition of the W in vias as a  function of via geometry. The SEM image was taken  perpendicularly to the cross section to insure a true image of  the aspect ratio. The drawn widths of the vias are 1.0 µm, 0.75 µm, and 0.5 µm, with corresponding aspect ratios (length to  area) of 2.3, 4.0, and 9.2. The specific parameters used in all  cases were a 13 pA beam, a pixel spacing of 0.026 µm, and a  dwell time of 0.5 µs. The dose given to each via was the  amount necessary to fill it with W. All three vias are larger (~0.1 µm) on the top and smaller (~0.1µm) at the base than  drawn. The vias end on the Al sheet layer. The nominal 1.0 µm via has a void at the bottom near the Al layer but the  others have good fill factors. The other vias do not have any  visible voids and have good fill factors.


Table 1 lists EDS measurements of the compositions at the  midpoint of each via. The reported composition for W  deposited on a flat surface is W = 75 at. %, C = 10 at. %, Ga = 10 at. %, and O = 5 at. % [1]. Two striking observations from  the EDS data are 1) the C is larger than the expected value, and 2) the Ga is only one-tenth of the expected value.


Via Position W C Ga O


0.5 µm


center


26


0.75 µm


67


28


1.0 µm


Table 1: EDS measurements of via compositions in at. %.


We turned to AES to measure the composition with better  spatial resolution than possible from the excitation volume of  EDS. Fig. 5 shows an AES spectrum of a W film to  demonstrate the quality of the data. The W, Ga, C, and O  peaks are labeled in Fig. 5. AES detected no elements other  than those four with their obvious sources.


1500


2000


Kinetic Energy (eV)


W W


W


WW


O


GaGa


Ga Ga


Figure 5: Auger spectrum of FIB-deposited W


Table 2 shows the compositions of flat surface W pads (bottom two rows) along with each of the three vias shown in  Fig. 4 taken from the AES spectra. “Bottom” and “top” refer  to the bottom of the via near the Al layer and the top near the  SiO2/vacuum interface. The average compositions in the vias  are consistent with those Table 1, but different from the  compositions of W deposited on a flat surface. In particular, the Ga composition at the bottom of the via is only one-tenth  the value in flat-surface W. The Ga content in the vias tends to  increase near the top of the vias, consistent with a transition to  surface-like deposition process. The C composition is also ~ 4  at. % higher in the vias than on flat surfaces.


bottom


73 23 1


top


68 28 4


70 27 1


66 29 3


73 24 1


71 23 5


Average NA 70 26 3 2


13 pA beam flat surface 65 21 13


1.7 nA beam flat surface 66 23 8


Table 2: Auger measurements of via compositions, in at. %.


Since the C to O ratio is not unity but rather near 10, most of


the (CO)- radicals that do not escape the growing tungsten  layer crack under the Ga+ beam. One can explain the C  increase with the Faraday cup model, postulating that C has  some difficulty escaping from the via relative to a flat surface. The same might be true about the O, but we did not have the  signal-to-noise resolution in the AES data to measure a  difference in O composition between a flat surface and a via.


The effective precursor-to-beam model and Faraday cup


model explain the decrease in Ga seen in the vias. The Ga+


ions interact with more W(CO)6 precursor molecules, resulting  in more W atoms per incident Ga+ ion than the surface value  of 1.1, causing the W to Ga ratio to increase. The C and O


atoms do not escape as readily from a via as from a flat


surface, so for each W(CO)6 precursor molecule that


decomposes, more C and O atoms will remain to make the W  film richer in C and O. Combining the Auger data with a


philosophy adhering to Occam's razor, one could conclude


that the main difference between a via and a surface is that all  atoms have more trouble escaping from a via than a surface.


The trapped Ga+ ions deposit their energy more efficiently,


and the W, C and O are not free to escape into the vacuum.


0 5 10 15 20 25


Resistance Versus Drawn Geometry


Via Length/Area (1/um)R = L/A


R = L/Aeff


R = L/A +      /Aconc


ρ


ρ ρ


Figure 6: Via resistance versus via length/area.


Starting with the equation R = ρ*L/A, where L is the length  and A is the drawn area, one should be able to make a straight  line by plotting R versus the quotient L/A. Fig. 6 shows such a  plot. The black-dotted line is this classical model using ρ = 250 µΩ-cm (or 2.5 Ω-µm), the resistivity of W deposited on a  flat surface. The data from the 2.5 µm thick SiO2 layer is  shown as “+” and “■”. The data from the 5.0 µm thick SiO2  layer is shown as “x”.


The empirical data shows that the resistivity of the FIB via W  curves upwards away from the classical model, but less far  less than anticipated from the Pt via data of Reference [4]. We  have conjured two models that fit the data well. The first is an  effective area model that adds one piece of physics with one  free parameter – the perimeter immediately inside the drawn  via area does not participate in conduction. The idea is that the  via sidewalls are coated with a material such as an oxide or  silicide that causes the perimeter of the via along the SiO2 not  to conduct electrons [10]. The second is a contact resistance  model following the work of Chen et al. with two free  parameters – the contact resistance between the W and the Al  dominates the total resistance for high aspect ratio vias [11,12].


In the effective area model, the resistance of the via becomes  R = ρL/Aeff,


where


Aeff = (w – 2∆)2,


and ∆ is the thickness of the dead perimeter of the via and w = √A is the square root of the drawn area A. Note that ∆ is  independent of A in the model. The dot-dashed curve is a fit to  the data where the resistivity is locked to 2.5 Ω-µm (the flatsurface value), and only ∆ is free to vary. A least squares fit  determines that ∆ = 0.12 µm.


In the contact resistance model, the total resistance of the via  comprises two components, 1) a bulk component given by


Rbulk = ρ*L/A,


and 2) a contact resistance term at the W/Al interface given by


Rcon = ρc/Acon,


where ρc is the specific contact resistance and Acon is the area  of contact between the W and the Al [10]. The contact area is  given by


Acon = (w – 2∆)2,


where ∆ is the amount of taper to each sidewall of the via and  w = √A is the square root of the drawn area. Fig. 4 shows that  the 0.75 µm and 0.5 µm vias taper ~ 0.13 µm to 0.64 µm and


0.35 µm at the W/Al, giving an estimate of 2∆ = 0.13 µm.


Estimates for ρc comes from Chen et al. who quote ρc = 2 Ω-


µm2 for clean metal-to-metal contacts and Demarco et al. who  quote ρc = 0.2 Ω-µm2 for W contacts to Si. The long-dashed


curve is a fit to the total resistance R = Rbulk + Rcon with ρ


locked to 2.5 Ω-µm (the flat surface value), ρc = 8.9 Ω-µm2,


and ∆ = 0.11 µm. The value of ∆ is higher than our estimate, and the value of ρc = 8.9 Ω-µm2 is higher than expected but


possible since 1) ρc increases sharply with decreasing area,


and 2) ρc depends critically on interface quality [10,11,12].


Domengès et al. attributed the increased resistance of vias  over the expected model to contact resistance. Our resistance  increase does not stem from contact resistance as we explicitly  verified with 4-point probe and by 2-point probe on W pads. We have modeled our increase in resistance with two distinct  models: 1) the effective area model, and 2) the contact  resistance model. Note that the two models have very similar  functional forms. The effective area model invokes a materials  effect along the via sidewalls that precludes electronic  conduction. The contact resistance model invokes a contact  resistance between the W and the Al, and a tapered shape to  the via that decreases the contact area from the drawn area. We include both models here because both may be at work  and we do not have the data to discern them.


Could other models explain the increased resistance of vias? The short answer is “yes”. Assuming that ρ ~ (L/A), for  instance, would lead to a quadratic fit in Fig. 6. Could the


measurably different compositions in the vias support this  assumption? The answer here is “no”. Sputter-deposited  tungsten-carbide (WC1-x) has a measured resistivity of ρ = 200-300 µΩ-cm, in good agreement with our value of 250 µΩcm on flat surfaces and vias [9]. This agreement prevents an  assumption that the resistivity increases with C composition in  the vias. Graphite has a resistivity of ~8000 µΩ-cm and could  lead to an increase in resistance, but graphite inclusions are  hard to believe in light of the SEM images. Furthermore, the  decrease in Ga content in the vias should lead to a decrease is  resistivity, not an increase. We are left to conclude that a  decreased via sidewall conductivity or W/Al contact area  dominate bulk compositional effects and lead to an increase in  via resistance from a simple, classical resistivity model.


Finally, is ∆ = 0.11 ~ 0.12 µm valid for all vias? Again, the  answer is “no”. We have preliminary data to show that ∆ is a  function of the beam and gas parameters whether one  interprets it as a dead sidewall or a decreased contact area. The  message in Fig. 6 is that the net area is less than the drawn  area, and that high-aspect ratio vias will have more resistance  than the classical model predicts.


Acknowledgment


The authors would like to thank David Leary of Avago  Technologies for his support of the Failure Analysis  Laboratory and this work.


1. Gianuzzi, L. and Stevie, F., Introduction to Focused


Ion Beams, Springer (2005).


2. Zaragoza, M. “Reliability Test Results for W FIB  interconnect Structures”, Integrated Reliability  Workshop Final Report, IEEE International (1999), pp. 14-19.


3. Langfischer, H., Basnar, B., Hutler, H., Bertagnolli, “Evolution of tungsten film deposition induced by  focused ion beam,” J. Vac. Sci. Technol. A20(4), Jul/Aug 2002, pp. 1408-1415.


4. Domengès, B. and Poirier. P., “Quantitative electrical  analysis of FIB prepared vias on BiCMOS and  CMOS090 designs”, Conf. Proc. from the 32nd  International Symposium for Test and Failure  Analysis (2006), pp. 67-70.


5. Orloff, J., Swanson, L., and Utlaut, M., High


Resolution Focused Ion Beams: FIB and


Applications, Kluwer Academic/Plenum Publishers (2003).


6. Iliadis, A.A., Andronescu, S.N., Talyansky, V., Edinger, K., Orloff, J.H., Woods, M.C., and Jones, K.A., Compound Semiconductors, IEEE  International Symp, 353 (1997).


7. Lide, D.R., Eds., Handbook of Chemistry and


Physics, 77th Edition, (1996-1997), pg. 12-42.


8. Ray, V., Antoniou, N., Bassom, N., Krechmer, A., and Saxonis, A., J. Vac. Sci. Technol. B21(6), (2003), pp 2715-2719.


9. Liao, M., Koide, Y., and Alvarez, J., J. Vac. Sci. Technol. B24(1), (2006), pp. 185-189.


10. Demarco, A.J., Melngailis, J., J. Vac. Sci. Technol. B


19(6), (2001), pp. 2543-2546.


11. Chen, K.N., Fan, A., Tan, C.S., and Reif, R., Electron  Device Letters 25(1), (2004), pp. 10-12.


12. Chen, K. N., Fan, A., Tan, C.S., and Reif, R., Appl. Phys. Lett. 86(1), (2005),  pp. 11903-1-3.


DOI: 10.1361/cp2008istfa141


Backside Circuit Edit on Full-Thickness Silicon Devices


Chad Rue


FEI Company, Hillsboro, OR, USA


Steven Herschbein and Carmelo Scrudato


IBM Corporation, Hopewell Jct., NY, USA


Circuit Edit (CE) is a widely-established technique employed  by semiconductor manufacturers. CE reduces Integrated  Circuit (IC) development costs by reducing the number of  mask sets that are required during the design-debug phase, and speeds overall time-to-market.


Most CE activities are performed with Focused Ion Beam (FIB) tools, which have evolved considerably over the years  to meet the needs of the CE market. One of the most  significant technique developments that has pushed the  evolution of FIB hardware is the advent of backside CE  techniques, [1,2,3] in which the FIB operator accesses the  critical circuitry through the backside (substrate side) of the  IC device. This approach is the overwhelming preference for  processor manufacturers in particular, due to the unique  constraints of these devices. For example, FlipChip and BGA  style packages naturally lend themselves to a backside  approach. Additionally, these devices tend to have extremely  dense circuitry and an abundance of “dummy” metallization  structures that impede frontside access.


Backside CE usually requires a considerable amount of  preparation prior to the actual FIB edit.[4,5] If the device is  covered with a heat-spreader, it must be removed to access the  silicon. The substrate silicon is then thinned to somewhere  between 30 and 150 μm of remaining silicon, depending on  the nature of the FIB that will be used for the edit. This limits  the time that must be spent “trenching” (milling with the ion  beam) through the substrate silicon. Next, the silicon surface  is carefully polished to a mirror-smooth finish. This ensures  IR transparency, which is important for navigational purposes  during the FIB edit. Finally, some labs perform a final  chemical etching step using laser-based tools, to locally thin  the silicon even further (to around 10 μm of remaining  silicon) over the sites of interest. [6,7]


The sample preparation required for a typical backside edit is  a significant barrier for some labs, as it requires specific  hardware and considerable operator expertise. Additionally, the process is time-consuming and occasionally fatal to IC  devices. Finally, even with the proper hardware and operator  know-how, there are instances in which it is not possible to  mechanically thin the silicon in the typical fashion. For  example, some modern IC devices are packaged on flexible  plastic substrates. These package types tend to warp the  silicon die, and corner-to-center height differences over 100


μm are occasionally observed. [8,9] The die distortion leads to  strain, which can cause cracks and fractures in the silicon  during mechanical grinding and polishing.


All of these limitations lead to the following questions: Can  backside CE be performed on full-thickness silicon devices? Is it possible to skip the global thinning step? What are the  advantages and disadvantages of this approach?


In this paper we will explore these questions. Sample trenches  will be shown, and trenching optimization experiments are  described. We will address the issues of navigation, including  IR imaging through full-thickness silicon, and how it depends  on the sample doping levels. Finally, we will present data on a  new navigational technique that can be employed to improve  targeting accuracy.


Use Cases. There are several situations in which the FIB  operator may wish to skip the global thinning step. The most  common example is when the silicon substrate is distorted, as  depicted in Figure 1.


Figure 1: This graph illustrates height differences (in  micrometers) in the silicon of a BGA-style device. The Z-axis  has been greatly exaggerated.


The “pin-cushioning” distortion shown in Figure 1 is common  in modern flip-chip plastic ball grid array (FC-PBGA) packages. These distortions arise due to differences in the  coefficients of thermal expansion of the various materials in  the package. Corner-to-center height variations in excess of  100 μm have been observed, resulting in significant stress on  the silicon. When the operator attempts to globally thin  devices under stress, they may fracture. In such cases, a fullthickness approach may be the only option.


In other cases, the act of globally thinning the silicon may  alter key characteristics of the sample. In a recent example, an  analysis was being performed on a device with suspected  delamination problems. Mechanical polishing would almost  certainly have perturbed the delamination phenomenon, and  the analysis would have been inconclusive. Instead, the fullthickness device was loaded into the FIB, and trenching was  performed to remove the silicon over one of the suspected  delamination sites. Once the substrate had been removed, the  delamination phenomenon could be examined with an optical  microscope.


Figure 2a: Top-down FIB view of a full-thickness device in  which all of the substrate silicon has been removed by FIB  trenching.


Figure 2b: The corresponding optical image of the sample. Delamination artifacts are clearly visible after the substrate  silicon was removed with the FIB.


Finally, globally-thinned devices are thermally and  mechanically fragile compared to their full-thickness  counterparts. They may be too weak to tolerate mechanical  socketing for electrical testing, and they may not be able to  dissipate heat as effectively. Both scenarios may destroy the  device during electrical testing.


Figure 3: Electrical testing on devices with thinned silicon  can result in heat build-up and catastrophic failure.


The mechanical and thermal limitations of devices with  thinned silicon can often be overcome by rebuilding the  package prior to electrical testing. [10] When this is not  possible, it may be a preferable to leave the silicon thick.


Finally, a significant amount of hardware and operator  expertise is needed to successfully thin devices. If a robust  methodology can be developed for full-thickness backside CE, then some FIB labs may want to reconsider their work flow, and weigh the pros and cons of the full-thickness approach.


IR imaging. When a sample is initially loaded into the FIB  tool, IR microscopy is used to image the circuitry through the  silicon, in order to locate the region of interest. Typically, thinner silicon results in a better IR image, which is one of the  primary reasons the die is thinned prior to backside CE. However, it is not always necessary to have thin silicon to  obtain a suitable IR image. The images depicted in Figure 4  were obtained with a high-performance IR microscope (VDS  Vosskühler, GmbH) and a standard broadband microscope  illumination source (Olympus Corporation, Japan).


Figure 4a: IR image of the surface of a 550 μm thick silicon  sample. Note the visible scratches in this image, which has a  horizontal field width of 96 μm.


Figure 4b: Corresponding IR image of the circuitry, viewed  through 550 μm of silicon.


Note that despite a poor surface quality (Figure 4a), the IR  image is quite clear, even though the silicon is very thick in  this case (about 550 μm).


Another example is shown in Figure 5. The initial image  obtained through full-thickness silicon (about 770 μm) is  adequate for coarse navigation. However, the image quality is  considerably better when the silicon is thinner.


Figure 5a: IR image of circuitry through about 770 μm of  silicon.


Figure 5b: IR image of circuitry through about 10 μm of  silicon.


In addition, the quality of the IR image depends on the amount  of doping in the silicon. Very heavily doped-substrates absorb  more IR light, and result in poorer images. Users may wish to  experiment with their devices to see what thickness of  remaining silicon yields acceptable optical imaging.


Figure 6: IR view of a corner fiducial (left), and the  corresponding top-surface FIB mark (right).


Figure 7a: IR view of an edit target location, viewed through  550 μm of silicon.


Figure 7b: The same view, but with CAD overlay.


Coarse Navigation. The initial navigational step in a fullthickness backside CE is similar to that typically performed in  conventional backside CE: the IR microscope is used to view  through the silicon and locate features in the corners of the  die. For convenience, FIB marks can be placed on the topsurface of the silicon (directly over the location of the lock  points), so that subsequent relocking can be done quickly in  the FIB, as shown in Figure 6.


After performing the coarse 3-point lock, the stage is driven to  the approximate location of the target site. Figure 7 shows an  IR image of a target area, viewed through 550 μm of silicon, and the corresponding image with CAD overlay.


Note again, that a great deal of circuitry structure is visible  through the thick silicon. However, some devices with higher  doping levels pose a greater challenge. We recently examined  a processor device that was thinned to 100 μm and carefully  polished. Because the silicon was heavily doped, the resulting  visibility was poorer than the images shown in Figures 4-7. In  extreme cases, the optical image may not be good enough for  coarse navigation.


Trenching. Once the approximate location of the target is  located, the silicon must be removed. Trenching through  several hundred microns of silicon requires specialized gasdelivery hardware. In these experiments, we utilized a  standard FEI Gas-Injection System (GIS) canister containing  XeF2.  The addition of XeF2 increases the rate of silicon  removal,[11] because of the following chemical reaction:


(1) 2XeF2(g) + Si(s) → SiF4(g) + Xe(g)


The standard delivery needle was replaced with a co-axial  style needle which optimizes gas delivery by providing better  gas flow symmetry and higher gas flux to the sample surface.


Figure 8: Cross-sectional view of the coaxial gas nozzle used  in these studies. Note that the central vertical bore is wider at  the bottom of the nozzle than at the top. This design  concentrates the gas flux at the sample surface.


In addition to specialized gas-injection hardware, other factors  can also affect trenching results on full-thickness devices. For  example, milling rates are maximized by the following  conditions:


A. Higher beam currents


B. Higher XeF2 gas pressures


C. Lower nozzle heights


D. Shorter loop times


Factors A and B are obvious to experienced operators, but  factors C and D may not be so obvious. Factor C, lowering the  nozzle height, results in higher local pressures at the sample  surface for a given gas flow rate. Nozzle height can have a  marked impact on the milling speed, as depicted in Figure 9  below.


5.0E+04


1.0E+05


1.5E+05


2.0E+05


150


Height of Nozzle Above Sample (um)


Figure 9: XeF2-assisted silicon removal rates for a 100x100 μm pattern, performed with a beam current of 21 nA, as a  function of nozzle height.


Pattern loop time is defined as the period of time before the  beam repeats a scan of a milling pattern. Loop time increases  as dwell time increases and as pixel spacing decreases. Longer  loop times result in more ion dose per raster. During gasassisted processes, longer loop times are more likely to have  gas depletion problems. That is, the adsorbed gas precursor  molecules may be consumed before the end of an individual  pixel event. This reduces the chemical component and  increases the sputtering component of the FIB mill, resulting  in a loss of efficiency and/or selectivity. This phenomenon is  illustrated in Figure 10.


Note that as the loop time increases, the silicon removal rate  decreases. This indicates that longer loop times are suffering  from gas-depletion, and that too much time is spent  performing straight sputtering under those conditions. By  contrast, shorter loop times spread the beam out over more  area per unit time, allowing dissociation of the XeF2


molecules without gas depletion. In this way, the chemistry is  allowed to do most of the work.


1.3E+05


1.4E+05


1.6E+05


1.7E+05


1.8E+05


1.9E+05


100 200 300 400 500 600


Pattern Loop Time (ms)


Figure 10: XeF2-assisted silicon removal rates for a 100x100 μm pattern, performed with a beam current of 21 nA, as a  function of pattern loop time.


By carefully controlling the above-mentioned factors, it is  possible to trench through thick silicon substrates in a  reasonable amount of time. The trench illustrated in Figure 11  was milled through 550 μm of silicon.


Figure 11: FIB view of a circular trench milled through 550 μm of silicon. The diameter of the milling pattern was 200 μm. Endpoint was achieved after 44 minutes of milling time. The  sample was imaged with a slight stage tile (21˚) to give a  sense of the aspect ratio.


This trench took approximately 44 minutes of milling time, and was performed with the following conditions: Beam  current = 21 nA, ion energy = 30 keV, dwell time = 200 ns, pixel overlap = -25%, refresh time = 0, XeF2 pressure (as  measured by the primary chamber gauge) = 1.2e-5 Torr.


Two more examples of trenches milled through thick silicon  devices are shown in Figures 12 and 13.


Figure 12: Top-down FIB view of a trench milled through  about 770 μm of silicon. This mill took approximately 70  minutes of milling time with 21 nA of beam current.


Figure 13: FIB view of a square trench milled through 550 μm of silicon. The sample was imaged with a slight stage tile (25˚) to give a sense of the aspect ratio.


The trench shown in Figure 13 is significant, because we were  able to use visual endpoint detection techniques during the


trenching process by viewing the outline of the active  diffusion wells in the live milling image. This technique is  often used in backside CE, but it is considerably more difficult  to detect on full-thickness trenches (where the aspect ratio is  higher and specialized gas nozzles must be used). Nevertheless, this result is encouraging and suggests that it is  possible to use this common endpointing technique on some  full-thickness backside edits.


Figure 14a: Top-down view of the trench shown in Figure 13. Note the visible details of the active wells in the bottom half of  the trench.


Figure 14b: The diffusion wells of the active circuitry have  been exposed, which provides a visible endpoint signal (this  image has been contrast-enhanced)


Local Navigation. Because of the long trenching times  required for a full-thickness backside CE, it is not practical to  physically expose the corner fiducials with individual  trenches. However, as described above, IR microscopy can be  used to coarsely locate the primary trench over the edit site.


Prior to attempting a critical edit, it is necessary to perform a  more precise local stage lock. We present here a new  technique that allows high navigational accuracy using  features found locally in the bottom of the edit trench.


First, the IR image is used to locate a number of features  within the trench that will serve as local alignment points.


Figure 15a: FIB view of a coarse trench, with CAD overlay. The circles mark areas that will be used for local alignment.


Figure 15b: IR image of one of the local alignment features.


As few as one local alignment point will work, but three  points are preferred. After locating the local alignment points  with the IR microscope, the features are physically exposed  using the ion beam. The CAD overlay is then applied to a FIB  image that simultaneously encompasses both the target site  and the local alignment point (or points). For the example  shown in Figure 16, a horizontal field width of 179 μm was  chosen.


Figure 16: FIB image of a coarse trench with CAD overlay. Three small mills have been performed to physically expose  features that will be used for a local alignment.


At this point in a typical backside edit, a simple one-point  correction is used to shift the CAD information to obtain a  better overlay to the FIB image. However, a careful analysis  of different parts of the FIB field-of-view may reveal that a  simple one-point correction is inadequate. In Figure 17, digital  magnification is used to illustrate the discrepancies between  the FIB image and the CAD overlay.


Note that each of the three regions has a slightly different  offset error. These different errors can arise from many  sources: operator error in the original stage lock, imprecise  calibration of the FIB image (magnification and/or rotation), local die distortions, or non-linearities in the ion column  deflection system, to name a few. Whatever the source of the  errors, it is usually impossible to achieve perfect  correspondence between a CAD overlay and every point  within a large field-of-view FIB image. Ultimately, these  errors can limit the accuracy of the final navigational step.


Figure 17: Digital magnification is used to illustrate CAD  overlay errors. Note that errors may be slightly different in  different parts of the field-of-view.


One solution to this problem is to perform a 3-point reregistration that stretches, shifts, and/or rotates the CAD  overlay to create a customized match of a particular FIB  image. Note that this is different from the original 3-point  global stage lock that was performed at the beginning of the  edit. The original 3-point global stage lock is a rather coarse  alignment, whereas the 3-point re-registration is a local  adjustment that is superimposed on the global lock to refine  the accuracy of the overlay.


Figure 18: The user identifies local offsets (3 in this image) which will be used to re-register the CAD overlay. The black  crosses mark visible features in the FIB image, and the white  crosses mark the corresponding polygon in the CAD overlay.


Using digital magnification, the user can zoom-in on the FIB  image and CAD overlay and specify a local offset for various  regions within the image. Figure 18 illustrates how the local  offsets could be defined for three regions in our example.


After the 3 local offsets are defined, the CAD overlay is  stretched, rotated and/or shifted to create a perfect match to  the FIB image, as depicted in Figure 19.


Figure 19: After performing the 3-point re-registration, the  CAD overlay is a much better match to the FIB image.


Digital magnification can also be used to position the milling  pattern over the target region, as depicted in Figure 20.


Figure 20: Digital magnification is used to accurately  position milling patterns after the 3-point re-registration.


Because the milling patterns are placed according to the  custom-stretched CAD overlay, their positional accuracy will


be better than what would be achieved from a single reference  point. Figure 21 illustrates the accuracy of a typical targeting  event using this technique.


Figure 21: Typical targeting result using the 3-point reregistration technique. In this case, the observed beamplacement error was 33 nm. The FIB image used for the  targeting event had a horizontal field width of 179 μm.


The white pattern (labeled #2 in the image) marks the  expected location of the target (a tungsten contact), based on  the 3-point re-registration technique. The actual, observed  position of the contact was 33 nm away from the expected  position. Recall that the FIB image that was used for this  targeting event had a horizontal field width of 179 μm.


Another advantage of this technique is that it is extremely  non-invasive. The process can be performed with a single  high-resolution, low-magnification FIB image, and does not  require the user to go to live milling to navigate to lock points. Other Considerations. After the target has been located, the  process for completing the edit is similar to traditional  backside CE. However, some unique factors should be  considered.


First, secondary electron intensity in the bottom of a fullthickness trench is considerably lower than in standard  backside trenches. Therefore, the usual techniques that are  employed to boost S/N (such as reducing the aspect ratio of  small access holes by using overlapping milling patterns) become even more critical. Visual endpointing may be less  reliable, and other endpointing techniques (such as stagecurrent measurement) may be useful.


Second, gas depletion effects can be a problem at the bottom  of full-thickness trenches. Gas-assisted etching processes  seem to work fairly well, but depositions can be more  difficult. It is often necessary to reduce the beam current


and/or increase the refresh time, in order to avoid milling  instead of depositing. Patience is required.


Third, the large difference in Z height between the top-surface  of the silicon and the bottom of the trench requires some  adjustments to the FIB hardware. For example, users typically  set the top-surface of the silicon to a pre-determined “eucentric” height before beginning an edit. However, on a  full-thickness sample this means that the eventual bottom of  the backside trench will be considerably lower than this ideal  height. The position of gas nozzles may be ill-suited to  working at the bottom of the trench. Additionally, the travel  range of the IR microscope may not be large enough to image  the bottom of the trench. To overcome these challenges, users  may wish to position the sample slightly above the normal “eucentric” position prior to beginning the edit.


Fourth, some edits are simply not feasible with full-thickness  substrates. For example, FIB users are occasionally asked to  bring probe pads up to the top surface of the backside silicon. This type of request is challenging even on traditional  backside samples (which usually have less than 100 μm of  silicon remaining). Performing this task on a full-thickness  trench (which is several times deeper and likely to have more  textured sidewalls), is probably not worth it. Electrical  probing is also sometimes performed at the bottom of  trenches. In such cases, users will need to carefully consider  the size requirements of the probing hardware, before  committing to a full-thickness approach.


Fifth, trench planarity and milling speed are sometimes at  odds with each other. For example, under extremely gasenhanced conditions, the material removal rate is maximized, but trench floors are often rounded, with the center deeper  than the edges. Conversely, when a trenching process is gasdepleted, it is common to observe that the edges are deeper  than the center. Figures 22a and 22b illustrate this  phenomenon.


Because speed is an important consideration in full-thickness  trenching, Silicon-on-Insulator (SOI) substrates are ideal  candidates for the full-thickness approach, [12] because they  tend to be self-planarizing. For example, the FIB operator can  proceed at maximum milling speeds until the buried oxide is  exposed. The beam is then switched off, but the XeF2 gas is  allowed to continue flowing over the sample. The remaining  silicon will be gradually attacked by the spontaneous nature of  reaction (1), and the bottom of the trench will widen, increasing the surface area of the work site without eroding  the buried oxide.


Finally, users should consider the economic tradeoffs of the  full-thickness approach. FIB tools are expensive, and FIB time  is valuable, whereas conventional thinning and polishing  equipment is relatively cheap. It may not always make good  economic sense to use FIB tools to perform long trenching  tasks. As always, the benefits and liabilities of the fullthickness approach should be analyzed against the “bigpicture” of a particular task. The technique may not be the


best solution in all cases, but it can be a useful tool to extend  the total capabilities of a FIB lab.


Figure 22a: A backside trench performed under gas-enhanced  conditions (beam current = 21 nA, pattern size = 100x100 μm, loop time = 5.1 msec). Note that the center is deeper than  the edges.


Figure 22b: A backside trench performed under gas-depleted  conditions (beam current = 21 nA, pattern size = 100x100 μm, loop time = 558 msec). Note that the edges are deeper  than the center.


Despite the challenges, backside CE on full-thickness silicon  devices is indeed possible. Modern IR camera technology is  adequate to view circuitry details through many full-thickness  devices. Silicon trenching can be performed in a reasonable  amount of time by a combination of high-flux gas delivery  hardware and optimized milling parameters. Navigational  techniques exist that allow high targeting accuracy without  relying on corner fiducials. Finally, the limitations associated  with gas depletion and IR objective positions can be overcome


by adjusting the sample height prior to the edit. Although it  may not be the best approach for every edit, the full-thickness  approach should be considered as one of the many options  available to the FIB operator.


References and Notes


[1] Livengood, R. H., Winer, P., Rao, V. R., “Application of


Advanced Micromachining Techniques for the


Characterization and Debug of High Performance


Microprocessors,” J. Vac. Sci. Technol. B, 17(1), (1999),


pp. 40-43.


[2] Lee, R., Antoniou, N., “FIB Micro-Surgery on Flip-Chips


from the Backside,” Proc 24th International Symposium


for Testing and Failure Analysis, Dallas, TX, November,


1998, pp. 455-459.


[3] Antoniou, N., “The Process of Editing Circuits Though the


Bulk Silicon,” Microelectronics Failure Analysis, Desk


Reference, 5th Ed., (2004), pp. 71-75.


[4] Barton, D. L., Cole, E. I. Jr., Bernhard-Höfer, K., “FlipChip and ‘Backside’ Sample Preparation Techniques,”


Microelectronics Failure Analysis, Desk Reference, 5th


Ed., (2004), pp. 42-48.


[5] Perungulam, S., Wills, K. S., “Chip Access Techniques,”


Ed., (2004), pp. 312-322.


[6] Ehrich, D. J., Tsao, J. Y., “A Review of LaserMicrochemical Processing,” J. Vac. Sci. Technol. B1,


(1983), 969.


[7] Silverman, S., Aucoin, R., Mallatt, J., Ehrlich, D., “Laser


Microchemical Technology: New Tools for Flip-Chip


Debug and Failure Analysis,” Proc 23rd International


Symposium for Testing and Failure Analysis, Santa Clara,


CA, 1997, pp. 211-213.


[8] Li, Y., “Accurate Predictions of Flip Chip BGA


Warpage,” Proceedings 53rd Electronics and Components


Technology Conference, 2003, pp. 549-553.


[9] Sawada, Y., Harada, K., Fujioka, H., “Study of Package


Warp Behavior for High-Performance Flip-Chip BGA,”


Microelectronics Reliability, Vol. 43, Issue 3 (2003), pp.


465-471.


[10] S. Herschbein, C. Rue, C. Scrudato, E. Hermann, “FIB


Chip Repair: Improving Success by Controlling BeamInduced Damage and Thermal / Mechanical Stress” Proc


30th International Symposium for Testing and Failure


Analysis”, Worcester, MA, November, 2004.


[11] Bassom, N., Mai, T., “Modeling and Optimization XeF2-


Enhanced FIB Milling of Silicon,” Proc 25th International


CA, November, 1999, pp. 255-261.


[12] Herschbein, S., Rue, C., Scrudato, C., “The Joy of SOI:


As Viewed from a Backside FIB Perspective,” 31st


International Symposium for Testing and Failure


Analysis”, San Jose, CA, November, 2005, pp. 78-83.


DOI: 10.1361/cp2008istfa151


Insulator Deposition for Through Conductor Editing


Chris Richardson, Mark Martin LSI Corporation, Fort Collins, CO


LSI Corporation, Danfield Court, Fort Collins, Colorado, 80525   Tel: (970) 206-5456 Email: chris.richardson@lsi.com


Tahir Malik, Jerrold P Barone


DCG Systems, Northport Loop East, Fremont, California, 94538


Tel: (510) 897-6800 Email: tahir_malik@dcgsystems.com


Circuit Edit (CE) through a conductor requires an insulator to  isolate the connection transiting the conductor.  We  investigate several recipes to determine not just the optimum  recipe but also the latitude to provide a means of throughput  optimization for a given edit requirement.  The results show  that trade-offs in deposition rate, robustness and isolation  quality can be made to enable this throughput optimization.


The process of a FIB deposited insulator for circuit edit has  been thoroughly investigated for almost two decades [1-6].  In  circuit edit insulator deposition has several applications:


A. Repassivation of an edit state after an edit


B. Isolation of two newly formed traces


C. Sealing a copper edit to reduce corrosion


D. Protecting the bottom of a trench when backside  editing by preserving the nwell contrast, and making  an anti-reflective coating, ARC


E. Lining an access hole through a power plane (frontside) or through the silicon (backside) (See  Figure 1)


Application E should be considered the most critical of  these several applications.   Bringing a signal through a  conductive material such as the power plane or silicon  requires that the access hole be lined with insulator. With the  onset of low-k technologies, the increase in backside bulk  design repair applications, and increase in SOI applications, the more critical the role insulator deposition plays in the  successful design edit.   Characteristics that are important in  this application are:


1. A conformal lining of the insulator deposition  through the conductor:  This is measured by cross  sectioning a deposit lining a hole.  How deep the hole  is without sidewall “pillowing” or lack thereof is a  measure of the quality of conformal lining.  (See  Figure 2)


Figure 1.  SEM micrographs show an application of a


through silicon backside edit (top) and a through power plane  frontside edit (bottom) requiring the lining of an access hole  with insulator deposition for a VIA connection.


2. Leakage current or resistivity:  Subsequent to the  insulator deposition the hole must be opened to the  underlying trace and then filled to enable this  characterization.  Micro-probes are used to make  static/dynamic measurements of the resistivity/ leakage currents of the insulator deposition.  The  lower the leakage generally the better the deposit.


This requires High Secondary Electron detection (SED) sensitivity to observe metal endpoint after  milling through FIB deposited insulator at low beam  currents.  Good quality insulator quality makes endpointing more reliable.


3. Deposition rate: This would be the lateral deposition  rate on a vertical surface.  The higher the deposition  rate the more productivity it provides.  However  consideration must be given to controlling material  over-etch before insulator starts depositing on the  surface i.e. efficiency of depositing the seed layer.


4. Resistance to ion bombardment:  During subsequent  edit steps the Insulator deposition may be eroded and  thus the protection it offered may degrade.  A cross  section can determine the effects of erosion of the  insulator deposition.


Undoubtedly there may be trade-offs between these  characteristics.  A high deposition rate may not have a  sufficiently conformal lining but may yield great isolation [3].  Great conformal lining may not show very good resistance to  ion bombardment.  The goal therefore is improved knowledge  of the quality of the horizontal isolation in an Insulator  deposition lined access hole as well as the typical wall  thickness of a deposit.  This knowledge will enable the FIB  engineer to make an educated decision as to the trade-offs  necessary to implement a successful FIB edit.   Note: We  expect the insulator lining an access hole through a conductor  to incorporate some of the conductor and thus may be of less  quality than that deposited across a surface.


This work was performed with an OptiFIB-IV equipped with  a dual jet configuration and a standard 30keV Coaxial PhotonIon column.   OptiFIB uses a mixture of Insulator A & Insulator B chemistries for insulator deposition   Manipulating  mixture ratio and beam scanning parameters provide a range  of insulator quality and deposition rates for a variety of circuit  edit applications.


Evaluation of Deposition Rate:


The first key to understanding the insulator deposition process  is to evaluate the possible combinations of chemistry that can  be used for the through conductor edit.  NOTE: The insulator  deposition chemistry used in these experiments are specific to  the DCG Circuit Edit systems, applications to other CE tools  have not been investigated.  For this experiment the chemistry  used for the insulator deposition was changed, and the  parameters used for the “digital mode” were optimized.  An  unpassivated test device with multiple 1μm wide parallel lines  was selected for evaluation.  Using insulator deposition, three  deposits were made, 1) Insulator B only, 2) Insulator A&B in  a “compatible mode” and 3) Insulator A&B in a “digital  mode”.   Table 1 shows the simple FIB parameters used for  this experiment.


Figure 2.  Illustration of a through silicon VIA after


deposition of the insulator (top) but before it is opened for  conductor deposition. Note the conductive trace from the Si


which extends through the insulator.  SEM cross-section


micrograph (bottom) shows a consecutive insulator deposition  operation after going through each decreasing metal layer (frontside).  A poor conformal deposition, which is referred to  as “pillowing”, could result in the possibility of lateral short  on subsequent conductor operations.


Insulator B  Compatibility*


Insulator A&B  Compatibility*


Insulator A&B  Digital


Beam Current


1000pA


Deposition Time


Scan Paramaters


32x45 pixel spacing, 500ns dwell time,


1.59ms refresh rate


15min


N/A


500pA


* Compatibility Mode refers to a deposition mode that has a 512x512 pixel spacing with a  100ns dwell time, with a 33ms refresh rate.


Table 1.  Table shows the parameters used for determining  deposition rate on a surface deposition.


“Pillowing”


Lateral


Conductor


induced short


Since most CE FIB’s are in a critical path for accelerating the  design debug phase, the throughput on the system is a critical  parameter.  The purpose of this experiment is to evaluate the  deposition rate of the three possible insulator deposition  materials using an optimized recipe for each deposition.  While consideration should be given for the amount of  material that is sputtered during the beginning of the  deposition, it was not measured; rather focus was placed on  the thickness of material deposited after fifteen minutes (see  Figure 3a, 3b, and 3c).  Table 2 summarizes the thickness of  deposited materials, and the rough deposition rate of each  material per minute.  Based on the results, the best throughput  on the system can be obtained using Insulator B; however the  other three key considerations for insulator deposition have  yet to be taken into consideration.


Figure 3a.  SEM cross-section micrograph shows the


Insulator B only deposition on the surface of the test device.


Figure 3b.  SEM cross-section micrograph shows the


Insulator A&B in compatibility mode deposition on the  surface of the test device.


Figure 3c.  SEM cross-section micrograph shows the


Insulator A&B in digital mode deposition on the surface of the  test device.


Site 1 Site 2 Site 3


Insulator B


Compatibility*1013 1304 1324 1214 20.23 Insulator A&B


Compatibility*472


508


362 447.3 7.46


745


698


680 707.7 11.79


Deposition


Rate


(nm/min)


Measurements in nm


Mean


Table 2.  Table summarizes the average vertical thickness and


a rough deposition rate calculation of the three different


insulator deposition options.


Evaluation of Conformal Lining, Ion bombardment  robustness and Leakage Current:


For this experiment a 130nm Copper technology flip-chip  device was selected for analysis.  The part was prepared using  a standard mechanical lapping technique to reduce the bulk  silicon thickness down to 50μm.  A trench was created using  the ion beam and gas chemistry to further reduce the thickness  of the device in a region of interest, to within approximately  three microns over the active regions [8]. Upon completion of  the trench activity, an in-situ FIB deposited insulator is put  down over the entire trench floor acting as an AR coating and  to passivate the silicon.


Table 3 summarizes the FIB parameters used for the DOE to  create a VIA through the silicon to evaluate the three key  characteristics to through conductor editing.


Insulator A&B


Digital**


Metal (EDI)


Pressure


I-Dep


50pA


100pA


Deposition Time Pressure


Dielectric (XeF2)


Conductor (Platinum)


Beam Current Pressure


Cap (Platinum)


Beam Current Deposition Time Pressure


3μmx3μm 5min20sec


2.50E-05 Torr


1.00E-05 Torr 2μmX2μm


1.20E-05 Torr


1μmx1μm


10pA


5.00E-05 Torr


0.75μmx0.75μm


5pA


1.10E-05 Torr


** Digital Mode refers to a deposition mode that has been optimized using digitally


enhanced paramaters.  The deposition was performed with a 30x43 pixel spacing, a 500ns  dwell time and a 1.44ms refresh rate.


3min


3μmx3μm


5min


Table 3.  Table shows the parameters used for determining a  conformal lining, leakage current, and the resistance to ion  bombardment.


To evaluate the electrical isolation proprieties of the  individual through conductor isolated VIAs, probe pads were  placed on a Vdd signal line and a measurement was made  from the bulk silicon to the individual probe pads. (See Figure  4a, 4b)


Figure 4a shows the insulator results of the Insulator B only, Insulator A&B compatible mode, and Insulator A&B digital


mode (left to right respectively).  Darkness is generally


considered a measure of the insulator deposition quality due


to the voltage contrast of the “charged-up” insulator.


Figure 4b shows the results of the 1μmx1μm VIA cut through  the insulator.


A simple two probe setup was used to measure between the  deposited VIA and the bulk silicon.  Based on the electrical  measurements taken (see Table 4), the electrical isolation, for  the worst case deposition of Insulator B only was greater than  7MΩ, while the best case deposition was Insulator A&B in  digital mode.


For evaluation of the ion bombardment resistance, a crosssection was performed on the electrically measured VIA, and  the ion bombardment resistance was measured by the change  in the opening of the VIA at the surface, post conductor fill.   Figures 5a, 5b, and 5c show the SEM micrographs, and Table  4 summarizes the effects of Insulator erosion.  In order to keep  the parameters consistent, all VIAs were measured near the  silicon to insulator interface.  Additionally, since the beam  current for the VIA cut was held constant,  the contribution of  erosion due to current density was neglected.   With the crosssection an evaluation can be made on how conformal the liner  is inside the VIA opening.


Starting Box  Dimension


Ending


Deposition  Measurement


1.06


7.55E+06


1.69


1.04E+07


1.15


2.46E+07


Insulator Erosion


Measured  Resistance (Ω)


Table 4 summarizes the effects of insulator erosion, and


provides the lateral (through the vertical insulator deposition


wall) electrical performance of the insulator isolation.


Figure 5a. SEM cross-section micrograph shows the results of  Ion erosion and the conformal nature of the insulator liner for  Insulator B only.


Figure 5b. SEM cross-section micrograph shows the results of  Ion erosion and the conformal nature of the insulator liner for  Insulator A&B in compatibility mode.


Figure 5c. SEM cross-section micrograph shows the results of  Ion erosion and the conformal nature of the insulator liner for  Insulator A&B in digital mode.


Based on the experimental results, Insulator B results in the  highest deposition rate, best conformal lining and the best  robustness in regards to ion erosion; however it exhibited poor  electrical isolation.  Insulator A&B in compatibility mode had  the lowest deposition rate, the worst robustness in regards to  ion erosion but had fair electrical isolation.  Insulator A&B in  digital mode had a fair deposition rate, fair ion erosion  robustness, and the best electrical isolation performance.


Insulator deposition is critical for Circuit Edit (CE) operations, whether the application is a frontside, through  power plane/redistribution metal edit, or backside, through  silicon edit, an intimate understanding of the properties of the  deposition are necessary to insure a higher possible CE  success rate.   The purpose of this paper was to gain a better  understanding of the trade-offs between deposition rates, ion  bombardment robustness, leakage currents, and quality of the  conformal side wall.  Through this evaluation it is now very  clear that the process will require custom tuning to a specific  application, digital/analog, frontside/backside. Armed with  this information, a FIB engineer can now start tuning the  process to suit their specific application.


The initial results show an electrical leakage characteristic  latterly through the silicon that may or may not be acceptable  to most applications; therefore more investigation is needed to  determine the amount of sidewall insulator deposition that  should be left to ensure a leakage characteristic that is  reasonable for the given application.   Additionally, an  investigation into the effects of thermal aging of the through  conductor edit should be considered.


[1] J. R. Baker, “Focused Ion Beam Insulator  Deposition,” ASM-ISTFA (1995) 43.


[2] M. T. Abramo et al., “Focused-ion-Beam insulator  Deposition: An advanced Technique for Device  Modification,” IEEE-ESREF (1995) 313.


[3] L. L. Hahn et al., “Focused-Ion Beam-Induced  Insulator Deposition for Chip circuit Modification,” Thin Solid Films 270 (1995) 422.


[4] H. Komano et al., “A Rewiring Technique for  Integrated Circuit Operation Analysis using a Silicon  Oxide Film Deposited by a Focused ion Beam,” JVST B9 (1991) 2653.


[5] M. T. Abramo et al., “”Focused Ion Beam Induced  Insulator Deposition at Decreased Beam Current  Density,” IEEE-IRPS (1997) 66.


[6] A. N. Campbell, “Electrical and Chemical  Characterization of FIB-Deposited Insulators”, ASMISTFA (1997) 223.


[7] E. Le Roy and M. Thompson Mat. “n-wells voltage  Contrast imaging with a Focused Ion Beam”, Mat. Res. Soc. Symp. Proc. Vol.792 (2004)


[8] M. A. Thompson, C. Richardson, E. Le Roy, T. Lundquist and W. B. Thompson “Coaxial, PhotonIon Technology Enables Direct Navigation to Buried  Nodes on Planarized Surfaces, including Silicon” Proc ISTFA (2002) 409.


DOI: 10.1361/cp2008istfa157


Creation of Solid Immersion Lenses in Bulk Silicon  Using Focused Ion Beam Backside Editing Techniques


P. Scholz, U. Kerst, C. Boit


Berlin University of Technology, D-10587 Berlin, Germany  philipp.scholz@tu-berlin.de, +49-30-314-26803


C.-C. Tsao*, T. Lundquist


DCG Systems, Fremont, CA 94538, USA


* currently with Solyndra, Fremont, CA 94538, USA


This work describes how Solid Immersion Lenses (SILs) can be  created in bulk silicon using a focused ion beam and a bitmap  milling process. The optical properties are in good agreement  with the expected results for the achieved lens geometries. An  improvement in lateral spatial resolution by a factor of 1.8 and in  image contrast by 170 % for backside analysis is demonstrated. The presented SILs are 32 µm in diameter with a field of view of  about 10 µm. This process can be an alternative when a regular  SIL placement on the chip is impossible or complex. The  advantages of this method are the use of a single kind of material (no air gaps and no additional lens material with different  n value), the ability to precisely position the SIL on the circuitry  and the fact that a SIL may be created in less than twenty  minutes of processing time.


The growing number of metal layers and the change in package  design force failure analysts to approach semiconductor devices  from the backside through the silicon bulk. Due to the absorption  behavior of the semiconductor material, these methods depend  on long wavelengths reducing the possible resolution. This  problem is addressed by forming a solid immersion lens out of  the bulk silicon of the chip backside, which results in an  improvement in image contrast and resolution.


The ability to resolve two points of an image is proportional to λ / NA, where λ is the wavelength and NA is the numerical  aperture defined by n · sin θ. n is the index of refraction of the  material between objective lens and object plane. θ is the half  angle of the acceptance cone of the objective (see Fig 1). When  using a solid immersion lens in silicon and calculating the  possible resolution, the value of n changes from ≈ 1 (air) to ≈ 3.5 (silicon) [1]. Effectively the air gap between SIL and objective  loses its limiting impact. This shows why a hemispherical SIL  can theoretically enhance the resolution for backside analysis by  the factor of the refractive index of silicon n ≈ 3.5. An influence


of doping on n can be ignored (less than 1 % for doping  concentrations less than 1019 cm-3 [2], as it is the case in this  work). n is also wavelength dependent. For the two laser  wavelengths used in this work n = 3.501 if λ = 1319 nm and  n = 3.551 if λ = 1064 nm [3].


Figure 1:  Determining minimum radius of the ideal SIL.


The shape of the SIL has to match certain criteria depending on  the parameters of the sample. Most important is the thickness t of  the remaining silicon out of which the lens is created. The SIL  has to be part of a virtual hemisphere touching the focal plane (see dashed curve in Fig. 2). For an ideal SIL the radius of the  theoretical hemisphere (now called radius of curvature r) needs  to be equal to the thickness t (r = t). If this condition is met, each  ray being reflected or emitted from the center of view on the  object plane and passing from silicon to air (or vice versa) through the lens, hits the surface at a perpendicular angle and  does not undergo refraction. Even if this condition is not  achieved, a useful lens can be created. In this case, resolution and  focal point deviate from the model in Fig. 1 (discussed later in  Realization of the SIL).


Figure 2:  Construction of a SIL in bulk silicon.


The maximum cone of light that can enter or exit the SIL should  be bigger than that reaching the objective lens (compare R and  Rmin in Fig. 1). Using the numerical aperture of the preferably  used objective the ideal minimum radius Rmin of the SIL can be  calculated. The numerical aperture in air (n = 1) is described by  sin θ. Assuming every ray from and to the center of view on the  object plane passes through the surface at a perpendicular angle, sin θ is equal to Rmin / r (see Fig. 1) which becomes Rmin = NA · r. This equation can be expanded to get a more universally valid  expression that takes the field of view (FOV) into account by  adding “+ FOV / 2”, leading to Eq. 1.


Rmin = NA · r + FOV / 2


(1) Previous works have successfully used SILs placed on the  surface of the wafer to increase the numerical aperture and  thereby the possible resolution: aplanatic or numerical aperture  increasing lens (NAIL) [4, 5, 6] and biconvex lens [7]. They all  have to be brought in good contact with the sample to reduce the  effect of the gap underneath the base of the lens. Due to the  construction of these lenses, they can only be used on objects at  least the lens base radius (R = 1.6 mm in [4]) away from an  obstacle, e.g. inner edge of opened chip area or package. Reducing the opening angle of the lens by a reasonable amount  gives the opportunity to create an almost cone shaped base [8] which increases the area that can be analyzed. This method also  needs a direct contact of the lens setup to the sample which can  cause problems in situations where an effective long working  distance is needed.


The still remaining interface between lens and sample can be  avoided by creating the lens out of the backside material as  presented in [9] using the process “forming the Si substrate into  solid immersion lens” (FOSSIL). A SIL with a base radius  R ≈ 220 µm and FOV ≈ 30 µm is created using a mechanical  computer controlled milling process for about 15 minutes. The  overall needed area has a radius of about 2.5 mm. Besides using  mechanical milling, lens shapes can also be produced by a  focused ion beam (FIB). Lenses with a base radius of R ≈ 75 µm [10] and R ≈ 24 µm [11] are presented. The processing time and  the optical properties are not discussed.


All the so far mentioned works use hemispherical refractive  lenses (hSILs). A different approach is the use of a planar  diffractive lens - dSIL (aka zone plate, Fresnel lens) [12]. These


structures can also be produced using a FIB. A diffractive lens  with the radius R = 100 µm (in this case equal to the overall  needed area) and FOV ≈ 20 µm can be created in about one hour  of processing time [13].


The goal of this work is to present a fast and practical solution  for the creation of solid immersion lenses in bulk silicon using  focused ion beam backside editing techniques. From all the  previously mentioned works this method was further pursued, because it has the potential to create a homogenous lens shape  with a good ratio of field of view to needed processing area in a  short period of time. The presented SIL having a radius  R ≈ 16 µm and FOV ≈ 10 µm needs an area with a radius of  about 20 µm and can be created in less than 20 minutes of  processing time. It can be especially helpful when an effective  long working distance is needed, e.g. due to restrictions from  package geometries or required cooling solutions. Apart from  improving the possibilities of backside optical analysis, this work  can also be a basis for the creation of micro optics.


Experiments and Results


Construction of the SIL


In these experiments the solid immersion lens is created out of  the bulk silicon of the chip backside by a focused ion beam. The  tool in use is an OptiFIB from DCG Systems. The so called  bitmap mode is the key function for the micromachining process. In this mode a 512 by 512 pixel 8-bit grayscale bitmap serves as  a template [14]. Its grayscale values control the dwell time (= the  period of time a certain pixel area is exposed to the ion beam). Equation 2 shows the relation between each of the 256 grayscale  values and the resulting dwell time DT.


DT = 200 ns,  if  gs = 0 or 1


DT = 300 ns + 50(gs – 2) ns,  if  gs ∈ {2, …, 255}  (2)


DT: dwell time [ns]


gs: grayscale value [-]


The minimum dwell time is indicated by black and the maximum  dwell time by white pixel color. The ion beam is blanked for a  grayscale value of 0 = black pixel color.


The desired SIL shape remains after removing the surrounding  material (see gray-marked area in Fig. 2). The bitmap template  for this procedure is designed from the mathematical model of a  hemisphere which leads to the calculation of the z values in  Eq. 3.


z = (a2 – x2 – y2) 0.5


(3)


x, y, z: coordinates


a: radius of hemisphere


Using this formula (Eq. 3) on a 512 by 512 matrix is the basis of  the bitmap creation. The result (with reduced height) is  illustrated as a 3D model in Fig. 3.


Figure 3:  3D model of hemisphere for bitmap.


The next step is the calculation of the grayscale values, which  depends on the needed shape and the processing method. In this  case, for the pure sputtering of shallow depths in a relatively  short period of time (10 min.) a linear relationship between z and  grayscale values is used. Experiments showed that this can be  assumed up to a grayscale value of 155. The sputtered depths  barely increased for larger values, which is one reason why an  ideal SIL shape as described in the introduction is not realized. Apart from finding a proper scaling factor (1.66 in this case), the  z values also have to be shifted and inverted to create the  grayscale bitmap. The top of the hemisphere model needs the  least amount of processing and the edge needs the most. Figure 4  shows the calculated data that will be saved as a bitmap file for  further processing.


Figure 4:  Grayscale values derived from the 3D model.


Realization of the SIL


The lens shaped surface is created by processing the bulk  material with the previously described bitmap template in a pure  ion beam sputtering process. The following gas assisted cleaning  step removes the damaged and nontransparent surface layer. The  resulting SIL is a spherical cap formed out of the remaining  silicon (compare Fig. 2). As mentioned earlier the geometries of  an ideal SIL are not realized because the depths that can  predictably be reached are limited. Another reason is that at  longer processing times the ion beam damages the surface too  much to be removed by the cleaning step. This results in the loss  of transparency at larger milling depths. The same problems  were observed for gas assisted etch processing. Decreasing the  beam energy or current is also not a real solution. It does lower


the surface damage, but also drastically increases the processing  time and reduces the homogeneity of the surface due to a smaller  beam spot.


Figure 5:  Cross section of the SIL.


A cross section is analyzed to measure the dimensions of the SIL  with the characterizing parameters height h and radius R as  shown in Fig. 5. A metal layer is deposited on the surface to  protect the bulk silicon from the ion beam that creates the cross  section. The silicon appears dark against the metal layer. The  cross section is observed at an angle of 52° reducing the vertical  dimension by 1.269 (=1/sin 52°). The radius of curvature r can  be calculated using Eq. 4 (see also Fig. 2).


r = (R2 + h2) / 2h


(4)


r: radius of curvature


R: radius of SIL


h: height of SIL


The SIL presented in this work (see Fig. 5, 6, 8, 10) has the  dimensions R = 16.3 µm, h = 1.4 µm and a calculated  r = 95.6 µm. The accuracy of the calculated r is better than five  percent based solely on the image resolution and the small h  value. The geometry of this lens was verified using atomic force  microscopy (AFM). The AFM measurements showed a  homogenous spherical shape deviating from a calculated sphere  by no more than 55 nm (3D overview in Fig. 6).


Figure 6: 3D image of AFM data.


Figure 7:  Illustrating the spherical shape of the SIL - observed  at an angle of 30°.


The calculation of the radius of curvature r (see Eq. 4) and the  principle of the SIL require a spherically shaped surface. This  condition was verified and is illustrated by superimposing a  circular ring on the picture of the cross section. Figure 7 shows  an example of a small ring that is observed at a thirty degree  angle reducing its height by fifty percent. The analysis of the SIL  presented in this work can be seen in Fig. 8. The radius of the  ring closely matches the calculated radius of curvature.


Figure 8:  Comparing calculated radius of curvature to actual  lens surface - observed at an angle of 52°.


The created SIL was built on a 55 µm or 60 µm thick sample and  was therefore not an ideal SIL that satisfies t = r. Despite not  meeting the ideal condition, this kind of SIL with a radius of  curvature r larger than the sample thickness t (see Fig. 9) still had  a positive optical effect that could be evaluated by the first-order  lens formula (Eq. 5) [15]. Using the fact that so = t and solving  this formula for si gives the opportunity to calculate the  transversal magnification M_T (Eq. 6) [15].


n1 / so + n2 / si = (n2 + n1) / r


(5)


M_T = (n1 · si) / (n2 · so)


(6)


n1: index of refraction in object space (3.5 in this case)


n2: index of refraction in image space (1 in this case)


so: object distance (= t in this case)


si: image distance


r: radius of curvature (negative in this case)


M_T: transversal magnification


Figure 9:  Spherical lens setup used to calculate expected results  for t ≠ r. Object A not being in the center of curvature B.


Note that for an ideal SIL in air with t = r the calculated  magnification would be M_T = n1 ≈ 3.5 - similar to the possible  improvement of resolution discussed in the introduction. One  thing that has to be kept in mind when using Eq. 5 is that it is  only valid in the paraxial region, where a small opening angle 2θ (see Fig. 1) is used and sin θ ≈ θ (in radian) can be assumed. For  the presented SIL the angle θ = arctan (R / t) = 16.5° differs by  less than 2 % from sin θ. Calculating M_T for this case leads to a  factor of 1.7 which can also be observed when comparing the  image features in Fig. 10 a) and b).


a)                                             b)


Figure 10:  1319 nm laser scanning images of SIL built on  55 µm thick sample - a) focused on the area outside and   b) inside of the SIL (scale adjusted to magnification inside SIL). Recurring structures can be compared. The SIL shows a  magnification of 1.7.


The created SILs are examined using a laser scanning  microscope. The result of one experiment is shown in Fig. 10  using a 100x objective with NA = 0.5 and a 1319 nm laser  wavelength. In Fig. 10 a) the picture is focused on the area  outside and in Fig. 10 b) inside of the SIL. The diameter of this  SIL is 32.6 µm (marked by 2R). An improvement in image  quality is clearly visible. The processing time for a structure like  this is 20 minutes or shorter. The pattern has a pitch value of  about 1.9 µm. The individual spots can be clearly distinguished  underneath the SIL, which is not the case without SIL. This  effect is analyzed by doing a line scan to measure the change in  pixel intensity (Fig. 11). This change is perceived as contrast and  significantly influences the ability to distinguish small details of  an image. The contrast can be calculated as shown in Eq. 7 [15].


contrast  = (Imax - Imin) / (Imax + Imin)


(7)


Imax: maximum of irradiance


Imin: minimum of irradiance


Figure 11:  Line scan over image features. Left without SIL, right with SIL. a) (top) comparable details from Fig. 10  b) (middle) region of line scan = dotted line - at same scale  c) (bottom) intensity scan of red dotted line in (b), normalized.


Using Eq. 7 on the objects of the line scan and comparing the  results with and without SIL leads to an improvement in contrast  by 170 %. The increase in contrast proves that the increased  feature size is not an empty magnification, but a true  improvement of image quality.


The SIL was also created on an optical test structure with a  sample thickness ≈ 60 µm and examined by a laser scanning  microscope using a 1064 nm laser (refractive index of silicon  n = 3.551 [3]) and a 100x objective with a numerical aperture of


0.5. Figure 12 a) shows the structure. The dashed circle indicates  where the SIL is created. It is observed that in group 9 (mirrored “9” above) the element 10 (mirrored “10” to the left) with a pitch  value of 1.23 µm can be clearly resolved and the element 11  almost. Therefore the limit of resolution without a SIL is in this  case a little below 1.23 µm. Putting the index of refraction along  with the measured radius of curvature of the SIL and the sample  thickness into Eq. 5 and 6 shows that the calculated transversal  magnification is ≈ 1.8. Figure 12 b) proves that this factor also  applies to the improvement in resolution. The pattern in the  center of the SIL (mirrored “10” above and “9” to the right) has a  pitch value of 0.69 µm and can be clearly resolved using the SIL  just like the 1.23 µm pattern without SIL.


The theoretically possible improvement in resolution by n ≈ 3.5  was not reached, on the one hand due to the mismatch of sample  thickness t and radius of curvature r and on the other due to the  limiting opening angle 2θ of the SIL (see Fig. 1). As mentioned  earlier the presented SIL has an angle θ = arctan (R / t) ≈ 16° for  a sample thickness between 55 and 60 µm. The used 100x  objective offers θ = arcsin NA = 30°. The effects of these two  factors however have an inverse relationship. Using the SIL on a  thinner sample creates a better (larger) opening angle but makes  the difference between r and t worse (larger) and vice versa. This  leads to the conclusion that a good compromise in favor of a fast  processing time is found here.


The results of the presented work demonstrate that the creation  of a solid immersion lens in bulk silicon using a Focused Ion  Beam is a promising solution to improve contrast and image  resolution for backside analysis of integrated circuits. A  procedure has been developed creating a lens with  homogeneously shaped surface. Although not every desired  shape has been realized, the optical properties of the designed  SILs are in good agreement with the expected results for the  achieved lens geometries (see Eq. 6). This FIB based process can  be an alternative when a regular SIL placement on the chip is  impossible or complex. The advantages of this method are the  use of a single kind of material (no air gaps and no additional  lens material with different n value) and the ability to precisely  position the SIL on the circuitry (CAD assisted navigation with  the OptiFIB provides a placement accuracy better than 0.1 µm


[16]). This work presents a quick way to improve image  resolution by a factor of 1.8 using backside editing tools and  techniques.


a)


b)


Figure 12:  1064 nm laser scanning images of optical test  structure under a 60 µm thick sample using 100x objective with  NA = 0.5. a) without and b) with SIL (scale adjusted to  magnification inside SIL). The pattern element 9 from group 10  in the center of the SIL - dashed circle in (a) - has a pitch value  of 690 nm and can be clearly resolved using the SIL.


Special thanks to Rudolf Schlangen (TU Berlin) for teaching FIB  and for continuous support. Further thanks go to Stefan Meister (TU Berlin) for AFM measurements and to Reiner Güther (FBH  Berlin) for support in optics and lens questions. Thanks to  Ultra Tec for sample preparation support.


[1] J. McDonald, “Optical Microscopy”, Microelectronics  Failure Analysis Desk Reference 5th Edition, 2004, pp. 540-558


[2] R.A. Soref, B.R. Bennett, “Electrooptical Effects in  Silicon”, IEEE Journal of Quantum Electronics Vol. QE-23, No. 1, 1987, pp. 123-129


[3] H.-G. Wagemann, Grundlagen der optoelektronischen  Halbleiterbauelemente, B. G. Teubner (Stuttgart 1998), p. 228


[4] S.B. Ippolito et al., “High Resolution Subsurface  Microscopy Technique”, Proc. 13th IEEE LEOS, 2000


[5] S.B. Ippolito, B.B. Goldberg, M.S. Ünlü, “Comparison of  Numerical Aperture Increasing Lens and standard  subsurface microscopy”, Proc. 14th IEEE LEOS, 2001, pp. 774-775


[6] S.B. Ippolito, B.B. Goldberg, M.S. Ünlü, “Theoretical  analysis of numerical aperture increasing lens microscopy”, J. Appl. Phys. 97, 2005


[7] N. Pakdaman, J.S. Vickers, “Bi-convex solid immersion  lens”, US Patent 6,778,327


[8] O. Breitenstein et al., “Lock-in thermal IR imaging using a  solid immersion lens”, Microelectronics Reliability Vol. 46, 2006, pp. 1508-1513


[9] T. Koyama et al., “High Resolution Backside Fault Isolation  Technique Using Directly Forming Si Substrate into Solid  Immersion Lens”, Proc. 41st IRPS, 2003, pp. 529-535


[10] M. Kitamura et al., “Focused Ion Beam Machining for  Optical Microlens Fabrication”, Jpn. J. Appl. Phys. Vol. 41, 2002, pp. 4019-4021


[11] Y. Fu, N.K. Bryan, “Semiconductor Microlenses Fabricated  by One-Step Focused Ion Beam Direct Writing”, IEEE  Trans. Semicond. Manuf. Vol. 15, 2002, pp. 229-231


[12] E. Coyne, F. Zachariasse “A working method for  prototyping solid immersion blazed-phase diffractive optics  for near-infrared laser microscopy”, J. Micromech. Microeng. 18, 2008, pp. 1-9


[13] F. Zachariasse, M. Goossens, “Diffractive lenses for high  resolution laser based failure analysis”, Proc. 31st ISTFA, 2005, pp. 1-7


[14] J Siebert, L Johri, D McCarty, S Voong, M Sengupta, H  Wang, "Enhanced Scanning Control of Charged Particle  Beam Systems", US Patent 7,230,240


[15] E. Hecht, Optics, Addison-Wesley (2nd Ed., 1974), p.134. p.144, p. 507


[16] DCG Systems, OptiFIB Manual


DOI: 10.1361/cp2008istfa163


S/D LDD Junction Stain/Delineation by Electrochemical Displacement with  Illumination


Re-Long Chiu, Tammy Chen, Shannon Chen


WaferTech LLC CAMAS Washington   rchiu@wafertech.com  360-8173364


This article describes the use of an optimized electrochemical  delineation technique with illumination to clearly delineate the  P-N junction on Si in short channel devices. In this process, the samples are exposed to a light source while in an aqueous  CuSO4/HF/H2SO4 solution which induces a junction voltage  between N- and P- type silicon. The N+/P+ dopant regions  become the cathode/anode electrode plates.  The treatment is  simple and reproducible which makes it a practical method for  identifying junction related problems at localized areas on a  chip.  Examples are provided to show the effectiveness of this  technique in identifying (1) junction implant shift, (2) N+/Pwell junction leak, (3) partially blocked NLDD implant, and


(4) P+/N+ junction in high voltage device.


Junction-related failures are usually invisible to inline  inspections and wafer acceptance test (WAT) monitors.  Secondary ion mass spectroscopy (SIMS) is typically used to  monitor the implant depth profiles, but it is not an option for  analyzing localized areas because of its large ion sputtering  area and known low lateral resolution.  Thus, more localized  analysis methods are desired to analyze the implantation  profiles in a specific area of a chip.


There are a number of junction stain treatments that have been  developed to highlight the junction profile.  For example, HFHNO3-CH3COOH (HNA) by different ratio is universally  used for staining P+.  Unfortunately, the etch procedure is  very complex, its process window is small, and the etch result  is dependent on a variety of parameters.  These combined  factors typically lead to a poor sample-to-sample  reproducibility.  Another available method is the junction  etching of TEM samples but the result depends on  temperature, etching time control, and complex TEM sample  preparations, as well as sample size limitations [1, 2].


Different from the HNA, the electrochemical displacement  process using an aqueous solution of CuSO4 and HF has been  known to delineate P-N junctions on Si [3, 4]. But, the  maximum junction resolution is about 2 microns which does  not meet the requirements for short channel devices. With


light illumination and optimization of a CuSO4/HF/H2SO4  solution, a finer junction resolution is achieved and can be  applicable to short channel devices.  It has been reported that  illumination improves the accuracy of staining results by  increasing the carrier concentrations in the vicinity of the  junction, which serves to stabilize the reaction and reduces the  effect of experimental variations, such as surface conditions [4, 5].


By placing the polished cross-section sample in the  CuSO4/HF/H2SO4 solution with illumination, a junction  voltage is induced between the n- and p-type silicon regions. The N+/P+ dopant areas, where the metals deposit, become  the cathode/anodic electrode plates.  The amount of metal  deposit increases with the process time.  The reaction at the  anodic electrode plate is different from that of the cathode  electrode plate.  By carefully removing the metal deposits  from the anodic and cathode electrode plates, a sharp image  contrast between n+ and p+ doped regions is observed by  Scanning Electron Microscope (SEM) at high magnifications.  This is due to the difference in the resulting morphology of  the two surfaces.  The electrode plate areas do not change  during a short electrochemical reaction time period. This  treatment is reproducible and the result is consistent.


Experimental Methods and Results


A 0.15 µm SRAM part was selected for the experiment.  The  samples were first mechanically cross-sectioned and polished.  They were then immersed in the Cu electrochemical  displacement solution of 5 g CuSO4.5H2O, 4 mL 49% HF, 5 mL 98% H2SO4 and 200 mL DI water at room temperature  with around 4000 lux illumination for about 15 sec.  By  keeping the sample cross-section site up, the light could  illuminate the surface directly.  Samples were then rinsed with  water, blown dry with nitrogen, baked, coated with Pt, and  inspected by SEM. Figure 1 shows Cu deposits that were  observed on the cross-sectioned sample of conductive areas (metal line, via, contact and Si-substrate). After Cu deposits  were removed by physically rubbing the surface with a cotton  swab, NMOS and PMOS source/drain (S/D) lightly doped  drain (LDD) junction profiles can be clearly delineated (see  Fig. 2a and Fig. 2b).


Figure 1: (a) Cu deposits on the cross-sectioned sample of  conductive areas (metal line, via, contact and Si substrate)


(b) zoom-in view.


Figure 2: NMOS (a) and PMOS (b) S/D LDD junction profiles  are clearly delineated after the removal of Cu deposits.


To optimize the junction stain condition, different stain  parameters, such as illumination, time, and without  electrolytic salt were experimented. Figure 3 shows a sample  that was stained under a weaker illumination condition (i.e. weak room light at ~20 lux) for 15 sec. The NMOS S/D LDD  stain result is similar to that of Fig. 2a (one with strong light  illumination), but the PMOS LDD profile is poor and barely  visible


(Fig. 3b). The weak room illumination condition  (20 lux) can  give an acceptable result because of the optical induced  junction voltage and the galvanic cell that automatically forms  between the Al and W in the electrolytic solution.


Figure 3: Sample stained under the normal room illumination  condition for 15 sec. (a) clear NMOS S/D LDD profile (b) poor PMOS LDD profile.


Figure 4a shows a sample that was stained without any  electrolytic salt (CuSO4.5H2O) for 15 sec under illumination.  In this case, even the NMOS junction profile is not delineated.  The experiment shows that the electrolytic salt plays a  dominant role in the junction profile.  For the stain time effect  comparison, the NMOS S/D LDD profile can be produced in  5 sec (Fig. 5a), but the PMOS profile is not clear even after  staining for up to 10 sec (Fig. 5b).


For better uniformity and image contrast, the Cu  electrochemical displacement solution of 5 g CuSO4.5H2O, 4 mL 49% HF, 5 mL 98% H2SO4 and 200 mL DI water at  room temperature with illumination for about 15 sec was used  as our standard procedure.


Figure 4:  Sample stained with no electrolyte salt (CuSO4.5H2O) for 15 sec with illumination. NMOS S/D LDD  junction profile isn’t delineated.


Figure 5: (a) NMOS S/D LDD profile is created after 5 sec of  stain (b) PMOS S/D LDD profile still not visible after 10 sec  of stain.


Application


Four examples are presented here to show the effectiveness of  this technique in identifying the root cause of (1) junction  implant shift, (2) N+/P-well junction leak, (3) partially  blocked NLDD implant, and (4) P+/N+ junction in high  voltage device.


Junction Implant Shift


This technique was successfully used to identify the root  cause of an N+ implant shift issue that had caused significant  yield loss on a 0.18 µm mix-mode device.  Figure 6 shows the  chip probing (CP) maps of the mix-mode product with reticlefield-dependent failure patterns.  The failed dies are  highlighted in dark color.  The failure mode was  Vdd_Shutdown (high leakage current), with no suspected root  cause from inline process history and WAT data analysis.  Emission microscopy was able to isolate a leakage location.  However, no defects were found upon de-layering or cross  sectioning of the failing units.


Figure 6: CP maps with reticle field dependence at wafer top. There are 7x10 die in one reticle; the failure dies are  highlighted by dark color.


Figure 7: (a) layout of N+, P+ and contact (b) image of  silicon substrate with N+ dopant shifted into P+ region   (marked by circle) (c) zoom in view.


Junction stain with illumination was subsequently done on a  polished cross-section sample and was able to highlight N+ implanted into a P+ region.  Figure 7a shows the N+/P+ location that were cross-sectioned and stained.


Figure 7b and 7c shows the SEM image of the N+ dopant  region shifted into the P+ region. This observed shift in N+ was able to explain for high leakage current failures and led to  the necessary corrective actions.


N+/P-well Junction Leak


The leakage current control is very important for the memory  device. For one e-Flash product which had failed the N+/Pwell junction leakage test item, the stain treatment again found  its usefulness. Figure 8a shows a schematic diagram of the  leakage test structure. Current is measured while a voltage  difference of 3.6 V is applied across the N+ and P-well. The  leakage current for this test structure on a normal wafer was ~10 pA, while the current on the failed structures measured ~100 µA. The failed test structure was cross-sectioned, stained, and viewed by SEM.  A clear image of the TiSi/N+/Pwell interface (Fig. 8b and 8c) was produced. The anomaly is  indexed by an arrow marker in Fig. 8c showing the TiSi  nearly touching the N+/P-well interface which creates the  likely path for the junction leakage.


Partially blocked NLDD Implant


A 0.18 µm product lot suffered low yield on one out of every  four wafers.  The electrical parameters and tool correlation  analysis pinpointed to an NLDD problem. The stain treatment  was applied to quickly confirm the suspected root cause.  Figure 9a and 9b compares the junction profiles of the normal  versus impacted wafers, respectively.  The NLDD profile was  abnormal for the impacted wafers--some NLDD implant was  partially blocked (indicated by arrows in Fig. 9b) due to  incomplete development of the photo resist.


Figure 8: (a) the leakage test structure schematic diagram


(b) TiSi close N+/P-well interface almost touching the P-well  indexed by arrow marker (c) zoomed in view to show.


P+/N+ Junction in High Voltage Device


Junction profile is also very important for the high voltage  technology devices. Junction profile evaluation was   applied on a 0.35 µm/24 V device during process technology  development. The results of the junction stains were observed  by using an SEM at high magnifications.  Figure 10 shows the  high contrast image between N+ and P+ regions for the


0.35 µm/24 V device.  The N+ (cathode plate) etched faster  than the P+ (anodic plate) during the electrochemical reaction  and hence, appeared darker in color.


Highly delineated junctions (e.g. N-/P- type S/D and LDD  profiles) were defined using the CuSO4/HF/H2SO4 as the  staining solution with illumination.  This electrochemical  displacement method was simple, as well as reproducible with  consistent results.  It was successfully applied to quickly  resolve junction related problems encountered by various  products ranging from 0.35 µm/24 V to 0.15 µm/1.5 V  devices.


Figure 9: Shows the junction profiles of the (a) normal versus


(b) impacted wafers for comparison.  The impacted wafer  shows partially blocked NLDD implant that is highlighted by  the arrow markers.


Figure 10: SEM photograph shows one 0.35 µm/24 V voltage  sample after junction stain treatment.  SEM image shows two  types of high contrast junction profile: the N+ (cathode plate) and the P+ (anodic plate, lighter in colour).


The authors would like to acknowledge Bernd Krüger and  Michael Huettinger for their assistance in critiquing the paper, Ganesh Yerubandi who read and commented the manuscript  and supports from members of Failure Analysis and Product  Engineering in WaferTech LLC.


[1] R.B. Marcus, T.T. Sheng Transmission Electron  Microscopy of Silicon VLSI Circuits and Structures (Wiley, New York, 1983), Chap. 5, P.124.


[2] W.T. Chang, T.E. Hsieh, G. Zimmermann and L. Wang   J. Vac. Sci. Technol. B Vol.25, No. 1, pp.202-207, January 2007.


[3] D.R. Turner, J. Electrochem. Soc.107, 810 (1960).


[4] Dinesh C. Gupta, Semiconductor Fabrication: Technology and Metrology (ASTM International, 1989), P.126-148.


[5]  R.L. Chiu, P.H. Chang and C.H. Tung, J. Electrochem. Soc.142, 525 (1995).


DOI: 10.1361/cp2008istfa168


A New Method of Wafer Level Plan View TEM Sample Preparation by DualBeam


Hyoung H. Kang,  Michael A. Gribelyuk, Oliver D. Patterson, and Steven B. Herschbein


IBM Microelectronics, 2070 Route 52, Hopewell Junction, NY, 12533


hhkang@us.ibm.com


Corey Senowitz


FEI Company, 5350 NE Dawson Creek Drive, Hillsboro, OR  97124


There is a high level of interest on the 300mm wafer  processing line in obtaining defect analysis with fast turn  around time, while preserving wafers [1]. As the size of killer  defects continues to shrink, conventional in-line  characterization methods are failing to provide answers  required by the semiconductor industry. Transmission electron  microscopy (TEM) is becoming more important than ever for  obtaining high resolution images and high materials contrast. Cross-sectional style TEM sample preparation techniques by  DualBeam (SEM/FIB) systems have been introduced, and are  widely used in both laboratory and manufacturing lines with  either in-situ or ex-situ lift out methods. By contrast, however, the plan view TEM sample has only been prepared in the  laboratory environment, and only after breaking the wafer.


In this paper we introduce for the first time a new  methodology for in-line, plan view TEM sample preparation at  the 300mm wafer level that does not require breaking the  wafer.  This novel TEM sample preparation technique allows  investigation of in-plan defects that are not otherwise easily  imaged.


Both FIB and TEM cross sections have been used to identify  electrically open defects successfully. In-line DualBeam is  being used for fast learning on electrically open and short  defects at metal level [2]. However, root cause analysis of  electrically short defects at contact array level is more  challenging. Using electron beam inspection and focused ion  beam tools along with special test structures to shorten the  learning cycle for elimination of short defects for SOI  technology was previously presented [3]. The benefit of this  technique on electrically short defects is presented later in this  paper.


A scanning transmission electron microscopy (STEM) detector can be added to in-line DualBeam systems. The inline, low acceleration voltage STEM running at 30keV allows  high resolution imaging and high material contrast for defect  analysis. Thin lamella TEM sample preparation and defect  observation can be done in one system so that very fast  learning is possible.


Methods of plan view TEM sample  preparation


The methodology of thin lamella TEM sample preparation for  plan view work in two different tool configurations is  presented. The first tool configuration is an FEI DA300 in-line  DualBeam system with an Omniprobe 200 in-situ sample lift  out system. The second tool is an FEI DA300 with a STEM  detector. The system with STEM detector has a pre-tilted  holder that allows top down STEM imaging. The detailed  procedure of thin lamella sample preparation is described in  the following section. A KLA eS32 electron beam inspection  tool was used for detection of the bright voltage contrast  defects shown in this paper.


Using conventional tilting stage method (without  pre-tilted holder)


Stage tilt in the conventional DualBeam system is limited due  to the complexity of tool configuration. The TEM sample  holder is located at the edge of wafer normal to the wafer. The  limit of the stage tilt and TEM sample holder angle makes it  difficult for plan view thin lamella TEM sample preparation in  a full wafer DualBeam system. However, by using the in-situ  lift out needle with several welding and cutting processes at  certain stage angles, we can quickly prepare plan view TEM  samples inside of the tool. The schematic and representative  images of key steps are shown in figure 1.


First, a chunk sample is prepared by angled ion beam, and the  sample is cut free.  The sample stays at 45 degree stage tilt for  the first sample lift out step (1). The in-situ lift out needle is  inserted, and the sample is now locally welded by metal  deposition on the needle and lifted out (2). In-line DualBeam  systems use tungsten metal deposition. While the needle is  holding the chunk sample, the stage is tilted back to 0 degrees. The stage is driven outside where the chunk sample was  prepared. The sample is lowered down to the surface carefully. Local Tungsten deposition is applied at the side of the chunk  sample to hold it lightly to the surface. The needle is now cut  and released from the chunk (3). The stage is tilted to the  angle where the surface is parallel to the electron beam. This  gives good control to make thin and uniform lamella sample  later (4). Tilt the stage back to 45 degrees. Insert the in-situ


needle to the chunk and weld again. Cut the local deposition  which is holding chunk on the wafer surface. Lift out the  chunk from the surface (5). Move the chunk to the TEM grid  location. Tilt the stage to 0 degrees where the grid is parallel  to the electron beam. Insert the needle to the TEM grid and  attach the chunk to the grid. Cut the needle free (6). The thin  lamella is prepared by top down ion beam at 52 degree stage  tilt (same as the regular cross section lamella sample  preparation). The TEM grid is then transported to off-line  TEM lab for further investigation.


Fig.1 Schematic and representative images of plan view TEM  sample preparation with non-tilted stage


Using pre-tilted holder method for in-line STEM  work


An in-line STEM system provides the ability to obtain quick  defect images on the manufacturing floor with high resolution. Bright field images, as well as dark field images, can be  achieved, providing superior materials contrast compared to  conventional secondary electron images. Due to the location  of the lamella sample and STEM detector, the TEM grid  holder pre-tilted to an angle of 38 degrees in the system.  That


allows attaching the chunk sample to TEM grid in a simple  fashion.


The schematic plan view lamella sample preparation method  using a DA300 STEM with pre-tilted holder is shown in figure


2. The chunk is prepared in the same fashion as the previous  method. The chunk is lifted out by in-situ needle at 0 degrees  stage tilt. Then the stage is tilted to 52 degrees. The chunk is  welded on the TEM grid at 52 degrees where the SEM is  normal to the top of the chunk surface (1). For thinning the  lamella the stage is tilted to 14 degrees, where the ion beam is  parallel to the lamella (2). The thin lamella TEM sample can  be observed simply by tiling stage to 52 degree and switching  detecting mode (3).


Fig.2. Schematic of plan view lamella sample preparation  with pre-tilted holder


This method using a pre-tilted TEM holder allows the lamella  thickness to be monitored and final lamella location to be  easily found. An operator can repeat steps 2 and 3 to reach  good thickness for STEM work.


Examples of plan view (S)TEM work


The isolation and analysis of short circuit defect types is more  challenging than opens because much less is known about  their location, size and direction. The plan view imaging  method has proven very effective in isolating short defects. The general location of these defects is first identified using  electron beam inspection at the post tungsten CMP level [3]. Two types of short defects observed by electron beam  inspection are introduced in this paper as examples of the  benefit of using in-line plan view TEM sample preparation.


Contact array to poly short


Two critical dimensions, contact size and contact to gate stack  space, define the process window for the contact process,  If  contacts are too small, contact opens result.  If contacts are too  large, then contact to gate shorts result.   Development of this  process is one of the key challenges for all future technologies.   In order to assist in this work for both bulk and SOI  technologies, contact array voltage contrast test structures  have been developed.   The diagram for a contact to gate  shorts test structure is shown in figure 3. This test structure  was designed to run experiments with various contact to poly


spaces [4], A bright voltage contrast signal appears where a  normally floating contact touches the poly line.


Fig. 3 Test structure specifically designed for detection of  contact (CA) to poly (PC) shorts.  The poly is grounded.


Figure 4 shows the SEM image seen upon locating the defect  site with the DA300 system. We used the non pre-tilted holder  method for the preparation of a plan view thin lamella for this  defect.


The TEM observation shows very good quality of TEM  sample over a large area. The thin lamella area in this example  is about 4um x 2 um as shown in figure 5 (top image). One  lamella can contain over 250 contacts for the statistical  analysis of the contact array distribution. The bright defect in  figure 4 reveals one contact is located too close to the poly  line causing the short as shown in figure 5 (bottom image). This plan view image provides the overall location of the  contact array with respect to the poly line. The results show  the location of the contact array is unsymmetrical. The  distance ratio from the poly line to the contact on each side is


0.78:1 for this sample. The distribution of the shape and size  of contacts also can be studied for process control of the  contact array level.


Fig.4. SEM image showing the bright voltage contrast signal  which indicates  a contact to poly  short


Fig.5. (top) low magnification image shows the area of thin  lamella is about 4 µm × 2µm, (bottom) TEM observation of  in-plan defect. A contact is located too close to poly line.


Silicide encroachment defect


The second example is a silicide encroachment defect. Plan  view (S)TEM analysis is very useful for understanding silicide  defects. . The electron beam inspection tool detected a bright  contact within the SRAM as shown in figure 6 (top image). A  thin lamella TEM sample was prepared using the pre-tilted  holder method. And the defect image was obtained by STEM  observation at 30keV in a DA300 STEM system. Figure 6 (bottom image) shows the defect between the contact and poly  line where potentially Nickel Silicide (NiSi) encroachment is  occurring. Figure 7 shows Energy Dispersive X-ray (EDX) mapping results. The Ni elemental map shows the


corresponding area of the dark contrast in figure 6 (bottom) contains higher Ni concentration, confirming that the defect is  NiSi encroachment.


The plan view image shows the NiSi defect in figure 6 is  formed offset from the contact. Using a cross sectional thin  TEM lamella this NiSi defect may not have been captured. The plan view study also shows other the potential NiSi  defects within this SRAM structure as indicated by arrows in  the bottom image of figure 6.


Fig.6. (top) Short detected by electron beam inspection, (bottom) Plan View STEM observation of NiSi encroachment  defect by in-line DualBeam STEM system


Fig. 7 EDX analysis shows the high Ni contents at the defect. It is NiSi encroachment defect causing the short between poly  and contact array.


In-line, full wafer plan view (S)TEM provides a quick turn  around solution for defect analysis in the manufacturing line. This novel lamella preparation technique allows investigation  of in-plane defects and is particularly beneficial for analysis of  shorts detected with voltage contrast inspection. Two  examples were presented, isolation of contact to poly shorts  within a voltage contrast test structure and isolation of silicide  encroachment shorts within bulk SRAM


This work was performed at the IBM Microelectronics  Division, Hopewell Junction, NY 12533 and at FEI Company, 5350 NE Dawson Creek Drive, Hillsboro, OR  97124.


[1] N. Bicais-Lepinay, F. Andre, S. Brevers, P. Guyader, C. Trouiller, L.F.Tz. Kwakman, S. Pokrant, D. Verkleij, R. Schampers, L. Ithier, E. Sicurani, C. Wyon, “In-line TEM  Sample Preparation and Wafer Return Strategy fo Rapid  Yield Learning” Proc. of SPIE, p. 615217, 2006.


[2] M. Schmidt, H. Kang, L. Dworkin, K. Harris, S. Lee, ”New methodology for ultra-fast detection and  reduction of non-visual defects at the 90nm node and  below using comprehensive e-test structure infrastructure  and in-line DualBeam FIB”, Proceedings of ASMC, pp.12-16, May 2006.


[3] O. D. Patterson, H. Kang, J. Strane, C. Lavoie, K. Barth, X. Ouyang, K. Wu, “Detection and Verification of  Silicide Pipe Defects on SOI Technology using Voltage  Contrast Inspection”,  ISTFA 2007


[4]  O. D. Patterson, H. H. Kang, K. Wu, P. Feichtinger, “InLine Process Window Monitoring using Voltage Contrast  Inspection”, Proceedings of ASMC, pp. 19-24, May 2008.


DOI: 10.1361/cp2008istfa172


Embedded Gold Markers for Improved TEM/STEM Tomography Reconstruction


Jian-Shing Luo, Chia-Chi Huang, and Jeremy D. Russell


Physical Failure Analysis Department, Inotera Memories, Inc., Taoyuan, Taiwan, Republic of China


The rapid advances in nanotechnology and the decreasing size  of features in the microelectronics industry have generated a  need for advanced characterization with high spatial resolution  in two (2D) and three dimensions (3D). As a result, the  demands for physical failure and materials analysis using the  transmission electron microscope (TEM) and the scanning  transmission electron microscope (STEM) are rapidly  increasing in areas such as thickness measurement, small  defect identification, and chemical element analysis.


Sample preparation is a crucial step in successful TEM or  STEM analysis. In addition, artifacts such as amorphous layers  and overlapping interfaces in small vias become more  significant as the dimensions of the TEM samples increase  relative to the decreasing device dimensions [1]. Electron  tomography (ET) provides a way to reconstruct a 3D object  from a series of 2D projections. ET offers an intermediate  resolution of about 1 nm with a field of view of hundreds of  nanometers, making it ideal for the characterization of many  nano-scale devices [2]. Previous studies [3-6] evaluated the  capabilities, applications, and limitations of bright field (BF) TEM and high-angle annular dark field (HAADF) STEM  tomography for 3D structural characterization.


Cross-correlation and Feature Tracking


Electron tomography includes four main steps: tomography  data acquisition, image processing, 3D reconstruction, and  visualization. After acquisition, tilt-series alignments are  performed to refine the relative image shifts and tilt-axis  orientation using image-processing software. The acquired tiltseries must be precisely aligned with the tilt axis to minimize  the blurring of small features and artifacts in the  reconstruction. Two methods are used to align the tilt-series: cross-correlation and feature tracking. The advantage of  cross-correlation alignment is its simplicity compared with the  feature tracking method. According to previous studies [4], satisfactory alignment results can be obtained if no image  distortions are present. However, in the case of thick samples, where the image features change drastically during tilting, the  interactive cross-section might not align when using crosscorrelation, but will align when using feature tracking. Feature  tracking enables the correction of x-y shifts and the average  tilt-axis orientation, and also allows image orientation and  magnification changes to be measured and compensated for.


This provides a more accurate image alignment in the case of  image distortion.


Fiducial Markers


Normally, about 10-20 nm of fiducial markers, such as gold  beads, are deposited onto one side of 100 mesh carbon-coated  grids during the feature-tracking process. Next, a 100-200 nm  thick TEM specimen (which was prepared by a dual beam  focused ion beam (DB FIB) system) is attached to the same  side of the carbon film as the fiducial markers using lift-out  techniques [7], as shown in Fig. 1(a). For traditional ET  samples, a distance of approximately 10-100 nm separates the  TEM specimen and fiducial markers, as shown in Fig. 1(b). This distance is based on the shape and thickness of the  specimen. Normally, the specimen is at the eucentric height  during ET analysis. Each point of the specimen describes a  circular motion around the tilt axis during tilting, with a radius  equal to the distance between the location of the tilt axis and  the point where we are actually looking, the optical axis (as  shown in Fig. 2(a) [8]). Ideally, the distance between the tilt  and optical axes is zero. As noted earlier, the distance between  the specimen and fiducial markers is from 10 to a couple  hundred nanometers. Therefore, the circular motion paths of  fiducial markers are longer during sample tilting compared  with each point in the specimen, as shown in Fig. 1(b), resulting in a change in focus and image shift problems [8]. This can make fiducial markers difficult to track or possibly  even disappear, especially with higher magnifications, thicker  samples, and higher tilt angles.


In addition, tomography images acquired from traditional flat, thin sections are incomplete because projection images cannot  be acquired from the range of directions lying close to the  plane of the sample. The lack of information at high tilt angles  is referred to as the missing wedge problem [3]. A cylindrical  or pillar specimen might offer a solution to this problem  because it can be rotated and imaged through a full 360 degree  range with no change in the electron path length through the  specimen. Furthermore, pillar samples eliminate the effect of  the carbon film on image quality and compositional analysis. However, it is difficult to deposit fiducial markers onto the  pillar specimen for the feature tracking process. In this paper, we present a new method for preparing electron tomography  samples with gold beads inside to improve the feature tracking  process and quality of 3D reconstruction.


Figure 1: (a) An optical image showing the traditional electron tomography sample. (b) A schematic diagram showing a distance, approximately 10 -100 nm, separating the TEM specimen and fiducial markers due to the sample shape and thickness in (a).


Figure 2: Schematic diagram showing the motion trace when an object is (a) at eucentric height, and (b) not at eucentric height, which causes a change in focus and image shift problems when the sample is tilted.


Procedure of Novel Electron Tomography Sample  Preparation


The first step of our method is to use a DB FIB to mill two  trenches approximately 2 μm square and 1 μm deep next to the  device or structure of interest to trap the deposited gold beads, as shown in Fig. 3(a). For via barrier layer evaluation, samples  were taken from a wafer processed until just after the barrier  layer was deposited into the contact holes. In this case, it was  not necessary to mill two trenches. The second step is to use a  syringe to drop a few droplets of protein solution with 10 nm  gold beads onto the sample surface, as shown in Fig. 3(b). The  third step is to drop an organic chemical solution onto the  sample surface to rinse out the organic or biological materials  of the protein solution. This is then coated with a thin layer of


epoxy, as shown in Fig. 3(c). After curing, the sample was  ready to fabricate an electron tomography sample using lift  out. A TEM lamella was thinned to a thickness of 100 to  200 nm using the DB FIB system, then deposited that on a  carbon film by ex-situ lift out. This technique is described in  detail elsewhere [7].


For our pillar type of electron tomography sample, the sample  preparation procedure is almost the same as above. The  difference is to replace the ex-situ lift out method with a pillar  TEM sample preparation method [9-10]. A TEM pillar sample  on the half Cu ring is shown in Fig. 4.


Figure 3: (a) Use the DB FIB system to mill two trenches  approx. 2 μm square and 1 μm deep next to the area of  interest. (b) Deposit the gold beads onto the sample surface. (c) Cover the gold beads and sample surface with a coat of epoxy.


(d) Deposit a Pt protection layer using the DB FIB system.


Figure 4: A BF-TEM image showing a TEM pillar sample  with an unfilled CB W via on a half Cu ring.


Electron Tomography


Electron tomography data was acquired on an FEI Tecnai F20  field emission TEM with a STEM system using the XPlore3D  tomography suite. For BF-TEM tomography, no objective  aperture was used to minimize the influence of diffraction  effects [4]. For STEM tomography, a small camera length of  70 mm was used to minimize diffraction effects for the  HAADF-STEM signal collection. Scanned images with  1024x1024 pixels were acquired using a frame time of 15-30  sec. Approximately 100-200 (S)TEM images with 1024x1024  pixels were acquired automatically over a tilt-range of more  than +/-60° in 1° steps. After acquisition, tilt-series alignments  were performed to refine the relative image shifts and tilt-axis  orientation using Inspect3D software. The 3D volume was  reconstructed using the simultaneous iterative reconstruction  technique (SIRT) in Inspect3D software. The result was  visualized by volume rendering using Amira software [3, 4].


This new sample preparation method described above was  used to characterize advanced dynamic random access  memory (DRAM) devices. Three examples are described here  to demonstrate the results. The first two examples evaluate the  barrier layer’s step coverage in a contact via hole. Example 1  uses a “contact to substrate” (CS) via; Example 2 uses a “contact to bit line” (CB) via.


BF-TEM tomography can be used to characterize the structure  of semiconductor devices with amorphous or weakly scattering  crystalline materials, such as seed and diffusion barrier layers  in unfilled metal vias [4]. Therefore, these two examples were  investigated using BF-TEM tomography. Example 3 is  performed on a W CB via and transistor gate device (GC) using HAADF-STEM tomography. All examples are from the  array structure of a DRAM (Figs. 5, 7, and 10), except the CS, which is in the periphery (Fig. 6).


Figure 5: A BF-TEM image showing the bit line (M0), borderless contact (CB), deep trench (DT) capacitor, transfer  gate (GC), and active area (AA) structures (n-type) of the  advanced trench DRAM.


(I) Barrier layer


Fig. 6(a) shows a BF-TEM image of the TiN barrier layer in  an unfilled W CS via, including the gold beads on the sample  surface and a via inside using our new electron tomography  sample preparation with ex-situ lift out. After image  processing and reconstruction, a 3D image of the via liner’s  profile was visualized by volume rendering, as shown in Fig. 6(b). Both the gold breads and barrier layer profile were  clearly shown in the 3D tomography reconstruction rendering  volume. By using x-y orthogonal slices through the 3D  reconstruction volume, the step coverage can be more easily  identified, as shown in Fig. 6(c, d).


One additional benefit of our new method is that the beads  inside the unfilled W via can be a calibration reference for the  thickness measurement of the barrier layer through the 3D  reconstruction rendering volume of the via, as shown in Fig. 6(c, d). The accurate bead size can be obtained by traditional  BF-TEM, as shown in Fig. 6(a). Fig. 7 shows a pillar type of


Pillar


Cu half ring


electron tomography sample prepared with gold beads inside  an unfilled CB W via using our new ET sample preparation  method. From the BF-TEM image, approximately 20 gold  beads were successfully embedded around the device. Unlike  the traditional ex-situ lift-out of ET samples, our method  isolated a single CB contract in our pillar sample, as shown in  Fig. 7(b). Also, the automatic recentering and refocusing of the  sample after tilting are quite smooth on our pillar sample  during tilt series acquisition for both BF-TEM and HAADFSTEM tomography, even at higher tilting angles, e.g., 70  degrees. Traditional samples would require manual focus or  recentering when using higher tilting angles during acquisition. The probable reason is the increased specimen thickness along  the electron beam direction with tilting angle, which results in  poor cross correlation quality causing recentering and  refocusing failures. The resulting 3D tomography   reconstruction renders volumes with feature tracking that are  better than those without feature tracking, as shown in Fig.


8(a, b). The CB bottom liner profile is clear when using x-y  orthogonal slices through the 3D reconstruction volume, as  shown in Fig. 8(c, d). This information is not obvious in the  BF-TEM image, as shown in Fig. 7(b). Another solution to  reduce the problem of this missing wedge [4, 11] is to use the  dual axis tomography holder without full 360 degrees rotation. This provides two tilt series recorded with mutually  perpendicular tilt axes. However, the half Cu ring might block  the sample during tilting along the pillar at higher angles, as  shown in Fig. 9. To overcome the blocking problem, we  developed a new pillar sample preparation method using  dicing saw. The details of this will be described in a future  publication.


Figure 6: (a) BF-TEM image and (b) 3D tomography reconstruction rendering volume of a via barrier layer with gold beads inside (c, d) series of x-y orthogonal slices show the barrier layer’s step coverage across the via. In all images, the dark, gold beads are  visible.


Figure 7 (a) A BF-TEM image showing a TEM pillar sample with an unfilled CB W via. (b) An enlarged BF-TEM image on the tip  of pillar in (a).


Figure 8: 3D tomography reconstruction rendering volume of a CB via barrier layer with gold beads inside (a) using feature  tracking (b) cross correlation only (c, d) series of x-y orthogonal slices showing the barrier layer’s step coverage across the via.


Figure 9: A tilted BF-TEM image showing a TEM pillar  sample with an unfilled CB W via at (a) 46, (b) 47, and (c) 48  degrees along the pillar direction.


(II) W via


For HAADF-STEM tomography, Fig. 10 shows an example of  a TEM pillar sample prepared by our new electron  tomography sample preparation method, with a CB via and  two GC stacks of a DRAM array structure. From the TEM and  STEM images, 20 gold beads were embedded in milled  trenches around the device. Fig. 11(a) shows the results after  the first “auto” tracking and “solve” steps. From the total bead  result errors, no obvious jumps occurred, as shown in Fig. 11(b). During bead correction, embedded beads are easy to  track and correct. After bead correction, the 3D tomography  reconstruction rendering is shown in Fig. 11(c) after applying  the alignments and 3D reconstruction on a raw series of 2D  images.


Figure 10: (a) BF-TEM (b) HAADF-STEM image shows the  structures of AA, M0, GC, CB, and DT surrounding with gold  beads and epoxy.


Half Cu ring


Figure 11: (a) An inversed STEM image with blue solution  circles (b) The results of total error per bead after first “autotracking” and “solve” steps (c) 3D tomography  reconstruction rendering volume in (a).


We have shown that our new electron tomography sample  preparation method improves image alignment, which is  essential for successful tomography in many contemporary  semiconductor device structures. We have also successfully  applied a modified version of the technique to deposit gold  beads onto TEM pillar samples for improved 3D  reconstruction.


The authors would like to thank Wendy Hsu and Teresa Lee  for their support in sample preparation.


[1] Mardinly, A.J. “Electron Tomography and ThreeDimensional Aspects of Transmission Electron  Microscopy,” Electronic Device Failure Analysis, Vol. 7, No.3 (2005), pp. 6-12.


[2] Midgley, P.A. and Weyland, M., “3D Electron  Microscopy in the Physical Sciences: the Development of  Z-contrast and EFTEM Tomography,” Ultramicroscopy  96 (2003), pp. 413-431.


[3] Kubel, C., Kubel, J., Kujawa, S., Luo, J.S., Lo, H.M., and  Russell, J.D., “Application of Electron Tomography for  Semiconductor Device Analysis,” Eighth International  Workshop on Stress-Induced Phenomena in Metallization, AIP Conference Proceedings, Vol. 817 (2006), pp. 223-228.


[4] Kubel, C., Voigt, A., Schoenmakers, R., Otten, M., Su, D., Lee, T.C., Carlsson, A., and Bradley, J., “Recent  Advances in Electron Tomography: TEM and HAADFSTEM Tomography for Materials Science and  Semiconductor Applications,” Microscopy & Microanalysis Vol. 11 (2005), pp. 378-400.


[5] Kimura, K., Hata, S., Matsumura, S., and Horiuchi, T., “Dark-Field Transmission Electron Microscopy for a Tilt  Series of Ordering Alloys: Toward Electron  Tomography,” Journal of Electron Microscopy, Vol. 54, No. 4 (2005), pp. 373-377.


[6] Luo, J.S., Russell J.D., Huang L.Y., and Chen T.P., “Applications of Electron Tomography on Advanced  DRAM,” 33rd International Symposium for Testing and  Failure Analysis (2007), pp. 115-120.


[7] Bicais-Lepinay, N., Andre, F., Pantel, R., Jullian, S., Margain, A., and Kwakman, L.F.T., “Lift-Out  Techniques Coupled with Advanced TEM  Charaterization Methods for Electrical Failure Analysis,” Microelectronics Reliability, Vol. 42, No. 9, (2002), pp. 1747-1752.


[8] FEI Company (2008). “Advanced Tecnai TEM software  for easy acquisition, reconstruction and visualization,” from http://cryoem.ucsd.edu/microscopes/polara_docs/ tomography_functional_description.pdf.


[9] Yaguchi T., Kamino T., Ohnishi T., Hashimoto T., Umemura K., and Asayama K., “FIB Micro-pillar  Sampling of Si Devices and Its 3D Observation,” Proceeding from the 29th ISTFA Conference (2003), pp. 282-296.


[10] Fukuda, M., Tomimatsu, S., Nakamura, K., Koguchi, M., Shichi, H., and Umemura, K., “A new FIB Fabrication  Method for Micropillar Specimens for Three-dimensional  Observation Using Scanning Transmission Electron  Microscopy,” Journal of Electron Microscopy 53(5) (2004), pp. 479-483.


[11] Penczek, P., Marko, M., Buttle, K., and Frank, J.,


“Double-tilt Electron Tomography,” Ultramicroscopy 60


(1995) pp. 393-410.


DOI: 10.1361/cp2008istfa180


Timing Sensitivity Analysis of Logical Nodes in Scan Design Integrated Circuits  by Pulsed Diode Laser Stimulation


T. Kiyan, C. Boit


Berlin University of Technology, D-10587 Berlin, Germany   tkiyan@mikro.ee.tu-berlin.de , +49-30-314-29954


C. Brillert


Infineon Technologies, D-81739 Munich, Germany


In this paper, a methodology based upon laser stimulation and  a comparison of continuous wave and pulsed laser operation  will be presented that localizes the fault relevant sites in a  fully functional scan chain cell. The technique uses a laser  incident from the backside to inject soft faults into internal  nodes of a master-slave scan flip-flop in consequence of  localized photocurrent. Depending on the illuminated type of  the transistors (n- or p-type), injection of a logic ‘0’ or ‘1’ into  the master or the slave stage of a flip-flop takes place. The  laser pulse is externally triggered and can easily be shifted to  various time slots in reference to clock and scan pattern. This  feature of the laser diode allows triggering the laser pulse on  the rising or the falling edge of the clock. Therefore, it is  possible to choose the stage of the flip-flop in which the fault  injection should occur. It is also demonstrated that the  technique is able to identify the most sensitive signal  condition for fault injection with a better time resolution than  the pulse width of the laser, a significant improvement for  failure analysis of integrated circuits.


Scanning the device with a 1064 nm wavelength laser beam  stimulates the active devices because of photocurrent  induction due to electron-hole pair generation. As a second  order effect, light absorption in interconnects may cause local  heat production, which can affect the sheet resistance of the  current path, temporarily altering the transistor characteristics. Several techniques have been developed using this effect in  dynamically driven integrated circuits (ICs) like LADA (Laser  Assisted Device Alteration) [1] and Delay Variation Mapping (DVM) [2]. LADA technique is also applied to SRAM (Static  Random Access Memory) structures to inject soft faults [3].


Single Event Upset Testing has been performed using a femto  second power laser [4-8]. Simulation models are developed  for better understanding of fault injection phenomena and the  upsets in SRAMs are simulated by using these models [9-10]. Design for Testability is mostly taken into consideration for  the design of modern ICs. Lock-in assisted soft defect  localization is introduced which localizes soft defects in scan  chain design circuitries [11-12].


The ideal stimulation would be done with a laser pulse that is  tunable in intensity and delay with respect to clock and scan  pattern in order to get maximum precision of the time  information when the circuit is most sensitive to fault  injection. This investigation uses a 1064 nm laser diode, which is dynamically triggered by the tester, very convenient  to adjust to the internal signal sequence and scan flip-flops are  exposed from the backside causing soft fault injection.


Experimental Set-up


The experimental set-up is shown in Fig. 1. Principally, we  use PHEMOS 1000 as a laser stimulation system for our  experiments. It has NIR laser light source and laser scanning  synchronization system synchronizing the position of a laser  beam with the electrical variations of the device under test. A  1064nm wavelength, 200 mW power laser is used for the  perturbation of the devices. The laser can operate in  continuous wave (CW) and pulsed mode. The pulse width can  be minimum 50 ns with 50 KHz repetition rate. The pulse  width and the frequency can be tuned by an external pulse  generator and shifted to the appropriate time slots through test  pattern. For our investigations, we also used 10ns laser pulse  length, although it is out of pulse width range specified by the  provider.


The device under test (DUT) is driven by Agilent 83000  tester. The laser pulse is triggered by Automatic Test  Equipment (ATE) and it is synchronized with the scan-in and  scan clock signal. The output of the scan chain is fed into a  Hamamatsu Dynamic Analysis of Laser Stimulation (DALS) Kit if the scanning mode is used. DALS employs an analog  integrator to integrate the output signal of the device per pixel  and therefore it can detect any electical change in the signal, for example duty cycle, amplitude, frequency or a missing  pulse if it changes the integrated signal. The DALS signal is  converted to a gray scale image by the image acquisition card  of PHEMOS 1000, while the laser is scanning an area. The  reflected laser light from the device is also collected by a  detector and these two images are overlaid for the localization. Moreover, the laser beam is positioned on a single point and  the output signal is analyzed at a LeCroy 6 GHz bandwidth  oscilloscope for more detailed investigations.


Figure 1: Experimental Set-up


Device Under Test


The DUT is produced in 90 nm technology and it is provided  by Infineon AG. We have chosen a scan chain which has 259  scan flip-flops and there is inversion between the scan-in and  the scan-out signals. A scan shift vector pattern is applied  which runs in a loop continuously. The scan flip-flops operate  in scan mode which means that they form a 259 long shift  register. The scan chain is addressed starting from 258 to 0. Flip-flop 0 is the closest to the output.


The schematic of one scan flip-flop is seen in Fig. 2. It is a  rising edge triggered two stage master-slave flip-flop. There is  a mux selecting the data or test-in input by a Test Enable (TE) pin. The master stage is driven by the inverted clock signal, while the second stage is driven by the clock signal. Therefore, the first stage is low level sensitive, while the  second stage is high level sensitive.


Figure 2: The schematic section of one scan flip-flop


The nominal operating voltage of the DUT is 1.2 V. We  decreased the supply voltage down to 0.715 V in order to have  stronger laser stimulation effect on timing, both in cw mode  and pulsed mode.


Continuous-wave Laser Stimulation


CW laser is utilized and a 128x128 pixel area is scanned. 50x  lens is used and a scan flush pattern, {001100…}, is applied  to the DUT, which is shifted in with a clock frequency of 2  MHz. The gray and overlaid images are seen in Fig. 3. Each  group of 3 spots indicates one scan flip-flop. The colors of the  spots in the right side of the image are inverted in respect to  the left side since there is an inverter between these two  groups of scan flip-flops.


The laser beam is positioned on white and black spots in  single spot mode and it was observed that when white spots  are exposed, the scan-out stays at logic high while the black  spots cause the scan out to be logic ‘0’. The output does not  switch anymore. It means that positioning the laser on a white  spot causes a stuck-at-one like fault, while black spots behave  like a stuck-at-zero fault.


Figure 3:The gray and the superimposed images (derived by  overlaying gray image on the reflected laser light


micrograph) for cw laser


If there is a stuck at fault in a circuitry, one way is to do a  reset operation to locate the problem. After reset, the first scan  shift pattern is applied. In this case, the reset pattern should


Laser Pulse Trigger  scan-out  DUT


input


stimuli


ATE


Scanner


Image


Processing


Unit


Detector   Laser


DALS Kit


Digital


Oscilloscope


come out. But if there is a defect, the faulty pattern will be  shifted out indicating the location of the stuck-at fault. One  can only localize one type of stuck-at faults, stuck-at-one or  stuck-at-zero with this technique. For example, if the reset sets  the scan flip-flops to ‘1’, then it would not be possible to  localize stuck-at-one faults. In some circuits, even the reset  operation is not available [13].


The CW laser stimulation technique presented here allows  locating both types of faults without any need of reset  operation. If there was a stuck-at fault in the middle of the  chain, scanning the device with laser beam would not change  the output when the flip-flops before the defect are  illuminated. Soft fault injection would be observable only if  the flip-flops after the break are exposed which points out the  location of the defect.


The intensity-laser power diagram for the three spots, which  are marked in Fig. 3, is seen in Fig. 4. The intensity depends  on the scan speed and the numbers of the frames that are  integrated. In this case, 10 frames were taken and the scanning  speed was 33 s/frame for a 128x128 pixel area. The intensity  is calculated by the image acquisition card qualitatively and it  just demonstrates the strength of the spots. It is not possible to  assign any voltage levels to the spots. The graph shows that  the strongest stimulation occurs when the laser hits the 1st site  although the intensity for the 2nd and the 3rd spots are weak. We assume that the minimum required laser energy to cause  an upset depends on the logic and the layout design of the  circuitry. In our previous work [14], the fault injection  occurred only when the laser beam hit the 1st site. After  exchanging the laser diode, the laser power increased by 43%. As a result, fault injection happens additionally in two areas, which gives a better insight into DUT operation.


Figure 4: Intensity-Laser Power diagram for three different  spots


Analysis of the Sensitive Sites


The superimposed image is overlaid on the layout of the  circuitry and the sensitive structures in a scan flip-flop to the  soft fault injection are acquired. These sensitive structures are  numbered in Fig. 3. The first and the second spots are related  to the reset and clock-controlled inverter and the transfer gate  in the master stage while the third one is in the clockcontrolled inverter and transfer gate of the slave part.


The schematic section of the sensitive circuitry in the master  stage is shown in Fig. 5. The node, which is pointed in Fig. 5, changes its state from high to low or from low to high  depending on the illuminated site. If the sensitive node is logic  low, there will be an upset when the pMOS-network in the  clock and reset controlled inverter is exposed and it will cause  1st spot to appear. If the sensitive node is logic high, it will  toggle to logic low once the laser beam hits the nMOSnetwork in the clock and reset controlled inverter, which will  make the 2nd spot to become visible. Mn1, Mn3, Mn4, Mn5  transistors are situated in the same active area as well as Mp1, Mp3, Mp4, Mp5. The overlay of the spots on the layout  proves that the drain terminals of Mp5 and Mn3 transistors are  the most sensitive to fault injection.


Figure 5: The schematic section of the sensitive structures in  the master stage


Figure 6: The schematic section of the sensitive structures in  the slave stage


The schematic section of the sensitive structure in the slave  stage is seen in Fig. 6. When the laser hits the drain of the  Mn9 and Mn6, the sensitive node flips from logic ‘1’ to ‘0’ which in turn causes the 3rd spot to become visible.


Sensitive  node


Pulsed Laser Stimulation


The laser pulse is triggered by tester with a pulse width of      50 ns and a signal frequency of 48 KHz. A scan shift pattern,


which has a 48 KHz signal frequency, is applied to DUT and


it is shifted in with 2 MHz scan clock signal.


At first, the laser pulse is triggered at the rising edge of the


clock and a 128x128 pixel area is scanned pixelwise. As a


result, the gray and the superimposed images are acquired


which are shown in Fig. 7. The investigations showed that


pulsing the laser at the rising edge of the clock causes


stimulation in the master stage. In this case, the 1st and the 2nd


spots become visible. When the laser pulse is triggered at the


falling edge of the clock, the n-network in the slave stage


causes a bit flip from ‘1’ to ‘0’ at the sensitive node which


causes the 3rd spot to appear.


Laser pulse is triggered at the rising edge of the clock


Laser pulse is triggered at the falling edge of the clock


Figure 7: The gray and the superimposed images for pulsed  laser triggered at the rising and the falling edge of the clock


These results prove that pulsed laser stimulation is able to  localize the defected scan flip-flop and the defected stage  within the scan flip-flop, which is not possible with ATPG (Automatic Test Pattern Generation) tools.


For further investigations, a stream that consists of only zeros, {1111…} is shifted into the scan chain and a laser pulse is  introduced to the system with a repetition rate of 48 KHz and  a pulse width of 50 ns. It is triggered at the rising edge of the  clock. In the second case, we applied {0000…} to the scan  input. The overlaid images are seen in Fig. 8. The white spots  are visible for the first image whereas there are only black  spots for the second case.


In order to probe the scan-out signal, we positioned the laser  beam on the white and black spots in single spot mode and  analyzed the output signal at the oscilloscope. As a result, we  observed a modulated scan-out signal due to the laser  stimulation. The oscilloscope images are seen in Fig. 9. Illumination of the white spots injects ‘1’ to the output stream  whereas black spots inject ‘0’ for one cycle at which the laser  pulse is triggered.


Test pattern: {1111…}


Test pattern: {0000…}


Figure 8:The overlaid images for pulsed laser


Figure 9: Laser pulse, scan clock and laser induced scan-out  pulse signals (100 ns/div)


Timing Sensitivity


The laser pulse is shifted in time to find out the time interval  in which the stimulation is the strongest. Consequently, it was  observed that there is a correlation between the intensity of the  laser induced signal and the clock to laser pulse delay. The  gray and the superimposed images are shown in Fig. 10 for


Laser pulse


Clock


Scan-out


different clock to laser pulse delays. When the delay increases, the number of the spots and their intensities decrease. Therefore, the effect is the strongest when the time delay  between the edges of the laser pulse and the scan clock is  small. The clock and the laser pulse signals are shown in Fig. 11 at which the best injection occurs for 50 ns and 10 ns pulse  width laser pulses.


delayrising(clock-laser pulse)=-4 ns


delayrising(clock-laser pulse)=6 ns


delayrising(clock-laser pulse)=0 ns


Figure 10: Gray and superimposed images for pulsed laser


Table 1: The laser pulse amplitude (laser peak power)


measured by a Tektronix SA-42 Optical to Electrical


Converter


Laser Pulse Width


Laser Power


10ns


50ns


65%


13.8mV (0.492mW)


100%


23.6mV (0.842mW)


30mV (1.071mW)


The amplitude and the laser peak power of the laser pulses for  two different laser pulse widths and laser powers are seen in  Table 1.


Figure 11: The clock and the laser pulse signals at which the


strongest injection occurs for 50 ns and 10 ns pulse width  (100 ns/div.)


delayrising(clock-laser pulse)=-6ns and the laser power is


delayrising(clock-laser pulse)=8ns and the laser power is 100%


delayrising(clock-laser pulse)=-2ns and the laser power is 65%


delayrising(clock-laser pulse)=6ns and the laser power is 65% Figure 12: The laser pulse and clock signals for 10ns laser  pulse width with different laser powers in boundary conditions (50 ns/division)


The boundary conditions of the laser pulse with respect to  clock signal are also shown in two directions for 10ns laser  pulse width and 65% and 100% of laser powers in Fig. 12. When the laser pulse is shifted further than those values, the  stimulation does not take place.


In Fig. 13, it is illustrated that the stimulated activity is  correlated to the edge of the clock signal pattern. The time  window width, in which the upset could occur, varies  depending on the laser power and the pulse width. The time  window for 10 ns pulse width and 65% power laser pulse is  narrower than 10 ns laser pulse with 100% power. Since the  laser power is higher for 50 ns width laser pulse, the time  window gets broader.


As a result, pulsed laser stimulation is able to define the most  critical point in time of a switching activity when the  minimum laser power at which the stimulation occurs. Tuning  the laser power down to the stimulation border narrows down  the effective time window.


Figure 13: The laser pulse width-delay (clock-laser pulse) diagram for different laser powers


Figure 14: The intensity versus supply voltage diagram for  white and black spots


In order to evaluate the laser stimulation intensity dependence  on supply voltage, the DUT is scanned with a scan speed of   33 s and 20 frames are integrated for various supply voltages. The intensities of the white and black spots which are marked  in Fig. 10, are calculated and an intensity-supply voltage  diagram (Fig. 14) is obtained. It shows that stimulating the


device at 0.8 V is also possible, which is a stable operating  condition regarding the jitter. Signal jitter was observed for  the working points lower than 0.715 V.


Figure 15: Scan Clock, Laser Pulse and Scan-out signals  (200 ns/div.)


laser pulse triggered at the 1.


clock pulse


laser pulse triggered at the 2. clock pulse


laser pulse triggered at the 3. clock pulse


Figure 16: The overlaid images for pulsed laser triggered at  different timing slots as indicated in Fig. 15


Localization of the Scan Flip-Flops


Pulsed laser allows triggering the laser pulse at a time of  interest and each spot can be allocated to a certain time slot in  time. We moved the laser pulse through different clock cycles.  The laser pulse is synchronized with the rising edge of the 1st, 2nd and 3rd clock pulses  (the clock pulses are numbered in Fig. 15) and the DUT is scanned pixelwise. The result-overlaid  images are shown in Fig. 16. It is shown that triggering the  laser pulse one or two clock pulses later causes the red spot to  appear at different areas. When the laser pulse is triggered  with the rising edge of the 1st clock, it stimulates the 226th flipflop while 2nd and 3rd stimulates 225th and 224th, respectively. Each red spot pinpoints related scan flip-flop. Thus, pulsed  laser stimulation on golden devices is able to localize scan  flip-flops for reverse engineering applications.


Simulations


The simulations were done by using TITAN circuit simulator  in order to reproduce the upset mechanism in circuit level. We  have used the model, which is seen in Fig. 17. A current  source, which is bypassing the drain electrode of the Mp5 and  the supply voltage, is used in order to model the additional  drain current induced by the laser illumination. The laser pulse  is modeled with a pulse in the current source.


Figure 17: The simulation model


Figure 18: The simulation results for 0.715mV power supply


Due to electron-hole generation, a photocurrent is induced  locally in reversed biased drain-bulk junction, which causes an  increase in the drain current. Consequently, this additional  drain current causes an upset.


The simulation results are seen in Fig. 18. When the input of  the scan cell is logic ‘1’, the voltage level at node X is 0 V. If  the laser pulse is triggered, the voltage at node X goes from ‘0’ to ‘1’ which causes output to flip from ‘1’ to ‘0’ for one  clock cycle.


The minimum current pulse amplitude at which the fault  injection occurs was measured with the aid of the simulations. As a result, a linear curve is obtained (Fig. 19). For the laser  diode power that we are using, it is possible to inject faults for  the supply voltages lower than 0.8 V (see Fig. 14).


Figure 19: The minimum required current source amplitude in  order to cause an upset for various supply voltages


Continuous-wave and pulsed laser stimulation on scan chains  causes soft fault injection in logical nodes of the scan flipflops, which results in the modulation of the scan-out. Using  the opportunity of shifting the laser pulse with respect to  clock, pulsed laser stimulation was successfully utilized for  time-resolved fault injection. The laser pulse is triggered on  the falling and the rising edge of the clock. It is shown that  triggering the laser pulse on the rising edge of the clock and  exposing the p-MOS network in the inverter of a master stage  injects logic ‘1’ while illumination of n-MOS network causes  logic ‘0’ injection. Hitting the n-MOS network with the laser  and pulsing the laser on the falling edge of the clock causes a  bit flip from ‘1’ to ‘0’ in the slave stage. As a result, this  technique is able to isolate the breaks in the scan chains and  also in the master or slave stages of a scan flip-flop if the  pulsed laser is used. While the ATPG tools help to localize the  defected scan flip-flop, they are not able to localize the  defected stage. It is also shown that pulsed laser stimulation  can be also used for reverse-engineering applications in  golden devices, for example to localize a desired scan flip-flop  in the chain.


Besides, pulsed laser stimulation methodology on scan chain  ICs identifies the most sensitive signal condition of a clock  driven circuitry to the laser stimulation. This information  gives a better insight into the physics of the laser stimulation  impact on the operation of a clock driven circuitry. It is  presented that the time resolution of the effective stimulation  correlates with the sharpness of the signal pattern edges and  the laser power for failure analysis applications. Therefore, the  minimum laser power needed to cause an upset in a logical  node and the laser pulse to clock delay are the decisive  parameters.


It is also presented that a current source connected to the drain  of the stimulated transistor models the additional drain  photocurrent and causes an upset in the flip-flop.


The authors would like to thank Christian Burmer (Infineon  AG Munich) for helpful discussions. Special thanks to Mr. Hiroyoshi Suzuki and Dr. Tomonori Nakamura (Hamamatsu  Photonics KK Japan) who helped integration of DALS and  1064 nm laser on PHEMOS 1000, Uwe Voss (TU-Berlin) for  his general support in tester related work.


[1] Rowlette J, Eiles T, “Critical timing analysis in  microprocessors using near-IR laser assisted device  alteration (LADA)”, Proceedings of International  Test Conference 2003, pp. 264-273.


[2] Sanchez K, Desplats R, Beaudoin F, Perdu P, “NIR  laser stimulation for dynamic timing analysis”, Microelectronics and Reliability 2005, pp. 1459-1464.


[3] Kong C. L., Castro, E., “Application of LADA for  Post-Silicon Test Content and Diagnostic Tool  Validation”, Proc 32nd Int’l Symp for Testing and  Failure Analysis, Austin, Texas, November 2006, pp. 431-437.


[4] Buchner S, Wilson D, Kang K, Gill D, Mazer J, Raburn W et al., “Laser simulation of single event  upsets”, IEEE Transactions on Nuclear Science, Vol.34 (1987), pp. 1227-1233.


[5] Buchner S, Kang K, Stapor WJ, Rivet S, “Spatial and  temporal dependence of SEU in a 64K SRAM”, IEEE Transactions on Nuclear Science Vol. 39 (1992), pp. 1630-1635.


[6] Darracq F, Beauchene T, Pouget V, Lapuyade H, Lewis D, Fouillat P et al., “Single event sensistivity  of a single SRAM cell”, IEEE Transactions on  Nuclear Science, Vol.49 (2002), pp. 387-391.


[7] Melinger J, Buchner S, McMorrow D, Dtapor W, Weatherford T, Campbell A et al., “Critical  evaluation of the pulsed laser method for single event  effects testing and fundamental studies”, IEEE  Transactions on Nuclear Science, Vol. 41 (1994), pp. 2574-2584.


[8] Pouget V, Fouillat P, Lewis D, Lapuyade H, Sarger  L, Roche F et al., “An overview of the applications of  a pulsed laser system for SEU testing”, Proceedings  of IEEE International On-line Testing Workshop  2000; pp. 52-57.


[9] Pouget V, Lapuyade H, Lewis D, Deval D, Fouillat  P, Sarger L., “SPICE modeling of the transient  response of irradiated MOSFETs”, IEEE  Transactions on Nuclear Science, Vol. 47 (2000), pp. 508-513.


[10] Douin A, Pouget V, Darracq F, Lewis D, Fouillat P, Perdu P, “Influence of Laser Pulse Duration in Single


Event Upset Testing”, IEEE Transactions on Nuclear  Science, Vol. 53 (2006), pp. 1799-1805.


[11] Burmer C, Brillert C, Qian Z, “Soft defects: challenge and chance for failure analysis”, Proc 14th  IPFA 2007, Bangalore, pp. 235-239.


[12] Qian Z, Brillert C, Burmer C, Grützner M, “Lock-in  assisted soft defect localization (LIA-SDL) and its  application in scan shift problems”, Proc 31st Int’l  Symp for Testing and Failure Analysis, San Jose, California, pp. 128-133.


[13] Crouch AL, “Debugging and diagnosing scan  chains”, Electronic Device Failure Analysis, Vol. 7 (2005), pp. 16-24.


[14] Kiyan T, Brillert C, Boit C, “Timing Analysis of  Scan Design Integrated Circuits Using Stimulation by  an Infrared Diode Laser in Externally Triggered  Pulsing Condition”, ESREF 2008.


DOI: 10.1361/cp2008istfa188


Dual Port RAM MBIST Failure Analysis using   Time Resolved Dynamic Laser Stimulation


Jonathan Shaw, Christopher McMahon


LSI Corporation, Fort Collins, CO, USA


Yin Shyang Ng, Félix Beaudoi1


DCG, Fremont, CA, USA


1 Currently with IBM, East Fishkill, NY, USA


In this paper we present the use of Dynamic Laser Stimulation (DLS) and Time-Resolved Dynamic Laser Stimulation (TRDLS) to provide fail site localization and complementary  information on a failed embedded memory IC. Memory Builtin Self Test (MBIST) is a standard method for testing  embedded memories in a System-On-a-Chip (SOC) device.  The MBIST tests are designed to provide the maximum fault  coverage for a SOC memory.  This high fault coverage comes  as a result of efficiently combining several write and read  operations.  These tests are often implemented with on chip  state machines that have little or no programmability. Very  often MBIST patterns can also be used to analyze failing  electrical signatures and often can pinpoint a fail operation and  a fail cell. However for some complex memory failure modes, even these fault optimized patterns do not provide adequate  fail site localization. In these cases, the MBIST method cannot  be adapted readily to perform in-depth electrical  characterization.


Dynamic Laser Stimulation (DLS) techniques such as LADA (Laser Assisted Device Alteration) and SDL (Soft Defect  Localization) enable spatial localization of dynamic failures [1,2]. The principle of DLS is based on test pattern pass/fail  status monitoring under Laser Stimulation. By observing the  pass-to-fail or fail-to-pass transitions, areas that are potentially  involved in the dynamic failure can be localized.  Typically, the DLS signature is created by triggering on a pass-to-fail or  fail-to-pass transition off of a specific failing vector in a  functional or scan test that ties directly to the failure being  analyzed.  However, in the case of MBIST failures the entire  MBIST test is run before a test result (pass or fail) is reported  to the tester and therefore the test results do not contain  detailed information about the failure mode.


An important extension to DLS techniques is the addition of  modulation capability to synchronize the laser beam with a  test pattern. Such a scheme would enable turning the laser on  or off during specific portions of the test sequence. This Time  Resolved DLS (TR-DLS) technique opens up a wide range of


new applications. For instance it allows searching the time  window for which the device is sensitive to Laser Stimulation. In this specific case the embedded Dual Port RAM memory IC  failed the MBIST test.  The failure signature was bitmapped  and was found to be a 4 column wide failure with randomly  distributed bits. A portion of a sample bitmap is shown in fig.


1. The 4 columns were read by a single sense amp. The most  likely failure mode was either a timing issue during either the  read or write, or an issue with the sense amp operation. However from the test results and bitmapping it was not  possible to narrow the failure mode down further. DLS was  first used to localize the failing area. Then TR-DLS was used  to target specific sequences of the MBIST pattern. The TRDLS maps that were obtained for each sequence of the MBIST  pattern clearly identified that the read operation was failing. The TR-DLS technique also provided different DLS signature  between a Port AB read and a Port B read sequence. The  signature for the Port B failure reinforced the theory that the  sense amp was the location of the failures.


Figure 1. Sample bitmap plot showing the 4 column wide


randomly failing bits for the Dual Port RAM failure.


MBIST Failure Description


An embedded Dual Port RAM within a 90nm IC failed one of  the Memory Built-In Self Test (MBIST). The first sequence of  MBIST testing used for this analysis, failed a Bit Line  Checker Board pattern consisting of 13 sequences of 37  operations per sequence. The total MBIST test pattern  sequence is quite long, approximately 3.77ms, due to other  successive non-failing MBIST sequences.


The embedded RAM being analyzed is a Dual Port RAM.  The first and second port is denoted as port A and port B. The  test data is accessed through either port A (A), port B (B) or  simultaneously through port A and port B (AB).


The qualitative MBIST test sequence is given below:


(Port A write)S1


(Port A read and write)S2


(Port AB read and Port A write)S3


(Port A read and write)S4


(Port A read)S5


(Port AB read Port A read and write)S6


(Port A read)S7


(Port B read and write)S8


(Port AB read Port A write)S9


(Port B read and write)S10


(Port B read)S11


(Port AB read Port B read and write)S12


(Port B read) S13


Further electrical characterization showed that the MBIST  failure was dependent on voltage and temperature. The Dual  Port RAM started to fail as the core power supply was  lowered. Additionally, the Dual Port RAM failed as the  operating temperature was decreased. Both failure  dependencies indicated that the Dual Port RAM may have a  timing issue that is causing the failure.


Dynamic Laser Stimulation


Dynamic Laser Stimulation makes use of a laser beam to  perturb the device under test. The laser beam is focused and  scanned using a scanning optical microscope over the area of  interest. Two types of perturbations can be induced as a  function of the laser beam wavelength.  Thermal Laser  Stimulation (TLS) is achieved using a laser wavelength above  1100nm. At such wavelength practically no photo-generation  of carriers takes place. The laser energy is converted into heat  within the device absorbing elements, causing a change in  their resistivity. Photoelectric Laser Stimulation (PLS) is  achieved using a laser wavelength below 1100nm. For such  wavelengths electron-hole pairs are generated by photon  absorption in silicon. They are dissociated at the pn junctions  in the silicon active layer, thus creating photocurrents. Both  TLS and PLS alter the dynamic behavior of ICs. Their  respective effects are strongly dependent on the nature of the  failure or the marginal behavior [3,4]


Several DLS techniques monitor the effect of laser stimulation  through the functional test status, pass or fail, of dynamically  stimulated ICs. Those are Resistive Interconnection  Localization (RIL) [5], Soft Defect Localization (SDL) [6] and  Laser Assisted Device Alteration (LADA) [7]. In those DLS  techniques a test pattern that stimulates marginal IC behavior  is looped repeatedly. The IC operation is set just on either side  of the pass/fail state limit. The laser beam is scanned across  the device surface and the pass or fail result is monitored for  each laser beam position. The corresponding pixel is colored  as function of the binary test result. Dynamic Laser  Stimulation techniques therefore detect areas sensitive to the  laser perturbation, i.e. for which the laser causes the device to  change state (fail-to-pass and/or pass-to-fail). The DLS  pass/fail approach is illustrated in fig. 2.


In Time-Resolved Dynamic Laser Stimulation (TR-DLS) a  means to modulate laser output synchronously with the test  pattern is added.  Such a scheme allows affecting the pass or  failing status of the device under test during a specific time  window of the test pattern. Timing information is thus added  to the DLS X-Y localization.


Figure 2. DLS based on the functional tests.


Experimental Setup


The failed IC was tested using a T6672 Advantest tester. The  DLS analysis is performed using the Emiscope III-gt dynamic  analysis platform from DCG Systems. The Emiscope III-gt  system integrates a Laser Scanning Microscope (LSM) with  dual 500mW 1064nm and 500mW 1340nm lasers. See fig. 3  for the Emisope III-gt docked to the T6672 Advantest tester.


The failed ICs were thinned down by parallel polishing to a  residual silicon thickness of approximately 100µm. A low  profile socket was also used in order to allow the use of Solid  Immersion Lenses (SIL) for high resolution backside LSM  imaging and DLS analysis.


Figure 3. Emisope III-gt docked to the T6672 Advantest tester.


To synchronize the laser modulation to the tester an external  Electro-Optic Modulator (EOM) was used. The EOM can  modulate the 1064nm wavelength with 15ns rise/fall time. The modulation is controlled by a 0-1V analog input through  a BNC connector. Such input would be typically connected to  a tester I/O signal that would turn on or off the laser output.  However in this case we could not flatten out the MBIST  pattern and we had to use an external pulse generator to  synchronize the laser output with the MBIST sequence. At the  start of the MBIST pattern a loop trigger was generated which  allows us to synchronize the external pulse generator with the  MBIST sequence. This pulse generator then controls a delay  for when the laser output is turned off and the duration for  which the laser output is turned on thus forming the laser  pulse.


In addition the LSM scan speed during DLS acquisition was  controlled externally by the tester. To do so the tester loop  trigger generated at the beginning of the test pattern was also  fed to the external LSM pixel clock synch. This allows  obtaining a dwell time per pixel equal to the test pattern loop  time, which is approximately 3.77ms for the entire MBIST  pattern.  A schematic diagram of the experimental setup is  shown in fig. 4


Figure 4. Schematic diagram of the TR-DLS experimental  setup.


DLS and TR-DLS Results


Prior to perform DLS the IC was set at the 50% Pass / 50% Fail limit. The DLS image was then averaged over several  frames in order to distinguish areas that are either mostly Fail  or mostly Pass under laser stimulation. The laser sensitive  area was first localized in the area of interest using a 20X  objective. By comparing the sensitivity between the two  lasers it was found that the IC was significantly more  sensitive to the 1064nm laser vs. the 1340nm laser. All  subsequent DLS acquisitions were then performed using the  1064nm laser using a 220X SIL lens.


The DLS results obtained in the laser sensitive areas are  shown in fig. 5. To reduce the DLS image acquisition time the  Region-Of-Interest (ROI) feature was used to limit the laser  scanning area. Therefore the image shown in fig. 5 was  cropped to display only the ROI DLS results. The  corresponding LSM image is shown in the right of fig. 5.


Several laser sensitive areas were found within the read/write  logic of the memory cell. The strong back and white signal  near the DLS image center corresponds to the sense amplifier. The DLS signature at the top and bottom of fig. 5 DLS image  corresponds to the bit line pre-charge circuitry, part of the  read circuitry. However some of those laser sensitive areas  might also have corresponded to write transistors as well.  A  DLS survey of this failure, using the default memory test  patterns, was not able to decouple a read or write failure.


To distinguish the difference between a read or a write failure  mechanism, the 1064nm laser beam was turned off during all  MBIST test pattern except for a given read or write sequence. Therefore 13 DLS images were acquired in the exact same  area for each of the 13 sequences. All other DLS acquisition  parameters were kept constant, i.e. identical laser power, same  number of averaged frames, scan direction, etc…


Only six sequences were found to be sensitive to the laser  stimulation.


Those are sequences which involves Port AB read only:


And sequences which involve Port B read only:


Furthermore all sequences involving Port AB read only had  an identical DLS signature. This is also true for the DLS  signature obtained during sequences involving Port B read  only. However, sequence S13 did not show a DLS signature  even though there is a port B read for this test. The reason for


this paradox has not been resolved. The respective cropped  ROI DLS images are given in fig. 6.


Figure 5. Cropped ROI DLS image (left) and corresponding  LSM image (right) obtained with the 1064nm laser beam with  a 220x SIL objective.


It can be noticed in fig. 6 that the DLS image obtained during  the Port AB read slightly differs from the DLS image  obtained during the entire MBIST pattern. Not only was the  DLS signal weaker, but the sense amplifier sensitivity is  asymmetric. The comparison between the Port AB read DLS  image and the Port B DLS image is even more instructive. For  the Port B read sequences, only the sense amplifier was  slightly sensitive to DLS Additionally, the Port B signature  was isolated to just on net in the sense amp circuit.


The first conclusion that we can obtain from the TR-DLS  results is that the failure is related to a read only failure, not a  write failure. Also, the fact that only the sense amp had a  weak signature for the Port B read indicates that the issue lies  with the sense amp only. The simultaneous port A and port B  reads would cause a slightly lower voltage swing on the bit  lines thereby decreasing the sense amp read voltage and  simply making the sense amp issue worse. The fact that only  the sense amp showed a signature during port B reads narrows  the focus of the investigation to determine how to improve the  operation of the sense amp specifically.


Figure 6. Cropped ROI DLS image for Port AB read


sequences, S3, S6, S9 and S12 (left) and cropped ROI DLS


image for Port B read sequences, S8 and S10 (right).


A Dual Port RAM Memory Built-in Self Test (MBIST) failure within an embedded Dual Port memory array was  analyzed using Dynamic Laser Stimulation (DLS). This  technique rapidly localized the failing area within the memory  read/write circuitry (about 21 transistors on about seven nets). However the DLS localization signature and the MBIST fail  information was not able to identify if the failure was related  to a write or read operation.  Without this fundamental  understanding of the fail mode there was little opportunity to  address the fail mode on the device.  To get the detail of  whether this was a read or write failure, it was necessary to  target specific sequences within the MBIST pattern.  To do so  the DLS laser output was modulated synchronously with the  test pattern using an Electro-Optic Modulator (EOM).  Such a  scheme allowed the laser to stimulate the failed IC only  during specific write or read operations within the MBIST  pattern. This paper outlines the successful use of a Time  Resolved Dynamic Laser Stimulation (TR-DLS) [8].  This  TR-DLS provided maps for each operation of the MBIST  pattern. With this information, the failure was clearly  identified as a read operation failure. The TR-DLS technique  also provided much refined site signature (down to just one  net) within the Sense Amp of the Port B of the Dual Port  RAM.  This information provided very specific indication on  how to improve the operation of that particular sense amp  circuitry within the Dual Port RAM Memory.


[1]  Beaudoin F. et al. “Laser Stimulation Applied to Dynamic  IC Diagnostics,” ISTFA (2003), pp. 371-377.


[2] Beaudoin F. et al. “Dynamic Laser Stimulation  Techniques for Advanced Failure Analysis and Design  Debug Applications,” Microelect. Reliab. 47 (2007), pp. 1517-1522.


[3]  Sanchez K. et al. “Delay Variation Mapping Induced by  Dynamic Laser Stimulation,” IRPS (2005), pp. 305-311.


[4]  Sanchez K. et al. “Dynamic Thermal Laser Stimulation  Theory and Application,” IRPS (2006), pp. 574-584.


[5] Cole Jr. E.I. et al. “Resistive Interconnection  Localization,” ISTFA (2001), pp. 43-50.


[6]  Bruce M.R. et al. “Soft Defect Localization (SDL) on  ICs,” ISTFA (2002), pp. 21-27.


[7]  Rowlette J.A. et al. “Critical Timing Analysis in  Microprocessors Using Near-IR Laser Assisted Device  Alteration (LADA),” ITC (2003), pp. 264-273.


[8] P Perdu, R Desplats, F Beaudoin , P Vedagarbha, M  Leibowitz, KR Wilsher, “Spatial and Temporal Selective  Laser Assisted Fault Localization,” US Patent # 6,967,491,  Nov-22-2005.


DOI: 10.1361/cp2008istfa193


Mixed Frequency Detection of Thermal Laser Stimulation (MF-TLS) and its  Application in Failure Analysis


Zhongling Qian, Christof Brillert, and Christian Burmer


Infineon Technologies, Failure Analysis, Munich, Germany  zhongling.qian@infineon.com


A new localization method called MF-TLS is introduced and  applied in failure analysis praxis. The method combines local  periodic thermal stimulation technique with periodic  excitation of the electrical fails. The mixed frequency signal is  detected by a lockin amplifier. MF-TLS was demonstrated on  fabricated opens in a metal line and shown to be in semiquantitative agreement with a capacitance modulation model. The technique was also applied to a scan shift problem and  produced a higher sensitivity compared with other dynamic  TLS methods. Limits and prospects of this new methodology  are described.


With the increasing number of metal layers and shrinking  feature size of VLSI circuits, traditional tools of defect  localization in failure analysis, such as emission microscopy  and thermal laser stimulation (TLS), have met a great  challenge [1-2]. On the other hand, modern ICs include a full  scan design, which allows improved diagnostics – sufficient to  isolate problems to a short list of candidates for faulty nets, in  the best case, to one single net. The corresponding physical  defect can be localized by using TLS (thermal laser  stimulation) technique in a static circuit in correlation with the  diagnosis results [3]. In order to handle soft fails with a  signature of a voltage, temperature, or frequency dependent  behavior, soft defect localization (SDL) method was  developed [4-5].  In SDL technique, heating due to the  absorption of  NIR laser energy will cause soft defects to  change their electrical behavior during dynamic testing, thus  changing the pass /fail status of the test. The further  development of SDL technique leads to dynamic laser delay  variation mapping (DVM) [6] and lockin assisted SDL (LIASDL)[7]. The voltage mode of LIA-SDL has been  successfully used in the scan test related failure analysis by  using amplitude detection [7] and the mapping of bypass  chains by using phase detection in high frequency range [8].


Lock-in amplifiers are used in commercial TLS instruments to  improve the detectable minimum current and S/N (ratio of  signal to noise) of detection system during localization of  static fails [9]. In operation, the intensity of NIR laser beam is  periodically modulated, typically 5 KHz to 50 KHz. The  narrow-band characteristic of lock-in detection can greatly  diminish both the external and internal noise produced at  frequency domains away from the lock-in frequency. Lock-in  amplifiers are also applied in localizations of dynamic fails [7-8, 10], where periodic inputs of devices are set as a reference  signal for lock-in amplifiers. Except amplitude detection, phase outputs from lockin amplifiers are also used to measure  relative delay of periodic signals. The frequency of periodic  inputs is selected to avoid the periodic internal signals, such as  PLLs and clocks. This method is very powerful for defect  localization in a dynamic function test with looped patterns, such as scan shift and logic tests.


However, in the modern IC chip, capacitors, such as  poly/diffusion capacitance, are integrated within a single chip  in order to reduce supply noise and variation during the  dynamic operating. These capacitors including those on test  boards also act as a low pass filter between VDD and VSS, which for dynamic TLS detection strongly decreases its  detection sensitivity. One possible method to reduce the  influence of such a low pass filter is to shift the detection  frequency to an optimized lower value by using mixed  frequency technique.


The mixed frequency technique can also be applied in the  direct localization of open sites in metal lines. It is well known  that a resistive via/metal open can be detected by using normal  TLS method [2]. The direct localization of a real open in  metal lines or vias in chips is a significant challenge to the  normal TLS and other failure analysis methods. In some cases, time integrated and resolved emissions can give an indication  of an open net, if this open line/via causes at least one floating  gate. Further localization of the open site can be finished by  using FIB cuts and passive voltage contrast imaging – a long a  tedious process.


Our paper starts by describing the system setup of the new  developed Mixed Frequency TLS (MF-TLS) technique. A  modulated capacitance model is developed to describe an  open metal line and confirmed by using test structures with  FIB slits. Next, the application MF-TLS to scan shift problems  is discussed in detail to demonstrate the unique capability of  this technique. Then, further possible applications to  localization of cross talking (x-talking) problems are  discussed. Finally a short conclusion is made.


Figure 1: General experimental setup of the MF-TLS system.  The physical model of an open metal line is shown in the  dotted block. L0 is the width of the metal gap. Rd is the  detection resistor.


The system setup is shown in Fig.1. The NIR laser is  periodically modulated with the frequency f1, while a  voltage/current signal with the frequency f2 is applied at the  operating device. For example, the f2 signal could be the scan  input/output, clock or other signals in the looped function test, or the AC part of external power supplies for devices. The  corresponding mixed frequency |f2±f1| is obtained from these  two signals by using a mixer and band pass (BP) filter and  used as a reference signal to lock-in amplifiers. The TLS  signal is sent to the input of the lockin amplifier. Its output is  then forwarded into the image processing unit for recording  the signal intensity versus position.


In Fig.2, the MF-TLS image with f2 at 500kHz shows a better  contrast in comparison with the image at 1.5kHz. The


experimental results showed a clear increase of detection  sensitivity and the contrast enhancement with increasing f2  from 1.5kHz to 500kHz. The result correlates qualitatively  with the formula above.


In this setup, the maximum detectable gap width was 0.1μm  with f2=500KHz. From the formula above, in order to localize  an open site with gap >0.1um, the frequency f2 or the  application AC voltage must be raised.  However, the AC  voltage can not be arbitrarily increased due to possible  isolation breakdown. The best choice is to move the frequency  f2 to a higher range or into RF range for a higher detection  limit for metal opens. In the higher frequency region, the  impedance matching between the signal generator and the test  devices must be taken into account for a better exciting of  open defects.


Figure 2: The experimental sample with different gap widths  in the metal lines on the meander test structures. The gap was  made by FIB modifications.


Figure 3: The MF-TLS experimental results of the metal line  with a 0.1μm FIB gap (x20): (a) f2:1.5kHz (b) f2:500kHz (c) overlay.  The laser is modulated at f1= 50KHz and f2 is the  frequency of AC power supply with Vpp=5V applied to the  metal line..


Application 2:  Scan Shift Test


A typical case for scan chain shift problem is shown in Fig. 4. This is a product with 0.13µm technology and 7 metal layers. The corresponding yield loss was 2% due to this type of  failure. One or more scan chains showed no scan output (SO). The fails showed no voltage and temperature dependence.


Scan CLK


Fail   SO


Ref    SO


SI


Figure 4: The timing diagram of the failed device showed a  scan chain problem without SO after the capture cycle.


The device was firstly inspected by using the EMMI and  normal TLS but not signal was observed. The current mode in  LIA-SDL normally is used for localization. However, in this  case, no signal was observed. In order to increase the  detection sensitivity, the MF-TLS method was used.


Typically, the scan chain consists of 4000 scan flip-flops (FF). The scan shift pattern works with a scan clock (SC) at 5 MHz.  The scan input (SI) is modified using “111000” in loop mode. Therefore SI signal has a frequency of 833 kHz. This signal  also serves as one input for the mixer. The input for the mixer  comes from the signal generator for the laser modulation.


Using MF-TLS a signal spot was found in the logic block and  located on the failed chain. The localization results from MFTLS are shown in Fig. 5. In comparison with the normal TLS  detection in the static mode and the LIA-SDL detection, this  localization method demonstrates additionally a higher  sensitivity. This improvement is attributed mainly due to the  reduced low pass filter effect between the power supply in  chips and test board achieved by using the mixing frequency  technique.


In order to determine the best choice for the difference  frequency, the MF-TLS spot was observed with for difference  frequencies in the range from 0.5 kHz to 50 kHz. The MFTLS images in Fig.5 were taken with the same setup in the  preamplifier and lockin amplifier and are shown in the same  scale for comparison.  The dependence of the MF-TLS signal, noise and SNR ratio on the difference frequency is shown in  Fig.6.


Generally there is no large SNR difference in the selected  difference frequency range due to using lockin amplifier (Triangles in Fig.6). At the lower difference frequency, the  MF-TLS signal is larger, but so is noise background. The  stronger noise in the lower frequency can be explained as 1/f


noise background. The tailing of the MF-TLS spot is due to  relatively short time constant in the lockin amplifier. For  comparison, the time constant and the laser scan speed in all  cases stayed as the same. With a longer time constant for  lower frequency difference and a corresponding slower scan  speed, this tailing effect can be greatly reduced.  However, it  means also a longer localization time.


Figure 5: The MF-TLS localization results are shown with the  difference frequency in the range from 0.5 kHz to 50 kHz: (a) overlay, (b) 50kHz, (c) 25kHz, (d)5.0kHz,(e) 1.0kHz,(f) 0.5kHz  and (g) direct LIA-SDL. The localization result using the  current mode of LIA-SDL is shown at the right side for  comparison. The overlay with layout showed the spot was  localized at one of the FFs of the highlighted scan chain.


MF-TLS


Difference Frequency (Hz)


signal  noise  S/N


Figure 6: The MF-TLS signal, background noise, and SNR  dependence on the difference frequency in the range 100Hz to  100 kHz in the log scale


On the contrary, at the higher frequency difference the MFTLS signal is weaker but along with a lower noise  background. Since no tailing effect was observed in this  frequency range, it is very suitable for a fine localization.


The benefits of MF-TLS methods have been demonstrated in  the localization of open sites in metal lines and the fail site in  scan chains.  The difference in both applications is due to two  different types of detection objects. The capacitance due to  open metal line was detected in the first case, while the  dynamic periodic current due to leakage/short in the second. In the first case, a higher difference frequency up to MHz or  RF range is needed to extend the maximum detection width of  open slits. In the second case, a lower difference frequency is  suitable for the rapid global localization with a higher  sensitivity. The fine localization can be completed in a higher  frequency up to 50kHz. Therefore, the choice of the difference  frequency must be made according to the possible fail  mechanisms during the application of this method for failure  analysis. Clearly a static EMMI and TLS inspection should be  performed first, in order to determine the fail is not just a  simple localization problem.


(b) (c)


(g)


(d) (e) (f)


Another possible application of MF-TLS is the  characterization and localization of crosstalk, which is very  important for signal integrity in design and layout  optimization, particularly in analog or mixed signal designs. Crosstalk is normally induced by undesired capacitive or  inductive coupling between neighboring circuits or metal  lines. In CMOS technologies, coupling capacitance dominates. Most of the crosstalk problems in a design can be found and  fixed by using automatic design tools. However, in some  cases, it is important to localize the crosstalk site for design  debug, particularly in the analog design. The crosstalk  coupling between two signal lines causes a mixed signal, which is very suitable for the localization by using the mixed  frequency technique in combination with TLS system and  lockin detection. An experiment with this direction will be  started in the near future.


In conclusion, this paper has introduced a new localization  method called MF-TLS. At one side, this method will increase  sensitivities of dynamic TLS localization methods.  The  shifting of the lockin detection frequency to a lower optimized  value can greatly reduced the low pass filter effect due to  capacitances in the chip and also capacitors on the power  supply board of testers. A lower difference frequency was  suggested for a global localization and a higher frequency was  selected for a fine and rapid localization.  On the other hand, this method can be applied to the direct localization of the  open site in metal line. For open metal lines, the experiment  results correlates well with the capacitor model for the gap in  the open metal line.  In order to obtain a better open detection, the frequency f2 must be raised to an optimized value. The  maximum slit width is about 0.1μm for our setup at the  moment.


[1] R.A. Falk, “Advanced LIVA/TIVA techniques” , ISTFA  2001


[2] E.I. Cole Jr. et al., “Resistive Interconnect Localization”, ISTFA,43-50 (2001)


[3] Z.-L. Qian et al, “Precise defect localization of scan logic  failures by thermal laser stimulation (TLS)”, ISTFA, 517-520 (2004)


[4] M.R. Bruce et al., “Soft Defect Localization (SDL)”, ISTFA, 21-27 (2002)


[5] F. Beaudoin  et al., “Laser Stimulation Applied to


Dynamic IC Diagnostics”, ISTFA, 371-377 (2003)


[6] K. Sanchez et al., “Dynamic Laser Delay Variation


Mapping (DVM) and Applications”, ISTFA, 106-114,


(2005)


[7] Z.-L. Qian et al. “LIA-SDL and its Application in Scanshift problems”, ISTFA 2005


[8] C. Brillert  et al, “Laser assisted Lock-in Phase & Spectral  Analysis Techniques at advanced IC Failure Analysis


with application to Jitter and Soft-Defects”, ISTFA 2007


[9] F. Beaudoin et al, “Lock-In Amplification Applied to  Thermal Laser Stimulation”,  2nd European Workshop on  Photonics Failure Analysis, Munich (2002)


[10] M. LaPierre and R. A. Falk, “Dynamic Thermal Laser  Signal Injection Microscopy (T-LSIM) on AC  Propagation Failures”, 43rd IRPS, 280-285 (2005)


DOI: 10.1361/cp2008istfa198


Differentiation Between Artifacts and True Defects in 45 nm BEOL Structures in   M-TLS Technique


A.Reverdy a, P. Perdu c, M. de la Bardonnie a, H.Murray b, P. Poirier a, B. Domengès b   a NXP Semiconductors, 2 rue de la girafe, 14000 Caen, France


b LaMIPS, Laboratoire commun NXP-CRISMAT, UMR 6508 CNRS ENSICAEN UCBN. 2, rue de la Girafe BP 5120, F-14079 Caen Cedex 5, France


c CNES, 18 avenue Edouard Belin, 31401 Toulouse, France


E-mail adress: Antoine.reverdy@nxp.com


Modulated Thermal Laser Stimulation (M-TLS) has been  established as a key technique to accurately localize defects at  elementary structure level, in deep submicron technologies. It  has been achieved by Thermal Time Constant analysis (TTC) which allows the study of thermal exchange dynamics. In this  paper, we demonstrate for the first time the efficiency of this  technique on 45 nm Back End Of the Line (BEOL) defective  test structure on image mode, and we underline the efficiency  of the developed technique to differentiate artifacts from true  defects in 45 nm BEOL structures.


Due to microelectronic technology developments, the Back  End Of the Line (BEOL) part of devices is becoming more  and more an important defective area. This observation  originates from the down scaling of metallization and the  increase in copper interconnects density and number of layers  in BEOL. Therefore, Failure Analysis (FA) turns into a real  challenge, and in order to stay competitive on next technology  nodes, FA techniques have to exceed their current limits.


In our aim to improve Thermal Laser Stimulation (TLS) based  fault isolation method [1], we previously developed a  Modulated – Thermal Laser Stimulation (M-TLS) approach


[2]. In this paper, we will study M-TLS signatures of 45 nm  Electro-migration (EM) test structures. This modulated  approach makes it possible to analyze the dynamics of thermal  exchanges involved in TLS using Thermal Time Constant (TTC) analysis. It allows us to extract additional  characteristics of the excited structure and obtain data not  accessible with the standard TLS technique [3]. In fact, instead of working on the magnitude of resistance variation  induced by the laser, we propose to image the phase-shift  between the pulse signal modulating the laser, and the M-TLS  response.


In this paper, we show that in some specific configurations, TLS images may contain spots that look like defective  signatures, but are actually just artifacts due to thermal


interactions with the surroundings. We demonstrate that  phase-shift imaging appears as a solution to differentiate this  kind of artifacts from real defective signatures.


Limitation of classical TLS


TLS technique is well known as one of the most widely used  techniques for defect localization purpose. This approach uses  an Infra-Red laser source (λ=1340 nm) to create a spatially  confined thermal gradient. The local temperature deviations (ΔT) induce a resistance variation (ΔR) that depends on the  resistance temperature coefficient (αTCR) of the conducting  materials, according to the formula:


T


TCR Δ


Δ


0 αρ


where ρ0 is the metal resistivity, αTCR is the metal thermal  coefficient of resistance, S the metal line section and L the  length heated by the laser.


In the case of Optical Beam Induced Resistance Change (OBIRCH) [4], the Device Under Test (DUT) is biased with a  constant voltage, and a specific amplification chain detects  current changes due to laser excitation. When the laser beam  scans the DUT, current variation is acquired for each position, and a virtual representation of the scanned area is made. This  technique is used to localize shorts [5], resistive paths [6], voids [7], and also to image current paths [8].


This next experiment demonstrates that classical TLS image  can contain spots not related to a real defect, but resulting  from interactions between the laser source, the thermally  stimulated structure and its vicinity. In this example, we  consider an EM copper line (width: 70 nm), designed in 45  nm CMOS technology, located on the third metal layer (figure 1.top). The structure was stressed (temperature and  current) with resistance value monitoring. Four other copper  lines, two on each side, are situated in the same horizontal  plane, with a 70 nm pitch, for extrusion detection purpose. Two perpendicular lines (measurement lines) are connected  with these extrusion lines, to detect potential migration  phenomenon which can induce shorts between the active  copper line and those extrusion lines (figure 1.top and


1.middle). This EM structure is analyzed using the OBIRCH  technique with a biasing voltage of 150 mV. Figure 1 presents  the resulting TLS signature (figure 1.bottom).


Figure 1: a: optical top-view of the studied 45 nm EM  structure. b: Detailed description of the center of the structure (Layout view: M3 oblique lines, M2  wavy lines). c: OBIRCH response related to the optical top view area.


Both electrical and thermal stresses applied on the EM  structure have induced an increase in the structure’s  resistance. Thus, we can reasonably expect the formation of  voids somewhere in the active line.


The obtained OBIRCH signature shows a clear spot in the  center of the studied line (figure 1.bottom, white arrow), which is consistent with a void signature. We also notice that  the spot location matches the area where measurement lines’ are implemented.


A Focus Ion Beam (FIB) cross section made at this specific  location reveals no physical defect correlated to the TLS  localization (figure 2). The same kind of signature was found  on four other samples from the same lot. Once again, no  physical defect is observed. Thus, we conclude that these  detected OBIRCH spots were just artifacts resulting from  copper environment change, and were not related to a real  defect.


Figure 2: SEM observation after FIB cross section in the  specific area designated by OBIRCH spot. No physical defect  is evident.


Due to the high reflection of copper (around 95%), the copper  surroundings acted as supplementary heat sources. So they  increased the amount of energy transferred to the studied line  targeting by the laser beam. Because TLS response is directly  linked to the amount of energy brought onto the structure, the  intense TLS spot appears as a consequence of this


phenomenon. Moreover, when the laser illuminates the  measurement lines, the active line is indirectly heated. As a  consequence, the OBIRCH spot is spatially enlarged, preferentially in the measurement line direction (top to  bottom).


MTLS phase shift analysis in image mode


M-TLS phase-shift principle


The principle of M-TLS analysis is exactly the same as  standard TLS approach; but instead of using a continuous  laser beam, we controlled the laser intensity to generate a  modulated TLS signal. This imposed TLS response can be  modeled by an exponential model introducing four TTC, two  for the heat-up and two for the cool-down mechanisms. The  first one models the self-response of the studied structure  illuminated by the laser, and the second one is more related to  interactions between the laser, the structure and its  surrounding (figure 3) [9].


Figure 3: Typical TLS response induced by a laser power  step (heat-up mechanism). It can be modeled by a  combination of two TTC: a predominant heat-up mechanism  due to laser illumination, characteristic of the structure (dotted red circle) and a second order cool-down mechanism  due to surrounding interaction (red circle).


Those TTC signatures have already been collected in “single  point illumination” mode (time domain). Unfortunately, time  domain analyses are hardly applicable in scan mode, and this  is why a frequency domain approach has been developed. At  the same time, we have established the link between  measurements taken in both time domain and frequency  domain (TTC and phase-shift measurements) [3]. This  methodology is compatible with synchronous detection  capability, noted for the signal to noise ratio improvement [10]. Furthermore, lock-in amplifier enables the study of  phase-shift measurements between the laser modulation  signal and the M-TLS response. As in the classic TLS  technique, if we synchronize the laser beam location with MTLS phase-shift acquisition, this new methodology allows 2-D maps reconstruction of M-TLS phase-shift measurements  of an area.


Phase-shift measurement can be achieved with the  combination of a lock-in amplifier (i.e.: synchronous  detection), a modulated laser source, and a “slow scan mode


Extrusion lines


Line studied


Measurement Lines


c


10 µm


-1 1


TLS signature


Laser


stimulation


Time (µs)


acquisition (figure 4). Due to thermal phenomena dynamics, modulation frequency has to be lower than a hundred  kilohertz (typical ~20 kHz). At the same time, lock-in  processing forces the laser scanner to stay several modulation  cycles on each illuminated pixel. Consequently, pixel dwell  time must be chosen around 500µs – 1ms, which can be time  consuming. For example, a 512 by 512 pixel image takes 262  seconds. One interesting way to overcome this limitation  consists in to decrease the pixel number per image (flexible  scan).


Figure 4: Principle of imaging in M-TLS mode. Phase-shift  and magnitude images are externally generated and treated  from in-phase (X) and out-of-phase (Y) signals from the lockin.


M-TLS phase-shift acquisition


First phase-shift images were made on the previously  described EM structure. To demonstrate the necessity to  perform a specific processing on M-TLS data, we present two  images using different treatment in figure 5. The top figure (figure 5.top) presents a direct acquisition of the phase-shift  information coming out from the lock-in. The bottom one  shows the same image built from the in-phase and the out-ofphase signals from the lock-in amplifier, and treated externally (figure 5.bottom).


Figure 5: M-TLS phase-shift signature of the described EM  structure (bias 150mV, mag. 20x, modulation frequency: 15  kHz). Top: without treatment. Bottom: with artifacts rejection  treatment.


Phase-shift ∆ϕ and magnitude R of the images calculated by  the lock-in are internally created from in-phase (X) and outof-phase (Y) components according to formulas:


arctan(XY


Δϕ


²


² Y


R +=     (3)


From equation (2), we note that if X values are very small, calculation artifacts can drastically jeopardize the result (figure 5.Top), which fluctuates between two extreme values (-180° and 180°). Unfortunately, this phenomenon makes raw  phase-shift images unusable directly. For a better  visualization of the information contained in phase-shift  images, we have developed a simple approach giving us an  artifact free phase-shift image (figure 5.Bottom). In this  configuration (current path imaging), one proper solution  consists in performing “Magnitude threshold treatment” on  the phase-shift image.


Differentiation between artifacts and true defect


Measurement on non defective area


Previous experiment shows that standard TLS image can  contain spots unrelated to a real defect (figure 1 and figure 2). In this part we will demonstrate that phase-shift analysis is  less sensitive to those phenomena, and appears as a relevant  technique to pinpoint this kind of artifact.


Firstly, we performed M-TLS acquisition in the same area as  figure 1. Figure 6 illustrates magnitude (top) and phase-shift (bottom) M-TLS response.


Figure 6: M-TLS magnitude signatures of the EM structure, at the “measurement line” location (bias 150mV, mag. 100x, modulation frequency: 15 kHz). Top: Magnitude image. Bottom: Phase-shift image. Region 1: regular area. Region 2: spot area.


As could be expected, the magnitude image in M-TLS mode (figure 6.top) presents the same global aspect as figure 1. It  shows an intense spot where “measurement lines” are located. The single difference can be found by studying the signal to  noise ratio but this is not the purpose of the study. We assume  that the spot is definitely not an artifact resulting from the  scanner speed, because M-TLS images are taken in slow scan  mode.


2  4  6  8


0  2  4  6  8


-38


-36-34-32


µm µm


0  10  20  30


-40


-36


-34


-32


-30


µm


0  0  10  20  30


-50


-100


-150


I


OBIRCH  amplifier


Trigger


modulation


Lock-In unit (X, Y  measurements)


Calculation  and


treatment


Magnitude and phaseshift imaging


Now, analyzing the phase-shift image, we notice that it  presents a spatial expansion (black arrow) in the same location  as the magnitude image. This is a direct consequence of the “magnitude threshold treatment” used, and is not a  representative of phase-shift signature variation.


The second result is more interesting. We note that opposite to  magnitude measurement, phase-shift is quasi-uniform, in  value, all along the copper line (~ -36°). The next table  contains mean values extracted from the previous acquisition. We compare the “regular signature” (1: current path into the  copper line apart from the spot: regular area) and the one  resulting from the measurement lines interaction (2: M-TLS  spot: spot area) in Table 1.


Regular value (1)


Spot value (2)


Magnitude (A.U.)


0.39


Phase-shift (deg.)


-35.8°


-35.9°


Table I: Mean values of phase-shift and magnitude extracted  from the regions highlighted on figure 6.


We have to be careful when comparing those quantitative  values because we deal with different unit systems. Nevertheless, since the magnitude varies more than 100%, and  phase-shift stays almost constant, the difference between the  regular and the spot areas is clearer. In this specific  configuration, phase-shift stays constant all along the line, and  appears consequently insensitive to those environmental  artifacts.


This last assumption stays in line with previous work [3]. In  fact, we have already demonstrated that in the first  approximation and under certain configurations, 1st harmonic  phase-shift of M-TLS signatures can be linearly linked to  single TTC describing the self thermal response of the  illuminated structure. Thus, if the excited structure does not  change in term of geometrical characteristic, it is not located  in a too dense copper environment, which is the case of our  copper line test structure, and it does not contain any defect, its phase-shift signature is unchanged.


We also note that phase measurement is more stable in the  artifact area. This comes from the lock-in processing. In fact, when the magnitude of the studied signal is large, the phaseshift measurement is more stable. Thus in the spot region, the  high amplitude makes the phase-shift measurement less noisy. This aspect justifies our previous mean value calculation  approach.


Finally, we show that M-TLS phase-shift analysis is quasiindifferent to this kind of artifact, and appears as a relevant  method to differentiate true defects and artifacts related to  interactions with the environment. This result can be  physically explained by the fact that, opposite to magnitude  analysis, phase-shift is independent of the amount of energy  transferred to the line, but depends only on the dynamics of  the heat exchanges involved. We can add that the change in  the copper surroundings density is too localized to  significantly affect thermal behavior dynamics.


Application to a real defective area


In a second experiment, we performed the same M-TLS  investigations near the anode side of our EM test structure. It  is considered as a preferential location for void formation, due to via influence [11]. Moreover, the electrical monitoring  shows in increase of the resistance value. Thus, we assume  that this anode via is affected by a metal  migration/degradation. A Focus Ion Beam / Scanning  Electron Microscopy (FIB/SEM) cross section will be made  after localization purpose, to confirm the presence of a defect. The main objective consists in analyzing the defect influence  on M-TLS acquisitions, and particularly on phase-shift  images. Hereafter, we compare magnitude to phase-shift  response in the anode area.


The required laser beam is supplied by a confocal laser  scanning microscope (LSM). Slow-scan capability of about 2  ms per pixel is needed. A cw high power laser with 1.3um  vacuum wavelength is used for thermal laser stimulation. A  second high power laser with a wavelength of 1064 nm can be  used for carrier injection. The microscope is equipped with  high NA 50x objective lens with silicon thickness correction. Measured laser powers are between 30-160 mW at the output  of the 50x lens. The lock-in amplifier has a maximum


detection frequency of 2 MHz. A preamplifier with variable  band pass filter is used for MF-TLS detection.


In the MF-TLS technique, the NIR laser is modulated with a  frequency f1. The narrow-band and stroboscopic-like  detection in the lock-in technique can greatly reduce both the  external noise and the effects from other frequency domains, such as scan clock and PLL’s. Appropriate selection of the  difference frequency reduces low pass filter effect due to inner  capacitances in the chip and capacitors on the power supply  board of testers in a dynamic circuit.


Application 1: Metal Open Detection


As a first demonstration, the mixed frequency dynamic TLS  technique was used to localize an open site in a metal line. A  modulated capacitance model (the dotted block in Fig.1.) is  used to describe the effect of laser heating on the open metal  line. The gap between the broken metal lines forms a capacitor  with capacitance C0. This capacitor can be filled with media  such as air, oxide or some mixtures, which usually has a quite  small thermal conductivity in comparison with Al or Cu metal  lines. Therefore, a higher temperature increase is expected at  this gap during the thermal laser radiations. The  corresponding thermal expansion of gap length L0 causes a  small variation of the capacitance during the absorption of  periodical NIR laser (f1). The capacitance variation can be  detected simultaneously with an application of AC voltage (f2) at the open metal line. The variable capacitor acts here as a  nonlinear frequency mixer. Resistor Rd is used for MF-TLS  detection and is much smaller than the impedance of C0 in a  low frequency range. Based on this model within the 1st order  linear approximation, the mixed frequency |f2±f1| TLS signal ∆U can be expressed as follows:


∆U ≈ -Ui (f2)·2πf2‧Rd‧C0‧α∆T(f1)/L0                   (1)


where Ui is the applied AC voltage with frequency f2, α is the  linear thermal expansion coefficient of the media in the gap  and ∆T(f1) is temperature increase due to the absorption of   NIR laser with a modulation frequency f1.


From Formula (1) above, it is clear that the detection  sensitivity is proportional to f2, the temperature variation and  the reciprocal of L0. In order to verify this model, an  experiment was made with metal line meander test structures. The open site was made by using FIB cuts (Fig.2) in a  meander test structure in order to obtain different gap widths  from 0.05 to 1um for a systematical experiment. A typical  result was shown in Fig.3.  In this case, the gap length is about


0.1μm and the open shows a resistance up to 50GOhm. The  modulation frequency f1 of the laser is 50kHz. The applied  AC voltage has a variable frequency f2. The reference  frequency for lockin amplified was then set to |f1-f2|.


-36-34


Figure 7: MTLS signatures of the EM structure, at the anode  side (white arrow), bias 100mV, mag. 100x, modulation  frequency: 15 kHz. Top: MTLS magnitude image. Bottom: MTLS phase-shift image.


Figure 7.up shows the M-TLS magnitude response. If we  compare it with the previous “non defective area” case, it  appears difficult to determine if this specific signature results  from a real defect or if it is again, an artifact due to interaction  with the close environment. The magnitude image contains a  clear spot at the anode side, which is very similar to the one  observed in figure 6. It could be problematic for FA engineers  to consider these two signatures as consequence of the same  physical root cause.


Lastly, we performed phase-shift imaging (figure 7.bottom), with the same experimental parameters. Opposite to the  previous investigation, we note that the phase-shift value  varies in the suspected location. Once again, phase-shift  response is relatively noisy, and a “mean value approach” is  relevant. Quantitative results are tabulated in Table II for  better interpretation.


0.12


0.22


-35.7°


-33.8°


Table II: Mean values of phase-shift and magnitude extracted  from the two regions highlighted in figure 7.


From table II, we clearly note that extracted values are  different. In the via area, the M-TLS signature has less of a  phase-shift, i.e. to a “faster response”. Using an appropriated  image processing, this variation can be detected without  difficulty (figure 7.bottom).


For a better interpretation, we perform the same phase-shift  analysis with various biasing conditions. Because magnitude  of TLS signals is dependent on current density in the excited  structure [12], we adjust the Lock-in sensitivity (i.e. input  amplification) to achieve the best dynamic range. Table III  summarizes mean values extracted from both via and copper  line areas.


Biasing conditions/ sensitivity


Regular value  Phase-shift (deg.) /magnitude (A.U.)


Spot  value


Relative  variation


150mV / 100mV


-35.7° / 0.18


-33.8° +1.9°


100mV / 50mV


-36.6° / 0.12


-33.9° +2.7°


50mV / 20mV


-38.2° / 0.06


-34.6° +3.6°


Table III: Mean values extracted from the suspected defective  area (Spot value) and non defective area (regular value) for  various biasing conditions.


First, we note that the measured regular values vary with the  biasing conditions and the lock-in sensitivity. This result can  be explained by looking at the ratio between magnitude of the  TLS response and the lock-in sensitivity. Unfortunately, when  dealing with various voltage levels, it is hard to compare two  measurements with different acquisition parameters. Nevertheless, this is not a limitation because the principal  information is contained in the relative variation between two  sets of data.


A more interesting result from table III is the relative variation  between the regular (1) and the spot (2) signatures. We note  that this relative variation increases when the biasing  condition decreases. Consequently, differentiation between  line and via signatures is easier. This trend can be explained  by the fact that the M-TLS signatures result from the  superposition of OBIRCH and Seebeck Effect Imaging (SEI) phenomenon, which occur simultaneously [13]. Therefore, when the biasing voltage goes down, the OBIRCH response  becomes smaller and smaller, while SEI signal stays constant. Thus, its influence grows more and more important in the  global M-TLS signature.  It is worth mentioning that the  modulation method can also be used with the so-called SEI  technique, based on gradients measurement in electrical  potential at metallic interfaces induced by a local heating. In  standard case, the DUT is grounded to avoid resistance  change detection. This phenomenon is known as  thermoelectric effect or Seebeck effect. Applied in failure  analysis, this technique can effectively pinpoint voids in metal  lines, which is the suspected kind of defect. Seebeck effect is  usually hidden by OBIRCH effect, but in a low biasing  condition SEI and OBIRCH induced signals are comparable. To validate the presence of a defect into via area, we perform  a dual beam cross section in this region (figure 8).


Figure 8: FIB / SEM cross section at the “current input side” of the studied Electromigration structure.


Figure 8 shows a void resulting from EM degradation (figure  7). It is localized at the top of via connection between metal  layers 2 and 3, as could be expected. This voiding formation  induces a local shrinking of the EM line. Consequently, thermal phenomena dynamics are speeded up, and by the way  the measured phase-shift value decreases. In the same time, this void also creates local interfaces which generate some  Seebeck potential. As we previously said, those two  phenomena act simultaneously, and are comparable in term of  intensity when applying low voltage biasing condition to the  DUT.


In this paper, we have demonstrated for the first time the  power of Modulated-Thermal Laser Stimulation in phase-shift  detection mode to accurately localize defects at elementary  structure level, in 45 nm BEOL test structure, in image mode. This modulated approach is also applicable to Seebeck Effect  Imaging application. This kind of SEI application appears as  an important aspect concerning electromigration phenomena  localization.


We have shown the efficiency of M-TLS phase-shift images  to identify artifact resulting from near vicinity interaction, which has a classic TLS signature similar with a defective  one. The case study demonstrates that phase-shift image is  insensitive to heterogeneous temperature distribution induced  by copper surroundings.


At the same time, we have confirmed that phase-shift analysis  is able to point out defective area where thermal dynamic  behaviors are impacted by the defect.


Our future research will be dedicated to Modulated Seebeck  Effect Imaging in phase-shift detection mode, where  interpretations are more complex.


The authors wish to thank J.Roux, T. Kume and Mr Ida from  Hamamatsu photonics for Lock-In Amplifier specific  integration in our PHEMOS 1000. They also would like to  thank Dr. Xiao-Mei Zhang for physical analysis (X-section) on our EM samples.


[1] F. Beaudoin et al., “Principles of Thermal Laser Stimulation Techniques”, Microelectronics Analysis desk reference, p417-425


[2] A. Reverdy et al., “3-D defect localization by Measurements and Modeling  of the Dynamics of Heat Transport in Deep Sub-micron Devices”, International Symposium for Testing and Failure Analysis, 2007


[3] A. Reverdy et al. “Fast and Rigorous Use of Thermal Time Constant to  Characterize Back End of the Line Test Structure in Advanced Technology”, accepted for oral presentation in the European Symposium Reliability of  Electron devices, Failure physics and analysis 2008, ESREF 2008.


[4] K. Nikawa and S. Tosaki, International Symposium for Testing and  Failure Analysis, 1993, pp. 303-310.


[5] K. Nikawa, "Failure analysis case studies using the IR-OBIRCH method”", Photonics Failure Analysis Workshop, Boston, Oct 1, 1999


[6] E. I. Cole Jr et al., “Resistive Interconnection Localization”, International  Symposium for Testing and Failure Analysis, 2001, pp.15-21. [7] E. Langer et  al., “Localization and Analysis of Metal-coati


[7] E. Langer et al., “Localization and Analysis of Metal-coating  Electromigration Degradation in 65 nm Technology nodes”, Electronic Device  Failure Analysis, Feb. 2008, vol. 10, Issue 1, pp.24-29.


[8] D. Lewis et al., “Implementing Laser-based Failure Analysis Methodolgies  Using Test Vehicles”, IEEE Transactions on Semiconductor


Manufacturing, May 2005, Vol. 18, No. 2, pp.279-288


[9] Reverdy A et al., “Dynamic study of the thermal laser stimulation response  on advanced technology structure”, Microelectron Reliab (2008), doi:10.1016/j.microrel.2008.05.003


[10] M. de la Bardonnie et al., “The effectiveness of OBIRCH based fault  isolation for sub-90nm CMOS technologies”, International Symposium for  Testing and Failure Analysis, 2005, pp. 49-58. ISTFA 2005


[11] E. Langer, “Electromigration in Copper Interconnects: Degradation  Studies and Failure Analysis”, International Symposium for Testing and  Failure Analysis, 2007, tutorial.


[12] K. Nikawa et al., “Failure Analysis Case Studies Using the IR-OBIRCH  Method”, Proceedings of the 8th Asian Test Symposium, 1999, pp.394


[13] A. Glowacki et al., “Characterization of thermoelectric devices in Ics as  stimulated by scanning laser beam”, International Reliability Physics  Symposium, 2005, pp. 450-457.


DOI: 10.1361/cp2008istfa204


Calibration of Nanoprobe Capacitance-Voltage Spectroscopy (NCVS)


Terence Kane and Michael P. Tenney


Andrew Erickson, and Peter Harris


Multiprobe, Inc., Santa Barbara, California, USA


MOSFET devices are routinely measured at the probe pad  level with conventional capacitance-voltage (CV) measurement instruments.  Such measurements are done at the  front end of line (FEOL) and back end of line (BEOL) process  completion levels.  The CV data is used to monitor the process  and verify certain parametrics such as effective oxide  thickness (EOT), Tox,  gate drain overlap capacitance (Miller  capacitance), trapped charge, diffusion/halo implant oxide  leakage, doping concentration, threshold implant level and  many others.  This type of testing is treated at length in the  classic text of Nichollian and Brews [1]. The introduction of  Nanoprobe Capacitance Voltage Spectroscopy (NCVS) of  discrete MOSFET devices and the method of performing  scanning capacitance imaging (SCM) have been previously  presented [2].  In that work, the authors used a capacitance  sensor to measure the capacitance of an individual failing  embedded DRAM capacitor.  This paper will describe  nanoprobe CV measurements of a discrete finger device from  a multiple finger test structure and show comparable results  obtained at the probe pad level, using an improved version of  the earlier capacitance sensor.  By comparing the BEOL test  structure measurements with NCVS results from a single  finger, we will verify and calibrate the nanoprobing technique.


CV curve analysis has been the primary metric for gate oxide  properties [3,4,5,6,7,8].  Test structures designed for CV  measurements are used to measure oxide and doping  properties of a process because the gate capacitance of a single  transistor is far too small to measure with available analyzer  equipment [4]. Meaningful nanoprobe CV characterization of  discrete MOSFET devices requires the development of a  capacitance measurement tool with sufficient sensitivity and  accuracy to measure structures with capacitance of less than  one femtoFarad.  The resonant sensor used for scanning  capacitance imaging is known to be able to measure  capacitance changes at this level [9].  The tools that have been  commercialized to do capacitance imaging have not been  applied or optimized to allow for discrete device CV  measurements.  However, an updated version of the resonant  capacitor design operating at about 1 GHz, has been integrated  into an Atomic Force Prober system [2].


Background


Historically, capacitance-voltage plots on kerf test site  structures have been generated to monitor such gate oxide


characteristics as oxide thickness (TOX) effective oxide  thickness (EOT), and overlap capacitance (COV) , among other  parameters.


Figure 1 shows an interesting capability incorporated into the  Atomic Force Prober enabling capacitance measurement  capability while imaging a memory array .  Using SCM at the  contact level has been shown before [2].  However, Figure 1  shown here is significant because the contrast in the  highlighted contact is related to the doping and not to a current  contrast mechanism such as leaky gates or silicide defects.  Therefore, it will not be highlighted by a current imaging  techniques such as PicoCurrent.


Figure 1: (TOP): AC Capacitance NCVS localization of low  dopant site of PFET device in a 45 nm SOI SRAM array.  The  contrast is not due to a smaller capacitance signal but a shift  in the effective flat band voltage relative to its neighbor as  shown by the embedded dC/dV vs V curves. (BOTTOM)


Also, the sample is an SOI part whose substrate has a buried  oxide layer isolating the Rx active area from the underlying  silicon substrate and therefore has no contact to the backside  of the die.  Such defects are tricky to locate using other  methods, but in the capacitance image, the CV flatband shift  in the implant connected to the contact is easily measured.  There is sufficient capacitive coupling through the barrier  oxide (BOX) to allow the contrast mechanism shown.  The  contrast mechanism is explained by the acquisition of AC  capacitance (dC/dV vs V) curves from the bright contact and  its neighbor. The vertical positions of the two curves are about  the same at the bottom of the figure (that is, the magnitude of  dC/dV is about the same) but the curve of the bright contact is  shifted about 500mV lower (to the left).


Since the image in Figure 1 is taken using the standard method  of applying an AC bias to the sample and demodulating the  resulting sensor signal using a lock-in-amplifier, the data  actually represent the derivative of the CV curve.  This  method of measuring the slope of the CV curve was pioneered  by Williams and is traditionally called SCM or Scanning  Capacitance Microscopy [10,11].  While it is possible to  integrate the AC capacitance curves to get a DC CV curve, the  results are still uncalibrated [12].


In order to calibrate the measurements of the NCVS, we  devised an experiment whereby a test structure with many  fingers of gates was measured at the BEOL level with a  conventional CV impedance analyzer.  After that  measurement, the same test structure was unlayered to contact  and analyzed by nanoprobe.  By removing Metal 1, the  source/drain fingers become isolated and can be individually  measured.  More importantly, the nano CV measurements  obtained at CA contact level on individual fingers can be  validated by comparison with the pad level data [3,4,5,6,7,8].  By extension, NCVS at CA contact level can provide a means  to localize dopant defects, identify anomalous buried trench  capacitor leakage, resistive back end of line (BEOL) via  stacks, especially for silicon on insulator (SOI) substrates with  a buried oxide layer that isolates the Rx active silicon area  from the underlying silicon substrate.


Description


The Atomic Force Probe (AFP) is routinely used to probe the  very closely spaced terminals of nanoscale transistors. Nanoprobing with various methods has made parametric  characterization of deep submicron sized devices possible [13,14,15].  The authors of this paper  favor the use of Atomic  Force Probing for reasons (no charge damage and Vt integrity) that have been described previously [15]. Collection of IV  parametrics through nanoprobing is now a common technique  for failure analysis in the most advanced semi technology  nodes.  Two factors are behind the trend:


1. IV parametrics can provide key information in  diagnosing the cause of a failure.


2. Conventional microscopy techniques, such as SEM, FIB, LSM (and its optical cousins), and even TEM  are becoming very difficult and unproductive in the  sub-100 nm regime [17].


The physics behind the trend is that each of the microscopic  techniques that are used in FA relies upon an interaction  between a roughly optimized probing beam (optimized, because these techniques are largely mature) and an ever  shrinking defect.  In contrast, IV measurements, even in  nanoscale transistors, are just as effective in determining  failure causes because the transistor is such a good defect  detector in and of itself.  The huge beta gain in these devices is  as good as or better than it was when they were orders of  magnitude larger.  Therefore, the only challenges for IV  nanoprobing are:


1. Making good contact to the device, which is  complicated by ever shrinking contacts and  changing materials.  This includes navigation to  memory cells and failing nets;


2. Providing clean, low leakage connections between  test equipment and the DUT;


3. Not affecting the sensitive device properties with  the measurement tools;


The AFP measurements presented here were carried out on  samples without any Focused Ion Beam or Electron Beam  imaging or modifications [16].


In contrast with IV parametric measurements at the nanoscale, NCVS does not share the benefit of using the device’s gain to  detect defects.   The capacitance sensor itself must be able to  measure the tiny amounts of charge flowing as the capacitance  is measured.  The sensitivity required for NCVS  measurements on real devices is equal to a typical gate  capacitance.  For a minimum design rule transistor, as would  be found in an SRAM array, the Cg is considerably less than a  femtoFarad.  The good news is that for MOSFET scaling  rules, the value has remained roughly constant for all nodes.  While the doping increases, the area shrinks, and the effective  gate oxide thickness shrinks at the same pace leaving the  capacitance and channel charge numbers roughly constant.  Therefore, a tool designed for 45 nm features will also likely  function with 32 nm features.  The only complication in this  argument is the fact that the leakage current for ultrathin  oxides increases exponentially with the decrease in dielectric  thickness.  Figure 2 shows a block diagram of the NCVS  electronics used in the paper.  The resonant sensor is not as  strongly sensitive to leakage currents as the standard bridge  type design.


Figure 2.  NCVS sensor and electronics block diagram.  The  curves can be extracted in two places: the “SCM” (as dC/dV  vs. V) and the “Sensor Output” (as C vs V).  The C vs. V  curves are the ones which have been calibrated in the present  study.  The image and curves in Fig 1 are from “SCM”.  The  Lock in Amplifier provides significant noise reduction for  imaging, at the expense of  losing the absolute value of  capacitance.


In addition to the extremely small capacitances involved, CV  metrology is also complicated by the proximity of  source/drain implants and the ready supply of minority  carriers and variations of channel doping with LDD, halo, and  threshold implants.  Therefore, conventional CV  measurements at the probe pad level are not used as a fault  localization technique.


The Impedance Analyzer’s resolution limit is far above the  capacitance of discrete devices and conversely, the  capacitance of a test structure far higher than that of a discrete  scanning capacitance sensor.  Therefore, the method used to  compare the data from each tool is to use a test structure, as  shown in Figure 3, measured at metallization, and then  delayered to expose smaller segments of the structure for  discrete NCVS probing.


The test structure has a total capacitance of about 0.6 pF and is  made up of 270 unit cells.  A unit cell is a gate finger  surrounded by a source-drain with a capacitance of about 2  femtoFarads.  On the particular test structure, the gate fingers  are connected at poly but the sources are only connected by  Metal 1. By removing M1, the individual tubs are isolated and  can be singled out as indicated by the dotted line in Figure 3.   Because the gates are all common, the gate was grounded and  the active probe was placed on one of the source contacts.  The measurements will still have a small Rs associated with  the silicide resistance across the finger and the contact  resistance of the probe to the contact.  The contact and probe  resistance together are less than 100 ohms, but the average  silicide resistance could be 100 ohms between each tungsten  contact on a small geometry FET.  See reference [18] for a  typical measurement of these values.


The total resistance is approximately:


Rseries = RProbe + RContact + RSilicide  300


The effective impedance of the finger is described by:


≅


≅ 83 k


This leads to the  happy result that series resistance can be  neglected, and only the capacitance will be measured:


Rseries <<


Figure 3.  Capacitance test site structure designed to minimize  series resistance, Rs ;  Blue = RX, Gold = PC, Green = CA, Red = M1  For the NCVS measurements the M1 was removed, one of the S/D fingers (shown in the box) was contacted with  the nano CV probe, and one of the gate contacts was  grounded.  The test structure has 270 fingers.  Cox is  approximately 0.6pF for all of the cells and an individual cell  is about 2 fF.


The resonant sensor design offers a further benefit because it  is very close to the DUT and has almost no parasitic cabling  capacitance.  Unlike the bridge transducer common to  traditional impedance analyzers, the resonator design is  unaffected by any dielectric leakage current flowing in the  DUT.  The drawback of this design so far is that the amplitude  in the resonator must be optimized so that it has sufficient  strength to measure values much less than a femtoFarad, but is  not so large that it causes unacceptable CV stretch out.  As  shown in Figure 2 there are two types of nano CV data: the “SCM” as dC/dV vs. V and the “Sensor Output” as C vs V.  The C vs. V curves are the ones calibrated in the present  study.  The image and curves in Fig 1 are from “SCM”.  The  Lock-in Amplifier provides significant noise reduction for  imaging at the expense of the loss of the absolute value of  capacitance.


Correlating specific defects in the test site structure with the  in-line C-V measurements offers opportunities for further


FEOL yield learning, and process control, especially for  scaled SION gate films (Eot < 1.5 nm) or high-k films.  Unlayering and performing multiple NCVS measurements at  the contact level of discrete FET devices comprising a C-V  test structure enables the localization of defect(s) indicated by  in-line C-V measurements. In addition, NCVS complements  conventional in-line capacitance-voltage measurements of test  site structures probed at the back end of line (BEOL) pad level [4,5,6,7,8].


Conventional C-V measurements at the probe pad level are  shown in Figure 4.


Figure 4:  Voltage versus capacitance data of the in-line  NFET test site structure shown in Figure 1 at 30 MHz.  Several corrections are necessary, due to leakage current  contributions as well as cable and M1 pad capacitance.


Measuring the C-V characteristics of a single finger of a  multifinger test site structure at CA by nano probing and  correlating them to pad level conventional CV measurements  represents an important advance in deep submicron device  characterization.


NCVS vs. Pad Level C-V Impedance Measurements


A 110 MHz frequency C-V impedance analyzer employing  the IV method for a grounded device was employed to  perform capacitance voltage measurements at the pad level of  the structure described in Figure 3 [4,5,6]. Next, as described  above, the same capacitance test structure was delayered to the  CA level and a single PC finger was characterized by NCVS.


Figure 5. Comparison of Pad Level C-V measurements (righthand scale) versus NCVS measurements (left-hand scale).  The  110 MHz bridge type impedance analyzer is strongly  influenced by leakage in the gate oxide film.  The NCVS data  taken with the GHz resonator is unaffected by leakage current  in the film but suffers some CV curve stretch-out from the  slightly higher GHz probing amplitude.  Optimization is in  progress.


The 110 MHz measurement suffers from excessive leakage in  the dielectric film above the flatband voltage and therefore the  data is inaccurate in accumulation. Excluding the signal  indicated by gate oxide leakage above 0.5 volts for this 1.5  volt Vdd technology, the capacitance at Vgs = 0.3 V of  approximately 3x10-13 F agrees with the in-line capacitance  measurements at 30 MHz (Figure 4).


The NCVS measurements at 1 GHz have a similar mid point  at 0.3 V, but as can be seen in the graph, the CV transition  takes place over a larger voltage than either of the standard 30  or 110 MHz curves.  If the standard methods can be taken as  accurate (there is a significant difference between them as  well) then we can conclude that the GHz data suffers from  stretch-out, a symptom of too high a probing voltage.   The  GHz data does not show any susceptibility to leakage in the  measurement and is therefore an improvement over the  standard measurements.  Because the total gate capacitance (Cgon) for one finger is about 2 femto farads, the measurement  is somewhat noisy.  These measurements validate the CA  level capacitance measurements obtained by (NCVS).  Nano  CV characterization offers opportunities for further FEOL  yield learning and process control, especially for scaled SION  gate films (Eot < 1.5nm) or high-k films.


In particular, for SOI technologies with buried nodes not  accessible at CA contact level, NCVS has already shown the  sensitivity to detect trench capacitor leakage in embedded  DRAM cells [2].


2 CAs, open corrected  4 CAs, open corrected  Corrected for CA-PC  & M1-PC Capacitance


Nano CV characterization offers opportunities for further  FEOL yield learning, process control, especially for scaled  SION gate films (Eot < 1.5nm) or high-k films. Nanoprobe  Capacitance Voltage Spectroscopy has demonstrated the  ability to detect buried trench capacitor leakage in SOI  embedded DRAM cells [2].  Correlating the NCVS  measurements, obtained at CA contact level on a finger of a  C-V test structure, with conventional C-V measurements at the  pad level have validated this new technique, especially for  characterizing discrete MOSFET devices.  The further scaling  in MOSFET gate length features enabled by high k gate films  underscores the importance of NCVS to detect trapped charge, gate-drain overlap (Miller Capacitance), as well as dopant  fluctuations in discrete devices.


It has been shown that a means is now available for AFPassisted SCM or multiple NCVS localization of junction  defects and electrical C-V measurements of gate oxide defects  without the exacting and time-consuming sample preparation  steps of conventional SCM analysis [10,11,12,13]. This  approach permits accumulation / inversion mode imaging and  rapid localization of the defect in the MOSFET (source or  drain) device.  Multiple AFP probe tips permit independent  biasing of source/drain tungsten via level contacts  simultaneously with AFP contacts to the gate for discrete  device C-V measurements.


The authors wish to acknowledge the efforts of Bruce Redder, Chris Molella and Paul Ronsheim of IBM in the sample  preparation procedures. Also the authors wish to acknowledge  the technical input of Jeff Snare and Kevin McStay for  technical C-V discussions


1.  E.H. Nicollian, J.R. Brews, MOS (Metal Oxide


Semiconductor) Physics and Technology, “C-V Curves,       pp. 384-385, (1984)


2. T. Kane, M. Tenney, A. Erickson, S. Phan, Challenges of


Atomic Force Probe Characterization of Logic Based


Embedded DRAM for on-Processor Applications, ISTFA


2007,  pp. 46-51 (2007)


3. Schmitz, J. ,  Test Site Design for Thin Gate Film


Capacitance Measurements, ICMTS, 2003


4. Verzi, B, Fundamentals of Ultra-Thin Gate Dielectric


Measurements, Agilent HF-CF Solutions, March 2004


5. Verzi, B. Novel Method to Measure Thin Gate Oxide


Films, International Conference of Solid State Device and


Materials, 2002.


6. Okawa, et. al. , Method for Measuring Thin Gate Oxide


Films, ICMTS, 2003.


7. T. Ishida, et. al., Microscopic C-V Measurements of SOI


Wafers by Scanning Capacitance Microscopy, Eur. Phys.


J. Appl. Phys. 27, 479-482 (2004).


8. Jean-Yves Rosaye, et. al. C-V and C-P Characterization


Sensitivities for Fast and Slow-State Traps in Very Thin


Oxide MOSFETS, Proceedings of International


Reliability Physics Symposium, pp. 353-35 (2004).


9. Matey, J.R. and Blanc, J.  Scanning Capacitance


Microscopy, J. Appl. Physics, 57 (5), 1 March 1985, pp.


[5] F. Beaudoin, D. Carisetti and al. “Backside failure  analysis of GaAs MMIC ASICs” The European  Physical Journal Applied Physics, 27 (1-3), p. 475, september 2004


[6] R. Pazirandeh, U. Zeimer, H. Kirmse, J. Wüfl, G. Tränkle, W.Österle “Defect analysis of degraded  InGaP/GaAs HBTs” 2004 IEEE CSIC digest.


[7] R.Lossy, N.Chaturvedi, P.Heymann, K. Köhler, S. Müller and J. Würfl “AlGaN/GaN HEMTs on Silicon  Carbide Substrates for Microwave Power Operation” International


conference


on


compound  semiconducteur Mfg (GaAsMANTECH) 2003.


[8] D. Mahaveer Sathaiyaa, and Shreepad Karmalkar “Thermionic trap-assisted tunneling model and its  application to leakage current in nitrided oxides and  AlGaN/GaN high electron mobility transistors ”


Journal of Applied Physics, Vol. 99, 2006.


[9] Shreepad Karmalkar, Naresh Satyan, and D. Mahaveer Sathaiya “On the Resolution of the  Mechanism for Reverse Gate Leakage in  AlGaN/GaN HEMTs” IEEE Electron Device Lett, Vol. 27, February 2006


[10]: W. Lu, V. Kumar, R. Schwindt, E. Piner, I. Adesida, “A comparative study of surface passivation on  AlGaN/GaN HEMTs” Solid-State Electronics, 1441-1444,  46 (2002)


DOI: 10.1361/cp2008istfa220


Photon Emission Spectral Signatures of AlGaN/GaN HEMT for Functional and  Reliability Analysis


Arkadiusz Glowacki, Christian Boit


Berlin University of Technology, Berlin, Germany  Einsteinufer 19, Sekr. E2, D-10587 Berlin, Germany  phone: +49-30-314-24922  fax: +49-30-314-25526  E-mail: aglowa@mikro.ee.tu-berlin.de


Richard Lossy, Joachim Würfl


Ferdinand Braun Institut für Höchstfrequenztechnik, Berlin, Germany


Non-degraded and degraded AlGaN/GaN HEMT devices have  been characterized electrically and investigated in various  operating modes using integral and spectrally resolved photon  emission (PE). In degraded devices the PE dependence on the  gate voltage differs from the non-degraded devices. Various  types of dependencies on the gate voltage have been identified  when investigating local degradation sites. PE spectroscopy  was performed at various bias conditions. For both devices  broad spectra have been obtained in a wavelength regime from  visible to near-infrared, including local performance variations. Signatures of the degradation have been determined in the  electrical characterization, in integral PE distribution and in  the PE spectrum.


AlGaN/GaN devices have the advantage of a two dimensional  electron gas (2DEG) in the channel for high speed applications  and a wide band-gap, extremely attractive for power  electronics applications. AlGaN/GaN high-electron mobility  transistors (HEMTs) are on their way to volume production  and have recently received much attention for their ability to  operate at high power levels. PE investigation results for  AlGaN/GaN HEMT devices are presented in this paper to  show the ability of the technique to not only localize weak  spots in the device but also deliver information about the  degradation mechanism and defects.


At first, the HEMT devices have been analyzed by PE integral  intensity measurements. Some devices have been intentionally  stressed to induce degradation in order to observe the  influence of the degradation on the PE integral intensity  distribution. Next, non-degraded and degraded devices have  been chosen for further analysis: electrical characterization  and most importantly spectrally resolved PE measurements. The PE spectra of the non-degraded and degraded devices  operated at different conditions (in on state and in pinch-off) have been analyzed and the degradation signatures have been  determined.


AlGaN/GaN technology & experimental setup


The high power, high gain Al0.25Ga0.75N/GaN-HEMT  structures   were designed and fabricated in Ferdinand Braun  Institut für Höchstfrequenztechnik, Berlin, using MOCVD  technique for epitaxial growth. The transistors are fabricated  using i-line stepper lithography in combination with electronbeam lithography for the T-gate structures (0.4 µm gate  length). A cross-sectional view of those devices is shown in  Fig. 1.


Figure 1: Cross sectional view of the 0.4µm gate length  AlGaN/GaN HEMT.


The layer sequence on top of a 400µm thick semi insulating  SiC substrate consist of a nucleation layer, following a 2.2µm  GaN buffer layer and a 25nm AlGaN (26% Al content) barrier  layer. A 2-dimensional electron gas (2DEG) quantum well is  formed under the AlGaN barrier layer which acts as transistor  channel.  A Ti/Al/Ti/Au metallization scheme covered with  WSiN/Au overlay metal is employed for the fabrication of the  source/drain ohmic contacts in such a way that pattern  delineation during rapid thermal annealing at 830°C is  preserved [1,2]. In order to optimize power density and gain, the transistor gate is designed as T-shape with a gate foot  length of 0.4µm. The distance between the source and drain  edge and the gate foot is 1µm and 6µm, respectively. The gate  contacts are made using Pt/Au metallization in order to create  the Schottky barrier.


The electrical measurements have been carried out using a  semiconductor parameter analyzer and the photon emission  measurements have been performed on the Hamamatsu  Photon Emission Microscope – Phemos 1000. The system is  equipped with a cooled Si-CCD detector with spectral  sensitivity in the visible and near infrared regime.


Device under test, degradation test and electrical  characterization


The employed sample is 4 finger x 125 µm, AlGaN/GaN  HEMT with via holes manufactured in technology  characterized in the previous chapter. No cap was used in this  particular device structure. The maximum safe power was  estimated at the level of 6W/mm. The top view of the device is  shown in the Fig. 2.


Figure 2: Top view of the device


The device has been stressed using a type of lifetime test. The  voltage of 28V has been applied to the drain and the  experimental setup has been configured to keep constant  power level of 3W and monitor the gate voltage. The stress  test progress waveform is shown in the Fig. 3.


Figure 3: The stress test progress waveform. The device  characterization moments are indicated with arrows.


The device degraded gradually without sudden gate current  increase. The device has been electrically tested before and  after the degradation test in moments indicated by arrows in  the Fig. 3. The results of the degradation on the output IV  characteristic and transfer characteristics are shown in the Fig.


4 – 6. The drain current decreased drastically with the  degradation while the gate current shows opposite tendency. In addition, the gate current for a degraded device becomes  positive at positive gate voltages, which is not the case for a  fresh, unstressed device.


Figure 4: The influence of the degradation on the output IV  characteristics


Figure 5: The influence of the degradation on the output  transfer, Id=f(Vg) characteristic @ Vd=15V.


Figure 6: The influence of the degradation on the output  transfer, Ig=f(Vg) characteristic @ Vd=15V.


PE distribution characterization


The PE distribution differs between the fresh and degraded  device and depends on the electrical operating condition.


Fresh, unstressed device has homogenous distribution of  photon emission. The PE inhomogeneity is visible only in the  pinch-off condition when no significant current flows through  the device. Once the channel is opened the current-related  homogenous photon emission becomes dominant. The PE  distributions of the fresh, reference device in pinch-off and on  state are shown in Fig. 7.


Figure 7: The 3D and 2D plots of the PE intensity of a fresh  device in pinch-off (top) and in on condition (bottom). The    circles and arrows indicate the locations/areas of interest for  further analysis.


The PE intensity integrated over the entire device area as a  function of the gate voltage and at constant Vd=10V is  presented in Fig. 8. The PE reaches a maximum at an  intermediate level of the gate voltage (around 0V). The  characteristic has a shape similar to the one known from the  MOSFETs, although the physical origin is different. Here, this  kind of shape is a combined effect of the transistor channel  behavior and the Schottky diode behavior. For the electrical  conditions indicated by circles, the PE spectrum has been  acquired.


As far as the stressed, degraded device is concerned the  situation is different. The PEM results show inhomogeneous  PE distribution all over the device regardless the electrical


condition. There are plenty of locations characterized by  stronger PE. The dependence of the intensities of the localized  photon emissions on the electrical condition vary from  location to location. Some locations characterized by the  strongest PE intensity have been chosen to show the  dependence of the intensity on the gate voltage and to acquire  the PE spectrum. Those locations are marked in Fig. 9.


Figure 8: The transfer Id=f(Vg) and the PE intensity as a  function of gate voltage @ Vd=10V for the fresh, unstressed  device. The circles indicate the electrical conditions for the PE  spectrum analysis.


The PE intensity integrated over the entire device area as a  function of the gate voltage is presented in Fig. 10. There is a  wide local maximum plateau in the range of gate voltage  values between -3V and -1V. As the gate voltage is increased  above 1V the drain current and therefore the PE intensity  increase rapidly. This rapid PE increase may be due to the  abnormal gate current behavior as presented in Fig. 6. The  gate current also increases rapidly in the positive gate voltages  regime.


When the PE intensity is integrated over the entire device area  the PE intensities of specific locations in the device are added  together. Therefore, it is not possible to isolate the pure  dependencies of PE intensities of those locations on the gate  voltage. To achieve this, maximum PE has been analyzed only  at these specific locations as indicated by the arrows and  circles in the Fig. 9. This has been repeated at various gate  voltages. The result is shown in Fig. 11 and 12 in linear and  logarithmic scale respectively.


Two groups of locations can be distinguished in terms of the  dependence type of the PE intensity on the gate voltage. In the  first group are locations that are characterized by PE intensity  having a peak maximum within the range of applied gate  voltages. The locations belonging to the second group are  characterized by the PE that is increasing with the gate voltage  without any peak maximum. Area #2, #3 and #4 belong to the  first group.  The PE intensity in areas #2 and #3 reaches a  maximum at -3V whereas in area #4 it is happening at -2.25V. Areas #1, #5 and #6 belong to the second group.


Figure 9: The 3D and 2D plots of the PE intensity of a  degraded device in various electrical conditions. The circles  and arrows indicate the locations of interest for further  analysis.


Figure 10: The transfer Id=f(Vg) and the PE intensity as a  function of gate voltage @ Vd=10V, for the degraded, stressed  device. The circles indicate the electrical conditions for the PE  spectrum analysis.


Figure 11: The transfer Id=f(Vg) and the PE intensities of the  locations indicated in Fig. 9 as a function of gate voltage @ Vd=10V, for the degraded, stressed device.


Figure 12: The transfer Id=f(Vg) and the PE intensities of the  locations indicated in Fig. 9 as a function of gate voltage @ Vd=10V, for the degraded, stressed device.


PE spectrum analysis


A set of broadband interference filters with the central  wavelength  ranging from 450 nm to 950 nm have been used  in order to collect the spectrum of the PE from the analyzed  devices. The filter FWHM parameter was in a range from 45  nm – 90 nm. For each filter case, after the detection of the  integrated PE intensity, the background PE has been  subtracted. Then, the measurement results have been  calibrated by the transmission characteristics of the optical  path components and the quantum efficiency of the Si-CCD  detector.


The PE spectrum has been analyzed in various electrical  conditions as indicated in Fig. 8 and 10 for fresh and degraded  devices respectively.


First the total PE intensity, integrated over the entire device  area has been characterized in terms of its spectrum at various  bias conditions. The results for the fresh, reference device is  presented in Fig. 12 and 13 as function of the wavelength and  photon energy respectively.


Figure 12: Photon emission spectra acquired for the fresh, unstressed device at various gate voltage values and Vd=10V (PE intensity as a function of wavelength).


Figure 13: Photon emission spectra acquired for the fresh, unstressed device at various gate voltage values and Vd=10V (PE intensity as a function of photon energy).


The observed spectrum does not originate from the direct  band-to-band recombination, as the bandgap energy of the  GaN material is 3.4 eV (out of Si CCD spectral range). In  silicon FETs, PE intensity increases exponentially into IR  representing an intra-band relaxation of carriers that picked up  kinetic energy in the strong field of the pinch off region in  near–Boltzmann distribution.  In case of GaN devices, the PE  spectrum of the devices has two characteristic features. For the  device operated in on-state the PE spectrum has a kink at  around the wavelength of 700 nm (1.77 eV) and reaches a  maximum at 850 nm (1.46 eV). For the device operated in the  pinch-off there is additional maximum at around the  wavelength of 750 nm (1.65 eV). The additional maximum  comes from the PE emissions located at the ends of the fingers, as indicated in Fig. 7 (top). The spectra of the maximum PE  from the locations indicated in Fig. 7 have been measured and  are presented in Fig. 14. Clearly, the PE spectrum has two  peaks: at 750 nm (1.65 eV) and 850 nm (1.46 eV).


Figure 14: Photon emission spectra acquired for the fresh, unstressed device in pinch-off condition (Vg=-5V and  Vd=10V) for the areas #1 and #2 as indicated in Fig. 7. PE  intensity plotted as a function of wavelength.


In case of stressed, degraded device the spectrum of the total  PE integrated over the entire device has been acquired at  various electrical conditions as indicated in Fig. 10. The  spectra are shown in Fig. 15 and 16. Regardless of the  electrical condition the overall PE spectra has two  characteristic points. Similarly to the fresh device case the  kink at around 700 nm (1.77 eV) exists and is followed by the  PE spectrum maximum at around 850 nm (1.46 eV). However, there is no maximum observed at the wavelength of 750 nm (1.65 eV) for a device operated in the pinch-off state. Another  difference is that the peak at 850 nm (1.46 eV) looks less  pronounced and kind of blurred in some other PE feature  characterized by continuous increase of the PE intensity with  the wavelength. Finally there is a relative intensity increase in  the short wavelength regime at negative gate voltages, which  has not been observed for the fresh device. This is most likely  mainly due to the PE contribution from the locations of the  type of A2 and A3 which show relatively strong PE intensity  at negative voltage and in the pinch-off condition.


Figure 15: Photon emission spectra acquired for the  degraded, stressed device at various gate voltage values and  Vd=10V. PE intensity plotted as a function of wavelength.


Figure 16: Photon emission spectra acquired for the  degraded, stressed device at various gate voltage values and  Vd=10V. PE intensity plotted as a function of photon energy.


The spectra have been acquired at locations indicated in Fig. 9  in order to find out if there are other spectrum features  characteristic only to localized degradation-related PEs. For  each of those locations the spectrum has been acquired for the  device operated in the electrical condition ensuring the  maximum PE intensity condition at this location, as indicated  in Fig. 11. The results of these measurements are presented in  Fig. 17 and 18 as a function of wavelength and photon energy  respectively.


The features already identified in the spectrum of the PE  intensity integrated over the entire device area are also present  in the PE spectrum of the particular degradation sites. The  kink is present at the wavelength of 700 nm (1.77 eV) and  local maximum at 850 nm (1.46 eV). In addition there are  additional peaks at the wavelengths of 750 nm (1.65 eV) and  780 nm (1.59 eV) for areas #1 and #2 respectively. The peak  at 750 nm (1.65 eV) has most likely the same physical  background as the peaks identified in the PE spectra at the


finger ends of the fresh device operated in the pinch-off  condition. It is possible that the fresh devices have weaker  version of degradation sites similar to those introduced by  application of the stress to the device. The additional peak at  780 nm (1.59 eV) may originate from slightly different  degradation type.


Figure 17: Photon emission spectra acquired for the  degraded, stressed device for the areas #1 - #6 as indicated in  Fig. 9, for electrical condition adjusted for each location in a  way to ensure the maximum PE intensity condition at this  particular location. PE intensity plotted as a function of  wavelength.


Figure 18: Photon emission spectra acquired for the  degraded, stressed device for the areas #1 - #6 as indicated in  Fig. 9, for electrical condition adjusted for each location in a  way to ensure the maximum PE intensity condition at this  particular location. PE intensity plotted as a function of  photon energy.


Photon emission in AlGaN/GaN HEMTs was studied under  the reliability requirements point of view. Fresh, non-degraded  and degraded devices were subject of investigation. Signatures  of the degradation have been determined in the electrical  characterization, in integral PE distribution and in the PE  spectrum. In terms of current consumption, degraded devices


are characterized by much lower current level. The  distribution of the PE integral intensity of the degraded device  is strongly inhomogeneous, unlike in case of reference, fresh  device. The spectrum of the PE from degradation sites has  additional maxima in the shorter wavelength regime. Similar  maxima are observed in fresh sample operated in the pinch-off  condition suggesting that the degradation mechanism  accelerated during a stress test is an enhanced version of what  is already present in the fresh sample.


Our results indicate clearly that the spectrally resolved PE  measurements can serve as significant help in the  identification of the degradation sites and mechanisms in  abnormally operating devices as well as to deliver additional  information about the trap centers or defects.


In comparison to other publications, for instance as presented  in [5], [6] and [7] our results differ slightly in terms of the  AlGaN/GaN HEMTs PE spectra. The mentioned publications  do not report any remarkable spectra features in the range of  photon energies of 1.5 – 2.5 eV as it was observed during our  experiments.


Possible mechanisms behind such a subgap emission are:


- intraband transitions of highly energetic electrons due to  scattering by charged centers,


- phonon assisted intraband transitions of electrons,


- direct intraband transitions of electrons,


- recombination via deep levels


as also listed in [5] and need to be investigated in detail. Such  a detailed study should be a subject to much wider research  program.


We would like to thank Hamamatsu Photonics K.K., Hamamatsu Photonics Germany, for their support of  experiments with equipment and advice and Reza Pazirandeh  from Ferdinand Braun Institut für Höchstfrequenztechnik for  his support of experiments with test structures and valuable  discussions.


[1] High power, high gain AlGaN/GaN-HEMTs with novel


powerbar design, R. Lossy, A. Liero, J. Würfl and G.


Tränkle,  IEDM-Transactions 2005 Washington DC,


pp580 – 582.


[2] Large area AlGaN/GaN HEMTs grown on insulating


silicon carbide substrates, R. Lossy, J. Würfl, N.


Chaturvedi, S. Müller and K. Köhler, physica status solidi


(a) Vol.194 (2), 2002.pp. 460-463.


[3] Fundamentals of Photon Emission in Silicon, C. Boit,


Microelectronics Failure Analysis, fifth Edition


2005,EDFAS, ASM International, ISBN: 0871708043,


p356-368.


[4] Analysis of Hot Carrier Transport in AlGaAs/InGaAs


Pseudomorphic


HEMT’s


means


Electroluminescence, G.Meneghesso et al, IEEE Trans.


Electron Devices, vol.47, no.1, Jan.2000 p2-10.


[5] Electroluminescence in AlGaN/GaN HEMTs, Nakao


Takeshi, Ono Yutaka, Akita Mitsutoshi, Kishimoto


Shigeru, Maezawa Koichi,  Mizutani Takashi, IEIC


Technical Report, Vol. 102, no.80, Page 53-67, (2002)


[6] Electroluminescence in AlGaN/GaN High Electron


mobility Transistors under High Bias Voltage, Nakao


Takeshi, Ohno Yutaka, Akita Mitsutoshi, Kishimoto


Shigeru, Maezawa Koichi,  Mizutani Takashi, Jpn. J. Appl.


Phys. Vol. 41 (2002) pp. 1990-1991


[7] A review of the failure modes and mechnisms of GaNbased HEMTs, Enrico Zanoni, Gaudenzio Meneghesso,


Giovanni Verzelessi, Francesca Danesin, Matteo


Meneghini, Fabiana, Rampazzo, Augusto Tazzoli, Franco


Zanon, IEDM07, Tech. Digest, IEEE International


Electron Device Meeting - Washington DC, 2007, pp. 381-


384.


DOI: 10.1361/cp2008istfa227


Laser Scanning Localization Technique for Fast Analysis   of High Speed DRAM devices


Martin Versen, Achim Schramm, Jan Schnepp  Sascha Hoch, Tapan Vikas


Qimonda AG, Am Campeon 1-12, D-85579 Neubiberg, Germany


Dorina Diaconescu


Infineon AG, Otto-Hahn-Ring 6, D-81739 München, Germany


Soft defect localization (SDL) is a method of laser  scanning microscopy that utilizes the changing pass/fail  behavior of an integrated circuit under test and  temperature influence. Historically the pass and fail  states are evaluated by a tester that leads to long and  impracticable measurement times for dynamic random  access memories (DRAM). The new method using a  high speed comparison device allows SDL image  acquisition times of a few minutes and a localization of  functional DRAM fails that are caused by defects in the  DRAM periphery that has not been possible before. This  new method speeds up significantly the turn-around time  in the failure analysis (FA) process compared to  knowledge based FA.


Standard methodologies for laser scanning localization  technique are shown in Fig. 1 and 2. The methods in Fig. 1 are known as TIVA (Thermally Induced Voltage  Alteration) and OBIRCH (Optical Beam Induced  Resistance Change): a constant current or voltage source  is applied to the device under test (DUT) and a voltage  or current drop or increase is measured at the device, respectively [1-4].


Both methods use an analogue input of the microscope  electronics. The input is valid basically throughout the  complete pixel dwell time, the time that is needed to  measure one location on the DUT. The disadvantage is  that local defects within a DRAM cannot be localized as  the interface and output does not change in case of an  array defect. For most problems, bitmapping of DRAM  array related failures and TIVA and OBIRCH for power  net problems in the periphery, the tool set is complete.


Nevertheless, functional failures that are caused by  soft defects in the periphery cannot be analyzed as they  have neither array specific addresses for bitmapping nor  a VDD dependency for TIVA or OBIRCH. Soft defect


localization (SDL) methods allow a localization of  functional fails within the periphery of the DRAM that  are not accessible with any bitmap. Laser scanning  localization with a test system utilizes the trigger or    synchronous  input of the microscope electronics shown  in Fig. 2: a functional pattern is executed and any local  defect may cause a fail depending on the pattern. The  tester evaluates the pass or fail result from the DUT and  sends a digital signal together with a trigger to the  microscope electronics.


Figure 1: Laser scanning localization setup with analog  input.


Figure 2: Laser scanning localization setup with  synchronous input.


DUT  Laser


PASS/FAIL information


Microscope  electronics X/Y location


Tester


Trigger  DUT


I/V information


X/Y location


Microscope  electronics


This technique allows the localization of any  temperature dependent defect that causes any function  failure. There are also some modifications to this method  to improve the signal to noise ratio. One example is the  use of a lock-in assisted SDL [5], but unfortunately  standard and the improved methods can not be used for  DRAMs.


The reason is that the operation frequencies are in >100 MHz range which require a memory test system  with quite long test execution times. The total test  runtime is usually much longer than the minimum pixel  dwell time. The test runtime consists of the pattern run  time itself and a test evaluation time of the used memory  test system. The test evaluation time that is required  before the next test is executed is also called test-to-test  index time and amounts roughly to 300ms which is  much longer than the pixel dwell time. The consequence  is that the pixel dwell time must be adjusted. If a  128x128pixel image should be acquired with this test-totest index time, a scan time of 82min (=128x128x  300ms) would be required and the method is not  applicable to DRAM with this memory test system.


Nevertheless there has been an attempt to utilize the  laser scanning methods for DRAMs [6]. Fig. 3 shows an  experimental configuration, in which a DRAM output is  directly connected to the microscope electronics using  again its analog input. The DRAM is operating at 100  MHz and the data speed is 200Mb/s. As the executed  pattern is a continuous Read, the output becomes quasistatic. The PASS/FAIL information is implicitly encoded  in the data out information. The usage is only limited as  any interruption of the continuous read, thus any  modification of the pattern, changes the measurable  signal. So this method is not generally applicable.


Figure 3: Laser scanning localization setup with analog  input, but tester excitation.


The newly proposed methodology is depicted in Fig.


4. It is a laser scanning localization technique similar to  the standard synchronous technique with the exception  that the tester only drives the DUT. The single bit  comparator (SBC) compares the data received with


previously programmed data values and sends either a  low or a high signal pulse (the PASS/FAIL signal form  before) to the analog input of the microscope. The  advantages are a data speed of up to 200Mb/s and an  adjustable pulse length for the PASS/FAIL signal that  can be changed according to both the pattern run time  and the pixel dwell time.


Figure 4: Laser scanning localization setup with the new  instrumentation, the Single Bit Comparator (SBC).


The next part of this paper describes the functional  blocks of the SBC, while the third part gives some  timing characteristics of the SBC. The fourth part shows  the successful demonstration and the application of the  new tool in the Failure Analysis (FA) lab.


1437-1444.


10. CC. Williams, J. Slinkman, W.P. Hough, H.K.


Wickramasinghe, “Lateral Dopant Profiling with 200nm


Resolution with Scanning Capacitance Microscopy”,


Appl. Phys. Lett. 55, 1662 (1989).


11. C.C. Williams, J. Slinkman, W.P. Hough, H. K.


Wickramasinghe, “Two Dimensional Dopant Profiling


using Scanning Capacitance Microscopy”, J. Vac. Sci.


Technol. B n. 8, 895 (1990)


12. V.V. Zavyalov, J. McMurray, C.C. Williams, Surface and


Tip Characterization for Quantitative Two Dimensional


Dopant Profiling by Scanning Capacitance Microscopy,


from Characterization and Metrology for ULSI


Technology: 1998 International Conference, American


Institute of Physics (AIP) Conference Proceedings, March


1998, pp 449-453 (1998).


13. K. Ramanujachar, Scanning Capacitance Microscopy at        Transistor Contact Level, ISTFA 2004, pp. 482-486


14. T. Tong, A. Erickson: Current Image Atomic Force


Microscopy (CI-AFM) Combined with Atomic Force


Probing (AFP) for Location and Characterization of


Advanced Technology Nodes, ISTFA 2004, pp. 42-46 .


15. T. Kane, M. Tenney, Electrical Characterization of sub30nm Gatelength SOI MOSFETs, Proceedings


International Symposium for Test and Failure Analysis,


ISTFA 2004, pp. 33-37


16. Stefan Doring, Investigations on the Influence of Focused


Electron Beam on Electrical Characteristics of Integrated


Devices, Proceedings International Symposium for Test


and Failure Analysis,  ISTFA 2007, pp. 210-213


17. R. Mulder et. al., Atomic Force Probe Analysis of NonVisible Defects in Sub-100nm CMOS Technologies.


ISTFA 2006, pp. 503-11.


18. T.Kane, M. Tenney, A. Erickson, Atomic Force Probe


Kelvin Measurements of Large MOSFET Devices at


Contact Level for Accurate Device Threshold


Characteristics, ISTFA 2006, pp. 497-502


DOI: 10.1361/cp2008istfa209


Analysis of Deep Trench Node Leakage Depth by applying Current Imaging  Technique at Silicon Level


S. Doering, M. Seitz, U. Zimmermann, P. Rodger, W. Werner


Qimonda Dresden GmbH & Co. OHG, Dresden, Germany   Stefan.doering.drs@qimonda.com


A common yield loss mechanism in DRAM products is an  increased cell leakage leading to the loss of the stored charge  that represents the information. A basic scheme of a Deep  Trench based memory cell is shown in Fig.1. There are several  leakage mechanisms for this type of DRAM cells, which could  lead to a failing cell: one of them is the leakage of the node.  Other leakage contributors could be the under STI leakage (not  shown in the graphic, because the leakage path lies  perpendicular to the drawn plane), the Deep SubVT (b), GIDL (c), the self gated leakage (d), SubVT leakage driven by the  array device (e), the leakage to the passing word line (f), junction leakage (g), leakage due to the vertical parasitic (h) and the gate oxide leakage (i).


Fig. 1: Schematic showing the basic structure of a deep trench  based memory cell with the  possible  leakage paths. For  visibility reasons except of the node leakage all other leakage  paths are drawn at the neighboring cells.


The node leakage mechanism is due to a leakage path from the  inner electrode of the deep trench capacitor to the outer  electrode, n-- or p-doped silicon, through the weak and/or   damaged dielectric. Except for node leakage, all other cell  leakage mechanisms can be isolated and narrowed down to  specific and very small areas of the failing cell, as seen in Fig.


1. Being able to narrow the defect site down to a few ten  nanometers  improves chances to find the defect significantly.  In case of a node leakage failure, the location of the defect can  be spread over the entire deep trench depth of up to six  microns,  making it very difficult to precisely localize the  defects. In addition, the use of surface area enlarging  techniques to increase trench capacitance makes it even more  difficult to pinpoint the  node leakage defect.


Scope of this work


To characterize the node leakage failure in a more detailed  way, we had used nano-probing technique [1-3] to first verify  the node leakage at a specific defective cell. After initial nanoprobing, the sample was polished top down below the contact  and transistor level.  The sample was then scanned with a  conductive probe tip, obtaining a current image [4-5] to verify  the node leakage at this level. If the target cell still shows  leakage, the sample can be further polished and imaged  creating a current map until the target cell does not show any  node leakage. Using this method, it is possible to pinpoint the  defect location in z-direction. For process engineers, the zlocation of the leakage provides useful information to track  down the root cause of failure and implement appropriate  corrective actions.


For verification of the node leakage mechanism, the chip was  delayered down to the contact level. This was done by top  down polishing with a final polish using a 0.25µm diamond  suspension on a hard silk polishing cloth. An oxide recess was  applied using diluted HF (1:100). The failing cell was  characterized using an AFM based nano-prober.


During nano-probing, the voltage applied to the bit line contact  was sweeped.  The gate contact was kept at a constant positive  voltage to open the access transistor of the failing cell. In  addition, one p well contact and one n well contact were held  at 0V (Fig. 2).


Fig. 2: AFM topography image of the chip at contact level  showing nano-probing setup for node leakage measurement.


For a functional cell, a high current is measured when a  negative voltage is applied at the bit line contact. The high  current is due to the forward-biased bit line to p well diode. When a positive voltage is applied to the bit line contact, a  small reverse diode leakage current is measured.  In contrast, the failing cell shows a very high leakage current with an  ohmic characteristic when both negative and positive voltages  are applied to the bit line contact (blue solid line in Fig. 3).  Except for the polarity, the measured IV curve (blue solid line) is quite similar to the IV curve obtained between the bit line  contact and n well (red dotted line in Fig. 3)


Fig. 3:  IV curves obtained during nano-probing  measurements.


This IV curves shown in Fig. 3 strongly suggest that that the  defect of the node dielectric is located below the p well, most  likely in the n well region.


In order to pinpoint the z-location of the failure, the chip was  further deprocessed into the p-well region. The approximate  position in z-direction after the first polishing step into silicon  is shown schematically in Figure 4.


Fig. 4:  Schematic showing the structure of a deep trench  based memory cell after the first polishing step into silicon.


At this point the navigation to the leaky capacitor was done  just using the motorized coarse positioners of the scanner  head. Since the accuracy of those motors is in the range of  2µm, an overview scan with a scan area of 8x8µm2 was done. To monitor the scanned trenches with respect to node leakage, the scanning tip was biased with -2 V. Figure 5 shows the  topography image near the defect site. The height range for  this image is set to 30 nm.  In the lower left corner, the  scanning tip is not yet in contact mode, so this is an artifact. Nearly no topography is obtained, except of some scratches  from the top down polishing. There is one bright feature that is  clearly visible (marked with the red circle in Fig. 5).


Fig. 5: Topography image of a “failed” capacitor site. Scratches are polishing artifacts. The bright spot was related  to a transferred signal saturation from the current image that  was taken in parallel.


This bright spot does not represent real topographical feature. It is an artifact from the over-saturated current image taken in  parallel. The current image was obtained with highest gain  setting to ensure a maximum sensitivity. At this setting, a  current compliance of approximately 90 nA is set.  A current  of more than 90 nA flowing through the tip creates an artifact (the bright spot in Fig. 5) in the topography image.


Fig. 6: Corresponding current image of Fig. 5.  Horizontal  and vertical line scans through the failing trench are also  shown..


The current image corresponding to the topography image of  Figure 5 is shown in Figure 6.  In the current image,  three  different features are visible. The background blue color  corresponds to the p-doped silicon of the p well. The bright  checker-board spots correspond to the n-type poly filled deep  trenches, which are separated by the node dielectric from the  surrounding p well.  The third feature is the dark spot that  corresponds to our failing capacitor, showing the highest  current of the whole image.


A high-magnification current image near the defect site is  shown in Figure 7. If the dielectric damage is located in the p  well region, the detected leakage current should be comparable  to the surrounding p well silicon.  The higher current in the  dark spot of the current image indicates the damaged site is  most likely below the p well and in the n well region.  Furthermore AFM results are consistent with the data obtained  from the IV measurements (Fig. 3), showing that the node  leakage is most likely to the n well.


Fig. 7:  High-magnification current image of Fig. 6.


As a preliminary result, we have confirmed the node leakage at  the defective cell at contact level by IV-characterization and at  p well level by current imaging.  Both methods indicate that  the inner electrode of the node is leaking to the n well. All cell  elements that have been polished away can be excluded as root  cause.


The next critical level is the transition of the trench right after  the collar oxide (Fig. 9). The sample was further deprocessed  by top-down polishing right below the oxide collar level of the  deep trench. To avoid using scan areas of 8x8µm2 for coarse  positioning of the probe tip, instead of the stepper motors of  the scanner head, the sample under the probe tip was moved  using a high accuracy sample stage with an absolute accuracy  better then 100 nm. The obtained current image is shown in  Figure 8.


Fig. 8:  Current image taken right under the oxide collar level  of the deep trench. The tip voltage was set to -1 V. No leaking  inner electrode visible at the target site at this level.


At this level, there is no node leakage current observed at the  defect site. In contrast, node leakage was measured previously  at both contact and p well levels.  The information obtained  from the current measurements shown in Fig. 9 indicated the  root cause for the node leakage at the failing cell was located  in the n well level.


Fig. 9:  The IV-characterization and the current image data at  the different preparation levels.


Problems/Difficulties


One side effect scanning under air condition with a biased tip  at silicon is the anodic oxidation of the sample at the scanned  area [6]. An example of this effect is shown in Figure 10. In  the worst case it is only possible to gain current information of  the sample for the first scan.


The effect can be reduced  by switching off  the light to optical  microscope,  by reducing the voltage applied to the tip, by  scanning under UHV conditions or by using an environmental  chamber and filling it with nitrogen.


Fig. 10 Topography and current image showing anodic  oxidation. The upper left area (brighter in the current image) is scanned for the second time.


AFM-based probing provided additional information regarding  the location of the node leakage. Since the deep trench is a  vertical device, the gained z-information is of value. In this  example, three analysis steps were done. First, the node  leakage was verified at contact level. In a second step, the  sample was deprocessed into the p well level and a current  image was obtained, confirming the node leakage to be located  below this level. In the third step the sample was further  deprocessed to the edge of the n well level. Again a current  image was obtained, showing no more leakage. With those  three measurements, we confined the node leakage to the small (compared to the whole deep trench) n well region.


We would like to thank Ralf Gerber from Qimonda Dresden  GmbH & Co. OHG for providing his presentation illustrating  all the possible leakage paths of the deep trench DRAM cell  under investigation.


[1] M. Gruetzner, Microelectronics Reliability Vol. 45 (2005) pp. 1509-1513


[2] R. Mulder, S. Subramanian, T. Chrastecky,


proceedings, ISTFA 2006, p 503


[3] C. Giret, D. Faure, proceedings, 11th IPFA 2004, p271


[4] T. X. Tong, A. N. Erickson, proceedings, ISTFA


2004, pp. 42-46


[5] R. Mulder, S. Subramanian, T. Chrastecky,


proceedings, ISTFA 2006, pp. 153


[6] H. Bloeß, G. Staikov, J. W. Schultze, Electrochemica  Acta Vol.47 (2001) pp. 335, AFM induced formation  of SiO2 structures in the electrochemical nanocell


DOI: 10.1361/cp2008istfa214


Backside Failure Analysis by Electroluminescence on Microwave Devices


M. Bouya a,b, D. Carisetti a,  P. Delaqueze a, J.C. Clement a


aTHALES Research and Technology, 91767 Palaiseau, France  M. Bouya a,b N. Malbert b, N. Labat b


bIMS Laboratory, University Bordeaux 1, 33405 Talence, France  P. Perdu c


c CNES Laboratory, 31401 Toulouse, France


III-V HBT (Heterojunction Bipolar Transistor) and HEMT (High Electron Mobility Transistor) are playing a key role for  power and RF low noise applications. As well as the  improvement of the MMIC performances, the localization of  the defects and the failure analysis of these devices are very  challenging. Active area thickness is only few nanometers, backside failure localization is mandatory because of thermal  drain or metal bridge covering the front side, materials  involved might be of ultimate hardness and/or high chemical  sensitivity while failure mechanisms strongly differ from Si  technology ones. To face these challenges, we have developed  a complete approach, without degrading the component, based  on backside failure analysis by electroluminescence. Its  efficiency and completeness have been demonstrated through  case studies.


Compound semiconductors devices have received much  attention for their ability to operate at high-power levels and  low noise in high frequency applications. They are crucial  components for the development of base stations in the  telecommunications networks and for civil, defense and space  radar applications.


The most used technologies for these applications are based  on the pseudomorphic GaAlAs/GaInAs HEMT and  GaInP/GaAs HBT. More recently, the high bandgap HEMT  technology based on gallium nitride materials with silicon  carbide substrate has been developed as it is a good candidate  to replace the GaAs HEMT technology for high power  applications.


The failure analysis methodology implemented for these  technologies is similar to the silicon one and basically  includes electrical diagnosis, chip access, defect localization  and physical analysis. Nevertheless, sample preparation  according to the different types of transistors and materials is  very complex and challenging.


For defect localization, we have intensively used light  emission microscopy, which is not currently applied to III-V  technologies.


The direct band gap of 1.45eV for GaAs and of 3.43eV for  GaN allows a higher rate detection of photons compared with


silicon components. The light emission is mainly due to  recombination of carriers generated by impact ionization in  GaAs HEMT [1], intraband transitions of carriers in GaN  HEMT [2, 3] and recombination of minority carriers in p-n  junctions in HBTs.


In addition, a very strong correlation has been established  between some failure modes and the light emission signature


[4]. In this paper, we will focus on two key issues, sample  preparation for localization by electroluminescence  observation, and describe two case studies of failure analysis  solved by backside light emission microscopy.


Front side analysis versus backside


Front side failure analysis is usually more difficult to  successfully carry out in the case of devices presenting a  thermal drain. The depackaging is also a key issue. Front side  removing of a plastic package is not satisfactory as nitric and  sulfuric acids can damage the GaAs material. In addition, some GaAs technologies use low K dielectrics (as BCB, Benzocyclobutene) that need very specific sample preparation  methods [5].


Even if front side depackaging can be manageable, thermal  drain of HBT or metal bridges of HEMT cover active area  hiding the region of interest under investigation (Figures 2, 3). It is why backside access is mandatory.


First case study: decrease of current gain in


GaInP/GaAs HBT after DC life test


The GaInP/GaAs HBT (Heterojunction Bipolar Transistor) under investigation presents a complex stacked structure (Fig. 1), with one 2µm x 35µm emitter finger. The test structures  are Technological Control Vehicle (TCV) encapsulated in a  DIL 24 ceramic package.


Four TCV have been submitted to 1000 hours of DC life test, in the following bias conditions: Vce = 5.7 V, Jce = 66kA/cm2, with a junction temperature estimated at 275°C.


Figure 1: Schematic cross section of a GaInP/GaAs HBT


Electrical diagnosis


After DC life-test, one part is considered as failed. It presents  a large decrease of the collector current and a collapse of all  Ice (Vce) characteristics in comparison with the reference  ones. The corresponding large decrease of the current gain is  reported in the following table:


C11 (failed  part)


C13 (good  part)


B18 (good  part)


C22


(reference  part)


Current


gain


Ib=100µA, Vce=5V


32


The EB and BC junctions are characterized with a Keithley  4200 system; the Fig. 2 shows the Ib-Vbe characteristic  measured with floating collector for the reference part and the  failed one. A large increase of the base current is observed for  Vbe lower than 1.3V.


Defect localization challenge


The surface observations performed by optical and SEM  microscopy do not allow to localize the area of defects and the  front side emission light analysis is not possible due to the  large thermal drain connecting the emitter finger to ground  backside metallization through two via holes inside the GaAs  substrate (Fig. 3 and Fig. 4).


To perform backside emission microscopy, the assembly is  molded in a low constraint epoxy resin. This allows the  ceramic removal by grinding and finally, the GaAs substrate is  thinned below 100µm.


A specific flat polishing process avoids any risk of  degradation of the device electrical functionality in spite of the  substrate weakness.


To bias the device, the base and collector are connected on the  pads by wire bondings whereas the emitter is connected by  microprobing metallization inside via holes on backside or  with the help of conductive silver glue.


Figure 2: Emitter-base diode characteristic measured with  floating collector: Ib=490µA at Vbe=1.13V for the failed part (in black line), Ib= 1.5µA for the reference part (in grey line).


Figure 3: Failed part observed by optical microscopy


Figure 4: Failed part observed by scanning electron  microscopy


Emitter contact


Collector contact


Base contact Ballast


Via holes areas


Under -Collector


Electroluminescence results and interpretations.


Electroluminescence experiments have been performed on the  reference part and on the failed one. The bias conditions were  defined according to the EB junction characteristics shown in  figure 2 and to the BC junction characteristics (not shown in  the paper).


While the reference part presents a normal and uniform  electroluminescence signature corresponding to the minority  carriers recombination in the base layer (Fig. 5), the failed part  presents a lower carrier recombination rate than the reference  part, with a very local non-radiative area under the emitter.  This specific signature observed on the failed part in Fig. 6 is  detailed below:


• (a) Weak light emission at the beginning of the finger  and progressive increase to the middle of emitter.


• (b) Local maximum of light emission which intensity  is similar to the reference part.


• (c) Area without light emission.


• (d) Other local maximum of light emission  equivalent to the reference part.


The base-collector junctions of the reference part (Fig. 7) and  of the failed one (Fig. 8) have also been observed by  electroluminescence technique. It appears that a non-radiative  area (c) is also observed on the BC junction of the failed part  and could be due to a local defect crossing the emitter down to  the collector.


Figure 5: Reference part, EB junction in forward mode  observed by backside emission microscopy at the same bias as  the failed part (Vbe=1.13V, Ibe=1.5µA)


Figure 6: Failed part, EB junction in forward mode observed  by backside emission microscopy (Vbe=1.13V, Ibe = 490µA)


Figure 7: Reference part, BC junction in forward mode  observed by backside emission microscopy (Vbc=1.1V, Ibc=130µA)


Figure 8: Failed part, BC junction in forward mode observed  by backside emission microscopy (Vbc=1.1V, Ibc=650µA)


Technological Analysis


The analysis has been continued by successive transverse FIB  cross-sections performed from the beginning of the finger  along the whole emitter.


The (a) area is characterized by the presence of a crack in the  emitter-base junction propagating from the beginning of the  emitter finger and located in the middle of the emitter (Fig. 9). This defect is assumed to explain the weak light emission of  the EB junction and also the decrease of the current gain after  the DC life test.


The (b) area does not present any defect in the epitaxial layers  as observed in a reference part (Fig. 10). The (c) area has been  burn out and presents a local crater in GaAs and GaInP layers  which explain the non emissivity of this emitter region (Fig. 11). In the area (d), the structure does not present any defect (Fig. 12).


This failure mechanism is characterized by a crack  propagation [6] during the DC life test from the beginning of  the emitter finger along the whole emitter. This defect is  assumed to induce a large variation of the current density  along the emitter and a local catastrophic thermal runaway.


c d


Figure 9: Failed part, FIB cross section at the beginning of  the emitter finger in area (a) defined in figure 6


Figure 10: Failed part, FIB cross section in area (b) defined  in figure 6


Figure 11: Failed part, FIB cross section in area (c).


Crater formation in GaAs and GaInP layers due to local  burnt out defined in figure 6


Figure 12: Failed part, FIB cross section in area (d) defined  in figure 6


Second case study:  Increase of the gate leakage  current in AlGaN/GaN HEMT after DC life test


The studied transistor is an eight fingers (W=8x75µm) AlGaN/GaN HEMT on SiC substrate encapsulated in a CuW  BMH 60 package. Its DC parameters are changed with a very  important increase of the gate leakage current after 2000 hours  of DC life test in the following conditions:


Vgs= -6.5V, Vds=25V, Ids=30mA, Tj=175°C.


The reference component present a gate leakage current  around 100 μA at Vds = 10V and Vgs = -6V. In the same  electrical bias conditions and after DC life test, the failure  component presents a gate leakage current around 2mA.


As observed in Fig. 13, a large gold bridge on BCB  connecting the source contacts prevents from performing a  front side light emission analysis. In this case, the backside  preparation is also necessary because the gold bridge chemical  removal step can degrade as well the interlevel dielectric BCB  as the source ohmic contacts resistivity.


A FIB opening through the metallization is feasible but would  spend time, due to the 5µm thickness of electrolytic gold, and  could deteriorate the device by ESD stress.


Figure 13: Optical view of the failed AlGaN/GaN  HEMT


Emission microscopy results


The backside light emission has required a specific  preparation of the device under investigation. It consists in a  backside diamond polishing to remove the CuW plate and to  thin the silicon carbide.


Electroluminescence measurements reveal light emission of  irregular intensity as local spots are observed (Fig. 14) along  the gate in the gate-drain area. This specific signature has  already been observed and may be linked to local defects  along the active area of the failed part inducing local changes  of the electrical field. To understand this failure mechanism, a  physical analysis has been performed.


Physical analysis


After thermal drain and BCB removal, local cracks of SiN  passivation located nearby the fourth (Fig. 15 (a) and 15(b)) and the fifth gate fingers (Fig. 16(a) and 16(b)) are identified  and correlated to light emission spots. On the contrary, no  crack has been observed in the SiN passivation on the  reference part.


These cracks may be induced at the foot of the T-shape gate  by defects due to local mechanical weakness or ionic  contamination. These defects are assumed to propagate during  the life test. The passivation cracks could explain the light  emission signature by local spots, this emission is mainly due  to an increase of surface traps [7].


On the other hand the gate leakage current is mainly due to  trap-assisted tunnelling mechanisms and direct tunnelling  mechanisms through the gate [8, 9]. Hence, the increase in the  gate current in this case can be attributed to surface defects


possibly acting as electron traps and contributing to the gate  leakage current [10].


Figure 16: (a) SEM observation of  5th gate finger after BCB  and Au thermal drain removal (b) zoom in the defect area with  crack in SiN.


Figure 14: Light emission from the backside through the SiC  substrate in AlGaN/GaN HEMT


Figure 15: (a) SEM observation of 4th gate finger after BCB  and Au thermal drain removal (b) zoom in the defect area  with crack in SiN


G


D


b  a


In this paper, we have reported a specific approach based on  backside failure analysis by electroluminescence to face the  challenging aspects of the failure analysis applied to the  localization of defects in compound semiconductor HBTs and  HEMTs. Two case studies have been detailed to underline the  very challenging sample preparation issues encountered for  backside analysis as well as the strong correlation between  failure mode and electroluminescence signatures.


ACKNOWLEDGMENT


The authors would like to thank Mr Jean Roux (HAMAMATSU Company)


[1] G. Meneghesso and al. “Analysis of hot carrier  transport in AlGaAs/InGaAs Pseudomorphic  HEMT’s by Means of Electroluminescence”. IEEE  Transactions on Electron Devices V.47, N°1, January  2000


[2] N. Shigekawa “Electroluminescence characterization  of AlGaN/GaN high-electron-mobility Transistors” Applied Physics Letters V. 79 N°8, 20 August 2001.


[3] Y Ohno, T Nakao, M Akita, S Kishimoto, K Maezawa  and T Mizutani “Electroluminescence in AlGaN/GaN  HEMTs” 2002 IOP Publishing Ltd.


[4] M.Bouya, D.Carisetti, N. Malbert , N. Labat , P. Perdu , J.C. Clément , M. Bonnet , G. Pataut “Study of  passivation defects by electroluminescence in  AlGaN/GaN HEMTS on SiC” Microelectronics  Reliability 47 (2007) 1630–1633, and ESREF 2007.


Vhigh


Vlow


even positive voltage on the VIN pin can trigger latch-up. The  pulse duration for latch-up triggering with the highest Vlow  setting (6.5 V) is 75 ns (see “A” in Fig. 5). At this pulse  duration the circuit latches for +4.2 V at the VIN pin. The  corresponding voltage transient at VIN is shown in Fig. 6. For  pulses shorter than 75 ns Vlow has to be again decreased to get  a sufficient amount of injected carriers for the activation of the  NPN transistor.


As will be seen in the following, negative and positive stress  voltages at the VIN pin lead to different latch-up triggering  mechanism. Therefore, the next results are split according to  the polarity of Vlow.


-4-2 0 2 4 6


low


A (TP=75ns)


Pulse duration [ns]


V      of Agilent 8114A   Voltage at pin VIN


Figure 5: Effect of pulse duration on latch-up trigger voltage.


For pulses shorter than ~135 ns even positive voltage on the VIN pin can trigger latch-up.


Latch-up behavior during negative stress voltages at VIN


Figure 7 shows an overlay of the infrared emission  microscopy image obtained during latch-up with 200 ns pulses  and a repetition rate of 1 kHz. EMMI identifies the latching  area of the chip, but not how it latches in detail and not which  structures exactly forms the activated parasitic SCR. To gain  full insight into the transient triggering mechanism of the


activated parasitic SCR and the involved carrier injecting  diffusions, optical investigations from device backside in nstimescale are done in-situ with a scanning TIM setup.


The TIM scan across the IR emitting area (dashed line in  Fig. 7) shows in Fig. 8 a strong free carrier injection (negative  phase shift) at position “A” (parasitic PNP transistor), high  heating at “B” and carrier injection at “C” (parasitic NPN  transistor). The corresponding schematic device cross section  is shown in Fig. 9. The P-guard ring and the grounded deep  N-tub are normally employed to prevent latch-up, however in  this case they complete a parasitic SCR.


A complete 2D TIM scan in the vicinity of the identified  parasitic SCR is shown in Fig. 10. It shows the free carrier  distribution during the beginning of latch-up at t = 250 ns. Carriers are injected due to forward biasing of P-source and  shallow N-tub of the PMOS transistor. This activates the  parasitic PNP transistor. TIM identifies clearly the source  diffusion of the PMOS transistor as the carrier emitter (negative phase shift, blue area) of the parasitic PNP  transistor. The layout of the investigated area is shown in  Fig. 11 with the identified parasitic PNP (Q1) and NPN (Q2) transistors. The NPN transistor then becomes active, causing  the SCR to latch.


-50 0 50


-100-50 0


50 100


RV=250Ω; TP=75ns; TLU


Time [ns]


NPN Emitter


PNP Emitter


Figure 6: Current, voltage and phase shift waveforms during  latch-up stress with 75 ns pulses. The NPN transistor is  activated earlier than the PNP transistor. The time instants of  the 2D phase cross sections are marked with triangles.


Figure 7: Mirrored IR emission image with top view overlay  of the chip during latch-up. The dashed line marks the cross  section of the parasitic SCR. The arrow marks the largest IR  emission area.


250


350


-200-100


0 100 200


TLU TP=200ns


y scan [µm]


75ns  480ns  1453ns  2030ns


Figure 8: Phase shift across the SCR during latching 200 ns  stress pulses showing strong free carrier injection at the  emitters (position “A” and “C”) and heating at the base –collector junction “B”.


P Source


Shallow N Tub


PMOS Transistor M1


P Guard Ring


Deep N Tub


VIN


R Sntub


R Pguard  Q2


Q1


Figure 9: Cross section of the active area with parasitic PNP (Q1) and NPN (Q2) transistors. VIN is biased with 50 V and  negative pulses are superimposed for latch-up tests.


Figure 10: 2D TIM phase map with layout overlay of active  area during -2.4 V 200 ns latch-up stress pulses showing four  areas (dashed ellipses) of free carrier injection (blue) at the  four source diffusions of PMOS transistor M1 at t = 250 ns. That indicates that the parasitic PNP transistor is activated, but not the parasitic NPN transistor.


Figure 12 shows the carrier and heat distribution during the  latched state at t = 400 ns. It shows the PMOS transistor M1  as carrier emitter (negative phase shift, blue area) of the PNP  transistor and the guard ring as collector, where strong heating  occurs (positive phase shift, bright area). The deep N-tub acts  as second emitter (upper blue area, see upper dashed ellipse) and completes the parasitic SCR. The corresponding phase  shift transients related to the latch-up pulse are shown in  Fig. 4, where the negative phase shift at P source shows, that


the PNP transistor is activated first (shorter base, higher gain). Figure 13 shows a movement of the active area to the corner  of the deep N-tub during latch-up due to heating. Considering  this movement the active area matches to the obtained EMMI  image shown in Fig. 14.


Figure 11: Layout of the investigated area with PMOS (M1), parasitic PNP (Q1) and NPN (Q2) transistors. The black  stripe at the bottom is added to get the same scale as in the  other 2D images (Fig. 10, 12–15 and 17).


Figure 12: 2D TIM phase map with layout overlay of active  area during -2.4 V 200 ns latch-up stress pulses showing two  active carrier emitters (dashed ellipses, blue area) at  t = 400 ns.


Latch-up behavior during positive stress voltages at VIN


The 2D TIM scan at t = 70 ns during stress pulses with 75 ns  duration (the device is not in latched state at this time) is  shown in Fig. 15. It shows two areas of excess carriers (see  dashed ellipses), which assists the latch-up process at short  pulses (holes activate the parasitic NPN transistor). The


reason is the forward biasing of the drain (P) – N-tub junction  of the PMOS transistor for N-tub voltages below the drain  potential (~15 V). The schematic cross section of PMOS  transistor with capacitive load is shown in Fig. 16. The  injected carriers activate the parasitic NPN transistor. After  discharge of the load capacity on the drain, the forward  current flow stops. The corresponding phase shift transient at  the outer drain diffusions is shown in Fig. 6 (P drain).


The 2D TIM phase map in Fig. 17 shows the carrier  distribution at t = 200 ns of 75 ns stress pulses. It shows the  activated parasitic NPN transistor Q2 as carrier emitter (negative phase shift, blue area). The corresponding phase  shift transients related to the latch-up pulse are shown in  Fig. 6. The negative phase shift at the deep N tub shows, that  now the NPN transistor is activated first. Opposite behavior  was observed for the 200 ns pulses, because the injected  carriers of the discharge current are vanished before the rising  edge of the stress pulse and therefore they can not activate the  parasitic NPN transistor (see P drain in Fig. 4).


Figure 13: 2D TIM phase map with layout overlay of active  area during -2.4 V 200 ns latch-up stress pulses showing  movement of active area (dashed ellipses, blue area) to the  corner of the deep N-tub at t = 2.5 µs.


Figure 14: IR emission image with layout overlay of active  area during latch-up. The dashed line marks the IR emission  area.


Figure 15: 2D TIM phase map with layout overlay of the  active area during 75 ns latch-up stress pulses showing two  significant areas (dashed ellipses) of free carrier injection (blue) at the outer drain diffusions of transistor M1 at  t = 70 ns.


Shallow N Tub PMOS Transistor


P Drain


CLoad


Figure 16: Schematic cross section of PMOS transistor with  capacitive load (CLoad). The drain – N-tub junction is forward  biased for VIN voltages below the voltage of the capacitive  load.


Figure 17: 2D TIM phase map with layout overlay of active  area during +4.2 V latch-up stress pulses with 75 ns duration  showing one area (dashed ellipse) of free carrier injection (blue) at the deep N-tub diffusion at t = 200 ns. That indicates  that the parasitic NPN transistor is activated, but not the  parasitic PNP transistor. The red areas indicate heating at the  shallow N-tub (collector of NPN).


Improvement of the latch-up robustness


Exemplarily, focused ion beam (FIB) surgery was employed  to eliminate the parasitic SCR by disconnecting the grounded  deep N-tub (emitter of parasitic NPN transistor) and therefore  to improve the latch-up robustness. Alternatively the use of  epi-substrates eliminated the latch-up problem, too.


The investigated power control devices latched during  negative spikes on the supply voltage between the M1  transistor, the P-guard ring and the grounded deep N-tub. These structures are normally employed to prevent latch-up, however the TIM analysis showed how the deep N-tub was  actually counter productive in this case. Removing it by FIB  or the use of epi-substrates improved the device robustness. In  comparison to EMMI analysis TIM can distinguish between  injected free carriers and heating with a higher time resolution  and can explain the dynamical effects during latch-up. TIM  also explained the higher latch-up sensitivity for shorter stress  pulses.


The authors would like to thank Mr. Randall Lee from  Keithley Instruments for his suggestions and mentoring this  paper.


[1] Bargstätd-Franke, S. et al., “Transient latch-up: Experimental analysis and device simulation” Proc  EOS/ESD Symp, 2003, pp. 70-78.


[2] Stellari, F. et al., “Electrical and Optical Characterization  of Latchup” Microelectronic Failure Analysis-Desk  Reference, ASM International, 2005, pp. 174-192.


[3] Danielak, W. et al., “Latch-up Root Cause Analysis for  New ASIC Design” Proc 33rd ISTFA, 2007, pp. 337-344.


[4] Domanski, K. et al., “External (transient) latchup  phenomenon investigated by optical mapping (TIM) technique” Proc EOS/ESD Symp, 2007, pp. 347-356.


[5] Litzenberger, M. et al., “Scanning Heterodyne  Interferometer Setup for the Time Resolved Thermal and  Free Carrier Mapping in Semiconductor Devices” IEEE  Trans. on Instrumentation and Measurements, Vol.54, 2005, pp. 2438-2445.


[6] Seliger, N. et al., “Time-resolved analysis of self-heating  in power VDMOSFETs using backside laserprobing“


Solid-State Electronics 41, 1997, pp. 1285-1292.


[7] Seliger, N. et al., “A laser beam method for evaluation of  thermal time constant in smart power devices“ Microel. Reliab., Vol. 37, 1997, pp. 1727-1730.


[8] Heer, M. et al., “Analysis of triggering behaviour of high  voltage CMOS LDMOS clamps and SCRs during ESD  induced latch-up”, Microel. Reliab. 46, 2006, pp.1591-1596.


[9] Pogany, D. et al., “Quantitative internal thermal energy  mapping of semiconductor devices under short current  stress using backside laser interferometry” IEEE  Transactions on Electron Devices, Vol. 49, 2002, pp. 2070-2079.


[10] Stadler, W. et al., “Device Simulation and Backside  Laser Interferometry - Powerful Tools for ESD  Protection Development”, Microel. Reliab. 42, 2002, pp. 1267-1274.


DOI: 10.1361/cp2008istfa242


Innovative method & use of UV technologies for dye penetrant sample preparation


Todd R. McDonald


Intel corporation Hillsboro Oregon


Today’s high volume FA labs are constantly looking for ways to  improve the data to customer cycle.  Current dye & pull sample  preparation  materials  and  methods  have  some  time  to  completion  requirements  that  cannot  be  avoided  without  compromising  data.  This  paper  demonstrates  that  significant  improvements in data cycle time and quality can be realized by  using a combination of the latest UV cure adhesives, masks, and  complimentary equipment such as LED cure lights and gantry  dispensing robots.


General observation of currently practiced methods for dye stain  sample preparation revealed that the widely used practice of


wiping and sanding dyed component surfaces prior to epoxy and  pull bolt application is very messy and time consuming. In high  volume operations this problem is magnified. It was discovered  that using high viscosity UV cure peelable masks prior to the


dye staining sufficiently kept them well protected from the dye  stain. The mask keeps the dye from penetrating and coating the  component surface, which can interfere with the subsequent


epoxy bonding/bolt attachment process step.


Additionally, during periods of high sample volumes and


demands for same day data, for as many as 300 dis-bonded


components, technicians recognized that that the preparation


and cure times and ergonomic demands required by existing


adhesives and dispense methods were inadequate to keep up


with demand.  Research experimentation and analysis revealed  that UV and visible light cure adhesives, Light curing


technologies and dispensing robots offered promising solutions  to these challenges.


Text


In  the  typical  process,  after  dye staining,  samples  are  wiped  clean of dye and surfaces are sanded (fig.1) to remove excess  dye and create a good bondable surface for the epoxy adhesive. Due to the substantial mess this processes generates and the time  involved to perform it, it became desirable to find an improved  method.   An  extensive  evaluation  of  peelable  UV  masks  demonstrated the material to be and ideal solution to eliminate  the  need  for  post  dye  stain  wiping  and  sanding  while  also  improving thru-put time by about 20 seconds per sample when  applied with a dispensing robot.  It is important to note that this  solution only  becomes a significant  time  improvement  when  using dispensing robot.


Figure 1: dyed & sanded component


Prior to dye staining, 12 samples were prepared with Dymax


9-318F peelable UV cure mask (fig. 2). Samples were then


submerged in Dykem red steel layout fluid bath and cycled


three times to 26 hg vacuum and then samples were removed


from dye and mask was peeled.  All 12 mask protected samples  revealed surfaces that were 97% cleaner compared to post dye  wiped samples.  Each of these samples were then prepared with  3m DP460 ns epoxy and then pulled.  All 12 samples pulled


successfully indicating that mask protected samples generate


adequately bondable surfaces.


Figure 2: bonding surface protected by peelable mask.


When  it  comes  to  adhesives known  in  the  current  art,  labs  typically  use  one  of  two approaches  to  deal  with  fast  data  requests.  One is to tackle the challenge with metal filled epoxy  putties like Faststeel or Metal Magic. The other approach is to  use two part heat accelerated cure epoxies that cure in about 2-3  hours.   With  metal  filled epoxies,  any  gains realized by the  quickness of cure are offset by ergonomics because technicians


cannot prepare high sample volumes with this material quickly  and  the  manually  intensive  mixing  process  quickly  fatigues  fingers and hands posing risk of repetitive motion injuries.


With two-part heat accelerated epoxy, it takes between 2 and 3  hours for the material to fully cure.  Add the extra oven drying  time for dye stain on top of the epoxy cure times and it becomes  clear that customers expecting data in only a few hours will be  disappointed in large part due to the several hours wait time for  epoxy to cure for component pulling.


Because  of  these  challenges,  UV  and  visible  light  cure  adhesives were researched and evaluated and determined to be a  good solution primarily for solid surface components, and hold  potential  for  socket  components  with  some  further  development.   These  light  cure  adhesives can  be  cured  and  ready for pulling in 20 seconds or less.  The curing light options  for these range from conventional  high powered UV lights to  New high  intensity  LED  curing  system and  even  visible  or  standard  light  sources.   For  some  applications  new  LED  technology may provide some advantages because they put off  mostly longer light waves that penetrate and cure first from the  deepest point near  the component  surface then upward to the  top surface of the adhesive which is very important for a good  robust pull ready bond.  This same process step of performed  using adhesive materials known in the current art will take 3 or  more  hours versus 30 seconds using UV adhesive and curing  technologies or visible light cure adhesives.


For our evaluation of  these new adhesives,  we used UV and  visible light cure adhesives from Dymax and Henkel Loctite. 12  samples were prepared using Dymax 621 multi-cure UV gel  adhesive and cured under a Phoseon high-powered LED unit for  15 seconds. Of the 12 samples, 6 were solid surface components (fig. 3) while the remaining 6 were socket components (fig. 4). Samples were then pulled to evaluate success of bonding.  All  12  samples  pulled successfully,  however  2  sockets exhibited  some socket fracturing indicating that some of the adhesive had  not fully cured at the interface of the shadowed areas around the  attached bolt.


Figure 3: Solid component with Dymax UV adhesive.


Figure 4: Socket component with Dymax UV adhesive.


A separate set of 16 samples (8 solid components and 8 sockets, were also prepared and evaluated using UV cure and visible


light cure adhesives from Henkel Loctite (fig. 7).   From this


group, all solid surface components pulled successfully, while  results for sockets were mixed with several failed pulls resulting  from uncured adhesive again in the shadowed areas where it is  difficult for cure lights to penetrate.


Figure 5: Socket with Henkel Loctite visible light cure adhesive


Manual dispensing of adhesives in high volumes often leads to  ergonomic fatigue and quality issues such epoxy flow thru on  sockets which results from manually controlled dispensing tips  contacting the socket surface (fig. 6). Gantry style robots (fig. 7) offer a solution to these challenges and have significantly come  down in price in the past few years, making them an affordable  option capable of  dispensing conventional  epoxies as well  as  UV adhesives and masks.


Single Bit Comparator Instrument


A functional block diagram of the single bit comparator  is shown in Fig. 5. The SBC consists of two CPLDs (Complex Programmable Logic Devices) called CPLD_1  and CPLD_2, an 8051 microcontroller, a display and  obligatory peripheral circuitry.


Figure 5:  Block diagram of the single bit comparator.


SBC


Data out


adjustable PASS/FAIL pulse


Microscope  electronics  X/Y location


CLK


switch button


pulse


CPLD_1


CPLD_2


8051


data in


qualifier


t_out


control


I/O


bus


expected data


& masking


display


The microcontroller forms together with the display, a rocker-switch and a button the user interface. The user  interface allows to define the expected data and an  associated bit-mask. Furthermore the user may define the  width of the output pulse controlling the microscope.


CPLD_2 acts as “glue logic” to connect all the other  devices. In particular it latches the expected data and the  bit mask and applies them as parallel 8 bit words to  CPLD_1. Additionally CPLD_2 drives the output pulse, which controls the input of the microscope.


CPLD_1 receives the same clock as the DRAM (driven by the tester), a qualifier (generated by the tester, active during read bursts) and a data-in line driven by the  DQ of the DRAM. When the qualifier is active CPLD_1  takes the serial data burst on the data-in line and  compares it to the expected data. The bit-mask allows to  restrict the comparison to arbitrary bits (burst positions). Whenever a match is identified the t_out signal to  CPLD_2 gets activated. CPLD_2 “stretches” this pulse  by means of an internal counter and generates the desired  output pulse of defined width to control the microscope.


For CPLD_1 a Xilinx Coolrunner II has been chosen, as this CPLD type works on rising and trailing clock  edge making it ideal to receive DDR data. Furthermore  this CPLD type allows to change easily the IO-voltage  from 1.5 V to 3.3 V. As the IO-voltage for CPLD_1 is  derived from the DRAMs supply voltage, the CPLDs  work as level translators between the DRAM / tester on  one side and the microcontroller / microscope on the  other side. Therefore the SBC can be used without  reprogramming or other complications for DDR1, DDR2  and DDR3. CPLD_2 has then been taken from the same  CPLD type for simplicity reasons and as it fitted easily  to the right performance / complexity class.


Verification of the SBC


The SBC functionality is verified by use of an IMS  bench test system that is also used as a test system for  the DRAM in the fourth part. The IMS tester acts here  simply as a very convenient waveform generator. Each  channel is also connected to a TEKTRONIX TDS 784A  oscilloscope for the timing measurements.


The waveforms and the timing definitions for the  incoming data and the qualifier that validate the data are  shown in Fig. 6. The CLK is running at a rate of 10ns or  a frequency of 100MHz. The data waveforms have a  data width of 5ns. As the inputs of CPLD_1 are not  synchronous, the edge placement has to be measured  with a simple 01010101 pattern and the use of the  masking bit. In the case of the first burst bit, all the bits  are masked except the first burst bit. The same applies  for the measurement for the last burst bit: all bits are  masked except the last one. The timings for the data


setup and data hold times for the first and the last burst  bit are measured with the oscilloscope’s cursor functions  and are included in Fig. 6. The timings do vary and this  has to be taken into account for validating the data in the  application. The tester edge accuracy is better than 250ps  so only tDH2 is possibly critical. Consequently the  qualifier placement has to be done carefully in the  application for either a PASS reference DUT or in the  PASS state of the failing DUT.


Figure 6:  Waveforms of the incoming CLK, data and  qualifier including the data setup and hold timings for  the qualifier.


The laser scanning localization of the defect on the  DRAM-device is done with a Hamamatsu laser scanning  microscope PHEMOS 1000 after a backside preparation  of the die. The DUT is scanned with a 1.3µm laser beam  which induces a local heating but no carrier generation. The reflected light can be used as input of the imaging  system and than an optical image of the die is obtained. On the other side, using the pulse generated by the SBC  as input, the DUT response to the laser beam position  can be mapped as an electrical image. A heat sensitive  defect will result in a spot in this image. The optical and  electrical images can be overlaid for an easier  identification of the fault location. One of the DRAM  data lines is used as the input to the SBC as it is shown  in Fig. 4 and the pulse from the SBC is the input to the  imaging system. The pulse signal is also monitored with  an oscilloscope in order to have a means to verify the  pass and fail behavior prior to integration with the  microscope.


DQS


DQ data


tDH2=0.4ns


tDS1=2.75ns


tDS2=4.3ns  tDH1=1.33ns


1st Case Study


Temperature dependent functional failures of four  DRAM devices are investigated. The failures are bit line  oriented and show a redundancy signature and  presumably suffer from a defect in the periphery of the  array [7]. These parts are final test fails and are analyzed  for test optimization purposes. The FAIL/PASS or  PASS/FAIL transitions lie in the temperature range from  40°C to 80°C, which is accessible with our IR laser. A  short-running test pattern covering these failures was  written. The pattern run time is 66µs in this case. The  length of the pulse that the SBC generates is set to a  smaller value like 33µs resulting in a duty cycle of 50% for a fail. Pulse lengths close to 100% may result in  distortions of the SDL image as the microscope and the  tester are not fully synchronized. If very short pulse  lengths like 10-20% are used, the signal is potentially  lost.


The pixel dwell time is set to 128µs, so that there are  two test executions per pixel. Therefore an image of  512x512 pixels can be recorded in about 34s. So the  acquisition time is much shorter than the 82min that  have been previously discussed in the introduction. The  pattern to pattern index time (see method in Fig. 2) of  300ms would not allow any of these images even of  smaller sizes at reasonable times (e.g. a 128x128 pixel  image with 300ms per pixel would result in 82min, but  the stability of the laser scanner is only guaranteed  within a time of approximately 15 to 20min).


The local illumination changes the PASS/FAIL state  of the DUT and thus the observed pulse signal. The SDL  images are overlaid with previously made backside  images of the die. These overlay images in x5 and x100  magnification are shown in Fig. 7. The area observed in  the overview image corresponds to the area where the  activation and internal reading should happen according  to the applied addresses during the pattern. The  superimposed images in x100 magnification allows a  layout overlay and a localization of single transistors. With the precise localization of the spots a preparation of  the component to this location is performed. The chip  was delayered down to the gate level by parallel lapping  of the metal layers and oxide plasma etching. A polysilicon short between two gates was found. A scanning  electron microscope (SEM) image of the short is shown  in Fig. 8. The defect location in the fuse evaluation  circuit explains very well the observed electrical fail  behavior (redundancy signature). For this analysis, another three samples have been investigated and the  new method proved to be successful on all parts, because  a defect was found in all cases.


Figure 7: Superimposed images of the backside and SDL  image in x5 and x100 magnification. The arrows mark  the position of the observed spot.


In this application case, the defect that is causing the  failure is located in the periphery of the DRAM (see also  spots in Fig. 7  – the DRAM cell array can be seen in the  regular square-like structure in the upper image). Failures caused by defects in the periphery are generally  very hard to analyze through bitmapping and knowledgebased FA as it can be seen in [7] for example.


Figure 8: SEM image of gate level shorts after lift-off of  the oxide on transistor level.


2nd Case Study


The second case study is a problem that occurred in a  final test insertion that has also been analyzed for test  optimization purposes. The fails are temperature  dependent write/read failure with a transition from fail to  pass state at ~40°C so that the SDL method is applicable.


The fail shows up at a single DQ (data line).  For a  burst length of 4, the fail occurs in a sequence of  seamless. In Fig. 9 such a sequence of reads is depicted  which are referenced to CLK. The expected data is  referenced to DQS and has twice the speed because this  is a DDR2 SDRAM. This sequence has toggling read  data with a periodicity of 16 shown as the second line  marked with 0 and 1 data in upper and lower sequences  of the graph in Fig. 9. The fails occurs for these reads  when, for instance, the data of the second read command  are complementary to the ones of the 6th read. This  observation points to a defect FIFO, as its depth is 8x2  storage cells in this case.


Figure 9: Seamless read data operation composed by  reads with a burst length of 4. The 3rd burst bit position  of the 2nd and 6th read must be complementary for fail  detection.


A micro-pattern, just including the minimum number  of required reads (6), was prepared in order to ensure the  short run time for the SDL localization, i.e. 10us at a  clock of 10ns, giving burst bits lengths of 5ns or a data  rate of 200Mb/s.


The fail/pass transition could be induced by using  only 5% of the maximum laser intensity. SBC is used  again to generate a fail/pass map of the chip. As input for  the SBC the failing DQ is used. This time, the pixel  dwell time for laser scanning could be reduced to 32µs, which allowed a total scan time of 8s for a resolution of  512x512 pixels. The overlay of the SDL-map with the  backside optical imagine of the die is presented in Fig.


10. The spot is located in the 4th FIFO cell of the failing


DQ, confirming the electrical failure analysis. The spot  marks precisely a gate contact of a SRAM circuit within  the respective FIFO cell. A cross-section of this contact, taken by standard TEM methods, is shown in Fig. 11. It  shows a resistive interface between the contact and the  upper (metal) layer. Additional EELS analysis reveals  carbon to be in the interface, which could be correlated  to some excursion in the cleaning process of the  respective lithography step.


Figure 10: Overview overlaid images of the backside  and SDL image in x20 magnification. The arrows mark  the position of the observed spot.


Figure 11: TEM image of a fail gate contact. The arrow  points to a bright interface layer at the top of the contact.


0 0


1 1


1 0


0 1


FAIL


RD


complementary data  Read Commands with bursts of 4 data bits


A new instrumentation tool was developed for use in  conjunction with a Hamamatsu laser scanning  microscope for soft defect localization in high speed  DRAM memories. The functionality of the tool was  verified and a successful application was demonstrated.  This method provides a means for localization of  temperature dependant defects like shorts and opens in  the DRAM periphery where bitmapping is not working  very well. The method could also be applied for defect  localization within the cell array, but bitmapping seems  to be faster in terms of turnaround times.


The authors want to thank Marcus Reiss from Infineon  for the TEM and the EELS analysis to clarify the root  cause of the second case study.


[1] E.I. Cole Jr. et al., “Resistive Interconnect Localization”, ISTFA Proceedings, 43-50 (2001).


[2] M.R. Bruce et al., “Soft Defect Localization (SDL)”, ISTFA Proceedings, 21-27 (2002).


[3] F. Beaudoin et al., “Laser Stimulation Applied to  Dynamic IC Diagnostics”, ISTFA Proceedings, 371-377 (2003).


[4] E. I. Cole Jr., Desk Reference of Microelectronics Failure  Analysis, 5th Edition, 415-416 (2005).


[5] Z. Qian, C. Brillert, C. Burmer, M. Grützner, “Lock-In  Assisted Soft Defect Localization (LIA-SDL) and its  Application In Scan Shift Problems“, ISTFA Proceedings, 128-135 (2005).


[6] M. Versen, D. Diaconescu, J. Touzel, “Soft defect  localization technique for design and debug on DRAM  devices”, ISTFA Proceedings, 426-430 (2006).


[7] M. Versen, D. Diaconescu, J. Touzel, “Case Study and  Fault Modelling for Wrong Redundancy Evaluation on  DRAM Devices”, ISTFA Proceedings, 252-257 (2007).


[8] M. Versen, A. Schramm, J. Schnepp, D. Diaconescu, “Test Instrumentation for a Laser Scanning Localization  Technique for Analysis of High Speed DRAM devices“, DATE08 Proceedings, pp.776-779 (2008).


DOI: 10.1361/cp2008istfa233


Novel application of the OBIRCh amplifier for timing failure localization


M. Sienkiewicza,b, S.Bruleb, P.Perdua, A.Firitib, O.Crepelb


a CNES - French Space Agency, 18, avenue Edouard Belin, 31401 Toulouse, France  b Freescale Semiconductor, 134, avenue Général Eisenhower, 31023 Toulouse, France


Soft defects localization by laser techniques on dynamically  working ICs is widely used for Failure Analysis (FA).  In this  context, many AC signal-oriented analysis methods have been  introduced to date (SDL, LADA…) or are under development (xVM…). Sophisticated tools are available to localize these  kinds of failures but not every FA laboratory has them. By  fully exploiting the capabilities of static localization tools, it is  possible to deal with timing issues. In this paper, we propose a  novel application of the OBIRCh amplifier related to the  timing issues on a real case study (mixed-mode device). This  novel and very simple application makes the analysis flow  time-attractive and enlarges the application field of mapping  techniques on the existing tools.


With the increasing IC complexity, soft defect issues become  more and more frequent. Many laser techniques have been  developed to date to address these kinds of failure: from static  to dynamic, as a function of type of circuit (analog or digitaloriented) and depending on the expected phenomena impact (thermal or photoelectric). The dynamic laser stimulation  techniques have been implemented on expensive tools that not  every FA laboratory has. Here we propose to localize the  device causing a timing failure by exploiting in a new way a  standard OBIRCh amplifier. In this paper we will present this  novel application through a case study. It will be followed by  the theoretical basics explaining the results.


Static Thermal Laser Stimulation techniques


Basics


The TLS [1] (Thermal Laser Stimulation) term regroups three  major static techniques: OBIRCh (Optical Beam Induced  Resistance Changes) [2], TIVA (Thermally Induced Voltage  Alteration [3]) and SEI (Seebeck Effect Imaging [3]). These  methods are the most commonly used localization techniques  in the FA process. They are based on the use of IR laser source  of 1.3µm wavelength to generate thermal phenomena. When  the DUT (Device Under Test) is unbiased (SEI) or biased in  the static conditions (OBIRCh & TIVA) and scanned by IR  laser beam, the thermal phenomena introduces local resistivity


changes and electromotive force generation. It allows the  localization of such failures as short circuits, interconnect  defects (metal-metal, metal - semiconductor, semiconductor -semiconductor), voids and DC current paths.


Tool description


The measurement schematic for TLS acquisition is shown in  figure 1.


Figure 1: OBIRCh acquisition system.


The constant voltage (Vsup) or current (Isup) is applied to the  DUT by means of the OBIRCh amplifier. Simultaneously, the  above amplifier detects changes in the electric signal (∆I or ∆V) occurring when the laser beam scans over the DUT. Therefore, the resulting signal is processed and visualized as a  gray scale level image on the screen. The detection system  involves the OBIRCh amplifier and consequently we will  focus on this tool in the following section.


The OBIRCh amplifier from Hamamatsu has 3 measurement  modes:


- constant voltage is applied and current variation is  measured (OBIRCh)


- constant current is applied and voltage variation is  measured (TIVA)


- no voltage is applied and voltage variation due to  Seebeck effect is measured (SEI).


No current is accepted on the amplifier input.


Moreover, it is possible to apply an external power supply to  the DUT. In this case a voltage variation is measured (OBIRCh amplifier is in detector mode).


For all modes the detection of the signal change is limited by  the pass bandwidth of the amplifier (~100Hz - 500kHz).


DUT


OBIRCh


amplifier


LASER  scan


Signal & Image  processing  System


Control System  Visualization


Vsup/Isup


∆I/∆V


Extended application


By analyzing the OBIRCh amplifier properties we realized  that, for certain conditions, this tool allows failure or sensitive  zone localization on the dynamically running devices. To  analyze mathematically this issue, we have taken into account  such parameters as laser scan speed, pixel time, frequency of  the electrical signal coming out from the DUT, failure  duration, and number of integrated frames.


The section below describes a case study where a novel  application of OBIRCh tool was used to localize a transient  failure. It will be followed by the mathematical explanation.


Case study


The analyzed device was a Freescale mixed-mode IC  processed in 0.8µm technology. The fault on this device was a  delayed output signal. FA was focused on the interface  circuitry between the digital and analog blocks which  presented a transient failure. The waveforms represented in  figure 2 show the functionality of the good and failing devices. For the good device, the input (command) and output (response) signals switched synchronously. For the failing  device the falling edge of the pulse switched with an  anomalous delay ∆τ dependent on temperature.


Figure 2: Waveforms of input IN and output OUT signals of  good and failing devices.


Due to the thermal sensitivity, we applied the TLS techniques  and tried to use the OBIRCh system to directly image the  delay variation ∆τ. To emulate the failure, the input signal was  cycled @ 1kHz in order to convert the variable ∆τ delay  parameter into a variable duty cycle parameter. Then, the  above duty cycle was analyzed by the OBIRCh amplifier. Figure 3 represents the output signal behaviour as a function of  temperature. At room temperature the falling edge of the  output signal switched with longer delay ∆τ (Fig.3a). When the  temperature raised the delay ∆τ decreased (Fig.3b).


a: Room temperature           b: High temperature


Figure 3: Waveforms of IN and OUT signals at room and high  temperature.


In reality, the OUT signal shown in figure 3 was a current  signal generated on the output of the DUT. It meant that we  could not apply it directly on the OBIRCh amplifier input (no  current accepted on this input). The chosen solution was to


convert this current into a voltage signal and to inject it on the  input of the amplifier. This function was assured by the  Current Probe Head module from HAMAMATSU (CPH), which allows the power absorption and I/V conversion. The  OBIRCh amplifier was switched in the voltage detector mode. Figure 4 represents the applied setup.


Figure 4: Experimental setup for transient failure detection  with the OBIRCh amplifier.


The abnormal delay, and so duty cycle variation, was detected  when the laser scanned above the temperature sensitive zone. The laser displacement was not synchronized with DUT  electrical signals. The scanning time was fixed at 16s per  image and the maximum image resolution at 1024x1024. Figure 5a shows the integration of 30 TLS frames with low  magnification lens. We could easily localize an abnormal  bright zone. The high magnification acquisition (Fig. 5b) highlighted two sensitive zones, identified as two nMOS  transistors used in the output driver block (Fig. 5c).


a: TLS image with low magnification (30integ)


b: TLS image with       c: Superimposed TLS image


high  magnification (20integ)   with high magnification


Figure 5: Transient failure localization by using OBIRCh  amplifier.


In the next step we compared these results with the normally  used SDL technique [4] acquisition. In this case we did not use  the OBIRCh amplifier but a dedicated DALS module


OUT


∆τ delay(T [°C])


GOOD PART


FAIL PART


IN


∆τ


I N


DUT  LASER


scan


Signal & Image  processing  System  Control System


Visualization


∆V


Probe Head


DUT Amplifier


VOUT


Function  generator


IOUT


(Dynamic Analysis by Laser Stimulation). The laser  displacement was synchronized with the device electrical input  signal and then, the measurement of the output signal was  taken at precise instants (DALS analog mode). In this  configuration only one acquisition was executed. The same  thermally sensitive zone was highlighted with low  magnification lens (Fig. 6a) and high magnification lens (Fig. 6b,c).


a: SDL image with low magnification (1integ)


b: SDL image            c: Superimposed SDL image


with high magnification        with high magnification


Figure 6: Transient failure localization by using SDL module.


Both configurations (OBIRCh amplifier and DALS module) pointed to the same failure site on the device. A chemical  deprocessing and delineation were performed and a physical  defect was observed at the silicon level (Fig. 7). The N implant  of the identified nMOS transistors was found masked over  several microns. As a consequence, these transistors did not  activate properly.


a: Reference inverters    b: Defective inverters


Figure 7: Optical inspection - comparison of Good/Fail  inverters (N implant masked over several microns).


Signal processing principle & mathematical approach


To better understand how the OBIRCh system processes an  AC signal coming from the DUT, a simple experiment can be  done (Fig. 8). A square signal, generated by a signal generator, is applied to the OBIRCh amplifier input via a resistor (in  order to avoid any potential damage to the amplifier).  For this


experiment, a 0V/1V signal at 10kHz combined with a 10kΩ  resistor was used. The Hamamatsu OBIRCh system was set in  TIVA mode with the following parameters: voltage set at 0V, laser speed at 4s/frame and image resolution at 1024x1024.


Figure 8: Experiment setup.


The signal voltage level, measured for each pixel, results in a  black and white pixel (Fig. 9): white pixel for a low level and  black pixel for a high level.


Figure 9: Pixel color versus signal voltage level.


The resulting frame is shown in figure 10 (1 frame only – real  picture obtained on the Hamamatsu system).


Three different duty cycles were used for this experiment: 10%


- 50% - 90%. The black pixel density directly depends on the  DUT signal duty cycle and is proportional to it.


Duty cycle @ 10%


1 frame 1024*1024 Detail


Duty cycle @ 50%


1 frame1024*1024 Detail


Duty cycle @ 90%


Figure 10: TLS image result (1 frame).


Now, let’s see what happens if we integrate several frames. We have to keep in mind that the DUT output signal and laser  displacement are not synchronized. This means that for the  selected pixel, the level of an electrical signal will be not  necessary the same for two consecutive acquisitions.


When we integrate the successive frames, an averaging  function is automatically executed for each pixel (Fig. 11). In  other words, we get a grey level colour proportional to the  signal duty cycle (we could also say proportional to the mean  value of the signal).


N region


P region


OBIRCH


amplifier (TIVA mode)


Signal  generator


10 kΩ


0V-1V / 10kHz


OUT  13 pixels


Laser beam displacement


a: frame 1            b: frame 2      c: average image


Figure 11: Averaging process during the integration


That way, after several integrations, we obtain a mapping of  the die showing the duty cycle variation versus the laser beam  impact. Darker areas correspond to a higher duty cycle, clearer  areas correspond to a lower duty cycle (Fig. 12). We thus can  localize, for example, thermal sensitive areas on the die  corresponding to the delays in a switching signal.


Figure 12: TLS frames integration versus duty cycle.


To describe this process mathematically let’s superimpose M  TLS images (frames). The average pixel value p can be  represented by equation 1:


∑


⋅


M


k


j


i


p


,


where i,j are pixel coordinates, k is the frame number and


ip represents the grayscale value of the pixel (i,j) in the kframe.


Assume that an AC signal, generated by the DUT output and  injected into the OBIRCh amplifier input, is periodic with  period T. Then, for one period, the number of measurements n  and so the number of visualized pixels, depends on the pixel  time* tpix (Fig.13):


t pix


n =


Figure 13: DUT output signal - electrical representation & image equivalent.


* Pixel time is a time when the moving laser beam scans above one pixel. This pixel time equals:


J


TFRAME


pix


where TFRAME -  time needed to scan


one image, I⋅J - number of pixel for one image, ½ - factor taking into account  the laser trajectory during scanning.


Note that for one pixel time, only one measurement is taken.


Let our AC signal be a square signal with period T. Remember  that this AC signal is not synchronized with the laser beam  displacement. Assume that for one signal period T and a given  pixel (i,j), the probability to take a measurement at instant s, where s∈(1…n), is the same. Hence, if M = n,


∀i∈(1…I), j∈(1…J)  & ∀l∈(1…I), m∈(1…J), (i,j)≠(l,m)


ip , =


lp ,


It means that by integrating n frames, all pixels will have  statistically the same gray scale value.


Now, let ∆τ represents a signal delay in the switching  introduced by the scanning laser beam and corresponding to  the timing failure (Fig 14). We assume that the time of failure  is long enough to be detected:


∆τ ≥ tpix                         (3)


Moreover, only duty cycle changes are permitted (there are no  frequency changes). Hence, the probability to detect a failure  P(∆τ) during one signal period T is:


ττ ∆=∆ )


Figure 14: Representation of the timing failure induced by the  scanning laser beam on DUT output signal.


Based on the previous mathematical explanation, the lowest  number of integrated frames M required to detect at least once  the failure, is described below:


))


1(


τ∆


〉


n


The parameters described above play a key role in sensitive or  failing zone localization. When they are wrongly chosen, the  failing area might not be localized. Hence, the electrical setup  should be carefully fixed. The unique parameter which is  arbitrary imposed is a frequency of the failing signal coming  from DUT. Sometimes the failure occurs for a frequency  range. In this case the favorable frequency is the highest one to  reduce TLS image acquisition time.


The type of failure also plays an important role in fixing the  analysis setup. The number of “failing” pixels depends  essentially on this data but can be influenced by external  parameters, such as pixel time and laser power. The increase  of pixel time, as well as increase of the laser power, results in a  greater thermal impact on the failing or sensitive area. By  increasing the pixel time, the time to acquire one frame  respectively increases. Sometimes the maximum laser thermal  power is not enough to introduce a sufficient thermal impact  on the device. Hence, we need to play with both parameters


DUT  OUT  4 pixels


1  2


tpix


s: 1       2      …     n


Duty cycle


Duty cycle 2


Duty cycle 3


REF  FAIL


(pixel time and laser power) to find a good compromise and  limit the time of the analysis.


The presented technique applied for timing failure localization  is low cost, and easy to apply, compared to the dynamic  techniques (SDL, DVM, PVM, etc.). Despite the above  advantages there are some limitations. This technique can be  use only for a failure where one of the signal edges is varying  under TLS (no frequency changes). The DUT output signal  frequency has to be included in the pass band defined by the  amplification system. In our case it was ~100Hz - 500kHz.  If  the frequency is outside of this range, the signal will be cut and  no failure will be localized. The time ∆τ, when the failure  occurs, has to be enough long to be detected by the OBIRCh  tool. If this time is shorter, we will be forced to apply another  localization technique, with a more sensitive tool, for example  DVM (Delay Variation Mapping [5]) by using TAC (Time to  Amplitude Converter).


Conclusion & Perspectives


In this paper we presented a new dynamic analysis application  of the OBIRCh amplifier usually used for static analysis. We  demonstrated, through a case study, how to solve a timing  issue by using the standard OBIRCh amplifier in an extended  mode. We compared these results with those obtained by  applying the SDL technique. Both methods successfully  localized the same temperature sensitive area, and finally, physical analysis highlighted an implant masking issue on the  identified transistors. Moreover, the mathematical approach  was presented. It was followed by discussion on the  optimization of the parameters and the limitations of the  technique.


We demonstrated in a case study that the SDL additional  module can be replaced by a “smart” and simple setup using a  traditional OBIRCh amplifier. However, this solution has   some limitations due to the OBIRCh amplifier characteristics  and the form of the DUT failing signal.


Now, the challenge worth pursuing is to extend this technique  on to such dynamic failures as amplitude variation under  DTLS (fixed duty cycle and frequency). This could be possible  to apply, not only for square signals, but also for sinusoidal  signals. We will work on it in the future.


The authors are very grateful to T. Zirilli (Freescale  Semiconductor, France SAS) for his support on the physical  analysis. Special thanks to A. Clark (Freescale Semiconductor, France SAS) for reviewing this paper.


[1] F. Beaudoin et al., “Principles of thermal laser stimulation  techniques”, Microelectronic Failure Analysis Desk  Reference, 2004, p417-425.


[2] K. Nikawa and S. Inoue, “New Capabilities of OBIRCh  Method for Fault Localization and Defect Detection”, ATS, 1997, p214-219.


[3] E.I. Cole Jr. et al., “TIVA and SEI Developments for  Enhanced Front and Backside Interconnection Failure  Analysis”, Microelectronic Reliability, Vol. 39, p. 991-996, 1999.


[4] Michael R. Bruce et al., “Soft Defect Localization (SDL) on ICs”, ISTFA, 2002, p21-27.


[5] K. Sanchez et al., “Delay Variation Mapping induced by  dynamic laser stimulation”, IEEE International, 2005, p305-311.


DOI: 10.1361/cp2008istfa493


Transient latch-up analysis of power control device with combined light


emission and backside transient interferometric mapping methods


M. Heer, D. Pogany


Institute for Solid State Electronics, Vienna University of Technology, 1040 Vienna, Austria


M. Street, I. Smith, F. Riedlberger


Diodes Incorporated, Zetex Technology Park, OL9 9LL Oldham, United Kingdom


D. Bonfert, H. A. Gieser


PS ATIS Analysis & Test of Integrated Systems, Fraunhofer-IZM, Hansastr. 27d, 80686 Munich, Germany


A case study of a transient induced latch-up (TLU) problem is  presented, which was identified during the development of a  60 V, 0.8 µm BiCMOS power control device. The mechanism  was characterized by controlled transient latch-up testing and  found to be fairly unusual, being triggered by a fast decreasing  not necessarily negative spike or glitch on the positive supply  pin. Emission Microscopy (EMMI) and Transient  Interferometric Mapping (TIM) successfully located the  parasitic silicon controlled rectifiers (SCR) structure. TIM is  an infra-red laser beam based technique for back side analysis. TIM analysis enables concurrent imaging of carrier injection  and heating in nanosecond timescale providing more detailed  information on the SCR action than more often used static  photon emission or dynamic TLP / PICA imaging.


Unavoidable parasitic SCRs are always present in bulk silicon  CMOS circuits. Under certain circumstances they can be  activated and lead to static or transient latch-up (TLU) [1–3]. Nowadays a lot of effort is done to prevent this. Guard rings  for collecting free carriers or low-resistance (higher doped) substrates are used, but the latch-up problem is not completely  vanished in modern CMOS devices. Latch-up can occur due  to carrier injection into an emitter of the SCR or due to  substrate currents (external triggered latch-up) [4].


The non-destructive transient interferometric mapping (TIM) technique is a powerful tool to analyze internal temperature  and free carrier distribution in electrostatic discharge (ESD) protection devices [5] and power devices on bulk [6] or SOI  substrates [7].


In this work we investigate the transient latch-up process in a  power control device, which sometimes failed during


reliability tests due to latch-up when negative spikes were  superimposed on the 50 V power supply. To investigate this  problem in detail, a non-destructive transient latch-up test  setup for negative pulses on the supply line was built and  incorporated in an Emission Microscopy (EMMI) system and  a scanning TIM setup.


Devices and methods


Investigated devices


The investigated power control integrated circuit (IC) is  fabricated in a 60 V, 0.8 µm BiCMOS process in bulk silicon. The packages of the investigated surface mounted devices are  opened and the silicon substrate of the 2100 µm × 1200 µm  chip is grinded to a die thickness of 220 µm and back side is  polished to get a sufficiently bright infrared image from the  device backside for optical investigations. The opened IC is  soldered upside down to the test board to access its backside  during operation.


Electrical methods


The schematic diagram of the measurement setup is shown in  Fig. 1. To emulate TLU events due to short negative pulses  applied to a 50 V supply voltage, we use a programmable  solid state pulser with a baseline option (Agilent 8114A), similarly as in [8]. Input voltage pin (VIN) and current sense  pin (S) are stressed, see Fig. 1. The pulser provides a 50 V  baseline (Vhigh) with a superimposed downward pulse (Vlow), which duration and magnitude can be varied. Vlow is varied  from -1.5 V to +6.5 V, providing thus negative and positive  stress voltages. The total current is measured at the ground pin (GND) using a Tektronix CT1 current probe. To avoid  destruction of the DUT during latch-up a current limiting  series resistor of 250 Ω was used in the load line. Additionally  after a few milliseconds the baseline voltage of the solid state  pulser is switched off in order to avoid damage to the DUT, if  a latch-up event has occurred.


Optical emission microscopy


The EMMI system is based on a Carl Zeiss LSM310 laser  scanning microscope and a cooled Photometrics AT200 CCD  camera. The EMMI system was combined with a currentlimited DC power supply and a pulse generator for EMMI  measurements during non-destructive latch-up events.


Optical transient interferometric mapping


The TIM setup is based on monitoring refractive index  changes due to temperature and free carrier concentration  changes caused by ESD or latch-up stress [9, 10]. The optical  phase shift Δφ is


( )


) z


z


l


h


th


π


∫


Δλϕ


where λ is the laser wavelength, l is the silicon substrate  thickness, kth is the temperature coefficient of the refractive  index, ΔT is the temperature change along the beam path, ke  and kh are the plasma optical coefficients for free electrons and  holes, Δce and Δch are the changes in the free electron and hole  concentration along the beam path. The resulting phase shift Δφ has therefore two components: a positive one – which is  proportional to the dissipated thermal energy density and a  negative one – related to free-carrier effect [5].


A scanning TIM method [5] was adapted for investigation of  internal temperature and free carrier distribution of the opened  power control IC during latch-up. In the scanning setup used, the device laterally moves and phase transients are recorded at  each position. Afterwards linear and 2D phase maps are  constructed at particular time instants.


During the reliability tests the current through the device was  not limited externally, thus during latch-up several metal  tracks on the chip were destroyed. A typical latch-up signature  of the latched chips is shown in Fig. 2. Since the original  latch-up site was not obvious, the latch-up current had to be  limited to make repetitive non-destructive latch-up tests  possible.


Electrical characterization of transient latch-up


The voltage and current transients for a non-latching stress  pulse of 200 ns duration are shown in Fig. 3 where the current


flow and therefore power dissipation stops after t = 400 ns. If  the pulse on the supply is slightly more negative, the device  latches after the rising edge of the 200 ns stress pulse. Figure 4 shows the voltage and current transients for a  latching 200 ns stress pulse, where the current settles at  150 mA due to the current limiting series resistor. The voltage  at VIN drops to 2.5 V.


In Fig. 5 the effect of pulse duration on latch-up trigger  voltage is investigated. The circuit is found to be more  sensitive for shorter pulses. For pulses shorter than ~135 ns


TIM signal


DSO


250 DUT


GND S


8114A Out


CT1


Figure 1: Schematic diagram of the transient latch-up setup  with Agilent 8114A solid state pulser and 4 channel digital  sampling oscilloscope (DSO).


Figure 2: Typical latch-up signature (mirrored). The found  parasitic SCR is marked by the dashed rectangle.


0 20 40 60


0 50 100 150


no TLU


Figure 3: Current and voltage waveform during a nonlatching 200 ns stress pulse showing no current flow after  t = 400 ns.


-100 0


TLU


Figure 4: Current, voltage and phase shift waveforms during  latch-up stress with 200 ns pulses. The PNP transistor is  earlier activated than the NPN transistor. The time instants of  the 2D phase cross sections are marked with triangles.


Labs processing over 200 samples per day will find these to be a  great  solution  as  they  provide  much  greater  accuracy  and  quality,  while  eliminating  ergonomic  factors  associated  with  manual dispensing.


Figure 6: Socket with epoxy flow thru issues.


Figure 7: Gantry style dispensing robot


UV peelable masks are a great addition to the dye stain process  and  the  time  they  save  coupled  with  the  improvement  to  adhesive bonding make them a winning proposition.


Use of UV cure and light accelerated adhesives on solid surface  pcb  components  for  pull  preparation  produces  great  results  while improving thru-put time of data dramatically compared to  conventional materials and methods.  Using a robot to dispense  this  material  further  improves  the  efficiency,  eliminates  the  manual dispensing ergonomic concerns and improves accuracy  and quality of dispensing.


Use of these materials on sockets is still somewhat questionable  and  requires  further  experimentation  to  understand  which  vendors  or  materials  may  be  best  suited  for  the  unique  challenges  that  the  difficult  to  penetrate  shadowed  areas  of  sockets present to UV and visible light curing equipment.


Any high volume lab performing dye and pull data collection  should seriously consider the benefits these new materials and  technologies offer, if they want to improve quality and thru-put  times.


DOI: 10.1361/cp2008istfa245


THE FAILURE ANALYSIS OF SPECIFIC SOURCE-TO-DRAIN  DISLOCATION AND CASE STUDY


C. H. Wang, S.W. Lai, C.Y.Wu, B.T. Chen, J.Y.Chiou, J.H. Chou


Taiwan Semiconductor Manufacture Company, Ltd., Taiwan


1,Nan-Ke N, Rd., Tainan Science Park, Tainan, Taiwan 741-44, R. O. C.


Phone: (886)6-5056688Ext.7068605   Fax: (886)6-5052007   Email: jhwangf@tsmc.com


A failure incurred in the front-end is typically a  bottleneck to production due the need for physical failure  analysis (PFA)  . Often the challenge is to perform timely  localization of the front-end defect, or finding the exact  physical defect for process improvement. Many process  parameters affect the device behaviour and cause the  front-end defect. Simply, the failures are of two types: high-resistance and leakage. A leakage mode defect is the  most difficult to inspect. Although conductive atomic force  microscopy and six probes nano-probing are popular tools  for front-end failure inspection, some specific defects still  need more effort. The electrical phenomenon and analysis  of a crystalline defect will be demonstrated in this paper. The details will be discussed below.


With the advancement in technology, more attention is  needed on process issues with the hope of fewer back-end  defect issues. Simultaneously, the failure in the front-end is  more difficult to inspect and resolve. Some of the front-end  defects are gate oxide quality, contact high resistance, poly-gate hump, contact spiking and crystalline, see Figure


1. These defects may be completely formed in the beginning  of the wafer process, but may worsen and/or enhance due to  subsequent heat stress processes.


Figure 1. Some possible defects incurred in the  front-end.


During PFA, localization of these front-end defects is  usually done by inspection tools, Photon Emission  Microscopy (PEM), Optical Beam Induced Resistance  Change (OBIRCH), and so on. However, when delayering  the sample below metal 2, a lot of electrical measurements  must be done to find where the defect may be. In the layout  design, the metals above metal 2 are for interconnect and


under Via 1 the metal is for circuit connection. When there  is a front-end defect the observed abnormal behaviour is  usually seen at Via 1 using passive voltage contrast. Of  course, the same electrical result can be obtained at contact  layer, and these candidates may be measured using  conductive atomic force microscopy or nano-probe. But  some specific defects can not be measured at contact, they  must be verified at the Via1 layer or using other methods. The difficulty in analysis is that after the removal of metal 1, the failure symptoms disappear. These are the most difficult  defects to inspect for front-end failure.


The specific front-end defect and basic theory


Any number of defect types may occur in  the front-end, but  the crystalline defect is most complicated. It can be at any  location within the device, and can only be observed by  transmission electron microscopy. Although it always exists  as a leakage failure mode, it is difficult to get a clear  physical defect picture. In order to understand the  crystalline defect, the discussion must begin from the  material science point.


Based on the defect geometry, the crystalline defect could  be classified into four types. (1) point defect; (2) line defect;


(3) area defect; and  (4) volume defect. Every different  geometry crystalline defect includes many categories as  depicted in Table 1.


Defect Type


Examples


Vacancy Defects


Interstitial Defects


Frenkel Defects


Extrinsic Defects


Straight Dislocations (edge or screw)Dislocation Loops


Stacking Faults


Twins


Grain Boundaries


Precipitates


Voids


Point or Zero-Dimensional Defects


Line or One-Dimensional Defects


Area or Two-Dimensional Defects Volume or Three-Dimensional Defects


Table 1. Examples of crystalline defect


From the electrical point of view, the line defect or  dislocation is a major front-end defect of concern. The  dislocation induces an electrical path through the junction or  point discharge phenomenon and causes serious leakage. Peculiarly it was observed that the dislocation shorted the  source and drain directly without leakage to bulk. The  failure localization and inspection methodology of these  special cases are demonstrated below.


The inspection method of specific dislocation case


Case 1:Embedded ROM failure using PEM


The first case was a ROM failure. The samples were  prepared for emission inspection where  abnormal emission  spots were found when compared with good samples (Figure 2.).


Figure 2. The emission inspection of ROM failure and  good dices


After tracing the emission spot, the sample was deprocess ed  and checked layer by layer. Abnormal passive voltage  contrast on the periphery circuit of the ROM was found at  Via 1. But the peculiar part is that after removal of metal 1, the abnormal passive voltage contrast phenomenon  disappeared (Figure 3). According to this data, metal 1  residue was highly suspected.


Figure 3. The conductive atomic force microscopy  topography of Via1 and contact on suspected failure  site


After cross section and spacing checks, no solid metal 1  residue was found. Base on  theory and experience, the  failuring circuit was localized to Via1 of the Vref node. The  failure was measured by nano-probe. A direct short between  Vref node (source node) and bit-line node (drain node) of  device was unexpectedly found. (Figure 4).


Figure 4.the nano-probing result on contact layer; it  shows the leakage from source to drain node.


The defect was seen using plane view transmission electron  microscopy. In plane view TEM, the dislocation from  source to drain through the poly gate was clearly visible. A  3D-TEM of  the plane view sample was done, and the  specific dislocation was clearly seen in the cross section  TEM pictures (Figure 5.).


Figure 5. The dislocation from source to drain node on  plane view and 3D-TEM


Back to the electrical analysis, we must know why the  abnormal voltage contract and C-AFM current mapping  disappeared on contact layer. From the circuit structure, the  key point is the metal 1 and the Vss node. When we  de-layered sample till Via1, because the metal 1 connects  the source to Vss node, and the charging induced device  partially turned on, therefore the current flow through the  partial turn-on devices and the abnormal voltage contrast  could be observed (Figure 6.). The same theory can be  applied for conductive atomic force microscopy. Because  bias of  the conductive atomic force microscopy is on  sample backside and negative backside bias attract more  holes on backside, it also makes NMOS partial turn-on and  the leakage could be measured by conductive atomic force  microscopy.


Figure 6.the model about Via1 abnormal voltage  contrast


The key point of this case is the Via 1 abnormal voltage  contrast and device measurement using nano-probing. The  failure can be localized to a small periphery suspect area, but needs an abnormal voltage contrast to locate which  device exactly failed. The next important part is the  nano-probe measurement on the failing device. This action  helps narrow down the candidates. Using these two hints, the specific dislocation was discovered.


Case 2: IO circuit leakage failure using OBIRCH  IO circuit leakage is the major failure mode for this case. From the testing data-log, it was known which pin is leaky. Localization of the failure was done using PEM and  OBIRCH. The success rate of OBIRCH was 100%. The  abnormal spots are all on the IO circuit of the leaky pins See   Figure 7.


Figure 7. The OBIRCH pictures on leaky pins and  good pins


After checking the layout and checking the abnormal  spots layer by layer, no failure phenomenon was found till  the contact layer. Based on the last experience and failure  map, a crystalline defect or poly residue was highly  suspected. As expected, the same specific dislocation was


found on plane view TEM pictures.  See Figure 8.


Figure 8. The dislocation induce IO pins leakage


OBIRCH is a powerful localization tool for leakage cases, especially for this case. Of course, when combined with  more information from others localization tools, the defect  can be localized more accurately.


Case 3: Poly-fuse Bit-line failure worse using  testing method


In this case the poly-fuse was applied to store the high or  low as memory. The basic structure includes a sense  amplifier, a poly-fuse, a pass gate and a program device.


Figure 9. The brief structure of memory


The major issue is bit-line failure. From the testing result  and structural analysis, the sense amplifier and pass gate  highly suspected, but nothing abnormal was found on these  circuits. Since the memory bias could not be done stably  without a tester, localizing the failure site using PEM and  OBIRCH is difficult. The only localization method was to  use the tester to program every bit one by one. Using a tester  it is possible to narrow down the candidate of a whole  bit-line to a single cell. After checking the suspected failure  cell layer by layer, no abnormal symptom was found till the  contact layer. Even the conductive atomic force microscope  had difficulty with this defect. Because the program device  is a big MOS transistor, there is no other solution but  measure every transistor using a six probe nano-probe. Fortunately, the leakage was found from source node to  drain node on two transistors. See Figure 10. The current  component curve and Id-Vd curve all show that there is  leaky path from source to drain.


Figure 10. The nano-probing data of failure transistor; it shows the leakage from source to drain node.


As expected, the dislocation was found from source to drain  on the failing transistor as seen in the last two cases.


Figure 11. The dislocation on program device


From electrical failure analysis a model was developed  based on this dislocation. When the bit was programmed a  20mA current was needed to burn the poly fuse open. But if  there is a dislocation on one of the program devices on this  bit-line, the path on the failing cell is always on. The defect   won’t allow the current to go high enough to burn the  correct poly fuse open. See  Figure 12. Therefore, all cells  on the same bit-line may suffer the same issue.


Figure 12. The model about dislocation and bit-line  failure


The electrical behaviour of the specific dislocation


The tough point of this dislocation is that it exists under the  contact layer, but there are no electrical symptom at contact  voltage contrast or conductive atomic force microscopy. This dislocation is like a highway from source node to drain  node, even though there is no leakage to bulk. This is  unbelievable from the TEM pictures and failure analysis  common sense, but it is true. The model developed matches  its electrical characteristic. This must be put in the defect  library and more attention must be placed on this kind of  dislocation.


“No defect is impossible if you can demonstrate it with what  you saw” I always said after finding this dislocation. Sometimes when the defect can’t be found after localization, there could be three reasons: 1.the defect is somewhere but  not on where inspected .2.the defect is there but can’t be  seen 3.the defect is there but the analyst doesn’t think it is a  true defect. For the first issue, further checking can be done, along the whole net. More time may be spent to solve this  issue. Transmission electrical microscopy can solve the  second issue if the localization of the defect is accurate. The  third issue is a major issue that will be encountered in the  future.


In the future, the defect under devices, like this dislocation  defect, will be a bigger challenge than before and need more  patient and skill of electrical and physical failure analysis.


On these cases, we got a lot of great support from TEM  supporting team. They provided us with perfect pictures and  excellent skill for 3D TEM pictures. Thanks to  all  colleagues who support our nano-probing measurement and  all others who worked with us.


[1] Frank siegelin, Anton Stuffer; “Dislocation related leakage in  advanced CMOS devices”, Proceedings of the 31th  International Symposium for testing and failure analysis, Nov. 2005 page59-63


[2] “crystalline defect in silicon”,2004, www.siliconfareast.com


[3]  C.H. Wang, C.M. Shen, C.J. Lin, Z.H. Lee, J.H.Chou, “ the  study and methodology of defects isolation for contacts of  non-isolated active regions on new logic designs,” Proceedings of the 31th International Symposium for testing  and failure analysis, Nov. 2005 page479-483


[4]  S.C. Liou, J.H. Chuang, J.C. Lee; “The physical failure  analysis of Iddq and Iddq_delta fail in 90nm logic products” Proceedings of 12 th IPFA 2005, page47-51


DOI: 10.1361/cp2008istfa249


Next Generation Laser Voltage Probing


Yin S Ng, William Lo, Kenneth Wilsher


We present an overview of Ruby, the latest generation of  backside optical laser voltage probing (LVP) tools [1, 2]. Carrying over from the previous generation of IDS2700  systems, Ruby is capable of measuring waveforms up to  15GHz at low core voltages 0.500V and below. Several new  optical capabilities are incorporated; these include a solid  immersion lens (SIL) for improved imaging resolution [3] and  a polarization difference probing (PDP) optical platform [4] for phase modulation detection. New developments involve  Jitter Mitigation, a scheme that allows measurements of jittery  signals from circuits that are internally driven by the IC’s  onboard Phase Locked Loop (PLL). Additional timing  features include a Hardware Phase-Locked Loop (HWPLL) scheme for improved locking of the LVP’s Mode-Locked  Laser (MLL) to the tester clock as well as a clockless scheme  to improve the LVP’s usefulness and user friendliness. This  paper presents these new capabilities and compares these with  those of the previous generation of LVP systems [5, 6].


Time Resolved Emission (TRE) has been widely utilized for  backside optical probing in Design Debug and Failure  Analysis. Of its several advantages over LVP, its ease of use  was the main driver in its acceptance by engineers and  designers. However, TRE is pushing its limits due to the  exponential reduction of emission at lower voltages inherent  with smaller technology process nodes. Even though TRE still  acquires waveforms on 45nm technologies hours of  integration are sometimes required.


LVP does not face the same voltage limitation as TRE. It was  shown that LVP scales almost linearly with voltage; waveforms at 500mV on 45nm devices have been obtained. LVP also offers the high bandwidth advantage of 15GHz and  beyond. However, the LVP technique needed several  improvements to be successful. Among these are overall ease  of use, improved resolution, higher signal to noise ratio, ability to probe devices with internal jitter, and the ability to  probe without requiring a clock synchronization signal.


This paper explains the improvements that were introduced on  this Ruby platform. These improvements are compared to the  previous generation of LVP tool, the IDS2700.


Laser Voltage Probing Improvement Overview


The LVP systems use short sampling pulses (~10 ps) from a  MLL to probe the voltage of a node within an integrated  circuit.  Because the reflected modulated signal detected is  weak -- on the order of 100-1000 ppm atop the returned  sampling pulse -- the signal must be repetitively sampled to  reduce the statistical noise inherent in the measurement  process.  This requires that the signal being probed be  repetitive and synchronized with a trigger event such that  multiple samplings at fixed time offsets from the trigger  always probe the same voltage state.  To capture a waveform, the MLL is adjusted such that the sampling pulses are  advanced slowly in time relative to the trigger event, thereby  reconstructing the waveform of interest.  The system thus  operates like an equivalent time-sampling oscilloscope, and is  able to capture high-speed waveforms, with timing resolution  as small as the MLL laser pulses, using optical measurement  techniques that need only be as fast as the relatively long  trigger rate.


Several new incorporations to the LVP tool consist of proven  technologies. A SIL [3] has been incorporated into the LVP  system. The use of SIL has been implemented in other optical  probing tools, specifically in the time-resolved emission (TRE) EmiScope product.  A PDP [4] optical scheme allows  the detection of phase modulations in the reflected signal. Although PDP has been used in previous generation LVP tools, we present the practical application of PDP on a SIL  incorporated optical system and on 45nm technologies and  beyond.


To expand the LVP tool’s capabilities and ease-of-use, new  timing features are also added. Jitter Mitigation is designed for  situations where the jitter between the Device-Under-Test (DUT) stimulus, which normally supplies the system trigger  and clock, and the DUT time-domain being probed is  excessive. A typical source of jitter is the onboard PLL used  for clock multiplication. Zero-Delay Triggering was  developed specifically but not exclusively for the application  of Jitter Mitigation due to the accumulation of jitter as the  signal of interest moves away from the trigger. In Clocked  Mode, synchronization via the new HWPLL scheme does  away with the tester clock and loop length restrictions that the  previous generation LVP tools had, making test pattern  generation significantly simpler. Lastly, a Clockless Mode has  been incorporated into the LVP tool where the laser sampling  pulse appears randomly within any given 10ns window. Implementation of ∆T measurements between the trigger  signal and the laser sampling pulse is essential for this purpose


as it provides actual timing data for each sampled data. This is  essential for the incorporation of the Clockless mode, where  the laser sampling pulse appears randomly within any given  10ns window.


In the following sections, we will present some examples of  SIL imaging and PDP acquisition. We will also discuss in  detail the implementation of Jitter Mitigation, clocked and  clockless modes.


Solid Immersion Lens


A hemispheric SIL has been incorporated to increase the  optical magnification from 100x with the Liquid Immersion  Lens (LIL) to 220x. The SIL also reduces the laser spot size  from 500 nm with the LIL [7] to 230 nm. In addition to the  improved optical imaging resolution that this provides, the  smaller spot size allows for more accurate placement of the  MLL laser spot, enabling probing of smaller geometries  without the effects of crosstalk. Figure 1 shows a Laser  Scanning Microscope (LSM) image on a 45nm technology IC, and Figure 2 shows waveforms taken off the transistors in  Figure 1.


Figure 1: SIL LSM image of a buffer chain on a 45nm  technology. LSM image was taken at 8x LSM zoom at 1024  pixel resolution, giving a field-of-view (FOV) of  approximately 9 x9µm.


Time/div: 20ps


Figure 2: Delay measurement of 55ps between the adjacent  buffer stages of Figure 1


Polarization Difference Probing


Polarization Difference Probing (PDP) has been previously  explained [4]. However, PDP had not been tested on a SIL  incorporated optical systems or for 45nm technologies.


Figure 3 shows the propagation of the incident beam through  the PDP optical block. The incident beam consists of two  orthogonal, linearly polarized beams. These 2 beams are  phase-shifted by the variable waveplate by θ/2, before  interacting with the DUT. Figure 4 shows the reflected beam  passing back into the PDP optical block. A phase-shift of δ is  caused by DUT interaction, before the variable waveplate  introduces an additional θ/2 phase shift. The 2 beams are then  made to interfere with each other in the two reflected arms, Reflected A and Reflected B, by polarizing beams splitters. The intensity of the power in Reflected A or B is given by the  interference equation


R ∝ (X/√2)2 + (Y/√2)2 ± 2(X/√2) (Y/√2) cos (θ + δ)


where X and Y are the amplitude of the two reflected polarized  beams. As a result, changes in δ is detected by the change in  the reflected intensity, R. By adjusting the variable waveplate, maximum sensitivity to changes in δ can be achieved in both  Reflected A and Reflected B, giving an improved SNR is the  resultant PDP waveform.


45nm transistor


Figure 3: Incident beam prorogating through PDP optical  block.


Figure 4: Reflected beam back through the PDP optical block


The explanation of PDP is not discussed here as detailed  understanding of phase shifts contributed by the many and  various interfaces of the process layers is still being modeled. Figure 5 shows an example of how PDP can improve the  signal-to-noise ratio (SNR).


Figure 5: Phase modulation is detected in both Reflected A  and B arms of the PDP block and the resulting PDP waveform  shows significantly improved signal-to-noise ratio (SNR).


Jitter Mitigation


In Normal (Trigger) Mode, an LVP system uses the Tester  Trigger as its System Trigger. That is, all waveform  acquisition timing is made relative to this Tester Trigger. In  the presence of DUT jitter, the Tester Trigger and the DUT  signal of interest will lose coherence and the acquired signal’s  transition times will be degraded through the Equivalent Time  Sampling and averaging process.


If a coherent clock signal from the DUT time-domain being  probed (referred to as the Q-Clock) is made available to the  LVP system (Figure 6), Jitter Mitigation mode can be used to  mitigate the effects of DUT jitter. In Jitter Mitigation Mode, one of the edges of this Q-Clock is used as the System Trigger, as opposed to the Tester Trigger. This edge is called the  Qualified Clock Edge (QCE). If this QCE is coherent with the


signal being probed, as indicated by the blue edges in Figure 7, then the effects of DUT Jitter is eliminated.


Figure 6: Jitter Mitigation Mode. In addition to a Tester  Trigger and Tester Clock, a DUT Core Clock (or, Q-Clock) is  now provided to the LVP system.


Figure 7: Timing diagram showing how the effects of Jitter  can be reduced in Jitter Mitigation.


Zero-Delay Triggering


In practice, the coherence time between the QCE and the DUT  Signal of Interest is limited, even if they are from the same  DUT Time Domain: Random jitter between the QCE and  DUT signal builds as the number of Q-Clock cycles between  them increases, until the jitter saturates at same maximum  value (Figure 8). This number may be as low as 10-20 QClock cycles. In this situation, Jitter Mitigation is ineffective  unless LVP measurements are made within the coherence time  of the QCE/DUT signal of interest. Since the Q-Clock signal  may have a period as short as a few hundred picoseconds, measurements must be made within a few nanoseconds of the  QCE for Jitter Mitigation to be effective. The Zero-Delay  Triggering provides this capability.


Figure 8: Diagram showing how the Q-Clock and the DUT  Signal of Interest lose coherence as the delay from the QCE  increases.


Tester  Trigger


Loop 2  Loop 1


Loop 3


Q-Clock Signal of  Interest


Q-Clock Signal of  Interest  Q-Clock


Signal of  Interest


PDP


QCE


Q-Clock


Signal of Interest


Normally, the Trigger for a given Test Loop initiates all the  data acquisition activity for that particular loop (Figure 9). Delay is measured relative to the trigger of the particular loop. Zero-Delay Triggering uses the previous Test Loop’s Trigger  event to initiate the data acquisition activity as illustrated in  Figure 10.


Figure 9: The current Test Loop’s Trigger event initiates the  activity, and the delay for the laser sampling pulse is  measured relative to this Trigger.


Figure 10: The previous Test Loop’s Trigger event #1 initiates  the activity, but the delay for the laser sampling pulse is  measured relative to the Trigger event #2.


Demonstration of Jitter Mitigation


A two function generator scheme was used to evaluate the  Jitter Mitigation Mode. Function Generator #1 represented the  tester or stimulus system that drives the DUT and also sends  the trigger signal to the Ruby LVP. Function Generator #2  represents the IC’s onboard PLL, in which it receives a  reference clock from the Function Generator #1 and outputs to  the DUT a jittery clock relative to the reference clock. The  DUT then behaved as the internal circuitry driven by the onboard PLL.


With this setup, the amount of jitter injected is under direct  control for investigation purposes. The jitter is introduced  using Function Generator #2 by phase modulating its output. This also enabled a zero-injected jitter condition that was used  as a baseline reference to the amount of jitter being mitigated.  Figure 11 and Figure 12 show the measurements of both the  zero-injected jitter condition and the injected jitter respectively.


Figure 11: Measurement of zero-injected jitter


σ = 11.285ps


Figure 12: Measurement of injected jitter


σ = 125.023ps


Figure 13 show the results of this investigation. The top  waveform is a baseline with no jitter having been introduced. The measured rise time is approximately 62 ps (20%-80%). The middle waveform shows the acquisition of the jittery  composite signal. The jitter manifested itself as a slow edge – giving a rise time of approximately 190 ps. Using Jitter  Mitigation, the bottom waveform shows the jitter being  mitigated to resemble the baseline signal, bringing the rise  time back down to 62 ps.


Time/div: 50 ps


Figure 13: (Top) Baseline waveform. (Middle) Injected jitter  signal. (Bottom) Injected jitter mitigated with Jitter  Mitigation.


Clocked Mode


The most efficient mode for an LVP tool to operate in is the  Clocked Mode. This was the only mode previous generation  LVP tools had. In Clocked Mode, the LVP tool controls the  timing of the laser sampling pulse in relation to the Tester  Trigger, phase shifting the laser sampling pulse to sweep  across the DUT’s signal of interest. In order for this to be done, synchronization is required between the MLL’s 100MHz  clock and the Tester. Therefore, it was mandatory for a Tester  Clock to be supplied to these LVP tools. For synchronization  to occur there must be an integral number of both Tester  Clocks and Laser Clocks in the Tester Loop. Implementation  of this synchronization happens in the timebase electronics, which is improved significantly with the new Hardware  Phase-Locked Loop (HWPLL).


IDS2700 (previous generation) Timebase


Figure 14 shows a block diagram of the IDS2700 timebase  electronics. The portion enclosed by the dashed lines is the  PLL circuitry which serves to lock the MLL’s 100MHz Clock  to the Tester Clock. To achieve the requirement of having an  integral number of Tester Clock and Laser Clock cycles within  a Tester Loop, the M and N divider in the PLL circuit divide  the Tester Clock and Laser  Clock, respectively, to derive a  common frequency to drive the Phase Comparator. The  VCXO used has a restricted tuning range of + 10ppm and the  M and N dividers have a restricted counting range. Together, this puts severe limitations on the usable Tester Clock  frequency and Tester loop lengths.


Figure 14: Block diagram of IDS2700 timebase. Section  enclosed within dashed box is equivalent, in basic operation, to the Hardware Phase Lock Loop (HWPLL) block shown in  Figure 15


Hardware Phase-Locked Loop (HWPLL) Timebase


Figure 15 shows a block diagram of the Ruby timebase  electronics. The essential component of this timebase


operation is the Hardware Phase Lock Loop (HWPLL). It  consists of Direct Digital Synthesizers (DDS) that is capable  of synthesizing a clock of any arbitrary frequency. This DDS  scheme is enabled by the improvement of the frequency tuning  range of the MLL (100 MHz + 25 kHz). Therefore, the DDS is  free to generate any arbitrary frequency that is within this 100  MHz + 25 kHz range to achieve the requirement of having an  integral number of Laser Clock cycles within a Tester Loop.


This removes the restriction placed on Tester Clock frequency  and Tester loop lengths, hence tremendously improving ease  of use.


Figure 15: Block diagram of Ruby timebase.


Direct Digital Synthesizer


For a given reference frequency, a Direct Digital Synthesizer (DDS) can generate a finite number of discrete frequencies  depending on the size of the frequency tuning word (FTW). In  order to generate any arbitrary frequency, the reference  frequency can be slightly changed. A dual DDS scheme is  used (Figure 16). DDS_A is part of the Phase Lock Loop (PLL) that maintains lock and synchronization with the Tester  Clock. DDS_B is used to synthesize the proper 100 MHz + 25  kHz Laser Clock signal. The reference frequency to both DDS  can vary continuously over the range of the VCXO output, giving this scheme the capability to generate an arbitrary  frequency output.


Figure 16: Simplified Block Diagram of the HWPLL dual  DDS scheme.


Clockless Mode


∆t


As discussed in the previous section, when an LVP tool is  phase-locked to the Tester Clock, the Laser Clock, and hence  the Laser sampling pulse, is under timebase control. This  timebase control allows the precise placement (nominal delay) of the laser’s pulses relative to the Tester Trigger. Therefore, laser sampling pulse timing can then be assumed based on  timebase parameters.


With the incorporation of ∆t, the LVP tool now measures the  actual laser sampling pulse nominal delay relative to the  Tester Trigger. A ∆t measurement is made at each tester loop  at the same time the laser sampling pulse samples the  electrical signal. Each measurement would be time-binned  accordingly.


Clockless Timebase


If no Tester Clock signal is available, the LVP’s timebase  switches to a fixed, internal 100MHz oscillator to supply the  Laser Clock. In this case, the laser pulses are not synchronized  to the Tester and the system operates in Clockless Mode (also  referred to as Random Sampling Mode).


Since the laser pulses are unsynchronized, a given laser pulse, n, after the Tester Trigger (and stop-delay) will wander quasirandomly over a 10ns period from one test loop to the next (Figure 17). For any particular loop, the waveform is sampled  wherever the pulse happens to fall in time for that loop. Since ∆t measurement of the sampling delay is determined for each  measurement and the acquired data binned accordingly, the  final waveform is still properly reconstructed with no loss in  timing accuracy relative to the Clocked Mode.


Figure 17: Clockless Mode timing diagram showing how  100MHz ML Laser clock wanders quasi-randomly relative to  trigger. As a result, nth laser pulse (red) after trigger event (and Stop-Delay) falls quasi-randomly over 10ns span.


By using a Variable ML Laser Pulse Counter to select a  different laser pulse (n+1, for example) different 10 ns spans  can be accessed. For finer control over the position of the 10


ns span, the variable Stop-Delay is used. Increasing/decreasing  the Stop-Delay interval by δt has a corresponding effect on the  sampling delay. The nth laser pulse still falls quasi-randomly  over a 10 ns span, but this span is shifted in time by δt (Figure  18). Varying the ML Counter value and Stop-Delay interval  thus gives precise control over the positioning of the 10 ns  span.


Figure 18: Effect of changing Stop-Delay time in Clockless  Mode. Sampling delay changes of < 10 ns are possible since  the resolution of the Stop-Delay is <100 ps.


Advantages and Disadvantages


Clockless Mode operation has the advantage of a simplified  test setup. It eliminates the need for the user to provide a  Tester Clock signal, but, perhaps more importantly; it allows  non-constant or unstable Tester Trigger periods to be used.


Trade-off is a loss of acquisition efficiency for time-spans <10  ns. This is caused by the unsynchronized laser sampling pulses  being spread quasi-randomly over a 10ns span (Figure 19). For timebase spans below 10ns, laser sampling pulses falling  outside the desired timebase span are of no interest and hence  discarded. Acquisition efficiency is approximately given by  timebase span /10 ns.


Figure 19: Loss of acquisition efficiency in Clockless Mode at  timebase span <10ns


Example of Clockless Application


Figure 20 shows the results of probing a (~500MHz nongated) ring oscillator. This might have been impossible with  the older generation LVP systems due to the jittery nature of  ring oscillators, which would not be able to provide a stable  Tester Clock required for proper operation.


Figure 20: Ring Oscillator waveforms in Clockless Mode


The ability to probe 45nm device node using SIL optics has be  shown. Further evaluation also shows that crosstalk effects of  closely-spaced nodes is eliminated by careful placement of the  probe under the highest magnificent of the LSM under SIL  imaging.


Polarization difference probing (PDP) has been proven and  tested under SIL imaging and for 45nm device nodes. The  PDP provides an additional means to improve the signal-tonoise ratio when necessary or if so desired.


Jitter Mitigation and Zero-Delay Triggering enables probing  of IC’s onboard PLL driven circuitry which would have been  previous impractical or impossible in the older generation  LVP tools.


The implementation of HWPLL in Clocked Mode removes the  loop length and clock period restrictions that the older  generation LVP tools had. These restrictions had been a major  barrier to the usability and productivity of the LVP tool. With  the new HWPLL, an arbitrary loop length and clock period  can be used, enabling simpler setup.


Lastly, incorporation of the Clockless Mode further enhances  the LVP’s ease of use. This expands the LVP’s application  into probing of ring oscillator, inconsistent loop length and of  IC’s mounted on system board, in which a tester clock may  not be available.


The authors wish to thank David Shykind and Patrick Pardy of  Intel Corporation for continued support and encouraging  feedback throughout the development of Ruby. We also  extend our sincere gratitude to John West of Texas  Instruments. Special thanks go to Félix Beaudoin and Ted  Lundquist for guidance and advice in writing this paper. Last  but not least, we recognize the work by all those at DCG  Systems who help make Ruby a success.


[1]


H. K. Heinrich, D. M. Bloom, B. R. Hemenway, K. McGroddy, and U. Keller, “Noninvasive Optical  Sheet Charge Density Probe for Silicon Integrated  Circuits”, IEEE Transactions on Electron Devices vol. 33 (11), 1987, p 1860.


[2]


M. Paniccia, T. Eiles, V.R.M. Rao, and W.M.Yee, “Novel Optical Probing Technique for FlipChip  Packaged Microprocessors”, International Test  Conference (ITC), 1998, p 740


Time/div: 500 ps


[3]


“Aplanatic Microlens and Method for Making Same” US Patent 5,282,088, granted 1/25/1994; “Bi-Convex  Solid Immersion Lens”, US Patent 6,594,086, granted 1/15/2003; “Bi-Convex Solid Immersion  Lens”, US Patent 6,778,327, granted 8/17/2004; “BiConvex Solid Immersion Lens”, US Patent 7,227,702, granted 6/5/2007.


[4]


W. K. Lo, N. Nataraj, N. Boiadjieva, P. Vedegarbha & K. Wilsher, “Polarization Difference Probing: A  New Phase Detection Scheme for Laser Voltage  Probing”, International Symposium for Testing and  Failure Analysis (ISTFA), 2004, p 9-17.


[5]  K. R. Wilsher and W. K. Lo, “Practical Optical  Waveform Probing of Flip-Chip CMOS Devices”, International Test Conference (ITC), 1999, p 932


[6]


K. Wilsher, W. Lo, T. Eiles, and G. Xiao, “Integrated  Circuit Waveform Probing Using Optical Phase Shift  Detection”, International Symposium for Testing and  Failure Analysis (ISTFA), 2000, p 479-485


[7]


T. Eiles, and P. Pardy, “Liquid Immersion Objective  for High-Resolution Optical Probing of Advanced  Microprocessors”, International Symposium for  Testing and Failure Analysis (ISTFA), 2001, p 167-70.


DOI: 10.1361/cp2008istfa256


A Study of the Photoelectric Effect Caused by a Laser Beam Used in a Beam  Bounce Technique in a C-AFM System


Hung-Sung Lin, Mong-Sheng Wu


United Microelectronics Corporation, Ltd.


No. 3, Li-Hsin Rd. II, Hsinchu Science Park, Taiwan 300, R.O.C.


Phone: 886-3-5782258 ext 33231 Fax:886-3-563-6722 Email:giant_lin@umc.com


The use of a scanning probe microscope (SPM), such as a  conductive atomic force microscope (C-AFM) has been  widely reported as a method of failure analysis in nanometer  scale science and technology [1-6]. A beam bounce technique  is usually used to enable the probe head to measure extremely  small movements of the cantilever as it is moved across the  surface of the sample. However, the laser beam used for a  beam bounce also gives rise to the photoelectric effect while  we are measuring the electrical characteristics of a device, such as a pn junction. In this paper, the photocurrent for a  device caused by photon illumination was quantitatively  evaluated. In addition, this paper also presents an example of  an application of the C-AFM as a tool for the failure analysis  of trap defects by taking advantage of the photoelectric effect.


A conductive atomic force microscope (C-AFM) is a precision  probing system based on a direct on-axis optical microscope  system. The optical path from the sample to the camera is a  straight line. In addition, in order for the C-AFM to work, a  deflection sensor that works by reflecting a laser beam off the  back of the cantilever onto a photon detector is usually used to  measure the extremely small movements of the cantilever. This technique is also known as beam bounce detection. The  light exposure sourced from a halogen bulb inside the optical  microscope and the laser beam used in the beam bounce  technique causes several possible semiconductor photon  interaction mechanisms and makes it more complicated to  analyze the electrical characteristics of a device. For example, when we are measuring a pn junction, the junction will behave  like a solar cell, photon detector or photodiode due to the  photoelectric effect. Nevertheless, the side effects caused by  the light exposure are not all bad. This paper will present an  example of an application of the C-AFM that helps determine  nanoscopic or even invisible defects by understanding the  small deviations from the norm of the IV behavior of this  pseudo optical device.


Experimental Details and Case Study I


In order to quantitatively evaluate the photoelectric effect  sourced from the exposure of a halogen bulb and a laser beam, the IV characteristics a pn junction were extracted and  analyzed from a device mechanically polished to expose  isolated tungsten plugs, as shown in Fig. 1.


Figure 1: Optical microscope view and schematic diagram of  a cross sectional pn junction during measurement.


After confirming the existence of the photoelectric effect  caused by the light exposure another device was chosen. This  device had a bright voltage contrast at the contact layer when  viewed in a focused ion beam (FIB) tool, as shown in Fig. 2. The device was probed using a C-AFM, and then the IV  characteristics of its pn junction were analyzed.


Figure 2: PVC carried out using a FIB on a sample lapped to  the contact level.


By understanding the behavior of this pseudo optical device, the defect type causing the bright passive voltage contrast (PVC) was verified. The experiment was done using a C-AFM  system called a Digital Instruments CP-II by Veeco. With the  guidance of a topographic image, a 50nm diamond coated  doped tip was used to probe the tungsten plugs with 125nm  diameter. The DC voltage was supplied from the bulk, which  formed a closed path for the circuit with the grounded probe  tip. The laser diode was powered from a low voltage supply  with a maximum output of 0.2mW in a wavelength range of  600 to 700nm. Figure 3 shows the I-V curves for a pn junction  of a device with and without light exposure. Even with zero  bias applied to the junction, a current of about 0.32nA was  measured in the reverse-bias direction with the photon  illumination sourced from a halogen bulb and a laser beam. The junction current was 0.18nA when the photon  illumination was only sourced from the laser beam. However, there was virtually no current when all the lights were turned  off. Obviously, the pn junction here acted as a solar cell and  the current was confirmed to be a photocurrent caused by the  photon illumination creating electron-hole pairs in the space  charge region that will be quickly swept out by the electric  field producing the photocurrent in the reverse-bias direction. In this case, about 56% of the photocurrent was caused by the  laser-beam and 44% by the halogen bulb.


Figure 3: The I-V characteristics of a pn junction in a device  with the light exposure sourced from a halogen bulb and a  laser beam (a), with light exposure sourced only from a laser  beam (b) and without any light exposure (c).


After confirming that the photoelectric effect was caused by  the light exposure from the halogen bulb and the laser beam, another device with bright PVC, as shown in Fig. 2, was used  to perform I-V measurements on N+/PW diffusion contacts. The purpose of this experiment was to investigate the  influence of the photoelectric effect on the I-V behavior of the  junction, both with and without bright PVC, and further  identify defect types. As shown in Fig. 4, the I-V  characteristics of the N+/PW diffusion contact with bright  PVC are different from that of the normal contact with gray  PVC. These differences in the electrical characteristics of the  1st, 3rd and the 4th quadrants will be individually discussed in  the following sections.


Figure 4: The I-V characteristics of a pn junction in a device  with bright PVC (a) and normal gray PVC (b).


In the 3rd quadrant, the N+/PW junction can be regarded as a  photodiode, operated with an applied reverse-bias voltage. The excess carriers generated within the space charge region  are swept out of the depletion region very quickly by the  electric field. As pn<ni2, to restore the pn=ni2 equilibrium, the  photon-generated current density from the space charge region  can be thought to be proportional to GL, the excess carrier  generation rate, or to be inversely proportional to τG, the  excess carrier generation lifetime. The current in the reversebias direction of the N+/PW junction with bright PVC is  stronger than that of the normal PVC, which means the former  has a higher GL or a lower τG.


In the 4th quadrant, the behavior of N+/PW junction can be  treated as a solar cell. As the diode becomes forward-biased, the magnitude of the electric field in the space charge region  decreases, but does not reach zero or change direction. The  photocurrent is always in the reverse-bias direction and the net  solar cell current is also always in the reverse-bias direction. There are two limiting cases of interest, the short circuit  current (V=0) and the open circuit voltage (I=0). The  photocurrent at V=0 is referred to as the short circuit current, and when the net current, subtracting the forward-biased  current from the photocurrent, is zero, the voltage produced is  the open circuit voltage VOC. As the diode becomes forward  biased (pn>ni2), to restore the pn=ni2 equilibrium, the  recombination current governs the source of the diode current  according to the relationship shown in equation (1).


AW


q


KT


qV


R τ


I : the recombination current


q : the charge


in : intrinsic concentration of electrons  V : applied voltage


K : Boltzmann’s constant


T : temperature


τ : lifetime


A : area


W : total space charge width


The VOC of the N+/PW junction with bright PVC is lower  than that of the normal PVC, which means the former has a  higher recombination current or a lower excess carrier  recombination lifetime. Based on the Shockley-Read-Hall  theory (SRH), the excess minority carrier lifetime is inversely  proportional to the density of the trap states, which can also be  used to account for what was observed in the 3rd quadrant.


In the 1st quadrant, the behavior of the N+/PW junction can  be considered as a forward-biased diode under low-level  injection. The minority carrier diffusion current, I, dominates  the source of the diode current according to the relationship  shown in equation (2).


( )10 −= kTqVeII                                                                (2) 


+


L D


Aqn


n q


kT


D µ= ,


p q kT


D µ=


I : reverse saturation current


nD : minority carrier electron diffusion current


D : minority carrier hole diffusion current  nL : minority-carrier electron diffusion length


L : minority-carrier hole diffusion length


N : density of acceptor impurity atoms


N : density of donor impurity atoms


nµ : electron mobility


pµ : hole mobility


It can be observed in the 1st quadrant that the current increase  speed or the slope of IV curve of the N+/PW junction with  bright PVC is lower than that of the normal PVC. Based on  the results observed in the 3rd and 4th quadrant as well as  from the Fab inline records, the explanation is that traps [7-8] allowed energy states forbidden within the bandgap to  develop, which was caused by some crystal defects inducing  shallower current increase speed owing to the degradation of  the carrier mobility.


Case Study II


This study involved a single wafer lot that suffered from a  large number of soft single column failures. Bit mapping  analysis showed the column failures only occurred at VCCmin  and VCCnom. It became normal at VCCmax. The failure bit  counts of the columns were highly sensitive to the level of  voltage supply. Based on these observations and through the


analysis of schematic circuits of critical paths of column  decoders, it was suspected that a leakage in the column  selectors associated with the failure columns was the electrical  root cause. For this analysis, a –2V DC bias was applied to the  sample stage during scanning, and the topography and current  mapping were recorded simultaneously, as shown in Fig. 5. Current mapping uses different colors to indicate the different  current levels in the contacts. The darker the contact the  higher the current. In this way, the leaky N+_diff. contacts at  Y-MUX of the failure column were successfully isolated. In  order to obtain further data, IV characterization of the failed  contacts was performed. Fig. 6 shows the IV curves for the  both failed and normal contacts used as a reference. The failed  contacts show a higher leakage current of about 0.5nA@2V, which is higher than the normal contact by about 0.4nA@2V. The IV results for leakage contacts can possibly explain the  soft single column behavior and also give some reliable  physical failure hypotheses.


Figure 5: Corresponding topography image (a) and current  mapping (b) of C-AFM on contact level.


Figure 6: The IV curves measured on contact level by C-AFM. As the failure location was pinpointed precisely, the sample  containing leaky contacts was prepared for plane-view  Transmission Electron Microscope (TEM) inspection. As  shown in Fig. 7, substrate dislocation believed to extend  through the junction of the N+/PW diode is responsible for the  increased junction leakage. This crystal defect played the role  of traps assumed to be distributed energy-wise across the  bandgap and spatially uniform, and causing higher excess


carrier generation rate that is responsible for the higher current  in the reverse-bias direction of the N+/PW junction. As a  result, substrate dislocation can explain the IV behavior of the  leaky contacts.


Figure 7: P-V TEM image on the Y-MUX N diffusion area  isolated by C-AFM.


The photoelectric effect caused by the light illumination  sourced from a halogen bulb and a laser beam during I-V  measurements using a C-AFM has been presented, and the  influence of traps acting as a generation or recombination  center on the I-V characteristics of a N+/PW junction with  bright PVC was studied. This paper also demonstrates the  application of a C-AFM as a tool for the analysis of allowed  energy states forbidden within the bandgap, which helped  reveal the existence of trap states. After identifying the  process step that failed and determining the defect types, corrective action can be taken to quickly improve yield. A  method based on the photoelectric effect has been developed  to determine nanoscopic or even invisible defects.


[1] Hung-Sung Lin, Ying-Chin Hou, Juimei Fu, Mong-Sheng  Wu, Vincent Huang, Ching-Heng Chou, “ A Case Study  of Defects due to Process-Design Interaction in Nano  Scale Technology”, 33th ISTFA Proceedings, Nov. 2007, pp. 172-175.


[2] Hung-Sung Lin, Chun-Ming Chen, Kuo-Hsiung Chen, Afung Wang, “A Case Study of Defects due to Process  Marginalities in Deep Sub-Micron Technology”, 18th  ESREF Proceedings, Oct. 2007, pp. 1604-1608.


[3] Hung-Sung Lin, Wen-Tung Chang, Chun-Lin Chen, Tsui-Hua Huang, Vivian Chiang, Chun-Ming Chen, “A  study of Asymmetrical Behaviour in Advanced Nano  SRAM Devices”, 13th IPFA Proceedings, Jul. 2006, pp. 63-66.


[4] Hung-Sung Lin, Wen-Tung Chang, Chia-Hsing Chao, Jesse Wang, Chang-Tan Lin, and Coswin Lin, “Failure


Analysis of Soft Single Column Failure in Advanced  Nano SRAM Device with Internal Probing Techniques”, 31th ISTFA Proceedings, Nov. 2005, pp. 46-48.


[5] Marc Porti, Montserrat Nafria, Xavier Aymerich, “Nanometer-Scale Analysis of Current Limited Stresses  Impact on SiO2 Gate Oxide Reliability Using C-AFM,” IEEE Trans. Nanotechnology, vol. 3, no. 1, pp. 55-60, Mar. 2004.


[6] T. X. Tong, A. N. Erickson, “Current Image Atomic  Force Microscopy (CI-AFM) combined with Atomic  Force Probing (AFP) for location and characterization of  advanced technology node”, 30th ISTFA Proceedings, Nov. 2004, pp. 42-46.


[7] You Lin Wu, Shi Tin Lin, “Two-Trap-Assisted Tunneling  Model for Post-Breakdown I-V Characteristics in  Ultrathin Silicon Dioxide,” IEEE Trans. Device and  Materials Reliability, vol. 6, no. 1, pp. 75-80, Mar. 2006.


[8] Shu K. Pang, Arlynn W. Smith, Ajett Rohatgi, Fellow, IEEE, “Effect of Trap Location and Trap-Assisted Auger  Recombination on Silicon Cell Performance,” IEEE  Trans. Electron Devices, vol. 42, no. 4, pp. 662-668, Apr.


DOI: 10.1361/cp2008istfa260


Applications of C-AFM and CBED Techniques to the Characterization   of Substrate Dislocations Causing SRAM Soft Single-Column Failure   Contained in a Wafer with (001) Plane/[100] Notch


Hung-Sung Lin, Tung-Hung Chen, Wen-Cheng Shu


SRAM memory is an ideal vehicle for defect monitoring and  yield improvement during process development because of its  highly structured architecture. However, the success rate of  defect detection, especially for soft single-column failures, is  decreasing when traditional physical failure analysis (PFA) with only the bitmap is available for guidance. This is due to a  variety of invisible or undetectable defects that cause leakage  in the device. In order to understand the leakage behavior in  advanced high voltage (HV) processes, a Conductive Atomic  Force Microscope (C-AFM) [1-4] is introduced to perform  junction-level fault isolation prior to attempting PFA. According to J. P. Morniroli [5], crystalline defects affect  convergent-beam electron diffraction (CBED) and large angle  convergent-beam electron diffraction (LACBED) patterns, so  CBED and LACBED techniques were also applied to the  specimens containing dislocations to allow further  characterization of these defects. In this study quantified data  extracted using the C-AFM is also used to establish a  connection between the failure mechanism discovered and the  soft single column failure mode.


A typical SRAM architecture is shown in Fig. 1. It contains  memory cells, row decoders (X-decoder), column decoders (Y-decoder), column selectors (Y-MUX), sense amplifiers, input/output circuits (I/O), buffer circuits, conditioning  circuits, equalizing circuits, data latch circuits, and so on. Usually decoding functions in an SRAM are performed by  using row and column decoders. The column decoder permits  the selection of 1 out of n bits from the accessed row. The  selected gates of a column selector controlled by the  AND/NAND column decoder permit the transfer of data from  the bit-lines to the column data lines. Sense amplifiers are  used to detect small variations on the bit-lines and amplify  them to access at the end full-swing signal. During the read  cycle, the word-line (WL) is asserted, and one word is  selected. At this time, part of the constant current I0 generated  by the current source flows into the cell named ICELL, as  shown in Fig. 2.


Figure 1: Simplified SRAM architecture.


Figure 2: Simplified SRAM read operation and its equivalent  circuit.


A small current change on the bit-line bar (BLB) is desirable  in order to achieve a high-speed readout. The Sense Amplifier (SA) amplifies this small current change on the BLB. It should  be noted that the SA should provide a wide operating margin  over all process, temperature and voltage ranges.  In this case, the failing bit counts were observed to be in a column  direction and were highly sensitive to the voltage supply level.


Based on these observations coupled with the principle of  SRAM operation, checking the critical path of the read/write  circuitry, especially in the Y-MUX area, is required in order to  quickly isolate the failing location. Checking the critical path  can  determine the defect type, which can be used to  reasonably account for the soft single-column failure and  quickly identify the correct course of action required to  achieve rapid yield enhancement.


Case Study: SRAM Soft Single-Column Failure


Preliminary Bitmapping Analysis:


Bitmapping analysis enables us to understand failure modes  and counts in terms of bit distribution and sensitivity to  voltage or testing pattern. A typical failure bitmapping in our  case study of a soft single-column failure is shown in Fig. 3. To confirm the failure mode, the SRAM was tested  thoroughly at several voltages. The test data showed column  failure only at VCCMIN=1.08V and VCCNOM=1.32V. However, it became normal at VCCMAX=1.50V. This provides  valuable insight into the defect properties.


Figure 3: Illustration of bit-mapping analysis for two bias  conditions, 1.32V (a) and 1.50V (b).


Static Thermal Laser Stimulation Analysis:


Figure 4: Illustration of reverse-side IR-OBIRCH technique  with a 100X objective.


A 1340nm wavelength InfraRed-Optical Beam Induced  Resistance Change (IR-OBIRCH) system was chosen in order  to detect the signals of current change derived from localized  resistive changes from the reverse side of the chip. The results  are shown in Fig. 4. OBIRCH spots were observed in the  corresponding Y-MUX area associated with the failure  column identified through the bitmapping of an SRAM  instance. The sample was physically de-processed, but no


physical defects were observed in the back-end metal layers. To further understand the electrical behaviour and accurately  pinpoint the defect location, C-AFM was introduced to  perform a transistor level internal probing analysis.


C-AFM Analysis:


Bitmapping analysis showed column failures only occurred at  VCCMIN=1.08V and VCCNOM=1.32V. It became normal at  VCCMAX=1.50V. The failing bit counts of the columns were  highly sensitive to voltage supply level. OBIRCH spots were  also observed in the corresponding Y-MUX area associated  with the failing column identified through the bitmapping. Based on these observations and a through analysis of the  schematic circuits of the critical paths of the column decoders, it was suspected that a leakage at the column selectors  associated with the failing columns was the electrical root  cause as the leakage at Y-MUX will result in the bitmapping  analysis signature with an alternation in the voltage levels  mentioned above. For C-AFM analysis, a –2V DC bias was  applied to the sample stage during scanning, and the  topography and current mapping were recorded  simultaneously, as shown in Fig. 5.


Figure 6: IV curves measured on contact level by C-AFM.


Current mapping uses different colors to indicate the different  current levels in the contacts. The darker the color the higher  the current level. In this way, the leaky N+_diff. contacts at  the Y-MUX of the failing column were successfully isolated. In order to obtain further data, IV characterization of the  failed contacts was performed. Fig. 6 shows the IV curves for  both the failed and normal contacts. The failed contacts show


a higher leakage current of about 0.5nA@2V, while the   normal contact shows a current of 0.1nA@2V. The IV results  for the leaky contacts can possibly explain the soft singlecolumn behavior and also give some reliable physical failure  hypotheses.


Plane-View and Cross-Sectional TEM Analysis:


As the failure location was pinpointed precisely, the sample  containing the leaky contacts was prepared for plane-view (PV) and cross-sectional (X-S) Transmission Electron  Microscope (TEM) inspection. As shown in Figs. 7 and 8, substrate dislocations believed to extend through the junction  of the N+/PW diode are responsible for the increased junction  leakage.


Figure 8: X-S TEM image on the Y-MUX N diffusion area  isolated by C-AFM.


This crystal defect played the role of traps assumed to be  distributed energy-wise across the bandgap and spatially


uniform, causing a higher excess carrier generation rate that is  responsible for the higher current in reverse-bias direction of  the N+/PW junction. As a result, substrate dislocations can  explain the IV behavior of the leaky contacts.


Observation of Splitting HOLZ Lines Using CBED and  LACBED:


Figure 9: P-V TEM real spatial image (a), CBED patterns  taken at position i  as a reference (b), CBED patterns taken at  position j (c), CBED patterns taken at position k (d), and  LACBED patterns combining real spatial image display with  twisting Bragg contours (e).


The crossed substrate dislocations within the active area were  also characterized using CBED and LACBED patterns with  sharp Bragg contours as shown in Fig. 9. As shown in Fig. 9(b), the Bragg contours with a high-index CBED pattern, raised from the active region with no defects, were used as a  reference to that raised from the substrate with defects, as  shown in Figs. 9(c) and 9(d). With the same incident axis, the  parallel splitting of the Bragg contours, as shown in Figs. 9(c) and 9(d), reflected by the local dislocation strain field, indicate different strain configuration corresponded to the  positions j and k. In addition to the reciprocal diffraction  patterns, the LACBED patterns, as shown in Fig. 9(e),


obtained through the manipulation of the focus from Fig. 9(d), display typical splittings and twistings, as shown in the  enclosed region, of the Bragg contours at the intersections  with the dislocation lines, as indicated by dashed lines, in  order to determine Burgers vector. The Burgers vectors of the  respective dislocations can be further deduced from the  number of nodes of the indexed contours based on ChernsPreston rules [6]. The bending contours denoted by the arrow  also indicate the strain field even extended to the substrate of  the STI region.


The Influence on SRAM Operation:


Based on the results from the leaky N+_diff contacts caused  by substrate dislocation, a leakage current, IL, exists in the  column selector, as shown in Fig. 10. This current drop also  changes the reference current of the bit line (BL) from I0 to I0- IL.


Figure 10: Simplified SRAM architecture.


Figure 11: Simplified current sense amplifier operation and  its equivalent circuit.


As shown in Fig. 11, normally, the current sense amplifier  amplifies the net current, subtracting the current, I0- ICELL, at  the BLB from the reference current I0 at the BL, in order to  determine the full swing for m ICELL and VOUT=mICELLRL.


However, the leakage current IL will erode the swing  VOUT=mICELLRL and reduce the swing to VOUT=m(ICELL- IL)RL. The worst case will result in no swing when IL=ICELL, which  will in turn result in a solid column failure. As the bit-lines are  acutely sensitive to noise, and if the noise margin is severe, dash-like instead of solid columns will occur as in our case. This can also account for why the failed BL became normal at  VCCMAX=1.50V. The explanation is as follows: The ON  resistance of the MOS consists of a series combination of  drain resistance (RD), source resistance (RS) and channel  resistance (RCH). Typically, by design, the contribution from  RD and RS is small enough such that the primary consideration  is the RCH. An expression for the channel resistance can be  derived as follows. In the ON state of the switch, the voltage  across the switch should be small and VGS should be large. Therefore,  the MOS device is assumed to be in the  nonsaturation region according to the Linear Bulk Charge  Model shown in equation (1). The channel resistance is given  as equation (2) where VDS is less than VGS-Vtn, but greater  than zero.


DS


tn


GS


OX


mV


L W








 −−


2 1


µ


d OX


W t


1+


≈


CH


ON RR ≈


ON


∂


I : drain current


C : gate oxide capacitance


W : channe width


L : channel length


GSV : gate to source voltage  tnV : threshold voltage


m : body-effect coefficient


V : drain to source voltage


t : oxide thickness


dW : depletion width


It can be seen that a lower value of RON is achieved for larger  values of VGS with a fixed channel width and length when VDS  remains at a small value. Therefore, at VCCMAX=1.5V, ICELL  increased because of the decrease in RON. In this study, however, the increase in IL was very limited according to the  IV results obtained using the C-AFM, as shown in Fig. 6. As a  higher swing for VOUT=m(ICELL- IL)RL could be obtained  because of the increase in the ICELL, accompanied with a very  limited change in IL, it became normal at VCCMAX=1.5V.


In this paper, the use of the C-AFM technique was  successfully demonstrated in the study of the characterization  of junction leakage caused by substrate dislocations. The  characterization of CBED and LACBED patterns of the  crossed substrate dislocations within the active area indicates  a different strain configuration and shows the strain field even  extends to the substrate of the STI region. The FA results  were used to explain the SRAM soft single-column failure. After identifying the process step that failed, and determining  the defect type, corrective action was taken to quickly  improve yield. This study demonstrated an efficient  methodology for overcoming the difficulties in detecting  nanoscopic, or even invisible defects, especially for complex  SRAM failure modes.


[1] Hung-Sung Lin, Wen-Tung Chang, Chia-Hsing Chao, Jesse Wang, Chang-Tan Lin, and Coswin Lin, “Failure  Analysis of Soft Single Column Failure in Advanced  Nano SRAM Device with Internal Probing Techniques”, 31th ISTFA Proceedings, Nov. 2005, pp. 46-48.


[2] Hung-Sung Lin, Ying-Chin Hou, Juimei Fu, Mong-Sheng  Wu, Vincent Huang, Ching-Heng Chou, “ A Case Study  of Defects due to Process-Design Interaction in Nano  Scale Technology”, 33th ISTFA Proceedings, Nov. 2007, pp. 172-175.


[3] Hung-Sung Lin, Chun-Ming Chen, Kuo-Hsiung Chen, Afung Wang, “A Case Study of Defects due to Process  Marginalities in Deep Sub-Micron Technology”, 18th  ESREF Proceedings, Oct. 2007, pp. 1604-1608.


[4] Hung-Sung Lin, Wen-Tung Chang, Chun-Lin Chen, Tsui-Hua Huang, Vivian Chiang, Chun-Ming Chen, “A  study of Asymmetrical Behaviour in Advanced Nano  SRAM Devices”, 13th IPFA Proceedings, Jul. 2006, pp. 63-66.


[5] J. P. Morniroli, J. W. Steeds, “Applications of CBED And  LACBED to The Characterization of Dislocations And  Stacking Faults”, Inst. Phys. Conference, Sep. 1991, pp. 417-420.


[6] Cherns D., Preston A.R., J. Electron Microscopy  Techniques, 1989, vol.13, pp. 111.


DOI: 10.1361/cp2008istfa265


Electroluminescence Analysis by Precise Tilt Polish Technique of   Edge-Emitting Laser Diode


Hiroyuki Ichikawa*, Kouichi Sasaki, and Kotaro Hamada


Analysis Technology Research Center, Sumitomo Electric Industries, Ltd., Japan *E-mail address: ichikawa-hiroyuki@sei.co.jp


Akira Yamaguchi


Semiconductor Technology R&D Laboratories, Sumitomo Electric Industries, Ltd., Japan


We have employed electroluminescence (EL) analysis of an  edge-emitting laser diode (LD) to detect possible defects. To  extract EL emission from a LD, we developed a tilt polish  technique of the bottom electrode. We can successfully  observed clear EL emission. A high yield of 99.2 % was  achieved by the introduction of the precise tilt polish  technique.


An edge-emitting laser diode (LD) is the key component for  optoelectronics systems. Since high reliability is required for  this type of LD, degradation during operation is not acceptable. Degradation analysis technology has been indispensable for  the improvement of the LD reliability. Electroluminescence (EL) analysis (one of the analysis methods), is commonly used  in the early stage of degradation analysis [1-3].  EL analysis  is suitable to specify the degrading region. EL luminescence is  generated from an active layer by the electron (current) injection. When an active layer is degraded, emission  efficiency decreases significantly. The degraded region can be  identified by mapping the EL intensity.


LD structure


The schematic structure of a conventional edge-emitting  GaInAsP/InP LD is shown in Figure 1. The substrate was  fabricated using InP and the active layer was fabricated using  GaInAsP. Width, length, and thickness of typical LD chip  were 250 µm, 300 µm, and 100 µm, respectively. To  concentrate the current injection into the active layer, a   buried heterostructure was adopted. Top, bottom, and both  sides of the active layer are covered by the electrode. Because  the electrode metal is not transparent for emission from an  active layer, emission cannot be extracted from the LD. Therefore, though EL analysis is powerful method, this  method has been limited to the application of LDs especially  designed for EL analysis.


To extract EL emission, use of window structures has been  reported [2,3]. The LD drawn in Figure 2(a) has the window


region partly formed within the top electrode. EL emission is  extracted through the top electrode window. The LD that is  shown in Figure 2(b) has the window region formed on the  bottom electrode. In this case, the laser diode has to be


Figure 1: Schematic structure of 1.3 µm GaInAsP/InP buried  heterostructure edge-emitting LD. (a) an outline of the LD  chip. (b) an enlarged cross sectional image around an active  layer indicating in dashed line in (a).


n-InP cladding layer


Contact layer


p-InP


cladding layer


n-InP current blocking layer


p-InP current blocking layer


i-GaInAsP active layer


Passivation layer


Top electrode


n-InP substrate


Bottom electrode


mounted on the carrier upside down to extract the EL. The  LDs described here were especially designed for EL analysis.  EL emission can be seen and the structure is suitable for  fundamental research. However, windowed LDs are not  suitable for field use (practical LDs), because light output  efficiency is decreased due to insufficient current injection. Therefore, we tried to develop an EL analysis technology that  is applicable to practical LDs.


Figure 2: LD structures that are designed for EL analysis. (a) EL is extracted through the top electrode window. (b) EL is  extracted through the bottom electrode window.


EL analysis method


Extraction of an EL emission from the top of an LD was  difficult. Therefore, an attempt was made to extract the EL  from the backside of an LD as shown in Figure 3. Exfoliation  of the bottom electrode is necessary for this purpose. A portion  of the bottom electrode has to be left intact for wiring to the  injection current. The remaining bottom electrode width  required post polishing to approximately 1/3 to 1/2 of LD  chip-width. The remaining electrode width ranged from 80 µm  to 125 µm for typical LD chip-width of 250 µm. Precise


control is necessary. To obtain the control required to partly  polish, we developed the tilt polish technique. Schematic  procedure of EL analysis is shown in Figure 4. (a) The  degraded-LD was prepared. (b) The LD chip was separated  from the carrier by melting the solder which connects the LD  chip and the carrier. (c) The LD chip was mounted on top of  the arm, upside down. (d) The LD chip was connected to the  top of the arm using solid wax. (e) The circular table was set  in motion. The bottom side of the LD chip was polished by the  arms-own-weight. (f) The wax was then melted; the LD chip  was separated from the arm. (g) The LD chip was mounted on  the carrier with polished surface facing up. (h) Wiring. (i) The  current was injected to the LD from the current source. And, EL emission was observed by the infrared microscope.


Figure 3: EL emission is extracted through the bottom  electrode window that is formed by partly polish of the bottom  electrode.


Tilt polish process shown in Figure 4(e) is the most important  process of the EL analysis. The procedure of the tilt polish is  similar to playing an analog record. The lapping sheet was  placed on the circular table and then the circular table was set  in motion. The LD chip on the top of the arm was polished by   the  arms-own-weight. The tilt angle was controlled within  the range of 10-15 degrees. Time to polish was approximately  30 seconds. Scanning electron micrograph (SEM) views of a  LD before and after the polish are shown in Figure 5. We have  carried out tilt polish for many LDs (1508), with only 12  failures. Though precise control was required, we achieved  high yield of 99.2 % by using this tilt polish technique.


Window region


Bottom electrode Top electrode


Active layer


1/3 – 1/2 of LD-width


Upside down


Figure 4: Schematic procedure of EL analysis. (a) the  degraded LD on the carrier. (b) separation from the carrier.


(c) mount on top of the arm. (d) fix by the wax. (e) tilt polish  by the circular table. (f) separation from the arm. (g) mount  with polished surface facing up. (h) wiring. (i) EL observation  by the infrared microscope.


Figure 5: SEM view of the LD chip. (a) the LD chip before  polish. The LD chip is mounted on the carrier. (b) the LD chip  after polish. The LD chip is mounted on the carrier with  polished surface facing up.


EL analysis of degraded LD


Next, we investigated the validity of this EL analysis method  by analyzing a practical degraded-LD. We prepared two 1.31 µm GaInAsP/InP Fabry-Perot LD. The LD structure was the  same as described in Figure 1. One of them was damaged by  an electrostatic discharge (ESD) test of 1.0 kV. The other LD  was used as a reference. Generally, tolerance to ESD of larger  than 1.0 kV is required for optoelectronics LDs. We carried  out the tilt polish process for both LDs using the same


(i)


(e)(c)


(h)


100 µm


procedure as shown in Figure 4. The mapping of EL intensity  from the backside of the LD is shown in Figure 6. Figures 6(a) and 6(b) represent emission using the reference LD and the  degraded-LD respectively. Three bright lines were observed  during EL analysis. The centerline represent EL emission from  an active layer and the two adjacent lines represent reflection  from the side electrode. EL emission was observed from facet  to facet for the reference LD. However, a dark region, which  indicates the degraded-region, was observed for the  degraded-LD. Therefore, we were able to judge the facet  region that was degraded by the ESD test.


Figure 6: The mapping of the EL intensity from the back side  of the LD. (a) the reference LD. The dashed line indicates  outline of the LD chip. (b) the degraded LD by the 1.0 kV ESD  test.


In conclusion, a process for EL analysis was developed that  was effective in performing degradation analysis of  optoelectronics LD. This method has merit to be applicable to  practical LDs. Though precise control was required, almost  100 % yield was achieved by introduction of tilt polish  technique.


[1] Y. Twu, L. S. Cheng, S. N. G. Chu, F. R. Nash, K. W. Wang and P. Parayanthal, “Semiconductor laser damage  due to human-body-model electrostatic discharge” J. Appl. Phys., Vol. 74, No. 3 (1993) pp. 1510-1520.


[2] T. Sasaki, H. Mori, M. Tachikawa and T. Yamada, “Aging tests of InP-based laser diodes heteroepitaxially  grown on Si substrates” J. Appl. Phys., Vol. 84, No. 12


(1998) pp. 6725-6728.


[3] E. Nomoto, K. Nakahara and M. Shimaoka, “Stress on  junction-down-mounted ridge-waveguide laser diodes” Jpn. J. Appl. Phys., Vol. 44, No. 4A (2005) pp. 1756-1758.


300 µm


EL emission


Degraded region


DOI: 10.1361/cp2008istfa269


A Novel OBIRCH Fault Isolation Method to Locate the Leakage Failure Point


Chi-Lin Huang ,Yu Hsiang Shu


Phone: 886-3-5782258 ext 37312 Fax: 886-3-563-6722 Email:Chi_lin_Huang@umc.com


Conventional isolation techniques, such as Optical Beam  Induced Resistance Change (OBIRCH) or photoemission  microscopy (PEM) frequently fail to locate failure points  when only applied to power pin of the semiconductor device. In this paper, a novel OBIRCH failure isolation technique is  utilized to detect leakage failures. Different test conditions are  presented to identify the differences in current when all input  pins are pulled high in an OBIRCH system. In order to verify  a failure point, it is necessary to perform electrical analysis of  the suspected failure point in the failing sample. In general, Conductive Atomic Force Microscope (C-AFM) and a NanoProber is sufficient to provide the electrical data required for  failure analysis. Experiment results, however, prove that this  novel OBIRCH failure isolation technique is effective in  locating the failure point, especially for leakage failures. The  failure mechanism is illustrated using cross-sectional TEM.


With the evolution of advanced process technology, failure analysis has become difficult when attempting to  isolate failure points, especially leakage failures. Standard  failure localization methods like OBIRCH, PEM, and LCD (Liquid Crystal Display) are sometimes not successful when  applied to a power pin only. A novel OBIRCH failure  isolation technique is presented in this paper. A simple circuit  shown in Figure 3 explains the failure isolation principle.


C-AFM and a Nano-Prober are utilized to verify the  suspected failure point in the sample. Based on the C-AFM,


leakage occurring at the diffusion contacts can be found in the  failing sample. The Nano-Prober is used to measure the  diffusion leakage; a high I-off current is measured at the  suspected location.


The failure mechanism is revealed through the crosssectional TEM image. The leakage path is identified as silicide  extending into the spacer, which causes the observed leakage  current.


Experiment and Results


To prove the effectiveness of the novel OBIRCH based  failure isolation technique, specimens manufactured using an  advanced process with soft defects were chosen as samples for  the experiment. Conventional failure isolation, which only


forced VDD and GND was deployed first. The suspected  failure point could not be isolated using the conventional  method, as shown in Figure 1. A novel failure isolation  technique was attempted. This technique utilizes different test  conditions to determine the difference in current when all  input pins are pulled high in the OBIRCH system. A  difference in the signal was observed between the  conventional and the novel failure isolation method on the  failing sample, as shown in Figure 2.


Figure 1: Conventional failure isolation (OBIRCH) did not  find the suspected failure point in (a) the good sample (b) the  failing sample.


Figure 2: Novel failure isolation technique using the OBIRCH  system. (a) No failure point was observed on the good sample.


(b) Failure point was observed on the failing sample.


(a) (a)


Therefore; when input pins are to go high, some circuits  gates are opened and current pass through those circuits by  comparison only forcing VDD and GND. If have any  abnormal current in those circuit, hot spot will be highlighted  by OBIRCH.


The simple circuit shown in Figure 3 explains why the  OBIRCH system isolated the suspected failure point on the  failing sample using the novel technique. If we force all the  input pins to go high, both the current flowing to the CMOS  inverter and the voltage becomes low at the output of the  CMOS inverter. Normally, the current passes through the  internal circuit and the output terminal voltage becomes high, so the N2 gate should be closed and the I-off current should  be very low in normal devices. However, a high I-off current  was measured on node A on the failing sample. Figure8 shows  the actual I-off current that was measured by the Nano-Prober  for both good and failing samples.


Figure 3:  A simple circuit used to simulate a high I-off  current path on the failing sample.


Figure 4: The high I-off current path is detected using the  OBIRCH system.


The high I-off current can be detected using the OBIRCH  system, and therefore the failure point can be located on the  failing sample due to high I-off current (Figure 4).


Figure 2 shows a difference in the signal between the  conventional and the novel failure isolation technique. After  deprocessing layer by layer down to the contact area, plane  view optical microscopy (PV-OM) and plane view secondary  electron microscopy (PV-SEM) were utilized to inspect the  failure point.  However, no defect was found in back-end  process on the failing sample.


C-AFM was used to verify the failure point. C-AFM has  a scale lateral resolution and is able to measure the current in  the pico-amp range. It is widely used for semiconductor  failure analysis application. The schematic is shown in Figure


5.


Figure 5: A schematic of Conductive Atomic Force  Microscopy.


C-AFM, identified the failure point. By combining  current mapping with an IV-curve, the leakage path can be  found, including gate oxide leakage, junction leakage and  poly contacts shorted to other contacts (poly, N+ or P+ contacts) [1]. Figure 6 shows the difference in the current  mapping of diffusion contacts by comparing both good and  failed samples.


According to the current mapping shown in Figure 6, it is  known that different color current mapping images react to  different electrical characteristics on the IV curve. Based on  the difference in the current mapping, leakages were found in  the failing sample as compared to the good sample (Figure 7).  To further confirm the results from the C-AFM, the  Nano-Prober was uesd to measure the device leakage current  at the failure point located using C-AFM. The Nano-Prober  technique uses four tungsten needles mounted to accurate  micro-manipulators in an SEM chamber. The four needles are  connected to electrical tracer equipment that enables IV  characteristics to be collected. By utilizing the Nano-Prober  technique, a complete electrical defect isolation and  characterization was performed. This aided in better  understanding of the electrical behavior of the failure point on  the failing sample. Figure 8 shows the difference in I-off


current for both the good and the failing sample using the  Nano-Prober. Obviously, the I-off current is higher in the  failing samples than in the good samples.


Input Pin


GND


I-off  current


VDD


0 Internal Circuit


N1


Node A


N2


Figure 6:  C-AFM current mapping image of (a) good sample   and (b) failing sample. Leaky diffusion contacts were found on  the failing sample by comparing good vs. failing samples  current mapping image.


Figure 7: I-V characteristics of the suspect failing location  are demonstrated for the good and failing samples. Diffusion  leakage is found on  the failing sample.


Diff


Figure 8: I-off current is measured for both the good and the  failing samples using the Nano-Prober. Measurement  conditions are Vg=Vs=0V with Vd swept from 0V to 2.1V. The  I-off current for the faling sample is 9.76E-07A and I-off  current for the  the good sample is 1.38E-09A when Vd=1.8V  and Vg=Vs=0V.


In order to understand the failure mechanism that caused  a leakage path in the failing NMOS transistor, cross-sectional  TEM imaging was utilized. Figure 9 shows that the silicide  extends to the spacer, which causes the diffusion lekage  shown in Figure 7 and the high I-off current shown in Figure


Silicide extends to spacer


Figure 9: A cross-sectional TEM image of the failing sample  is shown, the silicide extending into the spacer region is  observed.


Based on the cross-sectional TEM image, the leakage  current identified using C-AFM can be attributed to the silicde  extending into the spacer region. The leakage path is shown in  Figure 10, which shows a high I-off current on the failing  sample.


Figure 10: The Leakage path is due to the silicide extending  into the spacer region, which then causes the leakage current  in (b).


Advances in semiconductor technology have resulted in  high component density and small device dimensions. As the  technology continues to scale down, defect sizes tend to  decrease and non-visual defects (leakage) have become more  prominent. As a result defect isolation has become difficult.  The purpose of this work was to overcome the difficulty  in isolating failure points in devices exhibiting soft failures. However, a soft defect is usually not resolved using  conventional FA methods or tools, are not sufficient to  identify the root cause of the failure. In this paper, a novel  failure isolation technique using the OBIRCH system  combined with C-AFM/Nano-Prober successfully located soft  defects. Experiment results prove that this novel failure  isolation technique is capable of isolating soft defects and is  an excellent method for failure isolation involving  semiconductor failure analysis.


[1]. Z.H. Lee, C.J. Lin, S.W. Lai and J.H. Chou, "Gate Oxide  Defect Localization and Analysis by Using Conductive  Atomic Force Microscopy", ISTFA 2005, pp235-238


DOI: 10.1361/cp2008istfa273


Case Study of High Temperature Failure Analyses Using an On-Chip “Heater”


Fubin Zhang, Corey Lewis


Texas Instruments Inc. DDAO, Dallas, TX   fzhang@ti.com


Tim Duryea


Texas Instruments Inc. HVAL/MSA, Dallas, TX


Two cases of high temperature failure analyses are presented. In both cases an on-chip “heater” – power MOSFET was used  to achieve high temperature for both global fault isolation and  block/transistor level nodal analysis. The “heater” provides a  quick and effective way of changing the device temperature  without significantly modifying the bench setup. In both  cases, the results show improved probability of successfully  isolating the fail site, by performing OBIRCH analysis and  nodal analysis.


As the integrated circuit industry moves toward smaller  feature sizes to achieve lower cost and better performance, failure analysis faces more challenges. New techniques have  been developed to conquer some of these new territories  during the last two decades. High temperature failure is  definitely one of the most difficult areas for fault isolation  work. The most common way of analyzing high temperature  failures is to use a socket with a metal pin attached to a heater  to control the temperature of the device. However, this option  usually is not available for most of the evaluation boards. And  it is costly to have a temperature control socket on bench  setups. This paper will present two case studies of high  temperature failure analysis using an on-chip power MOSFET  to control failing device temperature.


High temperature failures of Mixed-signal and analog  power IC


Mixed-signal and analog power IC’s are widely used in  industry. Almost all of them have active power control  components such as high current or voltage BJTs, MOSFET’s, ect., integrated on the chip. Most of these devices are designed  to operate in a wide temperature range either because the  working environment they are used in or the heat generated  from their own operation. In many cases, the failure only  occurs at high temperature. This requires failure analysis to be  performed on the device at an elevated temperature. Traditionally an external heater is used to heat up the unit.


Methods and Analysis


Many mixed-signal or SOC (system on chip) IC’s contain  integrated linear regulators for power management purposes. These circuits are ideal for increasing die temperature because  they are inherently inefficient. Increasing the load current  and/or input supply rail will cause large on chip power  dissipation. Care should be used to insure the device is not  damaged by the loading so correlation devices should be  tested first. In addition to linear regulators, other common  circuits such as high current low-side or high-side power  switches could be used to increase die temperature.


The alternative way to heat up the device temperature is to use  an on-chip power FET (Field Effect Transistor) in the  regulators or power switches. The power generated from the  FET can be calculated as I2×Rdson, I is the current flowing  through the FET and Rdson is the on-state channel series  resistance. Figure 1 shows a simplified setup diagram for  heating up the DUT (Device under Test) temperature by  adjusting the amount of current flowing through the on-chip  power FET. The current I, can be modified by adjusting the  load resistance on the power FET output. Also, the power  dissipation of the DUT should be taken into consideration in  determination of the amount of current flowing through the  power FET to prevent over-heating or even damage to the  DUT. The advantage of this approach is it can be easily  realized on a bench setup or an evaluation board without  attaching any heat conducting unit to the DUT.


The die temperature also can be measured through an on-chip  temperature sensor. If the device does not have an integrated  temperature sensor for estimating the temperature then the die  temperature can be approximately measured using the reverse  diodes present in most ESD structures. Since the temperature  coefficient of a forward biased PN junction has a fairly  constant characteristic, it can be used to obtain a measure of  the die temperature. A device pin that is not needed for  reproduction of the failure, such as unused analog or digital  inputs, can be used for this purpose. By pulling out a constant  current from the pin’s ESD or substrate diode and  characterizing the voltage on the pin across temperature using  a thermal stream while the part is un-powered, a fairly  accurate die temperature senor can be obtained. This sensor


can then be used to determine how much heating is needed  from the integrated power transistor to achieve the desired  temperature the failure occurs at.


Figure 1: Simplified setup diagram for using power FET to  heat up the DUT temperature. The red dotted line indicates  the current flow through the power FET.


Global fault isolation at elevated temperature


PEM (Photon emission microscopy), TIVA (Thermal Induced  Voltage Alteration), OBIRCH (Optical Beam Induced  Resistance Change), and LIVA (Light Induced Voltage  Alteration) are some of the most commonly used global fault  isolation techniques [1]. For high temperature failures, it will  give us better chance to identify the fail site if global fault  isolation is performed at an elevated temperature. For  instance, if a leakage only exists at high temperature, most of  the time it is necessary to run PEM or OBRICH while the  failing device is heated.


Block or transistor level nodal analysis at high  temperature


When global fault isolation could not pin point the fail site, block/transistor level nodal analysis becomes critical to  identify the failure mechanism. This includes electrical  measurements such as voltages, currents, or waveforms  performed at block/transistor level to filter out the failing  blocks or transistors.


Case Study


Two devices are analyzed. Both were processed on the same  sub-micron Bi-CMOS technology. Both devices are mixedsignal power IC used in automotive applications (Figure 2).


Case 1


The failure mode was confirmed on the ATE (Automated Test  Equipment) and bench level setup. One analog block was  failing with leakage on an internal regulated power supply. Global fault isolation (PEM and OBIRCH) was not conclusive  even at high temperature. Through nodal analysis, the fail site  was narrowed down to the protection block (Figure 3) on the


3.3V power supply line for the FMON (fail monitoring) block. IV sweeps across the Zener diode showed a leakage (Figures  4 and 5). This Zener diode triggers the protection block to be  active and caused the device to fail. Although the diode is


leaking at room temperature, it is just close to the limit. The  leakage gets worse at high temperature, which pushed the  current over the edge, triggered the protection and caused the  failure. PEM over the Zener while directly biasing across the  Zener diode showed an emission site (Figure 6). TEM through  the emission site at the failing diode showed dislocation  defects in the silicon (Figure 7).


Figure 2: Optical image of the device die. Fail sites identified  in cases 1 and 2 are indicated with red arrows. The power  LDMOS used as a heater is highlighted with the blue  rectangular.


Figure 3: (Case 1) Schematic of the failing block.


Load


Power Supply


Power FET


Figure 4: (Case 1) IV sweeps from node F to GND shows a ~400nA leakage on the fail unit, with power on. The leakage  gets worse at high temperature, causing the part to fail.


Figure 5: (Case 1) IV sweeps across the failing Zener diode  show low level leakage on the failing device even at room  temperature.


Figure 6: (Case 1) PEM image at the failing Zener diode D6  showed an emission site (red arrow). A 4V bias was applied  across the diode while running the PEM.


Figure 7: (Case 1) TEM image shows silicon dislocation  defect (red arrows) at the failing diode.


Case 2


In this case, OBIRCH analysis was performed and revealed an  alteration site only when the device was heated using an onchip power FET. The OBIRCH analysis was performed using  a combination of horizontal and vertical scans to location the  alteration site (Figure 8) since the failure was triggered by the  laser and the unit would stay in the failing state without  cycling the power. The alteration site is at the cross of the two  transition lines and was identified to be in the thermal shut  down block. Micro probing and voltage measurements on  internal nodes of the failing thermal shut down block showed  incorrect biasing current for the thermal shut down resistor. A  leakage on the current biasing node F was isolated to a  location in Figure 9. FIB (Focused Ion Beam) cross section  found a launched tungsten plug (Figure 10). This defect  caused a larger bias current and the thermal shut down circuit  to act at a relatively lower temperature. Although in this case  global fault isolation did not pin point the fail site but it lead  to the malfunction block.


Figure 8: (Case 2) OBIRCH analysis image shows an  alteration site (red circle) in the thermal shutdown block bias  circuitry.


Figure 9: (Case 2) FIB slow scan image shows the isolated  metal 1 on node F remained bright (red arrow), indicating a  leakage.


Figure 10: (Case 2) FIB slow scan image shows a launched  tungsten plug (red arrows) between two adjacent metal lines.


Conclusions and Acknowledgments


An approach to analyze high temperature failures using an onchip power FET is presented. It can be used for both global  fault isolation and block/transistor level nodal analyses. As  demonstrated in the case study, this analysis technique has  generated positive results.


The authors would like to thank Daniel Callahan for his  support of the work in this paper.


[1] Microelectronics Failure Analysis, Desk Reference Fifth  Edition, Chapters 8 and 10.


DOI: 10.1361/cp2008istfa277


Development of PECS Application for Sample Preparation


Xianfeng Chen, Ming Li, Qiang Guo, W.T. Kary Chien


A cross sectional view of a device can provide  information for qualification, process monitor  and failure analysis. Therefore, cross sectional  polishing has been widely used in the  semiconductor industry. The typical polishing  procedure includes wafer cutting, planar  grinding, rough polishing, final polishing and  water cleaning. The purpose of final polishing  is to remove surface damage induced during  rough polishing. However, Final Polishing is  not a green sample preparation method  because much of the un-recycled submicron  abrasive used contaminates water. Also final  polishing is time-consuming and difficult to  control. Generally, the analyst must spend  more than 30 minutes to complete one final  polishing cycle. Samples including both  ductile and brittle material are prone to  smearing, distortion, edge rounding, micro-scratch, crystallization contamination, relief and embedding of the rolling abrasives  when improper polishing parameters such as  down force, direction, speed and time were  applied. Smearing, edge rounding, micro relief  and micro-scratch caused by crystallized  abrasive increase as final polishing is applied  to decrease artifacts induced during rough  polishing. In addition, specimen surface  contamination with polishing artifacts could  be worse after a chemical stain. Some  researchers reported that final polishing time  is about 8 minuets for IC sample cross-section  polishing [1][2]. Actually, final polishing time  depends strongly on rough polishing quality  and technician skill because it is difficult to  control down force and direction manually. Usually, the final polishing time is more than


that, even about 20minutes. As demand for  higher throughput increases the time spent  manually performing a final polish is the  improper method for cross-section  preparation.


PECS (Precise Etching and Coating System) is an ion beam based etching and sputter  coating system for SEM and TEM sample  preparation. Etching is the major function of  PECS. The ion beam can mill the specimen  and can be used, in a controlled way, to  expose any desired feature of the specimen. Ar  gas based plasma is available in the PECS  system. Ar plasma etching can act as a  cleaning step. Ar etching has been developed  to replace the time-consuming final polishing  step. In this work, we mainly focus on Ar  plasma cleaning performance on a sample  after rough polishing and a sample after a  short time final polishing.


Experiments


To evaluate performance of Ar plasma  cleaning, three samples were prepared for  SEM observation.


Sample1


A portion of an IC wafer with Cu/SiO2  interconnect was prepared using the following  steps: wafer cutting, planar grinding and rough  polishing. The rough polishing procedure was  run with 3M diamond lapping film from 9  micron down step by step to 6, 3,1 and


0.5micron. In this test the polishing cloth is  Porometric Polymer Pads with medium nap.


Sample2


A portion of an IC wafer with Cu/SiO2  interconnect was prepared following the  procedure of sample 1. Two additional steps  were added, 30 seconds of final polishing with


0.05micron colloidal silica suspension and  about 10 seconds of running water cleaning  executed on the same polishing cloth.


Ar plasma cleaning was applied to all samples  after polishing.


Result & Discussion


Fig.1 and Fig.2 are of sample1. Fig.1 in an  image of X-SEM image before Ar plasma  cleaning and Fig.2 is an image after Ar plasma  cleaning. By comparing Fig.2 with Fig.1, we  see sample surface damage induced by rough  polishing can’t be removed completely. Smearing and micro scratch are still observed  after Ar plasma cleaning as shown in Fig.2. Ar  plasma cleaning is not an effective method to  correct micro scratches.


Fig.1 sampe1 X-SEM image taken before Ar  plasma cleaning.


Fig.2 sampe1 X-SEM image taken before Ar  plasma cleaning. Cleaning parameters: I=100uA, T=2minute, E=6KeV, R=20rmp.


Fig.3 shows abrasive residue, relief, smearing  and crystallized abrasive. But no micro  scratches are observed. The main purpose of  the short time final polishing is to remove  micro scratches induced by rough polishing. Per the experiment of sample1, the conclusion  is made that the micro abrasive residue, relief  and crystallized abrasive were introduced  during final polishing. Fig.4, shows all these  artifacts can be removed after PECS Ar  plasma cleaning with gun parameter I=200uA, T=2 minute and E=6KeV. Anyway, 30seconds  final polishing.


Fig.3 Sample2: X-SEM image taken before Ar  plasma cleaning.


Fig.4 Sample2: X-SEM image taken after Ar  plasma cleaning by PECS.


Ar plasma cleaning has other advantages, it  can be used to replace time spent final  polishing. In Fig.2 and Fig.4, the  metallographic structure and interface are  observed. Ar plasma cleaning can also  decorate the sample cross section. Therefore, final polishing and stain can be combined into  one step improving sample quality and  throughput. Sometimes, chemical staining is  still necessary for silicon based oxide  thickness measurements because Ar plasma  etching has poor etch selectivity for  SiO2/SiN/Si. But chemical staining for


Abrasive


Smearing  Micro scratch

