---
title: "ISTFA-2007.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_a48de803a32745f12f8e79ffe5a6a4817295230462135641
file_size: 43141324
---

ISTFA  2007   Proceedings of the


33rd International Symposium


for Testing and Failure Analysis


November 4 – 8, 2007


San José McEnery Convention Center  San José, California, USA


Sponsored by


www.asminternational.org/istfa


www.asminternational.org


Published by


ASM International®


Materials Park, Ohio 44073-0002


TM


Copyright© 2007


by


All rights reserved


No part of this book may be reproduced, stored in a retrieval system, or transmitted, in any form or by any  means, electronic, mechanical, photocopying, recording, or otherwise, without the written permission of  the copyright owner.


First printing, November 2007


Great care is taken in the compilation and production of this Volume, but it should be made clear that NO  WARRANTIES, EXPRESS OR IMPLIED, INCLUDING, WITHOUT LIMITATION, WARRANTIES  OF MERCHANTABILITY OR FITNESS FOR A PARTICULAR PURPOSE, ARE GIVEN IN  CONNECTION WITH THIS PUBLICATION. Although this information is believed to be accurate by  ASM, ASM cannot guarantee that favorable results will be obtained from the use of this publication alone. This publication is intended for use by persons having technical skill, at their sole discretion and risk. Since  the conditions of product or material use are outside of ASM's control, ASM assumes no liability or  obligation in connection with any use of this information. No claim of any kind, whether as to products or  information in this publication, and whether or not based on negligence, shall be greater in amount than the  purchase price of this product or publication in respect of which damages are claimed. THE REMEDY  HEREBY PROVIDED SHALL BE THE EXCLUSIVE AND SOLE REMEDY OF BUYER, AND IN NO  EVENT SHALL EITHER PARTY BE LIABLE FOR SPECIAL, INDIRECT OR CONSEQUENTIAL  DAMAGES WHETHER OR NOT CAUSED BY OR RESULTING FROM THE NEGLIGENCE OF  SUCH PARTY. As with any material, evaluation of the material under end-use conditions prior to  specification is essential. Therefore, specific testing under actual conditions is recommended.


Nothing contained in this book shall be construed as a grant of any right of manufacture, sale, use, or  reproduction, in connection with any method, process, apparatus, product, composition, or system, whether  or not covered by letters patent, copyright, or trademark, and nothing contained in this book shall be  construed as a defense against any alleged infringement of letters patent, copyright, or trademark, or as a  defense against liability for such infringement.


Comments, criticisms, and suggestions are invited, and should be forwarded to ASM International.


ISBN-13:978-0-87170-863-2


ISBN-10: 0-87170-863-9


SAN: 204-7586


Materials Park, OH 44073-0002


Printed in the United States of America


Multiple copy reprints of individual articles available from Technical Department, ASM International.


EDFAS 2007-2008 BOARD OF DIRECTORS


EDFAS President


Mr. Gary Shade


Insight Analytical Labs


EDFAS Vice President


Mr. Tracy Myers


ON Seminconductors


|Board Members |Board Members |Affiliation |
|---|---|---|

|Mr. Gary Shade |EDFAS President |Insight Analytical Labs |

|Mr. Tracy D. Myers |EDFAS Vice President |ON Semiconductor |

|Dr. Lee Knauss |Secretary |Neocera |

|Mr. Richard J. Ross |Past President |IBM Systems and Technology (Retired) |

|Dr. Thomas Moore |Member at Large |OmniProbe |

|Dr. Seshagiri V. Pabisetty |Member at Large |Eagle Registration Inc. |

|Mr. Thomas S. Passek |Executive Director |ASM International |

|Dr. Philippe Perdu |Member at Large |CNES |

|Mr. Matthew Thayer |Financial Officer |Advanced Micro Devices |

|Mr. David P. Vallett |Member at Large |IBM Systems and Technology |

|Board Committees |Board Committees |Affiliation |
|---|---|---|

|Dr. Lawrence C. Wagner |ASM BOT Liaison |Texas Instruments, Inc. |

|Ms. Rose M. Ring |EDFA Chair |SMSC |

|Mr. Thomas Zanon |Education Chair |PDF Solutions Inc. |

|Mr. Chris Henderson |Events Chair |Semitracks Inc. |

|Dr. Aaron Falk |Journal Chair |Tum Focus Instruments Inc. |

|Dr. Vijay Chowdhury |Membership Chair |Altera Corporation |

|Mr. Gary Shade |Nominating Chair |Insight Analytical Labs |

|Mr. Jeremy Walraven |Website Chair |Sandia National Laboratories |

ISIFA/2007 ORGANIZING COMMITTEE


Chris Henderson


General Chair


SemiTracks, Inc.


David P. Vallett


Vice General Chair  IBM Systems


& Technology Group


||Activities Chairs |Activities Chairs |Activities Chairs |
|---|---|---|---|

|Dan J. |Bodoh |Martin Keim |Philippe Perdu |

|User Groups |Chair |Panel Discussion Chair |Audio/Visual Chair |

|Freescale |Semiconductor |Mentor Graphics Corporation |CNES |

|Vijay |Chowdhury |Tom Moore |William E. Vanderlinde |

|Publicity |Chair |EDFAS Liaison |Website Chair |

|Altera |Corporation |Omniprobe, Inc. |Laboratory for Physical Science |

|Robert |Herrick |Tracy Myers ||

|Local |Arrangements Chair |Exposition Chair ||

|Finisar |Corporation |ON Semiconductor ||

Nicholas Antoniou


Technical Program Chair  Consultant


Jeremy Walraven


Tutorial Vice Chair  Sandia National Labs


Cheryl Hartfield


Immediate Past General Chair  Omniprobe, Inc.


s


ISTFA 2007 TUTORIAL COMMITTEE


ISTFA 2007


Tutorial Program Chair


Zhiyong Wang


Intel Corporation


|Tutorial Committee Chair |Topic |Affiliation |
|---|---|---|

|Zhiyong Wang |Lead Free Packaging, Packaging, Lab Management |Intel Corporation |

|Jeremy A. Walraven |EOS/ESD, MEMS Devices |Sandia National Laboratories |

|Tracy Myers |Test and Logic Diagnostics |On Semiconductor |

|William E. Vanderlinde |Microscopy Tools, Fault Isolation |Laboratory for Physical Sciences |

|Becky Holdford |Packaging |Texas Instruments |

|Chris Richardson |FIB, Fault Isolation |LSI Logic |

|Cosme Furlong |FA Basics, Microscopy Tools, Fault Isolation |Worcester Polytechnic |

|Kendall Scott Wills |FA Basics, Packaging, Fault Isolation, Yield |Texas Instruments |

|Leo G. Henry |Failure Mechanisms |ESD-TLP Consulting & Testing |

|Rose M. Ring |Emerging Technologies, Device and Memory |SMSC |

|Susan Li |Device and Memory |Spansion |

|Sam Subramanian |Materials Characterization, Microscopy Tools |Freescale Semiconductor, Inc |

|James Griffin |Analog Device Failure Analysis |Analog Devices |

ISTFA 2007 SYMPOSIUM COMMITTEE


Technical Program Chair


Independent Consultant


CIRCUIT EDIT 1


MIKE PHANEUF, CHAIR


Fibics, Incorporated


MARSHA ABRAMO, CO-CHAIR  IBM Microelectronics


Ted Lundquist, Credence Systems Corp. Chad Rue, FEI Company


CIRCUIT EDIT 2


Ted Lundquist, Credence Systems Corp. Chris Richardson, LSI Logic


Chad Rue, FEI Company


EMERGING CONCEPTS


CHRISTIAN BOIT, CHAIR


TUB Berlin University of Technology  JAMES DEMAREST, CO-CHAIR


IBM


Steven Kasapi, Credence Systems Corp.


FA PROCESS 1 & 2


DAVID BURGESS, CHAIR  Accelerated Analysis


Anat Almog, Intel Corporation


Jeff Birdsley, Dell Incorporated


Pete Carlson, Feico


Yuan Chen, NASA


Steve Ferrier, Metatech Corporation  Jeff Hartsell, Dell Incorporated


Mike Lane, Intel Corporation


Johnny Lee, X-Fab Texas


Randy Lee, Keithley Instruments


Kwi Chuan Ng, Intel Corporation


IN-LINE METROLOGY & ANALYSIS


JANET TESHIMA, CHAIR  FEI Company


Tom Kelly, Imago Scientific Instruments Corp. Du Li


Art Rawers, Xilinx


Jeremy Russell, Inotera Memories


Bryan Tracy, Spansion LLC


NANOPROBING


SHAWN DECKER, CHAIR


South Dakota School of Mines


PHIL KASZUBA, CO-CHAIR


IBM Microelectronics


WILLIAM E. VANDERLINDE, CO-CHAIR  Laboratory for Physical Sciences


PACKAGE & ASSEMBLY LEVEL FA 1


DEEPAK GOYAL, CHAIR  Intel Corporation


ZEZHON FU, CO-CHAIR  Intel Corporation


Stephen Barbeau, IBM


Zezhong Fu, Intel Corporation


Arun Raman, Intel Corporation


Roger Stierman, Texas Instruments


PACKAGE & ASSEMBLY LEVEL FA 2


Andrew Mawer, Freescale Semiconductor  David Maxwell, Texas Instruments


PACKAGE & ASSEMBLY LEVEL FA 3


Ted Kolasa, Freescale Semicondutor


Andrew Mawer, Freescale Semicondutor  Roger Stierman, Texas Instruments


PHOTON BASED TECHNIQUES


STEPHEN IPPOLITO, CHAIR  IBM


AARON FALK, CO-CHAIR


OptoMetrics, Inc.


Franco Stellari, IBM Systems & Technology  Group


POSTERS


KENDALL SCOTT WILLS, CHAIR  Texas Instruments


REENA CHANPURA, CO-CHAIR  Texas Instruments


SAMPLE PREPARATION


ANDY SAXONIS, CHAIR  Analog Devices


Elvis Cooper, Analog Devices


John Guravage, Analog Devices  Tony Tollis, Analog Devices


SPM


RAMA GORUGANTHU, CHAIR  Advanced Micro Devices


JIM COLVIN, CO-CHAIR


Jim Colvin Consulting Services


Ron Potok, Advanced Micro Devices  Liang Wang, Advanced Micro Devices


SYSTEM LEVEL ANALYSIS AND TEST


MIKE LANE, CHAIR  Intel Corporation


YIELD ENHANCEMENT


CAROL BOYE, CHAIR  IBM Corporation


Yi Feng, IBM


Alfredo Herrera, Spansion LLC


ISTFA/2008


November 2-6, 2008


Oregon Convention Center Portland, Oregon USA


Participate in the premier event for the


microelectronics failure analysis community.


• Original, unpublished, and novel material is


solicited on testing, analysis, characterization,


and metrology of electronic devices and


systems from nanoscale to macroscale.


• Case studies, review papers, and noncommercial work from vendors are also


encouraged.


• Technical symposia, user groups, seminars, short


courses, and the largest equipment exposition in


the industry make ISTFA the best place to learn,


network, and accelerate your career!


For more information and to submit your abstract, visit the web at www.istfa.org.


Abstract Submisson Deadline:  March 31, 2008.


EDFAS 2007 Photo Contest • 1st Place: False Color Images


EBIC image of an analog device showing emitter leakage on an NPN  transistor. – Rafael Huerta and Zachary Gemmill


ASM


INTERIVATIONA


®


The Materials


Information Society


EDFAS34th International Symposium


Electronic Device Failure Analysis Society An Affiliate Society of ASM International®


for Testing and Failure Analysis™


2008 FIRST ANNOUNCEMENT AND CALL FOR PAPERS


ix


Contents


Session 1: Emerging Concepts


Integrated Raman – IR Thermography for Reliability and Performance


Optimization and Failure Analysis of Electronic Devices ......................................................1


M. Kuball1, A. Sarua1, J.W. Pomeroy1, A. Falk2, G. Albright2, M.J. Uren3, T. Martin3,


(1) H.H. Wills Physical Laboratory, Briston, United Kingdom; (2) Quantum Focus Instruments,


Vista, CA, USA; (3) QinetiQ Ltd., United Kingdom


Reduction of Acquisition Time for RIL, SDL, and LADA........................................................6


A. Mels, F. Zachariasse,


NXP Semiconductors, Nijmegen, The Netherlands


A New Approach for SRAM Soft Defect Root Cause Identification.....................................14


P. Egger1, Stefan Müller1, M. Stiftinger2,


(1) Infineon Technologies, Munich Germany; (2) Infineon Technologies, Neubiberg, Germany


3-D Defect Localization by Measurement and Modeling of the Dynamics of Heat


Transport in Deep Sub-Micron Devices.................................................................................20


A. Reverdy1, M. de la Bardonnie1, L.F.Tz. Kwakman1, M. Lamy2, C. Wyon3,


A. Doukkali4, H. Murray4, P. Perdu5,


(1) NXP Semiconductors, Crolles, France; (2) STMicroelectronics, Crolles, France;


(3) CEA-LETI/Minatec, Grenoble, France; (4) Laboratoire de Microélectronique ENSI-Caen Philips,  Caen, France; (5) CNES, Toulouse, France


Session 2: Circuit Edit 1


Effects of Backside Circuit Edit on Transistor Characteristics...........................................29


R.K. Jain1, T. Malik1, T.R. Lundquist1, Q.S. Wang1, R. Schlangen2, U. Kerst2, C. Boit2,


(1) Credence Systems Corp., Sunnyvale, CA, USA;


(2) Berlin University of Technology, Berlin, Germany


FIB Backside Circuit Modification at the Device Level, Allowing Access to


Every Circuit Node with Minimum Impact on Device Performance by Use of


Atomic Force Probing .............................................................................................................34


R. Schlangen1, U. Kerst1, C. Boit1, S. Schömann2, B. Krüger2,


R. Jain3, T. Malik3, T. Lundquist3,


(1) Berlin University of Technology, Berlin, Germany;


(2) Infineon Technologies, Munich, Germany; (3) Credence DCG, Sunnyvale, CA, USA


Deposition of Narrow, High Quality, Closely Spaced, but Isolated Conductors................41


V.V. Makarov, R.K. Jain,


Credence Systems Corp., Milpitas, CA, USA


x


Session 3: SPM Techniques


Challenges of Atomic Force Probe Characterization of Logic Based Embedded


DRAM for On-Processor Applications .................................................................................. 46


T. Kane1, M.P. Tenney1, A. Erickson2, S. Phan2,


(1) IBM Systems and Technology Group, Hopewell Junction, NY, USA;


(2) Multiprobe, Inc., Santa Barbara, CA, USA


Alternating Plane-View and Cross-Section Scanning Capacitance Microscope


Technique to Reveal Various Implant Issue ......................................................................... 52


T.-C. Chuang, C.-M. Shen, S.-C. Lin, C.-M. Huang, J.-H. Chou, J.C. Lee, Taiwan Semiconductor Manfacture Company, Ltd, Taiwan


Sub-Zeptofarad Sensitivity Scanning Capacitance Microscopy Sensor ........................... 56


H. Dongmo, P. Hammond, J. Weaver,


University of Glasgow, Glasgow, United Kingdom


Session 4: Sample Preparation


Backside 3-D Analysis of Power Device Using an ITO Electrode....................................... 61


Y. Goto,


Toyota Motor Corp., Aichi, Japan


Re-Thin a TEM Lamella by Using a Novel TEM Sample Preparation.................................. 67


C.R. Chen,


Material Science Service Corp., Taiwan


Applications for Parallel Grinding as an Alternative to Chemical Decapsulation


in Preparing Packaged Samples for Failure Analysis ......................................................... 71


C. Nail,


National Semiconductor Corporation, Sana Clara, CA, USA


Session 5: Photon Based Techniques


Three-Dimensional Nanometric Sub-Surface Imaging of a Silicon Flip-Chip Using


the Two-Photon Optical Beam Induced Current Method..................................................... 77


E. Ramsay, K.A. Serrels, M.J. Thomson, A.J. Waddie, R.J. Warburton,  M.R. Taghizadeh, D.T. Reid,


Heriot-Watt University, Edinburgh, United Kingdom


Near-IR Photon Emission Spectroscopy on Strained and Unstrained


60 nm Silicon nMOSFETs....................................................................................................... 81


S.L. Tan1, K.W. Ang2, K.H. Toh1, D. Isakov1, C.M. Chua3, L.S. Koh3, Y.C. Yeo2,


D.S.H. Chan1, J.C.H. Phang1,3,


(1) Centre for Integrated Circuit Failure Analysis and Reliability, Singapore;


(2) Silicon Nano Device Laboratory, Singapore; (3) SEMICAPS Pte Ltd., Singapore


xi


Failure Localization & Design Debug on Mixed-Mode ICs by Using the


Dynamic Laser Stimulation Techniques................................................................................86


M. Sienkiewicz1,2, K. Sanchez1, A. Firiti2, O. Crepel2, P. Perdu1, D. Lewis3,


(1) CNES, Toulouse, France; (2) Freescale Semiconductor, Toulouse, France;


(3) IMS, Talence, France


Session 6: In-Line Metrology and Inspection


Real-Time FTIR Etch Depth Measurements in Passive Integrated Silicon Substrates......93


F. Roullier1, B. Domengès1, P. Poirier1, J.P. Blanvillain2,


(1) LAMIPS, Caen, France; (2) NXP Semiconductors, Caen, France


Blind Deconvolution of SEM Images .....................................................................................97


W.E. Vanderlinde1, J.N. Caron2,


(1) Laboratory for Physical Sciences, College Park MD, USA;


(2) Research Support Instruments, Lanham, MD, USA


Nondestructive Defect Imaging through Image Intensity Analysis...................................103


J. Demarest, D. Bearup, A. Dalton, L. Hahn, B. Redder, F. Wallingford, IBM, Hopewell Junction, NY, USA


Automated TEM Sample Preparation on Wafer Level for


Metrology and Process Control ..........................................................................................107


B. Rijpers1, D. Verkleij2, E. Langer3,


(1) CD Metrology, Veldhoven, The Netherlands; (2) NanoElectronics Business Group,


Eindhoven, The Netherlands; (3) AMD, Dresden, Germany


Applications of Electron Tomography on Advanced DRAM .............................................115


J.-S. Luo, J.D. Russell, L.-Y. Huang, T.-P. Chen,


Inotera Memories, Inc., Taoyuan, Taiwan


Session 7: Package and Assembly Level FA 1


Al Pad Corrosion Mechanism Study When Dicing Saw .....................................................121


S. Duan, M. Li, Q. Yu, J. Su, S. Lin, C. Niou, W.T.K. Chien,


Semiconductor Manufacturing International Corp. Shanghai, China


Effect of Inter-Die Adhesive Profile on the Integrity of Die Surface in


Die Stacking Package............................................................................................................126


C.C. Flores, F.B. Aspera,


Intel Technology Philippines, Inc., Cavite, Philippines


Effect of Die Chip-Outs and Reflow Temperature on the Mechanical


Behavior of a 5-Die-Stacked Chip Scale Package ..............................................................130


D. Evan, L. Balacano, L.P. De La Rama


xii


Study of FBGA Burn Failure under THB Test..................................................................... 134


J. Zhou, W. Zheng, M. Lou, N. Feng, J. Lee, T. Lee,


Samsung Semiconductor China R&D Co. Ltd., Suzhou, China


A New Methodology for Electrical Debugging Short in Packages with the


Modified Daisy-Chain Die ..................................................................................................... 140


S.K. Hsiung, K.V. Tan, J. Soopikian,


LSI Logic Corporation, Fremont, CA, USA


Session 8: Posters


Study of a Systematic Low DPPM Reliability Defect without


Common Electrical Signature .............................................................................................. 146


F. Zhang,


Texas Instruments Inc., Dallas, TX, USA


Laser Assisted Lock-In Phase & Spectral Analysis Techniques at Advanced


IC Failure Analysis with Application to Jitter and Soft-Defects........................................ 151


C. Brillert, Z. Qian, C. Burmer,


Infineon Technologies AG, Munich, Germany


Localization of Cu/Low-k Interconnect Reliability Defects by


Pulsed Laser Induced Technique ........................................................................................ 156


T.L. Tan1, A.C.T. Quah2, C.L. Gan1, J.C.H. Phang2,3, C.M. Chua3, C.M. Ng4, A.-Y. Du5,


(1) Nanyang Technological University, Singapore; (2) Centre for Integrated Circuit


Failure Analysis and Reliability, Singapore; (3) SEMICAPS Pte Ltd., Singapore;


(4) Chartered Semiconductor Manufacturing Ltd., Singapore;


(5) Institute of Microelectronics, Singapore


Ultra Low Voltage Probing on 45 nm CMOS by Time Resolved


Emission (TRE) Technology ................................................................................................ 161


C.-L. Young1, P. Ng1, F. Contreras1, R. Ispasoiu2, J. Vickers2, D. Cotton2, C. Shaw2,


(1) Intel Corporation, Santa Clara, CA, USA;


(2) Credence Corporation, Sunnyvale, CA, USA


Masking Technique to Enable Multiple Site Defect Analysis on a Microchip.................. 165


J. Hahn,


Altera Corporation, San Jose, CA, USA


Ion Beam Imaging Methodology of Invisible Metal under Insulator Using


High Energy Electron Beam Charging ................................................................................ 168


C.H. Wang, S.P. Chang, C.F. Chang, J.Y. Chiou,


Taiwan Semiconductor Manufacture Company, Ltd., Taiwan


A Case Study of Defects Due to Process-Design Interaction in


Nano Scale Technology........................................................................................................ 172


J.-S. Lin, Y.-C. Hou, J. Fu, M.-S. Wu, V. Huang, C.-H. Chou, J.-C. Lin, United Microelectronics Corporation, Ltd., Taiwan


xiii


STI Punch-through Degradation Related Standby Current Failure in


HTOL Test – A Case Study ...................................................................................................176


W.-R. Chen, W.-C. Tseng, Y.-J. Lee, K.-W. Liu, L.-K. Kuo, S. Yin, C.-Y. Lu,


Macronix International Co., Ltd., Hsinchu, Taiwan


Bevel Etching: A Low Cost Alternative to FIB ....................................................................180


B. Seidl, J. Walter, M. Kirchberger,


Infineon Technologies AG, Regensburg, Germany


Cross-Sectional Sample Preparation Techniques for 2-D Doping


Profiling of Specific Site by SCM .........................................................................................185


T.-K. Lee, T.-S. Back, J.-H. Kim, Y.-B. Park, H.-J. Kim, S.-Y. Lee,


Hynix Semiconductor Inc., Kyoungki-do, Korea


The Failure Site Localization Using Absorbed Current Image and


Voltage Distribution Contrast...............................................................................................188


T. Nokuo1, Y. Eto1, Z. Marek2,


(1) JEOL Ltd., Tokyo, Japan; (2) JEOL USA, Inc., Peabody, MA, USA


A Simple Adapter for Soft Defect Localization Using OBIRCH .........................................191


T. Kolasa,


Freescale Semiconductor, Inc., Tempe, AZ, USA


Session 9: Package and Assembly Level FA 2


Studies of Galvanic Corrosion (Al-Ti Cell) on Microchip Al Bondpads


and Elimination Solutions.....................................................................................................193


H. Younan1, M. Zhiqiang1, Z. Siping1, G. Hao2,


(1) Chartered Semiconductor Mfg. Ltd., Singapore;


(2) National University of Singapore, Singapore


Construction of a 3-D Current Path Using Magnetic Current Imaging..............................197


F. Felt1, L. Knauss2, A. Gilbertson2, A. Orozco2,


(1) NASA Goddard Space Flight Center, Greenbelt, MD, USA; (2) Neocera, Beltsville, MD, USA


Investigation of Bond-Pad Etching Chemistries for Determination of


Probe/Bonding Related Sub-Pad Cracks.............................................................................206


V. Korchnoy,


Intel Israel, Haifa, Israel


Session 10: Nanoprobing


Investigation on the Influence of Focused Electron Beam on Electrical


Characteristics of Integrated Devices..................................................................................210


S. Doering, R. Harzer, W. Werner,


Qimonda Dresden GmbH & Co. OHG, Dresden, Germany


xiv


Combining the Nano-Probing Technique with Mathematics to Model and


Identify Non-Visual Failures................................................................................................. 214


C.-M. Shen, T.-C. Chuang, S.-C. Lin, L.-F. Wen, C.-M. Huang, Taiwan Semiconductor Manufacture Company, Ltd., Taiwan


Analysis of DC Failure in Advanced Memory Devices Using Nanoprobing and


Scanning Capacitance Microscopy..................................................................................... 219


J.-L. Lue, C.-S. Lin, A. Chiou, H.-C. Liao, H. Liu, B. Pai, S. Fan, T. Wang,


ProMOS Technologies Inc., Hsinchu, Taiwan


Measuring Static Noise Margin of 65 nm Node SRAMs Using a 7-Point SEM


Nanoprobing Technique....................................................................................................... 223


R.E. Stallcup1, Z. Cross1, W. James2, P. Ngo2,


(1) Zyvex Instruments L.L.C., Richardson, TX, USA;


(2) Microtech Analytical Labs, Plano, TX, USA


Session 11: Package and Assembly Level FA 3


Localized Die Metallization Damage Induced During Laser-Marking of a


Semiconductor Package ...................................................................................................... 226


P.E.B. Parañal,


A Novel Technique for Determining the Location of a Hermetic Leak in a


‘Metal Can’ (TO-x) Package .................................................................................................. 231


National Semiconductor Corporation, Santa Clara, CA, USA


BGA Package Level Failures Due to Contamination ......................................................... 236


J. Roepsch,


Raytheon, McKinney, TX, USA


Session 12: Failure Analysis Process 1


Failure Analysis Methodology for Li-Ion Incidents ............................................................ 242


J. Loud, X. Hu,


Exponent Inc., Menlo Park, CA, USA


Case Study and Fault Modeling for Wrong Redundancy Evaluation on


DRAM Devices....................................................................................................................... 252


M. Versen1, D. Diaconescu2, J. Touzel2,


(1) Qimonda AG, Neibiberg, Germany; (2) Infineon AG, München, Germany


Fault Isolation of Soft P-N Junction Break Down Due to Plasma Charging .................... 257


D. Nguyen, T. Dudar,


xv


Session 13: Yield Enhancement


Tool-Related ESD Surface Damage (ESDFOS) on Wafers in Cu-Technology ..................262


P. Jacob1, C. Hartfield2,


(1) Empa Swiss Federal Laboratories for Materials Testing and Research,  Duebendorf, Switzerland; (2) Texas Instruments, Dallas, TX, USA


Detection and Verification of Silicide Pipe Defects on SOI Technology Using


Voltage Contrast Inspection .................................................................................................270


O.D. Patterson1, H.H. Kang1, J. Strane1, C. Lovoie1, K. Barth1, X. Ouyang1, K. Wu2,


(1) IBM, Hopewell Junction, NY, USA; (2) KLA-Tencor, Hopewell Junction, NY, USA


Photo Process Margin Leading to IC Failure – A Case Study ...........................................275


V. Chowdhury, C. Hsu, A. Yu,


Failure Analysis of Multi-Fingered HV Symmetric Devices for


Charge-Pumping Circuit Applications.................................................................................280


L.-F. Wen, T.-C. Wang, C.-H. Chen,


Taiwan Semiconductor Manufacturing Company, Ltd., Hsinchu Taiwan


Voiding in Cu Technology through Photovoltaic-Driven


Electrochemical Dissolution.................................................................................................284


F.A. Baiocchi, J. DeLucca, J.T. Cargo,


LSI Corporation, Allentown, PA, USA


(1)


Laser Stimulation


By shining a laser onto the chip (from the back side) at a critical node, one is able to shift the timing of the circuit. Rowlette & Eiles [3] showed that there is in principle no threshold in  the laser power needed to shift the timing in a circuit, but that  the magnitude of the timing shift is related to the laser power  used.


Therefore, the laser is at least able to shift the timing by a  small amount, and this moves the threshold for pass / fail. However, the jitter remains, and hence the net effect is to have  shifted the entire normal distribution somewhat compared to  the case where the laser is not present or not hitting the critical  node. This situation is illustrated in Fig. 1. Along the x-axis a  relevant timing parameter is plotted. The probability that a test  will fail, on the y-axis, can be seen to vary smoothly from  100% to 0% as the timing parameter is varied.


For a given timing, the shifting of the distribution by laser  stimulation will cause the probability of the failure to change. Therefore the actual signal that is observed is the difference in  probabilities (see Fig. 1).


Sample Point (in AU)


Figure 1: Unshifted and shifted cumulative probability distribution of the chance of failing a particular test as function of  timing.


We have obtained experimental probability plots for various  different structures and tests and the Gaussian distribution is  indeed a reasonable model for fitting purposes.


For example, in Fig. 2, experimental results taken on a ring  oscillator both with and without laser illumination are shown. Also shown is the fitting with the Gaussian model of Eq. 1. This curve fitting yielded a timing shift of 7.5ps due to the  laser illumination. The spread, σ, of the Gaussian was 28ps for  both curves.


Although in the above explanation, we discuss targeting the  laser specifically at a known node, and measuring the time  shift, in practice, the laser will be scanned across the chip in  an attempt to localise those ‘spots’ that are actually sensitive  to the laser influence. The probability measurements at each (X,Y) location of the laser are combined into an image.


If the LADA image were a true reflection of the pass/fail  probability at each point on the screen, then it would be easy  l00%


to identify all spots. However we can only measure this probability by repeating the test a number of times. The estimated


Probability of Failure20%409%


signal strength


90%


observed


80%


probability is then the average number of times the test failed. The more often the IC is tested under identical conditions (i.e. with the laser pointed to the same spot), the more accurate (less noisy) the measurement of the probability will be. It does  not make a difference if the averaging is done by doing the


shift due


tests one after another (for example inside the tester) or on an


to laser


image-by-image basis (on the laser scan system).


laser offlaser on


So both the background and the spots will contain a certain


-4-2024


amount of noise. To be able to distinguish a spot from the  background, the signal has to be strong enough to rise significantly above the background noise level.


Image quality measure


Before we can determine whether a signal is actually detectable, we must establish a suitable measure for the image quality. A commonly employed measure is the Signal-to-Noise  Ratio (SNR) of an image (also more accurately known as Signal-to-Background Ratio). If S is the mean of the pixel values  inside the spot, B is the mean of the pixels outside the spot (the background) and σB the standard deviation of the background pixels, then the SNR can be defined as:


B


S


SNRσ−=


(2)


For certain applications like photoemission this gives a reasonable figure for image quality. However, an issue that effects our investigations into LADA is that the noise inside the  spot may contribute to the difficulty of distinguishing that spot  from the background and that the statistics of LADA are not  the same as those that apply to photoemission.


Compare for example simulated images A and B in Fig. 3: they both have a spot in the centre, which has the same SNR  according to the definition of Eq. 2. However the spot in image A is clearly visible, whereas the spot in image B is barely  discernible.


100%90%


/ Laser Off


- Laser On


An improvement to this image quality measure can be made


-Fitted with equation 1


by including the noise in the spot, σS, in the definition of sig70%


nal to noise ratio, like


60%


2


50%


SNR


40%


σ


σ +−


=


.


(3)


30% FailureProbability of20%


Now compare simulated images B and C in Fig. 3: they again


10%


both have a spot in the centre, but this time the SNR is the


0%


2****


same according to the definition of Eq. 3.


70.570.5570.670.6570.770.75


For LADA the definition of Eq. 3 is a better measure of image


Sample point (in ns)


quality and we will be using this definition throughout the rest  of this paper. The SNR according to this definition needs to be  roughly 1 for a spot to be well recognizable.


Figure 2: Actual distribution of ring oscillator structure fitted  with the cumulative probability distribution of a gaussian distribution


Signal-to-noise analysis


It is now possible to derive a theoretical model for the image  quality based on the spread on the probability distribution and  the shift introduced by the laser. Here we assume that the laser  is scanned in such a way that we record at each pixel, the result of N tests of the chip. Each test has a certain probability  of passing, p, and of failing, (1-p). The signal at each pixel  follows the binominal distribution. Therefore the expected  value of a pixel is


Np


E =


(4) and the standard deviation of each pixel value, σpixel, is given  by


)


1(


p


N


pixel −⋅=σ .


(5) If the probability of the test passing is ps inside the spot and pb  outside the spot, then the signal-to-noise ratio, SNR, following  Eq. 3, becomes


( )


( ) ( )BBS


−


+


+−


1


2 2 σσ


(6)


The Gaussian model of Eq. 1 for the probabilities ps and pb  can now be applied to this equation. For convenience, we will  normalize the distribution so that the mean (50% point) is at 0  and the spread is 1. The normalized sample point, t, becomes


σμ


=x


t


(7)


Stage 1


s1e6a£


se6oz


Average


DeviatiorStandard


and, if the time shift introduced by the laser is called xS, then  the normalized shift, s, becomes


S x


(


(8)


Using this normalized sample point and normalised shift to  estimate the probabilities gives


( )( )t


B S


Φ


(9)


The expression for the signal-to-noise ratio now becomes


( ) ( )


( ) ( )( ) ( ) ( )( )ttstst


⋅


(10)


An important point that arises from these equations is that it is  actually the ratio between shift and jitter that determines the  SNR. This implies that a 2ns shift with 2ns jitter would be  equivalent to having 30ps shift with 30ps jitter.


With Eq. 10 it becomes possible to estimate the expected image quality if the jitter and the shift are known. Take for example the ring oscillator of which the histograms are presented in Fig. 2. We also made a laser scan image of this device. Figure 4 shows a part of the image with three stages of  the ring oscillator visible.


Signal 46% 3%Noise 26% 4%SNR


4.1


Figure 4: LADA image of a ring oscillator integrated for 1024  frames with SNR calculation


A


C


SNR (eq 2): 3.1  SNR (eq 3): 2.2


SNR (eq 2): 3.1  SNR (eq 3): 0.7


SNR (eq 2): 0.9  SNR (eq 3): 0.7


Figure 3: Simulated images showing a comparison between the SNR figures of Eq. 1 and Eq. 2.


For each pixel 1024 tests were executed and the tester was set


Normalized Sample Point


so the sample point was at 70.637ns. This is 15ps from the  50% point. So with a spread of 28ps the normalized sample


point, t, becomes 0.54 and the shift of 7.5ps becomes a normalized shift, s, of 0.27. Filling in these figures into Eq. 10


gives an estimated SNR of 4.7.


To calculate the SNR from the image, the average values and


-4-2


24


standard deviations of the signals inside the spot and outside


Normalized


the spot were measured from the image and used with Eq. 3.


-1


Shift


The SNR when calculated from the image is 4.1, which is in  reasonable agreement with the theoretical value.


-2


Application of the model


Sample point selection


So the signal-to-noise ratio for LADA images is now reduced  to a function of three variables that can be influenced: the  sample point, t, the number of averages, N, and the shift introduced by the laser, s.


From the Fig. 1 it can be seen that there must be an optimum  sample point: if one would set the sample point too far to the  left (for example at –2) then the device will always fail, if one


would set it to far to the right (for example at +3) it would


2Optimal


always pass; so somewhere in between there should be an


1.5Sample Point


optimum (at approximately +0.5). This is illustrated in Fig. 5: for various shifts the SNR is calculated as a function of the


sample point.


0.5


Sample Point at 50% pass/fail


SNR1.5s=+2


-4-3-2-11234-0.5


s=+1


-1.5


Figure 5: Signal-to-Noise ratio as function of sample point for  different shifts with N=1


Figure 5 shows that the optimal sample point is somewhere  near half of the shift. Figure 6 shows the exact relation of the  optimal sample point as function of the shift. To optimise the  SNR the sample point should be selected according to this  curve, however when one starts with an analysis it is not yet  known how large the shift will be (or even the direction of the  shift). Therefore it is more practical to start out exactly at the  50% pass/fail point.


Figure 6: Optimum sample point as function of shift


The SNR obtained using both the optimal sample point and  the 50% pass/fail point are shown in Fig. 7 as function of the  shift. For small shifts (say below 1) the difference in SNR is  negligible, so the 50% point is a good choice. For larger shifts  it starts to make increasingly more difference. However, for  such strong signals, a high enough SNR is reached within 1 or  2 integrations anyway, so this is not important for practical  purposes.


-5


-2-101345


Figure 7: SNR in optimum sample point versus in 50% point


-0.5


s=-1


Sample Point


with N=1


Figure 7 also shows that for these small shifts the SNR ins=-2


creases almost linearly with the shift. In this regime Eq. 10  can be approximated by using a first order Taylor expansion:


π


SNR ≈


(11)


The number of integrations


The relation of the SNR to the number of integrations, N, is  clear from Eq. 10: it improves as just the square root of the  number of integrated samples. This means that the number of  tests N needed to distinguish the signal from the noise grows  rapidly as the signal gets weaker (see Fig. 8).


Figure 8: The number of tests to reach SNR = 1


If a certain image quality is desired, SNRDesired, then the number of times the test needs to be executed per pixel, NTests, can  be expressed as function of the SNR of a single test, SNRSingle  Test, like


Test


Single


Desired


⎟⎟⎠⎞


⎜⎜⎝⎛


=SNRSNR


N s


(12)


The actual integration (or averaging) can be done in the laser  scanning equipment, but can also be done inside the test system. The latter might allow for a faster repeat of the test by  utilizing test system features like error counts.


Acquisition time


The total time needed for the acquisition of the image can now  be expressed as function of the time needed for each test, TTest, the number of pixels in an image, NPixels, and a the number of  tests per pixel, NTests, like


Pixels


Tests


Per


n


Acquisitio


T


(13) If we use Eq. 11 to approximate the SNR of a single test, the


06


1 bit


acquisition time needed to obtain an image with a certain SNR  can be simplified to


8 bits


Probability of  Pass/ Fails


≈ π


(14) S


This means that the acquisition time increases linearly with an


increase in the number of pixels or the time per test, but decreases quadratically with an increase in shift.


As an example: to make a LADA image of 256x256 pixels  with a single test per pixel of 1ms will already take 65 seconds  per image. So in 10 minutes you could acquire almost 10 integrations. This means that you could detect a signal (SNRDesired=1) if the laser induces a normalised shift of approximately


0.6. So with a jitter of 100ps you would need at minimum  60ps shift to be able to detect a change within this time. Now  say the jitter was 200ps and the shift only 30ps. Then it would  already take more than 2½ hours to acquire the desired image.


10000


Testing multiple paths simultaneously


Before going into a discussion on how to reduce the acquisition time further, we will consider testing multiple paths in the


1000


same test. This would be the case, for example, when investigating a speed problem on the data path of a microprocessor:


100


If it was not known which bit on the data path was responsible  for the problem, it would be tempting to perform LADA by  using a pass/fail signal derived from testing the entire 32 bits


ofNr samples10


Sample Point at


of a calculation result.  In this way, laser scanning could be


Optimal


50% pass/fail


done without having to investigate the problem too deeply


beforehand.  However, as we show below, this approach can


0.511.522.53


cause a significant reduction in the signal to noise ratio.


Normalized Shift


What you are actually doing in this case is taking the results of  the individual paths together: the overall test will only pass if  all paths pass. If the noise in the paths is uncorrelated the  overall pass probability is obtained by multiplying the pass  probabilities of the individual bits. Only the probability curve  of the bit that is illuminated by the laser will actually be  shifted. In case b individual paths contribute to the test result  and the delays of all these paths are equal, the probabilities  become


( ) ( )( )( )b


b


−1


(15)


Figure 9 shows the effect for 8 bits. The curves get steeper (less jitter), however the shift decreases even more. Also shifts  in the one direction give a stronger signal than in the other: if  you speed up one path another path will become the slowest  path. The impact on the SNR is visible in Fig. 10.


Figure 9: probability distributions for testing 1 bit and 8 bits  simultaneously with -1, 0 and +1 shift on 1 bit


What was considered so far is the worst case scenario: all  paths have exactly the same delay. In real world problems one  is looking for the critical path, implying that all other paths are  faster. However if the difference in speed of these paths is in  the same order of magnitude as the shift that can be introduced, the decrease in SNR is still significant (see Fig. 10).


Figure 10: SNR when testing multiple bits simultaneously, with a delay of 0 between the paths and a delay of 1


For example with 8 bits and a normalized shift of -0.5 you  will need to integrate approximately 12 times longer to obtain  the same image quality; with 32 bits this even becomes more  than 85 times longer. When the other paths are faster, for example by one normalized unit, the increase in acquisition time  will still be more than a factor of 6 for the 32 bits case.


As it is usually not known beforehand what the various delays  are and what the expected direction of the shift introduced by  the laser is, you should not test more than one path simultaneously. Otherwise a considerable increase in acquisition  time can result.


Further reducing acquisition time


Besides choosing the optimal sample point and avoiding the  testing of multiple paths in the same test, there are a number  of other ways to improve the image quality.


0.2


4.5


Increasing laser power


s u


0.18


4


It is clear from Eq. 14 that increasing the shift is the most ef-u!)0.16


3.5


fective way to decrease the acquisition time. The most obvi-p0.14


Normalized Shift-3


ous solution to increasing the shift is increasing the laser a0.12


2.5


e


power. Our measurements on a ring oscillator circuit show dS0.1that the induced delay is linear with laser power (see Fig. 11). Y!


u


S0.06


1.5


0.08


Similar results were obtained by Rowlette and Eiles [3].


Therefore an increase in laser power gives rise to a quadratic


0.751 bit


decrease in the necessary acquisition time for weak signals.


8 bits delay = 1 AU


There is of course an upper limit to how much the laser power


0.25


can be increased before the device is damaged. Kong & Cas8 bits delay = 0 AU


tro [4] measured these damage thresholds for certain proc-


-224


esses.


Decreasing jitter


Another option is to decrease the jitter. Since the equation for


-0.75


SNR is written in terms of normalised shift (actual shift divided by jitter), reducing the jitter is just as effective in improving SNR as increasing the shift.


The jitter is caused by the measurement equipment, the measurement setup and also by the device itself. If the proper  measurement equipment is used the last two sources should be  dominant.


Altering the supply voltage


In the context of jitter reduction, we investigated the behaviour of a CMOS IC to LADA as the supply voltage is lowered. At first sight, since the currents of the MOSFETs are reduced, whilst the junction currents introduced by the laser stay the  same, one would expect stronger induced signals at lower  supply voltage. However, the jitter also increases when the  voltage is reduced. In Fig. 12 the jitter, the shift and their ratio  as function of supply voltage are displayed. For this particular  structure the normalized shift (absolute shift divided by the  jitter) improves by a factor of 2.7 when changing the supply  voltage from 1.9V to 1.0V, which gives a reduction in acquisition time of about 7 times.


Voltage (in V)


Figure 12: Shift and jitter as function over voltage for a test  structure


More complex effects are also seen. For example Fig. 13  shows that, in the ring oscillator of our previous examples, as  we change the supply voltage from 1.8V to 0.6V, the dark


Percentual change in delay time


spots become relatively stronger in their response compared to  the white spots. This means that certain transistors in a device  behave differently to a change in supply voltage than others  when it comes to LADA response.


-7%-6%-5%-4%-3%-2%-1%0%


11.21.41.61.8


10.02


1%


0


2%3%


a


山0.04Jitter


-


20.00


40.00


60.00


Laser Power (in mW out of the lens)


location of increase


location of decrease


Figure 11: Shift as function of laser power


0.06  ns)Time Shift (in0.04


0.6V


1.8V


0.02


Figure 13: Images of a ring oscillator at different voltages


0111


Adding decoupling


1.01.21.41.61.8


Besides the intrinsic jitter in the device, some additional jitter  is introduced by the measurement set-up. Possible causes include cross-talk and voltage noise.


The voltage noise can be improved by adding more decoupling capacitance external to the device. Unfortunately, this  does not necessarily improve the LADA results. Experimentally we find that the jitter indeed decreases, however at the  same time the shift introduced by the laser is also reduced. We  speculate that a dynamic voltage drop, which makes the effective operating voltage to be lower at the time of sampling. Therefore adding decoupling does not help as much as one  might assume at first.


Altering the operating temperature


Another factor we investigated is the temperature. Similarly to  what happens when changing the operating voltage, the currents in the transistors will be different at different temperatures, but the currents introduced by the laser will stay the  same.


Because doing extensive experiments at different temperatures  is very time consuming, some simulations were done on (part  of) a ring oscillator circuit (Fig. 14). The laser was modelled  by injecting a current into the drain of the nmos transistors  and into the nwell for the pmost transistors as suggested by  Rowlette and Eiles [3]. A limited number of experiments were  executed, which confirm the order of magnitudes and direction of the shifts induced by a change in temperature.


The results in Fig. 14 show that the temperature behaviour  depends strongly on the supply voltage. The direction of the  change can even be opposite at different supply voltages (as  was previously reported in [5]). The voltage where this inversion occurs is strongly process dependent. It is also clear from  fig. 14 that the effect of a change in temperature is relatively  small compared to the effect of a change in supply voltage.


This, together with the fact that it can be quite involved to  create a setup that allows the device to be heated or cooled in  a stable fashion, makes using the temperature for optimising  the acquisition time less attractive.


0.14


0.12


0C


0.1


-50C


--100C


Supply Voltage (in V)


Figure 14: Shift introduced into a ring oscillator depending  on voltage and temperature


Conclusions


Starting from the concept of the shmoo edge as a smooth transition from 100% fail to 100% pass, we have developed a  model of LADA signal strength. By combining this model  with a suitable measure for image quality, we derived equations for the acquisition time needed to discern a LADA response from the background noise.


Comparison of the model to experimental data shows that it is  indeed a realistic representation. For weak signals, we show  that the optimal condition, for minimum acquisition time, is at  the 50% pass/fail point of the shmoo plot. Under these conditions, the acquisition time decreases quadratically with an increase in laser-induced timing shift, or a decrease in jitter.


Extension of the model to the testing of multiple paths simultaneously, shows that this simultaneous testing should be  avoided, as it might strongly degrade the image quality.


We investigated a number of ways to improve the LADA response. Performing LADA at reduced supply voltages appears  to be a feasible avenue to achieve this. In some device types, it  resulted in a 7-fold reduction in acquisition time.


In conclusion the model offers a quantitative tool to estimate  the feasibility of a given LADA measurement and a guide to  optimising the required experimental set-up.


Acknowledgements


We thank our colleagues within the failure analysis department for their support, especially Bob Knoppers and Henk  Pomp for the preparation of the samples.


References


[1] M.R. Bruce, V.J. Bruce, D.H. Eppes, J. Wilcox, E.I. Cole  Jr. , P. Tangyunyong, C.F. Hawkins, “Soft Defect Localization (SDL) on ICs”, International Symposium for Testing and Failure Analysis (ISTFA), pp. 21-27, Nov., 2002.


[2] E.I. Cole Jr., P. Tangyunyong, C.F. Hawkins, M.R. Bruce, V.J. Bruce, R.M. Ring, and W.L. Chong, “Resistive Interconnection Localization”, International Symposium for Testing & Failure Analysis (ISTFA), pp. 43-50, Nov. 2001.


[3] J.A. Rowlette and T.M. Eiles , “Critical Timing Analysis  in Microprocessors Using Near-IR Laser Assisted Device  Alteration (LADA)”, International Test Conference (ITC), pp. 264-273, 2003


[4] C.L. Kong and E.P. Castro, “Application of LADA for  Post-Silicon Test Content and Diagnostic Tool Validation”, Proceedings of the 32nd International Symposium  for Testing and Failure Analysis (ISTFA), pp. 431-437, Nov. 2006


[5] R. Kumar and V. Kursun, “Impact of temperature fluctuations on circuit characteristics in 180nm and 65nm CMOS  technologies”, Proceedings of the International Symposium on Circuits and Systems (ISCAS), pp. 3858-3861, May 2006


A New Approach for SRAM Soft Defect Root Cause Identification


Peter Eggera*, Stefan Mller", Martin Stiftingerb


a) Infineon Technologies,COM BTS PFS FA2,Otto-Hahn-Ring 6,81739 Munich, Germany b)Infineon Technologies,AIM OPP ATM RI,Am Campeon 1-12,Neubiberg,Germany


* Corresponding author: peter.egger@infineon.com Tel.:++49(0)89 234-24613; Fax:++49(0)89 234 23497


Abstract


WL


With shrinking feature size of integrated circuits traditional FA techniques like SEM inspection of top down delayered devices


P1)--0P2


or cross sectioning often cannot determine the physical root


cause. Inside SRAM blocks the aggressive design rules of


transistor parameters can cause a local mismatch and therefore


a soft fail of a single SRAM cell. This paper will present a newN3


approach to identify a physical root cause with the help of


N4


nano probing and TCAD simulation to allow the wafer fab to


N1N2


implement countermeasures.


Introduction


BL


BLB


With shrinking feature size of integrated circuits the physical


Fig. 1: Schematic of 6T SRAM cell and transistor labelling


In addition to this, local transistor mismatch caused by


Session 14: System Level Analysis and Test


PCB Related Field Failures with ImAg Surface Finishes ...................................................293


A. Kurella, A. Munukutla, J.S. Lewis, Intel Corporation, Hillsboro, OR, USA


Series Capacitance in High Speed Differential Pairs –


A Failure Analysis Case Study .............................................................................................298


N. Konkol


Intel Corporation, Hillsboro, OR, USA


Concepts for In Situ Diagnostics in Analog Microelectronic Circuits ..............................301


T. Kolasa, A. Mendoza,


Wireless Advanced FA Tool (WAFT)....................................................................................306


T.F. Chee1, M. Zhang2,


(1) Intel Products Sdn Bhd, Kedah, Malaysia; (2) Intel Corporation, Hillsboro, OR, USA


xvi


Session 15: Circuit Edit 2


Low keV FIB Applications for Circuit Edit .......................................................................... 312


C. Rue1, R. Shepherd2, R. Hallstein2, R. Livengood2,


(1) FEI Company, Hillsboro, OR, USA; (2) Intel Corporation, Santa Clara, CA, USA


Using Statistical Methods to Optimize Patterning


Parameters for Tungsten Deposition .................................................................................. 319


M. DiBattista1, K. Skinner1, R. Kneedler1, L. Vasilvey1, L. Drybcak1, J. Zbranek1,


G. Hartigan2, M. Oosting2,


(1) FEI Company, Hillsboro, OR, USA; (2) FEI Company, Eindhoven, The Netherlands


Combine Micro-Probing and ORBICH to Catch Non-Recognizable


Fault in RF and Mixed-Mode Integrated Circuits................................................................ 327


C.-M. Shen, Y.-L. Chang, L.-F. Wen, T.-C. Chuang, S.-C. Lin, C.-M. Huang, J.-H. Chou, Taiwan Semiconductor Manufacture Company, Ltd, Taiwan


Session 16: Failure Analysis Process 2


Comparison of Active and Passive Voltage Contrast for Failure Localization................ 331


R. Rosenkranz, W. Werner,


Latch-Up Root Cause Analysis for New ASIC Design ....................................................... 337


W. Danielak1, W. Machado1, M. Jaffer1, S. Waldstein2, A. Jordan2, M. Sachdev, 3, D. Li3,


(1) Tundra Semiconductor Corp., Ottawa, ON, Canada; (2) Tundra Semiconductor Corp.,  South Portland, ME, USA; (3) University of Waterloo, Waterloo, ON, Canada


Analysis of Bridge Failure between PPG and LPP in Fin Cell Transistor ........................ 345


J. Lee, S.-W. Chung, S.P. Park, M.S. Chang, J.H. Lee, S.-J. Hong,  Hynix Semiconductor, Inc., Kyoungki-do, Korea


Silicon Dislocation Enhanced by Dynamic Voltage Stress ............................................... 348


Y.-C. Lin, R. Chen, S. Liang, S. Liao, C. Niou, W.T.K. Chien,


Semiconductor Manufacturing International Corp., Shanghai, China


Author Index.......................................................................................................................... 351


Integrated Raman – IR Thermography for Reliability and Performance  Optimization, and Failure Analysis of Electronic Devices


Martin Kuball, Andrei Sarua, and James W. Pomeroy


H.H. Wills Physics Laboratory, University of Bristol, Bristol BS8 1TL, United Kingdom


Aaron Falk and Grant Albright


Quantum Focus Instruments, Vista CA 92081, USA


Michael J. Uren and Trevor Martin


QinetiQ Ltd, Malvern WR14 3PS, United Kingdom


We report on the development of a novel thermography  technique, integrated Raman – IR thermography, illustrated  here on AlGaN/GaN electronic devices. As it is a generic  technique future application to Si, GaAs and other devices is  anticipated. While IR thermography can provide fast  temperature overviews, its current use for many of today’s  technologies is complicated by the fact that it does not provide  the spatial resolution needed to probe sub-micron/micron size  active device areas. Integrating IR with micro-Raman  thermography, providing temperature information with


0.5 m spatial resolution, enables unique thermal analysis of  semiconductor devices to a level not possible before. This  opens new opportunities for device performance and  reliability optimization, and failure analysis of modern  semiconductor technology, in research, development, and  quality control / manufacturing environments.


Device reliability is one of the major challenges for the  development of new technologies, for example of GaN and  SiC micro-electronics, but also for more traditional material  systems such as Si and GaAs when performance specifications  of devices such as power handling limits are increased. Although performance of a new technology can already be at  an acceptable level, there is often a lack in reliability in the  early stages of development [1], which obviously needs to be  tackled for real-life applications. Reliability is strongly  affected by device self-heating, i.e., the temperature rise in a  device induced by ohmic heat generation. Excessive device  peak temperatures can result in accelerated device aging and  often ultimately in device failure. Device failure rates can vary  up to exponentially with device temperature, dependent on  failure mechanism. Mapping of temperature in the active area  of a device is therefore not only key for the optimization of  device performance but also one important aspect to tackling  device reliability and premature device failure. However, traditional thermal imaging techniques such as IR


thermography lack the micron/sub-micron spatial resolution


[2] needed to measure accurately device peak temperature in  many of today’s electronic devices, in particular, of devices  with a small active region. For example, device heating in an  HFET occurs predominantly within a 0.5-1 μm size region  near to the gate contact. When measured using IR  thermography device temperatures are typically averaged over  a several micron size area, underestimating device peak  temperatures and therefore underestimating the probability of  device failure. Accurate knowledge of the device peak  temperature is furthermore essential for accelerated lifetime  testing. This is as detailed information on the actual junction


~0.5 μm spatial resolution, enables unique thermal analysis of


temperature is needed to extrapolate operating lifetimes from  such test data. While alternatively simulations could give  insight into device temperatures for this and other purposes, they typically exhibit a non-quantifiable margin of error, since  there are typically uncertainties in material parameters such as  in thermal conductivities and/or thermal boundary resistances. Unless validated experimentally, their accuracy is uncertain. There is a clear need for a new alternative thermography  technique beyond IR thermography, to enable accurate  thermal assessment of devices with sub-micron/micron spatial  resolution.


Recently Bristol University has shown micro-Raman  spectroscopy to be a suitable technique to measure electronic  device temperature with sub-micron/micron spatial resolution [3-6], including its use for validation of thermal simulations


[4]. In this contribution, we report on the integration of this  novel thermography technique into traditional IR  thermography. This new approach benefits from combining  the strengths of both techniques, i.e., the ability of IR to  provide quick large area temperature overviews of devices and  to identify thermal areas of interest, and the high spatial  resolution capability of Raman. While we demonstrate here  this new technique on the example of AlGaN/GaN electronic  devices due to their current sizable reliability issues, this  technique is generic and applications to other device systems  such as Si and GaAs are anticipated and will be explored in  future research. The here developed generic approach opens  new opportunities for device performance and reliability  optimization, and for device failure analysis.


Experimental details


A Raman microscope was used to perform micro-Raman  temperature measurements on electronic devices. This Raman  thermography technique is based on the analysis of phonon  energies, i.e., the energy of lattice vibrations, which are  dependent on temperature [3,5]. Measuring changes in phonon  energy induced by dissipating power in a device, i.e., by  device self-heating, is used to deduce temperature rise in the  active area of a device. A 50× (NA=0.55) objective lens with  working distance of 10 mm was used to focus the laser  beam, used to excite the Raman signal, onto the sample  surface into a spot size of about 0.5 m diameter, which is the  spatial resolution of the temperature measurement. Temperature accuracy was better than  5 – 10 C. More  details on Raman spectroscopy and the experimental setup can  be found in Ref. [3,5,7]. The Raman system was integrated  with a LN2-cooled 256×256 InSb detector array to allow  Raman and IR thermography analysis of same device areas. IR radiation was collected using a SiGe 15× (NA = 0.5) objective, with working distance of 16 mm. Pixel resolution  with working distance of ~16 mm. Pixel resolution of the infrared image is ~1.6 um giving a total field of view ofof the infrared image is 1.6 μm giving a total field of view of ~ 410 um x 410 μm. Thermal probing both of devices on 410 μm × 410 μm. Thermal probing both of devices on  wafer operated using micro-probers and of fully packaged  devices is possible using the developed integrated Raman – IR  thermography system.


Device self-heating was studied on the example of  AlGaN/GaN HFETs and ungated devices. The HFETs had a  source-drain gap of 4.8 μm and gate length of 1.2 μm,  250 μm fingers, and the ungated devices had 20 μm openings  between the contacts and were 150 μm wide. Devices with  narrower source drain openings and shorter gate lengths can


26.555.98531146


also be investigated using the here used thermal assessment


Temperatane (C)


approach [3,4]. The metalorganic vapor phase epitaxially


grown structure consisted of 30 nm of undoped Al0.25Ga0.75N Figure 1: Temperature map of a two finger 2x50 μm on 1.2 μm of undoped, insulating GaN deposited on a doublesided polished insulating 410 m thick 4H-SiC substrate.


Standard ohmic and Schottky contacts were employed. The


devices were mounted using a high thermal conductivity


epoxy on a well heat-sunk carrier. For the thermal analysis


presented here the devices were operated under DC bias.


6


Predominantly either the GaN E2 phonon, or the SiC E2(PO) phonon was analyzed in Raman thermography to determine  temperature.


8


We note that to avoid local heating of the device by the


probing laser beam during the Raman measurement, a sub1 6


bandgap laser excitation of 488 nm was used, i.e., there is no  significant absorption of the laser light in the device. Other  laser sources such as 532 nm could also be used, and even  above band gap lasers, however, the latter would only be  suitable if low laser powers are employed. Measured  temperatures correspond to device temperatures averaged over  the Raman probing depth of typically  1 – 2 μm in the  confocal microscope used, or over the thickness of the  semiconductor layer probed, whichever is smaller. Note that  each semiconductor has its characteristic phonon modes, i.e., in a layered device structure each individual layer and


consequently layer temperature can be probed selectively. In  Raman thermography temperature can only be accessed in  device areas where the semiconductor is exposed in between  the metal contacts, or alternatively temperature can be probed  by focusing the laser beam from the back of the chip through  the substrate onto the device.


Results and discussion


A temperature map of the two finger AlGaN/GaN HFET


working distance of ~10 mm was used to focus the laser


obtained by IR thermography is shown in Figure 1, with only  one of the two fingers operated. There is a hot spot in the


surface into a spot size of about 0.5 um diameter, which is the


vicinity of the operating finger as expected, while temperature  away from this heat generating region is decreasing due to


Temperature accuracy was better than ~ 5 - 10 °C. More


thermal diffusion. There is some artificial temperature contrast  away from the active device area with some areas showing  device temperatures as low as room temperature, which will  be discussed later. Figure 2 shows an IR linescan through the  center of the active device region illustrating that peak


Figure 1: Temperature map of a two finger 250 μm  AlGaN/GaN HFET, recorded using IR thermography through


sided polished insulating 410 um thick 4H-SiC substrate.


the back of the chip. Only the right hand finger of the device was operated, at 1 W.


2x50 um fingers, and the ungated devices had 20 um openings


50μm50m


40


35


30


25


60 80


d uI100 n120


140 160 180


source


drain8


IR


0 Raman  3D sim.


Position (μm)Position (m)


Figure  2: Temperature linescan through the center of the


the Raman probing depth of typically ~ 1 - 2 um in the


active finger of the AlGaN/GaN HFET of Figure 1, with the  finger operated a 1 W, recorded using IR and Raman  thermograph through the back of the chip. Corresponding  data can be recorded from the device top. For comparison  three dimensional finite difference simulation data are shown.


temperature occurs in the source-drain gap of the device. Linescan results of the Raman thermal measurements are also  displayed in Figure 2. Note both the Raman and IR data in  Figure 2 were recorded through the back of the chip to enable  a comprehensive comparison between Raman and IR data, to  assess not only temperature in the active area but also in areas  underneath the metal contacts. Corresponding data can be  recorded from the device top side [3,4,6]. Although both IR  and Raman clearly show the peak temperature occurring in the  source-drain gap of the HFET, on the drain side of the gate  contact where the peak electric field is located in the


es geses:


transistor, the IR measured device peak temperature is lower  by about 40% than the Raman determined temperature. Furthermore the temperature profile linewidth is wider using  the IR technique. This is consequence of the diffraction  limited spatial resolution of IR thermography, limited by the  wavelength probed, in our case of the 2 – 5.5 m spectral  window. Lateral averaging of temperature in IR when probing  devices with small active device regions therefore results in an  underestimation of device temperature, underestimating  potential risks for device failure. Thermal simulation can be  used in conjunction with IR thermography to estimate device  peak temperatures. However, unless the simulation parameters  are known to be accurate there is a non-quantifiable margin of  error for device peak temperature extrapolations based on IR  data.


Figure 2 also displays results of a finite difference simulation  of the investigated device. Heat is assumed to be generated in  a 0.4 μm wide region at the gate edge, with simulation  parameters similar to in [6]. Excellent agreement with the  Raman determined temperature as well as the linewidth of the  temperature profile was obtained, while differences between  the simulated and the IR determined temperatures exist due to  the above discussed spatial averaging of IR thermography. Table 1 summarizes the spatial resolution of both Raman and  IR for the here developed system, both the spatial resolution  estimated from the numerical aperture of the objectives [5], and the measured spatial resolution determined from the data  shown in Figure 2. The measured lateral spatial resolution for  IR is larger than the one estimated from the parameters of the  objective.


Although the use of micro-Raman spectroscopy is therefore  superior in terms of spatial resolution and peak temperature  accuracy to IR thermography, it needs to be noted that each  measurement point in Figure 2 takes several seconds to  record. A Raman linescan or a Raman map is typically  recorded by moving the probing laser beam point-by-point  sequentially over the device area measured. Although there  are certain approaches which can be used to speed up the  Raman measurement, this thermal probing approach is  therefore typically restricted to the analysis of limited device  areas, and recording temperature over an area similar to the IR  map shown in Figure 1, although possible, would be  impractical. This poses challenges for the analysis of large  ensembles of devices needed for the screening of electronic  devices, MMICs and reliability optimization, or for finding a  defect site within large device areas with potentially a high


temperature, i.e., subsequent device failure sites. Combing IR  with Raman thermography, i.e., using the integrated Raman –IR thermography approach developed here is therefore  beneficial. IR thermography is used to pre-screen devices to  obtain a quick overview of the device temperature distribution  as shown in Figure 1 to identify thermal areas of interest, and  micro-Raman thermal analysis as for example displayed in  Figure 2 can then be used to zoom into these selected areas to  obtain accurately device peak temperature. Obviously if the  target area is already known the initial IR thermal assessment  step can be omitted and just Raman thermal analysis is  performed. For example an IR map can be used to identify  inhomogeneities in temperature, e.g., related to defects, which  can be followed up by Raman thermography. Figure 3 shows  the effect a defect has on device temperature recorded with  Raman, not accessible in detail with IR thermography. A  significant temperature rise exists in the vicinity of this defect, the likely cause of a subsequent device failure observed. Such  defect areas or in general clusters of defects, commonly  statistically distributed over a wafer surface, can also result in  variations in device temperature and device lifetime when  considering devices from different parts of a wafer [8].


Apart from providing high lateral spatial resolution, Raman  thermography offers furthermore the possibility to also probe  temperature in three dimensions in a device structure. This is  achieved by confocal microscopy, i.e., by focusing the laser  beam at a well defined depth into the device structure. Figure  4 illustrates for an ungated device a three dimensional scan of  temperature measured from the device surface into the  substrates, using both the GaN and the SiC phonons to  determine temperature. Temperature decreases into the  substrate due to thermal diffusion through the substrate to the  heat sink. This makes the characterization of heat extraction  pathways through the device/substrate structure possible, important for the optimization of thermal management. It can


Figure 3: Raman temperature map in the vicinity of a defect  in an AlGaN/GaN HFET, recorded from the device top side. The defect is a micro-crack in the SiC substrate underneath  the device active area, with its location marked by “X”.


100°C100C  =155°C155C


wavelength probed, in our case of the 2 - 5.5 um spectral


210°C210C


Table 1: Estimated and measured lateral spatial resolution of  Raman and IR thermography for the developed system.


|Lateral Resolution |Raman |IR |
|---|---|---|

|Estimated, μm|0.5 |3-6 |

|Measured, um|0.4-0.6 |7-8 |

for example be used to support the development of advanced  thermal management approaches such as flip-chip  technologies [9]. Furthermore it can provide simulation with  adequate three-dimensional temperature data to fit their input  parameter space adequately for subsequent reliable and  validated thermal device simulations. We note that Raman can  probe temperature not only in DC as illustrated here, but also  with time-resolutions as short as nanoseconds, both in two and  in three dimensions [10]. This is a time-regime not accessible  using IR thermography. High time resolution, together with  high lateral and depth resolution, is therefore also possible  using integrated Raman – IR thermography.


The three dimensional measurement capability of Raman  thermography enables us here furthermore to gain detailed  insight into the depth resolution IR thermography actually  provides. This was not experimentally assessable before since  there was no technique available to measure temperature three  dimensionally. When measuring the ungated device of   Figure 4 using IR thermography a device temperature 50% lower than obtained with Raman was measured by IR. We  note as this device has a 20 m wide active device area there  is no lateral averaging of device temperature occurring in IR, i.e., this temperature discrepancy has a different origin from  the temperature difference between Raman and IR for the  HFET of Figure 2. Temperature appears to be averaged over a  depth in excess of 100 μm in IR thermography considering the  data of Figure 4. Since IR thermography is an IR intensity  measurement, it picks up temperature signals from a variety of  depths, and in particular areas such as the high-thermal  conductivity epoxy used to fix the chip onto the package with  its high IR emissivity contribute significantly, in the actual  device measurement and in the emissivity calibration needed  to convert the measured IR intensity into temperature values. Temperature determined with IR is therefore an average of the  temperature variation through the thickness of the chip  coupled with variations in emissivity, i.e., it is a complicated  depth averaging process which determines the temperature  measured by IR. This needs to be considering when analyzing  IR thermography images of devices, whereas Raman is able to


measure this temperature depth profile directly. We note that  IR thermography sometimes uses a non-transparent high IR  emissivity layer deposited onto the device surface to enhance  accuracy, if a device can be sacrificed, however, in many  cases (as here in our experiments) it is desirable to re-use the  device after analysis and such deposition step is therefore not  performed. We note that reasonable agreement between IR  and Raman was achieved after deposition of such a layer on


°C)Temperature (


top of a similar device, although then varying thermal


。。。。0


boundary resistances between device surface and coating from  coating-to-coating was found to affect temperature accuracy  of IR. We note that the temperature depth averaging of IR is  responsible for the artificial temperature contrast in the IR  thermography image of Figure 1 of the AlGaN/GaN HFET  away from the active device area where some device areas  appear to show temperatures as low as room temperature. This  is therefore a significant underestimation of the real surface  temperature of the chip.


The development of integrated Raman – IR thermography was  reported and its use was illustrated on AlGaN/GaN electronic  devices. As it is a generic technique further applications to  other device systems such as Si and GaAs will be possible. The results show how the advantages of IR thermography, namely its capability for quick thermal device overviews, and  the advantages of Raman thermography, namely its high  spatial resolution, peak temperature accuracy, and its threetemperature measurement capability can be combined. Spatial  averaging and depth averaging of temperature in IR  thermography was analyzed.


Acknowledgement


The work in Bristol was supported by EPSRC, the work at  QinetiQ by the ES domain of the UK MoD and the  KORRIGAN program.


note as this device has a 20 um wide active device area there


[1] Lee, C., Witkowski, L., Tseng, H.Q., Saunier, P., Birkhahn, R., Olson, D., Munns, G., Guo, S., Albert, B., “Effects of AlGaN/GaN HEMT structure on RF  reliability”, Electronics Lett., Vol. 41, No. 3 (2005), pp. 155-157


[2] Blackburn, D.L., “Temperature measurements of  semiconductor devices - A review”, 20th Annual IEEE  Semiconductor Thermal Measurement Symposium  Proceedings (2004), pp. 70-80.


[3] Kuball, M., Hayes, J.M., Uren, M.J., Martin, T., Birbeck, J.C.H., Balmer, R.S., Hughes, B.T., “Measurement of  temperature in high-power AlGaN/GaN HFETs using  Raman scattering”, IEEE Electron Dev. Lett., Vol. 23, No. 1 (2002), pp. 7-9.


[4] Kuball, M., Rajasingam, S., Sarua, A., Uren, M.J., Martin, T., Hughes, B.T., Hilton, K.P., Balmer, R.S., “Measurement of temperature distribution in multi-finger


300


200


20 30 40 50 60 70 80 90 100


。o


SiC substrate GaN


Depth (um)Depth (m)IR measured temperature


Figure 4: Raman temperature depth scan taken in the center  of a 20 μm wide AlGaN/GaN ungated device, operated at  4 W. The data were recorded by focusing the probing laser  beam from above the die into the sample. Also displayed is  the IR thermography determined temperature.


AlGaN/GaN HFETs using micro-Raman spectroscopy”, Appl. Phys. Lett., Vol. 82, No. 1 (2003), pp. 124-126.


[5] Sarua, A., Ji, H., Kuball, M., Uren, M.J., Martin, T., Hilton, K.P., Balmer, R.S., “Integrated Raman/IR  thermography probe for monitoring of self-heating in  AlGaN/GaN transistor structures”, IEEE Trans. Electron  Dev., Vol. 53, No. 10 (2006), pp. 2438-2447.


[6] Rajasingam, S., Pomeroy, J.W., Kuball, M., Uren, M.J., Martin,  T., Herbert, D.C., Hilton, K.P., Balmer, R.S., “Micro-Raman temperature measurements for electric  field assessment in active AlGaN/GaN HFETs”, IEEE  Electron Dev. Lett., Vol. 25, No. 7 (2004), pp. 456-458.


[7] Kuball, M., “Raman spectroscopy on GaN, AlGaN and  AlN for process and growth monitoring / control”, Surf. Interface Anal., Vol. 31, No. 10 (2001), pp. 987-999.


[8]  Pomeroy, J.W., Kuball, M., Wallis, D.J., Keir, A.M.,


Hilton, K.P., Balmer, R.S., Uren, M.J., Martin, T.,  Heard, P.J., “Thermal mapping of defects in AlGaN/GaN  heterostructure field-effect transistors using micro-Raman  spectroscopy”, Appl. Phys. Lett., Vol. 87, No. 10 (2005),  pp. 103508 1-3.


[9] Ji. H., Kuball, M., Sarua, A., Das, J., Ruythooren, D., Germain, M., Borghs, G., “Three dimensional thermal  analysis of a chip-chip mounted AlGaN/GaN HFET using  confocal micro-Raman spectroscopy”, IEEE Trans. Electron Dev., Vol. 53, No. 20 (2006), pp. 2658-2661.


[10] Kuball, M., Riedel, G.J., Pomeroy, J.W., Sarua, A., Uren, M.J., Martin, T., Hilton, K.P., Maclean, J.O., Wallis, D.J., “Time-resolved temperature measurement of AlGaN/GaN  electronic devices using micro-Raman spectroscopy”, IEEE Electron Dev. Lett., Vol. 28, No. 2 (2007), pp. 86-89.


Reduction of Acquisition Time for RIL, SDL and LADA


Arjan Mels & Frank Zachariasse


NXP Semiconductors, Nijmegen, The Netherlands  arjan.mels@nxp.com & frank.zachariasse@nxp.com


A timing change in an operating circuit induced by a laser  disturbing a data or clock path, can be used to localise a defect (RIL [1] or SDL [2]) or critical timing path (LADA [3]). Although the techniques RIL, SDL and LADA are slightly different, the main operating principle is the same and the theory  presented in this paper is applicable to all three methods. Throughout this paper we will refer to LADA, as all experimental results in this paper were obtained with a 1064nm laser  on defect free circuits.


Experience shows that LADA signals occur in a range of ‘strengths’. From case to case, the same laser power will cause  a ‘spot’ which can range from a very strong response to one ‘buried’ in noise and requiring much scan integration to identify. We have found that in practice users tend to optimise the  conditions for signal collection intuitively: they tend, for example, to position the test conditions far away from the shmoo  edge (the boundary between passing and failing) for strong  signals, but closer to or at the shmoo edge for weak signals, in  an attempt to obtain the cleanest possible signal in the least  time.


In this paper, we first define mathematically what ‘signal  strength’ actually means in LADA. From there, we demonstrate a statistical model of the LADA situation that explains  the optimal conditions for signal collection and the parameters  involved. We continue by testing this model against experimental data.


In addition we use the developed model to optimise the acquisition time. We have done so by varying some of the parameters involved and experimentally verifying their impact.


Theoretical model


Failure Probability


Consider an IC containing a circuit with ‘critical’ timing. At a  given operating voltage, there is a value of clock frequency (or other timing parameter, such as clock phase or edge  placement) where the timing in the chip stops working. An  example could be the set-up time or hold time for a flip-flop to  capture data, or a memory access time. Since it concerns a  digital test, which is either pass or fail, this timing represents a  highly non-linear response. In fact, in the absence of any timing jitter or voltage noise in the circuit, the response to an in6


finitesimally small change in timing could be from pass to fail – and hence ‘infinitely’ sharp.


However, in practice, any circuit will suffer from a variety of  noise sources - whether intrinsic (for example noise in  MOSFET current) or extrinsic (for example jitter on the input  clock). Therefore, in a real circuit, as you approach the shmoo  edge, and repeatedly test the chip, the probability of failure  decreases smoothly from 100 % to 0 % over some range (for  example a range in clock period or a range in voltage).


The jitter causing this smearing will typically follow a Gaussian distribution, when adding many sources of uncorrelated  noise, as dictated by the central limit theorem. For a Gaussian  distributed jitter, the probability of pass or fail is given by the  cumulative distribution function of the Gaussian distribution. When the mean of the Gaussian (and therefore the 50% point  of the cumulative distribution) is called μ and the standard  deviation σ, then the probability can be expressed as


⎟⎠⎞


⎜⎝⎛ −


erf


2 1


||Check layout and fail bit map for concerned layer|
|---|---|

|||

||Delayering to 1st. possible affected layer|

||+ Voltage contrast and inspection|

|、|、|

||Remove layer (stop at contact level)|

||Nano probing:  check for diode / gate leakages|

|*|*|

||Measure transfer characteristic of all cell transistors|

||→ Measure output characteristic of all cell transistors|

||+ Additional measurements?|

variations of the transistor parameters (e.g. threshold voltage


and maximum drain current) inside high density SRAM cells


are getting more and more important [2]. Nano probing tools


like atomic force probing (AFP) are able to determine the


electrical characteristic of every transistor of the SRAM cell of


interest in detail [3]. However, physical imaging of the root


cause is often not possible. Reliable two-dimensional implant


profile imaging is almost impossible.


This paper describes an approach to overcome this problem by


fitting the transistor characteristics of process and device


simulation to the measured transistor characteristics. This


helps to generate reliable fault hypotheses and allows the


wafer fab to react.


Analysis Flow and Set-up


The investigated structures are standard single port static


random access memories (SRAM) manufactured using a 130 nm technology (see figure 1).


The analysis was performed according to our standard SRAM analysis flow [4]. Figure 2 shows a simplified flow chart of the


SRAM analysis process. The analysis approach down to contact level used standard PFA methods like surface parallel


defects causing device failures are decreasing in size also [1].


polishing and SEM voltage contrast and imaging.


Fig. 2: Simplified analysis flow chart


The starting point for the usage of a nano-probing tool is the contact level of the SRAM cell. In our lab we are using AFM- on diffusions and gates was performed with a ‘current


and negative bias voltage) [5]. If there is no indication for  leakage, the transfer and output characteristic of all 6 SRAM  respect to the transistor specification and the transistor       matching within one SRAM cell.


The device failed at Vddmax with single cell fails (SCF)


SRAM cell failed if the read instruction follows the writeFig.4. Transfer characteristic NMOS drive transistor - linear


Standard FA techniques like TEM cross section do not show a         AFP current imaging is able to visualize gate leakages andphysical root cause within the area inspected (see images 6 and


transistor geometric effects can be excluded.


Also standard 2D implant dose profile imaging techniques like  Nano probing on contact level (CA) showed a significant


the device and implant profile dimensions are approaching the


typical area of few nm and therefore the area of interaction of


A shift in threshold voltage in the range of 100mV towards


the probe tip with the sample surface.


higher values and therefore lower maximum drain current


(approximately 35%) of NMOS2 is visible. This can explain the failure of the SRAM cell.


NMOS access transistors


60.0000E-6


50.0000E-6


NMOS drive transistors


1.0000E-12


UgM


10.0000E-12


0.000.200.400.600.801.001.201.401.60


100.0000E-12


1.0000E-9


000.0000E+0*


女


10.0000E-9


10.0000E-6


100.0000E-9


1.0000E-6


20.00008-6


W30.0000E-6


40.0000E-6


100.0000E-6


0.000.200.400.60    0.801.001.20   1.401.60


Ug[V]


N1Id [A] N2Id[A]


linear view; no mismatch


Fig.3. Transfer characteristic NMOS drive transistor    logarithmic view; shifted threshold voltage


000.0000E+0


20.0000E-6


30.0000E-6


transistors are measured. The collected data are evaluated with


p40.0000E-6 V50.0000E-6


imaging' approach using different biasing conditions (positive


70.0000E-6


80.0000E-6


based ‘atomic force prober' for nano probing. A leakage check


90.0000E-6


Problem description -case study


-◆-N1Id[A]---N2Id[A]


dependent on the write - read delay only. The concerned


instruction with a small delay of less then lus.


view; low maximum drain current


Both SEM imaging and voltage contrast on metal / via levels


and AFP current imaging gave no hint to a physical root cause.


leakage current from diffusion to well in the range of several


7). By comparing the actual size of failing and reference


nA. From circuit simulation it is known that few 100 of nA are


necessary to generate a fail of the SRAM cell. Therefore


leakages can be excluded as root cause for the failure.


scanning capacitance microscopy (SCM) and scanning


spreading resistance microscopy (SSRM) were used for root


mismatch of the two NMOS drive transistors N1 and N2 (see


cause analysis without a conclusive result [6 & 7]. However,


figure 1, 3, and 4 while the access transistors NMOS3 and 4


(fig. 5) and the PMOS behaved as expected.


=N3Id[A]N4Id[A]


Transfer characteristic NMOS accesses transistorFig.5.


Fig. 6 TEM cross section; comparison of fail and reference         transistor -no failure visible


Drain


Fig. 7 TEM cross section; detail of failing transistor


gate region, this failure hypothesis was dismissed.


TCAD simulation and failure analysis


Physical root cause determination by standard FA techniques      was not successful. To allow the wafer fab to implement


countermeasures to avoid this type of SRAM fail, a new approach for root cause identification was used. The measured transistor characteristic of the failing SRAM cell is the starting point for further investigations.


According to the measured transistor characteristics several failure hypotheses were introduced and the simulated transistor


characteristics were fitted to the results from nano probing.


The developed possible failure hypotheses were checked with  additionalnano probing measurements   and imaging  techniques.


Hypothesis I - gate depletion:


Ikeda et al report poly silicon gate depletion as root cause for


shifted threshold voltages inside a SRAM cell [8]. Figure 8


shows the simulated transfer characteristic for different poly


子


silicon dopant concentrations. The shift of the threshold


云


voltage towards higher voltages with lower polysilicon dopant concentration is visible.


Fig.8 Simulated NMOS transfer characteristic logarithmic      view) with different poly silicon dopand concentrations;     influence on threshold voltage visible


The root cause for gate depletion might be poly grains that are


too large. Grain boundaries represent fast diffusion paths for


dopants in polysilicon. Large polysilicon grains will result in  poor dopant distribution across the gate poly. A surface


parallel TEM was performed to allow an assessment of the poly grain size (Figure 9). The poly grain size looks regularly


distributed, no grain size difference between the two


mismatched NMOS transistors was observed. Due to the fact


that the grain size is significant smaller than the size of the


Source


-0,20,00,20,40,6    0,81,0  1,21.41,6  1E-16


1E-15


1E-14


1E-13


1E-12-


1E-11-


1E-10


a1E-9


1E-8


1E-7-


1E-6


1E-5-


1E-4-


1E-3


日期期1其群"海"际书!?p


0,01-


Vg[V]


1-1e21


-.-5e20--1e20-5e19-1e19--5e18=-1e18-*-5e17 1e17


Fail


transistor


Fig.9 Surface parallel TEM -poly grains without objection9


Hypothesis II - blocked LDD:


A second good correlation between simulated data and


measured transistor characteristic was found for partially


blocked LDD (lightly doped drain). Figures 10 and 11 show


the results from TCAD simulation. The black dots represent


the reference (pass) transistor. A fully blocked LDD (red dots)


will shift the threshold voltage towards lower values and can      Fig.11 Linear view of NMOS device characteristic of different be therefore excluded.


blocked LDD implant; no significant drain current visible for


Fig.10 Logarithmicview of simulated NMOS device     characteristic of different blocked LDD implant


A partially blocked extension might be another possible


physical failure hypothesis. For TCAD simulation, a nitride


blocking layer on the transistor active area was used to simulate this potential failure mode. Only a few nanometres of nitride is necessary to cause the measured shift of the threshold voltage.


thickness of blocking nitride larger than 7.5nm


With the help of TCAD simulation it is also possible to locate


the failure more precisely within the transistor. Figure 12


shows a simulation were the LDD blocking is located on one diffusion of the transistor only.


-0.20.00,20,40,60,81,01,2       1,41,6 0,0000


0000...0


0,0002


0,0004


0,0006---2.5nm Nitride 0,0008


0,0010--no Ext/Halo 0,0012


---POR


--12.5nm Nitride一一10nm Nitride---7.5nm Nitride--5nm Nitride


-0,20,00,20,4   0,60,8   1,01.2141,6


1E-16


1E-14hid


1E-13404


1E-12


1E-11


21E-10


1E-9


1E-8-


1E-7


11*1****1111


1E-5


1E-4


1E-3mmmmmmn... .Ja....


0,01


一■-POR


4**星


02222-- no Ext/Halo


---12.5nm Nitride-*- 10nm Nitride-=-7.5nm Nitride--5nm Nitride-.-2.5nm Nitride


N2→


Z


4.001.4


Fig.12 Logarithmic view of NMOS device characteristic of


single sided blocked LDD implant.


Black: POR; Red: no extension; Green: 10nm blocking layer;CA


gate


Blue: 20nm blocking layer; Cyan: 30nm blocking layer;


spacer


magenta: 40nm blocking layer; yellow: 50nm blocking layer;orange: 100nm blocking layer;


Solid lines: source sided anomaly;


Dotted lines: drain sided anomaly


compare thickness to


The solid lines represents a source sided anomaly while the


ref. transistor


dotted lines are a drain sided anomaly. Again, the threshold


shift depended on the location of the anomaly for partially        Fig.14 TEM cross section; layer to compare marked


In contrast to this simulation, the measuredtransfer


wrong. The additional layer might have been removed during a


All transistors were measured twice: The first measurement


cleaning process within the process flow.


As discussed above, a partial blocking of the LDD implant can


This means the partial blocking of LDD is located on both


sides of the transistor. A TEM analysis was performed towafer fab to investigate the influence on process steps around


measure the thickness of the spacer layers of a failing


Transfer Characteristics


120.00E-6


0..萌N4


100.00E-6


心


[


v]60.00E-6PI


40.00E-6


20.00E-6


000.00E+0


80.00E-6


→N1Id[A]=N2d[A]N1Id[A]SD-N2Id[A]SD


Fig.13 Linear view of measured NMOS device characteristic


1og11(0zadn)narps/1n))


no difference with respect to source drain definition


blocked LDD is visible (blue lines; black: reference).


No additional layer on top of the LDD area was found.


characteristic of the affected NMOS transistor is symmetrical


However, this fact does not mean this fault hypothesis is


with respect to the definition of source and drain (Figure 13).


was defined with drain inside the SRAM cell, the second one


with source inside the concerned SRAM. These measurements


were marked on Figure 13 with the extension SD.


analysisnot be proven by means of standard failure


techniques. Therefore several split lots were defined at the


the extension implant module. With these improvements, the


transistor in comparison to a reference (Figure 14).


occurrence of thisfailure was  reduced drastically.


cause of SRAM soft failures even if classical physical failure


analysis has to close the job with no physical defect found.


The interaction of nano probing and TCAD simulation can


Failure Physics and Analysis ESREF2005


Acknowledgments


[5] T.X. Tong and A.N. Erickson, "Current Image Atomic


whole Munich FA team for fruitful discussions and the


advanced technology node", ISTFA 2004


S. Gorlich for their general support.


[1] R. Mulder, S. Subramanian, T. Chrastecky; Atomic


Force Probing Analysis of Non-Visible Defects in


[8] S. Ikeda, Y. Yoshida, K. Ishibashi, Y. Mitsui; Failure


Sub-100nm CMOS Technologies, Proccedings from


the 32nd International Symposium for Testing and


Failure Analysis ISTFA 2006


[2] B. H. Calhoun, A. Chandrakasan; Analyzing Static


Noise Margin for sub Threshold SRAM in 65nm


CMOS; Proceedings of the 311. European Solid-State


Circuits Conference ESSCIRC 2005


[3] M. Griitzner; Advanced Electrical Analysis of


The paper shows a new approach to identify the physical root


Embedded Memory Cells Using Atomic Force  Probing;Proceedings of the 16thEuropean


Symposium on Reliability of Electron Devices,


give crucial hints for root cause identification.


[4] P. Egger, C. Burmer; SRAM Failure Analysis        Strategy; Proccedings from the 29nd International


Symposium for Testing and Failure Analysis ISTFA 2003


Force Microscopy (CI-AFM) combined with Atomic


The authors wish to thank F. Siegelin for TEM preparation, the


Force Probing for location and characterisation of


management of the FA lab in Munich especially F. Bruns and


[6] G. Zimmermann, A. Born, B. Ebersberger, C. Boit;


Appl. Phys. A76, pp885 (2003)


[7] S. Schoemann, D. Alvarez; Doping Mapping by


andsub-10nmSSRM - Reaching Maturity   Resolution, Proccedings from the 30h International


Symposium for Testing and Failure Analysis ISTFA 2004


Analysis of 6T SRAM on Low-Voltage and High


Frequency Operation;; IEEE Transaction on Electron


Devices Vol. 50 No. 5 May 2003


3-D Defect Localization by Measurement and Modeling of the Dynamics of   Heat Transport in Deep Sub-Micron Devices


A.Reverdy, M. de la Bardonnie, L.F.Tz. Kwakman


NXP Semiconductors, 860 rue Jean Monnet, 38920 Crolles, France,Antoine.reverdy@nxp.com


M. Lamy


STMicroelectronics, 850 rue Jean Monnet, 38926 Crolles, France


C. Wyon


CEA-LETI/Minatec, 17 rue des martyrs, 38054 Grenoble, France


A. Doukkali, H.Murray


Laboratoire de Microélectronique ENSI-Caen Philips, 2 rue de la Girafe, 14000 Caen, France


P. Perdu


CNES, 18 avenue Edouard Belin, 31401 Toulouse, France


Due to relentless down scaling of device geometries, failure  analysis is getting more and more complex. As a matter of  fact, the success rate of Thermal Laser Stimulation (TLS) techniques drops significantly for 90/65 nm CMOS devices  because of the lack of x, y and z accuracy.


In our aim to improve the TLS based fault isolation method, we have studied thermal time-constant signatures using a  Modulated Optical Beam Induced Resistance Change (MOBIRCH) technique that may provide accurate x and y  submicron resolution as well as depth or z-information of  defects in the interconnection part of devices. Both Modeling  and measurement results indicate that OBIRCH signal phase  shifts and heat-up & cool-down time constants indeed do  correlate with the location, dimensions and density of the  structures studied.


Nowadays, the Thermal Laser Stimulation technique is widely  used for fault localization in complex submicron devices. It is  well appropriate for localizing electrical defects in the Back  End Of the Line (BEOL: interconnection parts of devices), particularly shorts and resistive paths. The most commonly  used technique, is OBIRCH (Optical Beam Induce Resistance  Change), first developed by Nikawa and Tosaki in 1993 [1]. Other techniques like TIVA (Thermally Induced Voltage  Alterations) [2], TBIP (Thermal Beam Induced Phenomenon)


[3] and XIVA (Externally Induced Voltage Alteration) [4] are  based on the same physical principle and differ only by  biasing conditions and detecting methods.


OBIRCH was effective for old technologies, but the technique  started showing practical limitations when applied to 90-65  nm CMOS devices for two principal reasons. First, the  localization accuracy of approx 1 µm² (laser beam waist)


becomes insufficient to exactly pinpoint the defective zone  necessary for subsequent physical FIB-SEM or TEM  characterization.


So, the technique has to be improved such that the lateral  and/or depth resolution matches typical device dimensions. If  for example we consider a spot size of ~ 1µm², in 65nm  CMOS technology this area may cover up to 6 poly lines or 20  contacts (Figure 1). Since lateral resolution is difficult to be  improved, the failure analyst would be helped if additional  information could be extracted from the TLS signal, e.g. third  dimensional information (depth-information), geometrical  characteristics, or some environmental description of the fault  location. All these complementary defect characteristics  coupled with existing GDS file information, may improve the  knowledge of defect position.


Figure 1: Illustration of OBIRCH technique limitation:


SRAM 65 nm CMOS cell superimposed on the OBIRCH laser  beam (~1 µm²) showing that within the laser excited region  there are many contacts, transistors and metal lines!


Second, with the reduction of structural device dimensions, the supply voltage and operating current are lowered. As a  consequence, the OBIRCH detection ability drops  significantly. Hence, to keep OBIRCH effective on latest IC  generations it is required to increase its detection sensitivity.


One way to reach these goals is to use a Modulated laser  intensity combined with the OBIRCH technique (MOBIRCH). Instead of static laser illumination, our proposed method  works with a dynamic laser source, allowing temporal studies  of the alternating TLS current.  We will describe the operating  principles of a pulsed laser and provide most relevant details  of the experimental set-up. Through experimental data  obtained from MOBIRCH measurements on specific model  structures we will demonstrate that from the shape of the  OBIRCH signal information can be extracted about the heatup characteristics of the device under test (DUT) and that  measured Phase shifts are directly linked to geometrical  parameters (size and position of heated metal line) of the  DUT.


Thermal Laser Stimulation technique, from  static to dynamic laser heating


The main principle of static TLS [5] is to create a local  thermal gradient, with a spatially confined laser source. The  local temperature deviations induce a resistance variation (ΔR) that depends on the resistance temperature coefficient (αTCR) of the conducting materials, according to the formula:


L


R


TCR Δ


Δ


0 αρ


Where ρ0 is the metal resistivity, αTCR is the metal thermal  coefficient of resistance, S the metal line cross-section, L the  length heated, and ΔT is the temperature variation induced by  the laser.


Figure 2: Principle of OBIRCH in standard configuration  with a constant laser source.


In the case of OBIRCH, the Device Under Test (DUT) is  biased with a constant voltage source, and a specific  amplification chain detects current variations due to resistance  change (Figure 2).


The laser source used has a 1340 nm wavelength for two  principal reasons. Firstly, the corresponding energy causes  thermal, but no carrier generation phenomena. Actually with  silicon technologies due to silicon band gap (1.11eV), a  wavelength smaller than 1100 nm has enough energy to create  electron/hole pairs, and, thus, can induce a current in active  parts of the DUT. This phenomenon is employed in OBIC [6],


LIVA [7] and LADA [8] techniques, more dedicated to fault  localization in the active parts of the device.


Secondly, at this wavelength the silicon substrate, is almost  transparent (depends on substrate doping) [9] and the  measurement can also be done from the backside of the wafer, which is necessary when multiple metal layers do screen the  more embedded defects.


As pointed out before, the most important limitations of this  technique when applied to last generation devices are its  sensitivity and resolution. To counteract the reduced  sensitivity, we can use a modulated laser beam. It permits to  integrate a lock-in amplifier (L.I.) into the detection chain, which improves the S/N ratio and increases sensitivity [10].  Resolution can be significantly improved by using specific  optical systems like Solid Immersion Lenses [11] or Fresnel  diffractive lenses [12]. When using these lenses the resolution  can be improved by a factor of ~2 which allows to extend the  TLS applicability to one or two additional technology nodes. Anyway, in very high density features, a lot of elementary  structures can be covered by the spot size in x, y and z  direction.


Figure 3: Simulation of TLS response of an electrically active  line, in case of standard and Modulated OBIRCH.


Top: OBIRCH case, Middle: MOBIRCH case


Bottom: Vector representation of the TLS signal. MOBIRCH  technique gives access to more information (Δφ: phase-shift  between laser modulation and MOBIRCH signals, and ΔR: amplitude of the MOBIRCH signal)


To overcome this lack of spatial resolution, we have  developed an innovative evaluation technique, based on laser  beam modulated OBIRCH (MOBIRCH) that allows extraction  of additional information from the phase shift between  OBIRCH response and square laser modulation, not accessible


A  TLS signal Magnitude (A.B


ΔR


I


NWTY?MMP


ΔRRΔφ


1-dimensional vector  information (R)


2-dimensional vector  information (R & φ)


Dynamic-Laser spot displacement (A. U.) Static-Laser spot displacement (A. U.)


Laser power modulation (A. U.)


Static


stimulation


Detection


chain and  imaging


Laser beam λ = 1340 nm


in a standard configuration. It is mostly focused on the indicial  response under thermal laser stimulation.


As illustrated in figure 3, classical OBIRCH records amplitude  variations of an OBIRCH signal without any dynamic  information. Laser source modulation permits an access to this  time response signature that potentially contains additional  information about elementary structure involved in thermal  stimulation and therefore a more accurate localization (x, y, z) of defects.


It is worth mentioning that this modulation method can also be  applied to the so-called Seebeck technique that is based on the  measurement of gradients in electrical potential at metallic  interfaces induced by the thermal gradient. Here, the DUT is  grounded to avoid resistance change detection. This  phenomenon is known as thermoelectric effect or Seebeck  effect. Applied in failure analysis, this technique can  effectively pinpoint voids in metal lines [13].


Experimental Set-up


Test Structure description


For this study, we used a 65 nm Electro-Migration (EM) test  structure, composed of several embedded copper lines that are  different in terms of:


• Metal layer level (Metal 5 to metal 1)


• Line width (1100nm, 740nm, 480nm, 110nm, 90nm)


• Surrounding metal density


As such, this test structure allows studying the MOBIRCH  response of many different copper lines and it is believed that  from the specific responses one may extract information about  how the MOBIRCH signal of a real defective device will be  influenced by the nature and location of the defect:


The first variable, the specific metal level of the activated Cu  line, allows analyzing the depth influence on the MOBIRCH  time response. If a correlation exists, it is reasonable to expect  that one also can extract information about the depth of a  defect in a real device and, thus, to be able to introduce 3-D  fault localization.


With a similar reasoning, the second variable, the line width, can be linked to defect geometry (size of a short, dimension of  a void…).


Finally, studying different surrounding metal density  configurations permits to discriminate between MOBIRCH  responses in two distinct cases:


• The “Low-density environment” (LDE) configuration  allows a direct access of the laser to the activated Cu-line, and since no other copper lines exist in the near vicinity, the predominant heat loss mechanism consists of heat  transport to the silicon substrate that acts as an isothermal  heat sink.


• In the “High-density environment” (HDE) configuration, several other copper lines and copper dummy structures  exist in the near vicinity of the activated copper line both  in horizontal and vertical directions. In this particular case (partial) screening of the laser beam may occur and  several heat loss mechanisms have to be considered given  that both the silicon substrate and the Copper structures  act as thermal heat sink. Hence, this environment will  result in a different dynamic response of the MOBIRCH  signal.


In figure 4, the EM test structure and the two different density  regions are illustrated.


Figure 4: The used Test structure: Top: Cross-section of the  copper line in a Low-density environment. Middle: Top-view  of a studied copper line. Bottom: Cross-section of the copper  line in a High-density environment


Experimental setup


Experiments were made on a HAMAMATSU PHEMOS 2000  system, which incorporates a NIR laser-scanning microscope, and an operating system that permits slow scan acquisitions (1µs/pixel to few ms/pixel), in various scan areas (windows of  1024*1024 pixels to 32*32 pixels, horizontal and vertical line  scan, fixed point…). By using an acousto-optical module  implemented into the optical path, our 1340 nm NIR 400 mW  high power source can be modulated, either at 5 or 50 kHz  using an internal trigger or at any other frequency when using  an external trigger signal. After standard amplification, the  MOBIRCH signal is accessible at the output of either a  HAMAMATSU amplifier or a Stanford Research SR 850  DSP lock-in amplifier and can also be measured directly using  an oscilloscope.


The oscilloscope setup is primarily used to analyze the exact  shape of the MOBIRCH signal, when a precise point (HDE or  LDE) of the active line is illuminated by the laser.


Studied   line


Low-density


。metal


environment   High-density  metal


environment


The Stanford Research lock-in amplifier has been the  preferred choice for our phase-shift experiments because it  allows accessing additional LI-parameters (time-constant, rolloff, sensitivity, input configuration, harmonics  measurements…) and to freely select the modulation  frequency.


Finally, the Lock-in output signal is re-injected into the  HAMAMATSU acquisition card, treated and imaged by  PHEMOS 2000 software.


Figure 5: Experimental Setup for phase-shift imaging, and  MOBIRCH signal shape study.


Why a Lock-in amplifier?


Lock-in amplifiers are commonly used to detect and measure  a very small AC signal when this signal is obscured by noise. Such amplifiers use a phase-sensitive detection method to  single out the signal of interest, see figure 6.


In our case, we are using it in order to extract time constants  of heating and cooling process, which are specific for each  structure topology and its environment. These time constants  can be only properly measured with square signal stimulation  and not sinus stimulation, as it should be for usual Lock-In (LI) measurements.


This square stimulation is mandatory to target time constants. The rising edge (heating process) and respectively the falling  edge (cooling process) have to be as sharp as possible in order  to avoid any side effect on thermal answer. This thermal  response can be measured with a scope and we firstly did it. The main advantage of LI measurements is the great  improvement of S/N ratio, but in our case it is a powerful  measurement tool, which gives a direct access to OBIRCH  time constant, faster than oscilloscope measurements.


LI measurements use a reference signal (fref) to both modulate  the laser source, and to generate the LI internal reference  frequency by which the MOBIRCH current variations are  multiplied. Internally, the amplifier uses a phase-locked-loop (PLL) that is locked on this reference signal and that outputs a  reference sinusoidal wave that is essentially free of noise.


The MOBIRCH and the PLL output signals are multiplied  using a Phase Sensitive Detector (PSD), and after a Low  Frequency Filtering (LPF) the resulting signals are directly


outputted (X & Y), or analyzed in a Digital Signal Processor (DSP) to extract amplitude (R) and phase-shift (φ) information.  .


oo


Figure 6: Simplified functional block diagram of a Lock-in


一


amplifier


pope oo


When assuming a sinus modulation, φ and R can be calculated  as follows:


• MOBIRCH signal:


sin(


mob


ref


MOBIRCH


φ


ω +


• REFERENCE signal:


REFERENCE


• Signal after the Phase Sensitive Detector:


-.


])


.2


cos(.


PSD


ω


• The PSD output is passed through the Low Pass  Filter (LPF) to remove the 2.ω AC signal. If the  filtering is effective, the resulting signal can be  approximated as:


cos(


REF


MOB


LFP


X


φ −


The X signal is proportional to the MOBIRCH signal  amplitude, but also includes a cosine term that is phase shift  dependent. To extract the amplitude, a second PSD needs to  be used with a 90° shifted reference signal. The output of this  PSD after low frequency filtering is:


21


LPF


Y


From both PSD channel outputs, all characteristic parameters  of the MOBIRCH vector signal can be calculated in the DSP: The Magnitude:


²


² Y


MOB +=


and


the Phase


(tan 1XY


As we previously mentioned, MOBIRCH and trigger signals  are not sinusoidal waves, but can always be reduced to a series  of sine waves via Fourier Transform. As explained before, the


山  PLL   90° phase


shift


DSP for


R & φ  calculation


Internal  oscillator


Differential  Input


Reference  Input


Y Out


R Outφ Out


囟


X Out


Interface  Box  Signal


generator


Laser modulation


Reference frequency


Post


processing & imaging


Phase shift imaging   Shape study


square trigger signal is internally converted in a noise free sin  wave, but in fact, the lock-in amplifier can internally generate  a sin wave at any harmonic of the reference signal frequency. So, referring to the previous calculation, it allows measuring  amplitude and phase shift at each harmonic of the modulation  signal.


In our experiments we have used both the principal frequency  and the third harmonic to calculate the phase shift.


MOBIRCH shape study & analytical model


The exact shape of the time modulated OBIRCH signal is  determined by the heat-up and cool-down dynamics of the  electrically activated copper line in the test structure, as is  illustrated in figure 7. The studied Cu lines are illuminated by  a square modulated heat source (λ=1340 nm). The shape of  the MOBIRCH signal suggests that induced by the laser, the  local temperature of the line rises exponentially from an initial  value to a maximum value that depends on the laser power  and the heat transfer dynamics within the device structure. When the heat source is shut-off, the copper line temperature  decays exponentially to its initial value if the laser-off time is  long compared to the cool-down time constant.


From figure 7 it is concluded that the rise and decay of the  signal are dependent on line width and depth (figure 7a), and  on surrounding metal density (figure 7b).


To quantify these dependencies, we propose a simple model  that fits well with the experimental MOBIRCH signal and that  allows extraction of characteristic heat-up and cool-down time  constants from the Modulated-OBIRCH signal.


Time (sec.)


8。。


10 12


*10-5*10-5


Normalized magnitude (A.U.)0


Figure 7: Examples of MOBIRCH response shapes for  different line parameters:


Top: M5, 1100nm wide line in LDE (green line) versus M3, 480nm wide line in LDE (blue dotted line)


Bottom: M5, 1100 nm wide line in HDE (green line) or in  LDE (blue dotted line)


In a first approximation we use a first order model to describe  the exponential temperature variation, which is proportional to  current magnitude change:


cd


hu


down


Cool


up


Heat


τ


∝


.(


In this formalism, the information of interest is included in τhu  and τcd, the heat-up and cool-down time constants; a0 and a1  are respectively the offset and the magnitude of the signal. An  illustration of this model is given in figure 8:


Figure 8: Graphical representation of 1st order modeling. We  represent the two time constants extracted (green dotted line) from the model.


This 1st order model is well adapted to describe the response  of a metal line isolated in oxide (LDE). But it appears limited  when applied to metal lines in the high-density copper  environment (HDE). In the latter case, during both heat-up  and cool-down phases, the copper dummies environment does  significantly modify the heat loss mechanisms, and  consequently, the shape of the modulated-OBIRCH response. To better account for the influence of the surrounding metal  density, we need a more refined model that includes an  additional term that reflects the heat exchange between the  active copper line and it surrounding:


With:


⎥⎦


⎤


⎢⎣⎡


1 2


cd cd


aττ


α


Laser Power modulation  DUT temperature change


Time (A.U.)


τcd


τhu


Magnitude (A.U.)a0  a0+a1


1 2 1 2


CD


hu hu


HU


ττ


Where, during the heat-up phase, τ1hu is the principal time


constant describing the heating of the line  by laser


illumination, and τ2hu a secondary time constant describing


the cooling effect of the environment, which acts as heat sink.


During the cool-down phase, τ1cd is the principal time


constant describing the cooling of the heated line and τ2cd is


the secondary time constant describing the heating effect of


the also hot environment; a0 and a1 are amplitude and offset


coefficients.


The first exponential term illustrates the first order laser effect


(ON or OFF), and the second one describes second order


effects stemming from multiple environment exchanges,


detailed hereafter:


During heat-up phase:


• Secondary heat sources: dummies illuminated by the ue7,50 laser (directly or after reflection).


s u 0


7,00


见


• Heat sink: dummies at reference temperature 0(underneath the line).


w


血


a6,50上6,00


During cool-down phase:


• Remaining heat sources: hot dummies due to heat-up


110nm480nm740nm


phase.


||M 4 |M 4 |
|---|---|---|

||自||

All these environmental effects induce some system inertia, 1,101,20which is evidenced by a horizontal asymptote at the start of  the HDE response (figure 9), and well covered by the refined 0,901,00 model


)0


( =Δdt


8 0,70


d


2 0,80


Figure 9: simulation results of heat-up, cool-down 2nd order  analytical model superimposed on experimental MOBIRCH  response, for High and Low density copper environments.


All experimental MOBIRCH signals, obtained for both HDE  and LDE configurations, can be perfectly fitted with this 2nd  order analytical model. The goodness of fit: R-square is better  than 0.999 as it will be illustrated hereafter.


Time constant extractions and discussion


In figure 10 experimental results are obtained with the time  constant extraction setup, where the laser is pulsed at a  frequency of 10 kHz, and fixed at one point of the test  structure in the low density area. The data are directly  extracted from the OBIRCH signal captured by the  oscilloscope. The time constant values reported are the sum of  tau1 and tau2 (figure 10.a) and just tau2 (figure 10.b).


Figure 10: Time constants extracted from experimental  MOBIRCH signal shape, in Low Density copper Environment, versus line width and depth, the line width variation ranges  from 110 nm to 1100 nm.


Figure 10.a (up): Time constant τ = τ1+τ2 for metal level 4  and 5.


Figure 10.b (down): Time constant τ = τ2 for metal level 4.   From figure 10 we can conclude that metal 4 responds quicker  than metal 5, and that the heat-up and cool-down phases are  characterized by essentially the same time constant value (~6,5 and 7.5 µs for metal 4 and 5 respectively). The


舌48121620


measurements further show that there is no clear correlation  between line width and time constant. This most likely is due  to the fact that laser positioning is not sufficiently accurate to  ensure that the line is perfectly centered underneath the laser  beam each time. When comparing the absolute values of τ1+τ2 and τ2 (figure 10.a vs. figure 10.b), we find that τ2 is


Line width (nm)


M 5  M 4


0,40


Heat-up phase


△


Cool-down phase


8,50


8,00


Experimental  data


00121620


Modelling   results


3


Low-density metal  environment


740点1100nm


口


High-density metal  environment


-3metal environment


Heat-up Mechanism


a w0,60


10,50


Time (µs)


Line temperature (A. U.)ottf4o心Cool-down Mechanism


one order of magnitude smaller than τ1. This result is in line  with what would be expected for the studied line in a Low  Density Environment, where - since no copper dummies are  present - only the silicon substrate acts as a heat sink.


These initial results are interesting because they indicate that it  is possible to discriminate between two consecutive metal  layer levels, and, furthermore, that the complex heat-up and  cool-down mechanisms can be well described by a simple  model.


In figure 11 similar results are presented, but this time for  measurements in a High Density Environment.


Figure 11: Time constants extracted from experimental  MOBIRCH signal shape, in High Density copper  Environment, vs. line width and depth, the line width variation  ranges from 110 nm to 1100 nm.


Figure 11.a (up): Time constant τ = τ1+τ2 for metal level 4  and 5.


Figure 11.b (down): Time constant τ = τ2 for metal level 4.   From figure 11, we remark that time constant values are  significantly different for measurements made in a High  Density Environment (~ 11 µs instead of 7 µs). Also, in this  case the cool-down time constant is slightly lower than the  heat-up time constant (figure 11.a), the difference being  explained by larger secondary time constant values that  represent more important heat losses (figure 11.b). Interestingly, the time constant of metal 4 level under thermal  stimulation is higher than that of metal 5 level under thermal  stimulation. Again, this observation can be explained by the


fact that in a HDE the lines are not directly, but indirectly  heated by the laser due to the screening effect of upper metal  layers. Since this screening effect is more important for metal  4, heating is even more indirect and thus will take longer.


We have further analyzed the MOBIRCH signals obtained in  LDE, using a Fast Fourier Transform. By doing so, we are  able to calculate the phase shift between the laser modulation  and the MOBIRCH signal. Some results are illustrated in  figure 12.


Figure 12: Calculated phase shift from experimental  MOBIRCH signal vs. line width and depth for metal level 4  and 5. The line width variation ranges from 110 nm to 1100  nm.


The trends in phase shift are similar to that of time constant  i.e. metal 5 layer stimulation shows a more important phase  shift than metal 4 layer stimulation, and the observed line  width variations are identical. Hence, phase shift  measurements can equally well extract relevant information  about the heat dynamics, and moreover have the advantage  that they can be done fast and in an automated mode if a lockin setup is used as described earlier. Phase shift  measurements, therefore, will be the subject of the next  chapter.


Phase shift analysis and discussion


In the following, phase shift measurements are presented  obtained with the phase shift measurements setup, where the  laser is again pulsed at a frequency of 10 kHz, but in a single  line scan mode, where the laser is perpendicularly passed  across the test structure in the low and high density area.


First, we have studied the dependency of phase shift on line  width, as illustrated in figure 13 (LDE) and figure 14 (HDE).  Contrary to the time constant results obtained in a single spot  mode, the MOBIRCH phase shift shows a clear correlation  with the line width, in LDE and HDE case. Since the line scan  mode eliminates the problem of laser positioning, this type of  analysis gives an indication on the geometric dimension of the  studied line. But we can notice that in the HDE case, the  scanned line location can induce some measurement  variations, because of it relative position compared to  dummies position (figure 14). Based on these findings, it is  not unreasonable to expect that by phase shift analysis also  short circuit in failing devices can be identified. In addition, figures 13 and 14 demonstrate also the ability of this phase


M 5


M 4


M 4  M 5


shift detection technique to discriminate successive metal  layers, and as illustrated in figure 13.b, third harmonic  analysis gives a better discrimination (5° vs. 2° per metal  layer).


Coherent with the time constant measurements, we again find  that the phase shift values differ for HDE and LDE case (+50% for the HDE case) which suggests that also phase shift  measurements are sensitive to the local environment.


Figure 13: Phase shift measurements between the  experimental MOBIRCH signal and the modulation signal vs. line width, for 3 different metal levels, in Low Density  Environment.


Figure 13.a (up): 1st harmonic measurement.


Figure 13.b (down): 3rd harmonic measurement.


Figure 14: Phase shift measurements between the  experimental MOBIRCH signal and the modulation signal vs. line width, for 3 different metal levels, in High Density  Environment.


As a second parameter, we have studied the influence of the  metal layer level on the phase shift measurement. The results  in Low Density Environment are presented in Figure 15:


P


吕


Figure 15: Phase shift measurements between the


-85


experimental MOBIRCH signal and the modulation signal vs.


-90


metal layer level, for the min. line width, in LDE  Figure 15.a (top): 1st harmonic measurement.


-95


Figure 15.b (bottom): 3rd harmonic measurement.


shift (deg)Phase-100


As previously seen, in LDE, more embedded is the line in the


-105


dielectric, larger is the phase shift between the MOBIRCH  signal and the laser power modulation. The variation is linear  from metal 5 to metal 2 layers, and the more important  difference between layers metal 2 and 1 is explained by the  fact that the metal 1 layer is thinner and less wide (90 instead  of 110 nm) than the other metal layers studied. Third  harmonic analysis allows a better discrimination between  successive metal layers.


This last finding is interesting because it permits a 3-D  localization (x, y, z) of the active line, instead of just a 2-D


|喝 十|M 5 |
|---|---|

||M 4 |

|M 3 |M 3 |

-44


localization (x, y) in case of standard OBIRCH analysis.


忐命


The proposed innovative evaluation technique has already


品士


provided encouraging first results and appears very promising


shift (deg)Phase


49


for 3D fault isolation. MOBIRCH signatures of elementary  structures under square shaped thermal stimulation allow time  constant extraction from a second order model we have  developed. These measurements have been done from phase  shift detection method using a lock-in amplifier. It has  demonstrated its ability to add complementary information  like width information, depth information, or environmental  density information. While in the present study only test  structures have been evaluated it is expected that phase shift  measurements also will provide additional information about  type and location of electrical defects in real devices. When  coupled to GDS files, this additional characteristic  information will certainly help to improve the detection of  such defects. Our future research will therefore be focused on


Metal layer


|M5 |M4 |M3 |M2 |M1 |
|---|---|---|---|---|

|||十|||

Phase shift (deg)-28-32-36


|1 + 中 ☑||
|---|---|

|M 3 ||

|M 4 ||

|M 5 ||

-28


M5


M4


M3


M2


M1


-75


Phase shift (deg)台发台台


台


Phase shift (deg)-95


480 nm


740 nm


1100 nm


Metal 3;    Metal 4;     Metal 5      Line width (nm)


|最 4|重||
|---|---|---|

|厂|||

|工|壹|M 3 |

||本|M 4 |

|||M 5 |

the application of MOBIRCH to real case studies of failing  devices fabricated with latest CMOS technology.


The authors wish to thank C. Gallrapp for his preliminary  study on the analytical thermal model. They also would like to  thank S.Orain for his contribution on thermal phenomena  interpretation and J. Roux, T. Kume from Hamamatsu  photonics for Lock-In Amplifier specific integration in our  PHEMOS.


[1]  K. Nikawa and S. Tosaki, International Symposium  for Testing and Failure Analysis, 1993, pp. 303-310.


[2]  E.I. Cole Jr and al., “backside localization of open  and shorted IC interconnections”, International  Reliability Physics Symposium, 1998, pp. 129-136.


[3]  M. Palaniappan and al, “New Signal Detection  Methods for Thermal Beam Induced”, International  Symposium for Testing and Failure Analysis, 2001, pp. 171-177.


[4]  R.A. Falk, “advanced LIVA/TIVA Techniques”, International Symposium for Testing and Failure  Analysis, 2001, pp. 59-65.


[5] F. Beaudoin and al. “Modeling Thermal Laser  Stimulation”, Microelectronic Reliability, Vol. 41 (2001), pp. 1477-1482.


[6] G. Grasso and al, “Scanning Laser and Optical Beam  Induced Current Methods for Failure Analysis of  Electronic Devices”, Optical Storage and Scanning  Technology, SPIE, 1989, pp. 13-26.


[7]  R. A. Falk, “Advanced LIVA/TIVA techniques”, International Symposium for Testing and Failure  Analysis, 2001, pp. 59-65


[8] J. A. Rowlette and T. M. Eiles, “Critical timing  analysis in microprocessors using near-IR assisted  device alteration (LADA)”, International Test  Conference, 2003, pp. 264-273


[9]  R. A. Falk, “Near IR absorption in heavily doped  silicon – An empirical approach”, International  Symposium for Testing and Failure Analysis, 2000, pp. 121-127.


[10] M. de la Bardonnie and al., “The effectiveness of  OBIRCH based fault isolation for sub-90nm CMOS  technologies”, International Symposium for Testing  and Failure Analysis, 2005, pp. 49-58.


[11] S. B. Ippolito and al., “High spatial resolution  subsurface thermal emission microscopy”, Applied  Physics Letter 84 (22), (May 2004), pp. 4529-4531.


[12]F. Zachariasse and al., “Diffractive lenses for high  resolution laser based failure analysis”, International  Symposium for Testing and Failure Analysis, 2005, pp. 1-7.


[13]A. Glowacki and al., “Characterization of  thermoelectric devices in Ics as stimulated by  scanning laser beam”, International Reliability  Physics Symposium, 2005, pp. 450-457.


Effects of Backside Circuit Edit on Transistor Characteristics


RK Jain, T Malik, TR Lundquist, QS Wang


Credence Systems Corp, Sunnyvale, CA, U.S.A.


R. Schlangen, U. Kerst, C. Boit


Berlin University of Technology, D-10587 Berlin, Germany


Backside circuit edit techniques on integrated circuits (ICs) are becoming common due to increase number of metal layers  and flip chip type packaging.  However, a thorough study of  the effects of these modifications has not been published.  This in spite of the fact that the IC engineers have sometimes  wondered about the effects of backside circuit edit on IC  behavior.  The IC industry was well aware that modifications  can lead to an alteration of the intrinsic behavior of a circuit  after a FIB edit [1]. However, because alterations can be  controlled [2], they have not stopped the IC industry from  using the FIB to successfully reconfigure ICs to produce  working “silicon” to prove design and mask changes.


Edit Hole


Reliability of silicon device structures, transistors and diodes, are investigated by monitoring intrinsic parameters before and  after various steps of modification.


The increase in density of advanced process devices and the  decrease in interlayer material thickness have again increased  the difficulty for the FIB community to produce successful  circuit edits.  Circuits are modified not only to produce  prototypes during first silicon debug but they are also edited  for engineering samples to be distributed for system validation  and software development.  Therefore, accuracy and reliability


Ion beam


of the edit becomes very important—it must last more than a  few hours; it needs to last weeks if not longer. Front side  studies on affects of circuit edit ion beams on device  parameters such as threshold voltage (VT) have been


-Trench200x200μm


published [3, 4]1.  It does need to be noted that dynamic


N-well


affects of backside editing has been investigated at Intel [5]


p-diff


and the Technical University of Berlin [6].  But these have not  investigated transistor I-V curves.


Bulk


contacts□n-diff


There are some fundamental differences between backside and


N Well


0 H


Silicon


front side circuit editing.  For example, the edit incorporates


IP


(P-doped)


cutting an M1 line on a 6 metal layer 0.13 µm Copper process.


*o0口口


Two power planes and one dummy structure from the topside


Metal 1


cover the M1 line (Fig 1a).  From the backside there is some  dummy diffusion and poly covering the M1 (Fig 1b).


1 It might be that when gate dielectric was thicker there was


more of an issue due to charge injection into the dielectric and  as this dielectric has gotten thinner it becomes pretty much


self healing.


Starting from sample preparation to the completion of the edit  a backside circuit edit goes through some different process  steps compared to a front side edit.  The impact of each of  these backside edit steps is studied and will be presented in  this paper:


1. DUT thinning


2. n-Well exposure


3. STI exposure


4. Through silicon editing


(a)


(b)


Figure 1: (a) Typical frontside edit process on a standard  CMOS process [8]. (b) Typical backside edit process on a  standard CMOS process [9].


Experimental setup and procedure


A 30 keV CE FIB tool, is used for performing the backside  circuit modifications. The test chips used were fabricated in a  standard TSMC, 0.18 µm, 6 layer, Al process. Transistor  antenna structures2 are incorporated to be used to characterize  charge and other invasive effects of the FIB on transistor gates  as well as source/drains (Fig. 2, 3). The antenna ratios of these  structures are 1/10/1k with plate antennas of both Poly and  Metal1 (together) Test chip features include NMOS and  PMOS transistors, with and without gate protection diodes3.    Independent drains and gates are used. Common sources and  wells are used. Sources and Drains have Mtop nodes, as well  as Metal 1 nodes. Gate length = 0.18 µm and gate width = 5.0 µm.  The components of theses transistors are connected  directly to external pins simplifying investigations.  Only  nMos transistors were examined in this study.


NMOS


PMOS


Figure 2: pMOS & nMOS antenna device


Gate protect


(source drain)


Figure 3:  Close up view of the antenna device


FIB: Circuit Edit (process)


The device was characterized after each of the steps  highlighted in bold:


• Delid DUT; this then became the reference


2 The antenna structures associated with the gate would result  in a larger interaction cross section—experience more stress


from mechanical process, including trenching and accumulate  more charge.  However, these would also be averaged over a  larger area and thus very local effects would tend to be more  subdued.  So the “jury” is out in regards to what should be


expected from these structures.


3 In regards to FIB circuit editing, protection diodes, which are  designed in for ESD protection, generally protect the gate


from charge injection.


• Thin DUT down from 760 µm to 30 µm by using a  global polishing tool4 5.


~ 2.5 hrs


• Locally trench with the FIB to NWell voltage  contrast, including deposition of a protective  insulator.


~ 45 min


• Form access holes with the FIB to shallow trench  isolation (STI) (getting close to transistors)     ~ 5  min


• Deposit insulator to isolate future contacts through  the Si


~ 4 min


• Expose 1.50x1.50µm  M1 to source


~ 3 min


• Deposit low resistivity conductor


~ 2min


• Expose 1.50x1.50µm  M1 to drain


• Expose 1.50x1.50µm  M1 to gate


The measurement was done on four nmos transistors. Three of  the four nmos transistors have a protection diode.


Figure 4:  Optical image of the trench taken with a 700nm  source.  The fringes indicate a slope ~100nm/fringe.  Devices  1,2,3 have protection diode while 4 does not. (1) nmos, r=1, 50nm remaining silicon (2) nmos, r=10, 100nm remaining  silicon (3) nmos, r=1k, 150nm remaining silicon (4) nmos, r=1,  300nm remaining silicon.


4 Once it was “proven” to be non-invasive, thinning to 30um


enables the FIB work to go faster.  Heat sinking of course


becomes more of an issue, but when properly done everything  works well with Si actually running cooler as the heat sink has  better thermal conductivity than the Si itself.


5 Certainly not all devices can be globally thinned, some such  as those in QFP packaging require local milling.


diode


4                3      2     1


R1O_DRAIN


M6 nodes


Access holes through the silicon were ~ 2 µm x 2 µm; openings exposing poly-silicon or M1 were 1.5 µm x 1.5 µm.  All access and deposition operations were done using 50pA  beam currents.    Figure 5 and 6 shows M1 and Poly exposed  through the trench floor.


4um


Vt curve:


Figure 5: M1 exposure through floor of trench.


Protection Diode & 10k Antenna Structure


0.70


0.60


0.50


Figure 6: Gate Poly exposure through floor of trench.


Results


I-V and Vt curves were obtained in the following manner for  all four nmos transistors.  The graphs on NMOS with the  protection diode and r=1k is shown as an example:


• Before DUT thinning


• After DUT thinning


•  After trenching


• After Source contact


• After Drain contact


• After poly-silicon Gate contact


Note that the Vt is ~0.56V in every case.  In agreement with


出


the ~0 mA result in the I-v curves for Vg = 0.6V. IVcurves:


Protection diode and 1k antenna structure


7.00*Vgw0.60V


Vg=0.85V


-6.00-aVg=1.10V


+Vg=1.35V


5.00*Vg=1.60V*Vgr1.85V


+Vgm2.10V


4.00


088


-200


什


000


-0.15a0s0.250.450.650.051.051.251.451.6515-1.00


(ldmA)


Vd (V)


Figure 7: Typical I-V Curves; This was obtained before DUT  thinning.


0.20


0.10


0.0000.20.406081.2141.618


Vg(V)


Figure 8: Typical Vt Curve; This was obtained before DUT  thinning; Vt = 0.56V.


Discussion


It is certainly difficult to see much difference in the data from  one I-V curve set to another.  For high or low Gate Voltage  Vg the differences are greatest.  A better way to study the  impact of the sequential operations is to examine the I-V and  Vt curves of one transistor as it is impacted.  Figures 9 to 11  make these comparisons.  In Fig. 9, I-V curves for Vg = 0.6 V  shows ~0 mA in agreement with the almost unchanged Vt.  What stands out is the impact trenching has on the I-V and Vt  curves.  Thinning has negligible or no impact on these.  After  trenching the I-V and Vt curves show some change in Vt; Vt(trench) = 0.52 and Vt(Original) = .55.  The values are  within the margin of error and therefore we can conclude that


Poly


Vt remains unchanged.  The transistor with no protective  diode showed more change from thinning than those that had  protective diodes (see Fig12).


I-V Curves (Vg =0.6)


0.5 1


1.5 2


2.5 3


0.4


0.6


0.8


1.2


1.4


1.6


1.8


Orig


Thin


Trench Source Drain Gate


Figure 9: I-V curve comparisons showing impact of each  operation against the original (before thinning) for a  transistor with a protection diode and R = 1.


I-V Curves (Vg = 0.85 V)


1.8XY Longitudinal口X


Figure 10:  I-V curve comparisons showing the impact of  each operation against the original (before thinning) for a


Depth vs. Y-Axis


transistor with a protection diode and R = 1.


Vt Curves


0.00


0.30


0.40


Trench Source Drain


Figure 11: Vt curves showing the impact of each operation 0A


-Target Derthagainst the original (before thinning) for a transistor with a  protection diode and R = 1.  Again the biggest change occurs  from the trenching process.


The first thought was that charge injection is a possibility but  probably much less of an issue with thinner, possibly self32


healing thin gate dielectrics and further would be reduced due  to operations through the silicon ground plane.  (The Si not  only shields but can source secondary electrons to negate  positive ions.)  Further charge injection would not be likely as  the lack of change to the curves even when the gate is  contacted schematically—no charge injection changing the  gate capacitance.


Trench


Figure 12:  Vt curves showing the impact of each operation  against the original (before thinning) for a transistor with no  protection diode and R = 1. As the biggest change occurs  from the trenching process the other operations were not  included.


The second thought was that changes might arise from Ga  implantation (or implantation of knocked-on, edit-process  chemistries).  However, from the TRIM calculation [10] as  seen in Fig. 13, the range of Ga is much less that the  remaining Si thickness over the transistors investigated.  Thus  the impact of Ga and lattice damage is not the likely  explanation.


1000A


Figure 13: Range in green of 30keV Ga ions at normal  incidence into amorphous Si.  The gray shows knock-ons  which can produce lattice damage.


Nevertheless, comparisons were made for transistors with had  been trenched to 300 nm and 100 nm and no differences were  found in the impact that trenching had.


For these 180nm technology nMos transistors6 it is unlikely  that the Si thinness resulted in any local lattice effects such as  relaxation which could affect carrier mobility [11], but this  cannot be ruled out in advanced process technologies.


The introduction of leakage currents due to the thinning is not  expected to be significant and thus not likely to play a part in  the curve shifts seen.  It would be expected that more direct  contacts to active diffusions [12] might show an effect but this  was not investigated.


Undoubtedly here the explanation lies in the depth of the STI  which isolates each transistor when the silicon is removed to  below this level [6].


Even with the low beam currents used in this work, it is  surprising that the I-V and Vt curves exhibit so little variation   The invasive character of a FIB edit has surprising little effect  on the transistor functionality which is probably due to  performance functionality centralized at the channel region  and as long as that region is not impacted their will not be any  dramatic effects.  In any case the IC industry can rest assured  that using the FIB to reconfigure ICs to validate design and  mask changes remains a useful process.


It does need to be noted that dynamic affects of backside  editing has been investigated at Intel [4] and the Technical  University of Berlin [5, 6].  But these have not investigated  transistor I-V curves.  Reliability of silicon device structures, transistors and diodes are investigated by monitoring intrinsic  parameters before and after various steps of modification.


Special thanks to Hanna Nguyen of Credence Systems  Corporation for polishing the samples down to 30 µm.


[1] Romain Desplats et al., “Reliability of Bipolar and MOS  Circuits after FIB Modification”, ISTFA 2001, 289.


[2] S Herschbein, C Rue, C Scrudato, E Hermann, “FIB Chip  Repair: Improving Success by Controlling Beam-Induced  Damage and Thermal / Mechanical Stress”, ASM ISTFA  2004, 166.


[3] A. Campbell, et al., “Effect of FIB Irradiation on MOS  Transistors,” Proc. 35th IRPS 1997, pp. 72-81


6 nMos transistors would be the least affected by any lattice


modification affects from trenching the Si [11].


[4] J. Benbrik, et al., “FIB Irradiation Induced Damages on  CMOS and Bipolar Technologies,” Proc. 24th ISTFA  1998, pp. 49-55J. Rowelette et al., “Microwave signal  Propagation in Backside Focused Ion Beam (FIB) Fabricated Interconnects”, ASM-ISTFA (2002) 559.


[5] R Schlangen et al., “Electrical Performance Evaluation of  FIB Edited Circuits through Chip Backside Exposing  Shallow Trench Isolations”, IEEE-ESREF (2005) 1544.


[6] C. Boit et al., “Impact of Backside Circuit Edit on Active  Device Performance in Bulk Silicon ICs”, IEEE-ITC (2004) 482.


[7] S. Herschbein, et al, “Basic Technology & Practical  Applications of the FIB for the Laboratory Workplace,” Microelectronic Failure Analysis, Desk Reference, 4th  Edition (1999), 517.


[8] C Boit, K R Wirth, E Le Roy, “Voltage Contrast like  Imaging of N-Wells”, ASM-ISTFA 2003, 331.


[9] J Ziegler, SRIM & TRIM, www.srim.org/


[10] R Jammy, IEEE-IEDM 2005 Short Course.


[11] J P Huynh, J P Shannon, R W Johnson, M Santana, T Y  Chu, M Gonzalez, “Backside FIB Device Modifications  through the BOX Layer of an SOI Device”, ASM-ISTFA  2002, 403.


FIB Backside Circuit Modification at the Device Level, Allowing Access to Every  Circuit Node with Minimum Impact on Device Performance by Use of Atomic


Force Probing


Berlin University of Technology, D-10587 Berlin, Germany   Schlangen@mikro.ee.TU-Berlin.de , +49-30-314-25406


S. Schömann, B. Krüger


Infineon Technologies, D-81739 Munich, Germany


R. Jain, T. Malik, T. Lundquist


Credence DCG, CA 94089-1138 Sunnyvale, USA


Direct measurements of circuit node signals without changing  the performance of the circuitry are essential in modern FA  but often impossible for recent IC technologies. This paper  shows new methods, based on FIB backside circuit edit, allowing access to every existing circuit node at the device  level, and discusses options for probing and discrete  characterization.


Throughout the whole development of Failure Analysis (FA) discrete transistor characterization and probing of inner circuit  nodes has always been essential. As long as the number of  metal layers was moderate Focused Ion Beam (FIB) tools  were widely used to create electrical contacts to targeted  circuit nodes [1] through the frontside of the chip. But due to  technology innovation and Flip Chip packages the direct  access from the structured frontside to the inner circuit nodes  and especially to the transistor level is mostly blocked [2, 3].  For this reason, optical analysis tools, such as Time Resolved  Photon Emission or Laser Voltage Probing, were developed  and are widely used. These tools allow load-less probing of  inner circuit nodes through the thinned chip backside and  offer very high bandwidth. But because of the limits of optical  microscopy the lateral resolution is no longer sufficient to  resolve the smallest transistors on recent technologies.


For the characterization of single transistors, the most  common procedure is to take away all metal layers down to  the tungsten contacts by use of parallel lapping. After that, FIB pads may be deposited, followed by electrical  characterization at a regular probe station. Alternatively, a  SEM probe station can be used to characterize the suspected  transistors. During the past years Atomic Force Probing (AFP) was developed to a necessary level of stability to provide a  relatively fast solution, where no FIB deposition and no  vacuum based SEM system are needed for discrete device  characterization. The biggest disadvantage of these methods is  that they require the physical destruction of the circuitry. If  the root cause was located in the metal stack or can not be


found amongst the suspected transistors, the operator does not  have a second chance.


This paper shortly reviews the application of AFP from the  chip frontside, and then reviews the FIB backside circuit edit (CE) procedure, including all necessary preparation steps. The  main topic is direct probing and single transistor  characterization from the chip backside by use of a regular  probe station and AFP.


The paper shows how a new backside Circuit Edit (CE) procedure, named Contact to Silicide (CtS) can be used to  contact any inner circuit node. This method offers a way to do  probing and most of the desired single transistor  characterization without destroying circuit functionality.


To speed up the analysis routine, classical FIB pads can be  avoided by the use of AFP. This also minimizes the impact on  high frequency device performance, allowing high speed  testing and various discrete measurements on the same DUT. Experiments on ring oscillators (RO) are presented to  demonstrate general functionality and to elaborate on the  limitations of these methods.


AFP on parallel polished samples


Figure 1 shows the cross section through a readily prepared  DUT, illustrating the general idea of AFP. The sample has  been reduced to the device layer including the tungsten plugs.


Figure 1: AFP on lapped frontside sample


Highly controlled parallel lapping, followed by a short  decoration with buffered HF solution is typically utilized for  physical sample preparation.


The available AFP tools consist of up to 5 independently  moving Atomic Force Microscope (AFM) heads. In scanning  mode all heads run simultaneously in exactly the same motion. This delivers up to 5 independent images, all showing a  fraction of the area of interest. The single probe can then be  positioned on the targeted contact with sufficient accuracy for  recent technology geometries [5, 6].


In addition to the physical destruction of all metal layers, the  success rate of this method is also determined by the quality of  the lapping process. The operator has to remove the whole


FIB Pt


AFP needles


front-end including M1 whereas the tungsten contacts and  especially the device layer have to stay functional. For recent  technology this is already challenging, and if multiple  measurements in different chip areas are needed this approach


NW


注


PW


will face its limitations.


p-Poly


n-Poly


FIB backside procedure


CoSiIMD


To allow measurement access from the chip backside a W combination of mechanical grinding and FIB based milling is


necessary. The first important steps are illustrated in Figure 2.


Figure 2: FIB backside CE process flow


The backside sample preparation starts with depackaging and  mechanical thinning using either global lapping tools or more  localized grinding tools to reduce the remaining silicon  thickness (in this case to less than 30 μm in the relevant chip  area, as marked with line 1 in Figure 2). The mechanical  thinning has to be completed with a very accurate mechanical  fine polish to enable the following FIB preparation. Subsequently, a large trench covering the area of interest is  locally milled down using the FIB tool with XF2 assisted  etching until the operator stops (“endpoints”) on the n-well (NW) level.  The trench bottom at this stage is marked with  line 2. From this trench floor one or more small windows  down to the STI level can be opened using Iodine based etch  recipes. The finally remaining active chip area underneath the  opened STI window (below line 3) is then reduced to the  technologically determined height of the STI shapes (approximately 300 to 400 nm with different bulk / STI


technologies) [3, 4]. Presuming an adequate mechanical  thinning the necessary FIB preparation will take less than two  hours.


New Circuit Edit Opportunities


With the readily prepared chip, partly opened down to STI  level, the operator can use the STI / Si contrast for local fine  alignment with accuracy below 30 nm [2]. At this point the  currently available procedures to contact an inner circuit node  are illustrated in Figure 3.


Figure 3: Overview of possible contact methods


The classical way to do so is marked with (1) and contacts


mechanically removed bulk Silicon


directly to a metal line. The access hole has to be milled  through electrically unused area, in this case STI. In highly  integrated areas this access is very limited and often fully  blocked by transistors, poly lines or lower metal layers. The


FIB removed bulk Silicon


reduced space also enforces high aspect ratio holes, which  lead to an increased via resistance.


Method (2) was named Contact to Contact (CtC). The access


Si


hole is milled right through the drain or source region and  ends on one or more tungsten contacts. This allows the non  destructive formation of an ohmic contact to every device with


more than one tungsten contact [4].


STI


Direct Contact to Poly structures (3) can also be fabricated,


W


IMD


but until now this approach has not been fully characterized  and is not discussed further in this work.


Method number (4) was named Contact to Silicide (CtS). The  milling of the access hole is stopped right in the Silicide layer  which covers all source / drain areas in recent chip designs. The Infineon test samples used in this work are fabricated in  120 nm bulk / STI technology, and have an approximately  35 nm thick Cobalt Silicide layer. A characterization of the  achieved contact properties and a detailed description of the  milling Endpoint procedure were published in [4].


Figure 4 shows the layout of a typical CMOS structure. In this  case a 3-way NAND. The marked in- and output metal lines  might still be suitable targets for a direct contact to metal, but  the input to gate two and three would definitely be blocked. The dashed red line indicates the area where CtC and CtS  could be used. This already covers every CMOS output. CtP  could connect to any poly structure, but since every gate input  is driven by some other output, this is not necessary to cover  all probing and characterization needs.


accessible with


only via


contact to


Silicide or ContactoutSilicidecontact tocontact


four↑


Figure 4: CMOS structure with possible contact areas


The green bars, in between the n-FET gates, indicate areas  only accessible with CtS. Due to the drastically reduced height  of the Pt via (350nm, compared to 1-3μm with direct contact  to metal) the CtS can have reduced lateral dimensions and still  offer lower via resistance due to the reduced aspect ration  below 3/1. Recent FIB tools offer secure endpointing and


重


reasonable contact resistance with a contact width below  200nm. With such small lateral dimensions it now becomes


CtS


possible to contact a full transistor, even in highly integrated  areas.


Experimental Setup and Results


STI hole


fIN


Sample preparation and Test Structures


To show the general functionality of backside probing and  non destructive transistor DC characterization, Ring  Oscillators (ROs) where prepared using the previously  described FIB backside procedures.


35μm


1μm


Figure 5: Layout and FIB n-well image of used RO structures  including 10 circular STI openings and one enlarged view of  a CtS contacting a divider input


ILS


The layout and a FIB image of the used RO structure can be  seen in Figure 5. Every RO consists of a high frequency


inverter ring, a ten stage divider (1/1024), and an output stage.


CoSi


A special SBGA test socked, mounted in the FIB chamber,


and a vacuum feed through was used to monitor the output


node of interest


frequency of the ring oscillator in situ. This was done during  the full FIB preparation, including all necessary STI openings  and CtS formations. The impact on the monitored output  frequency remained below 3% throughout the full preparation, for all utilized circuitries discussed in this paper.


Probing by use of CtS


To enable first measurements a RO running at ~108MHz was  prepared as shown in the middle of Figure 5. All ten divider  stages were modified in the very same way. The layout of an  individual divider stage is shown in Figure 6. Every stage is


丁


pp-MOS


inn-MOS


metal 1


composed of eight 2-way NANDs and one inverter, carrying


the input signal. The selected measurement structure was the


metal 2


n-FET of this input inverter, which is highlighted in the


diff


layout. The routing of the input signal is marked from the


Npoly


input M1 towards the contact location.


5


☑n-well


Figure 6: Divider layout with CtS location


The dotted circle roughly indicates the STI opening areas  similar to the right part of Figure 5. The size of the contact  opening was 800nm x 200nm for all CtS. The length of  800nm reflects the expanse of source / drain whereas the


ROdivider1/1024


width of 200nm was chosen to be a good compromise


n-wells


between contact resistance and stress to the device due to the


fx1o


留迫


fx10


留器fx4 output


职


6fout


active probe close proximity to the transistor gate.


Figure 7: Needle placement in small STI hole to automatically  contact to the CtS on the trench floor


After the full FIB preparation, the resulting structure should  look like the cross-sectional view of Figure 7. The use of a  relatively small circular shaped STI opening (diameter < 3μm) has the big advantage that the utilized active probe needle  only has to be placed into this opening and automatically  contacts the small Pt contact on the bottom of the trench. Due  to this geometry, the trench side walls keep the measurement


needle in place, which drastically reduces the necessary needle


microscope


sooda


placement accuracy und setup stability. First results using this ~50Xapproach are shown in Figure 8. To power up the targeted  circuitry, the DUT was mounted on a regular probe station


111


and was connected to 1.2V nominal power supply voltage. All  shown scope traces were measured using a Picoprobe 12C-4-10 (fMAX = 500MHz) active probe needle in combination with  a regular oscilloscope.


Note that due to the use of the active probe only the switching


DuT


input


information and not the real inner voltage level is measured.


ATE


h 1.8o Ch2 56.0mv M


so.omv M 10.ons


Figure 8: Oscilloscope measurements on 4 divider stages


The relevant probe points are marked in the middle part of


p-FETH


无CtS→


G1首总2日n-well


鲁王polydiffn-FET☑metal 1


Figure 5. Starting at the inverter ring, the frequency is divided


by two with every individual divider stage. Since all probe G2 points are located on the divider input, the first input fX1


directly carries the RO frequency. The input to the second


divider (fX2) will be fX1 / 2 and so on.


At first, the RO output signal fOUT (measured directly via Vdd package and test socket connection, after all ten dividers / not


比□contact


via active probe) was compared to the next higher frequency


fX10, measured at the input of divider 10. The shown result


exactly matches the expected value (fX10 = 2 * fout).


After that, more measurements were done following the


divider chain towards the high frequency RO part. Figure 8


(right) shows one more result, measured at the input of stage


4, with fX4 = 128 * fX10 and also the ring frequency itself, fX1 =


1024 * fout = 108.53MHz.


All measured frequencies match the theoretical values.


Furthermore, the used standard Oscilloscope (fmax = 150MHz)


could be operated without the use of an external trigger,


directly synchronizing to the measured signal.


These results prove that the FIB prepared contacts (CtS) offer G1 sufficient connectivity for direct high speed probing, and


using a dedicated setup, combining state of the art active


YX


probes, automated test equipment (ATE) and a regular optical  microscope could become a very powerful high bandwidth  probing solution.


Figure 9 illustrates the general idea of such a toolkit, were the  output of the active probe is directly connected to an


G2


additional input of the ATE. The detected signal can also be  monitored on a regular scope, simultaneously.


out=107.6kHz


x4=13.78MkHz


Figure 9: schematic probing tool set for direct backside  probing using CtS and active probe needles


Characterization of single FETs


To successfully characterize a single transistor, every terminal


f x10=2154kHz


50mV / div50ns / diV


has to be connected, and it must be verified that nothing else


fx1= 108.53MkHz


but the transistor contributes to the measurement. In the way  proposed here, the whole circuitry stays functional. The  transistors are still surrounded by and electrically connected to  the rest of the circuitry. As a first example, two n-FETs out of  one divider NAND were used. The enlarged layout is shown


50mV / div2us / div50mV / div10is/d√


in Figure 10. With frontside AFP, the two n-FETs cannot be  measured separately, since only nodes fabricated with a  tungsten contact are accessible with this method.


Figure 10: layout of a NAND with CtS on the middle node of  the 2 series n-FET


With the proposed backside preparation technique, a CtS can  be placed right in the middle between the two FETs in series  connection (marked with X).   This contact can now serve as  drain for the measurement of two separated output  characteristics of the n-FETs. Together with contact Y, established in between the two p-FETs, and connections to  gate 1 & 2, the upper n-FET (2) is ready to be measured.


The emergence of multiple core, high speed microprocessors


Nibride spacer


in  90nm node technologies has also increased the requirement


hardmask.


for large amounts of costly SRAM on-processor cache to  avoid excessive finite cache penalties.


Pad nitride


However, by employing Logic based on-processor embedded


Pad oxide


DRAM cache in 65nm SOI applications, limitations in SRAM


SOI


cache involving standby current, requirements for error  correction circuity to address soft error rate (SER), and Vmin


BOX


cell stability can be overcome.1-14  IBM has pioneered low cost  embedded DRAM for SOI processors. 1,2


substrateBuned


Reported high performance embedded DRAM 65nm SOI


plate


designs with ~ 1.5ns latency and < 2ns random cycle  characteristics are enabled by strain engineered pass transistor


(a) Sidewall spacer formation


(b) Deep trench etch


with optimized source/drain junctions for sub-pA off


BitlineActiveStrapPassing


currents.1-12


Implementing a deep trench capacitor design versus a plate


Su


WLMT


type design for embedded DRAM cache in these SOI designs  means fewer mask steps (with lower cost) accompanied by a  significantly smaller DRAM cell size.1-2  Relative to SRAM, embedded DRAM cell size for 65nm SOI  cache designs  measures 0.127 μm2 (vs. 0.299um2 for SRAM) and for 45nm


NodePaly


BuriedPoly


SOI cache measures 0.067 μm2 (vs. 0.149um2). These  embedded DRAM cell sizes dramatically increase cache


Buried


capacity (2Mb and 4Mb cache reported) while simultaneously


reducing cost, power consumption, and soft error sensitivity as  well as occupying a smaller size footprint.1-2


(c) Capacitor formation(d) STI and pass transistor formation.


A common failure mechanism in embedded DRAM process is  trench capacitor leakage. In particular, leakage between  adjacent cells due to defects in the isolation is one example. Physical Failure Analysis (PFA) with microscopy after bit  mapping is tricky as many defects are non-visual or ‘Sub46


Microscopic’.  Even pA leakage levels will cause poor charge  retention in eDRAM cells.


Nanoprobing can supplement and even replace PFA on such  structures as long as the data is of sufficient integrity to place  each failure in the correct category on a pareto chart. 16   Knowing what failure class to look for will also be key to  correctly choosing which PFA technique to use for final root  cause determination.


While the spacing between individual nodes within these  DRAM cells is not as aggressive as six transistor SRAM cells  for the same technology 25, nano probing said DRAM cells  presents different measurement challenges.


Figure 1


Novel Sidewall Spacer Deep Trench (SSDT) process.1-5


Figure 2


Comparison of Bulk Silicon eDRAM cell with SOI eDRAM  cell (note elimination of collar in SOI design) 1, 2


SOI eDRAM Description


Logic-based embedded DRAM cache on a high performance  65nm SOI platform involves a novel sidewall spacer deep  trench (SDDT) process (Figure 1) that effectively provides


ENW OD


low sheet and contact resistance. Low parasitic leakage is  achieved by the superior SOI BOX isolation. The collar design  used in bulk silicon deep trench is eliminated (Figure 2) resulting in a significantly lowered buried strap resistance.1, 2   This IBM process is called Sidewall Spacer Deep Trench or  SSDT.


Elimination of the collar from bulk silicon eDRAM trench  design yielded significant reduction in strap resistance in the  SOI design. A 15% Ion improvement is realized when the  strap resistance is reduced from 3kΩ to 1kΩ 1, 2


Employing a high performance SOI platform with deep trench  capacitor design for Logic based embedded DRAM cache for  on-processor applications has reduced cost, power  consumption, while fitting in a smaller size footprint.1,2


Nanoprobing Challenges


The challenges to electrically characterize discrete embedded  DRAM cells as small as 0.127μm2  for 65nm SOI  technologies and  0.067 μm2 for 45nm SOI technologies  requiring femto amp current sensitivities are not  trivial.16,17,18,19  In comparison, nanoprobing of six transistor  SRAM cell arrays for 45nm SOI technologies may involve  cell areas as small as 0.249 μm2  however the larger cell size is  filled with 6 transistors and 11 or 12 contacts resulting in an  area with closer spacing between probes 25.  For DRAM, the  challenges to nanoprobing are different; the bitlines are not in  a regular pattern so that in order to insure the correct cell is  probed:


Bulk SiliconSOI Design


1. the failed bitline must either be counted from a corner


or mark,


STI501


2. a super high precision (50nm accuracy) stage must be  used or,


3. a means of highlighting the leaking cell must be used


cips1


for registration.


Counting is difficult and probing and marking of failed cells is  not a good option for eDRAM because the mark is usually


deposited in a FIB or SEM, potentially causing physical


Collar


damage to the memory cell or electrical anomalies (eg. a short  through the BOX layer in the case of SOI). It has become  common practice to use AFM or AFP current imaging to  localize defects.17, 20  On SOI samples however,  current  imaging is not very effective since often (as in this paper) there is no current path to ground.  Precision stage navigation  works fine for locating previously bit mapped cell failures but  it is severly limited in  localizing unmapped defects.  Therefore a cell to cell leakage analytical technique is highly  preferred.


Deep Trench Capacitor Leakage Imaging with Two probe  Current Imaging


In order to create an imaging technique capable of measuring  trench to trench leakage, the imaging technique must highlight  current passing between two bitlines.


Figure 3a


Optical View of nanoprobes measuring an embedded DRAM  cell. The two probes on the right are fixed, contacting  wordlines. On the left, two nanoprobes are scanning  simultaneously over the array of bitlines while maintaining the  bit line pitch to check for trench leakage


Figure 3b


CAD layout of the eDRAM array with the marked probing


nodes of the word lines and bit lines corresponding to Figure


3a (above)


This means that at least two contacts must be involved in the


process. It has become common practice to use one probe to


contact a well or substrate contact and therefore create a path


from one scanning probe to another fixed probe.16, 17


However, if in this case the leakage path is only between


adjacent cells, no current can be collected from the bit line to


the substrate. This is one difficulty of working with SOI. B/L A(held high)


B/LB(low)


Figure 3a shows an optical image of a four probe DT leakage  technique performed on a 65nm SOI eDRAM array.16  Two


W/LA (high)


W/L B(high\


probes on the right are stationary, contacting wordlines and


Leakage Path


holding them high. These are the wordline probes.


Additionally, two probes (one of which is biased), are


scanning an area on the array containing a trench to trench BOX


leakage defect. These are the bitline probes. The other bitline


probes are scanned simultaneously maintaining exactly the SXOTADT BSXsame spacing as the bitline contact pitch. When the biased  probe is scanned over a bitline contact, its grounded partner is


contacting an adjacent bitline. Furthermore, the wordline


probes activate the transfer device as shown in Figures 4 top, 4


middle, and 4 bottom.


The wordline probes also connect the BL’s to their respective


trenches.16  This measurement was done on a portion of the


array (chosen at a corner for clarity) and the resulting probe


current image is shown in figure 5


Figure 4


Top: Circuit layout showing the cross section orientation


Middle: SEM image of a FIB cross section through a  representative DT set similar to the set that was measured  electrically. The anomaly in the isolation between the trenches  is not necessarily a failure. The tricky nature of finding a  femto or pico amp leakage path between failing cells  underscores the importance of nanoprobing analysis.


Bottom: A schematic of the leakage path measured between  trenches. Note that the wordline blocks access directly to the  DT capacitor. The wordlines must be both toggled high to  allow access to the buried isolation.


W/L Transfer Device


Strap                                       Buried


Oxide


DT         DT


CA                                               CA


Adjacent B/L Node                Adjacent W/L


0 目:


且:


Failing B/L Node                      Failing W/L B/ B←LLB/■A


Figure 5


Current image showing leakage at failing bit line contact of


leaky eDRAM cell corresponding to the layout shown in


Figure 6  The current imaging is so sensitive that all of the


bitlines adjacent to the contacted wordlines pass some current 1.0 due to the leakage in the wordline gate oxide.  But the trench


I (uA)


that is leaking to its neighbor shows much higher current.


It is not possible to detect node to node leakage in an ordinary  nanoprober without the unique simultaneous scanning feature  except by painstaking checking of each pair of nodes.16, 17


WORDLINE OFF


0.0


Cell B


-1.0


B/L node


-2-1.5-1-0.500.5V(Volts)2


Figure 6


Detail of bit line nodes contacted during nanoprobing for deep  trench capacitor leakage measurement between adjacent cells


PICO CURRENT


Deep Trench Leakage IV measurements


16.09


-9PA


Figures 4 and 6 describe the layout of these nodes. The  eDRAM layout depicting bit line nodes and word line nodes  employed in detection of deep trench capacitor leakage  between adjacent cells is shown in Figure 4 bottom.


--33pA


For the current leakage IV measurements, two probes contact  the failing word line node and the adjacent word line node. Two other probes contact the bit line node in one cell and the  bit line node in the adjacent cell .16


Y(um)


--58pA


Nanoprobe current imaging of the adjacent bit line nodes  revealed leakage between two adjacent cells. Figure 5 shows  the current image.  By contacting bitline A and bitline B and  activating the corresponding wordlines, an electrical short is  measured. Next, by toggling one of the word lines off, the  deep trench capacitor is isolated from the bitline and no  current flows as the voltage is swept positive.  However as the


13.12-


bitline voltage sweeps negative, it crosses the threshold


18.32


X(um)


21.32


voltage of the wordline transfer gate and turns the transistor on  so that the leakage current is again measured beyond the  threshold voltage of this transfer gate device.  The leakage  must now be trench to trench and is not associated with either  a wordline defect, substrate shorts or silicide pipes.


Figure 7


Two IV curves between Bitline contacts to failing (leaking) adjacent cells. Toggling the word line on connects BLA and  BLB to the adjacent trenches (DTA and DTB), since there is a


DT capacitor


defect in the isolation between trenches, an electrical short  was measured.  With the wordline off, the Bitline A is


leakage


disconnected from DTA and no current flows.  The wordline  transistor turns back on when the voltage on Bitline A is swept  negative and the current resumes.


A correlation can be established between the nanoprobe  current imaging signatures with subsequent electrically probed


Cell A


measurements. Validation of the current imaging signature is  demonstrated by the resulting nanoprobing results and shows  the importance of current imaging as a rapid inspection  method for detection of defects in eDRAM cells.


WORDLINE ON


Scanning Capacitance


The scanning capacitance microscope has become a staple in  semiconductor metrology and failure analysis.18, 19, 21, 22  Until  now, it had not been available in conjunction with  nanoprobing.  The powerful combination of nano CV with  nano IV should be a compelling improvement over either  technique alone.  In the case of SOI, capacitance imaging is  evolving into an essential component.  In Figure 8 below, scanning capacitance imaging over the eDRAM array yielded  a bright contrast inspite of the fact that all contacts are  electrically isolated from the substrate contact by the BOX  layer.  The BOX layer is invisible to the capacitance  microscope because it sees the large BOX area capacitor in  series with the much smaller device capacitor measured.


Figure 8 shows a scanning capacitance image of the eDRAM  array, current imaging shows no contrast due to the presence  of the oxide layer insulation.


Figure 9


CV plot of the bit line contact node in the failing eDRAM cell (red plot) versus the bit line contact node in the non failing  eDRAM cell.  The Y scale is in femptoFarads and the X scale  is in volts.


CV plots were taken with the newly designed capacitance  sensor operating at 1 GHz. Without changing the tip following  AFP current imaging or AFP probing results, the sensor used  the same AFP tip to produce these results. An innovative  resonator type design coupled with contact measurements  enabled these measurements.


These plots exhibit depletion characteristics described in the  literature.18, 21, 22, 23.  The results have higher signal to noise  relative to CV and dC/dV vs. V plots reported with the typical  RCA style capacitance sensor.24, 25


The leaking DRAM cell’s BL CV curve does not show  depletion whereas all of the non-leaking cells gave virtually  identical depletion curves.  It can be assumed the leakage in  the cell loads the depletion bias and therefore affects the  curve.  As the technique of scanning capacitance imaging with  current imaging develops, it should prove to be an invaluable  tool for fast defect location in eDRAM .


High performance Logic-based embedded DRAM based on  the 65nm SOI platform have previously ben demonstrated  with  ~ 1.5ns latency and < 2ns random cycle cell  characteristics.1,-15  These designs employing on-processor eDRAM overcome  limitations in SRAM cache involving standby current, requirements for error correction circuity to address soft error  rate (SER), and Vmin cell stability.1,2  The challenges to  nanoprobing and electrically characterizing discrete embedded  DRAM cells (0.127 μm2 for 65nm SOI designs and 0.067 μm2   for 45nm SOI designs) in these embedded 2Mb caches and  4Mb caches are formidable. The demonstrated utility of  nanoprobing current imaging to rapidly scan and detect  defects in eDRAM cells coupled with complimentary scanning  capacitance image capability offers a rapid means of  identifying buried node leakages at contact  (CA) level.


The possibility of early detection (at CA level) of FEOL  defects offers the promise of localizing defects without the  time consuming sample preparation steps employed in  conventional PFA techniques.


The authors wish to acknowledge the innovative logic based  eDRAM design in on-processor SOI of John Barth, Paul  Parries, Subramanian Iyer, G. Wang, Greg Fredeman, Kenji  Yanagisawa, Toshiaki Kirhata, Barbar Khan, Herbert Ho, among others.


The authors wish to thank Herbert Ho, Wei Kong, Alberto  Cestero, Karanam Balasubramanyam, and Dave Albert for  their technical input to this paper.


In addition, the sample preparation efforts of Bruce Redder, the FIB cross sectional work of Aaron Shore as well as the


Solid State Circuits, vol. 38, no. 11, pp. 1974-1980, Nov.


Symposium for Testing and Failure Analysis, pp. 482-486  g, A. Erickson: Current Image Atomic Force  Microscopy (CI-AFM) Combined with Atomic Force  (AFP) for Location and Characterization of  ed Technology Nodes, ISTFA2004, International  Symposium for Testing and Failure Analysis, pp. 42-46  avyalov, J. McMurray, C.C. Williams, Surface and  aracterization for Quantitative Two Dimensional  Dopant Profiling by Scanning Capacitance Microscopy, Characterization and Metrology for ULSI  logy: 1998 International Conference, American  e of Physics (AIP) Conference Proceedings, March  p 449-453 (1998).


|technical input of Andrew acknowledged. References |Dalton are |gratefully |(2004) 20. T. Ton |
|---|---|---|---|

|1. J. Barth, et al, “A 500MHz SOI Embedded DRAM Amplifier”, ISSCC 2007, |Random Cycle Macro Featuring a pp. 486-487: March |1.5ns-Latency, 3T Sense 2007. |Probing Advanc |

|2. G. Wang, et al., “A 0.127 SOI Based Embedded Applications “, IEDM 2006 |μm2 High Performance DRAM for On-Processor 2006, session 21.1    December |65nm |(2004) 21. V.V. Z Tip Ch |

|3. W-H Lee, et al., “High Technology with Enhanced Advanced-Low−Κ BEOL, December 2005 |Performance Transistor IEDM 2005, |65nm SOI Strain and pp. 56-59, |from Techno Institut 1998, p |

|4. E. Leobandung, et al. VLSI |2005, pp. 126-127 |||

|5. S.H. Dhong et al., ISSC |2005, pp. 486-488, |March 2005. ||

|6. S. Iyer, et al., “Embedded for Blue Gene/L Chip”, IBM no 2/3, pp. 333-350, Mar/May, |DRAM: Technology J. Research Dev. 2005 |Platform , vol. 49, |J. Appl 23. Jean-Y Sensitiv |

|7. R. Matick, et. al. , “Logic Rationale for Use”, IBM J. pp. 145-165, Jan. , 2005 |Based eDRAM: Origins Research Dev., vol. |and 49, no. 1, |Oxide Reliabi 24. R. Palm |

|8. M. Kumar, et al., IEDM |2003, pp. 419-422, |December ||

|2003 ||||

|9. J. Amon, et al., IEDM 2004, |pp. 73-76, December |2004 ||

|10. W. Mueller, et al. , |VLSI-TSA 2006 |||

|11. D. Weiss, et al., “ The On-chip Third-Level Cache on an ISSCC Dig. Tech. Papers, pp.112-113, |3-MB Itanium 2002 |Subarray-Based Microprocessor,” |RCA R 26. T.Kane 30nm |

|12. J. Barth, et al., “A 500 MHz DRAM Macro with Direct |Muti-Banked Write and |Compilable Programmable |Novem |

|Pipeline,” ISSCC Dig. Feb.,2004 13. T. Kirihata, et al., “An 800 a Concurrent Refresh Mode, pp. 206-207, Feb.,2004 14. J. Clabes, et al.,”Design Power5 Micro Processor,” 56-57, Feb.,2004 15. H. Pilo, et al., “A 5.6-ns with 1.4Gb/s/pin and DDR3 |Tech. Papers, MHz “ ISSCC Dig. and ISSCC Dig. Random Cycle SRAM |Tech. Papers, MHz “ ISSCC Dig. and ISSCC Dig. Random Cycle SRAM |pp. 204-205, Embedded DRAM with Tech. Papers, Implementation of the Tech. Papers, pp. 144-Mb DRAM Interface”, IEEE J. |

|2003 16. S. Doering, “CB-CB-short und Zuverlässigkeit Fehlermechanismen, Grainau 17. A.N. Erickson, “Gate Fault Characterization Through Probing,” Proceedings of 42nd 18. E.H. Nicollian, J.R. Brews, Semiconductor) Physics and pp. 384-385, (1984) |presentation”: integrierter 2006 Localization the Use of  IRPS, 2004, MOS Technology, |presentation”: integrierter 2006 Localization the Use of  IRPS, 2004, MOS Technology, |FW: Qualität Schaltungen: and Parametric Atomic Force pp. 617-618 (Metal Oxide “C-V Curves, |

|19. K. Ramanujachar, Transistor Contact |Scanning Capacitance Level, Proc. of |Scanning Capacitance Level, Proc. of |Microscopy at International |

22. T. Ishida, et. al. Microscopic C-V Measurements of SOI  Wafers by Scanning Capacitance Microscopy, Eur. Phys. . Phys. 27, 479-482 (2004).


ves Rosaye, et. al. C-V and C-P Characterization  ities for Fast and Slow-State Traps in Very Thin  MOSFETS, Proceedings of International  lity Physics Symposium, pp. 353-351 (2004).


er, E.J. Denlinger, and H. Kawamoto, CapacitivePickup Circuitry for VideoDiscs, RCA Review, v. 43, March 1982, pp. 194+ (1982)


25. J.K. Clemens, Capacitive Pickup and the Buried  Subcarrier Encoding System for the RCA VideoDisc, eview, March 1978, v. 39, n.1., pp. 33-59 (1978) , M.P. Tenney, “Electrical Characterization of subGatelength SOI MOSFETs”, ISTFA 2004, ber 2004


Alternating Plane-View and Cross-Section Scanning Capacitance  Microscope Technique to Reveal Various Implant Issue


Tsan-Chang Chuang, Cha-Ming Shen, Shi-Chen Lin , Chen-May Huang, Jin-Hong Chou, Jon C.Lee  Taiwan Semiconductor Manufacture Company, Ltd., Taiwan


1,Nan-Ke N, Rd., Tainan Science Park, Tainan, Taiwan 741-44, R.O.C.


Phone: 886-6-5056688Ext.7062149   Fax: 886-6-5052007   Email: Chuangtc@tsmc.com


INTRODUCTION


The International Technology Roadmap for  Semiconductors identifies quantitative two-dimensional (2-D) and three-dimensional (3-D) dopant profiling as being  essential for the advancement of future generations of the  semiconductor technology [1]. Currently scanning capacitance  microscopy (SCM) is a 2-D carrier and/or dopant  concentration profiling technique under development that  utilizes the excellent spatial resolution of scanning probe  microscopy [2], [3]. It is based on the MOS characteristics  between the scanning probe and the substrate and is regarded  as having great potential for quantitative 2-D dopant  concentration profiling [3], [4], and related framework  diagram was shown as Fig-1.


Laser


Photo


detector


Conductive Probe


Semiconductor Sample


UHF ResonanCap Measuremen Chuck


Cap SensorElectronics


X-Y Stage


Sample Bias Voltage


Fig-1: Scanning Capacitance Microscopy (SCM) framework Diagram with signal measurement and process  unit.


As known to all, UHF resonant capacitance sensor is the  basis of the capacitance detection. The resonator connects to a  conductive probe via a transmission line. When the  electrically resonating probe tip contacts a semiconductor, the  sensor, the transmission line, probe and sample all become  part of the resonator. Generally speaking, whole system is  sensitive to variations as small as attofarads (10-22 F/√Hz  sensitivity) [5]. And that is to say, majority-carrier depth that  resonant capacitance sensor sensed is just ~ 4 lattice width. For failure analysis point of view, we need accurately localize  defect position to near angstrom level for the purpose of  making X-SCM analysis. Unfortunately, failure site localized  indications such as, EMMI, OBIRCH, TIVA have insufficient  capability to provide such precise position for X-SCM  analysis especially at extensive zone. Besides, related to PVSCM (Plane-View SCM), once the implant related defect was  revealed by VC(voltage contrast), C-AFM(ConductiveAtomic Force Microscope) or NP (Nano-Probing), further


action has to take to confirm the failure mode. PV-SCM has  limited capability to achieve the goal due to inherent “plane” trait. On top of that, deeper concentration profile just like  DNW is also one of restrictions to use.


For representing above contents more clearly, the following  cases would demonstrate the alternated and optimized  application of PV-SCM and X-SCM.


Case-1 Study:  JTAG Failure


A new tape out product was suffered zero yield, 90% dies  failed in JTAG  (Joint Test Action Group) test. Then JTAG  failure dice was picked for failure analysis, and a significant  signal was detected at periphery circuit by IR-OBIRCH  technique, as shown in Fig 2.


Figure 2: Dice with JTAG failure was detected a significant  signal by IR-OBIRCH technique.


Brighter SEM PVC (passive voltage contrast) than normal  was revealed, then current imaging and I-V curve using CAFM were extracted, shown as Fig 3(a), (b)  [6].


 curve using CAFM were extracted, shown as Fig 3(a), (b)  [6].


|Ref Ref |P+ P+ |F5|Failu P+ |
|---|---|---|---|

(a) C-AFM Current Imaging


re


-Failure P+-Ref P+


n+


P-well


Figure 3: (a) Current imaging showed P+ column contacts  suffered high reserve saturation leakage under the same OD  with salicide process. (b) I-V curve measured by C-AFM  showed smaller cut-in voltage and large reverse saturation  current than reference for all leakage column P+ contacts.


Current imaging showed P+ column contacts suffered high  reserve saturation leakage under the same OD with salicide  process. I-V curve measured by C-AFM showed smaller cut-in  voltage and large reverse saturation current than reference. Because  the OBIRCH signal at huge protection diode area is wild  enough, the follow up analysis is difficult to make judgment.


No physical abnormality could be found in this area even  use wet chemical stain or TEM. The failure mechanism still  not identified through conventional methods. X-SCM was  chosen to make analysis and got nothing exceptional at  localized wide site, shown as Fig 4.


Figure 4: Although X-SCM technique was chosen to make  analysis, SCM got nothing exceptional at localized site. That  is to say, these kinds of defects couldn’t be revealed by X-view.


Instead, for solving this issue, PV-SCM, shown as Fig 5, was applied to voyage at localized huge area and less P+ species per cubic was founded, shown as Fig 6.


(b) I-V curve measured by C-AFM


bias


Fig-5: Sketch map showed the extraction of SCM imaging. Before SCM measurement started, an oxide re-grown over the  sample.


(a) SCM mapping along the specific column of located


P+/NW area


(b) Quantification analysis at revealed failure site


Figure 6: (a) An abnormality was revealed by SCM  mapping along the specific row of located P+/NW area (b) The missed implantation issue was verified by the advanced  quantification analysis of SCM signal at suspected spot.


Because failure dice has strong correlation with Fab in-line  specific photo instrument, the failure mechanism should  attribute to the weakness of related machine.


Case-2 Study:  Stand-by Failure


From stand-by failure dice, A non-direct short between  specific failed pins was revealed through electrical failure  analysis, shown as Fig.7.


Located spot site


Extraordinary  concentration


Figure 7: The failure die suffered stand-by failure was  revealed a significant VDD to AVDD non-direct short  phenomenon through electrical failure analysis.


The failure die was detected a significant signal by IROBIRCH technique and well leakage was suspected, as shown  in Fig 8.


DNW


6 N


Figure 8: Momentous signal was detected at protection  diode circuit region by IR-OBIRCH technique and well-towell leakage was suspected.


No physical abnormality could be found in this area even  using chemical stain, SEM layer-by-layer observation, FIB  cross-sectional inspection or TEM analysis. The failure  mechanism was still not identified through these methods. So  SCM technique was chosen to make further analysis. According to our hypothesis, PV-SCM apparently lacks  strength to do this kind of analysis due to deep-end area from  si surface. X-SCM imaging was extracted, shown as Fig.9, and obviously DNW (Deep N-well) encroached to outside  NW laterally was revealed.


|Failure sample |Failure sample |Failure sample |Failure sample |Failure sample |Failure sample |Failure sample |
|---|---|---|---|---|---|---|

|a as|10|20|25|80|35|4|

|Passed sample |Passed sample |Passed sample |Passed sample |Passed sample |Passed sample |Passed sample |

Distance


P-sub


(b) X-SCM imaging


Figure 9: (a) Layout and X-view (b) Obviously DNW  encroached to outside NW laterally was revealed. From the  occurrence of isotropic extended DNW, it implied that excess  thermal budget leading to such kind of non-direct short  leakage.


Failure mode like that, isotropic extend of DNW, implied  that excess thermal budget leading to such kind of non-direct  short leakage should be the root cause.


Simulation also gave its approval for our inference. DNW  with updated recipe showed less lateral diffusion due to lower  thermal budget. Furthermore, related to DNW depth, SCM has  about 25% difference between TCAD simulator and SCM


technique, shown as Fig. 10.


Extraordinary spot


NWPW


Former recipe


Updated recipe


Figure 10: DNW with updated recipe showed less lateral  diffusion due to lower thermal budget. Furthermore, related  to DNW depth, SCM has about 25% difference between TCAD  simulator and SCM technique.


CONCLUSIONS


These cases illustrates that correct selection from either  plane-view or cross-sectional SCM analysis according to the  surrounding of defect could help to exactly and rapidly  diagnose the failure mechanism. X-SCM could make vertical  profile analysis but it need precise defect position just like  clockwork. PV-SCM could navigate at suspected area and  efficiently reveal defect to reduce FA cycle time. But it could  not provide deeper implant information due to the “plane” by  birth. Alternating and optimizing PV-SCM and X-SCM  techniques to navigate various implant issue could provide  corrective actions that suit local circumstance of defects and  identify the root cause.


|PW||N+ NW|PW NW|
|---|---|---|---|

|DNW|DNW|DNW|Distance |

Figure 11: CtS on n-FET (left) - with FIB pads (right)


To allow a first proof of concept without the use of AFP, minimized FIB pads were deposited (right part of Figure 11) and a regular probe station could be used. The measured  output characteristic of n-FET (2) is shown in Figure 12. For  this measurement, the source contact Y was kept on ground  potential and the second n-FET (1) could be used to block any  possible current through the rest of the circuitry. Therefore  gate 1 was also constantly connected to ground, enforcing nFET (1) to remain in the off-state.


FIB[nm]-500 50[nA]-10 0 10


0.5VDS[V]1.0


Figure 12: n-FET output characteristic measured with FIB


F


pads and a regular probe station (gate width- Wg =730nm,


←


and gate length- Lg =160nm )


!I


The plotted output characteristic indicates the presence of a 2μmvery high series resistance (>> 1k) in the drain - source  connection. This resistance is a summation of the two CtS


formations, the platinum lines leading to the FIB pads (Lshaped Pt depositions) and the needle contact resistance.


These results show, that single transistor characterization is


generally possible from the chip backside, leaving the full


circuitry intact, but to gain more precise results, the series


contact resistance has to be drastically reduced.


Measurements using AFP


To reduce the overall contact resistance another set of purely ohmic contact with less than 400Q each (60.Qum2 with measurements was carried out using a Multiprobe AFP


(Infineon PFA, Munich, Germany). The tool works with 4


heads and offers various scanning modes (contact & tapping


mode, current mapping…). To allow AFP measurements, the


DUTs had to be prepared with minimum surface topology. To


accomplish this, the whole area of interest was thinned down


to the STI level, revealing all 10 divider stages of the RO


AFP Needles


400


used. Figure 13 shows a FIB image of the thinned area.


[μA]200


mhmmm W"Cosi"


---Pa-e ---e


2223


-400


AV/△l≈750Q-0.3-0.20.00.2 [V] 0.3


64μm--


0M1


Figure 13: FIB image of oversized STI opening with marked  AFP measurement location


Note that the RO output frequency was monitored throughout  the full FIB procedure and did not change overall by more  than 3%.


The first step to do an AFP measurement is to do a coarse  optical alignment, placing all needles above the area of  interest. After that, the AFP needles are scanned across the  sample surface to precisely locate the targeted measurement  area. Figure 14 shows a topography image (middle part) of the  exact same area as the FIB image on the left. The created Pt  contacts are only 50nm higher than the Si or STI surface. This


VGs[V]


is due to a reduced Pt deposition (0.6x0.03μm2, 10s, 1pA),


[μA]n-FET (2) with G1= 0V const.+0


forming the CtS. The right part of the image shows a current


*0.2


80Drain =X


-*- 0.4


mapping of the same area. To acquire this image, a negative


Source=Y


*0.6


DC bias of -0.5V was applied to the scanning needle and only


60Gate = G2


*0.8-1.0


the conducting Pt material is visible. In combination with the


-+1.2


topology image, this offers a very secure identification of the


contacts and sufficient placement accuracy for the  measurements.


20


very high series resistance (>> 1kΩ) in the drain - source


topology-AFP-current


Figure 14: left) enlarged FIB image, arrows indicate CtS  locations  middle) AFP topography image-  right) AFP  current image- of the same area


To directly measure the pure contact resistance of the AFP in  combination with the FIB prepared Pt contacts, measurements  were first done on various CtS, all short circuited via direct  M1 connection. Results are shown in Figure 15. These  measurements prove the formation of a reproducible and  purely ohmic contact with less than 400 each (60μm2 with  the used contact size of 0.8x0.2μm2). Compared to frontside  AFP, where the tungsten needle is directly placed on the  tungsten plug, the CtS resistance is around 8 times higher, but  still acceptable for any measurement on small, hence high  ohmic transistors (gate width < 1μm).


Figure 15: calibration measurement using AFP on two CtS


For bigger transistors (power devices) the CtS size can be  increased, reducing the resistance in direct proportion.


Frontside AFP always contacts only one tungsten plug per  terminal, which can become a problem due to the increased  current density on power devices.


The intact circuitry during backside device characterization is  not only an advantage but also a limitation: In case of a simple  inverter, as shown in Figure 16, there is no way to measure  one transistor without the other interfering. To allow separate  measurements, the common drain node was cut and two CtS  were formed on the drain areas. The connection to source  could be done by any CtS on Vdd or Vss for the p- or n-FET  respectively.


Figure 16: layout of CMOS inverter with labeled  measurement points and cut location


Due to the cut, the modified divider stage stopped working  and the monitored RO output frequency dropped to zero. But  if necessary, the former connection could be reestablished  with only one Pt deposition in less than a minute of work (in  contrary to the frontside parallel polishing process), using the  two drain CtS after the AFP measurements.


Figure 17: n- & p-FET output characteristics, by use of CtS  and backside AFP ( Wg = 730nm  Lg = 160nm  )


The captured output characteristics of the n- and p-FET are  shown in Figure 17, respectively. The n-FET has a calculated  on-resistance of approximately 6k, indicating that the  influence of the 400 contact resistance can be neglected.


The general functionality of a new backside circuit edit  procedure named Contact to Silicide (CtS) is shown, enabling  the probing to inner circuit nodes and single transistor  characterization.


For probing, this method offers direct contact to every  silicided area on the chip, including every CMOS output. Due  to the extremely small contact sizes and the absence of FIB  pads, the additional load put to the targeted transistor can  almost be neglected. First measurements using simple active  probe tips on 120nm RO test chips allowed direct probing into  the 100MHz region. With the proposed high bandwidth setup, combining automated test equipment with state of the art  active probes, direct measurements in the GHz range seem to  be possible.


In terms of single device characterization, most established  methods are destructive to the circuitry because the physical  top down preparation requires full removal of the metal frontend. With the use of multiple CtS in combination with  backside atomic force probing, DC characterization of single  transistors becomes possible within a functioning circuitry. The measured contact resistance of the CtS AFP combination  was below 400 (with a CtS area of 800x200nm2), which is  in the same order of magnitude as frontside AFP. This value  scales directly with the contact size, allowing better  connectivity on bigger devices.


Since most state of the art localization techniques are applied  through the thinned bulk Si, the backside analysis  methodologies presented in this work could be very valuable  additional options to allow a full flow of localization, probing  and root cause analysis from the chip backside. Unlike usual  FA procedures the DUT can stay fully functional until the  very end. This allows the FA worker to alternate between high  speed probing and DC characterization.


Special thanks to Infineon PFA Dresden for providing the  test- structures and Credence Systems Corporation for general  support of FIB backside processing.


[1] M.A. Thompson, C. Richardson, E. Le Roy, T. Lundquist and  W.B. Thompson “Coaxial, Photon-Ion Technology Enables  Direct Navigation to Buried Nodes on Planarized Surfaces, including Silicon”  Proc. 28th ISTFA (2002) 409


[2] R. Schlangen, U. Kerst, A. Kabakow, C. Boit     ”Electrical


Performance Evaluation of FIB Edited Circuits through Chip  Backside Exposing Shallow Trench Isolations”


Proc. 16th ESREF (2005) 1544


[3] C. Boit, U. Kerst, R. Schlangen, A. Kabakow, E. Le Roy, T.R. Lundquist, S. Pauthner ”Impact of Backside Circuit Edit on  Active Device Performance in Bulk Silicon ICs”


Proc. 37th ITC (2004) 48.2


[4] R. Schlangen, P. Sadewater, U. Kerst, C. Boit “Contact to


Contacts or Silicide by use of Backside FIB Circuit Edit


allowing to approach every Active Circuit Node”


Proc. 17th ESREF (2006) 1498


[5] M.F. Bailon, P.F. Salinas, J.S. Arboleda, "Application of


Conductive AFM on the Electrical Characterization of


Single-bit Marginal Failure"


Proc. 12th IPFA (2005) 282


[6] M. Grützner, "Advanced electrical analysis of embedded


memory cells using Atomic Force Probing",


Microelectronics Reliability 45


Proc. 16th ESREF (2005) 1509


Deposition of Narrow, High Quality, Closely Spaced, but Isolated Conductors


V.V.Makarov and R.K. Jain


Credence Systems Corp., 1421 California Circle, Milpitas, CA 94035


Developed procedures to deposit narrow (<100nm), closely  spaced, low resistance conductors which exhibit good  electrical isolation are demonstrated.  The process parameters  which limit how narrow a line can be deposited and the   methods used to work-around these are discussed.  For these  depositions, 3pA ion beam current was used with a Mo(CO)6  precursor chemistry. The deposition method minimized the  incorporation of non-conductive precursor by-products. To  isolate adjacent conductors, a copper etch Credence FIB  chemistry was used. The advantages of this procedure over the  common practice when XeF2 chemistry is used is also  discussed and demonstrated.


During some process characterizations such as nano-probing  of memory cells, a probe structure is created (Fig. 1a)  [1].  This structure consists of high quality dielectric, low  resistance vias and conductors connecting transistor elements  to probing pads. This characterization activity measures I-V  curves of cell transistors, which requires operating current (~200µA) through the deposited conductors. This operating  current requires not only low resistance conductors but with  small dimensions for instance those required for < 90nm  process technologies these conductors must also be narrow  and minimally spaced (< 100nm).  This creates a significant  challenge during the deposition over-spray clean-up step that  is necessary to obtain electrically isolated conductors. These  narrow, high quality, closely spaced but isolated conductors  are also important in TeraHz detectors (Fig. 1b)  [2].


Figure  1a


3un


Figure 1b


Figure 1a: FIB micrograph of “wagon wheel” structure used  to probe SRAM cells for process characterization. Figure.1b: TeraHz detector structure.  Both structures require deposition  of narrow, high quality, closely spaced, but isolated  conductors.


In this work, we demonstrate the use of Mo(CO)6 for FIB  deposition of thin, high quality, narrowly spaced isolated  conductors.  To minimize lateral broadening of the conductor  lines, a one pixel wide line scan (OLS) FIB operation was  applied. This approach allows a reduction of the width of the  deposition down to the natural limit defined (in general) by  the beam spot size and precursor activation area diameter for  the given precursor at a given substrate. This OLS approach  also simplifies control over deposited conductor quality (conductivity). The primary quality control factor is  deposition yield which was controlled with the beam scan  speed.  We were able to optimize the process parameters very  close to those when deposition turns into etching, however the  deposition mechanism still dominated over etching.  Further, we compare quality and geometry of thin conductors  deposited under these conditions with those which were  deposited when the deposition was highly dominating over  etching. We offer a recipe for over-spray removal after  conductor deposition which allows isolation of narrowly  spaced conductors from each other without damage to the  dielectric in between the conductors. We compare this recipe


0话


with the common practice when the over-spray is removed  using XeF2 chemistry.


All the experiments were performed on a Credence P3X FIB  Circuit Edit system. Thin conductors were deposited using  3pA beam current (collimated mode) on the SiO2 substrate in  between Aluminum traces that are connected to an external  pin out to perform resistance measurements. To avoid high


contribution of the contact resistance between Al traces and  deposited conductors, Al traces were thinned down to ~0.2um  using FIB chemically enhanced Al etch with Iodine containing  chemistry, Ethylene Di-Iodide. After each conductor was  deposited its resistance was measured and then the conductor  was cut, so that next conductor could be deposited and  measured.  After the set of conductors was deposited, it was  covered with FIB deposited insulator and cross-sectioned to  view the conductor’s cross-sections.


μm


Beam Scan Control


The correlation between resistivity and deposition yield, when  conductor is deposited using FIB technology, is a wellestablished dependence [3, 4]. The best conductor material is  deposited at ion doses, which are close to but still lower than  the limit where deposition turns into etching. So, good  material deposition correlates with low deposition yield. Normally this means slow scan speeds since the lower the  scan speed the higher the ion dose per line. Indeed, the ion  dose delivered during each line scan for a given current I is  equal to I ×τ×n/Lφ , where τ is dwell time, n is number of  pixels in the line, φ is the beam diameter and L is the line  length.  Obviously, for a given current, I and φ may be  considered as constant parameters. It is convenient, therefore, for a given current, to use the value τ ×n/L as a measure of the  ion dose delivered to the line. One can see that the value τ ×n/L represents scan time per line length which actually is a  reciprocal beam scan speed 1/υ. Therefore,  the beam scan  speed can be used as a metric of the deposition conditions.


Scanning along a line the ion beam interacts with the  precursor collected on the surface. The amount of the  precursor in the spot depends on the time elapsed since the  previous visit of the spot by the beam. The ion beam  dissociates the precursor chemistry creating a volatile and a  non-volatile (deposited) byproduct. The precursor amount and  ion dose must be in a balance. If the ion dose is too high, the  precursor is “over-consumed” and one starts to see overetching in the area of the deposition. For the OLS scan scheme  the revisiting time is coincident with the retrace time.  Normally the time dependence of the precursor amount on the  surface may be well approximated by the form [5], A×[1 – exp(-t/τ)], where A is a parameter proportional to the gas  pressure and its residence time τ on the substrate. This  dependence demonstrates steady state coverage of the surface  with a precursor at times t exceeding approximately 3τ. Using  the OLS approach for deposition of Molybdenum lines (with  Mo(CO)6 precursor) with variable length, we found scan  speeds for different currents at which deposition was turning  into over-etch for various retrace times.  These dependencies  for the beam currents of 50pA and 1nA are shown in Fig.2.  Quite naturally these dependencies were successfully  approximated with the form (above) describing the collection  of the precursor on the surface.  This shows that the ion dose  can be used as a metric of the surface coverage with precursor.  We designate as (1/υ)max the reciprocal scan speed at which  one starts to see signs of an over-etch.


The results shown in Fig.2 allowed us to determine the  minimal retrace time at which the surface coverage could be


considered as a steady one.  This number turned out to be ~750us.  In all further experiments the retrace times were set  to be no less than 750us.


500


1500


2000


Time of Scan.Max per


50 100 150 200 250


Approximation (dotted lines):1/υ = A[1 - exp(-t/τ )],   τ  = 250µs


µS/µ


Saturation area


(1/υ)max


(I = 1nA) x 8(I = 50pA) x 1


Retrace time (µs)


Figure 2. Dependencies of the reciprocal scan speed at which  one starts to see signs of over-etching when depositing Mo  using Mo(CO)6 precursor with beam currents 50pA and 1nA. Approximation with an analytical form is shown with dotted  lines.


With the high beam currents (50pA and higher) the  experiments were done with the precursor pressure within the  working area ~0.1 torr.


For deposition of thin conductors, a collimated ion beam with  3pA current was used. With this current, under normal  pressure, even with steady positioning of the beam on the  sample surface (zero scanning speed), no over-etch was  observed, a pillar was created instead. This can be explained  by an additional mechanism of precursor replenishment when  low current is used. If the beam spot size and, accordingly, the  spot size of precursor activation area  become small if  compared to the surface diffusion length, the precursor  replenishment may occur not only by the gas arriving directly  from the nozzle, but also by surface diffusion from the area  surrounding the working spot. This means that the  replenishment in this case goes faster. With the reduced  pressure, surface coverage with the precursor and, accordingly, diffusion rate would be reduced. So, to find  conditions where the deposition started to turn into etching, the precursor pressure was reduced in the working area  approximately six times by reducing the gas flux from the  nozzle and moving the nozzle further out of surface. The  constraint of a minimal 750uS retrace time was still applied in  the experiments with 3pA current.


Results and Discussion


Search for a scan speed which provides a minimal advantage  of deposition over etching at lowered pressure of the precursor  gave a number (1/υ)max = 820uS/um.


In Fig.3 one can see the cross-section of a Mo line deposited


at a lowered pressure of Mo(CO)6 precursor at the scan speed -25nm of 820uS/um when 1/υ = (1/υ)max..   In Fig. 4 the precursor


pressure is slightly higher and the scan speed is 1024uS/um.


Over-etching is just beginning at the slower scan speed of


个


820uS/um where it is approximately 6nm deep and becomes  significantly greater at the higher scan speed of 1024uS/um.


240000x 10.00kV5.1mm 52°11:19:29AM


#1


Figure 3. Cross-section of Mo line deposited in 6 minutes at a  lowered pressure of Mo(CO)6 precursor and a scan speed  when 1/υ = (1/υ)max = 820µS/um. A slight over etch of about  6nm can be observed.


|Time (min) |Width (nm) |Height (nm) |Resistance (Ohm) |Resistivity (µOhm-cm) |
|---|---|---|---|---|

|1 |46 |28 |1.56x109 |9.42x104 |

|2 |62 |33 |14.37x103 |138 |

|4 |77 |42 |9.67x103 |147 |

|8 |118 |71 |3.57x103 |147|

|8 |118 |71 |3.57x103 |140 |

To characterize the rate of the deposition at lowered precursor  pressures, a matrix of varying deposition times was  performed. The matrix included  1, 2, 4 and 8 minute  deposition times. The one pixel wide line scan (OLS) beam  scanning was applied.  The length of the deposited conductors  was 20µm with 2µm of each end being used to contact the Al  traces, so the resistor length was 16um. Resistance was  measured for each deposition. To make sure that no overetching and, accordingly, no mixing with dielectric material  was involved into conductor formation, the scan speed was  increased in such a way that 1/υ = 0.75 x (1/υ)max = 650µS/um.   The results are listed in Table 1, they include the  width, height, resistance and calculated resistivity for each of  the deposited conductors.


magHVWDt8J712007


400nm


239 999 x 10.00 kv 5.1 mm| 52* 11:12:10AM


#3


Figure 4. Cross-section of Mo line deposited in 6 minutes at a  lowered pressure of Mo(CO)6 precursor and  a scan speed  when 1/  1.25 x (1/)max = 1024S/um.  The over-etch 1.25 x(1/ )max = 1024 S/um. The over-etch increases significantly up to approximately 25nm.


Similar data, for the conductors deposited at the standard  precursor pressure are presented in Table 2 for comparison.   Since the cross-sections of the conductors showed a semielliptical form, a factor pi/4 was applied in calculation of the


magHVWDtilt8/7/2007


400 nm


cross-section areas.


Table 1. Results of Mo conductors deposition using 3pA beam  current at lowered pressure, with beam scan parameter 1/υ =


0.75 x (1/υ)max = 650uS/um


Table 2. Results of Mo conductors deposition using 3pA beam  current at standard pressure, with beam scan parameter 1/υ = 650uS/um. Comparison with (1/υ)max  is not  applicable.


|1 |78 |33 |1.31x104 |167 |

|2 |126 |49 |5.69x103 |165 |

|4 |196 |94 |2.33x103 |165|

|4 |196 |94 |2.33x103 |201 |

|8 |n/a |n/a |n/a |201 n/a|

n/a


Conductors deposited at lower pressure and under conditions  where the balance between ion dose rate and precursor  amount on the surface was close to the over-etching limit, exhibit a significantly more subtle geometry and noticeably  lower resistivities. One conductor which was deposited during  a one minute deposition time and at lowered precursor  pressure measured anomalously high resistance/resistivity.


This is definitely related to the structure of the conductor.  Obviously, one minute of deposition time was not enough to  create a continuous conductor.  In figure 5 one can see a  fractured structure of the line which probably relates to  creation of the so-called transition layer [6].  Another factor  which is also evident in figure 5 and may contribute to the  results we obtained at lowered precursor pressure is step  coverage. The Al step height, though reduced from its original  thickness of 0.5um down to 0.2 um, was still too high for the  lines with subtle geometry. The step reduction was stopped at


0.2um because of massive protrusions in the residual Al which  started to show up at this level. Further continuation of the  thinning process could create floating islands of Al, which  would affect the results even more. Therefore, resistance and  resistivity numbers in Table 1 apparently still contain some  unknown contribution from the poor step coverage in the  contact regions. This component should be present also in the  data related to the conductors deposited at standard pressure, but its contribution may be not as high because of the  significantly thicker geometry of these conductors.


Figure 5. Fragments of two conductor depositions performed  at lowered precursor pressure. Two minute deposition time on  the left. One minute deposition time on the right. Note the  fractured structure of the conductor on the right.  Note the  lower part of the picture appears blurred because of the FIB  insulator deposition over- spray. This insulator deposition  was used for further processing of the line set.


Isolation of closely spaced conductors


Normally the requirement for small geometry conductors also  requires tight spacing between the conductors. The conductor


AMER 5.0KV x80.0k 6/21/2006


'500nm. .


deposition process is always accompanied by the over-spray  caused by the tails of the ion beam.  The over-spray has a  significant conductivity and may cause inadvertent electrical  shorting of the conductors that are supposed to be isolated.  Therefore cleaning of the over-spray is an inevitable part of  the conductor deposition process.  Common practice for the  over-spray cleaning is the use of a very efficient but very  aggressive XeF2 gas assisted etching chemistry.


In this work, we offer that for the over-spray cleaning  purpose, one needs to use an oxidizing chemistry that does not


enhance the dielectric removal but instead protects it from  deterioration by the ion beam. Simultaneously, this chemistry  must work as an efficient oxidizer that can neutralize electrical  conductivity of the over-spray.  A good example of this type  of chemistry is CU2, a Credence copper etch solution known  for its dielectric protection qualities.  In figure 6 we illustrate  the advantage of the use of CU2 instead of XeF2 for cleaning  the over-spray film connecting two adjacent and very close  Mo conductors. Because of a high aggressiveness of XeF2  gas  assisted etching, one cannot avoid damage to the dielectric in  between two conductors when using this chemistry (Fig. 6a).  In contrast to this, CU2 allows transfer of the conductive  deposition overspray material into a nonconductive material in  between the Mo lines with no visible damage to the dielectric (Figure 6b).


AMER 5.0kV x80.0k 6/21/2006


'500nm


Figure 6 a


EAG 5.0kV x30.0k


1.00um


Figure 6 b


Figure 6: (a) SEM micro-graph of narrow Mo lines isolated  from each other using XeF2 (b) SEM micrograph of narrow  Mo conductors isolated using chemistry for etching copper. Note negligible damage to the FIB deposited SiO2 dielectric  when copper etch chemistry protects it.


We also demonstrate the isolation of two closely spaced (~0.2um) Mo conductors using CU2 chemistry by means of


secondary electron emission contrast when one of the  disconnected conductors was floating.


gnu


Figure 7 a


Sun


Figure 7 b


Figure 7: FIB micrographs of (a) successful clean-up of space  between neighboring conductors using a copper etch FIB  chemistry with a mill box 8 x 0.2 µm (white mill box) at 50pA  for < 1min, and of (b) same lines with left trace floating to  show isolation. Voltage contrast indicates a very high  isolation resistance (> 1GOhm) [8]. Note, two red mill boxes  were used for the depositions.


1. In this work it is demonstrated that an enhancement  to the quality of Mo conductors deposited with FIB is  possible using ion beam scan speed as the main  control factor. It is shown that lower resistivity of the  conductor can be achieved when the deposition  process approaches so-called depletion mode and the  deposition mechanism has only slight advantage over  sputtering.


2. The other advantage of conductor deposition under  this conditions is very subtle line geometry allowing  to obtain width of a continuous line below 100nm if  beam current ~3pA is used


3. Faster thin conductor deposition using 3pA and  Mo(CO)6 can be done under conditions far from  depletion in cases where 200nm geometry and  resistivity on the level of ~200µOhmcm are  acceptable.


4. A successful isolation of tightly spaced conductors  using Credence copper-etch solution CU2 to remove  deposition over-spray, was demonstrated. Compared  to the normal practice where XeF2 is used, this  approach allows oxidizing the over-spray to a nonconductive state with no damage to the dielectric.


[1] Joseph Myers et al., “Novel Approach for  Enhancing Critical FIB Imaging for Failure  Analysis and Circuit Edit Applications”, ASMISTFA (2004) 151.


[2] R.Mendis et al., “Coherent generation and  detection of continuous THz waves using two  photomixers driven by laser diodes”, IEEE-Int. Conf. on Terahertz Electronics (2004) 200.


[3] T.Tao, W.Wilkinson, and J.Melngailis, “Focused  ion beam induced deposition of platinum for  repair processes”J. Vac. Sci. Technol. B 9(1)


(1991) 162.


[4] J.Puretz and L.W.Swanson, “Focused ion beam  deposition of Pt containing films”J. Vac. Sci. Technol. B 10(6) (1992), 2695.


[5] L.R.Harriott “Digital scan model for focused ion  beam induced gas etching”J. Vac. Sci. Technol. B 11(6) (1993) 2012


[6] H.Langfischer, B.Basnar, H.Hutter and  E.Bertagnolli, Evolution of tungsten film  deposition induced by focused ion beam” J. Vac. Sci. Technol. A 20 (2002) 1408


[7] V.V.Makarov and T.R.Lundquist, “FIB Milling  of Copper over Organic Dielectrics”, US Patent  No 7,060,196 (2006).


[8] C.R. Musil, J.L. Bartelt, and J. Melngailis, “Focused Ion Beam Microsurgery for  Electronics”, IEEE Electron Device Lett EDL-7


(1986) 285.


Challenges of Atomic Force Probe Characterization of Logic Based Embedded  DRAM for On-Processor Applications


Terence Kane, Michael P. Tenney,


IBM Systems and Technology Group, Hopewell Junction, New York


Andrew Erickson, Sebastien Phan


Multiprobe, Inc. Santa Barbara, California


Nanoprobing logic based SOI embedded DRAM cells for onprocessor designs poses different challenges than probing  conventional six transistor SRAM designs. This paper will  describe nanoprobing logic based embedded DRAM (eDRAM) cells in 65nm SOI applications. We will also  describe probe placement and measurement methodology for  electrical characterization of  leakage between deep trench  capacitors composing those eDRAM designs. The introduction  of nano CV metrology and scanning capacitance imaging for  use in characterizing DRAM capacitors will also be discussed.


(a) Layout and X-view


REFERENCES


[1] The International Technology Roadmap for Semiconductors,


Semiconductor Industry Association, San Jose, CA, 2001, p. 16.


[2] P. De Wolf, R. Stephenson, T. Trenkler, T. Clarysse, and T.


Hantschel, “Status and reviewof two-dimensional carrier and  dopant profiling using scanning probe microscopy,” J. Vac. Sci. Technol. B, Condens. Matter, vol. 18, pp. 361–368, 2000.


[3] A. C. Diebold, M. R. Kump, J. J. Kopanski, and D. G. Seiler,


“Characterization of two-dimensional dopant profiles: Status and


review,” J. Vac. Sci. Technol. B, Condens. Matter, vol. 14, pp.


196–201, 1996.


[4] C. C. Williams, “Two-dimensional dopant profiling by scanning  capacitance microscopy,” Annu. Rev. Mater. Sci., vol. 29, pp.


471–504, 1999.


[5] Application notes, Digital Instrument, Veeco Metrology Group.


[6] Jone C Lee, C.H.Chen, David Su, J.H. Chuang, “Investigation of


sensitivity improvement on Passive Voltage Contrast for Defect


Isolation”, ESREF processings (2002)


Sub-Zeptofarad Sensitivity Scanning Capacitance Microscopy Sensor


H. Dongmo, P Hammond and J. Weaver


University of Glasgow, Department of Electronics & Electrical Engineering  Oakfield Avenue, Glasgow, G12 8LT, UK


Scanning Capacitance Microscopy (SCM) is an Atomic Force  Microscopy (AFM) based technique that simultaneously  records topography and local capacitance with high spatial  resolution. This tool is based on the high frequency MOS  capacitor theory, and is routinely used in failure analysis to  discern the 2D carrier profiles and/or defects in insulator  layers of semiconductor devices. An ac voltage induces a  dynamic change in capacitance formed by the SCM tip and  oxidized semiconductor sample surface. Because of the small  contact area, sensitivity of the capacitance measurements must  be lower than 10-18 F in a 1 kHz bandwidth. SCM sensors  capable of such sensitivity are commonly based on the Radio  Corporation of America (RCA) capacitance sensor, and rely  on the detection of the frequency shift of a resonator. High  operating frequency for the resonator significantly improves  the measurement sensitivity. In this article, we describe a  sensor for SCM with sub-zeptofarad (< 10-21 F) sensitivity  based on the designs of Tran et. al., but realized using a phase – sensitive detection system. This results in improved low  frequency noise in the capacitance measurement. This design  has an operating frequency of 3 GHz when unloaded and a  resonator Q around 110, resulting in an improvement of the  system sensitivity over the conventional RCA CED sensor, and may be used in a commercial AFM system. The  performance of this sensor is discussed and two-dimensional  dopant profile from a semiconductor structure is presented. The limitations of bulk resonator SCM systems are discussed  and the prospects for monolithic sensors are described in the  context of a 0.35 µm SiGe BiCMOS process.


The Scanning Capacitance Microscope (SCM) [1, 2] is  routinely used to measure the majority carrier concentration  along the surface of a processed semiconductor sample. Practical SCM systems are usually based on conventional  Atomic Force Microscope (AFM) giving capability to map  topography with high spatial resolution. A conductive tip is  scanned across the oxidized sample surface and small changes  in the tip/sample voltage-dependant capacitance are measured  and used to extract information on the local dopant  concentration and/or discern defects in insulator layers of  semiconductor devices [3-5]. The tip/sample static capacitance  is extremely small (approximately 10-18 F) compared with  undesirable constant stray capacitance (typically 1 pF) and is


very difficult to measure. To overcome this, a dc bias  modulated by a small ac signal is applied to the Metal Oxide  Semiconductor (MOS) capacitor formed by the tip/sample  system, and changes in the MOS capacitance, C in response to  the applied bias, V are measured using a lock-in to give a  direct measure of the gradient dC/dV. An ultra-high  sensitivity capacitance sensor (lower than 10-18 F in a 1 kHz  bandwidth) is required to perform such measurement [6-8]. Most SCM systems derive from the Radio Corporation of  America (RCA) capacitance sensor originally designed for  capacitive-pickup from the CED VideoDisc [1, 9]. The RCA  capacitive pickup employs a form of slope detector, in which  the change in stylus-to-disc capacitance modulates the center  frequency of a transmission-line resonant circuit driven at a  fixed frequency (915 MHz). The operating point of the sensor (tuned using a varactor diode) can be chosen to maximize  sensitivity. The peak-to-peak sense voltage in the RCA sensor  is quite high (up to 10 V), leading to an objectionable  modification of the measured capacitance-voltage (C-V) curve  and significant distortion of images obtained near boundaries  between differently doped regions. The quality factor Q of  RCA CED capacitance sensor incorporated oscillator is of  about 30, and its capacitance detection limit is reported to be  about 5x10-21 F/√Hz under operating conditions.


Tran et al. [6, 7] have previously demonstrated capacitance  sensors with sub-zeptofarad sensitivity using a resonator  structure which is electrically essentially the same as that used  in the current work, at a slightly lower frequency. The  detection scheme used in the work of Tran et al. was based on  slope detection, in which the system is operated at a frequency  just off resonance. Changes in resonant frequency give rise to  an amplitude change in the detected signal. In the present  work, synchronous detection of the phase of the output of the  resonator is performed. In this way, the resonator may be  operated exactly on resonance, and variations due to oscillator  amplitude noise, changes in loaded Q and connector insertion  loss are all suppressed. In addition, the resonator has been  designed to allow incorporation into a commercial scanning  system for ease of use and simple force sensing for  topographic imaging and flying height control.


System Design


The complete SCM sensor incorporates a demodulator (Fig. 1), an RF oscillator and a coupled transmission line resonator. The filtered demodulator output is fed to a Lock-in Amplifier  to extract the dC/dV signal. The detection circuit uses  standard RF components assembled in a ‘direct conversion’ radio receiver scheme instead of conventional diode detector. This has the advantage that the system may be operated on  resonance making it insensitive to variations in oscillator  amplitude or resonator Q, reducing the system noise, especially at low frequencies. The use of synchronous  detection also results in the rejection of out – of – phase  broadband noise components, giving a 3dB improvement in  noise floor. The resonator PCB is designed to fit a Veeco  Dimension 3100 Scanning Probe Microscope (SPM) head. The SPM is used to control the tip-to-sample contact force (contact mode AFM) and also allows simple positioning of the  sample, scanning and data acquisition.


qunjump


Figure 1: Block diagram of demodulator system. O is a low 0cm123


phase-noise oscillator, S is a 3dB power splitter, D is a delay


line, A is an RF amplifier and M is a mixer / phase detector.


Considering the components of the system in detail, the heart


of the capacitance system is the microstrip line resonator (Fig.


2). The compact resonator is designed to fit the Veeco


Dimension 3100 Scanning Probe Dimension (SPM) head. It is


fabricated from lightweight low loss PTFE PCB and has a


symmetric structure allowing either RF port to be used for


input/output. The electrical length is λ/4 at the operating


frequency. The unloaded sensor has a resonant frequency of 3


GHz which was chosen to give an acceptably compact PCB,


avoiding excessive mechanical strain on the AFM scanner


piezo. The resonator was found to have a quality factor (Q) of


110. The increased operating frequency significantly improves


the measurement sensitivity [6, 8] (as sensitivity is inversely


proportional to √bandwidth); the design presented in this


paper has an operating frequency of 2.7 GHz and a Q of 85


once an AFM tip is attached to the end of the resonator. The


AFM tip used is a TiAu coated conductive diamond contact


mode probe mounted on a 13° tilt wedge. The metal coating


reduces the resistance of the probe, but rapidly wears away


from the apex of the tip itself. During operation, the sample  additionally loads the sensor, resulting in a few MHz shift in  the resonator frequency which is readily compensated for by a  small change in oscillator frequency. The oscillator used is an  ultra-low phase noise microwave synthesizer, type Agilent  8257D. This is chosen since phase noise on the synthesizer  appears directly at the output as noise in the capacitance  signal.


The resonator RF output port signal is amplified using a Low  Noise Amplifier (LNA) to correct for resonator insertion loss, and is applied to the mixer RF input for phase detection. The  reference signal for phase detection is derived from the same  oscillator using a power splitter. As the absolute phase shift  between reference and resonator output is undetermined and is  dependent strongly on the frequency and cable lengths used, the delay line connecting the reference to the mixer is chosen  to give approximately 90° phase shift at the mixer. The total  phase shift is finally set to exactly 90° by small adjustments of  oscillator frequency. The use of 90° phase shift at the mixer  gives maximum rate of change of mixer output voltage with  phase and also minimizes sensitivity to amplitude variations.


Figure 2: Photograph of the 3GHz resonator with the  cantilever mounted on a wedge. The design is symmetric, allowing either RF port to be used as an input or output.


In order to extract the dC/dV information from the output  signal, lock-in detection is necessary, as described above. An  AMETEK Signal Recovery Model 7265 DSP dual phase lockin amplifier detects the variation of mixer output with applied  sample modulation voltage.


Sensitivity


The noise level of the system has been characterized. Firstly, the change in output voltage as a function of oscillator  frequency was used to infer the capacitive sensitivity of the  system, based on a normal LC model of the resonant line. Next the noise present at the output of the system was  measured using a SRS SR780 Dynamic Signal Analyzer. The  signal from the mixer was first amplified using a low voltage


O


D


RF port


Cantilever


M


noise non-inverting amplifier (gain = 100) based on a Linear  technology LT1028C low voltage noise op amp to match the  intrinsic voltage noise level of the mixer (a 50 Ω system) to  the analyzer. The system sensitivity under normal operating  conditions was measured to be ΔV/ΔC=246.83 mV/fF. During  noise measurements, the tip is held far from the sample  surface to minimize the resonator load and any microphonic  contributions to the measured noise level. Prior to  measurements, the sense frequency is adjusted to null the  system output. From figure 3 it is seen that the broadband  noise floor has a value of 400 nV in a bandwidth of 256 Hz. This corresponds to a capacitive noise level of 0.62·10-21 F·Hz1/2. The other benefit of the demodulation scheme is a  reduction in the 1/f noise present in the system which has a  noise corner of approximately 800 Hz, as opposed to  approximately 20 kHz for the system of Tran et. al. This is  probably due to the elimination of the large background  carrier amplitude signal which is a necessary feature of a  slope-detector based system. In the current system the voltage  output is approximately zero in the absence of a capacitive  voltage shift, so that amplitude noise (e.g. from the source) is  suppressed. It is noticeable that if the condition of accurate  phase nulling is neglected in the current system then the low  frequency noise increases rapidly. The reduction of low  frequency noise is probably more significant than the modest  reduction in broadband noise floor in practice. The high  frequency noise spurs in the observed signal are attributed to  local electrical interference and are not of any practical  importance (one simply modulates the semiconductor bias at a  different frequency).


1.E-07


1.E-06


Noise voltage spectral density (V/VHz)1.E-05


1.E-04


1.E+02


1.E+03


1.E+04


1.E+05


Frequency (Hz)


Figure 3: Noise voltage spectral density of the instrument. The  system exhibits a low noise corner frequency. The 1/f noise is  better than Tran et al system. The noise spectrum is quite flat  above 1 kHz, thus the choice of a modulation frequency above  that value.


SCM Imaging Acquisition Procedure


High resolution SCM imaging requires a proper sample  preparation. Scanning Capacitance Microscopy is routinely  used as a qualitative analysis tool for failure analysis.


Quantitative two-dimensional doping distribution requires  careful attention to the data acquisition conditions and  processing of the measured values using dedicated  quantification software.


Sample preparation


The preparation of cross-sectioned silicon sample for SCM is  a critical step. The semiconductor structure surface imaged  using our system has been prepared using a standard SCM  preparation method [11-13]. The area of interest has first been  roughly delineated using a fine diamond saw. In order to make  an electrical measurement, a thin layer of TiAu (20nm) has  been evaporated on the sample. Using an epoxy resin, the  specimen has been sandwiched between two dummy quartz  plates and cured at 150 °C for 30 mn. The dummy sample  sandwich is then glued to the polishing machine aluminum  sample holder and cured for another 40mn at 150 °C. The  grinding and polishing of the top surface is carried out using a  rotating platten and diamond films in the following order of  grain size: 15-9-6-1-0.1 µm. In between the different  polishing steps the sample is rinsed in de-ionized water, blown  dry with nitrogen and inspected with an optical microscope. Final polishing is made with colloidal silica for two minutes. The direction of rotation for the final polishing is opposite to  the direction of the grinding. Once the sample is clean, the  native oxide is removed by dipping the sample surface in 1:10  aqueous solution of HF for 10 s. The sample is then rinsed  under running de-ionized water for 30 s. Oxide growth is  performed at 70 °C into hydrogen peroxide for 10 mn. This  oxidation technique results in an oxide thickness of 3-4 nm. The sample is then rinsed and annealed at 120 °C for 20 min. Finally, the sample backside is scratched to expose the TiAu  contact. The sample is then ready to be measured with our  SCM.


Experimental conditions


The present work was performed using a DI3100 AFM with a  laser optical lever detection system. In normal operation, this  laser is focused on the end of the cantilever. In such  configuration, light from this laser floods the region of  interest. This incident light can be a source for generating  excess electron-holes pairs in the semiconductor sample when  the laser energy is above the band gap. Therefore, laser  illumination of the area of interest extremely effects the SCM  measurement [14]. This effect cannot be completely  eliminated in this system, but can be minimized by aligning  the laser further back on the cantilever. The SCM sample  geometry can as well be optimized to reduce the effect of stray  capacitance that could additionally load the sensor and  degrade the measurement as described by Kopanski et al. [15] Images of simultaneously acquired topography and SCM  signal of a semiconductor test structure obtained using the  SCM system are presented in Figure 4.


20.0μm8.0


20.0 jm


Figure 4: 20µmx20µm scans of a semiconductor structure  obtained using the 3 GHz microstrip line resonator. (a) Topography. (b) Simultaneously acquired SCM image.


Towards a monolithic SCM


SCM has a great potential to be the first choice for  quantitative two-dimensional dopant profiling if some of its  weaknesses are addressed. The main experimental limitations  of the technique are the generation of photo carriers by the  stray light from the laser used for AFM force feedback and  stray capacitance which necessitates the use of lock-in  detection, allowing only the measurement of rate of change of  capacitance with applied voltage. The use of a monolithic  capacitive sensor may offer very significant benefits in this  regard. In particular, the use of piezoresistive cantilevers [16] offers a double advantage over the traditional optical beam  deflection technique: Compactness and freedom from light  generation of excess carriers. The use of a compact sensor will  allow the incorporation of the SCM sensor into test equipment  other than conventional AFMs, such as probers. The total  stray capacitance is reduced as the sensor dimensions shrinks. This is potentially an enormous benefit, dramatically reducing  microphonic noise and also potentially allowing the  quasistatic measurement of capacitance. The stray capacitance  to remote objects (such as the experimenter) is approximately  proportional to the total area of the resonant waveguide used. In the case of the system described above (figure 2) this is  approximately 30 mm2. A resonant line in a commercial 0.35 µm BiCMOS process of the type shown in figure 5, with an  operating frequency of approximately 6 GHz has an area  which is approximately 2000 times smaller, resulting in a stray  capacitance to the environment which is decreased by a  similar factor. The operating frequency of the probe is clearly  limited by the expensive nature of CMOS real estate. At 6  GHz operating frequency the required cantilever length fits  easily into a normal die area. Operation at these higher  frequencies would normally be expected to result in a  significant improvement in sensitivity. Unfortunately, the use  of a commercial die fabrication process limits the thickness of  metal and dielectric layers which can be used. The measured  loss of a line realized in the present case is 0.75 dB·mm-1, giving a resonator Q factor of about 3. The increased thermal  noise associated with these losses may be partially  compensated for by the use of a larger drive voltage, however, so that the sensitivity of the system to capacitance change is  expected to be degraded by approximately the square root of


5'0tu


20.0 V


Q only. The sensitivity of such a system with an optimized RF  chain is therefore expected to be of the order of 2 - 3·10-21  F·Hz-1/2. The use of a commercial SiGe BiCMOS process will  also allow the incorporation of significant parts of the signal  conditioning circuitry on-chip, reducing external electronic  complexity and further reducing microphonics and the  influence of stray capacitance.


A programme to develop such an SCM sensor is under way at  the James Watt Nanofabrication Centre (JWNC) of the  University of Glasgow. Figure 5 shows the first chip designed  to test the piezoresistive detection scheme. This chip was  realized using a foundry process provided by Austria Mikro  Systeme (AMS). The chip includes piezoresistive force  sensors, signal conditioning, test lines and the outline of test  cantilevers for subsequent processing. The chip has been used  mostly in the development of back-end micromachining  processes. Future chips will be used to test and validate the  design of the integrated RF oscillator and mixer-based  demodulator. The final SCM chip will comprise a cantilever  beam, an RF oscillator, a power splitter, and signal  conditioning circuitry (amplifiers, mixer, and filters).


Figure 5: Micrograph of SCM chip 1. This chip is designed to  test the piezoresistive deflection sensors.


The instrument presented in this paper is capable of  performing quantitative SCM with sub-zeptofarad sensitivity  in a 1 Hz bandwidth. This resolution is achieved using a non  optimized sense voltage. The phase-based measurement  allows operation at the resonant frequency of the instrument, improving the instrument noise over the design of Tran et al. and may be incorporated directly into a commercial AFM  system. It has been shown that a monolithic CMOS SCM  potentially offers a number of key advantages over hybrid  systems in the measurement of capacitance in semiconductor  systems.


This work was supported by Scottish Enterprise.


[1] J. R. Matey and J. Blanc, “Scanning Capacitance  Microscopy,” J. Appl. Phys, Vol. 57, No 5, pp. 1437-1444, 1985.


[2] C. D. Bugg and P. J. King, “Scanning Capacitance  Microscopy,” J. Phys. E, Vol. 21, pp. 147-151, 1988.


[3] A. Born and R. Wiesendanger, “Scanning Capacitance  Microscope as a Tool for the Characterization of  Integrated Circuits,” Appl. Phys. A, Vol. 66, pp. S421-S426, 1998.


[4] C. C. Williams, “Two-Dimensional Dopant Profiling by  Scanning Capacitance Microscopy,” Annu. Rev. Mater. Sci, Vol. 29, pp.471-504, 1999.


[5] T. Tran, J. N. Nxumalo, Y. Li, D. J. Thomson, G. E. Bridges, and D. R. Olivier, “Quantitative TwoDimensional Carrier Profiling of a 400 nm  Complementary Metal-Oxide-Semiconductor Device by  Schottky Scanning Capacitance Microscopy,” J. Appl. Phys, Vol. 88, No. 11, pp. 6752-6757, 2000.


[6] T. Tran, D. R. Olivier, D. J. Thomson and G. E. Bridges, “Zeptofarad (10-21) Resolution Capacitance Sensor for  Scanning Capacitance Microscopy,” Rev. Sci. Instrum, Vol. 72, No. 6, pp. 2618-2623, 2001.


[7] T. Tran, D. R. Olivier, D. J. Thomson and G. E. Bridges, “Capacitance Sensor with Sub-Zeptofarad (<10-21) Sensitivity for Scanning Capacitance Microscopy,” J. Vac. Sci. Technol. B, Vol. 20, No. 1, pp. 479-482, 2002.


[8] S. Lanyi, “Assessment of Sensitivity and Resolution  Limits of Scanning Capacitance Microscopes,” Acta  Physica Slovaca, Vol. 52, No. 2, pp. 55-64, 2002.


[9] R. C. Palmer, E. J. Denliger and H. Kawamoto, “Cutting  the VideoDisc Master,” RCA Rev, Vol. 43, No. 1, pp. 194-211, 1982.


[10] T. Yamamoto, Y. Suziki, M. Miyashita, H. Sugimura and  N. Nakagiri, “Development of a Metal Patterned  Cantilever for Scanning Capacitance Microscopy and its  Application to the Observation of Semiconductor  Devices,” J. Vac. Sci. Technol. B, Vol. 15, No. 4, pp. 1547-1550, 1997.


[11] V. A. Ukraintsev et al, “Silicon surface preparation for  two-dimensional dopant characterization,” AIP  Conference proceedings 449, Gaithersburg, MD, November. 1998, pp. 736-740.


[12] V. Raineri and S. Lombardo, “Effective channel length  and base width measurements by scanning capacitance  microscopy,” J. Vac. Sci. Technol. B, Vol. 18, No. 1, pp. 545-548, 2000.


[13] D. Goghero, V. Raineri and F. Giannazzo, “Study of  interface states and oxide quality to avoid contrast  reversal in scanning capacitance microscopy,” Appl. Phys. Lett, Vol. 81, No.10, pp 1824-1826, 2002.


[14] G. H. Buh et al, “Factors influencing the capacitancevoltage characteristics measured by the scanning  capacitance microscope,” J. Appl. Phys, Vol. 94, No. 4, pp. 2680-2685, 2003.


[15] J. J. Kopanski and J. F. Marchiando, “Quantitative  interpretation of Scanning Capacitance Microscope  Images as Two-Dimensional Dopant Profiles,” Proc 29th  International Symposium for Testing and Failure  Analysis, Santa Clara, November. 2003, pp. 398-405.


[16] M. Tortonese, RC Barrett and CF Quate, “Atomic  Resolution With An Atomic Force Microscope Using  Piezoresistive Detection” Appl. Phys. Lett, Vol. 62, No.8, pp 834-836, 1993.


Backside 3D Analysis of Power Device Using an ITO Electrode


Yasunori Goto


TOYOTA MOTOR Corp.  543, Kirigahora, Nishihirose, Toyota, Aichi, 470-0309 JAPAN TEL: +81-565-46-3370  FAX: +81-565-46-3382  E-mail: yasunori@goto.tec.toyota.co.jp


The power device has a vertical structure and analysis of  defective products generally occurs from the backside because  the surface is covered in an aluminum electrode and the  backside in a metallic electrode. We will discuss the  development of backside 3D analysis technique using  defective products that emerged due to the marginal valuation  of the power device development. First, it was verified that  applying a DC voltage uniformly to the entire backside would  be effective in placing a glass with an ITO (Indium Tin Oxide) transparent electrode in contact with the backside; therefore it  was able to specify a failure point using the IR-OBIRCH (Infra Red-Optical Beam Induced Resistance CHange) method


[1]. Then, a micro-sample was extracted without missing the  failure point and observed the 3D perspective method; thus it  was clear that existence of crystal lattice defects were thought  about as the cause of failure.


While improving the convenience of automobiles, we also  engage in initiatives to resolve global environmental issues. We believe it should develop automobiles friendly to people  and the environment. The core technology for making that  possible is hybrid technology, and the hybrid system (Fig.1) [2,3] is developed to harness its full potential.


Figure 1: Outline of Hybrid System


In the hybrid system, two sources of power, a high-efficiency  gasoline engine and a permanent magnet AC synchronous  electric motor, are combined to utilize the strong points of  each and to supplement their weak points, resulting in a  system that provides high efficiency and excellent driving  performance.


By aiming for synergy between motor power and engine  power, this marks a new generation of hybrid system for  achieving high levels of compatibility between environmental  performance and power.


Vehicles with the hybrid system enable high fuel efficiency  and reduced CO2 emissions in order to help preserve the  global environment. Under poor driving conditions when  engine efficiency is low, such as during initial acceleration, the electric motor powers the vehicle. Fuel efficiency  increases and CO2 emissions are controlled.


Furthermore, concerning good driving performance, the  hybrid system efficiently stores in the battery the energy  previously wasted when a vehicle decelerated and also stores  the surplus energy generated when driving in low speed  ranges, thus realizing energy regeneration. The vehicle then  reuses the stored energy when accelerating.


The hybrid system is equipped with a power control unit (Fig.2) as a major component to control the motor.


Figure 2: Power Control Unit.


This power control unit contains a high-voltage power circuit  for raising the voltage of the power supply system for the  motor and the generator to a high voltage of several 100 V, in  addition to an AC-DC inverter for converting between the AC  current from the motor and the generator and the DC current  from the battery.


p n pp


Gate


Aluminum


Emitter  Electrode


Polysilicon  Gate


Metallic


Collector


Electrode


Voltage [V]After applied


withstand voltage Before applied


withstand voltage


Current [A]


aatmm


The inverter and converter use the power device such as an  IGBT (Insulated Gate Bipolar Transistor), Diode or power  MOS as the semiconductor switching device (Figs.3 a, b, c), which were developed in the pursuit of smaller devices with  lower heat and improved efficiency.


a) IGBT                 b) Diode           c) Power MOS  Figure 3: Semiconductor switching devices.


Determining the failure’s cause through an investigation of  defective products and obtaining quick and accurate feedback  on the design and process are important to ensure the quality  of the power device development.


The power device has a vertical structure (Fig.4) and analysis  of defective products generally occurs from the backside  because the surface is covered in an aluminum electrode and  the backside in a metallic electrode.


Figure 4: Trench IGBT cross-section.


In this paper, the development of backside analysis technique  will be discussed using an IGBT with a trench cell structure as  the power device and defective products that emerged due to  the marginal valuation.


Experiments and Results


An IGBT with a trench structure was used as the power device (Fig. 4).


For the marginal valuation, a collector-emitter (CE) leakage  current was generated by applying a withstand voltage (Fig. 5). Failure analysis was conducted to discover the cause of the  leakage current and to create a more reliable product.


Figure 5: Ice leakage current vs. Vce voltage.


Site-specific analysis


To specify a failure point using the IR-OBIRCH method, the  metallic electrode was removed from the backside of the  abovementioned sample, then a DC voltage was applied by  probing to the exposed silicon on the backside and to the  aluminum electrode on the surface, resulting in an OBIRCH  image only at the probing point (Figs. 6 a, b). It was found that  the leakage location could not be specified using this method  because the same results were obtained when the probing  point was changed.


a) Overall image of a chip.


b) Enlarged image of a chip.


Figure 6: Backside image superimposed by IR-OBIRCH.


It was thought that the cause was that the DC voltage was not


uniformly applied to the entire backside and was built up in


one point. Therefore, it was proposed placing a glass with an


ITO transparent electrode in contact with the backside and


applying to a DC voltage so that the voltage would be


uniformly applied to the entire backside.


However, OBIRCH images were not obtained even when 90 using the glass with the ITO transparent electrode (Fig. 7). It


was thought about the problem of the infrared transmittance of 80 a glass with an ITO transparent electrode at a film thickness of


340nm; since the transmittance with the near-infrared rays of


1300nm used in the IR-OBIRCH method was measured and it 60 was found that the transmittance was 11.8% slightly (Fig. 8).


%T40


1000 um


Figure 7: Backside image with an ITO.


90


80


昌


Figure 8: Transmittance at a film thickness of 340nm.


The transmittance T is given approximately by [4]


T = exp (-αd)                                                          (Equation 1) Where α is the absorption co-efficient and d is the film of  thickness.


It was thought that the transmittance T was necessary about  50% at least, therefore, following Equation 1, the film  thickness d became about 110nm with the same manufacturing  method.


Using the film at a thickness of 120nm, the transmittance was


measured at 51.2% (Fig. 9) and it was predicted an adequate


transmittance to display OBIRCH images. As a result, it was


able to obtain a clear OBIRCH image using this glass with an


ITO transparent electrode (Figs. 10 a, b, c, d).


666.6671000


2500


Wavelength[nm]


Figure 9: Transmittance at a film thickness of 120nm.


。%T


古


b) 50 times enlarged image of a chip.


c) 200 times enlarged image of a chip.


d) 500 times enlarged image of a chip.


Figure 10: Backside image superimposed by IR-OBIRCH with  an ITO 120nm. The circle indicates the leak position.


Thus, it was verified that this method, which uses a glass with  an ITO transparent electrode as the backside electrode and  specifies from the backside, is effective in site-specific  analysis in a vertical power device.


Physical Analysis


Since the failure site of the IGBT collector-emitter leakage  current is speculated to be at the diffusion layer, trench  structure or emitter contact, it is essential to carry out physical  analysis without missing any failures that the abovementioned  sample is processed with precision from the backside.


First, the sample was ground about 5µm down from the tip of  the trench structure. Then, a micro-sample was extracted using  the FIB (Focused Ion Beam) method [5], and mounted on top  of a 3D holder (Figs. 11 a, b, c) [6, 7].


a) Overview of 3D holder.


b) Tip rotating mechanism and center needle.


c) Micro-sample placed on top of the needle.


Figure 11: Micro-sample mounted on the 3D holder.


Figure 3: Example of a package viewed in water immersion  using a stereomicroscope equipped with a fiber optic ring  illuminator. Note that the tops of some wires are exposed, while others are visible through the remaining package  material.


wires cut is shown in Figure 4. It goes without saying that all  as-received electrical performance characterization of the part  must be completed before this procedure is performed.


Figure 4: Example of a part that has been ground to the point  where all wires are cut.


Exposing silicone gel


An analyst needed to compare different silicone gel  compositions using Raman spectroscopy. It was necessary to  avoid introducing any contaminants to the gel to ensure a  clean spectrum. The part was first parallel ground to within a  few tens of microns of the top of the gel, as shown in Figure


5. The remaining material was broken apart using a sharp  pointed blade and removed from the gel with the blade until  no package fragments remained. The final result is shown in  Figure 6. This technique successfully provided clean  specimens that provided distinct and unadulterated Raman  spectra.


Figure 5: Example of a part that has been partially ground  through 15 micron diamond. The silicone gel can be clearly  viewed through the remaining package material.


无


"


..0


6月


DCD


Figure 6: Part shown in Figure 5 after removal of the  remaining mold compound with a sharp pointed blade. A  large clear area provided adequate material for Raman  spectroscopy.


Spatial mapping of PCB crack locations


Widespread cracking of a PCB was discovered after applying  a reliability stress to a series of parts whose surface devices  were encapsulated in a mold compound. Standard crosssectioning would not provide an adequate spatial  representation of the crack locations that would help to isolate  the cause of the cracking. Instead, the package was parallelground from the top down to the PCB solder mask, followed  by further grinding into the first ply of the PCB substrate. Typical examples of the appearance of the substrates are  shown in Figures 7 and 8. Visual inspection of the parts  revealed that the cracking was focused on the areas where a  high density of discrete resistors and capacitors could be  found. Modeling confirmed the high stress regions. The PCB  was re-designed to use smaller discretes and redistribute them  across the substrate, correcting the problem.


Inspecting and Analyzing Suspected Corrosion


A problem often encountered in the analysis of corrosion of  die metallization is that acid decapsulation can both introduce  corrosive agents and remove the preexisting agents. Using  parallel grinding techniques can allow the analyst to remove  all but a few microns of material mechanically, thus avoiding  the introduction of acids and allowing the remaining mold  compound to protect the area of interest from the introduction  of damage. Under these conditions, energy dispersive x-ray  spectroscopy (EDX) can be performed on the areas of interest. Typically, a 20 kilovolt (kV) electron beam will penetrate the  remaining package material, excite the underlying metal and, ideally, any corrosive agent present on the metal.


A test of this concept was performed on several parts on  which corrosion was suspected. The parts were parallel  ground to within 10 microns or less of the bottom of the packFigure 7: Packaged PCB that has been ground to the solder  mask. Arrows indicate typical regions of high discrete density  which led to substrate cracking and subsequent leakage of  solder during reflow.


Figure 8: Part shown in Figure 7 that has been ground past  the solder mask and into the underlying first ply of substrate. Note the lighter areas (shown at arrows) visible under fiber  optic ring illumination. These are lateral cracks that appear  in the same areas containing a high density of large surface  mounted discretes.


age material across the die surface. This resulted in the loss of  some package material in areas of the die that were not of  interest, while preserving areas that were. An example is  shown in Figure 9. Close inspection of the now-visible die  surface revealed locations near the bond pads exhibiting  evidence of corrosion, as shown in Figure 10.


One of the parts was inspected using a scanning electron  microscope (SEM) and using EDX at 20 kV. An area well  away from the die was selected to provide a control region for  comparison to the area to be inspected. Regions suspected of  containing aluminum metallization and/or corrosion product


were then analyzed. One such region is shown in Figure 11. EDX data at the area of interest, shown in Figure 12, showed  a significantly higher amount of aluminum than that for the


Area_4_Pin_1


control area, indicating that the electron beam did indeed  penetrate the remaining mold compound. No corrosive agents  were identified in the spectrum, however. This suggests that, while the technique does allow the region to be analyzed, more work is needed to ascertain whether this will allow for  the effective analysis of corrosive agents in the metallization.


Figure 9: Example of package material that has been ground  to a thickness of approximately 10 microns or less across the  die surface. Part is shown under fiber optic ring illumination. Boxed region is shown in Figure 10.


一3


1. Ball bonds that did not adhere to their pads, probably


否


due to corrosion of the aluminum.


2. Portion of the die where package material did not  adhere.


Figure 10: Region of die shown in Figure 9. Locations  exhibiting visual evidence of corrosion are shown at arrows.


NSC


LEI10.0kvX220100mWD9.9mm


Figure 11: SEM image showing area used for EDX analysis. Image obtained at 10 kV. Area 4B shown at arrow.


AI


PdPdS uAUPd


|0.50|1.00|Energy |(kV) |2.50|3.00|
|---|---|---|---|---|---|

C o u n t s


o


Figure 12: EDX spectrum of area 4B (dotted) shown in Figure  11, compared with the control area (solid). Note the  significantly elevated peak for aluminum (at arrow).


Parallel grinding can be a very useful tool within its inherent  limitations. Some of these have been discussed above. Others  include implicit assumptions about the package being  prepared. For example, this technique will generally produce a  parallel surface to the plane of interest only if the reference  plane (almost exclusively the opposite surface of the package) is indeed parallel to it. This is not universally true – the die  attach layer is not always even, resulting in a tilted die  surface; the package backside may have been de-soldered  from a board, requiring planarization of the backside that can  render it no longer parallel to the die surface, and so on. At a  minimum, very careful monitoring of the progress of the grind  through the package should be considered an essential  component of the procedure to minimize the risks to the part.  As mentioned above, successful application of parallel  grinding techniques generally requires practice parts to refine  the process for a particular application. This is, by extension, true of parallel grinding in general. It takes time and  experience to gain a level of expertise with this technique that  will allow the analyst to proceed with confidence to single  sample failures. The amount of practice needed will vary with  the baseline experience of the analyst, but is not a trivial  concern even for polishing experts. In addition, the equipment  and consumables used are not inexpensive. These factors  should be weighed by any analyst or laboratory considering  adding a parallel grinding capability to their existing  repertoire.


Each of the described applications represents a successful  sample preparation that yielded useful results for the  customer, except for the corrosion analysis. In this last case, parallel grinding appears to provide a sufficiently artifact-free  sample that can be analyzed. However, EDX analysis may not  be an appropriate technique. Assuming the corrosive agent or  catalyst is still present, other analytical techniques may prove  to be more useful, such as Auger or secondary ion mass  spectroscopy (SIMS) depth profiling of the thinned material  until a strong aluminum signal appears. Additional work is  needed to ascertain whether these or other tools can be  usefully brought to bear on a sample thus prepared.


The parallel-grinding method for package deprocessing has  demonstrated substantial versatility in removing package  material without introducing acid-related preparation artifacts. The principal drawback for the method is that it is highly  dependent on operator experience to produce successful  results. It is also time consuming versus chemical removal. These are important factors to consider when selecting a  sample preparation method.


I thank my colleagues at National Semiconductor for their  support; in particular, Fayik Bundhoo, Marty McVeigh, Jim  Sullivan and Martha Damey for providing parts and driving  the process, and Ted Hasegawa for his input on the  documentation. Walter Bachmann, now with Bachmann  Instruments, also made many helpful suggestions on these  techniques while he was with National Semiconductor. My  thanks also to Gwen Nail for her assistance with editing and  photodocumentation.


[1] Allied High Tech Products, Incorporated, MultiPrep™ System Operation Manual, (Rancho Dominguez, CA, 2006), pp. 27-30.


[2] Nail, C., “An Alternative to High-Temperature and  Acid/Solvent-Based Methods for Removing Integrated  Circuits from Ceramic or Other Problem Substrates,”


Proceedings of the 31st International Symposium for  Testing and Failure Analysis, San Jose, CA, November, 2005, pp. 489-495.


Appendix A


Partial List of Equipment and Materials Used in  Developing This Procedure


For those interested in suppliers for equipment to use for  parallel grinding, I am providing a partial list of the equipment  I used when developing this procedure, with the vendors and  part numbers, as applicable. There are a number of acceptable  vendors for most of the equipment and materials; this list is  not an endorsement of any particular supplier.


Equipment/ Material


|Parallel Polisher |Allied High-Tech |MultiPrep™ System / 15-2000 |
|---|---|---|

|Stereomicroscope |Leica |MZ-125 with IC A camera |

|Diamond Films |Allied High-Tech |15-micron/50-30045 9-micron/50-30050 6-micron /50-30055 |

|Mounting |SPI Supplies MTI Corporation |Crystalbond ™ 509 / 05110-AB Wax Rods / Wax- R1 |

|Adhesives: |SPI Supplies MTI Corporation |Crystalbond ™ 509 / 05110-AB Wax Rods / Wax- R1 |

|Clear |SPI Supplies MTI Corporation |Crystalbond ™ 509 / 05110-AB Wax Rods / Wax- R1 |

|(high temperature) |SPI Supplies MTI Corporation |Crystalbond ™ 509 / 05110-AB Wax Rods / Wax- R1 |

|Beeswax-based |SPI Supplies MTI Corporation |Crystalbond ™ 509 / 05110-AB Wax Rods / Wax- R1 |

|(low temperature) |SPI Supplies MTI Corporation |Crystalbond ™ 509 / 05110-AB Wax Rods / Wax- R1 |

Vendor


Name/Part #


1-micron /50-30065


Three-dimensional nanometric sub-surface imaging of a silicon flipchip using the two-photon optical beam induced current method


E. Ramsay, K. A. Serrels, M. J. Thomson, A. J. Waddie, R. J. Warburton, M. R. Taghizadeh, D.T. Reid


School of Engineering and Physical Sciences, Heriot-Watt University, Edinburgh, EH14 4AS, UK  e.ramsay@hw.ac.uk


By implementing two-photon optical-beam-inducedcurrent microscopy using a solid-immersion lens, imaging inside a silicon flip chip is reported with  166nm lateral resolution and an axial resolution  capable of resolving features only 100nm in height.


Sub-100nm feature sizes are now routine in silicon  integrated circuits, and consequently the industry has  identified a need for non-destructive wafer / mask  level microscopy for measuring the critical  dimensions of three-dimensional (3D) structures and  for defect detection. In an attempt to address this  need using optical imaging, the resolution of subsurface silicon laser-scanning microscopy can be  enhanced by the use of a Weierstrass solid immersion  lens (SIL) in a backside imaging geometry [1,2]. In  this approach a near-infrared laser is focused through  the silicon die, and a suitable SIL eliminates  spherical aberration which is caused by the  refractive-index mismatch at the silicon : air  interface. Such a SIL also increases the numerical  aperture (NA) of the system – up to a maximum  value where the NA equals the refractive index n of  the SIL – and so decreases the focal spot size. Using  a silicon SIL allows a maximum NA of 3.48. During  sample-scanned image acquisition, an increase in the  spatial sampling frequency also results because of an  optical lever effect, where a physical translation of  the SIL and sample results in a proportionately  smaller movement of the focused spot. It is well  known that in the lateral direction the reduction  factor equals the square of the refractive index, a  value of 12.1 in silicon. In the axial direction the  scaling factor is even greater and suggests the  possibility of using high-resolution 3D profiling  techniques to visualise the internal morphology of  silicon integrated circuits with nanometric resolution. We report here two-dimensional (2D) imaging  performance with a resolution of 166nm


and an extension to 3D sub-surface imaging with  approximately 100nm resolution.


High-resolution 2D imaging in twophoton optical-beam-induced current  mode


In silicon devices, standard optical beam induced  current microscopy is hindered by the contradictory  requirements of choosing a laser wavelength that can  penetrate up to several mm of silicon but be absorbed  sufficiently in the micron-scale device layer to  produce high contrast images. The issue of  penetration is also encountered in conventional  confocal imaging using light at 1064nm, where the  proximity of the band-edge means that the absorption  coefficient is around 80cm–1 and the light must be  double-passed through the silicon. An elegant  solution to this problem is to use the two-photon  optical beam induced current (TOBIC) effect [3] to  achieve high absorption of infrared radiation at the  beam focus but high transmission elsewhere in the  sample and in the SIL. Observable two-photon  absorption requires femtosecond laser illumination at  a wavelength longer than the bandedge of silicon (~1.05µm), and in this work we used a femtosecond  erbium-doped fiber laser, operating at 1.53µm, to  image a 0.35µm-feature size silicon flip-chip. The  laser produced pulses with a duration of around 400fs  at a repetition rate of around 30MHz, and the average  optical power at the sample was around 5mW.


The device had a polished 100µm-thick substrate and  the SIL was placed on the backside of this substrate  and was used in combination with a 0.42 NA  objective lens. The Gaussian laser beam, full-width  half-maximum (FWHM) diameter 3.3mm, overfilled  the 3mm-diameter pupil of the objective lens. This  also overfilled the SIL, and a simple ray tracing  analysis implied a maximum usable NA of 3.4. For  this NA value, the lateral point-spread function (PSF) calculated for the overfilled pupil has


aW


CL


OL


Femtosecond


Er:Fiber laserGM


PC


on XYZ scanning stage


GPIBDO RS485


Device under test


b GM


Figure 1 – Experimental schematic.  DO – Digital  Oscilloscope.  GM – Gold Mirror.  DM – Dichroic  Mirror.  CL – Collimating Lens


a diameter of 238nm. Taking account of the √-2  reduction in resolution caused by nonlinear imaging, the PSF diameter becomes 168nm. The sample and  SIL were scanned using stepper motors with a  minimum physical step of 100nm which  corresponded to a lateral optical step of 8.3nm  through the optical lever effect. Two-photon  photocurrent generation was detected using a digital  oscilloscope, and a desktop PC was used to control


10μm


0.9


0.8-0.7 8


166nm


S0.4


0.3


500nm


50-100-500501008o150200


the scanning and to visualise the data. Figure 1 above  shows the experimental configuration.


The device was imaged initially using relatively  coarse (800nm optical) stepping to provide a map  suitable for navigation purposes, shown in Figure  2(a). The lateral resolution was evaluated by  recording a higher resolution image of the area (left  inset, Fig. 2(a)). This region contained a finger of nsilicon under metal, and a resolution measurement  was inferred from a line-scan taken across the edge  of this feature. The result is shown in Figure 2(b) and  implies a resolution of 166nm, although this is


Figure 2 (a) TOBIC SIL image showing detail o tungsten contacts (insets); (b) line-scan data acros edge of feature showing resolution of 166nm


(b


Position (nm)


f  s


(~72μm physical)6000


Y (nm)


X(nm)


4000


u z


600


10001500 2000 2500 3000 3500 4000 4500


Y(nm)


w1000


zE800


3000600


(~225μm physical)1000 1500 2000 2500 3000 3500 4000 4500 X (nm)


u800


6000


Figure 3 (a) 3D profile of 3×3 grid of tungsten  contacts (1.25µm spacing); (b) corresponding crosssectional data


limited by the sharpness of the physical feature itself. Similar measurements performed at widely separated  points routinely implied sub-200nm resolutions. This  result improves on earlier performance obtained  using a similar system [4] and we attribute it to a new  ability to perform systematic axial scanning and so  achieve exact focusing within the component layer of  the chip. The experimental resolution of 166nm  essentially matches the calculated value (168nm) to  within the limits of experimental precision. Our  system is therefore diffraction limited in the lateral  direction with a resolution corresponding to just 11% of the free-space wavelength. At this resolution we  were able to clearly resolve individual features which  we believe are tungsten contacts arranged in a 3×3  grid at separations of 1.25µm. The right inset of Fig. 2(a) shows these contacts on the design schematic for  the device (circled).


Extension to nanometric 3D imaging


The strength of the TOBIC signal is sensitive to the  axial position of the beam focus relative to any  feature in the device, therefore a peak-detection  procedure can be used to profile the 3D morphology  of sub-surface features [5]. Unlike lateral motion, the  sub-surface focal-spot movement caused by axially  translating the sample is not simple to analyse  analytically. Using a ray-tracing model (ASAP, Breault Research Organization) we confirmed a  physical : optical scaling factor of 80 for the SIL  design used in this work, and subsequently used this


to calibrate our experimental data. This is at variance  with the accepted value of n3 which is quoted in the  literature [1]. However, the factor of n3 assumes that  only paraxial rays are considered. When non-paraxial  rays are included in the model the axial scaling factor  changes. The model also verified the familiar n2  lateral scaling factor.


3D profiling was performed by acquiring a set of 2D  images, each one recorded at a different axial  position of the sample. In the resulting data-cube, a  peak detection algorithm was used to find the axial  position corresponding to the maximum TOBIC  signal at each lateral position in the XY-plane. We  concentrated 3D profiling on the area of the device  containing the 3×3 grid of contacts with the aim of  determining their height. Fig. 3(a) shows a 3D profile  of the area, and Fig. 3(b) shows cross-sections  through this image. The axial scale was calibrated  using the results of the ray-tracing model described  earlier. The results indicate that the contacts have a  height of ~160nm, based on the difference in the  maximum photocurrent measured when the beam is  focused either on or between the contacts. The  absolute contact heights, as inferred from the crosssectional data (Fig. 2(b)), are consistent to ±60nm.


In summary, we have demonstrated imaging of subsurface features in 3D with lateral resolutions of  166nm and axial resolutions capable of clearly  resolving individual sub-micron features with heights  of around 100nm. We anticipate further  improvements using shorter excitation wavelengths  and other resolution enhancing techniques.


The authors would like to acknowledge the financial  assistance of the UK Engineering and Physical  Sciences Research Council, and would also like to  thank Credence Systems Corp., Sunnyvale, CA for  technical assistance.


[1] Ippolito, S.B.,  Goldberg, B.B. and Ünlü, M.S., "High spatial resolution subsurface microscopy," Applied Physics Letters Vol. 78, No. 26, (2001), pp. 4071-4073


[2]  M. Born and E. Wolf, Principles of Optics, 7th  Edition (Cambridge, 1999)


[3]  Xu, C. and Denk, W., “Two-photon optical beam  induced current imaging through the backside of  integrated circuits,” Applied Physics Letters Vol. 71, No. 18 (1997) pp2578-2580


[4] Ramsay, E., et al, “Two-photon optical-beaminduced current solid-immersion imaging of a silicon  flip chip with a resolution of 325 nm,” Optics Letters  Vol. 30, No. 1 (2005) pp26-28


[5]  Ramsay, E. Reid, D.T. and Wilsher, K., “Threedimensional imaging of a silicon flip chip using the  two-photon optical-beam induced current effect” Applied Physics Letters Vol. 81, No 1. (2002) pp7-9


Near-IR Photon Emission Spectroscopy on


Strained and Unstrained 60 nm Silicon nMOSFETs


SL Tan1, KW Ang2, KH Toh1, D Isakov1, CM Chua3, LS Koh3, YC Yeo2, DSH Chan1, JCH Phang1, 3


1Centre for Integrated Circuit Failure Analysis and Reliability (CICFAR), National University of Singapore                                2Silicon Nano Device Laboratory (SNDL), National University of Singapore 3SEMICAPS Pte Ltd, Singapore  E-mail: tansoonleng@nus.edu.sg


1.  Abstract


Spectral analysis of near IR photon emissions was  performed on unstrained as well as uniaxial tensile  strained nMOSFETs with physical gate length of 60 nm. The significant differences in the observed spectra could  be attributed to the strain-induced bandgap narrowing.  This shows that photon emission spectroscopy could  potentially be used as a tool to monitor strain in the  nMOSFET channel.


2.   Introduction


Spectral analysis of photon emissions from fault  locations can be used to characterize and identify defects  in integrated circuits [1].  Since each failure mechanism  has its own unique spectral signature, photon emissions  from fault locations can be used for the characterization of  defects [1,2].  Several photon emission spectroscopy  studies had been performed on n-MOSFETs in both the  visible and near IR range [3-6]. All these studies were  performed on unstrained nMOSFETs and there had been  no studies so far on the effects of strain in the silicon  channel on the spectra emitted by nMOSFETs.


Channel strain engineering has been extensively  explored as one of the methods to extend the drive current  IDsat performance as conventional CMOS transistor scaling  meets immense technological challenges. Strain in the  channel increases the drive current by enhancing the  mobility of carriers in the channel.  To improve electron  mobility in nMOSFETs, both lateral tension εxx (along [110] channel) and vertical compression εzz (perpendicular  to the [110] channel) are desired. An effective scheme to  realize these strain components in the transistor channel  makes use of silicon-carbon (Si1-yCy) source/drain regions  which is lattice-mismatched to the Si channel [7-9].


3. Spectroscopic Photon Emission Microscope System  A schematic of the spectroscopic photon emission  microscope system (SPEM) used to obtain the spectra is  shown in Fig. 1 [10]. The microscope is mounted together  with an InGaAs FPA detector which has a wavelength  sensitivity range between 0.9 µm and 1.6 µm.  The in-lens  SPEM system design uses one InGaAs FPA for both  panchromatic PEM imaging and spectroscopy and offers  ease of switching between the imaging and the  spectroscopic modes by just moving the dispersion  element in and out of the microscope optical axis without


the need for moving the detector. Light loss is reduced  with the in-lens design as no additional optical elements  such as mirrors are needed to redirect the light into the  dispersive element or from the dispersive element onto the  detector.


The dispersive element is a three-element prism  which is positioned in the infinity corrected path of the  optical microscope, between the objective lens and the  tube lens. The dispersive element is specially designed to  split the light from an emission spot on the device under  test into a wavelength spectrum for a wavelength range  from 0.9 µm to 1.6 µm with an efficiency of about 70%.


InGaAs FPA


Tube Lens


Dispersive Element


Objective


Focal Plane


Imaging and PEM Spectroscopy


Fig. 1: NIR SPEM  system setup


The objective lens collects and collimates the  light from the emission spot. The collimated light then  passes through the dispersive element and is scattered into  its component wavelengths. The spectrum is projected by  the tube lens onto an InGaAs FPA detector.  Fig. 2 shows  the emission spot during panchromatic PEM imaging and  the resulting spectrum after the insertion of the prism in  the spectroscopy mode. Calibration of the system using a  calibrated light source and bandpass filters is performed to  find the wavelength spread of the spectrum and  compensate for the difference in sensitivity of the system  at different wavelengths. Care is also taken to ensure that  the spectrum does not lie on any dead pixels.


Fig. 2: (a) Panchromatic PEM image and


(b)  corresponding spectroscopic image after  insertion of the dispersive element


4. Strained and Unstrained nMOSFETs Fabrication


The fabrication process flow for the strained  nMOSFET is given in Fig. 3 [8]. After LOCOS formation, p-well, threshold voltage VT  adjust and punchthrough  implants were performed. The gate stack comprised of  poly-Si and SiO2 with a thickness of 2.5 nm. After gate  etching, a SiN spacer with a SiO2 liner was then formed. This was followed by Si source/drain recess etch and  selective epitaxial growth of Si0.99C0.01 using the ultra-high  vacuum chemical vapor deposition (UHVCVD). On the  control wafer which has the unstrained nMOSFETs, a  selective Si epitaxy was performed to form raised Si  source/drain, therefore minimizing series resistance  differences between the unstrained and the strained-Si  nMOSFETs. Source/drain implantation and dopant  activation steps were then performed before contact  formation and metallization to complete the device  fabrication. Fig. 4 shows the SEM picture of a strained nFET with Si1-yCy source/drain regions and a gate length of  60 nm. Excellent growth selectivity and surface  morphology were demonstrated. No dislocation-like  defects were observed near the Si/Si1-yCy heterojunction


despite a substantial lattice mismatch between the two  materials, as depicted in the TEM micrograph in Fig. 5.


The lattice mismatch between Si1-yCy source/drain and  the adjacent transistor channel give rise to two major  strain components in the transistor channel [11]: the  lateral tensile strain εxx and the vertical compressive strain εzz. Near the vertical Si-Si1-yCy heterojunction, the Si lattice  experiences vertical compression, which is also linked to a  lateral tensile strain in Si which extends throughout the  channel region. The highest lateral tensile strain is  observed near the Si1-yCy source/drain which decreases as  it extends towards the transistor channel centre [7].


Fig. 3: Process sequence employed in the


fabrication of n-FETs with Si1-yCy source/drain.


Fig. 4: SEM micrograph of the strained n-FET


with Si1-yCy source/drain stressors.


Si 1-yC ySi 1-yC y


Si 1-yC y


0P-well, Punchthrough and VT  Implants  0SiO2 Gate Oxidation


oSDE Implant and Spacer Formation Si Source/Drain Recess Etch (~60 nm)


oS/D Implant and RTA at 900°C, 30s  LOCOS Formation


oPoly-Si Gate and Hardmask Deposition   oGate Patterning and Photoresist Trimming


0PECVD SiO2 Deposition and Metallization


Si1-yCy Selective Epitaxy


Fig. 5: TEM micrograph of 60 nm gate length LG  Si1-yCy source/drain transistor.


5. Results and Discussion


The Ids–Vds characteristics of the strained nMOSFETs


sample (SS) and the unstrained nMOSFETs sample (US)


are shown in Fig. 6. The strained device demonstrates a


higher drive current performance than the unstrained


device.  At a similar gate overdrive Vgs-VT of 1.2V, uV strained nMOSFET shows a 35% IDsat improvement over n the unstrained control nMOSFET, predominantly


attributed to strain-induced mobility enhancement. Fig. 7


and 8 show the substrate current characteristics Isub for


both the strained and unstrained devices.  The substrate


current is an indication of the strength of the emission.


The higher the substrate current, the stronger is the


emission. At a similar Vds, the strained nMOSFET shows a


higher maximum Isub as compared to the unstrained


nMOSFET. This is because strain enhances the electron


mobility and leads to a reduced electric field for velocity


saturation Esat.  This reduction of Esat contributes to a


reduced saturation drain voltage VDsat, which


concomitantly results in a higher lateral channel electric


field for impact ionization.  It is interesting to note that in


the presence of strain effects, the Isub-Vgs characteristics


deviate from the conventional bell-shaped curve. The


initial rise in Isub with increasing VGS is due to the


increased electron inversion charge density that supplies


the carriers for the impact ionization process.  When VGS


approaches VDS, the lateral channel electric field reduces


and Isub decreases rapidly even as Vgs continues to rise.


However, strained n-FET shows a much gradual decline in


the Isub at high Vgs.  This is attributed to a reduced VDsat as


a consequence of the strain induced effects.  Fig. 8 also


shows that for gate voltage at 1.5V, the intensity of the


emission for the strained sample decreases as Vgs


decreases but for unstrained sample, the intensity


increases Vgs decreases.


0 2 4


S.S Vgs=1.3V S.S Vgs=1.5V U.S Vgs=1.3V U.S Vgs=1.5V


0 4


Vds (V)


Fig. 6: Ids-Vds characteristics of strained (SS) and  unstrained (US) nMOSFETs


-150-100-50


US Vgs=1.3V US Vgs=1.5V SS Vgs=1.3V SS Vgs=1.5V


1.


0.


-50


-100


-150


Fig. 7: Substrate current Isub characteristics of strained (SS) and unstrained (US) nMOSFET as a function of Vds


US Vds=2.4V US Vds=2.2V SS Vds=2.4V SS Vds=2.2V


Isub (uA/mm)0.1


Vgs (V)


Vgs=1.5V


Fig. 8: Substrate current characteristics of strained and  unstrained nMOSFET as a function of Vgs


Ids (mA)


LG~ 60 nmSpacer


Strained-Si


Si  subssubs


Frontside photon emission spectroscopy was  performed on both the strained and unstrained sample  since there is only a single metal layer. Backside testing  was also not done as spectra information lower than the  wavelength corresponding to the Si bandgap will be  filtered by the silicon filter effect.  Fig. 9 and 10 show the  spectra collected from the strained and unstrained  nMOSFETs at Vgs = 1.3V and Vgs = 1.5V, respectively, with increasing drain voltage Vds. 8 frames of the spectra  whose integration time ranges from 5s to 15s depending  on the strength of the emission, are used to provide spectra  of reasonable signal to noise ratio. The intensities of the  spectra are then normalized by the integration time. Effects of the dielectrics interfaces on the spectra were not  taken into account as the dielectrics layer for the samples  are the same and thus have the same effects on the spectra  of both the strained and unstrained samples. Simulation on  the effects of the dielectrics conducted also showed that  the dielectrics have little effects on the frontside spectra.   Fig 11 shows a plot of the spectra of the strained and  unstrained nMOSFETs at Vgs = 1.3V together. There are  significant differences between the near-IR photon  emission spectra of the devices.  The intensity of the  spectra for the strained nMOSFETs is higher than that of  the unstrained nMOSFETs. This is consistent with the  substrate current plots in Fig. 7 and 8. The spectra of the  unstrained sample are more broad based and have  intensities which are relatively stronger at shorter  wavelengths. The unstrained device spectra have a peak at  around 1.18 µm and another smaller peak at around 1.45 µm. The 1.18 µm peak corresponds approximately to the  bandgap energy of Si.  These spectra are similar to  previously obtained spectra from unstrained nMOSFETs  with longer gate lengths [3,6] but significantly different  from the measured spectra reported by NC de Luna [5] and Stefan Rusu et al [12]  which showed a monotonic  spectrum with no obvious peaks. The 1.45 µm wavelength  peak had been previously observed and reported in  photoluminescence and electroluminescence of Si [13,14]. For strained nMOSFETs, the spectra are observed to  have much sharper peaks with its two main wavelength  peaks occurring at 1.25 µm and 1.32 µm, respectively. It  is also interesting to note that the intensity of the 1.25 µm  peak decreases significantly as Vds decreases, decreasing  the ratio of the peak intensity between the 1.25 µm and the


1.32 µm wavelengths.


We believe that the 1.25 µm and the 1.32 µm  wavelength peaks for the strained sample spectra are  attributed to the Si bandgap narrowing as a result of  strain-induced effects at the Si1-yCy/Si heterojunction. The  highest lateral tensile strain is observed near the Si1-yCy  drain which decreases as it extends towards the transistor  channel centre [7].  Hence, a larger conduction band  modulation is expected near the drain-end compared to  that at the Si channel centre due to reduced strain effects.  As Vds changes, the lateral electric field in the channel  changes and the point of maximum emission in the  channel shifts correspondingly, resulting in the change of  the ratio of the intensity between the 2 peaks.


While fully exploiting the ±15° tilt and 360° rotation functions  of the 3D holder, the micro-sample was thinned a columnar  sample using the FIB method with a thickness of up to 3µm  for 3D perspective observation by the STEM (Scanning  Transmission Electron Microscope) method [8] without  missing the OBIRCH image point in the sample (Fig. 12).


360°


±15°


Figure 12: Columnar sample.


As a result of the perspective observation of the 3µm columnar  sample, it was clear that the collector-emitter leakage current  due to the marginal valuation was created by a lattice defect  that existed in the diffusion layer between the trench structures (Figs. 13, 14).


Figure13: SE image by STEM.


Figure 14: TE image by STEM.


These results were given as feedback to the process engineers  and were helpful in building more reliable products.


We developed a technique that is capable of identifying with  precision the failure in a power device from the sample’s  backside direction using a glass with an ITO transparent  electrode as a backside electrode.


This technique can also be used to identify failures in the  power device for mounting products; because sampling is  conducted from the backside direction, the failure site can be


observed with precision and will not be missed, even when the


failure site is the contact portion of the surface wire and the  surface electrode (Figs. 15,16), which may lead to  improvements.


Furthermore, because other power devices with a vertical  structure comprising other elements than Si, such as SiC and  GaN, also have transparency in the near-infrared area, this  technique is deemed to be applicable to failure analyses of any  relevant devices and useful for the development of nextgeneration power devices.


Figure 15: Mounting product.


Figure 16: TE image by STEM.


The author would like to thank Masaru Iida, Tomoki  Nakazawa, and Tomonori Hayamizu for their technical  support, and I would also like to thank Yusuke Sekiya, Shinji  Wakaya, Akane Hasegawa for their daily operations.


[1] Nikawa, K., et al, “Failure Analysis Case Studies Using  the IR-OBIRCH (Infrared Optical Beam Induced  Resistance CHange) Method,” Eighth Asian Test  Symposium (ATS'99), pp. 394-399.


[2] Kawahashi, A., “A new-generation hybrid electric vehicle  and its supporting power semiconductor devices,” Proc 16th International Symposium on Power Semiconductor  Devices and ICs, Kitakyushu, Japan, May. 2004, pp23-29.


[3] Fujikawa, T., “Semiconductor technologies support new  generation hybrid car,” 2004 Symposium on VLSI  Circuits, pp.6-9.


[4] Gupta, L., Mansingh, A. and Srivastava, P. K., “Band Gap  Narrowing and the Band Structure of Tin Doped Indium  Oxide Films,” Thin Solid Films, Vol. 176, Issue 1 (1989), pp. 33- 44.


[5] Ohnishi, T., Ishitani, T., US patent 5270552.


[6] Koguchi, et al, “Three-dimensional STEM for observing  nanostructures,” Journal of Electron Microscopy, Vol. 50, No. 3 (2001), pp. 235-241.


[7] Goto, Y., Higuchi, T., “A 3D Analysis Technique for  Detecting Trace Metal Contamination,” Microelectronics Reliability, Vol. 46, Issues 9-11 (2006), pp.1542-1547.


[8] Yaguchi, T., et al, “A FIB Micro-Sampling Technique for  Three-Dimensional Characterization of a Site-Specific  Defect,” Microscopy Today, Vol. 12, No. 6 (2004), pp. 26-29.


Al electrode


Al wire


Re-thin a TEM Lamella by Using a Novel TEM Sample Preparation


C. R. Chen


Material Science Service Corp., 1F, No.27, Pu-ding Rd., Hsin-chu, Taiwan, R.O.C.


In regards to structural evaluation and failure analysis of  increasingly integrated and scaled-down Si devices, advanced structural and elemental characterization with high  spatial resolution is required. As such methods, atomic-level high resolution observation and elemental  analysis techniques like TEM (Transmission Electron Microscope) are gaining recognition.[1] The use of focused  ion beam (FIB) instruments has become a mainstream for  the preparation of TEM specimens. Especially, because of  the small spot size achievable by FIB instruments, FIB  specimen preparation techniques presently offer the best  spatial resolution where site specificity is required.[2]


Conventional FIB ex-situ lift-out is the most common technique for precise TEM sample preparation. A primary advantage to the ex-situ lift-out technique over other FIB  specimen preparation methods is that specimens may be  prepared from the starting bulk sample with little or no initial specimen preparation. This is particularly useful when  performing failure or defect analysis, since destructive  preparation of the original wafer or bulk sample may be  avoided. The concept of ex-situ lift-out was first described  in 1993 and, was then followed by other references to the  technique.[3-6] But this method has some limitations: samples cannot be reprocessed for further analysis; the carbon   film (or some other elements film) supported grid affects  the EDS analysis for carbon element; and amorphous sample surface caused by Ga ion damage affects the resolution  of high resolution TEM image.


So, in-situ lift-out technique was developed to overcome  these drawbacks and several commercial in-situ lift-out  tools [7-8] are usually used for cross sectional TEM sample  preparation. It lifts-out the sample and then attaches the  sample to a half-cut copper grid inside the FIB chamber by  mini-probing system.


This paper introduces a new and simple technique that can


overcome the above problems and a wide application of


TEM samples preparation.


Samples Preparation Procedures


The FIB ex lift-out technique allows thin lamellas to be


extracted from bulk material, which saves a lot of sample  pre-thinning time and is very successful in the preparation


of site specific cross sections and planar samples. This


novel sample preparation includes two parts of procedures. In first step gets a thin lamella by using conventional FIB


cutting method. Second step ex-situ lifts out the lamella and  put it onto a silicon base supported Cu ring by a static glass  needle. The detailed preparation steps are described below:


1. Conventionally get a precise cross-sectional TEM


sample lamella (with thickness 0.5~1um) by FIB, as


shown in Fig. 1. This preparation can be automated by  using scripts and macros.


2. Using a simple tool of static glass needle to put the


lamella onto a Si-base supported film by ex-situ lift-out  method, which is shown in Fig. 2. The Si-base film


(about 50-100um thick) is easily produced by traditionally polishing method.


Fig. 1 A precise cross-sectional TEM sample lamella by FIB  cutting


Fig. 2 Put the TEM lamella on a Si-base supported film by  ex-situ lift-out method. The area with color fringe is Si base  film.


0.7um


Si-base film


TEM lamella


3. Put the specimen into FIB chamber to stick the lamella  on Si-base supported film by depositing Pt or C to


achieve the preliminary sample, which the lamella is


fixed on the Si and will not fall during the subsequently ion-miller sputtering. The FIB and OM images  are shown in Fig. 3-4.


4. The specimen then can be observed by TEM and it also  can be reprocessed for further analysis, thinning by


ion-miller for example.


stick by FIB deposition


Fig. 3 The FIB image shows the preliminary TEM sample  whose lamella is stuck on Si-base supported film by FIB  deposition


Fig. 4 The OM image shows the preliminary TEM sample  whose lamella is stuck on Si-base supported film by FIB


deposition.


By using this novel method, it is easy, efficient and economic to get a TEM specimen.


In the following, we compare the difference of TEM images between these two methods of traditional lift out and  this new novel sample preparation.


We choose a LED (Light-emission diodes) product for example since this III-V compound material is easily been  damaged during FIB cutting, which there will exist an  about several to 30-nm-thick amorphous layer on the sample sidewall depends on the accelerated voltage of ion beam. The example is showed in Fig. 5. The amorphous layer on  sample sidewall will affect the resolution of TEM image  due to the extra electron scattering as electrons interact with  the amorphous layer.


Fig. 5 Examples of thickness of amorphous layer on the  sample sidewall versus various accelerated voltage of ion  beam.


Results comparison


The result as shown in Fig. 6 and 7 are the TEM images of  specimen prepared by the new method and subsequently  had been further processed by ion-miller with low energy  and low sputtering angle ion to reduce the artifact of amorphous effect on specimen sidewall. The images resolution  showed both in low and high magnification is very good  that quantum-well (QW) structure is clearly observed.


Fig. 6 TEM images of specimen prepared by the new


method with further processing by the ion-miller with low  energy and low sputtering angle ion. The image resolution  is very good. The quantum-well (QW) structure is clearly  observed.


For III-V compound materials in sample cutting process by  using FIB, since the selective etching effect of Ga-ion on  different elements of group-III and group-V is different, it


QW structure


TEM lamella for TEM observation


will form agglomerative spots of metal residue, as shown in  Fig.8, on the sample surface. By this novel method, the  sample surface is free of defects and spots.


20nm.


Fig. 7 The TEM images of specimen prepared by the new  method is further processed by the ion-miller with low energy and low sputtering angle ion. The image resolution is  very good. The quantum-well (QW) structure is clearly  observed.


Fig. 8 and 9 are TEM images whose specimen was prepared by conventional FIB ex-situ lift-out method. It can be  seen, the quantum well (QW) structure was not much  clearer than the former result.


Fig. 8 TEM image whose specimen was prepared by conventional FIB ex-situ lift-out method. It can be seen, the  quantum well (QW) structure was not clear.


50mm


Fig. 9 TEM image whose specimen was prepared by conventional FIB ex-situ lift-out method. It can be seen, the  quantum well (QW) structure was not clear.


The advantages of this novel sample preparation are:


(a) It can reduce the amorphous phenomenon on the sidewall of specimen, which could increase the TEM spatial resolution to atomic scale level.


(b) The cost is low for this method comparing to some  in-situ lift out method by using the mini-probing system. Since it just needs to prepare a silicon base Cu  ring by easy polishing method.


(c) No shield effect was found during the reprocess of  thinning by the ion-miller, since the silicon base film  was thin, it will not shadow the ion sputtering at the  sample target.


(d) No contamination induced by the ion-miller sputtering  was formed. For some commercial in-situ lift out  method, some element comes from Cu or Mo grids will  be detected by EDS (Electron dispersive spectrum) analysis after sample sputtered by ion-miller.


This is a solution to reprocess TEM lamella if specimen is  too thick to observe the nano-structure and too much ion  damage results in the amorphous sidewall effect. In addition, it can eliminate the carbon signal coming from the  carbon film supported grid for EDS analysis.


The examples highlighted here demonstrates the novel  method of low cost and high image quality TEM sample  preparation, which combines conventional FIB ex-situ lift  out and new method to support TEM lamella for reprocessing. Using a simple tool of static glass needle to put the  lamella onto a Si-base supported film by ex-situ lift-out  method, and subsequently stick the lamella on Si-base  supported film by FIB deposition to fix the lamella on the  Si for further ion-miller sputtering reprocess. It can reduce


00mm


Metal agglomeration


the amorphous phenomenon on the sidewall of specimen; no shield effect was found during the reprocess of thinning  by ion-miller; and no contamination induced by the  ion-miller sputtering was formed.


References:


1. T. Yaguchi, M.Konno, T. Kamino, M.Ogasawara, K. Kaji, T.Ohnishi, M.Watanabe, 3D observation of elemental distribution of Si-device using a dedicated  FIB/STEM System, Proceedings of the 31 International  Symposium for Testing and Failure Analysis


2. Lucille A. Giannuzzi, Brian W. Kempshall, Shawn D. Anderson and Brenda I. Prenitzer, Thomas M. Moore, FIB Lift-Out for Defect Analysis


3. M.H.F. Overwijk, F.C. van den Heuvel, and C.W.T. Bull-Lieuwma, J. Vac. Sci. Technol., B 11(6), (1993)


2021.


4. A.J. Leslie, K.I. Pey, K.S. Sim, M.T.F. Beh, F.P. Goh, ISTFA ’95, International Symposium for Testing and  Failure Analysis, 6-10 November 1995, Santa Clara, California, ASM Int., 353.


5. F.A. Stevie, T.C. Shane, P.M. Kahora, R. Hull, D. Bahnck, V.C. Kannan, and E. David, Surface and Interface Analysis, 23, (1995) 61.


6. L.R. Herlinger, S. Chevacharoenkul, D.C. Erwin, Proceedings of the 22


nd


International Symposium for  Testing and Failure Analysis, 18-22 November 1996, Los Angeles, California, 199.


7. Xtreme Access, Ascend Instrument, Beaverton, OR


8. Yaguchi T., Urao R., Kamino T., Ohnishi T., Hashimoto T., Umemura K., Tomimatsu S., Mater. Res. Soc. Symp. Proc. 636, Nonlithographic and Lithographic Methods of Nanofabrication: From Ultralarge-Scale Integration to  Photonics to Molecular Electronics (2001): D9.35/1-D9.35/6.


Applications for Parallel Grinding as an Alternative to Chemical Decapsulation in  Preparing Packaged Samples for Failure Analysis


Carl Nail


National Semiconductor Corporation, Santa Clara, California, United States  carl.nail@nsc.com


Acid etching of plastic packages can both remove key  evidence and introduce artifacts on decapsulated samples. Parallel grinding offers a non-chemical option for removing  package material that can minimize these risks. This technique  was used successfully on three different types of failure  analysis investigations. It also has potential for supporting the  analysis of corrosion defects, though additional work is  needed to confirm the utility of parallel grinding in this  application.


Injection-molded packages using a glass particle-reinforced  polymer matrix have become the dominant choice for  enclosing and protecting integrated circuit (IC) dice. This  option has proven to be a relatively inexpensive and reliable  alternative for ICs that will not be exposed to harsh  environments or require extraordinary efforts to address issues  of thermal management. When an analyst needs to inspect a  die inside a molded package, the typical choice for removing  this material is to use concentrated acids, often with  specialized high-temperature injection equipment, to remove  the mold compound (often referred to as “jet etching”). The  technique has proven reliable over many years, but it is not  artifact-free. Removing mold compound with acids poses the  risk of also removing material from the die surface that may  be a key contributor to a failure mechanism, especially when  investigating corrosion. If the mold compound rests atop a  printed circuit board (PCB), these chemicals can easily  damage the PCB. It is also difficult to control depth of  removal when only a partial removal of the package is desired. Consequently, it is desirable to have a workable alternative to  chemical decapsulation that can reliably preserve sensitive  structures and materials of interest.


The alternative described in this paper is to remove package  material mechanically, rather than chemically. Parallel lapping  or polishing equipment is routinely used in microelectronics  failure analysis for two purposes: to mechanically delayer  integrated circuits, usually for the purpose of inspecting each  process layer of interest for defects; and to cross-section IC’s  to specific locations that permit inspection of a defect or other


anomaly that cannot be analyzed from the surface [1]. The  same equipment can, however, also be used to remove  package material from packaged parts to facilitate inspection  and analysis of structures hidden beneath the surface of the  mold compound. The polishing cloth is replaced with large or  medium grit diamond polymer films that grind away material  rapidly. These films are also used for die cross-sectioning, as  opposed to the slower asperity-removal process associated  with polishing. The grinding is performed parallel to reference  planes on the package (usually the bottom of the package) to  maintain a surface that is parallel to the features of interest in  the package. The process can proceed to within a few microns  of the surface of the die, but should never actually reach the  die surface, as this would introduce an unacceptably high risk  for die damage. Parallel grinding offers the advantage of  removing material without introducing foreign chemistries  and at a rate and depth that are subject to precise control, repeatably within five microns or less.


Grinding Procedure


The basic procedure for the parallel grinding of packages is  given in the following description. It includes details on  equipment, materials, speeds, and other specifics that have  generated successful results in my laboratory. A partial list of  equipment and materials used is included in the Appendix. There is room, however, for a great deal of flexibility in the  procedure for experimentation with different materials and  techniques.


Package Analysis


A key element of using such techniques is to have a sound  knowledge of the interior structure of the package. This can be  obtained either from build sheets or, preferably, from  radiographic data obtained for the part of interest. Modern  radiographic equipment typically includes software that  allows for obtaining good measurements of thicknesses for  edge-viewed parts. One example of such a radiographic  measurement is shown in Figure 1. Even without such data, measurements can still be made on a radiograph using  calipers, followed by direct measurement of the part of  interest with the same calipers. For example, the ratio of the  overall package thickness on the radiograph to that measured


directly on the part provides a conversion factor to translate  any other radiographic measurement to its actual physical  counterpart on the package. Armed with this data, the analyst  can then use depth gauges on parallel polishing equipment to  set a fixed removal depth that permits rapid and safe removal  of bulk material to reach a depth of interest.


-1.0mm


Figure 1: Radiograph showing the distance from the top of  the package to the top of a silicone gel over the die.


Sample Preparation


The package must be mounted to a fixture that can, in turn, be  mounted onto the polishing equipment. Moreover, the side  being mounted to the fixture must be parallel to the internal  plane of interest. This usually means that the back side of the  package will be attached to the fixture. Especially for  packages with leads as shown in Figure 1 (i.e., leads that do  not allow for the backside to make contact with the fixture), this will require either the bending or trimming of the leads to  insure co-planarity between the package and the fixture. If  electrical integrity internal to the package is important, then  the best option is to gently grind away the leads down to the  level of the package base. Applying light pressure on a  tweezer-gripped package to a grinding wheel at 200 RPM  with 600-grit silicon carbide paper has proven successful for  removing the portion of leads extending below the package  base. It is important to hold the leads at an angle to the  grinding surface to avoid damage to the package base. Such  damage could cause the surface to be no longer parallel with  the plane of interest, making it impossible to correctly mount  the part.


Mounting


Most manufacturers of parallel polishing equipment will have  particular instructions for mounting parts to their fixtures, though they will all be similar. Parts are generally hotmounted to the fixture using one of several rigid adhesives, such as Crystalbond ™ or wax, which can be re-heated to  remove the part when grinding or polishing is completed. To  minimize the risks of heating-related artifacts, the lowest  temperature that will still melt the adhesive is best. Previous  work has shown a temperature of 70 degrees Celsius to be  safe and effective [2]. A liberal amount of adhesive is placed  on a heated fixture and allowed to completely melt. The part is


placed in the melted wax while hot, carefully centered on the  fixture, and pressed into place firmly to ensure an even  displacement of adhesive across the package surface. The  fixture is then removed to a cooling chuck and allowed to cool  to room temperature. During mounting, the adhesive may run  up the sides of the package and/or onto the top of the package. The adhesive should not be allowed to remain at or above the  top level of the package – such adhesive should be completely  removed using sharp blades and solvents before grinding. An  example of a mounted package is shown in Figure 2.


Figure 2: Example of a typical package sample mounted on a  polishing fixture.


Grinding


Select an appropriate size of diamond film and secure it to the  platen. The fixture is then placed on the polisher. To use a  parallel polisher for the applications described herein, it must  have a depth gauge that can continuously measure vertical  displacement of the polishing fixture. Before lowering the  polishing head, reset the depth gauge to zero. Lower the head  onto the diamond film slowly, so as not to crack the seal  provided by the adhesive. Continue to increase vertical  displacement until the depth gauge value increases from zero  to the value of the thickness to be removed.


If the polisher has a neutral or “parked” position for the head  for use between polishing steps, then place the head in that  position now. Start the platen rotation, sample rotation (if  available) and lubricant supply flow, then slowly lower the  polishing head down to the platen until full contact with the  diamond film is made.


Observe the progress of the grind on the depth gauge. It  should reduce from the preset starting thickness downward  towards zero. Check the progress of the grind several times  during the grind by inspecting the ground surface under a  stereomicroscope to ensure that it is proceeding without  problems. Once the gauge reads zero, pressure is no longer  being applied to the fixture, and the grind is complete. Raise  the head to the “parked” position, remove the polishing fixture


and inspect the progress of the grind. Stop grinding once a  satisfactory result is obtained.


The above description assumes that only one size of diamond  film is used. In fact, as with most grinding processes, several  progressively smaller sizes of diamond film are frequently  used to create a smooth surface finish. Unless otherwise  noted, the samples included in this paper progressed from 15  micron diamond to six micron to one micron. In addition, the  films often have elastic properties that make a true  determination of the zero point of the grind difficult. It is thus  very important to check progress of the grind often to avoid  over-grinding, and possibly destroying, the sample. As with  all metallographic techniques, it is extremely important to  obtain experience on practice samples prior to attempting to  prepare actual failures.


Examples of Applications


Applications for parallel grinding are limited only by the  imagination of the analyst. Examples of past successful  applications include the following:


Cutting bond wires


There are occasions where an analyst must electrically isolate  a die from the leads to facilitate electrical characterization of  the failure. Parallel grinding is a reliable and repeatable  technique to accomplish this. The part is ground close to the  wire tops using large grit diamond films, typically in the 9 to  15 micron range. The wires can typically be viewed through  thin package material using a fiber optic ring illuminator on a  stereomicroscope. An example appears in Figure 3. Smaller  grit sizes are then used to remove just enough of the package  and wire to isolate the wire or wires of interest. A part with all


0 1 2 3


Vds=1.5V Vds=1.4V Vds=1.3V


1.0


Energy (eV)


/su)Intensity (a.1


Wavelength (µm)


Fig. 9(a): Near-IR photon emission spectra from strained  nMOSFETs at Vgs=1.3V and at different Vds


Intensity (a.u)/s0.3


Fig. 9(b): Near-IR photon emission spectra from unstrained  nMOSFETs at Vgs=1.3V and at different Vds.


Intensity (a.u)/s2


Fig. 10(a): Near-IR photon emission spectra from strained  nMOSFETs at Vgs=1.5V and at different Vds.


Fig.10(b): Near-IR photon emission spectra from unstrained  nMOSFETs at Vgs=1.5V and at different Vds.


5.   Conclusion


Frontside near infrared photon emission spectroscopy  was successfully demonstrated on unstrained and uniaxial  tensile strained nMOSFETs with a physical gate length of  60 nm. The spectra collected from the spectral studies  show that there are significant differences in the near infra  red wavelength spectra of strained and unstrained devices. The significant difference between the spectra is believed  to be due to the effects of the lateral tensile strain effects  induced in the transistor channel by the Si1-yCy  source/drain. These differences in the near infrared spectra  show that photon emission spectroscopy can potentially be  used as a tool to estimate the strain in the silicon channel  of strained MOSFETs.


SL Tan is supported by a National University of  Singapore research scholarship and a grant from Chartered  Semiconductor Manufacturing Chartered Semiconductor  Postgraduate sub 90nm Project Development  Programme.. KW Ang is supported by a Singapore  Agency for Science, Technology and Research Graduate  Scholarship.   Work is partially supported under Singapore  Ministry of Education ARF Project R263-000-252-112.


1. Kolzer J, Boit C, Dallmann A, Deboy G, Otto J, Weinmann D, "Quantitative emission microscopy", J  Appl Phys, Vol 70, No 11, pg 23-41,1992.


2. JCH Phang, DSH Chan, SL Tan, WB Len, KH Yim, LS Koh, CM Chua, LJ Balk, “A review of near


infrared photon emission microscopy and  spectroscopy”, Proc IPFA  pp. 275-281..


3. M.Herzog, F.Koch;”Hot Carrier emission from  Silicon MOS devices” App. Phys Lett, 53, 26, pp. 2620-2622, 1988.


4. Len WB, Liu YY, Phang JCH, Chan DSH; “Near IR  continuous wavelength spectroscopy of photon  emissions from semiconductor devices”; Proc ISTFA  2003, pp. 311-316


5. N.C de Luna, M. F. Bailon,  A. B. Tarun; “Analysis


sIntensity (a.u)/


of near-IR photon emissions from 50-nm n- and pchannel Si MOSFETs”; IEEE Transactions on  Electron Devices, 52, 6,  pp. 1211-1214,  2005.


6. SL Tan, KH Toh, JCH Phang, DSH Chan, CM Chua, LS Koh, “Determination of intrinsic spectra from  frontside and backside photon emission  spectroscopy.” Proc IRPS, pp. 620-621, 2007


7. Yeo YC, ”Enhancing CMOS transistor performance  using lattice-mismatched materials in source/drain  regions” Semicond Sci Technol, 22, pp. S177–S182, 2007


8. Ang KW, Chui KJ, Tung CH, Samudra G.,  Balasubramanian N, Yeo YC, "Enhanced carrier  transport in strained bulk N-MOSFETs with siliconcarbon source/drain stressors," VLSI-TSA, pp. 138-139, 2007


9. Ang KW, Wan Chui KJ, Tung CH, . Balasubramanian N, Li MF, Samudra G, Yeo YC, Hot carrier reliability of strained n-MOSFET with  lattice mismatched source/drain stressor” Proc. IRPS, pp. 684-685, 2007


10. Tan SL, Toh KH, Phang JCH, Chan DSH, Chua, CM,  Koh LS, “A new near-IR continuous wavelength inlens photon emission spectroscopy system” Proc 14th  IPFA, pp. 240-244, 2007.


11. Yeo YC, "Strained-silicon transistors with siliconcarbon source/drain," Extended Abstracts of SSDM, 2006, pp. 162-163.


12. Stefan Rusu, Steve Seidel, Gary Woods, Dean  Grannes, Harry Muljono, Jeremy Rowlette, Keiko  Petrosky, “Backside Infrared Probing for Static  Voltage Drop and Dynamic Timing Measurements”, Proc. ISSCC Session 17, 2001.


13. V.V. Kveder, E.A. Steinman, S.A. Shevchenko, H.G. Grimmeiss, “Dislocation-related electroluminescence  at room temperature in plastically deformed silicon”, Physical Review B Vol. 51, No. 16, pp. 10520-10526,


1995.


14. S Binetti, S. Pizzini, E. Leoni, R. Somaschini, A. Castaldini, A. Cavallini, “Optical prperties of oxygen  precipitates and dislocations in silicon”, Journal of  Applied Physics Vol 92, No. 5, pp. 2437-2445, 2002.


Failure Localization & Design Debug on Mixed-Mode ICs


by Using the Dynamic Laser Stimulation Techniques


Magdalena SIENKIEWICZ1,2, Kevin SANCHEZ1, Abdellatif FIRITI2, Olivier CREPEL2, Philippe PERDU1, Dean LEWIS3


1: CNES – French Space Agency, 18, avenue Edouard Belin, 31401 Toulouse, France  2: Freescale Semiconductor, 134, avenue Général Eisenhower, 31023 Toulouse, France  3: IMS, Université de Bordeaux 1, 33405 Talence, France


Soft defect localization techniques based on laser stimulation  have become key techniques for a wide range of FA/debug  issues. In this paper, we demonstrate the ability of these  techniques to solve critical design issue in mixed-mode device  for automotive application which includes analog, logic, RF  and power. Utilizing a wide range of laser stimulation  techniques, we have determined the most efficient approach  for this device to achieve the shortest cycle time. We have  established a clear link between fault isolation by laser  stimulation techniques and the abnormal behavior of the  device with relevant and complete simulation at transistor  level.


Currently, laser stimulation techniques have demonstrated a  wide field of application for failure localization and design  debug. The static techniques such as TLS (Thermal Laser  Stimulation) [1], [2], [3], [4] and PLS (Photoelectric Laser  Stimulation) [5], [6] are commonly implemented in the  industrial equipment. Using TLS, the device is heated with a  1300nm infrared laser beam to localize the abnormal resistive  issues. Using PLS, a 1064nm wavelength laser, scanning the  device, contributes to the electron-hole pairs generation in  active areas (silicon) and, as consequence, to the additional  photocurrent injection.


The results of extensive technology progression are: device  miniaturization, increasing number of metal layers as well as  interconnections and voltage reduction. Moreover, the  evolution of mixed-mode ICs shows that the surface area of  the digital blocks increases compared to the area of the analog  blocks. In addition, complex interface circuitry is integrated  between analog and digital areas. This progression  necessitates more complex failure analysis on the mixed-mode  devices presenting a functional failure (soft defect). Static  laser stimulation techniques are generally limited and are not  able to localize these types of critical failure. Consequently, new techniques and tools are required to localize sensitive or  failing regions.


Recently, new and various dynamic optical techniques based  on laser stimulation have been developed and introduced in  failure analysis laboratories of the semiconductor industry and  research, like: SDL (Soft Defect Localization) [7], RIL  (Resistive Interconnection Localization) [8], LADA  (Laser  Assisted Device Alteration) [9], DVM  (Delay Variation  Mapping) [10], T-LSIM (Thermal Laser Signal Injection  Microscopy) [11], etc. Some of them use the device  functionality to localize sensitive areas (SDL, RIL, LADA…), others are based on parametric measure (DVM, T-LSIM…).  Experimental results presented here were obtained on a  mixed-mode IC from Freescale. This device, designed in  SmartMOSTM technology, is particularly complex. It is  important to underline the singularity and complexity of  Freescale’s devices because they include on the same chip  digital, analog, RF and power electronic applications, plus  several interfaces circuitries between them. So we have to take  into account all these aspects for electrical diagnostic and  failure analysis, which requires a different approach in term of  defect localization and design debug in comparison to pure  digital CMOS technology devices.


This paper describes diverse methodology applied on mixedmode advanced Freescale IC to localize sensitive areas and to  support design solutions in the industrial context of TtM (Time to Market). Three different approaches (SDL, DVM & PVM) of DTLS (Dynamic Thermal Laser Stimulation) [12] techniques implemented on the Meridian tool are used to  successfully resolve a soft defect problem.


Soft Defect


Soft Defect is a term used to describe abnormal device  functionality in a certain range of voltage, temperature, frequency and/or time etc., covered by the product data  specification. One of the ways to characterize device behavior  and to verify the electrical failure is Shmoo plot [13]. It allows  the creation of 2D or 3D plots, useful for fixing experimental  setup conditions. It consists on variation of at least two of  above mentioned electrical or environmental parameters, and  then observation of the specified IC outputs. If the result is in


the product data specification range, the DUT (Device Under


fTx [MHz]


Test) is PASS, otherwise it is FAIL.


NN之之


Shmoo plot can be modified when DUT is scanned with a


0.8NN


之


FAIL


0.9N^^


laser source. This external optical stimulation can be sufficient


0.7√卜，


PASS


to locally change the electrical state of the circuitry. Two 0.60.5√NN√NLkinds of disturbances are possible: thermal (resistivity 0.4√N2variation and Seebeck effect) with a 1300nm wavelength laser 0.3√or photoelectric (charge carrier generation) with 1064nm


0.2√√


wavelength laser. When a backside analysis is required, in


0.1√NN


88.18.28.38.48.5→Vbat [V]


both cases, the near infrared lasers enough penetrate through  the silicon substrate. The disturbance occurs as a function of  the laser beam focalization and can modify static or dynamic  behavior of an IC. In that way Shmoo plot can change the  device response from PASS to FAIL or from FAIL to PASS. Finally the sensitive regions are localized by studying changes  in the device behavior as a function of the laser beam position. Note that the sensitive areas can correspond to the defect, the  design failure or represent a normal IC behavior.


Sample presentation


The studied device is an advanced mixed-mode IC processed  in 0.25µm SmartMOSTM technology. It contains four metal


frx [MHz]A layers with an additional copper layer on the top which 1√0.97


之之


prevents observation of the circuitry from the frontside. This


product, actually under development, will be used in the


0.7


automotive domain. In order to assure functionality in the


difficult environment condition linked to the application field,


the device should be working over a wide range of


temperatures.


88.18.2√8.38.48.5→Vbut[V]


The selected case study presents a functional failure occurring  only at high temperature. The failure description is detailed  below.


Failure description


The analyzed device was an example of the Soft Defect. The  DUT was only failing at high temperature (around 100°C) where no data transfer could be done. First electrical  diagnostic focused the failure analysis on the block  responsible for data communication which did not respond. Temperature dependant, frequency and voltage sensitivity was  also observed. Modifying voltage supply Vbat and data  transmission frequency fTx it affected the DUT temperature. Performing Shmoo plot, signal propagation and heat  dissipation should be taken into account. Indeed, the device  response delay depends on the voltage and frequency. Moreover, in certain conditions we could observe variable  delay between the output signal and the input signal.


The classical concept of Shmoo plot is used to identify the  defective conditions and to select accurately the  environmental and electrical IC parameters during the  analysis. Figure 1 presents Shmoo plot (fTx versus Vbat) when  the DUT is heated at 90°C.


Figure 1:  Shmoo plot: Vbat variations as a function of


frequency of the input Tx signal (Note: DUT heated at 90°C).


Due to the IC temperature sensitivity the thermal laser  stimulation technique (TLS) is selected (1300nm wavelength  laser source). Figure 2 presents Shmoo plot (fTx versus Vbat)when the device was scanned with a 1300nm wavelength  laser. The impact of a laser beam is noticeable and the Shmoo  plot highlights the temperature sensitivity of the device. Figure 2 shows that the device starts to fail at a lower Vbat value.


Figure 2:  Shmoo plot: Vbat variations as a function of


frequency of the input Tx signal, when the device is submitted  to the laser stimulation (Note: DUT heated at 90°C).


Analysis


To avoid masking effect of the copper and metal layers and to  increase the success rate of the failure localization, the  analysis was performed from the backside. The device was  mechanically thinned and polished down to 120µm substrate thickness.


SDL APPROACH


EXPERIMENTAL SETUP


The IC can be emulated in two different ways: with an  electrical tester or with the help of programmed µcontroller  and additional electronic equipments such as power supply, function generator, etc. Generally, the control of digital  signals and accurate IC diagnostic are more flexible through a  tester. However, in case of the mixed-mode devices, a  dedicated board represents a better solution. This board with a µcontroller assures analog functions as well as digital  functions and is commonly used in FREESCALE failure  analysis lab. In addition, in our case, variable device response  delay requires variable DUT running time before taking a  correct measure of PASS/FAIL state when Shmoo plot


performed. This constraint is easily resolved with a dedicated


board. The µcontroller also achieves reset of the device each


time when its output becomes FAIL. Otherwise the output


would stayed FAIL all time.


The only dedicated board limitation is the impossibility to


generate directly the signal representing the IC functionality s


。


as PASS/FAIL signal or analogue signal. Moreover, these


etlsignals need to be compatible with the video system  implemented on the laser scanner microscope (LSM) in order  to assure the synchronization between the laser beam position  and the IC status. DLS (Dynamic Laser Stimulation) module  is additionally implemented to continuously monitor the IC  output and to generate the PASS/FAIL state or the analogue  signals.


Figure 3 presents the experimental setup used to localize  sensitive areas of the IC. The DUT (Vbat = 8V & 8.2V) was  connected to the µcontroller which was managed by Freescale  developed software.


Figure 3: Soft Defect Localization (SDL): Experimental setup  using DTLS technique.


The environmental and electric parameters are selected to put  the device close to the failed condition. Voltage is nominal,


0科


temperature is fixed at 90°C with a thermal handler and the fTx frequency of square input is chosen at 250kHz. The output Rx  square signal, having the same frequency, is sent to an  oscilloscope and DLS (Dynamic Laser Stimulation) module. This last module converts the output signal into a PASS/FAIL  signal. The laser module is not synchronized with DUT fTx frequency. Pixel dwell time included at least three Tx loops. In these conditions, the PASS/FAIL signal is converted by the  imaging system to the 2D map and superimposed with the  pattern image to precisely localize the sensitive areas inside  the device.


SDL EXPERIMENTAL RESULTS


Using the above setup, the following electrical and SDL  results are found. Figure 4 presents the input Tx signal  generated by the µcontroller and the output Rx signal


converted, thanks to DLS module, into the PASS/FAIL signal.


In normal condition, the output signal should be square as the 6


input signal, slightly shifted in time and with a changed 0?0 amplitude level. In the failed condition the Rx output signal is


not following the Tx input signal and the FAIL level (1V) is


generated by the DLS module. Otherwise PASS level (0V) is


sent to the imaging system.


Figure 4: Plots of input Tx, output Rx and PASS/FAIL signals  during the experiment.


DUT at 90°C, Vbat = 8V, fTx = 250kHz.


2D PASS/FAIL SDL mapping is obtained on a Meridan tool, and is illustrated in figure 5. The white color corresponds to  the PASS signal (0V), the black areas describe the FAIL  signal (1V). Two cases are identified: a – FAIL to PASS, b – PASS to FAIL state alteration. In the first case the IC  temperature is set upper to the failed limit, just beyond 90°C, where the DUT is failed. When the 1300nm wavelength laser


LASERDLS ModulePASSIFAILlmaging


beam is scanning over the sensitive area the device becomes


System


<个


PASS. Similarly in the second case, the IC is working  correctly for the temperature set below 90°C. The scanning  laser beam heats enough the DUT to switch the state from


DUTRx


Oscilloscope


PASS to FAIL over the sensitive areas.


To see the different sensitive areas localization from both  cases, a white square corresponding to PASS area from figure


Temperature


TRIG(Tx)


5a (FAIL to PASS) was added on the figure 5b (PASS to


control


uController


FAIL).


a: FAIL to PASS (Vbat = 8.2V)  b: PASS to FAIL (Vbat = 8V)


Figure 5: Backside SDL results: Evolution of the DUT


sensitive areas under Thermal Laser Stimulation (TLS) for  two different Vbat values (temperatures). DTLS setup: Pixel  dwell time: 13.6µs, zoom: 20X, Laser power: 23mW.


This PASS/FAIL mapping superimposed with the IC pattern  results in a correct localization of the sensitive devices (Figure  6).


a: FAIL to PASS (Vbat= 8.2V)  b: PASS to FAIL (Vbat= 8V) Figure 6: Backside SDL results: superposition of the pattern  image with SDL mapping (zoom: 80X).


Tx


Rx


PASS/FAIL


PASS 0 FAIL ■


These devices are located in the same sub block of the data  communication block. PASS region from figure 6a  corresponds to bipolar transistor (Q3). FAIL regions from  figure 6b point to bipolar transistor (Q4), NMOS transistors (M15 & M16) and resistor (R4) (see Figure 11).


The technique described above is relatively fast and often  efficient to localize the sensitive areas on the mixed-mode  device although it has some limitations. The result is a binary  information : PASS or FAIL state while the abnormal  behavior can be described by the variable signal delay, the  frequency changes, the amplitude level changes, etc.


Moreover, in advanced technology devices the defect can  progressively change or even disappear with electrical testing. Changing state from PASS to FAIL, what is necessary to  generate the SDL mapping of the sensitive IC, it increases the  risk.


To avoid these constraints and to better extract useful  information, more precise technique, around PASS conditions  but without FAIL state, should be used. The idea is to focus  on the parametric analysis, dedicated to the analog blocks, based on the study of time delay, output voltage, current, frequency or any other parameter describing the IC abnormal  functionality. This kind of analysis can help to faster  understand IC abnormal behavior and find the failure.


DVM APPROACH


Second applied technique is based on the time delay study  through the Delay Variation Mapping (DVM) methodology. Indeed, just before the failed condition we could observe an  important variation of the time delay between the input signal (Tx) and the output signal (Rx). This parametric technique  exploits the following DUT behavior: when the device, in  functional conditions, is scanned by 1300nm wavelength  laser, a slight, variable time shift appears between the Rx  output signal and the Tx input signal. This delay is converted  into variable voltage amplitude of an electrical signal with a  TAC (Time to Amplitude Converter) module and then sent to  the imaging system. Figure 7 presents the experimental setup.


Figure 7: Delay Variation Mapping (DVM): Experimental  setup using DTLS technique.


In comparison to the SDL technique, DVM requires  synchronization between IC activation and laser scanning (pixel clock signal). The localization system detector has a


fixed measure moment and time. The TAC output is a pulse  signal of variable amplitude, proportional to the time delay  between its two inputs, and not a continuous signal. The  perfect synchronization is applied.


In our case, DVM analysis takes more time to obtain 2D map  than SDL analysis because the synchronization between the  pixel clock and the laser position has to be taken into account. For the input frequency fTx chosen at 10kHz and applied  through the function generator (FG), it is not a critical point. We need 26 seconds to acquire an image 512x512 with DVM  technique instead of 5.3 seconds for the same resolution image  with SDL technique. The DUT is heated at 90°C.


DVM EXPERIMENTAL RESULTS


Figure 8 presents results obtained by using the above setup. This DVM case is shown for the temperature below 90°C. Distinct behavior of the DUT is observed when the  temperature of the device has changed. The black color  corresponds to the areas where there is no timing shift  between Tx and Rx signals induced by the laser stimulation (normal time delay propagation). The white and gray colors  describe areas where a positive, variable delay between Tx  and Rx signals is detected due to the laser stimulation (time  delay propagation increased). The bipolar transistor (Q4), NMOS transistor (M15) and resistor (R4) are accurately  localized.


Figure 8: Backside DVM results: sensitive area under


Thermal Laser Stimulation (TLS) for the temperature below


Rx尚


90°C (zoom: 80X).


LASERTAC


Imaging System


A high similarity between figure 8 and 5b (SDL: PASS to  FAIL) is observed. In both cases, the same structures are  sensitive when the DUT is scanned with 1300nm wavelength


DUT←TRIG OOscilloscope


laser, however with DVM technique the localization is more  precise. It confirms that the failure is located in the localized


二


sub-block.


FG


Temperature control


nController


PVM APPROACH


Phase Variation Mapping (PVM) is a second parametric  technique used to localize the sensitive areas. This technique  allows detection of the phase, amplitude or duty cycle  variation by multiplying two periodic signals of the same  frequency: the reference and the DUT output. As observed  before, when the device is scanned with 1300nm wavelength


Q4


M15


R4


laser, the phase of the output Rx signal varies. Staying in the  PASS state and changing the temperature of the DUT it is  possible to register a different mapping of this variation. Figure 9 presents the experimental setup. The fTx frequency of  square input is chosen at 500kHz and applied through the  function generator (FG). The DUT temperature is set below  90°C. The output signal Rx is multiplied by the square, reference signal (TRIG) of the same frequency and in time  quadrature. This particular setup conditions is favorable to  detect phase changes [14]. Afterwards the DC component is  extracted and amplified before sending to the imaging system.


VDDVDD


TRIG


LASERD>0>DC


System牙--Imaging


Q4193


290°专


+R4


MITM5


Figure 9: Phase Variation Mapping (PVM): Experimental  setup using DTLS technique.


PVM EXPERIMENTAL RESULTS


Interesting results are obtained with the PVM parametric  technique. Figure 10 presents PVM results for two different  temperatures below 90°C. The bipolar transistors (Q3 & Q4), NMOS transistor (M15) and resistor (R4) are again well  localized. The white color corresponds to the Rx signal  acceleration. The black color corresponds to the Rx signal  delay. Grey, homogeneous area describes no changes in the  propagation time. When the temperature is changed step by  step it is possible to register the evolution of the Rx signal  phase variation. During this evolution for each simple device  the delay and acceleration are observed.


Among various techniques tested and applied on this case  study, PVM technique gives the most precise mapping results


T-25C


T=100C


50


and the best sensitivity.


4.0


a: T


b: T+tT+4t


Figure 10: Backside PVM results: Evolution of the DUT  sensitive areas under Thermal Laser Stimulation (TLS) for


two different temperatures below 90°C (zoom: 80X).


VALIDATION THROUGH CADENCE SIMULATION


All localized devices are identified and located in one IC sub  block, inside the data communication block. Its simplified  electrical schematic extract is presented in figure 11. The  dashed square corresponds to the PASS device from figure 6a, the continuous squares describe the FAIL devices from figure  6b when SDL technique is used. In order to confirm a failure  and point at the failing device, electrical simulations are  performed on this sub block.


Figure 11: Simplified electrical schematic of sub block


highlighted by DTLS techniques and simulated in Cadence.


Signal propagation is observed for room (Figure 12a) and high  temperature (Figure 12b). V1 and V2 signals should switch  simultaneously. It properly works at 25°C. At higher  temperature the threshold voltage is reduced because of the  material property [15]. In consequence V1, V2, V3 and Vout  signals switch earlier. Moreover, the abnormal behavior of the  V2 signal is observed. Its low level reaches 0.9V instead of


0.4V with a slightly degraded edge. As a result, the switch of  V3 and Vout signals, having a threshold voltage at about 1V, is delayed.


M15 transistor is the root cause of the failure. Its properties  did not allow the correct functionality of this sub block. The  resistance Rds of M15 is strongly dependent on temperature. The failure mode is due to the undersized NMOS transistor. This case study is an example of the design failure.


Figure 12: Electrical simulations: Plot of signal propagation  in sub block highlighted by SDL at 25°C (a) and 100°C (b). V1: , V2: , V3: V1:7,V2:,V3:,Vout:o., Vout: .


右V1


DUT


所M16'M6


V2


V3


Vout


yw


Q3


13


O A2.0


02.0


AJ3.0


83.0


The goal of each analysis is firstly to localize the failure and  secondly to collect as much information about the failure  mechanism as possible. The latter aim is more important when  the matter is in the design weakness and not physical defect. In addition, for the mixed-mode devices its functional  behavior like phase variation, signal delay variation or  amplitude level changes, is more difficult to analyze.


The SDL technique, resulting in the binary response, does not  allowed to register more than two sensitivity levels. Hence, we  have less information about sensitive areas, however the most  sensitive zones are pinpointed. From the point of view of the  industrial application the results are easier to interpret. Moreover, most of time this technique is easy to implement  and efficient.


Comparing to the parametric DVM or PVM techniques, the  SDL technique is less precise. In case of the mixed-mode  devices, where the simple structures have different  dimensions, it is possible to miss localization of the failing  device. Therefore, the parameter that is more important than  image resolution, as it is in case of digital ICs, is the  sensitivity.


With DVM and SDL techniques the same sensitive structures  were localized. However, the DVM gave more information  because different sensitivity levels can be measured. This  technique is more precise and efficient but takes more time to  prepare the setup. It can be only used for the phase or duty  cycle issues.


The PVM technique is the most sensitive of three applied  techniques. However, providing more information than SDL  or DVM, it can be complex to analyze its results. It is easy to  setup and it can be used for the phase, duty cycle or amplitude  issues.


100 nm


Figure 4a: 2x magnified area of Fig. 3a (effective  magnification is 400,000x) before image processing.


Figure 4b: 2x magnified area of Fig. 3b (effective  magnification is 400,000x) after image processing.


In conclusion, we have shown that blind deconvolution is a  useful technique for improving images at the limit of  resolution in the SEM. However, the long acquisition time  required obtaining the appropriate signal-to-noise ratio place  significant restrictions on the SEM stability and the sample  robustness.


Figure 5a: SEM of gold sputtered cross-section, 200,000x  magnification.


Figure 5b: Same image as Fig. 5a following application of  blind deconvolution.


Figure 6a: 3x magnified area from Fig. 5a (effective  magnification is 600,000x) prior to image processing.


Figure 6b: Magnified area from Fig. 5b (effective  magnification is 600,000x) after image processing. Note the  thin filament that could not been seen prior to processing.


Figure 7: Image intensity vs. pixel number of a line plot from  the left side of Fig. 1, before and after deconvolution.  The  higher peaks, lower valleys, and greater detail are indicative  of improved resolution.


[1]  W.E. Vanderlinde, Proceedings of the 29th International  Symposium on Testing and Failure Analysis, ASM  International, p. 158 (2003).


[2]  A.C. Diebold, Handbook of Silicon Semiconductor  Metrology, Marcel Dekker, New York, p. 854 (2001).


[3]  J.N. Caron, N.M. Namazi, and C.J. Rollins, “Noniterative blind data restoration by use of an  extracted filter function,” Applied Optics, Vol. 41(32), p. 6884 (2002).


[4]  Y. Sudo, N. Baba, N. Miura, S. Ueno, and R. Kitai, "Application of self-deconvolution method to shift-andadd solar imaging," Applied Optics, Vol, 45, p. 2707 (2006).


[5]   E. S. Barriga, G. Erry, S. Yang, S. Russell, B. Raman, and P. Soliz, "Application of adaptive optics in retinal  imaging: A quantitative and clinical comparison with  standard cameras."  Proceedings of SPIE -- Volume  5688, Ophthalmic Technologies XV, p. 152 (2005).


[6]  C.W. Helstrom, "Image Restoration by the Method of  Least Squares," Journal of the Optical Society of  America, 57, p. 297, (1967).


[7]  D. Slepian, "Linear least-squares filtering of distorted  images," Journal of the Optical Society of America, Vol.  57, p. 918 (1998).


[8]  W.H. Richardson, “Bayesian-Based Iterative Method of  Image Restoration”, Journal of the Optical Society of  America, Vol. 62, p. 55, (1972).


[9]  L.B. Lucy, “An iterative technique for the rectification  of observed distributions”, Journal of Astronomy, Vol. 79, p. 745, (1974).


[10]  S. F. Burch, S. F. Gull, and J. Skilling. “Image  restoration by a powerful maximum entropy method,” Computer Vision, Graphics, and Image Processing, Vol. 23(2), p. 113, (1983).


[11] N. Wiener, The Extrapolation, Interpolation, and  Smoothing of Stationary Time Series with Engineering  Applications, (Wiley, New York, 1949).


[12] C.C. Cunningham, and D. Anthony, “Image  deconvolution of extended objects - A comparison of the  inverse Fourier and the Lucy techniques,” Icarus (ISSN  0019-1035), vol. 102, no. 2, p. 307-315 (1993).


[13] J. R. Fienup, D. Griffith, L Harrington, A. M. Kowalczyk, J. J. Miller, and J. A. Mooney, “Comparison  of Reconstruction Algorithms for Images from SparseAperature Systems," Proc. SPIE 4792-01 (2002).


[14] G.R. Ayers and J.C. Dainty, “Iterative blind  deconvolution method and its application,” Optics  Letters, Vol. 13, p. 547 (1988).


[15] D.G. Sheppard, B.R. Hunt, and M.W. Marcellin, “Iterative multi-frame super-resolution algorithms for  atmospheric-turbulence-degraded imagery,” Journal of  the Optical Society of America A, Vol. 15(4), p. 978 (1998).


[16] D. Kundur, and D. Hatzinakos, “A novel blind  deconvolution scheme for image restoration using  recursive filtering,” IEEE Transactions on Signal  Processing, Vol. 46(2), p. 375 (1998).


[17] T.J. Holmes, “Blind deconvolution of quantum-limited  incoherent imagery: maximum-likelihood approach,” Journal of the Optical Society of America A, Vol. 9, p. 1052 (1992).


[18] T.J. Schulz, “Multi-frame blind deconvolution of  astronomical images,” Journal of the Optical Society of  America A, Vol. 10(10), p. 1064 (1993).


[19] A.S. Carasso, “Direct Blind Deconvolution,” SIAM  Journal of Applied Mathematics, Vol. 61(6), p. 1980 (2001).


Nondestructive Defect Imaging Through Image Intensity Analysis


J. Demarest*, D. Bearup**, A. Dalton, L. Hahn***, B. Redder, F. Wallingford


IBM, Hopewell Junction, NY USA


* Currently at IBM, Albany, NY USA ** Currently at RPI, Troy, NY USA *** Currently at AMD, Austin, TX USA


The continually shrinking dimensions of today’s  semiconductor technology occasionally allow for novel  approaches in imaging defects. It has become desirable to  image subsurface voids prior to cross sectioning and some  efforts have been made to address this need including the  construction of specialized instrumentation [1]. The thickness  of the metallization levels at the 65 nm technology node and  smaller now allow for the use of the electron beam in a  scanning electron microscope (SEM) as a material sensor. At  high accelerating voltages (between 20-30 kV) in backscatter  imaging mode the numerical gray level values at each pixel  location can correlate to the amount of material directly under  the electron beam at that location. This is particularly evident  when dealing with defined geometries and material sets  offering high contrast changes between materials such as  those found in semiconductor technology like copper (Cu) metal and conventional dielectric materials. As a result, subsurface voids can be mapped to a reasonable representation  prior to cross sectioning and precise pinpointing of the defect  location in test structures can occur. This paper discusses this  methodology on 65 nm technology with Cu metal lines in a  low-k dielectric material for a two level metal test structure. To some extent this work represents a natural extension of a  paper presented previously by the author [2].


Given the existing trends within the semiconductor industry, today’s integrated circuits (IC) continually shrink in  dimensionality and increase in complexity. Current state-ofthe-art IC technology can have upwards of 10 metal levels and  multiple dielectric materials. This evolutionary process allows  for new opportunities for the failure analyst as the very nature  and construction of the hardware we work on changes. One  such opportunity has arisen due to the decreasing thickness of  metal wiring. The electron beam of conventional scanning  electron microscopes (SEM) can be used to map out  subsurface voids by sensing changes in image intensity caused  by the absence of metal in what should be fully dense metal  features. These changes in intensity are not readily apparent to


the human eye and thus this technique allows for additional  characterization and localization of the defect before  destructive cross sectioning takes place.


It has previously been shown by Gignac et al. that subsurface  defects can be detected using a transmission electron  microscope (TEM) with a scanning attachment by collecting  backscattered electrons (BSEs) with an accelerating voltage  on the order of 30-400 keV [1]. Specifically, 0.2 μm voids  were successfully detected below 0.65 and 3 μm of Cu metal  and conventional dielectric material using beam energies of 30  and 150keV, respectively. The use of high beam energies and  customized equipment improved the visual observation of  variations in patterned Cu.


Experimental Technique


The work discussed here uses a SEM with a lower  accelerating voltage (ranging from 15-27 kV) to detect  subsurface voids primarily using a beam energy of 27 kV. It  will be shown that voids as small as 17 nm can be detected  beneath 375 nm of copper metal using this technique. BSE  were collected to obtain a higher contrast between the metal  and nonmetal portions of the sample. The subsurface voids  cause changes in image intensity because of the lack of metal  mass when compared to a healthy part of the structure. These  changes in intensity (on the order of 10-30 gray levels) can be  translated to a 3-D difference map, relating to void thickness. A dual beam focused ion beam (FIB/SEM) was used to cross  section and image samples in order to characterize observed  changes in image intensity caused by the void to the physical  attributes of the void. The results validated the capability of  this technique as a non destructive method to locate and  visualize subsurface failures.


Reliability failure analysis often requires utilizing different  defect isolation techniques to localize defects on fully  constructed test chips in conjunction with extensive  delayering practices. The defects discussed here were part of a  stress migration (SM) performance study and represented an  extreme of the process variation. As a result the wafer  demonstrated a near 80 percent failure rate for the structure


under examination after being stressed at elevated temperature  for an extended period of time.


Figure 1: Schematic of the test structure examined during this  work. (A) Lower magnification top down view. (B) Higher  magnification of a small area of the test structure. (C) Cross  sectional view of the structure. The lower metal level is  represented by orange, the upper level by green, and the  interconnect level by yellow. The expected location of the void  is shown in (C).


The chips consist of multiple levels of Cu metallization in a  low-k dielectric at the 65 nm technology node. The test  structure examined consisted of two Cu metal levels  connected by a Cu interconnect. The lower level of the  structure is composed of large Cu metal plates which act as a  vacancy reservoir (Fig. 1). Voids were expected to form  directly under the interconnect location due to the higher  stresses associated with these types of features.


Figure 2: BSE SEM top down of failing link. Intensity as a  function of position is plotted. The upper end of the link  indicates a slight reduction of intensity in the profile  signifying the subsurface void location.


Figure 3: Spreadsheet color contour maps of healthy link (left) and failing link (right). Higher intensity corresponds to a  brighter pixel in the observed SEM image.


The defects in the test structure were isolated by using passive  voltage contrast in a SEM at accelerating voltages ranging  from 500 V to 5 kV. When a fail location was identified a  BSE image was acquired at about 80000X magnification and  27 kV (Fig. 2). The numerical intensities in the image  composing the regions surrounding the link ends were  extracted to a spreadsheet program such as Microsoft Excel or  Lotus 1-2-3 through custom written code. This allows for a  numerical representation of the individual pixel intensities and  a high level of control over subsequent mathematical  operations upon those intensities. The intensities values  corresponding to the two link ends are oriented identically and  aligned on a pixel by pixel basis. A color contour map of the  two link ends is shown in Fig. 3. The individual pixels  intensities can then be subtracted from each other to generate


a 3-D topography map (Fig. 4). This map can be viewed as a  reasonable approximation to the defect void and shape. Comparison cross sections were generated between failing  interconnects and adjacent healthy interconnects to rule out  intensity variations due to geometrical differences (Fig. 5). Consequently the observed variation in intensities is  predominately due to variations in metal mass due to the  presence of the void.


In an effort to understand the relationship between void  thickness and intensity ten fail sites were examined through  the described technique. The results of the change in intensity  between a healthy interconnect and a failing interconnect were  plotted as a function of void thickness as determined through  cross sectional analysis (Fig. 6). There is a slight decrease in  slope at the lower end of the intensity change on the x-axis.  This is may be a result of approaching the boundary of  sensitivity for this technique. Eliminating the curve at the  lower end of the intensity change, the slope (dt/dI) of the line  obtained is about 17 nm/gray level. This tells us that for every  17nm of void thickness, there is a loss of 1 gray level (GL) in  image intensity for this specific sample configuration.


Figure 4: Topographical contour map of subtracted  intensities generating an approximation of the defect void size  and shape.


Reference


Figure 5: Cross sectional comparison of a healthy reference  interconnect (left) and an adjacent failing interconnect (right). These two images indicate little geometrical variation in  structure profile.


Removal of approximately 75% of the metal over the  void demonstrated an increased variation in intensity on the  order of 50-70% which indicates the potential for improved  sensitivity through this technique as the thickness of the  metallization decreases with technological evolution. A range  of accelerating voltages were selected and applied to a sample  to examine the effect of this parameter upon this technique. The values selected for use were 15, 20, 25 and 27 kV. After  imaging with the SEM and making an intensity difference  map, sections of the via were chosen along the width and  length to show the effect of accelerating voltage. Averaging  20 pixels along the length and width was performed to ensure  a reasonable representation of the average intensities over the  structure (Fig. 7). All four accelerating voltages show the  same trend in intensity profile. For the void thickness along  the length and width of the via, 20 and 25kV appear to be the  most sensitive accelerating voltage due to the larger dynamic  range of intensity.


0 20 40 60 80 100 120 140


9


10


11


12


14


15


16


ΔΙ (graylevel)


Figure 6: Plot of change in intensity versus change in void  thickness indicating a sensitivity of this technique on the order  of 17 nm of void thickness per gray level.


Void


-30-20-10 0 10


60


Position (pixel)


15kV 20kV 25kV 27kV


45


Figure 7: Plots of intensity as a function of position with  variations in SEM accelerating voltage.


It has been demonstrated in this paper that high magnification  SEM BSE images can be used to determine the location and  relative thickness of a subsurface void through the use of  intensity subtraction. For the given sample conditions and  geometrical configuration examined the sensitivity of the  technique was determined to be on the order of 17 nm/GL  with improvements in sensitivity to be expected as  metallization thicknesses decrease at subsequent technology  nodes. The observed intensity variations are almost entirely  due to the presence of the void due to the near identical  geometrical nature of the paired interconnects. The most  sensitive accelerating voltages for this technique appear to be  in the range of 20-25 kV.  While this work has been  performed upon stressed test sites as part of a reliability  evaluation, it would be possible to use it to evaluate  subsurface defects from yield failures.  Examples of such  failure modes of interest might include variations in metal  trench profiles which might lead to local resistance increases  due to changes in cross sectional line area.


[1] Gignac, L. M., M. Kawasaki, S. H. Boettcher, and O. C. Wells. "Imaging and Analysis of Subsurface Cu  Interconnects by Detecting Backscattered Electrons in the  Scanning Electron Microscope." Journal of Applied  Physics 97 (2005).


[2] Demarest, J., “Image Intensity Analysis for Defect  Localization Utilizing SEM BSE Imaging.” Conference  Proceedings from the 32nd International Symposium on  Testing and Failure Analysis.  2006. 289-292.


Automated TEM Sample Preparation on Wafer Level for   Metrology and Process Control


Bart Rijpers


ASML, R&D Department, CD Metrology, Veldhoven, The Netherlands  bart.rijpers@asml.com, Phone: +31 40 268 5721


Dick Verkleij


FEI, NanoElectronics Business Group, Eindhoven, The Netherlands


Eckhard Langer


AMD, Materials Analysis Department, Dresden, Germany


As the feature size of semiconductor technology shrinks, cross-section metrology becomes more and more challenging. The generation of cross section metrology data is important  for the introduction of new advanced integration schemes, rapid yield learning, and continuous process control for stable  manufacturing. In this paper an automated way of TEM crosssection preparation by FIB is described to ensure fast cycle  time for preparation and analysis. A dual column FIB/SEM  system is used to prepare TEM samples from multiple  locations of a 300 mm wafer batch. Subsequently, the TEM  lamella is transferred to a grid using an ex-situ lift-out station. Two dedicated applications are shown, a Focus Exposure  Matrix (FEM) on patterned photo resist and a process control  case study on an etched poly-silicon transistor gate.


Device dimensions continue to shrink as predicted in the ITRS  roadmap. Currently, leading edge manufacturers are preparing  the 45 nm technology node for the production ramp. The  typical time offset between the R&D phase and the year of


production is assumed to be 3 years or shorter. Table 1 shows  typical feature sizes after litho/etch patterning processes for  today’s and future technology nodes and the methods used for  metrology. Although the table shows a clear introduction date  of new techniques, proven techniques such as top down CDSEM after litho and etch processes will continue to be utilized  throughout the introduction of further technology nodes. In  most cases, cross section metrology is used to assist in-line  metrology where top down inspection is not able to reveal the  information needed, like capping layer open etch steps or  profile inspection in the poly gate processes (e.g. footing, side  wall profile). Furthermore, cross section metrology is needed  for the development and optimization of resist and etch  processes, to calibrate in-line metrology equipment like CDSEM, Optical CD Metrology (OCD) or film thickness  measurements. There are other applications where in-line  metrology would be required, but cannot be used for technical  reasons. For example, monitoring of barrier step coverage, cavity etch processes in the SiGe module, or poly gate spacer  features can not be characterized in-line. Due to the shrinking  feature sizes and the new applications, cross section metrology  is challenged to deliver the required resolution [1]. Hence the  adapted ITRS roadmap (Table 1) shows a transition point  from SEM to TEM around 2006 for R&D, because crosssection TEM can disclose more technological details than


Table 1: ITRS Metrology Roadmap – 2006 Update (adapted from [9])


Technology Node


90 nm 80 nm 70 nm 65 nm 50 nm 45 nm 32 nm


Year of Production (HVM)


2004


2005


2006


2007


2009


2010


2013


R&D


2001


2002


2003


DRAM ½ Pitch (nm) (contacted)


70


65


32


MPU/ASIC Metal 1 ½ Pitch (nm)


107


78


68


52


MPU Physical Gate Length (nm)


37


28


18


Flash ½ Pitch (nm)  (Un-contacted Poly)


---


76


64


57


Cross Section Metrology


None


FIB-SEM FIB-SEM FIB-SEM FIB-TEM FIB-TEM FIB-TEM


crosssection SEM. Consequently, TEM sample preparation is  becoming more and more important, being a crucial step for  successful metrology. Two approaches are used nowadays: the  in-line extraction of a fully prepared TEM lamella or the inline extraction of a bulky sample for further preparation in an  off-line laboratory, or the in-line extraction of a. In this paper, we pursue the first option.


Cross Section Metrology Flows


The general flows for cross section metrology are described in  Fig. 1. One standard method that has been used for a long time  in the industry is cleaving the wafer in an off-line laboratory  for 90° SEM inspection. This implies the disadvantage that the  wafer cannot be processed further. In the late 1990’s, dual  column systems were introduced, allowing the FIB  preparation of local cross sections for tilted view SEM  inspection. The image resolution of the SEM columns, being  in the range of 3 nm or slightly better, is sufficient for some of  the metrology task in technology nodes up to 65 nm. For the  45 nm technology node and beyond, TEM has to be used more  frequently.


Figure 1: Flow Chart Process Control- Cross Section  Techniques


For TEM cross section metrology there are currently two  flows in use. Flow 1, which is pursued in this paper, uses a  FIB/SEM for fully automated TEM sample preparation with  subsequent manual lift-out. Flow 2 cuts bulky samples free  from the wafer in order to process them further in an off-line  laboratory. Both flows allow further processing of the wafer, which is a substantial benefit for manufacturing. While flow 1  is commonly applied for routine applications, flow 2 seems to  be appropriate for defect or root analysis in cases of process  excursions. More information about flow 2 can be found in


[2], [3], [4].


TEM sample preparation flow


We used the following equipment to perform the automated  TEM sample preparation and cross-section metrology:


1. DualBeam Expida 1275 with IC3D software for  automated TEM sample preparation on 300 mm  wafers on multiple locations. The system can run a  batch of wafers (FOUP).


2. Lift-out station: Olympus MX61-L 300 mm optical  microscope with motorized stage and Narishige  micromanipulator


3. Tecnai F20 X-TWIN: imaging of the cross section  with STEM or TEM.


4. IC3D offline software: software package to perform  metrology


Fig. 2 shows an automated TEM sample process flow image  sequence as performed in the DualBeam Expida 1275.


Figure 2: TEM sample preparation flow on DualBeam  FIB/SEM


The following steps are performed:


1. Two Pattern recognition Marks (PM) are made with  the FIB by depositing platinum squares and  subsequent PM  milling


2. Result after coarse milling of one ‘stairs’ Contour  with the highest ion beam current


3. Result after milling a second ‘stairs’ contour


4. After cut loose: FIB mills a “U” shape to separate  bottom and sidewalls from the bulk at 7° stage tilt


5. After further thinning of the sample with lowest  beam current


6. After Final Cut to cut the lamella loose. The lamella  is ‘floating’ by electrostatic forces ready for ex-situ  liftout.


The automatically prepared samples were imaged in High  Resolution STEM mode as well as in STEM mode in a TEM (see fig. 3). The samples were not plasma cleaned.


The STEM image in figure 3a illustrates the sufficient sample  quality for regular monitoring purposes. Figure 3b shows a  lattice image in HR-STEM at 10 Mx magnification. Taking  into account that the sample preparation was not operator  controlled, a reasonable overall quality of the lamella was  reached. Although a certain amount of side wall  amorphization was expected, lattice imaging of the silicon  substrate could be performed.


Figure 3: a) HAADF-STEM image of 193 nm photoresist  dense line pattern (110 kx). b)HR-STEM image of an


automated prepared TEM lamella of silicon <1 1 0>, 10 Mx  magnification


Yield and turn around time


During 2006, the yield of the automated TEM sample  preparation recipe was increased. The preparation yield  improvements are shown in Fig. 4. A stable process was  reached in December, resulting in an average yield of 92%. During this month, 73 samples were prepared fully  automatically.


Turnaround time while using this process is three days (for 16  samples); During the day the system is used for programming  and manual tasks. At night the automated recipes will run. Night 1 is used for deposition of a protective layer, night 2 for  TEM sample preparation, and day 3 for TEM imaging. Within  three days feedback about a complete batch of wafers will be  provided, enabling short feedback loops for e.g. photoresist  evaluation. Turnaround can be improved to two days, a  process discussed more extensively in the Discussion and  Future Improvements section at the end of this paper.


Sample thickness variation


In the standard recipes, the TEM lamella thickness is targeted  at 100 nm. If the thickness target is reduced, yield and quality  reductions are encountered. The lower limit for lamella  thickness was found to be in the 60-70 nm range. The sample  thickness variation is in the order of 12 nm (3σ), comparable  to [8].


0 10 20 30 40 50 60 70 80 90 100


28/09/200605/10/200612/10/200619/10/200626/10/200602/11/200609/11/200616/11/200623/11/200630/11/200607/12/200614/12/200621/12/200628/12/200604/01/200711/01/2007


Figure 4: Yield automated TEM sample preparation including  manual lift-out. Average yield in December 2006 was 92%


Ex-situ Lift-out


For the manual transfer of TEM samples to the TEM grid, an  ex-situ lift-out station was designed. It uses a motorized 300  mm stage which can be navigated using wafer maps. A CCD  camera on the microscope is used for pattern recognition (automated wafer alignment) and to save images of the TEM  grid for sample logistics. LabView software aligns the wafer  and drives to the target location based on wafer map  information from inline wafer metrology tools. An oil  hydraulic micro manipulator lifts the sample to the TEM grid. For convenient sample manipulation, a large depth-offocus/large working distance microscope objective (1000x  magnification) is used. In fig. 5, the lift-out station is shown in  a clean room. The right side of the figure shows a TEM  sample of approximately 10 µm width on a glass needle. With  this lift-out station it is possible to navigate quickly on a  300mm wafer, reducing the time needed for the lift out and  improving the success rate.


Figure 5: Lift-out station (left) and TEM sample on glass  needle (right)


Applications


Lithography Metrology


Up to the 80 nm technology node and higher, cleaved cross  sections are used to optimize photoresist processes. Side Wall  Angle (SWA) data was gathered from these images to select  the best process. This changed for the 70 nm node for two  reasons:


1. Variation between different lines became too large, as different engineers select different “best” process  settings. A quantitative technique was needed.


2. Comparison of different types of Metrology tools  became important. The need for Cross Section  Metrology data to compare e.g. CD-SEM (1D) with  OCD (2D) was needed.


Figure 6 shows the evolution from cross-section imaging to  cross-section metrology (FIB/SEM) towards calibrated STEM  metrology. It is a transition from qualitative process control to  quantitative process control. The final goal is calibrated  process control for the 45 nm technology node. Before a FIB  cross-section can be prepared, a protective coating needs to be


Platinum


Photoresist


applied. We use in-situ electron beam assisted platinum  deposition [10]. The advantage of this method is that it can be  applied locally and that it can be automated. A disadvantage is  that is takes a relatively long period of time for photoresist. The reason is that certain photo resists (e.g. the resist used at  193 nm exposure wavelength) are sensitive to e-beam  exposure. Therefore, the e-beam platinum deposition process  was optimized extensively to ensure that the resist does not  change during the protection phase. It is also possible to  prepare TEM samples without the need of a protective coating


[6], but this method is difficult to automate.


As an example, we show a process optimization at the 50 nm  node. Both cleaved cross sections and FIB prepared cross  sections were used. Cleaved Cross Section Images from an  offsite SEM lab are shown in Fig. 7. Cross-section metrology  data for these cleaved wafers is shown in Fig. 8, labeled as  wafer ID 1 to 4. From Fig. 7, it is difficult to decide which  process is the best one based on side wall angle (SWA). The  lines look tilted and metrology is not possible on these kinds  of images. Based on cross-section metrology data (SWA) shown in Fig. 8, process 1 was selected as the best process.


Multiple cross sections are generated to minimize  measurement noise. In this case, an average value was  calculated for bottom CD (BCD) and Side Wall Angle


(SWA).


Fig. 8 shows that the range of BCD values for the lines being  measured is between 10 and 18 nm. A better estimate for BCD  can be found when the average BCD value of approximately  90 lines is used. This will reduce a variation of 15 nm 3σ to  15/√90 = 1.6 nm 3σ. Now we are able to compare CD-SEM  metrology results to STEM metrology results.


The wafers are sent to CD-SEM to determine best energy and  focus settings in the Focus Exposure Matrix (FEM) for the  litho scanner. At selected locations cross section metrology  was performed. Target BCD at CD-SEM is 50 nm. There is a  difference between BCD value measured with CD-SEM and  with a cross-section STEM (table 2).


Figure 8: Cross Section Metrology results for wafer batch of 9 wafers (SWA on left Y-axis, BCD and BCD-range on right Y-axis)


80 nm Node and higher


50, 65 and 70 nm Node


45 nm Node and smaller


Cleaved Cross Section (XS)


FIB prepared XS


FIB prepared STEM Cross Section


Figure 6: Cleaved cross section (left), FIB/SEM Cross section  (center) and DF-STEM cross section (right)


Figure 7: Process ‘optimization’ based on Cross Section  Imaging (cleaved cross section images from offsite SEM-lab)


It is obvious that there is a correlation between SWA and  BCD. When the SWA is high (87º), the BCD value measured  by STEM is deviating more from the target BCD of 50 nm. When the lines are more sloped this offset is less pronounced. This is shown in Fig. 8. A lower purple bar (SWA) results in a  higher yellow bar (BCD). That the offset between CD-SEM  and STEM is dependent on the SWA is also in agreement with


Many approaches are able to resolve the same problem. Moreover, there exists other complementary and also nondestructive techniques like LADA (Laser Assisted Device  Alteration) [16] or PICA (Picosecond Imaging Circuit  Analysis) [17], etc. which could also be used. Anyway, the  success mainly depends on a good investigation of an  electrical diagnosis. Choice of electrical and environmental  parameters plays important part in the soft defect localization.


Design issue in industrial mixed-mode device has been  overcome by precise fault isolation with three DTLS  techniques (SDL, DVM and PVM) and advanced simulation  on the faulty area. The conjunction of DTLS accuracy and  simulation on mixed mode-device (analog, logic, RF and  power) is the main outcome of this paper. The mostly analog  techniques (DVM, PVM) used for sensitive area localization  are different from those used in the case of digital circuits.


The electrical setup constraints have been highlighted. The  tools used for sensitive area localization were different from  those used in the case of digital circuits. The electrical tester  was replaced by µcontroller and the analog functionality was  assured through specified board and additional electronic


tools. Three DTLS techniques were applied from the backside  of a failing mixed-mode IC and sensitive regions were  successfully localized. The parametric techniques (DVM & PVM) gave more precise results than the SDL technique. Afterwards the electrical simulations were performed on the  failing sub block and correlated with the electrical failure at a  high temperature. Finally, the design failure was confirmed  with very low cycle time of a few days.


In the discussion the different approach of mixed-mode  devices compared to the digital ICs was underlined and the  importance of the electrical setup was noticed.


The authors are very grateful to A. Colombie and T. Bousquet  from Freescale for the design support and useful information  about device functionality. We also wish to thank A. Clark  from Freescale for helpful discussion and A. Deyine-Barth  from Credence for her technical assistance.


[1] K. Nikwa and S. Tozaki, “Novel OBIC Observation  Method for Detecting Defect in Al Stripes Under Current  Stressing”, ISTFA, 1993, p303- 310.


[2] K. Nikawa and S. Inoue, “New Capabilities of OBIRCH  Method for Fault Localization and Defect Detection”, ATS, 1997, p214-219.


[3] K. Nikawa, “Failure analysis case studies using the IROBIRCH method”, Test Symposium, 1999, p394-399.


[4] F. Beaudoin et al, “Principles of thermal laser stimulation   techniques”, Microelectronic Failure Analysis Desk  Reference, 2004, p417-425.


[5] T. Wilson and E. M. MacCabe, “Theory of optical beam  induced current images of defects in Semiconductors”, J. Appl. Phys. 61(1), 1987, p191-195.


[6] K.C. Stevens and T.J. Wilson, “Locating IC defects in  process monitors and test structures using optical beam  induced current”, Microelectronic Engineering, Vol.12, 1990, p397-404.


[7] Michael R. Bruce et al, “Soft Defect Localization (SDL) on ICs”, ISTFA, 2002, p21-27.


[8] E.I. Cole et al., “Resistive Interconnection Localization”, ISTFA, 2001, p43-57.


[9] J. A. Rowlette et al, “Critical Timing Analysis in   Microprocessors Using Near-IR Laser Assisted Device  Alteration (LADA)”, ITC, 2003, p264-273.


[10] K. Sanchez et al, “Delay Variation Mapping induced by  dynamic laser stimulation”, IEEE International, 2005, p305-311 .


[11] R. A. Falk et al., ”New Application of Thermal Laser  Signal Injection Microscopy (T-LSIM)”, ISTFA, 2003, p25-35.


[12] F. Beaudoin et al, “Laser Stimulation Applied to  Dynamic IC Diagnostics”, ISTFA, 2003, p371-377.


[13] K. Baker et al, “Shmoo Plotting: The Black Art of IC  Testing”, IEEE, 1996, p932-933.


[14] K. Sanchez et al., “Phase Variation Mapping, a Dynamic  Laser Stimulation Technique with Picosecond Timing  Resolution“, IRPS, 2007, p534-541.


[15] R. Wang et al., “Threshold Voltage Variation with  Temperature in MOS Transistors”, IEEE Electron  Devices, Vol.18, Is. 6, June 1971, p386-388.


[16] J. A. Rowlette et al., “Critical Timing Analysis in  Microprocessors Using Near-IR Laser Assisted Device  Alteration (LADA)”, ITC, 2003, p264-273.


[17] J.A. Kash et al.,”Non-Invasive Backside Failure Analysis  of Integrated Circuits by Time-Dependent Light  Emission: Picosecond Imaging Circuit Analysis”, Microelectronic Failure Analysis, Desk Reference, 1999,


p505-510.


Real-Time FTIR Etch Depth Measurements in Passive Integrated Silicon  Substrates


F. Roullier, B. Domengès, P. Poirier,


LAMIPS, laboratoire de microélectronique ENSICAEN-NXP Semiconductors, CRISMAT, frederic.roullier@nxp.com   2 rue de la Girafe BP 5120, F-14079 Caen Cedex 5.


and J.P. Blanvillain


NXP Semiconductors, 2 rue de la Girafe BP 5120, F-14079 Caen Cedex .


This paper deals with real-time FTIR (Fourier Transform  Infrared Reflectometry) etch depth measurements performed  on passive integrated silicon substrates. High-density trench  capacitors are non-destructively characterized using an FTIR  Michelson type spectrometer. Based on effective medium  approximations, an effective index associated to the capacitor  layer is introduced which allows a good evaluation of the  capacitor hole depth. Obtained results correlate well with  those from SEM (Scanning Electron Microscopy) measurements performed on cross-sections, on a range going  from 12µm to 30µm depth.


NXP semiconductors has developed and implemented a  passive substrate technology [1,2] as a basis for System in  Package devices dedicated to high frequency applications. The  passive integration technology (PICS for Passive Integration  Connective Substrate) is based on the integration of passive  components in a silicon die (so-called passive die), on which  one or more active dies are flipped and connected. Passive  components are integrated, such as, resistors, inductors and  planar and high-density trench capacitors. The latter are based  on a 3-D architecture, that is a lattice of thousands of high  aspect ratio holes in highly doped silicon substrate (lower  plate of the capacitor), covered with a thin dielectric layer and  then with highly doped polysilicon (upper plate). Depth of  holes is a major parameter to control as it strongly influences  capacitance value. Till now, destructive characterization of the  depth and the shape of holes were performed through crosssections and scanning electron microscopy measurements. Not  only time but also money consuming, it appeared important to  introduce a non destructive technique of hole profile  measurements in order to improve the capability of the  process as well as ensuring the lowest possible cost. Among  non-destructive optical techniques, Fourier Transform InfraRed spectrometry appeared quite suitable for such analysis.


Indeed, it has been successfully applied to metrology issues in  high density Dynamic Random Access Memory chips [3]. Though aspect ratios of measured capacitor structures are  comparable, the measured dimensions in PICS capacitors  cannot any more be considered as small compared to infrared  wavelengths and physical interaction phenomena with infrared  beams are slightly different. Still, very promising results were  obtained with FTIR experiments, which will be presented in  the following paper.


Experimental


In order to test the ability of the technique, a first series of  measurements were performed on 62 different points of a  typical PICS wafer, which were processed in Epsilon pilot line  of NXP Semiconductors-Caen. Each measurement point  contains a 2µm pitch hole lattice on one mm² area, each hole  being characterized by a diameter of 1µm and a depth of  19µm. The equipment was a Nanometrics QS3300ME, used in  reflection mode with an unpolarized beam of a diameter of  5mm and a scan time per measurement site of 5s. In order to  test for repeatability and reproducibility, ten cycles of  measurements at the same site were performed as well as ten  cycles of loading and unloading of the wafers. A subsequent  cleavage of the wafer allowed comparative Scanning Electron  Microscopy measurements at 7 different points.


Figure 1. Optical image of wafer site measurements.


Capacitor site


A second series of experiments were then performed with our  own equipment, BIORAD 408M, on eight wafers, exhibiting a  depth of holes ranging from 12 to 30µm. Wafers were  characterized at a thirty-degree angle of incidence. The light  was generated by a Michelson interferometer (FTIR  spectrometer) with a wavelength ranging from 2.5µm to  45µm. Reference interferograms were acquired at PCM zone, free of PICS capacitors (Fig. 1). Finally, studied wafers were  cross-sectioned for comparative SEM measurements.


Review of FTIR thickness measurement  principles


Thickness measurements using FTIR spectrometers are based  on the measurement of path difference introduced by the  variation of spectral reflectance of the layer to be  characterized compared to the substrate. To differentiate and  measure it, the Michelson interferometer produces  interference signals, which contain infrared spectral  information generated after reflection from the sample (Fig. 2). A Fourier transform is employed to convert the  interferograms into intensity (or reflectance) vs wavenumber  spectra. The reflectance spectrum can then be computed by  taking the ratio of the sample beam to the reference beam and  several filtering operations will be performed. The filtered  spectrum is then Fourier analyzed to extract the fringe  frequency and therefore the layer thickness.


Figure 2. Principal scheme of Michelson interferometer.


The dimensions (width, depth and pitch) of the capacitor  structures are smaller but of the same order of magnitude as  the wavelength range and their optical properties can be  approximated using effective medium theories [3-4]. That  means that these structures are microscopically heterogeneous, but appear to be macroscopically homogeneous, and their  reflectance behavior can be approximated by a dielectric layer  with a different refractive index from that of silicon, the so  called effective index. The latter can be calculated using  several simple formulae [5-7] that take into account the  microtopology, i.e. the volume fraction of particles, here holes  to be characterized. In this case, both volume fractions (holes  and silicon matrix) are comparable and the Bruggeman  expression appears more appropriate. The combination of


holes and the silicon matrix constitute a mixture  microstructure, that is the effective medium itself. Its effective  dielectric constant (εeff) will be related to air (holes) and  silicon (matrix) dielectric constants by the formula :


eff


f


ε


, where f  and fa Si are hole  and silicon matrix volume fractions respectively.


Test measurements on 62 sites of a PICS wafer


Nanometrics application filmZ software can also display the  film thickness cartography (Fig. 3). Besides the expected  almost circular symmetry of etch depth distribution, two  aberrant points appear, which could be related to a  misalignment of the beam on the capacitor site, leading to a  very low signal. This can be explained by the difficulty to  center a 6" wafer on an 8" holder. Based on geometrical  characteristics of capacitor structures and effective medium  approximation calculations, an effective index of 3.04 [7] was  used which led to a very good correlation with SEM  measurements obtained from cross-section imaging (Fig. 4). To assess SEM measurement errors, which are usually  considered as high as ±2%, 54 and 54bis positions were  characterized, two times, with a one day interval between.


Figure 3. Etch depth (µm) cartography. Note the almost  circular symmetry and two artifact measurement points. Arrow indicates the SEM measurement point.


60 49


Comparative SEM and FTIR measurements  7 points of a wafer


18.5 19


19.5 20


58


54 54bis 53


Position


SEM FTIR


Figure4. Comparison of depth measurement results obtained  with SEM (plain line) and FTIR (dotted line) experiment.


Comparative SEM and FTIR measurements


10 15 20 25 30


7


17


Etch time (min)


SEM measurements


FTIR neff=3.04


FTIR n(Si)


Figure. 5. Comparative SEM and FTIR depth measurements. Arrowed points correspond to batch 2


c


Figure 6. SEM images of three wafers,


gher


corresponding to lower, medium and hi


values of hole depth a) 12.9µm, b) 20.3µm  and c) 29.8µm. Note the different hole


profiles, which will affect the opened volum ratio and thus optical properties.


pplication to various depths of hole


rmed on eight wafers, e depths ranging  from approximately 12 to 30µm. To test for reproducibility, a


second batch of three wafers was prepared. Results are given


in Fig. 5. Three curves are shown : one for SEM results, another for FTIR measurements based on a refractive index of


3.42 (typical of our silicon epitaxial layer) and the other for


A second set of measurements was perfo


corresponding to different etch times, thus hol


FTIR measurements corrected for neff= 3.04. Obviously, EMA (Effective Medium Approximation) theory improves the  correlation between SEM and FTIR results. One should note  that the deeper the hole the worse the underestimation of  depth by FTIR is.


To a first approximation, FTIR measurements based on EMA  eory give good estim


pth non-destructively.


Nevertheless, the hole


hould be improved, as  the calculated neff  index was evaluated for 19µm-deep holes.


TIR experiments performed on a classical FTIR Michelson


ectrometer (that is n


ed Infrared dedicated


system) have been quit


d as a non-destructive  metrology tool for PICS capacitor geometric characterization.


We wish to thank


their help


and technical assistance.


[1] F. Roozeboom, A. Kemmeren, J. Verhoeven, E. van den


[2]


l, Y. Bouttement, S. Bardy, L.


[3]


hal, C. Duran, J. Tower, A. Mazurenko, U.


[4]


. Huffman, Absorption and


[5]


hilos. Trans. R. Soc. Lond., 203


[6]


geman, Ann. Phys. 24 (1935) 636.


hnology,


th


ate of hole de


profile model s


SEM images of holes also point out the variation of hole  profile depending on the depth, though such a variation could  be expected also from one batch to the other (compare batch #1 and 2). SEM images of Fig. 6, corresponding to 12.9,


20.25 and 29.9µm hole depth, allow visualizing the hole  profile and clearly show that the opened volume ratio will be  dependant on the etching conditions, affecting the optical  properties of the layer. In an attempt to better understand the  key parameters allowing prediction of the layer  characteristics, further experiments are under progress. Using  a simple geometric model of hole profiles, we shall evaluate  as closely as possible the opened volume fraction as a first  step and then try to correlate this volume fraction to the  etching duration.


F sp


ot a Model Bas


e successfully use


It could be implemented as a on-line test, though some regular  destructive control were kept, but with a much lower  frequency, leading to a satisfactory spare of time and money. Indeed, the technique, based on EMA theory, requires a good  evaluation of the effective index parameter, i.e. the opened  volume fraction. To make it more accurate, it will be  necessary to take into account the differences on hole profile  with depth and etching duration.


P. Vargos and C. Harrison, for


We are very grateful to Prof. H. Murray for valuable  discussions.


This work was supported by "Conseil Régional de BasseNormandie".


Heuvel, H. Kretschman and T.Fric, Mat. Res. Soc. Symp. Proc. 783 (2003) 157.


D. Chevrie, C. Bune


Hamelin, E.Van Grunsven, M. Burghoorn, M. de Samber “ A Silicon based System in Package (SbSIP) Technology “ EMPC 2005, June 12-15 Brugge Belgium. [ please  check this]


P.A. Rosent


Mantz, P. Weidnerand A. Kasic, Characterization and  Metrology for ULSI Technology, AIP Conference  Proceedings, 2005, 620.


C.F. Bohren and D.R


Scattering of Light by Small Particles, John Wiley and  Sons, New York, 1983.


J.C. Maxwell Garnett, P


(1904) 385.


D.A.G. Brug


[7]  D.E. Aspnes, Thin Solid Films, 89 (1982) 249.


[8] P. Vargos and C. Harrison, Accent Opto-tec


(private communication).


Blind Deconvolution of SEM Images


William E. Vanderlinde


Laboratory for Physical Sciences, College Park, Maryland, USA


James N. Caron


Research Support Instruments, Lanham, Maryland, USA


Blind deconvolution techniques were used to enhance  scanning electron microscope (SEM) images in the range of  200,000x to 500,000x magnification. Typical SEM samples  were imaged including a gold island reference standard, a  plasma delayered integrated circuit, and an integrated circuit  cross section. Image resolution improvement up to 40% was  observed. However, it was necessary to use 16-bit TIFF  images with greater than 120:1 signal to noise ratio, which  required 10 minute frame times.


Shrinking integrated circuit feature sizes require constantly  improving metrology tools. The SEM remains a workhorse  tool for metrology but TEM and AFM are increasingly used to  image the smallest circuit features [1,2]. Thus it is desirable to  squeeze out every possible bit of resolution in the SEM for  semiconductor metrology and for analysis of nanotechnology  materials. In this paper we will discuss an image processing  technique called blind deconvolution.


As it applies to images, deconvolution is the process of  removing the blur function from an image.  Blind  deconvolution methods are used in cases where the blur  function cannot be measured or accurately modeled.  In some  cases, the application of a sharpening filter will suffice.  However, if accuracy is important, or the blur function is large  or non-symmetrical, more sophisticated methods, such as  maximum entropy or nonparametric finite support are  required.  Here we apply the self-deconvolving data  reconstruction algorithm (SeDDaRA) [3]. This approach  extracts the blur function directly from the image and uses a  conventional deconvolution method to remove it.  This is a  non-iterative method that has proven success on a large  variety of imaging systems [3,4,5].


Image Processing Methods


The blurred image g(x,y) can be described as a convolution of  the real scene f(x,y) and a blur function or point spread  function (PSF) as in


g(x,y)= f(x,y) ● d(x,y)+w(x,y)


where w(x,y) is a noise term, and  ‘●’  denotes convolution.  The objective of blind deconvolution is to find the best  estimate of f(x,y) from g(x,y) when the PSF and noise function  are unknown.  This relationship is evaluated by transferring  both sides of Eq. (1) into frequency space via a Fourier  transform, yielding


G(u,v) = F(u,v)  D(u,v)+W(u,v)


where (u,v) are the coordinates in frequency space, and the  transformed functions are represented by capital letters.


If the PSF can be measured or accurately modeled, a  deconvolution process can be applied to g(x,y) to estimate  f(x,y).  Many iterative deconvolution algorithms, such as nonnegative least squares and maximum entropy, can be found in  the literature [6,7,8,9,10]. However, several authors have  concluded that approximations to the Wiener filter [11] are  equally effective and operate faster [12,13]. Designated the  pseudo-inverse filter, the formula for deconvolution is


]


|


v)


D(u,


[|


(u,


*


v)D


G(u,


F(u,


2 +


where ‘*’ denotes the complex conjugate, and the parameter  C2 prevents the over-amplification of noise. The pseudo  inverse filter is easy to apply and provides good results when  used with SeDDaRA.


Without explicit knowledge of d(x,y), the function must be  estimated through blind deconvolution.  Research on blind  deconvolution extends back several decades, but studies by  Ayers and Dainty [14] spurred an increase in activity in the  astronomical community [15]. All methods require some prior  knowledge of either the scene, [16] the scene statistics, [17,18] or the shape of the blur function [19]. Most of these  techniques are iterative and can only be applied within certain  constraints.  In contrast, the SeDDaRA approach is noniterative and can be applied to a large variety of imaging  techniques and PSF types [3].


With SeDDaRA, the PSF in frequency space is assumed to  have the form


D(u,v)= [ KG  {|G(u,v)-W(u,v)|}]α(u,v)


(4)


where  α(u,v)  is a tuning parameter and KG is a real, positive  scalar.  Application of the smoothing filter {...} assumes that  D(u,v) is a slowly varying function.  Further assumptions for  this calculation are explained in a published paper [3]. After  some derivation, α(u,v) is found to be


|]


W(u,


| S


Ln[K


|}]


F'


S{|


Ln[K -


G


≈


(5)


where F'(u,v) is a reference image, provided by the user, that  satisfies


KF'  {| F'(u,v)|} ≈ K_F  {|F(u,v)|}.


The presence of a smoothing filter greatly relaxes this  condition. In Eq. (5), KG and KF’ must be determined such that  |D(u,v)|< 1. This condition is satisfied if we set KG = 1/Max[  {|G(u,v)|}]  and  KF' = 1/Max[  {|F'(u,v)|}].


The function  |F'(u,v)|  is the key to the success of the process.  It is a representation of spatial frequencies that one expects to  achieve.  With the presence of the smoothing filter, this  function need only to be similar to the spectrum of the actual  truth image |F(u,v)|.


Once D(u,v) has been estimated from Equation 4, F(u,v) is  calculated from Equation 3. An inverse FFT is applied to  F(u,v) to produce the improved image.


Images were acquired using a LEO 1550 FE Schottky field  emission scanning electron microscope at 10 or 20 keV  electron beam energy. A 30 micron aperture was used as it  typically provides the best compromise between beam current  and spot size for high resolution imaging. The beam current  was not measured. Images were acquired using “noise average – line average” mode with N=30 and scan speed settings as  high as “9” for 10.1 minute image acquisition times.


Typically SEM users will record images as 8-bit TIFF or  JPEG files using a slow scan of between 10 to 60 seconds per  frame. However, it was found that blind deconvolution was  not effective with these types of images. In order to achieve  improved resolution by blind deconvolution, two significant  modifications were required in how the images were captured  and stored.  First, the captured images were saved as 16-bit, as  opposed to 8-bit, TIFF images. Computer screens typically  show only 8-bits of gray scale, but the deconvolution results  were greatly improved when 16-bits of information were


preserved.  Once a SEM image is acquired, saving it as a 16-bit TIFF file does not present any particular problem except  for requiring somewhat larger file space.


The second change was to increase the signal-to-noise of the  images.  A typical 20 second SEM slow scan has about 20:1  signal to noise which is not adequate for the blind  deconvolution algorithm.  A much longer acquisition time of  10 minutes was found to provide an appropriate signal to  noise ratio of 120:1. SEMs can easily be used to take very  long image acquisitions as long as the beam and sample stage  are stable against drift, and the sample is resistant to damage.  An alternate way to increase the signal-to-noise would be to  increase the beam current, however that would degrade the  image resolution.


Both the 16-bit TIFF storage and the increased frame time act  to preserve the system blur function information in the image, making it possible for the blind deconvolution algorithm to  improve the image quality.


The following samples were selected for analysis: (1) an SEM  resolution standard consisting of gold islands on a carbon  substrate (500,000x magnification, 20 keV), (2) a plasma  delayered integrated circuit with gold sputter coating (200,000x magnification, 10 keV), and an integrated circuit  mechanical cross section with gold sputter coating (200,000x  magnification, 10 keV). Images of these samples, before and  after blind deconvolution, are seen in Figs. 1 through 6.


Fig. 1 shows a standard SEM resolution standard that consists  of gold islands on a carbon substrate. The magnification is  quite high, 500,000x. A further 2x magnification of part of  Fig. 1 is shown in Fig. 2. The acquisition time was 10  minutes. The gold-on-carbon sample image clearly benefits  from the blind deconvolution processing. The increase in fine  detail is visually discernable, and there do not appear to be  any artifacts typically produced by “sharpening” routines.


This image was used to assess the improvement in resolution.  The full-width half-maximum (FWHM) was measured for ten  random peaks in the unprocessed and processed images. The  average peak before processing had a width of 18.3 pixels, whereas the same peaks after processing had a width of 14.9  pixels.  The ratio of the improvement in FWHM over the  original FWHM provides a measure of improvement in the  resolution.  The average improvement in this image was  calculated to be 19.8% whereas the maximum improvement  found was 41%.


Fig. 3 shows the grain pattern of a heavily gold sputter-coated  aluminum line on a silicon chip. The magnification is  200,000x. Again, the acquisition time was 10 minutes. A  further 2x magnification of part of Fig. 3 is shown in Fig. 4. The resolution improvement is also noticeable, but there are  some slight artifacts such as the “ringing” that occurred at the  margins of the image. The very long acquisition time resulted  in the edges of the image being quite dark. The image  darkening was apparently due to carbon deposition since it did


50 nm


Figure 1a: SEM of a gold-on-carbon resolution standard, 500,000x magnification.


Figure 1b: Same image as Fig. 1a following application of  blind deconvolution.


not go away when the sample was vented to air as would be  expected if caused by charging effects.


Fig. 5 shows an integrated circuit mechanical cross-section  with a light sputter coating, again at 200,000x magnification. This sample was apparently cleaner as there was no darkening  from carbon deposition. Fig. 6 is a 3x close-up of the central  region of Fig. 5, showing improvement in fine details such as  a thin filament which is not visible in the unprocessed image. A line plot of image intensity vs. pixel number for the left side  of Fig. 1 before and after deconvolution is shown in Fig. 7.


Figure 2a: 2x magnified area of Fig. 1a (effective  magnification is 1,000,000x) before image processing.


Figure 2b: 2x magnified area of Fig. 1b (effective  magnification is 1,000,000) after image processing.


Figure 3a: SEM of gold sputter coating on aluminum metal  line, 200,000x magnification.


Figure 3b: Same image as Fig. 3a following application of  blind deconvolution.


We have found that blind deconvolution can improve the  resolution of an SEM image by up to 41%. The major  limitation to this technique is the very long image acquisition  time (as long as 10 minutes) required to obtain the necessary  signal to noise ratio. Since this technique would be primarily  valuable for images near the resolution limit, it is likely to be  used at very high magnification, i.e. 200,000x or above. At  that magnification, image drift of greater than 1 nm per minute  is liable to cause significant distortion to the image. Therefore, the stage and beam must be stable against drift to better than 1  nm per minute. The sample must also be sufficiently clean and  robust that 10-minute exposures do not cause charging, carbon  deposition, or beam damage. Beam sensitive materials such as  low-k dieletrics are probably not suitable subjects for this  technique. The long acquisition time also makes it unsuitable  for routine metrology measurements that require very rapid  throughput.


[11]. The correlation found is quite good (R2 = 0.89). This is  shown in Fig. 9. It means that targeting with CD-SEM (shown  in purple) at 50 nm will result in different offsets with STEM (shown in blue). Solutions for this CD-SEM issue are  currently under investigation [7].


y = 2.3463x - 193.65 R2 = 0.8918


0 2 4 6 8 10 12 14


84


85


86


87


88


SWA (degrees)


0 10 20 30 40 50 60


Offset


BCD CD-SEM


Figure 9: Graph showing the Side Wall Angle (SWA)


dependant offset between CD-SEM and STEM Bottom CD (BCD). 1Offset = BCDCD-SEM  – BCDSTEM


The uncertainty in the measurement result depends not only  on the precision of the Metrology tool, but also on other  effects such as sample-metrology tool interaction. For  example, photo resist has a certain Line Width Roughness  which leads to a measurement noise for the line width when  applying local measurement techniques (e.g. STEM). When  the average BCD value of multiple lines in a STEM sample is  calculated, the uncertainty of the measurement becomes


better. More information can be found in [5] and [12]. Tools  for Optical Critical Dimension (OCD) measurements or CDSEM’s (with extended measurement box) sample over a larger  area therefore reducing the uncertainty of the measurement.


The isofocal energy is the exposure dose where the BCD does  not change when focus is changed on the scanner. We used  four metrology techniques to measure the BCD value of resist  lines at this isofocal point on the same wafer at the same  location. The results are shown in Table 2.


As expected, Metrology techniques using a large sample area, like OCD, have a lower variation in BCD values than the local  techniques CD-SEM or FIB/SEM. The FIB/SEM result is  achieved after taking an average of 45 lines. The uncertainty  of the STEM is better than FIB/SEM cross-section  measurement, because the measurement result is an average of  a 100 nm thick sample. More information about the  importance of sampling on uncertainty will be published in


[13], [14]


The averaged BCD values between CD-SEM and FIB/SEM  differ by 10 nm. Between OCD and STEM this difference is  only 4 nm. This is a good indication that beam-sample  interaction during STEM metrology of photo resist is not  shrinking the resist. In fig. 10 the bottom CD values as  measured with 4 different Metrology tools are shown.


Table 2: Variation on isofocal (3σ) for four Metrology  techniques


Average Isofocal (nm)


Variation on isofocal (nm, 3σ)


OCD


47


STEM 51


2.2


FIB/SEM 55


6.2


CD-SEM 65


1.9


55


Defocus (nm)


FIB/SEM OCD CD-SEM STEM


Figure 10: Bottom CD Values measured on four Metrology  tools (65 nm dense lines)


Process control on gate level


For routine metrology after poly gate etch processes, top down  CD-SEM is used to monitor gate width uniformity across the  wafer. This data can be fed into an APC application in order  to optimize yield. Cross-section metrology is required if more  detailed information is needed, e.g. poly gate profile, poly  gate footing, and/or bottom and top CD measurements. This is  recommended for tool qualifications after preventive  maintenance or tool clean procedures. In the past, cross  section SEM was routinely applied for that, but with the  introduction of the 45 nm node, the SEM technique is  reaching its limits. Hence TEM has been chosen to substitute  for SEM because of the higher spatial resolution and  consequently the higher information content.


To ensure a fast turn around time for the TEM analysis, the  following preparation and analysis procedure was applied (see  the preceding Lithography Metrology section). First, the  location of interest, a dedicated scribe line test structure for  metrology that resides in a regular pattern on the wafer, was  defined. Fig. 10 shows a wafer map where 15 locations were  chosen for TEM cross section metrology. The subsequent  automated TEM sample preparation had a success rate of  83%, including the manual lift out.


Table 3: Side Wall Angle of 20 locations across the wafer


Figure 10: a) Wafer map with 15 locations for TEM sample


preparation b) FIB pattern recognition image for the


automated fine milling of the TEM lamella


The TEM images in Fig. 11 show an overview in a) containing the cross section of 5 dense poly gate lines and b) the center line. Details about poly gate profile, capping layer, or footing can be assessed from these cross sections. Figure 11  c) shows the gate oxide at atomic resolution.


Figure 11: TEM image of a fully automated prepared TEM  lamella a) overview b) center poly gate c) HR-STEM of gate  oxide


The image in Fig. 12 was used for the automated IC3D  measurements. The challenge was the undefined contrast  interface between poly silicon and the silicon oxide. Nevertheless, the SWA of 20 locations of the two horizontal  lines across the wafer shows a very high process stability for  the poly gate etch as shown in Table 3.


Figure 12: IC3D screen dump showing bottom CD, top CD  and gate height


To asses the quality of the automatically prepared TEM  lamella with respect to side wall amorphization, orthogonality, etc., a FIB lift out sample was manually prepared. The FIB  procedure is illustrated in an image sequence in Fig. 13.


1. Area of interest before preparation


2. Pt-deposition and first half rough milling with the  highest ion beam current - a ‘stairs’ contour is milled  into the sample


3. Second half rough milling


(X, Y) coordinate [mm]


SWA3 [°]


SWA4 [°]


(-65.43, 0.088)


88.44


88.43


(-20.57, 0.088)


(24.29, 0.088)


(1.88, 0.088)


(46.73, 0.088)


(91.60,0.088)


91.57


(0.088, -43.69)


(0.088, 1.07)


(0.088, 23.49)


(0.088, 68.37)


4. Top down Image


5. Milling a “U” shape to separate bottom and sidewalls  from the bulk at 7° stage tilt and final thinning of  TEM lamella only on very small length of 5µm


6. Final Cut with the low ion beam current (e.g. 50pA) to cut the lamella loose.


The electron transparent part of the sample is restricted to a  very small length of about 5 µm only. The bulk of the sample  provides good stability during the lift out extraction with the  glass needle.


Figure 13: Manual FIB preparation of lift out sample


Comparing both preparation flows, automated (Fig. 11) and  manual (Fig. 14), it can be stated that no significant difference  in the achieved quality if the TEM lamella was found.


Figure 14: TEM image of manual FIB preparation


Discussion and Future Improvements


In order to assess the productivity of the process flow  presented, the numbers of TEM samples generated in one  week were counted for different applications. To set up a new  process flow, a programming time of about 40 hours must be  spent. In the case of photoresist metrology, using the  automated equipment 24/7 for the rest of the week results in  68 TEM samples per week. Once the process flows exist, programming time can be reduced to two hours. Productivity  will them be 83 TEM samples per week. In the application for  etched poly gate structures, there is higher productivity  because platinum deposition takes less time. Productivity rises  to 91 samples per week when setting up the new process and  reaches 111 samples per week for repeating the process.


In order to become efficient in Semiconductor Metrology, the  turnaround time of TEM Metrology needs to be further  improved. In general there are five ways to reach that goal:


1. FIB Hardware improvements: Shorter milling times  need more intense ion beams. TEM preparation time  can be reduced using more advanced FIB columns.


2. New protective coating techniques: Regardless of  whether the deposition was assisted electron- or ion  beam, the deposition time has to be reduced. One  hour protective layer deposition to protect the resist  from shrinking, as described above, has to be reduced  significantly.


3. Process flow optimization: There is still the tendency  to do TEM sample preparation in a sequential  process, which can be understood because time to  data is an important parameter. The different flow  charts shown in fig. 1 clearly indicate the possibility  to use so called “pipe-line mode.” Separated stages of  the preparation process are carried out  simultaneously on different tools. For example, bulk  sample preparation is separated from final thinning. Reference [4] gives a good example of such a process  flow.


4. Full Automation: Improved automation of the  process in order to have less operator assistance.


5. Inline equipment use and automated sample  handling: when TEM Metrology has to be used in the  APC system, a turnaround time of less than five  hours is needed or the manufacturing flow will be  interrupted. Therefore, the sample preparation  equipment needs to be placed in the clean room, wafers must go back into the manufacturing line after  TEM sample extraction, and the TEM samples need  to be handled in an automated way.


Preparing TEM samples on multiple wafers in a batch is  possible in an automated way using a Dual Column FIB/SEM  system. The overall yield, including ex-situ lift-out, is more  then 90%. It is a challenge to make sure that the process is  stable over a long period of time (months). Hardware  improvements of Dual Column systems are needed, and on  their way, to improve turn around time even further. These  include optical wafer alignment and improved FIB resolution  at high beam current. There is no significant difference in the  quality of automated TEM samples compared to manually  prepared samples from a gate process control application. Cross-section metrology using TEM is anticipated to be  routinely used at the 45 nm node and beyond. The main  challenge is to get turnaround time below 5 hours. At the  moment this turnaround time is three days of running fully  automated sample preparation and platinum deposition at  night, and manual ex-situ liftout and TEM imaging during the  day. This turnaround time is for a full batch of wafers, which  means that within three days a process optimization based on  TEM data can be performed.  When variation on the isofocal


is used as a measure for Measurement Uncertainty, it is found  that uncertainty for STEM Metrology is comparable with CDSEM Metrology. This is achieved after taking the average of  45 photoresist profiles. Uncertainty for FIB/SEM Metrology is  worse than STEM Metrology, when the same amount of  profiles are used, because STEM Metrology uses an integrated  signal over a 100 nm thick sample; this reduces measurement  noise.


The authors would like to thank the following people for their  contributions to this work: Jeroen de Vries and Jurriaan van  Schaik  (ASML) for the many hours spent in programming the  Automated TEM sample preparation recipe and processing of  the TEM samples. Jeroen Meessen (ASML) for providing  CD-SEM data. Sarah Stoops for editing the manuscript.


[1]  Physical failure analysis in semiconductor industry - challenges to microscopy, E. Zschech, E. Langer, M. Meyer, M, H. Engelmann, H. Stegmann, H. Geisler, B. Tracy, G. Schneider, Techn. Proc. of the 6th Int. Conf. on Modeling and Simulation of Microsystems (MSM 2003)


[2] 3D observation of elemental distribution of Si-device  using a dedicated FIB/STEM system, T. Yaguchi, M. Konno, T. Kamino, M. Ogasawara, K. Kaji, T.


Onishi, ISFTA proceedings (2005)


[3] Transmission Electron Microscopy at SEM voltages, Bryan Tracy, Kirstin Alberi, Spansion,


http://www.sela.com/Presszone/Workshops/SELAHITACHI-2004/Spansion.pdf


[4] In-Line TEM Sample Preparation and Wafer Return  Strategy for Rapid Yield Learning, N. Bicais et al.,


ST, FEI, Philips Semiconductors, Proc. SPIE 6152, 615217 (2006)


[5] Total Test Repeatability, a new figure of merit of CD  metrology tools, H. Cramer et al, SPIE 2004


[6] ArF photo resist pattern sample preparation method  using FIB without protective coating, H. Okushima, T. Onozuka, Y. Kuroda, T. Yaguchi, K. Umemura,


R. Tamochi, K. Watanabe, I. Kawata, B. Rijpers,


Proc. SPIE 6152, 615244 (2006)


[7] Estimation of pattern shape based on CD-SEM image  by using MPPC method, T. Onozuka, Y. Ojima, J.


Meessen, B. Rijpers, Proc. SPIE 6152, 61521D


(2006)


[8] Automated High-quality TEM sample preparation, Y. Yamamoto, T. Ashata, et al., SII Nanotechnology,


Microsc Micoanal 12 (supp 2), 2006


[9]  International Roadmap For Semiconductors, table


adapted based on http://www.itrs.net/Links/2006


Update/2006UpdateFinal.htm and


http://www.itrs.net/Links/2004Update/


2004Update.htm


[10] A comparison of focused ion beam and electron


beam deposition processes, Lipp et al.,


Microelectron. Reliab., Vol. 36, No. 11/12, pp. 1779-1782, 1996


[11] CD-SEM based Critical Shape Metrology of


Integrated Circuits, D. Gorelikov, J. Remillard, N.


Sullivan, Proc. SPIE, 5375 (2004), pp. 605-613


[12] TEM Calibration Methods for Critical Dimension


Standards, G. Orji, R. Dixson, D. Garcia-Gutierrez, B. Bunday, M. Bishop, M. Cresswell, R. Allen, J.


Allgair, Proc. SPIE 6518, 651810 (2007)


[13] Impact of Sampling on Uncertainty: Semiconductor  Dimensional Metrology Applications, B. Bunday, B. Rijpers, B. Banke, C. Archie, I. Peterson, V.


Ukraintsev, A. Vladar, T. Hingst, M. Asano, to be


published


[14] The International Technology Roadmap for


Semiconductors (ITRS), 2007 Edition, Metrology


Section, to be published


Applications of Electron Tomography on Advanced DRAM


Jian-Shing Luo, Jeremy D. Russell, Lang-Yu Huang, and Tsang-Pei Chen


Physical Failure Analysis Department, Inotera Memories, Inc. Taoyuan, Taiwan, Republic of China


The rapid advances in nanotechnology and the decreasing size  of features in the microelectronics industry result in the need  for advanced characterization with high spatial resolution in  two and three dimensions (3D). Therefore, the demands for  physical failure and materials analysis using the transmission  electron microscope (TEM) or scanning transmission electron  microscope (STEM) are rapidly increasing, for instance  thickness measurement, small defect identification, chemical  element analysis, etc. However, some artifacts, such as  amorphous layers and overlapping interfaces in small vias, will  become more serious as the dimensions of the TEM sample  become larger relative to the ever-shrinking device dimensions


[1]. This makes accurate measurements and structure analysis  difficult. One solution is electron tomography as a way to  reconstruct a 3D object from a series of two-dimensional (2D) projections. Electron tomography offers an intermediate  resolution (of about 1 nm) with a field of view of hundreds of  nm making it ideal for the characterization of many nano-scale  devices [2]. Previously [3-5], several applications were  reported evaluating the capabilities and limitations of bright  field (BF) TEM and high angle annular dark field (HAADF) STEM tomography for 3D structural characterization in  materials science. It is well known that pursuing the  miniaturization of devices to lower the cost and increase highspeed performance are extremely important goals for dynamic  random access memory (DRAM). Therefore, electron  tomography has a high potential for application to new  generation DRAMs.


In the case of tungsten (W) via technologies, chemical vapor  deposition (CVD) W on physical vapor deposited (PVD) Ti/TiN is a common structure for the first level metal  interconnect in DRAM devices. CVD W has excellent step  coverage in high aspect ratio contacts. TiN serves as the  diffusion barrier to avoid fluorine (F) attacking underlying Si  at the bottom of the contact during W deposition. Ti reduces  the contact resistance by formation of TiSix with Si. TiN  barrier failure can lead to worm holes or the volcano effect [6, 7]. Therefore, the step coverage of Ti/TiN barrier layers is very  important to the electrical performance of W vias, which  require a good barrier for adhesion to SiO2 and to protect the Si  substrate from encroachment. From previous research [8], the  3D simulation method was used to predict the step coverage of  the barrier for investigation of different process conditions. However, it is still necessary to calibrate the model parameters


parameters with experimental data. In this paper, we report  several real-case examples of electron tomography on 90 nm  technology DRAM, including barrier layer step coverage, via  fill process observations and defect analysis.


The TEM cross sectional samples were prepared by the  focused ion beam (FIB), then lifted out and landed on a carbon  film with/without pre-absorbed Au beads. The lift-out  procedure is described in detail elsewhere [9-10]. The  thickness of TEM lamellae ranged from 100 nm to 200 nm.


Electron Tomography


Electron tomography data sets were acquired on an FEI Tecnai  F20 field emission TEM with STEM system using the  XPlore3D tomography suite. For BF-TEM tomography, no  objective aperture was used to minimize the influence of  diffraction effects [4]. For STEM tomography, a small camera  length of 70 mm was used to minimize efficiently diffraction  effects for the HAADF-STEM signal collection. Scanned  images with 1024x1024 pixels were acquired using a frame  time of 15-30 sec. Typically 1-200 (S)TEM images with  1024x1024 pixels were acquired automatically over a tilt-range  of more than +/-60° in 1 degree steps. After acquisition, tiltseries alignments were performed to refine the relative image  shifts and tilt-axis orientation using Inspect3D software. The  3D volume was reconstructed using the simultaneous iterative  reconstruction technique (SIRT) in Ispect3D software. The  result was visualized by volume rendering using Amira  software [3, 4].


(I) Barrier layer step coverage


In general, the step coverage of the barrier layer is evaluated  by using TEM or SEM for advanced DRAM. However, the  details of the barrier in high-aspect ratio vias are becoming  increasingly difficult to image using traditional SEM or TEM  2D images, due to the reduction of critical dimensions and the  resulting significant barrier layer curvature in the samples. One  example is shown in Fig. 1. Using thinner specimens is the  traditional way to improve the situation, but in this case it is  necessary to overcome the high proportion of amorphous


Figure 1: BF-TEM image shows overlapping barrier layer on  via’s sidewall and severe amorphous phenomenon in Si  substrate.


layer and bending phenomena in the samples. Electron  tomography is an alternative method to determine the quality  of the barrier layer in a W via [11].


BF-TEM tomography has a diffraction effect problem, which  limits the application on semiconductor devices [4]. However, BF-TEM tomography can be used to characterize the structure  of semiconductor devices with amorphous or weakly scattering  crystalline materials, such as seed and diffusion barrier layers  in un-filled metal vias. Fig. 2 (a) shows a BF-TEM image of  the TiN barrier layer in an unfilled W via, while Fig. 2(b) shows a full 3D reconstruction in which all the morphology of  the barrier layer is visible. However, by using x-y orthogonal  slices through the 3D reconstruction volume, the step coverage  can be more easily investigated, as shown in Figs. 2(c,d). Although diffraction contrast artifacts exist between the  strongly scattering WSix and barrier layer, as shown in Fig  2(b), poor step coverage can be easily observed at the bottom  corner of the barrier layer, as shown in Fig. 2(d). This  information is not visible in the BF-TEM image (Fig. 2(a)).


Figure 2: (a) BF-TEM image and (b) 3D tomography reconstruction rendering volume of a via barrier layer; (c) (d) series of  x-y orthogonal slices show the barrier layer’s step coverage across the via. Poor step coverage was found at the bottom corner  of the barrier layer, as indicated by the arrows in (d), which is not apparent in the BF-TEM image (a).


(c)


(d)


(II) Defect analysis


For defect analysis, Figs. 3(a-c) show an example of several  BF-TEM images of the array structure in a DRAM. A defect  was found beside a “contact to bit line” (CB) via’s bottom at  the failure address, as indicated by the arrow in Fig. 3(c). Furthermore, the defect was identified as W by compositional  analysis. From electrical test, the failure address had a leakage  problem from the CB to the p-well. This finding matches the  failure mechanism of leakage through the source/drain junction  to the p-well caused by the W inclusion. According to previous  studies [8, 9], the W residue can be formed during CVD W via  fill, if WF6 leaks to the active area (AA) through a weak  Ti/TiN barrier layer. The leakage path visualization is an  enabling factor for subsequent process improvement. However, it is difficult to provide detailed information to clarify the exact  position of the weak barrier and the leakage path in this  abnormal CB from a normal 2D BF-TEM image, as shown in  Fig. 3. In contrast, a 3D image can provide more details on the  relative relationship and feature shape. As mentioned earlier, BF-TEM tomography has diffraction effects, which result in  artifact formation and poor resolution in the BF-TEM  tomogram for strong scattering crystalline materials, such as  W. Therefore, to reduce the diffraction contribution in the  images and thereby obtain a high quality 3D reconstruction  volume, HAADF-STEM tomography was used to perform this  analysis. Fig. 4 shows the 3D HAADF STEM reconstruction  result on the same sample as Fig. 3. It is obvious that the W  inclusion is localized near the CB corner, as shown in Fig. 4 (b), and the 3D reconstruction volume also shows the CB 3D  profile and points to the weak barrier layer position indirectly,which provides more information to process and integration  engineers, for root cause clarification and process  improvement. The second example is shown in Fig. 5. Fig. 5(a) shows an abnormal via and bridge-like residue, as indicated by  the arrow, between the abnormal CB via and the transistor  gate. From electrical test and voltage contrast results, the  defect is believed to be an electrical short. In addition, it is  reasonable to conclude that the shape of the abnormal CB  resulted in poor step coverage of the barrier layer and is  therefore related to the uncompleted W via fill. Therefore, a  possible hypothesis for the mechanism of residue formation is  similar to the previous example, a worm hole was generated  from an abnormal via through a weak barrier layer to the gate, then W filled in the worm hole during the CVD W fill process. In this case, the root cause should be a photo lithography  problem, which caused an abnormal via shape and caused bad  barrier layer step coverage and poor W via fill quality. This is  consistent with the observation that such defects only occur in  certain regions where microloading in a known issue for  lithography. The 3D reconstruction rendering volume not only  shows the exact position of the worm hole but also the 3D  shape of the abnormal via, which provides more information to  improve the photo lithography process, as shown in Figs. 5 (b) and (c).


Figure 3: (a) BF-TEM image showing a defect beside the W  CB via of failure address (b) Magnified BF-TEM image in (a), and (c) Tilted XTEM image of (b).


Pt protection layer


Figure 4: (a) 3D HAADF-STEM reconstruction rendering  volume of the sample shown in Fig. 3(b). (b) rotated 3D  reconstruction rendering volume of (a), showing 3D CB  profile, weak barrier, as indicated by arrow, and W inclusion’s  position, which provide complete information for root cause  clarification.


(III) Via fill quality


The fill quality of a high aspect ratio W via influences the  device electrical characteristics. A standard (2D) scanning  electron microscope (SEM) cross-section is the routine way to  visualize the fill quality, as shown in Fig. 6. However, some  details of the void are hidden by the exact void shape and the  plane of the cross-section. By standard TEM, the situation is  worse, due to image overlap. Nevertheless, by using HAADF  STEM, and a 3D reconstruction rendering volume, the full  details of the void structure are visible, in this case represented  by x-y orthogonal slices through the 3D reconstruction  rendering volume of the via, as shown in Fig. 7. Comparing  with SEM 2D information, the 3D reconstruction more  accurately clarifies the quality of the whole W via fill process, which can be a critical contributor to the subsequent electrical  characteristics of the device.


Figure 5: (a) BF-TEM image showing an abnormal CB and  residue, as indicated by red arrow (b,c) different angle views  of 3D tomography reconstruction volume of (a), which show  the overall abnormal CB profile to aid  process improvement.


(b) (a)


Figure 6: A SEM cross section image shows a large seam in a  W via, but some shape-details are hidden.


Several cases were demonstrated to show the applications of  BF-TEM and HADDF-STEM tomography to analyze barrier  layer step coverage, defects, and W fill quality in advanced  DRAM. By appropriate use of BF-TEM or HAADF STEM  tomography optimal information for failure analysis, root cause  clarification and subsequent process improvements can be  obtained. Electron tomography holds significant advantages in  comparison to traditional TEM imaging for


cases.


The authors would like to thank all their colleagues in Inotera  Memories Inc. for their help in this work, particularly the  failure analysis I & II sections in the physical failure analysis  department. The authors are grateful to Charles Lin and Sofy  Tseng for their support on sample preparation.


[1] Mardinly, A.J. “Electron Tomography and TreeDimensional Aspects of Transmission Electron


Microscopy,” Electronic Device Failure Analysis, Vol. 7,


No.3, (2005) pp. 6-12.


[2] Midgley, P.A., Weyland, M., “3D Electron Microscopy in


the Physical Science: the Development of Z-contrast and


EFTEM Tomography,” Ultramicroscopy 96, (2003), pp.


413-431.


[3] Kubel, C., Kubel, J., Kujawa, S., Luo, J.S., Lo, H.M.,


Russell, J.D., “Application of Electron Tomography for


Semiconductor Device Analysis,” Eighth International


Workshop on Stress-Induced Phenomena in Metallization,


AIP Conference Proceedings, Vol. 817, (2006), pp. 223-


228.


[4] Kubel, C., Voigt, A., Schoenmakers, R., Otten, M., Su, D.,


Lee, T.C., Carlsson, A., Bradley, J., “Recent Advances in


Electron Tomography: TEM and HAADF-STEM


Tomography for Materials Science and Semiconductor


Figure 7: Partial series of x-y orthogonal slices of 3D  reconstruction rendering volume show the seams’ shape  changing across a W via.


(b)(a)


Applications,” Microsc. Microanal. Vol. 11, (2005), pp.


378-400.


[5] Kimura, K., Hata, S., Matsumura, S., Horiuchi, T., “DarkField Transmission Electron Microscopy for a Tilt Series of


Ordering Alloys: Toward Electron Tomography,” Journal


of Electron Microscopy, Vol. 54, No. 4, (2005), pp. 373-


377.


[ ] Stacy, W.T. et al, “Interfacial Structure of Tungsten Layers


Formed by Selective Low Pressure Chemical Vapor


Deposition,” J. Eelectrochem. Soc. 132, (1985), pp. 444-


448.


[ ] Lu, S., Chen, E., Huang, L.Y., Luo, J.S., Russell, J.D.,


“Applications of Transmission Electron Microscopy and


Secondary Ion Mass Spectrometry on Crystal Defect


Analysis and Electronic Characterisation of Advanced


512Mb DRAM,” Proceedings of the 32rd International


Symposium for Testing and Failure Analysis, Session 9:


Poster, (2006) pp. 196-201.


[ ] Bar, E., Lorenz, J., Ryssel, H., “3D Simulation of Sputter


Deposition of Titanium Layers in Contact Holes with High


Aspect Ratios,” Materials for Advanced Metallization,


European Workshop, (1997),  pp. 131-133.


[ ] Bicais-Lepinay, N., Andre, F., Pantel, R., Jullian, S.,


Margain, A., Kwakman, L.F.T., “Lift-Out Techniques


Coupled with Advanced TEM Charaterization Methods for


Electrical Failure Analysis,” Microelectronics Reliability,


Vol. 42, No. 9, (2002), pp. 1747-1752.


[ ] Young, R.J. et al, “In-Situ Sample Preparation and HighResolution SEM-STEM Analysis,” 30th International


Symposium for Testing and Failure Analysis, Session 16:


Sample Preparation 1, (2004).


[11] Stegmann, H., Zschech, E., “Electron Tomography of


Semiconductor Copper Interconnect Structures,” G.I.T.


Imaging & Microscopy, Vol. 4, (2002), PP. 8-9.


Al Pad Corrosion Mechanism Study when Dicing Saw


Shuqing Duan*, Ming Li, Qinqin Yu, Jie Su, Sanpen Lin, Chorng Niou, W.T.Kary Chien


Analytical Laboratory, Semiconductor Manufacturing International (Shanghai) Corp. 18 Zhangjiang Road, PuDong New Area, Shanghai, China 201203


*E-mail: Ivy_duan@smics.com


Two experiments were done to clarify the mechanism of mold  filler-induced PMD defect. The first experiment investigated the  effect of adhesive profile. Two experimental legs were run by  simulating a two-die stack configuration to simplify the  experiment. The dimensions of the dice and the film type  adhesive used in the experiment were shown in Table 1 and  Figure 6. The inter-die peripheral gap was present in Leg 1 and  absent in Leg 2. After unit assembly, the samples were tested. Leg 1 exhibited PMD-related electrical failure while Leg 2 did  not. The characteristic radial cracking of the passivation layer  was duplicated.


Figure 6:  Schematics of the two-die stack configuration used in  the experiment.


Figure 7: Optical micrograph showing the cross-section of the  die stack and the large mold filler trapped at the inter-die  peripheral gap (just before the edge of the inter-die adhesive). Table 1. Dimensions of the dice and adhesives used in the  experiment. Die1 is the bottom die while Die2 is the top die. Adhesive1 is the adhesive below Die1 while Adhesive2 is the  inter-die adhesive.


LEG1


Width (mm)


Length (mm)


Thickness


(mm)


Remarks


Adhesive1 8.20 (Y1) 10.60 (X1) 0.025 Die1


8.20 (Y1) 10.60 (X1) 0.075 Adhesive2 8.00 (Y3) 5.20 (X3)


0.025


Die2


8.60 (Y2) 5.40 (X2)


0.075


LEG2


8.20 (Y1) 10.60 (X1) 0.075 Adhesive2 8.20 (Y3) 5.40 (X3)


Size of adhesive2 is equal to the  intersection area between die1  and die2. Inter-die peripheral gap  is absent.


Size of adhesive2 is smaller than


the intersection area between


die1 and die2. Inter-die peripheral  gap is present.


Moreover, the second experiment investigated the mechanism of  mold filler entrapment using moire interferometry technique. The entrapment of large-sized mold fillers is likely to occur if  the separation distance between the top and bottom dice at the  inter-die peripheral gap region becomes larger during unit  processing at assembly. It was thought that it can happen if the  cantilever structure manifested by the top die exhibited “smiley” warpage. To validate the above hypothesis, an experiment was  conducted in which the samples were unmolded. The adhesive  and die dimensions of the unmolded samples were similar to  those samples used in Leg 1 of the first experiment. The die  stack setup provided a bottom die larger than the top die, and an  inter-die adhesive layer smaller than the top die in one  dimension. The stacked dice were mounted on a substrate strip  material that is similar to the substrate material used in the


actual failing samples. The overall die stacking configuration  simulated the actual die stack present in the actual failing units. Using moire interferometry technique, the warpage profile of  the top die was studied over a range of temperature by which the  unmolded dice may experience through the different processes  at assembly. This tempertaure range included room temperature  to molding temperature. Reflow temperature was excluded. The  warpage of the top die was taken by mapping the displacement  of the die surface with respect to the center of top die. The die  stack configuration in the sample ensured that the bottom die is  large enough to prevent significant addition of warpage  attributed to the bottom die. At room temperaure, the top die  exhibited a small degree of “frowning” warpage, a negative  value shown in Figure 8. As the temperature increases, the “frowning” warpage transitions to a “smiley” warpage (see  Figures 8 and 9). At molding temperature, the smiley warpage  of top die amounted to about 25 microns which is equivalent to  the thickness of inter-die adhesive.


Figure 8: Magnitude and direction of top die warpage  manifested by the unmolded two-die stacking sample over a  range of temperature.


Figure 9: Moire plot showing the “smiley” warpage of top die  at molding temperature.


Discussion of Results


In the second experiment, the mechanism that leads to the  entrapment of the mold fillers at the inter-die peripheral gap was  confirmed. The cantilever region of the top die exhibits evident  transition in warpage signature from “frowning” to “smiley” type as the temperature increases. This transition rooted from  the thermo-mechanical interaction between the silicon die and  the adhesive material. The silicon dice in the experiment were “paper-thin” which make them susceptible to warpage even at


low level of stress. The difference in the coefficient of thermal  expansion between the silicon die and the adhesive material  resulted to “smiley” warpage of top die and subsequent  enlargement of separation distance between the stacked dice in  the overhang region at elevated temperature like molding  temperature (see Figure 10). As the separation distance  increases, the maximum diameter of mold fillers that can be  trapped also increases. Hence, in the cross-section of failing  samples, the diameter of mold fillers trapped at the overhang  region was larger when compared to the designed adhesive  thickness. Upon solidification after molding process, the  molding compound exhibits shrinkage as it cools down to room  temperature. The shrinkage of molded package during cooldown provides the compaction of the trapped mold fillers. The  compaction through the mold filler particles develop high stress  points on the surface of the bottom die, which subsequently  causes the thin layers of passivation and metallization to break.


Figure 10: Schematic showing the warpage profile of top die at  molding temperature.


The solutions to prevent mold filler-induced PMD defect can be  generated from either material or assembly process perspectives. In the material aspect, the mold filler size needs adjustment such  that the maximum diameter of mold filler does not exceed the  separation distance between the stacked dice. This option will  require reassessment of the new formulation of the molding  compound material for use during high volume manufacturing. In the assembly process aspect, the ideal solution is to  implement 100% adhesive coverage on the intersection area  between the stacked dice. For film type adhesive-based  packages, this will require cutting the film adhesive into sizes  that equal or exceed the size of the top die. This option is  consistent with the results of the first experiment. Moreover, in  Figure 9, it can be observed that the warpage of top die  dramatically increases in the die overhang region. That  observation is essentially due to having the peripheral portion of  the silicon die not constrained by the adhesive layer. It can be  deduced also that the probability of having mold filler-induced  PMD defect decreases as the adhesive coverage increases. However, the level of tolerable inter-die peripheral gap needs  further study if applicable.


In broader sense, the implementation of 100% adhesive  coverage applies to all die stacking packages that either make  use of either film type or paste type adhesive material. The  previous work of Flores and Bantang demonstrated similar  mechanism governing the occurrence of mold filler-induced  PMD defect on paste type adhesive-based die stacking  package[2]. For such package configuration, the solution will  require complete spread of the adhesive material leading to the  formation of adhesive fillet to ensure 100% adhesive coverage. Additionally, the formation of inter-die peripheral gap is not


only attributed to the dimension mismatch and the insufficient  spread of the adhesive material. It can also be formed by offsetting the placement of top die or the inter-die adhesive layer. On these scenarios, the mechanism of PMD defect described in  this paper is believed applicable as well. Therefore, aside from  the adhesive profile, the placement of the die and the adhesive  must be controlled also.


In the conduct of failure analysis related to the PMD defect  described in this paper, the die backside FA approach can best  identify the mechanism of PMD defect. However, the whole  process can be tedious. Hence, the front side FA approach can  be modified to suit the need for further signature analysis once  the rootcause mechanism is established. An intermediate step of  mapping the mold filler particles at the periphery of the adhesive  using optical microscope is introduced before wet etching the  adhesive layer. The location of the PMD defect should match  the location of any of the large mold fillers. The crosssectioning approach is a “random-walk” FA approach which  may or may generate data that could support the mechanism of  mold filler-induced PMD.


The new rootcause mechanism of PMD defect found in die  stacking package was established. The ways to prevent the  occurrence of the mold filler-induced PMD defect includes  eliminating the presence of inter-die peripheral gap and  adjusting the filler size distribution of the molding compound  material. The FA approaches used to define the failure  mechanism were also described.


The authors would like to acknowledge the significant  contribution of the following people to establish the rootcause  mechanism described in this paper: Melvin Levardo, Mark  Siangco, Rommel Luna, Thomas Sandoval, Neil Caranto and  the late Rommel Casin.


[1] Flores, C.C., “Failure Analysis of Stacked-Chip Scale  Package”, International Symposium for Testing and Failure  Analysis (2000).


[2] C.C. Flores and S. Bantang, “Resolution of PassivationMetal Damage Issue in SCSP”, Proceedings of iPQRS


2006.


Effect of Die Chip-outs and Reflow Temperature on the Mechanical Behavior of a  5-Die-Stacked Chip Scale Package


Dennis Evan L. Balacano, Lito P. De La Rama


Intel Technology Philippines Inc., Gateway Business Park, Gen. Trias, Cavite, Philippines   dennis.evan.l.balacano@intel.com


The corrosion phenomenon was found at the edge area of bond  pad under OM images after dicing saw. Experiment showed  that the corrosion was related with the feed speed of dicing  saw. From SEM and OM results, there were some abnormal  contaminations around the corrosive area. Auger and TEM  with EDX system were used to characterize the corrosive  region and the related Al pad corrosion mechanism was  discussed. In this paper, Cu rich and O rich layers were  identified by TEM and EDX, which could be induced by  galvanic cell reaction.


Pad corrosion is a familiar sight in the field of semiconductor  manufacturing industry. Since the corrosive pad surface can  create an effective barrier to high-quality wire bonding, the  study of pad corrosion had attracted much attention. The  improvement of pad corrosion can make a major contribution  to semiconductor device yield [1-4]. The study of all kinds of  pad corrosion defects has been widely carried out by different  material analytical techniques [5-7], but TEM was hardly used  to analyze the pad corrosion in the published reports.


In this paper, optical microscopy (OM) and Scanning Electron  Microscopy (SEM) results indicated that the bad pad corrosion  was generated after wafer dicing saw and related to the feed  speed. After the pad surface elements were characterized by  Auger Electron Spectroscopy (AES), Transmission electron  microscopy (TEM) cross section analysis and energy  dispersion X-ray (EDX) results gave more detailed  information about the corrosive region of the pad surface. Cu  rich and O rich layers were revealed in TEM images. The pad  corrosion mechanism related to the galvanic reaction will also  be studied and discussed.


Results and Discussion:


Pad appearances and corrosion phenomenon


Figure 1 showed OM (Left) and SEM (Right) images of the  pad surface appearance after dicing saw process at different  feed speed. When the feed speed was 70mm/sec, it could be  observed that the pad surface (Fig.1-b) after dicing saw had no  obvious difference with the normal one (Fig.1-a) except for the  surface silicon dust caused by sawing. Decreasing the speed to  10mm/sec while the cutting manner was the same, discolor  stains were found at the pad edge area from OM image (Fig.1-


c). The SEM image showed that the surface around the stain  area was quite rough.


Fig. 1 OM and SEM images of the pad surface. a) Normal pad  surface; b) with the feed speed of 70mm/s; c) With the feed  speed of 10mm/s.


Figure 2-a is the schematics of partial wafer cross-section  structure. In order to explore what had happened at the pad  edge after dicing saw with the feed speed of 10mm/sec, SEM  was first used to check the cross-section of the pad stain area. As shown in Fig. 2-b, the deep corrosive area (the deepness  was about 200nm) along the pad edge was found from SEM  cross-section image. It seemed that there were some abnormal  layers at the pad corrosive area.


Composition analysis of the pad surface by AES


To confirm the above results and make certain the components  of the contaminated area, AES (Micro-lab350) was used to  determine pad surface elements after dicing sawing with the


feed speed of 10mm/sec. Three different characteristic points  A, B and C at the pad surface were analyzed respectively.


Fig.2 a) Pad Cross-section schematics; b) SEM cross-section  image at the pad corrosion area.


Fig.3. Auger results of different characteristic points. Point A: Corrosion area; point B: With some black stain; point C: Normal area.


Figure 3 showed the AES analysis results. Point C corresponds  to the normal area located in the center area of the pad as  shown in SEM image. The detected carbon, Oxygen and  Aluminum at point C were the routine elements at the pad  surface. The small amount of fluorine signal should result from  the pad etching process. At the point A in corrosion area, abnormal copper signal except for carbon and oxygen was  detected but no aluminum signal was detected. There were no  abnormal elements detected at the point B, which seemed to  have some abnormal contamination compared with the normal  area point C from SEM image. It was difficult to explain how  the abnormal contamination formed and what it was just from  AES results. Where copper signal on point A came from was  another problem to be solved.


Al


Point C


(Normal Area)


C O


Cu  Point A


Point B


Passivation 1 Passivation 2


Al Pad


Dielectric


Cu Metal


Barrier


200nm


Passivation


Fig.4 (a) TEM cross-section overview image at pad corrosion  area; (b) Two layers observed from the zoom in image;(c) Pits  covered with abnormal layer at the pad surface.


Copper diffusion TEM analysis


To fully understand the corrosion mechanism, TEM (TECNAI-F20) with EDX system was used to analyze the root  cause of the generation of Cu signal detected. Here, Focus Ion  Beam (FIB) was used to cut the specific location at pad  corrosion area to prepare TEM cross-section sample. TEM  images were showed in Fig. 4. In the area with abnormal  profile, the pad was divided into two layers, both of which had  different contrasts with the normal area (Fig.4-b). Pits covered  with abnormal layer at the pad surface were also observed in  the pad corrosion area (Fig.4-c). It was very clear from Fig.4-c  that the thickness of abnormal layer was more than 67nm.


Fig.5 EDX line scanning elements analysis result at the  abnormal layer around the pits.


EDX analysis on the abnormal layer around the pits showed  that only Aluminum and oxygen elements were detected in this  layer. From EDX line scanning analysis, this abnormal layer  was oxygen rich film, as shown in Fig. 5


The elements in the normal area and the abnormal two layers  of the pad were also analyzed with EDX separately. The  results are shown in Fig. 6. Only aluminum was detected at  point 1of the normal area. Both aluminum and copper signal  were detected at the two abnormal layers from the results of  Fig.6-a. Less aluminum signal was detected in the top layer. In  addition, the line scanning analysis along the labeled direction  by EDX (Fig.6-b) showed that copper content in the bottom  layer was less than that in the top layer. In other words, top  layer was copper rich layer.


Fig.6 EDX analysis results at the corrosion area (a) Point  analysis; (b) Line scanning analysis.


In addition, in the area  (similar to point B in AES analysis) around the corrosion site, Alumina layer was found very rough  and the thickness was obvious thicker than the normal native  alumina thickness (usually less than 10nm), as shown in Fig. 7-a. From the TEM results in Fig.7-b, the uniformity of the  barrier layer was also not good. The thickness of Ta barrier


O1


O3  O2


EDX result of O2


EDX result of O3


EDX result of O1


Cu


O  Al


Abnormal area


Cu metal  Barrier   Al pad


that used to prevent the diffusion between Cu metal and Al pad  was obviously thinner at the pad corner than that at the center, so pad corner could become a weak point to prevent copper  diffusion.


When dicing saw was in progress, the frame-mounted wafer  was automatically separated according to the programmed die  coordinates. At the same time, the cleaning wafer process was  run by using high pressure DI water and then followed by airblowing drying. DI Water was used to clean the contamination  at the die surface such as silicon dust or foreign materials that  may be attached either by electrostatic, mechanical, or  chemical means. In order to reduce the damage induced by  static charges, it is necessary to put some quantity of Carbon  dioxide into rinsing DI water when sawing and cleaning wafer. For the washing processes, CO2 resistance is the important  parameters for consideration and need to be controlled during  wafer precise dicing saw.


Fig.7 TEM Cross-section images (a) pad surface Alumina  around the corrosion area; (b) Ta barrier thickness at the pad  corner area.


Concerning the corrosion phenomenon, the following model  was given to explain it: As an acidic oxide, CO2 is soluble in  water and can react with water to give carbonic acid as shown  in the following chemical equation:


→


CO


H


The decrease in feed speed directly led to the increase in  sawing time when dicing saw. Thus the water with some H+ and CO32- would stay at the wafer surface for more time. Because the pad edge area was the concave plate, as shown in


Fig.2-a, it was easier to keep the carbonic acid under this  situation. Active Al pad soaked in the acid solvent could be  eroded away along the pad edge, which may account for the  rough pad surface around the corrosion area in Fig.7-a. But it  was not the main reason why the corrosion was so serious at  the pad edge.


From TEM images and EDX results, it was suspected that the  intensive copper signal at the corrosive area might originate  from the metal Cu diffusion. Severe copper diffusion could  have happened at the weak points of pad sidewall or corner, where there could have thinner or broken Ta barrier layer. When dicing saw process was in progress, the temperature of  wafer would rise. Due to the molecular thermal movement, metal Cu would tend to diffuse into the Al Pad region with  lower Cu concentration. Based on the published reports, it was  possible to form Al2Cu theta phase at the diffusion area [1-4,8]. Here two kinds of different active metal Al and Al2Cu were  exposed in the DI water with H2CO3 electrolyte, and the  galvanic cell was thus formed at the edge of the pad. More  active Al pad acted as the anode and Al2Cu as the Cathode. The DI water with CO2 cleaning could induce the following  reactions to happen between Al2Cu and the Al metal. According to the deduction and the results of AES and EDX, the corrosion product was considered to be Cu and  Al(OH)3[2,9].


OH


3 Ale


+ 2


The galvanic cell reaction made Al lose electron and be  oxidized. The pad surface corrosion due to classic galvanic  cell reaction thus occurred in this condition. The abnormal O  rich layer at Al pad surface should correspond to the corrosion  product Al(OH)x (Fig.6-a). At the Cu diffusion area (Fig.4), the top Cu rich layer should also be induced by galvanic cell  reaction. Cu was separated out of the Al2Cu and Al3+ turned  into the precipitate Al (OH)x. The bottom layer didn’t take part  in the reaction. At the area around the corrosion (as shown at  point B during AES analysis), it was suspected that the  abnormal thick alumina was also the production of galvanic  cell reaction, which led to the surface contamination from topview image.


With slow dicing saw feed speed and longer sawing time. Reaction equation (1) would happen which could induce Al  pad corrosion. Due to copper diffusion, reaction equation (2), (3), (4) happened, here, this Galvanic cell reaction should be  the root cause of severe Al pad corrosion in this paper.


Summary and Conclusions


It was possible to form Al2Cu at Cu diffusion area on the weak  point. Al and Al2Cu dissolved in the Carbonic acid and acted  as the anode and Cathode respectively. Galvanic cell reaction  thus occurred. With slow dicing saw feed speed, Al pad


Normal


Corner


corrosion was accelerated due to Galvanic cell reaction, which  was the root cause of Al pad bad corrosion.


To avoid the corrosion phenomenon and improve the  semiconductor device yield, from the point of view of the chip  fabrication process, the thicker Ta barrier layer with good  uniformity is important to prevent Cu diffusion, which may  effectively avoid the Al pad corrosion when dicing saw.


[1] Lawrence, J. D., McPherson and J.W., IEEE/IRPS, (1991)


pp. 102 - 106.


[2] Dunn, C. F., McPherson and J. W., Journal of the


Electrochemical Society, Solid State Science and


Technology, (1988) pp. 661-665.


[3] Hua, Y. N., et al., Proceedings of the 26th ISTFA


Symposium, (2000) pp. 369-372.


[4] Mautz, the 3rd ISCREMD, V94, (2005), pp 253-259.


[5] Daniel Cavasin and Abdullah Yassine, the 31 ISTFA


Symposiums, (2005) pp.31-36.


[6] Kim, D. K., MRSSP, V.594, (1999) pp. 129-134.


[7] Gladkikh, APL, V6, (1995), pp.1214.


[8] S.Mader, Thin Solid Films, V10, (1972), pp.377.


[9] R.T.Foley and T.H.Nguyen, J.Electrochem. Soc., V.129,


(1982), pp.464.


Effect of Inter-Die Adhesive Profile on the Integrity of Die Surface  in Die Stacking Package


Christopher C. Flores and France B. Aspera


Intel Technology Philippines, Inc., Gen. Trias, Cavite, Philippines


As the number of dice stacked within a microelectronic package  increases, the need to maintain die surface integrity also  increases. In this paper, one assembly packaging-related  rootcause mechanism about passivation-metal damage (PMD) will be featured. The profile of inter-die adhesive was found to  play an important role to maintain the integrity of die surface as  more dice are stacked in a microelectronic package. Recommended solution to prevent this type of failure will be  discussed.


Die stacking package technology is becoming popular in the  semiconductor industry. Microelectronic packages of this type  store more than one die or device (see Figure 1) making them  more cost-effective while increasing the capacity of the whole  microchip. As the number of dice stacked gets higher, the need  to maintain the surface integrity of the devices housed in the  package also increases. PMD defect is one of the known die  surface defects that need consideration for solution when  developing and running high volume manufacturing of  microelectronic products that make use of die stacking  technology. The adverse effects of PMD defect may include  high leakage current and reduced density of certain electronic  devices. Therefore, understanding the mechanisms governing  the rootcauses of PMD defect is important to ensure good  performance and reliability of microelectronic products.


Figure 1:  Schematic of typical die  stacking packages.


Previous work showed several mechanisms of PMD defect  ranging from electrostatic discharge (ESD), effect of packaging  material like that of angular fillers present on the inter-die  adhesive[1], contamination on die surface, mishandling of wafer  or singulated die, and even artifact of deprocessing. Its physical  presence may vary from a single hairline crack to a collection of  parallel or radial cracks. Small PMD defects may not be visible  under bright field optical microscope without staining the actual  defective die. When present in small sizes and unstained


condition, PMD defects are best observed under dark field  optical microscope and scanning electron microscope (SEM).


In this paper, the radial type of PMD defect will be discussed (see Figure 2). During the study, the PMD defect occurred in  two types of packages with two-die and three-die stack as  shown in Figure 1. The defect manifested electrically as  parametric failure characterized by high electrical current being  drawn into the device. Commonality in the location of the  failing die and commonality in the location of the PMD defect  on the die surface were established by electrical fault isolation (FI) and deprocessing of failing samples during physical failure  analysis (PFA). The failing die was consistently located at the  bottom of the die stack for both types of packages. Likewise, the  concentration of PMD defects was exhibited on the die surface  specifically around the periphery of the inter-die adhesive layer (see Figure 3) upon mapping the defects found on a number of  failing samples.


Figure 2: Optical micrograph of passivation-metal damage (radial type) as revealed upon wet etching the overlying  adhesive layer.


Figure 3: Result of PMD defect mapping. Die1 is failing bottom  die while Adhesive2 is the inter-die adhesive layer.


Experimental Section


In-depth failure analysis was conducted to determine the  mechanism of PMD defect. In the aforementioned deprocessing, the approach used was frontside failure analysis (FA). In such  approach, the sample was mechanically ground from the  molding compound until the mid-thickness of the silicon die  overlying the failing die. The residual silicon was removed  using dry etching technique followed by wet etching of the  inter-die adhesive layer to expose the surface of the failing die. When the failing device is deprocessed using frontside FA  approach, the PMD defect is obviously found but the evidence  to establish its rootcause mechanism is normally gone. Hence, a  new FA approach must be devised to preserve that potential  evidence.


In this study, backside FA approach was devised to gather both  the defect and the evidence linking the defect to its rootcause  mechanism. In backside FA, the failing sample was  mechanically ground from the solder ball side of the package  until about the mid-thickness of the failing silicon die. The  residual silicon was selectively etched using dry etching  technique. The thin film metallization layers of the failing die  are preserved during dry etching and subsequently inspected for  evidential cracks related to PMD using optical microscope (see  Figure 4) and SEM. When evidential crack was found, microsectioning across the crack was done using focused ion beam (FIB) milling technique. The FIB section was inspected under  SEM. Large spherical particle was found directly on the site  with the crack related to PMD defect (see Figure 5). The  composition of the spherical particle was determined using  energy dispersive X-ray spectroscopy (EDS) and was found  consistent with the silica filler particles of the molding  compound.


Figure 4: Optical micrograph showing the evidential crack  related to PMD defect upon die backside FA deprocessing.


Figure 5: SEM micrograpgh showing the FIB cut revealing the  spherical filler particle cracking the passivation-metal layer.


Likewise, cross-sectioning was done on failing samples to  determine how the mold filler was trapped between the stacked  dice. Cross-section showed that one dimension of the inter-die  adhesive layer was smaller relative to the dimension of the  stacked dice in similar direction. The under-sized adhesive layer  provided the molding compound to seep into the gap between  the stacked dice. Such gap is also located at the perihery of the  inter-die adhesive layer. Hence for discussion reference, it is  called as the inter-die peripheral gap or the die overhang region (see Figure 6). Being present in the molding compound  formulation, spherical filler particles were also found trapped in  the inter-die peripheral gap. By package design, the separation  distance between the stacked dice at the inter-die peripheral gap  must be equivalent to the thickness of the adhesive layer. Hence, it was expected that the maximum diameter of trapped mold  fillers must equate to the designed adhesive thickness. However  in the cross-section of failing samples, mold fillers larger than  the adhesive thickness were also trapped and provided  indentation on the passivation layer of the failing die (see Figure  7). The thickness of the adhesive layer on the failing sample was  generally within specification.  The observed disagreement  raised a hypothesis regarding the potential influence of the  profile of the inter-die adhesive layer on the separation distance  between the dice at the die overhang region which can  eventually result to PMD occurrence.


Deprocessing Result


The failing units are deprocessed to expose the dice. Corner  die cracks are observed on Die 3 of the failing units. Figure 4  shows the locations of the crack. The corner crack can be  found on any of the four corners of Die 3. Figures 5 and 6  show higher magnification images of the corner crack.


Figure 4. Crack locations on Die 3


Figure 5. Die-crack on a blown_up failing unit


Figure 6. Die-crack on an ISBLO failing unit.


As for an ISBLOQ failing units, no corner cracks are observed  on Die 3. But instead of corner cracks, die backside chip-outs  propagating to the active area are observed. Figure 7 shows the  cross-section image with a micro-crack propagating towards  the active area.


Figure 7. Cross-sectional image showing crack originating  from chip-out on the side of Die 3 which failed ISBLOQ


Figure 8 shows the chip-out on the die backside. This kind of  chip-out is observed on both Die 1 and Die 3. Chip-out on the  die backside is the common feature of the blown_up, ISBLO, and ISBLOQ failing units.


DIE 3  Crack


DIE 3


Crack


Chip-out


0.00E+00


5.00E-04


1.00E-03


1.50E-03


2.00E-03


2.50E-03


3.00E-03


3.50E-03


4.00E-03


0 0.2 0.4 0.6 0.8 1 1.2 1.4 1.6 1.8


Voltage


----- Good (30uA) ----- ISB (170uA)


Current


5.00E-03


1.00E-02


1.50E-02


2.00E-02


2.50E-02


3.00E-02


3.50E-02


4.00E-02


0.2 0.4 0.6 0.8 1


1.2 1.4 1.6 1.8


----- Good (30 uA) ----- Blown_up (37mA)


Figure 8. Chip-out on die backside


Fracture Surface Analysis


Backside chip-outs are observed on Die 3 of the failing unit  after deprocessing. Die 1 is also affected by backside chip-outs  but only Die 3 fails electrically. The chip-out is suspected to  be the nucleation site of the die crack and this may possibly  lead to the rootcause of the failure.


Fracture analysis is utilized to understand further the nature of  the die crack.  Results confirmed that the die crack originated  from the chip-out of the die. Figure 9 is a Scanning Electron  Microscope (SEM) image of the fracture surface of Die 3. Figures 10, 11, and 12 are taken from the blue (a), yellow (b), and red (c) areas, respectively, of Figure 9.


Figure 9: SEM Image of Die 3 Fracture Surface


Figure 10 shows the chip-out on Die 3. Based on historical  data, these chip-outs are most likely induced during die  singulation process. The local stress at the area of the chip-out  is much higher than that of the global stress. This geometrical  discontinuity in the die results in a non-uniform stress  distribution at the vicinity of the chip-out.


Figure 10: Image of left box in Figure 9


The fracture surface on Figure 11 is characterized by Wallner  Lines that are concaved to the right suggesting that the crack  initiated from the chip-out on the left. River marks are also


seen on the fracture surface. The River Marks on the fracture  surface suggest that the crack originated from the die backside. The chip-out is located at the die backside edge.


Figure 11: Image of center box in Figure 9


Figure 12 shows the three regions where separate propagation  of crack happened. The clear propagation boundaries are  indicative that the crack propagation is non-instantaneous and  nucleated from the edge chip-out.


Figure 12: Image of right box in Figure 9


It is important to note that this die crack location is near the  over-hang region of Die 3. Figure 13 shows the location of the  over-hang in Die 3.


Figure 13: Over-hang of Die 3


At the stress level when the crack propagates, the critical stress  intensity at the chip-out was overcome by the force applied on  the die. The source of the force is the high stress concentration  on the over-hang area of Die 3. The stress came from the  thermo-mechanical interaction of the failing die with its  neighboring dice and materials.


Considering that Die 1 also has chip-outs on its edges and no  die crack is observed on it after undergoing 3x reflow, this  suggests that chip-out alone is not the only cause of the die  crack. Stress concentration models taken at different areas of  the package are acquired to understand more this mechanical  phenomenon of the die crack.


DIE 3  Chip-out


DIE TOPSIDE


DIE BACKSIDE


Wallner Lines  River Marks


2 3


DIE 3 OVER-HANG


DIE 1  DIE 2  MOLD


DIE 3  DIE 4  DIE 5


SUBSTRATE


c  b


Stress Concentration Analysis


Thermo-mechanical models, taken at different sides of the  unit, are obtained to understand better the mechanical behavior  of the 5-die-stacked chip scale package. The color chart on the  bottom of every diagram indicates the level of mechanical  stress, blue indicates compressive force while red indicates  tensile force.


Figures 14 and 15 show the stress concentration along the  package length of the 5-die-stacked unit taken at room  temperature and at reflow temperature, 240ºC, respectively.


Figure 14: Stress concentration at room temperature along  the package length.


Figure 15: Stress concentration at 240ºC along the package  length.


Comparing the dice stress concentration at room temperature  and at reflow temperature, it can be observed that at 240ºC  temperature, Die 3 is highly stressed. The red and orange  regions are distributed around the over-hang area of Die 3. The  crack propagation on Die 3 is a response of the die to the  stress. The chip-out aggravated the stress experienced by the  die on that area. A die with no chip-outs will behave  differently since there will be no crack initiation point on the  stressed area. We can also observe that Die 1 experiences


lesser stress. This explains why even if chip-outs are present  on Die 1, die crack did not propagate on that die.


The stress concentration models discussed above show the  mechanical behavior of Die 3 on the 5-die-stacked chip scale  package. If die chip-outs coincide with the highly stressed area  of Die 3, and the unit is exposed on a reflow temperature of  240ºC, die crack will propagate. It will most likely form a  corner crack on Die 3 and cause Power ICCS failure. The  temperature change affects the profile of the package which  adds to the overall stress.


Corrective Actions


To address this die crack issue leading to Power ICCS failures, several corrective actions are put into place. The blade life of  die singulation process is reduced to a lower travel distance, slower speed and feed time parameters at saw are used, and a  backside chip-out monitor is put into place. These corrective  actions are intended to eliminate or minimize the die backside  chip-outs. Performance significantly improved after efforts to  reduce chip-out occurrences. From the 4% weekly trigger rate, it was trimmed down to almost 0%.


The combination of chip-outs and reflow temperature of 240ºC  can lead to Power ICCS failures like blown_up, ISBLO, and  ISBLOQ. If chip-outs are present on the area of the die with  the highest stress concentration and the unit is subjected to  reflow temperature of 240ºC, die crack will most likely  propagate from the chip-out.


We would like to acknowledge the support given by Michael  Bravo, Marlene Abelilla, Irene Cimatu, Raoul Masangcay, Janice Mariano, Marcial Ramos and John Saulon of Intel  Technology Philippines; and the support provided by our  Folsom, California colleagues; Jai Kim and Joseph Felde.


[1] C. Flores, Bottom Die Recovery Procedure for Stacked  Chip Scale Package, Intel Internal Document, 2001.


[2] D. Balacano and L. De La Rama, Power ICCS Package  FA Reports, Intel Internal Document, 2005.


[3] J. Felde, 256L/256L/64P/64P Finite Element Model for  Package Stress, Intel Internal Document, 2005.


[4] D. Hull, Fractography: Observing, Measuring and  Interpreting Fracture Surface Topography, 1999.


DIE 3  DIE 1


Reflow Temp


Room Temp


Study of FBGA Burn Failure under THB Test


Jianwei Zhou, Wei Zheng, Minyi Lou, Nufeng Feng, Jaisung Lee, Taekoo Lee


Samsung Semiconductor China R&D Co. Ltd.


Science Plaza 7F, International Science Park, Suzhou Industrial Park, Suzhou, 215021, P.R. China Jianwei.zhou@samsung.com, 86+512-62888288


Temperature humidity bias (THB) test is  widely used to evaluate the moisture resistance of non-hermetic packages in semiconductor industry. During THB test, one kind of 90FBGA was found severely burned and the evidence has been completely destroyed. This brings a great challenge to failure analysis.


In this paper, a double daisy chain structure substrate was designed to reproduce the short and burn failure. The substrate layout design,bias and high humidity environment were proved to be the three key factors inducing  dendrite grown and burn failure. A“corner-missing” phenomenon inspected through nano-focus X-ray was reported and it could finally verify the theory of electrochemical migration. The countermeasure to prevent burn failure was proposed to the designers. The insulation property degradation due to THB test was evaluated.


Key words: Burn Failure, THB, Dendrite,Corner-Missing, Substrate Layout, Insulation Degradation


1. Introduction


It is well known that temperature humidity bias (THB) test is widely used to evaluate the moisture resistance of non-hermetic packages in  the semiconductor industry. The high humidity environment, high temperature and bias will  reveal potential defects of package material and  potential design problem that is difficult to detect at normal conditions. The main failure mode in THB test is electrical short [1, 2], which will make the current increase over the limitation and burn the circuit. To find out the failure


mechanism of electrical short is not easy,because the failure cause will be destroyed when the circuit is burned. After analyzing a lot of  failure cases from THB test, the formation of  metal filaments or dendrites in high humidity conditions is thought to be the major cause for electrical shorts [3-9]. But the causes for metal filament formation are definitely specific at  various conditions or in different cases.


One kind of 90FBGA product was revealed experiencing severe burn failure during THB test(85ºC, 85%RH, 3.3V). There were 27 out of 116 samples failing within 1000h THB test. After inspection, it was found that the failures all had burned substrates on the adjacent plating bar near the edge of the package as shown in figure


110um


THB Burnt Sample


Fig.1 Burn failure at top layer of substrate


Because the failed section was severely burned, the evidence has been completely destroyed. This brought a great challenge to failure analysis.


To better study the failure mechanism,reproducing the failure will be necessary. The substrate was redesigned as a double daisy chain and 4 different areas. The 90FBGA with this kind of substrate experienced 1100h THB test.


Then failure analysis was done to find out the root cause. The failure mechanism was discussed.


The relative countermeasure was proposed. The  insulation property degradation that may induce short failure was also evaluated.


2. Experiment Setup


To ensure the failure mechanism is the same, the materials and the dimension of the package,the substrate vendor, the package manufacturing procedure, and the test conditions were all kept the same as with the previously burned 90FBGA.


Only dummy die samples were used because the burn failure all occurred in the substrate.


Furthermore, the substrate layout (2 layers) was redesigned to make the subsequent failure analysis more convenient.


Fig.2 Bottom layer of substrate


In figure 2, the bottom layer of the substrate is shown as a double daisy chain with pads on the red line connected to 3.3V and pads on the yellow line connected to 0V.


Fig.3 Top layer of substrate


In figure 3, the top layer is shown as a symmetrical structure.


Area 1: 7 traces (2 traces connected to 0V pads, 5 traces connected to 3.3V pads,spacing between traces is 110 m). This area is to simulate the failure site structure


of the previous burned 90FBGA. These biased traces extended to package edge as the plating bar.


Area 2: 4 traces (1 trace connected to 0V pads, 3 traces connected to 3.3V pads,spacing is 220 m). This area is to test how spacing will affect the short failure.


Area 3: 2 traces (both 2 traces connected to


3.3V pads, spacing is 110 m). This area is to examine the bias effect because there is no bias between these 2 traces.


Area 4: 3 traces (1 trace connected to 0V pads, 2 traces connected to 3.3V pads,spacing is 110 m). This area is to study the location effect. The traces in this area  are located deep inside package, do not extend to the package edge, and are not  directly exposed to air.


To force the voltage on the 90FBGA, a test  board designed for this THB test was used. Each package was connected with a 104  protective resistance in series to control the current value within 0.33mA (3.3V/104 ) and to prevent the  destruction of evidence if and when a short  failure occurred.


There were totally 200 units of this redesigned 90FBGA which were tested at the 85ºC, 85%RH,


3.3V condition. The failure criterion was  resistance less than 106 , while the original resistance was about 6*1011 .


3. Result & Analysis


3.1 Color-Changed of Copper Traces


Before THB test, appearance inspection was applied on the 90FBGA. The inspection result showed no obvious defects were found.


Fig.4 Side-look before THB test


But after 200h THB test, there were


color-changed phenomenon occurring around the copper trace on the package surface, as shown in  figure 5 and figure 6.


Fig.5 Side-look after 200h THB test (area 1)


Fig.6 Side-look after 200h THB test (area 2)


After EDS analysis, it was found the materials covering 0V copper traces surface and  surrounding 3.3V copper traces were mainly Cu and O. From this phenomenon, it was supposed that copper would firstly dissolve at the anode,then deposit at the cathode under bias and high humidity environment.


Fig.7 Copper ion dissolution curve


To verify the supposition above,semi-quantitative copper ion test sticks were used to identify whether copper ions would dissolve from the anode traces when there was  de-ionized water on package surface. The result


is shown in figure 7. It confirmed that under bias,Cu atoms at the anode would lose electrons and be oxidized to Cu+ or Cu2+, then dissolve into the de-ionized water. With increasing bias, the Cu+/Cu2+ dissolution rate would also increase.


3.2 Short Failure Analysis


3.3V


0V


After 350h THB, 3 out of 200 samples were found to be failing. With continued testing, more samples failed. Finally there were 13 samples failing in total after the 1100h THB test.


Through microscopic examination, a short connection induced by dendrites could be seen clearly between the adjacent 0V & 3.3V traces on failed samples’ surfaces as shown in figure 8.


Through its appearance, the metal that connected  the adjacent traces was supposed copper. This conclusion was confirmed by EDS analysis as  shown in figure 9.


The dendrites of failed samples were all found to be located on the package surface at area 1. No dendrites could be seen at areas 2, 3 or 4.


The detail experiment result is shown in table 1.


Fig.8 Short connection at area 1 after 1100h THB test


Table 1 Test result of different areas


Spacing Bias


Location


Test Result


Area 1 110um


Extend to package surfaceColor-changed, short failure due to dendrite grown


Area 2 220um


Extend to package surface Color-changed


Area 3 110um


Extend to package surface No defect


Area 4 110um


Inside package


No defect


Fig.9 EDS analysis of dendrite


According to previous reports, traditional dendrite formation should involve path formation resulting from micro-cracks or partial delamination [10]. But no micro-cracks or partial delamination could be found on these samples.


In this case, the package surface has provided a path for dendrite grown. In high humidity environment, a thin moisture layer that may contain only one or more molecular layers will  be present on the material surface. Combined with bias, copper dissolution and electrochemical migration easily occurred on the package surface.


The total electrochemical migration here may include four steps: (1) Moisture absorption and thin moisture layer formation on package surface.


(2) H2O molecule ionization. (3) Cu dissolution& Cu ion migration from anode to cathode. (4)Dendrite growth from cathode to anode.


The three key factors inducing dendrite grown in this case are voltage bias, traces directly extending to the package surface, and a high  humidity environment.


To further study this dendrite grown mechanism, nano-focus X-ray was used to analyze the failure section. From figure 10, it was found that the dendrite only grew on the


package surface, and there was a“corner-missing” phenomenon occurring at the anode. But after parallel polishing, no explanation such as an opening was found at this “corner-missing” anode. Considering the X-ray inspection mechanism, X-ray is very sensitive to  material density. With lower material density, the X-ray image color of this material will be brighter, and vice versa. So actually the“corner-missing” phenomenon is due to uneven density. Density of the copper at the anode corner is relatively lower than that around copper.


This “corner-missing” phenomenon is coincident with the dendrite formation mechanism described above. During electrochemical migration, the anode’s copper atom will lose electron and become a copper ion dissolving into the moisture layer, causing the copper density at the anode corner to become lower.


Fig.10 “Corner-missing” in X-ray analysis


4. Discussion


4.1 Insulation Degradation Evaluation


The insulation property degradation of


dielectric material was also a potential factor that can cause an electrical short failure [11, 12], and  this potential can’t be ignored. To analyze the insulation property degradation of dielectric material, an insulation resistance test was used.


Considering the dendrite that is located on the package surface would affect the substrate’s insulation resistance value, all samples were measured twice to eliminate this effect. The first time all samples were measured without any pretreatment. The second time all samples were measured after slight edge polishing was used to remove dendrites. The test result was as figure


11.


Fig.11 Insulation resistance of 90FBGA


From the figure, it was found the samples resistances after polishing showed some increment than that before polishing. It meant that dendrite formation on the package surface  can slightly decrease the substrate’s insulation resistance. And both insulation resistance curves showed decline after THB test. This means that the insulation property of the dielectric in the  package would degrade with the THB test time.


Before THB test, the samples resistance was about 6*1011 . But after 1100h THB test, the samples resistance degraded to only about 7*109


. But of course, this 7*109  resistance was still high enough to prevent dielectric failure occurring internal to the substrate.


4.2 Substrate Design Modification


According to the failure analysis result above,the substrate design of the burned 90FBGA


product was modified. No bias was applied on the adjacent plating bar any more. This modified 90FBGA design showed improved moisture resistance. Even after the 1100h THB test, no  electrical short failures were found.


5. Conclusion


Generally speaking, this experiment could finally reproduce the failure situation which occurred on the previously burned 90FBGA, and led to changes which can prevent the dendrites from forming and causing a failure.


A thin moisture layer would form on the package surface in a high humidity environment.


This moisture layer could cause electrochemical migration when biased adjacent traces extended to package surface. It turns out that the substrate layout design, the high humidity environment,and the bias were the three key factors inducing dendrite grown and short failure in this case.


To solve the burning or short failure problem and improve the package product reliability, the substrate layout design was found to be critical.


One necessary design rule that should be considered by the designers is avoiding forcing bias on an adjacent plating bar, or preventing biased adjacent traces from directly extending to the package surface and being exposed to air.


The insulation property of dielectric material in package can suffer degradation with THB test  time. But even the degraded resistance after 1100h THB test was still high enough to prevent dielectric failure occurring internal to the  substrate.


1. G. Harsanyi, G. Inzelt, “Comparing migratory resistive short formation abilities of conductor systems applied in advanced interconnection systems”, Microelectronics Reliability, Vol.41, pp.229-237, (2001).


2. K. H. Yip, Xue Ming, “Analysis of a new BGA THB failure and study on its mechanism”, Electronics Packaging


Technology Conference 2002, pp.410-412.


3. IPC


publication,


IPC-TR-476A, “Electrochemical migration: electrically  induced failures in printed wiring  assemblies”, Northbrook, IL, May 1997.


4. G. DiGiacomo, “Metal migration (Ag, Cu, Pb) in encapsulated modules and  time-to-fail model as a function of the  environment and package properties”, International Reliability Physics Symposium,pp.27-33, (1982).


5. E. Bumiller, M. Pecht, C. Hillman, “Electrochemical migration on HASL plated  FR-4 printed circuit boards”, Journal of  Surface Mount Technology, Vol.17, No.2, pp.37-41, (2004).


6. J. Augis, et. al., “A humidity threshold for  conductive anodic filaments in epoxy glass  printed wiring boards”, Proceedings of 3rd International


SAMPE


Electronics  Conference, pp.1023-1030, (1989).


7. W. Ready et. al., “Microstructure of  conductive anodic filaments formed during  accelerated testing of printed wiring boards”, Circuit World, Vol.21, No.4, pp.5-10, (1995).


8. K. Rogers, C. Hillman, M. Pecht and S. Nachbor, “Conductive Filament Formation  Failure in a Printed Circuit Board”, Circuit  World, Vol.25 (3), pp.6-8, (1999).


9. M. Pecht, C. Hillman, K. Rogers and D. Jennings, “Conductive Filament Formation: A Potential Reliability Issue in Laminated  Printed Circuit Cards with Hollow Fibers”, IEEE/CPMT, Vol.22. No.1, January 1999.


10. C. Hillman, “Improved Methodologies for  Identifying Root-Cause of Printed Board  Failures”, Microelectronics Failure Analysis  Desk Reference - 5th Edition, pp.524 – 541, ASM International, Materials Park, OH, (2004).


11. Y. Li, B. Gao, J. Unsworth, “Degradation of  epoxy insulation under combined high  humidity and elevated temperature”,


Proceedings of the 4th International  Conference on Properties and Applications  of Dielectric Materials, pp.752-755, (1994).


12. Kyung-Bum Lim, Duck-Chool Lee, “Study  of the surface degradation mechanism of an  epoxy insulator exposed to water”, Journal  of the Korean Physical Society, Vol.37, No.1, July 2000, pp.49-54.


A New Methodology for Electrical Debugging Short in Packages  with the Modified Daisy-Chain Die


Steve K. Hsiung, Kevan V. Tan, John Soopikian


LSI Logic Corporation, 3098 West Warren Avenue, Fremont, California 94539


Tel: (408) 433-8838 Fax: (408) 433-8193 Email: steve.hsiung@lsil.com


Packages with the Modified Daisy-chain (MDC) die  have been used increasingly to accelerate reliability  stress testing of IC packaging during package


development, qualification, and evaluation and


reliability monitor programs [1].  Utilizing this


approach in essence eliminates chip circuit failure


mechanisms.


Unlike packages with active die, in packages with the  MDC die, when short occurred between two daisychain pairs of I/Os, there are four possibilities that


can attribute to each pin of the two daisy-chain pairs. That makes the isolation of short failure difficult.


Time Domain Reflectometry (TDR) is a welldescribed technique to characterize package


discontinuity (open or short failure).  By using a bare  package substrate and a reference device, an analyst  can characterize the discontinuity and localize it:


within the package, the die-package interconnects, or  on the die [2].


Scanning SQUID (Superconducting Quantum


Interference Device) Microscopy, known as SSM, is  a non-destructive technique that detects magnetic


fields generated by current.  The magnetic field,


when converted to current density via Fast Fourier


Transform (FFT), is particularly useful to detect


shorts and high resistance (HR) defects [3].


In this paper, a new methodology that combines


Resistance Analysis, TDR Isolation and SSM


Identification for electrical debugging short in


packages with the MDC die will be presented. Case  studies will also be discussed.


Packages with active die had been major vehicles in  the mainstream for reliability stress tests. However, in a circumstance that package development needs to  be accomplished simultaneously or even prior to the


active die development, packages with non-active die  are necessary.


Packages with the Modified Daisy-chain (MDC) die, designed at LSI Logic, can be used for all phases of  accelerated reliability stress tests used for packages


with active die with major advantages: significant


less cost and delivery time; simpler board design; no  susceptibility to ESD by handling and conductive to  socketless-direct board attach test vehicles [4].


The MDC die simply consists of traces needed to


complete a substrate circuit. A daisy-chain pair on the  MDC die is comprised of two I/O pins that connected  by top metallization on the die. (Figure 1 and Figure  2).


Figure 1 A layout of a daisy-chain die in flip-chip


package


Figure 2 A bond-pad-design of the MDC die in wirebond packages


Since these package structures are different, the ATE  methodology varies: the packages with active die are  tested Continuity Open/Short, Functional Test etc


while the packages with the MDC die are tested only  Continuity Open/Short. By using the MDC die, dierelated detects are discounted [5].


The approaches for Continuity Open/Short failure


analysis in the package with active die distinguish


from that with the MDC die. Table 1 lists the


difference.


Active Die


MDC Die


Equipment Curve Tracer


Multimetre


Observation Diode Curve


Resistance


Measurement Pin vs VDD or  VSS


Pin to Pin in one  or two daisychain pair


Table 1 Comparison of FA approaches


Pin-to-pin short is a common failure mode. In


packages with active die, the failure could be easily


fused open during the ATE testing. That concern is


eased for package with the MDC die.


However, a new challenge has surfaced. For pin-topin short, there are only two pins involved in


packages with active die, but in packages with the


MDC die. two daisy-chain pairs that have totally four  pins involved.


Therefore, how to isolate chain-to-chain short with


four pins involved down to pin-to-pin short with only  two pins involved becomes necessary.


A new methodology for electrical debugging short in  packages with the MDC die that combines Resistance


Analysis, TDR Isolation and SSM Identification has  developed. Not only does it addresses the challenge  mentioned above but it improve efficiency of failure  analysis.


Resistance Analysis


As mentioned above, the MDC die consists of


multiple daisy-chain pairs. Each pair has two I/O pins  that are connected by top metallization (Figure 3).


Figure 3 A schematic of two daisy-chain pairs, A-B  and C-D on the MDC die


When pin-to-pin short occurred in packages with the  MDC die, it actually caused four pins short.  In the


illustration show above where pair A-B and pair C-D  are shorting, they are four possibilities that could


result in short:


A-C


A-D


B-C


B-D


It is critical to narrow down the four possibilities to  one. The Resistance Analysis is to measure resistance  in all four combinations and the one with least


resistance has pin-to-pin short.


The theory behind this new metrology is that short


always follows the path with least resistance.


Figure 4 is a schematic of the equivalent daisy-chain  circuits that proves the theory.


Metallization


Figure 4 A schematic of the circuits that show the  short follows the path of least resist


Take the above example, if the resistances measured  are as listed in the table below:


Combinations Resistance (Ohms)


2.6


1.3


3.1


Table 2 Resistance measurement


Then the short must be between pin B and pin C,


because the resistance is the least among all four


combinations.


TDR Isolation


Time Domain Reflectometry (TDR) Isolation, after  the short is narrow down to two pins, is the next step  to distinguish short in package substrate from die or  interconnects.


SSM Identification


Scanning SQUID Microscopy (SSM) is a nondestructive technique that detects magnetic fields


generated by current.  The magnetic field, when


converted to current density via Fast Fourier


shorts and high resistance (HR) defects.


Without Resistance Analysis and TDR Isolation,


SSM would have to be run four times for all


combination. Right now, only one scan is needed


followed by dada analysis. Table 3 shows how time  saving and cost reduction are significantly. That is  the biggest advantage of the new methodology.


Old  Way


New  Way


% in  Saving


Time Saving (hour)


Cost Reduction ($)


2,000


800 60% Table 3 Comparison of the old and new way


Case Studies


Case Study I


Background: One daisy-chain pair AE8-AE9 is


shorting to another daisy-chain pair AF8-AG7 in a  flip-chip package.


Resistance Analysis: The resistance measured


between all four pins as listed as:


Pin-to-Pin


Resistance (Ohms)


AE8-AF8


17.27


AE8-AG7


17.50


AE9-AF8


16.97


AE9-AG7


17.22


Table 4 Resistance measurement in Case Study I


The short is narrow down to pin AE9 and pin AF8  TDR Analysis: TDR signatures in the pin AE9 and  AF8 characterized short as package-substrate related (Figure 5 and Figure 6).


Figure 5 TDR signatures of the failing pin AE9 that  characterized short as package-substrate related


RAC=Rc


Figure 6 TDR signatures of the failing pin AF8 that  characterized short as package-substrate related.


SSM Identification: The unit was analyzed by SSM. First, the part was scanned from die backside, after


the die was thinned down to 100 microns. The SSM  current density overlaid substrate layout confirms


that the current goes through AE9 to AF8, meaning it  was the area where short occurred. Then the unit was  scanned from package side, after solder balls were


removed. The SSM current density overlaid substrate  layout confirmed that short occurred between pin


AE9 and pin AF8 in the substrate (Figure 7 and


Figure 8).


The interest area was parallel-lapped sequentially and  revealed anomalies in the 3rd layer substrate (Figure  9). The part was sent to substrate vendor for further  analysis.


Figure 7 SSM current density image taken from die  backside overlaid substrate layout shows the current  goes through AE9 and then made a turn at AF8 that


confirmed the short occurred between pin AE9 and


pin AF8


Figure 8 SSM current density image taken from


package side overlaid substrate layout shows the


current goes through AE9 and then take a turn at AF8, and again confirmed the short occurred between pin


AE9 and pin AF8 in the substrate


Figure 9 Optical image in dark field of an anomaly


between the via ring of pin AE9 and pin AF8 at 3rd


layer substrate.


Case Study II


Background: One daisy-chain pair D37-C38 is


shorting to another daisy-chain pair E37-C39 in a


wire-bond package.


AF8


AE9


AE9  AF8


Area of  Short


D37-E37


8.77


D37-C39


12.09


C38-E37


12.21


C38-C39


15.47


Table 5 Resistance measurement in Case Study II


Obviously, the shot should be between pin D37 and  E37.


TDR Analysis: TDR signatures in the pin AE9 and  AF8 characterized short as package-substrate related (Figure 10 and Figure 11).


Figure 10 TDR signatures of the failing pin D37 that  characterized short as package-substrate related


Figure 11 TDR signatures of the failing pin E37 that  characterized short as package-substrate related


SSM Identification: Mold compound in this wirebond package was thinned down the top of the loop  of the bond wires. The failure pin D37 and E37 was  powered up and scanned by SSM. The SSM current  density image overlaid X-ray image and substrate


layout indicates the area of short (Figure 12).


The substrate was parallel-lapped to the 2nd layer and  revealed anomalies material between metal traces of  the failing pin D37 and E37 (Figure 13).


Figure 12 SSM image overlaid X-ray image and


substrate layout indicate the area of short


Figure 13 Optical image of anomalies material


between I/O traces of the failing pin D37 and E37 at  2nd layer substrate


Conclusion


In this paper, a new methodology for electric


debugging short in packages with the Modified


Daisy-chain (MDC) die that combines Resistance


Analysis, TDR Isolation and SSM Identification is


introduced. Case studies have also proven it is


successful. Data has shown its biggest advantage of  time saving and cost reduction.


D37


E37


The authors wish to thank their colleagues at LSI  Logic, and Jan Gaudestad at Neocera Inc. for their  support in failure analysis.


[1] Grilletto, C, et al., “Modified Daisy Chain Test


Die”, Semiconductor International-Semiconductor


Packaging, December 2005, SP-8


[2] Tan, K, et al., “Integration of Package Analysis


Tools to Solve Discontinuity Failures”, 2005 ISTFA  Proceedings, pp.475


[3] Hsiung, S, et al., “Failure Analysis of Short Faults  on Advanced Wire-bond and Flip-chip Packages with  Scanning SQUID Microscopy”, 2004 ISTFA


Proceedings, pp.73


[4] Grilletto, C, LSI Logic Internal Presentation,


December, 1998


[5] Grilletto, C, “Electrical Testing of Reliability


Stressed Packages”, LSI Logic Internal Memo, May, 2000


Study of a systematic low DPPM reliability defect without common electrical signature


Fubin Zhang


Texas Instruments Inc. DDAO, Dallas, TX  fzhang@ti.com


Possible reliability failure mechanisms on mixed-signal IC are  reviewed and categorized. Based on the nature of reliability  and low DPPM failures on mixed signal IC, an analysis flow  is proposed including identification of individual failure  mechanisms, extraction of the systematic problems, and  implementation of corrective actions. Finally, a case of  successful isolation of a specific defect without common  electrical signature on mixed-signal devices is presented.


Integrated circuit reliability becomes more and more  important factors in the competition between semiconductor  companies. Failure analysis is crucial for identifying failure  mechanisms and improving IC device reliability. However, as  device feature sizes shrink and complexity increases  dramatically, it is more and more challenging to perform  failure analysis in a timely and cost-effective manner. Tricky  problems like low DPPM (Defective Part per Million), reliability failures make the analysis even more difficult and  time consuming. But it is essential to achieve the zero-defect  level in some specific applications such as the mixed-signal  devices used as power drivers and signal processors in severe  environments like the automotive, aerospace, and other heavy  industries. To this end, many innovative solutions for failure  analysis have been developed during the last decade.


Reliability failures of Mixed-signal IC


Figure 1 shows a simplified IC manufacturing and failure  flow. Most of the failing devices can be filtered out at wafer  level probing and package level final test. However, there are  still some parts which fail after reliability tests or in the  application field after a period of time. The nature of these  failures implies that the environmental and operational  conditions are playing an important role in the failure  mechanisms. These failures can be divided into two groups: 1) die related (for instance a latch-up occurred in one block); 2) package related problems (like delamination at die surface). For field returns, the failures also can be categorized into one  of these two types.


Sometime, reliability failures exhibit similar electrical  symptoms which provide a fast and effective signature  analysis approach to identify the root cause. However, this is  not always the case. Systematic low DPPM reliability failures  without common electrical characteristics require more detail  analysis and data collection and extraction, especial for  mixed-signal devices.


Methods and Analysis


Figure 2 shows major analysis steps to solve low DPPM  reliability problems without common electrical signature. Each step will be discussed in detail below:


Figure 1: Simplified IC manufacturing, testing and failing flow block diagram


Assembly  Packaging


Field


Application


Wafer


Processing


Reliability  testing


Fail Units Fail Units


Wafer Probe  test


Final test


Time-zero failures


Figure 2: Major steps in analyzing low DPPM reliability  failures on mixed-signal devices.


Identification and categorization of individual failure  mechanism


Mixed-signed devices consist of both a digital core and analog  blocks. In most cases, ATE data log review can indicate which  blocks are related to the failure. Then global fault isolation  techniques [1] including PEM (Photon Emission Microscopy) and Laser Scan Based OBIRCH (Optical Beam Induced  Resistance Change) or TIVA (Thermal Induced Voltage  Alteration) can be used to isolate the failure on the die. And, if  it’s possible and necessary, micro probing will be used to  isolate the fail site down to the transistor or metal line level  for analog blocks or cell level in the digital core. Finally, die  delayering and physical defect characterization are done to  identify the failure mechanism.


After the failure mechanism is identified, it should be  categorized and saved in a tracking system. Other than the  package related problems, most of the failure mechanisms of  silicon die can be categorized into interconnection level and  transistor level in terms of the locations of the physical  defects.


(1) Interconnection level (back end):


The defects at interconnection level primarily include  electrical resistive/open metal lines and leakage/short between  adjacent metal lines. Open via, under-etched metal residual  and ILD (Inter Level Dielectric) cracks causing metal-metal  leakage are typical interconnection level defects. For instance, a resistive via which becomes totally open after thermal cycle  test could cause a reliability failure.


(2) Transistor level (front end):


Transistor level defects could cause MOSFET threshold  voltage shift, substrate junction leakage and so on. Doping  defects, silicon level contaminations, silicon crystalline  defects and poly silicon defects are among the most frequent  ones. These defects could cause a weak transistor which will  fail after a period of time.


Extraction of systematic problems


The extraction of systematic problems should be based on  physical failure mechanisms and characterization of the  defects. It is helpful to periodically check categorized failure  mechanisms or physical defect signatures from the same  process technology to determine if any similarity occurred  between them even at a very low DPPM level. A tracking  system with failure analysis history is ideal for the extraction  of systematic problems.


Implementation of corrective actions


Corrective actions can be silicon manufacturing process  improvement, a circuit/package design change, or a test  program modification to solve the problems. Silicon  manufacturing process improvement is to eliminate the defect  from the process. The circuit/package design can be changed  to be more robust and will not fail even the same defects occur  again. Test program can be modified to filter out this type of  defects, for instance OVST (Over Voltage Stress Test).


Case Study


Two types of devices (A and B) are analyzed. Both are  processed on the same Bi-CMOS technology. They are mixedsignal IC used in automotive applications. Cases 1 and 2 are  from device A (Figure 3). Cases 3 to 6 are from device B (Figure 7).


Case 1


The failure mode was confirmed on the ATE and bench level  setup. One analog block was failing with leakage on an  internal regulated power supply. Global fault isolation (PEM  and liquid crystal analysis) was not conclusive. The fail site  was narrowed down to a section of V3int metal 1 line using  FIB isolations. A tungsten plug defect was observed (Figure  4) after it was parallel polished down to metal 1.


Case 2


This failure was an ADC (Analog to Digital Converter) nonlinearity problem. Global fault isolation did not provide  any direct information related to the failure. Extensive micro  probing revealed a leaky node in the ADC switching capacitor  network. FIB (Focused Ion Beam) cuts and voltage contrast  isolate the fail site down to a resistor network. Also a tungsten  plug defect was observed at metal 1 level (Figures 5 and 6).


Systematic


problem extraction  Individual analysis and


categorization


Corrective Action


Figure 3: Optical image of Device A die. Fail sites identified  in cases 1 and 2 are indicated with red arrows.


Figure 4: (Case 1) SEM (scanning electron microscopy) image of the cross section through the fail site showed an  anomaly between V3int and GND lines (blue arrows).


Figure 5: (Case 2) Close-up optical image of the failing area  at metal 1 level showed an anomaly (red arrow) next to node  rtree_vref_hi.


Figure 6: (Case 2) FIB image of the cross section through the  defect at metal 1 level showed a tungsten plug (red arrows) next to node rtree_vref_hi.


Figure 7: Optical image of Device B die. Fail sites identified  in cases 3 to 6 are pointed out with red arrows.


Case 3


In this case, an emission site was detected in the digital core (Figure 8). Incorrect digital voltage bias leads to a leakage on  the failing node. FIB cuts isolated the fail site to metal 1 line  on the node. A W-plug defect was observed on the FIB cross  section through the fail site (Figure 9).


Case 4


This was a failure related to an operational amplifier in the  analog blocks of the device. Micro probing revealed a leaky  node. FIB cuts and voltage contrast narrowed down the fail  site (Figure 10). A W-plug was observed at the fail site (Figure 11).


Figure 8: (Case 3) Photon emission microscopy image of the  failing die showed an emission spot (red arrow) in the digital  block.


Figure 9: (Case 3) FIB cross section through the fail site  showed a tungsten plug defect (blue arrows), bridging the two  adjacent metal 1 lines of LVL1<2> and LVL1<3>.


Case 5


This failure is a similar to case 3. PEM identified an  anomalous emission spot in the digital core (Figure 12). A  tungsten plug was observed on the cross section through the  fail site (Figure 13) at metal 1 level.


Case 6


In this case, PEM also lead to the fail site. However, the  defect was located in the digital core and right at the emission  site (Figures 14 and 15). FIB cross section showed a W-plug (Figure 16).


Figure 10: (Case 4) FIB slow scan and voltage contrast on  node 6 showed a leaky section of metal 1. The fully isolated  metal 1 section of node 6 remained bright, indicating a  leakage. Blue arrows point to FIB cuts.


Figure 11: (Case 4) FIB cross section through the fail site  showed a tungsten plug defect (blue arrows), bridging the two  adjacent metal 1 lines of LVL1<2> and LVL1<3>.


Figure 12: (Case 5) Photon emission microscopy image of the  failing die showed an emission spot (red arrow) in the digital  block. All other emission sites were the same as those on a  correlation unit.


Figure 13: (Case 5) FIB cross section through the fail site  showed a tungsten plug defect (red arrows), bridging the two  adjacent metal 1 lines of LVL3<2> and LVL3<3>.


Figure 14: (Case 6) Photon emission microscopy image of the  failing die showed an emission spot (red arrow) in the digital  block (top) and another emission site in the valve driver block (bottom red arrow). All other emission sites were the same as  those on a correlation unit.


Figure 15: (Case 6) Close-up optical image of the anomaly  observed between metal 1 lines of n4661 and n6211.


Figure 16: (Case 6) FIB cross section through the fail site  showed a tungsten plug defect (red arrows), bridging the two  adjacent metal 1 lines of nodes n4661 and n6211.


Summary


In all these 6 cases, they exhibit different electrical signature, but the same physical defects (tungsten plugs) were identified  as the root cause, indicating a systematic manufacturing  process related problem. All these devices were processed at  one fabrication site using the same Bi-CMOS technology and  were returned and analyzed during the 12 months of 2006. Although the DPPM for the devices was low, a process  improvement has been developed and implemented to solve  this systematic problem. It’s noted that the time period to  accumulate these cases is critical and phenomenal because of  the nature of low DPPM failures.


Conclusions and Acknowledgments


Major steps in failure analysis of low DPPM reliability  failures have been proposed. This includes Identification and  categorization of individual failure mechanism, Extraction of  systematic problems and Implementation of corrective actions. As demonstrated in the case study, this analysis methodology  can generate positive results, even for failures without  common electrical signatures.


The author would like to thank Daniel Callahan and Corey  Lewis for their support of the work in this paper.


[1] Microelectronics Failure Analysis, Desk Reference Fifth  Edition, Chapters 8 and 10.


Laser Assisted Lock-in Phase & Spectral Analysis Techniques at Advanced IC  Failure Analysis with Application to Jitter and Soft-Defects


Christof Brillert, Zhongling Qian, Christian Burmer


Infineon Technologies AG, Failure Analysis, Munich, Germany  christof.brillert@infineon.com


New developments concerning lock-in phase detection and  spectral analysis techniques applied to accessible IC signals  are introduced in detail. These techniques combine the thermal  laser stimulation (TLS) with the high sensitivity of lock-in to  phase variation or the selectable frequency detection in  spectrum analyzer. The difference to normal lock-in  techniques utilizing pulsed lasers is exemplary pointed out. Moreover the applications to phase related soft-defects and to  a design related jitter problem are shown. The power of such  techniques for direct mapping a signal path is shown. Further  benefits of lock-in phase methodology and spectral analysis  technique applied to 65 nm and 90 nm technology is presented  and illustrated using different case studies.


Failure analysis of high performance ICs with increasing  number of metal layers and sub micron feature size is an  ongoing topic of advanced failure analysis. The main backside  global localization techniques such as photoemission  microscopy (EMMI) or TLS have met a great challenge  [1,2]. Modern IC’s are frequently designed with full scan design  including the idea for design of testability (DFT). Based on  the implementation of diagnosis features in combination with  automatic test pattern generation (ATPG) a hierarchy list of  possible fault candidates can be generated - in best case one  suspicious net. A combination of physical localization of TLS  in static device mode with the results of software based  localization can be used for improved fault isolation [3]. In  principle, electrical failures showing a voltage, temperature or  phase dependency can be solved with optical probing  techniques like LVP (Laser Voltage Probing) or TRE (Time  resolved Emission) [4]. However, for these techniques usually  higher requirements concerning device preparation and/or  exact knowledge about useful probing area are required. Global localization of soft failure signatures can be  successfully solved with another method called soft defect  localization (SDL) [5-8].


In this paper a timing related lock-in phase and spectrum  approach is shown and discussed on different case studies. Especially the benefit and power of a direct global localization  with introduced techniques in comparison to time consuming  electrical and optical probing techniques is discussed.


Figure 1: General setup for laser related lock-in/spectral  techniques: With laser modulation for Lock-in TLS or periodic  stimulation SI and with lock-in phase & spectrum signal  analysis facilities at a device chain output SO or supply Vdd


General Setup


The general setup for laser based lock-in and spectral TLS  techniques is shown in figure 1.  Enhancement of signal with  lock-in technique can be realized by pulsing the laser beam or  aligning to a periodic input signal (SI) of a device chain. The  used laser is a 1.3 um high power laser (400 mW) which is  integrated in a photoemission microscope. Classical lock-in  technique related to laser based failure localization is done by  using a pulsed laser modulated with frequencies in the kHz  range [9]. As lock-in reference the periodic laser modulator  stimulation signal f is used. The detection is performed at the  relevant power supply Vdd. In case of lock-in phase detection  technique, an accessible device signal like the output of a  bypass chain of a failing IC can be used for detection and  a  corresponding input signal as reference signal. Therefore laser  beam pulsing is not required and applied. The phase technique  is not restricted to phase and operation frequency related  problems at digital chains. It can also be applied to recover a  periodic analog signal with very low voltage swing, particularly in a noisy environment. The accessibility of  failure related signals can be realized by test bus concepts, which are often integrated in modern mixed signal devices. The benefit and application of lock-in amplitude signal in  LIA-SDL was discussed in [10]. The periodic TLS/SDL signal  detection can also be realized as shown in the schematics by


selecting the particular frequency component from a spectrum  analyzer in the case where no reference signal is available.


Case study 1: Lock-in phase & amplitude at via  chain with laser modulation


During package qualification, a 5-die-stacked chip scale  package was being marginally triggered on high stand-by  current collectively known as Power ICCS failure. Affected  lots are subjected to 3x reflow at 240ºC. Post reflow failures  include blown_up, high standby current in Vcc pin (ISBLO), and high standby current in Vccq pin (ISBLOQ). Backside  chip-outs are observed on Die 1 and Die 3 of the three failures. Electrical validation showed that only Die 3 is failing. Corner  crack on Die 3 is common to the blown_up and ISBLO failing  units while crack on Die 3 backside is observed to propagate  toward the active area on ISBLOQ failing units. Fracture  analysis results show that the crack of the three failures all  originated from die backside chip-out. Thermo-mechanical  model of the package shows that, by design, Die 3 generates  the highest stress concentration. Results show that if chip-outs  are present on the area of the die with the highest stress  concentration and the unit is subjected to reflow temperature  of 240ºC, die crack will propagate from the chip-out. This  paper presents the unique failure mechanism observed on a 5-die-stacked chip scale package and the corrective actions  applied to solve the issue.


The increasing demand for high end electronic devices  incorporating multiple functions in a small form factor leads to  the widespread use of Stacked Chip Scale Packaging (SCSP) in the semiconductor industry. Multiple die stacking in various  combinations have been achieved. However, new failure  mechanisms are being observed due to the interaction of die  defect with the package stress.


The package of interest is a 5-die-stacked chip scale package  incorporating four active dice and one silicon spacer. During  package qualification, it was being marginally triggered on  high standby current collectively known as Power ICCS  failure. Failures include blown_up, ISBLO, and ISBLOQ. Fail  rate ranges from 0.31% to 0.8%. It can go as high as 4% fail  rate. The package schematic is shown in Figure 1. Die 3 or the  top Flash is always the failing die.


Figure 1. Schematic of a 5-die-stacked chip scale package


Lots affected by Power ICCS are subjected to three times  reflow (3xIR) at 240ºC in order to screen-out the failing units. Post reflow failing units fail blown_up, ISBLO, and/or  ISBLOQ. Die 3 is always the failing die. Failing units are  endorsed for failure analysis.


Failure Analysis Flow


Semiconductor Parameter Analyzer (SPA) is used to validate  the failures on Die 3 of the endorsed units. External and X-ray  inspection are performed prior to deprocessing. Initial failure  analysis approach is to expose Die 3 using a bottom die  recovery procedure. Removal of the unwanted materials on top  of Die 3 is achieved using a planar polishing technique.  The  molding compound and Die 5 are removed leaving the Die 4  silicon exposed.  Afterwhich, reactive ion etch of the Die 4  silicon is performed to expose the die attach adhesive on top of  Die 3.  The final step is to do acid jet etch, or partial  decapsulation, to remove the adhesive and expose the Die 3  active surface. Full decapsulation is performed later to expose  all sides of Die 3 and the remaining dice, Die 2 and Die 1. Fracture surface analysis of the die crack and cross-sectional  analysis on other failing units are performed. Thermomechanical model of the package is acquired to better  understand the failure mechanism.


DIE 1 = Flash  DIE 2 = Spacer  MOLD


DIE 3 = Flash   DIE 4 = xRAM  DIE 5 = xRAM


Results and Discussions


Electrical Validation


Electrical validation using SPA is performed on the failing  units. The common failures of the Power ICCS issue include  blown_up, ISBLO, and ISBLOQ. Figure 2 shows the electrical  curve of a blown_up failing unit with a current reading of 37  mA. The lower limit for blown_up failure is 400 uA. The  current reading of a good unit is around 30 uA.


Figure 2. I-V curve of a blown_up failing unit.


Figure 3 shows the electrical curve of an ISBLO failing unit  with a current reading of 170 uA.  The threshold for ISBLO  failure is 85 uA. Leakage current is measured at VCC value of


1.8V.


Figure 3. I-V curve of an ISB failing unit


Case study 3: Soft defect at bypass chain


The following case study show an example for application of  lock-in phase technique at a soft-defect. After ESD test  devices from 90 nm technology fail at bypass test with voltage  dependent signature at supply voltages below Vc = 0.95 V, shown in figure 4 (a) and (b). As lock-in reference the input  signal of the failing bypass chain was used. The result of  localization with lock-in phase technique with working point  at critical power supply voltage Vc is shown at figure 4 (c). The phase sensitive area is marked with an arrow. With minor  voltage change of the working point a 180° phase transition - anti phase - could easy be observed. After lift-off a ESD  damage at a n-MOS transistor of one driver before the bypass  output pin was observed. An SEM image of the defect is  shown at the inset of the figure 4 (c).


Devices with this characteristic soft-defect signature  at a bypass chain show sometimes a very weak EMMI/TIVAspot. Localization was not always direct, whereas the lock-in  phase technique provides us reliable direct localization of the  physical defect.


Figure 4: The output signal of a failing bypass chain  showed  180° phase transition to the input for Vdd < Vc (a) The bypass  chain phase dependence of supply voltage is shown (b) Localized phase lock-in spot is marked with an arrow at  location of the physical defect (c) the inset shows SEM image  with ESD damage after lift-off


Case study 4: Path mapping at high frequency  with Lock-in phase technique


At this case study the aim was to check if lock-in phase  technique can be utilized for global path mapping of a bypass  chain. A non failing device with bypass chains from 90 nm  technology was used. The device was thinned to 100 um  thickness. As lock-in reference the bypass input signal was  used. In contrast to case study 3 were the input signal  frequency was around 5 kHz in this case the input signal  frequency was increased up to 50 MHz for better phase  sensitivity. Moderate slow-scan and frame integration was


used to improve signal noise ratio. Under this conditions it  was possible to image the global path of a bypass chain  through the complete chip. The result of path mapping at the  central area of the chip with high NA 50x lens is shown at  figure 5 (a). The lock-in phase signal was green colorized and  an overlay with the pattern image was performed. The nets at  the layout which are related to the stimulated physical bypass  path are red colorized and overlaid to the image. The overlaid  green net shows an alternative fork which could be from  schematics view on the path. The schematics of fig. 5 (c) shows a part of the bypass which is mapped in fig. 5 (a). The  white arrows show at both figures 5 the signal propagation  direction of the bypass. The red arrows in the figures are  related to a multiplexer and a buffer. Especially larger buffers  on the bypass chain show strong lock-in phase signal  consequently it was therefore no great problem to map the  complete bypass with support of the layouts net list. Especially at the shown schematics can be seen that many  alternative forks and paths are existent. Normally it requires  digital simulation to decide which path through the  multiplexers is really used.


Figure 5: Lock-in phase signal overlaid with pattern image is  shown. Correlated nets of the bypass path are red colorized


(a) Corresponding schematics is shown (b)


For failure analysis it is important to know if e.g. a spot or fail  is related to such a chain like structure. In order to get this  information design support is required. With the shown  method path information can be fast measured independently  from the load of the design groups. Alternatively, with very  expensive and therefore not at all FA labs available backside  probing tools like LVP or TRE hundreds of buffers must be  measured in order to achieve the same result. Therefore this  feasibility case study shows the power of lock-in phase  technique as global localization facility.


Figure 6: Jitter on a failing output is shown at oscilloscope  trace with time scale of 2 ns (a) Output signal overlaid  additional  frequency component  of 28 MHz is shown at the  spectrum


Case study 5: Global localization of jitter path  due to spectral line mapping


A device manufactured with an 90nm technology shows at a  required output signal with 200 MHz a jitter of several 100 ps  which is shown at figure 6 (a).  In this case, no signal without  jitter can be used as reference signal for lock-in phase  detection. In order to localize the jitter origin, the jitter  variation must be used for the monitoring in SDL method. Due to careful analysis of the signal spectrum an additional   frequency component of 28 MHz was observed as shown in  fig. 6.  In order to perform a global localization the amplitude  of 28 MHz spectral line was used for TLS as shown in figure


1. To achieve a sufficient spectral signal for the spectrum  analyzer the output signal was pre amplified with a self  designed and built 28 MHz band pass. A reference signal like  lock-in technique was not direct available and not required. The spectrum analyzer provides an analog voltage which is  correlated to the selected spectral line amplitude. The result of  spectral line mapping is shown as grey image at figure 7.  Nets  which are related to the spectral amplitude signal are overlaid. The block which is related to that jitter problem could be  successful localized with that spectral line mapping technique. With other probing techniques like micro-probing on backside  FIB pads and TRE measurements the result of global spectral  localization could be confirmed.


Figure 7: Result of spectral mapping of the amplitude of only  one spectral line from spectrum analyzer and overlay with  relevant layout elements was performed (jitter path)


Conclusions and Outlook


An introduction to TLS lock-in phase/amplitude technique  with pulsed Laser was performed with SEI imaging and the  relation to connectivity and junction material contrast was  considered. Furthermore, the lock-in phase technique utilizing  internal/external  periodic chip signals was shown. Constrains  and potential for advanced localization of lock-in phase  technique was shown e.g. at soft-defect analysis. The  advanced sensitivity of lock-in phase technique was  demonstrated at a feasibility study with bypass path mapping. An additional spectral sensitive technique was shown at an  advanced jitter problem.


In the last years several timing and delay sensitivity  techniques were introduced. Time recovery units as detector  are very sensitive to frequency changes but flop at low signal  level as well as simple frequency counting techniques. As  shown spectral techniques have the advantage that they do not  need a stable reference signal and the expense to generate one  is not required. The universality and power of lock-in  technique and the unique sensitivity especially at noise and  low amplitude signals as encounter in modern analog part of  mixed signal devices is singular in failure analysis.


[1] R.A. Falk, “Advanced LIVA/TIVA techniques” , ISTFA  2001


[2] K. Nikawa et al., “New Capabilities of OBIRCH Method  for Fault Localization and Defect Detection,” Proc. of  Sixth Asian Test Symposium, pp. 219-219, (1997)


[3] Z. Qian et al., “Precise defect localization of scan logic  failures by thermal laser stimulation (TLS)”, ISTFA, 517-520 (2004)


[4] C. Burmer et al., “Fault Localization of a Scan Shift  Problem on Integrated Logic Designs”, ISTFA, pp. 384-390 (2003)


[5] E.I. Cole Jr. et al., “Resistive Interconnect Localization”, ISTFA,43-50 (2001)


[6] M.R. Bruce et al., “Soft Defect Localization (SDL)”, ISTFA, 21-27 (2002)


[7] F. Beaudoin  et al., “Laser Stimulation Applied to  Dynamic IC Diagnostics”, ISTFA, 371-377 (2003)


[8] K. Sanchez et al., “Dynamic Laser Delay Variation  Mapping (DVM) and Applications”, ISTFA, 106-114, (2005)


[9] F. Beaudoin et al., “Lock-In Amplification Applied to  Thermal Laser Stimulation”,  2nd European Workshop on  Photonics Failure Analysis, Munich (2002)


[10] Z. Qian et al. “LIA-SDL and its Application in Scan-shift  problems”, ISTFA 2005


[11] F. Beaudoin et. al., “Principles of Thermal Laser  Stimulation Techniques”, ISTFA 2005, pp. 417-425


Localization of Cu/Low-k Interconnect Reliability Defects by   Pulsed Laser Induced Technique


T.L. Tan 1, A.C.T. Quah 2, C.L. Gan 1, J.C.H. Phang 2, 3, C.M. Chua 3, C.M. Ng 4 and A.-Y. Du 5


1School of Materials Science and Engineering, Nanyang Technological University, Singapore


2Centre for Integrated Circuit Failure Analysis and Reliability (CICFAR), National University of Singapore  3SEMICAPS Pte Ltd, Singapore  4Chartered Semiconductor Manufacturing Ltd, Singapore  5Institute of Microelectronics (IME), Singapore  E-mail: tant0030@ntu.edu.sg


In this paper, the application of pulsed-TIVA for the  localization of Cu/low-k interconnect reliability defects in  comb test structures is described. Two types of subtle  dielectric defects which are otherwise not detectable with  conventional TIVA can be detected with pulsed-TIVA.


The advent of low-k and ultra low-k dielectrics has improved  the performance of advanced integrated circuits (IC) by  reducing the capacitance component of the interconnect RC  delay. However, interconnect scaling, together with the poorer  thermo-mechanical properties of low-k dielectrics compared  to the traditionally used SiO2, have amplified the reliability  concern for Cu/low-k interconnects [1, 2]. Hence, there is a  need to investigate the factors leading to current leakage and  subsequent dielectric breakdown to predict the IC operational  lifetime more accurately as well as identify weak points in the  advanced interconnect systems.


Voltage ramp (V-ramp) and constant voltage time dependent  dielectric breakdown (TDDB) tests on large comb structures  are widely used to characterize the reliability of low-k  dielectrics. The electrical stress often results in huge burn  marks which can be easily observed under an optical  microscope. However, these failure sites usually indicate  completely destructed Cu lines and dielectric, leaving little  evidence for failure analysis [3]. On the other hand, defect  localization on stressed samples without burn marks is  difficult and time consuming due to the large comb structure  area (~10-3 cm2) compared to the much smaller failure analysis  area for cross-sectional SEM or TEM (~10-8 cm2). One viable  approach to counter this problem is by using an improved test  structure specifically designed for TEM analysis [4]. This  design constrains the failure to a specific region at which the  TEM cross-section could be performed directly.


Another approach is to use laser induced fault localization  techniques for defect localization. These techniques use a  scanned near infrared laser beam in a scanning optical  microscope (SOM) to stimulate failures which are sensitive to  thermal stimulation. They are effective for localizing resistive  defects, electrical shorts or opens, and they can be categorized  as power alteration techniques or tester based techniques [5]. The power alteration techniques include Optical Beam  Induced Resistance Change (OBIRCH) and Thermally  Induced Voltage Alteration (TIVA), which are ac-coupled  detection systems, and Differential Resistance Measurement (DReM) which is a dc-coupled detection system [6]. Moreover, it has been shown that detection sensitivity can be  significantly enhanced by a gain factor of over 9 times with  the use of a pulsed laser with digital integration algorithm [7]. We have applied TIVA to localize the Cu/low-k interconnect  reliability defects. However, for standard comb structures, the  conventional laser induced detection systems are insensitive  for effective defect localization. Therefore, this paper  highlights the effectiveness of pulsed-TIVA with signal  integration algorithm for localization of Cu/low-k interconnect  failures. The enhanced detection sensitivity allows the  localization of two types of subtle dielectric defects which are  otherwise not detectable by conventional TIVA.


Test Structure and Electrical Stress


The test structure used for this study is a comb structure with  line-width/space of 0.18 m/0.18 m as shown in Fig. 1(a). The cross-section TEM image of the comb structure in Fig. 1(b) shows the copper (Cu) lines that are capped with a SiC  barrier layer on the top and enclosed by the Ta barrier at the  sidewall and bottom. The low-k dielectric is a carbon-doped  silicon oxide (SiOC) with a measured dielectric constant of


2.9. The structure was subjected to a voltage ramp at 150oC  with a compliance set at 10A. After electrical stress, no  defects were optically visible


Figure 1: (a) Cu/low-k dielectric comb structure with line  width/space of 0.18 m/0.18 m and total test area of 10-3  cm2 (b) Cross-section TEM image of the comb structure.


Sensitivity Comparison of TIVA & Pulsed-TIVA


The defects were then localized using pulsed-TIVA with  digital signal integration algorithm incorporated in  SEMICAPS SOM 1005. Finally, the localized defects were  examined by FIB/SEM and TEM cross-sections.


Fig. 2(a) shows the frontside TIVA image with the laser  scanned in parallel with the comb lines of comb sample A at  66 mW laser power. It shows a weak TIVA signal at the  circled defect location and a faint tail artifact at the right end  of the leakage site indicated by the arrow. Fig. 2(b) shows the  pulsed-TIVA image with the same laser power at 500 Hz  pulsing frequency with digital signal integration algorithm, which localizes the entire current leakage path caused by the  resistive short in the comb lines. The defect location appears  with the highest signal intensity along the leakage path. Fig. 2(c) shows the reflected image of the comb sample with  pulsed-TIVA signal overlaid in pseudo color. The three  images in Fig. 2 are formed from a montage of three separate  frame scans to cover the entire structure.


When the laser scans along the leakage path, heat is conducted  quickly to the rest of the structure from the laser spot. Thus, as  its temperature increases towards steady state, the change in  resistance of the shorted Cu lines gradually decays. This  converts to slow laser induced voltage change under constant  current sourcing. It is attenuated by the ac-coupling input of  TIVA detection system acting as a high pass filter. Thus, the  leakage path could not be effectively localized. On the other  hand, pulsed-TIVA amplifies and modulates the laser induced  transient response with a pulsed laser at 50% duty cycle. The  integration algorithm further accumulates the laser induced


response in each laser pulse pixel by pixel, eliminating the  tailing artifacts in ac-coupled detection mode. This enhances  the detection sensitivity by increasing the signal intensity as  shown by the vertical line profiles across the circled defect for  TIVA and pulsed-TIVA in Fig. 2(d). Therefore, at the same  laser power and biasing conditions, pulsed-TIVA is  significantly more sensitive than conventional TIVA.


(a) TIVA image


(b) Pulsed-TIVA image


(c) Pulsed-TIVA overlay


(d) Vertical line profile


Figure 2: (a) Frontside TIVA image of comb sample A at  66mW laser power (b) Pulsed-TIVA signal image at 66mW  laser power and pulsing frequency of 500Hz. (c) Reflected  and pulsed-TIVA overlay image of comb sample A. (d) TIVA  and pulsed-TIVA vertical line profiles across defect site.


(c) Reflected – Pulsed-TIVA overlay image


(d) Horizontal line profile


Figure 3: (a) Frontside TIVA image of comb sample B at  66mW laser power (b) Pulsed-TIVA image at 66mW laser  power and pulsing frequency of 500Hz (c) Reflected – pulsed-TIVA overlay image of comb sample B.(d) TIVA and pulsed-TIVA horizontal line profiles across defect site.  Defect localization of comb sample B was done with the laser  scanning perpendicular to the comb lines. Although the TIVA  signal image in Fig. 3(a) reveals a faint leakage path, it is not  sufficiently sensitive to detect the actual defect site. However, the pulsed-TIVA image in Fig. 3(b) shows the leakage path  and the defect can be clearly identified. The location of the  defect site is then revealed from the reflected – pulsed-TIVA  overlay image in Fig. 3(c). The horizontal line profiles across  the defect shown in Fig. 3(d) further exemplify the significant  enhancement in signal intensity with pulsed-TIVA compared


to the normal TIVA. Moreover, these results show that the  enhanced sensitivity of pulsed-TIVA in defect localization is  independent of scan orientation.


Physical Failure Analysis Results


From the several comb samples examined by pulsed-TIVA, two main types of Cu/low-k interconnect reliability defects  were observed. They are dielectric cracking from the top  corners of Cu lines and intra-metal dielectric breakdown. For  comb sample A, a progressive series of FIB cross-section cuts  were performed near the localized defect beginning from the  right as shown by the arrow in Fig. 4. The cross-sections at  the defect were then imaged with a SEM at locations AA’, BB’ and CC’.


Figure 4: Frontside reflected and pulsed-TIVA overlay  image of comb sample A indicating the cross-sectioned sites.


(a) SEM cross-section at AA’


(b) SEM cross-section at BB’


Figure 5: (a) SEM cross-section image at AA’ displaying  dielectric crack paths from Cu top corners and (b) at BB’ illustrating Cu extrusion through the crack paths.


The SEM cross-section images captured at AA’ and BB’ are  shown in Fig. 5(a) and (b). In Fig. 5(a), crack paths through  the dielectric are found at the top corners of the Cu lines. At


location BB’ where the pulsed-TIVA signal intensity is the  highest, an additional Cu extrusion along the crack path is  observed as shown in Fig. 5(b). A similar failure mode has  been reported in reference [8], whereby the crack paths and  Cu extrusion are believed to be due to mechanical forces  exerted from electrostatic attraction between the comb fingers  during the electrical stress. The initiation of these crack paths  are expected to be assisted by the high stress concentration  near the Cu corners, generated by thermal expansion  mismatch of Cu, Ta barrier, SiC cap and low-k dielectric  materials during wafer processing [9].


0 200 400 600 800


S i


E lectron  beam  position (A .U .)


C u trace


C u


D ie lectric


T a


Figure 6: (a) SEM and (b) TEM cross-section image at CC’ illustrating dielectric breakdown of the dielectric cap and  low-k dielectric. (c) STEM-EDX line profile taken along the  dotted line illustrating random Cu traces in the dielectric  region.


From cross-section line CC’, dielectric breakdown of the  dielectric cap barrier and the intra-metal low-k dielectric is  observed as shown in Fig. 6(a). The corresponding TEM  image in Fig. 6(b) shows that the breakdown occurred  between the upper regions of the Cu lines with random Cu  traces in the breakdown region indicated by the STEM-EDX  line profile in Fig. 6(c). This is in agreement with reports on  the weakest link in the Cu interconnect, which states that the  CMP interface (i.e. Cu/SiC interface) region experiences the  highest leakage and electric field and thus it is the most  probable failure region [10, 11]. The Cu traces could originate


from the Cu extrusions or were present at the CMP interface  prior to the dielectric breakdown.


Figure 7: TEM cross-section of another failing comb sample  displaying a combination of dielectric stack burn and  dielectric cracking through the Cu top corners.


Fig. 7 shows the TEM image of the localized defect from  another comb sample with similar pulsed-TIVA signals as  comb sample A and B. It reveals a combination of the intrametal dielectric breakdown and dielectric cracking through the  top corners of Cu lines. Since the defects that were localized  from the comb samples by pulsed-TIVA are similar defects  reported in the literature, the defects are not likely to be  caused by the laser stimulation.


Figure 8: (a) & (b) Pulsed-TIVA overlay images of comb  sample C with three distinct defective spots.


In addition, three distinct defective spots were localized in  comb sample C as shown in the reflected – pulsed-TIVA  overlay images in Fig. 8. Fig. 8(a) shows only the overlay  result of the selected area. Fig. 9 shows the FIB/SEM crosssection image of spot 2 with the highest signal intensity. A  dielectric stack breakdown failure which is similar to the  previous samples is observed. However, spot 1 and spot 3  with lower signal intensities display a different defect. Their  SEM cross-section images in Fig. 10(a) and 10(c) show  dielectric voiding on the sidewall of the Cu interconnect. The  corresponding TEM images in Fig. 10(b) and 10(d) further  reveal metal out-diffusion at the sidewall. We believe that  these are process related defects as they were developed at the  ends of the comb structure which experienced the weakest  electric field. Thus, they are not likely reliability failures


caused by the voltage ramp. Nevertheless, further analysis  could be done to verify the cause of this kind of process  defect.


Figure 9: SEM cross-sections images of defect at spot 2.


Figure 10: (a) SEM and (b) TEM cross-section images of  spot 1. (c) SEM and (d) TEM cross-section images of spot 3  showing metal out-diffusion.


Pulsed-TIVA with signal integration algorithm has effectively  localized Cu/low-k interconnect reliability defects which are  optically not visible and are otherwise not detectable with  conventional TIVA. The defects observed from the localized  sites are similar to failures reported in the literature and are  thus not due to laser induced damage. As a result, the use of  pulsed-TIVA could be further extended to localize subtle  Cu/low-k defects in comb structures, which are stressed under  constant voltage (TDDB tests) as well as stressed at different  test temperatures. From the subtle failures observed in the  interconnect system, we can then further understand the  factors causing the leakage and dielectric breakdown in the  Cu/low-k interconnects.


T.L. Tan and A.C.T. Quah would like to acknowledge the  research scholarships from Nanyang Technological University  and National University of Singapore, respectively, and a  grant from Chartered Semiconductor Manufacturing  Postgraduate Sub 90nm Project Development Programme.


[1] M. Morgen, E.T. Ryan, J.-H. Zhao, C. Hu, T. Cho and  P.S. Ho, “Low dielectric constant materials for ULSI  interconnects”, Annu. Rev. Mater. Sci., 2000, pp. 645.


[2] R. Tsu, J.W. McPherson and W.R. McKee, “Leakage and  breakdown reliability issues associated with low-k  dielectrics in a dual-damascene Cu process”, Proc. Intl. Reliability Phys. Symp. (IRPS), 2000, pp. 348.


[3] T.L. Tan, N. Hwang and C.L. Gan, “Bi-modal dielectric  breakdown failure mechanisms in Cu/SiOC low-k  interconnect system”, IEEE Transactions on Device and  Materials Reliability, vol. 7, (2007).


[4] T.L. Tan, C.L. Gan, A.-Y. Du, C.K. Cheng, C.M. Ng and  L. Chan, “Test structure design for precise understanding  of Cu/low-k dielectric reliability”, Proc. Intl. Reliability  Phys. Symp. (IRPS), 2007, pp. 632.


[5] J.C.H. Phang, D.S.H. Chan, M. Palaniappan, J.M. Chin, B. Davis, M. Bruce, J. Wilcox, G. Gilfeather, C.M. Chua, L.S. Koh, H.Y. Ng and S.H. Tan, “A review of laser  induced techniques for microelectronic failure analysis”, Proc. Intl. Symp. Physical & Failure Analysis of  Integrated Circuits (IPFA), 2004, pp. 255.


[6] A.C.T. Quah, L.S. Koh, C.M. Chua, M. Palaniappan, J.M. Chin and J.C.H. Phang, "DC-coupled laser induced  detection system for fault localization in microelectronic  failure analysis", Proc. Intl. Symp. Physical & Failure  Analysis of Integrated Circuits (IPFA), 2006, pp. 327.


[7] A.C.T. Quah, L.S. Koh, S.H. Tan, C.M. Chua and J.C.H. Phang, “Enhanced detection sensitivity with pulsed laser  digital signal integration algorithm”, Proc. Intl. Symp. Testing & Failure Analysis (ISTFA), 2006, pp. 234.


[8] G.B. Alers, K. Jow, R. Shaviv, G. Kooi and G.W. Ray, “Interlevel dielectric failures in Cu/low-k structures”, IEEE Transactions on Device and Materials Reliability, vol. 4, (2004), pp. 148.


[9] E.S. Ege and Y.-L. Shen, “Thermomechanical response  and stress analysis of copper interconnects”, J. Electronic  Materials, vol. 32, (2003), pp. 1000.


[10] J. Noguchi, T. Saito, H. Maruyama, M. Kubo, N. Ohashi  and K. Takeda, “Dependence of time-dependent dielectric  breakdown lifetime on the structure in Cu metallization”, Japanese J. Appl. Phys., vol. 43, (2004), pp. 7405.


At a typically lock-in TLS application with laser modulation  the reference phase is kept constant and the in-phase  component X is optimized to a certain test structure to get best  signal noise ratio. Unfortunately such an optimization is valid  only for the used test structure. At other structures sensitivity  loss can occur due to significant out of phase signal  components. Normally lock-in TLS signal is detected directly  with the lock-in amplifier or with use of a preamplifier with  narrow bandwidth around the laser modulation frequency f. Analog lock-in amplifier provide usually the in-phase and  quadrature component X,Y whereas modern digital lock-in  amplifier with two built in mixers can provide simultaneously  the lock-in amplitude and phase. At the following case studies  always the TLS phase P and the amplitude R mode are used. A comparison between lock-in phase and amplitude was  performed at a test structure containing a tungsten (W) via  chain realized with two metal layers of aluminum (Al). In  figure 2 the lock-in Seebeck signal of this test structure is  imaged separately in phase (a) and in amplitude (b). The laser  modulation frequency is selected to be sensitive to the top  metal layers Al-W junction and to reduce the possible effect  of the bottom metal layer with the inverse W-Al junction. The  images show clearly that there is a strong contrast difference  between the lock-in phase image and amplitude image. At  each top metal bar with only two single contacts a strong  black and white contrast in phase signal is observed, whereas  the amplitude signal shows a minor contrast. The generated  Seebeck voltage dV at a AL-W junction due to thermal  stimulation with the temperature difference of dT is given by   dV = (Q_AL –Q_W)*dT,


with the thermoelectrical power of  aluminium Q_Al (-3.4  uV/K) and tungsten Q_W (+3.6 uV/K) [11]. The lock-in  amplitude R of the via chain at the bottom metal plate is  dominated by the junction specific material term |Q_AL-Q_W| which is identical in the absolute value at both AL-W and WAL junctions on each of the top metal layer plate.  Laser  induced temperature variation dT is assumed as identical at  both junctions due to the symmetric via chain construction and  same scan and local absorption properties of the laser beam. The phase signal carries at this example the expected signal  inversion due to the different interfaces W-Al and AL-W at  each top metal layer plate. Therefore this example shows that  the separate consideration of lock-in amplitude and phase  provides mainly information on pure material properties of the  specific junction undisturbed from the local connection. The  phase information however maps the local connection  properties at the considered junction. Consequently for failure  analysis a better observation of material and connection


properties can be achieved especially if changes in material  and connection are located  close to each other.


Figure 2: Comparison at via chain of TLS lock-in phase (a) and amplitude (b) with pattern image (d) Line cross-section  through phase image: arrows mark center of two contacts on  top metal plate with different phase (c)


Case study 2: Lock-in phase at 65 nm ring  oscillator


The first case study for application of phase related lock-in  technique to a single device output signal will be a ring   oscillator structure in 65 nm technology. The oscillator  consists of 48 NAND logic gates with load. The ringoscillator generates a self generated and divided by 1024  signal frequency of ~ 164 kHz at an output pin. Therefore  internal signal oscillation frequency is around ~ 167 MHz. An  input or stimulation signal is not accessible therefore the  output signal itself is used as lock-in reference. The chip is  backside decapsulated and has a die thickness of 300 um. Laser scan with cw 1.3um laser and slow scan speed about ~ 572 sec per image was performed. High NA 50x lens with  thickness correction is used. The result of phase and amplitude  imaging of the ring oscillator is shown at fig. 3. The  considered oscillator chain at all images is marked with an  arrow. The lock-in phase image shows a fine structured image  of the complete oscillator chain with high signal noise ratio. In  the amplitude image at the location of the chain only a much  weaker unstructured background signal could be observed  with four times higher laser power as the comparable phase  image. Interpretation of such small signal in combination with  the outstanding lock-in sensitivity is difficult and can also be


effected due to back draw over the device supply connection. In digital dominated chip circuits, frequently the amplitude  information is lost due to amplitude decoupling with inverters  or buffers. The phase carries information about delay and can  be used for mapping of the functional parts of this oscillator  chain. The phase variation inside the chain can be related to  the different parts of the sub elements. Due to construction of  a load and NAND part all single elements could be good  resolved and show same local lock-in phase variation.


Analysis background of this case study was increased  current consumption on the ring oscillator domain. Functionality of all cells could be shown with phase imaging  and confirmed additionally that the current consumption  problem was not directly related to the oscillator. This  example demonstrates obviously the general utilization of  lock-in phase technique for analysis of frequency or delay  related problems.


Figure 3: Comparison at 65 nm technology: (a) Lock-in phase  image (b) Lock-in amplitude image. Pattern image is shown  as inset. Horizontal lines are disturbances due to laser  interaction with neighborhood circuits.


[11]V.C. Ngwan, C. Zhu and A. Krishnamoorthy, “Analysis  of leakage mechanisms and leakage pathways in intralevel Cu interconnects”, Proc. Intl. Reliability Phys. Symp. (IRPS), 2004, pp. 571.


Ultra Low Voltage Probing on 45 nm CMOS by   Time Resolved Emission (TRE) Technology


Chi-Lin (Kenny) Young, Paul Ng, Francisco Contreras


Intel Corporation, Santa Clara, CA, USA


Radu Ispasoiu, Jim Vickers, Dan Cotton, Chris Shaw


Credence Corporation, Sunnyvale, CA, USA


Ultra low voltage probing by TRE technology below 1.0V is very  challenging for Micro-processor debug in practical operation  condition. This is because the photo-emission rate reduces  exponentially as the power supply voltage (Vcc) decreases. In this  paper, a new technology with improved detector in Solid  Immersion Lens (SIL) TRE system was demonstrated for low  voltage and small node probing. This technology improves the  photon collection efficiency and lowers the dark noise to 8 KHz  with advance InP/InGaAs Avalanche Photo Diode (APD). The  performance gain of acquisition time reduction was shown on  45nm CMOS processor.


Optical probing has proven to be critical in the design debug  since the 0.25um process technology [1, 2]. Driven by  Moore’s law, a new process technology can be rolled out in  about every 24 months in the leading edge industry. To meet  the challenge of optical probing for smaller geometries due to  device shrinking, a critical innovation of SIL had been  developed for high resolution optical probing of advanced  microprocessor [3]. A numerical aperture (NA) value of 2.45  is achieved by direct silicon to die surface contact (Figure 1) to increase the through-silicon optical resolution to 0.25um  and optical collection efficiency to 3X compared to the Liquid  Immersion Objective (LIO) [4].


Figure 1: Solid Immersion Lens


TRE Technology is based on the hot carrier emission effects in  FETs [5]. An inversion layer is created with biased gate voltage. Then, the current is conducted with applied source to drain voltage. Under saturation conditions where the carrier can be accelerated in  very high speed in the so called Pinch-off region, the carriers can  emit photons.  TRE system detects these photon through a nearinfrared optimized InGaAs based Avalanche Photo Diode (APD) and displays the timing information similar to an oscilloscope.  For  debug application in probing a sub-micron device with bias voltage  below 1.0V, the dynamic emission based probing method becomes  much challenged. One reason is the less photon emission from  smaller device, and the other is that the light emission intensity  decreases exponentially against the reciprocal of the power supply  voltage (Vcc) [6].


For very weak signal detection, the lowering of system  detecting noise is the most effective way to get a good quality  of signal to noise ratio (S/N). Figure 2 illustrates the  simulation result based on one photon count of TRE probing; one photon event is detected at most for one test pattern  looping. The single event can be either signal or noise  depending on the probability of photon emission competing  with the noise rate. Assuming the same signal strength, figure  2(a) shows the TRE waveform for current detector (25KHz  dark noise) and 2(b) for new low noise detector (8KHz dark  noise).


Figure 2 (a): Simulated TRE waveform in noise environment  of 25 KHz


Figure 2 (b): Simulated TRE waveform in noise environment  of 8 KHz


In this paper, an improved detecting scheme was developed to  collect 30% more Photon Detection Efficiency (PDE) than  previous system. The APD with lower cooling temperature is  used as the LED source for fiber placement to allow removal  of fiber switch (Figure 3).


Figure 3 InGaAs/InP APD and used as LED for fiber  alignment


The APD bias controls the operating point to adjust detector  Jitter (TJ) and dark count rate (DCR). Higher bias produces  lower TJ and higher PDE but higher DCR, and lower bias  produces lower DCR but higher TJ and lower PDE. Further  detector temperature cooling results in the lower DCR of 8  KHz in low noise mode, and 15 KHz in the low jitter mode. Figure 4 shows the detecting time of achieving certain signal  to noise ratio versus the detector excess bias.


4 5 6 7 8 9 10 11 12 13 14 15


0.15


0.35


0.45


0.55


Low Jitter Mode:


DCR = 15,000 cps TJ = 52ps


PDE ≥ 60%


% Excess bias


Low Noise Mode:


DCR = 8,000 cps TJ = 65ps


PDE ≥ 50%


Figure 4 InGaAs/InP APD operation in two modes: Low  Noise and Low Jitter Mode


The performance gain definition is the acquisition time reduction  for achieving a given signal to noise ratio. The detecting emission  from a CMOS transistor, S and N are given by the following  expressions:


a c q


si g


l oop


a c q l oop


DCR


TJ


Where: Tacq is the acquisition time, Tloop is the loop duration, Rsig is the certain probability per tester loop pf detecting a  useful signal event, and DCR is the dark count rate.


The signal to noise ratio is given by:


S N


σ =


Plugging (1) into eqn. (2), and then solving for Tacq yields:


DCR TJ


⎛


⎞


⎛ ⎞


⎜


⎟


⎜ ⎟ ⎜


∆


⎝ ⎠ ⎝


⎠


In the case of strong signals, eqn. (3) can be approximated as:


s i g


⎜ ⎟∆⎝ ⎠


Thus, the performance gain is due to the collection efficiency  improvement (30%) of this detector.


For the weak signal or dark noise dominated regime, (3) can  be simplified as:


d e t


Therefore, the acquisition time reduction is mainly contributed by  the lower dark noise of 8 KHz as compared to 25 KHz of current  detector. The performance gain can achieve 3X for this signal  strength regime.


The performance gain of low noise 8 KHz detector (Phase II) versus the current 25 KHz (P-Spec) detector is compared in  two different signal strength domains: strong and weak signal  regimes. Figure 5 shows the waveform and S/N ratio  comparison for two different detectors at 1.1V (strong signal  regime).


Phase II (Low Jitter mode)


P-Spec


Figure 5 TRE waveforms and S/N ratio comparison for two  different detectors at 1.1V


In the weak signal domain, we compare the performance using a  very small single leg transistor (N) of 0.53um in 150us loop at 0.8  and 0.75V. Figure 6 (a) shows the waveforms acquired at 0.8V  from both detectors for different acquisition time. It’s very obvious  that the signal is easier to be detected by Phase II detector in 30-60  minute due to much less noise environment. However, for the PSpec one, the noise can only be averaged out after about 3 hour  acquisition.  Figure 6 (b) summarizes the S/N calculation for two  detectors. This is an extremely test case of one leg transistor. In  normal situation, the acquisition time can be improved 3-4X for  two leg and 5-9X for three leg transistors for both detectors.


Performance gain > 2~2.5X


30min 60min


60min


30min 90min


90min


120min


150min


180min


180min 210min 240min


Phase II


Figure 6 (a) shows the waveforms acquired at 0.8V from both  detectors for different acquisition time


0 1 2 3 4 5 6


60 90 120 150 180 210 240 270


Acqisition Time (min)


P-Spec Phase II


Figure 6 (b) Summarized S/N calculations for different  acquisition time for two detector comparison at 0.8V


Figure 7 shows the waveforms acquired from both detectors  and summarized S/N calculation. The performance gain is  increased when the signal strength is smaller. Again, this is an  extreme test case of one leg transistor. In normal situation, the  acquisition time can be improved 3-4X for two leg and 5-9X  for three leg transistors for both detectors.


Phase II (Low Noise mode), 2hr (S/N=2.8)


P-Spec, 6hr


(S/N=2.1)


3.5 4


Acqisition time (min)


Figure 7 Waveforms acquired from both detectors and  summarized S/N for different acquisition time at 0.75V


45nm devices show much stronger photo emission strength  compared to 65nm at a given voltage. In general, this is due to  the device scaling effect which builds up higher electrical  field accelerating the carriers (electron and hole) in saturation  region. Moreover, the combination of high-k dielectrics plus  metal gate electrodes on Intel’s 45nm transistors provides  significant performance gain in drive current and in sourcedrain leakage current reduction. Hence, process  scaling/channel length shrink is in favor of photon emission  based technology.


TRE has proven as a non invasive backside optical probing tool for  practical sub micron circuit device speed path debug. In this paper, the SIL TRE with low dark noise detector technology has been


successfully applied to optical probing for 45nm product debug.


The performance gain improvement in strong and weak signal


regime has been demonstrated against the current detector


technology. It has also demonstrated the capability on probing the  ultra low voltage at 0.75V for sub micron node of 45nm process. The authors would like to thank Intel team, Son Duong & Lee


Tran, for all the lab support. For product test case, we also like to  thank the support from Hubert Hsieh and Gila Yampolski. The


authors would like to acknowledge Travis Eiles for his technical


consultation.


[1] T.M. Eiles, G.L. Woods, and V.R. Rao, IEEE ISSCC  2000


[2] Travis Eiles, Patrick Pardy, “Liquid Immersion Objective  for High-Resolution Optical Probing of Advanced  Microprocessors”, ISTFA 2001


[3] James Vickers, et. Al., “Time-Resolved Photon Counting  System based on a Geiger-Mode InGaAs/InP APD and a  Solid Immersion Lens”, IEEE 2003


[4] E.B. Vaner, C.L. Young, H.M. Ng, Steven Maher, Travis  Eiles, Birk Lee, “Single Element Time Resolved  Emission Probing for Practical Microprocessor  Diagnostic Application, ISTFA 2002


[5] James Tsang, et. Al., “Time-Resolved Optical  Characterization of Electrical Activity in Integrated  Circuits”, Proceedings of IEEE, Vol. 88, 2000


[6] Stefan Rusu, et Al, “Backside Infrared Probing for Static  Voltage Drop and Dynamic Timing Measurement”, 2001  ISSCC


Masking Technique to Enable Multiple Site Defect Analysis on a Microchip


James Hahn


Altera Corporation, San Jose, CA, USA   jhahn@altera.com


As feature sizes are shrinking beyond 130nm, new subsets of  failures are coming to light.  These failures are more  systematic, marginal, and DFM (Design for  Manufacturability) related.  Multiple site defect analysis with  adjacent block comparisons and multiple site comparative  nanoprobing have become mandatory for these extraordinary  and non-visible defects.


There are instances where inspection or analysis will be  required at multiple sites over a wide area on a sample.  Traditional mechanical deprocessing techniques do not allow  us to maintain planarity over a relatively large area, typically  tens of microns (figure 1).


This requires the analyst to perform several iterations of  deprocessing not only to allow inspection at each  metallization layer but with the added complexity of having to  monitor multiple sites.  I.e. The analyst may have exposed  metal-4 near the edge of the die while having only reached  metal-7 at the center.  Having to monitor multiple sites at  different levels of deprocessing can become quite challenging  and time consuming.  The following ‘masking technique’ does  not necessarily address the issue of level planarization over a  large area but rather ‘adjusting’ the level at several local sites.  This enables analysis and, in our case described below, nanoprobing on multiple devices widely distributed over a  single sample.  Nanoprobing has proven to be an invaluable  tool for device characterization and failure analysis on  advanced technologies.


Our work required electrical characterization of numerous  transistors scattered over a large area (in semiconductor terms) on a 65nm test chip.  We were required to deprocess the  sample to the contact level at 3 groups of devices for the  purpose of nanoprobing.  Since nanoprobing is not currently  available in house, we were offered the services through our  foundry in Asia.  It was logistically prohibitive to ship the  sample back and forth overseas to complete this time critical  task; hence the motivation to develop a procedure to expose  all 3 groups at once.


Figure 1: Micrographs show unevenness of layer removal by  conventional parallel lapping technique (more pronounced at  the sample’s edges).


Methods and Results


A technique was developed that enables uniform multiple site  exposure on a microchip.


All sites of interest are physically located on the sample and  laser marked for future identification.  The sample is adhered  to a heated metal lapping disc using a commercially available  hot mounting wax.  Mechanical deprocessing is employed to  expose the first site.  A thin layer of the same wax is then  applied over site 1 to protect it from further material removal


(the masking step).  At room temperature, the wax is solid and  resistant to the rigors of mechanical lapping.  Application is  ideally performed under a microscope with long working  distance lenses (figure 2).


Figure 2: Wax is applied to heated sample situated on the  metal disc under a microscope.


Having considerable mass, the lapping disc retains heat and  thus the wax remains workable for a significant amount of  time.  Without the disc, the wax cools and hardens in a matter  of seconds.  It melts at 120°C and is soluble in acetone, which  simplifies adjustment, correction of mistakes and clean-up.


Mechanical deprocessing continues to a second site.  The disc  and sample are reheated, the mask spread over the second site, deprocessing continues, and so on until all sites are equally  exposed.  All deprocessing is done concurrently, eliminating  the need for repeated deprocessing and imaging/probing steps. The following cross-sectional diagrams (figures 3a-3g) illustrate the masking technique to expose 3 sites on a die for  analysis.  The animation depicts up to metal-3 only.  It is not  to scale- only for illustrative purpose.  Actual sites requiring  analysis may span hundreds or even thousands of bits.  Figure  4a-4c shows the final result in plan view of our 65nm test chip  sample.


Figure 3a: Cross-sectional view of 3 sites.


Figure 3b: Sample is lapped to desired level (contact) for site


Figure 3c: Site 1 is masked to protect from further lapping.


Figure 3d: Lapping continued until site 2 is reached.


Figure 3e: Mask is spread over site 2 for protection.


Figure 3f: Lapping continued until site 3 is reached.


Figure 3g: Masking material (wax) removed in acetone.  All 3  sites deprocessed to desired level and ready for inspection or  nanoprobing.


Figure 4a: Illustration shows progression of wax coverage  over 3 groups of devices.


Figure 4b: Actual final results, after wax removal, showing 3  groups ready for inspection.


Advanced technologies bring their own set of challenges and  innovations.  The failure analyst does not have the luxury of a  large supply of material for analysis.  Silicon is expensive (test  and time limited).  This innovative masking technique can be  utilized at all deprocessing levels of defect analysis and  comparative circuit analysis and is time, tools and labor  efficient.  It allows multiple site defect analysis across a large  area without the need to commit a sample to repeated  deprocessing steps.  Additionally, it enables multiple site  nanoprobing, a preferred and essential tool for electrical  validation of non-visible failures at technologies 90nm and  beyond.


[1] M. Weldy, L. Serrano, “Increasing Planarity for Failure  Analysis Using Blocked Reactive Ion Etching Combined  with Planar Polish,” Proceedings of the 31st ISTFA  Conference, Nov. 2005, pp. 206-208.


ION BEAM IMAGING METHODOLOGY OF INVISIBLE METAL  UNDER INSULATOR USING HIGH ENERGY ELECTRON BEAM  CHARGING


C. H. Wang, S. P. Chang, C. F. Chang, J. Y. Chiou


6,Creation Rd. 2, Science-Based Industrial Park, Hsin-Chu, Taiwan 300, R. O. C.


Phone: 886(0)3-5636688Ext.7072181   Fax: 886(0)6-5787778   Email: jhwangf@tsmc.com


Focused ion beam (FIB) is a popular tool for physical  failure analysis (FA), especially for circuit repair. FIB is  especially useful on advanced technology where the FIB is  used to modify the circuit for new layout verification or  electrical measurement. The samples are prepared till  inter-metal dielectric (IMD), then a hole is dug or a metal is  deposited or oxide is deposited by FIB. A common  assumption is made that metal under oxide can not be seen  by FIB. But a metal ion image is desired for further action. Dual beam, FIB and Scanning Electron Microscope (SEM), tools have a special advantage. When switching back and  forth from SEM to FIB the observation has been made that  the metal lines can be imaged. The details of this technique  will be discussed below.


Circuit modification is an important skill for electrical  failure analysis (EFA) and physical failure analysis (PFA). If some layout or circuit issues are suspected and  verification is required at the package level circuit  modification by FIB can be made without any mask changes. The dual beam tool can make the changes required due to  the advantages of the SEM and the FIB. The advantages are  listed in Figure 1.


Figure 1. The comparison of ion beam and electron  beam


The primary electron beam of the SEM can pass through  the atomic/molecular structure to get an image of more than  the surface of the device if the electron energy is high  enough. Also surface charging, positively or negatively, of  the material can be controlled by the electron beam energy. The electron beam is not used for circuit edit as is the FIB. The advantages of the SEM in seeing underlying layers is  not available during FIB edit. The FIB image is only of the  device surface so it limited in its application to help see  underlying layers. Another problem exists when the FIB is  used for imaging. The FIB can damage the device surface in  the area of the region to be modified. Figure 2 gives an


example of the beam interaction for the FIB and the SEM.


Figure 2. The interactions of ion beam and electron  beam


For circuit modification, the surface insulator must  always remain intact to prevent shorting. The  electron beam  can see through the insulator but the ion beam can’t. The  two beams are never quite aligned so much time is spent  trying to align the two images.


Under the correct conditions when switching between  the ion and electron beam, the underlying metal can be seen. By using a high- energy electron to bump the sample then  quickly switching to the FIB some patterns under the  insulator show up. This phenomenon helps to accurately  localize where to  mill. Based on the material interaction of  the electron beam and ion beam a model can be infered to  describe why in some cases the metal under the insulator can  be seen. A few examples of  the use of this phenomenon will  be presented.


The model


The physics of electron and ion beam material  interaction is well known. According to the secondary  electron yield curve for different materials, low-energy  electrons make the sample surface charge positively and  high-energy electrons make the surface charge negatively. An ion beam bump of the sample will make the surface  charge positively just the same as a low-energy electron  beam. The ability of the surface to hold charge will depend  upon the amount of surface charge leakage to ground. The  ability for an underlying metal line to hold charge will  depend upon the grounding of the metal line. See Figure 3.


Figure 3. Comparison chart of the beam material  interaction for ion and electron beams


When a focused high-energy electron beam is used to


see the metal buried under oxide, a negative charge is


induced and deep in the oxide and metal. The negative


charge exists on the floating metal and oxide, but not on a


grounded metal line. By switching between the ion beam to


bump the surface some secondary electrons are produced.


The image of the insulator or floating metal is bright


because the negative charge is rejected. The detector


receives the additional electrons making the image bright at


that location, see Figure 4. Grounded metal does not react


the same way. The switch induces an the electric field


between the negative charged oxide and the un-charged


grounded metal. The field draws some secondary electrons


making the buried grounded metal image on the FIB appear


as a shadow.


(a)                                         (b)


(a) 30KeV E-beam image of probing pad and power lines


(b) 500pA ion beam image of probing pad and power lines


(c) The model of high energy electron beam bumping


(d) The model of ion beam imaging after high energy  electron beam bumping


Figure 4. The charging and imaging model for  grounded and un-grounded metal that is buried under  an insulator


Key points of ion beam image for buried grounded  metal


There are some key points for ion beam imaging by  electron beam charging. First, the insulator above the metal  can’t be so thick that high-energy electron can’t pass  through. To thick an insulator does not allow the electron  beam to penetrate. The un-ground metal will not change  thus there is no charging difference between floating and  grounded metal, no shadow image of buried grounded metal  shows up. See Figure 5.


Figure 5. the insulator is so thick that we can’t get the  image by high-energy electron beam


Second, the sample must be charged enough negatively  the high-energy electron beam to produce a differential  image. The surface must be exposed long enough for the  significant negative charge building up to make a difference  between floating and grounding metal. See Figure 6.


Figure 6. The charging difference is not enough with  short-time high-energy electron beam exposure.


Application for circuit modification


By using the methodology and key points discussed on  dual beam imaging circuit modification by FIB can be made  accurately without a layout navigator. First, some  passivation must be removed from above the top metal to let  to allow the technique to obtain a  top metal image by a  high- energy electron beam (30KeV). Then the target  area  exposed to the high-energy electron beam for a moment is  exposed to the ion beam. Although the top metal is still  under the oxide a clear image for FIB cutting can be  obtained. See Figure 7.


Figure 7. The target ion beam and electron beam  image.


After confirming the location using a low beam current  ion beam, the ion beam imaging method is really accurate. Then the oxide can be removed above the target metal till a  bright metal image appears on the FIB. See Figure 8.


Figure 8. Exposed target metal, ion beam image


In Figure 9. the target metal is has been exposed and a   metal pad has been deposited for a micrometer needle probe.


Figure 9. Pt pad for needle probe


The case described is simple but is enough to verify the  methodology presented works. Of course this methodology  has been applied to many circuit modification cases.


The spacing between metal interconnects in a  semiconductor device is becoming smaller and smaller. More skill is required with advanced tools to edit the new  devices efficiently. New tools for advanced technology can  not always be expected to solve the new problems. In the  case of the FIB it is still a powerful tool for EFA and PFA  when combined with the technique discussed. A model has  been presented that explains the phenomenon between  high-energy electron beam surface charging and ion beam  charging. The phenomenon was shown to work on a real  case. The implementation of the model presented shows that  by paying attention to every detail of a process old tools can  be used for new technologies.


[1] Ahmed, H.; “nanostructure fabrication”, Proceedings of the  IEEE Volume 79, issue 8, aug. 1991 pages:1140-1148


[2] Lipp, S.;Frey, L.;Lehrer, C.;Demm, E.;Pauthner, S.;Ryssel, H.; “A comparison of focused ion beam and electron beam  induced deposition processes”,Relability of electron devices,


Ion beam image (84pA)


electron beam image(30KeV)


failure physics and analysis, 1996. proceedings of the 7th  EDFAS,8-11 Oct. 1996 pages: 1779-1782.


[3]  Y. Mashiko, H. Morimoto, H. Koyama, s. Kawazu, T. Kaito, and T. Adachi, “ A new VLSI diagnsis technique: focused ion  beam assisted multi-level circuit probing,” Proceedings of  1987 international reliability physics symposium, 1987, pp. 111-117


[4] M. Abramo and R. Wasielewski ; “FIB for failure analysis” Semiconductor international, pp 133-134,Oct 1997.


A Case Study of Defects due to Process-Design Interaction   in Nano Scale Technology


Hung-Sung Lin, Ying-Chin Hou, Juimei Fu, Mong-Sheng Wu, Vincent Huang, Ching-Heng Chou, Jian-Chang Lin


United Microelectronics Corporation, Ltd.


No. 3, Li-Hsin Rd. II, Hsinchu Science Park, Taiwan 300, R.O.C.


Phone: 886-3-5782258 ext 33231 Fax:886-3-563-6722 Email:giant_lin@umc.com


The difficulties in identifying the precise defect location and  real leakage path is increasing as the integrated circuit design  and process have become more and more complicated in nano  scale technology node. Most of the defects causing chip  leakage are detectable with only one of the FA (Failure  Analysis) tools such as LCD (Liquid Crystal Detection) or  PEM (Photon Emission Microscope). However, due to  marginality of process-design interaction some defects are  often not detectable with only one FA tool [1][2]. This paper  present an example of an abnormal power consumption  process-design interaction related defect which could only be  detected with more advanced FA tools.


Recently, power dissipation has become an important  constraint in a design. In fact, power considerations have been  the ultimate design criteria in many battery-powered portable  applications such as laptop/notebook computers, electronic  organizers, etc. The objective in these applications is  minimum power for maximum battery life time. Thus, it is  important to optimize power for power saving. Some processdesign related defects will cause additional power dissipation  of digital systems even when operations or functions are  normal. However, these defects, due to marginality of  process-design interaction, are often not detectable. In this  paper, we demonstrate how a combination of advanced FA  tools enables us to find the real leakage path [3].


Case Study: SRAM Core Power Leakage


Photon Emission Analysis:


PEM is a very well known technique used for the localization  and characterization of silicon defects such as failures due to  current leakage. In this case, a PEM equipped with MCT (MerCad Telluride, HgCdTe) detector system was adopted to  detect leakage from backside of the chip caused by the  reduction of supply voltage and the great number of  interconnected layers. The reduction in supply voltage reduces  the number of hot electrons. The shift in hot electron energy  moves the emission spectra to near IR or low photon energy  range in small feature size technology. An infra-red


transmission coefficient for SiO2 is close to 1 in the  wavelength between 1000 and 5000 nm. However, it is not  necessarily true of high infra-red transmission coefficient for  some low-k materials in modern processes. As a result, a  MCT detector with high quantum efficiency in near-IR spectra  was used to detect photo emission from backside of the chip.


Figure 1: Illustration of backside PEM(a) and IR-OBIRCH(b) technique with a 100x objective.


Figure 2: Illustration of backside PEM technique at a 20x  objective for severial bias conditions.


The results were shown in Fig. 1. Photon emission was  observed at the decoding area of an SRAM instance. The  layout checking showed that the emission sites correspond  exclusively to PMOS transistors of an array of inverter


CMOS. Several bias conditions, as shown in Fig. 2 were  applied to collect photon emission. No emission was detected  when the voltage was lowered below 1.1V. It reduced the  possibility of photon emission caused by forward bias junction  conditions because a forward biased junction injected many  minority carriers and increased the recombination activity  already at low voltages to observability level.


Static Thermal Laser Stimulation Analysis:


IR-OBIRCH (InfraRed-Optical Beam Induced Resistance  CHange) with 1340nm wavelength was chosen to detect the  signals of current change derived from localized resistivity  changes. Red OBIRCH spots, as shown in Fig. 1, were  detected at the same place (PMOS transistors of an array of  inverter CMOS) as PEM.  With the OBIRCH method, the  current varies under a constant voltage according to the  relationship shown in the equation below:








0 0


R V


TCRα


:


I∆ current change due to laser heating


TCRα resistance temperature coefficient


T∆ temperature increase due to laser heating


V the constant voltage applied to the device


R the resistance at room temperature


From equation (1), it can be noted that the current change may  either be positive or negative depending on the materials that  the current pass through underneath the OBIRCH spot [4].


Table 1: Resistivity and temperature coefficient of several  materials.


A simple interpretation inspired by Table 1 is that white  contrast or red spots on superimposition means that the   anomalous current occurs predominantly in silicon. Fig. 3  shows that the current increases by about 10.5% with thermal  laser scanning at a 0.1V voltage supply. EFA (Electrical  Failure Analysis) results obtained from PEM and OBIRCH  implied that the leakage is possibly casued by front-end  related defects. Although one of the samples was physically  deprocessed, no physical defect was observed. Anyway,


additional analyses are needed to further understand the  electrical behavior and accurately pinpoint the defect location.


Figure 3: The current fluctuations are detected when scanning  laser is switched on.


Internal Probing Analysis:


An SEM based nanoprobing technique has been applied as a  suitable tool for the internal probing in a PMOS transistor of  an array of inverter CMOS circuits for electric measurements. The output characteristics and transfer characteristics of the  PMOS are shown in Fig. 4.


Figure 4: PMOS output characteristics (Ids versus Vds) (a) and transfer characteristics (Ids versus Vgs) (b) of an inverter  CMOS .


It can be observed that the velocity saturation effect converts  the Ids relation to Vgs from a square law to almost a linear  law according to the relationship shown in the equation (2) and (3).  As Fig. 4 shows, the slope of the saturated current  lines is larger; and, in addition, the appearance of beyond  saturation due to channel length modulation can also be  observed. The output resistance Rout due to channel length  modulation is an inverse proportion to IDsat according to the  relationship shown in the equation (4) and (5).


m V


V


L W


GS


ox


Dsat


=µ


) sat


WC


ν








 ∆


DS


sat


DS D


out


dV


E


dV dI


out I


saturation current


effµ effective mobility


W channel width


L channel length


C gate oxide capacitance  :


GSV gate to source voltage difference


TV threshold voltage


m a factor based on linear bulk charge analysis


satν saturation velocity :


outR the output resistance


I drain current


V drain to source voltage difference :


E electric field :


saturation drain current


L∆ channel length modulation


The other important IV characteristics extracted from the  transfer curve of the PMOS device is that the threshold  voltage Vt is less than 0.1V, which is much lower than our  specifications. As a matter of course, high Ioff current can also  be expected according to the relationship shown in the  equation (6). This was measured to be above 0.5 uA.


t T


S V


off I


= 10                                                                     (6) :


off


I the off-state leakage current


= ,


: :


S the subthreshold swing


High Ioff current can also be used to explain the phenomenon  of the photon emission and the red spots stimulated by static  thermal laser. Leakage currents in silicon are the classic PEM  application for failure localization. According to Noel C. de  Luna, for the n-channel device, the emission mechanism is  researched to be photon emission from hot electrons  undergoing direct transitions in the high field drain depletion  region. For the p-channel device, the emission mechanism is  researched to be photon emission by direct hot electron  transitions with a contribution from direct hot-hole transitions


[5]. So, we can explain the phenomenon of photon emission in  PMOS based on lucky electron model as below. The current  through the inversion channel of a MOS transistor in ohmic  state is low resistive and usually not accompanied by light  emission. Only after pinch off, in saturation, it passes an SCR  from pinch off point to drain. The light emission is  proportional to the substrate current. MOSFET luminescence  depend on two factors [6]: (1) the number of electrons flowing  through the MOSFET channel and (2) the probability of each


electron to emit a photon according to the relationship shown  in the equation (7), (8) and (9).


m





 −


λ


λφ


i


β


sub


,


E the maximum electric field :


the saturation voltage


λ the characteristic length


:α the impact ionization coefficient


n the concentration of lucky electrons


0n the number of electrons


iφ potential


E kinetic energy :λ mean free path


I the substrate current


According to our experiments, PMOS is in saturated region  conditions accompanied by high Ioff current. In other words, the output of the inverter is in the logical state “low” with the  high leakage channel current in PMOS. Saturated PMOS  conditions produce high electrical field intensity along the  channel and increase the probability of each carrier to emit a  photon. Higher Ioff current supply a sufficient number of  carriers flowing through the channel. For these reasons, though the chip is in a static operation mode, a photon  emission can be detected in the PMOS transistors. According  to the findings, the PMOS transistors of inverter CMOS were  affected by SCE (short channel effect) as well as by a lower Vt  and a significant increase in leakage current. The SCE is the  decrease of the threshold voltage of the MOSFET as the  channel length is reduced. The short channel effect must be  contained in a scaled CMOS to allow for reduced nominal  threshold voltage without significant increase in leakage  current and variation. The SCE is an important consideration  in designing a device. One must make sure that the Vt does  not become too low for the minimum-channel-length device. The physics of the short-channel effect can also be understood  by considering lowering the surface potential energy barrier  from source to drain. As the channel length is reduced, the  surface potential barrier as well as the Vt is also reduced. When a drain bias is applied to a short channel device, the  barrier and the Vt will be further reduced. In our case, Vt and  Ioff of PMOS transistors at SRAM decoder area seem not to be  well controlled in scaled CMOS due to certain process, design  or process-design interaction marginalities.


Cross-Sectional TEM Analysis:


Once the PMOS failing transistor is identified, a TEM sample  is prepared in order to understand the SCE behavior with an


excessive reduced threshold voltage and the channel leakage  current in the off state. The resultant TEM image reveals a  smaller poly CD (about 57nm), which is about 37.8% smaller  than the target. From the MOSFET scaling point of view, the  scaling down of the device will not give the same electrical  behavior as the original one, that is, the electrostatic potential  profile of a scaled PMOS is not identical to that of the original  device. In order to keep the electrostatic potential unchanged, the corresponding Poisson’s equation should remain  unchanged for the scaled device, that is, β=1 according to the  relationship shown in equation (10). In our case, the device  dimension, channel length L, is scaled by a factor 1/1.6. However, the doping concentration, Nd, in the substrate is not  scaled by a factor 1.62. That means the scaled PMOS’ Nd in  substrate is lower than the requirement. Based on the  relationship between the threshold voltage and Nd as shown in  equation (11), a lower Vt and a significant increase in leakage  current can be expected.


L ⋅


si


fb


tp


C qN


2 −


:β generalized scaling factor


N substrate doping :


V bias voltage


tpV PMOS threshold voltage


V flat-band voltage


nφ potential


siε permittivity of silicon :


N n  substrate doping


In this case, the defect caused by the process-design  marginality is not visible by SEM or FIB analysis, but is  easily explained by the electrical data.


In this paper, some advanced FA tools, which form  combinations to precisely pinpoint the real leakage path, are  successfully demonstrated. After identifying the process step  that failed and determining the defect types, corrective action  can be taken to quickly improve yield. In this study, an  efficient methodology for overcoming the difficulties in  detecting defects due to marginality of process-design  interaction was established.


[1] Hung-Sung Lin, Wen-Tung Chang, Chun-Lin Chen, Tsui-Hua Huang, Vivian Chiang, Chun-Ming Chen, “A


study of Asymmetrical Behaviour in Advanced Nano  SRAM Devices”, 13th IPFA Proceedings, Jul. 2006, pp. 63-66.


[2] Bram Kruseman, Ananta Majhi, Camelia Hora, Stefan  Eichenberger, Johan Meirlevede, “Systematic Defects in  Deep Sub-Micron Technologies”, ITC International Test  Conference, pp. 290-299, 2004.


[3] Hung-Sung Lin, Wen-Tung Chang, Chia-Hsing Chao, Jesse Wang, Chang-Tan Lin, and Coswin Lin, “Failure  Analysis of Soft Single Column Failure in Advanced  Nano SRAM Device with Internal Probing Techniques”, 31th ISTFA Proceedings, Nov. 2005, pp. 46-48.


[4] R. Ross, K. Ly, M. de la Bardonnie, L.F.Tz. Kwakman, F. Lorut, M. Lamy, C. Wyon, “ORIRCH Driven Failure  Analysis for Process Development of 120nm to 65nm  Technology Nodes”, 30th ISTFA Proceedings, Nov. 2004, pp. 447-450.


[5] Noel C. de Luna, Michelle F. Bailon, Alvarado B. Tarun, “Analysis of Near-IR Photon Emission From 50nm n- and  p-Channel Si MOSFETs”, IEEE Trans. Electron Devices, vol. 52, no. 6, pp. 1211-1214. Jun. 2005.


[6] M. Remmach, R. Desplats, P. Perdu, J. P. Roux, M. Vallet, S. Dudit, P. Sardin, “Light Emission and TRE for  a 120nm Technology Case Study: How Much  Wavelength Shift”, 11th IPFA Proceedings, Jul. 2004, pp. 139-142.


STI Punch-through Degradation Related Standby Current Failure in HTOL Test - A Case Study


Wen-Rong Chen, Wei-Chun Tseng, Yi-Ju Lee, Kuang-Wen Liu, Li-Kuang Kuo, Shaw Yin, Chih-Yuan Lu


Macronix International Co., Ltd., Hsinchu, Taiwan  E-mail: wrchen@mxic.com.tw, Tel: 886-3-5786688


This report summarizes the analysis results of 0.13µm  technology 256Mbits NBit HTOL (High Temperature  Operational Life) induced standby current failures caused by  STI (Shallow Trench Isolation) punch through induced  leakage degradation.  Electrical analysis, EMMI and stress  experiment on test devices are employed to identify the failure  mechanisms, root causes, and corrective solutions.  From this  study, improvements could be achieved by circuit layout  modification.


During development of 0.13µm 256Mb Nitrided ROM (Read  Only Memory) (NROM/NBit) [1-2], a steadily increasing  standby current failure is found after HTOL test at 125℃.  As  the HTOL stress time increased, the standby current is  increased as shown in Fig. 1.  The standby current of the  failed sample is about 50~70µA.  To identify the leaky current  source, degraded samples were inspected by EMMI (Emission  Microscope Inspection) under standby mode.  Because the  suspected damaged devices are covered with wide metal buses  and with very tight space between metal lines, which makes  the front side EMMI image with low resolution.  Therefore, backside EMMI were used to obtain higher resolution and  clearer image on the suspected damaged locations.  The  backside EMMI image photo is shown in Fig. 2 indicates two  abnormal hot spots (failed locations), which belong to two  identical power line-switching circuits.  Moreover, each hot  spot locates near the center of the two adjacent pMOSs in  each power line switching circuit as shown in Fig. 3.  FIB (Focus Ion Beam), SEM (Scanning Electron Microscopy), PVC (Passive Voltage Contrast) and TEM (Transmission  Electron Microscopy) were used to find defects.  However, no  defect or physical damage could be found on these two  pMOSs (M3 and M4) by de-layering to substrate, parallel  lapping to poly-gate layer, SEM/PVC inspection, and crosssection TEM on STI region.  Therefore, the leaky standby  current may occur from the pMOSs itself or between two  transistors (M3 and M4).  The possible mechanisms for the  leakage degradation are pMOS Hot Electron Induced Punchthrough (HEIP) [3], gate oxide degradation [4], and isolation  degradation between devices [5].


5 20 40 60 80 95 99


99.9


Standby Current(uA)


HTOL0h


HTOL168h  HTOL500h


Figure 1: Standby current is increased with HTOL stress time (Sample size is 80 units).


Figure 2: Two photoemission hot spots(circled by dashed  lines) by backside EMMI at standby mode. Both of these two  hot spots locate between two pMOSs (M3 and M4 of Fig. 3).


Analysis and Discussion


Since the EMMI hot spots are found at the neighborhood of  two pMOSs, the circuit operation bias of Fig. 3 is reviewed.  The source side of transistor M1 and M2 are connected to  about 10.3V (HV-1) during HTOL test and the two transistors  M1 and M2 are turned on/off interlacedly.  Moreover, M3 and  M4 have the minimum active diffusion island isolation space


(0.32um) from chip layout as Fig. 4.  Therefore, the STI  isolation ability and quality are highly suspected to be the root  cause, because M3-to-M4 isolation space (0.32 um) is shorter  than the channel length (2 um) of the two pMOSs.  The HEIP  should be less possible to occur for long channel length  pMOSs.  So, the isolation quality is examined to check any  weakness by test devices.


Figure 3: One loading swithing circuit(one level shifter + one  pMOS) diagram for selecting/disabling power driving signal (PWR-1).


Figure 4: Layout diagram for M1~M4 of Fig. 3(Only with  Metal-1, contact, poly-Si gate, active diffusion layers. Not  fully scaled). The space length between M3 and M4 diffusion  is 0.32um. The channel length of M1~M4 is 2um.


Test devices shown in Fig. 5 are manufactured by the same  process flow, in the same wafer, and with the same isolation  space and depth as transistor M3-to-M4.  M1~M4 pMOS  transistors are with 2um channel length and with n+ polysilicon gate.  Isolation trench depth is 3400A by RIE


(Reaching Ion Etching) with nitride hard mask.  Then thermal  oxide is grown to remove RIE damage and thin silicon nitride  liner layer is deposited.  Next, the trench oxide is filled in by  HDP oxide followed by densification at high temperature and  CMP planarizaiton.


Figure 5: Schematic diagram of test devices for stress. (STI  space=0.32um, STI depth=0.34um)


The leakage current is significantly increased after -10.3V / 130sec DC voltage stress on test device as shown in Fig. 6.   The stress bias is applied to terminal-Hi, GND is connected to  terminal-Lo during stress.  As leakage measurement, connect  terminal-Hi to Vsweep and set terminal-Lo to GND for  forward mode.  The isolation leakage current starts to increase  obviously when sweep voltage across STI is lower than -9V.  This isolation degradation can be that stress injected holes are  accelerated to generate EHPs (Electron-Hole Pairs) at  terminal-Hi.  Since electrons are easier to be trapped at STI  oxide due to lower SiO2 potential barrier and higher energy  obtained from E-field for electrons, and holes are swept by  electric fields to Nwell terminals.  So, when the generated  electrons are trapped in STI, the majority carrier of Nwell is  depleted.  Therefore, leak path between p+ to p+ diffusion  regions is formed [5].  Besides, the forward and reverse mode (the hi and lo node are interchanged after stress) isolation  leakage in Fig. 6 are very different.  The additional  degradation can be attributed to the hot electrons’ damage at  terminal-Hi, because enhanced terminal-Lo current injection  in the reverse mode [6-7].  Moreover, STI silicon nitride liner  accelerates HEIP of pMOS, because electrons can be easily  trapped at the interface between trench thermal grown oxide  and silicon nitride liner [7-8].  By skipping the nitride liner  layer of the STI process, the stress-induced leakage  degradation is gone even after –11V/20ksec stress, while the  STI with silicon nitride liner process degrades obviously in  Fig. 7.  Therefore, that the nitride liner acts as a critical layer  for isolation punch-through degradation is proved, because  many traps exist in the nitride oxide interface and nitride  layer.  The trapped electrons degrade the characteristics of p+ to p+ isolation are shown as schematic diagram in Fig. 8.


To solve standby current failures, three actions are tried.  Firstly, if the stress voltage is -8V, even after 20ksec, no  isolation leakage degradation is found as shown in Fig. 9.  However, if stress voltage is high to -11V / 1660sec, the  isolation leakage will degrade about 4 orders at Vsweep=-8V.  Therefore, to limit the voltage across STI is a method to  prevent or mitigate the stress damage to STI.  Since the HV (High Voltage) operation bias is necessary for some functions, voltage limitation is not acceptable for this product.  Second,


skipping nitride liner process method could eliminate isolation  leakage demonstrated in previous paragraph.  Nitride liner is  usually used for preventing STI bottom corner oxidation and  keeping corner profile during succeeding high temperature  process steps.  However, skipping nitride liner of STI process  would cause mechanical stress induced substrate dislocation  defects and device off-state leakage [9].  It is not easy to  perform and needs a period of time to optimize [10].  An  alternative method is to modify circuit layout as Fig.10.  This  new layout is to let the stress voltage on M3-to-M4 (0.32um) of Fig.3 (old layout diagram) be changed to top and bottom in  Fig. 10(arrows with dashed lines).  By this way, M3-to-M2  and M1-to-M4 (1um) have wider space between their  diffusion islands and lower E-field.  Also, the chip has no  need to change process of FEOL  (Front End of Line).  So, the  chip layout change by metal line routing modification is fast, cheap, and simple way to solve punch-through induced  standby current problem.    After changing circuit layout as  Fig. 10, no standby current degradation occurs even after 1000  hours HTOL test shown in Fig. 11.


The STI punch through induced standby current degradation  is analyzed.  The p+-to-p+ leakage is due to stress induced hot  electron trapping on nitride liner by stress high voltage on test  devices.  One of solutions is removing the nitride liner that  could prevent isolation leakage degradation by high voltage  stress.  However it would result in substrate dislocation defect  and device off-state leakage.  Currently, the best solution is  using circuit layout change to modify the voltage across two  diffusion areas for solving HTOL induced standby current  degradation.


-4


-6


-8


-10


1E-13 1E-12 1E-11 1E-10 1E-9 1E-8 1E-7 1E-6


Sweep Voltage on Hi(V)


Hi_Before_Stress(forward) Lo_Before_Stress(reverse) Hi_After_Stress(forward) Lo_After_Stress(reverse)


Figure 6: Isolation degradation after -10.3V/130sec stress on  terminal-hi.  (Lo_After_Stress represents the sweep voltage  applying to terminal-lo, terminal-hi connecting to GND  during measurement.)


1E-13 1E-12 1E-11 1E-10 1E-9 1E-8 1E-7 1E-6 1E-5 1E-4 1E-3


With SiN liner Before Stress


With SiN liner After Stress


Without SiN liner Before Stress  Without SiN liner After Stress


Figure 7: Influence of the STI process with or without nitride  liner to isolation leakage before/after stress.  The STI without  liner nitride process has no degradation even after -11V / 20k  sec stress.


Figure 8: Schematic diagram showing the mechanism of the  HEIP of STI after HV stress.


-3


-7


1E-13 1E-12 1E-11 1E-10 1E-9 1E-8 1E-7


Sweep Voltage on Lo(V)


Bef_8V/30ks_stress  Aft_8V/30ks_stress  Bef_11V/16ks_stress  Aft_11V/16ks_stress


Figure 9: Isolation leakage of STI stress by limit stress  voltage/time to under -8V/30ksec has no degradation.  When  the stress voltage is increased to -11V, the leakage will  become high after 1660 sec stress.


e- e- eeee-


Figure 10: New layout diagram for M1~M4 of Fig. 3(Only  with Metal-1, contact, poly-Si, DIF layers. Not fully scaled). The space length between M1 and M3 diffusion is 0.32um. The channel length of M1~M4 is 2um.


HTOL0h (new)


HTOL168h (new) HTOL500h (new) HTOL1000h (new) HTOL 500h (old)


Figure 11: No standby current degradation is found after  1000h HTOL by new layout (Sample size is 77 units).


The authors would like to thank Sam Chen, Yufe Lin, W.P. Lu, Nancy Wong and Chester Lo for providing technical  advice and sample preparation assistance.


[1] B. Eitan, P. Pavan, H. Bloom, E. Aloni, A. Frommer, and  D. Finzi, “NROM: A novel localized trapping, 2-bit non179


volatile memory cell”, IEEE Electron Device Letter, Vol. 21, p545-545, (2000).  Note: Saifun NROMTM is  trademark of Saifun Semiconductor, Ltd. NBit is  trademark of Macronix International Co. Ltd.


[2] W.J. Tsai, N.K. Zous, C.C. Liu, C.H. Chen, T. Wang, S. Pan and C.Y. Lu, “Data retention of SONOS-type two-bit  storage flash memory cell”, Tech. Digest of International  Electron Devices Meeting (IEDM), p719-722, (2001).


[3] Mitsumasa Koyanagi, Alan G. Lewis, Russel A. Martin, Tiao-Yuan Huang, and Jhon Y. Chen,  “Hot-ElectronInduced Punchthrough (HEIP) Effect in Submicrometer  PMOSFET’s”, IEEE Trans. on Electron Devices, ED-34, No. 4, p839-844, (1987).


[4] Jone F. Chen, Kazunari Ishimaru, and Chenming Hu, “Enhanced Hot-Carrier Induced Degradation in Shallow  Trench Isolated Narrow Channel PMOSFET’s”, IEEE  Electron Device Letters Vol. 9, No. 9, p332 (1998)


[5] S.W. Hong, G.Y. Jin, H.W. Seo, D.I. Lee, J.H. Song, J.Y. Noh, Y.C. On, J.Y. Kim, D.H. Kim, H.H. Kim, D.J. Won, W.W. Lee, D.H. Song, K.Y. Lee, and W.S. Lee, “Evaluation of STI Degradation Causing DRAM Standby  Current Failure in Burn-in Mode Operation Using a  Carrier Injection Method”, Proceedings of the 40th  Annual International Reliability Physics Symposium, p283-286 (2002)


[6] Peng Fang, John T. Yue, Don Wollessen, “A Method to  Project Hot Carrier Induced Punch Through Voltage  Reduction for Deep Submicron LDD PMOS FETs at  Room and Elevated Temperature”, Proceedings of the  30th Annual International Reliability Physics  Symposium, p131-135 (1992)


[7] M.H. Cho, Y.I. Kim, J. Choi, D.S. Woo, J.P. Lee, Y.J. Park, W.S. Lee and B.I. Ryu, “Analysis DRAM Standby  Current Failure Due to Hot Electron Induced Punchthrough of PMOS Transistor”, Proceedings of the ISTFA  2005, p186-188 (2005)


[8] Jay-Kyu Lee, Sang-hyeon Lee, G.T. Jeong, T.Y. Chung, Kinam Kim, “Investigation of pMOSFET Hot Electron  Induced Punchthrough (HEIP) in Shallow Trench  Isolation”, Proceedings of European Solid-state Device  Research Conference.(2001)


[9] Beshan Tseng, “Skipping nitride liner effect on STI”, Macronix internal publication.


[10] Chih-Hang Tung, George T.T. Sheng, Chih-Yuan Lu, “ULSI Semiconductor Technology Atlas”, John Wiley & Sons, Inc., p235-252 (2003)


*) Bettina Seidl, Infineon Technologies AG, Wernerwerkstrasse 2, 93049 Regensburg, Germany


Bevel Etching: A Low Cost Alternative to FIB


B. Seidl*, J. Walter, M. Kirchberger


Microstructural diagnostic for electronic packaging  development and failure analysis under industrial  manufacturing conditions require fast but reliable  preparation routines. The aim of the presented poster is to  introduce a time and cost efficient preparation technique for  FESEM (field emission scanning electron microscope) investigations with focus on typical issues in electronic  packaging development and failure analysis. The new ion  beam based technique acts as a low cost alternative to FIB, able to prepare much wider section areas, combined in a  tool, which can also be used for standard ion beam  polishing processes.


During the past years the worldwide packaging  development efforts created systems containing an  increasing variety of different materials. The study and  description of essential interface phenomena like adhesion  and diffusion forced the failure analysts and engineers to  look for high quality, artifact-free and universal methods for  cross-section sample preparation. The common mechanical  treatment for grinding and polishing fails if grinding  particles, like diamond or silicon carbide become stuck in  soft materials, for example high lead solder.


Another unwanted artifact is the disappearing of aluminium  layers, due to corrosion by the grinding water residual ions. Due to these effects a lot of package failures remain hidden (micro cracks, voids) or the micro structure is physically  destroyed (metallic grain boundaries, intermetallic phases, porosity).


The FIB (focused ion beam), which is an alternative method  for such cross sectioning has following disadvantages: it is  an expensive and time-consuming method, and it is  producing relatively small section areas.


We introduce the new bevel etching technique which is  universally applicable for all materials and package devices, whose reliable brilliant process results allow to give the  name “low cost FIB”.


Furthermore the new preparation process treats a relatively  large section area compared to FIB techniques.


The bevel etching technique is normally performed by a  standard ion beam polishing tool, e.g. Bal-Tec RES-101, which requires no additional investment budget. Both  processes could be used alternatively with separate sample  holders.


During the past 5 years the ion beam polishing method was  established as a standard within Infineon Technologies and  has proven its benefit in many applications. [1]


Equipment and Method


Our method is based on a standard ion beam polishing tool  which is well known for preparation of standard cross  sections [2]. The ion beam polishing process requires an  especial sample holder, which allows to load complete  embedded cross-sections with 25 mm in diameter. The  equipment incorporates two ion beam sources and allows  continuous or oscillating specimen rotation. Angles of  incidence can be individually adjusted.


The bevel etching process requires a especial designed  sample holder with a sacrificial cover mounted over the  sample surface, which acts as an ion beam mask (see figure  1).


Figure 1: top view of bevel etching sample holder


Table


Sample


Cove


Cover  edge


To achieve a time efficient preparation result, a prepreparation of the particular sample is necessary, because of  the moderate abrasion rates of the ion beam bombardment  process. The most applicable pre-preparation is a standard  grinding process on a free standing cross section. The  grinding should be continued with a distance of 10 – 20µm  to the target plane.


The prepared sample has to be positioned in the sample  holder close to the sacrificial cover edge. The single ion  beam ablates the material behind the cover mask with a  given slope, during the beam position is oscillating to  enlarge the lateral dimensions of the section area (see figure  2).


Figure 2: schematic configuration of the bevel etching  process


The well prepared usable section area for FESEM analysis  reaches a length between 0.5 and 1.0mm, which overruns  FIB prepared areas a multiple times (see figure 3).


Figure 3: Bevel etching section area of Au- wirebonds on Al  pads


Table 1 shows typical parameter settings for bevel etching  and ion polishing processes on a Bal-Tec RES-101 tool.


Tool Parameters


Ion source type


Sattelfeld


Used ions


Ar+


Typical used ion energy


7kV


Section diameter


0.5 - 1mm


Angle of incidence:


For ion beam polishing (two  beams)


10° - 15°


For bevel etching (single  beam)


2°


Abrasion rate


~ 1 – 3µm/h


Max. sample size


4 x 5 x 1.5 mm (LWH)


Sample surface temperature  w/o cooling


< 120°C


Sample cooling option


liquid nitrogen


Sample holder slopes


35° and 90°


Table 1: Configuration parameters of the tool Bal-Tec RES101


In the following we focused on three examples, which will  illustrate the advantages of a bevel etch processing as  artifact free preparation technique, compared to standard  cross section and standard FIB techniques.


The first case describes the difficulties of preparing a gold  wire bonded on an aluminium pad. The standard cross  section process includes a wet grinding step, which is able  to procure aluminium corrosion. Even the use of de-ionized  water can start corrosion of the base aluminium material  under formation of voids and aluminium hydroxide (see  figure 4). Due to this effect a proper assessment of voiding, micro structure and cracking should be impossible.


To prevent such wet corrosion effects a water free  preparation technique is required. The FIB technique is able  to fulfil these demands. Figure 5 shows a typical FIB cut of  an Au wirebond imaged with a FESEM. The aluminium pad  metallization is undisturbed but parasitic grooves are visible  at the abraded surface. This artifact is omnipresent, if deep  FIB cuts are necessary. Another disadvantage is the long  processing time to perform these cuts.


Figure 4: Standard embedded cross section of a Auwirebond on Al pad after mechanical grinding/ polishing  and standard ion polishing, showing aluminium corrosion


Figure 5: FIB cut of a Au- wirebond on Al pad imaged with  FESEM


The bevel etching technique enables an artifact free dry  preparation of the described interconnect without showing  corrosion and grooves (see figure 6). The section area  within such a cut could reach up to 1mm lateral dimension (see figure 3).


Figure 6: Bevel etching of a Au- wirebond on Al pad


The second example describes the difficulties of preparing  soft materials, like solder layers containing a large lead  content (“high lead”). During the grinding and polishing  process the SiC and diamond particles get stuck in the soft  solder matrix and withstand the following standard ion  beam polishing step. The remaining particles complicate the  right interpretation of the taken SEM images, regarding  voiding, micro cracks and microstructure (see figure 7).


Figure 7: FESEM image of a high lead solder layer after  standard cross section processing


The FIB preparation of high lead solder layers is nearly  artifact free but time consuming to achieve large preparated  section areas. These are necessary to find and follow crack  paths and find out void distributions in the solder layer. The  small lateral dimensions of a standard FIB cut make a short  time analysis difficult (see figure 8).


Au


Al pad


imid


soft


grinding


groove


Figure 8: FESEM image of a FIB cut of a high lead solder


The bevel etched sample shows no grinding and polishing  particles at all. Patches of cracks, precipitations in the solder  and delaminations are clearly visible. Traces of the eroding  ion bombardment process are visible in the “background” of  the section area (see figure 9, with same magnification as  figure 8).


Figure 9: Bevel etching of a high lead solder layer showing  a crack path in the solder and delaminaton at chip backside


The last example shows an adhesive layer with silver filled  matrix. The preparation should be artifact free, without  filling up voids or smearing the glue matrix, so that  following analysis can focus on void distribution, micro  cracks and delamination at interfaces. Figure 10 shows  possible artifacts like smearing and inclusion of abrasion  debris in glue voids.


Figure 10: FESEM image of a adhesive glue layer after  standard cross section processing, showing grinding  residues in glue voids


FIB cutting is able to prevent these artifacts, but with the  known disadvantage of smaller lateral dimensions of the  usable section area for analysis (see figure 11).


Figure 11: FIB cut of an adhesive glue layer imaged with  FESEM, showing glue voids and the cut dimensions


The bevel etched adhesive glue layer shows well prepared  glue voids and no smearing effects. The section surface  shows some small grooves which are a topology effect from  the void edges, but don’t hinder a proper analysis (see  figure 12, same magnification as figure 11).


crack


delaminatio


leadfram


Figure 12: Bevel etching through an adhesive glue layer  with voids in the glue


The use of the bevel etching preparation technique can  significantly enhance the preparation quality of electronic  packaging samples. It was demonstrated that a various set of  materials, like metal interconnects, soft solders and glues  could be prepared without artifacts. The bevel etching  reveals following advantages compared to the known FIB  processing: it is time-saving, and it produces larger section  areas, worth to be named “low cost FIB” in this context. Furthermore the described process can easily be established  in failure analysis labs by integrating it into existing ion  beam polishing equipment.


The authors would like to thank N. Soellner and S. Wichmann for their support in sample preparation and  imaging.


[1] Mack W., Seidl B., Fischer R., Ort T., Walter J., Grünewald J., Berthold L., Petzold M.; “Ion beam  polishing for Embedded Cross-Sections and its  Advantages for FESEM Analysis in Electronic  Packaging”; Conference proceedings from 30th  Symposium for Testing and Failure Analysis, Boston, MA, USA, 14-18 Nov (2004), p. 338 – 345


[2] Grünewald W.; “Applications of the Ion Beam Etch  Equipment RESSEM / RES 120”; Bal-Tec  Usermeeting IFW Dresden, Dresden, Germany, 23-24  May (2006)


Key Words


Bevel etching, Bevel etch, FIB, Focused ion beam, FIB cut, Ion beam polishing, Cross section, Nailhead, Wirebond, Solder, Glue, Adhesive, Scanning electron microscopy, FESEM, SEM, Polishing, Embedded cross-section, Electronic packaging, Delamination, Sample preparation, Sample holder, Angle of incidence


leadframe


voi


Cross-sectional sample preparation techniques for 2D doping profiling of  specific site by SCM


Tae-Kwon Lee, Tae-Sun Back, Jong-Hyeop Kim, Yoon-Baek Park, Ho-Joung Kim, Soun-Young Lee


Research and Development Division, Hynix Semiconductor Inc. San 136-1, Ami-ri, Bubal-eub, Ichon-si, Kyoungki-do 467-701, Korea   tklee@hynix.com, 82-31-630-2373


Scanning Capacitance Microscopy (SCM) is an SPM technique  which measures capacitance variation between tip and sample  generated by applied AC bias while the tip is scanning in contact  mode.  SCM can image the carrier concentration profiles in two  dimensions with spatial resolution of about 10-20 nm on actual  devices. This capability makes the SCM a useful tool in the  development, manufacturing, testing and failure analysis of  semiconductor devices. [1] One of the effective SCM  applications in failure analysis is cross-sectional carrier profiling  of a failing site. In order to apply SCM cross-sectional carrier  profiling to failure analysis, site-specific sample preparation  techniques are needed.


Cross-sectional samples for SCM are routinely prepared by  manual polishing techniques. As integration becomes greater  and shrinkage of VLSI devices is greater, the SCM observation  site for failure analysis has been smaller and smaller. Due to the  problems of controlling the polishing rate and stopping at a  specific position manually, it is more difficult and timeconsuming to prepare site-specific SCM samples for crosssectional carrier profiling.


Micro-cleaving which mainly has been used for SEM sample  preparation is a good candidate for preparing a site-specific  sample to overcome the problems with conventional polishing  methods. Using this technique, we can cut the specimen fast and  easily with ㎛ level cutting accuracy.


Focused Ion Beam (FIB) milling is the more precise method to  perform cross-sectioning of a specific site. It has been used to  prepare site-specific cross-sectional samples for TEM  observation. By FIB milling, we can process and monitor  specimens simultaneously with sub- ㎛ accuracy. However  surface amorphization and charge trap layers formed during FIB  machining affect the SCM dC/dV signal. [2, 3] Lately it is  proposed that additional fine polishing with colloidal silica or  plasma etch can remove the damaged layer. [2, 3, 4]


In this study we have demonstrated and evaluated that microcleaving and FIB milling methods are acceptable for sitespecific SCM sample preparation.


Experiments & Result


Micro-Cleaving technique


Fig. 1. Schematic process flow of micro-cleaving sample  preparation.


The Micro-cleaving process for cross-sectional sample  preparation is follows. First, cut the sample to obtain crosssectional surface of a specific structure by using automated  cleaving system (We used SELA MC 600). Next, polish  backside of observation surface to reduce sample height. Finally, surface oxidation and UV illumination process is done to grow  thin oxide layer. (Fig. 1)


Fig. 2. AFM 3D image of cleaved surface of  Sub-Si. Measured  Rms roughness is 2.11Å


Coarse  Cleaving


Cleaving  plane


Observation


site


Fine  Cleaving


Backside  Polishing


Cleaning


Oxidation   UV treatment  W/F


Cuttin g


Cleaving  Plane


The cross-sectional surface obtained by micro-cleaving is very  smooth (Rms ≈ 2 Å), it is additional polishing not necessary to  get a smooth surface. (Fig. 2) Therefore we can reduce total  sample preparation time.


Fig. 3. SCM image of P-type doped Source/Drain prepared by  micro-cleaving techniques.


Figure 3 is a SCM image of P-MOS test pattern (Length is 10㎛) prepared by micro cleaving techniques. P-type Source/Drain  formed in N-Well is well observed.


The drawback of the Micro-cleaving method is that when the  need arises to cleave a fully processed device chemical etching  is needed to strip the layers above the layer of interest. Because  the front-end process patterns are covered with back end of the  process layers. The area of interest is not observable in a  microscope image - we choose the cleaving position through an  optical scope image in the automated micro-cleaving system.


To improve this problem an FIB is employed. With the  assistance of FIB milling, the upper layers are removed. The  cleaving position is identified and marked. Finally, the front end  structure of the sample is cleaved. (Fig. 4)


Fig. 4. Optical microscope images of cleaving location marked  by FIB(up), after micro-cleaving(down)


Figure 5 is an AFM/SCM image of a P-MOS in a DRAM  peripheral region made by FIB marking + the Micro cleaving  technique. When the specimen is broken into pieces by Microcleaving, the metal pattern is normally torn off. So the pattern  shapes in the AFM image are not as clear as in traditional  polishing methods. But the SCM data is not affected because the  data acquired at the doping region below the metal structures. STI and Source/Drain profile is well matched with expectation.


Fig. 5. AFM/SCM images of DRAM Cell Peri region prepared  by micro-cleaving. AFM(up), SCM(down)


FIB milling technique


First the sample is cleaved near the target with a Micro-cleaving  system and the cross-sectional area of target is milled with an  FIB. Then low energy milling is performed with an FIB to  remove the surface damage layer.(Fig. 6) Figure 7 is an  AFM/SCM image of a P-MOS in a DRAM peripheral region  prepared by FIB low energy milling technique.


Fig. 6. Optical scope images of specimen after low kV milling. Top view(left), cross-section view(right)


p+


N-Well


Marker for  cleaving


FIB milled area to  identify observation  pattern


G G


P+ P+ P+ P+


P+


Fig. 7. AFM/SCM images of DRAM Cell Peri region after low  energy ion milling. TEM image is inserted for comparison


The pattern shapes in the AFM image are of the same clarity as  in TEM images. But the carrier profile is not seen in the SCM  image. The assumption is made that Ga+ ions damages during  FIB milling were not fully removed by low energy ion milling.


To remove the remainder of the damaged layer, fine polishing is  used in which the specimen is polished on a polishing cloth with  a DI water flush instead of colloidal silica. (Fig. 8)


Fig. 8. Process flow of FIB milling sample preparation


Fig. 9. AFM/SCM images of DRAM Cell Peri region prepared  by FIB Milling & fine polishing with DI flushing.


Fig. 9 is an AFM/SCM image of a gate in an N-MOS transistor  in a DRAM peripheral region prepared by FIB milling. The  pattern shapes are clearly seen in the AFM image and the N-type  doping region is seen at the expected place.


In this study, we demonstrated that Micro-cleaving and FIB  milling are capable of preparing a cross-sectional sample of a  specific site for SCM observation.


Using the Micro-cleaving technique, a cross-sectional sample  can be prepared easily with higher accuracy and shorter time  than using a polishing method. However, Micro-cleaving can’t  be used by itself in the case of cross-sectioning a pattern formed  by front end processing of sub-micron patterns.


The FIB milling technique - though it is time-consuming due to  additional fine polishing - has higher accuracy in crosssectioning than Micro-cleaving. The FIB technique can assist the  Micro-cleaving technique in cleaving of front end patterns.


In conclusion, the techniques described were found to show  good SCM results and are applicable to preparing crosssectional sample of a specific site for SCM investigation.


1. Veeco Metrology & Instrumentation, “Electrical  Characterization with Scanning Probe Microscopes” www.veeco.com, Dimension 3100 application note AN90


2. David K. Fillmore and Shinxin Wang, “Investigation of LowEnergy Focused Ion Beam milling for Scanning Capacitance  Microscopy Sample Preparation” Proceedings of the 30th


International Symposium for Testing and Failure Analysis 2004.


3. K. Jarausch, J. F. Richards, L. Denney, A. Guichard, P.E. Russell, “Site specific 2-D implant profiling using FIB assisted  SCM”, Proceedings of the 28th International Symposium for


Testing and Failure Analysis 2002.


4. N. Rodurigez et al, “Evaluation of Scanning Capacitance  Microscopy Sample Preparation by Focused Ion Beam”


Microelectrics Reliability 46 (2006), pp. 1554-1557


AFM


SCM


FIB milling


Oxidation with UV illumination


SCM Observation


Micro Cleaving


Low kV milling


Fine Polishing with DI Flushing


n+ n+ n+


G G G


The failure site localization using absorbed current image and voltage  distribution contrast


Takeshi Nokuo, Yoshiyuki Eto


JEOL Ltd., 1-2 Musashino 3-chome, Akishima, Tokyo, Japan  nokuo@jeol.co.jp, TEL: 81-42-542-2249 FAX: 81-42-542-1924


Zane Marek


JEOL USA, Inc., 11 Dearborn road, Peabody, MA  marek@jeol.com


In failure analysis of semiconductor devices, it is important to  identify the accurate position of marginal contact to localize a  failure site. The advantage of the technique of absorbed  current image (AEI) to identify the accurate position of  marginal contact has been reported and widely recognized [1]. The authors have reported the development of an instrument  combining AEI method with nanoprobing to utilize it [2]. Meanwhile, in failure analysis, to detect smaller amount of  resistance-increased area is required due to the downsizing of  devices. For this purpose, the authors developed voltage  distribution contrast (VDIC) method besides AEI. This paper  reports the detection ranges of marginal contact for both AEI  and VDIC methods, which are experimentally evaluated.


Method


AEI Method


Figure 1 shows a principle of marginal contact detection by  AEI. One probe (Probe1) makes contact with the right end of  the interconnect, which is connected to the pre-amplifier for  AEI (current-to-voltage converter). The other probe (Probe2) makes contact with the left end of the interconnect, which is  connected to the ground potential. When the primary electron  beam irradiates on a side A, a constant current (Iaei) source is  generated. Then this Iaei will be divided to both amplifier and  ground potential. The current from side A to amplifier (Iaa) can be obtained from


( ) (


Ra


Rs


Rg


aei


aa II


×


When the primary electron beam irradiates on a side B, the  current from side B to amplifier (Iba) can be obtained from


ba II


Where


, then we can obtain


a RR 〈〈


g RR 〈〈


ba


aa II 〉〉


Here,  denotes the resistance from marginal contact to  amplifier,  denotes the resistance at marginal contact S,  denotes the resistance from marginal contact to ground  potential,  denotes the absorbed current.


aR


sR


gR


aeiI


Thus the boundary of the contrast appears at the marginal site  on the AEI [1].


Primary electron


Ground


Amplifier


Figure 1. A principle of marginal contact detection by AEI


VDIC method


Figure 2 shows a model of VDIC. One probe is connected to  the VDIC pre-amplifier (a high impedance voltage amplifier) and the other one is connected to the ground potential. When  the primary electron beam irradiates on both side A and B, the  same amount of absorbed current is generated. So, the primary  electron beam is focused on the side B, the absorbed current  generates a voltage of


g


V ×=


Then the primary electron beam is focused on the side A, the  absorbed current generates a voltage of


a IV


Here,  denotes the resistance from marginal contact to  amplifier,  denotes the resistance at marginal contact S,


Probe2


Probe1


Marginal contact Rs


Iaa


Iba Ia


Ibg


gR  denotes the resistance from marginal contact to ground


potential,  denotes the absorbed current. aeiI


Thus the boundary of the contrast appears at the marginal site  on the AEI [2].


Figure 2. A principle of marginal contact detection by VDIC


In this experiment, 2 test element groups (TEG) for  interconnect, which have different total resistance of 1.3MΩ  and 96kΩresistance were used. Both TEG have 4000 contacts  and contact pads at 1000 contacts, 120 contacts and 10  contacts shown in Figure 3. So AEI and VDIC method are  applied to all these 8 resistances shown Figure 4.


Figure 3. The sample, which is used for evaluation


Sample＼Contacts 4000


120


Sample #1


96kΩ 23kΩ 2.8kΩ 240Ω


Sample #2


1.3MΩ 320kΩ 39kΩ 3.3kΩ


Figure 4. Tables for total resistance (R)  of evaluation


Pictures for various resistances were shown in Figure 5. In  case of AEI, images can be observed from 1.3MΩ to 23kΩ. At a total resistance less than 23kΩ, the AEI amplifier was  not able to visualize the interconnects. The reason is assumed  that the lower resistance of interconnects causes the saturation  or instabilities of current-to-voltage converted amplifier. In


VDIC, images can be observed for all 8 resistances. But  comparing 320kΩ image with 1.3MΩ image, the image of


1.3MΩ is not as sharp as the image of 320kΩ. This might be  the result of a delay of the high impedance voltage amplifier.


AEI 240Ω


AEI 2.8kΩ


Figure 5-1. AEI pictures for sample #1


Figure 5-2. VDIC pictures for sample #1


Iaei


Rb


AEI 23kΩ


AEI 96kΩ


VDIC 240Ω


VDIC 2.8kΩ


VDIC 23kΩ


VDIC 96kΩ


Figure 5-3. AEI pictures for sample #2


Figure 5-4. VDIC pictures for sample #2


Figure 5.AEI and VDIC pictures for various resistances


We have evaluated the performances of our AEI and VDIC  methods. The detection range of the marginal contact for both  methods should be the same as the observable range of  imaging of various resistances. In Figure 5. the detection  ranges for both AEI and VDIC are plotted. X-axis represents  the total resistances of target interconnect, and Y-axis  represents the resistance of marginal contact. For AEI method, we can detect marginal contact, which has a resistance  minimum 23kΩ, in interconnect, which has more than 23kΩ


total resistance. For VDIC method, we can detect marginal  contact, which has a resistance of 240Ω to 1MΩ, and an  interconnect, which also has more than 240Ω to 1MΩ total  resistance.


AEI 3.3kΩ


AEI 39kΩ


AEI 320kΩ


AEI 1.3MΩ


It can be relatively said that the AEI has an advantage of  analyzing huge scales of TEG for interconnect and the VDIC  has an advantage of analyze interconnects in actual devices  which has relatively low resistance. Also the authors will try  to improve amplifiers to extend these detection ranges.


Figure 6. Detection range of AEI and VDIC method


[1] C. A. Smith, C. R. Bagnell, F. A. DiBianca, E. I. Cole, D. G. Johnson, W. V. Oxford, R. H. Propst, “Resistive  Contrast Imaging: A New SEM Mode for Failure  Analysis” IEEE Transaction on Electron Devices. ED-33, No.2. 1986, pp. 282-285.


[2] T. Nokuo, Y. Eto, Z. Marek, “A new method for failure  analysis with probing system based on scanning electron  microscope” 2007 IEEE International Reliability Physics  Symposium Proceedings. pp. 614-615.


101 102 103 104 105 106 107


101 102 103 104 105


106 107


AEI


VDIC


VDIC 3.3kΩ


VDIC 39kΩ


VDIC 320kΩ


VDIC 1.3MΩ


A Simple Adapter for Soft Defect Localization Using OBIRCH


Ted Kolasa


Freescale Semiconductor, Inc., Tempe, Arizona USA


In recent years Soft Defect Localization (SDL) has become an  increasingly used technique for identifying marginally  performing circuitry during microelectronic failure analysis.  This optical beam technique uses thermal and/or photonic  stimulation of the die to induce failures that can be expressed  by a change in digital state. [1]  This change in state can be  derived from various sources including digital or analog  outputs from a device, or a pass/fail output from a mini tester.  Equipment manufacturers have developed peripherals for their  tools that add SDL capability to existing optical beam tools, in  many cases providing excellent results. [2, 3]  However, these  upgrades add significant cost to the tool.


In this paper we present the design considerations for a simple  adapter that was developed in house to add SDL capability to  our Optical Beam Induced Resistance Change (OBIRCH) tool, including resolution of some unexpected problems.  We  will also present some SDL results produced using the  adapter.


Adapter Design


Figure 1 shows a simplified block diagram of the simple  adapter developed to add SDL capability to our OBIRCH tool.  The adapter essentially shows a step resistance change to the  OBIRCH tool whenever the digital input level toggles.  The  input logic signal controls switch SW1, which switches  parallel resistor R2 in and out of the current path.  In practice  the result is a noise free OBIRCH map that shows the bit  toggles as the laser scans across the sample


Design Considerations


For the original prototype, resistors R1 and R2 were originally  chosen to be the same to give a very large resistive delta when  the switch was activated.  The intent of this was to overcome  the effects of any noise in the current path.  For the switch, a  discrete npn transistor was chosen since it was readily  available and switching speed was not critical in this  application.  The base terminal was driven indirectly from the  digital input through a logic buffer to prevent loading of the  input signal.


When the first prototype SDL adapter was tested, the resulting  OBIRCH maps were very noisy.  It became apparent that the


cause was lack of isolation between the digital input and the  OBIRCH supply.  To correct this problem, separate isolated  grounds were designated for the digital section and the  OBIRCH loads.  In addition, we found that the large  resistance change was not necessary and that clean OBIRCH  maps could be achieved by reducing R2 so that R1 >> R2.  With these modifications, the resulting OBIRCH maps had  very little noise.


Figure 1: A simplified functional diagram of the SDL adapter.


While this adapter was built for use with an OBIRCH tool, the  design can apply directly to OBIC, and can also be used in  conjunction with a XIVA tool by simply inserting a series  resistor in the loading loop.


Sample SDL Results


The first opportunity to use this adapter in practice came when  failures were seen in a device during new product evaluation.  The failure manifested itself as an abnormal threshold shift in  a Vdd undervoltage monitor that could be seen externally  through an interrupt output pin.  Photoemission microscopy  and traditional OBIRCH examination did not yield useful  information to help identify the origin of malfunction.


Since the failure was observable as a digital output, the SDL  adapter was used next.  SDL maps were acquired across a  range of supply voltages, with particular attention paid to the  region between the Vdd undervoltage monitor transition point  for the failing unit and that of a normal unit.  We discovered a


sensitive location at a transistor in the undervoltage  comparator circuit in the failing unit.  When the laser  illuminated this transistor, the comparator output toggled, causing the external interrupt pin to toggle as well.  The SDL


Figure 2: A composite image showing the SDL map overlaid  on a section of the die containing the malfunctioning  comparator circuit.  The white arrow points toward an  abnormal bit toggle indication at a transistor.


Figure 3: A view of Figure 2 showing the SDL map only.  The  abnormal bit toggle indication is more visible in this view.


maps of this event are shown in figures 2 through 4.  Additional electrical and physical analysis of the suspect site  revealed no defects, but these findings helped the chip  designers to identify marginalities in this circuit design that  were corrected by modifications to the comparator circuit.


Figure 4: A magnified view of Figure 2 showing detail of the  abnormal SDL indication (arrow).


We have presented the design for an adapter that was  developed in house to facilitate Soft Defect Localization (SDL) testing.  This solution represents a simple, low cost  method to add SDL testing capability to our OBIRCH tool and  can also be used in conjunction with OBIC and XIVA tools  with little or no modification.  An early example of the SDL  results provided by this adapter was also presented.


[1] M. Bruce et al, “Soft Defect Localization (SDL) on ICs”,


Proc. 28th Int. Symp. Of Test and Failure Analysis (ISTFA), Nov. 2002, p. 21


[2]  “Dynamic Analysis by Laser Stimulation”, Technical  Note No. SSMS0008E01, Hamamatsu Corp., June 2005.


[3] D. Mitro et al, “Soft Defect Localization Techniques  without a Synchronization Signal to the Laser Scanning  Module”, Proc. 31st Int. Symp. Of Test and Failure  Analysis (ISTFA), Nov. 2005, p. 115


Studies of Galvanic Corrosion (Al-Ti Cell) on Microchip Al  Bondpads and Elimination Solutions


Hua Younan, Mo Zhiqiang, Zhao Siping and Gong Hao*


Chartered Semiconductor Mfg Ltd., 60 Woodland Industrial Park D, Street 2, Singapore 738406 Email: huayounan@charteredsemi.com


*Department of Materials Science and Engineering, National University of Singapore 119260 Email: msgonghao@nus.edu.sg


Galvanic corrosion (two metal corrosion) on microchip Al  bondpads may result in discolored or non-stick bondpad problem. In this paper, a galvanic corrosion case at bondpad  edge will be presented. Besides galvanic corrosion (Al-Cu cell), a concept of galvanic corrosion (Al-Ti cell) is proposed, which is used to explain galvanic corrosion at bondpad edge  with layers of TiN/Ti/Al matellization structure. A theoretical  model of galvanic corrosion (Al-Ti cell) is proposed to explain  chemically & physically failure mechanism of galvanic corrosion at bondpad edge. According to the theoretical model  proposed in this paper, galvanic corrosion on microchip Al  bondpads could be identified into two corrosion models: galvanic corrosion (Al-Cu cell) occurred mostly at the bondpad center and galvanic corrosion (Al-Ti cell) occurred specially at bondpad edge with TiN/Ti/Al matellization structure. In this paper, a theoretical model of galvanic corrosion (Ai-Ti cell) will be detail discussed so as to fully understand failure mechanis m of galvanic corrosion the bondpad edge. Moreover possible solutions to eliminate galvanic corrosion (Al-Ti cell) are also discussed.


Galvanic corrosion may result in discolored or non-stick


’


bondpad problem. In authors previous studies, theory,characteristics and eliminating solutions of galvanic corrosion(Al-Cu cell) have been studied [1-2]. After galvanic corrosion(Al-Cu cell), a lot of pinholes were found on Al bondpad  surface. However, recently another galvanic corrosion case  was found, which caused some  “hole-like ” defects at bondpad edge. For example, SEM micrograph (Fig. 1)showed that some  “hole-like ” defects were found at the bondpad edge after wafer die-sawing process. After performing studies, we believe that these defects  were not  only related galvanic corrosion (Al-Cu cell), also contributed  by galvanic corrosion (Al-Ti cell) as there was Al-Ti two  metal interface at bondpad edge with TiN/Ti/Al metallization  structure.


In this paper, we propose a theoretical model of galvanic corrosion (Al-Ti cell) and discuss chemically & physically


failure mechanism of galvanic corrosion at bondpad edge, and then discuss some eliminating solutions.


Introduction of Redox Potentials, Eo


In chemistry, Standard Electrode and Redox Potentials, Eo at 298 K (25o C) is used to estimate equilibrium tendency of a  chemical reaction. In general, oxidation states are written on  the left and reduction states are written on the right side of a  chemical equation:


Oxidation State + ne- ⇔ Reduction State


(1)Normally, H+/H2  is defined as Eo at 298 K (25o C) = 0.0 V.


2H+  + 2e- ⇔    H2   (Eo = + 0.000 V)


And then, Eo value for other chemical reaction will have a  relative value. If the Eo value in Eqn (1) is positive, the equilibrium tends to shift to the right, and if the Eo value in  Eqn (1) is negative, the equilibrium tends to shift to left. For exemple:


Au+   +  e- ⇔       Au  (Eo = + 1.68 V)


Fe2+ + 2e- ⇔       Fe (Eo = - 0.44 V)


In Eqn (3) Eo is positive (+1.68 V) and it tends to shift to the  right indicating that Au is difficult to corrode. While in Eqn


(4) Eo is negative and it tends to shift to the left indicating that  Fe is easy to corrode.


A Theoretical Model of Galvanic Corrosion (Al-Ti Cell)


Titanium (Ti) is transaction metal and its electronic configuration is: 1S22S22P63S23P64S23D2. Based on its electronic configuration, it may have possible oxidation states, namely Ti+, Ti2+ , Ti3+and Ti4+. Their Standard Electrode and  Redox Potentials, Eo at 298 K (25o C) are [3-4]:


Ti2+ +  2e- ⇔ Ti


Eo = -1.63 V


Ti4+ + e- ⇔ Ti3+Eo = -0.04 V


Ti3+ + e- ⇔ Ti2+Eo = -0.37 V


(7)TiO2+ +2 H++ e- ⇔ Ti3++ H2O Eo = + 0.10 V      (8)TiO2++2 H++  4e- ⇔ Ti  + H2O Eo = -0.89 V


[TiF6]2-+ 4e- ⇔ Ti    + 6F- Eo = -1.24 V


Cu2+   + 2e- ⇔ Cu


Eo = +0.34 V


Al3+  +  3e- ⇔ Al


Eo = -1.66 V


Based on the above Eo data, only high oxidation states of Ti3+ ,Ti4+(Eqn (6) and (7) are possible involved chemical reactions  of galvanic corrosion (Al-Ti cell). It is known that in galvanic  corrosion (Al-Cu cell) [1-2], the different of Eo value is about


2.0 V (Eqn (11) vs Eqn (12)). For high oxidation states of Ti3+and Ti4+the different of Eo value is about 1.62 V (Eqn (11) vs  Eqn (7)) and 1.29 V (Eqn (11) vs Eqn (7)). Therefore, the data  of electrochemical potentials show that it is  much possible to  have galvanic corrosion (Al-Ti cell).


The experimental results also support that high oxidation  states of Ti3+ , Ti4+  are possible involved galvanic corrosion (Al-Ti cell). In the experiments, after cross sectional polishing,the cross sectional sample was stained using the BOE(buffered oxide etch, NH4F/HF=13/2) solution. Cross sectional SEM results showed the  “crab-eye- ”like structures at the edge of the barrier metal as shown by the arrows in the  Figs 5-7. This means that Ti/TiN at the edge of the barrier  metal lines had oxidized into high oxidation states, which  couldn ’t react with BOE, but Ti/TiN at the center of the  barrier metal lines was still at low oxidation states, which was etched away by BOE solution during staining. Thus th ”e  crabeye- ”like structures were formed:


Ti/TiN (low oxidation states) + BOE ⇔ Chemical Reaction


(13)


Ti3+/Ti4+ (high oxidation states) + BOE ⇔ No Chemical  Reaction


(14)


Based on the above results, we can understand that at bondpad edge Ti/TiN has been oxidation into high oxidation  states, Ti4+/Ti3+ or Ti3+/Ti2+, which will form as a cathode, and  then Al3+/Al will form as an  anode. Therefore, we can  propose a theoretical model of galvanic corrosion (Al-Ti cell)as:


Anode:


Al3+  +  3e- ⇔  Al


Cathode:


Ti4+    +    e- ⇔ Ti3+


Eo = -0.04 V


(16)


Or/and


Ti3+    +    e- ⇔ Ti2+


Eo = -0.37 V


(17)


When bondpads are exposed to DI water or moisture (H2O)and oxygen (atmosphere) during wafer cleaning or wafer diesawing processes, galvanic corrosion (Al-Ti cell) may occur at bondpad edge.  O2 & moisture (H2O) may be involved in chemical reaction:


O2 + 2H2O + 4e ⇔ 4 OH-Eo =  + 0.401V


(18)


The new product OH-in Eqn (18) will react with Al and form  hydrated aluminum  hydroxide product:


4Al + 3O2 + 6H2O ⇔ 4 Al3+ +12 OH-⇔ 4Al(OH)3    (19)


During the cleaning process, corrosive product, Al(OH)3 may be cleaned away and a corrosive  “hole-like ”defect will be  formed at bondpad edge (Fig. 1).


Galvanic Corrosion (Al-Ti Cell) At Bondpad Edge


After studies, we have understood that galvanic corrosion (AlTi cell) only occurs at the bondpad edge with Ti/TiN/Al layers structure, while galvanic corrosion (Al-Cu cell) may occur at  both bondpad center and edge.


Galvanic corrosion (Al-Ti cell) may occur at both wafer fab  and assembly house. However, for most cases it occurred at  assembly house during/after wafer die-sawing/cleaning process. During/after wafer die sawing/cleaning processes, the  moisture (H2O) may be trapped at bondpad edge. From Eqn (18), moisture (H2O) will enhance corrosion at bondpad edge.


For example,  Figure 1 shows a galvanic corrosion (Al-Ti cell)case found in the assembly house. One can see that some  “hole-like ” defects were found at bondpad edge after wafer die sawing process.


TEM cross sectional photo showed that the  “hole-like ”defect had deeply into Al metal layer, which was damaged  about 50% of the metal thickness at bondpad edge (Fig. 2). While Figs 3-4 show another galvanic corrosion (Al-Ti cell)case. One can see that the  “hole-like ” defects had serious  damaged the bondpad edge. It is strongly believed that theses  defects were caused by both galvanic corrosion (Al-Cu cell) and galvanic corrosion (All-Ti cell).


Si dust was also found scattered around the corrosion area  “hole-like ”defects after wafer dicing.  We have performed  detailed studies connecting corrosion and Si dust, and proposed a theoretical model to explain why Si dust is often  concentrated around corrosion regions [5].


Figure 1: SEM micrograph showed a galvanic corrosion case  at the edge of bondpad after wafer die sawing process. A lot of  hole-like defects were formed


Figure 2: TEM cross section was done on a hole-like defect (Fig 1) and micrograph showed that the hole had deeply into  Al metal, which were damaged about 50 % at the edge of bondpad.


Figure 3: SEM micrograph showed another galvanic corrosion case at the edge of bondpad after wafer die sawing process. The  hole-like defects were formed at the edge of bondpad.


Figure 4: Close-up SEM micrograph showed the edge of  bondpad had been damaged seriously after wafer die sawing  process.


Figure 5: The cross sectional sample was stained using the BOE solution, the  “crab-eye- ”like structures were found.


This means that Ti/TiN at the edge of the barrier metal lines  had oxidized into high oxidation states  as it cannot react with  BOE.


Figure 6: Close-up of Figure 5 showed the  “crab-eye- ”like structures Ti/TiN layer


Figure 7: A diagram of bondpad structure showed Ti high  oxidation states at the edges of bondpad, which like the “crab-eye- ”like structure.


Elimination Solutions


After discussing the failure model of galvanic corrosion (Ai-Ti cell), we can understand that besides galvanic corrosion (AlCu cell), another galvanic corrosion (Al-Ti cell) may also  occur at bondpad edge with TiN/Ti/Al metallization structure.


Moreover, it is also known that moisture (H2O) may enhance  galvanic corrosion (Al-Ti cell). Therefore, in order to eliminate galvanic corrosion (Al-Ti cell), it is very important  to optimize a etch recipe to produce a good profile at bondpad  edge to prevent trapping moisture at the corner.


The possible solutions may be: (a). Optimize bondpad opening  etch process to get good profile at bondpad edge without  TiN/Ti footings. (b). Optimize etch recipe to control gauging  on Al bondpad. (c). Fully remove moisture (H2O) to prevent  galvanic corrosion (Al-Ti cell) at the bondpad edge. (d).


Grow up an Al oxide on bondpad & edge to prevent galvanic  corrosion. (e). Implement CO2 bubbling in DI water during  cleaning process to reduce OH- ions from galvanic corrosion(Eqn (18)). And (f) Use higher feed-rate (high sawing speed) to saw wafers so as to reduce DI water exposure time, and  optimizing sawing conditions such as DI water washing pressure, washing time, drying time and surfactant purge rate  etc [5].


A galvanic corrosion case at bondpad edge is studied.


Galvanic corrosion on microchip Al bondpads may be identified into two corrosion models: galvanic corrosion (AlCu cell) occurred mostly at the bondpad center [1-2] and


galvanic corrosion (Al-Ti cell) occurred specially at bondpad  edge with TiN/Ti/Al matellization structure. In this paper, a  theoretical model of galvanic corrosion (Al-Ti cell) is proposed to explain galvanic corrosion at bondpad edge. This  model can help us to understand chemically & physically  failure mechanism of galvanic corrosion at bondpad edge.


Both galvanic corrosion (Al-Cu cell) and galvanic corrosion(Al-Ti cell) had contributed to the  “hole-like ” defects at bondpad edge. Some possible solutions to eliminate galvanic corrosion (Al-Ti cell) are also discussed.


The authors would like to thank Material & Physical (TEM) FA team from Chartered Semiconductor Mfg Ltd, Singapore  for their technical contributions to this paper. Special thanks to  the Mentor for this paper from the Technical Committee of  ISTFA 2007 Conference for providing technical and professional advice.


[1]. Hua Younan, A Study on Discolored Bondpads &Galvanic Corrosion. The Proceedings from the 24th International Symposium for Testing and Failure Analysis, 15-19 Nov, Hyatt Regency, DFW-East Tower, Dallas, Texas, USA, 269-272  (1998).


[2]. Hua Younan, Low E. C., An L. H. and Shailesh Redkar, Failure Analysis and Elimination of Galvanic Corrosion  on Bondpads during Wafer Sawing. The proceedings from the 26th International Symposium for Testing and  Failure Analysis, Nov 12-16 2000, Meydenbauer Convention Center, Bellevue (Seattle), Washington, USA, 369-372 (2000).


[3].


“


”


Gu Guobang and Gu Yunli,  Inorganic Chemistry .


Chemical Industry publisher, China,  269-289, 368-374(1997).


[4].


Dalian Technology University,  Inorganic Chemictry- ”2 . Renmin Publisher, China, 180, 358-362 (1983).


[5]. Hua Younan, Zhao Si Ping, Mo Zhiqiang & Cho Jie Ying,Studies of Silicon Dust Corrosion on Microchip Al Bondpads and Elimination of Silicon Dust During Wafer  Sawing Process. The Proceedings of the 32nd International  Symposium for Testing and Failure Analysis (ISTFA  2006), Nov12-16 Nov, Austin, Texas, USA (2006).


Si3N4


SiO2 TiN Ti


Al oxide Ti high


oxidation states


(Ti3+/Ti4+)


Construction of a 3-D Current Path Using Magnetic Current Imaging


Frederick Felt, NASA Goddard Space Flight Center, Greenbelt, MD, USA  Lee Knauss, Neocera, Beltsville, MD, USA


Anders Gilbertson, Neocera, Beltsville, MD, USA


Antonio Orozco, Neocera, Beltsville, MD, USA


The need to miniaturize in the electronics industry  is driving smaller form factors, and resulting in  complex packaging innovations such as structures  with multiple devices stacked inside a three  dimensional package.  These structures present a  challenge for non-destructive fault isolation.


Two such modules recently exhibited failures on the  NASA Goddard Space Flight Center Solar Dynamic  Observatory (SDO) during board-level testing.  Each module consisted of eight vertically-stacked  mini-boards, each mini-board with a single  EEPROM microcircuit and capacitor, and  connected by external gold metallization to module  pins.  Both failed modules exhibited low-resistance  shorts between multiple pins.  The orthogonal  structure of the module prompted the use of  magnetic current imaging (MCI) in three planes in  order to construct an internal three-dimensional  current path for each of the failed modules.


Magnetic current imaging is able to “look through” non-magnetic, or de-gaussed packaging materials, allowing global imaging without physical  deprocessing of the stacked EEPROM modules, in  order to construct the internal current path and  localize defects.  To our knowledge, this is the first  time that this has been done.


Following global isolation of the defects, two types  of magnetic sensors were used in parallel with  limited deprocessing in order to more precisely  characterize suspect failure locations before  actually physically exposing the defects.  This paper  will show the process for using magnetic current  imaging with both SQUID and magnetoresistive (GMR) sensors to isolate defects in two stacked  EEPROM packages along with the final physical  analysis of the defects.


The failure analysis found that these devices were  damaged by external heat, possibly during oven  pre-conditioning or hot air soldering onto the board.  The manufacturer, 3-D Plus, was not implicated in  the failure.


An electrical short was discovered during a cardlevel safe-to-mate check of the C&DH S-Com  Assembly 1002Flt flight board, destined for  installation on the Solar Dynamic Observatory (SDO) satellite.   Electrical trouble-shooting found  that the low-resistance short disappeared when a  Vcc pin of a stacked EEPROM module was lifted.   The malfunctioning EEPROM module was  removed from the board and forwarded to the  NASA Goddard Space Flight Center for evaluation. The history of the part showed that the EEPROM  module was last powered at the manufacturer’s  location where it successfully passed all  qualification testing, including three-level  temperature testing.  Following delivery to a  NASA, subcontractor, the module was  preconditioned per manufacturer recommendation  for 24 hours at 125C in an oven with a ramp rate of  2C per minute, and then hand-soldered on the  1002Flt flight board following NASA standard  procedure.  Further investigation showed that the  part was one of a lot which had received a careful  pre-cap visual inspection by a NASA GSFC parts  engineer prior to encapsulation.  No internal defects  were noted during this inspection.


Following replacement of the faulty EEPROM  module, continued bench-level testing found a  second failure.  The C&DH S-Comm A flight board  failed the checksum test at room temperature.  Trouble-shooting found an electrical short of  approximately 2 ohms between an address line and


Vcc on a second EEPROM module.  This part was  removed from the circuit board and also forwarded  to the NASA GSFC Failure Analysis Laboratory for  examination.


For the purposes of this paper the first EEPROM  failure is designated, “Module 1”.  The second  device failure is designated “Module 2”.  This paper  reports on the failure investigation of these two  devices using magnetic current imaging to identify  the failure location by constructing a threedimensional current path inside the rectangular  devices.


Failure Analysis of Module 1


Examination of Module 1 in the GSFC Failure  Analysis Laboratory found no external evidence of  the failure.  Coordinate axes of the device were  chosen as shown in Figure 1 below.


Figure 1:  An external view of the EEPROM module shows  the coordinate axis used while performing orthogonal  magnetic current imaging.  These axes are used to define the  scanning planes in the body of the paper.


Radiography was performed on the module in three  orthogonal views: side, end, and top-down; as  shown in Figure 2.  For purposes of this paper the  top-down x-ray view shows the x-y plane of the  module.  The side view shows the x-z plane, and the  end view shows the y-z plane.


No anomalies were noted in the radiographic  images.  Excellent alignment of components on the  mini-boards permitted an uncluttered top-down


view of the mini-circuit boards.  The internal  construction of the module was seen to consist of  eight, stacked mini-boards, each with a single  microcircuit and capacitor.  The mini-boards  connected with the external module pins using the  gold-plated exterior of the package.  External  inspection showed that laser-cut trenches created an  external circuit on the device, which is used to  enable, read, or write to any of the eight EEPROM  devices in the encapsulated vertical stack.


Regarding nomenclature, the laser-trenched gold  panels on the exterior walls of the package were  labeled with the pin numbers.  The eight miniboards were labeled TSOP01 through TSOP08, beginning at the bottom of the package near the  device pins.


Figure 2:  Radiography, showing three orthogonal views of  the part, reveals internal construction of the module.


Pin-to-pin electrical testing confirmed that Vcc Pins  12, 13, 14, and 15 were electrically common, presumably through the common exterior gold  panel on the package wall.  Likewise, Vss Pins 24, 25, 26, and 27 were common.  Comparison to the xray images showed that these four pins funneled  into a single wide trace on the mini-boards.  All of  the Vss pins were shorted to the Vcc pins with a  resistance determined by the I-V slope at  approximately 1.74 ohms, the low resistance  indicating something other than an ESD defect.  Similarly electrical overstress was considered an  unlikely cause of failure as the part had not been


under power since the time it was qualified at the  factory.


The three-dimensional geometry of the EEPROM  module suggested the use of magnetic current  imaging (MCI) on three, or more flat sides in order  to construct the current path of the short within the  module.  As noted, the coordinate axes selected for  this analysis are shown in Figure 1.


Magnetic Current Imaging


Magnetic current imaging, as applied to fault  isolation in the semiconductor industry, is based on  the measurement of the magnetic field generated by  current carried in the structures of the device under  test (DUT).  The detected magnetic field is used to  map the current in the device by using a Fast  Fourier Transform back-evolution technique [1,2].  The resulting current map can then be compared to  a circuit diagram, an optical/infrared image, an xray, or a non-failing part to determine the fault  location.  As a tool for mapping electrical current in  electronic packaged devices, it was only recently  introduced to the semiconductor community in  1999 [2,3].  Since then, it has become a mainstream  tool for package-level fault isolation [4] and dielevel fault isolation [5-7].


For MCI applications on integrated circuits, magnetic fields are typically measured with a  SQUID (Superconducting Quantum Interference  Device) magnetic flux sensor or a magnetoresistive (MR) magnetic field sensor [8].  The primary  differences between these sensors correspond to  sensitivity and resolution.


SQUIDs are the most sensitive magnetic sensors  known [1], and for electronic fault isolation they are  typically designed to have field sensitivity around  20 pT (about 2 million times smaller than Earth's  magnetic field).  This allows one to scan currents of  500 nA at a working distance of about 400 microns.  As for all near field situations, the resolution is  limited by the scanning distance or, ultimately, by  the sensor size (typical SQUIDs are about 30 μm  wide), although software and data acquisition  improvements allow locating currents within 3  microns.  To operate, the SQUID sensor must be  kept cool (about 77 K) and in vacuum, while the


sample, at room temperature, is raster-scanned  under the sensor at some working distance z, separated from the SQUID enclosure by a thin, transparent diamond window.  This allows one to  reduce the scanning distance to tens of microns  from the sensor itself, improving the resolution of  the tool.


The best MR sensors are about 2 to 5 orders of  magnitude less sensitive than SQUIDs but they are  easier to scale down in size (below 100 nm) to  provide resolution less than 300 nm.  Although the  sensitivity is lower, the absence of an enclosure  allows one to bring the sensor closer to the circuit (scanning in soft contact mode) and thus, it has  magnetic sensitivity to map out sub-micron current  lines carrying as little as a few microamperes of  current [9,10].  This proximity along with the  smaller physical size of the sensor allows for  improved submicron resolution.


The typical MCI sensor configuration is sensitive to  magnetic fields in the perpendicular z direction (i.e., sensitive to the in-plane xy current distribution in  the DUT).  This does not mean that we are missing  vertical information; in the simplest situation, if a  current path jumps from one plane to another, getting closer to the sensor in the process, this will  be revealed as stronger magnetic field intensity for  the section closer to the sensor and also as higher  intensity in the current density map.  This way, vertical information can be extracted from the  current density images.  Further details about MCI  can be found elsewhere [8].


All MCI scans were taken with a Neocera Magma  C30 magnetic current imaging system with dual  SQUID and MR sensors.  This dual sensor built-in  capability allowed for quick, accurate registration  between magnetic scans (with either sensor) and  optical images of the scan area to physically locate  features detected in the magnetic/current density  images as presented in this paper [11].


Magnetic current imaging is a non-destructive  technology and little sample preparation was  required.  A super-conducting quantum interference  device was employed to detect and map the


magnetic field: scanning the side of the device with  gold panels connecting to the Vss and Vcc pins, in  the x-z plane.


The module was placed with this side up, on a  stable mount under the SQUID detector.  Because  magnetic current imaging is highly sensitive to  distance from a current path, the scan platform was  adjusted in order to level the top surface of the  EEPROM module prior to scanning.  Next, a  positive bias was applied to Vcc, which, due to the  low resistance of the short resulted in 0.71mA(rms) of alternating current at 5.3kHz, from Vcc to Vss.   A separation of approximately 100 microns was  maintained between the detector and the surface of  the gold-plated EEPROM module.  During scanning  the SQUID sensor remains in a fixed location, while  the scanning platform moves in incremental steps of  varying size, depending on the resolution required  and the time allowable for the scan.  The part was  de-gaussed to eliminate residual DC magnetism in  the Kovar leads of the module, which, in this  sample, were strong enough to saturate the sensor.     Figure 3 shows the first of several, orthogonal  images.  This current density map shows current  flowing in the  x-z  plane,  from external  pins to the


Figure 3:  A magnetic current image of the EEPROM module  in the x-z plane reveals current moving, undiminished, to the  TSOP08 level, and returning on the Vss panel to the external  pins.  This image is in the x-z plane.


gold Vcc panel on the side of the module, and then  progressing upward to the TSOP08 level where it


disappears.  Current reappears at the TSOP08 level  on the Vss gold panel, and moves downward to the  TSOP01 level where it transfers  to the external Vss  pins.  The current density map shows no current  loss along this path, on either the Vss or Vcc panels, thus isolating the fault to the top mini-board in the  EEPROM stack, TSOP08.


The part was rotated and magnetic current image  scanning was performed in the x-y plane at the top  of the EEPROM module.  The magnetic field map  overlay is shown in Figure 4.  Where the previous  magnetic current scan relied on current flowing  through the gold panels on the exposed outer  surface of the module, top-down magnetic current  imaging in the x-y plane demanded the capability of  detecting magnetic fields at a small, but important  distance—in the circuit board traces of  the TSOP08  mini-board.  This distance measures approximately


1.6 mm, or 1600 microns.


Figure 4:  An overlay of the magnetic field map on the top of  the module in the x-y plane shows that the null position of the  magnetic field approximately corresponds to the Vcc and Vss  traces leading to the errant capacitor in the preceding image.


Comparison of x-y plane magnetic field and current  density maps to the corresponding x-ray image, revealed that current entered at the Vcc mini-board  trace, the same location where it disappeared in the  x-z plane scan.  From there, current followed the  TSOP08 circuit board trace, passing under the  microcircuit and through the de-coupling capacitor  at one end of the module, and returning to the miniboard pin which connected to the external Vss  panel.  Obviously this result pointed toward failure


of the TSOP08 capacitor.  The x-ray image in  Figure 5 shows an overlay of the current density  map with SQUID thresholding turned on in order to  optimize current through the capacitor, the area of  particular interest.  Assuming that current was  constant along the entire circuit path, the higher  intensity of the magnetic field at the capacitor could  be due to one of two things: (1) either a change in  distance from the SQUID sensor or, (2) a necking  of the current path producing a locally stronger  magnetic field.


In this work we present the results for different VACC levels and doses but not for the other parameters like height of the inter  layer dielectrics, width and length of the transistor channel and  the gate oxide thickness.


To characterize the devices electrically at the contact level  before and after beam irradiation we assume that an AFM  based system does not change device parameters. This was verifie d by several measurements of a transistor after deprocessing the sample to the contact level. No change in  device characteristic could be observed after a series of measurements over a period of 2 days.


In the first step, a dependency of the device characteristics on SEM electron beam acceleration voltage (VACC) and electron


dose was investigated. To eliminate possible further influences  the VACC and D scales were obtained from a separate die with  the same preparation history and hILD across the SRAM cell  array.


The doses used were: 1.6·10-12As/µm2 (D1), 1.6·10-11As/µm2(D2), 9.3 ·10-11As/µm2 (D3), 4.7·10-10As/µm2 (D4), 2.8·10-9 As/µm2 (D5). The dose values were calculated by multiplying  electron beam current and exposure time divided by the  affected (scanned) area.


The doses cover the range from a “just exposed by accident”level over slow scans used for imaging, up to high dose levels ,i.e. high magnification coupled with long exposure time.


In the first experiment an acceleration voltage of 10kV was  chosen. This is a commonly used setting for standard top  down or cross section failure analysis tasks.


For the next experiments dose values were kept constant but  the VACC was decreased to 5kV and 1kV.


To have an in depth look at the cause of the device parameter  change, I-V characterization of the gate and source-drain regions as single components was performed. The goal was to  determine possible changes in gate leakage currents and  differences in the diode characteristics of the source-drain region to p-well.


Exposure of the nFET transistor at 10kV changes the device  characteristic immediately and drastically (Fig.1a and 1b). It is  clearly visible that even shortest exposure times (D1 equals 2s with a scanned area of 12x12µm2) lead to a significant change  in IL.


Besides the IL, all other transistor parameters are changed as well. With increasing dose the VTH shifts more than 300mV to  higher values and the ION decreases by a factor of 4.5. The  transistor slope S changed from 0.08V/dec up to 0.4V/dec for  the highest dose.


Transfer Characteristics (VACC=10kV)


1.E-14


1.E-13


1.E-12


1.E-11


1.E-10


1.E-09


1.E-08


1.E-05


UGate in V


initial D1


D2


D3


D4


D5


Fig.1a Input characteristics of the transistor at  VACC=10kV and different doses plotted in logarithmic scale.


0.E+00


2.E-05


3.E-05


4.E-05


5.E-05


6.E-05


7.E-05


8.E-05


Fig.1b Input characteristics of the transistor at  VACC=10kV and different doses plotted with a linear scale.


These facts are an important issue for standard SEM analyses  followed by nano probing device characterization. Compared  to a non-exposed reference transistor, it is most likely that a  single exposure of the electron beam on the target cell will lead  to significantly altered device characteristics caused by the  irradiation of the electron beam. Possible device failures might  become masked due to the strong effect of the electron beam  exposure.


In addition to the transistor I-V curves, gate leakage current to  the underlying pwell and diode characteristics of the sourcedrain region to pwell were obtained.


Comparison of gate leakage currents shows increasing leakage  values for higher doses D (Fig. 2). This might be due to gate  oxide degradation as a consequence of trapped electrons or  the creation of electron hopping paths due to the electron  bombardment.


Gate Leakage Current (VACC=10kV)


2E-11


3E-11


4E-11


5E-11


6E-11


7E-11


8E-11


9E-11


Dose in As/µm2


Fig.2 Increase of gate leakage with increasing dose of radiation.


Analysis of the source-drain region to pwell diode shows that  an increase in the applied dose affects the resistance and  leakage currents such that both values are increased (Fig. 3).


Source/Drain-pwell-diode (VACC=10kV)


1.E-15


1.E-03


-2.0 -1.5 -1.0 -0.5 0.0 0.5 1.0 1.5 2.0


Voltage in V


initial D5 D4 D3 D1


Fig.3 Resistance and leakage current of the source region to  pwell diode increase with a higher applied dose.


For the lower beam acceleration voltages used in our experiments these effects are reduced drastically.


Unfortunately it was not possible to avoid electron beam induced device characteristic change for all of the doses that were applied. For the worst case scenario (D5) device degradation could be observed even at VACC=1kV.


The trend charts are shown in Figs. 4a to 4d.


IL dependency from VACC and Dose


Dose in As/µm²


10kV


5kV


1kV


Resolution limit


Fig.4a Leakage current IL increases strongly with VACC and D.


VTH dependency from VACC and Dose


-0.10


-0.05


0.05


10kV 5kV 1kV


Fig.4b VTH decreases slightly for VACC=1kV and very small  doses at higher VACC. High doses and high VACC cause an increase of VTH.


Slope dependency from VACC and Dose


1.E-02


1.E-01


1.E+00


Fig.4c Slope S increases after electron beam irradiation. The  initial slope is 8 10-2V/dec.


ION dependency from VACC and Dose


-6.E-05


-5.E-05


-4.E-05


-3.E-05


-2.E-05


-1.E-05


Fig.4d ION  current decreases for10kV and 5kV VACC.


Additional measurements with time intervals of one week and  one month between exposure event and subsequent remeasurement of the transistor showed nearly no changes in  the electrical characteristics.


Our data confirm the effect of electron beam induced alteration  on integrated devices. It has been shown that several parameters influence the investigated device, e.g., beam acceleration voltage and dose used for radiation. It is also  shown that several device parameters are affected. Differences  in the unexposed transistor are evident for IL and ION as well as VTH and slope. While device leakage currents increase with  higher exposure, the ION values decrease. The VTH values shift  to higher values for VACC values of 5kV and 10kV if doses  higher then 1·10-11As/µm2 are applied. Otherwise (VACC=1kV or  D1 applied) the VTH shifts to smaller values.


There are several publications available explaining the effects  seen in our experiments [5, 6, 7, 8]. All of the explanations  propose two main contributors to the device alteration.


The first one is  trapped charge located in the gate oxide. The  positive charge up of the gate should lead to a shift of VTH in  negative direction. This seems to be the dominant mechanism for older CMOS technology nodes [9].


The second contributors are electrons trapped in interface states . From our data it appears that  for 10kV and 5kV accele ration voltages, this is the main culprit responsible for  changes in device characteristics. For VACC=1kV, VTH slightly  decreases , indicating that the effect of the trapped gate oxide  charge is dominant. From our point of view it might also be possible that charge is trapped in the interlayer dielectric. That  would explain the different behavior at VACC=1kV. With the  much shallower penetration depth at these low energies, the  electrons are only trapped in the ILD, and do not reach GOX or  bulk to GOX interface.


A decrease in ION currents might be also explained by an  increase of the resistance of the source drain regions either to the underlying nwell or to the connecting source-drain contact. Diode characteristics of the source drain contacts to the nwell  support this hypothesis.


In conclusion and as an answer to our initial questions it is  possible to state that measurements with our available SEM  based prober are possible, but under certain SEM conditions,i.e., low VACC and low doses. Only under these conditions, the  electron beam influence on electrical device parameters such as ION, IL, and S is negligible in most failure analysis cases . Special  applications like signal margin fails due to slightly misaligned  VTH values of two transistors in the sense amp lifier require a  reliability to VTH values better then 20mV. In this case it is  important to operate the SEM at low accelerating voltages and  simultaneously limit the dose applied to the device.


Our studies also show that it is critical to know the sample  history before electrical device characterizations are carried out since electron beam induced device parameter changes are  nearly unaltered over a long period of time after beam exposure.


[1] Takayuki Mizuno, Miho Takahashi, Yoshie Azuma, Hiroshi Yanagita, Kyoichiro Asayama, Koji Nakamae, proceedings, 45th Annual International Reliability  Physics Symposium, Phoenix, 2007


[2] M. Gruetzner, Microelectronics Reliability Vol. 45 (2005) pp. 1509-1513


[3] R. Mulder, S. Subramanian, T. Chrastecky,proceedings, ISTFA 2006, p 503


[4] C. Giret, D. Faure, proceedings, 11th IPFA 2004, p271


[5] W. Weber, R. Thewes, Experimental Methods for Investigating the Defect Properties of SiO2 in Metal  Oxide Semiconductor Transistors, J. Electrochem.


Soc., Vol. 145, No. 10, p 3638, 1998


[6] S. Shabde, A. Bhattacharyya, R. S. Kao, R. S. Muller, Analysis of MOSFET Degradation Due to HotElectron Stress in Terms of Interface State and FixedCharge Generation, Solid-state Electronics, Vol. 31, No. 11, p. 1603, 1988


[7] Jong-Son Lyu, Kee-Soo Nam, Choochon Lee,Determination of the Interface Trap Density in Metal  Oxide Semiconductor Field -Effect Transistor through  Subthreshold Slope Measurement, Jpn. J. Appl.


Phys., Vol. 32, p. 4393, 1993


[8] P. J. McWhorther, P. S. Winokur, Simple Technique for Separating the Effects of Interface Traps and  Trapped Oxide Charge in Metal-oxide-semiconductor Transistors, Appl. Phys. Lett., Vol. 48, p. 133, 1986


[9] S. Goerlich, Elektronenstrahltesten passivierter integrierter MOS-Bausteine. Fortschritt-Berichte VDI, Reihe 9, NR. 61, Düsseldorf: VDI-Verl., 1986-ISBN 3-18-146109-1


Combining the Nano-Probing Technique with Mathematics to   Model and Identify Non-Visual Failures


Cha-Ming Shen, Tsan-Chen Chuang, Shi-Chen Lin, Lian-Fon Wen, Chen-May Huang


1,Nan-Ke North Rd., Tainan Science Park, Tainan, Taiwan, R. O. C


In this paper, we focus on how to identify non-visual failures  by way of electrical analysis because some special failures  cannot be observed by SEM (scanning electron microscopy) or TEM (transmission electron microscopy) even when they  are precisely located by other analytical instrumentation or are  symptomatic of an authentic or single suspect. The  methodology described here was developed to expand the  capabilities of nano-probing via C-AFM (conductive atomic  forced microscopy), which can acquire detailed electrical data, and combining the technique with reasoned simulation using  various mathematic models emulating all of the significant  failure characteristics. Finally, a case study is presented to  verify that such defect modes can be identified even when  general PFA (physical failure analysis) cannot be  implemented for investigating non-visual failure mechanisms.


With the evolution of advanced process technology, failure  analysis has become more and more difficult because there are  more erratic defect types arising from more non-visual failure  mechanisms. For overcoming such difficulties in failure  analysis, nano-probing can be enhanced in order to acquire  more detailed electrical information before the implementation  of PFA (physical failure analysis) [1].


In this paper, we focus on how to solve non-visual failures  which cannot be observed by SEM or TEM even if they have  been located by nano-probing via C-AFM and an authentic or  single suspect was indicated via measuring and electrical  analysis. In order to overcome the difficulties of failure  analysis for such non-visual failures, a mathematic model for  specific failure simulation is proposed to explain those  characteristics impacted after electrical measurement data is  extracted by nano-probing.


Case Study and Experimental


In order to explain our methodology and the related  mathematical modeling, a typical single-side, blocked LDD (lightly doped drain) implantation case study is presented to  demonstrate our novel method for applying electrical analysis  to identify non-visual failures. This case study is chosen


because the LDD implantation issue is notorious as a chronic  problem for PFA experts.


First, let’s begin with the measured data from the nanoprobing of a failed transistor. As shown in Fig. 1, the failed  transistor exhibits a smaller saturation current and an  asymmetric behavior between the forward and reverse biased  I-V curves.


Figure 1: Comparison of forward (F) / reverse (R) Id-Vg  curves for a reference and a failed NMOS when VD=VG=1.2V. Note the smaller drift current and asymmetrical behavior of  the failed transistor test sweeps.


Because of the smaller drift current, a high-resistance issue  was the first idea to arise as a cause. But, considering the  inconsistent junction characteristics at both the drain and  source of the failed NMOS, there was no obvious difference  in the slope of the forward bias and this cause can be excluded (Figs. 2 and 3).


Figure 2: Quasi C-AFM I-V curve to check the junction  characteristic at the drain/source of the failed NMOS. indicating no high-resistance issues at the drain/source.


Figure 3: A typical high-resistance issue at the drain/source  was verified by a quasi C-AFM I-V curve. (Please notice the  forward-bias part of the I-V curve.)


Following this, the related implantation issues, which may  impact the carrier intensity of the source/drain or the threshold  dose of the channel, were highly suspect. Accordingly, based  on our previous study of such non-visual implantation issues


[2], these I-V curves and the unusual P-N junction  characteristics could be produced and explained by the “ideal  diode equation” and the “theory of the junction”.


The ideal diode equation is given by:


)1


/ −


kT


qV


J


L D


where


I    reverse saturation current


J   reverse saturation current density


A    interface area of P-N junction :


V    applied voltage


D   diffusion constant of hole


L    diffusion length for hole


:   N+ donor doping concentration


DN


D   diffusion constant of electron


nL    diffusion length for electron


:   PW accepter doping concentration


AN


in     intrinsic concentration


First, considering the above equations, since the value of the  delta of the reverse saturation current density, ∆JS, is inversely  proportional to the N+ doping concentration, ND, if the PW  concentration, NA, is kept constant then the leakage current of  this P-N junction is commensurate with the reverse-biased  current, ∆IS, and it should increase as the N+ implant  concentration decreases accordingly. But considering the  inconsistent result of the corresponding C-AFM measurement, there was neither larger leakage current when reverse biased  nor a smaller cut-in voltage when forward biased. Thus, the  suspected N+ implantation issue can also be excluded (Figs. 2  and 4).


Figure 4: Typical N+ implantation issue at the drain/source  was verified by a quasi C-AFM I-V curve. (Please notice the  off-state current on the reverse-bias side and the cut-in  voltage of the equivalent diode on the forward-bias side )


Consequently, after more deduction, a blocked LDD  implantation was the most reasonable failure mechanism that  fit our reasoning. (Fig. 5)


(a). Failed NMOS


(b). Reference NMOS


Figure 5: Comparison of the dopant profiles of a blocked  LDD implantation and a reference NMOS.  A conductance  channel under the gate would be disconnected at the  drain/source site.


Next, for satisfying the previous deduction due to the lack of  physical evidence, the equivalent mathematic models were  applied to describe the corresponding electrical I-V curves of  the target MOS (metal-oxide-semiconductor) transistor. (Figs. 6 and 7)


Figure 6: The missing LDD at the drain can be modeled as a  smaller resistor because of a masked effect in the depletion  region.


Figure 7: The missing LDD at the source can be modeled as a  larger resistor because there are dual voltage drops in both  the disconnected implantation region and the pinch-off site.


In most applications, more determinable electrical analysis for  the corresponding mathematical models would consider  specific theories or characteristic equations from  semiconductor physics. Thus, with a view to MOS  technology, the ideal equation for drift current operated in  linear and saturation regions can be described as follows.


If


V −≤   ,


(2[


OX


= µ


V −≥


V    Drain-Source voltage difference


GSV   Gate-Source voltage difference


thV     threshold voltage of MOS


I     drift current of MOS


C  Gate capacitor of MOS


W    channel width of MOS


L    channel length of MOS


Considering that the MOS behavior of such a failure mode  was related to a body effect and the source voltage, the  threshold voltage of the transistor should become:


Ψ


sb


V γ


thV    threshold voltage


tV    threshold voltage without body effect


sbV    Source-Body voltage difference


Then, let’s insert a single-side blocked LDD failure, the VGS  part would vary with the failure located site and the VDS part  would divide as:


1D


V   voltage drop at the disconnected LDD :


V   voltage drop at the channel


DV   voltage drop at the pinch-off site


In general operation, the forced VDS is equal to the biased VD  and the forced VGS is equal to the biased VG. But according to  previous hypothesis, VDS was only the parts of VD2 and VD3, and VGS was a variable dependent on such blocked LDD  implantation impacted on the drain or source site.


Therefore, according to the corresponding mathematic models  and representative equations, the resulting numerical analysis  illustrates how such a failure mechanism can affect the  abnormal NMOS characteristics and induce an asymmetrical  behavior on the malfunctioning transistor (Figs. 8 and 9).


Figure 8: According to the above equations, if the missing  LDD is at the drain site, an increasing ID would cause a  decreasing VDS and make the linear region of the MOS expand  to all ranges.


Figure 9: According to above equations, if the missing LDD is  at the source site, although the pinch-off condition could be  forced along, the dual shrinking factors of VGS and VDS still  result in a very small drift current for the MOS.


Finally, some related PFA images are presented to validate  our ratiocination and methodology. The discovered failures  suffering from the non-visual implantation issue was verified  by visual residual particles or associated artifacts from the  wafer process although physical essence of the blocked LDD  implantation was still non-visual via TEM observation. Thus, the application by means of electrical analysis that combines  the nano-probing technique with mathematic modeling was


demonstrated to be an effective tool for identifying non-visual  implantation issues and other related, unperceivable defect  modes. (Fig. 10)


Figure 10: A typical example of an LDD implantation issue  which was verified as a residual particle or visible artifact  from the wafer process although the actual missed  implantation region was non-visual to SEM and TEM.


At present, the nano-probing technique is a powerful tool for  electrical characterization of a device. In this paper, the  utilization of nano-probing was enhanced in order to acquire  more complete electrical information before conducting  definitive PFA. Also, the LDD implantation issue could be  explained by exclusive methodology and mathematical  modeling. Finally, the application of numerical analysis can  be used to illustrate the impacted characteristics of the MOS.


[1] Cha Ming Shen, Tsan Chen Chuang, Chen May Huang, Shi Chen Lin, and Jie Fei Chang,   "Coupling C-AFM  with Nano-probing Technique for Further Junction  Leakage Analysis", ISTFA 2006, pp. 167 - 171.


[2] Cha Ming Shen, Shi Chen Lin, Chen May Huang, Huay  Xan Lin, and Chi Hong Wang,   "Couple Passive Voltage  Contrast with Scanning Probe Microscope to Identify  Invisible Implant Issue", ISTFA 2005, pp. 212 - 216.


Analysis of DC Failure in Advanced Memory Devices Using Nanoprobing and  Scanning Capacitance Microscopy


Jen-Lang Lue, Chin-Shun Lin, Atup Chiou, Hsuen-Cheng Liao, Hsienwen Liu, Brian Pai,  Sam Fan and Tings Wang


ProMOS Technologies Inc., Hsinchu, Taiwan, R. O. C. Jen-lang_lue@promos.com.tw


This paper discusses the failure analysis process of a DC  failure using an in-FIB (Focused Ion Beam) nanoprobing  technique with four probes and a scanning capacitance  microscope (SCM) in advanced DRAM devices. CurrentVoltage (I-V) curves measured by the nanoprobing technique  indicate the curve of the failed device is different from that of  the normal device. The failed device causes a high leakage  current in the test. The cross-sectional 2-D doping profile of  SCM verifies the region of the P-Well has shifted to create a  leakage path that causes this failure.


The DC test that is used to detect the external functionality of  modern memory chips is one of the testing sequences during  electrical testing of memory in wafer sorting. The output  leakage current can be measured by applying appropriate DC  voltages to each pin. Figure 1 is a schematic diagram showing  the output leakage current that is measured in the test. To start  this test, all the I/O pins are set at floating status. Then the  voltages of VDDmax and ground (GND) are applied to two  power supply pins, VDD and VSS, respectively. The output  leakage current can be measured by applying the voltages of  VDDmax or 0 to each of the output pins (DQ), while all other  pins are grounded. If the pin is applied to the voltage of  VDDmax, the leakage current measured is called an “ILOH”.  If  the pin is applied with the voltage of 0, the leakage current  measured is called an “ILOL”. Once the value of the measured  leakage current is out of production specification, the chip is  scrapped for further operations.


A nanoprober combined with either a scanning electron  microscope or a focused ion beam system is used for electrical  characterization of integrated circuit for failure analysis or for  testing device quality in the semiconductor industry [1]. In  general, incorrect implantations will cause the failures in  semiconductor devices. As is well known, scanning  capacitance microscopy (SCM) allows for the visualization of  the 2-D implantation doping profiles in actual semiconductor  devices [2-3]. Therefore, once a failure site location of the


specific device is confirmed by the nanoprobing technique, further SCM analysis can be employed to identify the physical  causes on the device structures.


In this paper, we describe the failure analysis process which  combines an in-FIB nanoprobing technique with SCM by  using a specific case with advanced memory devices. The  device that is failed due to a high output leakage current in the  DC test is confirmed by nanoprobing for further verification  of the physical cause by SCM.


VDD


VSS


GND


or 0


CHIP


(0)


VDD max


VDD (VDD max)


VSS (0)


ILOH ILOL


VDD max or 0 VDD max


Figure 1: A schematic diagram showing the output leakage  currents that are measured in the test.


Problem Description and Failure Analysis


In our specific case, one advanced 512 Mega-bit DRAM  wafer was failed due to a high output leakage current (ILOH) in  the DC test of the final production test. The WAT (wafer  acceptance test) data on the test structure that monitors the  electrical characteristics of low Vt (threshold voltage) PMOSFET (PMOS) in the SA (sense amplifier) circuit showed  the measured Vt is out of specification. Although the failure in  the SA circuit did not contribute to that in the output circuit, analysis of the failure in the SA device was done to  understand if there is any hint for the failure of the output  circuit.


There are two PMOSs designed in the test structure for low Vt  PMOS of SA. The WAT data indicated that one PMOS has  failed, but another one is normal. This information provides a  comparison between the normal device and the failed device  for further nanoprobing and SCM analysis.


Nanoprobing was employed in a FEI FIB 200 system with a  Kammrath & Weiss prober-module. The SCM images of the  2-D doping profiles of the desired device structures were  obtained using a commercial DI-3100 Atomic Force  Microscope (AFM) equipped with a SCM application module. A 0.5V AC bias at 90 KHz and a 0.0V DC bias between the  conductive tip and the sample were used for this analysis.


The failed chip was polished to the contacts level for the  source (S), drain (D), gate (G) and bulk (B). The probing tips  were then applied to the contacts. The source voltage, the  drain voltage and the bulk voltage were set to simulate test  conditions of WAT. The ID – VG curves of the normal and  failed devices were then measured by ramping down the gate  voltage from 0.5 V to -2.0 V (Fig. 2). The curve of the failed  PMOS device has shifted to the right side of that of the normal  PMOS device. The failed device has a high current at a lower  gate voltage. This result indicates that there is a leakage path  in the regions of source or drain.


-4.0E-04


-3.0E-04


-2.0E-04


-1.0E-04


0.0E+00


1.0E-04


-2.0


VG (V)


Normal device Failed device


Figure 2: I-V curves showing the differences between the  normal device and the failed device.


Figure 3 shows the cross-sectional SCM images of the normal  and failed PMOS devices. The drain region is isolated by STI (shallow trench isolation) from the region of the P-Well in the


normal device. However, the region of the P-Well bridges the  drain region in the failed P-MOS device that causes a leakage  path of high current in the electrical test. This abnormality is  caused by the shift of the photo mask on the implantation of  the P-Well during the manufacturing process.


Figure 3: Cross-sectional SCM dC/dV phase images showing


(a) the drain region is isolated by STI from the region of the  P-Well in the normal device, (b) the drain region bridges the  region of the P-Well in the failed device.


Figure 5:  A magnetic current image overlay on an x-ray  image of the EEPROM module.  Thresholding was used to  show only the strongest current at the capacitor of the  TSOP08 mini-board.  Arrows indicate Vcc and Vss pins.  This  image is in the x-y plane.


With the defect likely located in the TSOP08  capacitor, the module was rotated again in order to  perform an MCI scan in the y-z plane, on the end of  the module close to the errant capacitor.


The magnetic current map overlay in Figure 6  clearly shows current climbing up the Vcc terminal  of the capacitor, and moving along an indistinct  path, apparently across the top of the capacitor to  the Vss terminal, where it descends to the minicircuit board, makes a small translation, and  disappears into the depth of the module.


This interesting result led to a decision to lap the  end of the module, stopping before harming the  capacitor, then repeating magnetic current imaging  using a GMR sensor.  The result shown in Figure 7, and on an x-ray overlay in Figure 8, produced a


high-resolution current map, which confirmed the  previous finding that current ascended the Vcc  termination  of the capacitor,  then moved along,  or


Figure 6:  An overlay of the SQUID current density map on a  photo of the module end appears to show current climbing  from the TSOP08 circuit boar and traversing through the  upper section of the capacitor.  This image is in the y-z plane.


Figure 7:  An overlay of the GMR current density map on the  lapped end of the module.  Current traversed at, or near, the  top of the capacitor.  Use of GMR and reduced distance  resulted in better resolution on the current map.  This image is  in the y-z plane


Figure 8:  An overlay of the GMR current map on an x-ray  image of the part shows current moving through the minicircuit board and capacitor.  The diffuse path at, or near, the  top of the capacitor suggests that current was distributed in a  thin sheet.  This image is in the y-z plane.


very near the top of the capacitor before   descending on the Vss termination.  It was  interesting to note that the current moving between  the capacitor terminations appeared diffuse, suggesting that the shorting path was a sheet-like  structure in the x-y plane, oriented edge-on in this  y-z scan.


A similar procedure was performed on the top of  the module.  The encapsulation was carefully  lapped to a level close to the top of the capacitor in  order to reduce the distance between the MCI  sensor and the current path.  This time, magnetic  current imaging was performed using a GMR  sensor for higher resolution.


The resulting current map seen in Figure 9 again  indicated that the defect was a sheet-like structure, necked on one end near the Vss capacitor  termination.  This result was initially disappointing  as it was considered likely that the short was due to  a crack in the capacitor and a short between  adjacent electrodes.  However, removal of the  remaining encapsulation above the errant capacitor  showed that the GMR scan was exactly on the  mark: a very flat, necked ribbon of metal, apparently solder, connected between both  terminations of the capacitor creating a lowresistance shorting path across the device; shown as


first seen in Figure 10, and fully revealed in Figure


Figure 9:  An overlay of the GMR current map on the optical  image shows current in blue; high points of the exposed   terminations in orange.  Current, shown in blue in this image, appears to move in a necked sheet between Vss and Vcc.  This  image is in the x-y plane.


Figure 10:  A low-power optical view of the capacitor with  thinned encapsulation partially removed reveals a flat ribbon  of solder connecting between Vss and Vcc terminations, exactly in the location predicted by magnetic current imaging.  This image is rotated 90 degrees CW from the preceding  image.  Note that the shape of the ribbon agrees with the  predicted shape in Figure 9.  This image is in the x-y plane.


Figure 11:  A full view of the top of the failed capacitor  reveals a ribbon of solder between terminations.  The shape of  the ribbon conforms closely with the GMR magnetic current  map seen in Figure 9.  This image is in the x-y plane.  The y-z  lapping plane used in the GMR scan of Figures 7 is seen  edge-on at bottom of this image.


Subsequent failure analysis determined that the  stacked EEPROM module had experienced thermal  stress, possibly during oven condition or hot-air  soldering by a subcontractor, sufficient to melt  solder on the capacitor terminations and cause  expansion of the encapsulant material, allowing  liquid solder to migrate through a low tunnel  created between the capacitor and the encapsulant, resulting in a low-resistance short between Vss and  Vcc and causing the failure of the stacked  EEPROM module.


Failure Analysis of Module 2


Examination of Module 2 in the GSFC Failure  Analysis Laboratory also found no external  evidence of the failure.  This device exhibited a  common short between Pins 11 through 16.  Pin 11  is identified as Rbusy, Pins 12 through 15 represent  Vcc, and Pin 16 is an address pin, A15.  The failure  of this device was first reported as an anomaly on  the address pin.


Following external inspection and radiography the  part was prepared for magnetic current imaging in  the same manner as Module 1.  However, as seen in  Figure 12, initial scanning in the x-z plane on the  module side with the shorted pins revealed that  current moved from the external Vcc pin to the Vcc


gold panel, and then proceeded a short distance to  the TSOP01 level, where it transitioned into the x-y  plane of the mini-board—an unexpected, but  interesting result.  Likewise, current exited the  mini-board at the TSOP01 level and proceeded  down the Vss panel to the Vss pin.


Figure 12:  A magnetic current image in the x-z plane on  Module 2 shows the current path ending at TSOP01.  This  image is in the x-z plane.


The part was rotated to the x-y plane, with pins up, for the next scan.  The SQUID sensor was able to fit  between the two rows of pins, but its motion and the  resulting area scan were restricted.  The distance  between the sensor and the TSOP01 circuit board  was augmented by the encapsulant required to mold  around the pins which curved inside the encapsulant  to the external gold panels.  Nevertheless magnetic  current imaging using a SQUID sensor produced a  rough map which showed the current path moving  in the x-y plane approximately mid-way across the  EEPROM module to a discontinuity in the current  path about equally distant from both sides and one  end of the part.


In order to improve resolution, the external leads of  the device were lapped off.  This reduced the  distance to the current path in the TSOP01 level and  eliminated stray interference from magnetic fields  native to the Kovar pins.  Gold wire bonds were  attached to the external gold panels in order to  provide current to the short.  This resulted in the


ideal situation of being able to perform a scan of the  entire device in the x-y plane, with the input current  attached to the end of the gold panels, about 12mm  distant from the sensor, and beyond range of  interference with the SQUID.


The current density map in Figure 12 shows the  current path in the x-y plane, entering the module at  Pin 11 and exiting at Pin 16.  Scanning was  repeated, with pins reconnected to show the current  path between Pin 16 and Vcc.  Comparison of the  two current density maps on an overlay of the x-ray  image confirmed a shorting location under the  microcircuit.  The suspect short location was  scanned at high-resolution using a GMR sensor.


The EEPROM module was mounted on a plastic  dummy block, cut through the TSOP03 level, and  lapped to the top of the TSOP01 level, isolating the  TSOP01 level in order to perform radiography  without interference from the other boards in the  EEPROM stack.  The resulting high-resolution xray imaged revealed a mass of high-density material  connecting between the circuit board traces for Pin  16, pin 11, and Vcc.  Inspection showed that solder


Figure 13:  A magnetic current image in the x-z plane on  Module 2 shows the current path ending at TSOP01.  A  possible discontinuity is seen at upper right.  This image is in  the x-y plane.


Figure 14:    A GMR magnetic current map in the x-z plane on  Module 2 shows the current path diverting from the circuit  board traces through a high-density mass, likely melted  solder.  The disturbance in the current path at upper left is  due to capacitance between traces on opposite sides of the  mini-board.  This image is in the x-y plane.


had melted off the microcircuit pins and moved  along the circuit board traces, pooling at  delaminations where the three traces were shorted  together.  An overlay of the GMR current density  map on the x-ray image in Figure 14 shows an exact  match with the defect location.


Deprocessing of this part revealed thermal damage  to the capacitor on the TSOP08 level, as well as the  TSOP01 level.  Inspection of the capacitors  revealed extensive melting of solder on the  terminations in addition to the radiographic  evidence which showed apparent solder which had  flowed from the microcircuit pins and pooled  between adjacent circuit board traces—resulting in  the actual short and failure of the module.  These  findings led to the conclusion that the part had  experienced a thermal stress sufficient to melt  solder, likely due to either thermal conditioning of  the part prior to installation on the board, or  shrouded, hot air soldering of the part.  The  evidence did not point to a manufacturing problem.


Magnetic current imaging using both SQUID and  GMR sensors was performed in orthogonal planes  on the rectangular sides of two stacked EEPROM  modules.  This is the first time, to our knowledge, that magnetic current imaging has been applied to


three-dimensional packaged devices in order to  construct the internal current path within each  device and isolate defect locations.  Magnetic  current imaging was critical in both of these  analyses, as x-ray imaging was unable to reveal any  defects, and traditional failure analysis techniques  were deemed laborious and risky.  Magnetic current  imaging has proved itself to be a valuable technique  for non-destructive fault isolation in complex  electronic devices.


[1] J. P. Wisko, SQUID sensors: Fundamentals, Fabrication and Applications, Chapter The Magnetic  Inverse Problem for NDE, pages 629-695, Kluwer  Academic Publishers, The Netherlands, 1996.


[2] E. F. Fleet et al., HTS scanning Microscopy of  Active Circuits, IEEE Transactions on Applied  Superconductivity, 9 (2): 4103 (1999).


[3] L. A. Knauss et al., Detecting Power Shorts from  Front and Backside of IC Packages Using Scanning  SQUID Microscopy.  In Proc. of the 25th Int'l Symp. on  Testing and Failure Analysis, page 11, Santa Clara, CA, November 1999.


[4] R. Dias et al., Integration of SQUID Microscopy into  FA Flow. In Proc. of the 27th Int'l Symp. on Testing and  Failure Analysis, Santa Clara, CA, November 2001.


[5] D. P. Vallet. Scanning SQUID Microscopy for Die  Level Fault Isolation. In Proc. of the 28th Int'l Symp. on   Testing and Failure Analysis, pages 391-396, Phoenix, AX, November 2002.


[6] L. A. Knauss et al., Advances in Scanning SQUID  Microscopy for Die-Level and Package-Level Fault  Isolation. Microelectronics Reliability, 43:1657-1662 (2003).


[7] A. Orozco et al., Fault Isolation of High Resistance  Defects using Comparative Magnetic Field Imaging. In  Proc. of the 29th Int'l Symp. on Testing and Failure  Analysis, pages 9-13, Santa Clara, CA, November 2003.


[8] L. A. Knauss et al., Current Imaging using Magnetic  Field Sensors. Microelectronics Failure Analysis Desk   Reference 5th Ed., pages 303-311 (2004).


[9] B. D. Schrag, et al., Scanning Magnetoresistance  Microscopy for Die-Level Sub-Micron Current Density  Mapping. In Proc. of the 29th Int'l Symp. on Testing and  Failure Analysis, pages 2-5, Santa Clara, CA, November


2003.


[10]  S. I. Woods, A. Orozco, and L. A Knauss, Advances in Magnetic Current Imaging for Die-Level  Fault Isolation, EDFA Vol. 8, No. 4, pages 26-30 (2006).


[11]  F. S. Felt, Analysis of a Microcircuit Failure using  SQUID and GMR Current Imaging.  In Proc. of the 31st  Int'l Symp. on Testing and Failure Analysis, San Jose, CA, November 2005.


Investigation of Bond-Pad Etching Chemistries for Determination of  Probe/Bonding Related Sub-Pad Cracks


Valentina Korchnoy


Intel Israel (74) Ltd. P. O. Box 1659, Haifa 31015, Israel   Email: valentine.korchnoi@intel.com, tel: 972-4-865-5818


Bond-pad integrity directly affects the performance of  microelectronic devices. Bond-pad cracking and the related  sub-pad cracking of Inter-Metal Dielectric (IMD) may  introduce a high reliability risk and cause units to fail at  environmental stress. Bond-pad cracks may be initiated by  probing during wafer sort and the wire bonding process  during assembly. This paper presents a comparative analysis  of the various chemistries used for exposure and decoration of  pad cracks. The investigation showed that a tri-iodine etch  provides clean and artifact-free exposure of the TiN barrier  layer of the pad and is the best (of the methods tried herein) for pad crack observation.


Wire bonding is the former, however, still very common  method for connecting the pads on a chip to those on the  package. The most widespread is gold wire ball bonding to the  aluminum chip bond pad by thermocompression or  thermosonics [1]. The major issue in establishing high-quality, reliable wire bonding is process control of variables such as  bonding temperature and loads during assembly. Some  additional reliability risk may be introduced by pad probing  during wafer sort. The most common bond integrity related  reliability problems for the Au ball/Al pad system are: InterMetallic Compound (IMC) formation and sub-pad cracks in  IMD layers [2].


Wire bond characterization is an essential part of process and  quality control. Post-bonding visual inspection performed  according to the MIL-STD-883 METHOD 2010 spec can  detect pad cracks and other wire bonding quality problems. In  addition, two types of process tests are used today – the wirepull test and the ball-shear test. However, when the chip is  encapsulated, the above mentioned methods aren’t applicable. Non-destructive analysis, such as scanning acoustic  microscopy, usually cannot detect sub-pad cracks if the cracks  are small, and layer delamination is absent. For reliabilityrelated wire-bonding problem analysis two approaches can be  applied. The first approach is based on the mechanical  polishing of metallographic cross-sections of a pad. However  the polishing process applies some mechanical force to the  bond pad, which may cause artifact crack formation or


smearing of soft metal materials. Cross-sectioning by Focused  Ion Beam (FIB) [3] overcomes this problem, however, it is  time-consuming and provides only limited statistics, since  only a limited number of bonding connections can be  examined.


The second approach includes pad exposure followed by pad  selective etch to examine sub-pad areas for barrier and IMD  cracks. Usually this method causes lose of IMC layer  information, however, it has been considered the best for subpad IMD cracks exposure, because all bonding connections  across the die can be exposed and examined simultaneously. As reported in the literature [4], [5], the most common  enchants for Au ball/Al pad etch are: aqua regia, KOH, cyanides, halogens, and hot phosphoric acid. In general, the  procedure is based on a high etch selectivity between the Au  ball/Al pad and the underlying TiN (or TiW) barrier sublayer. In this way, Au balls are etched (or stripped out) together with  Au/Al IMC and Al pads, exposing the TiN (TiW) barrier for  optical or SEM inspection. The main problem here is to  distinguish between cracks introduced by probing / bonding, and artifact cracks potentially caused by the etching process. The current paper presents a comparative analysis of the  various chemistries used for exposure of sub-pad cracks. The  investigation shows that the tri-iodine etchant provides clean  and artifact-free exposure of the TiN barrier layer of the pad  and is the best (of the methods tried within) for pad crack  observation.


Experiment


The method is developed on a plastic-encapsulated device  fabricated by 0.18 μm CMOS technology. The gold wire is  ball-and-wedge bonded by thermocompression on aluminum  bond-pads with an underlying TiN barrier sublayer.


This investigation was initiated by the failure analysis of  several units that supposedly suffered from Circuit Under Pad (CUP) cracking related to pad over-stress as a result of the  wire-bond process. This may bring the reliability risk and  cause the units to fail at environmental stress. Further  investigation shows that the units start to fail after Life Test (LT) and Temperature Cycling (TC) stresses. Reference units  that were not suspected as having CUP cracking issue, didn’t  fail after LT and TC stresses. In contrast  to the reference


units, the failing units developed high resistance or/and shorts  at several pins.


A method was needed for fast and artifact-free observation of  sub-pad cracks for easy identification of assembly lots  affected by pad over-stress.


Three kinds of units were used for this investigation:


1. Reference units – units from a lot that hasn’t been affected  by pad over-stress during assembly, and thus aren’t suspected  as having CUP cracks.  The units haven’t been subjected to  any environmental or thermo-mechanical stress and can be  considered as “free of cracks”. These units were taken for  etching technique development.


2. Units from a lot that has supposedly suffered from pad  over-stress during assembly, however successfully passed a  functionality screening test. These units haven’t been  subjected to any environmental or thermo-mechanical stress. Although these units do pass the electrical test, they might  have pad cracks which do not propagate into the active layers  of the device. These units are considered as having high  reliability risk.


3. Units from a lot that has supposedly suffered from pad  over-stress during assembly and was subjected to 500 cycles  or 1000 cycles of TC stress. These units had a high fallout rate  after stress, and are considered as having CUP issue with high  certainty.


The flow includes unit decapsulation using fuming nitric acid  followed by wire bond etching/lifting and Al pad etching to  expose the underlying TiN barrier layer for inspection by  optical microscope or SEM. Fuming nitric acid doesn’t affect  Au balls and only passivates Al pads.


The purpose of the experiment was to determine the best Au  balls/Al pads etch method for fast, reliable, and artifact-free   sub-pad crack observation.


Four different chemistries for TiN barrier exposure were   investigated. Reference unstressed good units that supposedly  did not have under-pad cracks were taken for the experiment. After the etch process development was finished, and the best  method was chosen, the method was applied to both reference  units and units that were suspected for having under-pad  cracks and failed after TC stress. Then the method was  checked on units supposedly having CUP issue that were not  subjected to TC stress and didn’t show any electrical failure. The purpose of the last experiment was to determine whether  the method was capable of identifying lots affected by  assembly/sort related pad over-stress.


The investigated chemistries were:


1. Aqua regia: a mixture of concentrated nitric acid (HNO3)  and 30% hydrochloric acid (HCl) in proportion 1:3.


2.  Ferric cyanide: K3Fe(CN)6 aqueous solution (4 g of salt in  10 ml of DI water), or a mixture of ferric cyanide aqueous  solution and 30% hydrogen peroxide in proportion 1:1.


3. Hot phosphoric acid: 80% H3PO4 aqueous solution.


4. Tri-iodine: KI 0.5 g + I2 0.25 g dissolved in 10 ml of DI  water, and 10 ml of methanol added.


A  variation of etching conditions (etch time and tech  temperature) was tried for each of the chemistries.


Optical inspection of exposed TiN barrier layer was  performed to document the results of the experiments. Dual  Beam FIB cross-sectioning has been implemented on failing  and reference units to prove that the method provides artifactfree results.


Aqua regia is a well-known dissolver for Au and Aucontained compounds. However, it shouldn’t dissolve Ti. The  etchant was applied to exposed Au balls/Al pads at room  temperature and etch time varied from 30 seconds to 15  minutes. It was found that aqua regia etches both Au and Al  with very low Au/Al selectivity. It was found too aggressive,  creating cracks in TiN layer. Fig. 1 presents typical results  obtained on a fresh unstressed unit after 4 minutes of etching  in aqua regia. One can see that  TiN layer cracks and  delamination occurred. As we do not expect to observe cracks  on unstressed units, we conclude that the cracks are an etching  artifact.


Figure 1: a. An optical micrograph showing TiN barrier  cracks, supposedly etching artifacts, observed on a reference  unstressed unit  exposed using aqua regia


b. Higher magnification optical micrograph.


Cyanides are the known Au enchants. A ferric cyanide  aqueous solution that was applied on exposed post  decapsulation Au balls/Al pads at 50°C, had very low etch  rate. Fig. 2 shows a pad area after four hours of etching in  ferric cyanide. One can see that the etching didn’t occur at all. It’s known that oxygen easily oxidizes gold in the presence of  CN- ions due to a strong [Au(CN)2]- ion formation as a result  of this reaction. Adding of O2 (by mixing a cyanide aqueous  solution with hydrogen peroxide) considerably accelerated  etch of Au and Al. Fig.2 (c) shows the pad area after 4  minutes etching in cyanide/peroxide solution at 50°C.  One  can see that Au balls/Al pads are almost gone, but the etching  isn’t clean.


Figure 2: a. An optical micrograph showing the pad area of a  reference  unstressed unit after decapsulation.


b. Same area after four hours etch in ferric cyanide - no etch  occurred.


c. Same area after etch in a ferric cyanide/ hydrogen  peroxide solution


Hot phosphoric acid is well-known as a common Al etchant. It should etch Al pads fast, and lift Au wire bonds while  keeping the underlying TiN barrier intact. Two different  etching conditions were tried. The first unit was etched in  phosphoric acid at 85°C for 8 minutes. The second unit was  etched at 125°C for 8 minutes.  Fig.3 presents the etching  results. The second unit was considerably over-etched. Not  only Au balls and Al pads had been removed, but the TiN  barrier was gone as well. The first unit shows a clean Al pad  etch, however higher magnification inspection shows that  some pads have tiny cracks in the TiN and lifting of this  barrier layer. As we do not expect to observe cracks on  unstressed reference units, the cracks should be considered to  be the etching artifact. We do not conduct more experiments  with lower etch temperature and shorter etch time, however  one can conclude that the tolerance of the process is low. The  TiN layer can be easily over-etched, and strong keeping of  etching conditions (time/temperature) is recommended for this  method.


Figure 3: a. An optical micrograph showing the pad area of  an  unstressed reference unit after phosphoric acid etch at  T=85°C.


b. Higher magnification of one of the pads showing presence  of a tiny break in the TiN barrier.


c. An optical micrograph showing pad area of an  unstressed  unit after phosphoric acid etch at T=125°C.


Halogen-containing solutions are common gold and aluminum  enchants. Tri-iodine is recommended in Handbook of Metal  Enchants as an Au etchant providing high selectivity to Ti and  TiN. Adding methanol to a tri-iodine aqueous solution should  provide a cleaner etch, more selective to TiN. Table 1 presents  etch conditions and results obtained in the tri-iodine  experiment.


Table 1: Etch conditions and results for tri-iodine etch  experiment


Unit


number


Etch


temperature, °C


Etch  time


Notes


20 5 min Au, Al etched, no TiN  cracks


20 8 min Au, Al etched, no TiN  cracks


20 20 min Au, Al etched, no TiN  cracks


55 40 sec Some Al pads remain  under-etched


60 25 sec Some Al pads remain  under-etched


From the data in  Table1 one can conclude that tri-iodine


provides clean Au ball/Al pad etch with low/medium Au to Al  selectivity and high selectivity to TiN. The process tolerance  is high: extending the etch time from 5 minutes to 20 minutes  doesn’t cause TiN barrier cracking or lifting. No etching


artifacts was seen on unstressed reference units. Fig.4 presents


the results obtained on the unstressed reference unit after triiodine application at room temperature during 5 minutes. The  TiN barrier layer is unaffected. These etching conditions are  considered to be the best tested herein and have been used on


units failed after 1000 cycles TC stress.  Fig.5 shows TiN


barrier crack found on a unit that was suspected as having a


CUP crack issue. The failing pad location matches the afterstress test electrical data.


Figure 4: a. An optical micrograph showing TiN barrier  layer, exposed using tri-iodine (reference unit).


c  a


Figure 5: An 0ptical micrograph showing sub-pad crack  identified by etching in Tri-iodine at the unit suspected having  CUP issue and electrically failed after 1000 cycles TC stress


Thus, the tri-iodine technique provides clean bond pad etching  for determination of probe/bonding related damage in the TiN  barrier. However, the question arises whether this technique is  artifact-free and doesn’t introduce the damage by itself. FIB  characterization has been used to cross-section the identified  problematic bond pads to address the question of potential wet  chemical etch enhanced damage. The unit suspected as having  a CUP issue from the assembly process, that failed after 1000  cycles of TC stress, was taken for analysis. The unit was  mechanically polished down to wire balls, and Dual Beam  FIB cross-section through the suspected (i.e., electrically  failed) bond pad was applied then. Fig. 6 presents the SEM  micrograph of FIB cross-section of the failing bond-pad. The  cross-section showed a crack related to Al-Au IMC, accompanied by IMC-pad delamination, and  a crack in the  TiN barrier layer of the pad propagating further into the IMD  layer.


Figure 6: SEM micrograph of the FIB cross-section done  through the failing pad showing a TiN barrier layer crack  propagating into the IMD layer.


The same FIB cross-sectioning technique was applied to  a  randomly chosen bond-pad of the reference unstressed unit. No sub-pad cracks were found in this case.


One can conclude that tri-iodine provides clean, fast, and  artifact-free exposure of the sub-pad area. Tri-iodine (KI 0.5 g +I2 0.25 g dissolved in 10 ml of DI water , and 10 ml of   methanol added) is chosen as the best method (from the four  tried). The recommended etching conditions are: room  temperature, etch time 5 minutes.


The chosen method was implemented on units from the lot #2  that has supposedly suffered from pad over-stress during  assembly,    however    successfully    passed the    functionality


screening test. The units have been unstressed and do not fail  electrically. However, they might have pad cracks which do  not propagate into the active layers of the device and   considered have a high reliability risk. Fig.7 shows the  exposed TiN barrier layer of the pads for one of these units. The cracks are clearly seen. This means that the units form the  affected lot have a high reliability risk


Figure 7: An optical micrograph showing TiN barrier cracks  exposed using tri-iodine etch. This unit was suspected as  suffering from a CUP cracking issue as a result of the wire  bonding process, but, it didn’t fail electrically.


This paper provides a comparative analysis of several bond  pad etching methods and gives detailed information of etch  chemistries and conditions (as temperature, time) used for   TiN barrier layer crack exposure. The investigation results  showed that tri-iodine etchant provides clean and artifact-free  exposure of the TiN barrier layer of the pad. The method  shows high tolerance to etching conditions (temperature/time). It  is considered the best (from the four methods tried) for pad  crack observation. The method can be used for bond-pad  related failure analysis and for fast determination of assembly  lots affected by pad over-stress and considered as having a  high reliability risk.


The author acknowledges her Intel coworkers: Ida Posimeinik, Leonid Alperin, Boris Maryanovsky , Alon Goldenberg, and  Yuval Greenzweig for help in FA work and fruitful  discussions.


[1] Chang C. and Sze S., ULSI Technology, McGraw-Hill  Companies, Inc., (New York, 1996), p.547-549


[2] Z.G.Song, T.Tun, C.K.Oh, S.Redkar and others: “Investigation of Bond-pad Related Inter-metal Dielectric  Crack”, ISTFA 2003 Proceedings, p.82-85


[3] Jacob P., Nicoletti G.: “New FIB-Supported Approach for  Wirebond Characterization”, ISTFA 2000 Proceedings, p.35- 40


[4] Lee T. and Pabbisetty S., Microelectronic Failure  Analysis, Desk Reference, 3rd edition, ASM International, 1997, p.111-113


[5] Walker P. and Tarn W., Handbook of Metal Enchants, CRS Press (Boston, 1991)


Au ball


TiN barrier


Upper metal


IMC


W plug


Investigation on the Influence of Focused Electron Beam on Electrical Characteristics of Integrated Devices


S. Doering, R. Harzer, W. Werner


Qimonda Dresden GmbH & Co. OHG, Dresden, Germany Stefan.doering.drs@qimonda.com


In recent years the application of nano probing systems has become widespread in semiconductor failure analysis. This is primarily due to the difficulties encountered in performing electrical characterization on latest technology nodes’integrated devices using standard probe stations (e.g. an optical microscope in combination with micrometer screw driven manipulators). Other reasons include the new capabilities offered by probing systems like current imaging  and the growing rate of non visible or parametric fails.


There are two different types of systems  available to electrically characterize devices at the contact level; one is  based on the Atomic Force Microscope (AFM) platform and  the other is a Scanning Electron Microscope (SEM) based  system. The AFM based systems utilize several AFM heads (e.g. four heads to characterize one bulk transistor consisting  of a gate, source, drain and corresponding well) equipped with  conductive probe tips to map the sample surface in contact or  non-contact mode. After scanning the area of interest, the  probe tips are placed on top of the desired structure and a  parametric analyzer extracts the data.


The SEM based systems are located in a high vacuum chamber  and the sample surface is monitored along with the probe tip  position by the SEM. These systems are also capable of  positioning the probe tips on top of contacts or metal lines and  it is possible to establish an ohmic contact to the device of  interest.


For the SEM based systems it is known that there is an impact on certain device parameters like transistor ION and IOFF which correlates  to the primary electron beam acceleration voltage [1]. Nevertheless both types of systems are used in the semiconductor failure analysis community obtaining significant results [2, 3, 4].


Scope of this work


In the forefront of this work two questions arose:


1. Is it possible to use our SEM/FIB based probing  system to do electrical characterization at device level


despite the fact that there is beam induced device  degradation?


2. What are the effects to consider if a beam exposed  sample has to be characterized by a nano probing  technique during the failure analysis flow?


This leads to the concern for the optimum SEM conditions to  avoid beam induced device degradation and the device parameters itself that are affected by beam radiation together  with their dependency on SEM parameters.


To answer these questions the following experimental setup  was employed.


Experimental Setup


As a representative device, a drive transistor (nFET) of a  Single Port SRAM manufactured in a 90nm CMOS process was  selected. The device parameters that were compared before  and after the beam exposure were saturation current (ION),transistor leakage current (IL), the subthreshold voltage (VTH)and the slope (S). ION current is IDS a t  VG=VDS=1.2V. The transistor leakage current IL is defined as ISD at VG=-0.3V. VTH values are obtained at IDS=8.25·10-7A.


Before the experiments started, potential parameters having an  effect on device characteristics such as  beam acceleration  voltage (VACC), beam dose (D); target device properties like  height of the inter layer dielectric (hILD), gate oxide thickness (dGOX), width (W) and length (L) of the transistor channel, and  the materials used were identified. As an additional parameter,the time between the beam exposure and the re-characterization was taken into account.


Since the implantation of the P-Well was performed on other  devices at the same time during the manufacturing process, it  might also cause the failure of those particular devices. This  physical result gives a clue to check the regions of the output  driver transistor circuits that adopt the P-Well implantation. Thus, one of the DQ pads that failed due to a high output  leakage current, ILOH, during the DC test was selected for  further analysis.  Figure 4 confirms the DQ pad failed in our  FIB nanoprobing tests when applying voltages to the VDD, VSS, and DQ pads, respectively. The failed DQ pad indicates a  very high output leakage current that is outside the production  specification.


This DQ pad was then de-processed to the layer of M0 BL (bit  line). A schematic layout of this pad and its adjacent circuitry  is shown in Fig. 5.  The power from VDD will go to the PMOS  transistor and the N-Well, and the power from Vss will go to  the NMOS transistor and the P-Well.  The DQ voltage will go  to the PMOS and NMOS transistors. The white dots  surrounding the PMOS indicate the contacts to the N-Well, and those surrounding the NMOS indicate the contacts to the  P-Well.


-1.0E-02


1.0E-02


2.0E-02


3.0E-02


4.0E-02


5.0E-02


20.0


40.0


60.0


t (sec)Normal DQ


Failed DQ


Figure 4: Output leakage currents of the normal and failed  DQ pads.


Figure 5: A schematic layout showing the areas of the DQ  pad and its adjacent circuitry.


-1.2E-08


-1.0E-08


-8.0E-09


-6.0E-09


-4.0E-09


-2.0E-09


2.0E-09


4.0E-09


V (V)


Normal pad


Failed pad


Figure 6: Current-Voltage characteristics of a P-N junction  diode in the normal and failed DQ pads.


P-Well


Contact


P-Well STI


Figure 7: SCM dC/dV phase images showing the profiles of  the P-Well and N-Well in (a) the normal and (b) the failed  devices.


Figure 8: A section analysis of SCM signals along the dashed  green line of Fig. 7b.


Since the ILOH failed in the DC test, the NMOS circuit was  therefore investigated. In addition, a P-Well shift was  observed earlier in the failed low Vt PMOS of the SA circuit, so we simply probed two Well contacts (one P-Well and one  N-Well) as indicated by arrows 1and 2 in Fig. 5 at the NMOS  to examine the I-V characteristics. Figure 6 shows the I-V  curves in the normal and failed DQ pads. Both curves behave  as a P-N junction diode. Nevertheless, the current in the failed  pad is higher than in the normal pad at the same forward221


biased condition.


From the cross-sectional SCM phase images along the two  Well contacts, it can be seen that the P-Well has shifted to the  left side of the normal position that separates the original NWell into two regions (Fig. 7a and 7b). In addition, a sectional  analysis of SCM data (Fig. 8) along the dashed green line in  Fig. 7b confirms the N-Well has been separated into two  regions by the shift of the P-Well even in the area between  STI and the P-Well.  Therefore, as indicated by arrow 1 (Fig. 7b), the areas of the P-N junction and the N-Well in the failed  pad are smaller than those of the normal pad. This probably  causes a higher current at the same forward-biased condition  because the area of the depletion region of the P-N junction is  reduced compared to that of the normal pad.


From the results mentioned above, we conclude that the shift  of the P-Well during the manufacturing process causes the  failure of a high output leakage current in the DC test for this  specific case.


In this paper, the failure analysis process for a specific case  that is failed due to a high output leakage current in the DC  test is demonstrated. Nanoprobing is a useful tool for the  confirmation of electrical characterization and localization of  device failures. Moreover, SCM provides helpful 2-D  implantation doping profiles for the verification of physical  causes of the failure devices. In this specific case, the shift of  the P-Well during the manufacturing process is identified as  the cause of DC failure.


The authors would like to present our thanks to our colleagues  at the Department of Electrical Failure Analysis and Product  Engineering in ProMOS for their insightful discussions of  circuit layouts.


[1] Liu, L., Wang, Y., Edwards, H., Sekel, D., and Corum, D., “Combination of SCM/SSRM analysis and  Nanoprobing techniques for Soft Single Bit Failure  Analysis,” Proc. 30th International Symposium for  Testing and Failure Analysis, Worcester, MA, Nov. 2004, pp. 38-41.


[2] Kleiman, R. N., O’Malley, M. L., Baumann, F. H., Gamo, J. P., and Tipm, G. L., J. Vac. Sci. Technol. B, 18 (4), (2000), pp. 2034-2038.


[3] Edwards, H., Ukrainstev, V. A., Martin, R. S., Johnson, F. S., Menz, P., Walsh, S., Ashburn, S., Wills, K. S., Harvey, K., and Chang, M. C., Journal of Applied  Physics, Vol. 87, (2000), pp. 1485-1495.


Measuring Static Noise Margin of 65nm Node SRAMs Using a 7-point SEM  Nanoprobing Technique


Richard E. Stallcup II, Ph.D., and Zachary Cross


Zyvex Instruments L.L.C., 1321 North Plano Road, Richardson, Texas, 75081, USA


William James, and Phuc Ngo


Microtech Analytical Labs LP, 538 Haggard Street, Suite 402, Plano, Texas, 75074, USA


Keywords: nano probing, SRAM, bit cell, butterfly curves, voltage transfer curves, VTC, static noise margin, SNM, 65nm technology  Abstract


Non-visual fails have become an ever present complication in


the IC industry. Nano probing SRAM bit cells at the inverter


level allows the cell to be tested and static noise margin


(SNM) to be measured. This paper explains how nano probing


of a 65nm technology 6 transistor bit cell was performed and


SNM dependence on supply voltage was measured for both


hold and read modes. Connection to the bit cell was made at


the Metal 1 layer with 7 nano probes to collect the voltage


transfer curves (VTCs) of the two inverters of the cell. In this


experiment, each inverter was tested by varying Vdd voltage


from 1.5, 1.2, 1.0, 0.8, 0.6, 0.4 and 0.2V while collecting the


VTC. The two VTCs of the cell are plotted to produce the


cell’s butterfly curve from which the SNM is found


graphically for each setting of Vdd.


In this paper we report, for the first time, a technique for


measuring the static noise margin (SNM) of in die 6T SRAM


bit cells using an SEM based nanoprobing system. The SNM


of a bit cell quantifies the amount of electrical noise that is


required, at the cell’s internal nodes, to flip the cell’s contents


[1,2]. This information is vital to the engineering cycle to


produce faster and more efficient SRAM designs. With the aid


of SEM based nanoprobing systems that are equipped with 8


or more probes, measurements such as SNM and bit cell


stability are now possible on in-die SRAM transistors.


The SRAMs measured for this paper were based on the 65nm


IC process and were obtained by purchasing an off-the-shelf


microprocessor. An Intel™ E6600 Dual Core Processor was


purchased from a mass market retail electronics supply store.


The depackaging and deprocessing of the chip was done at


MAL [3]. After careful depackaging, the chip was


mechanically polished with diamond grit down to the metal 2


layer. After thoroughly cleaning off the diamond mechanical


polish media, the deprocessing resumed with a colloidal silica


chemical mechanical polish (CMP) media until the copper


metal 1 layer was reached. At this level, interconnectivity of


the SRAM transistors was sufficient to allow SNM


measurements of an isolated SRAM bit cell. The chip was  then cleaned of the polish media and mounted on an aluminum  SEM specimen holder with vacuum compatible, single sided, adhesive, copper tape.


A Zyvex nProber™ System was used for all imaging and data  collection for this paper. It is a fully integrated system  consisting of a field emission gun (FEG) SEM, eight probe  and sample nano positioning system, computer aided design (CAD) navigation system, Keithley 4200-SCS parametric  analysis system with 8 SMU/preamp, a sample exchange  system and an in-situ sample and probe cleaning system. The  prober uses tri-axial cables to connect the analyzer through a  vacuum interface to each probe. This feature allows the  system to have low electrical leakage and noise (below 200fA) so that low level Ioff and critical leakage measurements on  SRAM transistors can be achieved. The prober was loaded  with eight Zyvex probes prepared using a proprietary Zyvex  process and bent to a 45 degree angle.


To avoid buildup of hydrocarbon contamination on the chip  during SEM imaging, the chip was decontaminated with a  down stream asher that is integrated into the nano prober’s  sample exchange system. This process is a well known  solution [4] to the “black box” problem that forms on samples  during SEM imaging. Once the chip was decontaminated of  hydrocarbons and transferred from the sample exchange  system onto the nano probing stage located in the SEM sample  vacuum chamber, the chip was ion sputter cleaned with an  integrated 5 keV argon ion source. This system removed  copper oxide from the metal 1 copper traces by using a 2mm  diameter argon ion beam with a beam energy of 5 keV. These  two steps, hydrocarbon decontamination and argon ion sputter  cleaning, are important tasks that greatly reduce the probe tip  to sample electrical contact resistance. These preparation steps  were carried out in-situ and, as a result, the chip stayed  contamination and oxide free for many hours of nano probing.


Figure 1(a) shows the schematic of the bit cell at metal 1 and  the large black dots indicate the nano probe tip/sample contact  locations for the two inverters of the bit cell. The SEM photo  in Fig. 1(b) shows 6 nano probes used to supply and measure


Figure 1: Schematic for the 6T bitcell at metal 1 showing the probe contact locations (a). SEM image taken at 1 keV of the nano  probes in contact with inverter 1 at the copper metal 1 layer (b).


voltage on one of the two inverters of a bit cell. Not shown is a  seventh nano probe placed on the well connection that is out  of the view of Fig. 1(b). Had this bit cell been based on silicon  on insulator technology, the seventh probe would not have  been necessary.


The voltage transfer curves (VTCs) of inverter 1 were  collected by supplying the needed fixed voltage to the Vdd, Vss, Wordline, and Bitline and sweeping voltage on the CL  connection while measuring voltage on the CH connection. The VTCs of inverter 2 were collected in the same manner  with the exception that the bias of the CH connection was  swept and voltage was measured at the CL connection. Data  was collected for both Read and Hold conditions whereas the  WL connection was held at Vdd for Read and 0.0 volts for  Hold.


The butterfly curves of Fig. 2 were created by taking the  VTCs of inverter 1 and inverting the curves and plotting them  with the VTCs of inverter 2. Figure 2 shows the butterfly  curves along with the graphically determined SNM for Read  and Hold with the Vdd held at 1.0 volts. The square having the  longest diagonal between the VTCs of the two inverters gives  the SNM by the length of the side of the square. If the  butterfly curve is asymmetric, as illustrated in Fig 2(a), by  having a small and a large square in the two openings of the  curve, then the smaller of the two squares is used for  determining the SNM [1]. Figure 2(a) shows that the SNM is  lower during the Read function and this is because the VTC is  degraded by the voltage divider across the pass gate transistor  and the drive transistor.


By collecting the SNM values for the bit under test and  varying the Vdd from 1.5V to 0.2V we can determine the bit’s  dependence on supply voltage and its ability to retain data. If  the supply voltage is lowered so that the SNM is just greater  than 0.0 then that point is the data retention voltage (DRV). Other factors can affect the SNM such as temperature and  process variation [2].


0.8 1


CH (V)


Read Vdd=1.0


SNM = 0.16 V VTC-1 Inv1


VTC  Inv2


Hold Vdd=1.0


SNM = 0.28 V


Figure 2: Butterfly plots of a 65nm node SRAM bit cell in read


(a) and hold conditions (b).


Individual transistors in SRAM, DRAM, flash RAM and logic  devices are now routinely nano probed at the tungsten contact  level with SEM based nano prober systems. With a nano  prober system fitted with 7 probes or more, the next level of  testing can now be conducted. SNM is an important metric in  determining the stability of 6T SRAM designs and their  dependency on supply voltage and other factors. With SEM  based nanoprobing, SNM can be measured on in-die bit cells.


Vdd


Vss


Inv1


Inv2


CH


Word


Bit


The authors would like to thank the PFA engineers of AMD  Austin, Texas for their valuable guidance in developing  butterfly probing as a new application for nanoprobing and  integration of this test into the nProber system.


[1] E. Seevinck, F. List, and J. Lohstroh, "Static-Noise Margin  Analysis of MOS SRAM Cells," JSSC, Vol. SC-22, No. 5, pps  748-754, Oct. 1987.


[2] B. Calhoun and A. Chandrakasan “Analyzing Static Noise  Margin for Sub-threshold SRAM in 65nm CMOS,” ESSCIRC, pp. 363-366, Sept. 2005.


[3] Microtech Analytical Labs, LP, 538 Haggard Street, Suite  402, Plano, Texas, 75074.


[4] R. Vane and R. E. Stallcup II, “Extending transistor  probing time in scanning electron microscopes and focused  ion beams with Evactron cleaning” in SCANNING 2005, edited by R. P. Becher, Proceedings of SCANNING 2005, Monterey, Calif., USA, Vol. 27 Num. 2, pp. 106-107.


LOCALIZED DIE METALLIZATION DAMAGE INDUCED DURING   LASER-MARKING OF A SEMICONDUCTOR PACKAGE


Paul Eric B. Parañal


Intel Technology Philippines, Inc., Gen. Trias, Cavite, Philippines  paul.b.paranal@intel.com


This paper presents a new fail mechanism for laser-marking  induced die damage. Discovered during package qualification, silica spheres – commonly used as fillers in the molding  material, was shown to act as a propagation medium that  promote the direct interaction of the scribing laser beam and  the die surface. Critical to the understanding of the fail  mechanism is the deprocessing technique devised to allow  layer by layer examination of the metallization and passivation  layers in an encapsulated silicon die. The technique also made  possible the inspection of the molding compound profile  directly on top of the affected die area.


Laser marking or scribing is but one of the ways by which the  package of a semiconductor device is marked or labeled. The  principle [1, 2] is quite simple: the package, which is made of  optically absorbing material, is exposed to a high energy  radiation source such as a laser beam. As energy is absorbed, a  rapid but localized heating in the material takes place until the  irradiated portion of the material melts or evaporates, leaving  behind an engraved area.


Over the years this method has gained popularity due to its  ability to produce indelible marks, rapidly, and with greater  flexibility. It is also environmentally clean and involves less  supply inventory and by-products – attractive reasons why it is  preferred more than ink-based marking technologies.


There are however, some instances where the laser marking  process for semiconductor packages become responsible for  device failures. As the semiconductor industry trends toward  developing smaller and thinner packages, the laser marking  process can produce deep marks that can actually burn its way  down to the die surface metallization. Issues in the mold  transfer process can also lead to package voids such that a  laser beam cutting through a large cavity (as shown in Figure  1) can also find its way to the die surface. In both cases, device  failures are due to the direct interaction of the scribing beam  with the encapsulated silicon which results to the melting of  the die metallization.


Figure 1: Top view (left) and cross-section (right) of a  package void in a laser marked area.


During qualification of a Flash package, a new fail mechanism  for laser marking-induced die damage was discovered. Apparently, melting of die metallization can also occur even at  normal laser marking parameters, at normal mark depths, and  without the known molding compound issues.


The succeeding sections of this paper will be devoted to the  discussion on the breakthrough fail mechanism. The failure  analysis approach used to uncover the new fail mechanism as  well as the root cause will also be covered.


The Fail Signature


It was first detected during device testing performed after the  laser marking process. The defect manifested in several units  as functional failures which, upon succeeding electrical  validation and fault isolation, were confirmed as a die level  defect.


Figure 2: Optical image of the die surface showing melted  metallization.


Die level inspection of a decapsulated unit found evidence of  localized melting of the die metallization (shown in Figure 2). This signature is similar to the die damage that occurs when a  scribing laser beam directly hits a die surface [3].


When the melted areas on the die is mapped and projected up  against the package, it is observed that the affected areas are  directly underneath the laser-marked characters on the package  surface.


In Figure 3 below, is a cross sectional diagram of a ball grid  array (BGA) package showing a die in “live bug” position and  the location of the die damage relative to the laser marked  area.


Figure 3: BGA package schematic cross-section showing the  laser mark and die damage locations.


Prior to decapsulation, an inspection of the package did not  reveal any irregularities. Although the damage on the die is  most likely induced during laser marking, there are no deep  laser marks or mold voids found in the package.


The Failure Analysis Flow


Shown in Figure 4 is the outline of the failure analysis flow  used for this issue.


Figure 4: The Failure Analysis Flow.


The left hand path represents the conventional FA flow that  gave us the image shown in Figure 2. This procedure, although


successful in locating and exposing the damaged area on the  die, destroys all evidence related to the interaction between the  laser beam and the encapsulating material that results into die  damage.


In order to preserve these data, a backside analysis approach  was devised. This is illustrated by the right-hand path in the  analysis flow.


After electrical validation of the functional failures, the  package material is removed by grinding off the unit from the  bottom and up to the silicon backside of the failing die. Reactive Ion Etch (RIE) in sulfur hexafluoride (SF6) environment is used to remove the silicon substrate until only  the metallization layers of the failing die and an intact mold  cap remains. A Focused Ion Beam (FIB) is used to crosssection the backside of the die metallization layers to expose  the defect and the immediate die passivation layers. A  mechanical cross-section of the package is performed to reveal  the full mold cap profile directly above the die defect. An  optical microscope and a Scanning Electron Microscope (SEM) is used to inspect the result of each step and to take the  pictures used for analysis.


Backside Deprocessing Approach


Figure 5 is an optical image of the die metallization backside  taken after removal of the package backside and the silicon  substrate. The image clearly shows the spot where the melting  of the die metallization occurred. Localized polishing using a  dimpler was employed to obtain this high contrast optical  image.


Figure 5: Backside image of melted metallization taken after  removal of the silicon substrate.


Metal Layer Shorts


A localized cross-section at the center of the melted area is  done using the FIB tool. Cross-section was performed from the  backside of the metallization layers. As shown in Figure 6, the  device failure is found to be primarily due to the melting of the  die metallization which resulted to shorted rows within the  metal layers. Cracks in the inter-layer dielectric (ILD) that  envelopes the metal rows served as channels for the melted  metallization to connect the adjacent metal rows.


Figure 6: SEM image showing a cross section of shorted  metal rows.


Mold Cap Profile


To allow the inspection of the different package layers directly  above the shorts location, a deeper FIB cut was performed.


The SEM image in Figure 7 shows that no irregularities can be  seen in the passivation layers of the die. There is also no laser  burn path in the molding compound that leads to the melted  metal layer. Instead of voids in the mold cap, large silica fillers  are found situated directly on top of the damaged area. Absence of indentations in the polyimide layer implies that the  silica filler is not exerting any unusual pressure on the die.


Figure 7: Die backside FIB cross-section of the region with  melted metallization.


In Figure 8 is the result of the mechanical cross-section  showing the mold cap profile of the failing unit. Directly on  top of the damaged area on the die are two large silica fillers, each about 50 microns in diameter, stacked one on top of the  other leading up to the laser marked area on the package  surface.


Figure 8: Mold cap cross-section showing a column formation  of large silica fillers between the damaged die area and the  laser marked region.


This image is proof that the melted metallization is directly  under a laser marked area. However, there is no laser burn  path that can be seen in the mold profile. Both the mark depth  and the mold cap clearance are also within the tolerance  values.


Clearly, the mechanism for metallization melting in this issue  is one where the laser beam is able to heat up the die surface  without creating damage in its path


Laser-Material Interaction


When a laser beam strikes a target material, the radiant energy  it carries is partly absorbed, reflected, and transmitted. This  distribution of energy is defined by the Beer-Lambert law [4] which relates the absorption of radiation with the optical  properties of the material and the wavelength characteristics of  the incident light.


It is during energy absorption that material heating occurs due  to the increase of the vibrational amplitudes of the atoms at the  lattice points. Consequently, a rise of temperature in the  material takes place. According to the laws of  thermodynamics, the rise in temperature will continue to  critical levels as long as the absorbed power density exceeds  the capacity of the material to conduct heat away from the  impact site. Exceeding the critical vibrational amplitudes, the  long range order of the crystal lattice is destroyed and the  material melts [1, 2].


Heating through laser energy absorption can be described by  the Fourier’s equation [5, 6]. The general form of which can be  stated as


Q


c 2p +∇κ=∂∂ρ    [1] where ρ is the material density, CP is the specific heat of the  material,  and κ is the thermal conductivity. This equation  gives us an expression on how temperature T changes as a  function of time t during laser irradiation.


The heat source Q represents the absorption of laser energy  derived from Beer-Lambert’s law and is further expressed as


z


0 e


where R is the reflectivity coefficient of the material, I0 is the  incident laser intensity, α is the wavelength-dependent  material absorption coefficient, and z is depth into the  material.


As described by the equations, material properties that can  promote laser heating are higher absorbance, higher thermal  conductivity, and lower specific heat capacity. Laser-system  dependent parameters, on the other hand, are the laser intensity  or power density and the duration of irradiation.


In order to explain how the laser beam can induce melting in  the die metallizations without evidence of damage in the beam  path, we further compare the properties of two key materials – the mold fillers which is made of silica (SiO2), and copper  which composes the die metallization.


Laser Heating in Copper and Silica


Table 1 lists a comparison of the relevant material properties  of copper and silica [7].


Table 1: Copper and Silica Material Data


By comparing the thermal conductivities and heat capacities of  copper and silica, it can be seen that the latter offers more  resistance to thermal effects due to laser heating.


Silica, which is used as fillers in molding materials, are  transparent beads of glass. Under 1064-nm wavelength  illumination (for an Nd:YAG laser), it has an index of  refraction approximately equal to 1.46 and a reflectivity of  about 2%. [7]


Using the laser scribing parameters (laser intensity and scan  rate) used at the time the failures occurred, it can be  approximated that the same conditions that can bring copper to  its melting temperature of 800°C will only produce a  temperature change of about 1°C  to silica.


These data signify that silica is indeed capable of transmitting  the wavelength of the scribing laser with minimal energy loss  brought by reflection, absorption and heat generation.


Laser Beam Transmission in Silica Spheres


The transmission of infrared rays in a silica sphere, approximated using the Snell’s Law, is shown using a ray  diagram in Figure 9. Similar to a lens, a ray passing through its  center will go undeflected while incident parallel rays can


come out focused on the other end resulting to an  amplification of the laser power density.


Figure 9: Ray diagram showing how parallel rays are  transmitted through a sphere.


Within the mold cap, a stack of silica spheres in contact even  at just a point, can act as a waveguide that will enable a laser  beam striking the topmost filler to be transmitted down to the  die surface.


Figure 10: Diagram showing laser beam transmission  through stacked silica spheres.


Figure 10 is a ray diagram showing the approximate beam  transmission path inside two stacked silica fillers. A ray  passing through the geometric centers of the spheres will  experience no deflection. The ray will be transmitted through  the transparent passivation layers of the die and ultimately  deliver the energy to the die metallization. Thus, melting of the  die metallization can occur even without evidence of damage  to the beam path. Damage occurs not because of heat transfer  but because of the unattenuated transmission of the laser beam, via the silica waveguide, down to the die surface during the  laser scribing process


Silica Filler Stacking: A Random Phenomenon


The possibility of laser induced failure due to the fail  mechanism discussed above relies on the probability of  satisfying two conditions: the columnar stacking of silica  fillers and the mark depth reaching the apex of the stacked  silica fillers. Both are random conditions that cannot be fully  understood until a study is done to see how silica fillers  reorder during mold transfer flow. However, we can already  identify the possible factors that can aggravate/enhance these


conditions. A higher density of large silica fillers increases the  probability of filler stacking while a lower mold cap clearance  and deeper laser marks increase the chance of the laser beam  reaching a column of silica fillers.


With the current trend of continuously decreasing package  dimensions, silica filler size is fast becoming a factor that can  seriously affect assembly yield. The right balance between  filler size and overall package performance should be studied  during package development.


[5]  Ganasan, Jaya,  “Soldering on Gold Plated Substrates – Solder Joint Reliability and Integrity of Surface  Components”.  IEEE, 1995, pp. 372-376


Failure Analysis Methodology for Li-ion Incidents


John Loud, MSEE, PE, Principal Engineer


Xiaoyun Hu, MSEE, Senior Engineer


Exponent Inc., United States of America (Exponent.com) jloud@exponent.com, xhu@exponent.com


The purpose of this paper is to lay out a scientific  methodology for investigating lithium ion (Li-ion) product  failures. The consumer product market continues to show  more and more demand for portable electronic devices that  require stored electrical energy. Li-ion technology has become  the most popular choice because of its high energy density, high cell voltage, low self-discharge rate, lack of “memory  effect” on its capacity, and because it is environmentally  preferred. However, the use of flammable solvents as the  electrolyte and the susceptibility for the cathode materials to  thermally decompose and generate oxygen leads to potentially  unsafe failures in Li-ion cells. Failure can occur due to  problems within a cell, or because of external factors that  affect a cell. The Li-ion cell(s) are typically located inside  portable products. Li-ion cells can be packaged in either a  plastic laminate covered foil pouch, or in a metal (aluminum  or steel) housing. Metal housed cells are typically contained in  cylindrical (such as “18650” - 18mm diameter and 65mm  long), or in prismatic (rectangular solid) housings. Cells  contained in metal housings can, under certain undesired  circumstances, build up internal heat and pressure that can  vent. Pouch-style cells cannot build up any appreciable  pressure, though they can become swollen and in some cases  overheat.


Undesired failures range from minor overheating of the cell  that causes minor melt or char damage to surrounding  materials, to energetic venting that may in rare cases include  flames and even ejected cell materials. Depending on their  severity, some incidents pose a credible ignition source for  surrounding combustible materials. Thermal dermal injury is  also possible due to expelled hot gasses and hot surfaces. While these types of failures have been known and explored  for many years in the engineering community, it is only with  the proliferation of these devices in society that these  undesirable, low probability events are gradually becoming  public knowledge. Extensive efforts have been devoted to  reduce the probability that such events will occur, including  external circuit protection to prevent electrically-induced  events, and novel cell designs and manufacturing methods  intended to prevent cell-initiated failures.


The need is great, however, to establish the root cause of each  undesired event so that steps can be taken to prevent future  events and also to determine whether an existing field  population has an unacceptably high risk of failure and should  therefore be removed from service.


A typical cylindrical cell structure is shown in Figure 1. The  cathode (positive) electrode employs LiCoO2 coating on an  aluminum current collector. The anode (negative) electrode  employs graphite coating on a copper current collector. A  porous polymeric membrane physically and electrically  isolates the two electrodes while allowing ion transfer.


Figure 1. Typical Li-ion cylindrical cell construction.


Fault Tree


Understanding of Li-ion cell failure mechanisms enables the  definition of an effective and useful fault tree. Possible causes  for an overheating Li-ion cell failure include:


1. An internal cell short circuit (manufacturing-related). Possible causes of an internal short circuit include:


a. A burr or other metal processing anomaly that  stresses the separator and eventually results in an  electrode-to-electrode short circuit.


b. Contamination in the electrode winding that  eventually penetrates the separator, resulting in an  electrode-to-electrode short circuit.


c. Contamination in the electrode winding that  dissolves into the electrolyte, then re-plates out on  the separator and dendritically grows through the  separator, resulting in an electrode-to-electrode short  circuit.


d. A lead anomaly that stresses the separator and  eventually results in an electrode-to-electrode short  circuit.


e. A lead to case or lead to electrode short circuit.


f. Misalignment of the electrodes such that contact  between the electrodes (including active materials) occurs.


g. Misalignment of the electrodes leading to plating of  metallic lithium around the edges of the separator.


h. Separator defects such as holes or tears.


i. Electrolyte contamination including moisture.


j. Electrode degradation. A local anode-to-cathode  imbalance where the cathode has insufficient lithium  can cause localized degradation (oxidation) of the  cathode. Similarly, if the anode has insufficient  capacity to absorb the lithium, plating will occur. Both of these processes may result in cell  overheating and venting.


k. Excessive mechanical forces on the electrode  winding resulting from swelling during charging if it  is wound too tightly or if it is too tightly constrained.


2. An internal cell short circuit (externally caused). Possible  causes for such an event include:


a. External mechanical crush of the cell housing or  pouch.


b. A pinpoint dent in the cell housing or pouch.


c. Excessive mechanical impact.


3. An external non-current-limited cell short circuit.


4. Overcharge of the cell, which may result in internal  heating and precipitate a cell internal short circuit. Such  internal short circuit events may be quite energetic since  the amount of energy stored at the time of the incident is  higher than that of a fully charged cell.


5. Overdischarge of the cell, which can result in dissolution  of the copper current collector, subsequent plating of the  dissolved copper onto the separator and dendrite growth  to form an electrode-to-electrode short circuit.


6. External heat. Externally heating a cell will cause it to fail  such that it may vent to dissipate its energy in an  undesirable manner. The cell housing may in some cases  also rupture and eject the cell contents.


7. High/low temperature charging. Charging a cell at too  high or too low a temperature can cause it to fail in an  undesirable manner.


Preventing Incidents


Once a battery pack manufacturer has taken steps to ensure  that its product can withstand a reasonable level of mechanical  abuse, and that its charge/discharge and protection circuitry  eliminates the potential for overcharge and overdischarge, there is nothing more that can be done to address the  possibility that some purchased cells have latent defects that  will some day result in an overheating event. There is no  incoming cell inspection or test that will identify all potential  latent cell defects. Nor do common cell protection features  such as positive temperature coefficient (PTC) devices, charge  interruption devices (CIDs) and separator thermal shutdown  provide any protection against such latent cell defects.


The only line of defense against latent cell defects is for a  battery pack manufacturer to reduce the probability of  purchasing such problem cells in the first place. There is no  practical number of cells that would have to be purchased and  then life tested to ascertain whether a specific supplier’s cells  have a probability of failure of, for example, 1 in 10 million. It  is no trivial matter to produce 10 million of anything with only  1 that has the potential to fail in an unsafe manner. While  history has shown that many cell manufacturers have at  different times produced cells that failed to meet their


expected failure rate, some use state-of-the-art manufacturing  equipment, rigorous maintenance methods and stringent  quality control procedures to effectively reduce the number of  defects in cells. Good monitoring and inspection programs  also increase the likelihood of detecting and eliminating any  defects that do occur.


Given the severity of a cell response to overcharge, most  manufacturers have standardized a design that requires a  minimum of two independent circuits to prevent overcharge. The concept is that no single-point component failure should  result in overcharge of the Li-ion cell(s). Most systems  employ a distributed protection system with the following four  main parts.


The charge regulator will not charge the cells beyond  approximately 4.2V/cell. Independent redundant overcharge  protection is achieved by having a separate cell protection  circuit. Cell protection circuits for single cell devices simply  include a cell voltage detection circuit and a switch to  interrupt charge current. Multi-cell batteries often include  detection circuitry that have, in addition to this switch, a 3-terminal fuse that will be blown to permanently disable the  battery pack once overcharge conditions have been detected. Overcharge protection circuitry must by necessity operate at a  voltage that is slightly above the highest allowable normal  charge voltage. The backup protection circuitry therefore  operates to interrupt charge current only after the cell is  slightly overcharged. The level of slight overcharge is  intended to be far below the threshold that is necessary to  cause a cell failure. It will, however, result in a cell that has  slightly more energy to dissipate should a subsequent cell fault  occur.


Battery design and manufacturing mistakes have also been  made with regards to charging circuit and protection circuitry. Mistakes that have resulted in overcharge include:


1. Poor routing of voltage sense wires in a multi-cell series  stack battery that bypassed the protection circuitry, and  resulted in the application of the stack charge to only a  portion of the stack.


2. A multi-cell chemistry charger that applied the incorrect  charge profile when it was unable to identify that the  battery being charged was a Li-ion battery.


3. Use of a generic connector that allowed parts from a  distributed system to be exchanged thus eliminating the  intended protection, and


4. Use of a charge regulator and protection system that was  not fully redundant, and therefore susceptible to a singlepoint failure.


AC Adapter or Power Source


Charge Regulator


Cell Protection Circuit


Lithium-ion Cell(s)


A failure modes and effects analysis (FMEA) can be an  effective tool used by many manufacturers to identify and  modify their design to reduce the probability of design related  incidents.


Relevant standards that provide minimum requirements  related to this technology include: “IEEE Standard for  Rechargeable Batteries for Cellular Telephones” [2], “Lithium  Batteries” [3], “Secondary cells and batteries containing  alkaline or other non-acid electrolytes - Safety requirements  for portable sealed secondary cells, and for batteries made  from them, for use in portable applications”[4], “Safety  Requirements for Lithium Secondary Cells and Batteries” [5], and “UN Manual of Tests and Criteria” [6].


Failure Analysis Methodology


Performing a scientific root cause failure analysis involves  systematically performing the following steps, which are  explained in detail in the following sections, to eliminate  branches from the fault tree and arrive at the root cause of a  given failure:


1. Background: Obtain background information (if  possible).


2. Exemplar Characterization: Document operation of an  exemplar unit to establish expected charge and discharge  and protection operation.


3. System Observations: Photographically document and  record observations about the incident remains.


4. Non-Destructive Analysis: Perform x-ray imaging of  cells, relevant electronic circuitry and other remains.


5. Incident Circuit Evaluation: Perform testing to assess the  operation of the AC adapter and charge regulator.


6. Incident Battery Analysis: Open the battery and inspect  and document all of its components, heat patterns, evidence of venting, and damage. Testing of the cell  protection circuitry should be performed to the degree  possible.


7. Cell Analysis: Evaluate cell(s) using non-destructive and  destructive techniques and gather all available  information contained in its remains.


8. Recreation Testing: Perform testing to attempt to recreate  the observed evidence.


9. Exemplar Analysis: Evaluate exemplar units to determine  whether a systematic defect exists that is expected to lead  to additional incidents with other in-service units. Many  of the above steps are also used on exemplar units.


10. Possible Additional Considerations: Additional issues that  may be explored under certain circumstances. A factory  audit may be desirable to explore these issues.


11. Draw Conclusions: Create a list of key facts, observations, and test results, and draw conclusions that  account for them all. State assumptions and relative  certainty of the stated conclusions. List additional  analysis that could be performed that may provide further  insight.


When followed, this general scientific methodology will  provide an experienced Li-ion incident investigator with most  if not all that can be learned about the root cause of an  incident. As a practical matter, time and cost often limit the


scope of an investigation such that the investigator must  decide what can be accomplished within the set budget  constraints. While the evidence is sometimes too badly  damaged to conclusively determine the root cause, and  multiple root causes for events often result in very similar  evidence, more often than not, we have found that credible  conclusions concerning root cause can be reached and that the  evidence that has been considered to reach those conclusions  has been well documented for peer review purposes.


Evidence that has the potential to be used in litigation should  not be altered in accordance with the principles outlined in  ASTM E860[1].


WARNING: Care must be exercised when performing any  testing that has the potential to overcharge Li-ion cells. Such  testing should only be performed by qualified personnel who  understand the associated hazards and how to safely  accommodate an overcharge event should it occur.


Background Information


Background information, when available, can provide  important information such as date of purchase or service  date, usage pattern for the incident unit, any observed  anomalies during its service history, whether the battery had  been replaced (perhaps with an inexpensive non-OEM  replacement), whether it was on charge at the time of the  incident, the type of charger being used, whether the unit had  been subjected to any recent stresses such as mechanical  impact or crush events, a description of the failure, the  location of the failure, etc. While potentially useful, experience has shown that background information from a  user is often a source of incorrect information. No amount of  assurance to some users will motivate them to disclose what  actually happened for the benefit of a scientific investigation. We have investigated and tested Li-ion products, reported in  high profile news reports to have caused injuries, that were  found to appear normal and still operate as expected. Unfortunately, it is a rare occurrence to have a consumer  admit to some events that the evidence clearly shows  occurred. Examples of where admissions are unlikely to be  forthcoming include a Li-ion product that was: dropped into a  toilet (rich in electrolytes) or other body of water, placed in a  microwave to “dry out,” dropped from a significant height, driven over by a vehicle, shot with a bullet, placed or left on a  burner or other heat source, placed close to a wood stove, subjected to multiple attempts to ignite it using a lighter, etc. While in many situations background information received  from the user is very useful in the root cause investigation, the  investigator must be cautious in relying upon such  information.


Photographs from or an inspection of the incident site will  often provide important information concerning the incident  and the product use environment. The location of the incident  and weather conditions can also provide useful information to  the investigator. For example, a Li-ion product was stored in  an unvented vehicle in direct sunlight in a hot climate.


Exemplar Characterization


The charge and discharge characteristics of an exemplar  device should be documented to allow among other things for  comparison. The minimum information required is the charge  termination voltage and verification that the charge regulator  terminates charge when charging is complete. A more  complete charge characterization can be obtained if a data  logger is used to record information such as the AC adapter (or power source) output voltage, the charge regulator output  voltage, the charge current, the temperature of the cell(s) during charging/discharging, and the ambient temperature.


It is also important to test and document how the redundant  protection circuit works in the event that the charge regulator  fails to limit the voltage to the cell(s) being charged. The tests  are often performed substituting the charge regulator with a  voltage and current-controlled power supply.


Normal discharge characterization and testing to demonstrate  operation of the overdischarge protection circuitry is  sometimes relevant. An environmental chamber may also be  needed in order to characterize operation of charge/discharge  inhibit features based on temperature.


System Observations


Recording observations about the “as received” condition of  the incident evidence is both useful and necessary to provide a  reference for future examination. Numerous photographs  should be taken to document general overview images and to  clearly record all of the specific observations made. Thorough  documentation at this stage is critical since numerous  subsequent steps will permanently alter the evidence as it is  disassembled and opened to allow further analysis.


Features to look for and document include overall thermal or  burn damage patterns, evidence of denting, openings in  enclosures that indicate the vent path, whether heat damage  was caused by internal heat from a cell or other overheated  component or from an external heat source, the orientation of  the product when polymers softened due to heat, etc. Examination for features or damage that indicates that the  product was abused prior to the incident should also be  performed at this time. Such indications can often be subtle as  they are often masked by the damage caused by the ensuing  event. Typical indications of mechanical abuse include dents  or cracks that cannot be explained by the incident. Dents in a  cell’s metal housing may often be masked or erased due to cell  swelling during the event. Indications of heat damage that  preceded an incident may also be masked by the damage  caused by the ensuing incident.


Some products are equipped with an internal indicator to show  whether it was subjected to moisture intrusion (including  moisture used during extinguishment efforts).


Non-Destructive Analyses


Overall x-ray imaging of the incident battery and cells, circuit  boards and surrounding damaged regions can provide valuable  information concerning the condition of components that are  not visible beneath the remains of a charred or damaged  plastic enclosure. Cell images provide overall damage and


vent patterns in the cell electrode winding. Circuit board  images provide information concerning whether or not a  propagating circuit board fault [7] may have occurred during  the incident. X-ray images also provide the ability to quickly  and easily determine the condition of various electronic  components such as 3-terminal fuses, and the condition of  bond wires within a component.


Circuit Evaluation


The goal of a circuit evaluation is to determine whether the  incident product’s circuitry adequately protected the Li-ion  cell(s) prior to the incident. Such testing is not always possible  since the circuits of interest are sometimes damaged during an  incident. Chief in the circuit evaluation is to determine  whether the charge regulator was functioning to correctly  charge and terminate charge to the now failed cell(s). The  charge circuitry should be carefully inspected to determine  whether it was damaged in the incident before it is powered  for testing. Figure 2 shows a correctly operating charging  profile from a 3-series-cell incident unit that was connected to  an exemplar battery for a charge regulator characterization  test. The cell voltage traces, VH, VM and VL, are  superimposed on each other as would be expected for cells  with balanced capacity.


0:00


1:00


2:00


3:00


4:00


5:00


6:00


Time (hh:mm)


-0.2 0


Vpack


VH


VM


VL


Vadaptor


Iadaptor


Figure 2. Incident system charging characterization.


Battery Analysis


Visual examination and detailed photo documentation  throughout this step are extremely important, because the  battery pack will be permanently altered when it is  disassembled. General damage patterns in addition to specific  observations (such as a housing breach or mechanical damage  to metal parts including cell housings) should be  photographically documented. Every attempt should be made  to minimize the alterations and additional damage caused by  opening a battery. Cell voltage(s) should be recorded when  the battery is first opened. An ultrasonic knife has been found  to be very helpful in the post-incident opening of today’s  consumer Li-ion products.


The interior and exterior of a battery should be checked for  evidence of electrolyte leakage. Loss of electrolyte may not  immediately result in the loss of functionality in a cell. Thus a  battery pack may continue to operate as electrolyte migrates  onto the adjacent protection circuitry. Electrolyte  contamination on adjacent protection circuitry causes  unintended parasitic conduction paths between nodes at  different potentials. Such parasitic paths have been found to


incapacitate protection circuitry, shift operating points, and in  some cases initiate a propagating circuit board fault [7] that  caused significant heat damage and even venting of an  adjacent Li-ion cell.


Additional x-ray imaging of the battery protection circuit  board may be performed during and after disassembly, since  key features may have been obscured when the battery was  intact. Also, new observations during disassembly may help  identify areas where higher magnification x-ray imaging is  appropriate.


When not damaged, the cell protection circuit must be tested  to evaluate its protection functionality against overcharge, over-discharge, short-circuit, cell imbalance, temperaturebased restrictions, etc. Figure 3 shows a typical oscilloscope  image in a single cell application in which the battery  protection circuit correctly operated to terminate charge when  the cell became slightly overcharged. The protection circuit  interrupted the charge voltage to the cell when the cell voltage  reached 4.35V. The over-voltage protection trip point thus can  be obtained to verify whether it is within the designed range  or not. When so equipped, all available recorded battery data  should be harvested. Some battery packs are equipped to  record cycle information, temperature of operation, noted  exceptions, and various conditions leading up to the incident.


Figure 3. Over-voltage protection trip point test, CH1-pack  voltage, CH2-cell voltage.


Cell Analysis


The cell(s) from the battery will typically be further analyzed  and may include:


1. Voltage, impedance, weight, and capacity measurements  as appropriate.


2. Evidence of electrolyte leakage such as salt accumulation, discoloration of cell sleeving material and plastic  housings, and corrosion.


3. Cell indentations, swelling, rupture, or other mechanical  anomalies.


4. Controlled vent operation evaluation.


5. High resolution x-ray examination of the cell that may  include imaging at various rotational angles. X-ray  imaging can reveal metal particulate contaminants, assembly problems, tab routing or dimensional anomalies, structural problems, and electrode winding alignment, as  well as incident disturbance patterns.


6. Computed tomography (CT) scanning to reconstruct a 3-D damage pattern of the incident cells and prepare for  destructive inspection of cell remains. High resolution  images may also reveal foreign contaminants inside a cell.


7. Cell disassembly and microscope inspection of cell  remains. The copper electrode typically survives a cell  overheating and venting incident and is therefore  available for further inspection. An examination of  incident cell remains or exemplar cells may include:


a. Evaluation of the overall damage pattern of the  remaining cell electrodes;


b. Microscopic inspection of the copper electrode  looking for signs of melted copper. Figure 4 shows  the typical appearance of a melted copper electrode. The signature thickened and rounded edge is an  indication of electrical faulting activity. Alloying  with the aluminum electrode causes the copper to  melt at a lower temperature, which can result in  regions of missing copper electrode.


c. Cross-section analysis allows the cell electrode  windings, active materials, and separator to be  viewed as they were while it was operating. Variations in active material thickness, gaps in the  active material, contaminant, and regional chemical  analysis on exposed surfaces can provide valuable  insight into mechanisms of failure.


d. Examination for signs of any manufacturing  irregularity, including electrode tab attachment, geometry, routing, etc.


e. SEM (Scanning Electron Microscope) or optical  microscopy imaging of key features identified during  visual inspection.


The new deprocessing approach successfully established the  fail mechanism of the functional failures. The unattenuated  laser beam transmission through the waveguide effect of  stacked silica fillers provided a way for direct interaction of  the scribing laser beam and the die surface. The localized  melting of the die metallization caused metal shorts leading to  the observed functional failures.


The author wishes to acknowledge Intel Philippines FMG  Q&R for the support especially to the Failure Analysis, Assembly, Test and Materials Engineering teams for their  invaluable contributions to this paper


[1] Marton, L., and A.B. El-Kareh.  Electron Beam and Laser


Beam Technology.  New York: Academic Press, 1968.


[2] Rubahnmpi, H.G., and H.G. Rubahn.  Laser Application


in Surface Science and Technology.  New York: John


Wiley & Sons, 1999.


[3] P. Paranal, Intel Internal Document. 2006.


[4] R. Ricci, M. Ditzler, L. Nestor. Discovering the BeerLambert Law. Journal of Chemical Education 71


(November 1994):983-985.


[5] L.D. Landau and E.M. Lifshitz, Fluid Mechanics,2nd Ed.


(Pergamon Press, Oxford, 1987), Chap. V.


[6] L.Zhigilei, et al. Computer Modeling of Laser Melting  and Spallation of Metal Targets. Invited Paper. SPIE


Proceedings, Vol. 5448 (2004).


[7] CRC Handbook for Chemistry and Physics. Online


version.


A Novel Technique for Determining the Location of a Hermetic Leak in a ‘Metal  Can’ (TO-x) Package


Root-cause analysis of hermetic leak failures is complicated  by the difficulty in isolating the leak location. Standard dye  penetrant inspection is not consistently successful. The  addition of pressure to the dye penetrant, followed by  metallographic mounting and preparation, and subsequently  followed by vacuum storage, greatly enhances the visibility of  the dye and more effectively decorates the leak location.


While molded plastic packaging is today the dominant option  for integrated circuit (IC) enclosures, the materials used do not  offer significant resistance to penetration by water vapor. For  very high reliability IC applications, hermetic enclosures that  are moisture-impermeable are required. In such a package, the  die rests on a substrate in an air enclosure, i.e. a “package  cavity”. The effect of the hermetic seal is to prevent gases and  liquids from entering the package cavity containing the die. The materials used also typically allow hermetic packages to  withstand higher temperatures than plastic packages [1].


One type of hermetic package uses a metal base enclosed by a  metal lid, often called a ‘metal can’ structure. These are a type  of transistor outline (TO) package. An example of such a  package is shown in Figure 1. The pins that connect the IC to  the outside world are fixed in the package base using glass  materials to make an impermeable seal. Figure 2 shows a  cross-sectional view of such a seal. The integrity of the  various seals is tested by, among other methods, pressurizing  the part in a helium atmosphere and detecting the evolution of  helium from the part after pressure is removed [2]. If the  amount of helium detected exceeds a defined rate, then some  portion of the overall hermetic seal is leaking. These leaks can  be caused by a number of mechanisms including, but not  limited to, delamination or cracking of one of the pin glass  seals, porosity in the glass, or cracks in the lid weldment. Establishing the root cause of such a failure is essential to  ensuring that there are no inherent problems in part  manufacture and to improving future yields in subsequent  assemblies. Thus, the ability to identify the specific location  on the part where a seal is leaking is an important element of  failure analysis.


Figure 1: TO-3 hermetically packaged part. The construction  is typical of all metal packages. Note glass seals surrounding  the pins at their penetration points on the metal base.


Bond Wire


Figure 2: Cross-sectional view of glass seal on a pin in a  hermetic metal package.


Dye penetrant has been used for many years in failure analysis  to identify the location of fine cracks. Dye is placed on the  surfaces of interest, where capillary flow draws dye into the  crack. This can be augmented by pressurizing the part after  Pin


Package Base


Glass


dye application to force dye into the cracks. Once the  recommended dwell time has expired, the dye is wiped off, after which the part is optically inspected for evidence of dye  remaining on the surface. If fluorescent dye is used, then the  inspection proceeds under illumination by ultraviolet light. Unfortunately, most dyes do not have good contrast with the  glasses used in pin seals and cleaning of the part surface is  complicated by the size and shape of TO packages. Any  circumferential delamination or crack along the glass interface  with the pin or the package base is difficult to distinguish due  to the optical discontinuity between glass and metal. The  failure may also be extremely small and thus may not decorate  well. This may still be the case even if developer is used. Consequently, techniques that can increase the visibility of the  penetrant at the failure location will improve the ability of the  analyst to detect the precise location of the failure and, ultimately, to identify the failure mechanism.


The enhancement described in this paper that can improve the  likelihood of identifying a leak location is to supplement the  basic pressurized dye penetrant inspection with additional  metallographic preparation and subsequent vacuum storage. This draws out the dye accumulated in the crack and at the  internal package base, creating a film on the failing interface  instead of a fine line.


The procedure for enhancing dye decoration is given in the  following description. The part used in this description was a  15-pin TO-3 package similar to that shown in Figure 1; the  method should produce similar results for any TO-x metal can  package.


Dye Penetrant Inspection


The part is first liberally coated with the dye penetrant of  choice. The dye selected for this analysis was an optical dye  with a red color, Magnaflux SKL-SP1. After application, the  part was pressurized to 40 p.s.i. for 24 hours, after which the  part surface was cleaned with an acetone rinse. No developer  is applied. At this point, the part should be inspected for any  obvious evidence of crack decoration using a  stereomicroscope. If nothing is revealed by the inspection, then the metallographic preparation may proceed.


Optical inspection of the TO-3 part after pressurized dye  penetrant application revealed a suspect pin, but a visual  inspection of the pin seal did not reveal a failure mechanism  and specific failure location. The pin of interest was marked  with a sawn notch on the side of the package base at the pin  location.


Metallographic preparation begins with mounting the part in  epoxy. The total sample size cannot exceed the size of the  epoxy mounting fixture to be used in the process, typically a  1-¼ inch diameter hard plastic or disposable cup. Such cups  are shown in Figure 3. The size limit is given to minimize the


amount of grinding time and media required to clear away  unwanted portions of the mount. Because of the size limits,


Figure 3: Typical 1-1/4 inch two-piece hard plastic and onepiece disposable mounting cups. Part shown in Figure 1 has  been cut to fit either of the cups.


Pin of  interest


Notch


Side of  package


Figure 4: Side view of a metallographic mount showing a  sawn notch on the side of the encapsulated TO3 package. This  notch indicates the position of the pin of interest in this  analysis.


the sample may need to be reduced in size; this is particularly  true of TO-3 cans with large flanges for screw holes. This is  typically done using a diamond saw.


The sample is then loaded into the cup, pins up, and epoxy is  poured into the cup over the part and covering the pins. Any  epoxy with good edge retention characteristics should work. To enhance edge retention, the epoxy was vacuumimpregnated for five minutes in a partial vacuum ranging from  25 to 30 inches of mercury.


To facilitate later preparation, the epoxy should cure clear, though translucent epoxies will also work. A final as-cast  mount is shown in Figure 4.


Grinding and Vacuum Storage


After curing, the mount is removed from the cup and prepared  using standard metallographic techniques. If the pins are not  completely encapsulated by the epoxy, then they may be  trimmed to the top of the mount using a diamond saw and  applying light pressure. It is important to keep loading to a  minimum in the saw to minimize the chance of transferring  stress to the glass seals and introducing cracking as an artifact. While this is a very small risk, it should be eliminated if  possible.


This mount was prepared using six-inch silicon carbide wetdry paper secured to grinding wheels turning at 270 RPM. The  grits used progressed downward from 320 to 600 as the mount  thinned. This was monitored by inspection using a  stereomicroscope. This part of the preparation was timeconsuming, as the entire length of the pins had to be ground  away. Although the epoxy holds the pins in place with respect  to the base, there is still some limited flexibility in the  material. Thus, excessive pressure in the grinding process  should be avoided as much as possible to avoid any risk of  crack artifacts, perceived or actual.


The partially ground mount is shown in Figure 5. This image  also reveals the presence of dye dissolved into the epoxy prior  to curing, which raises a concern regarding this technique. If  the epoxy has displaced the dye in the leak location, then it  may prevent the later use of vacuum to draw the dye out. With  this in mind, it was decided to grind the mount partially into  the glass seals, removing the curved meniscus at the bottom of  the glass and leaving a flat surface across the glass. This  would act to remove any epoxy at or near the surface of the  leak. It also serves the added purpose of removing all surface  epoxy from the glass, ensuring that the defective area of the  seal is completely exposed. This process is shown  schematically in Figures 6 and 7. Upon reaching the glass  seals, the part was prepared at 600-grit into the seals on both  the pin and the package base interfaces. The completed  preparation is shown in Figure 8.


At this point metallography was halted and the mount was  placed in vacuum storage at 28 inches of mercury. After 24  hours of vacuum storage, the part was again inspected. Inspection revealed that two points on the seal of interest were  decorated with red dye films. These locations are shown in  Figure 9. Once decorated, the cracks from which the dye  emerged also became more clearly visible, as shown in  Figures 10 and 11. This is important in that it supports the  finding that the cracks were in place prior to mounting the  part. Because the dye is being drawn through the cracks, the  dye had to be present in the crack before mounting, and thus  the cracks could not possibly be preparation artifacts.


Dissolved Dye


Figure 5: View of the plane of section for the mount shown  in  Figure 4. The suspected failing pin appears to be dissolving  dye penetrant into the mounting epoxy. Notch location shown  at arrow.


Figure 6: Schematic of glass seal shown in Figure 2, mounted  in epoxy.


Figure 7: Diagram in Figure 6 now prepared into the seal  interfaces. Epoxy in seal is likely cleared and the  metallographically flat surface will facilitate inspection.


y


Seal Interfaces


Plane of Section


Epoxy


Figure 8: Mount ground through 600 grit into the glass seal. Notch shown at arrow.


Figure 9: Area shown in Figure 8 after 24 hours of vacuum  storage. Note the presence of dye penetrant drawn from within  the package cavity (shown at arrows).


The large quantity of dye that migrated to the surface suggests  that the dye was present as a significant deposit inside the die  cavity on the inner crack surface, where the initial  pressurization of the dye forced it. This would mean that the  technique can be readily applied to more subtle leaks, such as  those along the package-to-glass or pin-to-glass interface that  would not otherwise be visible to visual inspection.


While the procedure has proven successful, the details  specified are not necessarily the best or only steps that can be  taken to generate useful results. There is room for a great deal  of flexibility in the procedure and for experimentation with  different materials and techniques.


Figure 10: Higher magnification view of upper crack shown   in Figure 9. Visible portions of the crack not obscured by dye  penetrant are shown at arrows.


Figure 11: Higher magnification view of lower crack shown   in Figure 9. Visible portion of the crack not obscured by dye  penetrant is shown at arrow.


Leaks in hermetic packages are difficult to locate for detailed  analysis. Dye penetrant testing alone is not always sufficient  to reveal the leak location. This enhanced technique utilizes  pressure to cause an accumulation of the dye inside the crack  and/or the cavity of the package of a hermetically defective  part. The part is then metallographically mounted and ground  parallel to the outer surface of the seal until all of the seal  interfaces are exposed. The mount is then stored under  vacuum, which draws the dye back through the leak location, decorating the surface of the mount at the exact failure  location.


This technique was successfully applied to a part to identify  the specific location and cause of a hermeticity failure in a  TO3 package. Inspection after preparation revealed two cracks  in the seal that the dye penetrant decorated when pulled out of  the package interior by the vacuum. In particular, the dye  spread across the surface of the part at the crack locations, revealing them to optical inspection using a stereo-zoom  microscope.


I thank my colleagues at National Semiconductor for their  support; in particular, Kevin Weaver for performing the initial  dye penetrant analysis of the part described in the paper, and  Ted Hasegawa for his input on the documentation. My thanks  also to Gwen Nail for her assistance with editing and  photodocumentation.


A note on the passing of Dr. William D. Forgeng, Professor  Emeritus, California Polytechnic State University, San Luis  Obispo, who left us last July. He taught metallography and  metallurgy to this author and an entire generation of students  at Cal Poly. Upon learning of his passing, I made a nostalgic  review of my laboratory notebook from his class on NonDestructive Testing…and found a factual error I had  inadvertently included in an early draft of this manuscript. Even from the great beyond, he is still correcting papers. He  will be missed.


[1] Application note MS011795, Hermetic Packages, National Semiconductor Corporation (Santa Clara, CA, 1999), p. 1.


[2] United States Department of Defense, Mil-Std-883G, Method 1014.12, Test Condition A (2006), pp. 1-7.


BGA Package Level Failures Due to Contamination


Jodi Roepsch


Raytheon, McKinney, TX USA   j-roepsch1@raytheon.com


Two instances of BGA package level failures were identified  during in-circuit electrical test.  The electrical opens occurred  as a result of contamination issues originating at the board  supplier.  Analytical techniques including optical inspection, SEM/EDS, Raman and FTIR were key in identifying  photoresist on the board surface in the first case study and  nickel carbonate contamination on the board surface in the  second case study.  In the first case study, resolution was  achieved with a Plasma etch process.  In the second case  study, CCAs were cleaned with a wet chemical etch process  formulated specifically to attack the nickel carbonate.


Complex Circuit Card Assemblies (CCAs), such as those with  greater than 30 layers and containing multiple high dollar  parts, are expensive to produce.  Consideration needs to be  given to such factors as the cost of materials, labor, assembly  equipment, utilities, etc.1  Occurrence of excessive scrap  adversely affects both cost and schedule.  As a result, rework  should be a consideration in some cases.


This paper will discuss two specific case studies where incircuit test revealed failures isolated to individual Ball Grid  Array (BGA) I/Os.  Typical failure analysis techniques were  carried out2 identifying contamination at the board level.  In  one case, a rework procedure was developed for the raw  Printed Wiring Board (PWB) prior to component assembly  with no risk to reliability.  For the second group, the  assembled CCAs were reworked with a somewhat aggressive  process.  This resulted in product with a potential reliability  risk due to nickel corrosion if the gold plating was not  continuous.  The risk was deemed acceptable since these units  would be engineering units only.


Typical manufacturing processes were implemented in the  build up of the PWBs and are outlined in Fig. 1 below.3


Once the failures were identified by in-circuit test, a failure  analysis plan was implemented including optical inspection, Scanning Electron Microscopy (SEM), Energy Dispersive  Spectroscopy (EDS), Raman Spectroscopy and Fourier  Transform Infrared Spectroscopy (FTIR).


Figure 1:  Process flow of typical procedures.


Case Study 1


Once in-circuit test identified a failure, the component and  PWB were both examined.  The component was then removed  via Hot Air Vac.  After component removal, the solder  typically has a rounded appearance resulting from its surface  tension.  In this case, the appearance of the solder on both the  BGA package and PWB were very flat in appearance.  This  led to further investigation.  (Fig. 2 and 3)


Figure 2 – Optical image of BGA removed from failure


location.  The solder has a flat appearance after Hot Air Vac  removal.


Figure 3 – SEM image showing solder on BGA has a flat  appearance after removal from PWB.   Hot Air Vac removal  will change the appearance of the solder but a flat


appearance is atypical.


A CCA was cross sectioned through the assembly capturing  several BGA solder joints.  A single bump was imaged in Fig.


4.  There was clear evidence that the solder from the BGA did  not mix with solder plate on the PWB pad.  (Fig. 5)  The grain  structure varied with the BGA solder ball having large grains  and the solder plate on the PWB having a very fine grain  structure.  The solder plate screen printed onto the board is a  60/40 Sn/Pb solder alloy while the BGA solder ball is a


SnPbBi alloy.  Also noted was a demarcation line between the  two solders indicating separation between the solder ball and  solder plate.  This data suggested contamination was present  either on the BGA solder ball or the PWB pad inhibiting joint  formation.  A device was pried from the failed board and both  the component and board examined.  Evidence of a low  weight material was identified on both the board and solder  ball.  (Fig. 6 and 7)  Raman Spectroscopy concluded this  material to be flux. (Fig. 8)  This data did not lead to  identifying a source of contamination contributing to joint  failure.  Therefore, boards and BGAs from stock were  examined for any evidence of contamination.


Figure 4 – Cross sectional view of failed BGA solder joint.


Figure 5 – High magnification view of solder joint.  The


screen printed solder on the PWB and solder ball from the  BGA did not mix.  The screen printed solder is in the lower  half of the image (small grains) and the BGA solder ball is in  the upper half of the image (large grains).


Figure 6 – Backscattered electron SEM image of PWB pad  after device was pried up.  The dark areas are a low weight  material on the pad surface.  Raman indicates flux is present.


Figure 7 – Backscattered electron SEM image of solder ball  after device was pried up from board.  The dark regions are a  low weight material on the solder ball surface.  FTIR


indicates flux is present.


At this point in the analysis, it was deemed necessary to begin  a stock screen of BGAs by SEM.  No evidence of  contamination was identified.  (Fig. 9)  On the other hand, a  stock screen of the PWBs identified a thin film low weight  contaminant.  (Fig. 10)  The thin film was not identified  initially because it was too thin for FTIR detection.  EDS  under low keV conditions determined the material contained  carbon and oxygen.  (Fig. 11)  Since the film was too thin for  detection by Raman and FTIR, a source could not be  conclusively determined.  The film was only observed on one  side of the board.  Once the thin film was identified on boards  from stock, it was obvious in Figure 6 that it was present on  the failures as well.


Figure 8:  Raman Spectroscopy determined the contamination  identified by SEM/EDS is flux residue.


Figure 9 – Image of solder balls on the BGA component.  No  evidence of a low weight contaminant observed by SEM/EDS.


Figure 10 – SEM image of board from stock.  The dark gray  areas on the BGA pads are a low weight contaminant.  This  material was only observed on one side of the board.


Discussions with the supplier indicated a particular process  step in which photoresist is placed on one side of the board to  protect the solder plate during etching.  The data suggested a  thin film of photoresist was left behind on the board.  Once  the source of the contamination was identified, a cost effective  solution was necessary to clean the boards in stock.


Figure 11a – Example EDS spectrum showing carbon and  oxygen are present in the thin film.  The thin film has peeled  up and folded back onto itself at the location of EDS  inspection.


Figure 11b – Spectrum of thin film indicates C and O present.


Plasma Cleaning Process


The boards were cleaned in an aggressive plasma etch  process.  The boards were placed in a direct plasma  configuration and were cleaned using oxygen and argon gases  at relatively high power settings.  The process took  approximately 1 hr total to run.  Each board was cleaned in  this aggressive process 3 times on the contaminated side and 1  time on the other.  Oxygen plasma is typically used to remove  organic contaminants.  Argon is then used to remove  inorganics.4


Plasma cleaning of the boards was sufficient to remove the  residue.  No evidence of the photoresist could be seen at low  keV by SEM after cleaning.  (Fig. 12)  Once the cleaning  process was deemed successful, all boards in stock were  plasma cleaned.  The supplier subsequently eliminated the  photoresist step in the process by etching both sides of the


board at the same time.  No additional solderability issues  have been identified to date.


Figure 12:  Board from stock after having been plasma  cleaned.  Low keV SEM imaging indicates majority of thin  layer contaminant has been removed.


Case Study 2


In-circuit electrical failures of an assembled board led to an  investigation into root failure cause.  Testing identified  electrical opens at BGA solder bumps to the PWB interface.  Investigation determined poor solder connection of the BGA  solder bumps to the gold plated PWB pads.  Gold is known to  readily absorb into molten SnPb solder making it a desirable  surface finish.5  This property of gold absorption into solder  and the lack of solderability to the pad indicated  contamination as a possible cause of failure.  Not surprisingly, contamination was identified on the PWB pad surfaces which  had originated at the unfilled vias.  The cracked flaky  appearance of the contaminant indicated the material was at  one time in liquid form. (Fig. 13)  A typical joint results in the  SnPb solder bump wetting to the pad on the PWB by  absorbing the gold plating and forming a Sn/Ni intermetallic  with the underlying nickel plating.    In instances where the  pads on the board contain contamination, the solder was  unable to wet and no solder joint was formed.  Elemental  analysis determined the contamination contains C, O and Ni.  (Fig. 14)  FTIR identified this material as nickel carbonate. (Fig. 15)  The source of the nickel carbonate was isolated to  the plating house but the exact cause could not be identified.  The supplier indicated a carbonate material was used to cure  the solder mask but the composition did not match the  contamination identified on the boards.


Considering costs to manufacture this type of board as well as  time restraints, it was necessary to formulate a cleaning  process in an attempt to salvage the CCAs.  The failure  occurred due to contaminant becoming trapped in the rather  small 7 mil vias.  At a later time, the contaminant leached onto  the pad surface resulting in poor solderability.  Investigative  studies into various acidic solutions led to success with a 10% Hydrochloric Acid solution.  The HCl solution was allowed to  react on the pad for 2 to 4 minutes.  The assembled board was


placed in DI water for a minute followed by the CCA wash.  Damage was only identified from the 10% HCl cleaning  process in instances when the gold plating was cracked or  flaking allowing underlying Ni to be attacked.  A  microsyringe was used to isolate the acid to a contaminated  pad thereby reducing the risk of damage to the board.    Although some damage to the pad was observed on the rare  occasion, this cleaning technique was deemed acceptable  since it would be restricted to test units and would not be used  on fielded units.  Successful cleaning of pads allowed multiple  boards to be returned to process flow and later installed in test  units resulting in a significant cost savings to the program.


Figure 13:  Low magnification image of contaminated pad on  PWB.  The bright areas have an elemental composition of  gold while the dark areas on the pads consist of nickel  carbonate contamination.  The contamination is leaching  from the via spreading onto the board surface.


To avoid reworking future lots, the PWB design was modified  to require filled vias.  There have been no additional rework  or failures due to carbonate contamination of PWBs since the  design change.


Figure 14a:  EDS data suggests the presence of C, O and Ni  on the gold plated surface.


Figure 14b: Spectrum 1 acquired on the pad surface.


Figure 14c:  Spectrum 2 demonstrates the composition of the  contamination in the via.


Figure 15:  FTIR suggests the material is nickel carbonate.


In both instances, the root failure cause was related to process  issues at the supplier.  In the first case study, a photoresist  material used to protect the solder on one side of the board  during an etch process was not completely removed by the  supplier.  A plasma clean was sufficient in cleaning the  photoresist from the solder allowing boards in stock to be  used.  The board supplier changed processes on future builds  by etching both sides of the board simultaneously eliminating  the need for the photoresist.  No future failures were identified  after this process change.


The second case study also was a failure initiating at the  supplier.  Material was trapped in vias due to their small  feature size, later leaching out onto the board surface.  The  source of the carbonate material was never fully understood  but could be isolated to the supplier.  Once the vias were filled  by the supplier, future failures were no longer identified.  A  rework process involving 10% HCl was carried out on failed  CCAs improving the solderability with replacement BGAs.  There was some concern with using this cleaning method  which was thus restricted to engineering boards only.


I would like to thank the following for their contributions:  Robert Champaign, Marlin Downey, Richard Fay, Derek  Johnson, Alyson Tuttle, Barbara Waller, and John Wolfgong.


[1]  Gilleo, K, “Area Array Packaging Handbook”, McGraw-Hill, (2002). pp.29.3, 29.12.


[2]  Roepsch, J., Snively, C. Todd, Champaign, R., “A  Systematic Approach to Failure Analysis”.  SMTA  Boston Conference Proceedings, June 2002, pp. 213-219.


[3]   Luke, Mike, “Printed Wiring Boards Technology I”. March 2007.  Raytheon. 13510 N Central Expy, Dallas, TX 75243.


[4]   Tuttle, Alyson.  Personal Communication.  Raytheon. 13510 N Central Expy, MS409, Dallas, TX 75243.


+ ΔV2 between t3 and t4, keep V + ΔV2 until t5, then ramp down  to V between t5 and t6 and stay there until the end. The  common mode or mid level for BF<7> and bBF<7> follows  the stimulus for RFAULT values from 1kΩ to 10kΩ. The  behavior changes for the RFAULT values of 20kΩ in the timing  range between t4 and t5. The voltage levels of the BF<7> and  bBF<7> lines are now determined by the voltage dividing  resistances of the transistor output resistances and the short  resistance. The output resistance is modified by the changed  gate supply voltage and the lines spread giving a decodable  fuse signal. This is the failure mode. After bumping back to  the nominal supply voltage between t5 and t6, the failure mode  is reversed by a lower BF<7> signal and the pass condition is  reached again. At this point, it remains unclear why the BF<7>


and bBF<7> signals are not returning to the original values  that they had before t4. To confirm this failure mode and this  simple model, AFM probing is used to determine the shorting  resistances in a two point measurement.


Figure 6: Timing diagram of an analog simulation for the  blown fuse address BF<7> and bBF<7>. The stimulus is the  supply voltage V(t) of the circuit.


AFM (atomic force microscope)- Probing and Root Cause  Investigation


In order to perform electrical measurements on contact level, a  Multiprobe AFP with four available probes was used.


Firstly, current mapping of the region of interest with an AFPprobe was performed. This region is scanned with a W-tip and  simultaneously the current flowing between sample and the tip  is measured and mapped [3]. The measurement was done by  applying a bias voltage at the AFP-tip of 1V (Fig. 7). The sign  and height of the tip current is included via the different grey  shades. The brighter contacts are p-well contacts able to carry  higher currents to the p-lightly doped substrate. The darker  gray contacts are connected to n-diffusion region and they  form with the p-well a direct biased diode. Additionally, 5 gate  contacts appear in the current map. They are faulty gates  contacts as they are not floating. All other gate contacts are not  visible in the current map. It seems that the faulty gate contacts  are connected to the drain/source contacts, because they have  the same grey shade like the larger contacts which run  horizontally in the centre of the image.


I-V measurements between contact “1” and the p-well contact  by AFP (atomic force probing) show a diode behaviour of the  n-p junction (Fig. 8a). This diode curve can also be measured  between any GND-contact and the p-well. All contacts 1 to 5  have a connection to the n-contact region. The contacts 1 to 5  are shorted between each other confirmed also by AFP (Fig. 8b). These measurements show ohmic shorts of 12.5kΩ (8µA  at approximately 100mV) which is in the range of the  simulated resistor values.


The root cause is shown in Fig. 9: the short is created by a  scratch below the STI (shallow trench isolation) in the active  area region visible after soft oxide lift-off; the gate contacts  and the gate oxide are still there and visible. The scratch was  produced during the planarization of the STI-oxide through a


fuse latch


address bus


blown fuse address <7,8>


blown fuse address b<7,8>


RFAULT


address  decoder


CMP (chemical mechanical polishing) process. The scratch  connects in total five gates. The fifth gate is missing in the  image at the circled position. It has been accidentally removed  during the lift-off.


Figure 7: Current mapping with AFP.


a.


b.


Figure 8: I-V plots of measurements between contact 1 and  the p-well contact in a) and the contacts 2 and 3 in b).


Figure 9: SEM image after oxide lift-off showing the scratch  that shorts the failing gates


Local shorts in the 10kΩ range after the fuse latch between the  fuse and inverted fuse information line cause an instable fail  situation: The fuse information is not properly outputted and  can be influenced by voltage bumps. The voltage trimmings  during test results either in a correct or induce a wrong  decoding and fails may occur.


The localization is achieved through knowledge based failure  analysis. A soft defect localization technique for this kind of  functional fails would be beneficial and is under development.


[1] J. Segura, C. F. Hawkins, “How it Works, How it Fails”,


IEEE press, 2004.


[2] J. Colvin, “A New Technique to Rapidly Identify Gate


Oxide Leakage in Field Effect Semiconductor Using a


Scanning Electron Microscope”, ISTFA Proceedings,


1990, pp. 331-336.


[3] Jon C. Lee, J. H. Chuang “Fault Localization in Contact


Level by Using Conductive Atomic Force Microscopy”,


ISTFA Proceedings, 2003, pp. 413-418.


Fault Isolation of Soft P-N Junction Break Down Due to Plasma Charging


Dat Nguyen and Taras Dudar


Texas Instruments Inc., Dallas, Texas USA Dat1998@yahoo.com


The P-N junctions are part of the construction of semiconductor devices. They are formed by the combination of P-type and N-type diffusions. P-N junctions exist in both digital and analog circuits. In this paper, we will discuss a soft(small early conduction) P-N junction breakdown. The P-N junction in this work is a part of a differential amplifier, which is widely used in Analog/Mixed signal devices. An N-P-N Bipolar Junction Transistor (BJT), for example, is made up of N-type, P-Type, and N-type diffusions. The P-N junction of interest in this report is part of an Analog circuit called a differential op-amp [1]. This circuit is designed to accept 2 input signals and to produce an output that is proportional to the difference between the 2 inputs (Figure 1).


Figure 1: A simple differential amplifier [1]. The drawing on the left is the differential amplifier symbol, and the drawing on the right is the electrical schematic.


A typical failure of a differential amplifier could be measured by the Output Offset (OO) voltage. However, when the offset voltage is well within the specification, the failure could be difficult to detect. It is even harder in the case where emitters are connected in parallel to make up a large BJT for the differential amplifier. In our case, there was a failure in one of the 240 parallel emitters (Figure 2) that has degraded the performance of the differential amplifier. There were two different device types with different failure modes were submitted to Failure Analysis (FA). In one case, a device type was submitted for analysis of OO failure mode, and in the other case, the device was submitted for no output failure mode. Both of these failure modes were eventually traced to the same soft junction failure of an emitter in the 240 emitter array. The differences in the failure mechanism were also correlated to the differences in the values of the input dynamic range for those two device types. The paper will outline the test techniques to detect the differential amplifier failure, the circuit analysis (design and simulation), the fault isolation, and the root cause analysis with data from the wafer fabrication process to support plasma charging on the emitter.


Figure 2: The image on the left is a typical BJT and the image on the right is a BJT with parallel multiple emitters. The top row shows the corresponding layout of N-P-N BJT.


C=Collector, B=Base, and E=Emitter.


Differential Op-amp Failure Mode


Failure analysis labs often receive devices with a variety of failure symptoms. However, there are cases where 2 or more symptoms are the result of the same failure mechanism. In this case, the same failure mechanism in two differential op-amp devices resulted in two distinct failure modes: out of spec OO for one and no output in the final stage of the 3 stage differential op-amp for the other.


The differential op-amp in this analysis was a typical three stage op-amp as shown in Figure 3. The first stage input differential pair was comprised of two big multi emitter NPN BJT transistors. Each transistor was laid out as 240 emitters connected in parallel. When one (1) of the 240 parallel emitters failed, it degraded the performance of the differential op-amp. The degraded performance was seen as OO or no output in the final stage.


Figure 3: A simplified 3 stage differential amplifier circuit.


V11


V12


Vs


VsVout


V21 V22


Vs+


VsV31 V32


Vs1st


2nd


3rd


Rf1


Rf2


Failure Analysis


The failure analysis followed the typical process of failure verification on the bench, which included bench measurements of the output voltage and the OO. Externally, the inputs and the outputs of each stage could be measured and tested though a special test mode. The failure mode was a no output on a 5MHz 10mV P-P AC differential signal. Global fault isolation techniques were applied, such as LASER Scan Microscopy(LSM) and Photon Emission Microscopy (PEM) analysis.


Both of these techniques were unsuccessful. The next step was to perform the circuit analysis by placing Focus Ion Beam(FIB) probe pads at various points on the three stages of the op-amp. The approach was as following: 1) to study the data base layout and schematic, 2) determine the location for nodal analysis, i.e. where to place probe points, 3) trace and locate the abnormal node, 4) isolate the circuit in question, and 5)characterize the circuit of interest. The analysis required the extensive use of the layout and schematic databases, especially the LVS (Layout Verses Schematic) helper, which links and highlights identical node between schematic and layout.


Since the soft failure on one of the emitters resulted in a very low (<20mV) DC voltage difference at the base, the fault isolation of the failed BJT required the application of external bias, nodal probing using Focus Ion Beam (FIB) pads,measurements were taken in both AC and DC formats using a Pico-probe, and finally, total isolation of the BJT in the differential pair for I/V curve trace comparisons.


From the op-amp circuitry shown in Figure 3, the first logical points to be measured were V21, V22, V31, and V32, which are the internal input nodes for 2nd and 3rd stages. Note that all measurements should be made using a Pico-probe to avoid loading on the active circuitry. The measurements were taken during an active mode while a 5MHz 10mV Peak-to-Peak (PP) AC differential signal was applied to the input. Also, with a low level sensitivity of the op-amp, varying the input’s amplitude could help to understand the working range of the op-amp. In this particular case, the failed op-amp output could be observed with an amplitude above 20mV P-P. This indicated an input offset problem. The outputs, V21 and V22 were found to be mismatched as well, although only by 90mV.


This proved that the failure came from the first stage of the opamp. With this information, various probe pads were placed inside the first stage of the op-amp to determine the various I/V levels. The amplification of the differential signal at the input required the identical BJT pair [1]. In this case there was an additional complication to the analysis. The dual input differential op-amp design, shown on Figure 4, was used in the first stage. The identification of the mis-matched BJT required the active measurement in both DC and AC modes. Also,comparison of the Vbe (Voltage drop from Vb to Ve) was needed.


Figure 4: Dual input differential op-amp. Vb1+=Vb1-,Vb2+=Vb2-.The image on the left is the same as on the right,but it is redrawn for the ease of recognition. The dashed lines indicate parallel emitters.


Measurements were taken and compared at the emitter, base,and collector of each BJT. Since the difference in the DC voltages at each node of the identical BJT pair was small (in the order of a few mV), the voltage drop, Vbe, from base to emitter was measured for each BJT. The delta of each matched pair Vbe (Vbe1-Vbe2) was also compared with another matched pair in the same op-amp. This was done to look at the integrity of the matched pair. The matched pair with a high delta Vbe is the one most likely having a mismatched BJT or one of the BJTs in the pair is bad. In this case, one input BJT pair had a delta Vbe of 10mV and the other only 2mV.


Furthermore, the Vb voltage showed a slightly (~9mV) higher voltage on the bad BJT. Forcing external current at the Base of the failing BJT during active mode operation should compensate for the voltage difference and rebalance the differential pair. For example, for the above mentioned BJT pair with a delta Vbe of 10mV, one of the BJTs had 9mV Vb higher than the other BJT. By forcing a current of 4µA at the base of this BJT, a balanced circuit and a normal output could be observed. After the bad BJT was identified, each BJT in the pair was isolated and characterized for comparison.


Using FIB, each terminal of the BJT pair was isolated from the rest of the circuitry. Once the BJT has been isolated, an I/V curve trace analysis on the P-N junction was done by forward biasing the P-N junction (Base to Emitter). In this case, an early conduction was observed between base and emitter(Figure 5). If there was a hard short or a hard leakage between base and emitter, a line through the origin would have been observed instead. The Gummel [2] plot was also obtained to present better information on the leakage (Figure 6).


The emitter in this case was laid out with 240 parallel emitters as shown in Figure 2, locating the exact faulty emitter required the combination of FIB cuts and curve tracing on base-toemitter. First, a FIB was used to cut out one row of emitters,and then an I/V curve trace from base to emitter was performed. If the bad emitter was included in the row, the I/V curve would become normal (curve 2 in Figure 5), else an early conduction curve would still be observed (curve 1 in Figure 5). The process was repeated until a failed row was found. After that a groups of emitters were cut out until a single emitter was isolated (Figure 7). Finally, the physical failure analysis of the defective emitter was performed using


FIB cross section, TEM, and TEM elemental analysis. Various attempts did not reveal any visible defects (figures 8-9).


Extensive Transmission Electron Microscope (TEM) analysis,which included chemical decoration, did not find any physical defects. Top down silicon decoration using various silicon decorating etches did not show any anomalies. An attempt to perform Scanning Capacitance Microscopy (SCM) was done without success due to the large doping profile.


Figure 5: I/V curve trace. This is a forward bias of the P-N junction, Base to Emitter. I/V curve (1) is from the leaky P-N junction where early conduction occurring at 0.35V. The curve (2) is from another BJT of the same pair.


Figure 6: Gummel plot, a logarithm of current vs base voltage. Curve 1-1 (bad BJT) is a base current and is compared against 2-1 (good BJT). Curve 1-2 (bad BJT) is a collector current is compared against 2-2 (good BJT). Note that trace 1-1 shows higher level of current leakage.


Figure 7: FIB isolation of a faulty emitter. A process of repeated cut-and-curve-trace was performed until a single faulty emitter was isolated.


Figure 8: This is an overall image of the BJT with 240 parallel emitters a contact level. Arrow points to the bad emitter.


Figure 9: High magnification image of the emitter in question(arrow). No anomalies are observed.


Simulation and Confirmation of Failure Mechanism


The FA measurement data was then input to simulation software. The failure electrical behavior can be reproduced and the results confirmed the leakage on one of the BJT pairs creating an offset. With the probe data,. During simulation,with the mismatch of 9mV at the base, forcing 4µA onto the base of the bad BJT also showed a balanced circuit and normal output. The simulation was also used to confirm the offset at the output of the first stage and the lack of the output in the final stage. The simulation also confirmed that the different failure modes (no output and high output offset voltage) were the result of the same failure mechanism. The degeneration resistor, Rd, (Figure 10) was different for those two devises which resulted in different input offset tolerances. The higher Rd provides the wider dynamic range and better Input Offset tolerance [3]. The device with a larger Rd resulted in a better offset tolerance. The output could still be detected for the same levels of input offset and the failure mode was OO out of specification. But in the other device with lower Rd and the lower offset tolerance, the failure was detected as no output.


Consequently, at test, some device types would fail OO while others have no output at all.


Figure 10: Dynamic Range/Offset Tolerance. High Rd provides wider input range and better offset tolerance.


Root Cause Analysis


Finding the root cause was a team effort from FA, Design,Test, and Fab. The failure mechanism, however, could be explained clearly using the fabrication processing data. Based on the wafer probe data and the process experimental data, an etch tool was charging the emitter (Figures 11-12). The etch time was intentionally increased and OO failure was correlated with the increase in the etch time. With a low level of plasma charging on the emitter, the electrical characteristics of the junction can altered without creating an obvious physical damage.


Figure 11: These images are taken from the grossly over etch time to decorate out failure. Charging on the emitter was correlated to the Output Offset failure at the wafer level. Tool A on the left caused aggressive damage to the corner of the emitter.


Figure 12: Tool correlation OO failures, that was due to charging on P-N junction.


Failure analysis on analog circuits often leads to the nodal analyses and internal probing of the circuit in question. Layout and schematic databases were essential in the analysis efforts.


A soft P-N junction break down, especially in the matched BJT pairs of an analog circuitry, presented only a small DC voltage change, and isolation of the failure required the understanding of the operation of the circuitry. The break down degraded the performance of the differential op-amp.


With a soft P-N junction failure, the Gummel plot showed a better profile of current leakage level compared to I/V curve trace. Isolation of the weak leakage was performed using a combination of I/V curve traces and FIB cuts. The real physical defect was not observable. However, with the helps of fab data, the failure can be explained as plasma charging.


Etch tool A


Before Flash Etch at Edge


122Å Etch


180Å Etch


250Å Etch


Etch tool B


[1] Paynter, Introductory Electronic Devices and Circuits,Prentice Hall (New Jersey, 2003), pp. 609.


[2] Schroder, Semiconductor Material and Device Characterization, Wiley & Son (New York, 1998), pp.


214-16.


[3] Hambley, Electronics, Prentice Hall (New Jersey, 2000),pp. 411-482.


Tool-Related ESD Surface Damage (ESDFOS) on Wafers in Cu-Technology


Peter Jacob


Empa Swiss Federal Laboratories for Materials testing and Research, 8600 Duebendorf, Switzerland  Peter.Jacob@empa.ch, phone +41-44-823-4288; Fax -4054


Cheryl Hartfield*


Texas Instruments, Dallas, TX 75235, U.S.A.


In many cases it is difficult to distinguish mechanical damage  from electrostatic surface impacts.  In recent years, several  investigations have resulted in publications on ESDFOS (Electrostatic Discharge From Outside to Surface). While the  diagnostics of the phenomena have been worked out quite  well for wafers with aluminum metallization, no formal  studies on ESDFOS impact to copper-metallized wafers have  been published. This paper investigates physical features of  Cu-metallized wafers artificially exposed to ESDFOS impacts  of variable severity, producing an understanding of damage  features to more easily facilitate recognition of EDSFOS  events.


In the last 3-4 years, the phenomenon known as ESDFOS (ESD From Outside to the device Surface) has been  intensively researched on semiconductor wafers fabricated  with aluminum interconnects.   ESDFOS is often  misdiagnosed and the root cause of the ESDFOS physical  signature, damaged passivation, attributed to “mechanical  damage”.   However, many of the ESDFOS-damaged  passivation areas are barely visible, even by SEM, with  dimensions on the passivation surface of a few microns.  Real  mechanical causes like robotic mishandling, probe needles, tweezers, etc. can all be excluded as contributors, since their  damage signature is much greater.  In previous work, a series  of artificially induced ESDFOS (using a Wimshurst machine) proved that small area “mechanical impact” damage was in  fact caused by electrostatic discharge into the passivation, generating interlevel shorts within the two top metal layers [1, 2].  This enabled identification of process causes of ESDFOS  and development of methods to reduce it [3, 4].


ESDFOS signatures on devices with Cu metallization have not  been investigated.  ESDFOS impacts will likely not be  identified when they occur on Cu devices, if the damage  signature does not match that of Al devices.  Since  manufacturing steps contributing to ESDFOS on Al devices


are also common for Cu technology, an investigation of the  ESDFOS sensitivity of Cu-technology devices was required. 1


ESDFOS in Cu Technology


The experimental set-up duplicated the previous set-up used  for the Al-technology devices [2]:  a Wimshurst machine with  its Leyden jars (capacitors) switched off and the maximum  voltage limited by spark gaps to 1-3kV was used.  A 30mm  diameter Al ball was used as a spark electrode in one test  series.  In the second series, an inversed needle with a ball  diameter of 2mm was used.


After selecting several fields on the wafer, ESDFOS impacts  were imparted to each area and evaluated.  The ESDFOS  damage was divided into 3 classes: weak, medium, and strong  impact.  Through variations using additional new electrodes  like flat plates and needle peaks, one single spark was able to  create a wide variety of impacts by splitting up (like a  thunderstorm strike) into different impacts of very different  severity.


The physical damage profile that ESDFOS imparts to Cu  devices is significantly different than that documented for Al  devices.  Comparing ESDFOS-caused defects to those on Altechnology, it is noteworthy that the characteristic damage  features of peaks and spikes found with Al metallization are  uncommon for devices with Cu metallization.  Four reasons  explain this difference.   First, the degree of CTE mismatch is  less for Cu and SiO2 than for Al and SiO2. Second, the  melting point is significantly higher for Cu than Al.  Third, the  thermal capacitance of Cu is higher than Al. Fourth, the  thermal conductivity of Cu is 2x that of Al. This causes the  energy introduced into a Cu metal line by an external spark to  distribute differently than it would in an Al metal line.  In Al  metal lines, the metal first becomes molten, leading to  secondary cracks which open leakage paths to the metal  underneath.  The Al penetrates immediately into such cracks, causing shorts.  This effect is supported by the smaller thermal  capacitance, which causes the energy to be quickly released


* Cheryl Hartfield is currently employed by Omniprobe, Inc. in Dallas, TX. Her new contact information is  hartfield@omniprobe.com, 214 572-6804.


SiO2  Al


specific heat cp [J/g/K] 0.702 0.75   0.897 0.385  melting point  Tm  [°C] 1410 1665 660.32 1084.4  heat of fusion Hm  [J/g] 1799.9 237


399.9 205.4


Energy required to melt  1 µm3 [nJ]


6.46 3.32 2.62 5.47


Table1. Amount of Energy required to melt 1 µm3 of


material, estimated based on thermal material data


and causes destruction.  In Cu technology, the higher thermal  capacitance and thermal conductivity “buffers” the energy.  The physical scenario in Al devices appears as follows: The  spark hits and cracks the passivation surface, and then the  spark charges the metal until (within some milliseconds) local  melting of the aluminum metal appears. Driven by  thermomechanical extension, the molten aluminum is pressed  into the cracks and forms needle-like-structures and shorts.  However, in the case of copper, the thermal and  thermomechanical conditions are different.  Since both the  melting temperature and the thermal energy needed for  melting copper are closer to silicon than aluminum, usually no  copper melting takes place. However, local thermomechanical  expansion still appears due to the thermomechanical mismatch  between Cu and SiO2, thus generating cracks in SiO2  interlevel dielectrics and passivation. Besides the spark impact  crack, these cracks often propagate in a horizontal direction, tearing off the structures within proximity of these cracks.  Electrically, both opens and shorts are created by this manner. The thickness and type of passivation also has an influence on  the severity and sensitivity to ESDFOS damage. The  passivation of the Cu wafers in this study is about 1.5x thicker  than the Al wafers previously studied, and the passivation  surface is planarized. This Cu-technology passivation  withstands a voltage of more than 1000V, compared to usually  500-700 V for classical oxynitride passivations. Since failures  on these Cu devices typically occur at higher voltages than on  Al devices, greater energy is involved in the failure, resulting  in more severe destruction (material disturbance) than usually  observed for Al devices.


In the investigated 5-level metal Cu technology, usually the  top 3 to 4 metal layers were structurally damaged due to  exposure to large ESDFOS impacts.  The damage consisted  mostly of vertical and horizontal cracks.  However, also some  very small ESDFOS impacts were found.  These show the  same texture as the larger ones, but the damage is very  limited, appearing on the passivation surface as only a very  minute crack (on the order of ~1um).  These cracks cause  local delamination and interlevel shorts, too, but not as  frequently as in Al-technology.  Figures 1-16 in the appendix  show a catalogue of typical surface and cross section views of  Cu-technology wafers exposed to ESDFOS of different  degrees of severity.  In some cases, surface electrostatic  effects were similar to ESDFOS effects observed on power  semiconductors with very thick metallization.  If the discharge  took place as a “splutter”- (a space-like discharge as a line  spark, which can be seen as “lightning” only in the presence  of extreme darkness) or “corona”-type, surface passivation is  molten and collected to a ball at the impact center. Also  particles can act as an elevated lightning discharger and be  glued to the passivation surface by the melting of material at  the moment of the impact.


Figure 11 shows the visible degradation of the separator and  the impact of a dissolved iron contaminant in an exemplar  cell, which had a lower than normal open circuit voltage. The  SEM image and elemental x-ray map in Figure 12 shows that  the contaminant is iron.


In another case, an iron particle was found lodged between the  separator and the bare copper electrode of an exemplar cell, as  shown in Figure 13 and Figure 14. While this small iron  particle had caused this cell to fail, it did not cause a thermal  runaway, hence the damage was minimal and the particle  could be found.


Figure 11. Dissolved contaminant found in an exemplar cell.


Figure 12. SEM image and Fe map of dissolved iron  contaminant on copper foil in Figure 11.


Figure 13. Particle (circled) found between separator and  outer copper winding.


Figure 14. SEM image of particle confirmed to be iron.


Electrolyte Leakage – Domino Sequence


In this case study a series of overheated notebook batteries  were received for a root cause failure analysis. Numerous cells  in each battery pack were observed to have overheated. External causes were eliminated. It was in the “NonDestructive Analysis” step that an x-ray revealed that there  had been significant melting of the circuit board copper traces. It was also observed that the cell that was adjacent to the trace  faulting region failed by overheating and venting. The plastic  battery enclosure showed clear evidence of long term  electrolyte leakage, as did at least one of the cell caps as  shown in Figure 15.


Base image


Fluorine map


Anode current collector


The only sequence of events to explain the learned key  information was that electrolyte leakage initiated faulting  between circuit board traces, which heated the adjacent cell, which experienced a thermal runaway and vented, thus  heating other cells in the pack which caused them to also  overheat and vent as well. No other sequence of events  explained all of the learned key information.


Figure 15. Salt build-up in the positive cap area.


Mechanical Crush – Does Your Dog Bite?


Significant mechanical deformation will occur to a metal cell  housing during an overheating/venting cell incident. The  ballooning of the cell’s metal housing is likely to mask or  eliminate evidence of mechanical deformation that occurred  prior to (or at the time of) the incident.


A divot was found to be hidden underneath a flat surface of  burnt plastic housing residue on the surface of a vented cell  metal housing during the initial inspection of the “Cell  Analysis” step as shown in Figure 16. This observation  indicates that this divot was filled up with melted material  during the incident. In other words, the divot preceded the  incident. A corresponding protrusion inside the metal housing  was observed on the inside surface as shown in Figure 17. Finally, the divots were found to line up with evidence of  electrical faulting on the surviving copper electrode. Such  divots have been found to be caused by canine teeth. Interestingly, the mechanical damage to this cell did not  immediately cause it to fail since the product cover was on at  the time of the incident and exhibited no corresponding  evidence of mechanical deformation.


Figure 16. A divot found beneath the flat burnt residue.


Figure 17. A corresponding protrusion found inside the can.


Overcharge – Liquid Intrusion


Liquid intrusion, especially from a source that contains a high  concentration of ions, is expected to create parasitic electrical  paths. Such paths can cause loss of charge regulation and in  addition, loss of the redundant overcharge protection circuit. There are well-meaning websites that provide instructions on  what to do if your phone gets dropped into a liquid. Electronic  equipment is not designed to operate correctly when subjected  to moisture intrusion and there is no easy way to determine  whether a cell protection circuit has been compromised from  such an exposure.


In this next case study the charge regulator and protection  circuits had both been severely damaged by moisture intrusion  as found in the “Circuit Evaluation” step. The surviving  evidence was preferential galvanic corrosion found on nodes  that had voltage present during normal operation, indicating  that it occurred while the device was still powered. Loss of  functionality of the charge regulator in addition to the  redundant protection circuit would have overcharged the cell, and overcharge was therefore determined to be the most likely  cause of the incident. Further cell analysis could have been  performed and may have provided information to confirm or  refute the overcharge root cause hypothesis.


External Heat


A Li-ion incident usually involves overheating of materials  close to the cell in the product. In multi-cell batteries, a failure  of one cell often results in heating of the adjacent cells and  secondary failures. It can often be difficult to conclusively  establish which cell was the initiating cell. It is common to see  pieces of melted plastic and charred plastic residue adhered to  the cell housing. Evidence of heat damage that preceded or  caused the incident can therefore easily be masked or  eliminated by the ensuing overheating incident. Recreation  testing has shown that there can be distinguishing  characteristics in the remains of a cell that has failed due to  the application of external heat, though testing is usually  required to identify the expected response for each type of  cell. For example, an externally heated cell can was found to  rupture solely due to the vapor pressure from the boiling  electrolyte and eject its contents, leaving a relatively  undamaged and clean metal housing. A similar response has  been observed in recreation testing whereby cells are  mechanically crushed, resulting in a massive internal cell fault  that creates a very rapid increase in cell pressure. The  expected response for any given cell is crucial to be able to  correctly interpret the observed evidence.


Microwaves have generally been found to leave clear and  surviving witness marks after an overheating incident. Other  known sources of heat that have caused field incidents include  hot plates, ovens, heating elements, lighters, torches, hot  engines, etc.


1. Undesired field failures of Li-ion products are an  unavoidable reality given their proliferation throughout  the world and the present state of cell technology, though  the actual failure rates are still extremely low.


2. The possible causes of undesired overheating Li-ion  incidents include:


a. Internal cell short circuit that results from many  possible latent cell defects,


b. Mechanically-induced cell internal short circuit,


c. Cell external short circuit,


d. Cell overcharge,


e. Cell overdischarge,


f. External heating of a cell, and


g. Cell charging at high/low temperature.


3. Issues that product manufacturers can address to reduce  the probability of having field failures are limited to the  mechanical integrity of their product that houses the Liion cell, and the robustness of the circuitry that prevents  overcharge and overdischarge. Since only the cell  manufacturer can control whether or not cells contain  latent defects, product manufacturers should select  suppliers who are able to credibly demonstrate their  ability to deliver cells with an acceptable failure rate.


4. The decision of whether a recall is indicated is an  involved process that requires:


a. Identification of the susceptible population,


b. Determination of the expected and potential severity  for the type of failure that is seen,


c. Creation of a hazard function to be used to predict  the probability that in-service cells will fail as a  function of time,


d. Comparison of the risk posed by the remaining inservice population with the risk posed by a  replacement population,


e. An assessment of the risk in light of the expected  severity, and


f. Working in concert with the appropriate  governmental agency whose duty it is to protect  consumers.


5. A scientific methodology for investigating Li-ion  incidents has been presented to determine, when possible, the root cause of an incident and the relative certainty of  that conclusion. Steps presented include:


a. Background: obtain background information (if  possible).


b. Exemplar Characterization: Document operation of  an exemplar unit to establish expected charge and  discharge and protection circuits’ operation.


c. System Observations: Photographically document  and record observations about the incident remains. d. Non-Destructive Analysis: Perform x-ray imaging of  cells, relevant electronic circuitry and other remains. e. Circuit Evaluation: Perform testing to assess the  operation of the AC adapter and charge regulator.


f. Battery Analysis: Open the battery and inspect and  document all of its components, heat patterns, evidence of venting, and damage and include testing  of the backup protection circuitry where possible.


g. Cell Analysis: Evaluate cell(s) using non-destructive  and destructive techniques and gather all available  information contained in its remains.


h. Recreation Testing: Perform testing to recreate the  observed evidence.


i. Exemplar Analysis: Evaluate exemplar units to  evaluate whether a systematic defect exists that is


expected to lead to additional incidents with other inservice units.


j. Possible Additional Considerations: Additional  issues that may be explored include a factory audit or  other specialized engineering investigation.


k. Draw Conclusions: Create a list of key information, and draw conclusions that account for all the known  information. State assumptions and relative certainty  of the stated conclusions.


6. Experience has shown that some fraction of Li-ion  incidents are found to be caused by accidental or  intentional abuse. It is therefore possible that some  fraction of the root cause conclusions are incorrectly  assigned to the broad category of manufacturing defects  because the evidence of abuse was in those cases  completely obliterated in the ensuing incident.


Dr. Rose Ray and Madhu Iyer of Exponent: Statistical  Analysis


Stig Nilsson, Dr. Quinn Horn, Daren Slee, Jan Swart and Dr. Jason Fu of Exponent: Peer review.


Exponent’s many clients who have retained us to perform  these interesting investigations.


[1] ASTM 860-97, Standard Practice for Examining And  Preparing Items That Are Or May Become Involved In  Criminal or Civil Litigation, 2006.


[2] IEEE Std 1725, IEEE Standard for Rechargeable  Batteries for Cellular Telephones. 2006.


[3] UL 1642, Lithium Batteries, 3rd edition April 26, 1995, revised June 24, 1999.


[4] IEC 62133, Secondary cells and batteries containing  alkaline or other non-acid electrolytes - Safety  requirements for portable sealed secondary cells, and for  batteries made from them, for use in portable  applications, 1st edition 2002.


[5] EN/IEC 61960, Safety Requirements for Lithium  Secondary Cells and Batteries, December 1, 2003.


[6] UN Manual of Tests and Criteria, 4th revised edition,


2000.


[7] Slee, Daren, “Printed Circuit Board Propagating Faults,” Proceedings, 30th International Symposium for Testing  and Failure Analysis,  November 2004.


[8] Loud, John et al, “On the Testing Methods of Simulating  a Cell Internal Short Circuit for Lithium Ion Batteries,” Long Beach Battery Conference, 2001.


[9] Swart, Jan et al, “Methods for Measuring the Mechanical  Safety Vent Pressure of Lithium ion Battery Cells,” IEEE  POSES Conference, 2006.


[10] Swart, Jan et al, “Lithium Ion Batteries for Hybrid  Electric Vehicles: A Safety Perspective,” AABC  Conference, 2005.


Case Study and Fault Modeling for


Wrong Redundancy Evaluation on DRAM Devices


Martin Versen


Qimonda AG, Am Campeon 1-12, D-85579 Neubiberg, Germany


Dorina Diaconescu, Jerome Touzel


Infineon AG, Otto-Hahn-Ring 6, D-81739 München, Germany


The characterization of failure modes of DRAM is often  straight forward if array related hard failures with specific  addresses for localization are concerned.


The paper presents a case study of a bitline oriented failure  mode connected to a redundancy evaluation in the DRAM  periphery. The failure mode analysis and fault modeling focus  both on the root-cause and on the test aspects of the problem.


Fail Description and Electrical Characterization


Test fallouts with a bitline oriented fail signature with a  redundancy signature (see bitmap in Fig. 1) are known over  several product generations. The redundancy signature consists  of two failing bitlines separated by 4 segments because of the  repair scheme.


Figure 1: Bitmap of bitline oriented failures with redundancy  signature.


The test pattern is a simple write/read pattern with voltage  trimmings. The test sequence consists of the following parts:


• Initialization


• voltage trimmed down – ΔV1


• Write “0” to the cell array


• voltage trimmed up + ΔV2


• Write “1” to the cell array


•  Read “1” from the cell array


A wrong bitline (BL) or spare bitline (SBL) is accessed during  the “Write 1” with the voltage trimmed up. For an analyzed  sample the fail sequence is valid for the row addresses in the  range from x=1800 to x=19ff and the column address y=103.  There are two possible scenarios, either a missed or a wrong  redundancy hit. In case of a missed redundancy hit, a timing  adjustment by shooting of a laser fuse that delays the  redundancy evaluation leads to a relaxation of the fuse and  subsequent address evaluation of the redundancy. The sample  has been opened partially and this fusing has been conducted  by Focus Ion Beam (FIB), but this does not change the fail  behaviour. Therefore the missed redundancy hit is excluded  and a wrong redundancy hit is assumed. As the component has  been opened already, the redundancy fuses were  photographed.


Although there is a kind of used electrical redundancy because  of the fail signature, no fuse is blown for this address in the  optical readout (see Fig. 2). A summary and a good match is  found in Table 1 if the optical readout is compared to fuse data  except that the column address y=103 is missing. Also, no  unintentional damage has been observed at any other fuse in  SEM images (not shown). The conclusion is that there is a  wrong redundancy hit because the failing address was neither  intentionally fused nor are the fuses damaged. The original  fusing has been successful and the problem must be elsewhere.  In order to generate a wrong redundancy hit on an unused  spare bitline without fusing, an enable fuse signal is required  that is decoded from the fused column address bits CA7 and  CA8 for this DRAM design. So for an unused spare bitline, a  defect in the address paths of either CA7 or CA8 may explain  a wrong hit.


Figure 2: Microscope images are made and stitched together for the optical read out for the fuses in the segment. The arrow marks  one dark (blown) fuse as an example.


Table 1: Fuse data and optically read out addresses show


identical results.


Fuse  data


optical


377


2FF


2DD


0B3


003


Column  addresses


059


Table 2 shows the available spare bitlines (SBL) for a wrong  hit that could replace the column address y=103. The SBL48  and SBL60 have the highest likelihood because one defect on  either CA7 or CA8 would be sufficient. Therefore, they  receive the highest priority. The SBL56 would require a defect  that affects both CA7 and CA8 which is somewhat more  unlikely and which is therefore priority 2. The SBL52 would  require some defect within the evaluation logic in a way that  one segment is affected but not the others although the  evaluation logic is shared between the segments. This is  inconclusive, so this possibility is rated as very unlikely and  gets therefore priority 3.


Table 2: Possible locations of spare bitlines (SBL) sorted  according to their likelihood to induce a failure.


No


SBL


priority


48


~ – 49 ~ 3000


~ – 49 ~ 3625


56


~ – 49 ~ 3420


~ – 49 ~ 3207


The component is opened and delayered down to the lowest  metal level and a passive voltage contrast (PVC) inspection in  a SEM is performed by checking the symmetry of dark and  bright metal line for the SBL locations. The PVC is widely  used in failure analysis in identifying leaky gate-contacts or  open contacts [2]. For 1kV accelerating voltage of the primary  electron beam, the gate contacts appear dark and the grounded  contacts bright. In higher metal layer, the method is less  effective as a metal line can connect a gate to a ground contact  and therefore the SEM-contrast of the metal line is similar to  that of the grounded contact. For SBL48 and SBL60 locations  no broken symmetry is observed. Fig. 3 shows the  corresponding SEM image for the voltage contrast on the  lowest metal layer for the SBL56 location which has been  priority 2. There are two bright lines in the middle of the  image marked with two bold arrows while the other symmetric  line above and below remain dark (marked with dotted  arrows). So this is a broken symmetry and the location of the  defect; SBL56 shows two contacts that are connected to the  well or diffusion region, they are therefore grounded, but they  should float. These signals correspond to the blown fuse  address <7> and <8>. These signals create the observed fuse  hit – the spare Bitline SBL56 with the fuse on addresses <7> and <8> blown would replace the column address y=103.


The broad location of the failure is thereby detected and it  supports the hypothesis of a wrong redundancy hit. Yet only  the exact location on transistor level can explain how the  failure may act and react electrically in a test. Therefore the  metal layer is carefully removed to the contact level. Again  SEM passive voltage contrast is performed on the defect  location; the corresponding SEM image is shown in Fig. 4.


Figure 3: SEM image with 0.7keV for voltage contrast on the lowest metal level.


The voltage contrast on contact level reveals that four gate  contacts are brighter than the other contacts in the dark row  indicated by the arrows in Fig. 4. These four contacts belong  to the gates of transistors for the blown fuses <7> and <8>. There are four signal lines because the fuse signal is


differential. The names of these lines are BF<7>, bBF<7>, BF<8> and bBF<8> and the “b” indicates the inverted signal (“b”=”bar”) of a differential pair of signals.


Figure 4: Voltage contrast on contact level. The voltage contrast on gate contact level shows that four contacts are brighter than the  others belonging BF7, bBF7, bBF8 and BF8.


4 contacts


belonging to  addresses


<7> and <8>


Failure mode and fault modeling


Analog simulations are performed in order to understand the  failure mode. Fig. 5 depicts a block diagram of the redundancy  circuit. There is an address bus connecting the fuse latches  with the address decoder. In a simple fault model [1], a short  fault is applied connecting the fuse address lines BF<7> and  bBF<7> which should carry a differential signal. This  differential high/low signals are connected to transistor gates  and should switch these in order to apply a fused address in the  decoder.


Figure 5: Block diagram and simplified fault model.


As the short occurs between differential signal lines, the  driving strengths of the transistors driving these lines  determine the resulting common potential. As the transistors  have roughly the same strength, the resulting level is the midlevel between the applied high voltage V and ground.


The timing diagram of an analog simulation is shown in Fig. 6. The discussed mid level is obtained around ½ V for RFAULT values of 1kΩ, 5 kΩ and 10 kΩ as the output resistance of the  transistors is larger than these values. Thus, the voltage falls  above the fault resistor.


The stimulus for the simulation is the changed supply voltage  in order to understand the changing failure mode for the test  pattern. The supply voltage for this circuit is a piecewise linear  with a voltage level of V – ΔV1 before t1, ramping linearly to V between t1 and t2, remaining at V until t3, ramping form V to V


f. EDS (Energy-dispersive X-ray spectroscopy) to  identify the elemental composition of foreign  material in cell remains.


g. XRD (X-ray diffraction) to provide useful  information about the chemical composition of a  region of remaining active material to determine  whether it was overcharged prior to the overheating  incident. The diffraction data of the cathode material  from a powder X-ray diffraction is used to identify  the changes of crystallographic structure, chemical  composition and physical properties that can only  have occurred due to an overcharge event. Challenges involved with this technique include  distinguishing between chemical changes that occur  due to heating from those that occur prior to or  during the incident. Interpreting the results obtained  from this technique is difficult given the wide  variability in the conditions that the cell materials  will be exposed to during and after the incident and  the requirement for precise knowledge about a cell’s  chemical composition. While there is great need for a  method that can reliably indicate whether an  overheated cell was overcharged prior to an incident, use of XRD for this purpose is still in its infancy and  has not yet received wide acceptance.


Figure 4. Melted copper electrode with thickened edge.


Recreation Testing


The purpose of recreation testing is to verify the root cause  hypothesis and the sequence of events that are believed to  have caused the incident being investigated. It can also  provide insight into the susceptibility of the remaining inservice population and the potential severity of an incident.


Exemplar Analysis


The evaluation of undamaged exemplar cells or products with  similar date codes has often proven very valuable in  identifying latent defects that are believed to have caused the  incident being investigated. Exemplar cell or product date  codes are very important in trying to identify a susceptible  field population when a systematic defect is identified.


Additional Considerations


Depending on the scope of work beyond root cause analysis  and what is found during an investigation, a cell or product  factory audit may provide valuable insight. If cell anomalies  are identified in an exemplar analysis, a factory visit may be  the only way to bound the population of cells that would be  expected to contain the identified anomaly. It would also  provide the opportunity to assess whether appropriate  manufacturing controls are in place to prevent future problems  of a similar or different nature. A detailed examination of  manufacturing quality documents, such as control charts, has  also been proven to provide valuable data for identifying and  bounding defective cell populations.


Other possible items to consider include an in-depth  engineering analysis of any identified unresolved problems  that arose during the investigation.


Draw Conclusions


The first step in drawing conclusions is to create a list of key  facts, observations, and test results that have been learned  from the investigation. All hypotheses that account for all or  most of what was learned must be considered. Generally, only  a single root cause hypothesis explains all that is known about  an incident. Sometimes, however, there are “holes” in the  information. The investigator should then state assumptions  that are made to reach conclusions. The investigator should  also characterize the relative certainty of the “most likely root  cause” of an incident based on the quality of the information  obtained during the investigation. The investigator should also  list other possible root causes, even if they are viewed to be  less likely, if the investigation process has not credibly  eliminated other branches of the fault tree. It may also be  appropriate to state which branches have been eliminated and  the bases for such elimination.


Statistical Analysis


Without exception, all commercially available Li-ion cells are  susceptible to undesirable failures (though a few  manufacturers claim to have new cathode materials that  prevent flaming failures and cell combustion). While failure  rates have in general been kept very low, the proliferation of  this technology dictates that there will necessarily be some  level of background failure rate associated with its use. On  occasion, however, something goes wrong and certain  populations will exhibit a higher than normal rate of failure. The first step is to determine whether the field incident(s) being investigated indicate a failure rate that exceeds the  expected failure rate.


If an elevated and unacceptably high failure rate is identified, consideration of a recall must evaluate issues far beyond a  simple arithmetic failure rate calculation. Assuming that the “normal” risk of failure of the product is acceptable, the goal  when considering whether to recall an in-service product is to  determine whether replacement of the existing field  population will result in a significantly reduced risk of injury  or loss. While the issues to be evaluated to make such a recall  determination certainly exceed the scope of this paper, they  include:


1. Identify the susceptible field population. The susceptible  population may be only a small fraction of the total inservice population of a given cell or product. The root  cause failure analysis may be critical in defining what  portion of the field population is susceptible to the  observed failure mode(s). Changes in production, raw  materials, operators, machine servicing, etc. may provide  credible scientific support to segment a field population  into groups with different expected failure rates. Tracking  failures by manufacturing date code may also provide  insight to identify a susceptible population. A lack of  failures within an observed date range is not necessarily  improbable when dealing with low frequency events and  can therefore only rarely be used to defend segmenting a  population.


2. Bound the expected and potential severity for the type of  failure that is seen. Multi-cell batteries typically have a  greater potential for a severe outcome than do single-cell  products. Variations in cell cathode materials, cell  electrolytes, or product construction will also affect  potential severity.


3. When possible, create a hazard function that can then be  used to predict the probability that in-service cells will  fail as a function of time. Such a predictive model must  be supported by the physics of the failure processes that  have been identified in the root cause analysis, as well as  the known failure data. Of critical importance to such a  predictive model is information concerning the expected  remaining service life for the product.


4. Evaluate the risk posed by the remaining in-service  population to compare it to the risk posed by a  replacement population. For example, it may be that the  risk posed by the remaining field population does not  significantly exceed the expected risk for a replacement


population by the time that an elevated failure rate is  identified for an infant mortality type hazard function.


5. The risk must then be assessed in light of the expected  severity for future incidents to make a final determination  concerning whether recall is indicated.


In the USA, such analysis concerning whether to recall is  conducted in concert with U.S. Consumer Product Safety  Commission under its guidelines and regulations.


The following are “snapshots” from actual Li-ion  investigations and were selected from the hundreds of  investigations that have been performed by the authors at  Exponent as far back as 1995.


AC Adapter or Charger Problems


Two case studies are provided to illustrate findings in the “Circuit Evaluation” step. In the first, the same charging plug  was used on different Li-ion products that had different  overcharge protection designs. Even though the plug fit  perfectly, use of the wrong charger resulted in a loss of  overcharge protection leading to overcharge of the pouch type  Li-ion cell, causing overheating and charring of surrounding  materials.


In the second, a switch-mode rapid charge AC adapter was  found to have an optocoupler that degraded over time that  resulted in a loss of regulation and an increase in the output  voltage. An increase in the output voltage caused the output  filter capacitor to fail and dry out. Loss of output capacitance  resulted in a high frequency, high voltage square wave being  supplied to the charge regulator. The regulator passed this  unexpected signal directly through, thus relying solely on the  redundant overcharge protection circuit to interrupt this very  unusual charging waveform. Some did not, resulting in  overcharge failures.


Internal Cell Fault – Manufacturing Problems


The manufacturing line of Li-ion cells is an extremely  complex process. From the incoming material quality check, to regular checkup of the tooling, to quality check of the final  product, great care needs to be paid to each process. Any  deviation from the control standard may result in batches of  cells with inherent manufacturing defects. Contaminants in the  raw materials used to make the electrode active materials may  later cause dendrite growth and an internal short circuit. A  dull cutting tool for the electrodes or tabs may result in  uneven cutting or edge burrs that over time can cause an  internal short circuit.


The cause of this next case study was found in the “NonDestructive Analysis” step when the x-ray image of an  incident cell was found to have a folded electrode tab in the  region of cell faulting as shown in Figure 5. The “Exemplar  Analysis” step revealed the same latent defect in a cell from a  similar date code.


Figure 5. Incident cell with folded electrode (left) and  exemplar cell with the same latent defect (right).


The cause of the following case study was established in the “Cell Analysis” step when an electrode connecting tab was  found to have penetrated through the insulation protection  tape, which made an intermittent short circuit with the positive  cell can, as shown in Figure 6 and Figure 7. This fault resulted  in copper migration and dendrite formation due to repetitive  overdischarge, as shown in Figure 8. This cell eventually  failed due to minor overheating caused by an internal short  circuit.


Figure 6. Excessive length electrode tab penetrated the  insulation tape and contacted the cell housing.


Figure 7. Blackened tip of the electrode tab from shorting to  the cell housing.


Figure 8. Copper dendrite formation observed on the  separator due to repetitive overdischarge.


The cause of a swollen pouch cell was found by doing a crosssection in the “Cell Analysis” step. A significant difference in  thickness on the two sides of the anode coating was found as  shown in Figure 9, which can indicate an anode/cathode  lithium capacity imbalance. The presence of fluorine, shown


in Figure 10, is consistent with lithium metal plating due to  the observed potential capacity imbalance. The plating of  lithium resulted in the chemical reduction of the electrolyte  and the generation of gases that caused the pouch cell to swell.


55 μm 92 μm


Figure 9. Uneven thickness of anode coating.


Figure 10. EDS analysis of anode coating.


Internal Cell Fault – Contamination


Iron contaminants have been a major concern for Li-ion cell  manufacturers over the years and have been cited as the  reason for major cell recalls. Iron contaminants can either  penetrate the separator or facilitate dendrite growth, resulting  in an electrode-electrode short circuit. While these effects of  iron contamination are well known, it is very difficult to  eliminate them from the raw materials that are used to make a  cell as well as from accidental introduction from production  line manufacturing equipment.


It is very difficult for an investigator to conclusively show that  iron contamination was the root cause of an incident due to  the severe damage that typically occurs. It is therefore  typically evidence found during the “Exemplar Analysis” step  that has provided proof of a systematic iron contamination  problem.


Energy considerations in Cu technology


Based on the assumptions made in [2], the energy balance can  be estimated.  First, the amount of spark energy introduced  into the device versus the amount dissipated for lightning


must be considered, along with acoustic emission, thermal and  ionization effects in the air spark channel.


A useful estimation approach for this is to compare the  damage to so-called FIB-popping damage, which is a special  case of ESDFOS.  In this case, a capacitor can be assumed, formed by the slightly conductive (due to ion beam  implantation) top area of the ion-beam-scanned passivation.  This area is defined by the field-of-view and, of course, the  ion bombardment duration, etc.  As a reasonable order of  magnitude estimation from daily FIB-working experience, an  area of about 100x100µm2 FIB field-of-view is assumed.  At a  usual passivation thickness of 1µm, the capacitance versus the  conductive parts of the IC results in:


C= ½ εo εr A/d ,


where C is capacitance, A is the cap area, d is the passivation  thickness, εr is the relative dielectric constant (about 5 for such  a passivation), εo is the permittivity of free space (8.854e-12  F/m), and the factor ½ accounts for an average metal coverage  of 50% underneath of the passivation.


Using these values, 0.2pF results.  Since the critical dielectric  breakdown voltage to 1kV was evaluated, the energy  introduced into the device surface is calculated to about


0.11µJ.   This amount of energy allows melting 20µm3 of Cu  or 33µm3 of SiO2 (Table 1), which seems to be the right order  of magnitude.  However, FIB-induced damage is usually  significantly less severe than that generated by the Wimshurst  machine.   We would roughly propose a factor 100 – 1000x in  energy needed to generate a similar grade of destruction by  FIB.   Considering the destruction severity bandwidth of the  Wimshurst machine experiment, we estimate the introduced  energy to about 1-10µJ.  This would mean that, depending on  the grade of destruction, only between 1/10 and 1/100 of the  total spark energy of about 300µJ is really introduced into the  device.  Higher amounts of energy are introduced in cases of  thick passivation (such as these Cu-technology wafer  samples), since more voltage is needed to crack the  passivation.  This explains the higher degree of destruction  observed in this study compared to wafers in Al-technology  with standard oxynitride passivation thickness.


Considering the physical effects which take place, a direct  spark damages the passivation surface first and causes cracks. However, any attempt to decrease ESDFOS sensitivity by  increasing the passivation thickness would be fatal; this would


0 20 40 60 80 100


GND problems


Ionizer related


Material selection


Media setup


slight faults


severe faults


caused


process stop


just let the spark introduce into non-passivated pads, generating more or less “classical” ESD damage via pads.  Thus, if there are any indications of ESDFOS, the corrective  action approach should be towards the process root causes.


Process Root Causes for ESDFOS


Significant static charge is especially generated by 1) the front  side detaping process after backgrinding wafers, 2) pick and  place processing (detaping wafers from the backside) and 3) washing/ rinsing processes.  Audits conducted by EMPA  across many different companies revealed that in general, ESD precautions are carefully made considering people, workplaces and floors.  However, much less attention is paid  to the process robotics: air ionizers which are switched off and  ionizer fans in operation without any ionizing effect (dirty  needles) were found in nearly every tool-ESD-audit, along  with tools where charging occurs and ionizers are totally  missing.


A hit list of process causes (verified in Al-technology in [4]) is summarized in Fig.  17.


Considering the tools, die pick and place processing most  frequently shows problems. These problems are related to the  fact that either charged devices (by loading the frame with the  dies on electrostatic active blue foil) are picked by the (grounded) picker head, or, the picker head itself has been  charged by robotic moves, e.g. in teflon bearings. It is  therefore of utmost importance to smoothen electrostatic  potential adaptations by useful installations of ionizers. Furthermore, all processes where the wafer/ dies are mounted


on blue foil are known to be critical.  Every lift-off from a  metal chuck generates surface charge on the wafer of  sometimes more than 3kV, which may discharge when sorting  back into wafer carriers unless protected by ionized air  streams. Recently, further knowledge has been collected  considering wafer dicing.  In this step, several physical effects  superimpose, generating both ESDFOS and ESDFOS-similar  damage.  The superimposed effects include charge generation  by water drop separation near the dicing wheel.  These effects  are similar to a “dirty” ultrasonic cleaning, both generating  mechanical forces and electrostatic charging.  At present, these effects are under investigation at EMPA and will be part  of a separate paper in the near future.


Since strong friction electricity allows sparking even from  isolated highly triboelectrical surfaces, the front side de-taping  process following wafer backgrinding turned out to be  extremely critical, too.  Surface charge measurements have  indicated surface voltages of 25kV and more. It could be  proven both by related failure analysis results as well as by  use of a touchless spark counter that in fact, severe ESDFOS  can be generated by de-taping, especially at high speed and  without ionizer protection.  It is unbelievable to the authors  that on one hand, all manufacturing facilities are subject to  strongly regulated ESD protection measures like antistatic  floors, shoes, clothes etc… while at the same time it is widely  accepted that such blue foil is used for direct wafer surface  contact.  Attempts to replace the blue foils by a better  antistatic material remain unsuccessful – all replacement foils  have shown severe problems with mechanical properties like  elasticity, robustness, adhesion, etc.


In total, it is expected that industry reports of ESDFOS for Cu  technology will be less than presented for Al technology.  This is due to the combined influences of apparently lower  frequency of ESDFOS occurrence and greater likelihood of  root cause misdiagnosis due to the greater average degree of  destruction observed when ESDFOS does occur.


Conclusions:


Guidelines and hints for proper diagnosis and failure analysis  interpretation in the case of ESDFOS on semiconductor  devices built using Cu technology are provided.  ESDFOS  damage to both Cu- and Al-technology devices results in  small to medium local surface damage at a site limited to an  area of a few microns, which would not be compatible for  external mechanically-induced damage.  The characteristic  spikes and peaks observed with ESDFOS damage on Altechnology wafers are absent from Cu-technology wafers.  The Al-technology wafers usually show damage involvement  limited to the top 2 metal layers, while in Cu-technology  wafers, the subsequent cracking and shorting usually reaches  deeper, causing both lateral as well as vertical shorts and  increasing the likelihood of misdiagnosis as mechanical  damage.  The evidence presented will improve the correct  diagnosis of ESDFOS-generated passivation damage for Cutechnology devices, enabling identification and correction of


Fig.  17: ESDFOS process root causes in assembly process  tools.  The most critical tools were pick & place, taping/ detaping and dicing.  In these steps, preventive measures  against ESDFOS should be taken, like good grounding, useful installation of ionizers, antistatic material and  process media selection etc.  Too many tools lack suitable  internal ESDFOS protection.  (Y-scale=% of investigated  tools)


the device process steps contributing to assembly final test  yield loss.


Acknowledgements:


The authors thank Joachim Reiner from Austria Micro  Systems, Graz (AT) for the calculation of the needed energies  for melting shown in Table 1 and for some valuable hints in  impact energy estimations.


[1] Jacob, P., Reiner, J.C., “Assembly Processes - a Surface


Electrostatic Discharge Killer for Devices and a FA


Challenge”, ASM-EDFAS, “Electronic device failure


analysis”.  2005, vol.  7, issue 2,  pp.6-12


[2] Jacob, P., Reiner J.C., ”Electrostatic Effects on


Semiconductor Tools”, Transactions on Device and


Microelectronics Reliability 44, 2004, pp.  1787-1792


[3] Jacob, P., Nicoletti, G., ”Manufacturing-Robotic-Induced


“Mechanical Damages” on Semiconductor Dies:


Mechanics, Electrostatics or What Else ?”, 12th


International Symposium on the Physical & Failure


Analysis of Integrated Circuits, IPFA 2005, June 27-July


1, 2005 Singapore, IEEE Catalogue No


05TH8827,pp.307-312


[4] Jacob, P., Nicoletti, G., “Surface Electrostatic Damage by


Micro-Process Robotic Machines: Diagnosis and


Reliability, Process-Auditing and Remedies”, Transactions


on Device and Materials Reliability, IEEE Transactions on


Device and Materials Reliability, Vol.  6, No.2, June 2006,


p. 213-220


Fig. 1: A very small ESDFOS impact, top view


Fig. 2: Cross section of the beginning of Fig.1; the top impact  has not disturbed the structure yet. Also, the crack doesn’t  reach the metal structures.


Fig. 3: Continuing the cross section to the crack’s center  shows structural damage  affecting the top two metal layers. In contrast to ESDFOS on aluminum devices, the direction of  damage is more vertical and without “needle spikes”.


Fig.4: This medium size ESDFOS impact shows severe  damage to the top 2-3 metal layer structure. Much of the  spark  energy has been consumed to melt the comparably  thick passivation – which could still not prevent the structural  damage.


Appendix


ESDFOS Damage Examples in Cu-Technology


Fig. 5: Similar to effects seen on power semiconductors with  their very thick metallization, balls have been observed, hiding ESDFOS impacts underneath. The ball is a “collection” of molten passivation material. Looking at this  image, no one would think about ESDFOS, but the cross  section shows, what happened…


Fig. 6: Cross section of Fig. 5. The ball was positioned  exactly on top of the slightly cracked piece of surface  passivation (white square). Since the adhesive contact of the  ball deteriorated during the continuous cross section  progress, the ball disappeared.


Fig. 7: In this case, the discharge cracked and locally melted  the passivation. Again, if not performed intentionally, no one  would suspect ESDFOS by looking at this image.


Fig. 8: Detail image of Fig. 8, indicating that still no damage  to the structure has been made. However, the horizontal part  of the crack at the right side show, that the passivation has  been  opened.


Fig. 9: Overview image of a small “ball-type” impact, apparently showing some passivation opening.


Fig. 10: The ball disappeared again during the cross  sectioning process.  However, in this case, the impact is more  severe and destructive than that of Fig. 6.


Fig. 11: It looks like a harmless particle on top of the  passivation, but a strange hole (arrow) indicates that  something strange happened….


Fig. 12: The cross section through the hole shows a severe  ESDFOS impact.


Fig. 13: The detailed magnification of Fig. 12 shows the three  top metal layers affected by this fulgurite-like surface ESD  impact.


Fig. 14: A very severe ESDFOS impact, hurting and shortcircuiting the three top metal layers.


Fig. 15: This extremely severe ESDFOS impact locally  destroyed even the four top metal layers


Fig. 16: Finally, the comparison to this very tiny crack, reaching through four metal levels, illustrates the wide variety  of severeness of ESDFOS damage textures.


Detection and Verification of Silicide Pipe Defects on SOI  Technology Using Voltage Contrast Inspection


Oliver D. Patterson, Hyoung H. Kang, Jay Strane, Christian Lavoie, Karl Barth, Xu Ouyang  IBM, Hopewell Junction, NY


Kevin Wu


KLA-Tencor, Hopewell Junction, NY


A methodology for detecting silicide pipes on SOI technology  in-line soon after their formation is described.     Techniques  currently exist to detect pipes in-line, but only much later in  the process.   This methodology, which is based on voltage  contrast inspection of test structures, allows experiments to be  completed more quickly providing much faster cycles of  learning.  Two different test structures are described.  The first  one was designed for other purposes but was adopted for  silicide pipe detection at M1.  The second was specially  designed and allows pipe detection at silicide anneal, W CMP  and M1.    A procedure for determining the cause of buried  shorts detected by the eS32 is also described.    Experimental  results are presented to demonstrate the benefit of this  technique.


Silicide pipes, which consist of deep lateral encroachment  from the source or drain of a device into the channel, are one  of the key defects that integration teams must overcome to  produce successful 45nm and 32nm technologies.  Therefore, effective characterization tools to detect and quantify silicide  pipe defects are essential.   Generally, pipe issues are detected  by failure analysis of functional structures such as SRAM  arrays at the fourth metal or later, much later in the process  than the point at which the defect forms.  Learning cycles  when relying on this metric are very slow.    Therefore great  motivation exists to develop techniques for detecting silicide  pipes much earlier in the process flow.


Electrically testable structures for detection of silicide pipes  may be created and tested as early as the first metal level (M1).  These structures suffer two major disadvantages.  First, to efficiently utilize the probe pads, large numbers of devices  must be tested in parallel.   The leakage current when all  devices are good is already large so that if only one device is  affected by the defect, the signal may be hidden within the  background leakage.  This leads to an upper bound on the size  of these test sites which limits their statistical significance.   Second, M1 test occurs much later in the process sequence  than when the silicide pipes are potentially formed.   Experiments therefore still take a long time and this metric


cannot be used to partition the process to track the formation  of the encroachment.


In-line voltage contrast (VC) inspection is being pursued as an  alternative approach.   In-line VC inspection has proven to be  very effective for detection of many types of yield limiting  defects, including missing spacer, contact opens and metal and  via opens, soon after formation [1,2,3].  This technique can  isolate the exact defective device, does not require pads  thereby saving space and can be applied much earlier than M1.   Silicide pipes may be detected on bulk technologies as early as  the silicide anneal step.   For instance, under electron  extracting conditions, a pipe on an nFET will short to the body  of the FET and therefore to the substrate showing a bright VC  signal as shown in Fig. 1.  This particular defect was detected  at W CMP.   For silicon-on-insulator (SOI) technologies  however, detection is more challenging.   Since the transistors  are isolated from the substrate, all transistor elements are  floating.  Therefore a pipe in the SRAM produces little if any  change in the VC signal.  An alternative approach is  necessary.    The proposed alternative approach is to use test  structures.


This paper describes two test structures useful for detection of  silicide pipes on SOI technology.   The first is a probe-able  test structure which was adopted for silicide pipe detection.   The second is a VC test structure specifically designed for  detection of silicide pipes.  How these work and their  advantages are described in Section 2.   Silicide pipes like  many other defect types are below the wafer surface when  detected.   Determining the cause of the VC signal, whether it  is a silicide pipe or another mechanism, can be very difficult.   In many situations, the VC defects are not visible to other  tools such as an in-line FIB.    This is because e-beam  inspection tools are capable of much larger beam currents than  other tools.   A procedure was developed to mark these defects  with an in-line FIB, when the FIB cannot see them, so they  can be re-isolated and analyzed using failure analysis (FA) lab  techniques such as planview and TEM.  This procedure is  described in Section 3.    This silicide pipe detection and  analysis methodology is actively being utilized at the IBM  Microelectronics Semiconductor Research & Development  Center.  Recent results are described in Section 4.


Figure 1:  top) Appearance of silicide pipe in bulk  SRAM.   bottom) Corresponding cross section showing the pipe.


2. Test Structures


Different test structures were used to detect silicide pipes for a  recent SOI technology.   Early in the technology development, specifically designed VC test structures were not available.   The structures on the mask set in use at that time were  evaluated for their usefulness for silicide pipe detection.   An  appropriate structure was found.  Eventually, as new mask sets  were prepared, a custom VC test structure was designed  offering a number of additional advantages.


Adopted Probe-able Test Structure at M1


The electrically testable structure shown in Fig. 2 was adopted  for detection of silicide pipes via VC inspection at M1.  Conveniently, the drains of the nFETS are connected to a long  metal line, which serves as a virtual ground.   The sources are  connected to small metal pads.   If a defect exists which shorts  the source to the drain, then the source metal pad will light up (emit more electrons) like the long metal line, as shown in Fig.


3.    Various mechanisms can cause this signal including a  silicide pipe.    Figure 4 shows the silicide pipe defect that  corresponds to the defect in Fig. 3.


Figure 2: Test structure adapted for VC inspection for silicide


pipes.  Blue – M1,  Green – gate, yellow – active, white


checkers – contact


Figure 3: VC signal for a  short


Figure 4: Silicide pipe defect corresponding to the VC signal  in Fig. 3.


Custom Designed VC Test Structure for Silicide Pipe  Detection


The advantages of in-line VC inspection can be more fully  exploited with a specially designed VC test structure.   The  main limitation of the structure presented above is that it is  first testable at M1.   The VC test structure shown in Fig. 5  was specifically designed for detection of silicide pipes using


VC inspection at the silicide anneal, W CMP and M1 levels.   The layout is derived from the target SRAM cell for this  technology.   As typical throughout the industry, it contains  six transistors including two nFET pass gates, two nFET pull  down gates and two pFET pull up gates.   The drains of all  four nFETs are grounded from a ground bus running along the  left and right edges of the image.   The sources of the nFETs, specifically the bitline (BL) and ground (GND) contacts will  typically be floating as all nFETs under normal VC inspection  conditions will be off.


Figure 5: VC test structure specifically designed to detect  silicide pipes.  Green – gate, yellow – active, pink – contact, red – rectangular contact


For this structure, the gates are also grounded.   The goal in  designing it this way was to ensure the gates stay off.   Unlike  the normal SRAM cell, thick gate oxide is used for this test  structure.  This is so that false positives due to gate oxide  leakage are eliminated.  The structure shown in Fig. 5 is just  one of a number of versions utilized at IBM.  For another  version of this structure, the contacts are moved further away  from the gate stack eliminating defects due to contact to gate  stack shorts.  For yet another, the gates are left floating, eliminating the possibility of defects due to shorts to the gate.    The mix of structures scanned depends on how we want to  balance the efficiency of the inspection with simplicity of data  interpretation.    Table 1 summarizes the structures mentioned  in this paragraph.    The most efficient inspection would be to  just inspect structure A.   Silicide pipes, contact to gate shorts  and missing spacer mechanisms would all be detected with  this inspection.   Interpretation of the data would be more  difficult however as it would be unclear without failure  analysis which defect mechanism caused each failure.   An  alternate plan would be to inspect both structures B and C.   Test structure C failures would uniquely be caused by silicide  encroachment.   If structure B had a higher number of fails, this would indicate a missing spacer issue.   There are actually  more mechanisms that can cause these structures to fail.  For  simplicity, they are not all listed here.   The point remains the  same; by using multiple structures different mechanisms can  be decoupled allowing interpretation of the results without  failure analysis.


A structure similar to these is reported in Moreau et al. but for  detection of dislocations on bulk technology [4].   The  structures reported in this paper are different from this  structure in that they very closely mimic the target SRAM cell  for the technology and because they are for SOI technology


and require a more complicated grounding strategy.   Grounding of the active area to enable inspection at the  silicide level is difficult because the active area is isolated  from the substrate by the buried oxide layer which defines  SOI.   Grounding was achieved by a large active area  capacitor similar to the way Weiner et al. [5] suggests  grounding a gate stack.    This capacitor is about 25% of the  structure area.  Additional grounding is added at the W CMP  step.  At this point in the process, the process flow provides a  way to contact the substrate through the buried oxide.


Table 1: Test structures and their sensitivity to different  failure mechanisms.


Figure 6 shows how the structure shown in Fig. 5 appears  during VC inspection at the W CMP level.   The cells are  separated in the x direction to allow space for the ground  buses.   In the y direction, just like for normal SRAM, many of  the contacts are shared between neighboring cells.   Therefore  in the columns containing the BL and GND contacts, the  contacts alternate between bright and dark.  All healthy BL  and GND contacts are floating (and appear dark) whereas all  the drain contacts are grounded (and appear bright).   When  one of the BL or GND contacts is bright, this indicates a  defect.  The arrow in Fig. 6 points to a bright BL contact.


Figure 6: VC signal for potential silicide pipe


This structure may be inspected after silicide anneal, W CMP  and M1, and numerous places in between.   This is because  contacts land on each drain source and gate and each of these  contacts is independently extended up to M1.  This structure, unlike the one in Fig. 3, is therefore useful for determining the  point in the process where such defects form and their  evolution with further processing and increased thermal  treatment.   Another advantage is that, when tested after  silicide anneal, some common defects that may cause a signal  in the first structure such as contact to poly shorts will be ruled  out because the contacts have not been formed yet.   At third  advantage is that the VC signal is strong enough to be detected  with a FIB.


3. Defect Verification with In-Line FIB


Verification of VC defects on the structure in Fig. 2 through  failure analysis is very difficult because they only show up  under the high beam current of a VC inspection tool.   This is  a common problem for many FEOL defect types detected with  VC inspection.   Failure analysis is critical for these defects  first to verify that the mechanism is a true killer defect and  then later to determine the cause from a number of possible  causes.


A procedure was developed to accurately mark defects like  this with an in-line FIB for planview analysis.  This procedure  consists of the following steps:


1. Blindly mark defects with an in-line FIB using the  KLARF from the VC inspection.  Alternately, X and  Y offsets from a known point on the design (e.g. the  top left of the test structure) may be used.   Marking  consists of placing vertical and horizontal marks  within microns of the defect and adding a large  fiduciary mark, visible with an optical microscope, somewhere nearby.


2. Reload the wafer in the inspection SEM and take  images of the defects and FIB marks.


3. Prepare a document for the FA analysis team  specifying the location of each defect on the wafer (i.e. which die and roughly where on the die) plus the  images taken in step 2.


Figure 7 shows the FIB mark for the defect in Fig. 4.


Figure 7: FIB marked defect


4.  Results


Apparatus


A KLA-Tencor eS32 E-beam inspection system was used for  VC inspection.   The test structure designs were placed on  mask sets fabricated at IBM’s building 323 300mm fab.   An  FEI DA300 dual beam tool was used for the FIB work


Experimentation


These structures are routinely inspected and trend charts are  routinely reported.  Samples are submitted to failure analysis  weekly to get to a sense of how many are silicide pipes and  how many are due to other mechanisms.   Figure 8 shows  some of the defect types detected using this structure.   This  information is useful for maintaining the yield loss Pareto for  this technology.


Figure 8: Failure types detected by test structure a.  top) Contact to gate stack misalignment, middle) systematic W


deformity over the gate stack, bottom) silicide pipe.


The most important use of this methodology is during yield  ramp for evaluation of split experiments.   The sample in Fig. 4 was part of an experiment to intentionally modulate the  number of silicide pipes by wafer using different metal  deposition thicknesses and pre-cleans.  Figure 9 shows that  silicide deposition 1 and pre-clean 1 produced the best results


as expected.  Figure 10 shows the results for another split  experiment investigating variables including silicide  composition, thickness and anneal temperature.    Splits S1  and S4 are much worse than the others.  Figure 11 shows a  scatter plot comparing the SRAM yield with the eS32 defect  count.    The VC inspection defect count predicts the SRAM  yield well with high defect counts correlating to low yields.  The results for these experiments were available for evaluation  within a week, weeks earlier than when they were later  confirmed with SRAM test.


0 5000 10000 15000 20000 25000


silicide dep 1


silicide dep 2


silicide clean 1


silicide clean 1b


silicide clean 2


Figure 9: Results of silicide pipe formation study.   Silicide  deposition 1 is better than silicide deposition 2.   Silicide clean  1 is better than silicide clean 2


Figure 10: Results of a study comparing  different metal


compositions and thicknesses and different anneal


5. Conclusions


VC inspection may be used to detect silicide pipes in-line and  other transistor level defect types soon after their formation.   For SOI technology, this is possible using special test  structures, two of which are described in this paper.   A  procedure for verification of the defects detected by this  methodology is also described.  This methodology may be  used to greatly shorten the learning cycle for elimination of  silicide pipe defects.


Figure 11: SRAM yield versus defect count for the second  study.   The outlier at a defect count of 300 is because almost  all defects landed on two die.   The VC inspection defect count  predicts the SRAM yield well with high defect counts


correlating to low yields.


We thank Scott Jansen, Greg Johnson, Larry Garrison for the  image of the silicide pipe in bulk technology.  We  acknowledge Asa Frye for running the split experiments  described in the Results section.  This work was performed at  the IBM Microelectronics, Semiconductor Research & Development Center, Hopewell Junction, NY 12533.


[1] O. D. Patterson, J. L. Drown, B. D. Crevasse, A. Salah, K. K. Harris, “Real Time Fault Site Isolation of Front-end  Defects in ULSI-ESRAM Utilizing In-Line Passive  Voltage Contrast Analysis”, Proceedings of ISTFA, Nov  2002, pp. 591-599.


[2] Patterson, O. D., Wu, K., Mocuta, D., Nafisi, K., “Test  Structure and e-Beam Inspection Methodology for In-line  Detection of (Non-visual) Missing Spacer Defects”, Proceedings of ASMC, 2007.


[3] R. Guldi, J. Shaw, J. Ritchison, S. Oestreich, K. Davis, R. Fiordalice, “Characterization of Copper Voids in Dual  Damascene Processes”, Proceedings of ASMC, April


2002.


[4] O. Moreau, A. Kang, V. Mantovani, I. Mica, M.L. Polignano, L. Avaro, C. Pastore, G. Pavia, Early detection  of crystal defects in the device process flow by electron  beam inspection”, Proceedings of ASMC, 2006, pp. 334-339.


[5] K.H. Weiner, G Verma, P. Nunan, I. De, “Apparatus and  methods for determining and localization of failures in  test structures using voltage contrast”, Patent US6861666,


Photo Process Margin Leading to IC Failures- A Case Study


Vijay Chowdhury, Clement Hsu and Ada Yu  Altera Corporation


101 Innovation Dr.


San Jose, CA 95134


Abstract:   Inherently small process margins in patterning are a


dominant cause of device yield variability, when process


conditions or production lines change. This paper highlights the


fact that in spite of a perfect lithographic model, the post OPC


variation can be substantial due to manufacturing variability.


Pattern integrity is a non-intuitive complex mix of


manufacturing process practices combined with manufacturable


design practices. Failure analysis is the only effective means for


filling the understanding gap for yield management in this case.


A case study of yield drop due to layout dependent process


marginality and a methodical approach to get to the root of the


problem are described in this paper.


Introduction:


As technologies shrink beyond 130nm, a more systematic class


of failures is cropping up1. This class of failures stems from


layout interaction with the manufacturing process. Slight


variability in the performance of manufacturing tools creates an


exaggerated effect on the product leading to very subtle but


nagging failures. Special attention and tools2 are required to


understand the underlying cause of these failures. Failures


studied in this paper did not fall into a major yield hit category;


however, they were very systematic in nature with a distinct


reticle pattern (Fig. 1). Electrically, they manifested on the


product as ‘read disturb’ failures with an orderly pattern i.e.: the


appearance of the failure was associated with certain specific


columns and rows (fig.2). This case study discusses the


investigation of this subtle failure mode and the approach taken


to understanding the root cause. Nanoprobing tools3 are


identified to be fundamental to detailed electrical analysis of


such failures.


Process/Device Integration:


The devices investigated in this study were fabricated using 0.13


μm CMOS technology. The 193 nm lithography with optical


proximity correction was used for active, gate and contact layers.


The 28Å gate oxide was formed by thermally nitrided oxide to


enable low-standby power applications. Super steep retrograde


indium/arsenic channel implant and tilted pocket with shallow


source/drain extension implant is used to control device short


channel effects.


Problem Description:


Several lots suffered reticle related failures with specific failing


bit locations (see table below). The CRAM cell flipped (“1” to


“0”) during read process.  Physical failure analysis showed no


field related pattern at the failure location. Several failure


scenarios were considered in the order of likeliness:


• Defective cell due to poor transistor performance


• High Vt due to lack of poly dopant activation


• Low Vt due to halo implant shadowing


Layout Observations:


The CRAM layout of failing columns was identical to the


passing columns in general. However, certain unique layout


features were observed in specific regions of the failing columns (Fig.3 ) These features had a narrow spacing in N-diffusion


(about half of the passing columns). Additionally, the core Nimplant was also narrower.


Results:


A thorough layout analysis followed by nanoprobing confirmed  the failure to be specific to certain transistors with  poor


performance.  Nano-probing was performed on failing bits to


understand the electrical nature of the failures. Results on two


samples suggested low current on NMOS transistor (Figs. 4 &5). The results confirmed that the transistors were weaker compared  to the control devices. The layout locations were immediately


sent to the fabrication house to check their in line wafers along  with the problem lot list (see table below). The KLA scan


showed abnormal photoresist pattern (Fig. 6&7) and the


locations matched suspect failing bits. The uniqueness of the


layout made the failing rows and columns more vulnerable to


this failure. The photoresist collapse hindered with the


dispersion of NLDD and pocket implants (Fig.9).  The column  and row failures were ascribed to blocked NLDD and pocket


implant.


The list of impacted lots was instrumental in identifying the


culprit tool (Fig. 8). A correlation done with the impact lots


confirmed the failures due to a bad tool. This tool was not


optimized for OPC.


Conclusion: Subtle read disturb failures seen on several lots and  products had a pattern specific marginality. These layout


dependent systematic failures are on the rise as technologies are  shrinking, small variations in the manufacturing window can


throw the balance off. The results of this work illustrate the


importance of a good DFM methodology. Handcrafting of


repeating layout elements and additionally a methodology to


lock these repeating elements to develop a uniform and robust


layout is imperative to high yield/performance /low cost as


process & design rule complexity, proximity effects keep


increasing with each new generation of technology.


Acknowledgement:


The authors would like to thank the Yield Enhancement teams


for their technical support.


Fig. 1 Composite wafer map showing failures with


a reticle pattern


Table: showing the lots with the intensity of the reticle


pattern on two distinct products of the family.


Failure Column Distribution


Failure Row Distribution


Fig. 2 Distribution of the failing bits shows a  systematic problem  with specific columns (158-159) and rows (1,5,9 &13) failing


persistently.


BITMAP  FAILURE  COLUMN


PRODUCT LOT RETICLE PATTERN


Faint


Yes


Product 1


Gross


Product 2


Fig. 3. Layout of the failing elements shows pattern uniqueness on   the failing  rows and columns when compared to the


non-failing elements


1.0E-05


2.0E-05


3.0E-05


4.0E-05


5.0E-05


6.0E-05


7.0E-05


8.0E-05


Series1 Series2 Series3 Series4


1.2E-04


1.4E-04


1.6E-04


Fig. 4 NMOS Id-Vd characteristics on sample #1.  Nanoprobing  results suggest low current on NMOS transistor (top-failing xtor) as compared to the control (bottom)


Ser ies1 Ser ies2 Ser ies3 Ser ies4


1.8E-04


2.0E-04


Fig. 5 NMOS Id-Vd characteristics on sample #2.  Nanoprobing  results suggest low current on NMOS transistor (top-failing xtor) as compared to the control (bottom)


Fig. 6. Inline wafer inspection at thick implant mask showed


abnormal photo resist pattern from lots processed from bad tool (top). Bottom picture from a good tool shown for comparison.


Fig. 7. A close up of photoresist collapse seen on top (failing) vs


bottom (passing identical region).  This was consistent with the


lots processed from bad tool.


Fig. 8. Graph compiled with the impact lot list showing high failure   rate correlated very well to a specific tool.


ig. 9. Drawing describes the manifestation of the failure at the


dhury et al, Translating Yield Learning Inot


N.-E. Microprocesses and


collapsed photoresist.


1.Vijay Chow


manufacturable Designs Proceedings of 32nd International


Symposium for Testing and Failure Analysis pp.402-406


2.  Myeong-Cheol Kim et al, Substrate temperature effects o


193 nm photoresist deformation and self aligned contact hole   etching performances Journal of Vacuum Science & Technolog vol24, Issue 5, pp 2331-2336


3. Kim, D.H.; Cho, S.H.; Lee,


Nanotechnology Conference, 2004. Digest of Papers. 200


International, Vol., Iss., Oct. 27-29, 2004, Pages: 192- 193


Failure Analysis of Multi-Fingered HV Symmetric Devices for Charge-Pumping Circuit  Applications


Liang-Feng Wen, Ting-Chien Wang , Chien-Hui Chen


Taiwan Semiconductor Manufacturing Company, Ltd.


25 Li-Hsin Rd., Hsinchu Science Park, Hsinchu, Taiwan, R.O.C.


The purpose of this paper is to present a systematic analysis  methodology for a newly taped-out High Voltage (HV) product that has encountered a 0% yield issue. In order to  identify the root cause and improve the yield, a series of  electrical analysis experiments designed to reveal the failure  phenomenon of the charge-pumping circuit were applied. Combining spice simulation data, I-V curve measurements, CAFM measurements and nano probing, the difference in  resistance for a multi-fingered symmetric device was revealed. A deductive method was then used to conduct layout analysis, and an in-line split experiment was developed to explain the  failure phenomenon experienced by the multi-fingered HV  symmetric device for a charge-pumping circuit.


The newly taped-out product that is discussed here is a  LCD driver with a single chip solution designed for TFT-LCD  panel module of a mobile phone, using a 1.8V/5V/32V HV  process. However, following the CP test, feedback from  customer indicated that chips tested from the pilot run wafers  did not meet the expected voltage target for the chargebumping circuit. [1] The measured driving current was only  around 10% of the expected level, which meant that lower  driving capability was unable to generate enough voltage to  supply power to the VGH and VGL pins of the common gate  of the TFT device on the panel. The initial yield is 0% based  on the original design specifications. This, of course, would  have induced a huge impact on the customer’s business.


In order to determine the root cause, a resistance test of  the step-up [2] circuit was analyzed. (Figure 1)


FIGURE 1: Schematic of the On-Resistance test circuit under  reset conditions.


A circuit was setup containing one capacitor and one  current meter in order to sample the current flow from the  output pad of the charge-pumping circuit. The driving current  was only about 10% of the expected level. The target voltage  for a step-up circuit is 19.2V. The output voltage of a good  sample is around 19.0V to 19.1V. However, the output voltage  of a bad sample is around 14.9V to 15.0V under the same  conditions. Figure 2 shows a comparison of the output voltage  for good and bad die. The Y-axis is the voltage of the C21P  pad. The slope of a good sample is linear, but a bad sample is  not.


FIGURE 2: An output voltage comparison between a  good/bad die. The Y axis is the voltage of the C21P pad. The  slope of a good sample is linear, but a bad sample is not.


To make a better comparison, the performance of the  output pins between good/bad samples was studied. Based on  the simulation data, the Ids value of a good pin is around –400~+800uA, as the C21P voltage was swept from –4~+5V. The pins that failed showed low Ids value (-40uA~+40uA). (Figure 3)


FIGURE 3:  The PMOS device performance of good/bad  charge-pumping pins.


It was suspected that the high resistance issue in the  step-up circuit was the cause of the low driving current of the  output pin, enabling reasonable speculation that the weak  performance of the multi-finger HV PMOS resulted in poor  circuit performance. (Figure 4)


Drain Source


FIGURE 4: A schematic of the partial charge-pumping circuit  of a multi-finger HV symmetric device


An FIB was conducted to clarify whether  there any  signal controls were causing errors in the charge-pumping  circuit Normal bias condition were applied to monitor whether  the gate voltage could be controlled as well as the designer  expected. The results showed that gate voltage could be well  controlled, and it was clarified that there were no design  issues.


Nano probing [3] was then carried out to measure the  Id vs. Vd and Vg to verify the electrical characteristic of the  multi-finger HV symmetric device. The probing result showed  that the higher Ron values were found in the multi-finger HV  symmetric device when compared to those of a single HV  symmetric device especially for the HV PMOS in the test line. The phenomenon that was causing the failure in the multifinger HV PMOS was confirmed. (Figure 5)


FIGURE 5: Nano probing results for a multi-finger HV  symmetric device


Therefore, after consulting the customer regarding the  placement of the multi-finger symmetric device on the actual  chip, the measurement of the C-AFM was continued. (Figure  6)


FIGURE 6: C-AFM measurement of the HV circuit.


Non-uniform current mapping was found in the stepup circuit. Poor salicide formation was found by using FIB


analysis on the multi-finger HV structure in the step-up circuit. (Figure 7)


FIGURE 7: Poor salicide was the root cause that induced high  Ron levels in the multi-finger HV symmetric device.


It was believed that poor salicide was the root cause  that induced high Ron levels in the multi-finger HV symmetric  device. This information was forward to the customer and the  FAB, layout structure and process conditions were thoroughly  reviewed. In order to identify the optimal process conditions, several photo experiments were conducted. The best process  conditions were created by increasing exposure energy by 25% and adjusting the exposure focus to its optimum setting. (Figure 8)


FIGURE 8: Process solution: Determine the best exposure  energy/focus using photo FEM experiment.


Using a systematic electrical and physical analysis of a new  pilot product where the yield was 0%, the root cause of the low  driving current that resulted in the failure of the charge  pumping circuit is successfully identified and resolved. Using  advanced nano probing technology, it was discovered that the  Ron of a multi-finger HV symmetric device is much higher  than that of a single device, and that the multi-finger HV  symmetric device was connected to a single high resistance  resistor. Non-uniform formation of W salicide on the OD of  source and drain node was revealed through PFA and was  identified as the root cause due to photo marginality when  removing the HVOX layer. The corrective action taken by the  FAB was to fine tune the process window based on the FEM  experiment by increasing the photo energy so that it opened  the OD of the source/drain. After the new process conditions  were applied, the yield was greatly improved from 0% to ~90%.


[1] C. Yoo and K.-L. Lee: “A Low-Ripple Poly-Si TFT  Charge Pump for Driver-Integrated LCD Panel”, IEEE  Transactions on Consumer Electronics, Vol. 51, No. 2, MAY  2005


[2] Emmanuel Racape, Jean-Michel Daga,” A PMOS-Switch  based charge pump, allowing lost cost Implementation on a  CMOS standard process”, Proceedings of ESSCIRC, Grenoble, France, 2005


[3]C.C. Wu and J.C. Lee, “Single device characterization by  Nano-probing to identify failure root cause”,  Proceedings of  the 31th ISTFA 2005.


Voiding in Cu technology through photovoltaic-driven electrochemical  dissolution


Frank A.Baiocchi, John DeLucca, James T. Cargo  LSI Corporation


Allentown PA 18109


Abstract:


It has been found that a process-design  interaction involving very large capacitor arrays is  capable of causing voiding in well-formed copper  trenches.  This voiding is believed to be caused by  the electrochemical dissolution of copper driven by  the photovoltaic effect realized at p-n junctions.  A  series of experiments was performed to reproduce  this voiding in a laboratory environment using  water and exposure to light or dark.  The  experiments were performed on two different size  capacitor arrays.   In addition, similar experiments  were performed on a large capacitor array that uses  the opposite dopant isolation scheme.  Conversely, copper dendrite growth was observed at the  features of interest instead of dissolution, even  under flowing de-ionized water (DI) conditions.  The results are discussed in the context of known  copper-water electrochemical equilibria and design  implications are discussed.


A yield failure was investigated on an  experimental design that contained a large MOS  capacitor array and had an electrical failure  signature indicating a high resistance in series with  the capacitor. The high resistance was eventually  isolated to a voided metal2 (M2) runner connected  to the large MOS capacitor structure as shown by  the Focused Ion Beam (FIB) cross section in figure


1. Electromigration voiding was ruled out since the  devices failed prior to operation at normal current  loads.  Also, there was no evidence of the missing  copper accumulating elsewhere in the device.


Figure 1: Focused ion beam (FIB) cross-section  image of a voided metal2 runner connected to a  large capacitor structure.


TEM images were obtained for a clearer look at  the structure of the voided metal and the dielectric  layers around it. The TEM image in figure 2  clearly shows that the material processing all  around the voided M2 runner was properly  performed.  The missing copper appears to have  been removed during normal processing steps, and  the shape of the voided region suggests that this  voiding happened in an isotropic manner, consistent with a wet etch or clean step, after the  vias to the M2 runner were opened.


The voiding is believed to be caused by the  electrochemical dissolution of copper during  normal process steps when metal is temporarily  exposed through via holes, and is believed to be  driven by the photovoltaic effect realized at p-n  junctions.


M2 runner  connecting  to MOS


capacitor


M3 strap

