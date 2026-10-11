---
title: "ISTFA-2005_compressed.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_46a81e5c7871a849ff163dd37b51f4b97295230462135641
file_size: 84868561
---

ISTFA  2005


Proceedings of the


31st International Symposium for


Testing and Failure Analysis


November 6–10, 2005


McEnery Convention Center  San Jose, California


Sponsored by


Published by


ASM International®


Materials Park, Ohio 44073-0002


www.asminternational.org


© 2005 ASM International. All Rights Reserved.


ISTFA 2005 Conference Proceedings from the 31st International Symposium


for Testing and Failure Analysis, Book + CD (#02207Z)


TM


Copyright© 2005


by


All rights reserved


No part of this book may be reproduced, stored in a retrieval system, or transmitted, in any form or by any  means, electronic, mechanical, photocopying, recording, or otherwise, without the written permission of  the copyright owner.


First printing,  October 2005


Great care is taken in the compilation and production of this Volume, but it should be made clear that NO  WARRANTIES, EXPRESS OR IMPLIED, INCLUDING, WITHOUT LIMITATION, WARRANTIES  OF MERCHANTABILITY OR FITNESS FOR A PARTICULAR PURPOSE, ARE GIVEN IN  CONNECTION WITH THIS PUBLICATION. Although this information is believed to be accurate by  ASM, ASM cannot guarantee that favorable results will be obtained from the use of this publication alone. This publication is intended for use by persons having technical skill, at their sole discretion and risk. Since  the conditions of product or material use are outside of ASM's control, ASM assumes no liability or  obligation in connection with any use of this information. No claim of any kind, whether as to products or  information in this publication, and whether or not based on negligence, shall be greater in amount than the  purchase price of this product or publication in respect of which damages are claimed. THE REMEDY  HEREBY PROVIDED SHALL BE THE EXCLUSIVE AND SOLE REMEDY OF BUYER, AND IN NO  EVENT SHALL EITHER PARTY BE LIABLE FOR SPECIAL, INDIRECT OR CONSEQUENTIAL  DAMAGES WHETHER OR NOT CAUSED BY OR RESULTING FROM THE NEGLIGENCE OF  SUCH PARTY. As with any material, evaluation of the material under end-use conditions prior to  specification is essential. Therefore, specific testing under actual conditions is recommended.


Nothing contained in this book shall be construed as a grant of any right of manufacture, sale, use, or  reproduction, in connection with any method, process, apparatus, product, composition, or system, whether  or not covered by letters patent, copyright, or trademark, and nothing contained in this book shall be  construed as a defense against any alleged infringement of letters patent, copyright, or trademark, or as a  defense against liability for such infringement.


Comments, criticisms, and suggestions are invited, and should be forwarded to ASM International.


ISBN: 0-87170-823-X


SAN: 204-7586


Materials Park, OH 44073-0002


Printed in the United States of America


Multiple copy reprints of individual articles available from Technical Department, ASM International.


EDFAS 2005-2006 BOARD OF DIRECTORS


EDFAS President


EDFAS Vice President


Mr. Gary F. Shade


Dr. Daniel L. Barton


Intel Corporation


Sandia National Laboratories


Hillsboro, OR


Albuquerque, NM


|Board Members Affiliation |Board Members Affiliation |Board Members Affiliation |
|---|---|---|

|Dr. Christian Boit |Secretary |TUB Berlin University of Technology |

|Mr. James J. Erickson |Member At Large |Boeing Satellite Systems, Inc. |

|Dr. Thomas M. Moore |Member At Large |Omniprobe, Inc. |

|Mr. Tracy D. Myers |Member At Large |LSI Logic Corporation |

|Mr. Thomas S. Passek |Executive Director |ASM International |

|Dr. Seshagiri V. Pabbisetty |Member At Large |Esparsa |

|Mr. Richard J. Ross |Immediate Past President |IBM Systems & Technology Group |

|Mr. Jerry M. Soden |Member At Large |Sandia National Laboratories |

|Mr. Matthew Thayer |Member At Large |Advanced Micro Devices |

|Board C ommittees Affiliation |Board C ommittees Affiliation |Board C ommittees Affiliation |

|Dr. Lawrence Wagner |ASM BOT Liaison |Texas Instruments, Incorporated |

|Mr. Thomas Zanon |Education Chair |Carnegie Mellon University |

|Dr. Jacob Phang |EDFA Chair |National University of Singapore |

|Dr. Lee Knauss |Events Chair |Neocera, Inc. |

|Dr. Vijay Chowdhury |Membership Chair |Altera Corporation |

|Mr. Richard J. Ross |Nominating Chair |IBM Systems and Technology Group |

|Mr. Jerry M. Soden |Website Chair |Sandia National Laboratories |

|ISTFA 2005 ORGANIZING COMMITTEE PROGRAM CHAIRS |ISTFA 2005 ORGANIZING COMMITTEE PROGRAM CHAIRS |ISTFA 2005 ORGANIZING COMMITTEE PROGRAM CHAIRS |ISTFA 2005 ORGANIZING COMMITTEE PROGRAM CHAIRS |
|---|---|---|---|

|Lee Knauss |Cheryl Hartfield |William E. Vanderlinde |Chris Henderson |

|General Chair |Vice General Chair |Tutorial Chair |Symposium Chair |

|Neocera, Inc. |Texas Instruments, Inc. |Lab. for Physical Sciences |Sandia National Laboratories |

|Activities Chairs ||||
|---|---|---|---|

|Nicholas Antoniou |Edward P. Keyes |Matthew |Thayer |

|Exposition Chair |Users’ Groups Chair |Immediate |Past General Chair |

|Private Consultant |Semiconductor Insights |Advanced |Micro Devices |

|Dan J. Bodoh |Philippe Perdu |David |P. Vallett |

|Finance/Registration Chair |Panel Discussion Chair |Publicity |Chair |

|Freescale Semiconductor |CNES-French Space Agency |IBM |Systems & Technology Group |

|Sandra Delgado |Richard J. Ross |Jeremy |A. Walraven |

|Social/Local Arrangements Chair |Publicity Chair & EDFAS |Liaison Audio/Visual |Chair |

|Accurel Systems, Intl. |IBM Systems & Technology |Group |Sandia National Laboratories |

|Symposium Chairs ||||

|Felix Beaudoin |Joseph Clement |Phillip Kaszuba |Jerry Soden |

|Die Level Fault Isolation |Optical Techniques |Nanotechnology/SPM |Test |

|Thales Microelectronics |Sandia National Laboratories IBM |Technology Group |Sandia National Laboratories |

|Carol Boye |Ray D. Harrison Ted |A. Kolasa |Bryan Tracy |

|Yield Enhancement |Package Level Analysis |Posters |Metrology & Materials Analysis |

|IBM Syst. & Technology Group |Texas Instruments, Inc. |Freescale Semiconductor, |Inc Spansion, LCC |

|David L. Burgess |Robert Herrick Optoelectronic Christopher |Richardson |Zhiyong Wang |

|Discretes, Passives & MEMS |Devices FA |Process/ Case |Histories Advanced Techniques |

|Accelerated Analysis |R.W. Herrick Consuting LSI Logic |Corporation |Intel Corporation |

|Jeff Birdsley |Ron Hylton Alan |Street ||

|System Level Analysis |Sample Preparation |Circuit Editing for FA, FI ||

|Dell Corporation |Maxim Integrated Products and |Debug ||

||Qualcomm, |Inc. ||

|Tutorial Chairs ||||

|Vijay Chowdhury |Kultaransingh Hooghan |Kultaransingh Hooghan |Chris Richardson |

|Device and Test |Microscopy Tools |Microscopy Tools |Microscopy Tools; Yield |

|Altera Corporation |Hooghan Consultancy & |Hooghan Consultancy & |LSI Logic Corporation |

|Services |Services |Inc. |Inc. |

|Cosme Furlong |||Rosalinda M. Ring |

|Fault Isolation; Sample Prep. |Susan Li |Susan Li |Device and Test; Fault |

|Worcester Polytechnic Institute |Device and Test; Yield |Device and Test; Yield |Isolation |

||Spansion, LCC |Spansion, LCC |Intel Corporation |

|Leo G. Henry ||||

|Failure Mechanisms |Tracy D. Myers |Tracy D. Myers |Chad Rue |

|ESD TLP Consulting/Testing |Device & Test; FA Management Microscopy Tools |Device & Test; FA Management Microscopy Tools |Fault Isolation; Yield IBM Systems & Technology |

|Rebecca L. Holdford |LSI Logic Corporation |LSI Logic Corporation ||

|Packaging ||||

|Texas Instruments, Inc. ||||

ISTFA 2005 TUTORIAL COMMITTEE


William E. Vanderlinde


Organizing Committee Tutorial Chairman  Laboratory For Physical Sciences


|Tutorial Committee Chair |Topic |Affiliation |
|---|---|---|

|Vijay Chowdhury |Device and Test |Altera Corporation |

|Cosme Furlong |Fault Isolation; Sample Preparation |Worcester Polytechnic Institute |

|Leo G. Henry |Failure Mechanisms |ESD TLP Consulting/Testing |

|Rebecca L. Holdford |Packaging |Texas Instruments, Inc. |

|Kultaransingh Hooghan |Microscopy Tools |Hooghan Consultancy & Services |

|Susan Li |Device and Test; Yield |Spansion, LLC |

|Tracy D. Myers |Device and Test; FA Management |LSI Logic Corporation |

|Chris Richardson |Microscopy Tools; Yield |LSI Logic Corporation |

|Rosalinda M. Ring |Device and Test;  Fault Isolation |Intel Corporation |

|Chad Rue |Fault Isolation; Yield |IBM Systems & Technology |

|Shankar Subamanian |Microscopy Tools |Freescale Semiconductor, Inc. |

|Jeremy A. Walraven |MEMS |Sandia National Laboratories |

|Kendall S. Wills |F/A Basics; Packaging; Sample Preparation |Texas Instruments, Inc. |

ISTFA 2005 SYMPOSIUM COMMITTEE


ADVANCED TECHNIQUES


OPTICAL TECHNIQUES


Zhiyong Wang, Chair


J. Joseph Clemen, Co-Chair


Rajen Dias, Intel Corporation


Michael Bruce, Co-Chair


William Lo, Credence Systems


Advanced MicroDevices


Antonio Orozco, Neocera, Inc.


Daniel Bodoh, Freescale Semiconductor


Michael Twiford, Agere Systems


R. Aaron Falk, OptoMetrix, Inc.


David Vallet, IBM Systems & Tech. Group


Steven Kasapi, Credence Systems


Philippe Perdu, CNES-French Space Agency


CASE HISTORIES


Peilin Song, IBM


Christopher Richardson, Chair  LSI Logic Corporation


OPTOELECTRONIC DEVICES


Tracy Myers, LSI Logic Corporation


Robert Herrick, Chair


Thomas Paquette, Insight Analytical Laboratories, Inc. R.W. Herrick Consulting  Richard McClelland, Philips Semiconductors, Inc.


Michael Cheng, JDS Uniphase


Timothy McGrady, ATMEL Corporation


David McElfresh, Sun Microsystems


Timothy Strand, Agility Communications


CIRCUIT EDIT for FA, FI, AND DEBUG


Daniel Vacar, Sun Microsystems


Alan Street, Chair  Qualcomm, Inc.


PACKAGE LEVEL ANALYSIS


Marsha Abramo, IBM Systems & Technology


Rajen Dias, Co-Chair


Theodore Lundquist, Credence Systems


Antoniou Nicholas, Private Consultant


Ray Harrison, Co-Chair


Kendall S. Wills, DMTS Texas Instruments, Inc.


Texas Instruments, Inc.


France Aspera, Intel Corporation


DIE LEVEL FAULT ISOLATION


Craig Hillman, DFR Solutions


Felix Beaudoin, Chair


Robert Jemison, RJI Technical Sales


CNES-French Space Agency


David Maxwell, Texas Instruments, Inc.


Romain Desplats, CNES-French Space Agency


Peter Nguyen, Chip Targets Inc.


Gil Gartiez, Tower Semiconductor


Kartik Ramanujachar, Texas Instruments, Inc.


Robert Lamothe, R & L Technologies


Daniel Sullivan, LSI Logic Corporation


Martine Simard-Normandin, Muanalysis  Jian Tian, Credence Systems


POSTER


SYSTEM LEVEL ANALYSIS


Jerome Touzel, Infineon


Theodore Kolasa, Chair


Jeff Birdsley, Chair


Loren Vermont, Department of Defense


Freescale Semiconductor, Inc.


Dell Corporation


Joseph Buben, USA Defense Logistics Agency Roger Bjork, Dell Corporation


DISCRETES, PASSIVES, & MEMS


Jack Henderson, USA Navel Surface Warfare Robert Knoell, Visteon Corporation


David Burgass, Chair


Randal Mulder, Freescale Semiconductor Inc. Jeff Harsell, Dell Corporation


Accelerated Analysis


Richard Blanchard, SVEWG


David Su, Taiwan Semiconductor Manufacturing  Company, LTD.


Michael Lane, Intel Corporation


Roland Blanton, Carnegie Mellon University  Mahmood Choudhry, International Rectifier


Daren Slee, Exponent Failure Analysis  Association


Dominique Collard, IEMN


SAMPLE PREPARATION


Praveen Shenoy, Fairchild Semiconductor


Ronald Hylton, Chair


Jan Swart, Exponent Failure Analysis  Association


Maxim Integrated Products


FA PROCESS


Brennan Davis, Advanced MicroDevices


TEST


Christopher Richardson, Chair


Jerry Soden, Chair


LSI Logic Corporation


Raymond Haythronthwaite, Semiconductor   Insights


Richard McClelland, Philips Semiconductors, Inc.


Michael Santana, Advanced MicroDevices


Robert Aitken, ARM Ltd.


Kei-Wean Yang, Tektronix, Inc.


Anne Gattiker, IBM Corporation


Chuck Hawkins, University of New Mexico


Thomas Paquette, Insight Analytical Laboratories, Inc. SPM TECHNIQUES


Rene Segers, Philips Semiconductors, Inc.


Philip Kaszuba, Chair


Martin Versen, Infineon Technologies


METROLOGY & MATERIALS ANALYSIS


IBM Technology Group


Anjali Vij, Texas Instruments, Inc.


Bryan Tracy, Chair


Roger Alvis, MIcromagnetics Inc.


Spansion LLC


Terence Kane, IBM Technology Group


YIELD ENHANCEMENT


Ercan Adem, Spansion LLC


Leon Moszkowicz, IBM Technology Group


Carol Boyd, Chair


Roger Alvis, Multiprobe, Inc.


Benjamin Schrag, Micromagnetics Inc.


IBM Systems and Technology Group


William Vanderline, Lab.for Physical Sciences Alfredo Herrera, Advanced MicroDevices


NANOTECHNOLOGY


Diana Mitro, Motorola


Oliver Patterson, Agere Systems


Thomas Taylor, Infineon Technologies


Zachary Levine, NIST


James Slinkman, Electronic Warfare Association


Paiboon Tangyunyong, Sandia National Laboratories


Chris Henderson, Sandia National  Laboratories


Org. Committee Symposium Chair


IN THE HEART OF TEXAS…


● Austin ranks in the top three "Best  Places for Business." (Forbes, 2003,


2004, 2005)


● Austin places first on the “Innovation  Index” – The top 10 places where ideas  happen. (Visa USA, 2004)


● Austin is one of the country’s top


technology cities, boasting more than  1,000 tech companies.


● Austin is headquarters for Dell


Computer Corporation and major


operations for IBM, Samsung,


Motorola, and Advanced Micro Devices. ● Austin’s University Of Texas is one of  the largest public universities in the


U.S. with nearly 50,000 students.


The 32nd International Symposium


ISTFA/2006


for Testing and Failure Analysis


November 12-16, 2006


Sponsored by:  EDFAS


Renaissance Austin Hotel • Austin, TX


Electronic Device Failure Analysis Society


FIRST ANNOUNCEMENT  AND CALL FOR PAPERS


This is your opportunity to participate in “THE PREMIERE EVENT”


for the Microelectronics Failure Analysis community.  We


encourage you to submit an abstract for potential inclusion in the


ISTFA 2006 Symposium.


ISTFA solicits original, previously unpublished papers on a wide


range of Testing and Failure Analysis topics of practical value to


anyone working to detect, understand and eliminate


microelectronic device and system failures.  Instructive case


studies, review papers, and root-cause analyses are


encouraged. Non-commercial papers from equipment vendors


dealing with new or unique tools and methodologies,


applications and results are welcome.  Papers will be selected


for inclusion in the technical program based on four factors:


novelty, completeness, quality, and benefit to the FA community.


Paper acceptance will be based entirely on the information


included in the extended abstract submission.


We are currently seeking abstracts on (but not limited to) the following relevant topics*


|Advanced Techniques |MEMS |Optoelectronic Devices |System Level Analysis |
|---|---|---|---|

|Circuit Edit for FA, FI, & Debug |Metrology & Materials Analysis |Package Level Analysis |Test |

|Die Level Fault Isolation |Nanotechnology Analysis |Sample Preparation |Yield Enhancement |

|Failure Analysis Process |Optical Techniques |SPM Techniques ||

AND… Any Other Topics Related to Testing and/or Failure Analysis


*For topic descriptions and pertinent information regarding abstract submission, please visit the ISTFA website at www.edfas.org/istfa.


CALL FOR PAPERS DEADLINE  April 3, 2006


Abstract Submission:


Only abstracts in English will be considered.  The abstract must be at least two pages, including representative  images, figures and references.  It is highly advisable to include sufficient detail to allow for fair evaluation of the  work discussed.  During the online abstract submission process, complete contact information for all co-authors, and biographical information for the presenting author will be required.  Submit your abstract online at  www.edfas.org/istfa on or before the submission deadline of April 3, 2006.


Manuscript and Presentation Submission:


All authors accepted into the ISTFA 2006 Symposium are required to electronically submit a full manuscript and  presentation. Pre-approval to present your work is highly recommended to ensure on-time submissions. All costs  associated with your participation at ISTFA are at your expense (included a discounted registration fee).


For inquiries or information on ISTFA 2006, you may contact: ASM International Customer Service, Materials


Park, Ohio 44073-0002 440.338.5151, or visit the web at www.edfas.org/istfa.


Contents


Session 1: Advanced Techniques 1


Diffractive Lenses for High Resolution Laser Based Failure Analysis…………………………………1             F. Zachariasse1, M. J. Goossens2, (1)Philips Semiconductors, Nijmegen, Netherlands; (2)Philips Research, Eindhoven, Netherlands


Dopant Region Imaging on Front Surface of Silicon Devices   Using a Coaxial Photon-Ion Column………………………………………………………………….….8           R. G. Pajak1, F. A. Baiocchi1, E. Le Roy2, (1)Agere Systems, Allentown, PA, USA; (2)Credence Systems Corp., Sunnyvale, CA, USA


Newly Developed Scanning Laser-SQUID Microscope………………………………………………..14            K. Nikawa, T. Sakai, NEC Electronics, Kawasaki, Japan


Session 2: Package Level Analysis 1


Stacked-Die Failure Mechanisms for an Octal, Current Input 20-Bit


Analog-to-Digital Converter…………………………………………………………………………..…21


B.K. Craigin, B.L. Zhou, J.R. Bridgmon, Texas Instruments Tucson Corporation,                                     Tucson, AZ, USA


Silver-on-Silver versus Tin-on-Silver Electrical Connectors for High Current and


High Vibration Applications……………………………………………………………………….……27


P. Singh1, J. Lloyd2, J. Demarest1, L. Palmer1, L. Fischer1, G. Hutt, G. Thompson, W. Brodsky1,             (1)IBM, Poughkeepsie, NY, USA; (2)IBM T. J. Watson Research, Yorktown Heights, NY, USA


Analysis of Al-over-Cu Bond Pad Hillock and Pit Hole Defects………………………………………31


D. Cavasin, A. Yassine, Advanced Micro Devices, Austin, TX, USA


Die Edge Thin Film Delamination on the Bottom Die of a


Stacked Chip Scale Package (SCSP)…………………………………………………………………....37


L. De la Rama, D. Nuarin, M. Nery, Intel Philippines Technology Philippines, Cavite, Philippines


Session 3: Die Level Fault Isolation


Multi-Point Probing on 65nm Silicon Technology using Static IREM-based Methodology………..40


D. R. Bockelman, S. Y. C. Chen, A. Rahman, I. Wan, S. M. Ettinger, Intel Corporation,                       Hillsboro, OR, USA


Failure Analysis of Soft Single Column Failure in Advanced Nano SRAM Device with Internal  Probing Techniques……………………………………………………………………………………....46   H. S. Lin, W. T. Chang, C. H. Chao, J. Wang, C. T. Lin, C. Lin,


UMC, Hsin-Chu City, Taiwan, ROC


The Effectiveness of OBIRCH Based Fault Isolation for Sub-90 nm CMOS Technologies………....49                        M. De la Bardonnie1, K. Ly2, R. Ross2, F. Lorut3, M. Lamy3, C. Wyon4, L. Kwakman1, Y. Hiruma5, J. Roux6, (1)Philips Semiconductors, Crolles, France, (2)Freescale Semiconductor, Crolles, France, (3)ST Microelectronics, Crolles, France, (4)CEA-LETI, Grenoble, France, (5)Hamamatsu  Photonics K. K., Hamamatsu city, Japan, (6)Hamamatsu France, Meylan, France   Dislocation Related Leakage in Advanced CMOS Devices……………………………………………59                         F. Siegelin, A. Stuffer, Infineon Technologies AG, Munich, Germany


Session 6: Circuit Edit for FA, FI, and Debug


Contacting Diffusion with FIB for Backside Circuit Edit —Procedures and Material  Analysis………………………………………………………………………………………………...….64                     U. Kerst1, P. Sadewater1, R. Schlangen1, C. Boit1, R. Leinkauf2, B. Simmnacher3, T. Lundquist4, E. LeRoy4, (1)TUB Berlin University of Technology, Berlin, Germany; (2)HMI Hahn Institut Berlin, Berlin, Germany; (3)Infineon Technologies, Munich, Germany; (4) Credence Systems  Corporation, Milipitas, CA, USA


Novel and Practical Method of Through Silicon FIB Editing of SOI Devices……………………......70                         R.K. Jain, T.R. Lundquist, M.E. Antolik, M.A. Thompson, Credence Systems Corporation, Sunnyvale, CA, USA


The Joy of SOI: As Viewed from a Backside FIB Perspective……………………………………...…78                         S. Herschbein, C. Rue, C. Scrudato, IBM Systems & Technology, Hopewell Junction, NY, USA


Session 7: Case Histories 1


Complementary Optical Techniques for Advanced IC Failure Analysis – Case Study………...……84                        J.Y. Liao1, H.L. Marks1, H. Deslandes2, (1)NVIDIA, Santa Clara, CA, USA; (2)Credence Systems  Corporation, Milpitas, CA, USA


Scanning Optical Microscopy Application in Micron® Memory Devices………………………….....90                         W.Y. Yuan, T.L.E. Poh, D. Lam, Micron Semiconductor Asia Pte. Ltd.,


Singapore, Singapore


Topside Defect Localization Using OBIRCH Analysis……………………………………………...…95                         C. Howard, A. Weerakoon, D. M. Mitro, D. Glaeser, Freescale Semiconductor, Inc.,  Austin, TX, USA


Advanced Electrical Characterization of 90 nm Soft Bit Failure by


Nano Probing Technique…………………………………………………………………………...…..101


C. Giret, D. Faure, Texas Instruments France, Villeneuve Loubet, France


Session 8: Optical Techniques 1


Dynamic Laser Delay Variation Mapping (DVM) Implementations and Applications………...….106


K. Sanchez1, R. Desplats1, F. Beaudoin2, P. Perdu1, S. Dudit3, G. Woods4, D. Lewis5; (1)CNES - French Space Agency, Toulouse, France; (2)THALES SECURITY SYSTEMS, Toulouse, France, (3)ST Microelectronics, Crolles cedex, France; (4) CREDENCE—DCG, Sunnyvale, CA, USA; (5) IXL, Université de Bordeaux, Talence, France


Soft Defect Localization Techniques without a Synchronization Signal to the Laser Scanning


Module………………………………………………………………………………………………..….115


D.M. Mitro, D. Glaeser, C. Howard, Freescale Semiconductor, Inc., Austin, TX, USA


Guideline for Interpreting IR Laser Stimulation Signal on Semiconductors for


Materials and for Improving Failure Analysis Flow……………………………………………...…..121


A. Firiti1, G. Haller1, F. Beaudoin2, P. Perdu3, D. Lewis4, P. Fouillat4, (1)ST Microelectronics, Rousset, France, (2)THALES Microelectronics, Toulouse Cedex 9, France, (3)CNES-French  Space Agency, 31401 Toulouse Cedex 9, France, (4)IXL laboratory, Talence, France


Lock-In Assisted Soft Defect Localization (LIA-SDL) and Its Application in


Scan Shift Problems……………………………………………………………………………………..128


C. Brillert, Z. Qian, C. Burmer, M. Grützner, Infineon Technologies AG, Munich, Germany


Session 9: System Level Analysis 1


Furthering the Business Proposition of a Robust System Level Failure Analysis Framework:


A Focus on Enabling Product Services……………………………………………………………...…135


R. Bjork, Dell, Round Rock, TX, USA


Unique Failure Modes from use of Sn-Pb and Lead-Free (mixed metallurgies) in


PCB Assembly: Case Study…………………………………………………………………………….140


F. Toth, G.F. Shade, Intel Corporation, Hillsboro, OR, USA


Analysis Methods for Characterizing Drop Test Robustness of Lead-Free FBGAs………………..145


J. Walter, R. Fischer, C. Birzer, Infineon Technologies AG, Regensburg, Germany


Developing a More Inclusive System Level ESD Characterization Methodology…………………..151


J. Rahardjo, S. Miller, L. Lopez, S.L. Williams, Dell Inc., Round Rock, TX, USA


Session 10: Advanced Techniques 2


X-ray Fluorescence Imaging for High Resolution Elemental Mapping…………………………..…158


M. Feser, W. Yun, A. Lyon, Y. Wang, S. Sehadri, Xradia Inc., Concord, CA, USA


3-D EBIC Technique using FIB and EB Double Beam System……………………………………...163


E. Yoshida, T. Tanaka, T. Oyamada, T. Koyama, J. Komori, S. Maegawa,  Renesas Technology Corp., Itami, Hyogo, Japan


Analysis of a Microcircuit Failure using SQUID and MR Current Imaging……………………….169


F.S. Felt, NASA Goddard Space Flight Center, Greenbelt, MD, USA


Session 11: Case Histories 2


Case Studies of the Use of Image Processing in Metrology and Failure Analysis…………………..178


K. Ramanujachar, Texas Instruments, Stafford, TX, USA


Single Device Characterization by Nano-probing to Identify Failure Root Cause…………………183


C.C. Wu, J.C. Lee, J.H. Chuang, T.T. Li, Taiwan Semiconductor Manufacturing Company, Ltd., Hsin-Chu City, Taiwan, ROC


Analysis of DRAM Standby Current Failure due to Hot Electron Induced


Punch-through (HEIP) of PMOStransistor……………………………………………..…………….186


M.H. Cho, Y.I. Kim, J. Choi, D.S. Woo, K.P. Lee, Y.J. Park, W.S. Lee, B.I. Ryu,  Samsung Electronics. Co. Ltd., Hwasung-City, Gyeonggi-Do, South Korea


Session 12: Poster


Stacked Die Analysis Using C-mode Scanning Acoustic Microscope…………………………..……189


L. Na, J. Khan, L. Adams, National Semiconductor Corporation, Santa Clara, CA, USA


DuPont EKC265TM as a Copper Metal Etchant to Assist FIB Edits through


Large Copper Power Supply Lines………………………………………………………………...…..194


R.E. Mulder, Freescale Semiconductor, Austin, TX, USA


Edge Enhancement for Acoustic Microscopy of Flip Chip Devices………………………………….199


D.J.D. Sullivan, A.J. Komrowski, L.A. Curiel, K.V. Tan, LSI Logic, Fremont, CA, USA


Method of Failure Site Isolation for Flash Memory Device Using FIB, Passive Voltage


Contrast Techniques……………………………………………………………………………………202


C. Yuan, S. Li, A. Gray, Spansion LLC, Sunnyvale, CA, USA


Increasing Planarity for Failure Analysis Using Blocked Reactive Ion Etching


Combined with Planar Polish…………………………………………………………………………..206


M.E. Weldy1, L. Serrano2, (1)Intel Corporation, Folsom, CA, USA; (2)Intel Corporation,  Santa Clara, CA, USA


Nanomechanical Characterization in the FIB………………………………………………………...209


T. Moore, Omniprobe, Inc., Dallas, TX, USA


Couple Passive Voltage Contrast with Scanning Probe Microscope to


Identify Invisible Implant Issue………………………………………………………………………...212


C. -M. Shen, S. C. Lin, C. M. Huang, H. X. Lin, C. H. Wang, Taiwan Semiconductor   Manufacture Company, Ltd., Tainan, Taiwan, ROC


CAD - Less Blind Navigation in Focused Ion Beam System………………………………………….217


V. Ray, Particle Beam Systes & Technology, Methuen, MA, USA  G. Gerlinsky, Titus Consulting, Saskatoon, Canada


Method of Detecting Trace Metal Contamination in Thick-Film SOI Device………………………220


Y. Goto1, M. Iida2, H. Eguchi1, (1)Toyota Motor Corporation, Aichi, Japan, (2)Japan Tecseed  Corporation, Aichi, Japan


The Radio ProbeTM: A New Measurement Tool for High Speed Integrated Circuits…………...…224


M. Kimball, Maxim Integrated Products, Beaverton, OR, USA


High Resolution Acoustic Microscopy with Low Frequency and Its Applications in


Analysis of Ferroelectrics…………………………………………………………………………...…..228


Q.R. Yin, H.F. Yu, H.R. Zeng, G.R. Li, A.L. Ding, Shanghai Institute of Ceramics,  Chinese Academy of Sciences, Shanghai, China


Automated Sample Preparation of Low-k Dielectrics for FESEM…………………………………..231


R.R. Cerchiara1, H.A. Cook, P.E. Fischione1, A.C. Robins1, D.W. Smith1, J.J. Gronsky1, J.M.


Matesa1, S.J. Rozeveld2, C.J. Wood2, E.R. Beach2, J. Waeterloos2, (1)E. A. Fischione Instruments, Inc., Export, PA, USA; (2)The Dow Chemical Company, Midland, MI, USA


Depth Measurement of Dislocations in Si Substrate by Stereo TEM………………………………..233


J.S. Bow, S. Yu, UMC, Tainan County, Taiwan, ROC


Gate Oxide Defect Localization and Analysis by Using Conductive


Atomic Force Microscopy……………………………………………………………………………....235


Z.H. Lee, C.J. Lin, S.W. Lai, J.H. Chou, Taiwan Semiconductor Manufacture Company, Ltd., Taiwan, Shan-Hua Tainan, Taiwan, ROC


A Novel Method to Observe the Silicide in TEM………………………………………………….…..239


P. Liu, Semiconductor Manufacturing International (Beijing) Corp., Beijing, China


The Enhancement of Abnormal Photon Emission Identification for Advanced


Processes using a Backside Cooling PEM System………………………………………………...…..241


C.H. Wang, S.W. Lai, Z.H. Lee, J.H. Chou, Taiwan Semiconductor Manufacture Company, Ltd., Taiwan, Tainan, Taiwan, ROC


Dynamic Electroluminescence Imaging (DEI) as an “Optical Oscilloscope” Probe………………..245


J. Hulse1, K. Sarault2, M. Simard-Normandin2, (1)National Research Council of Canada,  Ottawa, ON, Canada, (2)MuAnalysis Inc., Ottawa, ON, Canada


Thermal Imaging Product Power-up: Metrology for Capturing Thermal Defects on


Live Units Not Visible on Any Other Technique………………………………………………….…..249


N.T. Zamora, K.M. Chong, A. Gupta, Intel Technology Phils., Cavite, Philippines;


Intel Technology Sdn. Blvd., Penang, Malaysia; Intel Corporation, Chandler, AZ, USA


Single Via Deprocessing Techniques to Enable Physical Analysis for


Semiconductor Process Integration……………………………………………………………………253


J.E. Hammett, W. Qin, D. Theodore, Freescale Semiconductor Inc., Chandler, AZ, USA


EEPROM Failure Analysis Methodology : Can Programmed Charges be Measured


Directly by Electrical Techniques of Scanning Probe Microscopy (SPM)?.......................................256


C. De Nardi1, R. Desplats1, P. Perdu2, F. Beaudoin3, J. L. Gauffier4, (1)CNES-French Space  Agency, Toulouse, France, (2)CNES-French Space Agency, 31401 Toulouse Cedex 9, France, (3)THALES Security System, Toulouse Cedex 9, France, (4)Institut National des Sciences


Aplliquées (INSA), Toulouse, France


Stacked Polysilicon/Metal Capacitors Failure Analysis……………………………………………..262


D.T. Nguyen1, F. Huang2, (1)Texas Intruments Corp, Dallas, TX, USA; (2)Texas Instrument, Dallas, Texas, TX, USA


The Microstructure Evolution of Corrosion Phenomenon on Aluminum Bond Pads…………….266


J.S. Luo, H.M. Lo, J.D. Russell, Inotera Memories Inc., Taoyuan, Taiwan, ROC


Session 13: Failure Analysis Process


Studies on A Failure Analysis Flow of Surface Contamination, Corrosion, and Underetch on


Microchip Al Bondpads in Wafer Fabrication………………………………………………………..274


H. Younan, Chartered Semiconductor Mfg Ltd, Singapore, Singapore


Root Cause Analyses of Metal Bridging for Copper Damascene Process…………………………..283


Z.G. Song, S.P. Neo, S.K. Loh, C.K. Oh, Chartered Semiconductor Mfg Ltd, Singapore, Singapore


Strategies for the Analysis of Single Unit Failures in Low Failure Rate Applications……………..287


T. Kolasa, J. Kopycinski, A. Mendoza, Freescale Semiconductor, Tempe, AZ, USA


Failure Analysis Techniques for Lead-Free Solder Joints……………………………………………295


T. Castello1, D. Rooney1, D. Shangguan2, (1)Flextronics, Youngsville, NC, USA; (2)Flextronics, San Jose, CA, USA


Session 14: SPM Techniques 1


Transmission Electron Microscopy and Scanning Capacitance Microscopy


Analysis of Dislocation-Induced Leakages in n-channel I/O Transistors……………………………302


M.L. Anderson, P. Tangyunyong, T.A. Hill, C.Y. Nakakura, T.J. Headley, M.J. Rye, Sandia  National Laboratories, Albuquerque, NM, USA


Scanning Capacitance Microscopy Application for Bipolar and CMOS Doping Issues in


Semiconductor Failure Analysis………………………………………………………………………..307


C. Lin1, H. Ou 734491, C.H. Chao. 332201, S.S. Lu2, (1)No.3 Li-Hsin Rd. II , Science-Based


Industrial Park, Hsin-Chu City, Taiwan, ROC; (2)National Taiwan University, Taipei, Taiwan, ROC


Atomic Force Probing in Analog MOSFETs Measurement………………………………………….311


K. Chen, T. Chattergee, K. Christensen, J. Rosal, H. Edwards, Texas Instrumenst, Inc.,  Dallas, TX, USA


Session 15: Sample Preparation 1


Improvement of Electrical Contacts in the Failure Analysis for in-depth Characterization of


Structures and Products………………………………………………………………………………...316


M. Huettinger, J. Touzel, Infineon Technologies AG, Munich, Germany


The Versatile Application for In-situ Lift-out TEM Sample Preparation by


Micromanipulator and Nanomotor………………………………………………………………….…322


J.C. Lee, B.H. Lee, Taiwan Semiconductor Manufacturing Company, Ltd., Hsin-Chu City,  Taiwan, ROC


Failure Analysis of Electronic and Microelectronic Components with a


New Automatic Target Preparation System…………………………………………………………..327


K. Reiter1, H. Bundgaard2, (1)Fraunhofer Institute of Silicon Technology, Itzehoe, Germany, (2)Struers A/S, Ballerup, Denmark


Investigation of Passivation Damage from the Backside……………………………………………..332


S. Subramanian, E. Widener, T. Chrastecky, B.W. Jones, D. Jones, R. Mulder, Freescale  Semiconductor, Inc., Austin, TX, USA


Session 16: Optoelectronic Devices


An Atlas of ESD Failure Signatures in Vertical Cavity Surface Emitting Lasers………………..…336


D.T. Mathes, J. Guenter, B. Hawkins, B. Hawthorne, C. Johnson, Advanced Optical Components, Richardson, TX, USA


3-D Defect Characterization using Plan View and Cross-Sectional TEM/STEM Analysis………..344


T.J. Stark1, P.E. Russell2, C. Nevers3, (1)Materials Analytical Services, Raleigh, NC, USA; (2)North Carolina State University, Raleigh, NC, USA; (3)TriQuint Semiconductor,


Hillsboro, OR, USA


Physics of Failure Investigation of Dark VCSEL Devices: Detection of Reverse-Bias


Electroluminescence by Emission Microscopy…………………………………………………….….350


D.K. McElfresh, L.D. Lopez, R. Melanson, D. Vacar, Sun Microsystems Inc., San Diego, CA, USA


Session 17: Optical Techniques 2


Advanced Optical Testing of an Array in 65 nm CMOS Technology……………………………….355


F. Stellari1, P. Song1, T.A. Christensen2, (1)IBM Research, Yorktown Heights, NY, USA; (2)IBM, Rochester, MN, USA


Analog Circuit Failure Analysis Using Time-Resolved Emission……………………………………363


B.J. Cain1, G.L. Woods1, R. Herlein2, A. Syed1, T. Nomura3, (1)Credence Systems Corp,


Sunnyvale, CA, USA; (2)Credence Systems Corp, San Jose, CA, USA; (3)Credence Systems Corp, Kawasaki-shi,Kanagawa-ken, Japan


Session 18: Nanotechnology Analysis


X-Ray Nanoanalysis in the SEM………………………………………………………………………370


W.E. Vanderlinde1, D. Chernoff2, (1)Laboratory for Physical Sciences, College Park, MD, USA; (2)Small World LLC, Vienna, VA, USA


Kinematical Simulation of HOLZ Pattern for Uniaxial Strain Determination……………………..380


T.H. Chen, J.-S. Bow, UMC, Hsinchu, Taiwan, ROC


3D Observation of Elemental Distribution of Si-Device using a Dedicated FIB/STEM System…...382


T. Yaguchi1, M. Konno1, T. Kamino1, M. Ogasawara2, K. Kaji2, T. Ohnishi2, M. Watanabe3,


(1)Hitachi High-Technologies corporation, Hitachinaka-shi, Japan, (2)Hitachi High-Technologies  Corporation, Hitachinaka, Japan, (3)Lehigh University, Bethlehem, PA, USA


Session 19: Yield Enhancement


Burn-In Acceleration Considerations in 130nm and 90nm Products…………………………….….389


N. Wakai, Y. Kobira, T. Setoya, Toshiba Corporation, Yokohama, Japan  T. Oishi, S. Yamasati, Toshiba Corporation, Oita, Japan


Statistical Evaluation of Scan Test Diagnosis Results for Yield Enhancement of


Logic Designs…………………………………………………………………………………………....395


C. Burmer, H.-P. Erb, A. Leininger, M. Gruetzner, T. Schweinboeck, S. Trost,  Infineon Technologies, Munich, Germany


In-Line Voltage Contrast Inspection of Ungrounded Chain Test Structures for


Timely and Detailed Characterization of Contact and Via Yield Loss…………………………..….401


O.D. Patterson1, H. Wildman1, A. Ache1, K. Wu2, (1)IBM Corporation, Hopewell Junction,  NY, USA (2)KLA-Tencor, Hopewell Junction, NY, USA


E-BeamMagSpotTiltDetFWD04/29/05


20 μm


500kw1.50 kx352.0CDM-E4.998161852D115 R100K1 No2


Figure 7.  SEM image of the pattern of a lens after  implantation. At this point the silicon surface is still flat.


The plasma process after implantatation used CF4/O2 to  anisotropically etch silicon with an etch rate of 100 nm/min.  The etcher was a Unaxis Nextral NE860 which combines RF  parallel plate excitation with microwave excitation to achieve, simultaneously, a high plasma density, low pressure, and low


E-BeamMagSpotTiltDetFWD05/03/05


2μm


self bias of around 20V.  An etch time of 2 minutes was used,


5.00kV20.0 kX352.0CDM-E597612:13:07


and the depth achieved was approximately 200 nm.


Figure 8 shows an SEM image of the same diffractive lens  after plasma etching.  The surface is no longer flat but consists  of a series of concentric rings that form alternating high and


low regions on the silicon substrate.  A close-up is shown in  Fig. 9.


Optical performance


The lens shown in Fig. 8 has a 200 µm diameter and was  fabricated on a silicon IC made in a 0.12 µm CMOS  technology.  The die thickness was 115 µm, and the lens was  designed for use with a 1340 nm laser.  From geometrical  considerations, the rays travelling from the edge of the lens to  the focal point make a semi-angle of 41 degrees to the optical  axis, resulting in an effective NA of 2.3 for this lens.  The  diffraction-limited resolution is then 360 nm according to  equation (1).


09熊


5ODkV1.50 kX352 0CDM-E6.00612:0732 E-BeamMagSpotTiltDetFWD05/03/05


Figure 8.  SEM image of a diffractive lens, fabricated on the  back side of the silicon substrate of an IC.


Figure 9. Enlarged view of the lens of Fig.8, showing  concentric high areas (marked 1 and 3 for example) and low  areas (2 and 4,  for example).


1


2


3 4


4


Figure 10. Left : Circuit without diffractive lens; Right : Same area with diffractive lens.  Images were taken on a Hamamatsu Phemos  1000 laser scanning microscope, with a 100x, 0.7 NA NIR objective, and 1340 nm laser.  The stripes in the right hand image are  polysilicon gates of 0.12 µm.  The box marks gates at 0.5 µm pitch.  The arrow marks gates at 350 nm pitch.


Figure 10 shows a laser scanning confocal microscope image  of the circuit area underneath the lens.  On the left is the image  of the circuit without the diffractive lens in the optical path, and on the right, the same area in the circuit now with the  diffractive lens.  The images have been scaled and cropped to  show the same area.   The logic gates in the circuit show active  areas with polysilicon gates showing up dark.  Since gates with  500 nm pitch are clearly resolved while those with 350 nm  pitch are not, it is estimated that the lens approaches its  theoretical diffraction limit in this case.


Although no direct measurements were made, the throughput  efficiency, judged from the level of laser power needed to  obtain an image, was estimated at 10-20 % for this lens. We  are currently improving this efficiency by tuning the etch  process to obtain the target profile depth and by developing  multilevel lenses instead of binary ones. This will be especially  valuable for analyses requiring relatively high laser power at  the focal plane.


Designs with selectable focal length


Although the lens of Fig. 3 is designed so that its focus is at  the centre of a spherical wave front incident on the silicon (the  equivalent, in diffractive optics, of a hemispherical SIL), it is  also possible to design lenses with a different focal length [6].  In that case, rays entering the silicon do not continue straight


as in the hemispherical case.  For example, Fig. 11b shows a  lens with a focal length chosen such that position V of the  virtual image lies a distance 2d from the lens, where d is the  thickness of the silicon.  This provides a magnification of 2x  compared to the case of Fig. 11a, where both object and image  lie a distance d from the lens.


The resulting optical performance is shown in Fig. 12.  Here, 2  lenses of 160 µm diameter were formed in adjacent areas on a


0.12 µm technology die 270 µm thick.  Lens A is the  equivalent to the hemispherical design of Fig. 11a.  Lens B is  designed as shown in Fig. 11b. The design plots are shown  below the optical images.  Although both images were taken  with the same microscope objective, lens B gives twice the  magnification of lens A.  Both lenses have a diameter such that  the effective NA of the lenses is 0.99, so the theoretical  resolution limit is 825 nm for a 1340 nm laser.


Note from Figs. 10 and 12 that the useable field of view  through a diffractive lens appears to be between 15-20 % of  the silicon thickness.  For samples greater than 100 µm thick, this allows a lens positioning error of 5 µm without missing the  point of interest from the resulting view.


5µm


5


Figure 11. Schematic cross-section showing the paths of light rays incident on two diffractive lenses with different focal lengths.  Solid  lines mark the path of the light, and for lens B, the dotted lines show the position of the virtual image V.


B,my lit


FdeName dt


RendtomeinLaverScanaurnog


Dinte


Figure 12. Laser scanning microscope images of a 0.12 µm CMOS device through 2 different diffractive lenses.  The same microscope  objective was used to obtain both images.  Note that lens B has twice the magnification of that shown by lens A.  Lens B differs from A  in its construction only in the positions and sizes of the rings.


6820


A


B


和区


V


Silicon


d


Lens A


2d


Lens B


6


Conclusions and further work


We have shown that it is possible, in about 1 hour, to fabricate  on the back side of an IC a diffractive lens that increases the  imaging resolution of a laser scanning microscope by about a  factor 3.  The lens performance approaches diffraction limited  resolution, and can not only be fabricated using standard  equipment available in most failure analysis laboratories, but  also used together with any confocal laser scanning  microscope.  This concept offers significant advantages over  alternative methods of resolution increase, because it relaxes  constraints of package and die preparation for failure analysis, and can be designed to fit both the sample and optical system  at hand.


A significant limitation of the diffractive lens is its limited  throughput efficiency, which reduces the laser power delivered  to the focal plane.  Improvements to the throughput efficiency  and application to laser based fault localization methods are  currently under investigation.


Acknowledgments


We would like to thank Benno Hendriks, Arjan Mels, Wil  Ophey and Lingli Wang for valuable discussions.


References


[1] Rowlette, J.A and Eiles, T.M., “Critical timing analysis in  microprocessors using near-IR Laser assisted device  alteration (LADA)”, Proc. ITC, 2003, pp.264-273


[2] Bruce, M.  et al., “Soft defect localization on ICs”, Proc. ISTFA 2002, pp. 21-27


[3] Goruganthu, R.R. et al., “Spray Cooling for Time  Resolved Emission Measurements of ICs”, Proc. ISTFA  2004, pp. 18-23


[4] Koyama, T. et al., “High Resolution Backside Fault  Isolation Technique Using Directly Forming Si Substrate  into Solid Immersion Lens”, Proc. IRPS 2003, pp. 529-535


[5] Falk, R.A. “Optimizing Backside Image Quality”, Proc. ISTFA 2002, pp.156-161


[6] R.Brunner et al.,  “Diffraction-based solid immersion  lens”, J. Opt. Soc. Am. A, Vol. 21, No. 7, July 2004, p. 1186


[7] See for example M.Bass (Editor) “Handbook of Optics”,  Vol. 2, Chapter 8. McGraw-Hill, New York


[8] Zachariasse, F, and Walker, J.F.,   “Direct write patterning  of titanium films using focused ion beam implantation and  plasma etching”, Microelectronic Engineering Vol. 35,


(1997) pp. 63-66


7


Dopant Imaging on Front Surface of Silicon Devices with a  Coaxial Photon-Ion Column


Robert Pajak, Frank Baiocchi


Agere Systems, Allentown, PA


Erwan Le Roy


Credence Corporation, Milpitas, CA


Abstract


An n-well contrast enhancement process,


which is used for backside navigation has been  further developed to observe dopant regions on  top-down prepared devices.


Dopant regions for the following structures  were delineated:


p-active regions in n-wells;


n-active regions in p-wells;


n-well to p-well interface;


p+/p interface.


The enhancement process to obtain this  contrast was done on a Credence OptiFIB using a  coaxial FIB/optical column. Illumination of the  sample is a critical component of the process. First, the high contrast level obtained at a p/n  junction was only achieved by using light assisted  FIB oxide deposition. Second, sample  illumination was found to enhance contrast while  imaging the region of interest using the focused  ion beam. The contrast becomes permanent only  after the oxide is deposited.


Contrary to chemical etch techniques imaged  in a SEM, this enhancement process as well as the  imaging process were completed in-situ. Further, this process proved to be very reproducible.


This dopant contrast enhancement process  provides an alternative to wet chemical  delineation methods for the verification of dopant  photomask registration, for accomplishing reverse  engineering and for observing missing implants.


Introduction


The controlled introduction of dopants into  silicon is a fundamental part of semiconductor  device fabrication [1]. The electrical performance


of the various types of devices is ultimately  determined by the three dimensional distribution of  the dopants within the silicon.   However, unlike the  polysilicon or metal features that are patterned on  top of the silicon substrate, the dopant regions are  not easily imaged using standard optical or electron  microscopy techniques. The dopants are  incorporated within the silicon lattice at  concentrations of 0.1 to 0.000001 atomic %, which  makes it difficult to detect any difference in the  structure of the silicon related to dopant  concentration.


Given their importance, much work has been  done to develop experimental and theoretical  methods for characterizing dopant distributions in  silicon devices.  The one-dimensional diffusion of


|the common dopants, arsenic, phosphorous, and |the common dopants, arsenic, phosphorous, and |the common dopants, arsenic, phosphorous, and |
|---|---|---|

|boron, in |silicon have been |extensively |

|characterized spectrometry |using secondary ion (SIMS) [2] and spreading resistance |mass |

profiling (SRP) [3],  and this experimental data has  provided the basis for modeling of dopant profiles  in device simulators.  Two dimensional diffusion  profiles of actual transistor scale dopant regions are  harder to characterize [4]. These experiments  require a site specific cross section of the silicon  through the doped region of interest, followed by an  analysis of the dopant distribution on the two  dimensional surface of the cross section.  Given the  small lateral size of a typical transistor region (~several microns), and the very shallow depth from  the silicon surface of the diffused region (~0.3  microns), specialized analysis techniques with  nanometer spatial resolution and part per million  sensitivity to dopant concentrations are required.


8


Copyright ©2005 ASM International


Proceedings of the 31   International Symposium for Testing and Failure Analysis


November 6–10, 2005, McEnery Convention Center, San Jose, California, USA


# Dopant Imaging on Front Surface of Silicon Devices with a Coaxial Photon- Ion Column


st


®


Electron or scanning probe microscopy methods  can provide the required spatial resolution.  In  particular, scanning electron microscopy (SEM) has been widely used as an imaging tool, and  passive voltage contrast in the SEM has been  shown to provide useful doping information [5,6]. The sensitivity to dopant concentrations can be  further enhanced by a variety of techniques which  fall into either of two basic methods involving  chemical or electrical interaction with the sample. Chemical interactions with the sample, which  includes a wide variety of etching [7, 8, 9, 10] or  staining [11] methods, depends on etch rate or  film deposition rate changes with dopant type and  concentration. There are many types of recipes  used with many variations in each lab. Typical  chemical etching of doped regions involves a  combination of an oxidizer, such as nitric or  chromic acid, with an etch for silicon dioxide, such as hydrofluoric acid.  Electrical interaction  with the sample depends on change in resistance  or capacitance in the silicon with dopant type and  concentration.  The modification of atomic force  microscopes to measure capacitance (scanning  capacitance microscopy, SCM [12,13]) or  resistance (nano spreading resistance profiling, nSRP [14]) has provided useful methods for twodimensional dopant profiling, either on a silicon  cross section surface or on the top surface of the  silicon substrate.


In addition to fundamental measurements of  doping profiles for device modeling and  development, characterization of dopants is  important for the failure analysis community as  well.   The same processing defects that can affect  visible structures like poly gates or metal  interconnects, can impact the various dopant  levels.  For example, photoresist issues such as no  pattern wafers, misalignment, or extra resist  features can change the intended implant pattern  across the wafer or in specific transistors within  one die.  Since no visible structure is left behind  on the silicon die, it is difficult to determine the  root cause of the failure.  Typical methods that  may provide insight into such defects prior to


deprocessing the device include photon emission  microscopy (PEM), passive voltage contrast in a  SEM, or electron beam induced current (EBIC) in a  SEM.  After deprocessing the die, with all layers  removed down to the silicon substrate, the analyst  depends on chemical methods [7-11] to etch or stain  the silicon in the hopes of delineating the dopant  regions.  Since many methods exist for different  dopant types, if the correct one is not chosen at the  start, it may be difficult to try alternate methods due  to the destructive nature of this analysis.  Depending on the chemical mixture used as the  etchant, the top 0.2 microns of the silicon substrate  can be etched away in seconds.  The analyst usually  must optimize the method using extra samples prior  to working with the actual device of interest.


In this paper, a new technique for characterizing  dopant regions in silicon using a focused ion beam (FIB) tool is presented. This technique builds on  previous work for backside FIB navigation, in  which n-well contrast is observed, [15].  The  present work demonstrates that the technique, although not fully understood, can distinguish both  n and p type dopant regions.  We also show the  sensitivity of the method to various dopant  concentrations using characterization wafers  prepared with known dopant levels ranging from  1017cm-3 to ~1020cm-3.  Finally, the resolution of the  method for imaging real transistor dopant regions  on current fabricated devices was demonstrated.   The method provides a complementary alternative  to the chemical and electrical methods currently  available.


Device preparation:


A 130nm silicon device was mechanically  polished and chemically stripped of metal and  dielectric layers down to the silicon substrate. The  enhancement process described in [15] was  followed: the native oxide was removed using XeF2  for a few seconds. A FIB generated oxide was then  deposited on the doped regions; its thickness was  130nm.  Several dopant regions were revealed (Figure 1 and 2).


9


Figure 1 - FIB image at 6nA before process was  applied


Figure 2 - FIB image at 6nA after process was  applied


→ Dopant characterization on a top-down  non-prepared device:


Compared to backside processing, the front side  of the sample does contain topography associated  with various thick oxide features used for active  area isolation. This surface topography adds  additional contrast information. There is no clear  dopant contrast that can be observed.


→ Dopant characterization on a top-down  prepared device:


On the treated device the n-well regions  appeared white relative to p-wells (Figure 3). This  contrast difference is consistent with the n-well/pwell contrast reported during backside FIB  processing [15]. Further detailed observation of the  active diffusion regions within the wells reveals  interesting contrast changes.  The p-active regions  within the n-well appear brighter than the  surrounding n-well. On the other hand, the n-active  regions within the p-well appear darker than the  surrounding p-well, as observed in Figure 3.


Compared to backside processing, the front side  of the sample does contain topography associated  with various thick oxide features used for active  area isolation. This surface topography adds  additional contrast information. However, observation of wider active regions where edge  effects are not the dominant contrast mechanism  still shows that the p-active regions are brighter than  the surrounding n-wells and n-active regions are  darker than the surrounding p-wells.


These doping profiles can be more easily  observed by simply reversing the brightness level  using any imaging software brightness reverse  function. (Figure 4).


Treated area


Non-treated area


p-well


n-well


p-active


Fig 3 – FIB image with doping profiles


highlighting n/p-wells and p-actives. Field of  View = 20*20um2


10


n-active


Fig 4 – FIB image with brightness reversed  image showing active-regions. Field of View = 20*20um2


Characterization:


In order to characterize this phenomenon, the  contrast was studied on target silicon wafers  prepared with a simple n type implant pattern within  a p-type blanket silicon layer.  The n dopant regions  varied in concentration from ~10^17cm-3 to ~10^20cm-3. The implant depth for each sample was  approximately 300nm (Fig 5).


◆120keV As implant


Fig 5 – Implantation depth for target silicon  wafer


A sample with highly doped p+ regions in a p  substrate was also imaged.  These samples have no  other processed features other than the implanted  regions, eliminating any surface topography effects.


The observed contrast for p/n junctions with low  doping concentrations appears to be directly  influenced by the presence of light during the  imaging process with a Focused Ion Beam (figure 6  and 7).


FIB deposited oxide


Trench


n-well p-well


7.1*10^16 cm-3


6.0*10^17 cm-3


Fig 6– FIB image of n-wells and p-wells with  light ON


1.00E+20


1.00E+19


1.00E+17


3


u


0


31.00E+16


***


1.00E+15


***.......*...*****


1.00E+14


81.00E+18十


Fig 7 – FIB image of n-wells and p-wells with  light OFF


For the highly doped sample, the contrast  appeared weaker (figure 8). The light did not have  any influence on the contrast.


100um


0 0.1 0.2 0.3 0.4 0.5 0.6 0.7 0.8 0.9 1 micron


11


9.3 10^19cm-3


7.1 10^18cm-3


p-type n-type FIB deposited oxide


20.0kV 11.8mmx600SE(U)216/05 11:03


Fig 8 – FIB image of n-active regions (9.3


10^19cm-3) in highly doped p (7.1 10^18cm-3)  (light


OFF and light ON have the same contrast)


SEM and FIB comparison


For comparison, the same area of the chip  shown in figure 1 was treated using the FIB contrast  recipe. It was then imaged using a scanning electron  microscope (SEM). On the treated and the untreated  devices, most of the contrast observed in the SEM  image appeared to be related to the topography (figure 9 and 10). There was no obvious contrast  related to the dopant type.


6OUSE


5.0kV 14.5mm x6.00k SE(U) 2/24/0503:09


5,00um'


Fig 9 – SEM area of the untreated region at  low mag


Fig 10 – SEM area of the treated region (oxide  deposited) at low mag


However, at higher magnification, a slight  contrast difference between the n-well and p-well  was observed which was found to correlate with the  FIB image (figure 11). The n/p well contrast was  found to be opposite to the one observed in the FIB.  In addition, there was no obvious contrast  difference related to the active regions within each  well. The contrast level is sharper with a focused  ion beam using simultaneous optical imaging (figure 2 and 3).


el


Fig 11 – SEM area of the treated region at high  mag (oxide deposited)


12


Conclusion


The technique described is the first FIB based  method revealing permanent dopant contrast on  both p/n junctions and p/p+ regions. The contrast  level can be up to 80% depending on the dopant  concentration. This contrast can be observed for a  range of dopant concentration from 10^16cm-3 to  10^20cm-3. This sensitivity matches the  Semiconductor Industry Association (SIA) requirements for the next device generation. This  method is easily reproducible and can be further  developed to quantify the dopant concentration. Both the recipe and the imaging can be done in the  same chamber using a coaxial ion/photon column; the total time is less than 3min for a 10*10um2 area. This innovative method provides a fast and  reliable approach for identifying mask  misregistration, obtain reverse engineering  information and observe missing implants.


References:


[1] VLSI Technology, 2nd edition, S.M.Sze, editor, McGraw-Hill, Inc., NY, page 272, 1988.


[2] W. Vandervorst and F.R.Shepherd, J. Vac. Sci. Technology A, 5, 313, 1987


[3] R.G.Mazur and D.Dickey, J. Electrochem. Soc. 113,  255 (1966)  (SRP reference)


[4] A.C.Diebold, M.Kump, J.J. Kopanski, and  D.G.Seiler, Proceedings of the 3rd International  Workshop on Measurement and Characterization of


Ultra-Shallow Doping Profiles in Semiconductors, page 2.1, 1995.


[5] C.Y. Lin, J.H. Lee, Proceedings 29th ISTFA, p.87 (2003).


[6] S.L.Elliott, R.F. Broom, C.J.Humphreys, J.Appl. Phys. 91, 9116, (2002).


[7] K.H.Yang, J. Electrochem. Soc., 131, 1140 (1984).


[8] C.W. Pearce, J. Electrochem. Soc, 128, 920 (1981).


[9] H. Robbins, J. Electrochem. Soc, 109, 63 (1962).


[10] D.M.Maher and B Zhang,  J. Vac. Sci. Technol. B12, 347, (1994)


[11] S.T.Ahn and W.A.Tiller, J. Electrochem. Soc. Solid State Sci and Tech, 135 No.9, 2370, (1988)


[12] G.Neubauer et al., J. Vac. Sci. Technol. B14, 426 (1996).


[13] K. Jarausch, J.F. Richard, L. Denney, A. Guichard, P. Russell, Proceedings 28th ISTFA, p.471 (2002).


[14] P.Dewolf, T.Clarysse, W.Vandervorst, J.Snauwaert, and L. Hellemans, Proceedings of the  3rd International Workshop on Measurement and  Characterization of Ultra-Shallow Doping Profiles  in Semiconductors, page 32.1, 1995.


[15] E. Le Roy and M. Thompson Mat. Res. Soc. Symp. Proc. Vol.792 (2004)


13


Newly-Developed Scanning Laser-SQUID Microscope


K. Nikawa and S.Sakai


NEC Electronics Corporation, Kawasaki, Kanagawa, Japan  k.nikawa@necel.com, tetsuya.sakai@necel.com


The scanning laser-SQUID microscope can detect electrical


defects in a chip without requiring electrical contacts to the  chip. Using our new system, we can get magnetic flux images  of a 300mmφ wafer in air. Experiments with 256Mbit-DRAM  chips showed that IDDS testing results are correlated well with  laser-SQUID images, and that the spatial resolution is 0.59 µm in an intensity image, and 0.54 µm in a phase image. We  have also succeeded in localizing the open site in a whole chip  area of a 90nm-node logic IC chip.


In the field of failure analysis of ICs (integrated circuits), we  use emission microscopy, IR-OBIRCH (infrared opticalbeam-induced resistance change) methods, and electron beam  testing for localizing electrical defects nondestructively. These  methods, however, require electrical contact to the IC chips. Pattern defect inspection methods do not require electrical  contact, but they cannot discriminate between electrical and  non-electrical defects.


We have proposed a new nondestructive technique that can  detect electrical defects without requiring electrical contact to  the IC [1, 2]. The essence of this new method, scanning laserSQUID (superconducting quantum interference device) microscopy (“laser-SQUID” for short) is shown in Fig. 1. DCSQUID is used to detect the magnetic flux generated by OBIC (optical beam induced current). The IC or the laser beam is  then scanned and images are formed by mapping the magnetic  flux intensity or phase as a function of the laser beam position  in the IC.


The spatial resolution of laser-SQUID is much better than  conventional SQUID microscopy because it is limited by the  laser beam diameter and not the size of the SQUID detector or  the distance between the detector and the sample.  By  comparing a magnetic-flux image of a chip under test with  that of a reference chip, the laser-SQUID can be used to detect  shorts, opens, and high-resistance defects that are connected to  p-n junctions.


Laser-SQUID is compared to other nondestructive methods of  IC inspection and failure analysis in Fig. 2. The double-ended  arrows indicate the range of applicability of a particular  technique in the chip manufacturing process flow. As  indicated, the Laser-SQUID method has a much broader range  of application than the conventional methods.


Figure 1: Essence of the laser-SQUID. The spatial resolution  of the laser-SQUID is limited by the laser beam diameter and  not by the size of the SQUID detector or the distance between  the detector and the sample.


Figure 2: Applicability of Laser-SQUID in nondestructive


methods of IC inspection and failure analysis. The techniques


grouped together with IR-OBIRCH can detect electrical


defects, but require electrical contact to the IC. Pattern defect


inspection methods do not require electrical contact, but


cannot discriminate between electrical and non-electrical


defects. Laser-SQUID is sensitive to electrical defects without   requiring electrical contact to the IC.


Using our former system, we have demonstrated the basic  functionality of laser-SQUID [1, 2]. The gate-oxide-short site  of an IC chip mounted on a printed-circuit board was  observed from the front-side. In addition, open sites in 1stlevel-metal of a partially fabricated IC chip were observed  from the backside. In this latter observation, the 2nd-level  metal was deposited but not patterned. The spatial resolution


14


# Newly-Developed Scanning Laser-SQUID Microscope


was about 1.3 µm when observing an IC chip from the frontside using a 488-nm-wavelength laser. The spatial resolution  was about 100 µm, on the other hand, when observing an IC  chip from the backside using a 1064-nm-wavelength laser.


In our new system, not only the intensity but also the phase of  magnetic flux can be imaged simultaneously. A backside  observation of a 256Mbit DRAM chip using our new system  demonstrates that the spatial resolution is 0.59 µm in an  intensity image and 0.54 µm in a phase image. As shown in  Fig. 3, this result is better than our former results [1, 2], and  much better than the resolution obtained by others using a  similar type of microscopy [3, 4] or using conventional  scanning SQUID microscopy [5-8].


Spatial resolution (m)


Ceramic Stage


(X-Y scan)rm古signal


Controller


Magnetic field


Si wafer


Stage-scanSignal


bnRef.


Figure 3: Spatial Resolution vs. Sensitivity. HTS stands for  high-temperature-superconductor, and LTS stands for lowtemperature-superconductor.


ModulatedLLaser-scan signal


System


Laser beamFiberLaserP.G.


OpticalWavelength:11


The essence of our new laser-SQUID system is shown in Fig.


4. It can accommodate a 300mmφ wafer in air while our  former system [1, 2] could only accommodate a ~cm sized  sample in vacuum. The SQUID sensor and the ceramic stage  are magnetically shielded. The ceramic stage scans the sample  for wide-area imaging while the laser beam is scanned using  galvanometer mirrors for narrow-area imaging. The ceramic  stages utilize acoustic motors to avoid the generation of  magnetic noise. Their accuracy for scanning is +/-100 nm. A  HTS (high-temperature-superconducting) DC-SQUID is used  to detect magnetic flux induced by OBIC. The SQUID chip in  the SQUID sensor module is cooled down to about 77 K using  a liquid nitrogen cryostat. The distance between the sample  and the SQUID chip is usually set to about 0.4 to 0.6 mm,


while the center of the SQUID chip is usually positioned at  the center of the field of view.


The DC-SQUID chip in the SQUID sensor module is the same  as in our former system [1, 2]. It consists of a 5 mm square  large washer type of HoBa2Cu3O7-x high temperature  superconducting film deposited on a 1 mm thick SrTiO3  substrate. It has two step-edge Josephson junctions. Its  effective capture area for magnetic flux is 0.2 mm2. Background noise level is 31 µΦ0/Hz1/2 at 1 kHz (Φ0: flux  quantum = 2.07 x 10-15 Wb).


The Optical system was newly designed to give high spatial  resolution for backside observations using a 1065 nm  wavelength fiber laser. The laser beam is introduced from the


Sensitivity (T/Hz%):HTS:LTS


bottom side. The intensity of the laser beam is modulated with


1.E-08


an acousto-optic modulator and the resulting modulated


Morooka(2000)


SQUID output signal is detected using a lock-in amplifier. The fiber-laser, acousto-optic modulator, pulse generator


1.E-09


(P.G.) and lock-in amplifier are commercially available


Scanning SQUID


products. The maximum laser modulation frequency is 100


1.E-10


Kirtley(1995)


kHz, versus 10 kHz for our former system. The output signals  of the lock-in amplifier are used for imaging both intensity


。


and phase simultaneously.


1.E-12


Nikawa(2001)o◆


PC


1.E-13-This paper-Scaning Laser-SQUID


Phase dif.


-Beyer(1999)


1.E-14


Magnetic


1.E-071.E-061.E-051.E-04


Shield


signal


Intensity口 iàoPhase


SQUID sensor


Lock-in amp.


Daibo(2001)


Intensity image


Phase image


1.E-11


Chatraphorn (2000)


system1065nmSignal for Modulation


Figure 4: The Essence of Our New System. A 300mmφ wafer  can be observed in air. Magnetic-flux intensity and phase can  be imaged simultaneously.


Impact of Metal Pad Etch-Induced Plasma Damage on Dynamic Retention Time


Degradation during High Temperature Stress in High Density DRAM Technology……………....407


D. Kim, I.-G Kim, J.-Y. Noh, H.-J. Lee, S.-H Park, J.-H Lee, S.-W Lee, K.-H. Yang, J. Park,  D. Shin, K. Oh,  Samsung Electronics, Hwasung, South Korea


Effect of Ash Chemistries on TDDB Lifetime of Cu/ULK Interconnects………………………..….413


D.H. Su, L.C. Chen, J.B. Lai, J.L. Yang, R. Huang, R.L. Huang, J.S. Tsai, J.H. Shieh, S.M. Jang, and M.S. Liang, Taiwan Semiconductor Manufacturing Co., Hsin-Chu City, Taiwan, ROC


Session 20: Discretes, Passives, and MEMS


Deprocessing of Integrated Sealing Structures from MEMS Devices for Failure Analysis………..416


T.J. Barbieri1, J. Vandemeer2, (1)Freescale Semiconductor, Inc., Tempe, AZ, USA;  (2)Akustica, Inc., Pittsburgh, PA, USA


A New Non Destructive Method to Screen for Corona/Breakdown of a Transformer Core………422


G. Molle, Rockwell Collins Government Systems San Jose, San Jose, CA, USA


Unique Autoclave Stress Induced Failure Mechanism……………………………………………….427


J. Butchko, B.T. Gillette, Fairchild Semiconductor, Mountaintop, PA, USA


Hot Electron Induced Fiber Optic Transistor Beta Degradation, Recovery, and


Dynamics of Hydrogen Atoms at the Si-SiO2 Interface Layer………………………………………432


K. Seo, J. Monarch, B. Dunlap, Medtronic Microelectronics Center, Tempe, AZ, USA


Session 21: Metrology and Materials Analysis


Development of High Accuracy Automatic Magnification Calibration Function for


Scanning Transmission Electron Microscope………………………………………………………....436


H. Inada1, D. Terauchi1, R. Tsuneta2, M. Ozawa3, S. Aizawa1, K. Nakamura2, A. Takane1, M.


Konno3, H. Tanaka1, (1)Hitachi High-Technologies Corporation, Hitachinaka, Japan, (2)Hitachi  Ltd., Kokubunji, Japan, (3)Hitachi Science Systems, Hitachinaka, Japan


Methodology of Optimum-kV BSE Application in SEM and Summary of


Characteristic for Low Energy SEM/EDS/FIB…………………………………………………….....440


L.L. Lai, Semiconductor Manufacturing International(Beijing) Corp., Beijing, China


In-line High-Resistance Tungsten Plug Defect Monitoring with


An Advanced e-beam System…………………………………………………………………………..448


M. Tsai, J.H. Yeh, H. Liu, S. Lin, K. Wang, S.C. Lei, United Microelectronics Corp, Tainan  County, Taiwan, ROC; W.-Y. Wu, H.-C. Wu, Hermes Systems, Hsinchu City, Taiwan, ROC; H. Xiao, J. Jau, Hermes Microvision Inc., Milpitas, CA, USA


A Fast and Inexpensive Product Screening Method for R.O.H.S. Compliance…………………....451


P. Mazurkiewicz, Hewlett-Packard Corp., Fort Collins, CO, USA


An Overview of 300 mm SOI Starting Wafer Quality and Its Yield Detractors………………..…457


P.Y. Tsai1, J. Lee1, P. Ronsheim1, L. Burns1, R. Murphy1, M. Almonte1, G. Pfeiffer1, R. Kleinhenz1, M. Guse1, H. Hovel2, D. Sadana2, (1)IBM, Hopewell Junction, NY, USA; (2)IBM, Yorktown


Height, NY, USA


Session 22: System Level 2/Packaging 2/SPM 2


System Failures Due to Contamination Outgassing………………………………………….…...….465


M.A. Nailos, D. Stein, V. G. Hernandez, Dell, Inc., Round Rock, TX, USA


Using High Speed Camera Metrology in Support of Failure Analysis and


Product Development…………………………………………………………………………..….....…472


W. Hezeltine, R.L. Williams, F.Z. Liang, Intel Corp., Hillsboro, OR, USA


Integration of Package Analysis Tools to Solve Discontinuity Failures……………………...…...…475


K.V. Tan, S. Hsiung, LSI Logic, Inc., Fremont, CA


The Study and Methodology of Defects Isolation For Contacts of Non-Isolated


Active Region on New Logic Designs……………………………………………………………..…...479


C.H. Wang, C.M. Shen, C.J. Lin, Z.H. Lee, J.H. Chou, Taiwan Semiconductor Manufacture  Company, Ltd., Tainan, Taiwan, ROC


Focused Ion Beam (FIB) Method for Reconditioning Worn Tungsten


Atomic Force Probe (AFP) Tips……………………………………………………………………..…484


R.E. Mulder, S. Subramanian, T. Chrastecky, Freescale Semiconductor Inc., Austin, TX, USA


Session 23: Sample Preparation 2


An Alternative to High-Temperature and Acid/Solvent-Based Methods for


Removing Integrated Circuits from Ceramic or Other Problem Substrates……………………..…489


C.M. Nail, National Semiconductor Corporation, Santa Clara, CA, USA


Sectioning Integrated Circuit Ceramic Packages for Improved


Electromigration Failure Analysis………………………………………………………………….….496


B. Tracy, J. Barragan, Spansion, Sunnyvale, CA, USA  I. Grimberg, E. Raz, Sagitta, Kfar Saba, Israel


Session 24: Test


Advanced Scan Diagnosis Based Fault Isolation and Defect Identification for


Yield Learning……………………………………………………………………………………….….501


C. Eddleman1, N. Tamarapalli2, W.-T. Cheng3, (1)LSI Logic, Fort Collins, CO,USA; (2)Mentor  Graphics, Wilsonville, OR, USA; (3)Mentor Graphics Co., Wilsonville, OR, USA


Diagnosis of Multiple Scan Chain Faults……………………………………………………………..510


C.L. Kong, M.R. Islam, Intel Corporation, Santa Clara, CA, USA


Author Index……………………………………………………………………………………………517


Diffractive Lenses for High Resolution Laser Based Failure Analysis


Frank Zachariasse


Philips Semiconductors, Nijmegen, The Netherlands  frank.zachariasse@philips.com


Martijn Goossens


Philips Research, Eindhoven, The Netherlands   martijn.goossens@philips.com


In this paper we present a new method to increase the lateral  resolution available in laser scanning failure analysis tools.  By  fabricating a diffractive lens on the back side of the die, the  area of the circuit of interest, directly underneath the lens, may  be studied with a lateral resolution up to 3.5 times better than  without the lens.  This method is easily implemented with  standard equipment already present in most failure analysis  laboratories, and overcomes some significant problems  encountered with alternative resolution enhancing schemes.


Laser based fault localization methods, such as TIVA, SDL or  LADA have proved to be extremely powerful in the analysis of  90 nm and 65 nm CMOS technologies. [1,2]  For such  technologies, the laser is usually applied from the back side of  the die, through the silicon substrate, and infrared light with a  wavelength of typically 1340 or 1064 nm is used.  The  mechanism behind these techniques, where a focused laser  beam is used to disturb the operation of the IC, suggests that  they should in principle scale down well to further technology  nodes, regardless of operating voltage or clock speed. This  makes laser based localization a particularly strong candidate  for future fault localization in contrast to, for example, photoemission, which scales poorly.


However, a major drawback of optical methods is that the  minimum pitch of features that can be resolved (hereafter  termed resolution) is limited by diffraction effects to:


Resolution = 0.61λ / n sin θ


(Equation 1) Where λ is the wavelength in vacuum, n is the index of  refraction, θ is the semi-angle illustrated in Figs.1-2 and the  factor  (n sin θ) is the numerical aperture (NA) of the  microscope objective.  For a typical long working distance  100x objective with NA=0.7, this limits the resolution to about


1.1 µm with 1340 nm light, far larger than the circuit feature  size.


Advanced imaging systems that use a solid immersion lens (SIL) to increase the numerical aperture can significantly  improve the resolution. [3,4]  Commercial solutions, in which  the SIL is integrated in the microscope objective, are effective, but place significant limitations on the accessibility of the  device under test, because of the physical space required to  place the SIL lens in contact with the circuit whilst it is  operating.  Some combinations of package and socket prevent  the use of such a SIL lens.  In addition, these systems require  the die to be thinned to a precise thickness to optimise the  image quality.


In this paper we present an alternative method for improving  resolution that overcomes the above limitations. We show how  to fabricate a lens directly on the back side of the silicon of the  device under test (DUT).  This lens works on principles of  diffractive optics and is around 260 nm thick.


The advantages of the diffractive lens are threefold: Firstly, since the lens is fabricated directly on the back side of the  silicon die, the improved resolution can be obtained on any  existing laser scanning microscope, and does not require a  system specially equipped with a SIL objective.  Secondly, it is  not necessary to thin the die to a specific thickness, because  the lens may be designed, on the fly, to match the thickness at  hand.  Thirdly, since there is no need to bring a SIL objective  into contact with the DUT, long working distance objectives  may be used, thereby relaxing constraints on package and  socket choice and eliminating the risk of damage to either the  microscope objective or the DUT.


Since the diffractive lens works on principles of interference, it  will only produce an image with monochromatic light.  This  means that it is suitable for use with lasers, but not in  broadband situations such as photoemission.


Background


As light enters a flat silicon surface, it undergoes refraction.  (Fig. 1) Inside the silicon, the wavelength is shorter by a factor  of 3.5, the index of refraction of silicon. At the same time, by  Snell’s law, the sine of the semi-angle θ is reduced by the same


# Diffractive Lenses for High Resolution Laser Based Failure Analysis


Air, n=1


Semi-Angle θ


Silicon, n=3.5


factor.  Therefore, following equation 1, the diffraction-limited


resolution is not affected.  However, the silicon substrate  introduces a spherical aberration that can degrade the  resolution. [5]


If the NA of the light cone impinging on the focal plane is  increased, we can take advantage of the shorter wavelength in  silicon and obtain a better resolution.   This can be achieved by  arranging the silicon surface to be a lens shape.  Figure 2  illustrates such a solid immersion lens (SIL).


Figure 1. Light entering a flat silicon surface undergoes  refraction


Figure 2. A spherical silicon surface, centered on the focal  point, ensures all light rays hit the surface at an angle of  90 degrees: they are no longer bent when entering the  substrate.


A solid immersion lens may be implemented in various ways:  For example, by pressing a hemispherical piece of silicon onto  the DUT, or by removing a portion of the substrate, leaving  the lens shape standing. [3,4]


Diffractive lens design


In conventional optics, the shape of a lens is governed by the  fact that light rays travelling from one focal point and being


brought to a focus at another point by the lens all encounter the  same optical path length.  The design principle of diffractive  lenses, on the other hand, merely dictates that the different rays  should have the same phase at the focus, and not necessarily  the same absolute path length.


Referring to Fig. 3, we can discuss the design of a diffractive  lens by considering rays that take different paths through the  lens.  In the analysis it makes no difference whether we discuss  light travelling out of the silicon or into the silicon and we  choose the former.


Figure 3.  Ray geometry of the lens.


Let us consider 2 rays, travelling along paths AB and AC, with  an angle θ between them. Point A is the focal point of the lens.  Point B is outside the silicon by some distance, and point C is  on the silicon surface.  The lens is designed such that these  rays will continue in a straight line after they leave the silicon.  This means that all such rays together will form a spherical  wave-front outside the silicon, centred on A, and rays at all  points on the sphere connecting B and C (marked with a dotted  line) will be in phase.  The distances AB and AC are equal, both are radii of the spherical wave-front.


For a flat silicon surface however, the waves at B and C are  not in phase because the wavelength in air is longer than in  silicon, and AB travels some distance through air.


If instead we adjust the thickness of the silicon, reducing the  thickness as θ increases so as to exactly cancel the phase  difference between AB and AC, then the structure obeys the  design principle, and acts as a lens.  If this is done, then the  surface cross-section is shaped as shown schematically in  Fig. 4.   The depth of silicon removed increases from zero at  the centre of the lens, to a maximum of λ/(n-1).  At this point, the removed depth is such that it compensates one full  wavelength of phase shift, and we can allow the silicon to  return to the original thickness.  This process is repeated with  ever increasing radii.


For the ideal diffractive lens of Fig. 4, the phase of all rays is  compensated, and the throughput efficiency of the lens can


C


Silicon thickness d


θ


approach 100 %.  However, such a shape is difficult to  fabricate, and in this work, a binary approximation of the ideal  shape was used instead.


Figure 4. Ideal shape of a diffractive lens, shown  schematically in cross-section.


Figure 5.  (a):  Cross-section of a binary approximation to the  ideal shape of Fig. 4.  The corrugation amplitude is λ / 2(n-1)  (b): Plan view design plot of the same lens, with the crosssection line shown in grey.


As shown in Fig. 5, the cross section of this binary diffractive  lens has just 2 levels of depth.  The first step down is made  when the phase difference is λ/2, and the height of the steps is λ / 2(n-1), which is 268 nm for silicon with 1340 nm light.  In  calculating the radii at which these steps should be made for a


given wavelength and sample thickness, we followed the  example of Brunner et al. [6]  Note that a SIL lens designed  according to the above procedure automatically has the correct  shape to eliminate the effect of spherical aberration  encountered with back side microscopy.


For a binary lens, the phase of intermediate rays is not  perfectly compensated and much of the light interferes  destructively.  Therefore, the maximum theoretical transfer


←


efficiency is only 40.5 %. [7]


Fabrication


The DUT is prepared by mechanically polishing the back side  of the die to an optical finish.  The thickness of the silicon is  measured after polishing and is used as a parameter in the lens  design.


Resistless ion beam lithography is then used to fabricate the  diffractive lens.  In this process, the Focused Ion Beam (FIB) is programmed to implant areas that should remain high in the  final lens with a known ion dose, whereas areas that should  become low are not implanted.  The sample is then removed  from the FIB and plasma etched to a target depth of 268 nm in  a plasma etcher.  The process [8], illustrated in Fig. 6, relies on  the fact that materials implanted with gallium ions etch more  slowly in subsequent etching steps than unimplanted regions.  At the correct dose of ~100 pC/µm2, a complete etch-stop  effect is obtained.  Regions thus implanted contain a  concentration of gallium in the upper 30 nm of around  10 at. %.


Figure 6. Schematic cross-sectional representation of the  maskless FIB lithography process.  Silicon is implanted with  gallium to a depth of about 30 nm.  Subsequent plasma  etching develops this pattern to the selected depth.


The lenses shown in this paper were fabricated as follows:  For  lithography, the sample was loaded into an FEI Dual Beam  835 FIB and positioned with the point of interest at the centre  of the screen.  Navigation was performed by making  registration marks on the on the back side of the die, near the  corners, then noting in the laser scanning microscope the  positions of those marks relative to the GDS2 lay-out of the


Depth = 0


Depth = λ/(n-1)


Implant


Gallium ions


by FIB


After plasma etch, non-implanted


regions are deep


a


b


circuit.  This allows one to position the lens in the FIB to  within 5 µm of the intended position, despite the lack of direct  alignment features.


In order to write the patterns, a computer program was created  to generate a pattern file in a text format.  The pattern file  specifies the ring diameters, positions, and ion exposure dose  of all the regions to be implanted.  The exact design of lens  may be made just before lithography takes place, by selecting  the desired laser wavelength, sample thickness, and diameter  of the lens.  In addition, the beam current selected on the FIB  is a parameter in the design program, so that the correct  exposure time for each ring is calculated.  Effectively, this  means a unique lens may be designed and fabricated for each  case.  Figure 7 shows an SEM image of a lens taken  immediately after implantation.  The implant step causes a  darkening of the silicon surface when observed in the SEM.  The dose is sufficiently low that the FIB removes only a few  nanometers of silicon by sputtering during the implant.  For


ndocG20A


this lens, made with an implant dose of 100 pC/µm2 and a  beam current of 1000 pA, the implantation step takes 25  minutes.


The combination of magnetic shielding and laser modulation  with lock-in detection makes it possible to detect sub-picoTesla/Hz1/2 magnetic signals in the presence of micro-Teslaorder magnetic noise in our lab. The combination of high  frequency (100 kHz) modulation and laser beam scanning  have made it possible to obtain a laser-SQUID image in as  short a time as 30 seconds, compared to over 10 minutes using  our former system.


15


The actual system is shown in Fig. 5. In Fig. 5 (a) and (b), portions of the magnetic shield have been removed for clarity. Figure 5 (a) shows the state before setting a wafer. Figure 5


(b) shows the state after setting a wafer and introducing it  under the SQUID sensor. Figure 5 (c) shows the state during  observation: all the magnetic shields are in place.


5μm


(a) Before sample setting.


Intensity


SQUID


Wafer


4.6


jMn


4.4


Mm


in m


4.2(arb. unit)


0.59μm:FWHM


(b) After sample setting.


Phase0.54μm:FWHM


ILaser


-130-135


Magnetic Shield


-140(degree)


(c) Under observation.


Figure 5: Photos of Our New System.


Experimental Results and Discussion


Spatial resolution


A 256Mbit DRAM chip was used for demonstrating the  spatial resolution of our new laser-SQUID system. We  searched over the whole chip to locate the minimum sized  features that were resolved. Figure 6 shows that the spatial


resolution, defined as FWHM (full width at half maximum), is


0.59 µm for the intensity image, and 0.54 µm for the phase


image. These values are better than the estimated diffraction  limit (0.7 µm, NA=0.76) of the laser spot.


0123(μm)


(a) Intensity image


0123 (μm)


(b) Phase image


Figure6: Scanning laser-SQUID image showing the minimum  spatial resolution in our new system.


16


7X0-10


Selection of good chips from a wafer


Selecting good chips from a whole wafer is usually achieved  by probing and electrical-testing using ATE (Automated Test  Equipment). We have checked if it is possible to select good  chips from a wafer using the laser-SQUID. In general, it was  difficult to select good chips. In some cases, however, the  laser-SQUID was able to demonstrate this capability.


Figure 7 shows an example of good chip selection. Chips S.N. 1, 2, and 3 passed ATE testing while chip S.N. 4 failed IDDS  testing. The images in the 1st row of Fig. 7 are intensity  images of the whole chip (10.5 mm x 6.4 mm area) while  those in the 2nd row are phase images taken at the same time.


7x10-10


The image acquisition time for each chip was about 10


minutes (stage scanning mode). The images in the 3rd and 4th


rows are subtracted intensity and phase images, respectively,


using chip S.N. 1 as the baseline. These images show good


correlation between ATE testing and the laser-SQUID testing.


ce


FIB cut


|S.N. IDDS|1 GOOD|2 GOOD|3 GOOD|FAILURE|4|
|---|---|---|---|---|---|

|8||||||

|3||||||

|王||||||

|b||||||

|PHASE||||||

|SUBT. NSITYINTE|BASELINE|||||

|SUBT, PHASE|BASELINE|||||

Figure 7: Correlation between ATE testing and laser-SQUID


Phase (degree)


testing. Each image is of the whole chip (10.5 mm x 6.4 mm  area).  Scanning time for each was about 10 minutes (stage  scanning). Laser Modulation: 100 kHz.


Localizing open site from whole chip area


One of the most important functions of a failure analysis tool  is localizing defective sites from the whole chip area. Figures


180


8-11 demonstrate this function on a 90nm-node logic IC chip. Focused ion beam (FIB) cutting was used to create an  electrical open-site in the chip, which was then localized by  laser-SQUID.


Figures 8 and 9 compare the intensity and phase images, respectively, of the whole 5 mm x 5 mm chip area, before and


after FIB cutting. The FIB-cut site is clearly identified in both


\


imaging modes. The phase image, Fig. 9 (b), in particular, shows a drastic change at the FIB-cut site. Figures 10 and 11  show the intensity and phase images of the FIB-cut site in  more detail (1 mm x 1 mm area). The FIB-cut site is more  clearly and precisely identified in both the intensity image, Fig. 10 (b), and in the phase image, Fig. 11 (b). Again, the  phase image, Fig. 11 (b), shows a drastic change at the FIBcut site.


Intensity(arbitrary unit)


(a) Before FIB cut


Intensity (arbitrary unit)。


(b) After FIB cut


Figure 8: Laser-SQUID intensity images of a whole chip area (5 mm x 5 mm) before and after FIB cut.


-180KKAKAKIND


-180


M TWNO


Figure 9: Laser-SQUID phase images of a whole chip area (5  mm x 5 mm) before and after FIB cut.


17


口


metal


Figure 10: Laser-SQUID intensity images of a localized


conteact


defective area (1 mm x 1 mm) before and after FIB cut.


-njunction


个


p-sub.


p-njunction


一个p-sub.


Figure 11: Laser-SQUID phase images of a localized  defective area (1 mm x 1 mm) before and after FIB cut.


4x0-10


Note that the images in Fig. 10 and 11 are not only zooming  of the images in Fig. 8 and 9. This is because the center of the  SQUID chip is always positioned at the center of the field of  view. This causes differences in the detected magnetic  intensity and phase between wide scanning and narrow  scanning, even when the laser beam irradiates the same point  on the IC chip.


A model for localization


bitrary unit)Intensity (ar


The effect of the FIB-cut on laser-SQUID imaging was  modeled. The logic chip used has a very complicated  structure, so we use a simplified structure here to better  understanding the localization mechanism.


4x10-10


The simplified model of the structure of interest is shown in  Fig. 12 , which also shows the current flow during laser beam


↓


irradiation. Figures 12 (a), (b), and (c) show the current flow  when the laser irradiates the left side, the right side, and the  center of the metal line of interest, respectively. In each case, the total current flow is similar so the laser-SQUID  measurement should be similar. The contrast seen in the  intensity (Fig. 10-a) and phase (Fig. 11-a) images of the real


(arbitrary unit)Intensity


structure are created by its complicated design.


laser


contact metal


(a) Left-side irradiation


(b) Right-side irradiation


contact p-n junction


)Phase (degree


↑


(c) Center irradiation


Figure 12: Simple model: before FIB-cut. In the actual chip,


the metal line makes a closed circuit around the chip.


18


Figure 13 shows the current flow and laser-SQUID images  after the FIB cut is made. Figure 13 (a) shows the simplified  model with the FIB-cut and the actual images at the  corresponding location. Figures 13 (b), (c), and (d) show the  current flow when the laser beam irradiates the left side of the  FIB cut, the right side of the cut, and near the cut site, respectively.


(a) FIB-cut site with laser-SQUID images. Intensity image is  a part of Fig. 10(b) and phase image is a part of Fig. 11(b).


(b) Left-side irradiation


T


(c) right-side irradiation


(d) Near cut-site irradiation


Figure 13: Simple model: after FIB-cut


The current flow is drastically different for these three cases. When scanning across the cut, a 180-degree phase change is  expected because the direction of main current flow reverses  between the left-side-irradiation case, Fig 13 (b), and the  right-side-irradiation case, Fig. 13 (c). This explains why there  is a phase reversal at the FIB-cut site in the laser-SQUID  phase image shown in Fig. 13 (a). In the near-cut-siteirradiation case, Fig. 13 (d), the current flowing from left and  right compensate each other. This explains why the intensity  image shown in Fig. 13 (a) is dark at the FIB-cut location.


Conclusions


We have developed a new version of a scanning laser-SQUID  microscope. Its spatial resolution was demonstrated to be 0.59 µm for intensity imaging, and 0.54 µm for phase imaging. The


Intensity Image


usefulness of laser-SQUID was demonstrated using two  examples. In the first example, a case of IDDS test failure of  256Mbit-DRAM chip on a wafer, we succeeded in identifying


Phase Image


the good chips from the failed chip. In the second example, locating an electrical open created by FIB-cutting, we  successfully imaged a whole 90 nm-node logic chip and


oni


localized the open.


We would like to thank Toru Matsumoto, Hirotoshi Terada, Toshimichi Ishizuka, Yoshimitsu Aoki (Hamamatsu  Photonics), Tatsuoki Nagaishi (Sumitomo Electric Hightechs), Koji Akashi (Kyocera), Shoji Inoue, Hideo Nakayama (TDI), Hitoshi Yokoyama, Takeshi Mizukami (Elpida Memory), Abiko Hitoshi, Shinobu Asayama (NEC Electronics), and  many others at these companies.


[1] K. Nikawa and S. Inoue, “Novel Nondestructive and  Non-electrical-contact Failure Analysis TechniqueLaser-SQUID Microscopy -,” Proc 39th International  Reliability Physics Symposium, Orlando, FL, April and  May. 2001, pp. 289-293.


[2] Nikawa, K., “Laser-SQUID Microscopy as a Novel Tool  for Inspection, Monitoring and Analysis of LSI-chipdefects: Nondestructive and Non-electrical-contact  Technique,” IEICE Trans. Electron., Vol. E85-C, No. 3 (2002), pp. 746-751.


[3] Beyer, J., H. Matz, D. Drung, and Th. Schurig, “Magnetic  detection of photogenerated currents in semiconductor  wafers using superconducting quantum interference  devices,” Appl. Phys. Lett., Vol. 74, No. 19 (1999), pp. 2863-2865.


[4] Daibo, M., T. Kotaka, and A. Shikoda, “Photo-induced  magnetic field imaging of p–n junction using a laser  SQUID microscope,” Physica C, Vol. 357-360, Part 2 (2001), pp. 1483-1487.


[5] Knauss, L. A., B. M. Frazier, H. M. Christen, S. D. Silliman, K. S. Harshavardhan, E. F. Fleet, F. C. Wellstood, M. Mahanpour, and A. Ghaemmaghami, “Detecting Power Shorts from Front and Backside of IC  Packages Using Scanning SQUID Microscopy,” Proc 25th  International Symposium for Testing and Failure  Analysis, Santa Clara, CA, November. 1999, pp. 11-18.


[6] Chatraphorn, S., E.F. Fleet, F.C. Wellstood, L.A. Knauss, and T.M. Eiles, “Scanning SQUID microscopy of


19


integrated circuits,” Appl. Phys. Lett., Vol. 76, No. 16 (2000), pp. 2304-2306.


[7] Kirtley, J. R., M. B. Ketchen, K. G. Stawiasz, J. Z. Sun, W. J. Gallagher, S. H. Blanton, and S. J. Wind, “Highresolution scanning SQUID microscope,” Appl. Phys. Lett., Vol. 66, No. 9 (1995), pp. 1138-1140.


[8] Morooka, T., K. Tanaka, A. Odawara, S. Nakayama, A. Nagata, M. Ikeda, and K. Chinone, “Development of  scanning SQUID microscope for studying  superconducting films and devices,” Physica C, Vol. 335, (2000), pp. 157-163.


20


Stacked-Die Failure Mechanisms for an Octal, Current Input  20-Bit Analog-to-Digital Converter


Bob Craigin, Bin Ling Zhou, and Jason Bridgmon


Texas Instruments Tucson Corporation, Tucson, AZ, USA


Cross-section Drawing


Stacked-die packaging was used to make an octal 20-bit


analog-to-digital (A/D) converter by stacking two quad A/D  converter die in a single 48-lead QFN (quad flat-pack, no


top and bottom die thickness:6mils


leads) package. Reliability testing for product qualification


spacer attach:non-conductive epoxy silicon spacer thickness:8mils


initially failed only (biased) HAST test. Two failure


bottom die attach: silver-filled epoxy


mechanisms were identified. The first mechanism was silver  ion migration at sensitive analog inputs due to high  conductive die-attach fillets on the bottom die. The second


X-ray Image


mechanism was ILD delamination and passivation layer


spacer,


top die


cracking due to spacer-attach stress on the surface of the


bottom die


bottom die. Electrical failure analysis was aided by a self test  mode designed into the quad A/D converter. Package opening


lead-frame


and other standard failure analysis techniques required some  modification to accommodate the stacked-die package. This  work points to critical stacked-die assembly steps, including  conductive die-attach and nonconductive spacer-attach  application, where effects of moisture, bias, and thermal stress  must all be considered.


Stacked-Die Package-Advantages and Drawbacks


Stacked-die packaging allows multiple die to occupy the same  footprint as a single die. This can multiply the capacity or  processing power of a system by the number of stacked die  without increasing physical size. Further, stacked-die  packaging can increase capacity or processing power density  without additional silicon design and fabrication development  time [1], [2]. In the present case, an octal 20-bit analog-todigital (A/D) converter was made by stacking two quad A/D  converter die in a single 48-lead QFN package (Fig. 1). QFN  package dimensions and pin-count were identical for both the  octal and quad versions (7mm x 7mm x1mm, 48 pin). This  effectively doubled the number of A/D converter channels  available in the same QFN footprint while minimizing pin-out  changes. A primary use for the current input 20-bit A/D  converter is in computed tomography (CT) for medical  applications, and doubling the number of converter channels  in the same package simplifies upgrade that can double a  system’s resolution. Despite the advantages of the stacked-die  package, potential drawbacks have been identified. For  example, with reduced die thickness, thermal dissipation  problems multiply, and die-attach and wire-bond complexity  increase [2], [3], [4].


Figure 1: Cross-section drawing and x-ray image showing the  stacked-die structure using an 8mil thick silicon spacer and  two identical quad A/D converter die thinned to 6mils.


Quad A/D Converter-Brief Description


The Octal 20-bit A/D converter multiplexes integrated analog  input current to four delta-sigma converters, and has a  maximum data rate of 3.125kSPS (kilo-samples per second). The part is implemented via 0.5µm double-poly, double-metal  CMOS technology. It has relatively low power consumption  at 13.5mW/channel with total power consumption at 150mW  in the low power mode and 200mW in the high-speed mode. The A/D converter’s most unique feature is its ability to  integrate and convert very low-level (femtoAmp) input  currents. A block diagram of the device is shown in Fig. 2, an  optical image of the top die quad A/D converter is shown in  Fig. 3, and a SEM (scanning electron microscope) image of  the octal A/D converter with molding compound removed is  shown in Fig. 4. As shown in Figs. 1 and 4, the 48-lead QFN  package allows silicon spacer and quad A/D converter die to  have a thickness of 200µm and 150µm respectively. This is  relatively conservative compared with reported minimum  spacer and die thickness of 50µm to 75µm [1], [4]. High yield  for the quad A/D converter gave confidence that a high  percentage of good die could be packaged in the stacked-die  configuration. Although early qualification test results were  optimistic unexpected failures occurred in HAST (highly  accelerated stress test).


21


# Stacked-Die Failure Mechanisms for an Octal, Current Input 20-Bit Analog- to- Digital Converter


AGND


DGND


Figure 2: Block diagram of the octal, current input 20-bit A/D  converter; IN1-IN4 are bottom die analog inputs.


Figure 3: Optical image of the top die of the stacked-die  package, which is a quad, current input 20-bit A/D converter; analog inputs IN5-IN8 are at the upper edge.


WAGC


VREFDVDD


-→CLK


IN1


DUyb6+Switched


as


Digital


Intograton


ModutatorFitorControl-O RANGE2


06


IN3


-→ CUK.4X


Dug 0Swilched


-O RESET


integranor


IN2


Dusl Swilched


Δz


Dgital


Integrato


Modulator


We。


-O FORMAT


IN4


DLud


DOLK


Swilched


ISPDLOPWR O TEST


-O RANGE1


-0RANGED CONV


Integraton


-O DOLK


DDC118 5.(RV 21.6mm x25 SE(M)


2.00mm


INS


DualSwitched


Δ2


-→DVALID


Figure 4: SEM image of the octal A/D converter with molding


DigitalImput/Output


compound removed; analog inputs are at the left edge.


ModulatorFilterDOUT


or石


IN7


Dugl


-O DOUT


Reliability Testing


-→ DN


Since this was the company’s first ever stacked-die QFN


IN6


package, complete qualification was required. JEDEC


Dual Switched


az


Digitsl


-ODN


Standard reliability tests included temperature cycling (-65°C  to +150°C for 1000 cycles), autoclave (121°C at 2atm. for  240hrs), HTOL (high temperature operating life, 125°C,


IN87Switched万Intogrator


ModulatorFRer


biased for 1000hrs), and HAST (130C, 85% relative humidity,


Integrator


~2atm., biased for 96hrs). Parts were pre-conditioned  according to moisture sensitivity level 3 with simulated solder  re-flow temperature of 260°C (solder preconditioning) prior to  those tests. There were no failures for temperature cycle, autoclave, and HTOL. However, the first HAST test resulted  in up to 96% failure depending on assembly lot. Subsequent  failure analysis identified two distinct mechanisms responsible  for HAST failure. In all cases, failure only occurred for A/D  converter channels on the bottom die.


First Failure Mechanism


Electrical Failure Analysis


The first mechanism was determined to be silver ion migration  at bottom die analog input bond pads due to moisture, bias, and proximity of (silver-filled) conductive die-attach [5]. Failure analysis followed a standard flow starting at external  visual inspection. Electrical characteristics pointed primarily  to noise, offset, and gain error at analog input regions. Localization of failure to analog input regions was possible  because of an on-board self-test feature (test mode). Fig. 5  shows a simplified block diagram for test mode  implementation at an analog input (IN1). In test mode, switches SA and SB are opened and switches SAT and SBT are  used to transfer ~13pC charge packets from capacitor CTEST to  an integrator. Therefore, test mode disconnects analog inputs  from the integrators and A/D converters. The majority of  initial HAST failures operated properly in test mode. This  limited failure in those devices to analog inputs, analog input  ESD protection cells (not illustrated), and switches SGND, SA,


22


and SB. Thus the test mode function, designed as a system  debug and diagnostic tool, served additionally as an excellent  failure site location tool. As shown in the IV-characteristics of  Fig. 6, probing between a bottom die analog input and thermal  pad (mechanically connected to the die substrate via silverfilled die-attach) showed entirely different conductivity for  good and bad devices. Good and bad devices had the same  IV-characteristics between analog inputs and the die substrate.


CINTADC


Figure 5: Simplified block diagram showing implementation


thermal pad


of test mode at an analog input (IN1).


200 μm


-10


VM


silicon spacer


Figure 6: IV-characteristics between a bottom die analog


input and thermal pad (mechanically connected to the die


substrate via silver-filled die-attach) showing little conduction  for a good device over the 3V range and forward biased diode  characteristics for the bad device; good device characteristics  were repeatable while bad device characteristics were not.


Bottom Die Conductive Die-Attach Fillets


Good and bad devices were also compared by x-ray imaging  and package cross-sections. As shown in the package crosssections of Figs. 7 and 8, conductive die-attach fillets  extended up the sides near the top of failed bottom die. X-ray


imaging consistently found larger conductive die-attach fillets  on failed devices compared with good devices. Decapsulation  to expose the bottom die for inspection and electrical test was  primarily by parallel polish through the top die and into the  spacer followed by very quick (~12sec) exposure to fuming  HNO3 at 65°C. Minimal HNO3 exposure allowed most silverfilled die-attach to be retained, but in a somewhat degraded  state. This method of opening also left the bottom die in  electrically good condition. Bottom die cleaning with 2.5min  of CH4:O2 plasma and with a silver cleaning solution


CINT


NH4OH:H2O2 (1:1) resulted in improvement in noise-related  parameters and analog input IV-characteristics respectively. Further, as shown in Fig. 9, some die-attach was found on a  bottom die surface near bond-pads and silver residue was


sYo


identified by energy dispersive spectroscopy (EDS).


SVT


INU


-OVREF


CTEST


soso


1B


FTo


silicon spacer top die


Analog input with respect to thermal pad


Figure 7: Package cross-section of a failed device showing


bottom die conductive die-attach fillet height near the top of  the 150µm die.


字


吕


good 30 bad 8 (1st)


I [uA]8


bad 8 (3rd)


0.511.522.50 bad 8 (2nd)


Figure 8: Package cross-section of a good comparison device  showing no bottom die conductive die-attach fillet.


23


Figure 9: EDS spectrum showing silver in die-attach residue  found on the top surface of a bottom die.


Corrective Action-Fillet Height Reduction


Discussions with the assembly house revealed the method of  conductive die-attach application for the bottom die, which  was thinned to 150µm, was essentially the same method  previously used for 250µm thick single die (quad version). Proponents of tape-attachment for stacked-die cite fillet height  as a critical quality requirement, and give a requirement for  fillet height less than 50% of die thickness as an example [6]. Corrective action for excessive conductive die-attach fillet  height included additional inspection controls and a revised  dispense method using a star pattern. As mentioned  previously, a small percentage of failures did not pass test  mode and failed for a different mechanism. Implementation of  the revised conductive dispense method reduced HAST failure  rate to approximately 14%.


Second Failure Mechanism


ILD Delamination and Passivation Cracking


HAST failures subsequent to conductive die-attach fillet  height corrective action did not pass test mode, were not  isolated to analog input failure, and had electrical  characteristics indicating random failure in bottom die  converter channels. Unbiased bake and re-test showed no  improvement. After considerable effort to eliminate any  possible failure due to HAST board set-up and device  socketing, an abnormal C-mode scanning acoustic microscopy (CSAM) image was obtained. Fig. 10 shows CSAM results  for a failed device indicating an air gap, which was vertically  localized at or near the silicon spacer region. As shown in  Figs. 11 and 12, package cross-section of that device found  delamination of ILD (inter-level dielectric) layers and  passivation layer cracking. As shown in Figs. 13 and 14, a  second failed device with no abnormal CSAM signature was  cross-sectioned finding similar, but less extensive ILD  delamination and passivation cracking.


Figure 10: Worst-case CSAM image of a bottom die test mode  failure indicating an air gap, which was vertically localized at  or near the silicon spacer region.


Figure 11: Package cross-section through the red center  region in the CSAM image of Fig. 10 showing bottom die ILD  delamination (arrows) under the spacer-attach fillet.


24


DDC118 5.0kV 4.9mm x6.00k SE(U)


5.00um


Figure 12: Circuitry directly under an edge of the silicon  spacer of the package cross-section in Fig. 11 showing  passivation cracking (white arrows) and ILD delamination (black arrow), which occurred at a spin-on-glass (SOG) layer.


DAC118 5.0kV 5.7mm x1.30k SE(M)


40.0um


Figure 13: Package cross-section of a second failed device  showing passivation cracking (white arrow) and ILD  delamination (black arrow).


sIjlocus deoaj


sdeoel-eulepu


DAC118 5.0kV 5.7mm x3.50k SE(M)


. . . .10.0um


Figure 14: Higher magnification of Fig. 13 showing  passivation cracking (white arrow) and ILD cracking (black  arrow).


Silicon Spacer-Attach Stress on the Bottom Die


Additional failed devices were etched open and compared to  good devices etched by the same methods. As shown in Figs.


spacer attach


15 and 16, passivation cracks and metal corrosion were found  on signal lines that span most of the die width under the  silicon spacer. No passivation or metal damage was found on  good devices or on top die of failed devices. Bottom die ILD  delamination and passivation cracking occurred primarily at  the periphery of the silicon spacer under non-conductive  spacer-attach fillets. Delamination and cracking damage is  speculated as a result of high temperature excursion during the  solder preconditioning step, but in the end HAST temperature,


TLDDO


moisture, and bias caused device failure. Root cause of failure  was attributed to large difference in thermal coefficient of  expansion between silicon and the non-conductive spacerattach (~5:1). Design of experiment varied non-conductive  spacer-attach material and bond-line thickness. Meanwhile, three lots passed HAST by reducing solder preconditioning  temperature from 260ºC to 245ºC. Ultimately, corrective  action doubled bond-line thickness of the spacer-attach (from ~0.5mil to ~1mil), and mask revision passivated all probe  pads. Probe pads were openings in the passivation over top


sljoous deoaj


metal identical in structure to bond pads, but smaller in size (~8µm x 8µm). Probe pads were added by the designer to  facilitate debug by micro-probing. Numerous probe pads were


spacer-attach


distributed over the die surface, with a high concentration of  probe pads near signal lines where passivation cracks  occurred. Mask revision closed passivation etch windows over  probe pads to avoid filling unpassivated probe pads with  spacer-attach. These two additional improvements allowed the  octal A/D converter to pass HAST after solder  preconditioning at 260ºC.


Figure 15: Passivation cracks (arrows) and metal  discoloration (corrosion) found on a failed device bottom die; passivation cracks and metal discoloration were not found on  good devices or on top die of failed devices; a row of twelve  probe pads is visible above the two left most arrows.


25


Figure 16: Higher magnification image of a passivation crack (arrow) shown in Fig. 15.


Failure attributed to conductive die-attach silver ion migration  was associated with high die-attach fillets. Failure attributed to  ILD delamination and passivation cracking was associated  with mechanical stress from silicon spacer-attach. Although  the failure mechanisms were quite different, corrective action  in both cases was related to an attachment method in the  stacked-die package. Results of corrective action targeted at  those mechanisms allowed the device to pass reliability testing  for product qualification.


Interestingly, these failures occurred only in HAST testing  where both moisture and bias were applied after 260ºC solder  preconditioning. Failure did not occur in autoclave which  applied moisture but no bias, nor in HTOL, which applied bias  but no moisture. These failure mechanisms point to critical  stacked-die assembly steps where the effects of moisture, bias, and thermal stress must all be considered.


The authors would like to thank Fred Miranda for help with  HAST set-up and testing, Craig St. Martin of Amkor for  packaging support, and Jim Todsen for overall direction.


[1] M. Karnezos, “3-D Packaging: Where All Technologies  Come Together,” IEEE/ICPMT/SEMI 29th International  Electronics Manufacturing Technology Symposium, pp. 64-67, July 2004.


[2] T.Y. Lin, Z.P. Xiong, Y.F. Yao, L. Tok, Z.Y. Yue, B. Njoman, and K.H. Chua, “Failure Analysis of Full  Delamination on the Stacked die Leaded Packages,” 53rd  Electronic Components and Technology Conference  Proceedings, pp. 1170-1175, May 2003.


[3] M. Rencz, “Thermal Issues in Stacked Die Packages,”


21st Annual IEEE Semiconductor Thermal Measurement  and Management Symposium, pp. 307-312, March 2005.


[4] J. Brunner, I.W. Qin, and B. Chylak, “Advanced Wire  Bond Looping Technology for Emerging Packages,” IEEE/ICPMT/SEMI 29th International Electronics  Manufacturing Technology Symposium, pp. 85-90, July


2004.


[5] P. J. Boden, “Surface Mount Technology-A study of  Safety Considerations: Silver Migration and Adhesive  Flammability,” IEEE Transactions on Components, Packaging, and Manufacturing Technology-Part B: Advanced Packaging, Vol. 17, No. 1, pp. 83-90 February


1994.


[6] Y.M. Cheung and C.M. Chong, “New Proposed Adhesive  Tape Application Mechanism For Stacking Die  Applications,” ICEPT 5th International Conference on  Electronic Packaging Technology Proceedings, pp. 309-315, October 2003.


26


Contrary to known art, we have discovered that lubricated  tin-silver connectors have better electrical performance and  are more reliable than lubricated silver-silver connectors  under high-current and high-vibration conditions. The antifretting lubricant, that enhances the performance and  reliability of the tin-silver connectors, is a grease consisting  of a hydrocarbon oil in a nano-sized silica-particle base. Focused ion beam and scanning electron microscopy were  used to understand the contact degradation mechanism. The  superior electrical performance and reliability of the  lubricated tin-silver connectors is due to a mechanism that  replaces the tin plating from the contact surface with a  coating of silver. The removal of the tin plating may be due  to wear and the replacement by the silver coating may be  due to an electrochemical displacement reaction.


Separable tin-plated electrical connectors are known to  suffer fretting corrosion due to micro-motion between the  contact surfaces.1, 2 Minute tin particles wear off the contact  surface and oxidize. The buildup of tin oxide increases the  contact resistance until the i2R heating of the contact leads to  contact melt down and destruction. It is generally believed  that fretting corrosion is worsened if a tin-plated contact  surface is mated to a contact surface plated with a noble  metal such as gold or silver. As a general rule, contacts with  noble-metal plating are preferred for high-current, separable  connectors in high-vibration environments.3 It is common  practice not to recommend a connector design involving  noble-metal plating contacting tin plating.4


There are anti-fretting corrosion lubricants available that  purport to eliminate fretting corrosion.5 These lubricants are  greases comprised of oils in very finely divided solid  medium such as nano-sized silica. Capillary action keeps the  oil contained in the silica base, thus preventing the oil from  flowing away from the mated surfaces.


The influence of a silica-particle based oil lubricant on the  electrical performance and reliability of tin-silver and silversilver connectors was examined. Testing was done by  forcing controlled micro-motion between the contact  surfaces and noting the contact resistance degradation and  wear. The role of electromigration was studied by passing  current through the connection in the absence of vibration  and then analyzing the contacts.


Experimental procedure and results


Tin-plated and silver-plated contact surfaces were tested for


fretting corrosion as described in Table 1. Figure 1 is a  connector schematic showing that the electrical contact is  made between a flat contact member and a curved spring  member. The Sn-Ag connectors have tin-on-nickel plating  on the flat member and silver plating on the curved spring  member. The Ag-Ag connectors have silver-on-nickel  plating on the flat member and silver plating on the curved  spring member. The Sn-Ag and the Ag-Ag connectors were  tested for fretting corrosion using a machine that applied  oscillatory, controlled displacement at a fixed frequency. The vibration amplitude was 50 µm at 80 Hz. The direction  of vibration was perpendicular to the paper in Figure 1. The  contact load was 10 N. Contact metallurgies were tested  with and without lubrication. The contact current was 40 A.


Sn-Ag connector with and without lubricant and no  current:


Figure 2 shows the effect of lubricant on fretting corrosion  in a 19-hour fretting corrosion test run on a Sn-Ag connector  in the absence of any current flow. The picture to the left  shows that fretting corrosion occurred on the non-lubricated  specimen and the picture on the right shows that no fretting  corrosion occurred on the lubricated specimen. Figure 3  shows evidence of fretting corrosion on the non-lubricated  tin plating of the flat contact member. Energy dispersive  analysis of the fretting corrosion residue showed the  presence of only tin and oxygen. Build up of tin oxide is, therefore, evident. The tin-oxide build up was enough to  cause an electrical open at the contact points.


Sn-Ag connector with and without lubricant and 40-A  current:


Fretting corrosion testing with 40-A current flowing through  the contact showed that the non-lubricated contact failed in  about 2.4 days. Figure 4 shows plots of contact voltage drop  with 40 A flowing through the contact as a function of time. The contact resistance of the non-lubricated contact rose  sharply at 2.4 days. With lubricant, the contact did not fail  even after 31 days of testing; the contact resistance held  steady and low for the duration of the test.


In order to explain the improved performance and reliability  of the lubricated Sn-Ag connector, scanning electron  microscopy (SEM) and energy-dispersive X-ray analyses (EDX) were performed along with focused ion beam (FIB) milling. SEM and EDX analyses (Figure 5) show that the tin


Silver-silver versus tin-silver electrical connectors for high current and  high vibration applications


Prabjit Singh, James R. Lloyd, Larry Palmer, James Demarest, Larry Fischer, George Hutt, Gary  Thompson, and William Brodsky


International Business Machines Corporation, Poughkeepsie, NY 12601


27


# Silver-silver versus tin-silver electrical connectors for high current and


plating in the contact area was replaced by a coating of silver. The area outside the contact remained covered with tin  plating. To understand the mechanism by which the tin  plating in the contact area was replaced by a coating of silver, FIB cross sectioning was done. As shown in Figure 6, outside the contact area, the surface is as-plated tin-on-nickel  on copper. In the contact area, the tin and the nickel plating  have been replaced by a ~2-µm thick layer of silver.


Ag-Ag connector with lubricant and 40-A current:


Figure 7 shows the fretting corrosion of lubricated Ag-Ag  connector subjected to 40-A current and vibration for 45  days. There is heavy wear in the contact area. The wear is  through the silver and the underlying nickel plating down to  the copper. The contact resistance was almost twice that of  the lubricated Sn-Ag connector shown in Figure 4b.


Simultaneous testing of four different connectors at 40  Hz and vibration amplitude of 75 µm:


In this test the vibration frequency was lowered to 40 Hz and  the direction of vibration was changed to be perpendicular to  all the tests reported so far. The direction of vibration was


made horizontal and parallel to the plane of paper in Figure


1. The four connectors tested were: (a) Non-lubricated SnAg with 40-A current; (b) lubricated Sn-Ag with 50-A  current; (c) lubricated Ag-Ag with 50-A current; (d) lubricated Ag-Ag with 89-A current. The plots of contact  voltage drop versus vibration cycles are shown in Figure 8. As in the previous tests, the non-lubricated Sn-Ag connector  failed early and the lubricated Sn-Ag connector performed  better than the lubricated Ag-Ag connector.


Discussion


The poor reliability of non-lubricated Sn-Ag connectors is  no surprise. It is well known that tin suffers from fretting  corrosion. The high reliability of Ag-Ag connectors is also


Tin


|Table 1: Fretting test matrix: Micro-motion amplitude of 50 µm at 80 Hz. |Table 1: Fretting test matrix: Micro-motion amplitude of 50 µm at 80 Hz. |Table 1: Fretting test matrix: Micro-motion amplitude of 50 µm at 80 Hz. |Table 1: Fretting test matrix: Micro-motion amplitude of 50 µm at 80 Hz. |Table 1: Fretting test matrix: Micro-motion amplitude of 50 µm at 80 Hz. |
|---|---|---|---|---|

|Platings |Lubrication |Current, A |Days of testing |Results |

|Sn-Ag |Yes |0 |0.8 |No fretting |

|Sn-Ag |No |0 |0.8 |Heavy fretting |

|Sn-Ag |No |40 |2.4 days |Fretting led to contact failure in 2.4 days |

|Sn-Ag |Yes |40 |31 days |Very light wear, no fretting corrosion |

|Ag-Ag |Yes |40 |45 days |Excessive wear with exposed copper |

Si


Copper


Tin Nickel Copper


Figure 1: Schematic of the Sn-Ag contact geometry. The  Ag-Ag contact has silver plating on the flat member


instead of the tin plating as shown above.


huhuht


Figure 2: Fretting corrosion of tin-plated surface in contact with


silver-plated surface, with no electric current, for 19 hours. The


micrograph to the left is for a non-lubricated contact. The one to the  right is for a lubricated contact.


O


Sn


1.58 μm20000


U13b6NO5 S01.


1s: 0


1.48nnto


Figure 3: Energy dispersive X-ray analysis of the wear product on the  non-lubricated tin-plated contact area indicated the presence of Sn


and O. No electric current was passed through the connector.


28


expected. Noble metals are known to resist oxidation and  therefore fretting corrosion. The surprise was that the simple  act of lubricating the Sn-Ag connector improved its  performance and reliability well beyond that of the industry  accepted Ag-Ag connector. FIB cross sectioning showed  that this improvement came about as a result of the tin and  nickel plating being replaced by a coating of silver. The  mechanism by which the tin and nickel get replaced by  silver is not understood.


Positive current flowed from the curved spring member to  the flat member. The electromigration direction would move  the tin atoms towards the contact area of the flat member. But extensive electromigration testing coupled with FIB  cross-sectioning led to the conclusion that there was no  noticeable movement of tin or nickel. The displacement of  the tin and nickel was therefore most probably due to  mechanical action. The coating of the contact area of the flat  contact member with silver may have been due to an  electrochemical displacement reaction in which the grease  acted as the electrolyte. More work has to be done to explain  the electrochemistry of this displacement reaction.


The results of the simultaneous testing of the four connectors  studied, as displayed in Figure 8, illustrate the relative  performance and reliability of the four connector


metallurgies. The non-lubricated Sn-Ag connector begins to  suffer fretting corrosion immediately. Its contact resistance  rises steadily to the destruction of the connector. The  lubricated Ag-Ag connectors perform with low contact  resistance for about 6 to 9 million cycles. Beyond this, there  is a step increase in the contact resistance, believed to be due  to the wearing away of all the silver plating and the exposure  of the underlying copper in the contact area. The lubricated  Sn-Ag connector performs with low contact resistance  because the tin and the nickel plating gets replaced by a  silver coating about 2-µm thick .It is not clear why the  lubricated Sn-Ag connector has better wear and electrical  performance characteristics than Ag-Ag connector. We have  shown this effect to be reproducible. Clearly, there is merit  in pursuing this phenomenon further so that it can be  commercially exploited.


Time (ks)


(a)


Ag-plated louver on Sn-plated bus, MTS10


Time, s


0.0 500.0x103 1.0x106 1.5x106 2.0x106 2.5x106 3.0x106


0.042


0.044


0.046


0.048


0.050


0.052


0.054


0.056


0.058


0.060


0.062


t


i


e


o


y


,


Contact voltage at 40 A current (mV)


0.064


(b)


Figure 4: Contact voltage drop of Sn-Ag connector as a function of  time for (a) non-lubricated connector. (b) lubricated connector.


cou to


Figure 5: Contact area of lubricated Sn-plated surface in contact with  Ag-plated surface subjected to 31days of fretting corrosion. The


contact area of the tin-plated contact member is covered with silver.


Figure 6: Focused ion beam cross sectioning of a Sn-plated contact


that was vibrated against an Ag-plated contact for 31 days with


lubricant applied. The left cross section is outside the contact area.


The right cross section is in the middle of the contact area.


Nickel  Copper


Silver


29


Fretting corrosion testing has shown for the first time that  lubricated Sn-Ag connectors have superior performance and  reliability compared to lubricated Ag-Ag connectors. Focused ion beam analysis of the tin-on-nickel plated  surface subjected to fretting corrosion against silver-plated  surface showed that the tin and nickel plating in the contact  area was worn away and replaced by a coating of silver. The  detailed mechanism of this newly discovered phenomenon is


unclear. It may be that the tin and nickel plating are  mechanically worn away and replaced by silver by an  electrochemical displacement reaction in which the grease  acts as an electrolyte. Eventually with prolonged fretting  corrosion, the silver coating gets worn away exposing the  underlying copper, resulting in a jog in the contact resistance  to a higher value.


1. “Fretting Corrosion in Electric Contacts”, 20th Annual


Holm Seminar on Electric Contacts, Oct 29-31, 1974.


2. M. Antler, N. R. Aukland, H. Hardee and A. WehrAukland, “Recovery of Severely Degraded Tin-Lead


Plated Connector Contacts Due to Fretting Corrosion”,


IEEE Trans on Components and Packaging Technology,


Vol. 22, No. 1, March 1999.


3. A. K. Rudolphi and S. Jacobson, “Stationary Loading,


Fretting and Sliding of Silver Coated Copper Contacts –


Influence of Corrosion Films and Corrosion Atmosphere”,


Tribology International, Vol. 30, No. 3, pp 165-175, 1977.


4. E. Bock, “Mateability of Tin to Gold, Palladium and


Silver”, IEEE Electronic Components and Technology


Conference Proceedings, 40th, Vol. 1, 1990, pp 840-844.


5. B. Cichoski, “Giving Electrical Connectors the Slip”,


Machine Design, 2004.


0.02


0.04


0.06


0.08


0.10


0.12


心


0.14


0.16


0.18


0.20


0.22


100000 200000 300000 400000 500000 600000 700000 800000 900000 Elapsed Time (s)


Time (106) (s)


0                0.2                0.4                0.6


0.8


Figure 7: Lubricated Ag-Ag connector wear and the electrical


behavior of the contact. The silver plating wore down to the copper  in less than 45 days of fretting corrosion testing. The contact


voltage drop held steady at about 90 mV, about twice that of the


lubricated Sn-Ag connector.


0.0


2.6


5.6


8.6


11.6


14.6


17.6


20.6


23.6


0.2


0.4


0.6


Sn-Ag dry 40A


Ag-Ag lube 50A


Sn-Ag lube 50A Ag-Ag lube 89A


Vibration cycles (x106)


50


100


150


200


(


.


p


|


l


g


Contact voltage drop (V)


Vibr  cycles (106)


Figure 8: Simultaneous testing of 4 different connectors at 40 Hz and  vibration amplitude of 75 µm. The lubricated Sn-Ag connector showed  the best electrical performance and reliability. In this test, the


direction of vibration was perpendicular to that of the previously


reported tests.


30


Analysis of Al-over-Cu Bond Pad Hillock and Pit Hole Defects


Daniel Cavasin and Abdullah Yassine, Ph.D.


Advanced Micro Devices Personal Connectivity Solutions Group, Austin, TX, USA  daniel.cavasin@amd.com, abdullah.yassine@amd.com


Bond pad metal corrosion was observed during assembly


process characterization of a 0.13um Cu microprocessor  device. The bond pad consisted of 12kÅ of Al-0.5%Cu atop  9kÅ of Cu, separated by a thin Ta diffusion barrier. The  corrosion was first noted after the wafer dicing process. Analysis of the pad surface revealed pitting-type corrosion, consistent with published reports of classic galvanic cell  reactions between Al2Cu (theta phase) particles and the  surrounding Al pad metal. Analysis of the bond pads on samelot wafers which had not been diced showed higher-thanexpected incidence of hillock and pit hole defects on the Al  surface. Statistically designed experiments were formulated to  investigate the possibility that the observed pre-saw pad metal  defects act as nucleation sites for galvanic corrosion during  the sawing process. Analyses of the experimental samples  were conducted using optical and scanning electron  microscopy, along with focused ion beam deprocessing and  energy dispersive X-ray. This paper explores the relationship  between the presence of these pre-existing defects and the  propensity for the bond pads to corrode during the dicing  process, and reviews the conditions under which pit hole  defects are formed during the final stages of the Cu-metallized  wafer fabrication process. Indications are that strict control of  wafer fab backend processes can reduce or eliminate the  incidence of such defects, resulting in elimination of bond pad  corrosion in the wafer dicing process.


Bond pad corrosion is a well-known and widely-studied  defect [1-4]. Although much emphasis has been placed upon  controlling corrosion through manipulation of assembly  processes (e.g., wafer saw and rinse), there have been few  published analyses of the pit hole and hillock defects which  tend to act as nucleation points for the corrosion process [5-6]. In the case of hillock growth, it has been suggested that  residual stress mechanisms cause extrusion of Al grains or  underlying Cu nodules through the Al cap layer, resulting in  the hillock morphology [7, 8]. In the case of pit hole defects, residual stress and grain boundary diffusion have been  reported to play a role in diffusion-enhanced formation of  Al2Cu theta phase particles, which provide the anodic surface  of the galvanic reaction with the surrounding Al [9,10]. However, with regard to corrosion, both defects are benign in  the absence of moisture. The galvanic cell corrosion  mechanism, which relies upon the reaction of Al and H, will  not proceed unless an electrical pathway is provided which


bridges the anodic and cathodic portions of the cell in the  presence of H2O. Hence, triggering of the corrosion event  requires that a nucleation cell be exposed to moisture, as in the  wafer rinsing and the wafer dicing process. This latter  condition most commonly occurs at the location of a pit hole  defect, which has been opened during overetching or  corrosion events during the wafer fabrication process. As will  be shown, a similar possibility exists for mechanically  damaged hillocks.


During characterization of the assembly process for a newlyintroduced 0.13um Cu microprocessor device, post-saw bond  pad corrosion was observed. Representative micrographs of  corroded pads are shown in Figs. 1 and 2


Figure 1: Optical micrograph of corrosion on representative  bond pad.


Figure 2: Electron micrograph of corroded bond pad surface. Hillock and pit hole defects are evident.


31


# Analysis of Al-over-Cu Bond Pad Hillock and Pit Hole Defects


Examination of the bond pad surfaces on incoming (unsawn) wafers revealed the presence of large numbers of hillock and  pit hole defects, as shown in Fig. 3.


15.0kV3CDM-E11:03:465.00 kX4.6656.ohG95809 #12T1 L


Figure 3: Electron micrograph of representative bond pad  from unsawn wafer. High incidence of hillock and pit hole  defects is apparent.


Experimental


Experiments were conducted to correlate incoming wafer  bond pad condition and post-saw corrosion. Representative  wafers were selected from incoming lots and selected bond  pad sites were photographed using a scanning electron  microscope (SEM), to record pre-saw condition. These sites  were electronically mapped to allow them to be located again  after the dicing process. Wafers were diced using standard  assembly dicing parameters, then the selected bond pads were  re-examined in the SEM. Die were taken from both the pre  and post-saw sample groups and submitted for focused ion  beam (FIB) cross sectioning. Surface analysis was performed  using both EDX and Auger electron microscopy on samples  from both groups


Results and Discussion


Pit Holes


Post-saw corrosion defects were found to correlate to pre-saw  pit hole defect locations. In addition, some areas which  showed no apparent pit hole defects at the magnification used  showed distinct evidence of pit hole corrosion after the dicing  process. Figures 4 and 5 show representative examples of preand  post-saw defects.


Figure 4: Pre-saw bond pad surface, showing presence of  distinct pit holes (circled areas).


E-BeamSpctDetO9V28/04MagFWDTill


10μm


Figure 5: Post-saw bond pad surface from Fig. 4. Areas  which showed pre-existing pit holes are circled in black. Many of these pre-existing defects have become enlarged due  to the corrosion process. Pit holes observed in areas showing  no pre-existing defects are circled in red.


Results of high magnification SEM inspection and FIB cross  sections confirmed the presence of Al2Cu particles inside the  pre-saw bond pad pit holes, and the corrosion-induced  removal of surrounding Al material during the wafer dicing  process. The existence of such defects in as-received material  is an indication that the Al-0.5Cu bond pad surface material  had been overetched or corroded in the wafer fabrication  backend process, resulting in exposure of the underlying theta  phase particle. Figure 6 shows the pit hole morphology pre32


saw and Figure 7 shows the pit hole after the corrosion  process has taken place.


05-759 Corroded pads, pinholes


Figure 6: Electron micrograph of pit hole on pre-saw wafer. Theta phase Al2Cu single crystal is seen in center of pit hole (8,000X).


Figure 7: Electron micrograph  of post-saw pit hole location. Corrosion byproducts are visible on surface, and theta phase  particle has been dislodged from center (25,000X).


05-759 Corroded pads,pinholes


The observation that pit hole defects were most likely to show  corrosion after wafer saw (exposed theta phase particle post  saw corrosion site) did not explain the small number of  corrosion sites which were observed to occur in areas which  had previously shown no obvious pit holes. In the latter case, a number of possibilities were investigated, including: a) Residual contamination on the pad surface had resulted in a  moisture-accelerated chemical attack at those sites, removing  enough Al-0.5Cu material to expose the underlying theta  phase particle; b) The strain field associated with the presence  of the underlying theta phase particles in those locations had  created localized areas of high chemical energy, with the same  end result, and c) Penetration of the overlying Al-0.5Cu layer  had already begun in the wafer fab backend process, but had


CeriumLabs 5.0kV 6.4mm x50.0k SE(U)


not progressed to a point at which it would be visible at the  5000X magnification, and non-electrically conductive coating  conditions used for the SEM inspection procedures in the  experiment (the samples could not be conductively coated for


the as-received SEM inspection, as that would have corrupted  the results of the dicing experiment).


After conducting very high magnification inspection (>50,000X) and Auger electron analyses on selected bond pad  surface areas, it was determined that a combination of the  aforementioned hypotheses was most likely at play, with the  most apparent being c, the pre-existence of defects which had  in fact not been visible under the imaging conditions initially  applied for SEM inspection.


First, high magnification inspection confirmed that corrosion  processes had already begun to affect the bond pad material as  it had been received from the wafer fab, as shown in Figures 8  and 9.


EFeam Spot Magn Det wD F1 500 mm500k 2086000x CBEH 49 Hxmc PAB


CeriumLabs 5.0kV 6.4mm x100k SE(U)


300nm


EGeam Spot Naon De WD12m10 0 KV 3 0 25000xCDEM 5 4 GX3 Pard conrasion


Figure 8: Close-up (100,000X) image of pre-existing pit hole  defect sites. Presence of theta phase particle and corrosionrelated removal of surrounding Al-0.5Cu material is evident.


600nm


Figure 9: Further evidence of pre-existing corrosion sites on  incoming wafer material (50,000X).


33


Secondly, Auger analyses of selected areas of the bond pads  confirmed that sub-micron sized perforations existed on the  surface, and there was distinct evidence of residual S and F  within those sites. This latter finding confirmed that  contamination from wafer fab processes (i.e., metal etch,


passivation etch) was involved in the exposure of underlying


pt5


theta phase Al2Cu particles and the initiation of corrosion  cells. Figures 10 and 11 show representative Auger


micrographs, and Figures 12 and 13 show the corresponding


pt 4


energy spectra, taken from perforation sites and ‘clean’ 2 adjacent areas on bond pads from pre-dicing material. It is 5.


pt3


evident from these data that the residual element S is present  only in the pit hole defects themselves, not on the surrounding  surfaces; conversely, the F is found at low levels everywhere.


pt2


The presence of the residuals within the perforated areas


0s


suggests that chemical attack had already commenced prior to 00the final rinsing stages of the wafer processing, which C2卫2


pt1 (nef)


supports the hypothesis that overetching events, preferentially -sF


attacking the high strain energy sites above underlying theta


是.90


phase particles, were the most likely initiation modes for the  pit hole defects.


5001000150020002500


4/04/05 20.0kV 10.0kX1.0μm


Pt 4


重


Figure 10: Electron micrograph of pre-dicing bond pad 3 surface. Minute pit hole sites are apparent. Numbered sites


correspond to the Auger spectra shown in Figure 12, with site


Pt3


#1 being a ‘clean’ surface (no perforation), and sites 2-5 2 being sub-micron pit holes with exposed theta phase particles 6


P1


910卫o年思 C


÷


91


5001000150020002500 Pt2(ref)


Figure 11: Another area selected for Auger analysis. Spectra  are shown in Figure 13, with site #2 being the reference.


Kinetic Energy (eV)


Figure 12: Auger spectra sampled from the bond pad area  shown in Figure 10. High levels of S are confirmed within the  pit hole sites, while low levels of F are evident everywhere. Point 1 is the reference surface (no perforation). Theta phase  Al2Cu is also confirmed within the pit holes.


*x10


0510223 ope


Figure 13: Auger spectra sampled from the bond pad area  shown in Fig. 11. Point 2 is the reference surface. Residual S


4/04/05 20.0kV 10.0kX.bum


and F are observed, similar to Fig. 12.


Hillocks


The occurrence of hillock defects was observed to vary widely  within the wafer lot, with some wafers exhibiting >25 hillocks  per bond pad, and others exhibiting < 15 hillocks per bond


34


pad, under the SEM inspection conditions applied. While


hillocks are a fairly well-characterized phenomenon, their


presence in fine geometry Al-over-Cu bond pad material


presents unique problems not considered previous to the


introduction of Cu-metallized circuitry. Figure 14 shows a


FIB cross section of a hillock defect, in which the eruption in  the underlying Cu metal layer is clearly visible.


ProbeNeedle


Figure 14: FIB cross section of hillock defect in Al-over-Cu  bond pad metal layers. Sub-micron size pit hole perforations  are also visible in upper right of micrograph.


Exposed Cu (anode)


It has been suggested that hillock growth is the result of  thermal processes occurring during the metal deposition and  annealing stages in the wafer fab [7, 8]. These same processes  are also referenced in published studies of theta phase particle  formation in Al-Cu films [5,6]. It is therefore likely that  similar thermal and chemical conditions during backend wafer  fab processing lead to, in some cases, the formation of both  the hillock and pit hole defects. This likelihood is supported  by the observation of proportional defect density between the  two defect types on wafers examined during this study. Of  major concern with regard to hillocks are the possibilities of  hillock-initiated interlevel metal layer shorting within the Cu  layers of the integrated circuit, and the possibility for the  mechanical dislodging of the hillock during the probing, backgrinding, or wire bonding process. The former failure  mode is self explanatory; interlevel metal shorting will lead to  functional failure; the latter mode has lower probability, but is  nevertheless important to consider.


Any mechanical impact which shears the overlying Al-0.5Cu  layer from the bond pad surface has the potential to expose the  underlying Cu extrusion. This would result in the creation of a ‘virtual’ pit hole, susceptible to galvanic corrosion. The  exposed Cu would form the anode, and the adjacent Al the  cathode, exactly as occurs with the pit hole corrosion reaction  involving exposed theta phase Al2Cu. Figure 15 shows a  schematic representation of such an event. In this case, a  probe needle serves as the shearing mechanism for the Al cap  metal, resulting in the exposed underlying Cu.


Hillock growth mechanisms in Al-Cu thin films have been  associated with the presence of theta phase Al2Cu particles


[9].  However, in cases where the hillock’s base is clearly  emanating from an underlying Cu layer, as seen in Fig. 14,


another mechanism must be at play. In this latter case, it is  likely that the Cu-based hillock has formed due to stress  relaxation mechanisms similar to those identified in the  formation of certain kinds of Al film hillocks. Both Al and Cu  films have been observed to form such features under the  same conditions governing stress relaxation [10].


Figure 15: Schematic representation of mechanical shearing  of hillock from bond pad, resulting in exposure of underlying  Cu. A galvanic cell between the Cu (anodic) and Al (cathodic) is thus created.


Of greater concern in the case of hillock features emanating  from underlying Cu films, as shown in Fig. 14, is the  possibility that any breach in the diffusion barrier layer (typically TiN or Ta) which exists between the two films, would result in creation of a Cu-diffusion ‘source’, from  which Cu could freely diffuse into the overlying Al film (and  vice-versa). This effect would substantially increase the  occurrence of theta-phase particles in the Al film, with the  attendant impact upon further hillock and pit hole defect  accumulation within the bond pad.


Defect Reduction


Methods focusing on reduction of the kinetics of the  nucleation and growth mechanisms for both hillocks and theta  phase particle were utilized to effect a reduction in bond pad  defect density. The primary growth mechanism for theta phase  particles, grain boundary diffusion, was controlled via a  reduction in thermal processing temperatures in the wafer fab  front end. Stress accumulation during Cu and Al thin film  deposition processes, the primary driving force for hillock  formation, was similarly reduced by reduction of processing  temperatures. A 50 degree C reduction in metal film  deposition temperature was found to correspond to an overall  45-60% reduction in hillock and pit hole defect density. Wafers processed under the reduced temperature conditions  were observed to be significantly more robust to prolonged


Al


Cu


35


exposure to moisture during the wafer dicing process in  assembly. Table I shows the comparison of bond pad defect  densities before and after implementation of reduced  temperature metal deposition, as well as the corresponding  material’s propensity to develop bond pad corrosion during  the dicing process.


Table I: Comparison of bond pad defect density and corrosion  susceptibility before and after metal deposition temperature  decrease. Fifty degree C difference between ‘High’ and ‘Low’ deposition temperature.


|Wafer Number |Metal Deposition Temperature |Bond Pad Defect Average |Susceptibility to Corrosion @ 30 min. Dicing Duration |
|---|---|---|---|

|1 |High |20 |Yes |

|2 |High |18 |Yes |

|3 |High |17 |Yes |

|4 |High |14 |Yes |

|5 |High |19 |Yes |

|6 |High |14 |Yes |

|7 |High |22 |Yes |

|8 |High |20 |Yes |

|9 |Low |8 |No |

|10 |Low |7 |No |

|11 |Low |9 |No |

|12 |Low |6 |No |

|13 |Low |7 |No |

|14 |Low |8 |No |

It should also be noted that any reduction in actual defect  density on as-fabricated material would also enhance the  wafers’ resistance to wafer-fab-related corrosion nucleation, such as would occur due to residual halogens or prolonged  rinse processes.


The susceptibility of Al-over-Cu bond pads to corrosion has  been examined. It was found that material most susceptible to  bond pad corrosion during the wafer dicing process exhibited  a high number of bond pad hillock and pit hole defects asreceived from the wafer fabrication process. Analyses of these  defects revealed:


• Residual S and F within the pit hole locations


• The presence of theta phase Al2Cu particles within  the pit hole defects in most cases


• Evidence of pre-existing corrosion, surrounding the  pit hole locations, on wafers which had not been  subject to the dicing process


• Extruded Cu grains underlying Al surface hillocks  A significant reduction in bond pad hillock and pit hole defect  density was obtained by manipulation of the metal deposition  process temperature during wafer fabrication. After this  reduction, a significantly greater resistance to bond pad  corrosion during wafer dicing was observed.  The occurrence  of bond pad corrosion can be substantially reduced through


strict control of thermal processing and chemical rinsing  during the wafer fabrication process.


Acknowledgement


The authors wish to gratefully acknowledge the assistance of  Dr. Raman Sankar of Cerium Laboratories in Austin, TX, for  Auger analyses provided.


1. Mautz et. al., ‘Elimination of Bond Pad Corrosion  Caused by Solvent Exposure’, Proceedings of the 3rd  International Symposium on Corrosion and  Reliability of Electronic Materials and Devices, V94-29, pp 253-259.


2. Dunn, C. F., McPherson, J. W., ‘Recent Observations  on VLSI Bond Pad Corrosion Kinetics’, Journal of  the Electrochemical Society, Solid State Science and  Technology, march 1988, pp. 661-665.


3. Lawrence, J. D., McPherson, J.W., ‘Corrosion  Susceptibility of Al-Cu and Al-Cu-Si Films’, IEEE/IRPS, April, 1991, pp. 102 – 106


4. Hua, Y. N., et al., ‘Failure Analysis and Elimination  of Galvanic Corrosion on Bond Pads During Wafer  Saw’, Proceedings of the 26th ISTFA Symposium, November, 2000, pp. 369-372.


5. Younan, et. al., ‘Investigation and Elimination of  Discolored Bondpads on Microchip’, ICSE2002  Proceedings, Penang, Malaysia, pp. 383 - 387.


6. Thomas, S., Berg, H., ‘Micro-Corrosion of Al-Cu  Bonding Pads’, IEEE CHMT Transactions, Volume  10, No. 2, June 1987, pp. 252-257.


7. Kim, D. K., et al, ‘Diffusional Hillock Formation in  Al Thin Films Controlled by Creep’, Materials  Research Society Symposium Proceedings, Vol. 594, Nov.-Dec., 1999, pp. 129-134.


8. Gladkikh, et. al., ‘Hillock Formation During  Electromigration in Cu and Al Thin Films: Three  Dimensional Grain Growth’, Applied Physics Letters, V 6, No. 10, March, 1995, pp. 1214 – 1215


9. Puttlitz, A. F., Ryan, J. G., Sullivan, T. D., ‘Semiconductor Interlevel Shorts Caused by Hillock  Formation in Al-Cu Metallization’, IEEE CHMT  Transactions, Volume 12, No. 4, December 1989, pp. 619-626.


10. Mupidi, T., Kusama, Y., Field, D.P., ‘Effect of  Texture on Hillock Formation in Al thin Films’, Materials Research Society Symposium Proceedings, Vol. 721, April 2002, pp. 123-128.


36


Die Edge Thin Film Delamination on the Bottom Die of a   Stacked Chip Scale Package (SCSP)


Lito P. de la Rama, Dante G. Nuarin and Marilin H. Nery


Failure Analysis Engineer


Intel Technology Philippines Inc., Gateway Business Park,  Gen. Trias, Cavite, Philippines


Tel: +6346-433-6988


Fax: +6346-433-3289


Email: lito.p.de.la.rama@intel.com


The increasing demand for high end electronic devices


incorporating multiple functions in a small form factor leads  to the widespread use of Stacked Chip Scale Packaging (SCSP) in the semiconductor industry.  Multiple die stacking  in various combinations have been achieved. However, new  failure mechanisms are being observed due to new package  stress characteristics.


This paper will present a unique failure mechanism observed  on the bottom die of a multiple die stack package.  A detailed  discussion of the failure mechanism showing the interaction  between the presence of a high die attach adhesive fillet and  the die singulation damage initiating a thin film delamination  from the die edge towards the active circuit area causing  electrical failures will be presented.


Stacked Chip Scale Package


The package of interest is a 3-die stack chip scale package  incorporating two active die and one silicon spacer.  It is a ball  grid array package using a substrate with a glass/polymer  composite core.  The die attach material used is an epoxy  based adhesive with silica fillers for viscosity control.  The die  encapsulant used is another epoxy based molding compound  material.  The package schematic is shown in Figure 1.


Mae Camned


Tog Die


Aheen houce


m


Figure 1.  Schematic of the stacked chip scale package with 3  die.


During package qualification, failure analysis investigation  was triggered by several functional failures after thermal  stress.  The two active die used for the qualification were  Flash memory devices.  Electrical validation of the two active  die showed that only the bottom die is affected.  Electrical  fault isolation showed a common location near the die edges  which strongly suggests a systemic issue.


Failure Analysis Results


Failure analysis approach was to expose the bottom die using  a bottom die recovery procedure [1].  Removal of the  unwanted materials on top of the bottom die was achieved  using a planar polishing technique.  The molding compound  and the top die were removed leaving the silicon spacer  exposed.  After which, reactive ion etch of the silicon was  performed to expose the die attach adhesive on top of the  bottom die.  The final step was acid jet etch to remove the  adhesive and expose the bottom die surface.


Figure 2.  Optical images showing lift-off of the top metal  layer on the die.


Visual inspection of the affected area showed lift off of the  topmost metal layer near the die edge indicating delamination.


37


# Die Edge Thin Film Delamination on the Bottom Die of a Stacked Chip Scale Package ( SCSP)


Figures 2 and 3 show the optical image and the detailed SEM  images of the delamination.


Figure 3.  Detailed SEM image of the affected region


Normal Adhesive


confirmed the delamination between the topmost metal layer


Fillet


and the underlying metal layer.


To further understand the failure mechanism, a cross-section  of the affected area was performed to reveal the extent of the  delamination.  Cross-section was done using a polishing  wheel with various silica grits.  Final polishing was done  using fine diamond films followed by cloth with alumina  slurry.


Cross-section results confirmed the presence of a thin film  delamination between the topmost metal layer and the  underlying structures.  The delamination starts from the die  edge extending towards the active region as shown in Figure


4.  Moreover, the images in Figure 4 showed that the  metallization at the die edge, where the blade cuts during die  singulation, is lifted.


Figure 4.  Cross-section images showing the delamination  from the die edges towards the active region.  Die edge  damage at the scribeline is also present.


Comparative analysis of the cross-sections of the failing unit  and a good unit show the difference on the height of the die  attach adhesive as shown in Figure 5.  Within the same unit,


only the affected die edge showed the presence of a high die  attach adhesive fillet which reaches the die topside.  The  opposite side which is not failing has a normal adhesive fillet  height reaching only to half of the die height.


Topmost metal layer


Second metal layer


High Adhesive


Figure 5.  Comparison of the die attach adhesive fillet height  between a good unit and a failing unit.


The presence of the delamination at the die edge results from a  damage that is already present at this location induced during  die singulation.  When a high adhesive fillet reaches the  damaged area additional stress aggravates the damage leading  to propagation of the damage towards the active area.  In order  to understand this interaction, a thermo-mechanical model was  generated using the package material characteristic with  varying adhesive fillet height.  The modeling would determine  the locations of the stress concentration at different fillet  height [2].


HRMA AU


Maximum Stress is


226MPa and Occurs


Inboard of Die Edge


.1


ANSYS


Figure 6.  Thermo-mechanical model for the 0% adhesive  fillet case showing stress concentration near the edge of the  spacer on top of the bottom die.


38


Modeling result for a case of no adhesive fillet is presented in  Figure 6.  The stress concentration for this case is located near  the edge of the spacer on top of the bottom die with a  maximum value of 226MPa.  This region contains a triple  point where three different materials (mold compound, die and  adhesive) meet.  The differences in thermal expansion  coefficient of these materials would make this a high stress  region during thermal stress either during reflow or  temperature cycling.


Figure 7 presents the result for the 50% adhesive fillet height.  The image shows that the stress seems to be evenly distributed  on the region between the die edge and the spacer.  The  presence of the adhesive fillet distributes the stress away from  the spacer edge.  The maximum stress value of 220MPa is  comparable to the case with 0% adhesive.


Figure 7.  Modeling result for 50% adhesive fillet height  showing the stress movement towards the die edge.


For the case with an adhesive fillet which is comparable to the  observed adhesive fillet height of the failing units, the  modeling data showed the very localized stress concentration  at the die edge with a maximum stress value of 768MPa.  This  simulation supports the hypothesis that the observed  delamination could be an effect of the high adhesive fillet at  the failing location.  The damage that is induced at the edge  during die singulation is aggravated by this high stress  concentration thereby causing the thin film delamination.


Figure 8.  Simulation result for the 100% adhesive fillet  height showing the high stress concentration at the die edge.


In this paper we have presented a unique failure mechanism  for the bottom die of a Stacked Chip Scale Package (SCSP).  The interaction between a high die attach adhesive fillet and  damage at the die edge could lead to thin film delamination  from the die edge towards the active region.  The thermomechanical simulation done further validated the proposed  failure mechanism by showing that the stress concentration  would be highly localized at the die edge for a 100% adhesive  fillet height.


In order to avoid this type of failure, control of the adhesive  fillet height during die attach process should be done.  Furthermore, improvement on the die singulation process  should also be pursued.


We would like to acknowledge the support of Intel  Technology Philippines Flash Q&R group; Chaps Adriano, Rex Absin, Abel Estrella, Junwyn Lacsao and Roberto  Andico; and the Flash Products Group in Folsom, California; Kaushal Upadhyaya, Oscar Camposagrado and Dennis  Rosseau.


[1] Flores, Christopher, “Bottom Die Recovery Procedure for  Stacked Chip Scale Package”.  Intel Internal Publication.


[2] Winter, Keith, “SCSP Technical Issue Update”.  Intel  Internal document.


39


Multi-Point Probing on 65nm Silicon Technology using  Static IREM-based Methodology


Daniel Bockelman, Asifur Rahman, Ifar Wan, Steven Chen, Scott Ettinger


Intel Corporation., Hillsboro, OR USA  Email: dan.bockelman@intel.com


As silicon manufacturing processes move to smaller feature sizes, new silicon fault isolation and debug challenges arise.  This paper  presents a methodology for silicon fault isolation/debug that allows  for simultaneous probing of multiple locations on the die using  static infrared emission logic state imaging.  Recent tool  enhancements leading to more efficient fault isolation and debug  are reviewed.  Cases are presented from debug of 65nm products  showing how this methodology was used to achieve very low  throughput times on a variety of complex new failure mechanisms.


The scope of this paper is in the area of component-level  silicon fault isolation (FI) and IREM debug methodology.  The Infrared Emission Microscope (IREM) has been used  successfully to root cause a number of issues on silicon  quickly.  During early 65nm process technology debug, throughput times averaged less than one week per case when  using IREM methodology.


IREM-based Static Logic State Imaging (LSI) is a silicon  probing technique that takes advantage of the increased  leakage current of the latest silicon process technologies [1].  The technique allows the logic states of individual devices on  the die to be determined based on their infrared emission  signatures.  The technique is extremely useful for root cause  of flaky failure modes because it can be used in situations  where only a single test run is required.  The technique has  been proven to be effective on FI and Low Yield Analysis (LYA)/Root Cause debug cases.  IREM-based probing  methodology fills the gap between logic diagnosis and actual  defect localization [2].  This paper will show how using  IREM-based probing methods add to overall productivity by  making fault isolation and debug more efficient, as  demonstrated during 65nm first silicon debug.


Other companies have made investigation into static IREMbased probing techniques and have applied them to their own  debug and fault isolation cases [3,4,5,6].


Figure 1: Illustration of logic state imaging technique. (a) IREM emission image only. (b) Layout and actual logic values  have been superimposed on each device to show how  emissions vary with logic state.


40


IREM LSI Methodology


The primary factors differentiating IREM LSI methodology  from other probing techniques are the static approach and the  multi-probing aspect.  The device under test is loaded on the  device tester and a test pattern is applied to exercise the failing  mode.  The test is run exactly the same as with other probing  techniques, except that the pattern is not looped.  Instead, the  test runs at speed with any clock shrinks applied, with the  clock being halted at the cycle of interest.  The processor has  an On-Die Clock Shrink (ODCS) feature which allows the  clock to be halted at either the high or low phase of the clock.  IREM LSI runs individual test runs, stopping the clock at each  phase of interest, while capturing the corresponding IREM  images at each clock phase.  Then the device layout is  superimposed over the images, and each emission is mapped  to its corresponding device on silicon.  Using a mapping  method, the logic states of each device can then be determined  and a logic trace can be created.  By knowing this mapping, we can then determine the logic state of most other circuits on  the die.


Unit


An example illustrating this is shown in Figure 1.  In this


Failure VerificationVoltage/Freq.Characterization


image, p-type diffusions are the brown polygons and n-type  diffusions are the yellow polygons.  When the output of a


Macro Fault IsolationBus Failure Analysis


device is at logic 1, an emission is observed on the n-diffusion  region and when the output is at logic 0, an emission is


Micro Fault IsolationDetailed Circuit Analysis


IREM


observed on the p-diffusion region.


From device simulations, it was determined that the emission


LVP/TRE/LADA ProbingIREM Analysis


Fault Simulations


mechanism being observed is soft avalanche breakdown, in  which a high concentration of electron-hole plasma in the


Circuit Fault Isolation


drain region recombines in part through indirect radiative  recombination.  For a fixed supply voltage, this effect has


Theories,FIBs, and Verification


increased on every process generation since 0.18um.  Even  with reductions in supply voltages going from generation to


Silicon Tapeout


New


generation, the overall effect has increased and we now  observe considerably more emission intensity at 1.2V on  65nm process technology than we did at 1.8V on 0.18um.


What devices can and cannot be logic state mapped in this  way?  With the 65nm process technology and latest IREM  technology, almost any device can be successfully mapped to  a logic state with a reasonable integration time (<30sec).  The  smallest devices can be difficult to map in some cases, while  in other cases they are able to be mapped easily.  Nonminimum channel length devices have less leakage current  and are sometimes more difficult to map.  The primary  challenge to logic state mapping is when a large, bright device  is directly adjacent to a small, less bright emission.  In this  case, the bright emission can spread out and mask the smaller  emission.


IREM LSI methodology consists of the following steps:


1) Initial characterization is performed to determine the signal  name and clock cycle that the defect or speedpath is first  manifested (e.g., first scanout mismatch).


2) The device tester along with the ODCS capability of the  processor (or equivalent stop-clock capability) is used to halt the


processor at a specific clock cycle and clock phase after running  the test at speed up to that point.


3) While the processor is halted but maintaining a static state, the  IREM is used to capture static images of the area of the failing  signal.


4) The equivalent region of the layout is overlaid onto the IREM  images and scaled to fit precisely to the emission data.


5) The overlay images are used to create an on-die logic state  map, using the observed relationship between emission and logic  states.


If desired, steps 2-5 can be repeated for multiple clock cycles  and a timing waveform can be created for any signals of  interest on the die.


A primary advantage of the IREM LSI technique is that  multiple nodes can be probed simultaneously.  All signals  within the camera field of view are captured in a single  acquisition.


Units


Figure 2: IREM-Enhanced Fault Isolation/Debug Flow


Figure 2 shows the IREM-enhanced fault isolation/debug  flow.  For the case of hard failures, IREM probing is used to  trace back to the failing node and locate the root cause.  Simulations can be run to verify the results or to generate the  expected “should-be” response.  In the case of a speed fail, IREM probing can be used to identify the failing destination  latch, then one of the other probing tools such as Laser  Voltage Probe (LVP), Time Resolved Emission (TRE), or  Laser-Assisted Device Alteration (LADA) can be used for  precise isolation within the combinational logic circuits.


Results


To illustrate the effectiveness of IREM probing in 65nm process  products, we present three cases that were successfully root-caused. These cases were yielding die fallout and with the short throughput


41


time required to solve them, we were able to quickly determine  issues in process, design or test platforms.


Process Defect Case


One of the wafer fabs was seeing some reticle-dependant failures, which were suspected to be caused by a metal patterning issue.  These units were failing test patterns and were sent for debug.  Failure characterization was done and no voltage, frequency or  temperature dependency was found.  The failure seemed consistent  across these variables.  Scan data was then collected and the first  mismatch was found in an array control block.  With the region-ofinterest defined, we proceeded with IREM to check for any  emission abnormality in the suspected node and its surroundings.  The emission signature was collected with the latest 100X lens of  the infra-red microscope, and this allowed us to easily infer the  logic states of several nodes at once in a 96x76.8 micron window (0.3 um/pixel).  By mapping the IREM emissions to specific logic  states, we were able to determine whether a failure had propagated  to a particular node and start our back tracing from the observed  mismatching point to isolate the defect.  Several logic gates were  probed and after only one full day of probing activity, IREM  detected an unusual strong emission intensity coming from PMOS  devices of both an inverter and a pass gate in an XOR gate (Figure  3).


0o-aal0on


Figure 3: Abnormal IREM emission found with 100x lens and


40240240240240


ae owetm


the suspected node highlighted on the layout window.


sp


805006m*sonen


pt ano-0


Schematic studies were done and a theory was created, which


5.200


bgo cpbocco goo soesssod*680


pointed to a possible broken node.  Since the gates of these two  devices are connected to the same node, both would be in a floating


d 口日o009d


。r


orbcpo


state and could cause them to be partially on/off.  This would


explain the IREM emission abnormality of the PMOS device of the


inverter, which would be close to the linear mode, and would also E cause a possible contention on the terminals of the PMOS pass


0e也可


soun


gate.


Physical failure analysis was performed and indeed the theory held 2


n


true: a broken Metal-2 line was found on the suspected node, causing it to be electrically floating.  This issue was root-caused to  a weak photoresist due to minimum M2 line spacing, which was  falling over and blocking the succeeding etch (Figure 4).


Figure 4: Physical failure analysis result. A broken M2 line  found at the path of the suspected node, caused by a weak  photoresist falling over.


This case showed the effectiveness of the IREM system in logic  state imaging, which was essential in guiding us to the location of  the node where the defect was eventually found.


Design Hole Case


Another substantial fallout was identified during system level  testing where units failed to acknowledge an interrupt command.


Failure characterization showed us that two input pins were leaking  during tri-state mode, which revealed a typical Id curve from an


囍


NMOS device.  Temperature dependency was also found on some  units, which would start to recover at colder temperatures.


The first probing tool used for analysis was the IREM system due  to its multi-probing capability and fast fault localization.  One  failing unit was examined during tri-state mode and at the first  image acquisition on the IREM system, we were quickly able to  localize an emission abnormality on devices in the I/O pads of the  leaky pins (Figure 5).


Figure 5: (a) IREM image of passing condition on pin, showing a single PMOS device in saturation. (b) IREM image  of failing condition on adjacent pin on the same unit – contention is now observed on two NMOS devices.


42


Figure 6: (a) Passing condition on pin, showing a design hole  where we have a contention path – IREM showed a PMOS in  saturation. (b) Failing condition on adjacent pin on the same  unit – the design hole starts a secondary contention, where the  pin eventually fails (keepen NMOS becomes in saturation).


The layout locations were mapped to the schematic nodes, which  showed that the abnormally strong emission intensities were  coming from an NMOS pull-down device which has the  functionality of shutting off the output path of the input pins (Figure 6).  From this starting point, two possible paths were found  and IREM was used to verify the logic states of the devices on both


n H。


paths.  Extensive logic state imaging was done to rule out one path,


可


and the focus point diverged to the other one.  At this point, circuit


analysis was done and based on the emission signatures seen on the


ED


LE


IREM, it was discovered a source of contention existed for these  particular pins as part of their unique design.  This contention


situation would also cause the affected input only pins to allow data  to flow outside of the pad, an invalid condition.  The IREM  emission seen could then be the result of an enable transistor being  in saturation mode in this failing condition.  Circuit simulation was  done and proved the contention condition seen on these two leaky  pins.  This issue was thus root-caused as a design hole and a fix  was placed for the subsequent stepping.


This case was fully solved using merely the IREM system, which  was first able to quickly find the contention node and then rule out  one of the suspected paths by mapping the photon emissions of the  devices with their logic states.  Without its 100X emission detection  lenses and multi-probing capabilities, determining the source of this  problem would have been almost impossible.


Test Platform Issue Case


In this case, Sort Yield reported yield losses during array tests.  Some units were submitted for debug and during failure  characterization, flaky dependencies on voltage and frequency


were found.  However, it was also discovered that these units  started to heal as the die temperature increased.


Figure 7: Comparison of IREM 100x emissions at passing and  failing conditions for two different tests (VIH and VIL). VIL  test showed a clear mismatch at the output of the sense amp.


The failure was seen on a raster pattern and one of the first debug  attempts was to use LADA/TIVA (Thermal Induced Voltage  Alteration) FI system tools in order to localize a sensitive node. The  entire area was scanned, but no conclusive result was found.


Forcing a logic 0 to pin (VIL Test)


At Passing Condition


At Failing Condition


Forcing a logic 1 to pin (VIH Test)


drven Dad


on


Data   Gen


When Failing With  Data=0


0Rtt=0ff


0 1


NOU


PRREEUO ORTY


on 子


keepenkeepen


Ndv=1


off


Pad


data /data on 1


1?


0? 0


Double Contention


L5 00 rvdrven D


When Passing With  Data=0


D02


Rtt=0ff


Do


keepen


Ndv=0


data


data on 1


0  0


Contention Starts


Lt


43


Debug then proceeded with scanout data and IREM for logic state  imaging.  Scanout data in the passing and failing regions were  collected and the first scan mismatch was identified.  We confirmed  its wrong state value after analyzing the IREM emissions and  started our backtrace procedure to find the source of the logic  mismatch.  Narrowing down further the logic cone, we ended up  with a logic mismatch on a 3:1 MUX select signal, which was  interestingly driven by an I/O pad signal.  This I/O circuit was then  checked in IREM when forcing logic 1 and 0 at passing and failing  conditions.  This experiment successfully revealed an emission  mismatch in the sense-amp output of this pin when we were  driving a logic 0 to the pin (Figure 7).


With the failure localized and confirmed in the pad region, circuit  analysis was done to check the pad sense-amp and it was  discovered that the voltage reference for this particular pin was set  to ½ Vtt, instead of 2/3 Vtt as the other pins.  The focus point was  then directed to the inputs of the sense-amp: the pin voltage, result  of a voltage divider, and the voltage reference, which was  calculated internally on silicon (Figure 8).


Figure 8: Sense-amp (SA) for affected pin. VIL voltage is  applied on the tester channel. The actual voltage seen by the  unit is a result of a voltage divider. This voltage is then  compared against the voltage reference to produce a logic 0  or 1.


The theory was that for a logic zero input, the actual input voltage  at the sense-amp was still higher than the voltage reference, which  made the circuit incorrectly interpret it as a logic 1.  An experiment  was done to change the voltage divider resistance value to its  maximum and minimum and we discovered that for the maximum  resistance value (70ohm) at Vtt=1.2V and at cold temperature, the  unit started to pass, while for the minimum resistance value (45ohm), the unit failed at the same Vtt value and temperature  conditions.  This result proved our theory that the issue was the  wrong interpretation of a logic 0 by the sense-amp.  At this point, we decided to check the formula for the Vil setting for this pin and  we discovered that it was set higher than expected.  While the Vil  value was set to 0mV, a lower value needed to be forced onto the  pin in order to compensate for the added 50ohm termination  resistor from the tester channel.  We ran tests for different Vil


values and the unit started to pass when Vil was lower than -60mV  at Vcc=Vtt=1.2V at -18 degrees C.


This issue was then root-caused as a tester platform bug, where the  settings specified for the VIL level of the affected pin were set  incorrectly.  With the new formula, the actual voltage forced to the  pin for a logic zero changed from 0mV to approximately -400mV  at Vtt=1.2V. This gives us sufficient margin for error.


In this case, we can see how IREM helped us debug a failure that  was initially thought to be localized in a specific array circuit, but  ended up being caused by a tester environment issue. Without the  help of IREM logic state imaging at 100X resolution of specific  nodes, this issue could have been unresolved for many days.


We have presented in this paper some of the 65nm process  yield fallout cases in which IREM was the primary tool used  to identify the root-cause of the failure. The effectiveness of  the IREM LSI in a multi-probing environment has been  demonstrated in the success rate and the small time-to-solve  needed to localize the failing device. The methodology that  we have outlined has greatly facilitated the root cause activity  by allowing us to more accurately probe devices using the  IREM LSI methodology. Average throughput times for cases  utilizing the IREM LSI approach have consistently been less  than one week.


Four years ago, IREM LSI was a demonstrated theoretical  concept. Today, we have effectively applied it to many cases  on 130nm, 90nm, and now on today’s 65nm products. With  these results, we stress the importance of IREM and its LSI  methodology in our debug activity. They have proven to  increase efficiency and lower throughput times of cases and  by incorporating this methodology into the root cause flow, the efficiency gain can also be achieved on additional current  and future design/process technology projects.


The authors wish to acknowledge Syed Rahman, Cade Greenup, Daniel Lu, Matt Kirsch, and the rest of the RA2 silicon debug  team.  They also wish to acknowledge Len Neiberg and the LTD  LYA team, the RA2 lab support team (Vincent Nguyen and  Leonard Pecos), Horst Haussecker, Steve Seidel, Zoran Stanojevic, and Lise Varner for their support in IREM development efforts.


[1]  Bockelman, Dan, Chen, Steven, Obradovic, Borna, “Infrared  Emission-based Static Logic State Imaging on Advanced


Silicon Technologies”, ISTFA 2002


[2]  Venkataraman, Srikanth, “Diagnosis meets Physical Failure  Analysis: What is needed to succeed?”, ITC 2004 Panel


discussion “Diagnosis meets Physical Failure Analysis: How  Long can we Succeed?”


SA


Vcc


Vcct


Vil


50 ohm


Tester


½ Vcct


Vcct=1.2V When RTT was enabled:


1.2 x (50/50+70) = 0.30V (10000) – Pass at Cold


1.2 x (50/50+45) = 0.63V (11000) – Fail at Cold  When RTT was disabled (0xxxx), the test failed. To Tap H


Machine


RTTCOMP fuses (126:122): Enable at Bit#126


RTT (45~70 ohm)


44


[3]  Polonsky, Stas, et. al., “CMOS IC diagnostics using the


luminescence of OFF-state leakage currents”, ITC 2004


[4]  Stellari, Franco, et. al., “Testing and Diagnostics of CMOS


Circuits Using Light Emission from Off-State Leakage


Current”, IEEE Trans. On Electron Devices, September 2004, pg 1455


[5]  Song, Peilin, et. al., “A  Novel Scan Chain Diagnostics


Technique Based on Light Emission from Leakage Current”, ITC 2004


[6]  Polonsky, Stas, et. al., “Time-Resolved Measurements of SelfHeating in SOI and Strained-Silicon MOSFETs Using Photon  Emission Microscopy”, IEEE Electron Device Letters, April  2004, pg 208


45


Failure Analysis of Soft Single Column Failure in Advanced Nano SRAM Device  with Internal Probing Techniques


Hung-Sung Lin, Wen-Tung Chang, Chia-Hsing Chao, Jesse Wang, Chang-Tan Lin, Coswin Lin


United Microelectronics Corporation, Hsinchu, Taiwan, R.O.C.


Single column failure [1], one of the complex failure modes in  SRAM is possibly induced by multiform defect types at  diverse locations. Especially, soft single column failure is of  great complexity. As physical failure analysis (PFA) is  expensive and time-consuming, thorough electrical failure  analysis (EFA) is needed to precisely localize the failing area  to greater precision before PFA. The methodology involves  testing for failure mode validation, understanding the circuit  and using EFA tools such as IR-OBIRCH (InfraRed-Optical  Beam Induced Resistance CHange) and MCT (MerCad  Telluride, HgCdTe) for analysis. However, the electrical  failure signature for soft single column failure is usually  marginal, so additional techniques are needed to obtain  accurate isolation and electrical characterization instead of  blindly looking around. Thus in this discussion, we will also  present the use of internal probing techniques like C-AFM [2] (Conductive Atomic Force Microscopy) and a nanoprobing  technique [3] for characterizing electrical properties and  understanding the root cause.


SRAM common failure modes can be categorized as single  bit, twin-bit, multi-bits, row, column, I/O, block, etc. Through  the guide of failure mapping, the failure analyst can know the  location and range of the failing area such as a bit, a column  or a certain block. The traditional PFA methods usually  include plane-view (P-V) layer-by-layer check and crosssectional (X-S) inspection by SEM (Scanning Electron  Microscope), FIB (Focused Ion Beam), TEM (Transmission  Electron Microscope), SCM (Scanning Capacitor  Microscope), etc. These methods are probably sufficient for  some hard failures caused by particles, metal bridging, missing contacts or defects. However, these standard  techniques of failure analysis  are becoming less useful as we  face soft failures with wide range like a column containing  512 or more bits long in a cell and its decode region. Blindly  looking around is incapable of identifying root cause failures. This paper will show the process and the techniques used to  narrow down the failing area and pinpoint the failing location  minimizing the destructive physical analysis and further will  demonstrate the application of internal probing techniques  which allow the failure analyst to understand the electrical  behavior of the device. Furthermore, based on the electrical


data collected by C-AFM and nanoprobing, we can obtain  conclusive FA results of those softer mechanisms which were  previously invisible and rarely quantified in electrical  characteristics by standard FA techniques.


Case Study: Substrate dislocation in Y-MUX  and pull-down NMOS induces soft single column  failure


Preliminary Bit-mapping Analysis:


Bit-mapping analysis permits us to understand the failure  modes and counts in terms of bit distribution and sensitivity to  voltage or data pattern. A typical failure bit-mapping in our  case study of soft single column failure is shown in Fig. 1.


Figure 1: A partial column  failed and the range is from1028  to1525. The designed range of the column contains 512 bits  and is from1024 to 1535


Take, for example, a designed range of the column that  contains 512 bits and is from 1024 to 1535 in Y value. However, it shows only a partial column is failed and the  range is from 1028 to 1525 with pass bits at the head and the


46


# Failure Analysis of Soft Single Column Failure in Advanced Nano SRAM Device with Internal Probing Techniques


tail of the column. To further confirm its failure mode, the  failure is retested more thoroughly at various voltages. This  ensures the failure is reproducible and more importantly, reveals if it is voltage sensitive or dependent. The retested  data shows partial column failure only at VCCmin. However, it becomes normal at VCCnom and VCCmax. This provides  valuable hints of the defect properties.


Backside IR-OBIRCH and MCT Analysis:


After finishing bit-mapping analysis, backside MCT and IROBIRCH analysis are applied in static mode to try to locate  the defect position or narrow down the failing area to greater  precision. We follow standard operating conditions of the chip  powered by an HP4155 semiconductor parameter analyzer  and then acquire emission spots by MCT at the Y-MUX and  pull-down circuits of the column rather than the cell array as  shown in Fig. 2. Based on our FA experience, if MCT spots (for isolation of junction leak, GOX defect, hot carrier, forward bias, etc.) locate at the same place as IR-OBIRCH  ones (for isolation of  current/resistance change due to laser  heating), the possibility of the failure located just under the  spot will increase, so after MCT, IR-OBIRCH is also


AFM Image


C-AFM Image


introduced for analysis. As shown in Fig. 2, IR-OBIRCH  signals are also located at the Y-MUX and pull-down circuits. With the electrical data collected by MCT and IR-OBIRCH, one of the samples is physically deprocessed; However, no


valid defect or convergent discovery could be found by SEM.


"


Besides, passive voltage contrast (PVC) carried out with both


00


SEM and FIB tools also shows no contrast there. Somehow, it  seems to correspond to the result of the preliminary bitmapping analysis. Anyway, additional analysis is needed to


4.006.000.D0200408600


further understand the electrical behavior and precisely


0.03200


pinpoint the defect location.


Current:0.321 [mx


chana


Velese102 VJ


2.08-08


I，


Figure 2: IR-OBIRCH signals are located at the same place


024601012 ODE CO一


as MCT in Y-MUX and pull-down circuits of the column.


-2.0B-08


voltage


Internal Probing Analysis:


As the failure mechanism becomes more complex, we need  electrical characterization of a die’s internal circuits or a  single transistor for fault identification and defect  discrimination. Consequently, C-AFM and a nanoprobing  technique are introduced to do internal probing in the Y-MUX  and pull-down circuits for electrical characteristic  measurements. The other unit was parallel lapping down to  contact level and then mounted on a disc using silver paint. CAFM measurements were performed on a DI CP-II instrument


with a Doped Diamond-coated probe tip used to collect  current mapping as well as the topographical profile of the  sample’s surface.  A current mapping by C-AFM on the  contact level of the Y-MUX NMOS circuit is shown in Fig. 3. It shows the position of failed contacts with N+/PW early  breakdown. Since the failing area is pinpointed and can be  narrowed down to a single transistor, technique for in situ  device probing is performed by Zyvex S100 Nanoprober a  SEM integrated probing system with four Tungsten probe  needles for device parametric extraction. The value of needle  resistance is less than 200 ohms. As shown in Fig. 4, I/V  curves were measured and we found N+/PW early junction  breakdown 100nA@6.5V compared with the voltage  100nA@11.5V of the reference. Besides, pull-down NMOS  circuits also show the same electrical failure signature, but  even worse. Based on these results, we have high confidence  that soft single column failure is caused by the failure of early  N+/PW junction breakdown at the Y-MUX and pull-down  NOMS circuits. With the failing transistor isolated, additional  physical analysis is focused on this component to understand  the failure mechanism.


N+/PW leakage contact


Barkside IR-OBIRCH


Backside MCT


Figure 3: C-AFM current mapping identifies failed N+/PW


File Name:MCT#S-3220x1 tif


contact.


Rem2:Camera=MCT 30sex 20x


125-07


-a-Fail


1.05-07-时


0.05-00


+


6.05-08


Currsent


40E-08


File Name:OB0S-3-20-AlLt


Figure 4: IV curves measured on contact level by Zyvex S100  Nanoprober with Keithley 4200 System. Curve ”Fail” is  N+/PW early breakdown at 100nA@6.5V compared with the  voltage 100nA@11.5V of Ref.


P-V and X-S TEM Analysis:


Since the failing transistor could be isolated, a sample is  prepared to do P-V TEM inspection of Y-MUX and pull47


down NMOS transistors. The results show that early N+ junction leakage is due to substrate dislocation as shown in  Fig. 5. With the higher magnitude of TEM images, dislocation  passing through the N+ junction, stretching across the P-Well  and ending at the STI bottom can be seen clearly, as shown in  Fig. 6. By the index of the thickness gradient of the Newton  ring, it can be estimated that the depth of dislocation is over  400nm and that it will further induce early N+/PW junction  leakage. X-S TEM is also performed in another sample as  shown in Fig. 5. Deep substrate dislocation of about 296nm in  the P-Well can also be found. Poor device performance  caused by substrate dislocation in Y-MUX and pull-down  NMOS circuits will induce soft single column failure. In this  case study, substrate dislocation is not visible with SEM or  FIB, however, it can be easily identified and isolated by the  way of internal probing, which leads to conclusive FA results. The origin of the substrate dislocation is suspected by pattern  sensitive. Through the process tuning, BL failure had  vanished in later dislocation-free lots.


Substrate dislocation


Figure 5: X-S and P-V TEM inspection at Y-MUX NMOS  transistor. It shows deep substrate dislocation at about 296nm  in a P-Well.


P-V TEM Images


Dislocation


STI


STIAA-￥


AA


Junction depth


Newton ring of thickness gradient


Figure 6: P-V TEM inspection at pull down NMOS transistor. It shows the dislocation passes through the junction, stretches  across the P-Well and ends at the STI bottom. The depth of  dislocation is estimated at 400nm.


The arrangement of FA tools and FA procedure is important  for the isolation of die level faults with complex failure  modes, especially for the soft single column failure, which is  possibly induced by multiform defects at various locations. In  this study, the substrate defect responsible for the fault is  successfully identified with a series of FA procedures, from  bit-mapping analysis, OBIRCH, and MCT to C-AFM as well  as nanoprobing analysis and eventually PFA. The failing area  is narrowed down along the way from a column to a single  transistor’s junction. Internal probing is utilized to  demonstrate the IV characteristic of early N+/PW junction  breakdown caused by the substrate dislocations at the Y-MUX  and pull-down NMOS circuits. It also gives not only  qualitative but also quantitative analysis of junction leakage.


X-S TEM Image


P-V TEM Image


[1] Jian-Chang Lin, Yung-Tsai Hsu, Chih-Kuo Huang, WuChin Tsai, and Yung-Hua Chou, “Investigation of  Substrate Dislocation Induced Bit Line Soft Failure”, 30th  ISTFA Proceedings, Nov. 2004, pp. 109-114.


[2] T. X. Tong, A. N. Erickson, “Current Image Atomic Force  Microscopy (CI-AFM) combined with Atomic Force


Y-MUX NMOS


Probing (AFP) for location and characterization of  advanced technology node”, 30th ISTFA Proceedings, Nov. 2004, pp. 42-46.


[3] L. Liu, Y. Wang, H. Edwards, D. Sekel, D. Corum,  “Combination of SCM/SSRM Analysis and Nanoprobing  Technique for Soft Single Bit Analysis”, 30th ISTFA  Proceedings, Nov. 2004, pp. 38-41.


48


The Effectiveness of OBIRCH Based Fault Isolation   for Sub-90nm CMOS Technologies


M. de la Bardonnie 1, R. Ross 2, K. Ly 2, F. Lorut 3, M. Lamy 3, C. Wyon 4,  L.F.Tz. Kwakman 1


1 Philips Semiconductors, 2 Freescale Semiconductor, 3 STMicroelectronics, 4 CEA-LETI  860, Rue Jean Monnet, 38920 Crolles, France


Yasushi HIRUMA


Hamamatsu Photonics K.K. System Division,


812 Joko Cho, Hamamatsu city, 431-3196, Japan


Jean Roux


Hamamatsu France


Buro Club MEYLAN, 29Bd des Alpes, 38246 MEYLAN, France


With the nanometre range feature sizes of today’s CMOS


technology, failure analysis of latest generation IC devices  faces several challenges in the fields of fault localization, deprocessing and physical characterization [1]. In a business  context of fast technology developments and ramp-up to  production volumes, our fault localization methods are based  on quick and -so far- effective optical beam techniques (OBIRCH, NB-TLS,…) operated in a static mode. Unfortunately, the success rate of these methods has dropped  as process complexity has increased when moving forward  from the 120nm to the 65nm technology node.


Even though failure analysis performed with a latest  generation Phemos 2000 OBIRCH tool has given excellent  results for 120nm and 90nm technology developments, the  limitations of tool and technique become apparent when used  for the 65nm technology node and beyond. First, the OBIRCH  localization accuracy decreases when more device elements  are heated under the laser spot, which is the case if the beam  size remains constant and the integration density increases (Fig. 1a). Second, with the feature size being far smaller than  the optical resolution, the lack of pattern image resolution also  becomes a serious show-stopper, which is especially true for  backside analysis (Fig. 1b). Third, the number of metal layers  becomes higher, top metal layers are preventing the laser beam  from penetrating to the bottom ones and detection of lower  level device failures becomes less evident (Fig. 1c and 1d). Finally, irreversible, heat induced device damage (see  observed contact and silicide breakdowns in Fig. 1e and 1f) occurs more easily in the latest technologies and, thus requires  counter measures such as scanning at lower laser power this in  turn reduces the detectability of the electrical defects.


To overcome the aforementioned problems and to ensure a  high Failure Analysis success rate for the latest technology


nodes, some new system options and alternatives have been  evaluated. One of the investigated options is laser modulation  at well defined frequencies in conjunction with a lock-in  current amplifier. The important gains in the signal to noise  ratio (S/N) that can be obtained with this approach are  expected to provide a number of significant improvements  and, thus the ability to isolate failures that cannot be detected  with our current OBIRCH set-up. The improved S/N ratio  permits detecting faulty circuitry with higher sensitivity and   reducing the incident laser power to prevent device damage  during the analyses. Furthermore, a higher spatial resolution  may be a well appreciated bonus of the altered heat dissipation  kinetics that results from the pulsing of the laser. Another  promising technique is the use of a numerical aperture  increasing lens (NAIL) also called solid immersion lens (SIL). In case of coherent illumination, e.g. when using a laser source  of wavelength λ, the spatial resolution that can be obtained  using the lens is inversely proportional to the numerical  aperture NA according to the theory of diffraction [2]:


d = 0.82 * λ / NA


[1]


The numerical aperture NA is defined as the product n.sinθ  where n is the refractive index at the focal point (device under  test) and θ the maximum collective angle of the objective lens. The theoretical numerical aperture of a hemispherical silicon  lens directly in contact with the silicon substrate is 3.4 (θ = 90°, nSi = 3.4) which has to be compared to a theoretical value  of 1 for the conventional optical set-up. Consequently, applied  to backside analysis, using NAIL provides higher pattern  spatial resolution and a smaller OBIRCH spot [3], thus a better  fault isolation resolution. The real improvements that this  technique -combined with the aforementioned S/N ratio  enhancements obtained through the pulsed laser and lock-in  amplifier- can bring to the failure analysis of latest technology  will be reviewed in the next chapters.


49


# The Effectiveness of OBIRCH Based Fault Isolation for Sub- 90nm CMOS Technologies


Figure 1: OBIRCH limitations - laser beam size vs. 65nm  SRAM cell (a), poor resolution backside pattern image (b), OBIRCH spots from same sample before (c) and after (d) removal of metal dummies, contact (e) and silicide (f) breakdown.


Experimental setup


The commercial Phemos 2000 tool used for this work is  equipped with both lock-in and NAIL features. It is equipped  with a double side prober (DSP), allowing front side and  backside analysis of 300 mm wafers or smaller sized samples.  Its laser source operates at a wavelength of 1.3 µm and  delivers a maximum power of 400mW. Four different  objectives are selectable for OBIRCH use in this  configuration: 5x, 20x, 50x and NAIL optics. The laser is  conducted from the source to the device under test (DUT) through fibre optics and objective. Two different analysis  methods, biased and non-biased thermal laser stimulation, are  practiced with the tool. With these methods, fault detection  relies on the measurement of the Optical Beam Induced  Resistance Change (OBIRCH) and of the so-called Seebeck  effect. Principle of OBIRCH is to apply a constant voltage to  the device under test and measure the current variation while  the circuit is scanned by the heating laser. When the DUT is


not biased (0V is applied), the laser heat can produce a voltage  at metallic junctions that act as a thermocouple (known as  Seebeck effect). These small voltages are monitored by the  tool with a highly sensitive voltage amplifier.


The laser scan speed can be selected from 1s up to 572s at a  512x512 pixel resolution. Multiple frames can also be  integrated at each scanning speed. A combination of laser scan  speed and frame integration can improve the localization  efficiency. Two different lock-in frequencies can be selected  with each operating at a fixed frame scan speed: 5 KHz and 50  KHz at 572 and 72s, respectively. The NAIL applied to the  backside of the DUT is a hemispherical silicon lens with a NA  of 2.5, which -compared to the standard 50x objective with a  NA of 0.76 - is believed to enhance the spatial resolution  significantly.


Lock-in amplifier: Basic principle


Lock-in amplifiers are used to accurately measure very small  AC signals in the presence of background noise using  synchronous demodulation [4]. In the OBIRCH technique the  lock-in amplifier is coupled with a modulated laser. The  pulsed laser beam induces a thermal modulation of the device  under test at the laser spot location which in turns induces a  current modulation if metal lines and/or conductive defects are  heated. This current variation can be very weak depending on  the current density and nature of the defect but with the lock-in  amplifier’s ability to better extract a small current signal from  background noise the sensitivity of the OBIRCH method can  be greatly enhanced using this configuration.


The main stage of the lock-in setup is a mixer where the input  signal, the heat induced current variation i(t) transformed into  voltage α.i(t), is multiplied with a reference square signal r(t) at laser pulse frequency f. It is basically realized with an  inverter and a switch (Fig. 2).  The resulting signal m(t) is lowpass filtered in order to get its average, or DC level. If the  input signal is not synchronized with the reference, as is the  case for noise, the DC level is zero. For a square signal  ranging between +1V and -1V, the reference signal can be  expressed as its Fourier series:


)


[


]


∑∞=


=


sin


)1


r


φ


ω


π


[2]


where ω=2πf and φ is the phase shift  between i(t) and r(t). The  output of the mixer m(t) can then be written as:


α


[3]


Whenever laser heat sensitive i(t) changes with laser pulse, its  frequency component in common with any of the components


Figure 2: lock-in principle


of the reference -its fundamental in the best case- contributes  to a phase sensitive DC component. The Phase shift φ can lead  to positive or negative DC values, and determines the  amplitude of the output level s(t). Because most of the noise  shares no common frequency with the reference signal, its  contribution to the DC output signal is almost negligible. Three types of noise are frequently encountered in the output  of an experiment (Fig. 3). Noise generated by power supply  lines at discrete frequencies (50Hz or 60Hz) can be eliminated  by choosing a suitable, much higher lock-in operating  frequency. Electronic components flicker noise (1/f) is also  greatly reduced by the relatively high reference signal  frequency. Random white noise (shot noise and thermal noise) is affecting the whole frequency spectrum but is effectively  limited by the small bandwidth of the lock-in amplifier.


To quantify noise and S/N ratios in our experiments we have  adopted the following evaluation method: the noise level is  determined from an OBIRCH image in an area outside the  analyzed structure. Its intensity is given by the standard  deviation σ of the signal from the average value in this area, ideally the median value of the analog to digital converter at  the output of the lock-in. The signal level is determined in a  small area where the spot is clearly visible and distinct from  the noise. The maximum intensity within this spot area is taken  as the value for the signal. The such defined signal and noise  levels are used for S/N ratio calculation.


Pulsed laser beam heating


When a continuous laser illuminates a device structure in a  given area the structure will heat-up until a steady state  situation is obtained in which the various elements (i) of the  device structure have a temperature T(i) determined by the  thermal properties of these elements (heat capacity, thermal  conductivity, reflectivity,…), the exact device geometry and  the applied laser power. The time that is needed to reach this  steady state temperature profile can be written as τ heat-up (x,y). Once the laser heating is stopped the device will cool-down to  ambient temperature in a given time τ cool-down (x,y).


If the continuous laser is replaced by a modulated laser, its


Log (Frequency)


→(Hz)


1/f noise


White noise


(a.u)


50/60Hz


Noise


bandwidth


W


of lock-in


Figure 3: Noise reduction by Lock-in amplifier set-up


beam switching frequency f and duty cycle and the heat  transfer kinetics will determine whether a steady state  temperature will  be reached within the ‘laser-on’ cycle and if  the device will fully cool-down to ambient temperature in the ‘laser-off’ cycle. Typical heat-up and cool-down times were  calculated by simulation for an aluminium line in a silicon  oxide environment on top of a silicon substrate [5], and found  to be in the order of 5-10µs. However, when considering  device structures with multiple metal layers the heat  dissipation kinetics are clearly more complex, and therefore, it  is more difficult to estimate exact values for   τ heat-up (x,y) and  τ cool-down (x,y). Nevertheless, from basic physics principles it  is evident that the heat-up of buried metal lines  (Metal line 1  in Fig. 4) is slower than for the metal lines close to the  illuminated surface (Metal line 3 in Fig. 4) and that the  opposite may occur for the cool-down when it is assumed that  cool-down primarily goes via the silicon substrate. Hence, although valid as an order of magnitude indication, the  reported time constants for a single aluminium line can not be  applied for a multi-level Copper metallization scheme. On one  hand, copper has a higher thermal conductivity (401 vs. 237  Wm-1K-1 for Al) and lower specific heat (0.38 vs. 0.90 Jg-1K-1   for Al), i.e. is a material which accumulates less energy and  transfers heat more easily. Consequently, copper heats and  cools down more quickly than Aluminium, but reaches lower  steady state temperature for a given absorbed energy. On the  other hand, the fact that defects can be present in metal levels  1, 2,…n, means that the laser stimulation has to last long  enough to sufficiently heat-up the defective layer. As is  qualitatively illustrated in Fig. 4, absolute temperatures in  metal 1,2, 3 do differ and as a consequence of this, buried  metal level 1 may continue to heat also after the laser has been  switched off, due to the temperature gradient between metal 1  and metal 3. If the laser pulse frequency is too high or the laser  duty cycle too low, buried layers will not be heated sufficiently  and, thus will the OBIRCH sensitivity for defects in these  layers be lowered. Hence, for optimum results with a pulsed  laser/lock-in-amplifier set-up, the laser pulse frequency and  duty cycle as well as the phase shift of the lock-in amplifier  have to be selected with great care.


The laser pulse frequencies that can be selected on the Phemos  2000 tool are 5 and 50 KHz that given a fixed 50% duty cycle, correspond to 100 and 10µs laser stimulation per cycle,


i(t)


m(t) rm,


Input waveform


- 1


Noise Power)Log(


+1 口


Reference waveform   controlling switch


+ -


R


Low pass filter


s(t) >


Inverter


mixer


r(t)


51


Laser  beam


Metal line 3 Metal line 2 Metal line 1


heat


Metal3


Metal2


Metal1


工刀


time


Duty cycle


Laser intensity


20% 50%


Induced metal1 current


20%


50%小


intensityLaserInduced currents intensity


Figure 4: schematics of laser induced current at different  depths in metal1 to metal3 (a) and for different duty cycles on  metal1 (b).


respectively. When using a 5 KHz pulse frequency, thermal  equilibrium, will most likely be achieved within one cycle. However, with the use of a 50 KHz pulse frequency, such  equilibrium is no longer evident.


Until here, only static laser stimulation has been considered. During an OBIRCH experiment, however, the laser is scanned  dynamically to probe a certain device area. Again, depending  on the selected scan speed, the heat-up of the device does  reach a steady-state and the scanning can be considered as a  succession of steady states, or is incomplete and during the  scanning the maximum temperatures are not achieved: for  example, at ‘standard OBIRCH‘ conditions, a 4s scan and a  1024x1024 pixels resolution means that the laser heats each  pixel during 2 µs (taking into account the blanking time), a  time that given what has been said before, might be  insufficient to properly heat the structure.


Finally, it is worth to mention that there is also an advantage to  a pulsed laser beam operated in non-equilibrium conditions. If  sufficiently high laser power is available, the local temperature  will rise significantly but due to the short pulse time the heat  does not propagate very far in lateral directions. Compared to  a continuous laser situation, the laser energy is absorbed in a  smaller region, which improves the localisation accuracy of the  defects present in the device structure. This effect will be  evident in the experiments described hereafter.


Signal-Noise ratio measurements


Experimental set-up


Samples A and B used in this work for assessing the efficiency  of lock-in amplifier and NAIL optics, are 120 nm CMOS


devices that contain various test structures. In sample A, a  poly-silicon serpentine test structure (0.13µm large, 0.18µm  spaced) showed anomalies due to incomplete silicidation that  were revealed by several OBIRCH and Seebeck spots of  varying intensity. The sample was mounted in a package and  backside polished to 100µm thickness. To withstand the  pressure of the NAIL optics exerted at the sample surface, the  mechanical support of a package is mandatory. In sample B, a  stacked contact-via1 chain showed abnormal characteristics  due to a poorly deposited level1 metal. To allow front- and  backside analysis, this sample was backside polished to 80µm  thickness and subsequently glued with wax onto a 280µm thin  glass plate. For the backside analysis, the laser beam has to  pass the quartz chuck and the glass plate to reach the backside  of the sample.


To allow comprehensive testing of the real benefits of the  lock-in amplifier, two complementary experiments were run. In the first experiment, sample A was subjected to biased (1V) and non-biased (0V) backside thermal laser stimulation with  and without using the lock-in set-up. In the second experiment, sample B was subjected to both front- and backside thermal  laser stimulation, at different bias voltages. Sample A has got  numerous faint spots in the OBIRCH image making this  structure interesting for visual comparison between OBIRCH  methods. Most of these spots are also picked-up by the  Seebeck method. In the structure of sample B the one or two  OBIRCH spots found are very sensitive to laser heat which  allows good S/N ratio measurements. Given its I-V  characteristics this structure can be comfortably tested in the  current range 0.1, 0.5 and 2µA at respectively 0.3V, 0.6V and  1V. In both experiments, the 50x objective was used. It is  optimized for the 1.3µm laser lens (NA=0.76). The two  samples were subjected to OBIRCH analyses with and without  lock-in. Without lock-in, an integration of 50 frames has been  chosen for sample A to get best S/N results at still reasonable  measurement times (200 seconds). An integration of only 5  frames has been chosen for sample B to get minimum signal at  reasonably low laser power. The scan speed was arbitrary set  to 4s (2, 4, 8 and 16s are selectable), and a 1024x1024 pixels  frame was selected to get the highest pixel resolution. With the  lock-in configuration the following settings do apply: lock-in  at 5 KHz, one 512x512 pixels frame scan in 572s, or lock-in at  50Khz, one 512x512 pixels frame scan in 72s.


Results and discussion


The Seebeck spots (NB-TLS) obtained on sample A with and  without lock-in at different laser power settings are shown in  Fig 5. Gray scale levels have been adjusted to enhance the  visibility of the spots from the noise. When comparing the  images for each applied laser power, it is clear that the S/N  ratio is much improved when the lock-in at 5 KHz is used. The  spot contrast at 35 mW without lock-in is roughly similar to  the spot contrast at 13.4mW with lock-in. Similar qualitative  results have been obtained when applying a 1V bias (OBIRCH  effect). This first experiment shows that the lock-in set-up is  indeed effective in improving the S/N ratio of the  measurements and that it does increase the sensitivity of  detection for both thermal stimulation methods.


52


Figure 5: Backside Seebeck pictures of sample A at different  laser power settings with and without Lock-in at 5 KHz.


S/N ratio measurements on sample B at various bias voltages  in front and backside configurations confirm quantitatively the  same trend. Working front-side, the S/N ratio gain obtained  with a 5 KHz lock-in setup varies from 2.5 – 4.5 depending on  the applied voltage but is not influenced by the laser power (Fig. 6a). In backside mode, this gain factor is even larger and  reaches a value of 10 (Fig. 6b). The 2 to 3 times higher noise  levels that exist when working in backside mode are  effectively suppressed by the lock-in setup. Surprisingly, when  the lock-in is set at 50 KHz the average gain factor drops from  10 to 5 (Fig. 6b).


The drop in S/N ratio gain observed when switching from a  lock-in frequency of 5 KHz to 50 KHz is dominated by a sharp  decrease in signal strength. As a matter of fact, although the  noise level is improved by a factor 8-9, in line with  expectation given the fact that the noise is averaged over 10  times more noise values per unit time, the signal level has  become 15 times weaker. This drop in signal strength can be  the result of either a too high laser pulse frequency (too short  pulse width) that is no longer matched with the thermal heat-up  time constant of the structure under test or of a not well  adapted lock-in amplifier phase shift between reference and  input signals. In the former case, the temperature rise during a  laser pulse cycle will be lower and no equilibrium will be  reached, in the latter case the available signal is not optimally  averaged and the DC value amplitude not at its maximum  value. From these experiments it is concluded that the use of a  pulsed laser and a lock-in amplifier does provide distinct  advantages for Failure Analysis on latest generation devices. At constant laser power an almost tenfold S/N ratio  improvement can be achieved which means that the sensitivity  to smaller defects can be significantly increased. Alternatively, at constant S/N ratio the laser power can be reduced by a  factor of 10, which may be needed to avoid irreversible device  damage. Such damage can be caused by a combination of a too  high laser power and a too high device current density (high V  bias).


Nevertheless, there are still several other ways to improve the  SNR in the OBIRCH tool without use of lock-in and without


Laser power (mW)


S/N ratio gain factor0 1 2


35mwl13.4mW39mN1.3mW*/


Lockin 5kirz


4HO


without Look in


5 6


5.7 7.8 10.6 13.4 16.5


日1V 日0.6V 0.3V


0 2


gain factorS/N ratio


4 6 8 10 12


5.7 7.8 10.6 13.4 16.5 19.6 lock-in 5KHz


lock-in 50KHz


Figure 6: S/N ratio gain factor obtained when using lock-in  amplifier vs. laser power. Front-side measurements on sample  B at 3 different voltages with 5 KHz lock-in frequency (a) and  backside measurements on sample B at 1V for 5 and 50 KHz  lock-in frequencies (b).


increasing the laser power. One of them consists of reducing  the scan speed of the laser. At ‘standard ‘conditions a 4s scan  and a 1024x1024 pixels resolution mean that the laser heats  each pixel during 2 µs. If the thermal time constant of the  structure under test is higher than this value this would mean  that the structure will not heat-up to an equilibrium  temperature but to a lower temperature instead. In that case  increasing the scan time will lead to a locally higher  temperature and thus a higher signal. Since the temperature  increase is structure and material dependant, simulation would  be necessary to accurately calculate it [5]. In this study we  have limited ourselves to just an experimental verification of  the influence of the scan speed on the SNR. The results  obtained on sample B are presented in Fig. 7. A weak  dependence is confirmed in this log-log scale representation  with an S/N improvement factor of 2.4 when going from 1 to  572s, the respective minimum and maximum laser scan speed  available on the tool. The gain is hence noticeable but remains  minor compared to the gains that can be obtained using lockin. These results will be further investigated.


Another “classical” way to increase the SNR is to integrate  multiple frames in order to average out the fluctuations due to  noise. Fig. 7 shows how much can be gained when going from  1 to ~ 500 frame integrations. The slope of the line in this loglog scale representation is 0.5, indicating square-root  dependence between the S/N ratio and the number of  integrated frames. This relation is valid for the two tested  resolution configurations (1024x1024 pixels, 4s per frame and   512x512 pixels, 2s per frame). Hence, a S/N ratio gain factor  of ~10 can be achieved when switching from a ‘standard’ 5  frames integration to a 286 frames integration, which for the  512x512 pixels resolution takes an equivalent time as the lockin set-up at 5 KHz, i.e. 572 seconds.


Even though it is demonstrated here that S/N ratio  improvements can be obtained equally well with simple frame  integration as with lock-in, it needs to be emphasized that the  physical mechanisms of the pulsed and continuous laser  beam  OBIRCH methods are quite different and that the pulsed laser


53


1000


10 100


Number of Frames


512x512 2s  1024x1024 4s


Scan Time (s)


|r  po we )Laser  speed Objective  (mW X and  (pixels) Number of frames Scan  20x lock ) Slow scan (2  per  frame  (s) Y resolution  objective -in  5KHz  (1 ) Structure for|r  po we )Laser  speed Objective  (mW X and  (pixels) Number of frames Scan  20x lock ) Slow scan (2  per  frame  (s) Y resolution  objective -in  5KHz  (1 ) Structure for|r  po we )Laser  speed Objective  (mW X and  (pixels) Number of frames Scan  20x lock ) Slow scan (2  per  frame  (s) Y resolution  objective -in  5KHz  (1 ) Structure for|r  po we )Laser  speed Objective  (mW X and  (pixels) Number of frames Scan  20x lock ) Slow scan (2  per  frame  (s) Y resolution  objective -in  5KHz  (1 ) Structure for|r  po we )Laser  speed Objective  (mW X and  (pixels) Number of frames Scan  20x lock ) Slow scan (2  per  frame  (s) Y resolution  objective -in  5KHz  (1 ) Structure for|r  po we )Laser  speed Objective  (mW X and  (pixels) Number of frames Scan  20x lock ) Slow scan (2  per  frame  (s) Y resolution  objective -in  5KHz  (1 ) Structure for|r  po we )Laser  speed Objective  (mW X and  (pixels) Number of frames Scan  20x lock ) Slow scan (2  per  frame  (s) Y resolution  objective -in  5KHz  (1 ) Structure for|r  po we )Laser  speed Objective  (mW X and  (pixels) Number of frames Scan  20x lock ) Slow scan (2  per  frame  (s) Y resolution  objective -in  5KHz  (1 ) Structure for|
|---|---|---|---|---|---|---|---|

|B |1024 |50 ||4 |50x |52/26 √||

|C |1024 |50 ||4 |50x |1.3 to 3.9 √||

|D |1024 |30 ||4 |20x |3.9 to 13.4 √||

|E |512 |30 ||4 |50x |1.3 √|√|

Figure 7: S/N ratio vs. frame scan time (bottom scale) and  number of frames (top scale) - measurements on structure B.


Figure 8: OBIRCH picture of metal line on sample C with (a) and without (b) lock-in at 5 KHz. The metal line contains  holes of varying size.


beam and lock-in amplifier set-up still have other distinct  advantages. The most important one, already mentioned  before, is the concentration of the laser heat in a smaller area  that leads to an improved localisation accuracy of the defects  present in the device structure. With the conventional  OBIRCH set-up, multiple integration of frames leads to  smeared out or inexistent spots. This advantage of a lock-in  set-up is apparent in Fig. 8 and further illustrated in the case  studies presented hereafter. To obtain the results of Fig. 8, a 3 µm large metal2 line (electromigration structure in sample C), has been locally FIB-cut down to the underlying oxide to  create square holes in its centre with sizes of 0.1 to 2.2 µm². This line has contacts on each side, so that OBIRCH voltage  can directly be applied to it. Acquisition has been done with  pulsed laser and lock-in at 5 KHz, (Fig. 8a, 1frame, 572s, 512x512pixels) and repeated with continuous laser without  lock-in (Fig. 8b, 50frames, 4s, 1024x1024 pixels). The edge of  the metal line appears more contrasted, revealing the presence  of the side wall barrier metal and gradients in the current


density, and the 5 FIB milled locations are also visible. The  spots at the hole locations are well defined in Fig. 8a but much  larger and less contrasted in Fig. 8b despite the better pixel  resolution. Hence, for this particular case the spatial resolution  is much improved thanks to the use of the lock-in set-up.


S/N Ratio


Case studies


In the remainder various case studies on latest technology  devices are presented to illustrate the interest of adding the  lock-in capability to the standard OBIRCH tool. The  experimental conditions applied are summarized in Table 1.


Table 1: OBIRCH set-up used for the case studies


(1) lock-in 5KHz: 512x512 pixels, 1 frame, 572s per frame


(2) slow scan: 512x512 pixels, 1 frame, 572s per frame


Case study 1


Structure D is made of 2 interlaced via1 chains in 65 nm  technology. The fabrication process was stopped just after  metal2 deposition and a thin encapsulating SiCN layer was  added to protect the structure against environmental defects. The structure on this particular sample is defective because of  the presence of an abnormal extra layer at metal1-via1  interface that is revealed in OBIRCH and non-biased TLS  analyses. The S/N ratio gain when using the lock-in set-up that  was already shown on sample A for 120 nm CMOS technology   is confirmed for the 65 nm CMOS technology as well (see Fig. 9). On this sample, the laser power can be decreased by a  factor of 2 to maintain the same S/N ratio (3.9mW vs.


7.8mW).  Another sample of this structure D was subjected to  a biased (1V, 180nA) OBIRCH analysis. Without the use of  the lock-in no defect could be detected at all, while running the  analysis with lock-in at 5 KHz did reveal the defective area  with a clear spot (Fig. 10). Subsequent physical analysis  showed that ~3µm large copper particles were at the origin of


54


Without lock-in


Lock-in 5KHz


13.4mW7.8mW5.7mW3.9mW


它


No lock-in


Not avalable


Frant side


Back side


Frant sidle


52mW


52mlW


26mW


50frames


1 frame


Figure 9: Backside Seebeck pictures of 65nm technology  sample D at different laser power settings with and without  lock-in at 5 KHz.


1.32.23.9


Laser power(mVW)


Figure 10: Lock-in enabled fault isolation.  OBIRCH spot  acquired at 1V, 180nA using lock-in at 5 KHz (a). No spot is  detected without lock-in set-up (b).


this electrical defect, since shorting metal2 lines. This example  is a convincing proof that by adopting the lock-in set-up our  FA success rate for the 65 nm CMOS devices can still be  improved.


Case study 2


If the test structure of sample B is analysed in back-side  configuration, OBIRCH detects a weak and a strong spot but  only at high laser power (52 mW) and a high number (50) of  integrations (Fig. 11b). Under otherwise similar conditions, the  weak spot is not detected when the sample is analysed in front  side configuration (Fig. 11a). However, when switching to the  lock-in set-up and using a 5 KHz pulsed laser with a power of  only 26 mW the weak spot can be detected and distinguished  from its neighbour equally well as realized before in back-side  analysis mode (Fig. 11c). Physical characterization revealed   that the smaller defect was localized in the bottom part of the  structure, an abnormal narrow metal line. This example shows  again an appreciable gain in fault isolation sensitivity when the  lock-in set-up is used. For this particular case where the defect  is buried under several metal layers and normally only (more  complex and time consuming) back-side analysis is effective, the gains are so significant that even front-side analysis  becomes feasible again. Hence, the sensitivity of the OBIRCH


Figure 11: Front and back-side analyses of structure B  without (a and b) and with (c) lock in set-up.


Std Obirch (a)


Lock-in 5KHz (b)


Figure 12: OBIRCH pictures of FIB modified metal line at  various laser power settings without (left) and with lock-in at  5 KHz (right). Used FIB pattern in middle.


technique for defects present in bottom metal levels is  considerably improved by using the lock-in set-up.


Case study 3


Similar to what has been presented before, another  electromigration metal line on sample C was FIB-cut at one  edge in two different locations in order to study the practical  heat spread effect on the spot resolution (Fig. 12). Using the  same experimental conditions as previously described for this  structure, the shape of the FIB cut is clearly observable -even  at the lowest laser power- using lock-in. In contrast, without  lock-in, no laser power setting was able to provide clear  borders of the cut despite the higher acquisition resolution  used. Apparently, the lateral heat dissipation is better confined  with the short laser pulses, and this leads to much sharper and  well-defined defect localization.


Case study 4


A defect on structure D is causing a large red OBIRCH spot  without lock-in (fig.13b) and a small green spot with lock-in (fig. 13a). Red and green colours correspond with positive and  negative laser induced current variation, respectively and are  indicative for the nature of the dominant defect in the structure  under test at the probed location [6]. However, this example


55


Figure 13: A specific defect  location on sample D provides a  small green spot with  lock-in 5KHz (a) and a blurred red spot  without lock-in (b).


Figure 14: FIB modified electromigration metal line (Structure E). Location of the modification on the layout (a), OBIRCH picture without lock-in scanning at 4s per frame (b) and at 572s per frame (c), with 5KHz lock-in at 572s per  frame (d)


shows that one has to be careful with signal interpretations  when a lock-in set-up is used. As was pointed out before, the  filtered DC lock-in amplifier output signal may be positive or  negative depending on the phase shift between the input and  the reference signals. Since a phase shift off-set is not user  selectable but fixed for each lock-in frequency at one more or  less optimized value by the equipment manufacturer, the exact  phase shift (and thus the amplitude and polarity of the output  signal) will be determined by the thermal delay time in the  structure, i.e. the time it takes from the start of the laser pulse  to a sufficiently heated defect(s) causing a measurable  resistance change. This delay differs for defects present at the


top surface and defects that are present in deeper, buried  layers. The deeper the defect is located, the later its peak  temperature is obtained and the lower this temperature will be (Fig 4). For this particular example where the lock-in  frequency is 5 KHz (100 µs pulse time), the observed signal  polarity change suggests that the  thermal time constant τ heat-up (x,y) for this particular structure and defect must be in the  same 50-100 µs range, and thus, that the defect is probably  close to the silicon substrate. (this is supported by the red  OBIRCH spot that typically corresponds to defects in silicon, silicides or barrier layers).


This particular case study provides a very valuable hint how to  further refine the OBIRCH analysis and to develop a method  to determine at what depth the detected defects are located: for  this it is needed to equip the tool with adjustable settings for  the laser duty cycle and the phase shift off-set and to measure  the OBIRCH signal at a defect location as a function of the


2.5μm


duty cycle or of the phase shift off-set.


70μm


Case study 5


hole


Structure E is a 110 nm large C65 metal line with a small hole  fibbed in its middle, close to a much larger metal line. When  OBIRCH at 4s per frame is carried out on this structure, the  hole appears as a dark spot characteristic of negative current  variation and the metal line is also visible, dark with less  contrast (Fig 14b). However, a white perfectly vertical line not  matching any particular structure is visible above and below  the dark spot and line. This white line becomes less contrasted  at very slow scan of 572s (Fig 14c). Using conventional  OBIRCH operation, the laser scans a line from top to bottom. This “tail” effect is very likely due to some kind of current  filtering issue at the output of the OBIRCH amplifier, the  slower a vertical line scan the less current instability occurs. Lock-in offers an extra advantage, this phenomenon totally  disappears with lock-in at 5KHz running at 572s per frame.


The use of NAIL in conjunction with OBIRCH


While the use of NAIL optics has been reported most often in  conjunction with (dynamic) light emission microscopy where it  significantly does increase the photon flux into the detector [7-9], this optics may also improve OBIRCH results given the  fact that the laser spot can be better focused and concentrated. Best results are expected when NAIL and lock-in set-up are  combined to concentrate the laser spot and to reduce the heat  spread, respectively. The real interest and benefits of such a  configuration have been evaluated with an experiment on  structure A in which the amount of separation of two  neighbouring defects (OBIRCH spots) was measured with and  without the use of the NAIL optics. Fig. 15 shows the  normalized OBIRCH spot intensities obtained with backside  laser stimulation without lock-in (top) and with lock-in at 5  KHz (center and bottom). The maximum peak intensities are  separated by 13 pixels when using the standard 50x objective  and by 50 pixels when using the NAIL optics, i.e. the


56


Figure 15: Normalized current intensity of 2 OBIRCH spots in  structure A with 50x lens without lock-in (top), 50x lens with  lock-in (middle)  and with lock-in and NAIL optics (bottom)


additional magnification factor is about 3.8 ± 0.2, from which  it is concluded that the NAIL optic are equivalent to a 200x  lens. More importantly, it is concluded that with the NAIL  optics each OBIRCH spot is better defined, sharper (30 % reduced FWHM) and better separated from its neighbour (50 % decrease in intensity between the two peaks). The resolution  improvement using NAIL is shown in Fig. 16 for a structure  containing metal lines of varying width and pitch (530 nm  down to 230 nm for both line and space). These metal lines are  resolved down to 330 nm in presence of the NAIL when only a  530 nm resolution is achieved with standard optics. Despite  the fact that the focus was not perfectly adjusted with the  NAIL optics, the obtained results are already very promising. Hence, the use of NAIL optics in conjunction with a lock-in  OBIRCH set-up can be considered as an helpful bonus.


Figure 16: Image of metal1 lines of various widths taken   backside with (bottom) and without (top) NAIL optics.


The various experiments presented in this study have shown  that OBIRCH based fault isolation in latest generation CMOS  devices can be significantly enhanced by using a pulsed laser  in combination with a lock-in amplifier. Using such set-up  with appropriate settings for laser pulse frequency, scan speed   and phase shift off-set, a tenfold S/N ratio gain is achieved. This improved S/N ratio permits to detect faulty circuitry with  higher sensitivity and to isolate faults that can not be detected  with the traditional OBIRCH set-up.


But it is the combination of S/N ratio and spatial resolution  improvements that makes the lock-in set-up really attractive. The higher spatial resolution is a well appreciated bonus of the  altered heat dissipation kinetics that results from the pulsing of  the laser. It is shown that the heat spreading is significantly  reduced even with a 5 KHz pulse frequency, suggesting that  thermal heat-up of the defects in the devices takes typically 10-100 µs.  “Freezing” the laser energy in a small, confined area  permits to improve the analytical sensitivity for buried defects  and to obtain sharper, smaller and better defined spots.


It is demonstrated that for optimal results with the lock-in setup it is necessary to be able to adjust the amplifier phase shift  off-set and/or the laser pulse duty cycle. From our experiments  it is believed that by monitoring the OBIRCH signal as a


57


function of phase shift off-set or duty cycle, information can be  obtained on the depth at which the defect is located.


Finally, NAIL optics are shown to further improve spatial  resolution and sharpness, especially when NAIL is combined  with S/N ratio enhancing lock-in amplifier.


The benefits of the pulsed laser, lock-in amplifier and NAIL  optics have been demonstrated in several case studies on real  120-65 nm device structures. With these added features the  OBIRCH technique is shown to be effective for fault isolation  in 65nm technology, however, whether it will be sufficiently  sensitive and accurate for the future 45 nm and beyond devices  still remains to be seen.


Acknowledgements


Part of the presented work has been realized in the framework  of European Eureka program Medea+ A407.


[1] Kwakman, LFTz. et al., “The role of a Physical Analysis  Laboratory in a 300 mm IC development & Manufacturing  Center”, proc. 2005 International Conference on  Characterization and Metrology for ULSI technology, Richardson, Tx, March 2005, to be published


[2] Born, M. and Wolf E., Principles of Optics, Cambridge  University Press (7th Edition), p. 471.


[3] Ikuo, A. et al., “Photoemission and OBIRCH Analysis with  Solid Immersion Lens (SIL)”, proc 29th International  Symposium for Testing and Failure Analysis, Santa Clara, CA, Nov. 2003, pp. 325-329.


[4] Mandelis A., “Signal-to-noise ratio in lock-in amplifier  synchronous detection: A generalized communications systems  approach with applications to frequency, and hybrid (rate  window) photothermal measurements”, Rev. Sci. Instrum. 65 (11), Nov 1994, pp. 3309-3323.


[5] Baudoin, F. et al, “Implementing Thermal Laser  Stimulation in a Failure Analysis Laboratory”, proc 27th  International Symposium for Testing and Failure Analysis, Santa Clara, CA, Nov. 2001, pp. 151-160.


[6] Ross, R. et al, “OBIRCH driven Failure Analysis for  Process Development of 120nm to 65nm technology nodes”, proc 30th International Symposium for Testing and Failure  Analysis, Worcester, MA, Nov. 2004, pp. 447-450.


[7] Fletcher D.A. et al, “Near infrared imaging with a  microfabricated solid immersion lens”, Applied Physics letters  77 (14), Oct 2000, pp. 2109-2111


[8] Welzman, Y. et al., “VLSI design for functional failure  analysis in the <90nm and flip-chip era”, proc 29th  International Symposium for Testing and Failure Analysis, Santa Clara, CA, Nov. 2003, pp. 184-190.


[9] Ippolito S.B. et al, “High spatial resolution subsurface  thermal emission microscopy”, Applied Physics letters 84 (22), May 2004, pp. 4529-4531


58


Dislocation related Leakage in Advanced CMOS devices


Frank Siegelin and Anton Stuffer


Infineon Technologies AG, Munich, Germany    frank.siegelin@infineon.com,


With high implant doses, strained silicon technologies and


shrinking feature sizes, dislocation related failures seem to  gain more importance in advanced CMOS devices. On the  basis of case studies, different types of dislocations as well as  the electrical characteristics of the corresponding devices will  be presented.


Dislocations have long been known as a root cause for defects  in semiconductors. Especially when they are crossing the p/njunction of a device, leakage currents are a well known  mechanism  [1] [2]. Regarding the formation and promotion of  dislocations, process induced mechanisms have been identified  as major contributor  [3] [4]. E.g. the ion implantation processes  used for the formation of source, drain and well regions of  CMOS devices. Unfortunately, these implantations are  creating point defects and causes a lot of crystal damage  [5].


Subsequent annealing steps are introduced to repair these  damages, but still there is a chance for crystal defects to  remain close to critical areas of the completely processed  device. Especially high accumulated stress built up during the  formation of the shallow trench isolation (STI), oxidation or  gate stack formation promotes the formation of crystal  defects  [6].


The formation of stress induced dislocations is known to be a  two step process. It starts with the nucleation of a dislocation  loop which is the result of "precipitations" of the excess  interstitial population that exists after ion implantation


[7] [8] [9] followed by subsequent growth into critical regions  of a device. Ion implantation, oxidation process steps and gate  stack formation are major contributors to this behavior. With  the aid of finite element simulations, the dislocation dynamics  can be predicted for certain device structures  [10] [11]. In  addition, the doping of the substrate increases the velocity of  dislocations in comparison to undoped silicon  [12].


Electrical characteristics of devices can be indirectly or  directly affected by dislocations. They can change the point  defect concentration around the loop layer by emitting  [13] and capturing  [14] interstitials, thus causing enhanced/retarded  dopant diffusion.


In n-doped material, dislocations behave as acceptors. In ptype silicon they show a donor-like behavior  [12]. This  mechanism leads to the formation of a leakage path following  the propagation of the defect. Hence, if a dislocation reaches  into the p-n-junction of a device, it can increase the leakage  current when it lies across the device junction  [5] or finally  result in the total electrical failure of a device  [7].


In order to understand the mechanisms of the formation of  dislocation as well as their influence on device characteristics, detailed imaging of these defects is essential. Methods like xray topography and chemical decoration are commonly used to  show the positions and distribution of dislocations. But, these  techniques have a major drawback for in depth analysis since  they cannot give sufficient information about size, orientation  or type of the defect.


The most effective tool for detailed analysis of dislocations  and crystal defects is the transmission electron microscope (TEM). By using various operation modes like e.g. brightfield, dark-field or weak-beam imaging size, position and  orientation of a dislocation can be determined. Imaging under  various tilt angles can be employed as well as advanced  preparation techniques  [15] to get a 3-dimensional impression  of the defect.


The objective of the work presented here is to make a link  between the structural information about the defect and the  electrical characteristics. Different types of dislocations  characterized by their position, size, shape and orientation are  correlated and with the resulting change in the electrical  characteristics of affected devices. The electrical part of the  analysis, curve trace measurements mainly on contact level, were used to get I-V curves for source-drain- or diffusion-well  diode characteristics or leakages measurements, respectively.


59


# Dislocation related Leakage in Advanced CMOS devices


Case Studies


In the present work, three different types of dislocations are  discussed: (i) long ranging dislocation dipoles, (ii) stress  induced crystal defects and (iii) small dislocation loops.


(i) Dislocation dipoles


TIVA


The example for a long ranging dislocation dipole is from a


device which failed due to increased pin leakage. In this case,


the position of the fail was localized by backside emission


microscopy as well as by TIVA. The position of the failing


device was located within the ESD structure of the pad. TEM-OverviewSubsequent surface parallel delayering was performed to gain  direct access to the failing device. After FIB pad deposition,


the diffusion-to-well characteristic of the failing transistor was


measured and compared to a reference. Figure 1 shows the


ohmic leakage characteristic that was found for the affected gate


diffusion.


80


gate


2 μm


Voltage [V]


1.0 Figure 1: Diffusion-well characteristic generated by the  dislocation dipole shown in figure 2. In this case, a relatively  high leakage with an ohmic component in the zero-volt region  was found.


After localization and electrical characterization, a plan view  TEM sample of the area including the failing device was  prepared. After total lift-off by wet chemistry, further  preparation followed standard methods comprising mechanical  polishing and subsequent ion-milling. Figure 2 shows the  image from the localization as well as the corresponding TEM  micrograph. In this case, two dislocation dipoles, each longer  than 2 µm, were found right at the position of the TIVA signal. After additional thinning of the sample, the more detailed  bright-field and dark-field images in figure 3 show the exact  position of the lower dipole. It was found that the upper end of  the dislocation is reaching the top of the substrate in the gate  area. Imaging at various tilt angles shows that the defect is  inclined and reaching down towards the well. Due to the  additional thinning, in figure 3 the lower end of the dislocation  dipole is cut away, compared to the overview in figure 2.


Taking into account that along the propagation of a dislocation  a leakage path is opened  [1] [4], one can easily link this defect  to the measured IV-characteristic. In this case, the long  ranging dislocation dipole reaches from the diffusion down to  the substrate, thus opening the measured leakage path.


Figure 2: Plan view TEM image and the corresponding TIVA  image (different scale) of the failing device. The localized


Current [uA]400.0


TIVA signal directly corresponds to the position of the  dislocations.


-80


Figure 3:  Detailed plan-view bright- and dark-field TEM  images of the lower dislocation dipole shown in figure 2.


(ii) Stress induces crystal defects


As an example for a stress induced defects, the second case  study presents the analysis of single cell SRAM fail. In this  case, no elaborated localization procedure was necessary, since the position of the defective cell is well known from  descrambling the logic address of the failing bit. After surface  parallel delayering to contact level, all transistors of the 6TSRAM cell were characterized by measurements with the  atomic force prober (AFP). As shown in figure 4, source-drain  leakage was found for one n-FET within the SRAM cell.


0.2 µm


60


Figure 4: The dark lines correspond to the characteristics of  the failing device (red line) shown in figures 8. In this case, the transistor shows source drain-leakage, while no leakage to  the well was found. In comparison, the bright lines show the  characteristics of a reference transistor.


Since no gate leakage was measured and the diffusion-well  diodes were without any objection, a sample for TEM cross  section imaging was prepared.


TEM cross section imaging of the failing transistor showed  another typical type of crystal defect. As shown in figure 5, a  dislocation crossing the device from source to drain was  found. In order to estimate the position of the dislocation in ydirection, the sample was tilted around the z-axis. In figure 6  the sample was tilted by 25 degrees with respect to the edge-on  orientation of the gate. It can be seen that the defect is crossing  the channel at the level of the source / drain contact.


Figure 5: Cross section TEM image of a stress induced  crystal defect imaged at 0° tilt angle. In this case the  dislocation is spanning the device from source to drain.


Figure 6: Cross section TEM image of a stress induced  crystal defect imaged at 25° tilt angle. In this case the  dislocation is spanning the device from source to drain.


In this case, it is assumed that locally built-up stress is the root  cause for the generation of a defect at this specific position. Again, the dislocation induces a leakage path along its run  which results in the leakage characteristic shown in figure 4.


(iii) Dislocation loops


The third type of crystal defects discussed in this article are  small dislocation loops. The case study selected as an example  for this effect was coming up with a bit-line oriented failure in  the diffusion-type read-only memory (ROM). Coarse  localization of the failing cell was performed by backside  emission microscopy. The position of the emission spot in  combination with descrambling information from the known  bit-line reduced the number of fail candidates to a few. After  delayering to contact level, AFP measurements were carried  out on the pre-selected contacts. An increased leakage from  the diffusion contact to well was found for the failing ROMcell in comparison to a reference. The corresponding IVcharacteristics are shown in figure 7. In contrast to the other  types presented, no ohmic component was found in this case. At lower reverse bias voltages, the current measured is still  comparable to a good device. A minimum threshold voltage is  needed to get sufficient leakage.


61


Figure 7: IV-characteristics measured from the central  contact in figure 3a to well. The failing device (red line) shows  reduced Uth and leakage in reverse bias.


By focused ion beam (FIB) lift-out technique, a TEM sample  was prepared for cross-section imaging. The overview image  of the failing device is shown in figure 8, where a small  dislocation loop beneath the gate was found. More detailed  bright and dark-field imaging in figure 9 reveals the position  and the size of the dislocation. It is located a few nanometers  beneath the gate oxide and has a maximum diameter of about  30 nm.


100nm


Figure 8: In this case, cross-section TEM imaging shows a  dislocation loop in the channel of the failing transistor.


Figure 9: Detailed bright-field (BF) and dark-field (DF) image of the dislocation loop in the channel region. The size  of the loop is ~ 30 nm.


With the dimensions found, the dislocation cannot cross the


channel of the FET completely. Again, assuming the leakagepath model along the defect, the resulting electrical  characteristic in figure 7 can be explained. The effect of this


dislocation is comparable to a shortened gate length, since the  leakage path brings source and drain closer together. Finally, the electrical signature results in a reduced threshold voltage


04


of the failing transistor.


] [uACurrent


1-09


.02


3.0


In the case studies presented, three different types of  dislocations were found in failing devices processed in  advanced CMOS technologies. The dimensions of these  defects are ranging from long, line shaped dislocation dipoles  spanning several micro-meters to 30 nm dislocation loops. Comparing the morphology of the defects with the  corresponding electrical characteristics, a consistent model can  be proposed. The electrical behavior of the three cases can be  explained by the assumption, that a leakage path along the  propagation of the dislocation is created. This correlation is  emphasized by the summary of the findings given in table 1. It  shows how the type and the size of the defect are linked to the  electrical characteristic of the failing device. Reading this table  in the other direction, the type of defect can be deduced just  from the electrical curve trace measurements.


transistor 2


transistor 1


Based upon several case studies, the link between leakage path  and defect position has been emphasized by electrical  characterization and subsequent TEM imaging of failing  CMOS devices. As summarized in table 1, this understanding  of the correlation between the defect and its electrical footprint  can help to classify and identify dislocations. Therefore, having a detailed electrical characterization of a failing device


dislocation-loop


with respect to leakage paths and threshold voltages, a forecast  of the type of defect responsible can be given. This  understanding can help to reduce failure analysis turn around  time. Especially, since it reduces the need to analyze  dislocations by time consuming TEM analysis. The  classification of the defect can be performed by standard curve  trace measurements. In suitable cases, the identification of  dislocations can even be performed with inline screening  methods  [16].


Table 1: Summary of the electrical characteristics compared  with the type of dislocation found.


|case |type of dislocation |defect size |I-V characteristic|
|---|---|---|---|

|i |dislocation dipole |≥ 2 µm |diffusion-well leakage |

|ii |stress induced, ranging from source to drain |~ 400 nm |source-drain leakage |

|iii |dislocation loop in channel region |~ 30 nm |reduced Uth in reverse bias |

万


刁


I-V characteristic


BF


DF


50 nm


dislo a=25.6 deg


62


The author is indebted to Christof Brillert for providing the  failure localization and the electrical measurement data of  some of the examples shown


[1] Whelan, M., “Leakage currents of n/p silicon diodes with  different amounts of dislocations”, Solid-State  Electronics, Vol. 12, (1969), pp. 963-968.


[2] B. O. Kolbesen and H. P. Strunk, “Analysis, Electrical  Effects and Prevention of Process-Induced Defects in  Silicon Integrated Circuits”, VLSI Electronics  Microstructure Science, Academic Press (1985), pp. 143-222.


[3] Dellith, M.; Booker, G.; Kolbesen, B.; Bergholz, W. and  Gelsdorf, F., “A dislocation formation model of trenchinduced dislocations in dynamic random access  memories”, Journal of the Electrochemical Society, Vol. 143, No. 1, (1996), pp. 210-215.


[4] Garth, K.S.; Chen, Y.H. and Stephens, A.E., “Effects of  Dislocation and Bulk Micro Defects on Device Leakage”, SEMICON, Taiwan (2001).


[5] Miyake, M. and Takahashi, M., “Defects Induced by Deep  Preamorphization and Their Effects on Metal Oxide  Semiconductor Device Characteristics”, J. Electrochem. Soc. Vol. 144 No. 3 (1997), pp. 1020-1024.


[6] Fahey, P.; Mader, S.; Stiffler, S.; Mohler, R.; Mis, J. and  Slinkman, J., “Stress-induced dislocations in silicon  integrated circuits”, IBM Journal of Research and  Development Vol. 36, No. 2, (1992) 158-182.


[7] Li, J. and Jones, K.S., “311 defects in silicon: The source  of the loops”, Appl. Phys. Lett., Vol. 73, No. 25, (1998), pp. 3748-3750.


[8] Avci, I.; Law, M.; Kuryliw, E.; Saavedra, A. and Jones, K., “Modeling extended defect (311 and dislocation) nucleation and evolution in silicon”, J. Appl. Phys., Vol. 95, No. 5, (2004), pp. 2452-2460.


[9] Ibrahim Avci, “Modeling the Nucleation and Evolution of  Dislocation Loops in Silicon during Annealing and the  Effects of Mechanical Stress on Dislocation Loops”, PhD  Thesis, University of Florida, 2001.


[10] Izumi, S.; Sakai, S.; Miyake, T. and Ohta, H., “Application of three-dimensional dislocation dynamics  simulation to the STI semiconductor structure”, Mater. Sci. Eng. A, Vol. 395, No. 1-2, (2005), pp. 62-69.


[11] Ohta, H.; Miura, H.; Tamaki, Y.; Ikeda, T.; Hashimoto, C. and Ikeda, S., “Fabrication process design of dislocationfree semiconductor devices by using stress singularity  parameters”, J. Soc. Mater. Sci., Japan, Vol. 50, No. 3, (2001), pp. 303-308.


[12] Patel, J.R.; Testardi, L.R. and Freeland, P.E., “Electronic  effects on dislocation velocities in heavily doped silicon”, Phys. Rev. B, Vol.  13, No. 8, (1976) pp. 3548-3557.


[13] Huang, R.Y.S. and Dutton, R.W., “Experimental  investigation and modeling of the role of extended defects  during thermal oxidation”, J. Appl. Phys., Vol. 74, No. 1 (1993), pp. 5821-5827.


[14] Liu, J.; Law, M.E. and Jones, K.S., “Evolution of  dislocation loops in silicon in an inert ambient-I”, SolidState Electron. Vol. 38, No. 7, (1995),, pp. 1305-1312


[15] De Veirman, A., ”3-dimensional' TEM silicon-device  analysis by combining plan-view and FIB sample  preparation”, Mater. Sci. Eng. B, Vol. 102, No. 1-3 (2003), pp. 63-69.


[16] Baltzinger, J.; Desmercières, S.; Lasserre, S.; Champonnois, P. and Mercier, M., “E-beam inspection of  dislocations: Product monitoring and process change  validation”, in IEEE International Symposium on  Semiconductor Manufacturing Conference Proceedings, (2004) pp. 359-366.


63


Contacting Diffusion with FIB for Backside Circuit Edit – Procedures and  Material Analysis


U. Kerst, P. Sadewater, R. Schlangen, C. Boit,


TUB Berlin University of Technology


Einsteinufer 19 Sekr. E 2, D-10587 Berlin, Germany


+49-30-314-28518; fax: +49-30-314-25526; e-mail: uwe.kerst@tu-berlin.de


R. Leihkauf


HMI Hahn Meitner Institut Berlin, SE1, Kekulestr. 5, Berlin D-12489,Germany  B. Simmnacher


Infineon Technologies AG, Balanstr.73, Munich D-80598, Germany


T. Lundquist, E. Le Roy


Credence Systems Corporation, 1421 California Circle, Milpitas, CA 95035, USA


The feasibility, of low-ohmic FIB contacts to silicon with a  localized silicidation, was presented at ISTFA 2004 [1]. We  have systematically explored options in contacting diffusions  with FIB metal depositions directly. A demonstration of a  200nm x 200nm contact on source/drain diffusion level is  given. The remaining article focuses on the properties of FIB  deposited contacts on differently doped n-type Silicon. After  the ion beam assisted platinum deposition a silicide was  formed using a forming current in two configurations. The  electrical properties of the contacts are compared to furnace  anneal standards. Parameters of Schottky-barriers and thermal  effects of the formation current are studied with numerical  simulation. TEM images and material analysis of the low  ohmic contacts show a Pt-silicide formed on a silicon surface  with no visible defects. The findings indicate which process  parameters need a more detailed investigation in order to  establish values for a practical process.


The backside approach to FIB circuit edit becomes  increasingly mandatory because of C4 (FlipChip) packages as  well as on chips with many interconnect layers. For editing  circuits with very small transistor dimensions (below 100nm) it would be desirable to edit on silicon at the diffusion level  directly. To avoid going up one level to the poly-silicon or  first metal level, the FIB contact would connect through the  silicon to an existing contact from either the poly-silicon or  M1. Alternatively the silicon can be contacted directly by  forming a silicide between FIB deposited platinum and silicon. This capability will open up a new horizon in the circuit edit  world. The critical issues to be addressed are


1. Contact resistance as a FIB deposited interconnect to


silicon form a rectifying Schottky barrier, and


2. Endpointing within silicon with accuracy much better


than 50nm.


The feasibility of a process for low ohmic contact resistance  has been demonstrated recently using a local contact forming  procedure [1].


Process Options


Contacting diffusions requires a trench of an area larger than  1µm2 that endpoints on the STI level [2]. From there, as  illustrated in Figure 1, two major alternatives exist to contact a  highly doped diffusion area (typically source/drain) directly: Option 1 requires stopping the mini-trenching of the node  access hole within silicon when the highly doped area is  reached. Source/drain diffusion regions typically do not reach  below 50nm in current technology generations. This degree of  endpoint accuracy, while milling the node access hole is  difficult to achieve. Furthermore, inherent to FIB deposition, the thickness of the amorphization layer below the deposition  produced by Ga+ ion implantation is of this same order of  magnitude—50nm. Consequently this process needs further  investigation once the basic contact forming conditions are  under control.


Currently Option 2 is a promising procedure: Usually a  diffusion area is connected with multiple manufactured IC  contacts to an upper metal layer. Hence connecting to one or


Silicon  Substrate


Option 1


Option2


FIB Trench


S T I


ILD


Figure 1: Contacting diffusion. Option 1: Editing trench for contacting diffusion stops in silicon.


Option2: Editing trench stops on contact


64


# Contacting Diffusion with FIB for Backside Circuit Edit – Procedures and Material Analysis


more, but not all of the contacts provides an indirect  connection to the diffusion through the upper metal and  untouched contacts on the diffusion. The FIB node access hole  stops on the IC contact level, which can be easily done due to  endpoint from the increase of secondary electron emission  when the ion beam hits the contact material. The access hole is  positioned with a slight offset away from the gate. The  remaining portion of the diffusion closest to the gate maintains  the proper connection to the device. Figure 2 is a  demonstration of the Option 2 process into a 130nm  technology device. It is clearly visible that the size of the FIB  trench is similar to the minimum device features. The  electrical contact was deposited directly onto the metal plug  that fills the contact to diffusion, and it was as low ohmic as  any other contact from FIB deposited conductor to an  interconnect metal.


will be improved, and the requirement of high aspect ratio  holes will be diminished.   But reliably forming a broad level  plane, a consistent, repeatable distance above active circuitry  takes considerable technique development.


The process typically starts with the global mechanical  removal of the majority of the silicon substrate, down to less  than 100um of remaining material as described above.  Local  trenching of usually no less than 100um x 100um is then  performed at the navigation fiducial locations (optional), and  the repair site itself.  A high partial pressure of XeF2 and a  high beam current are used to achieve acceptable milling rates  over the large area.  The process of high volume silicon  removal is a simultaneous combination of beam driven and  spontaneous chemical etching [2].


Obtaining a uniform beam driven XeF2 etch rate across these  selected regions is critical in order to achieve a flat bottom  hole, and is at least partially dependent on the top surface  quality of the silicon at the start of the mill.  Achieving this  requires that a mirror smooth finish be applied to the starting  surface after the mechanical preparation.  Once in the FIB, the  surface is further cleaned and prepared by gas etching with a  non-fluorine precursor, such as bromine or an iodine  compound.  If these steps are skipped, non-uniformities  propagate and are amplified during the volume silicon  removal.  This will result in an uneven floor, and will promote  early punch-through into the active region, with the strong  possibility of device damage.


During the trench etch process, the operator must carefully  monitor the thickness of the remaining silicon to establish a  real-time location in Z-space.  There is little room for error, as  stopping accurately a few microns above the active region is  essential.  Trench mill endpointing is one of the most difficult  aspects of backside FIB on bulk processes.


One of the most accurate ways is thru the use of a laser OBIC  system.  This requires some elaborate hardware setup, including the ability to monitor ion beam induced current flow  from selected pins on the chip.  The output is a graphical  signature that suggests when the mill is nearing break-through  into the active region.  Still, it tends to leave about 3um of  material remaining [3].  Unfortunately, this is one technique  that does not seem to work effectively with SOI.


The most common method employs use of an in-situ NIR  optical microscope, either located off axis within the chamber, or resident within the ion column itself.  True thickness  measurements of the remaining silicon can be obtained by  multiplying the actual z-travel of the microscope objective by  the silicon index of refraction.  Unfortunately, this requires  repeated and time-consuming interruptions of the milling  process to make optical depth measurements.  The  measurements themselves are not particularly accurate, with  errors of +/- 3um being typical.  Note that 3-5um is the  desired final thickness of the silicon at the work plane, so the  final moments of trenching can be perilous!


79


Trench floor uniformity and flatness during the mill can be  determined by monitoring optical interference fringes  produced while imaging by NIR narrow band illumination.  This technique is extremely useful for monitoring and  preventing sudden punchthru into the active region should a  small spot be etching faster than the rest.  Corrections to the  mill pattern can be applied to help even out the floor [4].  Unfortunately, as shown in Figure 2, no amount of beam or  gas correction will result in a totally flat floor.  Invariably, the  trenching will have to be halted leaving several microns of


Remaining Bulk Silicon


backside silicon remaining over the target area in order to  avoid damage nearby.


Once the milling has terminated at the work plane, the  remaining silicon above the active region must be stabilized to  establish a suitable work surface.  An oxide deposition over  the entire exposed silicon region will prevent further attack  during subsequent targeted mills.  It is also an essential step in  order to provide the electrical insulation required between any  deposited metal lines and the naturally conductive silicon  substrate.


Navigation accuracy is compromised when attempting FIB  repair from a raised floor.  Local lock points can be drilled  down to unused structures, but again, the vertical distance is  large.  Even minor amounts of drift during the extended  drilling period can result in severe targeting inaccuracies.  Employment of one of the drift compensation methods  designed to improve accuracy during long milling periods is  recommended.


Another preparation and imaging technique has been reported  that induces a voltage contrast effect capable of highlighting  N-well implants in grounded p-type substrates [5].  The  primary purpose is as an alternative to the laser stage 3-point  lock by allowing a more direct visual CAD overlay alignment  to circuit features.  While this technique has merit, the spacial  resolution (and thus overall alignment accuracy) may in some  cases be limited by the relative size of these wells in  comparison to the actual circuit features to be targeted.  A  reported secondary use of induced voltage contrast is for  trench mill endpointing, as the strength of the signal is  proportional to the silicon remaining.


Any actual circuit access will require a high aspect ratio  drilling approach, as the thickness of the remaining silicon  floor must be factored into all modifications.  One can  anticipate the aspect ratio to be different at each point across  the trench floor, as a total thickness variation of several  microns or more can be expected.  In addition to insulating the  floor, the drill regions thru the remaining silicon must also be  filled / lined with oxide and redrilled prior to metal deposition  to prevent shorting to the substrate along the sidewalls.  Obtaining an accurate endpoint signal at the bottom of these  holes can be difficult.  All of this extra detail work will have  to be factored into the repair zone layout, as beam chemistry  actions at one node can have a profound effect on another site  in close proximity.  With the small, high aspect ratio drills


required by the tight geometries on today’s products, none of  this is easy to achieve.


Figure 2 FIB cross section of backside (silicon side up) contact to diffusion in 130nm technology, process Option 2 by  end-pointing on the diffusion contact


Generally process Option 2 is not as versatile as Option 1  though, and as features are getting much smaller, Option 1 is  gaining in importance. So, a more flexible approach requires  the technology of FIB contacts to diffusion within silicon.


Experimental Setup


Although the contact to diffusion procedure mainly targets  backside processes, basic evaluations were performed from the  front side because access is easier after polishing off the high  level metal layers. The contact size was 1µm x 1µm. Two test  structures have been used. The first structure was a solar cell  where a contact was placed directly onto the moderately  highly doped (front side) n-type emitter (peak concentration ~1019 atoms/cm3) region with ~1µm penetration depth. A  regular aluminum pad served as the counter electrode. To first  order the current flow was two dimensional [1]. The purpose  of this structure was to evaluate contact formation on  moderately doped regions with little risk of punching through  the emitter diffusion layer. The other test structure was a 130


nm process rectangular resistor defined by the STI boundary. The resistor received n+ source/drain implants but no silicide  formation. The penetration depth and peak level concentration  were not known but typically are ~1020 atoms/cm3 and 90nm  respectively. This test structure provided a quasi 1-dimensional current flow and the risk of punching through the  shallow diffusion was higher. The end pointing was based on  material contrast change in the end-point tool [3], which  evaluated average SE image brightness over time.


The thermal treatment consisted of either a well controlled  furnace anneal for reference purpose or a self heating of the  system driven by DC current to provide local (Joule) heating  which would not destroy package/chip integrity as would  furnace anneal on functional circuits. The current can either  flow through the access hole as illustrated in Figure 3 or just  flow parallel to the access hole by forcing a current along a  deposited Pt stripe between two probe needles. The latter is an  easier and more general procedure but does not directly create  heat where it is most needed for forming a contact—the Pt-Si  interface.


Figure 3: Circuit for electrical forming and 4-point  measurement of test structure resistance


Alternatively heat can be provided from a laser – experiments  are still on going.


Contact Formation Modeling


Device modeling was 2 dimensional which is appropriate for  the resistor structure but the modeling neglected lateral current  spreading to the much larger aluminum pad. However for a  qualitative understanding the error from current spreading is  not critical since the heat spreading description lacks well  defined parameters (see below). We used the semiconductor  modeling package DESSIS for the calculations. The device  was assumed to be electrically connected through 1µm  diameter probe needles and to be thermally adiabatic (probe  needle does not extract heat) e.g. all heat spreads out in the  device. In a 25nm thick Si-layer near the Pt-Si interface a 3  orders of magnitude higher electrical resistance was assumed  to account for the high resistivity of a contact as deposited. The area, that was simulated, ranged from -2000 µm to +2000 µm from the contact and extended 2000 µm into the substrate. The contact opening was 1µm in the covering SiO2 ARC  layer. DESSIS has no model for Joule heating in metal  interconnects, so formally the metal was replaced with Si, but  the above-defined properties were inserted. For Si and SiO2  default parameters were assumed [4] for both electrical and  thermal modeling. Whereas the default parameters were  established little is known about the thermal properties of the


I


Pt


SiO2


AL


SiO2 electrical barrier


65


deposited platinum. Usually in metals there is a relationship  between the electrical and thermal conductivity (WiedemannFranz law). However FIB deposited platinum consists of  substantial percentages of carbon and other impurities such  that the resistance is much higher than that of pure platinum


[5][6] and the assumptions of the Wiedemann-Franz law are  not expected to be met. Applying the Wiedemann-Franz law to  obtain the heat conductivity of FIB deposited Pt films from  electrical data leads to a very poor heat conductor – much  more thermally insulating than for example SiO2. Consequently the simulation result shows an insufficient  temperature increase at the Pt-Si interface to form a silicide (temperature below 400C) when forcing the current through  the platinum layer parallel to the interface.


x [µm]


-1


-0.75


-0.5


-0.25


0.25


0.5


1273 1023 823 623 473 423 383 372 369


Figure 4: Stationary heat distribution [°K] with 1.15mA  forming current and thermal conductivity according to  Wiedemann-Franz law


As illustrated in Figure 4, the heat mostly spreads through the  interfacial SiO2 between the substrate and the deposited Pt  and out into the substrate. The maximum temperature in the  deposited layer is already at 1000 °C while little heat reaches  the Pt-Si (dotted in Figure 4) junction. However, this was not  consistent with the experimental results in which we saw a  morphological change in the contact forming region before  and after current formation. To obtain a realistic (but not  exact) parameter for our simulations, we arbitrarily increased  in the simulation the thermal conductivity input parameter by  a factor of 5x and 50x, which lead to much higher  temperatures in the Si-Pt interface region. If, however, the  temperature exceeded the silicidation temperature by a couple  hundred degrees in the simulation volume the device is likely  to be destroyed locally at that particular point. Using, in our  experiments, conditions as simulated, we have not observed a  destructive process. Figure 5 depicts these simulated  temperatures at the Pt-Si junction as well as the maximum  temperature in the whole simulation area. Only the curves for  a 50x increased thermal conductivity lead to a sufficient  warming at the junction without reaching excessive  temperatures anywhere else e.g. in the deposited platinum  layer. Hence we fixed an enhancement factor for the thermal


conductivity in all other simulations in this discussion. We  certainly would prefer a more direct determination of the  thermal conductivity of FIB deposited Pt but the small volume  of FIB deposits makes it very difficult to obtain.


_100


D


1.0


1.5


2.0


I [mA]


◆


白


T_Inter X1 T_Max X1 T_Inter X5 T_Max X5 T_Inter X50 T_Max X50


Figure 5: Simulated temperature at the Pt-St interface (T_Inter) and maximum temperature (T_Max) within the  entire simulated area with multiples of thermal conductivity as  per the Wiedemann-Franz law


Electrical results


The electrical resistance was measured using Kelvin probing  with a “safe” (no forming) current level each time after  annealing at a higher current. Unlike previous experiments [1] the contact size was maintained after annealing (no geometry  degradation). The reference anneals in the furnace indicated a  resistance drop at about 400-500 C (see Figure 6).


0,0 0,1 1,0


x


10,0


100,0x 1000,0


300


400


500


600


T.Anneal [°C]


K1x1 K1x1.A


Figure 6: Resistance of deposited contacts after furnace  anneal over anneal temperature for a 1 µm2 contact


On the moderately doped n-type sample (Figure 7) a Schottky  Barrier was formed before annealing and a diode behavior  resulted. After sufficient current formation driven through the  contact at the Pt-Si interface, the annealing occurred and the  resistance was lowered dramatically.


Forming current I (through probe needle)         I


66


-1E-5-5E-6 0E+0 5E-6 1E-5


Voltage across contact [V]


Figure 7: Resistance lowering on moderately n- doped silicon


after current driven anneal (1 µm2contact)


On the highly n-doped (see Figure 8) sample the resistance  was ohmic from the beginning and only slightly improved  after a current anneal parallel to the Si interface. The high


doping concentration allowed tunneling and thermionic


emission across the Pt-Si barrier [7] (PtSi-Si barrier after  anneal). Experimentally platinum-silicide formation for low  ohmic contacts was demonstrated in 1982 [8].


-40X-30


-20


I0


-0.15


-0.05


0.05


0.15


init ial 4.3kΩ


post  500µA 4.5kΩ post  5mA 2.7kΩ


post  10mA 2.7kΩ


Figure 8: Resistance lowering on highly n-doped silicon(1µm2  contact) after current anneal (note curves include portion of  diffusion sheet resistance)


Pt-Si FIB Contact Processing


A Schottky barrier between highly n-doped silicon and FIB  deposited Pt has been investigated with numerical simulation  using DESSIS. Figure 9 shows simulated I-V curves for four  silicon doping levels from 1.5x1019cm-3 to 1.5x1020cm-3. In  this range the transition from rectifying to ohmic contact was  apparent e.g. the potential barrier in the silicon narrows to  allow tunneling. Our own measurements on test contacts to  silicon with doping levels of approximately 1-3x1019cm-3  supports those simulation results. 1.5x1020cm-3 is a realistic  doping level in the diffusions of a modern technology. But  approaching the diffusion from the backside, the effective  doping level at contact is less predictable. Furthermore, the  amorphization layer from the ion beam operation deteriorates


the electrical properties. Silicidation may overcome both  problems:


1. The amorphized layer may recrystallize after cooling


below the eutectic temperature which overall improves


the electrical properties and reorganizes the Pt-Si interface  in particular.


2. The barrier height of the Pt-Si contact drops by 50meV


[9].


Current [μA]


3. The doping level at the contact may be modulated by the  additional dopant material, the metal component of the


silicide, drawn into the silicon to solubility level at the  eutectic temperature [10].


-0.4


-0.35-0.2


-0.1


w


0.1


0.3


Junction Voltage [V]


1.5e19cm^-3 3e19cm^-3 6e19cm^-3-0-1.5e20cm^-3


Figure 9: Numerical simulation of Schottky barrier I-V-curves  for doping levels from 1.5x1019cm-3 to 1.5x1020cm-3


Current Driven Local Contact Formation


To understand the heat flow during the previous experiments a  time resolved device simulation has been performed. The  forming current was turned on instantaneously and the heat  spreading observed. Since the heat conductivity of the  deposited platinum was not known but plays a major role, the  results were qualitative in nature. Assuming the 50x higher  thermal conductivity than expected from the WiedemannFranz law (see discussion above) the process is still limited by  poor heat transfer. The silicon acts as heatsink with a very  high thermal conductivity. The heat transfer across the thin  SiO2 electrical barrier between the substrate and the deposited  Pt layer around the node access hole was fairly large. As  desired, the Joule heating was mainly created along the path  from the probe needle to the contact hole (see Figure 3) due to  the high resistivity of FIB deposited conductors. Instead of  being conducted to the contact hole and assisting silicidation, heat drained across and through the SiO2 film directly into the  substrate and was lost for local contact processing. In Figure  10 the current is injected from the upper left side and heat is  generated in the relatively poorly conducting FIB deposited Pt  layer. Over time the heat spread out but no clear preference  towards the contact was visible. Centering the current source  helps as indicated in Figure 11. A higher heat conductivity  than assumed will enhance the heat transfer to the silicidation  region.


forming current level [µA]  10, 50, 100,


500, 5000


10µA


5mA – 1.3 kΩ


500µA


-5 ，


- 0


-3


67


-5


-1-0.75-0.5-0.25


1-10


-1-0.75 0-0.5-0.25


-1-0.75


-0.5 E-0.25


Figure 11: Steady State qualitative heat distribution with asymmetric (left) and perfectly centered current source


TEM and Material Analysis


The contact microstructure has been exposed to TEM and  subsequent material analysis.


20nm


Figure 13 TEM image of FIB contact to diffusion as deposited. Below Pt-layer amorphized silicon by Ga implant (.~30nm  thick)


Figure 12: Cross section of FIB contact through dummy


metal on diffusion resistor after silicidation (forming


current parallel to the interface)


Figure 10: Heat spreading after 1, 2, 4, 7, 10 ms, Pt on top. Qualitatively, the Joule heating (bright is warm) spreads out from the


upper left corner, where the current flows in (probe needle) into the volume, easily passing through the SiO2 region


Pt-Si Interface


SiO2   Pt


1ms


2ms


4ms


7ms


10ms


68


Figure 12 displays a contact processed on a highly doped ndiffusion resistor after FIB Pt deposition and subsequent local  ohmic contact formation. In the TEM micrograph of a contact  as deposited on moderately doped silicon (Figure 13) the  amorphized layer of Ga implant into silicon is clearly visible  and has a thickness of ~30nm.


Figure 14: TEM image of Pt-Si-contact after driving the  forming current through it. 34nm-layer of recrystallized Pt, 20nm layer of Pt-silicide (see EDX in Figure 15)


The structure looks very different in Figure 14 after having  applied the forming current and the low ohmic character has  been verified. Two layers can be distinguished in the TEM  image whereas the amorphized zone disappeared.


The two layers have been checked for their respective  composition in material analysis by means of EDX (Energy  Dispersive X-ray Spectroscopy). The two spectra are  superimposed in Figure 15. The black 34nm layer is very  much recrystallized Pt with a Ga residual. The 20nm layer  looks like a silicide where the EDX profile identifies a strong  silicon peak in addition to the Pt signal.


lid


line) 20nm layer of Figure 14


The silicide layer does not display any defects in the TEM  image and has a lower Ga content compared to the layer  above. The ohmic contact properties are therefore determined  by the platinum silicide on a highly doped low defect Si  surface.


An effective contact to diffusion process can be established by  endpointing the FIB trench on the contact to diffusion. Presently connecting manufactured contacts (plugs) is an


34 nm


option. In the future a contact to Si based on local silicidation  is feasible. For a proper silicide formation between Pt and Si a  forming current will heat the contact to ~500C. Further  understanding of the thermal properties of FIB deposited


20 nm


platinum will help to optimize the annealing process. The  contact properties after proper formation are expected to  resemble a platinum silicide with a reduced gallium  contamination and a low defect Si crystal lattice with no  residual FIB amorphization damage. Given the material mix in  the system after deposition this is a very promising result.


100 nm


Acknowledgements:


Special thanks go to Andreas Eckert (TU-Berlin) for the  sample preparation, Claudia Keller (Infineon FA Munich) for  providing packages and Matthias Bauer (Infineon Dresden) for  providing the diffusion resistors.


Appendix:


Overview of simulation parameters


ρ(Pt-FIB) = 5*103µΩcm @ (300°K)


κ (Pt-FIB)= 1.465 mW / (°K cm)


κ5X (Pt-FIB)= 7.2 mW / (°K cm)


κ50X (Pt-FIB)= 72 mW / (°K cm)


Schottky Barrier model for tunneling current simulation:


Barrier height: 0.85eV (PtSi/n-Si)


Electrical carrier mobility: doping depended Masetti-model; E-field depended high field saturation (DESSIS default)


Pt Si


[1] C.Boit et al, Proc. 30 ASM-ISTFA (2004) 331


[2] C. Boit, U.Kerst, R. Schlangen et. al, Proc. ITC (2005)


[3] OptiFIB Users Guide Credence Corporation


[4] DESSIS 7.0, ISE AG, Zürich, CH (2001)


[5] A.J. DeMarco and J. Melngallis, J. Vac. Sci. Technol. B  19(6) (2001) 2543


[6] K.A. Telari, B.R. Rogers et. al., J. Vac. Sci. Technol. B  20(2) (2002) 59


[7] Rhoderick, Emlyn H., Metal-Semiconductor Contacts. - Oxford : Clarendon Pr. (1980)


Ga 90Ga atPt


[8] S.S. Cohen, P. A. Piacente et. al., J. Appl. Phys. 53(12),


(1982) 8856-8862


Ga


[9] Sze, S.M. Physics of Semiconductor Devices, p.293 John


why


P. Wiley (1981)


|2.00|4.00|6.00|8.00|10.00|
|---|---|---|---|---|

|Figure 15: EDX overlay of (fill) dark 34nm layer and of (so |Figure 15: EDX overlay of (fill) dark 34nm layer and of (so |Figure 15: EDX overlay of (fill) dark 34nm layer and of (so |Figure 15: EDX overlay of (fill) dark 34nm layer and of (so |Figure 15: EDX overlay of (fill) dark 34nm layer and of (so |

[10] C. Boit, F. Lau and R. Sittig, Appl. Phys. A 50 (1990) 197-205


69


Novel and Practical Method of Through Silicon FIB Editing of  SOI Devices


RK Jain, TR Lundquist, ME Antolik, MA Thompson


Credence Systems Corp, Sunnyvale, CA


Circuit edit techniques have been developed for silicon-oninsulator (SOI) devices using a coaxial photon-ion column. Novel trenching, navigation and milling methods, utilizing sub  pico-Amp beam currents provide enhanced capability for


D=129(xs)nm


editing devices with decreased geometries including buried


D=59 (xs)nm


(Box) thickness. Flat trenches 200x200µm were obtained


工


using real time optical fringe monitoring with 125nm accuracy


D-420(as)YFUC


with 950nm λ and FIB bit map milling to adjust for


D=194 (xs) nm


parallelism to the ILD0.  This bit map milling technique  controlled the etch rate to maintain trench flatness by  correlating the optical fringes to the bit map grayscales to vary


D=274(xs)nm


the dwell time of the ion beam across the trench floor.  Through highly accurate, CAD directed beam deflection


D=199(xs)nm


control, beam placement accuracy in the sub 20nm regime can  readily be accomplished, sub pA beam currents provide ultraD=312(xs)nm


controlled etch rates and high aspect ratio (HAR) capability.


Complete process definitions, techniques and results are  reported. These techniques have proven successful in circuit


D=318(xc)nm


edit below 90nm, and are expected to meet future technology  circuit edit requirements down to 45nm.


D=161(2s)nm


D=269(xs)nm


D-183(xs)nm


The cost of and time for mask reworking is increasing with  decreasing technology nodes. Circuit edit of semiconductor


D=307(xnm


devices is a great benefit [1] and its value to the IC industry  need not be lost.  As the number of IC metallization levels has


D=339(xx)nm


increased the difficulty of FIB editing has increased.  Then


with the advent of flip-chip packaging it became obvious that


through silicon editing was required for IC development to


continue. On flip-chip and planarized front side devices


navigation to the circuit node of interest is difficult because et


1 μm


the FIB can only see surface features.


SOI (silicon-on-insulator) CMOS devices unlike traditional  CMOS devices comprise a layer of silicon dioxide, buried  oxide (BOx), which insulates the bulk silicon from the active  silicon. Charge sensitivity is higher in SOI devices where  discharge paths are for the most part unavailable through the  BOx unlike the bulk silicon in regular CMOS processes [4].


Figure 1.Cross-section image to obtain layer thickness  information of Inter layer metal and dielectrics. The


information helps determine etch rate and dosage


Charging on the BOx can alter the threshold voltage (VT) of  charge sensitive gates [3]. Traditional CMOS through silicon  circuit edit recipes will not work on SOI devices due to lack of  n-well and shallow trench isolation (STI) structures in the bulk


70


# Novel and Practical Method of Through Silicon FIB Editing of SOI Devices


silicon [4].  Emphasis herein is put on novel trenching, navigation and milling methods. The Credence IDS OptiFIB  was used to perform all the work presented in this paper.  Tell  the readers what type of FIB system is utilized.  The devices  investigated were purchased on the open market so we did not  have access to electrical testing information on them. However, the device manufacturer was able to provide us with  very limited CAD information for the purposes of this paper.  The devices were cross-sectioned to determine the thickness  of the layers in them (Fig. 1).


DUT Preparation


The initial bulk silicon thickness was measured as ~750 µm.  Devices were globally thinned down to ~30µm, using a  lapping wheel. The final polish on these devices was done  using a 1µm silica slurry. The resulting surface finish is  required for uniform silicon removal and for a good optical  image in the FIB (Fig. 2).


35um6


Figure2.  Optical image through globally thinned silicon  enables CAD alignment through polished silicon without  milling seeker holes


In SOI devices, the layer of silicon dioxide insulates the active  silicon from the bulk silicon. Generally, this bulk silicon  cannot be connected to ground through the bumps. A good  ground connection is required for all FIB operations.  After the  final polish silicon was connected to ground using silver paste.


Fringe direction


The paste was conveniently contacted to the grounded sample


Substrate


holder.  The silver paste was removed using Acetone after the  edits were completed [2].


Global Navigation


Due to the lack of topography on the surface of polished


Interference creates fringes


silicon, the ion beam is unable to detect any features to  facilitate device to CAD alignment.  Rather than milling  seeker holes [5], real-time near-IR optics of the coaxial  photon-ion column readily enabled a CAD alignment through  the polished silicon (Fig. 2)[9]. A three-point CAD alignment


allowed a quick navigation to the area of the edit to begin  trenching.


Final Silicon Removal or Trenching


The polished silicon was locally thinned down using the FIB.  For thermal reasons [10] local trenching to the BOx is  required rather than global thinning. A 200x200µm trench was  started using a 20nA, 30keV beam.  The ion etch was  enhanced by using in-situ XeF2 gas [7].  From characterization  the depth etch rate for this 200x200 µm trench was determined  to be 1.5 µm /min.  (This rate included adjustments for lack of  trench floor co-planarity with the ILD0 surface.)  After 16.5  minutes the trench was stopped at ~5 µm from the actives (equation 1).


BC


ness


FinalThick


Thickness


Initial


etch


Rate


Etch


Time


−


--- (1)


Equation (1) Equation to calculate etch time


The beam current and energy were then dropped to 4nA and  15 keV respectively.  As a result, the etch rate was reduced to ~0.5 µm/min.  Lowering the beam current and energy not only  allowed greater control on the etch rate but it also reduced the  charge dosage and the Ga+ penetration into the trench floor.  All of which were very important to reduce the risk of  penetrating or damaging the thin barrier oxide (BOx) layer of  the device [2].  After ~7 minutes of trenching the FIB images  were closely monitored in the deepest point.  The direction of


optical fringes indicated the deepest point in the trench (Fig. 3a, 5a). These fringes were monitored simultaneously during  the FIB trenching operation using the photon-ion column. The  fringes moved from the thinnest point of the silicon to the  thickest point on the trench floor (Fig. 3a).  Using a “Bit Map  Milling Technique”, explained later in this section, the slope  of the trench was significantly reduced (Fig. 5b).


sio,


BOx


Figure 3a.  Direction of fringe movement with respect to a  relative slope of the trench floor


71


At the first sign of break through to the BOx, an in-situ, spontaneous Si-etch process with XeF2 without the ion beam  was utilized to remove any remaining silicon.  This was done  to avoid or minimize BOx exposure to the ion beam.


SiO2e5


Ion Beam


Dwell time increase


Direction of Fringe Mavement


Figure 3b.  Variation in dwell time to compensate for the lack


of trench floor co-planarity—more ions are striking the


thicker Si than the thinner.


Maintaining and controlling trench flatness to the highest  degree is also very important to reduce the risk of damaging  the BOx.   A “Bit Map Milling Technique” (BMMT) was  developed to control the etch rate and maintain trench flatness  by correlating the optical fringes to bit map grayscales by  varying dwell time of the ion beam across the trench floor (Fig. 3b). The photon portion of the coaxial photon-ion  column was used to monitor the trench flatness to ~½ fringe  spacing or 125nm accuracy with a narrow band 950nm  Interference Fringes


Lightλ'p-p州


wavelength (Fig. 4).


Dark


Thicknessλ2131 4m4m4m


Figure 4.Illustration of Peak-to-Peak calculation in  interference fringes


p 2


λλ =− ,


index


refractive


m =


= 1.9 for silicon


λ p-p = 249nm


--- (2)


Equation (2) Distance between fringes using 950nm λ


The correlation and correction of the slopes were done  manually. The slope was determined through the fringes in the  optical image, which was then used to adjust the dwell time  and thus corrected the slope.  The trench co-planarity to ILD0  was controlled and monitored from the beginning at 30µm Si  thickness.  The fringe intensity became stronger as the  remaining silicon in the trench floor thinned down.  The fringe  intensity was useful in qualitatively estimating the remaining  silicon thickness.  Data on the fringes of these trenches and


BOx over etch were collected.


Figure 5 Optical image of a trench floor using 950nm, narrow  band λ  while local thinning (a) contains 6 fringes indicating  a slope of 1494nm (b) corrected to1.5 fringes or a slope of


373.5nm


72


Optical Navigation to Seek Local Alignment  Targets


The non-etched BOx thickness was measured at ~129nm (Fig. 1).  Once the BOx was exposed, the trench floor was optically  imaged using 500nm wavelength (Fig. 6). [The 950nm light  does not see very well though the BOx because the BOx  thickness of 129nm is close to the 125nm at which first  interference occurs (See Fig. 4).]  Fine adjustments to remove  any offsets between the optical and FIB images were  performed.  The optical image enabled <350nm box placement  accuracy through the trench floor in milling to alignment  structures near the periphery of the 200x200µm trenches.


All SE (secondary electron) FIB imaging operations at this  stage were performed using sub-pico-Amp beam currents to  minimize both charge effects on the surface of the BOx as  well physical damage to the BOx. Appropriate box sizes were  used to mill down to first metal structures.   Alignment  structures with both X and Y components were chosen to  increase the accuracy of the alignment. Data on beam  placement accuracy was acquired.


Figure 6.  Optical image using 500nm λ  through BOx


enables <350nm BPA for milling local alignment holes.


Local alignment


Increased navigation accuracy and navigation speed within the  200x200µm trench were accomplished with an electronic  stage emulation [6].  The FIB system contained a single  injector (jet) chemistry delivery system. The jet was moved  into its injection position before aligning the electronic  deflection stage so as to avoid any beam deflection issues after  jet movement.  Three local alignment openings were used to  provide a more precise fit between the CAD and the DUT by  compensating for DUT tilt, DUT warpage, process tolerances, or magnification correction.  Devices are not made to absolute  but to relative dimensions, therefore, absolute positioning is  insufficient for accurate FIB placement; i.e., placement must  be according to the relative dimensions of the actual IC die


rather than the absolute positions of the idealized die. Inherently there was no advantage to this except in the faster  speed of emulated travel and in an improved consistency of  positioning accuracy.  The real advantage, however, was the  ease of relative calibration.  The deflection field was not  calibrated to absolute position but to relative position as  defined by the IC die under test.  Distortions across the die can  be locally corrected by a simple recalibration of local die  dimensions.  Alignments were performed at various  magnifications to gather data on the accuracy of this electronic  stage.


Essentially an X-Y mechanical stage is emulated with  precision X-Y electronic deflections. This electronic stage  utilizes a static deflection field about which the scanning field  is centered. Normally the scanning field is centered about the  beam 0,0 position—the position at which no voltage is applied  to the beam deflection plates.  By using three small field, high  resolution, single frame alignments, accurate beam placement  is achieved with the precision electronic deflections. This is  accomplished by increasing the working “field of view” by  means of local sub-images; i.e., by allowing CAD overlay to  be registered to alignment points that are located outside the  selected field of view with each alignment point accomplished  by a local registration to some feature within the local subimage (Fig. 7).  By precisely calibrating a static deflection  movement to local x.y alignment targets of the DUT, the  scanning voltage can be summed to this static deflection  voltage and thus the scanning center is moved precisely to this  new calibrated center. Alignment accuracy depends on the


号


location of the structure with respect to scanning center; the  closer the targeted area is to the center of the dynamic  deflection field the better the stage accuracy.  Minimal error


张


occurs within a 200x200µm operation field, i.e., the center of  the large area alignment field with a gradual degradation  towards the limits of the field allows users flexibility in noncritical situations to trade off throughput with precision.


Any repositioning of the beam appears instantaneous, as no  mechanics are required. The mechanical stage is not allowed


35*


to move when using this electronic stage. The precision of  movement depends entirely on local alignment to the DUT.  Alignment to smaller features increases the precision of the  stage.


Emulation of an X-Y mechanical stage with precision X-Y  electronic deflections yielded greater than 300x300-micron  deflection fields with 0.1-micron accuracy. The consistent  positioning accuracy and calibration ease enables verification  of probe-tips during mechanical probing and accurate  placement of design modifications.


Milling Operations with sub-pA Beam Currents


The local alignment points were quickly verified at high  magnification.  The sub-pA beam currents control the sudden  discharge events by decreasing the cumulative ion dose  delivered during operations near active circuit elements [2]. Sub-pA beam currents provide ultra-controlled etch rates and


73


high aspect ratio (HAR) milling capability. Controlled etch


220T


rates are essential for small technologies with decreasing


thickness of metal (Cu) and inter layer dielectric (ILD) there is


180+


increased risk of over-etching these layers [8].  A very


100 efficient secondary electron detector was used [11].   The 0 milling operations to M2 for the vias were performed using


1201


200x200nm boxes.  The operations were stopped based on the


image or more importantly secondary electron detection end


point curves (Fig. 8).


40-


*品品888R88


time <s>


up to 300x300µm


Figure 7.  Illustration of the Sub-Image Alignment Algorithm  for registering and accurately overlaying the CAD database to  the FIB generated image over a large area.  The order of the  alignment points is not important.


Reliable cutting of metal (Cu) lines in small boxes is also very


0,54cm


important in circuit edit operations.  An M1 line was isolated  in 500x400nm boxes using 500fA beam currents and OptiFIB  Cu etch chemistry.  Beam placement was centered on the M1  of interest.   The tightly spaced (200nm) M1 lines on the top  and bottom were exposed to the left and right to demonstrate  isolation of the target M1 line (Fig. 9).  The isolation of the  M1 of interest was demonstrated using endpoint and passive


180-200


voltage contrast in the FIB (Fig. 10,11).


200 8x


The 200x200µm trenches had anywhere from 1 to 6 fringes


60-


(Table 1). The peak-to-peak fringe distance was ~250nm


while using a 950nm wavelength (Equation 2). Therefore, the


slope of the trenches varied from 250nm to 1500nm from the


time(s)


0。98徐S6828a员9


deepest to the highest point.  The variation in slopes may be  attributed to the timing of correcting the slopes, as slope  corrections were carried out manually.


M2


-Alignment


Invisible


Target 2


Hidden


Figure 8.  Endpoint curve of a 200x200nm box to M2


Traces


2.5x2.5μm Registration Sub-Image 3 places


女Selected


2.5x2.5μm


Field of View FIB Milling Box


Alignment


Cut 1


Cut 2


/Target 3


Target 1上Registration Area


Target


M1


Figure 9. Target M1 Cu line exposed. Top and bottom Cu  lines were intentionally exposed to the left and right of the  target to evaluate Cu etch re-deposition.


220


M 1 c u t2


160+


M 1 c u t1


Figure 10. End point curves for Cut 1 and Cut 2 boxes.  A  sharp decline towards the end of each curve indicates the  completion of the cut operation.


74


Sometimes the operator allowed a trench slope to develop to  1µm before dwell times were changed.  An automated  correction routine would provide a tighter control of the slope. Also, the edges of the trenches had higher density fringes.  This could be attributed to higher gas density at the edges of  the trench.  This could also be controlled by an automated  correction routine as well.


a2


Target  M1  is0油eIsolated


0,75km


Figure 11. Passive voltage contrast image of the target M1 Cu  line confirmed electrical isolation of the line


Over etch into the BOx was measured from 3 to 25nm across  the trench (Table 1). The over etch happened in areas where  the BOx was first exposed during the final silicon removal (Fig. 8). Uniform Si removal and accurate end pointing to the  BOx minimizes the over etching of the BOx.  Minimizing  over-etch of the BOx is critical for the subsequent milling and  imaging operation required in a circuit edit operation.  The  lesser the over etch into the BOx the further away the ion  beam during imaging operations. Automating the Si removal


E-BeamSpot | Tilt | Mag |FWD| Det


500mm


process should reduce the over etch.


On the other hand stopping ~1 um away from the BOx maybe  one option.  However, a quantitative and repeatable end point  procedure will have to be developed to consider this option.  By using interference fringes in optical information channel  accurate end pointing to 1µm thick Si during final silicon  removal can be developed.  The remaining Si will also add  considerable amount of time to the edit, as it will need to be  electrically isolated and isolated from fluorine damage by  using in-situ insulator deposition [4].  Furthermore, any  thickness of material on top of the box will add HAR  complications to small box operations.


The beam placement accuracy (BPA) of the ion beam using  the optical image measured between 310 to 100nm (Fig. 13).


Measuring distances at very high magnifications between the  target structure and the structure that was actually opened  determined the BPA.  This BPA greatly depends on the final  through silicon alignments performed by the user.  Also, for a  given set of calibrations the BPA depended on the geometries  of the target structure.  If the target structures were isolated or  unique the BPA appeared to be better.  This may be due to the  fact that the user’s ability to target a unique and isolated  structure improves as opposed to targeting a repeating  structure or dense structure.


TABLE 1.  Trench and BPA data


|Results |Results |Results ||
|---|---|---|---|

|Parameter |Samples |Avg. Min |Max |

|Fringes |8 |3 1 |6 25nm |

|Over-etch into BOx |6 |8nm 3nm |310nm |

|Optical (BPA) |9 |200nm 100nm |310nm|

|Electronic stage (BPA) |9 |10nm 5nm |37nm |

D=122 (xs) nm


Figure 12.  Over-Etch 7nm


Figure 13.  BPA examples using optical image


(a) BPA: 310 nm (b) BPA: 100nm


75


Alignment structures with unique optical properties can be  engineered into the silicon for the purposes of editing [1].  Incorporation of color in the optical imaging may also help  yield better optical BPA.


The BPA of the FIB using the electronic stage emulation  ranged from 37 to 5nm (Fig. 14). The BPA was a function of  the accuracy of the electronic stage local alignments.  Higher  the magnification used during alignment the better BPA was.  The draw back of using higher magnification was that the ion  beam etched the alignment structures that were being used.  That is why sub-pA beam currents were very useful for high  magnification alignments (Fig. 15).  The alignment accuracy  also depended on the sizes and geometries of the alignment  structures.  Finer structures with X and Y components yielded  better results.  It may be useful to incorporate fine dummy (grounded) alignment structures [1] with X and Y component  to make full use of the electronic stage.  Old alignment targets  may be swapped with new structures that are opened as  operations move outward from the center of the deflection  field.  Box drift due to charging can also contribute to lower  BPA, however, sub-pA beam currents helped eliminate any  charging effect.


D-3R2000.


D-2


100V353.0100kX4.835 TLD-SLO KV3


53.0?100 kX4.836TLD-S


(a)                                         (b)


Figure 14. BPA examples using the electronic deflection stage


(a) BPA: 37nm  (b) BPA: 5nm


Successful through silicon circuit edit techniques on new  generation SOI devices using coaxial photon-ion column were  developed and described.  The optics enabled faster navigation  to trench sites without drilling fiducial sites for global  alignment.  We were able to apply optical techniques to edit  positioning <350nm accuracy.  The optical element was a  crucial stepping-stone for achieving a consistent BPA of 10nm  from the FIB.


A new BMMT technique for trenching, using the optical  component of the column, was developed to control the slope  of the trenches to minimize damage to the BOx.  The


electronic deflection stage produced BPAs that are required  for circuit edit at the 45nm technology node.  The use of subpA beam currents provided very controlled etch rates, which  are also necessity for decreasing technology nodes. The use  sub-pA beam with the FIB’s advanced SE detection system  allows the user to perform FIB operations with minimum ion  beam dose.  This will prevent damage to charge sensitive gates  and thus control VT shifts in the devices.


0.10 um


Figure 15. CAD alignment at 500fA using the electronic stage


t43


30HY-032m0


[1] RH Livengood, D Medeiros, “Design for (Physical) Debug for Silicon Microsurgery and Probing of FlipChip Packaged Integrated Circuits”, IEEE-ITC


E-Beam:SpotTitMagPWDDetBeamSpotTiltMagFWDDet


(1999) 877.


[2] S. Herschbein, C Rue, C Scrudato, E Hermann, “FIB  Chip Repair:  Improving Success by Controlling  Beam-Induced Damage and Thermal/Mechanical  Stress”, ASM-ISTFA (2004)


[3] AN Campbell, P Tangyunyong, JR Jessing, CE  Hembree, DM Fleetwood, SE Swanson, JM Soden, N  Antoniou, WE Vanderlinde, MT Abramo, “Focused  Ion Beam induced Effects on MOS Transistor  Parameters”, ASM-ISTFA (1999) 317.


[4] C. Boit, U. Kerst, P. Sadewater, R. Leihkaufa, S. Schömannb, E. Le Roy, T. Lundquist, “Contacting  Silicon with FIB for Backside Circuit Edit”, ASMISTFA (2004) 157


[5] M Abramo, L Hahn, L Moszkowicz, “Gas Assisted  Etching: An Advanced Technique foe Focused Ion  Beam Device Modification”, ASM-ISTFA (1994)


439.


76


[6] C.G. Talbot and D. Masnaghetti, US Patent No. 5401972


[7] H. Ximen, and C.G. Talbot, “Halogen-Based  Selective FIB Milling for IC Probe point Creation  and Repair”, ASM-ISTFA (1994) 141


[8] H Marchman, S Herschbein, C Scrudato, C Rue, L  Fischer, M Abramo, “The Impact of Geometris  Packing Density on FIB Editing of Advanced  Technology ICs”, ASM-ISTFA (2003).


[9] M.A. Thompson, C. Richardson, E. Le Roy, T. Lundquist and W. B. Thompson, “Coaxial, PhotonIon Technology Enables Direct Navigation to Buried  Nodes on Planarized Surfaces, including Silicon” Proc ISTFA (2002) 409.


[10] M Abramo, N Antoniou, D Barton, KN Hooghan, RH Livengood, “FIB Backside Isolation  Techniques”, Microelectronics Failure Analysis Desk  Reference 2001 Supplement, p1.


[11] L Wang, TM Montagne, S Etchin, SV Sankar, "Compact High Collection Efficiency Scintillator for  Electron Detection", US Patent 6,630,667 (2003)


77


The Joy of SOI:


As Viewed From A Backside


Focused Ion Beam (FIB) Perspective


Steven Herschbein, Chad Rue, Carmelo Scrudato


IBM Microelectronics, Hopewell Junction, NY  USA


For most advanced semiconductor products, the preferred


methodology for achieving Focused Ion Beam (FIB) circuit  modification and node access is through the backside of the  chip.  The high density of interconnect wiring and the  presence of C4 solder bumping has made complex edits  virtually impossible with conventional frontside techniques.     IBM has developed a set of procedures for performing  backside edit on circuits built using the Silicon-On-Insulator (SOI) process.  While the basic approach and techniques  parallel many of the established practices developed for  handling transistors built in conventional bulk silicon, there  are a number of key and critical differences.  In this paper, we  will address the basic instruction set developed for successful  FIB work on SOI product.  This will include backside silicon  surface preparation, charge control, endpointing during high  volume silicon removal, global and local coordinate lock  techniques, floor voltage contrast phenomena, floor  preparation and preservation, fill pattern issues and  advantages, and finally the target structure alignment, access, connection and/or removal.  Post process bake and handling  will also be discussed.


Focused Ion Beam (FIB) tools have found wide acceptance in  failure analysis and process development laboratories  throughout the semiconductor industry.  Beam induced  microsurgery, or the ability to selectively remove existing  materials and deposit new conductor and insulator layers, enables access to circuits deep within fully processed silicon.  FIB modification for chip repair and internal node signal  probing has become an integral part of the process for  bringing advanced products to market.


Logically, FIB circuit modification was initially performed  from the frontside of the device.  Early products contained  sufficient white space between back end of line (BEOL) metal  interconnects to allow unencumbered access to lower levels.   As devices become more complex, with more BEOL levels,


tighter geometries, and more extensive use of pattern fill, conventional frontside FIB methods faced insurmountable  challenges.  Even on relatively simple chip designs, flipchip  packaging, in common use by the late 1990’s, put severe  constraints on frontside FIB success.  The dense distribution  of raised solder bumps on the chip surface resulted in large  regions of the circuitry below being obscured and  inaccessible.  A major paradigm shift was required in order to  keep FIB circuit modification viable.


Evolution of the Backside FIB Process


One of the greatest advances in the field of FIB microsurgery  was the development of hardware and techniques making it  possible to gain access to circuit nodes thru the silicon  substrate.  As described in the breakthrough paper by  Livengood et al [1], a new generation of FIB tool was  introduced, along with a unique sample preparation process.  While much more labor intensive than conventional front side  repair, the backside approach provided unlimited access to the  active region, enabling direct transistor level modification.


The backside FIB method described and practiced throughout  the industry until very recently was designed to work with  semiconductor products manufactured using a conventional  single crystal bulk silicon process.    In fact, the vast majority  of chips produced worldwide are still manufactured using this  technology.  Bulk processes, like twin well CMOS, have no  demarcation layer shielding the vulnerable transistor  underside.  This puts them at risk during the preparatory  trenching step.   Protecting the underside of active devices  requires that an artificial trench floor be constructed, with all  FIB modification work commencing from this raised platform.  By contrast, state-of-the-art Silicon-On-Insulator (SOI) CMOS semiconductor processes essentially have this floor  built in as part of the basic device structure.  The resident  buried oxide floor creates a more natural starting point for  accomplishing the highly detailed FIB circuit access and edit  process.


IBM is the semiconductor industry leader in the development  of a production capable high performance SOI process.  As


78


# The Joy of SOI: As Viewed From A Backside Focused Ion Beam ( FIB) Perspective


such, the FIB labs at IBM have had better than 4 years of  experience in practicing the art of backside circuit  modification and access thru the buried oxide floor.


General Sample Preparation Issues


The basic process of backside sample preparation applies to  either bulk or SOI.  While it is possible to work with thick  silicon (typical starting point on our products is around  750um), we almost always thin to under 100um using a planar  pad polisher or vertically driven rotating bit milling machine (CNC or mechanical drive).  The choice of grinding methods  is usually dictated by what, if anything, surrounds the die.  If  there are no obstructions, then the planar polisher is the most  expeditious approach.  As shown in Figure 1 below, if there  are chip capacitors or other integral structures along the sides  at die height, then a vertical small bit tool may be the only  choice.


Figure 1: C4 mounted chip on ceramic flip-chip type  substrate. Mechanical grinding/milling was used to thin the  backside silicon from 760um down to below 100um.  Decoupling capacitors surrounding the die remain intact.


The local trenches for circuit access are usually formed by  etching the remaining silicon down to the work plane using  the FIB.  Some labs have also found that a chlorine gas cell  laser chemical etcher, used either alone or in conjunction with  the above grinding and FIB methods, to be a cost effective  solution for bulk silicon removal.


Conventional Bulk Silicon Backside FIB


For circuits produced in a bulk CMOS process, the initial  objective is to stop the local trench milling within a few  microns of the underside of the device source-drain (S-D) region.  All circuit edit work will eventually be performed  from this elevated work plane.  The closer and more uniform  this plane is to the active regions (less silicon remaining), the  easier subsequent work will be.  Placement accuracy of mills


Figure 2: Cross-sectional image showing sloped bulk silicon  trench floor above transistor active region.


The SOI Transistor Structure


IBM introduced the modern implementation of SOI into  volume production in 2000.  Tests show a 20-30% performance gain along with a matching reduction in power  consumption compared to similar designed and processed  bulk CMOS chips [6].  SOI greatly decreases transistor  junction capacitance by placing a fixed barrier of oxide of  approximately 0.15um thick beneath the entire active region.  From a transistor operational perspective, the presence of the  silicon substrate below the buried oxide (BOx) really is of  little consequence.  All electrical operation takes place in the  sub 0.25um single crystal silicon layer on top of the BOx.  The substrate below merely provides a mechanical and  thermal base.  With proper thermal and stress management, removal of that base for purposes of FIB and other backside  analysis techniques has little impact on the functionality of the  circuit under study.  Techniques for functional package  rebuilding were presented at this conference last year [7].


The SOI Backside FIB Process


Just as with the initial steps for bulk silicon, SOI backside  access typically begins with mechanical preparation down to  about 100um of silicon remaining.  The overall goal of the  backside FIB trenching process, however, is quite different.  Remember that with bulk processes the objective was to  accurately stop and leave a few microns of material to protect  the underside of the active region.  With SOI, the  manufacturer has built the protective barrier right into the  product.


While it will still aid IR imaging and overall etch uniformity,


mirror smooth starting surface prep for high volume XeF2 FIB


trenching is a less important factor with SOI.  Surface


cleaning with bromine can also be skipped, as the final


spontaneous milling step will level out any isolated spots that


break thru early.  Even knowing the exact location in Z


(thickness of silicon remaining), while helpful, is not


absolutely essential.


Through a combination of beam-driven and beam-off


spontaneous chemical milling, the backside silicon trenching 4a process becomes self-limiting.  The buried oxide insulator acts


as a natural etch stop towards the very end of the milling


process, resulting in a uniform, flat floor.  Once the first spot


breaks thru exposing the buried oxide, you simply terminate


the beam but allow the gas to continue flowing.  The


spontaneous etching will quickly remove the highly textured


thin silicon remaining on the BOx all the way out to the


perimeter edge, as shown below in Figure 3.  Thanks to fairly


high chemical selectivity, the oxide holds up well to the gasonly etch exposure.


Edge of die


ASTET71191111


Substrate thinned


Backside silicon damage


to about 100um


from exposure to XeF2


Figure 3: Perspective view of backside trench mill and SOI  floor showing uniform BOx layer across a wide expanse.


Bottom of trench work areas as large as 450um x 450um have  been opened by this technique in a single operation.  See  Figure 4 as an example.  Multiple trenches can even be placed  in close proximity.  This allows all of the subsequent circuit  access activity to occur on a planar surface in close proximity


15 uS PbrageMode: EectronPcceteration: 50 RYperture:37.50 umOY:50000mX300


to the target structures.


We have also seen a semi-permanent capacitive voltage  contrast effect on the exposed oxide floor that shows the  position of source-drain regions of each discrete transistor.  See Figure 4b.  This is similar to the n-well voltage contrast  technique developed for bulk silicon devices, but far more


spacially significant.  Direct access to the SOI floor takes this  technique to the next level.  SOI processes do not employ the  large substrate defining tubs used in the conventional bulk  CMOS structure, so whatever transmitted information you see  more accurately reflects the actual physical circuit layout.  Highly detailed capacitive voltage contrast imaging through  the BOx down to approximately 10um FOV has been  demonstrated.


Underfill


Buried Oxide


Figure 4a & 4b: Optical and FIB image of the trench floor  clearly show that the capacitive voltage contrast effect (bottom image) mirrors the optically transmitted (top image) layout data.  Cleared trench floor exceeds 350um across.  Local lock points were chosen within the trenched area.


81


The BOx floor is already an insulator, so no oxide deposition  is required to prevent substrate shorting.  See Figure 5 below.  Drills to conductor layers are done either through no longer  needed devices, or thru STI (the equivalent of field oxide  regions), directly into interlevel oxide.  In most cases, no new  oxide depositions are required for preventing sidewall shorts, greatly reducing edit complexity.


Local lock points are easily obtained, as a wealth of unused  and pattern fill structures exist near the repair zone, within a  half micron of the oxide floor.  In general, the use of local  locks mitigates the error introduced by applying straight line  algorithms from conventional die corner points.  This has  become a more pressing issue with the introduction of  mechanically flexible, low cost packaging.  The mechanical  stress due to the mismatch in coefficient of expansion can  result in severely bowed (pincushion) silicon.


|TOV:|5.38km|
|---|---|

Figure 5: Cross-sectional image of SOI trench floor showing  uniform BOx layer across a wide expanse.  The ‘X’ was milled  only as a visual aid to show the oxide region immediately  above active components.


Charge Control


Backside FIB operations, whether they be on bulk or SOI, will  require attention to the issue of charge control.  During  trenching, bulk processes might have adequate grounding  paths through junction contacts and package terminations.  SOI is clearly more at risk.  Either technology will benefit  from the use of basic sample grounding techniques, such as  carbon paint and tape from the exposed silicon to the sample  holder.


If conductors are to be deposited on the bulk process trench  floor, large expanses of the nearby silicon will need to be


covered with oxide to provide isolation.  SOI, with its  isolating barrier layers, will essentially already have this oxide  in place.  Either will require a temporary path to ground  during all circuit access operations as the large expanse of  floor oxide limits natural shunts in the immediate vicinity of  the repair zone.   A local ring strap or thin blanket deposition  of metal can be placed on top of any oxide, connected to a  trace that leads up onto the exposed backside silicon, or to a  plug drilled thru layers to a proper circuit ground point.  In  this way, much of the circuit modification work and imaging  done in the immediate area will benefit from some level of  beam charge reduction.  The connection lead is severed, and  the film/straps removed as part of the cleanup steps when the  work is completed.


Post-FIB Bake


It has been well documented that operation of a charged  particle beam in close proximity to transistors can have a  detrimental effect on their overall operation and stability [8, 9, 10].  Fortunately, baking the part after FIB exposure has also  been shown to reverse certain types of charge induces shifts.   Much of our backside access & functional repair work  requires that we operate in very close proximity to the  underside of active circuit elements.  With conventional bulk  process silicon a few microns of material remain, and this  seems to have the effect of shielding the active region from  damage.  Working directly on the BOx does increase the risk, as the trench floor lies within 0.25um of the active gate  region.


Last year we presented bake recovery results from a backside  cell disturb study done on SOI SRAMs.  Based on this and  other work, a bake of 200°C for 8 or more hours in dry N2  was determined to satisfy most demands, and has become part  of our standard procedure [7].


An unexpected side benefit of the high performance SiliconOn-Insulator fabrication process is that it also greatly  simplified backside FIB chip edit.  The built-in insulator layer  of known thickness and a uniform distance from the underside  of active structures provided a natural etch stop during  trenching, and a consistent starting point for circuit element  access.  While issues like charge control and residual charge  abatement require a little more forethought, neither presents a  real limitation to successful work.  The result was the  development of an extremely robust methodology for  performing backside FIB operations that avoids many of the  pitfalls of the conventional approach.


[1] R. Livengood, et al, “FIB Techniques to Debug Flip-Chip  Integrated Circuits,” Semiconductor International, March  1998, pp. 111-116.


82


[2] N. Bassom, et al, “Modeling and Optimizing XeF2-enhanced FIB Milling of Silicon,” Proc. 25th ISTFA, Santa Clara, CA, Nov. 1999, pp. 255-261.


[3] R. Ring, et al, “FIB Applications for Flip Chip Packaged  ICs,” EDFAS News, February 2001, pp. 32-36


[4] W. Tompson, et al, “A Novel Optical End Pointing  Technique Applied to Backside FIB Editing,” J. Vac. Sci. Technology,  B 21, 2003.


[5] C. Boit, et al, “Voltage Contrast like Imaging of NWells,” Proc. 29th ISTFA, Santa Clara, CA, Nov. 2003, pp. 331-337.


[6] R. Richmond, “Silicon on Insulator Technology,” SysOpt.com web page, a Jupiter Media Corporation news  site, Nov. 8, 2000.


[7] S. Herschbein, et al, “FIB Chip Repair: Improving  Success by Controlling Beam-Induced Damage and  Thermal/Mechanical Stress,” Proc. 30th ISTFA, Worcester, MA, Nov. 2004, pp. 166-171.


[8] A. Campbell, et al, “Effect of FIB Irradiation on MOS  Transistors,” Proc. 35th IRPS, Denver, CO, April 1997, pp. 72-81.


[9] J. Benbrik, et al, “FIB Irradiation Induced Damages on  CMOS and Bipolar Technologies,” Proc. 24th ISTFA, Dallas, TX, Nov. 1998, pp. 49-55.


[10] R. Desplats, et al, N. Antoniou, D. Monforte, “Reliability  of Bipolar & MOS Circuits after FIB Modification,” Proc. 27th ISTFA, Santa Clara, CA, Nov. 2001, pp. 288-298.


83


Complementary Optical Techniques for Advanced IC Failure Analysis –  Case Study


Joy Y. Liao and Howard Lee Marks


NVIDIA Corporation, Santa Clara, CA, USA


Herve Deslandes


Credence Systems Corporation, Milpitas, CA, USA


Figure 1.  Evolution of emission microscopy, from CCD  sensors to infrared focal plane arrays.


Photoemission


Thermal emissionThermal Emission


1.00


We investigated and demonstrated the advantages and


0.90InGaAs OE


0.90


IREMIPE


Sleonlansession"Filtering"


limitations of several optical methodologies as valuable silicon


080NO Themsal


REMYEOF


failure analysis techniques, and how they could be used in a


070


"ERNEN。TOE


denoopou


0.70


complementary manner to assist in shortening the diagnostic 1000Detection


0.40


8OL991uej ui040


IREM HTE0.30少on m


0.50so


CCOIE


0.60TV


time.


Thernal


Datection0.20


030


e护


pental


-010


Failure analysis for integrated circuits (ICs) is becoming more


010


dependent on optical techniques, especially for non-contact


400800120016002000240028003200 000


口0.00


testing through the backside of silicon.  These techniques have


CCD backside detectionWavelength [nm]


been studied in academic and industrial laboratories; among  them are infrared optical microscopy, light and thermal  emission microscopy, induced thermal effect imaging, etc. [1-7].  In emission microscopy, the HgCdTe focal plane arrays  replaced the CCD for backside acquisition since 1996.  About  2 years ago, cryogenic InGaAs focal plane arrays provided  another step in the performance ladder (Fig. 1).  Various  thermal detectors, including HgCdTe, InSb, and extended  InGaAs, are also available for thermal acquisition where a  compromise between sensitivity and resolution is necessary.  This is especially true for backside detection where the silicon  acts as a filter, depending on its thickness and doping level.  Laser stimulation with various wavelengths is also widely  investigated as a non-destructive, contactless failure analysis  technique.  In general, an infrared laser beam with a  wavelength greater than the silicon bandgap value is utilized  for thermally based applications such as thermally induced  voltage alteration (TIVA). The optical power is converted into  thermal energy which generates local heating when the laser is  scanned over the IC.   On the other hand, a laser beam with a  wavelength around the silicon bandgap value is employed for  photoelectric based applications such as light induced voltage  alteration (LIVA).  In this case, the optical power is converted  into electrical energy which induces a photoelectric effect  when the laser interacts with the IC.  Test vehicles were  designed for a better understanding of the interactive  mechanisms between ICs and various analysis tools.  The  analysis results revealed that certain defect types could be  identified using one technique but not another.  When  presented with an IC failure, what technique should the  analyst use so that defect localization can be achieved in a  quick and effective manner?


In this paper we investigated the benefit of using a dual  approach with laser scanning microscopy (LSM) and emission  microscopy (EM) for quick fault isolation on failed  semiconductor ICs.  Extensive experiments with both  techniques report advantages and limitations of one technique  over the other.  We present four failure analysis cases of  advanced graphics ICs with 0.14µm technology.  Multiple  wavelengths in EM (photo and thermal emissions) as well as  in LSM (LIVA and TIVA) were employed on the same  samples for fault isolation.  Physical defects were finally  identified during subsequent destructive physical analysis.


Experimental Details


The devices under test (DUT) are advanced graphics ICs with


0.14µm technology in ball grid array (BGA) packages.  Backside failure analysis was employed in Cases I, II, and III  due to the increased complexity of the layout which results in  increased density and layers of metallization.  The DUTs were  tested in their original BGA packages, with all substrate  resistors and capacitors intact.


Case I and II involved graphics devices that were subjected to  electrostatic discharge (ESD) stressing with charged-device  model (CDM) and human body model (HBM), respectively.  These devices were extensively analyzed with the optical  techniques available in the NVIDIA FA lab.


84


# Complementary Optical Techniques for Advanced IC Failure Analysis – Case Study


The samples in Case I are multilayer wire-bond encapsulated  devices in a BGA package.  In order to perform backside  analysis on wire-bond devices, it is necessary to expose the  backside of the silicon by removing the substrate material as  well as solder balls that cover the area of interest.  This  backside sample preparation has been successfully  accomplished without altering the original failure mode.  The  exposed silicon area was polished and coated with antireflective coating to minimize light diffusion.  The samples in  Case II are bare-die flip-chip devices in a BGA package; the  backside of silicon was polished and coated with antireflective coating.  For flip-chip devices, the silicon thickness  was approximately 700 µm and the pin of interest showed a  forward bias leakage of approximately 150 µA.


Case III involved two graphics devices that were subjected to  High Temperature Operating Life (HTOL) stressing.  The  devices exhibited no clock signals in a particular PLL.  The  samples are bare-die flip-chip devices in a BGA package, and  the backside of the silicon was polished and coated with antireflective coating.  The silicon thickness was approximately  700 µm, and curve trace analysis revealed slightly higher IDD  when the device was set in a power-up static mode.


The fourth example, where multiple optical techniques were  required to speed up defect localization, utilized the ability to  switch between a photoemission filter and a thermal emission  filter within the emission microscope.


Case I


Photoemission at low magnification revealed no emission  spots when the failing pin of DUT was biased at 150 µA.  When the current was increased to 1mA, both failed and  correlation units showed photoemission after a 100 second  acquisition (Fig. 2).  This indicates that at the higher current, in addition to the failing leakage, other elements also  connected to the biased pin would emit.  The leakage spot was  only identified at higher magnification.


Thermal emission at low magnification provided no indication  of the defect under the 150 µA bias condition.  The defect  location was observed only at higher magnification.  Adjustments were made of the detection duration and  repetition to avoid thermal saturation and properly accumulate  the emission signals.


The samples were tested with nonbiased laser stimulation  using a 1340nm laser (TIVA) or a 1080nm laser (LIVA),  while the current variation between the failing pin and ground  was monitored via the acquisition device.  Abnormal current  consumption induced by laser stimulation gives information  that assists failure analysts in localizing the physical defects in  ICs.  When interacting with silicon, the 1340nm laser induces  local heating but does not have sufficient energy to produce  electron-hole pairs.  Thermal gradients rather than  photocurrents are the results of the laser raster.  Therefore, TIVA quickly identified an abnormal current location at low


magnification, and pinpointed the exact location at higher  magnification with near-real time acquisition (Fig. 3).


The 1080nm laser, on the other hand, introduces photoelectric  effect in the semiconductor regions.  Hence, localization  information acquired with this laser scanning usually requires  further investigation.  Nonbiased LIVA revealed an  anomalous current location different from the defect location  identified with emission and TIVA (Fig. 4).


Figure 2.  Micrograph showing photoemission location biased  at 1.5mA after 100s acquisition.  The same location was  observed on both the failed unit and a correlation unit.  Magnifications are 1X (left) and 75X (right).


Figure 3.  Micrograph showing nonbiased TIVA location on  the failed unit with laser scanning at 2.7µs/pixel.  Magnifications are 5X (left) and 100X (right).


Figure 4.  Micrograph showing nonbiased LIVA location on  the failed unit with laser scanning at 2.7µs/pixel.  Magnifications are 5X (left) and 100X (right).  The location  was not observed on a correlation unit.


The same findings were observed on multiple samples that  showed leakage on the same pin, but not on a correlation unit.  Physical analysis revealed ESD damage at the location


85


identified by EM and TIVA.  Top view and cross section of  the damage are examined under SEM (Fig. 5 and 6).  TIVA is  most suitable for this resistive type of defect, as in Case I, due  to the fact that the thermal gradient associated with resistance  variation induces a Seebeck voltage which provides  information on defect localization [7].


Careful inspection of the vicinity of the LIVA-identified  location also revealed subtle ESD damage.  Design  Engineering, who was consulted regarding this finding, suspected that this gate was damaged because the protection  device was compromised and failed to adequately protect the  internal circuitry.  Therefore, LIVA identified a secondary  damage in Case I devices.


血n


SEI5.0kv X9,0001μmWD6.9mm  Figure 5.  SEM photograph showing damage at the ESD  protection diode on the location identified with EM and TIVA, after the device was deprocessed to expose silicon.


000


SEI5.0kv X9,0001μm WD5.1mm  Figure 6.  SEM photograph showing the cross-section of the  damage at the ESD protection diode on the location identified  with EM and TIVA.


Case II


Photoemission and thermal emission at low magnification  revealed no emission spots when the failing pin of DUT was  forward biased at 150 µA.  When forward biased at


approximately 4.5mA with a DC voltage of 1.2V, a number of  emission locations were revealed that were almost identical in  both failed and correlation devices.  Because the pin also  failed under a reverse bias condition, emission analysis under  reverse bias was also attempted. The number of emissions was  reduced to one, but the emission site revealed in the low  magnification micrograph in Fig. 7 appeared to be present for  both failed and correlation units.  At higher magnification, however, the leakage spot was separately identified as  different in the failed device verses the correlation unit.


Figure 7.  Micrograph showing photoemission location biased  at 2mA in the reverse bias direction after 50s acquisition.  The  same location was observed on both the failed unit and a  correlation unit at low mag.  Magnifications are 1X (left) and  75X (right).


Figure 8.  Micrograph showing nonbiased TIVA location on  the failed unit with laser scanning at 2.7µs/pixel.  Magnifications are 5X (left) and 100X (right).


LEI5.0kVX5,5001μm WD 13.0mm  Figure 9.  SEM photograph showing the ESD damage at the  location identified with EM and TIVA.


86


During laser simulation analysis, TIVA quickly identified an  abnormal current location at low magnification, and  pinpointed the exact location at higher magnification with


霭


near-real time acquisition (Fig. 8).  Nonbiased and biased  LIVA revealed too much information that was probably  characteristic of the pin, as the pin of interest is designed to  connect to numerous transistors and diodes.


Physical analysis found ESD damage at the location identified  by EM and TIVA (Fig. 9).  TIVA again provided quick and  precise defect localization in Case II.


Case III


Compared with a correlation unit (good device), device S/N  20 showed more backside photoemission locations, and S/N  18 revealed fewer sites (Fig. 10).  Thermal emission was  attempted; however, under this particular biasing condition, the technique failed to provide useful information because the  thermal conditions of the DUT would not stabilize within a  reasonable period of time before thermal saturation occurred.


Good


SN20


SN18


石抽


Figure 10.  Micrograph showing photoemission locations on a  correlation unit and two failed units (S/N 20 and S/N 18)


good


under the same bias conditions.  The malfunctioning PLL is  located at the bottom of the graphs.


Figure 11.  Micrograph showing high magnification (10X) photoemission locations on S/N 18.  Red arrow in the  unprocessed lower PEM image points to the anomalous  location, not detectable in the upper overlaid image.


Figure 12.  Micrograph showing high magnification (20X) photoemission locations on S/N 18.  Green circle indicates the  location of the anomalous PEM identified in Figure 11.  Red  circle indicates the location of the burned contacts revealed  during deprocessing.


出址


息 00


Figure 13.  Micrograph showing LIVA locations on a  correlation unit and both failed units under the same bias  conditions.  Green arrow in S/N 20 points to the anomalous  LIVA location that was not present on the correlation unit.


Anomalous PEM


Figure 14.  Micrograph showing high magnification (80X) LIVA location from multiple directions.  The offset of the LIVA  image over the reflected laser image results from the delay in  response time between the impact of the laser and the induced  resistance change.


87


Figures 11 and 12 give the photoemission images that we  obtained on S/N 18.  No anomalies were observed during  TIVA.  LIVA at low magnification identified, on multiple  samples, an anomalous high current density location in the  suspected PLL, when the device was biased with a constant  current.  However, this could have been overlooked if there  was no prior knowledge of the relative location of the  malfunctioning circuitry (Fig. 13).


Therefore, it is critical to properly adjust the scanning  resolution and intensity of the laser, in order to achieve  adequate spatial resolution and signal to noise.  The LSM  usually is required to use the maximum resolution (typically  1024x1024 pixels), at low magnification with a high


numerical aperture objective.  This may not be enough at  times in the case of a macro lens (1x or lower).  This is


because the scanning size could be greater than the spot size,


so that the defect could be missed by the laser.  Possible  solutions are either to reduce the field of view by reducing the  scan angle of the mirrors and keeping the same number of  pixels, or to underfill the entrance pupil of the objective lens. In this latter case, the beam diameter is smaller than the


口口


0 . 0 0


0。


objective aperture; hence the full numerical aperture of the  lens is not fully utilized.  Such optical design increases the  spot size on purpose so that it won’t miss the defect at low  magnification. Another possibility is to purposely defocus the  beam in order to increase the spot size. In all these cases the  goal is to have a spot size at least the size of the scan step.  In  practice when we switch to a higher magnification objective  this is no longer a problem because the system is optimized for  the largest NA lens (typically 100x) in order to get the best  resolution.  In this case study, at higher magnification, multiple scans from multiple directions were performed to  further improve the spatial resolution that is dependent on the  time delay between the impact of the laser and the induced  voltage alteration (Fig.14).


Figure 15.  Optical micrograph showing burned metal lines  crossing the anomalous LIVA area identified in Figures 13  and 14, indicating a possible EOS event.


Layer-by-layer deprocessing and subsequent inspection  revealed burned metals in the vicinity of the LIVA anomalous


current location (Fig. 15).  The vicinity of all photoemission  sites shown in Fig. 11 and 12 was also examined under SEM, when the devices were deprocessed to exposed silicon.  Only  one location on one sample (S/N 18) exhibited burned  contacts.  On the second sample (S/N 20), chip out and cracks  were revealed on the poly-capacitors over several areas in the  malfunctioning PLL.  Both electrical and physical analysis  findings indicated an Electrical Overstress (EOS) event, which    apparently happened during HTOL reliability stressing.


SEI3.0kVX1,40010kcmWD13.2mm  Figure 16.  SEM micrograph showing burned contacts in the  vicinity of the anomalous photoemission area identified in  Figure 11, indicating an EOS event.


OBIRCH analysis was performed using the OBIRCH amplifier


through micro-probes to isolate the defect. The positive node  was connected to the MCS node and the negative node was  connected to the BCSS node. Figure 16 shows the OBIRCH  site where MCS and BCSS are shorted. A FIB cross-section of  the OBIRCH site found a titanium defect (Fig. 17).


Figure 16: The OBIRCH site on the metal one lines where two  nodes run parallel to each other.


Figure 17: The arrow points to the defect found in the crosssection at the OBIRCH site. Energy Dispersive Spectroscopy, analysis of the defect revealed that the defect contained  titanium.


Localization


In Case 1 and Case 2, OBIRCH analysis was successful in  localizing the defect area near the beginning of the analysis. This localization was possible because the device could be held  in a quiescent state with little Idd current fluctuations. The  methodology of identifying anomalous high current vectors on  the Hilevel mini-tester proved effective for choosing a  condition for OBIRCH and light emission analysis.


In Case 3, an initial OBIRCH signal was not detectable on the  evaluation board. The Idd current needs to be stable with little  variation for the resistance change to show enough variation to  be detected [4]. If the device could be put into a sleep or  standby mode that stops the device’s internal clocks, the initial  OBIRCH analysis may have localized the defect. It is possible,


but unlikely, that this condition could be met. The


microcontroller would need to have a halt or sleep mode to put


Probe points  OBIRCH site


MCS           BCSS


99


the device in a state with little variation in the Idd current. If a


quiescent Idd method can’t be used to isolate an area to  investigate, other traditional isolation methods are necessary as  seen in Case 3.


Defect site identification


OBIRCH analysis has been shown to be effective in identifying  the defect once the failing signal is located and characterized. If  the OBIRCH amplifier can be used to force a voltage or current  directly across the defect, the OBIRCH technique is very  effective at pinpointing the defect location. This can be very  useful when the signals in question have long routes. As  technologies become more complex with many metal layers  and computer generated routing of signals, this isolation  technique becomes more important.


If the defect can be pinpointed, a FIB cross-section can be  performed instead of physical deprocessing techniques. This is  an advantage because physical deprocessing can be very  iterative and time consuming. FIB cross-sections can be  performed much faster. The time advantage of FIB crosssectioning versus top down deprocessing is magnified with  more complex technologies that have more metal layers. FIB  cross-sections can provide better defect detail. In the case of a  wafer fabrication defect, the FIB cross-section can be helpful in  pinpointing the process step where the defect originated


Observations


In Case 1, the defect appears to be a low resistance connection. The defect had a short from a signal to Vss. The output pchannel was saturated and a small resistance change due to the  localized heating of the optical laser in a very low resistance


would not cause much, if any change in the current.


In Case 2, the defect appears to be more tenuous and it  probably had a higher resistance connection. Also, because the  defect shorted two signals, there was potential for more


variation in the current through the defect.


In Case 2, there were multiple indications of the defect


location. OBIRCH analysis detected the defect as well as the


output p-channel transistor trying to drive the signal high. This


contrasts to Case 1 where only the output p-channel transistor  driving high was found with OBIRCH analysis. One difference


appears to be due to the resistance of the defect. The other  difference is that Case 2 had two signals shorted and Case 1  had a short to Vss. A light emission was also observed at the  defect location which might also be an indication of a high


resistance defect.


The analysis performed in these cases show that the analyst  will have a better chance of success if a combination of


techniques is used. Case 1 illustrates an important point. If a  cross-section was performed when the initial OBIRCH site was


identified, the defect may never have been found. The IDDQlike measurements are very important since they identify a


device state that is more likely to show light emissions, liquid


crystal hot spots or OBIRCH sites.


It has been our experience that OBIRCH analysis is a valuable  addition to the failure analysis toolset. It is more difficult to


isolate functional failures that are embedded in digital logic but  with the right combination of techniques and tools, the  isolation process can be done quickly. Once a failing signal is  isolated, OBIRCH again is useful for determining the exact  defect location. OBIRCH analysis has become a valuable tool  for defect localization but it cannot be used in all cases. In this  case study, OBIRCH analysis has helped improve success rates  and decrease analysis cycle time.


The authors would like to acknowledge Tricia Slovacek and  Chuck Petri for their physical analysis and cross-section  contributions, respectively.


[1] Nikawa K. and Tozaki S., “Novel OBIC Observation  Method For Detecting Defects in Al Stripes Under Current  Stressing” ISTFA proceedings 1993 (ASM International),


pp. 303-310


[2] Cole Jr. E.I., Tangyunyong P. and Barton D.L., “Backside  Localization of Open and Shorted IC Interconnections, Proceedings of IEEE International Reliability Physics


Symposium (1998), pp. 129-136


[3] F. Beaudoin, et. al., ”Emission Microscopy and Thermal  Laser Stimulation for Backside” ISTFA proceedings 2001


(ASM International), pp. 227-235


[4] Jacob, Peter and Beaudoin, Felix, “OBIRCH - Monitoring  As A Reliability-Failure-Analysis and Screening Tool” ISTFA proceedings 2001 (ASM International), pp. 397-


403


Advanced electrical characterization of 90 nm Soft Bit Failure  by Nano Probing technique


Christelle Giret and Damien Faure


Texas Instruments, NDAL, Villeneuve-Loubet, France


The Soft Bit failure (Single Bit Failure sensitive to voltage) of a


90nm SRAM cell presented a difficult challenge for the Failure  Analysis (FA) group. Physical analysis of these Soft SRAM  failures did not show any visual defects; therefore the FA  required an accurate electrical characterization. The transistor  characteristics of the failing SRAM transistors are needed in  order to speculate on the possible failure mechanism. The  Nano-Probing technique performed at Nice Device Failure  Analysis of Laboratory (NDAL) allowed us to identify  anomalies of I/V characteristics like Vt imbalance, low Gain, asymmetrical Vt, ID (Drive current) and Ron. Case studies of an  asymmetry phenomenon reported here lead to a correlation  between the failure mode and the electrical measurements. This  paper demonstrates a suitable electrical methodology and  characterization by Nano-Probing in order to successfully  manage a FA approach on this type of failure.


During the qualification efforts of our 90nm technology, 30% of the SRAM rejects were Soft Bit failures; these failures were  additionally binned based on the defective voltage: Vddmin, Vddmax, Shmoo hole or Data Retention. A cursory failure  analysis effort (PVC, STEM/TEM) for each type of failure  mode, failed to reveal any physical defects; and was classified  as Non-Visual Defect (NVD). An accurate electrical approach is  required to identify the defect. The Nano-Probing technique  with four probes was one technique which allowed a complete  measurement of the electrical parameters (Vt, ID, Ron, and Gain) of the transistors. The effectiveness of this technique has  already been demonstrated on the latest CMOS 130nm and  90nm technologies ([1] and [2]).


An accurate understanding of the failure mode by emulator  characterization and Nano-Probing technique of the six  transistors for the defective SRAM cell will be investigated in  this paper. Two cases studies performed at NDAL which  exhibited asymmetry of Vt,  ID and Ron will be presented in  details. Additionally, we will try to show the correlation  between the failure mode and the asymmetrical measurements  and we will discuss the different hypothesis of root cause.


SRAM cell


First, it is important to note the specifics of an SRAM cell This  SRAM (Figure.1) operates in two different modes, in Read and  Write mode; therefore the current into the transistors comes  from Source to Drain and also from Drain to Source during  SRAM operation.


Based on this functionality a better electrical methodology to  solve the soft bit fails was obtained.


Figure.1 Schematic view of an SRAM cell. The arrows  indicate the Drain (close to the memory point) and the source  of the Bit and Nbit pass transistors and the sense of the data  for Write and Read cycles


Failure Mode and Defect Isolation


Definition of the failure mode by ATE


The failing units binned as an “SRAM reject” by ATE (Automatic Test Equipment) can be sorted into two categories: Hard failure (all Vdd) and the Soft failure (Vddmin, Vddmax, Shmoo hole or Data Retention). To further classify the ”Soft  failures”: “Vddmin” corresponds to an SRAM cell that does  not operate at a low operating voltage; “Vddmax” corresponds  to  an SRAM cell that does not operate at a high operating


101


# Advanced electrical characterization of 90 nm Soft Bit Failure by Nano Probing technique


voltage;  “Shmoo hole” corresponds to an SRAM cell that  does not operate between two voltages; “Data retention” corresponds to an SRAM cell which keeps abnormally a value (1 or 0) during successive read/write operation at a specific  voltage value; the ATE indicates the value of retention voltage  and the defective voltage based on the checkerboard  configuration.


ESDA and Emulator characterization


ESDA (Enhanced Software Defect Analysis) was performed on  each defective unit according to ATE results. This technique  maps the defective bits, columns or rows in the bit map for the  Hard failure and precisely the Single Bit Fail (SBF) in the  SRAM for the Soft failure. ESDA characterization in addition to  the ATE results is sufficient to understand the failure modes of  the Hard failure, but is not sufficient for Soft Bit failures.


With the increase of NVD associated with the Soft Bit fails , another technique is needed to improve the defect isolation. The emulator characterization like ESDA characterization  locates also the SBF in the defective SRAM block. This  specific tool allowed to observe the defective single bits  during a read and write operation. This  tool is required to  accurately characterize the failure mode to help with the failure  analysis . We focus us in this paper only on the failure mode  which exhibited a Soft failure.


Failure mode


Results of Emulator characterization


Vddmin


Write 1 or  0 or no possible result


Vddmax


Stuck at 1 or  0 or no possible result


Shmoo hole Write 1 or 0 or no possible result


Retention SBF on 1 or 0 retention or no possible result


Table 1: Results of emulator characterization according to  the failure mode of Soft Bit Fails


Table 1 summarizes the emulator characterization performed on  all rejects exhibiting a Soft bit fail according to the ATE results . For a Vddmin or Shmoo hole reject, the emulator  characterization exhibited a Write 1 or 0 or no possible  characterization. A  “Write 1 (i.e. 0)” failure means that it is  impossible to write the value 1 (i.e. 0) in the defective SRAM  cell.


For a Vddmax reject, the result showed only a stuck 1 or 0 or no  possible characterization. This “stuck at 1 (i.e. 0)” failure means  that the defective SRAM cell is blocked at the value 1 (i.e 0) but it is impossible to know if there is a problem in read or write  cycles or both.


For a Retention reject, with the value of the retention voltage in  checkerboard or in inverse checkerboard configuration given  by ATE, the emulator isolates the defective SBF with the data (1 or 0) of retention.


In the last part of this paper, we will show the importance of  this accurate characterization of the failure mode to correlate  with the defect. Utilizing the results from the emulator, and  logically applying the information to the schematic, a probing  solution can be created to focus on the possibly defective  transistor.


Advanced Electrical Characterization   by Nano Probing technique


Conventional physical failure analysis techniques (SEM, PVC, TEM analysis) could not resolve the soft bit failure defect. A  new approach was needed. A failing device was deprocessed  down to contact level for nano-probe analysis. Utilizing the  Nano-Probing technique, a complete electrical defect isolation  and characterization was performed in order to guide the  analysis by better understanding the electrical behavior of the  failing bit.


Description of Nano Probing technique


The Nano-Probing technique uses 4 tungsten needles  mounted to accurate micro-manipulators in a SEM chamber. . The 4 needles are connected to a curve tracer to collect I/V  characteristics.


There are several advantages of this technique on an SRAM  device. This technique is  non-destructive, does not alter the  integrity of the electrical and physical characteristics of the  measured transistors, does not need FIB/Probe pads and  allows the analyst to directly contact the VIAs or signal lines. Additionally with the use of SEM, it is easier to identify, by  counting rows and columns, the failing cell with the higher  resolution that cannot be attained under a standard light  microscope micro-probe station.


Electrical characterization of SRAM cell


The first capability of this technique is to electrically isolate  the defect at each layer of the die. In this case, this technique  allows to find an electrical resistive I/V characteristic or current  leakage between two signals or current leakage of gate, of P/N  or N/P junction.


The second capability of this technique is to characterize  electrically the physical parameters of transistors. This step is  performed at contact level because all the transistors of the  SRAM cell are isolated. At this level, the Nano-Probing  technique allows the collection of all NMOS and PMOS  transistors I/V characteristics. The electrical measurements  performed on the six transistors of the defective SRAM cell  are: Threshold Voltage (Vt), Gain and (BVDSS mode) offcurrent leakage of transistor. When the 4 needles are put in  electrical contact on the source, drain, gate and well of one  transistor, the curve tracer is configured to obtain the I/V  characteristic ID versus Gate/Source Voltage (VGS) corresponding to the ON state of the transistor. So, the ID (current flows between drain and source when the transistor is  in ON state) is read directly on this I/V curve. Concerning the


102


Vt and the Ron (resistance when the transistor is in ON state), the Vt value is extrapolated of this electrical curve and the Ron is  calculated from the equation of the I/V curve.


The electrical measurement (Vt, Gain and the current leakage in  BVDSS mode) of the SRAM cell must be performed on the six  transistors  characterizing Source to Drain and Drain to Source  in order to get a full electrical characterization. For comparison, the same electrical measurements were performed on a  reference SRAM cell to validate the results of the NanoProbing technique.


Cases studies


We present two cases studies of asymmetry of Vt, ID and Ron. The units failed “SRAM Vd dmin up to 1.4V”. The results of the  emulator characterization is Write 0 for the unit #1 and Write 1  for the unit #2.The PVC/SEM inspection until contact level did  not showed any physical anomalies (Figure.2) and the NanoProbing technique until metal 1 level did not electrically isolate  the defect: no resistive I/V characteristic or current leakage  were detected. Therefore, the electrical measurements were  performed at contact level on the six transistors in the two  senses (from Source to Drain and from Drain to Source). The  characterization by Nano-Probing technique for each unit is   summarized in the Table 2 and Table 3.The tables show the  value of Vt extrapolated from the I/V curves, the ID (Drive  current) at the voltage VGS equal to 0.8V, 1.0V and 1.2V and the  Ron calculated at VGS equal to 1.3 V.


Figure.2 SEM view of the defective SRAM cell of unit #1 and #2 (white rectangle). No physical anomalies or abnormal  passive voltage contrast were detected.


Table 2: Results of electrical characterization by NanoProbing  for unit 1


Table 3: Results of electrical characterization by NanoProbing  for  unit 2


Note 1: The data label “(source)”  in the transistor name means  that the source with the gate is connected to the collector of  the curve tracer and the drain is connected to the ground with  the well during the electrical measurement to obtain I/V curves. The data label “(drain)” in the transistor name  corresponds to  the inverse.


Note 2: We limit the current to 20-25µA and the voltage to 1.4-1.6 Volts during measurement to prevent possible electrical  degradation of measured transistors. This one explains the  indication “###” which corresponds to a ID value greater than  20-25µA but no measured.


Note 3: The margin of error of Vt value is defined by the  coefficient of the best fit line, the Vt calculation, the experiment  error and the calibration error of the curve tracer


103


Figure.3  I/V curve of Vt measurement of Bit pass transistor for  the unit #1 in the 2 senses (top excel chart) and  I/V curve of  Vt measurement of NBit pass transistor for the unit #2 in the 2  senses (down excel chart)


Interpretation of results


Unit #1, the results shown in Table 2 exhibit a high Vt, a low ID  and a high Ron of the “Bit pass transistor (drain)” versus the “Bit pass transistor (source)”. The graph Figure 3 revealed the  difference of the “Bit pass transistor (drain)” versus the “Bit  pass transistor (source)”.


Unit #2, the results shown in Table 3 also exhibit a high Vt, a  low ID and a high Ron of the “Nbit pass transistor (drain)” versus the “Nbit pass transistor (source)”. The graph Figure 3  revealed the difference of the “Nbit pass transistor (drain)” versus the “Nbit pass transistor (source)”.


The electrical measurements of the two units showed the same  results on the opposite transistors in the same defective side: Bit pass transistor for unit #1 and Nbit pass transistor for unit #2.


The drain Vt measurement was obtained by connecting the  gate and drain to the collector and the source and well to the  ground. In this configuration, the drive current flows from  Source to Drain. The defective sense for the two units is from  Source to Drain which corresponds to the Write mode.


The comparison of I/V curves of Vt measurement of source side  and drain side of Bit pass transistor (unit #1) and Nbit pass  transistor (unit #2) showed the non-superposition of the two  senses measurement (Figure.3). This one confirms the  asymmetry problem.


The asymmetry of Vt is 240mV (unit #1) and 250mV (unit #2). For the two units, it is important to note that the ID at  VGS=0.8Volts for source side corresponds about to the ID at  VGS=1.2Volts for drain side. The defective SRAM cell needs a  higher voltage than the typical values to obtain a sufficient  current ID to transfer the data 1 or 0 from source to drain (Write  mode). This could explain the voltage sensitivity observed  during ATE evaluation.


For both units, all other transistors of the defective bit cell are  functioning within typical values of Vt, ID and Ron. These ones  are symmetrical in the two senses of measurement.


Therefore, these defective units present asymmetrical Vt, ID and  Ron of Bit pass transistor for unit #1 and Nbit pass transistor  for unit #2.


The electrical characterization of the Soft Bit cell failure using  the Nano-Probing technique revealed electrical anomalies (Imbalance of Vt, low Gain, Asymmetry of Vt, ID and Ron). The  information “Write 1 or 0” characterized by the emulator and  the detection of asymmetry in the sense of the Write mode  associated a “Write 0 reject” with Bit pass transistor and a “Write 1 reject” with Nbit pass transistors. 98% of cases of  Vddmin and Shmoo hole (Write 1 or Write 0) revealed this  asymmetry phenomenon.


Few Soft Bit failures corresponding to the Vddmax and  Retention fails exhibited low Gain of one transistor or  imbalance of Vt between two pass transistors or between the  cross-coupled inverters without asymmetry phenomenon  Source/Drain of the same transistor.


TEM analysis


After electrical isolation of the defective transistor by these  different techniques, the TEM analysis was performed in an  effort to isolate the physical cause of the asymmetrical  phenomenon. The TEM analysis (Figure.4) of the defective  units did not show any anomalies of the gate oxide thickness, crystalline defect or geometrical problems.


104


Figure.4  Typical TEM view of  a Single Bit fail Vddmin


For the Soft Bit fails from one FAB, the result of TEM analysis  revealed a physical anomaly: a poly notch (Figure.5); however, this result could not be attributed to the cause of the  asymmetrical phenomenon.


Figure.5  TEM view of  a polynotch (black circle)


One hypothesis of root cause could be a problem in the  composition of the gate oxide or contamination non visible  during TEM analysis. Based on this information, the  asymmetry phenomenon or imbalance Vt between two  transistors could be a new failure mechanism.


The incorporation of Nano-Probing into the FA techniques to  solve the Soft bit fails allowed to isolate and to find an  electrical failure even though a physical defect was not found. The electrical characterization in addition with the emulator  results leads to obtain the accurate correlation between the  failure mode and the electrical measurement. After emulator  characterization, Nano-Probing can be performed once the  device has been deprocessed down to contact level.


An electrical methodology, emulator associated with the NanoProbing technique, results in a success rate increase on Soft  Bit failures.


The authors would like to thanks the NDAL team and TEM lab  in Dallas for the failure analysis work.


[1] Giret C. and Faure D., “Electrical Characterization by SubMicron Probing Technique on 90nm CMOS technology  for Failure Analysis ” IPFA 2004


[2] C.Giret, D. Bru, D. Faure, M. Razani and D.Gobled, “Measurements of electrical characteristics by 4tips-0.2  micron probing technique for Semiconductor Failure  Analysis ” ESREF 2002


[3] V.K Wong, C.H. Lock, K.H. Siek and P.J Tan, “Electrical  Analysis to Fault Isolate Defects in 6T Memory Cells” IPFA 2002


105


Dynamic Laser Delay Variation Mapping (DVM) Implementations and  Applications


Kevin Sanchez, Romain Desplats, Felix Beaudoin, Philippe Perdu


CNES - French Space Agency, 18, avenue Edouard Belin, 31401 Toulouse, France  kevin.sanchez@cnes.fr


Sylvain Dudit


ST Microelectronics, 850 rue Jean Monnet, 38926 Crolles cedex, France


Gary Woods


CREDENCE-DCG, 1299 Orleans Drive, Sunnyvale, CA 94089-1138, USA


Dean Lewis


IXL, Université de Bordeaux 1, 33405 Talence, France


In this paper we report on the application field of Dynamic  Laser Stimulation (DLS) techniques to Integrated Circuit (IC) analysis. The effects of thermal and photoelectric laser  stimulation on ICs are presented. Implementations, practical  considerations and applications are presented for techniques  based on functional tests like Soft Defect Localization (SDL) and Laser Assisted Device Alteration (LADA). A new  methodology, Delay Variation Mapping (DVM), will also be  presented and discussed.


Failure Analysis and debug of integrated circuits can be  tackled using optical techniques. These techniques make use  of the silicon optical transparency in the near infrared (NIR) wavelength range (Silicon bandgap = 1.12 eV). Thus, by  working from the backside of a device, IC diagnosis can be  conducted on devices which require sample preparation: silicon thinning and polishing. Optical techniques may be  divided into two groups: light emission and laser stimulation  techniques. In this document, we are interested in the latter  which consist of stimulating of a device using a laser beam. The laser beam injects photons locally onto an area of the  device. Depending on the laser wavelength (1064 nm or 1340  nm) these photons may induce current (electron-hole pair  generation) or heat (phonons).


Static laser stimulation techniques used on ICs are known as  OBIC (Optical Beam Induced Current) [1] or LIVA (Light  Induced Voltage Alteration) [2] and OBIRCH (Optical Beam  Induced Resistance Change) [3], TIVA (Thermally Induced  Voltage Alteration) [4] or XIVA (Externally Induced Voltage  Alterations) [5]. In those laser stimulation techniques, device  parameters are monitored (e.g., current, voltage) according to  the laser position in order to localize sensitive region which  may be related to defective areas.


The whole challenge of static laser stimulation techniques lies  in the detection scheme and the ability to detect extremely  small variations in order to catch a wide range of defects. The  implementation of those static techniques involves a low noise  current or voltage amplifier connected to the device power  supply as shown in figure 1.


Figure 1: General principle of static laser stimulation. All  pins are maintained at static level and electrical variations  induced by the laser stimulation are amplified and monitored  in synchronization with laser scanning.


The efficiency and success of static laser stimulation has  permitted, by a continual evolution, to follow the IC  technology and to access increasing numbers of defects. The  setup has become more complex, such as the introduction of  lock-in detection to increase the signal to noise ratio. A  significant change came from the device stimulation side: from a static configuration to dynamic stimulation. While the  former approach required only a power supply to power-up  the device under test, the latter now requires full activation of  the device (often with an electrical tester).


While the laser-semiconductor interaction remains unchanged, dynamic laser stimulation techniques monitor different  parameters such as laser induced delay. Since the device is  activated by a tester in a loop, the induced current or heat may  affect signal propagation, slightly slowing down or speeding  up some signals.


106


# Dynamic Laser Delay Variation Mapping (DVM) Implementations and Applications


Case Study IV – Exploring the TIVA technique in the  fault isolation of resistive interconnect issues


The fourth case study explores the use of the TIVA technique  in the failure analysis of memory devices with functional  failures due to resistive or open interconnects. The suspected  circuitries were specially edited using a focused ion beam  machine so that one end of the via chain was connected to  VCC and the other end was connected to GND. The objective  was to set up the desired biasing conditions for TIVA  analysis. A constant current source was then applied across  the via chain. The resistive via appeared as a dark spot in the  TIVA overlay, as shown in Figure 10. Figure 11 shows the  focused ion beam cross-sectional view of the unfilled via.


A constant current source was applied across the metal  interconnect consisting mainly of long metal runners. The  location of the void in the metal runners showed up as a TIVA  spot, as shown in Figure 12. Figure 13 shows the top-down  SEM image of the void in the metal one interconnect.


Resistive open


TIVA image


TIVA overlay image


Figure 10: TIVA image of metal interconnect via chain.


93


Figure 11: FIB cross section of the unfilled via.


Figure 12: TIVA image indicating the location of the void in  the metal runner.


Figure 13: A top-down SEM view showing void in the metal  one interconnect.


In this paper, we have demonstrated the use of TIVA in the  failure analysis of 0.11μm technology memory devices. TIVA  is capable of fault isolation in both resistive open and resistive  short failure mechanisms. In cases where EMMI failed to pick  out any hot spots, TIVA was still able to identify the metallic  shorted location. The ability of TIVA to map out the current  path of a short provides additional information which will aid  the physical failure analysis process. TIVA has an inherent  advantage over EMMI: the laser beam is able to penetrate the  dense device structures and cause localized thermal heating, whereas photoemission from a site inside a device may be  blocked or highly attenuated from reaching the collection  optics. The TIVA technique will be useful even for advanced  technologies.


The authors would like to thank Semicaps Pte Ltd’s staff for  their continuous support, and particularly Chua Choon Meng, CEO, and Tan Soon Huat, sectional manager, for their helpful  discussion during the development of this technique on  Micron memory devices.


[1] E.I. Cole Jr., P. Tangyunyong, D.A. Benson, and D.L. Barton, “TIVA and SEI developments for enhanced front  and backside interconnection failure analysis,” Microelectronics Reliability, Vol. 39, pp. 991-996, 1999.


[2] E.I. Cole Jr., “Global fault isolation using induced voltage  alteration,” Microelectronics Reliability, Vol. 41, pp. 1145-1159, 2001.


[3] N. Lucarelli et al., “Thermally induced voltage alteration  application to ESD induced failures,” Microelectronics  Reliability, Vol. 43, pp. 1699-1704, 2003.


94


Topside Defect Localization Using OBIRCH Analysis


Clifford Howard, Anusha Weerakoon, Diana Mitro, and Dawn Glaeser   Freescale Semiconductor, Inc.


6501 William Cannon Dr. West, Austin, Texas 78735 U.S.A.


OBIRCH analysis is a useful technique for defect localization


not only for parametric failures, but also for functional analysis. However, OBIRCH results do not always identify the exact  defect location. OBIRCH analysis results must be used in  conjunction with other analysis tools and techniques to  successfully identify defect locations.


OBIRCH


Optical Beam Induced Resistance Change (OBIRCH) is an


analysis technique in which a laser is scanned across a die or


area of a die. The localized laser heating causes resistance


changes in some defect types. The effects of the resistance


change are monitored for defect localization. The technique is


instrumental in quickly identifying defect locations on failing


units and improving failure analysis cycle time. Thermal laser


stimulation for locating faults has been described by Nikawa


and Tozaki under the name OBIRCH [1] and by Cole, et. al. as


TIVA [2]. The tool that was used for the work included in this


paper is a Phemos-1000 OBIRCH instrument from Hamamatsu


Photonics and the terminology used will reflect this.


OBIRCH has been shown to be an effective tool in localizing


defects that fail parametric tests [3]. Defects causing functional


test failures can be more difficult to localize. One method


utilized in this paper is an IDDQ-like current measurement nV taken at each vector during functional pattern execution on a


tester platform. The tester used for some of these cases is an


开钾司界钾43野


泼2科


ETS570 mini-tester from Hilevel Technology, Inc. The device  must be paused in a quiescent state for the current  measurement to be valid. This technique can be used for scan  or functional patterns as long as the clocks can be controlled  for quiescent current measurements. The high current probe  head option of the Phemos-1000 is used like an ammeter in  series between the Hilevel mini-tester power supply and the  microcontroller Vdd supply. Anomalous currents in the


quiescient state can be localized with OBIRCH using this  configuration.


In the cases in which the OBIRCH technique is used in  conjunction with an external power supply and the high current  probe head option, it was found that the OBIRCH signal was  not necessarily at the defect location. A combination of  OBIRCH, light emission, schematic analysis and micro-probe  was employed to determine the defect location. Once a failing


signal was isolated, OBIRCH was used again to isolate the  defect using the OBIRCH amplifier to supply a voltage or  current directly across a defect’s current path. This paper will  discuss how OBIRCH analysis was used with other techniques  for defect isolation with case studies from the topside analysis  perspective on functional failures.


Case 1


This case involved a 0.25um CMOS microcontroller with three  metal layers. The failure occurred in multiple scan patterns. The scan implementation on this device was Mux-D. A Hilevel


mini-tester was used to exercise the Device Under Test, or  DUT. The combinatorial logic between flip-flops changes as  the data is shifted into the chains. Current measurements were  taken on the core Vdd supply with the pattern execution paused  at each vector of the shift-in sequence. The measurements were  performed on a correlation unit and the failing unit. Anomalous  currents were observed on some of the vectors during the shift  in sequence (Fig.1). This technique identified contention in the  circuit.


Core Idd by Vector


0性性**--200


800


1200


1400


1600


1780


1800


1820


1840


Vector number


Idd Fail Idd Corr


Figure 1: Idd measurements while paused during scan chain  loading. The failing unit and the correlation unit core Idd  currents match except for the vectors indicated by the arrows.


OBIRCH analysis was performed using the tester as the power  supply and the high current probe head to monitor the core Idd  current. The DUT was paused on a higher current vector and  an OBIRCH image was obtained (Fig. 2). Light emission  analysis was performed under the same conditions and the light  emission overlay image was obtained (Fig. 3)


95


# Topside Defect Localization Using OBIRCH Analysis


Figure 2: OBIRCH overlay image obtained using the high  current probe head while paused on a high current vector.


Figure 3: Light emission overlay image obtained while paused  at the same high current vector. The white arrow points to the  location where the OBIRCH signal was observed.


The layout of the area was examined and one signal was found  that could account for the light emissions and OBIRCH signal  observed (Fig. 4). This signal, N3813, was micro-probed  through Focused Ion Beam, or FIB, deposited probe points to  obtain the functional waveform. The functional waveform


showed that when the signal was supposed to be driven to a  logic “1”, the signal would only reach about one fourth of the  voltage level expected. The N3813 signal node was electrically  characterized with a parametric analyzer and a resistive short to


Vss was observed.


At this point, the Phemos-1000 was used for OBIRCH analysis  once again. The positive node of the OBIRCH amplifier was  tied to N3813 and the negative node was tied to Vss. A  different OBIRCH signal was found at another location on the  N3813 node (Fig. 5).


Figure 4: Layout of the n3813 signal (highlighted in black). While only metal 1 (red) and contact layer are displayed, the  highlighted signal has other metal and polysilicon layers  displayed. The output drive transistor is in the lower right  corner (circle). The light emissions were observed at the gates  that the signal was connected to (arrows). The location of the  defect was found to be at the dashed circle and not at the  output drive transistors as initially indicated by OBIRCH  analysis.


Figure 5: OBIRCH overlay image obtained using the OBIRCH  amplifier supply forcing the N3813 signal voltage through a  micro-probe with Vss at 0 Volts.


Physical deprocessing was done using standard face lapping


techniques. A defect was found between the N3813 signal node  and Vss at the metal 1 layer (Fig. 6). An SEM cross-section


image showed bridging metal between the N3813 signal and


Vss (Fig. 7)


Signal


Probe Points


Probe  Needle  shadow


96


Figure 6: Optical microscope image showing the defect.


Figure 7: SEM cross-section image of the defect.


Case 2:


The next analysis was performed on a 0.25um CMOS  Microcontroller device with three metal layers. A Hilevel minitester was used to confirm the scan failure.


As in Case 1, the power supply current measurement method  was used to collect the Idd current at each test vector in a scan


pattern for the failing unit and a correlation unit (Fig. 8).


Light emission and OBIRCH analysis using the high current  probe head was performed while paused on one of the high  current test vectors on the Hilevel mini-tester. Unique light  emission (Fig. 9) and OBIRCH sites were found (Fig. 10).


0 100 200 300 400 500 600 700


Test Vector #


Fail (uA)


Corr (uA)


Figure 8: Current on VDD by test vector


Figure 9: Unique light emission sites while pausing on a high  current test vector


Figure 10: OBIRCH image while paused on high current  vector. The dotted circle shows a diffuse OBIRCH site and the  solid circle shows a well defined OBIRCH site.


Area should not


have metal


97


It was noted that the two OBIRCH signals that were detected, appeared to be different in nature. One OBIRCH site was  diffuse and one was well defined.


The layout of the light emission and OBIRCH areas were


analyzed. It was found that all of the light emission and


OBIRCH sites could be attributed to one signal, n463. Further  inspection of the layout of the locations of the OBIRCH and


light emission sites identified a node to be micro-probed in


addition to n463. This node, IPBI__831 ran parallel to n463 at  metal 2 in the area of the light emission and the well defined  OBIRCH site. The diffuse OBIRCH signal was seen at the pchannel output drive transistor for n463. Functional microprobe of these nodes showed mid-band voltages on both  signals indicating a resistive short between the signals.


In order to further isolate the location of the short between  IPBI__831 and n463, OBIRCH analysis was performed using  the OBIRCH amplifier. The positive and negative sides of the


OBIRCH amplifier were tied to the micro-probe needles on the


suspected nodes to directly force a voltage across the suspected  defect. A unique OBIRCH site was identified (Fig. 11).


Figure 11: OBIRCH image while biasing one signal and  grounding the other with micro-probes.


The unique OBIRCH site (Fig. 11) corresponded to the welldefined OBIRCH site initially observed and one of the light  emission sites. At this site, IPBI__831 and n463 routed next to  one another in metal 2.


The failing unit was deprocessed using standard face lapping  techniques. An anomaly at the OBIRCH site was found at the  metal 2 layer (Fig. 12). A FIB cross-section was performed on  the anomaly perpendicular to the metal 2 lines (Fig. 13). The  defect observed appeared to be thin and probably higher  resistance than the defect found in Case 1.


Figure 12: Optical photo of anomaly at the OBIRCH site in  Fig. 11.


Figure 13: FIB cross-section image of defect shorting  IPBI__831 and N463


Case 3


This case involved a 0.5um CMOS technology microcontroller  with two metal layers. This device was exercised on an  evaluation board, or EVB, because the code to exercise the fail  mode was readily available. The device failed to toggle a  register bit, MCS, when programmed on the EVB.


Liquid crystal and light emission analyses were performed but  no anomalies were detected. OBIRCH analysis was performed  with microcontroller executing code to toggle the MCS register  bit. The high current probe head was used between the EVB  power supply and the core Vdd supply of the microcontroller. No OBIRCH signals were detected. A change in the EVB code  was done to set and hold the MCS bit high without stopping  the clocks on the microcontroller. Again, no OBIRCH site was  observed.


IPBI__831


Defect at Metal 2


N463


98


The circuitry associated with the MCS bit was micro-probed to


narrow the failure to a small area. The failing node, MCS, was  found to be pulled to a mid band voltage compared to the same  node in a correlation unit. The input to the inverter that


generated MCS was normal. The MCS node was then


electrically characterized with a parametric analyzer with


respect to VSS but no leakage or shorts were detected.


Light emission analysis was then repeated with the MCS signal  driven high. Light emission sites captured with the CCD


camera on the Phemos-1000 were noted at the gates of a signal  that had an adjacent metal line (Fig. 14). It was hypothesized  that the adjacent signal, BCSS, was held in co tention because


of a short between the MCS and BCSS metal lines. This would  result in an intermediate voltage on both signals. Figure 15  shows the layout of the area where the light emissions were  found with the MCS and BCSS signals highlighted.


Figure 14: The arrows point to the CCD light emission sites


on the die.


Figure 15: Layout image that shows the failing node, MCS,


and the adjacent metal line, BCSS. The area of light emission


is indicated by the black rectangle.


The MCS and BCSS nodes were electrically characterized and  found to have a short between them.


Case IV


In this case study we looked at a front side device where a  short between VDD and ground was measured during  electrical analysis.  We then used both photoemission and  thermal emission with the same camera and optics to diagnose  the location of the defect.  As shown in Fig. 17, the thermal  emission image gives one additional site when compared to  the photoemission image.  This corresponds to the location of  a purely resistive short that is emitting heat because of the


burned metal lines


Joule effect.  Deprocessing of the die confirmed a metal to  metal short at the location of the extra thermal emission site.  In this case, the photoemission mode was able to detect faults


p印[q]


by getting the emission of all gates that were incorrectly  biased, but the thermal image provided the exact defect  localization.  The ability to switch between photo and thermal


Q0Q


emission modes without changing the setup is beneficial in  minimizing the debug time.


One requirement for thermal emission is the ability to


OG顶]


synchronize the power supply that switches the device ON and  OFF with the acquisition of the detector.  This is especially  true in the new thermal cameras with an extended spectral  response.  As sensitivity increases with the cutoff wavelength  of the focal plane array going from 2500nm to 3000nm, the  detector saturates in less than 100ms at 1x under normal  operating conditions, simply because of the blackbody  radiation of the room.  Therefore, the improved detectors  require better synchronization with the tester or the power  supply controlling the DUT.


88


Figure 17.  A resistive short produces only heat whereas all  the wrong biased gates are showing both photo and thermal  emission.  In this case, photoemission does fault detection  whereas the thermal image pinpoints the origin of the fault.


We have demonstrated the advantages and limitations of EM  and LSM as valuable silicon FA techniques, and how they  could be complementary for shortening the diagnostics time.  In general, EM requires less tuning to start the analysis.  It  typically reveals more information than required, because not  only does the defect emit, transistor gates that are either  associated with the defect, or are driven under the specific bias  conditions also emit.  LSM is more selective, showing only  the location of anomalous current density.  However, the  detection of LSM stimulation is more difficult at lower  magnification, due to the fact that the spot size of the laser  beam could be too large compared to the defect size.


The authors gratefully thank NVIDIA Silicon Analysis Team  and Checkpoint Technologies for their assistance.


[1] J.A. Kash and J.C. Tsang, “Dynamic Internal Testing of


CMOS Circuits Using Hot Luminescence”, IEEE Electron


Device Letters, vol. 18, No. 7, July 1997.


[2] Stas Polonsky and Alan Weger, “Off-state Luminescence


in Metal-Oxide-Semiconductor Field-Effect-Transistors


and its Use as On-chip Voltage Probe”, Applied Physics


Letters, vol. 85, No. 12, September 2004.


[3] J.C. Tsang and J.A. Kash, “Picosecond Hot Electron Light


Emission from Submicron Complementary Metal-OxideSemiconductor Circuits”, Applied Physics Letters, vol. 70,


no. 7, July 1997.


[4] P. Vedagarbha, G.Woods, H. Koike and K. Sanchez,


“Laser-Induced Debug and Failure Analysis”,


Semiconductor International, December, 2004.


[5] E.I. Cole Jr., P. Tangyunyong, C.F. Hawkins, M.R. Bruce,


V.J. Bruce, R.M. Ring, and W.L. Chong, “Resistive


Interconnection Localization,” International Symposium


for Testing and Failure Analysis (ISTFA), pp. 43-50, Nov.


2001.


[6] M.R. Bruce, V.J. Bruce, D.H. Eppes, J. Wilcox, E.I. Cole


Jr., and P. Tangyunyong, “Soft Defect Localization (SDL)


on ICs,” International Symposium for Testing and Failure


Analysis (ISTFA), pp. 21-27, Nov. 2002.


[7] D. Lewis, V. Pouget, F. Beaudoin, G. Haller, P. Perdu, and


P. Fouillat, “Implementing Laser-Based Failure Analysis


Methodologies Using Test Vehicles”, IEEE Trans. On


Semiconductor Manufacturing, vol. 18, no. 2, May 2005.


89


Scanning Optical Microscopy Application in Micron® Memory Devices


Wong Yaw Yuan, Edmund Poh, David Lam


Micron Semiconductor Asia Pte. Ltd., Singapore


wongyyuan@micron.com, edmundpohtl@micron.com, davidlam@micron.com


The migration to smaller geometries has translated to an  increase in the number of transistors possible in each  integrated circuit. Failure analysis of such complex circuits  presents a major challenge to the semiconductor industry and  is a driving force behind the considerable interest in  nondestructive, cost-efficient, “shortcut” fault isolation  techniques. In this paper, we present the application of  thermal-induced voltage alteration (TIVA) for failure analysis  of 0.11µm technology memory devices and demonstrate the  key aspects of this technique. The back side TIVA results are  compared with analysis performed using back side emission  microscopy (EMMI), and the limitations of EMMI are  highlighted. The advantages and limitations of the TIVA  technique are also discussed.


Index Terms – TIVA, thermal-induced voltage alteration, EMMI, emission microscopy.


Memory circuits fail for many of the same reasons as other  integrated circuits—high operational and standby currents or  parametric and functional failures. With the rising interest in  thermal-induced voltage alteration (TIVA) techniques for the  failure analysis of integrated circuits, many applications have  been developed [1-3]. We have seen numerous improvements  and innovations to the TIVA technique, the latest being the  laser pulsing technique, in which a laser is turned on and off at  a preset frequency along its scan line.


We explore the use of TIVA to improve our failure analysis  process. The devices under test (DUT) are biased, using either  a self-fabricated switch box or DC active probes. The  scanning optical microscope (SOM) system used in the


78-3


evaluation was the Semicaps SOM1005, available from


Inscope Labs, and the back side photoemission microscope  used was the PHEMOS1000 system from Hamamatsu.


Working Principle


TIVA is a nondestructive fault isolation technique. The whole  concept of this technique is based on the Ohm’s law equation, V = I * R, where I is kept constant. In the experiment, the  DUT is first biased using a constant current source. A highpowered infrared red (IR, λ=1300nm, 500mW) Nd:YAG laser  beam is used as a localized heating source to induce changes  in the resistivity of the materials in the chip along its scanning  path, thus producing voltage alteration, which can then be  recorded as an “alteration mark.”


The setup for TIVA investigation on Micron® memory  devices is similar to that for back side EMMI analysis. Since a  bench-top tester is not available at the external lab, a selffabricated switch box is being developed for the purpose of  biasing the device into standby mode. It is absolutely critical  to bias the DUT into proper standby condition; that is, the  leakage location consuming power while all other circuits are  turned off. This is to maximize the signal-to-noise ratio of the  TIVA signal. For TSOP packaging part types, a deadbug  socket test card (see Figure 1) is designed to contain the back  side slot-decap unit such that the back side (bulk silicon) of  the device faces the optical microscope lens. For board-onchip (BOC) or flip chip packaging part type, the top side of  the package can be simply removed to expose the back side of  the die. An overview of the setup of the SOM system for  TIVA analysis is shown in Figure 2.


Figure 1: Deadbug socket test card holding a slot decap unit.


90


# Scanning Optical Microscopy Application in Micron Memory Devices


Figure 2: Block diagram of the setup of the SOM system for  TIVA analysis.


Case Study I – Application of current path mapping in  TIVA analysis to identify the possible levels of short


The first case study illustrates the feasibility of TIVA for fault  isolation of memory devices with current leakage failures and  shows how the current path aids in the physical failure  analysis process. A 256Mb memory device was reported to  have high operating and standby current. Both EMMI and  TIVA analysis were performed and the results are shown in  Figure 3. The back side EMMI image (top) shows a single  emission location. The TIVA image (bottom) maps out the  current leakage path. From the current leakage path, the  layout, and electrical analysis, we were able to isolate the  signals that were shorted and found that the prime suspect of  the short lay in the metal two level. Figure 4 shows the topdown SEM view of the contamination shorting the metal two  runners. This contamination confirmed our hypothesis. Given  the current path and the die layout, it is possible to postulate a  short to a specific metal line. This finding could prove to be  critical as technology continues to scale down to the 65nm  node where spatial resolution is limited by the capabilities of  optic lenses.


Deadbug tool


DUT  Optical


microscope  Shielded box


Switch box


SOM-TIVA  PSU


Bandpass  filter


Figure 3: A comparison of the results obtained between  EMMI and TIVA analysis.


Figure 4: Metallic contamination was found shorting the two  signals, corresponding to our understanding from TIVA  current mapping, electrical analysis, and circuit layout  tracing.


Case Study II – Application of TIVA in detecting resistive  shorts between the metal one runner and the cell-top plate


The second case study illustrates the ability of TIVA to detect  contamination in the BPSG layer, causing a short between  metal one and the cell-top plate. A 512Mb memory device  was confirmed to have marginally high operating and standby  current. Under EMMI analysis, the failing device exhibited no  distinct illegal photoemission. However, TIVA analysis  revealed the current paths associated with the short, as well as  the exact location of the short, as shown in Figure 5. The  focused ion beam (FIB) cross section at the suspected location  revealed the presence of contamination in the BPSG layer, shorting the metal one runner and top-cell plate, as shown in  Figure 6.


TIVA image  EMMI image


Figure 5: TIVA analysis pinpointing the exact location of the  short at 20X optical magnification.


Figure 6: Metallic contamination in the BPSG layer causing a  short between the metal one and top-cell plate.


There are two possible hypotheses for why EMMI could not  pick out the shorted location while TIVA could. First, the  short was a subtle one. It belonged to a rather resistive  category, and the thermal emission it exhibited was in the  deep infrared (IR) region. Second, the amount of thermal  emission coming out of the shorted location was highly  attenuated by the dense cell container structures and  polysilicon gates. TIVA located the short because it heated up  the device as the laser scanned along the preset path. The  dense structure posed no barrier to the penetration of the laser  beam, and by varying the intensity of the laser’s power, we  obtained an alteration mark, which was sufficiently magnified  to show the shorted location.


Case Study III – Examining the sensitivity of TIVA in  detecting very resistive shorts between two metals


The third case study examines the sensitivity of TIVA in  detecting minute current leakage as a result of a very resistive  short between two metal lines. Several 256Mb memory  devices were reported to have pin leakage issues. The  electrical signature showed that the failing pin was shorted to  ground with a leakage current varying from 6μA to 110μA. Curve tracing revealed that the short bore ohmic  characteristics; thus, it was probably a metallic short. A study  was conducted to understand how the sensitivity of the TIVA  technique fares with respect to the changes in device biasing  conditions and laser power intensity. It was proven that TIVA  could detect and pinpoint the location of the metal short even  down to 6μA of leakage current, as shown in Figure 7.


Short location


Figure 7: TIVA image of a 6μA pin leakage unit.


We attempted to vary the magnitude of the current source  from 2μA to 50μA. We kept the gain constant under fixed  bandwidth and adjusted the laser power to obtain a TIVA  signal significant enough to identify the short location. The  results are shown in Figure 8. Using a biased current source  as low as 2μA, we were still able to detect the TIVA signal  with as little laser power as 65 percent. This is important  because as the operating voltage of future devices decreases, it  will still be possible to obtain a TIVA signal despite the  minute current leakage caused by the short.


92


I = 10μA, V = 0.245V


Figure 8: A summary of the TIVA results obtained by varying  the base current and determining the minimum laser power to  obtain a distinguishable TIVA spot.


Figure 9 shows a cross-sectional view of the subtle metal-tometal short between the leakage pin and ground.


|I = 50μA, V = 0.863V |||
|---|---|---|

|I = 20μA, V = 0.464V |Minimum laser |power = 20% |

|I = 20μA, V = 0.464V |Minimum laser |power = 30% = 35% |

|I = 5μA, V = 0.128V |Minimum laser power |power = 30% = 35% |

|I = 5μA, V = 0.128V |Minimum laser |power = 30% = 35% |

|I = 5μA, V = 0.128V |I = 2μA, V = 52mV |Minimum laser |

Figure 9: Cross section reveals metal short between the  leakage pin and ground.


The goal of this paper is to present the implementation of  dynamic laser techniques and the practical challenges of  synchronizing a scanned laser beam with a tester. After a brief  review of laser-semiconductor interaction (dynamic signal  propagation variation) we will present LADA [6], SDL [7] and RIL [8,9] implementation with two short examples. Shmoo plots, functional tests and laser synchronization are  important factors to be looked at to conduct a successful IC  analysis. Finally, we will address the latest technique: Delay  Variation Mapping (DVM). With DVM, timing information is  monitored directly on one output pin and laser induced delays  can be tracked with greater sensitivity than previous  techniques. Delay Variation Mapping can be conducted at  high laser scanning speeds, greatly reducing analysis time. Implementation of Delay Variation Mapping, in both  frequency monitoring and direct time variation approaches, will be detailed.


Dynamic laser-semiconductor interaction


Near infrared laser stimulation is chosen for its capability to  penetrate the silicon substrate. It can be used to deliver an  accurate quantity of energy from the front or through the IC  silicon substrate (back side). The deposited energy locally  changes the IC electric properties and affects static electric  conditions and dynamic behavior. Two lasers effects, thermal (with a laser around 1300 nm) and photoelectric (with a laser  at 1064 nm), are used to induce various electrical  modifications. We measure the induced disturbances by laser  stimulation and process them for static and dynamic  applications.


Thermal Laser Stimulation (1340 nm)


A 1340 nm wavelength laser is used to perform Thermal Laser  Stimulation (TLS) from the front side or backside of ICs. Thermal Laser Stimulation locally increases the temperature (dT) of the material and changes its resistance (dR) as  highlighted in equation 1 for a metal line. ρ0 is the metal  resistivity at the reference temperature, L and S are  respectively the length and section of the line, αTCR is the  temperature coefficient of resistivity and δT the thermal  expansion coefficient.


)dT


S


L


dR


TCR δα


ρ


0 −


Eq(1)


In static applications these electrical alterations induce power  supply variations (current or voltage) and are exploited by  OBIRCH or TIVA techniques. Those techniques are known to  localize a wide range of defects such as polysilicon shorts, via  defects or voids.


In dynamic conditions, the device is activated and the  electrical variations induced by TLS influence the metal  propagation delay and the switching time of the transistors. A  resistive path may jeopardize device timing. If unexpected  resistance is caused by a local defect, heating the defect by  laser stimulation can slightly change signal propagation.


In figure 2, electrical simulation shows the effect of thermal  laser stimulation on a defect characterized by a positive  temperature coefficient of resistivity. In this case, signal  propagation is slowed down and the delay increases upon  TLS. The curve in figure 2 shows the buffer output signal  delay at several laser powers for both rising and falling edges.


Figure 2: Thermal dynamic laser stimulation of one resistive  defect between two successive inverters. Output switching is  affected as a function of internal heating, and time delay  variations are exploited to localize laser-sensitive areas.


The other effect induced by TLS is the perturbation of MOS  transistor switching time by heating contacts, junctions and  channels [10,11]. Thus, dynamic Thermal Laser Stimulation  can be used for defect localization, for timing characterization  or for localizing design anomalies.


Photoelectric Laser Stimulation (1064 nm)


Upon Photoelectric Laser Stimulation (PLS), electron-hole  pairs are generated in silicon. This carrier generation, G, in  silicon follows a Gaussian distribution (equation 2) and is a  function of the laser wavelength, laser intensity I0, axial  coordinate z and silicon absorption α related to the substrate’s  doping. η represents the photo-generation efficiency. w0 and  wSi(z) are respectively the beam waist at the focal point and  the beam radius at a distance z from the surface. [12]


z


hv I


G


Si α


ηα


(2


2 0


Eq(2)


With a laser at 1064 nm wavelength PLS can be performed on  the front and backside of a device. Generated electron-hole  pairs are dissociated by the internal electric fields due to  external biasing and PN junctions to generate a photocurrent. This photocurrent alters the electric properties of the IC and is  exploited by static techniques, OBIC and LIVA, to localize  junction issues, to read static transistor states (ON or OFF) or  other techniques, such as latch-up characterization.


On an activated IC, the photocurrent flow perturbs the electric  functionality of CMOS transistors by modifying the transistor  bias point and parasitic capacitance characteristics [13,14,15]. In order to determine the dynamic behavior of CMOS  structures under photoelectric laser stimulation, a simple  buffer was electrically modeled (left of figure 3). Transistor  characteristics were chosen to match with experimental results  obtained under PLS on PMOS and NMOS transistors. The  input voltage was varied from 0V to 4V and the output voltage  was calculated for both rising and falling edges at different  laser powers.


107


Figure 3: Electric simulation of photoelectric laser  stimulation on CMOS buffer, transistor illuminated: NMOS  and PMOS.


The influence on the dynamic behavior of the buffer stage  upon photoelectric laser stimulation on both NMOS and  PMOS transistors is shown in figure 3. We observe an output  signal advance or delay under PLS. This perturbation is a  function of the input rising or falling edge and the illuminated  NMOS or PMOS transistors. For an input rising edge, the  output signal is advanced when the NMOS transistor is  illuminated, and is delayed when the PMOS transistor is  illuminated. The opposite behavior is obtained for an input  falling edge.


We also observe that the output voltage pulse width is  increased when the NMOS transistor is illuminated and  reduced when the PMOS transistor is illuminated. This is  illustrated in figure 4.


Figure 4: General principle of delay variation and pulse width  variation induced by photoelectric laser stimulation on CMOS  inverter.


Thus, Photoelectric Laser Stimulation directly affects the  functionality of CMOS structures and advances or delays  signal propagation. Dynamic laser stimulation with PLS can  be used for the study of critical paths, timing characterization  or for the localization of design anomalies It can also be used  for the localization of defects such as junction issues. In fact, the PLS of defective gates or the presence of defects can  induce different timing variations.


Dynamic laser testing of ICs


Dynamic Laser Stimulation techniques are used to analyze  devices for which the failure can not be activated in static  mode. For dynamic laser testing, the device is activated by a  test pattern in a loop and PLS or TLS is applied. We have seen  that laser stimulation (TLS and PLS) can modify the time  delay propagation of gates and lines and affect the IC gate  delay. The challenge is to detect the very small variations


induced by laser stimulation as a function of the laser beam  position and the input vector.


The first approach for locating laser sensitive areas (as in  static laser stimulation) would be to monitor power supply line  variations. Pseudo-static IDDQ has been developed to observe  the power current variation as a function of input vector and  laser beam positions. But, the sensitivity is not always  sufficient to detect small laser induced electrical variations  due to noise generated by the tester. One other approach, developed in 1980, combines marginal voltage analysis with  photoelectric laser stimulation to localize design, process or  physical defects [16]. A key element of this approach involves  setting the device at the boundary between passing and failing  by controlling external parameters, in this case the power  voltage, to increase the laser stimulation effect.


However, not all dynamically activated circuits can be brought  to a halt at a given failing vector. Also, abnormal behavior  induced by soft defects, glitches, or time margin issues can not  be studied in a pseudo-static configuration. Only by activating  and testing the IC at full speed can such problems be tackled  by DLS.


Functional testing


To validate device behavior according to its specifications we  need to conduct a functional test. This test compares measured  outputs with expected ones where, for digital devices, possible  logical output states are either high (H) or low (L). For test  purposes, two other values may be found: for expected data, “X” is used to ignore the measured output value for the  comparison and “I” for indeterminate value measured by the  tester, when the measure is neither H nor L. During IC  functional tests, the measured outputs are compared with the  expected values for all input configurations chosen by the  user. The final result is either PASS, when all measured  vectors match the expected ones, or FAIL when one or more  differences are found.


Figure 5: Functional testing principles. Measured data (output vectors) is compared to expected data. The result is  either PASS or FAIL.


While functional testing appears basic, practical application  can become very complex. Indeed, levels and timings of all  pins must be set properly. If we were to take a basic counter  block, the device might work properly but fail the functional  test if the output strobe (when measurement occurs) was set


108


too early. As a result, the data would not be ready and the  measure would correspond to the previous expected count  value.


In dynamic laser stimulation based on functional tests, laser  stimulation is employed to perturb the IC dynamic behavior  and the functional test is used to detect the perturbation. For  example, without laser stimulation, the functional test of a  device under test is PASS and, under laser stimulation (PLS or  TLS), the same functional test can switch to FAIL. For  dynamic laser testing, the induced delay may be very small, a  few tens of picoseconds or less. In that case, the placement of  the output strobe plays a decisive role in detecting such  variations. In order to find optimal settings, several  configurations must be tried beforehand. Without going into  the details of parametric testing, several parameters are well  known to influence a functional test, such as: VDD level, frequency and temperature. Finding the appropriate setting can  be achieved with the next testing technique known as Shmoo  plotting with electric characterization of the IC failure mode.


Shmoo plots


A Shmoo is a cartoon creature, created and first drawn by the  cartoonist Al Capp. The Shmoo is shaped like a plump  bowling pin with legs, but no arms. This description was  brought to the testing world for mapping functional test results  in 2D vs. two parameters. The objective of a Shmoo plot is to  determine the influence of two parameters on device  functionality. In the example here, power supply and cycle  time (frequency) are studied. For each VDD and frequency  chosen between two limits, a functional test is run. Therefore, a multitude of tests are run automatically and displayed in a  2D matrix image.


Figure 6: Sample of Shmoo analysis. It shows the device  functionality as a function of external parameter variations  between two limits. In this case: frequency variation as a  function of power voltage variation. The gray color represents  the normal device functionality.


With this view it is much easier to find optimal IC  combinations for increasing dynamic laser stimulation  performance. In fact, if the IC VDD and frequency are chosen  close to the boundary between the PASS and FAIL areas (gray  and white in figure 6) the laser stimulation (PLS or TLS) effect is more able to change the IC functional test to PASS at  FAIL or to FAIL at PASS. Being close to the border raises the  chance of detecting the small laser influence.


Testing for DLS consideration


Practical considerations concerning the use of Shmoo plotting  involve laser-semiconductor interaction: In the case of a 1064  nm wavelength laser, for example, induced current depends on  a wide range of parameters [17] and usually has more effect  on delay propagation than do thermally induced disturbances. Another consideration of Shmoo plotting concerns high power  devices where the boundary between PASS and FAIL is rather  unstable when the same Shmoo plot is re-run. As a result, being too close to this frontier may yield unpredictable results  when combined with dynamic laser testing.


Dynamic Laser Techniques Implementation


DLS-tester Principle


Dynamic Laser Stimulation techniques such as Soft Defect  Localization (SDL), Laser Assisted Device Alteration (LADA) and Resistive Interconnection Localization (RIL) are  based on the functional test technique for characterizing  defective ICs. With these configurations, a laser beam (at 1340  nm for SDL and RIL and 1064 nm for LADA) scans an area  of the device pixel by pixel. For each pixel, a functional test is  run and a map is obtained, similar to a Shmoo plot. In this  case, X and Y represent the laser position on the circuit and  the color indicates the PASS or FAIL status. Ideally, when the  laser power is off, the resulting image should reveal only one  color, the functional test always being PASS or FAIL. When  the laser power is on, a few areas will appear differently, corresponding to laser sensitive areas.


DLS-tester Implementation


Implementation of such techniques requires the following  equipment: A laser scanning microscope (a motorized stage  being less efficient), a powerful enough laser source and a  tester to run the functional test. For practical considerations, a  video card is used to overlay the PASS or FAIL status (color) to an image of the area of the device.


To obtain a meaningful image, the laser scanning position  must be known while a functional test result is obtained. In the  simplest configuration, the LSM scanning signals (pixel, line  and frame clocks) are sent to the video card. Two other analog  inputs are used: one to take the laser reflected signal (voltage) and display an image and another one to grab the PASS or  FAIL status.


Concerning the synchronization between laser scanning and  device activation, the easiest DLS approach is to scan a device  pixel by pixel with a continuous laser beam. At each pixel, a  test sequence is sent to the device and the laser influence over  the whole test sequence may be detected. The best method to  ensure one test cycle per pixel is to use the pixel clock signal  to trigger the tester. In this case, the execution time of a test  sequence must be smaller than the pixel dwell time. But, for a  long test pattern, this approach may become prohibitive for  acquiring a 512x512 pixel DLS image, or impracticable to set  up if the maximum dwell time per pixel is smaller than the test  sequence duration. As a result, other approaches are used to  speed up the acquisition. In our view, asynchronous DLS (no


109


synchronization between laser scan and tester) is often the best  approach.


Figure 7: Setup for dynamic laser stimulation combining PLS  or TLS with functional test (RIL, LADA, SDL)


DLS-tester methodology


The key then is to acquire the PASS/FAIL (P/F) status from  the tester and feed it to the video card input with the proper  voltage levels. On most testers, comparison between the  measured data and expected output is done using a hardware  real-time comparator unit. Unfortunately, this unit is often  mixed with other tester electronic functions. To our  knowledge, only a few testers may have a real time  comparator signal available.


Another way to get the P/F status is to allocate an additional  output pin on the tester. This pin, DLS_OUTPUT, is not  connected to the device under test but sent directly to the LSM  video card. The advantage of this solution is that the level (e.g., 0 to 1 Volt amplitude) can be set easily on a tester. The  difficulty is maintaining the P/F status long enough for the  video card to grab the information. One solution is to duplicate  the test sequence. Instead of running one test sequence in a  loop, a conditional jump can be made to loop either the first  sequence or the duplicated sequence. If the functional test  yields a pass status, the first test sequence is looped and the  DLS_OUTPUT is low for all vectors. If the functional test  yields a fail status, then test sequence 2 is looped and the  DLS_OUTPUT is high for all vectors.


Figure 8: Software PASS/FAIL grabbing technique: duplication of test sequence and allocation of additional pins.


DLS-tester implementation summary


The above DLS-tester implementation scheme is fairly  straightforward. No additional hardware is required except for  one output pin (DLS_OUTPUT) allocation on the tester side.


Limitations of this approach are related to vector sequence  duplication, which works only if the tester memory depth is  sufficient, and to laser scanning speed versus time to execute a  functional test. Practical setup involves reduction of the test  sequence in order to spend as little time as possible per pixel. Another improvement involves using the LSM pixel clock as  an external trigger to control tester execution (e.g., to start the  functional test in a synchronous mode).


To optimize tester-video card synchronization, electronics can  be added to latch the PASS/FAIL pulse status, just long  enough to be valid for the video card.


DLS-tester implementation advantage and drawbacks


Dynamic analysis of integrated circuits often requires an  electrical tester to stimulate the device in a loop. Taking  advantage of its great testing capabilities makes sense. Most  testers are not yet “DLS ready” but easy hardware  implementation is possible by means of allocating an  additional output pin on the tester.


Conducting a successful DLS analysis requires knowledge of  laser-semiconductor interaction (e.g., device more sensitive at  low VDD) and a good knowledge of electrical testing. The  Shmoo plot approach is a useful test method for determining  the PASS/FAIL boundary. One last important parameter is the  number of vectors in a test sequence and the time required to  run such a sequence. As for all dynamic testing and probing  techniques, valuable time may be saved by fine tuning such  parameters.


DLS-tester case study


Several ASICs were found to fail in small temperature  windows. The failure is observed through a frequency  variation on one output. Initialization of the device is  composed by a voltage ramp, a short waiting time and an input  clock application. Depending on the temperature, the device  runs correctly or not. If the clock frequency is measurable on  one output, the device passes and fails when this output  frequency is different.


Device temperature is controlled by a thermal head and is  chosen to set the device in its failed mode. Thermal laser  stimulation is employed to locally heat the device and change  its functionality from fail to pass. The resulting DLS images  are in two colors, white for fail which are areas not sensitive to  TLS and black for thermally sensitive areas for which the  device is functional (fail-to-pass transition). The following  images are obtained. Three thermally sensitive areas are  localized. The first DLS image is acquired with a 5X objective  and the following three superimposed images are obtained  under higher magnification on each sensitive area.


The test sequence duration is 40ms and the laser scan speed  was chosen to maximize the illumination time per pixel at  10ms. In this condition, the mapping localization accuracy is  four pixels, which is not an issue here considering the wide  thermally sensitive areas. Such wide sensitive areas indicate a  design-process issue rather than a physical defect. Furthermore, we have localized the same three thermally  sensitive areas in two different devices which failed in


110


different temperature windows. Finally, no thermally sensitive  areas were found on electrically good devices. Improvements  in the circuit design to overcome the design-process  temperature sensitivity are underway.


Figure 9: Functional test dynamic laser stimulation with TLS. Localization of three sensitive areas (black), that switches the  device functionality from pass to fail.


Delay Variation Mapping (DVM)


A promising improvement to actual Dynamic Laser  Stimulation techniques is to directly observe the output signals  of a dynamically activated device upon laser stimulation. In  fact, when the laser induces a delay inside the device, this  delay may then be propagated to the output pins. By  monitoring the output pins it is possible to relate signal  propagation variations with laser position on the device.


DVM principle


Going back to laser-semiconductor interactions, laser  stimulation may induce an additional current flow in the  semiconductor active areas or a heat induced resistance  variation. When the device is activated by a test sequence, this  additional current or resistance variation can affect the gate  delay, thus modifying the total signal propagation delay. LADA, SDL and RIL techniques rely on the electrical tester  capabilities to detect signal propagation through a functional  test. With the Delay Variation Mapping (DVM) technique, the  signal propagation delay under laser stimulation is obtained by  measuring the propagation time according to the laser  scanning position. The principle of DVM is illustrated in  Figure 10.


The objective is to overcome the PASS/FAIL status limitation  and to directly measure a value in picoseconds instead. With  this approach, small variations (e.g., while maintaining a  PASS state) are measured as well as significant ones (e.g. PASS to FAIL).


Figure 10: Delay Variation Mapping: time delay  measurement is performed between input device activation  and output switching under laser stimulation.


DVM implementation


Laser induced delay variations are in the order of picoseconds  and nanoseconds. Such time measurement capabilities are not  easily available on an electrical tester. Therefore, for DVM  implementation, a time measurement unit is used to accurately  measure delay propagations with a resolution in the range of  picoseconds. In order to relate the LSM position with the  measured propagation time simultaneously, the X and Y  positions of the laser beam are acquired by the acquisition  unit.


Figure 11: Delay variation mapping setup: both laser position (x, y) and timing delay (t) are acquired to create picosecond  scale sensitive maps.


DVM methodology


A test sequence is applied at the input device in loop mode. Two synchronization signals are added at this test sequence. The first is used to command the laser modulation (ON/OFF) for choosing the illuminated vectors inside the test sequence. The second is a trigger pulse sent by the tester to the time  measurement unit. The time measurement unit measures the  time between the trigger and the switching of the output of  interest. For each time delay measurement, the laser beam  position (X and Y) is stored. The time delay between the  observed output signal and the trigger signal comprises the  delay measurement. At the end of the scan, a time delay image  in false color is extracted. Positive and negative timing  variations are superimposed on the laser reflected images. Figure 12 is a sample of a delay variation mapping obtained  on a logic counter under PLS.


111


Figure 12: Delay Variation Mapping sample obtained on  binary counter under PLS. The white value shows the PLS  sensitive area that induced a delay and the black shows the  PLS sensitive area that induced an advance.


Another way is to monitor the frequency instead of the delay  variations. To do this we have developed a specific setup to  measure the output frequency variation correlated with laser  stimulation (PLS or TLS). The output frequency of interest is  measured by counting switching numbers of one output in a  fixed temporal window. This measurement is correlated at  each laser beam position and data are presented in the shape of  a three dimensional matrix, laser position (X, Y) and output  frequency (Z). Such a setup can be advantageously used on  test structures and on defective ICs involving a frequency  output failure. In such cases, the advantage of frequency  variation mapping is the automatic and fast averaging of delay  variations induced by laser stimulation.


DVM benefits


The main advantage of DVM versus previous DLS techniques  is to open up measurement resolution, to show the full shade  of laser induced delay without being limited to either only  black (PASS) or white (FAIL). As presented in the next  paragraph, even where the PASS/FAIL approach works, DVM  may yield finer results.


From the tester point of view, electrical parameters must be  adjusted for dynamic laser stimulation in order to be as  sensitive as possible to laser stimulation. In addition, functional testing requires output strobe placement to detect  small timing variations within the PASS/FAIL status. With  DVM, the output strobe is automatically set to monitor all  variations.


The price to pay is an additional piece of electronics (time  measurement unit or frequency measurement unit) and a few  more synchronization signals: laser scanning pixel, line and  frame clocks must be sent to the timing board as well as the  tester trigger signal and the monitored device output (see  figure 11).


DVM – Case studies


In the following paragraphs, case studies obtained on 0.18µm  technology test structures are presented to illustrate the  implementation of DVM.


In the first case study the time delay between input pulse and  output pulse of a single inverter chain is measured. The left  image of figure 15 shows the delay variation mapping results  obtained under PLS. Four inverter chains are included in the  scanned area; they have the same input but separate outputs. In  the DVM image in figure 15, the observed output is labeled  number 1.


Figure 13: DVM images of inverter chain (0.18µm) under PLS  with a solid immersion lens and corresponding layout.


Dark pixels show the advance of the output signal induced by  Photoelectric Laser Stimulation while the opposite effect is  shown by the bright pixels. The above Delay Variation  Mapping result shows the sensitivity and the accuracy of this  approach. Both n and p transistors of the inverter chain were  localized and responded differently to the laser stimulation.


In the second case study the frequency variation is monitored  on a ring oscillator test structure upon PLS. In figure 14 the  gray color represents the normal frequency, i.e., areas not  sensitive to laser stimulation. Sensitive areas are highlighted  and we can observe different sensitivity levels as a function of  color. The black colors show the most sensitive area where the  ring oscillator activities and frequency slows down.


Figure 14: Frequency variation mapping under PLS. Gray  represents areas not sensitive to laser stimulation, i.e., frequency is not affected. Dark color shows areas where PLS  induces a decrease in frequency while the white color areas  are where PLS induces an increase in output frequency.


112


The sensitivity of DLS can be improved by increasing the  laser power and performing a fine adjustment of each variable. However, increasing the laser power can result in device  damage, which is especially true with smaller technologies. For example, upon TLS, thermal coefficient of variation  mismatch can result in metal discontinuities, whereas PLS can  induce destructive latchup. Also, refining all variables can be  quite time consuming.


The DVM methodology, when applicable, offers a higher  sensitivity while reducing the setup time. This increase in  sensitivity is highlighted in figure 14 for which the three  following group are distinguished:


Group 0 No variation, areas not sensitive to laser  illumination. Areas with normal propagation delay. Group 1 Very fine time variation (positive or negative). Areas that may not be sensitive enough for pass/fail  detection.


Group 2 Significant variations (positive or negative). Sensitive areas may be detected with pass/fail.


Figure 15: Representation of timing variation induced by  laser stimulation (originally in PASS state without laser  stimulation).


At a given laser power, DVM detects and localizes all  sensitive areas whereas DLS with functional test detects only  the group 2 sensitive areas, thus increasing the sensitivity of  DLS techniques.


More importantly, the understanding of the TLS and PLS  effects on dynamically activated ICs still needs to studied. For  instance, in the case studies presented above, the effects of  nearby test structures are also observed on the observed  output. The different CMOS structures are only linked by their  power supply (VDD, gnd) nodes. This is highlighted on the  DVM images of figure 16. On the left image, a nearby inverter  chain clearly appears which was unexpected. It means that the  Photoelectric Laser Stimulation of these structures affects the  time delay propagation of the observed chain. One hypothesis  is the presence of substrate currents generated in the active  region. It can affect the dynamic behavior of observed  structures by propagation through the substrate or by the  power supply lines. A similar effect is observed with the  frequency variation mapping. On the right image of figure 16, PLS highlights two ring oscillators, top and bottom, whereas  the observed output is just from the top one. It induces a  substrate current which perturbs the global device  functionality and not just the illuminated gates.


Figure 16: Delay (left) and frequency (right) variation  mapping under PLS. Under PLS some CMOS structures not  electrically linked with the observed output have an effect on  the observed output where they are stimulated by the laser.


To avoid perturbation from nearby gates under illumination  we can either reduce the laser power or use a pulsed or  modulated laser. In fact, recent modeling work shows the  advantage of pulsed laser compared to continuous wave: the  substrate photocurrent is limited and the laser perturbations  are more localized, resulting in an increase of dynamic laser  stimulation image accuracy [18].


More generally, a modulated and pulsed laser is useful for an  asynchronous setup and offers the possibility of illuminating  not only a limited area of interest (to avoid side effects) but  also a limited time frame of the test sequence (during one  vector of interest for example).


In this paper we have presented the principles of Dynamic  Laser Stimulation techniques as a function of laser stimulation  type (TLS or PLS) for failure analysis and design debug.  Implementation of these techniques requires a laser scanning  microscope (LSM), an electrical tester to stimulate the device (with a test sequence sent in a loop) and a detection scheme. For LADA (1064 nm laser), SDL and RIL (1340 nm laser) the  tester itself may be used to detect the laser effect on signal  propagations. Functional testing is used to compare measured  data with expected vectors. By linking the PASS/FAIL status  to the laser scanning positions, sensitive areas can be detected.  The last techniques presented, delay variation mapping and  frequency variation mapping, were shown to extend the  application field of existing dynamic laser stimulation  techniques based on functional testing to characterize  dynamically failed ICs. By adding an additional time  measurement unit, the whole range of timing variation is  measured. We have demonstrated the application, the  sensitivity and the accuracy of these techniques to localize  laser stimulated sensitive areas.


[1] T. Wilson and E.M. Mac Cabe, Journal of Applied  Physics, Volume 61, Issue 1, 1987, pp191-195


[2] E.I. Cole Jr, J.M. Soden, International Reliability Physics  Symposium 1994, pp388-398


113


[3] K. Nikawa and S. Tozaki, International Symposium for  Testing and Failure Analysis 1993, pp303-310


[4] E.I. Jr. Cole, P. Tangyunyong and D.LD Barton  International Reliability Physics Symposium 1998, pp129-136


[5] R.A. Falk, International Symposium for Testing and  Failure Analysis 2001, pp59-65


[6] J.A. Rowlette et al International Test Conference 2003, pp264-273


[7] M.R. Bruce, V.J. Bruce et al International Symposium  for Testing and Failure Analysis 2002, pp21-27


[8] Edward I. Cole Jr. et al, International Symposium for  Testing and Failure Analysis 2001, pp43-50


[9] Edward I. Cole Jr. et al International Symposium on the  Physical and Failure Analysis of Integrated Circuits  2002, pp15-21


[10] A. Firiti et al, Microelectronics Reliability 2004, Volume  44, Issues 9-11, pp1675-1680


[11] C. Boit et al, International Reliability Physics  Symposium 2004, pp357-360


[12] T. Wilson and E.M. McCabe, Journal of Applied  Physics, 61 (1), 1987, pp191-195


[13] D.J. Burns et al, International Reliability Physics  Symposium 1984, pp76-82


[14] H.K. Brown et al, System Theory, 1990, Twenty-Second  Southeastern Symposium, pp384-388


[15] K. Sanchez et al, International Reliability Physics  Symposium 2005, pp305-311


[16] D.J. Ager, G.F. Cornwell and I.W. Stanley  Microelectronics Reliability, vol 22, No 2, pp241-264


[17] K. Sanchez et al, International Symposium on the  Physical and Failure Analysis of Integrated Circuits (IPFA) 2005, pp21-26


[18] A. Douin et al “Electrical Modeling for Laser Testing  with Different Pulse Durations” 11th IEEE International  On-Line Testing Symposium, 2005


114


Soft Defect Localization Techniques without a


Synchronization Signal to the Laser Scanning Module


Diana Mitro, Dawn Glaeser, and Clifford Howard


Freescale Semiconductor, Inc., Austin, Texas U.S.A.


Soft Defect Localization (SDL) is an analysis technique  where changes in the pass/fail condition of a test are  monitored while a laser is scanned across a die.[1,2,3,4]


The technique has proven its usefulness for quickly  locating failing nodes for functional fails that are


temperature, frequency, and/or voltage dependant. The  localized heating from the laser can toggle the pass/fail


condition as it sweeps over failing nodes with the  aforementioned sensitivity.  The technique is instrumental


in identifying latent defect locations on conditional fails


even though they seldom produce light emissions or  liquid crystal hot spots. These fails often manifest  themselves after reliability stress or at the customer. The


technique can also be applied to support design groups  with first silicon analysis of timing race conditions and


identification of signals that are speed path limiters. The


main challenges associated with the technique are in  synchronizing the tester with the Laser Scanning Module


(LSM) and ensuring the laser can heat the device enough  to overcome the pass/fail threshold temperature of the


failing node.


Information about the Soft Defect Localization (SDL)


technique was first published and presented at ISTFA in  2002 by M.R. Bruce et al.[1] The paper introduced the  concept of scanning a laser across a die such that the  localized heat can change the pass/fail state of the failing


node to identify its physical XY location on the die.  The


technique was a natural development from the Resistive  Interconnect Localization (RIL) technique published by  E.I. Cole Jr. et al. in 2001.[2] Since the publication, many  failure analysis labs have been working on adapting their


existing Laser Scanning Modules (LSM) to perform SDL


analysis on conditional fails. The largest hurdle in  accomplishing this lies in the details of how to setup ones


test platform to run synchronously with the LSM.  Many


manufacturers have begun providing tester  synchronization features on their LSM’s as a result of the


industry’s desire to use the SDL technique.  However  many analysis labs may have older LSM’s which do not  have tester synchronization capability.  This paper will


discuss the techniques used to perform SDL analysis on  the Hamamatsu Phemos-1000 without pixel


synchronization using 2 different tester platforms: a


Hilevel mini-tester and an evaluation board.  The  importance of understanding the threshold temperature of  the fail-to-pass or pass-to-fail will also be investigated.


Basic Synchronization Principle


The laser’s role in SDL analysis is to scan across a die


and locally heat each pixel location.  When the laser i


located over the failing location, the heat from the laser


should change the test result from either a failing state to


a passing state or vice versa. Therefore at each pixel


location the LSM receives a digital pass or fail signal


from the tester. If a pass is assigned a digital value of 1


and a fail is assigned the digital value 0 the LSM should  color the pixel white if it passes and black if it fails (or


vice versa if the pass and fail digital assignments are


reversed). The key to synchronizing the tester to the LSM


is to time the length of the test to match the laser dwell


time on 1 pixel so that a valid pass or fail result is


determined at least once for each pixel.


Selection of the length of time used for SDL analysis


depends on balancing 3 factors: pixel dwell time, the  thermal equilibrium of the defect, and the test pattern  duration. The pixel dwell time is dependant on the


scanning speeds provided by the LSM. For example 16s is  the maximum scan speed provided by the basic  Hamamatsu Phemos 1000, however an upgraded Phemos  1000 can have scan speeds over than 1000s. The thermal  equilibrium depends on the length of time the defect  needs to be heated above the threshold temperature to  change the test state from a pass to a fail or vice ersa.


However, the length of time needed to achieve the  thermal equilibrium is also related to the laser spot size


(magnification) and device technology. On average, 50µs  is a reasonable value for thermal equilibrium. Finally, the


test pattern duration depends on the test hardware and the  number of vectors needed to exercise the fail and  determine the pass/fail result. In most cases the pixel


dwell time and test pattern duration are the parameters  that are dialed in to achieve synchronization, as theyar


usually easier to manipulate than the thermal equilibrium.


When setting up the test to match the pixel dwell time, th


test should be designed to balance the length of time  allotted to allowing the laser to heat the pixel area and to


sending the resulting pass or fail signal to the LSM.


115


# Soft Defect Localization Techniques without a Synchronization Signal to the Laser Scanning Module


During the heating portion, the test can be set to loop  several times to allow enough time for the laser to heat  the local area above the threshold temperature. After the


heating portion is complete, the next stage of the test  should output the pass or fail result for the remaining  potion of the pixel dwell time.  The pass or fail pulse


duration must meet the minimum duration requirements  of the pulse detector.


SDL with an Evaluation Board


The SDL technique was attempted using an evaluation  board platform on a microcontroller failing at high


frequency only. Neither light emission, nor liquid crystal


hot spots, nor OBIRCH signals had been detected on the  fail prior to attempting the SDL analysis. First the code


was timed to determine whether it fell within the 2µs to


2048µs pixel dwell time range given by the LSM on the  Hamamatsu Phemos-1000 used for the analysis. It was  found that one loop of the test code took 68ms to run  which was an order of magnitude too slow. The problem  was that the macro for the evaluation board ran through a


serial communication cable between the computer  running the EVB software and the device under test (DUT). To overcome this problem the code needed to be  translated to a format that could be downloaded directly


to the RAM in the device. The code was converted to  assembly language format and downloaded to the RAM. When the code was executed from the RAM it was  measured to take 3.6µs to run. This put the test into the


allowable range for SDL analysis on the given LSM. Delay loops were then added to the code to match the  128µs pixel dwell time needed to achieve the threshold  temperature and allow enough time for the pass/fail  measurement. 50% of the pixel dwell time was allocated


to laser heating to achieve the targeted 64µs needed for


thermal equilibrium and 50% to output the pass/fail  indicator.


The test code was written such that 2 port pins were  activated on the evaluation board to output the pass/fail  indicator signal and a pulse to time the length of 1 run of


the code. The timing pulse was used to measure the  effects of changing the delay loop parameter to dial in the


length of the code to precisely match the pixel dwell time.


The pass/fail indicator signal was programmed to be 0


when the device failed and 1 (Vdd) when the device  passed.


The heating portion of the code would continually write  to the failing register for the first 64µs (50%) of the code.


The test would then check to see if the correct information  was read from the register.  If it passed the indicator  would remain high for the remaining 64µs of the code and  if it failed it would be set to ground. When the code  looped back to the start of the code for the next pixel, conditional logic was employed to keep the pass/fail  indicator at its previous state until the result of the next


register verification was different than the previous state.


SDL with a Hilevel Tester


The synchronization principles were also applied to  perform SDL analysis on a 0.25um CMOS  microcontroller that failed at room temperature, low  voltage, and all frequencies.  The device passed at either


elevated temperatures or higher voltages making the  device a good candidate for the SDL analysis technique. The biggest challenges for implementing the SDL  technique with the Hilevel mini-tester were synchronizing


the LSM with the test loop and providing the pass/fail  indicator signal to the LSM.


A scan speed of 36s per 512X512 pixel frame was  selected.  The pixel dwell time for this scan speed s t up


was 128µs which provided enough time to heat each pixel  above the threshold temperature of the fail and output a  pass/fail result for each pixel. The failing units passed at


higher temperatures and voltage, therefore the voltage  level for the analysis was carefully selected to be about


100mV below the passing voltage threshold.  The 100mV  cushion was experimentally determined to ensure the  device always failed at room temperature and always  passed after at least 40µs (approximately 30% of the  128µs pixel dwell time) of laser heating. Without the  100mV safeguard, the pass/fail behavior of the device  was too unreliable and would produce noise instead of a  meaningful SDL result.  The test program was initially  designed such that the first 35% of the pixel dwell time


was allotted to heating and the remaining 65% of the pixel  dwell time was used to output the pass/fail indicator.


The pass/fail indicator was created by using the original


failing test pattern and adding conditional code and delay  loops to closely match the pixel dwell time requirement.


The pattern output a high signal (5V) to the LSM if the part failed and a low signal (0V) if the part passed. It also


was design to execute one time for each pixel scanned by


the LSM.  Figure 1 displays a small portion of the Hilevel


pattern code used to synchronize the tester with the pixel


dwell time and to provide a pass/fail indicator output  signal for each execution of the test pattern.


VECTOR # Command


Output Description


CTRG


Clear fail flag


STF


Use fail flag for CJMP


RSET


……


…… Rest of pattern to exercise unit


2459


CJMP 02469    0


Jump to vector 2469 if pat fai


ls


2460


2461


LOAD 00100    0


Set up delay loop for pass ind


icator


2462


DEC


Decrement loop counter


2463


LOOP@


2464


NOP


2465


JMP 00000    0


Loop back to the start of patte


rn


2466


Dummy vector


2467


2468


2469


NOP            0     Start of delay loop for f


ail indicator


2470


LOAD 07500    1


Change Output to high to indic


ate fail


2471


2472


2473


2474


JMP 00000      0


Loop back to the start of pat


tern


Figure 1: Example Hi-Level program code for pixel  synchronization and pass/fail indication.


116


The dotted box in Figure 1 outlines the conditional jump  used to jump to a different section of the test pattern when


the part failed. The conditional jump checks the Hilevel  pass/fail flag at the end of the pattern (pass – dashed line


box in Figure 1, fail – solid line box in Figure 1.) and  jumps to one section of the pattern (vector 2468 in Figure


1) to change the signal output level to 5V when it failed or  continued through the pattern to keep the output level at  0V when it passed.


Initially, the run time of the pattern for a pass condition


was not equal to the run time of the pattern for a fail  condition resulting in distortion of the SDL signal.  Figure


2 shows the SDL image when the pass and fail timing  loops did not match.  Note for this case, black indicates a  low tester output signal (pass) and white indicates a high


tester output signal (fail). The distortion above and below


the dark spot in the left image of Figure 2 is a result of the


timing mismatch between the pass and fail branches of  the test.  However, once the timing loops for the passing  and failing branches of the program were matched, the  distortion was eliminated as shown in the right image of  Figure 2.


mismatched pass/fail pattern


matching pass/fail loops


Figure 2: 50X magnification SDL images are displayed  where the duration of the pass and fail branches of the  test pattern are equal (right) and mismatched (left).


Another experiment was conducted to further understand  the effects of having a mismatch between the lengths of


the pass and fail branches of the test pattern.  In this s udy


first the pass and fail branch indicators were set to equal


7% and 47% of the 128µs pixel dwell time respectively.  An acceptable SDL signal was still obtained regardless of


this large mismatch. (Figure 3 left) The analysis was then


repeated after switching the pass and fail branch  indicators to 47% and 7%.  In this case an SDL signal was  detected however it is not as clear because of the noisier


field. (Figure 3 right)  The results indicate that the


technique can tolerate large mismatches between the pass  and fail indicator branches.  However, the best (most  compact and least noisy) SDL signal was obtained when  the pass and fail branches were equal.


5X SDL image


Pass = 7%, Fail = 47%


Pass = 47%, Fail = 7%


Figure 3: 5X magnification SDL images are displayed  where the duration of the pass and fail branches of the  test pattern varied.


Timing Variation Effects


Several other timing factors in the design of the test


program were varied to study their effects on producing a


clear SDL signal. First, the test pattern execution time


was varied to determine how closely the test pattern ime


must match the pixel dwell time. The delay loops within


the test pattern were varied to make the total test pattern


time 30% (test pattern = 170µs) and 110% longer (test  pattern = 270µs) than the 128µs pixel dwell time.  In both


cases the pass/fail indicator pulse ratios were set to  remain in the range of 60% to 75% (~80µs) of the pixel  dwell time. Both conditions produced an accurate SDL  signal as shown in Figure 4 below. The results show that  it is possible to get an SDL signal even if the total test


pattern time is longer than the pixel dwell time.


5X SDL Image


Test pattern length = 30%


Pixel Dwell Time


Test pattern length = 110% Pixel Dwell Time


Figure 4: 5X magnification SDL images are displayed  where the total test pattern time was 30% (left) and 110% longer than the 128µs pixel dwell time.  Both cases  produced SDL signals.


Next the total test time was held constant at 128µs to  equal the pixel dwell time and the pass/fail indicator  signal lengths were varied (while keeping the pass and


fail branch lengths equal to each other). SDL images w re


obtained with the pass/fail indicator signals set to 7%


(10µs), 46% (60µs), and 75% (95µs) of the pixel dwell  time. (Figure 5) The results showed that no SDL signal  was detected when the indicator signal was too short (7%


117


or 10µs). SDL signals were obtained when the indicator  was set to 46%, and an even better SDL signal with less


field noise was seen at 75% of the pixel dwell time. The


information indicates that maximizing the pass/fail  indicator with respect to the total pixel dwell time


improves the clarity of the SDL signal.  However, as the


length of time devoted to the pass/fail indicator is  increased, the length of time to heat the area is  proportionally decreased.  Decreasing the heating time too  much may result in determining an inaccurate pass/fil


signal if the test does not allow enough time for the laser


to heat the area above the threshold temperature to toggle


the pass/fail when on the defective region.


Pass/Fail Indicator = 7%


Pass/Fail Indicator = 46%


Pass/Fail Indicator = 75%


Figure 5: 5X magnification SDL images are displayed  where the pass/fail indicator time was varied to 7%, 46%,


and 75% of the pixel dwell time.


Threshold Temperature


The threshold temperature of the fail is the other factor to


be considered when performing SDL analysis.  The  temperature sensitivity of the part can greatly impact the


setup parameters of the SDL analysis. First, it must be


determined whether the pass/fail state of the device can be  toggled by the laser.  After establishing that the device is


sensitive to the laser, it should then be confirmed that the


device consistently outputs one result with no laser and  consistently outputs the opposite result when stimulated  by the laser.  There have been cases where a part displays


the proper temperature, voltage, or frequency sensitivity  needed to perform SDL analysis, however the SDL results  were too noisy to pinpoint a defective spot because the  output behavior of the device was too inconsistent.


Therefore, it is important that the laser is solely


responsible for the change in pass/fail result.


It is also useful to quantify the threshold temperature of


the fail.  If the threshold temperature is low (<40ºC) less


time can be devoted to heating and more time can be  dedicated to the pass/fail indicator signal when designing


the SDL program to maximize the clarity of the SDL


images. Devices with higher threshold temperatures  present a greater challenge to SDL analysis, however  several factors can be adjusted to optimize the results,


including pixel dwell time selection, heating to pass/fail


indicator ratio, laser power, and ambient temperature of  the device under test (DUT).


Some LSM’s have a continuous range of scan speeds  available, and other LSM’s have a menu of several  discreet scan speeds that may be selected.  The  Hamamatsu Phemos-1000 instrument used for the  analysis in this paper provides 8 scan speeds: 1s, 2s, 4s, 8s, 36s, 72s, 286s, and 572s. The corresponding pixel  dwell times for a 512X512 pixel frame are 2µs, 4µs, 8µs


16µs, 128µs, 256µs, 1024µs, and 2048µs respectively. The length of time to run the test pattern is usually the


first consideration when selecting a pixel dwell time.


Often the test run time can be a limiting factor, especially


on an evaluation board platform where a test can take  over 10ms when running through serial communication.


Once a test pattern that runs within the time allotted by


the pixel dwell time is obtained, the pixel dwell time that


is slightly longer than the test is selected. It is usually


easier to add delay loops to the test to match it to the


longer pixel dwell time than to shorten the test to match a


faster pixel dwell time. The longer pixel dwell time also


allows for more heating time and for a longer pass/fail


indicator pulse which has shown to produce better SDL  images. However, if a fail has a high threshold


temperature, a pixel dwell time may need to be selectd


that is much longer than the test pattern to allow more


time to heat the sample before determining the pass/fail


status of the pixel.


A microcontroller device that was failing at 125ºC and


56MHz (but passed at the same frequency at room  temperature) was found to have a very high threshold  temperature. The fail could also be reproduced at room  temperature and high frequency (88MHz). The threshold  temperature of the fail was lower the higher the frequency


selected.  56MHz was too low a frequency for SDL


because the threshold of the fail was over 100ºC at this


frequency which was too high to reproduce in the  laboratory environment.  88MHz was too fast because the  device would always fail at room temperature at this  frequency.  Therefore 66MHz was selected for SDL  analysis because the device consistently passed at room


temperature and consistently failed above 65ºC.  This  temperature seemed feasible for the analysis. The test  pattern took 3.6µs to run so delay loops could be added to


118


match most of the pixel dwell times available.  Because


the threshold temperature was still relatively high at


66MHz, the 128µs run time was selected initially.  50% of the pixel dwell time was allotted to heating the device


and 50% to outputting the pass/fail indicator.


Unfortunately this did not provide enough time for the


laser to heat the device to the threshold temperature to  toggle the pass/fail result.  The ratio of heating time to


pass/fail indicator time was increased, however the  threshold temperature was still not achieved even after the


ratio reduced the pass/fail indicator time below the  minimum limit.


The next option was to increase the pixel dwell time from


128µs to 256µs to determine if more heating time could  locally heat the device to 65ºC. This would have required


a large rewrite of the test program to match the newpixel


dwell time.  Instead another option was attempted.  A hot  chuck was placed in the Hamamatsu stage and the entire  DUT was preheated to 60ºC.  (All the DUT equipment  was rated to sustain this temperature.) The hypothesis was


that if the device was preheated, the laser would only  need to locally increase the temperature of the device


~5ºC to trigger the fail. The theory proved to work and a


SDL signal was obtained with this technique. (Figure 6,


Table 1)


20X SDL Overlay Image 200X SDL Overlay Image


50X SDL Overlay Image


50X SDL Image


Figure 6: SDL images were obtained from a device with a


high threshold temperature fail by preheating the DUT  with a hot chuck.


Table 1: Summary of SDL attempts on a 65ºC threshold  temperature fail.


Trial 1


Trial 2


Trial 3


Fail   Condition


65ºC & 66MHz


Pass   Condition


25ºC & 66MHz


Heating /  Pass & Fail  Indicator


(% Pixel  Dwell Time)


50% Heating


50%


Indicator


70% Heating


Heating


Mechanism Laser


Laser


DUT


preheated  to 60ºC + Laser


SDL Signal  Obtained?


NO


YES


Another device with temperature sensitivity was analyzed


with the SDL technique and presented a different kind of


threshold temperature hurdle. Instead of having a  threshold temperature that was very large, this device had


a threshold just above room temperature.  An SDL signal  was easily obtained for this device, however the spot was


so large that it did not pinpoint the failing location  precisely.  In this case an experiment was performed to


study the effects of changing the laser power to change


the size of the resulting SDL signal.  SDL images were


obtained with the laser power set to 85%, 50%, and 25%. (Figure 7) The results showed that reducing the laser  power for a low threshold temperature fail can help  pinpoint the failing location.


119


50X, 85% power


50X, 50% power


50X, 25% power


Figure 7: The effects of varying the laser power on fails


with low threshold temperatures are displayed. All  parameters were constant except laser power.  The  respective overlaid images are located to the left of their respective SDL images.


Following the basic synchronization principles discussed  has proven its usefulness for performing SDL analysis on


an LSM without any SDL synchronization features.  The  study shows that the minimum requirements for  performing successful SDL analysis is an LSM where a


pass/fail indicator signal can be substituted as input to  control the pixel coloration of the LSM data. Once this  minimum requirement is met, the test programs can be  carefully crafted to match the pixel dwell time of the  selected LSM scan speed to provide virtual  synchronization.  The study showed successful results  were obtained on 2 different test platforms: a Hileve  mini-tester and an evaluation board. The pixel dwell time,


test run time, and thermal equilibrium of the fail must all


be balanced when setting up synchronization for the SDL


technique. In most cases the pixel dwell time and the test  run time are the flexible parameters that can be adjusted


to achieve the desired synchronization. The effects of  varying the various timing parameters was observed and  compared to the quality of the resulting SDL images. It


was discovered that the SDL technique has a large  synchronization timing window.


SDL images can be obtained with some mismatch  between the test program length and the pixel dwell time,


however the SDL images appear to be clearer when the  timing matches exactly. The pass/fail indicator signal  must also meet the minimum pulse width for the LSM to


latch the result.  If the indicator signal is too short it will


not be recorded by the LSM.  If the indicator signal takes


too large a percentage of the total test time, the heating


time may be reduced to below the minimum time needed  for the laser to heat the sample to the threshold  temperature of the fail. Finally devices with high and low


failing threshold temperatures were studied.  Using a hot


chuck to preheat the DUT was found to be a successful  technique for performing SDL analysis on a high  temperature fail, and reducing the laser power was found  to help pinpoint the SDL signal to the failing location on a  low temperature fail.


We would like to thank Evan Chang and Bob Roche of  Hamamatsu for their support.


[1] M.R. Bruce et al, Soft Defect Localization (SDL), International Symposium for Testing and Failure  Analysis, pg. 21-27, (2002).


[2] E.I. Cole Jr. et al, Resistive Interconnect  Localization, International Symposium for Testing  and Failure Analysis, pg. 43-50, (2001).


[3] F. Beaudoin et al, Laser Stimulation Applied to  Dynamic IC Diagnostics, International Symposium  for Testing and Failure Analysis, pg. 371-377, (2003).


[4] G.L. Woods et al, Rapid Diagnostics of an ASIC IP  Block Using Dynamic Laser Scanning, International  Symposium on the Physical & Failure Analysis of  Integrated Ci4rcuits, pg. 27-31, (2005)


Ideal Silicon Thickness Determination


For backside investigation, reflected IR laser imaging could  be done through a polished silicon substrate with substantial  thickness but signal levels will be strongly reduced because of  the silicon absorption in the infra-red. Consequently, defect in  circuitry could be not observed during a failure analysis in live  mode for example. In this case, the only way to improve the  detection and observation is to use high frame integration  mode (long time). In order to prevent this problem and to  increase success rate of failure analysis, it appears more  practical to thin and polish the sample to an “ideal” silicon  thickness. From figures 5 and 6, it can be seen that 200µm of  silicon thickness with good polished surface can provide  identical TLS signal levels to that of a frontside prepared  sample. The effect of silicon thickness has been also  quantified through an introduced relative factor of  detectability on silicided resistors (see figure 7).


50 100 150 200 250 300 350 400 450 500 550 600


0,5 1,0 1,5 2,0 2,5 3,0


Reference (frontside)


Silicon thickness (µm)


P+ poly Silicided (4/360) N+ poly Silicided (4/360) P+ diff Silicided (4/360)


Figure 7: Detectability factor versus silicon thickness when  maximal laser power is used on silicided resistors.


When 100µm of silicon thickness is selected, backside  analysis improves detectability of TLS level by 1.2 to 2.6  factor range respectively for silicided diffused resistor and  polycrystalline resistor in comparison with sample analysed  by frontside.  This confirms that 100µm value appears as an  ideal silicon thickness which provides best electrical TLS  signal detectability and rigidity for physical characterisation.


W/L Dimensions Effect On TLS Signal


Section and W/L dimensions define the electrical resistance  value of resistors. Geometrical reduction (W/L) means that the  studied resistor can be entirely observed in the field of view. Consequently, an IR laser beam will irradiate and heat not  only a bulk resistor but also its interconnections. Resistivity  variations optically induced on a bulk resistor will be  translated by high OBIRCh signal. Simultaneously, the SEI  signal appears on interconnections and will be strongest and  dominates the OBIRCh signal. This phenomenon will be more  important for unsilicided resistors because of the higher  relative thermo-electrical power of the junction materials  between tungsten and the semiconductor structure. If identical  resistors contain silicide layer, its electrical resistance value  will be drastically modified and the Seebeck signal will be  attenuated because of reduced thermo-electrical power  between plugs in tungsten and silicide.


W/L=40/80


W/L=4/80


W/L=0.18/70


Figure 8: Impact of W/L reduction on TLS imaging


Silicid Layer Effects On TLS Signal


Experimental results displayed in figure 2 and 3 show that  TLS mapping difference is essentially due to the silicide layer. The IR laser beam is highly absorbed by the CoSi2 layer and  strong heat absorption will take place in this layer, whereas


124


the bulk resistor is more transparent to the 1,3µm laser  wavelength. Thermal inertia will induce heat diffusion  between the silicide layer and bulk of semiconductor resistors. Physical property of CoSi2 reduces electrical resistance of  covered bulk structure. Finally, it can be concluded that CoSi2  layer of 30 nm of thickness changes electrical characteristics  and thermal behaviour of studied resistors. Those behave like  metallic element when heated by the laser beam. Consequently, it can change TCR value of resistors and  modify radically TLS signatures. This last observation is very  important for improving our pseudo 3D localization  methodology which is presented through some case studies.


TCR Parameter Effect On TLS Signal


Thermal sensitivity of conductive elements (metallic/semiconductor) can be deduced by calculating the  TCR parameter value [8] from their linear R=f(T) curve. Experimental results demonstrate that positive TCR values are  obtained for silicided resistors (poly/Rdiff) whereas negative  and weakest positive TCR values are obtained only for n+/p+ unsilicided polysilicon resistor with smallest width (0.18µm). Silicided layer seems to be responsible of ten factor increasing  of TCR parameter on both resistors. These results demonstrate  that temperature sensitivity of semiconductor structure is  linked to W/L dimensions, resistor type, doping type and  above all to silicide layer (CoSi2).


Depth Fault Localization Methodology


From these results and guidelines, we have developed and  optimized a methodology for short circuit defect in IC, based  on TCR parameter extraction coupled with TLS localization


[8]. In other word, correlation between TCR value and TLS  colour can give indication about depth fault localization (z) and predict material involved in failure. Strong positive TCR  and black TLS colour means that defect is localised in BEOL, whereas a strong negative TCR value and white TLS colour  correspond to FEOL localization.


# Case Study: 1


The failed IC analysed is a 0.25µm technology products with  six metal layers. The short circuit was validated and the  extracted TCR value extracted was equal to + 0.001967 °C-1. Using the frontside Thermal Laser Stimulation (TLS) method  on PHEMOS 1000 system, the defect area was precisely  localized on this device.


Figure 9: Frontside defect localization using Thermal Laser  Stimulation (TLS) with a 50x objective.


Figure 9 shows grey colour localization on the OBIRCh image (on the left) and green colour on superimposed image (on the  right). By comparing TCR value to our TCR database and  observing grey TLS spot with white background colour, a  semiconductor short circuit is highly suspected to be  responsible for the failure. For this case, a fast delayering of  all metallic levels until polysilicon level has been done. The  defect was found to be a short in the active layer as depicted  on SEM and layout images on figure 10.


Figure 10: SEM image of the active short defect (right) and its  associated layout image (left).


# Case Study: 2


The failed device is a 0.25µm technology product showing a  short circuit between Vdd and Gnd. Thermal characterization  has permit to extract a TCR value of -0.00079 °C-1 indicating  that failure is probably due to semiconductor material and  localised in FEOL level. Defect was localised with accuracy  by using frontside TLS mapping as depicted in figure 11.


Figure 11: Frontside defect localization using Thermal Laser  Stimulation (TLS) with a 50x objective.


Figure 12: SEM image of the active short (right) and its


associated layout image (left).


Physical analysis consisted of removing quickly all metallic  level followed by a good SEM observation. Figure 12


125


highlights a problem in FEOL level, where failure mechanism  is a short active due probably to a parasitical micro-masking.


# Case Study: 3


The failed integrated circuit analysed was fabricated in


0.25µm technology with six metal layers. Failure mode was  validated as short circuit like previously and TCR value  extracted was equal to + 0.001973 °C-1. TCR value is very  close to the first case study and seems also to target failure in  FEOL level.


Figure 13: Frontside defect localization using Thermal Laser  Stimulation (TLS) with a 20x objective.


Figure 13 shows TLS localization with a grey TLS signal with  white TLS background colour. Like previously, semiconductors material is expected to be involved in failure  of this product.


Figure 14: SEM image of the active and polycrystalline short  circuit and its associated layout image.


A quick physical analysis reveals an active and polycrystalline  silicon short circuit as shown in figure 14. This failure was  probably induced by a parasitical micro-masking.


# Case Study: 4


This case study was introduced to demonstrate the feasibility  of the proposed methodology for accurately localizing short  defects in the BEOL level of an integrated circuit. The failed  integrated circuit is a HCMOS product in 0.18µm technology. The device presents a high leakage current between the analog  supplier Vdd and the analog ground GND. TCR parameter  value for this device was found to be positive and equal to


0.0015 °C-1. This means that the defect is probably localized  in the BEOL. From internal TCR table, tungsten (W) could be  the suspected material in the IC failure. The defect area was  detected and localized as a black TLS signature close to the  power supply rail by using thermal laser stimulation


techniques (see figure 15). Spatial extension of the OBIRCH  signature (right image) gives an indication about defect size  inducing a short circuit between numerous metal lines in the  BEOL.


Figure 15: Frontside defect localization using Thermal Laser  Stimulation (TLS) with a 50x objective.


A step by step physical analysis is performed in the backend  of the line levels and shows that the failure was located at  metal 1 induced by a metallic defect (see figure 16). This  result confirms also the hypothesis about defect size (5µm  length) formulated from the OBIRCH signature.


Figure 16: SEM image of the thermal laser stimulation  located aluminum (Al) defectivity (M1).


In this case, the short circuit was induced by the resistive  defect. However, it was found that the physical defect is in  aluminum instead of tungsten as expected from the extracted  TCR value. Due to the large nature of this aluminum defect, the observed TLS signal most likely originates from the  tungsten plugs which electrically connect the defective lines. In any case the defect location (BEOL) and material (Tungsten) was already identified from the exact TCR value, thus confirming the applicability of the proposed  methodology.


# Case Study: 5


The failed integrated circuit analysed is in 0.18µm technology. Failure mode was electrically validated as short circuit and  defect was localized under a black spot by using IR Thermal  Laser Stimulation technique. White background TLS  signature is observed around defect. In this case no TCR  parameter measurement was performed.


126


Figure 17: Frontside defect localization using Thermal Laser  Stimulation (TLS) with a 20x objective.


Figure 17 shows TLS localization with a black TLS spot and  white background TLS which means that defect is associated  to a semiconductors material.


Figure 18: SEM image of the active and polycrystalline short  circuit and its associated layout image.


After a quick physical delayering until polysilicon, failure  mode was short active silicon as shown on SEM image of  figure 18. Our hypothesis and interpretations are validated. This methodology has been successfully applied in our failure  analysis laboratory for enhancing defectivity yield in  manufacturing and improves significantly failure analysis.


Silicided/unsilicided polycrystalline silicon and diffused  silicon resistors from 0.18µm technology with n+ and p+ doping type have been studied. Thermal laser stimulation  techniques were applied and signatures were observed and  interpreted. Thermal characterizations provide positive TCR  values for both resistors type with W/L size over than 4/80  while negative values have been measured for small W/L  dimensions. First’s observations demonstrate that CoSi2  silicide layer increases highly TCR value of studied resistors. This work considerably improved our understanding and  interpretations of IR laser stimulation signatures provided by  PHEMOS1000 system. At the same time, these experimental  results also improved the 3D localization methodology  dedicated to short defect failure. It makes possible to  distinguish failures of the FEOL from those of the BEOL  level. Provided interpretations and experimental results  contribute to improve significantly failure analysis flow in  laboratories.


[1] K. Nikawa and S. Inoue, “New Capabilities of OBIRCH  Method for Fault Localization and Defect Detection”, Proc. Of Sixth Asian Test [1].


[2] F. Beaudoin, G. Haller, P. Perdu, R.Desplats, T. Beauchêne and D. Lewis, “Reliability defect monitoring  with thermal laser stimulation: biased versus unbiased”, Microelectronic reliability, vol.42, 2002.


[3] A. Firiti, F. Beaudoin, G. Haller, P. Perdu, D. Lewis and  P. Fouillat, “Implementing Thermal Laser and  Photoelectric Laser Stimulation in a Failure analysis  Laboratory”, Microelectronic Reliability, IPFA 2003.


[4] S. Kumar and L. Bouknight, “Modeling of Polycrystalline  Silicon Thermal Coefficient of Resistance”, IEEE int. Integrated Reliability Workshop Final Report, pp. 150-151, 1999.


[5] H-M. Chuang, K-B. Thei, Sheng-Fu and W-C. Liu, “Temperature-Dependant Characteristics of Polysilicon  and diffused Resistors”, IEEE transactions on electron  device, Vol.50, NO.5, pp. 1413-1415, 2003.


[6] C-C. Liu, K-B. Thei, H-M. Chung, K-W. Lin, C-C. Cheng, Y-S. Ho, C-W. Su, S-C. Wong, C-H. Lin and H. Carlos Diaz, “Characterization of Polysilicon Resistors in  Sub-0.25µm CMOS ULSI Applications”, IEEE Electron  Device Letters, vol. 22, NO.7, pp. 318-320, July 2001.


[7] A. Firiti, F. Beaudoin, G. Haller, P. Perdu, D. Lewis and  P. Fouillat, “Understanding the effects of NIR Laser  Stimulation on NMOS transistor”, Microelectronic  Reliability, ESREF 2004.


[8] A. Firiti, F. Beaudoin, G. Haller, P. Perdu, D. Lewis and  P. Fouillat, “Short defect characterization based on TCR  parameter extraction”, Microelectronic Reliability, ESREF 2003.


127


Lock-In Assisted Soft Defect Localization (LIA-SDL) and its Application  In Scan Shift Problems


Zhongling Qian, Christof Brillert, Christian Burmer, Markus Grützner


Infineon Technologies AG, Failure Analysis, Munich, Germany  zhongling.quian@infineon.com


120


Guideline for interpreting IR Laser Stimulation signal on semiconductors  materials and for improving failure analysis flow


A. Firiti, G. Haller


ST Microelectronics 13106, Rousset, France


firiti.ixl@st.com  / Gerald.haller@st.com


+33 (0) 4 42 68 68 52 / +33 (0) 4 42 68 55 78


F. Beaudoin, P. Perdu


CNES-THALES laboratory – Bpi 1414


18, avenue Edouard Belin, 31401 Toulouse, France


Felix.Beaudoin@cnes.fr  / Philippe.Perdu@cnes.fr


+33 (0) 5 61 27 34 41 / +33 (0) 5 61 28 20 17


D. Lewis, P. Fouillat


Laboratoire IXL, 351, Cours de la Libération, 33405 Talence, France  lewis@ixl.fr  / fouillat@ixl.fr


+ 33 (0) 5 40 00 27 64 / + 33 (0) 5 40 00 26 30


Infra-red Thermal Laser Stimulation (TLS) signatures  obtained on semiconductor materials can be difficult to  interpret and to distinguish from signatures from metallic  materials. Investigations presented here consist in the study of  TLS signals on unsilicided/silicided polycrystalline and  diffused silicon resistors of 0.18µm technology. The influence  of each process parameter on the TLS signal has been  observed and evaluated from the front and back side of the  circuit. This allowed us to quantify the effect of the silicon  substrate thickness on TLS signal detection and to determine  the ideal silicon thickness for sample preparation. This study  also completes our methodology based on the TCR parameter  which aims at improving defect localization in the depth (Z) of circuitry. As it will be shown through failure analysis case  studies, this methodology increases the physical analysis  success rate and reduces the turnaround time.


The semiconductor industry uses metals, insulators, alloys, crystalline and amorphous silicon for processing integrated  circuits. Polycrystalline silicon and diffused silicon structures  compose the majority of the front-end of the line level  process. They are the most active part of an integrated circuit  and are used for various applications. Polycrystalline silicon  can be used in circuitry as gate transistor, gate capacitor and  also as resistors, whereas diffused silicon material is used as  pn junctions, transistor source/drain connections, resistors and  active parts of capacitors. Their conductivity and performance  is monitored by using n+/p+ doping type and silicide layers as


CoSi2. IC reliability depends on their stability under electrical  and thermal stresses because of their high temperature  sensitivity compared to metallic materials. Thermal Laser  Stimulation (TLS) techniques, which include OBIRCh, TIVA  and SEI mapping techniques, have been extensively studied  and applied to detect defects such as shorts within IC’s  metallic materials [1], [2], [3]. But, for failure analysis it can  be difficult to differentiate TLS signature induced by frontend of the line material (FEOL) from those related to backend  of the line materials (BEOL) [8]. Here, we propose some  experimental results focused on semiconductor resistors in  order to interpret their impact on IR laser stimulation  signatures obtained using the PHEMOS1000 system. This  guideline significantly improves our failure analysis flow for  short defects and is based on material TCR parameters to gain  insight into the localization depth.


Devices Under Test


The studied structures are doped n+/p+ polycrystalline silicon  and diffused silicon bars processed in 0.18µm CMOS  technology at STMicroelectronics in Rousset, France. Devices  under test present various W/L ratio with or without silicide  layer (CoSi2) for reducing their electrical resistance and access  resistance. Interconnections are realized with tungsten (W) and aluminum (Al) is used for metallic lines. Generally, polysilicon resistors present higher resistance than diffused  resistors mainly because of the grain boundary regions [4, 5]. This physical property is responsible of the material electrical  conduction efficiency and thermal behaviour. The resistors we  studied are listed in table 1 which describes type of  semiconductor resistor, doping type, W/L ratio, resistance  value at ambient temperature and TCR values. It is interesting  to note that some TCR values of FEOL materials are negative.


121


# Guideline for interpreting IR Laser Stimulation signal on semiconductors materials and for improving failure analysis flow


By way of comparison, the TCR value of aluminium is  positive and equal to 0.0035 °C-1.


Table 1: Devices descriptions


Device


W/L


R0 (Ω)  TCR (°C-1)


P+sal: 4/360


769.14


0.003029295


P+unsal: 4/80


2280


0.000275439


P+unsal: 0.18/70 65089


-0.000136859


N+sal:4/360


660.75


0.002391525


N+unsal:4/80


2268


0.00029806


Polysilicon  R


N+unsal: 0.18/70 63350


-0.0000620


734.76


0.003068507


2301


0.001599305


P+unsal: 0.25/80 38223


0.001416739


686.46


0.003247729


1740


0.001572414


Diffused


N+unsal: 0.25/80 30310


0.001484659


Samples were prepared from frontside and backside for  performing IR thermal laser stimulation analysis. Frontside  preparation required parallel polishing until metal 1 to prevent  metallic screening problem (dummy and metal layers) and  getting easy access to resistors bars.


Experimental Set-Up


The experimental set-up is performed with PHEMOS 1000  equipment. The system uses a continuous wave infrared laser  with a wavelength of 1.3µm and an optical power of 100mW  which allows performing both front and backside TLS  observations. For the 50X objective, a maximum output laser  power of 20.7mW can be delivered to the device. The analysis  presented here was done at a maximum resolution of  1024x1024 pixels and a maximum laser power range of 100%. IR OBIRCh was selected with a constant voltage of 1 volt for  performing thermal laser stimulation analysis from frontside  and backside of samples. Reflected imaging and current  mapping signals were acquired with the highest scanning time  of 16s and 50x magnification. The TLS signal, which  corresponds to current variations induced by a change in the  material resistivity upon laser heating is detected and  amplified with an OBIRCh amplifier. It is expressed by next  relation:


∆i = - TCR*∆T*(Vsup/R0) = - (∆R/R0²)*Vsup


(1)


TCR and ∆T are respectively the Temperature Coefficient of  Resistance and temperature variations. Combination of theses  parameters corresponds to resistivity variations ∆R/R0, where  R0 is the resistance of the IC at ambient temperature. Vsup is  the constant voltage applied to the device.


The sign and colour of the coded TLS signal depends on the  TCR value of heated material and consequently on ∆R/R0². A  white TLS signature is associated to a negative TCR value and  a black TLS signature is associated with a strong positive or  weak positive TCR value. On the final superimposed image, a  white signal is associated with red colour whereas and a black  signal is associated with green colour as depicted in figure 1. A precise location of material in which a current flows is  obtained by superposing TLS images on laser-reflected


images (see figures 2 and 3). It can be important to notice that  the PHEMOS1000 software adjusts automatically the TLS  signal and makes an auto scale of the TLS measurement in  order to provide the best signal to noise ratio and current path  localization.


TCR<0


TCR>0∆i measurements


4095


2048


∆N: Coded TLS signal


Mean noise level


Superimposed colours


+∆imax


-∆imax


WHITE


BLACK


Figure 1: Diagram of TLS signal imaging construction on  PHEMOS 1000 system


Experimental Results


TLS Observations


The following results give an overview of TLS and  superimposed images obtained on resistors from both front  and backside through 100µm of silicon thickness. Figures 2  and 3 show TLS results obtained on both n+/p+ polycrystalline silicon and diffused resistors with W/L ratios  of 4/360 for silicided case and 4/80 for unsilicided case. The  TLS signatures highlight the current path within those  devices.


P+ polysilicon resistor N+ Polysilicon resistor


P+


Silicided  W/L=4/360


Unsilicided  W/L=4/80


N+


Figure 2: Frontside and backside TLS observations on p+/n+ polycrystalline silicon resistors


122


First observations indicate that backside TLS signatures seem  to be better than frontside. The explanation of this higher TLS  signal obtained from the backside is unclear and needs to be  further investigated. As it will be shown later, the TLS signal  amplitude is strongly dependent on the silicon thickness. The  following observations and interpretations are done on  backside TLS signatures.


P+ Diffused resistor


N+ Diffused resistor


Figure 3: Frontside and backside TLS observations on p+/n+ diffused silicon resistors


Black TLS signatures can be observed on both n+/p+ poly and  diffused resistors with silicide layer and high dimensions, whereas weak white signatures are observed particularly on  unsilicided polycrystalline resistors with small dimensions. In  other hand, a pronounced grey TLS signal can be observed  especially on diffused resistors with small geometry. These  first observations underline the impact of process parameters  on the TLS signal and highlight particularly the major  influence of the silicide layer and W/L ratio on the TLS  signal. The weak TLS intensity on all unsilicided poly and  diffused resistors is due to their high resistance and also to the  weak IR light absorption in bulk of studied materials. Longer  resistors of W/L=4/360 are not entirely observed in field of  view with 50x magnification. It is interesting to notice that  SEI signatures were observed on interconnections regions  from all studied resistors.


Black TLS signatures observed on silicided material can also  be observed on metallic lines during analysis. For failure  analysis it could be difficult to distinguish the black TLS  signature induced from semiconductors materials to the ones  from metallic materials. This issue can be solved by  electrically measuring the TCR parameter of shorted ICs and  correlated to the known TCR values. Before discussing the  impact of each parameter on TLS signal and colour, we


propose to evaluate more precisely silicon thickness effect in  backside analysis.


Silicon Substrate Thickness Effect On TLS Signal


Backside analysis can be considered as the best way to get  access to device’s active areas thus avoiding metal screening  issues. We have evaluated the influence of silicon thickness  by a qualitative TLS observation through various silicon  thicknesses of 375µm, 203µm, 110µm and 63 µm when the  maximum laser power is applied. Figure 4 demonstrates that  TLS signal level increases when the silicon thickness  decreases.


Silicided P+ polysilcon resistor


375µm


203µm


100µm


63µm


Silicided P+ diffused resistor


Figure 4: Qualitative TLS signal observation on silicided p+ polysilicon and diffused resistors (W/L=4/360) for various  silicon thicknesses


Laser power attenuation and TLS signal amplitude reduction  by silicon substrate thickness were studied and quantified  numerically on prepared samples. The methodology consists  of extracting the TLS signal and noise amplitudes from  regions of interest by using the Count function of the  PHEMOS1000 software and varying laser power range from  minimum to maximum by step of 10%. This function allows  analyzing the intensity data of the acquired image such as  maximum, minimum, average and distribution values of the  TLS signal. Experimental results obtained on all  polycrystalline and diffused resistors are displayed in figures 5  and 6.


0 10 20 30 40 50 60 70 80 90 100


0 500 1000 1500 2000 2500 3000 3500 4000


E


F


H


J


K


20.7 mW


Unsilicided devices - W/L=4/80


Silicided devices - W/L=4/360


Laser power (%)


1A


Figure 5: TLS signal measurement on polysilicon resistors  versus laser power for various silicon thicknesses.


123


Silicided and unsilicided devices


1Aa


Figure 6: TLS signal measurement on diffused resistors


versus laser power for various silicon thicknesses.


It can be important to notice that TLS level at 0% of laser  power corresponds to the noise level and can be considered  the zero level. A linear decrease of TLS signal amplitude is  obtained for all silicided and unsilicided diffused resistors and  only for silicided polycrystalline resistor when laser power  increases. It is important to underline that the TLS level  detected is the highest when the silicon thickness is reduced. These linear characteristics confirm the OBIRCh relation, the  weak dark colour observed and the weak positive TCR of  analysed material. For the unsilicided polycrystalline resistor  with small W/L geometry, characteristics are completely  different and no significant TLS variations are measured. This  behaviour and the observed white colour can be due to high  resistance of the bulk material, to the small negative TCR  value, and also to the absence of CoSi2 layer. From these  observations, an ideal silicon thickness can be determined for  sample preparation and signal detection enhancement.


A new localization method called LIA-SDL is introduced and  applied to scan shift problems. The method combines local  thermal stimulation technique with lock-in technique applied  to periodical test pattern. The localization capability on soft  defects is shown in comparison with SDL. Same localization  results are obtained. LIA-SDL technique requires no special  LSM (Laser Scan Microscope) facilities and is quite easy to  handle. Limits and prospects of this new methodology are  shown at several analysis examples.


With the increasing number of metal layers and shrinking  feature size of VLSI circuits, the traditional tools of defect  localization in failure analysis (FA), such as liquid crystal  thermography (LCT) or emission microscopy, have met a great  challenge [1-2]. On the other hand, modern ICs are designed  with the idea of design for testability (DFT) by using full scan  design. Correspondingly, the scan chain, scan logic tests or  BIST (Built-in Self Test) are replacing the traditional  functional tests and achieve at the same time a better test  coverage and reduced time for pattern development. These test  patterns are generated from ATPG (Automatic Test Pattern  Generation) tools. Furthermore, these scan patterns allow  improved diagnostics – sufficient to isolate a problem to a  short list of candidates for faulty nets, in best case, one single  net. The defects in the logic sea can be physically localized by  using TLS (thermal laser stimulation) technique in a static  circuit, combined with the results from scan diagnosis [3]. In  some cases, soft defects with a signature of a voltage, temperature, or frequency dependent behaviour in scan chain  test, are a challenge for this localization method. Formerly, laser voltage probing (LVP) is used to solve this problem [2], which needs a careful preparation of the devices and some  time to search the failed flip-flop (FF) in the scan chain and  the affected FET in the FF. Another localization method is soft  defect localization (SDL) [4-5], which will be discussed below  in detail. In this paper, a new localization method, named  Lock-In Assisted Soft Defect Localization (LIA-SDL) is  introduced to solve these problems.


Analysis at Scan Chains


As we know, the thermal laser stimulation (TLS) technique is  used for soft defect localization (SDL) [4-7]. Soft defects, which can be caused by resistive via’s, leaky gate oxides or  process marginality, are extremely difficult to localize [4-7]. In  SDL technique, heating due to the absorption of  NIR laser  energy or carrier injection will cause soft defects to change  their electrical behaviour during dynamic testing, thus  changing the pass/fail status of the test. In the case of a failed  scan chain due to a soft defect, the electrical failure signature  needs approximately a time N/2*T (N: the length of scan  chain; T: scan clock period) to reach the scan output (SO) pin. If during this process the laser beam has already moved to  another position, the localization result will be misleading. In  this case the scanning time per pixel must be long enough to  correlate the tester pass/fail information with the laser beam  position.


LIA-SDL Method


The idea presented here is based on the usage of the periodical  SI (scan input) signal of the scan chain tests as a reference  signal in the lock-in technique. As we know, the lock-in  technique is integrated in the commercial TLS instruments to  improve the detectable minimum current and S/N (signal to  noise ratio), in which the intensity of NIR laser beam is  modulated. In our technique, on the contrary, no modulation of  laser is needed. The narrow-band and stroboscopic-like  detection in the lock-in technique can greatly reduce both the  external noise and the effects from other frequency domains, such as scan clock and PLL’s. Therefore this method is very  powerful for defect localization in a dynamic circuit.


There are two kinds of detection modes, depending on the  detection objective:


128


# Lock-In Assisted Soft Defect Localization (LIA-SDL) and its Application In Scan Shift Problems


Voltage mode


The first mode is named voltage mode, in which the SO (scan  output) signal is used as the input signal, while SI is set as  reference signal to a lock-in amplifier, shown in Fig. 1. The  timing problem in SO can be reflected in the amplitude, phase  or X/Y component outputs of the lock-In amplifier. This setup  is similar to a SDL setup, and a long scanning time per frame  must be taken.


Figure 1: General experimental setup of lock-in amplifier in  voltage detection mode at scan-chain circuit. Two scan chains  with scan flip-flops (red boxes, FF) are shown. Between the  two chains are normal logic circuits (CLK: scan clock, SI: Scan chain input signal, SO: Scan chain output signal of the  two chains).


Current mode


The second mode is called current mode (Fig. 2), which is  much more powerful than the voltage mode. In this mode, a  current sensor is placed in the power supply line. Periodical  variations occur in the current drawing due to internal  switching transients, which are amplified and sent to the lockin amplifier. A periodical signal at scan-chain input (SI) activates the soft defect. In CMOS logic, the transition edges  lead to a main current consumption. Therefore, this method is  more sensitive to problems occurring during the raising or  falling edges. There are two main advantages of this detection  mode. At first, it does not need a scan output signal (SO), which makes it possible to detect all failed chains at the same  time with the same SI. Secondly, it is a much faster method to  localize the soft defects, since there is no time delay between  the defect induced current variation and the corresponding  detection.


In both modes, the reasonable choice of the reference  frequency will greatly increase S/N and therefore the detection  sensitivity.


Figure 2: Experimental setup of lock-in amplifier in AC   current detection mode. In contrast to the voltage mode (fig. 1) a current amplifier (I2U) is placed in the power supply  circuit.


Equipment


To provide the required laser beams a confocal laser scanning  microscope (LSM) is used. Slow-scan capability of about 2 ms  per pixel is needed. For thermal laser stimulation a cw high  power laser with 1.3um vacuum wavelength is used. A second  high power laser with a wavelength of 1064 nm can be used  for carrier injection. The microscope optic is equipped with  high NA 50x lens with silicon thickness correction. Measured  laser powers between 30-160 mW after 50x lens were used. The lock-in amplifier has a maximum detection frequency of 2  MHz. A preamplifier with variable band pass filter is used for  LIA-SDL detection in current mode. For voltage mode no  special amplifier is needed.


Case 1: Scan shift problem


A typical case for a scan-shift problem is shown in Fig. 3 - 5, corresponding to the two detection modes. This is a product  with 0.13µm technology and 7 metal layers. One or more scan  chains on one chip showed a voltage dependent scan shift  problem. The corresponding yield loss was 2%. The typical  failure signature is shown in timing diagrams at three different  supply voltages (Fig. 3). Typically, the scan chain consists of  4000 scan flip-flops (FF). With supply voltage larger than 1.4  V, the effected chain does work with scan clock (SC) at 1  MHz. With lower supply voltage, an apparent time shift of  edges or latch problem can be observed, shown in Fig. 3. The  SI pattern is chosen as “11001100”. Therefore SI signal has a  frequency of 250 kHz and serves also as the reference signal of  the lock-in amplifier. The localization results from LIA-SDL  are shown in Fig. 4 - 5. In both modes, a point-like spot was  located on one FET at the failed FF in the corresponding scan  chain.


129


Figure 3: The SO timing diagrams of a failed scan chain  showed voltage dependence with supply voltage at 1.5 V, 1.4  V and 1.15 V. The SI pattern is “11001100”, while SO is “1000100” at 1.4 V, and “10011001” at 1.15 V.


Figure 4: The results in LIA-SDL in the voltage mode showed  that a better localization in gate level can be obtained by  using a longer frame time of 286 s (right image). A shift of the  TLS spot from LIA-SDL is observed with frame time of 36 s (left image). The dotted red line is for better visibility of the  shift of TLS spot.


In the voltage mode, the shift of TLS spot strongly depends on  the location of the failed flip-flop (FF) and the length of scan  chain (Fig. 4). 286 s per frame are needed to achieve accurate  defect localization  in order to compensate sufficiently the  delay of the LIA-SDL signal.


In the current mode, only the AC current with the same  frequency 250 kHz as SI was detected by using lock-in  amplifier. In comparison with the current mode, only 8 s  scanning time per frame is needed to obtain accurate  localization. In comparison with the normal TLS detection in  the static mode, this localization method shows additionally a  higher sensitivity due to the reduced external noise and effects  from the signal of scan clock, shown in Fig. 5.


Figure 5: The normal TLS detection showed no TLS spot (a), while the LIA-SDL in the current mode showed a TLS spot in  the AC current detection mode (b). Image overlay of pattern  image with LIA-SDL image is shown in (c). The overlaid spot  is colored.


Case 2: Comparison SDL – LIA-SDL


The following case utilizes the same type of device from 130  nm technology. Analysis background was yield loss. From  previous failure analysis work it’s probable that the failure  signature corresponds to a leaky transfer gate inside one scan  flip-flop [2]. Therefore this device type is a good vehicle to  show the methodology of LIA-SDL in comparison with the  well known SDL technique.


Figure 6: Shmoo plot of failing scan chain. The transition  from working point at pass region to fail region (pass/fail) is  shown by an arrow.


The failing device shows voltage dependent failure at  one scan chain, shown at the shmoo plot in Fig. 6. The device  shows a duty cycle violation. Only at high supply voltages the


130


device becomes pass. The pass/fail limit is with standard  timing parameter slightly below 1.46 V main supply voltage. The minimum voltage value of the supply specification is not  achieved.


First, a SDL localization technique was applied to  this voltage dependent failure signature of the scan chain. For  SDL the fail/pass signal from the tester is generally used to  detect the failure as the laser passes over the sight. However, in this case specialized electronics is utilized, to directly detect  duty cycle violations like an additional or missing pulse in  scan chain patterns. Fig. 7 (c) shows a generated SDL signal  after a typical duty cycle violation. The duty cycle violation is  caused by laser beam stimulation at a SDL failing area of the  device. The voltage input of the LSM is used for mapping the  SDL signal with respect to laser beam position. The scan chain  is driven with an ‘1010101’ pattern, which is repeated in a  loop after initialisation of the scan test. The scan clock  frequency is 1 MHz.


Figure 7: Timing diagram of scan chain input signal (a) chain  output signal with duty cycle violation marked with a circle


(b) SDL signal, which is generated after this duty cycle (c)


In Fig. 8 the result of the SDL analysis from chip  backside with working point at the pass region is shown. Only  one area shows a very small spot like SDL signal. The frame  time was 300 seconds to avoid shifts in SDL spot due to  already described chain delay problem. With a change of scan  direction about 90 degree the spot location can be double  checked. The SDL image is always simultaneously stored with  the pattern image in order to confirm, that no instabilities of  LSM shifts the spot location in respect to the pattern image. The spot lies on a part of a scan flip-flip in the failing chain. Due to the fine spot size, the SDL signal can be related to pmos transistors of the scan flip-flop.


SDL spot


Figure 8: SDL image from chip backside at working point in  pass region. Lens magnification 50x plus 4x scanner  magnification is used. The marked green SDL spot is related  to the failing scan-chain.


n-mos


p-mos


Figure 9: LIA-SDL images in voltage mode: Working point in  fail region at 1.44 V supply voltage (a). Working point in  pass region at 1.46 V supply voltage (b). N-mos is related to  a probably failing transfer gate inside a scan flip-flop of the  fail chain.


For comparison with SDL, localization with LIA-SDL in the  voltage mode was performed. For lock-in reference the scanchain input pattern was utilized. The measured lock-in  frequency was with ‘101010’ pattern 500 kHz. The


131


localization results are shown in Fig. 9. Comparison with SDL  technique shows that the location of the spots at pass working  points exactly agree to high accuracy. On the other hand with  working point in fail region the sign of the LIA-SDL lock-in  amplitude inverts at the sensitive area. That is visualised by  selecting a red colour scale for the inverted signal. Surprisingly, the spots at the different working points do not  match with each other. They have reproducible different  locations in the same scan flip-flop. Precise layout overlay  shows, that the small red spot is related to the n-mos of one  transfer gate inside the same scan flip-flop. A defect which  causes locally a small leakage in such a scan flip-flop can be  responsible for the observed duty cycle violation. At this type  of failing devices a typical physical root cause is a dislocation  at one of the n-mos transfer gate transistors. P-mos transistors  are normally not affected. Therefore the fail/pass mode is  suitable for the localization of this type of duty cycle violation.  .


Case 3: Racing problem


The device of the following case has a voltage dependent  failure of a mixed chain after life test. This mixed chain is used  to test the RESET inputs of scan flip-flops. The technology is  the same as in case 1. For supply voltages below 1.0 V the  propagated test signal appears at the chain output pin two  clock cycles too early. The output of a pass mixed chain at 1.5  V and of a failing chain at 0.9 V is shown in Fig. 10.


Figure 10: The output signal (lower waveform) of mixed chain  each in PASS and in FAIL mode is shown. The failing two  clock cycles at the scan chain output are marked with an  ellipsoid.


For precise backside localization the failing devices were  thinned, polished and special packaged for backside access.


The adequate technique for localization is SDL. In  order to detect the fail/pass status a simple self built  comparator electronic was used to detect the earlier two clock  cycles by comparison with a tester generated reference signal. In case of detecting a pass to fail transition the output of the  electronic is set to high level. The comparator electronic needs  furthermore a tester trigger. The output signal of the electronic  is imaged with the LSM.


The used pattern is quite short and consists only of  about 70 clock cycles with a frequency of 1 MHz. The pattern  runs in a loop at a tester.


Figure 11.: Comparison SDL image at 1.1 V (a) with LIA-SDL  image in current mode  at 1.1 V (b)


The result of localization with SDL is shown in Fig. 11 (a). The SDL signal is red colored and overlaid with the pattern  image. SDL was performed at a supply voltage of 1.1 V. The  signal shows sensitive areas were due to thermal laser  stimulation a transition to fail status was generated. The  colored areas are related to different parts of the scan chain. That will be discussed later in detail.


Additionally, the new LIA-SDL technique in current  mode was applied to the same device. The result is shown in  Fig. 11 (b). The imaged output signal of the lock-in amplifier  is overlaid with the pattern image. The voltage values are  mapped with yellow/orange colour scale. Two big spot like  areas can be identified, which generate increased lock-in  signal.


A comparison between the SDL and lock-in image  shows, that the spots at both images are located at nearly the  same area. The spots at the lock-in images are in a kind of  saturation due to the four times higher laser power, which was  applied for imaging. At lower laser power the spots become  smaller like the SDL image and give comparable results. With  low laser power substructures of a scan flip-flop can be  identified, e.g. the left spot is split into two different sides. The  bigger one is related to a p-mos, whereas the smaller one to a  n-mos transistor.


In contrast to the LIA-SDL current mode the voltage  mode need direct access to the output signal. The lock-in  amplifier works as phase selective rectifier, which is therefore  very sensitive to phase jumps or the disturbance of the signal  periodicity. For this purpose an ideal high sensitive instrument  for detection of the two too early coming clock cycles. A phase  jump can be generated by a transition from pass to fail or vice  versa. Both transitions can be generated by thermal laser beam  irradiation at the faulty mixed chain.


At Fig. 12 the results of LIA-SDL in voltage mode at  the same device and location as the images in Fig. 11 are  shown. The supply voltage at fig. 12 (a) is set slightly above  the voltage limit of 1.0 V in pass region. Whereas in Fig. 12


(b) the supply voltage is slightly below the limit in fail mode. The coloured region represent the areas were due to laser  irradiation a significant lock-in signal is generated. Obviously, with LIA-SDL voltage and current mode – compare fig. 11 - nearly the same spot like structures can be observed.


Accurate comparison of both images in Fig. 12 show  spot like signals at different locations. The generated lock-in  signals are related to the failing mixed chain. The different  relevant parts of the mixed chain are marked with white boxes.


132


In Fig. 13 a schematic of the localized area is shown. The  schematic shows the functional relation between scan flip-flop  FF3 and FF10. The clock inputs (clk) of both flip-flops are  separated by clock buffer. The output Q from flip-flop FF3  controls via an inverter the reset (RST) of flip-flop FF10.


Obviously, due to laser irradiation at inverter (INV) and flip-flop (FF3) the reset problem of flip-flop FF10 can be  fixed and we observe a pass chain at green signal (Fig. 12 (b)). Otherwise due to thermal irradiation on the clock buffer and  flip-flop FF10 the pass chain is transferred in a fail mode (orange/yellow signal at Fig. 12 (a)). The imaging examples  show a typical timing problem called racing:


Race path 1: FF3 - INV


Race path 2: CLK BUFFER – FF10


The localization with LIA-SDL shows both races immediately.  Assumed a small delay in the clock buffer path is responsible  for the voltage dependent fail gives an understanding of the  shown racing problem. Thus in pass working point the thermal  stimulation by the laser increases the delay in the clock path  with the result of a failing device at race path 2. On the other  hand, with working point at the fail mode the laser increases  the delay in data path. Consequently, the assumed clock delay  is compensated by increased delay in datapath. Therefore the  device becomes pass at race path 2. According to the  assumption, the failure must be in clock buffer path (race path  2). Further localization in this case with LIA-SDL/SDL is not  possible. The limit of this technique is demonstrated, because, e.g., a small resistance change in nearly every part of the race  path 2 can be responsible for the timing failure. For finer  localization inside the race path laser voltage probing (LVP) might be useful, but was in this particular case not further  required. Due to the support of localization with LIASDL/SDL the failure hypothesis of a racing problem was  confirmed and isolated to race path 2. The problem was  understood and the further analysis was stopped.


The new method LIA-SDL is obviously an excellent method  for SDL localization at chain based problems. The comparison  shows nearly identical localization results between LIA-SDL  and classical SDL at the shown cases. In contrast to SDL the  advantage of LIA-SDL technique in current mode is, that no  output channel is required. A periodical input signal is  sufficient. Furthermore this new technique can also be utilized  for scan logic failures and for normal functional tests with  periodicity in the patterns. Without question, localization of  hard fails, which can be addressed periodically can gain from  the very good noise rejection and sensitivity of lock-in  technique.


Figure 12: LIA-SDL results in voltage mode: (a) working  point at pass region (pass/fail transition) (b) working point in  fail region (fail/pass transition). The related parts of the  failing mixed chain are marked with white frames.


Figure 13: Schematic of the localized part of the failing mixed  chain circuit


[1] C. Burmer et al., “Software Aided Failure Analysis Using  ATPG Tool”, IPFA  210-215 (2002)


133


[2] C. Burmer et al., “Fault Localization of a Scan Shift  Problem on Integrated Logic Designs”, ISTFA, pp. 384-390 (2003)


[3] Z.-L. Qian et al., “Precise defect localization of scan logic  failures by thermal laser stimulation (TLS)”, ISTFA, 517-520 (2004)


[4] E.I. Cole Jr. et al., “Resistive Interconnect Localization”, ISTFA,43-50 (2001)


[5] M.R. Bruce et al., “Soft Defect Localization (SDL)”, ISTFA, 21-27 (2002)


[6] F. Beaudoin  et al., “Laser Stimulation Applied to  Dynamic IC Diagnostics”, ISTFA, 371-377 (2003)


[7] E. I. Cole Jr., Desk Reference of  Microelectronics Failure  Analysis, 5th Edition,  415-416 (2005)


134


Furthering the Business Proposition of a Robust System Level Failure Analysis  Framework:   A Focus on Enabling Product Services


Roger Bjork


Dell Inc., Round Rock, TX, USA


A few years ago, along with colleagues from Intel and Dell, we shared with you the importance of Failure Analysis as a  business proposition[1], This paper will identify even more  business processes which will benefit from a robust System  Level Failure Analysis framework.


More and more companies strive to differentiate themselves  from their competition by focusing not just on product  features and price, but also on how well they serve their  customers. An effective Service Plan (Figure 1) is  fundamental in the provision of this service. No matter how  broad a company’s service offering portfolio, a fundamental  enabler of any Fault Management system is the ability to  identify and predict failures. Further, a robust Knowledge  Management system must exist to enable the collection and  dissemination of services intellectual property (IP) in an  effective manner, and facilitate a broad level commonality  analysis that provides the ability to monitor trends and shifts  in product performance.


Figure 1:  Service Plan


This paper will describe not only the benefits of such an  integrated Fault Management system, but also how the effect  of an integrated Failure Analysis Framework is a critical  component of such a system as part of a growing Services  business. Timely failure analysis data plays a critical role in


continuing to improve the customer experience related to  Fault Management.


There are three main customer-facing tenets of any superior  Services Plan (Figure 2). The first of these tenets is a group of  proactive measures called Prevention. Preventing product  problems from occurring requires focus and processes in the  following areas:


1. Reliability


2. Maintenance/Early Warning


3. System Performance & Tuning


The second tenet deals with the inevitable problems which  occur in a responsive and effective manner, thus reducing  and/or eliminating the potential negative customer experience. This Fault Management tenet contains the following elements:


1. Fault Isolation


2. Fault Resolution


The third and last tenet of a Services Plan supports managing  change. Included within the Change Management framework  are the following elements:


1. Deployment (installation and configuration)


2. Enhancements (upgrades and ongoing configuration  changes)


3. Retirement (end of life activities)


Figure 2:  Service Plan


135


A timely and actionable Failure Analysis Framework becomes  a critical component in enabling this Service Plan, with a  focus on driving improvements in reliability, establishing  monitors for early warning, and being an effective change  agent regarding new learnings (Figure 3).


Figure 3:  Failure Analysis Framework


This reinforces the shift from the traditional failure analysis  philosophy presented by Lane et al [1] to now providing a more  predictive role and helping to define the responsive nature of  the service plan.


The role of the Failure Analysis organization must shift to  support this strategy in several key areas (Figure 4):


1. Driving change to improve reliability:


a. Manufacturing changes (screening, etc.)


b. Running changes


c. Future design changes


2. Establishing new and better Early Warning Systems: a. Identifying additional protective measures


b. Continuous improvement


3. Improving Fault Isolation methodologies:


a. Troubleshooting steps


b. Diagnostics tools


Figure 4:  FA Focus Change


The remainder of this paper will provide details and examples  of where this change is happening and its effect on the  following areas:


1. Knowledge Management – the information interfaces  and flow required to transfer the IP obtained from  Failure Analysis to the various elements of the  Services Plan


2. Additional data sources for Failure Analysis


The fundamental role of a Failure Analysis framework is still  the development of actionable information, however the  demands of an improved Service Plan is requiring failure  analysis teams to take on a different perspective from their  traditional role.


Traditional Failure Analysis Applications


Improving Product Reliability


Failure analysis results have long been used to improve  product reliability.  It is quite common in industry today to  take the actionable results from the failure analysis process  and improve products currently under development and even  for next generation products. Timely data from the Failure  Analysis Process can also be used to improve products  currently in production. Continuous improvement can result in  running engineering changes, and even more urgently, in  improved production validation improvements (e.g., production screening functions).


Fundamentally, however, this is still a reactive response to  stimuli leaving little or no response option to the current  installed base of products. Further benefit can be derived by  shifting further left towards prevention. Utilizing modeling  tools is one method to help the organization learn now (vs. learn later). This technique, which has been predominant in  the aircraft and automotive industries, is now becoming a  necessity in the electronic and PC business (Figure 5).


Figure 5:  FA Modeling


136


Responsive vs. Reactive Failure Analysis


Failure Analysis organizations have also traditionally been  thought of as reactive organizations. The input to the failure  analysis process is often product which is already shipping (or  nearing its ship date) and the work is quite often very urgent.  Logistics and work flow processes are often optimized to  induce timely and actionable results from the failure analysis  process. Failure analysis organizations are well-trained to  react to stimuli. In today’s business climate, more is needed, however. Not only must the failure analysis team be quick to  react, they must be responsive. This means that the Failure  Analysis organizations must be cognizant of the timeliness of  their information and establish processes and systems that  function on a cadence in sync with their business. Beyond  reactive, these teams are agile – or prepared to react. A  responsive organization is also receptive to new ideas and  focuses on continued learning. This learning must come from  research as well as continuing education and must be an  ongoing source of input to the Knowledge Management  System. This will allow all learnings to be shared and  available, provide early commonality analysis through data  mining and focused research, and becomes a primary source  of investigative activity.


The Big Win - Installed Based Improvements


But what about products that are already installed and in use  by customers?  Is there opportunity for timely and actionable  failure analysis results to be applied to products that have  already been deployed? The answer is absolutely “yes!”   Output from the failure analysis process can and should be fed  into a robust Product Services process in order to glean even  more value from the failure analysis process and further  improve the customer experience. In many cases, it is possible  to respond in such a way that the customer is not even aware  that their equipment has a failure condition, hence the  customer experience remains positive.


Analogous to running changes in production, running changes  can be made to troubleshooting steps, maintenance  procedures, and diagnostic tools. Figure 6 illustrates the  advantage of the ability to impact the installed based.   In this  example, a power cable supplier had a process excursion  resulting in poor insulation.   The impact to the system was a  short between DC_IN+ and PS_ID, causing a no-power  condition on the motherboard. The field action was to simply  replace the motherboard. Had this policy continued, motherboards attached to cables of this vintage would  continue to fail, resulting in a very poor customer experience.   However, by ensuring that the diagnostic troubleshooting  steps were modified based on this finding, customers with  failed motherboards and cables of this vintage received both a  motherboard and a cable – thus preventing a recurrence of this  failure.


Figure 6 illustrates that the faulty cable was introduced in  month 5. Both a running change (introduced in month 10) and  the permanent change in future designs (introduced in month  15) ensure that future customers will not have this problem.


However, that leaves customers over a 5-month period that  could repeatedly experience this problem. The ability to  impact units already in the field is very powerful.


Poor Insulation - Power Cable


NonImpacted Defect


Introduced


Running


Change Next Gen


Production Month


Figure 6: FA Impact to Installed Base Population


An even more powerful opportunity is to use software to mask  hardware problems. It is common to make changes in BIOS  code and/or device drivers to mask problems found late in the  development cycle. Some hardware problems root caused by  the Failure Analysis team can also be resolved by software  changes. Technology in use today can not only notify  customers about such updates, but can proactively push  appropriate software updates to customers.


In addition to the reactionary steps noted above, there are  potentially proactive measures possible as well.   Actionable  failure analysis results can sometimes be translated into  improved system performance and tuning measures to  improve reliability. Also possible is the ability to impact  preventative maintenance steps to either improve reliability or  reduce the impact to the customer of an inevitable failure.


Impacting the installed base of products enables a much larger  payback of the failure analysis investment – not only in the  volume of products impacted, but also in the timeliness of the  impact. If an actionable result can be applied to the installed  base via the Services Program, the payback can not only be  multiples of that which affects only future products, but can  also begin to be realized much sooner.


Knowledge Management


The Key to Tying it All Together


Knowledge Management Systems are those processes which  harvest knowledge from various sources and then, in turn, provide this knowledge in the right form, to the right place, at  the right time. As mentioned earlier, actionable failure  analysis results typically feed into processes supporting  products under development and currently in production.


137


The following graphic illustrates not only this typical process  flow, but also the recently discussed flow for installed based  support.


Figure 7:  Integrated Workflow


As you can see, there must be systems to collect the failure  analysis results, and provide these to downstream processes.    Actionable Failure Analysis results are typically provided to  sustaining engineering teams via Trouble Tickets. A robust  Trouble Ticket process will encompass the full Root  Cause/Closed Loop Corrective Action/Preventative Action  scope. This ensure that not only are the symptoms and source  of the specific defect found and eliminated, but also the  process is improved in order to prevent future similar defects  from reaching customers. This formal “Lessons Learned” process is necessary to continue to improve product quality  generation over generation.


Referring again to Figure 7, one can see that including Service & Support organizations in the Trouble Ticket process enables  those organizations to modify Fault Management Services to  accommodate new discoveries from Failure Analysis.


Inputs to the Failure Analysis Process


Traditional Inputs


The most common source of material for the failure analysis  process is from the repair processes.   In fact, it is not  uncommon for suppliers to equate the repair process with the  failure analysis process – this is a big mistake.   The repair  process typically will only identify Level 2 failure analysis.


Note that the 3 levels of failure analysis are defined as  follows:


• Level 1 – is there a failure or not?


• Level 2 – identifying the specific failure mode.


Typically this is the component or subsystem which  has failed.


• Level 3 – identifying the true root cause of the Level  2 failure mode


Obtaining timely and actionable Level 3 failure analysis  results requires engineering and scientific resources and  processes.


Additional Inputs to the Failure Analysis Process


There are additional sources of material for the failure analysis  process, however.   Many of these sources already exist within  companies, but remain untapped today. One such source is  product which has been returned for potential safety concerns. It is a fact that some percentage of product will fail with a puff  of smoke. While the vast majority of these systems fail safely (the legal definition), it is a common practice for these  products to be shipped back to the supplier for confirmation  that there is no underlying safety issue that escaped detection  during either the development or production processes. These  systems which failed safely are a potentially rich source of  material for the failure analysis process. While the rate of  failure may be small, it is a significant source of negative  customer experience to have a product fail in such a manner. Failure analysis resources could be applied to determine if  there are even further improvements that can be made to  prevent such failures.


Other sources of failed material include products used inhouse by employees and executive escalations from major  customers. While the numbers of these excursions may be  limited, they nonetheless have the potential for a major  positive impact if and when actionable results can be  formulated. One of the key advantages of these alternate  sources is the fact that it is oftentimes faster to get the sample  into the failure analysis process than from traditional sources, thus supporting the timeliness of discovery.


Figure 8 illustrates these processes. The capture process is  critical to the timely nature of the failure analysis process.  The process to capture units directly from customers and  expedite them to the Failure Analysis team must have the  support of the Tech Support organization, have the ability to  identify specific units based on symptom criteria, and support  a specialized logistics system outside the standard break/fix  Return Material Authorization (RMA) process. The RMA  capture process, on the other hand, must be able to identify  units (again based on symptoms) entering the repair process - before any repair is attempted - and re-route them to the  Failure Analysis team. Likewise, captures from the Safety  Analysis team must be based on symptom criteria and further, have not suffered any destructive testing. Capturing units from  internal customers is likely to be similar to that of the RMA  capture process, and in many instances, is exactly the same  process.


138


Figure 8:  Failure Analysis Process Input Sources


It is clear that timely and actionable Failure Analysis results  can be used to not only improve the reliability of products, but  also to enable additional product services which improve the  overall customer experience. The viable failure analysis  organization has further advanced to become responsive – ready to react and actively engaged in continuous learning.


Systems to manage the flow of information from Failure  Analysis teams to various groups within an organization can  be simple or complex – but the goal is the same:   timely and  actionable information must be made available to a wide  variety of functions within a product organization to best  leverage continuous improvement.   These improvements can  impact not only products not yet deployed, but depending  upon circumstances, can also impact products already  installed.


In addition to providing actionable data to downstream  processes, Failure Analysis teams should consider multiple  sources of inputs. Most of these input sources already exist  and it is a matter of establishing the appropriate process flows. Timely and actionable results from a robust Failure Analysis  department continues to be a valuable source of product  improvement


The author would like to thank Mike Lane from Intel for his  continued support and clarity of purpose regarding the  concepts presented in this paper.


[1] Lane, M. et al, “System Level Failure Analysis Process:  Making Failure Analysis a Value Add Proposition in  Today’s High Speed Low Cost PC Environment,”


EDFAS Microelectronics Failure Analysis Desk  Reference, Fifth Edition (2004), pp. 15-21.


139


Unique Failure Modes from use of Sn-Pb and Lead-Free (mixed metallurgies) in PCB Assembly:  CASE STUDY


Frank Toth, and Gary F. Shade; Intel Corporation, Hillsboro, OR, USA {francis.toth.jr@intel.com, (503)-696-1546}


{gary.shade@intel.com, (503)-696-5937}


ABSTRACT


Printed Circuit Board (PCB) assemblies are


moving toward lead-free (LF) alloys and away


from the traditional Sn-Pb alloy [1].  This change


is creating new and unique failure modes as the


process adapts to accommodate the higher


temperatures of the new process [2].  In addition,


mis-processed lots are more likely due to the


complexity of assembling a mix of Sn-Pb and leadfree solders, components, PCBs, solder pastes, and


fluxes.  This case study helps to highlight the


challenge and provides an example of what can


happen, how to detect it, and how the defects can


cause reliability failures.


PCB assemblers are gradually moving toward LF


alloys mainly ternary Sn-Ag-Cu metallurgies. The


driving forces toward LF assembly include


regulation, environment, and global market


competition. Sn-Pb solder melts at 183oC; whereas


a typical Sn-Ag-Cu alloy melts at 20oC higher.


While this is the principal difference between the


Sn-Pb and LF PCB processes, there are other


significant challenges and issues to be considered


as the industry transitions to completely LF


assemblies. Some of these issues are:


1. Procuring 100% LF materials (PCBs,


components, connectors, pastes, etc)


2. Establishing LF processes that are backward


compatible with Eutectic


3. Determining thermal compatibility of boards


and components to new thermal profiles


4. Selecting solder paste chemistry to suit


assembly process and the soldered assembly


reliability and operating conditions [3]


5. Material and logistical control for simultaneous


processes; leaded and  LF


This case study examines motherboard failures


from a LF manufacturing process with leaded parts  being used on lead free boards utilizing LF pastes.


Samples


Four boards from one lot were identified with


electrical failures.  A common signature of


overheating was identified on two of the boards in  the area populated with two D-Pak FETs.  One of  the two boards was selected as representative and  will be discussed in this case study.   The two


FETs on this board are identified as Q1B2 and


Q3B2.


Procedure


The board was received and inspected both


visually and using real-time x-ray.  The visual


inspection did not detect any anomalies; however, the X-ray inspection identified potential voiding of  two FETs in D-Pak packages (Fig. 1).  The void is  in the heat tab area under the die. Both FETs were  then cross-sectioned in the plane indicated in


figures 1 and 2.


Figure 1:  X-ray images of FET component Q1B2 showing    possible voided areas. Cross section plane is shown by the  red lines.


Suspect  voided  areas  i


X


section  plane


5200 NE Elam Young Pkwy., MS HF1-08, Intel Corporation, Hillsboro, OR, 97124-6497


140


# Unique Failure Modes from use of Sn-Pb and Lead-Free (mixed metallurgies) in PCB Assembly: CASE STUDY


Figure 2:  X-ray image of FET component Q3B2 showing    possible voided area. The cross section plane is shown by the  red lines.


Q1B2:  Optical microscope inspection of FET  Q1B2 revealed that the solder had a layered  structure with distinct regions with different  microstructures (Fig. 3).  Additional inspection  using SEM with both secondary electron and backscattered detectors revealed that each layer had a  grain structure indicative of Sn-Pb and LF solder.  The separation of the regions was marked by the  sharp interface seen clearly in Figure 4.  EDS was  used to confirm the presence of two separate  regions one Sn-Pb and one LF.


Figure 3: Brightfield photomicrograph of cross sectioned  FET Q1B2. PCB/component interface; The grain structure  clearly shows the regions where LF solder did not intermix  with the Sn-Pb solder (see Fig. 4 for detail).  The void is to  the left, only partially visible in this view.


Figure 4: SEM photomicrographs of cross section Q1B2.


Solder of both types is clearly present; however it did not


melt long enough to intermix suggesting a lower temperature  Sn-Pb reflow profile was used.  Clear interface is shown


where LF/Sn-Pb solder did not coalesce.


Sn/Pb


grain


structure


LF


Suspect  voided  area


Sn-Pb      solder


Micro-crack


Eu


LF         solder


141


Figure 5:  SEM  images of FET Q3B2 showing ~ 3.5mm void  between component & PCB along the cross section plane.


Non-wet and voided illustrated. SEM image detail also


shown at 750X and 3000X.  Notice the eutectic


microstructure throughout the solder bulk and the IMC


evident at the PCB to solder interface.


Pb


see detail below


Figure 6:  EDS line scan of Q1B2 showing the boundary  between leaded and LF solder.


Q3B2:  Optical microscope inspection of FET


Q3B2 revealed that the solder had a single


microstructure and the presence of a large void


(Fig. 5). It shows the microstructure and the


presence of an intermetallic compound (IMC) at


the interface of the solder to the copper pad.  Using


SEM with both secondary electron and backscattered detectors revealed that the solder had a


microstructure typical for Sn-Pb solder.  EDS was


used to confirm the presence of lead and tin             (Fig. 6).  In the voided region, the surfaces were


inspected at higher magnification with no


intermetallic found.


The samples evaluated exhibit partly Sn-Pb


eutectic, partly Sn-Pb hypereutectic, (ie much more


tin than eutectic composition) layered structure.


See Fig. 7 for phase diagram.  Two aspects make


this microstructure very strange: (1) In part of the


solder joint, the Sn-Pb eutectic is near the FET and


in part of the joint, the Sn-Ag-Cu microstructure is


near the FET; (2) There has been no coalescence of


Sn-Pb eutectic and Sn-Ag-Cu segments. Even in


backward or forward compatibility solder joints


there is some amount of mixing. The PCB was


intended to use a LF process and reflow profile


with LF paste however the cross sections reveal a


Sn-Pb structure at the PCB interface suggesting


that leaded paste was printed unintended on a LF


PCB [4].


FET


PCB


5200 NE Elam Young Pkwy., MS HF1-08, Intel Corporation, Hillsboro, OR, 97124-6497 142


The layered structure, also suggests however


presence of LF paste as well. One hypothesis of


where the Sn-Ag-Cu paste comes from is that both  Sn-Pb and LF pastes may have been printed during  possible rework on these components. Traceability  to process control is very difficult to achieve


and/or validate for accuracy but evidence clearly


shows both Pb and LF pastes.


If rework was not a direct cause and a reflow


profile [5] such as shown in Figure 8 below was


used, proper mixing has not been achieved. This is  also aggravated by the large interface between the  FET component/PCB surface conducting heat


away rapidly, and causing the paste to only


partially melt. As a consequence, the electrical


performance of the overall system was affected


resulting in thermal hot spots on the PCB.


Although not uncommon for process voids to


occur under FET components, these FET samples  had extensive regions de-void of solder paste


material in the heat sink region resulting in hot


spots which caused the FETs to operate outside


their electrical specification causing an electrical


board fault.


Thermal analysis and X-ray were able to isolate the  failure to the FETs.  Cross-section and analysis of  the solder joint chemistry and microstructure were  critical to identify the root cause.  In this case


study, the failure was caused by two separate


issues; a) Improper mix of solder paste


b) Insufficient localized heat at the FET


components.  The solder paste material did  not reach a sufficient temperature to


complete melting and mixing.


Figure 7:  Ternary phase diagram of Sn-Ag-Cu. Melting  temperature of SAC solders converge around 218˚ C [6].


143


Figure 8:  Reflow  profile (temperature vs. time) shown for 9  thermocouples placed at various locations on the PCB board. Peak temperature ranging from 230-250˚C, soak temp 175-


217˚C and TAL (time above liquidus) above 218˚C shown.


With LF profiles the peak temperatures reach


approximately 250-260˚C compared to about 230-245˚C for reflow and wave respectively. As


transitioning to LF processes occur, a significant  requirement is to ensure that all materials can


withstand these elevated temperatures.


Corrective actions:


1. Make sure PCB manufacturers use only


Sn-Ag-Cu pastes on lead free process


2. Increase peak reflow temperature at the


FET thermal plane solder joints by at least  5˚C


This case study found leaded and LF parts within a  single PCB.  Installing leaded components onto a  LF board (or vice-versa) is a scenario that is


termed forward and backward compatibility


respectively (Fig. 9). Many cases and varieties of  this exist today and the number of cases is


increasing.


Mixed technology used in the transition from


eutectic to LF solders and components presents


increased risk to stress test and overall system


reliability.  Techniques developed for optimizing  and characterizing solder joints were utilized to


determine root cause for the failure.  These


techniques can also be used to detect improper


conditions before a failure occurs thus providing  better PCB reliability.


The increase in localized temperature and use of  Sn-Ag-Cu paste exclusively has remedied the


solderability problem observed on these samples.


Figure 9:  Board soldering compatibility


1. Overview of 2004 iNEMI Technology


Roadmap, Jim McElroy (iNEMI), IPC


Printed Circuits Expo/APEX/Designers


Summit, February 22-24, 2005, Anaheim, CA.


2. Norman J. Armendariz, ASM/EDFAS


Microelectronic Desk Reference, Fifth Ed.,


PCB SMT Solder Joint Failure Analysis


2004. p 513.


3. Promotional Literature:  “Kester Lead-Free


Solutions”, Kester Solder Co.


4. Private Communication; Mandy Mistkawi,


October 2004.


5. Prawin Paulraj Intel Corp. – LF reflow


profile


6. Phase Diagram Research, NIST,


Metallurgy Division, Gaithersburg, MD


144


Analysis Methods for Characterizing Drop Test Robustness of Lead-free FBGA´s


J. Walter *, R. Fischer, C. Birzer


Infineon Technologies AG, Regensburg, Germany


During the last few years the drop test has become more and  more important for electronic handheld components. Drop test  reliability for lead-free solder interconnects is an extreme  challenge today. Thus, the need for improved micro structural  diagnostics of new material combinations and crack detection  methods has increased.


The target of this paper is to summarize detection and analysis  methods for solder joint cracks, material characterization [1] and preparation methods of assembled printed circuit boards (PCB) after a drop test to completely understand lead-free  solder interconnect reliability in fine pitch ball grid array  packages (FBGA).


In particular, we will introduce the outstanding advantages of  embedded cross-sections combined with ion beam polishing (IBP), dye- or rather resin-penetration, selective tin etch and  micro-hardness measurements.


A main trend in microelectronics packaging during recent  years has been device miniaturization, especially in the  growing market of portable electronics such as notebooks, PDA-s and cellular phones. Therefore, the investigation of  reliability under mechanical drop or shock conditions has  become highly important [2]–[13]. One critical defect mode is  solder joint cracking between FBGA packages and the PCB (see Figure 1).


Figure 1:SEM image of a cracked solder ball after drop test


In order to prevent insufficient mechanical drop robustness of  the final portable electronics product, the semiconductor  manufacturers must assess the drop behaviour of their IC  components during package development. Most development  efforts focus on FBGA and PCB with lead-free solder joints, which will be the main future soldering technology, at least in  the portable electronics market. Lead-free solder joints behave  differently compared to tin-lead based solders due to the  changes in metallurgy and soldering temperatures. The target  of the mechanical shock studies and corresponding analytical  methods is to optimize the technological solution and to get a  deeper understanding about shock behaviour and failure  mechanisms.


Drop test


The evaluation of the drop test behaviour of IC components  requires controlled test methods on a standardized test board. This allows for the comparison of its drop/shock performance  independent of the end product. A commonly used method is  test standard JESD22-B111 (“Board Level Drop Test Method  of Components for Handheld Electronic Products”) [14].


The test vehicles used with this method are daisy-chain  packages, these are assembled on a standardized test board. This board uses built-up multilayer technology consisting of 8  copper layers, 1mm thickness and Cu-OSP (Organic  Solderability Preservative) pad finish, which is similar to  typical PCBs in portable electronics products. Fifteen equal  components are assembled on each of the test boards (see  Figure 2).


These boards are mounted with 4 screws in each corner on a  drop table with the packages hanging “face down”. The drop  table is driven down on guide rods and hits a base plate, which  is covered with a suitable material (see Figure 3).


77mm


132mm


Screw holes for  board fixture on  drop table


Figure 2: Example of test board according to JESD22-B111  with daisy-chained packages.


145


# Analysis Methods for Characterizing Drop Test Robustness of Lead-free FBGA´s


The drop height and the material on the base plate are adjusted  to reach a half-sine impact pulse of peak 1500G and 0.5ms  duration (controlled by an acceleration sensor mounted on the  drop table).


During the drop, the daisy-chained resistances are  continuously monitored. Intermittent interruptions, which can  be verified by interruptions in subsequent drops, are assessed  as failures. Electrical measurement after each drop without insitu monitoring is not sufficient, as broken solder joints  contacts may have partial mechanical contact again after the  drop pulse, which is then sufficient to show a nearly  unchanged electrical resistance value after completion of a  drop pulse.


According to JESD22-B111, up to 30 drops are performed  with this procedure. However, in some cases more drops are  necessary to get failures. One recommended quantity of  investigated samples is 60 devices (4 test boards with each 15  devices).


Figure 3: Schematic drop tester with PCB assembly on drop  table (picture from [11]).


After drop testing all test boards, the electrical failures are  documented by means of statistical methods such as Weibull  analysis.


Failure analysis


First, non-destructive analyses like Time Domain  Reflectometry (TDR) and X-ray microscopy of the open  connections could fail due to the insufficient spatial resolution  of the method. Next, mechanical cross-sectioning and highresolution scanning electron microscopy (SEM) are necessary. To simplify the interpretation of a high-resolution SEM  investigation an additional ion beam polishing step of the  mechanical polished embedded cross-section is recommended


[15]. In particular, the cross-section preparation of soft  materials by common mechanical grinding and polishing is  often affected by smearing effects. Interconnect failures such  as micro cracks and voids may remain masked, essential  details of the micro structure (grain boundaries, intermetallic  phases, porosity) cannot be investigated accordingly, and the  reliability of the analysis results is significantly reduced. Figure 4 describes the surface treatment of a cross-section  with two ion beam sources and an adapted sample holder  allowing loading complete embedded cross-sections with 25  mm in diameter.


Figure 4: Modified configuration for ion beam-based surface  polishing of cross-sections.


The first example shows a lead-free solder ball after a drop  test with a detected crack between the intermetallic compound (IMC) and the component copper pad (see Figs. 5.1 and 5.2). The ion beam polishing process removes scratches and  enhances the topography between different materials. Thus, secondary electron (SE) imaging allows easier detection of  cracks, IMC boundaries and voids.


Figure 5.1: SEM secondary electron (SE) image of a solder  joint crack mechanically polished only.


Testboard


146


Figure 5.2: SEM secondary electron (SE) image of same  position as Figure 5.1 after additional ion-beam polishing.


Quantitative analysis of crack areas


In addition to the electrical results, the following methods  allow quantitative analysis of (also partial) crack areas for all  solder joints of the package. Dye penetration test is a  commonly used preparation step [16]-[17]. In some cases an  epoxy-fluorescence resin-penetration method is a better choice  instead of the dye penetration method. This method is also  successful, if BGA´s with more than 300 solder balls are to be  inspected, while the standard dye penetration test could fail. The removal of these BGA´s of the board by standard method  needs higher shear or pull force, often resulting in cracking of  the package, smearing of the dye and possible  misinterpretation.


Figure 6: Embedded and planar grinded BGA before etching  with HCl.


During resin penetration method, the assembled device is  embedded face up or down with fluorescence resin under  vacuum, which is commonly used for embedded crosssections. The next step is top down grinding into the solder  ball area and then solder etching with Hydrogen Chloride


Acid (37 weight %). Figure 6 shows an image of an embedded  and grinded BGA before solder etching to inspect the solder  ball to component interface. After completely removing the  solder, together with the IMC and the copper pad, the solder  cracks can easily be detected with a UV-light microscope, showing a light green area.


Figure 7 shows a partially cracked solder joint marked by the  fluorescence resin. For statistical investigations the same  disbond templates as for the dye penetration tests can be used.


Figure 7: Crack (light region) with approx. 50% of pad area  in light green, activated by fluorescence light.


Interconnect characterization


For material characterization energy dispersive X-ray  spectroscopy (EDS) analysis is the most efficient method to  determine the IMC compositions of different solder or pad  material combinations, e.g. to detect small quantities of  additives in solder joints which enrich in the IMC. An  additional IBP step results in clearer grain boundaries for the  SEM/EDS inspection.


Platform B Results


• The serial port had no system or port level issues at 500V.


The system exhibited lock-up at 1kV, 2kV, 3kV and 4kV.


After the system was re-booted, system functionality was


restored.


Table 7: Platform B


I/O Port ESD Voltage Port Behavior System Behavior


500V


No Failure


1KV-4KV


Soft Failure


Parallel 500V-4KV


LOM 500V-4KV


500V-1KV


2KV-4KV


USB


Permanent Damage Permanent Damage


Video (VGA)


Platform


Air Discharge:


- no failure at all at 4KV


- no failure requiring


intervention to restore at 8KV


- no permanent damage 15KV Chassis Contact Discharge:


- no failure at all at 2KV


intervention to restore at 6KV


- no permanent damage at 8KV


Serial


Current  ESD Test(EN61000-4-2)


DCD Test


• The parallel port of Platform B lost video and exhibited a


system lock up at 500V and 1kV. A system AC power


cycle restored Platform B to full functionality.  At 2kV, the


system rebooted, but the system and the parallel port were


fully functional after an AC power cycle. At 3kV and 4kV


the system shut down, but again, functionality was restored


155


upon AC power cycle. ESD discharges to Platform B’s


parallel port induced no permanent damage, however, the


severity of the responses varied as the ESD event increased


in intensity.  The soft failures observed are considered high


severity since the potential for data loss is considerable.


• The LOM (LAN on Motherboard) in Platform B showed


no sensitivity to any of the ESD events (500V, 1kV, 2kV,


3kV and 4kV)


• The Video (VGA) port of Platform B showed no


sensitivity at 500V and 1 kV ESD levels. At 2kV, 3kV and


4kV, Platform B rebooted and failed to post (power-onself-test, lock up during boot). Once Platform B was AC


power cycled, the system fully recovered. Platform B ESD


sensitivity to 2kV and above should be investigated.


• The USB port on platform B exhibited permanent damage


when a 500V ESD event was applied. The system effect


was a lock up.  After AC power was cycled, Platform B


failed to boot. Motherboard LED diagnostics indicated a


memory issue (GYYY – green yellow yellow yellow).


Platform B has a high sensitivity to low levels of ESD; this


sensitivity can translate to high device failure rates in the


field. The USB port’s high sensitivity to low ESD event is


alarming in this case since the USB ports are defined as


hot-pluggable, which means a user is allowed to attach a


peripheral to the computer while the system is on.


Investigation of susceptibility of the USB port on platform


B has to be a high priority.


I/O Port Variation in Sensitivity


The study showed different sensitivity among I/O ports and  among different computer platforms. Each port ESD result  should be evaluated to decide whether improvement to ESD  sensitivity is required. For every system I/O port evaluation, the business decision to improve ESD sensitivity should  consider two different factors: usage model and historical  quality data for the I/O port in question.


System Power State


EN61000-4-2 and DCD is conducted with the system powered  on, while most IC/component level ESD tests are conducted  with the IC powered off. Table 8 summarizes the different  levels at which the EUT failed under DCD, EN61000-4-2, as  well as a direct discharge when the system was powered off. The direct discharge described in this table is very similar to  DCD, with the exception of leaving the AC power to off state. DCD (power on) failed at 200V whereas Direct Discharge (power off) failed at 4000V. Therefore, it is essential to have  the system fully powered on since ESD can easily trigger a  secondary effect like latch up as described by  Lakshminarayanan [8]. The system submitted to DCD in this  table experienced a latch up condition that led to EOS (Electrical Overstress) on the IC component.


Comparing to EN61000-4-2


With direct-pin ESD (DCD) testing, we have a very different  result on ESD susceptibility. Even though EN61000-4-2 is a


powered on ESD test, it does not address the ESD charge  flowing through the system I/O pins. In contrast to the  traditional ESD standard, DCD reveals higher sensitivity to  lower ESD voltage levels. Table 8 shows a failure at 200V  which is very low. To put this in perspective, it is very  difficult to feel ESD voltage below 3KV and walking on a  carpet can easily generate 1500V, even at 80% humidity.  The  user might not be aware of the ESD event at 200V which  occurs very frequently. The DCD test is able to catch system  failures at significantly lower ESD voltage levels.


Table 8: comparison between power state on DCD, Direct  Discharge, and RN61000-42


Test Method


SUT Power


State


Discharged  Voltage in Volts


System  Failure


DCD


ON


EOS


Direct Discharge


OFF


4000


None


EN61000-4-2  Air


8000


EN61000-4-2 - Contact


Case study results explain why electronic manufacturers  constantly customize their ESD testing beyond the current  ESD standards to include their learnings from previous field  experiences. However, field issues differ from one product to  another and even when testing is improved, electronic devices  continue to fail in the field. DCD provides upfront information  that can alleviate field issues and improve customer  experience. The goal of industry vendors is to improve  electronic device performance and reliability in the field. The  electronics industry needs to recognize that the ESD standards  as they apply today say nothing about power on testing at the  IC level or direct pin ESD discharge at the system level. Another factor current specifications do not address is ESD  transmitted through a cable path from a host to attached  device or vice versa. In other words, the user model needs to  be redefined to reflect a more accurate user environment.


Increased electronic device failures due to ESD are the result  of the advances in IC manufacturing technology, higher I/O  signal speed environments, an increasing number of electronic  products available to consumers, and the lack of a complete  specification that addresses powered on ESD events on I/O  interfaces. Electronic device designers are always looking for  a way to anticipate the usage model of their products to  provide the best consumer electronic device possible. The  increasing number of devices in the market make the  designer’s task very difficult.  The DCD ESD testing model  offers a new way to test electronic devices to help improve the  end customer experience as well as to reduce system level  failures due to ESD induced events. An industry wide ESD


156


standard could be the best solution since it can help regulate  the host device as well as the add-in devices.


The authors would like to thank Mr. Jeff Birdsley of Dell Inc. for his support and guidance. The authors would also like to  thank Mr. Bob Knoell of Visteon Corp. for reviewing the  paper and suggesting changes.


[1] M.A. Kelly, G.E. Servais abd T.V. Pfaffenbach, “An  Investigation of Human Body Electrostatic Discharge”, ISTFA 1993, 1993, pp167-173.


[2] Midwest Chapter ESD Association, Fundamentals of  Electrostatic Discharge: Part One – An Introduction to  ESD, 2001 <http://www.midwestesd.org/fundesd1.html> (28 June 2005).


[3] Chuck Hawkins, “EOS/ESD – What Are They, and How  Do You Tell the Difference”, Microelectronics Failure  Analysis UNM ECE-527 NTU IC535-NM Lecture 19, October. 2003.


[4] IEC/EN 61000-4-2, “Electrostatic Discharge Immunity  Test”, ESD ITE Specific Requirement.


[5] CISPR 24:1997 + Amendment 2:2002, “Information  technology equipment - Immunity characteristics - Limits  and methods of measurement”, CE - ITE Immunity  Requirements.


[6] M. Chagny, J.A. Naoum., “A Methodology for  Characterizing System-Level ESD Sensitivity”, ISTFA  2004, pp277-282.


[7] J. Deatherage, D. Jones, “Multiple Factors Trigger Cable  Discharge Event in Ethernet LANs”, Electronic Design, December.


2000, <http://www.elecdesign.com/Articles/ArticleID/4991/499


1.html> (29 June 2005).


[8] V. Lakshminarayanan, “Minimize ESD-induced  downtime”, EDN, March. 2005, pp83-88, <http://www.edn.com/article/CA509597.html> (7 July  2005).


[9] O.J. McAteer, Electrostatic Discharge Control, McGrawHill (New York, 1989).


[10] A. Amerasekera, C. Duvvury, ESD in Silicon Integrated  Circuit, John Wiley & Sons (New York, 1995).


157


X-ray Fluorescence Imaging For High Resolution Elemental Mapping


M. Feser, S. Seshadri, Y. Wang, W. Yun


Xradia Inc., Concord, CA USA  http://xradia.com, (925) 288-1228


X-ray fluorescence imaging is a novel non-destructive method to  obtain sub-100nm spatial resolution elemental maps with short  data acquisition times. The method has a wide range of  applicability in the field of semiconductor manufacturing and  semiconductor failure analysis. Imaging of copper interconnects  on ICs for the location of voids and shorts is one particular  application that is relevant for current and future needs of nondestructive inspection and failure analysis of backend processes.


X-ray fluorescence analysis is a widely used tool in  semiconductor manufacturing for characterization of thin films. Both electron and x-ray excited fluorescence instruments are  common. Sub-nanometer accuracy in the determination of film  thickness and the capability of determining film composition are  available on commercial instruments.


However, no technique is available to visualize these properties  with high spatial resolution on bulk samples. The spatial  resolution in current instruments is limited to the size of the  excited region, which can be as small as tens of micrometers for  x-ray beam excitation or on the order of a micrometer for electron  beam excitation.


Efforts are made to minimize the excitation spot size for electron  beam excitation by reducing the electron energy and thus  shrinking the volume in which x-rays can be excited [1]. But this  method restricts the analysis to only low-energy x-rays and  ultimately is limited to about 300nm resolution.


Alternatively, very thin samples (on the order of 100nm) can be  used to reduce the electron beam scattering in the samples. But  this methodology has the obvious limitation of preparing a very  thin, free-standing sample and therefore is only of limited  practical use outside the field of basic research.


To reach very high spatial resolution (<100nm) in x-ray  fluorescence analysis, the x-ray spectrometer has to be combined  with an x-ray imaging system that has an intrinsic x-ray imaging  resolution far lower than the excitation spot size. This can be  achieved with the use of a Fresnel zone plate as the x-ray imaging  optic. In this case a larger electron beam spot size can be used  without compromising the high spatial resolution of the imaging


system and, at the same time, retaining all the advantages of x-ray  fluorescence analysis such as high sensitivity to small elemental  concentrations and the quantitative measurement of thin films.


X-ray Fluorescence Imaging Using Zone Plates


The x-ray fluorescence imager described in this paper can be  operated as an attachment to electron-beam or x-ray beam  instruments. It easily can be accommodated on a standard  scanning electron microscope and the operation is similar to  existing energy or wavelength dispersive spectrometers.


X-ray imaging in this instrument is based on a high resolution xray lens known as a Fresnel zone plate. A zone plate is a  diffractive optic and takes the form of a circular transmission  grating as shown in Fig. 1. It consists of alternating concentric  grating rings, usually made of a metal and empty space. The  support of the zone plate is a very thin membrane that absorbs xrays very little. The height of the metal rings is chosen to be  either absorbing (for amplitude zone plates) or 180 degree phase  shifting (for phase zone plates).


Figure 1:  Schematic showing the principle of operation of a  Fresnel zone plate. X-rays from open zones interfere  constructively in the focus. The imaging resolution of a zone plate  is approximately equal to the outermost zone width ∆Rn.


The use of zone plates in x-ray imaging is already well  established and the theory of zone plates is well understood [2,3]. The imaging resolution of zone plates has continuously improved  over time and is connected to the advancement of nanofabrication  technology. Sub-20nm imaging resolution has been demonstrated


[4] already and further advances are expected.


If the first diffraction order of a zone plate is isolated by using an  appropriate aperture and/or central obscuration, it essentially


158


# X-ray Fluorescence Imaging For High Resolution Elemental Mapping


operates as a thin lens and as such obeys the basic imaging  equation


f


1=+ ,


where i and o are image and object distances respectively and f is  the focal length. The geometrical magnification M is then given  by


o i


M = .


(2)


A scanning electron micrograph of a partial zone plate is given in  figure (2).


Figure 2: A Scanning Electron micrograph of a gold zone plate  fabricated by Xradia Inc. The outermost zone width is 100nm and  the grating height is 1600nm..


In contrast to refractive lenses, zone plates are highly chromatic  and their focal length is inversely proportional to the wavelength  of the radiation. The use of a zone plate for x-ray fluorescence  imaging therefore requires the zone plate to fulfill the imaging  condition from Eq. 1 for the one particular wavelength of interest  for imaging. Other wavelengths are not imaged in-focus. Fig. 3  illustrates this for two wavelengths


1 λλ > . A central  obscuration is added to the zone plate for the creation of a  background-free region on the detector. The distances between  the source and the zone plate (L1) and between the zone plate and  the detector (L2) have to be readjusted to switch from imaging  one wavelength to another. The two wavelengths of interest could  be for example the x-ray fluorescence lines of copper and silicon  as shown in the applications section.


It is important to note that the spatial resolution of the x-ray  fluorescence image on the detector is not limited by the size of  the excitation spot. In fact, a larger excitation spot is typically  usually employed to image elemental distributions over a wider  field of view.


X-ray Fluorescence Imager Implementation


The system described in this paper is operated on a standard  JEOL-8600 electron probe micro analyzer. The x-ray  fluorescence imager has been fitted to one of the standard WDSports without any modification to the JEOL instrument. It also  keeps the same takeoff angle of 40 degrees as the WDS  spectrometers that ship with the JEOL-8600. Fig. 4 shows the  Xradia nanoXFi x-ray fluorescence imager highlighted as  installed on the JEOL-8600.


The use of a scanning electron microscope (SEM) platform is  advantageous, since it allows the use of standard electron  microscope functions such as high resolution secondary electron  imaging for location of the point of interest on the sample and  easy control of electron beam parameters. Especially tungsten  filament SEMs are a good choice, since for x-ray analysis a larger  electron current is needed and the electron probe size does not  affect the x-ray fluorescence image.


Typical electron beam parameters used for x-ray fluorescence  imaging are electron beam energies ranging from 2-25kV, beam  currents from 50nA to 5µA and electron beam spot sizes ranging  from a few µm to 40µm.


The x-ray fluorescence imager is equipped with a zone plate  manufactured by Xradia Inc. with a focal length of 2mm at  930eV x-ray energy (1.33nm wavelength) and an imaging  resolution of 50nm. It is operated in an x400 highly magnifying  geometry (at 1.33nm), in which the magnified fluorescence image  is formed on a CCD detector, which is nearly fully efficient for xrays with energies <5keV. The system has adjustments for  aligning the optical axis and a motorized focusing axis to enable  the detection of multiple elements.


Figure 4: Photograph of the experimental setup. The highlighted  portion is the Xradia nanoXFi x-ray fluorescence imager


installed on a JEOL-8600 Electron Probe Micro Analyzer.


159


One specific application of high-resolution x-ray fluorescence  imaging is the visualization and failure analysis of copper  interconnects. Sub-100nm resolution enables the detection of  defects such as voids and shorts and the inspection of copper  structures after CMP.


In the examples that follow the x-ray fluorescence imager was  used to image the Cu Lα1 (930 eV) and Si Kα1 (1.74 KeV) lines. In general, the x-ray fluorescence imager works best for x-ray  fluorescence lines <5kV to yield best throughput and signal to  background ratio.


To demonstrate the spatial resolution of the x-ray fluorescence  imager, we fabricated a copper structure consisting of lines with  varying line widths with a height of approximately 50nm. Fig. 5  shows one x-ray fluorescence image of the copper grating in an  area where the grating structure is defective (shown within the  white circle) and shows copper structures of varying sizes in a  random distribution. The grating pitch ranges from 180nm and  240nm in this image. Sub-100nm copper clusters are clearly  resolved. The electron microprobe was operated with a spot size  of 8 µm at 10kV and the beam current was 0.5µA. The effective


pixel size is 30nm. The total exposure time for this image was 10  minutes. During the image acquisition, small electron beam drifts  were observed. However due to the imaging nature of the  instrument, such drifts do not affect the x-ray fluorescence  imaging resolution.


Figure 5: X-Ray Fluorescence image of a copper zone plate. The  lines are 120nm wide and manufacturing defects smaller than  100nm are clearly visible.


Figure 3: Schematic showing the chromatic nature of a Fresnel zone plate. In the upper figure, the zone plate focuses x-rays


of wavelength 0λ . In the lower figure, the zone plate is translated towards the source such that rays of wavelength 1λ  are  focused on the detector. Notice that, in either case, only one wavelength is focused on the detector and the other wavelength  misses the detector completely.


1 um


160


Fig. 6 shows an area with finer lines of the same grating. The  experimental conditions were kept the same as before. The pitch  of these grating lines measured range from about 120nm to  140nm.


Figure 6: Image of a copper zone plate. The widths of the lines  measured range from 60nm to 70nm.


Next, the copper zone plate sample was replaced with a  multilayer copper sample. The imaging conditions were as  follows: Beam Voltage = 15KV, Beam Current = 1 µA. Fig. 7  shows the x-ray fluorescence image of the Cu Lα line.


Figure 7: Image of a Cu chip. The Cu regions appear as bright  and the Si regions appear dark. The widths of the Cu lines are  325nm.


Fig. 8 shows a blown-up version of the rectangular box of Fig. 7.


Figure 8: Magnified image of the rectangular region shown in  figure (7).


From Figs. 7 and 8, three layers of copper lines can be easily    seen. The number of layers seen depends upon the beam voltage  which determines the depth of penetration of the electrons into  the sample and the absorption of fluorescent x-rays before they  leave the sample. For imaging the Cu Lα line, the maximum  imaging depth is about 1.5µm and is limited by the absorption of  Cu Lα line within the sample. Actual values depend on the  specific makeup of the sample. To image structures deeper than  2µm, higher electron beam energies are necessary and the Cu Kα  line could be used for imaging.


The high spatial resolution obtained with the x-ray fluorescence  imager can be illustrated by comparing Fig. 7 with a typical  elemental map commonly obtained with an EDS/WDS  spectrometer by raster scanning the beam. Assuming that the  point spread function is 1.5 µm for 10-15kV electrons, the  convolution of Fig. 7 is shown in Fig. 9.


Figure 9: Convolution of figure (7) with a spreading function  assumed to be 1.5 µm.


The fine features clearly seen in Fig. 7 are completely lost in Fig.


9. This is to be expected since the spatial resolution of the  elemental x-ray maps obtained with EDX are limited by the  volume of interaction of the electrons inside the specimen  whereas the resolution of a zone plate is limited by the resolution  of the zone plate. The size of the electron beam on the sample  merely determines the field of view when using a zone plate.


For the same sample, the x-ray fluorescence imager has been  tuned to the Si Kα line at 1.74keV. In this mode, the main  constituent of the sample (Si) is imaged. Since x-rays generated  from Si get shadowed by copper lines running above, this  imaging mode is referred to as backlighting mode. The results are  shown in Fig. 10. The imaged area is exactly the same as shown  in Fig. 7 as were the operating conditions.


161


Figure 10: Image of the same area as in Fig. 7 using the Si Kα  line. Here, the Si regions appear bright and the Cu region  appears dark, since they shadow the x-rays produced by the Si.


Summary and Outlook


The experimental results demonstrate the power of the x-ray  fluorescence imaging technique in terms of spatial resolution  compared to EDS/WDS spectrometer fluorescence mapping. It is  important to note that the difference in spatial resolution spans  more than an order of magnitude. The other compelling property  of x-ray fluorescence imaging is the fact that it is a nondestructive method that can be applied to bulk samples such as  whole wafers in process. The high imaging resolution opens a  whole new range of applications relevant to the semiconductor  and nanotechnology industry. Elemental distribution with sub100nm resolution can be used for all sorts of patterned thin films  and patterned multilayer systems. Besides the already presented  applications in the characterization of copper interconnect  structures, this method is expected to open new possibilities in  thin film thickness and coverage characterization, elemental  analysis of contaminant particles and other applications that  require sub-100nm analytical resolution.


Multiple layers can be easily observed and upon proper  calibration, depth information can be easily obtained which is not  possible with conventional techniques. The integration times  needed to obtain an image are often in minutes compared to hours  required with conventional techniques. Elemental maps of  specific elements can be obtained one at a time and these maps  can be overlaid to generate a complete image of elemental  distributions in the sample of interest.


The simple integration of the x-ray fluorescence imager into  existing scanning electron microscopes or other electron beam  metrology platform makes it even more attractive, since no highcost standalone instrument is required.


Advances in nanofabrication techniques are expected to push the  resolution of zone plate lenses along with the ever decreasing  feature sizes on the ITRS roadmap [5] which makes it a  companion for future in-process metrology and offline failure  analysis.


[1] Sparks, C. J., “X-Ray Fluorescence Microprobe for       Chemical Analysis.” Synchrotron Radiation Research (H.


Winick and S. Doniach, Eds.) Plenum (New York, 1980) pp.


459-512


[2] Spiller, E. Soft X-Ray Optics SPIE (Washington, 1994) pp.


81-97


[3] Erko, A. I. et  al, Diffraction X-Ray Optics IOP Publishing


(Philadelphia, 1996) pp. 16-43


[4] Chao, W. et al, “Soft X-ray Microscopy at a spatial


resolution better than 15nm,” Nature, Vol. 435 (2005), pp.


1210-1213.


[5] ITRS. “Overall Roadmap Technology Characteristics”


International Technology Roadmap for Semiconductors 2004


Update pp. 1-21. The website address is:


http://www.itrs.net/Common/2004Update/2004Update.htm


162


3-D EBIC Technique using FIB and EB Double Beam System


Eiji Yoshida, Tomohiro Tanaka, Taro Oyamada, Tohru Koyama, Junko Komori, and Shigeto Maegawa  Renesas Technology Corp., 4-1, Mizuhara, Itami, Hyogo, 664-0005, Japan


yoshida, eiji@renesas, corn


We propose visualizing techniques of a diffusion layer using  an electron beam induced current (EBIC) for a site-specific  cross-section formed by focused ion beam (FIB) treatment. Moreover, we present a three-dimensional (3-D) EBIC  technique using a double beam (FIB & EB) system to  understmad the diffusion structure. This 3-D application of the  any local sectional EBIC technique is very useful for  delineating PN junctions mad pointing out implant defects in  ULSI devices. Furtfiermore, we applied the EBIC technique to  backside circuit editing with FIB. The end-point of the silicon  trench etching can be easily decided by observing the plane  EBIC images. Highly reliable backside circuit editing becomes  possible together with a DUV laser marking technique using  an IR-optical microscope system.


In modern ULSI devices, with their scaled-down structures, increasing number of metal layers mad the adoption of flip-chip  packaging, fault isolation and failure analysis has become  increasingly difficult. Doped structures, such as dopmat  distributions and PN junction profiles of source/drain or well  layers, and circuit design are the most significmat elements in  accomplishing high-speed, low-power devices. On the other


hand, there is the possibility of failure in a doped structure, which leads to serious problems because it is difficult to detect  the failure portion or may require a great deal of time to  resolve. Therefore, visualizing techniques of the diffusion  layer together with backside fault isolation techniques for fine


layer interconnects play a key role in developing high  performance devices and failure analysis.


Presently there are several techniques available for visualizing  the doped structure as a two-dimensional (2-D) profile [1].


Junction delineation by selective chemical etching is the most  common technique. The transmission electron microscopy (TEM) is a 2-D technique with very high spatial resolution, and when combined with chemical junction delineation, has  been reported to be capable of detecting dopant levels in the


low 10E16cm-3 range [2-5]. However, in practice it is difficult  to apply this technique to detect low-doped profiles, such as  well profiles. Furthermore, this technique lacks repeatability


owing to its dependence on chemical etching. Scanning probe  microscopy techniques, such as SCM (Scanning Capacitance  Microscopy) and SSRM (Scmming Spreading Resistance  Microscopy), can delineate a 2-D dopant distribution through  electrical characterization [6-8]. Nonetheless, the evaluation of


may exposed cross-section formed with FIB is impossible  because of the damaged layer on the surface of tile sample.


For the failure analysis of ULSI devices, it is necessary that the  mmlysis technique can be applied to any local cross-section. We have investigated visualizing techniques of the diffusion  layer in various local cross-sections formed by FIB using  EBIC [9]. It was found that the EBIC image that reflected the  diffusion profile including wells was obtained in the crosssection exposed by FIB treatment. Furthermore, we developed  a 3-D EBIC technique to understand the diffusion structure  using the sectional EBIC method.


For advmaced devices, the backside fault isolation technique  with FIB is especially difficult to apply without damaging the  DUT. Major problems of backside circuit editing with FIB  include difficulty in clear end-point detection for silicon trench  etching and accurate positioning of target interconnects. We  tried to apply the EBIC technique to the backside circuit  editing, and found it extremely effective for detecting the endpoint of silicon trench etching. Moreover, we developed a  laser maxking technique for accurate backside positioning. We  confirmed that the reliability of backside circuit editing  improved dramatically when combining these techniques.


Cross-Section EBIC with FIB


The electron-hole pair is generated by irradiating electron  beams (EB) to the PN junction, and is detected as EBIC  signals.


Cross-section exposed by FIB


Fig. 1 Block diagram of the cross sectional EBIC technique.


163


# 3-D EBIC Technique using FIB and EB Double Beam System


The EBIC image is formed by converting the electromotive  current detected by the EB irradiation in brightness, synchronizing witJa beam scanning, and displaying the image  on a CRT. Therefore, the EBIC image indicates the  distribution of the electrostatic potential such as the depletion  layer. We have investigated visualizing techniques of the  diffusion layer in any local cross-sections formed by FIB  treatment. A damaged layer of about 20-30nm exists on the  surface of cross-sections formed by FIB with an acceleration  voltage of 30KV. It is necessary to induce a carrier through the  damaged layer when the EB is scanned onto the cross-section, as shown in Fig. 1. However, the excitation area that extends  into the silicon substxate becomes small due to the lowering of  the energy of a primary EB. In dais experiment, the primary  EB within the range of 1-5KV witJa an acceleration voltage  was used in consideration of the detection performance of the  EBIC detector (current amplifier). The range in the excitation  area in that case was about 20-400nm as shown in Fig.2 [10].


1.4


%" 1.2


e E  • ~ 1.0


g& ~=~ 0.8


o ~  0.6


~ 0.4 c  c


rYLU 0.2


.... Primary EB(Eo)....I ........ i ....... i.....


_


"1 $i sub. Exci ta t ion"~- i i .Revi i i i i l l  . . . . . . . . . . . .  ! . . . . . . .  . . . . . . .


0 1 2 3 4 5 6 7 8 9 10


Primary EB Energy [Eo] (kev)


Fig.2 Range in the excitation area and extension radius as


it corresponds to the primary electron beam energy.


It was reported that the PN junction keeps its properties as a  junction even if its cross-section is exposed by FIB sectional  treatment [9]. The shallower n+/p junction of about 0.1 pm was  observed using a sectional EBIC technique shown in Fig.3. The electromotive current between the upper electrode and  silicon substxate was converted to the EBIC image. Fig.3(b) shows the EBIC image correlated to the structure in Fig.3(a). The depletion layer of the n+/p junction is visualized as a  bright contrast layer. Fig.3(c) shows the EBIC profiles on the  dotted line in Fig. 3(b) for each acceleration voltage. Increasing  the acceleration voltage causes the electromotive current to  increase. Therefore, it is possible to improve the sensitivity of  the EBIC signals by increasing the acceleration voltage of the  EB. However, the spatial resolution of the EBIC image  becomes degraded because of the expmasion of the excitation  volume. Thus, it was confirmed that EBIC strengda increases  as the EB energy increases.


Figure 8: SEM secondary electron (SE) image of an ion-beam  polished Cu/Ni/Sn ternary alloy as IMC and performed EDS  spot analysis.


copper pad


tin bulk


spot of EDS analysis


147


Figure 8 presents an SEM image after IBP of a solder to pad  interconnect with clear visible IMC.


Quantitative EDS analysis could detect a quantity of 3 at.% Nickel in the Cu6Sn5 phase (see Figure 9 and Table 1). If the  structure is smeared from the mechanical polishing, this  quantitative analysis would be impossible.


Figure 9: EDS spectra of the highlighted spot in Figure 4.


Standard less quantitative EDS analysis:


Element k-ratio (calc.)


ZAF


Atom % Element  Wt %


Sn-L


0.5411


1.082


42.96


58.54


Cu-K


0.4230


0.933


54.09


39.47


Ni-K


0.0221


0.900


2.95


1.99


Total


100.00


Table 1: Quantitative analysis of performed EDS spectra of  the highlighted spot in Figure 4.


The second important preparation method is the selective tin  etching method with a 2-Nitrophenol solution. The purpose of  this method is to allow for the possibility to inspect the  wetting behaviour of solder balls and to investigate the IMC  formation between the component/PCB pad and the tin of the  solder ball bulk over the whole pad area. Selective tin etching  is a treatment of the bare package, e.g. after reflow simulation  or the assembled device on board in a solution of 2-Nitrophenol and sodium hydroxide in water. The method can  also be used to remove the package from the board without  thermo-mechanical stress (instead of de-soldering).


For lead-free solder ball alloys, SnAg(0-4wt. %)Cu(0-1wt. %) plus additives is the most used alloy. On copper surfaces this  forms a scalloped IMC surface of Cu6Sn5 with more or less  Ag3Sn dendrites sitting above. This IMC formation has an  influence on the board reliability of the solder ball, especially  on drop test robustness. Figure 10 shows an example of an  Ag3Sn – dendrite on a component pad after selective tin  etching.


Figure 10: Ag3Sn – dendrite after selective tin etching.


Figure 11 points out a non-wetted area in a solder ball  interconnect. This investigation is used to compare the wetting  behaviours of different ball materials, pad surfaces, or  optimize reflow processes.


Figure 11: Non-wetted area of a solder ball, visible after  selective tin etching.


Micro hardness measurement is a powerful method that uses a  cross-sectioning technique to characterize mechanical  properties of solder balls. To ensure proper measurement, an  additional IBP process is used to prevent smearing and  scratches on the sample surface. The measurement itself is  performed with a micro indentor, e. g. a pyramidal Vickers  diamond (see Figure 12).


148


Figure 12: Imprint of micro hardness indentor in ion-beam  polished cross-section.


The indentor is pressed with a given force and time into the  material. The force – depth characteristics enable calculation  of following parameters of the solder ball material: Martens  hardness, Vickers hardness, plastic fraction of deformation, elastic deformation module (proportional to E modulus), and  creeping of material. A preferable test area is a bigger volume  of the solder bulk material to average over crystalline  precipitations in the bulk. This volume should contain Ag3Sn  or Cu6Sn5 dendrites. The results allow a prediction of the  ductility of the used solder material, which also affects the  reachable drop test performance. On the one hand, hardness  and ductility is determined by the reflow process, quantity, temperature profile, ramp down rates and its variations during  production process. On the other hand, it is affected by  elemental admixtures into the solder bulk material. Some  common admixtures into tin are elements such as Ag, Cu, Bi, Sb, In or lanthanides which influence inter-metallic formation  at the interfaces, solidification and crystal growth. A reduction  of silver content for instance reduces the micro hardness and  improves the ductility in general.


130 140 150 160 170 180 190 200 210 220 230 240 250


initial sphere


after


1st reflow


2nd reflow


SAC105 1% Ag


SAC305 3% Ag


SAC405 4% Ag


solder A


supplier A


Figure 13: Martens hardness values showing influence of  reflow process and silver content.


Figure 13 shows the influence on Martens hardness of the  number of reflow processes for a given solder. The softening  of the solder with the first reflow is dependent on the spheres  production process of the supplier, such as initial crystallinity. The hardening with more reflows is probably caused by  crystal growth and inter-metallic compound formation. The  figure shows the hardening effect with increasing silver  content in a tin based solder, containing 0.5% copper. This  increase is most likely caused by different solidification  behavior of varied silver content. Figure 14 points out the  correlation of the same variations as in Figure 13 to the plastic  fraction revealed by micro hardness measurement. The graph  gives an impression how the plasticity of the solder material  changes could be optimized. Demonstrating that this test  method gives additional access to material parameters of  solder materials affecting drop test robustness.


93 94 95 96 97 98 99 100


ductile


brittle


Figure 14: plastic fraction values showing influence of same  parameters as in Figure 13.


An overall method for investigation and interpretation of  solder joint interconnects after drop test does not exist. Only  the combination of different preparation, measurement and  imaging methods can provide the basic for the best  interpretation and assessment of different solder ball  interconnects and materials to determine drop test robustness. The best preparation methods are cross-sectioning together  with ion-beam polishing, dye or resin penetration tests and  chemical tin-etching with 2-Nitrophenol solution, in  combination with optical- and scanning electron microscopy  and µ-hardness measurement.


The authors would like to thank B. Seidl and M. Huettinger  for their support in sample preparation and preparation recipes  and K. Pressel for his general support in this abstract.


149


[1] Armendariz N. and Paulraj P. “Materials Characterization  of Lead Free Compositions for Minimum Temperature  SMT Processes at the SLI-Second Level Interconnect  Solder Joint”, 30th International Symposium for Testing  and Failure Analysis


[2] Yu Quiang., Watanabe K., Tsurusawa T., Shiratori M, Kakino M.and Fujiwara N., “The Examination of the drop  impact Test Method”, Inter. Society Conference on  Thermal Phenomena, 2004


[3] Chong D., Ng K.; Tan J.and Low P.; Drop Test  Reliability Assessment of leaded & Lead-free Solder Joits  for IC Packages ; 54th Electronic Components and  Technology Conference; 2004


[4] Chiu T.Z., Zeng K., Stiermann R., Edwards D., Ano K., “Effect of Thermal aging on board level drop reliability  for Pb-free BGA packages”; 54th Electronic Components  and Technology Conference, 2004


[5] Luan J.and Tee T.Y., “Analytical and Numerical analysis  of impact pulse parameters on consistency of drop impact  results”, 54th Electronic Components and Technology  Conference; 2004


[6] Amagai, M., Toyoda, Y., Ohnishi, T.and Akita, S., “High  drop test reliability: lead-free solders”, 54th Electronic  Components and Technology Conference; 2004


[7] Xie D. Arra M., Yi S. And Rooney D.; “Solder Joint  Behavior of Area Array Packages in Board Level Drop  for Handheld Devices”; 53rd Electronic Components and  Technology Conference; 2003


[8] Amagai, M.; Toyoda, Y.and Tajima, T. “High solder joint  reliability with lead free solders”, 53rd Electronic  Components and Technology Conference; 2003


[9] Tee T.Y., Ng H. S., Lim C.T., Pek, E.; Zhong Z., “Board  level drop test and simulation of TFBGA packages for  telecommunication applications”, 53rd Electronic  Components and Technology Conference, 2003


[10] Saha S.K.,. Mathew S. and Canamulla S. “Effect of  Intermetallic Phases on Performance in a mechanical  Drop Environment 96.5 Sn 3.5 Ag on Cu and Ni/Au Pad  Finishes”, 54th Electronic Components and Technology  Conference; 2004


[11] Canumalla S., Yang H.D., and Viswanadham P., “Method  for Measuring Package to Board Interconnection Shear  Strength for Area Array, Fine Pitch Packages” , 28 th  International Symposium for Testing and Failure  Analysis, 2002,


[12] Gupta V., Tian J., Hartfield Ch., Zeng K., Chiu Ch. and  Roger Stierman “Measurement of Solder Joint Strength  and its Dependence on Thermal Aging in Freestanding  and Board-Mounted Packages Using a Laser Spallation  Technique”, 28 th International Symposium for Testing  and Failure Analysis, 2002,


[13] Kujala A., Reinikainen T. and Ren W., “Transition to Pb–free Manufacturing Using Land Grid Array Packaging  Technology” 52th Electronic Components and  Technology Conference; 2002


[14] JEDEC STANDARD JESD22-B110 Subassembly  Mechanical Shock


[15] Mack W., Seidl B., Fischer R., Ort T., Walter J., Grünewald J., Berthold L., Petzold M. „Ion beam  polishing for Embedded Cross-Sections and its  Advantages for FESEM Analysis in Electronic  Packaging”, 30th International Symposium for Testing  and Failure Analysis, 2004


[16] K. Donghyun; J.M.D. Filho; P. Changyoung; A. Mawer; T.J. Moon.and G.Y. Masada, “Crack length analysis of  SnPb and SnAg solder joints in plastic ball grid array  packages from dye penetration studies”, 53rd Electronic  Components and Technology Conference, 2003.


[17] Armendariz N., PCB-SMT Assembly Failure Analysis  Tutorial, 30th International Symposium for Testing and  Failure Analysis


Developing a More Inclusive System Level ESD Characterization Methodology


Johan Rahardjo, Socorro Miller, Leo Lopez, Steve L. Williams


Dell Inc., Round Rock, Texas, USA


ESD (Electrostatic Discharge) has become an increasing  problem on electronic devices. The electronics industry is  always looking for ways to improve the reliability of  electronic devices by enhancing their test methods. The  industry has found that the current ESD test methods do not  encompass all possible scenarios to which electronic devices  are exposed at the customer site.


This paper describes a novel method to bridge the gap  between current system level ESD specifications and customer  real world situations. Field failure investigations led us to  discover a new customer situation where ESD is induced on a  computer system through a peripheral/cable that is already  attached (different than hot-plug event).  To simulate this  scenario, ESD was injected directly into the signal pins of the  bus being tested, creating what we call the DCD (Direct  Contact Discharge) test methodology. This paper compares  DCD against the current ESD standards and demonstrates that  introducing DCD into the current ESD testing methodology  will significantly lower the system field failures. DCD is not a  replacement for current ESD testing practices in the industry; DCD is a complement that allows a more inclusive ESD test  coverage.


ESD is the spark or event that typically occurs when two  objects of different electrostatic potential approach each other.  This phenomenon takes place most frequently in low humidity  conditions, where the likelihood of electrostatic potential  build-up increases. The transfer of electrostatic charge can be  caused by direct contact or induced by an electrostatic field.  The resulting electrostatic discharge generates high voltage  transients that might damage electronic components.


ESD events are recognized as a significant contributor of early  life failures and failures throughout the operating life of a  semiconductor device [1]. Technology advances in IC (Integrated Circuit) feature size and I/O bus speeds allow the  proliferation of affordable consumer devices that include  cellular phones, personal digital assistants (PDAs), printers,


and external storage, to mention a few. ESD affects  production yield, manufacturing cost, product quality, reliability, profitability, and customer satisfaction.  While few  components may be catastrophically or permanently damaged  to an extent where they fail completely, many may suffer  damage that is not immediately apparent. Electronic  manufacturers have found that testing devices to the industry  ESD specifications is not enough to ensure the reliability of  their designs. As a result, manufacturers of electronic devices  improve their test methods to include any lessons learned from  field issues. The goal is to ensure better performance of their  products in the field.


This paper starts with a brief overview of ESD theory and its  current effect on electronic devices. It continues by describing  the system level failure modes due to ESD. It then covers the  current ESD standards and test methodology, as well as  explaining how the specifications are applied to the electronic  devices. Following exploration of the gaps between the  current test methods and the actual customer environment, it  proposes a novel methodology to complement the current  ESD test methods. The analysis includes a comparison  between current test methods and the proposed method, where  it shows that the proposed method simulates real customer  environments. The theory is supported with data collected  using all the described ESD test methods on several computer  systems. The paper concludes by summarizing the result of  our experiment and recommending Direct Contact Discharge  as a viable solution for improving electronic device reliability  and customer experience.


Electrostatic Discharge Theory


Electrostatic Potential Generation


ESD is defined as the transfer of electrostatic charge between  two objects of different electrostatic potential. Electrostatic  charge is caused by an imbalance of electrons on the surface  of a material which produce an electric field. There are many  ways electrostatic potential is generated, but the most common  is triboelectric charging. Triboelectric theory dictates that  dissimilar materials will acquire charge separation when  mechanically rubbed together. This charge separation is due to


151


# Developing a More Inclusive System Level ESD Characterization Methodology


mechanical (phonon) energy transfer that releases electrons  from their parent atomic shells.


Table 1 shows material charge order; materials further apart  from each other on the table typically generate higher  electrostatic charge than materials closer together [3]. For  example, a human hand rubbed with silicon rubber generates  higher electrostatic charge than glass rubbed with wood.


Table 1: Material Charge Order


Charge


Material


Most Positive


Air


Human Hands Asbestos


Rabbit Fur


Arcrylic


Phenolic


Cellulose Acetate Glass


Quartz


Mica


Human Hair


Nylon


Wood


Wool


Lead


Silk


Aluminum


Paper


Cotton


Steel


Amber


Hard Rubber Nickel, Copper


Brass, Silver Gold, Platinum Silicon


Teflon


Most Negative


Silicon Rubber


Electrostatic voltage variables/factors


The level of electrostatic potential depends on friction, frictional area, humidity, temperature, contact pressure, and  area of dissimilar materials [3]. Table 2 shows the relationship  between relative humidity (RH) and charge voltage for a  given activity.


Table 2: Humidity vs. electrostatic voltage


at 20% RH at 80% RH


Walking across vinyl floor


12,000


250


Walking across synthetic carpet


35,000


1,500


Arising from foam cushion


18,000


Pick up polythylene bag


20,000


Slide Styrene box on carpet


Trigger vacuum solder remover


8,000


Aerosol circuit freeze spray


15,000


5,000


Static Voltages (V)


Activity


ESD damage


ESD damage to electronic components includes metallization  breakage (joule heating can blow open a metal line or contact  by melting, vaporization or electromigration), oxide rupture at  the transistor/field oxide, stress induced spiking of metal  through p-n junction (source/drain to substrate short circuit), and latch-up. At a computing system level, the damage might  show itself as shutdown, reboot, loss of video, and / or system  lock up.  Table 3 summarizes the effect of ESD on computer  systems (system level).


Table 3: System level ESD failure


System Response to  ESD Event


Damage


Mechanism


Lock up


Temporary functional  failure


Invalid State machine state  that requires system reset


Shut down


Possible permanent  damage given enough  repetition


Overcurrent or overvoltage  event that trips the PSU; requires a reset on AC to  clear fail-safe flag


Reboot


Overcurrent or overvoltage  event that trips the


motherboard regulator


Exothermic event


Permanent damage


EOS, latch up, thermal runaway


Current ESD Standard & Test Methodology


EN61000-4-2: ESD Immunity Test


There currently exist a number of test standards written to  evaluate the effects of ESD exposure.  EN61000-4-2 is  perhaps the best known and most widely applied standard to  electronic devices used in computers.  EN61000-4-2 is a  European Standard written to encompass system level testing. It defines environmental test parameters, such as humidity and  atmospheric pressure, that shall be present during testing and  also specifies the pulse criteria that the applied event shall  adhere to.


152


Table 4: EN61000-4-2 Standard


Test Name


ESD Level


Criteria


1 ±   2 kV Air Discharge


2 ±  4 kV


Air Discharge


3 ±   8 kV Air Discharge


3 ±  12 kV Air Discharge


4 ± 15 kV Air Discharge


1 ±  2 kV


Discharge


3 ±  6 kV


4 ±  8 kV


Test parameter


Electrostatic  Discharge (ESD)


Immunity


The ESD event chosen by the EN61000-4-2 standard is  referred to as the Human Body Model (HBM), whereas it is  designed to simulate the waveform of an ESD event that  would occur when applied through a person holding a metal  device, such as a screwdriver.  The standard dictates that the  ESD events shall be applied to all locations of the EUT (Equipment Under Test) that can be readily accessed during  normal operation.  EN61000-4-2 specifically excludes direct  ESD discharges to the EUT I/O pins or open connectors. Table 4 and Table 5 describe the test parameter and  acceptance criteria for EN61000-4-2 testing.


Table 5: EN61000-4-2 Passing Criteria


Performance


Definitions


The apparatus shall continue to operate as intended, i.e., normal unit  operation, and no degradation of performance


The apparatus shall continue to operate as intended after completion of the  test.  However, during the test, some degradation of performance is allowed  as long as there is no data loss or operator intervention to restore apparatus  function.


Temporary loss of function is allowed to include loss of volatile memory.  Operator Intervention is acceptable to restore apparatus function.


Enhancement on ESD test for the past few years


While testing to the procedures specified in EN61000-4-2  subjects the EUT to literally hundreds of ESD events, feedback taken as a result of field issues tends to indicate that  adherence to this standard alone does not adequately ensure  that an electronic device will operate without upset during its  end use. One such example was described by Chagny and  Naoum [6], where system upsets were experienced when a  floppy disk was inserted into the floppy disk drive.  In this  instance, the sliding metal flap had a residual charge.  As the  floppy was inserted into the drive, the charge transfer from the  flap to the drive structure produced an electromagnetic field  that in turn was interpreted by internal electronics as a valid  signal, causing the system to shut down.  Another example is  the Cable Discharge Event on the Ethernet LAN as described  by Deatherage and Jones [7]. When the charged cable is  connected, the ensuing high-energy discharge may damage the  transformer circuit or the Ethernet transceiver.


Approach taken to acquire   a more inclusive method


Electronic devices (computer systems) often contain several  I/O ports where devices are attached to interface with the  system; common computer I/O ports are: 1394, USB, PS2, Serial, Parallel, and LOM. The current system level standard  does not address the multiple ways that ESD can come into  these I/O ports. A case study was used to understand the most  common ESD failures at the system level (lock up, re-boot, loss of port functionality, IC exothermic events). It was  performed on common ports across two different computer  models.


There was historical data on system serial port failures due to  ESD transfer via the serial port. The electrostatic potential was  generated by friction between a portable device and its leather  case. The system passed the EN61000-4-2 test. However, quality data showed a high serial port failure rate that  translated into a replacement unit (whole system exchange). Using the DCD test methodology (explained below), we were  able to replicate the failure signature of the system and port’s  IC. It was determined that an ESD event was occurring when  the portable device was hot-plugged into the cradle that was  attached to the system’s serial port.


The goal of finding a new method is to include these three  usage models:


• First, an EUT-attached device receives an ESD discharge.


This method is equivalent to a statically-charged user


making contact with the I/O device already attached to the


system.


• Second, a charged device is hot-plugged into cable or


device attached to the EUT. This method is equivalent to a


user hot-plugging a portable device to an attached cradle.


• Third, a charged device is hot-plugged directly into the


EUT I/O port. This method is equivalent to a user walking


across a carpeted room holding an I/O device and inserting


it into the system’s I/O port.


DCD (Direct Contact Discharge)


Introduction to DCD (Direct Contact Discharge) method


DCD testing is performed by injecting contact discharge ESD  directly onto the I/O pin while the EUT is powered and fully  configured. A DCD test targets one I/O bus at a time at a  specific voltage level.  A typical starting voltage is 200V, increasing to 4kV.  The test setup is similar to EN61000-4-2  for tabletop equipment. The ESD gun simulator used during  this test is the Dito ESD Simulator (as shown in Fig. 1) from  EM Test with sharp electrode contact discharge tip (rise time


0.7~1.0 ns as described in EN61000-4-2).


153


Figure 1: Dito ESD Simulator


DCD Test Procedure


DCD testing is performed per the following steps:


• Step One: Select the I/O bus to be tested and identify the


pin-out of the I/O port. Knowledge of the pin-out will help


to understand the system’s reaction to the ESD event and


how to correct issues found during testing.


• Step Two: Power up the EUT and verify I/O port


functionality. A loopback plug or I/O device might need to


be attached to verify functionality. After functionality is


verified, remove the loopback plug or device from the I/O


bus under test.


• Step Three: Configure the ESD gun for contact discharge


and adjust to the starting voltage (typically 200V). The


ESD gun/waveform generator must comply with


EN61000-4-2.


• Step Four: Apply 10 discharges to the pin, making sure the


tip of the gun makes good contact. A dongle as shown in


Fig. 2 might be used if the pin is difficult to access.  It is


important to test one pin at the time to be able to isolate the


effects of the ESD event. Figure 2 shows the lab set up


created to test the USB ports in a system.


Figure 2: DCD Test Setup


Figure 2: DCD Test Flowchart


• Step Five: Observe/record system behavior to the ESD


event and verify functionality of the EUT. Functionality


testing must be performed not only on the tested port, but


also the whole system. The failure could be a functional


failure (lock up, loss of functionality, etc) or sublime


failure (slight increase in current or temperature of the


device related to the I/O under test). Such a failure might


cause a reliability issue after a period of time. The failure


might be induced by the electric field of the ESD or real


voltage induced by the ESD gun through the available


path. While some failures are instantly detected, many I/O


ports may suffer damage not immediately apparent (latent


defect). A very small increase in temperature (due to slight


increase in leakage and standby current on the IC of the


port under-test) might suggest this defect.


• Step Six: If a failure is detected, cycle the AC power and


verify whether the system recovers. Should the failure


remain (permanent damage), stop the test. Otherwise,


document this temporary upset and continue to step seven


below.


154


• Step Seven: Increase the ESD voltage level and repeat


steps four through step six. The DCD cycle ends when the


high ESD voltage limit is reached (typically 4kV for


DCD), or permanent damage is observed.


DCD Test Case study


Description of Experiment


During this case study, two different systems (desktop  computers) were submitted to DCD testing in addition to   traditional ESD testing. Tables 6 and 7 contain a summary of  the test results for each I/O port tested. To differentiate test  results, we will refer to them as Platform A and Platform B. The following system ports were tested: Serial, Parallel, integrated LOM, integrated Video (VGA), and USB. The  DCD test methodology was followed as outlined in the DCD  flow chart (refer to Fig.1). The system’s I/O ports were  submitted to the following ESD voltages: 500V, 1kV, 2kV, 3kV and 4kV.


It is important to note that Platform A and Platform B  exhibited failures due to ESD even after they had passed  traditional ESD testing.  It is also prominent that systems  failed at significantly lower voltage levels with DCD test as  compared to traditional EN61000-4-2 testing.  The tables also  show that each I/O bus fails at various ESD voltage levels. Each system and port behavior is discussed below.


Platform A Results


• The serial port had no issues at the system level or port


level when tested at 500V to each signal pin. Platform A


exhibited a lock-up at 1kV and the port was no longer


functional even after the system was power cycled. The


rest of the system’s functionality was preserved. 1kV was


enough to permanently damage the serial port in platform


A. The DCD testing cycle ended for this system at 1kV.


This kind of failure typically results in a motherboard or


whole system dispatch to the customer. In some instances,


since the ESD stimuli may still be present in the


customer’s environment, repeated unit replacements are


necessary.


• The parallel port had no issues at 500V. At 1kV the port


lost functionality during the ESD discharges and the


system locked up.  Following a system power cycle of


Platform A, port and system were fully functional. When


the ESD event was set to 2kV, 3kV, and 4kV the system


lost video and locked up. The diagnostic LED indicators


on the back of the system showed video engine failure


(GYGG – green yellow green green). Once again


rebooting the system allowed platform A to fully recover.


ESD discharges in the parallel port had no permanent


damage. The system’s loss of video and lock up behavior


constitutes a soft failure. While not permanent, this type of


failure is considered critical since the potential for data  loss is considerable.


Table 6: Platform A result


1KV


Permanent Damage


2KV


3KV-4KV


Video 500V-4KV


Parallel


LOM


• The LOM (LAN on Motherboard) port on platform A had


no errors at 500V and 1kV. At 2kV the system locked up,


but system/port functionality was restored after an AC


power cycle. The ESD field might have coupled onto some


other system signals, causing a logic failure. No


system/port issues were detected at 3kV and 4kV.


• System lock-up occurred at 500V testing to the VGA


signal pins. A system power cycle returned the video and


the system back to normal functionality. When the ESD


event was set to 1kV, 2kV, 3kV and 4kV, video was lost


and the system locked up. A reboot of Platform A restored


the system and video port to full operation.


• The USB port on platform A had no issues when subjected


to 500V, 1kV, 2kV, 3kV and 4kV. This is the port most


used and has high probability of experiencing hot-plug


usage.


(a) Cross-section structure.


De~


Lay


Si sub


(b) EBIC image correlated to Fig.3(a).


..,


o 3.0


IZ.


4.5 0


5 K V - -  /


500 1000 1500 2000 2500 3000  EBIC Current (xl0-SA)


(c) Profiles on the dotted line in Fig.3(b).


Fig.3 N+/p junction was observed using the sectional


EBIC technique.


As shown in Fig.4, the damaged layer exists on the surface of  the cross-section formed by FIB etching. This layer is  amorphous and several nmaometers thick, as shown in the  TEM photograph, and is formed by the physical impact of high  energy FIB. It influences the generation and recombination of  the carrier during EB irradiation. Therefore, we attempted to  reduce the damaged layer, mad investigated the influence on  EBIC detecting. Low-damage etching using low acceleration  FIB was applied as the removal process of the damaged layer. Fig.4 shows sectional TEM photographs before(a) mad after(b) removal processing. When the low acceleration beam of 5KV  was scmmed for 60 seconds, the damaged layer of 20nm or  more decreased to about 8nm. The change in the EBIC signals  was then observed. Fig.5 shows the chmage in the EBIC  image(a) and the EBIC strengda(b) at the acceleration voltage  of 1KV corresponding witJa the removal processing time.


164


,a er'K su . I


" - .................... (a) ~ ~ ; ~


" ';


":.i.


8 .7nm I # ~ '


" " .


/


Fig.4 Sectional TEM photographs showing the change in the  damaged layer before(a) and after(b) removal processing.


Osec 30sec 60sec 190secJ 120sec


1.8 )l~1-[~ 240sic 210iec 18~sec l i  0sec


0.0 50 100 150 200 250 300 350


EBIC Current (xl0-SA)


Fig.5 Change in the EBIC image(a) and the EBIC


strength(b) corresponding with the removal processing time. The acceleration voltage of FIB is 5KV and Ip 50pA, and  the acceleration voltage of EBIC is 1KV and Ie lnA.


A 0 . 6   E - t


0 . 9   e -


1.2


O n


A minimum of 90 seconds of removal processing actualized  the EBIC image. This couldn't be confirmed before processing (0sec). The EBIC strength increases greatly from 90sec to  150sec of removal processing so that the influence of the  damaged layer decreased. Moreover, it was observed that  continuing the removal processing caused the image to expand  downwaxd without changing the EBIC strength. It was  clarified that the damaged layer formed on the surface  decreased by the addition of low-damage etching using low  acceleration FIB, and that EBIC images can be observed using  a low energy beam of about 1KV. Despite these findings, the  optimization of the removal processing of the damaged layer is  difficult because the EBIC strength and area change due to the  removal processing conditions. It is then considered that the  damaged layer should not be removed and the EBIC images  should be observed with an acceleration voltage of 2-3KV for  a stable observation, because the influence of the damaged  layer is low at that acceleration voltage, as shown in Fig .2.


3-D Cross-Section EBIC


By using the sectional EBIC method, we developed a 3-D  EBIC technique that makes use of the best features of double  beam FIB equipped with EB. The block diagram of the 3-D  EBIC technique is shown in Fig.6. The double beam (FIB & EB) system used is the model SMI3000SE series with a  current image acquisition system produced by SII  NanoTechnology. In the double beam system, it is possible to  observe SEM images of the cross-section simultaneously with  slicing by FIB. The 3-D image consists of numerous EBIC  images, which are obtained automatically by repeating the  slice and acquisition. The 3-D image of a bipolar transistor is  shown in Fig.7. This is synthesized from fifty EBIC images


acquired by using a 0.1gm pitch. The EBIC images were  obtained by the EB with an acceleration voltage of 3KV.


l l -


/ pr°cess,nYA1


Fig.6 Block diagram of the 3-D EBIC method.


165


It has already been reported that the resolution of 2D-EBIC is  less thma 18nm using a primary EB with an acceleration  voltage of 3kV [9]. The resolution in the direction of the depth  is less thma 20nm, mad is determined by the pitch of FIB  slicing. This 3-D application of the local sectional EBIC  technique is very useful for delineating PN junctions and  pointing out implmat defects in ULSI devices. It was found that  3D-EBIC images can be synthesized with the double beam (FIB & EB) system, mad it was revealed that the 3-D diffusion  structure, including the wells, can be recognized in may part of  an ULSI device.


EBIC images were observed clearly with the double beam  system. In that system, it is possible to observe the EBIC  images of the trench floor simultaneously with the plane  etching by FIB. We acquired the EBIC signals using a primary  EB with an acceleration voltage of 15kV. According to the  Kanaya-Okayama Range shown in Fig.9 [10], the excitation  range was about 3~tm when the EB was irradiated to silicon.


Fig.10 shows the plane EBIC and SEM images of n-wells at  the acceleration voltage of 15KV for each remaining thickness  of the silicon trench. The sample device was fabricated by a  90nm process technology. The bright contrast areas in the  EBIC images indicate the depletion layer of the bottom of the  n-wells shown in Fig.10(a). It is found that the EBIC signals  change from the bottom to the edge of the n-wells as the  remaining thickness thins, as shown in Fig.10(b) and (c). This  is because the EBIC signals axe generated at the PN junctions  of the bottom of the n-wells when the remaining thickness is  thick. Subsequently, the EBIC signal is generated at the PN  junctions of the edge of the wells flarough the bottom. This is  because the excitation area becomes deep as the thickness  thins. Further thinning causes the EBIC signal to be lost as the  EB penetrate the n-wells, as shown in Fig.10(d). The EBIC  images of the wells chmage gradually as the remaining  thickness becomes thinner. However, no pattern can be  observed with SEM even in the same thickness shown in  Fig. 10(e).


Fig.7 3-D EBIC image of a bipolar transistor.


Backside Circuit Editing using Plane EBIC


Backside circuit editing is usually processed using global  mechanical thinning and local FIB etching from the backside  of the silicon substrate. The silicon trench is etched by FIB  after mechanical thinning. Silicon trench etching should be  stopped when the remaining thickness of the silicon substxate


is 1-3~tm, in order to avoid damaging the DUT. As previously  mentioned, end-point detection is a major problem in backside  circuit editing. We tried the plmae EBIC technique, for which  the spatial resolution is high and the signal detection is easy, to  decide a more accurate end-point of silicon trench etching, even though voltage contrast by FIB is commonly used [11]. The block diagram of that EBIC technique is shown in Fig.8. The p+ active area and n-well were connected with the EBIC  amplifier flarough the sample stage. P-sub was grounded. The


rY


EB


Fig.8 Block diagram of the EBIC technique for end-point  detection of silicon trench etching.


10.00


9.00


8.00


7.00


6.00


5.00


4.00


3.00


2.00


0.00


Kanaya-Okayama Range


~ J


Primary EB Energy (keY)


Fig.9 Excitation range in silicon as it corresponds to the  primary electron beam energy.


166


a, rel minin i , a* r


(c)


(d)


SEM at 1.7um remainint


shown in Fig.ll(c).  Fig . l l (d)  shows the IR image after  applying flae laser maxking surrounding the target interconnect  on the silicon backside. The laser mark and CAD layout  pattern axe linked with flae double beam (FIB & EB) system, mad flae target interconnect was edited by FIB. Fig. 12 shows  flae sectional SEM photograph of flae editing example of  drawing out flae M4 interconnect to the silicon backside. Thus, it was revealed flaat flaese techniques axe useful for backside  fault isolation as flaey help decide the trench end-point using  the plmae EBIC image as well as the positioning of the target  interconnects using the DUV laser marking.


(e)


Fig. 10 EBIC and SEM images of the silicon trench floor at an acceleration  voltage of 15KV for each remaining thickness of the trench. The bright


contrast areas in the EBIC images indicate the depletion layer of the n-wells.


The remaining flfickness of about 2gm where flae EBIC images


of flae n-wells disappear is flae optimum position for FIB


circuit editing. Thus, flae end-point of flae silicon trench etching


can be easily decided by observing the plane EBIC images due


to the high EBIC spatial resolution and flae strong EBIC signal.


Backside Circuit Editing using Laser Mark


After silicon trench etching, it is necessary to accurately decide  the position of target interconnects. Therefore, we developed a  neaJc-infrared (IR) optical microscope system wifla a  wavelengfla of 1300nm, equipped with a DUV laser marking  function. That system is flae model SOM3355-IR produced by  SII NanoTechnology. In the IR-optical microscope system, flae  coordinates are mutually linked by sharing flae double beam (FIB & EB) system wifla flae sample stage. The DUV laser wifla  a wavelength of 355nm was used for flae laser marking in flae  same column. Fig. l l (a)  shows flae IR-optical image from flae  silicon backside before flae trench was etched. The sample  device was fabricated by an 180mn process technology. Fig. 1 l(b) shows the IR-optical image of flae trench floor after  the trench was etched. The active area can be clearly  confirmed before mad after trench etching. In addition, by  overlaying the IR image wifla flae layout pattern using a CAD  linkage, the position for flae laser marking was determined, as


(a) IR optical image from the


silicon backside before trench


etching


~-.~,~:.. " ' -  ~. -":.~'~-t~


- - " - '  ~ "~--'~ " ~ "  '-=']~1


~ .~,.~.2. '°-- ~2"..-" ~ ,  ~,..--~i,.=..._,.21~3 N I ~ - ~ _ : _ .  ! - ~  ± _-ri,: i.,~.~l. ~ , . i


E1N ~ - ~ .


"~IN ---:I.IL"~':-t


~ M ~ I I ~ I I I B t : '  -" "--"  " ' " !"Z! .  -'-.:


(b) IR optical image of the trench  floor from the silicon backside


after trench etching.


(c) Overlaid image of the IR


optical image and CAD layout


pattern.


Fig. 11 IR optical image observation and DUV laser


marking with SOM3355-IR for backside circuit editing.


(d) IR optical image after


laser marking on the silicon  backside.


Fig. 12 Sectional SEM photograph of the editing example of  drawing out the M4 interconnect to the silicon backside.


167


We proposed visualizing techniques of the diffusion layer


using an EBIC for a site-specific cross-section formed by FIB  treatment, with the double beam (FIB & EB) system. By using


the sectional EBIC method, we developed the 3-D EBIC  technique to understmad the diffusion structure. The 3-D  application of the any local sectional EBIC technique is very


useful for delineating PN junctions and pointing out defects in  ULSI devices. The 3-D EBIC technique of high-spatial


resolution makes it possible to explore new methods of failure  analysis mad fault isolation concerning the diffusion layer and  active area. Moreover, we applied the plane EBIC technique to  backside fault isolation with FIB. It was clarified that the plane  EBIC technique facilitated in deciding the end-point of silicon


trench etching. Furthermore, highly reliable backside circuit  editing became possible together with the DUV laser marking


technique using an IR-optical microscope system.


We would like to thank N. Takeshita, T. ¥oshizawa and K. Nil  for offering the experiment samples and supporting the device  circuits. We would also like to thank T. Asahata mad H.


Takahashi from SII NmaoTechnology for their technical advice  and support in conducting our experiments.


[1] L.A.Heimbrook, F.A.Baiocchi, T.C.Bittaaer, M.Geva, H.S.Luftxnma and S.Nakahara, "Practical perspective of  shallow junction analysis", J.Vac.Sci.Technol.,1996, B14(1), pp.202-212


[2] R.Alvis, R. Sinclair and P.Griffin, "Physical  characterization of two-dimensional doping profiles for  process modeling", J.Vac.Sci.Technol.,1996, B14(1),


pp.231-235


[3] C.Spinella, V.Raineri, F.La Via and S.U.Campisano, "Two-dimensional junction profiling by selective  chemical etching: Applications to electron device  characterization ", J.Vac. Sci.Technol., 1996, B14(1),


pp.414-420


[4] D.Maher and B.Zhang, Proceedings of the Second  International Workshop on the Measurement and


Characterization of Ultra Shallow Doping Profiles in


Semiconductors (AIP), 1993, pp.263-267


[5] C.Hill, Proceedings of the First International Workshop  on the Measurement and Characterization of Ultra


Shallow Doping Profiles in Semiconductors (AIP), 1991,


pp.3-12


[6] Y.Huang, C.C.Williaxns,


mad M.A.Wendman,


"Quantitative two-dimensional dopant profiling of abrupt  dopant profiles by cross-sectional scanning capacitance  microscopy", J. Vac. Sci. Technol., 1996, A14(3),


pp. 1168-1171.


[7] H.Edwaxds, R.McGlothlin, R.S.Maxtin, Elisa U, M.Gribelyuk, R.Mahaffy, C.K.Shih,


R.S.List, V.A.Ukraintsev, "Scanning capacitance spectroscopy: An


analytical technique for pn-junction delineation in Si  devices", Appl.Phys.Lett., 1998, Vol.72, No.6, pp.698-700


[8] P.De Wolf, W.Vandervorst, H.Smith and N.Khalil, "Comparison of two-dimensional carrier profiles in  metal-oxide-semiconductor field-effect


transistor  structures obtained with scanning spreading resistance  microscopy


and


inverse


modeling",


J.Vac.Sci.Technol.,2000, B18(1), pp.540-544


[9] T. Koyaxna, M. Umeno, K. Sonoda, J. Komori and Y. Mashiko, "Locally delineating of junctions and defects by  local cross-section electron-beam-induced-current  technique ", Microelectronics reliability, Vol.41, pp. 1243-


1253 (2001).


[10] K. Kaxmya and S. Okayama, J. Phys. D 5 (1972), pp.43-58 [ll]Christian Boit, Kristin R. Wirth, and Erwan Le Roy, "Voltage Contrast like Imaging of N-Wells" Proc. 29 th  ISTFA, pp.331-337 (2003)


168


Analysis of a Microcircuit Failure using SQUID and MR Current Imaging


Frederick Felt


NASA Goddard Space Flight Center, Greenbelt, MD, USA


SQUID and MR magnetic sensors have separately been  used for fault isolation of shorts and resistive opens in  integrated circuits and packages.  These two  technologies were once considered to be mutually  exclusive, although recent studies [1] rather pointed to  their complementary character.  This paper shows, for  the first time, the use of these two sensors together to  isolate a low resistance short in a Quad-NAND gate  microcircuit.


Electrical test confirmed low resistance shorts between  three of the device pins.  However, internal optical  inspection found no evidence of failure.  The low  resistance of the shorts was deemed insufficient for  liquid crystal analysis.  Magnetic current imaging with a  SQUID sensor confirmed current flow through the  package lead frame and isolated the defect to the  microcircuit.  Due to package design and the resulting  distance of the scan plane, the SQUID was unable to  resolve the current path on the microcircuit.  In parallel  with the SQUID, a magnetoresistive (MR) probe was  employed to fit inside the device cavity, make direct  contact with the microcircuit, and map high-resolution  current images.  Two sites with high-current density  were accurately identified by MCI in input transistors.  Subsequent deprocessing revealed that the defects were  located under a broad sheet of aluminum metallization  which blocked optical detection, and rendered detection  by thermal emission difficult.


Anomalous performance of a Quad NAND gate  microcircuit was noted during environmental testing of  the IPE LVPC subsystem for the SWIFT project at  NASA Goddard Space Flight Center.  Trouble-shooting  of the subsystem determined that four pins were shorted  to ground.  Inspection was halted and the system was  powered down when the device was noted to be  overheating.  The malfunctioning device was forwarded  to the NASA GSFC Failure Analysis Laboratory for  evaluation.


The microcircuit is a 5962R9654201QXA device with a  0033 date code.  The part is a radiation-hardened, quadruple 2-input NAND gate microcircuit with Schmitt  triggers featuring 1.2-micron CMOS technology, and  rated for operation from –55C to +125C.  The device  was hermetically sealed in a 14-pin ceramic flat-pak  with metal lid.


The package was optically inspected and photodocumented (Figure 1). Radiographic examination  revealed a multi-level lead frame inside the ceramic  package.  Particle-impact noise detection (PIND) and  leak testing found no anomalies.


Curve tracer testing confirmed electrical shorts ranging  in resistance from approximately 2 to 5 ohms between  pins 6, 7, and 10; respectively Y2, Vss, and A4 (Figure  2). The I-V curves for essentially all other pin  combinations were noted to be unstable.


Figure 1: Top-down view of the Quad-NAND gate in a  ceramic package and metal lid with part markings.


The metal lid was removed from the ceramic package  revealing the internal package cavity with the  microcircuit (Figure 3).  Careful optical inspection of the  cavity and the microcircuit was performed both at low, and high magnification, but no anomalies were found.


169


With the lid open, curve tracer testing re-confirmed lowresistance electrical shorts between pins 6, 7, and 10.


Testing to this point indicated that the device was  malfunctional, but no evidence of failure had been  found.  Liquid crystal technique was ruled out as a  failure analysis tool because the low resistance of the  shorts, up to 5 ohms, was deemed insufficient to  generate Joule heating for detection by liquid crystal  analysis.  Calculation shows that a 5 mA current applied  through a 5.3-ohm short generates only 132.5  microwatts.  Obviously, applying higher current in order  to force detection using this method risked additional  damage to the failure site.  How, then, to proceed?


Figure 2: A curve-tracer plot indicates a linear 2-ohm short  between pins 7 and 10.  Shorts with Pins 6 and 10 were  similar, ranging up to 5 ohms.


Figure 3: Internal image of the die cavity after lid removal, showing the die, attach material, wires, and posts.


For this application, magnetic current imaging (MCI) appeared to be a suitable method for detection of the low  resistance shorts.  MCI is a non-destructive technique, which measures the magnetic field generated by moving  electric charge in a conductor.  Its reliance on current  detection, rather than traditional thermal detection used  in failure analysis, seemed ideal to map the lowresistance current path in this microcircuit.  By  comparison, liquid crystal analysis relies on the  secondary, and potentially hazardous, thermal effects  due to resistive current flow.  In theory, low resistance is  an obstacle for liquid crystal analysis, but an advantage  for magnetic current imaging. For this reason it was  modestly hoped that MCI current mapping could  identify the circuit path for each short, and that when  compared to the circuit layout, the maps could be used to  identify intersection common nodes in the current path  and assist the failure analysis process.  But as will be  shown, MCI was able to do somewhat more than  expected.


Magnetic Current Imaging


Magnetic current imaging (MCI), as applied to failure  detection in the semiconductor industry, is based on the  measurement of the magnetic field generated by current  carried in the structures of the device under test (DUT). The detected magnetic field is used to map the current in  the device by using a Fourier Transform back-evolution  technique [2, 3].  The resulting current map can then be  compared to a circuit diagram, an optical/infrared image, or a non-failing part to determine the fault location.  As a  tool for mapping electrical current in electronic  packaged devices, it was only recently introduced to the  semiconductor community in 1999 [3,4 ].  Since then, it  has become a mainstream tool for package-level fault  isolation [5, 6] and an effective tool for die-level fault  isolation [7-9].


For MCI applications on integrated circuits, magnetic  fields are typically measured with a SQUID (Superconducting Quantum Interference Device) or a  magnetoresistive (MR) sensor [10].  The differences  between these sensors correspond to sensitivity and  resolution.


SQUIDs are the most sensitive magnetic sensors known


[2], and for electronic fault isolation they are typically  designed to have field sensitivity around 20 pT (about 2


170


million times smaller than Earth's magnetic field).  This  allows one to scan currents of 500 nA at a working  distance of about 400 microns. As for all near field  situations, the resolution is limited by the scanning  distance or, ultimately, by the sensor size (typical  SQUIDs are about 30 µm wide), although software and  data acquisition improvements allow currents to be  located within 3 microns.  To operate, the SQUID sensor  must be kept cool (about 77 K) and in vacuum, while the  sample, at room temperature, is raster-scanned under the  sensor at some working distance z, separated from the  SQUID enclosure by a thin, transparent diamond  window. This allows one to reduce the scanning distance  to tens of microns from the sensor itself, improving the  resolution of the tool.


The best MR sensors are about 2 to 5 orders of  magnitude less sensitive than SQUIDs but they are  easier to scale down in size (below 100 nm) to provide  resolution less than 300 nm.  Although the sensitivity is  lower, the absence of an enclosure allows one to bring  the sensor closer to the circuit (scanning in soft contact  mode, typically 1-2 µm) and thus, it has magnetic  sensitivity to map out submicron current lines carrying  about 1 mA or more.  Images of currents as small as 300 µA have been obtained [11] with continuous  improvements.  This proximity along with the smaller  physical size of the sensor allows for improved  submicron resolution.


The typical MCI sensor configuration is sensitive to  magnetic fields in the perpendicular z direction (i.e., sensitive to the in-plane xy current distribution in the  DUT). This does not mean that we are missing vertical  information; in the simplest situation, if a current path  jumps from one plane to another, getting closer to the  sensor in the process, this will be revealed as stronger  magnetic field intensity for the section closer to the  sensor and also as higher intensity in the current density  map.  This way, vertical information can be extracted  from the current density images.  Further details about  MCI can be found elsewhere [10].


All MCI scans were taken with a Neocera Magma C30  Magnetic Current Imaging System with dual SQUID and  MR sensors.  This dual sensor built-in capability allowed  for quick, accurate registration between magnetic scans (with any sensor) and optical images of the scan area for  physical location of features detected in the current  density images.


Sample Preparation


The microcircuit in the open ceramic package was  mounted on a standard SEM puck, and placed in a  Teflon carrier.  Lead wires were micro-soldered to the  affected pins of the flat-pak device, and elevated slightly  above the aluminum puck to avoid shorting. This  assembly was degaussed at a distance from the MCI  instrument, and then placed in the MCI instrument for  analysis using the Magma tool.  Following standard  best-known procedures, the analysis started with a  SQUID magnetic scan.  A standoff distance of a few  mils was necessary in order to avoid contact between the  SQUID head and a ridge of solder around the device  cavity.


The purpose of scanning the entire device with SQUID  was primarily to inspect the lead frame inside the  ceramic package for shorts.  SQUID was expected to be  better than MR in this application, inasmuch as MR is  less sensitive than SQUID and therefore more dependent  on being close to a current path.  Feature resolution  using magnetic current imaging is fundamentally  dependent on distance for both techniques.  Both the  lead frame and the microcircuit were recessed inside the  package, but it was hoped that SQUID could map  current flow in the relatively wide dimensions of the  lead frame metal, whereas the feature size of  metallization on the microcircuit was much smaller.  Closer scanning by the SQUID was not possible because  the probe size was too large to fit inside the device  cavity.


Because the magnetic field is highly dependent on the  distance of the detector from the current-carrying source, accurate leveling of the microcircuit was necessary.  This was accomplished by touching down with a  measuring probe on each corner of the device.  Some  frustration was experienced at this step until it was  realized that the gentle pressure exerted by the  instrument at touchdown locations tended to push the  SEM puck slightly deeper into its carrier, and render  prior measurements useless. In addition, despite the  degaussing procedure, residual magnetization from the  nickel ring around the perimeter of the device cavity was  suspect of interfering with signal detection by the  SQUID.  For these reasons, the part was removed from  the SEM puck and the nickel ring was carefully lapped  off.  The device was re-mounted on a glass slide,


171


providing a more stable mount.  Lead wires were resoldered and secured in place by tape.  Electrical testing  confirmed that the pin-to-pin shorts were unchanged.


These changes were found to be adequate.  The device  was easily and successfully leveled.  Removal of the  solder ridge and nickel ring eliminated stray  magnetization and allowed the SQUID head to approach  a few mils closer to the device, resulting in greater  sensitivity and improved resolution of the instrument.


Fault Isolation


MCI SQUID testing was performed with Pin 6 grounded  and +1.4V applied to Pin 10, resulting in an applied  current of approximately 1.0 mA through the DUT.  (The instrument features an internal series 1300-ohm  resistor.)  Because of the extreme sensitivity of the  SQUID detector to magnetic fields, current was  alternated at a frequency of 9.557 kHz—a prime  number—in order to discriminate between the magnetic  field from the DUT and background magnetization from  the environment.


Using this set-up, the instrument successfully mapped  the intensity and up or down direction of the magnetic  field across the area of the DUT.  A Fourier Transform  algorithm was then used to convert the raw plot into a  current path, which loops in red starting at Pin 10; through the lead frame, bond wires, and microcircuit  before exiting at Pin 6 (Figure 4).  Two locations of high  current density, shown in yellow, indicate where the  arcing bond wires make their closest approach to the  scan plane of the SQUID.  Computer-generated arrows  superimposed on the plot point in the direction of  electron flow.


The magnetic current path was superimposed on the  optical photograph of the DUT in order to create a  composite image showing current flow through the  device package (Figure 5).  This result clearly  demonstrated that the anomalous short was located in the  microcircuit and not the lead frame of the DUT.  Resolution was lacking at the die because the  microcircuit was recessed in the device cavity several  hundred microns below the scan plane of the SQUID  head.  Nevertheless the current path appeared to favor  one side of the die, approximately in the region between  Pin 6 and Pin 10.


Similar maps were obtained when testing the shorts  between other pin combinations.  In all cases testing  indicated that the lead frame was okay, and not a source  of the shorting.


Close inspection of the images also showed evidence of  current leakage in the plane of the die, as well as through  bond wires at the upper and lower right of Figure 4.  Curiously these pins were electrically open, suggesting  that the detected current flow was due to parasitic  capacitance in the lead-frame.  The cause for the  racetrack patterns observed in both images is because of  remaining strong static magnetic field (DC field) leakage  onto the acquired data form the applied AC signal.  Comparison of the MCI map to the x-ray photograph  showed that the racetrack patterns overlay the lead frame  where lead frame traces converge at wire posts.


Figure 4:  Magnetic current imaging using the SQUID probe  shows the current path between Pins 6 and 10.  Computergenerated arrows indicate direction of current flow—a path  that matches an x-ray image of the lead frame.


172


Figure 5:  The current path detected by SQUID is  superimposed on an optical image of the DUT.  Pins are  labeled, with Pin 6 (Y2) at top, and Pin 10 (B3) at bottom.  Resolution was adequate for the package lead frame, but  could not discern detail on the die.  Nevertheless most current  appears to flow through the left side of the device.


In summary, magnetic current imaging using a SQUID  probe successfully mapped current through the package  lead frame of the DUT, but was unable to map detail on  the microcircuit because the SQUID dimensions  prohibited it from fitting inside the device cavity where  distance would be reduced and resolution improved. Nevertheless, the SQUID magnetic current map isolated  the failure to the die by conclusively demonstrating that  the short was not in the multi-level device lead frame.


Obtaining better resolution of the current path on the  microcircuit required the use of a giant magnetoresistance (MR) sensor.  This probe is smaller than the  SQUID, and consists of a sandwich structure  approximately 20 nm x 100 nm mounted on a substrate


1.0 x 1.5 mm, in a cantilever configuration.  This size  allowed the MR to fit within the device cavity and  actually touch the die.  Although less sensitive than  SQUID technology, the MR probe makes direct contact  with the die surface, a few microns from the current path  where magnetic field strength is much greater than in the  scan plane of the SQUID probe.  This distinct advantage  allows the less-sensitive MR probe to scan orders of  magnitude closer than the SQUID and resolve  microcircuit patterns only a few microns in size.


As seen in Figure 7, the DUT microcircuit features two  parallel rows of bond wires on opposing sides of the  microcircuit.  The die measures 2520 by 3160 microns, but 22 percent of its width is consumed with bond pads  and elevated wires.  These dimensions left the MR probe  only a few hundred microns of wiggle room.  Moreover, the suspect region identified by SQUID appeared to be  located near one row of wires.  To compensate, it was  found that the MR probe could be angled slightly, allowing it to scan an elongated rectangle bounded by  bond pads on one side, and extending inward  approximately 200 microns. Angling the probe in this  manner resulted in minor bending of the wires, but did  not short the wires or interfere with current mapping.  The MR probe had greater freedom in the length of the  die, but it was important to not go over the die edge, which could cause damage to the delicate probe.


Figure 7:  The DUT features two parallel rows of wires.  Scanning movement of the 1.0 by 1.5 mm MR probe was  constrained within this area.  The probe was angled slightly in  order to scan closer to the bond pads on the side of the  suspected defect.


Test current was increased from 1.0 mA used with the  SQUID, to 10 mA for the MR in order to compensate for  differences in sensor sensitivity.  The value of the series  sample load resistor in the electronics was decreased  from 1.3 kΩ to ~10 Ω.  Frequency was increased to 30.0  kHz in order to optimize the operation of the MR probe.   Magnetic current imaging with the MR probe was  initially performed with Pin 6 at ground and Pin 10 at +0.7 volts (peak-to-peak), with a 0.5 V offset.  The  resulting magnetic current map was overlaid with the


173


optical image is seen in Figure 15, at the end of this  paper.  A high-density current anomaly was noted in  each FET input transistor associated with the Pin 6 and  10 metallization.  Current flowing from the Pin 10 bond  pad conformed to the geometry of the metallization until  reaching the input transistor, at which point the current  should divide between the four metal transistor fingers.  Instead, a high-density current anomaly is seen in the  FET.  This anomaly appears to bend, possibly  downward, then diffuses, as noted in Figure 8, across a  plane to the FET associated with the Pin 6 bond pad, where a similar defect is seen.  The appearance of the  defects strongly suggested shorts.


Figure 8:  MR current mapping shows an anomaly of highcurrent density followed by diffusion over a plane.  A decrease  in field strength is seen as the metallization steps down into  the contact window, followed by an increase in density as  current converge.


MR mapping with high resolution at the suspect location  in the Pin 6 FET illustrates the direction of current flow  using computer-generated arrows at operator-selected  points (Figure 8).  This image is color-inverted for better  contrast.  Note that signal strength in the MR image  decreases as the current steps down approximately a  micron over the oxide step.  This illustrates the  sensitivity of the instrument to distance from the current  source.  Also note that the tail of the anomaly weakens  slightly without changing diameter.  This suggests a  second change in distance; presumably the current path  is sloping downward, increasing its distance from the


sensor.  This aspect of current mapping suggests some  ability to perform three-dimensional current path  analysis.


The magnetic current map seen in Figure 9 overlays the  optical image, and shows the approximate location of the  anomaly in the Pin 6 FET.  Optical and MCI images  appear to have an offset of about 7 microns, indicated by  opposing white arrows.  The lack of a distinct shoulder  in the geometry made determination of the misalignment  in the other axis difficult.


Figure 9:  The current map is superimposed on the optical  image, showing an anomaly inside the transistor.  Arrows  indicate a possible offset between optical and magnetic  images.


Similar results were obtained for the Pin 10 FET.  Figure  10 shows a close-up MR map superimposed on the  corresponding optical image.  The current, shown in blue  for enhancement, confirms a region of high-current  density in the transistor.  Instead of dividing among the  transistor fingers, current concentrates in an anomaly  with step down behavior, suggesting a descending  current path and likely short location.  The centerlines of  the current path and of the metallization stripe are  indicated with white lines. The white arrow inside the  FET is equal to the misalignment and shows the  probable corrected position of the anomaly, approximately near the base of the third finger counting  from left, a not uncommon failure location.  In this  image, the length of the shoulder as the current turns


174


before entering the FET is not sufficient to estimate  misalignment in the other axis.


Figure 10: The MR current map and optical overlay for the  Pin 10 FET are shown above.


Both suspect transistor locations were examined  optically and in the SEM.  No evidence of failure was  visible (Figure 11).  It was noted that a wide sheet of  metallization completely covered the transistors, leaving  only their topography visible, and concealing possible  defects underneath.


The top level of glassivation was removed using plasma  etch.  This exposed the underlying metal layer.  SEM  examination of this layer noted possible heat-affected  grain damage in the metal above the Pin 6 transistor.  The aluminum metallization was removed with  phosphoric acid.  Inspection next indicated that some  metal in the Pin 6 FET had etched, suggesting a possible  crack in the oxide.  SEM inspection at this site, shown in  Figure 12, confirmed evidence of thermal stress in the  oxide layer, exactly where predicted by MCI when  corrected for the ~7-micron misalignment.  The glass  was bubbled and deformed, indicating it had reached a  temperature sufficient to soften glass, approximately  1000C.  Two semicircular cracks suggested contraction  of the glass as it cooled and re-hardened.  Additional, smaller damage sites were also noted nearby.


This evidence confirmed the presence of a thermal defect  at the site predicted by MCI.  The non-adiabatic nature  of the damage indicated electrical overstress (EOS) as


the immediate cause of failure, although primary damage  by electrostatic discharge (ESD) could not be ruled out.


Figure 11:  No defects were seen during SEM inspection of  the Pin 6 input transistor at top glass.  A wide sheet of  metallization covers the transistor in this photo, leaving only  its topography visible.


Figure 12:  The Pin 6 input FET exhibited thermal damage to  the oxide layer above the transistor, indicating the glass had  reached a temperature sufficient to cause softening and  deformation, and likely indicating electrical overstress (EOS) was involved in the failure.


175


Figure 13:  An optical image of pin 10 showing transistor  metallization is seen above.  An arrow points to an anomaly, which appears to join the base of a transistor finger with the  polysilicon gates lying underneath, on both sides of the finger.


Inspection of the Pin 10 FET at the oxide found no  evidence of thermal stress at this level.  But careful  removal of the glass revealed a defect at the base of the  third finger in the transistor, at the location indicated by  MR magnetic current imaging.  Unfortunately a double  etch rendered further analysis of the microcircuit  impossible.  Nevertheless, optical inspection of the 24  input transistors on the Quad NAND gate, with a total of  96 fingers, had already shown that the third finger of the  Pin 10 input FET was unique—the only transistor finger  in the entire device with damage.  Its location, when  adjusted for the misalignment noted in Figure 10, closely  matched the defect site predicted in Figure 14 using MR  magnetic current imaging.


Figure 14.  A magnetic current map overlay of the  optical defect seen in Figure 13.  When adjusted for the  misalignment the predicted and actual defect sites match  closely.


In summary, the design and construction of this Quad  NAND gate resisted easy analysis.  Optical examination  could find no defects because both failure locations were  concealed under a wide sheet of metallization over the  transistors, leaving only their topography visible.  Because an aluminum sheet forms an excellent heat  spreader, liquid crystal analysis on this device would be  difficult or impossible.  Likewise, the aluminum sheet is  opaque to light emissions sensed by HgCdTe detectors, and to thermal emission by InSb detectors.


However, magnetic current imaging, using SQUID in  conjunction with a MR detector for the first time, was  able to isolate the failure to the die, then identify the  failure locations of two shorts on the die with an  accuracy of a few microns.


176


Figure 15.    An overlay of the optical and magnetic current images using MR shows current entering the Pin 10  transistor at right, and exiting through the Pin 6 transistor at left.  Instead of diffusing over the transistor fingers, highcurrent density defects are seen in each transistor.


[1] O. Crepel et al., Magnetic Current Imaging  Techniques: Comparative Case Studies.  In Proc. of the  30th Int'l Symp. on Testing and Failure Analysis, page  29-32, Worcester, MA, November 2004.


[2] J. P. Wisko, SQUID sensors: Fundamentals, Fabrication and Applications, Chapter The Magnetic  Inverse Problem for NDE, pages 629-695, Kluwer  Academic Publishers, The Netherlands, 1996.


[3] E. F. Fleet et al., HTS scanning Microscopy of  Active Circuits, IEEE Transactions on Applied  Superconductivity, 9 (2): 4103 (1999).


[4] L. A. Knauss et al., Detecting Power Shorts from  Front and Backside of IC Packages Using Scanning  SQUID Microscopy. In Proc. of the 25th Int'l Symp. on  Testing and Failure Analysis, page 11, Santa Clara, CA, November 1999.


[5] R. Dias et al., Integration of SQUID Microscopy into  FA Flow. In Proc. of the 27th Int'l Symp. on Testing and  Failure Analysis, Santa Clara, CA, November 2001.


[6] M. Pacheco et al., Scanning SQUID Microscopy for  New Package Technologies. .  In Proc. of the 30th Int'l  Symp. on Testing and Failure Analysis, page 29-32, Worcester, MA, November 2004.


[7] D. P. Vallet. Scanning SQUID Microscopy for Die  Level Fault Isolation. In Proc. of the 28th Int'l Symp. on   Testing and Failure Analysis, pages 391-396, Phoenix, AZ, November 2002.


[8] L. A. Knauss et al., Advances in Scanning SQUID  Microscopy for Die-Level and Package-Level Fault  Isolation. Microelectronics Reliability, 43:1657-1662 (2003).


[9] A. Orozco et al., Fault Isolation of High Resistance  Defects using Comparative Magnetic Field Imaging. In  Proc. of the 29th Int'l Symp. on Testing and Failure  Analysis, pages 9-13, Santa Clara, CA, November 2003. [10] L. A. Knauss et al., Current Imaging using  Magnetic Field Sensors. Microelectronics Failure  Analysis Desk  Reference 5th Ed., pages 303-311 (2004).


[11] B. D. Schrag, et al., Scanning Magnetoresistance  Microscopy for Die-Level Sub-Micron Current Density  Mapping. In Proc. of the 29th Int'l Symp. on Testing and  Failure Analysis, pages 2-5, Santa Clara, CA, November


2003.


177


Case studies of the use of Image Processing in Metrology and Failure Analysis.


Kartik Ramanujachar


Texas Instruments 12203 South West Freeway , Stafford, Texas , 77477


This paper describes the use of image processing techniques  in metrology and failure analysis through the discussion of  three case studies. The first two case studies are concerned  with images acquired with a scanning electron microscope. The last case study uses image data acquired with an atomic  force microscope. The first case study describes the use of    image processing techniques like edge detection that help to  automate the measurement of transistor critical dimension  from SEM micrographs. As is well known manual methods to  measure transistor CD are time consuming and also error  prone. We describe a technique that significantly automates  the process and hence enables both a rapid and accurate  extraction of   cumulative distribution function for transistor  CD. Measurements like transistor CD immediately raise  questions about the spatial resolution of the instrument ( in  our case SEM) on which the measurements were acquired . The second case study therefore addresses the question of  estimating the “on image” resolution of a SEM, independent  of the values quoted by an OEM specification sheet. We  utilize a cross correlation algorithm [1] and an appropriately  chosen sample and image  to estimate the “ on image” spatial  resolution of a SEM.  The final case study concerns atomic  force microscopy. As transistors are scaled into the deep  submicron scale AFM techniques are assuming a prominent  role in probing both memory and logic failures. Although the  typical AFM scan will only be a few microns on a side  occasionally large scans ( a few tens of  microns) are  acquired.
 We describe how information theoretic concepts  like entropy and mutual information combined with image  segmentation and nearest neighbor extraction can be used to  isolate those regions of the AFM scan that can potentially  benefit from further analysis.


Case Study 1


Automated Extraction of transistor CD from SEM  Micrographs.


The critical dimension of a transistor ( for our purposes the  transistor L) is an important parameter that dictates its  performance . It is also a significant process control


parameter. Frequently during the process development or  tuning it is required to measure this value from SEM  micrographs. Manual measurements are laborious, time  consuming and error prone.  We can significantly automate  the measurements and also improve their accuracy by  utilizing concepts from the image processing literature. In  particular edge detection can be used to extract image  intensity profiles that can be then be utilized to extract CD  measurements.


The technique that we have developed is the following. The  input image is a  well focused SEM image of the transistor  finger with the sidewall oxide/nitride removed. The latter  condition of side wall removal is not binding , but care must  be taken in delineating the measurement area if the side walls  are left in place. A typical input SEM image with multiple  transistor  fingers to be measured is shown in Fig 1.


Fig 1 Typical SEM micrograph used as input to the CD  estimation program.


The input image is convoluted with a Gaussian convolutional  kernel which in effect is a low pass filter and removes noise  from the image. The filtered image is then convoluted with a  Laplacian convolution kernel. The kernel takes the form of  the matrix [ -1 -1 -1 ; -1 8 -1 ; - 1 -1 -1]. The convolution  operation effectively replaces each pixel in the image with  eight times its value less the values of its immediate  neighbors. The net effect is to differentiate the image


178


# Case studies of the use of Image Processing in Metrology and Failure Analysis.


resulting in map of intensity gradients or delineation of the  edges. A number of other edge detection algorithms like the  Canny and Sobel filters may find applications in commercial  SEM software, but we chose the Log filter for its simplicity  and ease of implementation. The result of the application of  the Laplacian of a Guassian filter on the image in Fig 1 is  shown in  Fig 2. A line profile of intensity across the section  marked 1is displayed in Fig 3.


Fig 2  Edge detected image corresponding to the image in  Fig 1.


Fig 3.  Intensity Profile across region marked 1 in Fig 2. Zero crossing points are indicated by the two arrows.


Edge detection has resulted in an undershoot followed by an  overshoot of intensity about the nominal edges of the  transistor finger. The position of the true edge is the zero  crossing point marked at both ends with an arrow. An  algorithm has been developed to find the pixel positions of  the maxima (i.e the overshoot points) and the minima ( the  undershoot points) and estimate the zero crossing points. The


separation of the zero crossing points is the transistor CD. The pixel separation can be converted to a distance measure  with the help of a known distance which is typically a scale  bar that accompanies the SEM micrograph.  This process can  be repeated across the transistor width and statistics of   transistor length variation can be obtained.


Fig 4 shows the GUI interface of a program that has been  developed to implement the concepts described above.  It  allows the user to navigate to the image of interest, enter a  scale bar to calibrate distances and delineate those transistor  fingers across which we desire CD statistics. A cross- hair is  provided to mark the upper left, upper right and bottom right  of the region over which measurements are desired. The  output cumulative distribution function for all selected  regions is then computed and also saved for future reference. Fig 5 shows a typical distribution functions obtained. The  concepts and program described in the preceding section were  utilized to provide guidance to process engineers tuning gate  processes in the development phase of 90 nm technology.  The program was used to verify that poly CD variation was  not the root cause for single bit RAM failures in  microprocessor silicon. The program has also seen recent use  in the quantification of in die transistor CD variation in flash  memory.


Fig 4 Graphical user interface of program for automated  measurements of transistor CD.


179


Fig 5 Cumulative distribution function of transistor  critical dimension estimated for three chosen regions.


Case Study 2


Estimating spatial resolution of a SEM using crosscorrelation.


Transistor CD measurements invariably raise questions about  the spatial resolution of the instrument on which the  measurements were acquired. In this section we discuss the  use of a cross correlation algorithm [1] to estimate the spatial  resolution of a SEM image. While David Joy et al [1] discuss  a number of other techniques in their paper we have chosen  the straight cross correlation technique as it is easy to  implement.


In its essential form cross correlation in an image processing  context is a template matching tool. Given an image and a  template, cross correlation between the image and the  template would reveal those areas of the image where features  most closely resemble those in the template; in these locations  the cross correlation value would be a maximum. Consider  now an image which is very well focused such that its  features are sharply defined. If cross correlation is conducted  between a template and the image there would be little  uncertainty about the locations at which the image most  closely matched the template features, if at all. Conversely if  the image is not sharply focused and the cross correlation  carried out due to blurring of image features the uncertainty  about the locations of maximum matching would grow. This  uncertainty can be characterized with the full width at half  the maximum of a cross correlation function [1].  David Joy  et al proceed further and demonstrate how the full width at  half maximum of cross correlation peak can be used to  quantify spatial resolution. They consider an image that does  not exhibit any strong spatial dependence of intensity. They  demonstrate that two otherwise identical but slightly  displaced sections of the image would be correlated on the  same spatial scale as the inherent spatial resolution of the  image.


The concepts above can be demonstrated with the help of an  example.  The image chosen for analysis is an RIE etched  inter- metal dielectric show in Fig 6. As can be discerned


there is no significant spatial dependence of image intensity. Two image sections slightly displaced from one another are  chosen approximately in the center of the image. The first  image section chosen is shown by dotted lines on Fig 6. A  section of identical size displaced horizontally from this  section by 5 pixels constitutes the second section. The two  image sections are then cross correlated using a frequency  domain technique. It can be shown that the cross correlation  is obtained by the convolution of one image section and the  other image section   rotated by 90 degrees. In the frequency  domain this would be achieved simply by multiplying the  Fourier Transform of one image with the complex conjugate  of the Fourier Transform of the second image. The resulting  cross correlation function is shown in Fig 7.  A section  through the center of the cross correlation function is shown  in Fig 8. The full width at half maximum of this section is an  estimate of the spatial resolution. In the particular case  considered the value turns out to be 9.7 nm. The same  experiment can be conducted at varying values of the SEM   Kv to map the dependence of the spatial resolution on the  SEM accelerating voltage. Thus an “ on  image “ resolution  can be estimated independent of the specifications provided  by a manufacturer’s specification sheet.


Fig 6 SEM  image of etched IMD used for cross  correlation based estimation of spatial resolution.


Fig 7  Cross correlation function calculated by using two  sections in the center of  the image in Fig 5.


Fig 8 Section through the center of the cross correlation


function in Fig 7 . The full width at half maximum marked  by the arrows is the spatial resolution.


Case study 3:


Extracting regions of a current AFM scan that may  benefit from further analysis.


As transistors continue to be scaled aggressively into the deep  sub micron regime atomic force microscopy techniques are  being actively pursued to isolate both failures in memory and  logic of concurrent silicon. Several techniques including  scanning capacitance microscopy, current imaging and  spreading resistance find increasing use in the isolation of  transistor level defects.  The typical atomic force microscopy  scan is only a few microns on side, but occasionally scans can  span a few tens of microns on a side. In the case of these  larger scans, we need a way of isolating those regions of the  scan that are potential sites of anomalies or would benefit  from further analysis.


We begin by asking the question “Are there regions of the  image that are potentially more interesting than other regions ?” We can rephrase the same question in the following  manner “Do some regions of  the image contain more  information than other regions of the image?” When we  rephrase the interest attribute with the information attribute  we can utilize the whole body of information theory to help  guide us to an answer. Information theory provides two  concepts entropy and mutual information that we will put to  use in an image processing context.


Entropy is formally defined as -Σp log(p) where p is the  probability that a given pixel in the image will have an  intensity of a particular value. In practice the entropy is  computed by obtaining a histogram of image intensity which  helps us estimate the probability of a pixel acquiring a certain  intensity value. The mutual information contained by a region  of the image and its immediate surroundings can be shown to  have an upper bound that is the sum of  the entropies of   segments of the image in question. We can utilize these  concepts to isolate those regions of the image that have the  largest mutual information content. These regions can then be  subjected to more detailed  AFM investigation.


The method we adopt to implement the scheme outlined  above is as follows. The input image is segmented into its  constituent objects. Segmentation can be achieved in several  ways one of which is to use image intensity data sometimes  also called watershed segmentation [2]. Statistical  classification and clustering schemes  can also be used to  segment images. In our case the Matlab Image Processing  tool box built around the above mentioned methods was used  to segment an edge detected image.  The geometric centroid  and the extent ( span)  of the objects are then obtained. Fig 9  shows the input current AFM image that is then edge detected  and segmented into its constituent objects. Once the span of  each object in the segmented image is obtained, an entropy  value for each object  can be estimated. To estimate the  mutual information content of an object and its immediate  surroundings we need to establish the nearest neighbors of  any given object. We have solved this issue with a construct  that is called a Voronoi diagram. Formally the Voronoi  diagram is a construct that  collects together all points in a  collection of points  that are closer to any given point as  compared to other points. The Voronoi diagram of the  centroids of  the segmented image are shown in Fig 10. The  nearest neighbors of any given centroid are those whose  Voronoi polygons share a common edge with the Voronoi  polygon of the centroid of  interest.


With the nearest neighbors established and the entropy  content of each segmented object estimated we can compute  the mutual information content of any given region of the  image by summing the entropies of a segmented object and  all its immediate neighbors. Following this we can isolate  those regions of the image that have the highest mutual  information content. Fig 11 shows the result of the procedure


181


implemented  with the Matlab Image Processing ToolBox[2]. As can be discerned regions of low conductivity and possible  shorts in the AFM current image can be isolated. The  information theoretic technique we have outlined above  differs from alternative techniques of anomaly detection such  as those documented in [3].  In these cases alternative  probabilistic concepts like Bayesian inference methods and  novel intensity histogram schemes are used.


Fig 9  Current AFM image used as input to the Maximum  Entropy  program.


Fig 10 Voronoi Diagram showing the Voronoi cells of the  centroids of the segmented image.


In this contribution we have discussed three case studies of  the use of image processing in metrology and failure analysis. We demonstrated the use of edge detection and quantification  of image intensities to obtain probability distribution  functions for transistor CD. We examined the use of crosscorrelation to estimate the on image resolution of a SEM. Finally we explored the manner in which the concept of  entropy and mutual information can be utilized to isolate  regions of  current AFM scans that could benefit from further  analysis.


Fig 11 Results of the Maximum Entropy process. The  circled regions isolate those portions of the image with low  conductivity and the box identifies a region with potential  shorts.


I  would like to acknowledge Kendall Scott Wills who  directed the problem of CD extraction and automation to my  attention.


1. Metrics for resolution and performance for CD –SEMs   white paper by Joy David.C., Yeong.Uk.Ko.,Hwu.Justin.J  Oak Ridge National Laboratory OakRidge TN 37831


2. Matlab  Image Processing Tool-Box, from the Mathworks (2004)


3. "Finding Anomalies in an Arbitary Image"


Toshifumi Honda and Shree K. Nayar


Proc. of IEEE International Conference on Computer Vision,  Vancouver, Canada, July 2001.


182


Single Device Characterization by Nano-probing to  Identify Failure Root Cause


Chao-Chi Wu, Jon C. Lee, Jung-Hsiang Chuang, Tsung-Te Li,


Taiwan Semiconductor Manufacturing Company, Ltd.


6, Creation Rd. 2, Science-Based Industrial Park, Hsin -Chu, Taiwan 300, R. O. C. Tel: 886-3-5785112ext.2175 Fax: 886-3-5787778


ccwun~,tsmc.com, Clee~,tsmc.com, [hchuanq~,tsmc.com, ttli~,tsmc.com


In general failure analysis cases, a less invasive fault  isolation approach can be utilized to resolve a visual root  cause defect. In the case of nano technology, visual  defects are not readily resolved, due to an increase in  non-visible defects. The nor~visible defects result in a  lower success rate since conventional FA methods/tools


are not efficient in identifying the failure root cause. F or  the advanced na~ometer process, this phenomenon is  becoming more common; therefore the utilization of  advanced techniques are required to get more evidence  to resolve the failure mechanism. The use of na~oprobe  technology enables advanced device characterization h


order to obtain more clues to the possible failure  mechanism before utilizing the traditional physical  failure analysis techniques.


With the continued growth oft~e IC (Integrated Circuit) industry, (technology driving down to 90nm and below),


inspection and deprocessing tools have been developed  that are able to keep up with the advancing and  demanding imaging requirements [1]. However, the  fault isolation techniques for nanometer devices have not  been able to keep up wit~ the technology and failure  analysis on these nodes are become more challenging.


In earlier processes, WAT (Wafer Acceptance Test) parameters were good enough to monitor the behavior of  devices in chips; however for more complicated and  shrinking ULSI technology, this approach can't   accurately reflect the behavior of all devices contained


within the chip. A traditional device measurement  technique was to utilize a FIB to deposit metal lads and  then probe the pads using tungsten needles on a  micro-probe station. This methodology requires large  metal spacing and suffers from noise during device  measurements, and is becoming more difficult due to the


shrinking technology. Na~o-probing is an alternative  method that will overcome this predicament. Na~o-probing is capable of directly measuring the  behavior of source/drain junctions with a single probe, resistance measurement of two contacts with two probes, and full tza~sistor characterization with multiple probes.


With the obvious advantages of nano-probing, it is  important to note several disadvantages, such as contact  resistance, tip oxidation, sample preparation, and


test-timing issues affect the accuracy of probing result


[2]. In order to achieve low Rc on nanometer features, probe tips and the sample surface must keep clean and  free of oxides [3]. Excluding the issues noted above, the  probing results are reliable for electrical characterization  analysis.


Basic transistor parameters such as Vt, Ion-, I~at, and  junction behavior can be identified by means of I/V  curves measurements. This capability will help guide the  root cause failure analysis when comparing the  measured data with reference data.


PFA procedure


In this axticle, an embedded SRAM of an 110nm product  was malfunctioImg. Our first approach was to perform  emission microscopy in an effort to isolate the potential  failure area. The abnormal emission spots that are  different with reference are showing in Figure 1. After


mapping the emission spots to the layout, a PMOS  tza~sistor was identified as an area to focus the PFA  techniques. A top down analysis utilizing parallel  lapping and PVC techniques down to the contact level  failed to reveal any obvious abnormalities. Since no  visible defects were observed, additional  characterization is needed to better understand the cause  of the emitting PMOS tza~sistor.


183


# Single Device Characterization by Nano- probing to Identify Failure Root Cause


.1=


M•a•ure •


Clicktho 1• Point


i l l  ~llCK 1 + 1 5 ~ 9 3 - 8 9  i + 7 6 9 4 ¸ 0 2  h bl~tance I


Figure 1. Using EA4MI to isolate abnormal positions. Layout shows the EA4MI spots locate on PJ~IOS area.


Device Characterization


A wafer probing system wifla flaree micrommfipulators (Klocke Nanotechnik) was used in flae measurements, which was installed into a Hitachi FE-SEM S-4800. Utilizing this nano-probing technique, we cma measure


flae device characteristics at flae contact level (Figure 2). After comparing the I/V curves of flae emitting PMOS  transistor with a reference PMOS trmasistor, an abnormal  electrical characteristic cma be observed on the emitting  txmasistor (See Figure 2). The I/V curve of bad transistor  shows a lower Is~t mad higher Ion- current. In order to  understand the leakage pafla, flae current components of  Source, Drain, Gate, and Well/substmte node shall be  checked (See Table 1). Analysis of flae electrical results  indicates flae leakage pafla of flae emitting transistor is  between drain and substmte.


In order to furdaer validate flae electrical measurements, a PMOS txmasistor on flae periphery was also used for  confirmation. After comparing its result wifla a  reference, flae behavior was flae same. So flae difference  of PMOS found is reliable, it should be someflaing  abnormal to cause drain to substmte leak.


I'0E--03


1.0E-04


i u E


I 1 .0E-08


~


-1.5


vg(v)


Fail die


(Vd=-0.1V)


--~-- Fail die


(Vd=-1.0V)


Good die (Vd=-0.1V)


Good die (Vd=-I lO~


Figure 2 Device behavior is different between the P3/IOS  transistors o f  bad and good dice. The device o f  bad die  has higher loft.


Current flow Id (uA) Ig (uA) Is (uA) Ib (uA) Bad Ioff -6.81 6.08E-5


1.83


4.99


die Isat -113.66 -0.00523 106.45


7.06


Good Ioff -1.27 2.04E-5


1.11


0.164


die Isat -155.04 -0.00734 155.07


0.197


Tablel. It shows the current value o f  source, drain, gate, and well/substrate. Strong signals labeled with red  indicate leakage existed between drain and substrate.


Result


The conductive-AFM (C-AFM) has already been widely  used in FA cases and has become a standard FA tool to  identify failure location and help for realizing the failure  mechanism by current map and I/V curve [4]. As  mentioned above, the emitting PMOS transistor was  caused by a junction leakage issue. To further confirm  the results obtained using nano-probe technique, C-AFM  technique was used. A current map of the area was  obtained using a CAFM (shown in Figure 3) In the  current mapping image (positive bias from substmte to  tip), the N+ contact area is chosen to display a bright  color, however the P+ contact area shows the same color


as the N+ contact. This behavior indicated there was a  leakage path between P+ contact and substmte. Checking flae I/V curves of the different contacts to  substxate (Figure 3), the behavior of P+/N-well (blue  curve) seems like that of P-well pick up (yellow curve), not a normal P+/N-well (pink curve). This phenomenon  is meaningful, and it indicates the leakage is most likely


caused by a well issue.


To prove this theory, PFA evidence for N-well implant  was needed. Fgure.4 shows the plane view junction  stain and x-section SCM (Scanning Capacitance  Microscope) images. In plane view junction stain image,


there is no difference of contrast between N-well and  P-well, so the theory of a missed N-well implant issue  seems more probable. In the SCM x-section image, the  N type implant signals will be set on bright colors. However, in the N-well implant area, the signals axe not  clear. This result indicates no N-well implant is indeed


184


the root cause. After verifying all of the N-well implmats  steps, the mask issue of N-well implmat is identified.


O.OE.O0


_ io _1.o


-2.5[*04 II


Volt


Drain to sub (fai l)


Drain to sub (normal)


PW pick up


Figure 3 The P-well of  current mapping image should be  dark. The I/V of abnormal drain to substrate seems like  P-well pick up behavior.


due to the problem of  N-well miss implant. A SCJEI  x-section image indicates no N-well implant indeed.


Generally, nmao-probing system is a powerful tool for  electrical mmlysis; it can be used to characterize junction


behavior, short/resistance mad txmasistor/diode  measurements. For device behavior checking, the basic  parameters, such as Vt, Ion, and Is~t can be measured  easily, and the current flow to source, drain, gate, mad  well/substmte should also be identified to realize the  leakage path.


Because WAT parameters can't accurately reflect real  device behavior in circuit, the nmao-probing  measurements on suspected txmasistors are needed. It cma  obtain more electrical data to provide more hints, mad  saving more time to identify the root cause for the FA of


130nm technology and below.


Reference


[1] D. P. Vallet, '~robing the Future of Failure  Analysis", ASM International, 2001, Volume 4  Number4, 5-9.


[2] C. A. Waggoner, D. Smith, '~)btaining Low


Contact Resistance For Physical Sub-micron  Fault Isolation", ISTFA 2003.


[3] D. Faure, C.A. Waggoner, "A New Sub-micron  Probing Technique for Failure Analysis in  Integrated Circuits", ESREF 2002.


[4] Jon C. Lee, J. H. Chumag, "Fault Localization in  Contact Level by Using Conductive AFM", ISTFA, 2003.


Figure 4. Junction stain shows there is no difference of   contrast between N-well and P-well, which should be


185


n2


n1


p2


Jleak


p1


Analysis of DRAM Standby Current Failure due to Hot Electron Induced Punchthrough (HEIP) of PMOS transistor


M. H. Cho, Y. I. Kim, J. Choi, D. S. Woo, K. P. Lee, Y. J. Park, W. S. Lee, and B. I. Ryu


Technology Development Team 1, Memory Division, Device Solution Network, Samsung Electronics. Co. San #16 Banwol-Ri. Taean-Eup, Hwasung-City, Gyeonggi-Do, 445-701, South Korea


Tel: 82-31-208-2721; fax: 82-31-208-2769; e-mail: cmh12.cho@samsung.com


A standby current failure of the 80nm design-ruled Dynamic  Random Access Memory (DRAM) during burn-in stress was  investigated. In our case, hot electron induced punch-through (HEIP) of a PMOS transistor was a leakage current source. The bake test is a useful method to identify the mechanism of a  standby current failure due to hot carrier degradation.


According to the strong demand of reducing chip size, it is  difficult to fabricate DRAM with high performance and  stability. The standby current failure is the one of major  problems in DRAM. The standby currents of the test samples  after step stress burn-in test are shown in Fig. 1.


Fig. 1 The results of step stress burn-in test of 80nm designruled DRAM. Trench oxide thickness: 59Å, gate tab: 70nm.


As the burn-in voltage is increased, the standby current is  increased. In order to identify the location of the leakage  current source, a degraded sample is investigated with  PHEMOS. The PHEMOS image and the schematic diagram of  the fail position are shown in Fig.2. The leak position is a  PMOS transistor in the output driver of a level shifter circuit. The leakage current of the PMOS transistor can be induced by  the hot carrier induced (HCI) on-state current decrease of the  NMOS n1[1] ,by gate oxide breakdown of the PMOS transistor  in the output driver, or by hot electron induced punch-through (HEIP) of the PMOS transistor itself. The HEIP of the PMOS


Fig. 2 A schematic circuit diagram and a PHEMOS image of  a degraded CMOS level shifter. Fail position is an output  driver of the level shifter.


transistor can be induced as silicon nitride liner layer is  adapted to shallow trench isolation (STI). The interface  between the trench oxide and the liner silicon nitride layer acts  as the trap site of the hot electron, which induces punchthrough of PMOS transistor. [2] In this work, we clarify the  main cause of the PMOS transistor leakage with bake test.


To identify the main cause, the degraded samples were baked  for 1hr. The bake temperature was varied from 125oC to  300oC. It is known that the leakage current due to the oxide  breakdown cannot be recovered by thermal treatment. The  decrease in HCI on-state current of NMOS transistor has been  reported to be recovered by annealing at 125oC.[1] In the case  of the HEIP of PMOS, however,  the degradation is expected  to be recovered by annealing at higher temperature than  125oC, because it is induced by  the thicker trench oxide than  the gate oxide. Greater thermal energy will be required to  release trapped electrons from thicker oxide. The variation of  standby current values of the degrade samples before and after  thermal treatment are shown in Fig. 3. The degraded standby  current is not recovered after 125oC bake, which implies that  the mechanism of the standby current failure is not HCI onstate current decrease of NMOS. By the way, the degraded  standby current is recovered by about 20% and 90% after  240oC and 300oC bake, respectively. The recovery of the  degraded standby current implies that the degradation is not  due to PMOS gate oxide breakdown. The fact is supported by  the visual inspection that the degraded samples had no  physical damage. Thus, it can be concluded that the  degradation of the standby current is attributed to the HEIP of  the PMOS transistor in the output driver. As shown in Fig. 4, a


BI condition: Dynamic, @R.T, n=30


Burn-In Voltage (Arb. Unit)


186


# Analysis of DRAM Standby Current Failure due to Hot Electron Induced Punch-through ( HEIP) of PMOS transistor


recovery temperature of a hot carrier degraded PMOS is about  350 oC, which is higher than that of a NMOS by about 200 oC.


Fig. 3 Standby current after burn-in stress and bake. Bake at  125oC has no effect on standby current of degraded samples. Most of the degraded standby currents are recovered after  bake above 300oC.


Fig. 4  NMOS on-current and PMOS BV with hot carrier  stress and following bake anneal.


The schematic diagram of the mechanism of the HEIP of a  PMOS transistor is shown in Fig. 5. The trapped hot electron  at the interface between the trench oxide and the liner silicon  nitride layer gathers positive charges, leading to the channel  length shortening of the PMOS transistor. As the higher  electric field is applied at the drain of the PMOS transistor, the  more hot electrons are trapped at the interface. Thus, the HEIP  of the PMOS transistor can be improved by increasing trench  oxide thickness and increasing the channel length of the  PMOS transistor only at the trench edge; tapping gate as  shown in Fig. 5.


Fig.5  Schematics showing the mechanism of the HEIP of a  PMOS transistor.  a) cross-sectional view at the drain edge  and b) top view of a PMOS transistor. Increasing trench oxide  thickness reduces the electric field of the trapped hot  electrons, leading to improved HEIP characteristics. A gate  tap in b) increases the channel length at the trench edge, compensating the effective channel length shortening due to  trapped hot electrons


Fig. 6 HEIP characteristics of PMOS transistor with size of  gate tap. The trench oxide thickness is a) 59Å and b) 68Å


Recovery


Gate


Liner Trench ox.


Drain


Gate tap


: positive charge build-up : trapped hot electron


Source


effective


channel


shortening


Sample #


after BI


125oC bake  240oC bake  300oC bake


a) Trench Ox. 59A


Stress Time (sec)


gate tap 120nm  gate tap 110nm  gate tap  90nm  gate tap  70nm


b) Trench Ox. 68A


187


Fig. 7 The results of step stress burn-in test of 80nm designruled DRAM. Trench oxide thickness: 68, gate tab: 120nm.


Figure 6 shows HEIP characteristics of the PMOS transistor  with trench oxide thickness and gate tap size. The degradation  of PMOS transistor breakdown voltage (BV) is improved as  trench oxide thickness is increased or the size of the tapping  gate is increased. In Fig. 7, the results of the step stress burn-in  test with the samples are demonstrated. In the samples, the  HEIP of the PMOS transistor is improved by increasing trench  oxide thickness and size of the gate tap. The Standby current  failure is remarkably improved.


As the burn-in voltage is increased, the standby current, in  PMOS transistor in the output driver of a level shifter circuit, is increased. The leakage current of the PMOS transistor can  be induced by 3 causes. Those are HCI on-state current  decrease of the NMOS, gate oxide breakdown of the PMOS  transistor in the output driver, and HEIP of the PMOS  transistor itself. The recovery of the degraded standby current  above 300oC implies that degradation of the standby current is  attributed to the HEIP of the PMOS transistor in the output  driver. The HEIP of the PMOS transistor is improved by  increasing trench oxide thickness and size of the gate tap. The  bake test plays an important role in identifying the failure  mechanism of the standby current failure.


The authors appreciate to whom related to this work at  SAMSUNG ELECTRONICS MEMORY DIVISIONS.


[1] K. J. Lee et al., International Integrated reliability  workshop, 2004, pp173-174   .


[2] A. Hamada et al., IEEE Trans. ED., Vol. 38, No. 4, April, 1991, p895


BI condition: Dynamic, @R.T, n=50


188


Stacked-Die Analysis Using C-Mode Scanning Acoustic Microscope


Li Na, Jawed Khan, and Lonnie Adams


National Semiconductor Corporation, Santa Clara, CA USA  li.na@nsc.com,(408)721-4072


C-Mode Scanning Acoustic Microscopy (CSAM) has been  used as a nondestructive technique to detect electronic  package delaminations, die cracks, or mold compound voids. The analysis is usually performed by combining a throughscan with an interface-scan technique to determine the  existence and location of the delamination. In the past few  years, there is a significant demand for stacked-die  technology. The stacked-die device is mainly used in portable  consumer products. This kind of silicon integration  technology provides flexibility in space reduction, weight  saving and excellent electrical functionality. However, a  thinner thickness in the stacked-die package could complicate  CSAM analysis and sometimes may lead to false  interpretations. This is because thinner thickness has smaller  spacing between the adjacent interface, and shorter delay  times for ultrasound traveling from one interface to another. Therefore, the delamination between the die and die-attach  may not be easily detected by the traditional method and false  readings may even be expected. The first objective of this  paper is to briefly explain the CSAM mechanism. Based on  that, some of the drawbacks of current settings in detecting the  delamination for stacked-die packages will be displayed. The  last objective is to introduce Quantitative B-Scan Analysis  Mode (Q-BAM) and Zip-Slice technologies in order to better  understand and improve the reliability of detecting the  delamination in stacked-die packages. Therefore, a large  portion of this paper will focus on the Q-BAM and Zip-Slice  data acquisition and image interpretation.


Methods and Analysis


Mechanism of CSAM


1. The CSAM analysis combines through-scan mode with  reflection mode: In a regular nondestructive C-SAM analysis  on an electronic package, a through-scan is performed to  determine the existence of delaminations inside the package, followed by an interface-scan. In the through-scan mode, an  ultrasound is sent to the sample by a transducer on top of the  sample and an echo is received by a transducer at the bottom  of the sample. If there is a delamination anywhere inside the  package, the sound will reflect back, and the through-scan  image appears dark. Since the through-scan image is the  signal integration through the entire package thickness, one


may not be able to identify which interface the delamination  occurs by through-scan only. The interface-scan, on the other  hand, is used to isolate the delamination interface by focusing  and gating at a specific interface. The delamination is  determined by reading the echo polarity combined with  interface image, as shown in Fig. 1. Polarity and intensity of  the reflected waves depend upon the mismatch of the  acoustics impedance encountered at each interface. Therefore, a mathematically derived coefficient provides useful  information about ultrasonic wave reflection at an interface. The reflection coefficient R is defined as:


R=(Z2-Z1)/(Z2+Z1)


Equation 1


Where the Z1 and Z2 are the impedance of the two materials  on either side of interface. The impedances of most common  used material are listed in Table 1. Positive polarity reflection  coefficient implies the reflection wave does not experience a  polarity shift with respect to the incident wave. A negative  polarity means that a polarity shift has occurred.


Table1. The Acoustic Impedance of Common Materials,


[1][2].


Materials


Acoustic Impedance


Water


1.48


Mold compound


-6.76


20.04


41.83


Epoxy Resin


-3.12


2. Polarity may not always be useful information for image  interpretation: The most often misinterpretation is that positive  polarity shows no-delamination at the interface. In fact, the  sign of the echo may not be useful for image interpretation  depending upon the investigated interface. If the acoustic  impedance increases at the interface, for instance, from epoxy  resin to a silicon, the reflected echo of a positive incident  pulse will also be positive according to equation 1. At the  delamination site, the impedance decreases and the reflected  amplitude is negative. Therefore the echoes from area of  adhesion and delamination are positive and negative  respectively, whereas a decrease of impedance at the interface, results in a negative echo regardless of whether or not there is


189


# Stacked-Die Analysis Using C-Mode Scanning Acoustic Microscope


delamination. In this case, however, in order to understand the  polarity and to interpret the data correctly, one should be  aware of the impedance of the material on both sides of the  interface.


3. The reflection echo is a key for interface-scan: In interfacescan, the echo is received by the same transducer and  amplified. The time-of-flight into the specimen and back to  the transducer depends on the depth of the reflection interface. Hence the echoes from different interfaces are separated in  time. A certain interface is selected by gating the echo  electronically. The amplitude of the echo inside the gate the  with highest absolute value will determine the brightness or  color in the image. The intensity coefficient of the reflection  wave, I is defined as:  I={(Z2-Z1)/(Z2+Z1)}2 . I indicates the  fraction of incident energy that is reflected at the interface. Therefore, the larger the difference of Z2 and Z1, the smaller  the I.


Figure 1: A single-die electronic package (A) and its  corresponding pulse-echo waveform (B). In single-die  packages, an individual peak from each interface echo can be  easily identified. (1) is the front surface echo (water/molding  compound); (2) is first interface echo (die/molding  compound); (3) is the echo from interface between die/dieattach; (4) is the echo from the interface of die-attach/paddle, and so on.  In the stack-die package, the waveform from the  interface and subsurface are superimposed and sometimes  undistinguishable due to the tighter delay time.


Dilemma of CSAM for Stacked-Die


Figures 2A and 2B are interface and through-scan images for  a stacked die package. In Fig. 2B, it is obvious that the


delamination (dark area) appears somewhere inside the  package. Since the larger area of delamination occurs, the  ultrasound won’t be able to travel through the air and is  blocked by the delamination. No signal was observed, and the  though-scan image appears dark (color map #2). The  delamination interface is un-identified by through-scan alone. In single-die packages, one can identify the interface of  interest, then gate that interface and focus by maximizing that  interface echo. However, in stacked-die package, the interface  spacing is small and more interfaces are involved. The echoes  are not always differentiable, as shown in Fig. 3. This may  cause gating and focusing at specific interfaces to become  difficult. In Fig. 2A, the delaminations at the top-side of the  paddle and part of the lead frame are easily observed (color  map #24), but it is unlikely to focus on the top-die/die-attach  interface due to superimposed waveforms from all interfaces. Data may be mis-read if the echo is not able to be  maximized.


Figure 2: An interface-scan (A) (color map #24) and throughscan image (B) (color map #2) are displayed. The top-side  paddle delamination is observed; the top-side-lead frame is  partially delaminated as well. The image was obtained using  30MHz, 0.5 focal length transducer.


Leadframe


delamination


Die Paddle  delamination


Delamination Appears Dark.


190


Figure 3: Pulse-echo waveform from a stacked-die electronic  package. In stacked-die package, individual peak from each  interface echo are superimposed and individual echo is not  distinguishable.


Q-BAM


The Q-BAM displays a nondestructive cross section through  the line(s) defined on the interface scan portion of the image. The cross section shows the location and extent of the features  within the sample. The side scales provide the depth  information. Figure 4 gives the Q-BAM image of the same  sample as in Fig. 2. Figure 4A shows the cross-section where  cut at the larger (bottom)-die. The top half image shows the  cross section view of this location (the black line is where the  cut). From this image, one can see that the bottom-die top  surface looks good, but the interface between bottom-die and  die-attach is slightly delaminated. The lead frame at left hand  side is also delaminated, as indicated in Fig. 4. The right side  of the lead frame where the cut was performed has good  bonding. Figure 4B shows the cross-section where cut at the  smaller die. The bottom half of the image shows the cross  section view of this location. The delaminations at three  places are found: 1. top-die/die-attach. 2. bottom-die/dieattach, and 3. lead frame. It is interesting to see that the  bottom-die/die-attach interface delamination is only around  the outside of the smaller-die-attach area (compare to crosssection in Fig. 4A). There is no evidence of delamination at  the interface of the bottom-die/die-attach around the smallerdie area. This may be due to the fact that mounting smaller die  presses the center of the bottom-die further down, which  results in good bonding. This effect can be seen in the Fig. 4B. It indicates that the interface of the bottom-die/die-attach is  not completely delaminated and the area (under smaller-die) is  well attached. This will be further discussed and proved in the  next section, Zip-Slice.


Figure 4: The Q-BAM of the LLP package. In Fig. 4A, the cut  is at bottom-die and delamination at bottom-die/die-attach  interface is observed. The delaminations at the lead frame and  die-paddle are observed as well. It appears that the  delamination at top-die/die-attach is more severe. There is no  evidence of bottom-die/die-attach delamination around the  center area. The scan setting for this example is 33 nsec/div at  9843 ft/sec.


Zip-Slice and Three-Dimension Analysis


Zip-Slice 3D analysis acoustically “slices” the sample into as  many horizontal sections as one desires. The part is divided  into equal thicknesses. The Zip-Slice of the same sample is  shown in Fig. 5. In this example, the sample is sliced 30 times. The five most representative images are displayed in Fig. 5.  In Fig. 5A, the die-attach at bottom-die shows some  delaminations, but not in the center of smaller-die area. This  agrees with the observation from Q-BAM. In Fig. 5B, a severe  delamination is observed around the die-paddle and extended  die-attach delamination. In Fig. 5C, the top side of the bottomdie has good bonding and the lead frame has delamination at  three sides. Figure 5D shows that the smaller-die/die-attach  delamination at this location is severe. A good bonding of the  top-side of the smaller-die with molding compound is shown  in Fig. 5E. This agrees with the interface scan image (Fig. 2A).


die-paddle


2, 3, 4, etc


top-die  top-die/die-attach bottom die  die-paddle


leadframe


191


Figures 5 A-E: The Zip-Slice images displayed as individual  slices. The details are explained in the text. Note: 1. since the  cut is divided into equal thickness, the image from each slice  was not obtained at optimized focusing, 2. the data was  obtained with real sample, not from simulation. The color  map is designated by the author, 3. The five slices displayed  here were taken out of thirty slices, they are not necessary in  series, and are shown only for the demonstration purpose.


Figures 6 A and B: Assembled solid of the sample. The two  solids are cutout at different locations. In (A) the smaller die  shows good bonding (red) with the  molding compound. The  die attach under shows delamination (blue). The paddle is  delaminated (blue color.; In(B) the bigger die has a good  bond, but the die-attach is delaminated. Note: In order to get  a better view of the cross-section, the image is magnified five  times in the Z-direction.


Die Surface


Disbond Die Attach


Paddle disbond


192


It is worthy to note that the color scheme in Zip-slice is  different from those in interface scan and Q-BAM, and should  not be confused.


The assembling of the slices is shown in Fig. 6. Figure 6 gives  a three dimensional view of device. In order to get better view  of the interfaces in Z direction, the thickness of the device has  been purposely enlarged.


For stacked die package delamination inspection using Cmode acoustic microscope, traditional interface and through  scan techniques can not give enough of information when the  delamination occurs in multi-interfaces, and echoes from  adjacent interfaces are not sufficiently separated from each  other, as demonstrated in this paper. It is recommended that  different CSAM modes be applied in order to identify the  delamination interface(s) and avoid misreading and misinterpreting the information.


Note:


Please contact the author if an original color figure is needed.


[1]  Siettman, R. Dias, and K. Fiebelkorn, “Acoustic


Evaluation of Electronic Plastic Packages”, IEEE/IRPS


(1992), pp. 309-314.


[2]  Sonoscan’s Acoustic Micro Imaging Users’ Workshop,


May 5-7, 2004, Santa Clara, CA.


193


Randal Mulder; Product Analysis Engineer; Freescale Semiconductor, Inc.; 6501 William Cannon Drive, Austin, TX 78735; Ph:512-895-6572; Fax:512-895-3827; Email:R.Mulder@freescale.com


DuPont EKC265TM as a Copper Metal Etchant to Assist FIB Edits through Large  Copper Power Supply Lines


Randal Mulder


Freescale Semiconductor, Inc.; 6501 William Cannon Drive, Austin, TX 78735


At the 2004 ISTFA Symposium, this author presented a paper  on the use of EKC265TM as an etchant for the removal of


copper metallization for the planar deprocessing of  semiconductor devices with copper metallization [1]. A


participant at the symposium asked if EKC265TM could be used


to remove the copper metallization when using the focused ion  beam tool (FIB) to cut large windows through large copper  power supply lines to perform FIB edits on the lower metal  layers. Having never used EKC265TM for that purpose, this


author could not answer the question with certainty. Therefore, this paper is a follow-up to answer that question.


State of the art semiconductor technologies use multiple copper  metallization layers to route power and signals throughout the  semiconductor device.  These devices typically have a  minimum of four to six metal layers with the top one or two


layers predominately used to route the large power supply lines.  The density of the metal lines in the upper layers usually  obscure the signal lines that run at the lower metal layers (metal  layers 1-3) from view (Figure 1). Non-functioning devices


often require the use of a FIB to construct probe pads to the  signal lines at the lower metal layers for fault isolation or FIB


edits may be needed at the lower metal layers to verify design


fixes.


Figure 1: Optical image of a five metal layer, 0.12um copper  metallization technology device. The lower metal layers are  completely covered by the upper metallization layers.


To gain access to these lower signal lines, the FIB must be  used to cut large windows through the large power supply  lines. The problem is that cutting large windows through the  copper metallization is very difficult [2]. The copper in the  metal lines have pronounced grain boundaries (Figure 2) that  mill at different rates when exposed to an ion beam. The result  is a very uneven milling that causes holes to form or leaves  debris at the bottom of the FIB window. This makes isolating  or the prevention of damage to the lower metal layers nearly  impossible.


Figure 2: FIB ion beam image of expose copper metallization. The pronounced grain boundaries of the copper can be easily  seen.


This paper will demonstrate how EKC265TM can be used as a


copper metal etch to remove the copper of the power supply  lines. This allows the FIB to cut large windows through the  material layers to gain access to the lower metal layers for


probing or FIB edits. Results will be shown for FIB work using  EKC265TM and for FIB work without the using EKC265TM .


Methods and Results


Figure 3 is an SEM image of a large power supply line of a five  metal layer copper metallization semiconductor device. A  8x8um window has been cut through the passivation exposing  the underlying Metal 5. The metal layer is ~2500 angstroms  thick. To remove the metallization and continue the FIB  milling, the device was placed in EKC265TM at 75 degrees C


194


# DuPont EKC265TM as a Copper Metal Etchant to Assist FIB Edits through Large Copper Power Supply Lines


Figure 3: SEM image showing a power supply metal bus line (Metal 5) where an 8x8um window has been cut through the  passivation exposing the copper.


Figure 4: Copper (Cu) etch rate vs temperature for EKC265TM


[ 1].


Figure 5: SEM image showing power supply line (Metal 5)


after removal of the copper with EKC265TM. The underlying


barrier metal is now exposed.


for 30 seconds (Figure 4) removing the copper metallization  and exposing the underlying TaN barrier metal (Figure 5).


After the copper metallization was removed, the FIB was again  used to cut a smaller window through the barrier metal and the  underlying layer of inter-level dielectric (ILD) exposing Metal


4 (Figure 6). After exposing Metal 4, the device was again  placed in EKC265TM at 75 degrees C for 30 seconds to remove  the copper metallization and expose the barrier metal (Figure  7). A smaller FIB window (2x4um) was set up and the barrier  metal of Metal 4 and the lower ILD layer was milled away  exposing the signal lines at Metal 3 (Figure 8).


Figure 6: SEM image showing the power supply metal lines (Metal 5 and 4). A  2x6um window has been cut through the  barrier metal of Metal 5 and ILD layer exposing the copper at  the Metal 4 layer.


Figure 7: SEM image showing power supply lines (Metal 5


and 4) after removal of the copper with EKC265TM. The


underlying barrier metal of Metal 4 is now exposed.


195


Figure 8: SEM image showing the power supply metal lines


Metal 5 and 4 and the signal lines at Metal 3. A 2x4um


window was cut through the barrier metal of Metal 4 and


lower ILD layer exposing the copper at the Metal 3 layer.


After milling and etching through two power supply lines, the  results are very uniform (Figure 9). At this point, a FIB edit  could be performed on the exposed signal lines or the signals  lines could be probed. The device is completely functional  since windows cut through the power supply lines did not cut  the width of the lines leaving a path for current conduction. Also, the sides of the power supply lines have not been etched  away by the EKC265TM (Figure 10).  EKC265TM is very


viscous so it does not readily etch laterally giving a fairly good  anisotropic etch result which is unusual for a wet etch. What  lateral etching does occur is minimal (Figures 11). It’s obvious  from these results that several more layers of copper could be  etched away without any adverse effects on the functionality of  the device. These results will now be compared to results for a  device where EKC265TM was not used to remove the copper  and the FIB was used to remove all material layers.


Figure 9: SEM image looking down into the FIB window. The  FIB milling is very uniform and the Metal 3 signal lines are


fully exposed. FIB editing or probing can easily be performed  and the device remains functional.


Figure 10: SEM image of the device cross sectioned through


the center of the FIB window. This shows that the EKC265TM


did not etch away the remaining power line metallization at


Metal 5 and Metal 4 resulting in no loss of functionality of the  device.


Figure 11: Close-up SEM image showing that very little  lateral etching occurred on the Metal 5 layer even though  Metal 5 was exposed twice to EKC265TM.  Several more layers


of metallization could have been removed and the Metal 5  layer would have remained intact.


Figure 12 is an SEM image of a second device. Again, an  8x8um window was cut through the passivation with the FIB  exposing Metal 5. This time, EKC265TM was not used to


remove the copper metallization. Instead, a 2x6um FIB window  was cut through the copper and the barrier metal exposing the  underlying ILD layer. At this point, it can be clearly seen that  the results of milling through copper are not uniform. The  copper at the center bottom of the FIB window was slower  milling rate then the other areas resulting in a hole in the ILD  on the left side and a raised area in the middle.


FIB milling of the window was continued until Metal 4 was


exposed. Again, EKC265TM was not used to remove the copper


196


Figure 12: SEM image of the second device. The FIB was used  to mill an 8x8um through the passivation exposing Metal 5. The FIB was then used to cut a 2x6um window through the  copper metallization. The results are very non-uniform.


metallization and the FIB milling was continued until Metal 4  and the barrier metal were removed (Figure13). It can be  clearly seen that the non-uniform milling of Metal 5 has  propagated down through Metal 4. There is a small amount of  Metal 4 remaining at the center of the window while Metal 3 is  almost exposed on the left hand side of the window. The FIB  milling of was continued until most of Metal 3 was exposed. At  this point, there is still an area of dielectric remaining over th


Metal 3 at the center of the window due to the non-uniform  results of milling through the Metal 5 and Metal 4 copper  layers (Figure 14).  To clear away this dielectric, additional FIB  milling was performed. However, this resulted in damage to the  exposed Metal 3 signal lines (Figure 15). It is now doubtful if  this device is functional and any useful information can be  gained from it.


Figure 13: SEM image of the second device after the FIB was  used to continue milling the 2x6um window through Metal 4. The non-uniform results of milling through Metal 5 are


continued and exacerbated by the milling through Metal 4.


Figure 14: SEM image of the second device after the FIB was  used to mill away the remaining Metal 4 and underlying ILD


exposing most of Metal 3. There’s still an area of dielectric


remaining over Metal 3 that needs to be cleared off.


Figure 15: SEM image of the second device after the FIB was  used to remove the last of the dielectric over Metal 3. Removing all of the dielectric resulted in damage to the Metal  3 signal lines. It is now doubtful that the device has remained  functional.


This paper demonstrated how EKC265TM can be used to assist  FIB work on copper metallization technology semiconductor  devices. EKC265TM eliminates the need to use the FIB to  remove copper giving a much more uniform milling result.  This gives easy access to the signal lines of the lower metal  layers without jeopardizing the functionality of the device.


The use of EKC265TM does require extra time. The sample has  to be un-load from the FIB, etched with the EKC, and re-load  in the tool for every layer of metallization removed. However, it’s was found that this time is usually more then made up  when compared to dealing with the difficulties of milling  copper with the FIB alone as demonstrated in this paper. The


197


better results using EKC265TM also means a higher FIB edit


success rate which helps offsets the extra time need.


FIB tool vendors are now adding special gases to aid in the  milling of copper to provide a more uniform result. Having no


experience with these gases, this author can not comment on  their effectiveness when compared to using EKC265TM.


EKC265TM has the advantage that it can be used with older  tools without the expensive upgrade to install new gases. The  use of etchant gases in a FIB tools can also be problematic. Residual gas can sometimes remain in the tool after completion  of a sample and possibly damage a following sample when the  gas was not intended to be used.


[1] Randy Mulder, “DuPont EKC265TM PERR as a Copper


Metallization Etchant for the Physical Deprocessing of


Failing 0.12um Technology Devices,” ISTFA Proceedings


(2004).


[2] M. Abramo, “The impact of Feature Packing Density on


FIB Editing of Advanced Technology ICs,” ISTFA


Proceedings (2003).


[3] Kenneth Krieg, Douglas Thomson, Greg Bridges,


“Multiple Probe Deep Sub-micron Electrical


Measurements Using Leading Edge Micro-machined


Scanning Probes,” ISTFA Proceedings (2001).


198


Edge Enhancement for Acoustic Microscopy of Flip Chip Devices


Dr. Daniel J. D. Sullivan, Dr. Andrew J. Komrowski, Luis A. Curiel, Kevan V. Tan


LSI Logic, 3098 West Warren Ave., Fremont, CA 94538  dsulliva@lsil.com


Scanning Acoustic Microscopy (SAM) is a non-destructive


tool for analysis of packaged devices [1], [2]. SAM uses ultrasonic waves to probe samples for the detection of voids and  delamination in packaged microelectronics. Of specific  interest in flip chip parts are the interfaces between the die and  the underfill, and the underfill and the package.


New materials, package configurations, and technologies have  required adaptation of standard practices in SAM [3], [4]. The  detection of cracked die, voids or delamination in the underfill  or package are standard issues for SAM. SAM can routinely  detect large cracks through the central 80% of the die as  shown in Fig. 1., however the occurrence of smaller cracks at  the edge of the flip chip die is problematic.


Figure 1: Die crack in wire bond part detected with AMI.


The sawing and assembly operations may induce small cracks  at the die edge [5], [6]. These cracks do not cause yield loss or  reliability issues under normal circumstances since they are  located in the street section, which contains no live circuitry. If, however, the initially induced cracks are large, or the part  is overstressed, the cracks may propagate into the active  regions and cause failures in the die.


When cracks are found to propagate into active regions of the  die and cause failures, changes to either the stresses the parts  undergoes, the materials set, or the engineering of the devices  must be made.


Cracks in the edge region of the die were sometimes detected  by the standard SAM analysis; other times they were missed (as shown in Fig. 2).  Both IR analysis and the Edge Enhanced  SAM analysis were able to detect these defects later.


Figure 2: Normal scans of die with edge cracks.  Note that the  edge crack is not visible on either image.


The die cracks in discussion here are always detected by IR  imaging after the die is thinned and polished.  The sample  preparation time and analysis by IR takes a few hours. The  Edge Enhanced SAM analysis consumes only minutes and is  non-destructive to the die, i.e. thinning is not required.


Unit A


Unit B


199


# Edge Enhancement for Acoustic Microscopy of Flip Chip Devices


Figure 3: Edge enhanced images of the same die. Note that  the die edge crack is clearly visible in both images.


Several variants of the SAM analysis were attempted to detect  the small die edge cracks: Heated water, edge enhancing  transducers, and various parameter settings of the gain, timeof-flight, and trigger. Only a set alteration of the Time-ofFlight (TOF) and the gain enabled detection of die edge cracks  that were not apparent with normal SAM parameter settings.  Figure 3 shows the die edge cracks detected with the edge  enhanced parameter settings on the same units as shown in  Figure 2. Variation of the other experimental parameters had  little or no effect on the detection threshold of the die edge  cracks. The defects were confirmed by IR inspection through  the backside of the die after thinning and polishing as shown  in Fig. 4.


Figure 4: Edge Enhanced SAM Image of Flip Chip die. Arrow indicates the location of subsequent IR imaging.


Alteration in the standard Scanning Acoustic Microscopy  parameters, the gain and TOF, enable detection of die edge  cracks in assembled Flip Chip devices. IR imaging after  thinning and polishing of the die confirms the die edge cracks.  The SAM analysis can now replace the IR imaging for  detection of small die edge cracks taking minutes to complete  instead of the hours involved in the sample preparation for IR  imaging.


The authors wish to acknowledge the helpful suggestions of  Lisa Logan-Williams, Senior Applications Sales Engineer, Sonoscan Incorporated, Silicon Valley.


[1] Kessler, L.W., “Acoustic Microscopy” in Metals  Handbook, 9th Ed., Vol. 17, ASM International, Materials  Park, OH, 1989, pp. 465-482.


[2] Semmons, J.E., “Flip Chips and Acoustic Micro Imaging: An overview of Past Applications, Present Status, and  Roadmap to the Future”, Proceedings of ESREF  Conference, Dresden, Germany, Oct. 2000.


[3] Komrowski, A.J., et.al., “Advanced Acoustic Micro  Imaging Applications: Deciphering multiple acoustic  echoes and reflections”, Proceedings from the 30th ISTFA, Worcester, MA, 2004, pp.376 – 379.


[4] Curiel, L.A., et.al., “Backside Application of Acoustic  Micro Imaging on Plastic Ball Grid Array and Plastic  Quad Flat Pack Packages”, Proceedings from the 30th  ISTFA, Worcester, MA, 2004, pp.389 – 392.


[5] Hartfield, C.D., and Moore, T.M, “Acoustic Microscopy  of Semiconductor Packages” in Microelectronics Failure  Analysis Desk Reference 5th Ed., ASM International, Materials Park, OH, 2004, pp. 268-288.


[6] Vittu, J., et.al., “Damage Free Dicing of Low – K  Wafers” Future Fab International Issue 17.


201


Method of Failure Site Isolation for Flash Memory Device Using FIB, Passive Voltage Contrast Techniques


Caiwen Yuan, Susan Li, Andy Gray


Spansion LLC, Sunnyvale, California, USA


Current VLSI devices have very complicated circuit  designs and very small feature size.  As a result, fault  isolation on failing devices becomes more and more  challenging task. There are many existing fault isolation  techniques. One of the commonly used fault isolation  techniques is photon or thermal emission detection from  the failing circuits [1-3]. This method is to detect photon  or thermal emission from defective circuitry by using a  Si CCD detector (for photon emission) or HgCd detector (for thermal emission) [4]. The emission is normally  generated from either electron-hole recombination  process of the junction (photon) or resistive type local  heating (thermal), or combination of both. The emission  method can provide relatively localized sites for possible  circuit failures. However, for many cases, no emission  site can be detected on the failing devices due to their  low level of leakage current, covered failure site by top  metal layers (photon cannot penetrate through metal  layers).  Although backside photoemission technique is  commonly used to detect the failure site covered with  multiple metal layers, it has the disadvantages of more  time consuming and less success rate than the method  we introduced below.  Without a localized failure site, it  will be very difficult, sometime even impossible, to find  the physical evidence for the failures. For instance, for a  memory device, electrical analysis showed leakage along  a wordline; however, without knowing which bit is  failing along the leaky wordline (typically 1024 bits on  each wordline), physical delayering and SEM inspection  are not likely to find the defective bit, particularly for the  devices with new technology and processes.


This paper will describe a method that has been  successfully used for isolating the defective location  along a leaky wordline on a memory FLASH device.


Flash Memory


FLASH is a nonvolatile memory that is used in  applications where data needs to be retained after power  has been turned off.  FLASH is also capable of updating  data easily and has fast access speeds.  For NOR FLASH  memory devices, a wordline (polysilicon 2) is the control  gate that typically connects all the floating gates (polysilicon 1) along a row. On the other hand, the  bitline is the drain side of the memory cell that is  connected all the drain contacts for each cell through a


metal 1 line.  The source side of the memory cells is connected  together through silicided diffusion area.  Please see Figure 1 for  the array layout of the FLASH memory core cells.  For a typical  erased cell, there are no electrons on the floating gate and has a  low Vt (threshold voltage applied to the transistor to turn on the  gate). This allows IDS current to flow when 5V gate voltage is  applied during read (Figure 2).


Figure 1: Array Layout for Flash Memory Core Cells


On the other hand, for a typical programmed cell, the electrons  stored on the floating gate have increased its cell Vt threshold.  When a 5V gate voltage is applied, no IDS current flows (Figure  3). Program operation is achieved through hot electron injection.  Electrons are attracted to the high gate voltage and get trapped in  the floating gate (Figure 4).  Meanwhile, erase operation is  achieved through Fowler Nordheim tunneling.  The high electric  field between the source and the gate causes electrons to tunnel  off the gate and onto the source (Figure 5).


202


# Method of Failure Site Isolation for Flash Memory Device Using FIB, Passive Voltage Contrast Techniques


Figure 2: An erased cell “1”


Figure 3: A programmed cell “0”


Method and Analysis


AA common failure mode for newer technology devices  is that one or multiple leaky wordlines prevent single or  multiple sectors from being erased after endurance  cycling or other types of stress testing.  With leakage  from failing wordlines to the substrate, the wordlines  cannot be biased to high negative voltage for the erase  operation. Though the failing wordlines can be identified  through electrical testing; if no emission site detected, it  would be still very difficult to find the exact failing  location along the entire wordlines during physical  analysis.  SEM inspection on each single cell (total 1024


of them) along the failing row at each level has been proved to be  very time consuming and ineffective.


Figure 4: Program Operation


Figure 5: Erase Operation


To find a better way to isolate the failing site along a leaky row, a  special fault isolation technique is used and described in this  paper. If the wordline is shorted to the ground, the poly line and  its contact will become illuminated during PVC (passive voltage  contrast) analysis because it conducts current from the electron  beam to the ground through the poly wordline during SEM (Scanning Electron Microscope) inspection (Figure 6). However, due to the fact that there is no emission site detected along the


Control


Sourc


Dr


Subs


GN


10.4


Sour


Dra i


Subst


e- e- e- e- eProgram


Control Gate


6.1


Gnd


Floating Gate


Drai


Erase


4V


Float


O -12v


203


Figure 6: Passive Voltage Contrast Analysis shows the  leaky wordline illuminated under SEM inspection.


failing row, it is still very difficult to find exact failing  location along the leaky row.  Traditional fault isolation  by sectioning a long line into small sections and  checking for leakage can be used for this case.  However, the leakage checking is not done by  mechanical probing, rather by using the passive voltage  contrast information shown on leaky sections.  The leaky  section will still appear illuminated while non-leaky  section will become dark due to the fact that the leaky  path has been eliminated.  Binary search (cutting the  leaky section into half each time to eliminate 50% of the  cells which are not leaky) is recommended to use since it  is most efficient way to locate the failure site with  minimum number of isolation cuts.  Focused-ion-beam is  used for sectioning the leaky poly wordline since the tool  has very fine control to cut geometry as small as 0.2um.  A detailed procedure follows:


Step 1:


The failing device needs to be deprocessed down to  ILD0 level (inter level dielectric layer between metal 1  and poly 2) for passive voltage contrast analysis.  At this  level, the poly 2 wordline contact (to metal 1) should be  exposed, and will be illuminated if the wordline is leaky  to the substrate.


Step 2:


If PVC analysis confirmed the wordline to be leaky (poly 2 contact is illuminated), the device needs to be  dry-etched (RIE plasma etch) to expose poly 2 wordline  partially so that the entire leaky poly 2 line will show  illuminated under SEM inspection


Step 3:


Use a FIB (Focus Ion Beam) system to isolate the failure  site along the illuminated wordline [5].  For devices with


new technology and process, the poly 2 wordline geometry is  very small (~0.2um), small FIB beam current (<10pA) should be  used for cutting in order to avoid extra damage on the wordline  and in surrounding area.  The FIB cut can be done using IEE (Insulated Enhanced Etch) to reduce material redeposition during  the cutting. The size of cut should have a length longer than the  wordline width (~1.5x) with a depth of at least 1um deep. Use  single line as cutting pattern instead of a solid box to increase  accuracy for the cut. The location of the cut should be selected  between two contacts to limit the damage on the two adjacent  memory cells. As mentioned, a binary search for failure isolation  is strongly recommended since it is the most efficient way to  narrow down failure site.


Step 4:


Figure 9: After failure isolation, Dual Beam FIB crosssection is performed to further locate the defect for  inspection


The cross-section image in figure 9 (inside the red  rectangle) showed abnormality in the diffusion region


and indicated some masking issue when the STI formation and  implantation was performed.


A paper on how to isolate the wordline leakage using FIB cutting  and passive voltage contrast on the leaky wordline has been  presented.  The concept of this paper is not just limited to this  application; rather it can be used for all similar type of fault  isolation work for other applications.


1. Gary Shade, Microelectronics Failure analysis, ASM  international (Ohio, 2004) pp.347-355.


2. Christian Boit, Microelectronics Failure analysis, ASM  international (Ohio, 2004) pp.356-368.


3. Susan Li, Microelectronics Failure analysis, ASM  international (Ohio, 2004) pp.332-340


4. ACT Quah, JCH Phang, S Li, M Massoodi, C Yuan, LS  Koh, KH Chan, CM Chua, “CORRELATION OF  FLASH MEMORY DEFECTS DETECTED WITH  PASSIVE AND ACTIVE LOCALIZATION  TECHNIQUES,” ISTFA, 2004, pp. 604-608


5. Caiwen Yuan, Mehrdad Mahanpour, Hung-Jen Lin, Gene Hill, “Application of Focused Ion Beam in Debug  and Characterization of 0.13 µm Copper Interconnect  Technology”, ISTFA, 2002, pp. 183-188


205


Increasing Planarity for Failure Analysis Using Blocked Reactive Ion Etching  Combined with Planar Polish


Mary Elizabeth Weldy


Intel Corporation, Folsom, CA 95630  mary.weldy@intel.com


Leslie Serrano


Intel Corporation, Santa Clara, CA 95052  leslie.serrano@intel.com


Challenges in sample preparation for semiconductor failure  analysis are always increasing as more complex material and  smaller dimensions are required to meet the needs of the  semiconductor industry. These changes require the constant  need for more refined procedures in all areas of sample  preparation, including mechanical polish. This paper will  present a newly modified technique which increases the  planarity at the critical edge of the sample and results in a  larger planar region of interest.


In previous technologies it was difficult to mechanically  planar polish without losing the ROI (regions of interest) at  the extreme edge [1]. Recently, it has become even more  difficult with the introduction of copper and new isolation  materials such as CDO (carbon doped oxide) and other low K  dielectrics. In the past when using the failure analysis  techniques of RIE (reactive ion etching) in combination with  planar polishing, an edge effect was observed [2]. An edge  effect occurs when the active device structures at the edge of  the sample polish at a faster rate resulting in an angled  downward slope. The effect observed in this situation is due to  the higher density of active device regions next to the lower  density of the scribe line structures at the edge of the sample. This density difference also accentuates the polish rate, due to  variations of different materials such as copper or poly silicon  compared to isolation. When using conventional RIE and  planar polish, this edge effect and natural edge rounding often  results in multiple layers at the ROI (see Fig. 1) and in some  cases loss of ROI at the desired lower metal or poly layer.  It  also causes further analysis such as 1. Gate-ox defect  inspection, 2. SEM inspection for defects, (Pico-probing) 3. Atomic Force Microscopy and poly CD measurements to  become either more difficult or impossible if the ROI is lost.   As microprocessor critical dimensions become smaller and the  silicon more densely populated with thinner layers of gateoxide, there is an increased need for the analysis listed above. Hence, preparation such as deprocessing becomes increasingly


important. For example, it is critical to obtain a planar polish  though the salicide but not exceeding the poly silicon prior to  selective etch of the poly for gate-oxide defect inspection [3].


Figure 1: Optical micrograph of the ROI using planar polish. The ROI is at Metal 1, 2, 3 and 4. This micrograph shows the  edge effect and planarity issues.


This new method combines both a blocked RIE and a standard  planar polish which decreases the edge effect and increases  overall planarity. Half of the die or wafer piece opposite to the  edge ROI is blocked using copper tape before RIE etching (see Fig. 2).


Figure 2: Optical micrograph of sample with copper tape  blocking half of the die on the side opposite to ROI.


Scribe line Metal 1


Metal 2


Metal 3


Metal 4


ROI


Region of Interest


Half the die blocked with copper tape


206


# Increasing Planarity for Failure Analysis Using Blocked Reactive Ion Etching Combined with Planar Polish


The sample is then etched using RIE to remove nitride and  two to three layers of isolation (the amount of removal will  vary depending on the desired layer for analysis). The blocked  region remains untouched at the nitride cap over the top metal  layer. The ROI side of the sample is left with upper metal  layers exposed without isolation (see Fig. 3a.).


Polishing Wheel


Figure 3A: Cross-sectional view of die or wafer piece after  blocked RIE etch, before polish.


The upper metal layers are easily polished away in a matter of  seconds on a polishing wheel because the nitride and isolation  layers supporting the upper metal layers have been removed. This is referred to as skeleton etch, and it is followed by  skeleton polish. When the skeleton polish is performed, the  first area to make contact with the wheel is the highest point  on the sample, which, in this case, will be the blocked region  at the nitride cap (see Fig.3b).


Figure 3b: Cross-sectional view of die or wafer piece after  blocked RIE etch and polish.


When the nitride cap makes full contact with the wheel, it  slows the polishing rate and decreases the sloped angle of the  opposite edge ROI. At this point, inspection of the sample  under an optical microscope will reveal a reduction in the  fringes indicating an increased sample planarity and a larger  resulting ROI (see Figs. 4 and 5).


Figure 4: Optical micrograph of ROI using RIE blocking


and planar polish. Sample is now ready for further analysis (i.e. Pico-probing, gate-oxide defect etch, SEM inspection for  defects, AFM and other failure analysis methods).


Figure 5: Optical micrograph of neighboring ROI next to ROI  above in figure 4. This method enabled multiple cells  at the  same planarity.


Block RIE/Planar Polish Step Details


For this paper a flip chip packaged die was used. The size was  approximately 1cm x 1cm. The die was removed from the  package using conventional methods. The package underfill  epoxy, polyimide and package to die bumps were removed  with wet chemistry. A piece of a wafer processed through top  layer nitride deposition can also be used with this polishing  procedure.


Unblocked  Region after  RIE


Blocked  region


after RIE


Block


Unblocked  Region


after RIE  and Polish


Blocked


Region,   removed


from polish


Schematic Key


207


The sample was placed in the RIE. Half of the die, on the side  opposite to the ROI was blocked using copper tape (as seen in  Fig. 2). This prevented dry etching of the blocked region and  allowed etching of the un-blocked area. The recipes for nitride  and low K dielectric etching were already characterized in  previous work. The nitride layer and approximately two layers  of low K dielectric were removed using these recipes.  This  dry etch method is referred to as skeleton etch because the  isolation layers are removed leaving the metal unsupported. The unsupported metal layers can be easily polished away in a  matter of a few seconds using a tripod polishing tool to ensure  planarity. This is referred to a skeleton polish. Reducing the  polishing time in this manner also aids in decreasing the edge  effect or edge rounding. The longer a sample is polished, the  more edge rounding can be observed.


It is recommended that the analyst remove no more than two  layers at a time to reduce the risk of over etch/polish. Analysts  should stop RIE etch when the sample is one layer above the  layer of interest.


After the unsupported metal was removed during polish, the  skeleton polish/etch steps were repeated using low K dielectric  etch with reduced etching times (one to one and a half layers  of dielectric removal at a time) and skeleton polish. For this  sample, the target was metal one. Dry etching was  discontinued when the sample was skeleton etched/polished to  metal two. The tripod was used again to polish to the plane of  metal 1 plane of interest. Optical microscope inspection after  each step is critical in maintaining the integrity of the sample.


Conclusions and Acknowledgments


This method has been verified on dies, wafer pieces and dies  thinned and attached to blank silicon for support. It has proven  to be a successful delayering technique and helpful in  facilitating further analysis. It is useful for increasing overall  planarity and particularly helpful for the extreme edge.


The authors would like to acknowledge: Robert Small for  providing schematics, support of supervisors Phung-Loan  Nguyen in reviewing this document and Fimy Sahaida for  reviewing and providing coaching on the project.


[1]  Internal research, Intel Corporation, Folsom, CA. 2004.


[2] Hayes, Kathy “Tripod Polish,” Intel confidential  document, Oct. 2002 Hillsboro, Oregon


[3] Korchnoi, Valentina, “Investigation of Choline Hydroxide  for Selective Silicon Etch from a Gate Oxide Failure  Analysis Standpoint,” ISTFA Conference November 2002, pp 328-331.


208


Nanomechanical Characterization in the FIB


Thomas M. Moore


Omniprobe, Inc. 10410 Miller Road, Dallas, TX 75238  Ph. (214) 572-6800


Fax (214) 572-6801


moore@omniprobe.com,


The availability of the Focused Ion Beam (FIB) microscope


with its excellent imaging resolution, depth of focus and ion  milling capability have made it an appealing platform for  materials characterization at the sub-micron, or “nano” level. The FIB has already become popular for the preparation of  samples for TEM from bulk samples [1-3]. Nano-mechanical  characterization in the FIB is another extension of the FIB  capabilities into the realm of nano-technology.


A very important advantage of materials characterization in the  FIB is the ability to image and even isolate small structures  with the ion beam. In this way, the local mechanical properties  of thin films or beams can be directly measured. Extrapolating  mechanical properties of small structures from bulk property  data is not always appropriate. Also, “edge effect” properties  of thin films become more important as the surface to volume  ratio increases. The ability to measure the mechanical response  of tiny structures can be critical for rapid technology  development. For example, in the integrated circuit industry, new materials challenges have been posed by the conversion to  copper traces, low dielectric constant insulating layers and Pbfree solders. Rapid integration of these new materials requires  accurate finite element modeling of material behavior, which  depends on accurate thin film mechanical data of unfamiliar  materials.


A sensitive strain gauge has been embedded in the probe shaft  of an automated in-situ nanomanipulator for the FIB or  Scanning Electron Microscope (SEM) [4]. The strain gauge  used here is a tiny resistive gauge connected to a sensitive  Wheatstone bridge amplifier. The strain gauge is positioned to  maximize sensitivity to deflection of the probe shaft. The most  straightforward application of this system is automated surface  contact detection that is appropriate for a fine tip and  independent of electrical continuity to the FIB ground.  Beyond this purpose, this system can be used for such  mechanical tests as bending beam, nano-hardness and fracture  limit tests. This system can be used effectively in a qualitative  mode which is quite sufficient for many experiments. It can


also be used to obtain quantitative data with an NIST-traceable  calibrated load cell. In addition, nano-mechanical testing can  be combined with simultaneous electrical testing and video  recording of the image.


An example of the application of nano-mechanical testing to  the FIB environment is the fracture testing of tiny particles. This simple test provides important information about the  particle’s mechanical properties. Figure 1 shows the result of  such a fracture experiment. The ultimate fracture strength of  tiny particles can be assessed in a direct method by loading the  particles to failure. Figure 2 is the corresponding load vs. overtravel curve for such a measurement.


Figure 1: Result of a particle fracture test.


0 1 2 3 4 5 6 7 8


1.6


Overtravel (um)


Figure 2: Load vs. overtravel graph for a particle fracture  test.


209


# Nanomechanical Characterization in the FIB


0.5 1


1.5 2


2.5 3


0 0.6 1.2 1.8 2.4 3 3.6 4.2 4.8 5.4 6


Overtravel


Overtravel is defined as the displacement of the probe shaft  towards the center of the particle after the probe tip first makes  contact with the surface of the particle. Because of the size and  brittleness of the particle, these data include some compliance  of the fine probe tip as well as the elastic response of the  particle. The ultimate fracture strength of the particle (roughly  6mg load at fracture) is determined by calibrating the  measurement shaft with an NIST-traceable load cell. With an  automated testing routine, hundreds of particles can be  analyzed within two hours, and the data compiled can be used  for comparison of particles from a different production  process.


In another example, the process of in-line bond pad probing is  simulated with the nanomanipulator to determine the  conditions responsible for subsurface cracking of the Cu/low-k  dielectric stack beneath the bond pad (Figure 3).


Figure 3: The visualization of a scrub mark made with the  probe tip point [5].


Figure 4: The contact resistance versus overtravel (µm) diagram for a single scrubbing event as depicted in Fig. 3 [5].


This is a condition that can lead to an effect called “cratering” in which the bond (wire bond of flip chip bump) breaks away  from the die in the package and removes a portion of the  dielectric stack. In-line probing typically involves “scrubbing” the pad with the probe tip to break through any surface oxide  and give a reproducible contact resistance. In these  experiments, the pointed probe tip typically used for testing  tiny objects is replaced with a standard probe tip with a flat  bottom, which is used for in-line testing.   An interesting graph


that shows the physical behavior of a probe tip while  performing the scrubbing movement is shown in Figure 4 [5-6].


Figure 4 shows the effect of surface debris on contact  resistance during the scrubbing action. Figure 5 shows the  appearance of a bond pad after repeated touchdown and  scrubbing events. The probe tip loading information is shown  in Figure 6.


Figure 5: FIB image of a bond pad scrubbing test involving  multiple touchdowns. One event ran off the edge of the pad.


[6].


Figure 6: Probe load measurements recorded for 10 repeated  touchdown events. The 7th touchdown having lower force  correlated to scrubbing off the edge of the pad. The first  touchdown was held a long period of time prior to retracting


Surface damage and loading information can be combined  with subsurface damage revealed by subsequent in-situ lift-out  and TEM inspection of the probed areas. This in-situ lift-out  can be performed with the same nanomanipulator that is used  for the probing simulations. In addition, real time video of the  touchdown and scrubbing events can be captured  simultaneously with the electrical and mechanical data.


The study of MEMS structures with nanomechanical testing  offers a great opportunity for understanding such processes as  wear, stiction and elastic behavior of a dynamic compound  system. Figure 7 shows the testing of the load required to


210


deflect a Digital Light ProcessingTM (DLP™ a Texas  Instruments Technology) mirror device. Figure 8 shows a  typical load vs. displacement curve for this device. This is an  excellent example of the combination of the high resolution  imaging capabilities of the SEM or FIB with nanomechanical  testing performed by sensitive strain gauge attached to a  nanomanipulator. Exact placement and simultaneous visual  monitoring of the experiment increase efficiency and add a  great value to the data. Unlike in previous examples discussed  in this study, in this case the loads required for deflection are  in the micro-gram range.


Figure 7: Mirror deflection experiment using the Texas  Instruments DLP™ chip.


Calibration in this region often requires extrapolation of  calibration data, or special calibrated load cells. In the case  shown in Figs. 7 and 8, we extrapolated the calibration data  from an NIST-traceable load cell that operates in the milligram  range. This certainly provides a repeatable qualitative standard  with which mirrors of different lots can be accurately  compared. More accurate quantitative calibration would  require a dedicated calibration source.


Figure 8: Load in µg vs. deflection in µm for a mirror  deflection using the Texas Instruments DLP™ chip.


The examples highlighted here demonstrate the power and  flexibility of nanomechanical testing in the FIB or SEM with a  probe shaft that includes a built-in strain gauge. Loads that  range from grams to micrograms are achievable. Calibration is  limited only by the availability of calibrated load cells in the  smallest load ranges. Deflections in the range of a few  nanometers range can be accurately applied. Simultaneous  electrical, mechanical and visual data can be combined to  provide a revealing study of physical behavior of complex and  dynamic nanostructures.


The author wants to thank Rocky Kruger and Aaron Smith of  Omniprobe for their hard work to develop the hardware and  software for the nanomechanical test system. Specail thanks  also go to Cheryl Hartfield of Texas Instruments for review of  the manuscript and insightful discussions.


[1] Window, A. L. et al, Strain Gauge Technology, Applied  Science (London, New York, 1982).


[2] T.M. Moore, R.D. Kruger and C. Hartfield, U.S. Patent  6,420,722.


[3] T. M. Moore, U.S. Patent 6,570,170.


[4] Patent pending. Omniprobe, Inc.


[5] Hartfield, C. et al, “A Novel In-situ Methodology to  Characterize Bond Pad and Dielectric Mechanical  Behavior during Wafer Level Test,” IEEE Southwest Test  Workshop (SWTW) 2003.


[6] Hartfield, C. et al, “Mechanical and Electrical  Characterization of an IC Bond Pad Stack Using a Novel  In-situ Methodology”, 29th ISTFA Proceedings, pp. 486-495 (2003).


211


Couple Passive Voltage Contrast with Scanning Probe Microscope   to Identify Invisible Implant Issue


Cha-Ming Shen, Shi-Chen Lin, Chen-May Huang, Huay-Xan Lin, Chi-Hong Wang


Taiwan Semiconductor Manufacture Company, Ltd., Taiwan


1,Nan-Ke North Rd., Tainan Science Park, Tainan, Taiwan, R. O. C.


As rapid development of semiconductor process technology  has led to rapidly decreasing feature size on integrated  circuits, analysis techniques, which are used to look for the  root causes of failure, are increasingly challenged to maintain  their applicability in localizing exact fault position or catching  sight of the defect mode. Especially in advanced ULSI  technologies, PFA (physical failure analysis) frequently fails  to identify the defect because the type of defect may be  invisible even by SEM and TEM observation, or too tiny to be  localized.


Among most applications, PVC (passive voltage contrast) is a  popular technology to determine opens or shorts after  deprocessing. The difference in secondary electron emission, which is a function of surface work function, topography, and  local surface potential, assists us in revealing the abnormal  phenomenon at a failure site. That is to say, as a sample is  exposed to the electron beam, floating and grounded  structures acquire different surface potentials, which generate  different amounts of secondary electron emission, resulting in  variations in SEM contrast between structures.


Recently, SPM (scanning probe microscopy) offers another  solution for deep-submicron technologies because the  piezoelectric scanner of the SPM has very high resolution of  spatial dimensions, even in the nanometer range. Thus it is  able to probe deep-submicron or nanometer features  accurately. Furthermore, it can also provide current mapping  with high sensitivity and I-V (current–voltage) characterization of targets.


In this paper, our objective was to organize a judicious  reasoning method by coupling PVC with SPM for revealing  particular invisible defect modes, which were imperceptible to  observe and very difficult to identify by means of traditional  PFA techniques. In order to certify this compound method, it  is applied to an implant issue as a case study. Through solving  this particular defect mode, whose exact failure position could  not be determined even with the most sensitive PVC or highresolution SPM current mapping, the procedures and  contentions are illustrated further.


As most of us know, PVC is a popular failure analysis  technique to determine open or short issues [1]. SPM is  another powerful technique for measuring, characterization of  dielectric or judging gate-oxide integrity [2].


The purpose of our experiment was to establish a novel failure  analysis methodology that coupled passive voltage contrast  with scanning probe microscopy to reveal some particular  invisible defects. Because of different imaging mechanisms of  PVC and SPM, more diagnostic information is provided for  reasoning out failure mechanisms.


Generally, the reasoning method can be itemized as the  following steps concisely.


First, PVC is used for isolating the suspected AA (transistor  active area) around a localized position. Next, in order to  lessen questionable targets, SPM should be utilized to obtain a  current mapping around the region that had been detected as  abnormal by PVC. Sometimes even the highest resolution of  current mapping is unable to identify the failure In such cases, differential analysis must be utilized. One by one the I-V  curves of all contacts on the suspected and matching AA  should be measured by SPM to form a comprehensive data  set.


Following measurement and comparison, every contact with  an abnormal I-V curve is carefully checked based on its  attributes to expose the relationship between neighbors. Thereupon, a conceivable failure mechanism is proposed  according to the electrical information obtained by SPM and  theory of semiconductor physics. Simultaneously, the exact  defect site could be pointed out by matching the layout and  deductions from electrostatics. Finally, the proposed failure  mechanism should be reviewed for conformity with the  observed PVC.


In the following experiment, a sample of interest with 0.1um  process had BIST (built-in self test) failure around the edge of  wafer. Because emission microscopy could not detect a solid  hot spot, the failure site was located by using the test datalog


212


# Couple Passive Voltage Contrast with Scanning Probe Microscope to Identify Invisible Implant Issue


and fault diagnosis method. After deprocessing to the contact  layer and utilizing SEM PVC, all N+/PW contacts around the  suspected position and on the same active area were brighter  than normal (Fig. 1).


Figure 1: From 1kV SEM PVC, all N+/PW contacts on the  same active area showed brighter than reference.


Then the SPM tool was applied to obtain the current mapping  and measure I-V curves (Fig. 2 and 3). According to the  electrical information, both larger reverse saturation current  and larger drift current of forward bias showed there was an  abnormal P-N junction involved with the failure. The shift of  cut-in voltage implied insufficient N+ doping concentration in  the target area. Moreover, considering the features observed  by PVC, a poor N+ implant was highly suspected.


Figure 2: After current mapping of SPM, no abnormal contact  could be identified, although there were obviously abnormal  PVC on targets.


Figure 3: According to SPM I-V curve, both larger reverse  saturation current and drift current showed an abnormal P-N  junction. The forward cut-in voltage shift implied insufficient  N+ dopant in the located region.


Because the failure was induced not by full blocked, but only  partial, implant issue, chemical staining was not suited to the  occasion. So TEM was used successfully to substantiate the  indirect inference that a poor implant caused poor salicide  formation (Fig. 4). Subsequently, feedback from the KLA  team confirmed our inference.


Figure 4: Comparing rough shape at failure site to smooth  shape of reference, poor Co-salicide was revealed to be the  indirect inference. This was induced by prior poor N+ implant  process.


Failure


-1V Bias


+1V Bias


213


For further study, two more specific samples that suffered the  same failure type were selected for PFA. One had been  diagnosed and located to a fault buffer, and the other had an  irregular block SRAM failure.


Following the previous steps, the PVC of the first sample was  found to be abnormal with graded brightness along the located  N+/PW region (Fig. 5).  SPM measurements showed different  levels of reverse saturation current that corresponded to the  voltage contrast variations (Fig. 6).


Figure 5: From 1kV SEM PVC, there was graded brightness (i.e. N1>N2>N3) along located N+/PW region of the fault  buffer.


Figure 6: SPM measurements showing that different levels of  reverse saturation current (i.e. N1>N2>N3) corresponded to  the voltage contras. variations.


In the meanwhile, the other specimen which had block SRAM  failure showed similar results both in PVC and SPM after  deprocessing and measuring (Fig. 7 and 8).


Figure 7: From 1kV SEM PVC, there was graded brightness (i.e. N1>N2>N3) around the NMOS site of the block SRAM  failure region.


Figure 8: SPM measurement showed that different levels of  reverse saturation current (i.e. N1>N2>N3) corresponded to  above the voltage contrast variations.


Gathering these results, the abnormal implant issue could be  expressed by three different types of I-V curve (Fig. 9).


Figure 9:  Three different types of I-V curve


(a) Partial implantation induced leakage current


(b) Insufficient implantation induced Schottky barrier


(c) Too little implantation induced junction breakdown


Basically, these I-V curves and unusual P-N junction  characteristics could be produced and explained by the “ideal  diode equation” and “theory of the junction”.


N3 N2 N1


N1


N2


N3


214


The ideal diode equation is:


/ −


×


kT


qV


N C


N


L D


≡


where    :SI   reverse saturation current


:SJ   reverse saturation current density


:DN   N+ donor doping concentration


:AN   PW accepter doping concentration


:nD   diffusion constant of electron


:pD   diffusion constant of hole


:nL    diffusion length for electron


:pL    diffusion length for hole


:in     intrinsic concentration


:


constant variable


First, considering the above equation, since


∆


is  inversely proportional to DN , the corresponding reverse  saturation current  (i.e. commensurate with leakage current) would increase as the N+ implant concentration decreased  simultaneously. The related result was shown in Fig. 9(a).


After each FIB cut, zoom out the SEM image to view which  section of the leaky wordline still illuminating.  The illuminated  portion is the section that still contains the leaky path (failure site, Figure7), and more FIB cutting will be done at this section to  further narrow down the failing location.


Figure 7: FIB cut to isolate the leaky wordline.


Step 5:


In some cases, the FIB cut does not result in two different voltage  contrasts. This is probably because the wordline was not cut  through completely.  Then do a clean cut with a solid box pattern  with size of 0.5umx1um and depth of 0.01um. This will normally  clean up the residue and cut the line through.


Step 6:


Repeat Step 3, 4 and 5 until the illuminated wordline section only  contains several cells. For a typical memory device, a row  normally has 1024 memory cells, and maximum of 9 cuts will  narrow down the failure down to the last 2 cells (Figure 8).


Cell Number: 1024  512  256  128  64  32  16  8


4 2


FIB cuts:         1st       2nd       3rd      4th      5th       6th      7th    8th    9th


204


Figure 8: Binary search for failure site with FIB cuts can  isolate the failing location down to the last two cells


Step 7:


After the failure site is narrowed down to the last several  cells, FIB Dual Beam cross-section should be performed  to find out exact defect location in the suspected area (Figure 9).  Typical FIB cross-section can be easily done  in the area with a size of 8-10 memory cells, so that the  isolation work with FIB cut does not need to go down to  the last two cells in order to reduce damage in the failure  area before the final FIB cross-section work.


measurement techniques can measure signals with negative  SNRs, where the signal of interest is actually lower in  amplitude than the system noise.  See Figure 3 for a block  diagram of this system.  Figures 4 and 5 show the  improvement that can be achieved using this technique.  This  approach is probably not acceptable for a time sensitive  activity like automated testing but is useful for a Failure  Analysis application.


It should be noted that it is possible to reverse the connections  to feed the modulated signal to the probe and the unmodulated  signal to the DUT.  The mixer conversion gain of the  prototype probe is highly dependent upon the LO drive level, so we chose to use an unmodulated signal as the LO input.


Comparison to Current Technologies


Because the Radio Probe is best suited to measurement of  single-frequency signals, active probe technologies will  continue to be used to measure nonsinusoidal waveforms.  But  consider the challenges that high-frequency active probes  must meet.  They must have very low input capacitance and  yet have flat frequency response over a DC to RF bandwidth.  As frequencies go up, this combination becomes increasingly  difficult to achieve.  In contrast, the nodes of an RF amplifier  chain with a gain problem, for instance, can be measured with  a receiver that is specifically designed for that frequency  range.  With enough gain, such a receiver can be used to  monitor the RF signals at each circuit block, with minimal  loading or frequency aberrations.  This suggests that Radio  Probes can easily be fabricated to perform failure analysis on  RF ICs with frequency ranges exceeding the current state of  the art for active probes.  And as stated previously, Radio  Probes can be used to perform true differential mode  measurements on the internal nodes of RF IC's.  This  capability has not been demonstrated using commercially  available active probes.


The Laser Voltage Probe can also be used to measure high  speed signals, but it is very expensive.  In addition, it would  be much more difficult to increase its frequency range in  comparison to the Radio Probe.


The Radio Probe concept offers a number of advantages  compared to active probes.


First, the overall cost of a failure analysis setup is lower  because an expensive spectrum analyzer or high speed  oscilloscope is not required.  A lower cost RF generator and  DVM or DSO (preferred for differential measurements) would  be needed with the Radio Probe.  SNR reduction would  require a digital oscilloscope.


Second, the Radio Probe concept can be readily extended to  support analysis of state –of –the art ICs—all that is needed is  a receiver with the required frequency range and gain, and an  RF oscillator capable of generating the required frequency.  In


225


contrast, development of wideband active probes suitable for  probing IC circuit nodes appears to be relatively slow, perhaps  due to the small volume of units that could be sold versus  development cost.


Third, true differential mode internal measurements of RF ICs  can be made using the Radio Probe.


Fourth, SNR issues can be resolved by using an additional low  frequency signal generator, amplitude modulator, and perhaps  a buffer amplifier., All of these components are readily  available and inexpensive.


Finally, because of its predominantly resistive input  impedance, the Radio Probe does not significantly load RF  ICs and does not exhibit a resonant “peak’ due to parasitic  input capacitance and ground return inductance.  This is  comparable to current state –of –the art active probes costing  thousands of dollars more than the Radio Probe.


The Radio Probe is a single frequency measurement tool, so it  complements, rather than replaces, active probes.


Figure 1.  Block diagram of a Radio Probe.  The input


attenuator introduces a loss of -60 dB but the remaining


circuitry provides +60 dB, for an overall gain of 0 dB (A = 1).


Figure 2.  Photo showing two Radio Probes being used to  perform differential RF measurements on an RF IC.


Figure 3.  Diagram showing system to improve the SNR of the Radio Probe output.  F1 is modulated by the low frequency signal


F2, generating sidebands at (F1 + F2) and (F1 - F2).  When the modulated signal is mixed with F1 in the Radio Probe, it outputs  F2 + noise.   The SNR is improved by averaging the signal with the digital oscilloscope (DSO) .


226


1) .


Figure 4.  Low level, noisy output of Radio  Probe.


Figure 5.  Output of Radio Probe after signal  averaging.


227


High Resolution Acoustic Microscopy with Low Frequency and   Its Applications in Analysis of Ferroelectrics


Q. R. Yin*, H. F. Yu, H. R. Zeng, G. R. Li, and A. L. Ding


State Key Laboratory of High Performance Ceramics and Superfine Microstructure,  Shanghai Institute of Ceramics, Chinese Academy of Sciences, Shanghai 200050, China *Corresponding author: e-mail:qryin@sunm.shcnc.ac.cn


Tel.: +86-21-5241-2424, Fax: +86 -21-5241-3122


Ferroelectrics have spontaneous polarization, which can be


oriented along with electric field and show high dielectric  constant, high switching speed, nonvolatile memory character  and large capacity memories on a given silicon wafer. Large-scale manufacturing is presently underway to  incorporate ferroelectric materials as storage and bypass  capacitors in IC circuitry. Nondestructive observation of  domain structure of ferroelectrics, dynamic behavior under  external field and related phenomena is becoming  significant[1-3]. As a non-destructive and subsurface  characterizing technique, the acoustic microscopy based on a  commercial SPM was developed in our lab[4-7]. Its working  frequency is in the range of several kHz to decades of kHz, which is much lower than that of conventional acoustic  imaging techniques[7-8]. It also shows resolution of ~10nm. This technique was used for direct observation of local  ferroelectricity, elasticity and defects on several inorganic  functional materials, transparent PLZT ceramics, relax-based  PMN-PT crystal and lead-free Bi4Ti3O12 ceramics without any  special processing (polishing or etching) to the sample, which  is particularly useful and convenient for analyzing  ferroelectrics / semiconductor integrated material and devices.


Scanning probe acoustic microscope (SPAM) was homemade  based on the commercial Scanning Probe Microscope (SPM) (SPA 400, SPI3800N, Seiko Inc. Japan), as shown in Fig. 1. In  SPAM, a piezoelectric transducer was bonded onto a sample  holder of an SPM, and the sample was glued on the  transducer. An external function generator (33120A, Agilent  Inc.) provides sinusoidal excitation signals applied to the  piezoelectric transducer, which gives rise to flexural vibration  and emits acoustic waves into the sample and causes a  periodic local deformation of the sample’s surface underneath  the tip. The motion of the SPM tip is detected optically by  laser beam deflection from the backside of the cantilever. The  detection signal is then fed to a lock-in amplifier (Model 7280  DSP, signal recovery instrumentation) for imaging. In our  SPM, A 2μm-thick, 90μm-long Ti/Pt-coated Si cantilever


(Micro Masch, NSC12-B) with a spring constant of 14 N/m  and resonance frequency of 315 kHz was used.


Topography-feedback


Transducer  Sample


Personal Computer


Photodiode


Lock-in Amplifier


Scanner


Figure 1: The set-up of the low frequency scanning probe  acoustic microscope.


(b) ( )


Figure 2: LF-SPAM images of the (110)-oriented  PMN-33%PT single crystal. (a)The topography image and (b) the corresponding low frequency acoustic image. The  excitation frequency f =6.42kHz.


With the developed low frequency scanning probe acoustic  microscope (LF-SPAM) technique, the imaging studies were  conducted on PMN-33%PT single crystals[9]. Figure 2 is the  topography and its corresponding low frequency acoustic  image successfully acquired from a 40μm × 40μm area of the  sample. And figure 2(a) is the typical topography of the  polished crystal sample, which shows no more information  except for some polishing scratches. While in figure 2(b), significant difference from the topography image was noticed


228


# High Resolution Acoustic Microscopy with Low Frequency and Its Applications in Analysis of Ferroelectrics


namely the fingerprint pattern domains uniformly distributed  throughout the examined areas. It is to be noted that the lateral  resolution is down in the nanometer range. Careful  investigation of the acoustic image shows that similar  polishing scratches were mixed with the domain structure in  the acoustic image, whose positions correspond to the  scratches in the topography. They probably correspond to the  residual stress zones by the polishing scratches.


Figure 3: The surface topography image (a) and the  corresponding acoustic microscopy image (b) of the PLZT  transparent ceramics at f = 131.5 kHz.


Fig. 3(a) is the topography of the PLZT sample observed by  normal SFM that only shows surface scratches. Fig. 3(b) is a  SPAM image obtained from the same area (see the same  scratches in both images). The most unique and significant  feature of this SPAM image is that in a single image it not  only reveals the ferroelectric domain patterns similar to those  reported by piezoresponse SFM[10], but also reveals common  surface topology such as grain size, grain boundaries and  scratches or cracks simultaneously. The grains shown in the  image are less than 10 μm in size. This unique feature will  make it easier to investigate the interaction between domain  switching and microcrack initiation and propagation in  piezoelectric single crystals and other ferroelectric materials, which is an important research issue in the area of applications  of ferroelectrics. The periodic striation-like patterns of ∼300  nm in width shown in Fig. 3(b) is similar to the fingerprint  patterns observed in PZN-PT and PMN-PT single crystals by  Abplanalp et al.[10] using piezoresponse SFM and these  finger-print patterns were explained as ferroelectric domains  with anti-parallel polarizations. Compared with the  piezoresponse SFM image of domains obtained by Abplanalp  et al., the SPAM image in Fig. 3(b) shows a clearer and  sharper domain contrast.


Fig. 4(a) is another elastic response image of 3.5 × 3.5 μm2  scanning area in the Bi4Ti2.98Nb0.02O12 sample at 30 kHz  modulation frequency. As shown in Fig. 4(a), scale-like fine  structures perpendicular to the long axis of the plate-like  middle grain in the inserted top-right topography image of Fig. 4(a) can be clearly seen. The line scanning signal of line C–C′ in Fig. 4(a) reveals that the elastic structures arrange in a  scale-like form as observed in Fig. 4(c). The vertical distance  between the scale structures is down to 12 nm. The scale  structures of Fig. 4(b) can be clearly seen in the corresponding  three-dimensional configuration of Fig. 4(d). Note the  observed angle is rotated so as to get an optimum view effect.


The elastic structure parallel and perpendicular to the long axis  of plate-like grain would be a result of the crystal structure  arrangement in the Bi4Ti2.98Nb0.02O12 grains.


1μm


500nm


Figure 4: (a) Elastic response image of 3.5 × 3.5 μm2  scanning area of Bi4Ti2.98Nb0.02O12 ceramics with the  corresponding topography in the up-right corner. (b) Zoom  image of the area indicated in (a). (c) The line scanning  elastic signal of line C–C’ indicated in (b). (d) Three-dimensional image of (b) with rotated view angle.


Low frequency scanning probe acoustic microscope (SPAM) based on commercial scanning probe microscope was  successfully developed. The excitation frequency is in the  range of several kHz to decades of kHz, which is much lower  than that of the conventional acoustic imaging techniques. But  several applications of SPAM involving ferroelectric samples  with the resolution of 10nm were obtained. The expanding  scope of application for SPAM shows exciting possibilities for  non-destructive analyses in the microelectrics industry.


This work is supported by the National “973” Key Basic  Program of china (No. 2002CB613307).


229


[1] Gruverman, A. et al, “Imaging and Control of Domain  Structure in Ferroelectric Thin Films via Scanning Force  Microscopy”, Ann. Rev. Mater. Sci., Vol. 28 (1998), pp. 101-123.


[2] Ganpule, C. S. et al, “Domain Nucleation and Relaxation  Kinetics in Ferroelectric Thin Films”, Appl. Phys. Lett., Vol. 77, No. 20 (2000), pp. 3275-3277.


[3] Kalinin, S. V. et al, “Temperature Dependence of  Polarization and Charge Dynamics on The BaTiO3 (110) Surfaces by Scanning Probe Microscopy”, Appl. Phys. Lett., Vol. 78, No. 8 (2001), pp. 1116-1118.


[4] Yin, Q. R. et al, “SFM in Acoustic Mode and Its  Applications to Observation of Ferroelectric Domain”, Materials Science and Engineering B, Vol. 120  (2005), pp. 100-103.


[5] Yu, H. F. et al, “In Situ Characterization of Domain  Structure and Local Elasticity in Nb-doped Bi4Ti3O12  Ceramics by Scanning Probe Microscopy”, Materials  Letters, Vol. 59  (2005), pp. 1538-1541.


[6] Zeng, H. R. et al, “ Local Elasticity Imaging of  Ferroelectric Domains in Pb(Mg1/3Nb2/3)O3-PbTiO3  Single Crystals by Low-frequency Atomic Force Acoustic  Microscopy”, Solid State Communications, Vol. 133  (2005), pp. 521-525.


[7] Yamanaka, K. et al, “Ultrasonic Force Microscopy for  Nanometer Resolution Subsurface Imaging”, Appl. Phys. Lett., Vol. 64, (1994), pp.178-180.


[8] Rabe, U. et al, “High-resolution Characterization of  Piezoelectric Ceramics by Ultrasonic Scanning Force  Microscopy Techniques”, J. Phys. D: Appl. Phys., Vol. 35, (2002), pp.2621-2635.


[9] Yu, H. F. et al, “Distribution and Formation Mechanism  of The Domain Structure in PMN-33%PT Single  Crystals” , J. Phys. D: Appl. Phys., Vol. 37  (2004), pp.  2914-2917.


[10] Abplanalp, M. et al, “Scanning Force Microscopy of  Domain Structures in Pb(Zn1/3Nb2/3)O3-8% PbTiO3 and  Pb(Mg1/3Nb2/3)O3-29% PbTiO3”, J. Appl. Phys. , Vol. 91, No. 6  (2002), pp. 3797-3805.


230


Automated Sample Preparation of Low-k Dielectrics for FESEM


R. R. Cerchiara, H. A. Cook, P. E. Fischione, J. J. Gronsky, J. M. Matesa, A. C. Robins, D. W. Smith


E. A. Fischione Instruments, Inc., Export, PA 15632    Email: rr_cerchiara@fischione.com


E. R. Beach, C. J. Wood, S.J. Rozeveld, J. Waeterloos


The Dow Chemical Company, Midland, MI 48667


Silicon dioxide, which is the basis of the high - k technology  applied to microelectronic materials, has a dielectric constant  of ~3.9 to 4.2.  Introducing fluorine reduces electrical  polarizability and produces a fluorinated silicate glass (FSG). Alternatively, the addition of carbon to the network reduces  ionic polarization and produces an organo-silicate glass (OSG). If the silicon is completely replaced by carbon, an  organic polymer results and k is reduced to less than 2.7. Finally, nanoscale porosity may be introduced into either  organic (C- based) or inorganic (non - C or Si - based) systems to achieve the lowest possible dielectric constant. [1]  The SiLK* TM  resins, composed of aromatic hydrocarbons, are a family of highly cross – linked thermoset polymers with  isotropic dielectric properties.[2]  These resins are cured at  relatively high temperatures, and so exhibit both excellent  thermal stability (> 450oC) and low - k.[3]  Porosity has been  introduced by adding a sacrificial pore - generator (porogen) to the initially deposited film. After annealing, a distribution   of pores is achieved with diameters ranging from  approximately 1 to 3 nm. The dielectric constant of this “Y” generation of the resin has been  reduced to 2.2. [4]


150 nm


Patterning of SiLK* for high aspect ratio copper interconnects  has depended on reactive ion etching with O2/N2 gas mixtures. Selectivity versus silicon oxide, nitride or carbide exceeds  20:1 during the fabrication process with etch rates of 600 – 800 nm/min. Oxidizing plasmas can degrade the critical  dimensions by uneven or preferential removal of  hydrocarbons. Reactive ion etching is therefore also  accomplished with reducing plasmas such as N2/H2. The etch  rates for such gas mixtures range from 300 – 400 nm/min.


Rapid, efficient and automated sample preparation of cross - sections containing high - k dielectrics has been recently  demonstrated.[5] A standard process cycle combines plasma  cleaning (PC), argon ion beam etching (IBE), reactive ion  etching (RIE), and ion beam sputter coating (IBSC) in a single  vacuum chamber. An additional plasma cleaning step can be  inserted after the RIE step, so that any residual contamination  is removed prior to imaging or final sputter coating. This  technique has now been extended to microelectronic materials  that contain low - k dielectrics.


Because of their complex chemistry and low average atomic  number, cross – sectional samples containing such layers often  become damaged when mechanically sectioned or polished. The microstructure of an IMEC# Cu/porous-SiLK* dielectric  resin single damascene wafer after cleaving and plasma  cleaning is shown in Figure 1. The Cu lines separated by the  porous SiLK*Y resin are barely visible below the rough  fracture surface of the Si oxide and nitride layers. This sample  was then processed according to the protocol summarized in  Table 1.  The total processing time was 28.5 minutes.


FIG 1: IMEC Cu/P-SiLK*Y  single damascene wafer after a  cleave and plasma cleaning


TABLE 1: Sample Preparation Protocol for IMEC Cu/PSiLK*Y  Single Damascene Wafer


Step Process  Gas


Time (min.)


PC Ar / 25%O2 5


Removal


of


Hydrocarbon  Contamination


IBE Ar


Planarization


RIE Ar  / CF4 /  CHF3


Selective Etching  of low- k


PC Ar / 25%O2 2


Residue from RIE


After FESEM imaging to assess the uncoated sample surface, a conductive coating of 6 nm of Cr was added in a stand-alone  sputter coater. This processed and coated surface was then reimaged at 10kV and 100kX, Figure 2.


231


# Automated Sample Preparation of Low-k Dielectrics for FESEM


SiCN


SiOx


200 nm


SiLK


SiC


FIG 2: Surface of cross - section after PC + IBE + RIE +PC, followed by coating with 6 nm of Cr


Reactive ion etching of the high - k dielectrics was  accomplished by forming a reactive gas plasma of Ar, CF4 and  CHF3 which was directed perpendicular to the sample surface. Although chemically inert, the energetic Ar ions acted to  break the Si - Si bonds, supplying Si to stabilize SiF4 vapor  formation. Once the CF4 is ionized to CF3, F is released (CF4


+ e-  CF3 + F + e-). This F absorbs and etches Si to SiF4 (Si


(s) + 4F  SiF4 (vapor)). CHF3 is added as a F “deficient” species to enhance the etch selectivity of SiOx with respect to  Si.


Bombardment by Ar ions was also effective in breaking the  relatively weaker hydrogen bonds of the low - k dielectric. When the Ar / O2  ratio is increased in a CH2F2 / O2  / Ar  silicon carbide hard mask etch,  the selective etching of SiLK  trenches has been eliminated.[6] Therefore, the removal of the  low – k dielectric in this case was by physical sputtering  alone.  The action of the Ar ions during IBE and later RIE  also resulted in the decoration of the Cu lines.


Reactive ion etching with Ar / CF4 / CHF3 delineated both the  Si oxide and SiLK*Y resin, and the silicon carbide (and  nitride). No significant amount of RIE residue was detected. Depending on the local gas dynamics and rate of reaction  products of the reaction may not volatize, but remain at the  sample surface. [7] Plasma cleaning with Ar / 25%O2 has been  useful in removing such residue, which when formed on  silicon is a complex fluorocarbon polymer.


Automated sample preparation of microelectronic materials  containing high and low - k dielectrics has been accomplished  by combining plasma cleaning, ion beam etching, and reactive


ion etching.  A single RIE chemistry was effective in etching  both dielectrics as well as delineating the other phases present.


# Sample courtesy of the Inter-University Microelectronics  Center (IMEC), Belgium.


TM SiLK is a trademark of The Dow Chemical Company


[1] C. Case, “Fundamentals of low-k Chemistry”,  Future  Fab International, Vol. 17.


[2] A. L. S. Loke, “Process Integration Issues of Low  Permittivity Dielectrics with Copper for High  Performance Interconnects”, Ph.D. Thesis, Standford  University, 1999, p. 37.


[3] S. J. Martin, J. P. Godschalx, M. E. Mills, E. O. Shaffer II, P. H. Townsend, “Development of a Low  Dielectric Constant Polymer for the Fabrication of  Integrated Circuit Interconnect,” Advanced  Materials, Vol. 23, No. 12, 2000, p. 1769.


[4] R. Strittmatter, J. Waeterloos,  C. Mohler, K. Ender, J. Niu, G. Gavit, B. Landes, R. Hoofman, G. Verheijden, J. Michelon, D. Gidley, H. Peng, “Material Development and Integration of Porous  SiLK Resin with a Microporous Pore Morphology”, Unpublished, 2005.


[5] R. R. Cerchiara, P. E. Fischione, J. J. Gronsky, W. F. Hein, D. D. Martin, J. M. Matesa, A. C. Robins and  D. W. Smith, “Recent Developments in Automated  Sample Preparation for FESEM”, Proceedings of the  29th International Symposium for Testing and  Failure Analysis, Santa Clara, CA, Nov. 2-6, 2003, pp. 288 – 300.


[6] B. R. Murthy, Y. W. Chen, A. Krishnamoorthy, X. T. Chen, “SiLKTM Etch Optmiztion and Electrical  Characterization for 0.13 µm Interconnects”, Microelectronics Reliability, Vol. 45, 2005, p. 507.


[7] S.M. Rossnagel, Handbook of Plasma Processing, Noyes Publications, New York, 1990, p. 207.


232


Depth Measurement of Dislocations in Si Substrate by Stereo TEM


Jong-Shing Bow and Speed Yu


United Microelectronics Corporation, Product Engineering Division, Failure Analysis Department 2, Tainan, Taiwan, ROC  Jongs_bow@umc.com


Dislocations penetrating p-n junctions have been reported to  be paths where leakage occur [1, 2]. Traditional plane-view (P-V) TEM images, which have large fields of view and are  usually used to check the existence of dislocations, cannot tell  whether a dislocation goes through the p-n junction or not. While XTEM images tell the local depth of a small part of a  dislocation only, other methods have to be developed to  explore how a dislocation goes in the substrate. In this work, we modify the technique of stereo TEM, which was used to  study the 3D shapes of precipitates [3, 4], to study how a  dislocation runs in the Si substrate. When an adequate tilting  axis and a reference line are chosen, the depth of dislocations  can be measured accurately.


The sample was first tilted to the [1 0 0] or [1 1 0] exact zone, depending upon which type of wafer was used, to find the  dislocations at device failure sites, and the first image was  recorded. After choosing a suitable reference line to be the  tilting axis as well as the baseline for depth measurement, the  sample was tilted to a two beam condition with g =<1 -1 0> with a tilt angle larger then 10 degrees, and the second image  was recorded. The sample was then tilted in the opposite  direction with the same diffraction condition kept, and the  third image was recorded. These three images are used for  measuring the dislocation depth profile.


Fig. 1  Under focus CBED indicates the tilt direction.


The sense of tilting is easily determined from an under focus  CBED pattern. A typical example is shown in Fig. 1. In the  transmitted disc, a low magnification image of the sample is  observed. The directional relationship of the MOS pattern and  the electron diffraction pattern is then clearly defined.


The distances between a few chosen points on the dislocation  and the reference line were measured from above three  images. Relative depth of each point was then calculated from  the geometry.


Fig.2 TEM micrographs show a MOS with dislocations in the  Si substrate.. (a) BF images at [1 0 0] exact zone, (b) schematic diagram depicts the  nano-diffraction pattern insert  in (a), (c)&(d) BF images with g = [1 -1 0] , but viewed from  the opposite direction


Typical results are shown in Fig. 2. After the MOS structure  above the gate oxide (GOX) is removed, dislocations in the  substrate are clearly viewed. Dislocations have poor contrast  at exact zone diffraction condition (Fig. 2a), but are clearly  visible with a little tilting away from the exact zone and twobeam conditions (Fig. 2c and 2d). The relative projected  distances of dislocations “A” and “B” vary when they are  viewed from two opposite angles. This result indicates that  these two dislocations are at different depths. Three points on  the dislocation A were chosen and labeled “1,” “2,” and “3” as


0 0 4


z = [1 0 0 ]


Exact zone = [1 0 0]


0 2 2


0 4 0


0 0 4   0 2 2


3  2


Tilting direction


c


020


0 2  2


0 2 2  0 0 4


233


# Depth Measurement of Dislocations in Si Substrate by Stereo TEM


shown in Fig.2d. The distances between these points and the  reference line (the red dashed line) are measured in all three  images.


Considering the geometric relationship of L, h, R, θ, and φ in  Fig. 3, we get the formula below:


tanθ = (cosφ1R2 – cos φ2R1)/(sin φ1R2-sin φ2R1)


Since φ1 and φ2 are tilting angles of the TEM sample stage, and R1 and R2 are distances measured from the two tilt images, θ can thus be calculated. Then from the exact zone image, L is  obtained. Finally, h is calculated by the equation below:


h = R tanθ


Fig.3 Schematic diagrams show the relationship among R, L, h, θ, and φ before and after tilting.


Once the depth of those selected points are calculated, the  profile of the dislocation can be drawn by connecting these  points. The profiles of dislocations “A” and “B” are  schematically shown in Figure 4. Then we can know whether  this dislocation penetrates the p-n junction and contributes to  the leakage.


Fig.4  Depth profiles of dislocations in active area.


More examples and a detailed experimental procedure will be  presented in the poster.


The depth profiles of dislocations in the Si substrate can be  determined by stereo TEM.


This work was performed in 2004 at United Microelectronics  Corporation (UMC), FAB 12A, in Tainan, Taiwan, ROC.  The authors would like to thank the company for permission  to publish these data.


[1] Lin, J. C. et al, “Investigation of Substrate Dislocation  Induced Bit Line Soft Failure,” Proc. 30th ISTFA Nov. 2004, pp. 109-114.


[2] Zimmermann, C. et al, “Dislocation induced leakage of  p+-implanted ESD test macros in 90nm technology,” Proc. 30th ISTFA Nov. 2004, pp. 120-125.


[3] Edington, J. W., Practical Electron Microscopy in  Materials Science, Van Nostrand Reinhold Company, (New York, 1976). pp18 and pp.60-63.


[4] Thomas, G. and Goringe, M. J., Transmission Electron  Microscopy of Materials, John Wiley & Sons, Inc. (New  York, 1979), p47-50.


When the N+ implantation is decreased further the doping of  silicon surface is insufficient to form an Ohmic contact. Thus  a supplanted Schottky barrier would dominate the P-N  junction producing a smaller cut-in voltage and larger drift  current.  The corresponding diagram is shown in Fig. 9(b).


Further, if the doping concentration of the N+ region is too  low, the P-N junction will break down easily. This special  phenomenon could be explained by the following formulas.


The depletion layer width is:


N W+×


χ





 +


bi


s


q


2ε


where    :nχ   depletion width of N+ side


:W   depletion width of P-N junction


:biV   built-in voltage


:RV   reverse voltage


Based on the formulas, the junction breakdown occurred  because the depletion layer encroached upon the whole N+ region when reverse biased. The correspondent I-V curve was  shown in Fig. 9(c).


For such a worst implantation case, SCM (scanning  capacitance microscopy) can help to verify the irregular  implant profile at the located site (Fig. 10). And this ability is  the extension application of the SPM [3].


Figure 10:  SCM could verify the irregular implant profile  when the implant was nearly blocked in process.


The aim of our work was to overcome the difficulty in  detecting very tiny or even invisible defects. So a useful  method was developed that could infer the failure mechanism  and the location of defects before conclusive PFA.


The significance of the reasoning method is based on  electrical characterization and differential analysis, unlike  earlier methods which placed undue emphasis on sensitive  resolution SPM current mapping [4]. By coupling PVC with  SPM, the capability to identify tiny defects is not limited to  just distinguishing leakage or high-resistance under contacts


[5].


In the case studies, PVC could detect abnormal N+ contacts  due to improper implanting, and SPM could provide the  precise electrical characteristics. Then combining these two  types of results, different tactics can be adopted to deal with  different states. Thus failure analysis turn-around time would  be shortened and yield-improving strategy could be proposed  as soon as possible.


The kernel of such an approach was not only the practice that  combined with PVC and SPM but also the solid reasoning  based on semiconductor physics and theory of electrostatics. So even if there were multiple suspects or no specific bad  contact could be found, the electric information still could  provide the basis for analysis. Then the failure mechanism  could be reasoned, and the specific defect mode or position  could be deduced.


215


[1] Tctsuya Sakai, Noriaki Oda, Takashi Yokoyama, “Defect  Isolation and Characterization in Contact Array-Chain  Structures by using Voltage Contrast Effect,” 1999 IEEE  International Symposium, 11-13 Oct. 1999.


[2] M. P. Murell, M. E. Welland, S. J. O’Shea, T. M. H.Wong, J. R. Barnes, A. W. Mckinnon, M. Heyns, and  S. Verhaverbeke, “Spatially resolved electrical  measurements of SiO2 gate oxides using atomic force  microscopy” Applied Physics Letters, vol. 62, pp. 786-788.  1993.


[3] Kartik Ramanujachar “ Scanning Capacitance  Microscopy at transistor contact level” Proc. 30th Intl. Symposium for Testing and Failure.


[4] Jone C Lee, C. H. Chen, David Su, J. H. Chuang “Investigation Of Sensitivity Improvement On Passive  Voltage Contrast For Defect Isolation”, ESREF 2002.


[5] J. H. Chuang, Jone C. Lee “Fault Localization In Contact  Level By Using Conductive Atomic Force Microscopy” Proc. 29th Intl. Symposium for Testing and Failure. Analysis, Santa Clara, CA, Nov. 2003, pp. 413-418. 2003.


216


CAD – less Blind Navigation in Focused Ion Beam System


Valery Ray


Particle Beam System and Technology, Methuen, MA, USA  vray@partbeamsystech.com, +1-978-457-6763


Chris Gerlinsky


Titus Consulting, Saskatoon, Canada  chris@nopnop.ca


Traditional approaches to navigation in FIB Circuit Edit (CE)


include blind CAD navigation based on GDSII data from the  manufacturer [1] and navigation assisted by the in-situ Optical  Microscope (OM), either coaxial with the ion beam or not [2]. These two approaches are difficult to apply in security audit  and reverse engineering fields, where CAD data is unavailable  and objects of interest are either too small, or located in an  array that is too dense for imaging by in-situ OM. New  methodology, developed to address this navigational problem, is based on establishing a chip-specific system of coordinates  and determination of precise locations of the objects of interest  within the device. The work was performed on a Vectra 986  FIB system from FEI Company and a proprietary system for  optical scanning of semiconductor devices.


Study of the Device


Initial study of a device with unknown details of internal  functionality requires acquisition of the complete device image  under a high-magnification optical microscope (OM). While  OM images cannot reveal all the details about internal  structure of modern ULSI devices, most building blocks of  digital devices, such as ROM, RAM, EEPROM, CPU core, and many other units can be identified.


Constructing a high-resolution optical image of the device  begins by acquiring, in automated fashion, multiple digital  images under the OM. Acquired images are then correlated, to  compensate for the inaccuracies of the OM stage, and  assembled into the single image file (Fig. 1, as an example) of  the entire device. The image is studied by various manual and  automated techniques and locations of nodes of interest for  contacting are identified. It is often possible to identify  locations of the node of interest, even if the node itself is not  clearly resolved by the optical microscope. It should be  mentioned that sometimes identification of the nodes for  contacting requires more advanced techniques, such as full  device delayering and automated SEM imaging, however


discussion of these techniques are beyond the scope of this  publication.


Figure 1: Image file example of an off-the-shelf device. Actual  image is larger then 1GB and contains sufficient details to  identify functional blocks of the device and (zoom-on in right  bottom corner) even locate nodes of interest for contacting.


Identification of Reference Objects


In addition to the nodes of interest for FIB contacting, reference objects for conversion of the coordinate systems, and  locations of such objects, must be identified on the device


At least three, but preferably four, reference objects are needed  to facilitate conversion of the locations of nodes of interest  from the OM image file of the device to chip-specific  coordinates in the FIB. Highest possible accuracy coordinate – based navigation will be assured if chosen objects conform to  the specific set of requirements. The most critical requirement  for reference objects is that they must be clearly visible and  well resolved under the optical microscope and in the FIB  system. It is also critical for that reference objects surround  location(s) of the target nodes.


217


# CAD – less Blind Navigation in Focused Ion Beam System


Most convenient and frequently used reference objects are  stepper alignment marks, however any other reference objects  conforming to the described criteria would be acceptable.


Bitmap Coordinates


Since the OM image of the device is a rectangular array of  pixels (bitmap), the X and Y pixel numbers naturally become  the Cartesian coordinates of any location within the image.


Chip Navigation in a FIB system.


After the chip is aligned on the sample holder and loaded into  the FIB system with laser interferometer stage, stage  coordinates (X’s and Y’s) of the reference objects can be  determined and correlated with the bitmap coordinates. To  conduct this operation in an automated manner, we enter  bitmap coordinates of the reference objects as “User” coordinates into the “Lock” dialogue of the FIB software. After at least three reference objects are located on the FIB  stage, direct navigation by bitmap coordinates is possible to  any location within the area outlined by the reference objects. Typical accuracy of navigation by bitmap coordinates is in the  single micrometer range and is limited mainly by the  cumulative errors of the OM scanning stage and by coordinate  conversion.


Precision Localisation of Node Coordinates


To determine coordinates of the nodes with the accuracy  sufficient for blind navigation on modern ULSI devices, the  area containing the node of interest is deprocessed by the FIB  on a sacrificial device. Once the node of interest is exposed, “User” coordinates of the node are identified by precision  measurement with the laser stage of the FIB system. Since “User” coordinates are referenced to the device itself, these  coordinates are portable between devices and FIB systems and  can be used for making contacts to the node of interest on  multiple devices.


Enhancements of Navigational Accuracy


FIB software establishes a relationship between the “User” system of coordinates and the physical device, and accuracy of  this relation is inherently dependent on the accuracy of  locating reference objects within the device. While utilizing  edges and corners of the reference objects seems natural for  the operator, it is common that edges of the features printed on  integrated circuit are most strongly affected by the  manufacturing process variations.  In case of the planarized  devices, reference objects should be deprocessed to become  visible in a FIB, and edges of the objects are frequently  damaged during the deprocessing.


Centers of the objects and groups of objects are, however, much less susceptible to the position variations. Automated  location of centers of the reference objects by use of computerbased pattern recognition has been proposed [3] in the past, but it is not commercially available to the most of FIB users. We utilized a manual technique, which was found effective in  improving accuracy of locating reference objects (Fig. 2).


In this technique [4] a group of repair boxes is arranged on the  screen to outline the reference object. Two additional repair  boxes with zero width are placed in the center of the reference  object and the whole group of boxes is saved as a repair file  for future use. During the location process the whole group of  repair boxes is aligned to overlay reference object  symmetrically, thus automatically indicating a precise position  of the center of the pattern.


Figure 2: Box pattern overlay, aligned symmetrically with the  reference object. Interception point of two boxes with zero  width indicates location of the center of the reference, allowing repeatable lock even on damaged reference objects.


Residual errors are inherent to any positioning system, and  practically achievable accuracy of blind navigation with the  laser stage of Vectra system did not exceed ± 150 nm in our  experience.


To overcome residual positioning error problem and  successfully contact nodes in devices with linewidth below  350 nm by blind coordinate navigation, we utilized rectangular  repair boxes instead of traditional squares. In the arrangement  illustrated by Fig. 3 there are horizontal metal lines located  above the vertical line targeted for contacting. Relatively small  navigational errors in Y direction could cause a short between  the nodes, while even significant X direction errors would not  affect results of the contacting. With the available window  between the horizontal lines of 0.5 m, the error budget of ± 150 nm of stage positioning leaves only 200 nm of space  available for via height, if successful contacting is to be  guaranteed. With addition of the safety margin, a repair box  with dimensions of 150 nm X 600 nm provides assurance that  the contact will be successful.


218


Figure 3: Contacting deeper buried vertical node by  rectangular repair box. Safety margin above and below the  box accommodates residual positioning errors in Y direction  to avoid accidental short with the above-the-node horizontal  lines.


We developed and practically utilized methodology for  reliable coordinate-based navigation on integrated  semiconductor devices without CAD data from the  manufacturers. This method utilizes a proprietary system for  scanning integrated circuits under the optical microscope and  standard FIB equipment. Auxiliary techniques allowing  enhancement of navigational accuracy, developed for this  application, are equally applicable to the general navigation  procedures during generic FIB circuit modification (Circuit  Edit).


[1] FEI Company: “ Vectra 986+ Focused Ion Beam System  User’s Guide” , pp 244-260


[2] J.P.Wolpert and R.Lee, "In-situ use of an Optical  Microscope for FIB Microsurgery of Planarized Devices  Proc 25th International Symposium for Testing and  Failure Analysis, Santa Clara, CA, November 1999, pp. 127-133.


[3] Ray, V. et al, “ Small Via High Aspect Ratio Circuit Edit,”  Proc 29th International Symposium for Testing and  Failure Analysis, Santa Clara, CA, November 2003, pp. 355-361.


[4] Private communication. Mr. Alex Krechmer, from FEI  Company, Peabody, MA, is credited for the idea of box  pattern overlay.


219


Method of Detecting Trace Metal Contamination in Thick-Film SOI Device


Yasunori Goto, Hiroomi Eguchi


TOYOTA MOTOR Corporation, Kirigahora, Nishihirose, Toyota, Aichi, Japan  yasunori@goto.tec.toyota.co.jp


Masaru Iida


JAPAN TECSEED Corporation, Maruta, Kariya, Aichi, Japan  miida@nano.tec.toyota.co.jp


In the automotive IC using thick-film SOI (Silicon On  Insulator) semiconductor device [1][2], although metal  contamination is considered as one of the causes of failure, it  is difficult to detect the contamination in a device because of  very minute defect sizes and quantities of contaminant.


A thick-film SOI wafer has the gettering sites that trap heavy  metal impurities, such as Fe, Ni, and Cu, in the SOI layer on  BOX (buried oxide), improving the device yield. However, if  the gettering capability of a SOI wafer is inadequate, electrical  characteristics degradation by metal contamination arises and  the yield falls. At this time, an automotive IC was made  experimentally for evaluation of the gettering capability as  one of the purposes. In this IC, one of the output  characteristics varied from the standard, therefore failure  analysis was performed to find the trace metal elements  considered as one of the causes.


Figure 1 shows a trial production, which consisted of thickfilm SOI semiconductor devices. In detailed evaluation of  electrical characteristics, it is predicted that a leakage failure  occurred within the capacitor shown in Fig. 2.


Figure 1: A trial production consisted of thick-film SOI  semiconductor devices. It shows a predicted failure site in the  box.


Figure 2: Frontside observation predicted leakage failure  within the capacitor located in the box.


Figure 3 shows the backside image  superimposed by the IROBIRCH (Infra Red-Optical Beam Induced Resistance  CHange) [3] response, displaying the leakage current path  within the capacitor. Figure 4 shows the frontside observation  from which the upper wiring layer of the capacitor was  removed. As a result, it is found that it is difficult to localize  the leakage current path from the surface side.


Figure 3: Backside observation superimposed by IR-OBIRCH. Localization of leakage current path is displayed in the circle.


Figure 4:Frontside observation removed upper layer.


Then, marking lines are placed around the leakage point by  FIB (Focused Ion Beam) method, as shown in Fig. 5. A  leakage current path


10µm


leakage point


# Method of Detecting Trace Metal Contamination in Thick-Film SOI Device


micro-sample is picked up and mounted on a 3D (three  dimensional) specimen holder [4][5][6], as shown in Fig. 6. By making full use of 360-degree rotation and ±15-degree tilt  functions of the 3D holder, it is possible to fabricate a thinfilm of the micro-sample with sufficient accuracy, without  missing a leakage point. As a result, it is found that there is  the difference of 0.5µm between the original marking position  and the final thin-film position which processed the leakage  point into 0.1µm in thickness, as shown in Fig. 7. The  procedure is explained next.


Figure 5: Marking lines placed around the leakage point by  FIB.


Figure 6: A micro-sample picked up and mounted on the 3D  holder.


Figure 7: Final thin-film fabricated by FIB. It shows a  difference of 0.5µm between the marking line position and the  final film position.


As shown in the SE (Secondary Electron) cross-section image  of Fig. 8 by STEM (Scanning Transmission Electron  Microscope) method, when the micro-sample was thinned  from both sides into 1.4µm in thickness on the basis of the  marking lines, a failure point was exposed to one side, and the  size was 0.35µm. As shown in the TE (Transmission Electron) cross-section image of Fig. 9 by STEM method, it could be


predicted that failure site is spherical in shape, and the size  was 0.5µm. The top view that estimated the position of the  failure point inside the micro-sample of 1.4µm in thickness is  shown in Fig. 10.


Figure 8: SE cross-section image of 1.4µm in thickness.


The observed failure point is 0.35µm in size.


Figure 9: TE cross-section image of 1.4µm in thickness.


The observed failure point is 0.5µm in size. The failure site is  predicted to be spherical in shape.


Figure 10: Top view of the micro-sample of 1.4µm in  thickness. The position of the failure point is estimated inside  that.


Based on this result, the micro-sample was thinned from one  side to 0.7µm in thickness. By rotating and tilting the 3D


marking line


micro-sample


3D holder


1µm


difference of 0.5µm  marking line position


final film position


(0.1µm in thickness)


failure point


0.35µm


0.5µm


1.4µm


221


holder appropriately, it is found that the micro-sample could  be observed transparently from a slanting direction, as shown  in ZC (Z Contrast) cross-section image of Fig. 11 by STEM  method. Moreover, in the TE cross-section image shown in  Fig. 12 it became clear that the failure form is a spherical  shape as predicted. Figure 13 shows the micro-sample top  view of 0.7µm in thickness.


Figure 11: ZC cross-section image of 0.7µm in thickness.


Failure point is observed from a slanting direction by rotating  and tilting the 3D holder. Failure form is proved a spherical  shape.


Figure 12: TE cross-section image of 0.7µm in thickness.


Figure 13: Top view of the micro-sample of 0.7µm in  thickness.


Based on this result, the micro-sample was thinned from both  sides to 0.1µm in thickness, as shown in ZC and TE crosssection images of Fig. 14, 15 respectively. Figure 16 shows


the micro-sample top view of 0.1µm in thickness. As a result, it is possible to thin into 0.1µm in thickness without missing a  leakage point.


Figure 14: ZC cross-section image of 0.1µm in thickness.


Figure 15: TE cross-section image of 0.1µm in thickness.


Figure 16: Top view of the micro-sample of 0.1µm in  thickness.


Figure 17 shows an EDX (Energy Dispersive X-ray) analysis  point (black mark in the figure), and Fig. 18 shows the  spectrum obtained on the final thinned micro-sample of 0.1µm  in thickness with a probe diameter 1nm. It is found that only  Ni was detected as metal contamination, because Cu and Zn  are holder materials.


spherical shape


0.7µm


0.1µm


222


Figure 18: EDX data with the probe diameter 1nm. It shows  detected Si, O, and Ni (C: contamination, Cu and Zn: holder  materials, Ga: FIB ion source).


The quantitative analysis shows that Ni is 0.19% in the  number ratio of atoms, as shown in Table 1.


Table1: Quantitative Analysis.


Element Counts Wt % Atomic % Si-K


24261 89.90


83.98


O-K


1116


9.64


15.81


0.43


0.19


Therefore, the detected Ni becomes 7.5 atoms, if it is assumed  that the excited volume is a cylinder of diameter 1nm and   height of 100nm and the measured Ni concentration is  converted with that of Si atoms as shown in Fig. 19. If it is  assumed that the Ni atoms exist in the maximum plane (100nm2) intersecting the cylinder, the concentration of Ni  contamination is calculated to be 7.5e12atoms/cm2.


Fig.19 Analyzed shape and the number of conversion.


Since this amount of contamination is a level that affects the  electrical characteristics of a semiconductor device [7], it  becomes clear that the gettering capability of this SOI wafer is  inadequate. Therefore, the wafer manufacturing process was  improved.


By making full use of 3D perspective, it is possible to  fabricate a site-specific sample into 0.1µm in thickness,


without missing a failure point that has very minute quantities  of contaminant in a semiconductor device. Moreover, using  EDX, it is possible to detect trace metal contamination at  levels 1E12 atoms/cm2 that are conventionally detected only  by trace element analysis, such as ICP-MS (Inductively  Coupled Plasma-Mass Spectrometry), AAS (Atomic  Absorption Spectrometry), and TRXF (Total Reflection X-ray  Fluorescence).


I would like to thank Jiro Sakurai, Tomoki Nakazawa, and  Tomonori Hayamizu for their technical support, and I would  also like to thank Yuko Ota, Ayaka Taniyama, and Yusuke  Sekiya for their daily operations.


[1] T. Fujikawa, “Semiconductor technologies support new  generation hybrid car,” Symposium on VLSI Circuits, Jun. 2004, pp. 6-9.


[2] M. Hattori, F. Ito, M. Kako, “A very low on-resistance  SOI BiCDMOS LSI for automotive actuator control,” IEEE International SOI Conference, Oct. 2004, pp. 171-173.


[3] K. Nikawa, S. Inoue, K. Morimoto, S. Sone, “Failure  Analysis Case Studies Using the IR-OBIRCH (Infrared  Optical Beam Induced Resistance CHange) Method,” Eighth Asian Test Symposium (ATS'99), pp. 394-399.


[4] M. Koguchi, H. Kakibayashi, R. Tsuneta, et al, “Threedimensional STEM for observing nanostructures,” Journal of Electron Microscopy, Vol. 50, No. 3 (2001), pp. 235-241.


[5] T. Yaguchi, et al, “A FIB Micro-Sampling Technique for  Three-Dimensional Characterization of a Site-Specific  Defect,” Microscopy Today, Vol. 12, No. 6 (2004), pp. 26-29.


[6] K. Mcllwrath, N. Wang, “A Novel FIB method to prepare  TEM samples for 3D observation,” Proceedings of the  30th International Symposium for Testing and Failure  Analysis, Nov. 2004, pp. 320-323.


[7] J. Wang, P. Pianetta, K. Baur, S. Brennan, “Analytical  Techniques for Trace Elemental Analyses on Wafer  Surfaces for Monitoring and Controlling Contamination,” 19th Annual Semiconductor Pure Water and Chemicals  Conference, Mar. 2000.


Si atoms: 5e22(atoms/cm3) Analysis volume: 25π(nm3)∴ Detected Ni: 7.5atoms


1nm


metal contamination


Figure 17: EDX analysis point.


analysis point


223


The Radio Probe™


A New Measurement Tool for High Speed Integrated Circuits


Mark Kimball


Maxim Integrated Products  mark_kimball@or.mxim.com


A new tool designed to allow circuit node measurements in a


Radio Frequency (RF) integrated circuit (IC) will be  presented.  Our cost effective solution incorporates features  that make it well suited to the task of differential measurement  of circuit nodes within an RF IC.


The Problem


Probing the internal nodes of RF integrated circuits presents  unique challenges that are not well served by current probe  technology.  Passive probes can have very high frequency  response but their input impedance is typically between 500  and 1000 ohms, with an attendant high attenuation factor from  10:1 to 20:1.  Because internal circuit nodes of RF ICs can  have relatively high impedances, passive probes can  significantly load the circuit node being probed, greatly  altering the measured AC voltage.  State of the art active  probes currently have frequency responses up to 26 GHz and  input capacitance of 0.05 pF, but our experience with this type  of probe has shown that its frequency response is not very flat.  In addition, RF circuit problems are often related to parasitic  oscillations or poor frequency response, so spectrum analyzers  are needed in addition to the high frequency probe or passive  probe.  A state –of –the art commercially available 26 GHz  active probe currently costs approximately US$6000 for a  single probe.  Spectrum analyzers can cost US$20,000 and  high speed digital oscilloscopes can easily cost US$60,000 or  more, if refurbished units are not available.  If a number of RF  IC failure analysis stations must be equipped, costs can  quickly mount.


An additional problem not addressed by any of the currently  available IC active probes is the measurement of differential  signals.  Single ended measurements using an external ground  reference will contain common-mode as well as differentialmode signals, so single ended measurements are inherently  inaccurate.  And accurate differential mode measurements of  internal RF IC circuit nodes at GHz frequencies have not been  demonstrated in the past.


Theory of the Design


The Radio Probe is, in essence, an RF receiver with a passive  attenuator rather than an antenna at its input.  See Figure 1 for  a block diagram of the prototype design.


The Radio Probe avoids the need for an expensive spectrum  analyzer or high speed oscilloscope because it downconverts  its input to a low frequency signal that can be easily measured  using a low-frequency oscilloscope or DVM.  A relatively  inexpensive RF generator is used to supply the local oscillator (LO) input to a broadband receiver located near a probe tip, hence the name "Radio Probe".  The receiver output level is  proportional to the input RF voltage.  Because the probe has  high gain (60 dB or more), this gain can be exchanged for  high input impedance and resultant low loading factor.  High  gain broadband receivers can be built using off the shelf  components at relatively low cost compared to commercially  available active probes.  This will be illustrated later in this  paper.  The resistive (i.e. real) component of the input  impedance has some additional advantages.  An inevitable  drawback of active probes is current flow into their input  capacitance.  This current must flow back into the circuit  being probed, usually through some type of inductive circuit, either through an extended ground return or through a clip  lead attached to the device under test.  The input capacitance  of the probe, combined with the parasitic inductance of the  return connection results in a series resonant circuit that has  highly variable impedance near resonance.  Placing a large  passive resistance in series with this resonant circuit “kills” the Q of the parasitic tank circuit, flattening its response.  This  phenomenon is one of the reasons that passive probes with  attenuation factors of 10:1 or 20:1 are popular, despite their  low input impedance and high attenuation factor.
  Our  solution employs the same Q-killing feature, but uses a much  higher input resistance because its gain is high enough to  compensate for the attenuation factor.  The design presented  here achieves an input impedance of 50Kohms and an overall  attenuation factor of 0 dB.


Differential Measurements


Internal RF IC signals often are differential in nature, so  single ended measurements can have significant errors.  This


224


# The Radio Probe Probe A New Measurement Tool for High Speed Integrated Circuits


is because the single ended measurement contains both  common mode and differential mode signals.  To address this  issue, the Radio Probe design offers a way to perform  differential measurements.


It is well known that phase differences at the input of a mixer  will result in phase differences at the mixer output.  This is the  basis of quadrature encoding and decoding.  Probing  differential signals with a pair of radio probes will result in a  combination of common mode signals and differential mode  signals at a lower frequency.  If the phase differences of the  Local Oscillator (LO) inputs to both radio probes is zero, the  probe outputs  will contain the same common mode and  differential mode signals as the inputs, but downconverted to a  much lower baseband frequency.  This lower signal frequency  facilitates the extraction of the differential and common mode  signals, using either analog or digital techniques.  This idea is  complicated by the fact that the LO signal path to both radio  probes must have the same path length in order to minimize  the phase error. However, path length errors can be  characterized and calibrated out at the mixed down frequency  rather than the original RF frequency.  This technique offers  the possibility of making true differential-mode measurements  on RF IC circuit nodes over a wide frequency range, at  relatively low cost.  Figure 2 shows two Radio Probes being  used to perform a differential measurement on an RF  integrated circuit.


Practical Implementation of the Radio Probe


The prototype probes were constructed using off-the-shelf RF  amplifiers and mixers for the high frequency side, and  inexpensive video amplifiers for the low frequency (or "baseband") side.  The output bandwidth was set to a  maximum of 75MHz using an RC low-pass filter. Low-offset  operational amplifiers were used for the offset-nulling circuit.  The design operates using +/-5V supplies and draws  approximately 100 mA per probe.


Signal to Noise Issues


The basic Radio Probe concept is not without drawbacks.  One major issue is the fact that the probe requires high gain to  offset its high input impedance.  This degrades the Signal to  Noise Ratio (SNR) of the output signal.  This can be a  problem when attempting low level signal measurements.  But  improvements can be made in this aspect as well, using a  digital sampling oscilloscope (DSO).


SNR Improvement


It is well known that amplitude modulating a signal produces  sidebands at the sum and difference frequencies of the carrier  and modulator.  This amplitude modulated signal comprising  the carrier and upper and lower sidebands would be the input  to the Device Under Test (DUT).  If we use an unmodulated  RF signal as the LO input to our probe, its output will be the  same frequency as the low frequency modulation signal, with  added noise.  Averaging the signal with the DSO will produce  an output with a greatly improved SNR because the noise  averages to zero, while the desired signal “builds up”.  Such


With the traditional TEM observation method, diffraction  mode is employed to tilt the sample to the <110> crystal  orientation, because all IC patterns are deposited on the (001) crystal face and the (001) crystal face is normal to the (110) crystal face. In this case, the layer thickness measured from  the cross-section TEM image is accurate. Under this  condition, the sample has to be tilted to the (110) crystal face. The TEM image is shown in Figure 3. The silicide on the  Active Area (AA) is as dark as the substrate and the interface  is blurred.


It can be seen that the interface between the silicide and  substrate single crystal silicon is not distinguished clearly. Consequently, it is difficult to measure the thickness of the  silicide accurately. In order to observe the silicide layer  clearly and measure the thickness accurately, a novel method


239


# A Novel Method to Observe Silicide in TEM


is put forward to change the contrast of the single crystal  silicon substrate. The method is that the cross-section TEM  sample is tilted 3 degrees along the <400> crystal orientation. Using this method, the TEM images shown in Figure 4 were  obtained from the same TEM sample. In comparison with the  images in Fig 3, the TEM images with higher contrast can be  observed in Figure 4., The AA area shown in Figure 4 is  brighter than that shown in Figure 3.


Figure 3. Traditional X-section TEM images, the incident  electron beam direction is normal to the substrate single  crystal silicon (110) crystal face (the process is after contact  etch).


Shown in Figure 4 are the clear TEM images acquired with  this method. A clear interface is exhibited in the images. However, it needs to be verified that the thickness obtained  after tilting is the actual thickness. When the sample is tilted, the silicide cross section is perpendicular to the tilting plane, namely, the X-Z plane shown in Figure 2. Therefore, the  silicide thickness is constant regardless of the tilting angle  along <400> orientation.


Figure 4. The X-section TEM images after tilting the samples  along the <400> crystal orientation.


Due to the fact that substrate of wafer is the single crystal  silicon, the <400> crystal orientation can be easily determined


using Kikuchi line pattern [7]. The <400> crystal orientation in  the Kikuchi pattern is the widest and strongest one in all  Kikuchi lines, as shown in Fig 5. After locating the <400> crystal orientation, we first tilt the sample about 3 degrees  along this direction. Next, the objective aperture is used to  capture the main transmitting spot in the aperture center. Finally, we switch TEM to the image mode to get images. In  this way, the substrate contrast can be manipulated.


Silicide


<400>


Single crystal silicon substrate


Figure 5. the Kikuchi line in the diffraction mode. The blue  marked direction is the single crystal silicon <400> orientation


Using the novel method we developed, a clear interface  between the silicide and substrate single crystal silicon can be  obtained without affecting the accuracy of the measured  silicide thickness.


[1].Shi-Li Zhang.et al “Metal silicide in CMOS


technology: past, present, and future trends”     Critical review in Solid State and Materials science,


Vol. 28, No. 1 (2003), pp1-129.


[2].Tatsuya Ohguro. et al “Thermal stability of CoSi2  film for CMOS salicide IEEE journal of Transactions


on electro devices”, Vol. 47, No. 11 (2000), pp2208-


2213.


[3].Key-min Lee et al . “N+/P junction leakage  characteristics of salicide process for 0.15µm CMOS  device” IEEE journal of Transactions on electro  devices, Vol. 49, No. 5 (2002), pp937-939


[4] C.Y. Lin. et al. “Formation of Ni Germano-silicide on  single crystalline Si0.3Ge0.7/Si”, IEEE journal of  Electron Device Letters,  Vol. 23, No. 8 (2002), pp464-466.


[5] Stanley Wolf.   Silicon Process For the VLSI Era  Volume 4: Deep-submicron process technology (Lattice Press 2002), pp603-635,.


[6] Yu Zhou. material analysis method (China machine  press 2000), pp74-129,.


[7] Jin sheng Pan, Jian min Gong, Min bo Tian. The  fundament of material science, (Tsinghua university  press 1998), pp77-83,.


240


The Enhancement of Abnormal Photon Emission Identification for


Advanced Processes using a Backside Cooling PEM System


C. H. Wang, S. W. Lai, Z. H. Lee, J. H. Chou


1,Nan-Ke N, Rd., Tainan Science Park Tainan, Taiwan 741-44, R. O. C.


Phone: (886)6-5059688Ext.7068605   Fax: (886)6-5052007   Email: jhwangf@tsmc.com


As manufacturing technology allows semiconductor feature  size to shrink, the operating current maximum allowable  device leakage is reduced. Because of this, it is more  difficult to differentiate abnormal photon emission spots  from normal emission spots on more advanced devices, especially 0.13um and smaller process technologies. The  sensitivity of a photon emission microscope (PEM) is not  sufficient to differentiate the abnormal photon emissions  from normal device leakage emissions. In addition, high  chip temperature makes device leakage emissions more  prominent. This paper will present the principle of weak  photon emission inspection enhancement and the  development of a backside cooling system based on the  present PEM. It is an efficient and economical way to  localize failures based on the present PEM. The enhanced  PEM tool stabilizes the chip current and operating  temperature to lessen the emissions due to normal device  leakage using a backside cooling system.


Photon emission microscopy is currently an important and  widely applied method to localise semiconductor failures. The methodology makes use of the differences in emission  strength between abnormal and normal spots on the chip. Emission strength at a defect spot is usually significantly  stronger than the normal device leakage emission; defects  can thus be easily identified on the PEM image. However, in  recent chip designs the chip current and operating  temperature of the chip are higher. The higher temperature  results in stronger background emissions making the failure  spot less distinguishable.


Figure 1(a) and (b) show the PEM images of two chip  samples whose chip currents increase over time. No obvious  abnormal photon emission spots can be recognized by  comparing them with their good counterparts. Consequently, much more effort must be taken to pinpoint  the defect. Diagnostics such as analog power biasing, I/O  power biasing, dynamic photon emission inspection, etc. might have to be carried out. Additional labor and other


introduced costs might make these extensive measurements  uneconomical, and sometimes even impractical.


Figure 1: Ordinary emission inspection on two different  chips, (a) sample A: integrated 180s while biased with 2.2V  resulting in a chip current of 200mA., (b) sample B: integrated 180s while biased with 2.3V resulting in a chip  current of 230mA


This paper presents an economical and effective cooling  system applied on the PEM setup that can significantly  enhance the abnormal emission detection capability in new  advanced process chip designs. We will begin with a  discussion of the origin of normal and abnormal photon  emissions in a semiconductor chip. Then, the design of the


241


# The Enhancement of Abnormal Photon Emission Identification for Advanced Processes using a Backside Cooling PEM System


backside cooling system will be presented. At last, the  advantages of the improved system are demonstrated.


Phenomenon and Physical Principles


When operating the PEM, photon detector images usually  have to be integrated over a period of time to make the  abnormal emission sites intense enough to be identified. Normally, a longer integration time takes advantage of the  multiplying effect caused by the stronger emission at the  abnormal spot that makes the spot more distinguishable. On  the contrary, we reveal in the following case that the longer  the PEM image was integrated, the less distinct the emission  image appeared. This is probably due to the rapid increase  of the chip current that leads to high operating temperature  in the device and more importantly, stronger background  emissions. The temperature of the chip constantly registered  above 340K during the inspection process.


Physically, the background emission originates from the  heat induced by the operating power of the chip. The  increased temperature alters some temperature dependent  device parameters such as the threshold voltage of NMOS  and PMOS. When the temperature increases the threshold  voltage of NMOS decreases and that of PMOS increases (figure 2) [1]. As a result, the device can be switched on  more easily. Meanwhile, higher total chip current flows at  the same bias voltage (figure 3.).


Figure 2. Temperature dependence of threshold voltage


Figure 3. Temperature dependence of chip operation  current at VDD=2.52V on three samples


The impact ionization of hot electrons on the drain node is a  major source of photon emission [2]. The intensity of the  emission depends on two key variables: source-drain


current and electric field near the drain node. Normal device  leakage emission from the source-drain current increases  with chip temperature, registering more photons on the  integrated emission image. Unfortunately, photons emitted  by the defects such as gate oxide pinholes, metal  interconnection shorts, or floating gates have very weak  temperature dependency (figure 4.) [1]. Thus, it becomes  more difficult to recognize abnormal emission sites at  elevated chip temperature. Chip cooling becomes necessary  in this case to suppress the normal background emissions so  that abnormal emissions can be spotted in the integrated  PEM images [4] [5] [6] [7].


Figure 4. Temperature dependence of normal and abnormal  gate leakage current in MOSFETs


Backside Cooling System Design


We designed a backside cooling stage that can be integrated  into our present PEM to replace the standard iron plate stage (figure 5). The design incorporates sample trenches with  mounting screws to make the sample stable when cooled (figure 6a). There are four channels for flow of nitrogen gas  through the stage (figure 6b). Although we applied gaseous  nitrogen, liquid nitrogen can also be utilized if necessary for  enhanced thermal exchange. This indirect cooling method  not only makes the temperature controllable but also  prevents the temperature from dropping too fast.


Figure 5. The backside cooling system setup on the PEM


242


Figure 6. The design detail of the backside cooling system: (a). The design for stabilizing the sample on the backside  cooling system with sample trenches and screws, and (b) The N2 gas channels and connecting pipes.


Figure 7 compares the chip currents with and without  backside cooling. Results for both gaseous and liquid  nitrogen cooling are shown. Without cooling, the chip  current goes up from around 250mA initially to  approximately 350mA in 120 seconds. When gaseous  nitrogen cooling was applied, no significant chip current  increase was observed. Liquid nitrogen cooling further  decreased and stabilized the chip current.


Figure 7. Comparison of chip current over a period of 120  seconds with gaseous N2 cooling, liquid N2 cooling, and no  cooling. The beneficial effects of backside cooling are  clearly evident.


Abnormal Emission Localization and Failure  Analysis Results


PEM images of the samples of figure 1 were reacquired after  the backside cooling stage was installed (figure 8) The  abnormal emission spots have become more distinct. It is  now simpler to analyze the failure from the solid abnormal


emission, especially if it is the result of a leakage defect on  the front-end.


Figure 8. Low temperature photon emission inspection of  the two samples of figure 1. In this case, abnormal emission  spots are observed, (a) sample A: integrated 180s while  biased with 2.2V. The chip current is stable and one  abnormal emission spot (circled) is observed, and (b) sample B: integrated 180s while biased with 2.3V. The chip  current is also stable and multiple abnormal emissions (circled) are easily observed.


With the improved PEM images, abnormal emission spots  can be more dependably identified. Consequently, less  effort has to be made to localize the defect in the circuit. In  particular, soft and invisible defects like the poly leakage  and gate oxide pinholes induced by the antenna affect are  very difficult to pinpoint without the backside cooling stage. For example, after identifying the abnormal emission  locations in the samples of figure 8, de-layering and voltage  contrast examination revealed a pinhole on the abnormal  emission spot of sample A. For sample B, FIB milling


Trench for fixing sample   Screw for stabilizing sample


N2 gas


Gas out


243


revealed tungsten and copper extrusion below metal 1 at the  location of the multiple abnormal emission spots.


Figure 9. (a) A pinhole was found in sample A on the  channel (circled), and (b) Tungsten and Copper extrusion  through ILD (circled).


A simple and low cost PEM backside cooling system was  designed and fabricated. The cooling stage has proven to  effectively lower the chip current to minimize the  temperature dependent normal leakage emissions so that the  temperature independent abnormal emission spots can be  more easily detected. After applying the cooling stage to  various chips, the success rate of emission inspection  increased by approximately 50%. At the same time, failure  analysis execution time is significantly shortened. The  backside cooling system can be easily integrated into  present PEM systems.


Although diagnostic software has recently been popularly  applied to localize failures, it simply reports all possible  candidates as the source of a malfunction. However, verifying all of these possibilities requires tremendous  effort. On the other hand, PEM with backside cooling can  help localize the source of the failure, will be a simple, effective, and reliable tool for localizing failures in future  chips fabricated with advanced manufacturing processes.


[1] Masakazu Shimaya, “New Screening Concept for Deep  Submicron CMOS VLSIs Using Temperature  Characteristics of Leakage Currents in MOS Devices”,


IEEE 35th Annual International Reliability Physics  Symposium, 8-10 April 1997, pp. 49-56.


[2] B.Marchand , D. Blachier , C. Leroux , G. Ghibaydo , F. Balestra , and G.Reimbold, “Generation of Hot Carriers  by Secondary Impact Ionization in Deep Submicron  Devices: Model and Light Emission Characteristics”, IEEE 38th Annual International Reliability Physics  Symposium, San Jose,California, 2000, pp 93-97.


[3] Toshiaki Tsuchiya , Shigeru Nakajima “Emission  Mechanism and Dias-dependent Emission Efficiency  of Photons Induced by Drain Avalanche in Si  MOSFETs”, IEEE Sournal of Solid State Circuits, vol. SC-20, No. 1, Feb. 1985, pp. 325-332


[4] Y.Y. Liu, J. M. Tao, D. S. H. Chan, J. C. H. Phang, and  W. K. Chim “A New Spectroscopic Photon Emission  Microscope System for Semiconductor Device  Analysis”, Proceedings of the 5th International  Symposium for Physics and Failure Analysis of  Integrated Circuits, 27 Nov. 1 - Dec. 1995, pp. 60-65.


[5] F. H. Gaensslen, V. L. Rideout, E. J. Walker, and J. J. Walker, “Very Small MOSFET’s for Low-Temperature  Operation”, IEEE Transactions on Electron Devices, vol. Ed-24, No. 3, Mar. 1977, pp. 218-229.


[6] J. S. T. Huang, J.W. Schrankler, “Switching  Characteristics of Scaled CMOS Circuits at 77K”, IEEE Transactions on Electron Devices, vol. Ed-34, No. 1, Jan. 1987, pp. 101-106.


[7] Rama R. Goruganthu, David Bethke, Shawn McBride, Tom Crawford, Jonathan Frank, Dan Cotton, Tahir  Cader, “Spray Cooling for Time Resolved Emission  Measurements of ICs” Proceedings of the 30th  International Symposium for Testing and Failure  Analysis, November 14-18, 2004 Worcester, Massachusetts USA. pp. 18-23.


[5] Watt, I. M. The principles and practice of electron  microscopy, Cambridge University Press, (New York, 1997). Pp238-254.


eImage


h


R1


φ1


(a


(b


- +


249 nm


262 nm    147 nm


532 n m


234


Gate Oxide Defect Localization and Analysis by Using Conductive Atomic  Force Microscopy


Z. H. Lee, C. J. Lin, S. W. Lai and J. H. Chou


1, Nan-Ke N. Rd. Science Park, Shan-Hua Tainan, Taiwan 741-44, R.O.C.


This paper describes gate oxide defect localization and  analysis using Passive Voltage Contrast (PVC) and  Conductive Atomic Force Microscopy (C-AFM) in a real  product. If the defect exists on the gate oxide, the PVC  image of the contact/via connected to poly gate will become  brighter. Bright PVC image indicates that there is a leakage  path, but determination of the leakage path is not possible.  The C-AFM current mapping is more sensitive than PVC. Combining current mapping with an I-V curve, we can find  the leakage path including gate oxide leakage, junction  leakage, poly contact shorted to other contacts (poly, N+ or  P+ contacts), and so on. For gate oxide leakage, gate oxide  pinholes are exposed by using KOH wet etching in this  paper.


The trend of semiconductor technology is towards high  component density and small device dimensions. As the  technology continues to scale down, defect size tends to  decrease and non-visible defects such as crystal defect, gate  leakage and junction leakage will become important root  causes. Defect isolation has become more difficult.


Conductive atomic force microscopy (C-AFM), with  non-meter scale lateral resolution and the ability to measure  the current in pico-amp range, has been widely used for  semiconductor failure analysis (FA). In this experiment, Digital Instruments CP Ⅱ is used for the measurement. The  schematic is shown in Figure 1. The tip of C-AFM scans  over the sample and images a current map. In general, current mapping is more sensitive than PVC image, but may  not show obvious defects. An analysis to compare the I-V  curve of individual contacts is powerful and helpful for FA.


PVC is widely used in proceeding Physics Failure  Analysis (PFA). At the contact layer, a bright PVC image of  poly contact indicates there is a leakage path which may be  due to gate leakage, junction leakage, short to N+/P+ contact, and so on. However, the path the leakage current goes  through according to the PVC image can not be confirmed. Combining PVC with C-AFM current mapping and I-V  curves will increase the successful rate to find the front-end  leakage mode defect.


Wet etching is usually used to remove poly-silicon for  gate oxide integrity. KOH, TMAH, choline hydroxide are  popular etchants due to controllable etching rate and high  poly-silicon /SiO2 selectivity [2]. In this paper, 10% wt  KOH was used to etch poly-Si and expose gate oxide.


Figure 1: A schematic of Conductive Atomic Force  Microscopy.


Case study Ⅰ


In this case study, the specimen is manufactured using a  standard 0.13um CMOS process. Failure location is  determined by photoemission microscopy (PEM). After  de-layering, PVC imaging showed a brighter via connection  to poly gate, but no defect was found at inter-connect metal. The specimen was parallel lapped to contact layer and a  bright PVC image of the corresponding contact was  found(Figure 2).


Figure 2: The PVC image of contact layer. Bright PVC  image of the contact connected to poly gate indicates there  is a leakage path on the contact.


The bright PVC image implies that there is leakage from  the contact through a gate oxide, junction leakage, poly  contact shorted to other contacts (poly, N+ or P+ contacts) or


235


# Gate Oxide Defect Localization and Analysis by Using Conductive Atomic Force Microscopy


poly residue. However PVC imaging can’t provide enough  information to determine the real leakage path. Therefore  the specimen is imaged using the C-AFM. Figure 3 shows  the current map with brightness levels matched with the  previous PVC image.


Figure 3: The current map matched the previous PVC  image. It shows failed poly contact with brightness levels.


From the I-V curves (shown in Figure 4), the behaviour  of failed poly almost matches the one for Vss. However we  can’t distinguish if this poly short is to the Vss contact or  gate oxide leakage. After determining that a short to the Vss  contact was not likely, a gate oxide pinhole was suspected. The poly gate was etched with KOH after removal of the  salicide on the poly gate. SEM inspection revealed a gate  oxide pinhole (Figure 5).


The leakage path passed through the gate oxide pinhole, LDD, S/D and sailicide to Vss node (Figure 6). Compared  with Vss curve, the resistance of leakage path can be  ignored. Therefore the I-V curve of the failed poly nearly  matches the Vss curve.


Figure 4: These I-V curves show that the failed poly curve  nearly matched Vss curve.


Figure 5: A gate oxide pinhole was found after removal  poly-Si by KOH wet etching.


Figure 6: The leakage path passes through the gate oxide  pinhole, LDD, S/D and salicide to Vss node.


Case study Ⅱ


PVC images of a second sample shows bright poly  contacts at the contact layer (Figure 7). The C-AFM current  map revealed the same bright failed poly contacts as well (Figure 8).


Figure 7: The PVC image of the contact layer revealed  possible leakage on  poly contact A and B.


Fail poly


Adj. N


Adj. Vss


Vss


Failed poly A


Failed poly B


236


Figure 8: The C-AFM current map revealed brightness on  the same failed poly contacts.


The I-V curve of failed poly contact A is shown in  Figure 9. The literature indicates if corresponding source or  drain  (adjacent N+) I-V curve shows an early junction  breakdown at a negative bias region, a gate oxide short to  the corresponding S/D will be the cause of this failure [3]. The early junction breakdown is probably caused by slight  LDD damage when gate oxide breakdown occurred at the  S/D side.


Figure 9: The I-V curves indicate the corresponding S/D (adjacent N+A) has an early junction breakdown  phenomenon in negative bias region. The early junction  breakdown is probably caused by slight LDD damage when  gate oxide breakdown occurred at S/D side.


The I-V curve of the failed poly contact B is shown in  Figure 10. According to the I-V curve, it’s not shorted to the  N+ contact due to the mismatching curves of the failed poly  and N+ contact.  The literature indicates that gate oxide  breakdown will only occur at the S/D side but not at the  channel [4]. The I-V curves of the corresponding S/D (adjacent N+ B1 and B2) shows no earlier junction  breakdown at negative bias region. The gate oxide pinhole  should be in the channel but not the S/D side. The leakage  path passes through the gate oxide pinhole to S/D N+ contact (Figure 11). The shift of I-V curve is due to the resistance of  leakage path.


Figure 10: The I-V curves indicate the corresponding S/D (adjacent N+ B1 and B2) has no early junction breakdown  phenomenon in the negative bias region. Therefore, a gate  oxide pinhole should be in the channel but not at the S/D  side.


Figure 11: The leakage path A passes through gate oxide  pinhole, LDD to N+ node. The leakage path B passes  through gate oxide pinhole to the N+ node.


After removing poly-Si by KOH wet etching, gate oxide  pinholes for the failed poly A and B were found at the S/D  side and channel respectively (Figure 12).


Adj. N+ A


Adj. N+ B1 and B2


Early breakdown


A B


237


Figure 12: After removing poly-Si by KOH wet etching, gate oxide pinholes of the failed poly A and B were found at  the S/D side and channel respectively.


In these case studies, different types of gate oxide  defects will cause different leakage paths. According to the  I-V curve measured by C-AFM, we can distinguish between  short mode and gate oxide related leakage. For gate oxide  leakage, KOH wet etching was successfully used to identify  the gate oxide pinholes.


[1]  Jon C. Lee and J. H. Chuang, “Fault localization in  contact level by using conductive atomic force  microscopy”, Proceedings of the 29th International  Symposium for Testing and Failure Analysis 2003.


[2]  C. Smith, K Symond, “Novel Deprocessing Techniques  to Analyze Gate Level Defects”, ISTFA 95Proceedings, pp. 275~278(1995).


[3] Cheng-Piao Lin, Cheng-Hsu Wu and Cheng-chun Ting, “A novel electrical test by C-AFM to differentiate  gate-to-SD gate oxide short from non-gate oxide short  defect in real products”, Proceedings of the 30th  International Symposium for Testing and Failure  Analysis 2004.


[4] E. Wu, E. Nowak, J. Aitken, W. Abedeer, L. K. Han  and S. Lo. “Structure Dependence of Dielectric  Breakdown in Ultra-Thin Gate Oxides and Its  Relationship to Soft Breakdown Mode and Device  Failure”, IEDM 1998, pp. 187~190.


238


A Novel Method to Observe Silicide in TEM


Pan Liu


Semiconductor Manufacturing International Company, Beijing, China  Pan_Liu@smics.com


Transmission Electron Microscopy (TEM) is one of the most


powerful instruments for integrate circuit (IC) analysis as  fabrication technology shrinks into the deep sub-micron  region. A high quality TEM image with clear interface is very  important to get the correct information during failure  analysis, profile checking and thickness measurement.


In modern IC fabrication technology, metal silicide  technology in microelectronics has been a standard process to  reduce contact resistance. Many reported papers and published  books have investigated the phase of the silicide and salicide, Ti-silicide, Co-silicide Ni-silicde and such[1-5]. In fact, the  thickness of metal silicide is also an important parameter in  reducing the contact resistance, especially, the 130nm, 90nm  and beyond technology. The traditional method to measure the  thickness of silicide, however, has a dilemma as to whether to  obtain the clear interface or to get the true thickness.


In this paper, we report a novel method to improve the  interface contrast and get a true thickness by changing the  substrate single crystal contrast.


TEM contrast includes mass-thickness contrast, diffraction  contrast and phase contrast [6]. The phase contrast plays a  major role in changing the contrast of the single crystal  substrate. The electrons scatter as they are transmitted through  the silicon substrate. The atom density affects the scattering  probability. As the atom density increases, the scattering  probability also increases.,


Figure 1: Schematic illustrating the relationship between the  scattering probability and the tilting along <400> single  crystal silicon orientation.


In this paper, the substrate scattering probability is changed by  tilting the samples. Therefore, the contrast of the substrate is


changed as well. As shown in the schematic in Figure 1, the  electron transmits through six-atom-layer along (110) crystal  face; while in the right image, the electron transmits through  only three-atom-layer after tilting along <400> crystal  direction. As a result, atom layers in the right image show less  probability of scattering the transmitted electrons than those in  the left image. This is why we can acquire different image  contrast by tilting the sample along <400> crystal orientation.


The sample preparation procedure is shown in Figure 2. The  wafer is in the (001) crystal face orientation. We cut the (110) crystal face to prepare the X-section TEM samples. Polishing  and ion milling method were used to get thin TEM samples. The thickness of the observing area is less than 100nm. The  TEM samples were observed by FEI TF20 field emission  TEM.


Figure 2: Schematic illustrating the X-section TEM sample  preparation procedure..


244


Dynamic Electroluminescence Imaging as an “Optical Oscilloscope” Probe


John Hulse


Institute for Microstructural Sciences, National Research Council, Ottawa, Ontario, Canada


Keith Sarault


Department of Electrical Engineering, Carleton University, Ottawa, Ontario, Canada and MuAnalysis Inc, Ottawa, Ontario, Canada


Martine Simard-Normandin


MuAnalysis Inc, Ottawa, Ontario, Canada


Dynamic Electroluminescence Imaging (DEI) is a technique  used to observe semiconductor devices as they operate. Much  like a traditional oscilloscope, the technique delivers  waveform information that is useful for assessing the  operation of the circuits that comprise a device. It can be  thought of as a non-contact “optical oscilloscope probe”. The  technique has two major advantages over traditional electrical  oscilloscope probing. The technique is noninvasive and has a  theoretical bandwidth approaching 100 GHz. This means that  very fast signals can be observed without unduly loading or  otherwise interfering with the circuitry under test. Moreover, the characterization of signals at individual nodes along a  signal path allows problems that arise from intervening  interconnects and transmission lines to be identified. This  paper will show several examples of the radio frequency (RF) measurement capabilities of this technique that have been  demonstrated in our laboratory.


DEI is an optical technique wherein light emitted from  operating semiconductor devices is collected and time  correlated with an AC electrical signal that is exercising the  circuit. Light collection is performed with a conventional  microscope and imaged onto the photocathode of a Mepsicron  II™ imaging photomultiplier tube with control electronics  configured for single photon counting. The passage of an  electron pulse through the tube is used to generate an external  timing pulse for time correlation measurements.


The background count rate or dark count rate of the Mepsicron  II™ detector is better than 0.0001 counts per second per image  pixel. The quantum efficiency of the photocathode is generally  better than 5% throughout the visible spectrum (VIS) and well  into the near infrared (NIR). The system is capable of imaging  electroluminescent radiation arriving at the photocathode at a  rate of less than 1 photon per pixel every ten seconds.


Figure 1 shows the DEI measurement system information flow  topology.


Figure 1: The DEI measurement system.


McMullen et al. first described the DEI time correlated  imaging technique in 1987 [1]. This method, when applied to  logic circuitry, was further developed at IBM and given the  acronym PICA, for Picosecond Imaging Circuit Analysis. An  excellent review of this technique can be found in the fifth  edition of the Microelectronics Failure Analysis Desk  Reference [2]. More recently, an interesting technique that  sacrifices imaging capability for detector speed has been  described by Stellari et al. [3].


Three parts were tested to demonstrate the ability of the DEI  technique to non-invasively measure RF waveforms. These  were a discrete red light emitting diode (LED), a discrete  AlGaAs/GaAs HBT device, and an integrated AlGaAs/GaAs  HBT RF module. These parts each exhibit strong  electroluminescence in the near infrared (NIR) portion of the  electromagnetic spectrum that lies within the range of  sensitivity of the Mepsicron II™ detector. Indeed, since DEI is  a photon counting technique, the light from each of these had  to be attenuated by several orders of magnitude in order to  reduce the photon arrival rate to within the bandwidth of the  time correlated photon detection system. This illustrates the  sensitivity of this detector.


245


# Dynamic Electroluminescence Imaging as an ÏOptical OscilloscopeÓ Probe


The Red LED


The LED was forward biased at 1.6 V and a 900MHz  sinusoidal signal from a 50 Ω signal generator was coupled to  it through a 0.1 µF capacitor.  The signal generator power  level was configured to deliver -15.0 dBm into a 50 ohm load.  A 10 MHz reference signal from the signal generator served as  a time standard for the measurements.


Figure 2: Electroluminescence data detected from the red  LED driven at 900 MHz. The figure shows the measured data  as dots, and the fit with a 900.88 MHz sine wave shown as a  solid line.


Figure 3: The LED electroluminescence data of Figure 2 fitted  with the modified sinusoid as discussed in the text.


Figure 2 shows electroluminescence data detected from the  red LED. The driving frequency was set at 900 MHz. A sine  wave is not a good fit to the data. The peak maxima are  sharper than a sinusoid and the data is skewed somewhat in  time. This is because the electroluminescence is proportional


to the current flowing through the diode. However, the diode  current is exponentially related to the bias voltage and only  approximately linear in voltage over the range of the small AC  signal superimposed on the applied DC bias. This will make  the peak current and therefore the peak electroluminescence  sharper. The skew is a result of a modulation of the PN  junction capacitance by the applied AC signal.


A model that better describes the time-dependence of the  electroluminescence features a 900.88 MHz sinusoid with a  small exponential pre-factor, leading to sharpening of the  electroluminescence peaks and a small sinusoidal phase shift  at the same frequency. Figure 3 shows the improved fit of the  data that this model provides.


The AlGaAs/GaAs HBT


Figure 4 shows the measured DEI image data of the HBT. The  device was biased in the linear region of operation with the  collector at 0.0 V, the base at -1.0 V and the emitter at -4.0 V  through a 1 kΩ resistor. Again, a sinusoidal signal at -15.0  dBm into 50 Ω was coupled to the base through a 0.1 µF  capacitor. A 10 MHz reference signal from the signal  generator served as a time standard.


Figure 4: The DEI image of the AlGaAs/GaAs HBT.


The detected electroluminescence from the HBT was much  easier to interpret, as it showed the same waveform  characteristics as the driving signal. The HBT response is  linear in this case. This is advantageous, as it means that the  electroluminescence from such devices embedded in circuitry  can reveal the characteristics of the signal passing through the  device exactly.


246


Figure 5: The AlGaAs/GaAs HBT being driven at 2.00 GHz. The figure shows the measured data as dots and the fit with a


2.0006 GHz sine wave shown as a solid line.


The RF Module


The RF module was a two metal layer AlGaAs/GaAs HBT  high power differential distributed amplifier that has been  described by Wong et al. [4]. This part was not operating as  expected. The failure mode of the device under test (DUT) was low output gain. Figure 6 shows a simplified schematic of  the output buffer. The transistors identified as M3 through M6  are in fact lumped transistors. The circuit consists of a  differential input gain stage (M1, M2) followed by an emitter  follower buffer stage (M3, M4) and finally an output  differential gain stage (M5, M6). Depending on whether a  logic ‘1’ or a logic ‘0’ is present at the input, the two  differential stages will switch completely. Thus current will  only flow through one side of the differential pair.


Figure 6: Simplified schematic of the high power RF  differential distributed amplifier.


Since the device contained only two metal layers, front side  imaging was possible. Had more metal layers been present  backside imaging would have been preferred. The DUT was  exercised continuously with the output of an 8:1 differential  serializer driven at 4GHz with a 01h parallel input bit pattern. This input will produce a 500MHz pulse train with each pulse  250ps wide. It was necessary to inject the data continuously,


since the photon image and time signature of the DUT must  overcome the noise floor of the photon detector and the timing  circuitry respectively.


Input Differential Gain Stage


Figure 7 shows the luminescence of transistors M1 and M2. Using a Lorentzian curve fit to estimate the peak location and  the full width at half maximum (FWHM) from the data, a  pulse period of 1.997ns with a pulse width of 247ps was  calculated for M1 and a pulse with of 246ps was calculated for  M2. Notice in particular that Figure 7 shows that full  switching occurs between M1 and M2.


Figure 7: The electroluminescence waveforms from HBT M1  and M2 of the input differential gain stage.


Emitter Follower Buffer Stage


The emitter follower stage does not fully switch on or off  depending on the input data. Rather, the base current is  modulated slightly. Figure 8 shows the electroluminescence  observed from an HBT in each of M3 and M4. The signal was  barely visible above the noise floor. Had a longer acquisition  time been chosen, the time signature of these devices would  become more apparent. A Fourier transform of the waveforms  shown confirmed that there is a significant spectral component  at 500MHz.


247


Figure 8: The electroluminescence waveforms from HBT M3  and M4 of the emitter follower buffer stage.


Figure 9: The luminescence waveforms from HBT M5 and M6  of the output differential gain stage.


Output Differential Gain Stage


Figure 9 shows the luminescence of transistors in each of M5  and M6. Once again, using a Lorentzian curve fit to estimate  the peak location and the FWHM, a pulse period of 1.998ns  with a pulse width of 245ps was observed for M5 and a pulse  width of 246ps was observed for M6. Examining the  luminescence waveforms of these devices, it can be seen that  the devices do not fully switch since the photon count never  falls below 60 counts for M5 and never rises above 115 counts


for M6. Since these devices do not fully switch, the final  output differential voltage will be smaller than desired.


DEI has thus been shown to be able to localize the failure in  this example. The measurements took very little time, and  since no physical probing was required the measurements did  not interfere in any way with the operation of the circuit.


DEI is an optical imaging technique that capitalizes on the  emission of light that occurs as current flows through  semiconductor devices. The examples above demonstrate the  ability of DEI to function as a noninvasive “optical  oscilloscope”. Without loading or otherwise disturbing the  semiconductor devices being observed, the DEI method  enables the measurement of RF waveforms as they pass  through the devices. The degradation of signals passing  through circuitry can be identified along the signal path. In  this way failures can be identified at individual devices within  the circuitry of a DUT. Problems arising as signals progress  through connections and transmission lines can also be  revealed. The importance of this last point in failure analysis is  evident, particularly during diagnosis of a functional failure.


We would like to thank Richard Dudek of NRC for help in  mounting the HBT devices.


[1] McMullen, W.G., S. Charbonneau and M.L.W. Thewalt, Rev. Sci. Instrum. 58, 1626  (1987).


[2] Vallett, D., in “Microelectronics Failure Analysis Desk  Reference, Fifth Edition”, pp. 369-77, ASM International (Materials Park, OH, 2004).


[3] Stellari, F., A. Tosi, F. Zappa and S. Cova, IEEE Trans. Instrum. Meas. 53, 163 (2004).


[4] Wong, T. Y. K., A. P. Freundorfer, B. C. Beggs and J. E. Sitch. IEEE J. Solid-State Cir. 31, 1388 (1996).


248


Thermal Imaging Product Power-up:  Metrology for Capturing Thermal Defects  on Live Units Not Visible on any other Technique


Nova Zamora, Kam Meng Chong, Ashish Gupta


Intel Technology Phils., Cavite, Philippines, Intel Technology Sdn.Bhd., Penang, Malaysia  Intel Corporation, Chandler, AZ, USA


This paper presented the recent application of die powerup in  Thermal Imaging as applied to the detection of defects causing  thermal failure on revenue products or units not being  captured using other available techniques. Simulating the  condition on an actual computer setup, the infrared (IR) camera should capture images simultaneously as the entire  bootup process is being executed by the processor, thus  revealing a series of images and thermal information on each  and every step of the startup process. This metrology gives the  failure analyst a better approach to acquire a set of  information that substantiate in the conduct of rootcause  analysis of thermal-related failure in revenue units, especially  on customer returns.  Defective units were intentionally  engineered in order to collect the thermal response data and  eventually come up with a plot of all known thermal-related  defects.


Die Power-up technique is currently being practiced on  determining thermal-related issues on test vehicles. Test chips  have  temperature sensors that made the powerup process  simple and easy. Still, there is no existing non-destructive  approach yet that can  give a good indication of  a thermal  problem on revenue units.


Known defects causing thermal problems on revenue units, such as thermal interface material (TIM) degradation, voiding, and delamination were visible in acoustics. However, other  thermal-related failures such as thermal throttling and TIM  microcracking cannot be captured non-destructively by other  available techniques.  This motivated the team to come up  with a metrology that can be used to evaluate TIM integrity on  Products Packages.


The Metrology


The setup utilizes simulation of the actual condition the  devices undergo power-up, see Figure1. It used any readily  available computer motherboard to power on the CPU. The  infrared (IR) camera captures images simultaneously as the  entire bootup process is being executed by the processor, thus  revealing series of images and thermal information on each  and every step of the startup process.


Figure 1: Power-up setup on the device and the Thermal  Imaging tool.


The surface thermal response of the integrated heat spreader (IHS) is captured as a function of time using high speed IR  camera after thermal stimulation of a package or a part. Severe  defects such as gross voiding and TIM thickness variation  should be easily captured by the setup, as shown in Figure2.


Fundamentally, this study focused on known failure  mechanisms such as TIM voiding, TIM degradation, functional failures and thermal throttling units. Thermal  throttling failures are those that heated up earlier than  expected and unable to continue the power up process.


249


# Thermal Imaging Product Power-up: Metrology for Capturing Thermal Defects on Live Units Not Visible on any other Technique


Figure 2: IR camera setup enables easy acquisition of  severe defects such as voiding and TIM thickness  variation.


Power map data shows hotspots in the device that would show  significant thermal response compared to the other spots  during power-up. Center point C is where the highest intensity  is expected the product power map illustrated the main hotspot  to be located at the die center. Two points equidistant to the  center, points A and B, were monitored as well and are  expected to respond very similarly. See Figure3.


Figure 3: Three points were chosen for thermal response  data acquisition.  Left figure is the acoustic image and the  other  is the IR image upon power-up.


IR images and thermal response data acquired from the good  and failing units were compared. Uniform heating from the  center was captured on a good unit, as shown in Figure4.


Figure 4: Expected CSAM image (left) and IR image (right) of a good unit.


Thermal response in the form of Intensity and Intensity rate   values will be obtained simultaneously during IR image  acquisition. These values are basically the numeric data that  will be used to quantitatively analyze the units.


Plotted Intensity rate values clearly illustrated the thermal  behavior of devices during initial powerup. See Figure5.


Figure 5: Plotted Intensity rates obtained at the three  chosen spots on the device. Intensity rate consistent on all  good units.


Units that triggered functional failure showed severe voiding  problem. Defects like this, however, is so severe that it was  easily captured by both Acoustics and Thermal Imaging  techniques. Refer to Figure6.  dI/dt vs. time plot shown in  Figure7 illustrated slower and flatter response.


Responses on Point C of  2 Good units coincide


Responses on Points A & B


also overlapped


• Voids captured • Gross voids captured


• TIM thickness variation  captured


CSAM Image


IR Image of IHS


Figure 6: This unit triggered functional failure due to  gross solder TIM voiding, as shown on the acoustic image  on the left. The right figure is the thermal response  Infrared image upon die powerup.


Figure 7: Plotted thermal response Intensity showed the  failing unit triggered much flatter and slower responses as  compared to the good.


Good and voided units were intentionally subjected to temp  cycle stress in order to establish the effect of degradation on  the thermal performance. Thermal response data clearly  captured the significant decline on the Intensity rate after  solder TIM was degraded, see Figure8.


Figure 8: Plotted thermal responses of unit that has  undergone Temp-cycle stress. Much flatter and slower  responses was obtained.


Acoustics is good enough to capture obvious TIM defects on  failing units. However, some marginal defective units  available appeared clean on CSAM. Apparently, there is no  other approach used to check any indication of thermal issues  other than CSAM. Thermal imaging technique was then used  to analyze thermal-throttling failures that appeared clean in  Acoustics. One example is the unit shown in Figure9.


Figure 9: CSAM image of a unit that was intentionally  built to fail thermal throttling but should appear good or  acceptable in Acoustics.


Though Acoustics did not show anything, acquired thermal  response revealed that the failing unit is thermally performing  differently compared to a good unit. Intensity rate on the  center is almost half the expected value, and the equidistant  spots are not responding similarly, refer to Figure10. These  information helped isolated the defective region in the die.


Points A,B,C of a Failing  Responses triggered on


Points A,B,C of a Good


Responses on Points


A,B,C of a Good Unit


Smaller and flatter responses  from a stressed unit


251


Figure 10: Plotted thermal responses of an intentionally  built thermal throttling unit against a good unit.


Isolated area revealed physical defect at Die-TIM interface.  See Figure11.


Figure 11: This unit triggered thermal throttling failure  but showed acceptable level of voiding on acoustic, as  shown on left figure. The right figure is the SEM image  after the failing unit has been cross-sectioned.


Defective units were intentionally built in order to collect  more thermal response data and widen the baseline.


Though a more complicated setup and tedious sample prep are  required, this metrology is very promising in predicting  thermal-related issues on failing units without resorting to  destructive failure analysis. It has demonstrated the accurate  acquisition of quantitative thermal response data on any  chosen region on the device. TIM defects that were not  obvious in Acoustics were also captured. This metrology can  be used to establish a baseline/reference to check the thermal  indication that a failing unit has a thermal-related problem.


The authors would like to acknowledge Yongmei Liu and  Arun Raman for the technical inputs and guidance during the  course of the project. Also, thanks to Thomas Paddock for his  support.


1.     Y. Liu and A. Gupta, Thermal Imaging Die Power-up, iATTJ (2004)


Response on Point C  of a Good Unit


Response on Points A & C  of  a Failing unit almost coincide


DIE


cross section


region observed


Physical defect at  Die-TIM interface. solder


252


Single Via Deprocessing Techniques to Enable Physical Analysis for  Semiconductor Process Integration


Jacob Hammett, Wentao Qin, David Theodore


Freescale Semiconductor Inc, Chandler, AZ


Modern semiconductor devices are continuing to be scaled  down and the complexity of the processes involved in  producing the devices keeps increasing, in conjunction with  this, sample preparation and analysis are increasingly  important for accurately determining the sources of defects  and failure mechanisms in terms of process integration.  This  paper will discuss ways to characterize integration-driven  defects using deprocessing techniques and cross-section  imaging to obtain 3-D views of such defects. As an example a  single-via test structure is evaluated.  Such structures are  comparatively more susceptible to process variation.


This paper will discuss the techniques used to deprocess the  single-via structure using a combination of RIE, FIB, and wet  etching to expose the single via while maintaining the  integrity of the structure.  Such techniques enable improved  understanding of the sources of defects and also provide better  insight as to where to concentrate further analysis.  A  complete view of the structure also provides insight into  process integration issues such as misalignment that are not  always apparent in a 2-D cross-section.


It is commonly seen that certain structures are difficult to  represent with a 2-D cross-section.  This is particularly true  for single via test structures.  It is difficult to convey to  customers the true failure mechanism without a 3-D view of  the structure and the defect.  This was particularly true in the  case of a recent defect which resulted in high via resistance  due to an integration issue related to but not solely caused by  via misalignment.  There are a number of cases where high via  resistance have been investigated but via misalignment has not  been documented [1,2,3,4,5].  The direction of the  misalignment was unknown until after the via was already  cross-sectioned.  This uncertainty in direction of misalignment  along with the advantages of viewing the defect in 3-D led to  the development of a deprocessing scheme which would  enable such analysis.  The deprocessing however was not  simple since the structure consisted of an isolated via that  would fall apart during normal deprocessing steps such as


blanket wet etch or RIE.  A pin point deprocessing technique  was required to expose the via but keep the structure intact.


In order to deprocess the structure while keeping the singlevia intact, the first step was to remove the overlying high  stress passivation and TiN films by normal RIE processing  using a CH4 and O2 [6].  The removal of these films gave the  top metal 3 structure a better chance of surviving further  processing due to the removal of high stresses that these films  exert on the metal line.  The structure was then crosssectioned utilizing a micro-cleave and a die saw along  perpendicular directions (as shown in Fig. 1) to isolate the  single via.


Figure 1: Single Via Test Structure


The single via was now partially isolated.  FIB processing was  next performed to further isolate the via from the surrounding  ILD layers.  This process was carried out in a dual beam FIB  that allowed for precise milling of remaining ILD areas.  The  shaded regions in Fig. 2 between the via and both the cleaved  edge and the sawn edge were first removed.  This was  followed by an in-situ cut between the remaining metal 2 and  metal 3 line.  The resulting structure is shown in Fig. 3.


Via Location


Micro Cleave  Direction


and Location


Die Saw Direction  and Location


253


# Single Via Deprocessing Techniques to Enable Physical Analysis for Semiconductor Process Integration


Figure 2: Shaded Areas Removed by FIB


Figure 3: SEM Image of FIB prepared Structure


The single via structure was now in a state where only the ILD  stack directly beneath Metal 3 and the ILD stack directly  above Metal 2 were left intact.  To remove these layers a 1:1:1  solution of acetic acid, ammonium fluoride, and DI water was  used to remove the remaining ILD.  The sample was etched  for 6 minutes in the solution then dried thoroughly with  nitrogen.  This process removed the ILD in close proximity to  the via and allowed for viewing in 3-D but left enough ILD  around and beneath the structure to enable the structure to stay  intact.  The now completely isolated via was imaged to view  the single via in 3-D.   This particular via was chosen since it  exhibited the misalignment and a corresponding defect.


Figures 4-7 show SEM images that enable viewing of the  structure in 3-D.  The direction of the misalignment is visible  and the defect is found to extend from the bottom of the via  into the metal line.  The 3-D display carries more information  than the regular 2-D cross-sections normally used to show the  defect.  If the defect was cross-sectioned in any direction apart  from the correct direction, the misalignment would not be  visible, due to projection effects.


Figure 4: Backscatter SEM image showing the via defect at a  45 degree angle from both Metal 2 and 3


Figure 5: Backscatter SEM Image showing the defect as  viewed parallel to Metal 2.


Figure 6: Backscatter SEM Image showing the defect as  viewed perpendicular to Metal 2.


Micro  Cleave  Edge


Die Saw  Edge


Regions  Removed


254


Figure 7: Backscatter 2-D Cross-Section of defect showing no  misalignment


The 3D information also pointed the way to for additional  analysis.  A TEM cross-section was obtained at a diagonal to  the metal 2 and metal 3 lines to better capture the  misalignment and the defect (see figures 8 and 9 below).   The  results of the TEM analysis shows the origin of the defect and  what layers are present which allowed process engineers to  partition where the defect came from.  The root cause of the  defect remains under investigation.


Figure 8: TEM Image of Single-Via and defect


Figure 9: Higher Mag Image of Defect


Techniques were developed and used to isolate and deprocess  a single via test structure to be viewed in 3-D.  The resulting  3-D view of the structure and associated defect allowed for  improved understanding of the defect and its origin.  This  understanding enabled process optimization to minimize such  defect formation


[1] Saito, S.,“A Fine Process Control On The Via Hole Of  Multilevel Interconnection,” VLSI Multilevel


Interconnection Conference, 1989. Proceedings., Sixth  International IEEE 12-13 June 1989, pp. 432 – 438


[2] Koh, Leong-Tee., “A Study on the Effect of Post Metal  Etching Polymer Strip Process on Via Resistance,”


Material Research Society Symposium., 1999, Vol 564, pp. 451-457


[3] Dai, J.Y., “High Resistance Via Induced by Marginal  Barrier Metal Step Coverage and F Diffusion,”


Proceedings of 8th IPFA 2001, Singapore, pp. 183-186


[4] Sur, H., “Investigation of High Via Resistance on a


0.25um CMOS ASIC Technology,” 24th International  Symposium for Testing and Failure Analysis, 15-19


Novermber 1998, Dallas, Texas, pp. 273-278


[5] Gajda, J.J., “Analyzing High Via Resistance,”


Semiconductor International, May 1984


[6] Abramo, M.T., “Reactive Ion Etching for Failure


Analysis Applications,” Reliability Physics Symposium, 30th Annual Proceedings., International, 31 March -2


April 1992, pp. 315-319.


255


EEPROM Failure Analysis Methodology: Can Programmed Charges Be Measured  Directly by Electrical Techniques of Scanning Probe Microscopy?


Christophe De Nardi, Romain Desplats, Philippe Perdu


CNES, French Space Agency, DCT/AQ/LE, Toulouse, France


Christophe.Denardi@stage.cnes.fr


Félix Beaudoin


Thales Security System, Toulouse, France


Jean Luc Gauffier


LNMO, INSA Génie Physique, Toulouse, France


A method to measure “on site” programmed charges in  EEPROM devices is presented. Electrical Scanning Probe  Microscopy (SPM) based techniques such as Electric Force  Microscopy (EFM) and Scanning Kelvin Probe Microscopy (SKPM) are used to directly probe floating gate potentials. Both preparation and probing methods are discussed. Sample  preparation to access floating gate/oxide interfaces at a few  nanometers distance without discharging the gate proves to be  the key problem, more than the probing technique itself. Applications are demonstrated on 128 kbit EEPROMs from  ST Microelectronics and 64 kbit EEPROMs from Atmel.


In aerospace applications, memory devices are used to perform  many applications, including storage of mission parameter data  and the communication algorithms. These components must  endure harsh qualification tests as reliability is of utmost  importance.


In the case of Electrically Erasable Programmable Read Only  Memory (EEPROM) or flash-EEPROM, several tests are  performed.  These tests are i) endurance after a high number of  write/erase cycles, ii) data retention after temperature or field  ageing, and iii) sensitivity to internal contamination (mobiles  ions coming from device top layers) or external contamination (irradiations, atmospheric particles) [1]. All of these tests lead  to a reduction of programmed charge level in EEPROM which  may alter stored data integrity.


Usually, the current leakage through the cell bit line and the  storage transistor threshold voltage are monitored. Such tests  highlight EEPROM charge fluctuation without providing a  direct measurement of the charge density.


The objective of our paper is to determine if it is possible to  directly measure the quantity of programmed charge in such


non volatile memories in order to differentiate between two  fully functional nominal bits programmed at opposite logic  levels “1b” and “0b”. The final goal is to differentiate a  nominal “0b” binary state from a degraded “0b” in a device  that had been subjected to a known reliability test.


While an accurate calculation of the exact quantity of  programmed charge is complex, we target an accuracy  between 103 and 105 electrons for standard 5V EEPROM cell, causing a 3.5V shift in its threshold voltage [2]. Of course, the  mobile nature of the charge is a problem. While programming  by Fowler-Nordheim tunneling takes advantage of mobile  charge, it is also known that sources of energy may remove  charge from the floating gate thus erasing the programmed bit  value. For example, annealing at 120°C and UV illumination  are two known techniques used to reduce charge trapping. Sample preparation can also degrade the charge integrity if  special care is not taken.


After a quick review of EEPROM programming principles, we  will describe the descrambling technique that we used to locate  physically programmed data in the memory table. Then we  will present two sample preparation methodologies: front side  and back side. Finally, using a combination of Atomic Force  Microscopy (AFM) based techniques we will tackle the task to  differentiate a “0b” state from a “1b” state.


For this study, we have selected two similar NOR EEPROMs  with standard cell structures (see Figure 1). The first EEPROM  is a 128 kbit memory from ST Microelectronics. It uses a


0.35µm CMOS technology organized in a 16 kbit by 8 bit  array and operates with power supply levels from 5.5V to


2.5V. SEM cross sectional views of this device are presented  in Figure 2 and Figure 3. The second EEPROM is a 64 kbit  memory from Atmel, using a 0.35µm CMOS technology  organized in an 8 kbit by 8 bit array with 5V power supply.


256


# EEPROM Failure Analysis Methodology: Can Programmed Charges Be Measured Directly by Electrical Techniques of Scanning Probe Microscopy?


When a read voltage between VT1 and VT2 is applied  to the CG, the erased cell remains OFF. By  convention, this corresponds to the binary logic state “0b” whereas the programmed cell is conductive in  this condition and corresponds to the logic state “1b”.


Electrical Descrambling


AFM based techniques are meant to be used on small areas  since the maximum scan size is 100µm by 100µm due to  limited piezoelectric scanner x-y displacements. Therefore, the  area of interest must be located precisely beforehand to match  the electrical address with its physical location.


Figure 1: EEPROM cell structure. It is composed of two  NMOS transistors, the access transistor (AT) and the floating  gate transistor (FGT). The FGT has two gates: a control gate (CG) at poly 2 level and a floating gate (FG) at poly 1 level.


For EEPROMs, we have chosen emission microscopy (EMMI) to locate the physical address. The principle of EMMI is to  collect near infrared photons emitted by transistors during read  or write access [4]. Since the bulk silicon is virtually  transparent to these wavelengths, photon emissions can be  collected through the backside of the die, making this  approach suited for highly integrated technologies with a high  number of metal interconnect levels. By looping a write “F0h” (11110000b) cycle to a specific address, a high Vpp (12-20V) is applied to:


Metal 1  Spacers  Silicide  Poly 2  ONO  Poly 1  Tunnel  oxide


the FGT drain through the AT while programming a “1b” (programmed conductive state) with the FGT  control gate being grounded and its source floating.


Field oxide


the FGT control gate while programming a “0b” (erased blocked state) with the FGT drain floating  and its source being grounded. [3]


Figure 2: SEM cross section parallel to word lines (poly 2) showing the FGT physical structure of the 128 kbit EEPROM. The floating gate is located at poly 1 level and is isolated by  an Oxide Nitride Oxide (ONO) film, nitride spacers, and a 10-15 nm thin gate oxide.


Photons are collected over a period of time and the physical  location of the address becomes visible (see Figure 4). By  looping the program to exercise only one byte at a time, the  whole memory array organization is deduced. Since photons  are detected only during “1b” programming, localization of  bits within a single address is also achievable.


Metal 1


Spacers


W plug


Cell drain


AT source


and FGT drain


AT


FGT


Tunnel oxide


Figure 3: SEM cross section parallel to bit lines (metal 1) showing the access transistor (AT) and the floating gate  transistor of the 128 kbit EEPROM.


In a nonvolatile device such as this, the programmed data  corresponds to the charge density accumulated in the floating  gate (FG)/tunnel oxide interface. In this paper, EEPROM  conventions proposed in [3] are used:


Figure 4: EMMI image (left) and a superimposed LSM and  EMMI image (right) obtained from the back side of the die  with an HgCdTe camera with 10 min. integration time. The  byte address 1025d (401h) was programmed at “F0h” and  looped. Only the four most significant programmed bits at “1b” emit photons. Views are at 100X.


An erased cell has electrons stored in its FG and  presents a positive threshold voltage VT1, while a  programmed cell has no electrons in its FG and  presents a negative threshold voltage VT2.


257


Programmed charge in the EEPROM is stored at the  poly1/tunnel oxide interface. To make near field electrical  measurements, samples must be deprocessed to less than 100  nm distance from the interface. Indeed, metal coated AFM tips  must probe near the floating gates to be sensitive to electrical  charge without discharging them. Thus, two preparation  approaches where investigated:


Traditional front side layer by layer deprocessing, down to the ONO layer. Floating gate potentials will  be measured through ONO.


A relatively new and promising backside approach, by back side deprocessing to reveal the tunnel oxide  layer. Floating gate potentials will be measured  through the tunnel oxide.


It must be stressed that during the whole sample preparation  process, Reactive Ion Etching (RIE) is not recommended to  avoid charging oxides and thus disturbing the original FG  potentials. SEM and AFM inspections are performed on  separate samples for the same reasons.


Before hand, samples are dropped into HNO3 fuming acid at  90°C for 4-5min to remove the plastic package [5]. This is  followed by a standard cleaning procedure.


Front Side Deprocessing


The objective of the front side approach is to prepare samples  to expose the ONO layer. This is achieved in two steps:


1- Buffered Oxide Etch (BOE = 1ml HF + 5ml NH4F) to  expose poly 2, removing all silicide,


2- Choline hydroxide [6] [7] or Tetra Methyl  Ammonium Hydroxide (TMAH) [8] [9] to remove  poly 2 and expose ONO layer.


Figure 5: SEM view after front side deprocessing down to the  ONO layer. This approach is clearly data destructive. FG are  left partially etched and no longer electrically isolated.


In our experiment, front side deprocessing was found to be  destructive to programmed charge (see Figure 5). Indeed it is  difficult to perfectly expose the ONO layer with the poly 1  gates remaining isolated. The issue comes from the first BOE  etch step. On one hand it must be long enough (10-12 min) to


completely remove the WSi2 silicide and to expose poly 2. On  the other hand, as the BOE etching time is increased, the  spacers are weakened and no longer protect poly 1. As a  consequence, some floating gates are over-etched by the  following choline (or TMAH) treatment, and the FG charge  vanishes.


Backside preparation


The backside approach is particularly promising for detection  of gate oxide and tunnel oxide holes as well as other defects  like micro-cracks [10]. The objective of our back side  approach is to prepare the sample to expose the tunnel oxide  layer. We used a procedure similar to ones developed in [8] and [10], which can be summarized as follows:


1- Epoxy gluing to an AFM sample holder,


2- Bulk silicon removal by parallel lapping,


3- Selective chemical etch of remaining silicon using  choline hydroxide or TMAH,


4- SEM inspections or electrical AFM measurements.


Step 1


First of all, we glued the sample front side to a conductive  holder in order to manipulate it during the entire process. This  is necessary since the chip thickness after preparation will be  less than 4 µm. Thus, the sample is glued to a metal AFM disk  with Allied EP110 epoxy, which was found to be resistant to  TMAH and choline hydroxide. We cured the epoxy at 120°C  for half an hour.


Step 2


The sample, now mounted on the AFM disk, is attached to the  polishing holder using wax. It is now ready to be thinned by  parallel lapping the back side of the die. A 15µm diamond film  is used to thin the sample until its thickness is around 30µm. Then, 6µm diamond slurry and 1µm diamond slurry polishes  are used in succession to create a mirror finish. Indeed, any  cracks remaining on backside surface after polishing step  would lead to non-uniformity in the chemical etch. Figure 6  shows that choline hydroxide (or TMAH) preferentially etches  silicon scratches. After the final polishing step, the sample is  cleaned with a Q-tip soaked in a mixture of DI water and soap. Its thickness is around 25µm. This can be verified by laser  reflectometry measurements. Then the sample is removed from  the polishing holder by melting the wax.


AT field   oxide


FGT field   oxide


Poly 1 FG  Source line


Step 3


To remove the remaining silicon and leave the tunnel oxide  layer untouched, a solution with a low etch rate and a strong  silicon to oxide etch selectivity is needed. Two products  commonly used in Failure Analysis were tried: Choline  hydroxide solution in water and TMAH solution in methanol. For the first etch solution, we used 50% choline hydroxide  solution in water at 90°C. According to [6], the etch rate for  bulk silicon is 400 nm/min and the etch rate for oxide is 0.08  nm/min under these conditions, so silicon to oxide selectivity  is around 5000. For the second etch solution, we used 80ml of  25% TMAH solution in methanol mixed with 20ml of  isopropanol at 85°C. According to [8], etch rate of bulk silicon


258


To conclude, the presented backside preparation methodology  allows exposure of the tunnel oxide level, leaving it perfectly  intact with the floating gates remaining isolated.


is 350nm/min and 0.1nm/min for oxide, giving a selectivity of


3500. We found that both choline hydroxide and TMAH are  suitable for the backside approach and leave the tunnel oxide  and field oxide intact on 95% of the chip surface. Immediately  before choline or TMAH etch, we recommend a 5sec BOE dip  to remove the native oxide. The sample is inspected after the  first 40min choline or TMAH treatment. Subsequent etches of  10min each are used if the silicon is not completely removed. For both solutions it usually takes between 60min and 90min  to yield a surface free of silicon (see Figure 6).


EEPROM charge measurements


The objective is to directly measure EEPROM programmed  charge at its location, i.e. at the floating gate /tunnel oxide  interface. AFM electrical mode measurement [11] seemed  promising because it is very sensitive to electrostatic  interactions and provides a nanoscale spatial resolution, especially:


Electrostatic Force Microscopy (EFM) which  measures variations of electric field gradient between  tip and sample with 45mV resolution on 100nm thin  metal lines [12], [13].


Scanning Kelvin Probe Microscopy (SKPM) which  measures sample surface potential down to 10mV  resolution [14].


Both techniques use two scans [15]. The first scan records  topography in AFM tapping mode, whereas the second scan is  achieved at a 10nm to 100nm distance above the surface in  order to detect electric field. During the second EFM scan, the  cantilever experiences mechanical oscillations induced by  piezoelectric transducers while a DC voltage is applied to the  tip and/or the sample. The SKPM second scan is performed  with no induced mechanical oscillations. An AC voltage is  applied to the cantilever tip which experiences smaller  oscillations due only to Coulomb force interactions.


Figure 6: Choline hydroxide etching progress at t=0min (top  left) t=40min (top right), t=65min (bottom left) and t=70min (bottom right). Optical views are at 2.5X.


Step 4


The high viscosity of choline hydroxide, and TMAH to a  lesser extent, created rinsing and cleaning problems. After a  long DI water rinse, we recommend successive 2min ultrasonic  baths in PRS1000, acetone, and DI water. A key point must be  stressed: silicon or choline/TMAH residues obstruct AFM  charge measurements at floating gate interfaces. Indeed, it is  known that all electrical techniques are very dependant on the  sample surface. The tunnel oxide surface must be perfectly  clean and free of screen charges. In addition, the smoother the  surface is, the better the measurements will be. Figure 7 shows  the surface after backside preparation.


Front side measurements through ONO layer


As explained in the previous section, ONO, spacers, and field  oxides between cells are deteriorated by front side  deprocessing. As a consequence, floating gates are partially  etched and no longer isolated so the programmed charges  vanishes during front side deprocessing. Therefore the  backside approach is chosen.


Backside measurements trough tunnel oxide layer


Tapping AFM, EFM, and SKPM scans are performed on the  tunnel oxide layer from the backside of the sample on both the  64 kbit and 128 kbit devices. AFM tapping measurements  demonstrated perfect FGT tunnel oxide integrity since no  holes are detected (see Figure 8 left). The SKPM image of the  tunnel oxide surface (see Figure 8 right) shows a uniform  potential proving that its surface is free of electrical  contamination (screen charges, etc.) which could interfere with  the measurement of the programmed charge lying beneath the  surface. Probing 40-50nm deep, the SKPM image (not shown) demonstrated perfect integrity of the floating gates, spacers, and field oxides.


FGT  AT


A  B  C  E


Figure 7: SEM view of the 128 kbit EEPROM tunnel oxide  layer from the backside, showing drain contacts (A), spacers (B), tunnel oxide (C), field oxide (D) and source lines (E)


259


Field  oxide  Source  line


FGT  Spacer  AT


Drain  contact


Spacer  FGT  AT


Figure 8: Backside scans of the 128 kbit memory. (Left) Tapping AFM scan of tunnel oxide layer showing backside  topography information. The thick field oxide has a bump  bevel shape. No holes are detected in gate and tunnel oxides. (Right) SKPM scan (less than 5 nm depth) showing uniform  potential of oxide surface and spacer integrity. No electric  contamination such as screen charges was detected.


Figure 9: Amplitude AFM (left) and SKPM (right) scans on  the ”FOh” (“11110000b”) programmed byte area in the 64  kbit memory. SKPM detected two charged FGT gates (bright  in white circles) and two uncharged ones (dark in black  circles) as programmed in each byte center.


The SKPM results were very encouraging. It validated that our  backside sample preparation methodology did not remove all  programmed charges. It also validated the ability of the AFM  electrical mode to measure charges “on site”. But when open  loop SKPM scans were conducted, we produced only  qualitative and relative data (see Figure 10). Indeed, it is only  by comparison of two different levels of charges appearing in  the same SKPM scan (100µm by 100µm maximum size) that  we can further localize the failure analysis.


In order to image the charge in the tunnel oxide/FGT floating  gate interfaces, we needed to find the optimal SKPM  parameters (VDC tip, VAC tip, VDC sample and lift distance) to achieve maximum electrical sensitivity. In addition, when  imaging floating gate structures directly through oxide it is a  complex problem to stabilize SKPM signals. It is different  from measuring stable passive voltage contrast on biased metal  lines as presented in [12] and [13] or biased PN junctions as  shown in [14]. Indeed, the working point has to be found  where electric interactions between tip and tunnel oxide/FG  interfaces are stable. The best way to find this working point is  to scan first along a single line crossing charged and  uncharged tunnel oxide regions then optimize the SKPM  parameters to give maximum potential contrast.


The measured difference between nominal “0b” and “1b” EEPROM programmed cells is around 450mV. Knowing that  we can achieve a resolution up to 10mV, we also hope to  distinguish nominal “0b” from degraded “0b”.


Figure 9 shows a topographic amplitude AFM scan (left) and  an electrical SKPM scan (right) demonstrating charged and  uncharged floating gates on the 64 kbit memory sample. Notice that the topography is exactly the same for both types  of gate, proving that SKPM contrast only comes from the  electrostatic charge stored in the tunnel oxide/FG interface. With the AFM tip at positive DC voltage, attractive  electrostatic forces exist between the tip and electrons stored  in the floating gates, resulting in a high potential signal. Thus, charged gates are indicated by bright regions in the SKPM  images. Conversely, while scanning uncharged gates, the  positively charged AFM tip experiences only small repulsive  forces indicated by dark regions in the SKPM images.


Figure 10: Relative SKPM measurements between charged  FGT gates (bright) and uncharged ones (dark) in the 64 kbit  memory sample. SKPM differences detected between them are ≈ 450 mV as shown.


Knowing both the data we had programmed into the table  memory (“F0h”) and the physical location of each byte address  obtained by descrambling techniques, we confirmed our  SKPM recordings.


EFM measurements did not yield conclusive results possibly  because it probes deeper and is less sensitive than SKPM. Further investigations are underway.


With the goal of measuring “on site” programmed charges in  EEPROM devices, we have presented two sample preparation  methodologies: front side and backside. Only the backside


260


approach has been shown to maintain tunnel oxide integrity  and floating gate isolation. Despite the physical integrity of the  structure, the possibility that charges may have vanished  during the preparation process was still suspected.


Using SKPM, an AFM electrical mode, charged and  uncharged gates were differentiated thus validating both the  sample backside methodology and the probing technique. The  charges were successfully detected and were proven to not  have been dispersed during sample preparation.


In the comparison of two different gate charge levels, SKPM  appears limited to comparison of nearby gates that appear  within the field of view with a sufficient difference in charge  density to be detected.


[1] Jan Van Houdt, IMEC, “Non Volatile Memory  Reliability”, Tutorial of the 11th ESREF, October 2000.


[2] S.P. Skorobogatov, University of Cambridge, “Semiinvasive attacks. A new approach to hardware security  analysis”, technical report n°630, www.cl.cam.ac.uk, April 2005, pp. 66-72.


[3] S. Zink et al, ST Microelectronics, “Mémoire flash  programmable page par page”, Brevet FR 2803080, equivalent U.S. patent 2001021958.


[4] P. Sardin et al, ST Microelectronics, “Développement de  techniques de test optique: utilisation d’outils combinés”, Proceedings of the 9th ANADEF, Jun 2004.


[5] P. Perdu et al, CNES, “A review of sample backside  preparation techniques for VLSI”, Proceedings of the 11th  ESREF, October 2000.


[6] V. Korchnoy, Intel, “Investigation of Choline Hydroxide  for Selective Silicon Etch from Gate Oxide Failure  Analysis Standpoint”, Proceedings of the 28th ISTFA, November 2002, pp. 325-331.


[7] J. Higgins, WaferTech L.L.C., “Choline OH Silicon Etch  for Gate Oxide Punch Through and Gate Oxide Integrity”, Proceedings of the 27th ISTFA, November 2001, pp. 1-4


[8] F. Zachariasse, Philips Semiconductors, “CMOS FrontEnd Investigation Over Large Areas by Deprocessing  From The Back Side”, Proceedings of the 27th ISTFA, November 2001.


[9] M. Morris et al., ON Semiconductor, “The Use of TMAH  to Etch Silicon and Expose Metal Bridging Failures”, Proceedings of the 26Th ISTFA, November 2000, pp. 231-234.


[10] K. Upadhyaya et al., Intel, “Backside Imaging and AFM  Profiling of Tunnel Oxide, Poly 1, ONO and Poly 2  Layers on Flash Devices”, Proceedings of the 29th ISTFA, November 2003, pp. 447-451.


[11] A.N. Erickson, Multiprobe Inc., “The Role of the Atomic  Force Microscope in Failure and Yield Analysis”, Seminar slides of the 27th ISTFA, November 2001.


[12] U. Behnke et al, Duisburg University, “Voltage contrast  measurements on sub-micrometer structures with an


electric force microscope based tests system”, Proceedings of the 10th ESREF, October 1999.


[13] W. Mertin et al, Duisburg University, “Contactless  Voltage and Current Contrast Imaging with Scanning  Force Microscope Based Test System”, Proceedings of  the 26th ISTFA, November 2000, pp. 533-543.


[14] A. Doukkali et al, Laboratoire de Microélectronique  ISMRA Philips (LAMIP), “Surface potential mapping of  biased pn junction with kelvin probe force microscopy: application to cross-section devices”, Applied Surface  Sciences, March 2004.


[15] F.M. Sherry  et al, Digital Instruments Veeco Metrology  Group, “Electric Force Microscopy, Surface Potential  Imaging and Surface Electrical Modification with the  Atomic Force Microscope (AFM)”, Digital Instruments  application notes AN 27, www.veeco.com


261


Stacked Polysilicon/Metal Capacitors Failure Analysis


Dat Nguyen and Frank Huang


Texas Instruments Inc., Dallas, Texas  USA  dat@ti.com and c-huang19@ti.com


Polysilicon/Metal stacked capacitors save real estate, have


good density, have less parasitic capacitance, and have small  voltage coefficients. They can be used in most designs for  noise filtering, decoupling, and switching-cap designs.


Stacked capacitors come in many varieties, which include  polysilicon, nitride, and metal stacking. Regardless of the  process methodology, accurate and effective FA techniques  are needed to isolate the bad capacitor.  The FA approach  involves the use of thermal fault isolation like Liquid Crystal


[1] (LC) to narrow down to a stack of capacitors, then  parallel lapping down to expose the capacitor plate surface  for passive voltage contrast [2] (PVC) and performing  electrical characterization.


Beside the over voltage/current condition which causes  capacitor leakage, process failure mechanisms for stacked  capacitors are related to the steps which created the stacked  capacitors.  Brief process steps in 3 layer polysilicon/metal  stacked capacitors will be discussed in the following section.


Stacked Capacitor Process


Understanding the process associated with the making of a  device is an important step in finding the failures.


The capacitors are stacked above the diffusion area.  Polysilicon layer 1 (poly1) and the diffusion layer make up the  first capacitor, C1. Polysilicon layer 2 (poly2) and poly1 are  stacked to make up the second capacitor, C2.  Finally, the  metal0 layer and poly2 are stacked to form the third capacitor (Figures 1-2).  The process of making the stacked capacitors  involves the stacking of the polysilicon and dielectric to form  the first 2 capacitors (Figure 1A).  After the polysilicon was  stacked and patterned, contact windows are opened (Figure  1B). A layer of Platinum Silicide liner is then deposited across  the whole stack (Figure 1C). Then the metal0 plate is patterned  to make up the final and third stacked capacitor layer (Figure  1D).


A.


B.


C.


D.


Figure 1: Cross section view of triple stacked capacitors. A. shows diffusion, poly1, and poly2 stack. B. shows contact open  for liner deposition. C. shows the line deposition. D. shows  metal0 stacked onto poly2.


Poly1


Poly2


Dielectric


Si-Diffusion


Metal0 Dielectric


PtSi


Contact


Pt Liner


262


# Stacked Polysilicon/Metal Capacitors Failure Analysis


After the stacking of the capacitors, the capacitors are  connected in parallel to form a single capacitor as shown in  Figures 2-3.  From the top down image, poly2 plate is  connected to diffusion plate, and poly1 plate is connected to  metal0 plate.  The connection forms parallel capacitors with a  single capacitor value (Ct) that can be derived by adding these  3 capacitors (Figure 3).  By stacking capacitors a much larger  capacitor can be formed.


Figure 2: Complete top view of a stacked capacitor. Each  plate is labeled Diff, Poly1, and Poly2.  C1 is between poly1  and Diff, C2 is between poly2 and poly1, and C3 is between  metal0 and poly2. Metal1 is used to connect Poly2 plate to  diffusion plate and metal0 plate to poly1 plate.


Figure 3: Schematic of stacked capacitors.  The schematic  from the left is the exact arrangement as shown in Figure 2, and the schematic from the right is the simplified schematic:  C1 + C2 + C3 = Ct


Failure Analysis on stacked capacitors


For mixed signal devices, stacked capacitors are extremely  useful in capacitor coupling, and noise filtering.  Capacitors  are stacked, and placed in parallel. Because of the nature of  capacitor electrical characteristics and their use, capacitors are  often found to occupy large real estate, and located under large  power metal buses.  For poly/metal stacked capacitors, metal  coverage of capacitors hinders FA.  Also, when a stacked


capacitor fails, it is very challenging to isolate the failed  capacitor within the stack.


Because shorting of capacitors results in excessive leakage in  the circuit of interest, hotspot detection methods such as LC, TIVA [3], OBIRCH [4] etc. are commonly used. However, to identify a failed capacitor within the stack, passive voltage  contrast (PVC) was found to be most effective.  PVC can be  done using Scanning Electron Microscope (SEM) or Focus  Ion Beam (FIB). During PVC, any conductive material with  an electron path to diffusion will appear as bright.  On the  other hand, any conductive material or non-conductive  material without a path to diffusion will appear as dark.  As a  result, a capacitor with a path connection to diffusion will  appear as bright.


From Figure 2, at metal1 level with poly2 plate connecting to  diffusion, it can be inferred that only poly2 and any  metallization systems that connect to diffusion can be readily  seen as bright, and the rest, metal0 and poly1 capacitors, should appear as dark.  Moreover, when metal1 runners were  removed, capacitor plates within the stack became  independent and should be floating (dark contrast under  SEM/FIB). During SEM/FIB PVC inspection, since the  poly1 plate is located just above the diffusion plate, if  shorting between poly1 to diffusion occurred, poly1 plate  should have bright contrast. However, if poly1 is not shorted  to diffusion (dark contrast), in order to perform  PVC  inspection of shorting between poly2 to poly1, a thin layer of  FIB Platinum deposit is needed to tie poly1 to diffusion and  turn poly1 contrast to bright.  With poly1 appearing bright, any shorting between poly2 to poly1 will make poly2 appear  bright as well. Similarly, shorting of poly2 to diffusion using  platinum deposit should reveal whether or not metal0 plate  would appear bright due to shorting to poly2. Once the plates  become independent, beside PVC, shorting of any plate can  also be electrically verified by I/V curve tracing.


Capacitor Access


Access to the failed stacked capacitor for PVC requires  careful removal of any top layers by parallel lapping and the  remaining dielectric layer can be removed using chemical  etches. The parallel lapping should remove any top layers as  well as exposing metal1 for PVC.  After PVC at metal1, further parallel lapping or chemicals can be used to remove  metal1.  Below the metal1 layer, HF is used to further expose  the caps.


Under PVC, defective capacitors which fail due to vertical  shorting can be differentiated (Figures 4-6).


In the case shown in Figures 4-5, a defective stacked  capacitor was isolated using LC. The faulty stacked capacitor  is then revealed by parallel lapping down to metal1 for PVC  inspection (Figure 4). At this metal1 level, poly2 is still tied  to diffusion, the contrast on the left side of the picture shows  a good stacked capacitor, and the right side stacked capacitor


Metal0


Diff


C1  C2  C3


C1


C2


C3


Diff Poly2


Poly1 Metal0


Met0


Poly1  Diff


263


shows the short between all capacitors.  Metal1 and the  dielectrics were further removed to reveal all the capacitors (Figures 5-6). In each of the images in Figures 5-6, each  capacitor plate can be seen with Tungsten (W) contacts. In  Figures 5 and 6, all the metal connection system has been  removed.  The capacitors should all be floating (dark or  disconnected to diffusion).  In these figures, poly1 plate  appears as bright indicating that it is shorted to diffusion.


Electrically, with all the capacitor plates isolated, curve  tracing between the plates by probing can be used to  distinguish between metal shorting and capacitor leakage (Figures 7-8).  For a metal-to-metal short, a straight I/V line  can be seen, while, typically capacitor leakage shows a break  down I/V between the capacitor plates.  A known Good  capacitor shows no break down and an open I/V (a  horizontal line along the V axis).


Once a leakage was identified between the capacitor plates, the upper plate can be removed by the combination of  parallel lapping and/or chemicals to reveal the leakage site.  However, if there is a capacitor-capacitor short within a  stack as shown in Figures 4-6, the short can not be identified  from the SEM inspection.


Since the capacitors within the stack shared the same  Platinum liner, Platinum (Pt) liner removal is applied to  prove whether or not the short was due to un-etched Pt  residue (Figure 9).


Figure 4: FIB image of parallel lapping down to metal1 for  PVC. This metal1 level is 1 level above the stacked  poly/metal0 capacitor. Dark contrast (float) means the  capacitor is not connected to diffusion.  Bright contrast  indicates a short to diffusion.


Figure 5: SEM image of parallel lapping down to remove  metal1 for PVC. Bright contrast indicates electrical path to  diffusion.


Figure 6: SEM image after dielectric was removed to reveal  the stacked capacitor for PVC. Bright contrast shows short  between poly1 plate and diffusion plate.


Figure 7: Capacitor leakage between capacitor plates. Electrical characterization of the capacitor by I/V curve trace  of capacitor vs diffusion.


264


Figure 8: Capacitor resistive short, (metal to metal short). Electrical characterization of capacitor by I/V curve trace of  between capacitors.


Figure 9: SEM PVC of stacked caps. In this figure, the sample  has been subjected to Platinum etches, and stacked cap C05R, as shown in Figure 6, is no longer shorted to diffusion. All  capacitor plates appear as dark.


Poly/metal stacked capacitors present challenges in terms of  capacitor access and defect localization. The challenge of  access can be overcome using parallel lapping to expose the  contact and using chemicals to remove the dielectric.  As for  defect localization, LC or thermal localization (also  OBIRCH/TIVA) and PVC are used. PVC was found to be  effective in terms of finding the bad stacked capacitor and a  bad capacitor within the stack.  Internal probing between the  capacitors within a stack allowed the differentiation between  capacitor leakage and capacitor-capacitor shorting.  For  capacitor leakage, the defect can be identified by parallel  lapping to remove the upper capacitor plate.  For capacitorcapacitor short, if there is no visual defect seen, Pt chemical  etch can be applied for PVC inspection.


[1] S. Khandekar and K.S Wills, Microelectronic Failure  Analysis Desk Reference, 4th Edition, pp. 171-174 (1999).


[2] J. Colvin, “A New Technique to Rapidly Identify Gate  Oxide Leakage in Field Effect Semiconductors Using a  Scanning Electron Microscope”, ISTFA’s Proceedings, pp. 331 (1990).


[3] Edward I. Cole Jr., Microelectronic Failure Analysis Desk  Reference, 4th Edition, pp. 133, Electronic Device Failure  Analysis Society (1999)


[4]   K. Nikawa and S. Tozaki, ISTFA’s Proceedings, pp. 303-310 (1993).


[5]  E.I. Cole Jr., P. Tangyunyong, and D.L. Barton, IRPS


Proceedings, pp. 129-136 (1998).


265


The Microstructure Evolution of Corrosion Phenomenon on Aluminum Bond  Pads


Jian-Shing Luo, Hui-Min Lo and Jeremy D. Russell


Physical Failure Analysis Department, Inotera Memories, Inc. Taoyuan Taiwan, Republic of China


Integrated circuit bond pads are strongly affected by the  aluminum surface, due to oxide, and residual contaminants. A  thick oxide layer causes weak bonding and low conductivity, resulting in failure or reliability concerns. Generally, fluorine  residue on bond pads in the form of bonded or “free” AlF3  react with moisture to form HF which etches Al and results in  subsequent corrosion after Al bond pad opening [1]. It is  worth noting that the reaction product AlF3 is very difficult to  remove due to its lower vapor pressure. Furthermore, fluorine  ions are suspected to recycle themselves during the corrosion  process [1-2]. Therefore, fluorine residue control is very  important in bond pad formation. Auger electron spectroscopy (AES) signals come from within 5-6 nm of the surface so they  are a powerful aid for pad surface quality characterization, process troubleshooting and failure analysis. However, modern integrated circuits are covered by several µms of  polyimide around the pads as shown in Figure 1. The  polyimide causes charging which must be overcome to obtain  meaningful results. A new Ar sputter shadow method (ASSM) can efficiently reduce charging on the bond pad surrounded by  polyimide and leave an un-sputtered shadow area with unaffected pad properties at the edge for AES analysis [3]. In  addition, X-ray photoelectron spectroscopy (XPS) is also a  very popular tool for identification of the chemical state of  fluorine contamination on Al bond pads and several reports  have already been published using AES and XPS [1, 4-6].


From previous studies, it is assumed that fluorine residuals  result in the formation of a mixture of fluorine-containing  compounds, such as AlF3·xH2O, Al(OH)x, Al(OF)x,  AlF(OH)2, and AlF3, instead of effective surface passivation  by Al2O3 [1, 4]. To date, as far as the authors are aware the  detailed microstructures of fluorine corrosion on bond pads  have not been reported. In this paper, we report the  microstructure evolution of fluorine corrosion on bond pads in  a plastic box under specific environment conditions by using  transmission electron microscopy (TEM), optical microscopy (OM), focused ion beam (FIB) and scanning electron  microscopy (SEM). The elemental distributions and chemical  bonding were performed by using Gatan Image Filter (GIF)/TEM, energy dispersive X-ray (EDS)/Scanning TEM (STEM), AES and XPS, respectively.


Figure 1. Schematic shows the half cross-section structure of  bond pad with DRAM technology.


Samples used in this study were 0.11 um technology DRAM  chips with 70 × 70 um2 pads surrounded by about 5 um thick  polyimide. The nitride, oxide and TiN were dry etched with  fluorine-containing gas, such as CHF3, CH4, NF3…etc. The  samples were stored in a plastic box and exposed to an  environment with ~50% relative humidity (RH) at room  temperature (22 ℃ ) after exposing the Al pads. The  microstructures were investigated using a Tecnai TF20 field  emission gun TEM equipped with STEM, EDS and GIF  systems. The plan-view TEM samples were prepared by  conventional mechanical polishing and then ion milling. The  procedures of cross section TEM (XTEM) sample preparation  are described below. First, the defect surface is protected by  sputter coated Pt. Then in the FIB, e-beam and I-beam Pt is  successively deposited. Second, using a dicing saw cut the  chip to 30um width and 2mm long sticks and then glue the  sticks to a half copper ring with epoxy. Finally, use FEI DB  system to thin the sticks to a proper thickness for TEM  analysis. AES analysis was performed by using a PHI700  Auger Electron Spectrometer with cylindrical mirror analyser (CMA) manufactured by ULVAC-PHI, Inc. The details of  sample preparation and analysis procedure are described in  detail elsewhere [3]. Surface chemical bonding was  characterised by XPS, using a PHI Quantum 2000 Scanning  XPS microprobe system with a monochromatic Al Kα X-ray  source. The sputter raster size was approximately 1x1 mm2. The take off range and measuring spot were 45 degrees and 20  um in diameter. The F concentration of test samples is in the


266


# The Microstructure Evolution of Corrosion Phenomenon on Aluminum Bond Pads


range of 20 to 35 % on Al pad surface with C, Al, O, Ti, and  N by using XPS analysis.


In the present study, on Al pads with 35 at% fluorine residual, the corrosion phenomenon was observed after around 10 days  of storage and became more severe with time. Figure 2 shows  several flower-defects which were found on the surface of a  bond pad, by OM observation. In addition, it is apparent from  the tilted SEM image of Fig 3(b) that the defects are  embedded in the Al surface and raise above it. There are two  types of flower-defects on corroded Al pads from our  observation, similar to [1]. The main differences are the  thickness of defects and residual F concentration on Al pads. The thinner one is with lower F at% concentration, as shown  in Figure 3(b) and Figure 4.


Figure. 2 (a) An optical image shows corrosion appearance on  bond pad after few weeks. (b) Enlarged view shows flowerdefects occurrence on the surface of bond pad.


Figure 3. SEM image of corroded Al pad at (a) low  magnification (b) higher magnification and (c) the flower edge.


267


Figure 4. SEM image at corrosive Al pad of test sample with  lower F atomic % concentration.


From plan-view TEM analysis, the number and size of flowerdefects on Al pads increased markedly with time as shown in  Figure 5. After 10 days of storage in a plastic box, the  formation of flower-defects occurred on 35 at % residual  fluorine Al pads as shown in Figure 5(b). By observing the  FIB live image as many defects were sputtered through, it was  readily observed that the flower-defects did not only start to  grow at the Al grain boundaries, but also in Al grains. This  was also confirmed by plan-view TEM analysis (Figure 6). In  fact, the corrosion not only occurred in flower-defects, but  also in flower-defect free areas. Some small dark and white or  grey contrast spots are observed among flower-defect free  areas after a few days of storage and became more severe with  storage time, as shown in Figure 7. From EDS/STEM  analysis, the flower-defects are F rich on corroded Al pad, as  shown in Figure 8. This result is consistent with our AES  mapping results, as shown in Figure 9, and earlier study [3].


Figure 5. Plan-view image on corroded Al pad at (a) after Al  pad opening (b) 10 days (c) one month stored in plastic box.


Figure 6. SEM image on Al pad of test sample, with 35  atomic % fluorine residual, stored in plastic box after 10 days.


268


Figure 7. Plan-view TEM image of flower-defect free area in  corroded Al pad of test sample stored in plastic box (a) 10  days (b) 15 months.


Figure 8 (a) STEM image shows the flower-defect and (b) EDS/STEM line profiling from right-side to left-side of the  indicating red-line in 8(a).


酸


1um


Figure 9. (a) SEM image and (b) F (c) O elemental mappings  of bonding pad with higher F concentration residue.


It has been reported that the possible resources of fluorine  which caused further corrosion during storage are the volatile  by-product HF generated from the corrosion reaction [1], volatile “fluorine compounds“ from the surface of  surrounding bond pads, or wafer storage plastic box (e.g. PFA) [4]. However, the volatile fluorine re-absorbs on the Al  pad and continuously reacts with the Al pad resulting in  further corrosion. In addition, moisture also plays a very  important role in the corrosion mechanism or desorption  process, such as AlF3+3H2O Al(OH)3+3HF(volatile) [1-2]. According to the authors, it could explain the reason why  fluorine is rich in flower-defects and forms randomly. In  addition, some of the bigger flower-defects have cracks, as  shown in Figure 10. From EDS/TEM analysis, the fluorine  concentration in cracks is less than the rest of the flowerdefects. The size of grain-like structure at the centre is bigger  at the edge areas. One example is shown in Figure 11, and  there is no obvious difference in fluorine concentration  between the two areas. The cracks are suspected to be due to  stress release around the defects.


From present XTEM analysis, single and double-layer  structures were observed in flower-defect free area and  flower-defect area on corroded Al pads with longer period of  storage, respectively. One example is shown in Figure 12. The  top layer thickness is normally higher than lower layer in  bigger flower-defect for longer storage samples. From EELS  and EDS/STEM line profiling analysis, the oxygen is rich in  the lower layer and there is a homogenous fluorine  distribution for the double-layer structure, as shown in Figure


13. This result is consistent with our AES depth profile  results. The upper oxygen-rich thin layer, which is at the  interface of coating and electron beam Pt layers, should be  contamination during Pt coating in Figure 13 (b). K.-H Ernst  et al. have reported that no heterogeneities, such as  crystallites, were found on the surface of bond pads [4]. In the


269


present study, however, the corrosion layers consist of a nanocrystalline and amorphous structure for both single and double  corroded layers, according to TEM analysis. For confirmation  of the compounds in corroded layers, high resolution TEM (HRTEM), selected area electron diffraction pattern (SAED  DP) and XPS analysis were carried out. From high resolution  images analysis, the lattice spacing of small crystalline grains  is around 3.60 Å and 2.37 Å in single-layer and double-layer  structures, respectively, as shown in Figure 14. According to  the XRD pattern data, the lattice spacing 3.60 Å and 2.37 Å is  suspected to belong to AlF3 and Al, respectively [7-9]. Figure  15 shows the SAED diffraction patterns of double-layer and  single-layer structures, respectively. It reveals that the nanocrystalline region in the double-layer structure is Al, as shown  in Figure 15(a). As to the nano-crystalline region in the singlelayer structure, the lattice spacing includes 3.51, 2.26 and 1.96 Å, according to DP analysis of Figure 15 (b), which matches  closer to the XRD pattern of AF3 compared to others  candidates [8-9].


Figure 10. Plan-view TEM image shows the cracks in a big  flower-defect.


Figure 11.  Plan-view image at the (a) center (b) edge of  flower-defect.


270


Figure 12.  XTEM image of (a) FIB sample, (b) flower-defect  and (c) flower-defect free area on corrosive Al pad of test  sample stored for 15 months.


Figure 13. (a) TEM image of a part of flower-defect, showing  double-layer structure (b) oxygen GIF elemental mapping and


(c) Fluorine GIF elemental mapping in (a).


Figure 14. High resolution TEM images of apart of (a) double-layer (b) single-layer structure.


271


Figure 15. SAED diffraction patterns of (a) double-layer (b) single-layer structures.


S. Alberici et al. have reported that fluorine residuals existed  on Al as bonded or “free” AlF3 after pad opening. In this case, it is assumed the fluorine can induce, under particular  environmental conditions, gradually the formation of a  crystallite mixture of AlF3·xH2O, Al(OH)x, Al(OF)x, and  AlF(OH)2 instead of growth of a barrier to oxidation [1]. Therefore, it is reasonable to assume the nano-crystalline or  amorphous material could be AlF3 or compounds consisting of  Al, O, H and F after a period of storage time as mentioned  above. From our XPS data, Figure 16, the F 1s peaks of test  samples #1 and #2 are localized at around 686.5 and 687eV, respectively. Those peaks should be contributed by Al(OF)x (688.2-688.5 eV) and AlF3 (686.5 eV) [4]. The F 1s peaks  were slightly shifted compared to previous studies which  could be due to the mixing ratio of Al(OF)x to AlF3 [4]. Therefore, the root cause of different peak location between  the samples #1 and #2 could be related to the residual F  concentration as shown in Table 1. According to the above  results and previous study [1, 4], it is assumed that the nanocrystalline phase was Al and AlF3 in double-layer and singlelayer structures on corroded Al pads, respectively. And, the


amorphous materials properly include mainly Al(OF)x and  some Al(OH)x group compounds.


F1s Spectra


0.0000


500.0000


1000.0000


1500.0000


2000.0000


2500.0000


3000.0000


679


681


683


685


687


689


691


693


695


697


699


binding energy Sample #1


Sample #2


Figure 16. XPS spectra of F 1s on Al pad of samples 1 and 2. Table 1.  Element composition on Al bond pad surface


ID / at%


Sample #1


39.6


36.2


22.5


24.2


26.9


8.5


12.5


Ti


1.75


4.65


On Al pads with 35 atomic %, fluorine residual, corrosion was  observed after around 10 days of storage and became more  severe with time. There are two types of flower-defects on  corrosive Al pad. The main differences are the thickness of  the defects and residual F concentration. The corrosion not  only occurred in flower-defects, but also in flower-defect free  area. The fluorine is rich in flower-defects on corroded Al  pad. There are single and double-layer structures in flowerdefect free area and flower-defects on corrosive Al pads, respectively. The oxygen was rich in the lower layer for  double-layer structure. The corrosion layers consist of nanocrystalline and amorphous for both single and double-layer  structures. The nano-crystalline is AlF3 and Al suspected in  single and double -layer structures. The amorphous materials  properly include mainly Al(OF)x and some Al(OH)x group  compounds.


The authors would like to thank Virus Huang and Zack Wu  for support on sample preparation and literature search.


272


[1]   S. Alberici, D. Coulon, P. Joubin, Y. Mignot, L. Oggioni, P. Petruzza, D. Piumi, L. Zanotti, “ Surface treatment of  wire bonding metal pads”, Microelectronic Engineering, Vol. 70, (2003), pp. 558-565.


[2]   C.Y. Chang and S.M. Sze, ULSI Technology, McGrawHill International Editions (Singapore, 1996), chapter 7 “Etching” pp.359-360 and chapter 8 “Metallization” pp. 450-451.


[3]   Hui-Min Lo, Jian-Shing Luo and Jeremy D. Russell,“Ar  Sputter Shadow method (ASSM) -A novel way to  overcome the charging effect during AES bonding pad  analysis”, proceedings of “Microscopy of  Semiconducting Material 2005, Oxford, UK, Institute of  Physics Publishing – in press.


[4]   K.-H Ernst, D. Grman and R. Hauert, and E. Hollämder “Fluorine-induced Corrosion of Aluminium Microchip  Bond Pads: an XPS and AES Analysis”, Surface and  Interface Analysis, Vol. 21, (1994) pp. 691-696.


[5]   Dusan Grman, Roland Hauert, Egon Holländer, Markus  Amstutz, “Surface Analysis of Fluorine Contamination  on Microchip Bondpads“, Solid State Technology, Vol. 35(2), (1992), pp. 43-47.


[6]    J.H. Thomas, III, C.E. Bryson, III, T.R. Pampalone, “Xray Photoelectron Spectroscopy and Surface Charge  Build-up Used to Study Residue on Alumium Contacts  on Integrated Circuits”, Surface and Interface Analysis, Vol. 14, (1989) pp. 39-45.


[7]   Standard JCPDS diffraction pattern 04-0787 [Cubic Al], JCPDS-International Center for Diffraction Data, PDF-2  database, Newton Square, PA.


[8] Standard JCPDS diffraction pattern 77-0252 [Rhombohedra AlF3], JCPDS-International Center for  Diffraction Data, PDF-2 database, Newton Square, PA.


[9] Standard JCPDS diffraction pattern 44-0231 [Rhombohedra AlF3], JCPDS-International Center for  Diffraction Data, PDF-2 database, Newton Square, PA.


273


Studies on A Failure Analysis Flow of Surface Contamination, Corrosion and


Underetch on Microchip Al Bondpads in Wafer Fabrication


Hua Younan


Chartered Semiconductor Mfg Ltd


60 Woodland Industrial Park D, Street 2, Singapore 738406


A failure analysis flow is developed for surface  contamination, corrosion and underetch on microchip Al  bondpads and it is applied in wafer fabrication. SEM, EDX, Auger, FTIR, XPS and TOF-SIMS are used to identify the  root causes. The results from carbon related contamination, galvanic corrosion, fluorine-induced corrosion, passivation  underetch and Auger bondpad monitoring will be presented.  The failure analysis flow will definitely help us to select  suitable methods and tools for failure analysis of Al  bondpad-related issues, identify rapidly possible root causes  of the failures and find the eliminating solutions at both  wafer fabrication and assembly houses.


Aluminum bondpads on semiconductor microchips play an  important role in chips functionality and reliability. However, contamination, corrosion or underetch issues will  always affect the quality of microchip Al bondpads. In the  authors’ previous studies, we had made detailed discussion  on galvanic corrosion on microchip Al bondpads and  elimination solutions [1,3], discolored bondpads and  elimination solutions [2], fluorine-induced corrosion on  bondpads [4,5] and carbon-related contamination analysis  on bondpads using the fingerprints of EDX, FTIR, XPS, TOF-SIMS techniques [6] in wafer fabrication. In this  paper, we will present further study results on failure  analysis of bondpad surface contamination, corrosion and  underetch problems and recommend a failure analysis flow. We will make detailed descriptions of the materials analysis  tools in the flow with an explanation on why the analysis  tools are chosen and the order of how the analysis tools is   chosen. Moreover, some case studies for failure analysis of  bondpad related failures in wafer fabrication will also be  presented. This FA flow will definitely help us in selecting  suitable methods and tools for failure analysis of bondpadrelated issues, rapidly identify possible root causes of the  failures and find the eliminating solutions in wafer  fabrication (fab).


Identification of Bondpad Failures


It is a well-known fact that there are many types of bondpad  related failures in wafer fab. However, we can classify them  into three main groups: (a). Bondpad contamination, (b). Bondpad corrosion, and (c). Bondpad underetch. All failures  will affect the quality of Al bondpads and some of them   may result in non-stick on pads at the assembly bonding  processes.


Bondpad Contamination


Bondpad contamination can be further divided into surface  contamination and underneath contamination. In wafer fab, contamination will affect the quality of wafer, wafer yield   and device reliability. For example, bondpad quality  determines bonding and assembly yield.


In wafer fab, sources of contamination may be related to fab  processes, machines and tools, materials and chemicals, the  environment and human etc. If the failure is related to the  visible underneath contamination, cross sectional analysis is  necessary. It is difficult to get a clear and good quality of   cross sectional profile on Al bondpad using traditional  mechanical polishing technique as there is no passivation  layers on Al bondpads. Therefore, to obtain quality of cross  section on bondpad, FIB (focused ion beam) or TEM (transmission electron microscopy ) techniques are  recommended. In this paper, we will only discuss surface  contamination on Al bondpads, which may be due to wafer  fab processes, post-fab process (such as back-grinding and  Etest etc.) and wafer packaging materials.


Bondpad Corrosion


Bondpad corrosion is another main issue in wafer fab as  corrosive defects will seriously affect the quality of  bondpads and pose the problem of non-stick on pad (NSOP) during wire bonding at assembly process. For example, optical photos showed a good bonding die (Fig. 1) and a bad  bonding die with NSOP (Fig. 2).


The main corrosion issues in wafer fab are chlorine-induced  corrosion, fluorine-induced corrosion and galvanic corrosion (two-metal corrosion). The first two corrosion issues are   contamination-related but the later is not. They will be  further discussed in the next section.


Bondpad Underetch


From bondpad architecture, we can understand that the  layers on Al bondpad before bondpad opening process are: passivation Si3N4 and SiO2, TiN and Al alloy (Al-Cu, 0.5%-Si, 0.8%) layer. During bondpad opening processes, the  passivation (Si3N4 and SiO2) and TiN layers should be  etched away using the plasma process with CF4 gas or other  F-based gases so as to expose the surface of Al bondpads. However, underetch problems may occur at times due to   changing of etching parameters or the thickness of  passivation (Si3N4 and SiO2) and TiN layers. Therefore, N, O, Si and Ti may be detected by AES (Auger Electron  Spectroscopy) for some underetch cases or by EDX (energydispersive X-ray analysis) for some severe cases. Bondpad  underetch will also cause NSOP during the wire bonding  process at assembly house. Energy-Dispersive X-ray  Microanalysis (EDX) is the most commonly used tool in a


274


# Studies on A Failure Analysis Flow of Surface Contaminationg Corrosion and Underetch on Microchip Al Bondpads in Wafer Fabrication


FA lab for elemental analysis. It has been widely used to


analyze contamination, particles and thin films, etc. In this  study, EDX analysis was carried out on a Philips XL 30  FESEM (Field Emission Scanning Electron Microscope) using 5 kV electron beam accelerating voltage and 10 mm  working distance. A Lithium-drifted silicon EDX detector  was mounted at the left rear corner, resulting in an azimuth  angle of 45°. The energy scale of the spectra was calibrated  using standard Al/Cu alloy samples at their respective Kα  peaks (Al Kα line at 1.487 keV and Cu Kα line at 8.046  keV) with 5000 counts.


A Failure Analysis Flow


After years of studies, we have developed a failure analysis  flow of surface contamination, corrosion and underetch on  microchip Al bondpads in wafer fab, which is detail  described in detail in Table 2. In the past years, it has been  applied in failure analysis of bondpad-related failures in  wafer fab. For example, in the authors’ previous studies, carbon-related contamination analysis using EDX, FTIR, XPS, TOF-SIMS techniques [6], galvanic corrosion and  elimination solutions [1,3], fluorine-induced corrosion and  mechanism [4,5] and discoloration bondpad due to TiN  underetch [2] have been discussed. This failure analysis  flow has definitely help us in selecting suitable methods and  tools for failure analysis of bondpad-related issues, rapidly  identify possible root causes of the failures and find the  eliminating solutions for both wafer fab and assembly  problems.


Application Tips and Discussions


In wafer fab, it is very important to select a suitable method  and tool for failure analysis of bondpad-related issues as it  will help us to rapidly identify possible root causes of   failures and find the eliminating solutions. In this bondpad  failure analysis flow, SEM (Scanning Electron Microscopy), EDX (Energy-dispersive X-ray Microanalysis), AES (Auger  Electron Spectroscopy), FTIR (Fourier Transform Infrared  Spectroscopy), XPS/ESCA (X-ray Photoelectron  Spectroscopy/Electron Spectroscopy for Chemical Analysis) and TOF-SIMS (Time-of-flight Secondary Ion Mass  Spectrometry) techniques are involved.


In general, optical inspection is the first step to failure  analysis of bondpad failures, it will help us to understand the  whole situation and obtain information concerning the  failure such as: (a) Is there any visible  defect/particle/contamination? (b). Is the whole wafer  affected? (c). Is the affected area localized at the center or  the edge of the wafer? After optical inspection, SEM  inspection and EDX elemental analysis will be the next step  because simple and common tools might help us to solve  problems quickly. It is very common that for some of the  failures, optical and SEM/EDX analysis can draw a  conclusion. However, for some of the failure cases, we  should perform further analysis using AES, FTIR, XPS and  TOF-SIMS etc techniques as EDX is an elemental analysis


tool and it cannot provide chemical bonding information, etc.


Surface SEM/EDX Analysis


SEM/EDX is a simple, common and rapid analytical tool. Using SEM inspection, we can identify bondpad failure  mode and confirm that the failure is due to contamination, corrosion or underetch. In general, we can obtain more  surface information of the samples using a lower  acceleration voltage of SEM, but, on the other hand, using a  higher acceleration voltage SEM inspection, surface  charging problem can be reduced. Since bondpad samples  are less charging problem, a lower acceleration voltage (5kV) SEM inspection is recommend.


EDX can help us to further confirm the kind of elemental  contamination the failure is due to. However, we   understand that EDX is suitable to determine higher  concentration contamination as its lower detection limit is  relative higher, which is about 0.1-1.0%. Moreover, EDX is  not a surface analysis tool, but a volume analysis tool. Its  primary electron beam will penetrate into the sample and the  penetration depends on the electron beam acceleration  voltage. We have obtained the electron penetration data for  Al using Monte-Carlo simulation (Table 1).


Table 1 : Electron Penetration (in micron) Versus  Beam Acceleration Voltage


V 5kV 10kV 15kV 20kV 25kV 30kV  um 0.28 1.0 2.0 3.9 5.0 7.0


Therefore, in the flow, surface SEM/EDX (5KV) is  recommended so as to get more surface information and  eliminate interference elemental information from the  underneath layers.


1. Pinholes (With/Without Cu Seed and Si Dust   Galvanic Corrosion


If pinholes (with/without Cu seed) and Si dust are found  using SEM inspection, they are most likely due to galvanic  corrosion [1, 3]. Galvanic corrosion is also known as twometal corrosion. It is not contamination related, but from  electrochemical cell of Al-Cu or Al-Ti. For example, in  wafer fab, for metallization materials of bondpads, Cu is  added to Al or Al-Si to enhance the electromigration  resistance of the conductor and to control grain size of the  metal film on bondpads. However, the addition of Cu to Al  metallization will cause galvanic corrosion (Cu-Al) on Al  bondpads..


In galvanic corrosion (Al-Cu), Al3+/Al is the Anode and  Cu2+/Cu is the Cathode [1,3]:


Anode:   Al3+  + 3 e-   =  Al   Eo = - 1.662 V     (1)


Cathode:  Cu2+ +2 e-  = Cu   Eo = + 0.337 V    (2)


O2 + 2H2O + 4 e-       = 4 OH-       Eo = + 0.401 V    (3)


275


4Al + 3O2 + 6H2O = 4 Al+3 + 12OH- =4 Al(OH)3    (4)


The corrosive product is Al(OH)3, , which will be cleaned  away by DI water during cleaning processes and result in a  pinhole on Al bondpads  (Figs. 3-5). During galvanic  corrosion, the hole apparently continues until the Al2Cu  nucleus/seed is isolated electrically and physically from  aluminum matrix. Therefore, there is a nucleus centered  inside most pinholes due to galvanic corrosion. Therefore, Cu peak should be detected on the seed by the EDX, which  is shown in Figure 4.


Galvanic corrosion will be enhanced during wafer sawing  process. During DI water rinsing, the seed may be cleaned  away to form a pinhole without seed (Fig.5, SEM). Moreover, during wafer die-sawing process, Si dust may  scatter on the surface of bondpads, especially around  pinholes (Fig. 5, SEM/EDX). The pinholes and Si dust will  defiantly cause discoloration bondpads or NSOP. Therefore, it is very important to eliminate galvanic corrosion on Al   bondpads and some solutions have been discussed in  authors’ previous papers [1,3].


2. Cl  Chlorine Corrosion


Chlorine-induced corrosion is related to Cl contamination as  some Cl-based gases such as Cl2 , HCl, BCl3 are used in  wafer fab. Sometimes, it is also related to the wafer fab  environment. Chlorine from gases, chemicals and  environment will react with Al immediately and form the  corrosive product:


Al3+ + 3 Cl- = AlCl3   Water  soluble  (5)


Based on the author’s previous experiences, in wafer fab, chlorine-induced corrosion only affects metal lines and not   bondpads for the no-Cu processes as there is no Cl–related  processes during the bondpad opening process. Therefore,  Cl contamination and corrosion found on Al bondpads, it is  most likely due to environmental Cl contamination or postfab and assembly processes.


3. F Fluorine Corrosion


Fluorine-induced corrosion is related to F contamination as  some F-based chemical gases and materials such as CF4, CHF3, SF6, HF, BOE (NH4F+HF) etc are used in wafer fab. Besides this, wafer shipment packaging foam material may  also cause the F contamination and corrosion. Fluorine will  chemically react with Al and form Al fluoride compound. The chemical reaction is not immediate, but it needs some  time to grow the crystalline defects (Fig. 6). The corrosive  products may be [AlFx](x-3)-:


Al + xF- = [AlFx](x-3)- + 3e- (X=3 or 6) Water insoluble  (6)


The fluorine contamination on Al bondpads in wafer fab is  mainly from the bondpad opening processes and wafer  shipment packaging foam material. For example, CF4 gas is  used for passivation (Si3N4 and SiO2) etch or  photo-resist  strip (PRS)  using a mixture of O2  and CF4 gases.


Therefore, to prevent  F contamination on Al bondpads in  wafer fabs, EKC 265 or other chemicals are currently used  to remove F and polymer on Al bondpads in clean tech  module. In general, most of the F contamination can be  cleaned away by EKC 265 etc or other chemicals. Our  studies showed that during passivation etch and PRS  processes, certain amount of F would chemically react with  Al to form Al fluoride. Once Al fluoride  is formed on Al  bondpads, it is difficult to be removed by EKC 265 etc  chemicals or dry plasma cleaning process. This is why we  always detect a small amount of F on the normal bondpads  by AES. The mechanism and theoretical mode of F-induced  corrosion were studied in the authors’ works [4,5].


4. N, O, Si,  Si3N4 or SiO2, Severe Underetch


If N, O and Si are detected on bondpad by EDX, it is a  severe underetch case. These elements are most likely from  underetching of the passivation layers of Si3N4 and SiO2. However, we have to identify an underetch case from a  contamination case. In general, there is no visible  contamination or particles for underetch cases. Figure 7  shows a typical underetch case of the passivation layers (Si3N4 and SiO2). One can see that EDX detected high Si  peak, but SEM not showed does not show visible defects. This was a severe underetch case of passivation as EDX  detected high Si peak. Moreover, KOH testing may be used  to further confirm underetch of the passivation layers (Si3N4  and SiO2).


We do not recommend using EDX technique to determine  underetching of TiN layer as it is difficult to determine the  trace amount of TiN residue on bondpad due to its  limitations: (a). Although N Kα peak can be excited using 5  kV beam voltage energy, it may not be able to be detected  by EDX due to lower sensitivity of N element; (b). The  amount of TiN residue is too little to be detected by EDX  due to its relative-high lower limit of detection for N  element; (c). Ti Kα peak cannot be excited using 5 kV beam  accelerating voltage. To determine TiN residue using Ti Kα  peak, a higher beam acceleration voltage such as 10 kV or  higher should be used. However, another problem raised is  that the electron penetration will be about 1 um using 10 kV & 2 um using 15 kV (Table 1). In this situation, the signal  from underneath the TiW barrier metal layer will be also  detected (Fig. 8). This will result in confusion during the  identification of Ti peak. In other words, it is unable to  identify whether Ti peak is from TiN residue on surface or  from underneath the barrier metal (TiW) layer. Therefore, we strongly recommend using AES to determine TiN  residue on bondpads with Al/TiW/Ti metallization [2].


5. C Further Failure Analysis using FTIR, XPS and  TOF-SIMS


From the above discussion, one can see that for some   failures, optical and SEM/EDX analysis can draw a  conclusion. However EDX (and AES) technique can only  provide elemental information, which may not be sufficient  to identify sources of the carbon-related contamination as  there are a lot of contamination sources such as photo resist, EKC and the post-etch polymer removal chemicals, ink used  in assembly and the filter paper used in wafer shipment


276


packaging. Therefore, if EDX detect C contamination, we


are still unable to identify the root cause. Therefore, in the  FA flow, we suggest doing further failure analysis using  FTIR, XPS and TOF-SIMS techniques when necessary.


5.1 Fourier Transform Infrared Spectroscopy  (FTIR)


Fourier Transform Infrared Spectroscopy  (FTIR) technique, which can provide information on molecules and  compounds, is widely used to identify particles, polymers, organic and complex compounds. Therefore it is a very  powerful method to determine carbon-related contaminants. It is an easy way to identify the presence of certain  functional groups in a molecule, which may help us to  identify the sources of carbon contamination. In the authors’ previous paper, we had made some attempts using FTIR  fingerprints to identify the contamination source [6].


It is necessary to establish a FTIR spectra database, as this  technique is a physical comparison tool. In other words, we  should have enough initial analysis data and spectra for  reference or analyze some suspected candidates together  with the real samples. For example, if C contamination is  detected on Al bondpads of the wafer, the samples  investigated may be the contaminated wafer sample and  suspected candidate samples such as Photoresist, EKC 265, blue tape (used at the back-grinding process), filter paper (used at wafer shipment packaging) etc. Some candidate  materials from wafer fab and assembly processes were  published in the authors’ paper [6], which may be used as  reference material.


It is possible to use FTIR technique to identify the root  causes of carbon-related contamination. If the FTIR  spectrum of the contaminant matches with that of a  candidate material, this candidate material may be a possible  source. Therefore, based on the FTIR spectra, we can  identify the sources of carbon-related contamination for  some cases. For example, Figure 9 showed that FTIR  spectrum from  the contamination on bondpad matched very  well with that of the filter paper (1D2 rough paper). Therefore, we concluded that the contamination on bondpad  was most likely due to the filter paper during wafer  shipment. However, using FTIR technique, there are two  main limitations: (a). Analysis area should be larger than  machine capability, say more than 5um or above, (b). The  amount of contaminant should also be big enough to meet  the sensitivity of the machine. In other words, for some  small area/amount contamination or particle, it is difficult to  get the concluding spectra. Therefore, in few cases, when  this method does not yield unambiguous results, it is  necessary to do further analysis using other tools such as  XPS/ESCA or TOF-SIMS techniques which are capable of  providing more chemical nature of species under  investigation.


5.2 X-ray Photoelectron Spectroscopy (XPS)


XPS (or ESCA) is a versatile tool capable to provide  quantitative elemental and chemical state analysis of organic  and inorganic materials, which may help us further identify  possible root cause of carbon-related contamination. In the  FA flow, for some carbon contamination cases, if it is not  possible to identify root causes using EDX and FTIR  techniques, it is recommended that further investigation to


be done using XPS technique, especially in the cases where  the suspected materials are chemically similar. For example, the FTIR spectra of the blue tape (used in back grinding  process) and the scotch tape (used in assembly house) are  very similar. If a contamination is due to these materials, FTIR results cannot identify conclusively the source of the  contaminant.


We have made some attempts using XPS technique in  failure analysis of the carbon-related contamination and  found a fingerprint, C=O group, which can be used to  identify possible sources of carbon-related contamination. For example, XPS data was collected for a sample of the  blue tape used in wafer fab during the back-grinding  process. A curve-fit was carried out using the 1s electron  peak of carbon (C1s), the XPS result is shown in Figure 10, in which we can see that there are three chemical states   detected for carbon, C-C, C-O and C=O. The C=O peak  could be a fingerprint of XPS analysis. If the C=O  functional group is detected on the contamination, and then  this contaminant may be related to the blue tape and vice  versa. In wafer fab, we have used XPS technique by  determining the C=O peak to monitor the contamination due  to the blue tape during the wafer back-grinding process.


The fingerprint of C=O is also used in failure analysis to  determine contamination sources. For example, carbon  contamination was reported on Al bondpads, which was  suspected due to the blue tape during the wafer backgrinding process. However, XPS analysis results (Fig. 11) showed that besides C-O and C-C peaks, almost no C=O  peak was detected on the contaminant on the affected  bondpads. This result indicates that the contaminant on the  affected bondpads was not from the blue tape.


5.3 Time-of-flight Secondary Ion Mass Spectrometry (TOF-SIMS)


Sometimes, we are still unable to distinguish the sources of  contamination using EDX, FTIR and XPS fingerprints. In  such situations, another technique, TOF-SIMS may prove to  be useful. We have found that PDMS might be the  fingerprints of TOF-SIMS technique. PDMS is an  abbreviation for the organic compound  PolyDimethylSiloxane, (-CH3SiOCH3-)n, and its typical ions  in TOF-SIMS positive spectra are CH3Si+ (m/z 43), C3H9Si+ (m/z 73), C5H15OSi2+(m/z 147), C5H15O3Si3+(m/z 207), C7H21O2Si3+(m/z 221), and C7H21O4Si4+(m/z 281). Figure 12  showed the PDMS ion peaks at the positions m/z 73 and m/z


147. In failure analysis, we have used these fingerprints to  identify the root cause of carbon-related contamination [6].


6. No Abnormality Further Failure Analysis using AES


In failure analysis of Al bondpads, if optical and SEM  inspection and EDX analysis results do not show any   abnormality or visible defects, we still cannot conclude that  it is a good or normal bondpad. This is because (a). Some  contamination is not visible, especially those with underetch  problem; (b) The contamination is on very  the surface and (c). EDX technique is a volume/bulk analysis tool and not   sensitive to surface contamination. Therefore, for some  surface contamination and underetch residue/layer, EDX


277


cannot detect them. We have to use AES surface analysis


technique for further investigation.


In the FA flow, we recommend AES to be used for further  failure analysis if no abnormality is found using optical, SEM and EDX. Based on the previous experiences, using  AES, possible elements detected on the surface of a normal  Al bondpads may be C, O, F and Al and it is possible to  establish a data base as a control limit for C and F  contamination. If higher amounts of C and F are detected  and they are out of the control limits, we have to report it as  an abnormal case and find out its root causes. Of course, if  N, Si and Ti are detected on the surface of Al bondpads  using AES, it is defined as an abnormal case (refer to the  below discussion).


6.1 N, O and Si,  Si3N4 or SiO2 Underetch


In the above discussion, we know that EDX can only detect   severe underetch cases which are within its detection limit  and it cannot detect underetch cases due to its detection  limit. However, AES is a surface analysis tool and its  sensitivity for elements of N, O and Si are much higher than  that of EDX. Therefore, AES technique is recommended to  determine underetch cases. Therefore, if N, O and Si are  detected on Al bondpads, they are most likely due to  underetch of the passivation  (Si3N4 and SiO2).


6.2 N and Ti  ARC TiN Underetch


In the above section, we also discuss why we do not  recommend EDX technique to determine underetch of TiN  layer due to its limitations. Using EDX technique, we cannot  identify whether Ti peak is from the TiN residue on surface  or from underneath the barrier metal TiW layer. Therefore, AES is recommended to determine TiN residue on bondpads  with Ti/TiW/Al metallization. In failure analysis, if N and Ti  are detected on bondpads by AES, they are most likely due  to underetch of the ARC layer (TiN) [2].


6.3 C  Further Failure Analysis using XPS and TOFSIMS


Sometimes, carbon-related contamination cannot be  detected by EDX due to its detection limit and low  sensitivity. AES is one of the best tool to detect non-visible  carbon contamination. From the above discussion, we have  understood that it is normal to detect certain amount of C on  Al bondpads. However, the C level should be within the  control limit that we can establish using the production  wafers. After we can then use this control limit to control  the quality of the wafers. For example, if the concentration  of C is lower than the control limit, it is reported as a normal  bondpad. However, if higher carbon level is detected using  AES, it will be reported as an OOC (out of the control) case. In order to identify the root cause of carbon contamination, we can still use XPS and TOF-SIMS to do further analysis. However, for most of the cases, it is much difficult or not  possible to use FTIR technique to identify the sources of  invisible contamination case as the amount of contaminant  may be too little to be analyzed by FTIR.


6.4 F Fluorine Contamination


Fluorine – containing plasma, which is based on CF4 or   CHF3 gases, is used for passivation etch during bondpad  opening process in wafer fab. Thus, it is normal to detect


certain amounts of F contamination on a good Al bondpad. However, the F level should be at a lower level, which  cannot be detected by EDX due to its detection limit. It can  be detected by AES about 2-7 at%, which depends on wafer  Fab process.


Therefore, it is not recommended to use EDX to determine  the F contamination level on a normal bondpad. AES is one  of the best tools to detect the F level on a normal bondpad. We can also establish a control limit to control the quality of  the bondpads using the production wafers. In failure  analysis, if the concentration of F is lower than the control  limit, it is reported as a normal bondpad. However, if higher  level of F is detected using AES, it will be reported as an  OOC (out of the control) case.


Moreover, we should not only determine the surface F  contamination, but also the depth F contamination. For  example, after 50 A sputtering, the F level should be zero (or lower than the detection limit of AES). Therefore, for  some cases, even if the F level detected on the surface of  bondpad is lower than the control limit, it is still detected at  50A depth. In this situation, the bondpad will also be   reported as an abnormal bondpad.


6.5 O Bonding Issue


It is also very important to determine the oxygen level on Al  bondpads as Al oxide thickness will affect bondpad quality. It is very common to detect certain amount of O on a normal  bondpad as there is a very thin native Al oxide on surface of  bondpads. However, we have to control the thickness of the  Al oxide at a reasonable level. If Al oxide layer is too thick, it will result in non-stick on pad during assembly bonding  process. If Al oxide layer is too thin, it will result in  galvanic corrosion on bondpads. Therefore, we have to  determine the O level at 0A, 50A, 100A till the depth where  the pure Al is detected. For a normal bondpad, pure Al is  detected at about 150A-250A, depending on the wafer fab  process.


Therefore, in failure analysis, if the O level is found lower  than the control limit, it should be reported as a normal  bondpad. However, if higher O concentration or higher  depth is detected and out of the control limit using AES, it  should be reported as an abnormal case.


In this paper, a failure analysis flow for surface  contamination, corrosion and underetch on microchip Al  bondpads is developed. SEM, EDX, Auger, FTIR, XPS and  TOF-SIMS are used to identify the root causes. This  failure  analysis flow has been applied in wafer fabrication to  help  us in selecting suitable method and tool for failure analysis, identifying rapidly possible root causes of the failures and  finding the eliminating solutions. Detailed descriptions of  the materials analysis tools in the flow are presented with an  explanation on why the analysis tools are chosen and the  order of how the analysis tools is chosen.  The results from  carbon related contamination, galvanic corrosion, fluorineinduced corrosion, passivation underetch and Auger  bondpad monitoring have been also discussed.


278


In the FA flow, optical inspection is recommended as the


first step to failure analysis of bondpad failures so as to   understand the whole situation and obtain information  concerning the bondpad failures. SEM/EDX analysis will be  the next step as it is very common tool. For some of the  failures, SEM/EDX results can draw a conclusion. However, for some complex failure cases, further failure analysis  using AES, FTIR, XPS and TOF-SIMS etc. techniques  should be carried out so as to obtain more chemical bonding  information and identify possible root causes of the failures  on microchip Al bondpads.


The author would like to thank Mr Mo Zhiqiang from PSB, Singapore for his technical advice and contributions to this  paper. Special thanks to Dick McClelland from Philips  Semiconductors (Mentor for this paper from the Technical  Committee of ISTFA2005 Conference), for providing  technical and professional advice.


1. Hua Younan, A Study on Discolored Bondpads &


Galvanic Corrosion. The Proceedings from the 24th


International Symposium for Testing and Failure


Analysis, 15-19 Nov, Hyatt Regency, DFW-East


Tower, Dallas, Texas, USA, 269-272  (1998).


2. Hua Younan, Failure Analysis of Discolored Bondpads


in Wafer Fabrication. The Proceedings from the 25th


Analysis, 14-18 Nov, Santa Clara Convention Center,


Santa Clara, California, USA,149-159  (1999).


3. Hua Younan, E. C. Low, L. H. An and Shailesh Redkar,


Failure Analysis and Elimination of Galvanic Corrosion


on Bondpads during Wafer Sawing. The proceedings


from the 26th International Symposium for Testing and


Failure Analysis, Nov 12-16 2000, Meydenbauer


Convention Center, Bellevue (Seattle), Washington,


USA, 369-372 (2000).


4. Hua Younan, Shailesh Redkar, Lau Chi-Kwan and Mo


Zhiqiang (from PSB Corp., Singapore), A Study on


Non-Stick Aluminum Bondpads due to Fluorine


Contamination using SEM, EDX, TEM, IC, Auger,


XPS & TOF-SIMS Techniques. The proceedings from


the 28th International Symposium for Testing & Failure


Analysis (ISTFA'2002), 3-7 Nov, Phoenix Civic Plaza,


Phoenix, Arizona, USA p495-504 (2002).


5. Hua Younan, Shailesh Redkar, Ron Dickinson and Peh


Shirley, A Study on Fluorine-Induced Corrosion on


Microchip Aluminium Bondpads. The proceedings


from the 29th International Symposium for Testing &


Failure Analysis (ISTFA'2003), 2-6 Nov. 2003, Santa


Clara, California, USA, p249-255 (2003).


6. Hua Younan, Rao Ramesh, Lo Keng Foo and Mo


Zhiqiang, “Studies on Fingerprints of EDX, FTIR, XPS


and TOF-SIMS and Applications in Failure analysis of


Wafer Fabrication”. The Proceedings of the 30th


Analysis, Nov 14-18, Worcester’s Centrum Center,


Worcester, Massaehusetts, USA


279


Figure 1. Optical photo showed a good bonding die.


Figure 4 EDX detected higher Cu peak on the seed centered  the pinhole.


Figure 2. Optical photo showed a bad-bonding die with  NSOP problem.


Figure 3. SEM micrograph showed that the pinholes with  Cu seed were found on Al bondpad and they were most  likely due to galvanic corrosion.


Figure 5. SEM micrograph showed that Si dust scattered on  bondpad, especially around the pinhole, which was  introduced during wafer die-sawing process. The seed has  been cleaned away during wafer die sawing process.


Figure 6. SEM micrograph showed that fluorine reacted  with Al and formed fluoride crystalline defects on bondpad.


280


Figure 7. EDX detected high Si peak, on bondpad with


NSOP problem, which was most likely due to underetch of  passivation


Figure 8. The diagraph showed that if 10kV acceleration  voltage is used, the electron beam will penetrate into Al and  detect Ti signal from TiW layer, which will confuse with the  signal from surface TiN layer (if underetch).


Figure 9. FTIR spectra from the contamination on the  bondpad matched very well with that of the filter paper (1D2 rough paper).


Figure 10. XPS result of blue tape showed, besides C-O and  C-C groups, the C=O group  (fingerprint of XPS) was  found.


Figure 11. XPS result showed besides C-O and C-C groups, almost no C=O group was detected on the contaminated  bondpad. This indicated that the contamination on the  bondpad was not from the blue tape (Fig. 10).


Figure 12. TOF-SIMS results showed that PDMS peaks at  positions of m/z 73 & m/z 147, which could be the  fingerprint of TOF-SIMS.


10kV   5kV


TiW


281


282

