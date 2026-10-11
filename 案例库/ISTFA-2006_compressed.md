---
title: "ISTFA-2006_compressed.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_686e3b5ad586984da6cb8498be68a5ba7295230462135641
file_size: 67042538
---

ISTFA  2006TM   Proceedings of the


32nd International Symposium


for Testing and Failure Analysis


November 12–16, 2006  Renaissance Austin Hotel


Austin, Texas, USA


Sponsored by


www.asminternational.org/istfa


www.asminternational.org


Published by


ASM International®


Materials Park, Ohio 44073-0002


Copyright© 2006


by


All rights reserved


No part of this book may be reproduced, stored in a retrieval system, or transmitted, in any form or by any  means, electronic, mechanical, photocopying, recording, or otherwise, without the written permission of  the copyright owner.


First printing, November 2006


Great care is taken in the compilation and production of this Volume, but it should be made clear that NO  WARRANTIES, EXPRESS OR IMPLIED, INCLUDING, WITHOUT LIMITATION, WARRANTIES  OF MERCHANTABILITY OR FITNESS FOR A PARTICULAR PURPOSE, ARE GIVEN IN  CONNECTION WITH THIS PUBLICATION. Although this information is believed to be accurate by  ASM, ASM cannot guarantee that favorable results will be obtained from the use of this publication alone. This publication is intended for use by persons having technical skill, at their sole discretion and risk. Since  the conditions of product or material use are outside of ASM's control, ASM assumes no liability or  obligation in connection with any use of this information. No claim of any kind, whether as to products or  information in this publication, and whether or not based on negligence, shall be greater in amount than the  purchase price of this product or publication in respect of which damages are claimed. THE REMEDY  HEREBY PROVIDED SHALL BE THE EXCLUSIVE AND SOLE REMEDY OF BUYER, AND IN NO  EVENT SHALL EITHER PARTY BE LIABLE FOR SPECIAL, INDIRECT OR CONSEQUENTIAL  DAMAGES WHETHER OR NOT CAUSED BY OR RESULTING FROM THE NEGLIGENCE OF  SUCH PARTY. As with any material, evaluation of the material under end-use conditions prior to  specification is essential. Therefore, specific testing under actual conditions is recommended.


Nothing contained in this book shall be construed as a grant of any right of manufacture, sale, use, or  reproduction, in connection with any method, process, apparatus, product, composition, or system, whether  or not covered by letters patent, copyright, or trademark, and nothing contained in this book shall be  construed as a defense against any alleged infringement of letters patent, copyright, or trademark, or as a  defense against liability for such infringement.


Comments, criticisms, and suggestions are invited, and should be forwarded to ASM International.


ISBN-13:978-0-87170-844-1


ISBN-10: 0-87170-844-2


SAN: 204-7586


Materials Park, OH 44073-0002


Printed in the United States of America


Multiple copy reprints of individual articles available from Technical Department, ASM International.


EDFAS 2006-2007 BOARD OF DIRECTORS


EDFAS President


EDFAS Vice President


Dr. Daniel L. Barton


Dr. Christian Boit


Sandia National Laboratories


TUB – Berlin University of Technology


Albuquerque, NM


Berlin, Germany


|Board Members |Board Members |Affiliation |
|---|---|---|

|Dr. Lee Knauss |Member At Large |Neocera Incorporated |

|Dr. Thomas Moore |Member At Large |OmniProbe |

|Mr. Tracy Myers |Secretary |ON Semiconductors |

|Dr. Seshagiri Pabisetty |Member At Large |Eagle Registration Inc. |

|Mr. Thomas S. Passek |Executive Director |ASM International |

|Dr. Philippe Perdu |Member At Large |CNES |

|Mr. Gary Shade |Immediate Past President |Intel Corporation |

|Mr. Matthew Thayer |Financial Officer |Advanced Micro Devices |

|Mr. David Vallett |Member At Large |IBM Systems & Technology Group |

|Board C ommittees |Board C ommittees |Affiliation |

|Dr. Lawrence Wagner |ASM BOT Liaison |Texas Instruments, Incorporated |

|Dr. Edward I. Cole, Jr. |EDFA Chair |Sandia National Laboratories |

|Mr. Thomas Zanon |Education Chair |PDF Solutions Inc. |

|Ms. Cheryl Hartfield |Events Chair |Texas Instruments, Incorporated |

|Dr. Jacob C. H. Phang |Journal Chair |National University of Singapore |

|Dr. Vijay Chowdhury |Membership Chair |Altera Corporation |

|Mr. Richard J. Ross |Nominating Chair |IBM Systems and Technology Group |

|Mr. Srikanth Perungulam |Website Chair |Texas Instruments, Incorporated |

iii


ISTFA 2006 ORGANIZING COMMITTEE


ISTFA 2006


General Chair


Cheryl Hartfield


Texas Instruments, Inc.


Vice General Chair


Chris Henderson  SemiTracks, Inc.


Technical Program Chair


David P. Vallett


IBM Systems & Technology Group


Tutorial Program Chair


Tracy Myers


ON Semiconductors


Activities Chairs


|Nicholas Antoniou |Lee Knauss |William E. Vanderlinde |
|---|---|---|

|User Groups Chair |Immediate Past General Chair |Audio/Visual Chair |

|Credence Systems Corporation |Neocera, Inc. |Laboratory for Physical Sciences |

|Dan J. Bodoh |Thomas Moore ||

|Website Chair |EDFAS Liason |Jeremy A. Walraven |

|Freescale Semiconductor |Omniprobe, Inc. |Panel Discussion Chair |

|||Sandia National Laboratorie |

|Victoria Bruce |Philippe Perdu |Philippe Perdu |

|Local Arrangements/Publicity |Exposition Chair |Exposition Chair |

|Chair |CNES |CNES |

|Advanced Micro Devices |||

s


iv


ISTFA 2006 TUTORIAL COMMITTEE


Tracy D. Myers


|Tutorial Committee Chair |Topic |Affiliation |
|---|---|---|

|Vijay Chowdhury |EOS/ESD |Altera Corporation |

|Cosme Furlong |Fault Isolation; Microscopy Tools |Worcester Polytechnic Institute |

|Leo G. Henry |Failure Mechanisms |ESD TLP Consulting/Testing |

|Rebecca L. Holdford |Packaging; Yield |Texas Instruments, Inc. |

|Susan Li |Device and Test |Spansion, LLC |

|Tracy D. Myers |Device and Test; Emerging |ON Semiconductors |

|Tracy D. Myers |Technologies; Failure Management; |ON Semiconductors |

|Tracy D. Myers |Lead Free Packaging |ON Semiconductors |

|Chris Richardson |Fault Isolation; Focused Ion Beam |LSI Logic Corporation |

|Rosalinda M. Ring |Device and Test; Emerging Technologies |Intel Corporation |

|Sam Subramanian |Materials Characterization; Microscopy Tools |Freescale Semiconductor, Inc. |

|William E. Vanderlinde |Fault Isolation; Microscopy Tools |Laboratory for Physical Sciences |

|Zhiyong Wang |Lab Management; Lead Free Packaging |Intel Corporation |

|Jeremy A. Walraven |MEMS Devices |Sandia National Laboratories |

|Kendall S. Wills |Fault Isolation |Texas Instruments, Inc. |

v


ISTFA 2006 SYMPOSIUM COMMITTEE


ADVANCED TECHNIQUES


Seth Prejean, Adv Frank Zheng, Free


Intel Corporation


Nicholas Antoniou,


DIE LEVEL FAULT ISOLATION


POSTERS


|ISTFA 2006 |ISTFA 2006 |JOSEPH CLEMENT, CHAIR |JOSEPH CLEMENT, CHAIR |ROSALINDA M. RING, CHAIR |
|---|---|---|---|---|

|IS TFA 2006|IS TFA 2006|Sandia National Laboratories|Sandia National Laboratories|Intel Corporation|

|Technical  Program Chair|Technical  Program Chair||||

|Technical Program Chair |Technical Program Chair |Dan Bodoh, Freescale Semiconductor, Inc. |Dan Bodoh, Freescale Semiconductor, Inc. |Mike Bruce, Advanced Micro Devices |

|||Michael Bruce, Advanced Micro Devices |Michael Bruce, Advanced Micro Devices |Joseph Buben |

|||Edward Cole, Sandia National Laboratories |Edward Cole, Sandia National Laboratories |USA Defense Logistics Agency |

|||Theodore Lundquist, Credence Systems Corp. |Theodore Lundquist, Credence Systems Corp. |David Burgess, Accelerated Analysis |

|||Jerome Touzel, Infineon Technologies AG |Jerome Touzel, Infineon Technologies AG |Oscar Camposagrado, Intel Corp. Wen-Hsien Chuang, Intel Corp. |

|||DISCRETES, PASSIVES, MEMS, |DISCRETES, PASSIVES, MEMS, |David Dylis, IIT Research Institute |

|||||Lili Esfahani, Pericom Semiconductor |

|||OPTOELECTRONICS |OPTOELECTRONICS |Jack Henderson, Naval Surface |

|||DAVID BURGESS, CHAIR |DAVID BURGESS, CHAIR |Warfare |

|||Accelerated Analysis |Accelerated Analysis |Terrance Kane |

|||Richard Blanchard, SVEWG |Richard Blanchard, SVEWG |IBM Systems & Technology Group |

|||Mahmood Choudry, International Rectifier |Mahmood Choudry, International Rectifier |Martin Keim, Mentor Graphics |

|||Stan Silvus, Southwest Research Institute |Stan Silvus, Southwest Research Institute |Mark Kimball, Maxim Integrated |

|||||Products, Inc. |

|||METROLOGY AND MATERIALS |METROLOGY AND MATERIALS |Theodore Kolasa |

|||ANALYSIS |ANALYSIS |Freescale Semiconductor |

|David P. Vallett |David P. Vallett |SAM SUBRAMANIAN, CHAIR |SAM SUBRAMANIAN, CHAIR |Thomas Libbey, National Semiconductor |

|IBM Systems |IBM Systems |Freescale Semiconductor, Inc. |Freescale Semiconductor, Inc. |Perry Martin, Martin Testing Labs |

|and Technology Group |and Technology Group |Ercan Adem, Spansion LLC |Ercan Adem, Spansion LLC |John McDonald |

|||Roger Alvis, Imago Scientific Instruments Corp. |Roger Alvis, Imago Scientific Instruments Corp. |Quantum Focus Instruments |

|||Robert Hands, Department of Defense |Robert Hands, Department of Defense |Jacob Phang |

|||Srikanth Perugulam, Texas Instruments, Inc. |Srikanth Perugulam, Texas Instruments, Inc. |National University of Singapore |

|ADVANCED TECHNIQUES|ADVANCED TECHNIQUES|Chris Richardson, LSI Logic |Chris Richardson, LSI Logic |Thomas Paquette, Insight Analytical |

|RAJEN DIAS, CO-CHAIR |RAJEN DIAS, CO-CHAIR |Bryan Tracy, Spansion LLC |Bryan Tracy, Spansion LLC |David Su, TSMC, Ltd. |

|Intel Corporation BENAIAH SCHRAG, CO-CHAIR |Intel Corporation BENAIAH SCHRAG, CO-CHAIR |NANOTECHNOLOGY/NANOPROBING |NANOTECHNOLOGY/NANOPROBING |SCANNING PROBE |

|Micro Magnetics |Micro Magnetics |TERRANCE KANE, CO-CHAIR |TERRANCE KANE, CO-CHAIR |MICROSCOPY |

|Rama Goruganthu, Advanced Micro Devices |Rama Goruganthu, Advanced Micro Devices |PHILIP KASZUBA, CO-CHAIR |PHILIP KASZUBA, CO-CHAIR |RAMA GORUGANTHU, CHAIR |

|Philip Kaszuba, IBM Systems & Technology Group |Philip Kaszuba, IBM Systems & Technology Group |IBM Systems & Technology Group |IBM Systems & Technology Group |Advanced Micro Devices|

|||IBM Systems & Technology Group|IBM Systems & Technology Group|Advanced Micro Devices |

|Roger Stierman, Texas Instruments, Inc. |Roger Stierman, Texas Instruments, Inc. |Zachary Levine, NIST |Zachary Levine, NIST |Terence Kane |

|||Leon Moszkowicz |Leon Moszkowicz |Phillip Kaszuba |

|ANALYTICAL PROCESS|ANALYTICAL PROCESS|IBM Systems & Technology Group |IBM Systems & Technology Group |IBM Systems & Technology Group |

|ANALYTICAL PROCESS |ANALYTICAL PROCESS |Ben Schrag, Micro Magnetics Inc. |Ben Schrag, Micro Magnetics Inc. |Paiboon Tangyunyong |

|BRENNAN DAVIS, CHAIR |BRENNAN DAVIS, CHAIR |James Slinkman, EWA |James Slinkman, EWA |Sandia National Laboratories |

|Advanced Micro Devices Timothy Cheng, Freescale Semiconductor, Inc. |Advanced Micro Devices Timothy Cheng, Freescale Semiconductor, Inc. |Paiboon Tangyunyong |Paiboon Tangyunyong |Lise Varner, Intel Corporation |

|Michael Santana, Jr., |Advanced Micro Devices |William E. Vanderlinde, Laboratory for |William E. Vanderlinde, Laboratory for |Lawrence Wagner, Texas Instruments|

|||Physical Sciences ||SYSTEM LEVEL ANALYSIS |

|CHEMICAL/MECHANICAL |/MECHANICAL|||JEFF BIRDSLEY, CHAIR |

|SAMPLE PREP ||OPTICAL |FAULT ISOLATION |Dell Corporation |

|EDWARD KEYES, CHAIR||AARON FALK, |CHAIR |Roger Bjork, Dell Corporation |

|EDWARD KEYES, |CHAIR |OptoMetrix, Inc. ||Sridhar Canumalla, Nokia |

|Semiconductor Ted Kolosa, |Insights Freescale Semiconductor, Inc. |Grant Albright, |Quantum Focus Instruments |Robert Knoell, Visteon Corporation |

|Seth Prejean, Advanced Micro Devices|anced Micro Devices |Marc de la |Bardonnie, EFA |Michael Lane, Intel Corporation |

||Frank Zheng, Freescale Semiconductor, Inc.|Felix Beaudoin, Credence |Systems Corp. |Randall Schueller, Dell Corporation |

||scale Semiconductor, Inc. |Tom Kujawa, Hypervision |Inc. |Daren Slee, Exponent Failure Analysis |

|||Ted Levin, IBM |Systems & Technology Group |Jan Swart, Exponent Failure Analysis |

|CIRCUIT |EDIT/BEAM-BASED |Franco Stellari, IBM |Systems & Technology Group ||

|SAMPLE PREP ||Qian Zhongling, |Infineon Technologies AG |TEST DIAGNOSTICS |

|MARSHA |ABRAMO, CO-CHAIR |||ROWLAND BLANTON, CHAIR |

|IBM Systems & |Technology Group |PACKAGE |LEVEL ANALYSIS |Carnegie Mellon University |

|CAMERON |WAGNER, CO-CHAIR |DEEPAK GOYAL, |CO-CHAIR |Rao Desineni |

|||Intel Corporation ||IBM Systems & Technology Group |

||Credence Systems Corp. |Stephane Barbeau ||Brion Keller |

|Michael Phaneuf, |Fibics Inc. |IBM Systems & |Technology Group |Cadence Test Design Automation |

|Chad Rue, FEI |Company |Zezhong Fu, Intel |Corporation |Andreas Veneris, University of Toronto |

|Milton Tam, |Raytheon Company |Andrew Mawer, Freescale |Semiconductor ||

|||David Maxwell, |Texas Instruments, Inc. |YIELD ANALYSIS |

|||||CAROL BOYE, CHAIR |

|||||IBM Systems & Technology Group |

|||||Alfredo Herrera, Advanced Micro Devices |

|||||Diana Mitro, Motorola |

Lawrence Wagner, Texas Instruments


Oliver Patterson, Agere Systems


Thomas Taylor, Infineon Technologies AG


vi


33rd International Symposium for Testing and Failure Analysis


|ISTFA/2007|Sponsored by |
|---|---|

|November 4-8 • McEnery Convention Center • San Jose, CA |Electronic Device Failure Analysis Society |

|n 员||

|Dream||

--1"


wwwh.org


www.thetech.org


TheTech museum of innovation


201


FIRST


ANNOUNCEMENT  AND


CALL FOR PAPERS


ISTFA solicits original, previously unpublished  papers on a wide range of Testing and Failure  Analysis topics of practical value to anyone  working to detect, understand and eliminate  electronic device and system failures.  Instructive case studies, review papers, and  root-cause analyses are encouraged. Noncommercial papers from equipment vendors


dealing with new or unique tools and  methodologies, applications and results are  welcome.  Papers will be selected for inclusion  in the technical program based on four factors: novelty, completeness, quality, and benefit to the  FA community. Paper acceptance will be based  entirely on the information included in the  extended abstract


.


We are currently seeking abstracts on (but not limited to) the following relevant topics*


|Advanced Techniques |MEMS |Optoelectronic Devices |System Level Analysis |
|---|---|---|---|

|Circuit Edit for FA, FI, & Debug |Metrology & Materials Analysis |Package Level Analysis |Test |

|Die Level Fault Isolation |Nanotechnology Analysis |Sample Preparation |Yield Enhancement |

|Failure Analysis Process |Optical Techniques |SPM Techniques ||

AND… Any Other Topics Related to Testing and/or Electronics Failure Analysis


*For topic descriptions and information regarding abstract submission, please visit the ISTFA website at www.edfas.org/istfa.


CALL FOR PAPERS DEADLINE  April 2, 2007


vii


Take advantage of this opportunity to  participate in the PREMIERE international  event for the Microelectronics Failure  Analysis community. Submit your abstract  to be considered for inclusion in the ISTFA  2007 technical symposium.


Contents


Session 1: Advanced Techniques 1


# Session 1: Advanced Techniques 1


Near-field Scanning Microwave Probe for Rapid Detection of


Nonvisual and Parametric Defects in Cu/low-k Interconnect on


Production Wafers………………………………………………………………………….…………1


V.V. Talanov, A.R. Schwartz, Neocera, Inc. Beltsville, MD, USA


Noninvasive Acoustic Phonon Characterization of Dynamic MEMS…………………….….6


W.K. Wong, M. Palaniapan, C.L. Wong, S.R. Wang, F.E.H. Tay  National University of Singapore, Singapore;


Magnetic Current Imaging with Magnetic Tunnel Junction Sensors—


Case Study and Analysis…………………………………….……………………………………..13


B.D. Schrag, M.J. Carter, X. Liu, J.S. Hoftun, G. Xiao  Micro Magnetics, Inc., Fall River,  MA, USA


Session 2: System Level Analysis 1


Analysis and Identification of Off-Odor Compounds in Electronic


Systems……………………………………………………………………………………………..…20


M.A. Nailos1, D. Stein1, L.T. Nielsen2, A. Iwasinska2


(1) Dell, Inc., Austin, TX, USA; (2) Microanalytics, Round Rock, TX, USA


System Failure Analysis Process and Case Study……………………………………….……26


N. Konkol, Intel Corporation, Beaverton, OR, USA


Using a Unified Data Stream to Drive Failure Analysis for


Product Improvement in the Personal Computer (PC) Environment……………….………30


S. Horley1, J. Rascon2, (1) Intel Corporation, Hillsboro, OR, USA


(2) Intel Corporation, Chandler, AZ, USA


Session 3: Test and Diagnostics


Triangulating to a Defect’s Physical Coordinates


Using Multiple Supply Pad IDDQs—Test Chip Results………………………………………....36


J. Plusquellic, D. Acharyya, M. Tehranipoor, C. Patel  UMBC, Baltimore, MD, USA


Logical-to-Physical Device Navigation using


Place-and-Route Data as an Alternative to LVS..……………………………………………....46


R. Nicholson, Credence Systems Corporation, Milpatas, CA, USA


ix


Fundamental Considerations for CDM Failure in 90nm Products………………………......55


N. Wakai1, Y. Kobira1, M. Tsutsumi2, H. Egawa1


(1) Toshiba Corporation Semiconductor Company, Yokohama, Japan


(2) Toshiba Nanoanalysis Corporation, Yokohama, Japan


Session 4: Circuit Edit and Beam-Based Sample Preparation


Development of a Circuit Edit Process Scalable in


Dimension and Material……………………………………………………………………………..62


V.V. Makarov, N. Antoniou, Credence Systems Corporation, Sunnyvale, CA, USA


Quantitative Electrical Analysis of FIB Prepared Vias on


BiCMOS and CMOS090 Designs………………………………………………………………......67


B. Domenges1, P. Poirier2, (1) LAMIP, ENSICAEN-Philips, France


(2) Philips Semiconductor, France


Study on the Effect of FIB Electron Beam Assisted


Platinum Deposition on TEM Sample Analysis……………………………………………...…71


J. Hu, J. Zhou, M. Li, Q. Gao, C. Niou, K.W.T. Chien


Semiconductor Manufacturing International Corp., Shanghai, China


Experiment Study on Crystal/Amorphous Structure of


TEM Samples Prepared by FIB Milling………………………………………………………...…76


Q. Gao, M. Zhang, C. Niou, M. Li, W.T.K. Chien


Semiconductor Manufacturing International Company, Shanghai, China


Advanced Fringe Analysis Techniques in Circuit Edit…………...………………………...…79


R.K. Jain1, T. Malik1, T.R. Lundquist1, C.-C. Tsao1, W.J. Walecki2


(1) Credence Systems Corp, Sunnyvale, CA, USA


(2) Frontier, Semiconductor, San Jose, CA, USA


Session 5: Scanning Probe Microscopy


Direct Measurements of Charge in Floating Gate


Transistor Channels of Flash Memories Using


Scanning Capacitance Microscopy……………………………………………………………….86


C. De Nardi1, R. Desplats1, P. Perdu1, C. Guérin2, J.L. Gauffier3


T. B. Amundsen3, (1) CNES, French Space Agency, Toulouse, France


(2) DGA/CELAR, French Defense Department, Bruz, France


(3) LNMO, INSA Génie Physique, Toulouse, France


Development of Backside Scanning Capacitance


Microscopy Technique for Advanced SOI Microprocessors……………………….……......94


V. Narang1, P. Muthu1, J.M. Chin1, V. Lim2


(1) Device Analysis Laboratory, Singapore


(2) Institute of Microelectronics, Singapore


x


Material and Doping Contrast in Semiconductor Devices at


Nanoscale Resolution Using Scattering-Type Scanning


Near-Field Optical Microscopy………………………………………………………..………...…98


J. Wittborn1, R. Weiland1, D. Kazantsev2, A. Huber2


R. Hillenbrand2, F. Keilmann3, (1) Infineon Technologies


Munich, Germany; (2) Nano-Photonics Group, Martinsried   Germany, F. Keilmann, (3) Abteilung Molekulare


Strukturbiologie, Martinsried, Germany


Identification of Root Cause Failure in Silicon on Insulator


Body Contacted nFETs Using Scanning Capacitance


Microscopy and Scanning Spreading Resistance Microscopy………………………..…..102


J.S. McMurray, C.M. Molella,


IBM Microelectronics, Hopewell Junction, NY, USA


Session 7: Package Level Analysis 1


Intermittent Failures in High Pin Count Packaging…………………………….………...….109


R. Varma1, R. Brooks1, R. Twist1, J. Arnold1, C. Messick2


(1) Northrop Grumman Corporation, Electronic Systems, Linthicum, MD, USA


(2) Northrop Grumman Corporation, Mission Systems, Clearfield, UT, USA


Microstructure Analysis of Wafer Bump Nodule…………………………………………..….115


X. Chen, T. Ge, L. Tsou, M. Li, C. Niou, W.T. Kary Chien  SMIC Corporation, Shanghai, China


Packaging Material has Contributed to High Idd_Pd Failures in CMOS ICs………...…..118


P.M. Chi, C.G. Eng, N. Sulaiman, Avago Technologies, Penang, Malaysia


Session 8: Discretes, Passives, MEMS, and Optoelectronics


Inductive Operating Life Stress Metal Breakdown Mechanism………………………...…125


B. Gillette, Fairchild Semiconductor Corporation, Mountaintop, PA, USA


Root Cause Finding of a Diode Leakage Failure


Using Scanning Magnetic Microscopy and ToF-SIMS as Key Methods………………….132


H. Preu, W. Mack, T. Kilger, B. Seidl, J. Walter, P. Alpern, M. Kirchberger  Infineon Technologies AG, Regensburg, Germany


Temperature and Humidity Dependent Reliability Analysis of RGB LED Chips………..137


J.-X. Fu1, S. Souri1, J.S. Harris, Jr.2


(1) Exponent Failure Analysis Associates, Inc., Menlo Park, CA, USA


(2) Stanford University, Stanford, CA, USA


A Study of Low Leakage Failure Mechanism of


X7R Multiple Layer Ceramic Capacitor (MLCC)…………………………………...…………..142


Z. Wang, International Rectifier Corporation, Temecula, CA, USA


xi


A System for Electromechanical Reliability Testing of MEMS Devices…………..….…..147


S. Spinner, M. Doelle, P. Ruther, O. Paul, I. Polian, B. Becker  University of Freiburg, Freiburg, Germany


Session 9: Posters


Case Studies in Atomic Force Probe Analysis……………………………………………..…153


R. Mulder, S. Subramanian, T. Chrastecky


Freescale Semiconductor, Inc., Austin, TX, USA


FA/LIT Instrument Adjustments for Successful Analysis of


Packaged Semiconductor Devices……………………………………………………………...163


D.J.D. Sullivan, S.K. Hsiung, J. Soopikian  LSI Logic Corporation, Fremont, CA, USA


Coupling C-AFM with Nanoprobing Technique for


Further Junction Leakage Analysis…………………………………………………….……….167


C.-M. Shen, T.-C. Chuang, C.-M. Huang, S.-C. Lin, J.-F Chang


Taiwan Semiconductor Manufacture Company, Ltd., Tainan, Taiwan, ROC


Mixed-Signal Test Software Generation Process—


Open Environment, Software Engineering Methods and


Tools for Improving Quality and Productivity……………………………………………..…..172


S. Vock1, H.M. von Staudt2


(1) SEPT Europe, München, Germany


(2) Dialog Semiconductor, Kircheim/Teck, Germany


Conductive Atomic Force Microscopy Application for


Semiconductor Failure Analysis in Advanced Nanometer Process……………….……..178


K. Lin1, H. Zhang1, S.-S. Lu2


(1) United Microelectronics Corporation, Hsinchu, Taiwan, ROC


(2) National Taiwan University, Taipei, Taiwan, ROC


Laser Based Analysis on Analog Circuits with


Feedback Loops and a Case Study……………………………………………………………..182


F. Zhang, D. Maxwell, Texas Instruments, Inc., Dallas, TX, USA


A Novel Method to Inspect Deep Trench Capacitor Planar Profiles in DRAM…………..185


J.L. Lue, A. Huang, T. Wang


ProMOS Technologies, Inc., Hsinchu, Taiwan, ROC


Surface Defect Analysis by Using a Novel Backside


XTEM Sample Preparation Method……………………………………………………………..188


J.-S. Luo, L.-Y. Huang, W.-L. Gu, J.D. Russell  Inotera Memories, Inc. Taoyuan, Taiwan, ROC


xii


Application of EDS Technique for OSP Film Thickness Measurement…………………..193


P. Kongsubto, S. Kongwudthiti


Spansion Ltd., Pakkret Nonthaburi, Thailand


Applications of Transmission Electron Microscopy and


Secondary Ion Mass Spectrometry on Crystal Defect Analysis and


Electronic Characterization of Advanced 512Mb DRAM…………………………….……..196


S. Lu, E. Chen, L.-Y. Huang, J.-S. Luo, J.D. Russell   Inotera Memories, Inc., Taoyuan, Taiwan, ROC


Advanced Manual Package Pulling System for


Removing PCB Components in Preparation for


Crack Area Measurement and Disbond Type Mapping…………………………….………..202


T.R. McDonald, Intel Corporation, Hillsboro, OR, USA


Application of FIB Circuit Edit in Analysis of Memory Failure of SOI Devices..………..204


Z.G. Song, S.K. Loh, X.H. Zheng, S.P. Neo, C.K.Oh


Chartered Semiconductor Manufacturing Limited, Singapore


A Fast Inspection of Well Implantation by Using Plane-View Stain Method…..………..208


J.-C. Lin, W.-S. Wu, K.-S. Chen, J.-H. Yeh, Y.-C. Hou


United Microelectronics Corporation, Hsin-Chu, Taiwan, ROC


Microelectronic Packages (FC with Ceramic Substrates)


Solder Removal Method for Failure Analysis………….……………………………….……..214


T.I. Shih, T.H. Chen


Note on the Use of Principal Component Analysis (PCA) and


Clustering for the Analysis of Wafer Level ATPG data………………………………….…..219


K. Ramanujachar1, S. Draksharam.2


(1) Intel Corporation, Chandler, AZ, USA


(2) Texas Instruments, Stafford, TX, USA


Failure Analysis Navigation System Connecting


Hardware Analysis to Software Diagnosis……………………………………………………..221


A. Shimase1, A. Uchikado1, Y. Matsumoto1, S. Watarai1,


S. Kawanabe1, T. Suzuki1, T. Majima1, K. Hotta2, H. Terada.2


(1) Renesas Technology Corporation, Tokyo, Japan


(2) Hamamatsu Photonics, Shizuoka, Japan


Usage of SAM on Fatigue Crack of Solder Joint Induced by


Thermal Reliability Test…………………………………………………………………………...228


T.H. Chen, T.I. Shih


United Microelectronics Corporation, Hsin-chu, Taiwan, ROC


Laser Based Defect Localization for the


Failure Analysis of Advanced Product……………………………………………………..…..230


W.Y. Cheng, T.Y. Chiu, J.C. Lee, J.Y. Chiou


Taiwan Semiconductor Manufacturing Company, Hsin-chu, Taiwan, ROC


xiii


Enhanced Detection Sensitivity with


Pulsed Laser Digital Signal Integration Algorithm……………………………………….…..234


A.C.T. Quah1, J.C.H. Phang1, L.S. Koh2, S.H. Tan2, C.M. Chua2


(1) National University of Singapore, Singapore


(2) SEMICAPS Pte Ltd., Singapore


A Study of Flip-chip Open Solder Bump Failure Mechanism……………………..………..239


Z. Wang, M. Choudhry, International Rectifier Corporation, Temecula, CA, USA


Nondestructive Method for Detecting Solder Defects at the


Second Level Interconnect Using 3D X-Ray Tomography (uCT)…………………..……...243


F. Toth, G.F. Shade, Intel Corporation, Hillsboro, OR, USA


Deformation Study of Low K Dielectric after E-beam Exposure………………….………..246


X. Chen, Q. Gao, M. Li, C. Niou, W.T. Kary Chien  SMIC Corporation, Pudong, Shanghai, China


Realization of an Integrated IT System Covering the


Complete Failure Analysis Process……………………………………………………………..249


M. Grützner, Infineon Technologies AG, Munich, Germany


New Approach—Sample Preparation Techniques for


Plastic Small Outline Package (Frontside and Backside)……………………………….…..253


E. Marquez, D. Nguyen, Texas Instruments, Inc. Dallas TX, USA


The Electrical Characterization and Physical


Failure Analysis for Transistor Gate Leakage…………………………………………….…..257


T.-T. Li,C.-C. Wu, J.-H. Chuang, J.C. Lee


Taiwan Semiconductor Manufacturing Company, Ltd., Hsin-Chiu, Taiwan, ROC


Failure Analysis of Laser Blown Metal Fuse Failures in


Submicron Technology by C-AFM………………………………………………………….…..260


L.-F. Wen, C.-H. Chen, A.T. Chang


Combine Nanoprobing Technique with Difference Analysis to


Identify Nonvisual Failures…………………………………………………………………..…..264


C.-M. Shen, T.-C. Chuang, J.-F. Chang, J.-H. Chou


Taiwan Semiconductor Manufacturing Company, Ltd., Tainan, Taiwan, ROC


A Technique for Reliably Preparing Full-Length Metallographic


Cross-Sections of Integrated Circuit Bond Wires……………………………………….…..268


C. Nail, National Semiconductor Corporation, Santa Clara, CA, USA


130nm Backend Reliability Failures—Analysis to Corrective Action……………..……..273


G. Garteiz, A. Zylberman, Tower Semiconductor, Israel


xiv


Rapid Yield Learning with Effective Integration of


FMEA design for DOE on Test Chip……………………………………………………………..276


I.A.N. Goh, R. McMullan, B. Fairchild, J. Ilzhoefer  Texas Instruments, Inc., Dallas, TX, USA


Session 10: Metrology and Materials Analysis 1


Secondary Electron Potential Contrast for


Dopant Profiling of Silicon Carbide Devices……………………………………………..……279


M. Buzzo1, M. Ciappa2, W. Fichtner2


(1) Infineon Technologies, Villach, Austria


(2) Swiss Federal Institute of Technology, Zurich, Switzerland


Image Intensity Analysis for Defect Localization


Utilizing SEM BSE Imaging……………………………………………………………….………289


J. Demarest1, K. Chanda1, S. Klepeis1, B. Redder1 A. Shore1, Y. Wang1, C. Christiansen2, C. Rue3


(1) IBM, Hopewell Junction, NY, USA


(2) IBM Esses, Junction, VT, USA


(3) FEI Company, Hillsboro, OR, USA


Focused Ion Beam Grounding to Alleviate


Sample Charging for Scanning Auger Electron Spectroscopy……………..…………….293


C.F.H. Gondran, E. Morales, ATDF/SEMATECH, Austin, TX, USA


Energy Dispersive Spectrum (EDS) Study of


Copper Grid Effect on Semiconductor Failure Analysis………………………………..…..297


J. Hu, M. Li, Q. Gao, C. Niou, W.T. Kary Chien


Semiconductor Manufacturing International Corporation  PuDong New Area, Shanghai, China


Studies of Silicon Dust corrosion on Microchip


AI Bondpads and Elimination of Silicon Dust


During Wafer Sawing Process……………………………………………………………….…..300


H. Younan, Z. Siping, M. Zhiqiang, C.J. Ying


Chartered Semiconductor Manufacturing Ltd., Singapore


Session 11: Die Level Fault Isolation


Analysis of Delta Iddq Soft Failes on Pass Chips……………………………………………305


I. Österreicher1, S. Eckl1, B. Tippelt2, S. Döring2, R. Prang2, W. Werner2


(1) Infineon Technologies Dresden GmbH and Company OHG, Dresden, Germany


(2) Qimonda Dresden GmbH and Company OHG, Dresden, Germany


xv


Applications of Soft Defect Localization (SDL) on


AMD Advanced SOI Microprocessors……………………………………………………...…..311


Y.-X. Seah, M. Palaniappan, J.M. Chin


Advanced Micro Devices  Pte., Ltd., Singapore


Active Voltage Contrast for Failure Localization in Test Structures………..…………….316


R. Rosenkranz1, S. Döring1, W. Werner1, L. Bartholomäus1, S. Eckl2


(1) Qimonda Dresden GmbH and Company, Dresden, Germany


(2) Infineon Technologies Dresden GmbH and Company OHG, Dresden, Germany


Floating Substrate Passive Voltage Contrast (FSPVC)……………………...………………321


M.W. Jenkins, P. Tangyunyong, E.I. Cole, Jr.


J.M. Soden, J.A. Walraven, A.A. Pimentel


Sandia National Laboratories, Albuquerque, NM, USA


Fault Identification by Use of a Simulated


Passive Voltage Contrast Reference CAD Display…………………………………….……..328


R. Fredrickson, ON Semiconductor, Gresham, OR, USA


Session 12: Metrology and Materials Analysis 2


SEM and AFM Investigation for Accurate


Measurements of 193-nm Resist Profiles…………………………………….………………..334


R. Reiche, R. Bartkowiak, M. Heller, R. Rosenkranz


Qimonda Dresden GmbH and Company OHG, Dresden, Germany


A Novel Method for Deep Trench Profile Characterization and


Process Monitoring in 90nm DRAM Technology……………………………………………..339


K.-H. Huang, W.-L. Gu, M.-D. Liu, Y.-S. Wang, J.D. Russell  Inotera Memories, Inc., Taoyuan, Taiwan, ROC


Challenges in Evaluating Thickness, Phase, and Strain in


Semiconductor Devices Using High Resolution


Transmission Electron Microscopy…………………………………………………..………..343


R. Rai, J. Conner, S. Murphy, S. Subramanian


Austin Silicon Technology Solutions, Austin, TX, USA


Techniques for Analyzing Solder Joint Properties and


Damages in FBGA Packages…………………………………………..………………………351


S. Leinert, S. Jansen, N. Martin, D. Breuer, W. Werner


Qimonda Dresden, GmbH and Company, Dresden, Germany


xvi


Session 13: Chemical and Mechanical Sample Preparation


Back Side Die Preparation for Check of Backend Related Problems……………………356


M. Huettinger1, U. Papenberg1, J. Touzel1


A. Janeiro2, R. Guedes2, C. Caldeira2, C. Ribeiro2


(1) Infineon Technologies AG, Munich, Germany


(2) Infineon Technologies AG, Mindelo, Portugal


Development of the Polishing Technique for the


Observation of the Intermetallic Compound at Solder Joint.……………………………..361


P. Kongsubto, S. Kongwudthiti, N. Santipruksawong, J. Tippayamontri  T. Promket, Y. Singsa, Spansion Ltd., Nonthaburi, Thailand


Enhancement Method to Improve the Accuracy of


Intermetallic Area Inspection on the Bonding Pad through


Chemical and Mechanical Removal Process………………………………………………….370


P. Kongsubto, S. Kongwudthiti, Y. Yousoom, R. Lochingchairit  P. Kongjaroon, Spansion Ltd., Nonthabuti, Thailand


Session 14: Advanced Techniques 2


Functional IC Analysis Through Chip Backside with


Nano Scale Resolution—E-Beam Probing in FIB Trenches to STI Level……..………...376


R. Schlangen1, R. Leihkauf1, U. Kerst1, C. Boit1, B. Krüger2


(1) Berlin University of Technology, Berlin, Germany


(2) Infineon Technologies, Munich Germany


Use of a Solid Immersion Lens for Thermal IR Imaging…………….…………………….…382


O. Breitenstein1, F.Altmann2, T. Tiediger2, D. Karg3, V. Gottschalk4,


(1) Max Planck Institute of Microstructure Physics, Halle, Germany


(2) Fraunhofer Institute for Mechanics of Materials, Halle, Germany


(3) Thermosensorik GmbH, Erlangen, Germany


(4) ELMOS Semiconductor AG, Dortmund, Germany


Indirect Electrostatic Discharge Stressing Mechanism in


VLSI Chips with Multiple Power Supply Domains……………………………..…………..389


S. Sofer1, Y. Fefer1, Y. Shapira2,


(1) Freescale Semiconductor Israel Ltd., Herzella, Israel


(2) Tel Aviv University, Ramat Aviv, Israel


Planar Deprocessing of Advanced VLSI Devices…………………………………………..393


K.S. Wills, Texas Instruments, Dallas, TX, USA


An Advanced Integrated Circuit Analysis System………………………………..………..398


E. Keyes, J. Abt, Semiconductor Insights, Ottawa, Canada


xvii


Session 15: Yield Analysis


Translating Yield Learning Into Manufacturable Designs…………………………..…..…402


V. Chowdhury, I. Rahim, A. Yu, G. Venkitachalam  Altera Corporation, San Jose, CA, USA


Improving Yield Using Scan and DFT Based Analysis for


High Performance PowerPC© Microprocessor………………………………………………..407


R. Talacka1, N. Tendolkar1, C. Paquette2


(1) Freescale Semiconductor, Austin, TX, USA


(2) AMD, Austin, TX, USA


Yield Learning with Layout-aware Advanced Scan Diagnosis………………………….….412


J. Mekkoth1, M. Krishna1, J. Qian1, W. Hsu2, C.-H, Chen2


Y.-S. Chen2, N. Tamarapalli3, W.-T. Cheng3, J. Tofte3, M. Keim3


(1) Cisco Systems, Inc., San Jose, CA, USA


(2) Taiwan Semiconductor Manufacturing Company, Hsin-Chiu, Taiwan, ROC


(3) Mentor Graphics Corporation, Wilsonville, OR, USA


Defect Localization Technique for Logic Circuits in


Sub 90nm SOI Microprocessors……………………………………………………………..…..419


T. Kane, M.P. Tenney, J. Bruley, S. Boettcher,  IBM STG Division, Hopewell Junction, NY, USA


NBTI Reliability of Strained SOI MOSFETs…………………………………………...………..423


G. Thareja1, J. Lee1, A.V.-Y. Thean2, V. Vartanian2, B.-Y. Nguyen2


(1) University of Texas, Austin, TX, USA


(2) Freescale Semiconductor Inc., Austin, TX, USA


Session 16: Optical Fault Isolation


Soft Defect Localization Technique for


Design and Debug on DRAM Devices………………………………………….……………….426


M. Versen1, D. Diaconescu2, J. Touzel2


(1) Qimonda AG, Neubiberg, Germany


(2) Infineon AG, München, Germany


Application of LADA for Post-Silicon Test Content and


Diagnostic Tool Validation……………………………………………………………..…………431


C.L. Kong, E.P. Castro, Intel Corporation, Santa Clara, CA, USA


Voltage Noise and Jitter Measurement Using Time-Resolved Emission…………….…..438


S. Kasapi, G.L. Woods, Credence Systems Corporation, Milipitas, CA, USA


The Techniques for Short Failure Isolation on Advanced Technology…………………..444


H.N. Lin, C.H. Wang, K.L. Lin, W.S. Yang, C.J. Chen


Taiwan Semiconductor Manufacturing Company, Ltd., Taiwan


xviii


Session 17: Anayltical Process


Buttons and Threads—Tailoring Defect Analysis……………………………………………449


C.F.H. Gondran1, D.F. Paul2, S.K. Das3, B.J. Foran4, M.H. Clark4


(1) ATDF/SEMATECH, Austin, TX, USA


(2) Physical Electronics, Inc. Chanhassen, MN, USA


(3) IBM/SEMATECH, Austin, TX, USA


(4) ATDF/SEMATECH, Austin, TX, USA


Marginal Deviation of Thermal Budget Brings


Shallow Junction Formation Failure Forth Study………………………………...…………..453


T.-C. Chuang, C.M. Shen, J.H. Chou


Taiwan Semiconductor Manufacture Company, Ltd., Taiwan


Metal Slice Defect Induced Package Level Reliability Failure……………………………...457


M. Zhang, S. Liao, S. Liang, R. Lou, R. Chen, C. Niou, W.T. Kary Chien  Semiconductor Manufacturing International Company, Shanghai, China


Vanishing TiN ARC Coating as an Indicator of


EOS in Aluminum Top Metal Lines………………………………………………………….…..461


T.J. Barbieri1, J. Wang1, M. Kottke1, D. Theodore1, R. Wetz2


(1) Freescale Semiconductor, Inc., Tempe, AZ, USA


(2) Tyco Health Care/Valleylab, Boulder, CO, USA


Session 18: Package Level Analysis 2


Accelerated Corrosion of Printed Circuit Boards


Due to High Levels of Reduced Sulfur Gasses in


Industrial Environments…………………………………………………………….………….….469


P. Mazurkiewicz, Hewlett-Packard Company, Fort Collins, CO, USA


Fine MCP Decapsulation Technology Development………………………………………....474


J. Zhou, W. Zheng, T. Lee, Samsung Semiconductor China R&D Co., Ltd. Jiangsu Province, P.R. China


Correlation Study of Delamination Gap Detection Capability of


SAM and Cross Section/SEM Analysis……………………………………….……………..….480


T.S. Leng1, J.C.P. McKeon2, H.S. Jang3


(1)Texas Instruments, Kuala, Malaysia


(2) Sonix Incorporated, Springfield, VA, USA


(3) Sonix Incorporated, Seoul, Korea


Measurement Techniques for Thermally Induced Warpage to


Predict Ball-Grid Array Package-on-Package Solder Compatibility………..…………....488


T.B. Davis, M. Morrison, T. Krawzak, J. Reeder, T. Jiang  Micron Technology, Inc., Boise, ID, USA


xix


Session 19: Nanotechnology and Nanoprobing


Atomic Force Probe Kelvin Measurements of


Large MOSFET Devices at Contact Level for


Accurate Device Threshold Characteristics……………………………………………….…..497


T. Kane1, M.P. Tenney1, A. Erickson2, S. Phan2


(1) IBM STG, Fishkill, NY, USA


(2) Multiprobe, Inc., Santa Barbara, CA, USA


Atomic Force Probe Analysis of Nonvisible Defects in


Sub-100nm CMOS Technologies…………………………………………………………...……503


Freescale, Semiconductor, Inc., Austin, TX, USA


90nm Technology SRAM Soft Fail Analysis


Using Nanoprobing and Junction Stain TEM………………………………………………….512


G. Zimmermann1, S. Mueller2,


(1) Infineon Technologies Taiwan, Ltd., Hsin-Chiu, Taiwan, ROC


(2) Infineon Technologies AG, Munich, Germany


Nanoprobing Application on Characterization of


6T-SRAM Single Bit Failures with Different Gox Breakdown Defect……………...………517


C.-P. Lin, C.-H. Tang, C.-H Wu, C.-C. Ting


Taiwan Semiconductor Manufacturing Company, Ltd., Hsin-Chiu, Taiwan


In Situ Electron Microscopy Study of


Current-Induced Failure of Carbon Nanofibers………………………………….…………....521


M. Suzuki1, Y. Ominami1, Q. Ngo1, C.Y. Yang1,


K. Mcilwrath2, K. Jarausch2, A.M. Cassell3, J. Li3


(1) Santa Clara University, Santa Clara, CA, USA


(2) Hitachi High Technologies America, Inc., Pleasanton, CA, USA


(3) NASA Ames Research Center, Moffett Field, CA, USA


xx


Near-field scanning microwave probe for rapid detection of non-visual and  parametric defects in Cu/low-k interconnect on production wafers


Vladimir V. Talanov and Andrew R. Schwartz


Neocera, Inc., 10000 Virginia Manor Road, Beltsville, MD 20705, USA  schwartz@neocera.com


Abstract


We demonstrate the use of a near-field scanned microwave  probe (NSMP) for failure analysis (FA) of parametric defects  in Cu/low-k interconnect that leave no physical remnant (sometimes referred to as “non-visual defects”). This  technique is rapid, quantitative, non-contact, and provides  direct electrical measurements.


Introduction


It is widely known that low-k dielectrics, and particularly  porous low-k materials, are susceptible to electrical damage  during the integration process and thus it is necessary to  monitor their electrical properties to better understand the  effects of integration. Until now, there has been no metrology  to monitor low-k damage electrically during integration. In  response to this need, we have developed a methodology  based on a near-field scanning microwave probe and  demonstrated its use for direct non-contact electrical  characterization of low-k dielectric constant and damage after  deposition, during trench/via processing, and after  metallization. These measurements can be used for process  development and for yield enhancement through detection of  parametric defects that cannot be visualized as physical  defects using today’s detection techniques.


Apparatus description


In our near-field approach the spatial resolution is governed by  the probe geometry rather than the wavelength of the radiation  utilized [1]. Therefore, even at microwave frequencies with  wavelengths on the order of centimeters, such a probe can  achieve spatial resolution down to sub-microns. Our tool and  the method for quantitative measurements of dielectric  constant of blanket low-k films have been described in detail  elsewhere [2, 3]. The probe is formed by a parallel strip  transmission line resonator tapered down to ~10 micron tip  size and mounted inside a metallic sheath with the taper  protruding out via an opening in the sheath wall (Fig.1). It  operates in the balanced odd mode with a resonant frequency  F~4 GHz. An electrical near-field similar to the fringe field of


a parallel plate capacitor is formed at the electrically open tip. The tip-sample distance h is controlled using a shear-force (SF) method. Since the probe size is much less than the  radiation wavelength, a lumped element scheme can be used  to describe the probe-sample interaction.  When a dielectric  film on a metallic substrate is brought in close proximity to the  tip, the tip capacitance Ct=(2/Cg+2/Cf)−1 terminating the  resonator increases, and consequently the probe resonant  frequency F decreases by an amount dependent on the film  dielectric constant. For a low-loss sample the relationship  between the change in Ct and the relative shift in the probe  resonant frequency, ∆F, is:


F F


FZ


Ct


∆


−


=


0


2


1


(1)


where Z0≈100Ω is the transmission line characteristic  impedance, and FZ0Ct<<1. For a typical frequency  measurement precision of ~1 kHz, Eq. (1) yields sensitivity to


parallel strip


resonator resonant


frequency, FF


circulatorH


probe tip


coupling


loopI VCO


~4 GHz frequency


counter


wafer


sheath


microwave diode


xy-stage


⇒


frequencytracking  electronics


coax cable


h


k


丰丰Cg


Cf


tfilm


Z0


Al


quartz


Si, Cu


film dielectric  constant, k


口⇒


low-k film


Figure 1: Apparatus schematic showing the probe and  electronics. The inset shows the lumped element scheme for  the tip capacitance in the case of a low-k film on a metallic  substrate (e.g. Cu, low resistivity Si).


## Near-field scanning microwave probe for rapid detection of non-visual and parametric defects in Cu/low- k interconnect on production wafers


Proceedings of the 32nd International Symposium for Testing and Failure Analysis November 12-16, 2006, Renaissance Austin Hotel, Austin, Texas, USA


Copyright© 2006 ASM International®


Ct down to 10-18 F. If a parallel plate capacitor is formed, for  example, by a typical 0.4-µm-thick low-k film with k~2, such  sensitivity allows for a capacitor with area less than 10 µm2 to  achieve ~0.1% precision in k-value measurement, as desired  by today’s advanced process control. Note, that the area  required by Hg-probe or MIS-cap methods in this case is ~1  mm2 given their capacitance sensitivity of ~0.1 pF.


The NSMP is calibrated using a set of variable thickness SiO2  films thermally grown on low resistivity Si (which effectively  appears as a perfect conductor film backing for our probe). Using the approach developed in [3] the measured frequency  is converted into film dielectric constant with precision  1σ<0.3% and accuracy better than ±2%. Wafers up to 300mm  in diameter are held by a vacuum chuck and can be scanned  beneath the probe by a 350 by 350 mm travel xy-stage. The  apparatus is equipped with optical navigation and sits on a  vibration-isolated platform inside an environmental chamber.


Measurement after deposition


The test structure to measure the as-deposited dielectric  constant is a ~60×60 µm2 open area formed by a low-k film (with or without etch-stop, hard-mask and capping layers) with  a Cu backing, which can be either continuous or patterned as


9


will be discussed below. This test key is compatible with


n


damascene processing and can be repeated throughout the


e a


entire interconnect stack. Such a test key fits easily into an 80-µm-wide scribe line.


e


To confirm that the measurement is unaffected by the finite


test key size, we performed a line-scan across the edge of a


人


60×60 µm2 Cu pad buried under a 414-nm-thick low-k film (the film thickness was measured by ellipsometry at the same  site). The structure was located on a patterned 300 mm wafer  and surrounded by a variety of other test structures. The kvalue was extracted as a function of lateral position x  normalized by the tip size D. Outside of a transition range ~1.5×D wide the measured k-value exhibits no change (within  the measurement precision). Over the patch we obtained  k=3.21±0.01, which is in excellent agreement with the


nominal value of 3.20. Assuming the worst possible case of


the entire transition occurring above the patch, the minimal


000000o8


size of the test key needed to accommodate the two edge  transitions and a single sampling spot size ~D is


。0∞a。608 9


2×(1.5×D)+D=4×D≈40 µm.


co8


DDDDD△


△△公To further demonstrate the capability of the NSMP for in-line  monitoring of the deviation of the dielectric constant of low-k  materials across a 300 mm wafer we measured a number of  the above test keys located on three patterned wafers with  USG, low-k (LK) and ultra low-k (ULK) films. Two test keys  on nine die per wafer were mapped according to the scheme in  Fig. 2a and the etch-stop layer contribution was removed. For  all wafers we obtained k-values close to the nominal ones (Fig. 2b). The observed variations are likely due to the fact that the  large area of Cu backing the dielectric film affects the low-k  film morphology.


Since continuous Cu is not compatible with CMP technology  due to the copper loading issues, we investigated if a Cu grid  could be used in place of the continuous backing. Figure 3  shows the k-values measured with the probe centered over a  set of 60×60 µm2 test keys consisting of the low-k film over a  backing now formed by parallel Cu lines of variable pitch and  pattern density (these are actually OCD test keys, each with a  fixed pitch and density). The same LK wafer as above was  used for these measurements. One can see that for pattern  density of 50% (or greater) and nominal pitch less than ~0.25 µm the measured k-value is independent of pitch and has the  same value (3.141±0.005) as that obtained with the continuous  Cu pad backing (3.14). Note that for density greater than 50% a larger pitch is probably acceptable, but such test keys were


(b)


(a)


1 2 3 4 5 6 7 8 9


2.0


2.5


3.0


or


。3.5


4.0


心4


N


4.5


5.0


Dielectric constant


4


ULK LK USG


Die #


Figure 2: (a) Scheme of 9 die measured on 300 mm wafer.


(b) Results for mapping of k-value on three wafers (2 sites  per die) with USG, LK, and ULK dielectrics. The mean  values obtained over each wafer 4.12, 3.14, 2.57 are in good  agreement with pristine k-values of 4.20, 3.20 and 2.50, respectively.


low-k


S


LK


Cu


0.1 0.2 0.3 0.4 0.5 0.6


y


2.7 e2.8


2.9 w3.0 s3.1 p3.2


Cu backing pitch, µm


Backing Cu density:


50%


33%


20%


60µm


a


NCu


probe


60 µm


Figure 3: (a) Optical image of OCD test keys formed by 414-nm-thick LK film backed by patterned Cu. (b) Low-k film  dielectric constant “as measured” near the center over the  above test keys on die #5 as a function of the Cu backing  pitch at three Cu pattern densities. Etch-stop layers are not  shown for clarity in the sketch.


not available on the wafer under study. For pitches >0.3 µm  and Cu density <50% the “as measured” k-value appears lower  than the nominal because of reduced film geometrical  capacitance (see. Fig. 1) as compared to the case of continuous  backing. Thus, a grid backing with pitch much smaller than  the probe size and ≥50% pattern density appears as a perfect  conductor to the probe and can be used in conjunction with the  existing calibration method [3]. This also makes the result  independent of inevitable statistical variations in the grid  pattern. We also observed that the patterned Cu backing  provides better site-to-site repeatability, by about a factor of  three, than the continuous one, likely due to improved Cu  morphology.


Finally, it is important to note that because the transmission  line probe used includes two electrodes, there is no need for


ys


either type of Cu backing, the continuous or patterned, to be


xW


grounded, which enables measurements at all levels of the  interconnect structure.


Measurement during trench/via processing


This technique can also be used to electrically characterize  sidewall damage in patterned low-k dielectric films before  metallization. Analogous to the blanket film measurements  described above, the measurement is made on uniform  trenches etched into a low-k film backed by Cu or a Cu grid (Fig. 4 a).


To demonstrate the ability of this technique to detect damage, we processed two porous methylsilsesquioxane (MSQ) films (pristine k=2.20) on 300 mm Si wafers. Each film stack  consisted of a 50 nm SiC etch stop, 200 nm MSQ, and 75 nm  SiC cap, all on top of Cu (see Fig. 4c). Both films were etched  using a standard test reticle with various test vehicles and then  ashed using two different standard resist removal processes  which are known to cause different amounts of damage to the  MSQ material used. Wafer A was exposed to a low damage  ash while Wafer B was processed using conditions known to  cause more extensive damage to the MSQ film.


Each wafer had various sets of uniform etched trenches  intended for electrical comb capacitor measurements. Before  metallization, these test keys provide ideal test vehicles for our  technique. On each of the two wafers, dielectric constant  measurements were performed on a set of four test keys, all  with 0.125 µm linewidths (trench widths) and spacing between  the trenches varying from 0.175 to 0.4 µm. The “as measured” k-values for the test keys on both wafers are shown in Fig. 5. As discussed above, this kap depends on the k-values of the  films in the stack, including any contributions from damage, as well as the geometry of the structure including the air (k=1)


0.2 0.3 0.4


2.00


2.25 so2.50


2.75


3.00


td=14nm


td=34nm


Wafer A


Wafer B


Space (µm)


Figure 6:  Extracted k-values for the MSQ films using the  data in Fig. 5 and the model in Fig.42. The solid lines are  fits to the data as described in the text, from which the  thicknesses of the sidewall damage layers are extracted.


0.2


0.3


0.4


2.21


2.3


2.4


2.6


oT


。


Figure 5:  kap as a function of nominal spacing between  trenches. All structures had a nominal 0.125µm trench  width.


tip electrode, Al


trenchMSQ


SiC=


SiCHI


8kd


td


kmeas


ts


SiO2


点


pattern


sidewall  damage


film


ω、x


Q


(c) ∅(d)


Figure 4:  (a) 3D sketch of the probe tip above a patterned  low-k stack of the total thickness ts; typical tip size ~10 µm, tip-sample distance ~80 nm; (b) 3D sketch illustrating a  concept for the apparent dielectric constant kap; (c) Lumped  element scheme for the capacitance; (d) Lumped element  scheme for the sidewall damage contribution


contribution from the trenches (see Fig. 4c). For example, the  increase in kap for larger space is due primarily to the increase  in the fractional volume of material because the air-filled  trench width is fixed.


It is clear in Fig. 5 that Wafer B has suffered significantly  more damage than Wafer A. To quantify the result, we can use  the simple lumped element capacitor model shown in Fig. 4c  to extract effective k-values for the remaining MSQ dielectric  from the measured data (see Fig. 6). Again we see  significantly higher k-values for Wafer B, indicative of more  extensive damage, as well as the expected increase in k-value  for smaller spacing between trenches. Assuming that the  damage is limited primarily to the sidewalls of the trenches, we can build a simple model for the value of kMSQ in terms of  the thickness (td) and k-value (kd) of the damaged layer, as  shown in Fig. 4d. From this model we obtain the following  expression for kMSQ:


t


pristine


d


MSQ


)


(


2 −


+


where kpristine=2.2 is the undamaged k-value for the MSQ film. The fits of this model to the two data sets is shown by the  solid lines on Fig. 6, where the fitting parameter is the product  td·kd. If we assume that the damaged material on the sidewalls  has a k-value comparable to SiO2 (i.e., kd=4.2), then we obtain  damaged layers 14 nm and 34 nm thick on Wafers A and B, respectively.


To confirm the results of the microwave dielectric constant  measurements an HF decoration technique [4] was used. The  trenches on each wafer were filled with TEOS, crosssectioned, and then dipped in dilute HF. The SEM images for  the 0.125/0.175 structure are shown in Fig. 7. Because the  damaged dielectric material is selectively etched by the HF, the dark open regions seen on the image of Wafer B are  evidence of extensive damage on this wafer, in qualitative  agreement with the microwave results. Minimal sidewall  damage is seen on Wafer A.


Measurement after metallization


Finally, this technique can also be used to perform non-contact  capacitance measurements on miniature test keys after  metallization. The NSMP can precisely measure interline  capacitances on the order of one femto-Farad and therefore the


test keys can be orders of magnitude smaller (i.e. ~10×20 µm2) than traditional combs used in e-test. This is advantageous  because they take up significantly less real estate on the wafer  and do not suffer from the statistical pattern variations and  large fringe capacitances that plague comb capacitors. In  addition, the non-contact nature of the NSMP means that the  measurement is done without touching the wafer. By  measuring only two simple “open” and “short” test keys the  NSMP can be calibrated for quantitative interline capacitance  measurements.


Figure 8 shows the developed test key geometry. It is formed  by two interconnect wires of geometry under test with the net  interline capacitance between them ~ few femtoFarad. Each  wire is connected to the coupling pad. The probe electrodes  are aligned over the pads making the probe to capacitively  couple to the test key because of the microwave operating  frequency. Thus, the tip reactance terminating the probe is  1/iωCtot with the total capacitance seen by the probe given by:


IL


PG


PP


C


tot


5.0 1


(2)


Here


1 2


1 )


− +


is the tip-to-pad coupling


capacitance (generally, CC1≠CC2 due to geometry  imperfections), CPP is the pad-to-pad parasitic capacitance, CPG is the pad-to-ground parasitic capacitance, and CIL is the  total interline capacitance to be determined.  Generally, the tip  geometry and the tip-to-sample separation are unknown. Therefore, in order to perform quantitative measurements of  CIL a calibration for the unknown CC, CPP and CPG values is  required.  We propose to employ the approach similar to  conventional low frequency capacitance measurements using  the “short” and “open” calibration keys shown in Fig.8. The  tip capacitance for the “short” calibration key is:


sh C


C =                                                            (3) The tip capacitance for the “open” calibration key is:


op


5


0 1


(4)


Eqs. (2) – (4) yield for CIL:


( )( )( )totshshoptotopsh


(5)


CIL~0.5-5 fF


SiC


SiC Cu


C A TDO 20


200


pads


Figure 7:  SEM x-section images for 0.125/0.175 structure   on each wafer.


L


“short” “open”


Figure 8: Schematic drawing of capacitance test key along  with “short” and “open” calibration standards. L~20 µm.


Finally, from Eqs. (1) and (5), the following expression for the  total interline capacitance CIL is obtained:


( ) ( )( )( )totshshoptotop


sh


F


Z





 ∆


α2


Root Cause Isolation


The magnetic scanning results and associated optical image  overlays had identified clear shorts in the die.  The most  obvious current path fault was imaged between the VBAT1  and the VLDO traces.  These results also indicated a diffusion  of current into the digital section of the die, which was likely  the result of either multiple shorts or had been caused by some  global problem in fabrication or processing.


To verify the current mapping results the faulty ASIC was  imaged using scanning electron microscopy (SEM). Highmagnification SEM images clearly showed metal whiskers in  the VBAT1 to VLDO shorting area indicated by the current  mapping.  One such image is shown in Figure 6.  However, the current path imaged with the CS1000, which showed  shorting between metal layers, could not be directly isolated


10kuX6,0002xm000020 24 SEI


using the SEM without delayering the die. Further SEM  images showed seemingly random metal whiskers throughout  the die. The current leakage through the digital section was  explained by the very dense network of interconnects this


section being riddled with metal to metal shorts. Using the  SEM, it was also noted that the observed track spacing  between heavy metal traces was in violation of the design  rules. The initial assumption of a design rule violation was  thus corroborated.  After consultation with the vendor, it was  discovered that the vendor had accidentally disabled the  specified track spacing rules during layout.


Figure 5.  The overlaid full-die current density map shows the path of current through the die.


Discussion: Magnetic Tunnel Junction Sensors


Magnetic tunnel junction devices are thin film multilayer  structures which were first experimentally realized in 1995.  The core of a magnetic tunnel junction device is a tri-layer  consisting of two magnetic films (electrodes) separated by an  ultra-thin insulating layer.  When a voltage is applied across  this tri-layer, current can only traverse the structure via  quantum mechanical tunneling.  Due to the properties of the  tunneling process, the resulting device has an electrical  resistance which becomes dependent on the relative magnetic  orientations of the two electrode layers.  The performance on  an MTJ device is often quantified by using the percentage  change in resistance between the high-resistance and lowresistance states.  This quantity is called the magnetoresistance


Figure 6.  One of several SEM micrographs showing metal  whiskers on the die.  In this image, two whiskers are clearly  seen near the center of the image.


of the device.  Current MTJ sensors, such as the one used in  the above case study, can have magnetoresistance ratios  exceeding 200%, which allows them to easily beat the  sensitivity of the more traditional giant magnetoresistance (GMR) or anisotropic magnetoresistance (AMR) sensors, which have magnetoresistances of 15-20% and 2-3%, respectively.


In order to translate this superior behavior into a useful  device, several steps are taken.  First of all, one of the two  electrodes generally has its magnetization “pinned”.  This is  accomplished by a phenomenon called exchange bias which  occurs when an antiferromagnetic material is deposited  adjacent to this electrode.  This layer is typically called the “pinned layer” of the structure and its magnetization remains  fixed even in the presence of external fields of 500-1000 G or  more.  When the pinned layer’s magnetization is fixed in a  particular direction, the device’s properties become suitable  for use as a single bit of magnetic memory (this is the basis for  most of the new magnetic random access memory – or


MRAM– technologies).  If the pinned layer’s magnetization is  fixed in the perpendicular direction, the behavior of the device  becomes linear, making it an excellent candidate for use as a


Gold


low-field magnetic sensor. [5]


Buffer layer Free layer


-Ta


V.


In order to create MTJ sensors with high spatial resolution, the


Insulating barrier *


-CoFeBSiO2。<


MTJ film is patterned to microscopic dimensions using normal


Synthetic pinned layer


CoFeB


lithographic methods.  In addition, the sensor’s resistanceExchange bias layer<IrMn


versus-field response has been linearized.  The details of all of  these processes can be found elsewhere.  In addition, several


Buffer layerTa


additional layers of material are added to the above structure


for a variety of reasons.  These include a "seed layer" deposited below the electrodes to promote smooth and  epitaxial crystal growth, buffer layers above and below the  structure to protect from physical damage, and a layer of gold  so that the devices can be packaged using wire bonding.  Figure 7 shows the full layer structure of the MTJ sensors  used in this work.


Figure 7.  Schematic of the layer structure of the magnetic tunnel junction sensor device used for this study.  The two electrodes are CoFeB, a material chosen for its favorable spin polarization, and the insulating barrier is MgO, which is key to realizing large magnetoresistance ratios.


Analysis: Comparison of Sensor Technologies


Three types of sensors have been reported as suitable for the  purposes of magnetic current imaging:  superconducting  quantum interference device (SQUID) sensors [1,2], giant  magnetoresistive (GMR) sensors [3,4,6], and magnetic tunnel  junction (MTJ) sensors [3,5].  With magnetic current imaging, as with many other fault isolation techniques, sensitivity and  spatial resolution are two of the most important figures of  merit.  In the following discussion, we will make direct  comparisons between the performance of each type of sensor  on the basis of sensitivity, spatial resolution, form factor, and  other relevant parameters.


Magnetic and Current Density Sensitivity


The magnetic sensors used for magnetic current imaging  techniques have sensitivities which are specified using units of  magnetic field.  In general, magnetic sensitivity (SM) is


10-4


frequency dependent and the sensitivity at a certain frequency  is specified using units of nT/Hz1/2.  However, with regards to  semiconductor applications, the most relevant quantity is  actually the minimum detectable current (SI, which would be


z1/2)y (T/Hitivitld Senstic FieMagne可


specified using units of nA/Hz1/2).  Both of these related  quantities are also frequency-dependent, and the latter is also  distance-dependent.  The values of magnetic sensitivity SM are


古


given for all three types of sensors, for frequencies from 1 to  50000 Hz, in Figure 8.  In this figure, GMR and MTJ data are


GMR


measured, while the SQUID numbers have been taken from


MTJ古--SQUID2


previously published data [1].  The GMR sensor used for this


*--**


study is a commercially-available device representative of  those used for magnetic current imaging, while the MTJ  sensor was a typical unit fabricated by Micro Magnetics.  It


10-1210010102103104105


should be noted that the magnetic field sensitivity of MTJ


Frequency (Hz)


sensors further improves by an additional factor of 3-6 at  higher frequencies, while GMR and SQUID sensors have  already approached their white noise-limited sensitivity floor  by 50 kHz.  Because the amount of magnetic field created by a  given


amount


Figure 8.  Magnetic field sensitivity data as a function of  frequency for the three magnetic sensor technologies which  have been used for magnetic current imaging.


of current is dependent both on its geometry and on how far  away it is (and in some cases, on the geometry of the sensor), translating magnetic field sensitivity into current sensitivity  requires some assumptions.  Assuming the currents being  imaged can be approximated by relatively long current paths, the current sensitivity is simply proportional to the magnetic  sensitivity multiplied by the sensor-to-current distance z:


z


M


I


/


0μ


π


(Because a smaller SI indicates a better sensitivity, a minimal  distance between sensor and current leads to better  sensitivity).  The distance between the sensor and the current


(z) can be expressed as the sum of two terms: 1) the sensordependent distance (dS) between the sensor active area and the  physical bottom of the sensor, and 2) the sample-dependent  distance (dc) between the surface of the sample and the current  density to be imaged.  The latter of the above terms is  independent of the choice of magnetic sensor, so for the  purposes of comparison, we will focus on only the first term.  Figure 9 compares the current sensitivity, evaluated at 10000  Hz, for all three types of sensors.


Because the definitions of spatial resolution and sensitivity  above both depend on the sample-dependent distance between  the surface of the device and the actual current flow (denoted  dc), Figure 9 plots the current sensitivity as a function of this  parameter.  This figure covers the full range of dc values  expected for different types of samples.  For example, a frontside structure where the current is very close to the surface of  the sample might have dc = 1 µm.  A front-side device with  many intervening metal layers or a thick passivation would be  in the neighborhood of dc = 10 µm.  Finally, a thinned flipchip might feature dc = 80-150 µm while imaging a package  would likely result in a value of dc = 200-1000 µm.  It is  important to note that these values assume that the sensor  probe can be brought very close to the sample surface.  If this


is not possible (i.e. physical obstructions such as wirebonds  preventing the sensor from approaching), the effective value  of dc will be larger.


Figure 9.  Effective current resolution for each type of sensor


Current depth -- d (um)


top metalfront-side


flip-chippackage


levellower levels


12


.....GMR支-- SQUID-MTJ


ensitivity (uA/Hz2)Effective current s


古可


司古


MTJ SQUID


10-310-1


100


101102103


101


Current depth -- d(um)


10-1100


101102


103


to


Effective spatial resolution (um)a


.GMR


古司 2


104


in units of μA/Hz1/2, evaluated at 10000 Hz.  Data are  presented as a function of the sample-dependent distance  between the sample surface and the current to be imaged.


Figure 10.  Effective figure-of-merit for sensor spatial  resolution as a function of the sample-dependent distance  between the sample surface and the current to be imaged.


Spatial Resolution


Spatial resolution in magnetic current imaging is even more  difficult to cleanly define.  It can be defined as the minimum  spacing between two parallel current paths for which they can  still be individually resolved, or as the precision with which  the position of a current path can be specified.  Or, alternatively, it can be defined as size of the smallest defect of  a given type which can be located from the current density  map.  While no single definition of spatial resolution can fully  describe all situations, it is the case that the spatial resolution  of the technique, by most definitions, will be dependent on the  distance between the sensor and the current path, and in some  cases on the geometry (active area) of the sensor itself.  Quantifying this, one good figure-of-merit for the spatial  resolution (ds) of a given sensor is


w


z +


where z is (again) the sensor-to-current distance and w is the  lateral dimension of the sensor’s active area.  The actual  spatial resolution of the technique is generally equal to some  constant multiplied by the above expression, where the  constant depends on the definition of resolution which is used.  However, for the purposes of comparing sensors, the above  expression is quite useful.


Figure 10 shows the overall figure-of-merit for spatial  resolution for both GMR and MTJ sensors for each of these  cases, again presented as a function of the sample-dependent  current depth dc.  This figure shows that for samples with deep  currents (packages, unpolished flip-chips) the spatial


Table I.  Comparison of key parameters for the three types of sensors.  Current sensitivity values assume dc = 1 µm.  SQUID sensor  footprint is estimated from [6].


|Sensor Type|Field|Current Sensitivity @10 kHz, dc=1μm|Current Sensitivity @white- noise|Intrinsic Spatial Resolution|Sensor Geometry|Sensor|
|---|---|---|---|---|---|---|

|Sensor Type|Sensitivity|Current Sensitivity @10 kHz, dc=1μm|Current Sensitivity @white- noise|Intrinsic Spatial Resolution|Sensor Geometry|Footprint|

|Sensor Type|@10 kHz|Current Sensitivity @10 kHz, dc=1μm|Current Sensitivity @white- noise|Intrinsic Spatial Resolution|Sensor Geometry|Area|

||(nT/Hz1/2)|(uA/Hz1/2)|(uA/Hz1/2)|0.5ds(μm)||(mm2)|

|GMR|560|3.6|2.6|0.3|Horizontal cantilever|1.25|

|MTJ|4.2|0.09|0.02|3.8|Tapered vertical probe|0.045|

|SQUID|0.035|0.009|0.009|53|Vertical cylinder|3.14|

resolution of all sensors approaches the same value, while for  currents within ~30 μm of the surface, there is a sizable  advantage for GMR and MTJ sensors in terms of spatial  resolution.


Sensor Geometry and Footprint


Another consideration important in selecting a sensor is its  footprint and physical orientation.  Each of the three sensor  technologies has a different geometry and footprint, which  may in some cases restrict their use in some types of samples, particularly those with recessed surfaces, those requiring  powering by microprobes, or samples with wire bonds in close  proximity to the region of interest.  Figure 11 shows a  comparison of sensor form factors and footprints for the three  types of sensors.


Based on the most recent published work, the SQUID sensor  used for magnetic current imaging [6] is a tapered cone which


comes to a circular footprint which is more than 1.5 mm  across.  Because a very thin window separates the cryogenic  SQUID sensor from the room-temperature sample, these  sensors can only be safely utilized in non-contact mode.  GMR sensors have a rectangular footprint of 1.25 x 1.0 mm, and must be scanned in contact with the sample in order to  realize their primary advantage of high spatial resolution.  However, GMR sensors come on a cantilever which extends  almost horizontally, making accessing some devices more  difficult.  MTJ sensors have a vertical probe geometry, with a  thin probe that tapers at a 45° angle, and can be used for  contact-mode or non-contact-mode scanning.  The tapered  geometry creates a much smaller footprint of ~ 0.15 x 0.3 mm.  Because the sample used for the above case study had a total  area between wire bonds of just over 1 mm2, the MTJ sensor  was the only one which would have been suitable for this  work.


Discussion


(side view)


(relative footprint)


A full summary of the various parameters of interest are listed


1mm


for each sensor in Table I.


From Figures 9 and 10, it is clear that the best choice of  sensors is highly dependent on how close the sensor’s active  area can be brought with respect to the currents to be imaged


SQUID


(dc).  For samples with dc < 20 μm, the MTJ and GMR sensors  offer big advantages in terms of spatial resolution, and for  very small values of dc, the current sensitivity of these sensors  actually makes significant gains versus the SQUID (with the  MTJ’s current sensitivity making significant gains versus that


MTJ


of the SQUID for dc ~ 1 μm).  However, for samples with dc > 100 μm, the SQUID’s higher sensitivity is the deciding factor, as the spatial resolution of the three sensors begins to  approach the same sample-limited value in this case.  One  interesting conclusion that can be made is that only for very  small values of dc does the high spatial resolution of GMR  devices give them a significant advantage over MTJ sensors,


Figure 11.  Comparison of the three types of sensors in  terms of geometry (left) and footprint (right).


which have a much higher current sensitivity over the full  range of dc values.


Finally we note that MTJ sensors have noise characteristics  dependent on the size of the active area of the sensor.  The  limiting noise at Hz-kHz frequencies, which is 1/f in nature (see Figure 8), scales as the inverse of the square-root of the  sensor volume.  This allows the spatial resolution of an MTJ  sensor to be traded-off for increased sensitivity, by increasing  the lithographically-defined size of the sensor element.  While  similar relationships between sensitivity and resolution hold  for SQUID and GMR sensors, neither of these sensor  technologies currently allows the user to make this type of  trade-off.  Although it has not been demonstrated, it is  estimated that increasing the size of an MTJ sensor to that of  the SQUID sensor should result in a three- to five-fold  improvement in current and field sensitivity. This would be  useful, for example, for imaging samples with deep current  paths (i.e. packages), where a small sensor volume is not  critical.


References


1.  S. Chatraphorn, E. F. Fleet, F. C. Wellstood, L. A. Knauss, and T. M. Eiles, Scanning SQUID microscopy of integrated  circuits, Appl. Phys. Lett., 76, 2304 (2000).


2. D. P. Vallett, Scanning SQUID Microscopy for Die Level  Fault Isolation, Proc. 28th Int. Symp. for Test. and Failure  Analysis (ISTFA), Nov. 2002.


3.  B. D. Schrag, M. J. Carter, X. Y. Liu, and Gang Xiao, Scanning magnetoresistive microscopy for die-level submicron  current density mapping, Proc. 29th Int. Symp. Test. and Failure Analysis (ISTFA), Nov. 2003.


4.  B. D. Schrag,  Xiaoyong Liu, J. S. Hoftun, P. L. Klinger, T. M. Levin, and D. P. Vallett, Quantitative Analysis and  Depth Measurement via Magnetic Field Imaging, EDFA  Magazine, Nov. 2005.


5.  Xiaoyong Liu, C. Ren, and Gang Xiao, Magnetic tunnel  junction sensors with hard-axis bias field, J. Appl. Phys. 92, 4722 (2002).


6.  S. I. Woods, Nesco M. Lettsome Jr., A. B. Cawthorne, L. A. Knauss, and R. H. Koch, High Resolution Current Imaging  by Direct Magnetic Field Sensing, Proc. 29th Int. Symp. Test. and Failure Analysis (ISTFA), Nov. 2003.


Analysis and Identification of Off-Odor Compounds in Electronic Systems


Mary Ann Nailos, Dan Stein, from Dell, Inc.,


Dell, Inc.  Austin, TX, USA


Lawrence T. Nielsen, Anna Iwasinska, from Microanalytics


Microanalytics, a MOCON Company, Round Rock, TX, USA


The detection and identification of substances that  give rise to aromas and off-odors is often a difficult task. Perception of odors is very subjective and odor detection  thresholds vary from person to person. The identification of  trace levels of compounds responsible for perceived odors is  difficult using conventional analytical tools. This paper will  focus on a novel method for sampling and analyzing aromatic  volatile compounds using an analytical system specifically  designed for odor analysis.


Odor evaluation:


The human sense of smell varies widely from person  to person in terms of sensitivity as well as odor character  perception. What smells bad to one person may be perceived  as desirable or at least non-offensive to another. The out  gassing from the plastics and leathers of a new car is  perceived favorably by so many people that it has been  artificially manufactured and is available to revive that odor  long after the original compounds have dispersed.


Our sense of smell is considered our most primitive  sense, probably having originally developed as a warning  system. From experience, we often associate bad smells with  danger. Spoiled food, dead and decaying bodies, and fire all  have smells associated with them that mean to us that our  health may be at risk.


(6)


where ∆Fsh, ∆Fop and  ∆Ftot are the resonant frequency shifts  for the “short” calibration key, “open” calibration key, and the  test key under study, respectively, F0 is the resonant frequency  with no sample present, and α≈C0/Csh~0.01 is a small  correction factor (C0 is the tip capacitance with no sample  present). All values in the right hand side of Eq.(6) can be  experimentally measured or theoretically estimated with  accuracy on the order of a few percent. Thus, the CIL  measurement accuracy is estimated to be better than 10%.


Representative measured interline capacitance data are shown  in Fig. 9. A total of 6 structures were measured (in addition to  the “open” and ”short” calibration structures), all with line  length of 20 µm and with interline spacing ranging from 0.09 µm to 1.0 µm. Numerical simulations were also done using a  finite element model and those results are shown by the solid  line on Fig. 9. The agreement between the measurements and  the simulation validates the ability of our tool to perform  quantitative capacitance measurements on these small test  keys interline capacitance on the order of a few femto-Farads.


Conclusions


We have reported on a novel method that allows for spatially  localized in-line FA of non-visual and parametric defects in  Cu/low-k interconnect on production wafers after all three  main stages of the integration – dielectric deposition, dielectric  etch, and Cu metallization. The advantages of this metrology  are the following: a) it is a non-contact, non-invasive, and  non-contaminating (the probe is fabricated entirely from  quartz and aluminum); b) all the test keys are fully compatible  with the Cu dual-damascene technology; c) the test keys for  as-deposited and post-etch measurements are already in use by  other metrologies such as ellipsometry and  OCD/scatterometry, allowing for film thickness, k-value, and  CD measurements at the same site on the wafer; d)


measurements of dielectric constant on patterned wafer yield  the same precision (1σ<0.3%) and accuracy (±2%) for k-value  as those on a blanket wafer; and e) no electrical contact to or  grounding of the wafer is required since both probing  electrodes are located on the probe above the sample and  capacitively coupled to it.


O


[1] S. M. Anlage, V. V. Talanov, and A. R. Schwartz, in


Scanning Probe Microscopy: Electrical and


Electromechanical Phenomena at the Nanoscale, edited  by S. Kalinin and A. Gruverman (Springer, Berlin, 2006).


[2] V. V. Talanov, A. Scherz, R. L. Moreland, and A. R. Schwartz, Appl. Phys. Lett. 88, 134106 (2006).


[3] V. V. Talanov, A. Scherz, R. L. Moreland, and A. R. Schwartz, Appl. Phys. Lett. 88, 192906 (2006).


[4] S. Satyanarayana, R. McGowan, B. White, and S. Hosali, Semicon. Intl., 28 (6), 63 (2005).


0.0 0.2 0.4 0.6 0.8 1.0


0.5


1.0


1.5


2.0点 Interline capacitance (fF)2.56


Interline spacing (µm)


。 Measurement  Simulation


Figure 9: Interline capacitance measurements (symbols) performed using the test keys described in the text, along with  numerical simulation results (line).


Non-invasive acoustic phonon characterization of dynamic MEMS


W.K. Wong, M. Palaniapan, C.L. Wong, S.R. Wang


Centre for Integrated Circuit Failure Analysis and Reliability


Department of Electrical and Computer Engineering,


National University of Singapore


Singapore 117576


Email: wongwk@ieee.org


F.E.H. Tay


Department of Mechanical Engineering,


This paper describes an acoustic phonon-based  characterization technique as a novel tool for the  characterization of dynamic microelectromechanical (MEMS) devices such as resonators, switches, micromirrors, accelerometers and gyroscopes.  The technique intrinsically  features non-invasive characterization due to the favorable  transmission properties of acoustic phonons through device  packaging and high throughput due to universal detectability  from a single detection point, which facilitates high volume  wafer and package level testing.  The dependence of phonon  generation on material properties yields information not  obtained in existing electrical, optical and electron beam  testing techniques such as contact tribology, energy  dissipation, non-linear device behavior and device resonance  modes. Preliminary case study results show that phonon-based  characterization not only provides efficient, non-destructive  testing (NDT) of MEMS functionality, but also insights into  MEMS device lifecycle behavior.


Current tools and techniques for MEMS characterization  include optical methods such as Laser Doppler Vibrometry (LDV) [1] and electrical characterization [2].  While the LDV  is currently the workhorse technique for providing spatial  displacement information in MEMS devices, it requires  decapsulation of packaged devices for direct die access, which  introduces unwanted degradation to the device, compromises  the device environment and possibly disrupts device  functionality, e.g. loss of magnetic coupling in magneticallylatched MEMS microswitches. Precise laser probe positioning  requirements also limit LDV testing throughput.   Electrical  measurements are limited to extrinsic (“black box”) electrical  parameters such as switching conductivity and cannot directly  characterize device mechanical state in most cases, especially  where performance specifications call for cold-switching  operation.    On the other hand, acoustic phonons [3] are  intrinsically generated by dynamic MEMS devices during  actuation [4] and hence carry information pertaining to the  mechanical state of the device in the time domain such as


displacement, transient over/undershoot, damping factor, amplitude and phase response, resonance modes, etc.   For  contact-mode MEMS devices such as RF MEMS switches, acoustic phonons generated by the make and break switching  events carry information on the tribology of the switching  interfaces.   Furthermore, equivalent hot-switching mechanical  performance parameters can be obtained without potential  device degradation associated with electrical hot-switching  tests.  Acoustic phonons (being longitudinal vibrations of  molecular matter in the direction of the wave propagation) transmit well in most solids and hence can be detected on any  external surface on the MEMS device package or wafer as  long as an acoustic transmission path between the generation  and detection site exists.  The technique is easy to implement  even within the constraints of an inline manufacturing  environment as only a single, one-time mount between the  phonon detector and sample is needed.  Therefore, the  technique is amenable to both high measurement throughput  wafer-level testing and non-destructive functional testing for  reliability assessment in package-level testing [5].


Figure 1 shows an electrical block diagram of a basic phonon  detection setup using a piezoelectric transducer such as a lead  zirconate titanate (PZT) crystal paired with a preamplifier  with a voltage gain of 400.   The electrical response of the  PZT transducer (Morgan Ceramics’ PZT-5A) & preamplifier  used was characterized with a -3dB low-pass cutoff at 300  kHz and an intrinsic resonant peak at about 129.2 kHz with a -3dB bandwidth of 3.6 kHz.   In these experiments, the  electrical noise floor was measured at 200 µV.  The sample is  affixed to the PZT using a silicon-loaded paste for optimal  acoustic transmission between the device under test and the  PZT, although satisfactory signal detection sensitivity can  often be achieved using dry coupling especially for contact  mode MEMS devices where acoustic phonon generation  levels are relatively high.  Only a single mounting instance is  required as phonons from multiple generation sites are mostly  well-detected. This means that acoustic phonon detection does  not require repetitive probe positioning instances for multiple  device characterization, for example the LDV laser probe, and  hence can deliver much higher measurement throughput by  eliminating probe positioning overheads.


## Non-invasive acoustic phonon characterization of dynamic MEMS


6


Fig. 1 Schematic of a basic acoustic phonon detection system  for MEMS device characterization.


Proof of Concept Verification


Proof-of-concept was demonstrated using MEMS electrostatic  comb resonators operated in linear and non-linear modes.   Electrostatic resonators have been extensively studied [6] and


FileRontrolSetupMeasure Analyze Ublities Help


4:15FM


reliably fabricated and hence provide a well-understood #100m/dv盛@H


200/dy图


25.0Ba/s


圆佰


benchmark for technique verification.  The periodic  mechanical displacement of the resonator sets up phonon  waves that propagate throughout the bulk solid of the device.  Assuming a first-order pressure-displacement model, the  voltage output of a cylindrical piezoelectric transducer


→


assuming one-dimensional, lossless propagation and ignoring


AAVA2信reflection effects can be expressed as


33 tKx


r


王000s5.00ms/cky.nt0.0<0>T 10mV


hg


Vπ=


moreMleassummartsMarkersScales


where h is the thickness of the piezoelectric disc, g33 is the 0kFrequencyt1*1159.49 RHz7 p-pti)wmeH m162.01 kHz踏m□piezoelectric voltage constant along the axis of the phonon  propagation, r is the radius of the piezoelectric disc, and K is


the effective spring constant dependent on Young’s moduli E


of the propagation medium and piezoelectric transducer.


The proof-of-concept experiments using electrostatic comb


finger resonators were carried out on a Hitachi S-3500N


Scanning Electron Microscope (SEM) which allows in-situ


simultaneous device actuation and high resolution inspection


of device displacements down to about 10 nm under high


vacuum (around 10-5 Torr).  The MEMS resonators were


fabricated at MEMSCAP.  Figure 2 shows an SEM image of a


10 µm comb finger element from which actual peak to peak


displacement amplitudes of the resonator can be directly


ascertained (5.2 µm in this case).  Phonon measurements can


be performed in either high vacuum (10-5 Torr), low vacuum


(10-3 – 2.0 Torr) or atmospheric pressure (760 Torr).  Dynamic


device operation is characterized using time-domain


measurements of the driving signal vd and phonon plots Vout,


as acquired using a digital storage oscilloscope, as shown in


Fig. 3.


Fig. 2  Scanning electron microscope image of 10 µm


electrostatic comb resonator section with 5.2 µm peak-to-peak  vibration amplitude estimated using  full width half maximum (FWHM) criterion.


Fig. 3  Time-domain acoustic phonon waveform Vout (bottom) and reference driving signal vd (top) for electrostatic


resonator characterization.


1.


Resonator Performance Parameters and SEM  Displacement Measurements


For a resonator under electrostatic comb drive, the time  derivative of its displacement x is


( )


[


]


sin(


cos(


V


t v


t x


P


sys


D


ω


⎟⎟⎠⎞


⎜=⎜⎝⎛ ∂∂=


⎟⎟Ot)⎠⎞


⎜⎜⎝⎛∂∂⎟⎟


(2Kgs⎠⎞


⎜⎜⎝⎛ ∂∂


∂∂


where ksys is the system spring constant, VP is the DC bias, vd  is the AC excitation amplitude and ∂C/∂x is a constant [6].  From equation (2), we can derive an expression to describe  resonator displacement at resonance (under linear drive  conditions) as


Sample


15.2 µm


Function Generator:sine, square pulse


↓


10 µm


Preamplifier√


Power Supply DC


Transducer


4 Channels Oscilloscope


y’


Vout vd


⎟⎠⎞


⎜⎝⎛ +


sin


ωt


x C


ac


sys dc


(3)


where Q is the Q-factor of the resonator at its resonance  frequency. For the resonator samples used in this paper, ksys = 237 Nm-1 and ∂C/∂x = 1.8 nFm-1.


Characterization runs were carried out on resonator samples  under three low (linear) drive conditions: 1) VP = 3.0 V, vd =


0.20 V, 2) VP = 4.0 V, vd = 0.15 V and 3) VP = 4.0 V, vd = 0.20  V. From the characterization data, the experimental Q values  of the resonator sample were obtained from frequency  response profiles such as the example shown in Fig. 4.  Displacement measurements were also taken at the resonance  frequency.  Applying equation (3) with the measured Q values  and the resonator ksys and ∂C/∂x, a set of theoretical values for  the resonator peak to peak displacement amplitudes was  obtained as shown in Table I.


155


156


157


158


159


160


161


0 20 40 60 80


≥


/100人120


140


180


Sample 1A, Resonator 1a


Freq / kHz


Vac = 4.8 V(p-p)


Resonant Freq = 158.868 kHz


Fig. 4 MEMS resonator frequency response characterized  using phonon detection at atmospheric pressure.


Table I.  Comparison of measured and theoretical


displacements for resonators #1a.


The results in Table I show excellent agreement between  theoretical and measured resonator displacement amplitudes, with the results falling within the approximately 10% error  range imposed by the 10 nm SEM resolution limit. The results  confirm that the resonator samples comply with equation (3) in the linear operating mode.  Hence, the results confirm the  validity of SEM displacement measurements as a dependable


reference standard for describing the mechanical displacement  of the resonators.


2.


System Transfer Function Verification


To verify the first-order phonon-displacement relationship  described in equation (1), a generalized relationship  describing the order of the relationship is formulated as:


out kx V =


where Vout is the magnitude of the phonon electrical output, x  is the comb displacement and k is related to the system spring  constant of the resonator ksys, the electromechanical coupling  factor kp of the PZT material and preamplifier gain.  By  plotting ln (Vout) against ln (x), the order, n, of the phonondisplacement transfer function can be determined.


n = 0.95


n = 0.87


n = 0.97


-0.50


0.00


0.50


1.00


10人


言1.50


2.50


3.50 4.50 5.50 6.50 7.50 8.50 9.50


ln (x)


Vdc = 9.0V; Vac = 0.30V Vdc = 12.0V; Vac = 1.0V Vdc = 15.0V; Vac = 1.0V


Fig. 5  ln (Vout) against ln (x) plots for resonator #1a under 3  drive conditions.


Resonator specimens were driven under three different drive  conditions: 1) VP = 9.0 V, vd = 300 mV, 2) VP = 12.0 V, vd =


||Drive Conditions |Drive Conditions ||At resonance |At resonance ||
|---|---|---|---|---|---|---|

|Resonator |VP (V) |vd (V) |Q |x (nm) measured |x (nm) theory ||

|1a |3.0 |0.20 |20154 |92 |96 ||

|1a |4.0 |0.15 |17913 |91 |85 ||

|1a |4.0 |0.20 |17911 |117 |114 ||

1.0 V and 3) VP = 15.0 V, vd = 1.0 V representing low to high  drive conditions for this particular design.  Phonon and  displacement measurements were recorded at various vd drive  frequencies in order to obtain ln (Vout) against ln (x) plots for  each drive condition.  These plots are shown in Fig. 5.  From  the experimental runs conducted, the value of the transfer  function order approximates 1.0 for all three drive conditions  and indicates an approximately linear relationship (n=1) for  equation (4). Considering the 15-20% total error tolerance (200 uV noise floor in the electrical phonon and 10 nm in the  SEM displacement measurements), the results are in excellent  agreement with equation (1) with n values ranging from 0.85  to 0.97.     Therefore, we can conclude that the phonon output  provides a reasonably accurate first-order representation of  actual resonator displacements, and hence can be reliably used  in place of SEM or optical displacement measurements in “blind” testing situation where direct imaging of the MEMS


actuating element is either not required or not feasible (e.g. in  package-level NDT).


3.


Repeatability Tests


Repeatability studies were undertaken to verify technique  robustness to variations in experimental conditions and that  the measurement data obtained is a faithful reflection of  device performance without excessive contribution from  measurement artifacts.  Phonon measurements (Vmax) were  carried out on two resonator samples, #3a and #4a, to assess  the repeatability of the in-vacuum resonance frequency (fres) estimation.  A total of 5 dismount-remount cycles were carried  out on each sample with full characterization runs performed  using drive conditions VP = 9.0 V, vd = 0.30 V.  Only phonon  output data has been captured in this set of characterization  runs; no displacement measurements were recorded in order to  avoid any artifacts from electron-beam irradiation and  dielectric charging.  A summary of the resonators’ critical


Function Generator


parameters is provided in Table II.


X2x17


|Resonator |Expt. sequence |fres (kHz) |Vmax (mV) |
|---|---|---|---|

|3a |1 |156.59 |9.10 |

|3a |2 |156.57 |8.55 |

|3a |3 |156.64 |6.64 |

|3a |4 |156.42 |6.53 |

|3a |5 |156.57 |6.26 |

|4a |1 |158.44 |7.18 |

|4a |2 |158.24 |6.38 |

|4a |3 |158.43 |5.80 |

|4a |4 |158.44 |9.38 |

|4a |5 |158.23 |6.24 |

oMEMS↓Switch J3口


901


5V


470Q


Table II.  Summary of phonon-based measurements on


resonators #3a and #4a for repeatability assessment.


For resonator 3a, the mean of the resonance frequencies (fres) obtained for the five characterization runs is 156.56 kHz with  a standard deviation of 0.082 kHz. The mean phonon output at  resonance (Vmax) was 7.42 mV with a standard deviation of


1.307 mV. Resonator 4a had a mean resonance frequency of


158.36 kHz for the five runs with a standard deviation of


0.111 kHz. Its mean phonon output at resonance was 6.99 mV  with a standard deviation of 1.442 mV. These statistics show  that each mount cycle results in slight variations in both  resonators’ behaviour.  As these variations are generally  within the 15-20% system experimental error tolerances, we  can conclude that the present instrumentation exhibits good  repeatability as far as phonon-based resonator characterization  is concerned.


Experimental Case Study on RF Switch


Phonon and Electrical Lifecycle Tests


Here, we report the initial experimental results for phonon  lifecycle characterization of contact-mode MEMS devices  such as RF MEMS switches.  Time-domain mechanical


characterization of the switch elements could not be normally  carried out using existing approaches such as LDV as device  functionality is destroyed by depackaging.  The sample is a  commercially-available electromagnetically-driven and  magnetically latched, bipolar single pole-double throw (SPDT) RF switch.  Although specified for cold-switching  applications, the device was tested under hot-switching  conditions (about 10 mA d.c. switch load) using the circuit  shown in Fig. 6 in these first experiments to facilitate the  identification of the precise electrical make and break  instances, and hence allow direct comparison with the  simultaneously acquired phonon waveforms.  Time-domain  data was continuously acquired over the entire lifecycle of the  devices, typically around 100 million switching cycles.  The  failure criterion in these tests is the loss of electrical continuity  through the switch nodes J2/J3.


Fig. 6  Test circuit schematic for RF MEMS switch case study.


Phonon lifecycle testing results of the RF MEMS switches as  shown in Fig. 7 reveals changes in device behavior that are  not evident in the electrical responses.   During the useful life  phase of the switches (Fig. 7(a)), identical phonon responses  from both J2 and J3 switches are obtained, as expected from  the symmetric design of the SPDT switch.   As the switches  wear out asymmetrically, deviation from symmetric phonon  behaviour is observed (Fig. 7(b)), with increased phonon  generation observed in J3.  J3 subsequently failed prematurely  as shown from the continuous open-circuit state (Fig. 7(c)) while J2 maintained electrical continuity (not shown).   Upon  failure of electrical switching, mechanical cantilever actuation  is still present as evidenced by continuing phonon generation, albeit at significantly diminished levels for J3 (Fig. 7(c)).  This phonon lifecycle characteristic for J3 is summarized in  the phonon energy lifecycle plot of Fig. 8, where moderate  levels of acoustic energy are detected during the useful life  phase, which then gradually rises to a peak just before the  onset of J3 switch failure. Upon device failure, phonon  dissipation drops to levels below initial useful life (not  shown).  A possible failure mechanism relates to localized  resistive (Joule) heating and wear at the J3 switch contacts  during hot-switching device operation.  As the electrical  contact area wears out, the reduced effective switching area


results in higher switching current densities; the increased  arcing and Joule heating-induced stiction results in larger  acoustic phonon dissipation during the switch make event  with the contact pads.  The switch wear progresses until the  switch fails totally and electrical continuity is lost, resulting in  significantly reduced phonon generation due to the absence of  Joule heating and interfacial microwelding after switch failure (Fig. 7(c)).


-0.3-0.2-0.1


0.1


A


,


|


o


^


-0.099


-0.0985


-0.098


-0.0975


-0.097


-0.0965


Time (s)


Time(s)


(c)


Fig. 7 Phonon signatures of RF MEMS switch actuation:


(a) During steady-state phase; (b) just prior to J3 failure;


(c) after J3 failure.


From these results, the loss of electrical switching information  after electrical failure of the switch highlights the potential  usefulness of phonon detection in correctly identifying the  failure mechanism in such cases, particularly in devices which  continue to experience switching even after electrical  continuity is lost.  Also, acoustic phonon characterization  allows the actual switch make and break instances to be  ascertained even in a cold-switching configuration.   This  enables dynamic mechanical switching parameters (switching  delay, bounce time, etc.) to be assessed where electrical  detection of these events are not possible.


:


W


c


<


8


l


?


'


10


15


20h~25


30{n


·


B


u


.35


40


45


Time


Fig. 8  RF MEMS J3 switch acoustic phonon plot as a  function of lifecycle showing sustained elevated phonon  dissipation during the wearout phase prior to failure.


Failure Analysis of Failed J3 Contacts


Failure analysis was performed on failed RF switch  samples to verify the failure mechanism described above.   Using a dual-beam FEI Quanta 3D equipped with an  Omniprobe micromanipulator on decapsulated specimens, the  switching cantilever was dissected using the ion beam and  removed from the die; the start and end points in this fault  localization procedure are summarized in Fig. 9.   SEM and  energy dispersive X-ray (EDX) analysis were performed on  the two sections and the results are shown in Fig. 10.   In this  particular case, significant pitting was found on the die-side J3  contacts (Fig. 10(a)) which was exactly correlated to material  deposited on the switch cantilever pads (Fig. 10(b)).   Elemental analysis by EDX revealed that possible traces of  niobium (Nb) were found on the cantilever pads that are  normally present only on the die contacts in unstressed, good  devices (EDX analysis of pristine cantilever pads reveal only  gold is present), thus indicating elemental material transport  from the die contacts to the cantilever.    The surface pitting  and stiction in the switching event is most likely the source of  the high phonon generation levels recorded earlier as shown in  Fig. 7(b)).   To confirm this, more in-depth studies using much  larger sample sets would be required before a more general  conclusion can be made regarding the relationship between  acoustic phonon signatures and the device failure mechanism.


Initial  Phase


Mid Phase


Final Phase


Useful life


Wearout


J3 make


J2 make


J3 make J2 make  J3 electrical switching waveform


J3 electrical switching waveform


J3 electrical


switching


waveform


率0lc。1


d30 1S15.1mm Cuoraexne8dwellWD(a)


1000-0.1


900-


Fig. 9  Disassembly of RF MEMS device failure analysis  showing (a) SEM image of device after depackaging prior to


hV


0001.002003.004005006007.008009.0010.00


FIB disassembly; (b) Optical image of die after switch  cantilever removal; (c) Optical image of switch cantilever  after disassembly.


Acc.VSpot MagnDetWD


20l mu


2.00kV 3.01800xSE14.9 MEMS SPDT


Acc.V Spol MagnID6WD


2.00kV 3.0 505xD0W6.3 MEMS SPDT50 μm


Fig. 10  SEM and EDX analysis of RF MEMS J3 switching  elements showing matching pitting sites on (a) Die contacts;


(b) Switch pad; (c) EDX of switch pad confirming material  transport (Nb) from die contact to switch pad.


Niobium (Nb) not


800-


present in unstressed


700-


600-


10300 3


400-


300-


81


200-CPAN10Pollest190王 PR1E


100-


0-


NM1


11无PdNKeNN饰所 PS


Au


samples


100 µm


中


Proof-of-concept was demonstrated for a novel dynamic  MEMS characterization technique using acoustic phonon  detection on MEMS resonators and RF switches.   As acoustic  phonons carry information pertaining to the mechanical state  of the MEMS device and are sensitive to surface tribology, additional information on the device not available using  existing optical and electrical testing can be obtained, including phonon dissipation and lifecycle degradation.  Most  importantly, the phonon detection technique is relatively easy  to apply and promises high throughput compared to existing  optical techniques, which may make it suitable to meet massvolume inline MEMS testing goals in a cost-effective manner.


Acknowledgments


The authors would like to acknowledge the contribution of  Y.P. Xu and L. He for providing the resonator test samples.   Funding support for this work was obtained from NUS ARF  research grants R-263-000-316-101 and R-263-000-316-112.


[1] Vignola, J. F., Liu X., Morse S. F., Houston B. H., Bucaro, J. A., Marcus, M. H. and Photiadis, D. M., “Characterization of silicon micro-oscillators by scanning  laser vibrometry,”  Rev. Sci. Instr. Vol. 73  No. 10 (2002), pp. 3584-3588.


[2] van Spengen, W. M., Puers, R., Mertens, R.  and de Wolf, I., “A low frequency electrical test set-up for the  reliability assessment of capacitive RF MEMS switches,”  J. Micromech. Microeng. Vol. 13  (2003), pp. 604-612.


[3] Houston, B. H., Photiadis, D. M., Marcus, M. H. , Bucaro, J. A. , Liu, X. and Vignola, J. F., “Thermoelastic  loss in microscale oscillators,”  Appl. Phys. Lett. Vol. 80   No. 7 (2002), pp. 1300-1302.


[4] Yang, J., Ono, T. and Esashi, M., “Energy Dissipation in  Submicrometer Thick Single-Crystal Silicon Cantilevers,”  J. Microelectromech. Syst. Vol. 11 No. 6 (2002), pp. 775-783.


[5] de Wolf, I., Czarnecki, P., Jourdain, A.,  Modlinski, R. and Tilmans, H.A.C., “The influence of the package  environment of the functioning and reliability of  capacitive RF-MEMS switches,”  Microwave Journal  Vol. 48, No. 12 (2005), pp. 102-109.


[6] Tang, W. C., Nguyen T-C. H. and Howe, R.T., “Laterally  driven polysilicon resonant microstructures,” Sens. Actuators, Vol.  20 (1989), pp. 25-32.


Magnetic current imaging with magnetic tunnel junction sensors: case study and  analysis


Benaiah D. Schrag, Matthew J. Carter, Xiaoyong Liu, Jan S. Hoftun, and Gang Xiao


Micro Magnetics, Inc., Fall River, MA, USA


We describe the use of magnetic tunnel junction (MTJ) sensors for the purposes of magnetic current imaging.  First, a  case study shows how magnetic and current density images  generated using an MTJ sensor probe were used to isolate the  root cause of failure in a newly-designed ASIC.  We then give  a brief introduction to the operation and construction of MTJ  sensors.  Finally, a full comparison is made between the three  types of sensors which have been used for magnetic current  imaging: giant magnetoresistive (GMR) sensors, superconducting quantum interference devices (SQUIDs), and  magnetic tunnel junctions.  These three technologies are  quantitatively compared on the basis of spatial resolution, sensitivity, and geometry.


Case Study: Introduction


A small fabless design house was looking for quick fault  isolation and failure analysis on an ASIC they were  developing. They had limited in-house resources and wanted  to quickly correct any errors and get a working device to the  market. The ASIC, which contained analog and digital  sections, was a low-power, precision power monitoring and  conditioning device with a communication bus allowing  ganged operation of many units.  The entire lot of die from the  first shuttle run of the device was found to be non-functional. All the die exhibited shorts of some kind, though the exact  mechanism(s) involved differed from chip to chip.


Initial inspection using a test evaluation board showed  excessive supply currents, clamped output voltages, and nonfunctional logic. The test board was designed to allow the  ASIC to be power cycled, voltages ramped, logic tested and  the outputs monitored.  Per its design, the ASIC should have  drawn on the order of 10 µA from the supply, but the actual  devices had supply currents greater than 1 mA.  In no device  tested did the digital block exhibit a logic response of any  kind.  Some die had shorts between the voltage regulator (VLDO) and the battery ground (VBAT0) pins, some had  VLDO to battery voltage (VBAT1) shorts, and others had  both. Due to the varied fault modes it was initially thought  that a design rule might have been violated.  However, design  check, layout check, and database check found no such  violations.


The first technique used for analysis was liquid crystal.  The  technique seemed to indicate excessive joule heating in the  digital block of the ASIC.  However, the amount of power


dissipated was so great that the area darkened by the liquid  crystal included roughly one quarter of the full die.


Wafer dicing and microprobing were performed on one of the  failed die to try to isolate the cause of the faults. The die was  depassivated and individual sub-circuits were isolated and  tested. It was found during this process that the entire digital  block was non-functional. The digital block had apparent  over-current, failed communication logic, and failed logic  input and output.  The analog to digital converters  incorporated into the ASIC were also non-functional. They  relied heavily on the digital block, but this failed to explain an  over-current measured on their separate filter power  supply.  In addition, low resistances were measured between  several combinations of pins which should have been  electrically isolated. One of these low resistance shorts was  seen between a power supply trace (VBAT1) and a voltage  regulator trace (VLDO). Another was observed between  VLDO and the battery ground (VBAT0). It was not possible  to isolate the location of these shorts by probing.


The probing and liquid crystal both showed strong evidence of  a major defect in the digital block of the ASIC. Probing also  revealed several low resistance shorts that liquid crystal was  unable to detect due to insufficient power dissipation. Due to  the complex and varied faults found in the die, localizing  these faults using probing proved extremely difficult. Furthermore, the existence of many low-resistance shorts  highlighted the shortcomings of liquid crystal. A global view  of all the currents flowing through the device was requested  by the design company to understand the overall behavior and  specific fault locations of the device. To produce this current  map, scanning magnetic microscopy [1-4] was employed.


Sample Preparation


Magnetic scanning was performed using Micro Magnetics’ CS1000 scanning magnetic microscope.  The ASIC was  packaged in an open top ceramic leadless chip carrier (CLCC).  The surface of the ASIC was 4 mm below the top of  the LCC socket, and the total area of the die between the  wirebonds, which surrounded the die on all sides, was 1.2 mm  square.  Because of these spatial constraints, scanning was  performed using a standard vertical sensor probe using  magnetic tunnel junction (MTJ) sensor technology. [5]  This  sensor probe tapers to a point and has a very small footprint (< 150 x 300 µm), so that the sensor can be brought to within ~5 µm of the sample surface even with limited access.  A picture  of the MTJ sensor probe is shown in Figure 1.  Magnetic


## Magnetic current imaging with magnetic tunnel junction sensors: case study and analysis


13


scanning with MTJs can be done under ambient conditions, and no special preparation of the sample or the sensor probe  was done.  More details on the magnetic tunnel junction  technology can be found following the case study.


Scanning was done in AC mode.  In this mode, the CS1000 is  only sensitive to the user specified modulation frequency, so  no magnetic interference is possible. VBAT1 was powered  with 2.3 V and the current was monitored by the system.  A  300 mV peak-to-peak sine wave at 19 kHz was added on top  of the DC supply voltage for imaging. This modulation  voltage corresponded to ~500 µA RMS of AC current.


Magnetic Scanning and Current Mapping


Because the die being imaged had been depassivated, scanning was done in a non-contact, plane-following mode to  ensure that the sample would not be damaged.  In this mode, the system uses a level sensor to automatically calculate the


tilt of the sample surface.  The tilt is found by lowering the  sensor probe onto the sample at a number of different  positions on the die.  Each time the sensor probe contacts the  die, this level sensor automatically detects the contact force (the sensor is mounted on a very flexible assembly which  keeps this force to ~ 20 µN or less), immediately stops the  motion of the sensor probe, and registers the location of the  die surface to within 0.5 µm.  Once this procedure has been  performed for five different locations on the die, the  information collected is used to automatically calculate the tilt  of the sample surface.  During scanning, the system can then  move the sensor probe vertically to maintain a constant  distance (~5-10 µm, in this case) between the probe and the  die surface, without the need to physically level the die.


The MTJ mounted on the vertical probe was easily able to  enter the cavity and contact the die. Regions of interest (ROIs) were selected visually by drawing rectangles on the optical or  stitched image.  The field of view of the optical camera with  10X objective which was used is 543 x 408 µm. To create the  images of the full (2 x 2 mm) die the system captured and  blended 16 optical images to create a stitched image.  Conversion of the raw magnetic field data into maps of  current density was accomplished using Micro Magnetics’ VIsta analysis package.


Figure 1.  Picture of the MTJ vertical probe used for the  magnetic current imaging case study.


The first ROI to be magnetically imaged contained the current  path between the VBAT1 wire bond and the point at which  the current fans out into the die (Figure 2). Because this was  the known point of entry of current onto the die, it was a  logical starting point for tracing the current flow through the  die. The current mapping proceeded to follow the VBAT1  current along its metal 3 trace across the die. The current on  VBAT1 abruptly dropped to a perpendicular trace on metal 2. This was clearly an indication of a short between the VBAT1  metal 3 trace and the metal 2 trace below it. The rogue current  is then seen looping into a section that completed the VBAT1  to VLDO current path, as shown in Figure 3.  This was  immediately identified as a major fault.


Since liquid crystal had shown a large power dissipation over  the entire digital section of the die, this was the next area to be  imaged.  With the powering scheme being used, no current  should have been flowing either on the VLDO or into the  digital block. However, the earlier results had shown that the  VBAT1 current was shorted to the VLDO.  The stray VBAT1  current was mapped flowing along the VLDO branch into the  digital section.


Figure 3.  Current density image showing the flow of current  through a short between the normally-open VBAT1 (M3) and  VLDO (M2).


Figure 2.  Magnetic field image confirming that current was  entering the die through the VBAT1 wire bond, as expected.


co


290 pm


100pn


Figure 4.  The current density map showing current entering  the digital block.


The first images of this area showed the VLDO current path  approaching the digital block along the expected path.  As  seen in Figure 4, these results shows that the VBAT1 current  approached the digital block along an interconnect on M4, taking a 90 degree left hand turn, passing through a via down  a layer to a trace on M3, backtracking underneath its previous  path, and then taking another 90 degree turn. After dropping  down another layer and making more turns, the current  continues along the edge of the digital block but then appears  to disperse throughout the entire area immediately upon  entering.  This behavior was unexpected, because the  assumption was that the current should have followed the  VBAT1 trace around the digital block and to the VBAT0  trace. This indicated one or more shorts in the digital block, a  result which made sense in light of the liquid crystal results.  Figure 5 shows a full-die current density map showing the  path of the leakage current throughout the die.


Some dangerous commercial substances have no  odor at all and must have aromatic compounds added to them  to help us detect leaks or their build up to toxic levels.  Liquid  propane and natural gas (predominately methane) do not have  natural odors. The thiol compound ethyl mercaptan, whose  odor is detectable at the sub-ppb level, is added to these  hydrocarbon compounds so that leaks are easily detectable.1


There is some standardization in the field of odor  evaluation.2, 3 The American Society of Testing and Materials, (ASTM), the European Committee for Standardization (CEN) and the American National Standards Institute (ANSI) have  standard methods used for laboratory analysis of odors. In  general, the following three sensory scales are employed and  assessed by trained analysts.4, 5


The first is perception of odor intensity. The standard  ASTM method E544-99 describes the measurement and  quantification of odor intensity in comparison to a series of  concentrations of an n-butanol reference known as an Odor


Intensity Reference Scale (OIRS). The intensity (I) is given in  comparison to the perceived intensity of the reference.


The second scale is the hedonic tone (HT) which  measures the relative pleasantness / unpleasantness of the  odor. The more pleasant the odor, the closer the rating is to +10 on the scale. A neutral rating is given a 0 and the more  negatively perceived, the closer the rating is to -10. Hedonic  tone is a subjective rating and may also be influenced by the  personal experiences and olfactory memories of the analyst.


The final scale is based on odor descriptors. The  eight recognized descriptor categories are floral, fruity, vegetable, earthy, offensive, fishy, chemical and medicinal. Each of these categories is broken down further to better  describe the odor. For example, in the offensive category, an  odor may be described as burnt, manure, sour, vomit or fecal. Floral may be described as lavender, vanilla, rose-like, eucalyptus or perfumy.


The odor evaluation method used here differs from  the three methods cited above.  It is based on the  determination of the odor character of each isolated compound  in an analyzed sample by GC/Olfactometry. The odors of  isolated compounds are matched to the overall odor of the  whole sample. The method includes the simultaneous  identification of the isolated odor compounds by mass  spectrometry. This method has been used very effectively in  several fields, including food and beverage industries, agriculture and indoor environmental sampling. This paper  describes the application of this method to identify and  quantify an off-odor compound in a complex electronic  system.


Traditional analysis of residues and volatile organic  compounds:


The tools conventionally used to identify residues  and volatile compounds are Fourier Transform Infrared  Spectroscopy (FTIR) and Gas Chromatography Mass  Spectroscopy (GC-MS).


FTIR is used to identify organic compounds by  measuring absorption of infrared energy by covalent bonds in  different functional groups as they bend, twist and vibrate.  Functional groups are organic compounds composed of  groups of atoms that define the structure of a particular family  of compounds and at the same time, determine their  properties.6 Each compound has characteristic absorptions that  produce a spectrum that can be referenced against stored  spectral libraries for comparison. Volatile compounds  collected in a gas cell can be separated by gas chromatography (GC) and then identified by FTIR, but more often a Mass


## Analysis and Identification of Off-Odor Compounds in Electronic Systems


20


Spectrometry detector is used instead. FTIR can be more  effectively used to identify chemical residues left on surfaces. The GC-MS technique involves first the  chromatographic separation of volatile compounds extracted  from a sample followed by their detection and identification  using a mass spectrometer detector.  Simple methods exist to  collect and concentrate volatiles from liquid, solid or gas  phase samples and, in particular, from surfaces.


The problem with both methods is that neither is  particularly effective in odor identification. Many volatile  compounds have no odor at all and the substances that cause  odors are often present in trace amounts and well below  typical detection levels or at the spectral noise level. For this  reason, a GC-MS chromatogram or FTIR spectrum of a good  sample may look identical to that of a sample with an  offensive odor issue.


Case Study:


An off-odor was perceived in a product sample of an  electronic sub-assembly that was described as “burnt  transmission oil.” Due to differences in the sense of smell of  the untrained evaluators, it was difficult to gain consensus on  whether any particular sample had the offensive smell, or if  the smell was that normally associated with electronics and  plastics. Due to the complexity of the sample, it was difficult  to determine which component was the actual source of the  odor. After much “untrained sniffing,” most odor evaluators  were in agreement that the sample did have an unpleasant  smell (negative rating on the hedonic tone scale).


Preliminary analyses included GC-MS and FTIR of  the residue from the sample sub-assembly metal surface. A  large number of volatile organic compounds were detected, but no information was obtained as to which, if any, of these  compounds had an odor. Collection of volatiles for GC-MS  analysis was performed by heating the entire sample in an  oven at 40oC and collecting the headspace compounds in a  cooled carbon absorption trap. The trap was washed with  hexane to elute the headspace volatiles and the resulting  solution was injected into the gas chromatograph.


The complexity of the set of out gassed volatiles  from the sample of the electronic sub-assembly is shown in  the GC-MS chromatogram seen in Fig. 1. There are thousands  of individual compounds in the sample, most of which are not  resolved chromatographically.  From this data, it is not  possible to relate odors to individually identified compounds.


Fig. 1: GC-MS chromatogram of the complex sample. A  great number of compounds are present but no  information as to which may produce an odor can be  determined using this analysis by itself.


In tandem, FTIR was used to analyze the residues left  on the metal surfaces of the sample sub-assembly. The oils  used in the metal stamping process are designed to flash off in  a drying process. No cleaning process is used to remove  remaining residues. The cleanliness criteria specified was that  no visually perceptible residue remains on the surface. Residues were collected by flooding depressions in the  stamped metal with the solvent acetonitrile. The solution was  collected in a dropper and evaporated drop by drop onto an  aluminum-coated slide, thereby concentrating the residues so  that meaningful spectra could be obtained. The vendor  supplied samples of all oils used in their factory for various  stamping processes. Two particular oils matched the residues  on samples identified as having off-odors. These were not the  oils specified for stamping that particular part (Figs. 2 and 3).


Fig. 2: FTIR comparison of the specified oil #1 to residue  on “smelly” sample. Match is only 69.59%.


300


3000


26002000


1500


1200


Fig. 3: FTIR spectrum of non-specified oil #5 residue on “smelly” sample. Match is 95.52%.


8888228Mhte 05, nospied


*22888rs8


40 8


5分


At this point the root cause could not be proved  because there was no particular compound identified as the  cause of the odor and the analysis methods used could not  provide this information. The FTIR analysis only proved that  the wrong oil was used in manufacture of the sample subassembly.


In a complex sample finding root cause for an offodor can be very challenging. A systematic and scientific  method of evaluating off-odor compounds was needed to  quickly find root cause and measure the level of the  contaminant present in order to drive corrective action. This  was accomplished using specialized, highly sensitive  analytical instrumentation specifically designed for odor  analysis. The instrument provides for separation and detection  of volatile compounds using GC-MS and simultaneous  sensory analysis through a sniff port attachment. The sniff  port allows a trained analyst to assess odors as isolated  compounds that elute from the chromatogram in real time.


Odor Analysis Methodology Using Aromatrax™: Initial assessment:


Two “smelly” and one reference electronic subassembly samples were submitted for odor evaluation. Each  entire sample was wrapped in aluminum foil to prevent crosscontamination and loss of odor compounds. Each sample was  opened separately in a closed room and assessed by trained  odor analysts for the presence of off-odors. It was agreed that  the two “smelly” samples had an unpleasant “burnt” odor that  was absent or greatly reduced in the reference sample.


Sample collection, headspace sampling:


In order to measure volatile compounds a systematic  collection method must be followed. The collection vessel  should have the smallest volume that can accommodate the  sample. Glass jars with TeflonTM tops are often used because  they contribute only very low levels of interfering out gassed  species to the analysis. A pinhole in the TeflonTM top allows  insertion of the SPME fiber into the headspace of the closed  container. The fiber collects and concentrates the volatile  compounds for a set period of time (Fig. 4).


Fig. 4: SPME fiber collector and metal sample in 1 liter  glass jar. SPME fiber is inserted in a pin hole in the  TeflonTM jar cover to collect and concentrate volatile  organic compounds.


The SPME fiber is a 1 cm length of fused silica rod  coated with an 85-micron layer of polydimethylsiloxane and  carboxen (Supelco pn 57334-U).  A protective stainless steel  needle encases the fiber until it is ready to be used.  A plunger  is depressed to expose the fiber to the sample headspace and  then retracted after the collection time period is complete.  Collection time periods can be as short as minutes or even  seconds for very intense odor compound detection at the sniff  port.  In order to collect enough of the odor compound for its  identification, a collection time period of 24 hours or more  may be required.


Headspace sample collection can be modified to  accommodate large, complex samples. In our case study, the  entire reference and “smelly” samples were wrapped in  aluminum foil for sampling. Also, various component parts of  the intact samples were isolated using aluminum foil to  enclose them. An SPME fiber was then inserted into the  headspace through a pinhole in the aluminum foil.


Instrumentation:


The AromatraxTM odor analysis system is a modified  GC-MS system that combines traditional gas chromatography  with simultaneous sensory analysis by the addition of a sniff  port. This configuration allows a trained sensory analyst to  assess the odor of volatile compounds as they are separated  and elute individually from the chromatograph column.


The AromatraxTM system is built onto an Agilent  6890 GC with an Agilent 5973 Mass Spec Detector. The GC  inlet is equipped with a Merlin Microseal septum and is  operated in splitless mode. SPME collected samples are  thermally desorbed in the inlet at 250° C. There are two  tandem GC columns in the system, a 30 meter BP5 column  followed by a 30 meter BP20 column separated by a Deans  Switch for multidimensional chromatographic heartcutting.  There is Flame Ionization Detector (FID) detector for the first  column and a split to the Mass Selective Detector (MSD) and  sniff port for the second column.


Aromagrams:


As the separated compounds elute from the  chromatograph column, a trained analyst is stationed at the  sniff port and describes the odor and assigns an intensity level  to each in real time (Fig. 5 and 6). The result is an aromagram, the analog of a chromatogram in which only odors and their  intensities are plotted against their retention times. Because  the retention times of the aromagrams and GC-MS  chromatograms are synchronized, they can be superimposed. In this way, the offending odors are found to correspond to  narrow retention time windows in the GC-MS  chromatograms.


，


Fig. 5: An analyst at the sniff port records retention time,


description and relative intensity as compounds with odors mdsnh


Time linaed


unitn


2014


are eluted off of the GC chromatograph.


Fig. 6: Aroma description screen. The analyst selects the  descriptor that best characterizes the odor as it is detected.


In the case of a very complicated sample a very large  number of odors are normally detected at the sniff port.


Overlaying aromagrams and GC-MS chromatograms allows  the analyst to focus on the retention time windows of the  chromatograms where the off-odors are known to be located.  The image in Fig 7 is an aromagram of a survey  analysis of the Case Study sample. A strong “burnt” odor was  characterized at retention time of 17.6 minutes. Aromagrams  for all the samples tested showed the same “burnt” odor to be  present. The “burnt” character was correlated directly to the  offensive off-odor in the sample and it was most intense in a  metal part that had components that contained plastics and  resins. The reason that the “burnt” odor was found to some  degree in all the tested samples is because materials such as  plastics and resins are good absorbers of odors. There is  actually a transfer of the off-odor from the source to all other  components and this accounts for the presence of the odor in  the other areas.


*


Bhut


Aromagram from survey sample.


Numerous odors identified.


万


售


宁


CGEAA


至


紧


3-


eno


野


noreeh


7025X0nm


Fig. 7: Aromagram from survey sample. Each peak  represents a unique odor perceived by the analyst. A  relative intensity and descriptor is assigned to each odor.


|Aroms Data  Acqoition Actieve Daasiplees|会|会|会|1|T00|T00|同 mTe 200|同 mTe 200|同 mTe 200|||
|---|---|---|---|---|---|---|---|---|---|---|---|

|that Gencal Erart||||Thex ligun|then Parres|then Parres|Dsm|Dsm|Dsm|||

|||||||||||I||

|Gw taps||C8ao Lem|hae|hae|hae|hae|Athlyds ve|Hos Getertum|Hos Getertum|1- Pice||

|8-||Lencen|Ae|Ae|Ae|Ae|Naw|valed|valed|Femcay||

|R exccia||SXa|LOo|LOo|LOo|LOo||d***|d***|0||

|Fesh||grevwd na|yroc|yroc|yroc|yroc|nes|||H||

|Sm||giitpap|s|s|s|s|erob|3|3|Sexpy.||

|||||||||thats|thats|op||

|||||||||Matsom|Matsom|份||

|Orange|Sour|Green||
|---|---|---|---|

|Orange Peel|Pungent|Mally||

|Grapefruit|Swealy|Buttely||

Multi-dimensional Gas Chromatography:


After running a survey sample to establish the general location  of the offending odor, further refinement of the chromatogram  is needed for positive identification. This is accomplished  using Multi-Dimensional Gas Chromatography (MDGC).


Because the AromatraxTM system has two columns of  very different separation characteristics in series with a  Dean’s switch separating them, compounds eluting from the  first column can be diverted from entering the second column (Fig 8).  A “heartcut” from the first column is made when a  narrow retention time window thought to contain the target  odor occurs and the heartcut is passed through to the second  column.  All compounds eluting before or after the heartcut  are diverted from entering the second column and are thus “filtered out” of the analysis.


Fig. 8: There are many variations on the MDGC theme.  The  simplest configuration is shown in the diagram.  P (1 and 2) are  pressure feeds, V (1 and 2) are valves, MPA is the midpoint  aperture, FID is the flame ionization detector, CTT is the cryotrap, OSI is the open split interface, MSD is the mass selective  detector, an optional PID is the photo-ionization detector, and  OD is the olfactory detector.


The first column separates compounds based on their  boiling points. Next the “boiling point” heartcut window of


4600


compounds is then introduced to the second column that


4000


separates compounds by their polarity.  These two modes of


3500


separation are physically very different and the net effect is


that a narrow plug from the first column spreads out during


中 8


2000


passage through the second column. Very high


b


n280o u


chromatographic resolution of the heartcut compounds is


achieved in this way. In the present case study, the burnt odor


1800


compound was isolated from all other compounds.  A good  quality mass spectrum of the burnt odor compound was


1000


obtained at the same time the burnt odor appeared at the sniff


500


port.


1230****17301090928h6*1830


In the present case study, the burnt odor in the


Time.--


aromagram and GC-MS chromatogram was identified as a  sulfur compound having a low odor threshold.  The  identification was confirmed using a legitimate standard for  the suspected sulfur compound. An overlay of the GC-MS  heartcut chromatogram for the off-odor retention time window  and the simultaneous aromagram show a one-to-one  correlation of odor to mass spec peak (Fig. 9).


te167017%


Thehouml


25


1es0n's


160a'e


Fig. 9: Overlay of MDGC chromatogram and aromagram. The small peak that overlaps with the odor on the  aromagram would not be detected in a normal GC-MS


analysis. MDGC provides much better resolution and


INIGLdl


MSD


detection of peaks in the noise level range of the spectrum.


日d1


口AZ


Root cause analysis:


After isolation of the odor and identification of the  sulfur compound as the cause of the odor in the electronic


+00wew00+O9OPIDODCTT


sample, an attempt was made to determine its source. Confirmation analyses were performed on metal “coupons” of


Column 1


Column 2


several oils used by the vendor in their factory. The “coupons”


口


were prepared by dipping 3/4” X 3” pieces of bare metal into


P2


the various suspect oils and allowing them to air dry. The “coupons” were then wrapped in aluminum foil to isolate  them. At the lab, each “coupon” was placed in a one-liter jar  and allowed to equilibrate for 24 hours.  MDGC-Olfactometry  analysis done on the headspace of the oil samples was the  same as the analysis performed on the original samples. Two  of six oils were found to contain significantly high levels of  the compound (Fig 10).


Sulfur Compound  Standard


Fig 10 Comparison of two “coupons” with the sulfur  compound standard (bottom trace)


Three of the six “coupons” had extremely low levels  and one had undetectable levels of the sulfur compound (Fig  11).


毕


Overlay of MDGCchromatogram and


aromagram


B-不


Abundance600


e500


谷


burntodor


one


400 300


↑


1003719


Time (min)


1820


700 900


10-


900


2一


Sulfur Compound


Fig 11: Comparison of four different oil “coupons” with  the sulfur compound standard (top trace)


Further confirmation of the oil as the source was the  matching FTIR spectra of the oils containing the sulfur  compound to the residues found on the “smelly” samples (Fig  12).


2500Waanunders (cno-)2000


5300


Fig.12 FTIR analysis of residue on “smelly” samples has a


95.5% match to one of the oils containing the sulfur  compound.


Quantification of Odor Causing Compound:


The preceding analyses were used to detect and  identify odor causing compounds but do not give any  quantitative information.


The sulfur compound was quantified in the  headspace that was produced from actual metal parts from the  samples where the odor was found.  The off-odor stamped  metal samples were cut to give 7.6 cm X 16.3 cm pieces. These representative pieces were placed in 1 liter headspace  sampling jars and equilibrated for 24 hours.  The headspaces  from these pieces were analyzed as before, except that  quantitative results were obtained by comparing the obtained  GC-MS peak areas with those generated from a standard  curve for the pure sulfur compound.


A six-point standard curve for the sulfur compound (vapor pressure = 0.3 mm Hg) was made by diluting saturated  vapor to six appropriate concentration levels, obtaining their  headspace GC-MS peak areas and plotting them against  concentration (Fig. 13).


y = 2.0056x - 5.2321 R2 = 0.9946


-20 0 20 40 d60 80 E100 120 140 160 180


30


50


60


70


80


90


Benzyl Mercaptan concentration (ppb)


Fig. 13: Six point calibration curve developed from serial  dilutions of the pure sulfur compound standard.


The measured sulfur compound levels per square  centimeter of surface area from two “smelly” samples were


compared to the calibration curve and values of 0.39 ng/cm2


4na


and 0.045 ng/cm2 of the sulfur compound were obtained.


36


地


Conclusions:


The stamping equipment used in the manufacture of  the samples was not dedicated for use with any particular oil.


9328Ew5001%838


A constituent (sulfur compound) in two other oils used in the


安


factory, for the manufacture of different parts, was the source


4 8


of the odor on the “smelly” samples. The corrective action


was the elimination of the use of these oils from the factory


R


altogether. This was done in order to guarantee that the oils  specified in the manufacture of the parts did not become  contaminated due to the use of multiple oils with the same  manufacturing equipment.


Quality, supply chain management, and FA engineers  should be aware of this novel method of off-odor analysis. Without the correct approach, off odor analysis is difficult to  perform and time and resources may be wasted in analyses  that will not result in determination of root cause. Using  specialized equipment, a targeted approach, and analysts  trained in odor evaluation, off-odor analysis problems can be  definitively solved.


References:


1. Ethyl Mercaptan, definition; Dictionary web page, www.answers.com/topic/ethyl-mercaptan.


2. prEN 13725: Air Quality-Determination of Odor  Concentration by Dynamic Olfactometry., Technical  Committee CEN/TC 264, European Committee for  Standardization. September, 1999.


3. ASTM E54475, 88m “Standard Practice for  Suprathreshold Intensity Measurement, American  Society for Testing and Materials, Philadelphia, PA,


1989.


4. McGinley, Charles, P.E., St. Croix Sensory, Inc., Standardized Odor Measurement Practices for Air  Quality Testing, Presented at Air and waste  Management Association, Symposium on Air Quality  Measurement, Methods and technology, 2002, San  Francisco, CA, 13-15 November 2002


5. Laboratory Evaluations: Odor Evaluation Parameters, pgs. 1-7, Copyright 2002, PO Box 313, 3549, St. Croix Sensory, Inc Lake Elmo Ave, MN 55042, www.fivesenses.com


6. Morrison and Boyd, Organic Chemistry 3rd edition, Allan and Bacon, Inc., (Boston, May 1976), pg. 176


Sulfur Compound Co entration (ppb)


System Failure Analysis Process and Case Study


Nicholas Konkol


Intel Corporation, Beaverton, Oregon, U.S.A.


Failure analysis at the system level requires a well-defined  process and methodology in order to drive quality  improvements onto motherboards or other subsystems of a  personal computer. This process needs to be structured around  the type of failure mechanisms that an FA group desires to  understand. This paper discusses a specific case study  involving electrical overstress in a personal computer that  impacted the motherboard of the system. The case study  resulted in a solution to increase quality on motherboards in  the context of electrical overstress prevention.


The role of a Failure Analysis group is to establish a solid root  cause and clearly answer the critical question around why a  failure happened. This is increasingly more difficult when  understanding reliability based failures as opposed to time  zero quality related failures. As part of the Field Failure  Quality Improvement Team, the Failure Analysis group is  responsible for identifying problems with motherboards that  maybe due to a reoccurring situation and makes the necessary  recommendation that will result in elimination of the failure  mechanism. This process (Figure 1.) from identification to  elimination is implemented using the following steps: Sampling, FA/FI (Failure Analysis/ Fault Isolation), Pareto  analysis, Defect Trend, Failure Duplication, and Corrective  Action. This paper illustrates this process. And while it  outlines specifics for personal computer mother boards, this  process is viable for most consumer products.


Sampling


Pareto


FA/FI


Defect Trend


Failure Duplication


Corrective Action


Figure 1: System Failure Analysis Process Flow


Symptom Categories


Sampling:


Customers returned a number of motherboards with various  symptoms. The boards were classified under these types of  symptom categories: No Power, No POST (Power on Self  Test), and No LAN (local area network). The No Power  boards prevented end user PCs (Personal Computers) from  turning on. The No POST boards prevented end user PCs


from booting to Windows. And the No LAN boards prevented  end user PCs from making a network connection. The impact  of No Power failures was significantly more than the other  two categories, hence became the major focus area.


Failure Analysis/Fault Isolation


FA/FI :


In this case study, the motherboards within the No Power  failure symptom category were selected for analysis and sent  to the Electrical Failure Analysis/ Fault Isolation Lab.  Here, each board undergoes fault isolation. The lab utilizes different  methods to isolate the fault such as continuity checks, signal  observations, bus operation observations, functionality tests, stress tests, non intrusive captures, and material analysis. Equipment such as powerful logic analyzers, infrared cameras, curve tracers, high speed digital oscilloscopes, signal  generators, and digital volt meters help to employ their  techniques.  For example, memory and data address transfers  can be examined using a logic analyzer interfacing between  critical components on the motherboard. If a memory data or  address signal returns the wrong value, a curve tracer can be  used to test for an open or short bit on the memory bus. After  the open or short bit is verified by the curve tracer, a TDR (Time Domain Reflectrometry) is used to locate the open or  short at the PCB (printed circuit board) solder joint or within  the package itself. An example of a non intrusive method of  analysis would be to examine a board that powers on for three  seconds and then shuts down. An efficient debug technique is  to mount the board in a uniformly emissive and reflective  chamber, observe the board power cycle with an IR camera1, video subtract a gold board power cycle from the failure  board, and locate the short.


The case study began by examining No Power boards in order  to isolate the faults creating this condition. Each power rail  was examined for nominal voltage values. Power rails such as  3V, 1.5V, and 3V Standby were found to be shorted. Because  of power sequencing requirements, any of these shorts were  able to prevent the mother boards from turning on.


Fault Categories


Pareto Analysis:


Part of the EFA process includes the examination of various  Pareto items2. The failure system Pareto was divided into  several root cause Paretos (Figure 2.):


## System Failure Analysis Process and Case Study


26


Autu DnX


哺


tuSoN saN OH


nev


005 0030802OZYIsoro00


PO Slol


niw


eka90 580II081AT GNI


0231


U9F1


U1J1


ERIADU7A2


80%15%5%


LAN


3VVideoUSB ESD StandbyHo1


EPROM


ICH


SIO


PHY


d94YfXu 5F


Plug


V_3P3_STBY


Figure 2: Pareto Chart


V3PC ST8Y


ghIN OUT0902jamOJTVPSINGLE,U9G1


a. USB ESD Failures: due to signals shorted to ground on  the Universal Serial Bus. Failure analysis revealed that  this was caused by ESD (Electro Static Discharge) on the  USB connector. The ESD was moving onto the USB  connector, through the USB signals into the USB  Controller and shorting the power pins to ground.


b. Graphic EOS Failures: FA determined that the video  lines were shorted to ground. The cause of this was  determined to be due to a condition called hot plugging. Hot plugging is where a cable is connected while there is  still power on the signal path going through the cable. During this action an inductive spike occasionally  damaged the video controller through the analog video  signals. The result of the damage was power rail shorting  to ground and resulted in an Electrical Overstress (EOS) condition.


c. 3v Standby Line Failures: The third and most  significant failure Pareto appeared to be very random and  did not have the same failure mechanism. This pareto  became very intriguing since it was the major contributor  to NO Power failures returning from the field.


The Unified Data Stream concept is scalable to track and  provide the same high integrity data for any component within  and outside of the PC industry. The key is to establish  structure around the base aspects that UDS comprises: the  metric and indicator set, the data sources and their reporting  processes, verification of that data, indicator response  guidelines, and a quality system that is committed to act on the  data that is presented. The purpose of UDS is to demonstrate a  system that reflects trends and how those trends can be  mapped over time. Critical touch points need to be identified  and tracked and the data needs to be aligned to a consistent  date stamp. The net result is an effective quality operating  system fueled with the right information at the right time to  drive corrective action.


Acknowledgements


The authors would like to thank the members of the Unified  Data Stream Team for their dedication and continuous support  of the process that delivers timely and actionable information  for the purpose of improving product quality: John Blacker, Kevin Dunder, Robert H. Ellis, Kunaseelan Govindasamy, Neil Grant, Lynette Harmoning, Cang Ho, Siew Kiaw Tan, and Chris Wagner.


Component Defect Rates at Product Launch


Product A Verified Defect Rate


Product B Verified Defect Rate


Quality Goal


Product  Launch


Board Mfg Pilot  and Ramp


Board High Volume  Manufacturing


[1] Lane, Michael; Bjork, Roger; and Birdsley, Jeff , “Making Failure Analysis a Value Add Proposition in  today’s High speed Low Cost PC Environment”, ISFTA  Proceedings, Nov 2002.


[2] Schneider, John “A Brief Explanation of Sampling for  Paretos”, Intel Corporation, Hillsboro, Oregon.


Quiescent Signal Analysis (QSA) is an IDDQ method for detecting defects that is based on the analysis of multiple simultaneous measurements of supply port IDDQs. The nature of the information in the multiple IDDQs measurements also allows for the localization of the defect to physical coordinates in the chip. In previous work, we derived a hyperbola-based method from simulation experiments that is able to “triangulate” the position of the defect in the layout. In this paper, we evaluate the accuracy of this method using data collected from 12 chips fabricated in a 65 nm process.


Diagnosis is a process designed to identify the location of the fault in chips that have failed in the ﬁeld or at production test. It is a key component of failure analysis. The information gleamed from failure analysis is used to tune the fabrication process for the purpose of improving reliability and yield.


Hardware-based fault localization is challenged by increases in chip complexity as well as additional interconnection levels and the limitations on the spatial resolution of imaging technology [1]. The increase in difﬁculty and cost of performing hardware physical failure analysis is likely to move it into a sampling/veriﬁcation role. These trends continue to increase the importance of developing alternative software-based fault localization procedures.


Several “software-based” diagnostic methods have been proposed based on IDDQ measurements [2-9]. These methods can be classiﬁed as static, quasi-static and dynamic diagnostic test paradigms. For static, the diagnostic test set and test response are precomputed and stored in a fault dictionary. The quasi-static paradigm, the test set is pre-computed but the fault dictionary is eliminated. Instead, the test response is computed dynamically. Under the dynamic paradigm, both the diagnostic test set and response are computed dynamically during response analysis.


The QSA method that we propose in this work is a new approach to diagnosis and cannot be classiﬁed under these paradigms. It is complementary to these strategies and can be used in combination with them as a means of further improving diagnostic resolution. Moreover, QSA is more robust to the detrimental effects of increasing background leakage currents than these methods. This is true because, in QSA, the individual supply port currents are measured, in contrast to the global(chip-wide) IDDQ measured by other methods. The partitioning of the global leakage current across the multiple supply ports of the chip reduces its magnitude in each of the supply port measurements.


In previous works, we developed statistical defect detection and localization methods using simulation experiments. In[10], a hyperbola-based diagnostic method is proposed that is able to “triangulate” a defect’s location to a physical position in the layout of the chip. The method accomplishes this by computing the parameters for a pair of hyperbolas from the IDDQs measured at neighboring supply ports. The intersection of the hyperbolas identiﬁes the predicted location of the defect in the layout.


A calibration circuit (CC) is proposed in [10] as a means of solving several problems associated with this type of localization scheme. Calibration circuits are inserted into the design at positions directly beneath the supply ports, and through scan chain control, allow for the controlled insertion of a short between the power and ground rails. The supply port IDDQs measured under the calibration tests establish upper and lower bounds on the hyperbola parameters and allow the equations to be solved. Secondly, the CC data is used to calibrate the supply port IDDQs measured under a failing IDDQ pattern. Calibration reduces the detrimental effects on resolution caused by non-uniformities in the resistance of the power supply connections to the chip.


In this work, we elaborate and expand on the method described in [10] and evaluate its accuracy on 12 copies of a test chip.


The test chips are fabricated in a 65 nm, 10 metal layer technology and incorporate an array of test structures that allow a


Triangulating to a Defect’s Physical Coordinates Using Multiple Supply Pad IDDQs:Test Chip Results


Jim Plusquellic*, Dhruva Acharyya, Mohammad Tehranipoor and Chintan Patel


Dept. of CSEE, UMBC, Baltimore, MD 21250


plusquel, adhruva1, abhishek, tehrani, cpatel2@umbc.edu


*Chips designed while on sabbatical at IBM Austin Research Laboratory


## Triangulating to a Defect's Physical Coordinates Using Multiple Supply Pad IDDQs: Test Chip Results


defect to be emulated in one of 4,000 distinct locations on the chip. The design permits control over the magnitude of the emulated defect current and leakage current. The results of our analysis show that most defects can be located to a region less than 100 microns in diameter.


Test Chip Design


A block diagram of the test chip design is shown in Fig. 1a. It consists of a 80x50 array of test circuits (TCs) that occupies an area 558 microns wide and 380 microns high. Each TC consists of three ﬂip-ﬂops (FFs) connected in a scan chain conﬁguration, a shorting inverter, and a defect emulation transistor connected to a globally routed defect emulation wire. Fig. 1b shows a schematic diagram of two adjacent TCs. The shorting inverters and defect emulation transistors within each TC connect to the same point on the power grid.


The connection of the shorting inverters and the defect emulation transistors to power grid point sources enables introduction of two types of shorts in any one of the 4,000 TCs. Theﬁrst type shorts the power grid to ground through the inverter using FF1 and FF2; the second type shorts the power grid to the defect emulation wire using FF3. For the ﬁrst type, the external PWR supply voltage (see Fig. 1b) deﬁnes the shorting current’s magnitude.1 For the second type, an external voltage source(Defect source) controls the shorting current’s magnitude.


Given this conﬁguration, a defect can be emulated at any point in the array by setting the defect source to a value less than the PWR supply voltage and scanning a bit pattern into the scan chain such that exactly one FF3 contains a 0 and the remaining 11,999 FFs contain 1s.


In addition to controlling the magnitude of the defect current,the defect source inﬂuences the background leakage current’s magnitude, as measured through the PWR supply. As Fig. 1b shows, the total leakage current can be decomposed into two types, Ileak_i (inverter) and Ileak_d (defect). Given the defect emulation wire connects to the drains of 4,000 defect emulation transistors, only one of which is enabled in a particular experiment, the remaining 3,999 transistors sink leakage current from the PWR supply proportional to the magnitude of the defect source voltage. This leakage, Ileak_d, adds to the leakage current already present through the shorting inverters, Ileak_i.


Therefore, we can analyze a variety of shorting and leakage current conﬁgurations by controlling the states of the defect emulation transistors and voltage on the defect emulation wire.


Figure 2 shows the external instrumentation setup. Power ports V00 through V11 wire out of the chip on separate pins in the package. The individual power pins are each wired to a low resistance mechanical switch as shown along the top portion in Fig. 2. The switch can be conﬁgured in a left or right position.


1In our experiments, we held the PWR supply constant at 0.9 V.


Figure 1: (a) Block diagram of the test structure and (b) and test circuit (TC) details.


558 um


V00 V01


V10 V11


80x50 array


380 um


of TCs


TC0,0


TC49,0


TC0,79


TC49,79


inverter


shorting


FF1 FF2 FF3


+-


emulation defect


PWR


→+


Defect source


defect


emulation


六▼


transistor


supply


grid


wire


2 TC subset of the 80x50 array


0.9V


Ileak_i


Ileak_d


Figure 2: External Instrumentation Setup.


SUBSTRATE


PWRgrid


GNDgrid


Defect emulation Each transistor


by a scan FF


1010metallayers


V00


controlled


Source Meter


V10


-


mechanical switches


Global Current


Defect emulation


V11


AmmeterLocal Current


The left and right outputs of the switches connect to a common wire that routes to the global current source meter (GCSM)and local current ammeter (LCA), respectively.


0.32


The GCSM provides 0.9 Volts to the PWR grid and can measure current with a resolution less than 100 nA. The LCA is


0.3-


wired in series with the GCSM and allows measurement of the individual power port (local) currents at the same level of reso0.28


lution. For example, the switch conﬁguration in Fig. 2 allows


8 0.26


measurement of the local V00 current, I00, as well as the global


current. The defect emulation source meter (DESM) sets theI0u0.24 voltage of and measures current Idef through the defect emula0.22


tion wire on a separate pin in the package (not shown).


Power Grid Characterization Experiments


0100200300400500 0200300


We designed the ﬁrst set of experiments to determine how power grid resistance inﬂuences local currents’ magnitude. In these experiments, we disconnected the defect emulation wire,disabled the defect emulation transistors, and used the shorting inverters instead to provide stimulus to the grid.


We enabled each of the 4,000 shorting inverters from one of the chips, one at a time, and measured the global and local currents. Because we are interested in characteristics of the grid resistance and its inﬂuence on the local current distributions from layout point sources, we also performed the following steps. After testing each array element, we disabled the shorting inverter of the TC under test, measured the global and local leakage currents, and subtracted them from the values measured with the shorting inverter enabled. We then normalized these current differences by dividing them by the global current. This type of normalization virtually eliminates variations in the transistor current magnitudes introduced by process variations.


Figure 3 shows the current proﬁle derived from the normalized local currents, Inorm_00. The x- and y-axes represent the (x, y)plane of the TC array and the z-axis represents Inorm_00. Local currents are largest near V00 because TCs near this location draw a larger fraction of their current from V00 (maximum is approximately 31percent) than TCs further removed. The range of values of approximately 11 percent shows the effect of grid resistance on current distribution to the VDDs.


The smooth monotonically decreasing nature of the surface in Fig. 3 provides important “local” information that can be leveraged for detecting and localizing defects. Although we do not show the current proﬁles for the remaining three VDDs, the same characteristic shape exists in their surfaces; only the orientation is different. A key feature present in these proﬁles is the one-to-one mapping between the supply port IDDQs and the position of the enabled TC in the 2-D array.


The unique mapping relationship between layout position and the corresponding IDDQs enables a simple scheme for defect localization based on a lookup table. The lookup table maps


discrete positions in the layout to sets of supply port IDDQs.


The lookup table can be derived from simulation experiments and fast power grid simulators, such as ALSIM [11]. We present results of applying this technique to a set of chips in


[12]. In this work, we investigate a method based on an analytical model. We predict defect locations using only the measured IDDQs, and therefore a lookup table is not needed.


In either method, the accuracy of the localization methods are greatly improved by correcting for resistance variations in the power distribution systems of the chips. In previous work, we developed and demonstrated a calibration method capable of signiﬁcantly reducing the adverse impact of these types of variations [12] and [13]. This method is applied to the IDDQ data analyzed in this work.


Current Fraction Contour Analysis of the Power Grid


The smooth surface of the current proﬁle shown in Fig. 3 suggests that normalization, i.e., division by the global current, is effective at eliminating current magnitude as a parameter in the characterization of the power grid’s resistance. The elimination of the current magnitude parameter is also a desirable characteristic in a defect localization algorithm, i.e., the magnitude of the defect current should not inﬂuence the position predicted by a localization algorithm. In previous work, we demonstrated the effectiveness of a local form of normalization, in which the supply port IDDQs of neighboring VDD ports are used to compute a current ratio, e.g. I00/I01 [10]. Unfortunately, current ratios introduce non-linearity in the analytical model that complicates matters. An alternative that provides the beneﬁt of normalization and near linearity is to compute current fractions,e.g., I00/(I00 + I01).


Figures 4 and 5 plot the current fraction contours of chip C1 for VDD port pairings V00-V01 and V00-V10, respectively. The x-y plane represents the TC array. The lines within each plot delimit the iso-current fraction regions, i.e., positions in the Figure 3: Inorm_00 proﬁle.


x-coordinate


100y-coordinate


layout that posses a similar current fraction. The current fractions are computed as I00/(I00 + I01) in Fig. 4 and as I00/(I00 +I10) in Fig. 5.


An analytical model capable of describing these curves is complicated and must take into account the inﬂuence of all VDD ports in order to be complete. However, the behavior of the curves in the region surrounding the V00 supply port, identiﬁed as quarter Q0 in the ﬁgures, is less complex and appears quadratic in nature. Analytical models based on ellipses and hyperbolas are candidates for describing the curves in these regions.


Our analysis to date has determined that hyperbolas more accurately approximate these curves but our work in this area is on-going.


Hyperbola-based Model


Equation 1 and Figure 6 deﬁne and illustrate horizontally-oriented hyperbolas, as a model for the contours curves shown in region Q0 of Fig. 5. Vertically-oriented hyperbolas, appropriate for the curves shown in Fig. 4, are similarly deﬁned. The VDD ports V00 and V10 map onto the graph at the foci, labeled F1 and F2 in Fig. 6. The space between the foci represents the 2-D space of the TC array.


A key component to modeling the set or family of contour curves shown in region Q0 of Figures 4 and 5 is to deﬁne the relationship between them. Figure 6 deﬁnes an additional parameter c used to deﬁne the relationship among a family of hyperbolas designed to serve as models for the contour curves.


A family of hyperbolas is deﬁned as a set that share a common center and focus. The h and k parameters deﬁne the center of the hyperbolas, which corresponds to the midpoint between the foci.


x h–


)2


aa2


-------------------y k–( )2


b2


-------------------


–


The a and b parameters of Equation 1 shown in Fig. 6 need to be deﬁned in terms of the current fractions. However, the c parameter allows an alternative expression, Equation 2, that


eliminates b. Here, b2 is replaced with (c2 - a2). Parameter c is


constant for all hyperbolas in the family as the distance between their center, (h, k), and the coordinates of the power ports or foci. Therefore, only a needs to be deﬁned in terms of current fractions.


From the diagram shown in Fig. 6, a deﬁnes the point of intersection of the I00/(I00 + I10) hyperbola with the horizontal line deﬁned between the center (h, k) = (279,0) and V00 (F1 in theﬁgure). Therefore, a varies from 0, at the center, to L/2 at V00,where L is deﬁned as the distance between V00 and V10 (558 for the TC array). The current ratios at points along this line


a2


c2a2–-------------------


Figure 4: V00-V01 current fraction contours.


Figure 5: V00-V10 current fraction contours.


V0050100150200250300350400450500


150


Q0100 Q1250


Q2 Q3


Q2


Q3


V01


890


350


V0050100150200250300350400 450500 V01


Figure 6: Deﬁnitions of the hyperbola parameters


F1


F2


Horizontal Hyperbolas


279


558


center


(h, k)


increase from 0.5 at the center to a maximum current ratio, e.g.


0.60 for I00/(I00 + I10) near the V00 supply port.


Figure 7 shows the current fractions computed from chip C1 as each of the shorting inverters are enabled, one at a time, along the lines between V00-V01 and V00-V10. The x-axis represents the position of the enabled shorting inverter. The nearly linear shape of the curve reﬂects the uniform spacing of the contour curves along these lines in Figures 4 and 5. The linear nature of the curves allows a close approximation for a to be derived if the endpoints or bounds of the curves are known. Equation 3 can be used to derive a under these assumptions. Here, Iub and Ilb represent the upper and lower bounds on the current fractions at the endpoints and L represents the distance between the VDD ports.


A straightforward way of obtaining the upper and lower bounds, Iub and Ilb, is to embed calibration circuits (CCs) in the design at positions beneath the supply ports. For example, Fig.


1a identiﬁes four TCs in the array, TC0,0 through TC49, 79, that correspond to these positions. CCs are similar in design to the TCs shown in Fig. 1b, with only the shorting inverters present.


The upper and lower bounds are obtained by enabling each of the CCs, one at a time, and measuring the supply port IDDQs.


For example, the Iub and Ilb in Equation 3 for horizontal hyperbolas are I00 and I10 measured with TC00 enabled.


With the bounds deﬁned, defect localization is performed by calculating the parameter a for two pairings of orthogonally positioned VDD ports, e.g., V00-V01 and V00-V10. The a parameters are used in Equation 2 to derive a vertical and horizontal hyperbola. The intersection of the two hyperbolae


aL2-- L–Iub I00–( )Iub Ilb–( )---------------------------–   =


deﬁnes the predicted position of the defect in the layout.


IDDQ Defect Localization Experiments


These experiments are designed to investigate the accuracy of our defect localization methodology for defect currents and leakages that vary over a wide range of values. These objectives are better met through the use of the defect emulation transistors and corresponding defect emulation wire because both the position and magnitude of the emulated defect current can be controlled.


Data Collection Procedure


Unlike the power grid characterization experiments which tested all 4,000 elements of the TC array, these experiments tested only a 100-TC subset. Figure 8 shows the set of randomly selected TCs in the 80x50 array. The numbered positions are the TCs under investigation.


For each of the 12 chips, we performed a series of measurements for each TC under different voltage conﬁguration of the DESM--the source meter that drives the defect emulation wire.


The ﬁrst experiment for each chip is the leakage experiment. In this experiment, we set the state of all scan chain FFs to 1,which disables both the shorting inverters and the defect emulation transistors in all TCs in the array. We then swept the DESM across a sequence of voltages, from 0.9 V to 0.0 V in 50 millivolt intervals, for a total of 19 steps. At each DESM voltage, we measured a set of four local and four global currents through the supply ports. We performed the same operation sequence with each enabled defect emulation transistor, one at a time. The four local currents and four global currents from each experiment are referred to as a data set.


Data Sets and Quarter Selection Algorithm


For each chip, the data collection procedure produces 1,919 data sets, of which 19 represent leakage data and 1900 (19 *100 emulated defects) represent data from the emulated defect experiments. However, the emulated defect experiment with the DESM voltage set to 0.9 V is not meaningful because there is no voltage drop across the defect emulation transistor.


Therefore, we treat only 18 of the 19 data sets as emulated defects. With 12 chips, there is a total of 12 X 19 = 228 leakage data sets and 12 X 1800 = 21,600 emulated defect data sets.


For each emulated defect, we compute the position of the emulated defect by selecting a pair of orthogonally positioned supply ports. The supply ports selected are those surrounding the supply port with the largest measured IDDQ, called the primary port. The supply port with the largest IDDQ identiﬁes the quarter in which the defect lies. Figure 9 displays the four quarters of the TC array. For example, if I01 is largest in an emulated defect experiment, then V01 is selected as the primary port and V00 and V11 are selected as the orthogonal neighbors.


Figure 10 shows several examples of the method applied to predict the locations of emulated defects #0, #1, #4 and #28, as


Fri Feb 24 19:07:18 2006


-4.000


0.000 (1E+01) 4.000


8.000


12.000 (1E+01) 16.000


20.000


24.000 (1E+01) 28.000


32.000


36.000 (1E+01) 40.000


44.000


48.000 (1E+01) 52.000


56.000


60.000 (1E+01) 64.000


68.000


72.000 (1E+01)


40.000


41.000(1E-02)


42.000


43.000


45.000


fractioncurrent


46.000


47.000(1E-02)


48.000


49.000


50.000


51.000


52.000


53.000(1E-02)


54.000


55.000


57.000


58.000


59.000(1E-02)


60.000


61.000


62.000


63.000


64.000


65.000(1E-02)


66.000


67.000


69.000


70.000


Figure 7: Current fractions along lines between V00-V01 and V00-V10.


x and y coordinates of TC array


0.6


I00/(I00 + I10)


Fri Feb 24 22:38:36 2006


-4.900


0.000 (1E+01) 4.900


9.800


14.700 (1E+01) 19.600


24.500


29.400 (1E+01) 34.300


39.200


44.100 (1E+01) 49.000


53.900


58.800 (1E+01) 63.700


68.600


-2.300


0.000(1E+01)


2.300


4.600


6.900


9.200


11.500


13.800(1E+01)


16.100


18.400


20.700


23.000


25.300


27.600(1E+01)


29.900


32.200


34.500


36.800


39.100


|Q1 |Q3 |
|---|---|

|Q0 |Q2 |

41.400(1E+01)


43.700


identiﬁed in Fig. 8. For each of these emulated defects, two hyperbolas are derived, one vertical and one horizontal. The intersection of the hyperbola indicate the predicted location of the emulated defect (see defect #28 in the ﬁgure). The actual location is shown as a solid dot. The distance between the intersection of the hyperbola and the dot represents the prediction error.


Separating Defect Current and Background Leakage


The hyperbola-based localization algorithm maps the defect currents measured through each of the supply ports to an (x,y)position in the layout. Unfortunately, the currents measured also posses leakage current, which, if not subtracted, acts to“wash out” the current fractions described above and reduces the level of accuracy of the prediction algorithm.


One approach of eliminating leakage current from the measured values is through backtracking. This process is illustrated in Fig. 11. First, the leakage data from defect-free chips or simulations is used to build a proﬁle of the leakage relationship among the VDD ports. Regression analysis is applied to derive a slope of the best ﬁt line through the pair-wise plots of leakage data. For example, the graphs shown on the right side of Fig.


3v Standby Failure Defect Trend:


Early FI determined that all failures were due to power  shorting. A digital volt meter was used to confirm the power  rail shorts on the mother boards. Further examination  determined that the shorting was occurring within a  component on the board; however it was not always the same  device which clearly made it more difficult to determine the  true root cause. On some boards, only the PHY (physical  interface to the Ethernet) was shorted, on other boards the  ICH (I/O Controller Hub), and on others the SIO (serial I/O). In addition some mother boards had different combinations of  these 3 devices shorted out. Based on some preliminary  commonality analysis it was determined that all 3 devices  shared a common link – 3V Standby power. The circuit  diagram (Figure 3.) shows the common link and how these  devices tied back to the 3V Standby power line. It shows that  each of these components was sourced by the 3V Standby  power rail.


Figure 3: Common Link for Three Components


Investigation


The FA team hypothesized four possible causes that could  create a large current sink on the 3V Standby pins:


a. Voltage Feed Through (VFT)


b. Electro Static Discharge (ESD)


c. Defective Silicon


d. Over Voltage


Voltage Feed Through: VFT can occur during initial power  sequencing when two different power rails on a single  component can sequence at different times. For example, 5V  on a component can initially feed through to the 3V power  pins on the same component right after power is turned on. If  5V is on the 3V pins too long, the 3V pins can short to  ground. This hypothesis was eliminated by observing initial  power on timing with an oscilloscope.


Electro Static Discharge: ESD can be transferred by an end  user touching a personal computer mother board. The user  could either transfer high voltage static through front panel  connectors, or open the PC case and touch the mother board  itself. The ESD hypothesis was eliminated for three reasons: a. If a PC user accumulated a dangerous amount of static, the mother board is protected by a Faraday Cage (i.e. the  case); hence if ESD from an open case was the cause it is  unlikely it would have been specific to these 3 devices.


b. Secondly an ESD gun was used to create EOS through  the external Ethernet connector. This did not cause  shorting to the 3V Standby pins on the PHY. The PHY is  actually protected through the transformer. The  transformer provides isolation between the PHY and the  outside of the front panel connector.


c. Finally, the ESD gun when directly applied to the mother  board was used to cause 3V Standby shorting. But this  showed random type failures.


Defective Silicon: Defective silicon could arrive directly from  the supplier and placed on the mother board during assembly.


If this were the case, most of these boards would be caught  during the testing phases of the assembly process. It was noted  that not one board with a 3V Standby short in the PHY, SIO, or ICH was observed from any of the factories that are  responsible for assembly. This problem was only seen from  boards returned from end users. A significant amount of time  occurs from the assembly and testing of the board, integrating  it into a chassis, testing the entire PC, and being powered by  the end user. If defective silicon were causing a No Power  condition, it is likely that the PC would have never arrived to  the end user. In addition, it is also unlikely that three different  components produced by two different suppliers would all  have the same silicon defect. A sample of each component  was sent for silicon failure analysis. The results of the analysis  for each device revealed electrical overstress caused externally  to the part. The Defective Silicon hypothesis was eliminated. Over Voltage: The final hypothesis was that there was an  over voltage condition taking place. The team approached this  hypothesis from two different directions – empirical analysis  and theoretical simulation.


The empirical examination was not exact given the difficulty  of reproducing the precise conditions by the end user. Therefore indirect methods were used to verify the over  voltage hypothesis. First, it was demonstrated that noise could  be generated on the 3V Standby rail –not consistently, but  occasionally. Second, it was demonstrated that an over voltage  condition applied to the 3V Standby occasionally caused  shorts.


The theoretical simulation was derived from Ohm’s Law3 (Figure 4.) Assuming that the silicon was functioning as  expected then Z (impedance) in the device is held constant  under nominal load, or stays within range under dynamic load. Since Z does not short under normal operating condition and  bus activity cannot sink enough I (current) beyond operating  specifications of any of the devices, then V (voltage) would  have to change in order for electrical overstress. Since I=V/Z, then V must increase in order for I to increase. If the increase  in current is beyond the specifications of the component, then  Z can decrease to a zero ohm or close to zero ohm condition.  Ohm’s Law  V=IR


Figure 4: Ohm’s Law


This theoretical model was simulated by first booting a mother  board. The mother board was then switched to a sleep state. During the sleep state 3V Standby power remained active as  expected. Under these conditions, the load (produced by the  SIO, ICH, and PHY) on the 3V Standby Line was constant, and therefore Z was constant. Applying voltages greater than  4V to the 3V Standby rail increased current as predicted by  Ohm’s law. This increase in current overstressed the PHY  which lowered its Z close to zero Ohms. Therefore, the  shorted power pins on the PHY held the 3V Standby power  rail to zero Volts creating a No Power condition. The No  Power boards were the target Pareto item for the case study.


3V Standby Protection: A comparison was made between  the 3V Standby power rail on mother boards and the other  power rails on mother boards. It was noted that the other  power rails had more protection on them. For Example the  ICH is one of the components that receive 3V Standby EOS  on its 3V Standby power pins but not as much EOS on its


1.5V pins. The 1.5V pins have more protection (Figure 5.)


Figure 5: Circuit Protection for 1.5V but not for 3V Standby


But the 3V Standby power pins are sourced through a linear  regular from the external power supply (Figure 5.)


Design Change: A solution was derived to protect the 3V  Standby rail from an over voltage condition (Figure 6.) The  total cost was calculated based on exposure and rate of failure  and based on the cost of the solution. A positive ROI (Return  on Investment) was achieved. The FA team lead the effort to  get this changes incorporated in all future designed by  leveraging tools such as Engineering Advisories and Design  for Reliability guidelines.


Figure 6: Solution for EOS Protection


Summary


Conclusion


This case study performed by a Field Failure FA team shows  the importance of disciplines and well structured process in  identifying a common failure mechanism even though the  failure mode was different. This case demonstrated a sound  process for examining quality issues in response to customer  demand. It indicated how the FA process can be used to save  money by identifying failure trends and taking corrective  action. And finally it provides solutions and recommendation  to influence and direct the solutions path in order to affect the  PC industry.


The authors would like to thank the members of the Intel  Boards Failure Analysis Team for their dedication and  continuous support of the process that delivers timely and  actionable information for the purpose of improving product  quality: Mike Winscott, Pete Nicholas, and Orlando Diaz.


[1] “Case Studies of IR Based Rapid PC Motherboard  Failure Analysis” J. Swart, J. Woo, R. Zumwalt, J. Birdsley, Y. Taffese - ISTFA Proceedings, November  2002


[2] “A Brief Explanation of Sampling for Paretos” Schneider, John, Intel Corporation, Hillsboro, Oregon.


[3] “Electric Circuits” J. Nillson, S Riedel – AddisonWesley 1996.


[4] "Parameter Extraction and Electrical


Characterization of High Density Connector Using


Time Domain Measurements"  S. Pannala, A. Haridass, M. Swaminathan, —IEEE Transactions On Advanced


Packaging, Vol. 22, No. 1, February 1999.


[5] “Guideline for Measurement of Electronic Package


Inductance and Capacitance Model Parameters”—


JEDEC Publication #123, JC-15 Committee, October


1995.


[6] “Measuring Controlled-Impedance Boards with TDR” M.D. Tilden, “Measuring Controlled-Impedance Boards  with TDR,” – Printer Circuit Fabrication, February 1992.


[7] “Solder Joint Reliability of BGA, CSP, Flip Chip and  Fine Pitch SMT Assemblies,” McGraw Hill (1996)


[8] “Making Failure Analysis a Value Add Proposition in  today’s High speed Low Cost PC Environment”  Lane, Michael; Bjork, Roger; and Birdsley, Jeff , ISFTA


Proceedings, Nov 2002.


Using a Unified Data Stream to drive Failure Analysis for Product Improvement in the  Personal Computer (PC) Environment


Shirleen Horley, Joseph Rascon


Intel Corporation, Hillsboro, Oregon, USA  Intel Corporation, Chandler, Arizona, USA


The longer defective units are in the manufacturing pipeline  before they are detected, the more expensive it becomes. Economic pressures drive the requirement to capture failures  and perform root cause analysis further upstream in the  product manufacturing cycle. This places greater emphasis on  the ability to identify failures and perform value add analysis  to drive product improvements as early as possible. This paper  describes the method used to develop a reliable Unified Data  Stream (UDS) that feeds the failure analysis process which in  turn provides actionable information to product development  teams in the Personal Computer (PC) environment.


■□


This manuscript describes the development and


Component BComponent D


Component AComponent CComponentEComponentComponentF GComponent HComponentComponent IComponentK JComponent LComponent M


implementation of the Unified Data Stream designed to  replace ambiguity and uncertainty with a defect trend and  symptom pareto that drives action upstream. Focus will be on  the output of UDS enabling the prioritization of product  defects that feed the failure analysis system. Additionally, this  paper will touch on the application of the UDS system for  different types of pc components. The future of UDS is  without bounds as it can also be applied to a wide range of  products.


Certain components were not meeting quality goals and had  become significant contributors affecting motherboard quality [Figure 1]. The outgoing monitor indicated component quality  was at or just above goal but due to configuration and  application differences the outgoing indicator was not  accurately reflecting customers’ experience. In addition, customer data streams were reporting conflicting information [Figure 2]. Design and quality teams were bombarded by  competing and confusing data; too much time was being spent  trying to understand the data rather than act on it. The quality  system had become focused on reacting to issues rather than  driving product quality improvement.


0%5%10%15%20%25%30%35%


Contribution to Defect Rate


40%45%50%


Defective Material Pareto


Figure 1. Top contributors to motherboard quality.


Outgoing Monitor vs. Customer Experience


0 200 400 600 800 1000 1200 1400 1600 1800 2000


Outgoing Monitor


Customer A


Customer B


Goal


Figure 2. Outgoing monitor not reflecting customers’ experience.


The solution required the ability to deliver a single set of  indicators to drive focused improvement in product quality. Intel’s response was the formation of the Unified Data Stream  Team.


## Using a Unified Data Stream to drive Failure Analysis for Product Improvement in the Personal Computer (PC) Environment


Establishing a Unified Data Stream


The team’s goal was to provide high confidence product  performance data to facilitate decisions for continuous product  improvement, in short, “Timely Actionable Information1.” Their strategy was to thoroughly assess and understand the  processes that deliver the data, and establish confidence in the  results.


Using a holistic approach to identify product failures, the team  worked with component suppliers, motherboard  manufacturers, and system integration sites to collect a full  spectrum of reported failure data points [Figure 3]. On the left  side, test points from silicon wafer start through final test are  illustrated in this high volume manufacturing flow chart. Strategic points to collect failure data are shown on the right. The UDS team evaluated each data source that supplied  failure data to understand the methods each source used to  validate their reported failures. A verification test suite was  used to test all reported failures on internal logic and  functional test platforms. The end result was a verified failure  pareto.


Figure 3: Data extract points within High Volume  Manufacturing Test Flow.


Generating High Confidence Data


A questionnaire was distributed to each of the motherboard  assembly factories that were reporting factory line fallout. Responses to the questionnaire were used to evaluate each  site’s product test flow through in-circuit test, functional test, and final outgoing test. In addition, the questionnaire inquired  about each site’s debug process, on-site validation method, and the information each motherboard assembly factory used  to report a component failure. Team members also traveled to  the various factories for on-site assessment and data gathering. The team identified many similarities in the methods deployed  by each factory, and uncovered several differences that  required further investigation.


For example, each motherboard assembly factory agreed a  reported failure to be defined as a functional test failure that  was debugged to component where replacing the component  caused the board to pass functional test [Figure 4]. However, each factory’s method of tracking and ensuring the replaced  components were sent for verification testing was different. Some factories used a more sophisticated automated system to  track the replaced components, whereas others relied on a


Water Starts


manual process.


Wafer Sort Test internal logic test)


yssawqjA9 gluejj as1


Data Extract Point 1a


]luqoaj] 05101551(


Companent SupplierOutgoing


Figure 4. Process flow to determine reported component


douuA o


failure.


)nuonoueje s1(


Data Extract Point 1b


syd10g oeup cunpnJ


Each motherboard assembly factory also classified component  replacements due to functional test failures as either


snueoaw onux M6AeS OIPeJ


component defects or process defects. However, some  factories employed a validation process involving a variety of


UD O1 0SI


hardware and software to make that classification. There was  risk the motherboard assembly factories’ on-site validation


Motherboard


Data Extract Poin12Motherboard


tests could be passing defective components. The differences


Functional Test


Functional Fails


between motherboard assembly factories were determined to


Ship to System


impact the number of failures reported per week and the


Intagration Site


number of units shipped to for verification, which ultimately  affected the integrity of the data.


System Level Tests(final assembly.


Data Extract Poin1 3


final burn-in,


Falls


System Level


final functional tests)


Therefore, based on their findings, the team developed


Ship to


equivalency criteria for including a data source in the unified


End User


indicator package. General requirements were defined to  ensure each data source followed a similar reporting process.


Field Falures


Data Extract Point 4Field FailuresEnd User


Detailed criteria for reporting a failure were defined in order  to assure equivalent indicators from multiple reporting sites.


A statistician was consulted to determine the minimum  average weekly consumed volume for the targeted component, and the required number of units randomly selected from the  reported failures for verification testing in order to produce an  actionable pareto with 90% confidence. Volume impacts the  confidence of the data; therefore the preference is to go with  higher volume sources. Essentially, the higher the sampling


M B  P ro cess


M B  passes


Yes


Fail


No


No t a Repo rted  Failure


Functio nal


Test


Replace


Co mpo nent支


Debug to   Co mpo nent  defective


Repo rted Failure


No rmal P ro cess


P ass


with new


Co mpo nent?


ratio, the higher confidence the top issues identified are the  true top issues. However, the key is to determine the smallest  sample size required to accomplish the sampling objective2.


As part of the assessment of the factories on-site validation  tests to classify reported failures, the team used JMP, an  interactive statistical analysis tool, to calculate the maximum


Defect Rate


number of false passes that would be permitted without  negatively impacting the 90% confidence of the data. Correlation analysis was performed using units that pass each  factory’s on-site validation test. Factories were required to  demonstrate their on-site validation test would be stable over  time and maintained under a change control process to assure  hardware and software configuration will not change to  increase the probability of passing defective components.


How The Data Is Charted


It is the ability to unify the data by taking an aggregate of  several data sources (several component manufacturing sites, several board manufacturers, etc.) and producing a  representative set of indicators that feed the quality operating  system. In this example, the indicators include the following: Component Outgoing Quality, Motherboard Manufacturer and  Customer Reported Failures, Verified Failures, System  Integration Line Reject Rate (LRR), Verified Line Reject Rate (VLRR), Field Incident Rate (FIR), and Verified Field  Incident Rate.


Using volume weighted averages, data from several sources  are combined to represent one indicator package. The first  three indicators listed above are consolidated into one trend  chart that is updated and presented to quality forums on a  weekly basis. Figure 5 is an example representing outgoing  quality (solid green line) as the calculated predicted indicator, reported failure trend (dotted red line) as the motherboard  manufacturing factory line fallout for a component, and  verified failure trend (dashed blue line) as the results of  component verification testing. All data points are aligned to  the week the product was consumed at the motherboard  manufacturer and reported as a failure. In this example, the  reported failure trend represents a significantly higher defect  rate as compared to the outgoing quality monitor or the  verified defect trend. Such a gap drives internal investigation  to identify potential test holes in the verification process. Information regarding the reported failures that comprise the  gap is also communicated to the board manufacturer(s) to  determine cause for reporting false failures.


Sample of Aggregate Indicators for a Component


0 200 400 600 800 1000 1200


Reported Trend


Verified Trend


Figure 5. Example of Aggregate Indicator trend graph for a  Component. Using volume weighted averages, data from  several sources are combined to represent one indicator  package.


UDS was able to leverage data from existing failure analysis  programs that were established to report and verify  motherboard failures at system integration and in the field. At  product launch, a sufficient quantity of failures across the  range of symptoms is selected for failure analysis to establish  a comprehensive picture of product quality. Opportunities for  quality improvement are developed by monitoring system  integration and field returns data and selective sampling of  symptoms that likely contain new issues not previously  investigated. The sampling is based on the top pareto items  from the verification testing as well as the performance of  each product to goal.


Through the failure analysis process, component contribution  to a specific motherboard’s VLRR is identified and graphed. System integration failures are typically identified four to six  weeks after motherboard assembly and test. Field failure data  is collected ninety days after system shipment, and verified  within two months following data collection. System  integration and field failure data is also included in the UDS  data package.


Figure 6 is an example of Verified Line Reject Rate for a  motherboard product represented in a bridge chart. The bar  furthest to the left is VLRR for a specific timeframe (typically  one month), and the bar furthest to the right is the VLRR goal  for that timeframe. This bridge chart is used to highlight the  top contributors to VLRR that are affecting overall board  quality. If any one of the identified components in the bridge  chart is the same component being tracked by UDS, that  component’s contribution to the VLRR defect rate is included  in the UDS package.


Delect Rate


VLRR forspecifiedtimeframe


DefectiveComponent A


DefectiveComponent


RandomDefects


Figure 6. Example of VLRR bridge chart.


Figure 7 is an example of taking the failure rate for Defective  Component A (from Figure 6) and tracking it over time. The  component failure rate is graphed as a bar chart showing the  trend over time as compared to that component’s quality goal. This bar chart is used to identify the timeframe when the  component’s defect rate changes either increasing above or  decreasing below the component’s quality goal. Analyzing a  component’s defect rate over time enables the the quality  system to respond to defect rate increases and monitor defect  rate decreases once resolution has been implemented.


Example of Component Contribution to MB Failure Rate over Time (bar graph)


Tim e


Component  Defect  Rate


Figure 7. Example of Component Defect Rate bar chart.


Figure 8 is an example of taking Defective Component A (from Figure 6) and identifying the first level failure pareto  graphed as a bridge chart. The component’s contribution to  motherboard failure rate is analyzed to first level root cause to  detect trends and isolate any new issues that were not  recognized during board manufacturing.


Figure 8. Example of Component Contribution to VLRR  failure pareto (bridge chart).


To provide an overall view of component quality, the VLRR  bridge chart [Figure 6], the bar graph representing a specific  component’s contribution to VLRR over time [Figure 7], and  the first level failure pareto bridge chart [Figure 8] are all  incorporated into the UDS reported data.


Example of VLRR Bridge Chart


Figure 9 is an example of Verified Field Incident Rate for a  motherboard product represented in a bridge chart. The bar  furthest to the left is VFIR for a specific time frame (typically  three months), and the bar furthest to the right is the VFIR  goal for that time frame. This bridge chart is used to highlight


Postresolution


VLRR Goal


the top contributors to VFIR that are affecting board  reliability. If any one of the identified components in the  bridge chart is the same component being tracked by UDS, that component’s contribution to the VFIR defect is included  in the UDS package.


HISA


10.381


23


08


is18


Example of VFIR Bridge Chart


Figure 9. Example of VFIR bridge chart.


***


The objective of these graphs is to track different touch points  of a specified component’s contribution to board quality.


How The Data Is Used


Today’s UDS breakthrough system involves cross functional  and cross-geographical team members focused on identifying  product issues and driving action to meet the established  product quality goals. The team developed indicator response  guidelines to be used when analyzing data from all sources  The combined component information is reviewed weekly by  the UDS team. Actions are assigned to individual team  members to further investigate specific reported and verified  data points that exceed the limits documented in the response  guidelines. For example, when evaluating a reported failure  rate that is less than the goal, an investigation is required when  the nominal value increases for three consecutive weeks. Another example, when comparing the verified failure rate for  two sites that are reporting the same product, an investigation  is required when the upper and lower confidence intervals for  one site does not overlap the nominal value for the other site. This indicates statistically different results for the same  product.


Once the data is examined by the UDS team, it is prepared for  presentation to the quality forums. The individual trend charts, bridge charts, and bar graphs are organized into a PowerPoint


Example of Component Contribution to MB Failure Rate (bridge chart)


Component Contribution to VLRR


Issue A


Issue B


Issue C


presentation. The aggregate volume weighted averages for  each product’s verified failures are used to generate failure  paretos comparing the outgoing monitor with customer  verified failures [Figure 10]. The resulting symptom pareto  functions to prioritize top issues for root cause failure analysis  and generational product improvements. Failure categories are  used to give an understanding of the trend, but do not always  imply the same root cause. In this example, the verified failure  defect rate for Category A is greater than the outgoing monitor  for that category. Such information would drive investigation  into possible latent or induced defects downstream from  component manufacturing. Categories F and G represent an  issue that isn’t being captured at outgoing and would drive  investigation into possible test holes. In each of those two  categories, the failures are contributing to a common symptom  not captured by test.


Figure 10. Example of a failure pareto for comparing  outgoing monitor to verified defect rate representing  customers’ experience.


The verified product defects from each of the data sources are  used to feed the failure analysis system with a prioritized list  of top issues. The high confidence data ensures a failure  selection process that yields actionable failure analysis results. Based on the failure data, a representative sample of customer  returns that fail the outgoing tests are processed through unit  level failure analysis for the purpose of performing root cause  electrical fault isolation and physical failure analysis at the  component level. The failed units undergo electrical  characterization which uses signature analysis to classify the  failure type. A decision is then made to perform either DC  parametric, functional, or package failure. Electrical fault  isolation enables the failure to be localized down to an  individual or limited number of potential failing nodes. Sometimes, physical failure analysis requires destructive  mechanical de-processing for isolating the failure to a specific  circuit element. Unit level analysis is utilized to obtain enough  information about the defect to trace it back to a root cause  and drive corrective action [Figure 11].


O utgo ing  M o nit o r v s . V e rif ie d F a ilure  P a re to  f ro m  C us t o m e r D a t a


C at egor y  A


Cat egor y  B


Cat egor y  C


Cat egor y  D


Cat egor y  E


Cat egor y  F


Cat egor y  G


F a ilure  C a t e go rie s


Out going Monit or


Ver if ied Fai lure Rat e f rom Cust omer Dat a


Figure 11. Example of component failure analysis findings; scan of a connect in silicon.


In this example, the failure mode was determined to be  missing salicide in NMOS. The component level failure  analysis data identified the focused area that enabled the  component manufacturer to drive improvement and address  this marginal manufacturing problem. The results of unit level  analysis that point to component manufacturing process  defects are submitted to the appropriate engineering teams for  closed loop corrective action.


Customer returns that pass the outgoing tests are delivered to  the product engineering teams along with detailed failure data  for the prioritized top issues. With the participation of systems  validation and design engineers, root cause is determined and  new test patterns are developed to screen the defects from the  outgoing product. Test program improvement history is  tracked for future generational improvements.


All of this information including the failure data, the results  from root cause analysis, and the test patterns are delivered to  engineering product development teams and design for test (DFT) teams for future generations of products.


Results


In 2005, results from weekly analysis of the UDS information  were used to identify and drive action on multiple product  issues. Response to the UDS information has produced  extraordinary results, enabling improved quality goals at  product launch as demonstrated in Figure 12. The upper trend  line in Figure 12 represents the defect rate for a component  beginning at product launch to high volume manufacturing. The lower line represents the improvement in defect rate the  next generation product demonstrated after the UDS system  was implemented. This was a result of analyzing issues for the  previous generation, and taking corrective action in a timely  manner. As can be seen in Figure 12, the overall quality of the  next generation product is significantly improved and meets


goal. The issues were resolved prior to entry in to the  manufacturing pipeline.


Figure 12. Comparison of two generations of a product  beginning at their respective product launches.


Other benefits have been realized as an outcome of  implementing UDS.  Due to the integrity and timeliness of the  data, customer issues are quickly acknowledged and the  necessary information is forwarded to the appropriate  engineering teams.  Savings in time to resolution is results  oriented as the engineering teams are able to constructively  confront and solve issues that are quantified and analyzed.   Savings in cost is also accomplished as the data is used to  drive improvements in products, quality processes, and  methodologies.  Both have resulted in increased customer  confidence in product quality.


The UDS team took the challenge of obtaining product  performance data for the purpose of driving product  improvements and addressing quality issues. By consolidating  and verifying data from a variety of sources, UDS developed a  high integrity data stream that provides a holistic view of  individual component quality. UDS was designed to provide  Timely Actionable Information to feed the quality operating  system. Results of UDS have had a direct influence on failure  analysis, test-hole analysis and closure, and product design  improvements.


11 portray a hypothetical leakage relationship for VDD ports


Figure 9: Quarters, Qx, deﬁned for the TC array.


380


defect #0 defect #1


defect #4


defect #28


Figure 10: Example hyperbola based predictions of emulated defects.


Actual position


Predicted position


um


14


19


24


29


34


39


44


49


28


89


4 19 24 29 34 9 44 49 54 59 64 69 74 79


4 9 14 19 24 29 34 39 44 49 54 59 64 69 74 79


|1 74 |1 74 |||||||||||||||||||||||||||2 |2 ||||||
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|

|83 |83 |||||||||||||||||||||||39 |39 ||||||||||

|||||||||||||||||||||||||||||||||||32 33 |

||||||||||||||||||||||46 |46 |||||||||||||

||||||||35 |35 ||||||||66 |66 ||||||||||||||||||

|19 |19 ||60 |||||||61 |61 |||||||||||||49 |||||||||||

||||||18 ||||||||||||||||||||||||||||||

|||75 ||||||||||||||25 |25 ||||||||||||||||||

|6 |6 |76 |76 ||||||||||||||||||||||||||||||||

|10 96 |10 96 |||||63 |63 ||古|64 |64 |64 |64 |64 |64 |64 |64 |64 |64 |64 |64 |64 ||||||||68|98 ||||

||||78 |52 |52 |||||||||||||||||||86 |||||||||||

||||||||||||||||||||||||||||||||||||

|||36 |36 ||||||||||||||||||||||||||||||||

|9 ||||54 |54 ||||||||||||||||||||||||||||||

||12 |||||68 |6|6||||||||||||||||8 |||||||||||

||||||||||||||||||||||||||||||82.800 (1E+01) |||87 |||

|||||||||50 |45 |||||||||||||||||91 |91 ||||||||

||8|62 |62 ||||||||||||||80.500 ||||||21 ||||||||||||

||||||||||||||||||78.200 |||||||31 |31 |94 |94 ||||||||

|||||||||||||||||95 |75.900 ||||||||||||||||||

|27 ||||||||13 |80 |武守|43 ||||||73.600 |||||||37 |37 |||||||93 |||

|84 ||0 |||||59 ||||||79 ||||69.000 (1E+01) 71.300 ||||11 ||34 |57 |57 ||||||||||

|||||55 ||||||||||||66.700 |||||||||||||||||||

||48 ||||40 |||||||||||97 |64.400 |||14 |||44 |||||||||72 |1 ||

|47 ||58 |58 |58 ||||||88 |||||||62.100 ||||||||||||||||||

||||||||||||||||||59.800 |3 |3 |||70 |||||||||||9 ||

|51 |99 |||||92 |92 |||||90 ||||77 |57.500 |57.500 |57.500 |57.500 |||||||||||||||

|||||||||||38 |5 |||||||55.200 (1E+01) ||||||30 ||||||||||4 |

|||||||71 |71 ||||69 |42 ||||16 |52.900 |52.900 |52.900 |52.900 ||82 ||||||29 |||||||

||||||||||||||||||50.600 |50.600 |50.600 |50.600 |||||||||||||||

|0 4 |0 4 |0 4 |0 4 ||9 |9 |9 |9 |14 19 |14 19 |14 19 |14 19 |14 19 |14 19 |14 19 |24 |48.300 |29 ||34 |34 |34 |34 |34 |34 |39 |39 ||||44 49 |44 49 |44 49 ||

Figure 8: Positions of the 100 randomly selected TCs.


V22 and V00 through V11.


Second, the leakage components of the measured currents in a defective chip are obtained by selecting a VDD port whose IDDQ is minimally affected by the defect, e.g., V22 for the defect shown in Q0 on the left side of Fig. 11. The current measured from this port is then used in a backtracking process to obtain the leakage currents for VDD ports surrounding the defect site, e.g., V00, V01 and V10. The backtracking process is shown in Fig. 11 starting with I22. The dashed arrows indicate the process followed to obtain the desired leakage currents I00,I01 and I10. Last, the defect currents are obtained by subtracting the derived leakage components from the measured values.


In this work, we could not apply this method directly because of the small size of the power grid, i.e., all four supply port IDDQs possessed both leakage and defect current. Instead,Equation 4 was applied to approximate the leakage component


in the measured IDDQs. The left side of the equation is a defect current fraction with Im_large and Im_small representing the largest and smallest IDDQs measured from two of the four supply ports. The variable leak is solved for and represents the leakage


Im_largeleak


Slarge--------------


×














Im_smallleak–


) Im_largeleak


------------------------------------------------------------------------------------------------------------------- CFd=


CFd0.5


CF


mm0.5–CFcmcm0.5–--------------------------- CFc0.5–( )×


component of the smallest measured IDDQ. The variable Slarge is the slope of the regression line which characterizes the leakage relationship between these supply ports.


The right side of Equation 4, CFd, approximates the defect current fraction using variables CFm: the measured current fraction using the smallest and largest IDDQs, CFcm: the current fraction computed with both the emulated defect and calibration circuit (CC) enabled, and CFc: the current fraction computed with just the CC enabled. (Note, the CCs in these experiments are the TCs at the positions indicated in Fig. 1.)The range of the right side is 0.5 to a value close to the CC current fraction. For example, if the emulated defect is positioned mid-way between the supply ports, the largest and smallest IDDQs are similar and (CFm - 0.5) is 0 yielding CF = 0.5. If the defect is positioned close to a CC, then (CFm-0.5) ~=(CFcm-0.5) and the right side becomes CFc.


Application of this formula approximates the leakage current component in the smallest measured IDDQ. Backtracking is used to obtain the leakage components in the other measured supply port IDDQs. The leakages are subtracted from the measured values to obtain the defect current components used in the localization method.


Localization Results


We applied the hyperbola-based localization method to the 21,600 emulated defect data sets to determine its accuracy.


Accuracy is evaluated by computing the error, given as the Euclidean distance between the actual position of the enabled TC (emulated defect) and the position given by the intersection of the hyperbolas. This error is converted into a percentage by dividing it by 675 um, the Euclidean distance across the diagoFigure 11: Backtracking method to obtain leakage.


V01 V02


V11 V12


Q0 Q1


leakage01


leakage00


V21 V22


V20


leakage22


leakage11


3 sigma


limits


regression


line


defect’s location


nal of the array. Therefore, a 1% error is equivalent to an actual error of 6.75 um.


We explored two independent parameters of the method. In Section “Separating Defect Current and Background Leakage”,we described a method and a formula to extract the defect current component from the measured IDDQs. The control structure within the array allows the emulated defect to be disabled and the leakage to be measured. Therefore, it is possible to compute a precise value of defect current. We perform the analysis using the extracted and actual defect currents to determine the fraction of the error added by the extraction method.


In Section “Hyperbola-based Model”, we gave a linear expression to compute the a parameters for the hyperbolas. However,the actual behavior of a has a non-linear component, as shown in Fig. 7. We perform the analysis using the linear expression and the actual a curves in order to evaluate the fraction of the total error introduced by the linear approximation. In total, four analyses are performed. The largest errors occur in the analysis that uses the linear expression for a and the extracted defect currents, as expected. The best result is obtained using the a curves and the actual defect currents.


The results of applying the defect localization method to chip C2 are shown in Figures 12 and 13. The emulated defect numbers shown in Fig. 8 are sorted and plotted along the x-axis and the percent error is plotted along the y-axis. The criteria for sorting is distance to the primary supply port, e.g., the results shown on the left side of Figures 12 and 13 are closer to a VDD port while those listed on the right side are closer to the center of the grid. The numbers of the two emulated defects that represent the extremes are given in the ﬁgures as 74 and 28 (see Fig. 8).


As indicated in Section “Data Sets and Quarter Selection Algorithm”, 1,800 emulated defect experiments were performed on


each chip. For each emulated defect site, we varied the magnitude of the defect current by sweeping the DESM across 18 distinct voltages. The curves shown in Figures 12 and 13 plot only one error result for each emulated defect. The value shown is average error computed across all DESM voltages.


Chip C2 is shown because it portrays the worst case, i.e., the largest errors, among the twelve chips investigated in this work. Figure 12 gives the errors when the hyperbolas are derived using the linear expression for parameter a. The curve labeled Actual defect current gives the best result under the linear model. The curve labeled Extracted defect current gives the error when the defect current is estimated using the expression described in Section “Separating Defect Current and Background Leakage”. Figure 13 gives the errors in an analogous way under the condition that the a parameters for the hyperbolas are derived using the curve data.


The ﬁgures include a horizontal dashed line that identiﬁes 20%error. The errors for all but four of the emulated defects are below this line. In general, the errors using the curve data are smaller than those obtained under the linear model. This is expected since the curve data gives a more precise value for the hyperbola a parameter than the linear model. It is interesting to note that the prediction error using the Extracted defect current is smaller than the error obtained using the Actual defect current in several cases. This indicates that the hyperbola model used here is capable of only providing an estimate of the emulated defect’s location. The error curve labeled Actual defect current in Figure 13 also supports this statement. In this analysis, the error contributions introduced by estimating both the a parameters and defect currents are eliminated. The error that remains is largely due to hyperbola modeling inaccuracies of the contour curves, as shown in Figures 4 and 5.


The plots in Figures 14 and 15 give the errors for twelve chips,one plot for each of the four types of analyses. The error curves


Sun Jul  9 17:39:33 2006


-9.000


0.000 (1E+00) 9.000


18.000


27.000 (1E+00) 36.000


54.000 (1E+00) 63.000


72.000


81.000 (1E+00) 90.000


99.000


108.000 (1E+00) 117.000


126.000


135.000 (1E+00) 144.000


153.000


162.000 (1E+00)


-6.300


0.000


(1E+00)


6.300


12.600


18.900


25.200._L


VEHdAMM


31.500


37.800(1E+00)


44.100


50.400


56.700


69.300


75.600(1E+00)


81.900


88.200


94.500


100.800


107.100


113.400(1E+00)


119.700


132.300


138.600


Sun Jul  9 17:40:02 2006


126.0


(1E+00)dthhmM6.30012.60018.900


25.200


-t


Figure 12: Chip C2: Linear equation prediction results.


Figure 13: Chip C2: Curve derived prediction results.


sorted defect number


Actual defect current


Extracted defect current


74


for each of the twelve chips are superimposed.


The ﬁrst notable feature in the four plots is the large error for defect #48 (chip C5) of approximately 40 percent. Inspection of the data revealed that I01 is the largest current causing V01 to be chosen as the primary supply port. Under these conditions,the hyperbolas are derived in Q1 instead of Q0 (see Fig. 8). The erroneous current distribution in this sole experiment is likely the result of a corrupt scan operation. The analysis of this defect in the remaining eleven chips generated the expected result, i.e., the largest current is I00 and V00 is chosen as the primary supply port.


The plot in Fig. 14a gives the worst case error, as expected because the analysis is performed with extracted defect currents and linear equations for a. The variance in the errors


across the twelve chips for a given emulated defect is largest in this analysis, particularly for emulated defects close to the supply ports (left portion of the plot). The smaller level of variance in Fig. 14b suggests that the expression used to extract defect current introduces this error, and is less effective at estimating the defect current component for emulated defects close to the supply ports.


Similar comments can be made with regard to the error variance in Figures 14a and 15a, i.e., the use of the a curves reduces the level of error variance in Fig. 15a. Here, it is also clear that the defect current extraction formula is the main contributor to the error. As mentioned in Section “Separating Defect Current and Background Leakage”, the backtracking method is preferred in chips with larger numbers of supply ports.


Fri Jul  7 20:01:40 2006


-7.000


0.000 (1E+00) 7.000


14.000


21.000 (1E+00) 28.000


35.000


42.000 (1E+00) 49.000


63.000 (1E+00) 70.000


77.000


84.000 (1E+00) 91.000


98.000


105.000 (1E+00) 112.000


119.000


126.000 (1E+00)


-5.000


(1E+00)心Mh5.00010.00015.00020.000


25.000


30.000


%


65.000


75.000


80.000


85.000


90.000(1E+00)


95.000


100.000


105.000


110.000


115.000


120.000(1E+00)


125.000


130.000


135.000


Fri Jul  7 20:00:06 2006


(1E+00)AMMTha5.00010.00015.000


140.000


145.000


150.000(1E+00)


155.000


160.000


165.000


170.000


175.000


180.000(1E+00)


185.000


190.000


Fri Jul  7 19:58:45 2006


(1E+00)M5.00010.00015.000


Fri Jul  7 20:00:51 2006


(1E+00)wnnhm,5.00010.00015.000


Figure 15: Prediction errors in twelve chips using a curves.


Figure 14: Prediction errors in twelve chips using linear equation.


Actual defect current.


Defect #48


The errors are lowest in Fig. 15b, e.g., less than 15 percent, and the curves exhibit a high degree of consistency across the twelve chips. This latter feature demonstrates the effectiveness of the calibration technique to reshape the data to make chips of identical design appear very similar in hardware.


|1992. [4] I. Pomeranz and S. M. |Reddy. “On the Generation of Small |
|---|---|

|Dictionaries for Fault 1992. [5] Aitken, R.C., “A Comparison Location with Iddq Measurements”, |Location”, ICCAD, pp. 272-279, of Defect Models for Fault ITC, pp. 1051-1060, |

|1993. [6] Y. Gong and on S. Test Generation, ICCAD, pp. |Chakravarty, “On adaptive Diagnostic 181-184, 1995. |

|[7] P. Nigh, D. Forlenza, F. of IDDQ Diagnostic Software”, |Motika, “Application and Analysis ITC, pp. 319-327, 1997. |

|[8] Christopher L. Henderson and Jerry M.Soden, “Signature Analysis for IC Diagnosis and Failure Analysis”, ITC, pp. 310-318, 1997. [9] C. Thibeault, L. Boisvert, “Diagnosis method based on del- ta IDDQ probabilistic signatures: Experimental results”, ITC, pp. 1019-1026, 1998. [10] C. Patel, E. Staroswiecki, S. Pawar, D. Acharyya and J. Plusquellic. “Defect Diagnosis using a Current Ratio based Quiescent Signal Analysis Model for Commercial Power Grids”, JETTA, Volume 19, Issue 6, pp. 611-623, Dec 2003. [11] S. Nassif and J. Kozhaya, ”Fast Power Grid Simulation”, DAC, pp. 156-161, 2000. [12] D. Acharyya and J. Plusquellic, “Hardware Results Dem- onstrating Defect Localization using Power Supply Signal Measurements“, ISTFA, pp. 58-66, Nov. 2004. [13] D. Acharyya and J. Plusquellic, “Hardware Results Dem- onstrating Defect Detection Using Power Supply Signal Measurements”, VTS, pp. 433-438, 2005. |[8] Christopher L. Henderson and Jerry M.Soden, “Signature Analysis for IC Diagnosis and Failure Analysis”, ITC, pp. 310-318, 1997. [9] C. Thibeault, L. Boisvert, “Diagnosis method based on del- ta IDDQ probabilistic signatures: Experimental results”, ITC, pp. 1019-1026, 1998. [10] C. Patel, E. Staroswiecki, S. Pawar, D. Acharyya and J. Plusquellic. “Defect Diagnosis using a Current Ratio based Quiescent Signal Analysis Model for Commercial Power Grids”, JETTA, Volume 19, Issue 6, pp. 611-623, Dec 2003. [11] S. Nassif and J. Kozhaya, ”Fast Power Grid Simulation”, DAC, pp. 156-161, 2000. [12] D. Acharyya and J. Plusquellic, “Hardware Results Dem- onstrating Defect Localization using Power Supply Signal Measurements“, ISTFA, pp. 58-66, Nov. 2004. [13] D. Acharyya and J. Plusquellic, “Hardware Results Dem- onstrating Defect Detection Using Power Supply Signal Measurements”, VTS, pp. 433-438, 2005. |

Summary and Conclusion


A hyperbola-based defect localization method is applied to the data collected from a set of chips fabricated in a 65 nm technology. The test chips incorporate an array of test structures that permit the controlled insertion of a shorting defect. The method uses multiple supply port IDDQs to triangulate the physical location of the defect in the layout. The results of the analysis indicate that good diagnostic resolution is achievable, with localization errors less than 15% or 100 um in most cases.


We thank Dr. Sani Nassif, Chandler McDowell and Dr. Anne Gattiker of IBM Austin Research Laboratory for their support of this research.


[1] ITRS (http://public.itrs.net/)


[2] Gong Yiming, S. Chakravarty, “Using Fault Sampling to Compute IDDQ Diagnostic Test Sets”, VTS, pp. 74-79,


1997.


[3] S. Chakravarty, M. Liu, “IDDQ Measurement Based Diagnosis of Bridging Faults”, JETTA, Vol. 3, pp. 377-385,


Logical-to-physical Device Navigation using Place-and-Route Data   as an Alternative to LVS


Roger Nicholson


Credence Systems Corporation 1421 California Circle Milpitas, CA  95035  roger_nicholson@credence.com, Tel: (408) 541-5364, Fax: (408) 541-5330


Logical-to-physical device navigation for failure analysis is  often used to drive physical probers and focused ion beam  tools. Traditional methods of creating navigation data rely  upon the use of time consuming Layout-versus-Schematic (LVS) based methods. By using existing place-and-route data, full cross-linked navigation between schematic and physical  layout may be achieved in a fraction of the time that it takes  for the LVS methods to be used. Place-and-route data offers  significantly more information to the analyst than LVS based  data.


The LVS Bottleneck to Producing Navigation Data


When CAD navigation was first introduced as a means of  guiding physical probers and focused ion-beam systems in the  late 1980’s, analysts were forced into dealing with tools that  were part of the designer’s realm. Device analysts suddenly  had to learn how to run Layout-versus-Schematic (LVS) tools  which were used by designers to verify design consistency. The output files produced by these LVS runs were often  discarded by designers, but turned out to be of great value to  the analyst. These output files could be cross-mapped to  produce a logical-to-physical design correspondence and used  to guide physical analysis equipment to the proper locations. The basic LVS based method of generating CAD navigation  databases has persisted for over 18 years. For the multimegabyte designs of the late 80’s and early 90’s, this method  proved sufficient. For the multi-gigabyte designs of today, however, the application of the LVS method demonstrates  some serious limitations. The entire LVS processing and postprocessing can take days to weeks on today’s latest designs, and represents a bottleneck through which all CAD data must  flow in order to be useful to the analyst. (Fig. 1) In the end, the analyst simply wants to be able to cross-map the logical  schematic with the physical layout for the purpose of driving a  prober or FIB stage to the correct locations. The massive preprocessing requirement becomes a discouragement and the  full CAD data set is abandoned in favor of a simple, manual  navigation approach.


An additional challenge arises when considering the data that  is made available to the analyst using the LVS-based


approach. Some LVS tool vendor’s data facilitates the  identification of only nets and transistors, while other  vendor’s tools provide net, cell and pin identification. The  LVS data traditionally used to drive probers and focused ionbeam have typically been limited to being able to use only the  net and transistor information. More often the transistor  elements are not processed and the only thing made available  to the analyst is a cross-reference of electrical nets to the  physical layout, without any relevant cell or pin information.


Figure 1: Data flow through the LVS “bottleneck”


CAD Navigation Tailored for the Device Analyst


The real goal is to produce CAD navigation data that is well  suited to the device analyst. When considering today’s  probing tools and focused ion-beam systems, it is necessary to  step back and re-examine the needs of the device analyst. It is  also necessary to identify any existing design data that may be  used in order to entirely avoid the need to process data using  LVS. Effective CAD navigation for the device analyst must  meet the following requirements:


• Both physical layout and logical schematics must be able  to be viewed quickly and easily


• Cross-mapping between the logical and physical domains  must be easy to generate and use


• The cross-mapping must include the ability to physically  identify and locate circuit elements useful to the analyst  such as cells, input and output pins, nets and drivers


• EDA fault diagnostic tools must be able to easily transfer  their output data to the CAD navigation domain


It seems advantageous at this point to step back and reexamine the available design data in order to determine if an  easier way to generate cross-mapping data exists. Upon


## Logical-to-physical Device Navigation using Place-and-Route Data as an Alternative to LVS


46


examining the design data that is available, a particular set of  files is identified as being particularly useful. These files are  the Library Exchange Format (LEF) and Design Exchange  Format (DEF) files that are used in the design of standard cell  devices.


The LEF/DEF physical design formats were developed by  Cadence and released to the design community in 2000 to  promote interoperability and data exchange between design  tools. [1] DEF files contain the logical names of all of the cells  in an ASIC design, as well as the corresponding cell size, location and orientation. The DEF file also contains a listing  of all of the major nets connecting the cells within the device, and the physical coordinates used to route these nets between  cells. Since the DEF file contains both logical and physical  data in a single file, this suggests that the LVS and LVS-post  processing steps might be avoided altogether and that cell and  net cross-mapping can be produced within a matter of minutes  rather than days. The results of the LEF/DEF logical-tophysical cross mapping may be superimposed, or “highlighted” on the physical layout.


A number of physical layout editing tools have been able to  read and display LEF/DEF data for a number of years, so the  idea of reading this data and visually displaying it is not new. These layout editing tools, however, are not typically used to  drive physical analysis equipment. The device analysts who  use this equipment are usually not familiar with these files. Although used in the design community for years, these  LEF/DEF files have not been applied to physical device  analysis. The customized application of LEF/DEF  highlighting to the needs of specific analytical tools, such as


Top Level DEF


non-contact probers and focused ion-beam systems, is  addressed in this paper.


Lower Level DEF LEF


The use of LEF/DEF data in conjunction with directly reading


少


Cell Library


the layout and netlist data can result in the production of a  CAD navigation database which is ready to use in just


Y2


(Rotated)


minutes. (Fig. 2)


→X21


Physical Layout


Files


(GDS2)


(Netlist)


LEF/DEF


Circuit


一


Logical


汇


Figure 2: The Direct Read and LEF/DEF Approach to CAD  Navigation


The use of LEF/DEF data in CAD navigation has many  advantages and several disadvantages relative to the polygon  highlighting method. The most obvious disadvantage is that  the LEF/DEF data does not include any of the internal net or


transistor structures within the boundaries of a cell. Crossmapping nets that are located within cell boundaries is simply  not possible. However, there are some very significant  advantages to using LEF/DEF cross-mapping. The DEF  contains cell boundary information. It is easy to display the  cell boundaries on the physical layout in order to determine  where the active circuitry lies. Similarly, the LEF data  displays the individual pins on the cell. It is possible to use the  LEF data to identify specific input pins or net drivers. By  using LEF/DEF data, it is possible to produce a cross-linked  database in a fraction of the time that producing a LVS  database will require.


Dealing with Hierarchical DEF File Structures


There is an issue that must be addressed when attempting to  apply DEF file coordinates to a physical device. DEF files  may be hierarchically structured, with each individual DEF  file containing its own local coordinate system. This is not  conducive to full device navigation to absolute X-Y  coordinates on a device. The use of the DEF coordinates  requires tedious manual calculation of the absolute  coordinates for a specific cell location which requires adding  together all of the appropriate cell offsets obtained from the  individual levels of DEF hierarchy. In the example shown in  Fig. 3, the calculation of the absolute chip coordinate for  location a LEF library cell requires that the offset of the top  level DEF (X1,Y2) be added to the local offset (X2, Y2) in  the lower level DEF file. The calculation of the absolute  coordinates is further complicated by the fact the library cell  may be rotated.


X1


LEF/DEF Conversion


Figure 3: A diagram of nested DEF and LEF elements


▼LayoutLEF/DEFNetlist/


In order to utilize the raw coordinate data in the LEF/DEF


Viewer


Database


Cross-mapping**Schematic


files, these calculations must be performed by using a


spreadsheet in order to add together all of the appropriate  offsets. This manual process is tedious and inefficient, thereby  wasting valuable time that might otherwise be spent analyzing  data.


The manual offset calculation procedure may be replaced with  a LEF/DEF database creation tool. This tool reads in all of the  LEF and DEF files associated with a hierarchical design and  creates a single, query-driven binary database. Thus the only


pre-processing required to bring up a CAD design for  navigation is to create the LEF/DEF database, which can be  accomplished in a matter of minutes. The resulting database  takes cell, net or pin names as inputs and returns the absolute  X-Y chip coordinates for these structures.


An Efficient Method for Highlighting Physical Circuit  Elements


The use of LEF/DEF based system navigation in conjunction  with a layout and schematic provides some quick and useful  benefits when used with different types of analytical systems.


0NOR2X2


Figure 4: An Inverter Connected to Four Circuit Elements


Consider the inverter “cinv” shown in Fig. 4. The schematic in  Fig. 4 shows four cells connected to net “cob3”, which drives  the inverter input. The output of the inverter drives a single  cell through net “co3”. Figure 5 shows a comparison of  simultaneous net highlighting of nets “cob3” and “co3” using  traditional polygon highlighting (left side) versus LEF/DEF  highlighting (right side). There are a number of differences in  the information conveyed by the two methods.


保8毅


Figure 5: A Comparison of Polygon Highlighting versus  LEF/DEF Highlighting on the Inverter


The polygon highlighting shows electrically connected  polygon structures, including the polysilicon gates of inverter “cinv”. The net feeding the inverter input is somewhat  difficult to distinguish due to the overlapping of the  rectangular highlighted polygons in the center of the inverter. Another important thing to note is that the inverter cell  boundaries are not shown in the polygon highlighting.


The LEF/DEF highlighting of the same two nets on the right  shows a less complicated view. First, it should be noted that  the LEF/DEF nets are only highlighted along the centerline of  the polygons comprising that net – the entire width of the net  is not shown. This eliminates many distracting extra lines  from the image, while still clearly indicating the route of the


net. Also, the polysilicon gates are not highlighted, since these  are internal cell structures which are not contained in the LEF  or DEF files. The input net to the inverter is clearly observed  to be passing into one side and out the other side of the cell, since it is connected to three other cells. The cell boundaries  of the inverter are clearly shown, as well as the cell  boundaries of the cell adjacent to it. Both the polygon method  and the LEF/DEF method highlight the pin structures, however only the LEF/DEF is capable of identifying the pin  independent of the net that it is connected to. From the  polygon point of view, the pin is just another electrically  connected set of polygons without a unique identity.


cobarA ckB


It is clear that some information is missing in the LEF/DEF


cnt-4C


highlighting. Specifically, the polysilicon gate structures are


NOR3X4


not part of the LEF/DEF file and are therefore not highlighted.


ciny


at


cobar


a州c台co


It may be desirable to highlight these structures as well. The


INVX2ck-8squestion is how to achieve this without being forced to run


cnor


ADDHX2


some of the time-consuming LVS components in order to


A□√


ontr4


0 D


日


generate it. This problem is solved by using an algorithm  which extracts the electrically connected polygons  of a net  on-the-fly rather than relying upon LVS pre-processing. This  algorithm allows the selection of a polygon within the layout  view after which it calculates and highlights the electrical net  on-the-fly. The resulting highlighting may be superimposed  upon the LEF/DEF highlighting, thus giving us the advantages  of both highlighting methods.


Figure 6: Superimposition of electrically connected polygon  highlighting with LEF/DEF highlighting


Note in Fig. 6 that the net trace algorithm highlights the  outlines of the nets, while the LEF/DEF net centerline  highlighting is still visible. At this time only a single net may  be highlighted using the net trace algorithm, which is why the  inverter output still appears as a single centerline. The  advantage of this simultaneous highlighting method is that the  cell boundaries and pins may still be individually identified in  the LEF/DEF database while still highlighting the polysilicon  gates. All of this highlighting is achievable without running  any stage of the LVS process.


Identifying Specific Pins


Often it is desirable and useful to know the location of a  specific pin on a cell. LVS based cross-mapping methods


examine only the physical connectivity of the polygon  structures defined at various layers. The electrical connectivity  is determined by identifying the vias and contacts that are part  of the electrical net. As a result of this, a net, as determined by  LVS, is a connected collection of polygon structures, without  any unique identifying characteristics that would assist in the


CSIGPS Query Results


identification of cell pins. The device analyst must manually


国NET i_so2/co


identify individual pins within a cell.


CELLi_so2/cntr/cco


i_so2/cntr/cco(1628.810059 -1657.344971)(1635.410034-1652.304932)


The use of LEF data allows a more precise identification of


PIN Y (1635.120117 -1654.964966) (1635.270142 -1653.564941)


the pins. The LEF file contains a correspondence of the  physical positions of each pin in a cell with its logical  identification. Unlike the nets in the DEF file, the LEF file  does contain the physical geometric structure of the pins  themselves. Consider the example of the 3-input NOR gate  shown in Figure 7.


divide_4


Figure 7: Finding the output pin “Y” of the NOR gate “cco”


CELL "cco"NET


Consider the process of finding the driver for the net shown in  Figure 7. Using standard, LVS based polygon highlighting, the entire output net of cell “cco” is highlighted as shown in  Fig. 8 (background polygons have been removed for clarity)..


□


Figure 8: Polygon based highlighting of the output net


11


connected to cell “cco”


of


The net displayed in Fig. 8 shows a connection to three


姑.to0=80to of5次Rs


1210o、*21


内$0-2也1内102


1P


沙


Fto o-. . .2诽内ofo t10832jaus1019602


separate pins. In order to identify a specific pin using only


UFF2


PIP


polygon based highlighting, it is necessary to manually


examine each of the three pins in the physical layout and  deduce which of them is the correct one. In this case, the  output of cell “cco” could be located fairly easily by  determining which of the three locations is connected to


clkbuf


diffusion. For a small net, this is a relatively easy process, however, for large nets, it is not trivial.


Selecting the same net from the LEF/DEF database produces  two results. One is a listing of the specific cell, pin and metal  segment locations (Fig. 9). The second result is the net, cell  and pin highlighting shown in Fig. 10.


PIN Y(1634.890015-1656.219971)(1635.119995-1653.564941)


Figure 9: A Listing of the LEF/DEF Cells, Pins and Metal  Segments


By selecting the cell “I_SO2/CNTR/CCO” from the list, the  identity and location of the driving cell is indicated by  highlighting the cell boundary in the display. The system stage  may then immediately be moved to this location without


cntr


s1buf


having to manually search each terminal of the net.


clk


CCO


AAnor3x4


BUFX8


C<Bto OCmor3


in


NOR3X48-DON-counterDFFX2日CK Q->


、


d1


but


div4


PIN


Figure 10: LEF/DEF Highlighting of the same net


Dealing With Large Nets


A small net such as that shown in the previous example is  fairly easy to deal with using either polygon based or  LEF/DEF based highlighting. If the net contains more than a  few cells, however, the task of locating the driver becomes


quite tedious when one is attempting to use polygon


NET


highlighting. Consider the example shown in Fig. 11. This  schematic shows a clock net, which is driven by a single  buffer and drives 11 different cell inputs.


Figure 11: Schematic of a Clock Net Showing Location of the  Clock Buffer


The polygon net highlighting is not very useful in assisting the  analyst in finding the location of the clock driver. (Fig. 12)


Figure 12: Polygon Highlighting on the Clock net


In order to determine the location of the driver using polygon  highlighting only, it is necessary to manually examine the  entire net. Since LVS-based polygon highlighting is limited to  only nets and transistor elements, it is not possible to locate  the clock buffer cell directly. Instead, its physical location  must be determined using indirect means and manual visual  examination of the highlighted net.


The LEF/DEF place-and-route highlighting shows  significantly more information than the polygon highlighting. The clock buffer (net driver) is easily located in the layout  display by selecting it from a list of LEF/DEF elements (Fig. 13).


SiGPS Query Results


NET i_so2/cntr/clk


CELL i_so2/cntr/c2/d3


国 CELL i_so2/cntr/d8


国 CELL i_so2/cntr/d9


Strap


CELLi_so2/cntr/c1/d3


国 CELL i_so2/cntr/d9 CELL i_so2/cntr/c1/d3 CELL i_so2/clkbuf


器


i_so2/clkbuf (1597.130127 -1667.425049) (1600.430176 -1662.385010)


菌


Cut


PINY(1599.330076-1666.165039) (1599.630127-1664.345093)


Figure 13: Selecting the Clock Buffer Output Pin “Y” from  the LEF/DEF Element Highlighting List


Selecting the clock buffer output pin “Y” locates the physical  coordinates of this pin in the highlighted display (Fig. 14).


Figure 14: LEF/DEF highlighting showing the location of the  clock buffer ”clkbuf”


LEF/DEF Highlighting for Simple FIB Edit Planning


Consider the use of CAD data with a focused ion-beam  system. Traditionally, the use of CAD data for FIB edit  planning has been limited to the display of the GDS2 layout  data. The layout data aids in determining the locations of  buried conductors on planarized or flip-chip devices. With  regard to actual edit planning, however, the logical schematic


is often not considered at edit time due to the time and  difficulty of obtaining the LVS logical-to-physical crossmapping data. The process overhead becomes so severe that  many FIB users simply give up trying to use the logical data. Instead, the FIB operator settles for viewing the CAD layout  only, since it is easily obtained. The determination of the edit  structure is done off-line prior to the use of the FIB, and the  edit plan becomes a set of precisely defined modifications that  are handed down to the FIB operator to execute.


The use of LEF/DEF place-and-route data can provide a quick  and useful link to the logical domain for FIB edits. By  defining edits using the logical schematic, it is possible to  quickly and easily guide the creation of the physical edit  definition.


In the example considered previously, suppose that it were  desired to remove inverter “cinv” from the circuit shown in  Fig. 4. The LEF/DEF highlighting gives a simple and clear  indication of where the FIB edit ought to be performed (Fig. 15). The edits should occur in the region between cell  boundaries, in order to avoid affecting active regions.


Figure 15: Defining a FIB Edit to Isolate the Inverter


A cut is defined on the inverter input net at the edge of the cell  boundary. Openings are milled in both the input and the  output net in the region between cells, and a strap is deposited  between the two nets.


LEF/DEF Highlighting for Emission Analysis


Emission tools are becoming quite common in device analysis


甘


labs. These systems are capable of detecting photon and


0clkbuf


thermal emission of a device that is under either static or  dynamic bias. While emission tools are very efficient at  narrowing down the area of interest when searching for the  cause of a failure, the question of which analysis step to take  next is often most critical. Many users of emission tools  simply perform a destructive de-processing of the device after  locating anomalous emission locations. This is done on the  assumption that the location of a defect or artifact causing the  emission is located at the exact coordinate at which the  emission was observed. For thermal emission, this may be a  valid assumption since a physical defect and a local  temperature change are likely to correlate with one another. In


the case of photon emission, however, it is more often the case  that the emission is a side effect of a defect which is located in  an area farther away from the emission site itself. These types  of defects include resistive interconnects and opens or shorts  in upstream or downstream cells. In this situation, deprocessing the device in the hope that a defect will be  observed is very likely to result in a complete loss of the  artifact causing the failure. This is the result of being fooled  into only examining the site of photon emission for artifacts, rather than determining the extent of the area around the  emission site which may contribute to the failure.


The use of LEF/DEF place-and-route data provides a quick  and easy method of determining the region of interest  surrounding photon emission locations. Suppose that a photon  emission location were mapped to the physical layout in the  location indicated by the “X” in Fig.  16. By applying the  LEF/DEF highlighting overlay, it is possible to identify the


旦SIGPS Query Results


logical cell in which the emission occurs (Fig. 16) In this


NET i_so2/cntr/q8


example, the cell is identified as cell “d8.”


M2 (1589.553955 -1658.203003) (1589.553955-1656.541992)


|example, the cell is identified as cell "d8."|example, the cell is identified as cell "d8."|example, the cell is identified as cell "d8."|example, the cell is identified as cell "d8."|example, the cell is identified as cell "d8."|
|---|---|---|---|---|

|2227|2227|2227|2227|2227|

|rE cCccc|rE cCccc|rE cCccc|rE cCccc|rE cCccc|

|||||cood|

|||||一|

VIA VIA1(1589.553955 -1658.203003)(1589.553955-1658.203003)M1 (1589.553955-1658.203003) (1606.682983 -1658.203003)


VIA VIA1 (1606.682983 -1658.203003)(1606.682983 -1658.203003)M2 (1606.682983 -1661.541992)(1606.682983 -1655.348022)


VIA VIA1 (1606.682983 -1661.541992)(1606.682983-1661.541992)M1(1606.682983-1661.541992)(1613.293945-1661.541992)


VIA VIA1(1613.293945-1661.541992)(1613.293945-1661.541992)


Figure 16: Mapping the emission coordinate to the  corresponding logical cell on the physical layout


日□SIGPS Query Results


Rather than de-process the device at this stage, the LEF/DEF


NET i_so2/cntr/s8


data can be used to expand the upstream and downstream


CELLi_so2/cntr/d8


logic. This information is superimposed on the physical layout


CELLi_so2/cntr/a8


as shown in Fig. 17.


ADDHX28DFFX2


chand


信


Figure 17: Expanding the upstream and downstream path


98A8


from the emission location using LEF/DEF highlighting


cob3


Y NAND2X2


This expansion of logical elements defines a new region-ofinterest. Rather than concentrating only upon the area of the  emission itself, a new region-of-interest is produced which  incorporates the upstream and downstream components. It is


now possible to apply additional analysis techniques to this  newly defined region in order to search for anomalies.


LEF/DEF and Soft Defect Localization Techniques


A number of newer analytical techniques referred to as Soft  Defect Localization have been introduced which use laser  scanning to affect the pass/fail state of a device by inducing  localized laser heating. [2, 3] The use of LEF/DEF data to  expand from emission locations to produce a local region-ofinterest can produce a more refined target area for the  application of these laser scanning techniques. For example, the laser scan could be limited only to the new region-ofinterest, rather than the entire chip. In fact, if via resistance  was the primary suspect,  the targeting of the laser could even  be limited to the precise via locations listed in the LEF/DEF  database (Fig. 18).


M2 (1613.293945 -1665.485962) (1613.293945-1661.541992)


Figure 18: Listing of via and metal segments from the  LEF/DEF database


It may be desirable to map the logical elements in the regionof-interest back to the schematic. The list of logical elements  is shown in the LEF/DEF listing. (Fig 19)


CELLi_so2/cntr/cnand


Figure 19: List of LEF/DEF logical elements in the region-ofinterest


Mapping these cells and nets to the schematic display shows  which elements may need to be examined. (Fig. 20)


c8


555*85*85**


a8


ACOCK0您88DQN


qb8


d8


Figure 20: Elements in the region-of-interest mapped to the  schematic


Table 1


Comparison of names that may be used to reference the  three nets in Fig. 21


LVS Net


Name


Pin Path  Name


Net   Name


start1


i_so2/s1buf/Y


i_so2/start1


sclkout


i_so2/sclkbuf/Y


i_so2/sclkout


sdo


i_so2/sdobuf/Y


i_so2/sdo


Once the subset of upstream and downstream schematic  elements has been identified, the analyst may decide to  perform non-contact probing in order to identify a failing  element.


EDA Fault Diagnostic Tools and Place-and-Route Data


Fault diagnostic tools are used with scan devices. These tools  use the failure datalog from a tester to narrow down and  identify a subset of circuit elements which may be responsible  for a failure. The output results of a fault diagnostic may be  displayed in the form of either ASCII text or as a graphical  schematic segment. Once fault diagnostic data has been  generated, the next step is to perform a physical or electrical  analysis of the device in order to determine the exact cause of  failure. This requires the analyst to map the output of the fault  diagnostic tool to the corresponding physical chip coordinates  in order to drive a non-contact prober to those locations. The  challenge occurs when trying to correlate the output data from  the fault diagnostic with the available cross-mapping  produced by LVS methods. [4]


The problem with the LVS data that has typically been used to  drive physical probers is that the net naming produced does  not always conform to the hierarchical naming structure of the  netlist. In the LVS perspective, an electrical net must take on a  single name. From the perspective of the fault diagnostic tool  or hierarchical netlist, however, a net may be referred to by  multiple names. Consider the schematic showing several  output buffers shown in Fig. 21.


Figure 21: A set of three output buffers


When LVS cross-mapping is used to create a navigation  database, it begins at the top level pins and works its way  down into the circuit. In the example shown, the three nets  connected to the output pins would take on the names of the  pins themselves: “start1”, “sclkout”, and “sdo.”  The output of  a fault diagnostic tool will typically refer to cell and net names  that are associated with the hierarchical netlist structure. The  same three output nets shown in Fig. 21 would be associated  with the pin path names “s1buf/Y”, “sclkbuf/Y” and “sdobuf/Y.” The net segments themselves also have a name  that is associated with their location within the hierarchy of  the schematic: “i_so2/start1”, “i_so2/sclkout” and “i_so2/sdo.” A comparison of these names is summarized in  Table 1.


Suppose that a fault diagnostic tool indicated a fault on buffer “s1buf”. Here is how that diagnostic data would be  represented (some items have been removed for clarity):


Synopsys TetraMAX:


<type>  … <pin pathname> <cell name>


Example:


<type>  --   i_so2/s1buf/Y   (BUFX8)


Mentor YieldAssist:


…<type>…<pin pathname> <cell name> <net pathname>


… <type> … i_so2/s1buf/Y  BUFX8 i_so2/start1


If the LVS cross-mapping database only refers to the net  referenced above as “start1”, then it will not easily match with  the output of these fault diagnostic tools.


The use of LEF/DEF data provides a significant advantage  over LVS data when used with fault diagnostic tools. This is  because the DEF file often uses the same hierarchical pin  pathname and net pathname syntax as the fault diagnostic  tools. It then becomes a simple matter to copy the names from  the fault diagnostic log and use them to query the LEF/DEF  cross-mapping database. For the case of the “i_so2/s1buf/Y” pin path name referenced in the fault diagnostic examples  above, a query to the LEF/DEF database produces the  highlighted cell and output pin “Y” shown in Fig. 22.


Figure 22: Cell i_so2/s1buf with pin “Y” highlighted


This allows a direct correlation to be made between the fault  diagnostic output and the physical location on the chip. This  physical chip location may then be analyzed using standard  probing methods.


It should be noted that there are also a few situations in which  the LEF/DEF hierarchical naming convention does not exactly  match the netlist naming convention. Often the issue is a slight  difference in syntax, or the addition or deletion of extra  characters.  In cases such as this, it becomes necessary to  supply a character mapping capability to the cross-mapping  function in order to allow additional characters to be inserted  or deleted in the cross-mapped text strings.


LEF/DEF Highlighting Does Not Completely Replace LVS


The LEF/DEF highlighting approach is not a complete  replacement for the LVS-based method. As stated previously, LEF/DEF files are available for standard cell designs. These  designs use third-party cell libraries and as the building blocks  of the design. Individual cell instances are placed and  interconnected in order to form the complete chip design. In  the case of custom devices, the LEF/DEF information will not  exist. Likewise, analog devices do not utilize these files. For  these types of devices, the LVS-based method is clearly the  only alternative for producing useful logical-to-physical cross  mapping. The use of LEF/DEF data can significantly reduce  the amount of time and effort required to perform logical-tophysical and physical-to-logical cross-mapping in cases where  this data is available. A combination of LEF/DEF and LVS  cross-mapping methods may be used depending upon the  device type and the availability of the CAD data.


Future Applications


The applications of LEF/DEF highlighting to device analysis  need to be further explored. This paper has only addressed the  basic needs of generating CAD navigation data quickly and  easily. It is apparent that there is beneficial information in the  LEF/DEF data that can be used to assist with emission, probing and focused ion-beam applications. What remains is  to explore in more detail the possibilities of customizing the  LEF/DEF data to the needs of specific device analysis  methodologies.


One possible application that presents itself is the use of  LEF/DEF data to guide the analyst in pinpointing the location  of potential bridging faults using physical analytical methods. Bridging faults are often identified through the use of complex  software algorithms that create a fault dictionary containing  the locations of many of the possible net adjacencies in the  physical layout. By applying simulation to this model, it is  possible to generate a large number of output signatures which  may be correlated to specific potential bridging locations. When a device fails at test, the signature of the failing outputs  is compared to the signatures generated using the fault  dictionary. If a match is obtained, it may be assumed that a  bridging fault has occurred at one of the potential bridge  locations corresponding to that signature. This method  attempts to direct the analyst to locations which need to be  physically examined for defects. Fault dictionaries created in


this manner tend to be extremely large and impractical when  applied to large numbers of nets. [5] If the fault dictionary  approach is not used,  the location of adjacent nets which may  be susceptible to bridging faults may require a tedious manual  effort. [6] This extra effort to manually locate adjacent nets is  purely mechanical and does not contribute to the resolution of  the analysis.


Although the LEF/DEF database only contains the main  interconnects between cells, the information contained in this  database could be interpreted to present a complete list of all  nets which are adjacent to one another within a specified  region-of-interest. This would provide a set of specific  locations that might be examined using a variety of analysis  techniques. This approach would not be as comprehensive as  the creation of a complete fault dictionary, since it would only  address the main interconnects, but it could provide physical  analytical tools with a set of locations to examine in order to  determine whether or not a bridge exists.


In addition to providing lists of adjacent nets, the LEF/DEF  database could be modified to provide a concise list of   locations at which one net crosses over another net. These  locations would be useful when attempting to determine the  optimal location to place FIB edits.


Finally, there are also potential alternatives to using the  original LEF and DEF files directly. Comprehensive EDA  design databases such as Cadence®/Si2 OpenAccess and  Synopsys® Milkyway can provide netlist data, physical layout  and logical-physical cross-mapping. The software tools that  read these databases are used primarily in the design realm  rather than as a navigational aid for driving physical analysis. A current limitation is that the EDA vendor supplied software  tools capable of directly accessing these databases do not yet  link directly to many physical probers and focused ion-beam  systems.


The use of place-and-route data for the purposes of device  navigation provides the failure analyst with the ability to  generate logical-to-physical cross mapping in a very short  amount of time. The data contained within the place-and-route  database provides the analyst with critical information which  is often missing in LVS navigation databases: cells, nets, pins  and drivers. Therefore, the use of place-and-route data as an  alternative to LVS data provides the analyst with the ability to  generate a more useful set of CAD navigation data in a  fraction of the time.


[1] Santarini, M., EE Times, June 5, 2000.


[2] Cole E, Tangyunyong P, Hawkins C, Bruce M, Bruce V, Ring R., Chong, W., “Resistive Interconnection  Localization”, Conference Proceedings from the 27th  International Symposium for Testing and Failure  Analysis, Santa Clara, CA, pp. 43.


[3] Bruce, M., Bruce, V., Eppes, D., Wilcox, J., Cole, E., Tangyunyong, P., Hawkins, C. “Soft Defect Localization (SDL) on ICs,” Proceedings from the 28th International  Symposium for Testing and Failure Analysis, November  3-7, 2002, Phoenix, Arizona, pp. 21-27.


[4] Bodoh D, Blakely A, Garyet, T: “Diagnostic Fault  Simulation for the Failure Analyst”, Proceedings from the  30th International Symposium for Testing and Failure  Analysis, November 14-18, 2004, Worcester, Massachusetts.


[5] Vogels, T, Wojciech, M, Blanton, R.D., “Progressive  Bridge Identification,” Proceedings International Test  Conference 2003, Charlotte, NC, Sept.-Oct. 2003, pp.


309.


[6] Gopu, D. Ontko, G., Phan, C., Ramanujachar, K., Wills, S., Hales, A., “Precise Fail site Isolation using a  combination of Global, Software and Tester based  Isolation Techniques,” Proceedings form the 30th  International Symposium for Testing and Failure  Analysis, Worcester, MA, Nov. 2004, pp. 173.


Fundamental Considerations for CDM failure in 90nm Products


Nobuyuki Wakai, Yuji Kobira, Masayoshi Tsutsumi*, Hidemitsu Egawa


System LSI Q&R engineering dept. Toshiba Corporation Semiconductor Company *Semiconductor Analysis and evaluation center, Toshiba Nanoanalysis Corporation   8, Shinsugita, Isogo, Yokohama, Japan, 235-8522,


E-mail: nobuyuki,wakai@toshiba.co.jp


Tel: +81-45-770-3270


Fax: +81-45-770-3284


In the end, the features that a CE engineer encounters can be  different from the “Blue Print” GDSII data. Filler


metal features, sizing and other changes to the shape and size  of features can be generated after the GDSII is “taped out” but  before the chip is made. Traditionally, a CE engineer will get  the GDSII file for use in navigation. In the past, this has served the purpose but in more recent technologies this file information is not sufficient. A feature of interest can be located with the GDSII file information but above and around  that feature things can look and be very different than expected. For example, if a lower level metal is to be exposed, it may appear clear from the top on the GDSII file but in reality it is covered with fill metal. This means that the CE engineer encounters metal features (in the form of lines,rectangles or other shapes) on the way to the signal of interest without any foreknowledge of where these metal features reside. This challenge required us to develop a variable selectivity process so that when such filler metal is reached,the process is adjusted to have a selectivity or 1:1 between the  metal and dielectric. In the case where a metal line is to be


cut, the selectivity is adjusted to be higher for copper over dielectric. This process is described below.


度震


Variable Selectivity Processs


The challenge of maintaining floor flatness in the process of circuit editing through power planes has become more difficult with the introduction of copper into IC fabrication.


Since there is no volatile copper compound simple enough to  survive under ion bombardment (like AlI3 for Aluminum), the  mechanism of copper removal is exclusively due to ion beam  sputtering. As a result, the main approach for selectivity improvement must be dielectric protection rather than enhancement of copper removal and, on top of that,achievable selectivity for copper etching is unable to go as high as for etching other materials where volatile etch byproducts are created. But this is only one part of the difficulty, the other part is material re-deposition as illustrated in Figure


3. The sputtering process generates copper re-deposition all around the area exposed by the ion beam. This creates a vicious cycle where material that is to be removed re-deposits in the area making electrical isolation of a signal impossible.


Figure 3. Stepped trench formation when a highly selective copper etch process (selective over dielectric) is applied to cut a copper line embedded into the dielectric


When trying to cut copper embedded into dielectric using a highly selective process, one encounters a stepped trench formation with copper re-deposited on its walls. Sputtering has spatial anisotropy in obstructed areas and normally shows  a high percentage of atomization of the sputtered material [4]. Atomic copper is readily re-deposited on the walls of the stepped trench created by this selective copper etch process.


Thus the high selectivity of copper removal over the dielectric  creates and maintains the dielectric sidewalls of the trench,which in turn captures sputtered copper.  Significant topography change (trenching) results in processes whose selectivity of copper over dielectric is high.  This topography generally causes problems in reaching lines in underlying layers.


OP


Fill


The trench formation challenge is illustrated in details in the  set of sequential FIB micrographs in Fig.4.  A highly selective process (high etching rate of copper compared to that of dielectric) was applied to cut a copper line as it is shown in Fig.4a


Fig. 4a Initial view of the target copper line


Fig.4b. Selective removal of copper exposes dielectric under the line


Fig.4c. The dielectric under copper line is exposed almost


completely, but the cut is not completed. Highly selective


process creates a trench with walls on which copper is redeposited.  Removal of copper from the walls is very slow.


Fig. 4d. After a significant time the cut is done, but dielectric  floor is very uneven in the region of the trench.


magHVwo823/2008detHEW500.mm


60000x5.00kV 5.0mm5312:1816PM TLD 243μmAMER Inc


Figure 5. The stepped trench cross-section picture shows the  step height on the order of 0.15um. To improve contrast, the  SEM picture was taken in back-scattered electrons.


Therefore, an adjustment is needed to prevent the stepped trench formation like that shown in Figure 3. Obviously, one


0.15um


would like to reduce the portion of copper embedded into dielectric prior to copper etching.


For this purpose, a process has been developed whose sputter  selectivity between different interconnect materials (low-k and copper) can be adjusted. Selectivity adjustment is illustrated


Fig.6.


0 2 4 6 8 10


Copper (101)


High Selectivity Area Selectivity 1 : 1


for different grains


Dielectric


Copper (111)


Pre-cursor pressure / ion dose rate (a.u.)


Figure 6. The relationship between etch rate and selectivity  for copper over dielectric in the variable selectivity process.


Because the gaseous precursor inhibits sputter of the material  of interest, as the ratio of this pre-cursor pressure to the ion  dose rate increases, the etching rates of both dielectric and copper decrease. Dielectric etching rate decreases much faster  than that for copper in all its crystallographic orientations.


In the method developed, at the beginning of the copper etch  process conditions are applied where the etching rate of (111) grains is approximately equal to the etching rate of the


dielectric (first point of 1:1 selectivity in Figure 6). This


enables the reduction of removal of the dielectric where it is  exposed and prevents stepped trench formation. Once a


noticeable amount of copper is removed and dielectric from


underneath the copper is exposed, more protective conditions  of the copper etching process are applied—ion dose rate is


decreased (beyond the second point of 1:1 selectivity in Fig.6)to finish copper removal without breaking through the


dielectric.


Though this method is qualitative regarding the moment when one should switch from low to high level of dielectric protection, properly applied it maintains good floor flatness while removing multiple copper layers to reach a target line. An example of such a circuit edit job is shown in Figure 7. A  series of metal and dielectric layers are evenly removed to access a low level metal signal (metal 3) with good floor uniformity. Once metal 3 was evenly exposed it was easily isolated from the rest of the circuit (see dark spot in the middle of bottom right image of Figure 7).


Figure 7. Series of micrographs demonstrating even removal  of metal and dielectric over 4 layers of interconnect using 1:1 selectivity between metal and dielectric. ILD7 is SiO2, all  the others are low-k. Micrographs on the left are exposures of fill metal and on the right their removal. An isolating cut  in M3 layer is shown.


Cutting thin copper lines in tight circuitry


In the previous section, we showed a successful removal of multiple layers to reach a target line. Once at the signal level  line of interest, the process is adjusted for high selectivity to metal. Today’s advanced processes are able to produce very thin layers of interconnect material. Where once there was almost a micron of material thickness now there is much less  than half a micron. On top of that, line widths and spacing between lines have become less than 100 nm, which means that editing these devices requires performing FIB operations  in boxes with geometry similar to these dimensions. Normally  both, x and y dimensions of the box are required to be this small. Therefore the box area shrinks down to about 0.01μm2.


This has added to the difficulty of cutting metal signal lines because typical FIB current density is too high for this small  area of a FIB box and reducing the FIB current and current density makes imaging difficult. In order to control the effects  of the ion beam we use currents on the order of 1pA or lower. At this level, endpoint detection and imaging had to be improved and a secondary detector was appropriately designed to improve collection efficiency.


The low beam current operation has given us control of the process such that when cutting a copper line there is no undercut and the risk of shorting to an underlying metal line  is reduced. If the process is aggressive, the dielectric underneath the metal line can be damaged causing a short to  a metal line below (Figure 8, image on left).


Figure 8. Left –90nm wide line was cut using an excessive ion dose rate. Underlying dielectric is damaged and broke through to the next layer. Right -cut of a similar line with reduced ion dose rate and the same pre-cursor pressure. Dielectric is not over-etched and the cut is clean.


Alternatives


As the number of interconnect layers grows, access to a circuit node through the bulk silicon is offered as an alternative. Although this alleviates some of the concerns


regarding clearing large areas of the chip it still does not  alleviate the issue of selectivity between copper and lowk. In addition, approaching a circuit through the silicon(bulk or SOI) generally prohibits large area clearing and may make the requirement for copper selectivity and oxidation greater than for front side edit work. In addition, the proliferation of flip chip technology has been  relatively slow and represents a minority technology for the industry.


In order for a circuit edit process to scale it must do so not only in two dimensions as was traditionally necessary but instead in three dimensions and be able to handle copper and low-k dielectric materials. We have presented  how a variable selectivity copper and low-k process can assist in the scaling of the process and how it also addresses issues of evenly clearing dielectric with copper  embedded in it for access to a lower level node.  We also  show that low beam current (in the 1 pA range) helps control the beam and avoid undercutting of copper that can cause undesirable shorts.


1. JR Phillips, DP Griffis, PE Russell “Channeling Effects  during Focused-Ion-Beam Micro-machining of Copper”, JVSTA 18 (2000) 1061.


2. V.V.Makarov, W.B.Thompson, and T.R.Lundquist“Uniform Etching Copper over Organic Dielectrics”Proc. 5th AVS Inter Conf Microelectronics and Interfaces (2004) 186


3. S.Motegi, T. Ohuchi, T.R.Lundquist, and V.V.Makarov, “Addressing the Challenges of Editing Copper Devices”, Proceedings of LSI Testing Symposium, Osaka, Japan 10-12 November 2004


4. G. Carter, and J.S. Colligon, Ion Bombardment of Solids,Am. Elsevier (1968) New York.


Quantitative electrical analysis of FIB prepared vias on BiCMOS and CMOS090  designs


B. Domengès* and P. Poirier


*LAMIP,PPlaboratoire de microélectronique ENSICAEN-Philips, CNRT-CNRS,


Philips Semiconductor, 2 rue de la Girafe BP 5120, F-14079 Caen Cedex 5, FRANCE


In this study, the resistance of FIB prepared vias was  characterized by the Kelvin probe technique and their physical  characteristics studied using cross-sectional analysis. Two  domains of resistivity were isolated in relation to the ion beam  current used for the deposition of the via metal (Pt). Also submicrometer vias were investigated on 4.2 µm deep metal lines  of a BiCMOS aluminum based design and a CMOS 090  copper based one. It is shown that the controlling parameter is  the shape and volume of the contact, and that the contact  formation is favored by the amount of over-mill of the via into  the metal line it will contact.


With the increase of integration in ICs, typical device  modifications in FIB such as new connections through Pt or


TOS


W deposition have to deal with sub-micrometer vias reaching  deep metal lines. Though the resistance of such connections is  rarely a big issue because we are dealing with very low  currents of circuit operation, it appeared to us important to  quantify their electrical characteristics in relation with their  geometry, that is depth and size of the vias, the idea being to  improve their electrical quality and to be able to predict their  characteristics.


Experimental


Experiments have been performed on two different designs, a  BiCMOS one with four metallic aluminum based levels of  interconnect and a CMOS one with six copper based levels of  interconnect. Electrical characteristics were measured using  the Kelvin four-probe technique to avoid any influence of  probe contact resistance. That is, three different platinum  contacts were FIB prepared in each case on the same metal  line, allowing microprobing with four probes, two of them for  the voltage measurement and the other two for the current  forcing. For the BiCMOS design a Process Control Module  area was chosen, which consists of a superimposition of large  metal lines, in a staircase like design (Fig. 1). Contact from  the surface pad to each metal layer is ensured through stacking  of vias up to the fourth metal layer (M4 in Fig. 1(b)). For the


C090 design, a large M3 metal line with a large opened area  above it allowed preparation of three vias. Those should go  through or between upper metal filler layers, as seen in Fig. 5. Two series of experiments were performed. The first series  involved comparison of via resistance versus contact area  on  a mid-depth metal line (2.7 µm deep). The second series  studied the resistance of sub-micrometer vias (expected size


0.35 µm x 0.35 µm) with respect to contacted metal line  material of aluminum and copper based designs. Insulator  Enhanced Etching (IEE) gas (XeF B2B) was used to limit  redeposition effects, providing as high as possible aspect  ratios (ratio of the depth of the via over the width).


Subsequently to electrical characterization, cross-sections  were used to relate electrical performance and geometrical  characteristics.


Figure 1: a) Optical image of  Process Control Module used for via  experiment on BiCMOS design. b) Cross-section drawing of process  control module


Evolution of resistance versus contact area


Table 1 gives contact geometric characteristics and their  corresponding resistance. Indicated resistance values are mean  ones over the three identical vias. Resistance and via shape


are supposed to correlate according to the formula : R =  x L


/ S, where  is the resistivity of the deposited Pt (in fact a  mixture of C, Pt and Ga), L is the height of the via (or depth  of the contacted metal line) and  S is the cross sectional area  of the via. It clearly appears from table 1 that the relationship


M4 M3


M2


M1


poly


oxide


passivation


vias


b a


75 µm


M4


M3


poly  M4


## Quantitative electrical analysis of FIB prepared vias on BiCMOS and CMOS090 designs


67


of resistance versus the inverse of via area is not perfectly  linear. From the solid curve of figure 2, two different regimes  could be distinguished:  the low section values and the  sections higher than 2 µm². Furthermore, for low area values, one via out of three would show a much higher resistance than  the two others, indicating a rather bad reproducibility of the  experiment (in that case, those were not considered for the  calculation of the mean R value).


Table 1: BiCMOS M3 contacts : geometric parameters and  resistance


|Window size for access to metal line (µm²) |Theoretical via area S (µm²) |Theoretica l 1/S (µmP-2P) |Mean resistance value over the 3 vias ( ) |
|---|---|---|---|

|0.7 x 0.7 |0.49 |2.04 |405 |

|1 x 1 |1 |1 |186 |

|1.4 x 1.4 |2 |0.5 |136 |

|2 x 2 |4 |0.25 |45.9 |

|2.4 x 2.4 |5.76 |0.173 |26.1 |

|3 x 3 |9 |0.111 |16 |

|4 x 4 |16 |0.062 |6.8 |

Figure 2 : Evolution of via resistance versus theoretical and  measured via section. Lower 1/S value region is enlarged.


Cross sections have been performed to allow a true evaluation  of the via volume. It appeared that they were quite smaller  than expected even though Insulator Enhanced Etching (IEE) gas (XeF B2B) had been used for drilling the vias. They also show  some small voids and that the bottom surface of the vias is not  perfectly flat, leading to a much smaller contact surface than


pA05/24/06TiltMagHFW


2μm


expected or simply deduced from the aspect ratio of the


5.0011:53:1345.0°50.0 kX6.08μm


11.4x1.4


openings. Minimum contact area is considered to be  representative of the quality of the contact and is given with  corresponding R values in table 2 and represented by the


dashed curve in figure 2. Cross-sectional images of 1.4 m x


1.4 m vias are also shown Fig. 3, a big void explaining the  bad resistance in one of it.


Table 2: BiCMOS M3 contacts: measured geometric  parameters and resistance values


|Window size for access to metal line (µm²) |Minimum measured side length (µm) |Minimum measured Area (µmP2P) |Measured resistance value ( ) |
|---|---|---|---|

|0.7 x 0.7 |0.51 |0.26 |405 |

|1 x 1 |0.88 |0.77 |194 |

|1.4 x 1.4 |1.04 |1.08 |146 |

|1.4 x 1.4 |0.34 |0.11 |566 |

|2 x 2 |1.76 |3.1 |45 |

|2.4 x 2.4 |2.27 |5.15 |25 |

|2.4 x 2.4 |2.27 |9.67|15|

|3 x 3 |3.11 |9.67 |15 |

|4 x 4 |4.04 |16.16 |7 |

Figure 3. FIB cross section images of two 1.4 µm x 1.4 µm  vias. Note the voids in the bad via


The slope of resistance, R vs area, S, shows a break for via  sizes around 2 µmP2P (fig. 2). This could be related to FIB GaP+P


BiCMOS – via 1.4 x 1.4 - 566  M3


BiCMOS – via 1.4 x 1.4 -  146


Resistance versus inverse section


200人


。300


400


△


600


4.00


6.00


8.00


10.00


1/S (1/µm²)


Theo S Min S


50 100


150 200


.△


4.0015:03:0645.0°50.0 kX6.08 μmt


250


PA05/17/06TiltMagHFW


zirw


0.500


1.000


1.500


Contac t res is tance v ersus  inv erse s ec tion


0.0


20.0


40.0


60.0


80.0


100.0


120.0


140.0


160.0


180.0


200.0


ion current. It has been shown that resistivity of deposited Pt  increases with loop time, which is directly related to ion beam  current and window size [1, 2]. For intermediate size vias, the  loop time might not have been optimized, especially since the  ion beam current was higher than the theoretical one (1.6 pA  for 1 pA and 8.9 pA for 4 pA), because of a worn beam  defining aperture.


It is also interesting to note that the derived resistivity of  deposited Pt is much higher than that observed in the  literature. For instance, considering the 4 µm x 4 µm via, one


calculates  = 4200 µ cm, at least four times typical  resistivity of Pt straps. This confirms that role of the interface  between metal and deposited Pt, which probably results in a  contact resistance between platinum and Al or Cu. Its value  will also depend on the shape and area of the contact making  the expression of via total resistance more complex as  presented above.


Table 3 . Calculated BiCMOS M3 contact resistance


Window size for  access to metal


line (µm²)


Minimum  measured  Area (µmP2P)


Measured  resistance  value ( )


Contact resistance


1 x 1


0.77


194


152.2


1.4 x 1.4


1.08


146


127.5


2 x 2


3.1


34.5


2.4 x 2.4


5.15


18.7


3 x 3


9.67


11.7


4 x 4


16.16


7


Figure 4 : Evolution of contact resistance versus measured  via minimum area.


In an attempt to evaluate this contact resistance between  platinum and Al or Cu, we could calculate the theoretical  resistance of the vias, based on a square resistance of 12  for


deposited platinum, that is a 1200 µ cm resistivity, using the


expression R =  x L / S, with L = 2.7 µm and S as the  minimum measured contact area. To limit the influence of bad  filling and aspect ratio of small vias, we shall only consider  the largest ones. Resulting contact resistance values are given  in table 3 and its evolution versus contact area in figure 4.


Though the contact resistance should be considered as roughly  evaluated, it is interesting to note that its evolution shows a  break in the slope for contact areas around 2 µmP2P. We think of  a series of experiments that might allow sharpening these  measurements.


Characterization of sub-micronic vias


A second set of experiments was carried out in order to  compare sub-micron vias on 4.2 µm deep metal lines in  aluminum and copper-based designs. The smaller window  size, 0.7 µm x 0.7 µm was chosen to drill three contacts to M2  lines in the BiCMOS design and to the M3 line in the  CMOS090 design. Initial experiments showed a bad  reproducibility with some very high resistance value, mainly  due to an inadequate procedure. It was based on drilling the  three vias before their filling. We think this might favor the  redeposition of a very thin oxide layer prior to Pt deposition. This was corrected and the following steps were followed for  each via: drilling the via using XeFB2B gas (0.2 µs dwell, - 100% overlap) with an 11 pA current; direct filling of the via using a


0.2 µm x 0.2 µm x 4 µm window and 1 pA current. Table 4  gives details of electrical and geometrical measurements.


Table 4 . Sub-micronic contacts : geometric parameters and  resistance


Design


R (k )(Via 1)


R (k )(Via2)


R (k )(Via3)


Measured


section (µm²) Via 1 Via 3


BiCMOS


3.15


3.98


0.185 0.13


CMOS090 1.93


2.36


3.71


0.48 0.17


To evaluate via cross-sections, the area of the contact had in  two cases to be modalized by trapezoidal figures, as deduced  from FIB cross-section images (Fig. 5). Dependence of the  resistance of the contacts is linear with the total area of the  contact (Fig. 6). It is interesting to note that the nature of  metal doesn't seem to influence the electrical resistance of the  contact, the main parameter being the surface contact area. Indeed, drilling through the metal line will allow a larger area  of contact and thus a lower resistance.


pA03/16/06tilMagHFW


13.020:07:0545.035.0 kX8.69 μm


Figure 5. FIB cross section images of two vias. Note the protruding via inside the M3 metal line of CMOS090 design.


Figure 6. Evolution of via resistance versus measured via section.


BiCMOS – via 1


During this study, we confirmed that resistance of FIB vias is roughly linearly dependant on contact area. The study of the relationship of the resistance on a wide spectrum of areas  showed that the resistivity of the FIB deposited platinum varies with the Ga+ ion current used in relation to the loop time. Also, it appeared that to improve the resistance of a submicrometer via, it might be useful to drill deep inside the metal line to be contacted in order to increase the area of the  contact.


We wish to thank J.M. DALLET for performing four-probe


pA03/16/06TiltMagHFW


2 μm


13.017:48:2345.0°35.0 kX8.69 μm


qubic3 M2 via1


resistance measurements.


This work was supported by "Conseil Régional de BasseNormandie".


CMOS090 – via 3


M6, M5, M4


[1] Tao T., Ro J.S., Melngailis J., Xue Z. and Kaesz H.D., J.Vac. Sci. Technol., B8 (1990), 1826-1829


[2] Puretz J. and Swanson L.W., J.Vac. Sci. Technol., B10(1992), 2695-2698


1.5 2


y 03


w3.5 4


Study on the Effect of FIB Electron Beam Assisted Platinum Deposition on TEM Sample Analysis


Jianqiang_Hu, Jing_Zhou, Ming_Li, Qiang_Gao, Chorng_Niou, Kary_WT_Chien


Reliability Division, Semiconductor Manufacturing International (Shanghai) Corp.


18 Zhangjiang Road, PuDong New Area, Shanghai, China 201203


Electron beam assisted platinum film deposition has been found to be an effective method to protect the sample surface for both FIB and TEM analysis. In this paper, the phenomena of electron beam assisted deposition of platinum will be reviewed The results suggest that a 45 nm thick residual Pt film can effectively protects (100) silicon from damage induced by ion beam assisted Pt deposition. A carbon based organic layer under the electron beam assisted Pt has been observed. The mechanism and results on exposed oxide thickness measurements will be discussed. It is suggested that a carbon glue cap be used as a protective layer or


decomposed carbon


polysilicon be deposited in line before submitting the wafer


based gas


for TEM sample preparation and observation.


亚港港


Key words: FIB (focused ion beam), electron beam, TEM


precursor


organometallic


deposited metal


Focused ion beam (FIB) instruments have become extremely useful in the semiconductor industry because of advantages such as highly accurate position localization and stress free milling. With the combination of both ion beam and electron beam columns on the same platform, the dual beam (DB) FIB system has become much more versatile compared to a single column FIB system. Besides imaging, milling and chemical vapor deposition (CVD) with the ion beam column, the DB FIB system allows for scanning electron microscopy (SEM)imaging and electron beam assisted material deposition.


These capabilities combined in one system provide more efficient and enhanced techniques for transmission electron microscopy (TEM) cross­section specimen preparation.


With different extractor voltage and currents, the highly focused ion beam derived from a Ga+ liquid metal ion source removes the material by milling the specimen. The secondary ions and secondary electrons emitted from the interaction between the beam and the target material are collectedand can be used for imaging. The ion beam assisted CVD process involves the introduction of an organometallic gas precursor to the surface of the target material and the decomposition of the precursor by focused Ga+ ion beam in the defined pattern.


The interaction between the ion beam and the precursor results in the depositionof a metal film and the release of the volatile carbon based gas molecule. The process of electron beam assisted CVD is very similar to that of ion beam assisted CVD except that it is electrons rather than the Ga+ ion that is used to decompose the precursor. With the lower energy, the electron beam assisted Pt depositioncreates less damage to the sample surface than with ion beam assisted Pt deposition. [1]The process of electron beam assisted deposition is outlined in the schematic shown in Fig. 1.


Figure 1. Schematic drawing of the electron beam assisted metallicmaterial deposition.


In this paper, the discussions will focus on the phenomena related to electron beam assisted deposition of platinum, its effect on the formation of an amorphous layer on single crystal silicon as well as artifacts of an organic residue layer induced by electron beam assisted Pt deposition


The FEI 835 dual beam FIB system was used for TEM sample preparation studies in this paper.


Trimethyl–methylcyclopentadienyl–platinum (C9H16Pt) was used as the organometallic precursor. The voltage of the electron gun during electron beam assisted deposition was set to 5 kV. Similarly, the voltage and current for ion beam assisted Pt depositionwere 30 kV and 30 pA respectively. For both ion beam and electron beam assisted Pt depositions, the dwell times were 20us per pixel with an overlap of 200%


71


Effect of the electron beam assisted Pt film thickness on the (100) Si amorphous layer


Although the depositionefficiency of ion beam CVD is much higher than that of electron beam, [2] the direct ion beam assisted Pt deposition is not preferable due to the damage to the structure of interest during the actual deposition process.


Both electron beam and ion beam deposited Pt films will be discussed. Fig. 2a shows the schematic drawing of the final TEM sample prepared with FIB system techniques. The structure of interest was capped with both electron beam and ion beam assisted Pt films. The frame part at the top of the specimen represents the ion beam assisted Pt layer that has been destroyed during ion milling. This implies that the sacrifice of the Pt layer protected the structure of interest during FIB milling preparation for TEM analysis. The TEM image, in Fig. 2b, is a polysilicon structure that was capped with an electron beam assisted Pt layer. It has been fully protected from the focused ion beam induceddamage.


Figure 2 (a) Schematic drawing of FIB prepared TEM membrane with both E­beam and I­beam assisted Pt deposit on the structure of interest. (b) TEM image showing polysilicon completely protected by E­beam and I­beam assisted Pt layer.


Here the thickness of the E­beam assisted Pt layer is important. It is obvious that if the E­beam layer is not thick enough, the high­energy Ga+ ions can still penetrate through the thin film and damage the sample surface. Similarly, with a much thicker E­beam deposited Pt films would yield lower sample preparation efficiency. In the TEM image in Fig. 3a,a 20nm amorphous layer exists under the E­beam deposited Pt film whose thickness is about 30 nm. When the thickness of the E beam deposited Pt film was increased from 30 nm to 70 nm there was no underlying amorphous layer formation, as shown in Fig 3b.


Fig 3 TEM images showing the effect of the thickness of the E beam deposited Pt film on the underlying Silicon surface.; (a)Pt film thickness = 30 nm (b) Pt film thickness = 70 nm.


To study the effects of different thicknesses of E beam deposited Pt films for eliminating damage to the underlying silicon we designed an experiment. As outlined in the schematic drawing in Fig 4, three layers of electron beam assisted Pt with different rectangle patterns were deposited on the target sample one after another. (Refer to Fig. 4 for the


location and dimension of the rectangle patterns). The ion beam current, which contributes to the deposition rate, was set to 30 pA. The thickness of Pt (Z value) for all three rectangle patterns were set to 0.1 um. Thus the initial thickness of electron assisted Pt in area Ⅰ ,Ⅱ and Ⅲ was expected to be different (thickest at area Ⅲ , thinnest at area Ⅰ). Following the E beam Pt deposition, a one micron ion beam induced Pt layer was deposited over the structure.


Fig 4. A schematic drawing of the test structure consisting of electron beam assisted Pt deposited on Silicon with three rectangle patterns to study the effect of different E beam Pt thicknesses on preventing damageto the underlyingsilicon.


Fundamental consideration for CDM (Charged Device Model) breakdown was investigated with 90nm technology products  and others. According to the result of failure analysis, it was  found that gate oxide breakdown was critical failure mode for  CDM test. High speed triggered protection device such as  ggNMOS and SCR (Thyristor) is effective method to improve  its CDM breakdown voltage and an improvement for  evaluated products were confirmed. Technological progress  which is consisted of down-scaling of protection device size  and huge number of IC pins of high function package makes  technology vulnerable and causes severer CDM stress. Therefore, it is expected that CDM protection designing tends  to become severe. In order to solve these problems in the  product, fundamental evaluations were performed. Those are a  measurement of discharge parameter and stress time  dependence of CDM breakdown voltage.


Peak intensity and rise time of discharge current as critical  parameters are well correlated their package capacitance. Increasing stress time causes breakdown voltage decreasing. This mechanism is similar to that of TDDB for gate oxide  breakdown. Results from experiences and considerations for  future CDM reliable designing are explained in this report.


I. Introduction


This CDM was begun to make a mark in the point of  reproducibility of the failure caused by ESD (Electrostatic  Discharge) in the filed where semiconductor devices are  handled directly. Over 20 years passed after an appearance of  CDM (Charged Device Model) testing which is one of ESD  testing method for semiconductor device. Various types of  CDM testers were developed and phased-in as CPM (Charged  package model), Field-induced CDM tester and Hg-relay type  CDM tester [1-11]; we are investigating the fundamental  consideration of the parameters for CDM destruction since  CDM tester developed [12]. Some reports about reconsideration about for CDM tester specification and testing  method tend to be appeared recently [13].


On the other hand, development of semiconductor products is  drastically progressed. Silicon die with 65nm technology node  started to be shipped and high-performance BGA has taken  root in typical package. In general, down scaling of  semiconductor device is the one of sensitive factor for CDM  breakdown because of lack of energy change in source of  CDM stress. So consideration for protection device and circuit  is main item for against CDM breakdown.


We performed the fundamental consideration in the point of  mechanism for CDM breakdown by using the products and  TEG (Test Element Group) of Toshiba 90nm and 130nm  technology at this time. We reported the results of our  investigation about a confirmation for the typical CDM  breakdown in accordance with the result of physical and  electrical failure analysis. And a consideration for capacity  and discharge phenomenon from each type of packages (BGA  or another) is also main item of investigation. There is one  more concerned item which is possible to be problem in CDM  testing parameter of the future products.


II. Test


(1) About CDM


A simple concept of CDM is explained at first. Charging in  the semiconductor device by induction from charged object or  by tribo-electric with the sliding becomes a source of CDM  discharge. Air discharge which is caused by an approach of  charged device to GND and direct contact discharge is caused  by contact with charged device and GND are typical discharge  phenomena. Then, a drastic discharge current from charged  body is flown to GND through the pin of IC, and failure of  device will be caused by this current. This is simplified CDM  breakdown model.


HBM (Human Body Model) and MM (Machine Model) are  famous for general ESD models except for CDM. These are  established by a discharge from charged objects that are  assumed as human and machine for device handling. On the  other hand CDM is established by the discharge from charged  device. This is the different point and it is recognized that  CDM is more reproducible model in the point of realistic for


## Fundamental Considerations for CDM failure in 90nm Products


55


ESD failure in the field. There are many specs for CDM  testing method but these specifications are quite different each  other. ESD Association standard which had the severest specs  was mainly adopted in this investigation.


|PKG |x(mm) |y(mm) |Body thickness |
|---|---|---|---|

|P-TFBGA128 |7 |10 |0.87 |

|P-TFBGA317 |11 |11 |0.95 |

|P-TFBGA345 |12 |12 |0.95 |

|P-FBGA121 |10 |10 |1.0 |

|P-FBGA277 |13 |13 |1.1 |

|P-FBGA361 |15 |15 |1.07 |

|P-BGA272 |27 |27 |1.86 |

|P-BGA456 |27 |27 |1.86 |

|P-BGA736 |35 |35 |1.86 |

|E-BGA540 |42 |42 |1.4 |

Inner Resistance


of Device


Inner Inductance


Device


Capacitance


Resistance of


Discharge path


而OND


Fig.1 Equivalent Circuit for CDM Discharging


(2) Test


CDM Tester HED-C5000 (Hanwa Electronics Ind. Co., Ltd) was used for an evaluation. Three types of CDM testing  specification which is explained in chapter 2-(1) are available  by changing discharge kit.


Toshiba products of 90nm and 130nm are mainly used for an  evaluation and its list is shown in Table1. RISC core and  Analog core are installed in each product, respectively. And  more, TEG which has protection circuit with 130nm  technology is also used. Typical CDM breakdown  phenomenon was considered by analyzing of failure point  caused by CDM test with these test vehicles.


Various types of package, BGA as a representative, are  evaluated to obtain a capacitance for electrostatic as a  parameter CDM failure. A list of evaluated package with their  dimensions is shown in Table2.


Observation of discharge current caused from the product  with these packages was done by using Tectronix Transient  Digitizer SCD-5000 (band width 4.5GHz) and current  transducer (current probe).


Table1. List of evaluated products


||Technology Package Protection Device |Technology Package Protection Device |Technology Package Protection Device |
|---|---|---|---|

|Product-A Product-B |90nm |P-FBGA453 |ggSCR |

|Product-A Product-B |90nm |P-BGA456 |ggNMOS |

|Product-C Product-D |130nm |T-BGA868 |ggSCR |

|Product-C Product-D |130nm |P-BGA388 |ggSCR |

|TEG |130nm P-BGA388 -- |130nm P-BGA388 -- |130nm P-BGA388 -- |

Table2. List of evaluated package


III. Result and Consideration


(1) Study of CDM failure in the products


For the study of typical failure in 90nm technology product, CDM test for Product-A and Product-B was performed, and  their failures were considered in the point of both the circuit  diagram and physical analysis. Observed pictures of physical  analysis and their circuit diagram around failure points are  shown in Fig.2. Those of 130nm technology products (Product-C and Product-D) are also shown in Fig.3 to  compare each other.


It is found that CDM failure of both Product-A and Product-B  were caused by gate oxide breakdown. Ground gated NMOS (ggNMOS) was used as ESD protection device in Product-A  and ggNMOS triggered thyristor (ggSCR) was used in  Product-B, respectively. Although a structure of protection  circuit is different, gate oxide breakdown was caused as  common failure modes in CDM test for both products. A  similar result was obtained by test of Product-C and ProductD, that is, gate oxide breakdown was also observed in 130nm  technology products. SCR was used as protection device in  these products.


In general, CDM is the failure model which discharging  speed is the fastest in well-known ESD models. Schematic  image for compassion of discharge waveform is shown in  Fig.4.


Therefore, protection device which is optimized against for  the breakdown in HBM and MM is insufficient as the  protection circuit for CDM in the point of discharging speed. Before starting to operate, CDM discharge stress flows into  inner circuit and causes failure there. This is well-known  mechanism and reason why inner device tends to be failed in  CDM [8, 17-23].


There are some typical failure modes of CDM. Those are gate  oxide breakdown caused by tunneling current under high  electric field condition, melt filament of pn-junction caused by  high current through undersized pattern, interlayer dielectric  breakdown caused by high voltage apply and metal line


failure caused by high current through narrow lines. This  result agrees with these understandings in the point of gate


VDDC


oxide breakdown. In general, it is understood that high speed  triggered devices such as above-mentioned ggNMOS and


VDD


ggSCR are effective for protection circuit for CDM failure. A  replacement with high trigger speed device such as ggNMOS,


Breakdown!!


ggSCR and an optimization of their device dimension are  effective method for an improvement of CDM breakdown  voltage.


A result of optimization is shown in Table3. It is found that all  CDM breakdown voltage of these products were improved. According to these results, we conclude that gate oxide  breakdown is one of the most critical failure modes in CDM  for 90nm technology node products and this tendency is not  changed from 130nm technology. Protection circuit with high  trigger speed device which is based on the same concept for  previous generation technology is effective improvement  method for CDM breakdown voltage, even if product were  designed in 90nm technology.


guaeypomujj


□儿光


口 Notπ


Fast!?


High Electric field


18888 47立


Fig.2. Result for CDM failure analysis of 90nm Products


(1) Observed picture of failure analysis (Product-A)


(2) Circuit diagram around failed point (Product-A)


(3) Observed picture of failure analysis (Product-B)


(4) Circuit diagram around failure point (Product-B)


(1)                          (2)


Breakdown!


S5日000 0000


IS


Fig.3. Result for CDM failure analysis of 130nm Products


(1) Observed picture of failure analysis (Product-C)


P-well


(2) Observed picture of failure analysis (Product-D)


(3) Circuit diagram around failure point (Product-C)


Table3. Result of CDM breakdown voltage after improvement


||Before After |
|---|---|

|Product Product- -A B |+750V / -1000V +/- 1000V pass |

|C D Product- Product- |+500V / -500V +/- 1000V pass (+1kV-pass) / -800V +/- 1000V pass |

Improvement


Failed under Contact


+500V / -500V


+/- 1000V pass


1.5 kv xee.ok 1.s0nm


Fig.4. Comparison of typical discharge current waveform for  each ESD models (CDM, HBM and MM).


(Voltage value is set as typical judge condition for each type  of ESD model. “4pF” in CDM is for small module condition  of ESD-A specification.)


8.0


Fig.5. Procedure of package capacitance measurement


Ip1


(1) Charging by DC power


6.0


90% Ip1


(2) Drop into Faraday Cup and read Coulomb meter


Td


-10%Ip1


Ip3


N0.0 1


ground plane


-2.0


pago pin


Ip2


-4.0


heat slug


0.510


Fig.6. Schematic image of parasitic capacitance for CDM  charging [24]


time [ns]


PKG-size vs C-PKG


-10


-5-


200V MM {052}


020


土30


10 E5


2XAH8W}00{


40 50


1kVCDM4pF


01020304050


Area (mm2)


C-PKG vs RiseTime @500V


0 100 200 300 Rise Time (ps)400 500


面


C (pF)


∠41


C-PKG vs Ip@500V


meter


Coulomb


5 10


V d


15 20 25


Faraday Cup


C(pF)


die attach


iOp ia


TIME (NANOSECONDS)


lusniegoJ


yajpo ueu6u6d jeie


Fig.7. Correlation Package capacitance versus each  parameter


HV source


(1) Package size, (2) Rise time, (3) Peak current, Peak current


and rise time were obtained at 500V stress condition. (4)


非=


Schematic image of discharge current (Td indicates Rise time  and Ip1 indicates peak current.) [15]


(2) Capacitance and Discharge Phenomenon of Packages


We confirmed both the capacitance for various types of  packages which would be a source of electrostatic and an  actual phenomenon of CDM discharging to consider reliable  CDM designing in the future. Although we had data of  traditional package such as DIP, QFP, etc, there are few  reports about that of BGA type packages. We confirmed this  data which is essential items for current 90nm generation  product. Packages which their list is shown in Table2 were  used for this experiment.


Faraday Cup is used for measurement of package capacitance  and schematic image of its measurement procedure is shown  in Fig.5. First, charging is done through IC pins by using DC  power supply. Then, it is made drop into Faraday Cup. Total  charge is measured by Coulomb meter and it is changed to  capacitance by calculation. Finally, an observation for  discharge current from each package is done for the  consideration in the point of correlation between package  capacity and CDM stress.


There are many inner parasitic capacitances which are  generated by the encapsulated materials or portions, as shown  in Fig6. Although they need to be considered for the detail  electrostatic capacitance, the capacitance was measured on an  assumption as unity capacitor for simplified consideration of  relationship between them and other parameters at this time. Then, a mechanism for CDM failure is investigated by the  parameters in discharge waveform.


Correlations between capacitance and related parameters  which are package body size, peak current intensity and rise  time of discharge waveform are shown in Fig7, respectively. Rise time and peak current of discharge current waveform  were obtained at 500V stress condition. From these results, it  was found that every parameter has good correlations for  capacitance but its interpretation would be a little complicated. Fig.7 (1) indicates that large package has large capacitance. In  case that charged device drop on the ground is considered as  natural using condition, smaller capacitance becomes severer  condition and there was the same understanding [7]. Fig.7(2) gives us an additional understanding, that is, rise time of  discharge current is faster in smaller package. As it was  discussed in previous chapter, high trigger speed was  important factor for CDM reliable designing. So it is possible  to understand that smaller capacitance is severer factor for  CDM failure.


However, a gate oxide breakdown as critical failure mode  gives us another interpretation. Fig.7 (3) indicates that peak  current is increasing with larger capacitance. Higher leakage  current through gate oxide film is critical problem in the  reliability of general oxide film. The detail of this concern will  be discussed in next chapter as a consideration for change of  breakdown voltage.


(3) Change of breakdown voltage


Gate oxide breakdown as critical failure mode was confirmed  in previous chapter. There is concerned failure phenomenon  because of gate oxide breakdown. In particular, it will be  problem in 65nm or the latter-day technology which will be  mounted on the package which has huge number of IC pins  more than 1000 IC pins.


1 . 0 E - 1 0


1 . 0 E - 0 9:TDDB-NMOS


1 . 0 E - 0 8:TDDB-PMOS


1 . 0 E - 0 7


1 . 0 E - 0 6


1 . 0 E - 0 5


1 . 0 E - 0 4


1 . 0 E - 0 3


1 . 0 E - 0 2


1 . 0 E - 0 1


1 . 0 E + 0 0


1 . 0 E + 0 1


1 . 0 E + 0 2


TTF-TDDB (arb. Units)


1 . 0 E + 0 3


1 . 0 E + 0 4


2.2


2.8


3


3.2


3.4


3.6


Vg (TDDB) [V]


5 0 1 0 0 1 5 0 2 0 0 2 5 0 3 0 0


:CDM stress


3 5 0 4 0 0 4 5 0


CDM breakdown voltage


5 0 0


10000


Number of CDM stress (times)


Fig.8. Compared graph CDM stress time dependence of CDM  breakdown voltage and gate voltage dependence of TDDB  lifetime.


*Square indicates the data for CDM, circle indicates that for  TDDB.


TDDB is known for typical failure mode of gate oxide  breakdown. This is the model that a lower applied voltage for  long time causes oxide film breakdown. Increased leakage  current which flow through oxide film as tunneling current  keeps to damage during voltage applied, so time would be one  of the factors for breakdown.


There is a correlation between this TDDB failure model and  CDM failure. A product scale expansion such as increasing  number of IC pin raises a number of opportunities for CDM  discharge through critical MOSFET. This phenomenon causes  increasing of amount of CDM breakdown energy. Even if  CDM test condition is not changed in the point of stress times, energy for breakdown for critical portion would be increased  because of increasing of CDM stress time, eventually.


In order to consider this phenomenon quantitatively, CDM  stress time dependence for breakdown voltage was  investigated by using Product-A and TEG. Its result is shown  in Fig8. It is found that increasing of stress time causes the  decreasing of breakdown voltage. It is found that a increasing  of stress times from 3 times which is the common condition in  CDM test standard to 5 times cause about 20% degradation of  CDM breakdown voltage. In general, there is well relationship  between TDDB lifetime and gate voltage, higher gate voltage


causes lower TDDB lifetime. It is shown in the bottom graph  in Fig.8. Oxide film breakdown depends on the amount of  charge which is flown through the film. Therefore, it is  understood that a model for the degradation of CDM  breakdown voltage with increasing of CDM stress times is the  same as that of TDDB. As it is shown in Fig.7-(3), peak  current intensity tends to be higher in larger capacitance  package and this higher current causes higher applied voltage. There is a possibility of more CDM stress times will be  applied for a critical gate oxide film because the scale such as  IC pins, capacitance of packaged and peak discharge current  from it increases in developed and packaged product. Thus, CDM breakdown voltage might decrease even if the same  protection circuit and device are used. As discussed in section  3-(2), a consideration of protection device and circuit  triggered at high speed is indispensable. However, it is  understood that a scale of semiconductor product also needs to  be considered for CDM breakdown from the point of  breakdown energy which is expressed as a relationship  applied voltage and total CDM stress numbers of time.


Not only the trigger speed but also a scale of product must be  necessary for CDM reliability designing.  Now, Toshiba is  still investigating for future reliable product from the point of  accurate and quantified relationship for the these factors of  CDM breakdown


V. Conclusion


As a result of this evaluation for CDM failure mechanism, the following conclusions are obtained.


(1) Gate oxide breakdown was confirmed as critical CDM  failure mode in 90nm technology products.


(2) Improvement of CDM breakdown voltage in 90nm  technology is feasible by adopting of high trigger speed  protection device such as ggNMOS and ggSCR.


(3) Rise time is well-related with capacitance of packaged  product and this is critical parameters for CDM. Smaller  capacitance becomes severer condition in the point of trigger  speed.


(4) Peak current is well-related with capacitance of packaged  product and this is critical parameters for CDM. Larger  capacitance becomes severer condition in the point of gate  oxide breakdown based on TDDB.


In particular, CDM breakdown voltage will be degraded by  the increasing of total CDM stress time which is caused by  larger scale condition such as number of IC pins and larger  capacitance.


Not only the trigger speed but also a scale of product must be  necessary for CDM reliability designing.


Toshiba is still investigating future reliable product from the  point of accurate and quantified relationship for the these  factors of CDM breakdown


Reference


[1] T.S. Speakman, “A Model for Failure of Bipolar Silicon  Integrated Circuits Subjected to Electrostatic  Discharge.”, 12th Annual Proceedings, Reliability  Physics, 1974, p. 60-69


[2] P.R. Bossard, R.G. Chemelli and B.A. Unger, “ESD  Damage from Triboelectrically Charged IC Pins.”, EOS/ESD Symposium, 1980, p. 17-22


[3] Y. Fukuda, S. Ichiguro and M. Takahara, “ESD Protection  Network Evaluation by HBM and CDM (Charge  Package Model).”, EOS/ESD Symposium, 1986, p. 193-199


[4] R.G. Renninger, M.C. Jon, D.L. Lin, T. Diep, T.L. Welscher, “A Field-Induced Charge-Device Model  Simulator.”, EOS/ESD Symposium, 1989, p. 59-71


[5] R.G. Renninger, “Mechanisms of Charged-Device  Electrostatic Discharge.”, EOS/ESD Symposium, 1991, p  127-143


[6] K. Verhaege, G. Groeseneken, H.E. Maes, “Influence of  Tester, Test Method and Device on CDM ESD Testing.”, EOS/ESD Symposium, 1994, p.49-62


[7] M. Tanaka, M. Sakimoto, I. Nishimae, and K. Ando, “An  Advanced ESD Test Method for Charged Device  Model”, EOS/ESD Symposium, 1992, p. 76-81


[8] M. Chaine, C.T. Liong and H.F. San, “A correlation Study  between Different Types of CDM Testers and ‘Real’ Manufacturing In-Line Leakage Failures.”, EOS/ESD Symposium, 1994, p. 63-68


[9] M. Chaine, K. Verhaege, L. Avery, M. Kelly, H. Gieser, K. Bock, L.G. Henry, T. Meuse, T. Brodbeck, J. Barth, “Investigation into Socketed CDM (SDM) Tester  Parasitics”, EOS/ESD Symposium, 1998, p. 301-310


[10] M. Chaine, J. Barth, T. Brodbeck, L.G. Henry, M.A. Kelly, and T. Meuse, “The SDM Test Method: Past, Present, and Future”, Compliance Engineering


[11] L.F. DeChiaro, S. Vaidya, R.G. Chemelli, “Input ESD  Protection Networks for Fineline NMOS – Effects of  Stressing Waveform and Circuit Layout”, International  Reliability Physics Symposium, 1986, p. 206-214


[12] S.Inamasu, N.Wakai, et al., „The Fundamental  Consideration for Charged Device Model and Its Test  Method”, RCJ-EOS/ESD Symposium, 1994, p.73-78


[13] N.Kodama, T.Tsukagoshi, “Reconsideration of ESD  Tester for Charged Device Model”, RCJ-EOS/ESD Symposium, 2005, p.179-184


[14] JEDEC Standard JED22-C101C, “Field-Induced  Charged-Device Model Test Method for ElectrostaticDischarge-Withstand Thresholds of Microelectronic  Components”, 2004


[15] ESD Association Standard Test Method for Electrostatic  Discharge Sensitivity Testing Charged Device Model (CDM) Component, ESD STM 5.3.1-1999,


[16] JEITA ED4701/300 Test Method 305, “Charged Device  Model Electrostatic Discharge”


[17] C. Brennan, J. Sloan, D. Picozzi, “CDM failure Models in  a 130nm ASIC Technology”, EOS/ESD symposium,2004, p.182-186


[18] Y. Fong, C. Hu, “The Effects of High Electric Field  Transients on Thin Gate Oxide MOSFETs.”, EOS/ESD Symposium, 1987, p. 252-254


[19] Y. Fong, C. Hu, “Internal ESD Transients in Input  Protection Circuits.”, International Reliability Physics  Symposium , 1989, p. 77-81


[20] K.P. Cheung, “Plasma-charging damage and ESD, help  each other?”, EOS/ESD Symposium, 1999, p. 38-42


[21] C. Duvvury, A. Amerasekera, “Advanced CMOS  Protection Device Trigger Mechanisms during CDM.”, EOS/ESD Symposium, 1995, p.162-174


[22] K. Verhaege, C. Russ, J-M. Luchies, G. Groeseneken, F.G. Kuper, “Grounded-Gate nMOS Transistor  Behaviour under CDM ESD Stress Conditions.”, IEEE Transactions on Electron Devices, Vol. 44, No. 11, 1997, p. 1972-1980


[23] C. Russ, K. Verhaege, K. Bock, P.J. Roussel, G. Groeseneken and H.E. Maes, “A Compact Model for the  Grounded-Gate nMOS Behavior under CDM ESD  Stress”, EOS/ESD Symposium, 1996, p. 302-315


[24] M. Etherton, N. Qu, J. Willemen, W. Wilkening, S. Mettler, M. Dissegna, R. Stella, L. Zullino, A. Andreini, H. Gieser, H. Wolf and W. Fichtner, “Study of CDM  Specific Effects for a Smart Power Input Protection  Structure.”, EOS/ESD Symposium, 2004, p. 107-116


Development of a Circuit Edit Process Scalable in Dimension and Material


Vladimir V. Makarov Credence Systems Corporation, Sunnyvale, CA and Nicholas Antoniou


The ability to edit a circuit in silicon quickly and confidently is extremely valuable as it permits verification of changes or  fixes without the need to generate new reticles and fabricate new silicon. However, dramatic changes in the material used  in IC’s combined with the downward scaling of dimensions required the development of a scalable process not only in three dimensions but also in material. Details of this process and results are presented in this paper.


Semiconductor devices are continually being scaled down as per Moore’s law and adjustments to this law. At the sub 180  nm domain scaling has continued but is being accompanied by material changes that have little or no history in this field. Not only are the materials changing but also the physical layout of a chip is now considerably different than the “Blue  Print” of the design (GDSII data that is produced at the completion of design).


The toughest challenges facing CE today are listed below.


• Copper interconnect


• Filler metal, sizing and Optical Proximity Correction (OPC)


• Evolving low-k materials


• Feature shrinking, lateral and vertical


• Increasing number of interconnect layers


• Charge control


We describe how we scale the process by reducing the FIB volume of interaction with the sample and using a chemically  assisted process with variable selectivity between materials.


Copper Interconnect


Gallium Ion Beam sputter rates of traditional semiconductor  materials (silicon, silicon dioxide, aluminum, silicon nitride) are very similar. This allowed for even removal of areas of a  circuit regardless of the layout. Metal and dielectric could be  evenly and cleanly removed. This is not the case for copper and low-k dielectrics. Copper sputters at rates that differ by as  much as a factor of 4 depending on crystal orientation [1](See Figure 1). Low-k dielectrics sputter much faster than copper. A chemically assisted milling process was first developed to assist in the sputter of copper and to oxidize any


residual copper [2, 3]. Here we describe a new generation of this process whereby the low-k dielectric surrounding copper  is left intact when cutting a copper line and is removed at a similar etch rate to copper when the process is adjusted for clearing an area of dielectric with embedded metal so that a lower level signal can be accessed.


Figure 1. Straight sputter of copper with Gallium Ion FIB showing the difference in sputter rates between different crystal orientations.


What You See is Not What You Get


In addition to the scaling and new materials, CE engineers face other obstacles. Fill metal is used to improve planarity during CMP (chemical mechanical polishing) as a device is being built up. Circuit features are also adjusted often dramatically for photolithography. Optical Proximity Correction (OPC)


is needed as circuit feature size is shrunk but exposure wavelength of steppers is not. Features at 130 nm and 90 nm  are exposed using stepper light wavelength of 193 nm.


Adjustments such as those shown in Fig. 2 are made in the mask shop and the resulting files are not usually shared with  the analysts.


## Development of a Circuit Edit Process Scalable in Dimension and Material


62


Figure 2. Simple lines in GDSII are converted to intricate patterns for OPC and blank spaces are filled with metal lines  for better planarity of the circuit stack.


The TEM results in Fig 5 show the effect of the thickness of the E beam assisted Pt layer on the formation of an amorphous layer. It was our observation that the Si amorphous layer decreases as the thickness of the E beam deposited layer increases. When the thickness of the residual E beam Pt layer comes to 45 nm, there is no amorphous layer observed on the substrate surface. This result for a (100) Silicon substrate indicates that a residual 45 nm E beam Pt layer is sufficient to protect the surface from subsequent ion beam damage.


Fig 5 TEM image shows the thickness of the amorphouslayer changes with the thickness of the E beam Pt layer along the surface. There is no amorphous layer observed under the residual 45 nm E beam Pt film.


It should also be pointed out that the thickness of E beam Pt is certainly not the only factor that influences the formation of an amorphous layer on the sample, Other factors include ion beam energy, current, incident angle and the structure of the sample itself.


Organic residue layer induced by electron beam assisted Pt deposition


The resistivity of FIB­deposited Pt films is usually 10–5000 times that of pure Pt. [3] Ion beam induced Pt films incorporate


m


IT


impurity elements such as C, O and Ga. The amount of carbon


Pt deposited by


electron beamand gallium is influenced by the Ga+ ion flux and theorganometallic precursor flux. [4] The composition of the(100) si


deposited film depends on the extent of precursor dissociation


0.3um


as well as the efficiency of volatile byproduct diffusion away


一0.5um/


from the sample surface.


1 uim


Our studies showed that such a phenomena also happens in electron beam assisted Pt deposition and negatively effects


length


TEM observation of oxide defects. A detailed study was done to determine the impact of artifacts on oxide defect analysis.


As described in table 1, two wafers from the same lot were prepared for the experiment. Two TEM samples from wafer#01 were used for gate oxide pre­clean experiments. Sample 1a was capped with electron beam assisted Pt, and sample 1b was capped with carbon glue before the specimens were put into the FIB system. For a real process simulation, wafer #2 also underwent the same gate treatment as wafer #01,followed by a 25A gate oxide thermal growth and 1000 nm polysilicondeposition.Sample 2 from wafer #02 was prepared at the same test site as samples 1a & 1b, thus the thickness of the gate oxide under the polysilicon was expected to determine the effects of the pre­clean experiment. Since the structure of interest was the gate oxide, ion beam assisted Pt was directly deposited on the polysilicon.


|Wafer Number |Process Description |Sample Preparation Information |Sample Preparation Information |
|---|---|---|---|

|#01 |Gate oxide pre­clean |Sample 1a |E beam assisted P deposited as the protective layer |

|#01 |Gate oxide pre­clean |Sample 1b |Carbon glue capped as |

|#02 deposition |Gate oxide pre­clean + 25A gate oxide +1um polysilicon |Sample 2 |Polysilicon was in­line capped on gate oxide |

45nm


Table 1 Table describing the sample information for the experiment carried out to study the organic layer induced by electron beam assisted Pt deposition.


TEM results for sample 1a, 1b and 2 are shown in Fig. 6 a, b and c respectively. Fig 6a indicates the thickness of the oxide like layer under the E beam Pt to be 51A on sample 1a, which


100 nm


is an unexpected result. This bright contrast layer under the E beam Pt was thought to be caused by the E beam assisted Pt deposition. This suspicion was verified with the results of sample 2. In Fig 6c, the 25A gate oxide film under the polysilicon matches the target specification. This implies that there should be no oxide (or only a native oxidewith exposure to atmosphere) left over after the gate oxide pre­clean. In Fig


the protective layer


6b, an about 10A thick native oxide layer was observed under the carbon glue.


Figure 6 TEM images of experimental samples from Wafer #01 and #02 (a) Sample 1a, structure capped with electron beam assisted Pt deposition; (b) Sample 1b, structure capped with carbon glue before the sample was put into the FIB system; (c) Sample 2, structure capped with polysilicon.


A similar phenomenon was observed on an additional sample that consisted of an exposed structure of etched polysilicon.


From both TEM and STEM/EDX analysis (Figure 7a and 7b respectively), an organic residue under the E beam deposited Pt was detected along the sidewall of the polysilicon. Carbon,oxygen, gallium and platinum signals were detected within this layer. The silicon peak is thought to come from the sputtering of the Silicon substrate during FIB milling. These results indicate that the decomposition process of electron beam assisted Pt deposition is similar to that of ion beam assisted Pt deposition. ; The generation of impurities within the deposited films is due to the non­volatile, decomposed byproductor non­decomposed organometallic precursor.


51A


organic


10nm


6a


residue


10.8A


50 nm


7a


Right Fiatt


DankFiold


6b


00m


■EDXiBigtt Flaid Pslntt


中 B o 2


aGe


支型 0020


41060b


Figure 7: (a) TEM image showing organic residue along the sidewall of the poly silicon. (b) STEM image/EDX result of the bright phase organic layer showing the signal of carbon,oxygen, gallium,platinumand silicon.


5 mm


6c


Based on the discussion above, the impurity induced by electron beam assisted Pt deposition could make the measurement of the exposed oxide thickness unreliable. For analysis of oxideswithoutpassivation, the authors suggest that carbon glue rather than electron beam assisted Pt be used as the protective layer.. It is strongly recommended that polysilicon or a similar capping layer be placed on the oxide before the sample is submitted for TEM analysis.


Energy pixev)


From the TEM results of our study the following conclusions are made:


1. Electron beam assisted Pt deposition has been shown to be effective for protection of the exposed structure. A residual 45 nm Pt film can protect (100) Silicon from the damage induced by subsequent ion beam assisted Pt deposition.


2. Carbon based organic impurities resulting from the decomposition of the organometallic precursor can negatively affect the accuracy of TEM analysis. For thickness measurements of exposed oxides, a carbon glue or polysilicon film should be used as the protective layer prior to TEM analysis..


[1] B. W. Kempshall, L. A. Giannuzzi, B. I. Prenitzer, F. A.


Stevie and S. X. Da, J. Vac. Sci. Technol. B, Vol. 20, No.


1, (286) Jan/Feb 2002.


[2] S. Lipp, L. Frey, C. Lehrer, B. Frank, E. Demm, S.


Pauthner, and H.Ryssel, J. Vac. Sci. Technol. B 14, 3920(1996).


[3] T.Tao, J.Ro, J.Melngailis, Z.Xue, etc. JVST B8, 1826(1990).


[4] K.A.Taleri, B.R.Rogers, H.Fan, H.Shen, etc. JVST B 20(2) (590) Mar/Apr 2002


Experiment study on Crystal/Amorphous Structure of TEM Samples  Prepared by FIB Milling


Qiang Gao, Mark Zhang, Chorng Niou, Ming Li, W.T. Kary Chien


Semiconductor Manufacturing International Company PuDong New Area, Shanghai, China


It has been reported that a sample prepared by ion beam  milling has a sandwich structure with amorphous on two  sidewalls and crystal in the middle. In this paper, the  sandwich structure of such a single crystal TEM sample was  studied experimentally. A novel sample and its fabrication  process were reported. The sandwich structure can be observed  directly in TEM with this sample. When the crystal layer in  monocrystal silicon TEM sample is less than 18 nanometers, or  when the sample is thinner than 64 nanometers, the sample will  be observed as fully amorphous. Removal of the amorphous  layer on the sample sidewalls is crucial to get TEM pictures of  better quality


TEM (Transmission Electron Microscope) is one of the most  powerful instruments for IC (Integrated Circuit) analysis as  fabrication technology shrinks to deep sub-micron regimes. A high quality sample with few artifacts, high contrast and  definition is essential to TEM observation. However, the  TEM membrane is often damaged due to the implantation of  the high-energy ion beam, which greatly impacts TEM  analysis quality.


It has been reported [1] that the sample prepared using ion  beam milling has a sandwich structure with amorphous on  two sidewalls and crystal in the middle, as shown in figure 1. The sidewall amorphous layer attracted much interest


Fig. 1 Perspective schematic view of the TEM sample


because it has great impact on sample quality and its  thickness can not be observed in TEM directly. The top  surface damage of TEM sample is easy to be observed and  all previous research results are consistent with ours. For  sidewall damage, different results were obtained based on  different research methods [1-8]. A Monte-Carlo calculation  can simulate the impact of the ion and generate possible  routes for the ion and its effects. The ion will typically leave  a trail of vacancy-interstitial pairs, ending in a gallium  interstitial as the primary particle comes to rest. With many  such impacts, data can be accumulated to give a reasonable  approximation to the actual effects of many ion impacts. SRIM software is available for the calculation of penetration  depth and vacancy density. Walker et al. [2] investigated ion  beam damage to TEM sample prepared using FIB. The  reported amorphous layer is 5nm thick for glancing  incidence. Leslie et al. [3] studied the effect of tilt angle  between sample and beam on the degree of amorphization in  a pure silicon sample. Their results indicated that a sample  tilt angle of ±2ºfrom vertical position provides optimum  wedge removal conditions and the membrane remains as  single crystal. They also concluded that the degree of  amorphization/phase transformation is higher for more  sample tilt angles. Ishitani et al. [4] used EDX analysis to  determine gallium concentration in cross section. They  determined that the gallium concentration in silicon, due to  thinning using a 30 kV ion beam, was 4 at.% of the layer, on  the assumption that the implanted gallium was within the  first 10 nm of the sidewalls. Kato et al. [5] investigated the  depth of damage to a crystalline silicon caused by milling  using a 30 kV gallium beam and reported a 20 nm amorphous  layer, with the thickness being independent of beam current  over the range 100-500pA. Longford et al. [6] gave a HREM  image of the side edge of a silicon TEM cross section that  had been milled using a 500 pA beam current at 30 kV. The  amorphous layer was approximately 20 nm thick. The  physical thickness of the damaged layer is difficult to  measure directly due to the difficulties in preparing an  appropriate sample, and this leads to the disagreement  among different research. Suitable sample preparation  methods were reported in previous studies [1,8], which make  the direct observation of sidewall damage possible. The  physical thickness of amorphous layer is 23.5 nm with 30 kV  Ga+ milling on single crystal silicon, and the thickness  remains unchanged with beam current ranging from 30 pA to  1000 pA [1]. The measured damage layer is 22 nm with 50  kV Ga in reference 8.


Undamaged layer


Damaged layer


TEM Observation Direction


76


The diffraction contrast comes from intermediate crystal  fraction, while amorphous layer on both sidewalls contribute  little, or even do harm to the contrast. A general sample may


Orthogonal direction


provide qualitative information about amorphous rate when  viewed in a normal way in TEM through electron diffraction; however, you can not extract crystal from amorphous  because they are mixed together by electron penetration. In


Ta 355nmTc 455nm


this experiment, a series of processes were executed to build  a sample in which the sandwich structure can be directly


Positionmarker


inspected. With this sample, we can find out the critical


L810nm


thickness of TEM sample, and observe the thickness of the  crystal and amorphous layers in it.


Fig.3 TEM picture of the wedge sample. The bright contrast is  the full amorphous portion, marked as Ta. The bright area in the  silicon is the position marker.


Experiment


The sample was taken out of the TEM for subsequent  processing, to prepare the sample so it can be observed from the  orthogonal direction as shown in figure 3.


The cross section of a piece of silicon wafer was thinned  approximately to 20 micron in thickness with mechanical  polishing, and then mounted to a half copper ring. This  pre-thinned slice was fastened to the multi-stub holder and put  into FIB chamber, and milled, in the same ways as standard  pre-thinned sample preparation [7]. After the first side was  milled, the FIB stage, together with the sample, was rotated 15  degrees, and continued with second side milling. Then we  obtained a wedge shaped sample whose thickness changes  continuously at different positions along the sample, as shown  in figure 2. The small area near the thinner edge of the  membrane was totally removed with ion beam etching before  the final fine milling, This area will serve as a position marker  when the sample is observed in the TEM. For certainty, the  sample near the thinner edge will be viewed as full amorphous. Pictures of this sample were taken in TEM and the dimension  of Ta, Tc, and L was measured, as shown in figure 3. The  sample structure at the Tc and Ta interface aroused the greatest  interest. If we can view the sample from orthogonal direction as  shown in figure 3, we would see the structure evolution of the  wedge-shaped sample from the full amorphous at C side and  the thicker crystal at AB side. This direction is perpendicular to  face ABC in figure 2.


A drop of epoxy was coated on a smooth and clean cover glass. The sample was laid down onto the epoxy carefully, and  standing for sometime until the milled pit was filled with epoxy. One should take care not to immerse the whole sample in the  epoxy drop, because this will be an obstacle to subsequent  processing. Then the epoxy was solidified at 170 centigrade for  half an hour. The sample with the epoxy-coated face adhering  was then stuck to a piece of wafer. The wafer piece was  mounted to the multi piece holder of FIB and the holder was  inserted in the FIB chamber for further preparation using the “pick-up” method. Please be aware that at this time the milling  direction is parallel to the face ABC. The sample is a  cross-section of previous sample and its sidewall is parallel to  face ABC. Under careful control, the final membrane was  sampled at MM’ cross section as shown in figure 2. Figure 4 is  the overview of the sample observed in TEM. The “broken  sword” is the portion of the sample we are interested in. The  bright area surrounding the sword is the epoxy coated during  sample processing. The dark area is the silicon substrate. The  net structure is the supporting carbon film.


Position Marker


Epoxy


Tc Ta


support filmEpoxy


M’


Silicon substrate


Fig.2 Sketch map of the wedge sample


Fig 4 Overview of the final sample. The sword tip area is  corresponding to the 810 nm to the left position marker in  figure 3.


Results and discussion


Fig 5 Amorphous/crystal structure of the wedge sample  prepared using FIB milling.


Fig 6 Amorphous/crystal structure of the sample with critical  thickness. The 355nm is corresponding to the full amorphous  portion in fig 3.


Figure 5 is the overview of the sword tip. The sample structure, amorphous surrounded crystal, is clearly revealed as was  expected. One must take care to tilt the sample to the optimal  on-zone orientation for observation since electron diffraction  on such a tiny area is difficult because of the movement of the  sample during tilting. The dimension in figure 5 is consistent  with the Ta+Tc as shown in figure 3.


Figure 6 is the magnified sword tip in fig.5. The thickness of  amorphous and crystal at Ta and Tc interface was measured  respectively. The 355 nm segment in fig.6 corresponds to the  fully amorphous region observed in figure 3, while the  remaining portion in fig.6 is corresponds to the crystalline part  in fig.3. We can conclude from this the thickness at which a  TEM sample prepared using FIB ion beam milling no longer  appears crystalline under these conditions: 18 nm crystals in the  middle and 23 nm amorphous on each of the two sidewalls. Thus, with 30 kV Ga+ milling, the sample should be prepared  no thinner than 64 nanometers so as to avoid appearing fully  amorphous in the TEM under standard imaging conditions.


The 23 nm amorphous layer on each sidewall has great impact  on the quality of TEM sample. It also limits the practical  sample thickness to more than 600 angstroms. The critical  dimension shrinkage in modern IC fabrication demand thinner  gate oxide, narrow pitches and smaller defects. All these will  demand thinner TEM samples to get more clear information  from TEM analysis. To decrease the practical thickness of


TEM sample, we should remove the amorphous layers first. Broad beam (typically argon ion) milled samples have better  quality because the ions used typically have lower energy and  produce less damage to the sidewalls. As a standalone  technique, this method is not effective when precision location  is needed. There was several methods reported to reduce the  sidewall damage [4], such as gas assisted etching in FIB  chamber, broad beam milling after FIB milling, wet etching, and low kV FIB milling. Among all these methods, in our  experience, low kV FIB milling is more suitable for use in  failure analysis labs, and would be even more useful  if the FIB  resolution under lower accelerating voltage was greatly  improved.


A wedge shaped sample was fabricated using a pre-thinning  methodinvolving coating epoxy on one side of the sample to  build the support frame for a second sample preparation step at  90 degrees to the first thinning. The ”pick-up”  method was  then used to fabricate the final sample. With this sample, the  direct observation in TEM of the  amorphous /crystal/amorphous sandwich structure of the TEM sample  becomes possible. When this crystalline layer is less than 18 nm, the sample will be observed as fully amorphous in TEM under  standard imaging conditions. To avoid the monocrystlline  silicon portion of the sample appearing amorphous in the TEM, the total thickness of the sample should be no less than 64 nm  when prepared using 30 kV Ga+ FIB milling.


1. Qiang Gao, Mark Zhang, Chorng Niou, Ming Li, W.T. Kary Chien, Observation of the crystal damage on the  sidewalls of TEM sample prepared using FIB, Proc. ISTFA’2004, p563


2. Walker J.F., Reiner J.C. and Solenthaler C., Focused ion  beam sample preparation for TEM, Inst. Phys. Conf. Ser. 146, 629(1995).


3. Leslie A.J., K.L. Pey, K.S. Sim, M.T.F. Beh and G.P. Goh, TEM sample preparation using FIB: practical problems  and artifacts, Proc. ISTFA’95, p353-362.


4. T.Ishitani, H.Koike, T.Yaguchi, and T.Kamino, Implanted  gallium-ion concentrations of focused-ion-beam prepared  cross sections, J. Vac. Sci. Technol., B16, 1907(1998).


5. N. I. Kato, Y. Kohno, and H. Saka, Side-wall damage in a  transmission electron microscopy specimen of crystalline  Si prepared by focused ion beam etching, J. Vac. Sci. Technol., A 17(4), 1999, p1201-1204.


6. R.M.Langford, A.L.Petford-Long, preparation of TEM  cross-section specimens using FIB milling, J. Vac. Sci. Technol., A19(5), 2001, p2186-2193.


7. R.J.Young, P.D. Carleson, X. Da, T. Hunt and J.F. Walker, High-yield and high-throughput TEM sample preparation  using focused ion beam automation, Proc. ISTFA’98,p329


8. J.P.McCaffrey, M.W. Phaneuf, L.L. Madsen, Surface  damage formation during ion-beam thinning of samples for  transmission electron microscopy, Ultramicroscopy 87 (2001) 97-104


Advanced Fringe Analysis Techniques in Circuit Edit


RK Jain, T Malik, TR Lundquist, C-C Tsao


Credence Systems Corp, Sunnyvale, CA, U.S.A.


WJ Walecki


Frontier Semiconductor, San Jose, CA, U.S.A


Novel Fabry Perot [1] fringe analysis techniques for  monitoring the etching process with a coaxial photon-ion  column [2] in the Credence OptiFIB are reported. Presently  the primary application of these techniques in circuit edit is in  trenching either from the front side or from the backside of a  device.  Optical fringes are observed in reflection geometry  through the imaging system when the trench floor is thin and  semi-transparent.  The observed fringes result from optical  interference in the etalon formed between the trench floor (Si  in the case of backside trenching) and the circuitry layer  beyond the trench floor.  In-situ real-time thickness  measurements and slope correction techniques are proposed  that improve endpoint detection and control planarity of the  trench floor.  For successful through silicon edits, reliable  endpoint detection and co-planarity of a local trench is  important. Reliable endpoint detection prevents milling  through bulk silicon and damaging active circuitry.  Uneven  trench floor thickness results in premature endpoint detection  with sufficient thickness remaining in only part of the trench  area.  Good co-planarity of the trench floor also minimizes  variability in the aspect ratios of the edit holes, hence  increasing success rates in circuit edit.


Bulk silicon removal and endpoint detection


Through silicon circuit edit on a device begins with globally  thinning silicon to approximately 100µm.  The global thinning  is followed by local bulk silicon removal or trenching in up to  300x300 µm area using a 20nA beam current at 30keV beam  energy.  The current technique reduces the trench etch rate by  reducing the beam current and beam energy from (20nA, 30keV) to (4nA, 15keV).  The beam energy and current is  dropped once the fringe contrast on the optical image  increases [3].  The timing of this decision is subjective in  nature and depends on the user’s experience level.  For  instance a new user tends to drop the beam current and beam  energy at a higher remaining thickness of silicon compared to  an experienced user. Due to the qualitative nature of this  decision either the user can risk breaking through silicon and  damaging the circuitry or the user can slow down the  trenching speed, hence increasing the trenching time  significantly.  Furthermore, trench endpoint detection depends  on the ability to detect voltage contrast (VC) on n-wells [3];


voltage contrast quality is related to user experience, system  performance (good beam calibrations, beam energy and SE  detector quality), die dopant levels and n-well size and  density• (Fig. 1). A more robust endpoint detection technique  for trenching is necessary to overcome these dependences.  Therefore to address all the issues mentioned so far a  quantitative approach of in-situ remaining silicon thickness  measurement is required. Absolute remaining thickness of  silicon can be measured by using the optical beam of the  OptiFIB system.  Two in-situ thickness measurement  techniques are discussed. The first technique for the thick  sample regime measures the amplitude of the interference  fringes as a function of time at a certain region and is  discussed in detail in the section titled, “Absolute thickness  measurement based on fringe contrast variation”.   The second  technique for the thin sample regime uses two light sources  having wavelengths λ1 and λ2 and the observed shift between  their fringes which is discussed in detail in the section titled, “Absolute thickness measurement based on dual-wavelength  technique”.


Figure 1:  High density n-well image with excellent beam  current calibration and yet n-wells are difficult to see.


• Detecting n-well contrast presumes a p-substrate.  For an nsubstrate, p-wells would be detected.


## Advanced Fringe Analysis Techniques in Circuit Edit


79


Co-planarity


Even though corrections can be accomplished quickly, this  technique has limitations—control is ineffective when in the  chemistry depletion range (dwell time > 2µs).   Also, for Si  thicknesses > 30 µm, fringes can have non-linear patterns that  are hard to correct using this first order technique (Fig. 4).  However, dual chemistry injectors enables this linear  technique to be used for Si thicknesses > 50 µm. More, uniform gas flux delivery is another technique to improve the  planarity of the trench.  However, the SE collection efficiency  decreases due to direct interference in the SE collection path. Therefore, relying on VC endpoint becomes extremely risky.  Furthermore, with no optical information it is assumed that the  starting surface of the Si is perfectly planar.  Any initial nonco-planarity remains constant when a uniform gas delivery  system is used without any slope correction technique.


Co-planarity and flatness control are also crucial to circuit edit  efficiency and success. For instance during through silicon  circuit edit, if the remaining thickness of the trench floor  varies from 3 µm to 0.5 µm the aspect ratio of a 0.5x0.5 µm  hole can change quite significantly (Fig. 2).   For example for  the figure below if the inter-layer-dielectric thickness between  the active layer and metal 1 is 1 µm then the aspect ration can  vary for 3 to 8.  Higher aspect ratio holes lower the probability  of success and increase the time for an edit.


Edit Holes


N -well


contacts


n - diff  p - diff


Metal 1


0.5µm


3.0µm


Bulk Silicon


Figure 2:  The two edit holes show a significant difference in  aspect ratio because the resulting trench floor was not etched  co-planar with the interconnects.


For correction of trench floor co-planarity to the Si-SiO2  surface, the user infers slope in the trench floor using fringe  information in the optical image and then applies some  technique to correct that slope.  One correction technique is to  rotate the sample in 90o increments [4]. The physical rotations  of the part take care of the chemistry starved areas in the  trench. This technique is time consuming due to physically  rotating the device and it can only correct linear slopes. A  second technique is to increase or decrease the dwell time of  the beam in either X or Y axis (Fig. 3) [5].


Figure 4: Optical micrograph image of a non-linear sloped  trench floor.  Co-planarity is not corrected by a simple linear  variation of the ion beam dwell times.


During front side operations the user has the capability of  using near ultra violet filters in the OptiFIB system to see  through thick polyamide, silicon nitride or silicon-dioxide. With front side edits of copper devices co-planarity of  dielectric etch for a Cu plane line is extremely important.  For  process technologies < 0.13µm, low-k material and thinner  dielectric layers the significance of a planar etch process is  higher. Non-planar etching risks the exposure of unwanted  lower metal layers in the device and subsequent inadvertent  shorting (Fig 5).


Fringe direction


Siliton Bubatrete


--


Eliton


:88


8ub6


lon::


Figure 3:  Linear slope problem: When the trench floor coplanarity is near linear as in the top micrograph, a linear  change in dwell times can be applied to correct the slope.  Fringe flow direction reveals thin and thick regions of the  trench floor—fringes flow from the thinnest silicon to the  thickest.


Tawell time Inerease


Gas  Interforence crentes fringeaGas


Unlike aluminum it is very hard to volatilize copper and thus  prevent it from re-depositing.  Current Cu gases assisted etch  techniques in a FIB system rely on removing Cu while  protecting the underlying dielectrics [6].  The technique  becomes tougher when the underlying dielectrics become  thinner.  Therefore, dielectric etch planarity becomes more  significant with decreasing Cu geometries.  The optical image  taken in the OptiFIB system, using a 500 nm λ filter is able to  identify subtle slopes with  + 70 nm accuracy (Fig.6).


Figure 5. Uneven Cu etch exposes lower metal levels and  leads to inadvertent shorting.


Figure 6: Live optical image (λ=500nm) of a 10x10µm  window milled through 15µm thick passivation on the front  side of a Cu IC.  The fringes move from the (a) lower right  hand corner (b) to upper left hand corner. This fringe pattern


indicates a diagonal slope in the 10x10µm of passivation  being removed.


System


To calculate the topography of remaining Si in the trench floor  we have analyzed fringe patterns from a sequence of frames  recorded with a CCD camera.  The remaining thin Si film was  illuminated by a low coherence light beam emanating from a  lamp and filtered by a band pass filter. A simplified system  outline is illustrated in Figure 7.  Light emitted from the  illumination source (LS) is filtered (F) before filling the pupil  of microscope objective (O). The objective is adjusted to  focus at the trench floor for the optimum visibility of the  fringes.  The trench floor can be simulated as a two layer  system consisting of remaining Si as the top layer and the  second layer is the circuitry underneath the Si.  Reflected  beams from the two interfaces are collected and focused by  the same objective lens, which images on to the CCD sensor  plane.  A beam splitter (BS) is used to separate incident  illumination from reflected imaging beams.  The two layer  structure on the trench floor forms a classical Fabry-Perot  interferometer.  The pixel intensity recorded by CCD is the  result of interference of the two reflected beams with the path  difference defined by the remaining Si thickness.


LS


BS


CCD


DUT


Fringe


Figure 7. Experimental Setup


Thickness variation measurements using single  wavelength measurements


Fringe Formation


A model of a two-layer structure is presented in Figure 8.  It  comprises exposed crystalline silicon of thickness d residing  on supporting substrate of other material. Beams of incident  and reflected radiations of wavelength λ are perpendicular to  top surface of the material.  n1, n2, and n3 are complex and  generally wavelength dependent refractive indices of ambient, silicon, and support material respectively.


The complex amplitude of reflected radiation Er is related to  complex amplitude of incident radiation Ei by amplitude  reflection coefficient R: Er= R⋅ Ei.  For a simple two-layer


system the amplitude reflection coefficient R  is given by  Equation 1 [7].


ββ


,1


j j


−−


Signal (arb. units)


Crystalline Si


Ei


Er


n1


n2


|Support Material |n3 |
|---|---|

Figure 8: Geometry of model of the sample during  measurement


Where β is a term describing propagation inside the Si layer, and r12 and r23 are complex Fresnel coefficients describing  reflection from the interconnect layer and the Si-substrate  interfaces respectively.


λ


β


n ⋅


⋅


+−


It is clear because of β that the amplitude reflection coefficient  R depends both on wavelength and layer thickness, R = R (d,λ).


Our sample is probed with quasi-monochromatic light  characterized by central wavelength λc and spectral bandwidth ∆λ.  The illumination spectrum (defined by the optical filter  and the light source emission spectrum) together with the


Signal (arb.units)


responsivity of the  detector and optical transmission of the  optical components define the  system response function  W(λ).  The signal detected is therefore given by simple  integral:


∫


Signal


Since ∆λ is small (10nm in a typical case) we can neglect  dispersion of n1, n2, and n3 and assume in good approximation


that all wavelength dependence of signal [8] within ∆λ is due  to oscillatory term e-j2β in Equation 1.


Results of such simulation for bare silicon slab are presented  in Fig. 9, 10. Observed signal reveals strong Fabry-Perot  oscillations [9] when thickness becomes comparable or  smaller than the bandwidth determined coherence length. When film thickness becomes very small amplitude of the  oscillations saturates. Observed traces reveal a series of  fringes spaced by a distance corresponding to half the  wavelength propagating in the film, in our case fringes are  separated by approximately 125 nm as shown in Figure 10.


Film Thickness [um]


Figure 9: Reflected signal from sample shown in figure 8.  The following parameters were used forf simulation: λ = 900  nm; ∆λ = 7.1 nm in lower trace and 14 nm in upper trace, n1= 1, n2= 3.60- i0.0037 which are close to tabulated values [10], n3= 1. It assumes that the system response function W(λ) is perfect Gaussian centered at λc.


3.5


5.5


125 nm


Figure 10: Zoomed capture of lower trace shown in Figure 9.


5000


ϕ


(7)


ε


(8)


号


2000日


E


unif]Intensity [arb.8 1000口


00


100200300 Frame number


T


T+△T


Figure 11: Observed Fabry - Perot oscillations as a function  of etching time corresponding to one 9X9 µm pixel area on  array detector. Please note that frames collected by array are  numerated in this figure in the reverse chronological order. Excursion around frame number 164 has been caused by  intermittent hardware adjustment by operator.


Figure 12: Two consecutive frames collected at time T (left  panel) and time T+∆T revealing evolution of Fabry-Perot  interference pattern. Please note that fringes recorded at time  T+∆T are shifted with respect to fringes collected at earlier  time T.


To verify the simulation results we took a series of images  during the FIB trenching process and analyzed reflectance as a  function of time at a fixed pixel location.  The experimental  result is shown in Figure 12.  Since trenching rate and frame  rate are constant, the plot in Figure 11 is equivalent to those in  Figures 9 and 10.  The envelope of observed Fabry-Perot  oscillation has similar behavior graph simulated in Figure 10. The amplitude of oscillations saturates when thickness  becomes small.


Equation 6 describes a set of phase shifted images, where  phase shift between two consecutive frames is position  dependent function ∆ϕ(x,y). The task of fringe analysis is to  calculate ϕ(x,y) with the information from phase shift factor ∆ϕ(x,y).  To calculate the “wrapped” phase ϕw(x,y) we   developed our proprietary wrapped phase recovery algorithm  allowing us to recover wrapped phase with accuracy of about  5 % and speed comparable to algorithm commonly used in  phase shift optical interferometry [10].  Example of calculated  wrapped phase map is shown in panel (b) of Figure 13.


Fringe analysis


An array detector measured reflected light intensity as a  function of position on the sample, and we use collected  images to study position dependent thickness, and thickness  variation d = d(x,y).  In practice the array detector is collecting  series of signal images m =1, 2, 3…. at equal time intervals, where m numerates frames in the chronological order. Two  frames from such measurements are presented in Figure 12. During the etching process observed interference pattern is  evolving. The Fabry-Perot interference fringes evolved and  shifted in phase with respect one to another.


The amplitude of B(x,y) provides information about value of   the Fresnel coefficient r2,3 , which describes pattern residing  underneath Si film.  The amplitude B(x,y) is a quality map for  phase unwrapping algorithms, and example of such is  presented in panel (c) in Figure 13.  The quality map is a  cleaner image than the original optical image.  The cleaned  optical image will improve the box placement accuracy for the  ion beam using the optical image.  Utilizing the quality guided  unwrapping technique [11] it is possible to “un-wrap” phase ϕw(x,y) and to find unique function


( yx


unwrappedϕ


such


that:


If rate of etching


( yxε  is small (


()


<<


),


then fringe profile is approximated by:


i


unwrapped


(9)


cos


)    (6)


where i is a single integer constant, and does not depend on  spatial coordinates x, and y.


From Equation 9 we see that by performing unwrapping we  can determine thickness up to a constant additive multiple of  125 nm. This procedure is useful for determining thickness  variation of a measured layer, and for our purposes the  uniformity of the etch process.  An example of the recovered


where ϕ(x,y) is the phase factor related to thickness of Si and ∆ϕ(x,y) is the phase change as a result of etching.  A(x,y) and  B(x,y) are slowly varying functions of thickness d and can be  assumed constant.


layer thickness variation is presented in panels (d) and (e) in  figure 13.


Figure 13: An example of an interferogram analysis.. From  the initial data in form of set of image frames (a), the phase  wrapped image (b) and quality map (c) is extracted. Using  phase unwrapping algorithm thickness variation map (d) is  determined. Panel (e) represents the same data as presented   in panel (d) but displays it in 3D format. Please note that  noisy areas in top of the recovered map (e) corresponds to  areas of low quality fringes as shown in panel (b), and dark, devoid of signal areas of original data as shown in panel (a).


Error analysis and limitations of the method


The main source of the measurement error of the thickness  variation is the systematic error due to the unknown value of  the Fresnel coefficient r2,3 describing reflection from the  Sisubstrate interface.  In real samples the substrate layer may  comprise metals, dielectrics and multilayer structures. In the  extreme case, change of complex refractive index n3 may  affect phase of the observed oscillations by less thanπ


(which corresponds to maximum error of thickness variation  of silicon < 70 nm), and it does not affect spacing between  individual fringes.


(c) Cleaned Optical Image


(b) Phase


(a) Optical Image


Other sources of systematic errors may include errors of  determination of spectrum, and central wavelength of  impinging radiation. These contribute less than 1 nm to error  of determination of silicon thickness, and can be neglected.


We estimate the error of wrapped phase value determination  to correspond to the error of Si thickness of about +/- 6 nm.  This can be neglected with comparison to the systematic error  discussed above.


In general, in the thin sample thickness regime when fringes  have visibility > +/- 10% we estimate accuracy of this method  to be better than +/- 50 nm. Fringe visibility is directly  proportional to the contrast of the image.  As the sample gets


计


thinner the contrast increases.


年


Absolute thickness measurement  Fringe contrast variation


If the Fresnel coefficient r2,3 is approximately real in limit  Re(r2,3) >> Im(r2,3) and r2,3 > 0 than the envelope of observed  oscillation as function of silicon thickness d saturates in limit  of the thin film thickness and can be approximated by few  terms of its series expansion:


K


(10)


Taking derivatives of both sides and normalizing amplitude  the thickness is:


d S


const


∆∆


(11)


Normalization with respect to amplitude S eliminates variation  due to changes in optical alignment and to changes of r2,3  across the sample.


(e) Topography


(d) 2D  thickness


This method is used for rough estimate of Si layer thickness. The incremental change of sample thickness ∆d in the  denominator of Equation 11 can be determined with good  accuracy by counting Fabry-Perot oscillations.   The main  source of error is amplitude of the oscillation measurement. This technique requires fast collection of data.  Preliminary  results indicate that accuracy of this method is about +2µm.


Dual-wavelength technique


In order for better accuracy in endpoint detection of the FIB  trenching process we also investigated Si thickness  measurement using a two-wavelength technique. The  reflection coefficient depends only on ratio of Si film  thickness and probing wavelength.


( )λ


(12)


Equation 12 suggests that fringes measured at two close but  different, wavelengths λ1 and λ2 are shifted in phase one with  respect to the other.  For sufficiently thin slabs of Si, phase  shift between observed fringe patterns is proportional to  thickness of measured Si. By measuring phase change  between the two wavelengths Si film thickness is then known.  The physical insight is illustrated in Figure 14.


λ1


λ2


T1


T2 T3


Quality map B(x,y) will provide a cleaned image.  The  cleaned optical image will improve the box placement  accuracy for the ion beam using the optical image.


To improve circuit edit success rate and efficiency for through  silicon edit successful endpoint detection and planarity of etch  during bulk silicon removal is very important.  We have  proposed using Fabry-Perot fringe analysis techniques to  monitor and control the etch process with a coaxial photon-ion  column in the Credence OptiFIB.  The technique will be first  of its kind to provide an in-situ quantitative control technique  during FIB etching,.  With decreasing interlevel dielectric  thickness this tool will be useful for maintaining planarity  during front side edits. Si layer thickness variation across the  field results in various degrees of phase difference between  the two beams and therefore generates fringe pattern on the  2D display.


Figure 14: Intuitive explanation of two wavelength method. Crest of Fabry Perot fringes are observed when the optical  thickness of slab is a multiple of half wavelength of probing  radiation, which corresponds to a standing wave condition.    Note that nodes occur for each wavelength at slightly different  thicknesses. Phase shift of observed fringes at λ1 and λ2 is  proportional to thickness of the slab as long as phase shift is  smaller than 2π.


We would like to acknowledge help from Mr. Alexander  Pravdivstev from Frontier Semiconductor, who developed the  software package for graphics file format conversion.


[1] Hernandez, G. Fabry-Pérot Interferometers,  (1986), Cambridge: Cambridge University Press


Accuracy of measurement using the two-wavelength  technique is a fraction of a wavelength.  The drawback of this  technique is the so-called “thickness ambiguity” which limits  the upper limit of thickness measurement.  Thickness  ambiguity happens when the slope of the thickness variation  results in more than 2π phase shift.  For the case of λ1 = 990nm and λ2 = 1000nm that the accuracy is about 0.6µm and  thickness upper limit to avoid thickness ambiguity is about  14µm.


[2] C-C Tsao, P. Sudraud, P. Bouchet, and M. Thompson, LSITS, 2001


[3] C. Boit, K. Wirth, and E. Le Roy, ISTFA 2003, pp 331-337


[4] M.A. Thompson et al., ISTFA 2002, pp 409-417


[5] R.K. Jain et al., ISTFA 2005, pp 70-77


[6] V.V. Makarov, W.T. Thompson, T.R. Lundquist, M. Thompson and T.T. Miau, 3rd AVS International  Conference on Microelectronics and Interfaces February  2002, pp 115-117


[7] R. M. A Azzam, N. M. Bashray, “Ellipsometry and  Polarized Light, North-Holland, Amsterdam, ISBN 0-444-87016-4 (1987)


For the purposes of this discussion a flip chip device globally  thinned to 50 um will be considered.  The local trenching will  utilize absolute thickness measurement based on fringe  contrast variation using equation 11.  The technique has an  error of + 2 µm. This technique will be used until 10 µm  remaining Si thickness.  The dual-wavelength technique will  then be used to thin down the Si further with accuracies up to


+ 0.1 µm. Fringe based techniques combined with the existing  techniques will decrease etch time and improve chances of  accurate endpoint detection.    Relative thickness measurement  illustrated in Figure 13 can be utilized consistently by the FIB  to vary ion beam dwell time and to control flatness inside the  trench.


[8] Tabulated


values


were


found


on  http://ee.byu.edu/photonics/optical constants.phtml last  viewed on 6/21/2006 and are based on Edward D. Palik “Handbook of optical constants of solids”


[9] G. R. Fowles “Introduction to modern optics”, Dover (New York 1989)


[10]  J.E. Greivenkamp, and J. H.Bruning, “Phase Shifting  Interferometers,” in Optical Shop Testing, D. Malacara, Ed., Wiley, New York, 1992, pp, 501-598.


[11]  J. C. Wyant and K. Creath “Recent advances in  interferometric optical testing”, Laser Focus/Electro – Optics vol. 21, pp 118-132 (1985).


[12] D. J. Bone Applied Optics vol 30, pp. 3621- 3632, (1991).


Direct Measurements of Charge in Floating Gate Transistor Channels of Flash  Memories Using Scanning Capacitance Microscopy


Christophe De Nardi, Romain Desplats, Philippe Perdu


CNES, French Space Agency, DCT/AQ/LE, Toulouse, France


Christophe.Denardi@stage.cnes.fr


Christophe Guérin


DGA/CELAR, French Defense Department, Bruz, France


Jean Luc Gauffier, Thomas B. Amundsen


LNMO, INSA Génie Physique, Toulouse, France


Failure Analysis has to deal with challenging questions about  stored charges in floating gates in Non Volatile Memories (NVM) when reading does not give expected data. Access to  this information will help to understand failure mechanisms. A  method to measure on-site programmed charges in Flash  EEPROM devices is presented. Scanning Capacitance  Microscopy (SCM) is used to directly probe the carrier  concentration on Floating Gate Transistor (FGT) channels. The methodology permits mapping channels and active  regions from the die backside. Transistor charged values (ON/OFF) are measured and localized with a 15 nm  resolution. Both preparation and probing methods are  discussed. Applications are demonstrated on two different  Flash technologies: a two-transistor cell (2T-cell) from Atmel  and a one-transistor cell (1T-cell) from STMicroelectronics.


The reliability and retention of data stored in Non Volatile  Memory (NVM) are key issues for manufacturers of  microelectronics devices. In addition, whatever the kind of  applications – general public, space or military – the  confidentiality of data is a question of utmost importance.


In the case of EEPROM (Electrically Erasable Programmable  Read Only Memory) or Flash-EEPROM, data are related to  the presence or absence of a certain charge level (electrons) on  isolated gates (Floating Gates FGs). Depending on this charge  level, the memory cell is blocked or conductive. In order to  investigate the reliability of the stored data (e.g. after stress  test for space or military qualifications) it is necessary to be  able to measure (or read) these stored charges. Their density  must be directly probed on site, using physical measurements  to avoid software protection against unwanted access. Electrical techniques of AFM, with their high spatial  resolution (0.1nm for AFM, 15 nm for SCM, 40nm for  SKPM) and their high sensitivity to carriers, may achieve such  measurements to determine the logic value of each memory  bit.


In order to relate the AFM measurements with the logic  programming of the memory, data must be reconstructed as  bytes (8 bits) or words (K bits). For space and military  applications, the memory mapping is not provided. Therefore, to understand how information are stored, the whole memory  table organization must be deduced, i.e. the physical location  of each electronic address. This is the role of descrambling.


As we present in this paper, the descrambling step comes first. It is then followed by the IC deprocessing. The challenge is to  prepare the device with such finesse that the charges are not  removed (e.g. by chemical attack) and that the finishing  surface quality is compatible with the AFM electrical modes.  Of course, this step must be done at the precise location of the  memory bits under investigation.


The reading step will be performed by SCM. The Scanning  Kelvin Probe Microscopy (SKPM) approach for EEPROM [1] did not yield conclusive results for the Flash memories under  test selected for this paper. This limitation can be explained by  i) lower carrier sensitivity of the SKPM approach because it is  dependent on the gate oxide layer thickness and there is not  remaining substrate on the chips to assure a good polarization  of samples ii) lower electron concentration stored on Flash  FGs compared to EEPROM FGs. Indeed, the recent  technologies store fewer and fewer electrons, down to fewer  than 1000 electrons for 90nm-node NAND Flash [2]. The idea  of the SCM approach is to probe directly the carrier density in  Floating Gate Transistor (FGT) channels, which is the mirror  charge of the one stored onto FGs. Under these conditions, the  tip is directly in contact with the channel charge location and  the gate oxide layer does not screen the measurements. A map  of the channel capacity dC/dV(x,y) of each memory cell is  obtained which permits localizing blocked/conductive Flash  cells.


Because of the mobile nature of programmed charges


resolution (≈0.1nm for AFM, ≈15 nm for SCM, ≈40nm for


(electrons on FGs or holes on channels), special care must be  taken to maintain their integrity during the whole process. Preparation and reading have to be data non-destructive, which  is the main issue of the presented work.


## Direct Measurements of Charge in Floating Gate Transistor Channels of Flash Memories Using Scanning Capacitance Microscopy


86


A standard Scanning Probe Microscope (D3100 Veeco  Instruments) is used. The reader is referred to [3, 4, 5, 6] for  details about SCM principle and to [6, 7] for SKPM technique.


Devices Under Test


For this study, we have selected two Flash memories based on  different technologies at cell level.


The first NVM memory is a 1Mbit NOR Flash from Atmel  with 5V power supply [8]. Its cell (Figure 1) is composed of  two NMOS transistors: an Access Transistor (AT) and a  Floating Gate Transistor (FGT). This FGT is a FLOTOX type  one: it has two gates, a control gate (poly 2 CL) and a floating  gate (poly 1 FG) totally isolated from the structure, and has a  local thinning of its gate oxide at its drain side. This area is  called the Fowler Nordheim tunneling region. This twotransistor Flash cell from Atmel is physically very similar to an  EEPROM cell [9, 10], but the device works as a Flash one: the  program operation is byte selective, the erase operation is  sector (128 bytes) mode and the endurance is 104 cycles.


CNES DCT/AO LE


CNES DCT/AO/LE


Figure 1: 2T-Flash cell SEM cross-section parallel to bitline  BL. (Above) Cell general structure. (Below) Zoom on the


MIgQ0200nm


FLOTOX FGT. The gate oxide and tunnel oxide are  respectively measured 40nm and 8nm.


In such 2T-cell devices from Atmel, the data correspond to the  charge density accumulated in the floating gate (FG)/tunnel


oxide interface. The following conventions are used (see  Acknowledgments):


● An erase operation consists in injecting electrons onto  FGs whereas a program operation consists in extracting  electrons from FGs. Both operations are performed by  Fowler Nordheim tunneling.


An erased cell has between 103 and 105 electrons stored  onto its FG and presents a positive threshold voltage VT1 (≈ +2V) while a programmed cell has no electrons in its  FG and presents a negative threshold voltage VT2 (≈ -2V).  When a read voltage between VT1 and VT2 is applied to  the CL, the erased cell remains OFF which corresponds to  the “1” logic state, whereas the programmed cell is  conductive (“0” state).


The second NVM memory is a 4Mbit NOR Flash from ST  Microelectronics with 3V power supply [11]. Its cell (Figure  2) is composed of a single NMOS transistor: a FGT with two  gates, a control gate (poly 2 CL) and a floating gate (poly 1  FG).  This FGT is an ETOX type because it does not have a  preferential thinning location of its gate oxide. Its thickness is  uniform and measured around 8 nm. In such Flash devices, the  program operation is byte selective, the erase operation is  sector (64 Kbytes) mode and the endurance is 105 cycles.


腔zpm


SEU


CNES DCT/AO>LE


CNESOCT/ROLE


Figure 2: 1T-Flash cell SEM cross-section parallel to bitline  BL. (Above) Cell general structure. (Below) Zoom on the  ETOX FGT. Local thinning of the gate oxide is not present. The gate oxide thickness is uniform around 8nm.


2T-cell


Metal 2 WL


Metal 1 BL


AT


FGT


Source Line


Drain contact (W plug)


Zpm


SKU


Poly 2 CL  ONO


Poly 1 FG


Gate oxide


(≈40nm) 500nm


G1:0 Tunnel oxide


(≈8nm)


Source   Line


FGT  drain


Silicide CL


Uniform gate oxide


Source


Spacer


1T-cell


Cell drain


In such 1T-cell devices from STMicroelectronics, the data  correspond to the charge density accumulated in the floating  gate (FG)/gate oxide interface. The following conventions [12] are used (see Acknowledgements):


A program operation consists in injecting electrons onto  FGs by Channel Hot Electrons Injection. An erase  operation consists in extracting electrons from FGs by  Fowler Nordheim tunneling.


A programmed cell has between 103 and 105 electrons  stored onto its FG and presents a highly positive threshold  voltage VT1 (> +6V), while an erased cell has no electrons  in its FG and presents a slightly positive threshold voltage  VT2 (≈ +1V).


When a read voltage between VT1 and VT2 is applied to  the CL, the programmed cell remains OFF which  corresponds to the “0” logic state, whereas the erased cell  is conductive (“1” state).


It is important to underline that the conventions used by Atmel  for its 2T-cell memory are reversed compared to the ones used  by STMicroelectronics for its 1T-cell memory, which can lead  to confusion [13].


Electrical Descrambling


AFM based techniques are meant to be used on small areas  since the maximum scan size is 100µm by 100µm due to  limited piezoelectric scanner x-y displacements. Therefore, the  area of interest must be located precisely beforehand to match  the electrical address with its physical location.


Because of the sector-erase mode of Flash memories, we have  chosen a combination of Electron Beam Testing (EBT) and  Focused Ion Beam (FIB) cut techniques to perform the  descrambling. Indeed, non-destructive techniques (as EBT or  EMMI) are not sufficient to deduce the entire mapping of the  memory because of this impossibility to erase only one byte at  a time [14].


The descrambling is achieved on a different chip from the one  on which the reading is performed. The first step (Figure 3) consists in localizing all the word lines (metal 2 WL) by EBT, putting the memory in error mode. By trying to write the data “FFh” to a specific address initially at “00h” without doing a  sector erase operation, the WL of this address becomes visible. By looping this exercise, addressing a single WL each time, the addresses of all WLs are deduced. The second step (Figure  4) consists in trying to get the perpendicular information, i.e. to understand in which order the bits are stored along the same  WL. By cutting by FIB a single bit line (metal 1 BL), the  electronic address of the bit cut is deduced. By this  combination of EBT and FIB the whole organization of the  electronic addresses in the Flash table is determined (Figure 5  and Figure 6).


In both Atmel and STMicroelectronics memories, the results  show that there is a scrambling at bit level, i.e. bits constituting


the same address are stored far away from each other. Actually, each bit of the same weight but from successive  addresses are grouped together in blocks (Figure 5). Thus, to  read a “real” byte, it is necessary to probe their 8 bits located


●A program operation consists in injecting electrons onto


in 8 different blocks. Under these conditions, 8 bits which are  physical neighbors will constitute a “virtual” (scrambled) data. Thanks to the descrambling results, we can easily pass from “virtual” to “real” data and vice versa.


Figure 3: Principle of descrambling of WLs using EBT. The  figure shows the WL addressing of sector 2 which contains  addresses from 6000h to 7FFFh. The word 7D00h is  programmed in error mode in loop. Its WL, which accesses  addresses from 7D00h to 7DFFh, is localized by potential  contrast (1T-cell Flash memory).


●O00O0-


Unfortunately, it is quite difficult to enlarge the usable region (i.e. the 60µm large region with the appropriate silicon  thickness) during the sample preparation. Another idea was to  move it using a step by step approach. Each step consists in a  quick choline hydroxide etch followed by a SCM reading of  the obtained region. Doing that, a lot of areas of the Flash  table can be read by SCM. For example, Figure 10 shows  addresses initially programmed at “F0h” which are physically  located around 200µm far away from the previous ones (which  were programmed at “12h”). Figure 10 demonstrates again that  sample preparation is data non-destructive.


1:Height


200μm0.0


2:dCjdV Phase


20.0 μm


Figure 10: Contact AFM and Phase SCM on addresses  initially programmed at “F0h”=”11110000” from right to  left. This usable area was obtained after a successive chemical  etch.


Data Reading On 1T-Cell Flash Memory


Before preparation, a few addresses of the Flash table from  STMicroelectronics are programmed in order to have “AAh”= “10101010” virtual data (8 neighboring bits). Thanks to  descrambling, their physical locations are known and can be  scanned by AFM based techniques. Only the four most  significant bits are visible on Figures 11. The bit of weight “7” is on the left side of theses images.


Figure 11-1 shows the topography of the channel layer  obtained from the die backside of the 1T-cell device after  SCM preparation. Field oxides rise just 100nm above the  silicon surface. On a region totally free of silicon (not shown) the field oxide is measured to be 200nm taller than the  exposed tunnel oxide layer. Thus, the remaining silicon  thickness in the region of interest is deduced to be around  100nm.


The capacitance sensor is tuned in order to be sensitive only to  information coming from FGT P-channels (Figure 11-2). This  is done by applying a small AC voltage to the tip (0.5V) and a


DasZoon


500.0nm


DataZoon


360.0°


negative DC part (-0.4V). Under these conditions, the  amplitude SCM probing is preferentially sensitive to P-doped  areas. Thus, the signals coming from highly doped N-regions (A, C) are nearly null as the ones in thick field oxide (D). Changing the DC voltage to a small positive value (+0.1V), N  source/drain areas are preferentially detected and overlap the  interesting information coming from FGT channels.


As it was explained before, a FGT transistor in a blocked state (“0” for STMicroelectronics conventions) has a high density of  holes in its open (OFF) channel. Thus, the amplitude SCM  signal coming from its channel is strong and its corresponding  Phase is P-type (yellow in white circles).


Conversely, a FGT transistor in a conductive state (“1” for  STMicroelectronics conventions) has a depleted channel. Indeed, because of its slightly positive threshold voltage (VT≈+1V) and the probing conditions (DC=-0.4V and  AC=0.5V applied to the tip), the inversion layer is not reached. As a consequence, SCM signals coming from its channel are  very low, even null (in black circles). This conductive channel  is an undefined doped area: neither electrons nor holes are  detected (depletion layer). The Amplitude SCM difference  between a blocked channel and a conductive one is measured  around 100mV with only 0.5V AC and -0.4V DC voltages  applied to the tip. With the same voltage tip conditions, the  Phase SCM difference is around 80° (Figure 12).


FanData Zcom


300.0 hm


Data Zoon


500.0mVMetbreFDaaZscm


5.0nmMeeors


DataZoom


1:Helight


50μm0.0


2:dC/dVAmp


5.0 μm0.0


3:Deflection


2:dCdVPhase


5.0 μm


Figure 11: Contact AFM (Figure 11-1), Amplitude SCM (Figure 11-2) cantilever deflection (Figure 11-3) and Phase SCM (Figure  11-4) scans on active region levels prepared from the backside of 1T-cell Flash memory from STMicroelectronics. The blocked FGT  channels (“0” for STMicroelectronics conventions) are in white circles and the conductive ones (“1” for STMicroelectronics  conventions) in black circles. The data are measured as “1010” (from left to right) as the four most significant bits were initially  programmed. (A) Cell drain, (C) cell source, (D) field oxide, (J) FGT channel.


A J C


J


+ -


N  P


0  0  0  0   1   1  1  1


1       0        1      0


Figure 12: Relative Phase SCM measurements between a  blocked FGT channel (rich in holes) and a conductive one (depleted). The difference is measured around 80° as shown. In the blocked transistor, PN junctions between the P channel  and its surrounding N active regions are clearly detected. This  proves that its channel is open and its threshold voltage is  highly positive (>6V). In the depleted transistor, the phase  signal coming from is channel is undetermined. This proves  that the inversion layer is not totally reached (depletion mode) and thus the threshold voltage is slightly positive (≈1V).


On 1T-cell technology, our approach of successive chemical  etches to move the useful area is also validated. Indeed Figure  13 shows SCM reading of addresses programmed to “12h” which are located on different areas from the previous ones (programmed to “AAh”).


Figure 13: Contact AFM and Phase SCM on addresses  initially programmed at “12h”=”00010010”. Only the 4 main  significant bits are shown from right to left. This usable area  was obtained after a second chemical etch.


Discussion and Comparison


The SCM approach presented in this work was successful on  both 2T-cell and 1T-cell Flash technologies, but also on  various EEPROM devices we investigated. Indeed, we tried  this methodology on a lot of NVM devices based on floating  gate technology, from EEPROM types (not shown in this  paper) to Flash-EEPROM. In general, EEPROM is an easier  case because of higher charge level stored, larger floating  gates and channels. Up to now, in all the devices we have  tested, NVM data initially programmed were successfully  detected by SCM.


Both sample preparation and SCM reading appear to be data  non-destructive and repeatable on the 2T-cell and 1T-cell  Flash memories:


Keeping DC and AC voltages applied to the tip under a  low range, respectively [-1V, +1V] and [+0.25V, +3V], far away from high voltage levels [+8V, +20V] used to  program/erase Flash devices, the same area can be  scanned (read) multiple times by SCM. For example, we  scanned the same area in a continuous way during 4 hours (i.e. ≈ 12 successive scans of 20min each) without  significant loss in the level detection, proving that SCM  reading does not alter Flash data.


After preparation at active region layer, retention  capabilities of Flash devices are weakened. Thus, the  devices must be stored in a dark box to protect them from  light irradiations, thus avoiding a loss in programmed  charge level. After the first initial silicon oxidation (one  day in air), they are stored in a N2 (or vacuum) atmosphere to reduce evolution of the silicon backside  surface. Using these storage conditions, SCM probing of  areas (previously scanned or not) is achievable during a  long time after backside deprocessing. For example, we  tried to probe data on Flash devices which were prepared  two months before: the data were still present and  successfully detected.


Using a step by step chemical approach, the usable area  with the appropriate thickness is movable. The obtained  new area can be read by SCM and has the same  characteristics as the previous one, i.e data retention under  continuous SCM scans or under dark N2 storage  conditions. This demonstrates that the sample preparation  is also data non-destructive and repeatable.


This SCM approach presents three main advantages compared  to the SKPM methodology we have developed in [1]:


Higher carrier sensitivity, up to a single electron [6], thanks to the capacitance resonator.


Non dependent on the tunnel oxide thickness. Indeed, the  SCM measurements are not screened by the tunnel oxide  layer as SKPM ones are.


The conservation of a small silicon thickness on the  device backside. This leads to a higher electric conduction  and a flatter topography of the sample.


This approach is very promising for future Flash memories  which store less and less charge onto their FGs: down to 1000  electrons for 90nm-node NAND Flash device [2].


The main drawback of this approach is that the required  preparation (50-300nm remaining silicon on the chip backside) is quite impossible to achieve on the entire Flash array in a  single chemical etch (as SKPM does). Nevertheless, the usable  region is movable by successive chemical attacks. Thus, SCM  probing is achievable on different regions of the table memory.


1       0      0      0


1       0       1       0


With the goal of measuring on-site-programmed charges in  Flash-EEPROM, we have presented a complete methodology  on two different commercial memories: a 2T-cell from Atmel  and a 1T-cell from STMicroelectronics used for data or code  storing applications. The presented work starts with the  deduction of the memory table organization (descrambling). Then follows the sample preparation based on the backside  approach of the chip. The SCM technique permits probing  directly carrier density in the floating gate transistor channel of  each memory cell, thus making it possible to determine the  logic value of each bit (ON/OFF or 1/0). Both preparation and  probing techniques appear to be data non-destructive and  repeatable. Results show the quality and reliability of our  methodology: Flash data are not altered during the preparation  and are successfully measured (read).


AFM profiling has been previously shown by K. Upadhyaya et  al. [15] onto different layers of Intel Flash devices obtained  after backside deprocessing with choline hydroxide. Nevertheless, in the present paper, the first SCM application is  demonstrated from a die backside. This approach appears to be  highly carrier sensitive and promising for future Flash  technologies.


The author would like to thank Mr. Gilles Festes [9] from  Atmel and Mr. Bruno Leconte [12] from STMicroelectronics  for explaining the data conventions used by their respective  non volatile memory products. Unfortunately, these  conventions are opposite, which makes the task more complex.


[1] DeNardi, C. et al., “EEPROM Failure Analysis  Methodology: Can Programmed Charges Be Measured  Directly by Electrical Techniques of Scanning Probe  Microscopy?” Proc. 31st ISTFA, November 2005, pp. 256-261.


[2] Deleruyelle, D. et al., “Single-electron phenomena in  ultra-scaled floating gate devices and their impact on  electrical characteristics”, Proc. 1st International


Conference on Memory Technology and Design (ICMTD), May 2005, pp. 25-27.


[3] Veeco Metrology Group, “Application Modules: Dimension and Multimode Manual. Software Version


5.12r4. Revision B.”, 20 May 2003.


[4] Y. Takasaki, T.Yamamoto “Cross-section analysis of  electric devices by scanning capacitance microscope”, Proc. 10th ESREF, October 1999, pp. 987-990.


[5] A. Born and R. Wiesendanger, “Guidelines for TwoDimension Dopant Profiling using SCM”, Proc 26th  ISTFA, November 2000, pp. 521-527.


[6] Erickson, A.N., “The Role of the Atomic Force  Microscope in Failure and Yield Analysis”, Tutorial of the  27th ISTFA, November 2001.


[7] Doukkali, A. et al., ”Surface potential mapping of biased  pn junction with kelvin probe force microscopy: application to cross-section devices”, Applied Surface  Sciences, v 235, iss 4, August 2004, pp 507-512.


[8] Atmel, “AT29C010A data sheet. 1-Megabit (128Kx8) 5-volt Only Flash Memory”, (2005), Retrieved July 12, 2006, from http://www.atmel.com/dyn/resources/ prod_documents/doc0394.pdf


[9] Festes, G. et al., “ISSG RTO Grown Tunnel Oxide on  Advanced FLOTOX E2PROM Memories”, Proc. 1st  ICMTD, May 2005, pp. 215-218.


[10] B. Lojek, E. Daemen, and A. L. Renninger, “Ultra small  thin windows in floating gate transistors defined by lost  nitride spacers” U.S. Patent 6,624,027.


[11] STMicroelectronics “M29W400BB data sheet. 4Mbit (512x8 or 256x16, Boot Block) Low Voltage Single  Supply Flash Memory”, (June 2001), Retrieved July 12, 2006, from http://www.st.com/stonline/products/ literature/ds/6584/m29w400bb.pdf.


[12] S. Zink, C. Cavaleri and B. Leconte, “Page by page  programmable flash memory”, U.S. Patent 6,839,285  Brevet FR 2803080.


[13] Van Houdt, Jan, “Non Volatile Memory Reliability”, Tutorial of the 11th ESREF, October 2000.


[14] DeNardi, C. et al., “Descrambling techniques for  EEPROM and Flash memories: EMMI, EBT and FIB”, European FIB User Group (EFUG) meeting of the 16th  ESREF, October 2005.


[15] K.Upadhyaya and P.W.Blacker, “Backside Imaging and  AFM Profiling of Tunnel Oxide, Poly 1, ONO and Poly 2  Layers on Flash Devices”, Proc. 29th ISTFA, November  2003, pp. 447-451.


94


Δ


Material and doping contrast in semiconductor devices at nanoscale resolution  using scattering-type scanning near-field optical microscopy


J. Wittborn and R. Weiland


Infineon Technologies AG, 81739 Munich, Germany


D. Kazantsev*, A. Huber, and R. Hillenbrand


Nano-Photonics Group, Max-Planck-Institut für Biochemie, 82152 Martinsried, Germany


*Present address: Institute of Theoretical and Experimental Physics, B. Cheremushkinskaya 25, Moscow, 117218, Russia


F. Keilmann


Abteilung Molekulare Strukturbiologie, Max-Planck-Institut für Biochemie, 82152 Martinsried, Germany


The usefulness of scattering-type near-field optical microscopy  for mapping the material and doping in microelectronic devices at nanoscale resolution is demonstrated. Both amplitude and phase of infrared (λ = 10.7 μm) laser light scattered by a metallised, vibrating AFM tip scanned a few nanometers above the sample are detected and transformed into images showing contrast of materials, as well as of doping  concentration. Cross-sections through layers as thin as 20 nm(?/500) have been clearly imaged.


Background


To be able to distinguish the constituent materials as well as possible contaminants has long been an important issue in failure analysis of microelectronics. As devices continue to shrink new methods for material contrast imaging with sufficient resolution have to be developed.


Scanning electron microscopy (SEM), transmission electron microscopy (TEM) and scanning probe microscopy (SPM)provide nanoscale spatial resolution, but have only limited chemical sensitivity unless combined with other methods or instruments. Versions of SPM, such as scanning capacitance microscopy (SCM) [1,2,3,4] or scanning spreading resistance microscopy (SSRM) [5,6] give good doping contrast [7] but yield poor material contrast. Infrared spectroscopy, on the other hand, offers the required chemical sensitivity but its spatial resolution is limited to the micrometer scale due to diffraction. Scanning near-field infrared microscopy thus appears to be a logical step towards achieving chemical detection with nanoscale lateral resolution.


We have recently reported that scattering-type near-field optical microscopy (s-SNOM) operating at mid infrared[8,9,10] wavelengths, λ = 10.7 μm, can be applied for nanoscale resolved mapping of material and doping in crosssectional samples of microelectronic circuits [11].


The experimental set-up


Our experimental set-up basically consists of a home-built AFM combined with an infrared, laser light source and pseudo-heterodyne interferometric detection able to detect both amplitude and phase of the scattered light.


The AFM uses a Pt-coated Si tip which is oscillating at its mechanical resonance frequency Ω and is illuminated by focused infrared laser light of a tunable CO2-laser at ~30°incidence (see Fig. 1). Interferometrical detection of the backscattered light, combined with demodulation at higher harmonics of the tip oscillation, allows the recording of both amplitude and phase of the optical near-field interaction.


Figure 1: Schematic image of the experimental set-up.


Theory


The optical near-field scattering, depending on refractive index  and absorption of the sample, can be enhanced by phonon polaritons in polar dielectrics or plasmon polaritons in metals and doped semiconductors [12]. Using a wavelength near the polariton resonance of the material of interest thus causes sharp contrast between this and other materials.


## Material and doping contrast in semiconductor devices at nanoscale resolution using scattering- type scanning near-field optical microscopy


98


A dipole model for the field scattered by the tip that has proven to agree well with experimental results has been developed and is thoroughly described in a paper by Keilmann and Hillenbrand [13].


Experimental Results


Samples were prepared for imaging by cleaving and mechanical polishing to the cross-section of interest. No further sample preparation such as etching or metal-coating was necessary.


NPN-transistor


Figure 4: Principle of descrambling of BLs using FIB. By  cutting a BL (metal 1) without degrading metal 2 lines, all  values of bits accessed by this BL are modified. For example, cut n1 leads to data modification from FFh (=11111111) to  F7h (=11110111) of addresses 60FFh/61FFh/…./7FFFh. Thus, the physical location of BL of weight 3 for FFh  terminating addresses is determined (1T-cell Flash memory).


80X


WL addressing of sector 2


Cut n1 Cut n3 Cut n4 Cut n5 Cut n6


Cut n2 6000 to 60FF 7F00 to 7FFF


Details of the organization see Figure 6  WL addressing


of sector 2


7D00 to 7DFF


6000


to 60FF


7F00 to  7FFF


Figure 5: Global organization of the 1T-cell Flash memory  deduced by the combination of EBT and FIB descrambling  techniques. Bits of same weight are grouped in blocks. To  read a “real” data byte, we need to probe its 8 bits localized  in the 8 corresponding blocks. What is more, depending on if  the address is odd or even, these 8 bits are not localized in the  same location (1T-cell Flash memory).


|60FF 61FF 62FF 63FF 64FF 66FF 66FF|||67FF|
|---|---|---|---|

|60FD 61FD 62FD 63FD 64FD 65FD 66FD|||67FD|

|60FB 61FB 62FB 63FB 64FB 65FB 66FB|||67F8|

|60F9 61F9  62F9  63F9| 64F9| 66F 9 66F9|67F9|

|60F7 61F7  62F7  63F7| 64F7| 65F 7 66F7|67F7|

|60F5 61F5  62F5  63F5| 64F5| 65F 5 66F5|67F5|

|60F3 61F3  62F3  63F3| 64F3| 65F 3 66F3|67F3|

|60F1 61F1  63F1  63F1| 64F1| 65F 1 66F|1 67F1|

|60EF 61EF  62EF 63EF| 64EF| 65EF 66EF|67EF|

|60ED 61ED 62ED  63ED| 64ED| 65E D 66E|D 67ED|

|60EB 61EB 62EB  63EB 64EB||65EB  06EB| 67EB|

|60E961E9 62E9  63E964E9||65E9  66E9| 67E9|

|60E7 61E7  62E7  63E7| 64E7|65E7  66E7| 67E7|

|60E561E562E563E564E5||65E566E567E5||

|60E361E3  62E3 63E3 64E3||65E3 66E3 67E3||

|60E1 61E1 62E1 63E1 64E1||65E1 66E1 67E1||

Figure 6: Details of the organization of some bits of weight 3  for successive odd addresses. This table corresponds to the  region marked with a white rectangle in Figure 4. All bits in a  block of weight K are organized in the same way (1T-cell  Flash memory).


Programmed charges (electrons) in Flash Memories are stored  at the FG/gate oxide interface. This electron concentration  modifies the threshold voltage and the channel carrier  distribution of the FGT. By capacitance coupling through the  gate oxide, the hole density located in FGT channel is the  coupled image of the electron density stored onto its FG. The  SCM approach consists in probing this carrier (holes) density  located on FGT channels. The SKPM method which measures  FG potentials through gate oxide layers from the die backside


[1] did not yield conclusive results on the Flash devices  selected for this paper.


To make such SCM measurements, samples must be  deprocessed in a certain way that the AFM tip can scan close  enough (<300nm) the transistor channels without discharging  them. The SCM preparation goal is to prepare the chips from  the die backside up to the channels and active regions layer. This is done in two steps i) parallel lapping down to 10µm thin  silicon sample ii) thinning the remaining silicon down to a  thickness of 50-300nm by choline hydroxide chemical attacks. Based on its underlying principles, the SCM technique is  known to probe deep (during deep depletion mode) in the  semiconductor because it uses a DC and a AC voltages applied  on a metal coated tip in contact mode [3, 4, 5]. Thus, such  preparation makes possible a SCM probing down to FGT  channels.


In practice, it is quite impossible to achieve a 50-300nm thin  silicon layer on the entire memory. A bevel configuration with  a small slope (< 0.5%) is always obtained, where a small area (≈60µm large) is usable (Figure 7).


Figure 7: Optical view of 2T-cell Flash memory after SCM  preparation.


Carrier Density Measurements in FGT Channels


The objective is to directly measure carrier concentrations and  carrier types in FGT channels on Flash memories prepared at  active region levels from the die backside. SCM is a promising  tool to achieve such measurements:


Its capacitance resonator has a high sensitivity 10-22F/√Hz  to carriers which allows probing charges of a single  electron in theory [6].


Because it is a contact technique on an oxidized  semiconductor surface with DC and AC voltages applied  to the PtIr metal coated tip, SCM allows deep probing in  the semiconductor during the deep depletion mode [3, 4, 5]. This depletion depth (i.e the probing depth) is function  of the strength of applied field, the thickness of the oxide  between tip and sample and the free carrier concentration  of the sample. Playing with applied voltages, we found  that this Z-probing distance below the tip can be increased  up to ≈300nm. This allows probing down to FGT  channels from the backside substrate surface obtained  after preparation.


50X


Usable


2.5X


Bits of weight 7, odd addresses  Bits of weight 7, even addresses  Bits of weight 6, odd addresses  Bits of weight 6, even addresses  Bits of weight 5, odd addresses  Bits of weight 5, even addresses  Bits of weight 4, odd addresses  Bits of weight 4, even addresses


Bits of weight 3, odd addresses  Bits of weight 3, even addresses  Bits of weight 2, odd addresses  Bits of weight 2, even addresses  Bits of weight 1, odd addresses  Bits of weight 1, even addresses  Bits of weight 0, odd addresses  Bits of weight 0, even addresses


Sector 10       9         8        7         6         5        4     2  3  1  0


Zoom see Figure 4


Data Reading On 2T-Cell Flash Memory


Before preparation, a few addresses of the Flash table from  Atmel are programmed in order to have “12h”= “00010010” virtual data (8 neighbor bits). Thanks to descrambling, their  physical locations are known and can be scanned by AFM  based techniques. The most significant virtual bit is on the left  of Figures 8.


Figure 8-1 shows the topography of the channel layer obtained  from the die backside of 2T-cell memory after SCM  preparation. The structure is clean and undamaged. Field  oxides rise (D) just 50nm above the silicon surface and drain  contacts (A) are below it. An AFM scan on a region totally  free of silicon (not shown) was performed: the field oxide is  measured to be 200nm taller than the exposed tunnel oxide  layer. Thus, it is proven that there are only around 150nm of


Moasule


Dale Zuarm


350.0100Sectos


remaining silicon on the SCM region of interest. This  thickness is appropriate for probing down to FGT channels.


An Amplitude SCM signal (Figure 8-2) gives information


/100


about the carrier concentration. It is null on thick field oxides


05115225235


(D), weak on highly doped active areas (≈1019 at/cm3) as cell


Specbal RMSAmpl533#Temporal Foq 0.00Hz Spoctral Pricd 439gn


Spechal Freg 1228Aum


drains (A), S/D regions (B) and cell sources (C) and strong on


low-doped areas as exposed substrates (I, J) in open channels.


A Phase SCM signal (Figure 8-4) gives information about the


8 8


type of majority carriers, i.e. electrons or holes. It is null (0°)


on thick field oxide, dark (<-50°) on N-doped areas and yellow


2:dC/dVPhase


5.0μmg101821 21旭


(>+50°) on P-doped areas.


The Flash data are related to the concentration and the kind of  carriers in FGT channels, which lead to a conductive or a  blocked cell. A FGT transistor in a blocked state (“1” for  Atmel conventions) has a high density of holes in its channel, image of the high density of electrons stored onto its FG. Thus, its channel is open (OFF) and P-doped. Its corresponding  Amplitude SCM signal is strong and its Phase SCM signal is  yellow (in white circles).


Conversely, a FGT transistor in a conductive state (“0” for  Atmel conventions) has a high density of electrons in its  channel. Indeed, because of its negative threshold voltage (VT≈-2V) and the probing conditions (DC=-0.2V and AC=1V  applied to the tip), the inversion layer is reached. As a  consequence, a conductive FGT channel (in dark circles) appears with the same SCM levels as N source/drain regions. Electrical P-N junctions are not detected anymore between a  conductive N-type channel and its surrounding active regions. The Amplitude SCM difference between a blocked channel  and conductive one is measured around 600mV with only 1V  AC and -0.2V DC voltage applied to the tip. The Phase SCM  difference is around 180° (Figure 9).


FalHeoMencalsuteceAngeFneeCourtmFe


0 2.234


-176.518515.366-09.255 1380.000 0.0002.37.2470.220


Figure 9: Relative Phase SCM measurements between a  blocked FGT channel (rich in holes) and a conductive one (rich in electrons). The difference is measured around 180° as  shown. In the blocked transistor, PN junctions between the P  channel and its surrounding N active regions are clearly  detected. In the conductive transistor, the signal is a  homogenously N-type on source, channel, and drain areas. This proves that its inversion layer is reached and its  threshold voltage is negative.


1: Height


20.0 μm0.0


2:dC/dV Amp


20.0 jμm0.0


20.0μm0.0


2:dCAdVPhase


Figure 8: Contact AFM (Figure 8-1) Amplitude SCM (Figure 8-2) cantilever deflection (Figure 8-3) and Phase SCM (Figure 8-4) scans on active regions level prepared form the backside of 2T-cell Flash memory from Atmel. The blocked FGT channels (“1” for  Atmel conventions) are in white circles and the conductive ones (“0” for Atmel conventions) in black circles. The data are measured  as“12h”= “00010010” (from left to right) as they were initially programmed. (A) Cell drain, (B) S/D region, (C) cell source, (D) field  oxide, (I) AT channel, (J) FGT channel, (K) FGT tunnel oxide region.


A  B  C


I  J


AT  FGT


Messure


DaeZcon


500.0nmMosiuo


Dala Zcon


500.0m￥MossueTenDalaZoon


10.0 nmMealueRmDalaZoom


360.0*


1                 0


they 50


0   0   0   1    0   0   1  0


In Fig. 2 a cross-section through a vertical npn-transistor is shown. Figure 2a shows an SEM image of the same type of npn-transistor, for better comparison with the s-SNOM images  it is highlighted by oxide- and poly-etch. Figure 2b shows a topographic AFM image recorded simultaneously with the sSNOM images. Figure 2c shows the amplitude, and 2d the phase, s-SNOM images. The amplitude image shows sharp contrast between silicon, silicon oxide and the metallic areas –Al, W and TiN, in agreement with our earlier observations of a  similar sample [11]. The As-doped silicon region can also be out-lined. In the phase image the As-doped silicon is seen more clearly. It also shows good contrast between un-doped and doped silicon oxide. In addition, the silicon nitride passivation layer is shown very clearly in the phase image. It is  also worth noting that even though the surface is relatively rough, as shown in the topographic image, this does not seem to affect the quality of the s-SNOM images too much.


Figure 2: NPN-transistor: (a) SEM (secondary electron, inlens detector) image of the same type of NPN-transistor as shown in the s-SNOM images. (b) Topographic AFM image of  the same area as shown in the s-SNOM images. (c) Amplitude


image; silicon oxide appears dark, silicon intermediate, while metallic parts – Al, W, and TiN are bright. (d) Phase image;here the As-doped silicon, Al, and W appears bright, doped SiO2 intermediate, and Si and un-doped silicon oxide parts are dark. Note the very bright silicon nitride passivation!


LDMOS-transistor


A cross-section through an LDMOS-transistor was made by cleaving and polishing. In addition, this sample was ion-milled using argon ions at a grazing angle of 70°. In Fig. 3 a drain contact of such a transistor is displayed. Figure 3a shows an SEM image of the same drain contact taken after the s-SNOM imaging. To improve the contrast between the materials and doped areas, the sample was oxide- and poly-etched before SEM imaging. Furthermore the SEM image was cropped and rotated in order to simplify a comparison with the s-SNOM images. The etchants have clearly attacked a thin Ti-layer as marked in the image, as well as the highly doped area beneath the contact. Both these areas can be clearly seen in the phase and amplitude s-SNOM images in Fig. 3c and 3d, respectively. The thin Ti-layer is particularly clearly highlighted in the phase image. This layer is only about 20 nm thick. Beside these features the same distinctions can be made as in the images of the npn-transistor: In the amplitude image (Fig. 3d)the metallic, dielectric and semiconductor parts can be clearly differentiated. In the phase image (Fig. 3c) the doped area is very bright and TiN and W also clearly visible. Figure 3b shows a topographic AFM image taken simultaneously with the s-SNOM amplitude and phase images. It shows the effect of the varying polishing rate of the various materials, as well as some scratches left by the polishing procedure.


Figure 3: A cross-section through a drain contact in an LDMOS-transistor. (a) SEM (secondary electron, in-lens detector) image shown for comparison with the s-SNOM images. Please note how the thin Ti-layer has been etched away. (b) Topographic AFM image showing some scratches remnant from the polishing, as well as the effect of different polishing rates of the constituent materials. (c) S-SNOM phase  image. Noteworthy is the thin Ti-layer, as well as the highly doped area beneath the W contact. (d) S-SNOM amplitude image showing clear contrast between Si, SiO2 and the metallic areas; W, Ti, TiN and highly doped Si. It is also worth noting the slight contrast between the very bright TiN and the thin Ti-layer.


Comparison with other techniques


In comparison with already existing techniques, s-SNOM provides a number of advantages.


The most widely used microscopy technique in failure analysis  is probably scanning electron microscopy (SEM), which yields  nanoscale resolution and, in combination with decoration etching, both material and doping contrast [14]. The decoration etches are, however, non-quantitative and difficult to reproduce. Sometimes the result of decoration etches can lead to some confusion, as for example shown in Fig. 4a where  the etchant has attacked and removed most of the Ti layer, it has, however, also removed some silicon oxide at the interface  with the TiN. This may lead to the interpretation that there have been Ti also at this location, but as is shown in Fig. 4b this is not true.


Figure 4: Magnification of the cross-sectional image of a drain contact in a LDMOS-transistor shown in Fig. 3. (a) The  SEM (secondary electron, in-lens detector) image shows how both the silicon oxide and the Ti-layer have been etched away.


(b) S-SNOM phase image showing the Ti-layer.


SEM in combination with Auger spectroscopy, energy dispersive x-ray spectroscopy (EDX) or wavelength dispersive  x-ray spectroscopy (WDX) give good elemental sensitivity, the  spatial resolution is, however, rather poor.


Transmission electron microscopy (TEM) offers excellent spatial resolution, at this stage of development s-SNOM can hardly compete at this point. Zenhausern et al. claimed a 10 Å  resolution [15] using a version of s-SNOM, but if this can be reached in practical application remains to be shown. In combination with EDX or electron energy loss spectroscopy(EELS) TEM also yields elemental sensitivity [16,17]. One of the main drawbacks of TEM is the complicated and timeconsuming sample preparation necessary, in comparison the sample preparation needed for s-SNOM is very straightforward. In addition, for particular structures the requirements of TEM samples are causing problems [18]. For example, barrier layers around contacts of radius less than 50 nm are virtually impossible to image in any detail. This is because TEM-samples consist of lamellae of minimum ~50 nm  thickness that have to contain a cross-section of the region of interest, contacts smaller than that can thus not be crosssectioned but the lamella will rather contain the entire contact.


The barrier layer will than either be hidden by the contactmaterial or blurred by its own curvature. Since s-SNOM only requires a cross-section with one reasonably smooth surface this problem does not arise.


Determination of doping concentration range


By calculating the amplitude and phase response as a function of the doping concentration we have found [11] that for a wavelength of λ = 10.7 μm a resonance can be expected with Si at a doping concentration of about 3⋅1019 carriers/cm3.


Between approximately 3⋅1018 and 1021 carriers/cm3 the amplitude and phase responses changes, and thus it should be possible to map doping concentrations within this range.


Obviously areas with other doping concentrations, neighboring  to areas with doping within this range, can also be distinguished.


Doing the same calculation for a number of longer wavelengths it can be shown that the technologically most interesting range of doping concentrations, 1015 to 1021 carriers/cm3, can be covered by using a set of lasers operating at different wavelengths. The spatial resolution of the s-SNOM is not expected to increase with the longer wavelengths, since the resolution does not depend on the wavelength but rather on  the tip’s interaction with the sample. It should be noted that the  model available for such calculations is still under development.


We succeeded in mapping areas with various materials, as well  as doping levels between 3⋅1018 and 1021 carriers/cm3. Layers as thin as 20 nm could be clearly defined, suggesting a resolution in the nanometer range. The potential of s-SNOM to  combine the chemical sensitivity of infrared analysis with the spatial resolution of SPM makes it a promising tool for failure analysis of microelectronic circuits.


We acknowledge stimulating discussions with T. Taubner, N.


Ocelic and M. Brehm. Supported by BMBF within the young scientist competition in nanotechnology, 2002.


[1] Born, A. and Wiesendanger, R., “Scanning capacitance microscope as a tool for the characterization of integrated  circuits”, Applied Physics A, Vol. 66, (1998), pp. 421-426.


[2] Anand, S., “Another Dimension in Device Characterization – Scanning Capacitance Microscopy of InP-Based Laser Structures”, Circuits & Devices, March,(2000), pp. 12-18.


[3] Zimmerman, G., Born, A., Ebernsberger, B., and Boit,C., “Application of SCM for the microcharacterization of


semiconductor devices”, Applied Physics A, Vol. 76,(2003), pp. 885-888.


[4] Benstetter, G., Breitschopf, P., Frammelsberger, W.,Ranzinger, H, Reislhuber, P., and Schweinböck, T.,“AFM-based scanning capacitance techniques for deep sub-micron semiconductor failure analysis”,Microelectronic reliability, Vol. 44, (2004) pp. 1615-1619.


[5] De Wolf, P., Clarysse, T., Vandervorst, W., Hellemans,L., Niedermann, Ph., and Hänni, W., “Cross-sectional nano-spreading resistance profiling”, J. Vac. Sci.


Technol. B, Vol. 16(1), (1998), pp. 355-361.


[6] Schömann, S. and Alvarez, D., “Doping mapping by SSRM – reaching maturity and sub-10nm resolution”,Proceedings from the 30th International Symposium for Testing and Failure Analysis, (2004), pp. 346-349.


[7] Schweinböck, T., Schömann, S., Alvarez, D., Buzzo, M., Frammelsberger, W., Breitschopf, P., and Benstetter, G.


“New trends in the application of Scanning Probe Techniques in Failure Analysis”, Microelectronic reliability, Vol. 44, (2004), pp. 1541-1546.


[8] Knoll, B. and Keilmann, F., “Near-field probing of vibrational absorption for chemical microscopy“, Nature,Vol. 399, (1999), pp. 134-137.


[9] Knoll, B. and Keilmann, F., “Infrared conductivity mapping for nanoelectronics”, Applied Physics Letters,Vol. 77, (2000), pp. 3980-3982.


[10] Hillenbrand, R., Taubner, T., and Keilmann, F.,“Phonon-enhanced light–matter interaction at the nanometre scale”, Nature, Vol. 418, (2002), pp. 159-162.


[11] Hillenbrand, R., Huber, A., Kazantsev, D., Keilmann, F.,and Wittborn, J., “Infrared mapping of semiconductor device structures and doping profiles at nanoscale spatial  resolution”, submitted (2006).


[12] Ocelic, N., Hillenbrand, R., “Subwavelength-scale tailoring of surface phonon polaritons by focused ionbeam implantation”, Nature Materials, Vol. 3, (2004),pp. 606-609.


[13] Keilmann, F. and Hillenbrand, R., “Near-field microscopy by elastic light scattering from a tip”Philosophical Transactions of the Royal Society London. A, Vol. 362 (2004), pp. 787–805.


[14] Trudeau, F. G. and Joseph, T. W., “Metallographic Techniques for Semiconductor Device Failure Analysis”, Microelectronic Failure Analysis Desk Reference, 4th edition, ASM International (Materials Park, 1999) pp.


253-266.


[15] Zenhausern, F., Martin, Y., Wickramasinghe, H. K.,„Scanning Interferometric Apertureless Microscopy;Optical Imaging at 10 Angstrom Resolution“, Science,Vol. 269, (1995), pp. 1083-1085.


[16] Muller, D. A., Sorsch, T., Moccio, S., Baumann, F.


Evans-Lutterodt, H., K., and Timp, G., “The electronic structure at the atomic scale of ultrathin gate oxides”,Nature, Vol. 399, (1999), pp. 758-761.


[17] Batson, P. E., “Atomic resolution analytical microscopy”,IBM J. Res. Develop., Vol. 44, No 4, (2000), pp. 477-487,


[18] Mardinly, A. J., “Electron Tomography and ThreeDimensional Aspects of Transmission Electron Microscopy” Electronic Device Failure Analysis, Vol. 7,No. 3, (2005), pp. 6-12.


Identification of Root Cause Failure in Silicon on Insulator Body Contacted  nFETs using Scanning Capacitance Microscopy and Scanning Spreading  Resistance Microscopy


J.S. McMurray and C.M. Molella


IBM Microelectronics, Hopewell Jct., NY 12533


Root cause for failure of 90 nm body contacted nFETs was  identified using scanning capacitance microscopy (SCM) and  scanning  spreading  resistance  microscopy  (SSRM).   The  failure  mechanism was identified  using both  cross  sectional  imaging  and  imaging  of  the  active  silicon  -  buried  oxide (BOX) interface in plan view.  This is the first report of back -side plan view SCM and SSRM data for SOI devices. This  unique plan view shows the root  cause for  the failure is an  under doped link up region between the body contacts and the  active channel of the device.


A  number  of  90  nm  analog  circuitries  built  using  SOI  technology were found to fail at a higher than expected rate. Electrical probing showed unusually high off current in some  body contacted nFETs. Additionally, it was found that the off  current  could be modulated by applying a bias to the wafer  substrate.  This indicated that a positive charge in the BOX  could be causing an unwanted inversion layer leading to the  high off current. SCM [1] and SSRM [2] were used to examine  the carrier profiles of these failed devices.  A Veeco D5000  scanning probe microscope was used for both SCM and SSRM  measurements. The SSRM applications module available from  Veeco  was used  for  the  spreading resistance  measurements. The  SCM measurements  were  made  using a  custom sensor  described elsewhere [3].


Results from Cross Sectioned Samples


Sample preparation


SOI devices provide challenges for SCM analysis.  The main  problem is the SOI isolates the device.   Often,  most of the  voltage applied between the tip and sample is dropped across  the  BOX  resulting  in  no  SCM  signal.   If  the  device  (or  attached wiring) is large enough then a capacitance signal may  be  observed.  However,  the  signal  is  degraded  from what it  would  be  if  good  electrical  contact  were  established.   The  devices considered in this work are all small enough that no  SCM signal is obtained without establishing electrical contact.


Electrical  contacts  for  the  device  to  be  analyzed  can  be  fabricated with a focused ion beam (FIB).  First, a FIB section  is made into a plane of the device that will not be analyzed. The  FIB section is  extended through the device and  buried  oxide layer into the substrate silicon.  This trench is then filled  with FIB deposited metal [3]. The top surface of the wafer is  then  coated  with  an  approximately  7  nm  thick  layer  of  chromium.  It is found that this amount of chromium provides  a  good electrical  connection without optically obscuring the  wafer  surface.   This  is  important  since  optical  inspection  greatly aids precision cross sectioning.  A protective layer of  TEOS  is  added  to  preserve  the  chromium and  to  prevent  excessive edge rounding of the cross section during polishing A standard polishing tripod is used for the cross sectioning. The  sample  is  polished  using  successively  finer  diamond  lapping films until the area of interest is in the cross sectioned  plane.  The final lapping film used contained 100 nm diamond  particles.  To remove residual scratching, a brief polish using  colloidal silica is applied.   To create the thin surface oxide for  the  SCM  measurements,  the  samples  are  placed  under  an  ozone generating UV light for approximately 30 minutes [4].  This procedure  was followed with the FIB contact  passing  through the body contact and the imaging cross section placed  in  the  active  width  of  the  device.   This  configuration  is  illustrated in Fig. 1, which shows the added FIB contact and  layout data for the devices in question.


With this configuration, no SCM signal was observed in the  device  area.  The  SCM results  are  shown in Fig 2.  The  top  image is  the  topography and  the  bottom is  the  capacitance  signal. The SCM is set such that positive signals are p type and  negative are n-type. The capacitance signal is plotted such that  yellow to white colors represent p-type carriers and the brown  to black represent n-type as is indicated in the color bar to the  right of the capacitance image.  The black arrows above the  images in  Fig.  2  are  pointing  to  the  lateral  position  of  the  devices.  The poly gates are evident in the topographic image  due to differential polish.


## Identification of Root Cause Failure in Silicon on Insulator Body Contacted nFETs using Scanning Capacitance Microscopy and Scanning Spreading Resistance Microscopy


102


Figure 1: Sample one configuration showing the added FIB   contact passing through the body contact area of the device.  Green, cyan, purple and red regions represent, active silicon,  poly  silicon,  tungsten  interconnects,  and,  FIB  contact  bar   respectively.


It  was expected  that  the  body of  the  device  and  extension  would  be  observed.  The  high  doping  in  the  source  drain  regions result in a SCM signal which is too small to detect with  small tips.  The lack of SCM signal was originally thought to  be the result of sample preparation.  However, several more  samples were subsequently prepared and no SCM signal over  the  device  area  was  found  (Fig.  2).   The  p-type  substrate (bottom of SCM image in Fig.  2)  is  clearly seen below the  buried oxide, indicating that the capacitance sensor is working  properly.


The  lack  of  signal  was  later  attributed  to  poor  electrical  contact.   A  new SCM  cross  section  was  then  prepared  as  shown in Fig. 3.  The main difference between this new sample  and sample in Fig.  1  is  that  the location of  the SCM cross  section and the FIB contacts were exchanged.


Figure 4 shows the topographical image of SCM cross section  described in Fig. 3.  This cross section is through the body link  up region of a nFET and the source/drain/body of an adjacent  nFET.


Figure 2: Topography (top) and capacitance (bottom) images  of SCM cross section shown in Fig 1. No SCM signals were   observed under gates and above buried oxide.   p-type SCM  signals  were visible  in  substrate  below buried  oxide  in  the   capacitance image.  BOX thickness is 150 nm. SCM signals   expected at this vertical distance at arrowed locations.


Figure 3: Sample two configuration showing the added FIB  contact passing through the source/drain/body region of the   device. Green, cyan, purple and red regions represent, active   silicon., poly silicon, tungsten interconnects, and, FIB contact   bar respectively.


Gate,active  region


Wide poly over link up region.


Figure 4: Topography of a precision cross section compared   with layout data. Color coding of the layout data is the same   as  in  Figure  3.  Topography  from differential  polish  shows   section is through the body contact of a device (top left) and   the source/drain/body of an adjacent device (top right).


Figure  5  shows  the  capacitance  image  obtained  with  the  topographic  image  in  Figure  4.  No  capacitance  signal  is  observed in the body link up region of the left device while a  small  p-type  signal  from  the  body  of  the  right  device  is  observed.  A larger SCM signal is also observed from the tip  making contact with the tungsten wiring.  The no SCM signal  in the link up region, again suggests that there is a problem  with this region of the device.


To confirm that the problem was not electrical contact to the  left  device  shown in  Figure  4,  the  sample  was  repolished, slightly  further  into  the  source/drain/body  region  and  remeasured with SCM.  Results are shown in Figure 6.


The body and the extensions of the device are now measurable  by SCM.  This indicates that appropriate electrical contact to  the device was achieved during sample preparation and that  there is an unexpected problem in the body link up region of  the device.   The p-type signal from the body showed that the  device  was not  fully depleted.  Additionally,  an n-type  layer  which could explain the high off current was not imaged at the  interface above the BOX.


The fact that the off current could be modulated by substrate  bias  suggested  that  the  device  was  not  fully  depleted  and  indicated  that  the  problem was  at  or  near  the  silicon-BOX  interface.   To  visualize  the  problem  area  a  new  sample  preparation technique was needed, back-side plan view.


p- substrate


BOx


Tungsten Trenches


Figure  5:  Cross  sectional  SCM  image  from  sample.  Corresponding  topographic  image  is  found  in  Fig  4.  No  signal is observed in the body contact region of the left device   while  a  p-type  signal  from the  body  of  the  right  device  is   observed.


Figure  6:  SCM  image  for  sample  two.  The  sample  was  repolished  through  the  body  contact  region  into  the  active  section of the device.  SCM signal from device is present and   an inversion layer is not found below the device.


Back-Side Plan View Sample


Creation of back-side plan view samples suitable for SCM and  SSRM is similar to creating back-side plan view samples for  secondary ion mass spectrometry (SIMS).  Details of current  sample preparation techniques were given at this year’s SIMS  workshop [5].   Samples appropriate for SCM and SSRM have  the additional requirement that all the diffusions in the device  must  be  electrically  contacted.   A  brief  outline  of  the  procedure is given below.


Electrical  contact  to  the device  can be  obtained  by parallel  polishing  the  device  from the  front  side  until  the  tungsten  wiring contacts are exposed. A thin layer of chromium is then  sputtered over  the surface of the wafer.   For the devices in  question this contacts the source/drain and body contact.  This  can be seen from the layout data in Figures 1 or 3.  A blank  piece of silicon is epoxied to the chromium side of the sample. The sample is then mounted on the holder of an Allied High  Tech Multiprep polishing machine. The sample is then parallel  polished  to  remove  this  silicon  substrate.  The  polishing  is  continued  until  optical  fringing  is  seen  over  the  area  of  interest.


At this point, a thin layer of silicon was left over the buried  oxide.  This layer of silicon was removed using a CF4 reactive  ion etch (RIE) to expose underlying buried oxide.  The buried  oxide  layer  was  then  removed  using  a  timed  etch  of  10:1  buffered hydrogen fluoride.  This process exposes the device  silicon BOX interface.


Back Side Plan View SCM Results


The topography of the failing devices is shown in Figure 7-A.


The  silicon  being  raised  from the  surrounding  surface  is  a  result  of  the  STI  etched  away  during  the  BOX  removal  process.  The holes in the silicon on the right device are from  pitting induced in the CF4 RIE process.  Refinement of the  RIE process on subsequent samples has eliminated the holes. The tungsten wiring for the devices is visible, as well as the  heavily  n-type  doped  source/drain  regions  that  are  slightly  etched.  The body contact (near the lower tungsten wiring) and  the  linkup  region,  between  the  body  contact  and  the  source/drain/body, appear smooth.


Figure  7-B,  shows  the  SCM  image  corresponding  to  the  topography of  Figure  7-A.   This  image was taken with the  frequency of SCM sensor adjusted to the maximum slope of  the resonance curve on the high frequency side. As expected, small  magnitude  SCM  signals  are  evident  over  the  body  contact  and  source  drain  regions  indicating  a  large  carrier  density.  The polarity of the signal is also correct,  p-type for  the body contact  and  n-type for the source drain region.  A  large signal is  also obtained when the tip is in contact  with  tungsten wiring.


Figure 7.  Backside topography (A) and SCM (B).


images of failed body contacted pFETs.  SCM images show  that there is an area in which no carriers are detected in the   link up region between the body contact and the active area of   the device.


What is unexpected is that the body linkup region shows no  SCM signal.  It is also noted that the p-type signal from the  body contact  has  a  gradient  with the  signal  growing larger (smaller number of carriers) toward the link up region.  It is as  if  the carrier  density suddenly dropped  below the detectible  limit.  Initially this did not seem likely since SCM has been  shown to be sensitive to carrier densities below 1015 cm-3 [1] and the silicon wafers used in this technology are boron doped  to the 1015 cm-3 level.  Figures 2, 5 and 6 show the expected ptype response in the substrate showing that  the SCM sensor  used can easily detect this level of carriers.


Both the body contacted pFETs and nFETs were designed to  have similar carrier densities in the link up region. Electrical  probing of the pFETs confirmed that they were functioning as


expected.  Nearby pFETS were imaged and the results of these  measurements are given in Figure 8.


Figure 8 A shows the SCM image of a failed body contacted  nFETs.  This image was taken by setting the frequency of the  sensor  to  correspond  with  the  maximum slope  on  the  low  frequency side of the resonance curve.  The drive amplitude of  the RF generator was kept constant.  This caused the phase of  the capacitance signal to change.  But the phase of the series  resistance  signal  was unaffected.   The  phase  of  the  lock in  amplifier was also shifted 180 degrees, so that p-type signals  would still  appear  positive.    Note that  the  signal  from the  tungsten wiring changed phase,  indicating that  this  signal  is  due to a resistance effect.  The sensor is significantly loaded  when the tip contacts the wiring.  Otherwise the images look  very similar.


One possibility for a zero signal region is a balancing of the  capacitance signal with the series resistance signal.  The test  for  this  is  switching  the  capacitance  sensor  from the  high  frequency side of the resonance to the low frequency side. The  comparison of these setting is given in Fig 7-B and Fig 8-A. The fact  that  there is  no SCM signal  in the link up region  under  this  change  of  measurement  conditions  rules  out  the  lack of signal in the link up region being due to the balancing  of capacitance and series resistance signals.


Figure 8-B shows the SCM image of adjacent pFETs in the  circuit.  For these devices, the capacitance signal is evident for  all parts of the device. Particularly, the SCM signal in the ntype link up region is continuous between the body contact and  the body of the device.  This is in contrast to those observed in  Figures 7 and 8-A where SCM signal is observed.


Back Side Plan View SSRM Results


To understand the no SCM signal in the link up region of the  nFETs,  the  complimentary technique  SSRM was employed. Standard coated doped diamond tips from Nano-sensors were  used.   The  pressure  required  to  make  a  consistent  ohmic  contact to the silicon is such that the silicon is damaged during  resistance imaging.  As such, only one image can be recorded  before  the  surface  is  damaged  and  the  resistance  signal  is  changed due to the damage.   This effect is seen in Figure 9. The left half of the image was measured several times while  the  SSRM  parameters  of  pressure  and  bias  were  being  optimized.  The right half of the image is the first resistance  measurement for the region.  The pFETs in  Figure 9 are the  same as those in Figures 7 and 8.


The color bar in Figure 9-A represents the relative resistance  of the different regions.  The top of the color bar is the highest  resistance, the bottom the lowest.  The lowest resistance in the  image is  where  the  tip  is  contacting  the  tungsten wiring as  would be expected.   This  resistance level  is  consistent  with  directly contacting a bulk metal sample, again indicating that  the electrical contact to the devices is good.  The resistance  map also shows that there is a carrier gradient from the body


contact to the link up region and the carrier level in the link up  region is constant.


Figure  8:Back-side  SCM  image  of  failed  nFETs  (A)  and   functional adjacent pFETs (B).  Note that a n-type signal is   evident in the body contacted region of the pFETs while a ptype signal is lacking in the nFETs.


The SSRM sensor is designed so that a 1V change in its output  corresponds  to  a  one  order  of  magnitude  change in  carrier  density (6).  The black line in Figure 9-A shows the location of  a  line  profile  extracted  from  the  resistance  map.   This  resistance line profile is shown in Figure 9-B.  The red markers  show the location of the body contact and the center of the link  up region where no SCM signal is observed.  The change in  voltage from sensor output measured between the markers is


4.02  V.   The  expected  carrier  density  in  the  body  contact  region is nearly 1020 cm-3.  The SSRM data indicates that the  carrier density in the link up region to be less than 1016 cm-3, much less than the expected value of approximately 3 X 1017  cm-3.


Figure 9 A) Resistance image of failing pFETs. Left half of   image has been imaged multiple times.  The right half of the  image  was  measured  only  once.   B)  Resistance  profile   extracted from where the black line is in Figure A.  Vertical   distance between the markers is 4.02V.


Discussion of Results


Both cross sectional SCM and Back side plan view SCM show  that the device link up region of the body contacted nFETs was  devoid of a capacitance signal. The cross sectional results also  indicate  that  this  region is  a  high resistance  region since  it  isolated the source/drain/body region of the device from the  body contact. The SSRM results confirm that the link up has a  lower than expected carrier density.


The  low carrier  density  in  the  link  up  region  makes  these  devices susceptible to charge build up in the buried oxide.


The charge causes a complete depletion of the body contact  which makes the  body contacted  pFETs  essentially  floating  body devices.  It also allowed the edge of the device near the  link up region to invert, causing the high off current.


The  combination  of  SCM  and  SSRM  techniques  help  to  identify root cause of this problem to be an under doped link  up region.  The remaining question is why the link up region is  devoid of SCM signals, even though SCM sensor can detect  lower  carriers  concentrations  then  are  shown by the  SSRM  measurements.


The answer to this question is to realize that measurements in  thin slides  of  silicon found in SOI  devices  can be  different  from measurements in the bulk silicon.  In SCM measurements  of bulk samples, the extent of the depletion region is governed  by the Debye length. For SOI devices, if the thickness of the  silicon is thin compared to the depletion region that would be  formed over a bulk silicon samples, it is like a dielectric for  SCM measurements.  It  becomes impossible to  modulate  the  depletion region when there are too few carriers in the probing  volume  to  screen  the  field  from the  tip.   The  field  cannot  expand vertically to thicker than silicon layer and the lateral  extent of the depletion region is limited by the tip geometry  and the poly silicon underneath the silicon.


For thin silicon that has a low carrier concentration, it can be  helpful  to  think  of  the  number  of  carriers  in  the  probing  volume and the detection limit in terms of number of carriers  to  detect.   Figure  10  shows the  number  of  electrons in  the  possible  probing  volume  for  this  geometry.   For  this  calculation it is assumed that the silicon is 50 nm thick and the  tip radius is 15 nm.


Number of electrons in the probed volume.


Dopant Density (cm-3)


1e+15


1e+16


1e+17


1e+18


1e+19


0.01


0.1 1


100 1000 10000


Figure  10:  Possible  number  of  electrons  in  the  probing   volume  for  BACK side  plan  view  sample  as  a  function  of   dopant density.


For  the  carrier  density  seen  by  the  SSRM  technique  there  would be less than one carrier in the probing volume, which  would be undetectable.  If the carrier density is less than the


detection limit, the SCM effectively probes through the silicon  as if it were a dielectric.  This is exactly what is seen in Figures  7-B and 8-A.


SCM and SSRM were used to identify the root cause of the  failing body contacted  pFETs  to  be  an under  doped  linkup  region.   With this  information changes to  the  process  were  made  to  prevent  further  problems.   Good  electrical  contact  allows SCM analysis on cross sections of devices built using  SOI technology.  A method of ensuring good electrical contact  to  devices  using  a  FIB  was  demonstrated.   A new sample  preparation  technique,  back  side  plan  view,  with  electrical  contact for SCM and SSRM measurements, was described and  demonstrated.  An unexpected carrier detection limit for SCM  was discovered and explained as an effect of a limited number  of carriers in the probing volume.


The authors would like to thank Paul Ronsheim of IBM for  many useful discussions.


[1]   McMurray, J. S., “Two Dimensional Dopant Profiling by  Scanning Capacitance Microscopy”,  PhD Thesis, University  of Utah, Physics Department, 2000


[2] Dewolf, P. DE.,  “Two Dimensional Carrier Profiling of  Semiconductor Structures with Nanometer Resolution”,


PhD Thesis, University of Lueven, 1998


[3]  McMurray, J.S.  et al,  “Scanning Capacitance Microscopy  Evaluation of Junction Position in Vertical Dynamic Random  Access  Memory”,   Proc  8th International  Workshop  on: Fabrication, Characterization, and Modeling of Ultra-Shallow  Doping  Profiles  in  Semiconductors,  Daytona  FL,   June  5-8  2005 pp. 24-31


[4]  V.V.  Zavyalov,  et  al,  “A  Scanning  Capacitance  Microscope  Methodology  for  Quantitative  Analysis  of  P-N  Junctions,” J. Appl. Phys. 85(11), 7774 (1999)


[5]  Ronsheim, P. A.  et al,  “Device Specific Backside SIMS  Sample Preparation”,  Proc 19th Annual Workshop on SIMS, Rancho Mirage CA,  May 2006


[6]  SSRM  Applications  Module  Documentation,  Veeco  Instruments, Santa Barbara CA.


Intermittent Failures in High Pin Count Packaging


Ramesh Varma, Richard Brooks, Ronald Twist and James Arnold


Northrop Grumman Corporation, Electronic Systems, Linthicum, MD, USA


Cleston Messick


Northrop Grumman Corporation, Mission Systems, Clearfield, UT, USA


In a prequalification effort to evaluate the assembly process  for the industrial grade high pin count devices for use in a  high reliability application, one device exhibited  characteristics that, without corrective actions and/or  extensive screening, may lead to intermittent system failures  and unacceptable reliability. Five methodologies confirmed  this conclusion: (1) low post-decapsulation wire pull results;


(2) bond shape analysis showed process variation; (3) Failure  Analysis (FA) using state of the art equipment determined the  root causes and verified the low wire pull results; (4) temperature cycling parts while monitoring, showed  intermittent failures, and (5) parts tested from other vendors  using the same techniques passed all limits.


With present day high pin count packaging, intermittent  problems can be a function of the system design, software, testing and manufacturing techniques, making the  determination of the root cause of intermittent failures  extremely difficult.  Typically, system design engineers may  spend weeks trying to solve intermittent problems relating to a  design, when it may be just a function of the parts used in the  development.  Worse, field engineers trying to solve  intermittent failures in complex systems may spend significant  resources without discovering that the problem lies within the  high pin count integrated circuit.


Performing reliability testing several high pin count products  for use in a high reliability system found low wire pull results  on one such product.  Because these devices were plastic  encapsulated, the first step removed (de-encapsulated) the  plastic.  Next, the bonding wires were destructively pulled, measuring the necessary force.


Typically, this wire pull test results in the wire breaking at the  weakest point.  Initial inspections found that the test resulting  in the bond pulling up the pad area underneath the bond.  This  paper describes the failure analysis efforts used to determine  the validity of this test, the root cause of this anomaly and the  results of a test to conclude whether the low wire pull results  could cause a failure in a system.


Wire Pull Procedure and Results


Wire pull is a destructive test that measures the integrity of the  bonding process, where a gold wire connects the silicon based  die to the lead frame.  The first step removes the plastic  encapsulation material by either spraying or dripping fuming  nitric on the plastic, which causes the plastic to dissolve, exposing the wires and die.  Using a solvent to rinse the die  stops the chemical reactions.


Figures 1A-D: Decapsulation and wire pull process


Table 1 shows the wire pull results by date code for vendor A.  Date codes 0449 and 0537 failed the Mil-Std 883 lower limit  of 1.5 grams for a 0.9 mill wire, while Date code 0529 passed.


1A: Part prior to  decapsulation


1-C: Decapsulation by  Red Fuming Nitric


1B: Part after  decapsulation


1D: Typical; Wire  pull Tool


## Intermittent Failures in High Pin Count Packaging


109


Date Code


Min Max Avg SD


% Failure


# Wires  pulled


0449 0.1 8.3 2.5 1.0 23


0537 0.1 5.4 1.9 0.8 40


0529 2.7 5.0 3.2 0.4


Table 1: Wire pull test data Vendor A


Figure 2: Bond pads after wire pull


The bonds that lifted (Fig.2, right) generally had lower wire  pull results than the ones where the wire broke at the neck of  the ball.


Wire Bonding Process


A thermosonic process was used for wire bonding.  A  schematic of the wire bond is shown in Fig.2.  The gold ball is  alloyed to the Aluminum pads.


Figure 3: Wire bond schematic


Failure Analysis Planning


Upon the test failure, an FA effort started immediately with  the following objectives as listed:


1. Determine the validity of the test.  Did the testing  procedure cause the failure?


2. Should the limits and failure criteria be changed?


3. Are the failures limited to one date code?


4. Can a non-destructive test screen inadequate parts  from adequate parts?


5. What is the root cause of the failure?


6. Can communication of the root cause of the failure  to the vendor lead to a usable part?


7. Does the root cause lead one to conclude that the  part is unacceptable?


The possible root causes evaluated include:


1. Fuming nitric acid used to decapsulate the plastic  compromising the bond by over-etching and undercutting


2. Kirkendall voids (caused by Au-Al alloys of different  volumes) forming extensively across the bond


3. Kirkendall affects could cause lack of adhesion


4. Too much energy used during bonding, damaging the pad


5. The top barrier metal (Titanium) not adhering to the  Aluminum


6. The barrier metal under the Aluminum not adhering to the  dielectric


Failure Analysis


To determine the acceptability of the decapsulation process, a  part was decapuslated in two steps.  First, following the  normal process, only half of the die was exposed to acid  etching.  Again, following the normal process, but repeating  the process on the other half of the die, the first half of the die  was exposed for a second time.  A statistical analysis showed  no difference between the wires receiving the double etches  compared to the wire which received only a single etch.  Next, the etching mask was off-set so that the amount of exposed  wire on one side of the die was significantly larger than on the  other side.  Fig. 4 shows a significant difference in the amount  of wire exposed on the right, compared to the left.


Figure 4: Exposed wires


Although shorter wires on the left had a significantly lower  wire pull result when compared to the longer wires on the  right, no difference in failure rate occurred.


Another confirmation of the validity of this test comes from  data taken on other high pin count devices which did not  exhibit any failures.  Table 2 shows a big difference in the


data from vendor A, which did show intermittent failures, while vendors B and C did not.


Vendor A


Ser # Result Min Max Avg SD #C #A


Fail 0.1 3.4 1.4 1.1 9 31


43


Fail 0.1 3


0.9 0.6 0 40


54


Fail 0.4 4.9 3.1 1.2 37 3


56


Fail 0.9 6.6 3.2 1.1 35 5


64


Fail 0.7 5.7 2.7 0.9 30 8


72


Fail 0.3 4.1 2.6 1.1 23 17  120 Fail 0.4 6.4 2.7 1.1 27 13  154 Fail 1.5 8.3 3.6 1.2 33 7  188 Fail 1.2 4.6 2.4 1.8 40 0  Vendor B


Ser # Result Min Max Avg SD #C #A  11 Pass 5.2 8.9 7.2 1.0 37 3  24 Pass 6.1 10.6 7.7 0.8 40 0  42 Pass 6.0 12.2 8.1 1.5 40 0  72 Pass 6.4 10.5 8.7 0.8 40 0  76 Pass 5.9 9.8 8.6 0.8 40 0  84 Pass 6.0 9.0 7.3 0.7 40 0  90 Pass 6.1 9.0 7.1 0.7 40 0  105 Pass 5.0 10.2 8.5 0.9 40 0  110 Pass 6.0 11.5 9.2 0.7 40 0  Vendor C


Ser # Result Min Max Avg SD #C #A  59 Pass 4.9 9.8 7.2 1.3 39 1  60 Pass 6.2 8.1 8.1 1.1 40 0  88 Pass 3.9 9.3 6.7 1.4 39 1  108 Pass 5.1 8.6 6.3 0.9 40 0  177 Pass 5.4 10.0 7.5 1.3 40 0  178 Pass 7.1 12.1 8.6 0.8 40 0  249 Pass 5.1 10 7.7 1.3 40 0  252 Pass 4.9 9.6 6.6 1.2 35 5  261 Pass 5.3 7.9 7.9 1.6 40 0  263 Pass 5.0 9.1 7.3 1.5 40 0


Table 2: Wire pull test data


Failure Mode: #A Ball bond lifting, #C Break at the neck


SEM analysis provided the following micrographs showing  extreme variation in ball shapes and die pull results for one  date code, 0449.  SEM analysis of other date codes and other  vendors did not show such variation.  Date code 0449 serial #43 had an average of 0.9gm, a minimum 0.1gm, and a  maximum 3.0gm (Fig.5) and showed a very “elephant foot” shaped ball bond rather than the traditional “inverted  mushroom” shaped ball bond indicating a low temperature  and/or force during the scrub.   Figure 6 shows the SEM and  pull test results of another die from the same date code 0449.  The ball shape in Figure 6 is significantly different from  Figure 5.


Figure 5: SEM of Date Code 0449 SEM


Figure 6: Second die from Date Code 0449


Wire pull results: Average of 2.4 gms, Minimum of 1.2 gms, and a Maximum of 4.6 gms.


Assembly experts evaluated the gold ball shapes and  hypothesized that the shape variation showed extreme process  variations.  Further discussions included the idea that the  bonding technician possibly was varying the pressure and  temperature of the bonding processes according to the  integrity of the pad.


The ball shape on wire bond for date code 0449 (Fig.5) does  not pass typical industry inspection standards.  Bond crater  after wire pull shows a weak metal interface (Figures 7&8).


Auger depth profiling (Fig.9) of the pulled up pad on the  bottom of the ball shown in Figure 8 clearly indicates that the  Titanium film lifted with the ball.


Figure 7: SEM of bond site after wire pull


Figure 8: SEM of wire bond after pull


Figure 9: Auger depth profiling of the pulled up pad on the  bottom of the ball shown in Figure 8 definitely shows that the  Titanium lifted with the ball.  Notice Titanium (Ti) at the  surface which decreases as the Gold (Au) and the Aluminum (Al) increase


Figure 10: SEM micrograph shows the ion milling through  the bond, the pad and the underlying silicon


Figure 11: FIB cross section showing lifting Titanium


Figure 12: FIB Cross section details showing practically no  alloying of the Gold ball and the Aluminum pad


SEM, Focused Ion Beam (FIB) and Auger showed an  inadequate bonding process due to lifting Titanium for date  code 0449.  The same analysis for date code 0537 showed in  addition to lifting Titanium, no Au-Al intermetallic formation.  The FIB cross section (Figure 11) shows a normal ball bond, the Au-Al intermetallic with some Kirkendall voids, the  undercut Aluminum at the edge of the bond due to the Red  Fuming Nitric etch, and the underlying metal pads with the  accompanying Tungsten plugs.  Notice the abnormal Titanium  lifting.


The FIB milling was performed to investigate the lifting  bonds.  SEM analysis of the FIB cut revealed Titanium lifting  off the dielectric.  Further investigation revealed bonds that  lifted without wire pull (Fig.14).  This confirmed our  assumption that failures seen are clearly associated with poor  Titanium adhesion to the dielectric.  Auger depth profiling  further confirmed this conclusion (Fig.9).


The same SEM and FIB analysis was performed on date code


0537.  These die did not exhibit the extreme ball shape  variation seen on date code 0449.  Although some Titanium  lifting was found, the main cause for the low wire pull results  was that the Aluminum pad and the Gold bond did not form  adequate intermetallic (Fig.12 & 13).


Figure 13: This SEM of a date code 0537 pad shows where  the left half of the bond did not form an intermetallic, while  the right hand side shows the Titanium lifted.


Measurement of Intermittent Failures


The above analysis demonstrated a real problem in two  different date codes nearly a year apart.  However, the  question still existed:  Does this present a system reliability  problem?  In other words, does plastic encapsulation hold the  ball bond in close enough contact, that lifting pads or very  little actual alloying cause a real problem?


It is important to note that these devices passed all standard  reliability testing.  Upon revisiting this passing data, we


Figure 14: SEM of bond lift without wire pull.  Is the plastic  encapsulation sufficient to hold such a bond in place to make  reliable, constant contact?


discovered that many of the parts had failed testing after  undergoing the stresses.  However, it was the laboratory’s  procedure to retest the failures because experience had shown  that most of the failures in high pin count testing was due to  incomplete contact with each pin during testing.  Thus, the  laboratory implemented the procedure that all failing parts  would be cleaned, visually inspected for bent pins and  retested.  If the part passed, it was not considered a failure.


In order to investigate the impact of poor wire bond, the  laboratory performed active thermal cycles.  In this  experiment, each part was tested by continuously monitoring  the electrical signals from 185 pins while the device was  subjected to thermal cycle ranging from -55C to 125C.


One part that previously failed, but passed upon retest, went  through the above monitored thermal cycle twice with the  following results:


7 pins failed during the first cycle


10 pins failed during the second cycle.


2 pins failed only during the first cycle only


5 failed only during the second cycle.


Upon reaching thermal equilibrium, the part passed all  electrical tests which mean that these failures are intermittent  and can easily be missed by standard shock and thermal  cycle tests.


Forty five parts were subjected to one cycle of the monitored  thermal cycle with the following results:


15/15 (all) of the parts that had been thermal cycled for  1000 cycles from -55 to 125 degrees Centigrade showed  intermittent failures.


Only 6/15 parts that had been put on long term storage  test at 150 degrees Centigrade for 1000 hours showed  intermittent failures.


11/15 parts that had been stressed at 130 degrees  Centigrade and 85% humidity for 96 hours showed  intermittent failures.


All parts would pass at least once if tested enough at a  stable temperature.


The diode resistance was continuously measured as the  temperature changed from -55C to 125C. This cycle was  repeated a second time.  Note the intermittent failures shown  in Fig.15 when the part was heated.  These parts also failed  functionally.


Res


Figure 15: Diode Resistance vs. Time during temperature  variations.  The points outside of the curves indicate an  increase in resistance that lead to intermittent failures.


Summary of Failure Analysis


The FA effort met its objectives:


The test is valid and did not induce the failures:


Over etching or changing the length of the  exposed wires did not increase the failure rate.


FIB cross sections showed that the etching under  the bond pad by the red fuming Nitric acid was  not significant.


No, the parts failed electrical testing  intermittently at room temperature and during  thermal cycles.


No, although one date code did pass, and some  parts in all date codes passed, two date codes  manufactured almost a year apart exhibited  significant problems.


Yes, electrically monitoring the parts during  thermal cycling found intermittent failures


Both lifting Titanium and non-alloying were  found to be root causes.


Yes, the vendor is addressing the problem both  in implementing increased testing and working  with the assembly facility to ensure problems are  identified and the fabrication facility notified.


Without vendor action, the part would be  unacceptable in any high reliability system, although its use in many applications, such as  mobile phones, might be acceptable.


Decapsulation of plastic parts and wire pull testing can reveal  significant bonding problems and should be included in  qualification procedures.  Large ball bond shape variation is a  sign of potential bonding problems.  FIB milling and cross  section inspection of the ball bond and interfaces can discover  root causes of bonding problems.  Bonding problems can  cause intermittent failures and must be included in any  intermittent failure analysis.  Traditional testing where failing  parts are retested until passing can lead to incorrect results.


Intermittent failures pose significant problems for electronics  systems.  On a complex system, FA for this intermittent  problem would be so difficult that on most systems, it would  never be identified.  We recommend that reliability testing  should include temperature cycling under power to catch this  type of problem.  Further, de-capping and wire-pull tests also  provide valuable information to improve processes.


Silicon Turnkey Solutions (STS) of Fremont, California, particularly Zef Malik, provided the initial data and much  expertise in arriving at the conclusions reached in this paper.


Levine, L et.al.,  “Improving intermetallic reliability in ultra  fine pitch wire bonding”, SEMICON Singapore, 2004


Matusiewicz, G.R, Kirch, S.J, Seeley, V.J,  “The role of


Focused Ion Beam in physical failure Analysis”, IEEE/IRPS, 1991


Murali, V et.al., “Wire bonding of Aluminum/Polyimide


multilayer structures”,  IEEE/IRPS, 1992


Microstructure Analysis of Wafer Bump Nodule


Xianfeng Chen, Tingfeng Ge, Lisa Tsou, Ming Li, Chorng Niou, W.T. Kary Chien


SMIC (Shanghai) Corp.18 Zhangjiang Road, Pudong, Shanghai, China, 201203  Fairy_Chen@smics.com


The bump nodule growing in electroplating process could be  large enough to induce bump to bump short even if the nodule  would be weaken by re-flow process. In this work, the  microstructure of PbSn eutectic bump and Au bump nodules  was analyzed with FIB, SEM and EDS. In PbSn eutectic  bump nodule, void defects can be observed with FIB imaging. In Au bump nodule, eradiation-like grain structure around the  center of Silicon-contained particle can be observed. Based on  those analysis results, voids and particles are the source of  bump nodule growth. The reason for bump nodule formation  is that particles, voids and cathode morphology defects change  the roughness of cathode surface, which induces a higher  current density area and accelerate local electrocrystallization. Generally, particles, voids and cathode  morphology defects are caused by poor photolithography  process, tank corrosion and anode contamination such as  passivation membrane. Therefore, three conclusions are  proposed in this work: 1) where and when the nodules grow  can be identified according to their microstructures; 2) cleaning tank and anode periodically can effectively prevent  the bump nodules; 3) Qualified photo resist (PR) coating and  PR opening process are essential to prevent bump nodule  defects.


Evaporation, printing, stud bump and plating are four most  common technologies for wafer bump deposition. Evaporation  has the limitations of high cost and low throughput. Although  printing has an inexpensive vantage, it would suffer yield loss  for fine pitch application (below 200um). Stud bump also has  low throughput limit for mass-production. As the most applicable process, electroplating is increasingly used in wafer  bump deposition based on the considerations of bump size, pitch, high volume production and geometry.


Compared with vacuum evaporation sputtering technology, non-vacuum electroplating process can easily introduce  particles even in the clean room environment. Although the  wafer bump process has wider tolerance to the particle attack, it still induces serious wafer yield loss.


In this work, several effective failure analysis solutions and  process improvements are proposed to identify the sources of  nodular defects.


Short loop wafer was studied in this work. Bump structure  was based on PbSn eutectic bump with Cr/Cu-Cu/Ni as UBM (Under Bump Metal). The Cr film acts as the adhesion layer  and Ni as the barrier layer. Cr/Cu film was deposited with  PVD (Physical Vapor Deposition) process. Cu/Ni and PbSn  solder were deposited by two continuous separate  electroplating steps. There are PbSn layer1 and PbSn layer 2  on mushroom bump before they are processed with re-flow. Fig 1 illustrate PbSn eutectic bump before re-flow process.


Solder


Fig.1 The eutectic wafer bump before re-flow process


The other investigated bump structure was based on Au bump  with Ti/W UBM (shown on Fig.2). Au bump was also  deposited with electroplating.


Bump microstructure was analyzed with Hitachi SEM-4700  system after cross section polishing and Argon sputter milling, which had been processed with Gatan’s PECS (Precision  Etching Coating System). Nodular defect microstructure was  analyzed with FIB (Focus Ion Beam) imaging system and  EDS (Energy Dispersive Spectrum) was applied for defect  composition analysis.


Fig.2 Au bump schematics


Results and Discussions


Nodule defects can be observed on the top of eutectic bump  surface, as shown in Fig.3. From this image, we found that  nodules grow mainly on the edge of bump.


Ti/W


UBM


## Microstructure Analysis of Wafer Bump Nodule


115


Fig.3 SEM Image of eutectic wafer bump with nodular defects. T type of mushroom-like bump is normal and the F type one is abnormal. Arrow symbolized the direction of FIB milling.


Fig.4 SEM image of deformed bump; PbSn-1 layer has a bulge and UBM voids exists; PbSn-2 layer has no thickness  difference on each site.


Fig5. FIB image on the bottom of eutectic bump nodule. Voids are observed in solder PbSn-1 layer and UBM layer; Photo resist (PR) profile is not vertical.


Fig.6 FIB image of the bottom of bump without nodule, no  void is observed in the solder and UBM, PR profile is normal.


Figure 4 shows the SEM image of microstructure of deformed  bump with nodule. From the image, there is no thickness  difference on each site of PbSn-2 layer. So it can be concluded  that the nodule occurs on PbSn-1 layer if there is no other  defect-introduced issue at the UBM deposition steps. The  bottom of bump both on nodule and on no-nodule was also  analyzed by FIB imaging. Fig.5 shows that there are some  voids in both solder and UBM beneath the nodule. But on no  nodule site, the UBM and bump cross-section profile is  normal, as shown in Fig.6. The results conclusively confirm  the previous phenomena observed on bump surface that  nodule grows only on specific location where bump suffers


from void defects or poor PR opening. From Fig. 5, PR sidewall is not vertical, which is the one of the possible reasons for nodule formation.


Fig. 7 EDS-point analysis result of the particle in Au bump  nodule shown in Fig. 8. An abnormal element of Silicon was  detected.


The mechanism of nodule growth in Au bump was also  analyzed. Figure 8 shows grain structure of the Au bump. We  found radiation-like grains distributing around an embedded  particle. In normal sample, however, grains appear to be flaky  stack, as shown in Fig.9. From the EDS-point result (shown in  Fig.7), silicon signal illustrates that the particle is siliconcontained material. Figure 10 (a) shows the normal electrocrystallization and (b) illustrates radiation-like grain structure  formation when there are some particles attacking. Usually, Silicon contained residue falls from the inner walls of Eplating solution tank set. Or tank suffers contamination issue  because of some other abnormal operation procedures.


Fig.8 FIB image of Au bump nodular microstructure with  eradiation-like grains around the Si contained particle


Fig.9 FIB image of normal Au bump microstructure with  flake-like grains stacks.


(a)                                               (b)


Fig.10 Wafer Bump growth model (a) normal E-plating  growth model; (b) bump growth with particle attacking


Particle attacking increases nucleation numbers, which  accelerate electro-crystallization rate if there is no other


PbSn-2 PbSn-1 UBM


Void


Particle


Packaging Material has contributed to high Idd_Pd failures in CMOS ICs


Pun Meng Chi, Chew Gim Eng, Nazita Sulaiman


Avago Technologies (Mal) Sdn. Bhd.,Bayan Lepas Free Industrial Zone , Penang, Malaysia


An aggressive yield improvement program that  was undertaken by the engineering teams has culminated  in the works reported in this paper.  The power down  current (Idd_Pd) was one of the major failure modes   recorded for CMOS ICs. In essence, any improvement  made on the Idd_Pd test yield will inadvertently result in  substantial gain in terms of cost and production capacity. A taskforce to resolve high fallouts for the Idd_Pd was  then formed back in the year 2004. This taskforce  comprised of members from various engineering teams, for instance, Manufacturing, IC Design, Materials and  Failure Analysis (FA).  The length of investigation to  resolve the complex high Idd_Pd failures had spanned  over a period of a year. The team had devised a  comprehensive sets of DOEs (Design of Experiments) which were conducted at various contract manufacturing  facilities where the ICs were packaged. Results obtained  from these DOEs had conclusively pointed to molded  materials as the major factor contributing to high Idd_Pd  yield loss. Armed with this vital information, FA had  performed an indepth electrical diagnosis as well as  physical analysis on the molded materials. The analysis  results had confirmed contamination of the molding  materials by conductive carbonized resin as the cause of  high leakage current in ICs. Likewise, the material  supplier had found minute contamination in the resin  melt.


In essence, Idd_Pds that were measured in the  range of tens of microamps to thousands of microamps  in ICs could be largely attributed to leakages caused by  carbonized resin in the molded materials.


1.0. Introduction


The IC has various operating modes. One of the  operating modes, namely power down mode (PD mode), operates at low current to reduce the power consumption  of the device. In the power down mode, all blocks are  disabled except for the regulator block, which is required  to maintain the state of device.  The power down mode is  critical, especially for wireless products, which rely on  batteries for its operation. The duration between batteries  change is greatly influenced by this parameter. Thus, electrical testers are used to screen this parameter, Idd_Pd, which is the current consumption of the device  when in power down mode.


The Idd_Pd test measures the  current consumption of  the input supply voltage when in power down mode.


Main contributors to the Idd_Pd current are the voltage  regulator, supply leakage current and etc.


2.0 Rootcause Investigation


Mechanisms for high Idd_Pd in Navigation ICs could be  categorized into 3 areas:


1. Tester Related


Shift of tester measuring equipment. This factor has been  ruled out through calibration of tester equipment.


2. IC Related


Shift of process towards higher consumption devices, which are the faster speed devices. From the distribution  plot of wafer process parameter of the affected lots, no  shift was detected.


Cracks in dielectric layers causing higher leakage. The  failure analysis performed on units showing high Idd_Pd  did not detect abnormality of this nature.


Higher leakage caused by conductive material lodged  between supply voltage and ground. The failure analysis  performed on units showing high Idd_Pd did not detect  abnormality of this nature.


3. Package Related


Bad connection  at PD pin causing device to be in non  power down mode. This factor has been ruled out due to  good O/S test result on PD pin.


Higher leakage caused by conductive material lodged  between supply voltage and ground. This  was proven to  be the mechanism for high Idd_Pd.  The following  section  illustrated the design of experiments that were  carried out to arrive at this conclusion


## Packaging Material has contributed to high Idd_Pd failures in CMOS ICs


118


3. 0 Design Of Experiments


Numerous critical factors were considered when the  DOEs were devised (Please refer to the attached  fishbone diagram). The factors investigated including the  various subcon sites, die attach process as well as   different molding materials suppliers.


3.1 1st.Factor: Contract manufacturing sites related


Method : Wafers from same lot were assembled in Site P & Site T


Result :  Site T builds produced higher  Idd_Pd fallouts


Sub Con


Site T


Site P


Wafer Lot


Same


# of wafers


Test Yield


81.7%


92.9%


DC Fallout


13.7%


3.5%


Table1


Conclusion :  Site T’s assembly produced higher Idd_Pd  failures


3.2 2nd Factor :  Identify the affected  process stations


Method : Wafers from the same wafer lot assembled  with a combination of  process flows in  Site P & Site T   Result: DA process at Site T recorded low yield due to   high Idd_Pd failures


Process


C M


SS


IddPd%


Remark


1a Grind & Saw


DA  Test


T1  T


11.14%


Ctl lot


1b Grind & Saw


DA  DA  Cure


WB  Test


T1  T P


8.94% Eval   lot


2a Grind & Saw


P P


0.89% Ctl  Lot


2b Grind & Saw


P T T


6.51% Eval   Lot


Table2


Conclusion :  Molded materials  from different sources  were suspected to be the cause of Idd_Pd.


3.3


3rd.Factor : Identify molded materials from  different sources


Method : Build wafers from same wafer lot using  molded materials  from different sources at Site T & Site  P.


Result : Lots that were assembled using molded  materials from supplier A recorded low yield due to high  Idd_Pd fallouts


L/F


Supplier


CM


IddPd (%)


1 wafer


10.48


0.73


0.36


6.18


9.33


Table 3


ENVIRONMEN


MATERIALS


AND


Lint Free paper


IddPd


MACHINE & METHOD  Wafer packaging method


FOL Processes  MANWafer handling/transferring


ESD


Clean room environment


Different CM site


Different molders


Wafer backgrinding to  mounting


IC


Molded material suppliers vs CM built


0 2 4 6 8 10 12


A_T


A_T1


A_P


B_T


C_T


Supplier VS CM


Graph1


Conclusion : Molded materials from supplier A was the  main factor contributing to high  Idd_Pd failures


4.0 Analysis of ICs failing high Idd_Pd


4.1


Generic analysis flow for Idd_Pd failures:


Step1: Bench verification using 4156B parametric  analyzer on all pins


Step2: Power down the sensor using a control board  and power supply. Monitor the Idd current with a digital  multimeter


Step3: Fault localization using Photon Emission  Microscope or liquid crystal


Step4: Deprocess the IC for physical defect  identification


4.2


Signatures of  ICs failing  the Idd_Pd parameter  due to packaging material


Leakages due to packaging material would produce  consistent photon emission patterns on the IC (please  refer to Fig.1). Additionally, bench testing performs on  all pins using the 4156B parametric analyzer would  typically fail to detect any leakages or short.


Deprocessing performs on the IC  would not uncover  any physical defects on the emission locations.


Fig.1: Overlay image of the IC which was produced by  photon emission microscope. 2 emisison locations were  spotted.


4.3   Implement new analysis flow for Idd_Pd  failures


4.3.1 Bench testing would be performed on the  Idd_Pd failures at ambient and hot conditions for all  pins, for instance pin to pin, pin to ground and pin to  Vdd.  Leakages were noted on some pins during hot  test. Ironically, magnitude of the leakage would  increase substantially when some of these pins are  shaked vigorously (Fig.2). The above tests would be  repeated after the ICs are isolated from the packages  by removing all the gold interconnects.  Resistive  shorts would be observed on the fail pins under hot


est (Fig.3) for packaging related failures.


Fig.2: Electrical characteristic of a pin displaying  leakage after hot test. The characteristic of a good pin  was appended for comparison


Bad pin


Good pin


Fig.3:  Resistive shorts were measured on the failed  leads / pins after the gold interconnects were  removed.


4.3.2 Optical and electron beam microscopes were  the instruments used for visual examination. Black  substances were observed on the mold compound  between the affected leadframes of Idd_Pd failures.


(a) 25X Mag


(b) 50X Mag


(c) 100X Mag


(d) 100X Mag


Fig.4: Optical micrographs depicting the failure  locations where the leadframes appeared to be shorted / bridged by some black foreign materials


Fig.6: (a) and (b) were SEM micrographs depicting the  black foreign materials at different magnifications


4.3.3 Chemical analysis that was carried out on the black  foreign materials included:


SEM-EDX and Quantitative analysis


Micro-FTIR analysis


Element


Weight% Atomic%


C K


67.03


75.43


O K


28.73


24.27


Au M


4.24


0.29


Totals


100.00


Fig.7: EDX quantitative analysis has revealed Carbon as  the primary element in the composition of the black  material. The specimen was coated with Au element in  order to prevent charging.


Fig.8: (a) Micro-FTIR analysis of the black materials. Spectrum of Graphite was appended for comparison. (b) Micro-FTIR spectrum of the LCP material (mold  compound).  The analysis results have  established that  these black materials did not contain polymeric   structure.


5.0 Root Cause Investigation


Black foreign materials that were found between the  shorted leadframes were not chemicals from the LCP (liquid crystal polymer) used for  molding.  This fact was  confirmed by the Micro-FTIR analysis result (please  refer to Fig.8)


These materials contained high percentage of Carbon, appeared flat, shiny and compressed. Thus, conductive  carbon flakes were suspected to be the likely source.


The source of carbon was traced to the resin materials, LCP (Liquid crystal polymer) used in molding.


Two possibilities were investigated initially:


Original resin materials


Foreign introduction at molder’s location


Graphite


Black


LCP


Foreign introduction was ruled out after a thorough  investigation was conducted at molder’s site.  Purging of  the molding machine with PMMA at 360  -380 deg C  has successfully isolated a couple of machines which  were consistently producing contaminated purge blobs. These purge blobs contained black flakes which were  mildly conductive.  The injection screw from these  machines were then removed and examined.  It was  discovered that black compounds were deposited onto  the parts of the screw that have worn out.


These black compounds were suspected to be some kind  of “carbonized resin”.


What is“Carbonized resin”


All polymer materials are Hydrocarbon, made primarily  of 3 elements: “ Carbon”, “ Hydrogen” and “Oxygen”. In polymeric materials, these elements form long chains  or molecules and when synthesized with other elements, say “Fluorine”, “Sulphur” or other base metals will  create the modern plastics we use today. Under certain  conditions, repeated heating, exposure to high  temperature or UV lights, these molecules degrade or  degenerate into their basic elements: Carbon, Hydrogen  or Oxygen. In an injection molding process, this process  takes place all the time, but in minute quantities that are  too insignificant to effect the generic properties of the  molded product. However, when the melt in a processing  barrel retains materials for too long, these polymer will  degenerate and deposit these elements on the screw or  internal surfaces. Carbon will be deposited while  Hydrogen and Oxygen will vapourise and enter the  atmosphere as volatiles.


What could have happened


The defective screw, with the chipped flights was  deposited with the carbon which was formed when the  polymer melt had been trapped and repeatedly heated  over the production cycles.


Fig.9


Fig.10: These fragments were found to be conductive  with a  multimeter


Fig.11: Purged materials (PMMA) from the molding  machine


Carbon trapped by the injection screw could precipitate  onto the leadframes during the molding process, hence  causing minor leakage / short on the affected location / s.


6.0 Discussion


How carbon conducts electricity? Every carbon atom  essentially contains six negatively charged electrons. Two electrons reside in the inner shell, and this shell can  only contain two electrons, so it is full. Carbon atoms  have four outer,valence electrons in their next shell. This  outer electron shell can hold eight electrons, and atoms  in general are much more stable when their outer shell is  full. To obtain a full outer shell, carbon atoms form four  covalent bonds with other atoms. A covalent bond is   formed when two atoms share a pair of electrons. Carbon  atoms can bond together in chains, rings and meshlike  networks. In diamond, each carbon atom bonds  tetrahedrally to four other carbon atoms to form three  dimensional lattice. The shared electron pairs are held  tightly in sigma bonds between adjacent atoms.


Pure diamond is an electrical insulator – it does not  conduct electric current. It is colorless and hard.


Graphite is black and slippery and conducts electricity. In graphite, the atoms form planar,  or flat layers. Each  layer is made up of rings containing six carbon atoms. The rings are linked to each other in a structure that  resembles the hexagonal mesh of chicken wire. Each  atom has three sigma bonds and belongs to three  neighbouring rings. The fourth electron of each atom  becomes part of an extensive pi bond system. Graphite  conducts electricity, because the electrons in the pi bond  system can move around throughout the graphite.


7.0 Conclusions


Proactive steps were implemented at the molder’s site to  prevent a recurrence of similar problem. The measures  taken included: (1) More frequent preventive  maintenance (PM) performs  on the injection molding  machine (2) An additional gate was put in place to  buy  off the molded materials prior to shipment. A multimeter  and 20X magnification low power optical scope are the  instruments installed at this station.


Additionally, the procedures on how to verify such  failures has been proliferated to the labs at contract  manufacturers’ sites in order  to buy off low yield trigger  lots before they are being released by production.


8.0 Acknowledgments


The authors wish to acknowledge the following for their  knowledge, material and resource contribution to this  paper


1. Koay Ban Kuan, Noorazidi Azib, Cheah Chiang  Sun, Yeoh Chin Heong and Seow Chin Seang –  DOE design and process guidelines


2. Lim Swee Hong, Ang Siew May – Testing and  Analysis


9.0 References


1. Organic Chemistry. Fifth Edition. Robert  Thornton Morrison and Robert Neilson Boyd, New York University


2. Handbook of  Polymers in Electronics. B.D. Malhotra


3. Conductive Polymers and Plastics. Larry  Rupprecht, Editor


Inductive Operating Life Stress Metal Breakdown Mechanism


Bruce Gillette


Fairchild Semiconductor Corp, Mountaintop, Pennsylvania, USA  Bruce.Gillette@fairchildsemi.com


Experimental devices in a deteriorated state were encountered  after 168 hours of inductive operating life stress, (IOL) testing.  A metal grain boundary breakdown mechanism was  found during the analysis of the device, which was creating a  low resistance current path between terminals.  The AlSiCu  top metal was breaking down along the grain boundaries.  In  addition there was alloying of the Aluminum into the  underlying silicon.  This alloying was creating a short to the  gate, source, and drain.  Several variations in the metal stack, testing conditions, number, and dimensions of bond wires die  size and mold compound were evaluated to better understand  the cause of the inability to withstand IOL stress and to  provide a process solution.  The prevention of the AlSiCu  front metal grain boundary breakdown during inductive life  stress testing required a die size, bond wire dimension, and  testing condition change to meet the performance  specification.  This change resulted in a reduced grain  boundary breakdown and consequently prevented Al grain  boundary breakdown, TiW barrier breakdown, and Al alloy  spiking.  The die change and modified testing conditions  resulted in a successful pass through the IOL stress testing.


New product designs, process improvements, application  requirements, and materials changes may have an impact on  device reliability.  These changes can trigger new mechanisms  which degrade device function after being exposed to stress.  For successful product release, these mechanisms need to be  understood and prevented.  For example, metal grain  boundary breakdown can be very detrimental to a  semiconductor’s performance and reliability.  In particular, a  key parameter, the device’s on resistance and functionality, may be deeply modified by the breakdown of front (source) metal film grain boundaries.  Biased Inductive Life Stress test  is a reliability test of a semiconductor device’s ability to  absorb inductive energy.  Inductive Operating Life Stress  samples are subjected to repetitive energy spikes to uncover  weaknesses such as the ability to absorb inductive energy, gate oxide integrity, Safe Operating Area (SOA), Unclamped  Inductive Switching (UIS) issues, and bondwire and  metallization breakdown.


The typical source metallization used is an alloy of Al, usually  Al Si-1% Cu-0.5% (wt %) (Al(Si)(Cu)).  Al grain boundary  breakdown during inductive operating life stress testing can  result in intergranular isolation, source bondwire deterioration, and transistor structure destruction.  Industry wide, inductive  operating life stress deterioration mechanisms are typically as  a result of the breakdown of the source metal, gate oxide  breakdown, or SOA/UIS issues.  This paper will discuss a  combination of typical Inductive operating life metal  breakdown mechanisms, an investigation of their causes, and  solution to prevent the failure.


Device Analysis


Background: Biased inductive operating life stress caused  deterioration of experimental devices. The inductive operating  life stress test conditions were as follows: 168 Hour @ 27mJ, 2mH, 5A, 50Hz, 130C case temperature mounted in socket  using inductive life testing equipment. The standard source  metalization used is a stack consisting of Ti/TiW/Al(Si)(Cu).


Electrical Testing Results: The gate to source leakage (Igss) on the deteriorated devices was grossly shorted.  Drain to  source leakage (Idss) was also grossly shorted.


Electrical Analysis: The low resistance current path between  terminals suggests an Electrical Over Stress (EOS) type event. After baking the degraded devices at 100C for 2 hrs all units  were still gross shorts. This indicates it is not a moisture  related mechanism.  After 150C bake for 24hrs all units were  still grossly shorted between all terminals. This indicates it is  not Li+, Na+, K+ mobile ionic contamination mechanism.


Acoustic Package Inspection: The packages were analyzed  using an acoustic microscope (C-SAM) to determine if there  was a significant delamination after IOL Stress testing (Figure  1).  All units from the stressed test had good die to mold  compound and mold compound to header adhesion.


## Inductive Operating Life Stress Metal Breakdown Mechanism


125


Figure 1: C-SAM image of a unit in a deteriorated state, on  Inductive Operating Life Stress, showing no mold compound to die delamination.


Real Time X-Ray Package Inspection: The packages were  analyzed using an real time X-ray to determine if there was  bonding or die attach issues after IOL Stress testing (Figure 2). All units had no wire anomaly on Au wires. No voids mold/die attach and no package anomalies on any unit.


Figure 2: X-Ray photo of a die in a deteriorated state, note the  Al bondwire’s are not visible in X-Ray, with minor solder voids


Physical Analysis: The failing devices were decapsulated  using a jet etcher decapsulation tool.  All of the deteriorated  units had grain boundary breakdown of the top metal along the Al grain boundaries as well as Al grain boundary breakdown under the passivation. The passing test units also displayed varying degrees of Al grain boundary breakdown,the attached adjacent die that was not stressed, did not have Al  grain boundary breakdown (Figure 3).


Figure 3: SEM image of source metal showing severe granular breakdown on the left stressed die and no granular breakdown  on the right unstressed die.


The areas with the greatest grain boundary breakdown were  the source pads; (Figure 4) the gate pads did not have an issue(Figure 5).


Figure 4: Optical photo of Al grain boundary breakdown on the die on the left, the die on the right side is unstressed.


The Al grain boundary breakdown was severe, reaching down  to the Si surface (Figures 6). The on-state resistance of the  device was severely affected as each Al grain became increasingly isolated from the others and only maintained contact through the TiW barrier metal and the Al bondwires.


Figure 5: Optical image of the gate pad with no granular breakdown.


Figure 6: SEM/FIB cross section image of AlSiCu showing severe granular breakdown.


When the devices were decapsulated the Al bond wires either detached from the decapsulation procedure or detached when  touched with tweezers. The pure Al bond wires where subject  to Dispersive X-ray (EDX) analysis to determine if any contamination or other elements were present at the point of detach.   Results showed a peak of Silicon in the bondwire. The bond wire where also EDX analyzed for contamination,the analysis showed no Br/Na/Ba contamination on all IOL stressed units and Epoxy Mold Compound (EMC) area. This would indicate that alloying of the Al from the bondwire/top metal into the silicon and the silicon into the bondwire/top  metal had taken place.  (Figure 7, 8, 9, 10)


Fault Isolation: After chemical decapsulation the devices where hot spotted, which revealed pin point leakage sites at the source bondwires for both Igss, and Idss leakage.


Figure 7: SEM image of the detached Al bondwire, with alloy pitting, and Al grain boundary breakdown on the bonding pad.


A cross-section of a partially detached bondwire was preformed. Sever alloying of the Al into the silicon was observed. (Figure 9 & 10)


Figure 8: SEM of the source bondwire that detached after decapsulation.


Figure 9: Cross-section optical image of Al alloying into the silicon.


Figure 10: SEM Cross section of Al bondwire with metal alloying into the silicon.


Compositional Analysis: Differences in the grain boundary  breakdown behavior films were investigated, and one theory  discussed was that the granular breakdown was due to micro  aluminum casting hydrogen assisted embrittlement.  This  would be a moisture assisted event. To determine the  condition of the bond pads, a depth-sensitive X-Ray  Photoelectron Spectroscopy (XPS), also known as an Electron  Spectroscopy for Chemical Analysis (ESCA), on the source  bond pad was chosen for the analysis. The presence of  contaminants on both a stressed and an unstressed pad would  be analyzed. Also a sense of the surface oxide thickness  would be analyzed, with the idea that a thick hydrated oxide  on the stressed bond pad would confirm that high moisture  content is partially at fault. Die were sent to Lehigh University  with the following results: The research scientist in charge of  the XPS system manually broke away the mold compound to  allow unobstructed access to the die surfaces, and then  perform a set of scans. On the stressed side of the die, they  took surface data from a sequence of location across the pad. Each sampled area was approximately 300um x 80um. The  areas started at open surface on one side of the bond location, moving across the region with the failed bonds, and on to the  other open side.  Of these scans, all were uniform with the  exception of the scan that overlapped the bond that detached. The operator also performed a similar surface scan on an open  region of the unstressed pad. This differed in several minor  ways with the scans on the stressed side. The clear areas of the  stressed die showed strong surface signals of Al2O3 and SiO2.


The presence of each was not surprising, but the thickness of  the Al2O3 (greater than 7.5nm) is greater then the native  alumina (2-3nm). The silica signal was also higher than  expected for an alloy with low Si content since Si is not a  strong surface segregant in aluminum. Other peaks indicated  the presence of a 5-6 nm thick hydrocarbon layer (C-H bonds) and two types of nitrogen: oxidized (weakly associated with  the hydrocarbon) and organic nitrogen (bonded with carbon). This implies that there is a thin coating or patches of a  nitrogen-bearing polymer present. The area in which the wires  where previously attached show a similar signature, but with a


strong metallic (i.e., not oxidized) Si peak that probably comes from the bottom of the debonded regions. There are  less of the hydrocarbon and nitrogen signatures, probably because the surface was removed when the bonds failed. The  unstressed die also shows a thick alumina and silica layer. A lower hydrocarbon signature was present, and no oxidized nitrogen (consistent). This might imply that some of the hydrocarbon was created during the stressing process, but this was not conclusive. There were no signatures from elements such as chlorine that would act as aluminum corrosives. However, it is often the case in aluminum alloys that salt  corrosion does not leave a chlorine signature behind. So  chlorine can’t be rule out as a role in the failure process, nor does the analysis point to any other obvious agent. (Ref 6) After reviewing the Lehigh report the resident Chemist commented:  The hydrocarbon that he is seeing might be the mold compound, which is just a polymer. It is possible to get a reaction of some sort occurring between the mold compound and the surface of the metal.  He seems to imply this, because the unstressed die has a lower signature of the hydrocarbon.


The current dump on the stressed part could add enough energy to push reaction along.


FA Conclusions: All devices in a deteriorated state show  severe degradation of the front metal Aluminum caused by high temperature high power dissipation. Junction temperatures were extreme enough to breakdown the barrier metal allowing the Aluminum to migrate into the silicon eventually developing a short. Silicon migrating into the bond  wires causing the bond wires to lift following decapsulation of  the package was all so observed. Temperature’s for  breakdown of the barrier metal need to be approximant 400C.


This is occurring at very, localized regions under the bond wires. Projected sequence of events is high peak junction temperatures with insufficient thermal cool down period,causing degradation of the aluminum grain boundaries,forming regions of very, localized current under the bond wires producing ever higher temperatures until degradation of  the barrier metal and eventual shorting of the device due to silicon spiking.


Stress Conditions Experiment: To analyze the impact the stress conditions had on the devices in a deteriorated state an  experiment changing the inductor and energy was run.


IOL Test Condition A: Experimental devices were placed on IOL stress, with the following test conditions, 5mH, 30mj,50Hz; with the following results. Devices were decapsulated. Optical inspection of the stressed device’s after 168 hours showed severe source metal cracking/voiding and a dark  contrast in color from the adjacent unstressed channel. Two of  the (die #A01, #A02) opened devices were then placed backup on IOL stress. The stress site was changed to the previous unstressed sister die. Once again the 168 hour inspection showed similar results (i.e. source metal cracking/voiding and  a darken color.


IOL Test Condition B: Experimental devices were placed on  IOL stress, with the following test conditions, 5mH, 15mj,50Hz; with the following results. Devices were decapsulated. Optical inspection of the stressed devices after 168 hours showed no apparent signs of source metal cracking/voiding or darkened color on two (die #B01,#B02) of the three devices.


However, one device (die #B05) did show the presence of severe source metal cracking/voiding and a dark contrast in color. Once again the three decapsulated devices were placed  back-up on IOL test, however the stress site for die #B05 was changed to the previous unstressed sister die. The devices were inspected again after an addition 168 hours (total= 336 hours). Optical inspection of die #B01 showed no apparent signs of source metal degradation; however, die #B02 does appear, in small areas on the source metal, to show the onset of this metal cracking/voiding and darkening metal phenomenon. Die #B05 again showed severe source metal degradation after being stressed for 168 hours.


IOL Test Condition C: Experimental devices were placed on IOL stress, with the following test conditions, 10mH, 15mj,50Hz; with the following results. Devices were decapsulated. Optical inspection of the stressed devices after 264 hours showed no apparent signs of the presence of either source  metal cracking/voiding or darkening in color.


IOL Test Condition D: Experimental devices were placed on IOL stress, with the following test conditions, 10mH, 100mJ,10Hz with the following results. Devices were decapsulated. Optical inspection of the stressed devices after 264 hours showed no apparent signs of the presence of either source  metal cracking/voiding or darkening in color.


IOL Test Condition E: (Control):  Experimental devices were placed on IOL stress, with the following test conditions,2mH, 27mj, 50Hz; with the following results. Devices were  decapsulated. Optical inspection of the stressed device’s after  168 hours showed severe source metal cracking/voiding and a dark contrast in color from the adjacent unstressed channel.


Table 1: Test Condition Results  Test


Cell


Test-Cell


Description


Properties


5mH, 30mJ, 50Hz Different IOL  Test Conditions


failed


B 5mH, 15mJ, 50 Hz Different IOL  Test Conditions


C 10mH, 15mJ, 50 Hz Different IOL  Test Conditions


passed


10mH,


100mJ,


10Hz


Different IOL  Test Conditions


2mH, 27mJ, 50Hz Control (failed  IOL)


Bond Wire Experiment: Experiment was run to assess the  number of Aluminum bonds (5 mil. each) and its effect on the  devices Aluminum cracking phenomenon. Units with two 5


mil bondwires, and three 5 mil bondwire where placed on IOL stress. After 40 Hr the devices where taken off stress and  decapsulated with the following results: Visual analysis using  an optical microscope of the stressed die revealed no  significant differences between 2 or 3 bondwire connection;metal degradation and discoloration was seen on both. Under  higher magnification visible cracking of the source metal is evident. The metal is clearly degraded. Again no significant differences between 2 or 3 bondwire connection observed.


Another experiment was run to assess the diameter of the Aluminum bonds (5mil vs. 8mil). Units with two 5mil bondwire and two 8 mil bondwire where placed on IOL stress, after 40 Hr the devise where taken off stress and decapsulated  with the following results. Visual analysis using an optical microscope of the stressed die revealed a difference with the  bondwire diameter. The die with two 8 mil bondwires shows an improvement of the Aluminum grain boundary.


Top Metal Film Experiment: Experiment was run to assess  the effect of different top metal films on the devices Aluminum cracking phenomenon. Die with a Ti overcoat over  the AlSiCu where placed on IOL stress. This experiment would strengthen and protect the Al top metal from the hydrogen assisted embrittlement theory, with the following results. After 24 hours devices show signs of severe source  metal cracking/voiding and dark contrast in color from the adjacent unstressed channel. This was the first time this type  of experimental metal film stack was tried, and due to resource constraints the optimized process might not have been found.


Die Size Experiment: Simulation was done on a larger die and could pass a 6A, 100mJ, Inductive Operating Life Test at 10Hz rep. rate and JC 16°C/W and 11°C/W respectfully.


Thermal resistance was scaled based on total die area difference.


Current die size IOL test conditions: ID=6A, VG=5V,


VDD=14V, Vclamp=30V, Rg=10k , Rclamp=17k ,


Tjstart=25°C, Freq. =10Hz, Eclamp=102mJ, L=2.96mH,


tclp=1.18msec


0.020


0.040


0.060


0.080


0.100


Time (sec)


Peak Tj


Backside of Die Temperature


IC VDS


Vg (internal)251°C


Larger die size IOL test conditions:


ID=6A, VG=5V, VDD=14V, Vclamp=30V, Rg=10k ,Rclamp=17k , Tjstart=25°C, Freq. =10Hz, Eclamp=102mJ,L=2.96mH, tclp=1.14msec


Conclusions for Simulated IOL stress:


1. Based on this study the 100mJ, 6A, 10Hz condition  on both die sizes with the thermal resistance used the  peak temperature returns to the starting Tj after every  rep.  This test simulates the number of times the


device can withstand a single pulse event.


2. The Peak temperature delta from the starting Tj for


the small die is 226°C and for larger die is 135°C.


3. If the starting Tj is 150°C, this means the Peak Tj


during the clamping would be 376°C for the small


die and 285°C for the small die.


Experiment was then run to assess the effect of a different die size on the devices Aluminum cracking phenomenon. Devices were placed on IOL stress with the following results. Devices  were decapsulated. Optical inspection of the stressed devices after 500 hours showed no apparent signs of the presence of  either source metal grain boundary breakdown/voiding or  darkening of color to the surface of the stressed die.


Verification of experiments:


Three experimental test lots, with a larger die size, two 8 mil Al source bondwires, and IOL stress conditions of 100mJ, 6A,10Hz were reliability tested on the Inductive Operating Life stress. All three lots passed with out any metal grain boundary breakdown, Igss, Idss or RDSon shifts.


Final Conclusions:


The severe degradation of the AlSiCu top metal was caused by high temperature high power dissipation. Junction temperatures were extreme enough to breakdown the barrier metal allowing the Aluminum to migrate into the silicon,eventually developing an electrical short. Silicon migrating


into the bond wires causing the bond wires to lift following decapsulation of the package. Temperatures for breakdown of the barrier metal must be to be in excess of 400C. This occurred at very, localized regions under the bond wires.


Sequence of events was high peak junction temperatures with insufficient thermal cool down period, causing degradation of  the aluminum grain boundaries, forming regions of very,localized current under the bond wires producing ever higher temperatures until degradation of the barrier metal and eventual shorting of the device due to silicon spiking.


The current die size and bondwires diameter was insufficient in its current configuration. Several process solutions were  investigated to increase the robustness of the product. A  change from a small die size to a larger size and from a  smaller diameter bondwire to a larger diameter allowed sufficient thermal cool down period, preventing the metal grain boundary from breaking down, and resulted in a reliable process.


Metal grain boundary breakdown induced leakages are not new mechanism to the Inductive Operating Life stress. New  technologies, designs, new packaging materials, application requirements, and process changes can alter the signatures of these old mechanisms, making it harder to isolate the cause. Identifying and understanding these unique signatures leads to a better preventative solution which in turn produces a more robust product over time.


1. Rodney R. Stoltenburg, “Boundary of PowerMOSFET, Unclamped Inductive-Switching (UIS)Avalanche-Current Capability”, Proc. 1989  Applied Power Electronics Conference, pp 359-364, March 1989.


2. Application Note March 2002 AN-7515 (AN9322) Fairchild Semiconductor, A Combined Single Pulse and Repetitive UIS Rating System, pp 1-4


3. Applications Note AN10273_1 Philips Semiconductor, Power MOSFET Single-Shot and Repetitive Avalanche Ruggedness Rating, pp 2-4


4. Anthony F. J. Murray, Tim McDonald, Harold Davis, Joe Cao, Kyle Spring, Extremely Rugged MOSFET Technology with Ultra-Low Rds(on)Specified for A broad Range of EAR Conditions, PCIM 2000, IR UIS pp 4-8


5. D.L. Burgess, O.D. Trapp, Failure & Yield  Analysis Handbook 1992, Failure Examples,Overheating pp 5.11


6. Richard P. Vinci, Private Correspondence, Lehigh  University Analysis Report, pp 1,2


Vg (internal)161°C


Acknowledgment


The author would like to thank Lehigh University  Industrial Liaison program, Associate Professor of  Material Science and Engineering at Whitaker  Laboratory, Richard P. Vinci


The author would like to thank Ron Feiller as well as the   Device Concepts and Technology Development Teams, Global Operation Teams, Product Line Design Teams, and  Packaging Research and Development Teams for there  support and help.


Root Cause finding of a Diode Leakage Failure using Scanning Magnetic  Microscopy and ToF-SIMS as Key Methods


H. Preu, W. Mack, T. Kilger, B. Seidl, J. Walter, P. Alpern, M. Kirchberger


Infineon Technologies AG, Regensburg, Germany


One challenge in failure analysis of microelectronic devices is  the localization and root cause finding of leakage currents in passives. In this case study we present a successful approach for failure analysis of a diode leakage failure.


An analytical flow will be introduced, which contains standard  techniques as well as SQUID (superconducting quantum interference device) scanning magnetic microscopy and ToFSIMS as key methods for localization and root cause identification. [1]


The electrical failure occurred predominantly in consumer electronics used under certain climatic conditions. These climatic conditions were well reflected by a so called “SMT application test” (device soldered on test board; 35°C/ 95% rh  and 30V reverse bias, 21days). The proportion of the fail samples was in the range of a few percent.


After applying the SMT application test for 10-15 days a leakage current of 100μA to 1000μA was found under 30V reverse bias. The leakage could be sometimes recovered by drying the device on the test board. Thus, moisture and temperature had a major influence on the electrical behavior.


Location of the leakage current with sufficient spatial resolution is essential for subsequent sample preparation and further physical analysis in order to find the root cause. The main analysis steps will be presented as follows.


Experimental and Results


Several alternative paths for the leakage current exist (cf.


Fig. 1):


• through wire bond and the die


• through the mold compound (bulk)


• on mold compound surface (conductive contamination or residues)


• on test board PCB (conductive contamination or residues)To distinguish this various alternatives, SQUID scanning magnetic microscopy (Magma C20) was used which has the necessary spatial resolution [2-4]. To maintain the humidity in  the package and to avoid drying after the SMT application test, the failed devices were stored in a sealed box together with humid tissues prior to the SQUID measurement. For the SQUID measurement assembled diodes were used and operated with 30V reverse bias. The SQUID-analysis revealed  that the leakage current flows through the gold wire and therefore either through the die or along its surface but not on the package surface, the test board or through the mold compound bulk (cf. Fig. 2).


This could be confirmed by a further SQUID measurement at a resin embedded cross section of the device. With careful preparation and final ion beam polishing [5] any potential conductive contamination was removed from the cross section surface prior to the measurement. Fig. 3 shows how the leads in the cross section were contacted by means of conductive glue which then was contacted with the tips. In principal,sectioning of a diode does not destroy its basic electrical function due to its symmetrical design. Therefore SQUID analysis is also applicable in this particular case with a sectioned device. The diode was operated with -30V under reverse bias and currents in the range of 20μA were measured.


Figure 2: The bright shining symbolizes a high current density which can be attributed to the gold wire.


Figure 1: Cross section through the diode package.


## Root Cause finding of a Diode Leakage Failure using Scanning Magnetic Microscopy and ToF-SIMS as Key Methods


132


The resulting current density image is shown in Fig. 4. This


analysis clearly shows that the source of the failure must be


near the chip surface.


In a further preparation, fail samples were chemically decapsulated. Fig. 5 shows a detail of the chip surface after removing the mold compound. The only noticeable structure which was found is marked on the right hand side of Fig. 5.


By elemental analysis using SEM/EDX, aluminum and oxygen were detected at the suspicious structure indicating a potential presence of aluminum-hydroxide as a product of a corrosive reaction (cf. Fig. 6).


Figure 6: EDX mappings of the suspicious guard ring region. The arrows indicate the corrosion (aluminum oxide or


aluminum hydroxide).


Figure 4: Cross section of the diode package and


analysis result.


Figure 5: Detail of the chip surface after wet chemical decapsulation of a failed sample.


Figure 3: Cross section of the diode with electrical contacts and under the SQUID probe.


SEM


Si


Al-Guard ring Isolating SiN Passivation


Al-Pad


Additionally, we found in further resin embedded cross sections of failed samples corroded aluminum metallizations(guard ring around wire bond pad, cf. Fig. 7).


At that time, it was possible to explain the electrical failure with corrosion of aluminum to aluminum-hydroxide which leads under the presence of moisture to an increased conductivity.


To find the intrinsic reason for the corrosion it was essential to  avoid artifacts caused by wet grinding or chemical decapsulation during sample preparation. Especially the identification of corrosive elements should not be affected by any mechanical preparation.


Based on this, in a further step, a FIB preparation was initiated  with the aim to hit the corroded area. This required some pretreatment for FIB-navigation. After thinning the chip thickness  of a fail sample from the chip backside (Fig. 8), additional hints for contamination or corrosion at the guard ring region of  the chip surface were detected with IR-microscopy.


The device was then re-embedded to grind down the mold compound at the chip frontside to 20μm close to the chip surface as shown in Fig. 9.


After that, FIB cuts were performed (cf. Fig. 10 and Fig. 11) at  the region defined in Fig. 8 by IR-microscopy and the grinded  nailhead could be used for orientation (Fig. 10).


The SEM image in Fig. 12 shows a detail of the guard ring of FIB cut 1. Again, a clear evidence for corrosion of the aluminum metallization was identified.


To clarify the reason of the corrosion, a method had to be used  with low detection limits in combination with a high lateral resolution. Since the limited detection sensitivity of EDX did not allow identifying any corrosive element (EDX has a detection limit in the %-range), ToF-SIMS analysis was performed at the FIB cut 1 (Fig. 11 and Fig. 12) as shown in Fig. 13.


Figure 11: Detail of the FIB cut 1. The right arrow indicates the corroded alumina.


Figure 10: FIB cuts at the region of interest as


defined in Fig. 8.


Figure 9: Optical image of the top-down grinded


embedded sample. In fact, the sample is reduced to a partly transparent slice.


Figure 8: The cloudy regions indicated by the arrows are from corroded material.


Figure 7: Corrosion of aluminum metallization.


Al-Guard ring


Al-pad


FIB cut 1


Nailhead


Exactly at the position of the corroded guard ring an increased concentration of potassium was found.


To verify this result, a cross section of an other sample was prepared and analyzed with ToF-SIMS. Again ion polishing was applied as a final step to remove any potential contamination from the cross section surface.


At close range to the corroded aluminum metallization, an elevated concentration of potassium (K) exists. This confirms the previous result.


Potassium is known to be corrosive in combination with humidity and can be further accelerated by bias voltage.


Fig. 14 shows the ToF-SIMS mappings for Al, K and Si.


The next step of the analytical flow was to identify a potential  path of the potassium to penetrate into the package. With preparing cross sections with a fluorescent resin (Fig. 15) we could furthermore detect delamination between lead and mold compound to some extent.


Figure 13: ToF-SIMS analysis of potassium at the  FIB cut. The red circle indicates high potassium concentration.


Figure 14: ToF-SIMS analysis on a cross section.


Figure 12: Detail of FIB cut 1. The corroded aluminum guard ring (cf. Fig. 8) is visible.


Au wire bond


Al bond pad


Guard ring


K accumulation


Along these delamination migration of contaminants is possible.


The combination of the findings resulted in the following situation:


• Humidity is necessary for the failure.


• The electrical current flows through the wire bond along the chip surface.


• Corrosion of aluminum metallization on the chip surface took place.


• Potassium as a corrosive contaminant is found and can enhance aluminum corrosion [6].


• Lead-delamination is likely to enable potassium to migrate to the chip surface.


Therefore we inferred that in the presence of moisture conductive paths due to ionic contamination are formed and lead to the leakage current. With drying such a package,moisture is removed and the salt of the electrolyte remains which disables the leakage current.


Considering the different assembly processes of the diode, the  galvanic deflashing process with potassium-hydroxide was likely to be the source for the corrosive contaminant. To proof  the hypothesis, the process was changed and after the SMT application test no more leakage failure occurred.


In the previous paragraphs we revealed how the root cause of a leakage failure of a diode package was detected. Only the combination of techniques like SQUID, FIB and ToF-SIMS together with a careful sample preparation enabled this.


Furthermore this case shows that under certain conditions and with adequate sample preparation SQUID or ToF-SIMS can also be applied on cross-sections which is not typical for these  particular methods.


[1] H. Younan “Studies on A Failure Analysis Flow of Surface Contamination, Corrosion and Underetch on Microchip Al Bondpads in Wafer Fabrication”, 31st International Symposium for Testing and Failure Analysis  2005


[2] L.A. Knauss et al., “Detecting Power Shorts from Front and Backside of IC Packages Using Scanning SQUID Microscopy”, 25th International Symposium for Testing and Failure Analysis 1999


[3] F. Fleet et al., “HTS Scanning SQUID Microscopy of Active Circuits”, IEEE Transactions on Applied Superconductivity, 9(2) 4103, 1999.


[4] M. Pacheco et al., “Scanning SQUID Microscopy for New Package Technologies”, 30th International Symposium for Testing and Failure Analysis (2004)


[5] W. Mack et al., “Ion Beam Polishing for Embedded Cross-Sections and its Advantages for FESEM Analysis in Electronic Packaging”, 30th International Symposium for Testing and Failure Analysis 2004


[6] F. Beck, Integrierte Halbleiterschaltungen, Wiley-VCH(1993)


Figure 15: Cross section of the lead of the diode package (UV fluorescence).


Temperature and Humidity Dependent Reliability Analysis of RGB LED Chips


Jun-Xian Fu*, Shukri Souri


Exponent Failure Analysis Associates Inc., Menlo Park, CA USA


* jfu@exponent.com


James S. Harris, Jr.


Solid State and Photonics Laboratory, Stanford University, Stanford, CA USA


Temperature and humidity dependent reliability analysis was  performed based on a case study involving an indicator  printed-circuit board with surface-mounted multiple-die red, green and blue light-emitting diode chips. Reported  intermittent failures were investigated and the root cause was  attributed to a non-optimized reflow process that resulted in  micro-cracks and delaminations within the molding resin of  the chips.


Light emitting diodes (LED) have been investigated for  almost a century since the first carborundum LED was  reported by Henry Joseph Round in 1907 [1]. Benefiting from  the development of high quality compound semiconductor  materials, in-depth understanding of semiconductor device  physics and a strong market demand for high efficiency lightemitting devices, the solid-state lighting industry has made  significant strides over the past ten years [2]. Compared with  the LEDs based on group II-V or group IV semiconductor  materials, group III-V devices exhibit higher quantum  efficiencies. Among monochromatic devices, group III-V  LEDs cover a wide wavelength range, spanning ultra-violet to  infrared.


In the solid state lighting industry, ultra-violet or blue-light  stimulated phosphor has been investigated and  commercialized for white-light LEDs due to the relatively  wide visible spectral range that phosphor covers [3]. Ongoing  research and development efforts in the industry include  improving the reliability and light quality of phosphor based  white light LEDs. As a competing technology, multiple-die  LED chips are available in the market and have received  particular attention because of the flexibility and control in  achieving white light and different colors for indicator and  other applications. A popular multiple-die LED chip includes  three diodes for red, green, and blue (RGB) colors, which are  based on the semiconductor materials of AlGaInP and InGaN  with variable Indium compositions [4].


It is well known that the bandgap energy of semiconductor is  dependent on the temperature and, therefore, so is the  emission spectrum. The emission spectra of indirect bandgap  materials may have different behaviors from those of direct  bandgap materials. Materials with perfect crystal quality may  also have different temperature dependence compared to  materials with inherent lattice imperfections such as defects  and contamination. AlGaInP and InGaN have different  temperature dependence of emission spectra partially due to  the above two reasons [5].


Humidity in the environment is another factor that may  degrade the performance separately to, or combined with, temperature variations for non-hermetically sealed packaged  semiconductor devices [6]. The moisture accumulation at the  junction interface may generate surface charge accumulation  and so modify the junction characteristics. Furthermore, in  some scenarios, a harsh environment that includes high  humidity and high temperature, or fluctuations thereof, may  result in package damage. This can result in a common effect  known as popcorning in plastic packages [7]. For the LED  devices, the molding resin can also act as a lens and collimates  or diffuses the emitted light. This may introduce more  stringent requirements on the humidity and temperature  characteristics.


In this paper, we discuss an investigation of a reported  intermittent failure of packaged RGB LED chips and the  reliability analysis performed on the temperature and humidity  dependence of the device performance and characteristics. Various characterization methods were employed to study the  failure mechanism. Exposing the LED chips to elevated  temperatures during the PCB reflow process and subsequent  water washing are likely to have contributed to resin cracking, delaminations and intermittent connections.


System inspection


An indicator PCB board was reported to have degraded in  performance over time and eventually failed open-circuit or  exhibited intermittent behavior. The PCB had two surfacemounted RGB LED chips, and each chip had three LEDs. Visual inspection under high magnification revealed  deformation of the colorless resin lens, as compared to


## Temperature and Humidity Dependent Reliability Analysis of RGB LED Chips


137


exemplar devices and micro-cracks were observed around the  bonding wires inside the resin (Fig. 1).


Figure 1: Deformation of colorless resin lens (top) and microcracks along the bonding wires in the molding resin (bottom).


Initial diode measurements were performed using a digital  multi-meter under diode mode. The reported open-circuit  failures or intermittent failures were confirmed with only  some of the reported failed diodes within the RGB LED chips. Additional storage time was allowed before further  measurements were carried out. Repeated measurements  revealed self-healing and functionality recovery of the diodes  under test.


Figure 2: Photoemission microscopy of two report-failed  InGaN green LEDs.


Photoemission microscopy through the resin lens was  performed. As shown in Fig. 2, no obvious permanent darkspot or dark-line defect or other die-surface damage was  identified.


Curve-tracing results of the LED indicated that the turn-on  voltage at particular forward current and the leakage current at


particular reverse voltage were within the manufacturer’s  datasheet specification.


Scanning acoustic microscopy (SAM) was performed for two  RGB LED chips on the same PCB, one of them a reported  good chip (exemplar) with all three LEDs functional, and the  other one a chip with all three LEDs having reported opencircuit failure and then self-recovery after additional storage  time. As shown in Fig. 3, the failed chip exhibits a higher  delaminated area ratio as compared to the exemplar. Such  delamination may lead to the reported open-circuit and  intermittent failures.


Figure 3: SAM for two RGB LED chips on the same PCB, (top) a reported goof chip, and (bottom) a chip with reported  failures and self-recovery over time.


Based on the inspection, characterization and measurements  performed and discussed in this section, the reported opencircuit and intermittent failures of the LEDs within the RGB  LED chips are likely packaging related failures as a result of  the combination of elevated temperature and/or humidity  either during manufacturing or application. Therefore, additional characterization and reliability analysis was  performed to study the failure mechanism.


Temperature dependence analysis


Junction temperature measurement


Two methods were employed to measure and evaluate the  junction temperature of operating exemplar LEDs under  different conditions. The optical method is based on the  emitted light spectra, and the electrical method is based on the  voltage drop across the diode junction.


Regarding the optical characterization method, the lower  energy side of the emission peaks is generally related to the  density of states, with intensity ∝ (E-Eg)1/2. Whereas, the  higher energy side of the emission peaks is related to the  Bolzmann distribution, with intensity ∝ exp(-E/kT). The line  shape with temperature dependence of the emission peak at


the higher energy (short wavelength) side was clearly shown  for the AlGaInP red LED in Fig. 4. As shown in Fig. 4, the  temperature dependence was not significant for InGaN green  and blue LEDs. The mechanisms of abnormal temperature  dependence of InGaN LEDs have been investigated widely  and the generally accepted explanation involved the deep-trap  exciton localization and band-tail emission [5].


Figure 4: Light emission spectra from red (top), green (middle) and blue (bottom) LEDs within the same chip at  different ambient temperature, each LED operating  continuously with forward current of 25mA.


The central peak wavelength shifted as the ambient  temperature changed as shown the inset plots in Fig. 4. With  the ambient temperature heating up from 30°C to 160°C, the  central peak wavelength of all of the three LEDs in the same  chip red-shifted to longer wavelength. The central wavelength  of AlGaInP red LED shifted by 22.0nm, that of the InGaN  green LED shifted only by 4.5nm, and that of the InGaN blue  LED shifted by 10.5nm. The emission efficiency dropped


more than 50% for all the LEDs with AlGaInP LED dropping  the most.


When high resolution EDS spectrums are


collected (with reported beam spot <10nm), high  content of S and Pb, Bi, Nb, Ag are detected in


grains and boundaries with localized, concentrated  spots and/or regions (Fig. 14, 15, 16, 17).


Figure 14-17: High concentration of S, Bi, Pb, Sr  and Nb are detected in grains and in certain area  within a grain (spot 7) and grain boundary (spot  5).


8. TEM Selected Area Electron Diffraction


It is reported that when BaTiO3 is doped with


impurities, it can become a semiconductor [1].  In  order to examine the possibility of crystal structure  change, selective area electron diffraction (SAD) patterns are acquired on the sample in Fig. 9.


Distinguishingly different diffraction patterns are  obtained in the area where STEM/EDS analysis is  performed (Fig. 18, 19).


Although these patterns are not quantitatively


characterized, the most likelihood of these are


tetragonal and cubic centered crystal structures.


The former is ferroelectric and the latter is


paraelectric in nature.


Figure 18, 19: Two distinguishingly different


diffraction patterns are obtained in adjacent grains. They manifest difference their in lattice space and  angle indicating that they have different crystal  structure.


Result and Discussion:


1. The evidences obtained in the current study  demonstrate that this type of low leakage in  BaTiO3 capacitor is not caused by observable  physical defect such as fractures, voids, etc. in the  ceramic matrix.


2.  Since CCD camera on photon emission


microscope is designed to detect photons with


wavelength around 1010nm, which is


approximately the band gap energy of Si (1.1eV). Since BaTiO3 is a dielectric material with band


gap energy of 3.3eV, the fact that PEM can detect  strong emission signals manifests that narrow gap  leakage, i.e. semi-conducting behavior is taking


place in these leaky capacitors.


3. It is known that when the crystal structure of


BaTiO3 undergoes a phase transition from


tetragonal to a cubic unit cell, the material will


change from ferroelectric to paraelectric.  Thomas  Research Group recently reported that when doped  with impurities, BaTiO3 can be transferred from


dielectric material into semiconductor, and grain


boundary region is concluded in control of such


phase transition [4].


4. It is well known that being at the state of lowest  free energy, grain boundaries easily gathers


impurities inside crystal structure.


5. In light of the above information, and based on  the evidences collected in this analysis, a failure


mechanism is proposed for these low leakage


capacitors as follows:


Localized high concentration of impurities at grain  boundaries and inside certain grains induced


partial transition of the ferroelectric BaTiO3 into  paraelectric and/or exhibiting semiconductor


behavior that resulted in failures under bias at


assembly final test as well as latent field failures.  Furthermore, the fact that these latent field failures  did pass initial test suggests that a redistribution of  impurities inside the BaTiO3 matrix has taken


place under the influence of electric field.


Statistics shows that most field failures occurred in  regions with climate of high temperature. Hence


temperature plays an important role in the


redistribution of the impurities, i.e. it acts as a


driving force for the diffusion of impurities along  grain boundaries.


A combination of relatively low sintering


temperature and uncontrolled contamination in


raw materials in certain lot in the capacitor


manufacturing process is considered to be the


most probably root cause of this failure.


Conclusion:


A complete failure analysis process flow for low  leakage capacitor is developed. By employing  mechanical cross-section and emission  microscopic analysis, precise localization of  failure site is made possible even without any  observable physical sign. This failure analysis  process is easily applicable to any lab equipped  with basic failure analysis instrument.


Acknowledgement:


The author would like to express sincere  appreciation to Mr. Clifford Schuring, Dr. James  Qu at IR, to Mr. Terry at Material Analysis  Services for technical discussions. Special thanks  are due to the administrative support from the  organization of Center of Excellence, International  Rectifier, Corp.


[1] H. Kihsi, Y. Mizuno and H. Chazono, “Base  Metal Electrode Ceramic Capacitors: Past,  Present  and Future Perspectives”, AAPPS Bulletin  Vol. 14, No.2, April 2004 pp2-16


[2] B.A.Marinkovi, B.D.Stojanovic, VP.Malberti, M.Ciappa, P.Scacco, A .B.Pavlovic, M.M.Ristic, “Correlation of Microstructure and Dielectrical  Properties of BaTiO3 Sintered from Mechanically  Activated Powders”, Materials Structure, Vol. 6, No. 2, 1999, pp96-99


[3] Y.Kim, C.H.Chen, A.Saiki, N. Wakiya, K.Shinozaki and N. Mizutani “Effect of Nb and Sr  doping on Crystal Structure of Epitaxial BaTiO3  Thin Films on MgO Substrate”, J. of Phys D: Appl. Phys. 35, 2002 pp1499-1503.


[4].D.Thomas,


“Interfacial


States


in  Semiconducting BaTiO3”, Thomas Research  Group


http://www.chembio.uoguelph.ca/thomas/batio3_r esearch.html


[5]A.R. West, “Solid State Chemistry and Its  Application”, published by John Wiley and Sons, 1987, pp540-548.


A System for Electro-Mechanical Reliability Testing of MEMS Devices


Stefan Spinner


Computer Architecture Group, Institute for Computer Science, University of Freiburg, Germany and


Microsystem Materials Laboratory, Department for Microsystems Engineering (IMTEK), University of Freiburg, Germany  stspinne@informatik.uni-freiburg.de


Michael Doelle, Patrick Ruther, and Oliver Paul


Microsystem Materials Laboratory, Department for Microsystems Engineering (IMTEK), University of Freiburg, Germany {doelle|ruther|paul}@imtek.uni-freiburg.de


Ilia Polian and Bernd Becker


Computer Architecture Group, Institute for Computer Science, University of Freiburg, Germany {polian|becker}@informatik.uni-freiburg.de


This paper reports on a setup and a method that enables  automated analysis of mechanical stress impact on  microelectromechanical systems (MEMS). In this setup both  electrical and optical inspection are available. Reliability  testing is possible on a single chip as well as on the wafer  level. Mechanical stress is applied to the tested structure with  programmable static forces up to 3.6 N and dynamic loads at  frequencies up to 20 Hz. The applications of the presented  system include the postmanufacturing test, characterization  and stress screens as well as reliability studies. We report  preliminary results of long-term reliability testing obtained for  a CMOS-based stress sensor.


Microelectromechanical systems are employed in safetycritical fields such as automotive, aerospace and medical  applications. Therefore, their reliability is receiving growing  attention. This includes both ensuring the correct functioning  of a MEMS just after it has been fabricated, i.e. the  manufacturing test and studying the possible deterioration of  the device in its application. The latter issue is of special  importance, as MEMS applications often intrinsically involve  mechanical stress which could damage or destroy  microstructures [1].


The manufacturing test focuses on deciding whether a device  is ‘good’, i.e. can be shipped to the customer, or ‘bad’. In  high-volume manufacturing, electrical testing methods are  more attractive than optical or chemical techniques, as the  former result in high throughput and consequently low costs. Moreover, available automatic test equipment for integrated  circuits (ICs) can be leveraged [2]. The characterization of a  device serves the purpose of obtaining a better understanding  of its physical behavior. Available techniques range from  structural methods (optical, micro-Raman, scanning electron  and transmission electron microscopy) to chemical analysis (X-ray, Auger and secondary ion mass spectroscopy) and


special electrical approaches (thermally-induced voltage  alteration, resistive contrast imaging) [3]. Although these  methods provide detailed information on the behavior of both  fault-free and faulty devices, they are associated with  significant cost and are not applicable to volume  manufacturing. The reliability studies examine the device’s  ability to retain the desired functionality in possibly harsh  environments.


In this paper, we propose a system for the fully automated  wafer-level testing of mechanical stress impact on the  functionality of MEMS. The mechanical stress is induced by  an impact object that exerts a controlled force on the surface  of the device under test (DUT). The applied force level, force  duration, frequency of dynamic force loads and the location at  which the force is applied are user-defined and can be  precisely controlled. The system can step over a 6-inch wafer  without operator interaction and hence is well suited for longterm stress test runs. The electrical and optical inspection of  device behavior before, during, and after the application of  mechanical stress to the DUT is available.


Figure 1: Setup consisting of a position stage and a frame  holding the mechanical impact control unit. The inset shows  the probecard with its contacts and the mechanical impact  object that exerts a force on the wafer and hence the DUT.


## A System for Electro-Mechanical Reliability Testing of MEMS Devices


147


The system is modular, which implies a high degree of  flexibility with respect to the DUT, the impact object and the  type of analysis. Possible DUTs include micromechanical  sensors such as accelerometers or gyroscopes, which have to  be reliable in the presence of mechanical stress, as caused, e.g., by their plastic package. The devices may be CMOSbased MEMS or systems manufactured in one of the  numerous bulk or surface micromachining MEMS processes. Even conventional ICs used in harsh environments may be  interesting objects of investigation. To perform reliability test  for different DUTs, only the probecard, which is used for  electrical contacting, has to be exchanged. The impact object  can be selected freely out of a large number of possible  candidates. The impact object fixture is designed such that it  can accommodate objects ranging from needles of different  materials to bonding capillaries.


The remainder of the paper is organized as follows. The  proposed system is described in the next section. Experimental  results for a CMOS-based MEMS stress sensor chip are  reported in the section experimental results. The last section  concludes the paper.


Experimental Setup


The mechanical part of the measurement system is  schematically shown in Figure 1. It consists of a positioning  stage used for wafer stepping, a frame and a mechanical  impact control unit attached to the frame (see Figure 2). The  positioning stage consists of two linear stages (OWIS LIMES  120) for moving the wafer in the x and y directions, a linear  stage (OWIS HVM 60) for positioning in the z (vertical) direction, and a rotation stage (PI M-036) for further  alignment. A vacuum chuck to fix the wafers is mounted to  the rotation stage. The mechanical impact control unit shown  in Figure 3 comprises (i) a fixture for the impact object  controlled by a closed-loop xyz nanopositioning system (PI  P-611.3S NanoCube), (ii) a force sensor (ME-Messsysteme


KD40S5N) for surface detection and calibration, and (iii) a  manual xyz stage for coarse positioning of the NanoCube and  the impact object with respect to a probecard. This probecard (HTT GmbH, Dresden) is used to electrically contact the DUT  and is integrated into the mechanical impact control unit. Note  that for the application of mechanical stress, the impact object, e.g., a needle-like probe, is moved by the NanoCube, whereas  the probecard position is fixed relative to the mounting frame. This is achieved by a hole in the probecard through which the  impact object is translated towards the DUT, as shown in the  inset of Figure 1. A microscope can be attached to the system  for optical inspection.


In the mechanical stress experiment, the impact object is  repeatedly pressed by the NanoCube against predefined  positions on the wafer, which is fixed on the vacuum chuck. The stepping of the wafer underneath the probecard is  performed by the positioning stage. The mechanical impact  control unit is not moved in the xy plane during the  experiments. A micrograph taken during an experiment is


Figure 2: Photograph of the mechanical setup showing the  NanoCube, the manual stages for positioning the NanoCube, the probecard for electrically contacting the DUT and the  position stage to move the wafer with respect to the  NanoCube.


Figure 4: Micrograph of the wafer with the stress sensor and  the bond pads. The probecard needle and the mechanical  impact object are clearly visible as well.


Figure 3: Mechanical impact control unit consisting of the


NanoCube and manual position stages for x, y, and z  movement of the NanoCube. The force sensor and the  mechanical impact object are attached to the NanoCube.


shown in Figure 4.


An experiment is preceded by the following initialization  steps: (i) the position stage is calibrated by moving the linear  stages and the rotation stage to their zero position, (ii) the  wafer is moved in the xy plane such that the first DUT is  underneath the impact object, (iii) the NanoCube is manually  positioned close to the wafer surface, and (iv) the automatic  surface detection procedure runs for fine calibration of the  NanoCube in the z direction. The automatic surface detection  procedure moves the impact object in 1 m steps towards the  wafer surface until the force measured by the force sensor  increases significantly, i.e. the impact object touches the  wafer. The movement of the impact object is continued until  the predefined force level is achieved. The respective vertical  positions of the contact point and for the desired force value  are memorized.


During the experiment, the wafer is placed on the vacuum  chuck, which is part of the position stage. The linear stage for  the z direction brings the chuck into two positions: up and  down. In the upper position, the DUT on the wafer is  contacted by the needles of the probecard and electrical  measurements can be performed. In the lower position, the  wafer can be moved in the xy plane by the position stage  without damaging the DUT or other structures on the wafer by  the probecard contacts. Mechanical stress is only applied to  the DUT in the upper position.


Figure 5: Voltage drop across the LED junction versus the  ambient temperature.


Because of the difference of temperature dependence of the  emission spectra for LEDs with different materials in the  active region, the electrical method was used to measure the  junction forward voltage drop for particular pulsed current  driving conditions, to minimize any active heating. As shown  in Fig. 5, the temperature dependence of forward voltage drop  across the diode junction was calibrated using an  environmental chamber ambient temperature control. The  driving current signals for the LEDs were 25mA, 100Hz, and  with duty ratio of 0.5%. The heating effect due to forward  current can, therefore, be neglected. Based on the results


shown in Fig. 5, for a continuous driving current of 25mA, the  junction temperatures for red, green and blue LEDs were


43.4°C, 52.8°C, and 56.8°C, respectively.


Temperature uniformity and interference


It is difficult to control the temperature uniformity inside the  molding resin across the chip even for white-light illumination  applications. For indicator applications, the interference of  different LEDs within the same chip is shown in Fig. 6. The  LEDs were driven by three independent current sources. The  shifting of the emission peak of AlGaInP red LED cannot be  explained by spectrum pulling effect. A possible explanation  can be attributed to the local heating from other LEDs  changing the junction temperature.


Figure 6: Interference of LEDs within the same chip.


Humidity dependence analysis


Plastic package fidelity


The material used for colorless lens of the LED chips is  Nylon, which together with the plastic package may absorb a  certain amount of moisture during production stage or  application. Figure 7 shows the weight change between preand post-baking (120°C, 1hr) for incident chips and known  good samples on shelf and after excessive water wash. It is  noted that failed LED chips from incident PCBs have  observably higher moisture levels than exemplar chips and  unused good samples of the shelf.


Figure 7: Absorbed moisture measurements for LED chips  from incident PCB and unused or used known good chips.


Molding defects were observed as shown in Fig. 8. The  breakage of the resin lens may result due to poor production


monitoring or misapplication. Such breakage decreases the  immunity of devices to moisture ingression.


Humidity effect


A high temperature, high humidity un-powered stress test was  performed to evaluate the plastic package and resin lens. Moisture-induced contamination can easily be recognized as  shown in Fig. 9.


Figure 8: SEM image of RGB LED chip surface of the resin  lens and plastic package.


Figure 9: Effect of high temperature (85°C) and high humidity (85% relative humidity) stress test.


Based on the temperature and humidity dependence analysis  of the device’s performance and package fidelity, the PCB  reflow process and application were reviewed in detail. The  moisture accumulation inside the resin lens and plastic  package during the prolonged over-heating and subsequent  water washing in the reflow process is likely the root cause for  the micro-cracks along the bonding wires inside the molding  resin, leading to the subsequent degradation of emission and  intermittent or open-circuit failures. Due to the lack of  temperature uniformity inside the molding resin caused by the  different driving conditions of the three LEDs, residual  stresses can develop that may result in eventual delamination. It is essential to optimize the PCB reflow process and monitor  the driving conditions of multiple LEDs within the same chip  in order to take full advantage of long life time and reliable  device performance.


[1] E. Fred Schubert, Light Emitting Diodes, Cambridge  University Press (Cambridge, 2003)


[2] D. A. Steigerwald, J. C. Bhat, D. Collins, R. M. Fletcher, M. O. Holcomb, M. J. Ludowise, P. S. Martin, S. L. Rudaz, “Illumination with solid state lighting  technology,” IEEE J. Sel. Top. Quantum. Electron., Vol. 8, No. 2 (2002), pp. 310-320


[3] R. Mueller-Mach, G. O. Mueller, “White light emitting  diodes for illumination,” Proc. SPIE, Vol. 3938 (2000), pp. 30-41


[4] S. Muthu, F. J. Schuurmans, M. D. Pashley, “Red, green, and blue LED based white light generation: issues and  control”, 37th IAS Annual meeting, Vol. 1 (2002), pp. 327-333


[5] P. G. Eliseev, P. Perlin, J. Lee, M. Osinski, “’Blue’ temperature-induced shift and band-tail emission in  InGaN-based light sources,” Appl. Phys. Lett. Vol. 71, No. 5 (1997), pp. 569-57.


[6] M. Arik, J. Petroski, S. Weaver, “Thermal challenges in  the future generation solid state lighting applications: light emitting diodes,” Proc. IEEE Intersociety Conf. Thermal Phenomena, (2002), pp. 113-120


[7] G. S. Ganesan, H. M. Berg, “Model and analyses for  solder reflow cracking phenomenon in SMT plastic  packages”, IEEE Tran. Comp. Hybr. Manu. Techno., Vol. 16, No. 8 (1993) pp. 940-948


A Study of Low Leakage Failure Mechanism of  X7R Multiple Layer Ceramic Capacitor (MLCC)


Zhaofeng Wang, Sr. FA Enginner


Failure Analysis Lab, International Rectifier Corp. 41915 Business Park Dr. Temecula, CA92590


Tel. (951) 375-4270, e-mail zwang1@irf.com


This paper presents the result of a study  of a particular failure mechanism of BaTiO3  MLCC (multiple layer ceramic capacitor). A  unique technique of cross-section alternating with  emission microscope analysis is developed to  precisely locate the failure site for capacitors  exhibiting low leakage current in µA range. Thermal Imaging Microscope, Photon Emission  Microscope, SEM, STEM/EDS and TEM electron  diffraction pattern are employed for the  characterization of these low leakage failures. Evidence of high concentration impurities are  detected in the dielectric layer of BaTiO3 grain  boundaries as well as inside certain grains. TEM  diffraction imaging at the failure site shows  distinguishingly different diffraction patterns  within the matrix of BaTiO3 crystal structure. The  evidences point to a combination of impurities at  grain boundaries and BaTiO3 crystal change  induced by impurity as the failure mechanism.


Surface mount technology has been rapidly  expanding in microelectronic industry in the last  decade. As a highly reliable passive component, BaTiO3 based multiple layer ceramic capacitors (MLCC) has enabled manufacturers to achieve  high level of packaging density and assembly  automation.


BaTiO3 is a ferroelectric material. Its crystal unit  cell posses a permanent electric dipole (instead of  cubic, its crystal structure is tetragonal, i.e. distorted Perovskite structure). Neighboring unit  cells can all align together to produce a large  domain with a particular electric dipolar  orientation. Hence it has very high dielectric  constant (several orders of magnitude higher than  that of SiO2). The basic structure of a multilayer  ceramic capacitor consists of alternating thin  layers of dielectric ceramic material and metal  electrodes.


The most commonly reported MLCC failure  mechanisms are cracks, de-lamination between the  ceramic dielectric layers by thermo-mechanical  stress, or electric over stress in application.


The samples analyzed in this study are production  line final test rejects and latent field failures that  have low leakage current (in the range of tens to  hundreds of micron amp). They manifest no  evidence of the above mentioned mechanisms, i.e. there is no sign of any physical damage at the  leakage site.


Analysis Procedure


1. Electric Characterization of Failed Capacitors  The capacitors under investigation failed in field  application. Fig. 1 shows an unstable low leakage  IV curve.


leakage=85uA@12V


Figure 1: The leakage curve of a failed capacitor.


2. Thermal Imaging Microscope Analysis


Hot spot can be detected by thermal imaging  microscope with InSb camera (Fig. 2). The hot  spot is almost always near the edge of electrodes.


Figure 2: Detected hot spot region. Note: the blue  and white dashed lines indicate x-sections.


3. Cross-sectional Analysis


3.1. X-direction sectioning


A cross-section cut is made along x- direction  through the outer shell (dashed blue line in Fig. 2) with a slight angle such that the electrodes at the  opposite side of the hot spot are exposed, while  the electrodes at the failure side are un-disturbed.


142


This x-direction allows a visible contrast image of  the active area under optical microscope (Fig. 2).


Figure 3: A failed capacitor in an application


circuit.


Thanks to the unique nature of capacitor, physical  cross-section parallel to x and y direction does not  affect its electric behavior other than reducing its  capacitance in proportion to the area being  removed. The sectioned sample is subjected to  thermal imaging microscope analysis at the side  view. The hot spot location in x-direction is  confirmed, and its position in z-direction can also  be estimated at the sectioned surface (Fig. 3).


Figure 4: The hot spot in Figure 2 is shown after  x-direction sectioning.


Figure 4a: Optical (bright view) of the Figure 4. Note: electrodes at the hot spot area are not


exposed yet, i.e. undisturbed.


Figure 4b: Optical (dark view) of Figure 4


showing the contrast of the active area.


3.2 y-direction sectioning


With Fig. 4 as a reference, section is now made in  y-direction approaching the hot spot (Fig. 5).


Figure 5: Optical (dark view) of the sample after  both x and y-direction sectioning.


4. Photon Emission Microscope (PEM) Analysis


with Micro-Probing


Upon y-direction sectioning, the connection of the  multi-layer electrodes at one end is removed. Each  pair of parallel electrodes can be individually  probed. Micro-probing narrows the leakage down  to two specific layers. With the advantage of high  magnification lens in PEM, the hot spot can now  be precisely localized in x, y, z dimensions by  alternating between y-direction polishing and  PEM emission acquisition (Fig. 6).


x-direction


y-direction


Figure 6: The hot spot is precisely localized in x


(top), y (bottom) and z directions with microprobing under PEM.


5. SEM Examination


Figure 7, 8 are SEM images of the failure site.


There is no sign of physical damage or defect


observed except some contrast between grains.


Unfortunately, the limited resolution of beam spot  size of SEM prevents EDS analysis from


differentiating any compositional variation in the  grains or grain boundaries.


Figure 7, 8: SEM picture of the emission site.


6. Localized Cracks in High Leakage Failure


In the analysis of capacitors that have high leakage  current (in the range of tens to hundreds mA), high  contrast spot at the failure site can be readily seen  under dark field view (Fig. 9). SEM imaging


shows that localized micro-cracks are present at


the failure site, some trans-granular some intergranular (Fig. 10, 11).


In light of the evidence observed on the low


leakage caps, and the fact that micro-hardness test  conducted by an independent lab shows no


difference in material hardness, fracture toughness  between good and failed parts, even no difference  in various spots within a failed one, these microcracks are considered to be the effect of the


failure,


Figure 9: optical contrast at a high leakage spot.


Figure 10: A transgranular micro-crack observed  at a high leakage site. It is considered the effect of  failure, i.e. electric over stress.


Figure 11: An intergranular micro-crack observed  at a high leakage site. It is considered the effect of  failure, i.e. electric over stress.


7. STEM and High Resolution EDS Analysis


STEM imaging of atomic contrast shows


significant variation between adjacent grains and  even within a single grain (Fig. 12, 13).


Fig. 12: STEM image at the failure site showing


high compositional contrast among grains (the  darker region indicates lighter elements)


failure  center


Figure 13: Close-up of Figure 12 showing high  contrast in grain boundary (spot 5, 6), and also  within a single grain (spot No. 7).


The mechanical stress experiment itself is performed by  moving the vacuum chuck to the upper position, applying the  mechanical stress and simultaneously performing electrical  and/or optical inspection. Duration, frequency and absolute  level of mechanical stress can be chosen freely, limited only  by the parameters of the NanoCube and the force sensor used  in the automatic surface detection procedure. The employed  force sensor has a range of up to 5 N with a resolution of  5 mN; however it can be easily replaced by a different sensor  in case higher force values or better accuracy are necessary. The NanoCube in combination with the force sensor can apply  forces up to Fmax,eff = (3.61 ± 0.02) N at a frequency of up to  20 Hz. In principle, forces up to 30 N would be accessible by


the NanoCube. However, due the low stiffness of the force  sensor and a maximum travel range of the NanoCube of


L0 = 100 µm this value is reduced by almost one order of  magnitude. As the stiffness of the other sub-assemblies is  higher than that of the force sensor, their effect on the  maximum force value can be neglected. The options for  electrical measurements are determined by the capabilities of  the parameter analyzer, but it is also possible to use any  gauges for electrical measurement, which fits the needs of the  actual investigation of the DUT.


Once the measurement is finished for one DUT, the chuck is  moved to the lower position and the position stage places the  wafer so that the next die lies underneath the probecard. Next, the electrical measurement is repeated for this DUT, and so  on. The system makes possible for the full wafer  characterization of 6-inch wafers. The positioning stages  LIMES 120 have an accuracy of 2 m and a travel path length  of 200 mm. Consequently, no re-positioning in xy plane is  required during the experiment. However, a recalibration in  the z direction is done by repeating the wafer surface detection  procedure. Also the parameter analyzer is automatically  recalibrated after a certain time interval. Nevertheless, none of  the recalibration procedures involve any manual activity, so  that the experiment, once started, is fully automatic. The  whole experiment is controlled by a program developed using  LabVIEW, an integrated development environment by  National Instruments. All parts of the experimental setup, i.e. the parameter analyzer, the NanoCube, the linear stages, and  the force senor, are remotely controlled over GPIB and RS232  buses. The schematic view of the software control is shown in  Figure 5.


Dynamic Force Application


The complete measurement setup has a complex mechanical  behavior. If the NanoCube applies a force to the DUT some  components of the setup will be squeezed while others will be  stretched. This takes time till all components have reached a  static deformation. The overall behavior can be approximately  described by the differential equation


p


Figure 5: Schematic view of the system. The parameter  analyzer and the position stage are controlled over the GPIB  bus using a LabVIEW program developed for this purpose. The DUT is connected to the parameter analyzer using a  probecard. The NanoCube and the force sensor are controlled  via a RS232 serial interface.


Figure 6: Response of the measurement system to a force  jump from 0 N to 1 N applied at time 0.


where T, Kp, xe and Tv denote the time constant of the  exponential decay of the output force function xa, a  proportionality factor, the input force function, and a second  time constant. The ratio between T and Tv describe to height of  overshoot at the beginning of the output force function if a xe is a jump function. Figure 6 shows a respective response  measured at a force jump of 1 N at t = 0 s.


This behavior of the measurement system is unproblematic  during static measurements. An adjustment control can be  used to control the applied force in such a way that 0.2 s after  a force step the measured force is the targeted force within the  accuracy of the force sensor. The adjustment control works as  follows. First the NanoCube is programmed to move to a  position p. Second the force sensor delivers the actual force  applied to the DUT and sends this value to the computer that  calculates the deviation between the target force and the  applied force and sends a corrected position p’ to the  NanoCube.


For dynamic measurements it was not possible to implement  the adjustment control due to the slow communication speed  between the three invoked components of the measurement  setup: (i) NanoCube, (ii) force sensor, and (iii) computer. One  cycle has a duration of 20 ms. To get around this drawback, a  control system was implemented which learns the positions of  the NanoCube that are needed to apply the desired force  function to the DUT within the accuracy of the force sensor. The algorithm works as follows. First the computer sends an  array of predicted positions to the NanoCube. The NanoCube  moves in a given time step width to each given position in the  array. During the movement of the NanoCube the force sensor  measures the applied forces and sends an array with the force  evaluation to computer. These measured forces are then used  to determine a corrected position array. The new position  array then is sent to the NanoCube that uses the new positions. This procedure is iterated until a convergence to the desired  force function is achieved. The performed measurements  show that after five learning cycles the applied force function  differs from the desired force function by less than the  accuracy of the force sensor. Figure 7 shows the deviation  between the desired square function with jumps from 0 N to


1 N at 0 s and back to 0 N at 5 s. After five learning cycles the  deviation is given by the accuracy of the force sensor, i.e. 5 mN. The deviation at the jump positions is larger than the  force sensor accuracy, due to the rise and fall time constant of  the NanoCube.


Device Under Test


The device tested in this study is a CMOS-based stress sensor  similar to those presented in [4, 5]. It was fabricated using the


0.6 m triple metal, double poly CMOS process CX by  X-FAB AG (Erfurt, Germany). The stress sensitivity of the  sensor is based on the shear piezoresistance effect, also termed  the pseudo-Hall effect in silicon. The sensor has four  terminals, two of which serve as inputs and two serve as  outputs as shown in Figure 8. The sensor is biased with an  input current Iin. Upon application of a mechanical shear stress


xy the stress sensitive the pseudo-Hall voltage VpH is  measured. It is defined as


xy


pH


where 44, xy, and Vin are the piezoresistance sensitivity  coefficient, the shear stress, and the biasing voltage, respectively. Figure 8 illustrates the direction of Iin, VpH and


xy in case of a square stress sensor with four point contacts. The size of the active area of the sensor is approximately  13 m × 13 m. The sensor is a n-channel field effect  transistor. Its sides are aligned along the <110> crystal  direction parallel to the flat of the wafer flat.


Measurements


We applied a series of 600 stress cycles to a DUT. Each stress  cycle was composed of a period of 2 s in which a force of


1.3 N was applied to a location 250 m away from the sensor. This was followed by another 1.7 s in with zero force. A  spring contact probe (Feinmetall F58510S063L130) with head  and sleeve fixed using solder in order to eliminate any  suspension effects was used as the impact object. The  electrical response VpH of the device to mechanical stress


Figure 7: Deviation between the target force function with a  jump at 0 s to 1 N and at 5 s to 0 N and applied force function  of the first five learning cycle.


Figure 8: Schematic illustration of a four contact stress  sensor. In the presence of mechanical shear stress xy a  potential difference VpH arises between two opposing contacts.


during one stress cycle, is shown in Figure 9. The force is  applied between 1.0 s and 3.0 s. It can be seen that the sensor  responds to mechanical stress by a change of VpH of around


0.8 mV. We define VpH as the difference between VpH at 0 s  and its value at 2.0 s.


In order to characterize the degradation of the sensor due to


cyclic stress, VpH was measured for the first 600 stress  cycles. The results are shown in Figure 10. The values remain  roughly at the same level, suggesting that there is no  deterioration in the first 600 cycles. This is likely due to the  short overall duration of this measurement run of  approximately 40 minutes. Further experiments are currently  being conducted, using different forces, frequencies, application positions and impact object materials and shapes. The measurement setup also has proven its capability by other  measurements. As an example, the measurement setup was  used to determine the force versus VpH characteristic of the  stress sensor for a given position of the force application [6]. The measurement makes use of the accurate force  measurement of the system. The measurement system was  used also to determine mechanical parameters of a 3D silicon  force sensor [7]. In particular, the system was used to examine  the long term reliability of the 3D force sensor. In these  measurements the sensor was exposed 50 000 load cycles with  a target force of 500 mN [8]. The average applied force was


503.52 mN with a standard deviation of 0.32 mN.


We implemented a modular test system for wafer-level  electrical inspection of MEMS under mechanical stress. Test  parameters such as force level, frequency and location are  programmable, and the impact object can easily be changed. Wafers up to 6 inches in diameter can be stepped through the  system automatically. Consequently, the system is suited for  characterization and accelerated stress screens for different  types of MEMS. Although our preliminary data collected for a  CMOS-based stress sensor indicates no deterioration during


600 stress cycles, we are gathering more data using different  mechanical stress parameters and other impact objects.


While studying and improving the reliability of the device  under test is an important application of the equipment, our  long-term goal is to enhance our understanding of defect  mechanisms in MEMS. Of particular interest is the  applicability of structural test methods based on fault models  to MEMS testing as suggested in [9]. A further field of  investigations is the quantitative analysis of the influence of  built-in self test and self repair structures on MEMS reliability [10].


Acknowledgement


This work was supported by the DFG grant GRK 1103/1 “Embedded Microsystems” of the Deutsche  Forschungsgemeinschaft.


[1] J. Walraven. Failure mechanisms in MEMS. Int. Test  Conf., pages 828–833, 2003.


[2] T. Maudie, A. Hardt, R. Nielsen, D. Stanerson, R. Gieschke, and M. Miller. MEMS manufacturing testing: An accelerometer case study. Int. Test Conf., pages 843–849, 2003.


[3] J. Walraven. Tools and techniques for failure analysis and  qualification of MEMS. Int. Test Conf., pages 834–842,


2003.


[4] M. Doelle, P. Ruther, and O. Paul. A novel stress sensor  based on the transverse pseudo-Hall effect of MOSFETs. Proc. IEEE MEMS Conf. 2003, pages 490–493, 2003.


[5] M. Doelle, C. Peters, P. Gieschke, P. Ruther, and O. Paul. Two-dimensional high density piezo-FET stress sensor  array for in-situ monitoring of wire bonding processes. Dig. Tech. Papers MEMS 2004, pages 829-832, 2004.


[6] M. Doelle, C. Peters, P. Ruther, and O. Paul. Piezo-FET  Stress-Sensor Array for Wire-Bonding Characterization.


Figure 9: Stress sensitive signal VpH of the stress sensor as a  function of time. VpH was measured before, during and after  the application of approximately 1.3 N to the wafer.


Figure 10: Change of stress sensitive signal VpH caused by  the force impact for 600 measurement cycles.


J. Microelectromechanical Systems, Vol. 15, No. 1, pp. 120-130, Feb. 2006.


[7] P. Ruther, J. Bartholomeyczik, W. Dominicus, O. Paul, R. Roth, K. Seitz, W. Strauss, A. Trautmann, and M. Wandt. Three-Axial Silicon Force Sensor for Dimensional  Metrology of Micro Components. Proc. IEEE Sensors  2005, pages 1006-1009, Irvine, USA, 2005.


[8] S. Spinner, J. Bartholomeyczik, B. Becker, M. Doelle, O. Paul, I. Polian, R. Roth, K. Seitz, and P. Ruther. Electromechanical Reliability Testing of Three-Axial  Silicon Force Sensors. Proc. DTIP 2006, Stresa, Italy, pages 77-82, 2006.


[9] A. Kolpekwar, C. Kellen, and R.D. Blanton. MEMS fault  model generation using CARAMEL. Int. Test Conf., pages 557–566, 1998.


[10]N. Deb and R.D. Blanton. Built-in self test of CMOS  MEMS accelerometers. Int. Test Conf., pages 1076–1084,


2002.


Case Studies in Atomic Force Probe Analysis  


Randal Mulder, Sam Subramanian, Tony Chrastecky 


Freescale Semiconductor, Inc; 6501 William Cannon Drive, Austin, TX 78735 


Introduction 


The  use  of  Atomic  Force  Probe  (AFP)  analysis  in  the analysis  of  semiconductor  devices  is  expanding  from  its initial purpose of solely characterizing CMOS  transistors at the  contact  level  with  a  parametric  analyzer.  Other  uses found for the AFP include the full electrical characterization of  failing SRAM bit cells, current contrast  imaging of SOI transistors,  the  probing  of  metallization  layers  to measure leakages, and use with other tools, such as light emission, to quickly  localize  and  identify  defects  in  logic  circuits. The purpose  of  this  paper  is  to  present  several  case  studies  in regards to these activities and their results.  


Case Study I: AFP SRAM Bit Cell Electrical Characterization 


High Density SRAM Technologies (>100nm) 


SRAM bit cell electrical characterization has proven to be a useful  failure  analysis  tool  in  identifying  the  defects  that cause single bit cell failures [1]. By analyzing the entire bit cell,  the  location  and  type  of  defect  can  be  determined  to help  increase  the  probability  of  identifying  the  failure mechanism when the physical analysis is performed whether itís  in  the metal  layers of  the bit  cell or  in  the  transistors. This  type  of  analysis  is  performed  by  depositing  tungsten FIB pads on the bit line (BL), bit line bar (BLB), word line (WL),  Power  (VDD),  and  ground  (VSS)  (Figure  1)  [2]. Micro-probe needles connected to a parametric analyzer are used to sweep BL and BLB; and to bias the WL, VDD, and VSS. Electrical signatures produced by  the sweeping of the bit lines on a failing bit when compared to a passing bit  cell usually  indicates  the  type  of  defect  causing  the  bit  failure and its location within the bit cell. 


AFP  can  be  used  in  place  of  the  traditional method  using Focused  Ion Beam  (FIB) deposited  tungsten/platinum pads and micro-probe needles (T-4-10). Figure 2 shows a 0.25um SRAM array that has been deprocessed to the top of Via 2. The bit lines at Metal 3 have been polished off to isolate the failing bit  from  the other bits  in  the array and  to allow  for the AFP  to probe  the bit  line vias  and  the VDD  and VSS vias.  Because  the  AFP  has  only  four  available  heads  for 


probing, both the WL and VDD have to be powered with the same probe tip.  


Figure 1: Schematic of a 6T SRAM bit cell shows  that  five nodes BL, BLB, WL, VDD, and VSS have  to be biased  for the electrical characterization of the bit cell. 


The WL and VDD connections for the bit cell run the length of  the  array  along  the  rows  at  Metal  2  layer  for  this technology. At the edge of the SRAM array the FIB is used to  cut  a  small  whole  through  the  inter-level  dielectric  to expose  the  WL  at  Metal  2  (Figure  3).  Tungsten  is  then deposited to make contact from the Metal 2 WL to VDD at Via 2 (Figure 4). Both the WL and VDD can be powered by one  of  the  AFP  tips  at  the  VDD  via  at  the  failing  bit location. 


With this single FIB edit, the AFP can now be used to probe the  BL,  BLB,  VDD/WL  and  VSS  vias  and  analyze  the failing  bit  cell  (Figure  5).  Figure  6  shows  the  electrical results  for  the  failing  bit  cell.  The  electrical  signature indicates that there was a resistive defect in path between the BL  storage  node  and  the  BL  contact  to  the  bit  line. Transmission  Electron  Microscopy  (TEM)  cross  section analysis  through  the  BL  storage  node  and  BL  contact identified a poly-silicon defect in the BL pass gate transistor. This  extra  poly  caused  an  increase  in  the  length  of  the transistor  channel  increasing  resistance.  The  physical analysis  results  matched  the  electrical  analysis  results produced by the AFP. 


153


Figure 2:  Ion beam  image of a 0.25 CMOS SRAM array. The Metal  3  bit  lines have been polished off  exposing  the Via 2 plugs. The failing bit cell location and the location of the WL/VDD FIB  connection at  the  edge of  the array are shown. 


Figure  3: Close-up  ion  beam  image  of  at  the  edge of  the array. A FIB hole was cut  through  the oxide  to expose  the Metal 2 word line. 


Figure 4: Ion beam image at the edge of the array showing how  tungsten  is  deposited  to  attach  the  word  line  to  the VDD Via 2 plug. 


Figure  5:  Topographical  AFP  image  of  the  top  of  Via2 plugs  after  the  removal  of  Metal  3  for  a  failing  0.25um SRAM  bit  cell.  A  FIB was  used  to  connect  the word  line (WL)  to  the  VDD  metallization.  Complete  bit  cell characterization was performed with the AFP at these Via2 plugs. 


Figure  6:  AFP  electrical  characterization  results  for  the failing SRAM bit cell. The bit cell flips data states when the bit  line  bar  (BLB)  p-channel  load  transistor  is  swept indicating a  series  resistance problem between  the bit  line (BL) storage node and the bit line connection to the bit cell based on Spice simulation models. 


Figure  7:  TEM  cross  section  image  of  the  failing  node shows a poly defect  in  the gate of  the pass gate  transistor. The  length  of  the  transistor  channel  is  increased  causing greater channel resistance just as the electrical analysis and Spice modeling had predicted. 


Ultra High Density SRAM Technologies (<100nm) 


Full  electrical  characterization  of  sub-100nm  high  density layout  SRAM  arrays  is  more  difficult,  but  can  also  be performed  with  the  AFP.  The  type  of  AFP  analysis described  in the previous section, performed on the 0.25um SRAM bit cell, can not be performed on this SRAM layout due  to  the fact  that probing at any of the vias at the bit cell level would  require more  than  four probe heads  to bias all the  nodes.  The  layout  does  not  allow  for  FIB  edits  to  be made  to  reduce  the  overall  number  of  nodes.  Therefore  a second approach had to be taken.  


The entire bit cell circuit  in  the ultra high density  layout  is contained  at  Metal  1  and  lower.  Any  defect  at  Via  1  or higher  would  produce  a  double  bit  failure  at  a minimum. Therefore, all the layers above Metal 1 can be ignored as the source  of  the  failure  in  the  analysis  of  single  bit  failures. Figure 8  shows a SEM  image of a  failing sub-100nm ultra high  density  layout  SRAM  bit  cell.  The  sample  was deprocessed to the top of Metal 1 with Via 1 still remaining. Inspection with a SEM did not  reveal a  short at  the  top of Metal  1  within  the  bit  cell,  eliminating  that  as  a  possible cause of the failure. However, metal shorts at the bottom of the Metal 1 layer or a resistive interface between one of the Metal 1 lines and its underlying contact would not be visible with  SEM  inspection.  To  eliminate  these  two  failure mechanisms  as  a  possible  cause  of  the  failure,  the  sample was polished to remove Via 1 and to planarize the very top of Metal  1  to  the  surrounding  oxide  so  that AFP  analysis could  be  performed.  Figure  9  is  the  SEM  image  of  the failing bit cell after the polish.  


Figure 8: SEM  image of a  failing 90nm ultra high density SRAM bit cell  failure. The sample has been deprocessed to Metal 1 exposing Via 1 and Metal 1. SEM inspection did not reveal a short or defect at the top of Metal 1. (SN = storage node and SNB = storage node bar) 


Figure 9: SEM of Metal 1 after polishing to remove Via 1 and to planarize Metal1and the ILD0 for AFP analysis. The AFP is now able to scan and probe the Metal 1 to determine if the contact to Metal 1 interface is resistive or if there are metal shorts at the bottom of Metal 1. 


The failing bit cell was scanned with  the AFP. Figure 10 is the topographical image of the failing bit cell and Figure 11 is the corresponding current contrast image produced by the AFP. The current contrast image would indicate if any of the underlying Metal  1/contact/active  interfaces were  resistive. Since all Metal 1  lines are visible, a resistive  interface was eliminated as a possible cause for the failure. Probing of the Metal  1  nodes  was  then  performed  to  determine  if  there were any metal shorts between metal  lines at  the bottom of the Metal 1. Probing between  the nodes of bit cell did not reveal  any  leakage  and  reconfirmed  the  lack  of  a  resistive interface  by  producing  normal  diode  curves  through  the connection of the Metal 1/contact interface to the underlying source/drain of the transistors. 


Figure 10: Topographical AFP image of Metal 1. AFP probing of  the adjacent Metal 1  lines within  the  failing bit cell  did  not  indicate  a  short  at  the  bottom  of  the metallization. 


Figure  11:  Current  Contrast  AFP  image  of  the  Metal  1 layer. The results showed that the Metal 1 storage node(SN) lines  do  not  have  a  resistive  interface  to  the  underlying contacts.  The  probing  and  current  contrast  imaging  has eliminated  a  defect  in  the  Metal  1  layer  as  the  possible cause the bit cell failure. 


Based  on  this  data,  it  was  determined  that  there  was  no defect in the Metal 1 layer causing the single bit failure. The Metal  1  was  then  removed  by  mechanical  polishing.  The transistors of  the  failing bit cell were probed with  the AFP 


[3].  The  AFP  results  showed  that  the  BLB  p-channel transistor  was  faulty  (Figures  12  and  13).  Current conduction was minimal  at  low Vds  levels. A TEM  cross section  analysis  was  performed  on  the  faulty  p-channel transistor, but no physical defect was  found. However,  the AFP  analysis  was  successful  in  identifying  the  faulty  pchannel transistor as the cause of the bit cell failure and was able  to  analyze  the  entire  bit  cell  from  the Metal  1  layer down to the transistor level. 


Figure 12: Traditional AFP probing on  the contacts  found a  p-channel  load  transistor  in  the  failing  bit  had  low conductivity at low Vds. Ids measured 1uA at Vds=0.2V. 


Figure  13:  Probing  with  the  AFP  on  the  contacts  of  a passing bit cell  found  that  Ids measured 6uA at Vds=0.2V for the p-channel load transistors. 


Case Study II: SOI CMOS Current Contrast Imaging 


Current contrast  imaging of bulk semiconductor devices on the AFP  is performed by  scanning  the exposed contacts of the  transistors with  the probe  tips biased (and  the well bias through the back of the die or using one the tips to bias the well  at  the  well  contact)  and  measuring  the  conduction through the tips as they make contact to the various features of  the device  [4],  [5]. When  the  tips are  touching oxide or one of  the  contacts  connected  to  the gate of a  transistor, a minimal  amount  of  current  is  conducted  through  the  tips. When the tips touch a contact connected to a source or drain of a transistor, significantly more current conducts due to the forward  biasing  of  the  source/drain  to  well  diode.  This information  is  then used  to  construct  an  image of  the  area scanned  to allow  the user  to quickly evaluate  if a  transistor gate is leaky, or see a missing source/drain contact thatís not conducting (Figure 14). 


Figure  14:  AFP  current  contrast  imaging  of  a  bulk semiconductor  device.  In  this  image,  the  n-well  has  been biased  to ground with one of  the probe  tips while another probe tip is biased with a positive voltage and scanned over the  failing  bit.  The  biasing  causes  current  conduction through the source/drains of the p-channel transistors to the well. A gate contact  is also visible due  to a damaged gate oxide that allows for current conduction to the well. 


Another method  to  perform  current  contrast  imaging  is  to use the optical microscope on the AFP to illuminate the area of interest with light while scanning the area with the probes biased  to ground. The  light causes  the generation of photoelectrons in the silicon causing the active to be biased. This allows  the  tips  to scan  the area and measure  the amount of conduction  through  the  contacts  without  the  need  of manually biasing the wells (Figure 15). 


Figure  15:  AFP  current  contrast  imaging  of  a  bulk semiconductor device using  the  light on  the microscope at high magnification  to bias both the n   and p doped silicon. The probe  tips are biased  to ground as  they scan over  the area of interest resulting in the conduction of current.  


This same technique can be used to perform current contrast imaging  on  SOI  CMOS  transistors.  Although,  technically there  are  no wells  in  SOI  transistor  technology,  there  is  a small  substrate  region  in  the  source/drain  areas  and  under the  gates.  When  exposed  to  the  highest  intensity  of  the microscope  light at  the highest magnification,  this substrate region  generates  enough  photo  electrons  to  bias  the 


source/drain junctions and allow enough conduction through the AFP probed tips to produce an image. 


Figure  16  shows  a  current  contrast AFP  image  of  a 90nm SOI CMOS SRAM array containing a failing bit cell using the previously described method. In  the  image, a contact  to one of  the  transistor gates  is visible. This  indicates  that  the contact  is  conducting  current  through  the  gate  due  to possible  gate  oxide  damaged. AFP  probing  confirmed  the gate oxide leakage, but TEM cross section analysis through the  failing  transistor did not  find a defect  (Figure 17). The information  obtained  by  AFP  analysis  was  sufficient  to allow  changes  to be made  to  the gate oxide process  in  the wafer manufacturing facility thereby correcting the single bit failures. 


Figure 16: AFP  current  contrast  imaging of a SOI SRAM array  using  the  light  on  the  microscope  at  high magnification  to bias both  the n and p substrate under  the gates. For  this  device,  a  gate  contact  is  visible  indicating leakage through the gate. 


 Figure 17: AFP probe results for the gate contact shown in Figure  16  shows  gate  leakage  to  the  source  of  the transistor. 


Case Study III: Light Emission and AFP Analysis 


AFP analysis in conjunction with light emission analysis can significantly  reduce  the  cycle  time  in  analyzing  failing semiconductor  devices.  Figure  18  shows  a  semiconductor device  that  failed  due  to  high  standby  current.  A  light emission spot can be seen in one of the circuits. The circuit location  generating  the  emission  was  identified.  Tradition micro-probing  was  not  possible  at  this  location  so  the sample was  removed  from  the package and deprocessed  to the  top  of  the  contact  layer. AFP  current  contrast  imaging indicated a problem with the source and drain of one of the transistors (Figure 19). Probing and electrical analysis of the transistor  found  that  the  source  was  leaking  to  the  well (Figure  20).  SEM  inspection  of  the  transistor  showed  no defect  even  at  the  substrate  level  (Figure 21). Planar TEM analysis was performed and a dislocation was  found  in  the substrate (Figure 22).  


This case study demonstrates  the power of AFP analysis  in conjunction with  light emission  tools. Past analysis of  light emission  sights usually  required  several days of  traditional micro-probing (FIB probe pads and micro-probe needles) if the probing was at all possible. AFP results were obtained in a single afternoon. 


Figure  18:  Light  emission  analysis  identified  an  emission spot  in  the  logic of a device  that  failed standby IDD. Light emission  results  provide  by  the  Freescale  Tempe  Product Analysis Lab. 


Figure  19: Current  contrast  AFP  image  of  the  transistor shows  that  the  source/drain  contacts  for  the  suspect transistor  had  a  different  contrast  than  the  surrounding source/drain  contacts  indicating  that  they were  leaking  to the p-well. 


Figure  20:  Two  probe  AFP measurements  of  the  suspect transistor showed that the source and drain were leaking to the p-well. 


Figure 21: The sample was deprocessed down  to substrate and  inspected with  the  SEM. No  contact  spike  or  silicide problem was found. 


Figure  22:  Planar  TEM  image  of  the  failing  transistor shows a dislocation in the substrate that starts at the trench on  the  Source  side  and  extends  across  the  Gate  to  the Drain.  This was  the  source  of  the  light  emission  and  the standby  IDD  failure.  The  combination  of  light  emission, AFP, and TEM analysis resulted in the determination of the failure mechanism in a relatively short amount of time. 


Case Study IV: AFP Measurements on Copper Metallization 


In  this  case  study,  the  AFP  was  used  to  probe  copper metallization  lines  of  a  90nm CMOS DRAM  device.  The device had  a double  column  failure. The  column  lines  run adjacent  to  each other  at  the Metal 1  layer.  It was  thought that  there was  a  short  between  the metal  lines  of  the  two columns. However, deprocessing and inspection at the wafer 


manufacturing facility did not find a metal short so a sample was submitted for AFP analysis to determine if the columns were shorted. 


Figure 23  is  the  schematic  for  the DRAM columns.  It was determined  that AFP measurements  could  be made  on  the copper Via 1 plugs connected to the metal lines for the  


failing columns 51 and 52. The sample was deprocessed  to the top of Via 1, but the sample was slightly over polished to the point where the remaining oxide above the Metal 1 lines was  too  thin  to support the vias. The FIB was used to clear an  area  of  the  remaining  oxide  and  expose  the  Metal  1 copper  lines  of  the  failing  columns  (Figure  25). The AFP was used  to probe  the metal  lines (Figure 26 and 27). AFP results verified that one of the bit lines for each column was shorted  to one of  the bit  lines for  the other column (Figure 26  and  27).  Probing  on  the  metal  lines  for  the  adjacent passing column 50 and failing column 51 showed no short. Physical  analysis  of  the  failing  columns  did not  locate  the cause  of  the  short,  but  it  was  demonstrated  that  the  AFP could  probe  copper  metallization  and  obtain  electrical analysis  results.  It  should be noted  that copper vias can be difficult to probe. The copper vias can be damaged with just the probe force of the AFP tips pressing into them making it difficult  to  establish  electrical  contact.  The  copper  metal lines  appear  to  hold  up  better  to  probing  which  makes probing  the  metal  lines  more  attractive  than  probing  the copper vias. 


Figure  23:  Schematic  of  the DRAM  columns  showing  the desired location to probe. 


Failing Transistor 


Figure 24: AFP topographical image showing the failing columns 51 and 52 after the FIB was used to expose the Metal 1 lines. 


Figure 25: AFP current contrast image showing the failing columns 51 and 52 Metal 1 lines are exposed and available for probing. 


Figure 26: AFP probe results shows leakage between Metal 1 lines of column 51 and 52. 


Figure 27: AFP probe results showing no leakage between Metal 1 lines of column 50 and 51 compared to columns 52 and 52 in Figure 26. 


Case Study V: Surface Roughness Measurements 


The AFP  is a surface analysis tool that creates an image by measuring  the  displacement  of  the  probe  tip  as  it  scans across  the  surface.  The  tool  does  have  some  capability  to measure  the  roughness  of  a  surface  even  though  it wasnít designed  specifically  for  that  purpose.  As  the  AFP  scans over  an  area,  it measures  the deflection of  the probe  tip at numerous  points  along  each  scan  line  and  the  data  is recorded. The tool is set to 100 data points per scan line and 100  scan  lines per  image. The  tool  takes  the data  for each scan point  and constructs an  image based on  the measured deflection  to  the probe  tip. Measurements  can be made by making  statistical  calculations  on  the  recorded  data.  The distribution is usually a normal distribution centered at zero after the data has been normalized (the zero point is relative during the scan). Measurements of the surface roughness can be  estimated by  looking at  the  full width at half maximum (FWHM) of the distribution.  


In  this  case  study, package  lead-frames were  submitted  for surface  roughness  measurements.  Lead-frames  are  the backbone  of  a  packaged  semiconductor  device.  The semiconductor device is glued on the flag of the lead-frame. Wire  bonds  are  then  attached  from  the  bond  pads  on  the semiconductor device  to  the  lead  fingers of  the  lead-frame. Finally,  a  mold  compound  material  is  pressed  around  the semiconductor  device  and  the  body  of  the  lead-frame  to form  a  packaged  device.  The  lead-frame  supports  the structure  of  the  package  and  electrically  connects  the semiconductor  device  to  the  outside  world  (print  circuit board). 


Lead-frames,  which  are  made  of  copper,  usually  have  a roughing  agent  sprayed  on  them  to  allow  for  the  mold compound  to  adhere  more  strongly  to  the  surface  of  the lead-frame. This roughing agent consists of an adhesive and particulates of a designated size. In this case, the size of the particulates  was  rated  at  ~2000  angstroms  Package engineering  requested  that  the  size  of  the  particulates  be verified by measuring with  the AFP. A  lead-frame with no roughing agent was also provided for comparison. 


Figures 28 and 29 show the lead-frames to be measured. The surface of lead-frame in Figure 29 appears bright due to the surface roughing agent that was sprayed on the surface. The flag  of  the  lead  frame  was  chosen  as  the  location  for measurement. The AFP  tips were placed on  the  flag and a 15x15um box was  scanned. The  topographical AFP  image of the surface roughness for each sample is shown in Figures 30  and  31,  and  the  distribution  for  each  scan  is  shown  in Figures  32  and  33.  The  measurement  of  the  surface roughness  at  the FWHM of  the distribution  for  the  sample with no roughing agent is +/-50nm. The measurement of the surface  roughness  for  the  sample with  the  2000  angstrom roughing agent is +/-0.2um (or +/-2000 angstroms) which is a  multiple  of  the  expected  size  of  the  particulates  in  the roughing agent. This indicates that the particles are not in a single  layer on  the  lead-frame but  are  stacked  at  least  two layers high.  


It was  found  the quality of  these  types of measurements  is improved by making  the scan area as  large as possible and reducing  the scan rate. However, doing so greatly increases the  time  to make  a measurement  so  a  trade-off  has  to  be made between accuracy and speed. 


Figure 28: Optical photo of a package  lead-frame with no roughing agent sprayed onto the surface. 


Figure  29:  Optical  photo  of  a  package  lead-frame  with ~2000A roughing agent sprayed onto the surface. 


Flag 


Lead-Fingers 


Figure  30:  Topographical  AFP  image  of  the  lead-frame with no roughing agent. 


Figure  31:  Topographical  AFP  image  of  the  lead-frame with 2000A roughing agent. The particulates can be clearly seen. 


Conclusion 


In  this  paper,  several  case  studies  were  provided  to demonstrate  the  versatility  of  the  AFP.  The  AFP  was originally  designed  to  probe  and  electrically  characterize transistors  at  the  contact  layer.    However,  the  needs  and demands of the failure analysis environment have quickly  


Figure 34: The distribution of the AFP measurements at the FWHM point gives a measurement of +/-50nm for the leadframe with no roughing agent. 


Figure 35: The distribution of the AFP measurements at the FWHM  point  gives  a  measurement  of  +/-2000A  for  the lead-frame with the 2000A roughing agent. 


expanded its use. These expanded capabilities make the AFP more valuable for the failure analysis community. 


References 


[1]  R.Mulder, S.Subramanian, E. Widener, T.Chrastecky.          ì Improved SRAM 6T Bit Cell Failure Analysis using         MCSpice Bit Cell Defect Modelingî , Proceedings of        the 29st International Symposium for Testing and        Failure Analysis,p.363, (2003). 


[2]  R.Mulder,  ì A Simple FIB Metod for Constructing  


       Elecrically Isolated Microprobe Pads for the Electrical         Analysis of Failing 0.12um Technology SRAM Bit         Cellsî , Proceedings of  the 30st International  


       Symposium for Testing and Failure Analysis, p.538,         (2004). 


[3.]  Jon  C.  Lee  and  J.  H.  Chuang,  ì Fault  localization  in contact  level  by  using  conductive  atomic  force microscopyî ,  Proceedings  of  the  29th  International Symposium  for  Testing  and  Failure  Analysis,  p.413, (2003). 


[4]  Terence Kane, Michael P. Tenney, ì Electrical       


       Characterization of  of sub-30nm Gatelength SOI  


       MOSFETsî , Proceedings of the 30th International         Symposium for Testing  and Failure Analysis, p.33,        (2004). 


. 


FA/LIT Instrument Adjustments for Successful Analysis of Packaged  Semiconductor Devices


Dr. Daniel J. D. Sullivan, Steve K. Hsiung and John Soopikian


LSI Logic Corporation, 3098 West Warren Ave., Fremont, CA 94539  Tel: (408) 433-6171; Fax: (408) 433-8193; Emil: dsulliva@lsil.com


Failure Analysis Laser Inspection Tool (FA/LIT) is a tool for  analysis of packaged devices [1], [2]. FA/LIT uses an Nd: YAG  laser to ablate material from packaged microelectronics. Of  specific interest are the exposures of bond wires and stitch  bonds in molded BGAs and PQFP parts and traces in the  substrates of BGAs.  The operation removes molding  compound or solder mask by ablation to expose the  underlying area of interest as shown in Figure. 1.  With proper  setting and exposures, the underlying metal components are  unaffected by the laser and remain intact. Inspection of the  exposed area(s) or resistance measurements to the solder balls  or other areas exposed by the FA/LIT may then be done.


Figure 1: Molded BGA before and after FA/LIT. Note  exposure of traces under the solder mask and encapsulant.  Also exposed: bond wires, stitch bonds, solder mask, and die.  The areas exposed can be of various shapes, as shown by the  circle and polygon regions ablated in the encapsulant.


Differences in materials, package configurations, technologies, and requirements for electrical functionality of  the devices have required adaptation of standard settings and  configuration of the instrument. The removal of molding  compound and solder mask materials to expose stitch bonds  and substrate traces without alteration of the metals is key to  successful inspection of the device. FA/LIT can routinely  expose bond wires for inspection as shown in Figure. 2. However, concerns develop for the exposure of stitch bonds, the examination of small trace cracks, and any requirements to  maintain electrical functionality of devices.


Improper set up of the FA/LIT can induce: lifted stitch bonds, trace lifting and cracking, and electrical failures in the devices  being examined.


Figure 2: Optical image of exposed bond wires, stitch bonds, and traces in a BGA packaged device.


Assembly operations, reliability testing, or field use may  induce defects in a semiconductor device [3]. Typically the  failures of interest include lifted ball bonds, cracks in substrate  traces or the solder mask under mold compound, and shorts  between bond wires.  Other operations may involve the use of  the FA/LIT for breaking a trace or bond wire to allow  electrical testing of the unit without this connection, separation of shorted bond wires, and preparation for decap.


When failures are exposed by the FA/LIT it is often necessary  to also expose similar good areas to ensure the observed  defects are not artifacts induced by the laser.  An example of a  subtle laser induced failure is the popping of stitch bonds.  If  the stitch bonds are exposed and further hit by the laser, the  bonds quite often fail (pop).  False identification of lifted  stitch bond is easily avoided by examination of 1) the part  after it is just exposed by the FA/LIT, 2) adjacent known good  bonds, 3) known good stitch bonds on another location of the  part or on another part after the same FA/LIT treatment.


## FA/LIT Instrument Adjustments for Successful Analysis of Packaged Semiconductor Devices


163


Figure 3: Just exposed stitch bonds wire (left), and the same  location after further laser exposure (right).


When it is established that the defects are real, then FA may  make recommendations regarding changes to the materials set  or engineering of the devices.


Methods and Analysis


Cracks in traces, lifted or touching bond wires are sometimes  detected by other analyses such as: x-ray, SQUID, or TDR. [4],


[5], [6] Other times they are missed (this often depends on the  quality of the instruments) or such instruments are not readily  available.   Confirmation that trace crack or lifted stitch bonds  are real and/or completely open requires the area to be  exposed and a resistance measurement be made across the  defect.  A resistance check from the point just past the  observed defect to the solder ball/lead of the package may be  needed to ensure that the observed defect is the only failure  present and if it is resistive or open.  This is done to eliminate  the possibility that another open further along the trace or in  vias inline exist.


Figure 4: FA/LIT exposed crack. The same area after five  additional exposures to the laser; the crack is unaffected and  remains easily identifiable (no healing of the crack occurs).


The settings on the FA/LIT include: LaserCurrent (the current  used to generate the laser pulses), LaserQSwitch (the quality  setting of the beam), Fillspacing (the step size taken by the  laser between pulses), and FillStyle (the step pattern the laser  takes to fill the area indicated on the sample).  These need to  be set to match the operation and material of the sample.  The  system default settings along with settings for several different  materials are in Table 1.


Laser Current Q Switch Fillspacing FillStyle


Default


18 A


0.0762


Both@


PQFP


20 A


Both


Glob Top


Molded  BGA


SM A*


SM B


Ceramic


26 A


* SM – Solder Mask, brands A and B. @ Both cross and  racetrack fill styles are used to reduce patterning.


The variation of the parameters from the ideal result in several  kinds of failures in the process.  If the current is too high: the  organic materials burn, traces are lifted and crack, and stitch  bonds break.  If the current is too low the organic material  popcorns but is not removed.


Figure 5: Current settings on left are ok and on right too  high. The traces on the right have no support and are hanging  free.


Figure 6: Traces shown on left with a good fillspacing (0.07) and on right with poor fillspacing (0.2).  Note the material  remaining in the center left and the stripes in the right image.


The laser pattern even with good Fillspacing will leave ridges  on the part where the laser overlap does not remove material  as well.  The solution is to move the laser box slightly with  respect to the sample between shots.


Figure 7: Too low a power will popcorn the organic material  but not remove it.


Usually, FA/LIT is used in the final stage of failure analysis  when the electrical integrity of the part is no longer important.  However, in package development issues often the electrical  integrity is often a critical issue for parts examined by the  FA/LIT.


In one experiment several parts needed a cut in the power ring  in the substrate.  FA/LIT was used to remove mold compound  to expose the power ring to allow access for making the cut  without breaking the bond wires.  After the power ring was  cut, the parts were re-sealed with Hysol and then electrically  tested to determine the effect of the operation.


These parts failed functional test 100% although they passed  continuity test, demonstrating the bond wires remained intact. The exact mechanism causing the failures was unclear.  So  two experiments were done to try to understand and eliminate  the problem.


First, a copper plate was added to the plastic FA/LIT sample  stage and this was grounded to the instrument chaise (Figure 8  and Figure 9).  Further parts run through the FA/LIT process  all passed electrical test.


Also the failing parts were baked at 100ºC for 5 minutes and  then O2 ashed in plasma for 10 minutes. These parts recovered  and passed electrical test. The indication of these two  experiments is that the electrical state of the parts is affected  by the FA/LIT process.  The process places the parts into a  reversible electronic state that the causes failure in the  electrical tests.   Parts are known to fail if not properly  conditioned prior to electrical test.


The grounded sample holder prevents the part from going into  an unwanted state or allows return to a preferred state during  the process.  The plasma allows return of the part to the  preferred state.


Figure 8: Image of grounding setup


Figure 9: Image of sample in grounding sample holder with  DUT.


Matching the FA/LIT settings based upon operation and  sample material is critical in achieving good exposure of areas  of interest with minimal damage.  The use of practice samples, or areas away from the area of interest, to verify results before  operations on actual FA parts is strongly recommended.  This  is an excellent method for examination of Stitch bonds, package traces, and bond wires.  However care must be taken  to avoid inducement of false failures.


The installation of a grounded sample holder has been shown  to greatly improve electrical integrity of samples during the  Laser ablation procedure.   Use of the grounding sample  holder improved electrical test results from 0% pass to 100% pass in advanced CMOS devices.


Metal Plate


Chaise


Copper Wire


Sample Holder


We wish to thank Dr. Andrew Komorwski and May Soe for  their work on the early characterization of the FA/LIT  operations in our lab.


[1] Pacheco, M.; Wang, Z.; Skoglund, L.; Liu, Y.; Medina, A.; Raman, A.; Dias, R.; Goyal, D.; Ramanathan, S. "Advanced Fault Isolation and Failure Analysis  Techniques for Future Package Technologies." Intel  Technology


Journal. http://developer.intel.com/technology/itj/2005/volume09 issue04/art07_advfaultisolation/p01_abstract.htm


(November 2005).


[2] Lars Skoglund and Rajen Dias, “Laser Milling  Techniques for Stacked Die Package Applications,” ISTFA 2004, pp. 369-375.


[3] E.A. Amerasekera & F.N. Najim, "Failure Mechanisms  in Semiconductor Devices", 2nd Ed., Wiley, NY, 1997


[4]  “Failure Analysis of Short Faults on Advanced Wirebond and Flip-chip Packages with Scanning SQUID  Microscopy”, Steve Hsiung, Kevan Tan, et al, 2004  International Symposium for Testing and Failure  Analysis Proceeding, pp. 73


[5] Failure analysis of BGA package by a TDR approach Ming-Kun Chen; Cheng-Chi Tai; Yu-Jung Huang; IChih Wu Electronic Materials and Packaging, 2002. Proceedings of the 4th International Symposium on  Volume, Issue , 4-6 Dec. 2002 Page(s): 112 – 116


[6] L. A. Curiel, A. J. Komrowski, D. J. D. Sullivan,


“Backside Application of Acoustic Micro Imaging


(AMI) on Plastic Ball Grid Array (PBGA) and Plastic


Flat Pack (PQFP) Packages” ISTFA 2004 Proceedings, pages 389-392.


Coupling C-AFM with Nano-probing Technique for Further  Junction Leakage Analysis


Cha-Ming Shen, Tsan-Chen Chuang, Chen-May Huang, Shi-Chen Lin, Jie-Fei Chang


1,Nan-Ke North Rd., Tainan Science Park, Tainan, Taiwan, R. O. C.


With the evolution of advanced process technology, failure  analysis has become more and more difficult because more  defects are of the non-visual type from new failure  mechanisms. In this paper, a novel and effective methodology  which couples the Conductive Atomic Force Microscope (CAFM) with nano-probing technique is proposed to reveal  some particular failure modes which were not observable and  difficult to identify with traditional physical failure analysis (PFA) techniques.


C-AFM is a popular tool to determine dielectric film  characteristic and junction behavior by its specific tunneling  current measuring mechanism with repeatable precision. Since, it is able to plot the I-V curve of the target accurately, it has  become a powerful technique for analyzing high-resistance or  leakage issues [1].  Figure 1 shows the schematic framework  of the C-AFM measurement system.


Figure 1: Schematic framework of C-AFM measurement  system


Another modern tool is the Nano-probing system which  comprises four needles with a merged probing-station and  attached to the specimen stage of a scanning electron  microscope (SEM). The  measurement instrument is a  programmable curve tracer. The nano-probing technique was  set up to measure the full transistor characteristics.  The basic  MOS parameters, such as threshold voltage Vth, off-state  current Ioff, saturation current Isat had to be characterized by  four terminals, i.e. gate, drain, source, and bulk as shown in   Figure 2.


Figure 2: Measurement of MOS parameters using the Nanoprobing system


Utilization of the Nano-probing technique has not only  provided prompt electrical data feedback required for yield  enhancement but also  to detect global parameter shift by  process issue, previously known as wafer acceptance test (WAT) [2].


In this paper,  the capability of coupling C-AFM with Nanoprobing technique is used to distinguish cases with suffer  general junction leakage or gate leakage from those that from  the  fake junction leakage or gate leakage cases.


## Coupling C-AFM with Nano-probing Technique for Further Junction Leakage Analysis


167


Experiment and Analysis


In our experiment, the sample was manufactured by the  advanced 65nm SRAM process. The schematic circuit of a  standard SRAM cell is shown in Figure 3. The sample suffers  from Vcc_min failure and the MOSAID tester provided the test  datalog for fault diagnosis and classified it as a read/write  failure.


Figure 3: Schematic circuit of a standard SRAM cell.


The sample was polished and deprocessed to the contact layer.  The SEM is operated in passive voltage contrast mode (PVC) and the PVC micrograph is shown in Figure 4. A storage node  and a poly contact at the located failure bit were found to be at  a brighter contrast than normal one.


Figure 4: SEM PVC micrograph with 1keV e-beam energy  showing  the marked storage node and neighbor poly contact  with  brighter than normal contrast at the located failure bit.


Then, in order to distinguish the leakage path and get more  electrical information for succeeding PFA, the C-AFM tool  was utilized to acquire the current mapping and plot the  associated I-V curves of the storage node and neighbouring  poly contact shown in Figure 5.


Figure 5: C-AFM I-V curves of storage node and  poly  contact


Failure storage node  and Poly contact


According to the C-AFM results, the sweep current of the  storage node showed a little larger than normal on the reversebias side indeed. But the other sweep current at the suspected  poly contact seemed to be normall, although there was an  obvious abnormality in SEM PVC micrograph. However, the  Transmission Electron Microscope (TEM) micrograph in  Figure 6 shows an obvious salicide spike under the localized  storage node. The abnormality is highlighted in the red box in  Figure 6.


Figure 6: TEM micograph showing abnormal spiking salicide  under the located storage node


Besides, considering the R/W operation of the circuit, such a  small leakage may be the root cause of the read failure, but it  is insufficient to verify the write failure. Because of this, there  would be another abnormality associated with the apparent  spiking contact.


In order to verify the failure mode, Nano-probing was used to  measure more characteristics of the sample.  An artifact  associated with the junction leakage and an irregular Id-Vd curve was discovered at the localized NMOS with the brighter  PVC in Figure 7.


Figure 7: Failure and reference Id-Vd curves show an extra  current component due to the leakage.


Next, the off-state current components of target were  extracted and shown in Figure 8.  It was obvious that one of  the major failure mechanisms was due to quasi punch-through  from drain to source. And there seemed to be no gate oxide  integrity  (GOI) issue although an irresistible gate current was  induced by a larger voltage difference of Vgd (nearly 1.15 V).


Figure 8: Off-state current components of failed NMOS show  that major leakage current was from drain to source.


Thereupon the  Id-Vg  curves under variant biased conditions  were compared and shown in Figure 9 and 10. In which a  drain induced band-to-band leakage (DIBL) combined with a  gate induced drain leakage (GIDL) phenomenon was revealed  on the targeted NMOS. So such defect location was near the  channel of transistor was solid, but a thinner gate oxide or  poor dielectric quality was not a concern.


Failure


Figure 9: Comparison of Id-Vg curves for the failed NMOS  and reference when Vd=Vs=0.


Figure 10: Comparison of Id-Vg curves on different bias  conditions for the  failed NMOS.


In a previous junction leakage episode which was measured  by C-AFM in a prior step, there was only an artifact due to  DIBL of this failed device.


Combining all above results, it would appear that this failure  is induced by a tiny abnormality hidden between the corner of  active region and shallow trench isolation (STI) edge, and  maybe the serious DIBL was due to both the mutual capacitor  effect from drain to substrate and the punch-through from  drain to source as shown in Figure 11.


Figure 11: Failure was induced by a tiny abnormality hidden  at the corner of STI and active area.


Finally, TEM was used to demonstrate the reasoning after  adjusting the location of cross-section. In Figure 12, the Zcontrast illustrate spiking salicide and the existence of  affiliated residue between drain and source of the suspected  failure NMOS. The quasi punch-through leakage was induced  by the strong coupling effect between drain, source and  substrate when larger voltage difference is applied.


Figure 12: Enhanced TEM Z-contrast image showing the  hidden defect observed at the located failure bit.


The use of C-AFM and Nano-probing has allowed us to  understand the mechanisms associated with the apparent  junction leakage and fake gate leakage. Sometimes, the  measurement from PVC or C-AFM mapping does not provide  an adequate explanation of the mechanism  because it is too  general. This new methodology has allowed us  to discover  the contradiction between our earlier hypothesis and the  failure model, and to collect more electrical information, would be able to lead us to revise and understand the  cause of  the failure.


In order to overcome the difficulty in detecting very tiny or  even invisible defect, an effective method was to reason the  failure mechanism and consider the location of defect from  detailed electrical information before the most conclusive PFA  was developed.


In this paper, C-AFM was used to detect the abnormal  contacts quickly and Nano-probing could provide the precise  electrical characteristic further. Then, combining these variant  measuring results, the favorable tactics can be adopted to deal  with different states. Because a compound and mutual  mechanism could be dismembered to analyze, the capability to  identify very tiny or complex failure mode would not only  limit to distinguish the leakage or high-resistance under  abnormal contact. [3]


[1] Welland, M.E.; McKinnon, A.W.; Barnes, J.R.; O'Shea, S.J., Engineering Science and Education Journal, Volume  1, Issue 5, Oct. 1992, pg 203 – 210.


[2] C. Giret and D. Faure, “Electrical Characterization by  Sun-Micron Probing Technique on 90nm CMOS  technology for Failure Analysis”, Proc.  IPFA 2004, pg  271 - 274.


[3] J.H. Chuang, Jon C. Lee “fault isolation in contact level  by using conductive atomic force microscopy”, Proc  ISTFA 2003, pg 413 - 418.


Mixed-Signal Test Software Generation Process –


Open Environment, Software Engineering Methods and Tools for Improving  Quality and Productivity


Stefan Vock 1, Hans Martin von Staudt 2


1 SEPT Europe, Hausergasse1, D-82065 Baierbrunn (München), Germany


email: stefan.vock@septeurope.com; Tel: +49 (0) 89 / 622 99 881


2 Dialog Semiconductor, Neue Strasse 95, D-73230 Kirchheim/Teck, Germany  email: hansmartin.vonstaudt@diasemi.com


Typical mixed-signal ICs are approaching 1000 or even more  parametric tests. These tests are usually coded in a procedural  or a semi-object oriented language. The huge code base of the  programs is a significant challenge for maintaining code  quality which inherently translates into outgoing quality.


The paper will present software metrics of typical mixedsignal power management and audio devices with regard to  the number of tests conducted. It will be shown that classical  ways to handle test programs are error prone and tend to  systematically repeat known mistakes.


The adoption of selected software engineering methods can  avoid such mistakes and improves the productivity of the  mixed-signal test generation. Results of a pilot project show  significant productivity improvement. Open-source based software is employed to provide the necessary tool support. They  establish a potential roadmap to become independent of  proprietary tester specific tool sets.


Despite lots of efforts and approaches to generate stimulus for  mixed-signal testing in an automated way as ATPG does for  digital testing, today’s main stream methodology still is  parametric testing for the specified behaviour and  performance. Numerous methods for automatic test stimulus  generation have been suggested but none have gained wide  spread acceptance yet. Other techniques [1, 2] are using  specifically calculated stimulus to test various properties items  in parallel. But even if these techniques are employed they  require correlation to a “traditional” test method. Hence the  test engineer still is in charge to stimulate the device and  measure the responses by the means of his test program i.e. the  test software.


Productivity within the test program engineering process is  another topic this paper will address. Some ATE vendors are  pursuing a roadmap to establish a high-level tool like Excel or  graphical approaches to control the test flow [3, 4]. Even  though they make the test flow and the limits transparent and  easy to maintain, the whole complexity of device setup and  measurement is just delegated to the level below, which again


has to be described by the means of a programming language. Furthermore it introduces a break in the tool chain, so it is  unclear whether such an approach is able to improve  productivity and quality for complex mixed-signal devices.


Another challenge for all users of ATE is the multitude of  languages being used. All kinds of languages have been  employed: besides Basic, Pascal, C, C++ and Java various  proprietary language extensions have been introduced. Consequently nearly every ATE vendor is using a different set  of language, compiler/interpreter, debugger, etc. Migrating a  test setup from one ATE system to the other is associated with  significant manual effort. This has been highlighted by the  ITRS roadmap [5] but up to now there is very little progress. With the growing size of test programs it is indispensable to  introduce methods for assuring software quality. Interestingly  the quality criteria for test software are based on assessing the  measurement quality of a test setup like Gr&R (Gauge  Repeatability and Reproducibility) [6]. This is required but not  sufficient. If the devices used for the acceptance procedure  don’t fully challenge the logical behaviour of the test program  any remaining flaw will eventually later show up in high  volume production. Especially multi-site testing is susceptible  to logical errors when one of the sites is failing.


Facing these challenges it is not only consequential to apply  software engineering methodologies to the process of  generating test programs to increase quality, but also provide  the corresponding tools (see section 5) to support them and to  show how efficiency and productivity can improve. But also to  provide the necessary tool support open-source based software  is employed. They establish a potential roadmap to get away  from proprietary tester specific tool sets.


Test Software Metrics


Typical examples for mixed-signal testing are power  management and audio chips as found in mobile phones. They  increasingly integrate most of the analog base band  functionality. This usually comprises a charger, various linear  and switching regulators, the audio functions like voice and  HiFi CODECs and microphone and speaker amplifiers. These  chips can be seen as a conglomeration of mixed-signal


## Mixed-Signal Test Software Generation Process – Open Environment, Software Engineering Methods and Tools for Improving Quality and Productivity


172


functionality that for various reasons is not integrated into the  digital base band processor chip.


Table 1 lists a number of power management and audio ICs  which are in production or are production ready. To compare  the size of test programs it must be set in relation to the  number of tests conducted which reflect the general  complexity of the device. This is indicated with the complexity  grade rating. Lines of code (LoC) has been chosen as the  easiest way to measure the size of a program. The ICs are  listed in historical order.


It should be mentioned that these numbers do not include any  factory automation code (data logging, handler communication, equipment monitoring), which is maintained by a  completely different group of engineers and is independent  from the device’s complexity.


As expected program size scales with the number of tests and  the complexity of the device. In average a number of about 44  lines of code per test has been determined with a tolerance  band of ±10%. Only one project constitutes an outlier with a  50% higher number of code lines per test. Complexity-wise  there is no obvious explanation. Investigations revealed a far  more verbose programming style of the respective test  engineer. The other four consistent results belong to three


different test engineers.


Productivity vs. Quality


Error Inheritance


The easiest way to increase productivity is to reuse code  fragments or the whole test program of a given device and to  modify it until it can be applied to the new type of device. This  approach is straight forward and followed rather often, especially when the test program has to be generated by an  external subcontractor. The big advantage of this reuse  strategy is that the program code for a given device is selfcontained, it does not contain dependencies to other entities (functions, modules) that are part of other programs. Small  organisation will draw benefit from the easy way of assigning  the responsibility for test setups to individual test engineers  who in turn have full control of all the code.


Perhaps the biggest disadvantage of reuse by copying is the  inheritance of errors. When the next project is started based on  the copy of the previous one it automatically inherits all errors  which are not yet debugged. Figure 1 depicts this process.


A hidden bug (marked by a light grey ‘X’) is part of the  original test program. The third revision finally is the one  where the bug becomes obvious (dark ‘X’) and finally is  removed. Unfortunately a new program was started before as


Rev 1 X


Test Program A


Test Program B


method copied


Test Program C


method merged in


method copied method


copied


Test Program D


Bug becomes obvious and is fixed


Bug history becomes untraceable


Bug continues


to exist


New programs are started as copy from predecessor


Test program revisions


over time


Rev 2 X


Rev 3 X Rev 4 X Rev 5 X


Rev 1 X Rev 2 X Rev 3 X Rev 4 X Rev 5 X Rev 6 X


Rev 1 X Rev 2 X Rev 3


Rev 1 X Rev 2 X Rev 3 ?Rev 4 ?


Figure 1: Inheritance of “legacy” bugs


Complexity grade


IC / test program (different power  management ICs)


Lines of code (LoC)


Number of tests


LoC per test


Power


Audio


(A)


17,385


424


41.0


(B)


23,510


356


66.0


(C)


31,110


672


46.3


(D)


23,604


599


39.4


(E)


20,790


438


47.5


Table 1: Test program size in relation to tests conducted


copy of the second revision including the bug. So it lives on  and can spread. If code merging from various programs  happens the history of bug inheritance becomes untraceable.


As there is usually no control about the copy mechanism and  no organisational link between the independent test program  projects, errors that were thought to be extinct come back  again and again.


A better approach is to organise test programs into library  elements. Reuse is not applied to complete monolithic test  programs but to individual library elements which correspond  to building blocks in the devices to be tested (e.g. linear  regulators, switching regulators, charger, audio amplifier, CODEC, …).


As depicted in Figure 2 a test program is to be built up from  these library elements. Firstly this promises a productivity  improvement. Secondly and even more important is the fact  that every library element has a revision history on its own. Whenever a new test program is brought up it is created from  the recent version (head of development) of the library. That  means that any enhancements of the library for a new product  have to be provided by the testing expert.


The disadvantage associated to such an approach is clear as  well, it creates interdependencies between many more people  than before. The easy one-to-one relationship between test  program and test engineer no longer exists. Also psychological  barriers have to be overcome when reassigning responsibilities  from the product oriented engineer to the expert. Furthermore  bug fixing must be restricted to the expert such the cleaned  version becomes head of development.


Test  Prog  Product A


Lib 1


Testing Expert 1


Test  Engineer  Product  A


Test Prog ProductB


Test Engineer


Product B


Lib 2


Testing Expert 2


Figure 2: Test programs built from library elements


Software Engineering Methods Adopted


Coding Conventions and Reviews


Applying coding conventions is a base step in the process of  quality and efficiency improvement for a number of reasons.


1. Typically 80% of the lifetime cost of a piece of software  code goes into maintenance [7].


2. Especially with the view on the used library concept, the  enforced improvement of the readability of the software  code, allows the team members to understand new code  more quickly and thoroughly.


3. Hardly any software is maintained for its whole life by  the original author.


Code reviews are used to establish the coding conventions and  to continuously advance the users coding skills. Such the  source code’s quality gets assessed as it becomes part of the  overall quality of the shipped product. The adopted coding  conventions were derived from GNU coding conventions [8].


Rev 1


Library 1


methods referenced


Bug is recognized


Bug free method is referenced


Bug is extinguished


forever


New programs are started from the libraries


Revisions over time


Rev 2


Rev 4


Rev 5


Rev 6


Rev 1 Rev 2 Rev 3


Figure 3: Single Point of Failure & Enhancement Benefits


Rev 1 !Rev 2


Updated to head of


development


methods updated


Feedback to Test Expert


Redundancy Free Coding


Having this rule set within the coding conventions, redundancy  free coding becomes to single point of failure within the source  code. There are no multiple places within a project anymore  where to fix the same type of bug several times. As soon as  two lines of source code are repeated twice, moving this code  into a function solves this redundancy. However, this is the  ideal single point of failure approach. Within the given  environment there is room for personal judgement given.


Based on the “copy of source code method”, diagrammed in  Figure 1, the redundancy free coding rule together with the  library concept result in a different scenario, see Figure 3. The  test program A calls test method functions from the Library 1. The test engineer working on test program B discovers a flaw  in the referenced library method.  Based on the feedback via  the provided tool Bugzilla [9] ( see Section 5.4 ) the flaw is  extinguished forever by the test expert. Existing test programs  could be updated now to the library head of development. New  developments, test program C, will automatically benefit from  enhancements.


Unit-Tests: Test the Test Software


The concept behind unit tests is to generate test cases for all  methods and functions within the source code. These test cases  are then applied to the library elements for automatic  verification every time the source code is modified, to ensure  the original functionality is still maintained.


For test functions that call measurements on ATE some  specialties have to be regarded. It is normally not acceptable to  consume tester time for pure software verification purposes. Thus the emulator software which is available for most ATE  systems has to be used together with a predefined response  file. Unfortunately the authors have observed in particular for  recent platforms that the full equivalence between emulator  software and ATE is not guaranteed.


Figure 4 depicts how these three presented elements work  together to achieve better software quality.


Further Methods


Further adopted software engineering methods are linked and  included into the set of tools, described in the next chapter.


Tools


Open-Source vs. Commercial Tools


After picking software engineering techniques for test  program generation it is logical to also consider the tools  being used by this community. Besides various commercial  offerings the open-source based tools are of particular  interest. Their greatest advantage lies in the openness, which  allows adaptation to the specific needs of test engineering.


Figure 4: Software Engineering Methods Benefits


Apparently open-source is coming for free but its openness to  reconfiguration or even change also comes for a price: Usually  a consultant or service company is required to provide the  desired configuration. Nevertheless the achieved solution can  then be replicated any arbitrary number of times. If used on a  standard PC this constitutes a very reasonable working place  for a test engineer, open to any kind of enhancement.


Required Functionality


Figure 5 shows the three layers of functionality that need to be  integrated. The foundation layer is built up from functions  which apply to any program development process. Configuration and release management, bug tracking and  change request management are required in any serious  development process. They should be described in quality  procedures governing the process. From a corporate  perspective there is no interest at all for these function to  change unless a process improvement is desired. The tools


Figure 5: Tool functionality on different layers


Software Engineering Methods


Software Quality


improved


Coding Conventions Redundancy Free Coding Unit Tests


Readability


Maintainability


Single Point of Failure Modules Error Free


Software Engineering  Methods


Source Code


Coding Conventi


Redundancy Free i g  Unit t


adability


intainability  Single Point f il re  Modules rr r ree


Waveform  viewer avefor  vie er


Hardware  debug tools ard are


debug tools


Editorditor


Source code  debugger ource code  debugger


Docu -mentation


ocu -


entation


Configuration  and release  management onfiguration  and release  anage ent


Bug tracking ug tracking


Change


request  management hange


request  anage ent


Eclipse IDE


ATE


specific


plug-ins


Language


Change according  to technical


progress


Development  process  specific  plug-ins


Unit testnit test


W f r


i r


H r ware    d


t ols


Edit r


So  de  d


D   ment ti


Bug  tracking


i se IDE


Change only if  development


process requires


U it t t


Change request   management


used at this layer have to be identical for all ATE platform in  use, today and tomorrow.


The medium layer is language specific and contains source  code aware editor, the debugger and the automated  documentation tool. Also unit test tool resides here. Progress  in this layer should only happen if a shift to a new language  promises improvements in productivity or quality (or both). It  should be allowed to happen but rarely.


The upper layer is open to any ATE specific, technically  driven progress. As these plug-ins are loosely coupled to the  base functions changes can be applied easily.


Integration Platform


Having access to tools on their own is not necessarily  productive if they are not integrated into one consistent  workspace. This workspace has to be setup, enhanced and  customized in a way that the test engineer is always working  within in the same environment, very much independent from  the tester platform type. Using a common workspace results in  familiarity with the tools, their features and their handling, making the source code development, project handling and  debug much more effective.


Tools Employed


The ATE platform was a Credence Quartet running SunOS.  It  was chosen as the vendor’s development tools offered very  little comfort and integration. Furthermore this type of ATE is  programmed in plain C thus facilitating the integration of the  language specific tools.


The engineer’s PCs were just standard, equipped with 1 GB of  RAM.


Eclipse [10]


Eclipse is the used integration platform, providing the  workspace in which all other tools are integrated. It also comes  with a source code editor, with a wide range of powerful  source code and project handling functionality. This ranges  from simple functions like source code highlighting, over  function cross reference handling up to all kind of support for  the source code developer, all what is needed.


The plug-in mechanism of Eclipse makes it suitable to  integrate any current and upcoming requirement. Such the  tester specific tools of the Credence Quartet (shmoo tool, pattern editor, level editor) were made accessible by click on a  button. The Cygwin/X environment provides the necessary Xwindows emulation. Based on this tool set the resulting  workspace integration overcomes the  operating system barrier  between the different ATE platforms and the eclipse  workspace with the tool set.


All other tools listed below are plugged into Eclipse using  predefined and readily available plug-ins.


Subversion [11]


Subversion is the employed version control system. It is  integrated within the Eclipse workspace for the version control  for each project on a per file basis within the project. Furthermore this tool allows several engineers to work on the  same test program project, even on the same file in parallel  resolving the changes as long as they don’t overlap.


GDB: The GNU Project Debugger [12]


Current tester platforms come along with a source code  debugger. This ATE specific debugger (Codecenter) got  integrated into the Eclipse workspace. However, it is license  based and not the state of the art source code debugger  anymore. Due to this, GDB was integrated as well into the  Eclipse workspace and customized to handle the SunOS based  test program source code.


Bugzilla [9]


Bugzilla was integrated into the workspace environment for  change and enhancement request management. This applies  primarily to the libraries providing the test functions on a per  block type basis but also for the test program itself.  In  addition the features provided by Bugzilla are the basis to  track external requests, to assign and to guide the follow up of  tasks and to improve communication between the team  members on remaining issues that might affect the quality of  the test setup.


CppDoc  [13]


Proper documentation plays an important role in achieving the  goal of high quality source code within a team. All relevant  aspects regarding available functions have to be accessible  online. As part of the coding conventions it is specified that all  functions and their parameters need to be described in a  special comment format structure. CppDoc generates  automatically, on a mouse click, a HTML based  documentation for the specified projects, based on the  comments in the source code itself. This documentation offers  features like active index, search functions, relationship and  hierarchy links.


CUT C-Unit Tests[14]


To support the handling of these unit test cases the tool CUT (C Unit Test) was chosen from the available range of unit test  tools. This selection was based on the need for the tool to run  on SunOS based ATE systems as well and the ability to  generate the process logic as needed. Currently the final  implementation and usage of the unit tests is ongoing due to  extra challenges  in conjunction with the emulator of the used  ATE platform.


Table 2 lists the ICs and the corresponding test setups that  have been handled by pilot project. Again they are ordered  chronologically. Man effort is given relatively to the first test  program which is set to 100%. In addition to the man effort  directly invested into the test programs another 30% effort  went into the open-source tool chain configuration.


Tremendous differences in effort spent and productivity can be  observed. The first test program obviously worked as a pipe  cleaner. Productivity and program size are not significantly  better than the traditionally coded programs. It is suggested to  review a rework this program.


But the second test program can already leverage the work  invested in its predecessor. Man effort and code size go down  significantly. Even though the overall break even is not  achieved before the third test program is completed as well, it  becomes clear that the software engineering based approach to  generate test programs is successful in terms of productivity.


With respect to quality no proof of improvement can be given  yet. But from the methodologies used it can be expected that a  significant progress has been achieved


Conclusion and Outlook


This paper has shown that it is not only possible but  recommended to introduce software engineering  methodologies to the process of generating test programs. Productivity and quality improvements come along with it. The productivity improvement is the major point addressing  the need to significant reduce the time to marked of a test  application. The quality enhancement is the basis to meet the  continuously increasing quality measures from the customers. It also reduces the needed maintenance effort during the life  cycle of a test program. This frees up resources for other tasks. We consider Eclipse to be a well suited platform to integrate  ATE specific extensions while building up on a foundation of  general infrastructure and productivity tools that are required  to build a reliable, repeatable software generation process.


Therefore we would like to encourage the interested  community to discuss and eventually to pursue this direction. The adoption of open-source based tools by ATE vendors is  possible and probably cheaper than pursuing own routes of  proprietary languages and tools. It might require a cultural  change to more openness.


Only if enough momentum is gathering behind such a viable  technical solution the major concern of the ITRS roadmap [1] can be addressed.


The authors would like to thank Andreas Schmid of  EXCELSIS AG for the software engineering inputs and the  project team whose effort made the results possible.


[1] P.N. Variyam and Abhijit Chatterjee, “Enhancing test


effectiveness for analog circuits using synthesized


measurements”, Proc. VLSI Test Symposium, 1998, pp


132-137


[2] Ardext Technologies Inc., FASTest,


http://www.ardext.com/


[3] Teradyne IG-XL software, http://www.teradyne.com/


[4] Advantest Siteseer, http://www.advantest.de/


[5] The ITRS 2003: pp 27,


http://public.itrs.net/Files/2003ITRS/Test2003.pdf


[6] Measurements Systems Analysis, 3rd edition, AIAG


[7] Juan F. Ramil, Meir M. Lehman. "Defining and Applying  Metrics in the Context of Continuing Software Evolution," metrics, p. 199,  Seventh International Software Metrics


Symposium (METRICS'01),  2001


[8] GNU Coding Standards


http://www.gnu.org/prep/standards/


[9] Bugzilla, http://www.bugzilla.org/


[10] Eclipse, http://www.eclipse.org


[11] Subversion, http://subversion.tigris.org/


[12] The GNU Project Debugger


http://www.gnu.org/software/gdb


[13] CppDoc,  http://www.cppdoc.org/


[14] CUT:C Unit Test http://sourceforge.net/projects/cut/


IC / test  program


Lines of  code (LoC)


Number  of tests


LoC per


test


LoC of shared


code in


libraries


LoC per  test incl. shared  code


Man effort invested to


achieve complete  characterisation ready  test program


Power Audio


(F)


12,154


323


37.6


100 %


(G)


13,482


728


18.5


61.6 %


(H)


17,013


780


22.4


21,470


35.4


56.1 %


ICs are power management type


Table 2: Effort spent in pilot project and test program sizes  in relation to tests conducted


Conductive Atomic Force Microscopy Application for Semiconductor Failure  Analysis in Advanced Nanometer Process


Kun Lin, Hang Zhang


United Microelectronics Corporation, Hsinchu, Taiwan, R.O.C.


Shey-shi Lu


Graduate Institute of Electrical Engineering, National Taiwan University, Taipei, Taiwan, R.O.C


Conductive Atomic Force Microscopy (C-AFM) is a useful  tool for both electrical failure analysis (EFA) and physical  failure analysis (PFA). In this paper, the root cause of a  physical failure in an analysis image was verified from the  evidence of two-dimensional AFM profile depth  measurement. The other analysis technique, which is electrical  parameter extraction by contacting I-V spectroscopy  measurement, was also utilized to locate the possible defects. As a result, the failure mechanism was illustrated with an  AFM topography image, which showed the silicon surface  profile after removal of cobalt salicide (self-alignment  silicide) by dilute HF. The vertical junction leakage path was  identified with a C-AFM image.


Scaling of semiconductor technology is more complicated at  nanometer dimensions. This impacts conventional failure  analysis technology. SEM/FIB passive voltage contrast (PVC) is commonly used for detecting different potentials for failure  mode analysis, e.g.: opens, shorts, and leakage. However, as  the process progresses into the nano scale, manufacturing  parameters are trending toward extreme values. As the  transistor is fabricated with extra-shallow junctions and poly  gate oxide thickness of less than twenty angstroms, the  extremely small size of the contact circumference is  insufficiently charged by electrons or ions, so that PVC is less  sensitive to some of the failure modes, such as leakage, or  higher resistance.


Conductive Atomic Force Microscopy (C-AFM), which is  more accurate and sensitive than PVC, provides a large  dynamic current detecting range from 1pA to 10mA for widescale semiconductor failure analysis. The current mapping  image combines topography with electrical parameter  characterization, which makes it easier to compare between  good and bad contrast, as in PVC methodology. In this article, another analysis technique, electrical parameter extraction by  contacting I-V spectroscopy measurement, is also utilized to  verify the possible defects.


Experiment:


Electrical failure analysis (EFA) was performed using several  precision analytical techniques for defect localization, e.g. MCT (Mercury Cadmium Tellurium) detector, IR-OBIRCH (Infra-Red Optical Beam Induced Resistance Change) and  PEM (Photo Emission Microscopy). Physical failure analysis (PFA) was performed for failure mechanism discussion, using tools and techniques such as FIB (Focused Ion Beam), PVC (Passive Voltage Contrast), TEM (Transmission  Electron Microscopy), and C-AFM (Conductive Atomic  Force Microscopy).


Case Study: Nano-scale extra-shallow junctions affected  with silicide-roughness-induced leakage issue


Failure Analysis Procedure:


In this case study, a leakage current of 77uA at 0V was  measured on the failing sample. This leakage current was  compared with that of a good sample, which has leakage  current  lower than 6.8uA (Fig. 1.). Both the low-static state (0V) and the I-V characteristic curves of the failing  pin were  different from those measured from the reference sample.


Figure 1.a: The (good) reference sample I/V curve showed the


6.8uA current at “Low state (0V)”.


Figure 1.b: The I-V curve also show  early turn “ON state”, and “Low state leakage of 77uA@0V”.


A backside MCT photoemission detector technique was  performed, which attempted to localize the defect precisely. After zooming in to 1000x, a strong and solid MCT signal  spot was found at an electrostatic discharge (ESD) device, as  shown in Fig. 2.


## Conductive Atomic Force Microscopy Application for Semiconductor Failure Analysis in Advanced Nanometer Process


178


Figure 2: 1000x Zoom, a precise Backside MCT spot was  detected at the ESD protection device.


Passive voltage contrast (PVC) technique is used for detecting  different potentials. However, in this advanced nanometer  process sample, the extremely small contact size is  insufficiently charged, so that PVC is ineffective because of  its low sensitivity, as shown in Fig. 3.


Figure 3: Both n+ diffusion contacts of odd rows (indicated by  blue arrows) and p+ contacts of even rows (indicated by red  arrows) could not be distinguished by contrast difference  using FIB PVC.


C-AFM, which application is extended in the nanometer-scale  failure analysis, is introduced in this paper. C-AFM acquires  both topographical and electrical information by a contacting  signal feedback between an AFM probe tip and the sample  surface (Fig. 4).


Figure 4: C-AFM operation illustration.


The suspected MCT spot was widely scanned for more  accurate defect localization using C-AFM. There are three  images generated simultaneously while scanning the sample  surface using the C-AFM (Fig.4) . The top-left image is the  AFM topography. The bottom-left image is the current  mapping information and the bottom right image is the I/V  spectroscopic curve taken at a point on the sample. On Fig. 5, a green cross in a blue circle indicates where the I-V  spectroscopic measurement was performed on the sample, It  shows the normal n+ diffusion junction as a bright whiteyellow colored contact (Fig. 5). Based on the abnormal dark  black contact, a leakage issue was detected and was  confirmed by I-V curve spectroscopy (Fig. 6). The curve is  like that of a junction leakage issue, as shown in Fig. 6.


Figure 5: A good I-V spectroscopy measurement measured  from a  normal n+ diffusion junction shown  as bright white  on the C_AFM current map..


Figure 6: Three abnormal dark black contact rows were  detected as leakage sites, which was confirmed by I-V curve  spectroscopic  measurement.


Physical Failure Analysis Procedure:


Based on the C-AFM current map information,  a step-by-step  X-SEM FIB technique is used to search for the suspected n+ diffusion contact rows. An obviously abnormal deeper silicide  spike was found (Fig. 7) on the failing area. For advanced  inspection, TEM was performed and the silicide spike depth  of 65.4nm (Fig. 8) was measured, which is twice as deep as  average silcide roughness.


Figure 7: A silicide spiking at the suspected n+ diffusion  contact row was located by step-by-step FIB x-sectioning..


Figure 8: The abnormal silicide spike was measured as


65.4nm.


On the failing sample, after  removing the cobalt salicide using  dilute HF, the surface roughness distribution and geometry  were measured using AFM. It was determined that the surfaces  of the p+ diffusion rows were smoother than the n+ diffusion  rows and that they had fewer dark black cavities. The p+ vertical profile measurement was about 1.5nm,  and the n+ diffusion vertical measurement was about 40nm, as shown in  Fig. 9.


Figure 9: AFM Topographical Images: the left shows the p+ diffusion surface afm image with vertical profile measurement  of  1.494nm and the right afm image shows the dark black  surface cavities of the failing n+ diffusion. This had a  vertical  path of  39.686nm


Result and discussion:


Fig. 9 shows the AFM topographical image of the failing n+ diffusion with several deep surface cavities. After the silicide  process, the cavities were formed like a leakage valley. There  is a high-risk leakage source for an extra-shallow junction  transistor. As the process progresses into the nano scale, the  material selectivity for extra shallow junctions needs to be  tightly controlled.


Our research provides significant evidence that C-AFM  inspection is highly suitable for both electrical failure  analysis and physical failure analysis. In the case study, the  root cause of a electrical (leakage) failure was verified using  the two-dimensional AFM depth profile measurement. The  failure mechanism was then illustrated with an AFM  topography image. Based on the C-AFM results, the extrashallow junction leakage issue has been identified and  resolved. As a result, we have been able to subsequently  improve yields of these processes.


The authors would like to thank Dr. W. T. Chang for kind  advice and support.


[1] Tom. X. Tong, and A. N. Erickson. “Current Image  Atomic Force Microscopy (CI-AFM) Combined with  Atomic Force Probing (AFP) for Location and  Characterization of Advanced Technology Node,” 30th ISTFA, pp.42-45 (2004)


[2] C. P. Lin, C. H. W, and C. C. Ting “A Novel Electrical  Test by C-AFM to differentiate Gate to S/D Gate Oxide  Short from non-Gate Oxide Short Defect in Real  Product”, 30th ISTFA, pp.491-497 (2004)


[3] Z. H. LEE, C. J. Lin, S. W. Lai, and J. H. Chou “Gate  Oxide Defect Localization and Analysis by Using  Conductive Atomic Force Microscopy“ 31st ISTFA  pp.235-238 (2005)


[4] Kartik Ramanujachar “Case studies of the use of Image  Processing in Metrology and Failure Analysis” 31st ISTFA pp.178-182 (2005)


Laser Based Analysis on Analog Circuits with Feedback Loops and a Case Study


Fubin Zhang, David Maxwell


Texas Instruments Inc. DDAO, Dallas, TX fzhang@ti.com, dmaxwell@ti.com


Based on the understanding of laser based techniques’ physics theory and the topology/structure of analog circuit systems with feedback loops, the propagation of laser induced  voltage/current alteration inside the analog IC is evaluated. A  setup connection scheme is proposed to monitor this  voltage/current alteration to achieve a better success rate in  finding the fail site or defect. Finally, a case of successful  isolation of a high resistance via on an analog device is  presented.


Laser based techniques including OBIRCH [1], TIVA [2], and  LIVA [3] are some of the most effective for global fault  localization and have become widely used for integrated  circuit fault isolation. These techniques have been extensively  explored for years in integrated circuit global fault isolation. Analog circuits have been an essential building block since the  beginning of the IC era, and very often feedback loops exist in  these systems to enhance the device performance in all aspects. However, the analog IC devices with feedback loops have  been a challenge for failure analysis. In this paper, the  interaction between laser stimulation and the analog circuit  response is discussed. A method is presented to systematically  analyze analog circuits with feedback loops. Finally a failure  analysis case is used to demonstrate how this method was


applied in a real world analysis.


Laser Based Techniques


All the laser based techniques (TIVA, LIVA, OBIRCH and so  on) were developed based on the laser induced voltage/current  alteration on IC devices. A thermal laser beam (1340nm) is  used most commonly for detecting metal interconnection  defects such as resistive vias and metal bridging by altering the  resistance and in turn the current or voltage. A short  wavelength laser beam (1064nm) is used for analyzing active  region defects, since the short wavelength laser is able to  create electron and hole pairs in the active region and affect  the circuit behavior. All the laser based equipment have at  least one monitoring module, usually either a current or  voltage amplifier and/or a digital input to detect  voltage/current responses from the device under test (Figure  1). This monitor module is also synchronized with the laser  scanner to locate the laser sensitive sites on the DUT (Device  Under Test).


Analog Circuits with Feedback Loops


Feedback loops are used in most analog circuit systems to  improve stability and linearity. However, the feedback loop  introduces a major challenge for failure analysis. The feedback  system usually functions differently when the loop is  disconnected; the open loop response will behave significantly  different. This loop feature can cause the electrical analysis to  run in endless circles. Circuit systems with feed back networks  can be divided into three separate blocks (Figure 2), including  biasing, main signal path and feedback path. The biasing block


provides the power supply and voltage/current reference for


Laser Scanning Module


Monitoring


Module


(Analog/Digital)


Overlay Images


Figure 1: Simplified laser based system block diagram


## Laser Based Analysis on Analog Circuits with Feedback Loops and a Case Study


182


the whole circuit system, sometime even including an on-chip  regulator. The reference, a band gap voltage for instance, is  designed to be temperature, supply, and process independent. The main signal path in general consists of multi-stage  amplifiers. The feedback path could be a network of  resistors/capacitors, level shifters, or even more complicated  active components.


There are cases in which the circuit system cannot be simply  divided into these above-mentioned blocks; for instance, a  local feedback may be just a capacitor between the collector  and base of a BJT or the drain and gate of a MOSFET.


Figure 2: Block diagram of an analog circuit system; most  analog circuits with feedback loops can be divided into these  three blocks shown.


Feedback Circuit System Response to Laser Stimulus


A laser can cause thermal effects and/or electron hole pairs in  the circuit system, depending on the laser wavelength. This  thermal effect or electron hole pairs will change the electrical  characteristics of the local area; for instance, resistivity or  recombination current will change. This change can also be  reflected in the node voltages or through current alteration. During laser based analysis, the laser is scanned over the DUT  from either the front side or the backside. When this laser  beam passes the fail site, it stimulates a voltage/current  alteration. This alteration can be treated as a voltage or current  pulse signal. The shape and size of this pulse could vary and is  determined by the laser scanning speed, physical mechanism, local circuit structure and more. It can be simplified to a bellshape pulse signal which will propagate through the circuit  system. When we look at the three blocks in Figure 2, the laser  stimulated pulse signal will propagate differently. The detail of  the pulse signal propagation in the circuit system can be  analyzed using SPICE simulation to compute the pulse  response numerically or by calculating the transfer function  analytically. But in general, the propagation can be  summarized as follows:


(1) Biasing Block:


In the biasing block, this pulse signal has a much higher  chance to propagate to power supply connections than to the  main signal path. For instance, in a typical differential  amplifier, the CMRR (Common Mode Rejection Ratio) is


designed to be as high as possible to prevent the coupling from  biasing noise to the main signal path.


(2) Main signal path:


The inputs control the outputs through the main signal path. If  the laser induced pulse signal falls into the main signal path, it  will follow the direction from the input to the output.


(3) Feedback network:


This part is more complicated. The pulse signal will propagate  both directions. However, when the response reaches the  inputs, it will be transferred to the outputs. So, you will see a  combination of two responses at the outputs from two different  paths.


When using laser based techniques to perform global fault  isolation, all these factors should be considered while  monitoring the response to maximize the chance of identifying  a fail site.


Case Study


The device analyzed is a preamp unit used to amplify a small  analog input signal (Figure 3). The biasing block is not drawn  in the schematic. The main signal path for the overall system is comprised of Amp1, Amp2 and Amp3. The Amp0, Q1, D1, D2, R1, R2, and R3 form a feedback control loop to set the  input terminal biases. The failure mode was confirmed on ATE  to be input biasing out of specification. The input terminals  were therefore chosen for monitoring during the TIVA  analysis.


Figure 3: Simplified schematic of the preamp device analyzed  with a laser based technique.


The TIVA images showed an anomalous alteration spot at a  metal1 to metal2 via (Figures 4 and 5). Experimental TIVA analysis was also performed by monitoring first the power  supply and then the outputs. However, no abnormal response  was detected using these approaches. Electrical probing  confirmed the failing high resistance via. This via is located  between D1 and R2. The pulse response should have  propagated through R2, Amp0 and Q1, and then reached the  input terminal. TEM imaging of a cross section through the via  showed a layer of highly resistive (~180 ohms) material with a  high percentage of oxygen and fluorine at the bottom of the via (Figure 6).


Main Signal Path


(Gain stage)


Feedback network


Inputs


Outputs


Bias block


(Power Supply and Reference)


This real case demonstrated how to understand the propagation  of the laser induced pulse response in the feedback loop to  achieve a higher success rate with laser based analysis.


Figure 4: TIVA analysis image showed an alteration site at  the failing via (red arrow). Other alteration sites were in the  Amp0 block, the same as those on a known good unit.


Figure 5: High magnification TIVA image at the fail site of the  failing via. The red and blue spots mean the monitor module  received a signal when the laser was shined on that location.


Figure 6: TEM image of the failing via cross section. A high  resistance film was observed at the bottom of the via. EDX  showed a high percentage of oxygen and fluorine.


Conclusions and Acknowledgments


It is crucial to understand the propagation of laser induced  voltage/current pulses in a feedback circuit system in order to maximize the laser based analysis success rate. When the  failing block is known, a better setup connection to monitor  the most significant pins to the laser response has been proposed. As demonstrated in the case study, this setup  scheme showed positive results.


The authors would like to thank Dan Callahan, Ken Brawley, and Shelley Shafer for their support of the work in this paper.


[1] Nihawa K, Inoue S, “Various Contrasts Identifiable From the Backside of a Chip by 1.3 um Laser Beam Scanning and Current Changing Imaging” ISTFA (1996) pp.387


[2] Cole EI, Tangyunyong P, Barton DL, “Backside  localization of open and shorted IC interconnections”IRPS(1998) pp.129


[3] Cole EI, Soden JM, Rife JL, Barton DL, “Novel failure  analysis techniques using photon probing with a scanning  optical microscope”,  IRPS(1994) pp.388


A Novel Method to Inspect Deep Trench Capacitor Planar Profiles in DRAM


J. L. Lue, A. Huang, and T. Wang


ProMOS Technologies Inc.,Hsinchu Taiwan, R. O. C. Jen-lang_lue@promos.com.tw


This paper presents a novel method to inspect deep trench (DT) planar profiles at any particular depths using the  mechanical polishing method instead of the Focused Ion  Beam (FIB) milling method.  The sample is polished at a  small beveled angle and then inspected in the Scanning  Electron Microscope (SEM).  This method creates a large area  for the inspection of DT profiles. It is accurate and fast in  providing the result on process evaluation and failure analysis.  Since the FIB is not needed, it is also simple and cost  effective.


The inspection of plane-view deep trench (DT) capacitor  profiles in DRAM is very important for process monitoring, development, and failure analysis [1-3].  DT capacitors are  formed in the substrate Si after etching deep holes, about 7-8 µm, into the wafers.  The FIB is presently used to prepare the  sample for a plane-view DT profile inspection in the SEM  because it is able to mill the DT to a particular depth.  Fig. 1  shows the typical SEM images of DTs prepared by the FIB  milling method.  Nevertheless, the main drawbacks of using  FIB milling are that it is time-consuming, only a small area is  inspected and it is expensive.


To inspect the planar profiles of DTs at the depths of 1 µm, 2 µm, 3 µm, 4 µm, 5 µm and 6 µm in an area of 16 µm2  generally takes 4 hours to complete the results for one sample.  For process evaluation, collecting five samples per wafer used  to take several hours to obtain results.  With the shallow  angled FIB milling method, more information can be provided  in a slanted cut, but the process requires several cuts to inspect  the profiles for the overall depths of DTs [2].  Those results  are always limited by the drawbacks of using FIB.  Basically, the different depths have to be made step by step in FIB.  Therefore, the more depths that are required, the more time it  takes.


In order to provide fast results for the inspection of planar DT  profiles at any depths, a novel approach has been developed in  our laboratory using mechanical polishing instead of the FIB  milling method.  The sample is polished at a small beveled  angle and then is inspected in the SEM.  This method not only  provides the variation of the overall DT profiles in detail in a  quick way, but also inspects the DTs in a much larger area


than has ever been seen before.  In addition, this technique is  cost effective because the FIB is not needed. In this paper, the  methodology of this novel approach will be described and the  applications for the inspection of DTs will also be discussed.


Figure 1 Typical SEM images showing (a) the DT planar  profile at a particular depth, t, prepared by FIB milling from


(b) the cross section; the particular depth, t, of DTs can be  measured from the surface of Si substrate as an indicated line  before FIB milling.


The bevel polish has been used for years for the sample  preparation of Spreading Resistance Profiling (SRP) to  determine the carrier concentration and junction depth in a  SSM SRP system [4].   In this new approach, we apply the  bevel polish for the sample preparation of SEM to determine  the planar profiles of DTs.  The backside of the DT capacitor  DRAM chip is mounted onto a bevel sample mount at a small  beveled angle of 2˚52’.  The bevel sample mount is then  attached to a polishing holder for further mechanical grinding  and polishing using a slurry of 0.05 µm diamond abrasive on a


## A Novel Method to Inspect Deep Trench Capacitor Planar Profiles in DRAM


185


glass plate.  This polishing is accomplished within 10 minutes.  Then the DT planar profiles at any depths on the beveled  surface can be inspected in the SEM.  Figure 2 shows the  schematic diagram of a typical sample being polished.  The  DT Depth ( Δ Z) can be calculated from the distance of the  bevel edge to the particular DT (Δ X) on the beveled surface  via the equation:


Δ Z =Δ X sin α , where the bevel angleα =2˚52’


Δ Z =Δ X sin 2˚52’ = Δ X (0.05)


Once the bevel edge of the sample is found in the SEM, the


Δ X can then be measured.  Hence, the planar profile at a  particular depth of DT can be inspected accordingly.


Figure 2: A schematic diagram showing the sample mounted  on the bevel sample mount being polished.


In general, the whole process takes less than one hour to be  completed.  Moreover, the entire polished area is about 9  mm2, which is approximately 500K times of 16 µm2.  In the  FIB milling process, it is impossible to create a surface of 9  mm2 at one cut for inspection purposes.  As mentioned earlier, it takes few hours to produce an area of 16 µm2 for particular  depths using the FIB milling method.   This method actually  provides a much larger area for the inspection of DTs at any  depths than that used by the FIB milling method. The area  created by the new process is able to provide much more  information for monitoring and analysis


Figure 3 shows the typical SEM results of the DT planar  profiles at different depths for process evaluation.  The  distances measured ( Δ X), 40µm, 50µm, 60µm, and 100µm  from the bevel edge correspond respectively to the depths ( Δ


Z) of the DTs at 2 µm, 2.5 µm, 3 µm and 5 µm.  The  geometries of DTs can be examined and the critical  dimensions of DTs can be measured.  These results are very  important for process/integration engineers to justify the DT  etching process.


Figure 4 shows the SEM results of the abnormalities in the  structure of DTs, called a “DT-DT short”.  These  abnormalities, that will cause functional failures in the  electrical test, were found at the distance of 90 µm ( Δ X) from  the bevel edge, which refers to the depth ( Δ Z) of the DT at


4.5 µm.  These results that indicate the profile and position of  failure DTs will help engineers tune the etching process to  correct this problem.


Figure 3:  The SEM results showing the DT planar profiles  examined at different distances from the bevel edge, referring  to the depths of DT at 2 µm, 2.5 µm, 3 µm and 5 µm.


Figure 4:  The SEM results showing the “DT-DT short” at the  distance of 90 µm from the bevel edge, which refers to the  depth of DT at 4.5 µm


A novel approach has been developed to inspect DT planar  profiles using mechanical polishing instead of the FIB milling  method.  A large area can be created within 10 minutes for the  inspection of DT planar profiles in the SEM.  The variation of  overall DT planar profiles and the abnormalities on the  structures of DTs can be examined at the polished surface.  In  addition, this new technique is cost effective because the FIB  is not needed.


In summary, this new method provides a more efficient way to  inspect the variation of the overall DT profiles in detail for  process monitoring, development, and failure analysis.


The authors would like to present our thanks to the colleagues  at Department of Physical Failure Analysis in ProMOS for  their insightful discussion and support.


[1] J. L. Lue, J. Lee, E. Chen and J. S. Luo, “A Review of  TEM Observations of Failures of the Memory Cell in a  Deep Trench Capacitor DRAM”, Proc. 29th ISTFA (2003) p144.


[2] J. D. Russell and J-W Tseng, “A Method for Exact  Determination of DRAM Deep Trench Surface Area”, Proc. 30th ISTFA (2004) p140


[3] H. W Liu, E. Cheng, Y. M. Lin, S. Fan, K. Pan and J. L. Lue*, “A Novel Approach to Inspect Abnormalities on  the Deep Trench Capacitors in DRAM”, Proc. ICCM  2005 p594


[4] SSM Seminar: Standard and Advanced Spreading  Resistance Measurements, Solid State Measurements Inc:,


Surface Defect Analysis by Using a Novel Backside XTEM Sample Preparation  Method


Jian-Shing Luo, Lang-Yu Huang, Wen-Lon Gu and Jeremy D. Russell


Physical Failure Analysis Department, Inotera Memories, Inc. Taoyuan Taiwan, Republic of China


Typical gate characterization includes metallic contamination  and the F, B, P and N elements distributions in a gate stack (Nitride/WSix/doped poly-Si/SiO2/Si substrate) analysis, especially B and F. The F segregation and B penetration  influences the intrinsic reliability of thin gate oxides and Vt in poly-Si/SiO2/Si structures [15-16]. Therefore, F and B  controlling is very important to device performance. However, there is no concern of penetration into the Si substrate for N+poly silicon gates [17]. Fig. 9 shows the difference between  two poly-Si gate stacks SIMS depth profile results of  oxide/WSix/P implanted poly-Si/SiO2/Si structures. Fig. 9(a) clearly shows F contamination on the poly-Si layer surface. It  is believed that the contamination source of F came from the  NF3, which is the plasma cleaning gas of the poly-Si  deposition chamber cleaning process. After using SiH4 gas to  purge the chamber for a few hundred of seconds, no more F  contamination was found in the poly-Si layer of the gate stack, as shown in Fig 9 (b).


Depth


Figure 9: SIMS depth profiles showing the F, P, O and Si  distributions in a  poly-Si gate multilayer (a) before chamber  cleaning (b) after chamber cleaning.


As discussed above, the Vt of MOSFETs decreases as the  channel length is shortened and also as the drain bias is  increased [4]. For trench DRAM, the As dosage and depth  profile in the poly-Si electrode layer beside AA might  influence the device characteristics, especially on reliability  and Vt. A three-step process was adapted to form poly-Si  beside AA. The final structure is AA/un-doped poly-Si (UP2)/As doped poly-Si/un-doped poly-Si (UP1), as shown in  Fig. 1. The As dose and thickness of UP2 layer are critical for  Vt and device characteristics. Higher As dosage and thinner  poly-Si layer easily result in lower Rs and shorter channel  length due to higher As concentration around the source/drain  regions. One example is shown below. From electronic data, the Vt of product one is lower than that of product two. In  addition, the Rs of the UP2/dosed poly-Si/UP1 multi-layer of  product one is lower than that of product two. It is indicated  As concentration in UP2/dosed poly-Si/UP1 multi-layer was  higher for product one. From SIMS analysis, the dosage and  UP2 thickness are higher and thinner, the distance of As peak  and un-doped poly-Si layer surface, for product 1, as shown in  Fig. 10. It reveals that As dosage and UP2 thickness might be  the main root cause to explain why Vt was lower. In addition, it is very interesting that total As dosage of the wafer is higher  at the furnace top location, from further analysis. This could  be explained by the AsH3 and SiH4 gases being injected from  the furnace top to bottom during the process.


Figure 10: SIMS depth profiles showing As peak (right) of  product one is closer to the surface of UP2 than that of  product 2.


TEM and SIMS have been used extensively to support  technology development, failure analysis and manufacturing  of advanced DRAM. Several cases were demonstrated to show  the applications of TEM and SIMS on crystal defect and  microstructural characterisation of advanced 512 Mb DRAM.


The authors would like to thank all our colleagues in Inotera  Memories Inc. for their help in this work, particularly the  electrical failure analysis characterisation and failure analysis II sections.


[1] B Keeth, R. J. Baker, DRAM Circuit Design, the Institute


of Electrical and Electronics Engineers, Inc., New York,


2001.


[2] F. Siegelin and A. Stuffer, “Dislocation related Leakeage


in Advanced CMOS device,” Proceedings of the 31st


International Symposium for Testing and Failure Analysis


November 6-10, 2005, pp. 59-63.


[3] X.Z. Bo, N. Yao, S.R. Shieh, T.S. Duffy, and J.C. Sturm,


“Large-grain polycrystalline silicon films with low


intragranular defect density by low-temperature


solid-phase crystallization without underlying oxide,”


Journal of Applied Physics, vol. 91, 2002, pp. 2910-2915.


[4] C.Y. Chang, and S.M. Sze, ULSI Devices, Chapter 3


MOSFET Fundamentals, Wiley-Interscience, New York,


2000, pp. 88-89.


[5] J. Dubois, J. Knol, M. Bolt, H. Tuinhout, J. Schmitz, P.


Stock, “Impact of Source/drain Implants on Threshold


Voltage Matching in Deep Sub-micron CMOS


Technologies,” 32th European Solid-State Device


Research Conference, 2002, pp. 115-118.


[6]  J.A. Croon, E. Augendre, S. Decoutere, W. Sansen, H.E.


Maes, “Influence of Doping Profile and Halo Implantation


on the Threshold Voltage Mismatch of a 0.13um CMOS


Technology,” 32th European Solid-State Device Research


Conference, 2002, pp. 579-582.


[7] B.Y. Choi, I.H. Nam, J.D. Lee and B.G. Park,


“Sub-0.1-um NMOSFET with 12-nm n+-p Junction Using


5-keV As2+ Ion Implantation," Journal of the Korean


Physical Society, Vol. 39, No 1, July 2001, pp. 72-75.


[8] A. Budrevich and J. Hunter, “Characterization and


Metrology for ULSI Technology 1998 International


Conference”, 1999, pp. 169-181.


[9]  J. Amon, A. Kieslich, L. Heineck, T. Schuster J. Faul, J


Luetzen, C. Fan, C.C. Huang, B. Fischer, G. Enders, S.


Kudelka, U. Schroeder, K.H. Kuesters, G. Lange, J.


Alsmerier, “A highly manufacturable deep trench based


DRAM cell layout with a planar array device in a 70 m


technology,” Electron Devices Meeting, 2004. IEDM


Technical Digest. IEEE International. 13-15 Dec, 2004, pp.


73-76.


[10] A. John Mardinly, “Electron Tomography and  Three-Dimensional Aspects of Transmission Electron  Microscopy,” Electronic Device Failure Analysis, vol. 7, No.3, 2005, pp. 6-12.


[11] C. Kübel, S. Kujawa, J.S. Luo, H.M. Lo, J.D. Russell, ”Application of Electron Tomography for  Semiconductor Device Analysis,” in '8th International  Workshop of Stress-Induced Phenomena in Metallization', edited by E. Zschech, K. Maex, P.S. Ho, H. Kawasaki, T. Nakamura, AIP Conference Proceedings 817, 2006, pp. 223-228, American Institute of Physics, Melville, New  York.


[12] W.T. Stacy, E.K. Broadbent, and M.H. Norcott, “Interfacial Structure of Tungsten Layers Formed by  Selective Low Pressure Chemical Vapor Deposition,” J. Eelectrochem. Soc. 132, 1985, pp. 444-448.


[13] M.J. Wang, R.L. Jiang, J.W. Hsia, C.H. Wang, J.E. Chen, “Guardband Determination for the Detection of off-State  and Junction Leakages in DRAM Testing,” Test  Symposium, 2001. Proceedings, 10th Asian, 19-21 Nov. 2001, pp. 151-156.


[14] K. Ryoo, R. Drosd, and W. Wood, “Location effects of  extended defects on electrical properties of P+ -n  junction,” J. Electronchem. Soc., vol. 136, no. 3, 1989, pp. 768-771.


[15] D. Krüger, J. Dabrowski, P. Gaworzewski, and R. Kurps,K. Pomplun, “Fluorine incorporation into gate stacks of  advanced silicon memory technologies: Simulation, depth  distribution, and reliability,” Journal of Applied Physics, vol. 90, Issue 7, 2001, pp. 3578-3584.


[16] J. R. Pfiester, Frank K. Baker, Thomas C. Mele, Hsing-Huang  Tseng, Philip J. Tobin, James D. Hayden, James W. Miller, Craig, D. Gunderson, Louis C. Parrillo, “The effects of boron penetration on p+ polysilicon gated  PMOS devices,” IEEE Tran. Electron Devices, ED-37, vol. 37, 1990, pp. 1842- 1851.


[17] H.S. Momose, S. Nakamura, T. Ohguro, T. Yoshitomi, E. Morifuji, T. Nforimoto, Y. Katsumata,  H. Iwai, “Uniformity And Reliability Of 1.5 nm Direct Tunneling


Gate Oxide MOSFETs”,  VLSI Technology, 1997. Digest of Technical Papers, 1997 Symposium on June  10-12, 1997, pp. 15-16.


Advanced Manual Package Pulling System for Removing PCB Components in  preparation for Crack Area Measurement and Disbond Type Mapping.


Todd R.McDonald, Intel Corporation, Hillsboro, Oregon, USA


Existing tools widely used by industry to manually remove PCB components for disbond type mapping or crack area measurement, present significant ergonomic and process  quality concerns.


These manual removal tool designs typically employ some kind of fulcrum device and or additional fixturing with bolts attached to pry the component from the board.


The most common designs are flat head screw drivers modified with a bent shaft, but some elaborate lobe lever arm designs have emerged in recent years (Figure 1).  These designs often cause damage to some of the solder joints on components during pull, and frequently operators using these designs report safety concerns and ergonomic discomfort.


This paper evaluates these concerns and proposes a design solution that eliminates them.


Figure. Cam lever removal tool


Figure 2. Bolts bent by cam lever tool.


This uneven distribution of force across the solder joints could compromise data. Additionally the strong downward force applied to the lever arm of pry and cam-style removal tools presents safety and ergonomic risk to the operator. From an ergonomic perspective, tool users will inherently have differing physical strength abilities.  For many individuals, the force required to operate a cam lever removal tool design is too excessive. Furthermore, safety is an issue as the  component often releases from the PCB while hands are  applying intense downward pressure sending the hands and knuckles  at high force into the board populated with sharp components.  The manual pull tool system introduced here,demonstrates a dramatic reduction of these concerns (figures 3, & 4). With this tool there is no prying, lever or angular force applied to remove the component. The T-handle pull tool rotates using vertical threads to apply vertical removal force.


figure 3.  Board, component, pull box, and T-handle pull tool


## Advanced Manual Package Pulling System for Removing PCB Components in preparation for Crack Area Measurement and Disbond Type Mapping.


202


Components are prepared for pulling by attaching a ¼-20 bolt encapsulated ½ inch or higher up from the bolt base, using either Faststeel epoxy compound or Loctite E-120 HP epoxy.


When epoxy has cured, a box fixture closely fitting the dimensions of the component to be pulled is slipped over the top of the bolt and component. Large universal style box fixtures are often too wide and cannot be positioned flush against the PCB surface due to interfering peripheral obstructions. Additionally, fixtures that allow too much room between the fixture wall and the component allow the PCB to  flex too much increasing disbond irregularities in the separating joints. The system presented here uses a small ledge to navigate around peripheral components where the box fixture contacts the board Figures 5 & 6.


Figure 5: small ledge at base of pull box fixture for navigating around peripheral components.


The T-handle tool is positioned over the box fixture and threaded onto the bolt until it comes in contact with the top of the box fixture.  The T-handle tool is then actuated with both hands, one at each end, rotating until the component separates  from the PCB, usually indicated by a snapping sound figure 4.


Method and Analysis


Method


To quantify any reduction in manual force required by the operator to pull a component, a calibrated Chatillion DFIS 200  force meter was positioned and actuated at measured lengths on the handle or lever arms so that force could be normalized to foot pound figures. Six identical socket packages were pulled while manual actuation force was measured. Of these six samples, three were pulled using a current cam tool design and three were pulled using the advanced design being presented here. Force measurements for each group were compared for average required manual removal force.


Figure 4: Rotating the Manual pull tool over the box fixture to remove the component


Figure 6: T-handle & box fixture on densely populated board.


Analysis Results


The T-handle pull tool demonstrated a reduction in manual operator force by an average of 93% compared to the cam lobe  lever design. The presence of bent bolts and angular sample movement are not witnessed with the T-handle design as they are present with separated using cam lob levers. The T-handle tool eliminates the safety issues experienced with cam levers and pry tools of high downward force and impact of hand on sharp board components.


Cam lever removal tool


Advanced removal system


79 lbs force required


2 lbs force required


Ledge and peripheral components


Conclusions & Acknowledgement


This tool and method for manually pulling board components dramatically reduces required operator force while improving ergonomic, safety and function over currently used devices.


Additionally the new design reduces bending of pull bolts and angular pull direction that may interfere with availability and interpretation of subsequent disbond data. The author would like to give special thanks and recognition to Julie Schuchman of Intel for her assistance on this project.


Application of FIB Circuit Edit in Analysis of Memory Failure of SOI Devices


Z. G. Song, S. K Loh, X. H. Zheng, S.P. Neo and C. K. Oh


Failure Analysis Lab, QRA, Chartered Semiconductor Manufacturing Limited, Singapore


Silicon on insulator (SOI) is a semiconductor wafer  technology, which usually produces products with high  quality and reliability for astronautic application. Today it is  also employed to produce consumption devices with higher  speed and lower power than those produced by traditional  bulk silicon technology. This technology has advantages for  portable products, such as laptops, handheld devices and other  applications that depend on battery power. SOI wafer works  by placing a thin, insulating layer, such as silicon dioxide or  glass, between the thin layer of silicon, called T-Si, and the  silicon substrate. However, with the introduction of SOI  technology, failure analysis faces new challenges. For bulk  silicon technology, contact-level Passive Voltage Contrast (PVC) [1] is a powerful technique in analysis of memory  failure. It can easily identify an abnormal contact from the  normal contacts with the fact that the abnormal contact is  charged up to different potential from those potentials that the  normal contacts are charged up to, under lower-energy e-beam  or ion-beam inspection. However, for SOI technology, the  active contacts land on T-Si, which is insulated from silicon  substrate. Whether the active contacts are open or not, they are  at the same potential under e-beam or ion beam inspection  because they are all floating. So, contact-level PVC technique  is not suitable for SOI technology. Recently, a variety of  electrical characterization techniques for individual transistor, commonly called electrical failure analysis (EFA), have  emerged and become popular in failure analysis Lab. These  techniques include nano-probing in SEM or FIB [2], scanning  probe microscope [3] and FIB circuit edit [4]. In this paper, we will present two cases to demonstrate the application of  FIB circuit edit in analysis of memory failure of SOI devices.


Focused Ion Beam (FIB) is an indispensable tool in modern  semiconductor Failure Analysis laboratories. Besides these  applications, such as passive voltage contrast for fault  isolation of open or short failure, precisely cross-section for  defect analysis or process characterization and Transmission  Electron Microscope (TEM) sample preparation, recently FIB  is also intensively employed to do circuit edit [4, 5, 6] for  design debug and failure analysis because it possesses the  ability to selectively remove existing materials and deposit  new conductor and insulator layers. For our cases, FIB is  employed to deposit metal lines and micro-pads for accessing


to the related internal nodes of the suspected defective  transistors. Once the micro-pads are deposited, the sample is  ready for micro-probing to characterize the electrical behavior  of the transistors. Analyzing the electrical behavior will lead  to isolation of the defective location, which can be subject to  further physical analysis.


Figure 1 Ion-beam image of 10 pads deposited for accessing  to the 6 transistors of a SRAM cell


BL


BL-bar


Vdd


Vss


PSG1


PSG2


WL


PU1


PU2


PD2


PD1


Figure 2 The typical schematic of a 6-transistors SRAM cell.


First case was single bit failure of SRAM units manufactured  with 90 nm technology in SOI wafer. Conventional top-down  de-processing and SEM inspection for several units always  ended with root cause not found. Thus, one unit was deprocessed to contact level for FIB circuit edit. Figure 1 shows


## Application of FIB Circuit Edit in Analysis of Memory Failure of SOI Devices


204


the ion- beam image of the ten pads deposited for accessing to  the six transistors of the failing SRAM cell. The typical  schematic of a six-transistor SRAM cell is shown in Figure 2. After depositing the microprobe pads, using the FIB, the  electrical behavior of the six transistors was characterized  with micro-probing. The family of curves, Id-Vd curves at  different gate voltages, of the six transistors was measured  using an electrical characterization system with the biasing  condition for the source set at 0 volt, the drain was swept from  0 to 1.0 volt at 0.05 volts increment, and the gate was stepped  at 0.1, 0.325, 0.55, 0.775 and 1.0 volts. The measurements  were repeated with the source drain swapped. The family of  curves are shown on Figs. 3-8. It was found that the family  curves of pass-gate transistor 2 (PSG2), pull-down transistor 2 (PD2) and pull-up transistor 2 (PU2) were abnormal, while  those of pass-gate transistor 1 (PSG1), pull-down transistor 1 (PD1) and pull-up transistor 1 (PU1) were ok.


Figure 3 Family of curves of the PSG 1 (NMOS) – ok


Figure 4 Family of curves of PSG 2 (NMOS) – abnormal


Figure 5 Family of curves of PD 1 (NMOS) – ok


Figure 6 Family of curves of PD 2 (NMOS) – abnormal


Figure 7 Family of curves of PU 1 (PMOS) – ok


Figure 8 Family of curves of PU 2 (PMOS) – abnormal


Since the PSG2, PD2 and PU2 shared the common drain  contact and their drain currents were much less than those of  PSG1, PD1 and PU1. It implied that the common drain  contact of PSG2, PD2 and PU2 was high resistant or open. Thus the common drain contact was further submitted to  XTEM analysis and the XTEM picture as shown in Figure 9  revealed an amorphous layer under the common drain contact, leading to open failure of the common drain contact, which  was responsible for the single bit failure.


Figure 9 XTEM picture showing amorphous layer under the  contact.


Second case was the whole column failure with a single bit  pass for a SRAM unit. For this failure mode, logically the  defect should be the shorting of bit/bit-bar line to the word  line poly. To further identify the shorting location, the unit  was de-processed to contact level for FIB circuit edit. Four  pads were deposited for accessing to the bit/bit-bar line  contacts and word line contacts as shown in Figure 10.


Figure 10: Ion-beam image of 4 pads deposited for accessing  the bit/bit-bar line contacts and word line contacts.


Electrical characterization showed that an ohm shorting of  bit/bit-bar line to word line existed at left side, while it is ok at  right side (see Figure 11). XTEM analysis on the shorting  location showed certain residue at poly spacer sidewall, which  bridged the word line poly to the active of bit/bit-bar line (see  Figure 12). EDX analysis on the residue indicated that the  residue was Co or Co silicide (see Figure 13).


-80-40 0 40 80


-1


-0.5


Voltage (V)


Left Right


Figure 11 I-V curves showing bit/bit-bar line shorting to the  word line at left side.


Right


Figure 12: XTEM picture showing Co residue bridging the          word line poly to the bit/bit-bar active.


Left


P1


Figure 13: EDX analysis on the residue showing Co and Si  peaks.


In conclusion, FIB circuit edit and electrical characterization  is a good methodology for further narrowing down the  defective location of memory failure, especially for SOI  technology, where contact-level PVC is not suitable.


The authors would like to thank the management and  colleagues, especially TEM group of FA Lab, Chartered  Semiconductor Manufacturing Ltd, for their supports and  helps.


[1] Z. G. Song, G. Qian, J. Y. Dai, Z. R. Guo, S. K. Loh, C. S  Teh and S. Redkar, “Application of Contact-level Ionbeam Induced Passive Voltage Contrast in Failure  Analysis of Static Random Access Memory”, IPFA  Proceeding, pp. 103-107 (2001).


[2] C. C. Wu, J. C. Lee, J. H. Chuang, T. T. Li, “Single  Device Characterization by Nano-probing to Identify  Failure Root Cause”, ISTFA Proceedings, pp. 183-185, (2005).


[3] J. C. Lee and J. H. Chuang, “Fault Localization in  Contact Level by Using Conductive Atomic Force  Microscopy”, ISTFA proceedings, pp. 413-418 (2003).


[4] S.B. Herschbein, L. S. Fischer and A. D. Shore, “Basic  Technology and Practical Applications of Focused Ion  Beam for the Laboratory Workplace”, Microelectronic  Failure Analysis, Desk Reference 4th Edition, pp. 517-526.


[5] Randal Mulder, “A Simple FIB Method for Constructing  Electrically Isolated Microprobe Pads for the Electrical  Analysis of Failing 0.12um Technology SRAM Bit  Cells”, ISTFA proceedings, pp.538-545 (2004).


[6] J. Myers, M. Abramo, M. Anderson and M. W. Phaneuf, “A Novel Approach for Enhancing Critical FIB Imaging  for Failure Analysis and Circuit Edit Applications” ISTFA proceedings, pp.151-156, (2004).


A Fast Inspection of Well Implantation by Using Plane-View Stain Method


Jian-Chang Lin, Wen-Sheng Wu, Kuo-Shiung Chen, Jen-Hung Yeh, Ying-Chin Hou


United Microelectronics Corporation, Hsin-Chu, Taiwan, ROC(Jian_chang_lin@umc.com)


In the field of failure analysis, electrical failures caused by improper implantation are often difficult to debug especially for fully processed products. Familiar implantation failure issues include improper implantation concentration,error doping types, incorrect doping ranges, and etc. Although some FA equipments, such as secondary ion mass spectrometry (SIMS), spreading resistance probe (SRP) and scanning capacitance microscope (SCM) [1] [2] [3], can do detail or quantitative analysis for these failure issues, most of these FA jobs are time-consuming and have a detection limitation at the size of failure area. This limitation may restrict the FA applications because the failure area is usually small at the fully processed products after fault isolation. In  this paper, two examples with improper doping type and  concentration will be analyzed by using a newly developed FA method. Instead of using traditional cross-section (X-S) stain method, we utilize a plane-view stain method to compare the doping type and doping concentration between normal and  failed regions. With the aid of the plane-view stain method,we can have a quick check at the suspected failure area with improper front-end implantation before specific SCM analysis.


For front-end implantation failure in full process wafers,SEM X-S stain wet etching is a common and traditional FA  method to clarify the Well profiles. This method is useful for global failure issue but it’s not so useful to do specific site


observation after fault isolation. This is because it’s not easy  to do sample preparation and to well control the etching time. Therefore, back and forth FA jobs are sometimes unavoidable for this check.


Instead of using traditional X-S stain, plane-view stain


method has been tried to improve the above inconveniences.


The principle of plane-view stain is almost the same as X-S  stain. Both of them utilize different etching selectivity for Nand P-doping to clarify the N-doping and P-doping regions.


But by using plane-view stain method, sample preparation and etching time control are easier and with a higher success rate than X-S stain method. What we need to do in plane-view


stain sample preparation is to use hydrofluoric acid (HF) to


remove all layers above diffusion area and then use stain acid to do wet etching at the interest regions.


Below, we’ll introduce two real cases with improper


doping concentration and doping type by using plane-view


stain method to have a quick preview and then use specific


SCM to double confirm this result.


The first example using plane-view stain method:


In the example 1, the low yield wafer is using sub-micron process with 1-poly and 10-metal layers. As CP test data showed in Fig.1, this product suffers serious by-frame power leakage (Bin24) and memory function (Bin30) failures. The core power current is about 50mA@1V (20ohm) at power leakage failure dies (Fig.2). Liquid crystal detection (LCD)and backside (B/S) emission microscope (EMMI) are used to detect the leakage sites in both power leakage dies and function failure dies (Fig. 3 & 4). The LCD and EMMI spots are located at the same sites die-by-die and these sites are suspected to be the real failure sites according to FA  experience. But after FIB X-S and SEM plane-view layer-bylayer check, no obvious abnormality is found.


## A Fast Inspection of Well Implantation by Using Plane-View Stain Method


208


Figure 1: A typical CP map of low yield wafer in example 1.


Figure 2: I-V characteristic curve of power leakage failure dies (Bin24) and memory function failure dies (Bin30). The two-pin probing power current is about 50mA@1V at Bin24 dies.


Figure 3:LCD hot spot locations (the same as B/S EMMI spot sites)


Figure 4: B/S EMMI spot locations (the same as LCD hot spots site). A line shape is found for these  suspected emission spots.


Before specific SCM analysis, a quick check at N- and  P-diffusion areas by plane-view stain is executed for both power leakage and good dies. This stain solution is a mixed acid solution which consists of nitric acid (HNO3), acetic acid(CH3COOH) and hydrofluoric acid (HF). The etching selectivity is higher for N-doping than P-doping. This means the wet etching rate is higher at N-Well region than P-Well region. As Fig. 5 showed, the plane-view stain result reveals that the N-Well etching rate at hot spot sites is lower than normal sites. The remained pattern width of N-Well region at  hot spot site is obvious wider than normal site. This implies the N-doping concentration is lighter at hot spot site than normal site and results in relative lower etching rate. Similar etching rate difference can be observed at nearby P-Well region (the P-Well region is nearby failed N-Well region) but the etching rate there is higher than normal P-Well region.


This result also gives us a suggestion that higher P-doping concentration or improper extra N-doping at this abnormal PWell region. Besides, the location relations between B/S EMMI spots sites and the abnormal plane-view stain sites are pointed out in Fig. 6.


(d)


Figure 5:


(a) SEM plane-view pictures before and after plane-view stain wet etching. As SEM picture shows the etching rate is higher at N-Well region than P-Well region.


(b) At hot spot site, the etching rate at failed N-Well region(hot spot site) is lower than normal N-Well region.


The etching rate at nearby P-Well region is faster than normal P-Well region.


(c) The relation between failure sites and N-Well and P-Well regions are shown.


(d) The abnormal diffusion pattern widths at N-Well and PWell regions are pointed out due to higher and lower etching rates, respectively.


Figure 6: The location relations between B/S EMMI spots sites and the abnormal plane-view stain sites are pointed out.


In the sub-micron process, 20 to 30 sec’s plane-view stain time is long enough to distinguish obviously improper doping type or concentration in this example. According to the above results, extra N-doping in P-Well region or lighter Ndoping in N-Well region is suspected. Specific SCM is done to  clarify the exact failure mechanism and the result gives us a  strong evidence of improper implantation. Fig. 7 clearly indicates an extra N-doping signal within P-Well region at hot spot site and it’s the root cause of higher etching rate at failed P-Well regions. The same technique is applied at memory function failure dies and the result is similar to power leakage dies as shown in Fig. 8, but with smaller wet etching rate difference (smaller remained pattern width difference)between normal and failed sites.


Transmission electron microscopy (TEM) is more and more  important for the structural analysis and characterization of  materials for process evaluation and failure analysis in the  Integrated Circuit (IC) industry as device shrinkage continues. Sample preparation is critical to TEM analysis success. In  general, most TEM analyses are performed on cross section (XTEM) samples, for instance, line monitoring, construction  analysis, embedded defects analysis, etc. It is well known that  efficient XTEM sample preparation is essential to TEM  analysis for the semiconductor industry to perform yield  improvement and metrology. At present, there are many  methods used to prepare XTEM samples. The main techniques  used are: (1) dimpling or mechanical polishing and Ar+ ion  milling (2) pure mechanical polishing and focused ion beam (FIB) milling [1] (3) FIB milling and lift-out [2-4] (4) in-situ lift-out and FIB milling [5]. Among those sample preparation  methods, FIB milling using Ga ions is widely used in sample  preparation for scanning electron microscopy (SEM) and TEM  analysis, especially in localization and investigation of failures  or defect analysis. In general, a protection layer, such as Pt or  oxide, has to be deposited onto the specific area using FIB to  avoid ion damage, curtain effects and to reduce the amount of  rounding of the top of a TEM lamella during FIB milling [6]. However, a 20-30nm amorphous mixing layer is formed at the  interface of the protection layer and sample, as shown in Fig.


1. It is a problem to analyze the surface defect or structure, which is just a few nm or less thick on the surface, because the  defect or structure will be changed or damaged during the  protection layer deposition using FIB. One solution is to use  e-beam to replace the ion beam or deposit an intermediate  buffer layer between the protection layer and sample using  another deposition method, such as chemical vapor deposition (CVD), to reduce surface damage. However, there is still a  mixing layer under the e-beam deposited Pt layer and in  addition, target localization becomes difficult when using an  intermediate buffer layer. Backside polishing is a good choice  to avoid the mixing or damage layer [7]. In this paper, a novel  method of XTEM sample preparation is demonstrated for  site-specific surface defect analysis using backside polishing. The details of the new backside XTEM sample preparation  method and some examples will be reported in this paper. Comparing to Auger electron spectrometry (AES) results on  similar defects, more detailed and precise information is  observed using TEM analysis with this method. It is therefore  a complementary technique to traditional AES analysis on


surface defects for contamination with atomic level  concentration.


Figure 1: A mixing layer (arrowed) was formed under the Pt  protection layer deposited by the FIB system.


Methods and Results


Procedures of novel backside XTEM sample  preparation


The surface defects were initially found by an inspection  system that creates a defect map file which is subsequently  used in the lab to locate the defects using a high resolution  imaging system. Specific surface defects were localized using  a navigation system with the defect map and then marked  using ion beam milling for subsequent detailed analysis. In  this paper, analysis of three different types of site-specific  surface defects was demonstrated using our novel backside  XTEM sample preparation method. In detail, the procedure  includes two parts.  Firstly, mechanical backside polishing  and secondly in-situ lift-out [5]. To avoid damage to the  defect’s surface during FIB marking, only one low current ion  beam scan was done to define the locations of markers around  the defect. In general, several marks, 1µm long by 3µm deep, were defined by ion milling, as shown in Fig. 2. For the  backside polishing procedure, the first step is to cut (or  cleave) the sample, to the desired size, from a wafer after  defect localization and marking, as shown in Fig. 3(a), which


## Surface Defect Analysis by Using a Novel Backside XTEM Sample Preparation Method


188


illustrates the backside polishing procedure schematically.


Then, a slightly larger glass cover slip is glued onto the front


side of the sample using epoxy, as shown in Fig. 3(b).  Thermal wax was used to glue the glass and sample to the  polishing holder before backside mechanical polishing. Polishing the sample down to a few µm until the FIB marks  were visible under the optical microscope (OM) from the  backside. Acetone was then used to separate the sample and  glass from the polishing holder, as shown in Fig. 3(d). Then, the sample was ready for in-situ sample lift-out. In-situ lift-out is described in detail elsewhere [5]. After the in-situ lift-out, the final sample thinning was performed in the  traditional way. The micro-structure of surface defects was  characterized using XTEM. The compositional analysis was  performed using energy dispersive X-ray spectroscopy (EDS)/XTEM, AES or Gatan energy filtered TEM (EFTEM) analysis.


Figure 2 SEM image showing the surface defect and FIB  marks.


Figure 3 (a) Using dual beam FIB system mark the failure  location with low beam current (b) Glue a glass slide on top of  the sample with epoxy (c) Polish down the sample from the  backside (d) Using in-situ lift-out tool pick up the area marked  with dotted line


Examples


Fig. 4(a, b) show a bump defect on the Al metal line structure, oxynitride/TiNx/Al, with FIB marks under SEM and OM


respectively. After mechanical backside polishing of the  sample down to a few µm, the original front side FIB marks  were easily observed in the DB FIB, as shown in Fig. 5(a). After in-situ sample lift-out and fine ion milling, an embedded  defect was found in the metal layer, which caused a metal line  bump, as shown in Fig 5(b). From further EDS/TEM analysis, O, Ti and Fe elements were detected in this defect, as shown  in Figure 6. It was suspected that the defect came from the  chamber wall or other part of the processing equipment.


Figure 4 (a) SEM image showing a bump on the sample’s top  oxynitride layer (b) An optical image showing the surface  defect with FIB marks.


Surface defect


Marks


Glass


Figure 5 (a) Ion beam image showing original marks from the  backside after polishing is complete (b) SEM image showing  an embedded defect, which caused the surface bump, was  observed with no surface damage after using this technique.


Figure 6 (a) XTEM image showing the EDS test locations  indicated by arrows (b) and (c) are the EDS spectra of  locations 1 and 2 respectively.


Fig. 7 shows some tentacle-like void defects (circled), which  were observed on corroded metal pads. In general, AES is  normally the first tool considered for pad analysis. According  to the AES data, higher concentrations of F and Al were  present on the corroded metal pads in comparison with the  normal pads. This Al pad corrosion mechanism appears to be  different from a previous report on a similar issue [8]. Therefore, XTEM analysis was required to clarify the tentacle  and void structures. The XTEM sample was prepared using  our novel method of backside polishing to protect the defect  surface. After backside polishing, the original markers and  pads were clearly observed from the backside, as shown in Fig  8(b), without any surface damage. From the EDS/XTEM  analysis, voids were found in the Al metal line and the  tentacle-like defects mainly contained alumina and F. Because  the voids crossed almost the entire metal line it is suspected  that the corrosion happened during Al pad open.


Figure 7 (a) SEM image showing the tentacle-like and void  defects on an abnormal metal pad (b) OM image showing  defect FIB marks from the backside (c) XTEM image showing  the defects and normal structures, pad and vias.


It is well known that sample charging is a problem and needs  to be overcome or neutralized for AES analysis. Fig. 8(a) shows a circle surface defect on the poly-Si/Borosilicate glass (BSG)/Si structure. Due to charging during AES analysis, it is  a known fact that unknown peaks could appear on the  spectrum at low energy range or all the peaks could shift. Several methods are suggested to overcome charging effects, such as adopting lower beam energy, tilting sample to higher  angle, depositing a conductive coating, etc. [9]. However, it  takes extra time or procedures and becomes more complex to  analyze. After tilting the sample to 75 degrees with lower  beam energy, this circle surface defect was characterized to be  a SiOx layer using AES. Fig. 8(b) shows an oxygen elemental  distribution at the defect site. An alternative method is to use  our novel backside XTEM preparation method to prepare an  XTEM sample for TEM analysis. Figs 9 (a) and (b) show the  backside polishing XTEM images of circle surface defect. It  reveals that there is no interlayer between circle surface defect  and the amorphous Si layers. From EFTEM/XTEM analysis, the results confirmed the previous AES results, as shown in  Fig. 9(c).


Figure 8 (a) SEM image showing a circle defect on the  amorphous Si layer with laser marks (b) Oxygen distribution  map of (a), showing oxygen rich (yellow color) at circle  defect.


Figure 9 (a) XTEM image showing a SiOx layer on the normal  process amorphous Si layer (b) EFTEM image of defect layer  and normal process layers (c) Oxygen distribution map of (b).


In summary, the novel XTEM sample preparation method, which employs a combination of localization, backside  polishing and in-situ lift-out technologies, provides a useful  method to prepare damage-free XTEM samples for surface  defect analysis. From our results, the method can produce a  clean, pristine surface that is well characterized and could be  reproduced, successfully.


The authors would like to thank Sam Wang for support on  sample preparation.


[1] Z.G. Wang, N. Kato, K. Sasaki, T. Hirayama, and H. Saka,


“Electron Holographic Mapping of Two-dimensional


Doping Areas in Cross-Sectional Device Specimens


Prepared by the Lift-out Technique based on a Focus Ion


Beam,” Journal of Electron Microscopy, vol. 53(2), 2004,


pp. 115-119.


[2] L. R. Herlinger, S. Chevacharoenkul, D. C. Erwin, “TEM


Sample Preparation Using a Focused Ion Beam and a


Probe Manipulator,” Proceedings of the 22nd International


Symposium for Testing and Failure Analysis, 1996,


pp.199-205.


[3] L.A. Giannuzzi, J.L. Drown, S.R. Brown, R.B. Irwin, F.A.


Stevie, “Focused Ion Beam Milling and


Micromanipulation Lift-Out for Site Specific Cross-section


TEM Specimen preparation,” Mat. Res. Soc. Symp. Proc.,


vol. 480, 1997, pp.19-27.


[4] R. Rai, S. Subramanian, J. Conner, S. Rose, P. Schani and


J. Moss, “Specific Area Planar and Cross-sectional lift-out


Technologies: Procedures and Novel Applications,”


Proceedings of 26th International Symposium on Testing


and Failure Analysis, 2000, pp.415-419.


[5] R. J. Young, M. P. Bernas, M. V. Moore, Y. C. Wang, J. P.


Jordan, Hillsboro, OR; R. Schampers, I. van Hees, “ In-situ


Sample Preparation and High-Resolution SEM-STEM


Analysis,” 30th International Symposium for Testing and


Failure Analysis, Session 16: Sample Preparation 1, 2004.


[6] N.I. Kato, “Reducing Focus Ion Beam Damage to


Transmission Electron Microscopy Samples,” Journal of


Electron Microscopy, vol. 53(5), 2004, pp.451- 458.


[7] S. Subramanian, E. Widener, T. Chrastecky, D. Jones, B.


Jones and R. Mulder, “ Investigation of Passivation


Damage from the Backside,” Proceedings of the 31


November 6–10, 2005, pp. 332-335 McEnery Convention


Center, San Jose, California, USA.


[8] J.S. Luo, M. Lo, and J.D. Russell, “The Microstructure


Evolution of Corrosion Phenomenon on Aluminum Bond


Pads,” Proceedings of the 31th International Symposium


for Testing and Failure Analysis, November 6–10, 2005,


pp. 266-273, McEnery Convention Center, San Jose,


California, USA.


[9] H.M. Lo, J.S. Luo, and J.D. Russell, “Ar sputter shadow


method (ASSM) – a novel way to overcome the charging


effect during AES bond pad analysis,” Proceedings of the


14th Conference, Microscopy of Semi conducting


Materials, April 11-14, 2005, pp. 445-448.


Application of EDS Technique for OSP Film Thickness Measurement


Prong Kongsubto and Sirarat Kongwudthiti


Spansion (Thailand) Ltd. 229 Moo4  Changwattana Rd., Pakkret, Nonthaburi 11120  E-mail: prong.kongsubto@spansion.com Tel: 662-962-1180 ext. 30509


E-mail: sirarat.kongwudthiti@spansion.com Tel: 662-962-1180 ext. 30513


OSP (organic solderability preservatives) pad is one of pad  finishing technologies that Cu pad is coated with the thin film  of a kind of organic material to protect Cu from oxidation  during storage and many processes in IC manufacturing. The  thickness of the OSP film coated over Cu layer is in order of  micrometer. Normally, during solder ball attachment process  OSP will be cleaned out by soldering flux and heat to allow  Cu to expose and attach to solder ball. The point is that if the  thickness of OSP is too thin, the film cannot prevent copper  from oxidation during storage and heat cycles. On the other  hand, if the OSP film is too thick, OSP will not be perfectly  cleaned out by flux during soldering reflow process. Hence  this will bring to the bad solder joint because the presence of  some OSP residue can result in bad solder wetting. This can  affect on the attachment of solder ball and finally lead to  significantly weak solder joint.


Therefore, thickness of OSP film is one of the most critical  factors that we have to consider and control in order to  achieve desirable joint strength. Without OSP thickness  information we will be unable to be confident in the quality of  our product and unable to control incoming quality of  substrate (BT-resin type) from supplier site. So, it is highly  necessary to measure the OSP thickness or at least for  monitoring and analysis purposes.


Unfortunately, up to today, no any non-destructive technique  has been proposed to measure OSP thickness on substrate. In  this paper, we did the big step in development the technique  for OSP thickness estimation.


EDS technique was considered to apply for OSP thickness  measurement because of short analysis time and no damaging  on the sample.


Method and Results


The large board of copper coated with OSP of a certain  controlled thickness was built and cut into 4 x 4 cm size. These boards are called ‘test coupon’. The OSP thickness on  the test coupons were measured using UV spectrophotometer. These test coupons were used as correlation units. Since the  actual OSP thickness of test coupon has already been known  from UV spectrophotometer, so we will then set up the  correlation between the thickness obtained from EDS  technique and actual OSP thickness. As OSP is organic  material so that it mostly contains carbon as the major  element. EDS will be used to analysis in terms of


quantification. By EDS quantitative analysis, electron beam  will induced to the OSP surface and either atom of carbon or  copper from OSP layer can be exited and emitted in terms of  X-ray.  If the OSP layer is thinner, the electron beam tends to  penetrate through OSP film to Cu layer. Note that copper is  from the layer of copper sheet underneath OSP (See Figure 1).  In this case some percentage of copper could be observed in  addition to carbon and percentage of carbon would be so small  compared to that from thicker OSP layer. Hence, OSP  thickness can possibly be identified by carbon and copper  percentage obtained by EDS quantification method


Figure 1: X-ray emitted from OSP coated on copper compared  between low and high OSP thickness


Determination of the EDS parameter


Experimental design:


1) Control Factors:


a. Analysis location: Analysis done on the same  points.


b. Analysis area: 10um x 6um


## Application of EDS Technique for OSP Film Thickness Measurement


193


c. E-beam aperture size: 30 um


d. Working distance: 8 mm


2) Evaluated factors;


a. OSP film thickness: 0.1, 0.150, 0.20, 0.27 um (thickness value from UV spectrophotometer)


b. Accelerating voltage: 13, 15, 17


3) Response: %Carbon, %Carbon to %Cu ratio


4) Reading point: 15 for each thickness


Figure 2: The plot of carbon percentage (left) and C/Cu ratio (right) versus OSP thickness when 13 kv was used for EDS  quantification


Table 1: the differentiation of each couple OSP thickness level  by using 13 KV beam energy (data from Figure 2)


13 KV beam energy


OSP Thickness range %C differentiation C/Cu differentiation


0.20 - 0.27 um


74.555


74.539


0.15 - 0.20 um


26.414


26.957


0.10 - 0.15 um


60.445


61.984


Figure 3: The plot of carbon percentage (left) and C/Cu ratio (right) versus OSP thickness when 15 kv was used for EDS  quantification


Table 2: the differentiation of each couple OSP thickness level  by using 15 KV beam energy (data from figure 3)


15 KV beam energy


61.178


62.569


52.178


51.416


41.765


48.439


Figure 4: The plot of carbon percentage (left) and C/Cu ratio (right) versus OSP thickness when 13 kv was used for EDS  quantification


Table 3: the differentiation of each couple OSP thickness level  by using 17 KV beam energy (data from Figure 4)


17 KV beam energy


0.20-0.27 um


73.642


74.054


0.15-0.20 um


5.784


5.581


0.10-0.15 um


57.519


56.912


Note: Differentiation value source:


Differentiation value       =


MedianL


Above equation showed the calculation to obtain the  differentiation value in Table 1-3. The results showed that %C  differentiation value has no significant difference from C/Cu  ratio, hence we can consider either %C or C/Cu ratio. By  using statistical analysis, when accelerating voltage of 13 keV  and 17 keV were applied, the differentiation values between  the OSP thickness of 0.15 and 0.20 um are quite small as seen  in Figure 2 and 4. This means that accelerating voltage of 13  kev and 17 keV are not suitable to be utilized for OSP  thickness measurement because the adjacent OSP thickness  might not be well-distinguished. However, the differentiation  value for the use of 15 keV voltage is large enough to  differentiate each OSP thickness level effectively (see Figure  3). Based on the experimental results, accelerating voltage of  15 keV will be selected as the most appropriate voltage to  measure OSP thickness by EDS technique.


Establish the correlation between C/Cu ratio and OSP  thickness


EDS quantitative analysis was performed on 6 OSP thickness  levels. The analysis was done at different points on a test  coupon for 15 readings. The results are shown in Fig.2


Once the value of C/Cu ratio was obtained by EDS  quantitative analysis, we can then convert such value to OSP  thickness through the equation in Figure 5.


Figure 5: The relationship between C/Cu and the thickness in  polynomial fit with RSquare 0.996.


Evaluate the accuracy of the EDS technique for OSP  thickness measurement


The EDS quantitative analysis was performed at the same  point on a test coupon for 15 readings and repeated this  experiment for all OSP thickness levels (0.1, 0.15, 0.2, and


0.27um). The C/Cu ratio from those readings was collected  and plotted to obtain the equation (as shown below).


Thickness (um) = -0.003 + 0.00206 (C/Cu) + 0.00006 (C/Cu)2


A deviation of thickness from calculation above and that from  UV-Spectrophotometer was found and the plot of deviation is  shown in Figure 6. The error shown in Figure 6 is only due to  the error of EDS technique itself because the EDS analysis  was done at the same point for each thickness level.


0.015 0.016


0.023


0.011


0.02


0.04


0.06


0.08


0.12


0.15


0.27


Thickness level (um)


Figure 6: Error by EDS technique. Error is obtained from the  maximum deviation of calculated thickness (results from  equation) and thickness from UV-spectrophotometer (x-axis).


EDS quantitative analysis was proved that it can be utilized  for OSP thickness estimation. The suitable setting parameter  of our EDS system for this purpose is accelerating voltage of  15 KV. The relationship between C/Cu ratio and OSP  thickness was established. The maximum error of this  technique for OSP thickness measurement is 0.023 um


[1]   C. Richard Brundle, Charles A. Evans, Jr. and Shaun  Wilson, Encyclopedia of Material Characterization, pp.120-134


Applications of Transmission Electron Microscopy and Secondary Ion Mass  Spectrometry on Crystal Defect Analysis and Electronic Characterisation of  Advanced 512Mb DRAM


Serena Lu, Esther Chen, Lang-Yu Huang, Jian-Shing Luo and Jeremy D. Russell


In memory technology, the dynamic random access memory (DRAM) is one of the most frequently used integrated circuits. The reason for this is its lower price per bit by comparison  with other semiconductor memories. In general, a DRAM cell  consists of a MOSFET and capacitor to be a switch and charge  storing unit, respectively. The cell is able to hold binary  information in the form of stored charges on the capacitor.   Fig. 1 shows the bit line (M0), borderless contact (CB), deep  trench (DT) capacitor, transfer gate (GC)  and active area (AA) structures (n-type) of a 110nm technology 512Mb trench  DRAM. The basic DRAM constituents are shown in [1].


The capabilities of analytical transmission electron  microscopy (TEM), such as high spatial resolution, micro-chemical analysis, etc. have led to an increasingly  essential role for TEM-based analysis in process development, defect identification, yield enhancement, and root-cause  failure analysis with the DRAM industry. Other authors [2] reported that more and more device leakage problems are  related to crystal defects, such as dislocations, dislocation  loops and stacking faults, due to high implant doses, shallow  junctions, and feature size shrinkage, in particular, those  defects which cross pn-junction or source/drain areas of  transistors. It was reported that grain boundaries and  intragranular defects act as electrical potential barriers and  scattering sites, which decrease the carrier transport mobility


and also serve as midgap states to increase the leakage  currents [3]. Normally, these crystal defects are believed to be  induced by implantation, poly etching, oxidation gate stack  formation, and spacer nitride deposition processes. TEM is the  most effective tool for detailed analysis of dislocations and  crystal defects. In addition, it is well known that the device’s  performance and characteristics are highly dependent on the  implanted dosage and resulting dopant depth distribution. For  instance, the Vt of MOSFETs decreases as the channel length  is shortened and also as the drain bias is increased [4]. The  influencing factors of Vt performance are device geometry  doping, gate oxide thickness and interface charge fluctuations


[5]. Recently, the influences of doping profile and  implantation on Vt behavior have been studied [6-7]. Secondary Ion Mass Spectrometry (SIMS) has the same  sensitivity as the electrical test data of Vt on the dose variation


[8]. Therefore, for new technology research and development


of ULSI devices, SIMS also plays a very important role and  has been widely used, especially to characterize ion  implantation. SIMS applications are mainly to obtain  quantitative information about contamination levels, dopant  depth profiles and chemical composition information. Furthermore, SIMS has been used for manufacturing tool  performance control and in-fab equipment troubleshooting. In  this paper, we report several examples to carry out the  applications of TEM and SIMS on crystal defect analysis and  electronic characteristics of advanced 512 Mb DRAMs.


Figure 1:  XTEM image showing the structures of AA, bit  line, transistors, CB, and DTs.


Samples were characterised using an FEI Tecnai TF20 field  emission gun TEM equipped with scanning TEM (STEM), energy dispersive X-ray spectroscopy (EDS) and Gatan image  filter (GIF) systems. To prepare the cross section TEM (XTEM) sample, first, the failure address is protected by a Pt  layer deposited and marked using dual-beam focussed ion  Beam (DB FIB). Second, the sample is cut to 30um width and  2mm long sticks using a dicing saw or mechanical polishing  and then the sticks are glued to a half copper ring with epoxy. Finally, the DB FIB system is used to thin the sticks to a  suitable thickness for TEM analysis. The top-view TEM  samples were prepared by conventional mechanical polishing


## Applications of Transmission Electron Microscopy and Secondary Ion Mass Spectrometry on Crystal Defect Analysis and Electronic Characterisation of Advanced 512Mb DRAM


196


from the backside of the chip and then fine ion milling by DB  FIB. The dosage and depth profiles of implantation were  characterized by Cameca 4550 quadrupole SIMS. The SIMS  crater depth was measured by an ASIQ alpha-step.


TEM Applications


(I) Line monitoring


The number of structures or layers which require TEM for  reasons of contrast or resolution which is not possible by SEM  increases with new technology generations due to device  shrinkage. One example is shown in Fig. 2, showing a  top-view of a DT capacitor of 90 nm DRAM product with  hemispherical silicon grains (HSG) structure [9]. It is worth  noting that XTEM imaging is not suitable to investigate the  DT node structure of new DRAM generation with HSG  structure due to structure overlap. The overlapping structures  also appear on some other scaled down structures, such as vias  or contacts. From previous reports [10-11], 3-D tomography  may be one solution for this problem.


Figure 2: Top-view TEM imaging showing NO bilayer with  HSG structures in a DT of 90 nm technology 512 Mb DRAM.


Among the possible leakage paths for DRAM products: (1) junction leakage current (2) gate Induced drain leakage (GIDL) current (3) subthreshold leakage current of NMOS  transistor. Some of the leakage mechanisms are due to crystal  or other defects at or near the pn-junction for junction leakage.  Several cases were carried out as below.


(II) Junction leakage


Figs. 3(a) and (b) show an abnormal TiSix grain, identified by  EDS and GIF/XTEM as shown in Fig. 3 (c), growth under a  bit line W contact with TiNx/TiSix glue layer of 90 nm  technology DRAM. From electronic data, this failure address  had junction leakage problem. The abnormal TiSix grain  extended to the junction, causing leakage. One of similar cases  caused junction leakage problem as well, as shown in Fig. 4. W residue was found at end of worm hole. From previous  studies, the root-cause of worm hole and W residue were due


to WF6 penetrating TiNx glue layer to react with AA during W  CB formation [12].


Figure 3: (a) (b) XTEM images showing a TiSix abnormal  grain appeared under CB bottom (c) a Ti GIF elemental map  in (b)


Figure 4:  XTEM image showing worm hole from CB to AA.


By forcing the back-gate bias voltage Vbb to different levels  during electrical characterisation, the junction and off-state  leakages, through the “off” transfer gate, can be distinguished  individually [13]. For smaller Vbb the off-state leakage is  dominant, while, for more negative Vbb, junction leakage is  dominant. For the third junction leakage case, the failure  behavior was a dependency on Vbb only from electrical  testing. Actually, the retention performance got worse with  Vbb increasing. It reveals that this failure mechanism is  related to junction leakage. A dislocation was observed near  the junction by XTEM analysis, as shown in Fig. 5.


Figure 5: XTEM image showing dislocations, indicated by  arrow, under lower magnification and (b) Tilted XTEM image  showing a dislocation under the two beam condition.


(III) GIDL


Another case is a retention fail, which from electrical analysis


showed behavior consistent with GIDL. Fig. 6 show that


dislocations were observed at the source/drain area of the fail


address. This finding is reasonable to explain the failure


mechanism. The dislocation acted as a recombination/


generation center in the band gap, when it is at or near the


surface drain junction, which causes GIDL [14]. Figure 7 is


another example of a retention failure due to a stacking fault.


Figure 6: XTEM image showing dislocations, indicated by  arrows, at source/drain area of AA.


Figure 7: (a) XTEM image showing a crystal defect indicated  by arrows, at source/drain area of AA, under two beam  condition (b) HRTEM image of crystal defect in (a).


As mentioned earlier, Vt is influenced by channel length, poly-gate CD and source/drain implantation. One case related  to Vt low will be described.


SIMS applications


For SIMS applications on DRAM, most of the cases are to  determine implantation profiles, contamination, and thin film  properties. For these cases, projected range (Rp), depth profile  and dosage are the main parameters which are used to  investigate well definition, pn-junction formation, and  resistance reduction, etc. Fig. 8 is an example of implantation  profile analysis, showing the difference of two Boron depth  profiles due to replacement of the implanter’s accelerator  parts. The dose is higher by 3.6% after accelerator  replacement.


Figure 8: SIMS depth profile showing the B dosage difference  after replacement of implanter’s accelerator parts.


To confirm if there is junction leakage at the memory functional failure site which is pointed out by plane view stain method, conductive atomic force microscopy (CAFM) [4] is  used. Under negative bias voltage (biased at chuck) at N-MOS contact area, an improper CAFM signal at N-MOS contacts(indicates N-MOS contacts leaking or n+/P-Well leaking) is observed. By specific I-V curve measurement at failed NMOS contacts by CAFM, a large reverse junction leakage  current at –1V bias voltage is confirmed.


Figure 7:


(a) The diagram indicates the SCM X-S direction and location.


(b) By SCM analysis, an extra “N-doping” signal is found within P-Well diffusion region.


Figure 8: The plane-view stain SEM result at memory function failure sites.


Figure 9: CAFM image at EMMI spot site. At –1V CAFM bias voltage, abnormal CAFM signal at NMOS contacts indicates reverse junction leakage there.


The second example using plane-view stain method:


Improper Well concentration issue can also be quickly examined by plane-view stain technique as shown in example


2. In this example, the low yield wafer is a DRAM product using deep trench structure and sub-micron process. This DRAM product suffers serious leakage failure. The I-V curve in Fig. 10 indicates a direct short failure between bit lines is  the failure cause of leakage. Because the resistance between  adjacent bit lines is about 100ohm (10mA@1V) at most of failure dies, the failure mechanism of this bit line failure is  postulated to be back-end metal bridge issue.


Figure 10: The I-V characteristic curves between bit lines indicate direct short failure.


No structure abnormality is confirmed by SEM planeview and FIB X-S inspection at all layers above poly. With the aid of the related layout at contact, poly and diffusion areas in Fig. 11, it’s almost impossible for adjacent bit line shortage without metal or poly bridge except front-end implantation failure issue.


Figure 11: Poly and contact layout structure.


Before specific SCM analysis, this new plane-view stain technique is utilized again. The plane view stain result in Fig.


12 shows different etching rate randomly distributed at P-Well regions. This phenomenon strongly implicates the extra Ndoping in P-Well regions or improper P-doping control in PWell regions. In Fig. 13, the SCM result verifies this prediction. The extra N-doping is from highly N-doped poly within deep trench capacitor through broken (discontinuous)ONO layer. In Fig. 14, the SEM X-S inspection at un-finished wafer indicates the ONO weak points at deep trench bottom corners and these weak points form a N-doping diffusion path from deep trench to P-Well region.


Figure 12: The SEM plane-view picture after 25 sec stain. The diffusion area widths at P-Well region are random distributed.


Figure 13:


(a) SCM X-S picture perpendicular to poly. The P-Well region has been changed to N-Well region near the bottom corner of deep trench.


(b) The suspected N-doping diffusion path has been highlighted in this picture (from highly-doped N-type poly to P-Well region).


Figure 14: The SEM X-S inspection after plane-view stain treatment. The suspected ONO weak points are pointed out by arrows.


Failure mechanism and root cause studies


By determining the root cause of above low yield wafers  in example 1, the by-frame failure has been verified to be  caused by mask defect issue. Mask defect may cause improper  photo definition of N- and P-Well regions at defect sites. Therefore, extra N-doping appears in P-Well regions. In  example 2, the root cause has also been found to be caused by  poor ONO quality issue. Discontinuous ONO layer at bottom  corner of deep trench provides the chance of N-doping in deep  trench poly diffusing to P-Well regions which surround the  deep trenches.


Summary and Conclusions


Front-end implantation failure issue is always very  difficult to do FA especially in fully processed wafers. This is  because implantation failure at specific area is almost structure  invisible by SEM and FIB inspections. With the help of planeview stain technique, a fast preview at the suspected Well  regions can be done by 30 sec’s plane-view stain and SEM  plane-view check. This new developed technique can greatly  shrink the FA cycle time and avoid the unnecessary job of  specific SCM. Unlike traditional X-S stain, the difficulties of  sample preparation at the specific site and precise stain time  control can be completely eliminated. Besides, one Pt-coated  film on X-S sample surface before SEM observation is  unnecessary by using plane-view stain method.


[1] Kartik Ramanujachar, “Scanning Capacitance Microscopy  at Transistor Contact Level”, ISTFA 2004, pp. 482 – 486.


[2] Coswin Lin, Chia-Hsing Chao, “SCM Application in


Semiconductor Failure Analysis and Possible Solution for


Well Inspection of Advanced Nanometer Process”, ISTFA


2004, pp. 673 - 676.


[3] M.C. Huang, C.T. Lin, J.C. Lin, “Front-end Failure  Analysis of Integrated Circuits Uing Scanning Capacitance  Microscopy”, ISTFA 2004, pp. 677 - 679.


[4] Jon C. Lee, J.H. Chuang, “Fault Isolation in Contact Level  by Using Conductive Atomic Force Microscopy”, ISTFA  2003, pp. 413 - 418.


Microelectronic Packages (FC with Ceramic Substrates) Solder Removal Method  for Failure Analysis


T. I. Shih, Tung Hung Chen


United Microelectronics Corporation, Hsin-chu, Taiwan, R.O.C. Phone: 886-03-5782258 ext. 8733742  e-mail: T I Shih@umc.com


In order to do the failure analysis on flip chip connected with ceramic substrate, solder bump should be completely removed from chip surface. The die soldered on ceramic substrate of  flip chip package is likely damaged during the removing process for the high etching and abrasion resistance of ceramic substrate as well as the poor uniformity of mechanical polish. In this paper, a thermal method for the decapsulation  of flip chip package is developed, which included heat sink removal, ceramic substrate and solder bump separation, and  solder residue clean out from the chip surface. In the last step, three temperature levels of H2N2O6 – H2O (fuming Nitric  acid) were selected for the removal of eutectic, high-lead and  lead free solders, respectively.


Sn-base solder with excellent mechanical properties has  been extensively used in the connection of flip chip package. The flip chip technology (FCT) developed since the 1960s had versatile advantages, including high pin density, low assembly cost, and high reliability [1-5].


For the method of decapsulation, the manual grind and  polish is generally used in microelectronic industry to separate the flip chip from substrate. However, the manual method takes a long time and requires considerable human resources. According to our experience, the successful rate is estimated as low as 50% for chip separation, even down to 10% for an  acceptable surface condition for the electrical probing of  failure analysis. Fig. 1 shows an example of where manual decapsulation failed in providing uniform polish. (die corner was exposed first with respect to the rest if the die. (Up to date, however, there is no method to decapsulate the flip chip  bonded with ceramics substrate.


Figure. 1:  shows the sample with damaged die corner due to poor manual polish uniformity


Fig. 2: shows the IC packaging process flow. Ball placement is a critical step for IC assembly process . Several decapsulation methods had been adopted in FA labs namely,chemical/manual (mechanical) polishing methods, autodecapsulation, and laser decapsulation.


A number of rework and replacement for encapsulated  flip chip bonding have been investigated using available commercial underfill. [6-15]. Fig. 2 shows the manual decapsulation set-up. It includes a hot plate with temperature controller, fuming nitric acid, beaker and dropper. Fig. 3  shows an autodecapsulation machine (chemical etching facility). This method is used extensively  for the  decapsulation of conventional packages such as QFP, BGA and CSP. An alternative method with laser decapsulation is  shown in Fig. 4. The laser technology allows an operator to remove the individual layers of the mold compound all the way through the lead frames and to the substrate. The use of laser decapsulation is more convenient than cut and polish method, it also eliminates the need for costly and hazardous  chemicals with the comfort of knowing the process is accurate solder ball from pad for electrical test. Although large laser power could possibly damage the sample and pose danger to people and the environment.


As a safe, reliable and effective solution, the decapsulation method introduced on this paper. For further  application, it may be demonstrated that this decapsulation  method can be applied in industry’s existing solder rework procedures. The rework is achieved by thermal cycle  treatment removal of the silicon die, followed by solvent cleaning (or use the RIE machine) of the underfill residue and  heating melting point removal of solder ball in the die for eutectic, high-lead and lead free solders. It could be also  applied in the pre-rework of flip chip package and therefore  improve the package productivity.


## Microelectronic Packages (FC with Ceramic Substrates) Solder Removal Method for Failure Analysis


214


Figure. 2 IC package Process Flow.


Figure. 3 Equipment for manual decapsulation.


Figure. 4: Auto-decapsulation  machine.


Figure. 5 Laser decapsulation facility.


The sample polished using the mechanical polish decapsulation technique is shown in Figure. 5. The ceramic substrate is successfully removed from the chip. However, it has taken lots of human and time resource, furthermore, the poor uniformity of manual polish would increase the risk of die damage. The typical failure cases referred to the asmentioned decapsulation methods were seen in Fig. 6. The  chip damaged by autodecap due to the over etching of fuming nitric acid is shown in Fig. 6a. Fig. 6b shows the die corner damage for poor uniformity of manual polishing. The melted solder ball caused by the overheating on hot plate is shown in Fig. 6c. Furthermore, the solder residue on the pad surface as  seen in Fig. 6d is attributed to the insufficient temperature of oil bath.


Figure. 5: Example of sample polished using the manual polish decapsulation technique


Figure. 6 Failure cases of conventional decapsulation. (a)Auto-decap, (b) Manual polish, (c) Die delaminated by hot plate and (d) Solder ball removal by oil bath.


Sample background


Three types of substrate generally used in this study are listed in table 1. The eutectic and lead free solders bonded with ceramic substrate and the high lead solder on organic build up  substrate are subjected to examine the feasibility of decapsulation methods. The chemical composition, physical  specification and application of each solder material are listed  in table 2. Based on the melting temperature, the solder removing temperature ranges could be determined respectively for the different types of solder residue after bump separated from substrate.


Table 1. Three types of substrate.


Table 2. Three types of solder bump in the study.


Experiment and result


A sketch of flip chip packaged with ceramic substrate and heat  sink is shown in Fig. 7. There are some differences in structure detail because of the composition of solder ball and corresponding applications.


Figure. 7 A Sketch of ceramic flip-chip package with heat sink.


This decapsulation process is divided into following steps:


Step 1 : Heat sink removal for ceramic Flip-chip packages.


(If no heat sink in Flip-chip package, goes to Step 2.)


The heat sink could be removed from ceramic Flip-chip packages with fuming nitric acid at  75 deg C for 1 min. (or  directly heating the package on hot plate to 80 deg C and  carefully removing the heat sink with handy shovel). The chip back attached with heat sink would be damaged as shown in Fig. 8. Optical microscope (OM) images for the three solder  types of flip chip package before and after heat sink removal are shown in Fig.. 8.


Figure. 8 Failure case of heat sink removal by fuming nitric acid.


Figure. 8 OM images of flip chip packages before and after  heat sink removal for (a)(b) eutectic soldered with ceramics,(c)(d) lead free soldered with ceramics, and (e)(f) high lead soldered with organic.


Step 2 :Ceramic substrate and solder bump separation.


After heat sink removal, the solder bump of package could be separated from ceramic substrate with heating to 80 deg C on  hot plate after numbers of thermal cycle treatment to induce the crack within solder ball. The solder removed surface is  shown in Fig. 9. The residual underfill material on the chip  surface is observed by OM after the ceramic substrate was  removed.


Figure. 9: IC  Chip surface with solder residue on pad


Step 3 : Underfill removal


For the package with underfill, the underfill could be removed from chip surface with fuming nitric acid of 75 deg. C  for 1  min on the hot plate. (or directly etching the package to 80  deg. C using the Reaction Ion Etcher (RIE) with Ar plasma(environmental ) and carefully removing the underfill with N2 gun.) The IC with underfill removed is shown in Fig. 10.  The  samples with the underfill partially removed are shown  in  Figure. 11.


Figure 10:  IC Chip surface without underfill residue.


Figure 11: Two failure cases of underfill removal : (a) with  underfill residue on chip. (b) with underfill residue on chip  caused by solder ball damage.


Step 4 : Solder ball residue clean out from Al/Cu pad.


For the probing of failure analysis, the solder residue needed  to be completely removed from pad surface by heating above  the melting points of solders. the solder residue needed to be  completely removed from pad surface by heating above the


melting points of solders in oil-bath (Vacuum oil type :


FOMBLIN 6/16). The solder ball residue clean out from


Al/Cu pad process is shown in Fig. 12. As referred to table 2, the solder removing temperatures for eutectic, high-lead and  lead free solders are controlled in the ranges of 180~185 deg  C, 315~320 deg C and 215~220 deg. C , respectively. The


clear pad surfaces without solder residue are shown in Fig. 13. The decapsulation process introduced in this study is


summarized in Fig. 14.


Figure. 12 The Solder ball residue clean out from Al/Cu pad process.


Figure. 13 OM images for (a) eutectic, (b) lead free and (c)high lead solders have been clearly removed.


Figure. 14 The decapsulation process for flip chip with ceramics packaged device.


The conventional decapsulation process is achieved by thermal cycle treatment removal of the silicon die, followed by solvent cleaning (or use the RIE machine) of the underfill residue and heating melting point removal of solder ball in the die. A more effective, low-cost and highly reliable method of decapsulation for flip chip packaged with ceramics has been developed in this study, which could be applied as a standard procedure in industry’s existing solder rework process. Especially, the cleanup of solder residue (within 10 minutes above solder melting point) in this method is considered to greatly improve the solder rework quality.


Thanks to UMC all Failure Analysis team for its  contributions.


[1] M. McCormack, S. Jin, G.W. Kammlott and H.S .Chen,Appl. Phys. Lett. 63, 15 (1993).


[2] L.F. Miller, IBM J. Res. Develop. 13, 239 (1969).


[3] Pang, H.L.J, T. H. Low, Xu Luhua et al. Thermal cycling aging effects on Sn–Ag–Cu solder joint microstructure,


IMC and strength Thin Solid Films, 2004 (462-463): 370-375


[4] Pang, JHL, Low, T.H, Xiong B.S., Che F.X. “Design For  Reliability (DFR) Methodology for Electronic Packaging Assemblies”, Proceedings of IEEE, 2003 Electronics Packaging Technology Conference, Singapore 2003, pp. 470-478.


[5] F. A. Stam and E. Davitt, “Effects of thermomechanical cycling on lead and lead-free (SnPb and SnAgCu) surface  mount solder joints”, Microelectronics Reliability, 2001(41), p1815.


[6] Bodan Ma, Tong, and Ann Savoca, “ Novel Fast Cure and Reworkable Underfill Materials”, Electronic Components and Technology Conference, 2000. 2000 Proceedings. 50th. P252-5, 1998.


[7] D. Suryanarayana, J. A. Varcoe and J. V. Ellerson,“Repairability of Underfill Encapsulated Flip-Chip Packages”, Proc. of 45th Electronic Components & Technology Conference, p524-8, Las Vegas, NA, May,


[8] K. R. Grebe, J. M. McCeary, D. Suryanarayana and H. M. Tong, “Method of Fabricating a Reworkable Module”, U. S. Patent 52 74913, January, 1994.


[9] 4. T. Gregorich, H. Hoang and S. Mok, “Flip Chip on Board Replacement Process”, First Symposium on Flip  Chip Technology, San Jose, CA, Febuary, 1994.


[10] S. V. Vasan, P. T. Truong and G. Gody, “Flip Chip Rework Process”, Circuit World, Vol. 21, No. 3, p16,


[11] Y. Tsukada, S. Tsuchida and Y. Mashimoto, “ A Novel Chip Replacement Method for Encapsulated Flip Chip  Bonding”, Proc. of 43rd Electronic Components h Technology Conference, p 199-204, Orlando, FL, June,


1993.


[12] F. L. Pompeo, A. J. Call, J. T. Coffin and S. Buchwalter, ‘‘ Reworkable Encapsulation for Flip Chip Packaging”,Interpak 95, Hawaii, March, 1995.


[13] B. L. Gutierrez, C-Y Yu, “Semiconductor Die Encapsulant with Intrinsic Release layer”, U. S. Patent 5371328, December 6, 1994.


[14] H. S. Cole, T. A. Sitnik-Nieters, R. J. Wojnarowski, J. H.


Lupinski, “ Reworkable High Density Interconnect Structure Incorporating a Release layer”, U S. Patent  5434751, July, 1995.


[15] M. Balpinarli G. Gela T.A. Vaughan, “Ac and Dc Testing for Electrical insulation Value of Rubber Gloves”IEEE Transactions on Power Delivery, Vol. 3, No. 1,January, 1988.


Note on the use of Principal Component Analysis (PCA) and clustering for the analysis of  wafer level ATPG data


Kartik Ramanujachar


Intel Corporation, Chandler, AZ, USA


Satish Draksharam


Texas Instruments, Stafford, TX, USA


In this contribution we explore the use of Principal  Component Analysis and hierarchical clustering in the  analysis of wafer level ATPG (automatic test pattern  generation) failure data. The method outlined will enable the  selection of representative samples for physical failure  analysis (PFA), following fault isolation with automated scan  based software tools like Fast scan [1] or Tetramax [2].


Previous statistical analyses have in some form or manner  concentrated on “commonality”; for instance the most  frequently failing pattern as a criterion for extracting  representative die for PFA. We extend this principle of  commonality by utilizing hierarchical clustering to collect die  that are more similar to one another in their manner of failure  than to others. Similarity is established by principal  component analysis of the patterns that the die in a wafer fail.


A typical ATPG stuck at test involves observing device  response to a series of patterns. The patterns are automatically  generated by scan tools like Fastscan that comprehend a gate  level abstraction of the design. The number of patterns could  be many. In the particular case for which we will display  results, 40 patterns were involved. Judging commonality using  the entire series of patterns is a large dimension problem due  to the number of patterns. Our first task is to reduce the  dimensionality of the data, or equivalently reduce the number  of comparison variables used to judge similarity or dissimilarity.


In essence Principal component analysis (PCA) is a  dimensionality reduction tool [3].  In PCA we compute the covariance matrix of the input data. A singular value  decomposition of the co-variance matrix is then conducted  and the eigen vectors corresponding to the largest eigen values  are extracted. These eigen vectors capture the directions of the


maximum variance in the input data set. Any given input  vector can then be expressed as a linear combination of the  principal components by projecting the input data onto the  principal components.  The efficacy of PCA in dimensionality  reduction is shown in figure 1. At the top of the figure we  show that the original 61 die chosen for analysis fail any  number of the 40 patterns. However in the lower panel we  plot the projection coefficients (scores) and note that only a  few scores (about 5) are required to capture the entire variance  of the original data set.


Fig 1 Fail data (top panel) and PCA analysis (bottom panel)


The second step of the analysis process is to collect together  all die that have similar scores when projected onto the  principal components.  Similarity of scores implies  commonality.  A hierarchical clustering scheme is used to  accomplish the same. Hierarchical clustering works by  collecting data points which are most closely spaced (using a  Euclidean distance measurement) and successively building a  linkage tree or dendrogram.  The dendrogram for the data set  using the scores from PCA is shown in Fig 2.


## Note on the use of Principal Component Analysis (PCA) and clustering for the analysis of wafer level ATPG data


219


Fig 2 Dendrogram (hierarchical linkage) constructed from  PCA scores.


Having clustered the die we can now examine each cluster and  run scan analysis on a few select die in any given cluster. This  analysis will provide the die that is most promising from a FA  standpoint.


Fig 3 is a snap shot of the user interface of a software tool that  was developed to implement the ideas described above. The  software was developed using the Matlab statistics tool box  and GUI tool [4]. The software uses as input, pattern names  and pass / fail status on those patterns for a  number of die in a  wafer. Using this information PCA is performed and the  scores resulting from the PCA analysis are used for clustering. In the example shown PCA was used to segregate die into five  clusters. Fast scan software was then used to run analysis on a  few die within each cluster. Those die that came back with the  best isolation could then be directed to further physical failure  analysis for the possible identification of unique root cause.


PCA analysis and clustering are useful tools for  dimensionality reduction and commonality analysis of wafer  level ATPG data. Their utility in the extraction of die for PFA  has been illustrated in this contribution.


Fig 3 GUI of software tool developed to perform PCA and  hierarchical clustering. Different colors show the different  clusters.


[1] Fast Scantm , Mentor Graphics  Corp.


[2] Tetramaxtm , Synopsis Corp.


[3] The Elements of Statistical Learning, Data Mining,


Inference and Prediction Trevor Hastie, Robert Tibshirani,


Jerome Friedman . Springer Series in Statistics


[4] MatLab Statistics tool box, The Mathworks Corp (2003).


Failure Analysis Navigation System


Connecting Hardware Analysis to Software Diagnosis


Akira Shimase, Akihito Uchikado, Yoshikazu Matsumoto, Shinichi Watarai, Shinji Kawanabe,  Takeshi Suzuki and Toshiyuki Majima


Renesas Technology Corp., 5-20-1, Josui-honcho, Kodaira-shi, Tokyo, 187-8588, Japan  shimase.akira@renesas.com


Kazuhiro Hotta and Hirotoshi Terada


Hamamatsu Photonics K.K., 812 Joko-cho, Hamamatsu-shi, Shizuoka, 431-3196, Japan  k-hotta@sys.hpk.co.jp


The progress of semiconductor device manufacturing makes  failure analyses more difficult. Analysis is usually carried out  following a typical process of fault re-generation to modeling  of the fault origin (Figure 1). In the process, layout analysis to  pick up suspect nets is getting to be a time consuming work  due to finer wiring pitch and multi-layer structure in recent  semiconductors. Especially in the case of backside analysis, it  is a troublesome routine to recognize the position in an optical  microscope image containing only gate patterns (Figure 2).


A newly developed system, named Failure Analysis  Navigation System (=FA-Navigation System), can make it  easier to extract the nets passing through the signals detected  by the hardware analysis tool, such as emission microscopes or  OBIRCH [1] analysis tools. The FA-Navigation System can  also collate these nets to suspect nets deduced by software  diagnosis tools as possible failing nets. This paper introduces  the functions of the System and shows some case studies in  actual failure analyses.


Composition and Functions of FA-Navigation System


The FA-Navigation System installed into the control software  of the analysis tool communicates with a layout viewer that  operates DEF/LEF data or GDS data in another workstation (Figure 3). Main functions of the system are as follows.


Fault net/plug assumption/extraction


(by software diagnosis, IDDQ/scan methods etc.)


Fault phenomenon re-generation


(by tester etc.)


Physical analysis


(by SEM/TEM etc.)


Modeling


Fault site localization


(by hardware detection,


Emission/OBIRCH etc.)


Logic/circuit analysis  Layout analysis


Figure 1: Process flow example of failure analysis. The  failure is narrowed down to its origin following this process for effective counter measures.


Figure 3: Composition of FA-Navigation System and  connection between emission microscope or OBIRCH  analysis tool and EDA tool, such as a layout viewer.


Emission Microscope or  OBIRCH Analysis Tool


EDA Tool


FA-Navigation  System


Control  Software


Layout  Viewer


DEF/LEF


＋GDS


Ether net


PC


WS


Figure 2: Optical microscope image from surface and backside. In the case of backside observation, only gate patterns can be recognized.


Surface observation


Backside observation


Multilayer  structure


Flip chip  packaging


## Failure Analysis Navigation System Connecting Hardware Analysis to Software Diagnosis


221


(1) Locking the coordinate of the optical microscope stage of  the hardware analysis tool to the coordinate of the layout data  using selected proper mark set (Figure 4A)


(2) Setting and sending the location of the detected emissions  or OBIRCH signals to the layout viewer (Figure 4B)


(3) Sending commands to the layout viewer to extract nets  passing through the signals, receiving and listing up the names  of the nets (Figure 4C)


(4) Displaying the nets with histogram data that shows how  many signals are related each net visually (Figure 4D)


(5) Displaying the net information by highlighting selected  nets (Figure 4E)


Software diagnosis is applied to point out possible nets  explaining failure phenomena. Fault diagnosis of scan based  test, functional test and IDDQ test are utilized in our company  now [2][3]. In this paper, the IDDQ fault diagnosis is  especially useful for case studies. The result of the software  diagnosis can be loaded in the analysis window of the FANavigation System (Figure 4C), and the System correlates the  result to the nets extracted by the hardware analysis and  displays coincident nets in a sorted manner to make the failure  analysis easier. Example of this function will be presented in  some case studies below.


Case Study (1)


In the first case, the emission microscope detected two  emissions distanced 1300um apart in a standby condition. The  FA-Navigation System showed that only one net passed  through these two emissions (Figure 5A) and detailed layout  analysis showed that the gates of the net were located at the  emission sites (Figure 5B{1}). The net was obviously related  to the failure, so the fault localization went to the next step  named EBAC analysis (see Appendix). The EBAC image  showed the shape of the net and EBIC signals in the net at high  acceleration voltage were observed at the site connecting to  the substrate (Figure 5C{1}). Another EBIC signal unrelated  to the suspect net was observed (Figure 5C{2}). This indicated  that the second net was connected to the first net with the two  emissions.


Figure 4A: Alignment window of the FA-Navigation  System. Three point coordination lock and layout  image. Each position can tune in this window.


Figure 4D: Detailed analysis window of the FANavigation System with histogram. Highlight nets (more  than one) can be selected in this window.


Figure 4E: Analysis window with net highlight. The  image is loaded from the connected layout viewer.


Figure 4B: Area setting window of the FA-Navigation  System. Area data is sent to the layout viewer.


Imaginary  OBIRCH   image


Figure 4C: Analysis window of the FA-Navigation  System. Extraction command was sent and the extracted  nets were listed up in the table.


Through detailed layout analysis on two nets it was determined  the signals ran parallel to each other (Figure 5B{2}). Finally, a  short defect (particle related) between the nets was observed  using the SEM.


In this case, it took less than 10 minutes to identify the net  after detecting the emissions. The FA-Navigation System can  indicate suspect nets without the result of software diagnoses  in some cases such as this case, and shorten time for the layout  analysis.


Case Study (2)


In the next case of a standby current failure, multiple light  emissions were detected (Figure 6A), and the IDDQ test based  software diagnosis tool suggested that the failure was a short  defect. First, the FA-Navigation System extracted nets passing  through the emissions. However, at this stage, it was difficult  to recognize which nets were related to the failure, because  two nets similarly contained the fifteen emissions (Figure 6B  left). Next, the result of the software diagnosis was loaded into  the System and correlated the nets extracted from the  emissions. The nets in agreement were highlighted and sorted  by frequency (Figure 6B right). In the next step, a function  installed in the FA-Navigation System was used to check the  combination of the nets. This method assumes that the  emissions are respectively attached to nets, if the nets are not  too close. First, an operator moves the cursor and clicks on the  histogram bar indicating the most likely net to fail, NET001, (the net with largest number of emissions in many cases, and  the net coincident with the result of software diagnosis in this  case), resulting in a change in color of the affected rectangles (Figure 6C left). Second, the net with the largest number with  unchanged color, NET003, was chosen, and the color of  secondary affected rectangles was changed to another color (Figure 6C middle). On the third step, the same procedure was  carried out on NET007 (Figure 6C right). This result showed  the most likely set of the nets. Next, the nets were analyzed  using the EBAC analysis tool. FIB probe pads were made on  the NET001 and the NET003. The EBAC image acquired  from the NET001 also showed the shape of the NET003. This  investigation confirmed the existence of short circuit between  these two nets (Figure 6D). The detailed layout analysis  pointed out the closest site where a defect could exist (Figure  6E). SEM inspection and EDX analysis found barrier metal  residue on the suspect failing site.


It was a troublesome routine to check nets in each emission in  the case of multiple emissions. On the other hand, the System  prefers such a case, since the areas of each emission can be  easily set and the System picks up and shows possible nets  with a histogram. The correlation with the software diagnosis  result is also helpful, and optional emission distribution  function can be used to classify the emissions into net set.


Parallel run of the two nets


{1}


{2}


Short defect caused


by a particle here  Parallel run of nets


EBIC signal  in other net


Emissions  at the gates


EBIC signal   related to


of the net  the emissions


Figure 5B:


Layout image of the net. Two light emissions  were located at the two  gate positions in the  suspect net {1}. Parallel  lines existed in the net  with the EBIC signal  detected by the EBAC  analysis tool {2}.


Figure 5C:


EBAC image of the net. EBIC signal belonging  to the suspect net is at  the bottom of the image {1}. An additional EBIC  signal was found in the  middle of the suspect net {2}. The EBIC signal  was assumed to have  short circuit in these


Figure 6A: Multiple light emissions from the sample in  standby state. The IDDQ based software diagnosis  expected a short defect.


Figure 5A: Analysis window of the FA-Navigation System and the magnified light emission image superimposed on the optical microscope image.


Two emissions were detected at a distance of 1300um apart. The result of extracted nets related to these emissions indicated that both emissions were located on only one suspect net.


Only one net contained both emissions.


Case study (3)


This case is one of recent backside emission analysis. The  emission tool used in the case was equipped a cooled-CCD  detector that could only detect emission with the tools very  sensitive 20X lens and could detect two emissions from  backside of silicon. However, it was practically difficult to  recognize the gate pattern at this magnification (Figure 7A). After locking the coordinates using the peripheral patterns, the  FA-Navigation System extracted nets contained in these two  emissions. First, the number of the nets listed up on the table in  the analysis window was over a hundred because of fine pitch  patterns and multiple wiring layers in 90nm process rule. At  this stage, it was impossible to identify suspect nets. The result  of the IDDQ software diagnosis was loaded and correlated to  the nets on the table. As a result, four nets were contained in  both results. The FA-Navigation System re-sorted these nets in  upper columns and highlighted the result (Figure 7A). The  layout image indicated these four nets were two net chains, that is, one net drove another net. Moreover, the net chains ran  parallel a long way, so a short circuit between the pairs was  suspected (Figure 7B right). Since light emission generally  occurs at a gate in intermediate voltage, it was reasonable that  the gates of the NET001 and the NET005 were assumed to  generate the emissions because of the short defect. Next, the  OBIRCH analysis by flowing current between FIB probe pads  on NET001 and NET005 showed a turning back image (Figure  7B left). The image was the evidence of short circuit in these  nets and indicated the position of the short effect. The SEM  inspection after removing the upper layers found a short defect  originated from the fabrication process at the turning back  point.


NET003


NET001


Figure 6D: EBAC image constructed by the current detected from the FIB pad on the NET001. Bright reaction of the NET003 was a hard evidence of short circuit to the NET001.


Click!


NET007


Figure 6C: Histogram of the detailed analysis window  in the FA-Navigation System. Clicking NET001, NET003 and NET007 showed the distribution of the  emissions.


(These emissions  were observed in good die also.)


NET 001


Figure 6E: Layout image and its magnified image of the  closest site. The NET003 was close to the NET001 at the  right upper area. Residue of barrier metal was found at  the closest lower layer.


Figure 6B: Histogram of the detailed analysis window in the FA-Navigation System. Left part showed a raw  histogram of extracted nets, and right part was the  histogram after correlation with the result of the software diagnosis based on the IDDQ test.


Figure 7A:


Analysis window of the FANavigation System and


magnified light emission image


superimposed on the optical


microscope image.


Two light emissions were detected.


Four nets coincided with the result


of the software diagnosis were re-sorted   in the table of extracted nets.


The gate patterns were not able to


be recognized from the backside of


the substrate at this magnification.


NET 01NET 02


22112211111111


Coun


Cold-CCD detector Objective lensà 20X


NET001  NET002


2 2 1 2 2


1 1 1 1


1 1


Count


oled CCD de ector 20X


NET005 NET006  NET003 NET004  NET007  NET008  NET009  NET010  NET011  NET012  NET013  NET014


In the case of the backside analysis, only gate pattern could be  observed and it is considerably difficult to recognize where the  pattern is. Further, since emissions are faint at the highest  magnification in some cases, the detection of the emission  must be often restricted to lower magnification. At that time, the location of the emissions in the optical microscope image  is more difficult. The FA-Navigation System has a function to  lock the microscope and the layout coordinate in the peripheral  area with characteristic patterns, so the System makes it easier  to recognize the emission position in the case of backside  analyses too.


Case Study (4)


DEF/LEF data was used in above case studies as a layout data. There may be cases that DFE/LEF data is not left in the design  database, the data is difficult to open to fabrication sites or it  may require a tiresome security procedure to get the data. In  addition, even if the DEF/LEF data exits, macro cells are black  boxes in the data. GDS data is easier to prepare, contains  layout data of whole region and the data is certainly reflected  to the final design, so the recent FA-Navigation System has an  additional new option to trace net connection using GDS data.


Figure 8A: Emissions displayed in the FA-Navigation window. This low magnification (5X) image showed the  whole emission positions.


Figure 8B: Rectangles representing emissions enclose  semi-automatically. After setting some thresholds, ten  rectangles were enclosed


Figure 8C: Extracted nets and a suspect net highlighted in the analysis window. The result of the extracted nets  and checking the frequency of passing through  rectangles indicated the most suspect net containing  nine boxes.


Figure 7B: Layout and OBIRCH image at the extacted  nets. The layout image showed the relationship between four nets. The emissions were possibly at the gates of the NET001 and the NET005 with long parallel running. The OBIRCH image was acquired by current flow from the NET001 to the NET005.


Current path


between two nets


OBIRCH reaction turn back at the short point


NET002


NET005


NET006


NET 002


Layout image  OBIRCH image


Emissions


Figure 8D: Layout and EBAC image of suspect net.


The net expanded to left hand side in the layout image. On the other hand, the EBAC image stopped at the  center of the net. The magnified EBAC and SEM image  at the area showed the stopped position in the EBAC image.


Layout image


EBAC image


EBAC


The emissions detected in a sample containing function and  DC test error were displayed in the FA-Navigation window  after the coordination lock (Figure 8A). Emission areas were  set using other optional auto-enclosing function by adjusting  some thresholds (Figure 8B). Sending the emission area to the  layout viewer, the net trace was executed and the extracted  nets were displayed (Figure 8C). The EBAC tool analyzed the  most suspect net on the table and indicated the net was broken  in the middle way (Figure 8D). Finally, cross sectional SEM  inspection found a shrunk through hole did not reach to lower  wire at the breaking point.


Discussion on the System performance


The FA-Navigation System consists of hardware analysis tool, PC controlling the hardware and WS executing layout  operation (Figure 3). The WS with 2.4GHz MPU and 64GB  memory is used for failure analysis, and “Laker”/Novas is  applied in the case studies (1)-(3) and “Ismo”/JEDAT in the  case study (4) as the layout viewers. (Since we are checking  some layout viewers for the next FA-Navigation System that  will be more convenient on some performance, ease of the  operation and familiarity to many operators, the layout viewer  is possibly altered in the future.)


One of the important features of the System is a speed for  extracting nets, which mainly depends on the performances of  the WS and the layout viewer itself. In the case of analysis  using the DEF/LEF data, the time for extracting nets is short, since the net extraction is executed by text base search. In the  case of the GDS data, the extraction is executed by tracing  polygons described by the GDS data one after another. As a  result, the net trace takes definite time. For example in the case  study (4), it took 32 seconds for tracing total 64 nets passing  through each emission (The sample was 0.35um process LSI  with three aluminum layers, the size of the GDS data was  30MB.). Even in a recent LSI with about 3GB GDS data, the  net tracing test showed that the 23 nets tracing (3635 polygons  in the GDS data) took 105 seconds. If too many or too wide  emission areas are set, the required time is getting to be  extremely long. However, if the areas are suitably set and the  WS and the layout viewer are selected to have properly high  performance, the extraction time can be reasonable for failure  analysis.


Now, the System has been applied to actual failure analyses in  functional combination with another tools, such as the software  diagnosis and/or the EBAC analysis and so on. This combined  analysis methodology is getting to be commonly adopted and  improves the turn around time and the success rate of the  failure analyses.


While performance such as extracting time is improved, investigations on how to use the System and proposals on what  should be improved for the practical usage of the System or on  what functions should be installed in the System for effective  failure analyses will be necessary. As a result, the System is  expected to be refined and more useful for future devices.


The newly developed FA-Navigation System can connect the  sites of signals detected by emission microscope or OBRCH  analysis tool with the nets described in layout data. The  combination of software diagnosis, the layout analysis using  the FA-Navigation System and EBAC analysis (see Appendix) is effective for recent failure analyses. The combined failure  analysis process is put into a practical use now: Four case  studies showing the validity of the process are presented.


The authors appreciate to whom related to the development of  the failure analysis tools, Hitachi High-Technologies, Hitachi  Science Systems, Rigaku Aihara Seiki, Sanyu Seisakusyo and  Sanwa Koki for the EBAC analysis system and Hamamatsu  Photonics K.K. for the FA-Navigation System.


[1] Nikawa K. and Tozaki S.,


“Novel OBIC observation method for detecting defects in


Al stripes under current stressing”,


ISTFA, pp.303-310 (1993)


[2] Yamazaki I. Yamanaka H. Ikeda T. Takakura M. and


Sato Y.,


“An Approach to Improve the Resolution of DefectBased Diagnosis”,


Proc. 10th Asian Test Symposium, pp. 123-128 (2001)


[3] Sato Y. Yamazaki I. Yamanaka H. Ikeda T. and


Takakura M.,


“A Persistent Diagnostic Technique for Unstable


Defects”,


Proc. International Test Conference, pp. 242-249 (2002)


[4] Mizukoshi K. Oyamada T. Shimase A. Matsumoto K.


Yorisaki S. and Majima T.


“Fault Localization Using Electron Beam Current


Absorbed in LSI Interconnects,”


Proc The 2004 International Meeting for Future of


Electron Devices, Kansai, Kyoto, JAPAN, pp. 391-392 (2004)


[5] Perunglam S. and Gleason A.,


“Via Chain Failure Analysis using a Combination of EBeam and Optical Beam Techniques,”


ISTFA, pp.259-261 (2003)


Appendix


Analysis using Electron Beam Current absorbed in Nets


As this method has been often used in recent analyses in our  company and the method is referred to in the case studies of  this paper, it should be briefly introduced here.


We developed a tool constructed of a SEM, prober in vacuum  and current amplifiers (Figure A1), applied it to actual failure  analyses and named the method “EBAC (=Electron Beam  Absorbed Current)”[4]. The principle is similar to the “RCI (=Resistive Contrast Imaging)” method [5] (Figure A2). When  irradiated high-energy electrons penetrate into a  semiconductor device, electron current is absorbed in the wires  of the device. The two-dimensional absorbed current image  that shows the path of current flow is helpful for failure  analyses involving open and/or short defects (Figure A3 & A4). In actual semiconductor devices, images acquired by the  EBAC tool vary with the electron accelerating voltage (Figure  A5). EBIC signal appears in higher voltage condition at the  output position of CMOS circuits as a pair of bright and dark  signal. Since the EBIC signal is clearer and stronger than the  EBAC signal in showing the current path, it is often used for  recognizing the failing nets.


Figure A1: Main compositions and its internal  components of EBAC analysis tool


SEM Optics


Marking Unit


for test element group analysis


EBAC Main  Amplifier


Analyzing Chamber


Loading Chamber


Objective Lens


EBAC Pre-Amplifier


Gas Nozzle


Mechanical Probe


Sample Stage


Prober Stage


Piezo Actuator


SEM image


Vanish reaction


Open defect


Net layout shape


EBAC reaction


Figure A3: Open defect example EBAC analysis.


Open defect was found at the position where the EBAC  reaction vanished.


Figure A4: Short defect example of EBAC analysis.


Unexpected net connected to the net under analysis by a  short defect caused by a problem of fabrication process.


EBAC    image


Extra reaction


Net under analysis


Short defect  found by SEM


Unexpected net


Figure A2: Detection of electron beam absorbed  current image and secondary electron image from the  surface of test element group with via chain.


Via Probe


SE Detector


Amplifier


Probe


GND side Amp side


Amp. side


Recognition  impossible


Scan


Defect


GND side


Open/High-resistance Failure


Electron Beam


Figure A5: EBAC image dependence on the  accelerating voltage. EBIC reaction appears in higher  accelerating condition.


V0=10keV


V0=20keV


V0=30keV


EBIC signal


Pad


EBAC signal


Usage of SAM on Fatigue Crack of Solder Joint Induced By Thermal Reliability Test


Tung Hung Chen, T. I. Shih


United Microelectronics Corporation, Hsin-chu, Taiwan, R.O.C. Phone: 886-03-5782258 ext. 8736481  e-mail: east_chen@umc.com


Thermal fatigue cracking of lead-free solder joints within flipchip packages was investigated in this study by using scanning acoustic microscope (SAM) and SEM. The distribution of substrate delaminations was mapped with SAM of high depth resolution and observed in cross-section with SEM to find the mechanism of crack growth during thermal reliability tests. The study revealed that the interfacial crack always initiated from the pad edge. This is attributed to the coefficient of thermal expansion (CTE) mismatch between  underfill and the PCB substrate. The propagation of fatigue  crack within solder joint is closely related to the morphology of interfacial/intergranular intermetallic compound (IMC) formed at the elevated temperature of thermal cycle.


Solder joints within flip chip packages have suffered from the thermal reliability issue due to the CTE mismatch among package components. Several researches on solder joint structure and materials have been conducted to reveal the mechanism of crack initiation and propagation during the thermal-mechanical process [1-4]. As nondestructive analytical tool, C-mode scanning acoustic microscope (CSAM) is usually adopted to examine the void, fracture, or even micro crack occurring within flip chip packages. In this  study, solder joint cracking induced by thermal shock was  investigated by using SAM and SEM. According to the crosssectional SEM observation for the C-SAM located region, the influences of   the morphology of intermetallic compound(IMC) formed at solder/pad interface and solder grain boundaries on the propagation of a fatigue crack are  discussed.


The Sn-Ag soldered flip chip on a Ni metallized Cu pad of  substrate was subjected to a reliability test with numbers of thermal cycles between -40 to 125C degree in an air-to-air chamber and held at each temperature for 20 min. A Sonikon  MUCH III scanning acoustic microscope (SAM) with a transducer frequency of 110 MHz was used to detect the delamination of solder bonds across the flip chip. The defectmapped sample was then cross-sectioned the defects with grinding/polishing machine, and observed under SEM to look for the signs of crack initiation and propagation.


Fig. 1a shows the C-SAM images of flip-chip packages before and after the thermal cycle test. The bright contrast corresponds to the delamination region of solder joints with substrate. The diagonal distribution of delamination indicated the die corner suffered a higher thermal stress than the die edge. With adjustment of the gate range of the SAM waveform, a suspected reflection signal colored in red was  mapped out at the upper-left comer as labeled B in Fig. 1b.


Figure 1. C-SAM images showing solder bond delamination


(a) with bright contrast; (b) depicted in red.


For the region with serious C-SAM reflection signal as  labeled "A" in Figure 1b, the delamination between underfill  and substrate was clearly observed in the cross-section SEM  image of Fig. 2. The delamination induced by thermal cycling is attributed to the CTE mismatch between underfill and  substrate and considered to initiate the crack from the pad edge at the bottom of the solder joint.


Sn-Ag solder


Underfill


PCB substrate


Figure 2. Cross-section SEM image showing underfill/substrate delamination by  the solder ball.


## Usage of SAM on Fatigue Crack of Solder Joint Induced By Thermal Reliability Test


228


Figure 3. Cross-section SEM images showing (a) crack along the interface of solder bump and metallized pad; (b) close-up  picture of (a)


Fig. 3 shows the Cross-sectional SEM image of the solder bump at the suspected sits B in Fig. 1b. The Ag-Sn intermetallic compound (IMC) layer in bright contrast is  continuously formed between the solder ball and Nimetallized Cu pad. The fracture grown along the uneven  IMC/solder interface is clearly observed in the high  magnification image shown on Fig.3b . That the joint crack initiated from the pad edge was inferred from the opening between the underfill and substrate interface during the  thermal cycles. The propagation of the interface crack  between solder bump and IMC layer is mainly attributed to the thermal expansion coefficient mismatch and weak intercrystalline boundary between them. The continuous thick  layer of brittle Ag6Sn5 IMC formed on the pad surface has  been considered to deteriorate the stress reliability of flip chip package. [5]


Figure 4. Cross-section SEM image showing interfacial crack  propagation  into the solder bump along IMC path.


Another aspect of fatigue fracture propagation within the solder bump is shown in Fig. 4. For the center region of die with less thermal shock, as marked C in Fig. 1b, the interfacial crack initiated from the pad edge deviated from the solder/pad interface and propagated into the solder ball at the discontinuity of the IMC layer on the pad. However, the morphology of IMC precipitated from solder grain boundaries still affected the propagation direction of the crack within the solder ball due to the vulnerable inter-crystalline boundaries  formed at elevated temperatures of the thermal cycle. Apart  from the IMC boundary, the crack was considered to pass  along the solder grain boundaries, which lose their strength


during the thermal cycle [6]. The mechanism of thermal fatigue fracture through the solder joint is illustrated in Fig. 5.


Sn-Ag IMC


Ni pad


Figure 5. Schematic of thermal fatigue stress and crack propagation.


SAM with high frequency probe is a powerful tool to reveal the delamination within flip chip packages caused by thermal reliability testing. The function of colored reflection image is utilized to locate the solder bump of suspected disbonding. Cross-section SEM images revealed that the intergranular  fatigue crack which initiated from the pad edge was due to expansion coefficient mismatch between the underfill and  substrate. The continuity of Ag-Sn IMC formation at the solder/pad interface and solder grain boundary dominates the  fracture propagation within the solder joint.


[1] G. W. Xiao, Philip C. H. Chan, Annette Teng, Jian Cai,and Matthew M. F. Yuen, “Effect of Cu Stud  Microstructure and Electroplating Process on  Intermetallic Compounds Growth and Reliability of FlipChip Solder Bump,” IEEE Trans-CPMT-A, Vol 24, No.


4, (2001), pp. 682-690.


[2] Jeong-Won Yoon, Seung-Boo Jung, “High Temperature Reliability and Interfacial Reaction of Rutectic Sn–


0.7Cu/Ni Solder Joints During Isothermal Aging”,Microelectronics Reliability, 2005, in press.


[3] P. L. Tu, Y. C. Chan, K. C. Hung, J. K. L. Lai, “Study of  micro-BGA Solder Joint Reliability”, Microelectronics Reliability, Vol 41, (2001), pp. 287-293.


[4] P. L. Tu, Y. C. Chan, and Joseph K. L. Lai, “Effect of  Intermetallic Compounds on Vibration Fatigue of BGA  Solder Joint,” IEEE Trans. Advance Packag., Vol 24, No. 2, (2001), pp. 197-205.


[5] P. L. Tu, Yan C. Chan, and J. K. L. Lai, "Effect of Intermetallic Compounds on the Thermal Fatigue of Surface Mount Solder Joints", IEEE Trans. Comp.,Packag., Manufact., Vol 20, No. 1, (1997) pp. 87-93.


[6] R. E. Reed-Hill, R. Abbaschian, Physical Metallurgy Principles, PWS Publishing Co. (Boston, MA, 1994), pp.


870.


Laser Based Defect Localization for the Failure Analysis of Advanced Product


W.Y. Cheng, T.Y. Chiu, Jon C. Lee, J.Y. Chiou


Taiwan Semiconductor Manufacturing Company,


No 6, Creation Rd.2, Science-Based Industrial Park, Hsinchu, Taiwan 300, R.O.C.


Tel:886-3-5636688 ext.7072181 Fax:886-3-5787778


Richard_cheng@tsmc.com, TYChiucd@tsmc.com, clee@tsmc.com, jychioua@tsmc.com


Failure analysis is the key for yield improvement in  semiconductor industry. Based on FA results, the failure root cause of low yield can be found and then a failure mechanism can be proposed to make process or design change to improve yield.


Several methods and tools have been used for FA defect  isolation; emission microscopy (EMMI) is the most popular  tool among these techniques. But for advanced products, the  working voltage of chip is getting smaller, thus many emission spots from normal transistors will be observed,which indeed affects the judgment on the emission spots  from killer defects and increases the Failure Analysis (FA)difficulty. Laser scanning microscope (LSM) based techniques have been powerful defect isolation methods for many years. Contact/Via higher resistance, metal bridge and  S/D contact open induced hot spots can be detected by LSM  techniques but they are not easily caught by EMMI [1-2].


Furthermore, the defects are usually at the same locations of  spots that reduce much time for layout tracing before Physical Failure Analysis (PFA).


In this study, Checkpoint Infrascan 200TD was used to  perform defect localization. It is a laser based tool and with  two different wavelengths of laser source (1064 nm/1340nm). It also provides several control parameters to enhance the  capability of defect detection, such as laser power, scan speed, scan direction, bandwidth and bias condition. By the  selections of laser source and bias conditions, various techniques are  available, these include Thermally Induced  Voltage Alteration (TIVA) [3], Light Induced Voltage Alteration (LIVA) [4], Optical Beam Induced Resistance Change (OBIRCH) and Optical Beam Induced Current (OBIC).


It can also link to tester for Soft Defect Localization (SDL)


[5] and Laser Assisted Device Alteration (LADA) performing


[6]. In this article, TIVA and OBIRCH were used to get defect  locations. Some case studies will be discussed below.


The principle of OBIRCH/TIVA is when a laser beam  irradiates a circuit, it will cause the resistance change due to  the heating effect resulted from laser scanning [7].


Resistance change will induce current or voltage change  depending on whether the bias condition is constant voltage  or constant current. The former is OBIRCH and the latter is  TIVA [8-10].


Three FA cases with 80nm/90nm technologies were demonstrated; metal direct short, poly leakage and contact  high resistance were found in these cases. In order to get  better image resolution, backside thinning and polish were  performed for some samples.


Case study 1


In this case, power short was the major failure mode. The IV curves of the failed samples indicated large current  leakage between Vdd and Vss. Excepting that, direct short  phenomenon was also found on some neighboring pads by  HP4156 parametric measurement. Infrascan 200TD was applied to localize the failure site for the front side detection. A superimposed OBIRCH image showed distinct hot spots  beside probing pad (Figure 1a). Based on the comparison of  layout and superimposed image, the bridge type defect under  metal four was suspected. Focused Ion Beam (FIB) crosssection was performed to check the hot spot area step by  step, and Cu under polish of metal three was observed from  the cross section Scanning Electron Microscope (SEM)image (Figure 1b). The subsequent Transmission Electron  Microscope (TEM) analysis was also done to obtain clearer image (Figure 1c).


## Laser Based Defect Localization for the Failure Analysis of Advanced Product


230


Figure 1-a: Superimposed image shows the hot spots  locate on the edge of probing pad. (50X)


Figure 1b: FIB cross section image of metal-3 under polish.


Figure 1c: TEM image shows metal-3 under polish.


Case study 2


This case was a SRAM sample that suffered block failure. Backside detection was performed and a constant  current was applied for TIVA execution. Superimposed TIVA  image showed that the hot spots located in the circuit block  of I/O write buffer (Figure 2a). By the SEM Voltage Contrast (VC) inspection, brighter VC of N-poly contacts in NAND  gate was found (Figure 2b). A FIB cross-section showed abnormal salicide migration that induced N-poly leakage to  Oxide Define area (OD) (Figure 2c). A TEM image shows  clearer physical structure in figure 2d. The following Energy


Dispersive X-ray analysis (EDX) analysis indicated cobalt  existed in the center of N-poly and OD.


Figure 2a: Superimposed TIVA image shows hot spots locate on the I/O write buffer. (100X)


Figure 2b: SEM voltage contrast reveals abnormal contact  VC of N-poly.


Figure 2c: FIB cross section shows salicide migration of Npoly.


good


bad


Figure 2d: TEM image shows salicide migration inducing  N-poly leakage  to OD


Case study 3


This case was a functional failure and with local distribution. Backside EMMI detection could only get very  weak hot spots and it was difficult for layout tracing because  of high pattern density issue. By using laser based technique, the superimposed TIVA images with better resolution were  obtained (Figure 3a), which was very useful for locating the  hot spots exactly. From the voltage contrast comparisons  between the suspected site with hot spot and normal site, the gray Voltage Contrast (VC)  of a P+ contact was found(Figure 3b). A TEM image indicated an abnormal layer beneath the contact bottom (Figure 3c). The further Energy Dispersive X-ray analysis (EDX) showed the layer was oxygen rich material that caused high contact resistance.


Figure3a: Better image resolution with TIVA signal.


Figure 3b: SEM voltage contrast found abnormal contact VC of P+ contact.


Figure 3c: TEM images reveal abnormal interface between  contact bottom and salicide


Based on this study, laser based techniques are very  useful for the failure analysis of advanced products. By the  selection of control parameters, Infrascan 200TD provides  several capabilities of failure site localization and applies to  different failure modes. Better image resolution provided by  LSM technique makes the layout tracing clearer. Excepting  that, hot spot and layout study is also very important, it will  provide some hits to find out the failure location.


[1] H.W. Yang et al., “Novel IR-OBIRCH Application in Gate Oxide Failure Analysis,” Proce. 11th IPFA 2004, Taiwan, pp. 299-302.


[2] Lim Soon et al., “Application of IR-OBIRCH to the  Failure Analysis of CMOS Integrated Circuits,” Proce.


10th IPFA 2003,Singapore, pp. 86-91.


[3] Cole et al., IRPS (1999), p.129.


[4] Cole et al., IRPS (1994), p.388.


[5] M Bruce et al., ISTFA (2002), p.21.


[6] Jeremy A. Rowlette, Travis M. Eiles,., “Critical Timing  Analysis in Microprocessors Using Near-IR Laser Assisted Device Alteration ”, ITC 2003, p264 ~ p273.


[7] M. Tagami et al., “A New Failure Observation in 0.10-um-Wide Cu Lines Using Optical Beam Induced Resistance Changes (OBIRCH),” IEEE (2001), pp. 95-97.


[8] Kiyoshi Nikawa and Shoji Inoue, “New Capabilities of  OBIRCH Method for Fault Localization and Defect Detection,” IEEE (1997), pp. 214-219.


[9] K. Nikawa, “Optical Beam Induced Resistance Change (OBIRCH): Overview and Recent Results” IEEE (2003),pp. 742-743.


[10]F. Beaudoin et al., “Current Leakage Fault Localization  Using Backside OBIRCH” Proce. 8th IPFA 2001,Singapore, pp. 121-125.


Pulsed Laser Digital Signal Integration Algorithm


ACT Quah, JCH Phang


Centre for Integrated Circuit Failure Analysis & Reliability National University of Singapore


LS Koh, SH Tan, CM Chua


SEMICAPS Pte Ltd, Singapore


This paper describes a pulsed laser induced digital signal  integration algorithm for pulsed laser operation that is  compatible with existing ac-coupled and dc-coupled detection  systems for fault localization. This algorithm enhances laser  induced detection sensitivity without a lock-in amplifier. The  best detection sensitivity is achieved at a pulsing frequency  range between 500 Hz to 1.5 kHz.  Within this frequency  range, the algorithm is capable of achieving more than 9 times  enhancement in detection sensitivity.


A series of laser induced techniques have been developed over  the past decade to detect laser induced effects on integrated  circuits. These techniques have made the scanning optical  microscope an essential tool for active fault localization. These techniques involve the use of a scanned infrared laser  beam to stimulate failures which are sensitive to thermal  stimulation or carrier stimulation. Essentially, they can be  categorized as power alteration techniques or tester based  techniques [1].


The power alteration techniques based on thermal stimulation  include Optical Beam Induced Resistance Change (OBIRCH) [2,3], Thermally Induced Voltage Alteration (TIVA) [4,5], Thermal Beam Induced Phenomenon (TBIP) [6] and  Externally Induced Voltage Alteration (XIVA) [7], which are  ac-coupled detection systems. A new dc-coupled power  alteration technique called Differential Resistance  Measurement (DReM) [8] has also been developed. These  techniques are effective for localizing resistive effects such as  shorts or opens among the metallization stack and active  region. However, as integrated circuit technology advances  towards more metallization layers and the introduction of new  low k inter-layer dielectric materials with lower thermal  conductivities, the sensitivity of these power alteration  techniques is compromised due to reduced laser coupling  efficiency. There is also a limit on the maximum laser power  that can be delivered to the device due to potential laser


induced damage. Thus, there is a need to enhance the  sensitivity of the existing detection systems to optimize fault  localization.


The use of a pulsed laser with a lock-in amplifier to enhance  detection sensitivity was first introduced in 2001 [6]. Detection sensitivity is enhanced by pulsing the laser at a  specific frequency where the noise level is low together with a  lock-in amplifier for signal processing. It has been shown that  an improvement in signal to noise ratio of up to 10 times can  be achieved at a pulsing frequency of 5 kHz [9]. However, the  implementation of the lock-in methodology is usually more  complex and high sensitivity is achieved after fine tuning  various lock-in amplifier parameters like time constant, lockin frequency and phase difference between the reference  frequency and pulsed laser induced signal for each scan speed. In this paper, we describe a new pulsed laser digital signal  integration algorithm which has achieved sensitivity  enhancement without the use of a lock-in amplifier.  This  method can be applied to both ac-coupled and dc-coupled  detection systems.


AC-Coupled and DC-Coupled Detection Systems


The experimental setups of OBIRCH, TIVA and TBIP-XIVA  are shown in Fig. 1a, 1b and 1c respectively. OBIRCH is a  voltage bias, current detection technique while TIVA is a  current bias, voltage detection technique. TBIP-XIVA uses an  inductor to emulate current ‘choke’ to achieve a voltage bias, voltage detection configuration. These techniques are usually  implemented together with a high gain and low noise  amplifier in ac-coupled mode to selectively amplify the small  laser induced signal coupling which is superimposed on the  high dc value corresponding to the electrical bias of the device  under test (DUT). Fig. 1d shows the setup of the voltage bias, voltage detection, dc-coupled detection system. It uses a  balanced bridge configuration to eliminate the dc offset  associated with the electrical bias.   As the resistance of the  DUT changes upon thermal stimulation, the voltage change


## Enhanced Detection Sensitivity with Pulsed Laser Digital Signal Integration Algorithm


234


across the DUT is then measured with respect to reference  arm of the bridge.


vo


VB


Current  Amplifier


ac-coupled


IB


(a) OBIRCH


(b) TIVA


Rs


dc-coupled


R1


R2


R3


DUT R4


(c) TBIP-XIVA


(d) DReM


Figure. 1: Schematic diagrams of ac-coupled & dc-coupled  laser induced detection systems.


The signal line scan profiles of ac-coupled and dc-coupled  detection systems are shown in Fig. 2a and 2b. The  comparison shows that the signals from ac-coupled systems  contain an artifact which is commonly observed as the “tail” due to the derivative nature of the coupling mode.  This  artifact does not exist in dc-coupled system which allows a  better localization of laser induced defects [8].


artifact


μN


μS


225 250 275 300 325


Pixel No.


200 50


N 320


280 300


240 260


220


50 100 150 200 250


(a) ac-coupled


(b) dc-coupled


Figure 2:  Horizontal line scan signal profiles of (a) accoupled detection systems taken from TIVA signal micrograph  and (b) dc-coupled detection systems from DReM signal  micrograph showing the signal mean (μS), noise mean (μN), and noise standard deviation( N).


The pulsed laser digital signal integration algorithm is  incorporated in SEMICAPS SOM 1100 Scanning Optical  Microscope which is equipped with a 1064 nm laser for  carrier stimulation and a 1340 nm laser for thermal  stimulation.


i. Pulsed laser induced signal response


Laser induced signal waveforms are obtained by exciting the  1340 nm laser in point mode on a point of the single metal line  shown in Fig. 3.


Figure 3: Frontside image of 15.3  single metal line  electromigration sample with TIVA signal overlaid in pseudo  colour.


Fig. 4 and Fig. 5 show the pulsed laser induced response of  ac-coupled and dc-coupled detection systems at different  pulsing frequencies for TIVA and DReM setups respectively. Each figure shows the laser induced response after  amplification during laser beam “ON” and beam “OFF”. The  amplifier bandpass filter is adjusted for maximum noise  rejection without filtering the signal response.


These waveforms clearly indicate that the laser induced signal  attenuates with increasing pulsing frequency. Due to the  thermal time constant of the DUT, a finite time is required for  the sample to respond to the temperature change. Accumulating the signal over the entire period is expected to  be larger than a single digitized value. Since the pulsed TIVA  signal decays upon reaching thermal equilibrium as shown in  Fig. 4a, the accumulated signal is expected to saturate at  pulsing frequencies below 100 Hz. However, the accumulated  signal for pulsed DReM continues to increase since the dccoupled response would still remain at a lower pulsing  frequency. The pulsed TIVA waveform indicates the single  metal line requires approximately 5 ms to reach steady state  due to the high thermal time constant. The ac-coupling mode  also means that a “tailing” response is generated whenever the  laser is turned off. At a higher pulsing frequency, it can also  be observed that the induced signal lags the beam transition by  6 μs. This is the sum of the time delay in the actual turning on  of the laser upon triggering by the beam on-off signal and the  time taken for the laser to penetrate the passivation layer  above the metal.


During pulsing, the duty cycle is set at 50%, i.e. beam on time  is equal to beam off time. The amplified signal is digitized at  20 MHz. In the new signal integration algorithm, the signal  intensity over each pulse period is obtained by summing the  digitized signals during laser on and subtracting the digitized  signals during laser off. The new algorithm digitally  accumulates the signal intensity over a single pulse.


0 1 2 3


-3


-2-1


Beam “ON”


Time (ms)


Beam “OFF”


(a) Pulsed TIVA response at 100 Hz


Time (μs)


(b) Pulsed TIVA response at 5 kHz


75


(c) Pulsed TIVA response at 20 kHz


Figure 4: Pulsed laser induced response of ac-coupled system  with TIVA setup at different pulsing frequencies.


ii. Signal-to-Noise comparison


A series of experiments are conducted using TIVA and DReM  with and without incorporating the signal integration  algorithm on a 15.3  metal line structure in Fig 3. A root  mean square (r.m.s.) noise of 2 mV is measured across the  DUT in the TIVA detection system while a r.m.s. noise of 1.7  mV is measured across the DUT in the DReM system.  An  image signal-to-noise ratio (SNR) algorithm is then used to  compare the sensitivity of the techniques conducted at the  same laser power, magnification, biasing condition and signal  amplification. The image SNR measurement is defined by


N S


SNR


where μs denotes the signal mean and n denotes the noise  standard deviation. The SNR results from Fig. 6 show that the  signal to noise ratio or the sensitivity varies with pulsing  frequency. The sensitivity peaks between 500 Hz and 1000 Hz    due to stronger  accumulated signal.  As the pulsing frequency


(a) Pulsed DReM response at 100 Hz


(b) Pulsed DReM response at 5 kHz


(c) Pulsed DReM response at 20 kHz


Figure 5: Pulsed laser induced response of dc-coupled system  with DReM setup at different pulsing frequencies.


drops below 500 Hz, the detection systems are strongly  affected by low frequency noise thus compromising the  overall detection sensitivity. At higher pulsing frequency, the  sensitivities of both techniques with signal integration are  similar. However, pulsed DReM is more sensitive than pulsed  TIVA at lower frequency as the dc-coupled integrated signal  continues to increase with decreasing pulsing frequency and  the high common mode rejection ratio of the dc-coupled  amplifier reduces the noise level in DReM system. The best  detection sensitivity incorporating the integration algorithm is  achieved at a pulsing frequency range between 500 Hz to 1.5  kHz for a scan time of less than 10 minutes on a 512 x 512  image resolution. This frequency range is smaller than pulsing  frequency of 5 kHz or 50 kHz used by de la Bardonnie M et  al for the lock-in methodology [9].


Table 1 shows a comparison of the sensitivity of TIVA and  DReM without pulsing and with pulsed signal integration at  the frequency of highest sensitivity. It shows that the  algorithm improves sensitivity by a gain factor of more than 9  times.


0 25 50 75 100 125 150


2500


Pulsing Frequency (Hz)


Pulsed TIVA with Signal Integration Pulsed DReM with Signal Integration


Figure 6: Sensitivity with digital signal integration applied to  TIVA and DReM at different pulsing frequencies.


Table 1: SNR comparison between different laser induced  detection systems.


136.1


14.7


109.8


7.9


TIVA


Pulsed TIVA with Signal  Integration at 1.28 kHz


Pulsed DReM with Signal


Integration at 500 Hz


DReM


Laser Induced Detection  Systems


No.


Case Studies


Several case studies on the application of the pulsed laser  signal integration algorithm on semiconductor devices are  described in this section.


i. Case study 1: metal line structure


The same metal line structure in Fig. 7a used for sensitivity  comparison is biased at 1 mA. The conventional DReM signal  image with the resistive structure localized is shown in Fig. 7b. Fig. 7c shows that the DReM signal is greatly reduced  when the current drawn is reduced by 10 times to 100 μA. Fig. 7d shows tremendous signal enhancement when the  signal integration algorithm is implemented at a pulsing  frequency of 1.28 kHz. Induced signals from the bond pads  and neighboring bond wires that are indirectly connected to  the structure are also detectable.


ii. Case study 2: NMOS sample


Fig. 8 shows another case study using an NMOS transistor test  structure to emulate a point defect.  Thermal stimulation on  the channel causes localized power alteration across the biased  source  and  drain  which  is  detected  with  DReM  using  a


Figure 7: (a) Frontside overlay image of 15.3  single metal  line sample (b) Typical DReM signal image at 1mA biasing  current. (c) Weaken DReM signal image at 100 μA biasing  current. (d) Signal image with pulsed laser signal integration  algorithm applied to DReM detection system at 1.28 kHz.


Figure 8: (a) Frontside overlay image of an NMOS transistor (W/L: 40μm/0.4μm) (b) Typical DReM signal image at 10  mW laser power. (c) Weaken DReM signal image at 1.8 mW  laser power (d) Signal image with pulsed laser signal  integration algorithm applied to DReM detection system at


1.28 kHz.


laser power of 10 mW shown in Fig. 8b. The DReM signal  weakens when the laser power is reduced by almost 10 times


to 1.8 mW as shown in Fig 8c. Accumulating the induced  signal at 1.28 kHz greatly enhances the detection sensitivity  and strengthens the signal shown in Fig. 8d.


iii. Case study 3: DRAM sample


The last case study is a DRAM sample which fails on static  standby leakage in the cell. Fig. 9 shows the localization  images using pulsed TIVA technique with signal integration at  5x and 100x magnification. The conventional TIVA technique  was unable to localize any signal at low magnification.  The 2  sense amplifier signals, indicated in Fig. 9b (ii), were  localized by TIVA after high sample averaging at a higher  magnification of 20x and beyond where the laser power  density is stronger. At lower magnification, the signal is so  weak that the noise overwhelms the signal. Using the  algorithm with pulsed laser at 2.15 kHz, the defective sites in  Fig. 9b (ii) can be localized from 2.5x to 100x magnification. The enhanced sensitivity provided by the algorithm localizes  the signal from the leaky site which has a reverse contrast  from the signal from the 2 sense amplifier signals. This true  failure site is not visible with the conventional TIVA  technique.


a (i)


a (ii)


sense  amplifier leaky site


b (i)


b (ii)


Figure 9: a(i) Frontside overlay image of a DRAM device and  a(ii) pulsed TIVA signal image with digital signal integration  at 5x magnification. b(i) Frontside overlay image of a DRAM  device and b(ii) pulsed TIVA signal image with digital signal  integration at 100x magnification.


A digital signal integration algorithm for pulsed laser  operation has been developed and implemented in the  scanning optical microscope for high sensitivity fault  localization. The algorithm is compatible with existing accoupled and dc-coupled detection systems. The best detection


sensitivity is achieved at a pulsing frequency range between  500 Hz to 1.5 kHz.  Within this frequency range, the  algorithm is capable of achieving more than 9 times  enhancement in detection sensitivity.


[1] Phang JCH, Chan DSH, Palaniappan M, Chin JM, Davis  B, Bruce M, Wilcox J, Gilfeather G, Chua CM, Koh LS, Ng HY, Tan SH, “A Review of Laser Induced  Techniques for Microelectronic Failure Analysis”, Proc  Int Symp Physical & Failure Analysis of Integrated  Circuits (IPFA 2004), 5-8 Jul 04, Hsinchu, Taiwan, pg  255-261, 2004


[2] Nikawa K, Inoue S , "New Laser Beam Heating Methods  Applicable to Fault Localization and Defect Detection in  VLSI Devices ", Proc Int Rel Phy Symp (IRPS 1996), pg  346-354, 1996


[3] Nikawa K, Inoue S, “Various Contrasts Identifiable from  the Backside of a Chip by 1.3 m Laser Beam Scanning  and Current Change Imaging”, Proc Int Symp Testing & Failure Analysis (ISTFA 1996), 18-22 Nov 96, Los  Angeles, California, USA, pg 387-392, 1996


[4] Cole EI, Tangyunyong P, Barton DL, “Backside  Localization of Open and Shorted IC Interconnections”,  Proc Int Rel Phys Symp (IRPS 1998), 31 Mar 98 – 2 Apr  98, Reno, Nevada, USA, pg 129-136, 1998


[5] Cole EI, Tangyunyong P, Benson DA, Barton DL, "TIVA  and SEI Developments for Enhanced Front and Backside  Interconnection Failure Analysis", Proc Eur Symp Rel  Electron Devices, Failure Physics & Analysis (ESREF  1999), 5-8 Oct 99, Bordeaux, France, pg 991-996, 1999


[6] Palaniappan M, Chin JM, Davis B, Bruce M, Wilcox J, Chua CM, Koh LS, Ng HY, Tan SH, Phang JCH, Gilfeather G, “New Signal Detection Methods for  Thermal Beam Induced Phenomenon”, Proc Int Symp  Testing & Failure Analysis (ISTFA 2001), 11-15 Nov 01, Santa Clara, California, USA, pg 171-177, 2001


[7] Falk RA, "Advanced LIVA-TIVA Techniques", Proc Int  Symp Testing & Failure Analysis (ISTFA 2001), 11-15  Nov 01, Santa Clara, California, USA, pg 59-65, 2001


[8] Quah ACT, Koh LS, Chua CM, Palaniappan M, Chin JM, Phang JCH, "DC-Coupled Laser Induced Detection  System for Fault Localization in Microelectronic Failure  Analysis", Proc Int Symp Physical & Failure Analysis of  Integrated Circuits (IPFA 2006), 3-7 Jul 06, Singapore, pg 327-332, 2006


[9] de la Bardonnie M, Ross R, Ly K, Lorut F, Lamy M, Wyon C, Kwakman LFTz, "The Effectiveness of  OBIRCH Based Fault Isolation for Sub-90nm CMOS  Technologies", Proc Int Symp Testing & Failure Analysis (ISTFA 2005), 6-10 Nov 05, San Jose, California, USA, pg 49-58, 2005


A Study of Flip-chip Open Solder Bump Failure Mechanism


Zhaofeng Wang, Sr. FA Engineer, Tel. (951) 375-4270,  zwang1@irf.com


Mahmood Choudhry, FA Lab Manager, Tel (951) 375-4286,  mchoudh1@irf.com Failure Analysis Lab, International Rectifier Corp.


41915 Business Park Dr. Temecula, CA92590


The present paper is a study on flip-chip open


bump failure mechanism. Initial electrical testing


showed open circuit condition. Scanning acoustic


microscope (C-SAM) identifies delmanination on


particular bump(s). Initial cross-sectional images


suggested that the separation took place at Al –


TiW interface. However, EDS analysis on the


separated surface indicated the presence of Al


metal at both sides of the separation, which raises


a question of why the Al layer is cracked or


separated instead of interface de-lamination.


Research in literature and investigation at


assembly line points an ultrasonic cleaning step in


manufacturing process as a contributor to the open


bump failure. Examining virgin dice after bump


removal observed crack in nitride passivation


around the bump neck, indicating high stress level


during passivation film deposition and/or bump


formation process. Hence it is concluded that


ultrasonic cleaning in device assembly aggravates


preexisting stress in weak bump(s), resulting in


latent failure in field application.


Flip chip packaging is well known for its


advantage in size, performance, flexibility,


reliability and cost over traditional packaging


method in microelectronic manufacturing.


The flip-chip device in discussion is part of an


integrated circuit in a module in voltage regulation


application. The bump is constructed of Al pad


metal - TiW adhesive layer - Cu stud - Pb/Sn


solder (Fig. 1). The bumps are mounted onto a


print circuit of ceramic substrate.


Fig. 1: Illustration of the solder bump


construction.


Electric test on a failed device diagnoses an  intermittent and/or open circuit on a flip-chip die.


1. Non-destruction Inspection


The flip chip die in a failed module is inspected  with scanning acoustic microscope (C-SAM) and  x-ray. C-SAM detects dis-bond bump (s) in the die  while x-ray indicates no absence solder at such  bump (s) (Fig. 3).


Fig. 2: C-SAM and x-ray image of the  same die having dis-bond bump.


2. Cross-sectional analysis


Cross-sections are made through bumps that are  detected by C-SAM as well as their adjacent  normal ones. It confirms that the dis-bond bumps  indicated by C-SAM are indeed delaminated at AlTiW interface (Fig. 3).


De-lamination


Good bump


solder


Al pad


Si Nitride


TiW


Cu plated stud


Fig. 3: cross-section of a good and open  bond.


SEM close examination and EDS analysis of the  open bump showed that the delamination is not a  clear cut separation at Al-TiW interface. Al is  present at both sides of the separated surface, i.e. the 0.8um Al metal layer appears to be torn at or  near TiW layer.


239


Fig. 3a: close-up of a delaminated bump  showing Al fracture at the edge of nitride


passivation ring.


2. Die Pull Examination


In order to examine the interface of the Al-TiW  separation, a die-pull apparatus is devised by  modifying a micrometer gauge to make shear-free  die pull possible (Fig. 4)


Fig. 4: A glass slide is mounted onto the


flip chip die for die-pull (left side). A die-pull


apparatus is devised from a micrometer gauge


(right side). Tensile force is applied to the die by  pulling the meter knob (red arrow).


2.1. Introduction of Fracture Pattern in Metals


When ductile materials failed of fracture, i.e. to


crack or split into two or more fragments by


means of or as a result of force or strain, two


phenomena can usually be observed:


(a) fracture origin


(b) plastic deformation pattern at the  separation interface.


Such pattern usually manifests the cyclic stress


that supplies the energy for the propagation of


fracture. The curvature of such lines usually


represents propagation rate defined by the


boundary conditions.


Careful study of the two surfaces that separated  the die from a bump in light of metallurgical  fracture mechanism observes convincing evidence  of Al plastic deformation under cyclic stress (Fig. 5).


These patterns help to trace the possible fracture  origin(s).


TiW  Cu


Al fracture line


The origin of fracture appears to be located at two  areas:


(a) near passivation ring crack


(found in majority of the failed  bumps)


(b) within Al pad (found in some


failed bumps)


Fig. 5: An open bump after die-pull separation.  Evidence of pre-existing defect/strain in Al is


observed, some at the fracture origin, some in


middle of the fracture propagation path (Fig. 5a,


5b).


Fig. 5a: what appears to be a fracture origin in Al


radiating with “river” marks (red arrows), and  evidence of fracture propagation lines around it (blue arrows).


Fig. 5b: evidence fracture propagation lines


disrupted by a point defect in Al (dashed arrows).


3. Cyclic Stress Source: Ultrasonic Cleaning


The evidence of Al fracture propagation and


observable pattern of cyclic stress (Fig. 4, 5) leads  to an investigation on the source of such stress.


Reviewing of the manufacturing process reveals  that there is an ultrasonic cleaning step in the


module assembly line. However, this ultrasonic


cleaning step is a standard procedure in the


module assembly line for many years, while this  open bump failure occurred only recently.  Further  investigation discloses a recent change in


ultrasonic machine model.


Research in literature suggests that the frequency  and power rating of a given ultrasonic machine


can have significant impact on the stress it departs  onto devices subject to cleaning. It is frequency


not the power ratings that plays more important


role in producing high impact.


Fig. 6: Cavitations strength vs. Ultrasound


Frequency (Courtesy: Branson Ultrasonic Corp)


Fig.7: Affect of ultrasound frequency/sound to the  proximity of the surface for particle removal


(Courtesy: Branson Ultrasonic Corp)


The new ultrasonic machine in the module


assembly line does have the combination of lower  frequency, which has higher impact on the bumps. Statistics shows that the recent serge in flip chip


failures is in the hundreds of ppm level. Moreover, among 12 bumps on a failed chip, there is usually  only one bump that actually fails. Hence the


ultrasonic fact alone does not seem to explain the  open bump failure, otherwise this ultrasonic


cleaning step could have caused catastrophic


failures. There is some thing that initiates or


originates upon which the high impact ultrasonic  cleaning aggravagates.


4. Finite Element Analysis (FEA) of Solder Bumps   In an independent investigation on the open bump  issue, one of the customers of this product


performs FEA on the flip chip die focusing on


thermal and mechanical stress of the bumps. Their  FEA result indicates that stress level varies from


bump to bump, the highest stress is at the TiWnitride around the bump neck. The FEA report


concludes that thermal stress at the chip


manufacturing process and at the module assembly  process can possibly cause bump crack.


5. Die Defect Investigation


Since the entire Al-TiW interface is isolated from  external access (Fig. 1) in the module assembly,


the possibility of chemical corrosion as a


contributor to the failure during module assembly  process is excluded.


Pre-existing weakness and/or defect in the bump  interface(s) is then highly suspected. As a matter  of fact, this is proposed as the probable root cause  at the beginning of this open bump investigation. Nevertheless, die pull test data in the flip chip


manufacturing records does not show high fall rate  during that period of time.


Virgin dice are acquired from the chip


manufacturer. The solder bumps and the TiW


layer are subsequently etched followed by optical  inspection. Cracks in passivation layer were found  around one bump neck on some dice (Fig. 8).


Fig. 8: Evidence of fracture in nitride passivation  around the bump neck is found on a virgin die. Result and Discussion:


1. Evidences obtained from C-SAM, x-ray, crosssection, die-pull test and fracture propagation  pattern observation, DOE of C-SAM cleaning at  assembly line, and virgin bump analysis  demonstrated the flip chip bump open failure  mechanism to be:


(a) Pre-existing high stress and/or weak spot  in the bump formed during flip chip  process, especially at Al-TiW interface  around the bump neck acts as fracture/delamination precursor.


(b) High impact ultrasonic cleaning (due to  the change of ultrasonic machine model) in module assembly line aggravates and  propagates fracture and/or de-lamination  at the Al-TiW interface.


A failure analysis process flow for flip chip bump  open contact failure has been developed, which  not only allows the in depth study of UBM delamination failure mechanism, but also initiates  and enables the coordination between chip  manufacturer, module assembly site and customer  for a thorough investigation on the failure, implement preventative measures to improve  product quality and reliability.


Photon Emission Microscopy (PEM) is a passive type of  analysis. Passive techniques measures the emissions from the  sample and do not alter the sample. The physical origin of the  light emissions from the pn junctions can be easily understood  by studying the recombination of holes and electron under  forward and reverse bias conditions.


Figure 10: PEM image after backside sample preparation.


Backside emission


The Automated Selected Area Polisher (ASAP-1, commercially available in the market) is designed to thin and  polish small selected areas in electronic packages and waferlevel dies. The resultant thinned component is transparent to  infrared light, thus enabling backside failure analysis to be  carried out on the circuitry.


The automated selected area polisher utilizes a high precision  rotating chuck that holds a variety of tools, in various sizes, and is speed controllable. An adjustment is incorporated to  center the motion at the correct point of the package or wafer  under preparation. This chuck is attached to a Z-Stage that  moves vertically on linear bearings and is controlled. The  correct polishing pressure is applied. An X-Y stage holds the  sample and is located underneath the rotating chuck. This  stage is motorized and runs independently in X and Y  directions at user-set amplitudes, to produce the desired  dimensional ‘window’.


Selected area polishing on the backside was developed to aid  the test, debug, and failure analysis engineering. (and  semiconductor devices. ) Figure 12 shows the cross sectional  view of the selected area polishing on the backside. ASAP  incorporates adjustment for setting sweep center, along with  intuitive X and Y amplitude controls. Using standard tool  diameters enhances process reproducibility. This means that  one straightforward setup of the X-Y parameters will be  sufficient for the whole process.


Figure 11: Schematic of the sample preparation procedure  for PEM backside analysis on a cavity down sample.


Controlling the pressure, the provision of a controllable  loading system means that the correct pressure for specific  tool, tool diameter and abrasive can be selected. For SOP  package device, use 1mm drill bit and adjust the Y  coordinate only in creating the window.


Knowing the package information is needed to be able to  process the samples accurately. Figure 13 shows the crosssectional view of a cavity down in an SOP package. Critical  information, such as the package and copper thickness are  the some of the most important key parameters for backside  sample preparation.


Figure 12: Scanning Electron Microscope (SEM) image of  the cross-sectioned SOP device.


Figure 13: SOP device after backside sample preparation.


Conclusion and Acknowledgements


We presented a new sample preparation approach on Small  Outline Package (SOP) in removing the encapsulant while  preserving the integrity of the die, bond pads, bond wires and  lead frame interconnects. A special milling technique which  eliminates the need for repackaging process on backside  sample preparation was also presented.


I thank my friends and colleagues from Texas Instruments (TI) for their encouragement to write this paper. Special thanks to  David Maxwell, Thao To and Olivia Pambid for their inputs  and sharing their Failure Analysis (FA) knowledge.


[1] Steve Brockett, “Biased Backside Failure Analysis  Techniques for Small Plastic Packages”, IEEE.


[2] ISTFA Microelectronic Failure Analysis Desk Reference  4th edition ISTFA conference, pp. 55.


[3] ASAP-1 milling tools literature, www.ultratecusa.com.


Die


Copper heat slug


Wire bond


The Electrical Characterization and Physical Failure Analysis   For Transistor Gate Leakage


Tsung-Te Li, Chao-Chi Wu, Jung-Hsiang Chuang, Jon C. Lee


Taiwan Semiconductor Manufacturing Company, Ltd.


6, Creation Rd.2, Science-Based Industrial Park, Hsin-Chu, Taiwan 300, R.O.C. Tel: 03-5785112ext.2175 Fax: 886-3-5787778


ttli@tsmc.com, ccwun@tsmc.com, jhchuang@tsmc.com, clee@tsmc.com


Continuing advancements in semiconductor technology  have meant device scaling to nanometer feature sizes and  steadily increasing transistor densities. Killer yield defects in  these nanometer sized devices can be submicron in size and  frequently invisible


The emergence of advanced failure analysis has enabled  the detection of these invisible defects more recently [1-2].


In this article, the electrical and physical analysis of gate  leakage in nanometer transistors using C-AFM (conducting  atomic force microscopy), nano-probing, TEM (transmission  electron microscopy), and chemical decoration on simulated  overstressed devices is described.


A failure analysis case study involving a soft single bit  failure is first detailed. A suspected transistor with gate to  source/drain leakage was isolated first with C-AFM, a method  widely used for failure analysis of advanced semiconductor  products. Nano-probing was employed to measure the  electrical behavior of this individual device for further  analysis. The Id-Vg behavior of this suspect transistor differed  significantly as compared to a reference, non-failing device.  Exchanging the nodes of the source and drain while  sweeping the voltage, the Id-Vg behavior of the suspect  device was found to be similar to the reference device. However, an anomalous source to drain gate leakage in the  suspect device was measured from the current components of  the Ioff I-V plot. The asymmetry noted in the I-V behavior of  the suspect device indicated that gate leakage was only present  on one node of the source/drain region.


To confirm the hypothesis of source to drain leakage, the nano-probing results were compared to the simulation data  for a source to drain leakage on this device. When this  comparison was made, the nano-probing results matched the  simulated Id-Vg behavior for a S/D gate leakage.


Following this nano-probing analysis, TEM cross  sectioning of this failing device was performed. A local gate  oxide anomaly was observed. Based on this analysis, another  approach to further highlight the leakage point was  implemented. A voltage bias was applied to exaggerate the  gate leakage site.


Following this deliberate voltage overstress, a solution of  boiling 10%wt KOH was used to etch decorate the gate  leakage site followed by SEM inspection.


For C-AFM and nano-probing measurement, DI  Dimension 3100 and Hitachi N-6000 were used respectively  in this case study. Failure analysis was performed on the  SRAM soft single bit failure followed by C-AFM analysis as  shown as Figure 1(a) and 1(b).


C-AFM current mapping shown in Figure 1(a) disclosed  an anomalous signal in the SRAM contacts.  Comparing the  layout of the SRAM cell in Figure 1(a) with the C-AFM I-V  measurements shown in Figure 1(b), it was suspected that a  leakage existed between contact 2 and contact 1. The S/D gate  leakage was present in one node only, indicated by the T1  transistor shown in Figure 2.


T1 transistor


Fig. 1(a): The C-AFM current mapping and layout of SRAM  cell. The abnormal contacts can be found from C-AFM  current mapping.


Fig. 1(b): The I-V curves measured by C-AFM. S/D gate  leakage between Contact 1 and Contact 2 was suspected.


Po ly


Contact 3  Po ly


Contact 1


T2 transistor


Contact 2


Contact 4


Poly


Contact 3


Poly Contact 1


ntact 2


Contact


Bias=-1V


Bias=1V


C-AFM I-V CURVE


-3.E+03-2.E+03


0.E+00


2.E+03


3.E+03


V o l t a g e


Contact 1 Contact 2 Contact 3 Contact 4


## The Electrical Characterization and Physical Failure Analysis For Transistor Gate Leakage


257


Figure 2: (a) The T1 transistor with one node S/D leakage  was suspected from C-AFM data. The schematic is simplified  as shown in (b).


For further analysis, nano-probing was used to measure  the electrical behavior of the T1 transistor. When the leaky  node was set as drain, the Id-Vg behavior of the T1 transistor  was significantly different from that of the reference transistor  T2 (Figure 3). Exchanging the nodes of source and drain, the  Id-Vg behavior was similar between T1 and T2 transistors (Figure 4). Furthermore, S/D gate leakage in the T1 transistor  was observed from the Ioff current components (Figure 5). The asymmetry I-V behavior meant that the S/D gate leak  only happened on one node.


Figure 3: (a) The Source, Drain (leaky side) and Gate of T1  transistor were illustrated for the nano-probing measurement.


(b) The Id-Vg curves of abnormal transistor T1 and reference  transistor T2 are shown.


Figure 4: (a) Exchanging the S/D nodes, the Source (leaky  side), Drain and Gate of T1 transistor are illustrated for the  nano-probing measurement. (b) The Id-Vg curves of abnormal  transistor T1 and reference transistor T2 are similar.


Figure 5: (a) the current components IG, IS/D-1, IS/D-2 and IB of  T1 transistor are illustrated for the nano-probing  measurement. (b) The Ioff current components of T1 transistor  show S/D gate leakage.


To further confirm the nano-probing result and verify the  hypothesis of gate oxide leakage, a simulation of a S/D gate  leakage was performed. The Id-Vg simulation behavior  closely matched the nano-probing result shown in Figure 6.


Figure 6: (a) the schematic of the simulation condition.  (b) The simulation result shows the Id-Vg behavior nearly  matching the nano-probing data.


A local gate oxide anomaly (thinning) observed from the  cross sectional TEM images was believed responsible for the  S/D gate leakage in transistor T1 (shown in Figure 7). Since  the gate leakage site was small, a further approach to  exaggerate the gate leakage site was pursued.  A voltage bias  over-stress was applied between the leaky gate and S/D node. Next, the voltage over-stressed sample was polished to  polysilicide. Following this step, the sample was etched  decorated in boiling 10%wt KOH solution and then SEM  inspected.


A voltage over-stressed site was clearly visible at the  poly edge (Figure 8). An anomaly in the gate oxide was  highlighted which confirmed the suspected gate leakage in  only one node of the S/D of the T1 transistor.


Drain


The leaky S/D


G


Source  Drain


The


Leaky S/D  G


T1  T1


-3.0E-06-2.0E-06-1.0E-06


0.0E+00


1.0E-06


2.0E-06


3.0E-06


0.8


VS/D-1(V)


1.2


IS/D-1


IG


IS/D-2 andIB


N+


IS/D-1 The leaky S/D


IS/D-2


IB IG


Figure 7: Tiny gate oxide anomaly (indicated by the arrow) was identified in the TEM image of the gate leakage-site of  transistor T1.


Figure 8: The overstressed site was highlighted following  etching in boiling 10%wt KOH solution.


As device features scale down to nanometer range, nonvisible defects such as gate leakage defects will become more  frequently a source of failure. C-AFM and nano-probing will  be key tools for the fault isolation and electrical measurements  in these types of transistor failures


Different transistor leakage behaviors can be identified  with nano-probing measurements and then compared with  simulation data for increased confidence in the failure analysis  result. Furthermore, nano-probing can be used to apply  voltage stress on a transistor or a leakage path to worsen the  weak point and then observe the leakage site easier.


[1]. Jon C. Lee and J. H. Chuang, “Fault localization in  contact level by using conductive atomic force  microscope”, Proceeding of the 29th International  Symposium for Testing and Failure Analysis 2003.


[2]. C. C. Wu, Jon C. Lee, J. H. Chuang, and T. T. Li “ Single Device Characterization by Nano-probing to  Identify Failure Root Cause”, Proceeding of the 31st  International Symposium for Testing and Failure  Analysis 2005.


[3]. C. Smith and K. Symond, “Novel Deprocessing  Techniques to Analysis Gate Level Defects”, ISTFA 95  Proceedings, pp. 275~278 (1995).


Failure Analysis of Laser Blown Metal Fuse Failures  in Submicron Technology by C-AFM


Liang-Feng Wen, Chien-Hui Chen, Allen Timothy Chang


Taiwan Semiconductor manufacturing Company, Ltd.


No. 25 Li-Hsin Rd., Hsinchu Science Park Hsinchu, Taiwan, R.O.C.


This paper presents a method of using a Conductive Atomic  Force Microscope (C-AFM) to characterize a submicron metal  fuse that has been blown open inadequately by laser.  In order  to obtain a proper I-V curve measured using the C-AFM  without affecting the incompletely opened fuse, we propose a  method of preserving the fuse by coating its surface with spinon glass (SOG). This allows the entire fuse to be uniformly  exposed during dry etching, and enables accurate electrical  measurements to be made. By combining the data from the I-V  measurement as well as the data generated by the fuse sensing  circuitry, the difference in resistance between a fully opened  and partially opened fuse can be easily distinguished.


In circuitry with a high number of metallization layers, metal  fuses are easier to blow open by laser than deeply buried  polysilicon based fuses.  However, Bernstein, et. al., and Arndt  et. al,. have outlined problems with successfully blowing a  metal fuse, resulting in a damaged fuse that remains  conductive [1][2][3]. For this situation, we have developed a  technique to easily identify and characterize such problematic  fuses. Our work focused on the failing specimens from two  laser cutting machines, each set for a spot size of 3.1 µm at an  energy of 0.9µJ. Each group of samples was produced on  separate halves of a single 12 inch wafer. Specimens produced  by one laser were called Model A and specimens produced by  the other laser were called Model B.  The fuse bank stored  information such as wafer ID, die location (x,y), security keys, and other forms of identification. Model A specimens had a  5% higher failure rate than Model B after blowing their  respective fuses. In order to investigate the failure mechanisms  of Model A, several failure analysis experiments were  conducted on those failing dice. After deprocessing successive  layers of each die down to the substrate, we used an SEM to  inspect for abnormalities. During these inspections we found  no unusual phenomena. The passive voltage contrast (PVC) images from the metal fuse connections to the fuse sensing  circuit were found to be normal. That meant that the fuse  sensing circuit’s functionality was not affected by the laser cut. Therefore we decided to perform electrical measurements in  order to detect the difference between a poorly blown fuse and  a properly blown fuse.  First, a new delayering method to  avoid damaging the failure site while making the site suitable


for C-AFM measurements was developed. This method is  shown in Figure 1.


Figure 1: (a) The original fuse scheme, and (b) the structure  with an SOG film added to protect the poorly blown fuse from  being prematurely affected by dry etching.


Spin on glass (SOG) is a mixture of SiO2 and dopants in liquid  form. It was spin coated onto the wafer to fill the narrow  cavities created by the laser. Then the coated sample was put  into the oven for bake curing. These steps prevented later dry  etching processes from damaging the fuse while surrounding  dielectric layers were removed to allow SEM PVC inspection  and C-AFM measurement.  This is shown in Figure 2. Using


## Failure Analysis of Laser Blown Metal Fuse Failures in Submicron Technology by C- AFM


260


different PVC contrasts, we could verify if the blown fuse had  any sidewall residue.


Figure 2: Different PVC contrast images of SOG protected, dry etched metal fuses.  The top image was acquired with low  VC contrast and the bottom image was acquired with high  contrast.  Since it was SOG protected, the failure site could  resist the ion bombardment of dry etching. This method  allowed reliable C-AFM I-V curve measurements of the fuses.


Figure 3 shows the general schematic of the fuse sensing  circuit, with the fuse connections illustrated.


Figures 4 and 5 show different types of C-AFM electrical  measurements that were made on the fuse sensing circuit. A  blown fuse was defined as an open circuit between nodes A  and B and an unblown fuse was defined as a short between A  and B. For a blown fuse, the I-V curves for node A with  respect to ground showed the PMOS behavior and the curves  for node B with respect to ground showed both PMOS and  NMOS behaviors. It was observed that the I-V curve of node  A with respect to ground for a poorly blown fuse had the same  type of curve as the I-V curve of node A with respect to node  B for an unblown fuse.


To get more detailed analysis we overlapped all the measured  curves. The poorly blown fuse had some molten metal residues  so the fuse was still connected, as seen in Figure 6. With the  TEM and EDX analyses shown in Figure 7, the information


provided about laser penetration depth and the presence of  residues could explain the failure mechanism of Model A.


Figure 3: Schematic of fuse sensing circuit with unblown (a) and blown (b) metal fuses.


The authors would like to express sincere  appreciation to Ms. Alana Nakata for her  insightful input and advice. The authors are also  thankful to the management at IR Temecula  Center of Quality Excellence and IR Swansea  management for their support in this investigation.


[1] G.A.Riley, “Picking your Flip Chip: a  Comparison of Flipchip Methods and benefits” FlipChips.Com, pp1-6


[2] Y.Tsukada, H.Nishimura. “Fatigue Life  Analysis of Solder Joints in Flip Chip Bonding”, Journal of Electronic Packing, Sept. 2000 Vol122, Issue3 , pp207-213


[3] F.Zhang, M.Li, B.Balakrisnan, “Failure  mechanism of Lead-Free Solder Joints in Flip  Chip Packages”, J. of Electronic Material, Vol31, No.11, 2002, pp1256-1259.


[4] S.Brandenberg, S.Yeh “Electromigration  Studies of Flip Chip Bump Solder Joints ”, Delphi  Delco Electronics System PP1-8.


[5] J. Harman & E.W.Lamm, “The Impact of  Ultrasonic Frequency on Particle Removal”, Branson Ultrasonic Corp.


Non-Destructive Method for Detecting Solder Defects at the Second Level Interconnect  using 3D x-ray tomography (uCT)


Frank Toth, and Gary F. Shade; Intel Corporation, Hillsboro, OR, USA  5200 NE Elam Young Parkway


Hillsboro, Oregon 97124


{francis.toth.jr@intel.com, (503)-696-1546}


{gary.shade@intel.com, (503)-696-5937}


Optical and  electron microscopy allows  visualization and imaging in two dimensions of a  specimen’s surface without any conclusion being  possible of a samples’  three dimensional structure  or properties. A conventional X-ray radiography  system produces two-dimensional shadow images  of complete internal three-dimensional structures, but in a single two-dimensional shadow projection  the depth information is completely mixed[1,3]. An  X-ray tomography system, however allows  visualization and measurement of a threedimensional object’s structures without prior  sample preparation or destruction of the sample. In  case of solder joints at the second level interconnect  the solder joint shape and thickness is of the main  interest. Today’s printed circuit assemblies  comprise of several layers with components  populated on both sides of the PCBs[4]. This  presents challenges to conventional 2D nondestructive Xray techniques due to shadowing and  absorbtion of the x-ray energy. Tilting of the  samples while imaging helps to get around this  problem, however often it might not always be  adequate. In that case full 3D X-ray imaging is  needed to resolve the failure signature at the solder  joint location[5].


Several BGA components suspected of having a  non-wet solder failure mode condition were  considered for non-destructive 3D x-ray analysis. The two types  of components  evaluated were (0.8mm and 0.5mm pitch) BGA type #1 and type #2  arrays respectively. All samples were imaged using  3D- uCT Xray tomography methods. Inspection of  the components after reconstruction of images  revealed several solder joints exhibiting the non-wet


“snowman” or head-pillow failure mode as shown  in the cross section below[2]:


Figure 1.0 – shows cross section image of typical mode “H” failure signature.


3D X-ray imaging procedure


Figure 1.1 – shows data acquisition of x-ray shadow


images as sample  rotates through 180 degrees [1].


Figure 1.2 – software reconstruction step from the X-ray  projection image data [1].


## Non-Destructive Method for Detecting Solder Defects at the Second Level Interconnect using 3D x-ray tomography (uCT)


243


Figure 1.3. – shows summary of steps to obtain virtual


cross section image [1].


Figure 1.4 – showing BGA type #1 17X17 ball grid array. Solder joints in blue were identified as mode”H”.


Figure 1.5 – showing BGA type #2 14X14 ball grid array. Solder joints in blue were identified as mode”H”.


Figure 1.5- representative image of a virtual cross section  slice of BGA type #1 component at ball location B17.


Mode”H” failure signature shown by arrow.


Figure 1.6- representative image of an inverted grey scale  virtual cross section slice of BGA type #2 component at  ball location C1.. Mode “H” failure signature shown by  arrow.


A total of 6,084 solder joints were imaged nondestructively using this method followed by


destructive analysis (dye  stain and package pull) to  confirm the non-wet detection accuracy of the nondestructive X-ray technique. Dye stain and package  pull and X-ray data showed 100% correlation.


Figure 1.7 – dye stain and package pull (destructive


analysis) showing the solder joints at locations B17 and  C17. The depression on the solder joints show the mode “H” failure mode as depicted by the arrows.


Virtual cross sections obtained using 3D x-ray


tomography methods showed that it is possible to


evaluate non-destructively the solder joint  failure  mode “H” known as “head-pillow or snowman”  at  the second level interconnect. Virtual cross section  images revealed the non-wet  interface where the


solder joints did not coalesce. The solder joints


identified as non-wet were further  evaluated


destructively to verify that indeed the solder joints  exhibits the mode”H” failure mode. A total of 6084  solder joints of 0.8mm and 0.5mm pitch BGAs were  analyzed non-destructively using 3D-Xray


tomography. Correlation between dye stain and


package pull analysis and 3D- uCT X-ray  revealed  a 100% correlation. Major benefits of the 3D x-ray  technique is high confidence in detection for this


failure mode, reduced time to data, and reduced cost  associated with failure analysis.


PCB-side


Solder joint location B17


BGA –component side


Solder joint location C1


1. Skyscan NV- Aartselaar- Belgium –


Principles and Applications of micro-CT –


presentation.


2. Paul Mazurkiewicz -Advanced Analytical


Chemistry Techniques Enable Rapid, Cheap


and Concise Electronic Failure AnalysisProceeding form the 30th Symposium for


Testing and Failure Analysis (ISTFA –


2004).


3. Steve Wang, X-radia Inc- X-ray


Microtomography Tools for Advanced IC


Packaging Failure Analysis – EDFAS Desk


Reference 5th Edition.


4. Geepak Goyal, et al – Assembly Analytical


Forum Analytical Tool Roadmap ISTFA


2003 Rev 0 – White Paper.


5. Holger Roth, 3D or 2D- Choosing with


Today’s Technology - article SMT


Magazine, May 2001.


Deformation Study of Low K Dielectric after E-beam Exposure


Xianfeng Chen, Qiang Gao, Ming Li, Chorng Niou, W.T. Kary Chien


In this paper, the deformation mechanism of low K dielectric  film under electron beams (E-beams) is discussed, and the  effect of film deformation on the development of a low K  dielectric film etching recipe is investigated. To provide  meaningful data for process development, numerical analysis  was used in the failure analysis procedure. A correction factor  is formulated to calculate the change in thickness of the low K  dielectric film after E-beam exposure. In addition, scanning  electron microscope (SEM) settings for imaging low K  dielectric films are optimized to minimize deformation.


For the development of 90nm CMOS technology, an  interconnect structure composed of Cu metallization with low  K dielectric had replaced the previous Al / SiO2 interconnect  technology.


Many low K materials are currently available including  Teflon, Parylene and air. However, SiO2 is still considered as  the preferred dielectric in the semiconductor industry because  of its manufacturability, low cost, and reliability. To reduce  dielectric constant of a SiO2 based insulator, several  techniques can be used. One technique is to decrease the  polarizability by replacing O with CH3; while another is to  decrease the number of chemical bonds per unit volume by  introducing porosity or alternately by eliminating high K  impurities. Since the 1900s, the chemical industry had  engaged in developing such materials. Many scientists and  engineers in the semiconductor industry have investigated the  characteristics, manufacturing, and application of low K  dielectric. They focused mainly on: 1) the advantages of Cu / low K dielectric interconnects; 2) spin-on deposition and  chemical vapor deposition (CVD) technologies for low K  films; 3) new methods of chemical mechanical polishing (CMP) and etching of low K dielectric films; and 4) thermal  stability, adhesion, and reliability of low K dielectric films. In  this paper, our focus is on the new challenges encountered  during microstructure analysis and failure analysis of low K  dielectric films.


This work was based on AMAT low K dielectrics including  BD (Black Diamond) and NDC (Nitrogen Doped Carbide), which are deposited in PECVD (plasma enhanced chemical  vapor


deposition)


chambers.


NDC


uses


octamethylcyclotetrasiloxane C3H10Si as its precursor and BD  uses Trimethylsilane [(C-H3) 2-Si-O] 4 as its precursor.


Analytical tools included a Hitachi SEM-5200 scanning  electron microscope system for construction analysis and a  Hitachi E-1030 ion sputter tool for sample coating. Samples  were prepared both by mechanical cuts and by focused ion  beam (FIB) cuts using an FEI Dual Beam 835 system. Delineation stains were done with dilute 4.9% HF about 30  seconds. Transmission electron microscope (TEM) images  were obtained using an FEI Tecnai F20 system.


Figure 1.  SEM image of the metal 1 and IMD 2 layers


The test structure was based on a 90nm CMOS technology  Inter Metal Dielectric 2 (IMD2) layer after the via etching and  metal trench etching steps. No metal bone is present in the BD  structure. Figure 1 shows a cross sectional image of the layer  stack. The defined NDC film thickness is 500A and the BD  film thickness is 5860A. The metal 1 layer was deposited with  copper encircled with a TaN / Ta barrier layer.


Physical deformation of low K dielectric films can be  observed after E-beam irradiation. This deformation takes  forms such as dishing (Figure 2), cracking, delaminating (Figure 3), and bowing due to shrinkage (Figure 4). Under  these conditions, un-correct film thickness measurements  would be obtained, so critical dimension (CD) measurements  would be difficult to monitor accurately.


Figure 5 shows a TEM image of a via etching profile. The  image shows that the copper at the bottom of the via was  damaged because the NDC was over etched. Surely the  damaged copper will impact barrier deposition performance at  points A and B, which could result in an IC reliability issue. Therefore, we need a CD correction factor to optimize the


## Deformation Study of Low K Dielectric after E-beam Exposure


246


Figure 2.  SEM image of BD film with dishing


Figure 3  SEM image of IMD 2 dual damascene trench with  cracking and delamination between the BD and NDC films


IMD etching recipe during process development. So to obtain  accurate measurements of the via profile, it is important to  minimize the E-beam damage when taking SEM and TEM  images. In many ways BD and NDC behave just like  polymers, which are susceptible to E-beam induced damage  because they also charge easily under E-beam exposure.


The majority of the incident E-beam energy will be lost by  conversion into heat within the E-beam interaction volume.  This heat induces sample deformation. Also, when a CH3  chemistry is introduced into a SiO2 based dielectric such as  BD and NDC, it interrupts the Si-O bonds and creates  nanopores. These pores are removed by high energy E-beam  curing. These two mechanisms are the root causes of  deformations such as dishing and shrinkage. The degree of  deformation is proportional to the E-beam energy. Based on  this model, it can be easily understood that the film stresses  induced by E-beam curing will cause the cracking and  delamination shown in Fig. 3. Fig. 4 shows an FIB image of  bowing deformation in a via trench which could be caused by  E-beam or ion beam irradiation. So, optimization of the SEM  operating conditions is one of the most effective ways to avoid  E-beam induced damage. Since exposure to high-energy Ebeams causes the most severe damage to low K films, we can


decrease Vacc (accelerating voltage), exposure time, probing  current, and beam spot size to minimize the damage.  In  addition, we can also tilt the sample in the SEM chamber to  reduce E-beam interaction volume and avoid sample  deformation. Based on these findings, it can be concluded that  the via corners should suffer more damage than that of the  other areas because via corners have larger E-beam interaction  volume. However, damage caused by E-beam exposure can’t  be eliminated completely by optimizing SEM operating  parameters. So the true thickness of the low K dielectric film  can’t be directly measured with an E-beam or ion beam  microscopy system.


Dishing


Bowing


Cracking


Figure 4.  FIB image of a low K film via trench with bowing


Figure 5.  FIB image of a low K film via trench


Knowing the correct film thickness is a key factor in the  development of low K dielectric via etching processes. So if  no other measurement system is available, numerical analysis  is the best method to determine the original low K film  thickness when thickness measurements are performed after  E-beam exposure.


If only thickness (Y direction) shrinkage is considered, its  value can be best fitted with the Lagrange function:


( ) ( )


L X


B X F X


= ∑


Where LN (X) is the deviation between the true value and the  measured value at position X. In this case, this deviation is the  thickness shrinkage.  B I (X) is the interpolation coefficient,


)(


) (


( )(


X X X X


X X


B X


− −


=− −


F(XI)= XT-Xi


Where XT is the true BD or NDC film thickness and Xi is the  measured BD or NDC film thickness.


For example:


The data shown in Table 1 are the computed true values XT  and measured values Xi of the BD structure shown in Fig. 1. In this case, the low K dielectric film BD was imaged with the  SEM-5200, and the SEM imaging parameters are Vacc=1KV, Ie=10uA and Condense Lens 2 =5.0. We compared all of the  XT values with the thickness values measured by ellipsometry, which does no damage to low K dielectric films. We  concluded that the film thickness loss was approximately 2% compared to the parameters measured using the SEM. Also, the true thickness of the sample measured using the SEM  could be determined from XT= Xi + LN (X).


In another case, a low K dielectric film thickness is 6100A  measured by ellipsometry. With SEM parameters Vacc=5KV, Ie=10uA and Condense Lens=5.0, the measured Xi values for  this film were 5500A, 5480A and 5560A respectively on three  different sites with three E-beam scans.  The average  thickness loss was 9%.


From these two cases, it is reasonable to assume that the  higher the E-beam energy is, the greater deformation of low K  dielectric film would occur with E-beam exposure. During  failure analysis, the first priority is no sample damage. SEM  imaging with lower Vacc limits image resolution. Accordingly, lowering the condense lens setting can also  decrease low K dielectric film deformation due to E-beam  exposure. So whatever can lower E-beam energy can also  decrease low K dielectric deformation.


Table .1 Experimental data for computation of BD film  thickness


4500 5000 5500 6000


1 2 3 4 5 6 7 8 9 10


Xt Xi


If low K dielectric film deforms in the X direction and Y  direction at the same rate during E-beam exposure, the via


bottom and top CD could also be approximately calculated  using the method shown above.


Optimization of SEM operating parameters such as lowering  Vacc, probe current, and exposure time can minimize E-beam  and ion beam induced damage on low K dielectric films. With  numerical analysis using the Lagrange interpolation function, the deformation of low K dielectric films resulting from Ebeam exposure can be approximately calculated.


We would like to thank Ms. Bei Duohui of SMIC LTD group  for supporting our low K dielectric film deposition  experiments.


[1] Alex A. Volinsky, Joseph B. Vella, William W. Gerberich, Fracture Toughness, Adhesion and  Mechanical Properties of Low-K Dielectric Thin Film  Measured by Nano-indentation, Proc.. Thin Solid Films  429(2003), pp. 201-210


[2] S. S. Hwang, H. C. Lee, H. W. Ro, etc, Porosity Content  Dependence of TDDB Lifetime and Flat Band Voltage  Shift by Cu Diffusion in Porous Spin on Low K, San  Jose, CA, IRPS 2005, pp. 474-477.


[3] Gunnar Zimmermann, Copper / Low K Process  Characterization for 90nm Technology using SEM and  TEM Imaging, 12th International Syposium on Physical  and Failure Analysis of IC, Singapore, (2005) pp. 171-175.


[4] J. H. Butler, D.C. Joy, et al, Low Voltage Scanning  Microscopy of Polymers, Polymers Vol.36  No.9 (1995) pp. 1781-1790.


[5] Sergey Korenev, Jerry Kriebel, The Surface  Modification of Dielectric by a CW Electron Beam, Vacuum, vol. 62 (2001) pp. 237-240.


Realization of an Integrated IT System Covering the Complete  Failure Analysis Process


Markus Grützner


Infineon Technologies AG, Munich, Germany  markus.gruetzner@infineon.com


In the failure analysis process a large amount and variety of  data are involved: product information, images created by lab  equipment, requester and accounting information etc. An FA  lab usually makes use of software tools to handle all this data, to process analysis jobs, publish the results and to store data  for future reference and documentation. Instead of using  separate tools for image handling, sample tracking, report  creation and email, you can improve the workflows by  integrating all these functions in one single IT system. Especially in larger companies with numerous failure analysis  labs in different locations, connecting these labs brings  forward synergies by better and faster information exchange  and re-use of knowledge. This paper describes the process and  result of developing a dedicated FA software tool.


System Specification


Initial Scenario at Project Start


There were 11 analysis labs worldwide with a variety of  different workflows. Some of them worked for manufacturing  sites (wafer fabs and assembly), some for product design  support or customer complaints. Each lab had its own diverse  IT tools and was not connected to other labs. The fact that in  most cases the IT department did not provide support caused  extra maintenance effort for the FA staff. Since many of these  tools relied on outdated software platforms and had a long list  of change requests, a project was started to develop a unified  system for all sites.


Definition of Requirements


After project launch, an international team with representatives  from all labs and from the IT department was founded. To  prepare the system specification, requirements were collected  from all involved user groups: analysts, lab managers, internal  FA customers and IT specialists. One of the first steps was the  creation of flow diagrams of typical FA workflows to identify  the common processes and the local differences. To design a  suitable database structure, all necessary database fields were  collected from the participating labs and converted into a  common data model.


A subset of the global team, the “core team”, was established  to consolidate the collected information. To avoid


misunderstanding and to give the future users an idea of the  look and feel of the new software, a simple prototype of the  graphical user interface (GUI) was created. The final system  specification was signed off by all labs.


Due to the rather complex scope of this project, the team had  to cope with some difficulties. Since all labs had different  working processes and histories, a lot of effort had to be spent  for configurability while keeping the concept of having only  one single software version. Other problems were related to  the diverse wording used by the team members. For example, depending if you talk to an analyst from a wafer fab or from an  assembly site lab, you will get two completely different  definitions of what a “product” is and which attributes you  need to describe it. Further challenges were caused by the  nonuniform organization structure of the different labs – and  occasional re-organizations that changed the labs’ focus.


Make or Buy?


Based on the requirement specification, the team made a  market research for available LIMS software tools (Laboratory  Information Management System) [1] to be able to come to a “Make or Buy” decision. All evaluated tools would have  required major modifications to cover all requirements and to  be integrated smoothly into the company’s IT landscape. Especially interfacing with other corporate IT systems seemed  to be problematic with those commercial products, so the  project team went for a self-developed proprietary solution. The implementation was done by an external software vendor, supervised by the corporate IT department and the core team.


Main Features


The individual failure analysis labs differ in many aspects: organization (some labs report to quality management, others  to manufacturing or reliability departments), products (memory, logic, discretes, modules), function (EFA, PFA) and  motive (qualification, field returns, yield) [2]. Due to this  diversity, the project team had collected a large amount of  requirements. The list of features includes:


• identical software for all labs, but flexible design that  allows adaptation to all local business processes


• minimization of manual data entry by interfaces to other  databases


• automatic generation of report documents


## Realization of an Integrated IT System Covering the Complete Failure Analysis Process


249


• worldwide search of FA reports across all labs


• flexible and future-proof product data model


• failure classification catalogs


• look and feel similar to standard office software


• extensive management functions like workload  monitoring, cost accounting and cycle time calculation


• online job submission via web (intranet)


Some of the most important features are described in the  following section.


Analysis Types


Different workflows require different data. For certain jobs  you need dedicated tables and database fields to enter the  analysis results. But for other jobs these fields would not make  any sense and would rather confuse the users. Therefore  different types of analysis jobs were implemented to cover  these workflows. To illustrate the application of these diverse  job types, two examples are described in the following  paragraphs.


A typical workflow for wafer fab process monitoring might  look like this: cross section / chemical preparation / SEM  inspection & parameter measurement / comparison to target  values. Special catalogs provide the target values for a certain  wafer technology. After the analyst has entered the measured  parameters, the application creates a report containing an  overview table of data from all samples with automatic  highlighting of out-of-spec values.


A customer return might involve tester setup / failure  verification / package decapsulation / emission microscopy / microprobing etc. For this kind of jobs special catalogs have  been created to describe and classify the electrical and  physical failure for each sample.


Configurable Job Lists


Because the individual lab’s focus differs from other labs, users are interested in different job attributes. E.g. for an  analyst in a wafer fab lab, the field “package type” is surely  irrelevant. Therefore every user can configure his own  individual selection of attributes that are displayed in the job  lists (Fig. 1).


Figure 1: Customizable job lists


Image Handling


Images generated by the lab equipment, e.g. microscopes, can  automatically be imported to the system and assigned to a  specific job and sample. The image import works  independently from the lab machine’s operating system, no  matter if it is DOS, Windows or UNIX. This allows  connecting the system with older tools as well as with new  ones. After the images have been transferred, they can be  labeled, edited and selected for publishing using a built-in  image browser (Fig. 2 & 3).


Figure 2: Thumbnail preview and image details


Figure 3: Image selector


Classification of Failures


For a standardized classification of the analysis results, several  catalogs were implemented for electrical and physical failure  descriptions. This improves the searchability of analysis results  and the reuse of information.


Team Work


Multiple analysts can jointly work on an analysis job. It is  possible to assign tasks to individual persons or even groups of  analysts. Their individual tasks are stored for documentation of  the analysis process and to calculate the complete working  time (and costs) for each job (Fig. 4).


Figure 4: Tasks of an analysis job


Flexible Product Data Model


Analyzed products can be wafers, packaged devices, modules  etc. (Fig. 5). It is difficult to describe them with a fixed static  list of attributes. Therefore a flexible structure was developed, allowing products that contain multiple subcomponents. Fig. 6  shows an example of a multi-chip device. Each component  type comes with a suitable list of attributes, e.g. the field “mould compound” will only show up for packages, while “die  size” is only visible for  component type = die. With a rapidly  changing product portfolio, this hierarchical data model is able  to cover future developments.


Figure 5: Different product and subcomponent types


Figure 6: Modular product data model


Statistics and Reporting


During the analysis process each job has a certain status, e.g. on queue, work in progress, on hold, finished etc. All status  changes are logged in the database, allowing detailed statistical  evaluation of turnaround times (TAT). Also the actual working  time spent by the analysts can be entered for each job. By  combining TAT and working time, the flow factor can be  calculated. Cost transparency is another task for the lab  management. The information in the database allows accurate  cost calculation for the lab’s in-house customers. The  evaluation of the recorded tasks provides information about  the usage of particular analysis methods and can point out to  bottlenecks of equipment resources (e.g. SEM, FIB).


Data Security


Although the system completely resides within the corporate  network and is not connected to the internet, access to analysis  results is restricted. For some basic protection, users need a  valid account to log in at the web application. In addition  access permissions can be individually adjusted for each single  job using 3 different security levels:


• “for internal use” (access for all users)


• “limited access” (access only for defined group of users)


• “confidential” (no intranet web access)


This concept makes the data easily available for a large  number of users while still protecting the company’s  intellectual property.


System Architecture


Software


The system consists of 3 software components:


• a database


• a Windows-based application used by the lab staff (analysts and managers)


• a web application used by company-internal FA customers  to retrieve analysis results and submit new jobs


The Windows lab application provides better performance, while the advantage of the web application is the missing  installation effort for the large number of users.


One Database?


Putting all the company’s FA data into one single giant  database would have caused many problems, especially  regarding performance and flexibility. Therefore a mixed  architecture with both local and global components was chosen (Fig. 7). Each lab has its own local database which allows  location-specific configuration of the workflows to adapt the  tool to the particular business processes. As these local


applications can work independently from each other, the  complete system is very fail-safe. This architecture also  provides maximum database performance because the majority  of database queries are performed locally.


In addition there is a global search application that connects to  all local systems to perform simultaneous search queries. The  global search enables the users to find and share information  e.g. about the same product or technology at other sites.


Figure 7: Mixed system architecture with local and global  components


Interfaces


To avoid redundant and error-prone manual data entry, several  interfaces to other tools were implemented. Some interfaces  are used to submit complete analysis requests to the FA lab, e.g. from a complaint management system (covering the  customer complaint process) and a reliability planning tool (handling of qualification tests). Other interfaces allow  automatic import of detailed product information and user data (Fig. 8). The list of available interfaces includes:


• complaint management system


• reliability planning tool


• corporate address book


• product database (design data)


• lot number database (manufacturing data)


• archiving system (long-term archiving of old jobs)


Figure 8: Interfaces to other corporate IT systems


Conclusions and Acknowledgements


Meanwhile the new system has been rolled out at 15 labs and  is used by approx. 500 analysts and several thousands of  company-internal FA customers. Every month over 4000  analysis jobs are processed by the tool. The flexible  architecture made the adaptation to all the different business  processes possible and provides a future-proof solution. According to user surveys, the acceptance of the new tool is  very high, and all user groups recognize improvement of their  working processes. This confirms the decision of choosing a  proprietary solution that is tailored to the company’s  individual requirements.


The author would like to thank all present and past members of  the project team for their great work and dedication. Special  thanks go to Michael Beck, Karl Berglind, Folke Bruns, Joao  Gomes, Alexander Junghans, Gülnur Kösesoy, Werner Lehner, Peter Meis, Stefan Oberstein, Alexander Olbrich, Gerd  Roppelt, Michael Schebesta, Christian Schellenberger, Karin  Siefert, Filipe Silva, Miguel Torres, Constantin Wiemer.


[1] “Laboratory Information Management System”, Wikipedia Online Encyclopedia accessed July 28, 2006, http://en.wikipedia.org/wiki/Lims


[2] Richard J. Ross, “Management Principles and Practices  for the Failure Analysis Laboratory”, Microelectronics  Failure Analysis Desk Reference Fifth Edition, ISTFA  2005


New Approach: Sample preparation techniques for plastic small outline package (front-side and backside).


Erwin Marquez and Dat Nguyen


Texas Instruments Inc 12500 TI Blvd. M/S 8738 Dallas, Texas 75243  Email: erwin-marquez@ti.com, Phone: 214-8868913


As device packages become smaller, the job of failure  analysts becomes more difficult. Other complex  configurations such as Small Outline Packages (SOP) pose  unique problems. The difficulty of removing the encapsulant  while preserving the integrity of the die, bond pads, bond  wires and lead frame interconnects on a small outline  package pose a serious problem. A new sample preparation  technique is offered in order to expose the front side and  backside of the die. This technique dramatically reduced the  risk of damage and ensures the functionality of the device  after decapsulation.


In this paper, two sample preparation techniques for Small  Outline Package (SOP) devices will be presented. The first  technique is for front side sample preparation. A new  procedure using a jet etching system decapsulation was  developed specifically for small outline package devices. The  encapsulant is removed while preserving the integrity of the  die, bond pads, bond wires and lead frame interconnects. In  addition, we will show a method to eliminate the need for  repackaging for backside sample preparation. Both techniques  allow the failure analysts to do front-side or backside analysis  on any small package device.


The Small Outline Package (SOP) is a low-profile  rectangular surface-mount component package. Its chip is  bonded to an inner land contact area (usually a lead frame). External terminals exit parallel to the seating plane on two  opposite sides of the molded, flat package. SOP uses gull  wing formed leads and is a surface mount package with a  fixed lead pitch.


Figure 1: Cross-sectional view of a SOP device (Cavity up).


To enable successful failure analysis for this package type, we developed a failure analysis sample preparation method, which facilitates backside and front-side failure analysis  methods.


Figure 2: Plastic small outline package on US nickel.


Sample preparation procedure (Front-side)


One solution to the problem is to insert a second layer  between the gaskets. An Aluminum strip was inserted  between the gaskets before running the automated jet etching  system. Removing the plastic to expose the die usually  involves bending the leads out straight and using an  automated jet etching system. A small window (about the  size of the die) will be cut on the Al strip using a sharp  stencil under the microscope. Once set, the software enables  an entire etching program to be completed. This procedure  includes the following four steps:


1. Mounting the device in the position gasket.


2. Placing with the Aluminum tape in order to define  the area to be removed.


3. Mounting the second gasket.


4. Running the recipe from the automated jet etcher.


## New Approach: Sample preparation techniques for plastic small outline package ( front- side and backside).


253


Mounting the device on a position gasket.


The cornerstone of the successful acid decapsulation is the  correct selection of both the position and definition gaskets. Determine the width and the length of the package base from  the mechanical data or by direct measurement. The function of  the position gasket is to position the package and hold the  sample.


Figure 3: The position gasket firmly holds the device.


Covering with Aluminum.


Normally, a definition gasket is used to define the area of the  package that will be exposed to acid. But due to the very  small dimension of the die, Aluminum tape was used.


Using a sharp stencil knife create a small window in the  Aluminum. Remember that the size of the window should at  least match the size of the die that you want to expose. Cutting should be made under an ordinary optical  microscope for accurate result. This cut will define the area  that you want to be removed during the decapsulation  process.


Figure 4: Covering with Aluminum tape.


Mounting the second gasket.


Using vacuum grease, gently apply the sample to one side of  the secondary gasket and stack it above the position gasket  and the Aluminum. Ensure that the alignment between the  position and the secondary gasket is the same.


Ensure that the window in the Aluminum tape has no  contamination that will prevent the acid flow. The acid  should go freely and continuously remove the defined area.


Figure 5: Mount the second gasket and cover the Al strip.


Figure 6: shows the complete cross sectional view of the  entire sample preparation technique for front side  decapsulation. The Aluminum tape offers many advantages.  One advantage is to prevent the possible misalignment. Second, it allows the user to define any window size desired  for exposure.


Figure 6: Cross-sectional view of the front side sample prep.


It is very important to know whether the device has Copper  on top. If there is Copper on top of the device, run a fuming  acid mixture (fuming nitric acid (HNO3)/ concentrated  fuming Sulfuric acid (H2SO4) 3:1 at 70-90 °C. The HNO3 is  the primary enchants and the concentrated H2SO4 protects  the Copper lead frames and Copper bonding wires from  corrosion.


Place the stacked gasket on the decapsulation head. A nozzle  jets into the head from below, through which hot acid is


sprayed against the surface of the sample, etching a hole at  the milled cavity. The fuming nitric acid is taken from the  acid bottle, with the aid of a pump and sent through heat  exchanger. Then the fluid is circulated through the heat  exchanger until it reaches a pre-set temperature. A timer is  used to cut off the flow of the etchant to the device, depending upon package type and configuration.


The automated jet etcher exposes the die by removing the  mold compound. Different types of mold compound require  different temperatures and acid. It is very important to know  the exact type of mold compound, die size and FAB process (e.g. Copper on top) information.


Figure 7: Cross sectional view of the enhanced gasket.


It is necessary to perform the process on few dummy units  and run it on the automated jet etcher in order to standardize  times and ensure proper etching.


Figures 8 and 9 show the excellent result on the SOP  encapsulated device. Bond wire loop profile was preserved, lead frames are all intact, and the device is fully functional.


Figure 8: Optical image of the exposed die of a plastic small  outline package.


Figure 9: Close up view of the exposed die.


Automated milling tool (back-side):


Sample preparation procedure (Back-side)


Special milling techniques for backside sample preparation  eliminate the need for the repackaging process on backside  sample preparation. The development of reproducible  backside sample preparation and failure analysis methods  becomes more and more important because of the increasing  number of metal levels within a semiconductor device and  the ongoing transition to new packages. Quite often the  defects are located in the lowest chip levels, which make  electrical defect localization from the front side very  difficult. Quite often, repackaging is both time and resource  consuming which does not meet the failure analysis goals in  terms of cycle time and efficiency. This paper will give an  insight on providing solutions to meet these demands on  failure analysis.


We demonstrated a method to preserve an incompletely blown  metal fuse to allow analysis and explained how differences in  laser cutting machines resulted in the high failure repair rate of  customer product despite equivalent energy and spot size  settings. Analysis of the fuse bank circuitry on our wafers  helped us to find the critical physical differences between a  fully blown and a poorly blown fuse. By overcoming  difficulties in preserving the blown fuse failure sites for CAFM measurement, laser settings could be easily optimized to  ensure proper fuse opening.


[1] Joseph B. Bernstein, et. al., ”Laser Energy Limitation  for Buried Metal Cuts” IEEE Electron Device  Letters, vol.19, 1998, pp. 4-6.


[2] Joseph B. Bernstein, et. al., “Analysis of Laser Metal  Cut Energy Process Window” IEEE Transactions on  Semiconductor Manufacturing, 2000, pp. 228-234.


[3] K.Arndt, et. al.,“Reliability of Laser Activated Metal  Fuses in DRAMS” IEEE/CPMT Int’l Electronics  Manufacturing Technology Sympoisum, 1999, pp. 389-394.


[4] Jon C. Lee and J.H. Chuang “Fault Localization in  Contact Level by Using Conductive Atomic Force  Microscopy” ISTFA Proceedings, 2003 pp. 413-418.


Figure 4: Reference C-AFM I-V measurement of fully blown  and unblown fuses.


Figure 5: CAFM I-V measurement of the poorly blown fuse. The curve is the same as the curve for the unblown fuse.


Figure 6: Overall I-V curves of the poorly blown, fully blown, and unblown fuses. The poorly blown fuse has a high  resistance metal residue that causes it to appear electrically  similar to the unblown fuse.


Figure 7. Metal residue was revealed by TEM and EDS  analysis.


Combine Nano-Probing Technique with Difference Analysis to  Identify Non-Visual Failures


Cha-Ming Shen, Tsan-Cheng Chuang, Jie-Fei Chang, Jin-Hong Chou


1, Nan-Ke North Rd., Tainan Science Park, Tainan, Taiwan 741-44, R.O.C


The purpose of this paper is to present a novel deductive  methodology, which is accomplished by applying difference  analysis to Nano-probing technique. This methodology would  like to resolve the erratic device with a tailing failure or  puzzling feature, but not only to check if the suspect had  incorrect characteristic or mismatched transistor parameters.


For the application of Nano-probing, four individual tips are  connected to gate, drain, source and well of the transistor as  shown in Figure 1.  An electrical I-V measuring instrument is  coupled to the probe stations in the Scanning Electron  Microscope (SEM) to act as the semiconductor  characterization system.


Figure 1: Schematic diagram of Nano-probing system in  SEM, and the relationship between sample, tips and probe  stations.


In general, Nano-probing is sufficient to provide the data  required for failure analysis because all measurements of  transistor electrical characteristics are performed at the contact  level. However, in some special cases, although the potential  fault had been highlighted by test pattern, measurements of  the threshold voltage (Vth), breakdown voltage of


drain/source (BVds, saturation current (Isat), cut-off current (Ioff), and other data would indicate acceptable values.  Therefore, a more deliberate scheme is needed to overcome  such subtle failure modes which could not be characterized by  the parametric measurements of using Nano-probing nor  global checking of junction behavior [1].


Experiment and Results


In order to prove our novel methodology, the specimens with  90nm process and soft failures were chosen for the  experiment. This experiment started with failure localization  by way of fault diagnosis of test datalog. Then, SEM was  utilized to inspect abnormality after deprocessing layer by  layer down to the contact layer. Eventually, the SEM Passive  Voltage Contrast (PVC) is used to image the N+/PW contacts. Figure 2 shows the localized position where the PVC contrast  is higher than normal.


Figure 2: SEM PVC micrograph of N+/PW contacts at  located failed address ater delayering to contact layer  showing brighter PVC than reference contacts (right). Click  and hold “Styles and Formatting”, then drag it up to your  menu bar.


To further understand the failures on the device, electrical  characterization using C-AFM was conducted. But the


## Combine Nano-Probing Technique with Difference Analysis to Identify Non- Visual Failures


264


acquired electrical characterization from C-AFM (Fig. 3) did  not show any abnormalities that could account for the  anomaly observed during the SEM PVC analysis (Fig. 2).


Figure 3: C-AFM I/V curve. No abnormality was observed at  the failure site. The I/V curves taken at the failure site are  virtually the same as the reference sample.


Therefore, the application of Nano-probing was boosted to get  more electrical information to understand the defect type. In  our Nano-probing system, Zyvex KZ100 manipulator  controller system was installed on the Philips XL-40 SEM, and a Keithley 4200 semiconductor characterization system  was used for I-V measurement to acquire related transistor  parameters. Then three tungsten tips were connected to the  controlled manipulator probed to the gate, drain, and source of  the localized MOSFET, and the fourth tip contacted on the  well or substrate directly as shown in Figure 4.


Figure 4: Three probes contact on the n-channel MOSFET. The Gate probe is connected to the poly-gate of failed passgate, and the Drain / Source probe were connected to the  assigned drain and source. And the fourth tip connected to the  well was on the far side of this located failure transistor.


The common I-V characteristics and parameters related to the  on and off state of the transistor were measured in our Nanoprobing system and are shown in Table 1 and Figure 5.  These  results do not show any excessive feature or mismatched  characteristics. [2]


Table 1: Comparison of the  measurements  of transistor  parameters for  failure and reference.


Figure 5: Nano-probing results of failed and reference  devices showing no obviously excesssive features or  mismatched characteristics.


At first, considering the first failure model that lightly doped  drain (LDD) implantation was blocked, so the channel under  gate would be disconnected at drain site. Then the saturation  current swept from drain to source would decrease to behave  as high resistance contact. In such condition, an extra voltage  drop would fall between drain and source as in Figure 6 and 7.


Figure 6: The cross-section and implantation profile of the  first failure model showed the disconnected implantation  region would behave as a very high resistance.


Figure 7: The simulation result showed that saturation  current from drain to source would decrease to a half if the  implantation at LDD region had been blocked as the first  failure model.


Next, considering the second failure model that pocket  implantation of suspected transistor was blocked in the  meanwhile. Then, the depletion region would encroach to  contact the drain when a larger Vd was forced. So a punchthrough current associated with forced drain voltage would  arise to be the additional current component. In other words, the first failure model was similar to a gate controlled punchthrough transistor with a strong coupling between drain and  source as shown in Figure 8 and 9.


Figure 8: The cross-section and implantation profile of the  second failure model showed the pocket implantation nearby  the channel was blocked.


Figure 9: The modified simulation result showed the quasi  punch-through current associated with forced drain voltage  would arise an extra current component if the related pocket  implantation was also blocked as the second failure model.


So combing the differential analysis results and corresponding  failure models, such erratic failure mode should be caused by  abnormal pocket and LDD implantation. And because the  induced effects on electrical characteristic of such two failures  counteract each other, there is an artifact phenomenon with  matched measuring and drift current. So after summing up  both failure models, the synthesizing result and simulation  agreed with above different components proportionate to the  amount parameter. But the faking balance would be ripped up  in self-latch circuit when writing data, and the poor switching  capability caused the device to fail.


Furthermore, the feedback from in-line KLA team confirmed  that our ratiocination about the compound failure models was  accurate and valid. At last, these suffered wafers were  identified out by the similar test datalog, and the monitored  defect picture is shown in Figure 10.


Figure 10: Peeling particle of LDD photo resistanc  discovered by KLA team in the corresponding stage of  manufacturing process.


Summaries and Conclusion


The aim of our work was to overcome the difficulty in  detecting non-visual, erratic, and complex failure modes. And  the original idea of this deductive method was based on the  complete measurement of electrical characteristic by Nanoprobing and difference analysis.


The capability to distinguish erratic and invisible defect was  proven, even when the compound and complicated failure  mode resulted in a puzzling characteristic. So this  methodology was successful.


[1] C. Giret and D. Faure, “Electrical Characterization by  Sub-micron Probing Technique on 90nm CMOS  Technology for Failure Analysis”,  Proc IPFA 2004, pp. 65-67.


[2] W C.C. Wu and J.C. Lee, “Single Device  Characterization by Nano-probing to Identify Failure  Root Cause”,  Proc.  ISTFA 200, pp. 346-351.


A Technique for Reliably Preparing Full-Length Metallographic Cross-Sections of  Integrated Circuit Bond Wires


Carl Nail


National Semiconductor Corporation, Santa Clara, California, United States  carl.nail@nsc.com


Many problems encountered in failure analysis and product  development require analysis of the bond wires connecting the  integrated circuit die to the leadframe of the package. As an  example, electrical identification of an open circuit at the wire  is generally followed by physical identification of the point in  the wire where the open occurred (usually the ball bond, stitch  bond, or a package crack breaking the wire) and  characterization of the mechanism to establish the root cause. These wires are often encapsulated in a glass particlereinforced polymer package material, preventing direct  examination. Examination of the wires using radiographic  techniques, while valuable, provides insufficient resolution to  identify microcracks and other fine defects; it is also unable to  provide chemical data for addressing possible contamination  issues. Thus, removal of the package material surrounding the  wire is often required to facilitate examination of the wire. Chemical and plasma decapsulation techniques often  introduce artifacts that can invalidate the data obtained. These  can include damage to the free wire during subsequent  cleaning and inspection, loss of package material that might  yield information on cracking or delamination, or etching and  removal of contaminants and/or corrosive agents potentially  contributing to the failure. Focused ion beam cross-sectioning  is usually impractical because of the size of the wires and the  difficulty in locating them for sample preparation. The only  remaining technique for exposing the wire with a minimum of  preparation artifacts is metallographic cross-section.


Even though at least one authority has characterized crosssectional analysis as a “last resort” because its inherently  destructive nature often makes subsequent electrical testing  impossible [1], this is not entirely true. The ideal cross-section  exposes the entire wire simultaneously, allowing for direct  examination and/or measurement (including electrical  microprobing) of all interfaces and materials simultaneously. Given the small size of the bond wires and the angles they  make with the package and the leadframe, such a cross-section  can be extremely difficult to prepare. Aspect ratios in the  plane of section of 50:1 and greater are not uncommon,


requiring angular accuracies of less than one degree to ensure  capturing the full length of the wire. The difficulty in  obtaining such accuracy is compounded by the fact that most  standard package mold compounds are very nearly opaque. Because they cannot be seen, preparing high-precision crosssections of these ‘blind’ bond wires is virtually impossible to  accomplish using optical techniques alone. To overcome these  obstacles, a different technique has been developed that  generates reliable, repeatable cross-sections of bond wires  across most or all of their lengths, allowing unencumbered  and relatively artifact-free analysis of a given bond wire.


The basic method for cross-sectioning a ‘blind’ bond wire  involves a two-step procedure: radiographic analysis of the  sample and metallographic preparation of the sample to the  plane of interest.


Radiographic Analysis


As mentioned earlier, the key obstacle to obtaining high  precision in cross-sectioning packages is the inherently  opaque nature of the package material. Of course, navigators  on ocean-going ships have had the same problem for centuries  of not being able to see their final destination from where they  begin their voyages. They overcame it by creating accurate  charts and techniques for measuring progress towards a  destination. Much the same idea is used here. Instead of  charts, however, radiographic images of the part will be used  to ‘map’ the location of the wire of interest. Progress through  the cross section will be plotted on the radiograph, with  corrections applied as needed to ‘stay on course’ towards a  completely planar wire section.


The sample used to illustrate the technique is a leadless  leadframe package (LLP). The analyst will require access to  radiographic equipment capable of producing a hard-copy  printout with feature resolution in the twenty-micron range or  better. While a full 8.5” x 11” printout format is preferred, these techniques were perfected using 4” x 5” thermal printer  images; such print capability is completely acceptable. X-ray


## A Technique for Reliably Preparing Full-Length Metallographic Cross-Sections of Integrated Circuit Bond Wires


268


voltage and current settings should be the minimum that will  allow for the highest resolution and the best contrast for your  combination of equipment and sample.


As always, the sample should be optically inspected and  documented for any anomalies prior to destructive analysis. During inspection, any obvious externally visible features that  will later assist in tracking the cross-section should also be  noted. For example, the LLP has many visible leads on the  bottom surface, but is nearly featureless on the top surface. Consequently, the radiographs of the part were obtained  bottom-side up, to facilitate charting the cross-section against  the visible leads.


Once a radiograph is obtained, the analyst must identify two  planes. The first is the plane through which the wire of interest  passes (the ‘plane of interest’.) The second is a plane through  which the mount will be sawn after the metallographic mount  containing the sample has cured. This plane should be selected  so that it passes through features as clearly visible as possible  optically on the sample. The plane should also be set far  enough away from the plane of interest to allow for any  corrections to the plane during subsequent grinding of the  sample; it should also be clear of any die to minimize die  cracking during preparation. The lines representing these two  planes are then drawn on the radiograph. An example of such  a radiograph used for preparation of the LLP sample is shown  in Figure 1.


Figure 1: Radiograph of packaged part.


A. Line drawn on image to indicate plane of section for  the bond wire of interest.


B.  Line drawn parallel to the line shown at A indicating  the saw line for the mount.


Metallographic Preparation


Once radiographic analysis is complete, the sample may be  mounted using standard metallographic techniques. The


encapsulant used for mounting should be a clear-curing epoxy  with good edge retention. The sample in this example was  placed in a disposable mount cup which was already halffilled with previously cured epoxy. The sample was placed  with the leads facing up consistent with the orientation during  radiography, after which the mount was filled with freshly  mixed epoxy, vacuum-impregnated, and again allowed to  completely cure overnight. The next morning, the mount was  extracted from its cup and the sharp rim was ground off the  top edge. At this point, a permanent fine-line marking pen is  used to draw a line on the mount matching that of the ‘cut  line’ B shown in Figure 1. A glass slide is placed over the  previously identified features on the sample to align it  correctly, and then the line is drawn using the slide as a ruler. The process is shown in Figure 2; the final product is shown  in Figure 3.


Figure 2: Line is drawn on the mount through visible external  reference points on the part to indicate cutting axis for the  saw.


Figure 3: Higher-magnification view of line along which the  saw cut was made on the mount shown in Figure 2.


The part is then secured in a metallographic saw and cut along  the drawn line. It should be noted that the actual cut made by


the saw does not have to pass exactly through the line as  drawn. What is important is that the saw line is as close to  parallel with the desired final plane of section as possible, to  minimize the need for later corrections to the grinding plane  during subsequent sample preparation.


slide or clear drafting triangle. This allows the metallographer  to accurately track progress through the mount, adjusting  angle


and speed of the grind to permit stopping at exactly the right  plane of section. Examples are shown in Figures 4 and 5.


Tracking Progress


In general, only two features, widely separated, are needed to  establish the position of the current plane. A third point is  recommended as a check; of course, additional points are  welcome to establish a high degree of confidence. Viewing  external structures visible through the mount (such as the lead  surfaces) can also provide a ‘sanity check’ that the current  plane is correctly identified and not, for example, two or three  leads further in. The plane shown in the section  photomicrograph in Figure 4 is established by the three ball


After sawing, the mount is hand-ground using generally  accepted metallographic techniques. The prepared surface is  inspected frequently, using a stereomicroscope, to establish  the position of the plane of section with respect to the  package. Using the now-visible internal and external package  structures in the plane of section, the exact location of the  plane is indicated and tracked on the original radiograph using  a glass


Figure 4: Package in mount with grinding process partially  completed. Bond wires in the plane shown in the photograph  match those shown at the dotted line in the radiograph. This  dotted line is parallel to the line drawn through the wire of  interest, indicating that no corrections are necessary at this  point.


B. Line drawn parallel to the line shown at A indicating  the saw line for the mount.


C. Dotted line indicating the plane of section shown in  the photograph.


A C


Figure 5: Package in mount with grinding process completed  through 600 grit. Bond wires in the plane shown in the  photograph match those shown at the dotted line in the  radiograph. This dotted line is parallel to the line drawn  through the wire of interest, indicating that no corrections are  necessary at this point. Boxed region shown in Figure 6.


C.  Dotted line indicating the plane of section shown in  the photograph.


bonds, the single wire to their left (the wire would appear  significantly different, or not at all, if the section were deeper   in) and correlation between the sectioned leads on either end  with their surface appearance in the mount.


In the event that inspection reveals a misalignment in the  plane of section as it is being prepared, the analyst must begin  taking measures to correct the direction of preparation. This  usually consists of one of two types of grinding variations: either apply differential pressure to the mount (heavier on the  side that is not ground as deeply as the other) or, if a grinding  wheel is being used, apply uniform pressure without counterrotating the mount on the grinding wheel at the outside edge  of the grinding media, with the side that is not ground as  deeply being closest to the outside rim of the wheel. This  takes advantage of the higher sheet feet per minute speed  found at the larger radial distance from the center of the  wheel. The further from the center, the faster the speed, and  the faster the removal rate [2]. Continue to monitor progress  until the problem is corrected.


Darkfield Imaging


The sample in Figure 5 is prepared through 600-grit silicon  carbide (SiC). At this distance from the wire (approximately  100 to 200 microns), the analyst can begin taking advantage  of some of the optical properties of the mold compound to  facilitate viewing the wire of interest. The glass reinforcement  particles and epoxy resins of most mold compounds are  slightly translucent, allowing light to penetrate somewhat  below the surface of the sample. Direct lighting through the  lens generally floods the surface with too much light to see  any subsurface details. However, using a fiber-optic ring  illuminator on a stereomicroscope or darkfield illumination in  a standard metallographic microscope sends grazing light  across the surface at a shallow angle. The light is scattered by  the translucent materials and creates a ‘backlit’ effect within  the sample, allowing for some illumination of subsurface  features. This effect has been observed by other investigators  in the past, especially as it applies to printed circuit boards [3]. In fact, a good time to convert from 600-grit to 800-grit SiC is  when the wire of interest becomes visible in darkfield.


The next series of images will serve to illustrate this  phenomenon. Figure 6 shows that region of Figure 5  containing the wire of interest. Though the image does not  reproduce particularly well, it does reveal some locations  where the wire is beginning to be visible. Figure 7 shows the  same region after approximately one minute of grinding using  800 grit. The wire is now clearly visible below the surface of  the part. After a second minute of grinding at 800 grit, the  ability to resolve significant features of the wire is  substantially improved, as shown in Figure 8. Compare this  with another image of the same area obtained using brightfield  illumination (shown in Figure 9). Note that, even though the  mold compound above the wire has been substantially  thinned, it is still nearly impossible to see the wire because of  the amount of light reflected from the surface of the sample


and the absence of scattered light within the sample that had  been provided by the shallow-angle illumination.


Figure 6: Area of section shown in box in Figure 5. Darkfield  illumination is just beginning to reveal the wire location  through certain glass particles (at arrows).


Figure 7: Area in Figure 6 after approximately one minute of  grinding at 800 grit. Wire in darkfield is now clearly visible.


The intrinsic value of using darkfield imaging in this  application is twofold. First, the ability to detect the wire of  interest earlier in sample preparation significantly reduces the  risk of inadvertently damaging or destroying the wire. Material removal rates can be reduced in a timely fashion  without compromising speed and efficiency in sample  preparation. Second, the ability to resolve fairly detailed  features of the wire below the prepared surface means that, often, the entire wire need not be exposed. This can be  extremely important in circumstances when either the angle of  approach is not perfect, or the wire has sweep or kinks that  place portions of the wire well out of the two dimensional  plane of section. These conditions result in part of the wire


being buried in mold compound when the rest of the wire is  exposed and sectioned. The ability to image the wire even  under these circumstances significantly enhances the ability of  the analyst to deliver useful results to the customer even with  less than perfect sample preparation.


Figure 8: Area in Figure 7 after approximately one additional  minute of grinding using 800 grit. Wire visibility in darkfield  continues to improve.


Figure 9: Area shown in Figure 8 using brightfield  illumination. Note that the wire is barely visible, though ball  and stitch bonds can clearly be seen (at arrows).


In the case of the sample preparation in this example, the wire  sweep, though minor, has still made obtaining the full wire  section too risky – the chances of sectioning through or  pulling out the wire in later polishing steps is too great. Figure  10 shows the sample after the final grinding step at 1200-grit  SiC. Though the wire is not completely visible in brightfield  illumination, it is clearly visible with good resolution in  darkfield. The sample, as prepared, will permit inspection of  all wire surfaces and interfaces. It will also permit  microprobing, if needed, of the die bond pad, the ball bond,


the wire above the stitch bond, and the pin. This allows for  confirmation of the location of a circuit open even if visual  inspection of the wire is not conclusive. Preservation of the  surrounding package material also permits visual inspection of  any cracking or delamination that may have contributed to a  wire break, assisting the analyst in determining the root cause  of a failure.


Figure 10: Area in Figure 9 after grinding at 1200 grit, brightfield illumination. Ball, stitch, and wire surfaces of  interest are revealed to the satisfaction of the customer. Minor  wire sweep creates too much risk to pursue additional  grinding to reveal remaining portion of the wire.


This technique has been used to expose wires on 37 different  samples to the satisfaction of the customers and this analyst. In several cases, subsequent electrical analysis of the sample  has revealed information for the analyst that has led to finding  the root cause of failure; data that could not have been  obtained without exposing both the ball and the stitch bonds  simultaneously.


My thanks to Terry Vincent at National Semiconductor for her  discussion on the use of radial speed differences as a grinding  tool. My thanks also to Gwen Nail for her assistance with  editing and photodocumentation.


[1] Martin, P. L., Electronic Failure Analysis Handbook, McGraw-Hill (New York, NY, 1999), p. 12.11.


[2] Vincent, T., National Semiconductor Corporation, Santa  Clara, California, 2005, Private Communication.


[3] Vanderlinde, W. E., “Forensic Microscopy in the Failure  Analysis Laboratory,” Proceedings of the 26th  International Symposium for Testing and Failure  Analysis, Bellevue, Washington, November, 2000, pp.101-2.


130nm Backend Reliability Failures: Analysis to Corrective Action


Gil Garteiz, Amir Zylberman


Tower Semiconductor, Israel


gilga@towersemi.com, amirzi@towersemi.com


Tower successfully completed a product qualification of its


130nm copper process this year. The key to this achievement  was finding and eliminating a dominant failure mechanism,


which appeared during HTOL stress. This paper will cover the  failure analysis, in-line problem identification, and corrective  actions taken that eventually lead to successful product


qualification.


Tower uses an SRAM array for 130nm technology


development and process qualification. The first attempts to  pass HTOL stress testing with this vehicle failed with high


failure rates. Failure modes were functional predominated by  single bit and column failures sometimes coinciding with


elevated levels of standby current.


Electrical Characterization


Electrical tests and characterization of the failures showed


their behavior was consistent with shorted nodes inside the


SRAM array. In column failures, shorts from failed columns to  ground were measured. In single bits, shorts were found inside  memory cells, or from individual memory cells to VDD / VSS.


Fault Isolation


For single bit failures, no further isolation is necessary since  the physical location of the failed bit is known. In some cases  the actual shorted node inside the single bit is known based on  analog test results as previously explained1.


For column failures, Thermal Laser Stimulation (TLS) was


used to pinpoint the short locations (see Fig. 1).


Physical Analysis


Layer removal by parallel lapping followed by SEM inspection  was used to identify the physical defects causing shorts.  The  challenge was to remove material until <=100nm of dielectric  remained above the desired metal layer for inspection.  This is  necessary because in copper technologies it is more likely to


have a short circuit on top of metal lines than near the bottom  as in aluminum-based process flows.


Figure 1: TLS pinpoints the short location in a failing column.


After finding the failure mechanism (see Fig 2), further


analysis was required to identify it and determine how / when  in the process it was introduced. To this end, cross-sectional  TEM specimens were prepared.


Figure 2: SEM inspection showing a typical defect shorting  two Cu lines.


S/TEM imaging and EDS analysis revealed two key pieces of  information. First, the defect was composed primarily of


copper, and second; the defect was introduced during


fabrication (See Fig. 3).


## 130nm Backend Reliability Failures: Analysis to Corrective Action


273


Mechanism Summary


Copper residues or “flakes” were being deposited or being


formed by corrosion likely during or after the copper polishing  process step. These flakes could cause failures in HTOL and  not at wafer probe for several reasons. Two possible


explanations follow:


First, the flakes created high resistance shorts between copper  lines and compromised the nitride - barrier seal. The shorts did  not result in functional failures at wafer sort, but left a pathway  open for copper to migrate along the short and slowly lower


the resistance until functional failure did occur.


Second, when the flakes were initially deposited, a very small  oxide layer or distance existed from adjacent metal lines. This  layer was strong enough to isolate the short during the wafer


probe, but not enough to pass HTOL.


Figure 3. S/TEM imaging of a typical defect. Note that the  nitride layer directly above the Cu lines conforms to the


defect. This indicates its presence before the nitride was


deposited. On the other hand, the observed void must have  been formed sometime after the nitride layer deposition; otherwise it would have been filled in.


Process Correction  In-line Inspection


Establishing that in-line defects caused HTOL failures meant  that potential failures could be caught in-line through


inspection. It would be much faster to inspect wafers for flakes  after short process loops than to process devices to end of line, assemble them, and run HTOL to accomplish the same thing. Therefore short metal loops were run and inspected. All


defects found were reviewed manually to discard irrelevant


defect types (voids etc.). Potential failure-causing flakes were  identified (See Fig. 4).


Figure 4. In-line SEM image of a typical Cu flake found on a  Cu line. Line: light grey, space: dark grey.


Process Splits


Once reliable in-line detection of these defects was in place, several process splits were devised and run. Results from full  inspection of all splits were then evaluated.


Figure 5.Evaluation of splits based on in-line inspection  results. X-axis: process splits A, B, and Standard, Y-axis: reviewed defect count.


Process splits investigated included several variables such as: Down force during polish, polish time, post-polish clean time, cleaning recipe, post cleaning treatment, and queue time delay (to next layer processing).  The most beneficial effect was


noticed when modifying the post-polish cleaning recipe.


Figure 5 shows results evaluating two cleaning recipes (splits  A, B) with respect to the standard. Process split B was selected  as the final corrective action.


New Qualification Results


After implementing the new process change, the EFR and AFR  failure rates for this technology were reduced by factors of 3.4  and 2.75 respectively.


A case study on a 130nm reliability failure and process


corrective action has been presented. The failure mechanism  found – copper residues after copper CMP – poses an


interesting challenge: Trying to keep an inherently dirty


process step clean. Good results were obtained in this case by  fine-tuning the cleaning recipe.


1. G. Garteiz, Failure Analysis of Functional Failures in a  Designed for FA SRAM, 30th ISTFA Proceedings, p. 581 (2004).


Rapid Yield Learning with Effective Integration of FMEA design for DOE on Test Chip


Ivan A. N. Goh, Russell McMullan, Brock Fairchild, John Ilzhoefer


Foundry Technology Engineering,


Texas Instruments Inc., 13560 North Central Expressway, MS3735, Dallas, TX 75243  ivan.goh@ti.com, (214) 801-3522


As semiconductor technology advances from one node to the  next, fabrication also becomes increasingly challenging to  ramp up production with the most desirable yield and reliable  product in a timely manner. At an advanced technology node  such as 65nm, the interaction between product design, process  margin, and process equipment continues to limit the product  yield and reliability performance.


Traditional methods, which usually rely on sequential  feedback of each experimental lot, require too many learning  cycles to achieve target performance, yield, and reliability  levels.


This paper describes a methodology that potentially  accelerates the progression of identifying process and productdesign interactions and marginalities during the development  stage. Not only can this methodology result in a quicker ramp  to production, it also has the benefits of improving costs, yield, and reliability.


Various manufacturing issues that affect product  performance and reliability


With past technology nodes, yield ramp from technology  development to production was limited by production line  random defect density, complexity of the product, and the  process robustness. However, at 130nm and more advanced   nodes, great efforts have been spent solving product-toprocess and process-to-toolset sensitivities, which result in  complex parametric yield and process robustness issues [1, 4]. Some of these design-for-manufacturing (DFM) issues can be  attributed to tighter design rules for SRAM and logic  components that result in increased device-to-process  interactions. These interactions may reduce process margin  needed for optimal product performance [2, 3]. In addition, yield issues due to speed and timing margins have also  required additional rounds of design fix. Providing a solution  for these issues can lead to more robust process baseline and  more reliable product.


Adding to these DFM issues is the distribution of more and  more production across several factories on various locations. Even more complications may arise as toolsets and software  between these factories are not consistent. In order to achieve  target product yield level or defect density within budget and  timeline requirements, it is imperative that a fast and effective


method is used to identify critical areas of interaction between  product design sensitivities, process marginalities, and toolset  differences.


Using FMEA test chip arrays for rapid yield  learning


Careful analysis of critical product design and process  interactions can be identified using standard failure mode  effect analysis (FMEA). Risk analysis of these interactions  can be performed and mitigated by applying various FMEA  test chips arrayed across the reticle floor plan. This approach  allows yield and reliability learning to occur at each process  baseline learning cycle. When this type of learning occurs, the  outcome produces more efficient learning with fewer learning  cycles, and it provides a yield ramp in a more cost-effective  manner.


This application of different chip design options on a single  reticle can also effectively reduce the number of wafers  required to achieve similar results using typical process splits  to identify process marginality as shown in Figure 1.


The failure analysis (FA) resources to achieve yield learning  and early failure rate (EFR) learning are reduced as more  detailed analysis focuses on a few wafers with important  process split conditions. The definition of each die in the array  is listed in Table 1.


Figure 1: 6x6 litho mask layout for various FMEA option. A  represents Nominal Design; B is Vmin; C represents Beta, and D is Contact and Poly design adjustments in the  embedded SRAM.


## Rapid Yield Learning with Effective Integration of FMEA design for DOE on Test Chip


276


Table 1:  Definitions of FMEA options shown in Figure 1.


Option Cell


Design Definition


A Nominal  Cell


These chips have nominal placement  and sizing of all SRAM and Logic  features.


VMIN  Cell


In VMIN cell design, the size of a


driver gate transistor is varied from the  nominal size in order to evaluate the


sensitivity at which Vmin soft fails


become increasingly more prevalent at  the 90nm node and below.


BETA


Test Cell  Design


IN BETA test cell design, the size of all  the core PMOS gate CDs are reduced  from nominal sizing to identify the


interaction and matching of NMOS and  PMOS transistors in the SRAM


possibly influencing SRAM


performance.


D ContactPoly Cell  Design


In the contact-poly SRAM array, risk in  contact loop is paramount due to the


tight design rule in the SRAM cell


design. The size and placement of poly  gate and contact features in the SRAM  array are crucial. Both factors are


sensitive to etch and lithographic


processes. The design variations of


poly gate and contacts were applied to  test chip D.


The system-on-chip (SOC) product that is considered for  production has sufficiently large areas of SRAM. SRAM, which is designed with more cells per unit area to reduce  production cost, can also result in product sensitivity issues. To mitigate these risks, various layout design-of-experiments (DOE) are considered mainly in the SRAM region. In  addition, the failure modes in a 6-T SRAM are also easier to  isolate and characterize with bitmap and nano-probe  capability. More detailed physical failure analysis can be  conducted to understand the root cause of the fail mode.


By understanding the critical nature of FMEA in the SRAM, different design options are able to be implemented across the  reticle shot. As a result, more data is collected from each  wafer within this reticle set compared to a standard nominal  design reticle set for each learning cycle. In addition to the  data from the nominal dies, more data is extracted from the  other dies with alternative options (e.g., B, C and D). The  number of silicon wafers that are required to accomplish  similar experimental objectives, compared to a product with a  normal reticle set, are reduced by approximately 50%.


Results from FMEA design DOE test chip


The arrayed reticle design discussed in this paper helps to  explore several process-design interactions. The optimal  design option for the production reticle set could be identified


from the results of the initial arrayed experimental mask set  and the various process optimization activities. The design-toprocess interactions had measurable impact on inline process  data, inline defects, voltage contrast (bright or dark) data, electrical parametrics, wafer sort bins, yield, SRAM bitmaps, and limited burn-in data. The final decision for the process  and product design requires a more complete dataset.


Selecting the best option for mass production


Performing a side-by-side analysis of options A through D, the contact-poly cell option D with optimized contact size, shape, and placement in the SRAM area exhibited the best  overall product. And, the SRAM yield performance was  improved compared with other design options.


However, some classical contact issues were observed on  some wafers. These issues included open contacts due to  smaller contact and poly-gate shorted to contact possibly as a  result of larger contacts or non-optimized placement of poly  and contact.  Figure 2 and 3 illustrate these contact issues.


Figure 2: Physical failure analysis showing classical contactto-poly gate short.


Figure 3: Physical Failure analysis showing typical contact


open.


Figure 4 illustrates the yield window defined by contact CD, contact-to-poly spacing. Option D was capable of minimizing  yield loss due to contact opens or shorts. The contact  placement on this design had the largest distance to the nearby  poly line producing the largest margin for gate-to-contact  shorts. For the same option, the early burn-in results looked  very promising compared to the nominal design and other  options. The interaction between etch recipe and etch toolset


sets the post-etch profile of the contact and also plays a very  significant role toward the yield and reliability performance.


Figure 4: Yield window defined by contact process.


The testing results also showed that VMIN and BETA cell  designs yielded poor results due to reduced SRAM margin. Design and process conditions that resulted in these wafer  characteristics were easily avoided in the final production  mask set.


Option D was chosen over the other test cell designs for the  final production reticle set. The initial production with this  option was populated with the various process targets centered  showed a consistent and high yield level for several lots.


Summarizing the steps involved with this methodology is  shown in Figure 5. It provides a quick reference of how using  the FMEA integrated test cell design flow improves yield  learning rapidly for subsequent production ramp.


Figure 5: Integrated FMEA design flow for rapid yield


learning. All the pre-production stages with the arrayed


reticle set are enclosed within the dotted lines.


This paper demonstrates the successful application of a FMEA  design DOE reticle for extracting process-design interaction  information.


Relative Contact CD, Contact-to-poly spacing


Poly. (SRAM Column fails)


Poly. (Yield)


This approach provides insights to early learning cycles in  achieving accelerated critical learning for yield and reliability  improvements. The resources invested to produce the mask set  with various design options are believed to be worth the  upfront preparation costs due to more thorough learning  enabled on process-to-design interactions.


To maximize the benefits of this investment, the equivalent  efforts in generating DOEs on silicon and effective analysis of  the process sensitivities also must occur.


[1] Richard Goering, “90-, 65-nm yields prey to leakage”, EE  Times, 10/24/2005.


[2] Ann Steffora Mutschler, “DFM Is Real, Impacting Yield  Today, Mentor’s Rhines Says”, Electronic News , 7/11/2006


[3] Laura Peters, DFM Becomes More Than Hype, Semiconductor International, June 2006.


[4] P. T. Patel, Yield challenges require new DFM approach, EE Times, 11/21/2005.


Contact  Shorts


Contact  Open


Optimal  Yield


Secondary Electron Potential Contrast for Dopant Profiling of Silicon Carbide Devices


Marco Buzzo


Infineon Technologies, A-9500 Villach, Austria marco.buzzo@infineon.com


Mauro Ciappa and Wolfgang Fichtner


Swiss Federal Institute of Technology (ETH), CH-8092 Zurich, Switzerland.


SiC has been considered for decades as a promising material  for power device applications due to its high operating temperature, high breakdown voltage and dynamic behavior


[1]. The first commercial products were proposed less than 10  years ago and their growth in the market is ratified by their increasing appearance on new generation devices [2]. An increase in available wafer size, and improved manufacturability of SiC wafers have resulted in an increase in  demand for SiC [3] With the increase in demand for SiC  devices, the demand for more reliable characterization and  Failure Analysis  techniques have increase. In order to insure  long term reliability of the SiC product, more reliable dopant  profiling techniques need to be developed. Unlike silicon, SiC  is unique when compared to silicon due to the extreme physical  properties, which make the generally accepted electrical dopant  profiling techniques either unreliable, or not viable.


Presently, scanning probe techniques such as Scanning Capacitance (SCM) and Scanning Spreading Resistance Microscopy (SSRM) are the most common techniques  used for  the acquisition of 2D dopant profiles in sub-micron silicon  devices [4-6]. Both techniques require a conducting probe to be scanned in contact across the surface of a cross-sectioned sample, and the result is an excellent surface image [7]. When used for quantitative measurements, their reproducibility and  repeatability are heavily impacted by the non-idealities of the  samples (e.g. surface states and fixed charges in SCM) and by  the experimental conditions (e.g. applied pressure and bias in  SSRM). The repeatability and reproducibility issues are further exasperated due to extreme hardness of SiC which creates challenge for the conventional micro-sectioning processes, especially when trying to obtain the levels of surface roughness required by the scanning probe techniques.


Furthermore, the tribologic aspects also represent a major issue  for the endurance of the diamond-coated probes used in  SSRM.


Recently, Secondary Electrons Potential Contrast (SEPC) by  Scanning Electron Microscopy (SEM) emerged as a powerful  tool for two -dimensional quantitative dopant imaging [8]. The  main component of the SEPC signal arises from the difference in the built-in potential between differently doped regions;which is very high in wide-band-gap semiconductors and  particularly intense in SiC.


In this paper after discussing the physical principles leading to  the dopant contrast and the proper experimental setup, we will  investigate the impact of relevant factors such as experimental  conditions, surface effects, and sample preparation on the  image quality. The quantitative capabilities of this technique  are demonstrated by the analysis of different test structures  and prototypes of power devices such as MOSFET and JFET.


Mechanism of contrast formation


In bipolar junction, the main component of the SEPC arises as a  consequence of the potential contrast due to the built -in potential, which produces a stray electric field irradiating from  the surface of the semiconductor sample. Along the trajectory  towards the detector, the low-energy secondary electrons (few  eV) are either accelerated or retarded by the local electric field, depending on the emission site.


Fig. 1 Stray potential and stray electric field resulting at the  surface of an abrupt unbiased SiC junction produced by the  built-in potential (simulation by DESSIS).


## Secondary Electron Potential Contrast for Dopant Profiling of Silicon Carbide Devices


Fig. 2 ExB filter consisting of a tube where an electric and


crossed magnetic field deviate the SE depending on their kinetic energies. Only the slow SE can pass through the filter


and reach the detector.


In Figure 1, the stray electric field produced by an unbiased  SiC abrupt junction (ND˜1016cm-3 and NA˜1019cm-3) has been  simulated quantitatively by the device simulator DESSIS [9] under the assumption of a complete dopant activation and that


a grounded detector is placed 400 µm above the sample  surface. The equipotential lines are almost radial and the


surface potential in the quasi-neutral p-type region is higher  than the potential in the quasi-neutral n-type region. In the


quasi-neutral regions the field lines are open loops and point in  opposite directions. The electric field accelerates electrons


emitted from p-type doped regions and retards electrons  emitted from n-type doped regions.


For the junction under consideration the built in potential is  about 3V. In general, Vbi can be expressed as a function of the  dopant concentrations [16] by


ln


bi


q kT


V =


where k  is the Boltzmann constant, T is the absolute temperature, q is the elementary charge, NA and ND are respectively the concentration of acceptors and donors.


The maximum difference in the kinetic energy between accelerated and retarded electrons equals the built -in potential, which is for the junction under consideration about 3V. In  summary, the SEPC image of an unbiased junction is expected  to consist of bright zones, corresponding to p-doped regions, and of dark zones, corresponding to n-doped regions.


Efficient Detection


As described before, the overall range of the signal variation is  within some few Volts. Due to such a reduced dynamic of the  signal, the measurements have to be carried with a SEM  equipped with a suitable SE detector, which can operate


Fig. 3 Sketch of the test structure used to compare the SE  detectors.


as a low-pass filter, in order to cut off the high-energy tail of


the secondary electron spectrum. In the past, through-the-lens detectors (TLD) have been successfully used [10]; however


with the adnvanced SEM technologies, low pass filter has  been implemented by the use of an E×B filter operated in  conjunction with a conventional TLD.


The filter consists of a tube where the perpendicular electric


and magnetic fields are both normal to the SE trajectory (Fig. 2). The design of the filter ensures that only the SE not


exceeding a certain kinetic energy are deflected by the Coulomb and Lorentz forces and can pass through the tube,


and the non filtered SE collide with the walls and are not  transmitted.


The effect of the filter on the signal has been investigated by


acquiring secondary electrons (SE) images with different detectors and under different experimental conditions. The


SEM used is a cold field emission Hitachi S-4700 equipped with  both a conventional Everhard -Thornley (E-T) and a throughthe-lens E×B detector.


A SiC test-structure has been manufactured on a 4H-SiC 4º-off n-type  substrate (ND˜1018cm-3), on which an epitaxial layer (ND˜ 1016cm-3 nitrogen) has been deposited. As shown in Fig. 3, those steps have been followed by the implantation at 320 keV  of highly-doped aluminium p+-wells (NA˜1019cm-3) with a fluence of 2.8 × 1014cm-2. The samples have been manually  cleaved in air.


Figure 4 shows the SEPC maps of the cross-sectioned sample


acquired (a) using the E-T detector at 500V, (b) using the ExB  at 500V and (c) at 20kV. The quantitative comparison of images


has been carried out by extracting the profile of the grey levels  along the symmetry axis of the implanted region, as shown in


Fig. 4d. The profiles have been acquired from the images by  the software analiSYS  and the contrast C has been normalized


and expressed according to the usual relation


sub


where Ix is the grey level at a given location and Isub represents  the average grey level of the substrate layer, assumed as the

